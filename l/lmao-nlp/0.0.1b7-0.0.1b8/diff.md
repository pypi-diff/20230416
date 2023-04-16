# Comparing `tmp/lmao-nlp-0.0.1b7.tar.gz` & `tmp/lmao-nlp-0.0.1b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmao-nlp-0.0.1b7.tar", last modified: Fri Apr 14 20:03:00 2023, max compression
+gzip compressed data, was "lmao-nlp-0.0.1b8.tar", last modified: Sun Apr 16 15:46:09 2023, max compression
```

## Comparing `lmao-nlp-0.0.1b7.tar` & `lmao-nlp-0.0.1b8.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 20:03:00.531409 lmao-nlp-0.0.1b7/
--rw-r--r--   0 johnnygreco   (501) staff       (20)    11357 2023-04-02 19:11:18.000000 lmao-nlp-0.0.1b7/LICENSE
--rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-14 20:03:00.531253 lmao-nlp-0.0.1b7/PKG-INFO
--rw-r--r--   0 johnnygreco   (501) staff       (20)     4116 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b7/README.md
--rw-r--r--   0 johnnygreco   (501) staff       (20)      764 2023-04-02 17:52:45.000000 lmao-nlp-0.0.1b7/pyproject.toml
--rw-r--r--   0 johnnygreco   (501) staff       (20)       38 2023-04-14 20:03:00.531461 lmao-nlp-0.0.1b7/setup.cfg
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1275 2023-04-14 20:02:57.000000 lmao-nlp-0.0.1b7/setup.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 20:03:00.526239 lmao-nlp-0.0.1b7/src/
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 20:03:00.527133 lmao-nlp-0.0.1b7/src/lmao/
--rw-r--r--   0 johnnygreco   (501) staff       (20)      203 2023-04-14 20:02:57.000000 lmao-nlp-0.0.1b7/src/lmao/__init__.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 20:03:00.527754 lmao-nlp-0.0.1b7/src/lmao/adapters/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       94 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b7/src/lmao/adapters/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1100 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b7/src/lmao/adapters/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1573 2023-04-14 14:29:05.000000 lmao-nlp-0.0.1b7/src/lmao/adapters/chatbot.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     3939 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b7/src/lmao/adapters/classification.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1533 2023-04-14 19:44:53.000000 lmao-nlp-0.0.1b7/src/lmao/adapters/fermi.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2673 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b7/src/lmao/factory.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 20:03:00.527975 lmao-nlp-0.0.1b7/src/lmao/lm/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       38 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b7/src/lmao/lm/__init__.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 20:03:00.528494 lmao-nlp-0.0.1b7/src/lmao/lm/clients/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       67 2023-04-11 21:11:07.000000 lmao-nlp-0.0.1b7/src/lmao/lm/clients/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2101 2023-04-13 18:36:40.000000 lmao-nlp-0.0.1b7/src/lmao/lm/clients/anthropic.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     5157 2023-04-13 18:52:54.000000 lmao-nlp-0.0.1b7/src/lmao/lm/clients/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2626 2023-04-13 20:15:49.000000 lmao-nlp-0.0.1b7/src/lmao/lm/clients/openai.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 20:03:00.528959 lmao-nlp-0.0.1b7/src/lmao/lm/schemas/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       47 2023-04-11 21:04:00.000000 lmao-nlp-0.0.1b7/src/lmao/lm/schemas/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1145 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b7/src/lmao/lm/schemas/anthropic.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      420 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b7/src/lmao/lm/schemas/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2718 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b7/src/lmao/lm/schemas/openai.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1974 2023-04-13 20:12:50.000000 lmao-nlp-0.0.1b7/src/lmao/lm/utils.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 20:03:00.529188 lmao-nlp-0.0.1b7/src/lmao/orchestrators/
--rw-r--r--   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:32:08.000000 lmao-nlp-0.0.1b7/src/lmao/orchestrators/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:32:03.000000 lmao-nlp-0.0.1b7/src/lmao/orchestrators/base.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 20:03:00.529660 lmao-nlp-0.0.1b7/src/lmao/prompters/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       71 2023-04-14 19:07:04.000000 lmao-nlp-0.0.1b7/src/lmao/prompters/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      496 2023-04-14 19:07:04.000000 lmao-nlp-0.0.1b7/src/lmao/prompters/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1852 2023-04-14 19:31:31.000000 lmao-nlp-0.0.1b7/src/lmao/prompters/classification.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      756 2023-04-14 19:45:56.000000 lmao-nlp-0.0.1b7/src/lmao/prompters/fermi.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 20:03:00.530480 lmao-nlp-0.0.1b7/src/lmao/tasks/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       94 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b7/src/lmao/tasks/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      836 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b7/src/lmao/tasks/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      786 2023-04-14 19:04:53.000000 lmao-nlp-0.0.1b7/src/lmao/tasks/chatbot.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1234 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b7/src/lmao/tasks/classification.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      601 2023-04-14 19:41:35.000000 lmao-nlp-0.0.1b7/src/lmao/tasks/fermi.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 20:03:00.531089 lmao-nlp-0.0.1b7/src/lmao_nlp.egg-info/
--rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-14 20:03:00.000000 lmao-nlp-0.0.1b7/src/lmao_nlp.egg-info/PKG-INFO
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1022 2023-04-14 20:03:00.000000 lmao-nlp-0.0.1b7/src/lmao_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 johnnygreco   (501) staff       (20)        1 2023-04-14 20:03:00.000000 lmao-nlp-0.0.1b7/src/lmao_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 johnnygreco   (501) staff       (20)      288 2023-04-14 20:03:00.000000 lmao-nlp-0.0.1b7/src/lmao_nlp.egg-info/requires.txt
--rw-r--r--   0 johnnygreco   (501) staff       (20)        5 2023-04-14 20:03:00.000000 lmao-nlp-0.0.1b7/src/lmao_nlp.egg-info/top_level.txt
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:46:09.361138 lmao-nlp-0.0.1b8/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)    11357 2023-04-02 19:11:18.000000 lmao-nlp-0.0.1b8/LICENSE
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-16 15:46:09.360967 lmao-nlp-0.0.1b8/PKG-INFO
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     4307 2023-04-16 15:45:41.000000 lmao-nlp-0.0.1b8/README.md
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      764 2023-04-02 17:52:45.000000 lmao-nlp-0.0.1b8/pyproject.toml
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       38 2023-04-16 15:46:09.361179 lmao-nlp-0.0.1b8/setup.cfg
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1274 2023-04-16 15:46:05.000000 lmao-nlp-0.0.1b8/setup.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:46:09.353820 lmao-nlp-0.0.1b8/src/
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:46:09.354841 lmao-nlp-0.0.1b8/src/lmao/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      208 2023-04-16 15:46:05.000000 lmao-nlp-0.0.1b8/src/lmao/__init__.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:46:09.355454 lmao-nlp-0.0.1b8/src/lmao/adapters/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       94 2023-04-16 15:36:03.000000 lmao-nlp-0.0.1b8/src/lmao/adapters/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1095 2023-04-16 15:21:34.000000 lmao-nlp-0.0.1b8/src/lmao/adapters/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1573 2023-04-14 14:29:05.000000 lmao-nlp-0.0.1b8/src/lmao/adapters/chatbot.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     5360 2023-04-16 15:28:06.000000 lmao-nlp-0.0.1b8/src/lmao/adapters/classification.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2166 2023-04-16 15:33:44.000000 lmao-nlp-0.0.1b8/src/lmao/adapters/fermi.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2935 2023-04-16 15:38:10.000000 lmao-nlp-0.0.1b8/src/lmao/factory.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:46:09.355882 lmao-nlp-0.0.1b8/src/lmao/lm/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       38 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b8/src/lmao/lm/__init__.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:46:09.357167 lmao-nlp-0.0.1b8/src/lmao/lm/clients/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       89 2023-04-16 15:10:02.000000 lmao-nlp-0.0.1b8/src/lmao/lm/clients/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2101 2023-04-16 15:14:43.000000 lmao-nlp-0.0.1b8/src/lmao/lm/clients/anthropic.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     5157 2023-04-13 18:52:54.000000 lmao-nlp-0.0.1b8/src/lmao/lm/clients/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1176 2023-04-16 15:28:44.000000 lmao-nlp-0.0.1b8/src/lmao/lm/clients/cohere.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2626 2023-04-13 20:15:49.000000 lmao-nlp-0.0.1b8/src/lmao/lm/clients/openai.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:46:09.358220 lmao-nlp-0.0.1b8/src/lmao/lm/schemas/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       89 2023-04-16 15:04:41.000000 lmao-nlp-0.0.1b8/src/lmao/lm/schemas/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1145 2023-04-16 15:15:01.000000 lmao-nlp-0.0.1b8/src/lmao/lm/schemas/anthropic.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      420 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b8/src/lmao/lm/schemas/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1061 2023-04-16 15:15:31.000000 lmao-nlp-0.0.1b8/src/lmao/lm/schemas/cohere.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2713 2023-04-16 14:59:50.000000 lmao-nlp-0.0.1b8/src/lmao/lm/schemas/openai.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1974 2023-04-13 20:12:50.000000 lmao-nlp-0.0.1b8/src/lmao/lm/utils.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:46:09.358438 lmao-nlp-0.0.1b8/src/lmao/orchestrators/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:32:08.000000 lmao-nlp-0.0.1b8/src/lmao/orchestrators/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:32:03.000000 lmao-nlp-0.0.1b8/src/lmao/orchestrators/base.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:46:09.359040 lmao-nlp-0.0.1b8/src/lmao/prompters/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       71 2023-04-14 19:07:04.000000 lmao-nlp-0.0.1b8/src/lmao/prompters/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      496 2023-04-14 19:07:04.000000 lmao-nlp-0.0.1b8/src/lmao/prompters/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1881 2023-04-16 15:22:27.000000 lmao-nlp-0.0.1b8/src/lmao/prompters/classification.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      756 2023-04-14 19:45:56.000000 lmao-nlp-0.0.1b8/src/lmao/prompters/fermi.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:46:09.360095 lmao-nlp-0.0.1b8/src/lmao/tasks/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       94 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b8/src/lmao/tasks/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      852 2023-04-16 15:38:11.000000 lmao-nlp-0.0.1b8/src/lmao/tasks/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      786 2023-04-14 19:04:53.000000 lmao-nlp-0.0.1b8/src/lmao/tasks/chatbot.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1234 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b8/src/lmao/tasks/classification.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      601 2023-04-14 19:41:35.000000 lmao-nlp-0.0.1b8/src/lmao/tasks/fermi.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-16 15:46:09.360776 lmao-nlp-0.0.1b8/src/lmao_nlp.egg-info/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-16 15:46:09.000000 lmao-nlp-0.0.1b8/src/lmao_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1082 2023-04-16 15:46:09.000000 lmao-nlp-0.0.1b8/src/lmao_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        1 2023-04-16 15:46:09.000000 lmao-nlp-0.0.1b8/src/lmao_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      288 2023-04-16 15:46:09.000000 lmao-nlp-0.0.1b8/src/lmao_nlp.egg-info/requires.txt
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        5 2023-04-16 15:46:09.000000 lmao-nlp-0.0.1b8/src/lmao_nlp.egg-info/top_level.txt
```

### Comparing `lmao-nlp-0.0.1b7/LICENSE` & `lmao-nlp-0.0.1b8/LICENSE`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b7/PKG-INFO` & `lmao-nlp-0.0.1b8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmao-nlp
-Version: 0.0.1b7
+Version: 0.0.1b8
 Summary: LMAO: Language Model Adapters and Orchestrators
 Home-page: https://github.com/johnnygreco/lmao
 Author: Johnny Greco
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `lmao-nlp-0.0.1b7/README.md` & `lmao-nlp-0.0.1b8/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # 🙊 LMAO: **L**anguage **M**odel **A**dapters and **O**rchestrators
-> Leveraging the power of large LMs for downstream NLP tasks
 
