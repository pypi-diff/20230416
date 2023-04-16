# Comparing `tmp/customtex-0.1.1.tar.gz` & `tmp/customtex-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customtex-0.1.1.tar", max compression
+gzip compressed data, was "customtex-0.1.2.tar", max compression
```

## Comparing `customtex-0.1.1.tar` & `customtex-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1074 2023-02-19 23:01:00.422635 customtex-0.1.1/LICENSE
--rw-r--r--   0        0        0     1723 2023-02-20 00:03:41.306184 customtex-0.1.1/README.md
--rw-r--r--   0        0        0      103 2023-02-19 23:01:00.423086 customtex-0.1.1/customtex/__init__.py
--rw-r--r--   0        0        0     2837 2023-02-19 23:01:00.423531 customtex-0.1.1/customtex/files_text.py
--rw-r--r--   0        0        0     3114 2023-02-19 23:01:00.423772 customtex-0.1.1/customtex/load_presets.py
--rw-r--r--   0        0        0      962 2023-02-19 23:01:00.423980 customtex-0.1.1/customtex/main.py
--rw-r--r--   0        0        0     4455 2023-02-19 23:01:00.424183 customtex-0.1.1/customtex/parser.py
--rw-r--r--   0        0        0       61 2023-02-19 23:01:00.424486 customtex-0.1.1/customtex/presets/hypersetups.json
--rw-r--r--   0        0        0     1582 2023-02-19 23:01:00.424708 customtex-0.1.1/customtex/presets/languages.json
--rw-r--r--   0        0        0      936 2023-02-19 23:01:00.424914 customtex-0.1.1/customtex/presets/macros.json
--rw-r--r--   0        0        0     2662 2023-02-19 23:01:00.425157 customtex-0.1.1/customtex/presets/sectionstyles.json
--rw-r--r--   0        0        0     2142 2023-02-19 23:01:00.425367 customtex-0.1.1/customtex/presets/templates.json
--rw-r--r--   0        0        0     4185 2023-02-20 00:03:41.306525 customtex-0.1.1/customtex/presets/theoremstyles.json
--rw-r--r--   0        0        0     1741 2023-02-19 23:01:00.426066 customtex-0.1.1/customtex/presets/titlestyles.json
--rw-r--r--   0        0        0      678 2023-02-20 00:03:41.306751 customtex-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2595 1970-01-01 00:00:00.000000 customtex-0.1.1/setup.py
--rw-r--r--   0        0        0     2351 1970-01-01 00:00:00.000000 customtex-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-02-19 23:01:00.422635 customtex-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1723 2023-04-16 16:05:03.670623 customtex-0.1.2/README.md
+-rw-r--r--   0        0        0      103 2023-02-19 23:01:00.423086 customtex-0.1.2/customtex/__init__.py
+-rw-r--r--   0        0        0     2837 2023-02-19 23:01:00.423531 customtex-0.1.2/customtex/files_text.py
+-rw-r--r--   0        0        0     3114 2023-02-19 23:01:00.423772 customtex-0.1.2/customtex/load_presets.py
+-rw-r--r--   0        0        0      962 2023-02-19 23:01:00.423980 customtex-0.1.2/customtex/main.py
+-rw-r--r--   0        0        0     4455 2023-02-19 23:01:00.424183 customtex-0.1.2/customtex/parser.py
+-rw-r--r--   0        0        0       61 2023-02-19 23:01:00.424486 customtex-0.1.2/customtex/presets/hypersetups.json
+-rw-r--r--   0        0        0     1582 2023-02-19 23:01:00.424708 customtex-0.1.2/customtex/presets/languages.json
+-rw-r--r--   0        0        0      942 2023-04-16 16:05:03.670968 customtex-0.1.2/customtex/presets/macros.json
+-rw-r--r--   0        0        0     2662 2023-02-19 23:01:00.425157 customtex-0.1.2/customtex/presets/sectionstyles.json
+-rw-r--r--   0        0        0     2142 2023-02-19 23:01:00.425367 customtex-0.1.2/customtex/presets/templates.json
+-rw-r--r--   0        0        0     4185 2023-02-20 00:03:41.306525 customtex-0.1.2/customtex/presets/theoremstyles.json
+-rw-r--r--   0        0        0     1741 2023-02-19 23:01:00.426066 customtex-0.1.2/customtex/presets/titlestyles.json
+-rw-r--r--   0        0        0      678 2023-04-16 16:05:03.671283 customtex-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2595 1970-01-01 00:00:00.000000 customtex-0.1.2/setup.py
+-rw-r--r--   0        0        0     2351 1970-01-01 00:00:00.000000 customtex-0.1.2/PKG-INFO
```

### Comparing `customtex-0.1.1/LICENSE` & `customtex-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `customtex-0.1.1/README.md` & `customtex-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# CustomTeX v0.1.1
+# CustomTeX v0.1.2
 
 ### A CLI utility for setting up LaTeX projects
 CustomTeX is a command line utility for setting up LaTeX projects based on some predefined styles for titles, section headers, theorems, etc.
 
 For the moment, the utility is intended for a personal use, since there aren't many options for customization. However, we aim to design a more general system for creating LaTeX projects based on dynamic and fully customizable templates.
 
 ## Installation
```

