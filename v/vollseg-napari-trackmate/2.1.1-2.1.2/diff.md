# Comparing `tmp/vollseg-napari-trackmate-2.1.1.tar.gz` & `tmp/vollseg-napari-trackmate-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/vollseg-napari-trackmate/dist/.tmp-b4gmgn2m/vollseg-napari-trackmate-2.1.1.tar", last modified: Sun Apr 16 18:07:21 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/vollseg-napari-trackmate/dist/.tmp-tpchekwi/vollseg-napari-trackmate-2.1.2.tar", last modified: Sun Apr 16 18:19:18 2023, max compression
```

## Comparing `vollseg-napari-trackmate-2.1.1.tar` & `vollseg-napari-trackmate-2.1.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:07:21.751479 vollseg-napari-trackmate-2.1.1/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:07:20.645973 vollseg-napari-trackmate-2.1.1/.github/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:07:20.853178 vollseg-napari-trackmate-2.1.1/.github/workflows/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2814 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/.github/workflows/test_and_deploy.yml
--rwxrwxrwx   0 debian    (1000) debian    (1000)      992 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/.gitignore
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:07:20.907912 vollseg-napari-trackmate-2.1.1/.napari-hub/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      463 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/.napari-hub/DESCRIPTION.md
--rwxrwxrwx   0 debian    (1000) debian    (1000)      542 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/.napari-hub/config.yml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1211 2022-12-31 12:38:29.000000 vollseg-napari-trackmate-2.1.1/.pre-commit-config.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/MANIFEST.in
--rwxrwxrwx   0 debian    (1000) debian    (1000)     4320 2023-04-16 18:07:21.754480 vollseg-napari-trackmate-2.1.1/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2911 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/README.md
--rwxrwxrwx   0 debian    (1000) debian    (1000)      274 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/pyproject.toml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1876 2023-04-16 18:07:21.763478 vollseg-napari-trackmate-2.1.1/setup.cfg
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:07:20.666354 vollseg-napari-trackmate-2.1.1/src/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:07:21.220270 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      433 2023-01-24 18:36:39.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    10964 2022-12-29 02:30:28.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_data_model.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      644 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_sample_data.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2118 2023-02-01 20:25:52.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_temporal_plots.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:07:21.662202 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_tests/
--rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_tests/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-01-07 19:22:05.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_tests/test_reader.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      115 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_tests/test_sample_data.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      566 2023-01-07 18:24:47.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_tests/test_widget.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      133 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_tests/test_writer.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-04-16 18:07:19.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_version.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    90693 2023-04-16 18:03:25.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_widget.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      923 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_writer.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      357 2023-01-07 18:24:48.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/launch.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1514 2023-01-03 11:40:24.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/napari.yaml
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:07:21.709577 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/resources/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6153 2022-03-22 02:26:26.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/resources/kapoorlogo.png
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:07:21.432804 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     4320 2023-04-16 18:07:19.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1189 2023-04-16 18:07:20.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-04-16 18:07:19.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       82 2023-04-16 18:07:19.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       85 2023-04-16 18:07:19.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-04-16 18:07:19.000000 vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)      619 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.1/tox.ini
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:19:18.698117 vollseg-napari-trackmate-2.1.2/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:19:17.466679 vollseg-napari-trackmate-2.1.2/.github/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:19:17.691665 vollseg-napari-trackmate-2.1.2/.github/workflows/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2814 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.2/.github/workflows/test_and_deploy.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      992 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.2/.gitignore
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:19:17.759513 vollseg-napari-trackmate-2.1.2/.napari-hub/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      463 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.2/.napari-hub/DESCRIPTION.md
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      542 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.2/.napari-hub/config.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1211 2022-12-31 12:38:29.000000 vollseg-napari-trackmate-2.1.2/.pre-commit-config.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.2/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.2/MANIFEST.in
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4320 2023-04-16 18:19:18.700125 vollseg-napari-trackmate-2.1.2/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2911 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.2/README.md
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      274 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.2/pyproject.toml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1876 2023-04-16 18:19:18.711491 vollseg-napari-trackmate-2.1.2/setup.cfg
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:19:17.487865 vollseg-napari-trackmate-2.1.2/src/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:19:18.147737 vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      433 2023-01-24 18:36:39.000000 vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    10964 2022-12-29 02:30:28.000000 vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/_data_model.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      644 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/_sample_data.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2118 2023-02-01 20:25:52.000000 vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/_temporal_plots.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:19:18.605713 vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/_tests/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/_tests/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-01-07 19:22:05.000000 vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/_tests/test_reader.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      115 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/_tests/test_sample_data.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      566 2023-01-07 18:24:47.000000 vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/_tests/test_widget.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      133 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/_tests/test_writer.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-04-16 18:19:16.000000 vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/_version.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    90769 2023-04-16 18:18:19.000000 vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/_widget.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      923 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/_writer.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      357 2023-01-07 18:24:48.000000 vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/launch.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1514 2023-01-03 11:40:24.000000 vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/napari.yaml
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:19:18.652509 vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/resources/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6153 2022-03-22 02:26:26.000000 vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/resources/kapoorlogo.png
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-16 18:19:18.383309 vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4320 2023-04-16 18:19:16.000000 vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1189 2023-04-16 18:19:17.000000 vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-04-16 18:19:16.000000 vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       82 2023-04-16 18:19:16.000000 vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       85 2023-04-16 18:19:16.000000 vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-04-16 18:19:16.000000 vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      619 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.2/tox.ini
```

### Comparing `vollseg-napari-trackmate-2.1.1/.github/workflows/test_and_deploy.yml` & `vollseg-napari-trackmate-2.1.2/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.1/.gitignore` & `vollseg-napari-trackmate-2.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.1/.napari-hub/config.yml` & `vollseg-napari-trackmate-2.1.2/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.1/.pre-commit-config.yaml` & `vollseg-napari-trackmate-2.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.1/LICENSE` & `vollseg-napari-trackmate-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.1/PKG-INFO` & `vollseg-napari-trackmate-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.1.1
+Version: 2.1.2
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Author: Varun kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
```

### Comparing `vollseg-napari-trackmate-2.1.1/README.md` & `vollseg-napari-trackmate-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.1/setup.cfg` & `vollseg-napari-trackmate-2.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_data_model.py` & `vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/_data_model.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_sample_data.py` & `vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/_sample_data.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_temporal_plots.py` & `vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/_temporal_plots.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_tests/test_widget.py` & `vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_widget.py` & `vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -931,17 +931,19 @@
             unique_dynamic_properties = []
             phenotype_plot_class._repeat_after_plot()
             plot_ax = phenotype_plot_class.plot_ax
             plot_ax.cla()
 
             for unique_track_id in _to_analyze:
 
