# Comparing `tmp/carate-0.3.6.tar.gz` & `tmp/carate-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carate-0.3.6.tar", last modified: Thu Apr 13 20:04:07 2023, max compression
+gzip compressed data, was "carate-0.3.7.tar", last modified: Sun Apr 16 13:12:09 2023, max compression
```

## Comparing `carate-0.3.6.tar` & `carate-0.3.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 20:04:07.588658 carate-0.3.6/
--rw-r--r--   0 developer  (1001) developer  (1001)    33670 2023-03-27 16:07:17.000000 carate-0.3.6/LICENSE
--rw-r--r--   0 developer  (1001) developer  (1001)     7206 2023-04-13 20:04:07.588658 carate-0.3.6/PKG-INFO
--rw-r--r--   0 developer  (1001) developer  (1001)     6636 2023-04-05 20:48:54.000000 carate-0.3.6/README.md
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 20:04:07.585324 carate-0.3.6/carate/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 21:05:18.000000 carate-0.3.6/carate/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)      949 2023-04-04 21:05:18.000000 carate-0.3.6/carate/automate.py
--rw-r--r--   0 developer  (1001) developer  (1001)     7619 2023-04-04 21:05:18.000000 carate-0.3.6/carate/config.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1944 2023-04-04 21:05:18.000000 carate-0.3.6/carate/default_interface.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 20:04:07.585324 carate-0.3.6/carate/evaluation/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 21:05:18.000000 carate-0.3.6/carate/evaluation/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)    19159 2023-04-04 21:05:18.000000 carate-0.3.6/carate/evaluation/base.py
--rw-r--r--   0 developer  (1001) developer  (1001)      299 2023-04-04 21:05:18.000000 carate-0.3.6/carate/evaluation/classification.py
--rw-r--r--   0 developer  (1001) developer  (1001)    11463 2023-04-13 19:57:17.000000 carate-0.3.6/carate/evaluation/regression.py
--rw-r--r--   0 developer  (1001) developer  (1001)     7059 2023-04-04 21:05:18.000000 carate-0.3.6/carate/load_data.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 20:04:07.585324 carate-0.3.6/carate/models/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 21:05:18.000000 carate-0.3.6/carate/models/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)      483 2023-04-04 21:05:18.000000 carate-0.3.6/carate/models/base_model.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2048 2023-04-04 21:05:18.000000 carate-0.3.6/carate/models/cgc_classification.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1723 2023-04-04 21:05:18.000000 carate-0.3.6/carate/models/cgc_regression.py
--rw-r--r--   0 developer  (1001) developer  (1001)      905 2023-04-04 21:05:18.000000 carate-0.3.6/carate/optimizer.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 20:04:07.585324 carate-0.3.6/carate/plotting/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 21:05:18.000000 carate-0.3.6/carate/plotting/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)    12811 2023-04-13 19:49:45.000000 carate-0.3.6/carate/plotting/base_plots.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1313 2023-04-13 19:45:37.000000 carate-0.3.6/carate/plotting/plot_classification.py
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-13 19:15:30.000000 carate-0.3.6/carate/plotting/plot_regression.py
--rw-r--r--   0 developer  (1001) developer  (1001)     5375 2023-04-04 21:05:18.000000 carate-0.3.6/carate/run.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 20:04:07.588658 carate-0.3.6/carate/utils/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 21:05:18.000000 carate-0.3.6/carate/utils/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2559 2023-04-04 21:05:18.000000 carate-0.3.6/carate/utils/convert_to_json.py
--rw-r--r--   0 developer  (1001) developer  (1001)     6362 2023-04-04 21:05:18.000000 carate-0.3.6/carate/utils/model_files.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1650 2023-04-04 21:05:18.000000 carate-0.3.6/carate/utils/training_result_parser.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 20:04:07.585324 carate-0.3.6/carate.egg-info/
--rw-r--r--   0 developer  (1001) developer  (1001)     7206 2023-04-13 20:04:07.000000 carate-0.3.6/carate.egg-info/PKG-INFO
--rw-r--r--   0 developer  (1001) developer  (1001)     1065 2023-04-13 20:04:07.000000 carate-0.3.6/carate.egg-info/SOURCES.txt
--rw-r--r--   0 developer  (1001) developer  (1001)        1 2023-04-13 20:04:07.000000 carate-0.3.6/carate.egg-info/dependency_links.txt
--rw-r--r--   0 developer  (1001) developer  (1001)       59 2023-04-13 20:04:07.000000 carate-0.3.6/carate.egg-info/entry_points.txt
--rw-r--r--   0 developer  (1001) developer  (1001)      154 2023-04-13 20:04:07.000000 carate-0.3.6/carate.egg-info/requires.txt
--rw-r--r--   0 developer  (1001) developer  (1001)        7 2023-04-13 20:04:07.000000 carate-0.3.6/carate.egg-info/top_level.txt
--rw-r--r--   0 developer  (1001) developer  (1001)     1022 2023-04-13 20:03:40.000000 carate-0.3.6/pyproject.toml
--rw-r--r--   0 developer  (1001) developer  (1001)      459 2023-04-13 20:04:07.588658 carate-0.3.6/setup.cfg
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 20:04:07.588658 carate-0.3.6/tests/
--rw-r--r--   0 developer  (1001) developer  (1001)     4661 2023-03-29 18:42:59.000000 carate-0.3.6/tests/test_classification.py
--rw-r--r--   0 developer  (1001) developer  (1001)      732 2023-04-12 18:04:08.000000 carate-0.3.6/tests/test_cli.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2217 2023-03-29 18:42:59.000000 carate-0.3.6/tests/test_config.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2642 2023-04-12 18:04:08.000000 carate-0.3.6/tests/test_data_loader.py
--rw-r--r--   0 developer  (1001) developer  (1001)      902 2023-04-13 19:42:15.000000 carate-0.3.6/tests/test_plotting.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2344 2023-03-30 15:56:56.000000 carate-0.3.6/tests/test_regression.py
--rw-r--r--   0 developer  (1001) developer  (1001)      546 2023-03-27 16:07:17.000000 carate-0.3.6/tests/test_runner.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1522 2023-03-29 18:42:59.000000 carate-0.3.6/tests/test_utils_convert_py_to_json.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-16 13:12:09.148313 carate-0.3.7/
+-rw-r--r--   0 developer  (1001) developer  (1001)    33670 2023-03-27 16:07:17.000000 carate-0.3.7/LICENSE
+-rw-r--r--   0 developer  (1001) developer  (1001)     7206 2023-04-16 13:12:09.148313 carate-0.3.7/PKG-INFO
+-rw-r--r--   0 developer  (1001) developer  (1001)     6636 2023-04-05 20:48:54.000000 carate-0.3.7/README.md
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-16 13:12:09.144980 carate-0.3.7/carate/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.7/carate/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      949 2023-04-15 18:59:22.000000 carate-0.3.7/carate/automate.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     7619 2023-04-15 18:59:22.000000 carate-0.3.7/carate/config.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1944 2023-04-15 18:59:22.000000 carate-0.3.7/carate/default_interface.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-16 13:12:09.148313 carate-0.3.7/carate/evaluation/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.7/carate/evaluation/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)    19159 2023-04-15 18:59:22.000000 carate-0.3.7/carate/evaluation/base.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      299 2023-04-15 18:59:22.000000 carate-0.3.7/carate/evaluation/classification.py
+-rw-r--r--   0 developer  (1001) developer  (1001)    11480 2023-04-16 12:42:34.000000 carate-0.3.7/carate/evaluation/regression.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     7059 2023-04-15 18:59:22.000000 carate-0.3.7/carate/load_data.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-16 13:12:09.148313 carate-0.3.7/carate/models/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.7/carate/models/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      483 2023-04-15 18:59:22.000000 carate-0.3.7/carate/models/base_model.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2048 2023-04-15 18:59:22.000000 carate-0.3.7/carate/models/cgc_classification.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1723 2023-04-15 18:59:22.000000 carate-0.3.7/carate/models/cgc_regression.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      905 2023-04-15 18:59:22.000000 carate-0.3.7/carate/optimizer.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-16 13:12:09.148313 carate-0.3.7/carate/plotting/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.7/carate/plotting/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)    12834 2023-04-15 18:59:22.000000 carate-0.3.7/carate/plotting/base_plots.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1263 2023-04-15 18:59:22.000000 carate-0.3.7/carate/plotting/plot_classification.py
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.7/carate/plotting/plot_regression.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     5375 2023-04-15 18:59:22.000000 carate-0.3.7/carate/run.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-16 13:12:09.148313 carate-0.3.7/carate/utils/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.7/carate/utils/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2559 2023-04-15 18:59:22.000000 carate-0.3.7/carate/utils/convert_to_json.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     6362 2023-04-15 18:59:22.000000 carate-0.3.7/carate/utils/model_files.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1650 2023-04-15 18:59:22.000000 carate-0.3.7/carate/utils/training_result_parser.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-16 13:12:09.148313 carate-0.3.7/carate.egg-info/
+-rw-r--r--   0 developer  (1001) developer  (1001)     7206 2023-04-16 13:12:09.000000 carate-0.3.7/carate.egg-info/PKG-INFO
+-rw-r--r--   0 developer  (1001) developer  (1001)     1065 2023-04-16 13:12:09.000000 carate-0.3.7/carate.egg-info/SOURCES.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)        1 2023-04-16 13:12:09.000000 carate-0.3.7/carate.egg-info/dependency_links.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)       59 2023-04-16 13:12:09.000000 carate-0.3.7/carate.egg-info/entry_points.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)      154 2023-04-16 13:12:09.000000 carate-0.3.7/carate.egg-info/requires.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)        7 2023-04-16 13:12:09.000000 carate-0.3.7/carate.egg-info/top_level.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)     1022 2023-04-16 13:12:03.000000 carate-0.3.7/pyproject.toml
+-rw-r--r--   0 developer  (1001) developer  (1001)      459 2023-04-16 13:12:09.148313 carate-0.3.7/setup.cfg
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-16 13:12:09.148313 carate-0.3.7/tests/
+-rw-r--r--   0 developer  (1001) developer  (1001)     4661 2023-03-29 18:42:59.000000 carate-0.3.7/tests/test_classification.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      732 2023-04-12 18:04:08.000000 carate-0.3.7/tests/test_cli.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2217 2023-03-29 18:42:59.000000 carate-0.3.7/tests/test_config.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2642 2023-04-12 18:04:08.000000 carate-0.3.7/tests/test_data_loader.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      902 2023-04-13 19:42:15.000000 carate-0.3.7/tests/test_plotting.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2828 2023-04-16 12:44:17.000000 carate-0.3.7/tests/test_regression.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      546 2023-03-27 16:07:17.000000 carate-0.3.7/tests/test_runner.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1522 2023-03-29 18:42:59.000000 carate-0.3.7/tests/test_utils_convert_py_to_json.py
```

### Comparing `carate-0.3.6/LICENSE` & `carate-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `carate-0.3.6/PKG-INFO` & `carate-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carate
-Version: 0.3.6
+Version: 0.3.7
 Summary: Providing reproducible modeling
 Author-email: "Julian M. Kleber" <julian.m.kleber@gmail.com>
 Project-URL: Homepage, https://www.codeberg.org/sail.black/carate.git
 Project-URL: Bug Tracker, https://www.codeberg.org/sail.black/carate.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `carate-0.3.6/README.md` & `carate-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `carate-0.3.6/carate/automate.py` & `carate-0.3.7/carate/automate.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.6/carate/config.py` & `carate-0.3.7/carate/config.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.6/carate/default_interface.py` & `carate-0.3.7/carate/default_interface.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.6/carate/evaluation/base.py` & `carate-0.3.7/carate/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.6/carate/evaluation/regression.py` & `carate-0.3.7/carate/evaluation/regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,22 +148,23 @@
             override,
             normalize,
             custom_size,
         ) = self._get_defaults(locals())
 
         # data container
         result = {}
-        test_mse = []
-        train_mae = []
-        train_mse = []
-        
 
         save_model_parameters(model_net=model_net, save_dir=result_save_dir)
         for i in range(num_cv):
+            
             tmp = {}
+            test_mse = []
+            train_mae = []
+            train_mse = []
+
             loaded_dataset: torch.utils.data.Dataset
             (
                 test_dataset,
                 train_dataset,
                 test_loader,
                 train_loader,
                 loaded_dataset,
```

