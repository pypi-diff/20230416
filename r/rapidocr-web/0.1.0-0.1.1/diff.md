# Comparing `tmp/rapidocr_web-0.1.0-py3-none-any.whl.zip` & `tmp/rapidocr_web-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 42644 bytes, number of entries: 13
--rw-r--r--  2.0 unx       74 b- defN 23-Apr-16 02:52 rapidocr_web/__init__.py
--rw-r--r--  2.0 unx     1492 b- defN 23-Apr-16 02:52 rapidocr_web/api.py
--rw-r--r--  2.0 unx     1128 b- defN 23-Apr-16 02:52 rapidocr_web/ocrweb.py
--rw-r--r--  2.0 unx     2954 b- defN 23-Apr-16 02:52 rapidocr_web/task.py
--rw-r--r--  2.0 unx    16958 b- defN 23-Apr-16 02:52 rapidocr_web/static/css/favicon.ico
--rw-r--r--  2.0 unx     2065 b- defN 23-Apr-16 02:52 rapidocr_web/static/css/main.css
--rw-r--r--  2.0 unx    86341 b- defN 23-Apr-16 02:52 rapidocr_web/static/js/jquery-3.0.0.min.js
--rw-r--r--  2.0 unx     8202 b- defN 23-Apr-16 02:52 rapidocr_web/templates/index.html
--rw-r--r--  2.0 unx     4576 b- defN 23-Apr-16 02:53 rapidocr_web-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-16 02:53 rapidocr_web-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       96 b- defN 23-Apr-16 02:53 rapidocr_web-0.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-Apr-16 02:53 rapidocr_web-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1101 b- defN 23-Apr-16 02:53 rapidocr_web-0.1.0.dist-info/RECORD
-13 files, 125092 bytes uncompressed, 40794 bytes compressed:  67.4%
+Zip file size: 42638 bytes, number of entries: 13
+-rw-r--r--  2.0 unx       74 b- defN 23-Apr-16 03:00 rapidocr_web/__init__.py
+-rw-r--r--  2.0 unx     1492 b- defN 23-Apr-16 03:00 rapidocr_web/api.py
+-rw-r--r--  2.0 unx     1128 b- defN 23-Apr-16 03:00 rapidocr_web/ocrweb.py
+-rw-r--r--  2.0 unx     2954 b- defN 23-Apr-16 03:00 rapidocr_web/task.py
+-rw-r--r--  2.0 unx    16958 b- defN 23-Apr-16 03:00 rapidocr_web/static/css/favicon.ico
+-rw-r--r--  2.0 unx     2065 b- defN 23-Apr-16 03:00 rapidocr_web/static/css/main.css
+-rw-r--r--  2.0 unx    86341 b- defN 23-Apr-16 03:00 rapidocr_web/static/js/jquery-3.0.0.min.js
+-rw-r--r--  2.0 unx     8202 b- defN 23-Apr-16 03:00 rapidocr_web/templates/index.html
+-rw-r--r--  2.0 unx     4576 b- defN 23-Apr-16 03:00 rapidocr_web-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-16 03:00 rapidocr_web-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       96 b- defN 23-Apr-16 03:00 rapidocr_web-0.1.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-Apr-16 03:00 rapidocr_web-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1101 b- defN 23-Apr-16 03:00 rapidocr_web-0.1.1.dist-info/RECORD
+13 files, 125092 bytes uncompressed, 40788 bytes compressed:  67.4%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: rapidocr_web/static/js/jquery-3.0.0.min.js
 Comment: 
 
 Filename: rapidocr_web/templates/index.html
 Comment: 
 
