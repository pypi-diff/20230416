# Comparing `tmp/fenjing-0.1.0.tar.gz` & `tmp/fenjing-0.1.3.linux-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.1.0.tar", last modified: Sun Apr  2 06:15:05 2023, max compression
+gzip compressed data, was "fenjing-0.1.3.linux-x86_64.tar", last modified: Sun Apr 16 05:56:27 2023, max compression
```

## Comparing `fenjing-0.1.0.tar` & `fenjing-0.1.3.linux-x86_64.tar`

### file list

```diff
@@ -1,23 +1,38 @@
-drwxr-xr-x   0 cube      (1000) cube      (1000)        0 2023-04-02 06:15:05.063400 fenjing-0.1.0/
--rw-r--r--   0 cube      (1000) cube      (1000)    16725 2023-03-31 12:04:28.000000 fenjing-0.1.0/LICENSE
--rw-r--r--   0 cube      (1000) cube      (1000)     3874 2023-04-02 06:15:05.063400 fenjing-0.1.0/PKG-INFO
--rwxr-x---   0 cube      (1000) cube      (1000)     3436 2023-04-02 06:13:58.000000 fenjing-0.1.0/README.md
-drwxr-xr-x   0 cube      (1000) cube      (1000)        0 2023-04-02 06:15:05.062400 fenjing-0.1.0/fenjing/
--rwxr-x---   0 cube      (1000) cube      (1000)      204 2023-04-02 05:40:13.000000 fenjing-0.1.0/fenjing/__init__.py
--rw-r--r--   0 cube      (1000) cube      (1000)       60 2023-03-31 08:38:41.000000 fenjing-0.1.0/fenjing/__main__.py
--rw-r--r--   0 cube      (1000) cube      (1000)     2482 2023-04-02 06:09:14.000000 fenjing-0.1.0/fenjing/cli.py
--rwxr-x---   0 cube      (1000) cube      (1000)      637 2023-03-31 09:59:29.000000 fenjing-0.1.0/fenjing/example.py
--rwxr-x---   0 cube      (1000) cube      (1000)       36 2023-03-31 08:02:21.000000 fenjing-0.1.0/fenjing/exceptions.py
--rwxr-x---   0 cube      (1000) cube      (1000)     2759 2023-03-26 05:40:10.000000 fenjing-0.1.0/fenjing/int_vars.py
--rwxr-x---   0 cube      (1000) cube      (1000)    37000 2023-03-31 08:46:50.000000 fenjing-0.1.0/fenjing/pattern.py
--rw-r--r--   0 cube      (1000) cube      (1000)      873 2023-04-02 06:07:23.000000 fenjing-0.1.0/fenjing/scan_url.py
--rwxr-x---   0 cube      (1000) cube      (1000)     1719 2023-04-02 05:49:41.000000 fenjing-0.1.0/fenjing/shell_cmd.py
--rw-r--r--   0 cube      (1000) cube      (1000)     3876 2023-04-02 05:49:57.000000 fenjing-0.1.0/fenjing/test_form.py
-drwxr-xr-x   0 cube      (1000) cube      (1000)        0 2023-04-02 06:15:05.063400 fenjing-0.1.0/fenjing.egg-info/
--rw-r--r--   0 cube      (1000) cube      (1000)     3874 2023-04-02 06:15:05.000000 fenjing-0.1.0/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 cube      (1000) cube      (1000)      377 2023-04-02 06:15:05.000000 fenjing-0.1.0/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 cube      (1000) cube      (1000)        1 2023-04-02 06:15:05.000000 fenjing-0.1.0/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 cube      (1000) cube      (1000)       30 2023-04-02 06:15:05.000000 fenjing-0.1.0/fenjing.egg-info/requires.txt
--rw-r--r--   0 cube      (1000) cube      (1000)        8 2023-04-02 06:15:05.000000 fenjing-0.1.0/fenjing.egg-info/top_level.txt
--rw-r--r--   0 cube      (1000) cube      (1000)       38 2023-04-02 06:15:05.063400 fenjing-0.1.0/setup.cfg
--rw-r--r--   0 cube      (1000) cube      (1000)      860 2023-03-31 12:05:47.000000 fenjing-0.1.0/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-16 05:56:27.254000 ./
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-16 05:56:27.254000 ./usr/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-16 05:56:27.254000 ./usr/local/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-16 05:56:27.255000 ./usr/local/lib/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-16 05:56:27.255000 ./usr/local/lib/python3.11/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-16 05:56:27.416000 ./usr/local/lib/python3.11/site-packages/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-16 05:56:27.258000 ./usr/local/lib/python3.11/site-packages/fenjing/
+-rw-r--r--   0 user      (1000) user      (1000)      198 2023-04-16 05:52:30.000000 ./usr/local/lib/python3.11/site-packages/fenjing/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)       60 2023-03-31 08:38:41.000000 ./usr/local/lib/python3.11/site-packages/fenjing/__main__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-16 05:56:27.318000 ./usr/local/lib/python3.11/site-packages/fenjing/__pycache__/
+-rw-r--r--   0 user      (1000) user      (1000)      528 2023-04-16 05:56:27.266000 ./usr/local/lib/python3.11/site-packages/fenjing/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 user      (1000) user      (1000)      298 2023-04-16 05:56:27.258000 ./usr/local/lib/python3.11/site-packages/fenjing/__pycache__/__main__.cpython-311.pyc
+-rw-r--r--   0 user      (1000) user      (1000)     5089 2023-04-16 05:56:27.259000 ./usr/local/lib/python3.11/site-packages/fenjing/__pycache__/cli.cpython-311.pyc
+-rw-r--r--   0 user      (1000) user      (1000)     1020 2023-04-16 05:56:27.273000 ./usr/local/lib/python3.11/site-packages/fenjing/__pycache__/example.cpython-311.pyc
+-rw-r--r--   0 user      (1000) user      (1000)      404 2023-04-16 05:56:27.267000 ./usr/local/lib/python3.11/site-packages/fenjing/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0 user      (1000) user      (1000)     4073 2023-04-16 05:56:27.266000 ./usr/local/lib/python3.11/site-packages/fenjing/__pycache__/form.cpython-311.pyc
+-rw-r--r--   0 user      (1000) user      (1000)     2878 2023-04-16 05:56:27.267000 ./usr/local/lib/python3.11/site-packages/fenjing/__pycache__/int_vars.cpython-311.pyc
+-rw-r--r--   0 user      (1000) user      (1000)    86398 2023-04-16 05:56:27.315000 ./usr/local/lib/python3.11/site-packages/fenjing/__pycache__/pattern.cpython-311.pyc
+-rw-r--r--   0 user      (1000) user      (1000)     1972 2023-04-16 05:56:27.273000 ./usr/local/lib/python3.11/site-packages/fenjing/__pycache__/request.cpython-311.pyc
+-rw-r--r--   0 user      (1000) user      (1000)     1822 2023-04-16 05:56:27.271000 ./usr/local/lib/python3.11/site-packages/fenjing/__pycache__/scan_url.cpython-311.pyc
+-rw-r--r--   0 user      (1000) user      (1000)     2705 2023-04-16 05:56:27.318000 ./usr/local/lib/python3.11/site-packages/fenjing/__pycache__/shell_cmd.cpython-311.pyc
+-rw-r--r--   0 user      (1000) user      (1000)     7289 2023-04-16 05:56:27.272000 ./usr/local/lib/python3.11/site-packages/fenjing/__pycache__/test_form.cpython-311.pyc
+-rw-r--r--   0 user      (1000) user      (1000)     2476 2023-04-16 05:52:51.000000 ./usr/local/lib/python3.11/site-packages/fenjing/cli.py
+-rw-r--r--   0 user      (1000) user      (1000)      637 2023-04-02 06:25:33.000000 ./usr/local/lib/python3.11/site-packages/fenjing/example.py
+-rw-r--r--   0 user      (1000) user      (1000)       36 2023-03-31 08:02:21.000000 ./usr/local/lib/python3.11/site-packages/fenjing/exceptions.py
+-rw-r--r--   0 user      (1000) user      (1000)     2043 2023-04-02 06:07:31.000000 ./usr/local/lib/python3.11/site-packages/fenjing/form.py
+-rw-r--r--   0 user      (1000) user      (1000)     2759 2023-03-26 05:40:10.000000 ./usr/local/lib/python3.11/site-packages/fenjing/int_vars.py
+-rw-r--r--   0 user      (1000) user      (1000)    37000 2023-03-31 08:46:50.000000 ./usr/local/lib/python3.11/site-packages/fenjing/pattern.py
+-rw-r--r--   0 user      (1000) user      (1000)      853 2023-04-02 05:33:58.000000 ./usr/local/lib/python3.11/site-packages/fenjing/request.py
+-rw-r--r--   0 user      (1000) user      (1000)      861 2023-04-16 05:52:32.000000 ./usr/local/lib/python3.11/site-packages/fenjing/scan_url.py
+-rw-r--r--   0 user      (1000) user      (1000)     1719 2023-04-02 05:49:41.000000 ./usr/local/lib/python3.11/site-packages/fenjing/shell_cmd.py
+-rw-r--r--   0 user      (1000) user      (1000)     3864 2023-04-16 05:52:36.000000 ./usr/local/lib/python3.11/site-packages/fenjing/test_form.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-16 05:56:27.421000 ./usr/local/lib/python3.11/site-packages/fenjing-0.1.3-py3.11.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3991 2023-04-16 05:56:26.290000 ./usr/local/lib/python3.11/site-packages/fenjing-0.1.3-py3.11.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      412 2023-04-16 05:56:26.881000 ./usr/local/lib/python3.11/site-packages/fenjing-0.1.3-py3.11.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-16 05:56:26.371000 ./usr/local/lib/python3.11/site-packages/fenjing-0.1.3-py3.11.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       30 2023-04-16 05:56:26.667000 ./usr/local/lib/python3.11/site-packages/fenjing-0.1.3-py3.11.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        8 2023-04-16 05:56:26.728000 ./usr/local/lib/python3.11/site-packages/fenjing-0.1.3-py3.11.egg-info/top_level.txt
```

### Comparing `fenjing-0.1.0/PKG-INFO` & `./usr/local/lib/python3.11/site-packages/fenjing-0.1.3-py3.11.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.1.0
+Version: 0.1.3
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 
 焚靖是一个针对Jinja2 SSTI的命令行脚本，具有强大的自动绕过WAF功能
 
 ## 演示
 
 ![CTFShow web365](assets/demo.webp)
 
