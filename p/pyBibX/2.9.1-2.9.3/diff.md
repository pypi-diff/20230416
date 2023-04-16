# Comparing `tmp/pyBibX-2.9.1.tar.gz` & `tmp/pyBibX-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyBibX-2.9.1.tar", last modified: Mon Apr 10 01:55:19 2023, max compression
+gzip compressed data, was "dist\pyBibX-2.9.3.tar", last modified: Sun Apr 16 01:59:37 2023, max compression
```

## Comparing `pyBibX-2.9.1.tar` & `pyBibX-2.9.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 01:55:19.000000 pyBibX-2.9.1/
--rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-2.9.1/LICENSE
--rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-2.9.1/MANIFEST.in
--rw-rw-rw-   0        0        0     9131 2023-04-10 01:55:19.000000 pyBibX-2.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     8694 2023-04-10 01:54:14.000000 pyBibX-2.9.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 01:55:18.000000 pyBibX-2.9.1/pyBibX/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-2.9.1/pyBibX/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 01:55:18.000000 pyBibX-2.9.1/pyBibX/base/
--rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-2.9.1/pyBibX/base/__init__.py
--rw-rw-rw-   0        0        0   263502 2023-04-10 01:50:45.000000 pyBibX-2.9.1/pyBibX/base/pbx.py
-drwxrwxrwx   0        0        0        0 2023-04-10 01:55:19.000000 pyBibX-2.9.1/pyBibX/base/stws/
--rw-rw-rw-   0        0        0     1287 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Arabic.txt
--rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Bengali.txt
--rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Bulgarian.txt
--rw-rw-rw-   0        0        0     1518 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Czech.txt
--rw-rw-rw-   0        0        0     4212 2017-08-01 12:33:33.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-English.txt
--rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Finnish.txt
--rw-rw-rw-   0        0        0     3234 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-French.txt
--rw-rw-rw-   0        0        0     4350 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-German.txt
--rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Hindi.txt
--rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Hungarian.txt
--rw-rw-rw-   0        0        0     2379 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Italian.txt
--rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Marathi.txt
--rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Persian.txt
--rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Polish.txt
--rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Portuguese-br.txt
--rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Romanian.txt
--rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Russian.txt
--rw-rw-rw-   0        0        0     2420 2017-08-01 12:33:16.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Spanish.txt
--rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Swedish.txt
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-2.9.1/pyBibX/base/stws/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 01:55:18.000000 pyBibX-2.9.1/pyBibX.egg-info/
--rw-rw-rw-   0        0        0     9131 2023-04-10 01:55:17.000000 pyBibX-2.9.1/pyBibX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1047 2023-04-10 01:55:17.000000 pyBibX-2.9.1/pyBibX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 01:55:17.000000 pyBibX-2.9.1/pyBibX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      205 2023-04-10 01:55:17.000000 pyBibX-2.9.1/pyBibX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-10 01:55:17.000000 pyBibX-2.9.1/pyBibX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-10 01:55:17.000000 pyBibX-2.9.1/pyBibX.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-04-10 01:55:19.000000 pyBibX-2.9.1/setup.cfg
--rw-rw-rw-   0        0        0     1077 2023-04-10 01:51:00.000000 pyBibX-2.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:59:37.000000 pyBibX-2.9.3/
+-rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-2.9.3/LICENSE
+-rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-2.9.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     9131 2023-04-16 01:59:37.000000 pyBibX-2.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8694 2023-04-10 01:54:14.000000 pyBibX-2.9.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 01:59:37.000000 pyBibX-2.9.3/pyBibX/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-2.9.3/pyBibX/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:59:37.000000 pyBibX-2.9.3/pyBibX/base/
+-rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-2.9.3/pyBibX/base/__init__.py
+-rw-rw-rw-   0        0        0   263628 2023-04-16 01:55:01.000000 pyBibX-2.9.3/pyBibX/base/pbx.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:59:37.000000 pyBibX-2.9.3/pyBibX/base/stws/
+-rw-rw-rw-   0        0        0     1287 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Arabic.txt
+-rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Bengali.txt
+-rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Bulgarian.txt
+-rw-rw-rw-   0        0        0     1518 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Czech.txt
+-rw-rw-rw-   0        0        0     4212 2017-08-01 12:33:33.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-English.txt
+-rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Finnish.txt
+-rw-rw-rw-   0        0        0     3234 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-French.txt
+-rw-rw-rw-   0        0        0     4350 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-German.txt
+-rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Hindi.txt
+-rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Hungarian.txt
+-rw-rw-rw-   0        0        0     2379 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Italian.txt
+-rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Marathi.txt
+-rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Persian.txt
+-rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Polish.txt
+-rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Portuguese-br.txt
+-rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Romanian.txt
+-rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Russian.txt
+-rw-rw-rw-   0        0        0     2420 2017-08-01 12:33:16.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Spanish.txt
+-rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Swedish.txt
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-2.9.3/pyBibX/base/stws/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:59:37.000000 pyBibX-2.9.3/pyBibX.egg-info/
+-rw-rw-rw-   0        0        0     9131 2023-04-16 01:59:36.000000 pyBibX-2.9.3/pyBibX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1047 2023-04-16 01:59:36.000000 pyBibX-2.9.3/pyBibX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 01:59:36.000000 pyBibX-2.9.3/pyBibX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      210 2023-04-16 01:59:36.000000 pyBibX-2.9.3/pyBibX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-16 01:59:36.000000 pyBibX-2.9.3/pyBibX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-16 01:59:36.000000 pyBibX-2.9.3/pyBibX.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-04-16 01:59:37.000000 pyBibX-2.9.3/setup.cfg
+-rw-rw-rw-   0        0        0     1082 2023-04-16 01:58:53.000000 pyBibX-2.9.3/setup.py
```

### Comparing `pyBibX-2.9.1/LICENSE` & `pyBibX-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.1/PKG-INFO` & `pyBibX-2.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBibX
-Version: 2.9.1
+Version: 2.9.3
 Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
 Home-page: https://github.com/Valdecy/pyBibX
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyBibX-2.9.1/README.md` & `pyBibX-2.9.3/README.md`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.1/pyBibX/base/pbx.py` & `pyBibX-2.9.3/pyBibX/base/pbx.py`

 * *Files 0% similar despite different names*

