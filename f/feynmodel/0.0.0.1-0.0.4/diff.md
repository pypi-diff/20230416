# Comparing `tmp/feynmodel-0.0.0.1.tar.gz` & `tmp/feynmodel-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feynmodel-0.0.0.1.tar", max compression
+gzip compressed data, was "feynmodel-0.0.4.tar", max compression
```

## Comparing `feynmodel-0.0.0.1.tar` & `feynmodel-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,25 @@
--rw-r--r--   0        0        0    35149 2023-02-04 09:01:50.386436 feynmodel-0.0.0.1/LICENSE
--rw-r--r--   0        0        0     2311 2023-02-04 10:52:21.449238 feynmodel-0.0.0.1/README.md
--rw-r--r--   0        0        0      175 2023-02-04 09:38:51.111590 feynmodel-0.0.0.1/feynmodel/__init__.py
--rw-r--r--   0        0        0     1305 2023-02-04 09:31:55.457892 feynmodel-0.0.0.1/feynmodel/base_class.py
--rw-r--r--   0        0        0      321 2023-02-04 10:50:23.478693 feynmodel-0.0.0.1/feynmodel/coupling.py
--rw-r--r--   0        0        0      292 2023-02-04 10:50:27.986752 feynmodel-0.0.0.1/feynmodel/coupling_order.py
--rw-r--r--   0        0        0      432 2023-02-04 10:50:19.413639 feynmodel-0.0.0.1/feynmodel/decay.py
--rw-r--r--   0        0        0      279 2023-02-04 09:45:53.916315 feynmodel-0.0.0.1/feynmodel/feyn_model.py
--rw-r--r--   0        0        0      325 2023-02-04 10:50:13.779566 feynmodel-0.0.0.1/feynmodel/form_factor.py
--rw-r--r--   0        0        0      398 2023-02-04 10:50:09.243506 feynmodel-0.0.0.1/feynmodel/function.py
--rw-r--r--   0        0        0        0 2023-02-04 09:10:00.042739 feynmodel-0.0.0.1/feynmodel/interface/feynarts.py
--rw-r--r--   0        0        0      254 2023-02-04 10:56:23.188423 feynmodel-0.0.0.1/feynmodel/interface/qgraf.py
--rw-r--r--   0        0        0     1466 2023-02-04 10:50:51.339058 feynmodel-0.0.0.1/feynmodel/interface/ufo.py
--rw-r--r--   0        0        0      339 2023-02-04 10:50:04.883449 feynmodel-0.0.0.1/feynmodel/lorentz.py
--rw-r--r--   0        0        0      674 2023-02-04 10:50:00.819396 feynmodel-0.0.0.1/feynmodel/parameter.py
--rw-r--r--   0        0        0     3056 2023-02-04 10:49:46.741212 feynmodel-0.0.0.1/feynmodel/particle.py
--rw-r--r--   0        0        0      450 2023-02-04 10:49:55.182322 feynmodel-0.0.0.1/feynmodel/vertex.py
--rw-r--r--   0        0        0     1655 2023-02-04 10:56:54.198832 feynmodel-0.0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3297 1970-01-01 00:00:00.000000 feynmodel-0.0.0.1/setup.py
--rw-r--r--   0        0        0     3284 1970-01-01 00:00:00.000000 feynmodel-0.0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-16 11:59:08.907960 feynmodel-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2374 2023-04-16 11:59:08.907960 feynmodel-0.0.4/README.md
+-rw-r--r--   0        0        0      174 2023-04-16 11:59:08.907960 feynmodel-0.0.4/feynmodel/__init__.py
+-rw-r--r--   0        0        0      336 2023-04-16 11:59:08.907960 feynmodel-0.0.4/feynmodel/coupling.py
+-rw-r--r--   0        0        0      284 2023-04-16 11:59:08.907960 feynmodel-0.0.4/feynmodel/coupling_order.py
+-rw-r--r--   0        0        0      447 2023-04-16 11:59:08.907960 feynmodel-0.0.4/feynmodel/decay.py
+-rw-r--r--   0        0        0     4036 2023-04-16 11:59:08.907960 feynmodel-0.0.4/feynmodel/feyn_model.py
+-rw-r--r--   0        0        0      340 2023-04-16 11:59:08.907960 feynmodel-0.0.4/feynmodel/form_factor.py
+-rw-r--r--   0        0        0      383 2023-04-16 11:59:08.907960 feynmodel-0.0.4/feynmodel/function.py
+-rw-r--r--   0        0        0        0 2023-04-16 11:59:08.907960 feynmodel-0.0.4/feynmodel/interface/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 11:59:08.907960 feynmodel-0.0.4/feynmodel/interface/feynarts.py
+-rw-r--r--   0        0        0     2603 2023-04-16 11:59:08.907960 feynmodel-0.0.4/feynmodel/interface/qgraf.py
+-rw-r--r--   0        0        0     5250 2023-04-16 11:59:08.907960 feynmodel-0.0.4/feynmodel/interface/ufo.py
+-rw-r--r--   0        0        0      354 2023-04-16 11:59:08.907960 feynmodel-0.0.4/feynmodel/lorentz.py
+-rw-r--r--   0        0        0        0 2023-04-16 11:59:08.907960 feynmodel-0.0.4/feynmodel/model/__init__.py
+-rw-r--r--   0        0        0      277 2023-04-16 11:59:08.907960 feynmodel-0.0.4/feynmodel/model/mssm.py
+-rw-r--r--   0        0        0      248 2023-04-16 11:59:08.907960 feynmodel-0.0.4/feynmodel/model/sm.py
+-rw-r--r--   0        0        0      689 2023-04-16 11:59:08.907960 feynmodel-0.0.4/feynmodel/parameter.py
+-rw-r--r--   0        0        0     3143 2023-04-16 11:59:08.907960 feynmodel-0.0.4/feynmodel/particle.py
+-rw-r--r--   0        0        0     1313 2023-04-16 11:59:08.907960 feynmodel-0.0.4/feynmodel/ufo_base_class.py
+-rw-r--r--   0        0        0      777 2023-04-16 11:59:08.907960 feynmodel-0.0.4/feynmodel/util.py
+-rw-r--r--   0        0        0      494 2023-04-16 11:59:08.907960 feynmodel-0.0.4/feynmodel/vertex.py
+-rw-r--r--   0        0        0     1574 2023-04-16 11:59:10.951982 feynmodel-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3274 1970-01-01 00:00:00.000000 feynmodel-0.0.4/setup.py
+-rw-r--r--   0        0        0     3222 1970-01-01 00:00:00.000000 feynmodel-0.0.4/PKG-INFO
```

### Comparing `feynmodel-0.0.0.1/LICENSE` & `feynmodel-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `feynmodel-0.0.0.1/README.md` & `feynmodel-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # FeynModel
 
 FeynModel is a project to develop an XML dialect for describing Feynman Models.
-It is in design very close to the UFO format, but not as restrictive.
+It is in design very close to the UFO format, but not as restrictive (-> less complete).
 
 [![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/feynml.svg)
 
 
 [![test][a t image]][a t link]     [![Coverage Status][c t i]][c t l] [![Codacy Badge][cc c i]][cc c l]  [![Codacy Badge][cc q i]][cc q l]  [![Documentation][rtd t i]][rtd t l]
 
 ## Installation
 ```sh
