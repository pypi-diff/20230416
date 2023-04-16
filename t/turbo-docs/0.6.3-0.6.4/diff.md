# Comparing `tmp/turbo_docs-0.6.3.tar.gz` & `tmp/turbo_docs-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\turbo_docs-0.6.3.tar", last modified: Fri Apr 14 17:05:47 2023, max compression
+gzip compressed data, was "dist\turbo_docs-0.6.4.tar", last modified: Sun Apr 16 15:37:08 2023, max compression
```

## Comparing `turbo_docs-0.6.3.tar` & `turbo_docs-0.6.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 17:05:47.025899 turbo_docs-0.6.3/
--rw-rw-rw-   0        0        0     1483 2023-04-14 17:05:47.024893 turbo_docs-0.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     1027 2023-04-14 16:55:11.000000 turbo_docs-0.6.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-14 17:05:47.026893 turbo_docs-0.6.3/setup.cfg
--rw-rw-rw-   0        0        0      849 2023-04-14 17:05:22.000000 turbo_docs-0.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 17:05:47.007217 turbo_docs-0.6.3/turbo_docs/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.6.3/turbo_docs/__init__.py
--rw-rw-rw-   0        0        0     3668 2023-04-14 17:05:00.000000 turbo_docs-0.6.3/turbo_docs/generate.py
-drwxrwxrwx   0        0        0        0 2023-04-14 17:05:47.023899 turbo_docs-0.6.3/turbo_docs/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.6.3/turbo_docs/utils/__init__.py
--rw-rw-rw-   0        0        0      893 2023-04-12 00:51:47.000000 turbo_docs-0.6.3/turbo_docs/utils/cli_options.py
--rw-rw-rw-   0        0        0     1794 2023-04-11 19:29:42.000000 turbo_docs-0.6.3/turbo_docs/utils/directory.py
--rw-rw-rw-   0        0        0      687 2023-04-14 14:45:03.000000 turbo_docs-0.6.3/turbo_docs/utils/openai_api.py
-drwxrwxrwx   0        0        0        0 2023-04-14 17:05:47.017900 turbo_docs-0.6.3/turbo_docs.egg-info/
--rw-rw-rw-   0        0        0     1483 2023-04-14 17:05:46.000000 turbo_docs-0.6.3/turbo_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-04-14 17:05:46.000000 turbo_docs-0.6.3/turbo_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 17:05:46.000000 turbo_docs-0.6.3/turbo_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-14 17:05:46.000000 turbo_docs-0.6.3/turbo_docs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-04-14 17:05:46.000000 turbo_docs-0.6.3/turbo_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-14 17:05:46.000000 turbo_docs-0.6.3/turbo_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 15:37:08.091327 turbo_docs-0.6.4/
+-rw-rw-rw-   0        0        0     1805 2023-04-16 15:37:08.091327 turbo_docs-0.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2023-04-16 15:34:04.000000 turbo_docs-0.6.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-16 15:37:08.092335 turbo_docs-0.6.4/setup.cfg
+-rw-rw-rw-   0        0        0      726 2023-04-16 15:35:24.000000 turbo_docs-0.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:37:08.061574 turbo_docs-0.6.4/turbo_docs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.6.4/turbo_docs/__init__.py
+-rw-rw-rw-   0        0        0     5623 2023-04-16 15:25:13.000000 turbo_docs-0.6.4/turbo_docs/generate.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:37:08.088812 turbo_docs-0.6.4/turbo_docs/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.6.4/turbo_docs/utils/__init__.py
+-rw-rw-rw-   0        0        0     1471 2023-04-16 15:13:12.000000 turbo_docs-0.6.4/turbo_docs/utils/cli_options.py
+-rw-rw-rw-   0        0        0     1624 2023-04-16 15:18:24.000000 turbo_docs-0.6.4/turbo_docs/utils/directory.py
+-rw-rw-rw-   0        0        0      763 2023-04-16 15:13:17.000000 turbo_docs-0.6.4/turbo_docs/utils/openai_api.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:37:08.082810 turbo_docs-0.6.4/turbo_docs.egg-info/
+-rw-rw-rw-   0        0        0     1805 2023-04-16 15:37:07.000000 turbo_docs-0.6.4/turbo_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-04-16 15:37:07.000000 turbo_docs-0.6.4/turbo_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 15:37:07.000000 turbo_docs-0.6.4/turbo_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-16 15:37:07.000000 turbo_docs-0.6.4/turbo_docs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-04-16 15:37:07.000000 turbo_docs-0.6.4/turbo_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-16 15:37:07.000000 turbo_docs-0.6.4/turbo_docs.egg-info/top_level.txt
```

### Comparing `turbo_docs-0.6.3/PKG-INFO` & `turbo_docs-0.6.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 Metadata-Version: 2.1
 Name: turbo_docs
