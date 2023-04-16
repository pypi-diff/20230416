# Comparing `tmp/enum_properties-1.4.0.tar.gz` & `tmp/enum_properties-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enum_properties-1.4.0.tar", max compression
+gzip compressed data, was "enum_properties-1.5.0.tar", max compression
```

## Comparing `enum_properties-1.4.0.tar` & `enum_properties-1.5.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1073 2023-02-16 05:48:06.639467 enum_properties-1.4.0/LICENSE
--rw-r--r--   0        0        0     4345 2023-04-08 09:04:38.023115 enum_properties-1.4.0/README.rst
--rw-r--r--   0        0        0    22470 2023-04-09 03:39:36.450011 enum_properties-1.4.0/enum_properties/__init__.py
--rw-r--r--   0        0        0     1878 2023-04-09 03:44:31.094954 enum_properties-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     5130 1970-01-01 00:00:00.000000 enum_properties-1.4.0/setup.py
--rw-r--r--   0        0        0     5804 1970-01-01 00:00:00.000000 enum_properties-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-02-16 05:48:06.639467 enum_properties-1.5.0/LICENSE
+-rw-r--r--   0        0        0     4345 2023-04-08 09:04:38.023115 enum_properties-1.5.0/README.rst
+-rw-r--r--   0        0        0    22832 2023-04-16 00:18:17.368670 enum_properties-1.5.0/enum_properties/__init__.py
+-rw-r--r--   0        0        0     1878 2023-04-15 23:04:18.596595 enum_properties-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5130 1970-01-01 00:00:00.000000 enum_properties-1.5.0/setup.py
+-rw-r--r--   0        0        0     5804 1970-01-01 00:00:00.000000 enum_properties-1.5.0/PKG-INFO
```

### Comparing `enum_properties-1.4.0/LICENSE` & `enum_properties-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `enum_properties-1.4.0/README.rst` & `enum_properties-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `enum_properties-1.4.0/enum_properties/__init__.py` & `enum_properties-1.5.0/enum_properties/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 try:
     from functools import cached_property
 except ImportError:  # pragma: no cover
     # todo remove when python 3.7 support is dropped
     cached_property = property  # pylint: disable=C0103
 
 
-VERSION = (1, 4, 0)
+VERSION = (1, 5, 0)
 
 __title__ = 'Enum Properties'
 __version__ = '.'.join(str(i) for i in VERSION)
 __author__ = 'Brian Kohan'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2022-2023 Brian Kohan'
 
@@ -73,29 +73,33 @@
 
 class _SProp(_Prop):
     """Symmetric property interface - private"""
 
 
 def s(  # pylint: disable=C0103
     prop_name,
-    case_fold=False
+    case_fold=False,
+    match_none=False
 ):
     """
     Add a symmetric property. Enumeration values will be coercible from this
     property's values.
 
     :param prop_name: The name of the property
     :param case_fold: If False, symmetric lookup will be
         case sensitive (default)
+    :param match_none: If True, none values will be symmetric, if False
+        (default), none values for symmetric properties will not map back to
+        the enumeration value.
     :return: a named symmetric property class
     """
     return type(
         prop_name,
         (_SProp,),
-        {'symmetric': True, 'case_fold': case_fold}
+        {'symmetric': True, 'case_fold': case_fold, 'match_none': match_none}
     )
 
 
 def p(prop_name):  # pylint: disable=C0103
     """
     Add a property of the given name to the enumeration class by inheritance.
     Properties must be specified in the order in which they appear in the
@@ -114,28 +118,28 @@
     A member specialization identifier class - private. Used to wrap
     specialized member functions and tag them with their enum values so the
     Enum classdict can identify them.
 
     :param wrapped: The wrapped member function
     :param value: The value to specialize for
     """
-    def __init__(self, wrapped, value):
+    def __init__(self, wrapped, values):
         self.wrapped = wrapped
-        self.value = value
+        self.values = values
 
 
-def specialize(value):
+def specialize(*values):
     """
     A decorator to specialize a method for a given enumeration value.
 
-    :param value: The enumeration value to specialize
+    :param values: The enumeration value(s) to specialize
     :return: A decorated specialized member method
     """
     def specialize_decorator(method):
