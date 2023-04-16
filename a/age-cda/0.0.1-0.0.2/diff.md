# Comparing `tmp/age_cda-0.0.1.tar.gz` & `tmp/age_cda-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "age_cda-0.0.1.tar", last modified: Sun Apr 16 07:08:37 2023, max compression
+gzip compressed data, was "age_cda-0.0.2.tar", last modified: Sun Apr 16 07:21:19 2023, max compression
```

## Comparing `age_cda-0.0.1.tar` & `age_cda-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:08:37.633049 age_cda-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-16 07:08:22.000000 age_cda-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-16 07:08:37.633049 age_cda-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-16 07:08:22.000000 age_cda-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:08:37.625049 age_cda-0.0.1/age_cda/
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-16 07:08:22.000000 age_cda-0.0.1/age_cda/Check.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-16 07:08:22.000000 age_cda-0.0.1/age_cda/Exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 07:08:22.000000 age_cda-0.0.1/age_cda/Graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-16 07:08:22.000000 age_cda-0.0.1/age_cda/Lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-16 07:08:22.000000 age_cda-0.0.1/age_cda/VERSION.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-16 07:08:22.000000 age_cda-0.0.1/age_cda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:08:37.621049 age_cda-0.0.1/age_cda/lib_windows/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:08:37.621049 age_cda-0.0.1/age_cda/lib_windows/x64/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:08:37.629049 age_cda-0.0.1/age_cda/lib_windows/x64/Release/
--rw-r--r--   0 runner    (1001) docker     (123)  2727424 2023-04-16 07:08:22.000000 age_cda-0.0.1/age_cda/lib_windows/x64/Release/gsl.dll
--rw-r--r--   0 runner    (1001) docker     (123)   422912 2023-04-16 07:08:22.000000 age_cda-0.0.1/age_cda/lib_windows/x64/Release/gslcblas.dll
--rw-r--r--   0 runner    (1001) docker     (123)    17408 2023-04-16 07:08:22.000000 age_cda-0.0.1/age_cda/lib_windows/x64/Release/lib_windows.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:08:37.621049 age_cda-0.0.1/age_cda/lib_windows/x86/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:08:37.633049 age_cda-0.0.1/age_cda/lib_windows/x86/Release/
--rw-r--r--   0 runner    (1001) docker     (123)  2125824 2023-04-16 07:08:23.000000 age_cda-0.0.1/age_cda/lib_windows/x86/Release/gsl.dll
--rw-r--r--   0 runner    (1001) docker     (123)   240640 2023-04-16 07:08:23.000000 age_cda-0.0.1/age_cda/lib_windows/x86/Release/gslcblas.dll
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-16 07:08:23.000000 age_cda-0.0.1/age_cda/lib_windows/x86/Release/lib_windows.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:08:37.625049 age_cda-0.0.1/age_cda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-16 07:08:37.000000 age_cda-0.0.1/age_cda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-16 07:08:37.000000 age_cda-0.0.1/age_cda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 07:08:37.000000 age_cda-0.0.1/age_cda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-16 07:08:37.000000 age_cda-0.0.1/age_cda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 07:08:37.633049 age_cda-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-16 07:08:23.000000 age_cda-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:21:19.985695 age_cda-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-16 07:21:09.000000 age_cda-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-16 07:21:19.985695 age_cda-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-16 07:21:09.000000 age_cda-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:21:19.977695 age_cda-0.0.2/age_cda/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-16 07:21:09.000000 age_cda-0.0.2/age_cda/Check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-16 07:21:09.000000 age_cda-0.0.2/age_cda/Exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 07:21:09.000000 age_cda-0.0.2/age_cda/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-16 07:21:09.000000 age_cda-0.0.2/age_cda/Lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-16 07:21:09.000000 age_cda-0.0.2/age_cda/VERSION.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-16 07:21:09.000000 age_cda-0.0.2/age_cda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:21:19.977695 age_cda-0.0.2/age_cda/lib_windows/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:21:19.977695 age_cda-0.0.2/age_cda/lib_windows/x64/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:21:19.981695 age_cda-0.0.2/age_cda/lib_windows/x64/Release/
+-rw-r--r--   0 runner    (1001) docker     (123)  2727424 2023-04-16 07:21:10.000000 age_cda-0.0.2/age_cda/lib_windows/x64/Release/gsl.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   422912 2023-04-16 07:21:10.000000 age_cda-0.0.2/age_cda/lib_windows/x64/Release/gslcblas.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    17408 2023-04-16 07:21:10.000000 age_cda-0.0.2/age_cda/lib_windows/x64/Release/lib_windows.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:21:19.977695 age_cda-0.0.2/age_cda/lib_windows/x86/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:21:19.985695 age_cda-0.0.2/age_cda/lib_windows/x86/Release/
+-rw-r--r--   0 runner    (1001) docker     (123)  2125824 2023-04-16 07:21:10.000000 age_cda-0.0.2/age_cda/lib_windows/x86/Release/gsl.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   240640 2023-04-16 07:21:10.000000 age_cda-0.0.2/age_cda/lib_windows/x86/Release/gslcblas.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-16 07:21:10.000000 age_cda-0.0.2/age_cda/lib_windows/x86/Release/lib_windows.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:21:19.977695 age_cda-0.0.2/age_cda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-16 07:21:19.000000 age_cda-0.0.2/age_cda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-16 07:21:19.000000 age_cda-0.0.2/age_cda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 07:21:19.000000 age_cda-0.0.2/age_cda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-16 07:21:19.000000 age_cda-0.0.2/age_cda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 07:21:19.985695 age_cda-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-16 07:21:10.000000 age_cda-0.0.2/setup.py
```

### Comparing `age_cda-0.0.1/LICENSE` & `age_cda-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.1/PKG-INFO` & `age_cda-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: age_cda
-Version: 0.0.1
+Version: 0.0.2
 Summary: Detection of Community by maximizing modularity
 Home-page: https://github.com/Munmud/Community-Detection-Modularity
 Author: Moontasir Mahmood
 Author-email: moontasir042@gmail.com
 License: Apache2.0
 Keywords: Community-Detection,Modularity,Reichardt and Bornholdt,Newman,partition network,k means cluster
 Classifier: Programming Language :: Python :: 3.9
