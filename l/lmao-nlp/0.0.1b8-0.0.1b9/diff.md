# Comparing `tmp/lmao-nlp-0.0.1b8.tar.gz` & `tmp/lmao-nlp-0.0.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmao-nlp-0.0.1b8.tar", last modified: Sun Apr 16 15:46:09 2023, max compression
+gzip compressed data, was "lmao-nlp-0.0.1b9.tar", last modified: Sun Apr 16 15:54:31 2023, max compression
```

## Comparing `lmao-nlp-0.0.1b8.tar` & `lmao-nlp-0.0.1b9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:46:09.361138 lmao-nlp-0.0.1b8/
--rw-r--r--   0 johnnygreco   (501) staff       (20)    11357 2023-04-02 19:11:18.000000 lmao-nlp-0.0.1b8/LICENSE
--rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-16 15:46:09.360967 lmao-nlp-0.0.1b8/PKG-INFO
--rw-r--r--   0 johnnygreco   (501) staff       (20)     4307 2023-04-16 15:45:41.000000 lmao-nlp-0.0.1b8/README.md
--rw-r--r--   0 johnnygreco   (501) staff       (20)      764 2023-04-02 17:52:45.000000 lmao-nlp-0.0.1b8/pyproject.toml
--rw-r--r--   0 johnnygreco   (501) staff       (20)       38 2023-04-16 15:46:09.361179 lmao-nlp-0.0.1b8/setup.cfg
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1274 2023-04-16 15:46:05.000000 lmao-nlp-0.0.1b8/setup.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:46:09.353820 lmao-nlp-0.0.1b8/src/
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:46:09.354841 lmao-nlp-0.0.1b8/src/lmao/
--rw-r--r--   0 johnnygreco   (501) staff       (20)      208 2023-04-16 15:46:05.000000 lmao-nlp-0.0.1b8/src/lmao/__init__.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:46:09.355454 lmao-nlp-0.0.1b8/src/lmao/adapters/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       94 2023-04-16 15:36:03.000000 lmao-nlp-0.0.1b8/src/lmao/adapters/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1095 2023-04-16 15:21:34.000000 lmao-nlp-0.0.1b8/src/lmao/adapters/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1573 2023-04-14 14:29:05.000000 lmao-nlp-0.0.1b8/src/lmao/adapters/chatbot.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     5360 2023-04-16 15:28:06.000000 lmao-nlp-0.0.1b8/src/lmao/adapters/classification.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2166 2023-04-16 15:33:44.000000 lmao-nlp-0.0.1b8/src/lmao/adapters/fermi.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2935 2023-04-16 15:38:10.000000 lmao-nlp-0.0.1b8/src/lmao/factory.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:46:09.355882 lmao-nlp-0.0.1b8/src/lmao/lm/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       38 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b8/src/lmao/lm/__init__.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:46:09.357167 lmao-nlp-0.0.1b8/src/lmao/lm/clients/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       89 2023-04-16 15:10:02.000000 lmao-nlp-0.0.1b8/src/lmao/lm/clients/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2101 2023-04-16 15:14:43.000000 lmao-nlp-0.0.1b8/src/lmao/lm/clients/anthropic.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     5157 2023-04-13 18:52:54.000000 lmao-nlp-0.0.1b8/src/lmao/lm/clients/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1176 2023-04-16 15:28:44.000000 lmao-nlp-0.0.1b8/src/lmao/lm/clients/cohere.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2626 2023-04-13 20:15:49.000000 lmao-nlp-0.0.1b8/src/lmao/lm/clients/openai.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:46:09.358220 lmao-nlp-0.0.1b8/src/lmao/lm/schemas/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       89 2023-04-16 15:04:41.000000 lmao-nlp-0.0.1b8/src/lmao/lm/schemas/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1145 2023-04-16 15:15:01.000000 lmao-nlp-0.0.1b8/src/lmao/lm/schemas/anthropic.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      420 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b8/src/lmao/lm/schemas/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1061 2023-04-16 15:15:31.000000 lmao-nlp-0.0.1b8/src/lmao/lm/schemas/cohere.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2713 2023-04-16 14:59:50.000000 lmao-nlp-0.0.1b8/src/lmao/lm/schemas/openai.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1974 2023-04-13 20:12:50.000000 lmao-nlp-0.0.1b8/src/lmao/lm/utils.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:46:09.358438 lmao-nlp-0.0.1b8/src/lmao/orchestrators/
--rw-r--r--   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:32:08.000000 lmao-nlp-0.0.1b8/src/lmao/orchestrators/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:32:03.000000 lmao-nlp-0.0.1b8/src/lmao/orchestrators/base.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:46:09.359040 lmao-nlp-0.0.1b8/src/lmao/prompters/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       71 2023-04-14 19:07:04.000000 lmao-nlp-0.0.1b8/src/lmao/prompters/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      496 2023-04-14 19:07:04.000000 lmao-nlp-0.0.1b8/src/lmao/prompters/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1881 2023-04-16 15:22:27.000000 lmao-nlp-0.0.1b8/src/lmao/prompters/classification.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      756 2023-04-14 19:45:56.000000 lmao-nlp-0.0.1b8/src/lmao/prompters/fermi.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:46:09.360095 lmao-nlp-0.0.1b8/src/lmao/tasks/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       94 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b8/src/lmao/tasks/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      852 2023-04-16 15:38:11.000000 lmao-nlp-0.0.1b8/src/lmao/tasks/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      786 2023-04-14 19:04:53.000000 lmao-nlp-0.0.1b8/src/lmao/tasks/chatbot.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1234 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b8/src/lmao/tasks/classification.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      601 2023-04-14 19:41:35.000000 lmao-nlp-0.0.1b8/src/lmao/tasks/fermi.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:46:09.360776 lmao-nlp-0.0.1b8/src/lmao_nlp.egg-info/
--rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-16 15:46:09.000000 lmao-nlp-0.0.1b8/src/lmao_nlp.egg-info/PKG-INFO
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1082 2023-04-16 15:46:09.000000 lmao-nlp-0.0.1b8/src/lmao_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 johnnygreco   (501) staff       (20)        1 2023-04-16 15:46:09.000000 lmao-nlp-0.0.1b8/src/lmao_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 johnnygreco   (501) staff       (20)      288 2023-04-16 15:46:09.000000 lmao-nlp-0.0.1b8/src/lmao_nlp.egg-info/requires.txt
--rw-r--r--   0 johnnygreco   (501) staff       (20)        5 2023-04-16 15:46:09.000000 lmao-nlp-0.0.1b8/src/lmao_nlp.egg-info/top_level.txt
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:54:31.080398 lmao-nlp-0.0.1b9/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)    11357 2023-04-02 19:11:18.000000 lmao-nlp-0.0.1b9/LICENSE
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-16 15:54:31.080239 lmao-nlp-0.0.1b9/PKG-INFO
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     4299 2023-04-16 15:48:01.000000 lmao-nlp-0.0.1b9/README.md
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      764 2023-04-02 17:52:45.000000 lmao-nlp-0.0.1b9/pyproject.toml
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       38 2023-04-16 15:54:31.080451 lmao-nlp-0.0.1b9/setup.cfg
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1274 2023-04-16 15:54:27.000000 lmao-nlp-0.0.1b9/setup.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:54:31.071094 lmao-nlp-0.0.1b9/src/
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:54:31.072250 lmao-nlp-0.0.1b9/src/lmao/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      208 2023-04-16 15:54:27.000000 lmao-nlp-0.0.1b9/src/lmao/__init__.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:54:31.073316 lmao-nlp-0.0.1b9/src/lmao/adapters/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       94 2023-04-16 15:36:03.000000 lmao-nlp-0.0.1b9/src/lmao/adapters/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1095 2023-04-16 15:21:34.000000 lmao-nlp-0.0.1b9/src/lmao/adapters/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1573 2023-04-14 14:29:05.000000 lmao-nlp-0.0.1b9/src/lmao/adapters/chatbot.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     5360 2023-04-16 15:28:06.000000 lmao-nlp-0.0.1b9/src/lmao/adapters/classification.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2166 2023-04-16 15:33:44.000000 lmao-nlp-0.0.1b9/src/lmao/adapters/fermi.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2935 2023-04-16 15:38:10.000000 lmao-nlp-0.0.1b9/src/lmao/factory.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:54:31.073871 lmao-nlp-0.0.1b9/src/lmao/lm/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       38 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b9/src/lmao/lm/__init__.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:54:31.075336 lmao-nlp-0.0.1b9/src/lmao/lm/clients/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       89 2023-04-16 15:10:02.000000 lmao-nlp-0.0.1b9/src/lmao/lm/clients/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2101 2023-04-16 15:14:43.000000 lmao-nlp-0.0.1b9/src/lmao/lm/clients/anthropic.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     5157 2023-04-13 18:52:54.000000 lmao-nlp-0.0.1b9/src/lmao/lm/clients/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1176 2023-04-16 15:28:44.000000 lmao-nlp-0.0.1b9/src/lmao/lm/clients/cohere.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2626 2023-04-13 20:15:49.000000 lmao-nlp-0.0.1b9/src/lmao/lm/clients/openai.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:54:31.076534 lmao-nlp-0.0.1b9/src/lmao/lm/schemas/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       89 2023-04-16 15:04:41.000000 lmao-nlp-0.0.1b9/src/lmao/lm/schemas/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1145 2023-04-16 15:15:01.000000 lmao-nlp-0.0.1b9/src/lmao/lm/schemas/anthropic.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      420 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b9/src/lmao/lm/schemas/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1061 2023-04-16 15:15:31.000000 lmao-nlp-0.0.1b9/src/lmao/lm/schemas/cohere.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2713 2023-04-16 14:59:50.000000 lmao-nlp-0.0.1b9/src/lmao/lm/schemas/openai.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1974 2023-04-13 20:12:50.000000 lmao-nlp-0.0.1b9/src/lmao/lm/utils.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:54:31.076887 lmao-nlp-0.0.1b9/src/lmao/orchestrators/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:32:08.000000 lmao-nlp-0.0.1b9/src/lmao/orchestrators/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:32:03.000000 lmao-nlp-0.0.1b9/src/lmao/orchestrators/base.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:54:31.077668 lmao-nlp-0.0.1b9/src/lmao/prompters/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       71 2023-04-14 19:07:04.000000 lmao-nlp-0.0.1b9/src/lmao/prompters/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      496 2023-04-14 19:07:04.000000 lmao-nlp-0.0.1b9/src/lmao/prompters/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1881 2023-04-16 15:22:27.000000 lmao-nlp-0.0.1b9/src/lmao/prompters/classification.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      756 2023-04-14 19:45:56.000000 lmao-nlp-0.0.1b9/src/lmao/prompters/fermi.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:54:31.079030 lmao-nlp-0.0.1b9/src/lmao/tasks/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       94 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b9/src/lmao/tasks/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      852 2023-04-16 15:38:11.000000 lmao-nlp-0.0.1b9/src/lmao/tasks/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      786 2023-04-14 19:04:53.000000 lmao-nlp-0.0.1b9/src/lmao/tasks/chatbot.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1234 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b9/src/lmao/tasks/classification.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      601 2023-04-14 19:41:35.000000 lmao-nlp-0.0.1b9/src/lmao/tasks/fermi.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:54:31.080043 lmao-nlp-0.0.1b9/src/lmao_nlp.egg-info/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-16 15:54:31.000000 lmao-nlp-0.0.1b9/src/lmao_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1082 2023-04-16 15:54:31.000000 lmao-nlp-0.0.1b9/src/lmao_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        1 2023-04-16 15:54:31.000000 lmao-nlp-0.0.1b9/src/lmao_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      288 2023-04-16 15:54:31.000000 lmao-nlp-0.0.1b9/src/lmao_nlp.egg-info/requires.txt
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        5 2023-04-16 15:54:31.000000 lmao-nlp-0.0.1b9/src/lmao_nlp.egg-info/top_level.txt
```

### Comparing `lmao-nlp-0.0.1b8/LICENSE` & `lmao-nlp-0.0.1b9/LICENSE`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b8/PKG-INFO` & `lmao-nlp-0.0.1b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmao-nlp
-Version: 0.0.1b8
+Version: 0.0.1b9
 Summary: LMAO: Language Model Adapters and Orchestrators
 Home-page: https://github.com/johnnygreco/lmao
 Author: Johnny Greco
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `lmao-nlp-0.0.1b8/README.md` & `lmao-nlp-0.0.1b9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # 🙊 LMAO: **L**anguage **M**odel **A**dapters and **O**rchestrators
 
 <img src="assets/icon.png" height="210" align="right" />
 
