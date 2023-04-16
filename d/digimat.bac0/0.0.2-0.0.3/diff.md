# Comparing `tmp/digimat.bac0-0.0.2.tar.gz` & `tmp/digimat.bac0-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digimat.bac0-0.0.2.tar", last modified: Sun Apr 16 10:30:59 2023, max compression
+gzip compressed data, was "digimat.bac0-0.0.3.tar", last modified: Sun Apr 16 10:41:01 2023, max compression
```

## Comparing `digimat.bac0-0.0.2.tar` & `digimat.bac0-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-16 10:30:59.400419 digimat.bac0-0.0.2/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-16 10:30:59.400153 digimat.bac0-0.0.2/PKG-INFO
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       38 2023-04-16 10:30:59.400515 digimat.bac0-0.0.2/setup.cfg
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      958 2023-04-16 09:32:27.000000 digimat.bac0-0.0.2/setup.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-16 10:30:59.397030 digimat.bac0-0.0.2/src/
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-16 10:30:59.397562 digimat.bac0-0.0.2/src/digimat/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       57 2014-09-24 08:13:04.000000 digimat.bac0-0.0.2/src/digimat/__init__.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-16 10:30:59.399812 digimat.bac0-0.0.2/src/digimat/bac0/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       25 2023-04-15 20:24:12.000000 digimat.bac0-0.0.2/src/digimat/bac0/__init__.py
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     8245 2023-04-16 10:27:22.000000 digimat.bac0-0.0.2/src/digimat/bac0/bacnet.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-16 10:30:59.399323 digimat.bac0-0.0.2/src/digimat.bac0.egg-info/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-16 10:30:59.000000 digimat.bac0-0.0.2/src/digimat.bac0.egg-info/PKG-INFO
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      375 2023-04-16 10:30:59.000000 digimat.bac0-0.0.2/src/digimat.bac0.egg-info/SOURCES.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-16 10:30:59.000000 digimat.bac0-0.0.2/src/digimat.bac0.egg-info/dependency_links.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-16 10:30:59.000000 digimat.bac0-0.0.2/src/digimat.bac0.egg-info/namespace_packages.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-15 16:54:48.000000 digimat.bac0-0.0.2/src/digimat.bac0.egg-info/not-zip-safe
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       28 2023-04-16 10:30:59.000000 digimat.bac0-0.0.2/src/digimat.bac0.egg-info/requires.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-16 10:30:59.000000 digimat.bac0-0.0.2/src/digimat.bac0.egg-info/top_level.txt
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-16 10:41:01.780372 digimat.bac0-0.0.3/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-16 10:41:01.780089 digimat.bac0-0.0.3/PKG-INFO
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       38 2023-04-16 10:41:01.780471 digimat.bac0-0.0.3/setup.cfg
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      958 2023-04-16 10:40:57.000000 digimat.bac0-0.0.3/setup.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-16 10:41:01.776996 digimat.bac0-0.0.3/src/
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-16 10:41:01.777526 digimat.bac0-0.0.3/src/digimat/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       57 2014-09-24 08:13:04.000000 digimat.bac0-0.0.3/src/digimat/__init__.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-16 10:41:01.779708 digimat.bac0-0.0.3/src/digimat/bac0/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       25 2023-04-15 20:24:12.000000 digimat.bac0-0.0.3/src/digimat/bac0/__init__.py
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     8287 2023-04-16 10:39:38.000000 digimat.bac0-0.0.3/src/digimat/bac0/bacnet.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-16 10:41:01.779227 digimat.bac0-0.0.3/src/digimat.bac0.egg-info/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-16 10:41:01.000000 digimat.bac0-0.0.3/src/digimat.bac0.egg-info/PKG-INFO
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      375 2023-04-16 10:41:01.000000 digimat.bac0-0.0.3/src/digimat.bac0.egg-info/SOURCES.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-16 10:41:01.000000 digimat.bac0-0.0.3/src/digimat.bac0.egg-info/dependency_links.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-16 10:41:01.000000 digimat.bac0-0.0.3/src/digimat.bac0.egg-info/namespace_packages.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-15 16:54:48.000000 digimat.bac0-0.0.3/src/digimat.bac0.egg-info/not-zip-safe
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       28 2023-04-16 10:41:01.000000 digimat.bac0-0.0.3/src/digimat.bac0.egg-info/requires.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-16 10:41:01.000000 digimat.bac0-0.0.3/src/digimat.bac0.egg-info/top_level.txt
```

### Comparing `digimat.bac0-0.0.2/setup.py` & `digimat.bac0-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='digimat.bac0',
-    version='0.0.2',
+    version='0.0.3',
     description='Digimat BACnet BAC0 Wrapper',
     namespace_packages=['digimat'],
     author='Frederic Hess',
     author_email='fhess@st-sa.ch',
     url='http://www.digimat.ch',
     license='PSF',
     packages=find_packages('src'),
```

### Comparing `digimat.bac0-0.0.2/src/digimat/bac0/bacnet.py` & `digimat.bac0-0.0.3/src/digimat/bac0/bacnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,16 @@
         return len(self.points(key, objectType, outOfService))
 
     @functools.cache
     def points(self, key=None, objectType=None, outOfService=False):
         items=[]
         if key:
             key=key.lower()
+        if key=='*':
+            key=None
         for point in self._device.points:
             if not outOfService and point.bacnet_properties['outOfService']:
                 continue
             if objectType and objectType!=point.properties.type:
                 continue
             if key:
                 if key not in point.properties.name.lower() and \
```

