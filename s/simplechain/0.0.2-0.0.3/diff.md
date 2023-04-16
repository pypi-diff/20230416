# Comparing `tmp/simplechain-0.0.2.tar.gz` & `tmp/simplechain-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplechain-0.0.2.tar", last modified: Mon Mar 13 20:59:19 2023, max compression
+gzip compressed data, was "simplechain-0.0.3.tar", last modified: Sun Apr 16 16:54:24 2023, max compression
```

## Comparing `simplechain-0.0.2.tar` & `simplechain-0.0.3.tar`

### file list

```diff
@@ -1,59 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-03-13 20:59:19.437616 simplechain-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-03-02 13:34:38.000000 simplechain-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      600 2023-03-13 20:59:19.434615 simplechain-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2518 2023-03-13 20:58:40.000000 simplechain-0.0.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-03-13 20:59:19.438615 simplechain-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1103 2023-03-13 20:59:09.000000 simplechain-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-13 20:59:19.370615 simplechain-0.0.2/simplechain/
--rw-rw-rw-   0        0        0        0 2023-03-05 22:14:57.000000 simplechain-0.0.2/simplechain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-13 20:59:19.386619 simplechain-0.0.2/simplechain/pipeline/
--rw-rw-rw-   0        0        0      419 2023-03-07 20:36:53.000000 simplechain-0.0.2/simplechain/pipeline/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-13 20:59:19.389616 simplechain-0.0.2/simplechain/pipeline/data_loaders/
--rw-rw-rw-   0        0        0        0 2023-03-05 21:04:39.000000 simplechain-0.0.2/simplechain/pipeline/data_loaders/__init__.py
--rw-rw-rw-   0        0        0      138 2023-03-05 22:18:13.000000 simplechain-0.0.2/simplechain/pipeline/data_loaders/user_input.py
--rw-rw-rw-   0        0        0     1222 2023-03-08 22:10:48.000000 simplechain-0.0.2/simplechain/pipeline/module.py
-drwxrwxrwx   0        0        0        0 2023-03-13 20:59:19.395614 simplechain-0.0.2/simplechain/pipeline/prompt_templates/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:41:29.000000 simplechain-0.0.2/simplechain/pipeline/prompt_templates/__init__.py
--rw-rw-rw-   0        0        0      223 2023-03-05 22:32:39.000000 simplechain-0.0.2/simplechain/pipeline/prompt_templates/base_template.py
--rw-rw-rw-   0        0        0     4162 2023-03-07 18:33:03.000000 simplechain-0.0.2/simplechain/pipeline/prompt_templates/conversation_prompts.py
--rw-rw-rw-   0        0        0     1867 2023-03-05 22:32:39.000000 simplechain-0.0.2/simplechain/pipeline/prompt_templates/database_prompts.py
-drwxrwxrwx   0        0        0        0 2023-03-13 20:59:19.399614 simplechain-0.0.2/simplechain/pipeline/providers/
--rw-rw-rw-   0        0        0        0 2023-03-05 21:07:33.000000 simplechain-0.0.2/simplechain/pipeline/providers/__init__.py
--rw-rw-rw-   0        0        0      534 2023-03-07 04:38:40.000000 simplechain-0.0.2/simplechain/pipeline/providers/database.py
--rw-rw-rw-   0        0        0      373 2023-03-05 21:26:57.000000 simplechain-0.0.2/simplechain/pipeline/providers/search.py
--rw-rw-rw-   0        0        0      869 2023-03-08 23:29:30.000000 simplechain-0.0.2/simplechain/pipeline/standard_modules.py
-drwxrwxrwx   0        0        0        0 2023-03-13 20:59:19.400617 simplechain-0.0.2/simplechain/stack/
--rw-rw-rw-   0        0        0      479 2023-03-13 20:57:40.000000 simplechain-0.0.2/simplechain/stack/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-13 20:59:19.407616 simplechain-0.0.2/simplechain/stack/databases/
--rw-rw-rw-   0        0        0        0 2023-03-05 00:08:11.000000 simplechain-0.0.2/simplechain/stack/databases/__init__.py
--rw-rw-rw-   0        0        0      519 2023-03-09 17:10:16.000000 simplechain-0.0.2/simplechain/stack/databases/base.py
--rw-rw-rw-   0        0        0     8271 2023-03-10 19:12:08.000000 simplechain-0.0.2/simplechain/stack/databases/sql.py
-drwxrwxrwx   0        0        0        0 2023-03-13 20:59:19.409616 simplechain-0.0.2/simplechain/stack/image_generators/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:53:34.000000 simplechain-0.0.2/simplechain/stack/image_generators/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-13 20:59:19.413615 simplechain-0.0.2/simplechain/stack/search_engines/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:42:47.000000 simplechain-0.0.2/simplechain/stack/search_engines/__init__.py
--rw-rw-rw-   0        0        0      214 2023-03-05 21:26:57.000000 simplechain-0.0.2/simplechain/stack/search_engines/base.py
--rw-rw-rw-   0        0        0     2887 2023-03-05 21:26:57.000000 simplechain-0.0.2/simplechain/stack/search_engines/google_serper.py
-drwxrwxrwx   0        0        0        0 2023-03-13 20:59:19.418614 simplechain-0.0.2/simplechain/stack/text_embedders/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:53:13.000000 simplechain-0.0.2/simplechain/stack/text_embedders/__init__.py
--rw-rw-rw-   0        0        0      291 2023-03-12 17:43:22.000000 simplechain-0.0.2/simplechain/stack/text_embedders/base.py
--rw-rw-rw-   0        0        0     1144 2023-03-13 20:11:00.000000 simplechain-0.0.2/simplechain/stack/text_embedders/openai.py
-drwxrwxrwx   0        0        0        0 2023-03-13 20:59:19.422615 simplechain-0.0.2/simplechain/stack/text_generators/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:47:34.000000 simplechain-0.0.2/simplechain/stack/text_generators/__init__.py
--rw-rw-rw-   0        0        0      184 2023-03-08 18:14:03.000000 simplechain-0.0.2/simplechain/stack/text_generators/base.py
-drwxrwxrwx   0        0        0        0 2023-03-13 20:59:19.426615 simplechain-0.0.2/simplechain/stack/text_generators/llms/
--rw-rw-rw-   0        0        0        0 2023-03-05 00:03:03.000000 simplechain-0.0.2/simplechain/stack/text_generators/llms/__init__.py
--rw-rw-rw-   0        0        0      784 2023-03-08 18:14:03.000000 simplechain-0.0.2/simplechain/stack/text_generators/llms/llm.py
--rw-rw-rw-   0        0        0     1176 2023-03-08 18:14:03.000000 simplechain-0.0.2/simplechain/stack/text_generators/llms/openai.py
-drwxrwxrwx   0        0        0        0 2023-03-13 20:59:19.431616 simplechain-0.0.2/simplechain/stack/vector_databases/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:53:21.000000 simplechain-0.0.2/simplechain/stack/vector_databases/__init__.py
--rw-rw-rw-   0        0        0     2834 2023-03-12 19:01:09.000000 simplechain-0.0.2/simplechain/stack/vector_databases/annoy.py
--rw-rw-rw-   0        0        0      872 2023-03-12 16:45:38.000000 simplechain-0.0.2/simplechain/stack/vector_databases/base.py
--rw-rw-rw-   0        0        0      708 2023-03-05 00:01:34.000000 simplechain-0.0.2/simplechain/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-13 20:59:19.382614 simplechain-0.0.2/simplechain.egg-info/
--rw-rw-rw-   0        0        0      600 2023-03-13 20:59:19.000000 simplechain-0.0.2/simplechain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1602 2023-03-13 20:59:19.000000 simplechain-0.0.2/simplechain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-13 20:59:19.000000 simplechain-0.0.2/simplechain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-03-13 20:59:19.000000 simplechain-0.0.2/simplechain.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-13 20:59:19.432616 simplechain-0.0.2/tests/
--rw-rw-rw-   0        0        0       33 2023-03-01 21:32:35.000000 simplechain-0.0.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.237884 simplechain-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-03-02 13:34:38.000000 simplechain-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      600 2023-04-16 16:54:24.236884 simplechain-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2902 2023-04-11 15:12:28.000000 simplechain-0.0.3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-16 16:54:24.237884 simplechain-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1103 2023-04-16 16:54:12.000000 simplechain-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.083884 simplechain-0.0.3/simplechain/
+-rw-rw-rw-   0        0        0        0 2023-03-05 22:14:57.000000 simplechain-0.0.3/simplechain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.109884 simplechain-0.0.3/simplechain/pipeline/
+-rw-rw-rw-   0        0        0      419 2023-03-07 20:36:53.000000 simplechain-0.0.3/simplechain/pipeline/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.113885 simplechain-0.0.3/simplechain/pipeline/data_loaders/
+-rw-rw-rw-   0        0        0        0 2023-03-05 21:04:39.000000 simplechain-0.0.3/simplechain/pipeline/data_loaders/__init__.py
+-rw-rw-rw-   0        0        0      138 2023-03-05 22:18:13.000000 simplechain-0.0.3/simplechain/pipeline/data_loaders/user_input.py
+-rw-rw-rw-   0        0        0     1222 2023-03-08 22:10:48.000000 simplechain-0.0.3/simplechain/pipeline/module.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.121884 simplechain-0.0.3/simplechain/pipeline/prompt_templates/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:41:29.000000 simplechain-0.0.3/simplechain/pipeline/prompt_templates/__init__.py
+-rw-rw-rw-   0        0        0      223 2023-03-05 22:32:39.000000 simplechain-0.0.3/simplechain/pipeline/prompt_templates/base_template.py
+-rw-rw-rw-   0        0        0     4162 2023-03-07 18:33:03.000000 simplechain-0.0.3/simplechain/pipeline/prompt_templates/conversation_prompts.py
+-rw-rw-rw-   0        0        0     1867 2023-03-05 22:32:39.000000 simplechain-0.0.3/simplechain/pipeline/prompt_templates/database_prompts.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.127883 simplechain-0.0.3/simplechain/pipeline/providers/
+-rw-rw-rw-   0        0        0        0 2023-03-05 21:07:33.000000 simplechain-0.0.3/simplechain/pipeline/providers/__init__.py
+-rw-rw-rw-   0        0        0      534 2023-03-07 04:38:40.000000 simplechain-0.0.3/simplechain/pipeline/providers/database.py
+-rw-rw-rw-   0        0        0      373 2023-03-05 21:26:57.000000 simplechain-0.0.3/simplechain/pipeline/providers/search.py
+-rw-rw-rw-   0        0        0      869 2023-03-08 23:29:30.000000 simplechain-0.0.3/simplechain/pipeline/standard_modules.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.142883 simplechain-0.0.3/simplechain/stack/
+-rw-rw-rw-   0        0        0      226 2023-04-11 18:57:45.000000 simplechain-0.0.3/simplechain/stack/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.155884 simplechain-0.0.3/simplechain/stack/databases/
+-rw-rw-rw-   0        0        0        0 2023-03-05 00:08:11.000000 simplechain-0.0.3/simplechain/stack/databases/__init__.py
+-rw-rw-rw-   0        0        0      519 2023-03-09 17:10:16.000000 simplechain-0.0.3/simplechain/stack/databases/base.py
+-rw-rw-rw-   0        0        0     8271 2023-03-10 19:12:08.000000 simplechain-0.0.3/simplechain/stack/databases/sql.py
+-rw-rw-rw-   0        0        0     2805 2023-04-11 21:35:31.000000 simplechain-0.0.3/simplechain/stack/factory.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.156884 simplechain-0.0.3/simplechain/stack/image_generators/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:53:34.000000 simplechain-0.0.3/simplechain/stack/image_generators/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.157884 simplechain-0.0.3/simplechain/stack/pdf_loaders/
+-rw-rw-rw-   0        0        0        0 2023-04-10 15:02:16.000000 simplechain-0.0.3/simplechain/stack/pdf_loaders/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.169885 simplechain-0.0.3/simplechain/stack/search_engines/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:42:47.000000 simplechain-0.0.3/simplechain/stack/search_engines/__init__.py
+-rw-rw-rw-   0        0        0      214 2023-03-05 21:26:57.000000 simplechain-0.0.3/simplechain/stack/search_engines/base.py
+-rw-rw-rw-   0        0        0     2887 2023-03-05 21:26:57.000000 simplechain-0.0.3/simplechain/stack/search_engines/google_serper.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.186886 simplechain-0.0.3/simplechain/stack/text_embedders/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:53:13.000000 simplechain-0.0.3/simplechain/stack/text_embedders/__init__.py
+-rw-rw-rw-   0        0        0      345 2023-04-11 15:48:43.000000 simplechain-0.0.3/simplechain/stack/text_embedders/base.py
+-rw-rw-rw-   0        0        0     1112 2023-04-11 15:45:29.000000 simplechain-0.0.3/simplechain/stack/text_embedders/openai.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.189884 simplechain-0.0.3/simplechain/stack/text_generators/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:47:34.000000 simplechain-0.0.3/simplechain/stack/text_generators/__init__.py
+-rw-rw-rw-   0        0        0      184 2023-03-08 18:14:03.000000 simplechain-0.0.3/simplechain/stack/text_generators/base.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.203884 simplechain-0.0.3/simplechain/stack/text_generators/llms/
+-rw-rw-rw-   0        0        0        0 2023-03-05 00:03:03.000000 simplechain-0.0.3/simplechain/stack/text_generators/llms/__init__.py
+-rw-rw-rw-   0        0        0     2194 2023-04-11 21:48:56.000000 simplechain-0.0.3/simplechain/stack/text_generators/llms/ai21.py
+-rw-rw-rw-   0        0        0      784 2023-03-08 18:14:03.000000 simplechain-0.0.3/simplechain/stack/text_generators/llms/llm.py
+-rw-rw-rw-   0        0        0     1176 2023-03-08 18:14:03.000000 simplechain-0.0.3/simplechain/stack/text_generators/llms/openai.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.228885 simplechain-0.0.3/simplechain/stack/vector_databases/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:53:21.000000 simplechain-0.0.3/simplechain/stack/vector_databases/__init__.py
+-rw-rw-rw-   0        0        0     3163 2023-04-11 15:49:56.000000 simplechain-0.0.3/simplechain/stack/vector_databases/annoy.py
+-rw-rw-rw-   0        0        0     1120 2023-04-11 15:49:25.000000 simplechain-0.0.3/simplechain/stack/vector_databases/base.py
+-rw-rw-rw-   0        0        0     2451 2023-04-10 19:19:49.000000 simplechain-0.0.3/simplechain/stack/vector_databases/faiss.py
+-rw-rw-rw-   0        0        0      708 2023-03-05 00:01:34.000000 simplechain-0.0.3/simplechain/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.101883 simplechain-0.0.3/simplechain.egg-info/
+-rw-rw-rw-   0        0        0      600 2023-04-16 16:54:23.000000 simplechain-0.0.3/simplechain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1764 2023-04-16 16:54:23.000000 simplechain-0.0.3/simplechain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 16:54:23.000000 simplechain-0.0.3/simplechain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-16 16:54:23.000000 simplechain-0.0.3/simplechain.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 16:54:24.235885 simplechain-0.0.3/tests/
+-rw-rw-rw-   0        0        0       33 2023-03-01 21:32:35.000000 simplechain-0.0.3/tests/__init__.py
```

### Comparing `simplechain-0.0.2/LICENSE` & `simplechain-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.2/PKG-INFO` & `simplechain-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplechain
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package of AI services in modular form
 Author: Rahel Gunaratne
 Author-email: rahel.gunaratne@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `simplechain-0.0.2/README.rst` & `simplechain-0.0.3/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+
+text_gen = TextGenerator("openAI", "text-ada")
+text_gen = TextGeneratorOpenAI("text-ada")
+text_gen = TextGeneratorLLM("text-ada")
+
+text_gen = TextGenerator().hyperparameters() # get
+
+text_gen = TextGenerator().model("text-ada").hyperparameters({"temperature": 0.9}) # set
+text_gen = TextGenerator().model("text-ada").preset("QA") # set
+text = text_gen.generate(prompt)
+
+
+
+
+
+
+
 ================
 TODO
 ================
 
 - [ ] Add a testing framework using LLM's as testers
 - [ ] Add unit testing for each module and integrations tests
 - [ ] Add CI/CD before pushing to master
@@ -21,15 +38,15 @@
 ==============
 pip install -r requirements.txt
 
 `python setup.py sdist bdist_wheel`
 
 twine upload dist/*
 
-twine upload -u 'kael558' -p 'A6C4Yh@uMuwrsdg' --repository-url https://upload.pypi.org/legacy/ dist/*
+twine upload -u <username> -p <pass> --repository-url https://upload.pypi.org/legacy/ dist/*
 
 pip install --index-url "https://test.pypi.org/simple/<package_name>"
```

