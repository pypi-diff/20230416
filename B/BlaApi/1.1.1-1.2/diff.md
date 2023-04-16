# Comparing `tmp/BlaApi-1.1.1.tar.gz` & `tmp/BlaApi-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlaApi-1.1.1.tar", last modified: Fri Apr 14 23:00:47 2023, max compression
+gzip compressed data, was "BlaApi-1.2.tar", last modified: Sun Apr 16 17:07:41 2023, max compression
```

## Comparing `BlaApi-1.1.1.tar` & `BlaApi-1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 23:00:47.245520 BlaApi-1.1.1/
-drwxrwxrwx   0        0        0        0 2023-04-14 23:00:47.235528 BlaApi-1.1.1/BlaApi/
--rw-rw-rw-   0        0        0        0 2023-04-14 21:39:20.000000 BlaApi-1.1.1/BlaApi/__init__.py
--rw-rw-rw-   0        0        0     3453 2023-04-14 15:16:36.000000 BlaApi-1.1.1/BlaApi/client.py
--rw-rw-rw-   0        0        0     3739 2023-04-14 22:25:59.000000 BlaApi-1.1.1/BlaApi/diary.py
-drwxrwxrwx   0        0        0        0 2023-04-14 23:00:47.242522 BlaApi-1.1.1/BlaApi.egg-info/
--rw-rw-rw-   0        0        0      750 2023-04-14 23:00:47.000000 BlaApi-1.1.1/BlaApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-04-14 23:00:47.000000 BlaApi-1.1.1/BlaApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 23:00:47.000000 BlaApi-1.1.1/BlaApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-14 23:00:47.000000 BlaApi-1.1.1/BlaApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-14 23:00:47.000000 BlaApi-1.1.1/BlaApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-04-14 15:51:29.000000 BlaApi-1.1.1/LICENSE
--rw-rw-rw-   0        0        0      750 2023-04-14 23:00:47.244520 BlaApi-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       97 2023-04-13 16:43:57.000000 BlaApi-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-14 23:00:47.245520 BlaApi-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     3782 2023-04-14 23:00:42.000000 BlaApi-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:07:41.855654 BlaApi-1.2/
+drwxrwxrwx   0        0        0        0 2023-04-16 17:07:41.842660 BlaApi-1.2/BlaApi/
+-rw-rw-rw-   0        0        0        0 2023-04-16 12:18:24.000000 BlaApi-1.2/BlaApi/__init__.py
+-rw-rw-rw-   0        0        0     3568 2023-04-16 15:55:24.000000 BlaApi-1.2/BlaApi/client.py
+-rw-rw-rw-   0        0        0     3923 2023-04-16 16:19:00.000000 BlaApi-1.2/BlaApi/diary.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:07:41.852657 BlaApi-1.2/BlaApi.egg-info/
+-rw-rw-rw-   0        0        0     5890 2023-04-16 17:07:41.000000 BlaApi-1.2/BlaApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-04-16 17:07:41.000000 BlaApi-1.2/BlaApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 17:07:41.000000 BlaApi-1.2/BlaApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-04-16 17:07:41.000000 BlaApi-1.2/BlaApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-16 17:07:41.000000 BlaApi-1.2/BlaApi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-04-16 12:18:24.000000 BlaApi-1.2/LICENSE
+-rw-rw-rw-   0        0        0     5890 2023-04-16 17:07:41.854655 BlaApi-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5239 2023-04-16 17:06:18.000000 BlaApi-1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-16 17:07:41.855654 BlaApi-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     3706 2023-04-16 17:07:17.000000 BlaApi-1.2/setup.py
```

### Comparing `BlaApi-1.1.1/BlaApi/client.py` & `BlaApi-1.2/BlaApi/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-import os
 import json
 import httpx
 from fake_useragent import UserAgent as ua
 
 class Client:
     client = httpx.Client() # instanciate 
     #! BLA credentials must be passed in as string
     def __init__(self, username: str, password: str):
         # Random UserAgent
         self.headers = {'UserAgent': str(ua().chrome)}
         self.username = username
         self.password = password
         self.token = self.login().get('token')
+        self.student_ids = self.login().get('student_ids')
+        self.student_names = self.login().get('student_names')
         
     def login(self):
         # Construct API endpoint URL
         endpoint = "login"
         api_url = f"https://beaconlightacademy.edu.pk/app/restapi.php?endpoint={endpoint}&rnd=1667581678739&username={self.username}&password={self.password}"
         
         # Send POST request to API endpoint with headers
@@ -45,16 +46,16 @@
             name = s.get('studentName')
             student_names.append(name)
 
 
         # Return retrieved data as dictionary
         output = {
             'token': token,
-            'student_id': student_ids,
-            'student_name': student_names
+            'student_ids': student_ids,
+            'student_names': student_names
 
         }
         return output
 
     def get_diary_list(self):
         # Construct API endpoint URL
         endpoint = "diaryList"
```

### Comparing `BlaApi-1.1.1/BlaApi/diary.py` & `BlaApi-1.2/BlaApi/diary.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,19 +2,24 @@
 from BlaApi.client import Client
 
 class Diary:
     def __init__(self, username, password):
         self.username = username
         self.password = password
         self.client = Client(self.username, self.password)
+        self.student_ids = self.client.student_ids
 
-    def search_by_student_id(self, student_id, passthru=None):
+    def search_by_student(self, student_number=0, passthru=None):
 
         diary = self.client.get_diary_list()
 
+        # select the student id on the index: student_number
+
+        student_id = self.student_ids[student_number]
+        
         # parse output from diary list function
         # if student id is a match then
         # return the diaries as a list
 
         # allows passing of already searched list 
         # to perform further sorting
```

### Comparing `BlaApi-1.1.1/LICENSE` & `BlaApi-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `BlaApi-1.1.1/setup.py` & `BlaApi-1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Package meta-data.
 NAME = 'BlaApi'
 DESCRIPTION = 'A wrapper for the beacon light api.'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'deaddogfuneral@gmail.com'
 AUTHOR = 'Omer-Farooqui'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '1.1.1'
+VERSION = '1.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
      'httpx', 'fake_useragent',
 ]
 
 # What packages are optional?
@@ -93,15 +93,15 @@
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
-    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*", "old", "main", "old"]),
+    packages=find_packages(),
     # If your package is a single module, use this instead of 'packages':
     # py_modules=['mypackage'],
 
     # entry_points={
     #     'console_scripts': ['mycli=mymodule:cli'],
     # },
     install_requires=REQUIRED,
```

