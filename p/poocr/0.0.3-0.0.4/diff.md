# Comparing `tmp/poocr-0.0.3.tar.gz` & `tmp/poocr-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poocr-0.0.3.tar", last modified: Sun Apr  9 13:57:08 2023, max compression
+gzip compressed data, was "poocr-0.0.4.tar", last modified: Sun Apr 16 10:13:24 2023, max compression
```

## Comparing `poocr-0.0.3.tar` & `poocr-0.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 13:57:08.378192 poocr-0.0.3/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poocr-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     4588 2023-04-09 13:57:08.378192 poocr-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4067 2023-04-02 05:09:27.000000 poocr-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 13:57:08.241899 poocr-0.0.3/poocr/
--rw-rw-rw-   0        0        0      523 2023-03-25 11:20:01.000000 poocr-0.0.3/poocr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 13:57:08.291442 poocr-0.0.3/poocr/api/
--rw-rw-rw-   0        0        0      265 2023-03-25 11:08:27.000000 poocr-0.0.3/poocr/api/__init__.py
--rw-rw-rw-   0        0        0    20975 2023-01-30 12:39:04.000000 poocr-0.0.3/poocr/api/ocr.py
--rw-rw-rw-   0        0        0     9854 2023-04-09 13:56:17.000000 poocr-0.0.3/poocr/api/ocr2excel.py
-drwxrwxrwx   0        0        0        0 2023-04-09 13:57:08.300441 poocr-0.0.3/poocr/core/
--rw-rw-rw-   0        0        0     4071 2023-01-30 12:39:04.000000 poocr-0.0.3/poocr/core/OCR.py
--rw-rw-rw-   0        0        0      223 2023-01-22 06:56:13.000000 poocr-0.0.3/poocr/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 13:57:08.354573 poocr-0.0.3/poocr/lib/
--rw-rw-rw-   0        0        0     1017 2023-01-28 13:49:56.000000 poocr-0.0.3/poocr/lib/CommonUtils.py
--rw-rw-rw-   0        0        0     1132 2023-01-30 12:39:04.000000 poocr-0.0.3/poocr/lib/Config.py
--rw-rw-rw-   0        0        0      852 2023-01-30 12:39:04.000000 poocr-0.0.3/poocr/lib/Const.py
--rw-rw-rw-   0        0        0        0 2023-01-22 10:20:33.000000 poocr-0.0.3/poocr/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 13:57:08.282447 poocr-0.0.3/poocr.egg-info/
--rw-rw-rw-   0        0        0     4588 2023-04-09 13:57:08.000000 poocr-0.0.3/poocr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2023-04-09 13:57:08.000000 poocr-0.0.3/poocr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 13:57:08.000000 poocr-0.0.3/poocr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-09 13:57:08.000000 poocr-0.0.3/poocr.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       40 2023-04-09 13:57:08.000000 poocr-0.0.3/poocr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-09 13:57:08.000000 poocr-0.0.3/poocr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      732 2023-04-09 13:57:08.381190 poocr-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poocr-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 13:57:08.376191 poocr-0.0.3/tests/
--rw-rw-rw-   0        0        0      181 2023-01-30 12:39:04.000000 poocr-0.0.3/tests/__init__.py
--rw-rw-rw-   0        0        0      704 2023-04-09 12:49:12.000000 poocr-0.0.3/tests/test_tencent.py
+drwxrwxrwx   0        0        0        0 2023-04-16 10:13:24.294331 poocr-0.0.4/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poocr-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     4588 2023-04-16 10:13:24.294331 poocr-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4067 2023-04-02 05:09:27.000000 poocr-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 10:13:24.231025 poocr-0.0.4/poocr/
+-rw-rw-rw-   0        0        0      523 2023-03-25 11:20:01.000000 poocr-0.0.4/poocr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 10:13:24.274127 poocr-0.0.4/poocr/api/
+-rw-rw-rw-   0        0        0      265 2023-03-25 11:08:27.000000 poocr-0.0.4/poocr/api/__init__.py
+-rw-rw-rw-   0        0        0    20975 2023-01-30 12:39:04.000000 poocr-0.0.4/poocr/api/ocr.py
+-rw-rw-rw-   0        0        0    10432 2023-04-16 10:12:06.000000 poocr-0.0.4/poocr/api/ocr2excel.py
+drwxrwxrwx   0        0        0        0 2023-04-16 10:13:24.278120 poocr-0.0.4/poocr/core/
+-rw-rw-rw-   0        0        0     4071 2023-01-30 12:39:04.000000 poocr-0.0.4/poocr/core/OCR.py
+-rw-rw-rw-   0        0        0      223 2023-01-22 06:56:13.000000 poocr-0.0.4/poocr/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 10:13:24.287268 poocr-0.0.4/poocr/lib/
+-rw-rw-rw-   0        0        0     1017 2023-01-28 13:49:56.000000 poocr-0.0.4/poocr/lib/CommonUtils.py
+-rw-rw-rw-   0        0        0     1132 2023-01-30 12:39:04.000000 poocr-0.0.4/poocr/lib/Config.py
+-rw-rw-rw-   0        0        0      852 2023-01-30 12:39:04.000000 poocr-0.0.4/poocr/lib/Const.py
+-rw-rw-rw-   0        0        0        0 2023-01-22 10:20:33.000000 poocr-0.0.4/poocr/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 10:13:24.268112 poocr-0.0.4/poocr.egg-info/
+-rw-rw-rw-   0        0        0     4588 2023-04-16 10:13:24.000000 poocr-0.0.4/poocr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2023-04-16 10:13:24.000000 poocr-0.0.4/poocr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 10:13:24.000000 poocr-0.0.4/poocr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-16 09:44:14.000000 poocr-0.0.4/poocr.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       40 2023-04-16 10:13:24.000000 poocr-0.0.4/poocr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-16 10:13:24.000000 poocr-0.0.4/poocr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      732 2023-04-16 10:13:24.298346 poocr-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poocr-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 10:13:24.292810 poocr-0.0.4/tests/
+-rw-rw-rw-   0        0        0      181 2023-01-30 12:39:04.000000 poocr-0.0.4/tests/__init__.py
+-rw-rw-rw-   0        0        0      823 2023-04-16 09:36:45.000000 poocr-0.0.4/tests/test_tencent.py
```

### Comparing `poocr-0.0.3/LICENSE` & `poocr-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `poocr-0.0.3/PKG-INFO` & `poocr-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poocr
-Version: 0.0.3
+Version: 0.0.4
 Summary: pip install poocr
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poocr/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poocr/blob/main/README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poocr Version: 0.0.3 Summary: pip install poocr
+Metadata-Version: 2.1 Name: poocr Version: 0.0.4 Summary: pip install poocr
 Home-page: https://www.python-office.com/ Author: CoderWanFeng Author-email:
 1957875073@qq.com License: MIT Project-URL: Bug Tracker, https://github.com/
 CoderWanFeng/poocr/issues Project-URL: Documentation, https://github.com/
 CoderWanFeng/poocr/blob/main/README.md Project-URL: Source Code, https://
 github.com/CoderWanFeng/poocr Platform: any Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE
 [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/ads%2F1040x100-
```

