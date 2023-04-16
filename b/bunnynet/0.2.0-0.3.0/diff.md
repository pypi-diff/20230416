# Comparing `tmp/bunnynet-0.2.0.tar.gz` & `tmp/bunnynet-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bunnynet-0.2.0.tar", max compression
+gzip compressed data, was "bunnynet-0.3.0.tar", max compression
```

## Comparing `bunnynet-0.2.0.tar` & `bunnynet-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1061 2023-04-16 12:03:51.759701 bunnynet-0.2.0/LICENSE
--rw-r--r--   0        0        0       12 2023-04-16 12:03:51.759701 bunnynet-0.2.0/README.md
--rw-r--r--   0        0        0      106 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/__init__.py
--rw-r--r--   0        0        0     6086 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/client.py
--rw-r--r--   0        0        0      360 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/exceptions.py
--rw-r--r--   0        0        0      275 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/hashing.py
--rw-r--r--   0        0        0     8989 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/httpclient.py
--rw-r--r--   0        0        0     1975 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/log_client.py
--rw-r--r--   0        0        0      138 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/__init__.py
--rw-r--r--   0        0        0      111 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/bunny_ai_image_blueprint.py
--rw-r--r--   0        0        0      860 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/edge_rule.py
--rw-r--r--   0        0        0      515 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/edge_rule_action_type.py
--rw-r--r--   0        0        0      590 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/edge_rule_trigger.py
--rw-r--r--   0        0        0      219 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/edge_rule_trigger_type.py
--rw-r--r--   0        0        0      732 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/hostname.py
--rw-r--r--   0        0        0      107 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/pattern_matching_type.py
--rw-r--r--   0        0        0    15739 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/pull_zone.py
--rw-r--r--   0        0        0       76 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/pull_zone_type.py
--rw-r--r--   0        0        0      969 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/storage_object.py
--rw-r--r--   0        0        0     1905 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/storage_zone.py
--rw-r--r--   0        0        0      107 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/trigger_matching_type.py
--rw-r--r--   0        0        0     1748 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/pull_zone_client.py
--rw-r--r--   0        0        0     1127 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/storage_endpoints.py
--rw-r--r--   0        0        0     8007 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/storage_zone_client.py
--rw-r--r--   0        0        0     1307 2023-04-16 12:03:51.759701 bunnynet-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 bunnynet-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-16 12:25:46.125018 bunnynet-0.3.0/LICENSE
+-rw-r--r--   0        0        0       12 2023-04-16 12:25:46.125018 bunnynet-0.3.0/README.md
+-rw-r--r--   0        0        0      106 2023-04-16 12:25:46.125018 bunnynet-0.3.0/bunnynet/__init__.py
+-rw-r--r--   0        0        0     6086 2023-04-16 12:25:46.125018 bunnynet-0.3.0/bunnynet/client.py
+-rw-r--r--   0        0        0     2050 2023-04-16 12:25:46.125018 bunnynet-0.3.0/bunnynet/exceptions.py
+-rw-r--r--   0        0        0      275 2023-04-16 12:25:46.125018 bunnynet-0.3.0/bunnynet/hashing.py
+-rw-r--r--   0        0        0     8980 2023-04-16 12:25:46.125018 bunnynet-0.3.0/bunnynet/httpclient.py
+-rw-r--r--   0        0        0     1975 2023-04-16 12:25:46.125018 bunnynet-0.3.0/bunnynet/log_client.py
+-rw-r--r--   0        0        0      138 2023-04-16 12:25:46.125018 bunnynet-0.3.0/bunnynet/models/__init__.py
+-rw-r--r--   0        0        0      111 2023-04-16 12:25:46.125018 bunnynet-0.3.0/bunnynet/models/bunny_ai_image_blueprint.py
+-rw-r--r--   0        0        0      860 2023-04-16 12:25:46.125018 bunnynet-0.3.0/bunnynet/models/edge_rule.py
+-rw-r--r--   0        0        0      515 2023-04-16 12:25:46.125018 bunnynet-0.3.0/bunnynet/models/edge_rule_action_type.py
+-rw-r--r--   0        0        0      590 2023-04-16 12:25:46.125018 bunnynet-0.3.0/bunnynet/models/edge_rule_trigger.py
+-rw-r--r--   0        0        0      219 2023-04-16 12:25:46.125018 bunnynet-0.3.0/bunnynet/models/edge_rule_trigger_type.py
+-rw-r--r--   0        0        0      732 2023-04-16 12:25:46.125018 bunnynet-0.3.0/bunnynet/models/hostname.py
+-rw-r--r--   0        0        0      107 2023-04-16 12:25:46.125018 bunnynet-0.3.0/bunnynet/models/pattern_matching_type.py
+-rw-r--r--   0        0        0    15739 2023-04-16 12:25:46.125018 bunnynet-0.3.0/bunnynet/models/pull_zone.py
+-rw-r--r--   0        0        0       76 2023-04-16 12:25:46.125018 bunnynet-0.3.0/bunnynet/models/pull_zone_type.py
+-rw-r--r--   0        0        0      969 2023-04-16 12:25:46.125018 bunnynet-0.3.0/bunnynet/models/storage_object.py
+-rw-r--r--   0        0        0     1905 2023-04-16 12:25:46.125018 bunnynet-0.3.0/bunnynet/models/storage_zone.py
+-rw-r--r--   0        0        0      107 2023-04-16 12:25:46.125018 bunnynet-0.3.0/bunnynet/models/trigger_matching_type.py
+-rw-r--r--   0        0        0     1748 2023-04-16 12:25:46.125018 bunnynet-0.3.0/bunnynet/pull_zone_client.py
+-rw-r--r--   0        0        0     1127 2023-04-16 12:25:46.125018 bunnynet-0.3.0/bunnynet/storage_endpoints.py
+-rw-r--r--   0        0        0     8007 2023-04-16 12:25:46.125018 bunnynet-0.3.0/bunnynet/storage_zone_client.py
+-rw-r--r--   0        0        0     1307 2023-04-16 12:25:46.129018 bunnynet-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 bunnynet-0.3.0/PKG-INFO
```

### Comparing `bunnynet-0.2.0/LICENSE` & `bunnynet-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bunnynet-0.2.0/bunnynet/client.py` & `bunnynet-0.3.0/bunnynet/client.py`

 * *Files identical despite different names*

### Comparing `bunnynet-0.2.0/bunnynet/httpclient.py` & `bunnynet-0.3.0/bunnynet/httpclient.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import urllib.parse
 from typing import Any, Iterator, Type, TypeVar, cast
 
 import deserialize
 import requests
 
 from bunnynet.exceptions import BunnyHTTPException
