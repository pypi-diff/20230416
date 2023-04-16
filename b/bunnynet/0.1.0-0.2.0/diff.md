# Comparing `tmp/bunnynet-0.1.0.tar.gz` & `tmp/bunnynet-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bunnynet-0.1.0.tar", max compression
+gzip compressed data, was "bunnynet-0.2.0.tar", max compression
```

## Comparing `bunnynet-0.1.0.tar` & `bunnynet-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1061 2023-04-15 16:59:51.124462 bunnynet-0.1.0/LICENSE
--rw-r--r--   0        0        0       12 2023-04-15 16:59:51.124462 bunnynet-0.1.0/README.md
--rw-r--r--   0        0        0      106 2023-04-15 16:59:51.124462 bunnynet-0.1.0/bunnynet/__init__.py
--rw-r--r--   0        0        0     5708 2023-04-15 16:59:51.124462 bunnynet-0.1.0/bunnynet/client.py
--rw-r--r--   0        0        0      360 2023-04-15 16:59:51.124462 bunnynet-0.1.0/bunnynet/exceptions.py
--rw-r--r--   0        0        0      275 2023-04-15 16:59:51.124462 bunnynet-0.1.0/bunnynet/hashing.py
--rw-r--r--   0        0        0     8734 2023-04-15 16:59:51.124462 bunnynet-0.1.0/bunnynet/httpclient.py
--rw-r--r--   0        0        0     1959 2023-04-15 16:59:51.124462 bunnynet-0.1.0/bunnynet/log_client.py
--rw-r--r--   0        0        0      138 2023-04-15 16:59:51.124462 bunnynet-0.1.0/bunnynet/models/__init__.py
--rw-r--r--   0        0        0      111 2023-04-15 16:59:51.124462 bunnynet-0.1.0/bunnynet/models/bunny_ai_image_blueprint.py
--rw-r--r--   0        0        0      860 2023-04-15 16:59:51.124462 bunnynet-0.1.0/bunnynet/models/edge_rule.py
--rw-r--r--   0        0        0      515 2023-04-15 16:59:51.124462 bunnynet-0.1.0/bunnynet/models/edge_rule_action_type.py
--rw-r--r--   0        0        0      590 2023-04-15 16:59:51.124462 bunnynet-0.1.0/bunnynet/models/edge_rule_trigger.py
--rw-r--r--   0        0        0      219 2023-04-15 16:59:51.124462 bunnynet-0.1.0/bunnynet/models/edge_rule_trigger_type.py
--rw-r--r--   0        0        0      732 2023-04-15 16:59:51.124462 bunnynet-0.1.0/bunnynet/models/hostname.py
--rw-r--r--   0        0        0      107 2023-04-15 16:59:51.124462 bunnynet-0.1.0/bunnynet/models/pattern_matching_type.py
--rw-r--r--   0        0        0    15739 2023-04-15 16:59:51.128462 bunnynet-0.1.0/bunnynet/models/pull_zone.py
--rw-r--r--   0        0        0       76 2023-04-15 16:59:51.128462 bunnynet-0.1.0/bunnynet/models/pull_zone_type.py
--rw-r--r--   0        0        0      969 2023-04-15 16:59:51.128462 bunnynet-0.1.0/bunnynet/models/storage_object.py
--rw-r--r--   0        0        0     1905 2023-04-15 16:59:51.128462 bunnynet-0.1.0/bunnynet/models/storage_zone.py
--rw-r--r--   0        0        0      107 2023-04-15 16:59:51.128462 bunnynet-0.1.0/bunnynet/models/trigger_matching_type.py
--rw-r--r--   0        0        0     1748 2023-04-15 16:59:51.128462 bunnynet-0.1.0/bunnynet/pull_zone_client.py
--rw-r--r--   0        0        0     1127 2023-04-15 16:59:51.128462 bunnynet-0.1.0/bunnynet/storage_endpoints.py
--rw-r--r--   0        0        0     6966 2023-04-15 16:59:51.128462 bunnynet-0.1.0/bunnynet/storage_zone_client.py
--rw-r--r--   0        0        0     1307 2023-04-15 16:59:51.128462 bunnynet-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 bunnynet-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-16 12:03:51.759701 bunnynet-0.2.0/LICENSE
+-rw-r--r--   0        0        0       12 2023-04-16 12:03:51.759701 bunnynet-0.2.0/README.md
+-rw-r--r--   0        0        0      106 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/__init__.py
+-rw-r--r--   0        0        0     6086 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/client.py
+-rw-r--r--   0        0        0      360 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/exceptions.py
+-rw-r--r--   0        0        0      275 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/hashing.py
+-rw-r--r--   0        0        0     8989 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/httpclient.py
+-rw-r--r--   0        0        0     1975 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/log_client.py
+-rw-r--r--   0        0        0      138 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/__init__.py
+-rw-r--r--   0        0        0      111 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/bunny_ai_image_blueprint.py
+-rw-r--r--   0        0        0      860 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/edge_rule.py
+-rw-r--r--   0        0        0      515 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/edge_rule_action_type.py
+-rw-r--r--   0        0        0      590 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/edge_rule_trigger.py
+-rw-r--r--   0        0        0      219 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/edge_rule_trigger_type.py
+-rw-r--r--   0        0        0      732 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/hostname.py
+-rw-r--r--   0        0        0      107 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/pattern_matching_type.py
+-rw-r--r--   0        0        0    15739 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/pull_zone.py
+-rw-r--r--   0        0        0       76 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/pull_zone_type.py
+-rw-r--r--   0        0        0      969 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/storage_object.py
+-rw-r--r--   0        0        0     1905 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/storage_zone.py
+-rw-r--r--   0        0        0      107 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/models/trigger_matching_type.py
+-rw-r--r--   0        0        0     1748 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/pull_zone_client.py
+-rw-r--r--   0        0        0     1127 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/storage_endpoints.py
+-rw-r--r--   0        0        0     8007 2023-04-16 12:03:51.759701 bunnynet-0.2.0/bunnynet/storage_zone_client.py
+-rw-r--r--   0        0        0     1307 2023-04-16 12:03:51.759701 bunnynet-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 bunnynet-0.2.0/PKG-INFO
```

### Comparing `bunnynet-0.1.0/LICENSE` & `bunnynet-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bunnynet-0.1.0/bunnynet/client.py` & `bunnynet-0.2.0/bunnynet/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -155,7 +155,18 @@
             key=key,
             expiration=expiration,
             token_countries=token_countries,
             token_countries_blocked=token_countries_blocked,
         )
 
         return parsed_url.scheme + "://" + parsed_url.netloc + parsed_url.path + "?" + urllib.parse.urlencode(signature)
