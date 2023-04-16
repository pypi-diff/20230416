# Comparing `tmp/html4quiz-0.0.23.tar.gz` & `tmp/html4quiz-0.0.24.tar.gz`

## Comparing `html4quiz-0.0.23.tar` & `html4quiz-0.0.24.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 html4quiz-0.0.23/0.0.22README.md
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 html4quiz-0.0.23/0.0.22pyproject.toml
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 html4quiz-0.0.23/updatePackage.txt
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src/html4quiz/__init__.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src/html4quiz/_common.py
--rw-r--r--   0        0        0    26651 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src/html4quiz/_generateEm.py
--rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src/html4quiz/_scoreEm.py
--rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src/html4quiz/makeChoices.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src - 0.0.21/html4quiz/__init__.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src - 0.0.21/html4quiz/_common.py
--rw-r--r--   0        0        0    11158 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src - 0.0.21/html4quiz/_generateEm.py
--rw-r--r--   0        0        0    17875 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src - 0.0.21/html4quiz/_generateMakeHTMLs.py
--rw-r--r--   0        0        0    10486 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src - 0.0.21/html4quiz/_scoreEm.py
--rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src - 0.0.21/html4quiz/makeChoices.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src - 0.0.22/html4quiz/__init__.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src - 0.0.22/html4quiz/_common.py
--rw-r--r--   0        0        0    26651 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src - 0.0.22/html4quiz/_generateEm.py
--rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src - 0.0.22/html4quiz/_scoreEm.py
--rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src - 0.0.22/html4quiz/makeChoices.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.23/LICENSE.txt
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 html4quiz-0.0.23/README.md
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 html4quiz-0.0.23/pyproject.toml
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 html4quiz-0.0.23/PKG-INFO
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 html4quiz-0.0.24/0.0.22README.md
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 html4quiz-0.0.24/0.0.22pyproject.toml
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 html4quiz-0.0.24/updatePackage.txt
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src/html4quiz/__init__.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src/html4quiz/_common.py
+-rw-r--r--   0        0        0    26651 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src/html4quiz/_generateEm.py
+-rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src/html4quiz/_scoreEm.py
+-rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src/html4quiz/makeChoices.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src - 0.0.21/html4quiz/__init__.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src - 0.0.21/html4quiz/_common.py
+-rw-r--r--   0        0        0    11158 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src - 0.0.21/html4quiz/_generateEm.py
+-rw-r--r--   0        0        0    17875 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src - 0.0.21/html4quiz/_generateMakeHTMLs.py
+-rw-r--r--   0        0        0    10486 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src - 0.0.21/html4quiz/_scoreEm.py
+-rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src - 0.0.21/html4quiz/makeChoices.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src - 0.0.22/html4quiz/__init__.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src - 0.0.22/html4quiz/_common.py
+-rw-r--r--   0        0        0    26651 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src - 0.0.22/html4quiz/_generateEm.py
+-rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src - 0.0.22/html4quiz/_scoreEm.py
+-rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.24/src - 0.0.22/html4quiz/makeChoices.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.24/LICENSE.txt
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 html4quiz-0.0.24/README.md
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 html4quiz-0.0.24/pyproject.toml
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 html4quiz-0.0.24/PKG-INFO
```

### Comparing `html4quiz-0.0.23/0.0.22README.md` & `html4quiz-0.0.24/0.0.22README.md`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.23/0.0.22pyproject.toml` & `html4quiz-0.0.24/0.0.22pyproject.toml`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.23/updatePackage.txt` & `html4quiz-0.0.24/updatePackage.txt`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.23/src/html4quiz/_common.py` & `html4quiz-0.0.24/src/html4quiz/_common.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.23/src/html4quiz/_generateEm.py` & `html4quiz-0.0.24/src/html4quiz/_generateEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.23/src/html4quiz/_scoreEm.py` & `html4quiz-0.0.24/src/html4quiz/_scoreEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.23/src/html4quiz/makeChoices.py` & `html4quiz-0.0.24/src/html4quiz/makeChoices.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.23/src - 0.0.21/html4quiz/_common.py` & `html4quiz-0.0.24/src - 0.0.21/html4quiz/_common.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.23/src - 0.0.21/html4quiz/_generateEm.py` & `html4quiz-0.0.24/src - 0.0.21/html4quiz/_generateEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.23/src - 0.0.21/html4quiz/_generateMakeHTMLs.py` & `html4quiz-0.0.24/src - 0.0.21/html4quiz/_generateMakeHTMLs.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.23/src - 0.0.21/html4quiz/_scoreEm.py` & `html4quiz-0.0.24/src - 0.0.21/html4quiz/_scoreEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.23/src - 0.0.21/html4quiz/makeChoices.py` & `html4quiz-0.0.24/src - 0.0.21/html4quiz/makeChoices.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.23/src - 0.0.22/html4quiz/_common.py` & `html4quiz-0.0.24/src - 0.0.22/html4quiz/_common.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.23/src - 0.0.22/html4quiz/_generateEm.py` & `html4quiz-0.0.24/src - 0.0.22/html4quiz/_generateEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.23/src - 0.0.22/html4quiz/_scoreEm.py` & `html4quiz-0.0.24/src - 0.0.22/html4quiz/_scoreEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.23/src - 0.0.22/html4quiz/makeChoices.py` & `html4quiz-0.0.24/src - 0.0.22/html4quiz/makeChoices.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.23/LICENSE.txt` & `html4quiz-0.0.24/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.23/pyproject.toml` & `html4quiz-0.0.24/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "html4quiz"
-version = "0.0.23"
+version = "0.0.24"
 authors = [
   { name="Sukmock Lee", email="smlee@inha.ac.kr" },
 ]
 description = "A package that generates questionnaires as HTML files to be distributed over the network and scores answers in text files submitted by students."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -21,8 +21,8 @@
     "Development Status :: 4 - Beta"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/generateNscore/html4quiz"
 "Bug Tracker" = "https://github.com/generateNscore/html4quiz/issues"
 "Documentation" = "https://github.com/generateNscore/html4quiz/wiki"
-"Source" = "https://github.com/generateNscore/html4quiz"
+"readme" = "https://github.com/generateNscore/html4quiz/blob/main/README.md"
```

