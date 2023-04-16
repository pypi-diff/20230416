# Comparing `tmp/pydicts-0.2.0.tar.gz` & `tmp/pydicts-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydicts-0.2.0.tar", max compression
+gzip compressed data, was "pydicts-0.3.0.tar", max compression
```

## Comparing `pydicts-0.2.0.tar` & `pydicts-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-04-10 16:27:20.112887 pydicts-0.2.0/LICENSE
--rw-r--r--   0        0        0     2044 2023-04-12 05:43:21.075383 pydicts-0.2.0/README.md
--rw-r--r--   0        0        0      143 2023-04-12 05:41:59.410380 pydicts-0.2.0/pydicts/__init__.py
--rw-r--r--   0        0        0     2814 2023-04-11 05:44:25.702913 pydicts-0.2.0/pydicts/classes.py
--rw-r--r--   0        0        0     5382 2023-04-12 05:11:39.114325 pydicts-0.2.0/pydicts/lod.py
--rw-r--r--   0        0        0     1052 2023-04-12 05:25:02.458349 pydicts-0.2.0/pydicts/lod_xyv.py
--rw-r--r--   0        0        0     3199 2023-04-12 05:34:00.504366 pydicts-0.2.0/pydicts/lod_ymv.py
--rw-r--r--   0        0        0        0 2023-04-10 16:27:20.112887 pydicts-0.2.0/pydicts/tests/__init__.py
--rw-r--r--   0        0        0      913 2023-04-12 05:37:22.137372 pydicts-0.2.0/pydicts/tests/test_lod.py
--rw-r--r--   0        0        0      409 2023-04-12 05:32:28.379363 pydicts-0.2.0/pydicts/tests/test_lod_ymv.py
--rw-r--r--   0        0        0      407 2023-04-12 05:46:36.401389 pydicts-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2561 1970-01-01 00:00:00.000000 pydicts-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-10 16:27:20.112887 pydicts-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2829 2023-04-16 10:00:29.766815 pydicts-0.3.0/README.md
+-rw-r--r--   0        0        0      144 2023-04-16 09:59:09.244813 pydicts-0.3.0/pydicts/__init__.py
+-rw-r--r--   0        0        0     2814 2023-04-11 05:44:25.702913 pydicts-0.3.0/pydicts/classes.py
+-rw-r--r--   0        0        0     5382 2023-04-12 05:11:39.114325 pydicts-0.3.0/pydicts/lod.py
+-rw-r--r--   0        0        0     1052 2023-04-12 05:25:02.458349 pydicts-0.3.0/pydicts/lod_xyv.py
+-rw-r--r--   0        0        0     8792 2023-04-15 22:54:44.487769 pydicts-0.3.0/pydicts/lod_ymv.py
+-rw-r--r--   0        0        0        0 2023-04-10 16:27:20.112887 pydicts-0.3.0/pydicts/tests/__init__.py
+-rw-r--r--   0        0        0      913 2023-04-12 05:37:22.137372 pydicts-0.3.0/pydicts/tests/test_lod.py
+-rw-r--r--   0        0        0      409 2023-04-12 05:32:28.379363 pydicts-0.3.0/pydicts/tests/test_lod_ymv.py
+-rw-r--r--   0        0        0      407 2023-04-16 09:58:44.859812 pydicts-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3346 1970-01-01 00:00:00.000000 pydicts-0.3.0/PKG-INFO
```

### Comparing `pydicts-0.2.0/LICENSE` & `pydicts-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydicts-0.2.0/pydicts/classes.py` & `pydicts-0.3.0/pydicts/classes.py`

 * *Files identical despite different names*

### Comparing `pydicts-0.2.0/pydicts/lod.py` & `pydicts-0.3.0/pydicts/lod.py`

 * *Files identical despite different names*

### Comparing `pydicts-0.2.0/pydicts/lod_xyv.py` & `pydicts-0.3.0/pydicts/lod_xyv.py`

 * *Files identical despite different names*

### Comparing `pydicts-0.2.0/pydicts/tests/test_lod.py` & `pydicts-0.3.0/pydicts/tests/test_lod.py`

 * *Files identical despite different names*

### Comparing `pydicts-0.2.0/PKG-INFO` & `pydicts-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,60 @@
 Metadata-Version: 2.1
 Name: pydicts