-                for k in _trackmate_objects.unique_fft_properties[
-                    unique_track_id
-                ].keys():
+                for countk, k in enumerate(
+                    _trackmate_objects.unique_fft_properties[
+                        unique_track_id
+                    ].keys()
+                ):
 
                     unique_fft_properties_tracklet = (
                         _trackmate_objects.unique_fft_properties[
                             unique_track_id
                         ][k]
                     )
 
@@ -1010,30 +1012,30 @@
                                 cluster_time,
                                 cluster_speed,
                                 cluster_motion_angle,
                                 cluster_acceleration,
                                 cluster_distance_cell_mask,
                                 cluster_radial_angle,
                                 cluster_cell_axis_mask,
-                                k,
+                                countk + 1,
                             ]
                         )
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
-                                    k,
+                                    countk + 1,
                                 ]
                             )
 
                         if size_catagories_json is not None:
 
                             unique_shape_properties.append(
                                 [
@@ -1042,15 +1044,15 @@
                                     cluster_volume,
                                     cluster_eccentricity_comp_first,
                                     cluster_eccentricity_comp_second,
                                     cluster_surface_area,
                                     cluster_class,
                                     cluster_class_score,
                                     cluster_class_name,
-                                    k,
+                                    countk + 1,
                                 ]
                             )
 
                         global_data_cluster_plot = []
 
                         global_data_dynamic_cluster_plot = []
 
@@ -1088,15 +1090,15 @@
                                     "Time": cluster_time,
                                     "Speed": cluster_speed,
                                     "Motion Angle": cluster_motion_angle,
                                     "Acceleration": cluster_acceleration,
                                     "Distance cell to tissue": cluster_distance_cell_mask,
                                     "Radial Angle": cluster_radial_angle,
                                     "Cell Axis Mask": cluster_cell_axis_mask,
-                                    "cluster_id": cluster_id,
+                                    "id": cluster_id,
                                 }
                             )
 
                             if len(global_data_dynamic_cluster_plot) == 0:
                                 global_data_dynamic_cluster_plot = (
                                     data_dynamic_cluster_plot
                                 )
@@ -1147,15 +1149,15 @@
                                         "Volume": cluster_volume,
                                         "Eccentricity_Comp_First": cluster_eccentricity_comp_first,
                                         "Eccentricity_Comp_Second": cluster_eccentricity_comp_second,
                                         "Surface_Area": cluster_surface_area,
                                         "Class": cluster_class,
                                         "Class_Score": cluster_class_score,
                                         "Class_Name": cluster_class_name,
-                                        "cluster_id": cluster_id,
+                                        "id": cluster_id,
                                     }
                                 )
                             else:
                                 data_cluster_plot = pd.DataFrame(
                                     {
                                         "Time": cluster_time,
                                         "Radius": cluster_radius,
```

### Comparing `vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/_writer.py` & `vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/_writer.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/napari.yaml` & `vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/napari.yaml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate/resources/kapoorlogo.png` & `vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate/resources/kapoorlogo.png`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate.egg-info/PKG-INFO` & `vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.1.1
+Version: 2.1.2
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Author: Varun kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
```

### Comparing `vollseg-napari-trackmate-2.1.1/src/vollseg_napari_trackmate.egg-info/SOURCES.txt` & `vollseg-napari-trackmate-2.1.2/src/vollseg_napari_trackmate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.1/tox.ini` & `vollseg-napari-trackmate-2.1.2/tox.ini`

 * *Files identical despite different names*

