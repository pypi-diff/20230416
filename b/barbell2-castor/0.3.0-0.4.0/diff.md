# Comparing `tmp/barbell2_castor-0.3.0.tar.gz` & `tmp/barbell2_castor-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/barbell2_castor-0.3.0.tar", last modified: Sat Apr 15 21:53:44 2023, max compression
+gzip compressed data, was "dist/barbell2_castor-0.4.0.tar", last modified: Sat Apr 15 22:03:48 2023, max compression
```

## Comparing `barbell2_castor-0.3.0.tar` & `barbell2_castor-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 21:53:44.899058 barbell2_castor-0.3.0/
--rw-r--r--   0 ralph      (501) staff       (20)      784 2023-04-15 21:53:44.898802 barbell2_castor-0.3.0/PKG-INFO
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 21:53:44.896680 barbell2_castor-0.3.0/barbell2_castor/
--rw-r--r--   0 ralph      (501) staff       (20)      105 2023-04-15 21:53:40.000000 barbell2_castor-0.3.0/barbell2_castor/__init__.py
--rw-r--r--   0 ralph      (501) staff       (20)     9836 2023-04-15 21:52:42.000000 barbell2_castor-0.3.0/barbell2_castor/api.py
--rw-r--r--   0 ralph      (501) staff       (20)     8004 2023-04-15 21:51:29.000000 barbell2_castor-0.3.0/barbell2_castor/castor2sqlite.py
--rw-r--r--   0 ralph      (501) staff       (20)      628 2023-04-15 12:26:09.000000 barbell2_castor-0.3.0/barbell2_castor/utils.py
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 21:53:44.898385 barbell2_castor-0.3.0/barbell2_castor.egg-info/
--rw-r--r--   0 ralph      (501) staff       (20)      784 2023-04-15 21:53:44.000000 barbell2_castor-0.3.0/barbell2_castor.egg-info/PKG-INFO
--rw-r--r--   0 ralph      (501) staff       (20)      391 2023-04-15 21:53:44.000000 barbell2_castor-0.3.0/barbell2_castor.egg-info/SOURCES.txt
--rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-15 21:53:44.000000 barbell2_castor-0.3.0/barbell2_castor.egg-info/dependency_links.txt
--rw-r--r--   0 ralph      (501) staff       (20)       20 2023-04-15 21:53:44.000000 barbell2_castor-0.3.0/barbell2_castor.egg-info/entry_points.txt
--rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-15 12:23:48.000000 barbell2_castor-0.3.0/barbell2_castor.egg-info/not-zip-safe
--rw-r--r--   0 ralph      (501) staff       (20)       34 2023-04-15 21:53:44.000000 barbell2_castor-0.3.0/barbell2_castor.egg-info/requires.txt
--rw-r--r--   0 ralph      (501) staff       (20)       16 2023-04-15 21:53:44.000000 barbell2_castor-0.3.0/barbell2_castor.egg-info/top_level.txt
--rw-r--r--   0 ralph      (501) staff       (20)       38 2023-04-15 21:53:44.899133 barbell2_castor-0.3.0/setup.cfg
--rw-r--r--   0 ralph      (501) staff       (20)     1372 2023-04-15 12:28:09.000000 barbell2_castor-0.3.0/setup.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 22:03:48.590108 barbell2_castor-0.4.0/
+-rw-r--r--   0 ralph      (501) staff       (20)      784 2023-04-15 22:03:48.589865 barbell2_castor-0.4.0/PKG-INFO
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 22:03:48.588055 barbell2_castor-0.4.0/barbell2_castor/
+-rw-r--r--   0 ralph      (501) staff       (20)      105 2023-04-15 22:03:45.000000 barbell2_castor-0.4.0/barbell2_castor/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     9836 2023-04-15 21:52:42.000000 barbell2_castor-0.4.0/barbell2_castor/api.py
+-rw-r--r--   0 ralph      (501) staff       (20)     6005 2023-04-15 22:03:25.000000 barbell2_castor-0.4.0/barbell2_castor/castor2sqlite.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1630 2023-04-15 22:02:16.000000 barbell2_castor-0.4.0/barbell2_castor/query.py
+-rw-r--r--   0 ralph      (501) staff       (20)      628 2023-04-15 12:26:09.000000 barbell2_castor-0.4.0/barbell2_castor/utils.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 22:03:48.589559 barbell2_castor-0.4.0/barbell2_castor.egg-info/
+-rw-r--r--   0 ralph      (501) staff       (20)      784 2023-04-15 22:03:48.000000 barbell2_castor-0.4.0/barbell2_castor.egg-info/PKG-INFO
+-rw-r--r--   0 ralph      (501) staff       (20)      416 2023-04-15 22:03:48.000000 barbell2_castor-0.4.0/barbell2_castor.egg-info/SOURCES.txt
+-rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-15 22:03:48.000000 barbell2_castor-0.4.0/barbell2_castor.egg-info/dependency_links.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       20 2023-04-15 22:03:48.000000 barbell2_castor-0.4.0/barbell2_castor.egg-info/entry_points.txt
+-rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-15 12:23:48.000000 barbell2_castor-0.4.0/barbell2_castor.egg-info/not-zip-safe
+-rw-r--r--   0 ralph      (501) staff       (20)       34 2023-04-15 22:03:48.000000 barbell2_castor-0.4.0/barbell2_castor.egg-info/requires.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       16 2023-04-15 22:03:48.000000 barbell2_castor-0.4.0/barbell2_castor.egg-info/top_level.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       38 2023-04-15 22:03:48.590178 barbell2_castor-0.4.0/setup.cfg
+-rw-r--r--   0 ralph      (501) staff       (20)     1372 2023-04-15 12:28:09.000000 barbell2_castor-0.4.0/setup.py
```

### Comparing `barbell2_castor-0.3.0/PKG-INFO` & `barbell2_castor-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: barbell2_castor
-Version: 0.3.0
+Version: 0.4.0
 Summary: Utilities for interfacing with Castor EDC
 Home-page: https://github.com/rbrecheisen/barbell2_castor
 Author: Ralph Brecheisen
 Author-email: r.brecheisen@maastrichtuniversity.nl
 License: MIT license
 Description: UNKNOWN
 Keywords: barbell2_castor
