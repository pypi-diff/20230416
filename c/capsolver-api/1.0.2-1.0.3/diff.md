# Comparing `tmp/capsolver_api-1.0.2.tar.gz` & `tmp/capsolver_api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capsolver_api-1.0.2.tar", last modified: Sun Apr 16 14:48:05 2023, max compression
+gzip compressed data, was "capsolver_api-1.0.3.tar", last modified: Sun Apr 16 15:28:50 2023, max compression
```

## Comparing `capsolver_api-1.0.2.tar` & `capsolver_api-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 14:48:05.046254 capsolver_api-1.0.2/
--rw-rw-rw-   0        0        0      501 2023-04-16 14:48:05.045743 capsolver_api-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 14:48:05.044209 capsolver_api-1.0.2/capsolver_api.egg-info/
--rw-rw-rw-   0        0        0      501 2023-04-16 14:48:04.000000 capsolver_api-1.0.2/capsolver_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-04-16 14:48:04.000000 capsolver_api-1.0.2/capsolver_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 14:48:04.000000 capsolver_api-1.0.2/capsolver_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-16 14:48:04.000000 capsolver_api-1.0.2/capsolver_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-16 14:48:04.000000 capsolver_api-1.0.2/capsolver_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 14:48:05.046766 capsolver_api-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      833 2023-04-16 14:48:02.000000 capsolver_api-1.0.2/setup.py
--rw-rw-rw-   0        0        0      733 2023-04-11 20:21:54.000000 capsolver_api-1.0.2/tester.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:28:50.647375 capsolver_api-1.0.3/
+-rw-rw-rw-   0        0        0      501 2023-04-16 15:28:50.646863 capsolver_api-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 15:28:50.618523 capsolver_api-1.0.3/capsolver_api/
+-rw-rw-rw-   0        0        0      736 2023-04-07 21:00:53.000000 capsolver_api-1.0.3/capsolver_api/__init__.py
+-rw-rw-rw-   0        0        0     3853 2023-04-08 10:03:50.000000 capsolver_api-1.0.3/capsolver_api/capsolver_py.py
+-rw-rw-rw-   0        0        0      205 2023-04-08 08:44:48.000000 capsolver_api-1.0.3/capsolver_api/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:28:50.632427 capsolver_api-1.0.3/capsolver_api/recognitions/
+-rw-rw-rw-   0        0        0     1054 2023-04-08 09:37:26.000000 capsolver_api-1.0.3/capsolver_api/recognitions/aws_waf.py
+-rw-rw-rw-   0        0        0     1062 2023-04-08 09:37:26.000000 capsolver_api-1.0.3/capsolver_api/recognitions/funcaptcha.py
+-rw-rw-rw-   0        0        0     1062 2023-04-08 09:37:26.000000 capsolver_api-1.0.3/capsolver_api/recognitions/hcaptcha.py
+-rw-rw-rw-   0        0        0     1301 2023-04-07 20:39:29.000000 capsolver_api-1.0.3/capsolver_api/recognitions/image_to_task.py
+-rw-rw-rw-   0        0        0     1007 2023-04-08 09:37:59.000000 capsolver_api-1.0.3/capsolver_api/recognitions/recaptcha.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:28:50.645835 capsolver_api-1.0.3/capsolver_api/tasks/
+-rw-rw-rw-   0        0        0     1279 2023-04-08 09:34:47.000000 capsolver_api-1.0.3/capsolver_api/tasks/cloudflare_challenge.py
+-rw-rw-rw-   0        0        0     1280 2023-04-08 09:33:49.000000 capsolver_api-1.0.3/capsolver_api/tasks/cloudflare_turnstile.py
+-rw-rw-rw-   0        0        0     1302 2023-04-08 09:34:38.000000 capsolver_api-1.0.3/capsolver_api/tasks/datadome.py
+-rw-rw-rw-   0        0        0     1544 2023-04-08 09:34:31.000000 capsolver_api-1.0.3/capsolver_api/tasks/funcaptcha.py
+-rw-rw-rw-   0        0        0     1874 2023-04-08 09:34:23.000000 capsolver_api-1.0.3/capsolver_api/tasks/geetest.py
+-rw-rw-rw-   0        0        0     2047 2023-04-08 09:34:15.000000 capsolver_api-1.0.3/capsolver_api/tasks/hcaptcha.py
+-rw-rw-rw-   0        0        0     1250 2023-04-08 09:34:09.000000 capsolver_api-1.0.3/capsolver_api/tasks/mtcaptcha.py
+-rw-rw-rw-   0        0        0     2056 2023-04-08 09:34:03.000000 capsolver_api-1.0.3/capsolver_api/tasks/recaptchav2.py
+-rw-rw-rw-   0        0        0     2146 2023-04-08 09:33:58.000000 capsolver_api-1.0.3/capsolver_api/tasks/recaptchav3.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:28:50.625218 capsolver_api-1.0.3/capsolver_api.egg-info/
+-rw-rw-rw-   0        0        0      501 2023-04-16 15:28:50.000000 capsolver_api-1.0.3/capsolver_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      798 2023-04-16 15:28:50.000000 capsolver_api-1.0.3/capsolver_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 15:28:50.000000 capsolver_api-1.0.3/capsolver_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-16 15:28:50.000000 capsolver_api-1.0.3/capsolver_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-16 15:28:50.000000 capsolver_api-1.0.3/capsolver_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 15:28:50.647895 capsolver_api-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      872 2023-04-16 15:28:43.000000 capsolver_api-1.0.3/setup.py
```

### Comparing `capsolver_api-1.0.2/setup.py` & `capsolver_api-1.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup, find_packages
 
+print(find_packages())
+
 classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ]
 
 setup(
     name='capsolver_api',
-    version='1.0.2',
+    version='1.0.3',
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
-
     install_requires=["requests"],
-    packages=find_packages(),
-    package_dir={"capsolver_api": ""},
+    packages=['capsolver_api', 'capsolver_api.tasks', 'capsolver_api.recognitions'],
     include_package_data=True,
     python_requires=">=3",
 
 )
```

