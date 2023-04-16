# Comparing `tmp/tahoma-2.2.3.tar.gz` & `tmp/tahoma-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tahoma-2.2.3.tar", last modified: Wed Apr  5 16:52:00 2023, max compression
+gzip compressed data, was "tahoma-2.2.4.tar", last modified: Sun Apr 16 07:56:23 2023, max compression
```

## Comparing `tahoma-2.2.3.tar` & `tahoma-2.2.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-04-05 16:52:00.506413 tahoma-2.2.3/
--rwxrwx---   0 neptune   (1000) neptune   (1000)     1070 2023-02-18 00:22:37.000000 tahoma-2.2.3/LICENSE
--rwxrwx---   0 neptune   (1000) neptune   (1000)      142 2023-02-21 14:35:21.000000 tahoma-2.2.3/MANIFEST.in
--rwxrwx---   0 neptune   (1000) neptune   (1000)     6133 2023-04-05 16:52:00.506898 tahoma-2.2.3/PKG-INFO
--rwxrwx---   0 neptune   (1000) neptune   (1000)     5471 2023-04-05 16:49:55.000000 tahoma-2.2.3/PYPI_README.md
--rwxrwx---   0 neptune   (1000) neptune   (1000)     5471 2023-04-05 16:50:21.000000 tahoma-2.2.3/README.md
--rwxrwx---   0 neptune   (1000) neptune   (1000)     1201 2023-02-21 21:29:00.000000 tahoma-2.2.3/pyproject.toml
--rwxrwx---   0 neptune   (1000) neptune   (1000)       41 2023-02-21 17:24:01.000000 tahoma-2.2.3/requirements.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       38 2023-04-05 16:52:00.508003 tahoma-2.2.3/setup.cfg
--rwxrwx---   0 neptune   (1000) neptune   (1000)      125 2023-02-15 20:31:23.000000 tahoma-2.2.3/setup.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-04-05 16:52:00.500725 tahoma-2.2.3/tahoma/
--rwxrwx---   0 neptune   (1000) neptune   (1000)      134 2023-02-21 18:24:33.000000 tahoma-2.2.3/tahoma/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)       22 2023-04-05 16:51:41.000000 tahoma-2.2.3/tahoma/__version__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)     5469 2023-04-05 15:40:09.000000 tahoma-2.2.3/tahoma/get_devices_url.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-04-05 16:52:00.504508 tahoma-2.2.3/tahoma/icons/
--rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.3/tahoma/icons/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)    21160 2023-02-15 08:39:56.000000 tahoma-2.2.3/tahoma/icons/connected_house.png
--rwxrwx---   0 neptune   (1000) neptune   (1000)    29722 2023-02-15 17:48:11.000000 tahoma-2.2.3/tahoma/icons/water heater.png
--rwxrwx---   0 neptune   (1000) neptune   (1000)      668 2023-02-21 09:02:06.000000 tahoma-2.2.3/tahoma/install_tahoma.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)    35274 2023-04-05 16:45:21.000000 tahoma-2.2.3/tahoma/tahoma.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-04-05 16:52:00.505006 tahoma-2.2.3/tahoma/temp/
--rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:32:54.000000 tahoma-2.2.3/tahoma/temp/__init__.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-04-05 16:52:00.505990 tahoma-2.2.3/tahoma/test/
--rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.3/tahoma/test/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2021-07-13 15:25:04.000000 tahoma-2.2.3/tahoma/test/test.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-04-05 16:52:00.503210 tahoma-2.2.3/tahoma.egg-info/
--rwxrwx---   0 neptune   (1000) neptune   (1000)     6133 2023-04-05 16:52:00.000000 tahoma-2.2.3/tahoma.egg-info/PKG-INFO
--rwxrwx---   0 neptune   (1000) neptune   (1000)      542 2023-04-05 16:52:00.000000 tahoma-2.2.3/tahoma.egg-info/SOURCES.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)        1 2023-04-05 16:52:00.000000 tahoma-2.2.3/tahoma.egg-info/dependency_links.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       46 2023-04-05 16:52:00.000000 tahoma-2.2.3/tahoma.egg-info/entry_points.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       41 2023-04-05 16:52:00.000000 tahoma-2.2.3/tahoma.egg-info/requires.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)        7 2023-04-05 16:52:00.000000 tahoma-2.2.3/tahoma.egg-info/top_level.txt
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-04-16 07:56:23.678277 tahoma-2.2.4/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     1070 2023-02-18 00:22:37.000000 tahoma-2.2.4/LICENSE
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      142 2023-02-21 14:35:21.000000 tahoma-2.2.4/MANIFEST.in
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     6133 2023-04-16 07:56:23.678441 tahoma-2.2.4/PKG-INFO
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     5471 2023-04-05 16:49:55.000000 tahoma-2.2.4/PYPI_README.md
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     5471 2023-04-05 16:50:21.000000 tahoma-2.2.4/README.md
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     1201 2023-02-21 21:29:00.000000 tahoma-2.2.4/pyproject.toml
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       41 2023-02-21 17:24:01.000000 tahoma-2.2.4/requirements.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       38 2023-04-16 07:56:23.678954 tahoma-2.2.4/setup.cfg
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      125 2023-02-15 20:31:23.000000 tahoma-2.2.4/setup.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-04-16 07:56:23.671422 tahoma-2.2.4/tahoma/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      134 2023-02-21 18:24:33.000000 tahoma-2.2.4/tahoma/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       22 2023-04-16 07:53:03.000000 tahoma-2.2.4/tahoma/__version__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     5469 2023-04-05 15:40:09.000000 tahoma-2.2.4/tahoma/get_devices_url.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-04-16 07:56:23.675872 tahoma-2.2.4/tahoma/icons/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.4/tahoma/icons/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    21160 2023-02-15 08:39:56.000000 tahoma-2.2.4/tahoma/icons/connected_house.png
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    29722 2023-02-15 17:48:11.000000 tahoma-2.2.4/tahoma/icons/water heater.png
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      668 2023-02-21 09:02:06.000000 tahoma-2.2.4/tahoma/install_tahoma.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    35274 2023-04-16 07:49:29.000000 tahoma-2.2.4/tahoma/tahoma.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-04-16 07:56:23.676628 tahoma-2.2.4/tahoma/temp/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:32:54.000000 tahoma-2.2.4/tahoma/temp/__init__.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-04-16 07:56:23.677883 tahoma-2.2.4/tahoma/test/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.4/tahoma/test/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2021-07-13 15:25:04.000000 tahoma-2.2.4/tahoma/test/test.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-04-16 07:56:23.674321 tahoma-2.2.4/tahoma.egg-info/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     6133 2023-04-16 07:56:23.000000 tahoma-2.2.4/tahoma.egg-info/PKG-INFO
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      542 2023-04-16 07:56:23.000000 tahoma-2.2.4/tahoma.egg-info/SOURCES.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        1 2023-04-16 07:56:23.000000 tahoma-2.2.4/tahoma.egg-info/dependency_links.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       46 2023-04-16 07:56:23.000000 tahoma-2.2.4/tahoma.egg-info/entry_points.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       41 2023-04-16 07:56:23.000000 tahoma-2.2.4/tahoma.egg-info/requires.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        7 2023-04-16 07:56:23.000000 tahoma-2.2.4/tahoma.egg-info/top_level.txt
```

### Comparing `tahoma-2.2.3/LICENSE` & `tahoma-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.3/PKG-INFO` & `tahoma-2.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahoma
-Version: 2.2.3
+Version: 2.2.4
 Summary: This is a very easy API for controlling Somfy Tahoma's devices written in Python3, thanks to the pyoverkiz API. You just need a three-word input to control a device
 Author-email: Pzim-devdata <contact@pzim.fr>
 Project-URL: Homepage, https://github.com/pzim-devdata/tahoma
 Project-URL: Bug Tracker, https://github.com/pzim-devdata/tahoma/issues
 Keywords: tahoma,somfy,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tahoma-2.2.3/PYPI_README.md` & `tahoma-2.2.4/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.3/README.md` & `tahoma-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.3/pyproject.toml` & `tahoma-2.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.3/tahoma/get_devices_url.py` & `tahoma-2.2.4/tahoma/get_devices_url.py`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.3/tahoma/icons/connected_house.png` & `tahoma-2.2.4/tahoma/icons/connected_house.png`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.3/tahoma/icons/water heater.png` & `tahoma-2.2.4/tahoma/icons/water heater.png`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.3/tahoma/install_tahoma.py` & `tahoma-2.2.4/tahoma/install_tahoma.py`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.3/tahoma/tahoma.py` & `tahoma-2.2.4/tahoma/tahoma.py`

 * *Files 0% similar despite different names*

```diff
@@ -526,23 +526,23 @@
             if len(url)== 0 :
                 print("There is no match. The <NAME> you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIQUE part of word from this results as <NAME> argument\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
                 exit()
             if len(url) > 1 :
                 print("There is more than one match. The <NAME> you gave is not exact. Choose a UNIQUE part of word from this results as <NAME> argument : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
                 exit()
 
-            if remove_accent(action).lower() == "comfort" or remove_accent(action).upper() == "confort" :
+            if remove_accent(action).lower() == "comfort" or remove_accent(action).lower() == "confort" :
                 fonction = Command(OverkizCommand.SET_HEATING_LEVEL,['comfort'])
-            elif remove_accent(action).lower() == 'comfort-1' or remove_accent(action).upper() == "confort-1" :
+            elif remove_accent(action).lower() == 'comfort-1' or remove_accent(action).lower() == "confort-1" :
                 fonction = Command(OverkizCommand.SET_HEATING_LEVEL,['comfort-1'])
-            elif remove_accent(action).lower() == 'comfort-2' or remove_accent(action).upper() == "confort-2" :
+            elif remove_accent(action).lower() == 'comfort-2' or remove_accent(action).lower() == "confort-2" :
                 fonction = Command(OverkizCommand.SET_HEATING_LEVEL,['comfort-2'])
             elif remove_accent(action).lower() == 'eco' :
                 fonction = Command(OverkizCommand.SET_HEATING_LEVEL,['eco'])
-            elif remove_accent(action).lower() == 'off' or remove_accent(action).upper() == "eteindre" :
+            elif remove_accent(action).lower() == 'off' or remove_accent(action).lower() == "eteindre" :
                 fonction = Command(OverkizCommand.SET_HEATING_LEVEL,['off'])
             else :
                 print( "\n'"+action+"'"+" is not a valide action.\n")
                 print("Please provide one of this argument as action : [comfort comfort-1 comfort-2 eco off]")
                 exit()
             str1 = " "
             print("Output action : "+remove_accent(action).lower()+" "+remove_accent(category)+" "+str1.join(good_name)+ " \nwith url : "+str1.join(url))
```

### Comparing `tahoma-2.2.3/tahoma.egg-info/PKG-INFO` & `tahoma-2.2.4/tahoma.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahoma
-Version: 2.2.3
+Version: 2.2.4
 Summary: This is a very easy API for controlling Somfy Tahoma's devices written in Python3, thanks to the pyoverkiz API. You just need a three-word input to control a device
 Author-email: Pzim-devdata <contact@pzim.fr>
 Project-URL: Homepage, https://github.com/pzim-devdata/tahoma
 Project-URL: Bug Tracker, https://github.com/pzim-devdata/tahoma/issues
 Keywords: tahoma,somfy,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tahoma-2.2.3/tahoma.egg-info/SOURCES.txt` & `tahoma-2.2.4/tahoma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