-        return _Specialized(method, value)
+        return _Specialized(method, values)
 
     return specialize_decorator
 
 
 class SymmetricMixin:  # pylint: disable=R0903
     """
     This mixin enables symmetric Enum_ creation from properties marked
@@ -330,15 +334,16 @@
                 for attr in set(dir(class_dict)).difference(set(dir(self))):
                     setattr(self, attr, getattr(class_dict, attr))
                 for item, value in class_dict.items():
                     self[item] = value
 
             def __setitem__(self, key, value):
                 if isinstance(value, _Specialized):
-                    self._specialized_.setdefault(value.value, {})[key] = value
+                    for en_val in value.values:
+                        self._specialized_.setdefault(en_val, {})[key] = value
                 elif key in EnumPropertiesMeta.EXPECTED:
                     dict.__setitem__(self, key, value)
                 elif key in EnumPropertiesMeta.RESERVED:
                     raise ValueError(f'{key} is reserved.')
                 elif self._ep_properties_:
                     # are we an enum value? - just kick this up to parent class
                     # logic, this code runs once on load - its fine that it's
@@ -443,14 +448,16 @@
                 setattr(
                     val,
                     member_name,
                     specialization.wrapped.__get__(val)
                 )
 
         def add_sym_lookup(prop, p_val, enum_inst):
+            if p_val is None and not prop.match_none:
+                return
             if not isinstance(p_val, Hashable):
                 raise ValueError(
                     f'{cls}.{prop}:{p_val} is not hashable. Symmetrical '
                     f'enumeration properties must be hashable or a list of '
                     f'hashable values.'
                 )
             cls._ep_symmetric_map_[p_val] = enum_inst
```

### Comparing `enum_properties-1.4.0/pyproject.toml` & `enum_properties-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "enum-properties"
-version = "1.4.0"
+version = "1.5.0"
 description = "Add properties and method specializations to Python enumeration values with a simple declarative syntax."
 authors = ["Brian Kohan <bckohan@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/bckohan/enum-properties"
 homepage = "https://enum-properties.readthedocs.io"
 readme = "README.rst"
 keywords = ["enum",  "properties", "defines", "field"]
```

### Comparing `enum_properties-1.4.0/setup.py` & `enum_properties-1.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['enum_properties']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'enum-properties',
-    'version': '1.4.0',
+    'version': '1.5.0',
     'description': 'Add properties and method specializations to Python enumeration values with a simple declarative syntax.',
     'long_description': "|MIT license| |PyPI version fury.io| |PyPI pyversions| |PyPI status| |Documentation Status|\n|Code Cov| |Test Status|\n\n.. |MIT license| image:: https://img.shields.io/badge/License-MIT-blue.svg\n   :target: https://lbesson.mit-license.org/\n\n.. |PyPI version fury.io| image:: https://badge.fury.io/py/enum-properties.svg\n   :target: https://pypi.python.org/pypi/enum-properties/\n\n.. |PyPI pyversions| image:: https://img.shields.io/pypi/pyversions/enum-properties.svg\n   :target: https://pypi.python.org/pypi/enum-properties/\n\n.. |PyPI status| image:: https://img.shields.io/pypi/status/enum-properties.svg\n   :target: https://pypi.python.org/pypi/enum-properties\n\n.. |Documentation Status| image:: https://readthedocs.org/projects/enum-properties/badge/?version=latest\n   :target: http://enum-properties.readthedocs.io/?badge=latest/\n\n.. |Code Cov| image:: https://codecov.io/gh/bckohan/enum-properties/branch/main/graph/badge.svg?token=0IZOKN2DYL\n   :target: https://codecov.io/gh/bckohan/enum-properties\n\n.. |Test Status| image:: https://github.com/bckohan/enum-properties/workflows/test/badge.svg\n   :target: https://github.com/bckohan/enum-properties/actions\n\nEnum Properties\n#######################\n\nAdd properties to Python enumeration values with a simple declarative syntax.\n`Enum Properties <https://enum-properties.readthedocs.io/en/latest/>`_ is a\nlightweight extension to\n`Python's Enum class <https://docs.python.org/3/library/enum.html>`_. Example:\n\n.. code:: python\n\n    from enum_properties import EnumProperties, p\n    from enum import auto\n\n    class Color(EnumProperties, p('rgb'), p('hex')):\n\n        # name   value      rgb       hex\n        RED    = auto(), (1, 0, 0), 'ff0000'\n        GREEN  = auto(), (0, 1, 0), '00ff00'\n        BLUE   = auto(), (0, 0, 1), '0000ff'\n\n    # the named p() values in the Enum's inheritance become properties on\n    # each value, matching the order in which they are specified\n\n    Color.RED.rgb   == (1, 0, 0)\n    Color.GREEN.rgb == (0, 1, 0)\n    Color.BLUE.rgb  == (0, 0, 1)\n\n    Color.RED.hex   == 'ff0000'\n    Color.GREEN.hex == '00ff00'\n    Color.BLUE.hex  == '0000ff'\n\nProperties may also be symmetrically mapped to enumeration values, using\ns() values:\n\n.. code:: python\n\n    from enum_properties import EnumProperties, s\n    from enum import auto\n\n    class Color(EnumProperties, s('rgb'), s('hex', case_fold=True)):\n\n        RED    = auto(), (1, 0, 0), 'ff0000'\n        GREEN  = auto(), (0, 1, 0), '00ff00'\n        BLUE   = auto(), (0, 0, 1), '0000ff'\n\n    # any named s() values in the Enum's inheritance become properties on\n    # each value, and the enumeration value may be instantiated from the\n    # property's value\n\n    Color((1, 0, 0)) == Color.RED\n    Color((0, 1, 0)) == Color.GREEN\n    Color((0, 0, 1)) == Color.BLUE\n\n    Color('ff0000') == Color.RED\n    Color('FF0000') == Color.RED  # case_fold makes mapping case insensitive\n    Color('00ff00') == Color.GREEN\n    Color('00FF00') == Color.GREEN\n    Color('0000ff') == Color.BLUE\n    Color('0000FF') == Color.BLUE\n\n    Color.RED.hex == 'ff0000'\n\n\nMember functions may also be specialized to each enumeration value, using the\n@specialize decorator.\n\n.. code:: python\n\n    from enum_properties import EnumProperties, specialize\n\n    class SpecializedEnum(EnumProperties):\n\n        ONE   = 1\n        TWO   = 2\n        THREE = 3\n\n        @specialize(ONE)\n        def method(self):\n            return 'method_one()'\n\n        @specialize(TWO)\n        def method(self):\n            return 'method_two()'\n\n        @specialize(THREE)\n        def method(self):\n            return 'method_three()'\n\n    SpecializedEnum.ONE.method() == 'method_one()'\n    SpecializedEnum.TWO.method() == 'method_two()'\n    SpecializedEnum.THREE.method() == 'method_three()'\n\nPlease report bugs and discuss features on the\n`issues page <https://github.com/bckohan/enum-properties/issues>`_.\n\n`Contributions <https://github.com/bckohan/enum-properties/blob/main/CONTRIBUTING.rst>`_ are\nencouraged!\n\n`Full documentation at read the docs. <https://enum-properties.readthedocs.io/en/latest/>`_\n\nInstallation\n------------\n\n1. Clone enum-properties from GitHub_ or install a release off PyPI_ :\n\n.. code:: bash\n\n       pip install enum-properties\n\n\n.. _GitHub: http://github.com/bckohan/enum-properties\n.. _PyPI: http://pypi.python.org/pypi/enum-properties\n",
     'author': 'Brian Kohan',
     'author_email': 'bckohan@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://enum-properties.readthedocs.io',
```

### Comparing `enum_properties-1.4.0/PKG-INFO` & `enum_properties-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enum-properties
-Version: 1.4.0
+Version: 1.5.0
 Summary: Add properties and method specializations to Python enumeration values with a simple declarative syntax.
 Home-page: https://enum-properties.readthedocs.io
 License: MIT
 Keywords: enum,properties,defines,field
 Author: Brian Kohan
 Author-email: bckohan@gmail.com
 Requires-Python: >=3.7,<4.0
```

