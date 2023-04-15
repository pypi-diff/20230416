# Comparing `tmp/checkyoself-0.0.3.tar.gz` & `tmp/checkyoself-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkyoself-0.0.3.tar", last modified: Mon Mar 27 22:02:33 2023, max compression
+gzip compressed data, was "checkyoself-0.1.4.tar", last modified: Sat Apr 15 22:17:47 2023, max compression
```

## Comparing `checkyoself-0.0.3.tar` & `checkyoself-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0    34020 2023-03-27 21:54:37.804506 checkyoself-0.0.3/LICENSES/AGPL-3.0-or-later.txt
--rwxr-xr-x   0        0        0    16814 2020-10-15 16:18:28.682002 checkyoself-0.0.3/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0        0        0    18375 2023-03-27 21:54:37.804506 checkyoself-0.0.3/LICENSES/CC-BY-SA-4.0.txt
--rwxr-xr-x   0        0        0     6916 2020-10-15 16:18:28.682002 checkyoself-0.0.3/LICENSES/CC0-1.0.txt
--rwxr-xr-x   0        0        0      119 2023-03-27 12:56:54.771725 checkyoself-0.0.3/LICENSES/LicenseRef-DCO-1.1-license.txt
--rw-r--r--   0        0        0     3390 2023-03-27 22:00:56.793090 checkyoself-0.0.3/README.md
--rw-r--r--   0        0        0      866 2023-03-27 22:02:33.001312 checkyoself-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-27 21:54:37.808506 checkyoself-0.0.3/src/checkyoself/__init__.py
--rw-r--r--   0        0        0     4331 2023-03-27 21:54:37.808506 checkyoself-0.0.3/src/checkyoself/chikkity.py
--rw-r--r--   0        0        0        0 2023-03-27 21:54:37.808506 checkyoself-0.0.3/src/checkyoself/kb/__init__.py
--rw-r--r--   0        0        0      252 2023-03-27 21:54:37.812506 checkyoself-0.0.3/src/checkyoself/kb/apt.yml
--rw-r--r--   0        0        0      107 2023-03-27 21:54:37.812506 checkyoself-0.0.3/src/checkyoself/kb/apt.yml.license
--rw-r--r--   0        0        0       68 2023-03-27 21:54:37.812506 checkyoself-0.0.3/src/checkyoself/kb/bin.yml
--rw-r--r--   0        0        0      107 2023-03-27 21:54:37.812506 checkyoself-0.0.3/src/checkyoself/kb/bin.yml.license
--rw-r--r--   0        0        0        0 2023-03-27 21:54:37.812506 checkyoself-0.0.3/src/checkyoself/kb/path.yml
--rw-r--r--   0        0        0      107 2023-03-27 21:54:37.812506 checkyoself-0.0.3/src/checkyoself/kb/path.yml.license
--rw-r--r--   0        0        0     3736 1970-01-01 00:00:00.000000 checkyoself-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    34020 2023-04-15 22:15:06.800763 checkyoself-0.1.4/COPYING
+-rw-r--r--   0        0        0    34020 2023-03-27 21:54:37.804506 checkyoself-0.1.4/LICENSES/AGPL-3.0-or-later.txt
+-rwxr-xr-x   0        0        0    16814 2020-10-15 16:18:28.682002 checkyoself-0.1.4/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0        0        0    18375 2023-03-27 21:54:37.804506 checkyoself-0.1.4/LICENSES/CC-BY-SA-4.0.txt
+-rwxr-xr-x   0        0        0     6916 2020-10-15 16:18:28.682002 checkyoself-0.1.4/LICENSES/CC0-1.0.txt
+-rwxr-xr-x   0        0        0      119 2023-04-15 21:58:07.541934 checkyoself-0.1.4/LICENSES/LicenseRef-DCO-1.1-license.txt
+-rw-r--r--   0        0        0     3595 2023-04-15 22:17:40.357234 checkyoself-0.1.4/README.md
+-rw-r--r--   0        0        0      961 2023-04-15 22:17:47.249255 checkyoself-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-27 21:54:37.808506 checkyoself-0.1.4/src/checkyoself/__init__.py
+-rw-r--r--   0        0        0     4331 2023-03-27 21:54:37.808506 checkyoself-0.1.4/src/checkyoself/chikkity.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:54:37.808506 checkyoself-0.1.4/src/checkyoself/kb/__init__.py
+-rw-r--r--   0        0        0      252 2023-03-27 21:54:37.812506 checkyoself-0.1.4/src/checkyoself/kb/apt.yml
+-rw-r--r--   0        0        0      107 2023-03-27 21:54:37.812506 checkyoself-0.1.4/src/checkyoself/kb/apt.yml.license
+-rw-r--r--   0        0        0       68 2023-03-27 21:54:37.812506 checkyoself-0.1.4/src/checkyoself/kb/bin.yml
+-rw-r--r--   0        0        0      107 2023-03-27 21:54:37.812506 checkyoself-0.1.4/src/checkyoself/kb/bin.yml.license
+-rw-r--r--   0        0        0        0 2023-03-27 21:54:37.812506 checkyoself-0.1.4/src/checkyoself/kb/path.yml
+-rw-r--r--   0        0        0      107 2023-03-27 21:54:37.812506 checkyoself-0.1.4/src/checkyoself/kb/path.yml.license
+-rw-r--r--   0        0        0      228 2023-04-15 22:15:06.800763 checkyoself-0.1.4/tests/test_cli.py
+-rw-r--r--   0        0        0     4053 1970-01-01 00:00:00.000000 checkyoself-0.1.4/PKG-INFO
```

### Comparing `checkyoself-0.0.3/LICENSES/AGPL-3.0-or-later.txt` & `checkyoself-0.1.4/COPYING`

 * *Files identical despite different names*

### Comparing `checkyoself-0.0.3/LICENSES/CC-BY-4.0.txt` & `checkyoself-0.1.4/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `checkyoself-0.0.3/LICENSES/CC-BY-SA-4.0.txt` & `checkyoself-0.1.4/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `checkyoself-0.0.3/LICENSES/CC0-1.0.txt` & `checkyoself-0.1.4/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `checkyoself-0.0.3/README.md` & `checkyoself-0.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -125,7 +125,11 @@
 Copyright 2020 David Seaward and contributors
 SPDX-License-Identifier: AGPL-3.0-or-later
 ```
 
 Shared under AGPL-3.0-or-later. We adhere to the Contributor Covenant 2.1, and
 certify origin per DCO 1.1 with a signed-off-by line. Contributions under the
 same terms are welcome.