### Comparing `simplechain-0.0.2/setup.py` & `simplechain-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'A package of AI services in modular form'
 LONG_DESCRIPTION = 'A package of AI services in modular form easily configurable and deployable'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="simplechain",
```

### Comparing `simplechain-0.0.2/simplechain/pipeline/module.py` & `simplechain-0.0.3/simplechain/pipeline/module.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.2/simplechain/pipeline/prompt_templates/conversation_prompts.py` & `simplechain-0.0.3/simplechain/pipeline/prompt_templates/conversation_prompts.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.2/simplechain/pipeline/prompt_templates/database_prompts.py` & `simplechain-0.0.3/simplechain/pipeline/prompt_templates/database_prompts.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.2/simplechain/pipeline/providers/database.py` & `simplechain-0.0.3/simplechain/pipeline/providers/database.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.2/simplechain/pipeline/standard_modules.py` & `simplechain-0.0.3/simplechain/pipeline/standard_modules.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.2/simplechain/stack/databases/base.py` & `simplechain-0.0.3/simplechain/stack/databases/base.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.2/simplechain/stack/databases/sql.py` & `simplechain-0.0.3/simplechain/stack/databases/sql.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.2/simplechain/stack/search_engines/google_serper.py` & `simplechain-0.0.3/simplechain/stack/search_engines/google_serper.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.2/simplechain/stack/text_embedders/openai.py` & `simplechain-0.0.3/simplechain/stack/text_embedders/openai.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Union, List, Dict
 
 import numpy as np
 import openai
 from pydantic import root_validator
 
