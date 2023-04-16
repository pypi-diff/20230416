# Comparing `tmp/mine-3.0.tar.gz` & `tmp/mine-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mine-3.0.tar", max compression
+gzip compressed data, was "mine-3.0.1.tar", max compression
```

## Comparing `mine-3.0.tar` & `mine-3.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1088 2020-10-23 17:27:35.488744 mine-3.0/LICENSE.md
--rw-r--r--   0        0        0     2840 2023-04-15 20:56:22.116675 mine-3.0/README.md
--rw-r--r--   0        0        0      216 2023-04-15 20:56:22.117593 mine-3.0/mine/__init__.py
--rw-r--r--   0        0        0     6624 2023-04-15 20:56:22.117919 mine-3.0/mine/cli.py
--rw-r--r--   0        0        0     2865 2023-04-15 20:56:22.118231 mine-3.0/mine/common.py
--rw-r--r--   0        0        0     6669 2023-04-15 20:56:22.118536 mine-3.0/mine/manager.py
--rw-r--r--   0        0        0      232 2020-10-23 17:27:35.490798 mine-3.0/mine/models/__init__.py
--rw-r--r--   0        0        0      424 2021-05-25 20:38:13.436751 mine-3.0/mine/models/_bases.py
--rw-r--r--   0        0        0     1803 2020-10-23 17:27:35.491009 mine-3.0/mine/models/application.py
--rw-r--r--   0        0        0     3083 2023-04-15 21:11:38.472518 mine-3.0/mine/models/computer.py
--rw-r--r--   0        0        0      501 2020-10-23 17:27:35.491219 mine-3.0/mine/models/config.py
--rw-r--r--   0        0        0     5145 2020-10-23 17:27:35.491342 mine-3.0/mine/models/data.py
--rw-r--r--   0        0        0     6544 2022-09-12 19:07:44.627359 mine-3.0/mine/models/status.py
--rw-r--r--   0        0        0     1052 2020-10-23 17:27:35.491579 mine-3.0/mine/models/timestamp.py
--rwxr-xr-x   0        0        0     2667 2023-04-15 20:56:22.118831 mine-3.0/mine/services.py
--rw-r--r--   0        0        0      573 2023-04-15 20:56:22.119108 mine-3.0/mine/settings.py
--rw-r--r--   0        0        0       34 2020-10-23 17:27:35.491927 mine-3.0/mine/tests/__init__.py
--rw-r--r--   0        0        0     1038 2023-04-15 20:56:22.119410 mine-3.0/mine/tests/conftest.py
--rw-r--r--   0        0        0        9 2020-10-23 17:27:35.492167 mine-3.0/mine/tests/files/.gitignore
--rw-r--r--   0        0        0      513 2020-10-23 17:27:35.492276 mine-3.0/mine/tests/files/mine-in.yml
--rw-r--r--   0        0        0      587 2020-10-23 17:27:35.492361 mine-3.0/mine/tests/files/mine-out.yml
--rw-r--r--   0        0        0     3996 2023-04-15 20:56:22.119702 mine-3.0/mine/tests/test_cli.py
--rw-r--r--   0        0        0     3506 2023-04-15 20:56:22.119999 mine-3.0/mine/tests/test_manager.py
--rw-r--r--   0        0        0     1489 2023-04-15 20:56:22.120292 mine-3.0/mine/tests/test_models_application.py
--rw-r--r--   0        0        0     4234 2023-04-15 21:06:06.553234 mine-3.0/mine/tests/test_models_computer.py
--rw-r--r--   0        0        0      316 2023-04-15 20:56:22.120872 mine-3.0/mine/tests/test_models_config.py
--rw-r--r--   0        0        0      682 2023-04-15 20:56:22.121156 mine-3.0/mine/tests/test_models_data.py
--rw-r--r--   0        0        0     4961 2023-04-15 20:56:22.121453 mine-3.0/mine/tests/test_models_status.py
--rw-r--r--   0        0        0     1750 2023-04-15 20:56:22.121738 mine-3.0/mine/tests/test_models_timestamp.py
--rw-r--r--   0        0        0     3217 2023-04-15 20:56:22.122027 mine-3.0/mine/tests/test_services.py
--rw-r--r--   0        0        0     2324 2023-04-15 21:16:46.750689 mine-3.0/pyproject.toml
--rw-r--r--   0        0        0     4351 1970-01-01 00:00:00.000000 mine-3.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2019-05-21 02:49:19.000000 mine-3.0.1/LICENSE.md
+-rw-r--r--   0        0        0     2840 2023-04-16 19:11:58.196023 mine-3.0.1/README.md
+-rw-r--r--   0        0        0      340 2023-04-16 19:25:03.010573 mine-3.0.1/mine/__init__.py
+-rw-r--r--   0        0        0     6624 2023-04-16 19:11:58.197283 mine-3.0.1/mine/cli.py
+-rw-r--r--   0        0        0     2865 2023-04-16 19:11:58.197615 mine-3.0.1/mine/common.py
+-rw-r--r--   0        0        0     6669 2023-04-16 19:18:48.322162 mine-3.0.1/mine/manager.py
+-rw-r--r--   0        0        0      232 2019-05-21 02:49:19.000000 mine-3.0.1/mine/models/__init__.py
+-rw-r--r--   0        0        0      424 2021-06-02 19:31:21.821486 mine-3.0.1/mine/models/_bases.py
+-rw-r--r--   0        0        0     1803 2019-05-21 02:49:19.000000 mine-3.0.1/mine/models/application.py
+-rw-r--r--   0        0        0     3083 2023-04-16 19:11:58.197913 mine-3.0.1/mine/models/computer.py
+-rw-r--r--   0        0        0      501 2019-05-21 02:49:19.000000 mine-3.0.1/mine/models/config.py
+-rw-r--r--   0        0        0     5145 2020-05-16 16:13:05.000000 mine-3.0.1/mine/models/data.py
+-rw-r--r--   0        0        0     6544 2022-09-08 17:31:06.428139 mine-3.0.1/mine/models/status.py
+-rw-r--r--   0        0        0     1052 2019-05-21 02:49:19.000000 mine-3.0.1/mine/models/timestamp.py
+-rwxr-xr-x   0        0        0     2667 2023-04-16 19:11:58.198225 mine-3.0.1/mine/services.py
+-rw-r--r--   0        0        0      573 2023-04-16 19:13:26.811463 mine-3.0.1/mine/settings.py
+-rw-r--r--   0        0        0       34 2016-09-23 05:48:42.000000 mine-3.0.1/mine/tests/__init__.py
+-rw-r--r--   0        0        0     1038 2023-04-16 19:11:58.198685 mine-3.0.1/mine/tests/conftest.py
+-rw-r--r--   0        0        0        9 2016-09-23 02:41:14.000000 mine-3.0.1/mine/tests/files/.gitignore
+-rw-r--r--   0        0        0      513 2016-09-23 02:41:14.000000 mine-3.0.1/mine/tests/files/mine-in.yml
+-rw-r--r--   0        0        0      587 2016-09-23 02:41:14.000000 mine-3.0.1/mine/tests/files/mine-out.yml
+-rw-r--r--   0        0        0     3996 2023-04-16 19:11:58.199066 mine-3.0.1/mine/tests/test_cli.py
+-rw-r--r--   0        0        0     3506 2023-04-16 19:11:58.199194 mine-3.0.1/mine/tests/test_manager.py
+-rw-r--r--   0        0        0     1489 2023-04-16 19:11:58.199324 mine-3.0.1/mine/tests/test_models_application.py
+-rw-r--r--   0        0        0     4234 2023-04-16 19:11:58.199638 mine-3.0.1/mine/tests/test_models_computer.py
+-rw-r--r--   0        0        0      316 2023-04-16 19:11:58.199968 mine-3.0.1/mine/tests/test_models_config.py
+-rw-r--r--   0        0        0      682 2023-04-16 19:11:58.200223 mine-3.0.1/mine/tests/test_models_data.py
+-rw-r--r--   0        0        0     4961 2023-04-16 19:11:58.200402 mine-3.0.1/mine/tests/test_models_status.py
+-rw-r--r--   0        0        0     1750 2023-04-16 19:11:58.200536 mine-3.0.1/mine/tests/test_models_timestamp.py
+-rw-r--r--   0        0        0     3211 2023-04-16 19:21:47.166045 mine-3.0.1/mine/tests/test_services.py
+-rw-r--r--   0        0        0     2329 2023-04-16 19:26:09.147871 mine-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4366 1970-01-01 00:00:00.000000 mine-3.0.1/PKG-INFO
```

### Comparing `mine-3.0/LICENSE.md` & `mine-3.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mine-3.0/README.md` & `mine-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mine-3.0/mine/cli.py` & `mine-3.0.1/mine/cli.py`

 * *Files identical despite different names*

### Comparing `mine-3.0/mine/common.py` & `mine-3.0.1/mine/common.py`

 * *Files identical despite different names*

### Comparing `mine-3.0/mine/manager.py` & `mine-3.0.1/mine/manager.py`

 * *Files identical despite different names*

### Comparing `mine-3.0/mine/models/application.py` & `mine-3.0.1/mine/models/application.py`

 * *Files identical despite different names*

### Comparing `mine-3.0/mine/models/computer.py` & `mine-3.0.1/mine/models/computer.py`

 * *Files identical despite different names*

### Comparing `mine-3.0/mine/models/data.py` & `mine-3.0.1/mine/models/data.py`

 * *Files identical despite different names*

### Comparing `mine-3.0/mine/models/status.py` & `mine-3.0.1/mine/models/status.py`

 * *Files identical despite different names*

### Comparing `mine-3.0/mine/models/timestamp.py` & `mine-3.0.1/mine/models/timestamp.py`

 * *Files identical despite different names*

### Comparing `mine-3.0/mine/services.py` & `mine-3.0.1/mine/services.py`

 * *Files identical despite different names*

### Comparing `mine-3.0/mine/settings.py` & `mine-3.0.1/mine/settings.py`

 * *Files identical despite different names*

### Comparing `mine-3.0/mine/tests/conftest.py` & `mine-3.0.1/mine/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mine-3.0/mine/tests/files/mine-in.yml` & `mine-3.0.1/mine/tests/files/mine-in.yml`

 * *Files identical despite different names*

### Comparing `mine-3.0/mine/tests/files/mine-out.yml` & `mine-3.0.1/mine/tests/files/mine-out.yml`

 * *Files identical despite different names*

### Comparing `mine-3.0/mine/tests/test_cli.py` & `mine-3.0.1/mine/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mine-3.0/mine/tests/test_manager.py` & `mine-3.0.1/mine/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `mine-3.0/mine/tests/test_models_application.py` & `mine-3.0.1/mine/tests/test_models_application.py`

 * *Files identical despite different names*

