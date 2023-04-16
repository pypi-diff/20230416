# Comparing `tmp/strplus-0.0.7.tar.gz` & `tmp/strplus-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strplus-0.0.7.tar", max compression
+gzip compressed data, was "strplus-0.0.8.tar", max compression
```

## Comparing `strplus-0.0.7.tar` & `strplus-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-04-14 07:41:30.953611 strplus-0.0.7/LICENSE
--rw-r--r--   0        0        0     2348 2023-04-14 19:36:57.172317 strplus-0.0.7/README.md
--rw-r--r--   0        0        0      672 2023-04-14 23:02:53.571036 strplus-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      160 2023-04-14 07:41:30.953611 strplus-0.0.7/strplus/__init__.py
--rw-r--r--   0        0        0     2749 2023-04-14 19:54:07.942014 strplus-0.0.7/strplus/cases.py
--rw-r--r--   0        0        0      548 2023-04-14 20:50:24.051003 strplus-0.0.7/strplus/functions.py
--rw-r--r--   0        0        0     1137 2023-04-14 23:01:10.671058 strplus-0.0.7/strplus/strplus.py
--rw-r--r--   0        0        0     2983 1970-01-01 00:00:00.000000 strplus-0.0.7/setup.py
--rw-r--r--   0        0        0     2926 1970-01-01 00:00:00.000000 strplus-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-14 07:41:30.953611 strplus-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2343 2023-04-16 14:30:37.167669 strplus-0.0.8/README.md
+-rw-r--r--   0        0        0      847 2023-04-16 10:54:10.661534 strplus-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      161 2023-04-16 09:50:28.142670 strplus-0.0.8/strplus/__init__.py
+-rw-r--r--   0        0        0     4243 2023-04-16 11:19:57.781075 strplus-0.0.8/strplus/cases.py
+-rw-r--r--   0        0        0      542 2023-04-16 09:50:28.152670 strplus-0.0.8/strplus/functions.py
+-rw-r--r--   0        0        0     3868 2023-04-16 11:19:57.781075 strplus-0.0.8/strplus/strplus.py
+-rw-r--r--   0        0        0     2982 1970-01-01 00:00:00.000000 strplus-0.0.8/setup.py
+-rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 strplus-0.0.8/PKG-INFO
```

### Comparing `strplus-0.0.7/LICENSE` & `strplus-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `strplus-0.0.7/README.md` & `strplus-0.0.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -27,39 +27,39 @@
 Python extra functions for strings ❤️
 </h1>
 
 <br>
 <br>
 <br>
 <br>
+
+[Documentation](https://wiseupdata.github.io/strplus/index.html)  🚀
+
 <br>
+
+## Features ✨️
+
+- Wrapper Class
+- +234 test in 32 Tests files!
+- Simple use! 
+
 <br>
 
+### Simple use example 😍
 ```
-from strplus import Str
-s = Str("hello")
-assert s.upper() == "HELLO"
+>>> my_string = Str('this_is-an_example')
+>>> my_string.camel()
+'thisIsAnExample'
 ```
-
-<br>
-<br>
 <br>
-<br>
-<a href="https://github.com/wiseupdata/wiseupdata">
-<img align="center" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/under_construction.gif" width="300" />
-</a>
+
+> Check the documentations for more examples: [Documentation](https://wiseupdata.github.io/strplus/index.html)! 
 
 <br>
 <br>
-<br>
-
-
-![](https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/20230414_203231_image.png)
-
-
 
 # References 🌍 🗄️
 
 1. [Wise Up Data](https://github.com/wiseupdata)
 2. [Emojis](https://github.com/wiseupdata/emojis)
 3. [Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)
```

#### html2text {}

