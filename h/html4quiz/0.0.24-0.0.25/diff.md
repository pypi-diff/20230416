# Comparing `tmp/html4quiz-0.0.24.tar.gz` & `tmp/html4quiz-0.0.25.tar.gz`

## Comparing `html4quiz-0.0.24.tar` & `html4quiz-0.0.25.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 html4quiz-0.0.24/0.0.22README.md
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 html4quiz-0.0.24/0.0.22pyproject.toml
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 html4quiz-0.0.24/updatePackage.txt
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src/html4quiz/__init__.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src/html4quiz/_common.py
--rw-r--r--   0        0        0    26651 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src/html4quiz/_generateEm.py
--rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src/html4quiz/_scoreEm.py
--rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src/html4quiz/makeChoices.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src - 0.0.21/html4quiz/__init__.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src - 0.0.21/html4quiz/_common.py
--rw-r--r--   0        0        0    11158 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src - 0.0.21/html4quiz/_generateEm.py
--rw-r--r--   0        0        0    17875 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src - 0.0.21/html4quiz/_generateMakeHTMLs.py
--rw-r--r--   0        0        0    10486 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src - 0.0.21/html4quiz/_scoreEm.py
--rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src - 0.0.21/html4quiz/makeChoices.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src - 0.0.22/html4quiz/__init__.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src - 0.0.22/html4quiz/_common.py
--rw-r--r--   0        0        0    26651 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src - 0.0.22/html4quiz/_generateEm.py
--rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src - 0.0.22/html4quiz/_scoreEm.py
--rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src - 0.0.22/html4quiz/makeChoices.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.24/LICENSE.txt
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 html4quiz-0.0.24/README.md
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 html4quiz-0.0.24/pyproject.toml
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 html4quiz-0.0.24/PKG-INFO
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 html4quiz-0.0.25/0.0.22README.md
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 html4quiz-0.0.25/0.0.22pyproject.toml
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 html4quiz-0.0.25/README.md
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 html4quiz-0.0.25/updatePackage.txt
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.25/src/html4quiz/__init__.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.25/src/html4quiz/_common.py
+-rw-r--r--   0        0        0    26651 2020-02-02 00:00:00.000000 html4quiz-0.0.25/src/html4quiz/_generateEm.py
+-rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.25/src/html4quiz/_scoreEm.py
+-rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.25/src/html4quiz/makeChoices.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 html4quiz-0.0.25/src - 0.0.21/html4quiz/__init__.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 html4quiz-0.0.25/src - 0.0.21/html4quiz/_common.py
+-rw-r--r--   0        0        0    11158 2020-02-02 00:00:00.000000 html4quiz-0.0.25/src - 0.0.21/html4quiz/_generateEm.py
+-rw-r--r--   0        0        0    17875 2020-02-02 00:00:00.000000 html4quiz-0.0.25/src - 0.0.21/html4quiz/_generateMakeHTMLs.py
+-rw-r--r--   0        0        0    10486 2020-02-02 00:00:00.000000 html4quiz-0.0.25/src - 0.0.21/html4quiz/_scoreEm.py
+-rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.25/src - 0.0.21/html4quiz/makeChoices.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.25/src - 0.0.22/html4quiz/__init__.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.25/src - 0.0.22/html4quiz/_common.py
+-rw-r--r--   0        0        0    26651 2020-02-02 00:00:00.000000 html4quiz-0.0.25/src - 0.0.22/html4quiz/_generateEm.py
+-rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.25/src - 0.0.22/html4quiz/_scoreEm.py
+-rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.25/src - 0.0.22/html4quiz/makeChoices.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.25/LICENSE.txt
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 html4quiz-0.0.25/pyproject.toml
+-rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 GitHub/html4quiz/README.md
+-rw-r--r--   0        0        0     5345 2020-02-02 00:00:00.000000 html4quiz-0.0.25/PKG-INFO
```

### Comparing `html4quiz-0.0.24/0.0.22README.md` & `html4quiz-0.0.25/0.0.22README.md`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.24/0.0.22pyproject.toml` & `html4quiz-0.0.25/0.0.22pyproject.toml`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.24/updatePackage.txt` & `html4quiz-0.0.25/updatePackage.txt`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.24/src/html4quiz/_common.py` & `html4quiz-0.0.25/src/html4quiz/_common.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.24/src/html4quiz/_generateEm.py` & `html4quiz-0.0.25/src/html4quiz/_generateEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.24/src/html4quiz/_scoreEm.py` & `html4quiz-0.0.25/src/html4quiz/_scoreEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.24/src/html4quiz/makeChoices.py` & `html4quiz-0.0.25/src/html4quiz/makeChoices.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.24/src - 0.0.21/html4quiz/_common.py` & `html4quiz-0.0.25/src - 0.0.21/html4quiz/_common.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.24/src - 0.0.21/html4quiz/_generateEm.py` & `html4quiz-0.0.25/src - 0.0.21/html4quiz/_generateEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.24/src - 0.0.21/html4quiz/_generateMakeHTMLs.py` & `html4quiz-0.0.25/src - 0.0.21/html4quiz/_generateMakeHTMLs.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.24/src - 0.0.21/html4quiz/_scoreEm.py` & `html4quiz-0.0.25/src - 0.0.21/html4quiz/_scoreEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.24/src - 0.0.21/html4quiz/makeChoices.py` & `html4quiz-0.0.25/src - 0.0.21/html4quiz/makeChoices.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.24/src - 0.0.22/html4quiz/_common.py` & `html4quiz-0.0.25/src - 0.0.22/html4quiz/_common.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.24/src - 0.0.22/html4quiz/_generateEm.py` & `html4quiz-0.0.25/src - 0.0.22/html4quiz/_generateEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.24/src - 0.0.22/html4quiz/_scoreEm.py` & `html4quiz-0.0.25/src - 0.0.22/html4quiz/_scoreEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.24/src - 0.0.22/html4quiz/makeChoices.py` & `html4quiz-0.0.25/src - 0.0.22/html4quiz/makeChoices.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.24/LICENSE.txt` & `html4quiz-0.0.25/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.24/pyproject.toml` & `html4quiz-0.0.25/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "html4quiz"
-version = "0.0.24"
+version = "0.0.25"
 authors = [
   { name="Sukmock Lee", email="smlee@inha.ac.kr" },
 ]
 description = "A package that generates questionnaires as HTML files to be distributed over the network and scores answers in text files submitted by students."
-readme = "README.md"
+readme = "D:\\GitHub\\html4quiz\\README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Topic :: Education :: Testing",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Education",
@@ -21,8 +21,8 @@
     "Development Status :: 4 - Beta"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/generateNscore/html4quiz"
 "Bug Tracker" = "https://github.com/generateNscore/html4quiz/issues"
 "Documentation" = "https://github.com/generateNscore/html4quiz/wiki"
-"readme" = "https://github.com/generateNscore/html4quiz/blob/main/README.md"
+
```

