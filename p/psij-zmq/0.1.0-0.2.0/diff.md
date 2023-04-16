# Comparing `tmp/psij-zmq-0.1.0.tar.gz` & `tmp/psij-zmq-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psij-zmq-0.1.0.tar", last modified: Sun Apr 16 12:56:17 2023, max compression
+gzip compressed data, was "psij-zmq-0.2.0.tar", last modified: Sun Apr 16 13:02:04 2023, max compression
```

## Comparing `psij-zmq-0.1.0.tar` & `psij-zmq-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 12:56:17.711206 psij-zmq-0.1.0/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1065 2022-10-28 14:30:18.000000 psij-zmq-0.1.0/LICENSE
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      390 2023-04-16 12:56:17.711206 psij-zmq-0.1.0/PKG-INFO
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      180 2023-04-16 12:55:07.000000 psij-zmq-0.1.0/README.md
--rw-rw-r--   0 merzky    (1001) merzky    (1001)       38 2023-04-16 12:56:17.711206 psij-zmq-0.1.0/setup.cfg
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      997 2023-04-16 12:55:07.000000 psij-zmq-0.1.0/setup.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 12:56:17.711206 psij-zmq-0.1.0/src/
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 12:56:17.711206 psij-zmq-0.1.0/src/psij-descriptors/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      259 2023-04-16 12:55:07.000000 psij-zmq-0.1.0/src/psij-descriptors/zmq_service_descriptor.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 12:56:17.711206 psij-zmq-0.1.0/src/psij-zmq/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)       97 2023-04-16 12:55:07.000000 psij-zmq-0.1.0/src/psij-zmq/__init__.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 12:56:17.711206 psij-zmq-0.1.0/src/psij-zmq/executors/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      162 2023-04-16 12:55:07.000000 psij-zmq-0.1.0/src/psij-zmq/executors/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     5262 2023-04-16 12:55:07.000000 psij-zmq-0.1.0/src/psij-zmq/executors/zmq_service.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      137 2023-04-16 12:55:07.000000 psij-zmq-0.1.0/src/psij-zmq/version.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 12:56:17.711206 psij-zmq-0.1.0/src/psij_zmq.egg-info/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      390 2023-04-16 12:56:17.000000 psij-zmq-0.1.0/src/psij_zmq.egg-info/PKG-INFO
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      374 2023-04-16 12:56:17.000000 psij-zmq-0.1.0/src/psij_zmq.egg-info/SOURCES.txt
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        1 2023-04-16 12:56:17.000000 psij-zmq-0.1.0/src/psij_zmq.egg-info/dependency_links.txt
--rw-rw-r--   0 merzky    (1001) merzky    (1001)       32 2023-04-16 12:56:17.000000 psij-zmq-0.1.0/src/psij_zmq.egg-info/requires.txt
--rw-rw-r--   0 merzky    (1001) merzky    (1001)       26 2023-04-16 12:56:17.000000 psij-zmq-0.1.0/src/psij_zmq.egg-info/top_level.txt
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 13:02:04.010134 psij-zmq-0.2.0/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1065 2022-10-28 14:30:18.000000 psij-zmq-0.2.0/LICENSE
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      146 2023-04-16 13:00:30.000000 psij-zmq-0.2.0/MANIFEST.in
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      390 2023-04-16 13:02:04.010134 psij-zmq-0.2.0/PKG-INFO
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      180 2023-04-16 12:55:07.000000 psij-zmq-0.2.0/README.md
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        6 2023-04-16 13:00:50.000000 psij-zmq-0.2.0/RELEASE
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       32 2023-04-16 12:55:07.000000 psij-zmq-0.2.0/requirements.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       38 2023-04-16 13:02:04.010134 psij-zmq-0.2.0/setup.cfg
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      997 2023-04-16 12:55:07.000000 psij-zmq-0.2.0/setup.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 13:02:04.006134 psij-zmq-0.2.0/src/
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 13:02:04.010134 psij-zmq-0.2.0/src/psij-descriptors/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      259 2023-04-16 12:55:07.000000 psij-zmq-0.2.0/src/psij-descriptors/zmq_service_descriptor.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 13:02:04.010134 psij-zmq-0.2.0/src/psij-zmq/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       97 2023-04-16 12:55:07.000000 psij-zmq-0.2.0/src/psij-zmq/__init__.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 13:02:04.010134 psij-zmq-0.2.0/src/psij-zmq/executors/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      162 2023-04-16 12:55:07.000000 psij-zmq-0.2.0/src/psij-zmq/executors/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     5262 2023-04-16 12:55:07.000000 psij-zmq-0.2.0/src/psij-zmq/executors/zmq_service.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      137 2023-04-16 13:01:43.000000 psij-zmq-0.2.0/src/psij-zmq/version.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2023-04-16 13:02:04.010134 psij-zmq-0.2.0/src/psij_zmq.egg-info/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      390 2023-04-16 13:02:03.000000 psij-zmq-0.2.0/src/psij_zmq.egg-info/PKG-INFO
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      430 2023-04-16 13:02:03.000000 psij-zmq-0.2.0/src/psij_zmq.egg-info/SOURCES.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        1 2023-04-16 13:02:03.000000 psij-zmq-0.2.0/src/psij_zmq.egg-info/dependency_links.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       32 2023-04-16 13:02:03.000000 psij-zmq-0.2.0/src/psij_zmq.egg-info/requires.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       26 2023-04-16 13:02:03.000000 psij-zmq-0.2.0/src/psij_zmq.egg-info/top_level.txt
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1653 2023-04-16 12:55:07.000000 psij-zmq-0.2.0/tag_and_release.sh
```

### Comparing `psij-zmq-0.1.0/LICENSE` & `psij-zmq-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psij-zmq-0.1.0/setup.py` & `psij-zmq-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `psij-zmq-0.1.0/src/psij-zmq/executors/zmq_service.py` & `psij-zmq-0.2.0/src/psij-zmq/executors/zmq_service.py`

 * *Files identical despite different names*