+
+Submit security and conduct issues as private tickets. Sign commits with
+`git commit --signoff`. For a software bill of materials run `reuse spdx`. For
+more details see CONDUCT, COPYING and CONTRIBUTING.
```

### Comparing `checkyoself-0.0.3/pyproject.toml` & `checkyoself-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 [project]
 name = "checkyoself"
-version = "0.0.3"
 description = "Which online repositories does my system rely on?"
 authors = [
     { name = "David Seaward", email = "david@librem.one" },
 ]
 dependencies = [
     "click>=8.1.3",
     "parse>=1.19.0",
     "ruamel-yaml>=0.17.21",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
+dynamic = []
+version = "0.1.4"
 
 [project.license]
 text = "AGPL-3.0-or-later"
 
 [project.optional-dependencies]
 
 [project.scripts]
 checkyoself = "checkyoself.chikkity:check"
 
+[project.urls]
+Source = "https://gitlab.com/lfdo/checkyoself"
+Project = "https://lofidevops.neocities.org"
+
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "carmine>=0.0.3",
 ]
 
+[tool.pdm.version]
+source = "scm"
+
 [tool.syllabub.project]
 conduct = "contributor-covenant-2.1"
 copyright = "Copyright 2020 David Seaward and contributors"
 origin = "DCO-1.1-git-signoff"
-sbom = "reuse spdx"
 title = "Check yo' self (dibbity deb remix)"
-url = "https://lofidevops.neocities.org"
```

### Comparing `checkyoself-0.0.3/src/checkyoself/chikkity.py` & `checkyoself-0.1.4/src/checkyoself/chikkity.py`

 * *Files identical despite different names*

### Comparing `checkyoself-0.0.3/PKG-INFO` & `checkyoself-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: checkyoself
-Version: 0.0.3
+Version: 0.1.4
 Summary: Which online repositories does my system rely on?
 Author-Email: David Seaward <david@librem.one>
 License: AGPL-3.0-or-later
+Project-URL: Source, https://gitlab.com/lfdo/checkyoself
+Project-URL: Project, https://lofidevops.neocities.org
 Requires-Python: >=3.10
 Requires-Dist: click>=8.1.3
 Requires-Dist: parse>=1.19.0
 Requires-Dist: ruamel-yaml>=0.17.21
 Description-Content-Type: text/markdown
 
 # Check yo' self (dibbity deb remix)
@@ -137,7 +139,11 @@
 Copyright 2020 David Seaward and contributors
 SPDX-License-Identifier: AGPL-3.0-or-later
 ```
 
 Shared under AGPL-3.0-or-later. We adhere to the Contributor Covenant 2.1, and
 certify origin per DCO 1.1 with a signed-off-by line. Contributions under the
 same terms are welcome.
+
+Submit security and conduct issues as private tickets. Sign commits with
+`git commit --signoff`. For a software bill of materials run `reuse spdx`. For
+more details see CONDUCT, COPYING and CONTRIBUTING.
```

