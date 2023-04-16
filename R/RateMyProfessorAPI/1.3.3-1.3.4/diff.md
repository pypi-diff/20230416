# Comparing `tmp/RateMyProfessorAPI-1.3.3.tar.gz` & `tmp/RateMyProfessorAPI-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RateMyProfessorAPI-1.3.3.tar", last modified: Wed Dec 28 23:37:56 2022, max compression
+gzip compressed data, was "RateMyProfessorAPI-1.3.4.tar", last modified: Sun Apr 16 21:19:42 2023, max compression
```

## Comparing `RateMyProfessorAPI-1.3.3.tar` & `RateMyProfessorAPI-1.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 23:37:56.896709 RateMyProfessorAPI-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2022-12-28 23:37:45.000000 RateMyProfessorAPI-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       64 2022-12-28 23:37:45.000000 RateMyProfessorAPI-1.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2022-12-28 23:37:56.896709 RateMyProfessorAPI-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2022-12-28 23:37:45.000000 RateMyProfessorAPI-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 23:37:56.896709 RateMyProfessorAPI-1.3.3/RateMyProfessorAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2022-12-28 23:37:56.000000 RateMyProfessorAPI-1.3.3/RateMyProfessorAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2022-12-28 23:37:56.000000 RateMyProfessorAPI-1.3.3/RateMyProfessorAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-28 23:37:56.000000 RateMyProfessorAPI-1.3.3/RateMyProfessorAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2022-12-28 23:37:56.000000 RateMyProfessorAPI-1.3.3/RateMyProfessorAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-28 23:37:56.000000 RateMyProfessorAPI-1.3.3/RateMyProfessorAPI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 23:37:56.896709 RateMyProfessorAPI-1.3.3/ratemyprofessor/
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2022-12-28 23:37:45.000000 RateMyProfessorAPI-1.3.3/ratemyprofessor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 23:37:56.896709 RateMyProfessorAPI-1.3.3/ratemyprofessor/json/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2022-12-28 23:37:45.000000 RateMyProfessorAPI-1.3.3/ratemyprofessor/json/header.json
--rw-r--r--   0 runner    (1001) docker     (123)      242 2022-12-28 23:37:45.000000 RateMyProfessorAPI-1.3.3/ratemyprofessor/json/professorquery.json
--rw-r--r--   0 runner    (1001) docker     (123)      442 2022-12-28 23:37:45.000000 RateMyProfessorAPI-1.3.3/ratemyprofessor/json/ratingsquery.json
--rw-r--r--   0 runner    (1001) docker     (123)     8092 2022-12-28 23:37:45.000000 RateMyProfessorAPI-1.3.3/ratemyprofessor/professor.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2022-12-28 23:37:45.000000 RateMyProfessorAPI-1.3.3/ratemyprofessor/school.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-28 23:37:56.896709 RateMyProfessorAPI-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2022-12-28 23:37:45.000000 RateMyProfessorAPI-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:19:42.083994 RateMyProfessorAPI-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-16 21:19:29.000000 RateMyProfessorAPI-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-16 21:19:29.000000 RateMyProfessorAPI-1.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-16 21:19:42.083994 RateMyProfessorAPI-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-16 21:19:29.000000 RateMyProfessorAPI-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:19:42.083994 RateMyProfessorAPI-1.3.4/RateMyProfessorAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-16 21:19:42.000000 RateMyProfessorAPI-1.3.4/RateMyProfessorAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-16 21:19:42.000000 RateMyProfessorAPI-1.3.4/RateMyProfessorAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 21:19:42.000000 RateMyProfessorAPI-1.3.4/RateMyProfessorAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-16 21:19:42.000000 RateMyProfessorAPI-1.3.4/RateMyProfessorAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-16 21:19:42.000000 RateMyProfessorAPI-1.3.4/RateMyProfessorAPI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:19:42.083994 RateMyProfessorAPI-1.3.4/ratemyprofessor/
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-16 21:19:29.000000 RateMyProfessorAPI-1.3.4/ratemyprofessor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:19:42.083994 RateMyProfessorAPI-1.3.4/ratemyprofessor/json/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-16 21:19:29.000000 RateMyProfessorAPI-1.3.4/ratemyprofessor/json/header.json
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-16 21:19:29.000000 RateMyProfessorAPI-1.3.4/ratemyprofessor/json/professorquery.json
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-16 21:19:29.000000 RateMyProfessorAPI-1.3.4/ratemyprofessor/json/ratingsquery.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-04-16 21:19:29.000000 RateMyProfessorAPI-1.3.4/ratemyprofessor/professor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-16 21:19:29.000000 RateMyProfessorAPI-1.3.4/ratemyprofessor/school.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-16 21:19:42.083994 RateMyProfessorAPI-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-16 21:19:29.000000 RateMyProfessorAPI-1.3.4/setup.py
```

### Comparing `RateMyProfessorAPI-1.3.3/LICENSE` & `RateMyProfessorAPI-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `RateMyProfessorAPI-1.3.3/PKG-INFO` & `RateMyProfessorAPI-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RateMyProfessorAPI
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python web scraper to get professor ratings from ratemyprofessor.com website.
 Home-page: https://github.com/Nobelz/RateMyProfessorAPI
 Author: Nobel Zhou
 Author-email: nxz157@case.edu
 Project-URL: Issue Tracker, https://github.com/Nobelz/RateMyProfessorAPI/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `RateMyProfessorAPI-1.3.3/README.md` & `RateMyProfessorAPI-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `RateMyProfessorAPI-1.3.3/RateMyProfessorAPI.egg-info/PKG-INFO` & `RateMyProfessorAPI-1.3.4/RateMyProfessorAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RateMyProfessorAPI
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python web scraper to get professor ratings from ratemyprofessor.com website.
 Home-page: https://github.com/Nobelz/RateMyProfessorAPI
 Author: Nobel Zhou
 Author-email: nxz157@case.edu
 Project-URL: Issue Tracker, https://github.com/Nobelz/RateMyProfessorAPI/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `RateMyProfessorAPI-1.3.3/ratemyprofessor/__init__.py` & `RateMyProfessorAPI-1.3.4/ratemyprofessor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     :param school_name: The school's name.
     :return: List of schools that match the school name. If no schools are found, this will return an empty list.
     """
     school_name.replace(' ', '+')
     url = "https://www.ratemyprofessors.com/search/schools?query=%s" % school_name
     page = requests.get(url)
-    data = re.findall(r'/school\?sid=(\d+)', page.text)
+    data = re.findall(r'"legacyId":(\d+)', page.text)
     school_list = []
 
     for school_data in data:
         try:
             school_list.append(School(int(school_data)))
         except ValueError:
             pass
```

### Comparing `RateMyProfessorAPI-1.3.3/ratemyprofessor/professor.py` & `RateMyProfessorAPI-1.3.4/ratemyprofessor/professor.py`

 * *Files identical despite different names*

### Comparing `RateMyProfessorAPI-1.3.3/ratemyprofessor/school.py` & `RateMyProfessorAPI-1.3.4/ratemyprofessor/school.py`

 * *Files identical despite different names*

### Comparing `RateMyProfessorAPI-1.3.3/setup.py` & `RateMyProfessorAPI-1.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='RateMyProfessorAPI',
-    version='1.3.3',
+    version='1.3.4',
     description='Python web scraper to get professor ratings from ratemyprofessor.com website.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Nobelz/RateMyProfessorAPI',
     author='Nobel Zhou',
     author_email='nxz157@case.edu',
     classifiers=[
```

