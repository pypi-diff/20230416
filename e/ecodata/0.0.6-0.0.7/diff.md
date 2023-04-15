# Comparing `tmp/ecodata-0.0.6.tar.gz` & `tmp/ecodata-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecodata-0.0.6.tar", last modified: Fri Apr 14 09:20:54 2023, max compression
+gzip compressed data, was "ecodata-0.0.7.tar", last modified: Sat Apr 15 22:51:46 2023, max compression
```

## Comparing `ecodata-0.0.6.tar` & `ecodata-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 09:20:54.804653 ecodata-0.0.6/
--rw-rw-rw-   0        0        0     1698 2023-04-14 09:20:54.803642 ecodata-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1414 2023-04-14 09:20:36.000000 ecodata-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-04-14 09:20:54.804653 ecodata-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      941 2023-04-14 09:20:32.000000 ecodata-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:20:54.783700 ecodata-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 09:20:54.783700 ecodata-0.0.6/src/api/
-drwxrwxrwx   0        0        0        0 2023-04-14 09:20:54.802644 ecodata-0.0.6/src/api/ecodata.egg-info/
--rw-rw-rw-   0        0        0     1698 2023-04-14 09:20:54.000000 ecodata-0.0.6/src/api/ecodata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-04-14 09:20:54.000000 ecodata-0.0.6/src/api/ecodata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 09:20:54.000000 ecodata-0.0.6/src/api/ecodata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-04-14 09:20:54.000000 ecodata-0.0.6/src/api/ecodata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 09:20:54.000000 ecodata-0.0.6/src/api/ecodata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 22:51:46.380522 ecodata-0.0.7/
+-rw-rw-rw-   0        0        0     1547 2023-04-15 22:51:46.379524 ecodata-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1262 2023-04-15 22:51:00.000000 ecodata-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-15 22:51:46.380522 ecodata-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      933 2023-04-15 22:49:32.000000 ecodata-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 22:51:46.361572 ecodata-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 22:51:46.378526 ecodata-0.0.7/src/ecodata.egg-info/
+-rw-rw-rw-   0        0        0     1547 2023-04-15 22:51:46.000000 ecodata-0.0.7/src/ecodata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-04-15 22:51:46.000000 ecodata-0.0.7/src/ecodata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 22:51:46.000000 ecodata-0.0.7/src/ecodata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-04-15 22:51:46.000000 ecodata-0.0.7/src/ecodata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 22:51:46.000000 ecodata-0.0.7/src/ecodata.egg-info/top_level.txt
```

### Comparing `ecodata-0.0.6/PKG-INFO` & `ecodata-0.0.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Metadata-Version: 2.1
 Name: ecodata
-Version: 0.0.6
-Summary: Extracción de series de tiempo de las seis principales instituciones económicas para el Perú
+Version: 0.0.7
+Summary: Extracción de series de tiempo de las cinco principales instituciones económicas para el Perú
 Home-page: https://github.com/mauricioalvaradoo/ecodata
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Ecodata
-Extracción de series de tiempo de las seis principales instituciones económicas para el Perú:
+Extracción de series de tiempo de las cinco principales instituciones económicas para el Perú:
 1. BCRP
 2. YahooFinance
 3. FRED
-4. IMF
-5. WorldBank
-6. OCDE
+4. WorldBank
+5. OCDE
 
 ```
 # Instalación mediante PyPI
 !pip install ecodata
 ```
 
 
-## Versión 0.0.6
+## Versión 0.0.7
 * Para el Banco Central de Reserva del Perú (`BCRP`), `Yahoo Finance`, Federal Reserve Economic Data (`FRED`) y el `World Bank`, se cuenta con ambas métodos: `get_data()` y `search()`.
-* Para el IMF, únicamente se cuenta únicamente con `search()`. Recomendamos por el momento extraer las series en [EconDB](https://www.econdb.com/tree/).
-* Para la OCDE, se cuenta únicamente con `get_data()`.
+* Para la OCDE, se cuenta únicamente con el método `get_data()`.
 
 
 ## Métodos
 Para cada institución se tienen dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
 ```
 get_data()
 ```
```

### Comparing `ecodata-0.0.6/README.md` & `ecodata-0.0.7/src/ecodata.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,32 @@
+Metadata-Version: 2.1
+Name: ecodata
+Version: 0.0.7
+Summary: Extracción de series de tiempo de las cinco principales instituciones económicas para el Perú
+Home-page: https://github.com/mauricioalvaradoo/ecodata
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # Ecodata
-Extracción de series de tiempo de las seis principales instituciones económicas para el Perú:
+Extracción de series de tiempo de las cinco principales instituciones económicas para el Perú:
 1. BCRP
 2. YahooFinance
 3. FRED
-4. IMF
-5. WorldBank
-6. OCDE
+4. WorldBank
+5. OCDE
 
 ```
 # Instalación mediante PyPI
 !pip install ecodata
 ```
 
 
-## Versión 0.0.6
+## Versión 0.0.7
 * Para el Banco Central de Reserva del Perú (`BCRP`), `Yahoo Finance`, Federal Reserve Economic Data (`FRED`) y el `World Bank`, se cuenta con ambas métodos: `get_data()` y `search()`.
-* Para el IMF, únicamente se cuenta únicamente con `search()`. Recomendamos por el momento extraer las series en [EconDB](https://www.econdb.com/tree/).
-* Para la OCDE, se cuenta únicamente con `get_data()`.
+* Para la OCDE, se cuenta únicamente con el método `get_data()`.
 
 
 ## Métodos
 Para cada institución se tienen dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
 ```
 get_data()
 ```
```

### Comparing `ecodata-0.0.6/setup.py` & `ecodata-0.0.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='ecodata',
-    version = '0.0.6',
+    version = '0.0.7',
     authors = [
         'Mauricio Alvarado',
         'Andrei Romero'
     ],
-    description = 'Extracción de series de tiempo de las seis principales instituciones económicas para el Perú',
+    description = 'Extracción de series de tiempo de las cinco principales instituciones económicas para el Perú',
     long_description = long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mauricioalvaradoo/ecodata',
     classifier = [
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
+        'Operating System :: OS Independent'
     ], 
-    package_dir={'':'src/api'},
-    packages=setuptools.find_packages(where='src/api'),
+    package_dir={'':'src'},
+    packages=setuptools.find_packages(where='src'),
     python_requires='>=3.6',
     install_requires = [
         'pandas',
         'numpy',
         'yfinance',
         'requests'
     ]
```

