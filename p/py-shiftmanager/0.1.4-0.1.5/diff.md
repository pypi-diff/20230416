# Comparing `tmp/py_shiftmanager-0.1.4.tar.gz` & `tmp/py_shiftmanager-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_shiftmanager-0.1.4.tar", last modified: Fri Apr 14 14:16:37 2023, max compression
+gzip compressed data, was "py_shiftmanager-0.1.5.tar", last modified: Sun Apr 16 10:35:24 2023, max compression
```

## Comparing `py_shiftmanager-0.1.4.tar` & `py_shiftmanager-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-14 14:16:37.360815 py_shiftmanager-0.1.4/
--rw-r--r--   0 amitnakash   (501) staff       (20)       17 2023-04-11 08:18:28.000000 py_shiftmanager-0.1.4/MANIFEST.in
--rw-r--r--   0 amitnakash   (501) staff       (20)      318 2023-04-14 14:16:37.360646 py_shiftmanager-0.1.4/PKG-INFO
--rw-r--r--   0 amitnakash   (501) staff       (20)     8231 2023-04-14 14:15:13.000000 py_shiftmanager-0.1.4/Readme.md
-drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-14 14:16:37.359246 py_shiftmanager-0.1.4/py_shiftmanager/
--rw-r--r--   0 amitnakash   (501) staff       (20)      289 2023-04-13 06:10:21.000000 py_shiftmanager-0.1.4/py_shiftmanager/__init__.py
--rw-r--r--   0 amitnakash   (501) staff       (20)      428 2023-04-09 13:34:58.000000 py_shiftmanager-0.1.4/py_shiftmanager/logger.py
--rw-r--r--   0 amitnakash   (501) staff       (20)     5300 2023-04-14 13:52:18.000000 py_shiftmanager-0.1.4/py_shiftmanager/shiftmanager_compute.py
--rw-r--r--   0 amitnakash   (501) staff       (20)     5531 2023-04-14 13:54:57.000000 py_shiftmanager-0.1.4/py_shiftmanager/shiftmanager_io.py
--rw-r--r--   0 amitnakash   (501) staff       (20)      802 2023-04-14 14:07:57.000000 py_shiftmanager-0.1.4/py_shiftmanager/timeout.py
--rw-r--r--   0 amitnakash   (501) staff       (20)     3372 2023-04-13 22:49:11.000000 py_shiftmanager-0.1.4/py_shiftmanager/worker.py
-drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-14 14:16:37.360332 py_shiftmanager-0.1.4/py_shiftmanager.egg-info/
--rw-r--r--   0 amitnakash   (501) staff       (20)      318 2023-04-14 14:16:37.000000 py_shiftmanager-0.1.4/py_shiftmanager.egg-info/PKG-INFO
--rw-r--r--   0 amitnakash   (501) staff       (20)      406 2023-04-14 14:16:37.000000 py_shiftmanager-0.1.4/py_shiftmanager.egg-info/SOURCES.txt
--rw-r--r--   0 amitnakash   (501) staff       (20)        1 2023-04-14 14:16:37.000000 py_shiftmanager-0.1.4/py_shiftmanager.egg-info/dependency_links.txt
--rw-r--r--   0 amitnakash   (501) staff       (20)       12 2023-04-14 14:16:37.000000 py_shiftmanager-0.1.4/py_shiftmanager.egg-info/requires.txt
--rw-r--r--   0 amitnakash   (501) staff       (20)       16 2023-04-14 14:16:37.000000 py_shiftmanager-0.1.4/py_shiftmanager.egg-info/top_level.txt
--rw-r--r--   0 amitnakash   (501) staff       (20)       38 2023-04-14 14:16:37.360883 py_shiftmanager-0.1.4/setup.cfg
--rw-r--r--   0 amitnakash   (501) staff       (20)      595 2023-04-14 14:16:30.000000 py_shiftmanager-0.1.4/setup.py
+drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-16 10:35:24.768645 py_shiftmanager-0.1.5/
+-rw-r--r--   0 amitnakash   (501) staff       (20)       17 2023-04-11 08:18:28.000000 py_shiftmanager-0.1.5/MANIFEST.in
+-rw-r--r--   0 amitnakash   (501) staff       (20)      318 2023-04-16 10:35:24.768547 py_shiftmanager-0.1.5/PKG-INFO
+-rw-r--r--   0 amitnakash   (501) staff       (20)     8233 2023-04-16 10:34:31.000000 py_shiftmanager-0.1.5/Readme.md
+drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-16 10:35:24.767778 py_shiftmanager-0.1.5/py_shiftmanager/
+-rw-r--r--   0 amitnakash   (501) staff       (20)      289 2023-04-13 06:10:21.000000 py_shiftmanager-0.1.5/py_shiftmanager/__init__.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)      428 2023-04-09 13:34:58.000000 py_shiftmanager-0.1.5/py_shiftmanager/logger.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)     5684 2023-04-16 10:28:32.000000 py_shiftmanager-0.1.5/py_shiftmanager/shiftmanager_compute.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)     5915 2023-04-16 10:28:56.000000 py_shiftmanager-0.1.5/py_shiftmanager/shiftmanager_io.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)      820 2023-04-16 10:30:37.000000 py_shiftmanager-0.1.5/py_shiftmanager/timeout.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)     3555 2023-04-16 10:08:49.000000 py_shiftmanager-0.1.5/py_shiftmanager/worker.py
+drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-16 10:35:24.768393 py_shiftmanager-0.1.5/py_shiftmanager.egg-info/
+-rw-r--r--   0 amitnakash   (501) staff       (20)      318 2023-04-16 10:35:24.000000 py_shiftmanager-0.1.5/py_shiftmanager.egg-info/PKG-INFO
+-rw-r--r--   0 amitnakash   (501) staff       (20)      406 2023-04-16 10:35:24.000000 py_shiftmanager-0.1.5/py_shiftmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 amitnakash   (501) staff       (20)        1 2023-04-16 10:35:24.000000 py_shiftmanager-0.1.5/py_shiftmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 amitnakash   (501) staff       (20)       12 2023-04-16 10:35:24.000000 py_shiftmanager-0.1.5/py_shiftmanager.egg-info/requires.txt
+-rw-r--r--   0 amitnakash   (501) staff       (20)       16 2023-04-16 10:35:24.000000 py_shiftmanager-0.1.5/py_shiftmanager.egg-info/top_level.txt
+-rw-r--r--   0 amitnakash   (501) staff       (20)       38 2023-04-16 10:35:24.768676 py_shiftmanager-0.1.5/setup.cfg
+-rw-r--r--   0 amitnakash   (501) staff       (20)      595 2023-04-16 10:34:01.000000 py_shiftmanager-0.1.5/setup.py
```

### Comparing `py_shiftmanager-0.1.4/Readme.md` & `py_shiftmanager-0.1.5/Readme.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Py-ShiftManager
-#### v0.1.4
+#### v0.1.5
 
 Py-ShiftManager is a Python module that provides a managed queue environment for handling IO and computational tasks, allowing you to easily manage concurrency and multiprocessing without worrying about the details.
 
 ## Installation
 You can install Py-ShiftManager using pip:
 `pip install py-shiftmanager`
 
