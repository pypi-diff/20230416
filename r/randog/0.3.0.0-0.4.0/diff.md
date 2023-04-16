# Comparing `tmp/randog-0.3.0.0.tar.gz` & `tmp/randog-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "randog-0.3.0.0.tar", last modified: Sat Mar 25 02:00:00 2023, max compression
+gzip compressed data, was "randog-0.4.0.tar", last modified: Sun Apr 16 06:41:50 2023, max compression
```

## Comparing `randog-0.3.0.0.tar` & `randog-0.4.0.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 02:00:00.091379 randog-0.3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-25 01:59:50.000000 randog-0.3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-03-25 02:00:00.091379 randog-0.3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-25 01:59:50.000000 randog-0.3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 02:00:00.083379 randog-0.3.0.0/randog/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-25 01:59:50.000000 randog-0.3.0.0/randog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-03-25 01:59:50.000000 randog-0.3.0.0/randog/_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 02:00:00.083379 randog-0.3.0.0/randog/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-25 01:59:50.000000 randog-0.3.0.0/randog/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-25 01:59:50.000000 randog-0.3.0.0/randog/_utils/nullsafe.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-25 01:59:50.000000 randog-0.3.0.0/randog/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 02:00:00.091379 randog-0.3.0.0/randog/factory/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-25 01:59:50.000000 randog-0.3.0.0/randog/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-03-25 01:59:50.000000 randog-0.3.0.0/randog/factory/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-03-25 01:59:50.000000 randog-0.3.0.0/randog/factory/_bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-25 01:59:50.000000 randog-0.3.0.0/randog/factory/_by_callable.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-25 01:59:50.000000 randog-0.3.0.0/randog/factory/_by_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-03-25 01:59:50.000000 randog-0.3.0.0/randog/factory/_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-25 01:59:50.000000 randog-0.3.0.0/randog/factory/_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-03-25 01:59:50.000000 randog-0.3.0.0/randog/factory/_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-03-25 01:59:50.000000 randog-0.3.0.0/randog/factory/_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-03-25 01:59:50.000000 randog-0.3.0.0/randog/factory/_decimal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-03-25 01:59:50.000000 randog-0.3.0.0/randog/factory/_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-03-25 01:59:50.000000 randog-0.3.0.0/randog/factory/_float.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-03-25 01:59:50.000000 randog-0.3.0.0/randog/factory/_from_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-03-25 01:59:50.000000 randog-0.3.0.0/randog/factory/_int.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-03-25 01:59:50.000000 randog-0.3.0.0/randog/factory/_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-03-25 01:59:50.000000 randog-0.3.0.0/randog/factory/_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-03-25 01:59:50.000000 randog-0.3.0.0/randog/factory/_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-03-25 01:59:50.000000 randog-0.3.0.0/randog/factory/_timedelta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-03-25 01:59:50.000000 randog-0.3.0.0/randog/factory/_union.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 02:00:00.083379 randog-0.3.0.0/randog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-03-25 01:59:59.000000 randog-0.3.0.0/randog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-25 01:59:59.000000 randog-0.3.0.0/randog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:59:59.000000 randog-0.3.0.0/randog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-25 01:59:59.000000 randog-0.3.0.0/randog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 02:00:00.091379 randog-0.3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-03-25 01:59:50.000000 randog-0.3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:41:50.052102 randog-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-16 06:41:40.000000 randog-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-16 06:41:50.052102 randog-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-16 06:41:40.000000 randog-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:41:50.052102 randog-0.4.0/randog/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-16 06:41:41.000000 randog-0.4.0/randog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-04-16 06:41:41.000000 randog-0.4.0/randog/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-16 06:41:41.000000 randog-0.4.0/randog/_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:41:50.052102 randog-0.4.0/randog/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:41:41.000000 randog-0.4.0/randog/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-16 06:41:41.000000 randog-0.4.0/randog/_utils/nullsafe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-16 06:41:41.000000 randog-0.4.0/randog/_utils/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-16 06:41:41.000000 randog-0.4.0/randog/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:41:50.052102 randog-0.4.0/randog/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_by_callable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_by_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_from_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_from_pyfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_timedelta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_union.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:41:50.052102 randog-0.4.0/randog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-16 06:41:49.000000 randog-0.4.0/randog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-16 06:41:49.000000 randog-0.4.0/randog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 06:41:49.000000 randog-0.4.0/randog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-16 06:41:49.000000 randog-0.4.0/randog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 06:41:50.052102 randog-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-16 06:41:41.000000 randog-0.4.0/setup.py
```

### Comparing `randog-0.3.0.0/LICENSE` & `randog-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `randog-0.3.0.0/PKG-INFO` & `randog-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: randog
-Version: 0.3.0.0
+Version: 0.4.0
 Summary: Generate data randomly
 Home-page: UNKNOWN
 Author: k-izumi
 Author-email: k.izumi.ysk@gmail.com
 Maintainer: k-izumi
 Maintainer-email: k.izumi.ysk@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/unaguna/random-obj-generator/issues
 Project-URL: Documentation, https://unaguna.github.io/random-obj-generator/
 Project-URL: Source Code, https://github.com/unaguna/random-obj-generator
-Description: **randog 0.3.0.x — Randomly object generator**
+Description: **randog 0.4.0 — Randomly object generator**
         
         **randog** is a package which helps to generate data randomly.
         
         ## Install
         
         You can install from PyPI.
```

