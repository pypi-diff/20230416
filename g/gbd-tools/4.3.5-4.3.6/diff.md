# Comparing `tmp/gbd_tools-4.3.5.tar.gz` & `tmp/gbd_tools-4.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbd_tools-4.3.5.tar", last modified: Wed Feb 15 10:31:48 2023, max compression
+gzip compressed data, was "gbd_tools-4.3.6.tar", last modified: Sun Apr 16 13:27:40 2023, max compression
```

## Comparing `gbd_tools-4.3.5.tar` & `gbd_tools-4.3.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 10:31:48.890116 gbd_tools-4.3.5/
--rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.3.5/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.3.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3757 2023-02-15 10:31:48.890116 gbd_tools-4.3.5/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3248 2023-02-07 16:30:01.000000 gbd_tools-4.3.5/README.md
--rwxrwxr-x   0 root         (0) root         (0)    10950 2023-02-07 16:30:01.000000 gbd_tools-4.3.5/gbd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 10:31:48.882116 gbd_tools-4.3.5/gbd_core/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.3.5/gbd_core/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8294 2023-02-07 16:30:01.000000 gbd_tools-4.3.5/gbd_core/api.py
--rw-rw-r--   0 root         (0) root         (0)     1151 2023-01-02 08:37:48.000000 gbd_tools-4.3.5/gbd_core/contexts.py
--rw-rw-r--   0 root         (0) root         (0)    10046 2023-01-09 18:14:00.000000 gbd_tools-4.3.5/gbd_core/database.py
--rw-rw-r--   0 root         (0) root         (0)     5050 2023-02-07 16:30:01.000000 gbd_tools-4.3.5/gbd_core/grammar.py
--rw-rw-r--   0 root         (0) root         (0)     5479 2023-01-09 18:14:00.000000 gbd_tools-4.3.5/gbd_core/query.py
--rw-rw-r--   0 root         (0) root         (0)    12287 2023-02-15 10:31:38.000000 gbd_tools-4.3.5/gbd_core/schema.py
--rw-rw-r--   0 root         (0) root         (0)     4628 2023-01-02 08:38:26.000000 gbd_tools-4.3.5/gbd_core/util.py
--rw-rw-r--   0 root         (0) root         (0)     3355 2023-01-05 08:44:08.000000 gbd_tools-4.3.5/gbd_core/util_argparse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 10:31:48.882116 gbd_tools-4.3.5/gbd_init/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.3.5/gbd_init/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7676 2023-01-05 09:18:19.000000 gbd_tools-4.3.5/gbd_init/cnf_extractors.py
--rw-rw-r--   0 root         (0) root         (0)     3853 2023-01-05 10:39:03.000000 gbd_tools-4.3.5/gbd_init/cnf_transformers.py
--rw-rw-r--   0 root         (0) root         (0)     2033 2023-01-02 08:38:45.000000 gbd_tools-4.3.5/gbd_init/gbdhash.py
--rw-rw-r--   0 root         (0) root         (0)     3458 2023-01-05 09:55:11.000000 gbd_tools-4.3.5/gbd_init/initializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 10:31:48.882116 gbd_tools-4.3.5/gbd_server/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.3.5/gbd_server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 10:31:48.882116 gbd_tools-4.3.5/gbd_server/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 10:31:48.886116 gbd_tools-4.3.5/gbd_server/static/img/
--rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.3.5/gbd_server/static/img/gbd_logo.jpg
--rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.3.5/gbd_server/static/img/gbd_logo.png
--rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.3.5/gbd_server/static/img/gbd_logo_small.png
--rw-rw-r--   0 root         (0) root         (0)     1737 2022-12-19 19:01:08.000000 gbd_tools-4.3.5/gbd_server/static/main.css
--rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.3.5/gbd_server/static/w3.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 10:31:48.886116 gbd_tools-4.3.5/gbd_server/templates/
--rw-rw-r--   0 root         (0) root         (0)     4068 2023-02-10 15:21:05.000000 gbd_tools-4.3.5/gbd_server/templates/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 10:31:48.890116 gbd_tools-4.3.5/gbd_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3757 2023-02-15 10:31:48.000000 gbd_tools-4.3.5/gbd_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      772 2023-02-15 10:31:48.000000 gbd_tools-4.3.5/gbd_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-15 10:31:48.000000 gbd_tools-4.3.5/gbd_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-02-15 10:31:48.000000 gbd_tools-4.3.5/gbd_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-02-15 10:31:48.000000 gbd_tools-4.3.5/gbd_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-02-15 10:31:48.000000 gbd_tools-4.3.5/gbd_tools.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)    12040 2023-02-10 15:21:05.000000 gbd_tools-4.3.5/server.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-15 10:31:48.890116 gbd_tools-4.3.5/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     1034 2023-02-15 10:31:38.000000 gbd_tools-4.3.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:27:40.510542 gbd_tools-4.3.6/
+-rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.3.6/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.3.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-04-16 13:27:40.510542 gbd_tools-4.3.6/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3248 2023-02-07 16:30:01.000000 gbd_tools-4.3.6/README.md
+-rwxrwxr-x   0 root         (0) root         (0)    10950 2023-02-07 16:30:01.000000 gbd_tools-4.3.6/gbd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:27:40.506542 gbd_tools-4.3.6/gbd_core/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.3.6/gbd_core/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8294 2023-02-07 16:30:01.000000 gbd_tools-4.3.6/gbd_core/api.py
+-rw-rw-r--   0 root         (0) root         (0)     1151 2023-01-02 08:37:48.000000 gbd_tools-4.3.6/gbd_core/contexts.py
+-rw-rw-r--   0 root         (0) root         (0)    10046 2023-02-15 10:46:17.000000 gbd_tools-4.3.6/gbd_core/database.py
+-rw-rw-r--   0 root         (0) root         (0)     5050 2023-02-07 16:30:01.000000 gbd_tools-4.3.6/gbd_core/grammar.py
+-rw-rw-r--   0 root         (0) root         (0)     5479 2023-01-09 18:14:00.000000 gbd_tools-4.3.6/gbd_core/query.py
+-rw-rw-r--   0 root         (0) root         (0)    12347 2023-02-15 10:51:41.000000 gbd_tools-4.3.6/gbd_core/schema.py
+-rw-rw-r--   0 root         (0) root         (0)     4628 2023-01-02 08:38:26.000000 gbd_tools-4.3.6/gbd_core/util.py
+-rw-rw-r--   0 root         (0) root         (0)     3355 2023-01-05 08:44:08.000000 gbd_tools-4.3.6/gbd_core/util_argparse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:27:40.506542 gbd_tools-4.3.6/gbd_init/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.3.6/gbd_init/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7676 2023-01-05 09:18:19.000000 gbd_tools-4.3.6/gbd_init/cnf_extractors.py
+-rw-rw-r--   0 root         (0) root         (0)     3853 2023-01-05 10:39:03.000000 gbd_tools-4.3.6/gbd_init/cnf_transformers.py
+-rw-rw-r--   0 root         (0) root         (0)     2033 2023-01-02 08:38:45.000000 gbd_tools-4.3.6/gbd_init/gbdhash.py
+-rw-rw-r--   0 root         (0) root         (0)     3458 2023-01-05 09:55:11.000000 gbd_tools-4.3.6/gbd_init/initializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:27:40.506542 gbd_tools-4.3.6/gbd_server/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.3.6/gbd_server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:27:40.506542 gbd_tools-4.3.6/gbd_server/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:27:40.510542 gbd_tools-4.3.6/gbd_server/static/img/
+-rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.3.6/gbd_server/static/img/gbd_logo.jpg
+-rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.3.6/gbd_server/static/img/gbd_logo.png
+-rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.3.6/gbd_server/static/img/gbd_logo_small.png
+-rw-rw-r--   0 root         (0) root         (0)     1737 2022-12-19 19:01:08.000000 gbd_tools-4.3.6/gbd_server/static/main.css
+-rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.3.6/gbd_server/static/w3.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:27:40.510542 gbd_tools-4.3.6/gbd_server/templates/
+-rw-rw-r--   0 root         (0) root         (0)     4190 2023-04-16 13:00:14.000000 gbd_tools-4.3.6/gbd_server/templates/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:27:40.510542 gbd_tools-4.3.6/gbd_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-04-16 13:27:40.000000 gbd_tools-4.3.6/gbd_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      772 2023-04-16 13:27:40.000000 gbd_tools-4.3.6/gbd_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 13:27:40.000000 gbd_tools-4.3.6/gbd_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-04-16 13:27:40.000000 gbd_tools-4.3.6/gbd_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-04-16 13:27:40.000000 gbd_tools-4.3.6/gbd_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-16 13:27:40.000000 gbd_tools-4.3.6/gbd_tools.egg-info/top_level.txt
+-rwxrwxr-x   0 root         (0) root         (0)    12040 2023-02-10 15:21:05.000000 gbd_tools-4.3.6/server.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 13:27:40.510542 gbd_tools-4.3.6/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1034 2023-04-16 13:27:36.000000 gbd_tools-4.3.6/setup.py
```

### Comparing `gbd_tools-4.3.5/LICENSE` & `gbd_tools-4.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.3.5/PKG-INFO` & `gbd_tools-4.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd_tools
-Version: 4.3.5
+Version: 4.3.6
 Summary: GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser, Karlsruhe Institute of Technology (KIT)
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.3.5/README.md` & `gbd_tools-4.3.6/README.md`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.3.5/gbd.py` & `gbd_tools-4.3.6/gbd.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.3.5/gbd_core/api.py` & `gbd_tools-4.3.6/gbd_core/api.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.3.5/gbd_core/contexts.py` & `gbd_tools-4.3.6/gbd_core/contexts.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.3.5/gbd_core/database.py` & `gbd_tools-4.3.6/gbd_core/database.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.3.5/gbd_core/grammar.py` & `gbd_tools-4.3.6/gbd_core/grammar.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.3.5/gbd_core/query.py` & `gbd_tools-4.3.6/gbd_core/query.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.3.5/gbd_core/schema.py` & `gbd_tools-4.3.6/gbd_core/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,21 +36,23 @@
     table: str = None
     column: str = None
     default: str = None
 
 
 class Schema:
 
-    IN_MEMORY_DB_NAME = "in_memory"
+    # in-memory database name for CSV files is always "main"
+    IN_MEMORY_DB_NAME = "main"
 
-    def __init__(self, dbname, path, features, context):
+    def __init__(self, dbcon, dbname, path, features, context):
         self.dbname = dbname
         self.path = path
         self.features = features
         self.context = context
+        self.dbcon = dbcon
 
     @classmethod
     def is_database(cls, path):
         if not os.path.isfile(path): 
             eprint("Creating Database {}".format(path))
             sqlite3.connect(path).close()
             return True
@@ -71,26 +73,24 @@
             raise SchemaException(str(e))
 
     @classmethod
     def from_database(cls, path):
         dbname = cls.dbname_from_path(path)
         con = sqlite3.connect(path)
         features = cls.features_from_database(dbname, path, con)
-        con.close()
         context = cls.context_from_database(dbname)
-        return cls(dbname, path, features, context)
+        return cls(con, dbname, path, features, context)
 
     @classmethod
     def from_csv(cls, path):
         dbname = cls.IN_MEMORY_DB_NAME
         con = sqlite3.connect("file::memory:?cache=shared", uri=True)
         features = cls.features_from_csv(dbname, path, con)
-        con.close()
         context = cls.context_from_csv(dbname)
-        return cls(dbname, path, features, context)
+        return cls(con, dbname, path, features, context)
 
     # Import CSV to in-memory db, create according schema info
     @classmethod
     def features_from_csv(cls, dbname, path, con) -> typing.Dict[str, FeatureInfo]:
         features = dict()
         with open(path) as csvfile:
             csvreader = csv.DictReader(csvfile)
```

