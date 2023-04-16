# Comparing `tmp/ai-talks-0.8.992.tar.gz` & `tmp/ai-talks-0.8.993.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-talks-0.8.992.tar", last modified: Sun Apr 16 00:37:27 2023, max compression
+gzip compressed data, was "ai-talks-0.8.993.tar", last modified: Sun Apr 16 00:41:08 2023, max compression
```

## Comparing `ai-talks-0.8.992.tar` & `ai-talks-0.8.993.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:37:27.618276 ai-talks-0.8.992/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1074 2023-04-09 09:49:53.000000 ai-talks-0.8.992/LICENSE
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     2749 2023-04-16 00:37:27.617367 ai-talks-0.8.992/PKG-INFO
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1939 2023-04-16 00:26:02.000000 ai-talks-0.8.992/README.md
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:37:27.591808 ai-talks-0.8.992/ai-talks/
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:37:27.596607 ai-talks-0.8.992/ai-talks/src/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.992/ai-talks/src/__init__.py
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:37:27.597942 ai-talks-0.8.992/ai-talks/src/styles/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.992/ai-talks/src/styles/__init__.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      735 2023-03-23 21:57:52.000000 ai-talks-0.8.992/ai-talks/src/styles/menu_styles.py
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:37:27.605544 ai-talks-0.8.992/ai-talks/src/utils/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.992/ai-talks/src/utils/__init__.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     3695 2023-04-15 19:59:55.000000 ai-talks-0.8.992/ai-talks/src/utils/conversation.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1836 2023-04-16 00:24:55.000000 ai-talks-0.8.992/ai-talks/src/utils/footer.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      616 2023-04-09 19:46:48.000000 ai-talks-0.8.992/ai-talks/src/utils/helpers.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     7261 2023-04-15 22:07:51.000000 ai-talks-0.8.992/ai-talks/src/utils/lang.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     3672 2023-04-16 00:01:03.000000 ai-talks-0.8.992/ai-talks/src/utils/stt.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      416 2023-04-15 19:59:55.000000 ai-talks-0.8.992/ai-talks/src/utils/tts.py
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:37:27.612384 ai-talks-0.8.992/ai_talks.egg-info/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     2749 2023-04-16 00:37:27.000000 ai-talks-0.8.992/ai_talks.egg-info/PKG-INFO
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      571 2023-04-16 00:37:27.000000 ai-talks-0.8.992/ai_talks.egg-info/SOURCES.txt
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        1 2023-04-16 00:37:27.000000 ai-talks-0.8.992/ai_talks.egg-info/dependency_links.txt
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)       42 2023-04-16 00:37:27.000000 ai-talks-0.8.992/ai_talks.egg-info/entry_points.txt
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      167 2023-04-16 00:37:27.000000 ai-talks-0.8.992/ai_talks.egg-info/requires.txt
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        1 2023-04-16 00:37:27.000000 ai-talks-0.8.992/ai_talks.egg-info/top_level.txt
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      846 2023-04-09 19:26:49.000000 ai-talks-0.8.992/pyproject.toml
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)       38 2023-04-16 00:37:27.618447 ai-talks-0.8.992/setup.cfg
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1336 2023-04-16 00:37:21.000000 ai-talks-0.8.992/setup.py
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:37:27.614526 ai-talks-0.8.992/tests/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.992/tests/__init__.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      180 2023-04-09 19:59:55.000000 ai-talks-0.8.992/tests/test_helpers.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:41:08.447320 ai-talks-0.8.993/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1074 2023-04-09 09:49:53.000000 ai-talks-0.8.993/LICENSE
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     2749 2023-04-16 00:41:08.446688 ai-talks-0.8.993/PKG-INFO
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1939 2023-04-16 00:26:02.000000 ai-talks-0.8.993/README.md
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:41:08.427938 ai-talks-0.8.993/ai-talks/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:11:52.000000 ai-talks-0.8.993/ai-talks/__init__.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     4245 2023-04-15 23:59:36.000000 ai-talks-0.8.993/ai-talks/chat.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:41:08.429295 ai-talks-0.8.993/ai-talks/src/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.993/ai-talks/src/__init__.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:41:08.430426 ai-talks-0.8.993/ai-talks/src/styles/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.993/ai-talks/src/styles/__init__.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      735 2023-03-23 21:57:52.000000 ai-talks-0.8.993/ai-talks/src/styles/menu_styles.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:41:08.436620 ai-talks-0.8.993/ai-talks/src/utils/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.993/ai-talks/src/utils/__init__.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     3695 2023-04-15 19:59:55.000000 ai-talks-0.8.993/ai-talks/src/utils/conversation.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1836 2023-04-16 00:24:55.000000 ai-talks-0.8.993/ai-talks/src/utils/footer.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      616 2023-04-09 19:46:48.000000 ai-talks-0.8.993/ai-talks/src/utils/helpers.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     7261 2023-04-15 22:07:51.000000 ai-talks-0.8.993/ai-talks/src/utils/lang.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     3672 2023-04-16 00:01:03.000000 ai-talks-0.8.993/ai-talks/src/utils/stt.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      416 2023-04-15 19:59:55.000000 ai-talks-0.8.993/ai-talks/src/utils/tts.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:41:08.444173 ai-talks-0.8.993/ai_talks.egg-info/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     2749 2023-04-16 00:41:08.000000 ai-talks-0.8.993/ai_talks.egg-info/PKG-INFO
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      609 2023-04-16 00:41:08.000000 ai-talks-0.8.993/ai_talks.egg-info/SOURCES.txt
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        1 2023-04-16 00:41:08.000000 ai-talks-0.8.993/ai_talks.egg-info/dependency_links.txt
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)       42 2023-04-16 00:41:08.000000 ai-talks-0.8.993/ai_talks.egg-info/entry_points.txt
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      167 2023-04-16 00:41:08.000000 ai-talks-0.8.993/ai_talks.egg-info/requires.txt
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)       15 2023-04-16 00:41:08.000000 ai-talks-0.8.993/ai_talks.egg-info/top_level.txt
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      846 2023-04-09 19:26:49.000000 ai-talks-0.8.993/pyproject.toml
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)       38 2023-04-16 00:41:08.447614 ai-talks-0.8.993/setup.cfg
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1305 2023-04-16 00:40:52.000000 ai-talks-0.8.993/setup.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:41:08.445685 ai-talks-0.8.993/tests/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.993/tests/__init__.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      180 2023-04-09 19:59:55.000000 ai-talks-0.8.993/tests/test_helpers.py
```

### Comparing `ai-talks-0.8.992/LICENSE` & `ai-talks-0.8.993/LICENSE`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.992/PKG-INFO` & `ai-talks-0.8.993/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-talks
-Version: 0.8.992
+Version: 0.8.993
 Summary: A ChatGPT API wrapper, providing a user-friendly Streamlit web interface
 Home-page: https://github.com/dKosarevsky/AI-Talks
 Author: Dmitry Kosarevsky
 Author-email: if.kosarevsky@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ai-talks-0.8.992/README.md` & `ai-talks-0.8.993/README.md`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.992/ai-talks/src/styles/menu_styles.py` & `ai-talks-0.8.993/ai-talks/src/styles/menu_styles.py`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.992/ai-talks/src/utils/conversation.py` & `ai-talks-0.8.993/ai-talks/src/utils/conversation.py`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.992/ai-talks/src/utils/footer.py` & `ai-talks-0.8.993/ai-talks/src/utils/footer.py`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.992/ai-talks/src/utils/helpers.py` & `ai-talks-0.8.993/ai-talks/src/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.992/ai-talks/src/utils/lang.py` & `ai-talks-0.8.993/ai-talks/src/utils/lang.py`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.992/ai-talks/src/utils/stt.py` & `ai-talks-0.8.993/ai-talks/src/utils/stt.py`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.992/ai_talks.egg-info/PKG-INFO` & `ai-talks-0.8.993/ai_talks.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-talks
-Version: 0.8.992
+Version: 0.8.993
 Summary: A ChatGPT API wrapper, providing a user-friendly Streamlit web interface
 Home-page: https://github.com/dKosarevsky/AI-Talks
 Author: Dmitry Kosarevsky
 Author-email: if.kosarevsky@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ai-talks-0.8.992/ai_talks.egg-info/SOURCES.txt` & `ai-talks-0.8.993/ai_talks.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
+ai-talks/__init__.py
+ai-talks/chat.py
 ai-talks/src/__init__.py
 ai-talks/src/styles/__init__.py
 ai-talks/src/styles/menu_styles.py
 ai-talks/src/utils/__init__.py
 ai-talks/src/utils/conversation.py
 ai-talks/src/utils/footer.py
 ai-talks/src/utils/helpers.py
```

### Comparing `ai-talks-0.8.992/pyproject.toml` & `ai-talks-0.8.993/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.992/setup.py` & `ai-talks-0.8.993/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 # Read the contents of the requirements.txt file
 with open("requirements.txt") as f:
     requirements = [line.strip() for line in f.readlines() if not line.startswith("-f")]
 
 setup(
     name="ai-talks",
-    version="0.8.992",
-    packages=find_packages(include=["ai-talks.*, chat.py"]),
+    version="0.8.993",
+    packages=find_packages(),
     install_requires=requirements,  # Use the parsed requirements here
     entry_points={
         "console_scripts": [
             "ai-talks=chat:run_agi",
         ],
     },
     author="Dmitry Kosarevsky",
```

