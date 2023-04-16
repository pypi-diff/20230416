# Comparing `tmp/render_engine_microblog-2023.1.0a5.tar.gz` & `tmp/render_engine_microblog-2023.4.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render_engine_microblog-2023.1.0a5.tar", last modified: Thu Feb 23 05:40:39 2023, max compression
+gzip compressed data, was "render_engine_microblog-2023.4.1a5.tar", last modified: Sun Apr 16 21:52:11 2023, max compression
```

## Comparing `render_engine_microblog-2023.1.0a5.tar` & `render_engine_microblog-2023.4.1a5.tar`

### file list

```diff
@@ -1,18 +1,31 @@
-drwxr-xr-x   0 jaymiller   (501) staff       (20)        0 2023-02-23 05:40:39.134292 render_engine_microblog-2023.1.0a5/
--rw-r--r--   0 jaymiller   (501) staff       (20)     1066 2023-01-13 06:04:21.000000 render_engine_microblog-2023.1.0a5/LICENSE.md
--rw-r--r--   0 jaymiller   (501) staff       (20)     1767 2023-02-23 05:40:39.133996 render_engine_microblog-2023.1.0a5/PKG-INFO
--rw-r--r--   0 jaymiller   (501) staff       (20)     1392 2023-01-16 22:30:30.000000 render_engine_microblog-2023.1.0a5/README.md
--rw-r--r--   0 jaymiller   (501) staff       (20)      617 2023-02-23 05:40:07.000000 render_engine_microblog-2023.1.0a5/pyproject.toml
--rw-r--r--   0 jaymiller   (501) staff       (20)       38 2023-02-23 05:40:39.134348 render_engine_microblog-2023.1.0a5/setup.cfg
-drwxr-xr-x   0 jaymiller   (501) staff       (20)        0 2023-02-23 05:40:39.118739 render_engine_microblog-2023.1.0a5/src/
-drwxr-xr-x   0 jaymiller   (501) staff       (20)        0 2023-02-23 05:40:39.125794 render_engine_microblog-2023.1.0a5/src/render_engine_microblog/
--rw-r--r--   0 jaymiller   (501) staff       (20)       33 2023-01-16 22:39:21.000000 render_engine_microblog-2023.1.0a5/src/render_engine_microblog/__init__.py
--rw-r--r--   0 jaymiller   (501) staff       (20)      595 2023-02-23 04:40:41.000000 render_engine_microblog-2023.1.0a5/src/render_engine_microblog/collection.py
-drwxr-xr-x   0 jaymiller   (501) staff       (20)        0 2023-02-23 05:40:39.128496 render_engine_microblog-2023.1.0a5/src/render_engine_microblog.egg-info/
--rw-r--r--   0 jaymiller   (501) staff       (20)     1767 2023-02-23 05:40:39.000000 render_engine_microblog-2023.1.0a5/src/render_engine_microblog.egg-info/PKG-INFO
--rw-r--r--   0 jaymiller   (501) staff       (20)      396 2023-02-23 05:40:39.000000 render_engine_microblog-2023.1.0a5/src/render_engine_microblog.egg-info/SOURCES.txt
--rw-r--r--   0 jaymiller   (501) staff       (20)        1 2023-02-23 05:40:39.000000 render_engine_microblog-2023.1.0a5/src/render_engine_microblog.egg-info/dependency_links.txt
--rw-r--r--   0 jaymiller   (501) staff       (20)       52 2023-02-23 05:40:39.000000 render_engine_microblog-2023.1.0a5/src/render_engine_microblog.egg-info/requires.txt
--rw-r--r--   0 jaymiller   (501) staff       (20)       24 2023-02-23 05:40:39.000000 render_engine_microblog-2023.1.0a5/src/render_engine_microblog.egg-info/top_level.txt
-drwxr-xr-x   0 jaymiller   (501) staff       (20)        0 2023-02-23 05:40:39.133517 render_engine_microblog-2023.1.0a5/tests/
--rw-r--r--   0 jaymiller   (501) staff       (20)      502 2023-01-13 07:06:41.000000 render_engine_microblog-2023.1.0a5/tests/test_collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:52:11.578457 render_engine_microblog-2023.4.1a5/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:52:11.578457 render_engine_microblog-2023.4.1a5/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:52:11.578457 render_engine_microblog-2023.4.1a5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:52:11.578457 render_engine_microblog-2023.4.1a5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:52:11.578457 render_engine_microblog-2023.4.1a5/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-16 21:52:11.578457 render_engine_microblog-2023.4.1a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 21:52:11.578457 render_engine_microblog-2023.4.1a5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:52:11.578457 render_engine_microblog-2023.4.1a5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:52:11.578457 render_engine_microblog-2023.4.1a5/src/render_engine_microblog/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/src/render_engine_microblog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/src/render_engine_microblog/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:52:11.578457 render_engine_microblog-2023.4.1a5/src/render_engine_microblog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-16 21:52:11.000000 render_engine_microblog-2023.4.1a5/src/render_engine_microblog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-16 21:52:11.000000 render_engine_microblog-2023.4.1a5/src/render_engine_microblog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 21:52:11.000000 render_engine_microblog-2023.4.1a5/src/render_engine_microblog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-16 21:52:11.000000 render_engine_microblog-2023.4.1a5/src/render_engine_microblog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-16 21:52:11.000000 render_engine_microblog-2023.4.1a5/src/render_engine_microblog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:52:11.578457 render_engine_microblog-2023.4.1a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/tests/test_collection.py
```

### Comparing `render_engine_microblog-2023.1.0a5/LICENSE.md` & `render_engine_microblog-2023.4.1a5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `render_engine_microblog-2023.1.0a5/PKG-INFO` & `render_engine_microblog-2023.4.1a5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render_engine_microblog
-Version: 2023.1.0a5
+Version: 2023.4.1a5
 Summary: Microblog Parser and Collection for Render Engine
 Project-URL: homepage, https://github.com/kjaymiller/render_engine_microblog/
 Project-URL: repository, https://github.com/kjaymiller/render_engine_microblog/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
```

