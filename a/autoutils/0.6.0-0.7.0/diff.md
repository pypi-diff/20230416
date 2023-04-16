# Comparing `tmp/autoutils-0.6.0.tar.gz` & `tmp/autoutils-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoutils-0.6.0.tar", max compression
+gzip compressed data, was "autoutils-0.7.0.tar", max compression
```

## Comparing `autoutils-0.6.0.tar` & `autoutils-0.7.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1067 2021-11-26 12:10:42.533080 autoutils-0.6.0/LICENSE
--rw-r--r--   0        0        0       11 2021-11-26 12:10:42.533080 autoutils-0.6.0/README.md
--rw-r--r--   0        0        0        0 2021-11-26 12:10:42.533080 autoutils-0.6.0/autoutils/__init__.py
--rw-r--r--   0        0        0     3689 2021-11-26 12:10:42.533080 autoutils-0.6.0/autoutils/api.py
--rw-r--r--   0        0        0     8739 2022-01-21 08:17:11.564216 autoutils-0.6.0/autoutils/color.py
--rw-r--r--   0        0        0     3411 2022-03-16 04:58:09.024977 autoutils-0.6.0/autoutils/file.py
--rw-r--r--   0        0        0    19290 2023-02-01 15:50:59.518146 autoutils-0.6.0/autoutils/log.py
--rw-r--r--   0        0        0        0 2022-01-30 10:00:59.513000 autoutils-0.6.0/autoutils/matrixcli/__init__.py
--rw-r--r--   0        0        0    35272 2022-01-30 12:33:26.416456 autoutils-0.6.0/autoutils/matrixcli/api.py
--rw-r--r--   0        0        0     7437 2022-01-30 12:33:26.160457 autoutils-0.6.0/autoutils/matrixcli/client.py
--rw-r--r--   0        0        0     1765 2022-01-30 10:00:59.513000 autoutils-0.6.0/autoutils/matrixcli/errors.py
--rw-r--r--   0        0        0    24836 2022-01-30 10:00:59.513000 autoutils-0.6.0/autoutils/matrixcli/room.py
--rw-r--r--   0        0        0     1509 2022-01-30 10:00:59.513000 autoutils-0.6.0/autoutils/matrixcli/user.py
--rw-r--r--   0        0        0     3253 2022-01-03 22:44:46.832714 autoutils-0.6.0/autoutils/redis.py
--rw-r--r--   0        0        0     4243 2023-02-01 13:54:48.920005 autoutils-0.6.0/autoutils/script.py
--rw-r--r--   0        0        0    12163 2022-01-30 12:31:32.712461 autoutils-0.6.0/autoutils/server.py
--rw-r--r--   0        0        0     5889 2022-12-15 16:38:35.642334 autoutils-0.6.0/autoutils/thread.py
--rw-r--r--   0        0        0      784 2023-02-01 15:52:15.182474 autoutils-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      869 1970-01-01 00:00:00.000000 autoutils-0.6.0/setup.py
--rw-r--r--   0        0        0     1152 1970-01-01 00:00:00.000000 autoutils-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2021-11-26 12:10:42.533080 autoutils-0.7.0/LICENSE
+-rw-r--r--   0        0        0       11 2021-11-26 12:10:42.533080 autoutils-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2021-11-26 12:10:42.533080 autoutils-0.7.0/autoutils/__init__.py
+-rw-r--r--   0        0        0     3689 2021-11-26 12:10:42.533080 autoutils-0.7.0/autoutils/api.py
+-rw-r--r--   0        0        0     8739 2022-01-21 08:17:11.564216 autoutils-0.7.0/autoutils/color.py
+-rw-r--r--   0        0        0     3411 2022-03-16 04:58:09.024977 autoutils-0.7.0/autoutils/file.py
+-rw-r--r--   0        0        0    19290 2023-02-01 15:50:59.518146 autoutils-0.7.0/autoutils/log.py
+-rw-r--r--   0        0        0        0 2022-01-30 10:00:59.513000 autoutils-0.7.0/autoutils/matrixcli/__init__.py
+-rw-r--r--   0        0        0    35272 2022-01-30 12:33:26.416456 autoutils-0.7.0/autoutils/matrixcli/api.py
+-rw-r--r--   0        0        0     7437 2022-01-30 12:33:26.160457 autoutils-0.7.0/autoutils/matrixcli/client.py
+-rw-r--r--   0        0        0     1765 2022-01-30 10:00:59.513000 autoutils-0.7.0/autoutils/matrixcli/errors.py
+-rw-r--r--   0        0        0    24836 2022-01-30 10:00:59.513000 autoutils-0.7.0/autoutils/matrixcli/room.py
+-rw-r--r--   0        0        0     1509 2022-01-30 10:00:59.513000 autoutils-0.7.0/autoutils/matrixcli/user.py
+-rw-r--r--   0        0        0     3253 2022-01-03 22:44:46.832714 autoutils-0.7.0/autoutils/redis.py
+-rw-r--r--   0        0        0     4243 2023-02-01 13:54:48.920005 autoutils-0.7.0/autoutils/script.py
+-rw-r--r--   0        0        0    12163 2022-01-30 12:31:32.712461 autoutils-0.7.0/autoutils/server.py
+-rw-r--r--   0        0        0     6437 2023-04-16 05:46:21.738135 autoutils-0.7.0/autoutils/thread.py
+-rw-r--r--   0        0        0      784 2023-04-16 05:47:03.462303 autoutils-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      869 1970-01-01 00:00:00.000000 autoutils-0.7.0/setup.py
+-rw-r--r--   0        0        0     1152 1970-01-01 00:00:00.000000 autoutils-0.7.0/PKG-INFO
```

### Comparing `autoutils-0.6.0/LICENSE` & `autoutils-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autoutils-0.6.0/autoutils/api.py` & `autoutils-0.7.0/autoutils/api.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.6.0/autoutils/color.py` & `autoutils-0.7.0/autoutils/color.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.6.0/autoutils/file.py` & `autoutils-0.7.0/autoutils/file.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.6.0/autoutils/log.py` & `autoutils-0.7.0/autoutils/log.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.6.0/autoutils/matrixcli/api.py` & `autoutils-0.7.0/autoutils/matrixcli/api.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.6.0/autoutils/matrixcli/client.py` & `autoutils-0.7.0/autoutils/matrixcli/client.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.6.0/autoutils/matrixcli/errors.py` & `autoutils-0.7.0/autoutils/matrixcli/errors.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.6.0/autoutils/matrixcli/room.py` & `autoutils-0.7.0/autoutils/matrixcli/room.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.6.0/autoutils/matrixcli/user.py` & `autoutils-0.7.0/autoutils/matrixcli/user.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.6.0/autoutils/redis.py` & `autoutils-0.7.0/autoutils/redis.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.6.0/autoutils/script.py` & `autoutils-0.7.0/autoutils/script.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.6.0/autoutils/server.py` & `autoutils-0.7.0/autoutils/server.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.6.0/autoutils/thread.py` & `autoutils-0.7.0/autoutils/thread.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 __author__ = ('Reza Zeiny <rezazeiny1998@gmail.com>',)
 
 import logging
 import multiprocessing
 from concurrent.futures.thread import ThreadPoolExecutor
 from datetime import datetime