### Comparing `html4quiz-0.0.23/PKG-INFO` & `html4quiz-0.0.24/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: html4quiz
-Version: 0.0.23
+Version: 0.0.24
 Summary: A package that generates questionnaires as HTML files to be distributed over the network and scores answers in text files submitted by students.
 Project-URL: Homepage, https://github.com/generateNscore/html4quiz
 Project-URL: Bug Tracker, https://github.com/generateNscore/html4quiz/issues
 Project-URL: Documentation, https://github.com/generateNscore/html4quiz/wiki
-Project-URL: Source, https://github.com/generateNscore/html4quiz
+Project-URL: readme, https://github.com/generateNscore/html4quiz/blob/main/README.md
 Author-email: Sukmock Lee <smlee@inha.ac.kr>
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,19 +18,10 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # html4quiz
 
 ## What is it?
 
-html4quiz is a package that helps you generates question sheets with as many HTML files as you want and allows you to grade answers from text files submitted by students.
+html4quiz is a package that helps you generate question sheets with as many HTML files as you want and allows you to score answers in text files submitted by students.
 
-## Description
-<ul>
-<li><a href="https://github.com/generateNscore/html4quiz/blob/main/README.md">READMe</a></li>
-</ul>
-
-
-## Help
-<ul>
-<li><a href="https://github.com/generateNscore/html4quiz/wiki">Documentation</a></li>
-</ul>
+## <a href="https://github.com/generateNscore/html4quiz/blob/main/README.md">READMe</a>
```

#### html2text {}

```diff
@@ -1,19 +1,17 @@
-Metadata-Version: 2.1 Name: html4quiz Version: 0.0.23 Summary: A package that
+Metadata-Version: 2.1 Name: html4quiz Version: 0.0.24 Summary: A package that
 generates questionnaires as HTML files to be distributed over the network and
 scores answers in text files submitted by students. Project-URL: Homepage,
 https://github.com/generateNscore/html4quiz Project-URL: Bug Tracker, https://
 github.com/generateNscore/html4quiz/issues Project-URL: Documentation, https://
-github.com/generateNscore/html4quiz/wiki Project-URL: Source, https://
-github.com/generateNscore/html4quiz Author-email: Sukmock Lee
+github.com/generateNscore/html4quiz/wiki Project-URL: readme, https://
+github.com/generateNscore/html4quiz/blob/main/README.md Author-email: Sukmock
+Lee
 inha.ac.kr> License-File: LICENSE.txt Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Education Classifier: Intended Audience
 :: End Users/Desktop Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Topic :: Education :: Testing Requires-Python: >=3.7
 Description-Content-Type: text/markdown # html4quiz ## What is it? html4quiz is
-a package that helps you generates question sheets with as many HTML files as
-you want and allows you to grade answers from text files submitted by students.
-## Description
-    * READMe
-## Help
-    * Documentation
+a package that helps you generate question sheets with as many HTML files as
+you want and allows you to score answers in text files submitted by students.
+## READMe
```

