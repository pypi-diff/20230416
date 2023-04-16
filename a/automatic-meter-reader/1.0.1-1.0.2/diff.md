# Comparing `tmp/automatic-meter-reader-1.0.1.tar.gz` & `tmp/automatic-meter-reader-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automatic-meter-reader-1.0.1.tar", last modified: Sat Feb  4 17:53:02 2023, max compression
+gzip compressed data, was "automatic-meter-reader-1.0.2.tar", last modified: Sun Apr 16 11:35:11 2023, max compression
```

## Comparing `automatic-meter-reader-1.0.1.tar` & `automatic-meter-reader-1.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 17:53:02.485505 automatic-meter-reader-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-02-04 17:53:02.485505 automatic-meter-reader-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 17:53:02.481505 automatic-meter-reader-1.0.1/automatic_meter_reader/
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/automatic_meter_reader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 17:53:02.485505 automatic-meter-reader-1.0.1/automatic_meter_reader/cameras/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/automatic_meter_reader/cameras/espcam_120_deg.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 17:53:02.481505 automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 17:53:02.485505 automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/gas_bk25/
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/gas_bk25/meter_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/gas_bk25/template_0.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/gas_bk25/template_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/gas_bk25/template_2.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 17:53:02.485505 automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/lorenz_1997/
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/lorenz_1997/meter_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/lorenz_1997/template_0.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/lorenz_1997/template_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/lorenz_1997/template_2.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 17:53:02.485505 automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/wehrle_cold/
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/wehrle_cold/meter_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/wehrle_cold/template_0.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/wehrle_cold/template_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/wehrle_cold/template_2.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 17:53:02.485505 automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/wehrle_hot/
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/wehrle_hot/meter_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/wehrle_hot/template_0.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/wehrle_hot/template_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/wehrle_hot/template_2.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 17:53:02.485505 automatic-meter-reader-1.0.1/automatic_meter_reader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-02-04 17:53:02.000000 automatic-meter-reader-1.0.1/automatic_meter_reader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-02-04 17:53:02.000000 automatic-meter-reader-1.0.1/automatic_meter_reader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-04 17:53:02.000000 automatic-meter-reader-1.0.1/automatic_meter_reader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-04 17:53:02.000000 automatic-meter-reader-1.0.1/automatic_meter_reader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-04 17:53:02.000000 automatic-meter-reader-1.0.1/automatic_meter_reader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-04 17:53:02.489505 automatic-meter-reader-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 17:53:02.485505 automatic-meter-reader-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    40523 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/tests/test_image.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    34548 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/tests/test_image2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-02-04 17:51:10.000000 automatic-meter-reader-1.0.1/tests/test_readout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:35:11.010325 automatic-meter-reader-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-16 11:35:11.010325 automatic-meter-reader-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:35:11.006325 automatic-meter-reader-1.0.2/automatic_meter_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/automatic_meter_reader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:35:11.010325 automatic-meter-reader-1.0.2/automatic_meter_reader/cameras/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/automatic_meter_reader/cameras/espcam_120_deg.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:35:11.006325 automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:35:11.010325 automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/gas_bk25/
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/gas_bk25/meter_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/gas_bk25/template_0.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/gas_bk25/template_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/gas_bk25/template_2.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:35:11.010325 automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/lorenz_1997/
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/lorenz_1997/meter_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/lorenz_1997/template_0.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/lorenz_1997/template_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/lorenz_1997/template_2.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:35:11.010325 automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/wehrle_cold/
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/wehrle_cold/meter_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/wehrle_cold/template_0.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/wehrle_cold/template_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/wehrle_cold/template_2.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:35:11.010325 automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/wehrle_hot/
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/wehrle_hot/meter_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/wehrle_hot/template_0.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/wehrle_hot/template_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/wehrle_hot/template_2.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:35:11.010325 automatic-meter-reader-1.0.2/automatic_meter_reader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-16 11:35:10.000000 automatic-meter-reader-1.0.2/automatic_meter_reader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-16 11:35:11.000000 automatic-meter-reader-1.0.2/automatic_meter_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 11:35:10.000000 automatic-meter-reader-1.0.2/automatic_meter_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-16 11:35:10.000000 automatic-meter-reader-1.0.2/automatic_meter_reader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-16 11:35:10.000000 automatic-meter-reader-1.0.2/automatic_meter_reader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 11:35:11.010325 automatic-meter-reader-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:35:11.010325 automatic-meter-reader-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    40523 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/tests/test_image.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    34548 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/tests/test_image2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-16 11:34:40.000000 automatic-meter-reader-1.0.2/tests/test_readout.py
```

### Comparing `automatic-meter-reader-1.0.1/automatic_meter_reader/__init__.py` & `automatic-meter-reader-1.0.2/automatic_meter_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.1/automatic_meter_reader/cameras/espcam_120_deg.json` & `automatic-meter-reader-1.0.2/automatic_meter_reader/cameras/espcam_120_deg.json`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/gas_bk25/meter_config.json` & `automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/gas_bk25/meter_config.json`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/gas_bk25/template_0.jpg` & `automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/gas_bk25/template_0.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/gas_bk25/template_1.jpg` & `automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/gas_bk25/template_1.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/gas_bk25/template_2.jpg` & `automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/gas_bk25/template_2.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/lorenz_1997/meter_config.json` & `automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/lorenz_1997/meter_config.json`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/lorenz_1997/template_0.jpg` & `automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/lorenz_1997/template_0.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/lorenz_1997/template_1.jpg` & `automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/lorenz_1997/template_1.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/lorenz_1997/template_2.jpg` & `automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/lorenz_1997/template_2.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/wehrle_cold/meter_config.json` & `automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/wehrle_cold/meter_config.json`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/wehrle_cold/template_0.jpg` & `automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/wehrle_cold/template_0.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/wehrle_cold/template_1.jpg` & `automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/wehrle_cold/template_1.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/wehrle_cold/template_2.jpg` & `automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/wehrle_cold/template_2.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/wehrle_hot/meter_config.json` & `automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/wehrle_hot/meter_config.json`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/wehrle_hot/template_0.jpg` & `automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/wehrle_hot/template_0.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/wehrle_hot/template_1.jpg` & `automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/wehrle_hot/template_1.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.1/automatic_meter_reader/meter_models/wehrle_hot/template_2.jpg` & `automatic-meter-reader-1.0.2/automatic_meter_reader/meter_models/wehrle_hot/template_2.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.1/automatic_meter_reader.egg-info/SOURCES.txt` & `automatic-meter-reader-1.0.2/automatic_meter_reader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.1/dev-requirements.txt` & `automatic-meter-reader-1.0.2/dev-requirements.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,197 +1,167 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --extra=dev --output-file=dev-requirements.txt
 #
 asttokens==2.2.1
     # via stack-data
-attrs==22.2.0
-    # via pytest
 backcall==0.2.0
     # via ipython
 build==0.10.0
     # via pip-tools
-certifi==2022.12.7
-    # via requests
-charset-normalizer==3.0.1
-    # via requests
 click==8.1.3
     # via pip-tools
 colorama==0.4.6
     # via
     #   build
     #   click
     #   ipython
     #   pytest
-comm==0.1.2
+comm==0.1.3
     # via ipykernel
 contourpy==1.0.7
     # via matplotlib
 cycler==0.11.0
     # via matplotlib
-debugpy==1.6.6
+debugpy==1.6.7
     # via ipykernel
 decorator==5.1.1
     # via ipython
-exceptiongroup==1.1.0
-    # via pytest
 executing==1.2.0
     # via stack-data
 flake8==6.0.0
     # via automatic-meter-reader (setup.py)
-fonttools==4.38.0
+fonttools==4.39.3
     # via matplotlib
-idna==3.4
-    # via requests
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.21.1
+ipykernel==6.22.0
     # via
     #   automatic-meter-reader (setup.py)
     #   ipywidgets
-ipympl==0.9.2
+ipympl==0.9.3
     # via automatic-meter-reader (setup.py)
-ipython==8.9.0
+ipython==8.12.0
     # via
     #   ipykernel
     #   ipympl
     #   ipywidgets
 ipython-genutils==0.2.0
     # via ipympl
-ipywidgets==8.0.4
+ipywidgets==8.0.6
     # via ipympl
 jedi==0.18.2
     # via ipython
-jupyter-client==8.0.2
+jupyter-client==8.2.0
     # via ipykernel
-jupyter-core==5.2.0
+jupyter-core==5.3.0
     # via
     #   ipykernel
     #   jupyter-client
-jupyterlab-widgets==3.0.5
+jupyterlab-widgets==3.0.7
     # via ipywidgets
 kiwisolver==1.4.4
     # via matplotlib
-matplotlib==3.6.3
+matplotlib==3.7.1
     # via
     #   automatic-meter-reader (setup.py)
     #   ipympl
 matplotlib-inline==0.1.6
     # via
     #   ipykernel
     #   ipython
 mccabe==0.7.0
     # via flake8
-meter-digits-recognizer==0.1.9
+meter-digits-recognizer==0.1.11
     # via automatic-meter-reader (setup.py)
 nest-asyncio==1.5.6
     # via ipykernel
-numpy==1.24.1
+numpy==1.24.2
     # via
     #   automatic-meter-reader (setup.py)
     #   contourpy
     #   ipympl
     #   matplotlib
     #   meter-digits-recognizer
     #   opencv-python
-    #   torchvision
-opencv-python==4.7.0.68
+opencv-python==4.7.0.72
     # via
     #   automatic-meter-reader (setup.py)
     #   meter-digits-recognizer
-packaging==23.0
+packaging==23.1
     # via
     #   build
     #   ipykernel
     #   matplotlib
     #   pytest
 parso==0.8.3
     # via jedi
 pickleshare==0.7.5
     # via ipython
-pillow==9.4.0
+pillow==9.5.0
     # via
     #   ipympl
     #   matplotlib
-    #   meter-digits-recognizer
-    #   torchvision
-pip-tools==6.12.2
+pip-tools==6.13.0
     # via automatic-meter-reader (setup.py)
-platformdirs==2.6.2
+platformdirs==3.2.0
     # via jupyter-core
 pluggy==1.0.0
     # via pytest
-prompt-toolkit==3.0.36
+prompt-toolkit==3.0.38
     # via ipython
 psutil==5.9.4
     # via ipykernel
 pure-eval==0.2.2
     # via stack-data
 pycodestyle==2.10.0
     # via flake8
 pyflakes==3.0.1
     # via flake8
-pygments==2.14.0
+pygments==2.15.0
     # via ipython
 pyparsing==3.0.9
     # via matplotlib
 pyproject-hooks==1.0.0
     # via build
-pytest==7.2.1
+pytest==7.3.1
     # via automatic-meter-reader (setup.py)
 python-dateutil==2.8.2
     # via
     #   jupyter-client
     #   matplotlib
-pyzmq==25.0.0
+pywin32==306
+    # via jupyter-core
+pyzmq==25.0.2
     # via
     #   ipykernel
     #   jupyter-client
-requests==2.28.2
-    # via torchvision
 six==1.16.0
     # via python-dateutil
 stack-data==0.6.2
     # via ipython
-tomli==2.0.1
-    # via
-    #   build
-    #   pyproject-hooks
-    #   pytest
-torch==1.13.1
-    # via
-    #   meter-digits-recognizer
-    #   torchvision
-torchvision==0.14.1
-    # via meter-digits-recognizer
 tornado==6.2
     # via
     #   ipykernel
     #   jupyter-client
 traitlets==5.9.0
     # via
     #   comm
     #   ipykernel
     #   ipympl
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
-typing-extensions==4.4.0
-    # via
-    #   torch
-    #   torchvision
-urllib3==1.26.14
-    # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
-wheel==0.38.4
+wheel==0.40.0
     # via pip-tools
-widgetsnbextension==4.0.5
+widgetsnbextension==4.0.7
     # via ipywidgets
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `automatic-meter-reader-1.0.1/pyproject.toml` & `automatic-meter-reader-1.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "numpy",
     "opencv-python",
-    "meter-digits-recognizer",
+    "meter-digits-recognizer>=0.1.11",
 ]
 dynamic = ["version"]
 
 [project.urls]
 repository = "https://github.com/ardiloot/automatic-meter-reader"
 
 [project.optional-dependencies]
```

### Comparing `automatic-meter-reader-1.0.1/tests/test_image.jpg` & `automatic-meter-reader-1.0.2/tests/test_image.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.1/tests/test_image2.jpg` & `automatic-meter-reader-1.0.2/tests/test_image2.jpg`

 * *Files identical despite different names*

