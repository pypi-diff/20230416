# Comparing `tmp/japura-0.1.0.tar.gz` & `tmp/japura-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "japura-0.1.0.tar", last modified: Mon Apr  3 07:33:22 2023, max compression
+gzip compressed data, was "japura-0.2.0.tar", last modified: Sun Apr 16 09:02:00 2023, max compression
```

## Comparing `japura-0.1.0.tar` & `japura-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:33:22.147575 japura-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-03 07:33:09.000000 japura-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-03 07:33:22.147575 japura-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-03 07:33:09.000000 japura-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:33:22.147575 japura-0.1.0/japura/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-03 07:33:09.000000 japura-0.1.0/japura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-03 07:33:09.000000 japura-0.1.0/japura/efs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-03 07:33:09.000000 japura-0.1.0/japura/key.py
--rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-04-03 07:33:09.000000 japura-0.1.0/japura/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:33:22.147575 japura-0.1.0/japura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-03 07:33:22.000000 japura-0.1.0/japura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-03 07:33:22.000000 japura-0.1.0/japura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 07:33:22.000000 japura-0.1.0/japura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-03 07:33:22.000000 japura-0.1.0/japura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-03 07:33:22.000000 japura-0.1.0/japura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-03 07:33:09.000000 japura-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 07:33:22.151576 japura-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:33:22.147575 japura-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-03 07:33:09.000000 japura-0.1.0/tests/test_efs.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-03 07:33:09.000000 japura-0.1.0/tests/test_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-03 07:33:09.000000 japura-0.1.0/tests/test_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:00.064868 japura-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-16 09:01:48.000000 japura-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-16 09:02:00.064868 japura-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-16 09:01:48.000000 japura-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:00.064868 japura-0.2.0/japura/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-16 09:01:48.000000 japura-0.2.0/japura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-16 09:01:48.000000 japura-0.2.0/japura/efs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-16 09:01:48.000000 japura-0.2.0/japura/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-04-16 09:01:48.000000 japura-0.2.0/japura/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:00.064868 japura-0.2.0/japura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-16 09:02:00.000000 japura-0.2.0/japura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-16 09:02:00.000000 japura-0.2.0/japura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 09:02:00.000000 japura-0.2.0/japura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-16 09:02:00.000000 japura-0.2.0/japura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-16 09:02:00.000000 japura-0.2.0/japura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-16 09:01:48.000000 japura-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 09:02:00.064868 japura-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:00.064868 japura-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-16 09:01:48.000000 japura-0.2.0/tests/test_efs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-16 09:01:48.000000 japura-0.2.0/tests/test_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-16 09:01:48.000000 japura-0.2.0/tests/test_sql.py
```

### Comparing `japura-0.1.0/LICENSE` & `japura-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `japura-0.1.0/PKG-INFO` & `japura-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: japura
-Version: 0.1.0
+Version: 0.2.0
 Summary: The Python library for securing and managing web resources.
 Author-email: Joumaico Maulas <joumaico@gmx.com>
 License: MIT License
         
         Copyright (c) 2023 joumaico
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,31 +28,31 @@
 Project-URL: Homepage, https://github.com/joumaico/japura/
 Project-URL: Documentation, https://joumaico.github.io/japura/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Japura
 
-[![Made with Python](https://img.shields.io/badge/Python->=3.10-blue?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
+[![Made with Python](https://img.shields.io/badge/Python->=3.9-blue?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 [![Python package](https://github.com/joumaico/japura/actions/workflows/python-package.yml/badge.svg)](https://github.com/joumaico/japura/actions/workflows/python-package.yml)
 [![Upload Python Package](https://github.com/joumaico/japura/actions/workflows/python-publish.yml/badge.svg)](https://github.com/joumaico/japura/actions/workflows/python-publish.yml)
 
 **Japura** offers a comprehensive set of tools for managing web-based projects like database management, password management, and file encryption. Whether you're a developer working on a large-scale web application or an individual looking to streamline your workflow, this package provides a robust and flexible solution for managing web resources.
 
 ## Installing Japura and Supported Versions
 
 ```console
 $ pip install japura
 ```
 
-Japura officially supports Python 3.10+.
+Japura officially supports Python 3.9+.
 
 ## Links
 * Documentation: https://joumaico.github.io/japura/
 * PyPI Releases: https://pypi.org/project/japura/
 * Source Code: https://github.com/joumaico/japura/
```

