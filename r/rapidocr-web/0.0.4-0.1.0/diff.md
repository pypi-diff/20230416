# Comparing `tmp/rapidocr_web-0.0.4-py3-none-any.whl.zip` & `tmp/rapidocr_web-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 41403 bytes, number of entries: 12
--rw-r--r--  2.0 unx       74 b- defN 23-Mar-28 11:16 rapidocr_web/__init__.py
--rw-r--r--  2.0 unx     1414 b- defN 23-Mar-28 11:16 rapidocr_web/ocrweb.py
--rw-r--r--  2.0 unx     3206 b- defN 23-Mar-28 11:16 rapidocr_web/task.py
--rw-r--r--  2.0 unx    16958 b- defN 23-Mar-28 11:16 rapidocr_web/static/css/favicon.ico
--rw-r--r--  2.0 unx     2065 b- defN 23-Mar-28 11:16 rapidocr_web/static/css/main.css
--rw-r--r--  2.0 unx    86341 b- defN 23-Mar-28 11:16 rapidocr_web/static/js/jquery-3.0.0.min.js
--rw-r--r--  2.0 unx     8202 b- defN 23-Mar-28 11:16 rapidocr_web/templates/index.html
--rw-r--r--  2.0 unx     2644 b- defN 23-Mar-28 11:17 rapidocr_web-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-28 11:17 rapidocr_web-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 23-Mar-28 11:17 rapidocr_web-0.0.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-Mar-28 11:17 rapidocr_web-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1025 b- defN 23-Mar-28 11:17 rapidocr_web-0.0.4.dist-info/RECORD
-12 files, 122093 bytes uncompressed, 39667 bytes compressed:  67.5%
+Zip file size: 42644 bytes, number of entries: 13
+-rw-r--r--  2.0 unx       74 b- defN 23-Apr-16 02:52 rapidocr_web/__init__.py
+-rw-r--r--  2.0 unx     1492 b- defN 23-Apr-16 02:52 rapidocr_web/api.py
+-rw-r--r--  2.0 unx     1128 b- defN 23-Apr-16 02:52 rapidocr_web/ocrweb.py
+-rw-r--r--  2.0 unx     2954 b- defN 23-Apr-16 02:52 rapidocr_web/task.py
+-rw-r--r--  2.0 unx    16958 b- defN 23-Apr-16 02:52 rapidocr_web/static/css/favicon.ico
+-rw-r--r--  2.0 unx     2065 b- defN 23-Apr-16 02:52 rapidocr_web/static/css/main.css
+-rw-r--r--  2.0 unx    86341 b- defN 23-Apr-16 02:52 rapidocr_web/static/js/jquery-3.0.0.min.js
+-rw-r--r--  2.0 unx     8202 b- defN 23-Apr-16 02:52 rapidocr_web/templates/index.html
+-rw-r--r--  2.0 unx     4576 b- defN 23-Apr-16 02:53 rapidocr_web-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-16 02:53 rapidocr_web-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       96 b- defN 23-Apr-16 02:53 rapidocr_web-0.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-Apr-16 02:53 rapidocr_web-0.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1101 b- defN 23-Apr-16 02:53 rapidocr_web-0.1.0.dist-info/RECORD
+13 files, 125092 bytes uncompressed, 40794 bytes compressed:  67.4%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: rapidocr_web/__init__.py
 Comment: 
 
+Filename: rapidocr_web/api.py
+Comment: 
+
 Filename: rapidocr_web/ocrweb.py
 Comment: 
 
 Filename: rapidocr_web/task.py
 Comment: 
 
 Filename: rapidocr_web/static/css/favicon.ico
@@ -15,23 +18,23 @@
 
 Filename: rapidocr_web/static/js/jquery-3.0.0.min.js
 Comment: 
 
 Filename: rapidocr_web/templates/index.html
 Comment: 
 
