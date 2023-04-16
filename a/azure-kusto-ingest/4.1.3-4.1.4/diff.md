# Comparing `tmp/azure-kusto-ingest-4.1.3.tar.gz` & `tmp/azure-kusto-ingest-4.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/azure-kusto-ingest-4.1.3.tar", last modified: Sun Mar 26 08:35:24 2023, max compression
+gzip compressed data, was "dist/azure-kusto-ingest-4.1.4.tar", last modified: Sun Apr 16 10:49:29 2023, max compression
```

## Comparing `azure-kusto-ingest-4.1.3.tar` & `azure-kusto-ingest-4.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 08:35:24.000000 azure-kusto-ingest-4.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-03-26 08:35:24.000000 azure-kusto-ingest-4.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-03-26 08:35:15.000000 azure-kusto-ingest-4.1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 08:35:24.000000 azure-kusto-ingest-4.1.3/azure/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 08:35:24.000000 azure-kusto-ingest-4.1.3/azure/kusto/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-26 08:35:15.000000 azure-kusto-ingest-4.1.3/azure/kusto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 08:35:24.000000 azure-kusto-ingest-4.1.3/azure/kusto/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-26 08:35:15.000000 azure-kusto-ingest-4.1.3/azure/kusto/ingest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-26 08:35:15.000000 azure-kusto-ingest-4.1.3/azure/kusto/ingest/_ingest_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-03-26 08:35:15.000000 azure-kusto-ingest-4.1.3/azure/kusto/ingest/_resource_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-03-26 08:35:15.000000 azure-kusto-ingest-4.1.3/azure/kusto/ingest/_status_q.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-03-26 08:35:15.000000 azure-kusto-ingest-4.1.3/azure/kusto/ingest/_stream_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-26 08:35:15.000000 azure-kusto-ingest-4.1.3/azure/kusto/ingest/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-03-26 08:35:15.000000 azure-kusto-ingest-4.1.3/azure/kusto/ingest/base_ingest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-03-26 08:35:15.000000 azure-kusto-ingest-4.1.3/azure/kusto/ingest/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-03-26 08:35:15.000000 azure-kusto-ingest-4.1.3/azure/kusto/ingest/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9977 2023-03-26 08:35:15.000000 azure-kusto-ingest-4.1.3/azure/kusto/ingest/ingest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-03-26 08:35:15.000000 azure-kusto-ingest-4.1.3/azure/kusto/ingest/ingestion_blob_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-03-26 08:35:15.000000 azure-kusto-ingest-4.1.3/azure/kusto/ingest/ingestion_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-03-26 08:35:15.000000 azure-kusto-ingest-4.1.3/azure/kusto/ingest/managed_streaming_ingest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-03-26 08:35:15.000000 azure-kusto-ingest-4.1.3/azure/kusto/ingest/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-03-26 08:35:15.000000 azure-kusto-ingest-4.1.3/azure/kusto/ingest/streaming_ingest_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 08:35:24.000000 azure-kusto-ingest-4.1.3/azure_kusto_ingest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-03-26 08:35:24.000000 azure-kusto-ingest-4.1.3/azure_kusto_ingest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-26 08:35:24.000000 azure-kusto-ingest-4.1.3/azure_kusto_ingest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 08:35:24.000000 azure-kusto-ingest-4.1.3/azure_kusto_ingest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-26 08:35:24.000000 azure-kusto-ingest-4.1.3/azure_kusto_ingest.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-26 08:35:24.000000 azure-kusto-ingest-4.1.3/azure_kusto_ingest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-26 08:35:24.000000 azure-kusto-ingest-4.1.3/azure_kusto_ingest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-26 08:35:24.000000 azure-kusto-ingest-4.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-03-26 08:35:15.000000 azure-kusto-ingest-4.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/azure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/azure/kusto/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/_ingest_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/_resource_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/_status_q.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/_stream_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/base_ingest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9977 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/ingest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/ingestion_blob_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/ingestion_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/managed_streaming_ingest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/streaming_ingest_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/azure_kusto_ingest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/azure_kusto_ingest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/azure_kusto_ingest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/azure_kusto_ingest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/azure_kusto_ingest.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/azure_kusto_ingest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/azure_kusto_ingest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/setup.py
```

### Comparing `azure-kusto-ingest-4.1.3/PKG-INFO` & `azure-kusto-ingest-4.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-kusto-ingest
-Version: 4.1.3
+Version: 4.1.4
 Summary: Kusto Ingest Client
 Home-page: https://github.com/Azure/azure-kusto-python
 Author: Microsoft Corporation
 Author-email: kustalk@microsoft.com
 License: MIT
 Description: Microsoft Azure Kusto Ingest Library for Python
         ===============================================
