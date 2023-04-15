# Comparing `tmp/algo-ops-0.0.1.6.8.tar.gz` & `tmp/algo-ops-0.0.1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algo-ops-0.0.1.6.8.tar", last modified: Sun Mar 19 19:56:03 2023, max compression
+gzip compressed data, was "algo-ops-0.0.1.6.9.tar", last modified: Sat Apr 15 23:54:31 2023, max compression
```

## Comparing `algo-ops-0.0.1.6.8.tar` & `algo-ops-0.0.1.6.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-03-19 19:56:03.846059 algo-ops-0.0.1.6.8/
--rw-r--r--   0 tandonp    (501) staff       (20)     1071 2022-03-24 04:58:29.000000 algo-ops-0.0.1.6.8/LICENSE
--rw-r--r--   0 tandonp    (501) staff       (20)       24 2022-03-21 02:23:19.000000 algo-ops-0.0.1.6.8/MANIFEST.in
--rw-r--r--   0 tandonp    (501) staff       (20)     2534 2023-03-19 19:56:03.845867 algo-ops-0.0.1.6.8/PKG-INFO
--rw-r--r--   0 tandonp    (501) staff       (20)     2083 2022-06-03 05:15:50.000000 algo-ops-0.0.1.6.8/README.md
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-03-19 19:56:03.842216 algo-ops-0.0.1.6.8/algo_ops/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-09 07:46:32.000000 algo-ops-0.0.1.6.8/algo_ops/__init__.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-03-19 19:56:03.843762 algo-ops-0.0.1.6.8/algo_ops/dependency/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-13 23:06:19.000000 algo-ops-0.0.1.6.8/algo_ops/dependency/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)     2460 2023-03-19 19:09:30.000000 algo-ops-0.0.1.6.8/algo_ops/dependency/sys_util.py
--rw-r--r--   0 tandonp    (501) staff       (20)     5315 2023-03-19 19:10:06.000000 algo-ops-0.0.1.6.8/algo_ops/dependency/tester_util.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-03-19 19:56:03.844503 algo-ops-0.0.1.6.8/algo_ops/ops/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-13 23:06:19.000000 algo-ops-0.0.1.6.8/algo_ops/ops/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)     5477 2023-03-19 19:44:28.000000 algo-ops-0.0.1.6.8/algo_ops/ops/cv.py
--rw-r--r--   0 tandonp    (501) staff       (20)     7026 2023-03-19 19:09:12.000000 algo-ops-0.0.1.6.8/algo_ops/ops/op.py
--rw-r--r--   0 tandonp    (501) staff       (20)       19 2022-06-08 03:22:52.000000 algo-ops-0.0.1.6.8/algo_ops/ops/settings.py
--rw-r--r--   0 tandonp    (501) staff       (20)     2213 2022-06-08 03:22:52.000000 algo-ops-0.0.1.6.8/algo_ops/ops/text.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-03-19 19:56:03.844758 algo-ops-0.0.1.6.8/algo_ops/paraloop/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-02-28 05:34:12.000000 algo-ops-0.0.1.6.8/algo_ops/paraloop/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)     1669 2022-06-03 07:00:28.000000 algo-ops-0.0.1.6.8/algo_ops/paraloop/paraloop.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-03-19 19:56:03.845021 algo-ops-0.0.1.6.8/algo_ops/pickleable_object/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-09 07:46:32.000000 algo-ops-0.0.1.6.8/algo_ops/pickleable_object/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)      760 2023-03-19 19:11:09.000000 algo-ops-0.0.1.6.8/algo_ops/pickleable_object/pickleable_object.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-03-19 19:56:03.845414 algo-ops-0.0.1.6.8/algo_ops/pipeline/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-13 23:06:19.000000 algo-ops-0.0.1.6.8/algo_ops/pipeline/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)     3396 2023-03-19 19:11:29.000000 algo-ops-0.0.1.6.8/algo_ops/pipeline/cv_pipeline.py
--rw-r--r--   0 tandonp    (501) staff       (20)     7637 2023-03-19 19:13:35.000000 algo-ops-0.0.1.6.8/algo_ops/pipeline/pipeline.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-03-19 19:56:03.845673 algo-ops-0.0.1.6.8/algo_ops/plot/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-13 23:06:19.000000 algo-ops-0.0.1.6.8/algo_ops/plot/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)     2080 2023-03-19 19:14:03.000000 algo-ops-0.0.1.6.8/algo_ops/plot/plot.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-03-19 19:56:03.843285 algo-ops-0.0.1.6.8/algo_ops.egg-info/
--rw-r--r--   0 tandonp    (501) staff       (20)     2534 2023-03-19 19:56:03.000000 algo-ops-0.0.1.6.8/algo_ops.egg-info/PKG-INFO
--rw-r--r--   0 tandonp    (501) staff       (20)      746 2023-03-19 19:56:03.000000 algo-ops-0.0.1.6.8/algo_ops.egg-info/SOURCES.txt
--rw-r--r--   0 tandonp    (501) staff       (20)        1 2023-03-19 19:56:03.000000 algo-ops-0.0.1.6.8/algo_ops.egg-info/dependency_links.txt
--rw-r--r--   0 tandonp    (501) staff       (20)       75 2023-03-19 19:56:03.000000 algo-ops-0.0.1.6.8/algo_ops.egg-info/requires.txt
--rw-r--r--   0 tandonp    (501) staff       (20)        9 2023-03-19 19:56:03.000000 algo-ops-0.0.1.6.8/algo_ops.egg-info/top_level.txt
--rw-r--r--   0 tandonp    (501) staff       (20)      195 2023-03-19 19:54:12.000000 algo-ops-0.0.1.6.8/pyproject.toml
--rw-r--r--   0 tandonp    (501) staff       (20)       74 2023-03-18 06:13:49.000000 algo-ops-0.0.1.6.8/requirements.txt
--rw-r--r--   0 tandonp    (501) staff       (20)       38 2023-03-19 19:56:03.846116 algo-ops-0.0.1.6.8/setup.cfg
--rw-r--r--   0 tandonp    (501) staff       (20)      789 2023-03-19 19:52:38.000000 algo-ops-0.0.1.6.8/setup.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-15 23:54:31.603409 algo-ops-0.0.1.6.9/
+-rw-r--r--   0 tandonp    (501) staff       (20)     1071 2022-03-24 04:58:29.000000 algo-ops-0.0.1.6.9/LICENSE
+-rw-r--r--   0 tandonp    (501) staff       (20)       24 2022-03-21 02:23:19.000000 algo-ops-0.0.1.6.9/MANIFEST.in
+-rw-r--r--   0 tandonp    (501) staff       (20)     2534 2023-04-15 23:54:31.603244 algo-ops-0.0.1.6.9/PKG-INFO
+-rw-r--r--   0 tandonp    (501) staff       (20)     2083 2022-06-03 05:15:50.000000 algo-ops-0.0.1.6.9/README.md
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-15 23:54:31.599842 algo-ops-0.0.1.6.9/algo_ops/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-09 07:46:32.000000 algo-ops-0.0.1.6.9/algo_ops/__init__.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-15 23:54:31.601102 algo-ops-0.0.1.6.9/algo_ops/dependency/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-13 23:06:19.000000 algo-ops-0.0.1.6.9/algo_ops/dependency/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     2460 2023-03-19 19:09:30.000000 algo-ops-0.0.1.6.9/algo_ops/dependency/sys_util.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     5315 2023-03-19 19:10:06.000000 algo-ops-0.0.1.6.9/algo_ops/dependency/tester_util.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-15 23:54:31.601794 algo-ops-0.0.1.6.9/algo_ops/ops/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-13 23:06:19.000000 algo-ops-0.0.1.6.9/algo_ops/ops/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     5477 2023-03-19 19:44:28.000000 algo-ops-0.0.1.6.9/algo_ops/ops/cv.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     7026 2023-03-19 19:09:12.000000 algo-ops-0.0.1.6.9/algo_ops/ops/op.py
+-rw-r--r--   0 tandonp    (501) staff       (20)       19 2022-06-08 03:22:52.000000 algo-ops-0.0.1.6.9/algo_ops/ops/settings.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     2213 2022-06-08 03:22:52.000000 algo-ops-0.0.1.6.9/algo_ops/ops/text.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-15 23:54:31.602074 algo-ops-0.0.1.6.9/algo_ops/paraloop/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-02-28 05:34:12.000000 algo-ops-0.0.1.6.9/algo_ops/paraloop/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     1911 2023-04-15 23:53:29.000000 algo-ops-0.0.1.6.9/algo_ops/paraloop/paraloop.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-15 23:54:31.602361 algo-ops-0.0.1.6.9/algo_ops/pickleable_object/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-09 07:46:32.000000 algo-ops-0.0.1.6.9/algo_ops/pickleable_object/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)      760 2023-03-19 19:11:09.000000 algo-ops-0.0.1.6.9/algo_ops/pickleable_object/pickleable_object.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-15 23:54:31.602776 algo-ops-0.0.1.6.9/algo_ops/pipeline/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-13 23:06:19.000000 algo-ops-0.0.1.6.9/algo_ops/pipeline/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     3396 2023-03-19 19:11:29.000000 algo-ops-0.0.1.6.9/algo_ops/pipeline/cv_pipeline.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     7637 2023-03-19 19:13:35.000000 algo-ops-0.0.1.6.9/algo_ops/pipeline/pipeline.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-15 23:54:31.603054 algo-ops-0.0.1.6.9/algo_ops/plot/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-13 23:06:19.000000 algo-ops-0.0.1.6.9/algo_ops/plot/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     2080 2023-03-19 19:14:03.000000 algo-ops-0.0.1.6.9/algo_ops/plot/plot.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-15 23:54:31.600684 algo-ops-0.0.1.6.9/algo_ops.egg-info/
+-rw-r--r--   0 tandonp    (501) staff       (20)     2534 2023-04-15 23:54:31.000000 algo-ops-0.0.1.6.9/algo_ops.egg-info/PKG-INFO
+-rw-r--r--   0 tandonp    (501) staff       (20)      746 2023-04-15 23:54:31.000000 algo-ops-0.0.1.6.9/algo_ops.egg-info/SOURCES.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)        1 2023-04-15 23:54:31.000000 algo-ops-0.0.1.6.9/algo_ops.egg-info/dependency_links.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)       75 2023-04-15 23:54:31.000000 algo-ops-0.0.1.6.9/algo_ops.egg-info/requires.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)        9 2023-04-15 23:54:31.000000 algo-ops-0.0.1.6.9/algo_ops.egg-info/top_level.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)      195 2023-03-19 19:54:12.000000 algo-ops-0.0.1.6.9/pyproject.toml
+-rw-r--r--   0 tandonp    (501) staff       (20)       74 2023-03-18 06:13:49.000000 algo-ops-0.0.1.6.9/requirements.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)       38 2023-04-15 23:54:31.603458 algo-ops-0.0.1.6.9/setup.cfg
+-rw-r--r--   0 tandonp    (501) staff       (20)      789 2023-04-15 23:54:21.000000 algo-ops-0.0.1.6.9/setup.py
```

### Comparing `algo-ops-0.0.1.6.8/LICENSE` & `algo-ops-0.0.1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `algo-ops-0.0.1.6.8/PKG-INFO` & `algo-ops-0.0.1.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algo-ops
-Version: 0.0.1.6.8
+Version: 0.0.1.6.9
 Summary: Algo-Ops Algorithm Prototyping Framework
 Home-page: https://github.com/prateekt/algo-ops
 Author: Prateek Tandon
 Author-email: prateek1.tandon@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `algo-ops-0.0.1.6.8/README.md` & `algo-ops-0.0.1.6.9/README.md`

 * *Files identical despite different names*

### Comparing `algo-ops-0.0.1.6.8/algo_ops/dependency/sys_util.py` & `algo-ops-0.0.1.6.9/algo_ops/dependency/sys_util.py`

 * *Files identical despite different names*

### Comparing `algo-ops-0.0.1.6.8/algo_ops/dependency/tester_util.py` & `algo-ops-0.0.1.6.9/algo_ops/dependency/tester_util.py`

 * *Files identical despite different names*

### Comparing `algo-ops-0.0.1.6.8/algo_ops/ops/cv.py` & `algo-ops-0.0.1.6.9/algo_ops/ops/cv.py`

 * *Files identical despite different names*

### Comparing `algo-ops-0.0.1.6.8/algo_ops/ops/op.py` & `algo-ops-0.0.1.6.9/algo_ops/ops/op.py`

 * *Files identical despite different names*

### Comparing `algo-ops-0.0.1.6.8/algo_ops/ops/text.py` & `algo-ops-0.0.1.6.9/algo_ops/ops/text.py`

 * *Files identical despite different names*

### Comparing `algo-ops-0.0.1.6.8/algo_ops/paraloop/paraloop.py` & `algo-ops-0.0.1.6.9/algo_ops/paraloop/paraloop.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import multiprocessing
-from typing import Callable, List, Any, Sequence
+from typing import Callable, List, Any, Sequence, Optional
 
 
 def _sequential(
     func: Callable, params: Sequence[Any], debug: bool = False
 ) -> List[Any]:
     """
     Sequentially runs a function.
@@ -20,39 +20,51 @@
         if debug:
             print(param)
         result = func(param)
         results.append(result)
     return results
 
 
-def _pool(func: Callable, params: Sequence[Any]) -> List[Any]:
+def _pool(
+    func: Callable, params: Sequence[Any], num_cores: Optional[int] = None
+) -> List[Any]:
     """
     Implements paraloop using multiprocessing pool.
 
     param func: The function to parallelize
     param params: Inputs to function
