# Comparing `tmp/SrbAI-0.0.5.tar.gz` & `tmp/SrbAI-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/SrbAI/SrbAI/dist/.tmp-v94knmwb/SrbAI-0.0.5.tar", last modified: Sun Apr 16 07:24:36 2023, max compression
+gzip compressed data, was "/home/runner/work/SrbAI/SrbAI/dist/.tmp-ytiqcu0b/SrbAI-0.0.6.tar", last modified: Sun Apr 16 16:25:28 2023, max compression
```

## Comparing `SrbAI-0.0.5.tar` & `SrbAI-0.0.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:24:36.000000 SrbAI-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-16 07:22:53.000000 SrbAI-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-16 07:24:36.000000 SrbAI-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-16 07:22:53.000000 SrbAI-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-16 07:22:53.000000 SrbAI-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 07:24:36.000000 SrbAI-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-16 07:22:53.000000 SrbAI-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:24:36.000000 SrbAI-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:24:36.000000 SrbAI-0.0.5/src/SrbAI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-16 07:24:36.000000 SrbAI-0.0.5/src/SrbAI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-16 07:24:36.000000 SrbAI-0.0.5/src/SrbAI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 07:24:36.000000 SrbAI-0.0.5/src/SrbAI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-16 07:24:36.000000 SrbAI-0.0.5/src/SrbAI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 07:24:36.000000 SrbAI-0.0.5/src/SrbAI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:24:36.000000 SrbAI-0.0.5/src/srbai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:24:36.000000 SrbAI-0.0.5/src/srbai/Alati/
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-04-16 07:22:53.000000 SrbAI-0.0.5/src/srbai/Alati/Transliterator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 07:22:53.000000 SrbAI-0.0.5/src/srbai/Alati/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:24:36.000000 SrbAI-0.0.5/src/srbai/Glas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 07:22:53.000000 SrbAI-0.0.5/src/srbai/Glas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:24:36.000000 SrbAI-0.0.5/src/srbai/JezickiModeli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:24:36.000000 SrbAI-0.0.5/src/srbai/JezickiModeli/FastText/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 07:22:53.000000 SrbAI-0.0.5/src/srbai/JezickiModeli/FastText/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-16 07:22:53.000000 SrbAI-0.0.5/src/srbai/JezickiModeli/FastText/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-16 07:22:53.000000 SrbAI-0.0.5/src/srbai/JezickiModeli/FastText/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-16 07:22:53.000000 SrbAI-0.0.5/src/srbai/JezickiModeli/FastText/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-16 07:22:53.000000 SrbAI-0.0.5/src/srbai/JezickiModeli/FastText/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-04-16 07:22:53.000000 SrbAI-0.0.5/src/srbai/JezickiModeli/FastText/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-16 07:22:53.000000 SrbAI-0.0.5/src/srbai/JezickiModeli/FastText/similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-04-16 07:22:53.000000 SrbAI-0.0.5/src/srbai/JezickiModeli/FastText/text_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 07:22:53.000000 SrbAI-0.0.5/src/srbai/JezickiModeli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:24:36.000000 SrbAI-0.0.5/src/srbai/Klasifikatori/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 07:22:53.000000 SrbAI-0.0.5/src/srbai/Klasifikatori/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:24:36.000000 SrbAI-0.0.5/src/srbai/NER/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-16 07:22:53.000000 SrbAI-0.0.5/src/srbai/NER/NER_classla.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 07:22:53.000000 SrbAI-0.0.5/src/srbai/NER/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:24:36.000000 SrbAI-0.0.5/src/srbai/SintaktickiOperatori/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-16 07:22:53.000000 SrbAI-0.0.5/src/srbai/SintaktickiOperatori/POS_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 07:22:53.000000 SrbAI-0.0.5/src/srbai/SintaktickiOperatori/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-16 07:22:53.000000 SrbAI-0.0.5/src/srbai/SintaktickiOperatori/spellcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-04-16 07:22:53.000000 SrbAI-0.0.5/src/srbai/SintaktickiOperatori/stemmer_nm.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 07:22:53.000000 SrbAI-0.0.5/src/srbai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-16 07:22:53.000000 SrbAI-0.0.5/src/srbai/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:28.000000 SrbAI-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-16 16:23:38.000000 SrbAI-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-04-16 16:25:28.000000 SrbAI-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-16 16:23:38.000000 SrbAI-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-16 16:23:38.000000 SrbAI-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 16:25:28.000000 SrbAI-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-16 16:23:38.000000 SrbAI-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:28.000000 SrbAI-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:28.000000 SrbAI-0.0.6/src/SrbAI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-04-16 16:25:28.000000 SrbAI-0.0.6/src/SrbAI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-16 16:25:28.000000 SrbAI-0.0.6/src/SrbAI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 16:25:28.000000 SrbAI-0.0.6/src/SrbAI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-16 16:25:28.000000 SrbAI-0.0.6/src/SrbAI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 16:25:28.000000 SrbAI-0.0.6/src/SrbAI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:28.000000 SrbAI-0.0.6/src/srbai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:28.000000 SrbAI-0.0.6/src/srbai/Alati/
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-04-16 16:23:38.000000 SrbAI-0.0.6/src/srbai/Alati/Transliterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:23:38.000000 SrbAI-0.0.6/src/srbai/Alati/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:28.000000 SrbAI-0.0.6/src/srbai/Glas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:23:38.000000 SrbAI-0.0.6/src/srbai/Glas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:28.000000 SrbAI-0.0.6/src/srbai/JezickiModeli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:28.000000 SrbAI-0.0.6/src/srbai/JezickiModeli/FastText/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:23:38.000000 SrbAI-0.0.6/src/srbai/JezickiModeli/FastText/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-16 16:23:38.000000 SrbAI-0.0.6/src/srbai/JezickiModeli/FastText/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-16 16:23:38.000000 SrbAI-0.0.6/src/srbai/JezickiModeli/FastText/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-16 16:23:38.000000 SrbAI-0.0.6/src/srbai/JezickiModeli/FastText/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-16 16:23:38.000000 SrbAI-0.0.6/src/srbai/JezickiModeli/FastText/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-04-16 16:23:38.000000 SrbAI-0.0.6/src/srbai/JezickiModeli/FastText/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-16 16:23:38.000000 SrbAI-0.0.6/src/srbai/JezickiModeli/FastText/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-04-16 16:23:38.000000 SrbAI-0.0.6/src/srbai/JezickiModeli/FastText/text_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:23:38.000000 SrbAI-0.0.6/src/srbai/JezickiModeli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:28.000000 SrbAI-0.0.6/src/srbai/Klasifikatori/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:23:38.000000 SrbAI-0.0.6/src/srbai/Klasifikatori/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:28.000000 SrbAI-0.0.6/src/srbai/NER/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-16 16:23:38.000000 SrbAI-0.0.6/src/srbai/NER/NER_classla.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:23:38.000000 SrbAI-0.0.6/src/srbai/NER/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:28.000000 SrbAI-0.0.6/src/srbai/SintaktickiOperatori/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-16 16:23:38.000000 SrbAI-0.0.6/src/srbai/SintaktickiOperatori/POS_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:23:38.000000 SrbAI-0.0.6/src/srbai/SintaktickiOperatori/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-16 16:23:38.000000 SrbAI-0.0.6/src/srbai/SintaktickiOperatori/spellcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-04-16 16:23:38.000000 SrbAI-0.0.6/src/srbai/SintaktickiOperatori/stemmer_nm.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:23:38.000000 SrbAI-0.0.6/src/srbai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-16 16:23:38.000000 SrbAI-0.0.6/src/srbai/test.py
```

### Comparing `SrbAI-0.0.5/LICENSE` & `SrbAI-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.5/PKG-INFO` & `SrbAI-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: SrbAI
-Version: 0.0.5
+Version: 0.0.6
 Summary: Library for processing serbian language
 Home-page: https://github.com/Serbian-AI-Society/SrbAI
 Author: Serbian AI Society
 Author-email: nikola.milosevic86@gmail.com
 Project-URL: Bug Tracker, https://github.com/Serbian-AI-Society/SrbAI/issues
 Project-URL: Road Map, https://github.com/Serbian-AI-Society/SrbAI/projects/1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6.15
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 SrbAI - Python biblioteka za procesiranje srpskog jezika
 ========================================================
 
 SrbAI je projekat prikupljanja algoritama i modela za procesiranje srpskog jezika u jedinstvenu Python biblioteku. Biblioteka treba da sadrži kako osnovne metode za procesiranje srpskog, poput stemmera, prepoznavanje vrsta reči (part-of-speech tagging), negacija, do naprednijih funkcionalnosti, poput prepoznavanje imenovanih entiteta (named entity tagging), klasifikacije, itd. Biblioteka jednostavno može da se proširi novim metodima, tako da je ideja da se veći broj studenata, doktoranada i drugih ljudi koji rade i su zainteresovani za razvoj srpskog procesiranja jezika uključe u razvoj projekta.