-from bunnynet.storage_endpoints import StorageEndpoint
 
 BASE_URL = "api.bunny.net"
 
 T = TypeVar("T")
 
 
 class HttpClient:
@@ -39,15 +38,15 @@
         :raises BunnyHTTPException: On any failure to validate
 
         :returns: Any data in the response
         """
         _ = self
 
         if not response.ok:
-            raise BunnyHTTPException(response)
+            raise BunnyHTTPException.generate_from_response(response)
 
         return response.json()
 
     def get_raw(
         self,
         endpoint: str,
         *,
@@ -77,15 +76,15 @@
             timeout=10,
         )
 
         if not raw_response.ok:
             if attempts > 1 and (raw_response.status_code >= 500):
                 return self.get_raw(endpoint, attempts=attempts - 1)
 
-            raise BunnyHTTPException(raw_response, "Failed to get data")
+            raise BunnyHTTPException.generate_from_response(raw_response, "Failed to get data")
 
         return raw_response.content
 
     def get(
         self,
         endpoint: str,
         response_type: Type[T],
```

### Comparing `bunnynet-0.2.0/bunnynet/log_client.py` & `bunnynet-0.3.0/bunnynet/log_client.py`

 * *Files identical despite different names*

### Comparing `bunnynet-0.2.0/bunnynet/models/edge_rule.py` & `bunnynet-0.3.0/bunnynet/models/edge_rule.py`

 * *Files identical despite different names*

### Comparing `bunnynet-0.2.0/bunnynet/models/edge_rule_action_type.py` & `bunnynet-0.3.0/bunnynet/models/edge_rule_action_type.py`

 * *Files identical despite different names*

### Comparing `bunnynet-0.2.0/bunnynet/models/edge_rule_trigger.py` & `bunnynet-0.3.0/bunnynet/models/edge_rule_trigger.py`

 * *Files identical despite different names*

### Comparing `bunnynet-0.2.0/bunnynet/models/hostname.py` & `bunnynet-0.3.0/bunnynet/models/hostname.py`

 * *Files identical despite different names*

### Comparing `bunnynet-0.2.0/bunnynet/models/pull_zone.py` & `bunnynet-0.3.0/bunnynet/models/pull_zone.py`

 * *Files identical despite different names*

### Comparing `bunnynet-0.2.0/bunnynet/models/storage_object.py` & `bunnynet-0.3.0/bunnynet/models/storage_object.py`

 * *Files identical despite different names*

### Comparing `bunnynet-0.2.0/bunnynet/models/storage_zone.py` & `bunnynet-0.3.0/bunnynet/models/storage_zone.py`

 * *Files identical despite different names*

### Comparing `bunnynet-0.2.0/bunnynet/pull_zone_client.py` & `bunnynet-0.3.0/bunnynet/pull_zone_client.py`

 * *Files identical despite different names*

### Comparing `bunnynet-0.2.0/bunnynet/storage_endpoints.py` & `bunnynet-0.3.0/bunnynet/storage_endpoints.py`

 * *Files identical despite different names*

### Comparing `bunnynet-0.2.0/bunnynet/storage_zone_client.py` & `bunnynet-0.3.0/bunnynet/storage_zone_client.py`

 * *Files identical despite different names*

### Comparing `bunnynet-0.2.0/pyproject.toml` & `bunnynet-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bunnynet"
-version = "0.2.0"
+version = "0.3.0"
 description = "A client for the bunny.net APIs"
 
 license = "MIT"
 
 authors = [
     "Dale Myers <dale@myers.io>"
 ]
```

### Comparing `bunnynet-0.2.0/PKG-INFO` & `bunnynet-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bunnynet
-Version: 0.2.0
+Version: 0.3.0
 Summary: A client for the bunny.net APIs
 Home-page: https://github.com/dalemyers/bunnynet
 License: MIT
 Keywords: bunny,bunny.net,cdn
 Author: Dale Myers
 Author-email: dale@myers.io
 Requires-Python: >=3.10,<4.0
```

