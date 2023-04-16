# Comparing `tmp/json5kit-0.3.1.tar.gz` & `tmp/json5kit-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json5kit-0.3.1.tar", last modified: Fri Apr 14 13:24:47 2023, max compression
+gzip compressed data, was "json5kit-0.3.2.tar", last modified: Sun Apr 16 15:01:46 2023, max compression
```

## Comparing `json5kit-0.3.1.tar` & `json5kit-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-04-14 13:24:47.501735 json5kit-0.3.1/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1072 2023-04-13 16:58:14.000000 json5kit-0.3.1/LICENSE
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2273 2023-04-14 13:24:47.501847 json5kit-0.3.1/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1415 2023-04-13 21:46:23.000000 json5kit-0.3.1/README.md
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1213 2023-04-14 13:24:47.502330 json5kit-0.3.1/setup.cfg
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       38 2023-04-13 16:58:14.000000 json5kit-0.3.1/setup.py
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-04-14 13:24:47.497236 json5kit-0.3.1/src/
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-04-14 13:24:47.500376 json5kit-0.3.1/src/json5kit/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)    11877 2023-04-14 13:21:37.000000 json5kit-0.3.1/src/json5kit/__init__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     7345 2023-04-14 13:19:22.000000 json5kit-0.3.1/src/json5kit/nodes.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3629 2023-04-13 21:44:53.000000 json5kit-0.3.1/src/json5kit/visitor.py
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-04-14 13:24:47.501567 json5kit-0.3.1/src/json5kit.egg-info/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2273 2023-04-14 13:24:47.000000 json5kit-0.3.1/src/json5kit.egg-info/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      286 2023-04-14 13:24:47.000000 json5kit-0.3.1/src/json5kit.egg-info/SOURCES.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2023-04-14 13:24:47.000000 json5kit-0.3.1/src/json5kit.egg-info/dependency_links.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       77 2023-04-14 13:24:47.000000 json5kit-0.3.1/src/json5kit.egg-info/requires.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        9 2023-04-14 13:24:47.000000 json5kit-0.3.1/src/json5kit.egg-info/top_level.txt
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-04-16 15:01:46.781928 json5kit-0.3.2/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1072 2023-04-13 16:58:14.000000 json5kit-0.3.2/LICENSE
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2273 2023-04-16 15:01:46.782038 json5kit-0.3.2/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1415 2023-04-13 21:46:23.000000 json5kit-0.3.2/README.md
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1213 2023-04-16 15:01:46.782484 json5kit-0.3.2/setup.cfg
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       38 2023-04-13 16:58:14.000000 json5kit-0.3.2/setup.py
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-04-16 15:01:46.779127 json5kit-0.3.2/src/
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-04-16 15:01:46.780733 json5kit-0.3.2/src/json5kit/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)    11877 2023-04-14 13:21:37.000000 json5kit-0.3.2/src/json5kit/__init__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     7422 2023-04-16 15:01:38.000000 json5kit-0.3.2/src/json5kit/nodes.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3629 2023-04-13 21:44:53.000000 json5kit-0.3.2/src/json5kit/visitor.py
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-04-16 15:01:46.781777 json5kit-0.3.2/src/json5kit.egg-info/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2273 2023-04-16 15:01:46.000000 json5kit-0.3.2/src/json5kit.egg-info/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      286 2023-04-16 15:01:46.000000 json5kit-0.3.2/src/json5kit.egg-info/SOURCES.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2023-04-16 15:01:46.000000 json5kit-0.3.2/src/json5kit.egg-info/dependency_links.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       77 2023-04-16 15:01:46.000000 json5kit-0.3.2/src/json5kit.egg-info/requires.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        9 2023-04-16 15:01:46.000000 json5kit-0.3.2/src/json5kit.egg-info/top_level.txt
```

### Comparing `json5kit-0.3.1/LICENSE` & `json5kit-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `json5kit-0.3.1/PKG-INFO` & `json5kit-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json5kit
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Roundtrip parser and CST for JSON, JSONC and JSON5.
 Home-page: https://github.com/tusharsadhwani/json5kit
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `json5kit-0.3.1/README.md` & `json5kit-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `json5kit-0.3.1/setup.cfg` & `json5kit-0.3.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = json5kit
-version = 0.3.1
+version = 0.3.2
 description = A Roundtrip parser and CST for JSON, JSONC and JSON5.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tusharsadhwani/json5kit
 author = Tushar Sadhwani
 author_email = tushar.sadhwani000@gmail.com
 license = MIT
```

### Comparing `json5kit-0.3.1/src/json5kit/__init__.py` & `json5kit-0.3.2/src/json5kit/__init__.py`

 * *Files identical despite different names*

### Comparing `json5kit-0.3.1/src/json5kit/nodes.py` & `json5kit-0.3.2/src/json5kit/nodes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from __future__ import annotations
 import sys
 
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing import Self
+
 if sys.version_info >= (3, 8):
-    from typing import Protocol, Self, runtime_checkable
+    from typing import Protocol, runtime_checkable
 else:
     from typing_extensions import Protocol, Self, runtime_checkable
 
 
 @runtime_checkable
 class Json5Node(Protocol):
     """Sets the expectation from a JSON5 node: be able to convert back to source."""
@@ -37,15 +42,15 @@
         return self.source + "".join(
             trivia.source for trivia in self.trailing_trivia_nodes
         )
 
     def to_json(self) -> str:
         return self.source
 
-    def replace(self, value: object) -> Self:
+    def replace(self, value: object) -> "Self":
         # TODO: pass specific source?
         source = str(value)
 
         primitive_class = type(self)
         return primitive_class(source, value, self.trailing_trivia_nodes.copy())
```

### Comparing `json5kit-0.3.1/src/json5kit/visitor.py` & `json5kit-0.3.2/src/json5kit/visitor.py`

 * *Files identical despite different names*

### Comparing `json5kit-0.3.1/src/json5kit.egg-info/PKG-INFO` & `json5kit-0.3.2/src/json5kit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json5kit
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Roundtrip parser and CST for JSON, JSONC and JSON5.
 Home-page: https://github.com/tusharsadhwani/json5kit
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

