# Comparing `tmp/chibi_apache-0.0.1.tar.gz` & `tmp/chibi_apache-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chibi_apache-0.0.1.tar", last modified: Sun Apr 16 03:12:13 2023, max compression
+gzip compressed data, was "chibi_apache-0.0.2.tar", last modified: Sun Apr 16 03:33:25 2023, max compression
```

## Comparing `chibi_apache-0.0.1.tar` & `chibi_apache-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-16 03:12:13.908444 chibi_apache-0.0.1/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      150 2023-04-16 01:59:23.000000 chibi_apache-0.0.1/AUTHORS.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3586 2023-04-16 01:59:23.000000 chibi_apache-0.0.1/CONTRIBUTING.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       89 2023-04-16 01:59:23.000000 chibi_apache-0.0.1/HISTORY.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      470 2023-04-16 01:59:23.000000 chibi_apache-0.0.1/LICENSE
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      262 2023-04-16 01:59:23.000000 chibi_apache-0.0.1/MANIFEST.in
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1387 2023-04-16 03:12:13.908444 chibi_apache-0.0.1/PKG-INFO
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      706 2023-04-16 03:11:56.000000 chibi_apache-0.0.1/README.rst
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-16 03:12:13.905111 chibi_apache-0.0.1/chibi_apache/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      432 2023-04-16 02:19:52.000000 chibi_apache-0.0.1/chibi_apache/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1781 2023-04-16 03:06:38.000000 chibi_apache-0.0.1/chibi_apache/apache.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-16 03:12:13.908444 chibi_apache-0.0.1/chibi_apache.egg-info/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1387 2023-04-16 03:12:13.000000 chibi_apache-0.0.1/chibi_apache.egg-info/PKG-INFO
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      606 2023-04-16 03:12:13.000000 chibi_apache-0.0.1/chibi_apache.egg-info/SOURCES.txt
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        1 2023-04-16 03:12:13.000000 chibi_apache-0.0.1/chibi_apache.egg-info/dependency_links.txt
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        1 2023-04-16 03:12:13.000000 chibi_apache-0.0.1/chibi_apache.egg-info/not-zip-safe
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       14 2023-04-16 03:12:13.000000 chibi_apache-0.0.1/chibi_apache.egg-info/requires.txt
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       13 2023-04-16 03:12:13.000000 chibi_apache-0.0.1/chibi_apache.egg-info/top_level.txt
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-16 03:12:13.908444 chibi_apache-0.0.1/docs/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      613 2023-04-16 01:59:23.000000 chibi_apache-0.0.1/docs/Makefile
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       28 2023-04-16 01:59:23.000000 chibi_apache-0.0.1/docs/authors.rst
--rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)     4859 2023-04-16 01:59:23.000000 chibi_apache-0.0.1/docs/conf.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       33 2023-04-16 01:59:23.000000 chibi_apache-0.0.1/docs/contributing.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       28 2023-04-16 01:59:23.000000 chibi_apache-0.0.1/docs/history.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      309 2023-04-16 01:59:23.000000 chibi_apache-0.0.1/docs/index.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1150 2023-04-16 01:59:23.000000 chibi_apache-0.0.1/docs/installation.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      774 2023-04-16 01:59:23.000000 chibi_apache-0.0.1/docs/make.bat
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       27 2023-04-16 01:59:23.000000 chibi_apache-0.0.1/docs/readme.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       79 2023-04-16 01:59:23.000000 chibi_apache-0.0.1/docs/usage.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      457 2023-04-16 03:12:13.908444 chibi_apache-0.0.1/setup.cfg
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1076 2023-04-16 03:11:24.000000 chibi_apache-0.0.1/setup.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-16 03:12:13.908444 chibi_apache-0.0.1/tests/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       24 2023-04-16 01:59:23.000000 chibi_apache-0.0.1/tests/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1487 2023-04-16 03:09:33.000000 chibi_apache-0.0.1/tests/default.conf
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1487 2023-04-16 03:06:16.000000 chibi_apache-0.0.1/tests/default_clean.conf
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3824 2023-04-16 03:08:57.000000 chibi_apache-0.0.1/tests/test_chibi_apache.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-16 03:33:25.106835 chibi_apache-0.0.2/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      150 2023-04-16 01:59:23.000000 chibi_apache-0.0.2/AUTHORS.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3586 2023-04-16 01:59:23.000000 chibi_apache-0.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       89 2023-04-16 01:59:23.000000 chibi_apache-0.0.2/HISTORY.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      470 2023-04-16 01:59:23.000000 chibi_apache-0.0.2/LICENSE
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      262 2023-04-16 01:59:23.000000 chibi_apache-0.0.2/MANIFEST.in
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     5171 2023-04-16 03:33:25.106835 chibi_apache-0.0.2/PKG-INFO
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     4490 2023-04-16 03:32:07.000000 chibi_apache-0.0.2/README.rst
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-16 03:33:25.103502 chibi_apache-0.0.2/chibi_apache/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      432 2023-04-16 03:33:18.000000 chibi_apache-0.0.2/chibi_apache/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1781 2023-04-16 03:06:38.000000 chibi_apache-0.0.2/chibi_apache/apache.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-16 03:33:25.103502 chibi_apache-0.0.2/chibi_apache.egg-info/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     5171 2023-04-16 03:33:25.000000 chibi_apache-0.0.2/chibi_apache.egg-info/PKG-INFO
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      606 2023-04-16 03:33:25.000000 chibi_apache-0.0.2/chibi_apache.egg-info/SOURCES.txt
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        1 2023-04-16 03:33:25.000000 chibi_apache-0.0.2/chibi_apache.egg-info/dependency_links.txt
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        1 2023-04-16 03:33:25.000000 chibi_apache-0.0.2/chibi_apache.egg-info/not-zip-safe
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       14 2023-04-16 03:33:25.000000 chibi_apache-0.0.2/chibi_apache.egg-info/requires.txt
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       13 2023-04-16 03:33:25.000000 chibi_apache-0.0.2/chibi_apache.egg-info/top_level.txt
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-16 03:33:25.103502 chibi_apache-0.0.2/docs/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      613 2023-04-16 01:59:23.000000 chibi_apache-0.0.2/docs/Makefile
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       28 2023-04-16 01:59:23.000000 chibi_apache-0.0.2/docs/authors.rst
+-rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)     4859 2023-04-16 01:59:23.000000 chibi_apache-0.0.2/docs/conf.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       33 2023-04-16 01:59:23.000000 chibi_apache-0.0.2/docs/contributing.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       28 2023-04-16 01:59:23.000000 chibi_apache-0.0.2/docs/history.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      309 2023-04-16 01:59:23.000000 chibi_apache-0.0.2/docs/index.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1150 2023-04-16 01:59:23.000000 chibi_apache-0.0.2/docs/installation.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      774 2023-04-16 01:59:23.000000 chibi_apache-0.0.2/docs/make.bat
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       27 2023-04-16 01:59:23.000000 chibi_apache-0.0.2/docs/readme.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       79 2023-04-16 01:59:23.000000 chibi_apache-0.0.2/docs/usage.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      457 2023-04-16 03:33:25.106835 chibi_apache-0.0.2/setup.cfg
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1076 2023-04-16 03:33:18.000000 chibi_apache-0.0.2/setup.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-16 03:33:25.106835 chibi_apache-0.0.2/tests/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       24 2023-04-16 01:59:23.000000 chibi_apache-0.0.2/tests/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1487 2023-04-16 03:31:51.000000 chibi_apache-0.0.2/tests/default.conf
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1487 2023-04-16 03:06:16.000000 chibi_apache-0.0.2/tests/default_clean.conf
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     4901 2023-04-16 03:31:55.000000 chibi_apache-0.0.2/tests/test_chibi_apache.py
```

### Comparing `chibi_apache-0.0.1/CONTRIBUTING.rst` & `chibi_apache-0.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `chibi_apache-0.0.1/chibi_apache/apache.py` & `chibi_apache-0.0.2/chibi_apache/apache.py`

 * *Files identical despite different names*

