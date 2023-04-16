# Comparing `tmp/py_spacy_redact_message-0.0.23.tar.gz` & `tmp/py_spacy_redact_message-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_spacy_redact_message-0.0.23.tar", last modified: Sun Apr 16 10:23:36 2023, max compression
+gzip compressed data, was "py_spacy_redact_message-0.0.24.tar", last modified: Sun Apr 16 10:53:51 2023, max compression
```

## Comparing `py_spacy_redact_message-0.0.23.tar` & `py_spacy_redact_message-0.0.24.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-16 10:23:36.896273 py_spacy_redact_message-0.0.23/
--rw-r--r--   0 alexilin   (501) staff       (20)     1068 2023-04-15 10:09:58.000000 py_spacy_redact_message-0.0.23/LICENSE
--rw-r--r--   0 alexilin   (501) staff       (20)      447 2023-04-16 10:23:36.896114 py_spacy_redact_message-0.0.23/PKG-INFO
--rw-r--r--   0 alexilin   (501) staff       (20)       30 2023-04-15 10:08:06.000000 py_spacy_redact_message-0.0.23/README.md
-drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-16 10:23:36.894871 py_spacy_redact_message-0.0.23/py_spacy_redact_message/
--rw-r--r--   0 alexilin   (501) staff       (20)        0 2023-04-15 10:52:13.000000 py_spacy_redact_message-0.0.23/py_spacy_redact_message/__init__.py
--rw-r--r--   0 alexilin   (501) staff       (20)      780 2023-04-16 09:51:51.000000 py_spacy_redact_message-0.0.23/py_spacy_redact_message/main.py
-drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-16 10:23:36.895950 py_spacy_redact_message-0.0.23/py_spacy_redact_message.egg-info/
--rw-r--r--   0 alexilin   (501) staff       (20)      447 2023-04-16 10:23:36.000000 py_spacy_redact_message-0.0.23/py_spacy_redact_message.egg-info/PKG-INFO
--rw-r--r--   0 alexilin   (501) staff       (20)      393 2023-04-16 10:23:36.000000 py_spacy_redact_message-0.0.23/py_spacy_redact_message.egg-info/SOURCES.txt
--rw-r--r--   0 alexilin   (501) staff       (20)        1 2023-04-16 10:23:36.000000 py_spacy_redact_message-0.0.23/py_spacy_redact_message.egg-info/dependency_links.txt
--rw-r--r--   0 alexilin   (501) staff       (20)       77 2023-04-16 10:23:36.000000 py_spacy_redact_message-0.0.23/py_spacy_redact_message.egg-info/entry_points.txt
--rw-r--r--   0 alexilin   (501) staff       (20)       12 2023-04-16 10:23:36.000000 py_spacy_redact_message-0.0.23/py_spacy_redact_message.egg-info/requires.txt
--rw-r--r--   0 alexilin   (501) staff       (20)       24 2023-04-16 10:23:36.000000 py_spacy_redact_message-0.0.23/py_spacy_redact_message.egg-info/top_level.txt
--rw-r--r--   0 alexilin   (501) staff       (20)       89 2023-04-16 10:05:29.000000 py_spacy_redact_message-0.0.23/pyproject.toml
--rw-r--r--   0 alexilin   (501) staff       (20)       38 2023-04-16 10:23:36.896310 py_spacy_redact_message-0.0.23/setup.cfg
--rw-r--r--   0 alexilin   (501) staff       (20)      836 2023-04-16 10:23:27.000000 py_spacy_redact_message-0.0.23/setup.py
+drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-16 10:53:51.793865 py_spacy_redact_message-0.0.24/
+-rw-r--r--   0 alexilin   (501) staff       (20)     1068 2023-04-15 10:09:58.000000 py_spacy_redact_message-0.0.24/LICENSE
+-rw-r--r--   0 alexilin   (501) staff       (20)      597 2023-04-16 10:53:51.793680 py_spacy_redact_message-0.0.24/PKG-INFO
+-rw-r--r--   0 alexilin   (501) staff       (20)       30 2023-04-15 10:08:06.000000 py_spacy_redact_message-0.0.24/README.md
+drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-16 10:53:51.791968 py_spacy_redact_message-0.0.24/py_spacy_redact_message/
+-rw-r--r--   0 alexilin   (501) staff       (20)        0 2023-04-15 10:52:13.000000 py_spacy_redact_message-0.0.24/py_spacy_redact_message/__init__.py
+-rw-r--r--   0 alexilin   (501) staff       (20)      780 2023-04-16 09:51:51.000000 py_spacy_redact_message-0.0.24/py_spacy_redact_message/main.py
+drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-16 10:53:51.793489 py_spacy_redact_message-0.0.24/py_spacy_redact_message.egg-info/
+-rw-r--r--   0 alexilin   (501) staff       (20)      597 2023-04-16 10:53:51.000000 py_spacy_redact_message-0.0.24/py_spacy_redact_message.egg-info/PKG-INFO
+-rw-r--r--   0 alexilin   (501) staff       (20)      393 2023-04-16 10:53:51.000000 py_spacy_redact_message-0.0.24/py_spacy_redact_message.egg-info/SOURCES.txt
+-rw-r--r--   0 alexilin   (501) staff       (20)        1 2023-04-16 10:53:51.000000 py_spacy_redact_message-0.0.24/py_spacy_redact_message.egg-info/dependency_links.txt
+-rw-r--r--   0 alexilin   (501) staff       (20)       77 2023-04-16 10:53:51.000000 py_spacy_redact_message-0.0.24/py_spacy_redact_message.egg-info/entry_points.txt
+-rw-r--r--   0 alexilin   (501) staff       (20)       12 2023-04-16 10:53:51.000000 py_spacy_redact_message-0.0.24/py_spacy_redact_message.egg-info/requires.txt
+-rw-r--r--   0 alexilin   (501) staff       (20)       24 2023-04-16 10:53:51.000000 py_spacy_redact_message-0.0.24/py_spacy_redact_message.egg-info/top_level.txt
+-rw-r--r--   0 alexilin   (501) staff       (20)       89 2023-04-16 10:05:29.000000 py_spacy_redact_message-0.0.24/pyproject.toml
+-rw-r--r--   0 alexilin   (501) staff       (20)       38 2023-04-16 10:53:51.793906 py_spacy_redact_message-0.0.24/setup.cfg
+-rw-r--r--   0 alexilin   (501) staff       (20)      987 2023-04-16 10:53:47.000000 py_spacy_redact_message-0.0.24/setup.py
```

### Comparing `py_spacy_redact_message-0.0.23/LICENSE` & `py_spacy_redact_message-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `py_spacy_redact_message-0.0.23/py_spacy_redact_message/main.py` & `py_spacy_redact_message-0.0.24/py_spacy_redact_message/main.py`

 * *Files identical despite different names*

### Comparing `py_spacy_redact_message-0.0.23/setup.py` & `py_spacy_redact_message-0.0.24/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.23'
+VERSION = '0.0.24'
 DESCRIPTION = 'Redact message using spacy NER'
-LONG_DESCRIPTION = """## Installation\n\n```pip install ym_csv_pii_sanitizer```\n\n```python -m spacy download en_core_web_sm```\n\n## Usage\n\n```ym_csv_pii_sanitizer PATH_TO_CSV_FILE```"""
+LONG_DESCRIPTION = """
+    ## Installation\n\n
+    Create a Python virtual environment in the directory.
+    ```
+    python3 -m venv .venv
+    source .venv/bin/activate
+    ```
+    ```pip install ym_csv_pii_sanitizer```\n\n
+    ```python -m spacy download en_core_web_sm```\n\n
+    ## Usage\n\n```ym_csv_pii_sanitizer PATH_TO_CSV_FILE```
+"""
 
 setup(
     name="py_spacy_redact_message",
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
```

