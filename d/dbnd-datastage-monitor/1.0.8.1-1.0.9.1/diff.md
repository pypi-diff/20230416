# Comparing `tmp/dbnd-datastage-monitor-1.0.8.1.tar.gz` & `tmp/dbnd-datastage-monitor-1.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnd-datastage-monitor-1.0.8.1.tar", last modified: Tue Nov 22 15:16:16 2022, max compression
+gzip compressed data, was "dbnd-datastage-monitor-1.0.9.1.tar", last modified: Tue Nov 22 16:26:38 2022, max compression
```

## Comparing `dbnd-datastage-monitor-1.0.8.1.tar` & `dbnd-datastage-monitor-1.0.9.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:16.874887 dbnd-datastage-monitor-1.0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 15:16:09.000000 dbnd-datastage-monitor-1.0.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      230 2022-11-22 15:16:09.000000 dbnd-datastage-monitor-1.0.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1437 2022-11-22 15:16:16.874887 dbnd-datastage-monitor-1.0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 15:16:16.875887 dbnd-datastage-monitor-1.0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      845 2022-11-22 15:16:09.000000 dbnd-datastage-monitor-1.0.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:16.867886 dbnd-datastage-monitor-1.0.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:16.869886 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/
--rw-rw-rw-   0 root         (0) root         (0)       73 2022-11-22 15:16:09.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      298 2022-11-22 15:16:09.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:16.871886 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/data/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3640 2022-11-22 15:16:09.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/data/datastage_config_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:16.871886 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/datastage_client/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/datastage_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12298 2022-11-22 15:16:09.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/datastage_client/datastage_api_client.py
--rw-rw-rw-   0 root         (0) root         (0)     4810 2022-11-22 15:16:09.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/datastage_client/datastage_assets_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:16.872887 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/fetcher/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/fetcher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1902 2022-11-22 15:16:09.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/fetcher/multi_project_data_fetcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:16.872887 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/metrics/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/metrics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2139 2022-11-22 15:16:09.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/metrics/prometheus_metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:16.873887 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/multiserver/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/multiserver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1809 2022-11-22 15:16:09.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/multiserver/datastage_multiserver.py
--rw-rw-rw-   0 root         (0) root         (0)     4087 2022-11-22 15:16:09.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/multiserver/datastage_services_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:16.873887 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/syncer/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/syncer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8427 2022-11-22 15:16:09.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/syncer/datastage_runs_syncer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:16.874887 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/tracking_service/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/tracking_service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      721 2022-11-22 15:16:09.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/tracking_service/datastage_servers_configuration_service.py
--rw-rw-rw-   0 root         (0) root         (0)     4261 2022-11-22 15:16:09.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/tracking_service/dbnd_datastage_tracking_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:16.870886 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1437 2022-11-22 15:16:16.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1489 2022-11-22 15:16:16.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:16.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      178 2022-11-22 15:16:16.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:16.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      100 2022-11-22 15:16:16.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2022-11-22 15:16:16.000000 dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:38.226846 dbnd-datastage-monitor-1.0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 16:26:26.000000 dbnd-datastage-monitor-1.0.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      230 2022-11-22 16:26:26.000000 dbnd-datastage-monitor-1.0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1437 2022-11-22 16:26:38.226846 dbnd-datastage-monitor-1.0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 16:26:38.227846 dbnd-datastage-monitor-1.0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      845 2022-11-22 16:26:26.000000 dbnd-datastage-monitor-1.0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:38.206844 dbnd-datastage-monitor-1.0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:38.215845 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2022-11-22 16:26:26.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      298 2022-11-22 16:26:26.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:38.220845 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/data/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3640 2022-11-22 16:26:26.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/data/datastage_config_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:38.221845 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/datastage_client/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/datastage_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12298 2022-11-22 16:26:26.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/datastage_client/datastage_api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     4810 2022-11-22 16:26:26.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/datastage_client/datastage_assets_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:38.221845 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/fetcher/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/fetcher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2022-11-22 16:26:26.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/fetcher/multi_project_data_fetcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:38.222846 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/metrics/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/metrics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2139 2022-11-22 16:26:26.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/metrics/prometheus_metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:38.223846 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/multiserver/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/multiserver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1809 2022-11-22 16:26:26.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/multiserver/datastage_multiserver.py
+-rw-rw-rw-   0 root         (0) root         (0)     4087 2022-11-22 16:26:26.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/multiserver/datastage_services_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:38.223846 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/syncer/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/syncer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8427 2022-11-22 16:26:26.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/syncer/datastage_runs_syncer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:38.224846 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/tracking_service/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/tracking_service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      721 2022-11-22 16:26:26.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/tracking_service/datastage_servers_configuration_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     4261 2022-11-22 16:26:26.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/tracking_service/dbnd_datastage_tracking_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:38.219845 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1437 2022-11-22 16:26:38.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1489 2022-11-22 16:26:38.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:38.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      178 2022-11-22 16:26:38.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:38.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      100 2022-11-22 16:26:38.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2022-11-22 16:26:38.000000 dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor.egg-info/top_level.txt
```

### Comparing `dbnd-datastage-monitor-1.0.8.1/LICENSE` & `dbnd-datastage-monitor-1.0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnd-datastage-monitor-1.0.8.1/PKG-INFO` & `dbnd-datastage-monitor-1.0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-datastage-monitor
-Version: 1.0.8.1
+Version: 1.0.9.1
 Summary: Machine Learning Orchestration
 Home-page: https://github.com/databand-ai/dbnd
 Author: Evgeny Shulman
 Author-email: evgeny.shulman@databand.ai
 Maintainer: Evgeny Shulman
 Maintainer-email: evgeny.shulman@databand.ai
 License: UNKNOWN
