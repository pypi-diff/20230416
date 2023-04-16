# Comparing `tmp/xia_engine_terraform-0.0.2-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_terraform-0.0.4-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 154211 bytes, number of entries: 7
--rw-r--r--  2.0 unx      201 b- defN 23-Apr-16 16:11 xia_engine_terraform/__init__.py
--rw-r--r--  2.0 unx   388096 b- defN 23-Apr-16 16:45 xia_engine_terraform/engine.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-16 16:45 xia_engine_terraform-0.0.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      700 b- defN 23-Apr-16 16:45 xia_engine_terraform-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-16 16:45 xia_engine_terraform-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-Apr-16 16:45 xia_engine_terraform-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      646 b- defN 23-Apr-16 16:45 xia_engine_terraform-0.0.2.dist-info/RECORD
-7 files, 389915 bytes uncompressed, 153045 bytes compressed:  60.7%
+Zip file size: 129408 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      394 b- defN 23-Apr-16 20:13 xia_engine_terraform/__init__.py
+-rw-r--r--  2.0 unx   356104 b- defN 23-Apr-16 20:13 xia_engine_terraform/engine.cpython-310-darwin.so
+-rw-r--r--  2.0 unx      152 b- defN 23-Apr-16 20:13 xia_engine_terraform-0.0.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      699 b- defN 23-Apr-16 20:13 xia_engine_terraform-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Apr-16 20:13 xia_engine_terraform-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-Apr-16 20:13 xia_engine_terraform-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      650 b- defN 23-Apr-16 20:13 xia_engine_terraform-0.0.4.dist-info/RECORD
+7 files, 358128 bytes uncompressed, 128236 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_terraform/__init__.py
 Comment: 
 
-Filename: xia_engine_terraform/engine.cp39-win_amd64.pyd
+Filename: xia_engine_terraform/engine.cpython-310-darwin.so
 Comment: 
 
-Filename: xia_engine_terraform-0.0.2.dist-info/LICENSE.txt
+Filename: xia_engine_terraform-0.0.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_terraform-0.0.2.dist-info/METADATA
+Filename: xia_engine_terraform-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_terraform-0.0.2.dist-info/WHEEL
+Filename: xia_engine_terraform-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_terraform-0.0.2.dist-info/top_level.txt
+Filename: xia_engine_terraform-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_terraform-0.0.2.dist-info/RECORD
+Filename: xia_engine_terraform-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_terraform/__init__.py

```diff
@@ -1,8 +1,10 @@
 from xia_engine_terraform.engine import TerraformEngine, TerraformConnectParam, TerraformClient
+from xia_engine_terraform.engine import TerraformLocalEngine, TerraformLocalConnectParam, TerraformLocalClient
 
 
 __all__ = [
-    "TerraformEngine", "TerraformConnectParam", "TerraformClient"
+    "TerraformEngine", "TerraformConnectParam", "TerraformClient",
+    "TerraformLocalEngine", "TerraformLocalConnectParam", "TerraformLocalClient"
 ]
 
-__version__ = "0.0.2"
+__version__ = "0.0.4"
```

## Comparing `xia_engine_terraform-0.0.2.dist-info/METADATA` & `xia_engine_terraform-0.0.4.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: xia-engine-terraform
-Version: 0.0.2
+Version: 0.0.4
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform/0.0.2/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform/0.0.4/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: jinja2
+Requires-Dist: google-cloud-storage
 Requires-Dist: xia-engine
 
 .. image:: https://img.shields.io/pypi/v/xia-engine-terraform.svg?color=blue
    :alt: PyPI-Server
    :target: https://pypi.org/project/xia-engine-terraform/
 
 ====================================
@@ -27,9 +26,7 @@
 =============================
 
 Install the package::
 
     pip install
 
 
-
-
```

