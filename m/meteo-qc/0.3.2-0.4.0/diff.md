# Comparing `tmp/meteo_qc-0.3.2.tar.gz` & `tmp/meteo_qc-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meteo_qc-0.3.2.tar", last modified: Sat Jan 21 18:54:28 2023, max compression
+gzip compressed data, was "meteo_qc-0.4.0.tar", last modified: Sun Apr 16 20:05:40 2023, max compression
```

## Comparing `meteo_qc-0.3.2.tar` & `meteo_qc-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 kittnjdr  (1000) kittnjdr  (1000)        0 2023-01-21 18:54:28.139593 meteo_qc-0.3.2/
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     1070 2022-11-24 10:14:49.000000 meteo_qc-0.3.2/LICENCE
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     6266 2023-01-21 18:54:28.139593 meteo_qc-0.3.2/PKG-INFO
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     5703 2023-01-21 18:53:08.000000 meteo_qc-0.3.2/README.md
-drwxrwxr-x   0 kittnjdr  (1000) kittnjdr  (1000)        0 2023-01-21 18:54:28.139593 meteo_qc-0.3.2/meteo_qc/
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)      544 2022-11-29 17:25:49.000000 meteo_qc-0.3.2/meteo_qc/__init__.py
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     3016 2022-11-29 21:27:44.000000 meteo_qc-0.3.2/meteo_qc/_colum_mapping.py
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     4311 2022-11-29 21:30:56.000000 meteo_qc-0.3.2/meteo_qc/_data.py
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     5349 2022-12-08 21:03:52.000000 meteo_qc-0.3.2/meteo_qc/_main.py
-drwxrwxr-x   0 kittnjdr  (1000) kittnjdr  (1000)        0 2023-01-21 18:54:28.139593 meteo_qc-0.3.2/meteo_qc/_plugins/
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)        0 2022-11-24 10:14:49.000000 meteo_qc-0.3.2/meteo_qc/_plugins/__init__.py
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     1784 2022-12-07 14:02:36.000000 meteo_qc-0.3.2/meteo_qc/_plugins/generic.py
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     8796 2023-01-18 18:24:54.000000 meteo_qc-0.3.2/meteo_qc/_plugins/values.py
-drwxrwxr-x   0 kittnjdr  (1000) kittnjdr  (1000)        0 2023-01-21 18:54:28.139593 meteo_qc-0.3.2/meteo_qc.egg-info/
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     6266 2023-01-21 18:54:28.000000 meteo_qc-0.3.2/meteo_qc.egg-info/PKG-INFO
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)      366 2023-01-21 18:54:28.000000 meteo_qc-0.3.2/meteo_qc.egg-info/SOURCES.txt
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)        1 2023-01-21 18:54:28.000000 meteo_qc-0.3.2/meteo_qc.egg-info/dependency_links.txt
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)        7 2023-01-21 18:54:28.000000 meteo_qc-0.3.2/meteo_qc.egg-info/requires.txt
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)        9 2023-01-21 18:54:28.000000 meteo_qc-0.3.2/meteo_qc.egg-info/top_level.txt
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     1154 2023-01-21 18:54:28.139593 meteo_qc-0.3.2/setup.cfg
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)       37 2022-11-24 10:14:49.000000 meteo_qc-0.3.2/setup.py
+drwxrwxr-x   0 kittnjdr  (1000) kittnjdr  (1000)        0 2023-04-16 20:05:40.956931 meteo_qc-0.4.0/
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     1070 2022-11-24 10:14:49.000000 meteo_qc-0.4.0/LICENCE
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     6266 2023-04-16 20:05:40.956931 meteo_qc-0.4.0/PKG-INFO
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     5703 2023-01-21 18:53:08.000000 meteo_qc-0.4.0/README.md
+drwxrwxr-x   0 kittnjdr  (1000) kittnjdr  (1000)        0 2023-04-16 20:05:40.956931 meteo_qc-0.4.0/meteo_qc/
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)      544 2022-11-29 17:25:49.000000 meteo_qc-0.4.0/meteo_qc/__init__.py
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     3016 2022-11-29 21:27:44.000000 meteo_qc-0.4.0/meteo_qc/_colum_mapping.py
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     4311 2022-11-29 21:30:56.000000 meteo_qc-0.4.0/meteo_qc/_data.py
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     5349 2022-12-08 21:03:52.000000 meteo_qc-0.4.0/meteo_qc/_main.py
+drwxrwxr-x   0 kittnjdr  (1000) kittnjdr  (1000)        0 2023-04-16 20:05:40.956931 meteo_qc-0.4.0/meteo_qc/_plugins/
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)        0 2022-11-24 10:14:49.000000 meteo_qc-0.4.0/meteo_qc/_plugins/__init__.py
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     2368 2023-04-14 16:53:40.000000 meteo_qc-0.4.0/meteo_qc/_plugins/generic.py
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     9361 2023-04-14 17:31:13.000000 meteo_qc-0.4.0/meteo_qc/_plugins/values.py
+drwxrwxr-x   0 kittnjdr  (1000) kittnjdr  (1000)        0 2023-04-16 20:05:40.956931 meteo_qc-0.4.0/meteo_qc.egg-info/
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     6266 2023-04-16 20:05:40.000000 meteo_qc-0.4.0/meteo_qc.egg-info/PKG-INFO
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)      366 2023-04-16 20:05:40.000000 meteo_qc-0.4.0/meteo_qc.egg-info/SOURCES.txt
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)        1 2023-04-16 20:05:40.000000 meteo_qc-0.4.0/meteo_qc.egg-info/dependency_links.txt
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)        7 2023-04-16 20:05:40.000000 meteo_qc-0.4.0/meteo_qc.egg-info/requires.txt
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)        9 2023-04-16 20:05:40.000000 meteo_qc-0.4.0/meteo_qc.egg-info/top_level.txt
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     1154 2023-04-16 20:05:40.956931 meteo_qc-0.4.0/setup.cfg
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)       37 2022-11-24 10:14:49.000000 meteo_qc-0.4.0/setup.py
```

### Comparing `meteo_qc-0.3.2/LICENCE` & `meteo_qc-0.4.0/LICENCE`

 * *Files identical despite different names*

### Comparing `meteo_qc-0.3.2/PKG-INFO` & `meteo_qc-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meteo_qc
-Version: 0.3.2
+Version: 0.4.0
 Summary: quality control meteorological data in a pandas.DataFrame
 Home-page: https://github.com/jkittner/meteo-qc
 Author: Jonas Kittner
 Author-email: jkittner@users.noreply.github.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `meteo_qc-0.3.2/README.md` & `meteo_qc-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `meteo_qc-0.3.2/meteo_qc/__init__.py` & `meteo_qc-0.4.0/meteo_qc/__init__.py`

 * *Files identical despite different names*

### Comparing `meteo_qc-0.3.2/meteo_qc/_colum_mapping.py` & `meteo_qc-0.4.0/meteo_qc/_colum_mapping.py`

 * *Files identical despite different names*

### Comparing `meteo_qc-0.3.2/meteo_qc/_data.py` & `meteo_qc-0.4.0/meteo_qc/_data.py`

 * *Files identical despite different names*

### Comparing `meteo_qc-0.3.2/meteo_qc/_main.py` & `meteo_qc-0.4.0/meteo_qc/_main.py`

 * *Files identical despite different names*

### Comparing `meteo_qc-0.3.2/meteo_qc/_plugins/values.py` & `meteo_qc-0.4.0/meteo_qc/_plugins/values.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import math
 from datetime import timedelta
 
 import pandas as pd
 
 from meteo_qc._data import register
 from meteo_qc._data import Result
 
