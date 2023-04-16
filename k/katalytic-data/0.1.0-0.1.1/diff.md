# Comparing `tmp/katalytic-data-0.1.0.tar.gz` & `tmp/katalytic-data-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-data-0.1.0.tar", last modified: Sun Apr 16 10:46:57 2023, max compression
+gzip compressed data, was "katalytic-data-0.1.1.tar", last modified: Sun Apr 16 11:10:06 2023, max compression
```

## Comparing `katalytic-data-0.1.0.tar` & `katalytic-data-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       87 2023-04-16 10:46:14.695647 katalytic-data-0.1.0/.coveragerc
--rw-r--r--   0        0        0      641 2023-04-16 10:46:14.695647 katalytic-data-0.1.0/.gitignore
--rw-r--r--   0        0        0      841 2023-04-16 10:46:14.695647 katalytic-data-0.1.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      542 2023-04-16 10:46:14.695647 katalytic-data-0.1.0/.travis.yml
--rw-r--r--   0        0        0      821 2023-04-16 10:46:52.892540 katalytic-data-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-16 10:46:14.695647 katalytic-data-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2083 2023-04-16 10:46:14.695647 katalytic-data-0.1.0/README.md
--rw-r--r--   0        0        0     1516 2023-04-16 10:46:52.448762 katalytic-data-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      228 2023-04-16 10:46:14.695647 katalytic-data-0.1.0/scripts/cleanup.sh
--rw-r--r--   0        0        0     1262 2023-04-16 10:46:14.695647 katalytic-data-0.1.0/scripts/conda.sh
--rw-r--r--   0        0        0      792 2023-04-16 10:46:14.695647 katalytic-data-0.1.0/scripts/find_requirements.py
--rw-r--r--   0        0        0      114 2023-04-16 10:46:14.695647 katalytic-data-0.1.0/scripts/pytest.sh
--rw-r--r--   0        0        0     3107 2023-04-16 10:46:14.695647 katalytic-data-0.1.0/scripts/release.sh
--rw-r--r--   0        0        0      470 2023-04-16 10:46:14.695647 katalytic-data-0.1.0/scripts/setup.sh
--rw-r--r--   0        0        0      144 2023-04-16 10:46:14.695647 katalytic-data-0.1.0/scripts/should_skip_release.sh
--rw-r--r--   0        0        0      239 2023-04-16 10:46:14.695647 katalytic-data-0.1.0/scripts/should_skip_travis_build.sh
--rw-r--r--   0        0        0     1699 2023-04-16 10:46:14.695647 katalytic-data-0.1.0/scripts/venv.sh
--rw-r--r--   0        0        0      381 2023-04-16 10:46:14.695647 katalytic-data-0.1.0/src/katalytic/checks.py
--rw-r--r--   0        0        0     2455 2023-04-16 10:46:14.695647 katalytic-data-0.1.0/src/katalytic/data.py
--rw-r--r--   0        0        0      772 2023-04-16 10:46:14.695647 katalytic-data-0.1.0/tests/test_checks.py
--rw-r--r--   0        0        0     5465 2023-04-16 10:46:14.695647 katalytic-data-0.1.0/tests/test_data.py
--rw-r--r--   0        0        0     3128 1970-01-01 00:00:00.000000 katalytic-data-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/.coveragerc
+-rw-r--r--   0        0        0      641 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/.gitignore
+-rw-r--r--   0        0        0      841 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0      542 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/.travis.yml
+-rw-r--r--   0        0        0     1235 2023-04-16 11:10:02.179073 katalytic-data-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     2083 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/README.md
+-rw-r--r--   0        0        0     1516 2023-04-16 11:10:01.738853 katalytic-data-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      228 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/scripts/cleanup.sh
+-rw-r--r--   0        0        0     1262 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/scripts/conda.sh
+-rw-r--r--   0        0        0      792 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/scripts/find_requirements.py
+-rw-r--r--   0        0        0      114 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/scripts/pytest.sh
+-rw-r--r--   0        0        0     3107 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/scripts/release.sh
+-rw-r--r--   0        0        0      470 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/scripts/setup.sh
+-rw-r--r--   0        0        0      144 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/scripts/should_skip_release.sh
+-rw-r--r--   0        0        0      239 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/scripts/should_skip_travis_build.sh
+-rw-r--r--   0        0        0     1699 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/scripts/venv.sh
+-rw-r--r--   0        0        0      381 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/src/katalytic/checks.py
+-rw-r--r--   0        0        0     2455 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/src/katalytic/data.py
+-rw-r--r--   0        0        0      772 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/tests/test_checks.py
+-rw-r--r--   0        0        0     5465 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/tests/test_data.py
+-rw-r--r--   0        0        0     3128 1970-01-01 00:00:00.000000 katalytic-data-0.1.1/PKG-INFO
```

### Comparing `katalytic-data-0.1.0/.gitignore` & `katalytic-data-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.1.0/.gitlab-ci.yml` & `katalytic-data-0.1.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.1.0/.travis.yml` & `katalytic-data-0.1.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.1.0/CHANGELOG.md` & `katalytic-data-0.1.1/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,15 @@
+## 0.1.1 (2023-04-16)
+### Fix
+* Test the new token ([`7b08c42`](https://github.com/katalytic/katalytic-data/commit/7b08c428164a5c37c205b10687ce274622579a70))
+* Test the new token ([`4680b23`](https://github.com/katalytic/katalytic-data/commit/4680b2379099e206fef1ee4aef176547ef0c9f64))
+* Test the new token ([`9b71e3e`](https://github.com/katalytic/katalytic-data/commit/9b71e3e81fe35735673620732b1f54fc86f7e3d4))
+
+
 ## 0.1.0 (2023-04-16)
 ### Feature
 * Add is_collection() ([`bf29261`](https://github.com/katalytic/katalytic-data/commit/bf2926172f56d000d1f09318ab212c7b9747a8b0))
 * Add is_primitive() ([`ed950cc`](https://github.com/katalytic/katalytic-data/commit/ed950ccdd8e4cd4d4439cb0ab9c763d55135461d))
 * Add sort_dict_by_values() ([`6b3c985`](https://github.com/katalytic/katalytic-data/commit/6b3c9856c69e088467087345743a38e6294def7a))
 * Add sort_dict_by_keys() ([`5c05e48`](https://github.com/katalytic/katalytic-data/commit/5c05e48c4cc8afaf6a861103784690ebc153dcc8))
 * Add map_dict_values() ([`ba289c5`](https://github.com/katalytic/katalytic-data/commit/ba289c5f5cb21ff66d89bb833f30e2be678e15da))
 * Add map_dict_keys() ([`f6b1410`](https://github.com/katalytic/katalytic-data/commit/f6b141050b901456041bf049dc3b329c2d8fcec8))
-
-
```

### Comparing `katalytic-data-0.1.0/LICENSE.txt` & `katalytic-data-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.1.0/README.md` & `katalytic-data-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.1.0/pyproject.toml` & `katalytic-data-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-data"
-version = "0.1.0"
+version = "0.1.1"
 description = "This plugin adds utilities for working with data to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic-data-0.1.0/scripts/conda.sh` & `katalytic-data-0.1.1/scripts/conda.sh`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.1.0/scripts/find_requirements.py` & `katalytic-data-0.1.1/scripts/find_requirements.py`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.1.0/scripts/release.sh` & `katalytic-data-0.1.1/scripts/release.sh`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.1.0/scripts/venv.sh` & `katalytic-data-0.1.1/scripts/venv.sh`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.1.0/src/katalytic/data.py` & `katalytic-data-0.1.1/src/katalytic/data.py`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.1.0/tests/test_checks.py` & `katalytic-data-0.1.1/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.1.0/tests/test_data.py` & `katalytic-data-0.1.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.1.0/PKG-INFO` & `katalytic-data-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-data
-Version: 0.1.0
+Version: 0.1.1
 Summary: This plugin adds utilities for working with data to the katalytic namespace
 Keywords: high-level,data conversion
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

