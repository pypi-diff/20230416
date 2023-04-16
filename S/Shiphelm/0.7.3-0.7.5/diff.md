# Comparing `tmp/Shiphelm-0.7.3.tar.gz` & `tmp/Shiphelm-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shiphelm-0.7.3.tar", last modified: Thu Apr 13 17:02:57 2023, max compression
+gzip compressed data, was "Shiphelm-0.7.5.tar", last modified: Sun Apr 16 19:02:40 2023, max compression
```

## Comparing `Shiphelm-0.7.3.tar` & `Shiphelm-0.7.5.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:02:57.869741 Shiphelm-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 17:02:47.000000 Shiphelm-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-13 17:02:47.000000 Shiphelm-0.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-04-13 17:02:57.869741 Shiphelm-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-04-13 17:02:47.000000 Shiphelm-0.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 17:02:47.000000 Shiphelm-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 17:02:57.873741 Shiphelm-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-13 17:02:47.000000 Shiphelm-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:02:57.869741 Shiphelm-0.7.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:02:57.869741 Shiphelm-0.7.3/src/Shiphelm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-04-13 17:02:57.000000 Shiphelm-0.7.3/src/Shiphelm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-13 17:02:57.000000 Shiphelm-0.7.3/src/Shiphelm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:02:57.000000 Shiphelm-0.7.3/src/Shiphelm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 17:02:57.000000 Shiphelm-0.7.3/src/Shiphelm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 17:02:57.000000 Shiphelm-0.7.3/src/Shiphelm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:02:57.869741 Shiphelm-0.7.3/src/shiphelm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:02:47.000000 Shiphelm-0.7.3/src/shiphelm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-04-13 17:02:47.000000 Shiphelm-0.7.3/src/shiphelm/helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-13 17:02:47.000000 Shiphelm-0.7.3/src/shiphelm/helmdocker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-04-13 17:02:47.000000 Shiphelm-0.7.3/src/shiphelm/helmkube.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-04-13 17:02:47.000000 Shiphelm-0.7.3/src/shiphelm/helmswarm.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-13 17:02:47.000000 Shiphelm-0.7.3/src/shiphelm/helmtest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:02:57.869741 Shiphelm-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-13 17:02:47.000000 Shiphelm-0.7.3/tests/test_module1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:02:40.412449 Shiphelm-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-16 19:02:29.000000 Shiphelm-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-16 19:02:29.000000 Shiphelm-0.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-04-16 19:02:40.412449 Shiphelm-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-04-16 19:02:29.000000 Shiphelm-0.7.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-16 19:02:29.000000 Shiphelm-0.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-16 19:02:40.412449 Shiphelm-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-16 19:02:29.000000 Shiphelm-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:02:40.408449 Shiphelm-0.7.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:02:40.412449 Shiphelm-0.7.5/src/Shiphelm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-04-16 19:02:40.000000 Shiphelm-0.7.5/src/Shiphelm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-16 19:02:40.000000 Shiphelm-0.7.5/src/Shiphelm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 19:02:40.000000 Shiphelm-0.7.5/src/Shiphelm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-16 19:02:40.000000 Shiphelm-0.7.5/src/Shiphelm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-16 19:02:40.000000 Shiphelm-0.7.5/src/Shiphelm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:02:40.412449 Shiphelm-0.7.5/src/shiphelm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:02:29.000000 Shiphelm-0.7.5/src/shiphelm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-04-16 19:02:29.000000 Shiphelm-0.7.5/src/shiphelm/helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-16 19:02:29.000000 Shiphelm-0.7.5/src/shiphelm/helmdocker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-04-16 19:02:29.000000 Shiphelm-0.7.5/src/shiphelm/helmkube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-16 19:02:29.000000 Shiphelm-0.7.5/src/shiphelm/helmswarm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:02:40.412449 Shiphelm-0.7.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-16 19:02:29.000000 Shiphelm-0.7.5/tests/test_module1.py
```

### Comparing `Shiphelm-0.7.3/LICENSE` & `Shiphelm-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Shiphelm-0.7.3/PKG-INFO` & `Shiphelm-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shiphelm
-Version: 0.7.3
+Version: 0.7.5
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
-Metadata-Version: 2.1 Name: Shiphelm Version: 0.7.3 Summary: Docker and
+Metadata-Version: 2.1 Name: Shiphelm Version: 0.7.5 Summary: Docker and
 kubernetes integration library Home-page: https://gameplex-software.github.io/
 ShipHelm/ Author: Gameplex Software Author-email: info@gameplexsoftware.com
 Keywords: SkiffUI,kubernetes,docker Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `Shiphelm-0.7.3/README.md` & `Shiphelm-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `Shiphelm-0.7.3/setup.py` & `Shiphelm-0.7.5/setup.py`

 * *Files identical despite different names*

### Comparing `Shiphelm-0.7.3/src/Shiphelm.egg-info/PKG-INFO` & `Shiphelm-0.7.5/src/Shiphelm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shiphelm
-Version: 0.7.3
+Version: 0.7.5
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
-Metadata-Version: 2.1 Name: Shiphelm Version: 0.7.3 Summary: Docker and
+Metadata-Version: 2.1 Name: Shiphelm Version: 0.7.5 Summary: Docker and
 kubernetes integration library Home-page: https://gameplex-software.github.io/
 ShipHelm/ Author: Gameplex Software Author-email: info@gameplexsoftware.com
 Keywords: SkiffUI,kubernetes,docker Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `Shiphelm-0.7.3/src/shiphelm/helmdocker.py` & `Shiphelm-0.7.5/src/shiphelm/helmdocker.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,104 +12,88 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ----------------------------------------------------------------------------
 import docker
 
 class helmdocker:
-    def __init__(remote_address = None, remote_is_TLS = None):
+    def __init__(remote_address=None, remote_is_TLS=None):
         try:
             helmdocker.client = docker.from_env()
         except:
             helmdocker.client = docker.from_env(base_url=remote_address, tls=remote_is_TLS)
 
-    @staticmethod
-    def get_running_containers():
+    def get_running_containers(self):
         return helmdocker.client.containers.list()
 
-    @staticmethod
-    def get_container_by_id(container_id):
+    def get_container_by_id(self, container_id):
         return helmdocker.client.containers.get(container_id)
 
-    @staticmethod
-    def get_container_stats(container_id):
+    def get_container_stats(self, container_id):
         container = helmdocker.client.containers.get(container_id)
         stats = container.stats(stream=False)
         return stats
 
-    @staticmethod
-    def get_container_ports(container_id):
+    def get_container_ports(self, container_id):
         container = helmdocker.client.containers.get(container_id)
         ports = container.attrs['NetworkSettings']['Ports']
         return ports
 
-    @staticmethod
-    def search_containers(name):
-        return helmdocker.containers.list(filters={"name": name})
+    def search_containers(self, name):
+        return helmdocker.client.containers.list(filters={"name": name})
 
-    @staticmethod
-    def change_container_ports(container_id, ports):
+    def change_container_ports(self, container_id, ports):
         container = helmdocker.client.containers.get(container_id)
         container.reload()
         container.ports.update(ports)
 
-    @staticmethod
-    def rename_container(container_id, new_name):
+    def rename_container(self, container_id, new_name):
         container = helmdocker.client.containers.get(container_id)
         container.rename(new_name)
 
-    @staticmethod
-    def add_container_to_network(container_id, network_name):
+    def add_container_to_network(self, container_id, network_name):
         network = helmdocker.client.networks.get(network_name)
         container = helmdocker.client.containers.get(container_id)
         network.connect(container)
 
-    @staticmethod
-    def remove_container_from_network(container_id, network_name):
+    def remove_container_from_network(self, container_id, network_name):
         network = helmdocker.client.networks.get(network_name)
         container = helmdocker.client.containers.get(container_id)
         network.disconnect(container)
 
-    @staticmethod
-    def create_network(network_name):
+    def create_network(self, network_name):
         helmdocker.client.networks.create(network_name)
 
-    @staticmethod
-    def delete_network(network_name):
+    def delete_network(self, network_name):
         network = helmdocker.client.networks.get(network_name)
         network.remove()
 
-    @staticmethod
-    def run_container(image, command=None, detach=False, ports=None, environment=None, volumes=None):
+    def run_container(self, image, command=None, detach=False, ports=None, environment=None, volumes=None):
         container = helmdocker.client.containers.run(
             image=image,
             command=command,
             detach=detach,
             ports=ports,
             environment=environment,
             volumes=volumes
         )
         return container
 
-    @staticmethod
-    def get_container_environment(container_id):
+    def get_container_environment(self, container_id):
         container = helmdocker.client.containers.get(container_id)
         environment = container.attrs['Config']['Env']
         return environment
 
-    @staticmethod
-    def set_container_environment(container_id, environment):
+    def set_container_environment(self, container_id, environment):
         container = helmdocker.client.containers.get(container_id)
         container.reload()
         container.update(env=environment)
 
-    @staticmethod
-    def get_container_volumes(container_id):
+    def get_container_volumes(self, container_id):
         container = helmdocker.client.containers.get(container_id)
         volumes = container.attrs['HostConfig']['Binds']
         return volumes
 
-    @staticmethod
-    def set_container_volumes(container_id, volumes):
+    def set_container_volumes(self, container_id, volumes):
         container = helmdocker.client.containers.get(container_id)
         container.reload()
-        container.update(binds=volumes)
+        container.update(binds=volumes)
```