-pip install [--user] feynml
+pip install [--user] feynmodel
 ```
 
 or from cloned source:
 
 ```sh
 poerty install --with docs --with dev
 poetry shell
@@ -23,14 +23,15 @@
 ## Documentation
 
 *   <https://pyfeyn2.readthedocs.io/en/stable/feynml/>
 *   <https://apn-pucky.github.io/pyfeyn2/feynml/index.html>
 
 ## Related:
 
+*   <https://github.com/APN-Pucky/feynml>
 *   <https://github.com/APN-Pucky/pyfeyn2>
 
 
 ## Development
 
 
 ### package/python structure:
@@ -44,18 +45,17 @@
 [pypi image]: https://badge.fury.io/py/feynmodel.svg
 [pypi link]: https://pypi.org/project/feynmodel/
 [pypi versions]: https://img.shields.io/pypi/pyversions/feynmodel.svg
 
 [a t link]: https://github.com/APN-Pucky/feynmodel/actions/workflows/test.yml
 [a t image]: https://github.com/APN-Pucky/feynmodel/actions/workflows/test.yml/badge.svg
 
-
-[cc q i]: https://app.codacy.com/project/badge/Grade/135bae47c6344ab0bfb180135ea1db44
+[cc q i]: https://app.codacy.com/project/badge/Grade/6604fe515a7e4ebf927b44f8f5f79dc0
 [cc q l]: https://www.codacy.com/gh/APN-Pucky/feynmodel/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/feynmodel&amp;utm_campaign=Badge_Grade
