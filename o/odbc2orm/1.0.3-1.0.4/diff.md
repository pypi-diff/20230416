# Comparing `tmp/odbc2orm-1.0.3.tar.gz` & `tmp/odbc2orm-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odbc2orm-1.0.3.tar", last modified: Sun Apr 16 14:14:06 2023, max compression
+gzip compressed data, was "odbc2orm-1.0.4.tar", last modified: Sun Apr 16 14:24:52 2023, max compression
```

## Comparing `odbc2orm-1.0.3.tar` & `odbc2orm-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 14:14:06.553750 odbc2orm-1.0.3/
--rw-rw-rw-   0        0        0     6129 2023-04-16 14:14:06.553750 odbc2orm-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5368 2023-04-16 13:12:27.000000 odbc2orm-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 14:14:06.538116 odbc2orm-1.0.3/odbc2orm/
--rw-rw-rw-   0        0        0        0 2023-04-14 04:28:25.000000 odbc2orm-1.0.3/odbc2orm/__init__.py
--rw-rw-rw-   0        0        0     5271 2023-04-16 13:06:20.000000 odbc2orm-1.0.3/odbc2orm/__main__.py
--rw-rw-rw-   0        0        0      331 2023-04-16 13:02:50.000000 odbc2orm-1.0.3/odbc2orm/config.py
--rw-rw-rw-   0        0        0     3316 2023-04-16 12:34:31.000000 odbc2orm-1.0.3/odbc2orm/convert.py
--rw-rw-rw-   0        0        0     3958 2023-04-14 07:48:05.000000 odbc2orm-1.0.3/odbc2orm/database.py
--rw-rw-rw-   0        0        0     4407 2023-04-16 13:06:53.000000 odbc2orm-1.0.3/odbc2orm/template.py
--rw-rw-rw-   0        0        0      957 2023-04-14 06:31:26.000000 odbc2orm-1.0.3/odbc2orm/version.py
-drwxrwxrwx   0        0        0        0 2023-04-16 14:14:06.553750 odbc2orm-1.0.3/odbc2orm.egg-info/
--rw-rw-rw-   0        0        0     6129 2023-04-16 14:14:06.000000 odbc2orm-1.0.3/odbc2orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2023-04-16 14:14:06.000000 odbc2orm-1.0.3/odbc2orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 14:14:06.000000 odbc2orm-1.0.3/odbc2orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-16 14:14:06.000000 odbc2orm-1.0.3/odbc2orm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-04-16 14:14:06.000000 odbc2orm-1.0.3/odbc2orm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-16 14:14:06.000000 odbc2orm-1.0.3/odbc2orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      369 2023-04-16 14:14:06.553750 odbc2orm-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2016 2023-04-16 14:13:31.000000 odbc2orm-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:24:52.604457 odbc2orm-1.0.4/
+-rw-rw-rw-   0        0        0     6225 2023-04-16 14:24:52.604457 odbc2orm-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5464 2023-04-16 14:24:08.000000 odbc2orm-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 14:24:52.573202 odbc2orm-1.0.4/odbc2orm/
+-rw-rw-rw-   0        0        0        0 2023-04-14 04:28:25.000000 odbc2orm-1.0.4/odbc2orm/__init__.py
+-rw-rw-rw-   0        0        0     5271 2023-04-16 13:06:20.000000 odbc2orm-1.0.4/odbc2orm/__main__.py
+-rw-rw-rw-   0        0        0      331 2023-04-16 13:02:50.000000 odbc2orm-1.0.4/odbc2orm/config.py
+-rw-rw-rw-   0        0        0     3316 2023-04-16 12:34:31.000000 odbc2orm-1.0.4/odbc2orm/convert.py
+-rw-rw-rw-   0        0        0     3958 2023-04-14 07:48:05.000000 odbc2orm-1.0.4/odbc2orm/database.py
+-rw-rw-rw-   0        0        0     4407 2023-04-16 13:06:53.000000 odbc2orm-1.0.4/odbc2orm/template.py
+-rw-rw-rw-   0        0        0      957 2023-04-14 06:31:26.000000 odbc2orm-1.0.4/odbc2orm/version.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:24:52.588828 odbc2orm-1.0.4/odbc2orm.egg-info/
+-rw-rw-rw-   0        0        0     6225 2023-04-16 14:24:52.000000 odbc2orm-1.0.4/odbc2orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2023-04-16 14:24:52.000000 odbc2orm-1.0.4/odbc2orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 14:24:52.000000 odbc2orm-1.0.4/odbc2orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-16 14:24:52.000000 odbc2orm-1.0.4/odbc2orm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-04-16 14:24:52.000000 odbc2orm-1.0.4/odbc2orm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-16 14:24:52.000000 odbc2orm-1.0.4/odbc2orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      369 2023-04-16 14:24:52.620081 odbc2orm-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2016 2023-04-16 14:24:27.000000 odbc2orm-1.0.4/setup.py
```

### Comparing `odbc2orm-1.0.3/PKG-INFO` & `odbc2orm-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odbc2orm
-Version: 1.0.3
+Version: 1.0.4
 Summary: Convert ODBC schema to ORM
 Home-page: https://github.com/pe2mbs/odbc2orm
 Author: Marc Bertens-Nguyen
 Author-email: m.bertens@pe2mbs.nl
 Project-URL: Source Public, https://github.com/pe2mbs/odbc2orm/
 Project-URL: Bug Reports, https://github.com/pe2mbs/odbc2orm/issues
 Project-URL: Say Thanks!, https://github.com/pe2mbs/odbc2orm/saythanks
