# Comparing `tmp/artemis-common-0.3.1b0.tar.gz` & `tmp/artemis-common-0.3.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artemis-common-0.3.1b0.tar", last modified: Sat Apr 15 21:24:44 2023, max compression
+gzip compressed data, was "artemis-common-0.3.2b0.tar", last modified: Sun Apr 16 05:15:11 2023, max compression
```

## Comparing `artemis-common-0.3.1b0.tar` & `artemis-common-0.3.2b0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:24:44.817450 artemis-common-0.3.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-15 21:24:44.813450 artemis-common-0.3.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:24:44.813450 artemis-common-0.3.1b0/artemis_common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:24:44.813450 artemis-common-0.3.1b0/artemis_common/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/clients/async_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/clients/params_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/clients/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:24:44.813450 artemis-common-0.3.1b0/artemis_common/config/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/config/config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/config/pem.key
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/config/uvicorn_disable_logging.json
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/custom_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:24:44.813450 artemis-common-0.3.1b0/artemis_common/models/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/models/bases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:24:44.813450 artemis-common-0.3.1b0/artemis_common/models/dal/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/models/dal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/models/dal/fred.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/models/dal/user_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/models/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/models/model_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:24:44.813450 artemis-common-0.3.1b0/artemis_common/models/server/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/models/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/models/server/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/models/server/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:24:44.813450 artemis-common-0.3.1b0/artemis_common/server/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/server/exception_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:24:44.813450 artemis-common-0.3.1b0/artemis_common/server/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/server/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/server/middlewares/logging_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/server/swagger.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/server/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/artemis_common/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:24:44.813450 artemis-common-0.3.1b0/artemis_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-15 21:24:44.000000 artemis-common-0.3.1b0/artemis_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-15 21:24:44.000000 artemis-common-0.3.1b0/artemis_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 21:24:44.000000 artemis-common-0.3.1b0/artemis_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-15 21:24:44.000000 artemis-common-0.3.1b0/artemis_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-15 21:24:44.000000 artemis-common-0.3.1b0/artemis_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 21:24:44.817450 artemis-common-0.3.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-15 21:24:32.000000 artemis-common-0.3.1b0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-15 21:24:42.000000 artemis-common-0.3.1b0/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:15:11.673708 artemis-common-0.3.2b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-16 05:15:11.673708 artemis-common-0.3.2b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:15:11.669708 artemis-common-0.3.2b0/artemis_common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:15:11.669708 artemis-common-0.3.2b0/artemis_common/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/clients/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/clients/params_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/clients/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:15:11.669708 artemis-common-0.3.2b0/artemis_common/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/config/config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/config/pem.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/config/uvicorn_disable_logging.json
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/custom_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:15:11.669708 artemis-common-0.3.2b0/artemis_common/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/models/bases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:15:11.673708 artemis-common-0.3.2b0/artemis_common/models/dal/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/models/dal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/models/dal/fred.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/models/dal/user_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/models/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/models/model_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:15:11.673708 artemis-common-0.3.2b0/artemis_common/models/server/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/models/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/models/server/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/models/server/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:15:11.673708 artemis-common-0.3.2b0/artemis_common/server/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/server/exception_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:15:11.673708 artemis-common-0.3.2b0/artemis_common/server/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/server/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/server/middlewares/logging_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/server/swagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/artemis_common/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:15:11.669708 artemis-common-0.3.2b0/artemis_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-16 05:15:11.000000 artemis-common-0.3.2b0/artemis_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-16 05:15:11.000000 artemis-common-0.3.2b0/artemis_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 05:15:11.000000 artemis-common-0.3.2b0/artemis_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-16 05:15:11.000000 artemis-common-0.3.2b0/artemis_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-16 05:15:11.000000 artemis-common-0.3.2b0/artemis_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 05:15:11.673708 artemis-common-0.3.2b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-16 05:14:59.000000 artemis-common-0.3.2b0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-16 05:15:10.000000 artemis-common-0.3.2b0/version
```

### Comparing `artemis-common-0.3.1b0/artemis_common/clients/async_client.py` & `artemis-common-0.3.2b0/artemis_common/clients/async_client.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.3.1b0/artemis_common/clients/params_model.py` & `artemis-common-0.3.2b0/artemis_common/clients/params_model.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.3.1b0/artemis_common/config/config.py` & `artemis-common-0.3.2b0/artemis_common/config/config.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.3.1b0/artemis_common/config/config_loader.py` & `artemis-common-0.3.2b0/artemis_common/config/config_loader.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.3.1b0/artemis_common/config/uvicorn_disable_logging.json` & `artemis-common-0.3.2b0/artemis_common/config/uvicorn_disable_logging.json`

 * *Files identical despite different names*

### Comparing `artemis-common-0.3.1b0/artemis_common/consts.py` & `artemis-common-0.3.2b0/artemis_common/consts.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.3.1b0/artemis_common/custom_logging.py` & `artemis-common-0.3.2b0/artemis_common/custom_logging.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.3.1b0/artemis_common/exceptions.py` & `artemis-common-0.3.2b0/artemis_common/exceptions.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.3.1b0/artemis_common/logging.py` & `artemis-common-0.3.2b0/artemis_common/logging.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,13 +32,9 @@
             )
             body = HTTPLog([log_item])
 
             with ApiClient(self.configuration) as api_client:
                 api_instance = LogsApi(api_client)
                 api_instance.submit_log(content_encoding=ContentEncoding.GZIP, body=body)
 
-        except Exception as ex:
-            print(ex)
-            print(self.version)
-            print(self.service)
-            print(self.env)
+        except Exception:
             self.handleError(record)
```

### Comparing `artemis-common-0.3.1b0/artemis_common/models/bases.py` & `artemis-common-0.3.2b0/artemis_common/models/bases.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.3.1b0/artemis_common/models/dal/fred.py` & `artemis-common-0.3.2b0/artemis_common/models/dal/fred.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.3.1b0/artemis_common/models/jwt.py` & `artemis-common-0.3.2b0/artemis_common/models/jwt.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.3.1b0/artemis_common/models/model_parser.py` & `artemis-common-0.3.2b0/artemis_common/models/model_parser.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.3.1b0/artemis_common/models/server/response.py` & `artemis-common-0.3.2b0/artemis_common/models/server/response.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.3.1b0/artemis_common/server/exception_handlers.py` & `artemis-common-0.3.2b0/artemis_common/server/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.3.1b0/artemis_common/server/middlewares/logging_middleware.py` & `artemis-common-0.3.2b0/artemis_common/server/middlewares/logging_middleware.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.3.1b0/artemis_common/server/swagger.py` & `artemis-common-0.3.2b0/artemis_common/server/swagger.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.3.1b0/artemis_common/server/utils.py` & `artemis-common-0.3.2b0/artemis_common/server/utils.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.3.1b0/artemis_common/token.py` & `artemis-common-0.3.2b0/artemis_common/token.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.3.1b0/artemis_common.egg-info/SOURCES.txt` & `artemis-common-0.3.2b0/artemis_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `artemis-common-0.3.1b0/setup.py` & `artemis-common-0.3.2b0/setup.py`

 * *Files identical despite different names*

