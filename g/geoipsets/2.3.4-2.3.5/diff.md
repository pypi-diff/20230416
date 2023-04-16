# Comparing `tmp/geoipsets-2.3.4.tar.gz` & `tmp/geoipsets-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoipsets-2.3.4.tar", last modified: Tue May  3 02:24:30 2022, max compression
+gzip compressed data, was "geoipsets-2.3.5.tar", last modified: Sun Apr 16 20:52:26 2023, max compression
```

## Comparing `geoipsets-2.3.4.tar` & `geoipsets-2.3.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jules     (1000) jules     (1000)        0 2022-05-03 02:24:30.851465 geoipsets-2.3.4/
--rw-r--r--   0 jules     (1000) jules     (1000)       26 2021-12-22 19:45:35.000000 geoipsets-2.3.4/MANIFEST.in
--rw-r--r--   0 jules     (1000) jules     (1000)     3557 2022-05-03 02:24:30.851465 geoipsets-2.3.4/PKG-INFO
--rw-r--r--   0 jules     (1000) jules     (1000)     2973 2022-05-03 01:30:24.000000 geoipsets-2.3.4/README.md
-drwxr-xr-x   0 jules     (1000) jules     (1000)        0 2022-05-03 02:24:30.851465 geoipsets-2.3.4/geoipsets/
--rw-r--r--   0 jules     (1000) jules     (1000)        6 2022-05-03 02:16:04.000000 geoipsets-2.3.4/geoipsets/VERSION
--rw-r--r--   0 jules     (1000) jules     (1000)       14 2021-12-22 19:45:35.000000 geoipsets-2.3.4/geoipsets/__init__.py
--rw-r--r--   0 jules     (1000) jules     (1000)     8066 2022-02-06 00:33:19.000000 geoipsets-2.3.4/geoipsets/__main__.py
--rw-r--r--   0 jules     (1000) jules     (1000)     8317 2022-05-03 02:14:02.000000 geoipsets-2.3.4/geoipsets/dbip.py
--rw-r--r--   0 jules     (1000) jules     (1000)     8531 2022-01-09 22:00:59.000000 geoipsets-2.3.4/geoipsets/maxmind.py
--rw-r--r--   0 jules     (1000) jules     (1000)      895 2022-01-04 02:03:31.000000 geoipsets-2.3.4/geoipsets/utils.py
-drwxr-xr-x   0 jules     (1000) jules     (1000)        0 2022-05-03 02:24:30.851465 geoipsets-2.3.4/geoipsets.egg-info/
--rw-r--r--   0 jules     (1000) jules     (1000)     3557 2022-05-03 02:24:30.000000 geoipsets-2.3.4/geoipsets.egg-info/PKG-INFO
--rw-r--r--   0 jules     (1000) jules     (1000)      350 2022-05-03 02:24:30.000000 geoipsets-2.3.4/geoipsets.egg-info/SOURCES.txt
--rw-r--r--   0 jules     (1000) jules     (1000)        1 2022-05-03 02:24:30.000000 geoipsets-2.3.4/geoipsets.egg-info/dependency_links.txt
--rw-r--r--   0 jules     (1000) jules     (1000)       55 2022-05-03 02:24:30.000000 geoipsets-2.3.4/geoipsets.egg-info/entry_points.txt
--rw-r--r--   0 jules     (1000) jules     (1000)       24 2022-05-03 02:24:30.000000 geoipsets-2.3.4/geoipsets.egg-info/requires.txt
--rw-r--r--   0 jules     (1000) jules     (1000)       10 2022-05-03 02:24:30.000000 geoipsets-2.3.4/geoipsets.egg-info/top_level.txt
--rw-r--r--   0 jules     (1000) jules     (1000)       38 2022-05-03 02:24:30.851465 geoipsets-2.3.4/setup.cfg
--rw-r--r--   0 jules     (1000) jules     (1000)     1228 2022-01-04 02:03:31.000000 geoipsets-2.3.4/setup.py
+drwxr-xr-x   0 jules     (1000) jules     (1000)        0 2023-04-16 20:52:26.508489 geoipsets-2.3.5/
+-rw-r--r--   0 jules     (1000) jules     (1000)       26 2021-12-22 19:45:35.000000 geoipsets-2.3.5/MANIFEST.in
+-rw-r--r--   0 jules     (1000) jules     (1000)     3588 2023-04-16 20:52:26.508489 geoipsets-2.3.5/PKG-INFO
+-rw-r--r--   0 jules     (1000) jules     (1000)     2973 2022-05-03 01:30:24.000000 geoipsets-2.3.5/README.md
+drwxr-xr-x   0 jules     (1000) jules     (1000)        0 2023-04-16 20:52:26.505156 geoipsets-2.3.5/geoipsets/
+-rw-r--r--   0 jules     (1000) jules     (1000)        5 2023-04-16 20:51:36.000000 geoipsets-2.3.5/geoipsets/VERSION
+-rw-r--r--   0 jules     (1000) jules     (1000)       14 2021-12-22 19:45:35.000000 geoipsets-2.3.5/geoipsets/__init__.py
+-rw-r--r--   0 jules     (1000) jules     (1000)     8066 2022-02-06 00:33:19.000000 geoipsets-2.3.5/geoipsets/__main__.py
+-rw-r--r--   0 jules     (1000) jules     (1000)     8317 2022-05-03 02:14:02.000000 geoipsets-2.3.5/geoipsets/dbip.py
+-rw-r--r--   0 jules     (1000) jules     (1000)     8531 2022-01-09 22:00:59.000000 geoipsets-2.3.5/geoipsets/maxmind.py
+-rw-r--r--   0 jules     (1000) jules     (1000)      895 2022-01-04 02:03:31.000000 geoipsets-2.3.5/geoipsets/utils.py
+drwxr-xr-x   0 jules     (1000) jules     (1000)        0 2023-04-16 20:52:26.508489 geoipsets-2.3.5/geoipsets.egg-info/
+-rw-r--r--   0 jules     (1000) jules     (1000)     3588 2023-04-16 20:52:26.000000 geoipsets-2.3.5/geoipsets.egg-info/PKG-INFO
+-rw-r--r--   0 jules     (1000) jules     (1000)      350 2023-04-16 20:52:26.000000 geoipsets-2.3.5/geoipsets.egg-info/SOURCES.txt
+-rw-r--r--   0 jules     (1000) jules     (1000)        1 2023-04-16 20:52:26.000000 geoipsets-2.3.5/geoipsets.egg-info/dependency_links.txt
+-rw-r--r--   0 jules     (1000) jules     (1000)       54 2023-04-16 20:52:26.000000 geoipsets-2.3.5/geoipsets.egg-info/entry_points.txt
+-rw-r--r--   0 jules     (1000) jules     (1000)       24 2023-04-16 20:52:26.000000 geoipsets-2.3.5/geoipsets.egg-info/requires.txt
+-rw-r--r--   0 jules     (1000) jules     (1000)       10 2023-04-16 20:52:26.000000 geoipsets-2.3.5/geoipsets.egg-info/top_level.txt
+-rw-r--r--   0 jules     (1000) jules     (1000)       38 2023-04-16 20:52:26.508489 geoipsets-2.3.5/setup.cfg
+-rw-r--r--   0 jules     (1000) jules     (1000)     1278 2023-04-16 20:51:36.000000 geoipsets-2.3.5/setup.py
```

### Comparing `geoipsets-2.3.4/PKG-INFO` & `geoipsets-2.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: geoipsets
-Version: 2.3.4
+Version: 2.3.5
 Summary: Utility to build country-specific IP sets for ipset/iptables and nftables.
 Home-page: https://github.com/chr0mag/geoipsets
 License: GPLv3
