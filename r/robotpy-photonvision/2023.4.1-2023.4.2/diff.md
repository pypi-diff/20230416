# Comparing `tmp/robotpy-photonvision-2023.4.1.tar.gz` & `tmp/robotpy-photonvision-2023.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotpy-photonvision-2023.4.1.tar", last modified: Sun Apr 16 05:55:29 2023, max compression
+gzip compressed data, was "robotpy-photonvision-2023.4.2.tar", last modified: Sun Apr 16 06:24:44 2023, max compression
```

## Comparing `robotpy-photonvision-2023.4.1.tar` & `robotpy-photonvision-2023.4.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:55:29.055727 robotpy-photonvision-2023.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:55:29.051727 robotpy-photonvision-2023.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:55:29.051727 robotpy-photonvision-2023.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/.github/workflows/dist.yml
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/.github/workflows/scan.yml
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-16 05:55:29.055727 robotpy-photonvision-2023.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:55:29.051727 robotpy-photonvision-2023.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:55:29.051727 robotpy-photonvision-2023.4.1/gen/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/gen/Packet.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/gen/PhotonCamera.yml
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/gen/PhotonPipelineResult.yml
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/gen/PhotonPoseEstimator.yml
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/gen/PhotonTargetSortMode.yml
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/gen/PhotonTrackedTarget.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/gen/PhotonUtils.yml
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/gen/RobotPoseEstimator.yml
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/gen/SimPhotonCamera.yml
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/gen/SimVisionSystem.yml
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/gen/SimVisionTarget.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:55:29.051727 robotpy-photonvision-2023.4.1/photonvision/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/photonvision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:55:29.051727 robotpy-photonvision-2023.4.1/photonvision/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/photonvision/src/headers.patch
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/photonvision/src/module.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/photonvision/src/sources.patch
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-16 05:55:28.000000 robotpy-photonvision-2023.4.1/photonvision/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:55:29.055727 robotpy-photonvision-2023.4.1/robotpy_photonvision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-16 05:55:28.000000 robotpy-photonvision-2023.4.1/robotpy_photonvision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-16 05:55:29.000000 robotpy-photonvision-2023.4.1/robotpy_photonvision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 05:55:28.000000 robotpy-photonvision-2023.4.1/robotpy_photonvision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-16 05:55:28.000000 robotpy-photonvision-2023.4.1/robotpy_photonvision.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 05:55:28.000000 robotpy-photonvision-2023.4.1/robotpy_photonvision.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-16 05:55:28.000000 robotpy-photonvision-2023.4.1/robotpy_photonvision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-16 05:55:28.000000 robotpy-photonvision-2023.4.1/robotpy_photonvision.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 05:55:29.055727 robotpy-photonvision-2023.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:55:29.055727 robotpy-photonvision-2023.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/tests/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/tests/test_photonvision.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-16 05:55:21.000000 robotpy-photonvision-2023.4.1/tests/test_pose_estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:24:44.555797 robotpy-photonvision-2023.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:24:44.551797 robotpy-photonvision-2023.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:24:44.551797 robotpy-photonvision-2023.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/.github/workflows/dist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/.github/workflows/scan.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-16 06:24:44.555797 robotpy-photonvision-2023.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:24:44.555797 robotpy-photonvision-2023.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:24:44.555797 robotpy-photonvision-2023.4.2/gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/gen/Packet.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/gen/PhotonCamera.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/gen/PhotonPipelineResult.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/gen/PhotonPoseEstimator.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/gen/PhotonTargetSortMode.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/gen/PhotonTrackedTarget.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/gen/PhotonUtils.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/gen/RobotPoseEstimator.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/gen/SimPhotonCamera.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/gen/SimVisionSystem.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/gen/SimVisionTarget.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:24:44.555797 robotpy-photonvision-2023.4.2/photonvision/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/photonvision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:24:44.555797 robotpy-photonvision-2023.4.2/photonvision/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/photonvision/src/headers.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/photonvision/src/module.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/photonvision/src/sources.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-16 06:24:44.000000 robotpy-photonvision-2023.4.2/photonvision/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:24:44.555797 robotpy-photonvision-2023.4.2/robotpy_photonvision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-16 06:24:44.000000 robotpy-photonvision-2023.4.2/robotpy_photonvision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-16 06:24:44.000000 robotpy-photonvision-2023.4.2/robotpy_photonvision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 06:24:44.000000 robotpy-photonvision-2023.4.2/robotpy_photonvision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-16 06:24:44.000000 robotpy-photonvision-2023.4.2/robotpy_photonvision.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 06:24:44.000000 robotpy-photonvision-2023.4.2/robotpy_photonvision.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-16 06:24:44.000000 robotpy-photonvision-2023.4.2/robotpy_photonvision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-16 06:24:44.000000 robotpy-photonvision-2023.4.2/robotpy_photonvision.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 06:24:44.555797 robotpy-photonvision-2023.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:24:44.555797 robotpy-photonvision-2023.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/tests/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/tests/test_photonvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-16 06:24:32.000000 robotpy-photonvision-2023.4.2/tests/test_pose_estimator.py
```

### Comparing `robotpy-photonvision-2023.4.1/.github/workflows/dist.yml` & `robotpy-photonvision-2023.4.2/.github/workflows/dist.yml`

 * *Files identical despite different names*

### Comparing `robotpy-photonvision-2023.4.1/LICENSE` & `robotpy-photonvision-2023.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robotpy-photonvision-2023.4.1/PKG-INFO` & `robotpy-photonvision-2023.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotpy-photonvision
-Version: 2023.4.1
+Version: 2023.4.2
 Summary: RobotPy wrappers for photonvision
 Home-page: https://github.com/robotpy/robotpy-photonvision
 Author: RobotPy Development Team
 Author-email: robotpy@googlegroups.com
 License: MIT
 Description: # robotpy-photonvision
         This is a python wrapper around the Photonvision Photonlib library. The RobotPy project is not associated with or endorsed by Photonvision.
