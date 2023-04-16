# Comparing `tmp/dbnd-dbt-monitor-1.0.8.1.tar.gz` & `tmp/dbnd-dbt-monitor-1.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnd-dbt-monitor-1.0.8.1.tar", last modified: Tue Nov 22 15:16:16 2022, max compression
+gzip compressed data, was "dbnd-dbt-monitor-1.0.9.1.tar", last modified: Tue Nov 22 16:26:37 2022, max compression
```

## Comparing `dbnd-dbt-monitor-1.0.8.1.tar` & `dbnd-dbt-monitor-1.0.9.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:16.208819 dbnd-dbt-monitor-1.0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 15:16:09.000000 dbnd-dbt-monitor-1.0.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      224 2022-11-22 15:16:09.000000 dbnd-dbt-monitor-1.0.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1431 2022-11-22 15:16:16.208819 dbnd-dbt-monitor-1.0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 15:16:16.209819 dbnd-dbt-monitor-1.0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      774 2022-11-22 15:16:09.000000 dbnd-dbt-monitor-1.0.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:16.202818 dbnd-dbt-monitor-1.0.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:16.204818 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/
--rw-rw-rw-   0 root         (0) root         (0)       73 2022-11-22 15:16:09.000000 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2022-11-22 15:16:09.000000 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:16.205818 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/data/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2336 2022-11-22 15:16:09.000000 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/data/dbt_config_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:16.206818 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/fetcher/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/fetcher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2544 2022-11-22 15:16:09.000000 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/fetcher/dbt_cloud_data_fetcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:16.206818 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/multiserver/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/multiserver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1593 2022-11-22 15:16:09.000000 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/multiserver/dbt_multiserver.py
--rw-rw-rw-   0 root         (0) root         (0)     2386 2022-11-22 15:16:09.000000 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/multiserver/dbt_services_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:16.207819 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/syncer/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/syncer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3011 2022-11-22 15:16:09.000000 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/syncer/dbt_runs_syncer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:16.207819 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/tracking_service/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/tracking_service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3870 2022-11-22 15:16:09.000000 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/tracking_service/dbnd_dbt_tracking_service.py
--rw-rw-rw-   0 root         (0) root         (0)      709 2022-11-22 15:16:09.000000 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/tracking_service/dbt_servers_configuration_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:16.205818 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1431 2022-11-22 15:16:16.000000 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1024 2022-11-22 15:16:16.000000 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:16.000000 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      142 2022-11-22 15:16:16.000000 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:16.000000 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       82 2022-11-22 15:16:16.000000 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-11-22 15:16:16.000000 dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:37.212742 dbnd-dbt-monitor-1.0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 16:26:26.000000 dbnd-dbt-monitor-1.0.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      224 2022-11-22 16:26:26.000000 dbnd-dbt-monitor-1.0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1431 2022-11-22 16:26:37.212742 dbnd-dbt-monitor-1.0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 16:26:37.213742 dbnd-dbt-monitor-1.0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      774 2022-11-22 16:26:26.000000 dbnd-dbt-monitor-1.0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:37.204741 dbnd-dbt-monitor-1.0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:37.207742 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2022-11-22 16:26:26.000000 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2022-11-22 16:26:26.000000 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:37.209742 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/data/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2336 2022-11-22 16:26:26.000000 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/data/dbt_config_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:37.210742 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/fetcher/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/fetcher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2544 2022-11-22 16:26:26.000000 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/fetcher/dbt_cloud_data_fetcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:37.211742 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/multiserver/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/multiserver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1593 2022-11-22 16:26:26.000000 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/multiserver/dbt_multiserver.py
+-rw-rw-rw-   0 root         (0) root         (0)     2386 2022-11-22 16:26:26.000000 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/multiserver/dbt_services_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:37.211742 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/syncer/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/syncer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3011 2022-11-22 16:26:26.000000 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/syncer/dbt_runs_syncer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:37.212742 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/tracking_service/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/tracking_service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3870 2022-11-22 16:26:26.000000 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/tracking_service/dbnd_dbt_tracking_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      709 2022-11-22 16:26:26.000000 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/tracking_service/dbt_servers_configuration_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:37.209742 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1431 2022-11-22 16:26:37.000000 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1024 2022-11-22 16:26:37.000000 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:37.000000 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      142 2022-11-22 16:26:37.000000 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:37.000000 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       82 2022-11-22 16:26:37.000000 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2022-11-22 16:26:37.000000 dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor.egg-info/top_level.txt
```

### Comparing `dbnd-dbt-monitor-1.0.8.1/LICENSE` & `dbnd-dbt-monitor-1.0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnd-dbt-monitor-1.0.8.1/PKG-INFO` & `dbnd-dbt-monitor-1.0.9.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-dbt-monitor
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

### Comparing `dbnd-dbt-monitor-1.0.8.1/setup.cfg` & `dbnd-dbt-monitor-1.0.9.1/setup.cfg`

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

### Comparing `dbnd-dbt-monitor-1.0.8.1/setup.py` & `dbnd-dbt-monitor-1.0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/data/dbt_config_data.py` & `dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/data/dbt_config_data.py`

 * *Files identical despite different names*

### Comparing `dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/fetcher/dbt_cloud_data_fetcher.py` & `dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/fetcher/dbt_cloud_data_fetcher.py`

 * *Files identical despite different names*

### Comparing `dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/multiserver/dbt_multiserver.py` & `dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/multiserver/dbt_multiserver.py`

 * *Files identical despite different names*

### Comparing `dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/multiserver/dbt_services_factory.py` & `dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/multiserver/dbt_services_factory.py`

 * *Files identical despite different names*

### Comparing `dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/syncer/dbt_runs_syncer.py` & `dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/syncer/dbt_runs_syncer.py`

 * *Files identical despite different names*

### Comparing `dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/tracking_service/dbnd_dbt_tracking_service.py` & `dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/tracking_service/dbnd_dbt_tracking_service.py`

 * *Files identical despite different names*

### Comparing `dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor/tracking_service/dbt_servers_configuration_service.py` & `dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor/tracking_service/dbt_servers_configuration_service.py`

 * *Files identical despite different names*

### Comparing `dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor.egg-info/PKG-INFO` & `dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-dbt-monitor
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

### Comparing `dbnd-dbt-monitor-1.0.8.1/src/dbnd_dbt_monitor.egg-info/SOURCES.txt` & `dbnd-dbt-monitor-1.0.9.1/src/dbnd_dbt_monitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

