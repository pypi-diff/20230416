# Comparing `tmp/poshare-0.1.0.tar.gz` & `tmp/poshare-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poshare-0.1.0.tar", max compression
+gzip compressed data, was "poshare-0.2.0.tar", max compression
```

## Comparing `poshare-0.1.0.tar` & `poshare-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      706 2023-04-12 15:32:04.662601 poshare-0.1.0/README.md
--rw-r--r--   0        0        0       93 2023-04-12 15:32:04.662601 poshare-0.1.0/poshare/__init__.py
--rw-r--r--   0        0        0      722 2023-04-12 15:32:04.662601 poshare-0.1.0/poshare/guoren.py
--rw-r--r--   0        0        0      836 2023-04-12 15:32:04.662601 poshare-0.1.0/poshare/po.py
--rw-r--r--   0        0        0     2497 2023-04-12 15:32:04.666602 poshare-0.1.0/poshare/xueqiu.py
--rw-r--r--   0        0        0      494 2023-04-12 15:32:04.666602 poshare-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 poshare-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      755 2023-04-16 02:16:04.267695 poshare-0.2.0/README.md
+-rw-r--r--   0        0        0       93 2023-04-16 02:16:04.267695 poshare-0.2.0/poshare/__init__.py
+-rw-r--r--   0        0        0      722 2023-04-16 02:16:04.267695 poshare-0.2.0/poshare/guoren.py
+-rw-r--r--   0        0        0      836 2023-04-16 02:16:04.271694 poshare-0.2.0/poshare/po.py
+-rw-r--r--   0        0        0     2497 2023-04-16 02:16:04.271694 poshare-0.2.0/poshare/xueqiu.py
+-rw-r--r--   0        0        0      494 2023-04-16 02:16:04.271694 poshare-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1400 1970-01-01 00:00:00.000000 poshare-0.2.0/PKG-INFO
```

### Comparing `poshare-0.1.0/README.md` & `poshare-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # poshare
 
 poshare是一个获取公开投资组合的工具，po时`portfolio`的缩写，share代表分享。
 
+# 安装
+
+```
+pip install poshare --upgrade
+```
+
 ## 雪球
 
 ```python
 from poshare import Xueqiu
 
 Xueqiu.config({
     'cookie': 'your xueqiu cookie'
```

### Comparing `poshare-0.1.0/poshare/guoren.py` & `poshare-0.2.0/poshare/guoren.py`

 * *Files identical despite different names*

### Comparing `poshare-0.1.0/poshare/po.py` & `poshare-0.2.0/poshare/po.py`

 * *Files identical despite different names*

### Comparing `poshare-0.1.0/poshare/xueqiu.py` & `poshare-0.2.0/poshare/xueqiu.py`

 * *Files identical despite different names*

### Comparing `poshare-0.1.0/PKG-INFO` & `poshare-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 Metadata-Version: 2.1
 Name: poshare
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: pluto
 Author-email: mayuanchi1029@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Js2Py (>=0.74,<0.75)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: fake-useragent (>=1.1.3,<2.0.0)
-Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: pandas (>=1.5.0,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # poshare
 
 poshare是一个获取公开投资组合的工具，po时`portfolio`的缩写，share代表分享。
 
+# 安装
+
+```
+pip install poshare --upgrade
+```
+
 ## 雪球
 
 ```python
 from poshare import Xueqiu
 
 Xueqiu.config({
     'cookie': 'your xueqiu cookie'
```

