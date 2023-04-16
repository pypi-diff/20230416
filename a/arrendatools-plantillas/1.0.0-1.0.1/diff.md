# Comparing `tmp/arrendatools_plantillas-1.0.0.tar.gz` & `tmp/arrendatools_plantillas-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrendatools_plantillas-1.0.0.tar", last modified: Sun Apr 16 10:13:15 2023, max compression
+gzip compressed data, was "arrendatools_plantillas-1.0.1.tar", last modified: Sun Apr 16 10:52:09 2023, max compression
```

## Comparing `arrendatools_plantillas-1.0.0.tar` & `arrendatools_plantillas-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 10:13:15.019917 arrendatools_plantillas-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-04-16 10:13:12.000000 arrendatools_plantillas-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      751 2023-04-16 10:13:15.019917 arrendatools_plantillas-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1100 2023-04-16 10:13:12.000000 arrendatools_plantillas-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 10:13:15.019917 arrendatools_plantillas-1.0.0/arrendatools_plantillas/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-16 10:13:12.000000 arrendatools_plantillas-1.0.0/arrendatools_plantillas/__init__.py
--rw-r--r--   0 root         (0) root         (0)      418 2023-04-16 10:13:12.000000 arrendatools_plantillas-1.0.0/arrendatools_plantillas/plantilla.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 10:13:15.019917 arrendatools_plantillas-1.0.0/arrendatools_plantillas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      751 2023-04-16 10:13:15.000000 arrendatools_plantillas-1.0.0/arrendatools_plantillas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      297 2023-04-16 10:13:15.000000 arrendatools_plantillas-1.0.0/arrendatools_plantillas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 10:13:15.000000 arrendatools_plantillas-1.0.0/arrendatools_plantillas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-16 10:13:15.000000 arrendatools_plantillas-1.0.0/arrendatools_plantillas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-04-16 10:13:15.019917 arrendatools_plantillas-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      872 2023-04-16 10:13:13.000000 arrendatools_plantillas-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 10:52:09.799722 arrendatools_plantillas-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-04-16 10:52:07.000000 arrendatools_plantillas-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      751 2023-04-16 10:52:09.799722 arrendatools_plantillas-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1100 2023-04-16 10:52:07.000000 arrendatools_plantillas-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 10:52:09.799722 arrendatools_plantillas-1.0.1/arrendatools_plantillas/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-16 10:52:07.000000 arrendatools_plantillas-1.0.1/arrendatools_plantillas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 10:52:09.799722 arrendatools_plantillas-1.0.1/arrendatools_plantillas/filters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-16 10:52:07.000000 arrendatools_plantillas-1.0.1/arrendatools_plantillas/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      753 2023-04-16 10:52:07.000000 arrendatools_plantillas-1.0.1/arrendatools_plantillas/filters/numero_a_palabras.py
+-rw-r--r--   0 root         (0) root         (0)      418 2023-04-16 10:52:07.000000 arrendatools_plantillas-1.0.1/arrendatools_plantillas/plantilla.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 10:52:09.799722 arrendatools_plantillas-1.0.1/arrendatools_plantillas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      751 2023-04-16 10:52:09.000000 arrendatools_plantillas-1.0.1/arrendatools_plantillas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      394 2023-04-16 10:52:09.000000 arrendatools_plantillas-1.0.1/arrendatools_plantillas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 10:52:09.000000 arrendatools_plantillas-1.0.1/arrendatools_plantillas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-16 10:52:09.000000 arrendatools_plantillas-1.0.1/arrendatools_plantillas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-04-16 10:52:09.799722 arrendatools_plantillas-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      907 2023-04-16 10:52:08.000000 arrendatools_plantillas-1.0.1/setup.py
```

### Comparing `arrendatools_plantillas-1.0.0/LICENSE` & `arrendatools_plantillas-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arrendatools_plantillas-1.0.0/PKG-INFO` & `arrendatools_plantillas-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrendatools_plantillas
-Version: 1.0.0
+Version: 1.0.1
 Summary: Módulo de Python que aplica plantillas usando jinja 2. Además incluye algunos filtros adicionales como el convertir un número a palabras.
 Home-page: https://github.com/hokus15/ArrendaToolsPlantillas
 Author: hokus15
 Author-email: hokus@hotmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `arrendatools_plantillas-1.0.0/README.md` & `arrendatools_plantillas-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `arrendatools_plantillas-1.0.0/arrendatools_plantillas.egg-info/PKG-INFO` & `arrendatools_plantillas-1.0.1/arrendatools_plantillas.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrendatools-plantillas
-Version: 1.0.0
+Version: 1.0.1
 Summary: Módulo de Python que aplica plantillas usando jinja 2. Además incluye algunos filtros adicionales como el convertir un número a palabras.
 Home-page: https://github.com/hokus15/ArrendaToolsPlantillas
 Author: hokus15
 Author-email: hokus@hotmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `arrendatools_plantillas-1.0.0/setup.py` & `arrendatools_plantillas-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 setup(
     name='arrendatools_plantillas',
     version=__version__,
     description='Módulo de Python que aplica plantillas usando jinja 2. Además incluye algunos filtros adicionales como el convertir un número a palabras.',
     url='https://github.com/hokus15/ArrendaToolsPlantillas',
     author='hokus15',
     author_email='hokus@hotmail.com',
     license='MIT',
-    packages=['arrendatools_plantillas'],
+    packages=['arrendatools_plantillas', 'arrendatools_plantillas.filters'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