```

### Comparing `azure-kusto-ingest-4.1.3/README.rst` & `azure-kusto-ingest-4.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.3/azure/kusto/ingest/__init__.py` & `azure-kusto-ingest-4.1.4/azure/kusto/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.3/azure/kusto/ingest/_ingest_telemetry.py` & `azure-kusto-ingest-4.1.4/azure/kusto/ingest/_ingest_telemetry.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.3/azure/kusto/ingest/_resource_manager.py` & `azure-kusto-ingest-4.1.4/azure/kusto/ingest/_resource_manager.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.3/azure/kusto/ingest/_status_q.py` & `azure-kusto-ingest-4.1.4/azure/kusto/ingest/_status_q.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.3/azure/kusto/ingest/_stream_extensions.py` & `azure-kusto-ingest-4.1.4/azure/kusto/ingest/_stream_extensions.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.3/azure/kusto/ingest/base_ingest_client.py` & `azure-kusto-ingest-4.1.4/azure/kusto/ingest/base_ingest_client.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.3/azure/kusto/ingest/descriptors.py` & `azure-kusto-ingest-4.1.4/azure/kusto/ingest/descriptors.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.3/azure/kusto/ingest/exceptions.py` & `azure-kusto-ingest-4.1.4/azure/kusto/ingest/exceptions.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.3/azure/kusto/ingest/ingest_client.py` & `azure-kusto-ingest-4.1.4/azure/kusto/ingest/ingest_client.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.3/azure/kusto/ingest/ingestion_blob_info.py` & `azure-kusto-ingest-4.1.4/azure/kusto/ingest/ingestion_blob_info.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.3/azure/kusto/ingest/ingestion_properties.py` & `azure-kusto-ingest-4.1.4/azure/kusto/ingest/ingestion_properties.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.3/azure/kusto/ingest/managed_streaming_ingest_client.py` & `azure-kusto-ingest-4.1.4/azure/kusto/ingest/managed_streaming_ingest_client.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.3/azure/kusto/ingest/status.py` & `azure-kusto-ingest-4.1.4/azure/kusto/ingest/status.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.3/azure/kusto/ingest/streaming_ingest_client.py` & `azure-kusto-ingest-4.1.4/azure/kusto/ingest/streaming_ingest_client.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.3/azure_kusto_ingest.egg-info/PKG-INFO` & `azure-kusto-ingest-4.1.4/azure_kusto_ingest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-kusto-ingest
-Version: 4.1.3
+Version: 4.1.4
 Summary: Kusto Ingest Client
 Home-page: https://github.com/Azure/azure-kusto-python
 Author: Microsoft Corporation
 Author-email: kustalk@microsoft.com
 License: MIT
 Description: Microsoft Azure Kusto Ingest Library for Python
         ===============================================
```

### Comparing `azure-kusto-ingest-4.1.3/azure_kusto_ingest.egg-info/SOURCES.txt` & `azure-kusto-ingest-4.1.4/azure_kusto_ingest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.3/setup.py` & `azure-kusto-ingest-4.1.4/setup.py`

 * *Files identical despite different names*

