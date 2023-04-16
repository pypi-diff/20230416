# Comparing `tmp/md410_2023_conv_common-2.30.0.tar.gz` & `tmp/md410_2023_conv_common-2.31.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md410_2023_conv_common-2.30.0.tar", max compression
+gzip compressed data, was "md410_2023_conv_common-2.31.0.tar", max compression
```

## Comparing `md410_2023_conv_common-2.30.0.tar` & `md410_2023_conv_common-2.31.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       22 2021-11-21 15:16:13.135043 md410_2023_conv_common-2.30.0/md410_2023_conv_common/__init__.py
--rw-r--r--   0        0        0     1565 2022-11-20 17:36:07.421701 md410_2023_conv_common-2.30.0/md410_2023_conv_common/build_pdf.py
--rw-r--r--   0        0        0      126 2023-03-26 18:50:48.341169 md410_2023_conv_common-2.30.0/md410_2023_conv_common/constants.py
--rw-r--r--   0        0        0      732 2022-12-03 15:46:20.199481 md410_2023_conv_common-2.30.0/md410_2023_conv_common/data.json
--rw-r--r--   0        0        0     1747 2022-11-23 19:06:38.833446 md410_2023_conv_common-2.30.0/md410_2023_conv_common/emailer.py
--rw-r--r--   0        0        0     3885 2023-04-02 18:26:14.690792 md410_2023_conv_common-2.30.0/md410_2023_conv_common/models.py
--rw-r--r--   0        0        0     1132 2023-04-02 18:59:20.727548 md410_2023_conv_common-2.30.0/md410_2023_conv_common/parse_partial_reg_csv.py
--rw-r--r--   0        0        0      337 2023-03-27 19:41:11.870834 md410_2023_conv_common-2.30.0/md410_2023_conv_common/partial_data.json
--rw-r--r--   0        0        0      929 2022-11-21 18:50:52.563758 md410_2023_conv_common-2.30.0/md410_2023_conv_common/sqs.py
--rw-r--r--   0        0        0   257914 2022-11-23 19:07:34.648965 md410_2023_conv_common-2.30.0/md410_2023_conv_common/test.pdf
--rw-r--r--   0        0        0      652 2023-04-02 19:01:08.877058 md410_2023_conv_common-2.30.0/pyproject.toml
--rw-r--r--   0        0        0      233 2022-11-20 18:26:26.731254 md410_2023_conv_common-2.30.0/readme.md
--rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 md410_2023_conv_common-2.30.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2021-11-21 15:16:13.135043 md410_2023_conv_common-2.31.0/md410_2023_conv_common/__init__.py
+-rw-r--r--   0        0        0     1565 2022-11-20 17:36:07.421701 md410_2023_conv_common-2.31.0/md410_2023_conv_common/build_pdf.py
+-rw-r--r--   0        0        0      126 2023-03-26 18:50:48.341169 md410_2023_conv_common-2.31.0/md410_2023_conv_common/constants.py
+-rw-r--r--   0        0        0      732 2022-12-03 15:46:20.199481 md410_2023_conv_common-2.31.0/md410_2023_conv_common/data.json
+-rw-r--r--   0        0        0     1747 2022-11-23 19:06:38.833446 md410_2023_conv_common-2.31.0/md410_2023_conv_common/emailer.py
+-rw-r--r--   0        0        0     4018 2023-04-07 15:53:34.813247 md410_2023_conv_common-2.31.0/md410_2023_conv_common/models.py
+-rw-r--r--   0        0        0     1132 2023-04-02 18:59:20.727548 md410_2023_conv_common-2.31.0/md410_2023_conv_common/parse_partial_reg_csv.py
+-rw-r--r--   0        0        0      337 2023-03-27 19:41:11.870834 md410_2023_conv_common-2.31.0/md410_2023_conv_common/partial_data.json
+-rw-r--r--   0        0        0      929 2022-11-21 18:50:52.563758 md410_2023_conv_common-2.31.0/md410_2023_conv_common/sqs.py
+-rw-r--r--   0        0        0   257914 2022-11-23 19:07:34.648965 md410_2023_conv_common-2.31.0/md410_2023_conv_common/test.pdf
+-rw-r--r--   0        0        0      652 2023-04-16 06:47:20.446887 md410_2023_conv_common-2.31.0/pyproject.toml
+-rw-r--r--   0        0        0      233 2022-11-20 18:26:26.731254 md410_2023_conv_common-2.31.0/readme.md
+-rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 md410_2023_conv_common-2.31.0/PKG-INFO
```

### Comparing `md410_2023_conv_common-2.30.0/md410_2023_conv_common/build_pdf.py` & `md410_2023_conv_common-2.31.0/md410_2023_conv_common/build_pdf.py`

 * *Files identical despite different names*

### Comparing `md410_2023_conv_common-2.30.0/md410_2023_conv_common/data.json` & `md410_2023_conv_common-2.31.0/md410_2023_conv_common/data.json`

 * *Files identical despite different names*

### Comparing `md410_2023_conv_common-2.30.0/md410_2023_conv_common/emailer.py` & `md410_2023_conv_common-2.31.0/md410_2023_conv_common/emailer.py`

 * *Files identical despite different names*

### Comparing `md410_2023_conv_common-2.30.0/md410_2023_conv_common/models.py` & `md410_2023_conv_common-2.31.0/md410_2023_conv_common/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,32 +103,41 @@
             self.name_badge = self.full_name
             self.auto_name_badge = True
 
 
 class PartialRegistrationItems(BaseModel):
     welcome: int = 0
     dist_conv: int = 0
