# Comparing `tmp/age_cda-0.0.3.tar.gz` & `tmp/age_cda-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "age_cda-0.0.3.tar", last modified: Sun Apr 16 08:20:36 2023, max compression
+gzip compressed data, was "age_cda-0.0.4.tar", last modified: Sun Apr 16 08:25:46 2023, max compression
```

## Comparing `age_cda-0.0.3.tar` & `age_cda-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:20:36.476528 age_cda-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-16 08:20:25.000000 age_cda-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-16 08:20:36.476528 age_cda-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-16 08:20:25.000000 age_cda-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:20:36.468528 age_cda-0.0.3/age_cda/
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-16 08:20:25.000000 age_cda-0.0.3/age_cda/Check.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-16 08:20:25.000000 age_cda-0.0.3/age_cda/Exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 08:20:25.000000 age_cda-0.0.3/age_cda/Graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-16 08:20:25.000000 age_cda-0.0.3/age_cda/Lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-16 08:20:25.000000 age_cda-0.0.3/age_cda/VERSION.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-16 08:20:25.000000 age_cda-0.0.3/age_cda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:20:36.468528 age_cda-0.0.3/age_cda/lib_ubuntu/
--rwxr-xr-x   0 runner    (1001) docker     (123)    17160 2023-04-16 08:20:25.000000 age_cda-0.0.3/age_cda/lib_ubuntu/library.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:20:36.468528 age_cda-0.0.3/age_cda/lib_windows/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:20:36.468528 age_cda-0.0.3/age_cda/lib_windows/x64/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:20:36.472528 age_cda-0.0.3/age_cda/lib_windows/x64/Release/
--rw-r--r--   0 runner    (1001) docker     (123)  2727424 2023-04-16 08:20:26.000000 age_cda-0.0.3/age_cda/lib_windows/x64/Release/gsl.dll
--rw-r--r--   0 runner    (1001) docker     (123)   422912 2023-04-16 08:20:26.000000 age_cda-0.0.3/age_cda/lib_windows/x64/Release/gslcblas.dll
--rw-r--r--   0 runner    (1001) docker     (123)    17408 2023-04-16 08:20:26.000000 age_cda-0.0.3/age_cda/lib_windows/x64/Release/lib_windows.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:20:36.468528 age_cda-0.0.3/age_cda/lib_windows/x86/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:20:36.476528 age_cda-0.0.3/age_cda/lib_windows/x86/Release/
--rw-r--r--   0 runner    (1001) docker     (123)  2125824 2023-04-16 08:20:26.000000 age_cda-0.0.3/age_cda/lib_windows/x86/Release/gsl.dll
--rw-r--r--   0 runner    (1001) docker     (123)   240640 2023-04-16 08:20:26.000000 age_cda-0.0.3/age_cda/lib_windows/x86/Release/gslcblas.dll
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-16 08:20:26.000000 age_cda-0.0.3/age_cda/lib_windows/x86/Release/lib_windows.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:20:36.468528 age_cda-0.0.3/age_cda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-16 08:20:36.000000 age_cda-0.0.3/age_cda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-16 08:20:36.000000 age_cda-0.0.3/age_cda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 08:20:36.000000 age_cda-0.0.3/age_cda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-16 08:20:36.000000 age_cda-0.0.3/age_cda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 08:20:36.476528 age_cda-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-16 08:20:26.000000 age_cda-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:25:46.484860 age_cda-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-16 08:25:35.000000 age_cda-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-16 08:25:46.484860 age_cda-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-16 08:25:35.000000 age_cda-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:25:46.480860 age_cda-0.0.4/age_cda/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-16 08:25:35.000000 age_cda-0.0.4/age_cda/Check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-16 08:25:35.000000 age_cda-0.0.4/age_cda/Exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 08:25:35.000000 age_cda-0.0.4/age_cda/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-16 08:25:35.000000 age_cda-0.0.4/age_cda/Lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-16 08:25:35.000000 age_cda-0.0.4/age_cda/VERSION.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-16 08:25:35.000000 age_cda-0.0.4/age_cda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:25:46.480860 age_cda-0.0.4/age_cda/lib_ubuntu/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17160 2023-04-16 08:25:35.000000 age_cda-0.0.4/age_cda/lib_ubuntu/library.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:25:46.480860 age_cda-0.0.4/age_cda/lib_windows/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:25:46.480860 age_cda-0.0.4/age_cda/lib_windows/x64/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:25:46.484860 age_cda-0.0.4/age_cda/lib_windows/x64/Release/
+-rw-r--r--   0 runner    (1001) docker     (123)  2727424 2023-04-16 08:25:36.000000 age_cda-0.0.4/age_cda/lib_windows/x64/Release/gsl.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   422912 2023-04-16 08:25:36.000000 age_cda-0.0.4/age_cda/lib_windows/x64/Release/gslcblas.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    17408 2023-04-16 08:25:36.000000 age_cda-0.0.4/age_cda/lib_windows/x64/Release/lib_windows.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:25:46.480860 age_cda-0.0.4/age_cda/lib_windows/x86/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:25:46.484860 age_cda-0.0.4/age_cda/lib_windows/x86/Release/
+-rw-r--r--   0 runner    (1001) docker     (123)  2125824 2023-04-16 08:25:36.000000 age_cda-0.0.4/age_cda/lib_windows/x86/Release/gsl.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   240640 2023-04-16 08:25:36.000000 age_cda-0.0.4/age_cda/lib_windows/x86/Release/gslcblas.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-16 08:25:36.000000 age_cda-0.0.4/age_cda/lib_windows/x86/Release/lib_windows.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:25:46.480860 age_cda-0.0.4/age_cda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-16 08:25:46.000000 age_cda-0.0.4/age_cda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-16 08:25:46.000000 age_cda-0.0.4/age_cda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 08:25:46.000000 age_cda-0.0.4/age_cda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-16 08:25:46.000000 age_cda-0.0.4/age_cda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 08:25:46.484860 age_cda-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-16 08:25:36.000000 age_cda-0.0.4/setup.py
```

### Comparing `age_cda-0.0.3/LICENSE` & `age_cda-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.3/PKG-INFO` & `age_cda-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: age_cda
-Version: 0.0.3
+Version: 0.0.4
 Summary: Detection of Community by maximizing modularity
 Home-page: https://github.com/Munmud/Community-Detection-Modularity
 Author: Moontasir Mahmood
 Author-email: moontasir042@gmail.com
 License: Apache2.0
 Keywords: Community-Detection,Modularity,Reichardt and Bornholdt,Newman,partition network,k means cluster
 Classifier: Programming Language :: Python :: 3.9
