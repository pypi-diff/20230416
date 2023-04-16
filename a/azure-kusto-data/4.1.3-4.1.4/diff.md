# Comparing `tmp/azure-kusto-data-4.1.3.tar.gz` & `tmp/azure-kusto-data-4.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/azure-kusto-data-4.1.3.tar", last modified: Sun Mar 26 08:35:24 2023, max compression
+gzip compressed data, was "dist/azure-kusto-data-4.1.4.tar", last modified: Sun Apr 16 10:49:29 2023, max compression
```

## Comparing `azure-kusto-data-4.1.3.tar` & `azure-kusto-data-4.1.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 08:35:24.000000 azure-kusto-data-4.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-03-26 08:35:24.000000 azure-kusto-data-4.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 08:35:24.000000 azure-kusto-data-4.1.3/azure/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 08:35:24.000000 azure-kusto-data-4.1.3/azure/kusto/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 08:35:24.000000 azure-kusto-data-4.1.3/azure/kusto/data/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/_cloud_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/_string_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    27136 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/_token_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 08:35:24.000000 azure-kusto-data-4.1.3/azure/kusto/data/aio/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/aio/_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/aio/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/aio/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/aio/streaming_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/client_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/client_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/client_request_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/data_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28429 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/kcsb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/kusto_trusted_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/streaming_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/azure/kusto/data/wellKnownKustoEndpoints.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 08:35:24.000000 azure-kusto-data-4.1.3/azure_kusto_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-03-26 08:35:24.000000 azure-kusto-data-4.1.3/azure_kusto_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-03-26 08:35:24.000000 azure-kusto-data-4.1.3/azure_kusto_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 08:35:24.000000 azure-kusto-data-4.1.3/azure_kusto_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-26 08:35:24.000000 azure-kusto-data-4.1.3/azure_kusto_data.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-26 08:35:24.000000 azure-kusto-data-4.1.3/azure_kusto_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-26 08:35:24.000000 azure-kusto-data-4.1.3/azure_kusto_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-26 08:35:24.000000 azure-kusto-data-4.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 08:35:24.000000 azure-kusto-data-4.1.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 08:35:24.000000 azure-kusto-data-4.1.3/tests/aio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/tests/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16579 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/tests/aio/test_async_token_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-03-26 08:35:15.000000 azure-kusto-data-4.1.3/tests/aio/test_kusto_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/azure/kusto/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/azure/kusto/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/_cloud_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/_string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27136 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/_token_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/azure/kusto/data/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/aio/_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/aio/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/aio/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/aio/streaming_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/client_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/client_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/client_request_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/data_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28429 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/kcsb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/kusto_trusted_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/streaming_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/wellKnownKustoEndpoints.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/azure_kusto_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/azure_kusto_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/azure_kusto_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/azure_kusto_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/azure_kusto_data.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/azure_kusto_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/azure_kusto_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/tests/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/tests/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16579 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/tests/aio/test_async_token_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/tests/aio/test_kusto_client.py
```

### Comparing `azure-kusto-data-4.1.3/PKG-INFO` & `azure-kusto-data-4.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-kusto-data
-Version: 4.1.3
+Version: 4.1.4
 Summary: Kusto Data Client
 Home-page: https://github.com/Azure/azure-kusto-python
 Author: Microsoft Corporation
 Author-email: kustalk@microsoft.com
 License: MIT
 Description: Microsoft Azure Kusto Library for Python
         ========================================
