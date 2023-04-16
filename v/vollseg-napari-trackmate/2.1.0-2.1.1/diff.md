# Comparing `tmp/vollseg-napari-trackmate-2.1.0.tar.gz` & `tmp/vollseg-napari-trackmate-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vollseg-napari-trackmate-2.1.0.tar", last modified: Mon Apr  3 07:24:15 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/vollseg-napari-trackmate/dist/.tmp-b4gmgn2m/vollseg-napari-trackmate-2.1.1.tar", last modified: Sun Apr 16 18:07:21 2023, max compression
```

## Comparing `vollseg-napari-trackmate-2.1.0.tar` & `vollseg-napari-trackmate-2.1.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-s---   0 uzj81mi  (302337) jsy      (302032)        0 2023-04-03 07:24:15.027612 vollseg-napari-trackmate-2.1.0/
-drwxr-s---   0 uzj81mi  (302337) jsy      (302032)        0 2023-04-03 07:24:14.922360 vollseg-napari-trackmate-2.1.0/.github/
-drwxr-s---   0 uzj81mi  (302337) jsy      (302032)        0 2023-04-03 07:24:14.937639 vollseg-napari-trackmate-2.1.0/.github/workflows/
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)     2814 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/.github/workflows/test_and_deploy.yml
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)      992 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/.gitignore
-drwxr-s---   0 uzj81mi  (302337) jsy      (302032)        0 2023-04-03 07:24:14.939868 vollseg-napari-trackmate-2.1.0/.napari-hub/
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)      463 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/.napari-hub/DESCRIPTION.md
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)      542 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/.napari-hub/config.yml
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)     1211 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/.pre-commit-config.yaml
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)     1487 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/LICENSE
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)       96 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/MANIFEST.in
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)     4320 2023-04-03 07:24:15.028030 vollseg-napari-trackmate-2.1.0/PKG-INFO
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)     2911 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/README.md
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)      274 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/pyproject.toml
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)     1876 2023-04-03 07:24:15.029601 vollseg-napari-trackmate-2.1.0/setup.cfg
-drwxr-s---   0 uzj81mi  (302337) jsy      (302032)        0 2023-04-03 07:24:14.926238 vollseg-napari-trackmate-2.1.0/src/
-drwxr-s---   0 uzj81mi  (302337) jsy      (302032)        0 2023-04-03 07:24:14.991164 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)      433 2023-01-26 21:14:09.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/__init__.py
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)    10964 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_data_model.py
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)      644 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_sample_data.py
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)     2118 2023-02-01 20:38:39.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_temporal_plots.py
-drwxr-s---   0 uzj81mi  (302337) jsy      (302032)        0 2023-04-03 07:24:15.011274 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_tests/
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)        0 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_tests/__init__.py
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)      107 2023-01-07 19:22:38.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_tests/test_reader.py
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)      115 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_tests/test_sample_data.py
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)      566 2023-01-07 18:28:11.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_tests/test_widget.py
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)      133 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_tests/test_writer.py
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)      160 2023-04-03 07:24:14.984625 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_version.py
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)    81982 2023-04-03 07:22:29.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_widget.py
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)      923 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_writer.py
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)      357 2023-01-07 18:28:11.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/launch.py
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)     1514 2023-01-03 12:16:33.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/napari.yaml
-drwxr-s---   0 uzj81mi  (302337) jsy      (302032)        0 2023-04-03 07:24:15.012279 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/resources/
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)     6153 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/resources/kapoorlogo.png
-drwxr-s---   0 uzj81mi  (302337) jsy      (302032)        0 2023-04-03 07:24:15.003440 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate.egg-info/
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)     4320 2023-04-03 07:24:14.992907 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate.egg-info/PKG-INFO
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)     1189 2023-04-03 07:24:14.995047 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)        1 2023-04-03 07:24:14.996819 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)       82 2023-04-03 07:24:14.998719 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate.egg-info/entry_points.txt
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)       85 2023-04-03 07:24:14.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate.egg-info/requires.txt
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)       25 2023-04-03 07:24:14.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate.egg-info/top_level.txt
--rw-r-----   0 uzj81mi  (302337) jsy      (302032)      619 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/tox.ini
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:07:21.751479 vollseg-napari-trackmate-2.1.1/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:07:20.645973 vollseg-napari-trackmate-2.1.1/.github/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:07:20.853178 vollseg-napari-trackmate-2.1.1/.github/workflows/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2814 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/.github/workflows/test_and_deploy.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      992 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/.gitignore
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:07:20.907912 vollseg-napari-trackmate-2.1.1/.napari-hub/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      463 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/.napari-hub/DESCRIPTION.md
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      542 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/.napari-hub/config.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1211 2022-12-31 12:38:29.000000 vollseg-napari-trackmate-2.1.1/.pre-commit-config.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/MANIFEST.in
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4320 2023-04-16 18:07:21.754480 vollseg-napari-trackmate-2.1.1/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2911 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/README.md
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      274 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/pyproject.toml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1876 2023-04-16 18:07:21.763478 vollseg-napari-trackmate-2.1.1/setup.cfg
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:07:20.666354 vollseg-napari-trackmate-2.1.1/src/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:07:21.220270 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      433 2023-01-24 18:36:39.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    10964 2022-12-29 02:30:28.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_data_model.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      644 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_sample_data.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2118 2023-02-01 20:25:52.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_temporal_plots.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:07:21.662202 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_tests/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_tests/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-01-07 19:22:05.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_tests/test_reader.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      115 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_tests/test_sample_data.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      566 2023-01-07 18:24:47.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_tests/test_widget.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      133 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_tests/test_writer.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-04-16 18:07:19.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_version.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    90693 2023-04-16 18:03:25.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_widget.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      923 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_writer.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      357 2023-01-07 18:24:48.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/launch.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1514 2023-01-03 11:40:24.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/napari.yaml
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:07:21.709577 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/resources/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6153 2022-03-22 02:26:26.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/resources/kapoorlogo.png
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:07:21.432804 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4320 2023-04-16 18:07:19.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1189 2023-04-16 18:07:20.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-04-16 18:07:19.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       82 2023-04-16 18:07:19.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       85 2023-04-16 18:07:19.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-04-16 18:07:19.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      619 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/tox.ini
```

### Comparing `vollseg-napari-trackmate-2.1.0/.github/workflows/test_and_deploy.yml` & `vollseg-napari-trackmate-2.1.1/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.0/.gitignore` & `vollseg-napari-trackmate-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.0/.napari-hub/config.yml` & `vollseg-napari-trackmate-2.1.1/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.0/.pre-commit-config.yaml` & `vollseg-napari-trackmate-2.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.0/LICENSE` & `vollseg-napari-trackmate-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.0/PKG-INFO` & `vollseg-napari-trackmate-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.1.0
+Version: 2.1.1
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Author: Varun kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
```

### Comparing `vollseg-napari-trackmate-2.1.0/README.md` & `vollseg-napari-trackmate-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.0/setup.cfg` & `vollseg-napari-trackmate-2.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_data_model.py` & `vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_data_model.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_sample_data.py` & `vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_sample_data.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_temporal_plots.py` & `vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_temporal_plots.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_tests/test_widget.py` & `vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_widget.py` & `vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -843,75 +843,96 @@
         _Color_tracks(spot_attributes, track_attributes)
 
     def _refreshTrackData(pred):
 
         nonlocal _to_analyze
         unique_tracks, unique_tracks_properties, track_id = pred
         features = {
-            "time": np.asarray(unique_tracks_properties, dtype="float64")[
+            "time": np.asarray(unique_tracks_properties, dtype="float16")[
                 :, 0
             ],
             "generation": np.asarray(
-                unique_tracks_properties, dtype="float64"
+                unique_tracks_properties, dtype="float16"
             )[:, 2],
-            "speed": np.asarray(unique_tracks_properties, dtype="float64")[
+            "radius": np.asarray(unique_tracks_properties, dtype="float16")[
                 :, 3
             ],
-            "directional_change_rate": np.asarray(
-                unique_tracks_properties, dtype="float64"
+            "volume_pixels": np.asarray(
+                unique_tracks_properties, dtype="float16"
             )[:, 4],
-            "total-intensity": np.asarray(
-                unique_tracks_properties, dtype="float64"
+            "eccentricity_comp_first": np.asarray(
+                unique_tracks_properties, dtype="float16"
             )[:, 5],
-            "volume_pixels": np.asarray(
-                unique_tracks_properties, dtype="float64"
+            "eccentricity_comp_second": np.asarray(
+                unique_tracks_properties, dtype="float16"
             )[:, 6],
-            "acceleration": np.asarray(
-                unique_tracks_properties, dtype="float64"
+            "surface_area": np.asarray(
+                unique_tracks_properties, dtype="float16"
             )[:, 7],
             "cluster_class": np.asarray(
-                unique_tracks_properties, dtype="float64"
+                unique_tracks_properties, dtype="float16"
             )[:, 8],
             "cluster_score": np.asarray(
-                unique_tracks_properties, dtype="float64"
+                unique_tracks_properties, dtype="float16"
             )[:, 9],
+            "total_intensity": np.asarray(
+                unique_tracks_properties, dtype="float16"
+            )[:, 10],
+            "speed": np.asarray(unique_tracks_properties, dtype="float16")[
+                :, 11
+            ],
+            "motion_angle": np.asarray(
+                unique_tracks_properties, dtype="float16"
+            )[:, 12],
+            "acceleration": np.asarray(
+                unique_tracks_properties, dtype="float16"
+            )[:, 13],
+            "distance_cell_mask": np.asarray(
+                unique_tracks_properties, dtype="float16"
+            )[:, 14],
+            "radial_angle": np.asarray(
+                unique_tracks_properties, dtype="float16"
+            )[:, 15],
+            "cell_axis_mask": np.asarray(
+                unique_tracks_properties, dtype="float16"
+            )[:, 16],
         }
         print("Refreshing track data")
         for layer in list(plugin.viewer.value.layers):
             if (
                 "Track" == layer.name
                 or "Boxes" == layer.name
                 or "Track_points" == layer.name
             ):
                 plugin.viewer.value.layers.remove(layer)
-        vertices = unique_tracks[:, 1:]
-        plugin.viewer.value.add_points(vertices, name="Track_points", size=1)
-        print("Added vertices")
+
         plugin.viewer.value.add_tracks(
             unique_tracks,
             name="Track",
             features=features,
         )
         print("Track data refreshed")
         if str(track_id) not in TrackidBox and track_id is not None:
             _to_analyze = [int(track_id)]
         show_phenotype()
         select_track_nature()
 
     def show_phenotype():
 
-        nonlocal _to_analyze, size_catagories_json
+        nonlocal _to_analyze, size_catagories_json, _trackmate_objects
 
         phenotype_plot_class._reset_container(
             phenotype_plot_class.scroll_layout
         )
-        if _to_analyze is not None:
+
+        if _to_analyze is not None and _trackmate_objects is not None:
 
             unique_fft_properties = []
             unique_shape_properties = []
+            unique_dynamic_properties = []
             phenotype_plot_class._repeat_after_plot()
             plot_ax = phenotype_plot_class.plot_ax
             plot_ax.cla()
 
             for unique_track_id in _to_analyze:
 
                 for k in _trackmate_objects.unique_fft_properties[
@@ -952,38 +973,67 @@
                             cluster_volume,
                             cluster_eccentricity_comp_first,
                             cluster_eccentricity_comp_second,
                             cluster_surface_area,
                             cluster_class,
                             cluster_class_score,
                         ) = unique_shape_properties_tracklet
+
+                        unique_dynamic_properties_tracklet = (
+                            _trackmate_objects.unique_dynamic_properties[
+                                unique_track_id
+                            ][k]
+                        )
+                        (
+                            cluster_time,
+                            cluster_speed,
+                            cluster_motion_angle,
+                            cluster_acceleration,
+                            cluster_distance_cell_mask,
+                            cluster_radial_angle,
+                            cluster_cell_axis_mask,
+                        ) = unique_dynamic_properties_tracklet
+
                         cluster_class_name = []
                         if size_catagories_json is not None:
                             for i in range(cluster_class.shape[0]):
                                 if cluster_class[i] is not None:
                                     cluster_class_name.append(
                                         size_catagories_json[
                                             str(int(cluster_class[i]))
                                         ]
                                     )
                                 else:
                                     cluster_class_name.append(None)
 
+                        unique_dynamic_properties.append(
+                            [
+                                cluster_time,
+                                cluster_speed,
+                                cluster_motion_angle,
+                                cluster_acceleration,
+                                cluster_distance_cell_mask,
+                                cluster_radial_angle,
+                                cluster_cell_axis_mask,
+                                k,
+                            ]
+                        )
                         if size_catagories_json is None:
 
                             unique_shape_properties.append(
                                 [
                                     cluster_time,
                                     cluster_radius,
                                     cluster_volume,
                                     cluster_eccentricity_comp_first,
                                     cluster_eccentricity_comp_second,
                                     cluster_surface_area,
                                     cluster_class,
                                     cluster_class_score,
+                                    k,
                                 ]
                             )
 
                         if size_catagories_json is not None:
 
                             unique_shape_properties.append(
                                 [
@@ -992,19 +1042,76 @@
                                     cluster_volume,
                                     cluster_eccentricity_comp_first,
                                     cluster_eccentricity_comp_second,
                                     cluster_surface_area,
                                     cluster_class,
                                     cluster_class_score,
                                     cluster_class_name,
+                                    k,
                                 ]
                             )
 
                         global_data_cluster_plot = []
-                        index_array = []
+
+                        global_data_dynamic_cluster_plot = []
+
+                        for count, i in enumerate(
+                            range(len(unique_dynamic_properties))
+                        ):
+
+                            current_unique_dynamic_properties = (
+                                unique_dynamic_properties[i]
+                            )
+                            cluster_time = current_unique_dynamic_properties[0]
+                            cluster_speed = current_unique_dynamic_properties[
+                                1
+                            ]
+                            cluster_motion_angle = (
+                                current_unique_dynamic_properties[2]
+                            )
+                            cluster_acceleration = (
+                                current_unique_dynamic_properties[3]
+                            )
+                            cluster_distance_cell_mask = (
+                                current_unique_dynamic_properties[4]
+                            )
+                            cluster_radial_angle = (
+                                current_unique_dynamic_properties[5]
+                            )
+                            cluster_cell_axis_mask = (
+                                current_unique_dynamic_properties[6]
+                            )
+
+                            cluster_id = current_unique_dynamic_properties[-1]
+
+                            data_dynamic_cluster_plot = pd.DataFrame(
+                                {
+                                    "Time": cluster_time,
+                                    "Speed": cluster_speed,
+                                    "Motion Angle": cluster_motion_angle,
+                                    "Acceleration": cluster_acceleration,
+                                    "Distance cell to tissue": cluster_distance_cell_mask,
+                                    "Radial Angle": cluster_radial_angle,
+                                    "Cell Axis Mask": cluster_cell_axis_mask,
+                                    "cluster_id": cluster_id,
+                                }
+                            )
+
+                            if len(global_data_dynamic_cluster_plot) == 0:
+                                global_data_dynamic_cluster_plot = (
+                                    data_dynamic_cluster_plot
+                                )
+                            else:
+                                global_data_dynamic_cluster_plot = pd.concat(
+                                    [
+                                        global_data_dynamic_cluster_plot,
+                                        data_dynamic_cluster_plot,
+                                    ],
+                                    ignore_index=True,
+                                )
 
                         for count, i in enumerate(
                             range(len(unique_shape_properties))
                         ):
 
                             current_unique_shape_properties = (
                                 unique_shape_properties[i]
@@ -1022,14 +1129,16 @@
                             cluster_surface_area = (
                                 current_unique_shape_properties[5]
                             )
                             cluster_class = current_unique_shape_properties[6]
                             cluster_class_score = (
                                 current_unique_shape_properties[7]
                             )
+
+                            cluster_id = current_unique_shape_properties[-1]
                             if size_catagories_json is not None:
 
                                 cluster_class_name = (
                                     current_unique_shape_properties[8]
                                 )
                                 data_cluster_plot = pd.DataFrame(
                                     {
@@ -1038,176 +1147,251 @@
                                         "Volume": cluster_volume,
                                         "Eccentricity_Comp_First": cluster_eccentricity_comp_first,
                                         "Eccentricity_Comp_Second": cluster_eccentricity_comp_second,
                                         "Surface_Area": cluster_surface_area,
                                         "Class": cluster_class,
                                         "Class_Score": cluster_class_score,
                                         "Class_Name": cluster_class_name,
+                                        "cluster_id": cluster_id,
                                     }
                                 )
                             else:
                                 data_cluster_plot = pd.DataFrame(
                                     {
                                         "Time": cluster_time,
                                         "Radius": cluster_radius,
                                         "Volume": cluster_volume,
                                         "Eccentricity_Comp_First": cluster_eccentricity_comp_first,
                                         "Eccentricity_Comp_Second": cluster_eccentricity_comp_second,
                                         "Surface_Area": cluster_surface_area,
                                         "Class": cluster_class,
                                         "Class_Score": cluster_class_score,
+                                        "cluster_id": cluster_id,
                                     }
                                 )
 
-                            for _ in range(np.asarray(cluster_time).shape[0]):
-                                index_array.append(int(count))
-
-                            data_cluster_plot = data_cluster_plot.mask(
-                                data_cluster_plot.astype(object).eq("None")
-                            ).dropna()
-
                             if len(global_data_cluster_plot) == 0:
                                 global_data_cluster_plot = data_cluster_plot
                             else:
                                 global_data_cluster_plot = pd.concat(
                                     [
                                         global_data_cluster_plot,
                                         data_cluster_plot,
                                     ],
                                     ignore_index=True,
                                 )
 
             if len(_to_analyze) <= 2:
-                global_data_cluster_plot["index"] = index_array[
-                    0 : len(global_data_cluster_plot)
-                ]
 
-                global_data_cluster_plot = global_data_cluster_plot.set_index(
-                    "index"
+                sns.scatterplot(
+                    global_data_dynamic_cluster_plot,
+                    x="Time",
+                    y="Speed",
+                    hue="cluster_id",
+                    ax=plot_ax,
                 )
-                global_data_cluster_plot.drop_duplicates(
-                    global_data_cluster_plot
+
+                plot_ax.set_title("Speed")
+                plot_ax.set_xlabel("Time (min)")
+
+                phenotype_plot_class._repeat_after_plot()
+                plot_ax = phenotype_plot_class.plot_ax
+
+                sns.scatterplot(
+                    global_data_dynamic_cluster_plot,
+                    x="Time",
+                    y="Motion Angle",
+                    hue="cluster_id",
+                    ax=plot_ax,
                 )
-                if size_catagories_json is None:
-                    sns.lineplot(
-                        global_data_cluster_plot,
-                        x="Time",
-                        y="Class",
-                        hue=global_data_cluster_plot.index.values.tolist(),
-                        ax=plot_ax,
-                    )
-                    sns.move_legend(plot_ax, "lower right")
-                if size_catagories_json is not None:
-                    sns.lineplot(
-                        global_data_cluster_plot,
-                        x="Time",
-                        y="Class_Name",
-                        hue=global_data_cluster_plot.index.values.tolist(),
-                        ax=plot_ax,
-                    )
-                    sns.move_legend(plot_ax, "lower right")
-                plot_ax.set_title("Cluster class")
+
+                plot_ax.set_title("Motion Angle")
+                plot_ax.set_xlabel("Time (min)")
+
+                phenotype_plot_class._repeat_after_plot()
+                plot_ax = phenotype_plot_class.plot_ax
+
+                sns.scatterplot(
+                    global_data_dynamic_cluster_plot,
+                    x="Time",
+                    y="Radial Angle",
+                    hue="cluster_id",
+                    ax=plot_ax,
+                )
+
+                plot_ax.set_title("Radial Angle")
+                plot_ax.set_xlabel("Time (min)")
+
+                phenotype_plot_class._repeat_after_plot()
+                plot_ax = phenotype_plot_class.plot_ax
+
+                sns.scatterplot(
+                    global_data_dynamic_cluster_plot,
+                    x="Time",
+                    y="Acceleration",
+                    hue="cluster_id",
+                    ax=plot_ax,
+                )
+
+                plot_ax.set_title("Acceleration")
+                plot_ax.set_xlabel("Time (min)")
+
+                phenotype_plot_class._repeat_after_plot()
+                plot_ax = phenotype_plot_class.plot_ax
+
+                sns.scatterplot(
+                    global_data_dynamic_cluster_plot,
+                    x="Time",
+                    y="Distance cell to tissue",
+                    hue="cluster_id",
+                    ax=plot_ax,
+                )
+
+                plot_ax.set_title("Distance cell to tissue")
+                plot_ax.set_xlabel("Time (min)")
+
+                phenotype_plot_class._repeat_after_plot()
+                plot_ax = phenotype_plot_class.plot_ax
+
+                sns.scatterplot(
+                    global_data_dynamic_cluster_plot,
+                    x="Time",
+                    y="Cell Axis Mask",
+                    hue="cluster_id",
+                    ax=plot_ax,
+                )
+
+                plot_ax.set_title("Cell Axis Mask")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
-                sns.lineplot(
+                sns.scatterplot(
                     global_data_cluster_plot,
                     x="Time",
                     y="Radius",
-                    hue=global_data_cluster_plot.index.values.tolist(),
+                    hue="cluster_id",
                     ax=plot_ax,
                 )
-                sns.move_legend(plot_ax, "lower right")
+
                 plot_ax.set_title("Radius")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
-                sns.lineplot(
+                sns.scatterplot(
                     global_data_cluster_plot,
                     x="Time",
                     y="Volume",
-                    hue=global_data_cluster_plot.index.values.tolist(),
+                    hue="cluster_id",
                     ax=plot_ax,
                 )
-                sns.move_legend(plot_ax, "lower right")
+
                 plot_ax.set_title("Volume")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
-                sns.lineplot(
+                sns.scatterplot(
                     global_data_cluster_plot,
                     x="Time",
                     y="Surface_Area",
-                    hue=global_data_cluster_plot.index.values.tolist(),
+                    hue="cluster_id",
                     ax=plot_ax,
                 )
-                sns.move_legend(plot_ax, "lower right")
+
                 plot_ax.set_title("Surface_Area")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
-                sns.lineplot(
+                sns.scatterplot(
                     global_data_cluster_plot,
                     x="Time",
                     y="Eccentricity_Comp_First",
-                    hue=global_data_cluster_plot.index.values.tolist(),
+                    hue="cluster_id",
                     ax=plot_ax,
                 )
-                sns.move_legend(plot_ax, "lower right")
+
                 plot_ax.set_title("Eccentricity Comp First")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
-                sns.lineplot(
+                sns.scatterplot(
                     global_data_cluster_plot,
                     x="Time",
                     y="Eccentricity_Comp_Second",
-                    hue=global_data_cluster_plot.index.values.tolist(),
+                    hue="cluster_id",
                     ax=plot_ax,
                 )
-                sns.move_legend(plot_ax, "lower right")
+
                 plot_ax.set_title("Eccentricity Comp Second")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
+                if not global_data_cluster_plot["Class"].isna().all():
+                    if size_catagories_json is None:
+                        sns.scatterplot(
+                            global_data_cluster_plot,
+                            x="Time",
+                            y="Class",
+                            hue="cluster_id",
+                            ax=plot_ax,
+                        )
+
+                    if size_catagories_json is not None:
+                        sns.scatterplot(
+                            global_data_cluster_plot,
+                            x="Time",
+                            y="Class_Name",
+                            hue="cluster_id",
+                            ax=plot_ax,
+                        )
+
+                    plot_ax.set_title("Cluster class")
+                    plot_ax.set_xlabel("Time (min)")
+
+                    phenotype_plot_class._repeat_after_plot()
+                    plot_ax = phenotype_plot_class.plot_ax
+
             data_fft_plot = pd.DataFrame(
                 {
                     "Frequ": unique_fft_properties[0][2],
                     "Amplitude": np.sum(unique_fft_properties, axis=0)[3],
                 }
             )
 
             data_time_plot = pd.DataFrame(
                 {
                     "Time": unique_fft_properties[0][0],
                     "Intensity": np.sum(unique_fft_properties, axis=0)[1],
                 }
             )
 
-            sns.lineplot(data_time_plot, x="Time", y="Intensity", ax=plot_ax)
+            sns.scatterplot(
+                data_time_plot, x="Time", y="Intensity", ax=plot_ax
+            )
             plot_ax.set_title("Cell Intensity")
             plot_ax.set_xlabel("Time (min)")
             plot_ax.set_ylabel("Amplitude")
 
             phenotype_plot_class._repeat_after_plot()
             plot_ax = phenotype_plot_class.plot_ax
 
-            sns.lineplot(data_fft_plot, x="Frequ", y="Amplitude", ax=plot_ax)
+            sns.scatterplot(
+                data_fft_plot, x="Frequ", y="Amplitude", ax=plot_ax
+            )
             plot_ax.set_title("FFT Intensity")
             plot_ax.set_xlabel("Frequency (1/min)")
             plot_ax.set_ylabel("Amplitude")
 
     def return_color_tracks(pred):
 
         if not isinstance(pred, int):
@@ -1426,14 +1610,30 @@
                     plot_ax.set_ylabel("Class")
 
                     stat_plot_class._repeat_after_plot()
                     plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
+                    _trackmate_objects.mitotic_mean_distance_cell_mask,
+                    _trackmate_objects.mitotic_var_distance_cell_mask,
+                    linestyle="None",
+                    marker=".",
+                    mfc="green",
+                    ecolor="green",
+                )
+                plot_ax.set_title("Cell-tissue distance")
+                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_ylabel("um")
+
+                stat_plot_class._repeat_after_plot()
+                plot_ax = stat_plot_class.plot_ax
+
+                plot_ax.errorbar(
+                    _trackmate_objects.time,
                     _trackmate_objects.mitotic_mean_directional_change,
                     _trackmate_objects.mitotic_var_directional_change,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
@@ -1576,14 +1776,30 @@
                     plot_ax.set_ylabel("Class")
 
                     stat_plot_class._repeat_after_plot()
                     plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
+                    _trackmate_objects.non_mitotic_mean_distance_cell_mask,
+                    _trackmate_objects.non_mitotic_var_distance_cell_mask,
+                    linestyle="None",
+                    marker=".",
+                    mfc="green",
+                    ecolor="green",
+                )
+                plot_ax.set_title("Cell-tissue distance")
+                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_ylabel("um")
+
+                stat_plot_class._repeat_after_plot()
+                plot_ax = stat_plot_class.plot_ax
+
+                plot_ax.errorbar(
+                    _trackmate_objects.time,
                     _trackmate_objects.non_mitotic_mean_directional_change,
                     _trackmate_objects.non_mitotic_var_directional_change,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
@@ -1723,14 +1939,30 @@
                     plot_ax.set_ylabel("Class")
 
                     stat_plot_class._repeat_after_plot()
                     plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
+                    _trackmate_objects.all_mean_distance_cell_mask,
+                    _trackmate_objects.all_var_distance_cell_mask,
+                    linestyle="None",
+                    marker=".",
+                    mfc="green",
+                    ecolor="green",
+                )
+                plot_ax.set_title("Cell-tissue distance")
+                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_ylabel("um")
+
+                stat_plot_class._repeat_after_plot()
+                plot_ax = stat_plot_class.plot_ax
+
+                plot_ax.errorbar(
+                    _trackmate_objects.time,
                     _trackmate_objects.all_mean_directional_change,
                     _trackmate_objects.all_var_directional_change,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
@@ -2023,14 +2255,15 @@
         if (
             _trackmate_objects is not None
             and _track_ids_analyze is not None
             and value is not None
         ):
 
             track_id = value
+
             show_track(track_id)
 
     widget_for_cloud_auto_encoder_modeltype = {
         CloudAutoEncoder: plugin.cloud_auto_encoder_model,
         "No(Encoder)": plugin.cloud_auto_encoder_model_none,
         CUSTOM_MODEL_CLOUD_AUTO_ENCODER: plugin.model_folder_cloud_auto,
     }
@@ -2110,17 +2343,18 @@
             model_cluster = get_model_cluster(
                 *model_selected_cloud_auto_encoder,
                 *model_selected_cluster,
             )
 
             try:
                 device = torch.device("cuda:0")
+                model_cluster.to(device)
             except ValueError:
                 device = torch.device("cpu")
-            model_cluster.to(device)
+                model_cluster.to(device)
         else:
             model_cluster = None
 
         plugin.progress_bar.value = 0
         plugin.progress_bar.show()
         num_points = 0
         if model_selected_cloud_auto_encoder is not None:
```

### Comparing `vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_writer.py` & `vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_writer.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/napari.yaml` & `vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/napari.yaml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/resources/kapoorlogo.png` & `vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/resources/kapoorlogo.png`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate.egg-info/PKG-INFO` & `vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.1.0
+Version: 2.1.1
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Author: Varun kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
```

### Comparing `vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate.egg-info/SOURCES.txt` & `vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.0/tox.ini` & `vollseg-napari-trackmate-2.1.1/tox.ini`

 * *Files identical despite different names*

