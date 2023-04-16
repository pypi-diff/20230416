# Comparing `tmp/py-build-cmake-0.1.6.tar.gz` & `tmp/py-build-cmake-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-build-cmake-0.1.6.tar", last modified: Thu Apr 13 18:50:59 2023, max compression
+gzip compressed data, was "py-build-cmake-0.1.7.tar", last modified: Sun Apr 16 00:43:24 2023, max compression
```

## Comparing `py-build-cmake-0.1.6.tar` & `py-build-cmake-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1065 2023-04-13 18:50:42.637587 py-build-cmake-0.1.6/LICENSE
--rw-r--r--   0        0        0     5147 2023-04-13 18:50:42.637873 py-build-cmake-0.1.6/README.md
--rw-r--r--   0        0        0     1400 2023-04-13 18:50:42.673798 py-build-cmake-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      133 2023-04-13 18:50:42.674785 py-build-cmake-0.1.6/src/py_build_cmake/__init__.py
--rw-r--r--   0        0        0    30441 2023-04-13 18:50:42.675201 py-build-cmake-0.1.6/src/py_build_cmake/build.py
--rw-r--r--   0        0        0     9139 2023-04-13 18:50:42.675561 py-build-cmake-0.1.6/src/py_build_cmake/build_component.py
--rw-r--r--   0        0        0    10381 2023-04-13 18:50:42.675873 py-build-cmake-0.1.6/src/py_build_cmake/cli.py
--rw-r--r--   0        0        0     7896 2023-04-13 18:50:42.676179 py-build-cmake-0.1.6/src/py_build_cmake/cmake.py
--rw-r--r--   0        0        0     2393 2023-04-13 18:50:42.676452 py-build-cmake-0.1.6/src/py_build_cmake/cmd_runner.py
--rw-r--r--   0        0        0     9717 2023-04-13 18:50:42.676814 py-build-cmake-0.1.6/src/py_build_cmake/config.py
--rw-r--r--   0        0        0    28479 2023-04-13 18:50:42.677202 py-build-cmake-0.1.6/src/py_build_cmake/config_options.py
--rw-r--r--   0        0        0      289 2023-04-13 18:50:42.677518 py-build-cmake-0.1.6/src/py_build_cmake/datastructures.py
--rw-r--r--   0        0        0     4105 2023-04-13 18:50:42.677886 py-build-cmake-0.1.6/src/py_build_cmake/help/__init__.py
--rw-r--r--   0        0        0      173 2023-04-13 18:50:42.678170 py-build-cmake-0.1.6/src/py_build_cmake/help/__main__.py
--rw-r--r--   0        0        0        0 2023-04-13 18:50:42.678328 py-build-cmake-0.1.6/src/py_build_cmake/py.typed
--rw-r--r--   0        0        0    20011 2023-04-13 18:50:42.678614 py-build-cmake-0.1.6/src/py_build_cmake/pyproject_options.py
--rw-r--r--   0        0        0     2529 2023-04-13 18:50:42.678933 py-build-cmake-0.1.6/src/py_build_cmake/tags.py
--rw-r--r--   0        0        0     6305 1970-01-01 00:00:00.000000 py-build-cmake-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-16 00:43:05.473989 py-build-cmake-0.1.7/LICENSE
+-rw-r--r--   0        0        0     5147 2023-04-16 00:43:05.474225 py-build-cmake-0.1.7/README.md
+-rw-r--r--   0        0        0     1400 2023-04-16 00:43:05.527303 py-build-cmake-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      133 2023-04-16 00:43:05.528112 py-build-cmake-0.1.7/src/py_build_cmake/__init__.py
+-rw-r--r--   0        0        0    30441 2023-04-16 00:43:05.528502 py-build-cmake-0.1.7/src/py_build_cmake/build.py
+-rw-r--r--   0        0        0     9139 2023-04-16 00:43:05.528834 py-build-cmake-0.1.7/src/py_build_cmake/build_component.py
+-rw-r--r--   0        0        0    10451 2023-04-16 00:43:05.529134 py-build-cmake-0.1.7/src/py_build_cmake/cli.py
+-rw-r--r--   0        0        0     7896 2023-04-16 00:43:05.529402 py-build-cmake-0.1.7/src/py_build_cmake/cmake.py
+-rw-r--r--   0        0        0     2393 2023-04-16 00:43:05.529648 py-build-cmake-0.1.7/src/py_build_cmake/cmd_runner.py
+-rw-r--r--   0        0        0     9717 2023-04-16 00:43:05.529910 py-build-cmake-0.1.7/src/py_build_cmake/config.py
+-rw-r--r--   0        0        0    28479 2023-04-16 00:43:05.530274 py-build-cmake-0.1.7/src/py_build_cmake/config_options.py
+-rw-r--r--   0        0        0      289 2023-04-16 00:43:05.530549 py-build-cmake-0.1.7/src/py_build_cmake/datastructures.py
+-rw-r--r--   0        0        0     4105 2023-04-16 00:43:05.530872 py-build-cmake-0.1.7/src/py_build_cmake/help/__init__.py
+-rw-r--r--   0        0        0      173 2023-04-16 00:43:05.531112 py-build-cmake-0.1.7/src/py_build_cmake/help/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-16 00:43:05.531249 py-build-cmake-0.1.7/src/py_build_cmake/py.typed
+-rw-r--r--   0        0        0    20011 2023-04-16 00:43:05.531551 py-build-cmake-0.1.7/src/py_build_cmake/pyproject_options.py
+-rw-r--r--   0        0        0     2529 2023-04-16 00:43:05.531834 py-build-cmake-0.1.7/src/py_build_cmake/tags.py
+-rw-r--r--   0        0        0     6305 1970-01-01 00:00:00.000000 py-build-cmake-0.1.7/PKG-INFO
```

### Comparing `py-build-cmake-0.1.6/LICENSE` & `py-build-cmake-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `py-build-cmake-0.1.6/README.md` & `py-build-cmake-0.1.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 keywords = ["some", "keywords"]
 classifiers = ["Topic :: Scientific/Engineering"]
 urls = { "Documentation" = "https://tttapa.github.io/py-build-cmake" }
 dependencies = ["numpy"]
 dynamic = ["version", "description"]
 
 [build-system] # How pip and other frontends should build this project
-requires = ["py-build-cmake~=0.1.6"]
+requires = ["py-build-cmake~=0.1.7"]
 build-backend = "py_build_cmake.build"
 
 [tool.py-build-cmake.module] # Where to find the Python module to package
 directory = "src-python"
 
 [tool.py-build-cmake.sdist] # What to include in source distributions
 include = ["CMakeLists.txt", "src/*"]
```

