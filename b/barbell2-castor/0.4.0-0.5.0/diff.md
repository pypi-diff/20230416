# Comparing `tmp/barbell2_castor-0.4.0.tar.gz` & `tmp/barbell2_castor-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/barbell2_castor-0.4.0.tar", last modified: Sat Apr 15 22:03:48 2023, max compression
+gzip compressed data, was "dist/barbell2_castor-0.5.0.tar", last modified: Sat Apr 15 22:15:46 2023, max compression
```

## Comparing `barbell2_castor-0.4.0.tar` & `barbell2_castor-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 22:03:48.590108 barbell2_castor-0.4.0/
--rw-r--r--   0 ralph      (501) staff       (20)      784 2023-04-15 22:03:48.589865 barbell2_castor-0.4.0/PKG-INFO
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 22:03:48.588055 barbell2_castor-0.4.0/barbell2_castor/
--rw-r--r--   0 ralph      (501) staff       (20)      105 2023-04-15 22:03:45.000000 barbell2_castor-0.4.0/barbell2_castor/__init__.py
--rw-r--r--   0 ralph      (501) staff       (20)     9836 2023-04-15 21:52:42.000000 barbell2_castor-0.4.0/barbell2_castor/api.py
--rw-r--r--   0 ralph      (501) staff       (20)     6005 2023-04-15 22:03:25.000000 barbell2_castor-0.4.0/barbell2_castor/castor2sqlite.py
--rw-r--r--   0 ralph      (501) staff       (20)     1630 2023-04-15 22:02:16.000000 barbell2_castor-0.4.0/barbell2_castor/query.py
--rw-r--r--   0 ralph      (501) staff       (20)      628 2023-04-15 12:26:09.000000 barbell2_castor-0.4.0/barbell2_castor/utils.py
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 22:03:48.589559 barbell2_castor-0.4.0/barbell2_castor.egg-info/
--rw-r--r--   0 ralph      (501) staff       (20)      784 2023-04-15 22:03:48.000000 barbell2_castor-0.4.0/barbell2_castor.egg-info/PKG-INFO
--rw-r--r--   0 ralph      (501) staff       (20)      416 2023-04-15 22:03:48.000000 barbell2_castor-0.4.0/barbell2_castor.egg-info/SOURCES.txt
--rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-15 22:03:48.000000 barbell2_castor-0.4.0/barbell2_castor.egg-info/dependency_links.txt
--rw-r--r--   0 ralph      (501) staff       (20)       20 2023-04-15 22:03:48.000000 barbell2_castor-0.4.0/barbell2_castor.egg-info/entry_points.txt
--rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-15 12:23:48.000000 barbell2_castor-0.4.0/barbell2_castor.egg-info/not-zip-safe
--rw-r--r--   0 ralph      (501) staff       (20)       34 2023-04-15 22:03:48.000000 barbell2_castor-0.4.0/barbell2_castor.egg-info/requires.txt
--rw-r--r--   0 ralph      (501) staff       (20)       16 2023-04-15 22:03:48.000000 barbell2_castor-0.4.0/barbell2_castor.egg-info/top_level.txt
--rw-r--r--   0 ralph      (501) staff       (20)       38 2023-04-15 22:03:48.590178 barbell2_castor-0.4.0/setup.cfg
--rw-r--r--   0 ralph      (501) staff       (20)     1372 2023-04-15 12:28:09.000000 barbell2_castor-0.4.0/setup.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 22:15:46.787475 barbell2_castor-0.5.0/
+-rw-r--r--   0 ralph      (501) staff       (20)      784 2023-04-15 22:15:46.787188 barbell2_castor-0.5.0/PKG-INFO
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 22:15:46.784995 barbell2_castor-0.5.0/barbell2_castor/
+-rw-r--r--   0 ralph      (501) staff       (20)      258 2023-04-15 22:15:43.000000 barbell2_castor-0.5.0/barbell2_castor/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     9836 2023-04-15 21:52:42.000000 barbell2_castor-0.5.0/barbell2_castor/api.py
+-rw-r--r--   0 ralph      (501) staff       (20)     6634 2023-04-15 22:13:15.000000 barbell2_castor-0.5.0/barbell2_castor/castor2sqlite.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1630 2023-04-15 22:02:16.000000 barbell2_castor-0.5.0/barbell2_castor/query.py
+-rw-r--r--   0 ralph      (501) staff       (20)      628 2023-04-15 12:26:09.000000 barbell2_castor-0.5.0/barbell2_castor/utils.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 22:15:46.786842 barbell2_castor-0.5.0/barbell2_castor.egg-info/
+-rw-r--r--   0 ralph      (501) staff       (20)      784 2023-04-15 22:15:46.000000 barbell2_castor-0.5.0/barbell2_castor.egg-info/PKG-INFO
+-rw-r--r--   0 ralph      (501) staff       (20)      416 2023-04-15 22:15:46.000000 barbell2_castor-0.5.0/barbell2_castor.egg-info/SOURCES.txt
+-rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-15 22:15:46.000000 barbell2_castor-0.5.0/barbell2_castor.egg-info/dependency_links.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       20 2023-04-15 22:15:46.000000 barbell2_castor-0.5.0/barbell2_castor.egg-info/entry_points.txt
+-rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-15 12:23:48.000000 barbell2_castor-0.5.0/barbell2_castor.egg-info/not-zip-safe
+-rw-r--r--   0 ralph      (501) staff       (20)       34 2023-04-15 22:15:46.000000 barbell2_castor-0.5.0/barbell2_castor.egg-info/requires.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       16 2023-04-15 22:15:46.000000 barbell2_castor-0.5.0/barbell2_castor.egg-info/top_level.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       38 2023-04-15 22:15:46.787549 barbell2_castor-0.5.0/setup.cfg
+-rw-r--r--   0 ralph      (501) staff       (20)     1372 2023-04-15 12:28:09.000000 barbell2_castor-0.5.0/setup.py
```

### Comparing `barbell2_castor-0.4.0/PKG-INFO` & `barbell2_castor-0.5.0/barbell2_castor.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
-Name: barbell2_castor
-Version: 0.4.0
+Name: barbell2-castor
+Version: 0.5.0
 Summary: Utilities for interfacing with Castor EDC
 Home-page: https://github.com/rbrecheisen/barbell2_castor
 Author: Ralph Brecheisen
 Author-email: r.brecheisen@maastrichtuniversity.nl
 License: MIT license
 Description: UNKNOWN
 Keywords: barbell2_castor
