# Comparing `tmp/ecodata-0.1.3.tar.gz` & `tmp/ecodata-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecodata-0.1.3.tar", last modified: Sat Apr 15 23:16:21 2023, max compression
+gzip compressed data, was "ecodata-0.1.4.tar", last modified: Sat Apr 15 23:23:22 2023, max compression
```

## Comparing `ecodata-0.1.3.tar` & `ecodata-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 23:16:21.145617 ecodata-0.1.3/
--rw-rw-rw-   0        0        0     1547 2023-04-15 23:16:21.144621 ecodata-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1262 2023-04-15 23:15:37.000000 ecodata-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-15 23:16:21.145617 ecodata-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      933 2023-04-15 23:15:33.000000 ecodata-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 23:16:21.127665 ecodata-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 23:16:21.143623 ecodata-0.1.3/src/ecodata.egg-info/
--rw-rw-rw-   0        0        0     1547 2023-04-15 23:16:21.000000 ecodata-0.1.3/src/ecodata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-04-15 23:16:21.000000 ecodata-0.1.3/src/ecodata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 23:16:21.000000 ecodata-0.1.3/src/ecodata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-04-15 23:16:21.000000 ecodata-0.1.3/src/ecodata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 23:16:21.000000 ecodata-0.1.3/src/ecodata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 23:23:22.767218 ecodata-0.1.4/
+-rw-rw-rw-   0        0        0     1547 2023-04-15 23:23:22.766196 ecodata-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1262 2023-04-15 23:22:49.000000 ecodata-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-15 23:23:22.767218 ecodata-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      933 2023-04-15 23:22:53.000000 ecodata-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 23:23:22.747246 ecodata-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 23:23:22.765221 ecodata-0.1.4/src/ecodata.egg-info/
+-rw-rw-rw-   0        0        0     1547 2023-04-15 23:23:22.000000 ecodata-0.1.4/src/ecodata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-04-15 23:23:22.000000 ecodata-0.1.4/src/ecodata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 23:23:22.000000 ecodata-0.1.4/src/ecodata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-04-15 23:23:22.000000 ecodata-0.1.4/src/ecodata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 23:23:22.000000 ecodata-0.1.4/src/ecodata.egg-info/top_level.txt
```

### Comparing `ecodata-0.1.3/PKG-INFO` & `ecodata-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecodata
-Version: 0.1.3
+Version: 0.1.4
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
 
 
-## Versión 0.1.3
+## Versión 0.1.4
 * Para el Banco Central de Reserva del Perú (`BCRP`), `Yahoo Finance`, Federal Reserve Economic Data (`FRED`) y el `World Bank`, se cuenta con ambas métodos: `get_data()` y `search()`.
 * Para la OCDE, se cuenta únicamente con el método `get_data()`.
 
 
 ## Métodos
 Para cada institución se tienen dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
 ```
```

### Comparing `ecodata-0.1.3/README.md` & `ecodata-0.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ```
 # Instalación mediante PyPI
 !pip install ecodata
 ```
 
 
-## Versión 0.1.3
+## Versión 0.1.4
 * Para el Banco Central de Reserva del Perú (`BCRP`), `Yahoo Finance`, Federal Reserve Economic Data (`FRED`) y el `World Bank`, se cuenta con ambas métodos: `get_data()` y `search()`.
 * Para la OCDE, se cuenta únicamente con el método `get_data()`.
 
 
 ## Métodos
 Para cada institución se tienen dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
 ```
```

### Comparing `ecodata-0.1.3/setup.py` & `ecodata-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='ecodata',
-    version = '0.1.3',
+    version = '0.1.4',
     authors = [
         'Mauricio Alvarado',
         'Andrei Romero'
     ],
     description = 'Extracción de series de tiempo de las cinco principales instituciones económicas para el Perú',
     long_description = long_description,
     long_description_content_type='text/markdown',
```

### Comparing `ecodata-0.1.3/src/ecodata.egg-info/PKG-INFO` & `ecodata-0.1.4/src/ecodata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecodata
-Version: 0.1.3
+Version: 0.1.4
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
 
 
-## Versión 0.1.3
+## Versión 0.1.4
 * Para el Banco Central de Reserva del Perú (`BCRP`), `Yahoo Finance`, Federal Reserve Economic Data (`FRED`) y el `World Bank`, se cuenta con ambas métodos: `get_data()` y `search()`.
 * Para la OCDE, se cuenta únicamente con el método `get_data()`.
 
 
 ## Métodos
 Para cada institución se tienen dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
 ```
```