### Comparing `poocr-0.0.3/README.md` & `poocr-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `poocr-0.0.3/poocr/__init__.py` & `poocr-0.0.4/poocr/__init__.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.3/poocr/api/ocr.py` & `poocr-0.0.4/poocr/api/ocr.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.3/poocr/api/ocr2excel.py` & `poocr-0.0.4/poocr/api/ocr2excel.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,20 @@
 @Date    ：2023/3/25 18:53 
 @Description     ：
 '''
 import json
 from pathlib import Path
 
 import pandas as pd
-from poocr.api.ocr import VatInvoiceOCR
+from pofile import get_files
 from poprogress import simple_progress
 
+import poocr
+from poocr.api.ocr import VatInvoiceOCR
+
 
 def VatInvoiceOCR2Excel(intput_path, output_excel=None, img_url=None, configPath=None):
     abs_intput_path = Path(intput_path).absolute()
     if output_excel.endswith('.xlsx') or output_excel.endswith('xls'):
         abs_output_excel = Path(output_excel).absolute()
     elif output_excel:  # 指定了，但不是xlsx或者xls结束
         print(f'输出结果名：output_excel参数，必须以xls或者xlsx结尾，您的输入:{output_excel}有误，请修改后重新运行')
@@ -37,7 +40,18 @@
         res_df.append(pd.DataFrame(dict_pandas, index=[0]))
     res_excel = res_df[0]
     for index, line_df in enumerate(res_df):
         if index == 0:
             continue
         res_excel = res_excel._append(line_df)
     pd.DataFrame(res_excel).to_excel(str(abs_output_excel))
+
+
+def TrainTicketOCR2Excel(input_path: str, output_excel: str = r'./TrainTicketOCR2Excel.xlsx', img_url: str = None,
+                         configPath: str = None) -> None:
+    ticket_list = []
+    ticket_files = get_files(input_path)
+    for ticket in simple_progress(ticket_files):
+        ticket_info = poocr.ocr.TrainTicketOCR(img_path=ticket, img_url=img_url, configPath=configPath)
+        ticket_list.append(ticket_info)
+    ticket_df = pd.DataFrame(ticket_list)
+    ticket_df.to_excel(output_excel, index=None)
```

### Comparing `poocr-0.0.3/poocr/core/OCR.py` & `poocr-0.0.4/poocr/core/OCR.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.3/poocr/lib/CommonUtils.py` & `poocr-0.0.4/poocr/lib/CommonUtils.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.3/poocr/lib/Config.py` & `poocr-0.0.4/poocr/lib/Config.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.3/poocr/lib/Const.py` & `poocr-0.0.4/poocr/lib/Const.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.3/poocr.egg-info/PKG-INFO` & `poocr-0.0.4/poocr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poocr
-Version: 0.0.3
+Version: 0.0.4
 Summary: pip install poocr
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poocr/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poocr/blob/main/README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poocr Version: 0.0.3 Summary: pip install poocr
+Metadata-Version: 2.1 Name: poocr Version: 0.0.4 Summary: pip install poocr
 Home-page: https://www.python-office.com/ Author: CoderWanFeng Author-email:
 1957875073@qq.com License: MIT Project-URL: Bug Tracker, https://github.com/
 CoderWanFeng/poocr/issues Project-URL: Documentation, https://github.com/
 CoderWanFeng/poocr/blob/main/README.md Project-URL: Source Code, https://
 github.com/CoderWanFeng/poocr Platform: any Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE
 [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/ads%2F1040x100-
```

### Comparing `poocr-0.0.3/setup.cfg` & `poocr-0.0.4/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f6f 6372 0d0a 7665 7273 696f   = poocr..versio
-00000020: 6e20 3d20 302e 302e 330d 0a64 6573 6372  n = 0.0.3..descr
+00000020: 6e20 3d20 302e 302e 340d 0a64 6573 6372  n = 0.0.4..descr
 00000030: 6970 7469 6f6e 203d 2070 6970 2069 6e73  iption = pip ins
 00000040: 7461 6c6c 2070 6f6f 6372 0d0a 6c6f 6e67  tall poocr..long
 00000050: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000060: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 00000090: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
```

### Comparing `poocr-0.0.3/tests/test_tencent.py` & `poocr-0.0.4/tests/test_tencent.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,10 +12,12 @@
 
     def test_idcard_ocr(self):
         res = IDCardOCR(
             img_path=r'C:\Users\Lenovo\Desktop\temp\正面.jpg')
         print(res)
 
     def test_VatInvoiceOCR2Excel(self):
-        VatInvoiceOCR2Excel(intput_path=r'C:\Users\Lenovo\Desktop\temp\v1-微信图片_20230409204718.png',
+        VatInvoiceOCR2Excel(intput_path=r'C:\Users\Lenovo\Desktop\temp\Snipaste_2023-04-09_22-23-48.png',
                             output_excel=r'./VatInvoiceOCR2Excel.xlsx',
                             configPath=r'./poocr-config.toml')
+    def test_TrainTicketOCR2Excel(self):
+        TrainTicketOCR2Excel(input_path='', output_excel='',configPath='fdasf')
```

