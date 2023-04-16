# Comparing `tmp/easy-file-process-0.1.0.tar.gz` & `tmp/easy-file-process-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy-file-process-0.1.0.tar", last modified: Sun Apr 16 08:49:13 2023, max compression
+gzip compressed data, was "easy-file-process-0.1.1.tar", last modified: Sun Apr 16 09:43:38 2023, max compression
```

## Comparing `easy-file-process-0.1.0.tar` & `easy-file-process-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 08:49:13.380927 easy-file-process-0.1.0/
--rw-rw-rw-   0        0        0     1088 2023-04-16 08:07:53.000000 easy-file-process-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      740 2023-04-16 08:49:13.379410 easy-file-process-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       47 2023-04-16 08:20:16.000000 easy-file-process-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 08:49:13.291373 easy-file-process-0.1.0/easy_file_process.egg-info/
--rw-rw-rw-   0        0        0      740 2023-04-16 08:49:12.000000 easy-file-process-0.1.0/easy_file_process.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-04-16 08:49:12.000000 easy-file-process-0.1.0/easy_file_process.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 08:49:12.000000 easy-file-process-0.1.0/easy_file_process.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-04-16 08:49:12.000000 easy-file-process-0.1.0/easy_file_process.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-16 08:49:12.000000 easy-file-process-0.1.0/easy_file_process.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13199 2023-03-01 02:46:34.000000 easy-file-process-0.1.0/file.py
--rw-rw-rw-   0        0        0       42 2023-04-16 08:49:13.380927 easy-file-process-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     4004 2023-04-16 08:48:13.000000 easy-file-process-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 09:43:38.402078 easy-file-process-0.1.1/
+-rw-rw-rw-   0        0        0     1088 2023-04-16 08:07:53.000000 easy-file-process-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      740 2023-04-16 09:43:38.399498 easy-file-process-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2023-04-16 08:20:16.000000 easy-file-process-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 09:43:38.287818 easy-file-process-0.1.1/easy_file_process.egg-info/
+-rw-rw-rw-   0        0        0      740 2023-04-16 09:43:37.000000 easy-file-process-0.1.1/easy_file_process.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-04-16 09:43:37.000000 easy-file-process-0.1.1/easy_file_process.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 09:43:37.000000 easy-file-process-0.1.1/easy_file_process.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-04-16 09:43:37.000000 easy-file-process-0.1.1/easy_file_process.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-16 09:43:37.000000 easy-file-process-0.1.1/easy_file_process.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 09:43:38.395763 easy-file-process-0.1.1/file/
+-rw-rw-rw-   0        0        0    13199 2023-03-01 02:46:34.000000 easy-file-process-0.1.1/file/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-04-16 09:43:38.402078 easy-file-process-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     4030 2023-04-16 09:43:18.000000 easy-file-process-0.1.1/setup.py
```

### Comparing `easy-file-process-0.1.0/LICENSE` & `easy-file-process-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easy-file-process-0.1.0/PKG-INFO` & `easy-file-process-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-file-process
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple encapsulation of basic file operations
 Home-page: https://github.com/caojiachen1/simple-file-process
 Author: Billy Cao
 Author-email: caojiachen1@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `easy-file-process-0.1.0/easy_file_process.egg-info/PKG-INFO` & `easy-file-process-0.1.1/easy_file_process.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-file-process
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple encapsulation of basic file operations
 Home-page: https://github.com/caojiachen1/simple-file-process
 Author: Billy Cao
 Author-email: caojiachen1@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `easy-file-process-0.1.0/file.py` & `easy-file-process-0.1.1/file/__init__.py`

 * *Files identical despite different names*

### Comparing `easy-file-process-0.1.0/setup.py` & `easy-file-process-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'easy-file-process'
 DESCRIPTION = 'A simple encapsulation of basic file operations'
 URL = 'https://github.com/caojiachen1/simple-file-process'
 EMAIL = 'caojiachen1@outlook.com'
 AUTHOR = 'Billy Cao'
 REQUIRES_PYTHON = '>=3.10.0'
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'moviepy' , 'opencv-python' , 'ffmpeg' , 'pypdf2'
     # 'requests', 'maya', 'records',
 ]
 
@@ -101,16 +101,17 @@
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
     # packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
+    packages=['file'],
     # If your package is a single module, use this instead of 'packages':
-    py_modules=['file'],
+    # py_modules=['file'],
 
     # entry_points={
     #     'console_scripts': ['mycli=mymodule:cli'],
     # },
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
```