-[cc c i]: https://app.codacy.com/project/badge/Coverage/135bae47c6344ab0bfb180135ea1db44
+[cc c i]: https://app.codacy.com/project/badge/Coverage/6604fe515a7e4ebf927b44f8f5f79dc0
 [cc c l]: https://www.codacy.com/gh/APN-Pucky/feynmodel/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/feynmodel&utm_campaign=Badge_Coverage
 
 [c t l]: https://coveralls.io/github/APN-Pucky/feynmodel?branch=master
 [c t i]: https://coveralls.io/repos/github/APN-Pucky/feynmodel/badge.svg?branch=master
 
 [rtd t i]: https://readthedocs.org/projects/pyfeyn2/badge/?version=latest
 [rtd t l]: https://pyfeyn2.readthedocs.io/en/latest/?badge=latest
```

### Comparing `feynmodel-0.0.0.1/feynmodel/base_class.py` & `feynmodel-0.0.4/feynmodel/ufo_base_class.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-class BaseClass(object):
+class UFOBaseClass(object):
     """The class from which all FeynRules classes are derived."""
 
     require_args = []
 
     def __init__(self, *args, **options):
-        assert(len(self.require_args) == len (args))
-    
+        assert len(self.require_args) == len(args)
         for i, name in enumerate(self.require_args):
             setattr(self, name, args[i])
-    
+
         for (option, value) in options.items():
             setattr(self, option, value)
 
     def get(self, name):
         return getattr(self, name)
-    
+
     def set(self, name, value):
         setattr(self, name, value)
-        
+
     def get_all(self):
         """Return a dictionary containing all the information of the object"""
         return self.__dict__
 
     def __str__(self):
         return self.name
 
     def nice_string(self):
-        """ return string with the full information """
-        return '\n'.join(['%s \t: %s' %(name, value) for name, value in self.__dict__.items()])
+        """return string with the full information"""
+        return "\n".join(
+            ["%s \t: %s" % (name, value) for name, value in self.__dict__.items()]
+        )
 
     def __repr__(self):
         replacements = [
-            ('+','__plus__'),
-            ('-','__minus__'),
-            ('@','__at__'),
-            ('!','__exclam__'),
-            ('?','__quest__'),
-            ('*','__star__'),
-            ('~','__tilde__')
-            ]
+            ("+", "__plus__"),
+            ("-", "__minus__"),
+            ("@", "__at__"),
+            ("!", "__exclam__"),
+            ("?", "__quest__"),
+            ("*", "__star__"),
+            ("~", "__tilde__"),
+        ]
         text = self.name
-        for orig,sub in replacements:
-            text = text.replace(orig,sub)
-        return text
+        for orig, sub in replacements:
+            text = text.replace(orig, sub)
+        return text
```

### Comparing `feynmodel-0.0.0.1/feynmodel/parameter.py` & `feynmodel-0.0.4/feynmodel/parameter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from feynmodel.base_class import BaseClass
+from feynmodel.ufo_base_class import UFOBaseClass
 
 
-class Parameter(BaseClass):
+class Parameter(UFOBaseClass):
 
     require_args = ["name", "nature", "type", "value", "texname"]
 
     def __init__(self, name, nature, type, value, texname, lhablock=None, lhacode=None):
 
         args = (name, nature, type, value, texname)
 
-        BaseClass.__init__(self, *args)
+        UFOBaseClass.__init__(self, *args)
 
         args = (name, nature, type, value, texname)
 
-        #global all_parameters
-        #all_parameters.append(self)
+        # global all_parameters
+        # all_parameters.append(self)
 
         if (lhablock is None or lhacode is None) and nature == "external":
             raise Exception('Need LHA information for external parameter "%s".' % name)
         self.lhablock = lhablock
         self.lhacode = lhacode
