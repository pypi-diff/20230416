# Comparing `tmp/html4quiz-0.0.22.tar.gz` & `tmp/html4quiz-0.0.23.tar.gz`

## Comparing `html4quiz-0.0.22.tar` & `html4quiz-0.0.23.tar`

### file list

```diff
@@ -1,16 +1,23 @@
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 html4quiz-0.0.22/updatePackage.txt
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.22/src/html4quiz/__init__.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.22/src/html4quiz/_common.py
--rw-r--r--   0        0        0    26651 2020-02-02 00:00:00.000000 html4quiz-0.0.22/src/html4quiz/_generateEm.py
--rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.22/src/html4quiz/_scoreEm.py
--rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.22/src/html4quiz/makeChoices.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 html4quiz-0.0.22/src - 0.0.21/html4quiz/__init__.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 html4quiz-0.0.22/src - 0.0.21/html4quiz/_common.py
--rw-r--r--   0        0        0    11158 2020-02-02 00:00:00.000000 html4quiz-0.0.22/src - 0.0.21/html4quiz/_generateEm.py
--rw-r--r--   0        0        0    17875 2020-02-02 00:00:00.000000 html4quiz-0.0.22/src - 0.0.21/html4quiz/_generateMakeHTMLs.py
--rw-r--r--   0        0        0    10486 2020-02-02 00:00:00.000000 html4quiz-0.0.22/src - 0.0.21/html4quiz/_scoreEm.py
--rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.22/src - 0.0.21/html4quiz/makeChoices.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.22/LICENSE.txt
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 html4quiz-0.0.22/README.md
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 html4quiz-0.0.22/pyproject.toml
--rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 html4quiz-0.0.22/PKG-INFO
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 html4quiz-0.0.23/0.0.22README.md
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 html4quiz-0.0.23/0.0.22pyproject.toml
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 html4quiz-0.0.23/updatePackage.txt
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src/html4quiz/__init__.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src/html4quiz/_common.py
+-rw-r--r--   0        0        0    26651 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src/html4quiz/_generateEm.py
+-rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src/html4quiz/_scoreEm.py
+-rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src/html4quiz/makeChoices.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src - 0.0.21/html4quiz/__init__.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src - 0.0.21/html4quiz/_common.py
+-rw-r--r--   0        0        0    11158 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src - 0.0.21/html4quiz/_generateEm.py
+-rw-r--r--   0        0        0    17875 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src - 0.0.21/html4quiz/_generateMakeHTMLs.py
+-rw-r--r--   0        0        0    10486 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src - 0.0.21/html4quiz/_scoreEm.py
+-rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src - 0.0.21/html4quiz/makeChoices.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src - 0.0.22/html4quiz/__init__.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src - 0.0.22/html4quiz/_common.py
+-rw-r--r--   0        0        0    26651 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src - 0.0.22/html4quiz/_generateEm.py
+-rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src - 0.0.22/html4quiz/_scoreEm.py
+-rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.23/src - 0.0.22/html4quiz/makeChoices.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.23/LICENSE.txt
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 html4quiz-0.0.23/README.md
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 html4quiz-0.0.23/pyproject.toml
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 html4quiz-0.0.23/PKG-INFO
```

### Comparing `html4quiz-0.0.22/src/html4quiz/_common.py` & `html4quiz-0.0.23/src/html4quiz/_common.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.22/src/html4quiz/_generateEm.py` & `html4quiz-0.0.23/src/html4quiz/_generateEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.22/src/html4quiz/_scoreEm.py` & `html4quiz-0.0.23/src/html4quiz/_scoreEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.22/src/html4quiz/makeChoices.py` & `html4quiz-0.0.23/src/html4quiz/makeChoices.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.22/src - 0.0.21/html4quiz/_common.py` & `html4quiz-0.0.23/src - 0.0.21/html4quiz/_common.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.22/src - 0.0.21/html4quiz/_generateEm.py` & `html4quiz-0.0.23/src - 0.0.21/html4quiz/_generateEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.22/src - 0.0.21/html4quiz/_generateMakeHTMLs.py` & `html4quiz-0.0.23/src - 0.0.21/html4quiz/_generateMakeHTMLs.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.22/src - 0.0.21/html4quiz/_scoreEm.py` & `html4quiz-0.0.23/src - 0.0.21/html4quiz/_scoreEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.22/src - 0.0.21/html4quiz/makeChoices.py` & `html4quiz-0.0.23/src - 0.0.21/html4quiz/makeChoices.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.22/LICENSE.txt` & `html4quiz-0.0.23/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.22/README.md` & `html4quiz-0.0.23/0.0.22README.md`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.22/pyproject.toml` & `html4quiz-0.0.23/0.0.22pyproject.toml`

 * *Files identical despite different names*