### Comparing `gbd_tools-4.3.5/gbd_core/util.py` & `gbd_tools-4.3.6/gbd_core/util.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.3.5/gbd_core/util_argparse.py` & `gbd_tools-4.3.6/gbd_core/util_argparse.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.3.5/gbd_init/cnf_extractors.py` & `gbd_tools-4.3.6/gbd_init/cnf_extractors.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.3.5/gbd_init/cnf_transformers.py` & `gbd_tools-4.3.6/gbd_init/cnf_transformers.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.3.5/gbd_init/gbdhash.py` & `gbd_tools-4.3.6/gbd_init/gbdhash.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.3.5/gbd_init/initializer.py` & `gbd_tools-4.3.6/gbd_init/initializer.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.3.5/gbd_server/static/img/gbd_logo.jpg` & `gbd_tools-4.3.6/gbd_server/static/img/gbd_logo.jpg`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.3.5/gbd_server/static/img/gbd_logo.png` & `gbd_tools-4.3.6/gbd_server/static/img/gbd_logo.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.3.5/gbd_server/static/img/gbd_logo_small.png` & `gbd_tools-4.3.6/gbd_server/static/img/gbd_logo_small.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.3.5/gbd_server/static/main.css` & `gbd_tools-4.3.6/gbd_server/static/main.css`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.3.5/gbd_server/static/w3.js` & `gbd_tools-4.3.6/gbd_server/static/w3.js`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.3.5/gbd_server/templates/index.html` & `gbd_tools-4.3.6/gbd_server/templates/index.html`

 * *Files 12% similar despite different names*

