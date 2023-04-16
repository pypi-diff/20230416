# Comparing `tmp/airthings-exporter-0.0.1.tar.gz` & `tmp/airthings-exporter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airthings-exporter-0.0.1.tar", last modified: Sun Nov 27 22:50:02 2022, max compression
+gzip compressed data, was "airthings-exporter-0.0.2.tar", last modified: Sun Apr 16 21:56:18 2023, max compression
```

## Comparing `airthings-exporter-0.0.1.tar` & `airthings-exporter-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 max        (501) staff       (20)        0 2022-11-27 22:50:02.428460 airthings-exporter-0.0.1/
--rw-r--r--   0 max        (501) staff       (20)      113 2022-11-27 22:50:02.428323 airthings-exporter-0.0.1/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)      340 2022-11-27 20:40:09.000000 airthings-exporter-0.0.1/README.md
--rw-r--r--   0 max        (501) staff       (20)      387 2022-11-27 21:52:03.000000 airthings-exporter-0.0.1/pyproject.toml
--rw-r--r--   0 max        (501) staff       (20)       38 2022-11-27 22:50:02.428497 airthings-exporter-0.0.1/setup.cfg
-drwxr-xr-x   0 max        (501) staff       (20)        0 2022-11-27 22:50:02.426331 airthings-exporter-0.0.1/src/
-drwxr-xr-x   0 max        (501) staff       (20)        0 2022-11-27 22:50:02.427426 airthings-exporter-0.0.1/src/airthings/
--rw-r--r--   0 max        (501) staff       (20)     3197 2022-11-27 18:08:01.000000 airthings-exporter-0.0.1/src/airthings/CloudCollector.py
--rw-r--r--   0 max        (501) staff       (20)        0 2022-11-27 21:04:52.000000 airthings-exporter-0.0.1/src/airthings/__init__.py
--rw-r--r--   0 max        (501) staff       (20)      649 2022-11-27 22:41:38.000000 airthings-exporter-0.0.1/src/airthings/main.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2022-11-27 22:50:02.428188 airthings-exporter-0.0.1/src/airthings_exporter.egg-info/
--rw-r--r--   0 max        (501) staff       (20)      113 2022-11-27 22:50:02.000000 airthings-exporter-0.0.1/src/airthings_exporter.egg-info/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)      382 2022-11-27 22:50:02.000000 airthings-exporter-0.0.1/src/airthings_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 max        (501) staff       (20)        1 2022-11-27 22:50:02.000000 airthings-exporter-0.0.1/src/airthings_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 max        (501) staff       (20)       59 2022-11-27 22:50:02.000000 airthings-exporter-0.0.1/src/airthings_exporter.egg-info/entry_points.txt
--rw-r--r--   0 max        (501) staff       (20)       43 2022-11-27 22:50:02.000000 airthings-exporter-0.0.1/src/airthings_exporter.egg-info/requires.txt
--rw-r--r--   0 max        (501) staff       (20)       10 2022-11-27 22:50:02.000000 airthings-exporter-0.0.1/src/airthings_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-16 21:56:18.698779 airthings-exporter-0.0.2/
+-rw-r--r--   0 max        (501) staff       (20)      113 2023-04-16 21:56:18.698656 airthings-exporter-0.0.2/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      812 2022-11-27 23:09:31.000000 airthings-exporter-0.0.2/README.md
+-rw-r--r--   0 max        (501) staff       (20)      387 2023-04-16 21:56:08.000000 airthings-exporter-0.0.2/pyproject.toml
+-rw-r--r--   0 max        (501) staff       (20)       38 2023-04-16 21:56:18.698813 airthings-exporter-0.0.2/setup.cfg
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-16 21:56:18.696733 airthings-exporter-0.0.2/src/
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-16 21:56:18.697723 airthings-exporter-0.0.2/src/airthings/
+-rw-r--r--   0 max        (501) staff       (20)     3326 2023-04-16 21:32:40.000000 airthings-exporter-0.0.2/src/airthings/CloudCollector.py
+-rw-r--r--   0 max        (501) staff       (20)        0 2022-11-27 23:11:13.000000 airthings-exporter-0.0.2/src/airthings/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)      666 2023-04-16 21:24:49.000000 airthings-exporter-0.0.2/src/airthings/main.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-16 21:56:18.698513 airthings-exporter-0.0.2/src/airthings_exporter.egg-info/
+-rw-r--r--   0 max        (501) staff       (20)      113 2023-04-16 21:56:18.000000 airthings-exporter-0.0.2/src/airthings_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      382 2023-04-16 21:56:18.000000 airthings-exporter-0.0.2/src/airthings_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2023-04-16 21:56:18.000000 airthings-exporter-0.0.2/src/airthings_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 max        (501) staff       (20)       59 2023-04-16 21:56:18.000000 airthings-exporter-0.0.2/src/airthings_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 max        (501) staff       (20)       43 2023-04-16 21:56:18.000000 airthings-exporter-0.0.2/src/airthings_exporter.egg-info/requires.txt
+-rw-r--r--   0 max        (501) staff       (20)       10 2023-04-16 21:56:18.000000 airthings-exporter-0.0.2/src/airthings_exporter.egg-info/top_level.txt
```

### Comparing `airthings-exporter-0.0.1/src/airthings/CloudCollector.py` & `airthings-exporter-0.0.2/src/airthings/CloudCollector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import requests as requests
 from prometheus_client.metrics_core import GaugeMetricFamily
 from prometheus_client.registry import Collector
 
 
 class CloudCollector(Collector):
