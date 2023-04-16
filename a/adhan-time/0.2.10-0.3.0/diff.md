# Comparing `tmp/adhan_time-0.2.10.tar.gz` & `tmp/adhan_time-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adhan_time-0.2.10.tar", max compression
+gzip compressed data, was "adhan_time-0.3.0.tar", max compression
```

## Comparing `adhan_time-0.2.10.tar` & `adhan_time-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-04-16 15:41:08.846886 adhan_time-0.2.10/LICENSE
--rw-r--r--   0        0        0       60 2023-04-16 15:41:08.846886 adhan_time-0.2.10/README.md
--rw-r--r--   0        0        0       69 2023-04-16 15:41:08.846886 adhan_time-0.2.10/adhan/__init__.py
--rw-r--r--   0        0        0     1265 2023-04-16 15:41:08.846886 adhan_time-0.2.10/adhan/client.py
--rw-r--r--   0        0        0       51 2023-04-16 15:41:08.846886 adhan_time-0.2.10/adhan/const.py
--rw-r--r--   0        0        0      456 2023-04-16 15:41:08.846886 adhan_time-0.2.10/adhan/models.py
--rw-r--r--   0        0        0      449 2023-04-16 15:41:08.846886 adhan_time-0.2.10/adhan/utils.py
--rw-r--r--   0        0        0      597 2023-04-16 15:41:22.587073 adhan_time-0.2.10/pyproject.toml
--rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 adhan_time-0.2.10/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-07 16:48:47.839077 adhan_time-0.3.0/LICENSE
+-rw-r--r--   0        0        0       60 2023-04-07 16:48:47.839175 adhan_time-0.3.0/README.md
+-rw-r--r--   0        0        0       69 2023-04-07 17:07:58.337323 adhan_time-0.3.0/adhan/__init__.py
+-rw-r--r--   0        0        0     1265 2023-04-08 11:54:53.944612 adhan_time-0.3.0/adhan/client.py
+-rw-r--r--   0        0        0       51 2023-04-08 11:54:13.084228 adhan_time-0.3.0/adhan/const.py
+-rw-r--r--   0        0        0      456 2023-04-08 11:11:03.572063 adhan_time-0.3.0/adhan/models.py
+-rw-r--r--   0        0        0      449 2023-04-08 11:23:44.568585 adhan_time-0.3.0/adhan/utils.py
+-rw-r--r--   0        0        0      596 2023-04-08 13:09:44.253431 adhan_time-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 adhan_time-0.3.0/PKG-INFO
```

### Comparing `adhan_time-0.2.10/LICENSE` & `adhan_time-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adhan_time-0.2.10/adhan/client.py` & `adhan_time-0.3.0/adhan/client.py`

 * *Files identical despite different names*

### Comparing `adhan_time-0.2.10/pyproject.toml` & `adhan_time-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "adhan-time"
-version = "0.2.10"
+version = "0.3.0"
 description = "A complete wrapper for the aladhan API"
 authors = ["Abdullah Ahmed <abdullah@softcomnetworks.com>"]
 homepage = "https://github.com/geektype/adhan.py"
 repository = "https://github.com/geektype/adhan.py"
 license = "Apache License 2.0"
 keywords = ["adhan", "prayer", "aladhan", "prayer times", "islamic prayer times"]
 readme = "README.md"
```

### Comparing `adhan_time-0.2.10/PKG-INFO` & `adhan_time-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adhan-time
-Version: 0.2.10
+Version: 0.3.0
 Summary: A complete wrapper for the aladhan API
 Home-page: https://github.com/geektype/adhan.py
 License: Apache-2.0
 Keywords: adhan,prayer,aladhan,prayer times,islamic prayer times
 Author: Abdullah Ahmed
 Author-email: abdullah@softcomnetworks.com
 Requires-Python: >=3.10,<4.0
```

