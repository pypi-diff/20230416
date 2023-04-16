# Comparing `tmp/unvtray-0.2.0.tar.gz` & `tmp/unvtray-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unvtray-0.2.0.tar", last modified: Sun Apr 16 04:57:41 2023, max compression
+gzip compressed data, was "unvtray-0.2.1.tar", last modified: Sun Apr 16 05:26:34 2023, max compression
```

## Comparing `unvtray-0.2.0.tar` & `unvtray-0.2.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.129049 unvtray-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.121049 unvtray-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.125049 unvtray-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-16 04:57:32.000000 unvtray-0.2.0/.github/workflows/build-and-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-16 04:57:32.000000 unvtray-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 04:57:32.000000 unvtray-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-04-16 04:57:41.125049 unvtray-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-04-16 04:57:32.000000 unvtray-0.2.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     2484 2023-04-16 04:57:32.000000 unvtray-0.2.0/make_icons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.125049 unvtray-0.2.0/package/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.121049 unvtray-0.2.0/package/icons/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.125049 unvtray-0.2.0/package/icons/128x128/
--rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-04-16 04:57:32.000000 unvtray-0.2.0/package/icons/128x128/unvtray.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.125049 unvtray-0.2.0/package/icons/256x256/
--rw-r--r--   0 runner    (1001) docker     (123)    56350 2023-04-16 04:57:32.000000 unvtray-0.2.0/package/icons/256x256/unvtray.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.125049 unvtray-0.2.0/package/icons/32x32/
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-16 04:57:32.000000 unvtray-0.2.0/package/icons/32x32/unvtray.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.125049 unvtray-0.2.0/package/icons/512x512/
--rw-r--r--   0 runner    (1001) docker     (123)   165906 2023-04-16 04:57:32.000000 unvtray-0.2.0/package/icons/512x512/unvtray.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.125049 unvtray-0.2.0/package/icons/64x64/
--rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-04-16 04:57:32.000000 unvtray-0.2.0/package/icons/64x64/unvtray.png
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-16 04:57:32.000000 unvtray-0.2.0/package/net.unvanquished.unvtray.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-16 04:57:32.000000 unvtray-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 04:57:41.129049 unvtray-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.125049 unvtray-0.2.0/unvtray/
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-16 04:57:32.000000 unvtray-0.2.0/unvtray/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.125049 unvtray-0.2.0/unvtray/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   203376 2023-04-16 04:57:32.000000 unvtray-0.2.0/unvtray/assets/FreeMonoBold.otf
--rw-r--r--   0 runner    (1001) docker     (123)   218008 2023-04-16 04:57:32.000000 unvtray-0.2.0/unvtray/assets/unvanquished.png
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-16 04:57:32.000000 unvtray-0.2.0/unvtray/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-16 04:57:32.000000 unvtray-0.2.0/unvtray/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-16 04:57:32.000000 unvtray-0.2.0/unvtray/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-04-16 04:57:32.000000 unvtray-0.2.0/unvtray/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-04-16 04:57:32.000000 unvtray-0.2.0/unvtray/servers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-16 04:57:32.000000 unvtray-0.2.0/unvtray/tray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.125049 unvtray-0.2.0/unvtray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-04-16 04:57:41.000000 unvtray-0.2.0/unvtray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-16 04:57:41.000000 unvtray-0.2.0/unvtray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 04:57:41.000000 unvtray-0.2.0/unvtray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-16 04:57:41.000000 unvtray-0.2.0/unvtray.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-16 04:57:41.000000 unvtray-0.2.0/unvtray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-16 04:57:41.000000 unvtray-0.2.0/unvtray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:26:34.917501 unvtray-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:26:34.913500 unvtray-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:26:34.913500 unvtray-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-16 05:26:25.000000 unvtray-0.2.1/.github/workflows/build-and-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-16 05:26:25.000000 unvtray-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 05:26:25.000000 unvtray-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-04-16 05:26:34.917501 unvtray-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-04-16 05:26:25.000000 unvtray-0.2.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2484 2023-04-16 05:26:25.000000 unvtray-0.2.1/make_icons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:26:34.913500 unvtray-0.2.1/package/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:26:34.913500 unvtray-0.2.1/package/icons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:26:34.913500 unvtray-0.2.1/package/icons/128x128/
+-rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-04-16 05:26:25.000000 unvtray-0.2.1/package/icons/128x128/unvtray.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:26:34.913500 unvtray-0.2.1/package/icons/256x256/
+-rw-r--r--   0 runner    (1001) docker     (123)    56350 2023-04-16 05:26:25.000000 unvtray-0.2.1/package/icons/256x256/unvtray.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:26:34.913500 unvtray-0.2.1/package/icons/32x32/
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-16 05:26:25.000000 unvtray-0.2.1/package/icons/32x32/unvtray.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:26:34.913500 unvtray-0.2.1/package/icons/512x512/
+-rw-r--r--   0 runner    (1001) docker     (123)   165906 2023-04-16 05:26:25.000000 unvtray-0.2.1/package/icons/512x512/unvtray.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:26:34.913500 unvtray-0.2.1/package/icons/64x64/
+-rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-04-16 05:26:25.000000 unvtray-0.2.1/package/icons/64x64/unvtray.png
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-16 05:26:25.000000 unvtray-0.2.1/package/net.unvanquished.unvtray.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-16 05:26:25.000000 unvtray-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 05:26:34.917501 unvtray-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:26:34.917501 unvtray-0.2.1/unvtray/
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-16 05:26:25.000000 unvtray-0.2.1/unvtray/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:26:34.917501 unvtray-0.2.1/unvtray/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   203376 2023-04-16 05:26:25.000000 unvtray-0.2.1/unvtray/assets/FreeMonoBold.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   218008 2023-04-16 05:26:25.000000 unvtray-0.2.1/unvtray/assets/unvanquished.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-16 05:26:25.000000 unvtray-0.2.1/unvtray/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-16 05:26:25.000000 unvtray-0.2.1/unvtray/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-16 05:26:25.000000 unvtray-0.2.1/unvtray/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-04-16 05:26:25.000000 unvtray-0.2.1/unvtray/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-04-16 05:26:25.000000 unvtray-0.2.1/unvtray/servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-16 05:26:25.000000 unvtray-0.2.1/unvtray/tray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:26:34.917501 unvtray-0.2.1/unvtray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-04-16 05:26:34.000000 unvtray-0.2.1/unvtray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-16 05:26:34.000000 unvtray-0.2.1/unvtray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 05:26:34.000000 unvtray-0.2.1/unvtray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-16 05:26:34.000000 unvtray-0.2.1/unvtray.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-16 05:26:34.000000 unvtray-0.2.1/unvtray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-16 05:26:34.000000 unvtray-0.2.1/unvtray.egg-info/top_level.txt
```

### Comparing `unvtray-0.2.0/.github/workflows/build-and-publish.yml` & `unvtray-0.2.1/.github/workflows/build-and-publish.yml`

 * *Files identical despite different names*

### Comparing `unvtray-0.2.0/LICENSE.txt` & `unvtray-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `unvtray-0.2.0/PKG-INFO` & `unvtray-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unvtray
-Version: 0.2.0
+Version: 0.2.1
 Summary: Unvanquished Tray
 Author-email: Maximilian Stahlberg <viech@unvanquished.net>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://unvanquished.net
 Project-URL: Repository, https://github.com/Unvanquished/unvanquished-tray-browser
 Keywords: unvanquished
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `unvtray-0.2.0/README.md` & `unvtray-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `unvtray-0.2.0/make_icons.py` & `unvtray-0.2.1/make_icons.py`

 * *Files identical despite different names*

