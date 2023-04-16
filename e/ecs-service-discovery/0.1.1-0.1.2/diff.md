# Comparing `tmp/ecs_service_discovery-0.1.1.tar.gz` & `tmp/ecs_service_discovery-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecs_service_discovery-0.1.1.tar", max compression
+gzip compressed data, was "ecs_service_discovery-0.1.2.tar", max compression
```

## Comparing `ecs_service_discovery-0.1.1.tar` & `ecs_service_discovery-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    16725 2023-03-12 12:50:13.531742 ecs_service_discovery-0.1.1/LICENSE
--rw-r--r--   0        0        0     3214 2023-03-31 07:22:14.894858 ecs_service_discovery-0.1.1/README.rst
--rw-r--r--   0        0        0      225 2023-03-31 10:15:35.571096 ecs_service_discovery-0.1.1/ecs_service_discovery/__init__.py
--rw-r--r--   0        0        0     1923 2023-03-12 12:50:13.532742 ecs_service_discovery-0.1.1/ecs_service_discovery/cli.py
--rw-r--r--   0        0        0     4001 2023-03-31 05:09:27.319912 ecs_service_discovery-0.1.1/ecs_service_discovery/ecs_sd_common.py
--rw-r--r--   0        0        0     3806 2023-03-31 10:14:55.557618 ecs_service_discovery-0.1.1/ecs_service_discovery/ecs_service_discovery.py
--rw-r--r--   0        0        0     8379 2023-03-31 10:15:36.075102 ecs_service_discovery-0.1.1/ecs_service_discovery/prometheus_sd.py
--rw-r--r--   0        0        0      723 2023-03-31 10:14:22.583225 ecs_service_discovery-0.1.1/ecs_service_discovery/stats.py
--rw-r--r--   0        0        0     2289 2023-03-31 10:15:35.571096 ecs_service_discovery-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4221 1970-01-01 00:00:00.000000 ecs_service_discovery-0.1.1/setup.py
--rw-r--r--   0        0        0     4672 1970-01-01 00:00:00.000000 ecs_service_discovery-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-03-12 12:50:13.531742 ecs_service_discovery-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3214 2023-03-31 07:22:14.894858 ecs_service_discovery-0.1.2/README.rst
+-rw-r--r--   0        0        0      225 2023-04-16 14:14:44.969920 ecs_service_discovery-0.1.2/ecs_service_discovery/__init__.py
+-rw-r--r--   0        0        0     1923 2023-03-12 12:50:13.532742 ecs_service_discovery-0.1.2/ecs_service_discovery/cli.py
+-rw-r--r--   0        0        0     4001 2023-03-31 05:09:27.319912 ecs_service_discovery-0.1.2/ecs_service_discovery/ecs_sd_common.py
+-rw-r--r--   0        0        0     3806 2023-03-31 10:14:55.557618 ecs_service_discovery-0.1.2/ecs_service_discovery/ecs_service_discovery.py
+-rw-r--r--   0        0        0     8786 2023-04-16 09:16:17.633828 ecs_service_discovery-0.1.2/ecs_service_discovery/prometheus_sd.py
+-rw-r--r--   0        0        0      723 2023-03-31 10:14:22.583225 ecs_service_discovery-0.1.2/ecs_service_discovery/stats.py
+-rw-r--r--   0        0        0     2289 2023-04-16 14:14:44.969920 ecs_service_discovery-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4221 1970-01-01 00:00:00.000000 ecs_service_discovery-0.1.2/setup.py
+-rw-r--r--   0        0        0     4672 1970-01-01 00:00:00.000000 ecs_service_discovery-0.1.2/PKG-INFO
```

### Comparing `ecs_service_discovery-0.1.1/LICENSE` & `ecs_service_discovery-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ecs_service_discovery-0.1.1/README.rst` & `ecs_service_discovery-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `ecs_service_discovery-0.1.1/ecs_service_discovery/cli.py` & `ecs_service_discovery-0.1.2/ecs_service_discovery/cli.py`

 * *Files identical despite different names*