-from queue import Queue
+from queue import Queue, Empty
 from threading import Thread, Lock
 
 from func_timeout import func_timeout
 from func_timeout.exceptions import FunctionTimedOut
 
 logger = logging.getLogger(__name__)
 
@@ -30,16 +30,20 @@
         self.daemon = True
         self.start()
 
     def run(self):
         """
             Run
         """
-        while True:
-            task_detail, func, args, kwargs = self.pool.tasks.get()
+        logger.info(f"Start worker {self.name}")
+        while self.pool.get_running():
+            try:
+                task_detail, func, args, kwargs = self.pool.tasks.get(timeout=1)
+            except Empty:
+                continue
             task_id = task_detail["id"]
             timeout = None
             if type(func) == tuple:
                 func, timeout = func
             task_detail["start_dt"] = datetime.now()
             self.is_working = True
             if not callable(func):
@@ -64,14 +68,15 @@
                 self.pool.tasks.task_done()
                 logger.debug(f"Finish running function {func.__name__} in thread {self.name}.")
                 task_detail["end_dt"] = datetime.now()
                 duration = task_detail["end_dt"] - task_detail["insert_dt"]
                 if self.pool.log_detail:
                     logger.info(f"Task {task_id} Complete in {self.name} in {duration}")
             self.is_working = False