### Comparing `unvtray-0.2.0/package/icons/128x128/unvtray.png` & `unvtray-0.2.1/package/icons/128x128/unvtray.png`

 * *Files identical despite different names*

### Comparing `unvtray-0.2.0/package/icons/256x256/unvtray.png` & `unvtray-0.2.1/package/icons/256x256/unvtray.png`

 * *Files identical despite different names*

### Comparing `unvtray-0.2.0/package/icons/32x32/unvtray.png` & `unvtray-0.2.1/package/icons/32x32/unvtray.png`

 * *Files identical despite different names*

### Comparing `unvtray-0.2.0/package/icons/512x512/unvtray.png` & `unvtray-0.2.1/package/icons/512x512/unvtray.png`

 * *Files identical despite different names*

### Comparing `unvtray-0.2.0/package/icons/64x64/unvtray.png` & `unvtray-0.2.1/package/icons/64x64/unvtray.png`

 * *Files identical despite different names*

### Comparing `unvtray-0.2.0/pyproject.toml` & `unvtray-0.2.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -27,14 +27,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 
 [tool.setuptools]
-packages = ["unvtray"]
+packages = ["unvtray", "unvtray.assets"]
 
 [tool.setuptools.package-data]
 "unvtray.assets" = ["*.otf", "*.png"]
 
 [tool.black]
 line-length = 79
```

### Comparing `unvtray-0.2.0/unvtray/__main__.py` & `unvtray-0.2.1/unvtray/__main__.py`

 * *Files identical despite different names*

### Comparing `unvtray-0.2.0/unvtray/assets/FreeMonoBold.otf` & `unvtray-0.2.1/unvtray/assets/FreeMonoBold.otf`

 * *Files identical despite different names*

### Comparing `unvtray-0.2.0/unvtray/assets/unvanquished.png` & `unvtray-0.2.1/unvtray/assets/unvanquished.png`

 * *Files identical despite different names*

### Comparing `unvtray-0.2.0/unvtray/common.py` & `unvtray-0.2.1/unvtray/common.py`

 * *Files identical despite different names*

### Comparing `unvtray-0.2.0/unvtray/launch.py` & `unvtray-0.2.1/unvtray/launch.py`

 * *Files identical despite different names*

### Comparing `unvtray-0.2.0/unvtray/ping.py` & `unvtray-0.2.1/unvtray/ping.py`

 * *Files identical despite different names*

### Comparing `unvtray-0.2.0/unvtray/server.py` & `unvtray-0.2.1/unvtray/server.py`

 * *Files identical despite different names*

### Comparing `unvtray-0.2.0/unvtray/servers.py` & `unvtray-0.2.1/unvtray/servers.py`

 * *Files identical despite different names*

### Comparing `unvtray-0.2.0/unvtray/tray.py` & `unvtray-0.2.1/unvtray/tray.py`

 * *Files identical despite different names*

### Comparing `unvtray-0.2.0/unvtray.egg-info/PKG-INFO` & `unvtray-0.2.1/unvtray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unvtray
-Version: 0.2.0
+Version: 0.2.1
 Summary: Unvanquished Tray
 Author-email: Maximilian Stahlberg <viech@unvanquished.net>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://unvanquished.net
 Project-URL: Repository, https://github.com/Unvanquished/unvanquished-tray-browser
 Keywords: unvanquished
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `unvtray-0.2.0/unvtray.egg-info/SOURCES.txt` & `unvtray-0.2.1/unvtray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

