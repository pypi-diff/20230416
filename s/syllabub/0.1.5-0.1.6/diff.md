# Comparing `tmp/syllabub-0.1.5.tar.gz` & `tmp/syllabub-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syllabub-0.1.5.tar", last modified: Sat Apr 15 21:08:03 2023, max compression
+gzip compressed data, was "syllabub-0.1.6.tar", last modified: Sat Apr 15 22:37:02 2023, max compression
```

## Comparing `syllabub-0.1.5.tar` & `syllabub-0.1.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    34020 2023-04-15 20:57:16.685095 syllabub-0.1.5/COPYING
--rw-r--r--   0        0        0    34020 2022-09-20 10:56:30.499965 syllabub-0.1.5/LICENSES/AGPL-3.0-or-later.txt
--rw-r--r--   0        0        0    17023 2022-11-22 13:53:30.786895 syllabub-0.1.5/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0        0        0    21305 2022-11-22 13:53:30.786895 syllabub-0.1.5/LICENSES/CC-BY-SA-3.0.txt
--rw-r--r--   0        0        0    18375 2023-03-23 19:07:45.171020 syllabub-0.1.5/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0        0        0     7048 2022-09-20 10:56:30.835967 syllabub-0.1.5/LICENSES/CC0-1.0.txt
--rwxr-xr-x   0        0        0      119 2023-04-15 20:57:16.685095 syllabub-0.1.5/LICENSES/LicenseRef-DCO-1.1-license.txt
--rw-r--r--   0        0        0     3500 2023-04-15 21:07:50.942381 syllabub-0.1.5/README.md
--rw-r--r--   0        0        0      946 2023-04-15 21:08:03.222410 syllabub-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-03 20:16:16.766703 syllabub-0.1.5/src/syllabub/__init__.py
--rw-r--r--   0        0        0      145 2023-04-15 21:03:20.445784 syllabub-0.1.5/src/syllabub/builtin/.gitignore.mustache
--rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/.gitignore.mustache.license
--rw-r--r--   0        0        0     5488 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/CONDUCT.COVENANT
--rw-r--r--   0        0        0      136 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/CONDUCT.COVENANT.license
--rw-r--r--   0        0        0     8579 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/CONDUCT.UBUNTU
--rw-r--r--   0        0        0      134 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/CONDUCT.UBUNTU.license
--rwxr-xr-x   0        0        0     1421 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/CONTRIBUTING.DCO
--rwxr-xr-x   0        0        0      119 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/CONTRIBUTING.DCO.LICENSEREF
--rw-r--r--   0        0        0      143 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/CONTRIBUTING.DCO.LICENSEREF.license
--rw-r--r--   0        0        0      143 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/CONTRIBUTING.DCO.license
--rwxr-xr-x   0        0        0      119 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/LicenseRef-DCO-1.1-license.txt
--rwxr-xr-x   0        0        0      143 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/LicenseRef-DCO-1.1-license.txt.license
--rw-r--r--   0        0        0     1000 2023-03-29 12:10:26.916921 syllabub-0.1.5/src/syllabub/builtin/Makefile.mustache
--rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/Makefile.mustache.license
--rw-r--r--   0        0        0     1374 2023-04-15 21:03:20.445784 syllabub-0.1.5/src/syllabub/builtin/README.md.mustache
--rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/README.md.mustache.license
--rw-r--r--   0        0        0        0 2023-04-03 16:49:55.680967 syllabub-0.1.5/src/syllabub/builtin/__init__.py
--rw-r--r--   0        0        0      174 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/cli.py.mustache
--rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/cli.py.mustache.license
--rw-r--r--   0        0        0    10442 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/logo.png
--rw-r--r--   0        0        0      193 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/logo.png.license
--rw-r--r--   0        0        0       87 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/pdm.lock.license.mustache
--rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/pdm.lock.license.mustache.license
--rw-r--r--   0        0        0      810 2023-04-15 21:03:20.445784 syllabub-0.1.5/src/syllabub/builtin/pyproject.toml.mustache
--rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/pyproject.toml.mustache.license
--rw-r--r--   0        0        0      197 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/test_cli.py.mustache
--rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.1.5/src/syllabub/builtin/test_cli.py.mustache.license
--rw-r--r--   0        0        0     2686 2023-04-15 21:03:20.445784 syllabub-0.1.5/src/syllabub/cli.py
--rw-r--r--   0        0        0     5180 2023-04-15 21:03:20.445784 syllabub-0.1.5/src/syllabub/metadata.py
--rw-r--r--   0        0        0      232 2023-03-23 19:07:45.179020 syllabub-0.1.5/tests/test_cli.py
--rw-r--r--   0        0        0     3955 1970-01-01 00:00:00.000000 syllabub-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    34020 2023-04-15 20:57:16.685095 syllabub-0.1.6/COPYING
+-rw-r--r--   0        0        0    34020 2022-09-20 10:56:30.499965 syllabub-0.1.6/LICENSES/AGPL-3.0-or-later.txt
+-rw-r--r--   0        0        0    17023 2022-11-22 13:53:30.786895 syllabub-0.1.6/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0        0        0    21305 2022-11-22 13:53:30.786895 syllabub-0.1.6/LICENSES/CC-BY-SA-3.0.txt
+-rw-r--r--   0        0        0    18375 2023-03-23 19:07:45.171020 syllabub-0.1.6/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0        0        0     7048 2022-09-20 10:56:30.835967 syllabub-0.1.6/LICENSES/CC0-1.0.txt
+-rwxr-xr-x   0        0        0      119 2023-04-15 20:57:16.685095 syllabub-0.1.6/LICENSES/LicenseRef-DCO-1.1-license.txt
+-rw-r--r--   0        0        0     3500 2023-04-15 22:36:54.236411 syllabub-0.1.6/README.md
+-rw-r--r--   0        0        0      956 2023-04-15 22:37:02.836436 syllabub-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-03 20:16:16.766703 syllabub-0.1.6/src/syllabub/__init__.py
+-rw-r--r--   0        0        0      145 2023-04-15 21:03:20.445784 syllabub-0.1.6/src/syllabub/builtin/.gitignore.mustache
+-rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.1.6/src/syllabub/builtin/.gitignore.mustache.license
+-rw-r--r--   0        0        0     5488 2023-03-23 19:07:45.179020 syllabub-0.1.6/src/syllabub/builtin/CONDUCT.COVENANT
+-rw-r--r--   0        0        0      136 2023-03-23 19:07:45.179020 syllabub-0.1.6/src/syllabub/builtin/CONDUCT.COVENANT.license
+-rw-r--r--   0        0        0     8579 2023-03-23 19:07:45.179020 syllabub-0.1.6/src/syllabub/builtin/CONDUCT.UBUNTU
+-rw-r--r--   0        0        0      134 2023-03-23 19:07:45.179020 syllabub-0.1.6/src/syllabub/builtin/CONDUCT.UBUNTU.license
+-rwxr-xr-x   0        0        0     1421 2023-03-23 19:07:45.179020 syllabub-0.1.6/src/syllabub/builtin/CONTRIBUTING.DCO
+-rwxr-xr-x   0        0        0      119 2023-03-23 19:07:45.179020 syllabub-0.1.6/src/syllabub/builtin/CONTRIBUTING.DCO.LICENSEREF
+-rw-r--r--   0        0        0      143 2023-03-23 19:07:45.179020 syllabub-0.1.6/src/syllabub/builtin/CONTRIBUTING.DCO.LICENSEREF.license
+-rw-r--r--   0        0        0      143 2023-03-23 19:07:45.179020 syllabub-0.1.6/src/syllabub/builtin/CONTRIBUTING.DCO.license
+-rwxr-xr-x   0        0        0      119 2023-03-23 19:07:45.179020 syllabub-0.1.6/src/syllabub/builtin/LicenseRef-DCO-1.1-license.txt
+-rwxr-xr-x   0        0        0      143 2023-03-23 19:07:45.179020 syllabub-0.1.6/src/syllabub/builtin/LicenseRef-DCO-1.1-license.txt.license
+-rw-r--r--   0        0        0     1000 2023-03-29 12:10:26.916921 syllabub-0.1.6/src/syllabub/builtin/Makefile.mustache
+-rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.1.6/src/syllabub/builtin/Makefile.mustache.license
+-rw-r--r--   0        0        0     1374 2023-04-15 21:03:20.445784 syllabub-0.1.6/src/syllabub/builtin/README.md.mustache
+-rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.1.6/src/syllabub/builtin/README.md.mustache.license
+-rw-r--r--   0        0        0        0 2023-04-03 16:49:55.680967 syllabub-0.1.6/src/syllabub/builtin/__init__.py
+-rw-r--r--   0        0        0      174 2023-03-23 19:07:45.179020 syllabub-0.1.6/src/syllabub/builtin/cli.py.mustache
+-rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.1.6/src/syllabub/builtin/cli.py.mustache.license
+-rw-r--r--   0        0        0    10442 2023-03-23 19:07:45.179020 syllabub-0.1.6/src/syllabub/builtin/logo.png
+-rw-r--r--   0        0        0      193 2023-03-23 19:07:45.179020 syllabub-0.1.6/src/syllabub/builtin/logo.png.license
+-rw-r--r--   0        0        0       87 2023-03-23 19:07:45.179020 syllabub-0.1.6/src/syllabub/builtin/pdm.lock.license.mustache
+-rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.1.6/src/syllabub/builtin/pdm.lock.license.mustache.license
+-rw-r--r--   0        0        0      810 2023-04-15 21:03:20.445784 syllabub-0.1.6/src/syllabub/builtin/pyproject.toml.mustache
+-rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.1.6/src/syllabub/builtin/pyproject.toml.mustache.license
+-rw-r--r--   0        0        0      197 2023-03-23 19:07:45.179020 syllabub-0.1.6/src/syllabub/builtin/test_cli.py.mustache
+-rw-r--r--   0        0        0      107 2023-03-23 19:07:45.179020 syllabub-0.1.6/src/syllabub/builtin/test_cli.py.mustache.license
+-rw-r--r--   0        0        0     2686 2023-04-15 21:03:20.445784 syllabub-0.1.6/src/syllabub/cli.py
+-rw-r--r--   0        0        0     5180 2023-04-15 21:03:20.445784 syllabub-0.1.6/src/syllabub/metadata.py
+-rw-r--r--   0        0        0      232 2023-03-23 19:07:45.179020 syllabub-0.1.6/tests/test_cli.py
+-rw-r--r--   0        0        0     3965 1970-01-01 00:00:00.000000 syllabub-0.1.6/PKG-INFO
```

### Comparing `syllabub-0.1.5/COPYING` & `syllabub-0.1.6/COPYING`

 * *Files identical despite different names*

### Comparing `syllabub-0.1.5/LICENSES/AGPL-3.0-or-later.txt` & `syllabub-0.1.6/LICENSES/AGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `syllabub-0.1.5/LICENSES/CC-BY-4.0.txt` & `syllabub-0.1.6/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `syllabub-0.1.5/LICENSES/CC-BY-SA-3.0.txt` & `syllabub-0.1.6/LICENSES/CC-BY-SA-3.0.txt`

 * *Files identical despite different names*

### Comparing `syllabub-0.1.5/LICENSES/CC-BY-SA-4.0.txt` & `syllabub-0.1.6/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `syllabub-0.1.5/LICENSES/CC0-1.0.txt` & `syllabub-0.1.6/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `syllabub-0.1.5/README.md` & `syllabub-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `syllabub-0.1.5/pyproject.toml` & `syllabub-0.1.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 dependencies = [
     "chevron>=0.14.0",
     "tomli>=2.0.1",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 dynamic = []
-version = "0.1.5"
+version = "0.1.6"
 
 [project.license]
 text = "AGPL-3.0-or-later"
 
 [project.optional-dependencies]
 
 [project.scripts]
 syllabub = "syllabub.cli:invoke"
 
 [project.urls]
-Source = "https://gitlab.com/lfdo/syllabub"
+Source = "https://gitlab.com/lfdo/toolchain/syllabub"
 Project = "https://lofidevops.neocities.org"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `syllabub-0.1.5/src/syllabub/builtin/CONDUCT.COVENANT` & `syllabub-0.1.6/src/syllabub/builtin/CONDUCT.COVENANT`

 * *Files identical despite different names*

### Comparing `syllabub-0.1.5/src/syllabub/builtin/CONDUCT.UBUNTU` & `syllabub-0.1.6/src/syllabub/builtin/CONDUCT.UBUNTU`

 * *Files identical despite different names*

### Comparing `syllabub-0.1.5/src/syllabub/builtin/CONTRIBUTING.DCO` & `syllabub-0.1.6/src/syllabub/builtin/CONTRIBUTING.DCO`

 * *Files identical despite different names*

### Comparing `syllabub-0.1.5/src/syllabub/builtin/Makefile.mustache` & `syllabub-0.1.6/src/syllabub/builtin/Makefile.mustache`

 * *Files identical despite different names*

### Comparing `syllabub-0.1.5/src/syllabub/builtin/README.md.mustache` & `syllabub-0.1.6/src/syllabub/builtin/README.md.mustache`

 * *Files identical despite different names*

### Comparing `syllabub-0.1.5/src/syllabub/builtin/logo.png` & `syllabub-0.1.6/src/syllabub/builtin/logo.png`

 * *Files identical despite different names*

### Comparing `syllabub-0.1.5/src/syllabub/builtin/pyproject.toml.mustache` & `syllabub-0.1.6/src/syllabub/builtin/pyproject.toml.mustache`

 * *Files identical despite different names*

### Comparing `syllabub-0.1.5/src/syllabub/cli.py` & `syllabub-0.1.6/src/syllabub/cli.py`

 * *Files identical despite different names*

### Comparing `syllabub-0.1.5/src/syllabub/metadata.py` & `syllabub-0.1.6/src/syllabub/metadata.py`

 * *Files identical despite different names*

### Comparing `syllabub-0.1.5/PKG-INFO` & `syllabub-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: syllabub
-Version: 0.1.5
+Version: 0.1.6
 Summary: Keep Python project conventions up-to-date and worry less about trifling matters. 🍰
 Author-Email: David Seaward <david@librem.one>
 License: AGPL-3.0-or-later
-Project-URL: Source, https://gitlab.com/lfdo/syllabub
+Project-URL: Source, https://gitlab.com/lfdo/toolchain/syllabub
 Project-URL: Project, https://lofidevops.neocities.org
 Requires-Python: >=3.10
 Requires-Dist: chevron>=0.14.0
 Requires-Dist: tomli>=2.0.1
 Description-Content-Type: text/markdown
 
 # Syllabub project bolt-on
```

