# Comparing `tmp/py_shiftmanager-0.1.5.tar.gz` & `tmp/py_shiftmanager-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_shiftmanager-0.1.5.tar", last modified: Sun Apr 16 10:35:24 2023, max compression
+gzip compressed data, was "py_shiftmanager-0.1.6.tar", last modified: Sun Apr 16 11:50:20 2023, max compression
```

## Comparing `py_shiftmanager-0.1.5.tar` & `py_shiftmanager-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-16 10:35:24.768645 py_shiftmanager-0.1.5/
--rw-r--r--   0 amitnakash   (501) staff       (20)       17 2023-04-11 08:18:28.000000 py_shiftmanager-0.1.5/MANIFEST.in
--rw-r--r--   0 amitnakash   (501) staff       (20)      318 2023-04-16 10:35:24.768547 py_shiftmanager-0.1.5/PKG-INFO
--rw-r--r--   0 amitnakash   (501) staff       (20)     8233 2023-04-16 10:34:31.000000 py_shiftmanager-0.1.5/Readme.md
-drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-16 10:35:24.767778 py_shiftmanager-0.1.5/py_shiftmanager/
--rw-r--r--   0 amitnakash   (501) staff       (20)      289 2023-04-13 06:10:21.000000 py_shiftmanager-0.1.5/py_shiftmanager/__init__.py
--rw-r--r--   0 amitnakash   (501) staff       (20)      428 2023-04-09 13:34:58.000000 py_shiftmanager-0.1.5/py_shiftmanager/logger.py
--rw-r--r--   0 amitnakash   (501) staff       (20)     5684 2023-04-16 10:28:32.000000 py_shiftmanager-0.1.5/py_shiftmanager/shiftmanager_compute.py
--rw-r--r--   0 amitnakash   (501) staff       (20)     5915 2023-04-16 10:28:56.000000 py_shiftmanager-0.1.5/py_shiftmanager/shiftmanager_io.py
--rw-r--r--   0 amitnakash   (501) staff       (20)      820 2023-04-16 10:30:37.000000 py_shiftmanager-0.1.5/py_shiftmanager/timeout.py
--rw-r--r--   0 amitnakash   (501) staff       (20)     3555 2023-04-16 10:08:49.000000 py_shiftmanager-0.1.5/py_shiftmanager/worker.py
-drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-16 10:35:24.768393 py_shiftmanager-0.1.5/py_shiftmanager.egg-info/
--rw-r--r--   0 amitnakash   (501) staff       (20)      318 2023-04-16 10:35:24.000000 py_shiftmanager-0.1.5/py_shiftmanager.egg-info/PKG-INFO
--rw-r--r--   0 amitnakash   (501) staff       (20)      406 2023-04-16 10:35:24.000000 py_shiftmanager-0.1.5/py_shiftmanager.egg-info/SOURCES.txt
--rw-r--r--   0 amitnakash   (501) staff       (20)        1 2023-04-16 10:35:24.000000 py_shiftmanager-0.1.5/py_shiftmanager.egg-info/dependency_links.txt
--rw-r--r--   0 amitnakash   (501) staff       (20)       12 2023-04-16 10:35:24.000000 py_shiftmanager-0.1.5/py_shiftmanager.egg-info/requires.txt
--rw-r--r--   0 amitnakash   (501) staff       (20)       16 2023-04-16 10:35:24.000000 py_shiftmanager-0.1.5/py_shiftmanager.egg-info/top_level.txt
--rw-r--r--   0 amitnakash   (501) staff       (20)       38 2023-04-16 10:35:24.768676 py_shiftmanager-0.1.5/setup.cfg
--rw-r--r--   0 amitnakash   (501) staff       (20)      595 2023-04-16 10:34:01.000000 py_shiftmanager-0.1.5/setup.py
+drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-16 11:50:20.363793 py_shiftmanager-0.1.6/
+-rw-r--r--   0 amitnakash   (501) staff       (20)       17 2023-04-11 08:18:28.000000 py_shiftmanager-0.1.6/MANIFEST.in
+-rw-r--r--   0 amitnakash   (501) staff       (20)      318 2023-04-16 11:50:20.363651 py_shiftmanager-0.1.6/PKG-INFO
+-rw-r--r--   0 amitnakash   (501) staff       (20)     8415 2023-04-16 11:47:22.000000 py_shiftmanager-0.1.6/Readme.md
+drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-16 11:50:20.362642 py_shiftmanager-0.1.6/py_shiftmanager/
+-rw-r--r--   0 amitnakash   (501) staff       (20)      289 2023-04-13 06:10:21.000000 py_shiftmanager-0.1.6/py_shiftmanager/__init__.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)      428 2023-04-09 13:34:58.000000 py_shiftmanager-0.1.6/py_shiftmanager/logger.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)     5684 2023-04-16 10:28:32.000000 py_shiftmanager-0.1.6/py_shiftmanager/shiftmanager_compute.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)     5915 2023-04-16 10:28:56.000000 py_shiftmanager-0.1.6/py_shiftmanager/shiftmanager_io.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)      820 2023-04-16 10:51:53.000000 py_shiftmanager-0.1.6/py_shiftmanager/timeout.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)     3555 2023-04-16 10:08:49.000000 py_shiftmanager-0.1.6/py_shiftmanager/worker.py
+drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-16 11:50:20.363438 py_shiftmanager-0.1.6/py_shiftmanager.egg-info/
+-rw-r--r--   0 amitnakash   (501) staff       (20)      318 2023-04-16 11:50:20.000000 py_shiftmanager-0.1.6/py_shiftmanager.egg-info/PKG-INFO
+-rw-r--r--   0 amitnakash   (501) staff       (20)      406 2023-04-16 11:50:20.000000 py_shiftmanager-0.1.6/py_shiftmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 amitnakash   (501) staff       (20)        1 2023-04-16 11:50:20.000000 py_shiftmanager-0.1.6/py_shiftmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 amitnakash   (501) staff       (20)       12 2023-04-16 11:50:20.000000 py_shiftmanager-0.1.6/py_shiftmanager.egg-info/requires.txt
+-rw-r--r--   0 amitnakash   (501) staff       (20)       16 2023-04-16 11:50:20.000000 py_shiftmanager-0.1.6/py_shiftmanager.egg-info/top_level.txt
+-rw-r--r--   0 amitnakash   (501) staff       (20)       38 2023-04-16 11:50:20.363838 py_shiftmanager-0.1.6/setup.cfg
+-rw-r--r--   0 amitnakash   (501) staff       (20)      595 2023-04-16 11:41:58.000000 py_shiftmanager-0.1.6/setup.py
```

### Comparing `py_shiftmanager-0.1.5/Readme.md` & `py_shiftmanager-0.1.6/Readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Py-ShiftManager
-#### v0.1.5
+#### v0.1.6
 
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
-#### added in v0.1.4/5
+#### added in v0.1.6
 * 🛠️ Task submission now supports both *args and **kwargs. 
 
 ## Usage
 Here's an example of how to use Py-ShiftManager to handle IO tasks:  
 `from py_shiftmanager import ShiftManager_IO`.  
 Now, lets also import *timeout_timer* wrapper:  
 `from py_shiftmanager.timeout import timeout_timer`