-from simplechain.stack import TextEmbedder
+from simplechain.stack.text_embedders.base import TextEmbedder
 from simplechain.utils import get_from_dict_or_env
 
 
 class TextEmbedderOpenAI(TextEmbedder):
     model_name = "text-embedding-ada-002"
 
     @root_validator()
@@ -18,16 +18,16 @@
             values, "openai_api_key", "OPENAI_API_KEY"
         )
         values["openai_api_key"] = openai_api_key
         openai.api_key = openai_api_key
 
         return values
 
-    def embed(self, text: Union[List[str], str]) -> Union[List[np.ndarray], np.ndarray]:
-        if isinstance(text, str):
-            text = text.replace("\n", " ")
-            return openai.Embedding.create(input=[text], model=self.model_name)['data'][0]['embedding']
-        embeddings = openai.Embedding.create(input=list(text), model=self.model_name)
-        print(embeddings)
+    def embed(self, text: str) -> np.ndarray:
+        text = text.replace("\n", " ")
+        return openai.Embedding.create(input=[text], model=self.model_name)['data'][0]['embedding']
 
+
+    def embed_all(self, texts: List[str]) -> List[np.ndarray]:
+        embeddings = openai.Embedding.create(input=texts, model=self.model_name)
         return [embedding['embedding'] for embedding in embeddings['data']]
