# Comparing `tmp/py_spacy_redact_message-0.0.25.tar.gz` & `tmp/py_spacy_redact_message-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_spacy_redact_message-0.0.25.tar", last modified: Sun Apr 16 10:57:30 2023, max compression
+gzip compressed data, was "py_spacy_redact_message-0.0.26.tar", last modified: Sun Apr 16 10:58:43 2023, max compression
```

## Comparing `py_spacy_redact_message-0.0.25.tar` & `py_spacy_redact_message-0.0.26.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-16 10:57:30.661903 py_spacy_redact_message-0.0.25/
--rw-r--r--   0 alexilin   (501) staff       (20)     1068 2023-04-15 10:09:58.000000 py_spacy_redact_message-0.0.25/LICENSE
--rw-r--r--   0 alexilin   (501) staff       (20)      592 2023-04-16 10:57:30.661702 py_spacy_redact_message-0.0.25/PKG-INFO
--rw-r--r--   0 alexilin   (501) staff       (20)       30 2023-04-15 10:08:06.000000 py_spacy_redact_message-0.0.25/README.md
-drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-16 10:57:30.660414 py_spacy_redact_message-0.0.25/py_spacy_redact_message/
--rw-r--r--   0 alexilin   (501) staff       (20)        0 2023-04-15 10:52:13.000000 py_spacy_redact_message-0.0.25/py_spacy_redact_message/__init__.py
--rw-r--r--   0 alexilin   (501) staff       (20)      780 2023-04-16 09:51:51.000000 py_spacy_redact_message-0.0.25/py_spacy_redact_message/main.py
-drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-16 10:57:30.661486 py_spacy_redact_message-0.0.25/py_spacy_redact_message.egg-info/
--rw-r--r--   0 alexilin   (501) staff       (20)      592 2023-04-16 10:57:30.000000 py_spacy_redact_message-0.0.25/py_spacy_redact_message.egg-info/PKG-INFO
--rw-r--r--   0 alexilin   (501) staff       (20)      393 2023-04-16 10:57:30.000000 py_spacy_redact_message-0.0.25/py_spacy_redact_message.egg-info/SOURCES.txt
--rw-r--r--   0 alexilin   (501) staff       (20)        1 2023-04-16 10:57:30.000000 py_spacy_redact_message-0.0.25/py_spacy_redact_message.egg-info/dependency_links.txt
--rw-r--r--   0 alexilin   (501) staff       (20)       77 2023-04-16 10:57:30.000000 py_spacy_redact_message-0.0.25/py_spacy_redact_message.egg-info/entry_points.txt
--rw-r--r--   0 alexilin   (501) staff       (20)       12 2023-04-16 10:57:30.000000 py_spacy_redact_message-0.0.25/py_spacy_redact_message.egg-info/requires.txt
--rw-r--r--   0 alexilin   (501) staff       (20)       24 2023-04-16 10:57:30.000000 py_spacy_redact_message-0.0.25/py_spacy_redact_message.egg-info/top_level.txt
--rw-r--r--   0 alexilin   (501) staff       (20)       89 2023-04-16 10:05:29.000000 py_spacy_redact_message-0.0.25/pyproject.toml
--rw-r--r--   0 alexilin   (501) staff       (20)       38 2023-04-16 10:57:30.661947 py_spacy_redact_message-0.0.25/setup.cfg
--rw-r--r--   0 alexilin   (501) staff       (20)      981 2023-04-16 10:57:19.000000 py_spacy_redact_message-0.0.25/setup.py
+drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-16 10:58:43.851754 py_spacy_redact_message-0.0.26/
+-rw-r--r--   0 alexilin   (501) staff       (20)     1068 2023-04-15 10:09:58.000000 py_spacy_redact_message-0.0.26/LICENSE
+-rw-r--r--   0 alexilin   (501) staff       (20)      592 2023-04-16 10:58:43.851567 py_spacy_redact_message-0.0.26/PKG-INFO
+-rw-r--r--   0 alexilin   (501) staff       (20)       30 2023-04-15 10:08:06.000000 py_spacy_redact_message-0.0.26/README.md
+drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-16 10:58:43.850054 py_spacy_redact_message-0.0.26/py_spacy_redact_message/
+-rw-r--r--   0 alexilin   (501) staff       (20)        0 2023-04-15 10:52:13.000000 py_spacy_redact_message-0.0.26/py_spacy_redact_message/__init__.py
+-rw-r--r--   0 alexilin   (501) staff       (20)      780 2023-04-16 09:51:51.000000 py_spacy_redact_message-0.0.26/py_spacy_redact_message/main.py
+drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-16 10:58:43.851357 py_spacy_redact_message-0.0.26/py_spacy_redact_message.egg-info/
+-rw-r--r--   0 alexilin   (501) staff       (20)      592 2023-04-16 10:58:43.000000 py_spacy_redact_message-0.0.26/py_spacy_redact_message.egg-info/PKG-INFO
+-rw-r--r--   0 alexilin   (501) staff       (20)      393 2023-04-16 10:58:43.000000 py_spacy_redact_message-0.0.26/py_spacy_redact_message.egg-info/SOURCES.txt
+-rw-r--r--   0 alexilin   (501) staff       (20)        1 2023-04-16 10:58:43.000000 py_spacy_redact_message-0.0.26/py_spacy_redact_message.egg-info/dependency_links.txt
+-rw-r--r--   0 alexilin   (501) staff       (20)       77 2023-04-16 10:58:43.000000 py_spacy_redact_message-0.0.26/py_spacy_redact_message.egg-info/entry_points.txt
+-rw-r--r--   0 alexilin   (501) staff       (20)       12 2023-04-16 10:58:43.000000 py_spacy_redact_message-0.0.26/py_spacy_redact_message.egg-info/requires.txt
+-rw-r--r--   0 alexilin   (501) staff       (20)       24 2023-04-16 10:58:43.000000 py_spacy_redact_message-0.0.26/py_spacy_redact_message.egg-info/top_level.txt
+-rw-r--r--   0 alexilin   (501) staff       (20)       89 2023-04-16 10:05:29.000000 py_spacy_redact_message-0.0.26/pyproject.toml
+-rw-r--r--   0 alexilin   (501) staff       (20)       38 2023-04-16 10:58:43.851792 py_spacy_redact_message-0.0.26/setup.cfg
+-rw-r--r--   0 alexilin   (501) staff       (20)      985 2023-04-16 10:58:38.000000 py_spacy_redact_message-0.0.26/setup.py
```

### Comparing `py_spacy_redact_message-0.0.25/LICENSE` & `py_spacy_redact_message-0.0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `py_spacy_redact_message-0.0.25/PKG-INFO` & `py_spacy_redact_message-0.0.26/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: py_spacy_redact_message
-Version: 0.0.25
+Version: 0.0.26
 Summary: Redact message using spacy NER
 Author: Alex Ilin
 Author-email: ilin.alex.mail@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Installation
 
 
     Create a Python virtual environment in the directory.
-    ```
-    python3 -m venv .venv
-    source .venv/bin/activate
-    ```
+    ```python3 -m venv .venv```
+
+
+    ```source .venv/bin/activate```
+
+
     ```pip install ym_csv_pii_sanitizer```
 
 
     ```python -m spacy download en_core_web_sm```
 
 
     ## Usage
```

