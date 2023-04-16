# Comparing `tmp/Hunabku_siiu-0.0.1.tar.gz` & `tmp/Hunabku_siiu-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hunabku_siiu-0.0.1.tar", last modified: Thu Mar 30 18:05:34 2023, max compression
+gzip compressed data, was "Hunabku_siiu-0.0.2.tar", last modified: Sun Apr 16 08:07:16 2023, max compression
```

## Comparing `Hunabku_siiu-0.0.1.tar` & `Hunabku_siiu-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:05:34.418580 Hunabku_siiu-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:05:34.418580 Hunabku_siiu-0.0.1/Hunabku_siiu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-03-30 18:05:34.000000 Hunabku_siiu-0.0.1/Hunabku_siiu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-30 18:05:34.000000 Hunabku_siiu-0.0.1/Hunabku_siiu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 18:05:34.000000 Hunabku_siiu-0.0.1/Hunabku_siiu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 18:05:34.000000 Hunabku_siiu-0.0.1/Hunabku_siiu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-30 18:05:34.000000 Hunabku_siiu-0.0.1/Hunabku_siiu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-30 18:05:17.000000 Hunabku_siiu-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-03-30 18:05:34.418580 Hunabku_siiu-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-03-30 18:05:17.000000 Hunabku_siiu-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:05:34.418580 Hunabku_siiu-0.0.1/hunabku_siiu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 18:05:17.000000 Hunabku_siiu-0.0.1/hunabku_siiu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-30 18:05:17.000000 Hunabku_siiu-0.0.1/hunabku_siiu/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:05:34.418580 Hunabku_siiu-0.0.1/hunabku_siiu/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-03-30 18:05:17.000000 Hunabku_siiu-0.0.1/hunabku_siiu/endpoints/SIIU.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 18:05:34.418580 Hunabku_siiu-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-03-30 18:05:17.000000 Hunabku_siiu-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:07:16.570952 Hunabku_siiu-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:07:16.570952 Hunabku_siiu-0.0.2/Hunabku_siiu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-16 08:07:16.000000 Hunabku_siiu-0.0.2/Hunabku_siiu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-16 08:07:16.000000 Hunabku_siiu-0.0.2/Hunabku_siiu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 08:07:16.000000 Hunabku_siiu-0.0.2/Hunabku_siiu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-16 08:07:16.000000 Hunabku_siiu-0.0.2/Hunabku_siiu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-16 08:07:16.000000 Hunabku_siiu-0.0.2/Hunabku_siiu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-16 08:06:57.000000 Hunabku_siiu-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-16 08:07:16.570952 Hunabku_siiu-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-16 08:06:57.000000 Hunabku_siiu-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:07:16.570952 Hunabku_siiu-0.0.2/hunabku_siiu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 08:06:57.000000 Hunabku_siiu-0.0.2/hunabku_siiu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-16 08:06:57.000000 Hunabku_siiu-0.0.2/hunabku_siiu/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:07:16.570952 Hunabku_siiu-0.0.2/hunabku_siiu/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-04-16 08:06:57.000000 Hunabku_siiu-0.0.2/hunabku_siiu/endpoints/SIIU.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 08:07:16.570952 Hunabku_siiu-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-16 08:06:57.000000 Hunabku_siiu-0.0.2/setup.py
```

### Comparing `Hunabku_siiu-0.0.1/Hunabku_siiu.egg-info/PKG-INFO` & `Hunabku_siiu-0.0.2/Hunabku_siiu.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hunabku-siiu
-Version: 0.0.1
+Version: 0.0.2
 Summary: Hunabku plguin
 Home-page: https://github.com/colav/Hunabku_plugins
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
```

### Comparing `Hunabku_siiu-0.0.1/PKG-INFO` & `Hunabku_siiu-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hunabku_siiu
-Version: 0.0.1
+Version: 0.0.2
 Summary: Hunabku plguin
 Home-page: https://github.com/colav/Hunabku_plugins
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
```

### Comparing `Hunabku_siiu-0.0.1/README.md` & `Hunabku_siiu-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `Hunabku_siiu-0.0.1/hunabku_siiu/endpoints/SIIU.py` & `Hunabku_siiu-0.0.2/hunabku_siiu/endpoints/SIIU.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 from hunabku.HunabkuBase import HunabkuPluginBase, endpoint
 from hunabku.Config import Config, Param
 from pymongo import MongoClient
-
+from elasticsearch import Elasticsearch, helpers
+from elasticsearch_dsl import Search
+import time
 
 class SIIU(HunabkuPluginBase):
     config = Config()
-    config += Param(db_uri="mongodb://localhost:27017/",
+    config += Param(mdb_uri="mongodb://localhost:27017/",
                     doc="MongoDB string connection")
-    config += Param(db_name="siiu",
+    config += Param(mdb_name="siiu",
                     doc="MongoDB name for SIIU")
+    config += Param(es_uri="http://localhost:9200",
+                    doc="Elastic Search url")
+    config += Param(es_user="elastic",
+                    doc="Elastic Search user")
+    config += Param(es_pass="colav",
+                    doc="Elastic Search password")
+    config += Param(es_project_index="siiu_project",
+                    doc="Elastic Search siiu project index name")
 
     def __init__(self, hunabku):
         super().__init__(hunabku)
-        self.dbclient = MongoClient(self.config.db_uri)
+        self.dbclient = MongoClient(self.config.mdb_uri)
+        basic_auth = (self.config.es_user, self.config.es_pass)
+        self.es = Elasticsearch(self.config.es_uri, basic_auth=basic_auth)
 
     @endpoint('/siiu/project', methods=['GET'])
     def siiu_project(self):
         """
         @api {get} /siiu/project Project
         @apiName Project
         @apiGroup SIIU
@@ -39,28 +51,65 @@
             # all the products for the user
             curl -i http://apis.colav.co/siiu/project?apikey=XXXX&search=keyword
             # An specific product
             curl -i http://apis.colav.co/siiu/project?apikey=XXXX&CODIGO=2013-86
 
         """
         if self.valid_apikey():
+
             keyword = self.request.args.get('search')
+            codigo = self.request.args.get('CODIGO')
             if keyword:
-                data = list(self.dbclient[self.config.db_name]["project"].find({
-                            "$text": {
-                                "$search": keyword,
-                                "$caseSensitive": False
-                            }
-                            }, {'_id': 0}))
+                if not self.es.indices.exists(index=self.config.es_project_index):
+                    response = self.app.response_class(
+                        response=self.json.dumps(
+                            {"msg": f"Internal error, index {self.config.es_project_index} not found in Elastic Search"}),
+                        status=500,
+                        mimetype='application/json'
+                    )
+                    return response
+                body = {"query": {
+                    "bool": {
+                        "should": [
+                            {"match": {"NOMBRE_CORTO":  keyword}},
+                            {"match": {"NOMBRE_COMPLETO": keyword}},
+                            {"match": {"PALABRAS_CLAVES": keyword}},
+                            {"match": {"descriptive_text.TEXTO_INGRESADO": keyword}}
+                        ]
+                    }
+                }
+                }
+                # get the start time
+                st = time.time()
+                s = Search(using=self.es, index=self.config.es_project_index)
+                s = s.update_from_dict(body)
+                s = s.extra(track_total_hits=True)
+                s.execute()
+                data = [hit.to_dict() for hit in s.scan()]
                 response = self.app.response_class(
                     response=self.json.dumps(data),
                     status=200,
                     mimetype='application/json'
                 )
+                # get the end time
+                et = time.time()
+                # get the execution time
+                elapsed_time = et - st
+                print(f'Search for "{keyword}" Execution time:', elapsed_time, 'seconds')
                 return response
+            if codigo:
+                data = list(self.dbclient[self.config.mdb_name]
+                            ["project"].find({'CODIGO': codigo}, {'_id': 0, }))
+                response = self.app.response_class(
+                    response=self.json.dumps(data),
+                    status=200,
+                    mimetype='application/json'
+                )
+                return response
+
             data = {
                 "error": "Bad Request", "message": "invalid parameters, please select the right combination of parameters."}
             response = self.app.response_class(
                 response=self.json.dumps(data),
                 status=400,
                 mimetype='application/json'
             )
```

### Comparing `Hunabku_siiu-0.0.1/setup.py` & `Hunabku_siiu-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,14 +78,17 @@
         long_description_content_type="text/markdown",
 
         # Dependent packages (distributions)
         # put you packages here
         install_requires=[
             'flask>=1.1.2',
             'requests>=2.22.0',
-            'hunabku'
+            'hunabku',
+            'pymongo',
+            'elasticsearch',
+            'elasticsearch_dsl',
         ],
     )
 
 
 if __name__ == "__main__":
     main()
```

