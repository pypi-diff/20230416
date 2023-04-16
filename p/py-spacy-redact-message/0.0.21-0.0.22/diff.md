# Comparing `tmp/py_spacy_redact_message-0.0.21.tar.gz` & `tmp/py_spacy_redact_message-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_spacy_redact_message-0.0.21.tar", last modified: Sun Apr 16 09:56:44 2023, max compression
+gzip compressed data, was "py_spacy_redact_message-0.0.22.tar", last modified: Sun Apr 16 10:07:41 2023, max compression
```

## Comparing `py_spacy_redact_message-0.0.21.tar` & `py_spacy_redact_message-0.0.22.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-16 09:56:44.193622 py_spacy_redact_message-0.0.21/
--rw-r--r--   0 alexilin   (501) staff       (20)     1068 2023-04-15 10:09:58.000000 py_spacy_redact_message-0.0.21/LICENSE
--rw-r--r--   0 alexilin   (501) staff       (20)      245 2023-04-16 09:56:44.193442 py_spacy_redact_message-0.0.21/PKG-INFO
--rw-r--r--   0 alexilin   (501) staff       (20)       30 2023-04-15 10:08:06.000000 py_spacy_redact_message-0.0.21/README.md
-drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-16 09:56:44.191939 py_spacy_redact_message-0.0.21/py_spacy_redact_message/
--rw-r--r--   0 alexilin   (501) staff       (20)        0 2023-04-15 10:52:13.000000 py_spacy_redact_message-0.0.21/py_spacy_redact_message/__init__.py
--rw-r--r--   0 alexilin   (501) staff       (20)      780 2023-04-16 09:51:51.000000 py_spacy_redact_message-0.0.21/py_spacy_redact_message/main.py
-drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-16 09:56:44.193224 py_spacy_redact_message-0.0.21/py_spacy_redact_message.egg-info/
--rw-r--r--   0 alexilin   (501) staff       (20)      245 2023-04-16 09:56:44.000000 py_spacy_redact_message-0.0.21/py_spacy_redact_message.egg-info/PKG-INFO
--rw-r--r--   0 alexilin   (501) staff       (20)      384 2023-04-16 09:56:44.000000 py_spacy_redact_message-0.0.21/py_spacy_redact_message.egg-info/SOURCES.txt
--rw-r--r--   0 alexilin   (501) staff       (20)        1 2023-04-16 09:56:44.000000 py_spacy_redact_message-0.0.21/py_spacy_redact_message.egg-info/dependency_links.txt
--rw-r--r--   0 alexilin   (501) staff       (20)       77 2023-04-16 09:56:44.000000 py_spacy_redact_message-0.0.21/py_spacy_redact_message.egg-info/entry_points.txt
--rw-r--r--   0 alexilin   (501) staff       (20)       12 2023-04-16 09:56:44.000000 py_spacy_redact_message-0.0.21/py_spacy_redact_message.egg-info/requires.txt
--rw-r--r--   0 alexilin   (501) staff       (20)       24 2023-04-16 09:56:44.000000 py_spacy_redact_message-0.0.21/py_spacy_redact_message.egg-info/top_level.txt
--rw-r--r--   0 alexilin   (501) staff       (20)      516 2023-04-16 09:56:39.000000 py_spacy_redact_message-0.0.21/pyproject.toml
--rw-r--r--   0 alexilin   (501) staff       (20)       38 2023-04-16 09:56:44.193666 py_spacy_redact_message-0.0.21/setup.cfg
+drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-16 10:07:41.145393 py_spacy_redact_message-0.0.22/
+-rw-r--r--   0 alexilin   (501) staff       (20)     1068 2023-04-15 10:09:58.000000 py_spacy_redact_message-0.0.22/LICENSE
+-rw-r--r--   0 alexilin   (501) staff       (20)      446 2023-04-16 10:07:41.145215 py_spacy_redact_message-0.0.22/PKG-INFO
+-rw-r--r--   0 alexilin   (501) staff       (20)       30 2023-04-15 10:08:06.000000 py_spacy_redact_message-0.0.22/README.md
+drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-16 10:07:41.144182 py_spacy_redact_message-0.0.22/py_spacy_redact_message/
+-rw-r--r--   0 alexilin   (501) staff       (20)        0 2023-04-15 10:52:13.000000 py_spacy_redact_message-0.0.22/py_spacy_redact_message/__init__.py
+-rw-r--r--   0 alexilin   (501) staff       (20)      780 2023-04-16 09:51:51.000000 py_spacy_redact_message-0.0.22/py_spacy_redact_message/main.py
+drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-16 10:07:41.145036 py_spacy_redact_message-0.0.22/py_spacy_redact_message.egg-info/
+-rw-r--r--   0 alexilin   (501) staff       (20)      446 2023-04-16 10:07:41.000000 py_spacy_redact_message-0.0.22/py_spacy_redact_message.egg-info/PKG-INFO
+-rw-r--r--   0 alexilin   (501) staff       (20)      393 2023-04-16 10:07:41.000000 py_spacy_redact_message-0.0.22/py_spacy_redact_message.egg-info/SOURCES.txt
+-rw-r--r--   0 alexilin   (501) staff       (20)        1 2023-04-16 10:07:41.000000 py_spacy_redact_message-0.0.22/py_spacy_redact_message.egg-info/dependency_links.txt
+-rw-r--r--   0 alexilin   (501) staff       (20)       77 2023-04-16 10:07:41.000000 py_spacy_redact_message-0.0.22/py_spacy_redact_message.egg-info/entry_points.txt
+-rw-r--r--   0 alexilin   (501) staff       (20)       12 2023-04-16 10:07:41.000000 py_spacy_redact_message-0.0.22/py_spacy_redact_message.egg-info/requires.txt
+-rw-r--r--   0 alexilin   (501) staff       (20)       24 2023-04-16 10:07:41.000000 py_spacy_redact_message-0.0.22/py_spacy_redact_message.egg-info/top_level.txt
+-rw-r--r--   0 alexilin   (501) staff       (20)       89 2023-04-16 10:05:29.000000 py_spacy_redact_message-0.0.22/pyproject.toml
+-rw-r--r--   0 alexilin   (501) staff       (20)       38 2023-04-16 10:07:41.145433 py_spacy_redact_message-0.0.22/setup.cfg
+-rw-r--r--   0 alexilin   (501) staff       (20)      834 2023-04-16 10:07:25.000000 py_spacy_redact_message-0.0.22/setup.py
```

### Comparing `py_spacy_redact_message-0.0.21/LICENSE` & `py_spacy_redact_message-0.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `py_spacy_redact_message-0.0.21/py_spacy_redact_message/main.py` & `py_spacy_redact_message-0.0.22/py_spacy_redact_message/main.py`

 * *Files identical despite different names*