### Comparing `chibi_apache-0.0.1/chibi_apache.egg-info/SOURCES.txt` & `chibi_apache-0.0.2/chibi_apache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chibi_apache-0.0.1/docs/Makefile` & `chibi_apache-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chibi_apache-0.0.1/docs/conf.py` & `chibi_apache-0.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chibi_apache-0.0.1/docs/installation.rst` & `chibi_apache-0.0.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `chibi_apache-0.0.1/docs/make.bat` & `chibi_apache-0.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chibi_apache-0.0.1/setup.py` & `chibi_apache-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,10 +26,10 @@
     license="WTFPL",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='chibi_apache',
     name='chibi_apache',
     packages=find_packages(include=['chibi_apache', 'chibi_apache.*']),
     url='https://github.com/dem4ply/chibi_apache',
-    version='0.0.1',
+    version='0.0.2',
     zip_safe=False,
 )
```

### Comparing `chibi_apache-0.0.1/tests/default.conf` & `chibi_apache-0.0.2/tests/default.conf`

 * *Files identical despite different names*

### Comparing `chibi_apache-0.0.1/tests/default_clean.conf` & `chibi_apache-0.0.2/tests/default_clean.conf`

 * *Files identical despite different names*

### Comparing `chibi_apache-0.0.1/tests/test_chibi_apache.py` & `chibi_apache-0.0.2/tests/test_chibi_apache.py`

 * *Files 19% similar despite different names*

```diff
@@ -98,14 +98,15 @@
         self.assertEqual( result, self.content_clean )
 
 
 class Test_chibi_apache_file( unittest.TestCase ):
     def setUp( self ):
         self.file_service = Chibi_path( 'tests/default.conf' )
         self.expected = expected_default
+        self.temp_folder = Chibi_temp_path()
 
     def test_should_be_a_dict( self ):
         service = Chibi_apache( self.file_service )
         result = service.read()
         self.assertIsInstance( result, dict )
 
     def test_should_be_the_expected( self ):
@@ -115,7 +116,31 @@
 
     def test_write_should_work( self ):
         service = Chibi_apache( self.file_service )
         result = service.read()
         service.write( result )
         result_after_save = service.read()
         self.assertEqual( result, result_after_save )
+
+    def test_write_should_remove_the_directory_cgi_bin( self ):
+        service = Chibi_apache( self.file_service )
+        result = service.read()
+        result.Directory.pop( '"/var/www/cgi-bin"' )
+        new_conf_path= self.temp_folder.temp_file( extension='conf' )
+        new_conf = new_conf_path.open( chibi_file_class=Chibi_apache )
+        new_conf.write( result )
+        result_after_save = new_conf.read()
+        self.assertNotIn( '"/var/www/cgi-bin"', result_after_save.Directory )
+
+    def test_write_should_work_if_change_the_property( self ):
+        service = Chibi_apache( self.file_service )
+        result = service.read()
+        self.assertTrue( result.User != 'root' )
+
+        result.pop( 'User' )
+        result.User = 'root'
+
+        new_conf_path= self.temp_folder.temp_file( extension='conf' )
+        new_conf = new_conf_path.open( chibi_file_class=Chibi_apache )
+        new_conf.write( result )
+        result_after_save = new_conf.read()
+        self.assertEqual( 'root', result_after_save.User )
```