```diff
@@ -3977,23 +3977,23 @@
             summary   = pegasus.generate(**tokens) # max_new_tokens = 1024, max_length = 1024, 
             summary   = tokenizer.decode(summary[0])
         else:
             summary   = 'No abstracts were found in the selected set of documents'
         return summary
     
     # Function: Abstractive Text Summarization
-    def summarize_abst_chatgpt(self, article_ids = [], join_articles = False, api_key = 'your_api_key_here', query = 'from the following scientific abstracts, summarize the main information in a single paragraph using around 250 words'):
-        def query_chatgpt(prompt, model = 'text-davinci-002', n = 1):
+    def summarize_abst_chatgpt(self, article_ids = [], join_articles = False, api_key = 'your_api_key_here', query = 'from the following scientific abstracts, summarize the main information in a single paragraph using around 250 words', model = 'text-davinci-003', max_tokens = 250, n = 1, temperature = 0.8):
+        def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
             response = openai.Completion.create(
                                                 engine      = model,
                                                 prompt      = prompt,
-                                                max_tokens  = 100,
+                                                max_tokens  = max_tokens,
                                                 n           = n,
                                                 stop        = None,
-                                                temperature = 0.8
+                                                temperature = temperature
                                                 )
             return response.choices[0].text.strip()
         openai.api_key = api_key
         abstracts      = self.data['abstract']
         corpus         = []
         if (len(article_ids) == 0):
             article_ids = [i for i in range(0, abstracts.shape[0])]
```

### Comparing `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Arabic.txt` & `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Arabic.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Bengali.txt` & `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Bengali.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Bulgarian.txt` & `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Bulgarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Czech.txt` & `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Czech.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-English.txt` & `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-English.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Finnish.txt` & `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Finnish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-French.txt` & `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-French.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-German.txt` & `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-German.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Hindi.txt` & `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Hindi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Hungarian.txt` & `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Hungarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Italian.txt` & `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Italian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Marathi.txt` & `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Marathi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Persian.txt` & `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Persian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Polish.txt` & `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Polish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Portuguese-br.txt` & `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Portuguese-br.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Romanian.txt` & `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Romanian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Russian.txt` & `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Russian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Spanish.txt` & `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Spanish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Swedish.txt` & `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Swedish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.1/pyBibX.egg-info/PKG-INFO` & `pyBibX-2.9.3/pyBibX.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBibX
-Version: 2.9.1
+Version: 2.9.3
 Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
 Home-page: https://github.com/Valdecy/pyBibX
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyBibX-2.9.1/pyBibX.egg-info/SOURCES.txt` & `pyBibX-2.9.3/pyBibX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.1/setup.py` & `pyBibX-2.9.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyBibX',
-    version='2.9.1',
+    version='2.9.3',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyBibX',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
@@ -18,18 +18,18 @@
         'bert-extractive-summarizer',
         'matplotlib',
         'networkx',
         'numpy',
         'pandas',
         'plotly',
         'scipy',
+        'scikit-learn',
         'sentencepiece',
         'sentence-transformers',
         'squarify',
-        'sklearn',
         'torch', 
         'torchvision',
         'torchaudio',
         'transformers',
         'umap-learn',
         'openai',
         'wordcloud'
```

