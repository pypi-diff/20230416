# Comparing `tmp/rolv-0.0.2.tar.gz` & `tmp/rolv-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rolv-0.0.2.tar", last modified: Sun Apr 16 15:09:49 2023, max compression
+gzip compressed data, was "rolv-0.0.3.tar", last modified: Sun Apr 16 21:04:34 2023, max compression
```

## Comparing `rolv-0.0.2.tar` & `rolv-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,25 @@
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-16 15:09:49.296079 rolv-0.0.2/
--rw-r--r--   0 dorus     (1000) dorus     (1000)      312 2023-04-16 15:09:49.296079 rolv-0.0.2/PKG-INFO
--rw-r--r--   0 dorus     (1000) dorus     (1000)      227 2023-04-16 13:51:30.000000 rolv-0.0.2/README.md
--rw-r--r--   0 dorus     (1000) dorus     (1000)      438 2023-04-16 13:26:21.000000 rolv-0.0.2/pyproject.toml
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-16 15:09:49.292746 rolv-0.0.2/rolv/
--rw-r--r--   0 dorus     (1000) dorus     (1000)       97 2023-04-16 15:07:42.000000 rolv-0.0.2/rolv/__init__.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     2742 2023-04-16 15:06:20.000000 rolv-0.0.2/rolv/bashrc.py
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-16 15:09:49.296079 rolv-0.0.2/rolv/src/
--rwxr-xr-x   0 dorus     (1000) dorus     (1000)       35 2023-04-16 13:33:55.000000 rolv-0.0.2/rolv/src/build_local
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-16 15:09:49.296079 rolv-0.0.2/rolv.egg-info/
--rw-r--r--   0 dorus     (1000) dorus     (1000)      312 2023-04-16 15:09:49.000000 rolv-0.0.2/rolv.egg-info/PKG-INFO
--rw-r--r--   0 dorus     (1000) dorus     (1000)      230 2023-04-16 15:09:49.000000 rolv-0.0.2/rolv.egg-info/SOURCES.txt
--rw-r--r--   0 dorus     (1000) dorus     (1000)        1 2023-04-16 15:09:49.000000 rolv-0.0.2/rolv.egg-info/dependency_links.txt
--rw-r--r--   0 dorus     (1000) dorus     (1000)       66 2023-04-16 15:09:49.000000 rolv-0.0.2/rolv.egg-info/entry_points.txt
--rw-r--r--   0 dorus     (1000) dorus     (1000)        5 2023-04-16 15:09:49.000000 rolv-0.0.2/rolv.egg-info/top_level.txt
--rw-r--r--   0 dorus     (1000) dorus     (1000)      547 2023-04-16 15:09:49.296079 rolv-0.0.2/setup.cfg
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-16 21:04:34.663756 rolv-0.0.3/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      312 2023-04-16 21:04:34.663756 rolv-0.0.3/PKG-INFO
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      533 2023-04-16 17:44:08.000000 rolv-0.0.3/README.md
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      438 2023-04-16 13:26:21.000000 rolv-0.0.3/pyproject.toml
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-16 21:04:34.660423 rolv-0.0.3/rolv/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     2153 2023-04-16 21:04:02.000000 rolv-0.0.3/rolv/__init__.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      831 2023-04-16 20:17:20.000000 rolv-0.0.3/rolv/config.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1837 2023-04-16 20:16:15.000000 rolv-0.0.3/rolv/executables.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1511 2023-04-16 20:13:52.000000 rolv-0.0.3/rolv/lib.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      840 2023-04-16 20:40:22.000000 rolv-0.0.3/rolv/package.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     3950 2023-04-16 20:13:52.000000 rolv-0.0.3/rolv/rc.py
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-16 21:04:34.660423 rolv-0.0.3/rolv/src/
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-16 21:04:34.660423 rolv-0.0.3/rolv/src/config/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      371 2023-04-16 20:10:37.000000 rolv-0.0.3/rolv/src/config/default_aliases_and_functions
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-16 21:04:34.663756 rolv-0.0.3/rolv/src/executables/
+-rwxr-xr-x   0 dorus     (1000) dorus     (1000)       93 2023-04-16 15:53:31.000000 rolv-0.0.3/rolv/src/executables/gitc
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      633 2023-04-16 20:13:04.000000 rolv-0.0.3/rolv/src/executables/readme.md
+-rw-r--r--   0 dorus     (1000) dorus     (1000)        6 2023-04-16 20:19:07.000000 rolv-0.0.3/rolv/src/version
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-04-16 21:04:34.660423 rolv-0.0.3/rolv.egg-info/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      312 2023-04-16 21:04:34.000000 rolv-0.0.3/rolv.egg-info/PKG-INFO
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      388 2023-04-16 21:04:34.000000 rolv-0.0.3/rolv.egg-info/SOURCES.txt
+-rw-r--r--   0 dorus     (1000) dorus     (1000)        1 2023-04-16 21:04:34.000000 rolv-0.0.3/rolv.egg-info/dependency_links.txt
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      130 2023-04-16 21:04:34.000000 rolv-0.0.3/rolv.egg-info/entry_points.txt
+-rw-r--r--   0 dorus     (1000) dorus     (1000)        5 2023-04-16 21:04:34.000000 rolv-0.0.3/rolv.egg-info/top_level.txt
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      613 2023-04-16 21:04:34.663756 rolv-0.0.3/setup.cfg
```

### Comparing `rolv-0.0.2/setup.cfg` & `rolv-0.0.3/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rolv
-version = 0.0.2
+version = 0.0.3
 summary = Package to quickly set up linux terminal environment.
 home_page = https://github.com/dwrolvink/rolv
 author = https://github.com/dwrolvink
 author_email = dwrolvink@protonmail.com
 license = GNU General Public License v3 or later (GPLv3+)
 
 [options]
@@ -13,14 +13,16 @@
 python_requires = >=3.9
 
 [options.package_data]
 * = *.md, LICENSE, src/**
 
 [options.entry_points]
 console_scripts = 
-	rolv = rolv:version
+	rolv = rolv:help_text
+	rolv.version = rolv:version
 	rolv.install = rolv:install
+	rolv.disclaimer = rolv:disclaimer
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