```diff
@@ -5,28 +5,26 @@
 
 [img]
 ****** Python extra functions for strings â¤ï¸ ******
 
 
 
 
+[Documentation](https://wiseupdata.github.io/strplus/index.html) ð
+## Features â¨ï¸ - Wrapper Class - +234 test in 32 Tests files! - Simple use!
 
-
-``` from strplus import Str s = Str("hello") assert s.upper() == "HELLO" ```
-
-
-
-[img]
-
-
-![](https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/
-20230414_203231_image.png) # References ð ðï¸ 1. [Wise Up Data](https://
-github.com/wiseupdata) 2. [Emojis](https://github.com/wiseupdata/emojis) 3.
-[Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-
-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)
+### Simple use example ð ``` >>> my_string = Str('this_is-an_example') >>>
+my_string.camel() 'thisIsAnExample' ```
+> Check the documentations for more examples: [Documentation](https://
+wiseupdata.github.io/strplus/index.html)!
+
+# References ð ðï¸ 1. [Wise Up Data](https://github.com/wiseupdata) 2.
+[Emojis](https://github.com/wiseupdata/emojis) 3. [Pypi Deploy](https://
+www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-
+pypi-using-poetry-on-ubuntu-22-04)
 
 --- #### Maintainer ð¤ ð¨âð» Sivio Liborio ð§
 silvio.liborio@wiseupdata.com silvio-de-melo-liborio_[LinkedIN]
```

### Comparing `strplus-0.0.7/pyproject.toml` & `strplus-0.0.8/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strplus"
-version = "0.0.7"
+version = "0.0.8"
 authors = ["Silvio Liborio <silvio.liborio@wiseupdata.com>"]
 readme = "README.md"
 
 description = "Python extra functions for strings"
 
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -18,11 +18,19 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.0"
 ipykernel = "^6.22.0"
+sphinx = "^6.1.3"
+yummy-sphinx-theme = "^0.1.1"
+pytest-cov = "^4.0.0"
+coverage = "^7.2.3"
+black = "^23.3.0"
+isort = "^5.12.0"
+sphinx-material = "^0.0.35"
+pygments = "^2.15.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `strplus-0.0.7/strplus/functions.py` & `strplus-0.0.8/strplus/functions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from strplus.cases import *
 
+
 def get_separator(input_string):
-    separators = [',', ';', '|', ' ', '\t', ':', '/', '\\', '\n']
-    
+    separators = [",", ";", "|", " ", "\t", ":", "/", "\\", "\n"]
+
     # check each separator in the order of priority
-    for sep in [',', ';', '|', ' ', '\t', ':', '/', '\\', '\n']:
+    for sep in [",", ";", "|", " ", "\t", ":", "/", "\\", "\n"]:
         if sep in input_string:
             sep_count = input_string.count(sep)
             if sep_count == 1:
                 return sep
             elif sep_count > 1:
                 return max(separators, key=input_string.count)
-    
+
     # if no separator was found, return None
-    return None
+    return None
```

### Comparing `strplus-0.0.7/setup.py` & `strplus-0.0.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['strplus']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'strplus',
-    'version': '0.0.7',
+    'version': '0.0.8',
     'description': 'Python extra functions for strings',