### Comparing `py_spacy_redact_message-0.0.25/py_spacy_redact_message/main.py` & `py_spacy_redact_message-0.0.26/py_spacy_redact_message/main.py`

 * *Files identical despite different names*

### Comparing `py_spacy_redact_message-0.0.25/py_spacy_redact_message.egg-info/PKG-INFO` & `py_spacy_redact_message-0.0.26/py_spacy_redact_message.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: py-spacy-redact-message
-Version: 0.0.25
+Version: 0.0.26
 Summary: Redact message using spacy NER
 Author: Alex Ilin
 Author-email: ilin.alex.mail@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Installation
 
 
     Create a Python virtual environment in the directory.
-    ```
-    python3 -m venv .venv
-    source .venv/bin/activate
-    ```
+    ```python3 -m venv .venv```
+
+
+    ```source .venv/bin/activate```
+
+
     ```pip install ym_csv_pii_sanitizer```
 
 
     ```python -m spacy download en_core_web_sm```
 
 
     ## Usage
```

### Comparing `py_spacy_redact_message-0.0.25/setup.py` & `py_spacy_redact_message-0.0.26/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.25'
+VERSION = '0.0.26'
 DESCRIPTION = 'Redact message using spacy NER'
 LONG_DESCRIPTION = """## Installation\n\n
     Create a Python virtual environment in the directory.
-    ```
-    python3 -m venv .venv
-    source .venv/bin/activate
-    ```
+    ```python3 -m venv .venv```\n\n
+    ```source .venv/bin/activate```\n\n
     ```pip install ym_csv_pii_sanitizer```\n\n
     ```python -m spacy download en_core_web_sm```\n\n
     ## Usage\n\n```ym_csv_pii_sanitizer PATH_TO_CSV_FILE```"""
 
 setup(
     name="py_spacy_redact_message",
     version=VERSION,
```

