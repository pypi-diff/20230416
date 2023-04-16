# Comparing `tmp/pdbr-0.8.4.tar.gz` & `tmp/pdbr-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdbr-0.8.4.tar", max compression
+gzip compressed data, was "pdbr-0.8.5.tar", max compression
```

## Comparing `pdbr-0.8.4.tar` & `pdbr-0.8.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-04-13 15:22:51.909584 pdbr-0.8.4/LICENSE
--rw-r--r--   0        0        0     6273 2023-04-13 15:22:51.909584 pdbr-0.8.4/README.md
--rw-r--r--   0        0        0      286 2023-04-13 15:22:51.921584 pdbr-0.8.4/pdbr/__init__.py
--rw-r--r--   0        0        0     1239 2023-04-13 15:22:51.921584 pdbr-0.8.4/pdbr/__main__.py
--rw-r--r--   0        0        0     1206 2023-04-13 15:22:51.921584 pdbr-0.8.4/pdbr/_cm.py
--rw-r--r--   0        0        0     1485 2023-04-13 15:22:51.921584 pdbr-0.8.4/pdbr/_console_layout.py
--rw-r--r--   0        0        0    15974 2023-04-13 15:22:51.921584 pdbr-0.8.4/pdbr/_pdbr.py
--rw-r--r--   0        0        0     1306 2023-04-13 15:22:51.921584 pdbr-0.8.4/pdbr/cli.py
--rw-r--r--   0        0        0     1421 2023-04-13 15:22:51.921584 pdbr-0.8.4/pdbr/helpers.py
--rw-r--r--   0        0        0        0 2023-04-13 15:22:51.921584 pdbr-0.8.4/pdbr/middlewares/__init__.py
--rw-r--r--   0        0        0      492 2023-04-13 15:22:51.921584 pdbr-0.8.4/pdbr/middlewares/django.py
--rw-r--r--   0        0        0      334 2023-04-13 15:22:51.921584 pdbr-0.8.4/pdbr/middlewares/starlette.py
--rw-r--r--   0        0        0      782 2023-04-13 15:22:51.921584 pdbr-0.8.4/pdbr/runner.py
--rw-r--r--   0        0        0     3242 2023-04-13 15:22:51.921584 pdbr-0.8.4/pdbr/utils.py
--rw-r--r--   0        0        0     1762 2023-04-13 15:22:51.921584 pdbr-0.8.4/pyproject.toml
--rw-r--r--   0        0        0     7608 1970-01-01 00:00:00.000000 pdbr-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-16 13:52:29.197787 pdbr-0.8.5/LICENSE
+-rw-r--r--   0        0        0     6273 2023-04-16 13:52:29.201787 pdbr-0.8.5/README.md
+-rw-r--r--   0        0        0      286 2023-04-16 13:52:29.209787 pdbr-0.8.5/pdbr/__init__.py
+-rw-r--r--   0        0        0     1239 2023-04-16 13:52:29.209787 pdbr-0.8.5/pdbr/__main__.py
+-rw-r--r--   0        0        0     1206 2023-04-16 13:52:29.209787 pdbr-0.8.5/pdbr/_cm.py
+-rw-r--r--   0        0        0     1485 2023-04-16 13:52:29.209787 pdbr-0.8.5/pdbr/_console_layout.py
+-rw-r--r--   0        0        0    16695 2023-04-16 13:52:29.209787 pdbr-0.8.5/pdbr/_pdbr.py
+-rw-r--r--   0        0        0     1306 2023-04-16 13:52:29.209787 pdbr-0.8.5/pdbr/cli.py
+-rw-r--r--   0        0        0     1421 2023-04-16 13:52:29.209787 pdbr-0.8.5/pdbr/helpers.py
+-rw-r--r--   0        0        0        0 2023-04-16 13:52:29.209787 pdbr-0.8.5/pdbr/middlewares/__init__.py
+-rw-r--r--   0        0        0      492 2023-04-16 13:52:29.209787 pdbr-0.8.5/pdbr/middlewares/django.py
+-rw-r--r--   0        0        0      334 2023-04-16 13:52:29.209787 pdbr-0.8.5/pdbr/middlewares/starlette.py
+-rw-r--r--   0        0        0      782 2023-04-16 13:52:29.209787 pdbr-0.8.5/pdbr/runner.py
+-rw-r--r--   0        0        0     3242 2023-04-16 13:52:29.209787 pdbr-0.8.5/pdbr/utils.py
+-rw-r--r--   0        0        0     1762 2023-04-16 13:52:29.209787 pdbr-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0     7608 1970-01-01 00:00:00.000000 pdbr-0.8.5/PKG-INFO
```

### Comparing `pdbr-0.8.4/LICENSE` & `pdbr-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.4/README.md` & `pdbr-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.4/pdbr/__main__.py` & `pdbr-0.8.5/pdbr/__main__.py`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.4/pdbr/_cm.py` & `pdbr-0.8.5/pdbr/_cm.py`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.4/pdbr/_console_layout.py` & `pdbr-0.8.5/pdbr/_console_layout.py`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.4/pdbr/_pdbr.py` & `pdbr-0.8.5/pdbr/_pdbr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import inspect
 import io
 import re
-from inspect import getsourcelines
 from pathlib import Path
 from pdb import Pdb
 
 import sqlparse
 from rich import box, markup
 from rich._inspect import Inspect
 from rich.console import Console
@@ -121,17 +120,16 @@
                     style="warning",
                     print_layout=False,
                 )
 
         do_help.__doc__ = base.do_help.__doc__
         do_h = do_help
 
-        def _get_syntax_for_list(self, with_line_range=False):
-            line_range = None
-            if with_line_range:
+        def _get_syntax_for_list(self, line_range=None):
+            if not line_range:
                 first = max(1, self.curframe.f_lineno - 5)
                 line_range = first, first + 10
             filename = self.curframe.f_code.co_filename
             highlight_lines = {self.curframe.f_lineno}
 
             return Syntax.from_path(
                 filename,
@@ -152,59 +150,80 @@
                 return []
 
         def do_l(self, arg):
             """l
             List 11 lines source code for the current file.
             """
             try:
-                self._print(
-                    self._get_syntax_for_list(with_line_range=True), print_layout=False
-                )
+                self._print(self._get_syntax_for_list(), print_layout=False)
             except BaseException:
                 self.error("could not get source code")
 
         def do_longlist(self, arg):
             """longlist | ll
             List the whole source code for the current function or frame.
             """
             try:
-                self._print(self._get_syntax_for_list(), print_layout=False)
+                lines, lineno = self._getsourcelines(self.curframe)
+                last = lineno + len(lines)
+                self._print(
+                    self._get_syntax_for_list((lineno, last)), print_layout=False
+                )
             except BaseException:
                 self.error("could not get source code")
 
         do_ll = do_longlist
 
+        def do_source(self, arg):
+            """source expression
+            Try to get source code for the given object and display it.
+            """
+            try:
+                obj = self._getval(arg)
+                lines, lineno = self._getsourcelines(obj)
+                last = lineno + len(lines)
+                self._print(
+                    self._get_syntax_for_list((lineno, last)), print_layout=False
+                )
+            except BaseException as err:
+                self.error(err)
+
         def do_search(self, arg):
             """search | src
             Search a phrase in the current frame.
             In order to repeat the last one, type `/` character as arg.
             """
             if not arg or (arg == "/" and not self._latest_search_arg):
                 self.error("Search failed: arg is missing")
                 return
 
             if arg == "/":
                 arg = self._latest_search_arg
             else:
                 self._latest_search_arg = arg
 
-            lines, lineno = getsourcelines(self.curframe)
+            lines, lineno = self._getsourcelines(self.curframe)
             indexes = [index for index, line in enumerate(lines, lineno) if arg in line]
 
             if len(indexes) > 0:
                 bigger_indexes = [
                     index for index in indexes if index > self.curframe.f_lineno
                 ]
                 next_line = bigger_indexes[0] if bigger_indexes else indexes[0]
                 return super().do_jump(next_line)
             else:
                 self.error(f"Search failed: '{arg}' not found")
 
         do_src = do_search
 
+        def _getsourcelines(self, obj):
+            lines, lineno = inspect.getsourcelines(obj)
+            lineno = max(1, lineno)
+            return lines, lineno
+
         def get_varstable(self):
             variables = self._get_variables()
             if not variables:
                 return
             table = Table(title="List of local variables", box=box.MINIMAL)
 
             table.add_column("Variable", style="cyan")
```