```

### Comparing `SrbAI-0.0.5/README.md` & `SrbAI-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.5/setup.py` & `SrbAI-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SrbAI",
-    version="0.0.5",
+    version="0.0.6",
     author="Serbian AI Society",
     author_email="nikola.milosevic86@gmail.com",
     description="Library for processing serbian language",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Serbian-AI-Society/SrbAI",
     project_urls={
@@ -27,9 +27,9 @@
         "torch>=1.10.2",
         "classla==1.1.0",
         "nlu"
 
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.6.15",
+    python_requires=">=3.7",
 )
```

### Comparing `SrbAI-0.0.5/src/SrbAI.egg-info/PKG-INFO` & `SrbAI-0.0.6/src/SrbAI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: SrbAI
-Version: 0.0.5
+Version: 0.0.6
 Summary: Library for processing serbian language
 Home-page: https://github.com/Serbian-AI-Society/SrbAI
 Author: Serbian AI Society
 Author-email: nikola.milosevic86@gmail.com
 Project-URL: Bug Tracker, https://github.com/Serbian-AI-Society/SrbAI/issues
 Project-URL: Road Map, https://github.com/Serbian-AI-Society/SrbAI/projects/1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6.15
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 SrbAI - Python biblioteka za procesiranje srpskog jezika
 ========================================================
 
 SrbAI je projekat prikupljanja algoritama i modela za procesiranje srpskog jezika u jedinstvenu Python biblioteku. Biblioteka treba da sadrži kako osnovne metode za procesiranje srpskog, poput stemmera, prepoznavanje vrsta reči (part-of-speech tagging), negacija, do naprednijih funkcionalnosti, poput prepoznavanje imenovanih entiteta (named entity tagging), klasifikacije, itd. Biblioteka jednostavno može da se proširi novim metodima, tako da je ideja da se veći broj studenata, doktoranada i drugih ljudi koji rade i su zainteresovani za razvoj srpskog procesiranja jezika uključe u razvoj projekta.