-    'long_description': '<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="Wise Up Data\'s Instagram" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/instagram.png" />   \n</a> \n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s Discord" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/discord.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data | Twitter" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/twitter.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s LinkedIN" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/linkedin.png" />\n</a>\n\n![visitors](https://visitor-badge.glitch.me/badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n![license](https://img.shields.io/github/license/wiseupdata/strplus)\n\n---\n\n<br>\n<br>\n\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/python.png" width="300" />\n</a>\n\n<h1>\nPython extra functions for strings ❤️\n</h1>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n\n```\nfrom strplus import Str\ns = Str("hello")\nassert s.upper() == "HELLO"\n```\n\n<br>\n<br>\n<br>\n<br>\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="center" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/under_construction.gif" width="300" />\n</a>\n\n<br>\n<br>\n<br>\n\n\n![](https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/20230414_203231_image.png)\n\n\n\n# References 🌍 🗄️\n\n1. [Wise Up Data](https://github.com/wiseupdata)\n2. [Emojis](https://github.com/wiseupdata/emojis)\n3. [Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)\n\n<br>\n<br>\n---\n\n#### Maintainer 🤗 👨\u200d💻\n\nSivio Liborio\n\n📧 silvio.liborio@wiseupdata.com\n\n<a href="https://www.linkedin.com/in/silvio-de-melo-liborio">silvio-de-melo-liborio <img align="left" alt="LinkedIN" width="18px" src="https://raw.githubusercontent.com/wiseupdata/wsl-latest/main/assets/linkedin.svg" />\n</a>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n\n> WiseUpData\n',
+    'long_description': '<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="Wise Up Data\'s Instagram" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/instagram.png" />   \n</a> \n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s Discord" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/discord.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data | Twitter" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/twitter.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s LinkedIN" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/linkedin.png" />\n</a>\n\n![visitors](https://visitor-badge.glitch.me/badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n![license](https://img.shields.io/github/license/wiseupdata/strplus)\n\n---\n\n<br>\n<br>\n\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/python.png" width="300" />\n</a>\n\n<h1>\nPython extra functions for strings ❤️\n</h1>\n\n<br>\n<br>\n<br>\n<br>\n\n[Documentation](https://wiseupdata.github.io/strplus/index.html)  🚀\n\n<br>\n\n## Features ✨️\n\n- Wrapper Class\n- +234 test in 32 Tests files!\n- Simple use! \n\n<br>\n\n### Simple use example 😍\n```\n>>> my_string = Str(\'this_is-an_example\')\n>>> my_string.camel()\n\'thisIsAnExample\'\n```\n<br>\n\n> Check the documentations for more examples: [Documentation](https://wiseupdata.github.io/strplus/index.html)! \n\n<br>\n<br>\n\n# References 🌍 🗄️\n\n1. [Wise Up Data](https://github.com/wiseupdata)\n2. [Emojis](https://github.com/wiseupdata/emojis)\n3. [Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)\n\n<br>\n<br>\n---\n\n#### Maintainer 🤗 👨\u200d💻\n\nSivio Liborio\n\n📧 silvio.liborio@wiseupdata.com\n\n<a href="https://www.linkedin.com/in/silvio-de-melo-liborio">silvio-de-melo-liborio <img align="left" alt="LinkedIN" width="18px" src="https://raw.githubusercontent.com/wiseupdata/wsl-latest/main/assets/linkedin.svg" />\n</a>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n\n> WiseUpData\n',
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
@@ -1,38 +1,34 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['strplus']
 package_data = \ {'': ['*']} setup_kwargs = { 'name': 'strplus', 'version':
-'0.0.7', 'description': 'Python extra functions for strings',
+'0.0.8', 'description': 'Python extra functions for strings',
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
-\n
-\n
-\n\n```\nfrom strplus import Str\ns = Str("hello")\nassert s.upper() ==
-"HELLO"\n```\n\n
-\n
-\n
-\n
-\n\n[img]\n\n\n
-\n
-\n
-\n\n\n![](https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/
-20230414_203231_image.png)\n\n\n\n# References ð ðï¸\n\n1. [Wise Up
-Data](https://github.com/wiseupdata)\n2. [Emojis](https://github.com/
-wiseupdata/emojis)\n3. [Pypi Deploy](https://www.digitalocean.com/community/
-tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-
-04)\n\n
+\n\n[Documentation](https://wiseupdata.github.io/strplus/index.html) ð\n\n
+\n\n## Features â¨ï¸\n\n- Wrapper Class\n- +234 test in 32 Tests files!\n-
+Simple use! \n\n
+\n\n### Simple use example ð\n```\n>>> my_string = Str(\'this_is-
+an_example\')\n>>> my_string.camel()\n\'thisIsAnExample\'\n```\n
+\n\n> Check the documentations for more examples: [Documentation](https://
+wiseupdata.github.io/strplus/index.html)! \n\n
+\n
+\n\n# References ð ðï¸\n\n1. [Wise Up Data](https://github.com/
+wiseupdata)\n2. [Emojis](https://github.com/wiseupdata/emojis)\n3. [Pypi
+Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-
+packages-to-pypi-using-poetry-on-ubuntu-22-04)\n\n
 \n
 \n---\n\n#### Maintainer ð¤ ð¨\u200dð»\n\nSivio Liborio\n\nð§
 silvio.liborio@wiseupdata.com\n\nsilvio-de-melo-liborio_[LinkedIN]\n\n\n
 \n
 \n
 \n
 \n
```