+    banquet: int = 0
     md_conv: int = 0
     theme: int = 0
     pins: int = 0
 
+
 class PartialRegistration(BaseModel):
     reg_num: Optional[int]
     attendee: PartialAttendeeModel
     items: PartialRegistrationItems
     timestamp: datetime
     cost: float = 0
     emails: Optional[list]
     names: Optional[str]
     reg_num_string: Optional[str]
 
     def __init__(self, **data: Any):
         super().__init__(**data)
         if not self.cost:
-            for field in ("welcome", "dist_conv", "banquet", "md_conv", "theme", "pins"):
+            for field in (
+                "welcome",
+                "dist_conv",
+                "banquet",
+                "md_conv",
+                "theme",
+                "pins",
+            ):
                 self.cost += getattr(constants, f"COST_{field.upper()}", 0) * getattr(
                     self.items, field, 0
                 )
         if self.attendee.email:
             self.emails = [self.attendee.email]
         else:
             self.emails = None
```

### Comparing `md410_2023_conv_common-2.30.0/md410_2023_conv_common/parse_partial_reg_csv.py` & `md410_2023_conv_common-2.31.0/md410_2023_conv_common/parse_partial_reg_csv.py`

 * *Files identical despite different names*

### Comparing `md410_2023_conv_common-2.30.0/md410_2023_conv_common/sqs.py` & `md410_2023_conv_common-2.31.0/md410_2023_conv_common/sqs.py`

 * *Files identical despite different names*

### Comparing `md410_2023_conv_common-2.30.0/md410_2023_conv_common/test.pdf` & `md410_2023_conv_common-2.31.0/md410_2023_conv_common/test.pdf`

 * *Files identical despite different names*

### Comparing `md410_2023_conv_common-2.30.0/pyproject.toml` & `md410_2023_conv_common-2.31.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "md410_2023_conv_common"
-version = "2.30.0"
+version = "2.31.0"
 description = "Common libraries for applications related to the 2023 Lions MD410 Convention"
 authors = ["Kim van Wyk <vanwykk@gmail.com>"]
 repository = "https://gitlab.com/md410_2023_conv/md410_2023_conv_common"
 readme = "readme.md" 
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `md410_2023_conv_common-2.30.0/PKG-INFO` & `md410_2023_conv_common-2.31.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md410-2023-conv-common
-Version: 2.30.0
+Version: 2.31.0
 Summary: Common libraries for applications related to the 2023 Lions MD410 Convention
 Home-page: https://gitlab.com/md410_2023_conv/md410_2023_conv_common
 Author: Kim van Wyk
 Author-email: vanwykk@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

