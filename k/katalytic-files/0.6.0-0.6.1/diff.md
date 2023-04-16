# Comparing `tmp/katalytic-files-0.6.0.tar.gz` & `tmp/katalytic-files-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-files-0.6.0.tar", last modified: Sat Apr 15 06:36:58 2023, max compression
+gzip compressed data, was "katalytic-files-0.6.1.tar", last modified: Sun Apr 16 11:20:02 2023, max compression
```

## Comparing `katalytic-files-0.6.0.tar` & `katalytic-files-0.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       87 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/.coveragerc
--rw-r--r--   0        0        0      641 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/.gitignore
--rw-r--r--   0        0        0      841 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      542 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/.travis.yml
--rw-r--r--   0        0        0     1235 2023-04-15 06:36:54.312829 katalytic-files-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     2031 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/README.md
--rw-r--r--   0        0        0     1608 2023-04-15 06:36:53.869051 katalytic-files-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      228 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/scripts/cleanup.sh
--rw-r--r--   0        0        0     1262 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/scripts/conda.sh
--rw-r--r--   0        0        0      792 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/scripts/find_requirements.py
--rw-r--r--   0        0        0      114 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/scripts/pytest.sh
--rw-r--r--   0        0        0     3107 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/scripts/release.sh
--rw-r--r--   0        0        0      470 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/scripts/setup.sh
--rw-r--r--   0        0        0      144 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/scripts/should_skip_release.sh
--rw-r--r--   0        0        0      239 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/scripts/should_skip_travis_build.sh
--rw-r--r--   0        0        0     1699 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/scripts/venv.sh
--rw-r--r--   0        0        0    12492 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/src/katalytic/files.py
--rw-r--r--   0        0        0    42174 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/tests/test_files.py
--rw-r--r--   0        0        0     3172 1970-01-01 00:00:00.000000 katalytic-files-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/.coveragerc
+-rw-r--r--   0        0        0      641 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/.gitignore
+-rw-r--r--   0        0        0      841 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0      542 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/.travis.yml
+-rw-r--r--   0        0        0     1040 2023-04-16 11:19:58.263116 katalytic-files-0.6.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/LICENSE.txt
+-rw-r--r--   0        0        0     2031 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/README.md
+-rw-r--r--   0        0        0     1608 2023-04-16 11:19:57.838904 katalytic-files-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      228 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/scripts/cleanup.sh
+-rw-r--r--   0        0        0     1262 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/scripts/conda.sh
+-rw-r--r--   0        0        0      792 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/scripts/find_requirements.py
+-rw-r--r--   0        0        0      114 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/scripts/pytest.sh
+-rw-r--r--   0        0        0     3107 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/scripts/release.sh
+-rw-r--r--   0        0        0      470 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/scripts/setup.sh
+-rw-r--r--   0        0        0      144 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/scripts/should_skip_release.sh
+-rw-r--r--   0        0        0      239 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/scripts/should_skip_travis_build.sh
+-rw-r--r--   0        0        0     1699 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/scripts/venv.sh
+-rw-r--r--   0        0        0    12492 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/src/katalytic/files.py
+-rw-r--r--   0        0        0    42174 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/tests/test_files.py
+-rw-r--r--   0        0        0     3172 1970-01-01 00:00:00.000000 katalytic-files-0.6.1/PKG-INFO
```

### Comparing `katalytic-files-0.6.0/.gitignore` & `katalytic-files-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.6.0/.gitlab-ci.yml` & `katalytic-files-0.6.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.6.0/.travis.yml` & `katalytic-files-0.6.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.6.0/CHANGELOG.md` & `katalytic-files-0.6.1/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,20 @@
+## 0.6.1 (2023-04-16)
+### Fix
+* Test the new token ([`f2838d7`](https://github.com/katalytic/katalytic-files/commit/f2838d7ca49a27e8bbf718fab5d55b64868cf734))
+* Test the new token ([`43d505a`](https://github.com/katalytic/katalytic-files/commit/43d505aab96beaa6807188d72aece63de7d9f812))
+
+
 ## 0.6.0 (2023-04-15)
 ### Feature
 * Add load_text() and save_text() ([`2283da7`](https://github.com/katalytic/katalytic-files/commit/2283da70eddcc90f3ff90f14f9c611ffb310adf6))
 * Add load_text() and save_text() ([`4eb85d6`](https://github.com/katalytic/katalytic-files/commit/4eb85d66245efad828f14b0ccd48858a473e9394))
 
 
 ## 0.5.0 (2023-04-15)
 ### Feature
 * **load_json:** Remove sort_keys parameter. I will add a function for that later, probably in katalytic-data ([`8e188c0`](https://github.com/katalytic/katalytic-files/commit/8e188c08fc22497090f8ca07d8aaa47aa1856dd4))
 
 
 ## 0.4.0 (2023-04-15)
 ### Feature
 * Add load_json() and save_json() ([`a4fed13`](https://github.com/katalytic/katalytic-files/commit/a4fed135abe77732c337b33ec65b0ffa69f8536d))
-
-
-## 0.3.28 (2023-04-14)
-### Fix
-* Release ([`7043dfa`](https://github.com/katalytic/katalytic-files/commit/7043dfa14dce58436232d997624b03d07efb8a7a))
-
-
-## 0.3.27 (2023-04-13)
-### Fix
-* Uncomment "flit build" ([`a58c44f`](https://github.com/katalytic/katalytic-files/commit/a58c44fcb419e698c778db5661e6c594397d3f0e))
-
-
-## 0.3.26 (2023-04-13)
-### Fix
-* Skipping shell scripts ([`a021fff`](https://github.com/katalytic/katalytic-files/commit/a021ffffd87a06e3e0f59b32bbff0e05101e46f7))
-
-
```

### Comparing `katalytic-files-0.6.0/LICENSE.txt` & `katalytic-files-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.6.0/README.md` & `katalytic-files-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.6.0/pyproject.toml` & `katalytic-files-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-files"
-version = "0.6.0"
+version = "0.6.1"
 description = "This plugin adds utilities for working with files to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic-files-0.6.0/scripts/conda.sh` & `katalytic-files-0.6.1/scripts/conda.sh`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.6.0/scripts/find_requirements.py` & `katalytic-files-0.6.1/scripts/find_requirements.py`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.6.0/scripts/release.sh` & `katalytic-files-0.6.1/scripts/release.sh`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.6.0/scripts/venv.sh` & `katalytic-files-0.6.1/scripts/venv.sh`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.6.0/src/katalytic/files.py` & `katalytic-files-0.6.1/src/katalytic/files.py`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.6.0/tests/test_files.py` & `katalytic-files-0.6.1/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.6.0/PKG-INFO` & `katalytic-files-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-files
-Version: 0.6.0
+Version: 0.6.1
 Summary: This plugin adds utilities for working with files to the katalytic namespace
 Keywords: automation,filesystem
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

