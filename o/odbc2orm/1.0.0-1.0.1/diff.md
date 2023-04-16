# Comparing `tmp/odbc2orm-1.0.0.tar.gz` & `tmp/odbc2orm-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odbc2orm-1.0.0.tar", last modified: Sun Apr 16 13:42:18 2023, max compression
+gzip compressed data, was "odbc2orm-1.0.1.tar", last modified: Sun Apr 16 13:51:59 2023, max compression
```

## Comparing `odbc2orm-1.0.0.tar` & `odbc2orm-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 13:42:18.572788 odbc2orm-1.0.0/
--rw-rw-rw-   0        0        0      887 2023-04-16 13:42:18.572788 odbc2orm-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5368 2023-04-16 13:12:27.000000 odbc2orm-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 13:42:18.525897 odbc2orm-1.0.0/odbc2orm/
--rw-rw-rw-   0        0        0        0 2023-04-14 04:28:25.000000 odbc2orm-1.0.0/odbc2orm/__init__.py
--rw-rw-rw-   0        0        0     5271 2023-04-16 13:06:20.000000 odbc2orm-1.0.0/odbc2orm/__main__.py
--rw-rw-rw-   0        0        0      331 2023-04-16 13:02:50.000000 odbc2orm-1.0.0/odbc2orm/config.py
--rw-rw-rw-   0        0        0     3316 2023-04-16 12:34:31.000000 odbc2orm-1.0.0/odbc2orm/convert.py
--rw-rw-rw-   0        0        0     3958 2023-04-14 07:48:05.000000 odbc2orm-1.0.0/odbc2orm/database.py
--rw-rw-rw-   0        0        0     4407 2023-04-16 13:06:53.000000 odbc2orm-1.0.0/odbc2orm/template.py
--rw-rw-rw-   0        0        0      957 2023-04-14 06:31:26.000000 odbc2orm-1.0.0/odbc2orm/version.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:42:18.572788 odbc2orm-1.0.0/odbc2orm.egg-info/
--rw-rw-rw-   0        0        0      887 2023-04-16 13:42:18.000000 odbc2orm-1.0.0/odbc2orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2023-04-16 13:42:18.000000 odbc2orm-1.0.0/odbc2orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 13:42:18.000000 odbc2orm-1.0.0/odbc2orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-16 13:42:18.000000 odbc2orm-1.0.0/odbc2orm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-04-16 13:42:18.000000 odbc2orm-1.0.0/odbc2orm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-16 13:42:18.000000 odbc2orm-1.0.0/odbc2orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      369 2023-04-16 13:42:18.572788 odbc2orm-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2100 2023-04-16 13:41:13.000000 odbc2orm-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:51:59.330267 odbc2orm-1.0.1/
+-rw-rw-rw-   0        0        0     6129 2023-04-16 13:51:59.330267 odbc2orm-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5368 2023-04-16 13:12:27.000000 odbc2orm-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 13:51:59.283417 odbc2orm-1.0.1/odbc2orm/
+-rw-rw-rw-   0        0        0        0 2023-04-14 04:28:25.000000 odbc2orm-1.0.1/odbc2orm/__init__.py
+-rw-rw-rw-   0        0        0     5271 2023-04-16 13:06:20.000000 odbc2orm-1.0.1/odbc2orm/__main__.py
+-rw-rw-rw-   0        0        0      331 2023-04-16 13:02:50.000000 odbc2orm-1.0.1/odbc2orm/config.py
+-rw-rw-rw-   0        0        0     3316 2023-04-16 12:34:31.000000 odbc2orm-1.0.1/odbc2orm/convert.py
+-rw-rw-rw-   0        0        0     3958 2023-04-14 07:48:05.000000 odbc2orm-1.0.1/odbc2orm/database.py
+-rw-rw-rw-   0        0        0     4407 2023-04-16 13:06:53.000000 odbc2orm-1.0.1/odbc2orm/template.py
+-rw-rw-rw-   0        0        0      957 2023-04-14 06:31:26.000000 odbc2orm-1.0.1/odbc2orm/version.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:51:59.327269 odbc2orm-1.0.1/odbc2orm.egg-info/
+-rw-rw-rw-   0        0        0     6129 2023-04-16 13:51:59.000000 odbc2orm-1.0.1/odbc2orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2023-04-16 13:51:59.000000 odbc2orm-1.0.1/odbc2orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 13:51:59.000000 odbc2orm-1.0.1/odbc2orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-16 13:51:59.000000 odbc2orm-1.0.1/odbc2orm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-04-16 13:51:59.000000 odbc2orm-1.0.1/odbc2orm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-16 13:51:59.000000 odbc2orm-1.0.1/odbc2orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      369 2023-04-16 13:51:59.334948 odbc2orm-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2016 2023-04-16 13:51:33.000000 odbc2orm-1.0.1/setup.py
```

### Comparing `odbc2orm-1.0.0/README.md` & `odbc2orm-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `odbc2orm-1.0.0/odbc2orm/__main__.py` & `odbc2orm-1.0.1/odbc2orm/__main__.py`

 * *Files identical despite different names*

### Comparing `odbc2orm-1.0.0/odbc2orm/convert.py` & `odbc2orm-1.0.1/odbc2orm/convert.py`

 * *Files identical despite different names*

### Comparing `odbc2orm-1.0.0/odbc2orm/database.py` & `odbc2orm-1.0.1/odbc2orm/database.py`

 * *Files identical despite different names*

### Comparing `odbc2orm-1.0.0/odbc2orm/template.py` & `odbc2orm-1.0.1/odbc2orm/template.py`

 * *Files identical despite different names*

### Comparing `odbc2orm-1.0.0/odbc2orm/version.py` & `odbc2orm-1.0.1/odbc2orm/version.py`

 * *Files identical despite different names*

### Comparing `odbc2orm-1.0.0/setup.py` & `odbc2orm-1.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,19 +9,18 @@
         return True
 
     def is_pure( self ):
         return True
 
 
 setup(  name                = 'odbc2orm',
-        version             = '1.0.0',
+        version             = '1.0.1',
         description         = 'Convert ODBC schema to ORM',
-        long_description    = """This package convert an ODBC schema into a sqlalchemy ORM schema.
-Its primary written for MS Access schemas, but it should work for all ODBC 
-relational databases.""",
+        long_description    = open("README.md","r" ).read(),
+        long_description_content_type = 'text/markdown',
         author              = 'Marc Bertens-Nguyen',
         author_email        = 'm.bertens@pe2mbs.nl',
         url                 = 'https://github.com/pe2mbs/odbc2orm',
         install_requires    = [ 'PyYAML',
                                 'pyodbc',
                                 'Mako'],
         classifiers         = [ 'Environment :: Console',
```