### Comparing `ecs_service_discovery-0.1.1/ecs_service_discovery/ecs_sd_common.py` & `ecs_service_discovery-0.1.2/ecs_service_discovery/ecs_sd_common.py`

 * *Files identical despite different names*

### Comparing `ecs_service_discovery-0.1.1/ecs_service_discovery/ecs_service_discovery.py` & `ecs_service_discovery-0.1.2/ecs_service_discovery/ecs_service_discovery.py`

 * *Files identical despite different names*

### Comparing `ecs_service_discovery-0.1.1/ecs_service_discovery/prometheus_sd.py` & `ecs_service_discovery-0.1.2/ecs_service_discovery/prometheus_sd.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #  Copyright 2020-2022 John Mille <john@compose-x.io>
 
 from __future__ import annotations
 
 import json
 import pathlib
 from os import path
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Union
 
 import yaml
 
 try:
     from yaml import CDumper as Dumper
     from yaml import CSafeDumper as SafeDumper
 except ImportError:
@@ -136,25 +136,36 @@
         raise KeyError(
             f"Container definition for {container_name} not found in task definition",
             task_def["taskDefinitionArn"],
             [_container["name"] for _container in task_def["containerDefinitions"]],
         )
     labels = {
         "job": job_name,
-        "ecs_cluster_arn": task["clusterArn"],
-        "ecs_task_definition_arn": task_def["taskDefinitionArn"],
-        "ecs_task_family": task_def["family"],
-        "ecs_task_launch_type": task["launchType"],
+        "__meta_ecs_cluster_arn": task["clusterArn"],
+        "__meta_ecs_task_definition_arn": task_def["taskDefinitionArn"],
+        "__meta_ecs_task_family": task_def["family"],
+        "__meta_ecs_task_launch_type": task["launchType"],
     }
     labels.update(container_def["dockerLabels"])
+    to_add: dict = {}
+    to_del: list[str] = []
+    for label_name, label_value in labels.items():
+        if label_name.startswith("ecs_"):
+            to_add[f"__meta_{label_name}"] = label_value
+            to_del.append(label_name)
+    for label_to_del in to_del:
+        del labels[label_to_del]
+    labels.update(to_add)
     task_instance = set_else_none("_instance", task)
     if task_instance:
-        labels["ecs_task_instance"]: str = task_instance["containerInstanceArn"]
+        labels["__meta_ecs_task_instance"]: str = task_instance["containerInstanceArn"]
         if keyisset("ec2InstanceId", task_instance):
