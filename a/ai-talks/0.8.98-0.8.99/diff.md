# Comparing `tmp/ai-talks-0.8.98.tar.gz` & `tmp/ai-talks-0.8.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-talks-0.8.98.tar", last modified: Sun Apr 16 00:26:55 2023, max compression
+gzip compressed data, was "ai-talks-0.8.99.tar", last modified: Sun Apr 16 00:30:39 2023, max compression
```

## Comparing `ai-talks-0.8.98.tar` & `ai-talks-0.8.99.tar`

### file list

```diff
@@ -1,17 +1,31 @@
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:26:55.301083 ai-talks-0.8.98/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1074 2023-04-09 09:49:53.000000 ai-talks-0.8.98/LICENSE
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     2748 2023-04-16 00:26:55.300551 ai-talks-0.8.98/PKG-INFO
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1939 2023-04-16 00:26:02.000000 ai-talks-0.8.98/README.md
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:26:55.298075 ai-talks-0.8.98/ai_talks.egg-info/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     2748 2023-04-16 00:26:55.000000 ai-talks-0.8.98/ai_talks.egg-info/PKG-INFO
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      275 2023-04-16 00:26:55.000000 ai-talks-0.8.98/ai_talks.egg-info/SOURCES.txt
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        1 2023-04-16 00:26:55.000000 ai-talks-0.8.98/ai_talks.egg-info/dependency_links.txt
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)       42 2023-04-16 00:26:55.000000 ai-talks-0.8.98/ai_talks.egg-info/entry_points.txt
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      167 2023-04-16 00:26:55.000000 ai-talks-0.8.98/ai_talks.egg-info/requires.txt
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        1 2023-04-16 00:26:55.000000 ai-talks-0.8.98/ai_talks.egg-info/top_level.txt
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      846 2023-04-09 19:26:49.000000 ai-talks-0.8.98/pyproject.toml
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)       38 2023-04-16 00:26:55.301310 ai-talks-0.8.98/setup.cfg
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1402 2023-04-16 00:26:02.000000 ai-talks-0.8.98/setup.py
-drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:26:55.299148 ai-talks-0.8.98/tests/
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.98/tests/__init__.py
--rw-r--r--   0 kosarevskiydp   (502) staff       (20)      180 2023-04-09 19:59:55.000000 ai-talks-0.8.98/tests/test_helpers.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:30:39.098869 ai-talks-0.8.99/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1074 2023-04-09 09:49:53.000000 ai-talks-0.8.99/LICENSE
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     2748 2023-04-16 00:30:39.098364 ai-talks-0.8.99/PKG-INFO
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1939 2023-04-16 00:26:02.000000 ai-talks-0.8.99/README.md
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:30:39.071014 ai-talks-0.8.99/ai-talks/
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:30:39.075834 ai-talks-0.8.99/ai-talks/src/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.99/ai-talks/src/__init__.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:30:39.076783 ai-talks-0.8.99/ai-talks/src/styles/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.99/ai-talks/src/styles/__init__.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      735 2023-03-23 21:57:52.000000 ai-talks-0.8.99/ai-talks/src/styles/menu_styles.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:30:39.087585 ai-talks-0.8.99/ai-talks/src/utils/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.99/ai-talks/src/utils/__init__.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     3695 2023-04-15 19:59:55.000000 ai-talks-0.8.99/ai-talks/src/utils/conversation.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1836 2023-04-16 00:24:55.000000 ai-talks-0.8.99/ai-talks/src/utils/footer.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      616 2023-04-09 19:46:48.000000 ai-talks-0.8.99/ai-talks/src/utils/helpers.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     7261 2023-04-15 22:07:51.000000 ai-talks-0.8.99/ai-talks/src/utils/lang.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     3672 2023-04-16 00:01:03.000000 ai-talks-0.8.99/ai-talks/src/utils/stt.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      416 2023-04-15 19:59:55.000000 ai-talks-0.8.99/ai-talks/src/utils/tts.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:30:39.096420 ai-talks-0.8.99/ai_talks.egg-info/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     2748 2023-04-16 00:30:38.000000 ai-talks-0.8.99/ai_talks.egg-info/PKG-INFO
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      571 2023-04-16 00:30:39.000000 ai-talks-0.8.99/ai_talks.egg-info/SOURCES.txt
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        1 2023-04-16 00:30:38.000000 ai-talks-0.8.99/ai_talks.egg-info/dependency_links.txt
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)       42 2023-04-16 00:30:38.000000 ai-talks-0.8.99/ai_talks.egg-info/entry_points.txt
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      167 2023-04-16 00:30:38.000000 ai-talks-0.8.99/ai_talks.egg-info/requires.txt
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        9 2023-04-16 00:30:38.000000 ai-talks-0.8.99/ai_talks.egg-info/top_level.txt
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      846 2023-04-09 19:26:49.000000 ai-talks-0.8.99/pyproject.toml
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)       38 2023-04-16 00:30:39.098997 ai-talks-0.8.99/setup.cfg
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)     1403 2023-04-16 00:30:36.000000 ai-talks-0.8.99/setup.py
+drwxr-xr-x   0 kosarevskiydp   (502) staff       (20)        0 2023-04-16 00:30:39.097761 ai-talks-0.8.99/tests/
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)        0 2023-03-22 15:12:34.000000 ai-talks-0.8.99/tests/__init__.py
+-rw-r--r--   0 kosarevskiydp   (502) staff       (20)      180 2023-04-09 19:59:55.000000 ai-talks-0.8.99/tests/test_helpers.py
```

### Comparing `ai-talks-0.8.98/LICENSE` & `ai-talks-0.8.99/LICENSE`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.98/PKG-INFO` & `ai-talks-0.8.99/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-talks
-Version: 0.8.98
+Version: 0.8.99
 Summary: A ChatGPT API wrapper, providing a user-friendly Streamlit web interface
 Home-page: https://github.com/dKosarevsky/AI-Talks
 Author: Dmitry Kosarevsky
 Author-email: if.kosarevsky@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ai-talks-0.8.98/README.md` & `ai-talks-0.8.99/README.md`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.98/ai_talks.egg-info/PKG-INFO` & `ai-talks-0.8.99/ai_talks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-talks
-Version: 0.8.98
+Version: 0.8.99
 Summary: A ChatGPT API wrapper, providing a user-friendly Streamlit web interface
 Home-page: https://github.com/dKosarevsky/AI-Talks
 Author: Dmitry Kosarevsky
 Author-email: if.kosarevsky@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ai-talks-0.8.98/pyproject.toml` & `ai-talks-0.8.99/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ai-talks-0.8.98/setup.py` & `ai-talks-0.8.99/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 # Read the contents of the requirements.txt file
 with open("requirements.txt") as f:
     requirements = [line.strip() for line in f.readlines() if not line.startswith("-f")]
 
 setup(
     name="ai-talks",
-    version="0.8.98",
+    version="0.8.99",
     exclude_package_data={"": ["secrets.toml"]},
-    packages=find_packages(exclude=["secrets.toml", ], include=["chat.py", ]),
+    packages=find_packages(exclude=["secrets.toml", ], include=["ai-talks.*"]),
     install_requires=requirements,  # Use the parsed requirements here
     entry_points={
         "console_scripts": [
             "ai-talks=chat:run_agi",
         ],
     },
     author="Dmitry Kosarevsky",
```