### Comparing `mine-3.0/mine/tests/test_models_computer.py` & `mine-3.0.1/mine/tests/test_models_computer.py`

 * *Files identical despite different names*

### Comparing `mine-3.0/mine/tests/test_models_data.py` & `mine-3.0.1/mine/tests/test_models_data.py`

 * *Files identical despite different names*

### Comparing `mine-3.0/mine/tests/test_models_status.py` & `mine-3.0.1/mine/tests/test_models_status.py`

 * *Files identical despite different names*

### Comparing `mine-3.0/mine/tests/test_models_timestamp.py` & `mine-3.0.1/mine/tests/test_models_timestamp.py`

 * *Files identical despite different names*

### Comparing `mine-3.0/mine/tests/test_services.py` & `mine-3.0.1/mine/tests/test_services.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import pytest
 
 from mine import services
 from mine.tests.conftest import FILES
 
 
-@pytest.yield_fixture
+@pytest.fixture
 def tmp_dir(tmpdir):
     cwd = os.getcwd()
     tmpdir.chdir()
     yield str(tmpdir)
     os.chdir(cwd)
```

### Comparing `mine-3.0/pyproject.toml` & `mine-3.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "mine"
-version = "3.0"
+version = "3.0.1"
 description = "Share application state across computers using Dropbox."
 
 license = "MIT"
 
 authors = ["Jace Browning <jacebrowning@gmail.com>"]
 
 readme = "README.md"
