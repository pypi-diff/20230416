# Comparing `tmp/EasyMLSelector-0.0.4.tar.gz` & `tmp/EasyMLSelector-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyMLSelector-0.0.4.tar", last modified: Wed Jan 11 00:53:01 2023, max compression
+gzip compressed data, was "EasyMLSelector-0.0.5.tar", last modified: Sun Apr 16 19:25:01 2023, max compression
```

## Comparing `EasyMLSelector-0.0.4.tar` & `EasyMLSelector-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-01-11 00:53:01.926809 EasyMLSelector-0.0.4/
--rw-rw-rw-   0        0        0     1080 2023-01-11 00:02:11.000000 EasyMLSelector-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1040 2023-01-11 00:53:01.925810 EasyMLSelector-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      548 2023-01-11 00:49:15.000000 EasyMLSelector-0.0.4/README.md
--rw-rw-rw-   0        0        0      588 2023-01-11 00:52:27.000000 EasyMLSelector-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-11 00:53:01.927810 EasyMLSelector-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-11 00:53:01.913810 EasyMLSelector-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-01-11 00:53:01.923812 EasyMLSelector-0.0.4/src/EasyMLSelector.egg-info/
--rw-rw-rw-   0        0        0     1040 2023-01-11 00:53:01.000000 EasyMLSelector-0.0.4/src/EasyMLSelector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-01-11 00:53:01.000000 EasyMLSelector-0.0.4/src/EasyMLSelector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-11 00:53:01.000000 EasyMLSelector-0.0.4/src/EasyMLSelector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-01-11 00:53:01.000000 EasyMLSelector-0.0.4/src/EasyMLSelector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3581 2023-01-11 00:34:08.000000 EasyMLSelector-0.0.4/src/EasyMLSelector.py
--rw-rw-rw-   0        0        0        0 2023-01-10 23:19:00.000000 EasyMLSelector-0.0.4/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 19:25:01.595098 EasyMLSelector-0.0.5/
+-rw-rw-rw-   0        0        0     1080 2023-01-11 00:02:11.000000 EasyMLSelector-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1256 2023-04-16 19:25:01.594103 EasyMLSelector-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      763 2023-04-16 18:59:35.000000 EasyMLSelector-0.0.5/README.md
+-rw-rw-rw-   0        0        0      589 2023-04-16 18:58:05.000000 EasyMLSelector-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 19:25:01.595098 EasyMLSelector-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 19:25:01.584101 EasyMLSelector-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 19:25:01.590103 EasyMLSelector-0.0.5/src/EasyMLSelector.egg-info/
+-rw-rw-rw-   0        0        0     1256 2023-04-16 19:25:01.000000 EasyMLSelector-0.0.5/src/EasyMLSelector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-04-16 19:25:01.000000 EasyMLSelector-0.0.5/src/EasyMLSelector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 19:25:01.000000 EasyMLSelector-0.0.5/src/EasyMLSelector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-16 19:25:01.000000 EasyMLSelector-0.0.5/src/EasyMLSelector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4982 2023-04-16 19:15:41.000000 EasyMLSelector-0.0.5/src/EasyMLSelector.py
+-rw-rw-rw-   0        0        0        0 2023-01-10 23:19:00.000000 EasyMLSelector-0.0.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 19:25:01.592102 EasyMLSelector-0.0.5/tests/
+-rw-rw-rw-   0        0        0      218 2023-01-11 00:44:04.000000 EasyMLSelector-0.0.5/tests/test.py
```

### Comparing `EasyMLSelector-0.0.4/LICENSE` & `EasyMLSelector-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `EasyMLSelector-0.0.4/PKG-INFO` & `EasyMLSelector-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 Metadata-Version: 2.1
 Name: EasyMLSelector
-Version: 0.0.4
-Summary: Training and Testing for a large number of ML models in one go.
+Version: 0.0.5
+Summary: Training and Testing for a set of scikit-learn models in one go.
 Author-email: wmjg <w.michaelgardner@gmail.com>
 Project-URL: Homepage, https://github.com/wmjg-alt/EasyMLSelector
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## EasyMLSelector
+```
+    pip install EasyMLSelector
+```
     * A class for training and testing many models found in sklearn.
     * Training and Testing for a large number of ML models in one go.
+    * NOTE: Works best with type_filter="regressor"
+    * Best Used with a small dataset to begin an investigation into the best models for your data.
 
 ### Don't know what kind of model is going to best suit your data?
 ```
-from EasyMLSelector import EasyMLSelector
+    from EasyMLSelector import EasyMLSelector
 ```
 
 ### It's as easy as taking your X and y data and using these 2 commands
 ```
-M = EasyMLSelector(type_filter="regressor", Xy_tuple=(X,y))
-M.model_loop()
+    M = EasyMLSelector(type_filter="regressor", Xy_tuple=(X,y))
+    M.model_loop()
 ```
 
 #### Then toy around with the best performing model:
 ```
-M.test_best()
+    M.test_best()
 ```
 ```
-M.best_model
+    M.best_model
 ```
```

### Comparing `EasyMLSelector-0.0.4/pyproject.toml` & `EasyMLSelector-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0","scikit-learn",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "EasyMLSelector"
-version = "0.0.4"
+version = "0.0.5"
 authors = [{ name="wmjg", email="w.michaelgardner@gmail.com" },]
-description = "Training and Testing for a large number of ML models in one go."
+description = "Training and Testing for a set of scikit-learn models in one go."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `EasyMLSelector-0.0.4/src/EasyMLSelector.egg-info/PKG-INFO` & `EasyMLSelector-0.0.5/src/EasyMLSelector.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 Metadata-Version: 2.1
 Name: EasyMLSelector
-Version: 0.0.4
-Summary: Training and Testing for a large number of ML models in one go.
+Version: 0.0.5
+Summary: Training and Testing for a set of scikit-learn models in one go.
 Author-email: wmjg <w.michaelgardner@gmail.com>
 Project-URL: Homepage, https://github.com/wmjg-alt/EasyMLSelector
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## EasyMLSelector
+```
+    pip install EasyMLSelector
+```
     * A class for training and testing many models found in sklearn.
     * Training and Testing for a large number of ML models in one go.
+    * NOTE: Works best with type_filter="regressor"
+    * Best Used with a small dataset to begin an investigation into the best models for your data.
 
 ### Don't know what kind of model is going to best suit your data?
 ```
-from EasyMLSelector import EasyMLSelector
+    from EasyMLSelector import EasyMLSelector
 ```
 
 ### It's as easy as taking your X and y data and using these 2 commands
 ```
-M = EasyMLSelector(type_filter="regressor", Xy_tuple=(X,y))
-M.model_loop()
+    M = EasyMLSelector(type_filter="regressor", Xy_tuple=(X,y))
+    M.model_loop()
 ```
 
 #### Then toy around with the best performing model:
 ```
-M.test_best()
+    M.test_best()
 ```
 ```
-M.best_model
+    M.best_model
 ```
```

