# Comparing `tmp/gameyamlspiderandgenerator-1.1.0.tar.gz` & `tmp/gameyamlspiderandgenerator-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameyamlspiderandgenerator-1.1.0.tar", max compression
+gzip compressed data, was "gameyamlspiderandgenerator-1.1.1.tar", max compression
```

## Comparing `gameyamlspiderandgenerator-1.1.0.tar` & `gameyamlspiderandgenerator-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     1069 2023-04-14 04:39:09.582935 gameyamlspiderandgenerator-1.1.0/LICENSE
--rwxr-xr-x   0        0        0      809 2023-04-14 04:39:09.583123 gameyamlspiderandgenerator-1.1.0/README.md
--rwxr-xr-x   0        0        0      610 2023-04-14 04:39:09.583410 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/__init__.py
--rwxr-xr-x   0        0        0      980 2023-04-14 04:39:09.583612 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/__main__.py
--rwxr-xr-x   0        0        0      753 2023-04-14 04:39:09.583800 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/exception.py
--rwxr-xr-x   0        0        0       52 2023-04-14 04:39:09.584087 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/hook/__init__.py
--rwxr-xr-x   0        0        0      194 2023-04-14 04:39:09.584282 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/hook/_base.py
--rwxr-xr-x   0        0        0     2365 2023-04-16 02:41:59.202807 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/hook/search.py
--rwxr-xr-x   0        0        0       56 2023-04-14 04:39:09.584827 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/plugin/__init__.py
--rwxr-xr-x   0        0        0     2406 2023-04-14 04:39:09.585063 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/plugin/_base.py
--rwxr-xr-x   0        0        0     6406 2023-04-16 03:52:20.134307 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/plugin/itchio.py
--rwxr-xr-x   0        0        0     7531 2023-04-16 03:03:23.223332 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/plugin/steam.py
--rwxr-xr-x   0        0        0        0 2023-04-14 04:39:09.585883 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/util/__init__.py
--rwxr-xr-x   0        0        0     1026 2023-04-16 02:34:35.477228 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/util/config.py
--rwxr-xr-x   0        0        0     1187 2023-04-16 02:34:35.339573 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/util/fgi.py
--rwxr-xr-x   0        0        0     1706 2023-04-16 02:46:20.126317 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/util/fgi_yaml.py
--rwxr-xr-x   0        0        0     1944 2023-04-16 02:40:43.137333 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/util/plugin_manager.py
--rwxr-xr-x   0        0        0     2611 2023-04-16 02:40:42.901945 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/util/spider.py
--rwxr-xr-x   0        0        0      617 2023-04-16 03:53:49.412367 gameyamlspiderandgenerator-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-04-14 04:39:09.582935 gameyamlspiderandgenerator-1.1.1/LICENSE
+-rwxr-xr-x   0        0        0      809 2023-04-14 04:39:09.583123 gameyamlspiderandgenerator-1.1.1/README.md
+-rwxr-xr-x   0        0        0      610 2023-04-14 04:39:09.583410 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/__init__.py
+-rwxr-xr-x   0        0        0      980 2023-04-14 04:39:09.583612 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/__main__.py
+-rwxr-xr-x   0        0        0      753 2023-04-14 04:39:09.583800 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/exception.py
+-rwxr-xr-x   0        0        0       52 2023-04-14 04:39:09.584087 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/hook/__init__.py
+-rwxr-xr-x   0        0        0      194 2023-04-14 04:39:09.584282 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/hook/_base.py
+-rwxr-xr-x   0        0        0     2365 2023-04-16 02:41:59.202807 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/hook/search.py
+-rwxr-xr-x   0        0        0       56 2023-04-14 04:39:09.584827 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/plugin/__init__.py
+-rwxr-xr-x   0        0        0     2406 2023-04-14 04:39:09.585063 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/plugin/_base.py
+-rwxr-xr-x   0        0        0     6406 2023-04-16 03:52:20.134307 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/plugin/itchio.py
+-rwxr-xr-x   0        0        0     7531 2023-04-16 03:03:23.223332 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/plugin/steam.py
+-rwxr-xr-x   0        0        0        0 2023-04-14 04:39:09.585883 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/util/__init__.py
+-rwxr-xr-x   0        0        0     1132 2023-04-16 04:31:11.710886 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/util/config.py
+-rwxr-xr-x   0        0        0     1187 2023-04-16 02:34:35.339573 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/util/fgi.py
+-rwxr-xr-x   0        0        0     1706 2023-04-16 02:46:20.126317 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/util/fgi_yaml.py
+-rwxr-xr-x   0        0        0     1944 2023-04-16 02:40:43.137333 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/util/plugin_manager.py
+-rwxr-xr-x   0        0        0     2611 2023-04-16 02:40:42.901945 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/util/spider.py
+-rwxr-xr-x   0        0        0      617 2023-04-16 04:31:41.930635 gameyamlspiderandgenerator-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.1.1/PKG-INFO
```

### Comparing `gameyamlspiderandgenerator-1.1.0/LICENSE` & `gameyamlspiderandgenerator-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.1.0/README.md` & `gameyamlspiderandgenerator-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/__init__.py` & `gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/__init__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/__main__.py` & `gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/__main__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/exception.py` & `gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/exception.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/hook/search.py` & `gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/hook/search.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/plugin/_base.py` & `gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/plugin/_base.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/plugin/itchio.py` & `gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/plugin/itchio.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/plugin/steam.py` & `gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/plugin/steam.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/util/config.py` & `gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/util/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,20 +13,23 @@
         # Compatibility with the old version
         return self.__getattribute__(item)
 
     def __setitem__(self, key, value):
         # Compatibility with the old version
         self.__setattr__(key, value)
 
-    def load(self, file_name: str | None):
-        if file_name is None:
+    def load(self, file_data: str | dict | None):
+        if type(file_data) is dict:
+            self.__dict__.update(file_data)
+            return
+        if file_data is None:
             self.__dict__.update(default_config)
             return
         try:
-            with open(file_name, "r", encoding="utf-8") as fp:
+            with open(file_data, "r", encoding="utf-8") as fp:
                 self.__dict__.update(fgi.load(fp))
         except Exception:
             raise ReadOrWriteConfigFailed from None
 
     def update(self, data: dict):
         self.__dict__.update(data)
```

### Comparing `gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/util/fgi.py` & `gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/util/fgi.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/util/fgi_yaml.py` & `gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/util/fgi_yaml.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/util/plugin_manager.py` & `gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/util/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/util/spider.py` & `gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/util/spider.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.1.0/pyproject.toml` & `gameyamlspiderandgenerator-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gameyamlspiderandgenerator"
-version = "1.1.0"
+version = "1.1.1"
 description = ""
 authors = ["kaesinol"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gameyamlspiderandgenerator-1.1.0/PKG-INFO` & `gameyamlspiderandgenerator-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gameyamlspiderandgenerator
-Version: 1.1.0
+Version: 1.1.1
 Summary: 
 License: MIT
 Author: kaesinol
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