-Platform: UNKNOWN
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 ![badge](https://github.com/chr0mag/geoipsets/actions/workflows/python-tests.yaml/badge.svg) ![PyPI](https://img.shields.io/pypi/v/geoipsets) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/geoipsets) [![Downloads](https://pepy.tech/badge/geoipsets)](https://pepy.tech/project/geoipsets) ![GitHub](https://img.shields.io/github/license/chr0mag/geoipsets)
 
 Installation
 ------------
 
@@ -51,9 +51,7 @@
   -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                         directory where geoipsets should be saved (default: /tmp)
   -c CONFIG_FILE, --config-file CONFIG_FILE
                         path to configuration file (default: /etc/geoipsets.conf)
   --checksum            enable checksum validation of downloaded files (default)
   --no-checksum         disable checksum validation of downloaded files
 ```
-
-
```

### Comparing `geoipsets-2.3.4/README.md` & `geoipsets-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `geoipsets-2.3.4/geoipsets/__main__.py` & `geoipsets-2.3.5/geoipsets/__main__.py`

 * *Files identical despite different names*

### Comparing `geoipsets-2.3.4/geoipsets/dbip.py` & `geoipsets-2.3.5/geoipsets/dbip.py`

 * *Files identical despite different names*

### Comparing `geoipsets-2.3.4/geoipsets/maxmind.py` & `geoipsets-2.3.5/geoipsets/maxmind.py`

 * *Files identical despite different names*

### Comparing `geoipsets-2.3.4/geoipsets/utils.py` & `geoipsets-2.3.5/geoipsets/utils.py`

 * *Files identical despite different names*

### Comparing `geoipsets-2.3.4/geoipsets.egg-info/PKG-INFO` & `geoipsets-2.3.5/geoipsets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: geoipsets
-Version: 2.3.4
+Version: 2.3.5
 Summary: Utility to build country-specific IP sets for ipset/iptables and nftables.
 Home-page: https://github.com/chr0mag/geoipsets
 License: GPLv3
-Platform: UNKNOWN
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 ![badge](https://github.com/chr0mag/geoipsets/actions/workflows/python-tests.yaml/badge.svg) ![PyPI](https://img.shields.io/pypi/v/geoipsets) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/geoipsets) [![Downloads](https://pepy.tech/badge/geoipsets)](https://pepy.tech/project/geoipsets) ![GitHub](https://img.shields.io/github/license/chr0mag/geoipsets)
 
 Installation
 ------------
 
@@ -51,9 +51,7 @@
   -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                         directory where geoipsets should be saved (default: /tmp)
   -c CONFIG_FILE, --config-file CONFIG_FILE
                         path to configuration file (default: /etc/geoipsets.conf)
   --checksum            enable checksum validation of downloaded files (default)
   --no-checksum         disable checksum validation of downloaded files
 ```
-
-
```

### Comparing `geoipsets-2.3.4/setup.py` & `geoipsets-2.3.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     classifiers=[
         "Operating System :: POSIX :: Linux",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     packages=find_packages(exclude=("tests",)),
     include_package_data=True,
     install_requires=["requests", "beautifulsoup4"],
     entry_points={
         "console_scripts": [
             "geoipsets=geoipsets.__main__:main",
```

