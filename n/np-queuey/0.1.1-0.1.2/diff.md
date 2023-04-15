# Comparing `tmp/np_queuey-0.1.1.tar.gz` & `tmp/np_queuey-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_queuey-0.1.1.tar", last modified: Sat Apr 15 00:22:18 2023, max compression
+gzip compressed data, was "np_queuey-0.1.2.tar", last modified: Sat Apr 15 22:58:32 2023, max compression
```

## Comparing `np_queuey-0.1.1.tar` & `np_queuey-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      227 2023-04-13 16:35:48.733260 np_queuey-0.1.1/README.md
--rw-r--r--   0        0        0     2357 2023-04-15 00:22:18.421726 np_queuey-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       73 2023-04-13 23:41:50.797573 np_queuey-0.1.1/src/np_queuey/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.1.1/src/np_queuey/hueys/__init__.py
--rw-r--r--   0        0        0     8490 2023-04-15 00:21:39.512663 np_queuey-0.1.1/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py
--rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.1.1/src/np_queuey/jobs/__init__.py
--rw-r--r--   0        0        0     6771 2023-04-15 00:21:38.677120 np_queuey-0.1.1/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py
--rw-r--r--   0        0        0      245 2023-04-15 00:21:39.508662 np_queuey-0.1.1/src/np_queuey/jobs/run_small_jobs.py
--rw-r--r--   0        0        0     3019 2023-04-13 23:41:51.924236 np_queuey-0.1.1/src/np_queuey/queues.py
--rw-r--r--   0        0        0       51 2023-04-13 23:41:50.828823 np_queuey-0.1.1/src/np_queuey/tasks.py
--rw-r--r--   0        0        0      140 2023-04-15 00:21:38.620120 np_queuey-0.1.1/src/np_queuey/utils.py
--rw-r--r--   0        0        0      593 2023-04-13 20:34:38.147095 np_queuey-0.1.1/tests/test_huey.py
--rw-r--r--   0        0        0     1668 1970-01-01 00:00:00.000000 np_queuey-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      227 2023-04-13 16:35:48.733260 np_queuey-0.1.2/README.md
+-rw-r--r--   0        0        0     2365 2023-04-15 22:58:32.469679 np_queuey-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-04-13 23:41:50.797573 np_queuey-0.1.2/src/np_queuey/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.1.2/src/np_queuey/hueys/__init__.py
+-rw-r--r--   0        0        0     8523 2023-04-15 22:58:13.363400 np_queuey-0.1.2/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.1.2/src/np_queuey/jobs/__init__.py
+-rw-r--r--   0        0        0     6771 2023-04-15 00:21:38.677120 np_queuey-0.1.2/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py
+-rw-r--r--   0        0        0      262 2023-04-15 22:53:44.311082 np_queuey-0.1.2/src/np_queuey/jobs/run_small_jobs.py
+-rw-r--r--   0        0        0     3019 2023-04-13 23:41:51.924236 np_queuey-0.1.2/src/np_queuey/queues.py
+-rw-r--r--   0        0        0       51 2023-04-13 23:41:50.828823 np_queuey-0.1.2/src/np_queuey/tasks.py
+-rw-r--r--   0        0        0      140 2023-04-15 00:21:38.620120 np_queuey-0.1.2/src/np_queuey/utils.py
+-rw-r--r--   0        0        0      593 2023-04-13 20:34:38.147095 np_queuey-0.1.2/tests/test_huey.py
+-rw-r--r--   0        0        0     1668 1970-01-01 00:00:00.000000 np_queuey-0.1.2/PKG-INFO
```

### Comparing `np_queuey-0.1.1/pyproject.toml` & `np_queuey-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "np_queuey"
-version = "0.1.1"
+version = "0.1.2"
 description = "Tools for submitting and processing jobs through a message queue for Mindscope Neuropixels workflows."
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "huey>=2.4.5",
     "np-config>=0.4.17",
@@ -54,15 +54,15 @@
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm.scripts]
 ruff = "ruff --fix src"
 blue = "blue src"
 pytest = "pytest --cov"
-bump = "pdm bump patch"
+bump = "bump -p pyproject.toml"
 
 [tool.pdm.scripts.prebuild]
 composite = [
     "blue",
     "ruff",
     "pytest",
 ]
```

### Comparing `np_queuey-0.1.1/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py` & `np_queuey-0.1.2/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,18 +51,20 @@
     write_input_json(foraging_id_and_filename)
     write_shell_script(foraging_id_and_filename)
     with np_tools.ssh('hpc-login') as ssh:
         logger.debug(
             'Launching mtrain_lims on hpc for %s', foraging_id_and_filename
         )
         ssh.run(hpc_cmd(foraging_id_and_filename))
-    verify_behavior_session_uploaded(foraging_id_and_filename)
+    verify_behavior_session_uploaded.schedule(
+        foraging_id_and_filename, delay=60
+    )
 
 
-@huey.task(retry_delay=20, retries=3)
+@huey.task(retry_delay=60, retries=3)
 def verify_behavior_session_uploaded(
     foraging_id_and_filename: tuple[str, str]
 ) -> None:
     _, output_json = input_output_jsons(foraging_id_and_filename)
 
     if not np_config.normalize_path(output_json).exists():
         msg = f'{output_json} does not exist'
```

### Comparing `np_queuey-0.1.1/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py` & `np_queuey-0.1.2/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.1.1/src/np_queuey/queues.py` & `np_queuey-0.1.2/src/np_queuey/queues.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.1.1/tests/test_huey.py` & `np_queuey-0.1.2/tests/test_huey.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.1.1/PKG-INFO` & `np_queuey-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-queuey
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tools for submitting and processing jobs through a message queue for Mindscope Neuropixels workflows.
 Author-Email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