+        logger.info(f"Terminate worker {self.name}")
 
 
 class ThreadPool:
     """
         Pool of threads consuming tasks from a queue
     """
 
@@ -81,38 +86,49 @@
         self.name = name
         self.tasks_data = {}
         self.save_detail = save_detail
         self.log_detail = log_detail
         self.tasks_mutex = Lock()
         logger.info(f"{self.name} Create {worker_count} Worker With MAX_QUEUE: {total_queue}")
         self.workers = []
+        self._running = True
         for index in range(worker_count):
             self.workers.append(Worker(self, index=index))
 
+    def get_running(self):
+        return self._running
+
+    def _check_running(self):
+        if not self._running:
+            raise Exception("the threadpool stopped")
+
     def add_task(self, func, *args, **kargs) -> int:
         """Add a task to the queue"""
-        self.tasks_mutex.acquire()
-        task_id = len(self.tasks_data.keys()) + 1
-        task_detail = {
-            "id": task_id,
-            "status": "pending",
-            "insert_dt": datetime.now()
-        }
-        if self.save_detail:
-            self.tasks_data[task_id] = task_detail
+        self._check_running()
+        with self.tasks_mutex:
+            task_id = len(self.tasks_data.keys()) + 1
+            task_detail = {
+                "id": task_id,
+                "status": "pending",
+                "insert_dt": datetime.now()
+            }
+            if self.save_detail:
+                self.tasks_data[task_id] = task_detail
 
-        self.tasks.put((task_detail, func, args, kargs))
-        self.tasks_mutex.release()
+            self.tasks.put((task_detail, func, args, kargs))
         return task_id
 
-    def wait_completion(self):
+    def wait_completion(self, terminate: bool = False):
         """
             Wait for completion of all the tasks in the queue
         """
+        self._check_running()
         self.tasks.join()
+        if terminate:
+            self._running = False
 
     def get_task_data(self, task_id: int) -> dict:
         """
             Get task data
         """
         return self.tasks_data.get(task_id)
```

### Comparing `autoutils-0.6.0/pyproject.toml` & `autoutils-0.7.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoutils"
-version = "0.6.0"
+version = "0.7.0"
 description = "Some Good Function"
 authors = ["Reza Zeiny <rezazeiny1998@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rezazeiny/autoutils"
 repository = "https://github.com/rezazeiny/autoutils"
 keywords = ["autoutils"]
```

### Comparing `autoutils-0.6.0/setup.py` & `autoutils-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'redis>=4.0,<5.0',
  'requests>=2.0,<3.0',
  'sshtunnel>=0.1,<1.0',
  'urllib3>=1.0,<2.0']
 
 setup_kwargs = {
     'name': 'autoutils',
-    'version': '0.6.0',
+    'version': '0.7.0',
     'description': 'Some Good Function',
     'long_description': '# autoutils',
     'author': 'Reza Zeiny',
     'author_email': 'rezazeiny1998@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/rezazeiny/autoutils',
```

### Comparing `autoutils-0.6.0/PKG-INFO` & `autoutils-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoutils
-Version: 0.6.0
+Version: 0.7.0
 Summary: Some Good Function
 Home-page: https://github.com/rezazeiny/autoutils
 License: MIT
 Keywords: autoutils
 Author: Reza Zeiny
 Author-email: rezazeiny1998@gmail.com
 Requires-Python: >=3.6,<4.0
```

