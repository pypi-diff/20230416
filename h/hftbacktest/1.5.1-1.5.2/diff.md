# Comparing `tmp/hftbacktest-1.5.1.tar.gz` & `tmp/hftbacktest-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hftbacktest-1.5.1.tar", last modified: Sun Apr 16 13:35:56 2023, max compression
+gzip compressed data, was "hftbacktest-1.5.2.tar", last modified: Sun Apr 16 13:59:13 2023, max compression
```

## Comparing `hftbacktest-1.5.1.tar` & `hftbacktest-1.5.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:35:56.435825 hftbacktest-1.5.1/
--rw-r--r--   0 kaz       (1000) kaz       (1000)     1079 2022-11-14 13:24:06.000000 hftbacktest-1.5.1/LICENSE
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     6872 2023-04-16 13:35:56.435825 hftbacktest-1.5.1/PKG-INFO
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     5763 2023-04-16 13:34:17.000000 hftbacktest-1.5.1/README.rst
-drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:35:56.431825 hftbacktest-1.5.1/hftbacktest/
--rw-rw-r--   0 kaz       (1000) kaz       (1000)    11501 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/__init__.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     1011 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/assettype.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)    13846 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/backtest.py
-drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:35:56.431825 hftbacktest-1.5.1/hftbacktest/data/
--rw-r--r--   0 kaz       (1000) kaz       (1000)     1592 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/data/__init__.py
-drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:35:56.431825 hftbacktest-1.5.1/hftbacktest/data/utils/
--rw-r--r--   0 kaz       (1000) kaz       (1000)       44 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/data/utils/__init__.py
--rw-r--r--   0 kaz       (1000) kaz       (1000)    11299 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/data/utils/binancefutures.py
--rw-r--r--   0 kaz       (1000) kaz       (1000)     2160 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/data/utils/snapshot.py
--rw-r--r--   0 kaz       (1000) kaz       (1000)     6707 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/data/utils/tardis.py
--rw-r--r--   0 kaz       (1000) kaz       (1000)    11514 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/data/validation.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     6194 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/marketdepth.py
-drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:35:56.435825 hftbacktest-1.5.1/hftbacktest/models/
--rw-rw-r--   0 kaz       (1000) kaz       (1000)        0 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/models/__init__.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)    10007 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/models/latencies.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     3305 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/models/queue.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     4143 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/order.py
-drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:35:56.435825 hftbacktest-1.5.1/hftbacktest/proc/
--rw-r--r--   0 kaz       (1000) kaz       (1000)        0 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/proc/__init__.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     5866 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/proc/local.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)    14794 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/proc/nopartialfillexchange.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)    22145 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/proc/partialfillexchange.py
--rw-r--r--   0 kaz       (1000) kaz       (1000)     5903 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/proc/proc.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     3252 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/reader.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)    13631 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/stat.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     2149 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/state.py
--rw-r--r--   0 kaz       (1000) kaz       (1000)      876 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/typing.py
-drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:35:56.431825 hftbacktest-1.5.1/hftbacktest.egg-info/
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     6872 2023-04-16 13:35:56.000000 hftbacktest-1.5.1/hftbacktest.egg-info/PKG-INFO
--rw-rw-r--   0 kaz       (1000) kaz       (1000)      908 2023-04-16 13:35:56.000000 hftbacktest-1.5.1/hftbacktest.egg-info/SOURCES.txt
--rw-rw-r--   0 kaz       (1000) kaz       (1000)        1 2023-04-16 13:35:56.000000 hftbacktest-1.5.1/hftbacktest.egg-info/dependency_links.txt
--rw-rw-r--   0 kaz       (1000) kaz       (1000)        1 2023-02-22 13:33:16.000000 hftbacktest-1.5.1/hftbacktest.egg-info/not-zip-safe
--rw-rw-r--   0 kaz       (1000) kaz       (1000)       48 2023-04-16 13:35:56.000000 hftbacktest-1.5.1/hftbacktest.egg-info/requires.txt
--rw-rw-r--   0 kaz       (1000) kaz       (1000)       12 2023-04-16 13:35:56.000000 hftbacktest-1.5.1/hftbacktest.egg-info/top_level.txt
--rw-r--r--   0 kaz       (1000) kaz       (1000)     1249 2023-04-16 13:35:56.435825 hftbacktest-1.5.1/setup.cfg
--rw-r--r--   0 kaz       (1000) kaz       (1000)       61 2023-02-22 13:27:55.000000 hftbacktest-1.5.1/setup.py
+drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:59:13.758521 hftbacktest-1.5.2/
+-rw-r--r--   0 kaz       (1000) kaz       (1000)     1079 2022-11-14 13:24:06.000000 hftbacktest-1.5.2/LICENSE
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)     6872 2023-04-16 13:59:13.758521 hftbacktest-1.5.2/PKG-INFO
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)     5763 2023-04-16 13:46:03.000000 hftbacktest-1.5.2/README.rst
+drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:59:13.750521 hftbacktest-1.5.2/hftbacktest/
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)    11501 2023-04-16 13:48:02.000000 hftbacktest-1.5.2/hftbacktest/__init__.py
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)     1011 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/assettype.py
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)    13846 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/backtest.py
+drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:59:13.754521 hftbacktest-1.5.2/hftbacktest/data/
+-rw-r--r--   0 kaz       (1000) kaz       (1000)     1592 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/data/__init__.py
+drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:59:13.758521 hftbacktest-1.5.2/hftbacktest/data/utils/
+-rw-r--r--   0 kaz       (1000) kaz       (1000)       44 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/data/utils/__init__.py
+-rw-r--r--   0 kaz       (1000) kaz       (1000)    11299 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/data/utils/binancefutures.py
+-rw-r--r--   0 kaz       (1000) kaz       (1000)     2160 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/data/utils/snapshot.py
+-rw-r--r--   0 kaz       (1000) kaz       (1000)     6707 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/data/utils/tardis.py
+-rw-r--r--   0 kaz       (1000) kaz       (1000)    11514 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/data/validation.py
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)     6194 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/marketdepth.py
+drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:59:13.758521 hftbacktest-1.5.2/hftbacktest/models/
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)        0 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/models/__init__.py
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)    10007 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/models/latencies.py
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)     3305 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/models/queue.py
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)     4143 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/order.py
+drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:59:13.758521 hftbacktest-1.5.2/hftbacktest/proc/
+-rw-r--r--   0 kaz       (1000) kaz       (1000)        0 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/proc/__init__.py
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)     5866 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/proc/local.py
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)    14794 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/proc/nopartialfillexchange.py
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)    22145 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/proc/partialfillexchange.py
+-rw-r--r--   0 kaz       (1000) kaz       (1000)     5903 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/proc/proc.py
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)     3252 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/reader.py
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)    13631 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/stat.py
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)     2149 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/state.py
+-rw-r--r--   0 kaz       (1000) kaz       (1000)      876 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/typing.py
+drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:59:13.754521 hftbacktest-1.5.2/hftbacktest.egg-info/
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)     6872 2023-04-16 13:59:13.000000 hftbacktest-1.5.2/hftbacktest.egg-info/PKG-INFO
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)      908 2023-04-16 13:59:13.000000 hftbacktest-1.5.2/hftbacktest.egg-info/SOURCES.txt
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)        1 2023-04-16 13:59:13.000000 hftbacktest-1.5.2/hftbacktest.egg-info/dependency_links.txt
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)        1 2023-02-22 13:33:16.000000 hftbacktest-1.5.2/hftbacktest.egg-info/not-zip-safe
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)       48 2023-04-16 13:59:13.000000 hftbacktest-1.5.2/hftbacktest.egg-info/requires.txt
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)       12 2023-04-16 13:59:13.000000 hftbacktest-1.5.2/hftbacktest.egg-info/top_level.txt
+-rw-r--r--   0 kaz       (1000) kaz       (1000)     1249 2023-04-16 13:59:13.758521 hftbacktest-1.5.2/setup.cfg
+-rw-r--r--   0 kaz       (1000) kaz       (1000)       61 2023-02-22 13:27:55.000000 hftbacktest-1.5.2/setup.py
```

### Comparing `hftbacktest-1.5.1/LICENSE` & `hftbacktest-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.1/PKG-INFO` & `hftbacktest-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hftbacktest
-Version: 1.5.1
+Version: 1.5.2
 Summary: High-frequency trading and market making backtesting tool
 Home-page: https://github.com/nkaz001/hftbacktest
 Author: nkaz001
 Author-email: nkaz001@protonmail.com
 License: MIT
 Project-URL: Docs, https://hftbacktest.readthedocs.io/en/latest/
 Project-URL: GitHub: issues, https://github.com/nkaz001/hftbacktest/issues
