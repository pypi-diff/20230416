# Comparing `tmp/pluthon-0.3.3.tar.gz` & `tmp/pluthon-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluthon-0.3.3.tar", last modified: Fri Mar 31 13:11:39 2023, max compression
+gzip compressed data, was "pluthon-0.3.5.tar", last modified: Sat Apr 15 22:55:26 2023, max compression
```

## Comparing `pluthon-0.3.3.tar` & `pluthon-0.3.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-03-31 13:11:39.678069 pluthon-0.3.3/
--rw-r--r--   0 travis    (1000) travis    (1000)     1776 2023-03-31 13:11:39.678069 pluthon-0.3.3/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)     1001 2023-03-31 13:11:02.000000 pluthon-0.3.3/README.md
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-03-31 13:11:39.674069 pluthon-0.3.3/pluthon/
--rw-r--r--   0 travis    (1000) travis    (1000)      594 2023-03-31 13:11:02.000000 pluthon-0.3.3/pluthon/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4583 2023-03-31 13:11:02.000000 pluthon-0.3.3/pluthon/pluthon_ast.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2582 2023-03-31 13:11:02.000000 pluthon-0.3.3/pluthon/pluthon_functional_data.py
--rw-r--r--   0 travis    (1000) travis    (1000)    17868 2023-03-31 13:11:02.000000 pluthon-0.3.3/pluthon/pluthon_sugar.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-03-31 13:11:39.678069 pluthon-0.3.3/pluthon.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)     1776 2023-03-31 13:11:39.000000 pluthon-0.3.3/pluthon.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)      275 2023-03-31 13:11:39.000000 pluthon-0.3.3/pluthon.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2023-03-31 13:11:39.000000 pluthon-0.3.3/pluthon.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       12 2023-03-31 13:11:39.000000 pluthon-0.3.3/pluthon.egg-info/requires.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       13 2023-03-31 13:11:39.000000 pluthon-0.3.3/pluthon.egg-info/top_level.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       38 2023-03-31 13:11:39.678069 pluthon-0.3.3/setup.cfg
--rw-r--r--   0 travis    (1000) travis    (1000)     1682 2023-03-31 13:11:02.000000 pluthon-0.3.3/setup.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-15 22:55:26.906589 pluthon-0.3.5/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1776 2023-04-15 22:55:26.902589 pluthon-0.3.5/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)     1001 2023-04-15 22:54:47.000000 pluthon-0.3.5/README.md
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-15 22:55:26.902589 pluthon-0.3.5/pluthon/
+-rw-r--r--   0 travis    (1000) travis    (1000)      594 2023-04-15 22:54:47.000000 pluthon-0.3.5/pluthon/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4583 2023-04-15 22:54:47.000000 pluthon-0.3.5/pluthon/pluthon_ast.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2582 2023-04-15 22:54:47.000000 pluthon-0.3.5/pluthon/pluthon_functional_data.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    17937 2023-04-15 22:54:47.000000 pluthon-0.3.5/pluthon/pluthon_sugar.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-15 22:55:26.902589 pluthon-0.3.5/pluthon.egg-info/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1776 2023-04-15 22:55:26.000000 pluthon-0.3.5/pluthon.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)      275 2023-04-15 22:55:26.000000 pluthon-0.3.5/pluthon.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        1 2023-04-15 22:55:26.000000 pluthon-0.3.5/pluthon.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       12 2023-04-15 22:55:26.000000 pluthon-0.3.5/pluthon.egg-info/requires.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       13 2023-04-15 22:55:26.000000 pluthon-0.3.5/pluthon.egg-info/top_level.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       38 2023-04-15 22:55:26.906589 pluthon-0.3.5/setup.cfg
+-rw-r--r--   0 travis    (1000) travis    (1000)     1682 2023-04-15 22:54:47.000000 pluthon-0.3.5/setup.py
```

### Comparing `pluthon-0.3.3/PKG-INFO` & `pluthon-0.3.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluthon
-Version: 0.3.3
+Version: 0.3.5
 Summary: Pluto-like programming language for Cardano Smart Contracts in Python
 Home-page: https://github.com/imperatorlang/pluthon
 Author: nielstron
 Author-email: n.muendler@web.de
 License: MIT
 Keywords: python cardano smart contract blockchain verification haskell
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pluthon-0.3.3/README.md` & `pluthon-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pluthon-0.3.3/pluthon/__init__.py` & `pluthon-0.3.5/pluthon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from .pluthon_functional_data import *
 except ImportError as e:
     logging.error(
         "Error, trying to import dependencies. Should only occur upon package installation",
         exc_info=e,
     )
 
-VERSION = (0, 3, 3)
+VERSION = (0, 3, 5)
 
 __version__ = ".".join([str(i) for i in VERSION])
 __author__ = "nielstron"
 __author_email__ = "n.muendler@web.de"
 __copyright__ = "Copyright (C) 2023 nielstron"
 __license__ = "MIT"
 __url__ = "https://github.com/imperatorlang/pluthon"
```

### Comparing `pluthon-0.3.3/pluthon/pluthon_ast.py` & `pluthon-0.3.5/pluthon/pluthon_ast.py`

 * *Files identical despite different names*

### Comparing `pluthon-0.3.3/pluthon/pluthon_functional_data.py` & `pluthon-0.3.5/pluthon/pluthon_functional_data.py`

 * *Files identical despite different names*

### Comparing `pluthon-0.3.3/pluthon/pluthon_sugar.py` & `pluthon-0.3.5/pluthon/pluthon_sugar.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,14 +188,15 @@
 UnListData = wrap_builtin_unop(uplc_ast.BuiltInFun.UnListData)
 UnIData = wrap_builtin_unop(uplc_ast.BuiltInFun.UnIData)
 UnBData = wrap_builtin_unop(uplc_ast.BuiltInFun.UnBData)
 EqualsData = wrap_builtin_binop(uplc_ast.BuiltInFun.EqualsData)
 MkPairData = wrap_builtin_binop(uplc_ast.BuiltInFun.MkPairData)
 MkNilData = wrap_builtin_unop(uplc_ast.BuiltInFun.MkNilData)
 MkNilPairData = wrap_builtin_unop(uplc_ast.BuiltInFun.MkNilPairData)
+SerialiseData = wrap_builtin_unop(uplc_ast.BuiltInFun.SerialiseData)
 
 # Generic Utils
 
 TraceConst = lambda x, y: Trace(Text(x), y)
 TraceError = lambda x: Apply(Error(), Trace(Text(x), Unit()))
```

### Comparing `pluthon-0.3.3/pluthon.egg-info/PKG-INFO` & `pluthon-0.3.5/pluthon.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluthon
-Version: 0.3.3
+Version: 0.3.5
 Summary: Pluto-like programming language for Cardano Smart Contracts in Python
 Home-page: https://github.com/imperatorlang/pluthon
 Author: nielstron
 Author-email: n.muendler@web.de
 License: MIT
 Keywords: python cardano smart contract blockchain verification haskell
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pluthon-0.3.3/setup.py` & `pluthon-0.3.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     version=pluthon.__version__,
     description="Pluto-like programming language for Cardano Smart Contracts in Python",
     author=pluthon.__author__,
     author_email=pluthon.__author_email__,
     url=pluthon.__url__,
     py_modules=["uplc"],
     packages=find_packages(),
-    install_requires=["uplc==0.6.1"],
+    install_requires=["uplc==0.6.2"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     license=pluthon.__license__,
     classifiers=[
         "Development Status :: 3 - Alpha",
         # Indicate who your project is intended for
         "Intended Audience :: Developers",
```