```

### Comparing `dbnd-datastage-monitor-1.0.8.1/setup.cfg` & `dbnd-datastage-monitor-1.0.9.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.0.8.1
+version = 1.0.9.1
 license_file = LICENSE
 description = Machine Learning Orchestration
 long_description_content_type = text/markdown
 long_description = file: README.md
 platforms = any
 author = Evgeny Shulman
 author_email = evgeny.shulman@databand.ai
```

### Comparing `dbnd-datastage-monitor-1.0.8.1/setup.py` & `dbnd-datastage-monitor-1.0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/data/datastage_config_data.py` & `dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/data/datastage_config_data.py`

 * *Files identical despite different names*

### Comparing `dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/datastage_client/datastage_api_client.py` & `dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/datastage_client/datastage_api_client.py`

 * *Files identical despite different names*

### Comparing `dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/datastage_client/datastage_assets_client.py` & `dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/datastage_client/datastage_assets_client.py`

 * *Files identical despite different names*

### Comparing `dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/fetcher/multi_project_data_fetcher.py` & `dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/fetcher/multi_project_data_fetcher.py`

 * *Files identical despite different names*

### Comparing `dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/metrics/prometheus_metrics.py` & `dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/metrics/prometheus_metrics.py`

 * *Files identical despite different names*

### Comparing `dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/multiserver/datastage_multiserver.py` & `dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/multiserver/datastage_multiserver.py`

 * *Files identical despite different names*

### Comparing `dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/multiserver/datastage_services_factory.py` & `dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/multiserver/datastage_services_factory.py`

 * *Files identical despite different names*

### Comparing `dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/syncer/datastage_runs_syncer.py` & `dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/syncer/datastage_runs_syncer.py`

 * *Files identical despite different names*

### Comparing `dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/tracking_service/datastage_servers_configuration_service.py` & `dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/tracking_service/datastage_servers_configuration_service.py`

 * *Files identical despite different names*

### Comparing `dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor/tracking_service/dbnd_datastage_tracking_service.py` & `dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor/tracking_service/dbnd_datastage_tracking_service.py`

 * *Files identical despite different names*

### Comparing `dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor.egg-info/PKG-INFO` & `dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-datastage-monitor
-Version: 1.0.8.1
+Version: 1.0.9.1
 Summary: Machine Learning Orchestration
 Home-page: https://github.com/databand-ai/dbnd
 Author: Evgeny Shulman
 Author-email: evgeny.shulman@databand.ai
 Maintainer: Evgeny Shulman
 Maintainer-email: evgeny.shulman@databand.ai
 License: UNKNOWN
```

### Comparing `dbnd-datastage-monitor-1.0.8.1/src/dbnd_datastage_monitor.egg-info/SOURCES.txt` & `dbnd-datastage-monitor-1.0.9.1/src/dbnd_datastage_monitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

