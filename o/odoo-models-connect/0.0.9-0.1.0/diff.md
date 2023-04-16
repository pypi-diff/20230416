# Comparing `tmp/odoo_models_connect-0.0.9.tar.gz` & `tmp/odoo_models_connect-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo_models_connect-0.0.9.tar", last modified: Sun Mar  5 19:02:27 2023, max compression
+gzip compressed data, was "odoo_models_connect-0.1.0.tar", last modified: Sun Apr 16 14:54:31 2023, max compression
```

## Comparing `odoo_models_connect-0.0.9.tar` & `odoo_models_connect-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-05 19:02:27.234213 odoo_models_connect-0.0.9/
--rw-rw-rw-   0        0        0     2955 2023-03-05 19:02:27.233211 odoo_models_connect-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     2577 2023-03-05 19:01:39.000000 odoo_models_connect-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-03-05 19:02:27.197211 odoo_models_connect-0.0.9/odoo_models_connect/
--rw-rw-rw-   0        0        0     5875 2023-03-05 19:00:47.000000 odoo_models_connect-0.0.9/odoo_models_connect/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-05 19:02:27.228213 odoo_models_connect-0.0.9/odoo_models_connect.egg-info/
--rw-rw-rw-   0        0        0     2955 2023-03-05 19:02:27.000000 odoo_models_connect-0.0.9/odoo_models_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-03-05 19:02:27.000000 odoo_models_connect-0.0.9/odoo_models_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-05 19:02:27.000000 odoo_models_connect-0.0.9/odoo_models_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-03-05 19:02:27.000000 odoo_models_connect-0.0.9/odoo_models_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-03-05 19:02:27.000000 odoo_models_connect-0.0.9/odoo_models_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-05 19:02:27.236210 odoo_models_connect-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1450 2023-03-05 19:02:02.000000 odoo_models_connect-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:54:31.855806 odoo_models_connect-0.1.0/
+-rw-rw-rw-   0        0        0     2955 2023-04-16 14:54:31.855806 odoo_models_connect-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2577 2023-04-12 01:10:18.000000 odoo_models_connect-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 14:54:31.841163 odoo_models_connect-0.1.0/odoo_models_connect/
+-rw-rw-rw-   0        0        0       39 2023-04-12 01:10:18.000000 odoo_models_connect-0.1.0/odoo_models_connect/__init__.py
+-rw-rw-rw-   0        0        0     5905 2023-04-12 01:10:18.000000 odoo_models_connect-0.1.0/odoo_models_connect/connect_odoo.py
+-rw-rw-rw-   0        0        0      686 2023-04-12 01:41:36.000000 odoo_models_connect-0.1.0/odoo_models_connect/fields.py
+-rw-rw-rw-   0        0        0     3305 2023-04-16 14:51:40.000000 odoo_models_connect-0.1.0/odoo_models_connect/models.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:54:31.852296 odoo_models_connect-0.1.0/odoo_models_connect.egg-info/
+-rw-rw-rw-   0        0        0     2955 2023-04-16 14:54:31.000000 odoo_models_connect-0.1.0/odoo_models_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-04-16 14:54:31.000000 odoo_models_connect-0.1.0/odoo_models_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 14:54:31.000000 odoo_models_connect-0.1.0/odoo_models_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-04-16 14:54:31.000000 odoo_models_connect-0.1.0/odoo_models_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-16 14:54:31.000000 odoo_models_connect-0.1.0/odoo_models_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 14:54:31.855806 odoo_models_connect-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1454 2023-04-16 14:51:40.000000 odoo_models_connect-0.1.0/setup.py
```

### Comparing `odoo_models_connect-0.0.9/PKG-INFO` & `odoo_models_connect-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo_models_connect
-Version: 0.0.9
+Version: 0.1.0
 Summary: Library to improve interaction and communication with odoo for integration with other technologies.
 Home-page: https://github.com/DeijoseDevelop/odoo_models_connect
 Author: Deiver Jose Vazquez Moreno
 Author-email: estudiandovazmore@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `odoo_models_connect-0.0.9/README.md` & `odoo_models_connect-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `odoo_models_connect-0.0.9/odoo_models_connect/__init__.py` & `odoo_models_connect-0.1.0/odoo_models_connect/connect_odoo.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,18 @@
     username = None
     password = None
     uid = None
 
     def __init__(self, url: str, db: str):
         self.__url = url
         self.__db = db
-        self.__models = xmlrpc.client.ServerProxy('{}/xmlrpc/2/object'.format(url))
-        self.__common = xmlrpc.client.ServerProxy('{}/xmlrpc/2/common'.format(url))
+        self.__models = xmlrpc.client.ServerProxy(
+            '{}/xmlrpc/2/object'.format(url))
+        self.__common = xmlrpc.client.ServerProxy(
+            '{}/xmlrpc/2/common'.format(url))
 
     def authenticate(self, email: str, password: str):
         """authenticates the user in the odoo system with email and password.
 
         Args:
             email (str): user email.
             password (str): user password.
@@ -158,8 +160,8 @@
         self.__models.execute_kw(
             self.__db,
             self.uid,
             self.password,
             model_name,
             'unlink',
             [[int(object_id)]]
-        )
+        )
```

### Comparing `odoo_models_connect-0.0.9/odoo_models_connect.egg-info/PKG-INFO` & `odoo_models_connect-0.1.0/odoo_models_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-models-connect
-Version: 0.0.9
+Version: 0.1.0
 Summary: Library to improve interaction and communication with odoo for integration with other technologies.
 Home-page: https://github.com/DeijoseDevelop/odoo_models_connect
 Author: Deiver Jose Vazquez Moreno
 Author-email: estudiandovazmore@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `odoo_models_connect-0.0.9/setup.py` & `odoo_models_connect-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.9'  # Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+VERSION = '0.1.0'  # Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 # Debe coincidir con el nombre de la carpeta
 PACKAGE_NAME = 'odoo_models_connect'
 AUTHOR = 'Deiver Jose Vazquez Moreno'  # Modificar con vuestros datos
 AUTHOR_EMAIL = 'estudiandovazmore@gmail.com'  # Modificar con vuestros datos
 # Modificar con vuestros datos
 URL = 'https://github.com/DeijoseDevelop/odoo_models_connect'
 
 LICENSE = 'MIT'  # Tipo de licencia
 DESCRIPTION = 'Library to improve interaction and communication with odoo for integration with other technologies.'  # Descripción corta
 # Referencia al documento README con una descripción más elaborada
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding='utf-8')
 LONG_DESC_TYPE = "text/markdown"
 
 
-# Paquetes necesarios para que funcione la libreía. Se instalarán a la vez si no lo tuvieras ya instalado
+# Paquetes necesarios para que funcione la librería. Se instalarán a la vez si no lo tuvieras ya instalado
 INSTALL_REQUIRES = [
-    'schematics>=2.1.0'
+    'python-dotenv>=1.0.0'
 ]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
```