### Comparing `Shiphelm-0.7.3/src/shiphelm/helmkube.py` & `Shiphelm-0.7.5/src/shiphelm/helmkube.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,98 +13,91 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ----------------------------------------------------------------------------
 
 from kubernetes import client, config
 
 class helmkube:
-    def __init__(remote_address = None, remote_is_TLS = None):
-      try:
-        helmkube.kubeclient = client
-        helmkube.api_client = helmkube.kubeclient.ApiClient()
-        namespace = "default"  # modify as needed
-      except:
-        pass
-        #Finish: Remote Kubernetes connection
+    def __init__(self, remote_address = None, remote_is_TLS = None):
+        try:
+            helmkube.kubeclient = client
+            self.api_client = helmkube.kubeclient.ApiClient()
+            namespace = "default"  # modify as needed
+        except:
+            pass
+            #Finish: Remote Kubernetes connection
 
-    @staticmethod
-    def get_running_containers():
-        api_instance = helmkube.kubeclient.CoreV1Api(helmkube.api_client)
+    def get_running_containers(self):
+        api_instance = helmkube.kubeclient.CoreV1Api(self.api_client)
         pods = api_instance.list_pod_for_all_namespaces(watch=False)
         containers = []
         for pod in pods.items:
             for container in pod.spec.containers:
                 containers.append(container)
         return containers
 