@@ -53,20 +53,20 @@
 `import requests`  
 `@timeout_timer(seconds=3)`  
 `def get_status(url):`  
 `   return requests.get(url).status_code`  
 We can assign single tasks to the queue:  
 `manager.new_task(get_status, "http://www.google.com")`  
 `manager.new_task(get_status, "http://www.facebook.com")`  
-`manager.new_task(get_status, "http://www.twitter.com")`   
+`manager.new_task(get_status, url="http://www.twitter.com")`   
 Or we can submit a batch by passing a list of tuples:  
-`tasks = [(get_status, "http://www.google.com"),(get_status, "http://www.facebook.com")]`  
+`tasks = [(get_status, ("http://www.google.com",)),(get_status, {"url": "http://www.facebook.com"})]`  
 `manager.new_batch(tasks)`  
 
-**Note**: you can also pass in *lambda* functions.
+**Note**: you can also pass in *lambda* functions. Also make sure that with using new_batch() you pass arguments in a nested tuple.
 
 # Handle the tasks
 `manager.handle_work()`  
 *ShiftManager* spins up the workers and starts consuming tasks from the input queue.  
 Since we applied the *timeout_timer* decorator, if a task takes longer than 3 seconds - it will be terminated, but you'll still recieve a result with the task details, and that it has ran out of time.  
 
 # Wait for the tasks to complete