-            labels["ecs_instance_ec2_instance_id"] = task_instance["ec2InstanceId"]
+            labels["__meta_ecs_instance_ec2_instance_id"] = task_instance[
+                "ec2InstanceId"
+            ]
     return labels
 
 
 def create_prometheus_target_definition(
     task: dict, job_name: str, host_ip: str, container: dict, prometheus_port: int
 ) -> dict:
     """
```

### Comparing `ecs_service_discovery-0.1.1/ecs_service_discovery/stats.py` & `ecs_service_discovery-0.1.2/ecs_service_discovery/stats.py`

 * *Files identical despite different names*

### Comparing `ecs_service_discovery-0.1.1/pyproject.toml` & `ecs_service_discovery-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ecs_service_discovery"
-version = "0.1.1"
+version = "0.1.2"
 description = "ECS Service Discovery"
 authors = ["John Preston <john@ews-network.net>"]
 readme = "README.rst"
 license = "MPL-2.0"
 keywords = ["ecs", "service discovery", "observability"]
 classifiers = [
   "Development Status :: 4 - Beta",
@@ -71,15 +71,15 @@
 
 [tool.coverage.run]
 omit = [
   "*/cli.py"
 ]
 
 [tool.tbump.version]
-current = "0.1.1"
+current = "0.1.2"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?:(?P<rc>[\S]+))?
```

### Comparing `ecs_service_discovery-0.1.1/setup.py` & `ecs_service_discovery-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 entry_points = \
 {'console_scripts': ['ecs-sd = ecs_service_discovery.cli:main',
                      'ecs-service-discovery = ecs_service_discovery.cli:main']}
 
 setup_kwargs = {
     'name': 'ecs-service-discovery',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'ECS Service Discovery',
     'long_description': '=====================\nECS Service Discovery\n=====================\n\n.. image:: https://img.shields.io/pypi/v/ecs_service_discovery.svg\n        :target: https://pypi.python.org/pypi/ecs_service_discovery\n\nYet another tool to perform ECS API based service discovery.\nPrimarily aimed at gapping the lack of integrations for ECS Anywhere.\n\nFeatures\n==========\n\n* Creates Prometheus scraping configuration, from scanning ECS clusters & services, based on docker labels\n\nInstallation\n==============\n\nDocker\n--------\n\nHead to `Public ECR`_ to obtain the image\n\n.. code-block::\n\n    docker run --rm -it -v ~/.aws:/root/.aws public.ecr.aws/compose-x/ecs-service-discovery\n\n\nPython\n---------\n\nFor your user only\n\n.. code-block::\n\n    pip install pip --user ecs-service-discovery\n\nVia virtual environment\n\n.. code-block::\n\n    pip install ecs-service-discovery\n\n\nUsage\n=======\n\n.. code-block::\n\n    usage: ecs-sd [-h] [-d OUTPUT_DIR] [--profile PROFILE] [-p PROMETHEUS_PORT] [--intervals INTERVALS] [--prometheus-output-format PROMETHEUS_OUTPUT_FORMAT] [_ ...]\n\n    positional arguments:\n      _\n\n    options:\n      -h, --help            show this help message and exit\n      -d OUTPUT_DIR, --output_dir OUTPUT_DIR\n      --profile PROFILE     aws profile to use. Defaults to SDK default behaviour\n      -p PROMETHEUS_PORT, --prometheus-port PROMETHEUS_PORT\n      --intervals INTERVALS\n                            Time between ECS discovery intervals\n      --prometheus-output-format PROMETHEUS_OUTPUT_FORMAT\n                            Change the format of generated files. JSON or YAML.\n\nExamples\n==========\n\nECS Compose-X\n-----------------\n\nInstall `ecs-compose-x`_ & deploy to AWS\n\n.. hint::\n\n    you will need to use the `x-vpc`_ extension to deploy the service in the right VPC to get prometheus scraping.\n    you can use the `x-cluster`_ extension to specify the ECS Cluster you want to deploy the service to.\n\nDocker Compose\n-----------------\n\nAfter cloning the repository, run `docker compose up`. It will spin the service discovery, along with prometheus & grafana to run the demo with.\nYou can access prometheus via `localhost:9090` and grafana via `localhost:3000` (admin:admin by default).\n\nIn prometheus, you can look at the configuration and service discovery. You should see the discovered targets that prometheus is going to try\nto scrape.\n\nAWS Policy requirements\n=========================\n\n.. code-block:: yaml\n\n          PolicyName: ECSServiceDiscoverySimple\n          PolicyDocument:\n            Version: "2012-10-17"\n            Statement:\n              - Effect: Allow\n                Action:\n                  - ecs:ListClusters\n                  - ecs:ListContainerInstances\n                  - ecs:ListTasks\n                  - ecs:DescribeContainerInstances\n                  - ssm:DescribeInstanceInformation\n                  - ecs:DescribeTasks\n                  - ecs:DescribeTaskDefinition\n                Resource: \'*\'\n\n\n.. _Public ECR: https://gallery.ecr.aws/compose-x/ecs-service-discovery\n.. _ecs-compose-x: https://docs.compose-x.io/installation.html\n.. _x-cluster: https://docs.compose-x.io/syntax/compose_x/ecs_cluster.html\n.. _x-vpc: https://docs.compose-x.io/syntax/compose_x/vpc.html\n',
     'author': 'John Preston',
     'author_email': 'john@ews-network.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ecs_service_discovery-0.1.1/PKG-INFO` & `ecs_service_discovery-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecs-service-discovery
-Version: 0.1.1
+Version: 0.1.2
 Summary: ECS Service Discovery
 License: MPL-2.0
 Keywords: ecs,service discovery,observability
 Author: John Preston
 Author-email: john@ews-network.net
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