```diff
@@ -26,21 +26,23 @@
                 {% endfor %}
             </fieldset>
             <br />
             <fieldset>
                 <legend>Filter for specific instances</legend>
                 <input type="text" name="query" class="query" placeholder="Query for Instances" value="{{ query }}">
                 <button type="submit" class="submit" formaction="/" name="action" value="show" title="Query for instances and selected features">Show</button>
-                <button type="submit" class="submit" formaction="/getinstances" form="mainform" name="action" value="download" title="Download $file. Download instances with 'wget --content-disposition -i $file'">Download</button>
+                <button type="submit" class="submit" formaction="/getinstances" name="action" value="download" title="Download $file">Download</button>
                 <br />
                 Query Shortcuts: <a href="{{ url_for('quick_search', track='main_2022') }}">Main 2022</a>, <a href="{{ url_for('quick_search', track='anni_2022') }}">Anniversary 2022</a>
             </fieldset>
             <br />
             <div class="info">
-                Found {{ total }} Benchmark Instances.
+                Found {{ total }} Benchmark Instances. 
+                Click on "Download" to get a text file with the selected instances URLs. 
+                Use this file to fetch the instances, e.g., using <b>wget --content-disposition -i $file</b>.
             </div>
         </form>
     </header>
     
     <div class="content">
         <table>
             <tr>
```

