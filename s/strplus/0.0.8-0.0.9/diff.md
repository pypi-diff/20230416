# Comparing `tmp/strplus-0.0.8.tar.gz` & `tmp/strplus-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strplus-0.0.8.tar", max compression
+gzip compressed data, was "strplus-0.0.9.tar", max compression
```

## Comparing `strplus-0.0.8.tar` & `strplus-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-04-14 07:41:30.953611 strplus-0.0.8/LICENSE
--rw-r--r--   0        0        0     2343 2023-04-16 14:30:37.167669 strplus-0.0.8/README.md
--rw-r--r--   0        0        0      847 2023-04-16 10:54:10.661534 strplus-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      161 2023-04-16 09:50:28.142670 strplus-0.0.8/strplus/__init__.py
--rw-r--r--   0        0        0     4243 2023-04-16 11:19:57.781075 strplus-0.0.8/strplus/cases.py
--rw-r--r--   0        0        0      542 2023-04-16 09:50:28.152670 strplus-0.0.8/strplus/functions.py
--rw-r--r--   0        0        0     3868 2023-04-16 11:19:57.781075 strplus-0.0.8/strplus/strplus.py
--rw-r--r--   0        0        0     2982 1970-01-01 00:00:00.000000 strplus-0.0.8/setup.py
--rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 strplus-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-14 07:41:30.953611 strplus-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2353 2023-04-16 14:38:50.577526 strplus-0.0.9/README.md
+-rw-r--r--   0        0        0      847 2023-04-16 14:39:44.897503 strplus-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      161 2023-04-16 09:50:28.142670 strplus-0.0.9/strplus/__init__.py
+-rw-r--r--   0        0        0     4243 2023-04-16 11:19:57.781075 strplus-0.0.9/strplus/cases.py
+-rw-r--r--   0        0        0      542 2023-04-16 09:50:28.152670 strplus-0.0.9/strplus/functions.py
+-rw-r--r--   0        0        0     3868 2023-04-16 11:19:57.781075 strplus-0.0.9/strplus/strplus.py
+-rw-r--r--   0        0        0     2994 1970-01-01 00:00:00.000000 strplus-0.0.9/setup.py
+-rw-r--r--   0        0        0     2931 1970-01-01 00:00:00.000000 strplus-0.0.9/PKG-INFO
```

### Comparing `strplus-0.0.8/LICENSE` & `strplus-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `strplus-0.0.8/README.md` & `strplus-0.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 Python extra functions for strings ❤️
 </h1>
 
 <br>
 <br>
 <br>
 <br>
+<br>
+<br>
 
 [Documentation](https://wiseupdata.github.io/strplus/index.html)  🚀
 
 <br>
 
 ## Features ✨️
```

#### html2text {}

```diff
@@ -5,14 +5,16 @@
 
 [img]
 ****** Python extra functions for strings â¤ï¸ ******
 
 
 
 
+
+
 [Documentation](https://wiseupdata.github.io/strplus/index.html) ð
 ## Features â¨ï¸ - Wrapper Class - +234 test in 32 Tests files! - Simple use!
 
 ### Simple use example ð ``` >>> my_string = Str('this_is-an_example') >>>
 my_string.camel() 'thisIsAnExample' ```
 > Check the documentations for more examples: [Documentation](https://
 wiseupdata.github.io/strplus/index.html)!
```

### Comparing `strplus-0.0.8/pyproject.toml` & `strplus-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strplus"
-version = "0.0.8"
+version = "0.0.9"
 authors = ["Silvio Liborio <silvio.liborio@wiseupdata.com>"]
 readme = "README.md"
 
 description = "Python extra functions for strings"
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `strplus-0.0.8/strplus/cases.py` & `strplus-0.0.9/strplus/cases.py`

 * *Files identical despite different names*

### Comparing `strplus-0.0.8/strplus/functions.py` & `strplus-0.0.9/strplus/functions.py`

 * *Files identical despite different names*

### Comparing `strplus-0.0.8/strplus/strplus.py` & `strplus-0.0.9/strplus/strplus.py`

 * *Files identical despite different names*