-Filename: rapidocr_web-0.1.0.dist-info/METADATA
+Filename: rapidocr_web-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: rapidocr_web-0.1.0.dist-info/WHEEL
+Filename: rapidocr_web-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: rapidocr_web-0.1.0.dist-info/entry_points.txt
+Filename: rapidocr_web-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapidocr_web-0.1.0.dist-info/top_level.txt
+Filename: rapidocr_web-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: rapidocr_web-0.1.0.dist-info/RECORD
+Filename: rapidocr_web-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `rapidocr_web-0.1.0.dist-info/METADATA` & `rapidocr_web-0.1.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidocr-web
-Version: 0.1.0
+Version: 0.1.1
 Summary: A cross platform OCR Library based on OnnxRuntime.
 Home-page: https://github.com/RapidAI/RapidOCR
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Download-URL: https://github.com/RapidAI/RapidOCR.git
 Keywords: ocr,text_detection,text_recognition,db,onnxruntime,paddleocr,openvino,rapidocr
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rapidocr-web Version: 0.1.0 Summary: A cross
+Metadata-Version: 2.1 Name: rapidocr-web Version: 0.1.1 Summary: A cross
 platform OCR Library based on OnnxRuntime. Home-page: https://github.com/
 RapidAI/RapidOCR Author: SWHL Author-email: liekkaskono@163.com License:
 Apache-2.0 Download-URL: https://github.com/RapidAI/RapidOCR.git Keywords:
 ocr,text_detection,text_recognition,db,onnxruntime,paddleocr,openvino,rapidocr
 Platform: Any Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

## Comparing `rapidocr_web-0.1.0.dist-info/RECORD` & `rapidocr_web-0.1.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 rapidocr_web/api.py,sha256=u6Vc7e93XQYyuPX6EOiafgfi0EY-mKf7tingL2CSmIw,1492
 rapidocr_web/ocrweb.py,sha256=fw9XEBoJZqUjbH19izaHJvXfQ-prwO_LoPjQuE3g8QY,1128
 rapidocr_web/task.py,sha256=l6PrccgTQDcvS8ZppZMfYuIPCYK-6ym_-02NWRm4Uak,2954
 rapidocr_web/static/css/favicon.ico,sha256=CBE1NF6iiIax8WqZVR-vPRaPTcmWjlTWsk1fzEbSd8c,16958
 rapidocr_web/static/css/main.css,sha256=2HcVvoa5oSQONnuC6IjjmBd127Jv9Y5EFJGy32nTEZk,2065
 rapidocr_web/static/js/jquery-3.0.0.min.js,sha256=JmvOoLtYsmqlsWxa7mDSLMwa6dZ9rrIdtrrVYRnDRH0,86341
 rapidocr_web/templates/index.html,sha256=xUe3Xce289Of4XTfeafPTX5JMRsOTdgv2Md5EQwxm48,8202
-rapidocr_web-0.1.0.dist-info/METADATA,sha256=fiDI35xhftWUoJ2zgaGwuMZQNbfcuS2kN6tLnnO4Sv4,4576
-rapidocr_web-0.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rapidocr_web-0.1.0.dist-info/entry_points.txt,sha256=q3Vx7ES3NeGhonzyiGS8mVFDVVgK-J5M8bGSktcC92I,96
-rapidocr_web-0.1.0.dist-info/top_level.txt,sha256=dArjxF38AFvTF1Ae-mGaxBhwnETUJ4sLF_nQ93HC5A4,13
-rapidocr_web-0.1.0.dist-info/RECORD,,
+rapidocr_web-0.1.1.dist-info/METADATA,sha256=7C3yB0iuZsd_0j94IVT9U6CZURq_-yB5xqfT0086xtI,4576
+rapidocr_web-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rapidocr_web-0.1.1.dist-info/entry_points.txt,sha256=gKWhYdRif2OyYYQBX6An49Q7XaLO-nuCR2AoIp6LrS8,96
+rapidocr_web-0.1.1.dist-info/top_level.txt,sha256=dArjxF38AFvTF1Ae-mGaxBhwnETUJ4sLF_nQ93HC5A4,13
+rapidocr_web-0.1.1.dist-info/RECORD,,
```