```

### Comparing `barbell2_castor-0.3.0/barbell2_castor/api.py` & `barbell2_castor-0.4.0/barbell2_castor/api.py`

 * *Files identical despite different names*

### Comparing `barbell2_castor-0.3.0/barbell2_castor/castor2sqlite.py` & `barbell2_castor-0.4.0/barbell2_castor/castor2sqlite.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,29 +8,14 @@
 from barbell2_castor.api import CastorApiClient
 
 
 logging.basicConfig()
 logger = logging.getLogger(__name__)
 
 
-""" --------------------------------------------------
-Extract Castor data via API and stores in Python 
-dictionary. Dictionary has the following structure:
-
-    data = {
-        'dpca_idcode': [],
-        'dpca_typok$1': [],
-        'dpca_typok$2': [],
-        'dpca_typok$3': [],
-        ...
-    }
-
-where the different options of each option group gets its own
-column in the final table. 
-"""
 class CastorToDict:
 
     def __init__(
             self,
             study_name, 
             client_id, 
             client_secret, 
@@ -47,31 +32,23 @@
         client = CastorApiClient(self.client_id, self.client_secret)
         study = client.get_study(self.study_name)
         study_id = client.get_study_id(study)
         self.data = client.get_study_data(study_id)
         return self.data
 
 
-""" --------------------------------------------------
-Takes Castor data from Excel export file and stores it
-in Python dictionary.
-"""
 class CastorExcelToDict:
 
     def __init__(self):
         self.data = {}
 
     def execute(self):
         return self.data
 
 
-""" --------------------------------------------------
-Converts Python dictionary with Castor data to SQLite3
-format for easy querying.
-"""
 class DictToSqlite3:
 
     CASTOR_TO_SQL_TYPES = {
         'string': 'TEXT',
         'textarea': 'TEXT',
         'radio': 'TINYINT',
         'dropdown': 'TINYINT',
@@ -171,58 +148,14 @@
                 conn.close()
 
     def execute(self):
         self.create_sql_database(self.data)
         return self.output_db_file
 
 
-""" --------------------------------------------------
-"""
-class CastorQuery:
-
-    def __init__(self, db_file):
-        self.db = self.load_db(db_file)
-        self.output = None
-
-    def __del__(self):
-        if self.db:
-            self.db.close()
-            self.db = None
-
-    def load_db(self, db_file):
-        try:
-            db = sqlite3.connect(db_file)
-            return db
-        except sqlite3.Error as e:
-            logger.error(e)
-        return None
-
-    @staticmethod
-    def get_column_names(data):
-        column_names = []
-        for column in data.description:
-            column_names.append(column[0])
-        return column_names
-    
-    def to_csv(self, output_file):
-        self.output.to_csv(output_file, sep=';', index=False)
-
-    def execute(self, query):
-        self.output = None
-        cursor = self.db.cursor()
-        data = cursor.execute(query)
-        df_data = []
-        for result in data:
-            df_data.append(result)
-        self.output = pd.DataFrame(df_data, columns=self.get_column_names(data))        
-        return self.output
-
-
-""" --------------------------------------------------
-"""
 if __name__ == '__main__':
     def main():
         c2d = CastorToDict(
             study_name='ESPRESSO_v2.0_DPCA',
             client_id=open(os.path.join(os.environ['HOME'], 'castorclientid.txt')).readline().strip(),
             client_secret=open(os.path.join(os.environ['HOME'], 'castorclientsecret.txt')).readline().strip(),
             log_level=logging.INFO,
@@ -231,12 +164,9 @@
         d2q = DictToSqlite3(
             data=data,
             output_db_file='castor.db',
             add_timestamp=False,
             log_level=logging.INFO,
         )
         db_file = d2q.execute()
-        query_engine = CastorQuery(db_file)
-        df = query_engine.execute(
-            'SELECT dpca_idcode, dpca_typok$1, dpca_typok$2 FROM data WHERE dpca_typok$1 = 1;')
-        print(df.head())
+        print(db_file)
     main()
```

### Comparing `barbell2_castor-0.3.0/barbell2_castor/utils.py` & `barbell2_castor-0.4.0/barbell2_castor/utils.py`

 * *Files identical despite different names*

### Comparing `barbell2_castor-0.3.0/barbell2_castor.egg-info/PKG-INFO` & `barbell2_castor-0.4.0/barbell2_castor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: barbell2-castor
-Version: 0.3.0
+Version: 0.4.0
 Summary: Utilities for interfacing with Castor EDC
 Home-page: https://github.com/rbrecheisen/barbell2_castor
 Author: Ralph Brecheisen
 Author-email: r.brecheisen@maastrichtuniversity.nl
 License: MIT license
 Description: UNKNOWN
 Keywords: barbell2_castor
```

### Comparing `barbell2_castor-0.3.0/setup.py` & `barbell2_castor-0.4.0/setup.py`

 * *Files identical despite different names*

