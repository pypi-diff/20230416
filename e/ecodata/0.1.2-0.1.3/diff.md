# Comparing `tmp/ecodata-0.1.2.tar.gz` & `tmp/ecodata-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecodata-0.1.2.tar", last modified: Sat Apr 15 23:12:30 2023, max compression
+gzip compressed data, was "ecodata-0.1.3.tar", last modified: Sat Apr 15 23:16:21 2023, max compression
```

## Comparing `ecodata-0.1.2.tar` & `ecodata-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 23:12:30.356844 ecodata-0.1.2/
--rw-rw-rw-   0        0        0     1547 2023-04-15 23:12:30.355846 ecodata-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1262 2023-04-15 23:12:09.000000 ecodata-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-15 23:12:30.356844 ecodata-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      933 2023-04-15 23:12:12.000000 ecodata-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 23:12:30.336897 ecodata-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 23:12:30.354872 ecodata-0.1.2/src/ecodata.egg-info/
--rw-rw-rw-   0        0        0     1547 2023-04-15 23:12:30.000000 ecodata-0.1.2/src/ecodata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-04-15 23:12:30.000000 ecodata-0.1.2/src/ecodata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 23:12:30.000000 ecodata-0.1.2/src/ecodata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-04-15 23:12:30.000000 ecodata-0.1.2/src/ecodata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 23:12:30.000000 ecodata-0.1.2/src/ecodata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 23:16:21.145617 ecodata-0.1.3/
+-rw-rw-rw-   0        0        0     1547 2023-04-15 23:16:21.144621 ecodata-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1262 2023-04-15 23:15:37.000000 ecodata-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-15 23:16:21.145617 ecodata-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      933 2023-04-15 23:15:33.000000 ecodata-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 23:16:21.127665 ecodata-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 23:16:21.143623 ecodata-0.1.3/src/ecodata.egg-info/
+-rw-rw-rw-   0        0        0     1547 2023-04-15 23:16:21.000000 ecodata-0.1.3/src/ecodata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-04-15 23:16:21.000000 ecodata-0.1.3/src/ecodata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 23:16:21.000000 ecodata-0.1.3/src/ecodata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-04-15 23:16:21.000000 ecodata-0.1.3/src/ecodata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 23:16:21.000000 ecodata-0.1.3/src/ecodata.egg-info/top_level.txt
```

### Comparing `ecodata-0.1.2/PKG-INFO` & `ecodata-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecodata
-Version: 0.1.2
+Version: 0.1.3
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
 
 
-## Versión 0.1.2
+## Versión 0.1.3
 * Para el Banco Central de Reserva del Perú (`BCRP`), `Yahoo Finance`, Federal Reserve Economic Data (`FRED`) y el `World Bank`, se cuenta con ambas métodos: `get_data()` y `search()`.
 * Para la OCDE, se cuenta únicamente con el método `get_data()`.
 
 
 ## Métodos
 Para cada institución se tienen dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
 ```
```

### Comparing `ecodata-0.1.2/README.md` & `ecodata-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ```
 # Instalación mediante PyPI
 !pip install ecodata
 ```
 
 
-## Versión 0.1.2
+## Versión 0.1.3
 * Para el Banco Central de Reserva del Perú (`BCRP`), `Yahoo Finance`, Federal Reserve Economic Data (`FRED`) y el `World Bank`, se cuenta con ambas métodos: `get_data()` y `search()`.
 * Para la OCDE, se cuenta únicamente con el método `get_data()`.
 
 
 ## Métodos
 Para cada institución se tienen dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
 ```
```

### Comparing `ecodata-0.1.2/setup.py` & `ecodata-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='ecodata',
-    version = '0.1.2',
+    version = '0.1.3',
     authors = [
         'Mauricio Alvarado',
         'Andrei Romero'
     ],
     description = 'Extracción de series de tiempo de las cinco principales instituciones económicas para el Perú',
     long_description = long_description,
     long_description_content_type='text/markdown',
```

### Comparing `ecodata-0.1.2/src/ecodata.egg-info/PKG-INFO` & `ecodata-0.1.3/src/ecodata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecodata
-Version: 0.1.2
+Version: 0.1.3
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
 
 
-## Versión 0.1.2
+## Versión 0.1.3
 * Para el Banco Central de Reserva del Perú (`BCRP`), `Yahoo Finance`, Federal Reserve Economic Data (`FRED`) y el `World Bank`, se cuenta con ambas métodos: `get_data()` y `search()`.
 * Para la OCDE, se cuenta únicamente con el método `get_data()`.
 
 
 ## Métodos
 Para cada institución se tienen dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
 ```
```