@@ -17,15 +17,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Office/Business :: Financial :: Investment
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE
 
 ===========
 HftBacktest
 ===========
 
 |codacy| |codeql| |pypi| |downloads| |license| |docs|
@@ -47,15 +47,15 @@
 
 Getting started
 ===============
 
 Installation
 ------------
 
-hftbacktest supports Python 3.7+. You can install hftbacktest using ``pip``:
+hftbacktest supports Python 3.8+. You can install hftbacktest using ``pip``:
 
 .. code-block:: console
 
  pip install hftbacktest
 
 Or you can clone the latest development version from the Git repository with:
```

### Comparing `hftbacktest-1.5.1/README.rst` & `hftbacktest-1.5.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 Getting started
 ===============
 
 Installation
 ------------
 
-hftbacktest supports Python 3.7+. You can install hftbacktest using ``pip``:
+hftbacktest supports Python 3.8+. You can install hftbacktest using ``pip``:
 
 .. code-block:: console
 
  pip install hftbacktest
 
 Or you can clone the latest development version from the Git repository with:
```

### Comparing `hftbacktest-1.5.1/hftbacktest/__init__.py` & `hftbacktest-1.5.2/hftbacktest/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     'validate_data',
     'correct_local_timestamp',
     'correct_exch_timestamp',
     'correct_exch_timestamp_adjust',
     'correct'
 )
 