@@ -24,25 +24,26 @@
 
 The basic idea is that nodes that belong to the same community will have similar eigenvector values for these dominant eigenvectors. By grouping nodes with similar eigenvector values together, communities can be identified.
 
 ## Installation
 
 ### Install via PIP
 ```cmd
-pip install apache-age-community-detection
+pip install age-cda
 ```
 
 ### Build from Source
 ```cmd
 sudo apt-get update
 sudo apt-get install libeigen3-dev
 git clone https://github.com/Munmud/Community-Detection-Modularity
 cd Community-Detection-Modularity
 python setup.py install
 ```
+- [Configure GSL - GNU Scientific Library](https://solarianprogrammer.com/2020/01/26/getting-started-gsl-gnu-scientific-library-windows-macos-linux/)
 
 ### Unit Test
 ```cmd
 python -m unittest test_community.py
 ```
 
 ## Instruction
```

### Comparing `age_cda-0.0.3/README.md` & `age_cda-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,25 +10,26 @@
 
 The basic idea is that nodes that belong to the same community will have similar eigenvector values for these dominant eigenvectors. By grouping nodes with similar eigenvector values together, communities can be identified.
 
 ## Installation
 
 ### Install via PIP
 ```cmd
-pip install apache-age-community-detection
+pip install age-cda
 ```
 
 ### Build from Source
 ```cmd
 sudo apt-get update
 sudo apt-get install libeigen3-dev
 git clone https://github.com/Munmud/Community-Detection-Modularity
 cd Community-Detection-Modularity
 python setup.py install
 ```
+- [Configure GSL - GNU Scientific Library](https://solarianprogrammer.com/2020/01/26/getting-started-gsl-gnu-scientific-library-windows-macos-linux/)
 
 ### Unit Test
 ```cmd
 python -m unittest test_community.py
 ```
 
 ## Instruction
```

### Comparing `age_cda-0.0.3/age_cda/Check.py` & `age_cda-0.0.4/age_cda/Check.py`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.3/age_cda/Exception.py` & `age_cda-0.0.4/age_cda/Exception.py`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.3/age_cda/Graph.py` & `age_cda-0.0.4/age_cda/Graph.py`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.3/age_cda/Lib.py` & `age_cda-0.0.4/age_cda/Lib.py`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.3/age_cda/lib_ubuntu/library.so` & `age_cda-0.0.4/age_cda/lib_ubuntu/library.so`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.3/age_cda/lib_windows/x64/Release/gsl.dll` & `age_cda-0.0.4/age_cda/lib_windows/x64/Release/gsl.dll`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.3/age_cda/lib_windows/x64/Release/gslcblas.dll` & `age_cda-0.0.4/age_cda/lib_windows/x64/Release/gslcblas.dll`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.3/age_cda/lib_windows/x64/Release/lib_windows.dll` & `age_cda-0.0.4/age_cda/lib_windows/x64/Release/lib_windows.dll`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.3/age_cda/lib_windows/x86/Release/gsl.dll` & `age_cda-0.0.4/age_cda/lib_windows/x86/Release/gsl.dll`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.3/age_cda/lib_windows/x86/Release/gslcblas.dll` & `age_cda-0.0.4/age_cda/lib_windows/x86/Release/gslcblas.dll`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.3/age_cda/lib_windows/x86/Release/lib_windows.dll` & `age_cda-0.0.4/age_cda/lib_windows/x86/Release/lib_windows.dll`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.3/age_cda.egg-info/PKG-INFO` & `age_cda-0.0.4/age_cda.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: age-cda
-Version: 0.0.3
+Version: 0.0.4
 Summary: Detection of Community by maximizing modularity
 Home-page: https://github.com/Munmud/Community-Detection-Modularity
 Author: Moontasir Mahmood
 Author-email: moontasir042@gmail.com
 License: Apache2.0
 Keywords: Community-Detection,Modularity,Reichardt and Bornholdt,Newman,partition network,k means cluster
 Classifier: Programming Language :: Python :: 3.9
@@ -24,25 +24,26 @@
 
 The basic idea is that nodes that belong to the same community will have similar eigenvector values for these dominant eigenvectors. By grouping nodes with similar eigenvector values together, communities can be identified.
 
 ## Installation
 
 ### Install via PIP
 ```cmd
-pip install apache-age-community-detection
+pip install age-cda
 ```
 
 ### Build from Source
 ```cmd
 sudo apt-get update
 sudo apt-get install libeigen3-dev
 git clone https://github.com/Munmud/Community-Detection-Modularity
 cd Community-Detection-Modularity
 python setup.py install
 ```
+- [Configure GSL - GNU Scientific Library](https://solarianprogrammer.com/2020/01/26/getting-started-gsl-gnu-scientific-library-windows-macos-linux/)
 
 ### Unit Test
 ```cmd
 python -m unittest test_community.py
 ```
 
 ## Instruction
```

### Comparing `age_cda-0.0.3/age_cda.egg-info/SOURCES.txt` & `age_cda-0.0.4/age_cda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `age_cda-0.0.3/setup.py` & `age_cda-0.0.4/setup.py`

 * *Files identical despite different names*