-Filename: rapidocr_web-0.0.4.dist-info/METADATA
+Filename: rapidocr_web-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: rapidocr_web-0.0.4.dist-info/WHEEL
+Filename: rapidocr_web-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: rapidocr_web-0.0.4.dist-info/entry_points.txt
+Filename: rapidocr_web-0.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapidocr_web-0.0.4.dist-info/top_level.txt
+Filename: rapidocr_web-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: rapidocr_web-0.0.4.dist-info/RECORD
+Filename: rapidocr_web-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rapidocr_web/ocrweb.py

```diff
@@ -2,50 +2,43 @@
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
 import argparse
 from pathlib import Path
 from wsgiref.simple_server import make_server
 
 from flask import Flask, render_template, request
-try:
-    from .task import OCRWebUtils
-except:
-    from task import OCRWebUtils
+from rapidocr_web.task import OCRWebUtils
 
 root_dir = Path(__file__).resolve().parent
 
 app = Flask(__name__, template_folder='templates')
 app.config['MAX_CONTENT_LENGTH'] = 3 * 1024 * 1024
 processor = OCRWebUtils()
 
 
 @app.route('/')
 def index():
-    if not app.config['is_api']:
-        return render_template('index.html')
+    return render_template('index.html')
 
 
 @app.route('/ocr', methods=['POST'])
 def ocr():
     if request.method == 'POST':
         img_str = request.get_json().get('file', None)
-        ocr_res = processor(img_str, is_api=app.config['is_api'])
+        ocr_res = processor(img_str)
         return ocr_res
 
 
 def main():
     parser = argparse.ArgumentParser('rapidocr_web')
     parser.add_argument('-ip', '--ip', type=str, default='0.0.0.0',
                         help='IP Address')
     parser.add_argument('-p', '--port', type=int, default=9003,
                         help='IP port')
-    parser.add_argument('-api', '--is_api', action='store_true',
-                        default=False, help='Whether to use the api format.')
     args = parser.parse_args()
 
-    app.config['is_api'] = args.is_api
     server = make_server(args.ip, args.port, app)
     server.serve_forever()
 
 
 if __name__ == '__main__':
     main()
```

## rapidocr_web/task.py

```diff
@@ -1,55 +1,45 @@
 # -*- encoding: utf-8 -*-
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
 import base64
 import copy
 import json
+from collections import namedtuple
 from functools import reduce
 from typing import List, Tuple, Union
-from collections import namedtuple
 
 import cv2
 import numpy as np
-
 from rapidocr_onnxruntime import RapidOCR
 
 
 class OCRWebUtils():
     def __init__(self) -> None:
         self.ocr = RapidOCR()
         self.WebReturn = namedtuple(
             'WebReturn',
             ['image', 'total_elapse', 'elapse_part', 'rec_res'])
 
-    def __call__(self, img_content: str, is_api=False) -> namedtuple:
+    def __call__(self, img_content: str) -> namedtuple:
         if img_content is None:
             raise ValueError('img is None')
-
-        img = self.prepare_img(img_content, is_api)
+        img = self.prepare_img(img_content)
         ocr_res, elapse = self.ocr(img)
-
-        if is_api:
-            return self.get_api_result(ocr_res)
         return self.get_web_result(img, ocr_res, elapse)
 
-    def prepare_img(self, img_str: str, is_api: bool) -> np.ndarray:
-        if not is_api:
-            img_str = img_str.split(',')[1]
-
+    def prepare_img(self, img_str: str) -> np.ndarray:
+        img_str = img_str.split(',')[1]
         image = base64.b64decode(img_str + '=' * (-len(img_str) % 4))
         nparr = np.frombuffer(image, np.uint8)
         image = cv2.imdecode(nparr, cv2.IMREAD_COLOR)
         if image.ndim == 2:
             image = cv2.cvtColor(image, cv2.COLOR_GRAY2BGR)
         return image
 
-    def get_api_result(self, ocr_res: List) -> str:
-        return json.dumps(ocr_res, indent=2, ensure_ascii=False)
-
     def get_web_result(self,
                        img: np.ndarray,
                        ocr_res: List,
                        elapse: List) -> Tuple[Union[str, List, str, str]]:
         if ocr_res is None:
             total_elapse, elapse_part = 0, ''
             img_str = self.img_to_base64(img)
@@ -69,15 +59,15 @@
                                     total_elapse=f'{total_elapse:.4f}',
                                     elapse_part=elapse_part,
                                     rec_res=rec_res)
         return json.dumps(web_return._asdict())
 
     @staticmethod
     def img_to_base64(img) -> str:
-        img = cv2.imencode('.jpg', img)[1]
+        img = cv2.imencode('.png', img)[1]
         img_str = str(base64.b64encode(img))[2:-1]
         return img_str
 
     @staticmethod
     def draw_text_det_res(dt_boxes: np.ndarray,
                           raw_im: np.ndarray) -> np.ndarray:
         src_im = copy.deepcopy(raw_im)
```