### Comparing `customtex-0.1.1/customtex/files_text.py` & `customtex-0.1.2/customtex/files_text.py`

 * *Files identical despite different names*

### Comparing `customtex-0.1.1/customtex/load_presets.py` & `customtex-0.1.2/customtex/load_presets.py`

 * *Files identical despite different names*

### Comparing `customtex-0.1.1/customtex/main.py` & `customtex-0.1.2/customtex/main.py`

 * *Files identical despite different names*

### Comparing `customtex-0.1.1/customtex/parser.py` & `customtex-0.1.2/customtex/parser.py`

 * *Files identical despite different names*

### Comparing `customtex-0.1.1/customtex/presets/languages.json` & `customtex-0.1.2/customtex/presets/languages.json`

 * *Files identical despite different names*

### Comparing `customtex-0.1.1/customtex/presets/macros.json` & `customtex-0.1.2/customtex/presets/macros.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333333%*

 * *Differences: {"'math'": "{insert: [(0, '\\\\newcommand{\\\\RR}{\\\\ensuremath{\\\\mathbb{R}}}'), (1, "*

 * *           "'\\\\newcommand{\\\\NN}{\\\\ensuremath{\\\\mathbb{N}}}'), (2, "*

 * *           "'\\\\newcommand{\\\\ZZ}{\\\\ensuremath{\\\\mathbb{Z}}}'), (3, "*

 * *           "'\\\\newcommand{\\\\QQ}{\\\\ensuremath{\\\\mathbb{Q}}}'), (4, "*

 * *           "'\\\\newcommand{\\\\CC}{\\\\ensuremath{\\\\mathbb{C}}}'), (5, "*

 * *           "'\\\\newcommand{\\\\FF}{\\\\ensuremath{\\\\mathbb{F}}}')], delete: [5, 4, 3, 2, 1, 0]}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "math": [
-        "\\newcommand{\\R}{\\ensuremath{\\mathbb{R}}}",
-        "\\newcommand{\\N}{\\ensuremath{\\mathbb{N}}}",
-        "\\newcommand{\\Z}{\\ensuremath{\\mathbb{Z}}}",
-        "\\newcommand{\\Q}{\\ensuremath{\\mathbb{Q}}}",
-        "\\newcommand{\\C}{\\ensuremath{\\mathbb{C}}}",
-        "\\newcommand{\\F}{\\ensuremath{\\mathbb{F}}}",
+        "\\newcommand{\\RR}{\\ensuremath{\\mathbb{R}}}",
+        "\\newcommand{\\NN}{\\ensuremath{\\mathbb{N}}}",
+        "\\newcommand{\\ZZ}{\\ensuremath{\\mathbb{Z}}}",
+        "\\newcommand{\\QQ}{\\ensuremath{\\mathbb{Q}}}",
+        "\\newcommand{\\CC}{\\ensuremath{\\mathbb{C}}}",
+        "\\newcommand{\\FF}{\\ensuremath{\\mathbb{F}}}",
         "\\newcommand{\\set}[1]{\\ensuremath{\\left\\lbrace#1\\right\\rbrace}}",
         "\\newcommand{\\abs}[1]{\\ensuremath{\\left|#1\\right|}}",
         "\\newcommand{\\norm}[1]{\\ensuremath{\\left\\lVert#1\\right\\rVert}}",
         "\\newcommand{\\gen}[1]{\\ensuremath{\\left\\langle#1\\right\\rangle}}",
         "\\newcommand{\\floor}[1]{\\ensuremath{\\left\\lfloor#1\\right\\rfloor}}",
         "\\newcommand{\\ceil}[1]{\\ensuremath{\\left\\lceil#1\\right\\rceil}}"
     ],
