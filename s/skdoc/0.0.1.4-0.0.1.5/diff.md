# Comparing `tmp/skdoc-0.0.1.4-py3-none-any.whl.zip` & `tmp/skdoc-0.0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 2568 bytes, number of entries: 7
--rw-r--r--  2.0 unx       41 b- defN 23-Apr-16 07:50 skdoc/__init__.py
+Zip file size: 3377 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       21 b- defN 23-Apr-16 13:05 skdoc/__init__.py
 -rw-r--r--  2.0 unx       40 b- defN 23-Apr-16 07:55 skdoc/placeholder.py
--rw-r--r--  2.0 unx     1071 b- defN 23-Apr-16 08:00 skdoc-0.0.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx      933 b- defN 23-Apr-16 08:00 skdoc-0.0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-16 08:00 skdoc-0.0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Apr-16 08:00 skdoc-0.0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      531 b- defN 23-Apr-16 08:00 skdoc-0.0.1.4.dist-info/RECORD
-7 files, 2714 bytes uncompressed, 1622 bytes compressed:  40.2%
+-rw-r--r--  2.0 unx     1280 b- defN 23-Apr-16 13:04 skdoc/report.py
+-rw-r--r--  2.0 unx     1071 b- defN 23-Apr-16 16:15 skdoc-0.0.1.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1165 b- defN 23-Apr-16 16:15 skdoc-0.0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-16 16:15 skdoc-0.0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Apr-16 16:15 skdoc-0.0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      604 b- defN 23-Apr-16 16:15 skdoc-0.0.1.5.dist-info/RECORD
+8 files, 4279 bytes uncompressed, 2325 bytes compressed:  45.7%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
 Filename: skdoc/__init__.py
 Comment: 
 
 Filename: skdoc/placeholder.py
 Comment: 
 
-Filename: skdoc-0.0.1.4.dist-info/LICENSE
+Filename: skdoc/report.py
 Comment: 
 
-Filename: skdoc-0.0.1.4.dist-info/METADATA
+Filename: skdoc-0.0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: skdoc-0.0.1.4.dist-info/WHEEL
+Filename: skdoc-0.0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: skdoc-0.0.1.4.dist-info/top_level.txt
+Filename: skdoc-0.0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: skdoc-0.0.1.4.dist-info/RECORD
+Filename: skdoc-0.0.1.5.dist-info/top_level.txt
+Comment: 
+
+Filename: skdoc-0.0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## skdoc/__init__.py

```diff
@@ -1 +1 @@
-from skdoc.placeholder import placeholder
+from .report import *
```

## Comparing `skdoc-0.0.1.4.dist-info/LICENSE` & `skdoc-0.0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

