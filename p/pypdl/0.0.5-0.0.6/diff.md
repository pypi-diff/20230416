# Comparing `tmp/pypdl-0.0.5.tar.gz` & `tmp/pypdl-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdl-0.0.5.tar", last modified: Sat Mar 25 18:02:18 2023, max compression
+gzip compressed data, was "pypdl-0.0.6.tar", last modified: Sun Apr 16 17:10:28 2023, max compression
```

## Comparing `pypdl-0.0.5.tar` & `pypdl-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-25 18:02:18.720157 pypdl-0.0.5/
--rw-rw-rw-   0        0        0     1086 2023-03-20 10:21:57.000000 pypdl-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     8170 2023-03-25 18:02:18.717553 pypdl-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     7581 2023-03-25 18:01:40.000000 pypdl-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-25 18:02:18.692046 pypdl-0.0.5/pypdl/
--rw-rw-rw-   0        0        0       30 2023-03-21 10:24:52.000000 pypdl-0.0.5/pypdl/__init__.py
--rw-rw-rw-   0        0        0    12053 2023-03-25 16:57:33.000000 pypdl-0.0.5/pypdl/main.py
--rw-rw-rw-   0        0        0      770 2023-03-25 16:56:33.000000 pypdl-0.0.5/pypdl/test.py
--rw-rw-rw-   0        0        0     3901 2023-03-25 14:19:38.000000 pypdl-0.0.5/pypdl/utls.py
-drwxrwxrwx   0        0        0        0 2023-03-25 18:02:18.716144 pypdl-0.0.5/pypdl.egg-info/
--rw-rw-rw-   0        0        0     8170 2023-03-25 18:02:18.000000 pypdl-0.0.5/pypdl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-03-25 18:02:18.000000 pypdl-0.0.5/pypdl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-25 18:02:18.000000 pypdl-0.0.5/pypdl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-03-25 18:02:18.000000 pypdl-0.0.5/pypdl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-25 18:02:18.000000 pypdl-0.0.5/pypdl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-25 18:02:18.720157 pypdl-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      927 2023-03-25 17:54:41.000000 pypdl-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:10:28.139815 pypdl-0.0.6/
+-rw-rw-rw-   0        0        0     1086 2023-03-20 10:21:57.000000 pypdl-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     8170 2023-04-16 17:10:28.138816 pypdl-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7581 2023-03-25 18:04:56.000000 pypdl-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 17:10:28.122077 pypdl-0.0.6/pypdl/
+-rw-rw-rw-   0        0        0       30 2023-03-21 10:24:52.000000 pypdl-0.0.6/pypdl/__init__.py
+-rw-rw-rw-   0        0        0    12123 2023-04-16 17:07:01.000000 pypdl-0.0.6/pypdl/main.py
+-rw-rw-rw-   0        0        0      770 2023-03-25 16:56:33.000000 pypdl-0.0.6/pypdl/test.py
+-rw-rw-rw-   0        0        0     3901 2023-03-25 14:19:38.000000 pypdl-0.0.6/pypdl/utls.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:10:28.138816 pypdl-0.0.6/pypdl.egg-info/
+-rw-rw-rw-   0        0        0     8170 2023-04-16 17:10:28.000000 pypdl-0.0.6/pypdl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-04-16 17:10:28.000000 pypdl-0.0.6/pypdl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 17:10:28.000000 pypdl-0.0.6/pypdl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-16 17:10:28.000000 pypdl-0.0.6/pypdl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-16 17:10:28.000000 pypdl-0.0.6/pypdl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 17:10:28.139815 pypdl-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      927 2023-04-16 17:09:50.000000 pypdl-0.0.6/setup.py
```

### Comparing `pypdl-0.0.5/LICENSE` & `pypdl-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdl-0.0.5/PKG-INFO` & `pypdl-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pypdl
-Version: 0.0.5
+Version: 0.0.6
 Summary: A concurrent python download manager
 Home-page: https://github.com/m-jishnu/pypdl
 Author: m-jishnu
 Author-email: <jishnum499@gmail.com>
 License: MIT
 Keywords: python,downloader,concurrent-downloader,parrel-downloader,download manager,fast-downloader
-Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pypdl
 
 pypdl is a Python library for downloading files from the internet. It provides features such as multi-threaded downloads, retry download incase of failure and option to continue downloading using a different url if necessary, progress tracking, pause/resume functionality and many more.
```

### Comparing `pypdl-0.0.5/README.md` & `pypdl-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pypdl-0.0.5/pypdl/main.py` & `pypdl-0.0.6/pypdl/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,27 +63,28 @@
                 progress = json.loads(json_file.read_text(), object_hook=lambda d: {
                                       int(k) if k.isdigit() else k: v for k, v in d.items()})
             segment = total / num_connections
             self._dic['total'] = total
             self._dic['connections'] = num_connections
             self._dic['paused'] = False
             for i in range(num_connections):
-                if not json_file.exists() or progress == {}:
+                try:
+                    # try to use progress file to resume download
+                    start = progress[i]['start']
+                    end = progress[i]['end']
+                    curr = progress[i]['curr']
+                    size = progress[i]['size']
+                except:
+                    # if not able to use progress file then calculate the start, end, curr and size
                     # calculate the beginning byte offset by multiplying the segment by num_connections.
                     start = int(segment * i)
                     # here end is the ((segment * next part ) - 1 byte) since the last byte is downloaded by next part except for the last part
                     end = int(segment * (i + 1)) - (i != num_connections - 1)
                     curr = start
                     size = end - start + (i != num_connections - 1)
-                else:
-                    # use progress file to resume download
-                    start = progress[i]['start']
-                    end = progress[i]['end']
-                    curr = progress[i]['curr']
-                    size = progress[i]['size']
 
                 self._dic[i] = {
                     'start': start,
                     'curr': curr,
                     'end': end,
                     'filepath': f'{filepath}.{i}.part',
                     'size': size,
```

### Comparing `pypdl-0.0.5/pypdl/test.py` & `pypdl-0.0.6/pypdl/test.py`

 * *Files identical despite different names*

### Comparing `pypdl-0.0.5/pypdl/utls.py` & `pypdl-0.0.6/pypdl/utls.py`

 * *Files identical despite different names*

### Comparing `pypdl-0.0.5/pypdl.egg-info/PKG-INFO` & `pypdl-0.0.6/pypdl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pypdl
-Version: 0.0.5
+Version: 0.0.6
 Summary: A concurrent python download manager
 Home-page: https://github.com/m-jishnu/pypdl
 Author: m-jishnu
 Author-email: <jishnum499@gmail.com>
 License: MIT
 Keywords: python,downloader,concurrent-downloader,parrel-downloader,download manager,fast-downloader
-Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pypdl
 
 pypdl is a Python library for downloading files from the internet. It provides features such as multi-threaded downloads, retry download incase of failure and option to continue downloading using a different url if necessary, progress tracking, pause/resume functionality and many more.
```

### Comparing `pypdl-0.0.5/setup.py` & `pypdl-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'A concurrent python download manager'
 with open("README.md", "r") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name="pypdl",
     version=VERSION,
```

