# Comparing `tmp/age_cda-0.0.2.tar.gz` & `tmp/age_cda-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "age_cda-0.0.2.tar", last modified: Sun Apr 16 07:21:19 2023, max compression
+gzip compressed data, was "age_cda-0.0.3.tar", last modified: Sun Apr 16 08:20:36 2023, max compression
```

## Comparing `age_cda-0.0.2.tar` & `age_cda-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:21:19.985695 age_cda-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-16 07:21:09.000000 age_cda-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-16 07:21:19.985695 age_cda-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-16 07:21:09.000000 age_cda-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:21:19.977695 age_cda-0.0.2/age_cda/
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-16 07:21:09.000000 age_cda-0.0.2/age_cda/Check.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-16 07:21:09.000000 age_cda-0.0.2/age_cda/Exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 07:21:09.000000 age_cda-0.0.2/age_cda/Graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-16 07:21:09.000000 age_cda-0.0.2/age_cda/Lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-16 07:21:09.000000 age_cda-0.0.2/age_cda/VERSION.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-16 07:21:09.000000 age_cda-0.0.2/age_cda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:21:19.977695 age_cda-0.0.2/age_cda/lib_windows/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:21:19.977695 age_cda-0.0.2/age_cda/lib_windows/x64/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:21:19.981695 age_cda-0.0.2/age_cda/lib_windows/x64/Release/
--rw-r--r--   0 runner    (1001) docker     (123)  2727424 2023-04-16 07:21:10.000000 age_cda-0.0.2/age_cda/lib_windows/x64/Release/gsl.dll
--rw-r--r--   0 runner    (1001) docker     (123)   422912 2023-04-16 07:21:10.000000 age_cda-0.0.2/age_cda/lib_windows/x64/Release/gslcblas.dll
--rw-r--r--   0 runner    (1001) docker     (123)    17408 2023-04-16 07:21:10.000000 age_cda-0.0.2/age_cda/lib_windows/x64/Release/lib_windows.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:21:19.977695 age_cda-0.0.2/age_cda/lib_windows/x86/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:21:19.985695 age_cda-0.0.2/age_cda/lib_windows/x86/Release/
--rw-r--r--   0 runner    (1001) docker     (123)  2125824 2023-04-16 07:21:10.000000 age_cda-0.0.2/age_cda/lib_windows/x86/Release/gsl.dll
--rw-r--r--   0 runner    (1001) docker     (123)   240640 2023-04-16 07:21:10.000000 age_cda-0.0.2/age_cda/lib_windows/x86/Release/gslcblas.dll
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-16 07:21:10.000000 age_cda-0.0.2/age_cda/lib_windows/x86/Release/lib_windows.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:21:19.977695 age_cda-0.0.2/age_cda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-16 07:21:19.000000 age_cda-0.0.2/age_cda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-16 07:21:19.000000 age_cda-0.0.2/age_cda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 07:21:19.000000 age_cda-0.0.2/age_cda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-16 07:21:19.000000 age_cda-0.0.2/age_cda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 07:21:19.985695 age_cda-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-16 07:21:10.000000 age_cda-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:20:36.476528 age_cda-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-16 08:20:25.000000 age_cda-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-16 08:20:36.476528 age_cda-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-16 08:20:25.000000 age_cda-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:20:36.468528 age_cda-0.0.3/age_cda/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-16 08:20:25.000000 age_cda-0.0.3/age_cda/Check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-16 08:20:25.000000 age_cda-0.0.3/age_cda/Exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 08:20:25.000000 age_cda-0.0.3/age_cda/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-16 08:20:25.000000 age_cda-0.0.3/age_cda/Lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-16 08:20:25.000000 age_cda-0.0.3/age_cda/VERSION.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-16 08:20:25.000000 age_cda-0.0.3/age_cda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:20:36.468528 age_cda-0.0.3/age_cda/lib_ubuntu/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17160 2023-04-16 08:20:25.000000 age_cda-0.0.3/age_cda/lib_ubuntu/library.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:20:36.468528 age_cda-0.0.3/age_cda/lib_windows/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:20:36.468528 age_cda-0.0.3/age_cda/lib_windows/x64/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:20:36.472528 age_cda-0.0.3/age_cda/lib_windows/x64/Release/
+-rw-r--r--   0 runner    (1001) docker     (123)  2727424 2023-04-16 08:20:26.000000 age_cda-0.0.3/age_cda/lib_windows/x64/Release/gsl.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   422912 2023-04-16 08:20:26.000000 age_cda-0.0.3/age_cda/lib_windows/x64/Release/gslcblas.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    17408 2023-04-16 08:20:26.000000 age_cda-0.0.3/age_cda/lib_windows/x64/Release/lib_windows.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:20:36.468528 age_cda-0.0.3/age_cda/lib_windows/x86/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:20:36.476528 age_cda-0.0.3/age_cda/lib_windows/x86/Release/
+-rw-r--r--   0 runner    (1001) docker     (123)  2125824 2023-04-16 08:20:26.000000 age_cda-0.0.3/age_cda/lib_windows/x86/Release/gsl.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   240640 2023-04-16 08:20:26.000000 age_cda-0.0.3/age_cda/lib_windows/x86/Release/gslcblas.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-16 08:20:26.000000 age_cda-0.0.3/age_cda/lib_windows/x86/Release/lib_windows.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:20:36.468528 age_cda-0.0.3/age_cda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-16 08:20:36.000000 age_cda-0.0.3/age_cda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-16 08:20:36.000000 age_cda-0.0.3/age_cda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 08:20:36.000000 age_cda-0.0.3/age_cda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-16 08:20:36.000000 age_cda-0.0.3/age_cda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 08:20:36.476528 age_cda-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-16 08:20:26.000000 age_cda-0.0.3/setup.py
```

### Comparing `age_cda-0.0.2/LICENSE` & `age_cda-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.2/PKG-INFO` & `age_cda-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: age_cda
-Version: 0.0.2
+Version: 0.0.3
 Summary: Detection of Community by maximizing modularity
 Home-page: https://github.com/Munmud/Community-Detection-Modularity
 Author: Moontasir Mahmood
 Author-email: moontasir042@gmail.com
 License: Apache2.0
 Keywords: Community-Detection,Modularity,Reichardt and Bornholdt,Newman,partition network,k means cluster
 Classifier: Programming Language :: Python :: 3.9