-    def __init__(self, client_id, client_secret, device_id):
+    def __init__(self, client_id, client_secret, device_id_list):
         self.client_id = client_id
         self.client_secret = client_secret
-        self.device_id = device_id
+        self.device_id_list = device_id_list
 
     def collect(self):
         gauge_metric_family = GaugeMetricFamily('airthings_gauge', 'Airthings sensor values')
-        data = self.__get_cloud_data__()
-        self.__add_samples__(gauge_metric_family, data)
+        access_token = self.__get_access_token__()
+        for device_id in self.device_id_list:
+            data = self.__get_cloud_data__(access_token, device_id)
+            self.__add_samples__(gauge_metric_family, data, device_id)
         yield gauge_metric_family
 
-    def __add_samples__(self, gauge_metric_family, data):
-        labels = {'device_id': self.device_id}
+    def __add_samples__(self, gauge_metric_family, data, device_id):
+        labels = {'device_id': device_id}
         if 'battery' in data:
             gauge_metric_family.add_sample('airthings_battery_percent', value=data['battery'], labels=labels)
         if 'co2' in data:
             gauge_metric_family.add_sample('airthings_co2_parts_per_million', value=data['co2'], labels=labels)
         if 'humidity' in data:
             gauge_metric_family.add_sample('airthings_humidity_percent', value=data['humidity'], labels=labels)
         if 'pm1' in data:
@@ -40,19 +42,18 @@
                                            value=float(data['radonShortTermAvg']),
                                            labels=labels)
         if 'temp' in data:
             gauge_metric_family.add_sample('airthings_temperature_celsius', value=data['temp'], labels=labels)
         if 'voc' in data:
             gauge_metric_family.add_sample('airthings_voc_parts_per_billion', value=data['voc'], labels=labels)
 
-    def __get_cloud_data__(self):
-        access_token = self.__get_access_token__()
+    def __get_cloud_data__(self, access_token, device_id):
         headers = {'Authorization': f'Bearer {access_token}'}
         response = requests.get(
-            f'https://ext-api.airthings.com/v1/devices/{self.device_id}/latest-samples',
+            f'https://ext-api.airthings.com/v1/devices/{device_id}/latest-samples',
             headers=headers)
         data = response.json()['data']
         return data
 
     def __get_access_token__(self):
         data = {
             "grant_type": "client_credentials",
```

### Comparing `airthings-exporter-0.0.1/src/airthings/main.py` & `airthings-exporter-0.0.2/src/airthings/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from airthings.CloudCollector import CloudCollector
 
 parser = argparse.ArgumentParser(
     prog='airthings-exporter',
     description='Prometheus exporter for Airthings devices')
 parser.add_argument('--client-id')
 parser.add_argument('--client-secret')
-parser.add_argument('--device-id')
+parser.add_argument('--device-id', action='append')
 args = parser.parse_args()
 
 REGISTRY.register(CloudCollector(args.client_id, args.client_secret, args.device_id))
 
 
 def main():
     start_http_server(8000)
```