```

### Comparing `simplechain-0.0.2/simplechain/stack/text_generators/llms/llm.py` & `simplechain-0.0.3/simplechain/stack/text_generators/llms/llm.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.2/simplechain/stack/text_generators/llms/openai.py` & `simplechain-0.0.3/simplechain/stack/text_generators/llms/openai.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.2/simplechain/stack/vector_databases/annoy.py` & `simplechain-0.0.3/simplechain/stack/vector_databases/annoy.py`

 * *Files 15% similar despite different names*

```diff
@@ -44,23 +44,33 @@
         self.i = 0
 
         self.path_to_metadata_file = path_to_metadata_file
         self.metadata = get_metadata(path_to_metadata_file)
 
     def add(self, embed: np.ndarray, metadata: Any):
         """
-        Add a name and its embed to the database
+        Add an embed and its metadata to the database
         :param embed:
         :param metadata:
         :return:
         """
         self.index.add_item(self.i, embed)
         self.i += 1
         self.metadata.append(metadata)
 
+    def add_all(self, embeds: np.ndarray, metadatas: List[Any]):
+        """
+        Add a list of embeds and their metadatas to the database
+        :param embeds:
+        :param metadatas:
+        :return:
+        """
+        for embed, metadata in zip(embeds, metadatas):
+            self.add(embed, metadata)
+
     def save(self):
         """Save the data"""
         # Save the index
         self.index.build(self.n_trees)
         self.index.save(self.path_to_index_file)
 
         # Save metadata to json
