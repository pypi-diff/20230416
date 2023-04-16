# Comparing `tmp/pylint_keyword_only_args_plugin-0.2.2.tar.gz` & `tmp/pylint_keyword_only_args_plugin-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylint_keyword_only_args_plugin-0.2.2.tar", max compression
+gzip compressed data, was "pylint_keyword_only_args_plugin-0.2.3.tar", max compression
```

## Comparing `pylint_keyword_only_args_plugin-0.2.2.tar` & `pylint_keyword_only_args_plugin-0.2.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      410 2023-04-15 06:23:07.303291 pylint_keyword_only_args_plugin-0.2.2/README.md
--rw-r--r--   0        0        0       71 2023-04-14 02:31:08.436703 pylint_keyword_only_args_plugin-0.2.2/pylint_keyword_only_args_plugin/__init__.py
--rw-r--r--   0        0        0     1455 2023-04-15 06:37:14.205163 pylint_keyword_only_args_plugin-0.2.2/pylint_keyword_only_args_plugin/checker.py
--rw-r--r--   0        0        0      159 2023-04-14 02:30:27.305357 pylint_keyword_only_args_plugin-0.2.2/pylint_keyword_only_args_plugin/keyword_only_args.py
--rw-r--r--   0        0        0     1025 2023-04-15 06:38:24.538133 pylint_keyword_only_args_plugin-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1302 1970-01-01 00:00:00.000000 pylint_keyword_only_args_plugin-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      410 2023-04-15 06:23:07.303291 pylint_keyword_only_args_plugin-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 07:44:39.407073 pylint_keyword_only_args_plugin-0.2.3/pylint_keyword_only_args_plugin/__init__.py
+-rw-r--r--   0        0        0     1663 2023-04-16 15:20:11.843003 pylint_keyword_only_args_plugin-0.2.3/pylint_keyword_only_args_plugin/checker.py
+-rw-r--r--   0        0        0      211 2023-04-15 07:49:11.615918 pylint_keyword_only_args_plugin-0.2.3/pylint_keyword_only_args_plugin/keyword_only_args.py
+-rw-r--r--   0        0        0     1162 2023-04-16 15:23:10.441846 pylint_keyword_only_args_plugin-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1302 1970-01-01 00:00:00.000000 pylint_keyword_only_args_plugin-0.2.3/PKG-INFO
```

### Comparing `pylint_keyword_only_args_plugin-0.2.2/pylint_keyword_only_args_plugin/checker.py` & `pylint_keyword_only_args_plugin-0.2.3/pylint_keyword_only_args_plugin/checker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import builtins
-from typing import Iterable
+from typing import TYPE_CHECKING
 
-from astroid.nodes import Call, Assign, Tuple, Attribute
+from astroid.nodes import Assign, Attribute, Call, Tuple
 from pylint.checkers import BaseChecker
 
+if TYPE_CHECKING:
+    from collections.abc import Iterable
+
 
 class KeywordOnlyArgsChecker(BaseChecker):
     name = "keyword-only-args"
     priority = -100
     msgs = {
         "C0004": (
             "Only keyword arguments allowed to callable.",
@@ -15,32 +18,41 @@
             "Positional arguments to callable not allowed. "
             "Example: func_call(a=1, b=2) - good, func_call(a, b) - bad, func_call(a, b=2) - bad.",
         ),
     }
     options = (
         (
             "skip-names-list",
-            {"default": "", "type": "string", "help": "Comma separated list of callable names to skip"}
+            {
+                "default": "",
+                "type": "string",
+                "help": "Comma separated list of callable names to skip",
+            },
         ),
     )
 
-    def visit_call(self, node: Call) -> None:
+    def visit_call(self: "KeywordOnlyArgsChecker", node: Call) -> None:
         nodes: Iterable = [node]
         if isinstance(node, Assign):
             if isinstance(node.value, Call):
                 nodes = [node.value]
 
             if isinstance(node.value, Tuple):
                 nodes = node.value.elts
 
-        skip_names_list = [*dir(builtins), *self.linter.config.skip_names_list.split(","), "Path"]
+        skip_names_list = [
+            *dir(builtins),
+            *self.linter.config.skip_names_list.split(","),
+            "Path",
+        ]
         for _node in nodes:
-            if isinstance(_node.func, Attribute):
-                node_name = _node.func.attrname
-            else:
-                node_name = _node.func.name
+            node_name = (
+                _node.func.attrname
+                if isinstance(_node.func, Attribute)
+                else _node.func.name
+            )
 
             if node_name in skip_names_list:
                 return
 
             if _node.args:
                 self.add_message("keyword-only-args", node=_node)
```

### Comparing `pylint_keyword_only_args_plugin-0.2.2/pyproject.toml` & `pylint_keyword_only_args_plugin-0.2.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylint-keyword-only-args-plugin"
-version = "0.2.2"
+version = "0.2.3"
 description = "Plugin for pylint which checks that call statements has only keyword args"
 authors = ["Konstantin Shestakov <winmasta@yandex.ru>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/winmasta"
 repository = "https://github.com/winmasta"
 keywords = ["pylint", "positional", "args", "lint"]
@@ -20,18 +20,25 @@
 python = "^3.11"
 pylint = "*"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
+black = "*"
 pytest = "*"
+ruff = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pylint."messages control"]
 disable = ["missing-docstring"]
 
 [tool.pylint.format]
 max-line-length = 119
+
+[tool.ruff]
+line-length = 119
+select = ["ALL"]
+ignore = ["D100", "D101", "D102", "D103", "D104", "D203", "D212"]
```

### Comparing `pylint_keyword_only_args_plugin-0.2.2/PKG-INFO` & `pylint_keyword_only_args_plugin-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylint-keyword-only-args-plugin
-Version: 0.2.2
+Version: 0.2.3
 Summary: Plugin for pylint which checks that call statements has only keyword args
 Home-page: https://github.com/winmasta
 License: MIT
 Keywords: pylint,positional,args,lint
 Author: Konstantin Shestakov
 Author-email: winmasta@yandex.ru
 Requires-Python: >=3.11,<4.0
```

