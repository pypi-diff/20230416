# Comparing `tmp/SrbAI-0.0.3.tar.gz` & `tmp/SrbAI-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/SrbAI/SrbAI/dist/tmpcvss5cj6/SrbAI-0.0.3.tar", last modified: Mon Feb 28 22:08:08 2022, max compression
+gzip compressed data, was "/home/runner/work/SrbAI/SrbAI/dist/.tmp-kukpdx7n/SrbAI-0.0.4.tar", last modified: Sun Apr 16 07:13:46 2023, max compression
```

## Comparing `SrbAI-0.0.3.tar` & `SrbAI-0.0.4.tar`

### file list

```diff
@@ -1,33 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 22:08:08.000000 SrbAI-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1057 2022-02-28 22:07:09.000000 SrbAI-0.0.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 22:08:08.000000 SrbAI-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 22:08:08.000000 SrbAI-0.0.3/src/srbai/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-02-28 22:07:09.000000 SrbAI-0.0.3/src/srbai/test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 22:08:08.000000 SrbAI-0.0.3/src/srbai/NER/
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-02-28 22:07:09.000000 SrbAI-0.0.3/src/srbai/NER/NER_classla.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-28 22:07:09.000000 SrbAI-0.0.3/src/srbai/NER/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 22:08:08.000000 SrbAI-0.0.3/src/srbai/Alati/
--rw-r--r--   0 runner    (1001) docker     (121)     2853 2022-02-28 22:07:09.000000 SrbAI-0.0.3/src/srbai/Alati/Transliterator.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-28 22:07:09.000000 SrbAI-0.0.3/src/srbai/Alati/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 22:08:08.000000 SrbAI-0.0.3/src/srbai/SintaktickiOperatori/
--rw-r--r--   0 runner    (1001) docker     (121)     8410 2022-02-28 22:07:09.000000 SrbAI-0.0.3/src/srbai/SintaktickiOperatori/stemmer_nm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-02-28 22:07:09.000000 SrbAI-0.0.3/src/srbai/SintaktickiOperatori/POS_tagger.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-28 22:07:09.000000 SrbAI-0.0.3/src/srbai/SintaktickiOperatori/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 22:08:08.000000 SrbAI-0.0.3/src/srbai/JezickiModeli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-28 22:07:09.000000 SrbAI-0.0.3/src/srbai/JezickiModeli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-28 22:07:09.000000 SrbAI-0.0.3/src/srbai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 22:08:08.000000 SrbAI-0.0.3/src/srbai/Klasifikatori/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-28 22:07:09.000000 SrbAI-0.0.3/src/srbai/Klasifikatori/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 22:08:08.000000 SrbAI-0.0.3/src/srbai/Glas/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-28 22:07:09.000000 SrbAI-0.0.3/src/srbai/Glas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 22:08:08.000000 SrbAI-0.0.3/src/SrbAI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-02-28 22:08:08.000000 SrbAI-0.0.3/src/SrbAI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3581 2022-02-28 22:08:08.000000 SrbAI-0.0.3/src/SrbAI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-02-28 22:08:08.000000 SrbAI-0.0.3/src/SrbAI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-02-28 22:08:08.000000 SrbAI-0.0.3/src/SrbAI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-28 22:08:08.000000 SrbAI-0.0.3/src/SrbAI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-02-28 22:07:09.000000 SrbAI-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      969 2022-02-28 22:07:09.000000 SrbAI-0.0.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-28 22:08:08.000000 SrbAI-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3581 2022-02-28 22:08:08.000000 SrbAI-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2988 2022-02-28 22:07:09.000000 SrbAI-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:13:46.000000 SrbAI-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-16 07:11:58.000000 SrbAI-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-04-16 07:13:46.000000 SrbAI-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-16 07:11:58.000000 SrbAI-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-16 07:11:58.000000 SrbAI-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 07:13:46.000000 SrbAI-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-16 07:11:58.000000 SrbAI-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:13:46.000000 SrbAI-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:13:46.000000 SrbAI-0.0.4/src/SrbAI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-04-16 07:13:46.000000 SrbAI-0.0.4/src/SrbAI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-16 07:13:46.000000 SrbAI-0.0.4/src/SrbAI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 07:13:46.000000 SrbAI-0.0.4/src/SrbAI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-16 07:13:46.000000 SrbAI-0.0.4/src/SrbAI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 07:13:46.000000 SrbAI-0.0.4/src/SrbAI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:13:46.000000 SrbAI-0.0.4/src/srbai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:13:46.000000 SrbAI-0.0.4/src/srbai/Alati/
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-04-16 07:11:58.000000 SrbAI-0.0.4/src/srbai/Alati/Transliterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 07:11:58.000000 SrbAI-0.0.4/src/srbai/Alati/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:13:46.000000 SrbAI-0.0.4/src/srbai/Glas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 07:11:58.000000 SrbAI-0.0.4/src/srbai/Glas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:13:46.000000 SrbAI-0.0.4/src/srbai/JezickiModeli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:13:46.000000 SrbAI-0.0.4/src/srbai/JezickiModeli/FastText/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 07:11:58.000000 SrbAI-0.0.4/src/srbai/JezickiModeli/FastText/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-16 07:11:58.000000 SrbAI-0.0.4/src/srbai/JezickiModeli/FastText/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-16 07:11:58.000000 SrbAI-0.0.4/src/srbai/JezickiModeli/FastText/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-16 07:11:58.000000 SrbAI-0.0.4/src/srbai/JezickiModeli/FastText/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-16 07:11:58.000000 SrbAI-0.0.4/src/srbai/JezickiModeli/FastText/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-04-16 07:11:58.000000 SrbAI-0.0.4/src/srbai/JezickiModeli/FastText/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-16 07:11:58.000000 SrbAI-0.0.4/src/srbai/JezickiModeli/FastText/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-04-16 07:11:58.000000 SrbAI-0.0.4/src/srbai/JezickiModeli/FastText/text_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 07:11:58.000000 SrbAI-0.0.4/src/srbai/JezickiModeli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:13:46.000000 SrbAI-0.0.4/src/srbai/Klasifikatori/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 07:11:58.000000 SrbAI-0.0.4/src/srbai/Klasifikatori/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:13:46.000000 SrbAI-0.0.4/src/srbai/NER/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-16 07:11:58.000000 SrbAI-0.0.4/src/srbai/NER/NER_classla.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 07:11:58.000000 SrbAI-0.0.4/src/srbai/NER/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:13:46.000000 SrbAI-0.0.4/src/srbai/SintaktickiOperatori/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-16 07:11:58.000000 SrbAI-0.0.4/src/srbai/SintaktickiOperatori/POS_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 07:11:58.000000 SrbAI-0.0.4/src/srbai/SintaktickiOperatori/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-16 07:11:58.000000 SrbAI-0.0.4/src/srbai/SintaktickiOperatori/spellcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-04-16 07:11:58.000000 SrbAI-0.0.4/src/srbai/SintaktickiOperatori/stemmer_nm.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 07:11:58.000000 SrbAI-0.0.4/src/srbai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-16 07:11:58.000000 SrbAI-0.0.4/src/srbai/test.py
```

### Comparing `SrbAI-0.0.3/LICENSE` & `SrbAI-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.3/src/srbai/Alati/Transliterator.py` & `SrbAI-0.0.4/src/srbai/Alati/Transliterator.py`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.3/src/srbai/SintaktickiOperatori/stemmer_nm.py` & `SrbAI-0.0.4/src/srbai/SintaktickiOperatori/stemmer_nm.py`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.3/src/srbai/SintaktickiOperatori/POS_tagger.py` & `SrbAI-0.0.4/src/srbai/SintaktickiOperatori/POS_tagger.py`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.3/setup.py` & `SrbAI-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SrbAI",
-    version="0.0.3",
+    version="0.0.4",
     author="Serbian AI Society",
     author_email="nikola.milosevic86@gmail.com",
     description="Library for processing serbian language",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     project_urls={
@@ -19,15 +19,16 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "numpy",
         "nltk",
-        "torch==1.10.2",
-        "classla==1.1.0"
+        "torch>=1.10.2",
+        "classla==1.1.0",
+        "nlu"
 
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.6",
+    python_requires=">=3.6.15",
 )
```