-`python -m fenjing scan --url 'http://xxx/'`
+`python -m fenjing crack --method GET --inputs name --url 'http://xxx/'`
 
 ## 快速上手
 
 在以下方法中选择一种
 
 ### 使用pip安装运行
 
@@ -34,15 +34,15 @@
 python -m fenjing scan --url 'http://xxx/'
 ```
 
 ### 下载并运行docker镜像
 
 ```shell
 docker pull marven11/fenjing
-docker run marven11/fenjing scan --url 'http://xxx/'
+docker run --net host -it marven11/fenjing scan --url 'http://xxx/'
 ```
 
 ### 手动安装
 
 ```shell
 git clone https://github.com/Marven11/Fenjing
 cd Fenjing
@@ -119,14 +119,17 @@
     - 其中的字符串也支持上面的任意字符串绕过
 
 
 ## 详细使用
 
 ### 作为命令行脚本使用
 
+- scan: 扫描整个网站
+- crack: 对某个特定的表单进行攻击
+
 ```
 Usage: python -m fenjing scan [OPTIONS]
 
 Options:
   --url TEXT       需要扫描的URL
   --exec-cmd TEXT  成功后执行的shell指令，不填则进入交互模式
   --help           Show this message and exit.
```

### Comparing `fenjing-0.1.0/fenjing/cli.py` & `./usr/local/lib/python3.11/site-packages/fenjing/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from urllib.parse import urlparse
 from traceback import print_exc
 
 from .test_form import test_form, Form, submit_form_input