@@ -42,49 +43,60 @@
         delta: float,
 ) -> tuple[bool, pd.DataFrame]:
     df = s.to_frame()
 
     def _compare(s: pd.Series[float]) -> bool:
         if len(s) == 1:
             return False
-        return bool(abs(s[0] - s[1]) > delta)
+
+        diff = abs(s[0] - s[1])
+        if math.isnan(diff):
+            return False
+
+        return bool(diff > delta)
 
     df['flag'] = df.rolling(
         window=2,
         min_periods=1,
         closed='right',
-    ).apply(_compare).astype(bool)
+    ).apply(_compare)
+    # if there are not enough valid obervations, rolling returns NaN.
+    # Converting this to a bool results in True sind float('nan') is truthy
+    # set all NaN to False, since we don't want to flag them here
+    df['flag'] = df['flag'].replace([float('nan')], [0.0]).astype(bool)
     # TODO: also return where, and make sure the spike or dip is labelled
-    # correctly
-    return bool(df['flag'].any()), df[df['flag'] == True]  # noqa: E712
+    # correctly with surroundings, maybe an additional rolling?
+    data: pd.DataFrame = df[df['flag'] == True]  # type: ignore[assignment] # noqa: E712,E501
+    return bool(df['flag'].any()), data
 
 
 def _is_persistent(
         s: pd.Series[float],
         window: int,
         excludes: list[float],
 ) -> tuple[bool, pd.DataFrame]:
     df = s.to_frame()
     df['flag'] = False
     if len(df) <= window:
-        return False, df[df['flag'] == True]  # noqa: E712
+        return False, df[df['flag'] == True]  # type: ignore[return-value] # noqa: E712,E501
 
     def _equals(x: pd.Series[float]) -> bool:
         if len(x) >= window:
             first_val = x.iloc[0]
             return bool(((x == first_val) & (~x.isin(excludes))).all())
         else:
             return False
 
     df['flag'] = df[s.name].rolling(
         window=window,
         min_periods=1,
         closed='right',
     ).apply(_equals).astype(bool)
-    return bool(df['flag'].any()), df[df['flag'] == True]  # noqa: E712
+    data: pd.DataFrame = df[df['flag'] == True]  # type: ignore[assignment] # noqa: E712,E501
+    return bool(df['flag'].any()), data
 
 
 @register('temperature', lower_bound=-40, upper_bound=50)
 @register('dew_point', lower_bound=-60, upper_bound=50)
 @register('relhum', lower_bound=10, upper_bound=100)
 @register('windspeed', lower_bound=0, upper_bound=30)
 @register('winddirection', lower_bound=0, upper_bound=360)
```

### Comparing `meteo_qc-0.3.2/meteo_qc.egg-info/PKG-INFO` & `meteo_qc-0.4.0/meteo_qc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meteo-qc
-Version: 0.3.2
+Version: 0.4.0
 Summary: quality control meteorological data in a pandas.DataFrame
 Home-page: https://github.com/jkittner/meteo-qc
 Author: Jonas Kittner
 Author-email: jkittner@users.noreply.github.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `meteo_qc-0.3.2/setup.cfg` & `meteo_qc-0.4.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = meteo_qc
-version = 0.3.2
+version = 0.4.0
 description = quality control meteorological data in a pandas.DataFrame
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jkittner/meteo-qc
 author = Jonas Kittner
 author_email = jkittner@users.noreply.github.com
 license = MIT
```

