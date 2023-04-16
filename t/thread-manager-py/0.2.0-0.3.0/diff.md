# Comparing `tmp/thread-manager-py-0.2.0.tar.gz` & `tmp/thread-manager-py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thread-manager-py-0.2.0.tar", last modified: Sat Apr  8 02:26:47 2023, max compression
+gzip compressed data, was "thread-manager-py-0.3.0.tar", last modified: Sun Apr 16 15:22:06 2023, max compression
```

## Comparing `thread-manager-py-0.2.0.tar` & `thread-manager-py-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 raynor     (501) staff       (20)        0 2023-04-08 02:26:47.457311 thread-manager-py-0.2.0/
--rw-r--r--   0 raynor     (501) staff       (20)     1072 2023-04-05 03:36:31.000000 thread-manager-py-0.2.0/LICENSE
--rw-r--r--   0 raynor     (501) staff       (20)       58 2023-04-05 05:54:07.000000 thread-manager-py-0.2.0/MANIFEST.in
--rw-r--r--   0 raynor     (501) staff       (20)     3196 2023-04-08 02:26:47.457360 thread-manager-py-0.2.0/PKG-INFO
--rw-r--r--   0 raynor     (501) staff       (20)     2553 2023-04-08 02:20:26.000000 thread-manager-py-0.2.0/README.md
-drwxr-xr-x   0 raynor     (501) staff       (20)        0 2023-04-08 02:26:47.455061 thread-manager-py-0.2.0/pool_manager/
--rw-r--r--   0 raynor     (501) staff       (20)      174 2023-04-07 11:25:51.000000 thread-manager-py-0.2.0/pool_manager/__init__.py
--rw-r--r--   0 raynor     (501) staff       (20)     2679 2023-04-08 02:05:57.000000 thread-manager-py-0.2.0/pool_manager/manager.py
--rw-r--r--   0 raynor     (501) staff       (20)        0 2023-04-05 05:38:12.000000 thread-manager-py-0.2.0/requirements.txt
--rw-r--r--   0 raynor     (501) staff       (20)       79 2023-04-08 02:26:47.457538 thread-manager-py-0.2.0/setup.cfg
--rw-r--r--   0 raynor     (501) staff       (20)      879 2023-04-08 02:22:52.000000 thread-manager-py-0.2.0/setup.py
-drwxr-xr-x   0 raynor     (501) staff       (20)        0 2023-04-08 02:26:47.455301 thread-manager-py-0.2.0/tests/
--rw-r--r--   0 raynor     (501) staff       (20)     5648 2023-04-08 02:18:23.000000 thread-manager-py-0.2.0/tests/test_package.py
-drwxr-xr-x   0 raynor     (501) staff       (20)        0 2023-04-08 02:26:47.456473 thread-manager-py-0.2.0/thread_manager/
--rw-r--r--   0 raynor     (501) staff       (20)      281 2023-04-06 06:21:25.000000 thread-manager-py-0.2.0/thread_manager/__init__.py
--rw-r--r--   0 raynor     (501) staff       (20)      497 2023-04-07 07:04:40.000000 thread-manager-py-0.2.0/thread_manager/argument.py
--rw-r--r--   0 raynor     (501) staff       (20)      252 2023-04-05 12:40:39.000000 thread-manager-py-0.2.0/thread_manager/decorator.py
--rw-r--r--   0 raynor     (501) staff       (20)     3651 2023-04-07 10:00:08.000000 thread-manager-py-0.2.0/thread_manager/manager.py
-drwxr-xr-x   0 raynor     (501) staff       (20)        0 2023-04-08 02:26:47.457202 thread-manager-py-0.2.0/thread_manager_py.egg-info/
--rw-r--r--   0 raynor     (501) staff       (20)     3196 2023-04-08 02:26:47.000000 thread-manager-py-0.2.0/thread_manager_py.egg-info/PKG-INFO
--rw-r--r--   0 raynor     (501) staff       (20)      448 2023-04-08 02:26:47.000000 thread-manager-py-0.2.0/thread_manager_py.egg-info/SOURCES.txt
--rw-r--r--   0 raynor     (501) staff       (20)        1 2023-04-08 02:26:47.000000 thread-manager-py-0.2.0/thread_manager_py.egg-info/dependency_links.txt
--rw-r--r--   0 raynor     (501) staff       (20)        1 2023-04-08 02:26:47.000000 thread-manager-py-0.2.0/thread_manager_py.egg-info/not-zip-safe
--rw-r--r--   0 raynor     (501) staff       (20)       28 2023-04-08 02:26:47.000000 thread-manager-py-0.2.0/thread_manager_py.egg-info/top_level.txt
+drwxr-xr-x   0 raynor     (501) staff       (20)        0 2023-04-16 15:22:06.640183 thread-manager-py-0.3.0/
+-rw-r--r--   0 raynor     (501) staff       (20)     1072 2023-04-05 03:36:31.000000 thread-manager-py-0.3.0/LICENSE
+-rw-r--r--   0 raynor     (501) staff       (20)       58 2023-04-05 05:54:07.000000 thread-manager-py-0.3.0/MANIFEST.in
+-rw-r--r--   0 raynor     (501) staff       (20)     3553 2023-04-16 15:22:06.640241 thread-manager-py-0.3.0/PKG-INFO
+-rw-r--r--   0 raynor     (501) staff       (20)     2910 2023-04-16 15:18:45.000000 thread-manager-py-0.3.0/README.md
+drwxr-xr-x   0 raynor     (501) staff       (20)        0 2023-04-16 15:22:06.638401 thread-manager-py-0.3.0/pool_manager/
+-rw-r--r--   0 raynor     (501) staff       (20)      171 2023-04-16 15:18:45.000000 thread-manager-py-0.3.0/pool_manager/__init__.py
+-rw-r--r--   0 raynor     (501) staff       (20)     3373 2023-04-16 15:18:45.000000 thread-manager-py-0.3.0/pool_manager/manager.py
+-rw-r--r--   0 raynor     (501) staff       (20)        0 2023-04-05 05:38:12.000000 thread-manager-py-0.3.0/requirements.txt
+-rw-r--r--   0 raynor     (501) staff       (20)       79 2023-04-16 15:22:06.640441 thread-manager-py-0.3.0/setup.cfg
+-rw-r--r--   0 raynor     (501) staff       (20)      879 2023-04-16 15:21:39.000000 thread-manager-py-0.3.0/setup.py
+drwxr-xr-x   0 raynor     (501) staff       (20)        0 2023-04-16 15:22:06.638858 thread-manager-py-0.3.0/test/
+-rw-r--r--   0 raynor     (501) staff       (20)        0 2023-04-16 15:18:45.000000 thread-manager-py-0.3.0/test/__init__.py
+-rw-r--r--   0 raynor     (501) staff       (20)     1068 2023-04-16 15:18:45.000000 thread-manager-py-0.3.0/test/test_base.py
+-rw-r--r--   0 raynor     (501) staff       (20)     2735 2023-04-16 15:18:45.000000 thread-manager-py-0.3.0/test/test_pool_manager.py
+-rw-r--r--   0 raynor     (501) staff       (20)     4420 2023-04-16 15:18:45.000000 thread-manager-py-0.3.0/test/test_thread_manager.py
+drwxr-xr-x   0 raynor     (501) staff       (20)        0 2023-04-16 15:22:06.639471 thread-manager-py-0.3.0/thread_manager/
+-rw-r--r--   0 raynor     (501) staff       (20)      278 2023-04-16 15:18:45.000000 thread-manager-py-0.3.0/thread_manager/__init__.py
+-rw-r--r--   0 raynor     (501) staff       (20)      497 2023-04-14 10:05:45.000000 thread-manager-py-0.3.0/thread_manager/argument.py
+-rw-r--r--   0 raynor     (501) staff       (20)      251 2023-04-16 15:18:45.000000 thread-manager-py-0.3.0/thread_manager/decorator.py
+-rw-r--r--   0 raynor     (501) staff       (20)     4155 2023-04-16 15:18:45.000000 thread-manager-py-0.3.0/thread_manager/manager.py
+drwxr-xr-x   0 raynor     (501) staff       (20)        0 2023-04-16 15:22:06.640065 thread-manager-py-0.3.0/thread_manager_py.egg-info/
+-rw-r--r--   0 raynor     (501) staff       (20)     3553 2023-04-16 15:22:06.000000 thread-manager-py-0.3.0/thread_manager_py.egg-info/PKG-INFO
+-rw-r--r--   0 raynor     (501) staff       (20)      515 2023-04-16 15:22:06.000000 thread-manager-py-0.3.0/thread_manager_py.egg-info/SOURCES.txt
+-rw-r--r--   0 raynor     (501) staff       (20)        1 2023-04-16 15:22:06.000000 thread-manager-py-0.3.0/thread_manager_py.egg-info/dependency_links.txt
+-rw-r--r--   0 raynor     (501) staff       (20)        1 2023-04-16 15:22:06.000000 thread-manager-py-0.3.0/thread_manager_py.egg-info/not-zip-safe
+-rw-r--r--   0 raynor     (501) staff       (20)       33 2023-04-16 15:22:06.000000 thread-manager-py-0.3.0/thread_manager_py.egg-info/top_level.txt
```

### Comparing `thread-manager-py-0.2.0/LICENSE` & `thread-manager-py-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thread-manager-py-0.2.0/PKG-INFO` & `thread-manager-py-0.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thread-manager-py
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python Thread Manager
 Home-page: https://github.com/sanggi-wjg/py-thread-manager
 Author: SangGi
 Author-email: girr311@naver.com
 Project-URL: Bug Tracker, https://github.com/sanggi-wjg/py-thread-manager/issues
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
@@ -19,62 +19,73 @@
 Python Thread Manager
 
 [![✅Build And Test ✅](https://github.com/sanggi-wjg/py-thread-manager/actions/workflows/build-test.yml/badge.svg)](https://github.com/sanggi-wjg/py-thread-manager/actions/workflows/build-test.yml)
 [![PyPI version](https://badge.fury.io/py/thread-manager-py.svg)](https://badge.fury.io/py/thread-manager-py)
 [![PyPI](https://img.shields.io/pypi/pyversions/thread-manager-py.svg)](https://pypi.python.org/pypi/thread-manager-py)
 <br/>
 [![CodeFactor](https://www.codefactor.io/repository/github/sanggi-wjg/thread-manager-py/badge)](https://www.codefactor.io/repository/github/sanggi-wjg/thread-manager-py)
-
+[![PyPI](https://img.shields.io/pypi/dm/thread-manager-py.svg)](https://pypi.org/project/thread-manager-py/)
 
 
 ## Install
 ```shell
 pip install thread-manager-py
 ```
 
 
 ## Pool Manager Usage
-#### You can find examples in `tests/test_package.py`.
+#### You can find examples in `test/test_pool_manager.py`.
 
 
 ### Simple Usage
 ```python
 import os
 from pool_manager import PoolManager
 
-def _calculate(x):
+def calculate(x):
     print(f"[{os.getpid()}]  func: {x}\t\t", r := x ** 5 ** 2, flush=True)
     return r
 
 manager = PoolManager()
-manager.add_task(_calculate, [i for i in range(2, 22)])
+manager.add_task(calculate, [i for i in range(2, 22)])
 manager.run_map()
-manager.add_task(_calculate, [i for i in range(2, 22)])
-manager.add_task(_calculate, [i for i in range(2, 22)])
+
+manager.add_task(calculate, [i for i in range(2, 22)])
+manager.add_task(calculate, [i for i in range(2, 22)])
 manager.run_map()
+
 task_result = manager.get_task_result()
 ```
 
+```python
+with PoolManager() as manager:
+    manager.add_task(calculate, [i for i in range(2, 22)])
+    manager.add_task(calculate, [i for i in range(2, 22)])
+    manager.add_task(calculate, [i for i in range(2, 22)])
+    manager.run_map()
+```
 
 
 ## Thread Manager Usage
-#### You can find examples in `tests/test_package.py`.
+#### You can find examples in `test/test_thread_manager.py`.
 
 
 ### Simple Usage
 ```python
 import time
 from thread_manager import ThreadManager, ThreadArgument
 
 def print_something(name: str, number: int):
     print(name, number)
     time.sleep(1)
 
+    
 thread_manager = ThreadManager(print_something, [
-    ThreadArgument(thread_name=f"Thread:{x}", args=(x, x), kwargs={}, ) for x in range(1, 23)
+    ThreadArgument(thread_name=f"Thread:{x}", args=(x, x) )
+    for x in range(1, 23)
 ])
 thread_manager.run()
 ```
 
 
 ### Get Thread Error
 ```python
```

### Comparing `thread-manager-py-0.2.0/README.md` & `thread-manager-py-0.3.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -2,62 +2,73 @@
 Python Thread Manager
 
 [![✅Build And Test ✅](https://github.com/sanggi-wjg/py-thread-manager/actions/workflows/build-test.yml/badge.svg)](https://github.com/sanggi-wjg/py-thread-manager/actions/workflows/build-test.yml)
 [![PyPI version](https://badge.fury.io/py/thread-manager-py.svg)](https://badge.fury.io/py/thread-manager-py)
 [![PyPI](https://img.shields.io/pypi/pyversions/thread-manager-py.svg)](https://pypi.python.org/pypi/thread-manager-py)
 <br/>
 [![CodeFactor](https://www.codefactor.io/repository/github/sanggi-wjg/thread-manager-py/badge)](https://www.codefactor.io/repository/github/sanggi-wjg/thread-manager-py)
-
+[![PyPI](https://img.shields.io/pypi/dm/thread-manager-py.svg)](https://pypi.org/project/thread-manager-py/)
 
 
 ## Install
 ```shell
 pip install thread-manager-py
 ```
 
 
 ## Pool Manager Usage
-#### You can find examples in `tests/test_package.py`.
+#### You can find examples in `test/test_pool_manager.py`.
 
 
 ### Simple Usage
 ```python
 import os
 from pool_manager import PoolManager
 
-def _calculate(x):
+def calculate(x):
     print(f"[{os.getpid()}]  func: {x}\t\t", r := x ** 5 ** 2, flush=True)
     return r
 
 manager = PoolManager()
-manager.add_task(_calculate, [i for i in range(2, 22)])
+manager.add_task(calculate, [i for i in range(2, 22)])
 manager.run_map()
-manager.add_task(_calculate, [i for i in range(2, 22)])
-manager.add_task(_calculate, [i for i in range(2, 22)])
+
+manager.add_task(calculate, [i for i in range(2, 22)])
+manager.add_task(calculate, [i for i in range(2, 22)])
 manager.run_map()
+
 task_result = manager.get_task_result()
 ```
 
+```python
+with PoolManager() as manager:
+    manager.add_task(calculate, [i for i in range(2, 22)])
+    manager.add_task(calculate, [i for i in range(2, 22)])
+    manager.add_task(calculate, [i for i in range(2, 22)])
+    manager.run_map()
+```
 
 
 ## Thread Manager Usage
-#### You can find examples in `tests/test_package.py`.
+#### You can find examples in `test/test_thread_manager.py`.
 
 
 ### Simple Usage
 ```python
 import time
 from thread_manager import ThreadManager, ThreadArgument
 
 def print_something(name: str, number: int):
     print(name, number)
     time.sleep(1)
 
+    
 thread_manager = ThreadManager(print_something, [
-    ThreadArgument(thread_name=f"Thread:{x}", args=(x, x), kwargs={}, ) for x in range(1, 23)
+    ThreadArgument(thread_name=f"Thread:{x}", args=(x, x) )
+    for x in range(1, 23)
 ])
 thread_manager.run()
 ```
 
 
 ### Get Thread Error
 ```python
```

### Comparing `thread-manager-py-0.2.0/pool_manager/manager.py` & `thread-manager-py-0.3.0/pool_manager/manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,109 @@
 import collections
+import logging
 import multiprocessing
 from multiprocessing import Pool
+from multiprocessing.pool import MapResult, IMapIterator
 from queue import PriorityQueue
 from typing import Callable, Any
 
+log = logging.getLogger("pool.manager")
+
 
 class PoolManager:
-    _instance = None
     default_timeout = 30
 
     def __new__(cls, *args, **kwargs):
         if not hasattr(cls, 'instance'):
-            cls._instance = super(PoolManager, cls).__new__(cls)
-        return cls._instance
+            cls.instance = super(PoolManager, cls).__new__(cls)
+        return cls.instance
 
     def __init__(self, process_count: int = multiprocessing.cpu_count()):
         """
         Constructor
         :param process_count: number of cpu processor, can not exceed than multiprocessing.cpu_count()
         :type process_count: int
         """
         self.task_queue: PriorityQueue = PriorityQueue()
         self.task_result_queue: collections.deque = collections.deque()
         self.pool: Pool = Pool(min(process_count, multiprocessing.cpu_count()))
+        log.debug(f"pool manager inited, {min(process_count, multiprocessing.cpu_count())}")
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.close()
 
     def is_empty_task(self) -> bool:
         return self.task_queue.empty()
 
     def has_task(self) -> bool:
         return not self.task_queue.empty()
 
     def clear_task(self) -> bool:
         while self.has_task():
             self.task_queue.get(False)
+        log.debug("task_queue cleared")
         return True
 
+    def close(self):
+        self.clear_task()
+        self.pool.close()
+
     def add_task(self, callable_func: Callable, *arguments: list, priority: int = 100):
         """
 
         :param callable_func: task function
         :type callable_func: Callable
         :param arguments: func arguments
         :type arguments: list
         :param priority: task priority
         :type priority: int
         """
         self.task_queue.put((priority, callable_func, *arguments), timeout=self.default_timeout)
+        log.debug(f"task_queue put, {priority}, {callable_func}. {arguments}")
 
     def _get_task(self) -> Callable:
         return self.task_queue.get()
 
     def add_task_result(self, task_result: Any):
-        self.task_result_queue.append(task_result)
+        if isinstance(task_result, list):
+            self.task_result_queue.append(task_result)
+
+        elif isinstance(task_result, MapResult):
+            self.task_result_queue.append(task_result.get())
+
+        elif isinstance(task_result, IMapIterator):
+            self.task_result_queue.append([r for r in task_result])
+
+        else:
+            log.warning("task_results not saved.")
+            # assert False, "task_results not saved."
 
     def get_task_result(self) -> collections.deque:
         return self.task_result_queue.copy()
 
+    def _run(self, pool_func: Callable):
+        while not self.is_empty_task():
+            _, func, arguments = self._get_task()
+            result = pool_func(func, arguments)
+            log.debug(f"task_queue run, {func}")
+            self.add_task_result(result)
+
     def run_map(self):
         """
         https://stackoverflow.com/questions/26520781/multiprocessing-pool-whats-the-difference-between-map-async-and-imap
         """
-        while not self.is_empty_task():
-            _, func, arguments = self._get_task()
-            result = self.pool.map(func, arguments)
-            self.add_task_result(result)
+        self._run(self.pool.map)
 
     def run_map_async(self):
         """
 
         """
-        while not self.is_empty_task():
-            _, func, arguments = self._get_task()
-            result = self.pool.map_async(func, arguments)
-            self.add_task_result(result.get())
+        self._run(self.pool.map_async)
 
     def run_imap(self):
         """
 
         """
-        while not self.is_empty_task():
-            _, func, arguments = self._get_task()
-            result = self.pool.imap(func, arguments)
-            self.add_task_result([r for r in result])
+        self._run(self.pool.imap)
```

### Comparing `thread-manager-py-0.2.0/setup.py` & `thread-manager-py-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='thread-manager-py',
-    version='0.2.0',
+    version='0.3.0',
     url='https://github.com/sanggi-wjg/py-thread-manager',
     author='SangGi',
     author_email='girr311@naver.com',
     description='Python Thread Manager',
     packages=find_packages(exclude=['tests']),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `thread-manager-py-0.2.0/thread_manager/manager.py` & `thread-manager-py-0.3.0/thread_manager/manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import collections
+import logging
 import threading
-from _thread import _ExceptHookArgs as except_hook_args
+from _thread import _ExceptHookArgs as ExceptHookArgs
 from threading import Thread, RLock
 from typing import List, Callable
 
 from .argument import ThreadArgument
 
+log = logging.getLogger("thread.manager")
+
 
 class ThreadManager:
     default_concurrency = 10
 
     def __init__(self, callable_func: Callable, thread_arguments: List[ThreadArgument], except_hook: Callable = None):
         """
         Constructor
@@ -28,20 +31,25 @@
         # configs
         self.concurrency: int = self.default_concurrency
         self.is_interrupted: bool = False
         self.consumer_lock = RLock()
         # errors
         self.error_deque = collections.deque()
         self.set_exception_hook(self.add_errors if except_hook is None else except_hook)
+        log.debug(f"thread manager inited, "
+                  f"func: {self.func.__name__}, "
+                  f"thread_arguments_count: {self.thread_arguments_count}, "
+                  f"except_hook: {'default except_hook' if except_hook is None else except_hook}")
 
     def set_exception_hook(self, except_hook: Callable):
         threading.excepthook = except_hook
 
-    def add_errors(self, error: except_hook_args):
+    def add_errors(self, error: ExceptHookArgs):
         self.error_deque.append(error)
+        log.debug(f"error appended : {error}")
 
     def get_errors(self) -> collections.deque:
         return self.error_deque.copy()
 
     def get_error_count(self) -> int:
         return len(self.error_deque)
 
@@ -51,20 +59,22 @@
     def set_concurrency(self, number: int):
         """
         동시 실행 수 설정
         :param number: number of concurrency, 동시 실행 수
         :type number: int
         """
         self.concurrency = number
+        log.debug(f"concurrency changed to {number}")
 
     def stop(self):
         """
         Stop ThreadManager
         """
         self.is_interrupted = True
+        log.debug(f"requested to stop")
 
     def start_thread(self, start: int, end: int):
         """
         Execute Thread
         :param start: index of start
         :type start: int
         :param end: index of end
@@ -87,18 +97,17 @@
                     th.start()
                 for th in self.threads:
                     th.join()
                 del self.threads
 
     def run(self):
         start_index = 0
-        while True:
-            is_exceed_index = start_index >= self.thread_arguments_count
-            if self.is_interrupted or is_exceed_index:
-                return
+        # 중지 상태 혹은 완료 되면 종료
+        while not self.is_interrupted and (start_index <= self.thread_arguments_count):
             # 만약 end_index 가 총 실행 크기 보다 크다면 end_index 를 실행 크기로 맞추어 IndexError 방지
             end_index = start_index + self.concurrency
             if end_index > self.thread_arguments_count:
                 end_index = self.thread_arguments_count
 
             self.start_thread(start_index, end_index)
+            log.debug(f"{start_index}~{end_index} threads finished")
             start_index += self.concurrency
```

### Comparing `thread-manager-py-0.2.0/thread_manager_py.egg-info/PKG-INFO` & `thread-manager-py-0.3.0/thread_manager_py.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thread-manager-py
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python Thread Manager
 Home-page: https://github.com/sanggi-wjg/py-thread-manager
 Author: SangGi
 Author-email: girr311@naver.com
 Project-URL: Bug Tracker, https://github.com/sanggi-wjg/py-thread-manager/issues
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
@@ -19,62 +19,73 @@
 Python Thread Manager
 
 [![✅Build And Test ✅](https://github.com/sanggi-wjg/py-thread-manager/actions/workflows/build-test.yml/badge.svg)](https://github.com/sanggi-wjg/py-thread-manager/actions/workflows/build-test.yml)
 [![PyPI version](https://badge.fury.io/py/thread-manager-py.svg)](https://badge.fury.io/py/thread-manager-py)
 [![PyPI](https://img.shields.io/pypi/pyversions/thread-manager-py.svg)](https://pypi.python.org/pypi/thread-manager-py)
 <br/>
 [![CodeFactor](https://www.codefactor.io/repository/github/sanggi-wjg/thread-manager-py/badge)](https://www.codefactor.io/repository/github/sanggi-wjg/thread-manager-py)
-
+[![PyPI](https://img.shields.io/pypi/dm/thread-manager-py.svg)](https://pypi.org/project/thread-manager-py/)
 
 
 ## Install
 ```shell
 pip install thread-manager-py
 ```
 
 
 ## Pool Manager Usage
-#### You can find examples in `tests/test_package.py`.
+#### You can find examples in `test/test_pool_manager.py`.
 
 
 ### Simple Usage
 ```python
 import os
 from pool_manager import PoolManager
 
-def _calculate(x):
+def calculate(x):
     print(f"[{os.getpid()}]  func: {x}\t\t", r := x ** 5 ** 2, flush=True)
     return r
 
 manager = PoolManager()
-manager.add_task(_calculate, [i for i in range(2, 22)])
+manager.add_task(calculate, [i for i in range(2, 22)])
 manager.run_map()
-manager.add_task(_calculate, [i for i in range(2, 22)])
-manager.add_task(_calculate, [i for i in range(2, 22)])
+
+manager.add_task(calculate, [i for i in range(2, 22)])
+manager.add_task(calculate, [i for i in range(2, 22)])
 manager.run_map()
+
 task_result = manager.get_task_result()
 ```
 
+```python
+with PoolManager() as manager:
+    manager.add_task(calculate, [i for i in range(2, 22)])
+    manager.add_task(calculate, [i for i in range(2, 22)])
+    manager.add_task(calculate, [i for i in range(2, 22)])
+    manager.run_map()
+```
 
 
 ## Thread Manager Usage
-#### You can find examples in `tests/test_package.py`.
+#### You can find examples in `test/test_thread_manager.py`.
 
 
 ### Simple Usage
 ```python
 import time
 from thread_manager import ThreadManager, ThreadArgument
 
 def print_something(name: str, number: int):
     print(name, number)
     time.sleep(1)
 
+    
 thread_manager = ThreadManager(print_something, [
-    ThreadArgument(thread_name=f"Thread:{x}", args=(x, x), kwargs={}, ) for x in range(1, 23)
+    ThreadArgument(thread_name=f"Thread:{x}", args=(x, x) )
+    for x in range(1, 23)
 ])
 thread_manager.run()
 ```
 
 
 ### Get Thread Error
 ```python
```