+
+    def purge_url(self, url: str, *, wait: bool = True) -> None:
+        """Purge a URL from the cache.
+
+        :param url: The URL to purge from the CDN cache
+        :param wait: Set to false to enable an async purge
+        """
+
+        _ = self._http_client.get_raw(
+            "purge?url=" + urllib.parse.quote(url) + "&async=" + ("false" if wait else "true")
+        )
```

### Comparing `bunnynet-0.1.0/bunnynet/httpclient.py` & `bunnynet-0.2.0/bunnynet/httpclient.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,70 +49,74 @@
 
     def get_raw(
         self,
         endpoint: str,
         *,
         attempts: int = 3,
         domain: str = BASE_URL,
-    ) -> str:
+        access_key: str | None = None,
+    ) -> bytes:
         """Perform a GET to the endpoint specified.
 
         :param endpoint: The endpoint to perform the GET on
         :param attempts: Number of attempts remaining to try this call
         :param domain: Override the domain to something else
+        :param access_key: The access key to use instead of the default
 
         :raises BunnyHTTPException: If something goes wrong in a call
 
         :returns: The response
         """
 
         url = "https://" + domain + "/" + endpoint
 
         raw_response = requests.get(
             url,
             headers={
-                "AccessKey": self._token,
+                "AccessKey": access_key or self._token,
             },
             timeout=10,
         )
 
         if not raw_response.ok:
             if attempts > 1 and (raw_response.status_code >= 500):
                 return self.get_raw(endpoint, attempts=attempts - 1)
 
             raise BunnyHTTPException(raw_response, "Failed to get data")
 
-        return raw_response.text
+        return raw_response.content
 
     def get(
         self,
         endpoint: str,
         response_type: Type[T],
         *,
         attempts: int = 3,
         domain: str = BASE_URL,
+        access_key: str | None = None,
     ) -> T:
         """Perform a GET to the endpoint specified.
 
         :param endpoint: The endpoint to perform the GET on
         :param response_type: The type of item the response contains
         :param attempts: Number of attempts remaining to try this call
         :param domain: Override the domain to something else
+        :param access_key: The access key to use instead of the default
 
         :raises BunnyHTTPException: If something goes wrong in a call
 
         :returns: The response deserialized and cast to the passed in `response_type`
         """
 
         url = "https://" + domain + "/" + endpoint
 
         raw_response = requests.get(
             url,
             headers={
-                "AccessKey": self._token,
+                "AccessKey": access_key or self._token,
             },
             timeout=10,
         )
 
         try:
             response_data = self.extract_data(raw_response)
         except BunnyHTTPException as ex:
```

### Comparing `bunnynet-0.1.0/bunnynet/log_client.py` & `bunnynet-0.2.0/bunnynet/log_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,8 +63,8 @@
             + status_codes_string
             + "&search=&start="
             + str(start_index)
             + "&end="
             + str(end_index)
         )
 
-        return self.http_client.get_raw(endpoint, domain="logging.bunnycdn.com")
+        return self.http_client.get_raw(endpoint, domain="logging.bunnycdn.com").decode("utf-8")
```

### Comparing `bunnynet-0.1.0/bunnynet/models/edge_rule.py` & `bunnynet-0.2.0/bunnynet/models/edge_rule.py`

 * *Files identical despite different names*

### Comparing `bunnynet-0.1.0/bunnynet/models/edge_rule_action_type.py` & `bunnynet-0.2.0/bunnynet/models/edge_rule_action_type.py`

 * *Files identical despite different names*

### Comparing `bunnynet-0.1.0/bunnynet/models/edge_rule_trigger.py` & `bunnynet-0.2.0/bunnynet/models/edge_rule_trigger.py`

 * *Files identical despite different names*

### Comparing `bunnynet-0.1.0/bunnynet/models/hostname.py` & `bunnynet-0.2.0/bunnynet/models/hostname.py`

 * *Files identical despite different names*

### Comparing `bunnynet-0.1.0/bunnynet/models/pull_zone.py` & `bunnynet-0.2.0/bunnynet/models/pull_zone.py`

 * *Files identical despite different names*

### Comparing `bunnynet-0.1.0/bunnynet/models/storage_object.py` & `bunnynet-0.2.0/bunnynet/models/storage_object.py`

 * *Files identical despite different names*

### Comparing `bunnynet-0.1.0/bunnynet/models/storage_zone.py` & `bunnynet-0.2.0/bunnynet/models/storage_zone.py`

 * *Files identical despite different names*

### Comparing `bunnynet-0.1.0/bunnynet/pull_zone_client.py` & `bunnynet-0.2.0/bunnynet/pull_zone_client.py`

 * *Files identical despite different names*

### Comparing `bunnynet-0.1.0/bunnynet/storage_endpoints.py` & `bunnynet-0.2.0/bunnynet/storage_endpoints.py`

 * *Files identical despite different names*

### Comparing `bunnynet-0.1.0/bunnynet/storage_zone_client.py` & `bunnynet-0.2.0/bunnynet/storage_zone_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -201,7 +201,36 @@
 
         self.http_client.delete(
             endpoint=f"{storage_zone.name}/{path}/{file_name}",
             response_type=object,
             domain=StorageEndpoint.from_name(storage_zone.region or "").value,
             access_key=storage_zone.password,
         )
+
+    def get_text_file(
+        self,
+        *,
+        storage_zone_name: str | None = None,
+        storage_zone: StorageZone | None = None,
+        path: str,
+        file_name: str,
+    ) -> str:
+        """Get a text file.
+
+        Either the storage zone or the storage zone name must be provided. The
+        former will be used in the case where both are provided.
+
+        :param storage_zone_name: The name of the storage zone to get the file from
+        :param storage_zone: The storage zone to get the file from
+        :param path: The path of the file
+        :param file_name: The name of the file
+
+        :returns: The text from the file
+        """
+
+        storage_zone = self._resolve_storage_zone(storage_zone_name=storage_zone_name, storage_zone=storage_zone)
+
+        return self.http_client.get_raw(
+            endpoint=f"{storage_zone.name}/{path}/{file_name}",
+            domain=StorageEndpoint.from_name(storage_zone.region or "").value,
+            access_key=storage_zone.password,
+        ).decode("utf-8")
```

### Comparing `bunnynet-0.1.0/pyproject.toml` & `bunnynet-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bunnynet"
-version = "0.1.0"
+version = "0.2.0"
 description = "A client for the bunny.net APIs"
 
 license = "MIT"
 
 authors = [
     "Dale Myers <dale@myers.io>"
 ]
```

### Comparing `bunnynet-0.1.0/PKG-INFO` & `bunnynet-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bunnynet
-Version: 0.1.0
+Version: 0.2.0
 Summary: A client for the bunny.net APIs
 Home-page: https://github.com/dalemyers/bunnynet
 License: MIT
 Keywords: bunny,bunny.net,cdn
 Author: Dale Myers
 Author-email: dale@myers.io
 Requires-Python: >=3.10,<4.0
```