-from .utils.request import common_request
+from .request import common_request
 from .scan_url import yield_form
 import click
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger("cli")
```

### Comparing `fenjing-0.1.0/fenjing/example.py` & `./usr/local/lib/python3.11/site-packages/fenjing/example.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.0/fenjing/int_vars.py` & `./usr/local/lib/python3.11/site-packages/fenjing/int_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.0/fenjing/pattern.py` & `./usr/local/lib/python3.11/site-packages/fenjing/pattern.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.0/fenjing/scan_url.py` & `./usr/local/lib/python3.11/site-packages/fenjing/scan_url.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 
-from .utils.request import common_request
-from .utils.form import parse_forms
+from .request import common_request
+from .form import parse_forms
 
 from bs4 import BeautifulSoup
 
 def parse_urls(html):
     if isinstance(html, str):
         bs = BeautifulSoup(html, "html.parser")
     elif isinstance(html, BeautifulSoup):
```

### Comparing `fenjing-0.1.0/fenjing/shell_cmd.py` & `./usr/local/lib/python3.11/site-packages/fenjing/shell_cmd.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.0/fenjing/test_form.py` & `./usr/local/lib/python3.11/site-packages/fenjing/test_form.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 from functools import wraps, partial, lru_cache
 from collections import Counter
 from typing import Iterable
 from itertools import groupby
 
 from .shell_cmd import exec_cmd_payload
-from .utils.request import common_request
-from .utils.form import Form, fill_form, random_fill
+from .request import common_request
+from .form import Form, fill_form, random_fill
 
 
 logger = logging.getLogger("test_form")
 
 
 def get_possible_input(url: str, form):
     """
```

