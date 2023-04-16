# Comparing `tmp/capsolver-api-1.0.1.tar.gz` & `tmp/capsolver_api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capsolver-api-1.0.1.tar", last modified: Tue Apr 11 21:44:30 2023, max compression
+gzip compressed data, was "capsolver_api-1.0.2.tar", last modified: Sun Apr 16 14:48:05 2023, max compression
```

## Comparing `capsolver-api-1.0.1.tar` & `capsolver_api-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 21:44:30.420220 capsolver-api-1.0.1/
--rw-rw-rw-   0        0        0      501 2023-04-11 21:44:30.420220 capsolver-api-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-11 21:44:30.420220 capsolver-api-1.0.1/capsolver_api.egg-info/
--rw-rw-rw-   0        0        0      501 2023-04-11 21:44:30.000000 capsolver-api-1.0.1/capsolver_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-04-11 21:44:30.000000 capsolver-api-1.0.1/capsolver_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 21:44:30.000000 capsolver-api-1.0.1/capsolver_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-11 21:44:30.000000 capsolver-api-1.0.1/capsolver_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-11 21:44:30.000000 capsolver-api-1.0.1/capsolver_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 21:44:30.420220 capsolver-api-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      849 2023-04-11 21:44:13.000000 capsolver-api-1.0.1/setup.py
--rw-rw-rw-   0        0        0      733 2023-04-11 20:21:54.000000 capsolver-api-1.0.1/tester.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:48:05.046254 capsolver_api-1.0.2/
+-rw-rw-rw-   0        0        0      501 2023-04-16 14:48:05.045743 capsolver_api-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 14:48:05.044209 capsolver_api-1.0.2/capsolver_api.egg-info/
+-rw-rw-rw-   0        0        0      501 2023-04-16 14:48:04.000000 capsolver_api-1.0.2/capsolver_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-04-16 14:48:04.000000 capsolver_api-1.0.2/capsolver_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 14:48:04.000000 capsolver_api-1.0.2/capsolver_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-16 14:48:04.000000 capsolver_api-1.0.2/capsolver_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-16 14:48:04.000000 capsolver_api-1.0.2/capsolver_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 14:48:05.046766 capsolver_api-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      833 2023-04-16 14:48:02.000000 capsolver_api-1.0.2/setup.py
+-rw-rw-rw-   0        0        0      733 2023-04-11 20:21:54.000000 capsolver_api-1.0.2/tester.py
```

### Comparing `capsolver-api-1.0.1/setup.py` & `capsolver_api-1.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,29 +3,27 @@
 classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ]
 
 setup(
-    name='capsolver-api',
-    version='1.0.1',
+    name='capsolver_api',
+    version='1.0.2',
     author='seadhy',
     author_email='seadhy@protonmail.com',
     description='capsolver python libary',
     long_description='i will write',
     long_description_content_type="text/markdown",
     url="https://github.com/seadhy/capsolver-api",
     project_urls={
         "Bug Tracker": "https://github.com/seadhy/capsolver-api/issues",
     },
     classifiers=classifiers,
 
-    install_requires=[
-        "requests",
-    ],
+    install_requires=["requests"],
     packages=find_packages(),
-    package_dir={"capsolver_py": ""},
+    package_dir={"capsolver_api": ""},
     include_package_data=True,
     python_requires=">=3",
 
 )
```

### Comparing `capsolver-api-1.0.1/tester.py` & `capsolver_api-1.0.2/tester.py`

 * *Files identical despite different names*