### Comparing `carate-0.3.6/carate/load_data.py` & `carate-0.3.7/carate/load_data.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.6/carate/models/cgc_classification.py` & `carate-0.3.7/carate/models/cgc_classification.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.6/carate/models/cgc_regression.py` & `carate-0.3.7/carate/models/cgc_regression.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.6/carate/optimizer.py` & `carate-0.3.7/carate/optimizer.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.6/carate/plotting/base_plots.py` & `carate-0.3.7/carate/plotting/base_plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,17 @@
     max_val = []
     min_val = []
     avg_val = []
 
     arr_res = np.zeros((len(result), len(result[0][key_val])))
 
     for i, res in enumerate(result):
-        assert len(res[key_val]) == arr_res.shape[1], str(len(res[key_val])) +str(arr_res.shape[1])
+        assert len(res[key_val]) == arr_res.shape[1], str(len(res[key_val])) + str(
+            arr_res.shape[1]
+        )
         arr_res[i, :] = res[key_val]
 
     for i in range(arr_res.shape[1]):
         max_val.append(get_max(arr_res[:, i].tolist()))
         min_val.append(get_min(arr_res[:, i].tolist()))
         avg_val.append(get_avg(arr_res[:, i].tolist()))
```

### Comparing `carate-0.3.6/carate/plotting/plot_classification.py` & `carate-0.3.7/carate/plotting/plot_classification.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,23 +31,21 @@
     """
 
     legend_text = path_to_directory.split("/")[-1]
 
     if data_name is None:
         data_name = f"{legend_text}.json"
 
-  
     result = get_stacked_list(
-            path_to_directory=path_to_directory,
-            num_cv=5,
-            json_name=data_name,
-        )
+        path_to_directory=path_to_directory,
+        num_cv=5,
+        json_name=data_name,
+    )
 
-  
     plot_range_band_single(
-            result,
-            file_name=f"{legend_text}_{parameter}",
-            save_dir=save_dir,
-            key_val=parameter,
-            alpha=0.4,
-            legend_text=legend_text,
-        )
+        result,
+        file_name=f"{legend_text}_{parameter}",
+        save_dir=save_dir,
+        key_val=parameter,
+        alpha=0.4,
+        legend_text=legend_text,
+    )
```

### Comparing `carate-0.3.6/carate/run.py` & `carate-0.3.7/carate/run.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.6/carate/utils/convert_to_json.py` & `carate-0.3.7/carate/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.6/carate/utils/model_files.py` & `carate-0.3.7/carate/utils/model_files.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.6/carate/utils/training_result_parser.py` & `carate-0.3.7/carate/utils/training_result_parser.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.6/carate.egg-info/PKG-INFO` & `carate-0.3.7/carate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carate
-Version: 0.3.6
+Version: 0.3.7
 Summary: Providing reproducible modeling
 Author-email: "Julian M. Kleber" <julian.m.kleber@gmail.com>
 Project-URL: Homepage, https://www.codeberg.org/sail.black/carate.git
 Project-URL: Bug Tracker, https://www.codeberg.org/sail.black/carate.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `carate-0.3.6/carate.egg-info/SOURCES.txt` & `carate-0.3.7/carate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `carate-0.3.6/pyproject.toml` & `carate-0.3.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "carate"
-version = "0.3.6"
+version = "0.3.7"
 authors = [
   { name="Julian M. Kleber", email="julian.m.kleber@gmail.com" },
 ]
 description = "Providing reproducible modeling"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `carate-0.3.6/tests/test_classification.py` & `carate-0.3.7/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.6/tests/test_cli.py` & `carate-0.3.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.6/tests/test_config.py` & `carate-0.3.7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.6/tests/test_data_loader.py` & `carate-0.3.7/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.6/tests/test_plotting.py` & `carate-0.3.7/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.6/tests/test_regression.py` & `carate-0.3.7/tests/test_regression.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,35 @@
 """
 Perform tests on the functionality of running models against
 a regression dataset
 
 :author: Julian M. Kleber
 """
+import os
 from typing import Type
 import logging
 
 import torch
 
+from amarium.utils import append_slash, load_json_from_file
+
 from carate.run import RunInitializer
 import carate.models.cgc_regression as CGCR
 from carate.evaluation.regression import RegressionEvaluation
 from carate.load_data import StandardDatasetMoleculeNet, StandardDatasetTUDataset
 from tests.utils import check_dir_paths, check_result_files
 
 logging.basicConfig(
     filename="train.log",
     encoding="utf-8",
     level=logging.DEBUG,
     format="%(asctime)s %(message)s",
 )
 
 
-def test_regression_multitaksing():
-    check_dir_paths()
-    config_filepath = "tests/config/regression_alchemy_test.py"
-    run_title = "ALCHEMY_test"
-    data_set_name = "alchemy_full"
-    runner = RunInitializer.from_file(config_filepath=config_filepath)
-    result_dir = f"tests/results/{run_title}"
-    assert str(runner.data_set) == "StandardTUDataset"
-    runner.run()  # takes instance attributes as parameters for the run() function
-
-    check_result_files(
-        result_dir=result_dir,
-        data_set_name=data_set_name,
-        run_title=run_title,
-        override=True,
-    )
-
 
 def test_regression_override():
     check_dir_paths()
     config_filepath = "tests/config/regression_test_config_override.py"
     run_title = "ZINC_test"
     data_set_name = "ZINC_test"
     runner = RunInitializer.from_file(config_filepath=config_filepath)
@@ -51,14 +37,16 @@
     assert str(runner.data_set) == "StandardTUDataset"
     runner.run()  # takes instance attributes as parameters for the run() function
 
     check_result_files(
         result_dir=result_dir, run_title=run_title, data_set_name=data_set_name
     )
 
+    verify_len_json(result_dir, dataset_name="ZINC_test")
+
 
 def test_regression_no_override():
     check_dir_paths()
 
     config_filepath = "tests/config/regression_test_config_no_override.py"
     run_title = "ZINC_test"
     data_set_name = "ZINC_test"
@@ -69,7 +57,36 @@
 
     check_result_files(
         result_dir=result_dir,
         run_title=run_title,
         data_set_name=data_set_name,
         override=True,
     )
+
+    verify_len_json(result_dir, dataset_name="ZINC_test")
+
+
+def test_regression_multitaksing():
+    check_dir_paths()
+    config_filepath = "tests/config/regression_alchemy_test.py"
+    run_title = "ALCHEMY_test"
+    data_set_name = "alchemy_full"
+    runner = RunInitializer.from_file(config_filepath=config_filepath)
+    result_dir = f"tests/results/{run_title}"
+    assert str(runner.data_set) == "StandardTUDataset"
+    runner.run()  # takes instance attributes as parameters for the run() function
+
+    check_result_files(
+        result_dir=result_dir,
+        data_set_name=data_set_name,
+        run_title=run_title,
+        override=True,
+    )
+
+    verify_len_json(result_dir, dataset_name="alchemy_full")
+
+def verify_len_json(result_dir:str, dataset_name:str)->None:
+
+    
+    result_file = append_slash(result_dir) + f"data/CV_1/{dataset_name}.json"
+    result = load_json_from_file(result_file)
+    assert len(result["MAE Train"]) == 2
```

### Comparing `carate-0.3.6/tests/test_runner.py` & `carate-0.3.7/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.6/tests/test_utils_convert_py_to_json.py` & `carate-0.3.7/tests/test_utils_convert_py_to_json.py`

 * *Files identical despite different names*