@@ -34,19 +34,19 @@
     "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
 
 python = "^3.8"
 
-YORM = "^1.4"
-psutil = "^2.2"
+YORM = "^1.6"
+psutil = "^4.4"
 crayons = "~0.1"
-minilog = "^2.0"
-universal-startfile = "*"
+minilog = "^2.1"
+universal-startfile = "^0.2"
 
 [tool.poetry.dev-dependencies]
 
 # Formatters
 black = "^22.1"
 tomli = "*" # missing 'black' dependency
 isort = "^5.10"
@@ -59,30 +59,30 @@
 types-setuptools = "*"
 
 # Testing
 pytest = "^7.1"
 pytest-describe = "^2.0"
 pytest-expecter = "^3.0"
 pytest-random = "*"
-pytest-cov = "^3.0"
+pytest-cov = "^4.0"
 freezegun = "*"
 
 # Reports
 coveragespace = "^6.0"
 
 # Documentation
 mkdocs = "^1.4"
 pygments = "^2.11"
 
 # Tooling
 pyinstaller = "*"
 sniffer = "*"
 MacFSEvents = { version = "*", platform = "darwin" }
 pync = { version = "*", platform = "darwin" }
-ipython = "^7.16.3"
+ipython = "^8.10.0"
 
 [tool.poetry.scripts]
 
 mine = "mine.cli:main"
 
 [tool.black]
```

### Comparing `mine-3.0/PKG-INFO` & `mine-3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mine
-Version: 3.0
+Version: 3.0.1
 Summary: Share application state across computers using Dropbox.
 Home-page: https://pypi.org/project/mine
 License: MIT
 Author: Jace Browning
 Author-email: jacebrowning@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,19 +23,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Utilities
-Requires-Dist: YORM (>=1.4,<2.0)
+Requires-Dist: YORM (>=1.6,<2.0)
 Requires-Dist: crayons (>=0.1,<0.2)
-Requires-Dist: minilog (>=2.0,<3.0)
-Requires-Dist: psutil (>=2.2,<3.0)
-Requires-Dist: universal-startfile
+Requires-Dist: minilog (>=2.1,<3.0)
+Requires-Dist: psutil (>=4.4,<5.0)
+Requires-Dist: universal-startfile (>=0.2,<0.3)
 Project-URL: Documentation, https://mine.readthedocs.io
 Project-URL: Repository, https://github.com/jacebrowning/mine
 Description-Content-Type: text/markdown
 
 # Overview
 
 This program lets you synchronize application data using Dropbox.
```