-    @staticmethod
-    def get_container_by_id(container_id):
-        return helmkube.get_container_by_id(container_id)
+    def get_container_by_id(self, container_id):
+        return self.get_container_by_id(container_id)
 
-    @staticmethod
-    def get_container_stats(container_id):
-        api_instance = helmkube.kubeclient.CoreV1Api(helmkube.api_client)
+    def get_container_stats(self, container_id):
+        api_instance = helmkube.kubeclient.CoreV1Api(self.api_client)
         namespace = "default"  # modify as needed
         pod_name = container_id  # use container ID as pod name
         container_name = container_id  # use container ID as container name
         container_stats = api_instance.read_namespaced_pod_container_status(
             name=pod_name,
             namespace=namespace,
             container=container_name
         )
         return container_stats
 
-    @staticmethod
-    def get_container_ports(container_id):
-        api_instance = helmkube.kubeclient.CoreV1Api(helmkube.api_client)
+    def get_container_ports(self, container_id):
+        api_instance = helmkube.kubeclient.CoreV1Api(self.api_client)
         namespace = "default"  # modify as needed
         pod_name = container_id  # use container ID as pod name
         container_name = container_id  # use container ID as container name
         container = api_instance.read_namespaced_pod(
             name=pod_name,
             namespace=namespace
         )
         ports = container.spec.containers[0].ports
         return ports
 