### Comparing `japura-0.1.0/README.md` & `japura-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Japura
 
-[![Made with Python](https://img.shields.io/badge/Python->=3.10-blue?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
+[![Made with Python](https://img.shields.io/badge/Python->=3.9-blue?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 [![Python package](https://github.com/joumaico/japura/actions/workflows/python-package.yml/badge.svg)](https://github.com/joumaico/japura/actions/workflows/python-package.yml)
 [![Upload Python Package](https://github.com/joumaico/japura/actions/workflows/python-publish.yml/badge.svg)](https://github.com/joumaico/japura/actions/workflows/python-publish.yml)
 
 **Japura** offers a comprehensive set of tools for managing web-based projects like database management, password management, and file encryption. Whether you're a developer working on a large-scale web application or an individual looking to streamline your workflow, this package provides a robust and flexible solution for managing web resources.
 
 ## Installing Japura and Supported Versions
 
 ```console
 $ pip install japura
 ```
 
-Japura officially supports Python 3.10+.
+Japura officially supports Python 3.9+.
 
 ## Links
 * Documentation: https://joumaico.github.io/japura/
 * PyPI Releases: https://pypi.org/project/japura/
 * Source Code: https://github.com/joumaico/japura/
```

### Comparing `japura-0.1.0/japura/efs.py` & `japura-0.2.0/japura/efs.py`

 * *Files identical despite different names*

### Comparing `japura-0.1.0/japura/key.py` & `japura-0.2.0/japura/key.py`

 * *Files identical despite different names*

### Comparing `japura-0.1.0/japura/sql.py` & `japura-0.2.0/japura/sql.py`

 * *Files identical despite different names*

### Comparing `japura-0.1.0/japura.egg-info/PKG-INFO` & `japura-0.2.0/japura.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: japura
-Version: 0.1.0
+Version: 0.2.0
 Summary: The Python library for securing and managing web resources.
 Author-email: Joumaico Maulas <joumaico@gmx.com>
 License: MIT License
         
         Copyright (c) 2023 joumaico
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,31 +28,31 @@
 Project-URL: Homepage, https://github.com/joumaico/japura/
 Project-URL: Documentation, https://joumaico.github.io/japura/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Japura
 
-[![Made with Python](https://img.shields.io/badge/Python->=3.10-blue?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
+[![Made with Python](https://img.shields.io/badge/Python->=3.9-blue?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 [![Python package](https://github.com/joumaico/japura/actions/workflows/python-package.yml/badge.svg)](https://github.com/joumaico/japura/actions/workflows/python-package.yml)
 [![Upload Python Package](https://github.com/joumaico/japura/actions/workflows/python-publish.yml/badge.svg)](https://github.com/joumaico/japura/actions/workflows/python-publish.yml)
 
 **Japura** offers a comprehensive set of tools for managing web-based projects like database management, password management, and file encryption. Whether you're a developer working on a large-scale web application or an individual looking to streamline your workflow, this package provides a robust and flexible solution for managing web resources.
 
 ## Installing Japura and Supported Versions
 
 ```console
 $ pip install japura
 ```
 
-Japura officially supports Python 3.10+.
+Japura officially supports Python 3.9+.
 
 ## Links
 * Documentation: https://joumaico.github.io/japura/
 * PyPI Releases: https://pypi.org/project/japura/
 * Source Code: https://github.com/joumaico/japura/
```

### Comparing `japura-0.1.0/pyproject.toml` & `japura-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 dependencies = [
     "bcrypt>=4.0.1",
     "cryptography>=40.0.1",
     "pymysql>=1.0.3",
 ]
 dynamic = ["version"]
```

### Comparing `japura-0.1.0/tests/test_key.py` & `japura-0.2.0/tests/test_key.py`

 * *Files identical despite different names*

### Comparing `japura-0.1.0/tests/test_sql.py` & `japura-0.2.0/tests/test_sql.py`

 * *Files identical despite different names*

