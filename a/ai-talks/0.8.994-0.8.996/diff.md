# Comparing `tmp/ai-talks-0.8.994.tar.gz` & `tmp/ai-talks-0.8.996.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-talks-0.8.994.tar", last modified: Sun Apr 16 00:47:30 2023, max compression
+gzip compressed data, was "ai-talks-0.8.996.tar", last modified: Sun Apr 16 00:49:18 2023, max compression
```

## Comparing `ai-talks-0.8.994.tar` & `ai-talks-0.8.996.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:47:30.664445 ai-talks-0.8.994/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1074 2023-04-09 09:49:53.000000 ai-talks-0.8.994/LICENSE
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     2749 2023-04-16 00:47:30.663396 ai-talks-0.8.994/PKG-INFO
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1939 2023-04-16 00:26:02.000000 ai-talks-0.8.994/README.md
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:47:30.614565 ai-talks-0.8.994/ai-talks/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:11:52.000000 ai-talks-0.8.994/ai-talks/__init__.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     4245 2023-04-15 23:59:36.000000 ai-talks-0.8.994/ai-talks/chat.py
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:47:30.616855 ai-talks-0.8.994/ai-talks/src/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.994/ai-talks/src/__init__.py
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:47:30.626797 ai-talks-0.8.994/ai-talks/src/styles/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.994/ai-talks/src/styles/__init__.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      735 2023-03-23 21:57:52.000000 ai-talks-0.8.994/ai-talks/src/styles/menu_styles.py
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:47:30.638484 ai-talks-0.8.994/ai-talks/src/utils/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.994/ai-talks/src/utils/__init__.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     3695 2023-04-15 19:59:55.000000 ai-talks-0.8.994/ai-talks/src/utils/conversation.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1836 2023-04-16 00:24:55.000000 ai-talks-0.8.994/ai-talks/src/utils/footer.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      616 2023-04-09 19:46:48.000000 ai-talks-0.8.994/ai-talks/src/utils/helpers.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     7261 2023-04-15 22:07:51.000000 ai-talks-0.8.994/ai-talks/src/utils/lang.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     3672 2023-04-16 00:01:03.000000 ai-talks-0.8.994/ai-talks/src/utils/stt.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      416 2023-04-15 19:59:55.000000 ai-talks-0.8.994/ai-talks/src/utils/tts.py
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:47:30.658397 ai-talks-0.8.994/ai_talks.egg-info/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     2749 2023-04-16 00:47:30.000000 ai-talks-0.8.994/ai_talks.egg-info/PKG-INFO
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      609 2023-04-16 00:47:30.000000 ai-talks-0.8.994/ai_talks.egg-info/SOURCES.txt
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        1 2023-04-16 00:47:30.000000 ai-talks-0.8.994/ai_talks.egg-info/dependency_links.txt
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)       51 2023-04-16 00:47:30.000000 ai-talks-0.8.994/ai_talks.egg-info/entry_points.txt
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      167 2023-04-16 00:47:30.000000 ai-talks-0.8.994/ai_talks.egg-info/requires.txt
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)       15 2023-04-16 00:47:30.000000 ai-talks-0.8.994/ai_talks.egg-info/top_level.txt
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      846 2023-04-09 19:26:49.000000 ai-talks-0.8.994/pyproject.toml
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)       38 2023-04-16 00:47:30.664712 ai-talks-0.8.994/setup.cfg
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1314 2023-04-16 00:47:22.000000 ai-talks-0.8.994/setup.py
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:47:30.661193 ai-talks-0.8.994/tests/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.994/tests/__init__.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      180 2023-04-09 19:59:55.000000 ai-talks-0.8.994/tests/test_helpers.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:49:18.050741 ai-talks-0.8.996/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1074 2023-04-09 09:49:53.000000 ai-talks-0.8.996/LICENSE
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     2749 2023-04-16 00:49:18.050097 ai-talks-0.8.996/PKG-INFO
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1939 2023-04-16 00:26:02.000000 ai-talks-0.8.996/README.md
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:49:18.030937 ai-talks-0.8.996/ai_talks/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:11:52.000000 ai-talks-0.8.996/ai_talks/__init__.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     4245 2023-04-15 23:59:36.000000 ai-talks-0.8.996/ai_talks/chat.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:49:18.035401 ai-talks-0.8.996/ai_talks/src/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.996/ai_talks/src/__init__.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:49:18.036403 ai-talks-0.8.996/ai_talks/src/styles/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.996/ai_talks/src/styles/__init__.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      735 2023-03-23 21:57:52.000000 ai-talks-0.8.996/ai_talks/src/styles/menu_styles.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:49:18.046224 ai-talks-0.8.996/ai_talks/src/utils/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.996/ai_talks/src/utils/__init__.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     3695 2023-04-15 19:59:55.000000 ai-talks-0.8.996/ai_talks/src/utils/conversation.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1836 2023-04-16 00:24:55.000000 ai-talks-0.8.996/ai_talks/src/utils/footer.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      616 2023-04-09 19:46:48.000000 ai-talks-0.8.996/ai_talks/src/utils/helpers.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     7261 2023-04-15 22:07:51.000000 ai-talks-0.8.996/ai_talks/src/utils/lang.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     3672 2023-04-16 00:01:03.000000 ai-talks-0.8.996/ai_talks/src/utils/stt.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      416 2023-04-15 19:59:55.000000 ai-talks-0.8.996/ai_talks/src/utils/tts.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:49:18.034838 ai-talks-0.8.996/ai_talks.egg-info/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     2749 2023-04-16 00:49:17.000000 ai-talks-0.8.996/ai_talks.egg-info/PKG-INFO
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      609 2023-04-16 00:49:17.000000 ai-talks-0.8.996/ai_talks.egg-info/SOURCES.txt
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        1 2023-04-16 00:49:17.000000 ai-talks-0.8.996/ai_talks.egg-info/dependency_links.txt
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)       51 2023-04-16 00:49:17.000000 ai-talks-0.8.996/ai_talks.egg-info/entry_points.txt
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      167 2023-04-16 00:49:17.000000 ai-talks-0.8.996/ai_talks.egg-info/requires.txt
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)       15 2023-04-16 00:49:17.000000 ai-talks-0.8.996/ai_talks.egg-info/top_level.txt
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      846 2023-04-09 19:26:49.000000 ai-talks-0.8.996/pyproject.toml
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)       38 2023-04-16 00:49:18.050912 ai-talks-0.8.996/setup.cfg
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1314 2023-04-16 00:49:15.000000 ai-talks-0.8.996/setup.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:49:18.048487 ai-talks-0.8.996/tests/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.996/tests/__init__.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      180 2023-04-09 19:59:55.000000 ai-talks-0.8.996/tests/test_helpers.py
```

### Comparing `ai-talks-0.8.994/LICENSE` & `ai-talks-0.8.996/LICENSE`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.994/PKG-INFO` & `ai-talks-0.8.996/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-talks
-Version: 0.8.994
+Version: 0.8.996
 Summary: A ChatGPT API wrapper, providing a user-friendly Streamlit web interface
 Home-page: https://github.com/dKosarevsky/AI-Talks
 Author: Dmitry Kosarevsky
 Author-email: if.kosarevsky@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ai-talks-0.8.994/README.md` & `ai-talks-0.8.996/README.md`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.994/ai-talks/chat.py` & `ai-talks-0.8.996/ai_talks/chat.py`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.994/ai-talks/src/styles/menu_styles.py` & `ai-talks-0.8.996/ai_talks/src/styles/menu_styles.py`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.994/ai-talks/src/utils/conversation.py` & `ai-talks-0.8.996/ai_talks/src/utils/conversation.py`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.994/ai-talks/src/utils/footer.py` & `ai-talks-0.8.996/ai_talks/src/utils/footer.py`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.994/ai-talks/src/utils/helpers.py` & `ai-talks-0.8.996/ai_talks/src/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.994/ai-talks/src/utils/lang.py` & `ai-talks-0.8.996/ai_talks/src/utils/lang.py`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.994/ai-talks/src/utils/stt.py` & `ai-talks-0.8.996/ai_talks/src/utils/stt.py`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.994/ai_talks.egg-info/PKG-INFO` & `ai-talks-0.8.996/ai_talks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-talks