```

### Comparing `SrbAI-0.0.5/src/SrbAI.egg-info/SOURCES.txt` & `SrbAI-0.0.6/src/SrbAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.5/src/srbai/Alati/Transliterator.py` & `SrbAI-0.0.6/src/srbai/Alati/Transliterator.py`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.5/src/srbai/JezickiModeli/FastText/__main__.py` & `SrbAI-0.0.6/src/srbai/JezickiModeli/FastText/__main__.py`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.5/src/srbai/JezickiModeli/FastText/embedding.py` & `SrbAI-0.0.6/src/srbai/JezickiModeli/FastText/embedding.py`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.5/src/srbai/JezickiModeli/FastText/globals.py` & `SrbAI-0.0.6/src/srbai/JezickiModeli/FastText/globals.py`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.5/src/srbai/JezickiModeli/FastText/io_utils.py` & `SrbAI-0.0.6/src/srbai/JezickiModeli/FastText/io_utils.py`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.5/src/srbai/JezickiModeli/FastText/model.py` & `SrbAI-0.0.6/src/srbai/JezickiModeli/FastText/model.py`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.5/src/srbai/JezickiModeli/FastText/similarity.py` & `SrbAI-0.0.6/src/srbai/JezickiModeli/FastText/similarity.py`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.5/src/srbai/JezickiModeli/FastText/text_preprocessing.py` & `SrbAI-0.0.6/src/srbai/JezickiModeli/FastText/text_preprocessing.py`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.5/src/srbai/SintaktickiOperatori/POS_tagger.py` & `SrbAI-0.0.6/src/srbai/SintaktickiOperatori/POS_tagger.py`

 * *Files identical despite different names*

### Comparing `SrbAI-0.0.5/src/srbai/SintaktickiOperatori/spellcheck.py` & `SrbAI-0.0.6/src/srbai/SintaktickiOperatori/spellcheck.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,18 @@
             new_path = ""
             for p in path:
                 if i<path_len-2:
                     new_path = new_path + p + os.path.sep
                     i = i + 1
             if dictionary == 'sr-latin':
                 dictionary = new_path + os.path.sep+"Resursi"+os.path.sep+"Recnici"+os.path.sep+ "Serbian (Latin).dic"
+                dictionary = dictionary.replace(os.path.sep+os.path.sep,os.path.sep)
             if dictionary == 'sr-cirilic':
                 dictionary = new_path + "/Resursi/Recnici/Serbian (Cyrilic).dic"
+                dictionary = dictionary.replace(os.path.sep + os.path.sep, os.path.sep)
 
         self.trie = {}
         self.max_cost = 2
         self.load_dictionary(dictionary)
 
 
     def load_dictionary(self, dictionary):
```

### Comparing `SrbAI-0.0.5/src/srbai/SintaktickiOperatori/stemmer_nm.py` & `SrbAI-0.0.6/src/srbai/SintaktickiOperatori/stemmer_nm.py`

 * *Files identical despite different names*

