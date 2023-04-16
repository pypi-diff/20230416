# Comparing `tmp/skdoc-0.0.1.3-py3-none-any.whl.zip` & `tmp/skdoc-0.0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2560 bytes, number of entries: 7
--rw-r--r--  2.0 unx       35 b- defN 23-Apr-16 07:47 skdoc/__init__.py
--rw-r--r--  2.0 unx       40 b- defN 23-Apr-16 07:15 skdoc/placeholder.py
--rw-r--r--  2.0 unx     1071 b- defN 23-Apr-16 07:47 skdoc-0.0.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx      933 b- defN 23-Apr-16 07:47 skdoc-0.0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-16 07:47 skdoc-0.0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Apr-16 07:47 skdoc-0.0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      531 b- defN 23-Apr-16 07:47 skdoc-0.0.1.3.dist-info/RECORD
-7 files, 2708 bytes uncompressed, 1614 bytes compressed:  40.4%
+Zip file size: 2568 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       41 b- defN 23-Apr-16 07:50 skdoc/__init__.py
+-rw-r--r--  2.0 unx       40 b- defN 23-Apr-16 07:55 skdoc/placeholder.py
+-rw-r--r--  2.0 unx     1071 b- defN 23-Apr-16 08:00 skdoc-0.0.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx      933 b- defN 23-Apr-16 08:00 skdoc-0.0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-16 08:00 skdoc-0.0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Apr-16 08:00 skdoc-0.0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      531 b- defN 23-Apr-16 08:00 skdoc-0.0.1.4.dist-info/RECORD
+7 files, 2714 bytes uncompressed, 1622 bytes compressed:  40.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: skdoc/__init__.py
 Comment: 
 
 Filename: skdoc/placeholder.py
 Comment: 
 
-Filename: skdoc-0.0.1.3.dist-info/LICENSE
+Filename: skdoc-0.0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: skdoc-0.0.1.3.dist-info/METADATA
+Filename: skdoc-0.0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: skdoc-0.0.1.3.dist-info/WHEEL
+Filename: skdoc-0.0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: skdoc-0.0.1.3.dist-info/top_level.txt
+Filename: skdoc-0.0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: skdoc-0.0.1.3.dist-info/RECORD
+Filename: skdoc-0.0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## skdoc/__init__.py

```diff
@@ -1 +1 @@
-from placeholder import placeholder
+from skdoc.placeholder import placeholder
```

## Comparing `skdoc-0.0.1.3.dist-info/LICENSE` & `skdoc-0.0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `skdoc-0.0.1.3.dist-info/METADATA` & `skdoc-0.0.1.4.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skdoc
-Version: 0.0.1.3
+Version: 0.0.1.4
 Summary: Automated documentation engine for scikit-learn models
 Home-page: UNKNOWN
 Author: Denis Abdullin, Emile Antat
 Author-email: denisabdullincz@gmail.com, eoea754@gmail.com
 License: UNKNOWN
 Keywords: python,scikit-learn,sklearn,machine learning,documentation
 Platform: UNKNOWN
```

