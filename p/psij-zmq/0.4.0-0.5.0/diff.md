# Comparing `tmp/psij-zmq-0.4.0.tar.gz` & `tmp/psij-zmq-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psij-zmq-0.4.0.tar", last modified: Sun Apr 16 13:24:19 2023, max compression
+gzip compressed data, was "psij-zmq-0.5.0.tar", last modified: Sun Apr 16 13:27:43 2023, max compression
```

## Comparing `psij-zmq-0.4.0.tar` & `psij-zmq-0.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 13:24:19.614796 psij-zmq-0.4.0/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1065 2022-10-28 14:30:18.000000 psij-zmq-0.4.0/LICENSE
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      186 2023-04-16 13:22:54.000000 psij-zmq-0.4.0/MANIFEST.in
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      390 2023-04-16 13:24:19.614796 psij-zmq-0.4.0/PKG-INFO
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      180 2023-04-16 12:55:07.000000 psij-zmq-0.4.0/README.md
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        6 2023-04-16 13:24:09.000000 psij-zmq-0.4.0/RELEASE
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 13:24:19.610797 psij-zmq-0.4.0/bin/
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     6648 2023-04-16 12:55:07.000000 psij-zmq-0.4.0/bin/zmq_service.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)       32 2023-04-16 12:55:07.000000 psij-zmq-0.4.0/requirements.txt
--rw-rw-r--   0 merzky    (1001) merzky    (1001)       38 2023-04-16 13:24:19.614796 psij-zmq-0.4.0/setup.cfg
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1025 2023-04-16 13:23:53.000000 psij-zmq-0.4.0/setup.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 13:24:19.610797 psij-zmq-0.4.0/src/
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 13:24:19.610797 psij-zmq-0.4.0/src/psij-descriptors/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      259 2023-04-16 12:55:07.000000 psij-zmq-0.4.0/src/psij-descriptors/zmq_service_descriptor.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 13:24:19.610797 psij-zmq-0.4.0/src/psij-zmq/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        6 2023-04-16 13:24:04.000000 psij-zmq-0.4.0/src/psij-zmq/VERSION
--rw-rw-r--   0 merzky    (1001) merzky    (1001)       97 2023-04-16 12:55:07.000000 psij-zmq-0.4.0/src/psij-zmq/__init__.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 13:24:19.610797 psij-zmq-0.4.0/src/psij-zmq/executors/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      162 2023-04-16 12:55:07.000000 psij-zmq-0.4.0/src/psij-zmq/executors/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     5262 2023-04-16 12:55:07.000000 psij-zmq-0.4.0/src/psij-zmq/executors/zmq_service.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 13:24:19.610797 psij-zmq-0.4.0/src/psij_zmq.egg-info/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      390 2023-04-16 13:24:19.000000 psij-zmq-0.4.0/src/psij_zmq.egg-info/PKG-INFO
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      446 2023-04-16 13:24:19.000000 psij-zmq-0.4.0/src/psij_zmq.egg-info/SOURCES.txt
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        1 2023-04-16 13:24:19.000000 psij-zmq-0.4.0/src/psij_zmq.egg-info/dependency_links.txt
--rw-rw-r--   0 merzky    (1001) merzky    (1001)       32 2023-04-16 13:24:19.000000 psij-zmq-0.4.0/src/psij_zmq.egg-info/requires.txt
--rw-rw-r--   0 merzky    (1001) merzky    (1001)       26 2023-04-16 13:24:19.000000 psij-zmq-0.4.0/src/psij_zmq.egg-info/top_level.txt
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1622 2023-04-16 13:20:38.000000 psij-zmq-0.4.0/tag_and_release.sh
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 13:27:43.385364 psij-zmq-0.5.0/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1065 2022-10-28 14:30:18.000000 psij-zmq-0.5.0/LICENSE
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      186 2023-04-16 13:22:54.000000 psij-zmq-0.5.0/MANIFEST.in
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      390 2023-04-16 13:27:43.385364 psij-zmq-0.5.0/PKG-INFO
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      180 2023-04-16 12:55:07.000000 psij-zmq-0.5.0/README.md
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        6 2023-04-16 13:27:31.000000 psij-zmq-0.5.0/RELEASE
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 13:27:43.385364 psij-zmq-0.5.0/bin/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     6648 2023-04-16 12:55:07.000000 psij-zmq-0.5.0/bin/psij_zmq_service.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       32 2023-04-16 12:55:07.000000 psij-zmq-0.5.0/requirements.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       38 2023-04-16 13:27:43.385364 psij-zmq-0.5.0/setup.cfg
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1030 2023-04-16 13:27:20.000000 psij-zmq-0.5.0/setup.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 13:27:43.385364 psij-zmq-0.5.0/src/
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 13:27:43.385364 psij-zmq-0.5.0/src/psij-descriptors/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      259 2023-04-16 12:55:07.000000 psij-zmq-0.5.0/src/psij-descriptors/zmq_service_descriptor.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 13:27:43.385364 psij-zmq-0.5.0/src/psij-zmq/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        6 2023-04-16 13:27:33.000000 psij-zmq-0.5.0/src/psij-zmq/VERSION
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       97 2023-04-16 12:55:07.000000 psij-zmq-0.5.0/src/psij-zmq/__init__.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 13:27:43.385364 psij-zmq-0.5.0/src/psij-zmq/executors/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      162 2023-04-16 12:55:07.000000 psij-zmq-0.5.0/src/psij-zmq/executors/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     5262 2023-04-16 12:55:07.000000 psij-zmq-0.5.0/src/psij-zmq/executors/zmq_service.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 13:27:43.385364 psij-zmq-0.5.0/src/psij_zmq.egg-info/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      390 2023-04-16 13:27:43.000000 psij-zmq-0.5.0/src/psij_zmq.egg-info/PKG-INFO
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      451 2023-04-16 13:27:43.000000 psij-zmq-0.5.0/src/psij_zmq.egg-info/SOURCES.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        1 2023-04-16 13:27:43.000000 psij-zmq-0.5.0/src/psij_zmq.egg-info/dependency_links.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       32 2023-04-16 13:27:43.000000 psij-zmq-0.5.0/src/psij_zmq.egg-info/requires.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       26 2023-04-16 13:27:43.000000 psij-zmq-0.5.0/src/psij_zmq.egg-info/top_level.txt
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1617 2023-04-16 13:24:37.000000 psij-zmq-0.5.0/tag_and_release.sh
```

### Comparing `psij-zmq-0.4.0/LICENSE` & `psij-zmq-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psij-zmq-0.4.0/bin/zmq_service.py` & `psij-zmq-0.5.0/bin/psij_zmq_service.py`

 * *Files identical despite different names*

### Comparing `psij-zmq-0.4.0/setup.py` & `psij-zmq-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         packages=find_packages(where='src') + ['psij-descriptors'],
         package_dir={'': 'src'},
 
         package_data={
             '': ['README.md', 'LICENSE']
         },
 
-        scripts=['bin/zmq_service.py'],
+        scripts=['bin/psij_zmq_service.py'],
 
         entry_points={
         },
 
         install_requires=install_requires,
         python_requires='>=3.7'
     )
```

### Comparing `psij-zmq-0.4.0/src/psij-zmq/executors/zmq_service.py` & `psij-zmq-0.5.0/src/psij-zmq/executors/zmq_service.py`

 * *Files identical despite different names*

### Comparing `psij-zmq-0.4.0/tag_and_release.sh` & `psij-zmq-0.5.0/tag_and_release.sh`

 * *Files 1% similar despite different names*

```diff
@@ -51,11 +51,11 @@
 
 }
 
 release () {
     echo "======================================================================="
     echo "Push to PyPi. This will require your username and password"
     echo "======================================================================="
-    echo twine upload --skip-existing dist/*
+    twine upload --skip-existing dist/*
 }
 
 "$@"
```