### Comparing `pdbr-0.8.4/pdbr/cli.py` & `pdbr-0.8.5/pdbr/cli.py`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.4/pdbr/helpers.py` & `pdbr-0.8.5/pdbr/helpers.py`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.4/pdbr/runner.py` & `pdbr-0.8.5/pdbr/runner.py`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.4/pdbr/utils.py` & `pdbr-0.8.5/pdbr/utils.py`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.4/pyproject.toml` & `pdbr-0.8.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdbr"
-version = "0.8.4"
+version = "0.8.5"
 description = "Pdb with Rich library."
 authors = ["Can Sarigol <ertugrulsarigol@gmail.com>"]
 packages = [
     { include = "pdbr" }
 ]
 readme = "README.md"
 homepage = "https://github.com/cansarigol/pdbr"
@@ -52,15 +52,15 @@
 min_confidence = 80
 paths = ["pdbr", "tests"]
 sort_by_size = true
 verbose = false
 
 [project]
 name = "pdbr"
-version = "0.8.4"
+version = "0.8.5"
 
 [tool.setuptools]
 py-modules = []
 
 [tool.ruff]
 select = [
     "E",  # pycodestyle errors
```

### Comparing `pdbr-0.8.4/PKG-INFO` & `pdbr-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbr
-Version: 0.8.4
+Version: 0.8.5
 Summary: Pdb with Rich library.
 Home-page: https://github.com/cansarigol/pdbr
 Author: Can Sarigol
 Author-email: ertugrulsarigol@gmail.com
 Requires-Python: >=3.7.9,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