### Comparing `strplus-0.0.8/setup.py` & `strplus-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['strplus']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'strplus',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Python extra functions for strings',
-    'long_description': '<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="Wise Up Data\'s Instagram" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/instagram.png" />   \n</a> \n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s Discord" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/discord.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data | Twitter" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/twitter.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s LinkedIN" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/linkedin.png" />\n</a>\n\n![visitors](https://visitor-badge.glitch.me/badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n![license](https://img.shields.io/github/license/wiseupdata/strplus)\n\n---\n\n<br>\n<br>\n\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/python.png" width="300" />\n</a>\n\n<h1>\nPython extra functions for strings ❤️\n</h1>\n\n<br>\n<br>\n<br>\n<br>\n\n[Documentation](https://wiseupdata.github.io/strplus/index.html)  🚀\n\n<br>\n\n## Features ✨️\n\n- Wrapper Class\n- +234 test in 32 Tests files!\n- Simple use! \n\n<br>\n\n### Simple use example 😍\n```\n>>> my_string = Str(\'this_is-an_example\')\n>>> my_string.camel()\n\'thisIsAnExample\'\n```\n<br>\n\n> Check the documentations for more examples: [Documentation](https://wiseupdata.github.io/strplus/index.html)! \n\n<br>\n<br>\n\n# References 🌍 🗄️\n\n1. [Wise Up Data](https://github.com/wiseupdata)\n2. [Emojis](https://github.com/wiseupdata/emojis)\n3. [Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)\n\n<br>\n<br>\n---\n\n#### Maintainer 🤗 👨\u200d💻\n\nSivio Liborio\n\n📧 silvio.liborio@wiseupdata.com\n\n<a href="https://www.linkedin.com/in/silvio-de-melo-liborio">silvio-de-melo-liborio <img align="left" alt="LinkedIN" width="18px" src="https://raw.githubusercontent.com/wiseupdata/wsl-latest/main/assets/linkedin.svg" />\n</a>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n\n> WiseUpData\n',
+    'long_description': '<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="Wise Up Data\'s Instagram" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/instagram.png" />   \n</a> \n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s Discord" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/discord.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data | Twitter" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/twitter.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s LinkedIN" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/linkedin.png" />\n</a>\n\n![visitors](https://visitor-badge.glitch.me/badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n![license](https://img.shields.io/github/license/wiseupdata/strplus)\n\n---\n\n<br>\n<br>\n\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/python.png" width="300" />\n</a>\n\n<h1>\nPython extra functions for strings ❤️\n</h1>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n\n[Documentation](https://wiseupdata.github.io/strplus/index.html)  🚀\n\n<br>\n\n## Features ✨️\n\n- Wrapper Class\n- +234 test in 32 Tests files!\n- Simple use! \n\n<br>\n\n### Simple use example 😍\n```\n>>> my_string = Str(\'this_is-an_example\')\n>>> my_string.camel()\n\'thisIsAnExample\'\n```\n<br>\n\n> Check the documentations for more examples: [Documentation](https://wiseupdata.github.io/strplus/index.html)! \n\n<br>\n<br>\n\n# References 🌍 🗄️\n\n1. [Wise Up Data](https://github.com/wiseupdata)\n2. [Emojis](https://github.com/wiseupdata/emojis)\n3. [Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)\n\n<br>\n<br>\n---\n\n#### Maintainer 🤗 👨\u200d💻\n\nSivio Liborio\n\n📧 silvio.liborio@wiseupdata.com\n\n<a href="https://www.linkedin.com/in/silvio-de-melo-liborio">silvio-de-melo-liborio <img align="left" alt="LinkedIN" width="18px" src="https://raw.githubusercontent.com/wiseupdata/wsl-latest/main/assets/linkedin.svg" />\n</a>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n\n> WiseUpData\n',
     'author': 'Silvio Liborio',
     'author_email': 'silvio.liborio@wiseupdata.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,22 +1,24 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['strplus']
 package_data = \ {'': ['*']} setup_kwargs = { 'name': 'strplus', 'version':
-'0.0.8', 'description': 'Python extra functions for strings',
+'0.0.9', 'description': 'Python extra functions for strings',
 'long_description': '\n_[Wise_Up_Data\'s_Instagram]_\n \n\n_[wise_Up_Data\'s
 Discord]\n\n\n_[wise_Up_Data_|_Twitter]\n\n\n_[wise_Up_Data\'s_LinkedIN]\n\n\n!
 [visitors](https://visitor-badge.glitch.me/
 badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n!
 [license](https://img.shields.io/github/license/wiseupdata/strplus)\n\n---\n\n
 \n
 \n\n\n[img]\n\n\n
 ****** \nPython extra functions for strings â¤ï¸\n ******
 \n\n
 \n
 \n
 \n
+\n
+\n
 \n\n[Documentation](https://wiseupdata.github.io/strplus/index.html) ð\n\n
 \n\n## Features â¨ï¸\n\n- Wrapper Class\n- +234 test in 32 Tests files!\n-
 Simple use! \n\n
 \n\n### Simple use example ð\n```\n>>> my_string = Str(\'this_is-
 an_example\')\n>>> my_string.camel()\n\'thisIsAnExample\'\n```\n
 \n\n> Check the documentations for more examples: [Documentation](https://
 wiseupdata.github.io/strplus/index.html)! \n\n
```

### Comparing `strplus-0.0.8/PKG-INFO` & `strplus-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strplus
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python extra functions for strings
 Author: Silvio Liborio
 Author-email: silvio.liborio@wiseupdata.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -43,14 +43,16 @@
 Python extra functions for strings ❤️
 </h1>
 
 <br>
 <br>
 <br>
 <br>
+<br>
+<br>
 
 [Documentation](https://wiseupdata.github.io/strplus/index.html)  🚀
 
 <br>
 
 ## Features ✨️
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: strplus Version: 0.0.8 Summary: Python extra
+Metadata-Version: 2.1 Name: strplus Version: 0.0.9 Summary: Python extra
 functions for strings Author: Silvio Liborio Author-email:
 silvio.liborio@wiseupdata.com Requires-Python: >=3.9,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown [Wise_Up_Data's
@@ -13,14 +13,16 @@
 
 [img]
 ****** Python extra functions for strings â¤ï¸ ******
 
 
 
 
+
+
 [Documentation](https://wiseupdata.github.io/strplus/index.html) ð
 ## Features â¨ï¸ - Wrapper Class - +234 test in 32 Tests files! - Simple use!
 
 ### Simple use example ð ``` >>> my_string = Str('this_is-an_example') >>>
 my_string.camel() 'thisIsAnExample' ```
 > Check the documentations for more examples: [Documentation](https://
 wiseupdata.github.io/strplus/index.html)!
```