## Comparing `rapidocr_web-0.0.4.dist-info/RECORD` & `rapidocr_web-0.1.0.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 rapidocr_web/__init__.py,sha256=m-UGKHJ-31qL7pBis4nfoFz5fzb-dXsiTLNqY-xpSoA,74
-rapidocr_web/ocrweb.py,sha256=KSESry7Itw1VAlp4IawpBKFZw-50M5zqS5lvnmczweE,1414
-rapidocr_web/task.py,sha256=007GYAXKbbCAL6M0165PyeBWG8U6CrL7Kh6OO4n3NO0,3206
+rapidocr_web/api.py,sha256=u6Vc7e93XQYyuPX6EOiafgfi0EY-mKf7tingL2CSmIw,1492
+rapidocr_web/ocrweb.py,sha256=fw9XEBoJZqUjbH19izaHJvXfQ-prwO_LoPjQuE3g8QY,1128
+rapidocr_web/task.py,sha256=l6PrccgTQDcvS8ZppZMfYuIPCYK-6ym_-02NWRm4Uak,2954
 rapidocr_web/static/css/favicon.ico,sha256=CBE1NF6iiIax8WqZVR-vPRaPTcmWjlTWsk1fzEbSd8c,16958
 rapidocr_web/static/css/main.css,sha256=2HcVvoa5oSQONnuC6IjjmBd127Jv9Y5EFJGy32nTEZk,2065
 rapidocr_web/static/js/jquery-3.0.0.min.js,sha256=JmvOoLtYsmqlsWxa7mDSLMwa6dZ9rrIdtrrVYRnDRH0,86341
 rapidocr_web/templates/index.html,sha256=xUe3Xce289Of4XTfeafPTX5JMRsOTdgv2Md5EQwxm48,8202
-rapidocr_web-0.0.4.dist-info/METADATA,sha256=9bExLp2ETbJ3wYXLtv-eM7ikyiHbEyuUCJ9rN_vbOL0,2644
-rapidocr_web-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rapidocr_web-0.0.4.dist-info/entry_points.txt,sha256=ivlPn9JP6ziblPQyG6N4H4cXfrJZ9FD5rvSYhnEc8cU,59
-rapidocr_web-0.0.4.dist-info/top_level.txt,sha256=dArjxF38AFvTF1Ae-mGaxBhwnETUJ4sLF_nQ93HC5A4,13
-rapidocr_web-0.0.4.dist-info/RECORD,,
+rapidocr_web-0.1.0.dist-info/METADATA,sha256=fiDI35xhftWUoJ2zgaGwuMZQNbfcuS2kN6tLnnO4Sv4,4576
+rapidocr_web-0.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rapidocr_web-0.1.0.dist-info/entry_points.txt,sha256=q3Vx7ES3NeGhonzyiGS8mVFDVVgK-J5M8bGSktcC92I,96
+rapidocr_web-0.1.0.dist-info/top_level.txt,sha256=dArjxF38AFvTF1Ae-mGaxBhwnETUJ4sLF_nQ93HC5A4,13
+rapidocr_web-0.1.0.dist-info/RECORD,,
```

