# Comparing `tmp/typer_builder-0.0.8.tar.gz` & `tmp/typer_builder-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_builder-0.0.8.tar", max compression
+gzip compressed data, was "typer_builder-0.0.9.tar", max compression
```

## Comparing `typer_builder-0.0.8.tar` & `typer_builder-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      998 2023-03-05 04:09:53.796929 typer_builder-0.0.8/LICENSE
--rw-r--r--   0        0        0     1602 2023-04-16 14:13:46.762430 typer_builder-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3623 2023-04-16 14:11:14.594706 typer_builder-0.0.8/readme.md
--rw-r--r--   0        0        0    10293 2023-04-16 14:07:29.485030 typer_builder-0.0.8/src/typer_builder/Dependencies.py
--rw-r--r--   0        0        0     2496 2023-04-16 14:04:36.241894 typer_builder-0.0.8/src/typer_builder/Dependencies_test.py
--rw-r--r--   0        0        0      330 2023-04-16 14:13:46.762430 typer_builder-0.0.8/src/typer_builder/__init__.py
--rw-r--r--   0        0        0     4964 2023-04-16 14:04:06.414731 typer_builder-0.0.8/src/typer_builder/build_app.py
--rw-r--r--   0        0        0      661 2023-04-16 14:04:16.258455 typer_builder-0.0.8/src/typer_builder/build_app_test.py
--rw-r--r--   0        0        0        0 2023-03-05 04:09:53.800929 typer_builder-0.0.8/src/typer_builder/py.typed
--rw-r--r--   0        0        0     4520 1970-01-01 00:00:00.000000 typer_builder-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      998 2023-03-05 04:09:53.796929 typer_builder-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1602 2023-04-16 17:46:20.604004 typer_builder-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3623 2023-04-16 14:11:14.594706 typer_builder-0.0.9/readme.md
+-rw-r--r--   0        0        0    10293 2023-04-16 14:19:37.368576 typer_builder-0.0.9/src/typer_builder/Dependencies.py
+-rw-r--r--   0        0        0     2496 2023-04-16 14:04:36.241894 typer_builder-0.0.9/src/typer_builder/Dependencies_test.py
+-rw-r--r--   0        0        0      330 2023-04-16 17:46:20.604004 typer_builder-0.0.9/src/typer_builder/__init__.py
+-rw-r--r--   0        0        0     4982 2023-04-16 17:45:34.261306 typer_builder-0.0.9/src/typer_builder/build_app.py
+-rw-r--r--   0        0        0      661 2023-04-16 14:04:16.258455 typer_builder-0.0.9/src/typer_builder/build_app_test.py
+-rw-r--r--   0        0        0        0 2023-03-05 04:09:53.800929 typer_builder-0.0.9/src/typer_builder/py.typed
+-rw-r--r--   0        0        0     4520 1970-01-01 00:00:00.000000 typer_builder-0.0.9/PKG-INFO
```

### Comparing `typer_builder-0.0.8/LICENSE` & `typer_builder-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `typer_builder-0.0.8/pyproject.toml` & `typer_builder-0.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "typer-builder"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 packages = [{ include = "typer_builder", from = "src" }]
 classifiers = []
 keywords = []
```

### Comparing `typer_builder-0.0.8/readme.md` & `typer_builder-0.0.9/readme.md`

 * *Files identical despite different names*

### Comparing `typer_builder-0.0.8/src/typer_builder/Dependencies.py` & `typer_builder-0.0.9/src/typer_builder/Dependencies.py`

 * *Files identical despite different names*

### Comparing `typer_builder-0.0.8/src/typer_builder/Dependencies_test.py` & `typer_builder-0.0.9/src/typer_builder/Dependencies_test.py`

 * *Files identical despite different names*

### Comparing `typer_builder-0.0.8/src/typer_builder/build_app.py` & `typer_builder-0.0.9/src/typer_builder/build_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     if not isinstance(dependencies, Dependencies):
         dependencies = Dependencies(*dependencies)
 
     module = import_module(module_name)
     assert module.__file__, f"module {module_name!r} has no __file__"
     assert Path(module.__file__).stem == "__init__", f"expected a package for {module_name!r}"
 
-    name = name or module_name.rpartition(".")[-1]
+    name = name or module_name.rpartition(".")[-1].replace("_", "-")
     app = Typer(name=name, help=module.__doc__, **(typer_options or {}))
 
     if hasattr(module, "callback"):
         app.callback()(_prepare_typer_func(module.callback, dependencies, event_loop))
 
     for submodule_info in iter_modules(module.__path__, prefix=module_name + "."):
         submodule_name = submodule_info.name.rpartition(".")[-1]
```

### Comparing `typer_builder-0.0.8/src/typer_builder/build_app_test.py` & `typer_builder-0.0.9/src/typer_builder/build_app_test.py`

 * *Files identical despite different names*

### Comparing `typer_builder-0.0.8/PKG-INFO` & `typer_builder-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typer-builder
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

