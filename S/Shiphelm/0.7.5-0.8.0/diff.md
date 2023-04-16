# Comparing `tmp/Shiphelm-0.7.5.tar.gz` & `tmp/Shiphelm-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shiphelm-0.7.5.tar", last modified: Sun Apr 16 19:02:40 2023, max compression
+gzip compressed data, was "Shiphelm-0.8.0.tar", last modified: Sun Apr 16 21:15:14 2023, max compression
```

## Comparing `Shiphelm-0.7.5.tar` & `Shiphelm-0.8.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:02:40.412449 Shiphelm-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-16 19:02:29.000000 Shiphelm-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-16 19:02:29.000000 Shiphelm-0.7.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-04-16 19:02:40.412449 Shiphelm-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-04-16 19:02:29.000000 Shiphelm-0.7.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-16 19:02:29.000000 Shiphelm-0.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-16 19:02:40.412449 Shiphelm-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-16 19:02:29.000000 Shiphelm-0.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:02:40.408449 Shiphelm-0.7.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:02:40.412449 Shiphelm-0.7.5/src/Shiphelm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-04-16 19:02:40.000000 Shiphelm-0.7.5/src/Shiphelm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-16 19:02:40.000000 Shiphelm-0.7.5/src/Shiphelm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 19:02:40.000000 Shiphelm-0.7.5/src/Shiphelm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-16 19:02:40.000000 Shiphelm-0.7.5/src/Shiphelm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-16 19:02:40.000000 Shiphelm-0.7.5/src/Shiphelm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:02:40.412449 Shiphelm-0.7.5/src/shiphelm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:02:29.000000 Shiphelm-0.7.5/src/shiphelm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-04-16 19:02:29.000000 Shiphelm-0.7.5/src/shiphelm/helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-16 19:02:29.000000 Shiphelm-0.7.5/src/shiphelm/helmdocker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-04-16 19:02:29.000000 Shiphelm-0.7.5/src/shiphelm/helmkube.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-16 19:02:29.000000 Shiphelm-0.7.5/src/shiphelm/helmswarm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:02:40.412449 Shiphelm-0.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-16 19:02:29.000000 Shiphelm-0.7.5/tests/test_module1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:14.639871 Shiphelm-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-16 21:14:59.000000 Shiphelm-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-16 21:14:59.000000 Shiphelm-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-04-16 21:15:14.639871 Shiphelm-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-04-16 21:14:59.000000 Shiphelm-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-16 21:14:59.000000 Shiphelm-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-16 21:15:14.639871 Shiphelm-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-16 21:14:59.000000 Shiphelm-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:14.635871 Shiphelm-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:14.639871 Shiphelm-0.8.0/src/Shiphelm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-04-16 21:15:14.000000 Shiphelm-0.8.0/src/Shiphelm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-16 21:15:14.000000 Shiphelm-0.8.0/src/Shiphelm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 21:15:14.000000 Shiphelm-0.8.0/src/Shiphelm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-16 21:15:14.000000 Shiphelm-0.8.0/src/Shiphelm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-16 21:15:14.000000 Shiphelm-0.8.0/src/Shiphelm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:14.639871 Shiphelm-0.8.0/src/shiphelm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:14:59.000000 Shiphelm-0.8.0/src/shiphelm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-04-16 21:14:59.000000 Shiphelm-0.8.0/src/shiphelm/helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-16 21:14:59.000000 Shiphelm-0.8.0/src/shiphelm/helmdocker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-16 21:14:59.000000 Shiphelm-0.8.0/src/shiphelm/helmkube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-16 21:14:59.000000 Shiphelm-0.8.0/src/shiphelm/helmswarm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:14.639871 Shiphelm-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-16 21:14:59.000000 Shiphelm-0.8.0/tests/test_module1.py
```

### Comparing `Shiphelm-0.7.5/LICENSE` & `Shiphelm-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Shiphelm-0.7.5/PKG-INFO` & `Shiphelm-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shiphelm
-Version: 0.7.5
+Version: 0.8.0
 Summary: Docker and kubernetes integration library
 Home-page: https://gameplex-software.github.io/ShipHelm/
 Author: Gameplex Software
 Author-email: info@gameplexsoftware.com
 Keywords: SkiffUI,kubernetes,docker
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Shiphelm Version: 0.7.5 Summary: Docker and
+Metadata-Version: 2.1 Name: Shiphelm Version: 0.8.0 Summary: Docker and
 kubernetes integration library Home-page: https://gameplex-software.github.io/
 ShipHelm/ Author: Gameplex Software Author-email: info@gameplexsoftware.com
 Keywords: SkiffUI,kubernetes,docker Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `Shiphelm-0.7.5/README.md` & `Shiphelm-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `Shiphelm-0.7.5/setup.py` & `Shiphelm-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `Shiphelm-0.7.5/src/Shiphelm.egg-info/PKG-INFO` & `Shiphelm-0.8.0/src/Shiphelm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shiphelm
-Version: 0.7.5
+Version: 0.8.0
 Summary: Docker and kubernetes integration library
 Home-page: https://gameplex-software.github.io/ShipHelm/
 Author: Gameplex Software
 Author-email: info@gameplexsoftware.com
 Keywords: SkiffUI,kubernetes,docker
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Shiphelm Version: 0.7.5 Summary: Docker and
+Metadata-Version: 2.1 Name: Shiphelm Version: 0.8.0 Summary: Docker and
 kubernetes integration library Home-page: https://gameplex-software.github.io/
 ShipHelm/ Author: Gameplex Software Author-email: info@gameplexsoftware.com
 Keywords: SkiffUI,kubernetes,docker Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `Shiphelm-0.7.5/src/shiphelm/helm.py` & `Shiphelm-0.8.0/src/shiphelm/helm.py`

 * *Files identical despite different names*

### Comparing `Shiphelm-0.7.5/src/shiphelm/helmdocker.py` & `Shiphelm-0.8.0/src/shiphelm/helmdocker.py`

 * *Files identical despite different names*

### Comparing `Shiphelm-0.7.5/src/shiphelm/helmkube.py` & `Shiphelm-0.8.0/src/shiphelm/helmkube.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,72 +16,73 @@
 
 from kubernetes import client, config
 
 class helmkube:
     def __init__(self, remote_address = None, remote_is_TLS = None):
         try:
             helmkube.kubeclient = client
