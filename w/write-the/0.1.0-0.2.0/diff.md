# Comparing `tmp/write_the-0.1.0.tar.gz` & `tmp/write_the-0.2.0.tar.gz`

## Comparing `write_the-0.1.0.tar` & `write_the-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,22 @@
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 write_the-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.1.0/write_the/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.1.0/write_the/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.1.0/write_the/__main__.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 write_the-0.1.0/write_the/cli/__init__.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 write_the-0.1.0/write_the/cli/utils.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.1.0/write_the/docs/__init__.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 write_the-0.1.0/write_the/docs/chain.py
--rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 write_the-0.1.0/write_the/docs/docstring.py
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 write_the-0.1.0/write_the/docs/write.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 write_the-0.1.0/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 write_the-0.1.0/README.md
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 write_the-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 write_the-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 write_the-0.2.0/test.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 write_the-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/__main__.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/cli/__init__.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/cli/utils.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/cst/__init__.py
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/cst/docstring_adder.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/cst/docstring_remover.py
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/cst/function_and_class_collector.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/cst/node_extractor.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/cst/node_remover.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/cst/utils.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/docs/__init__.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/docs/chain.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/docs/write.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 write_the-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 write_the-0.2.0/README.md
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 write_the-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 write_the-0.2.0/PKG-INFO
```

### Comparing `write_the-0.1.0/write_the/cli/__init__.py` & `write_the-0.2.0/write_the/cli/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typer
-from ..__about__ import __version__
-from ..docs import write_the_docs
+from write_the.__about__ import __version__
+from write_the.docs import write_the_docs
 from .utils import list_python_files
 from pathlib import Path
 from rich.console import Console
 from rich.syntax import Syntax
 from typing import List
 
 app = typer.Typer()
@@ -33,15 +33,15 @@
         None,
         "--node",
         "-n",
         help="Generate docs for specific nodes (functions and classes).",
     ),
 ):
     """
-    Write the docs!
+    Document and format your code!
     """
     if file.is_dir():
         files = list_python_files(file)
     else:
         assert file.suffix == ".py"
         files = [file]
     for file in files:
```

### Comparing `write_the-0.1.0/write_the/cli/utils.py` & `write_the-0.2.0/write_the/cli/utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.1.0/write_the/docs/chain.py` & `write_the-0.2.0/write_the/docs/chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from langchain.prompts import PromptTemplate
 from langchain.chains import LLMChain
 from langchain.llms import OpenAI
 
 llm = OpenAI(temperature=0, max_tokens=2000)
-docs_template = "\nWrite Google style docstrings for the following code, using the multi-line format with a description and examples. The first lines describe the code. Include parameter type definitions where possible, and specify any exceptions raised and side effects of the function. For functions with multiple return values or ambiguous behaviour, provide clear guidelines for documenting the behaviour. Please refer to the Google style guide for more information. Any notes should be include in the `Notes:` section of the docstring. Only return the docstring its self. Return each docstring on a single line with the name of the function/class as the key and the docstring as the value. Separate each result by a newline. If the function is a method return the name in the format Class.method. The class docstring should only contain Description and Attributes. Each result should be separated by multiple newlines. \n---\nEXAMPLE\n---\n\ndef add(a, b): \n    return a + b \nHere are formatted docstrings for only add:\nadd:\n  Sums 2 numbers.\n  Args:\n    a (int): The first number to add.\n    b (int): The second number to add.\n  Returns:\n    int: The sum of `a` and `b`.\n  Examples:\n    >>> add(1, 2)\n    3\n\n\n---\nCODE\n---\n{code}\nHere are formatted docstrings for only {nodes}:\n"
+docs_template = "\nWrite Google style docstrings for the following code, using the multi-line format with a description and examples. The first lines describe the code. Include parameter type definitions where possible, and specify any exceptions raised and side effects of the function. For functions with multiple return values or ambiguous behaviour, provide clear guidelines for documenting the behaviour. Please refer to the Google style guide for more information. Any notes should be include in the `Notes:` section of the docstring. Only return the docstring its self. Return each docstring on a single line with the name of the function/class as the key and the docstring as the value. Separate each result by a newline. If the function is a method return the name in the format Class.method. The Class docstrings should contain Description and Attributes. Each result should be separated by multiple newlines. \n---\nEXAMPLE\n---\n\ndef add(a, b): \n    return a + b \nHere are formatted docstrings for only add:\nadd:\n  Sums 2 numbers.\n  Args:\n    a (int): The first number to add.\n    b (int): The second number to add.\n  Returns:\n    int: The sum of `a` and `b`.\n  Examples:\n    >>> add(1, 2)\n    3\n\n\n---\nCODE\n---\n{code}\nHere are formatted docstrings for only {nodes}:\n"
 docs_prompt = PromptTemplate(input_variables=["code", "nodes"], template=docs_template)
 docs_chain = LLMChain(llm=llm, prompt=docs_prompt)
 
 
 def run(code, nodes: list) -> str:
     """
     Generates docstrings for a given code and list of nodes.
```

### Comparing `write_the-0.1.0/write_the/docs/write.py` & `write_the-0.2.0/write_the/docs/write.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,73 +1,81 @@
 from pathlib import Path
-import ast
+import libcst as cst
 from black import format_str, FileMode
-from .docstring import DocstringAdder, get_node_names, remove_docstrings, process_tree
+
+from write_the.cst import nodes_to_tree
+from write_the.cst.docstring_adder import DocstringAdder
+from write_the.cst.docstring_remover import remove_docstrings
+from write_the.cst.function_and_class_collector import get_node_names
+from write_the.cst.node_extractor import extract_nodes_from_tree
+from write_the.cst.node_remover import remove_nodes_from_tree
 from .chain import run
 
 
 def write_the_docs(
     filename: Path, nodes=[], force=False, inplace=False, context=True
 ) -> str:
-    '''
-    Writes docstrings to a given file.
+    """
+    Generates docstrings for a given file.
     Args:
-      filename (Path): The path to the file to write the docstrings to.
-      nodes (list): A list of nodes to write docstrings for.
-      force (bool): If True, overwrite existing docstrings.
-      inplace (bool): If True, write docstrings to the same file.
-      context (bool): If True, write docstrings for all nodes in the file.
+      filename (Path): The path to the file to generate docstrings for.
+      nodes (list): A list of nodes to generate docstrings for.
+      force (bool): Whether to overwrite existing docstrings.
+      inplace (bool): Whether to generate docstrings in the same file.
+      context (bool): Whether to send context with the code (can improve docstings).
     Returns:
-      str: The modified source code with the docstrings added.
+      str: The source code with the generated docstrings.
     Notes:
-      If `nodes` is empty, docstrings will be written for all nodes in the file.
-      If `context` is False, docstrings will only be written for the nodes in `nodes`.
+      If `nodes` is provided, `force` is set to `True` and `context` is set to `False`.
     Examples:
-      >>> write_the_docs('example.py', nodes=['add', 'subtract'], force=True, inplace=True, context=False)
-      'def add(a, b):
-          """Adds two numbers.
+      >>> write_the_docs("example.py")
+      "def add(a, b):
+          \"\"\"Sums 2 numbers.
           Args:
               a (int): The first number to add.
               b (int): The second number to add.
           Returns:
               int: The sum of `a` and `b`.
-          """
-          return a + b
-      def subtract(a, b):
-          """Subtracts two numbers.
-          Args:
-              a (int): The first number to subtract.
-              b (int): The second number to subtract.
-          Returns:
-              int: The difference of `a` and `b`.
-          """
-          return a - b'
-    '''
+          \"\"\"
+          return a + b"
+    """
     with open(filename, "r") as file:
         source_code = file.read()
+
     source_code = format_str(source_code, mode=FileMode())
-    tree = ast.parse(source_code)
+    tree = cst.parse_module(source_code)
     extract_specific_nodes = False
+
     if nodes:
         extract_specific_nodes = True
+        force = True
     else:
         nodes = get_node_names(tree, force)
-    processed_tree = remove_docstrings(tree, nodes)
+    if not nodes:
+        return source_code
+    remove_docstrings_tree = remove_docstrings(tree, nodes)
     if not context:
         if extract_specific_nodes:
-            processed_tree = process_tree(processed_tree, nodes, False)
+            extracted_nodes = extract_nodes_from_tree(remove_docstrings_tree, nodes)
+            processed_tree = nodes_to_tree(extracted_nodes)
         else:
             all_nodes = get_node_names(tree, False)
             nodes_to_remove = [n for n in all_nodes if n not in nodes]
-            processed_tree = process_tree(processed_tree, nodes_to_remove, True)
-    code = ast.unparse(processed_tree)
+            processed_tree = remove_nodes_from_tree(
+                remove_docstrings_tree, nodes_to_remove
+            )
+        code = processed_tree.code
+    else:
+        code = remove_docstrings_tree.code
     result = run(code=code, nodes=nodes)
     docstring_dict = {}
     for line in result.split("\n\n"):
         (node_name, docsting) = line.split(":", 1)
         docstring_dict[node_name] = docsting + "\n\n"
-    modified_tree = DocstringAdder(docstring_dict, force).visit(tree)
+    modified_tree = remove_docstrings_tree.visit(DocstringAdder(docstring_dict, force))
+
     if not inplace and extract_specific_nodes:
-        modified_tree = process_tree(tree, nodes, False)
-    modified_tree = ast.fix_missing_locations(modified_tree)
-    modified_code = ast.unparse(modified_tree)
+        extracted_nodes = extract_nodes_from_tree(tree, nodes)
+        modified_tree = nodes_to_tree(extracted_nodes)
+
+    modified_code = modified_tree.code
     return format_str(modified_code, mode=FileMode())
```

### Comparing `write_the-0.1.0/LICENSE.txt` & `write_the-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `write_the-0.1.0/README.md` & `write_the-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `write_the-0.1.0/pyproject.toml` & `write_the-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,16 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "typer[all]",
   "langchain",
-  "black"
+  "black",
+  "libcst",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/wytamma/write-the#readme"
 Issues = "https://github.com/wytamma/write-the/issues"
 Source = "https://github.com/wytamma/write-the"
```

### Comparing `write_the-0.1.0/PKG-INFO` & `write_the-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: write-the
-Version: 0.1.0
+Version: 0.2.0
 Summary: AI-powered Code Generation and Refactoring Tool
 Project-URL: Documentation, https://github.com/wytamma/write-the#readme
 Project-URL: Issues, https://github.com/wytamma/write-the/issues
 Project-URL: Source, https://github.com/wytamma/write-the
 Author-email: wytamma <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Requires-Dist: black
 Requires-Dist: langchain
+Requires-Dist: libcst
 Requires-Dist: typer[all]
 Description-Content-Type: text/markdown
 
 # Write-The: AI-powered Code Generation and Refactoring Tool
 
 [![PyPI - Version](https://img.shields.io/pypi/v/write-the.svg)](https://pypi.org/project/write-the)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/write-the.svg)](https://pypi.org/project/write-the)
```