#### html2text {}

```diff
@@ -1,14 +1,16 @@
 
  [GBD-Logo]
  Select feature database for display {% for dbname in databases %} {% if dbname
 == selected %} # {% else %} o {% endif %} {{_dbname_}} {% endfor %}
  Filter for specific instances [{{ query }}         ] Show Download
 Query Shortcuts: Main_2022, Anniversary_2022
-Found {{ total }} Benchmark Instances.
+Found {{ total }} Benchmark Instances. Click on "Download" to get a text file
+with the selected instances URLs. Use this file to fetch the instances, e.g.,
+using wget --content-disposition -i $file.
 hash       {{ feature }}
 {{_item_}} {{_item_}}    {{ item }}
 {% if pages > 0 %} Showing 1000 of {{ total }} instances. Select page: {% for i
 in range(0, pages) %} {% if i == page %} {{ i + 1 }} {% else %} {{ i + 1 }} {%
 endif %} {% endfor %} {% else %} Found {{ total }} instances. {% endif %}
 If you find this useful, please cite: A_Problem_Meta-Data_Library_for_Research
 in_SAT
```

### Comparing `gbd_tools-4.3.5/gbd_tools.egg-info/PKG-INFO` & `gbd_tools-4.3.6/gbd_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd-tools
-Version: 4.3.5
+Version: 4.3.6
 Summary: GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser, Karlsruhe Institute of Technology (KIT)
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.3.5/gbd_tools.egg-info/SOURCES.txt` & `gbd_tools-4.3.6/gbd_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.3.5/server.py` & `gbd_tools-4.3.6/server.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.3.5/setup.py` & `gbd_tools-4.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='gbd_tools',
-  version='4.3.5',
+  version='4.3.6',
   description='GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes',
   long_description=open('README.md', 'rt').read(),
   long_description_content_type="text/markdown",
   url='https://github.com/Udopia/gbd',
   author='Markus Iser, Karlsruhe Institute of Technology (KIT)',
   author_email='markus.iser@kit.edu',
   packages=[
```