-Version: 0.2.0
+Version: 0.3.0
 Summary: Module to use dictionaries in various situations
 License: GPL-3.0
 Author: turulomio
 Author-email: turulomio@yahoo.es
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
-# pydicts
-Module to use dictionaries in various situations
+# PyDicts  [![PyPI - Downloads](https://img.shields.io/pypi/dm/pydicts?label=Pypi%20downloads)](https://pypi.org/project/pydicts/)
+
+Module to use dictionaries, list of dictionaries and other data structures 
+
+I've developed this module because I needed this kind of methods developing with Django and python
 
 ## Acronyms
 pydicts uses several acronyms to call functions and parameters
 
 - lod: List of dictionaries `[{"a":1,"b":2}, {"a":3,"b":4}]`
 - lood: List of ordered dictionaries (OrderedDicts from collections module) `[OrderedDict([('a', 1), ('b', 2)]), OrderedDict([('a', 3), ('b', 4)])]`
 - lol: List of lists `[[1, 2, 3], [4, 5, 6]]` 
 - dod: Dictionary of dictionaries `{'key2': {'a': 1, 'b': 2}, 'key1': {'a': 1, 'b': 2}}`
 - lod_ymv: List of dictionaries with year-month-value keys `[{'year': 2021, 'month': 1, 'value': 12.12}, {'year': 2023, 'month': 3, 'value': 13.03}]`
 - lod_xyv: List of dictionaries with x-y-value keys `[{'X': 21, 'Y': 12, 'value': 180}, {'X': 2, 'Y': 122, 'value': 170}]`
 
 ## LOD
+
+### dod2lod
+
+### lod2dictkv
+
+### lod2dod
+
+### lod2dod_tuple
+
+### lod2list
+
+### lod2list_distinct
+
+### lod2lol
+
+### lod2lood
+
+### lod_average
+
+### lod_average_ponderated
+
 ### lod_has_key
 
 Returns a boolean. Checks if list of dictionaries has a key
 
 ```python
 >>> from pydicts.lod import lod_has_key
 >>> lod=[{"a":1, "b":4},{"a":2, "b":5}]
@@ -38,14 +62,26 @@
 True
 >>> lod_has_key(lod,"d")
 False
 >>> lod_has_key([],"d")
 False
 ```
 
+### lod_max
+
+### lod_max_value
+
+### lod_median
+
+### lod_min
+
+### lod_min_value
+
+### lod_order_by
+
 ### lod_print
 
 Prints a list of dictionaries in a tabulated way
 
 ```python
 >>> from pydicts.lod import lod_print
 >>> lod=[{"a":1, "b":4},{"a":2, "b":None}]
@@ -54,14 +90,16 @@
 |   a |   b |
 |-----+-----|
 |   1 |   4 |
 |   2 |     |
 +-----+-----+
 ```
 
+### lod_rename_key
+
 ### lod_sum
 
 Sums all values from a lod key. None values are ignored by default
 
 ```python
 >>> from pydicts.lod import lod_sum
 >>> lod=[{"a":1, "b":4},{"a":2, "b":None}]
@@ -73,20 +111,38 @@
 Traceback (most recent call last):
   File "<stdin>", line 1, in <module>
   File "/home/keko/Proyectos/pydicts/pydicts/lod.py", line 46, in lod_sum
     r=r+d[key]
 TypeError: unsupported operand type(s) for +: 'int' and 'NoneType'
 ```
 
+### lod_sum_negatives
+
+### lod_sum_positives
+
+## LOD_XYV
+
+### lod_xyv_transformation
+
+## LOD_YMV
+
+### lod_ymv_transposition
+
+### lod_ymv_transposition_sum
+
+### lod_ymv_filling
 
 ## Testing
 poetry run pytest
 
 ## CHANGELOG
 
+### 0.3.0 (2023-04-16)
+- Added lod_ymv_transposition_with_porcentages
+
 ### 0.2.0 (2023-04-12)
 - Added lod_print with tabulate module
 - Improving documentation
 - Refactorized modules to lod_xyv, lod_ymmv
 
 ### 0.1.0 (2023-04-10)
 - First version addapting listdict_functions from reusingcode
```