@@ -21,15 +21,17 @@
 This package convert an ODBC schema into a sqlalchemy ORM schema.
 Its primary written for MS Access schemas, but it should work for all ODBC 
 relational databases. for this only the driver should be configured. And for 
 the target project extra packages may be needed (see **Required packages for target project**).
 
 
 # Licence
-This package is under GNU GENERAL PUBLIC LICENSE, Version 2 only
+This package is under GNU GENERAL PUBLIC LICENSE, Version 2 only. 
+Therefore article 9 of "GNU GENERAL PUBLIC LICENSE, Version 2, June 1991" does not apply. 
+
 See LICENCE file for the GNU GENERAL PUBLIC LICENSE, Version 2, June 1991
 
 
 # Required packages for target project
 Assumming **sqlalchemy** is already in your project. The following two 
 packages are required when accessing MS Access databases; 
 * sqlalchemy-access
```

### Comparing `odbc2orm-1.0.3/README.md` & `odbc2orm-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 This package convert an ODBC schema into a sqlalchemy ORM schema.
 Its primary written for MS Access schemas, but it should work for all ODBC 
 relational databases. for this only the driver should be configured. And for 
 the target project extra packages may be needed (see **Required packages for target project**).
 
 
 # Licence
-This package is under GNU GENERAL PUBLIC LICENSE, Version 2 only
+This package is under GNU GENERAL PUBLIC LICENSE, Version 2 only. 
+Therefore article 9 of "GNU GENERAL PUBLIC LICENSE, Version 2, June 1991" does not apply. 
+
 See LICENCE file for the GNU GENERAL PUBLIC LICENSE, Version 2, June 1991
 
 
 # Required packages for target project
 Assumming **sqlalchemy** is already in your project. The following two 
 packages are required when accessing MS Access databases; 
 * sqlalchemy-access
```

### Comparing `odbc2orm-1.0.3/odbc2orm/__main__.py` & `odbc2orm-1.0.4/odbc2orm/__main__.py`

 * *Files identical despite different names*

### Comparing `odbc2orm-1.0.3/odbc2orm/convert.py` & `odbc2orm-1.0.4/odbc2orm/convert.py`

 * *Files identical despite different names*

### Comparing `odbc2orm-1.0.3/odbc2orm/database.py` & `odbc2orm-1.0.4/odbc2orm/database.py`

 * *Files identical despite different names*

### Comparing `odbc2orm-1.0.3/odbc2orm/template.py` & `odbc2orm-1.0.4/odbc2orm/template.py`

 * *Files identical despite different names*

### Comparing `odbc2orm-1.0.3/odbc2orm/version.py` & `odbc2orm-1.0.4/odbc2orm/version.py`

 * *Files identical despite different names*

### Comparing `odbc2orm-1.0.3/odbc2orm.egg-info/PKG-INFO` & `odbc2orm-1.0.4/odbc2orm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odbc2orm
-Version: 1.0.3
+Version: 1.0.4
 Summary: Convert ODBC schema to ORM
 Home-page: https://github.com/pe2mbs/odbc2orm
 Author: Marc Bertens-Nguyen
 Author-email: m.bertens@pe2mbs.nl
 Project-URL: Source Public, https://github.com/pe2mbs/odbc2orm/
 Project-URL: Bug Reports, https://github.com/pe2mbs/odbc2orm/issues
 Project-URL: Say Thanks!, https://github.com/pe2mbs/odbc2orm/saythanks
@@ -21,15 +21,17 @@
 This package convert an ODBC schema into a sqlalchemy ORM schema.
 Its primary written for MS Access schemas, but it should work for all ODBC 
 relational databases. for this only the driver should be configured. And for 
 the target project extra packages may be needed (see **Required packages for target project**).
 
 
 # Licence
-This package is under GNU GENERAL PUBLIC LICENSE, Version 2 only
+This package is under GNU GENERAL PUBLIC LICENSE, Version 2 only. 
+Therefore article 9 of "GNU GENERAL PUBLIC LICENSE, Version 2, June 1991" does not apply. 
+
 See LICENCE file for the GNU GENERAL PUBLIC LICENSE, Version 2, June 1991
 
 
 # Required packages for target project
 Assumming **sqlalchemy** is already in your project. The following two 
 packages are required when accessing MS Access databases; 
 * sqlalchemy-access
```

### Comparing `odbc2orm-1.0.3/setup.py` & `odbc2orm-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         return True
 
     def is_pure( self ):
         return True
 
 
 setup(  name                = 'odbc2orm',
-        version             = '1.0.3',
+        version             = '1.0.4',
         description         = 'Convert ODBC schema to ORM',
         long_description    = open("README.md","r" ).read(),
         long_description_content_type = 'text/markdown',
         author              = 'Marc Bertens-Nguyen',
         author_email        = 'm.bertens@pe2mbs.nl',
         url                 = 'https://github.com/pe2mbs/odbc2orm',
         install_requires    = [ 'PyYAML',
```