### Comparing `py-build-cmake-0.1.6/pyproject.toml` & `py-build-cmake-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py-build-cmake-0.1.6/src/py_build_cmake/build.py` & `py-build-cmake-0.1.7/src/py_build_cmake/build.py`

 * *Files identical despite different names*

### Comparing `py-build-cmake-0.1.6/src/py_build_cmake/build_component.py` & `py-build-cmake-0.1.7/src/py_build_cmake/build_component.py`

 * *Files identical despite different names*

### Comparing `py-build-cmake-0.1.6/src/py_build_cmake/cli.py` & `py-build-cmake-0.1.7/src/py_build_cmake/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
     def get_cmaker():
         from .build import _BuildBackend as backend
         from .datastructures import PackageInfo
         from .cmd_runner import CommandRunner
         source_dir = Path(directory or '.').resolve()
         config_settings = {
-            "--cross": cross,
-            "--local": local,
+            "--cross": list(cross),
+            "--local": list(local),
         }
         # Read configuration and package metadata
         cfg, pkg, metadata = backend.read_all_metadata(source_dir,
                                                        config_settings,
                                                        verbose)
 
         if not cfg.cmake:
@@ -72,20 +72,22 @@
 @click.option("--native",
               is_flag=True,
               help="When the configuration requests cross-compiling, "
               "configure for a native build instead. Has no effect otherwise.")
 @click.option("--local",
               type=click.Path(exists=False, file_okay=True, dir_okay=False),
               required=False,
+              multiple=True,
               help="Specifies a toml file that overrides the "
               "tool.py-build-cmake section of pyproject.toml, "
               "similar to py-build-cmake.local.toml.")
 @click.option("--cross",
               type=click.Path(exists=False, file_okay=True, dir_okay=False),
               required=False,
+              multiple=True,
               help="Specifies a toml file that overrides the "
               "tool.py-build-cmake.cross section of pyproject.toml, "
               "similar to py-build-cmake.cross.toml.")
 @click.version_option(__version__, "-v", "--version")
 @click.pass_context
 def cli(ctx: click.Context, **kwargs):
     ctx.obj = cmake_command(**kwargs)
```

### Comparing `py-build-cmake-0.1.6/src/py_build_cmake/cmake.py` & `py-build-cmake-0.1.7/src/py_build_cmake/cmake.py`

 * *Files identical despite different names*

### Comparing `py-build-cmake-0.1.6/src/py_build_cmake/cmd_runner.py` & `py-build-cmake-0.1.7/src/py_build_cmake/cmd_runner.py`

 * *Files identical despite different names*

### Comparing `py-build-cmake-0.1.6/src/py_build_cmake/config.py` & `py-build-cmake-0.1.7/src/py_build_cmake/config.py`

 * *Files identical despite different names*

### Comparing `py-build-cmake-0.1.6/src/py_build_cmake/config_options.py` & `py-build-cmake-0.1.7/src/py_build_cmake/config_options.py`

 * *Files identical despite different names*

### Comparing `py-build-cmake-0.1.6/src/py_build_cmake/help/__init__.py` & `py-build-cmake-0.1.7/src/py_build_cmake/help/__init__.py`

 * *Files identical despite different names*

### Comparing `py-build-cmake-0.1.6/src/py_build_cmake/pyproject_options.py` & `py-build-cmake-0.1.7/src/py_build_cmake/pyproject_options.py`

 * *Files identical despite different names*

### Comparing `py-build-cmake-0.1.6/src/py_build_cmake/tags.py` & `py-build-cmake-0.1.7/src/py_build_cmake/tags.py`

 * *Files identical despite different names*

### Comparing `py-build-cmake-0.1.6/PKG-INFO` & `py-build-cmake-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-build-cmake
-Version: 0.1.6
+Version: 0.1.7
 Summary: Modern, PEP 517 compliant build backend for creating Python packages with
 Keywords: pep517,cmake
 Author-email: Pieter P <pieter.p.dev@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -86,15 +86,15 @@
 keywords = ["some", "keywords"]
 classifiers = ["Topic :: Scientific/Engineering"]
 urls = { "Documentation" = "https://tttapa.github.io/py-build-cmake" }
 dependencies = ["numpy"]
 dynamic = ["version", "description"]
 
 [build-system] # How pip and other frontends should build this project
-requires = ["py-build-cmake~=0.1.6"]
+requires = ["py-build-cmake~=0.1.7"]
 build-backend = "py_build_cmake.build"
 
 [tool.py-build-cmake.module] # Where to find the Python module to package
 directory = "src-python"
 
 [tool.py-build-cmake.sdist] # What to include in source distributions
 include = ["CMakeLists.txt", "src/*"]
```