-    @staticmethod
-    def search_containers(name):
-        api_instance = helmkube.kubeclient.CoreV1Api(helmkube.api_client)
+    def search_containers(self, name):
+        api_instance = helmkube.kubeclient.CoreV1Api(self.api_client)
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
 
-    @staticmethod
-    def change_container_ports(container_id, ports):
-        api_instance = helmkube.kubeclient.CoreV1Api(helmkube.api_client)
+    def change_container_ports(self, container_id, ports):
+        api_instance = helmkube.kubeclient.CoreV1Api(self.api_client)
         namespace = "default"  # modify as needed
         pod_name = container_id  # use container ID as pod name
         container_name = container_id  # use container ID as container name
         container = api_instance.read_namespaced_pod(
             name=pod_name,
             namespace=namespace
         )
         container.spec.containers[0].ports = ports
         api_instance.patch_namespaced_pod(
             name=pod_name,
             namespace=namespace,
             body=container
         )
 
-    @staticmethod
-    def rename_container(container_id, new_name):
-        api_instance = helmkube.kubeclient.CoreV1Api(helmkube.api_client)
+    def rename_container(self, container_id, new_name):
+        api_instance = helmkube.kubeclient.CoreV1Api(self.api_client)
         namespace = "default"  # modify as needed
         pod_name = container_id  # use container ID as pod name
         container_name = container_id  # use container ID as container name
         container = api_instance.read_namespaced_pod(
             name=pod_name,
             namespace=namespace
         )
@@ -112,25 +105,25 @@
         api_instance.replace_namespaced_pod(
             name=pod_name,
             namespace=namespace,
             body=container
         )
 
     @staticmethod
-    def add_container_to_network(container_id, network_name):
+    def add_container_to_network(self, container_id, network_name):
         # Kubernetes has a different networking model, so this method is not applicable
         pass
 
     @staticmethod
-    def remove_container_from_network(container_id, network_name):
+    def remove_container_from_network(self, container_id, network_name):
         # Kubernetes has a different networking model, so this method is not applicable
         pass
 
     @staticmethod
-    def create_service(service_name, app_name, container_port):
+    def create_service(self, service_name, app_name, container_port):
         namespace = "default"  # modify as needed
         v1 = helmkube.kubeclient.CoreV1Api()
         service_manifest = {
             "apiVersion": "v1",
             "kind": "Service",
             "metadata": {
                 "name": service_name,
@@ -148,13 +141,13 @@
                 ],
                 "type": "ClusterIP"
             }
         }
         v1.create_namespaced_service(namespace, service_manifest)
 
     @staticmethod
-    def set_container_volumes(container_name, volumes):
+    def set_container_volumes(self, container_name, volumes):
         namespace = "default"  # modify as needed
         v1 = helmkube.kubeclient.CoreV1Api()
         container = v1.read_namespaced_pod(container_name, namespace)
         container.spec.volumes = volumes
         v1.replace_namespaced_pod(container_name, namespace, container)
```

### Comparing `Shiphelm-0.7.3/src/shiphelm/helmswarm.py` & `Shiphelm-0.7.5/src/shiphelm/helmswarm.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,96 +16,86 @@
 import docker
 
 
 
 class helmswarm:
     def __init__(self, remote_address=None, remote_is_TLS=None):
         try:
-            except:
+            pass
+        except:
             helmswarm.client = docker.DockerClient(base_url=remote_address, tls=remote_is_TLS)
 
