# Comparing `tmp/ai-talks-0.8.8.8.8.tar.gz` & `tmp/ai-talks-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-talks-0.8.8.8.8.tar", last modified: Sun Apr 16 00:04:04 2023, max compression
+gzip compressed data, was "ai-talks-0.8.9.tar", last modified: Sun Apr 16 00:07:22 2023, max compression
```

## Comparing `ai-talks-0.8.8.8.8.tar` & `ai-talks-0.8.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:04:04.028201 ai-talks-0.8.8.8.8/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1074 2023-04-09 09:49:53.000000 ai-talks-0.8.8.8.8/LICENSE
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     2734 2023-04-16 00:04:04.027735 ai-talks-0.8.8.8.8/PKG-INFO
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1922 2023-04-15 19:25:22.000000 ai-talks-0.8.8.8.8/README.md
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:04:04.013652 ai-talks-0.8.8.8.8/ai_talks.egg-info/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     2734 2023-04-16 00:04:03.000000 ai-talks-0.8.8.8.8/ai_talks.egg-info/PKG-INFO
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      481 2023-04-16 00:04:03.000000 ai-talks-0.8.8.8.8/ai_talks.egg-info/SOURCES.txt
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        1 2023-04-16 00:04:03.000000 ai-talks-0.8.8.8.8/ai_talks.egg-info/dependency_links.txt
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)       42 2023-04-16 00:04:03.000000 ai-talks-0.8.8.8.8/ai_talks.egg-info/entry_points.txt
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      167 2023-04-16 00:04:03.000000 ai-talks-0.8.8.8.8/ai_talks.egg-info/requires.txt
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)       10 2023-04-16 00:04:03.000000 ai-talks-0.8.8.8.8/ai_talks.egg-info/top_level.txt
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      846 2023-04-09 19:26:49.000000 ai-talks-0.8.8.8.8/pyproject.toml
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)       38 2023-04-16 00:04:04.028326 ai-talks-0.8.8.8.8/setup.cfg
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1382 2023-04-16 00:04:01.000000 ai-talks-0.8.8.8.8/setup.py
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:04:04.014570 ai-talks-0.8.8.8.8/src/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.8.8.8/src/__init__.py
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:04:04.018239 ai-talks-0.8.8.8.8/src/styles/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.8.8.8/src/styles/__init__.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      735 2023-03-23 21:57:52.000000 ai-talks-0.8.8.8.8/src/styles/menu_styles.py
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:04:04.024573 ai-talks-0.8.8.8.8/src/utils/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.8.8.8/src/utils/__init__.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     3695 2023-04-15 19:59:55.000000 ai-talks-0.8.8.8.8/src/utils/conversation.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1797 2023-04-15 19:25:22.000000 ai-talks-0.8.8.8.8/src/utils/footer.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      616 2023-04-09 19:46:48.000000 ai-talks-0.8.8.8.8/src/utils/helpers.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     7261 2023-04-15 22:07:51.000000 ai-talks-0.8.8.8.8/src/utils/lang.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     3672 2023-04-16 00:01:03.000000 ai-talks-0.8.8.8.8/src/utils/stt.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      416 2023-04-15 19:59:55.000000 ai-talks-0.8.8.8.8/src/utils/tts.py
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:04:04.027001 ai-talks-0.8.8.8.8/tests/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.8.8.8/tests/__init__.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      180 2023-04-09 19:59:55.000000 ai-talks-0.8.8.8.8/tests/test_helpers.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:07:22.182547 ai-talks-0.8.9/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1074 2023-04-09 09:49:53.000000 ai-talks-0.8.9/LICENSE
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     2730 2023-04-16 00:07:22.182121 ai-talks-0.8.9/PKG-INFO
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1922 2023-04-15 19:25:22.000000 ai-talks-0.8.9/README.md
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:07:22.167618 ai-talks-0.8.9/ai_talks.egg-info/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     2730 2023-04-16 00:07:22.000000 ai-talks-0.8.9/ai_talks.egg-info/PKG-INFO
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      481 2023-04-16 00:07:22.000000 ai-talks-0.8.9/ai_talks.egg-info/SOURCES.txt
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        1 2023-04-16 00:07:22.000000 ai-talks-0.8.9/ai_talks.egg-info/dependency_links.txt
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)       42 2023-04-16 00:07:22.000000 ai-talks-0.8.9/ai_talks.egg-info/entry_points.txt
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      167 2023-04-16 00:07:22.000000 ai-talks-0.8.9/ai_talks.egg-info/requires.txt
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        1 2023-04-16 00:07:22.000000 ai-talks-0.8.9/ai_talks.egg-info/top_level.txt
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      846 2023-04-09 19:26:49.000000 ai-talks-0.8.9/pyproject.toml
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)       38 2023-04-16 00:07:22.182668 ai-talks-0.8.9/setup.cfg
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1401 2023-04-16 00:07:17.000000 ai-talks-0.8.9/setup.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:07:22.168213 ai-talks-0.8.9/src/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.9/src/__init__.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:07:22.169193 ai-talks-0.8.9/src/styles/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.9/src/styles/__init__.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      735 2023-03-23 21:57:52.000000 ai-talks-0.8.9/src/styles/menu_styles.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:07:22.178668 ai-talks-0.8.9/src/utils/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.9/src/utils/__init__.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     3695 2023-04-15 19:59:55.000000 ai-talks-0.8.9/src/utils/conversation.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1797 2023-04-15 19:25:22.000000 ai-talks-0.8.9/src/utils/footer.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      616 2023-04-09 19:46:48.000000 ai-talks-0.8.9/src/utils/helpers.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     7261 2023-04-15 22:07:51.000000 ai-talks-0.8.9/src/utils/lang.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     3672 2023-04-16 00:01:03.000000 ai-talks-0.8.9/src/utils/stt.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      416 2023-04-15 19:59:55.000000 ai-talks-0.8.9/src/utils/tts.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:07:22.180871 ai-talks-0.8.9/tests/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.9/tests/__init__.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      180 2023-04-09 19:59:55.000000 ai-talks-0.8.9/tests/test_helpers.py
```

### Comparing `ai-talks-0.8.8.8.8/LICENSE` & `ai-talks-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.8.8.8/PKG-INFO` & `ai-talks-0.8.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-talks
-Version: 0.8.8.8.8
+Version: 0.8.9
 Summary: A ChatGPT API wrapper, providing a user-friendly Streamlit web interface
 Home-page: https://github.com/dKosarevsky/AI-Talks
 Author: Dmitry Kosarevsky
 Author-email: if.kosarevsky@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ai-talks-0.8.8.8.8/README.md` & `ai-talks-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.8.8.8/ai_talks.egg-info/PKG-INFO` & `ai-talks-0.8.9/ai_talks.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-talks