```

### Comparing `customtex-0.1.1/customtex/presets/sectionstyles.json` & `customtex-0.1.2/customtex/presets/sectionstyles.json`

 * *Files identical despite different names*

### Comparing `customtex-0.1.1/customtex/presets/templates.json` & `customtex-0.1.2/customtex/presets/templates.json`

 * *Files identical despite different names*

### Comparing `customtex-0.1.1/customtex/presets/theoremstyles.json` & `customtex-0.1.2/customtex/presets/theoremstyles.json`

 * *Files identical despite different names*

### Comparing `customtex-0.1.1/customtex/presets/titlestyles.json` & `customtex-0.1.2/customtex/presets/titlestyles.json`

 * *Files identical despite different names*

### Comparing `customtex-0.1.1/pyproject.toml` & `customtex-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "customtex"
-version = "0.1.1"
+version = "0.1.2"
 description = "A CLI utility for setting up LaTeX projects"
 authors = ["Mario Vago Marzal <mariovagomarzal@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/mariovagomarzal/customtex"
 repository = "https://github.com/mariovagomarzal/customtex"
 include = ["LICENSE", "README.md"]
```

### Comparing `customtex-0.1.1/setup.py` & `customtex-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['string-color>=1.2.3,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['customtex = customtex.main:customtex']}
 
 setup_kwargs = {
     'name': 'customtex',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'A CLI utility for setting up LaTeX projects',
-    'long_description': "# CustomTeX v0.1.1\n\n### A CLI utility for setting up LaTeX projects\nCustomTeX is a command line utility for setting up LaTeX projects based on some predefined styles for titles, section headers, theorems, etc.\n\nFor the moment, the utility is intended for a personal use, since there aren't many options for customization. However, we aim to design a more general system for creating LaTeX projects based on dynamic and fully customizable templates.\n\n## Installation\nCustomTeX is a Python library and can be installed using pip:\n\n    pip install customtex\n\nNo additional dependencies are required.\n\n## Usage\nTo generate the main files of a LaTeX project with CustomTeX, you have to run the `customtex` command followed by the path, main file name and language options and the `init` or the `template` subcommand. For example:\n\n    customtex --path /path/to/directory --name main --lang english init [options]\n\nThis will create a LaTeX project with the following structure in the `path/to/directory` directory:\n\n    /path/to/directory\n    ├── main.tex\n    └── tex\n        ├── macros.tex\n        └── preamble.tex\n\n\n### The `init` subcommand\nThe `init` subcommand creates a project based on the options that the utility provides. Run `customtex init --help` to see the available options.\n\n### The `template` subcommand\nThe `template` subcommand creates a project based on a template. A template consist of a list of options from the `init` subcommand that are run when invoking the `template` option followed by the name of the template.\n\nRun `customtex template --help` to see the available templates.\n\n## License\nCustomTeX is licensed under the MIT license. See the LICENSE file for more information.\n",
+    'long_description': "# CustomTeX v0.1.2\n\n### A CLI utility for setting up LaTeX projects\nCustomTeX is a command line utility for setting up LaTeX projects based on some predefined styles for titles, section headers, theorems, etc.\n\nFor the moment, the utility is intended for a personal use, since there aren't many options for customization. However, we aim to design a more general system for creating LaTeX projects based on dynamic and fully customizable templates.\n\n## Installation\nCustomTeX is a Python library and can be installed using pip:\n\n    pip install customtex\n\nNo additional dependencies are required.\n\n## Usage\nTo generate the main files of a LaTeX project with CustomTeX, you have to run the `customtex` command followed by the path, main file name and language options and the `init` or the `template` subcommand. For example:\n\n    customtex --path /path/to/directory --name main --lang english init [options]\n\nThis will create a LaTeX project with the following structure in the `path/to/directory` directory:\n\n    /path/to/directory\n    ├── main.tex\n    └── tex\n        ├── macros.tex\n        └── preamble.tex\n\n\n### The `init` subcommand\nThe `init` subcommand creates a project based on the options that the utility provides. Run `customtex init --help` to see the available options.\n\n### The `template` subcommand\nThe `template` subcommand creates a project based on a template. A template consist of a list of options from the `init` subcommand that are run when invoking the `template` option followed by the name of the template.\n\nRun `customtex template --help` to see the available templates.\n\n## License\nCustomTeX is licensed under the MIT license. See the LICENSE file for more information.\n",
     'author': 'Mario Vago Marzal',
     'author_email': 'mariovagomarzal@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mariovagomarzal/customtex',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `customtex-0.1.1/PKG-INFO` & `customtex-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: customtex
-Version: 0.1.1
+Version: 0.1.2
 Summary: A CLI utility for setting up LaTeX projects
 Home-page: https://github.com/mariovagomarzal/customtex
 License: MIT
 Author: Mario Vago Marzal
 Author-email: mariovagomarzal@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: string-color (>=1.2.3,<2.0.0)
 Project-URL: Repository, https://github.com/mariovagomarzal/customtex
 Description-Content-Type: text/markdown
 
-# CustomTeX v0.1.1
+# CustomTeX v0.1.2
 
 ### A CLI utility for setting up LaTeX projects
 CustomTeX is a command line utility for setting up LaTeX projects based on some predefined styles for titles, section headers, theorems, etc.
 
 For the moment, the utility is intended for a personal use, since there aren't many options for customization. However, we aim to design a more general system for creating LaTeX projects based on dynamic and fully customizable templates.
 
 ## Installation
```