```

### Comparing `simplechain-0.0.2/simplechain/stack/vector_databases/base.py` & `simplechain-0.0.3/simplechain/stack/vector_databases/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,19 +6,29 @@
 
 class VectorDatabase(ABC):
     @abstractmethod
     def add(self, embed: np.ndarray, metadata: Any):
         """
         Add a name and its embed to the database
         :param metadata:
-        :param name:
         :param embed:
         :return:
         """
         pass
+
+    @abstractmethod
+    def add_all(self, embeds: np.ndarray, metadatas: List[Any]):
+        """
+        Add a list of names and their embeds to the database
+        :param metadatas:
+        :param embeds:
+        :return:
+        """
+        pass
+
     @abstractmethod
     def save(self):
         """
         Build the database
         :return:
         """
         pass
@@ -28,7 +38,11 @@
         """
         Given a query embed, get the k nearest neighbors with their distances
         :param query_embed:
         :param k:
         :return: k nearest neighbors as strings with their distances
         """
         pass
+
+
+
+
```

### Comparing `simplechain-0.0.2/simplechain/utils.py` & `simplechain-0.0.3/simplechain/utils.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.2/simplechain.egg-info/PKG-INFO` & `simplechain-0.0.3/simplechain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplechain
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package of AI services in modular form
 Author: Rahel Gunaratne
 Author-email: rahel.gunaratne@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `simplechain-0.0.2/simplechain.egg-info/SOURCES.txt` & `simplechain-0.0.3/simplechain.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,26 +16,30 @@
 simplechain/pipeline/prompt_templates/base_template.py
 simplechain/pipeline/prompt_templates/conversation_prompts.py
 simplechain/pipeline/prompt_templates/database_prompts.py
 simplechain/pipeline/providers/__init__.py
 simplechain/pipeline/providers/database.py
 simplechain/pipeline/providers/search.py
 simplechain/stack/__init__.py
+simplechain/stack/factory.py
 simplechain/stack/databases/__init__.py
 simplechain/stack/databases/base.py
 simplechain/stack/databases/sql.py
 simplechain/stack/image_generators/__init__.py
+simplechain/stack/pdf_loaders/__init__.py
 simplechain/stack/search_engines/__init__.py
 simplechain/stack/search_engines/base.py
 simplechain/stack/search_engines/google_serper.py
 simplechain/stack/text_embedders/__init__.py
 simplechain/stack/text_embedders/base.py
 simplechain/stack/text_embedders/openai.py
 simplechain/stack/text_generators/__init__.py
 simplechain/stack/text_generators/base.py
 simplechain/stack/text_generators/llms/__init__.py
+simplechain/stack/text_generators/llms/ai21.py
 simplechain/stack/text_generators/llms/llm.py
 simplechain/stack/text_generators/llms/openai.py
 simplechain/stack/vector_databases/__init__.py
 simplechain/stack/vector_databases/annoy.py
 simplechain/stack/vector_databases/base.py
+simplechain/stack/vector_databases/faiss.py
 tests/__init__.py
```

