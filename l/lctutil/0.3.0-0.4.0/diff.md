# Comparing `tmp/lctutil-0.3.0.tar.gz` & `tmp/lctutil-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lctutil-0.3.0.tar", last modified: Sun Apr 16 07:14:44 2023, max compression
+gzip compressed data, was "lctutil-0.4.0.tar", last modified: Sun Apr 16 12:33:25 2023, max compression
```

## Comparing `lctutil-0.3.0.tar` & `lctutil-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 07:14:44.015651 lctutil-0.3.0/
--rw-rw-rw-   0        0        0      328 2023-04-16 07:14:44.015651 lctutil-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-16 06:41:27.000000 lctutil-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 07:14:44.009650 lctutil-0.3.0/lctutil/
--rw-rw-rw-   0        0        0        0 2023-04-16 06:06:37.000000 lctutil-0.3.0/lctutil/__init__.py
--rw-rw-rw-   0        0        0     3320 2023-04-15 03:32:49.000000 lctutil-0.3.0/lctutil/ac_matcher.py
--rw-rw-rw-   0        0        0     5766 2023-04-15 13:05:08.000000 lctutil-0.3.0/lctutil/extract_base_info.py
--rw-rw-rw-   0        0        0     1456 2023-04-15 12:42:02.000000 lctutil-0.3.0/lctutil/openai.py
--rw-rw-rw-   0        0        0     1147 2023-04-15 06:04:07.000000 lctutil-0.3.0/lctutil/stock_infos.py
-drwxrwxrwx   0        0        0        0 2023-04-16 07:14:44.014652 lctutil-0.3.0/lctutil.egg-info/
--rw-rw-rw-   0        0        0      328 2023-04-16 07:14:43.000000 lctutil-0.3.0/lctutil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-04-16 07:14:43.000000 lctutil-0.3.0/lctutil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 07:14:43.000000 lctutil-0.3.0/lctutil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-16 07:14:43.000000 lctutil-0.3.0/lctutil.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-16 07:14:43.000000 lctutil-0.3.0/lctutil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 07:14:44.015651 lctutil-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      592 2023-04-16 07:14:39.000000 lctutil-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:33:25.558132 lctutil-0.4.0/
+-rw-rw-rw-   0        0        0      328 2023-04-16 12:33:25.558132 lctutil-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2023-04-16 12:32:34.000000 lctutil-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 12:33:25.553131 lctutil-0.4.0/lctutil/
+-rw-rw-rw-   0        0        0        0 2023-04-16 06:06:37.000000 lctutil-0.4.0/lctutil/__init__.py
+-rw-rw-rw-   0        0        0     3321 2023-04-16 07:45:57.000000 lctutil-0.4.0/lctutil/ac_matcher.py
+-rw-rw-rw-   0        0        0     5766 2023-04-15 13:05:08.000000 lctutil-0.4.0/lctutil/extract_base_info.py
+-rw-rw-rw-   0        0        0     1502 2023-04-16 09:10:14.000000 lctutil-0.4.0/lctutil/openai.py
+-rw-rw-rw-   0        0        0     1147 2023-04-15 06:04:07.000000 lctutil-0.4.0/lctutil/stock_infos.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:33:25.557132 lctutil-0.4.0/lctutil.egg-info/
+-rw-rw-rw-   0        0        0      328 2023-04-16 12:33:25.000000 lctutil-0.4.0/lctutil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-04-16 12:33:25.000000 lctutil-0.4.0/lctutil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 12:33:25.000000 lctutil-0.4.0/lctutil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-16 12:33:25.000000 lctutil-0.4.0/lctutil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-16 12:33:25.000000 lctutil-0.4.0/lctutil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 12:33:25.559132 lctutil-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      592 2023-04-16 12:32:53.000000 lctutil-0.4.0/setup.py
```

### Comparing `lctutil-0.3.0/lctutil/ac_matcher.py` & `lctutil-0.4.0/lctutil/ac_matcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             start_index = end_index - key_length + 1
             mt = query[start_index: end_index + 1]
             if mt not in has_seen:
                 has_seen.append(mt)
                 ans.append((mt, tags))
         return ans
 
-from .base_infos import info_stock_names, all_gainian, all_bankuai_2, all_bankuai_3
+from .stock_infos import info_stock_names, all_gainian, all_bankuai_2, all_bankuai_3
 
 S_NAME_TAG = "STOCK"
 S_BK_TAG = "BK"
 S_GAINIAN_TAG = "GAINIAN"
 
 stock_ac = AC()
 stock_ac.init_slot_list_ac(info_stock_names, S_NAME_TAG)
```

### Comparing `lctutil-0.3.0/lctutil/extract_base_info.py` & `lctutil-0.4.0/lctutil/extract_base_info.py`

 * *Files identical despite different names*

### Comparing `lctutil-0.3.0/lctutil/openai.py` & `lctutil-0.4.0/lctutil/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     openai.api_key = apikeys[api_k_index] 
     api_k_index = api_k_index + 1
 
 
 @retry(wait=wait_random_exponential(min=9, max=20), stop=stop_after_attempt(3))
 def get_embeddings(texts: List[str]) -> List[List[float]]:
     set_api_key_inturn()
+    if type(texts) == "str": texts = [texts]
     response = openai.Embedding.create(input=texts, model="text-embedding-ada-002")
     data = response["data"]  # type: ignore
     return [result["embedding"] for result in data]
 
 
 @retry(wait=wait_random_exponential(min=9, max=20), stop=stop_after_attempt(3))
 def get_chat_completion(
```

### Comparing `lctutil-0.3.0/lctutil/stock_infos.py` & `lctutil-0.4.0/lctutil/stock_infos.py`

 * *Files identical despite different names*

### Comparing `lctutil-0.3.0/setup.py` & `lctutil-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='lctutil',
-    version='0.3.0',
+    version='0.4.0',
     packages=find_packages(),
     install_requires=[
         "pyahocorasick",
         "openai",
         "tenacity"
     ],
     py_modules=["lctutil"],
```

