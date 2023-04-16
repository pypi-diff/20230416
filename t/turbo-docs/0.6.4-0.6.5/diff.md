# Comparing `tmp/turbo_docs-0.6.4.tar.gz` & `tmp/turbo_docs-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\turbo_docs-0.6.4.tar", last modified: Sun Apr 16 15:37:08 2023, max compression
+gzip compressed data, was "turbo_docs-0.6.5.tar", last modified: Sun Apr 16 16:10:30 2023, max compression
```

## Comparing `turbo_docs-0.6.4.tar` & `turbo_docs-0.6.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 15:37:08.091327 turbo_docs-0.6.4/
--rw-rw-rw-   0        0        0     1805 2023-04-16 15:37:08.091327 turbo_docs-0.6.4/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2023-04-16 15:34:04.000000 turbo_docs-0.6.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-16 15:37:08.092335 turbo_docs-0.6.4/setup.cfg
--rw-rw-rw-   0        0        0      726 2023-04-16 15:35:24.000000 turbo_docs-0.6.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:37:08.061574 turbo_docs-0.6.4/turbo_docs/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.6.4/turbo_docs/__init__.py
--rw-rw-rw-   0        0        0     5623 2023-04-16 15:25:13.000000 turbo_docs-0.6.4/turbo_docs/generate.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:37:08.088812 turbo_docs-0.6.4/turbo_docs/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.6.4/turbo_docs/utils/__init__.py
--rw-rw-rw-   0        0        0     1471 2023-04-16 15:13:12.000000 turbo_docs-0.6.4/turbo_docs/utils/cli_options.py
--rw-rw-rw-   0        0        0     1624 2023-04-16 15:18:24.000000 turbo_docs-0.6.4/turbo_docs/utils/directory.py
--rw-rw-rw-   0        0        0      763 2023-04-16 15:13:17.000000 turbo_docs-0.6.4/turbo_docs/utils/openai_api.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:37:08.082810 turbo_docs-0.6.4/turbo_docs.egg-info/
--rw-rw-rw-   0        0        0     1805 2023-04-16 15:37:07.000000 turbo_docs-0.6.4/turbo_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-04-16 15:37:07.000000 turbo_docs-0.6.4/turbo_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 15:37:07.000000 turbo_docs-0.6.4/turbo_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-16 15:37:07.000000 turbo_docs-0.6.4/turbo_docs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-04-16 15:37:07.000000 turbo_docs-0.6.4/turbo_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-16 15:37:07.000000 turbo_docs-0.6.4/turbo_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 16:10:30.741118 turbo_docs-0.6.5/
+-rw-rw-rw-   0        0        0     1862 2023-04-16 16:10:30.740124 turbo_docs-0.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2023-04-16 15:34:04.000000 turbo_docs-0.6.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-16 16:10:30.742119 turbo_docs-0.6.5/setup.cfg
+-rw-rw-rw-   0        0        0      726 2023-04-16 16:09:43.000000 turbo_docs-0.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:10:30.721076 turbo_docs-0.6.5/turbo_docs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.6.5/turbo_docs/__init__.py
+-rw-rw-rw-   0        0        0     6057 2023-04-16 16:08:18.000000 turbo_docs-0.6.5/turbo_docs/generate.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:10:30.738120 turbo_docs-0.6.5/turbo_docs/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.6.5/turbo_docs/utils/__init__.py
+-rw-rw-rw-   0        0        0     1471 2023-04-16 15:13:12.000000 turbo_docs-0.6.5/turbo_docs/utils/cli_options.py
+-rw-rw-rw-   0        0        0     1624 2023-04-16 15:18:24.000000 turbo_docs-0.6.5/turbo_docs/utils/directory.py
+-rw-rw-rw-   0        0        0      763 2023-04-16 15:13:17.000000 turbo_docs-0.6.5/turbo_docs/utils/openai_api.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:10:30.731078 turbo_docs-0.6.5/turbo_docs.egg-info/
+-rw-rw-rw-   0        0        0     1862 2023-04-16 16:10:30.000000 turbo_docs-0.6.5/turbo_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-04-16 16:10:30.000000 turbo_docs-0.6.5/turbo_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 16:10:30.000000 turbo_docs-0.6.5/turbo_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-16 16:10:30.000000 turbo_docs-0.6.5/turbo_docs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-04-16 16:10:30.000000 turbo_docs-0.6.5/turbo_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-16 16:10:30.000000 turbo_docs-0.6.5/turbo_docs.egg-info/top_level.txt
```

### Comparing `turbo_docs-0.6.4/PKG-INFO` & `turbo_docs-0.6.5/turbo_docs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 Metadata-Version: 2.1
-Name: turbo_docs
-Version: 0.6.4
+Name: turbo-docs
+Version: 0.6.5
+Summary: UNKNOWN
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -60,7 +63,8 @@
 ```
 
 Copy all code files in the directory to the clipboard:
 
 ``` 
 python generate.py --copy
 ```
+
```

### Comparing `turbo_docs-0.6.4/README.md` & `turbo_docs-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.6.4/setup.py` & `turbo_docs-0.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name="turbo_docs",
-	version="0.6.4",
+	version="0.6.5",
 	packages=find_packages(),
 	install_requires=[
 		"requests",
 		"openai",
 		"click",
 		"pyperclip",
 	],
```

### Comparing `turbo_docs-0.6.4/turbo_docs/generate.py` & `turbo_docs-0.6.5/turbo_docs/generate.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,16 +124,24 @@
 
 					prompt = f'Generate a concise docstring for the following Python function. Do not include argurments and returns.\n\n{func.dumps()}'
 					docstring = openai_api.gpt_completion_wrapper(prompt)
 					docstring_formatted = format_docstring(docstring)
 					func.value.insert(0, docstring_formatted)
 
 				# Write the modified code back to the file
-				with open(file_path, "w") as f:
-					f.write(red.dumps())
+				try:
+					with open(file_path, "w") as f:
+						f.write(red.dumps())
+				except PermissionError:
+					print(f"Permission denied for file: {file_path}.")
+					print("To resolve this issue, please try the following steps:")
+					print("1. Close the file if it is open in any text editor or IDE.")
+					print("2. Check the file permissions and ensure your user account has write access.")
+					print("3. Run the command prompt or terminal with administrator privileges.")		
+					break		
 
 
 @click.command()
 @cli_options.copy
 @cli_options.create_readme
 @cli_options.create_readme_plus
 @cli_options.create_tests
```

### Comparing `turbo_docs-0.6.4/turbo_docs/utils/cli_options.py` & `turbo_docs-0.6.5/turbo_docs/utils/cli_options.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.6.4/turbo_docs/utils/directory.py` & `turbo_docs-0.6.5/turbo_docs/utils/directory.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.6.4/turbo_docs/utils/openai_api.py` & `turbo_docs-0.6.5/turbo_docs/utils/openai_api.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.6.4/turbo_docs.egg-info/PKG-INFO` & `turbo_docs-0.6.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 Metadata-Version: 2.1
-Name: turbo-docs
-Version: 0.6.4
+Name: turbo_docs
+Version: 0.6.5
+Summary: UNKNOWN
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -60,7 +63,8 @@
 ```
 
 Copy all code files in the directory to the clipboard:
 
 ``` 
 python generate.py --copy
 ```
+
```