-Version: 0.6.3
+Version: 0.6.4
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 
 
+# Turbo Docs
 
-## Turbo-Docs
-Turbo-Docs is a package for Python creating formatted, user-friendly README.md files and unit tests. 
+Turbo Docs is a set of command-line utilities made for automating document creation and data entry tasks. Its utilities make it easy to create, package, and distribute Python packages for use by others. The code utilizes Python libraries like requests, openai, click, pyperclip, and redbaron in order to automate data entry tasks, formatting docstrings and wrapping text to 80 characters. The CLI application can generate a README summarizing the code, unit tests and docstrings for Python functions.
 
-### Installation
-Using pip:
-```bash
-pip install turbo_docs
-```
+## Requirements
 
-Using setup.py
-```bash
-python setup.py install
-```
+- Setuptools library
+- Wheel library
+- Twine
+- Requests
+- OpenAI
+- Click
+- pyperclip
+- Redbaron
 
-### Usage
-Using the command line: 
-```bash
-turbo_docs [OPTION]
-```
+## Features
+
+- Automate data entry tasks via copy to clipboard
+- Generate a README summarizing the code
+- Generate unit tests
+- Generate concise docstrings for functions
 
-- Create a Formatted and User-Friendly Readme.md file:
+## Usage
 
-```bash
-turbo_docs --create_readme
+Generate a README.md summarizing your code: 
+
+```
+python generate.py --create_readme
 ```
 
-- Create a Formatted and User-Friendly Readme.md file for large repos:
+Generate a README.md for larger repositories:
 
-```bash
-turbo_docs --create_readme_plus
+```
+python generate.py --create_readme_plus
 ```
 
-- Create Unit Tests for each code file: 
+Generate unit tests for the code files (work in progress):
 
-```bash
-turbo_docs --create_tests
+```
+python generate.py --create_tests
 ```
 
-### Requirements
-- Python 3.8+
-- Setuptools
-- Wheel
-- Twine
-- OpenAI
-- Requests
-- Click
-- Pyperclip
+Generate and insert docstrings for each Python function:
 
-### Developed by
+```
+python generate.py --create_docstring
+```
 
-This code is developed by [Jamie Voynow](https://github.com/voynow), a software developer with an aim to make the process of creating and managing documentation easier. For more information, visit the [GitHub repository](https://github.com/voynow/turbo-docs).
+Copy all code files in the directory to the clipboard:
+
+``` 
+python generate.py --copy
+```
```