-> The data scientist's toolkit for leveraging the power of large LMs for downstream NLP tasks
+> The data scientist's toolkit for adapting large LMs to solve a diverse set of tasks
 
 <br>
 
 `lmao` is an open-source library for integrating large language models (LLMs) from providers like [OpenAI](https://platform.openai.com/docs/introduction) and [Anthropic](https://console.anthropic.com/docs/api) into your NLP workflows. For example, it can be used to pre-annotate text datasets using zero- or few-shot learning with Claude or GPT-4. LMAO is in the (very) early stages of development. New features will be added with high cadence and documentation is coming soon.
 
 ## Installation
 The package is available on PyPI and can be installed with pip:
```

### Comparing `lmao-nlp-0.0.1b8/pyproject.toml` & `lmao-nlp-0.0.1b9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b8/setup.py` & `lmao-nlp-0.0.1b9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version__ = "0.0.1-beta.8"
+__version__ = "0.0.1-beta.9"
 
 install_requires = [
     "pydantic>=1.10.7",
     "requests>=2.28.2",
     "tiktoken>=0.3.3",
 ]
```

### Comparing `lmao-nlp-0.0.1b8/src/lmao/adapters/base.py` & `lmao-nlp-0.0.1b9/src/lmao/adapters/base.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b8/src/lmao/adapters/chatbot.py` & `lmao-nlp-0.0.1b9/src/lmao/adapters/chatbot.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b8/src/lmao/adapters/classification.py` & `lmao-nlp-0.0.1b9/src/lmao/adapters/classification.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b8/src/lmao/adapters/fermi.py` & `lmao-nlp-0.0.1b9/src/lmao/adapters/fermi.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b8/src/lmao/factory.py` & `lmao-nlp-0.0.1b9/src/lmao/factory.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b8/src/lmao/lm/clients/anthropic.py` & `lmao-nlp-0.0.1b9/src/lmao/lm/clients/anthropic.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b8/src/lmao/lm/clients/base.py` & `lmao-nlp-0.0.1b9/src/lmao/lm/clients/base.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b8/src/lmao/lm/clients/cohere.py` & `lmao-nlp-0.0.1b9/src/lmao/lm/clients/cohere.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b8/src/lmao/lm/clients/openai.py` & `lmao-nlp-0.0.1b9/src/lmao/lm/clients/openai.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b8/src/lmao/lm/schemas/anthropic.py` & `lmao-nlp-0.0.1b9/src/lmao/lm/schemas/anthropic.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b8/src/lmao/lm/schemas/cohere.py` & `lmao-nlp-0.0.1b9/src/lmao/lm/schemas/cohere.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b8/src/lmao/lm/schemas/openai.py` & `lmao-nlp-0.0.1b9/src/lmao/lm/schemas/openai.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b8/src/lmao/lm/utils.py` & `lmao-nlp-0.0.1b9/src/lmao/lm/utils.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b8/src/lmao/prompters/classification.py` & `lmao-nlp-0.0.1b9/src/lmao/prompters/classification.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b8/src/lmao/prompters/fermi.py` & `lmao-nlp-0.0.1b9/src/lmao/prompters/fermi.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b8/src/lmao/tasks/base.py` & `lmao-nlp-0.0.1b9/src/lmao/tasks/base.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b8/src/lmao/tasks/chatbot.py` & `lmao-nlp-0.0.1b9/src/lmao/tasks/chatbot.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b8/src/lmao/tasks/classification.py` & `lmao-nlp-0.0.1b9/src/lmao/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b8/src/lmao/tasks/fermi.py` & `lmao-nlp-0.0.1b9/src/lmao/tasks/fermi.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b8/src/lmao_nlp.egg-info/PKG-INFO` & `lmao-nlp-0.0.1b9/src/lmao_nlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmao-nlp
-Version: 0.0.1b8
+Version: 0.0.1b9
 Summary: LMAO: Language Model Adapters and Orchestrators
 Home-page: https://github.com/johnnygreco/lmao
 Author: Johnny Greco
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `lmao-nlp-0.0.1b8/src/lmao_nlp.egg-info/SOURCES.txt` & `lmao-nlp-0.0.1b9/src/lmao_nlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

