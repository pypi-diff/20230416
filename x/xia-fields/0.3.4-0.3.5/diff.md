# Comparing `tmp/xia_fields-0.3.4-cp39-none-win_amd64.whl.zip` & `tmp/xia_fields-0.3.5-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 459514 bytes, number of entries: 9
--rw-r--r--  2.0 unx     1177 b- defN 23-Mar-30 20:36 xia_fields/__init__.py
--rw-r--r--  2.0 unx   366080 b- defN 23-Mar-30 20:40 xia_fields/base.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   415232 b- defN 23-Mar-30 20:41 xia_fields/fields.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   385024 b- defN 23-Mar-30 20:42 xia_fields/fields_ext.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Mar-30 20:42 xia_fields-0.3.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     3308 b- defN 23-Mar-30 20:42 xia_fields-0.3.4.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Mar-30 20:42 xia_fields-0.3.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Mar-30 20:42 xia_fields-0.3.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      770 b- defN 23-Mar-30 20:42 xia_fields-0.3.4.dist-info/RECORD
-9 files, 1171853 bytes uncompressed, 458188 bytes compressed:  60.9%
+Zip file size: 385092 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     1177 b- defN 23-Apr-16 09:20 xia_fields/__init__.py
+-rw-r--r--  2.0 unx   324328 b- defN 23-Apr-16 09:21 xia_fields/base.cpython-310-darwin.so
+-rw-r--r--  2.0 unx   376344 b- defN 23-Apr-16 09:20 xia_fields/fields.cpython-310-darwin.so
+-rw-r--r--  2.0 unx   358792 b- defN 23-Apr-16 09:20 xia_fields/fields_ext.cpython-310-darwin.so
+-rw-r--r--  2.0 unx      152 b- defN 23-Apr-16 09:21 xia_fields-0.3.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     3271 b- defN 23-Apr-16 09:21 xia_fields-0.3.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Apr-16 09:21 xia_fields-0.3.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-16 09:21 xia_fields-0.3.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      780 b- defN 23-Apr-16 09:21 xia_fields-0.3.5.dist-info/RECORD
+9 files, 1064963 bytes uncompressed, 383748 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: xia_fields/__init__.py
 Comment: 
 
-Filename: xia_fields/base.cp39-win_amd64.pyd
+Filename: xia_fields/base.cpython-310-darwin.so
 Comment: 
 
-Filename: xia_fields/fields.cp39-win_amd64.pyd
+Filename: xia_fields/fields.cpython-310-darwin.so
 Comment: 
 
-Filename: xia_fields/fields_ext.cp39-win_amd64.pyd
+Filename: xia_fields/fields_ext.cpython-310-darwin.so
 Comment: 
 
-Filename: xia_fields-0.3.4.dist-info/LICENSE.txt
+Filename: xia_fields-0.3.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_fields-0.3.4.dist-info/METADATA
+Filename: xia_fields-0.3.5.dist-info/METADATA
 Comment: 
 
-Filename: xia_fields-0.3.4.dist-info/WHEEL
+Filename: xia_fields-0.3.5.dist-info/WHEEL
 Comment: 
 
-Filename: xia_fields-0.3.4.dist-info/top_level.txt
+Filename: xia_fields-0.3.5.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_fields-0.3.4.dist-info/RECORD
+Filename: xia_fields-0.3.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_fields/__init__.py

```diff
@@ -14,8 +14,8 @@
     "JsonField", "DictField", "CompressedStringField",
     "Int64Field", "Int32Field", "SFixed64Field", "SFixed32Field",
     "UInt64Field", "UInt32Field", "Fixed64Field", "Fixed32Field",
     "DoubleField", "DateField", "TimestampField", "TimeField", "DateTimeField",
     "OsEnvironField"
 ]
 
-__version__ = "0.3.4"
+__version__ = "0.3.5"
```

## Comparing `xia_fields-0.3.4.dist-info/METADATA` & `xia_fields-0.3.5.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: xia-fields
-Version: 0.3.4
+Version: 0.3.5
 Summary: X-I-A Field Protocol
-Home-page: https://develop.x-i-a.com/docs/xia-fields/0.3.4/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-fields/0.3.5/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 .. image:: https://img.shields.io/pypi/v/xia-fields.svg?color=blue
    :alt: PyPI-Server
    :target: https://pypi.org/project/xia-fields/
@@ -94,9 +92,7 @@
 Each field could has it own validation process by overriding `validate()` method.
 Here are the already defined validation parameter applied for ALL fields:
 
 * required: Field value couldn't be None
 * min_value: Minimum value
 * max_value: Maximum value
 * choices: Value must be defined among those values
-
-
```