```

### Comparing `azure-kusto-data-4.1.3/README.rst` & `azure-kusto-data-4.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.3/azure/kusto/data/_cloud_settings.py` & `azure-kusto-data-4.1.4/azure/kusto/data/_cloud_settings.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.3/azure/kusto/data/_converters.py` & `azure-kusto-data-4.1.4/azure/kusto/data/_converters.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.3/azure/kusto/data/_models.py` & `azure-kusto-data-4.1.4/azure/kusto/data/_models.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.3/azure/kusto/data/_telemetry.py` & `azure-kusto-data-4.1.4/azure/kusto/data/_telemetry.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.3/azure/kusto/data/_token_providers.py` & `azure-kusto-data-4.1.4/azure/kusto/data/_token_providers.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.3/azure/kusto/data/aio/_models.py` & `azure-kusto-data-4.1.4/azure/kusto/data/aio/_models.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.3/azure/kusto/data/aio/client.py` & `azure-kusto-data-4.1.4/azure/kusto/data/aio/client.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.3/azure/kusto/data/aio/response.py` & `azure-kusto-data-4.1.4/azure/kusto/data/aio/response.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.3/azure/kusto/data/aio/streaming_response.py` & `azure-kusto-data-4.1.4/azure/kusto/data/aio/streaming_response.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.3/azure/kusto/data/client.py` & `azure-kusto-data-4.1.4/azure/kusto/data/client.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.3/azure/kusto/data/client_base.py` & `azure-kusto-data-4.1.4/azure/kusto/data/client_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -169,20 +169,23 @@
                 "name": "x-ms-user",
                 "value": client_details.user_name_for_tracing,
                 "property": lambda p: p.user,
             },
         ]
 
         for header in special_headers:
+            value: str
             if properties and header["property"](properties) is not None:
                 value = header["property"](properties)
             else:
                 value = header["value"]
 
             if value is not None:
+                # Replace any characters that aren't ascii with '?'
+                value = value.encode("ascii", "replace").decode("ascii", "strict")
                 request_headers[header["name"]] = value
 
         if properties is not None:
             if properties.get_option(ClientRequestProperties.no_request_timeout_option_name, False):
                 timeout = mgmt_default_timeout
             else:
                 timeout = properties.get_option(ClientRequestProperties.request_timeout_option_name, timeout)
```

### Comparing `azure-kusto-data-4.1.3/azure/kusto/data/client_details.py` & `azure-kusto-data-4.1.4/azure/kusto/data/client_details.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.3/azure/kusto/data/client_request_properties.py` & `azure-kusto-data-4.1.4/azure/kusto/data/client_request_properties.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.3/azure/kusto/data/data_format.py` & `azure-kusto-data-4.1.4/azure/kusto/data/data_format.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.3/azure/kusto/data/exceptions.py` & `azure-kusto-data-4.1.4/azure/kusto/data/exceptions.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.3/azure/kusto/data/helpers.py` & `azure-kusto-data-4.1.4/azure/kusto/data/helpers.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.3/azure/kusto/data/kcsb.py` & `azure-kusto-data-4.1.4/azure/kusto/data/kcsb.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.3/azure/kusto/data/kusto_trusted_endpoints.py` & `azure-kusto-data-4.1.4/azure/kusto/data/kusto_trusted_endpoints.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.3/azure/kusto/data/response.py` & `azure-kusto-data-4.1.4/azure/kusto/data/response.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.3/azure/kusto/data/security.py` & `azure-kusto-data-4.1.4/azure/kusto/data/security.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.3/azure/kusto/data/streaming_response.py` & `azure-kusto-data-4.1.4/azure/kusto/data/streaming_response.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.3/azure/kusto/data/wellKnownKustoEndpoints.json` & `azure-kusto-data-4.1.4/azure/kusto/data/wellKnownKustoEndpoints.json`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.3/azure_kusto_data.egg-info/PKG-INFO` & `azure-kusto-data-4.1.4/azure_kusto_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-kusto-data
-Version: 4.1.3
+Version: 4.1.4
 Summary: Kusto Data Client
 Home-page: https://github.com/Azure/azure-kusto-python
 Author: Microsoft Corporation
 Author-email: kustalk@microsoft.com
 License: MIT
 Description: Microsoft Azure Kusto Library for Python
         ========================================
```

### Comparing `azure-kusto-data-4.1.3/azure_kusto_data.egg-info/SOURCES.txt` & `azure-kusto-data-4.1.4/azure_kusto_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.3/setup.py` & `azure-kusto-data-4.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.3/tests/aio/test_async_token_providers.py` & `azure-kusto-data-4.1.4/tests/aio/test_async_token_providers.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.3/tests/aio/test_kusto_client.py` & `azure-kusto-data-4.1.4/tests/aio/test_kusto_client.py`

 * *Files identical despite different names*