-Version: 0.8.994
+Version: 0.8.996
 Summary: A ChatGPT API wrapper, providing a user-friendly Streamlit web interface
 Home-page: https://github.com/dKosarevsky/AI-Talks
 Author: Dmitry Kosarevsky
 Author-email: if.kosarevsky@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ai-talks-0.8.994/ai_talks.egg-info/SOURCES.txt` & `ai-talks-0.8.996/ai_talks.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
-ai-talks/__init__.py
-ai-talks/chat.py
-ai-talks/src/__init__.py
-ai-talks/src/styles/__init__.py
-ai-talks/src/styles/menu_styles.py
-ai-talks/src/utils/__init__.py
-ai-talks/src/utils/conversation.py
-ai-talks/src/utils/footer.py
-ai-talks/src/utils/helpers.py
-ai-talks/src/utils/lang.py
-ai-talks/src/utils/stt.py
-ai-talks/src/utils/tts.py
+ai_talks/__init__.py
+ai_talks/chat.py
 ai_talks.egg-info/PKG-INFO
 ai_talks.egg-info/SOURCES.txt
 ai_talks.egg-info/dependency_links.txt
 ai_talks.egg-info/entry_points.txt
 ai_talks.egg-info/requires.txt
 ai_talks.egg-info/top_level.txt
+ai_talks/src/__init__.py
+ai_talks/src/styles/__init__.py
+ai_talks/src/styles/menu_styles.py
+ai_talks/src/utils/__init__.py
+ai_talks/src/utils/conversation.py
+ai_talks/src/utils/footer.py
+ai_talks/src/utils/helpers.py
+ai_talks/src/utils/lang.py
+ai_talks/src/utils/stt.py
+ai_talks/src/utils/tts.py
 tests/__init__.py
 tests/test_helpers.py
```

### Comparing `ai-talks-0.8.994/pyproject.toml` & `ai-talks-0.8.996/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.994/setup.py` & `ai-talks-0.8.996/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of the requirements.txt file
 with open("requirements.txt") as f:
     requirements = [line.strip() for line in f.readlines() if not line.startswith("-f")]
 
 setup(
     name="ai-talks",
-    version="0.8.994",
+    version="0.8.996",
     packages=find_packages(),
     install_requires=requirements,  # Use the parsed requirements here
     entry_points={
         "console_scripts": [
             "ai-talks=ai_talks.chat:run_agi",
         ],
     },
```