@@ -94,18 +94,18 @@
 **Note**: Once initialized, queue size cannot be changed.  
 # Add some tasks to the input queue
 We can assign single tasks, like so:  
 `manager.new_task(lambda x: x**2, 3)`  
 `manager.new_task(lambda x: x**3, 4)`  
 `manager.new_task(lambda x, y: x**4 + y, 5, 9)`  
 or submit a batch by passing a list of tuples:  
-`tasks = [(lambda x: x**2, 3),(lambda x: x**3, 4)]`
+`tasks = [(lambda x: x**2, (3,)),(lambda x: x**3, (4,))]`
 `manager.new_batch(tasks)`
 
-**Note**: Accepting *lambda* functions and normal functions.
+**Note**: Accepting *lambda* functions and normal functions. Also make sure that with using new_batch() you pass arguments in a nested tuple.
 
 # Handle the tasks
 `manager.handle_work()`  
 *ShiftManager* will start the workers and begin performing the calculations.
 
 # Get the results
 `results = manager.get_results()`
```

### Comparing `py_shiftmanager-0.1.5/py_shiftmanager/shiftmanager_compute.py` & `py_shiftmanager-0.1.6/py_shiftmanager/shiftmanager_compute.py`

 * *Files identical despite different names*

### Comparing `py_shiftmanager-0.1.5/py_shiftmanager/shiftmanager_io.py` & `py_shiftmanager-0.1.6/py_shiftmanager/shiftmanager_io.py`

 * *Files identical despite different names*

### Comparing `py_shiftmanager-0.1.5/py_shiftmanager/timeout.py` & `py_shiftmanager-0.1.6/py_shiftmanager/timeout.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import threading
 
 def timeout_timer(seconds=5, func=None, error_message='Task timed out.'):
     """ Timeout wrapper, sets a seconds countdown on a separate running thread with using join().
         Setting the thread daemon flag to True, so that it exits when the time runs out and program ended.
     """
     if func is None:
-        return lambda f: timeout_timer(f, seconds, error_message)
+        return lambda f: timeout_timer(seconds, f, error_message)
 
     def wrapper(*args, **kwargs):
         result = {"task": func.__name__, "args": args, "kwargs": kwargs}
         def target():
             result["result"] = func(*args, **kwargs)
         thread = threading.Thread(target=target)
         thread.daemon = True
```

### Comparing `py_shiftmanager-0.1.5/py_shiftmanager/worker.py` & `py_shiftmanager-0.1.6/py_shiftmanager/worker.py`

 * *Files identical despite different names*

### Comparing `py_shiftmanager-0.1.5/setup.py` & `py_shiftmanager-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 # long_description = Path('Readme.md').read_text()
 
 setup(
     name='py_shiftmanager',
-    version='0.1.5',
+    version='0.1.6',
     description='A simplified, all-in-one shop for handling multithreading/multiprocessing using a managed queue system.',
     # long_description=long_description,
     packages=find_packages(),
     install_requires=[
         'dill==0.3.6',
     ],
     classifiers=[
```