### Comparing `render_engine_microblog-2023.1.0a5/README.md` & `render_engine_microblog-2023.4.1a5/README.md`

 * *Files identical despite different names*

### Comparing `render_engine_microblog-2023.1.0a5/pyproject.toml` & `render_engine_microblog-2023.4.1a5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 [build-system]
-requires = ["setuptools", "wheel"]
+requires = ["setuptools", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "render_engine_microblog"
-version = "2023.1.0a5"
+dynamic = ["version"]
 description = "Microblog Parser and Collection for Render Engine"
 readme = "README.md"
 
 dependencies = [
-    "render-engine >= 2023.1.0a1",
+    "render-engine >= 2023.4.2a1",
 ]
 
 [project.optional-dependencies]
     dev = ["pytest", "pytest-mock"]
 
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 
+[tool.setuptools_scm]
+local_scheme = "no-local-version"
+
 [project.urls]
 homepage = "https://github.com/kjaymiller/render_engine_microblog/"
 repository = "https://github.com/kjaymiller/render_engine_microblog/"
 
 [tool.pytest.ini_options]
-pythonpath = ["src"]
+pythonpath = ["src"]
```

### Comparing `render_engine_microblog-2023.1.0a5/src/render_engine_microblog/collection.py` & `render_engine_microblog-2023.4.1a5/src/render_engine_microblog/collection.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 class MicroBlogPost(BlogPost):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.content = self._content
 
     @property
     def _slug(self):
-        base_date = parser.parse(self.date)
-        return base_date.strftime("%Y%m%d%H%M")
-
+        for attr in ["date_published", "date"]:
+            if getattr(self, attr, None):
+                return getattr(self, attr).strftime("%Y%m%d%H%M")
     @property    
     def _title(self):
         return ""
 
 class MicroBlog(Blog):
     template = "blog.html"
     PageParser = MarkdownPageParser
```

### Comparing `render_engine_microblog-2023.1.0a5/src/render_engine_microblog.egg-info/PKG-INFO` & `render_engine_microblog-2023.4.1a5/src/render_engine_microblog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render-engine-microblog
-Version: 2023.1.0a5
+Version: 2023.4.1a5
 Summary: Microblog Parser and Collection for Render Engine
 Project-URL: homepage, https://github.com/kjaymiller/render_engine_microblog/
 Project-URL: repository, https://github.com/kjaymiller/render_engine_microblog/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
```