```

### Comparing `robotpy-photonvision-2023.4.1/docs/Makefile` & `robotpy-photonvision-2023.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `robotpy-photonvision-2023.4.1/docs/api.rst` & `robotpy-photonvision-2023.4.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `robotpy-photonvision-2023.4.1/docs/conf.py` & `robotpy-photonvision-2023.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `robotpy-photonvision-2023.4.1/docs/make.bat` & `robotpy-photonvision-2023.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `robotpy-photonvision-2023.4.1/gen/PhotonCamera.yml` & `robotpy-photonvision-2023.4.2/gen/PhotonCamera.yml`

 * *Files identical despite different names*

### Comparing `robotpy-photonvision-2023.4.1/gen/PhotonPoseEstimator.yml` & `robotpy-photonvision-2023.4.2/gen/PhotonPoseEstimator.yml`

 * *Files identical despite different names*

### Comparing `robotpy-photonvision-2023.4.1/gen/PhotonTrackedTarget.yml` & `robotpy-photonvision-2023.4.2/gen/PhotonTrackedTarget.yml`

 * *Files identical despite different names*

### Comparing `robotpy-photonvision-2023.4.1/gen/RobotPoseEstimator.yml` & `robotpy-photonvision-2023.4.2/gen/RobotPoseEstimator.yml`

 * *Files identical despite different names*

### Comparing `robotpy-photonvision-2023.4.1/gen/SimPhotonCamera.yml` & `robotpy-photonvision-2023.4.2/gen/SimPhotonCamera.yml`

 * *Files identical despite different names*

### Comparing `robotpy-photonvision-2023.4.1/photonvision/__init__.py` & `robotpy-photonvision-2023.4.2/photonvision/__init__.py`

 * *Files identical despite different names*

### Comparing `robotpy-photonvision-2023.4.1/photonvision/src/headers.patch` & `robotpy-photonvision-2023.4.2/photonvision/src/headers.patch`

 * *Files identical despite different names*

### Comparing `robotpy-photonvision-2023.4.1/photonvision/src/sources.patch` & `robotpy-photonvision-2023.4.2/photonvision/src/sources.patch`

 * *Files identical despite different names*

### Comparing `robotpy-photonvision-2023.4.1/pyproject.toml` & `robotpy-photonvision-2023.4.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = [
     "robotpy-build<2024,>=2023.0.0",
-    "pyntcore~=2023.3.2",
-    "robotpy-apriltag~=2023.3.2",
-    "robotpy-wpimath~=2023.3.2",
-    "wpilib~=2023.3.2",
+    "pyntcore~=2023.4.1",
+    "robotpy-apriltag~=2023.4.1",
+    "robotpy-wpimath~=2023.4.1",
+    "wpilib~=2023.4.1",
 ]
 
 [tool.robotpy-build.metadata]
 name = "robotpy-photonvision"
 description = "RobotPy wrappers for photonvision"
 author = "RobotPy Development Team"
 author_email = "robotpy@googlegroups.com"
 url = "https://github.com/robotpy/robotpy-photonvision"
 license = "MIT"
 install_requires = [
-    "pyntcore<2024.0.0,>=2023.3.2",
-    "robotpy-apriltag<2024.0.0,>=2023.3.2",
-    "robotpy-wpimath<2024.0.0,>=2023.3.2",
-    "wpilib<2024.0.0,>=2023.3.2",
+    "pyntcore<2024.0.0,>=2023.4.1",
+    "robotpy-apriltag<2024.0.0,>=2023.4.1",
+    "robotpy-wpimath<2024.0.0,>=2023.4.1",
+    "wpilib<2024.0.0,>=2023.4.1",
 ]
 
 [tool.robotpy-build]
 base_package = "photonvision"
 
 [tool.robotpy-build.static_libs."photonvision-opencv".maven_lib_download]
 artifact_id = "opencv-cpp"
@@ -32,15 +32,15 @@
 
 libs = ["opencv460"]
 
 [tool.robotpy-build.wrappers."photonvision".maven_lib_download]
 artifact_id = "PhotonLib-cpp"
 group_id = "org.photonvision"
 repo_url = "https://maven.photonvision.org/repository/internal"
-version = "v2023.4.1"
+version = "v2023.4.2"
 
 use_sources = true
 sources = [
     "photonlib/PhotonCamera.cpp",
     "photonlib/PhotonPipelineResult.cpp",
     "photonlib/PhotonPoseEstimator.cpp",
     "photonlib/PhotonTrackedTarget.cpp",
```

### Comparing `robotpy-photonvision-2023.4.1/robotpy_photonvision.egg-info/PKG-INFO` & `robotpy-photonvision-2023.4.2/robotpy_photonvision.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotpy-photonvision
-Version: 2023.4.1
+Version: 2023.4.2
 Summary: RobotPy wrappers for photonvision
 Home-page: https://github.com/robotpy/robotpy-photonvision
 Author: RobotPy Development Team
 Author-email: robotpy@googlegroups.com
 License: MIT
 Description: # robotpy-photonvision
         This is a python wrapper around the Photonvision Photonlib library. The RobotPy project is not associated with or endorsed by Photonvision.
```

### Comparing `robotpy-photonvision-2023.4.1/robotpy_photonvision.egg-info/SOURCES.txt` & `robotpy-photonvision-2023.4.2/robotpy_photonvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