-    @staticmethod
-    def get_running_containers():
-        return helmswarm.client.services.list()
-
-    @staticmethod
-    def get_container_stats(service_id):
-        service = helmswarm.client.services.get(service_id)
-        stats = service.stats()
+    def get_running_containers(self):
+        return helmswarm.client.containers.list()
+
+    def get_container_by_id(self, container_id):
+        return helmswarm.client.containers.get(container_id)
+
+    def get_container_stats(self, container_id):
+        container = helmswarm.client.containers.get(container_id)
+        stats = container.stats(stream=False)
         return stats
-    
-    @staticmethod
-    def get_containerports(service_id):
-        service = helmswarm.client.services.get(service_id)
-        ports = service.attrs['Endpoint']['Ports']
+
+    def get_container_ports(self, container_id):
+        container = helmswarm.client.containers.get(container_id)
+        ports = container.attrs['NetworkSettings']['Ports']
         return ports
 
-    @staticmethod
-    def search_containers(name):
-        return helmswarm.client.services.list(filters={"name": name})
-    
-    @staticmethod
-    def change_container_ports(service_id, ports):
-        service = helmswarm.client.services.get(service_id)
-        service.update(EndpointSpec={'Ports': ports})
-
-    @staticmethod
-    def rename_container(service_id, new_name):
-        service = helmswarm.client.services.get(service_id)
-        service.update(name=new_name)
+    def search_containers(self, name):
+        return helmswarm.client.containers.list(filters={"name": name})
+
+    def change_container_ports(self, container_id, ports):
+        container = helmswarm.client.containers.get(container_id)
+        container.reload()
+        container.ports.update(ports)
+
+    def rename_container(self, container_id, new_name):
+        container = helmswarm.client.containers.get(container_id)
+        container.rename(new_name)
 
-    @staticmethod
-    def add_container_to_network(service_id, network_name):
+    def add_container_to_network(self, container_id, network_name):
         network = helmswarm.client.networks.get(network_name)
-        service = helmswarm.client.services.get(service_id)
-        network.connect(service)
+        container = helmswarm.client.containers.get(container_id)
+        network.connect(container)
 
-    @staticmethod
-    def remove_container_from_network(service_id, network_name):
+    def remove_container_from_network(self, container_id, network_name):
         network = helmswarm.client.networks.get(network_name)
-        service = helmswarm.client.services.get(service_id)
-        network.disconnect(service)
+        container = helmswarm.client.containers.get(container_id)
+        network.disconnect(container)
 
-    @staticmethod
-    def create_network(network_name):
+    def create_network(self, network_name):
         helmswarm.client.networks.create(network_name)
 
-    @staticmethod
-    def delete_network(network_name):
+    def delete_network(self, network_name):
         network = helmswarm.client.networks.get(network_name)
         network.remove()
 
-    @staticmethod
-    def run_container(image, command=None, detach=False, ports=None, environment=None, volumes=None):
+    def run_container(self, image, command=None, detach=False, ports=None, environment=None, volumes=None):
         container = helmswarm.client.containers.run(
             image=image,
             command=command,
             detach=detach,
             ports=ports,
             environment=environment,
             volumes=volumes
         )
         return container
 
-    @staticmethod
-    def get_container_environment(container_id):
+    def get_container_environment(self, container_id):
         container = helmswarm.client.containers.get(container_id)
         environment = container.attrs['Config']['Env']
         return environment
 
-    @staticmethod
-    def set_container_environment(container_id, environment):
+    def set_container_environment(self, container_id, environment):
         container = helmswarm.client.containers.get(container_id)
         container.reload()
         container.update(env=environment)
 
-    @staticmethod
-    def get_container_volumes(container_id):
+    def get_container_volumes(self, container_id):
         container = helmswarm.client.containers.get(container_id)
         volumes = container.attrs['HostConfig']['Binds']
         return volumes
 
-    @staticmethod
-    def set_container_volumes(container_id, volumes):
+    def set_container_volumes(self, container_id, volumes):
         container = helmswarm.client.containers.get(container_id)
         container.reload()
-        container.update(binds=volumes)
+        container.update(binds=volumes)
```