### Comparing `turbo_docs-0.6.3/setup.py` & `turbo_docs-0.6.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup, find_packages
 
 setup(
-    name="turbo_docs",
-    version="0.6.3",
-    packages=find_packages(),
-    install_requires=[
-        "requests",
-        "openai",
-        "click",
-        "pyperclip",
-    ],
-    entry_points={
-        "console_scripts": [
-            "turbo_docs=turbo_docs.generate:driver"
-        ],
-    },
-    classifiers=[
-        "Development Status :: 3 - Alpha",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-    ],
-    long_description=open("README.md", encoding="utf-8").read()
+	name="turbo_docs",
+	version="0.6.4",
+	packages=find_packages(),
+	install_requires=[
+		"requests",
+		"openai",
+		"click",
+		"pyperclip",
+	],
+	entry_points={
+		"console_scripts": [
+			"turbo_docs=turbo_docs.generate:driver"
+		],
+	},
+	classifiers=[
+		"Development Status :: 3 - Alpha",
+		"Intended Audience :: Developers",
+		"License :: OSI Approved :: MIT License",
+		"Programming Language :: Python :: 3",
+		"Programming Language :: Python :: 3.6",
+		"Programming Language :: Python :: 3.7",
+		"Programming Language :: Python :: 3.8",
+		"Programming Language :: Python :: 3.9",
+	],
+	long_description=open("README.md", encoding="utf-8").read()
 )
```

### Comparing `turbo_docs-0.6.3/turbo_docs/utils/directory.py` & `turbo_docs-0.6.4/turbo_docs/utils/directory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,57 @@
 import json
 import os
 from pathlib import Path
 from typing import List, Dict
 
 def ignored_files_init() -> List[str]:
-    """ Initialize a list of ignored files and including README.md, docs.md, etc.
+	"""
+    Initialize the list of files to be ignored.
     """
-    ignored_files = ["README.md", "tests"]
-    for file in os.listdir():
-        if file[0] == ".":
-            ignored_files.append(file)
-    return ignored_files
+	ignored_files = ["README.md", "tests", "setup.py"]
+	for file in os.listdir():
+		if file[0] == ".":
+			ignored_files.append(file)
+	return ignored_files
 
 def read_gitignore() -> List[str]:
-    """ Read .gitignore file and return the list of ignored files.
+	"""
+    Read .gitignore file and return a list of ignored files.
     """
-    ignore_files = ignored_files_init()
-    try:
-        with open(".gitignore", "r") as gitignore:
-            for line in gitignore:
-                ignore_files.append(line.strip())
-    except FileNotFoundError:
-        raise ValueError(".gitignore file required for excluding files from documentation generation")
-    return ignore_files
+	ignore_files = ignored_files_init()
+	try:
+		with open(".gitignore", "r") as gitignore:
+			for line in gitignore:
+				ignore_files.append(line.strip())
+	except FileNotFoundError:
+		raise ValueError(".gitignore file required for excluding files from documentation generation")
+	return ignore_files
 
 def ignore_filepath(filepath: str, ignore_files: List[str]) -> bool:
-    """ Check if a filepath should be ignored based on the ignore_files list.
+	"""
+    Checks if a filepath includes a particular file or folder to ignore.
     """
-    for part in Path(filepath).parts:
-        if part in ignore_files:
-            return True
-    return False
+	for part in Path(filepath).parts:
+		if part in ignore_files:
+			return True
+	return False
 
 def get_files() -> Dict:
-    """ Retrieve the content of all files in the current directory, excluding those listed in the ignore_files.
+	"""
+    Retrieve files from directory ignoring items from .gitignore and formatting tab
+    indentation.
     """
-    files_dict = {}
-    ignore_files = read_gitignore()
+	files_dict = {}
+	ignore_files = read_gitignore()
 
-    # Iterate over files
-    for root, _, files in os.walk("."):
-        for file in files:
-            filepath = os.path.join(root, file).replace(".\\", "")
-
-            # If not in ignore, collect file text
-            if not ignore_filepath(filepath, ignore_files):
-                with open(filepath, "r") as f:
-                    content = f.read().replace(" " * 4, "\t")
-                files_dict[filepath] = content
-    return files_dict
+	# Iterate over files
+	for root, _, files in os.walk("."):
+		for file in files:
+			filepath = os.path.join(root, file).replace(".\\", "")
+
+			# If not in ignore, collect file text
+			if not ignore_filepath(filepath, ignore_files):
+				with open(filepath, "r") as f:
+					content = f.read()
+				if content:
+					files_dict[filepath] = content.replace(" " * 4, "\t").strip()
+	return files_dict
```

