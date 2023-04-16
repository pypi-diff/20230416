# Comparing `tmp/skdoc-0.0.1.1-py3-none-any.whl.zip` & `tmp/skdoc-0.0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2110 bytes, number of entries: 5
--rw-r--r--  2.0 unx     1071 b- defN 23-Apr-16 07:32 skdoc-0.0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      997 b- defN 23-Apr-16 07:32 skdoc-0.0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-16 07:32 skdoc-0.0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-16 07:32 skdoc-0.0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      385 b- defN 23-Apr-16 07:32 skdoc-0.0.1.1.dist-info/RECORD
-5 files, 2557 bytes uncompressed, 1390 bytes compressed:  45.6%
+Zip file size: 2138 bytes, number of entries: 5
+-rw-r--r--  2.0 unx     1071 b- defN 23-Apr-16 07:36 skdoc-0.0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1039 b- defN 23-Apr-16 07:36 skdoc-0.0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-16 07:36 skdoc-0.0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-16 07:36 skdoc-0.0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      386 b- defN 23-Apr-16 07:36 skdoc-0.0.1.2.dist-info/RECORD
+5 files, 2600 bytes uncompressed, 1418 bytes compressed:  45.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: skdoc-0.0.1.1.dist-info/LICENSE
+Filename: skdoc-0.0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: skdoc-0.0.1.1.dist-info/METADATA
+Filename: skdoc-0.0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: skdoc-0.0.1.1.dist-info/WHEEL
+Filename: skdoc-0.0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: skdoc-0.0.1.1.dist-info/top_level.txt
+Filename: skdoc-0.0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: skdoc-0.0.1.1.dist-info/RECORD
+Filename: skdoc-0.0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `skdoc-0.0.1.1.dist-info/LICENSE` & `skdoc-0.0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `skdoc-0.0.1.1.dist-info/METADATA` & `skdoc-0.0.1.2.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: skdoc
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: Automated documentation engine for scikit-learn models
 Home-page: UNKNOWN
+Author: ['Denis Abdullin', 'Emile Antat']
 Author-email: denisabdullincz@gmail.com
 License: UNKNOWN
 Keywords: python,scikit-learn,sklearn,machine learning,documentation
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