@@ -25,15 +25,15 @@
 #### added in v0.1.3
 * 🛠️ Improved handling of queue exceptions - a better managing solution for large incoming amount of tasks.  
 * 🛠️ Improved task submission logic.
 * 🔒 Improved encapsulation.
 * 🛠️ New method added - `configure()`; read more under *'API'* section.   
 * 🛠️ Improved concurrency and parallelism in the IO module.
 * ⌫ Deprecated methods - `queue_in_size()`, `queue_out_size()` 
-#### added in v0.1.4
+#### added in v0.1.4/5
 * 🛠️ Task submission now supports both *args and **kwargs. 
 
 ## Usage
 Here's an example of how to use Py-ShiftManager to handle IO tasks:  
 `from py_shiftmanager import ShiftManager_IO`.  
 Now, lets also import *timeout_timer* wrapper:  
 `from py_shiftmanager.timeout import timeout_timer`
@@ -167,15 +167,15 @@
 Allows the user to configure the following attributes by passing keyword arguments:  
 * `daemon: bool` - reconfigure workers daemon status. 
 * `put_timeout: int` - reconfigure timeout (in seconds) for input queue task submission (default is `1` second).
 * `num_of_workers: int` - reconfigure number of workers.  
 
 **timeout_timer**  
 `@timeout_timer(seconds: int = 5)`  
