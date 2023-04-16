# Comparing `tmp/easyexplore-0.7.3.tar.gz` & `tmp/easyexplore-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyexplore-0.7.3.tar", last modified: Sat Apr  1 21:59:46 2023, max compression
+gzip compressed data, was "easyexplore-0.7.4.tar", last modified: Sun Apr 16 18:41:34 2023, max compression
```

## Comparing `easyexplore-0.7.3.tar` & `easyexplore-0.7.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-01 21:59:46.284145 easyexplore-0.7.3/
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    34924 2022-06-08 17:04:34.000000 easyexplore-0.7.3/LICENSE
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     6495 2023-04-01 21:59:46.283609 easyexplore-0.7.3/PKG-INFO
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     5834 2022-06-08 17:04:34.000000 easyexplore-0.7.3/README.md
-drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-01 21:59:46.268580 easyexplore-0.7.3/easyexplore/
--rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-08 17:04:34.000000 easyexplore-0.7.3/easyexplore/__init__.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    17324 2022-06-08 17:04:34.000000 easyexplore-0.7.3/easyexplore/anomaly_detector.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    71221 2023-04-01 21:43:51.000000 easyexplore-0.7.3/easyexplore/data_explorer.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    50281 2022-06-08 17:04:34.000000 easyexplore-0.7.3/easyexplore/data_import_export.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)   246750 2022-06-08 17:04:34.000000 easyexplore-0.7.3/easyexplore/data_visualizer.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)   118207 2022-06-08 17:04:34.000000 easyexplore-0.7.3/easyexplore/interactive_visualizer.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)   117800 2022-06-08 17:04:34.000000 easyexplore-0.7.3/easyexplore/unsupervised_machine_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    81723 2022-06-08 17:04:34.000000 easyexplore-0.7.3/easyexplore/utils.py
-drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-01 21:59:46.272545 easyexplore-0.7.3/easyexplore.egg-info/
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     6495 2023-04-01 21:59:46.000000 easyexplore-0.7.3/easyexplore.egg-info/PKG-INFO
--rw-r--r--   0 giannibalistreri   (501) staff       (20)      670 2023-04-01 21:59:46.000000 easyexplore-0.7.3/easyexplore.egg-info/SOURCES.txt
--rw-r--r--   0 giannibalistreri   (501) staff       (20)        1 2023-04-01 21:59:46.000000 easyexplore-0.7.3/easyexplore.egg-info/dependency_links.txt
--rw-r--r--   0 giannibalistreri   (501) staff       (20)      381 2023-04-01 21:59:46.000000 easyexplore-0.7.3/easyexplore.egg-info/requires.txt
--rw-r--r--   0 giannibalistreri   (501) staff       (20)       12 2023-04-01 21:59:46.000000 easyexplore-0.7.3/easyexplore.egg-info/top_level.txt
--rw-r--r--   0 giannibalistreri   (501) staff       (20)       38 2023-04-01 21:59:46.284426 easyexplore-0.7.3/setup.cfg
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     2640 2023-04-01 21:43:51.000000 easyexplore-0.7.3/setup.py
-drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-01 21:59:46.282488 easyexplore-0.7.3/test/
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     3528 2022-06-08 17:04:34.000000 easyexplore-0.7.3/test/test_anomaly_detector.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     2283 2022-06-08 17:04:34.000000 easyexplore-0.7.3/test/test_data_explorer.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     3359 2022-06-08 17:04:34.000000 easyexplore-0.7.3/test/test_data_import_export.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    61864 2022-06-08 17:04:35.000000 easyexplore-0.7.3/test/test_data_visualizer.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     3899 2022-06-08 17:04:35.000000 easyexplore-0.7.3/test/test_interactive_visualizer.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    38657 2022-06-08 17:04:35.000000 easyexplore-0.7.3/test/test_unsupervised_machine_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    11116 2022-06-08 17:04:35.000000 easyexplore-0.7.3/test/test_utils.py
+drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-16 18:41:34.621934 easyexplore-0.7.4/
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    34924 2022-06-08 17:04:34.000000 easyexplore-0.7.4/LICENSE
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     6495 2023-04-16 18:41:34.621480 easyexplore-0.7.4/PKG-INFO
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     5834 2022-06-08 17:04:34.000000 easyexplore-0.7.4/README.md
+drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-16 18:41:34.599916 easyexplore-0.7.4/easyexplore/
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-08 17:04:34.000000 easyexplore-0.7.4/easyexplore/__init__.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    17324 2022-06-08 17:04:34.000000 easyexplore-0.7.4/easyexplore/anomaly_detector.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    71221 2023-04-01 21:43:51.000000 easyexplore-0.7.4/easyexplore/data_explorer.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    50281 2022-06-08 17:04:34.000000 easyexplore-0.7.4/easyexplore/data_import_export.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)   246752 2023-04-16 18:34:47.000000 easyexplore-0.7.4/easyexplore/data_visualizer.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)   118207 2022-06-08 17:04:34.000000 easyexplore-0.7.4/easyexplore/interactive_visualizer.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)   117800 2022-06-08 17:04:34.000000 easyexplore-0.7.4/easyexplore/unsupervised_machine_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    81723 2022-06-08 17:04:34.000000 easyexplore-0.7.4/easyexplore/utils.py
+drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-16 18:41:34.606068 easyexplore-0.7.4/easyexplore.egg-info/
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     6495 2023-04-16 18:41:34.000000 easyexplore-0.7.4/easyexplore.egg-info/PKG-INFO
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)      670 2023-04-16 18:41:34.000000 easyexplore-0.7.4/easyexplore.egg-info/SOURCES.txt
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)        1 2023-04-16 18:41:34.000000 easyexplore-0.7.4/easyexplore.egg-info/dependency_links.txt
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)      381 2023-04-16 18:41:34.000000 easyexplore-0.7.4/easyexplore.egg-info/requires.txt
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)       12 2023-04-16 18:41:34.000000 easyexplore-0.7.4/easyexplore.egg-info/top_level.txt
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)       38 2023-04-16 18:41:34.622090 easyexplore-0.7.4/setup.cfg
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     2640 2023-04-16 18:35:32.000000 easyexplore-0.7.4/setup.py
+drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-16 18:41:34.620312 easyexplore-0.7.4/test/
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     3528 2022-06-08 17:04:34.000000 easyexplore-0.7.4/test/test_anomaly_detector.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     2283 2022-06-08 17:04:34.000000 easyexplore-0.7.4/test/test_data_explorer.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     3359 2022-06-08 17:04:34.000000 easyexplore-0.7.4/test/test_data_import_export.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    61864 2022-06-08 17:04:35.000000 easyexplore-0.7.4/test/test_data_visualizer.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     3899 2022-06-08 17:04:35.000000 easyexplore-0.7.4/test/test_interactive_visualizer.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    38657 2022-06-08 17:04:35.000000 easyexplore-0.7.4/test/test_unsupervised_machine_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    11116 2022-06-08 17:04:35.000000 easyexplore-0.7.4/test/test_utils.py
```

### Comparing `easyexplore-0.7.3/LICENSE` & `easyexplore-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `easyexplore-0.7.3/PKG-INFO` & `easyexplore-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyexplore
-Version: 0.7.3
+Version: 0.7.4
 Summary: Toolbox for easy and effective data exploration
 Home-page: https://github.com/GianniBalistreri/easyexplore
 Author: Gianni Francesco Balistreri
 Author-email: gbalistreri@gmx.de
 License: GNU
 Keywords: data-exploration interactive-visualization plotly machine-learning
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easyexplore-0.7.3/README.md` & `easyexplore-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `easyexplore-0.7.3/easyexplore/anomaly_detector.py` & `easyexplore-0.7.4/easyexplore/anomaly_detector.py`

 * *Files identical despite different names*

### Comparing `easyexplore-0.7.3/easyexplore/data_explorer.py` & `easyexplore-0.7.4/easyexplore/data_explorer.py`

 * *Files identical despite different names*

### Comparing `easyexplore-0.7.3/easyexplore/data_import_export.py` & `easyexplore-0.7.4/easyexplore/data_import_export.py`

 * *Files identical despite different names*

### Comparing `easyexplore-0.7.3/easyexplore/data_visualizer.py` & `easyexplore-0.7.4/easyexplore/data_visualizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -760,15 +760,15 @@
                                     if not isinstance(self.subplots[plot]['kwargs'].get('layout'), dict):
                                         self.subplots[plot]['kwargs'].update({'layout': {}})
                                 else:
                                     self.subplots[plot]['kwargs'].update({'layout': {}})
                             else:
                                 self.subplots[plot]['kwargs'].update({'layout': {}})
                         else:
-                            self.subplots[plot]['kwargs'].update({'layout': {}})
+                            self.subplots[plot].update({'kwargs': {'layout': {}}})
                     else:
                         raise DataVisualizerException('Subplots dictionary should contain dictionaries'.format(self.subplots))
             else:
                 raise DataVisualizerException('Subplots parameter should be a dictionary containing dictionaries -> Dict[str, dict]'.format(self.subplots))
 
     def _hierarchical_data_set(self, value_feature: str, color_features: List[str] = None) -> pd.DataFrame:
         """
```

### Comparing `easyexplore-0.7.3/easyexplore/interactive_visualizer.py` & `easyexplore-0.7.4/easyexplore/interactive_visualizer.py`

 * *Files identical despite different names*

### Comparing `easyexplore-0.7.3/easyexplore/unsupervised_machine_learning.py` & `easyexplore-0.7.4/easyexplore/unsupervised_machine_learning.py`

 * *Files identical despite different names*

### Comparing `easyexplore-0.7.3/easyexplore/utils.py` & `easyexplore-0.7.4/easyexplore/utils.py`

 * *Files identical despite different names*

### Comparing `easyexplore-0.7.3/easyexplore.egg-info/PKG-INFO` & `easyexplore-0.7.4/easyexplore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyexplore
-Version: 0.7.3
+Version: 0.7.4
 Summary: Toolbox for easy and effective data exploration
 Home-page: https://github.com/GianniBalistreri/easyexplore
 Author: Gianni Francesco Balistreri
 Author-email: gbalistreri@gmx.de
 License: GNU
 Keywords: data-exploration interactive-visualization plotly machine-learning
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easyexplore-0.7.3/easyexplore.egg-info/SOURCES.txt` & `easyexplore-0.7.4/easyexplore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easyexplore-0.7.3/setup.py` & `easyexplore-0.7.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 with open('requirements.txt', 'r') as _requirements:
     requires = _requirements.read()
 
 requires = [r.strip() for r in requires.split('\n') if ((r.strip()[0] != "#") and (len(r.strip()) > 3) and "-e git://" not in r)]
 
 setuptools.setup(
     name='easyexplore',
-    version='0.7.3',
+    version='0.7.4',
     author='Gianni Francesco Balistreri',
     author_email='gbalistreri@gmx.de',
     description='Toolbox for easy and effective data exploration',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='data-exploration interactive-visualization plotly machine-learning',
     license='GNU',
```

### Comparing `easyexplore-0.7.3/test/test_anomaly_detector.py` & `easyexplore-0.7.4/test/test_anomaly_detector.py`

 * *Files identical despite different names*

### Comparing `easyexplore-0.7.3/test/test_data_explorer.py` & `easyexplore-0.7.4/test/test_data_explorer.py`

 * *Files identical despite different names*

### Comparing `easyexplore-0.7.3/test/test_data_import_export.py` & `easyexplore-0.7.4/test/test_data_import_export.py`

 * *Files identical despite different names*

### Comparing `easyexplore-0.7.3/test/test_data_visualizer.py` & `easyexplore-0.7.4/test/test_data_visualizer.py`

 * *Files identical despite different names*

### Comparing `easyexplore-0.7.3/test/test_interactive_visualizer.py` & `easyexplore-0.7.4/test/test_interactive_visualizer.py`

 * *Files identical despite different names*

### Comparing `easyexplore-0.7.3/test/test_unsupervised_machine_learning.py` & `easyexplore-0.7.4/test/test_unsupervised_machine_learning.py`

 * *Files identical despite different names*

### Comparing `easyexplore-0.7.3/test/test_utils.py` & `easyexplore-0.7.4/test/test_utils.py`

 * *Files identical despite different names*