@@ -74,12 +74,13 @@
 [[3,4,5],[0,1,2]]
 ```
 - List community
 - Each community has list of nodes
 
 ### Samples
 - [Creating Graph](https://github.com/Munmud/Community-Detection-Modularity/blob/main/Samples/sample1.py)
+- [Zachary's karate club](https://github.com/Munmud/Community-Detection-Modularity/blob/main/Samples/sample2.py)
 
 ### Reference
 - [Finding community structure in networks using the eigenvectors of matrices](https://arxiv.org/pdf/physics/0605087.pdf)
 - [Modularity and community structure in networks](https://www.pnas.org/doi/10.1073/pnas.0601602103)
 - [Statistical Mechanics of Community Detection](https://ia903002.us.archive.org/33/items/arxiv-cond-mat0603718/cond-mat0603718.pdf)
```

### Comparing `age_cda-0.0.2/README.md` & `age_cda-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -60,12 +60,13 @@
 [[3,4,5],[0,1,2]]
 ```
 - List community
 - Each community has list of nodes
 
 ### Samples
 - [Creating Graph](https://github.com/Munmud/Community-Detection-Modularity/blob/main/Samples/sample1.py)
+- [Zachary's karate club](https://github.com/Munmud/Community-Detection-Modularity/blob/main/Samples/sample2.py)
 
 ### Reference
 - [Finding community structure in networks using the eigenvectors of matrices](https://arxiv.org/pdf/physics/0605087.pdf)
 - [Modularity and community structure in networks](https://www.pnas.org/doi/10.1073/pnas.0601602103)
 - [Statistical Mechanics of Community Detection](https://ia903002.us.archive.org/33/items/arxiv-cond-mat0603718/cond-mat0603718.pdf)
```