### Comparing `randog-0.3.0.0/README.md` & `randog-0.4.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-**randog 0.3.0.x — Randomly object generator**
+**randog 0.4.0 — Randomly object generator**
 
 **randog** is a package which helps to generate data randomly.
 
 ## Install
 
 You can install from PyPI.
```

### Comparing `randog-0.3.0.0/randog/_examples.py` & `randog-0.4.0/randog/_examples.py`

 * *Files identical despite different names*

### Comparing `randog-0.3.0.0/randog/factory/__init__.py` & `randog-0.4.0/randog/factory/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,18 +12,20 @@
 from ._datetime import DatetimeRandomFactory, randdatetime
 from ._list import randlist
 from ._dict import DictItem, DictRandomFactory, randdict
 from ._by_callable import ByCallableFactory, by_callable
 from ._by_iterator import ByIteratorFactory, by_iterator
 from ._union import UnionRandomFactory, union
 from ._from_example import from_example, FromExampleContext
+from ._from_pyfile import from_pyfile
 
 __all__ = [
     "from_example",
     "FromExampleContext",
+    "from_pyfile",
     "Factory",
     "randchoice",
     "const",
     "randbool",
     "randint",
     "randfloat",
     "randdecimal",
```

### Comparing `randog-0.3.0.0/randog/factory/_base.py` & `randog-0.4.0/randog/factory/_base.py`

 * *Files identical despite different names*

### Comparing `randog-0.3.0.0/randog/factory/_bool.py` & `randog-0.4.0/randog/factory/_bool.py`

 * *Files identical despite different names*

### Comparing `randog-0.3.0.0/randog/factory/_by_callable.py` & `randog-0.4.0/randog/factory/_by_callable.py`

 * *Files identical despite different names*

### Comparing `randog-0.3.0.0/randog/factory/_by_iterator.py` & `randog-0.4.0/randog/factory/_by_iterator.py`

 * *Files identical despite different names*

### Comparing `randog-0.3.0.0/randog/factory/_choice.py` & `randog-0.4.0/randog/factory/_choice.py`

 * *Files identical despite different names*

### Comparing `randog-0.3.0.0/randog/factory/_date.py` & `randog-0.4.0/randog/factory/_date.py`

 * *Files identical despite different names*

### Comparing `randog-0.3.0.0/randog/factory/_datetime.py` & `randog-0.4.0/randog/factory/_datetime.py`

 * *Files identical despite different names*

### Comparing `randog-0.3.0.0/randog/factory/_decimal.py` & `randog-0.4.0/randog/factory/_decimal.py`

 * *Files identical despite different names*

### Comparing `randog-0.3.0.0/randog/factory/_dict.py` & `randog-0.4.0/randog/factory/_dict.py`

 * *Files identical despite different names*

### Comparing `randog-0.3.0.0/randog/factory/_float.py` & `randog-0.4.0/randog/factory/_float.py`

 * *Files identical despite different names*

### Comparing `randog-0.3.0.0/randog/factory/_from_example.py` & `randog-0.4.0/randog/factory/_from_example.py`

 * *Files identical despite different names*

### Comparing `randog-0.3.0.0/randog/factory/_int.py` & `randog-0.4.0/randog/factory/_int.py`

 * *Files identical despite different names*

### Comparing `randog-0.3.0.0/randog/factory/_list.py` & `randog-0.4.0/randog/factory/_list.py`

 * *Files identical despite different names*

### Comparing `randog-0.3.0.0/randog/factory/_str.py` & `randog-0.4.0/randog/factory/_str.py`

 * *Files identical despite different names*

### Comparing `randog-0.3.0.0/randog/factory/_time.py` & `randog-0.4.0/randog/factory/_time.py`

 * *Files identical despite different names*

### Comparing `randog-0.3.0.0/randog/factory/_timedelta.py` & `randog-0.4.0/randog/factory/_timedelta.py`

 * *Files identical despite different names*

### Comparing `randog-0.3.0.0/randog/factory/_union.py` & `randog-0.4.0/randog/factory/_union.py`

 * *Files identical despite different names*

### Comparing `randog-0.3.0.0/randog.egg-info/PKG-INFO` & `randog-0.4.0/randog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: randog
-Version: 0.3.0.0
+Version: 0.4.0
 Summary: Generate data randomly
 Home-page: UNKNOWN
 Author: k-izumi
 Author-email: k.izumi.ysk@gmail.com
 Maintainer: k-izumi
 Maintainer-email: k.izumi.ysk@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/unaguna/random-obj-generator/issues
 Project-URL: Documentation, https://unaguna.github.io/random-obj-generator/
 Project-URL: Source Code, https://github.com/unaguna/random-obj-generator
-Description: **randog 0.3.0.x — Randomly object generator**
+Description: **randog 0.4.0 — Randomly object generator**
         
         **randog** is a package which helps to generate data randomly.
         
         ## Install
         
         You can install from PyPI.
```

### Comparing `randog-0.3.0.0/randog.egg-info/SOURCES.txt` & `randog-0.4.0/randog.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 LICENSE
 README.md
 setup.py
 randog/__init__.py
+randog/__main__.py
 randog/_examples.py
 randog/exceptions.py
 randog.egg-info/PKG-INFO
 randog.egg-info/SOURCES.txt
 randog.egg-info/dependency_links.txt
 randog.egg-info/top_level.txt
 randog/_utils/__init__.py
 randog/_utils/nullsafe.py
+randog/_utils/type.py
 randog/factory/__init__.py
 randog/factory/_base.py
 randog/factory/_bool.py
 randog/factory/_by_callable.py
 randog/factory/_by_iterator.py
 randog/factory/_choice.py
 randog/factory/_const.py
 randog/factory/_date.py
 randog/factory/_datetime.py
 randog/factory/_decimal.py
 randog/factory/_dict.py
 randog/factory/_float.py
 randog/factory/_from_example.py
+randog/factory/_from_pyfile.py
 randog/factory/_int.py
 randog/factory/_list.py
 randog/factory/_str.py
 randog/factory/_time.py
 randog/factory/_timedelta.py
 randog/factory/_union.py
```

### Comparing `randog-0.3.0.0/setup.py` & `randog-0.4.0/setup.py`

 * *Files identical despite different names*

