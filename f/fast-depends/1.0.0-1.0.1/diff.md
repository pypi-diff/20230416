# Comparing `tmp/fast_depends-1.0.0.tar.gz` & `tmp/fast_depends-1.0.1.tar.gz`

## Comparing `fast_depends-1.0.0.tar` & `fast_depends-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fast_depends-1.0.0/wtf.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-1.0.0/fast_depends/__about__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fast_depends-1.0.0/fast_depends/__init__.py
--rw-r--r--   0        0        0     7272 2020-02-02 00:00:00.000000 fast_depends-1.0.0/fast_depends/construct.py
--rw-r--r--   0        0        0     9960 2020-02-02 00:00:00.000000 fast_depends-1.0.0/fast_depends/injector.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 fast_depends-1.0.0/fast_depends/model.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fast_depends-1.0.0/fast_depends/provider.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 fast_depends-1.0.0/fast_depends/types.py
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 fast_depends-1.0.0/fast_depends/usage.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 fast_depends-1.0.0/fast_depends/utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-1.0.0/scripts/lint.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-1.0.0/scripts/publish.sh
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-1.0.0/scripts/test-cov.sh
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-1.0.0/scripts/test.sh
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fast_depends-1.0.0/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-1.0.0/LICENSE
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 fast_depends-1.0.0/README.md
--rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 fast_depends-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 fast_depends-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-1.0.1/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-1.0.1/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 fast_depends-1.0.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-1.0.1/fast_depends/__about__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fast_depends-1.0.1/fast_depends/__init__.py
+-rw-r--r--   0        0        0     7272 2020-02-02 00:00:00.000000 fast_depends-1.0.1/fast_depends/construct.py
+-rw-r--r--   0        0        0     9960 2020-02-02 00:00:00.000000 fast_depends-1.0.1/fast_depends/injector.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 fast_depends-1.0.1/fast_depends/model.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fast_depends-1.0.1/fast_depends/provider.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 fast_depends-1.0.1/fast_depends/types.py
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 fast_depends-1.0.1/fast_depends/usage.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 fast_depends-1.0.1/fast_depends/utils.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fast_depends-1.0.1/scripts/lint.sh
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-1.0.1/scripts/publish.sh
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-1.0.1/scripts/test-cov.sh
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-1.0.1/scripts/test.sh
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 fast_depends-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 fast_depends-1.0.1/README.md
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 fast_depends-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5803 2020-02-02 00:00:00.000000 fast_depends-1.0.1/PKG-INFO
```

### Comparing `fast_depends-1.0.0/fast_depends/construct.py` & `fast_depends-1.0.1/fast_depends/construct.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.0/fast_depends/injector.py` & `fast_depends-1.0.1/fast_depends/injector.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.0/fast_depends/model.py` & `fast_depends-1.0.1/fast_depends/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.0/fast_depends/usage.py` & `fast_depends-1.0.1/fast_depends/usage.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.0/LICENSE` & `fast_depends-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.0/pyproject.toml` & `fast_depends-1.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fast-depends"
-description = "FastDepends - extracted and cleared from HTTP domain Fastapi Dependency Injection System"
+description = "FastDepends - extracted and cleared from HTTP domain logic FastAPI Dependency Injection System. Async and sync are both supported."
 readme = "README.md"
 authors = [
     { name = "Pastukhov Nikita", email = "diementros@yandex.ru" },
 ]
 
 keywords = ["fastapi", "dependency injection"]
 
@@ -41,32 +41,31 @@
     "pydantic>=1.8",
     "anyio",
 ]
 
 dynamic = ["version"]
 
 [project.urls]
-Homepage = "https://lancetnik.github.io/FastDI/"
-Documentation = "https://lancetnik.github.io/FastDI/"
-Tracker = "https://github.com/Lancetnik/FastDI/issues"
-Source = "https://github.com/Lancetnik/FastDI"
+Homepage = "https://lancetnik.github.io/FastDepends/"
+Documentation = "https://lancetnik.github.io/FastDepends/"
+Tracker = "https://github.com/Lancetnik/FastDepends/issues"
+Source = "https://github.com/Lancetnik/FastDepends"
 
 [project.optional-dependencies]
 test = [
     "coverage[toml]>=7.2",
     "pytest>=7",
     "pytest-asyncio>=0.21",
     "pytest-xdist[psutil]",
 
     "asyncmock; python_version < '3.8'",
 ]
 
 doc = [
     "mkdocs-material >=8.1.4,<9.0.0",
-    "mkdocstrings[python]>=0.18",
     "mdx-include >=1.4.1,<2.0.0",
     "mkdocs-markdownextradata-plugin >=0.1.7,<0.3.0",
 ]
 
 dev = [
     "FastDepends[test]",
     "FastDepends[doc]",
@@ -152,15 +151,15 @@
 parallel = true
 branch = true
 concurrency = [
     "multiprocessing",
     "thread"
 ]
 source = [
-    "fastdi",
+    "fast_depends",
     "tests"
 ]
 context = '${CONTEXT}'
 omit = [
     "**/__init__.py",
 ]
```