@@ -45,15 +45,15 @@
 python -m unittest test_community.py
 ```
 
 ## Instruction
 
 ### import
 ```py
-from age_community_detection import Graph
+from age_cda import Graph
 ```
 
 ### Create Graph
 ```py
 nodes = [0, 1, 2, 3, 4, 5]
 edges = [[0, 1], [0, 2], [1, 2], [2, 3], [3, 4], [3, 5], [4, 5]]
 g = Graph.Graph()
```

### Comparing `age_cda-0.0.1/README.md` & `age_cda-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 python -m unittest test_community.py
 ```
 
 ## Instruction
 
 ### import
 ```py
-from age_community_detection import Graph
+from age_cda import Graph
 ```
 
 ### Create Graph
 ```py
 nodes = [0, 1, 2, 3, 4, 5]
 edges = [[0, 1], [0, 2], [1, 2], [2, 3], [3, 4], [3, 5], [4, 5]]
 g = Graph.Graph()
```

### Comparing `age_cda-0.0.1/age_cda/Check.py` & `age_cda-0.0.2/age_cda/Check.py`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.1/age_cda/Exception.py` & `age_cda-0.0.2/age_cda/Exception.py`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.1/age_cda/Graph.py` & `age_cda-0.0.2/age_cda/Graph.py`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.1/age_cda/Lib.py` & `age_cda-0.0.2/age_cda/Lib.py`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.1/age_cda/lib_windows/x64/Release/gsl.dll` & `age_cda-0.0.2/age_cda/lib_windows/x64/Release/gsl.dll`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.1/age_cda/lib_windows/x64/Release/gslcblas.dll` & `age_cda-0.0.2/age_cda/lib_windows/x64/Release/gslcblas.dll`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.1/age_cda/lib_windows/x64/Release/lib_windows.dll` & `age_cda-0.0.2/age_cda/lib_windows/x64/Release/lib_windows.dll`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.1/age_cda/lib_windows/x86/Release/gsl.dll` & `age_cda-0.0.2/age_cda/lib_windows/x86/Release/gsl.dll`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.1/age_cda/lib_windows/x86/Release/gslcblas.dll` & `age_cda-0.0.2/age_cda/lib_windows/x86/Release/gslcblas.dll`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.1/age_cda/lib_windows/x86/Release/lib_windows.dll` & `age_cda-0.0.2/age_cda/lib_windows/x86/Release/lib_windows.dll`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.1/age_cda.egg-info/PKG-INFO` & `age_cda-0.0.2/age_cda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: age-cda
-Version: 0.0.1
+Version: 0.0.2
 Summary: Detection of Community by maximizing modularity
 Home-page: https://github.com/Munmud/Community-Detection-Modularity
 Author: Moontasir Mahmood
 Author-email: moontasir042@gmail.com
 License: Apache2.0
 Keywords: Community-Detection,Modularity,Reichardt and Bornholdt,Newman,partition network,k means cluster
 Classifier: Programming Language :: Python :: 3.9
@@ -45,15 +45,15 @@
 python -m unittest test_community.py
 ```
 
 ## Instruction
 
 ### import
 ```py
-from age_community_detection import Graph
+from age_cda import Graph
 ```
 
 ### Create Graph
 ```py
 nodes = [0, 1, 2, 3, 4, 5]
 edges = [[0, 1], [0, 2], [1, 2], [2, 3], [3, 4], [3, 5], [4, 5]]
 g = Graph.Graph()
```

### Comparing `age_cda-0.0.1/age_cda.egg-info/SOURCES.txt` & `age_cda-0.0.2/age_cda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.1/setup.py` & `age_cda-0.0.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,14 +12,28 @@
     long_description_content_type="text/markdown",
     author           = 'Moontasir Mahmood',
     author_email     = 'moontasir042@gmail.com',
     url              = 'https://github.com/Munmud/Community-Detection-Modularity',
     license          = 'Apache2.0',
     install_requires = [],
     packages         = ['age_cda'],
-    package_data={'age_cda': ['lib_ubuntu/*.so', 'lib_windows/x64/Release/*.dll', 'lib_windows/x86/Release/*.dll']},
-    keywords         = ['Community-Detection', 'Modularity', 'Reichardt and Bornholdt','Newman', 'partition network', 'k means cluster'],
+    package_data     = {
+        'age_cda': 
+                    [   
+                        'lib_ubuntu/*.so', 
+                        'lib_windows/x64/Release/*.dll', 
+                        'lib_windows/x86/Release/*.dll'
+                    ]
+    },
+    keywords         = [
+        'Community-Detection', 
+        'Modularity', 
+        'Reichardt and Bornholdt',
+        'Newman', 
+        'partition network', 
+        'k means cluster'
+    ],
     python_requires  = '>=3.9',
     classifiers      = [
         'Programming Language :: Python :: 3.9'
     ]
 )
```