-A decorator that attaches a timeout counter to your methods, use it to set a time limit to tasks in seconds; `5` seconds by default.  
+A decorator that attaches a timeout counter to your methods, use it to set a time limit to tasks in seconds; `seconds=5` by default.  
 
 **context_manager**
 implement it using the `with` keyword:  
 `with ShiftManager_Compute() as manager:`  
 `   manager.new_task(lambda x: x**2, 4)`  
 `   manager.new_task(lambda x: x**4, 13)`  
 then get the results:
```

### Comparing `py_shiftmanager-0.1.4/py_shiftmanager/shiftmanager_compute.py` & `py_shiftmanager-0.1.5/py_shiftmanager/shiftmanager_compute.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,29 +82,37 @@
     """ Task and queue management """
     def new_task(self, func: Callable, *args, force: bool = False, **kwargs) -> NoReturn:
         new_task = {"arrival_time": int(datetime.datetime.now().timestamp()), "func": dill.dumps(func), "args": args, "kwargs": kwargs}
         self.__submit_task(new_task, force)
 
     def new_batch(self, tasks: List, force: bool = False) -> NoReturn:
         for task in tasks:
-            if len(task) == 1:
-                func = task[0]
+            try:
+                if len(task) == 1:
+                    func = task[0]
+                    args = ()
+                    kwargs = {}
+                elif len(task) == 2:
+                    func, arg_or_kwarg = task
+                    if isinstance(arg_or_kwarg, tuple or str or int or list):
+                        args = arg_or_kwarg
+                        kwargs = {}
+                    elif isinstance(arg_or_kwarg, dict):
+                        args = ()
+                        kwargs = arg_or_kwarg
+                    else:
+                        raise TypeError("invalid argument type in task batch.")
+                elif len(task) == 3:
+                    func, args, kwargs = task
+            except TypeError:
+                func = task
                 args = ()
                 kwargs = {}
-            elif len(task) == 2:
-                func, arg_or_kwarg = task
-                if isinstance(arg_or_kwarg, tuple):
-                    args = arg_or_kwarg
-                    kwargs = {}
-                else:
-                    args = ()
-                    kwargs = arg_or_kwarg
-            else:
-                func, args, kwargs = task
-            self.new_task(func, *args, force=force, **kwargs)
+            finally:
+                self.new_task(func, *args, force=force, **kwargs)
 
     def handle_work(self) -> NoReturn:
         """ start pool without close() to enable continuous acceptance of new submitted tasks """
         self.__pool = multiprocessing.Pool(processes=self.__num_of_workers, initializer=self.__worker.work,
                                     initargs=(self.__q_in, self.__q_out))
 
     def get_results(self) -> List:
```

### Comparing `py_shiftmanager-0.1.4/py_shiftmanager/shiftmanager_io.py` & `py_shiftmanager-0.1.5/py_shiftmanager/shiftmanager_io.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,29 +83,37 @@
     """ Task and queue management """
     def new_task(self, func: Callable, *args, force: bool = False, **kwargs) -> NoReturn:
         new_task = {"arrival_time": int(datetime.datetime.now().timestamp()), "func": dill.dumps(func), "args": args, "kwargs": kwargs}
         self.__submit_task(new_task, force)
 
     def new_batch(self, tasks: List, force: bool = False) -> NoReturn:
         for task in tasks:
-            if len(task) == 1:
-                func = task[0]
+            try:
+                if len(task) == 1:
+                    func = task[0]
+                    args = ()
+                    kwargs = {}
+                elif len(task) == 2:
+                    func, arg_or_kwarg = task
+                    if isinstance(arg_or_kwarg, tuple or str or int or list):
+                        args = arg_or_kwarg
+                        kwargs = {}
+                    elif isinstance(arg_or_kwarg, dict):
+                        args = ()
+                        kwargs = arg_or_kwarg
+                    else:
+                        raise TypeError("invalid argument type in task batch.")
+                elif len(task) == 3:
+                    func, args, kwargs = task
+            except TypeError:
+                func = task
                 args = ()
                 kwargs = {}
-            elif len(task) == 2:
-                func, arg_or_kwarg = task
-                if isinstance(arg_or_kwarg, tuple):
-                    args = arg_or_kwarg
-                    kwargs = {}
-                else:
-                    args = ()
-                    kwargs = arg_or_kwarg
-            else:
-                func, args, kwargs = task
-            self.new_task(func, *args, force=force, **kwargs)
+            finally:
+                self.new_task(func, *args, force=force, **kwargs)
 
     # def queue_in_size(self) -> int or NoReturn:
     #     try:
     #         return self.__q_in.qsize()
     #     except NotImplementedError:
     #         logger.logger.error("Input-queue .qsize() not implemented; exited gracefully.")
```

### Comparing `py_shiftmanager-0.1.4/py_shiftmanager/timeout.py` & `py_shiftmanager-0.1.5/py_shiftmanager/timeout.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import threading
 
-def timeout_timer(func=None, seconds=5, error_message='Task timed out.'):
+def timeout_timer(seconds=5, func=None, error_message='Task timed out.'):
     """ Timeout wrapper, sets a seconds countdown on a separate running thread with using join().
         Setting the thread daemon flag to True, so that it exits when the time runs out and program ended.
     """
     if func is None:
         return lambda f: timeout_timer(f, seconds, error_message)
 
     def wrapper(*args, **kwargs):
-        result = {"task": func.__name__, "args": args}
+        result = {"task": func.__name__, "args": args, "kwargs": kwargs}
         def target():
             result["result"] = func(*args, **kwargs)
         thread = threading.Thread(target=target)
         thread.daemon = True
         thread.start()
         thread.join(seconds)
         if thread.is_alive():
```

### Comparing `py_shiftmanager-0.1.4/py_shiftmanager/worker.py` & `py_shiftmanager-0.1.5/py_shiftmanager/worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                 self.__is_working = True
                 func = dill.loads(task['func'])
                 args = task['args']
                 kwargs = task['kwargs']
                 try:
                     result = func(*args, **kwargs)
                 except Exception as err:
-                    result = {"error": err, "task": func.__name__, "args": args}
+                    result = {"error": err, "task": func.__name__, "args": args, "kwargs": kwargs}
                 qu_in.task_done()
                 try:
                     lock2.acquire()
                     qu_out.put(result, timeout=1)
                 except queue.Full:
                     logger.logger.error("OUTPUT-QUEUE IS FULL.")
                 finally:
@@ -89,15 +89,18 @@
                     self.__is_hired = False
                     qu_in.task_done()
                     break
                 self.__is_working = True
                 func = dill.loads(task['func'])
                 args = task['args']
                 kwargs = task['kwargs']
-                result = func(*args, **kwargs)
+                try:
+                    result = func(*args, **kwargs)
+                except Exception as err:
+                    result = {"error": err, "task": func.__name__, "args": args, "kwargs": kwargs}
                 qu_in.task_done()
                 try:
                     lock4.acquire()
                     qu_out.put(result, timeout=1)
                     lock4.release()
                 except queue.Full:
                     lock4.release()
```

### Comparing `py_shiftmanager-0.1.4/setup.py` & `py_shiftmanager-0.1.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 # long_description = Path('Readme.md').read_text()
 
 setup(
     name='py_shiftmanager',
-    version='0.1.4',
+    version='0.1.5',
     description='A simplified, all-in-one shop for handling multithreading/multiprocessing using a managed queue system.',
     # long_description=long_description,
     packages=find_packages(),
     install_requires=[
         'dill==0.3.6',
     ],
     classifiers=[
```

