# Comparing `tmp/pywencai-0.5.3.tar.gz` & `tmp/pywencai-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywencai-0.5.3.tar", max compression
+gzip compressed data, was "pywencai-0.6.0.tar", max compression
```

## Comparing `pywencai-0.5.3.tar` & `pywencai-0.6.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1062 2023-04-12 16:09:07.777218 pywencai-0.5.3/LICENSE
--rw-r--r--   0        0        0     1814 2023-04-12 16:09:07.777218 pywencai-0.5.3/README.md
--rw-r--r--   0        0        0      516 2023-04-12 16:09:07.781218 pywencai-0.5.3/pyproject.toml
--rw-r--r--   0        0        0       23 2023-04-12 16:09:07.781218 pywencai-0.5.3/pywencai/__init__.py
--rw-r--r--   0        0        0    39677 2023-04-12 16:09:07.781218 pywencai-0.5.3/pywencai/hexin-v.js
--rw-r--r--   0        0        0     3768 2023-04-12 16:09:07.781218 pywencai-0.5.3/pywencai/wencai.py
--rw-r--r--   0        0        0     2349 1970-01-01 00:00:00.000000 pywencai-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-16 04:33:37.146306 pywencai-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2004 2023-04-16 04:33:37.146306 pywencai-0.6.0/README.md
+-rw-r--r--   0        0        0      530 2023-04-16 04:33:37.146306 pywencai-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-04-16 04:33:37.146306 pywencai-0.6.0/pywencai/__init__.py
+-rw-r--r--   0        0        0    39677 2023-04-16 04:33:37.146306 pywencai-0.6.0/pywencai/hexin-v.js
+-rw-r--r--   0        0        0     3768 2023-04-16 04:33:37.146306 pywencai-0.6.0/pywencai/wencai.py
+-rw-r--r--   0        0        0     2589 1970-01-01 00:00:00.000000 pywencai-0.6.0/PKG-INFO
```

### Comparing `pywencai-0.5.3/LICENSE` & `pywencai-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywencai-0.5.3/README.md` & `pywencai-0.6.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![PyPI version](https://badge.fury.io/py/pywencai.svg)](https://badge.fury.io/py/pywencai)
+[![Downloads](https://static.pepy.tech/badge/pywencai/month)](https://pepy.tech/project/pywencai)
 # pywencai
 
 获取同花顺问财数据
 
 ## 环境依赖
 
 由于程序中执行了js代码，请先保证已安装了[Node.js](https://nodejs.org/en/)
```

### Comparing `pywencai-0.5.3/pyproject.toml` & `pywencai-0.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "pywencai"
-version = "0.5.3"
+version = "0.6.0"
 description = ""
 authors = ["pluto <mayuanchi1029@gmail.com>"]
 readme = "README.md"
 
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://pypi.tuna.tsinghua.edu.cn/simple/"
 default = true
 
 [tool.poetry.dependencies]
-python = ">=3.8, <3.11"
+python = "^3.8"
 PyExecJS = "^1.5.1"
 requests = "*"
-pandas = "^1.5.0"
+pandas = {version = "^1.5.0 || ^2.0.0"}
 fake-useragent = "^1.1.1"
 
 [tool.poetry.group.dev.dependencies]
 notebook = "^6.4.12"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `pywencai-0.5.3/pywencai/hexin-v.js` & `pywencai-0.6.0/pywencai/hexin-v.js`

 * *Files identical despite different names*

### Comparing `pywencai-0.5.3/pywencai/wencai.py` & `pywencai-0.6.0/pywencai/wencai.py`

 * *Files identical despite different names*

### Comparing `pywencai-0.5.3/PKG-INFO` & `pywencai-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: pywencai
-Version: 0.5.3
+Version: 0.6.0
 Summary: 
 Author: pluto
 Author-email: mayuanchi1029@gmail.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyExecJS (>=1.5.1,<2.0.0)
 Requires-Dist: fake-useragent (>=1.1.1,<2.0.0)
-Requires-Dist: pandas (>=1.5.0,<2.0.0)
+Requires-Dist: pandas (>=1.5.0,<3.0.0)
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
+[![PyPI version](https://badge.fury.io/py/pywencai.svg)](https://badge.fury.io/py/pywencai)
+[![Downloads](https://static.pepy.tech/badge/pywencai/month)](https://pepy.tech/project/pywencai)
 # pywencai
 
 获取同花顺问财数据
 
 ## 环境依赖
 
 由于程序中执行了js代码，请先保证已安装了[Node.js](https://nodejs.org/en/)
```