-Version: 0.8.8.8.8
+Version: 0.8.9
 Summary: A ChatGPT API wrapper, providing a user-friendly Streamlit web interface
 Home-page: https://github.com/dKosarevsky/AI-Talks
 Author: Dmitry Kosarevsky
 Author-email: if.kosarevsky@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ai-talks-0.8.8.8.8/pyproject.toml` & `ai-talks-0.8.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.8.8.8/setup.py` & `ai-talks-0.8.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 # Read the contents of the requirements.txt file
 with open("requirements.txt") as f:
     requirements = [line.strip() for line in f.readlines() if not line.startswith("-f")]
 
 setup(
     name="ai-talks",
-    version="0.8.8.8.8",
+    version="0.8.9",
     exclude_package_data={"": ["secrets.toml"]},
-    packages=find_packages(exclude=["secrets.toml", ]),
+    packages=find_packages(exclude=["secrets.toml", ], include=["chat.py", ]),
     install_requires=requirements,  # Use the parsed requirements here
     entry_points={
         "console_scripts": [
             "ai-talks=chat:run_agi",
         ],
     },
     author="Dmitry Kosarevsky",
```

### Comparing `ai-talks-0.8.8.8.8/src/styles/menu_styles.py` & `ai-talks-0.8.9/src/styles/menu_styles.py`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.8.8.8/src/utils/conversation.py` & `ai-talks-0.8.9/src/utils/conversation.py`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.8.8.8/src/utils/footer.py` & `ai-talks-0.8.9/src/utils/footer.py`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.8.8.8/src/utils/helpers.py` & `ai-talks-0.8.9/src/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.8.8.8/src/utils/lang.py` & `ai-talks-0.8.9/src/utils/lang.py`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.8.8.8/src/utils/stt.py` & `ai-talks-0.8.9/src/utils/stt.py`

 * *Files identical despite different names*