### Comparing `age_cda-0.0.2/age_cda/Check.py` & `age_cda-0.0.3/age_cda/Check.py`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.2/age_cda/Exception.py` & `age_cda-0.0.3/age_cda/Exception.py`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.2/age_cda/Graph.py` & `age_cda-0.0.3/age_cda/Graph.py`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.2/age_cda/Lib.py` & `age_cda-0.0.3/age_cda/Lib.py`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.2/age_cda/lib_windows/x64/Release/gsl.dll` & `age_cda-0.0.3/age_cda/lib_windows/x64/Release/gsl.dll`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.2/age_cda/lib_windows/x64/Release/gslcblas.dll` & `age_cda-0.0.3/age_cda/lib_windows/x64/Release/gslcblas.dll`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.2/age_cda/lib_windows/x64/Release/lib_windows.dll` & `age_cda-0.0.3/age_cda/lib_windows/x64/Release/lib_windows.dll`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.2/age_cda/lib_windows/x86/Release/gsl.dll` & `age_cda-0.0.3/age_cda/lib_windows/x86/Release/gsl.dll`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.2/age_cda/lib_windows/x86/Release/gslcblas.dll` & `age_cda-0.0.3/age_cda/lib_windows/x86/Release/gslcblas.dll`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.2/age_cda/lib_windows/x86/Release/lib_windows.dll` & `age_cda-0.0.3/age_cda/lib_windows/x86/Release/lib_windows.dll`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.2/age_cda.egg-info/PKG-INFO` & `age_cda-0.0.3/age_cda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: age-cda
-Version: 0.0.2
+Version: 0.0.3
 Summary: Detection of Community by maximizing modularity
 Home-page: https://github.com/Munmud/Community-Detection-Modularity
 Author: Moontasir Mahmood
 Author-email: moontasir042@gmail.com
 License: Apache2.0
 Keywords: Community-Detection,Modularity,Reichardt and Bornholdt,Newman,partition network,k means cluster
 Classifier: Programming Language :: Python :: 3.9
@@ -74,12 +74,13 @@
 [[3,4,5],[0,1,2]]
 ```
 - List community
 - Each community has list of nodes
 
 ### Samples
 - [Creating Graph](https://github.com/Munmud/Community-Detection-Modularity/blob/main/Samples/sample1.py)
+- [Zachary's karate club](https://github.com/Munmud/Community-Detection-Modularity/blob/main/Samples/sample2.py)
 
 ### Reference
 - [Finding community structure in networks using the eigenvectors of matrices](https://arxiv.org/pdf/physics/0605087.pdf)
 - [Modularity and community structure in networks](https://www.pnas.org/doi/10.1073/pnas.0601602103)
 - [Statistical Mechanics of Community Detection](https://ia903002.us.archive.org/33/items/arxiv-cond-mat0603718/cond-mat0603718.pdf)
```

### Comparing `age_cda-0.0.2/age_cda.egg-info/SOURCES.txt` & `age_cda-0.0.3/age_cda.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -7,13 +7,14 @@
 age_cda/Lib.py
 age_cda/VERSION.py
 age_cda/__init__.py
 age_cda.egg-info/PKG-INFO
 age_cda.egg-info/SOURCES.txt
 age_cda.egg-info/dependency_links.txt
 age_cda.egg-info/top_level.txt
+age_cda/lib_ubuntu/library.so
 age_cda/lib_windows/x64/Release/gsl.dll
 age_cda/lib_windows/x64/Release/gslcblas.dll
 age_cda/lib_windows/x64/Release/lib_windows.dll
 age_cda/lib_windows/x86/Release/gsl.dll
 age_cda/lib_windows/x86/Release/gslcblas.dll
 age_cda/lib_windows/x86/Release/lib_windows.dll
```

### Comparing `age_cda-0.0.2/setup.py` & `age_cda-0.0.3/setup.py`

 * *Files identical despite different names*