```

### Comparing `barbell2_castor-0.4.0/barbell2_castor/api.py` & `barbell2_castor-0.5.0/barbell2_castor/api.py`

 * *Files identical despite different names*

### Comparing `barbell2_castor-0.4.0/barbell2_castor/castor2sqlite.py` & `barbell2_castor-0.5.0/barbell2_castor/castor2sqlite.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,27 +146,45 @@
         finally:
             if conn:
                 conn.close()
 
     def execute(self):
         self.create_sql_database(self.data)
         return self.output_db_file
+    
+
+class CastorToSqlite3:
+
+    def __init__(
+            self,
+            study_name,
+            client_id,
+            client_secret,
+            output_db_file='castor.db',
+            add_timestamp=False,
+            log_level=logging.INFO, 
+            ):
+        self.castor2dict = CastorToDict(study_name, client_id, client_secret, log_level)        
+        self.output_db_file = output_db_file
+        self.add_timestamp = add_timestamp        
+        self.log_level = log_level
+        logging.root.setLevel(self.log_level)
+
+    def execute(self):
+        data = self.castor2dict.execute()
+        dict2sqlite = DictToSqlite3(data, self.output_db_file, self.add_timestamp, self.log_level)
+        return dict2sqlite.execute()
 
 
 if __name__ == '__main__':
     def main():
-        c2d = CastorToDict(
+        extractor = CastorToSqlite3(
             study_name='ESPRESSO_v2.0_DPCA',
             client_id=open(os.path.join(os.environ['HOME'], 'castorclientid.txt')).readline().strip(),
             client_secret=open(os.path.join(os.environ['HOME'], 'castorclientsecret.txt')).readline().strip(),
-            log_level=logging.INFO,
-        )
-        data = c2d.execute()
-        d2q = DictToSqlite3(
-            data=data,
             output_db_file='castor.db',
             add_timestamp=False,
             log_level=logging.INFO,
         )
-        db_file = d2q.execute()
+        db_file = extractor.execute()
         print(db_file)
     main()
```

### Comparing `barbell2_castor-0.4.0/barbell2_castor/query.py` & `barbell2_castor-0.5.0/barbell2_castor/query.py`

 * *Files identical despite different names*

### Comparing `barbell2_castor-0.4.0/barbell2_castor/utils.py` & `barbell2_castor-0.5.0/barbell2_castor/utils.py`

 * *Files identical despite different names*

### Comparing `barbell2_castor-0.4.0/barbell2_castor.egg-info/PKG-INFO` & `barbell2_castor-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
-Name: barbell2-castor
-Version: 0.4.0
+Name: barbell2_castor
+Version: 0.5.0
 Summary: Utilities for interfacing with Castor EDC
 Home-page: https://github.com/rbrecheisen/barbell2_castor
 Author: Ralph Brecheisen
 Author-email: r.brecheisen@maastrichtuniversity.nl
 License: MIT license
 Description: UNKNOWN
 Keywords: barbell2_castor
```

### Comparing `barbell2_castor-0.4.0/setup.py` & `barbell2_castor-0.5.0/setup.py`

 * *Files identical despite different names*