+    param num_cores: Number of cores to use
+
     return:
         Results of function executions
     """
-    num_cores = multiprocessing.cpu_count()
+    if num_cores is None:
+        num_cores = multiprocessing.cpu_count()
     with multiprocessing.Pool(num_cores) as p:
         return p.map(func, params)
 
 
-def loop(func: Callable, params: Sequence[Any], mechanism: str = "pool") -> List[Any]:
+def loop(
+    func: Callable,
+    params: Sequence[Any],
+    mechanism: str = "pool",
+    num_cores: Optional[int] = None,
+) -> List[Any]:
     """
     Executes function calls with list of parameters using specified mechanism.
 
     param func: The function
     param params: The parameters to use
     param mechanism: The mechanism
+    param num_cores: Number of cores to use
+
     return:
         Results of function executions
     """
     if mechanism == "pool":
-        return _pool(func=func, params=params)
+        return _pool(func=func, params=params, num_cores=num_cores)
     elif mechanism == "sequential":
         return _sequential(func=func, params=params, debug=False)
     elif mechanism == "debug":
         return _sequential(func=func, params=params, debug=True)
     else:
         raise ValueError("Unsupported mechanism: " + str(mechanism))
```

### Comparing `algo-ops-0.0.1.6.8/algo_ops/pickleable_object/pickleable_object.py` & `algo-ops-0.0.1.6.9/algo_ops/pickleable_object/pickleable_object.py`

 * *Files identical despite different names*

### Comparing `algo-ops-0.0.1.6.8/algo_ops/pipeline/cv_pipeline.py` & `algo-ops-0.0.1.6.9/algo_ops/pipeline/cv_pipeline.py`

 * *Files identical despite different names*

### Comparing `algo-ops-0.0.1.6.8/algo_ops/pipeline/pipeline.py` & `algo-ops-0.0.1.6.9/algo_ops/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `algo-ops-0.0.1.6.8/algo_ops/plot/plot.py` & `algo-ops-0.0.1.6.9/algo_ops/plot/plot.py`

 * *Files identical despite different names*

### Comparing `algo-ops-0.0.1.6.8/algo_ops.egg-info/PKG-INFO` & `algo-ops-0.0.1.6.9/algo_ops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algo-ops
-Version: 0.0.1.6.8
+Version: 0.0.1.6.9
 Summary: Algo-Ops Algorithm Prototyping Framework
 Home-page: https://github.com/prateekt/algo-ops
 Author: Prateek Tandon
 Author-email: prateek1.tandon@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `algo-ops-0.0.1.6.8/algo_ops.egg-info/SOURCES.txt` & `algo-ops-0.0.1.6.9/algo_ops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `algo-ops-0.0.1.6.8/setup.py` & `algo-ops-0.0.1.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setuptools.setup(
     name="algo-ops",
-    version="0.0.1.6.8",
+    version="0.0.1.6.9",
     author="Prateek Tandon",
     author_email="prateek1.tandon@gmail.com",
     description="Algo-Ops Algorithm Prototyping Framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/prateekt/algo-ops",
     packages=setuptools.find_packages(),
```

