# Comparing `tmp/ecodata-0.0.7.tar.gz` & `tmp/ecodata-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecodata-0.0.7.tar", last modified: Sat Apr 15 22:51:46 2023, max compression
+gzip compressed data, was "ecodata-0.0.8.tar", last modified: Sat Apr 15 22:57:37 2023, max compression
```

## Comparing `ecodata-0.0.7.tar` & `ecodata-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 22:51:46.380522 ecodata-0.0.7/
--rw-rw-rw-   0        0        0     1547 2023-04-15 22:51:46.379524 ecodata-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1262 2023-04-15 22:51:00.000000 ecodata-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-04-15 22:51:46.380522 ecodata-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      933 2023-04-15 22:49:32.000000 ecodata-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 22:51:46.361572 ecodata-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 22:51:46.378526 ecodata-0.0.7/src/ecodata.egg-info/
--rw-rw-rw-   0        0        0     1547 2023-04-15 22:51:46.000000 ecodata-0.0.7/src/ecodata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-04-15 22:51:46.000000 ecodata-0.0.7/src/ecodata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 22:51:46.000000 ecodata-0.0.7/src/ecodata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-04-15 22:51:46.000000 ecodata-0.0.7/src/ecodata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 22:51:46.000000 ecodata-0.0.7/src/ecodata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 22:57:37.022667 ecodata-0.0.8/
+-rw-rw-rw-   0        0        0     1547 2023-04-15 22:57:37.021680 ecodata-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1262 2023-04-15 22:57:19.000000 ecodata-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-15 22:57:37.022667 ecodata-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      933 2023-04-15 22:56:30.000000 ecodata-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 22:57:37.003336 ecodata-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 22:57:37.020674 ecodata-0.0.8/src/ecodata.egg-info/
+-rw-rw-rw-   0        0        0     1547 2023-04-15 22:57:36.000000 ecodata-0.0.8/src/ecodata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-04-15 22:57:36.000000 ecodata-0.0.8/src/ecodata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 22:57:36.000000 ecodata-0.0.8/src/ecodata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-04-15 22:57:36.000000 ecodata-0.0.8/src/ecodata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 22:57:36.000000 ecodata-0.0.8/src/ecodata.egg-info/top_level.txt
```

### Comparing `ecodata-0.0.7/PKG-INFO` & `ecodata-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecodata
-Version: 0.0.7
+Version: 0.0.8
 Summary: Extracción de series de tiempo de las cinco principales instituciones económicas para el Perú
 Home-page: https://github.com/mauricioalvaradoo/ecodata
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Ecodata
 Extracción de series de tiempo de las cinco principales instituciones económicas para el Perú:
@@ -16,15 +16,15 @@
 
 ```
 # Instalación mediante PyPI
 !pip install ecodata
 ```
 
 
-## Versión 0.0.7
+## Versión 0.0.8
 * Para el Banco Central de Reserva del Perú (`BCRP`), `Yahoo Finance`, Federal Reserve Economic Data (`FRED`) y el `World Bank`, se cuenta con ambas métodos: `get_data()` y `search()`.
 * Para la OCDE, se cuenta únicamente con el método `get_data()`.
 
 
 ## Métodos
 Para cada institución se tienen dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
 ```
```

### Comparing `ecodata-0.0.7/README.md` & `ecodata-0.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ```
 # Instalación mediante PyPI
 !pip install ecodata
 ```
 
 
-## Versión 0.0.7
+## Versión 0.0.8
 * Para el Banco Central de Reserva del Perú (`BCRP`), `Yahoo Finance`, Federal Reserve Economic Data (`FRED`) y el `World Bank`, se cuenta con ambas métodos: `get_data()` y `search()`.
 * Para la OCDE, se cuenta únicamente con el método `get_data()`.
 
 
 ## Métodos
 Para cada institución se tienen dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
 ```
```

### Comparing `ecodata-0.0.7/setup.py` & `ecodata-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='ecodata',
-    version = '0.0.7',
+    version = '0.0.8',
     authors = [
         'Mauricio Alvarado',
         'Andrei Romero'
     ],
     description = 'Extracción de series de tiempo de las cinco principales instituciones económicas para el Perú',
     long_description = long_description,
     long_description_content_type='text/markdown',
```

### Comparing `ecodata-0.0.7/src/ecodata.egg-info/PKG-INFO` & `ecodata-0.0.8/src/ecodata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecodata
-Version: 0.0.7
+Version: 0.0.8
 Summary: Extracción de series de tiempo de las cinco principales instituciones económicas para el Perú
 Home-page: https://github.com/mauricioalvaradoo/ecodata
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Ecodata
 Extracción de series de tiempo de las cinco principales instituciones económicas para el Perú:
@@ -16,15 +16,15 @@
 
 ```
 # Instalación mediante PyPI
 !pip install ecodata
 ```
 
 
-## Versión 0.0.7
+## Versión 0.0.8
 * Para el Banco Central de Reserva del Perú (`BCRP`), `Yahoo Finance`, Federal Reserve Economic Data (`FRED`) y el `World Bank`, se cuenta con ambas métodos: `get_data()` y `search()`.
 * Para la OCDE, se cuenta únicamente con el método `get_data()`.
 
 
 ## Métodos
 Para cada institución se tienen dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
 ```
```