-LMAO is an open-source library for integrating large language models (LLMs) from providers like [OpenAI](https://platform.openai.com/docs/introduction) and [Anthropic](https://console.anthropic.com/docs/api) into your NLP workflows. For example, it can be used to pre-annotate text datasets using zero- or few-shot learning with Claude or GPT-4. LMAO is in the (very) early stages of development. New features will be added with high cadence and documentation is coming soon.
+<img src="assets/icon.png" height="210" align="right" />
+
+> The data scientist's toolkit for leveraging the power of large LMs for downstream NLP tasks
+
+<br>
+
+`lmao` is an open-source library for integrating large language models (LLMs) from providers like [OpenAI](https://platform.openai.com/docs/introduction) and [Anthropic](https://console.anthropic.com/docs/api) into your NLP workflows. For example, it can be used to pre-annotate text datasets using zero- or few-shot learning with Claude or GPT-4. LMAO is in the (very) early stages of development. New features will be added with high cadence and documentation is coming soon.
 
 ## Installation
 The package is available on PyPI and can be installed with pip:
 ```bash
 pip install lmao-nlp
 ```
 > ⚠️ Don't forget the `-nlp` extension on the distribution name!
@@ -22,56 +27,61 @@
 
 If you want to install all the optional dependencies (e.g., to build the docs), use the `all` extra:
 
 ```bash
 pip install -e ".[all]"
 ```
 
-## LM Providers
-The plan is to add support for all major LM providers (both for external API-based models and locally run models). At this early stage of development, [OpenAI](https://platform.openai.com/docs/introduction) and [Anthropic](https://console.anthropic.com/docs/api) are the only supported providers. You'll need an activate API key from OpenAI and/or Anthropic to use the LMAO library.
+## LM Clients
+The plan is to add support for all major LM providers (both for external API-based models and locally run models). Currently, the following providers are supported:
 
+- [OpenAI](https://platform.openai.com/docs/introduction)
+- [Cohere](https://docs.cohere.ai/docs)
+- [Anthropic](https://console.anthropic.com/docs/api)
 
-## Quickstart
-
-### 😀 😐 😖 Perform sentiment analysis with ChatGPT
-```python
-from lmao import factory
+You'll need an activate API key from one or more of these providers to use `lmao`.
 
-# create a sentiment analysis task using an adapter for OpenAI's GPT-3.5-turbo model
-model = factory.create_task("sentiment_analysis", "openai")
-
-# predict sentiment of the given text
-result = model.predict("This LMAO package is awesome!")
-
-print(result.prediction)
-# output: 'positive'
-```
+## Quickstart
 
-### 🤖 Create a Claude chatbot
+### 🤖 Create a ChatGPT chatbot
 ```python
 from lmao import factory
 
-# create a chatbot using Anthropic's Claude under the hood
-chatbot = factory.create_chatbot("anthropic")
+# create a chatbot using OpenAI's ChatGPT under the hood
+chatbot = factory.create_chatbot("openai")
 
 response = chatbot.chat("Hello! Tell me a joke, please!")
 
 print(response.text)
-# output: Why was six afraid of seven? Because seven eight nine!
+# output: Why did the tomato turn red? Because it saw the salad dressing!
 
 # the chatbot object keeps track of the chat history
 response = chatbot.chat("Haha! Can you please explain why this is funny?")
 
 print(response.text)
-# output: Sure! This is a pun based joke. It plays on the homophones
-# 'seven' and 'ate', and 'nine'. When spoken aloud, "seven eight nine"
-# sounds like the phrase "seven ate nine". The joke implies that seven ate
-# (devoured) the number nine, which is why six (the previous number) would
-# be afraid of seven. It's a silly pun, but that's why some people find
-# that type of simple wordplay amusing.
+# output: This joke is funny because it plays on the idea of personification,
+# where the tomato is given human-like characteristics, such as being able to
+# see and react to its environment. It also sets up an expectation that there
+# is a serious reason for the tomato turning red, but the punchline delivers
+# a silly and unexpected twist, which makes it humorous. Finally, the wordplay
+# on "dressing" which sounds similar to "stressin'" adds to the comedic effect.
+```
+
+### 😀 😐 😖 Perform sentiment analysis with Cohere
+```python
+from lmao import factory
+
+# create a sentiment analysis task using an adapter for Cohere's command-xlarge-nightly
+model = factory.create_task("sentiment_analysis", "cohere")
+
+# predict sentiment of the given text
+result = model.predict("This LMAO package is awesome!")
+
+print(result.prediction)
+# output: 'positive'
 ```
 
 ### 🪐 Solve Fermi Problems with Claude!
 ```python
 from lmao import factory
 
 # create a Fermi Task task using an adapter for Anthropic's Claude
```

### Comparing `lmao-nlp-0.0.1b7/pyproject.toml` & `lmao-nlp-0.0.1b8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b7/setup.py` & `lmao-nlp-0.0.1b8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from setuptools import find_packages, setup
 
-__version__ = "0.0.1-beta.7"
+__version__ = "0.0.1-beta.8"
 
 install_requires = [
     "pydantic>=1.10.7",
     "requests>=2.28.2",
     "tiktoken>=0.3.3",
 ]
 
-
 extras_require = {
     "dev": [
         "pre-commit>=3.2.1",
         "pytest>=7.2.2",
         "responses>=0.23.1",
     ],
     "docs": [
```

### Comparing `lmao-nlp-0.0.1b7/src/lmao/adapters/base.py` & `lmao-nlp-0.0.1b8/src/lmao/adapters/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 
 from lmao.lm.clients.base import BaseClient, ChatHistory, ClientResponse
-from lmao.prompters.base import Prompter
+from lmao.prompters import Prompter
 
 __all__ = ["BaseAdapter", "BaseChatbotAdapter", "BaseTaskAdapter"]
 
 
 class BaseAdapter(ABC):
     def __init__(self, client: BaseClient, endpoint_method_name: str):
         self.client = client
```

### Comparing `lmao-nlp-0.0.1b7/src/lmao/adapters/chatbot.py` & `lmao-nlp-0.0.1b8/src/lmao/adapters/chatbot.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b7/src/lmao/adapters/classification.py` & `lmao-nlp-0.0.1b8/src/lmao/adapters/classification.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from typing import List, Optional
 
 from lmao.adapters.base import BaseTaskAdapter
 from lmao.lm.clients.anthropic import AnthropicClient
 from lmao.lm.clients.base import BaseClient, ClientResponse
+from lmao.lm.clients.cohere import CohereClient
 from lmao.lm.clients.openai import OpenAIClient
 from lmao.prompters.classification import ClassificationPrompter, SentimentAnalysisPrompter
 
 __all__ = [
     "AnthropicSentimentAnalysisAdapter",
     "AnthropicTextClassificationAdapter",
+    "CohereSentimentAnalysisAdapter",
+    "CohereTextClassificationAdapter",
     "OpenAISentimentAnalysisAdapter",
     "OpenAITextClassificationAdapter",
     "SentimentAnalysisAdapter",
     "TextClassificationAdapter",
 ]
 
 
@@ -65,14 +68,54 @@
             client=AnthropicClient(api_key),
             endpoint_method_name="complete",
             include_neutral=include_neutral,
             **kwargs,
         )
 
 
+class CohereClassificationMixin:
+    def postprocess_response(self, response: ClientResponse) -> ClientResponse:
+        if response.text is not None:
+            response.text = response.text.strip()
+        return response
+
+    def to_endpoint_kwargs(self, request) -> dict:
+        return {"prompt": request}
+
+
+class CohereTextClassificationAdapter(CohereClassificationMixin, TextClassificationAdapter):
+    def __init__(
+        self,
+        categories: List[str],
+        lowercase: bool = True,
+        api_key: Optional[str] = None,
+        api_version: str = "2022-12-06",
+        **kwargs
+    ):
+        super().__init__(
+            client=CohereClient(api_key, api_version=api_version),
+            endpoint_method_name="complete",
+            categories=categories,
+            lowercase=lowercase,
+            **kwargs,
+        )
+
+
+class CohereSentimentAnalysisAdapter(CohereClassificationMixin, SentimentAnalysisAdapter):
+    def __init__(
+        self, include_neutral: bool = True, api_key: Optional[str] = None, api_version: str = "2022-12-06", **kwargs
+    ):
+        super().__init__(
+            client=CohereClient(api_key, api_version=api_version),
+            endpoint_method_name="complete",
+            include_neutral=include_neutral,
+            **kwargs,
+        )
+
+
 class OpenAIClassificationMixin:
     def postprocess_response(self, response: ClientResponse) -> ClientResponse:
         if response.text is not None:
             response.text = response.text.strip()
         return response
 
     def to_endpoint_kwargs(self, request) -> dict:
```

### Comparing `lmao-nlp-0.0.1b7/src/lmao/adapters/fermi.py` & `lmao-nlp-0.0.1b8/src/lmao/adapters/fermi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from typing import Optional
 
 from lmao.adapters import BaseTaskAdapter
 from lmao.lm.clients import AnthropicClient, BaseClient, ClientResponse
+from lmao.lm.clients.cohere import CohereClient
 from lmao.lm.clients.openai import OpenAIClient
 from lmao.prompters import FermiProblemPrompter
 
-__all__ = ["FermiProblemAdapter", "AnthropicFermiProblemAdapter", "OpenAIFermiProblemAdapter"]
+__all__ = [
+    "FermiProblemAdapter",
+    "AnthropicFermiProblemAdapter",
+    "CohereFermiProblemAdapter",
+    "OpenAIFermiProblemAdapter",
+]
 
 
 class FermiProblemAdapter(BaseTaskAdapter):
     def __init__(self, client: BaseClient, endpoint_method_name: str):
         super().__init__(client, endpoint_method_name, prompter=FermiProblemPrompter())
 
 
@@ -19,14 +25,27 @@
 
     def postprocess_response(self, response: ClientResponse) -> ClientResponse:
         if response.text is not None:
             response.text = response.text.strip()
         return response
 
     def to_endpoint_kwargs(self, request) -> dict:
+        return {"prompt": request}
+
+
+class CohereFermiProblemAdapter(FermiProblemAdapter):
+    def __init__(self, api_key: Optional[str] = None, api_version: str = "2022-12-06"):
+        super().__init__(client=CohereClient(api_key, api_version=api_version), endpoint_method_name="complete")
+
+    def postprocess_response(self, response: ClientResponse) -> ClientResponse:
+        if response.text is not None:
+            response.text = response.text.strip()
+        return response
+
+    def to_endpoint_kwargs(self, request) -> dict:
         return {"prompt": request}
 
 
 class OpenAIFermiProblemAdapter(FermiProblemAdapter):
     def __init__(self, api_key: Optional[str] = None):
         super().__init__(client=OpenAIClient(api_key), endpoint_method_name="chat")
```

### Comparing `lmao-nlp-0.0.1b7/src/lmao/factory.py` & `lmao-nlp-0.0.1b8/src/lmao/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,37 +4,44 @@
 import lmao.lm.clients as clients
 import lmao.tasks as tasks
 
 __all__ = ["create_chatbot", "create_client", "create_task"]
 
 
 class ObjectMapping(NamedTuple):
-    name_to_client: dict = {"anthropic": clients.AnthropicClient, "openai": clients.OpenAIClient}
+    name_to_client: dict = {
+        "anthropic": clients.AnthropicClient,
+        "cohere": clients.CohereClient,
+        "openai": clients.OpenAIClient,
+    }
     name_to_history: dict = {"anthropic": clients.AnthropicChatHistory, "openai": clients.OpenAIChatHistory}
     name_to_task: dict = {
         "sentiment_analysis": tasks.TextClassification,
         "text_classification": tasks.TextClassification,
         "fermi_problem": tasks.FermiProblem,
         "chatbot": tasks.Chatbot,
     }
     task_to_adapter: dict = {
         "chatbot": {
             "anthropic": adapters.AnthropicChatbotAdapter,
             "openai": adapters.OpenAIChatbotAdapter,
         },
         "sentiment_analysis": {
             "anthropic": adapters.AnthropicSentimentAnalysisAdapter,
+            "cohere": adapters.CohereSentimentAnalysisAdapter,
             "openai": adapters.OpenAISentimentAnalysisAdapter,
         },
         "text_classification": {
             "anthropic": adapters.AnthropicTextClassificationAdapter,
+            "cohere": adapters.CohereTextClassificationAdapter,
             "openai": adapters.OpenAITextClassificationAdapter,
         },
         "fermi_problem": {
             "anthropic": adapters.AnthropicFermiProblemAdapter,
+            "cohere": adapters.CohereFermiProblemAdapter,
             "openai": adapters.OpenAIFermiProblemAdapter,
         },
     }
 
 
 _m = ObjectMapping()
 
@@ -57,12 +64,14 @@
     client_name: str, chat_history: bool = False, **kwargs
 ) -> Union[clients.BaseClient, Tuple[clients.BaseClient, clients.ChatHistory]]:
     max_length = kwargs.pop("max_length", 5)
     Client, History = _m.name_to_client[client_name], _m.name_to_history[client_name]
     return (Client(**kwargs), History(max_length=max_length)) if chat_history else Client(**kwargs)
 
 
-def create_task(task: str, client_name: str, **kwargs) -> Union[tasks.ModelProtocol, tasks.QAProtocol, tasks.Chatbot]:
+def create_task(
+    task: str, client_name: str, **kwargs
+) -> Union[tasks.ModelTaskProtocol, tasks.QATaskProtocol, tasks.Chatbot]:
     task, client_name = _validate_task_input(task, client_name)
     Task = _m.name_to_task[task]
     client_adapter = _m.task_to_adapter[task][client_name](**kwargs)
     return Task(client_adapter) if task != "chatbot" else create_chatbot(client_name, **kwargs)
```

### Comparing `lmao-nlp-0.0.1b7/src/lmao/lm/clients/anthropic.py` & `lmao-nlp-0.0.1b8/src/lmao/lm/clients/anthropic.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b7/src/lmao/lm/clients/base.py` & `lmao-nlp-0.0.1b8/src/lmao/lm/clients/base.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b7/src/lmao/lm/clients/openai.py` & `lmao-nlp-0.0.1b8/src/lmao/lm/clients/openai.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b7/src/lmao/lm/schemas/anthropic.py` & `lmao-nlp-0.0.1b8/src/lmao/lm/schemas/anthropic.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b7/src/lmao/lm/schemas/openai.py` & `lmao-nlp-0.0.1b8/src/lmao/lm/schemas/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from typing import Dict, List, Optional, Union
 
 from pydantic import Extra, Field, validator
 
-from lmao.lm.schemas.base import API_DEFAULTS, BaseSchema
+from lmao.lm.schemas import API_DEFAULTS, BaseSchema
 
 __all__ = ["OpenAIChatSchema", "OpenAICompleteSchema", "openai_model_regex"]
 
 
 model_versions = r"(?:3\.5-turbo|4)"
 date_label_pattern = r"(?:0[1-9]|1[012])(?:0[1-9]|[12][0-9]|3[01])$"
 openai_model_regex = dict(
```

### Comparing `lmao-nlp-0.0.1b7/src/lmao/lm/utils.py` & `lmao-nlp-0.0.1b8/src/lmao/lm/utils.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b7/src/lmao/prompters/classification.py` & `lmao-nlp-0.0.1b8/src/lmao/prompters/classification.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List
 
 from lmao.prompters.base import Prompter, build_prompt_template
 
-__all__ = ["ClassificationPrompter"]
+__all__ = ["ClassificationPrompter", "SentimentAnalysisPrompter"]
 
 
 class ClassificationPrompter(Prompter):
     task = "classification"
 
     template = build_prompt_template(
         intro=(
```

### Comparing `lmao-nlp-0.0.1b7/src/lmao/prompters/fermi.py` & `lmao-nlp-0.0.1b8/src/lmao/prompters/fermi.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b7/src/lmao/tasks/base.py` & `lmao-nlp-0.0.1b8/src/lmao/tasks/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 from typing import NamedTuple, Protocol, runtime_checkable
 
 from lmao.adapters.base import BaseAdapter
 from lmao.lm.clients.base import ClientResponse
 
-__all__ = ["task_errors", "ModelProtocol", "QAProtocol", "TaskResponse"]
+__all__ = ["task_errors", "ModelTaskProtocol", "QATaskProtocol", "TaskResponse"]
 
 
 class TaskErrors(NamedTuple):
     CLIENT_ERROR: str
     PREDICTION_ERROR: str
 
 
@@ -19,20 +19,20 @@
 class TaskResponse:
     prediction: str
     client_response: ClientResponse
     success: bool
 
 
 @runtime_checkable
-class ModelProtocol(Protocol):
+class ModelTaskProtocol(Protocol):
     adapter: BaseAdapter
 
     def predict(self, text: str, **kwargs) -> TaskResponse:
         ...
 
 
 @runtime_checkable
-class QAProtocol(Protocol):
+class QATaskProtocol(Protocol):
     adapter: BaseAdapter
 
     def ask(self, question: str, **kwargs) -> TaskResponse:
         ...
```

### Comparing `lmao-nlp-0.0.1b7/src/lmao/tasks/chatbot.py` & `lmao-nlp-0.0.1b8/src/lmao/tasks/chatbot.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b7/src/lmao/tasks/classification.py` & `lmao-nlp-0.0.1b8/src/lmao/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b7/src/lmao/tasks/fermi.py` & `lmao-nlp-0.0.1b8/src/lmao/tasks/fermi.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b7/src/lmao_nlp.egg-info/PKG-INFO` & `lmao-nlp-0.0.1b8/src/lmao_nlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmao-nlp
-Version: 0.0.1b7
+Version: 0.0.1b8
 Summary: LMAO: Language Model Adapters and Orchestrators
 Home-page: https://github.com/johnnygreco/lmao
 Author: Johnny Greco
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `lmao-nlp-0.0.1b7/src/lmao_nlp.egg-info/SOURCES.txt` & `lmao-nlp-0.0.1b8/src/lmao_nlp.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 src/lmao/adapters/classification.py
 src/lmao/adapters/fermi.py
 src/lmao/lm/__init__.py
 src/lmao/lm/utils.py
 src/lmao/lm/clients/__init__.py
 src/lmao/lm/clients/anthropic.py
 src/lmao/lm/clients/base.py
+src/lmao/lm/clients/cohere.py
 src/lmao/lm/clients/openai.py
 src/lmao/lm/schemas/__init__.py
 src/lmao/lm/schemas/anthropic.py
 src/lmao/lm/schemas/base.py
+src/lmao/lm/schemas/cohere.py
 src/lmao/lm/schemas/openai.py
 src/lmao/orchestrators/__init__.py
 src/lmao/orchestrators/base.py
 src/lmao/prompters/__init__.py
 src/lmao/prompters/base.py
 src/lmao/prompters/classification.py
 src/lmao/prompters/fermi.py
```