-__version__ = '1.5.1'
+__version__ = '1.5.2'
 
 
 # JIT'ed latency models
 ConstantLatency = jitclass()(ConstantLatency_)
 FeedLatency = jitclass()(FeedLatency_)
 ForwardFeedLatency = jitclass()(ForwardFeedLatency_)
 BackwardFeedLatency = jitclass()(BackwardFeedLatency_)
```

### Comparing `hftbacktest-1.5.1/hftbacktest/assettype.py` & `hftbacktest-1.5.2/hftbacktest/assettype.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.1/hftbacktest/backtest.py` & `hftbacktest-1.5.2/hftbacktest/backtest.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.1/hftbacktest/data/__init__.py` & `hftbacktest-1.5.2/hftbacktest/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.1/hftbacktest/data/utils/binancefutures.py` & `hftbacktest-1.5.2/hftbacktest/data/utils/binancefutures.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.1/hftbacktest/data/utils/snapshot.py` & `hftbacktest-1.5.2/hftbacktest/data/utils/snapshot.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.1/hftbacktest/data/utils/tardis.py` & `hftbacktest-1.5.2/hftbacktest/data/utils/tardis.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.1/hftbacktest/data/validation.py` & `hftbacktest-1.5.2/hftbacktest/data/validation.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.1/hftbacktest/marketdepth.py` & `hftbacktest-1.5.2/hftbacktest/marketdepth.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.1/hftbacktest/models/latencies.py` & `hftbacktest-1.5.2/hftbacktest/models/latencies.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.1/hftbacktest/models/queue.py` & `hftbacktest-1.5.2/hftbacktest/models/queue.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.1/hftbacktest/order.py` & `hftbacktest-1.5.2/hftbacktest/order.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.1/hftbacktest/proc/local.py` & `hftbacktest-1.5.2/hftbacktest/proc/local.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.1/hftbacktest/proc/nopartialfillexchange.py` & `hftbacktest-1.5.2/hftbacktest/proc/nopartialfillexchange.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.1/hftbacktest/proc/partialfillexchange.py` & `hftbacktest-1.5.2/hftbacktest/proc/partialfillexchange.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.1/hftbacktest/proc/proc.py` & `hftbacktest-1.5.2/hftbacktest/proc/proc.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.1/hftbacktest/reader.py` & `hftbacktest-1.5.2/hftbacktest/reader.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.1/hftbacktest/stat.py` & `hftbacktest-1.5.2/hftbacktest/stat.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.1/hftbacktest/state.py` & `hftbacktest-1.5.2/hftbacktest/state.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.1/hftbacktest/typing.py` & `hftbacktest-1.5.2/hftbacktest/typing.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.1/hftbacktest.egg-info/PKG-INFO` & `hftbacktest-1.5.2/hftbacktest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hftbacktest
-Version: 1.5.1
+Version: 1.5.2
 Summary: High-frequency trading and market making backtesting tool
 Home-page: https://github.com/nkaz001/hftbacktest
 Author: nkaz001
 Author-email: nkaz001@protonmail.com
 License: MIT
 Project-URL: Docs, https://hftbacktest.readthedocs.io/en/latest/
 Project-URL: GitHub: issues, https://github.com/nkaz001/hftbacktest/issues
@@ -17,15 +17,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Office/Business :: Financial :: Investment
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE
 
 ===========
 HftBacktest
 ===========
 
 |codacy| |codeql| |pypi| |downloads| |license| |docs|
@@ -47,15 +47,15 @@
 
 Getting started
 ===============
 
 Installation
 ------------
 
-hftbacktest supports Python 3.7+. You can install hftbacktest using ``pip``:
+hftbacktest supports Python 3.8+. You can install hftbacktest using ``pip``:
 
 .. code-block:: console
 
  pip install hftbacktest
 
 Or you can clone the latest development version from the Git repository with:
```

### Comparing `hftbacktest-1.5.1/hftbacktest.egg-info/SOURCES.txt` & `hftbacktest-1.5.2/hftbacktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.1/setup.cfg` & `hftbacktest-1.5.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 	
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	
 	Topic :: Office/Business :: Financial :: Investment
 
 [options]
-python_requires = >=3.7
+python_requires = >=3.8
 packages = find:
 zip_safe = False
 include_package_data = True
 install_requires = 
 	numba ~= 0.56
 	numpy < 1.24, >= 1.18
 	pandas
```