-            self.api_client = helmkube.kubeclient.ApiClient()
+            config.load_kube_config()
+            helmkube.api_client = helmkube.kubeclient.ApiClient()
             namespace = "default"  # modify as needed
         except:
             pass
             #Finish: Remote Kubernetes connection
 
     def get_running_containers(self):
-        api_instance = helmkube.kubeclient.CoreV1Api(self.api_client)
+        api_instance = helmkube.kubeclient.CoreV1Api(helmkube.api_client)
         pods = api_instance.list_pod_for_all_namespaces(watch=False)
         containers = []
         for pod in pods.items:
             for container in pod.spec.containers:
                 containers.append(container)
         return containers
 
     def get_container_by_id(self, container_id):
         return self.get_container_by_id(container_id)
 
     def get_container_stats(self, container_id):
-        api_instance = helmkube.kubeclient.CoreV1Api(self.api_client)
+        api_instance = helmkube.kubeclient.CoreV1Api(helmkube.api_client)
         namespace = "default"  # modify as needed
         pod_name = container_id  # use container ID as pod name
         container_name = container_id  # use container ID as container name
         container_stats = api_instance.read_namespaced_pod_container_status(
             name=pod_name,
             namespace=namespace,
             container=container_name
         )
         return container_stats
 
     def get_container_ports(self, container_id):
-        api_instance = helmkube.kubeclient.CoreV1Api(self.api_client)
+        api_instance = helmkube.kubeclient.CoreV1Api(helmkube.api_client)
         namespace = "default"  # modify as needed
         pod_name = container_id  # use container ID as pod name
         container_name = container_id  # use container ID as container name
         container = api_instance.read_namespaced_pod(
             name=pod_name,
             namespace=namespace
         )
         ports = container.spec.containers[0].ports
         return ports
 
     def search_containers(self, name):
-        api_instance = helmkube.kubeclient.CoreV1Api(self.api_client)
+        api_instance = helmkube.kubeclient.CoreV1Api(helmkube.api_client)
         namespace = "default"  # modify as needed
         label_selector = f"name={name}"
         pods = api_instance.list_namespaced_pod(
             namespace=namespace,
             label_selector=label_selector
         )
         containers = []
         for pod in pods.items:
             for container in pod.spec.containers:
                 containers.append(container)
         return containers
 
     def change_container_ports(self, container_id, ports):
-        api_instance = helmkube.kubeclient.CoreV1Api(self.api_client)
+        api_instance = helmkube.kubeclient.CoreV1Api(helmkube.api_client)
         namespace = "default"  # modify as needed
         pod_name = container_id  # use container ID as pod name
         container_name = container_id  # use container ID as container name
         container = api_instance.read_namespaced_pod(
             name=pod_name,
             namespace=namespace
         )
@@ -89,15 +90,15 @@
         api_instance.patch_namespaced_pod(
             name=pod_name,
             namespace=namespace,
             body=container
         )
 
     def rename_container(self, container_id, new_name):
-        api_instance = helmkube.kubeclient.CoreV1Api(self.api_client)
+        api_instance = helmkube.kubeclient.CoreV1Api(helmkube.api_client)
         namespace = "default"  # modify as needed
         pod_name = container_id  # use container ID as pod name
         container_name = container_id  # use container ID as container name
         container = api_instance.read_namespaced_pod(
             name=pod_name,
             namespace=namespace
         )
```

### Comparing `Shiphelm-0.7.5/src/shiphelm/helmswarm.py` & `Shiphelm-0.8.0/src/shiphelm/helmswarm.py`

 * *Files identical despite different names*