```

### Comparing `feynmodel-0.0.0.1/feynmodel/particle.py` & `feynmodel-0.0.4/feynmodel/particle.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from feynmodel.base_class import BaseClass
+from feynmodel.ufo_base_class import UFOBaseClass
 
 
-class Particle(BaseClass):
+class Particle(UFOBaseClass):
     """A standard Particle"""
 
     require_args = [
         "pdg_code",
         "name",
         "antiname",
         "spin",
@@ -31,24 +31,24 @@
         "line",
         "propagating",
         "goldstoneboson",
     ]
 
     def __init__(
         self,
-        pdg_code,
-        name,
-        antiname,
-        spin,
-        color,
-        mass,
-        width,
-        texname,
-        antitexname,
-        charge,
+        pdg_code=None,
+        name=None,
+        antiname=None,
+        spin=-99999999999,
+        color=None,
+        mass=None,
+        width=None,
+        texname=None,
+        antitexname=None,
+        charge=-99999999999999999,
         line=None,
         propagating=True,
         goldstoneboson=False,
         **options
     ):
 
         args = (
@@ -60,18 +60,18 @@
             mass,
             width,
             texname,
             antitexname,
             float(charge),
         )
 
-        BaseClass.__init__(self, *args, **options)
+        UFOBaseClass.__init__(self, *args, **options)
 
-        #global all_particles
-        #all_particles.append(self)
+        # global all_particles
+        # all_particles.append(self)
 
         self.propagating = propagating
         self.goldstoneboson = goldstoneboson
 
         self.selfconjugate = name == antiname
         if 1:  # not line:
             self.line = self.find_line_type()
```

### Comparing `feynmodel-0.0.0.1/pyproject.toml` & `feynmodel-0.0.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,36 @@
 [tool.poetry]
 name = "feynmodel"
-version = "0.0.0.1"
+version = "0.0.4"
 description = "Models for constructing Feynman diagrams"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
-repository = "https://github.com/APN-Pucky/feynml"
+repository = "https://github.com/APN-Pucky/feynmodel"
 
 [tool.poetry.dependencies]
 python = "^3.8"
+# These must remain flexible to allow for different versions of the same package
+# and let the user decide which version to use
+ufo_sm = "*"
+ufo_mssm = "*"
 particle = "*"
 xsdata = {version = "*", extras = ["cli","lxml","soap"]}
-cssutils= "*"
-cssselect ="*"
 #pyqgraf = {path= "../pyqgraf", develop = true }
 #ipyparallel = "*"
 deprecated = "*"
 deprecation = "*"
 smpl_io = "*"
 smpl_doc = "*"
 smpl_util= "*"
 
-pyqgraf = {version = ">=0.0.3", optional = true}
-pyhepmc = {version = "*", optional = true}
-
-[tool.poetry.extras]
-interface = ["pyqgraf", "pyhepmc"]
-
-
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-pyhepmc = "*" # for testing
-pyqgraf = ">=0.0.3" # for testing
-pre-commit = "^2.20.0"
+pre-commit = ">=2.20,<4.0"
 pytest = "*"
 pytest-cov =  "*"
 pytest-profiling =  "*"
 pytest-line-profiler-apn = ">=0.1.3"
 ipython =  "*"
 jupyterlab =  "*"
 jupyter = "*"
