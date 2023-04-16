# Comparing `tmp/lctutil-0.1.0.tar.gz` & `tmp/lctutil-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lctutil-0.1.0.tar", last modified: Sun Apr 16 06:40:32 2023, max compression
+gzip compressed data, was "lctutil-0.2.0.tar", last modified: Sun Apr 16 07:09:22 2023, max compression
```

## Comparing `lctutil-0.1.0.tar` & `lctutil-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 06:40:32.539573 lctutil-0.1.0/
--rw-rw-rw-   0        0        0      328 2023-04-16 06:40:32.538573 lctutil-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 06:40:32.533571 lctutil-0.1.0/lctutil.egg-info/
--rw-rw-rw-   0        0        0      328 2023-04-16 06:40:32.000000 lctutil-0.1.0/lctutil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-04-16 06:40:32.000000 lctutil-0.1.0/lctutil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 06:40:32.000000 lctutil-0.1.0/lctutil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-16 06:40:32.000000 lctutil-0.1.0/lctutil.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-16 06:40:32.000000 lctutil-0.1.0/lctutil.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-16 06:40:32.534571 lctutil-0.1.0/req_utils/
--rw-rw-rw-   0        0        0        0 2023-04-16 06:06:37.000000 lctutil-0.1.0/req_utils/__init__.py
--rw-rw-rw-   0        0        0     1456 2023-04-15 12:42:02.000000 lctutil-0.1.0/req_utils/opt_openai.py
--rw-rw-rw-   0        0        0       42 2023-04-16 06:40:32.539573 lctutil-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      609 2023-04-15 12:46:44.000000 lctutil-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 06:40:32.537573 lctutil-0.1.0/stock_infos/
--rw-rw-rw-   0        0        0        0 2023-04-16 06:06:37.000000 lctutil-0.1.0/stock_infos/__init__.py
--rw-rw-rw-   0        0        0     3320 2023-04-15 03:32:49.000000 lctutil-0.1.0/stock_infos/ac_matcher.py
--rw-rw-rw-   0        0        0     1147 2023-04-15 06:04:07.000000 lctutil-0.1.0/stock_infos/base_infos.py
--rw-rw-rw-   0        0        0     5766 2023-04-15 13:05:08.000000 lctutil-0.1.0/stock_infos/extract_base_info.py
+drwxrwxrwx   0        0        0        0 2023-04-16 07:09:22.534518 lctutil-0.2.0/
+-rw-rw-rw-   0        0        0      328 2023-04-16 07:09:22.533518 lctutil-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-16 06:41:27.000000 lctutil-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 07:09:22.528517 lctutil-0.2.0/lctutil.egg-info/
+-rw-rw-rw-   0        0        0      328 2023-04-16 07:09:22.000000 lctutil-0.2.0/lctutil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-04-16 07:09:22.000000 lctutil-0.2.0/lctutil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 07:09:22.000000 lctutil-0.2.0/lctutil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-16 07:09:22.000000 lctutil-0.2.0/lctutil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-16 07:09:22.000000 lctutil-0.2.0/lctutil.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 07:09:22.532518 lctutil-0.2.0/lctutils/
+-rw-rw-rw-   0        0        0        0 2023-04-16 06:06:37.000000 lctutil-0.2.0/lctutils/__init__.py
+-rw-rw-rw-   0        0        0     3320 2023-04-15 03:32:49.000000 lctutil-0.2.0/lctutils/ac_matcher.py
+-rw-rw-rw-   0        0        0     5766 2023-04-15 13:05:08.000000 lctutil-0.2.0/lctutils/extract_base_info.py
+-rw-rw-rw-   0        0        0     1456 2023-04-15 12:42:02.000000 lctutil-0.2.0/lctutils/openai.py
+-rw-rw-rw-   0        0        0     1147 2023-04-15 06:04:07.000000 lctutil-0.2.0/lctutils/stock_infos.py
+-rw-rw-rw-   0        0        0       42 2023-04-16 07:09:22.534518 lctutil-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      593 2023-04-16 07:08:32.000000 lctutil-0.2.0/setup.py
```

### Comparing `lctutil-0.1.0/req_utils/opt_openai.py` & `lctutil-0.2.0/lctutils/openai.py`

 * *Files identical despite different names*

### Comparing `lctutil-0.1.0/setup.py` & `lctutil-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='lctutil',
-    version='0.1.0',
+    version='0.2.0',
     packages=find_packages(),
     install_requires=[
         "pyahocorasick",
         "openai",
         "tenacity"
     ],
-    py_modules=["req_utils", "stock_infos"],
+    py_modules=["lctutils"],
     # Metadata
     author='LCT',
     author_email='your.email@example.com',
     description='LCT utils',
     url='https://github.com/yourusername/mypackage',
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `lctutil-0.1.0/stock_infos/ac_matcher.py` & `lctutil-0.2.0/lctutils/ac_matcher.py`

 * *Files identical despite different names*

### Comparing `lctutil-0.1.0/stock_infos/base_infos.py` & `lctutil-0.2.0/lctutils/stock_infos.py`

 * *Files identical despite different names*

### Comparing `lctutil-0.1.0/stock_infos/extract_base_info.py` & `lctutil-0.2.0/lctutils/extract_base_info.py`

 * *Files identical despite different names*

