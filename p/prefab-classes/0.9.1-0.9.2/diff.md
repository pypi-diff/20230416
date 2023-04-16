# Comparing `tmp/prefab_classes-0.9.1.tar.gz` & `tmp/prefab_classes-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefab_classes-0.9.1.tar", last modified: Thu Jan 26 16:27:05 2023, max compression
+gzip compressed data, was "prefab_classes-0.9.2.tar", last modified: Sun Apr 16 07:33:45 2023, max compression
```

## Comparing `prefab_classes-0.9.1.tar` & `prefab_classes-0.9.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 16:27:05.886217 prefab_classes-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-01-26 16:26:53.000000 prefab_classes-0.9.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-01-26 16:27:05.882217 prefab_classes-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-01-26 16:26:53.000000 prefab_classes-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-01-26 16:26:53.000000 prefab_classes-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-26 16:27:05.886217 prefab_classes-0.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 16:27:05.878217 prefab_classes-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 16:27:05.882217 prefab_classes-0.9.1/src/prefab_classes/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-01-26 16:26:53.000000 prefab_classes-0.9.1/src/prefab_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-01-26 16:26:53.000000 prefab_classes-0.9.1/src/prefab_classes/_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 16:27:05.882217 prefab_classes-0.9.1/src/prefab_classes/compiled/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-26 16:26:53.000000 prefab_classes-0.9.1/src/prefab_classes/compiled/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34380 2023-01-26 16:26:53.000000 prefab_classes-0.9.1/src/prefab_classes/compiled/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-01-26 16:26:53.000000 prefab_classes-0.9.1/src/prefab_classes/compiled/rewrite_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-01-26 16:26:53.000000 prefab_classes-0.9.1/src/prefab_classes/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 16:27:05.882217 prefab_classes-0.9.1/src/prefab_classes/dynamic/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-01-26 16:26:53.000000 prefab_classes-0.9.1/src/prefab_classes/dynamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-01-26 16:26:53.000000 prefab_classes-0.9.1/src/prefab_classes/dynamic/_attribute_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 16:27:05.882217 prefab_classes-0.9.1/src/prefab_classes/dynamic/_attribute_class_maker/
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-01-26 16:26:53.000000 prefab_classes-0.9.1/src/prefab_classes/dynamic/_attribute_class_maker/_attribute_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-01-26 16:26:53.000000 prefab_classes-0.9.1/src/prefab_classes/dynamic/_attribute_class_maker/regenerate_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-01-26 16:26:53.000000 prefab_classes-0.9.1/src/prefab_classes/dynamic/autogen.py
--rw-r--r--   0 runner    (1001) docker     (123)    10640 2023-01-26 16:26:53.000000 prefab_classes-0.9.1/src/prefab_classes/dynamic/method_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    15535 2023-01-26 16:26:53.000000 prefab_classes-0.9.1/src/prefab_classes/dynamic/prefab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-01-26 16:26:53.000000 prefab_classes-0.9.1/src/prefab_classes/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-01-26 16:26:53.000000 prefab_classes-0.9.1/src/prefab_classes/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-01-26 16:26:53.000000 prefab_classes-0.9.1/src/prefab_classes/sentinels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 16:27:05.882217 prefab_classes-0.9.1/src/prefab_classes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-01-26 16:27:05.000000 prefab_classes-0.9.1/src/prefab_classes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-01-26 16:27:05.000000 prefab_classes-0.9.1/src/prefab_classes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 16:27:05.000000 prefab_classes-0.9.1/src/prefab_classes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-26 16:27:05.000000 prefab_classes-0.9.1/src/prefab_classes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-01-26 16:27:05.000000 prefab_classes-0.9.1/src/prefab_classes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 16:27:05.882217 prefab_classes-0.9.1/src/prefab_classes_hook/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-01-26 16:26:53.000000 prefab_classes-0.9.1/src/prefab_classes_hook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-01-26 16:26:53.000000 prefab_classes-0.9.1/src/prefab_classes_hook/import_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:33:45.689636 prefab_classes-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-04-16 07:33:45.689636 prefab_classes-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 07:33:45.689636 prefab_classes-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:33:45.685636 prefab_classes-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:33:45.685636 prefab_classes-0.9.2/src/prefab_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:33:45.689636 prefab_classes-0.9.2/src/prefab_classes/compiled/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/compiled/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36138 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/compiled/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/compiled/rewrite_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:33:45.689636 prefab_classes-0.9.2/src/prefab_classes/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/dynamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/dynamic/_attribute_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:33:45.689636 prefab_classes-0.9.2/src/prefab_classes/dynamic/_attribute_class_maker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/dynamic/_attribute_class_maker/_attribute_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/dynamic/_attribute_class_maker/regenerate_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/dynamic/autogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/dynamic/method_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15521 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/dynamic/prefab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/sentinels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:33:45.685636 prefab_classes-0.9.2/src/prefab_classes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-04-16 07:33:45.000000 prefab_classes-0.9.2/src/prefab_classes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-16 07:33:45.000000 prefab_classes-0.9.2/src/prefab_classes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 07:33:45.000000 prefab_classes-0.9.2/src/prefab_classes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-16 07:33:45.000000 prefab_classes-0.9.2/src/prefab_classes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-16 07:33:45.000000 prefab_classes-0.9.2/src/prefab_classes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:33:45.689636 prefab_classes-0.9.2/src/prefab_classes_hook/
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes_hook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:33:45.689636 prefab_classes-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/tests/test_versions_match.py
```

### Comparing `prefab_classes-0.9.1/LICENSE.md` & `prefab_classes-0.9.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.1/PKG-INFO` & `prefab_classes-0.9.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefab_classes
-Version: 0.9.1
+Version: 0.9.2
 Summary: Boilerplate Generator for Classes
 Author: David C Ellis
 Project-URL: Homepage, https://github.com/davidcellis/PrefabClasses
 Project-URL: Documentation, https://prefabclasses.readthedocs.io/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -21,17 +21,22 @@
 
 # PrefabClasses - Python Class Boilerplate Generator  #
 ![PrefabClasses Test Status](https://github.com/DavidCEllis/PrefabClasses/actions/workflows/auto_test.yml/badge.svg?branch=main)
 
 Writes the class boilerplate code so you don't have to. 
 Yet another variation on attrs/dataclasses.
 
-Either written lazily when you first access the methods or
-eagerly when the class is compiled into a .pyc. Can optionally
-be made to rewrite .py source code with plain classes.
+Unlike `dataclasses` or `attrs`, `prefab_classes` has a
+focus on performance and startup time in particular.
+This includes trying to minimise the impact of importing
+the module itself.
+
+Classes are written lazily when you first access the methods or
+eagerly when the module is compiled into a .pyc or rewritten out
+to a new .py source file.
 
 The dynamic method of evaluating lazily is more flexible, while
 the compiled method is faster (once the .pyc file has been generated).
 
 For more detail look at the [documentation](https://prefabclasses.readthedocs.io).
 
 ## Usage ##
```

### Comparing `prefab_classes-0.9.1/README.md` & `prefab_classes-0.9.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 # PrefabClasses - Python Class Boilerplate Generator  #
 ![PrefabClasses Test Status](https://github.com/DavidCEllis/PrefabClasses/actions/workflows/auto_test.yml/badge.svg?branch=main)
 
 Writes the class boilerplate code so you don't have to. 
 Yet another variation on attrs/dataclasses.
 
-Either written lazily when you first access the methods or
-eagerly when the class is compiled into a .pyc. Can optionally
-be made to rewrite .py source code with plain classes.
+Unlike `dataclasses` or `attrs`, `prefab_classes` has a
+focus on performance and startup time in particular.
+This includes trying to minimise the impact of importing
+the module itself.
+
+Classes are written lazily when you first access the methods or
+eagerly when the module is compiled into a .pyc or rewritten out
+to a new .py source file.
 
 The dynamic method of evaluating lazily is more flexible, while
 the compiled method is faster (once the .pyc file has been generated).
 
 For more detail look at the [documentation](https://prefabclasses.readthedocs.io).
 
 ## Usage ##
```

### Comparing `prefab_classes-0.9.1/pyproject.toml` & `prefab_classes-0.9.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 package-dir = {"" = "src"}
 
 [tool.setuptools.dynamic]
 version = {attr = "prefab_classes.__version__"}
 
 [project.optional-dependencies]
 testing = ["pytest", "pytest-cov"]
-performance = ["attrs", "pydantic"]
+performance = ["attrs", "pydantic", "cattrs"]
 docs = ["sphinx", "myst-parser", "sphinx_rtd_theme"]
 build = ["build", "twine"]
 
 [project.urls]
 "Homepage" = "https://github.com/davidcellis/PrefabClasses"
 "Documentation" = "https://prefabclasses.readthedocs.io/"
```

### Comparing `prefab_classes-0.9.1/src/prefab_classes/_typing.py` & `prefab_classes-0.9.2/src/prefab_classes/_typing.py`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.1/src/prefab_classes/compiled/generator.py` & `prefab_classes-0.9.2/src/prefab_classes/compiled/generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,17 @@
     PREFAB_INIT_FUNC,
     DECORATOR_NAME,
     ATTRIBUTE_FUNCNAME,
     FIELDS_ATTRIBUTE,
     COMPILED_FLAG,
     COMPILE_ARGUMENT,
     CLASSVAR_NAME,
+    INTERNAL_DICT,
 )
-from ..dynamic import prefab
+from ..dynamic import prefab, attribute
 from ..exceptions import CompiledPrefabError
 
 assignment_type = "ast.AnnAssign | ast.Assign"
 prefab_essentials = {DECORATOR_NAME, ATTRIBUTE_FUNCNAME}
 
 
 def _is_classvar(item):
@@ -49,28 +50,28 @@
         if "KW_ONLY" in item.annotation.value:
             return True
 
 
 # noinspection PyArgumentList
 @prefab
 class Field:
-    name: str
-    field: assignment_type
-    default: "None | ast.expr" = None
-    default_factory: "None | ast.expr" = None
-    init_: bool = True
-    repr_: bool = True
-    kw_only: bool = False
-    exclude_field: bool = False
-    annotation: "None | ast.expr" = None
-    attribute_func: bool = False
-
-    def __prefab_post_init__(self):
-        # Special variable to indicate if a field should be made KW_ONLY
-        self._kw_only_flagged = False
+    name: str = attribute()
+    field: assignment_type = attribute()
+    default: "None | ast.expr" = attribute(default=None)
+    default_factory: "None | ast.expr" = attribute(default=None)
+    init_: bool = attribute(default=True)
+    repr_: bool = attribute(default=True)
+    compare: bool = attribute(default=True)
+    kw_only: bool = attribute(default=False)
+    exclude_field: bool = attribute(default=False)
+    annotation: "None | ast.expr" = attribute(default=None)
+    attribute_func: bool = attribute(default=False)
+
+    # Indicator that this Field should be made KW_ONLY
+    _kw_only_flagged = attribute(default=False, init=False, repr=False)
 
     @cached_property
     def default_factory_call(self):
         return ast.Call(func=self.default_factory, args=[], keywords=[])
 
     def ast_attribute(
         self,
@@ -95,14 +96,18 @@
         except KeyError:
             init_ = True
         try:
             repr_ = keys["repr"].value
         except KeyError:
             repr_ = True
         try:
+            compare = keys["compare"].value
+        except KeyError:
+            compare = True
+        try:
             kw_only = keys["kw_only"].value
         except KeyError:
             kw_only = False
         try:
             exclude_field = keys["exclude_field"].value
         except KeyError:
             exclude_field = False
@@ -125,46 +130,59 @@
         return cls(
             name=name,
             field=field,
             default=default,
             default_factory=default_factory,
             init_=init_,
             repr_=repr_,
+            compare=compare,
             kw_only=kw_only,
             exclude_field=exclude_field,
             annotation=annotation,
             attribute_func=True,
         )
 
 
-# noinspection PyAttributeOutsideInit,PyProtectedMember
+# noinspection PyProtectedMember
 @prefab
 class PrefabDetails:
-    name: str
-    node: ast.ClassDef
-    decorator: ast.Call
-    init: bool = True
-    repr: bool = True
-    eq: bool = True
-    iter: bool = False
-    match_args: bool = True
-    kw_only: bool = False
-    frozen: bool = False
-    compile_prefab: bool = False
-    compile_plain: bool = False
-    compile_fallback: bool = False
-    compile_slots: bool = False
-
-    def __prefab_post_init__(self):
-        self._resolved_fields: "None | dict[str, Field]" = None
-        self._prefab_map: "None | dict[str, 'PrefabDetails']" = None
-        self._flag_kw_only: "None | ast.AnnAssign" = None
-        self._defined_attr_names: "None | set[str]" = None
-        self._func_arguments: "None | dict[str, list[str]]" = None
-        self._resolved_func_arguments: "None | dict[str, list[str]]" = None
+    name: str = attribute()
+    node: ast.ClassDef = attribute()
+    decorator: ast.Call = attribute()
+    init: bool = attribute(default=True)
+    repr: bool = attribute(default=True)
+    eq: bool = attribute(default=True)
+    iter: bool = attribute(default=False)
+    match_args: bool = attribute(default=True)
+    kw_only: bool = attribute(default=False)
+    frozen: bool = attribute(default=False)
+    compile_prefab: bool = attribute(default=False)
+    compile_plain: bool = attribute(default=False)
+    compile_fallback: bool = attribute(default=False)
+    compile_slots: bool = attribute(default=False)
+
+    # Private internal variables
+    _resolved_fields: "None | dict[str, Field]" = attribute(
+        default=None, init=False, repr=False, compare=False
+    )
+    _prefab_map: "None | dict[str, 'PrefabDetails']" = attribute(
+        default=None, init=False, repr=False, compare=False
+    )
+    _flag_kw_only: "None | ast.AnnAssign" = attribute(
+        default=None, init=False, repr=False, compare=False
+    )
+    _defined_attr_names: "None | set[str]" = attribute(
+        default=None, init=False, repr=False, compare=False
+    )
+    _func_arguments: "None | dict[str, dict[str, None | ast.Expr]]" = attribute(
+        default=None, init=False, repr=False, compare=False
+    )
+    _resolved_func_arguments: "None | dict[str, dict[str, None | ast.Expr]]" = attribute(
+        default=None, init=False, repr=False, compare=False
+    )
 
     @property
     def field_names(self):
         return list(self.fields.keys())
 
     @property
     def field_list(self):
@@ -197,15 +215,15 @@
 
     @property
     def func_arguments(self):
         if self._func_arguments is None:
             self.gather_methods_arguments()
         return self._func_arguments
 
-    @cached_property
+    @property
     def resolved_func_arguments(self):
         if self._resolved_func_arguments is None:
             raise CompiledPrefabError(
                 "Inheritance has not yet been resolved, "
                 "call resolve_inheritance first"
             )
         return self._resolved_func_arguments
@@ -220,26 +238,26 @@
             ctx=ast.Load(),
         )
         call = ast.Call(func=attrib, args=args, keywords=keywords)
         return ast.Expr(value=call)
 
     @property
     def pre_init_call(self):
-        pre_init_args = self.resolved_func_arguments[PRE_INIT_FUNC]
+        pre_init_args = self.resolved_func_arguments[PRE_INIT_FUNC].keys()
         call_args = [
             ast.keyword(arg=attrib, value=ast.Name(id=attrib, ctx=ast.Load()))
             for attrib in pre_init_args
             if attrib != "self"
         ]
 
         return self.call_method(PRE_INIT_FUNC, keywords=call_args)
 
     @property
     def post_init_call(self):
-        post_init_args = self.resolved_func_arguments[POST_INIT_FUNC]
+        post_init_args = self.resolved_func_arguments[POST_INIT_FUNC].keys()
         call_args = [
             ast.keyword(arg=attrib, value=ast.Name(id=attrib, ctx=ast.Load()))
             for attrib in post_init_args
             if attrib != "self"
         ]
         return self.call_method(POST_INIT_FUNC, keywords=call_args)
 
@@ -360,15 +378,15 @@
         self._prefab_map = prefabs
 
         # Because this uses a python dict and dicts preserve
         # order this means if a subclass replaces a value
         # it will remain in its original place in the init function
         # but with the new default value (or with the default removed)
         new_fields: dict[str, Field] = {}
-        func_arguments: dict[str, list[str]] = {}
+        func_arguments: dict[str, dict[str, "None | ast.Expr"]] = {}
         for parent_name in reversed(self.parents):
             if parent_name not in prefabs:
                 raise CompiledPrefabError(
                     f"Compiled prefabs can only inherit from other compiled prefabs in the same module.",
                     f"{self.name} attempted to inherit from {parent_name}",
                 )
             prefabs[parent_name].resolve_inheritance(prefabs)
@@ -386,15 +404,15 @@
         if self._resolved_fields is None:
             raise CompiledPrefabError(
                 "Inheritance has not yet been resolved, "
                 "call resolve_inheritance first"
             )
         return self._resolved_fields
 
-    @cached_property
+    @property
     def compile_flag(self) -> ast.Assign:
         compiled_flag = ast.Assign(
             targets=[ast.Name(id=COMPILED_FLAG, ctx=ast.Store())],
             value=ast.Constant(value=True),
         )
         return compiled_flag
 
@@ -409,28 +427,34 @@
         assignment = ast.Assign(
             targets=[target],
             value=ast.List(elts=field_consts, ctx=ast.Load()),
         )
         return assignment
 
     @property
+    def internals_assignment(self) -> ast.Assign:
+        return ast.Assign(
+            targets=[ast.Name(id=INTERNAL_DICT, ctx=ast.Store())],
+            value=ast.Dict(keys=[], values=[]),
+        )
+
+    @property
     def slots_assignment(self) -> ast.Assign:
         """Generate slots"""
         # Don't use resolved fields as we only want fields new to this class
         slot_consts = [ast.Constant(value=name) for name in self.field_names]
         target = ast.Name(id="__slots__", ctx=ast.Store())
         assignment = ast.Assign(
             targets=[target], value=ast.Tuple(elts=slot_consts, ctx=ast.Load())
         )
 
         return assignment
 
     @property
     def match_args_assignment(self) -> ast.Assign:
-
         field_consts = [
             ast.Constant(value=field.name)
             for field in self.resolved_field_list
             if not field.exclude_field
         ]
         target = ast.Name(id="__match_args__", ctx=ast.Store())
         assignment = ast.Assign(
@@ -450,14 +474,17 @@
         kw_defaults = []
 
         body = []
 
         if PRE_INIT_FUNC in self.resolved_func_arguments:
             body.append(self.pre_init_call)
 
+        # Get post_init_args
+        post_init_args = self.resolved_func_arguments.get(POST_INIT_FUNC, {})
+
         has_default = False
 
         args.append(ast.arg(arg="self"))
 
         for field in self.resolved_field_list:
             # if init is false, just assign the default value in the body
             if field.init_ is False:
@@ -465,19 +492,23 @@
                     assignment_value = field.default
                 else:
                     assignment_value = field.default_factory_call
             else:
                 # Define the init signature
                 assignment_value = ast.Name(id=field.name, ctx=ast.Load())
                 if field.default or field.default_factory:
-                    # Include the annotation if this is an annotated value
-                    if hasattr(field, "annotation"):
-                        arg = ast.arg(arg=field.name, annotation=field.annotation)
-                    else:
-                        arg = ast.arg(arg=field.name)
+
+                    # If the argument is given to post_init with a different annotation
+                    # Copy that annotation to __init__
+                    post_annotation = post_init_args.get(field.name, None)
+
+                    arg = ast.arg(
+                        arg=field.name,
+                        annotation=post_annotation if post_annotation else field.annotation
+                    )
 
                     # For regular defaults, assign in the signature as expected
                     if field.default:
                         if field.kw_only:
                             kw_defaults.append(field.default)
                         else:
                             defaults.append(field.default)
@@ -507,28 +538,30 @@
 
                 # Simpler code for values with no defaults
                 else:
                     if has_default and not field.kw_only:
                         raise SyntaxError(
                             "non-default argument follows default argument"
                         )
-                    if field.annotation:
-                        arg = ast.arg(arg=field.name, annotation=field.annotation)
-                    else:
-                        arg = ast.arg(arg=field.name)
+
+                    # If the argument is given to post_init with a different annotation
+                    # Copy that annotation to __init__
+                    post_annotation = post_init_args.get(field.name, None)
+
+                    arg = ast.arg(
+                        arg=field.name,
+                        annotation=post_annotation if post_annotation else field.annotation
+                    )
 
                     if field.kw_only:
                         kw_defaults.append(None)
                         kwonlyargs.append(arg)
                     else:
                         args.append(arg)
 
-            # Define the body
-            post_init_args = self.resolved_func_arguments.get(POST_INIT_FUNC, [])
-
             if field.name not in post_init_args and field.exclude_field:
                 raise CompiledPrefabError(
                     f"{field.name} is an excluded attribute but is not passed to post_init"
                 )
 
             if field.name in post_init_args:
                 # Factories should still run
@@ -635,24 +668,23 @@
             returns=None,
         )
 
         return repr_func
 
     @property
     def eq_method(self) -> ast.FunctionDef:
-
         arguments = [ast.arg(arg="self"), ast.arg(arg="other")]
 
         # elt = element I guess - but this is the terminology used in the
         # tuple AST function so elt it is.
         class_elts = []
         other_elts = []
 
         for field in self.resolved_field_list:
-            if not field.exclude_field:
+            if field.compare and not field.exclude_field:
                 class_elts.append(field.ast_attribute())
                 other_elts.append(field.ast_attribute("other"))
 
         if len(class_elts) > 0:
             class_tuple = ast.Tuple(elts=class_elts, ctx=ast.Load())
             other_tuple = ast.Tuple(elts=other_elts, ctx=ast.Load())
 
@@ -696,15 +728,14 @@
         eq_func = ast.FunctionDef(
             name="__eq__", args=args, body=body, decorator_list=[], returns=None
         )
         return eq_func
 
     @property
     def iter_method(self) -> ast.FunctionDef:
-
         arguments = [ast.arg(arg="self")]
 
         body = [
             ast.Expr(value=ast.Yield(value=field.ast_attribute()))
             for field in self.resolved_field_list
             if not field.exclude_field
         ]
@@ -729,24 +760,14 @@
             decorator_list=[],
             returns=None,
         )
 
         return iter_func
 
     @property
-    def frozen_exception_import(self) -> ast.ImportFrom:
-        import_call = ast.ImportFrom(
-            module="prefab_classes.exceptions",
-            names=[ast.alias(name="FrozenPrefabError")],
-            level=0,
-        )
-
-        return import_call
-
-    @property
     def frozen_setattr_method(self) -> ast.FunctionDef:
         arguments = [ast.arg(arg="self"), ast.arg(arg="name"), ast.arg(arg="value")]
         args = ast.arguments(
             posonlyargs=[],
             args=arguments,
             kwonlyargs=[],
             kw_defaults=[],
@@ -807,21 +828,20 @@
                     )
                 ],
                 value=ast.Name(id="value", ctx=ast.Load()),
             )
             else_body = [assign]
 
         cond_body = [
-            self.frozen_exception_import,
             ast.Raise(
                 exc=ast.Call(
-                    func=ast.Name(id="FrozenPrefabError", ctx=ast.Load()),
+                    func=ast.Name(id="TypeError", ctx=ast.Load()),
                     args=[
                         ast.Constant(
-                            value="Can not set or change values on frozen instances."
+                            value=f"{self.name!r} object does not support attribute assignment"
                         )
                     ],
                     keywords=[],
                 )
             ),
         ]
 
@@ -846,21 +866,20 @@
             args=arguments,
             kwonlyargs=[],
             kw_defaults=[],
             defaults=[],
         )
 
         body = [
-            self.frozen_exception_import,
             ast.Raise(
                 exc=ast.Call(
-                    func=ast.Name(id="FrozenPrefabError", ctx=ast.Load()),
+                    func=ast.Name(id="TypeError", ctx=ast.Load()),
                     args=[
                         ast.Constant(
-                            value="Can not delete attributes on frozen instances."
+                            value=f"{self.name!r} object does not support attribute deletion"
                         )
                     ],
                     keywords=[],
                 ),
             ),
         ]
 
@@ -880,44 +899,56 @@
 
         :param prefabs: Details on all prefabs in this module - for handling inheritance
         """
 
         # Handle inheritance
         self.resolve_inheritance(prefabs)
 
-        # Remove existing fields
-        # Clear the fields from he self.node body
+        # Remove values from the body
+        # Keep the annotated values to re-insert the annotations later
+        body_annotations = []
         for item in self.field_list:
+            if isinstance(item.field, ast.AnnAssign):
+                body_annotations.append(item.field)
             self.node.body.remove(item.field)
 
         if self._flag_kw_only is not None:
+            body_annotations.append(self._flag_kw_only)
             self.node.body.remove(self._flag_kw_only)
 
         # Build body
         body = []
         if not self.compile_plain:
             body.append(self.compile_flag)
             body.append(self.fields_assignment)
+            # body.append(self.internals_assignment)
+
         if self.compile_slots and "__slots__" not in self.defined_attr_names:
             body.append(self.slots_assignment)
         if self.match_args and "__match_args__" not in self.defined_attr_names:
             body.append(self.match_args_assignment)
+
+        # Re-insert annotations
+        for item in body_annotations:
+            item.value = None
+            body.append(item)
+
         if (self.init and "__init__" not in self.defined_attr_names) or not self.init:
             body.append(self.init_method)
         if self.repr and "__repr__" not in self.defined_attr_names:
             body.append(self.repr_method)
         if self.eq and "__eq__" not in self.defined_attr_names:
             body.append(self.eq_method)
         if self.iter and "__iter__" not in self.defined_attr_names:
             body.append(self.iter_method)
         if self.frozen:
             body.append(self.frozen_setattr_method)
             body.append(self.frozen_delattr_method)
 
-        # Add functions andd definitions to the body
+        # Add functions and definitions to the body
         # Remove the @prefab decorator
         # Check if a class starts with what we assume is a docstring.
         if (
             len(self.node.body) > 0
             and isinstance(self.node.body[0], ast.Expr)
             and isinstance(self.node.body[0].value, ast.Constant)
             and isinstance(self.node.body[0].value.value, str)
@@ -928,21 +959,21 @@
             self.node.body = body + self.node.body
         self.node.decorator_list.remove(self.decorator)
 
 
 class GatherClassAttrs(ast.NodeVisitor):
     def __init__(self):
         super().__init__()
-        self.attrnames = set()
-        self.func_arguments = dict()
+        self.attrnames = set()  # set of attribute/function names - to help avoid re-assigning methods
+        self.func_arguments: dict[str, dict[str, "None | ast.Expr"]] = dict()
 
     def visit_FunctionDef(self, node: ast.FunctionDef):
         self.attrnames.add(node.name)
         args = node.args.args + node.args.kwonlyargs
-        arguments = [item.arg for item in args]
+        arguments = {item.arg: item.annotation for item in args}
         self.func_arguments[node.name] = arguments
 
     def visit_Assign(self, node: ast.Assign):
         for target in node.targets:
             self.attrnames.add(getattr(target, "id"))
 
     def visit_AnnAssign(self, node: ast.AnnAssign):
```

### Comparing `prefab_classes-0.9.1/src/prefab_classes/compiled/rewrite_source.py` & `prefab_classes-0.9.2/src/prefab_classes/compiled/rewrite_source.py`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.1/src/prefab_classes/dynamic/_attribute_class.py` & `prefab_classes-0.9.2/src/prefab_classes/dynamic/_attribute_class.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,31 +3,38 @@
 # BY regenerate_attribute.py
 # MODIFY THOSE MODULES AND RERUN regenerate_attribute.py
 
 from ..sentinels import NOTHING
 from ..exceptions import LivePrefabError
 
 class Attribute:
-    COMPILED = True
-    PREFAB_FIELDS = ['default', 'default_factory', 'init', 'repr', 'kw_only', 'exclude_field', '_type']
-    __slots__ = ('default', 'default_factory', 'init', 'repr', 'kw_only', 'exclude_field', '_type')
-    __match_args__ = ('default', 'default_factory', 'init', 'repr', 'kw_only', 'exclude_field', '_type')
+    __slots__ = ('default', 'default_factory', 'init', 'repr', 'compare', 'kw_only', 'exclude_field', '_type')
+    __match_args__ = ('default', 'default_factory', 'init', 'repr', 'compare', 'kw_only', 'exclude_field', '_type')
+    init: bool
+    repr: bool
+    compare: bool
+    kw_only: bool
+    exclude_field: bool
 
-    def __init__(self, default=NOTHING, default_factory=NOTHING, init: bool=True, repr: bool=True, kw_only: bool=False, exclude_field: bool=False):
+    def __init__(self, *, default=NOTHING, default_factory=NOTHING, init: bool=True, repr: bool=True, compare: bool=True, kw_only: bool=False, exclude_field: bool=False):
         self.__prefab_pre_init__(init=init, default=default, default_factory=default_factory, kw_only=kw_only)
         self.default = default
         self.default_factory = default_factory
         self.init = init
         self.repr = repr
+        self.compare = compare
         self.kw_only = kw_only
         self.exclude_field = exclude_field
         self._type = NOTHING
 
     def __repr__(self):
-        return f'{type(self).__qualname__}(default={self.default!r}, default_factory={self.default_factory!r}, init={self.init!r}, repr={self.repr!r}, kw_only={self.kw_only!r}, exclude_field={self.exclude_field!r})'
+        return f'{type(self).__qualname__}(default={self.default!r}, default_factory={self.default_factory!r}, init={self.init!r}, repr={self.repr!r}, compare={self.compare!r}, kw_only={self.kw_only!r}, exclude_field={self.exclude_field!r})'
+
+    def __eq__(self, other):
+        return (self.default, self.default_factory, self.init, self.repr, self.compare, self.kw_only, self.exclude_field) == (other.default, other.default_factory, other.init, other.repr, other.compare, other.kw_only, other.exclude_field) if self.__class__ == other.__class__ else NotImplemented
 
     @staticmethod
     def __prefab_pre_init__(init, default, default_factory, kw_only):
         if not init and default is NOTHING and (default_factory is NOTHING):
             raise LivePrefabError('Must provide a default value/factory if the attribute is not in init.')
         if kw_only and (not init):
             raise LivePrefabError('Attribute cannot be keyword only if it is not in init.')
```

### Comparing `prefab_classes-0.9.1/src/prefab_classes/dynamic/_attribute_class_maker/_attribute_template.py` & `prefab_classes-0.9.2/src/prefab_classes/dynamic/_attribute_class_maker/_attribute_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # COMPILE_PREFABS
+# type: ignore
 # !THIS IMPORT MUST STAY AT THE TOP!
 from prefab_classes import prefab, attribute
 
 # noinspection PyUnresolvedReferences
 from ..sentinels import NOTHING
 
 # noinspection PyUnresolvedReferences
 from ..exceptions import LivePrefabError
 
 
-@prefab(compile_prefab=True, compile_slots=True, eq=False)
+@prefab(compile_prefab=True, compile_slots=True, compile_plain=True, kw_only=True)
 class Attribute:
     # Note that the interpreted form of prefab would fail here
     # as it would interpret _NOTHING as no value provided
     # compiled prefabs do not interpret this way.
     default = attribute(default=NOTHING)
     default_factory = attribute(default=NOTHING)
     init: bool = attribute(default=True)
     repr: bool = attribute(default=True)
+    compare: bool = attribute(default=True)
     kw_only: bool = attribute(default=False)
     exclude_field: bool = attribute(default=False)
-    _type = attribute(default=NOTHING, init=False, repr=False)
+    _type = attribute(default=NOTHING, init=False, repr=False, compare=False)
 
     @staticmethod
     def __prefab_pre_init__(init, default, default_factory, kw_only):
         if not init and default is NOTHING and default_factory is NOTHING:
             raise LivePrefabError(
                 "Must provide a default value/factory "
                 "if the attribute is not in init."
```

### Comparing `prefab_classes-0.9.1/src/prefab_classes/dynamic/_attribute_class_maker/regenerate_attribute.py` & `prefab_classes-0.9.2/src/prefab_classes/dynamic/_attribute_class_maker/regenerate_attribute.py`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.1/src/prefab_classes/dynamic/autogen.py` & `prefab_classes-0.9.2/src/prefab_classes/dynamic/autogen.py`

 * *Files 15% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     Using this as a decorator indicates that the function will return a string
     which should be used to replace the function itself for that specific class.
     """
     # globs can be a given empty dict, so specifically check for None.
     globs = globs if globs is not None else {}
 
     def __get__(self, instance, cls):
-        # Include the defaultvalue class used as a placeholder for defaults
         local_vars = {}
         code = func(cls)
         exec(code, globs, local_vars)
         # Having executed the code, the method should now exist
         # and can be retrieved by name from the dict
         method = local_vars[func.__name__]
         method.__qualname__ = f"{cls.__qualname__}.{method.__name__}"
```

### Comparing `prefab_classes-0.9.1/src/prefab_classes/dynamic/method_generators.py` & `prefab_classes-0.9.2/src/prefab_classes/dynamic/method_generators.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,29 +40,63 @@
 # ----------------------------------------------------------------------
 
 from ..constants import (
     PRE_INIT_FUNC,
     POST_INIT_FUNC,
     PREFAB_INIT_FUNC,
     FIELDS_ATTRIBUTE,
+    INTERNAL_DICT,
 )
 from ..sentinels import NOTHING
-from ..exceptions import FrozenPrefabError
 from .autogen import autogen
 
 
 def get_init_maker(*, init_name="__init__"):
     globs = {}
 
     def __init__(cls):
+        # Get the internals dictionary and prepare attributes
+        internals = getattr(cls, INTERNAL_DICT)
+        attributes = internals["attributes"]
+
+        # Handle pre/post init first - post_init can change types for __init__
+        # Get pre and post init arguments
+        pre_init_args = []
+        post_init_args = []
+        post_init_annotations = {}
+
+        for func_name, func_arglist in [
+            (PRE_INIT_FUNC, pre_init_args),
+            (POST_INIT_FUNC, post_init_args),
+        ]:
+            try:
+                func = getattr(cls, func_name)
+                func_code = func.__code__
+            except AttributeError:
+                pass
+            else:
+                argcount = func_code.co_argcount + func_code.co_kwonlyargcount
+                arglist = func_code.co_varnames[:argcount]
+
+                for item in arglist:
+                    if item != "self":
+                        func_arglist.append(item)
+
+                if func_name == POST_INIT_FUNC:
+                    post_init_annotations.update(func.__annotations__)
+
         pos_arglist = []
         kw_only_arglist = []
-        for name, attrib in cls._attributes.items():
-            if attrib._type is not NOTHING:
+        for name, attrib in attributes.items():
+            # post_init annotations can be used to broaden types.
+            if name in post_init_annotations:
+                globs[f"_{name}_type"] = post_init_annotations[name]
+            elif attrib._type is not NOTHING:
                 globs[f"_{name}_type"] = attrib._type
+
             if attrib.init:
                 if attrib.default is not NOTHING:
                     if isinstance(attrib.default, (str, int, float, bool)):
                         # Just use the literal in these cases
                         if attrib._type is NOTHING:
                             arg = f"{name}={attrib.default!r}"
                         else:
@@ -105,38 +139,17 @@
         if pos_args and kw_args:
             args = f"{pos_args}, *, {kw_args}"
         elif kw_args:
             args = f"*, {kw_args}"
         else:
             args = pos_args
 
-        # Get pre and post init arguments
-        pre_init_args = []
-        post_init_args = []
-
-        for func_name, func_arglist in [
-            (PRE_INIT_FUNC, pre_init_args),
-            (POST_INIT_FUNC, post_init_args),
-        ]:
-            try:
-                func = getattr(cls, func_name)
-                func_code = func.__code__
-            except AttributeError:
-                pass
-            else:
-                argcount = func_code.co_argcount + func_code.co_kwonlyargcount
-                arglist = func_code.co_varnames[:argcount]
-
-                for item in arglist:
-                    if item != "self":
-                        func_arglist.append(item)
-
         assignments = []
         processes = []  # post_init values still need default factories to be called.
-        for name, attrib in cls._attributes.items():
+        for name, attrib in attributes.items():
             if attrib.init:
                 if attrib.default_factory is not NOTHING:
                     value = f"{name} if {name} is not None else _{name}_factory()"
                 else:
                     value = name
             else:
                 if attrib.default_factory is not NOTHING:
@@ -182,17 +195,19 @@
         return code
 
     return autogen(__init__, globs)
 
 
 def get_repr_maker(will_eval=True):
     def __repr__(cls):
+        internals = getattr(cls, INTERNAL_DICT)
+        attributes = internals["attributes"]
         content = ", ".join(
             f"{name}={{self.{name}!r}}"
-            for name, attrib in cls._attributes.items()
+            for name, attrib in attributes.items()
             if attrib.repr and not attrib.exclude_field
         )
         if will_eval:
             code = (
                 f"def __repr__(self):\n"
                 f"    return f'{{type(self).__qualname__}}({content})'"
             )
@@ -231,54 +246,54 @@
 
     return autogen(__eq__)
 
 
 def get_iter_maker():
     def __iter__(cls):
         field_names = getattr(cls, FIELDS_ATTRIBUTE)
-        if cls._attributes:
+        if field_names:
             values = "\n".join(f"    yield self.{name} " for name in field_names)
         else:
             values = "    yield from ()"
         code = f"def __iter__(self):\n{values}"
         return code
 
     return autogen(__iter__)
 
 
 def get_frozen_setattr_maker():
     def __setattr__(cls):
         field_names = getattr(cls, FIELDS_ATTRIBUTE)
 
         # Make the fields set literal
-        fields_delimited = ", ".join(f"'{field}'" for field in field_names)
+        fields_delimited = ", ".join(f"{field!r}" for field in field_names)
         field_set = f"{{ {fields_delimited} }}"
 
         # Dynamic prefabs are not slotted so it is possible to insert into the dict
         body = (
             f"    if hasattr(self, name) or name not in {field_set}:\n"
-            f'        raise FrozenPrefabError("Can not set or change values on frozen instances.")\n'
+            f'        raise TypeError("{cls.__name__!r} object does not support attribute assignment")\n'
             f"    else:\n"
             f"        self.__dict__[name] = value\n"
         )
         code = f"def __setattr__(self, name, value):\n{body}"
 
         return code
 
     # Pass the exception to exec
-    return autogen(__setattr__, {"FrozenPrefabError": FrozenPrefabError})
+    return autogen(__setattr__)
 
 
 def get_frozen_delattr_maker():
     def __delattr__(cls):
-        body = '    raise FrozenPrefabError("Can not delete attributes on frozen instances.")\n'
+        body = f'    raise TypeError("{cls.__name__!r} object does not support attribute deletion")\n'
         code = f"def __delattr__(self, name):\n{body}"
         return code
 
-    return autogen(__delattr__, {"FrozenPrefabError": FrozenPrefabError})
+    return autogen(__delattr__)
 
 
 init_maker = get_init_maker()
 prefab_init_maker = get_init_maker(init_name=PREFAB_INIT_FUNC)
 repr_maker = get_repr_maker(will_eval=True)
 repr_maker_no_eval = get_repr_maker(will_eval=False)
 eq_maker = get_eq_maker()
```

### Comparing `prefab_classes-0.9.1/src/prefab_classes/dynamic/prefab.py` & `prefab_classes-0.9.2/src/prefab_classes/dynamic/prefab.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 from ._attribute_class import Attribute
 from ..constants import (
     FIELDS_ATTRIBUTE,
     COMPILED_FLAG,
     CLASSVAR_NAME,
     PRE_INIT_FUNC,
     POST_INIT_FUNC,
+    INTERNAL_DICT,
 )
 from ..exceptions import PrefabError, LivePrefabError, CompiledPrefabError
 from ..sentinels import NOTHING, KW_ONLY
 from .method_generators import (
     init_maker,
     repr_maker,
     repr_maker_no_eval,
@@ -74,38 +75,41 @@
 
 def attribute(
     *,
     default=NOTHING,
     default_factory=NOTHING,
     init=True,
     repr=True,
+    compare=True,
     kw_only=False,
     exclude_field=False,
 ):
     """
     Additional definition for how to generate standard methods
     for an instance attribute.
 
     :param default: Default value for this attribute
     :param default_factory: 0 argument callable to give a default value
                             (for otherwise mutable defaults, eg: list)
     :param init: Include this attribute in the __init__ parameters
     :param repr: Include this attribute in the class __repr__
+    :param compare: Include this attribute in the class __eq__
     :param kw_only: Make this argument keyword only in init
     :param exclude_field: Exclude this field from all magic method generation
                           apart from __init__
                           and do not include it in PREFAB_FIELDS
 
     :return: Attribute generated with these parameters.
     """
     return Attribute(
         default=default,
         default_factory=default_factory,
         init=init,
         repr=repr,
+        compare=compare,
         kw_only=kw_only,
         exclude_field=exclude_field,
     )
 
 
 def _make_prefab(
     cls: type,
@@ -131,22 +135,24 @@
     :param frozen: Prevent attribute values from being changed once defined
                    (This does not prevent the modification of mutable attributes such as lists)
     :return: class with __ methods defined
     """
     # If this function is called then this is a dynamic prefab
     setattr(cls, COMPILED_FLAG, False)
 
+    # Make the internals dict
+    prefab_internals: dict[str, dict[str, Attribute]] = {}
+    setattr(cls, INTERNAL_DICT, prefab_internals)
+
     # We need to look at type hints for the type hint
     # syntax variant.
     # If a key exists and is *NOT* in __annotations__ then all
     # annotations will be ignored as it becomes complex to fix the
     # ordering.
-
-    # Make a copy of the __annotations__ dictionary
-    cls_annotations = getattr(cls, "__annotations__", {}).copy()
+    cls_annotations = getattr(cls, "__annotations__", {})
 
     cls_annotation_names = cls_annotations.keys()
 
     cls_attributes = {k: v for k, v in vars(cls).items() if isinstance(v, Attribute)}
 
     cls_attribute_names = cls_attributes.keys()
 
@@ -185,43 +191,39 @@
 
                 if kw_flag or kw_only:
                     attrib.kw_only = True
 
                 attrib._type = cls_annotations[name]
                 new_attributes[name] = attrib
 
-            # Remove the original annotation
-            del cls.__annotations__[name]
         cls_attributes = new_attributes
     else:
         for name, attrib in cls_attributes.items():
             if kw_only:
                 attrib.kw_only = True
 
             delattr(cls, name)
             # Some items can still be annotated.
             try:
-                attrib._type = cls.__annotations__[name]
-                del cls.__annotations__[name]
-            except (AttributeError, KeyError):
-                # AttributeError as 3.9 does not guarantee the existence of __annotations__
+                attrib._type = cls_annotations[name]
+            except KeyError:
                 pass
 
-    setattr(cls, f"_{cls.__name__}_attributes", cls_attributes)
+    prefab_internals['local_attributes'] = cls_attributes
 
     mro = cls.__mro__[:-1]  # skip 'object' base class
 
     # Handle inheritance
     if mro == (cls,):  # special case of no inheritance.
         attributes = cls_attributes.copy()
     else:
         attributes = {}
         for c in reversed(mro):
             try:
-                attributes.update(getattr(c, f"_{c.__name__}_attributes"))
+                attributes.update(getattr(c, INTERNAL_DICT)["local_attributes"])
             except AttributeError:
                 pass
 
     # Check pre_init and post_init functions if they exist
     try:
         func = getattr(cls, PRE_INIT_FUNC)
         func_code = func.__code__
@@ -291,17 +293,18 @@
                     raise SyntaxError(
                         "non-default argument follows default argument",
                         f"defaults: {names}",
                         f"non_default after default: {name}",
                     )
 
     setattr(cls, FIELDS_ATTRIBUTE, valid_fields)
-    cls._attributes = attributes
+    prefab_internals["attributes"] = attributes
+
     if match_args and "__match_args__" not in cls.__dict__:
-        cls.__match_args__ = tuple(valid_fields)
+        setattr(cls, "__match_args__", tuple(valid_fields))
 
     if init and "__init__" not in cls.__dict__:
         setattr(cls, "__init__", init_maker)
     else:
         setattr(cls, "__prefab_init__", prefab_init_maker)
     if repr and "__repr__" not in cls.__dict__:
         if use_eval_repr:
@@ -317,15 +320,15 @@
         setattr(cls, "__delattr__", frozen_delattr_maker)
 
     return cls
 
 
 @dataclass_transform(field_specifiers=(attribute,))
 def prefab(
-    cls: type = None,
+    cls=None,
     *,
     init=True,
     repr=True,
     eq=True,
     iter=False,
     match_args=True,
     kw_only=False,
@@ -402,15 +405,15 @@
 
 
 def build_prefab(
     class_name: str,
     attributes: list[tuple[str, Attribute]],
     *,
     bases: tuple[type, ...] = (),
-    class_dict: dict[str, object] = None,
+    class_dict: "None | dict[str, object]" = None,
     init=True,
     repr=True,
     eq=True,
     iter=False,
     match_args=True,
     kw_only=False,
     frozen=False,
```

### Comparing `prefab_classes-0.9.1/src/prefab_classes/exceptions.py` & `prefab_classes-0.9.2/src/prefab_classes/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,11 +27,7 @@
 
 class LivePrefabError(PrefabError):
     pass
 
 
 class CompiledPrefabError(PrefabError):
     pass
-
-
-class FrozenPrefabError(PrefabError):
-    pass
```

### Comparing `prefab_classes-0.9.1/src/prefab_classes/funcs.py` & `prefab_classes-0.9.2/src/prefab_classes/funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,26 +52,26 @@
     funcdef = f"def asdict(obj): return {out_dict}"
     globs, locs = {}, {}
     exec(funcdef, globs, locs)
     method = locs["asdict"]
     return method
 
 
-def as_dict(inst, *, excludes: "None | tuple[str, ...]" = None):
+def as_dict(inst, *, excludes: "None | tuple[str, ...]" = None) -> dict[str, object]:
     """
-    Represent the prefab as a dictionary of attribute names and values.
+    Represent the prefab as a dictionary of attribute names stuband values.
     Exclude any keys listed in `excludes`
 
     This **does not** recurse.
 
     :param inst: instance of prefab class
     :param excludes: tuple of field names to exclude from the resulting dict
     :return: dictionary {attribute_name: attribute_value, ...}
     """
-    return _as_dict_cache(type(inst), excludes)(inst)
+    return _as_dict_cache(inst.__class__, excludes)(inst)
 
 
 @lru_cache
 def _as_dict_json_wrapper(excludes: "None | tuple[str, ...]" = None):
     def _as_dict_json_inner(inst):
         """Wrapper that gives a more accurate TypeError message for serialization"""
         try:
@@ -116,15 +116,15 @@
     return default
 
 
 def to_json(
     inst,
     *,
     excludes: "None | tuple[str, ...]" = None,
-    dumps_func: Callable[[object], str] = None,
+    dumps_func: "None | Callable[..., str]" = None,
     **kwargs,
 ) -> str:
     """
     Output the class attributes as JSON
 
     If no dumps function it will attempt to reuse the basic encoder
```

### Comparing `prefab_classes-0.9.1/src/prefab_classes/sentinels.py` & `prefab_classes-0.9.2/src/prefab_classes/sentinels.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 # KW_ONLY sentinel 'type' to use to indicate all subsequent attributes are
 # keyword only
 class _KW_ONLY_TYPE:
     def __repr__(self):
         return "<KW_ONLY Sentinel Object>"
 
 
-KW_ONLY = _KW_ONLY_TYPE
+KW_ONLY = _KW_ONLY_TYPE()
```

### Comparing `prefab_classes-0.9.1/src/prefab_classes.egg-info/PKG-INFO` & `prefab_classes-0.9.2/src/prefab_classes.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefab-classes
-Version: 0.9.1
+Version: 0.9.2
 Summary: Boilerplate Generator for Classes
 Author: David C Ellis
 Project-URL: Homepage, https://github.com/davidcellis/PrefabClasses
 Project-URL: Documentation, https://prefabclasses.readthedocs.io/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -21,17 +21,22 @@
 
 # PrefabClasses - Python Class Boilerplate Generator  #
 ![PrefabClasses Test Status](https://github.com/DavidCEllis/PrefabClasses/actions/workflows/auto_test.yml/badge.svg?branch=main)
 
 Writes the class boilerplate code so you don't have to. 
 Yet another variation on attrs/dataclasses.
 
-Either written lazily when you first access the methods or
-eagerly when the class is compiled into a .pyc. Can optionally
-be made to rewrite .py source code with plain classes.
+Unlike `dataclasses` or `attrs`, `prefab_classes` has a
+focus on performance and startup time in particular.
+This includes trying to minimise the impact of importing
+the module itself.
+
+Classes are written lazily when you first access the methods or
+eagerly when the module is compiled into a .pyc or rewritten out
+to a new .py source file.
 
 The dynamic method of evaluating lazily is more flexible, while
 the compiled method is faster (once the .pyc file has been generated).
 
 For more detail look at the [documentation](https://prefabclasses.readthedocs.io).
 
 ## Usage ##
```

### Comparing `prefab_classes-0.9.1/src/prefab_classes.egg-info/SOURCES.txt` & `prefab_classes-0.9.2/src/prefab_classes.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 src/prefab_classes/dynamic/_attribute_class.py
 src/prefab_classes/dynamic/autogen.py
 src/prefab_classes/dynamic/method_generators.py
 src/prefab_classes/dynamic/prefab.py
 src/prefab_classes/dynamic/_attribute_class_maker/_attribute_template.py
 src/prefab_classes/dynamic/_attribute_class_maker/regenerate_attribute.py
 src/prefab_classes_hook/__init__.py
-src/prefab_classes_hook/import_hook.py
+tests/test_versions_match.py
```

### Comparing `prefab_classes-0.9.1/src/prefab_classes_hook/import_hook.py` & `prefab_classes-0.9.2/src/prefab_classes_hook/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Hook into the import mechanism and sneakily translate our modules before python gets there
 """
 import sys
 
 # We probably shouldn't be importing from here, but it also halves the import time.
 try:
-    from _frozen_importlib_external import PathFinder, SourceFileLoader
+    from _frozen_importlib_external import PathFinder, SourceFileLoader  # type: ignore
 except ImportError:
     from importlib.machinery import PathFinder, SourceFileLoader
 
-from . import PREFAB_MAGIC_BYTES
-
+__version__ = "v0.9.2"
+PREFAB_MAGIC_BYTES = b"PREFAB_CLASSES_v0.9.2"
 
 __all__ = ["prefab_compiler", "insert_prefab_importhook", "remove_prefab_importhook"]
 
 
 HOOK_REWRITE = "# COMPILE_PREFABS"
 
 
@@ -43,14 +43,15 @@
 class PrefabHacker(SourceFileLoader):
     def __getattribute__(self, item):
         return super().__getattribute__(item)
 
     def source_to_code(self, data, path, *, _optimize=-1):
         # Only import the generator code if it is actually going to be used
         from prefab_classes.compiled.generator import compile_prefabs
+
         # Here we don't mind that importlib.util is slow to import
         # as we only do this on the compiling run
         from importlib.util import decode_source
 
         src = decode_source(data)
         prefab_src = compile_prefabs(src)
 
@@ -62,19 +63,25 @@
     @staticmethod
     def make_pyc_hash(source_bytes):
         # Modify the data given to the hash with extra data
         hash_input_bytes = b"".join([PREFAB_MAGIC_BYTES, source_bytes])
         try:
             # The fast way
             from _imp import source_hash
-            from _frozen_importlib_external import _RAW_MAGIC_NUMBER
+
+            try:
+                # Fastest
+                from _frozen_importlib_external import _RAW_MAGIC_NUMBER  # type: ignore
+            except ImportError:
+                # Slightly slower as importlib gets imported
+                from importlib._bootstrap_external import _RAW_MAGIC_NUMBER  # type: ignore
 
             return source_hash(_RAW_MAGIC_NUMBER, hash_input_bytes)
         except ImportError:
-            # The "correct" way
+            # The "correct"/slow way
             from importlib.util import source_hash
 
             return source_hash(hash_input_bytes)
 
     # noinspection PyUnresolvedReferences,PyProtectedMember
     def get_code(self, fullname):
         """
@@ -90,23 +97,31 @@
 
         Concrete implementation of InspectLoader.get_code.
         Reading of bytecode requires path_stats to be implemented. To write
         bytecode, set_data must also be implemented.
         """
         # These imports are all needed just for this function.
         # Unlike most of the other imports I don't know if there's a "right" place
-        # to get these from. They are also in _bootstrap_external but that's already
-        # wrong and slower anyway.
-        from _frozen_importlib_external import (
-            cache_from_source,
-            _classify_pyc,
-            _validate_hash_pyc,
-            _compile_bytecode,
-            _code_to_hash_pyc,
-        )
+        # to get these from.
+        try:
+            from _frozen_importlib_external import (
+                cache_from_source,
+                _classify_pyc,
+                _validate_hash_pyc,
+                _compile_bytecode,
+                _code_to_hash_pyc,
+            )
+        except ImportError:
+            from importlib._bootstrap_external import (
+                cache_from_source,
+                _classify_pyc,
+                _validate_hash_pyc,
+                _compile_bytecode,
+                _code_to_hash_pyc,
+            )
 
         source_path = self.get_filename(fullname)
         source_bytes = None
         source_hash_data = None
         check_source = True
         try:
             bytecode_path = cache_from_source(source_path)
```