```

### Comparing `feynmodel-0.0.0.1/setup.py` & `feynmodel-0.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['feynmodel', 'feynmodel.interface']
+['feynmodel', 'feynmodel.interface', 'feynmodel.model']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['cssselect',
- 'cssutils',
- 'deprecated',
+['deprecated',
  'deprecation',
  'particle',
  'smpl_doc',
  'smpl_io',
  'smpl_util',
+ 'ufo_mssm',
+ 'ufo_sm',
  'xsdata[cli,lxml,soap]']
 
-extras_require = \
-{'interface': ['pyqgraf>=0.0.3', 'pyhepmc']}
-
 setup_kwargs = {
     'name': 'feynmodel',
-    'version': '0.0.0.1',
+    'version': '0.0.4',
     'description': 'Models for constructing Feynman diagrams',
-    'long_description': '# FeynModel\n\nFeynModel is a project to develop an XML dialect for describing Feynman Models.\nIt is in design very close to the UFO format, but not as restrictive.\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/feynml.svg)\n\n\n[![test][a t image]][a t link]     [![Coverage Status][c t i]][c t l] [![Codacy Badge][cc c i]][cc c l]  [![Codacy Badge][cc q i]][cc q l]  [![Documentation][rtd t i]][rtd t l]\n\n## Installation\n```sh\npip install [--user] feynml\n```\n\nor from cloned source:\n\n```sh\npoerty install --with docs --with dev\npoetry shell\n```\n\n## Documentation\n\n*   <https://pyfeyn2.readthedocs.io/en/stable/feynml/>\n*   <https://apn-pucky.github.io/pyfeyn2/feynml/index.html>\n\n## Related:\n\n*   <https://github.com/APN-Pucky/pyfeyn2>\n\n\n## Development\n\n\n### package/python structure:\n\n*   <https://mathspp.com/blog/how-to-create-a-python-package-in-2022>\n*   <https://www.brainsorting.com/posts/publish-a-package-on-pypi-using-poetry/>\n\n[doc stable]: https://apn-pucky.github.io/feynmodel/index.html\n[doc test]: https://apn-pucky.github.io/feynmodel/test/index.html\n\n[pypi image]: https://badge.fury.io/py/feynmodel.svg\n[pypi link]: https://pypi.org/project/feynmodel/\n[pypi versions]: https://img.shields.io/pypi/pyversions/feynmodel.svg\n\n[a t link]: https://github.com/APN-Pucky/feynmodel/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/feynmodel/actions/workflows/test.yml/badge.svg\n\n\n[cc q i]: https://app.codacy.com/project/badge/Grade/135bae47c6344ab0bfb180135ea1db44\n[cc q l]: https://www.codacy.com/gh/APN-Pucky/feynmodel/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/feynmodel&amp;utm_campaign=Badge_Grade\n[cc c i]: https://app.codacy.com/project/badge/Coverage/135bae47c6344ab0bfb180135ea1db44\n[cc c l]: https://www.codacy.com/gh/APN-Pucky/feynmodel/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/feynmodel&utm_campaign=Badge_Coverage\n\n[c t l]: https://coveralls.io/github/APN-Pucky/feynmodel?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/feynmodel/badge.svg?branch=master\n\n[rtd t i]: https://readthedocs.org/projects/pyfeyn2/badge/?version=latest\n[rtd t l]: https://pyfeyn2.readthedocs.io/en/latest/?badge=latest\n',
+    'long_description': '# FeynModel\n\nFeynModel is a project to develop an XML dialect for describing Feynman Models.\nIt is in design very close to the UFO format, but not as restrictive (-> less complete).\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/feynml.svg)\n\n\n[![test][a t image]][a t link]     [![Coverage Status][c t i]][c t l] [![Codacy Badge][cc c i]][cc c l]  [![Codacy Badge][cc q i]][cc q l]  [![Documentation][rtd t i]][rtd t l]\n\n## Installation\n```sh\npip install [--user] feynmodel\n```\n\nor from cloned source:\n\n```sh\npoerty install --with docs --with dev\npoetry shell\n```\n\n## Documentation\n\n*   <https://pyfeyn2.readthedocs.io/en/stable/feynml/>\n*   <https://apn-pucky.github.io/pyfeyn2/feynml/index.html>\n\n## Related:\n\n*   <https://github.com/APN-Pucky/feynml>\n*   <https://github.com/APN-Pucky/pyfeyn2>\n\n\n## Development\n\n\n### package/python structure:\n\n*   <https://mathspp.com/blog/how-to-create-a-python-package-in-2022>\n*   <https://www.brainsorting.com/posts/publish-a-package-on-pypi-using-poetry/>\n\n[doc stable]: https://apn-pucky.github.io/feynmodel/index.html\n[doc test]: https://apn-pucky.github.io/feynmodel/test/index.html\n\n[pypi image]: https://badge.fury.io/py/feynmodel.svg\n[pypi link]: https://pypi.org/project/feynmodel/\n[pypi versions]: https://img.shields.io/pypi/pyversions/feynmodel.svg\n\n[a t link]: https://github.com/APN-Pucky/feynmodel/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/feynmodel/actions/workflows/test.yml/badge.svg\n\n[cc q i]: https://app.codacy.com/project/badge/Grade/6604fe515a7e4ebf927b44f8f5f79dc0\n[cc q l]: https://www.codacy.com/gh/APN-Pucky/feynmodel/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/feynmodel&amp;utm_campaign=Badge_Grade\n[cc c i]: https://app.codacy.com/project/badge/Coverage/6604fe515a7e4ebf927b44f8f5f79dc0\n[cc c l]: https://www.codacy.com/gh/APN-Pucky/feynmodel/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/feynmodel&utm_campaign=Badge_Coverage\n\n[c t l]: https://coveralls.io/github/APN-Pucky/feynmodel?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/feynmodel/badge.svg?branch=master\n\n[rtd t i]: https://readthedocs.org/projects/pyfeyn2/badge/?version=latest\n[rtd t l]: https://pyfeyn2.readthedocs.io/en/latest/?badge=latest\n',
     'author': 'Alexander Puck Neuwirth',
     'author_email': 'alexander@neuwirth-informatik.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'https://github.com/APN-Pucky/feynml',
+    'url': 'https://github.com/APN-Pucky/feynmodel',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'extras_require': extras_require,
     'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `feynmodel-0.0.0.1/PKG-INFO` & `feynmodel-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,45 @@
 Metadata-Version: 2.1
 Name: feynmodel
-Version: 0.0.0.1
+Version: 0.0.4
 Summary: Models for constructing Feynman diagrams
-Home-page: https://github.com/APN-Pucky/feynml
+Home-page: https://github.com/APN-Pucky/feynmodel
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: interface
-Requires-Dist: cssselect
-Requires-Dist: cssutils
 Requires-Dist: deprecated
 Requires-Dist: deprecation
 Requires-Dist: particle
-Requires-Dist: pyhepmc; extra == "interface"
-Requires-Dist: pyqgraf (>=0.0.3); extra == "interface"
 Requires-Dist: smpl_doc
 Requires-Dist: smpl_io
 Requires-Dist: smpl_util
+Requires-Dist: ufo_mssm
+Requires-Dist: ufo_sm
 Requires-Dist: xsdata[cli,lxml,soap]
-Project-URL: Repository, https://github.com/APN-Pucky/feynml
+Project-URL: Repository, https://github.com/APN-Pucky/feynmodel
 Description-Content-Type: text/markdown
 
 # FeynModel
 
 FeynModel is a project to develop an XML dialect for describing Feynman Models.
-It is in design very close to the UFO format, but not as restrictive.
+It is in design very close to the UFO format, but not as restrictive (-> less complete).
 
 [![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/feynml.svg)
 
 
 [![test][a t image]][a t link]     [![Coverage Status][c t i]][c t l] [![Codacy Badge][cc c i]][cc c l]  [![Codacy Badge][cc q i]][cc q l]  [![Documentation][rtd t i]][rtd t l]
 
 ## Installation
 ```sh
-pip install [--user] feynml
+pip install [--user] feynmodel
 ```
 
 or from cloned source:
 
 ```sh
 poerty install --with docs --with dev
 poetry shell
@@ -51,14 +48,15 @@
 ## Documentation
 
 *   <https://pyfeyn2.readthedocs.io/en/stable/feynml/>
 *   <https://apn-pucky.github.io/pyfeyn2/feynml/index.html>
 
 ## Related:
 
+*   <https://github.com/APN-Pucky/feynml>
 *   <https://github.com/APN-Pucky/pyfeyn2>
 
 
 ## Development
 
 
 ### package/python structure:
@@ -72,18 +70,17 @@
 [pypi image]: https://badge.fury.io/py/feynmodel.svg
 [pypi link]: https://pypi.org/project/feynmodel/
 [pypi versions]: https://img.shields.io/pypi/pyversions/feynmodel.svg
 
 [a t link]: https://github.com/APN-Pucky/feynmodel/actions/workflows/test.yml
 [a t image]: https://github.com/APN-Pucky/feynmodel/actions/workflows/test.yml/badge.svg
 
-
-[cc q i]: https://app.codacy.com/project/badge/Grade/135bae47c6344ab0bfb180135ea1db44
+[cc q i]: https://app.codacy.com/project/badge/Grade/6604fe515a7e4ebf927b44f8f5f79dc0
 [cc q l]: https://www.codacy.com/gh/APN-Pucky/feynmodel/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/feynmodel&amp;utm_campaign=Badge_Grade
-[cc c i]: https://app.codacy.com/project/badge/Coverage/135bae47c6344ab0bfb180135ea1db44
+[cc c i]: https://app.codacy.com/project/badge/Coverage/6604fe515a7e4ebf927b44f8f5f79dc0
 [cc c l]: https://www.codacy.com/gh/APN-Pucky/feynmodel/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/feynmodel&utm_campaign=Badge_Coverage
 
 [c t l]: https://coveralls.io/github/APN-Pucky/feynmodel?branch=master
 [c t i]: https://coveralls.io/repos/github/APN-Pucky/feynmodel/badge.svg?branch=master
 
 [rtd t i]: https://readthedocs.org/projects/pyfeyn2/badge/?version=latest
 [rtd t l]: https://pyfeyn2.readthedocs.io/en/latest/?badge=latest
```

