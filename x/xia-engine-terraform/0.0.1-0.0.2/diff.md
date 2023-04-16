# Comparing `tmp/xia_engine_terraform-0.0.1-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_terraform-0.0.2-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 156214 bytes, number of entries: 7
--rw-r--r--  2.0 unx      166 b- defN 23-Apr-15 16:24 xia_engine_terraform/__init__.py
--rw-r--r--  2.0 unx   389632 b- defN 23-Apr-16 06:14 xia_engine_terraform/engine.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-16 06:14 xia_engine_terraform-0.0.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      700 b- defN 23-Apr-16 06:14 xia_engine_terraform-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-16 06:14 xia_engine_terraform-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-Apr-16 06:14 xia_engine_terraform-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      646 b- defN 23-Apr-16 06:14 xia_engine_terraform-0.0.1.dist-info/RECORD
-7 files, 391416 bytes uncompressed, 155048 bytes compressed:  60.4%
+Zip file size: 154211 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      201 b- defN 23-Apr-16 16:11 xia_engine_terraform/__init__.py
+-rw-r--r--  2.0 unx   388096 b- defN 23-Apr-16 16:45 xia_engine_terraform/engine.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-16 16:45 xia_engine_terraform-0.0.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      700 b- defN 23-Apr-16 16:45 xia_engine_terraform-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-16 16:45 xia_engine_terraform-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-Apr-16 16:45 xia_engine_terraform-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      646 b- defN 23-Apr-16 16:45 xia_engine_terraform-0.0.2.dist-info/RECORD
+7 files, 389915 bytes uncompressed, 153045 bytes compressed:  60.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_terraform/__init__.py
 Comment: 
 
 Filename: xia_engine_terraform/engine.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_engine_terraform-0.0.1.dist-info/LICENSE.txt
+Filename: xia_engine_terraform-0.0.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_terraform-0.0.1.dist-info/METADATA
+Filename: xia_engine_terraform-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_terraform-0.0.1.dist-info/WHEEL
+Filename: xia_engine_terraform-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_terraform-0.0.1.dist-info/top_level.txt
+Filename: xia_engine_terraform-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_terraform-0.0.1.dist-info/RECORD
+Filename: xia_engine_terraform-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_terraform/__init__.py

```diff
@@ -1,8 +1,8 @@
-from xia_engine_terraform.engine import TerraformEngine, TerraformConnectParam
+from xia_engine_terraform.engine import TerraformEngine, TerraformConnectParam, TerraformClient
 
 
 __all__ = [
-    "TerraformEngine", "TerraformConnectParam",
+    "TerraformEngine", "TerraformConnectParam", "TerraformClient"
 ]
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
```

## Comparing `xia_engine_terraform-0.0.1.dist-info/METADATA` & `xia_engine_terraform-0.0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine-terraform
-Version: 0.0.1
+Version: 0.0.2
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform/0.0.1/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform/0.0.2/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_engine_terraform-0.0.1.dist-info/RECORD` & `xia_engine_terraform-0.0.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_engine_terraform/__init__.py,sha256=leFwzVDd_wdmdMW6o7EM9FbvEKjFHGqQhLRY0tFZK3g,166
-xia_engine_terraform/engine.cp39-win_amd64.pyd,sha256=jFSQuRWrKhc2lfPJZnvl8BtFrIE869REr5eOAt_d3pg,389632
-xia_engine_terraform-0.0.1.dist-info/LICENSE.txt,sha256=WB-w9CuI3gzpFzRjX4F3eIZ56mg24bUewXiu42z75DU,152
-xia_engine_terraform-0.0.1.dist-info/METADATA,sha256=01SQrkGUF954MO5UCRXIyGTuBmKgCncW6gbcE2KqpXs,700
-xia_engine_terraform-0.0.1.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_engine_terraform-0.0.1.dist-info/top_level.txt,sha256=9T86e-QQo91fnAOB3rD5xeM_4EPL7Edk_oOlmR_xquQ,21
-xia_engine_terraform-0.0.1.dist-info/RECORD,,
+xia_engine_terraform/__init__.py,sha256=yOWHD2830jVm9TpfKtbLbVusOuZ9C34RCYeUzmd5Unc,201
+xia_engine_terraform/engine.cp39-win_amd64.pyd,sha256=IA_7fMp2_5MSYc3hcWPtKVDgROzVUcQZYFSraKqrK-0,388096
+xia_engine_terraform-0.0.2.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
+xia_engine_terraform-0.0.2.dist-info/METADATA,sha256=EQSYb90ULLcx0IqKYm63ZowNqw3LnrRH1a9xfkR_1MQ,700
+xia_engine_terraform-0.0.2.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_engine_terraform-0.0.2.dist-info/top_level.txt,sha256=9T86e-QQo91fnAOB3rD5xeM_4EPL7Edk_oOlmR_xquQ,21
+xia_engine_terraform-0.0.2.dist-info/RECORD,,
```

