# Comparing `tmp/ai-talks-0.8.8.2.tar.gz` & `tmp/ai-talks-0.8.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-talks-0.8.8.2.tar", last modified: Sat Apr 15 23:38:02 2023, max compression
+gzip compressed data, was "ai-talks-0.8.8.8.tar", last modified: Sat Apr 15 23:44:41 2023, max compression
```

## Comparing `ai-talks-0.8.8.2.tar` & `ai-talks-0.8.8.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-15 23:38:02.257633 ai-talks-0.8.8.2/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1074 2023-04-09 09:49:53.000000 ai-talks-0.8.8.2/LICENSE
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     2732 2023-04-15 23:38:02.257250 ai-talks-0.8.8.2/PKG-INFO
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1922 2023-04-15 19:25:22.000000 ai-talks-0.8.8.2/README.md
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-15 23:38:02.242856 ai-talks-0.8.8.2/ai_talks.egg-info/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     2732 2023-04-15 23:38:02.000000 ai-talks-0.8.8.2/ai_talks.egg-info/PKG-INFO
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      512 2023-04-15 23:38:02.000000 ai-talks-0.8.8.2/ai_talks.egg-info/SOURCES.txt
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        1 2023-04-15 23:38:02.000000 ai-talks-0.8.8.2/ai_talks.egg-info/dependency_links.txt
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)       46 2023-04-15 23:38:02.000000 ai-talks-0.8.8.2/ai_talks.egg-info/entry_points.txt
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      167 2023-04-15 23:38:02.000000 ai-talks-0.8.8.2/ai_talks.egg-info/requires.txt
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)       14 2023-04-15 23:38:02.000000 ai-talks-0.8.8.2/ai_talks.egg-info/top_level.txt
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-15 23:38:02.243919 ai-talks-0.8.8.2/pkg/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-04-15 23:36:34.000000 ai-talks-0.8.8.2/pkg/__init__.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      103 2023-04-15 21:38:36.000000 ai-talks-0.8.8.2/pkg/run_agi.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      846 2023-04-09 19:26:49.000000 ai-talks-0.8.8.2/pyproject.toml
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)       38 2023-04-15 23:38:02.257748 ai-talks-0.8.8.2/setup.cfg
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1384 2023-04-15 23:37:30.000000 ai-talks-0.8.8.2/setup.py
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-15 23:38:02.245192 ai-talks-0.8.8.2/src/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.8.2/src/__init__.py
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-15 23:38:02.247622 ai-talks-0.8.8.2/src/styles/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.8.2/src/styles/__init__.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      735 2023-03-23 21:57:52.000000 ai-talks-0.8.8.2/src/styles/menu_styles.py
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-15 23:38:02.254518 ai-talks-0.8.8.2/src/utils/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.8.2/src/utils/__init__.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     3695 2023-04-15 19:59:55.000000 ai-talks-0.8.8.2/src/utils/conversation.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1797 2023-04-15 19:25:22.000000 ai-talks-0.8.8.2/src/utils/footer.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      616 2023-04-09 19:46:48.000000 ai-talks-0.8.8.2/src/utils/helpers.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     7261 2023-04-15 22:07:51.000000 ai-talks-0.8.8.2/src/utils/lang.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     3672 2023-04-15 23:37:33.000000 ai-talks-0.8.8.2/src/utils/stt.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      416 2023-04-15 19:59:55.000000 ai-talks-0.8.8.2/src/utils/tts.py
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-15 23:38:02.256060 ai-talks-0.8.8.2/tests/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.8.2/tests/__init__.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      180 2023-04-09 19:59:55.000000 ai-talks-0.8.8.2/tests/test_helpers.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-15 23:44:41.754109 ai-talks-0.8.8.8/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1074 2023-04-09 09:49:53.000000 ai-talks-0.8.8.8/LICENSE
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     2732 2023-04-15 23:44:41.753200 ai-talks-0.8.8.8/PKG-INFO
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1922 2023-04-15 19:25:22.000000 ai-talks-0.8.8.8/README.md
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-15 23:44:41.736110 ai-talks-0.8.8.8/ai_talks.egg-info/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     2732 2023-04-15 23:44:41.000000 ai-talks-0.8.8.8/ai_talks.egg-info/PKG-INFO
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      512 2023-04-15 23:44:41.000000 ai-talks-0.8.8.8/ai_talks.egg-info/SOURCES.txt
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        1 2023-04-15 23:44:41.000000 ai-talks-0.8.8.8/ai_talks.egg-info/dependency_links.txt
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)       46 2023-04-15 23:44:41.000000 ai-talks-0.8.8.8/ai_talks.egg-info/entry_points.txt
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      167 2023-04-15 23:44:41.000000 ai-talks-0.8.8.8/ai_talks.egg-info/requires.txt
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)       14 2023-04-15 23:44:41.000000 ai-talks-0.8.8.8/ai_talks.egg-info/top_level.txt
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-15 23:44:41.737427 ai-talks-0.8.8.8/pkg/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-04-15 23:36:34.000000 ai-talks-0.8.8.8/pkg/__init__.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      106 2023-04-15 23:42:17.000000 ai-talks-0.8.8.8/pkg/run_agi.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      846 2023-04-09 19:26:49.000000 ai-talks-0.8.8.8/pyproject.toml
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)       38 2023-04-15 23:44:41.754326 ai-talks-0.8.8.8/setup.cfg
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1384 2023-04-15 23:44:32.000000 ai-talks-0.8.8.8/setup.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-15 23:44:41.738442 ai-talks-0.8.8.8/src/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.8.8/src/__init__.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-15 23:44:41.739400 ai-talks-0.8.8.8/src/styles/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.8.8/src/styles/__init__.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      735 2023-03-23 21:57:52.000000 ai-talks-0.8.8.8/src/styles/menu_styles.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-15 23:44:41.745611 ai-talks-0.8.8.8/src/utils/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.8.8/src/utils/__init__.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     3695 2023-04-15 19:59:55.000000 ai-talks-0.8.8.8/src/utils/conversation.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1797 2023-04-15 19:25:22.000000 ai-talks-0.8.8.8/src/utils/footer.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      616 2023-04-09 19:46:48.000000 ai-talks-0.8.8.8/src/utils/helpers.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     7261 2023-04-15 22:07:51.000000 ai-talks-0.8.8.8/src/utils/lang.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     3672 2023-04-15 23:44:34.000000 ai-talks-0.8.8.8/src/utils/stt.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      416 2023-04-15 19:59:55.000000 ai-talks-0.8.8.8/src/utils/tts.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-15 23:44:41.748411 ai-talks-0.8.8.8/tests/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.8.8/tests/__init__.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      180 2023-04-09 19:59:55.000000 ai-talks-0.8.8.8/tests/test_helpers.py
```

### Comparing `ai-talks-0.8.8.2/LICENSE` & `ai-talks-0.8.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.8.2/PKG-INFO` & `ai-talks-0.8.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-talks
-Version: 0.8.8.2
+Version: 0.8.8.8
 Summary: A ChatGPT API wrapper, providing a user-friendly Streamlit web interface
 Home-page: https://github.com/dKosarevsky/AI-Talks
 Author: Dmitry Kosarevsky
 Author-email: if.kosarevsky@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ai-talks-0.8.8.2/README.md` & `ai-talks-0.8.8.8/README.md`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.8.2/ai_talks.egg-info/PKG-INFO` & `ai-talks-0.8.8.8/ai_talks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-talks
-Version: 0.8.8.2
+Version: 0.8.8.8
 Summary: A ChatGPT API wrapper, providing a user-friendly Streamlit web interface
 Home-page: https://github.com/dKosarevsky/AI-Talks
 Author: Dmitry Kosarevsky
 Author-email: if.kosarevsky@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ai-talks-0.8.8.2/ai_talks.egg-info/SOURCES.txt` & `ai-talks-0.8.8.8/ai_talks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.8.2/pyproject.toml` & `ai-talks-0.8.8.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.8.2/setup.py` & `ai-talks-0.8.8.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of the requirements.txt file
 with open("requirements.txt") as f:
     requirements = [line.strip() for line in f.readlines() if not line.startswith("-f")]
 
 setup(
     name="ai-talks",
-    version="0.8.8.2",
+    version="0.8.8.8",
     exclude_package_data={"": ["secrets.toml"]},
     packages=find_packages(exclude=["secrets.toml", ]),
     install_requires=requirements,  # Use the parsed requirements here
     entry_points={
         "console_scripts": [
             "ai-talks=pkg.run_agi:main",
         ],
```

### Comparing `ai-talks-0.8.8.2/src/styles/menu_styles.py` & `ai-talks-0.8.8.8/src/styles/menu_styles.py`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.8.2/src/utils/conversation.py` & `ai-talks-0.8.8.8/src/utils/conversation.py`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.8.2/src/utils/footer.py` & `ai-talks-0.8.8.8/src/utils/footer.py`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.8.2/src/utils/helpers.py` & `ai-talks-0.8.8.8/src/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.8.2/src/utils/lang.py` & `ai-talks-0.8.8.8/src/utils/lang.py`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.8.2/src/utils/stt.py` & `ai-talks-0.8.8.8/src/utils/stt.py`

 * *Files identical despite different names*

