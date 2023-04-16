# Comparing `tmp/cdk_proxy_api_client-0.2.1.tar.gz` & `tmp/cdk_proxy_api_client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk_proxy_api_client-0.2.1.tar", max compression
+gzip compressed data, was "cdk_proxy_api_client-0.2.2.tar", max compression
```

## Comparing `cdk_proxy_api_client-0.2.1.tar` & `cdk_proxy_api_client-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    10280 2023-03-08 09:09:19.917488 cdk_proxy_api_client-0.2.1/LICENSE
--rw-r--r--   0        0        0     4404 2023-03-26 16:28:29.410881 cdk_proxy_api_client-0.2.1/README.md
--rw-r--r--   0        0        0      181 2023-04-07 15:31:20.720589 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/__init__.py
--rw-r--r--   0        0        0     1163 2023-03-26 16:47:51.442956 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/admin_auth/__init__.py
--rw-r--r--   0        0        0      133 2023-03-10 11:53:55.066691 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/admin_auth/exceptions.py
--rw-r--r--   0        0        0     4492 2023-03-30 12:32:52.183010 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/cli/__init__.py
--rw-r--r--   0        0        0     4062 2023-03-30 15:55:35.980876 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/cli/main_parser.py
--rw-r--r--   0        0        0     5728 2023-03-14 12:38:20.148498 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/client_wrapper.py
--rw-r--r--   0        0        0      601 2023-03-08 21:22:30.578973 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/common/__init__.py
--rw-r--r--   0        0        0     1174 2023-03-26 16:44:44.959697 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/common/logging.py
--rw-r--r--   0        0        0     3012 2023-03-10 11:34:33.523871 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/errors.py
--rw-r--r--   0        0        0       93 2023-03-08 21:22:30.582973 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/models/__init__.py
--rw-r--r--   0        0        0     1467 2023-03-08 10:34:32.551495 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/models/v1b1.py
--rw-r--r--   0        0        0     1400 2023-03-26 16:47:51.434956 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/proxy_api.py
--rw-r--r--   0        0        0        0 2023-03-14 12:46:32.223933 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/specs/__init__.py
--rw-r--r--   0        0        0     3825 2023-04-04 16:14:07.707858 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/specs/tenant_mappings-input.json
--rw-r--r--   0        0        0     2930 2023-04-04 15:57:38.770731 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/tenant_mappings/__init__.py
--rw-r--r--   0        0        0      414 2023-03-10 12:11:17.799028 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/tenant_mappings/exceptions.py
--rw-r--r--   0        0        0      800 2023-03-26 16:00:22.879474 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/tools/__init__.py
--rw-r--r--   0        0        0    11030 2023-04-07 15:30:59.300327 cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/tools/import_tenants_mappings.py
--rw-r--r--   0        0        0     2430 2023-04-07 15:31:20.720589 cdk_proxy_api_client-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5902 1970-01-01 00:00:00.000000 cdk_proxy_api_client-0.2.1/setup.py
--rw-r--r--   0        0        0     6035 1970-01-01 00:00:00.000000 cdk_proxy_api_client-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    10280 2023-03-08 09:09:19.917488 cdk_proxy_api_client-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4404 2023-03-26 16:28:29.410881 cdk_proxy_api_client-0.2.2/README.md
+-rw-r--r--   0        0        0      181 2023-04-16 08:58:42.448296 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/__init__.py
+-rw-r--r--   0        0        0     1163 2023-03-26 16:47:51.442956 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/admin_auth/__init__.py
+-rw-r--r--   0        0        0      133 2023-03-10 11:53:55.066691 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/admin_auth/exceptions.py
+-rw-r--r--   0        0        0     4849 2023-04-16 08:51:39.880237 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/cli/__init__.py
+-rw-r--r--   0        0        0     4473 2023-04-16 08:53:07.712280 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/cli/main_parser.py
+-rw-r--r--   0        0        0     5728 2023-03-14 12:38:20.148498 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/client_wrapper.py
+-rw-r--r--   0        0        0      601 2023-03-08 21:22:30.578973 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/common/__init__.py
+-rw-r--r--   0        0        0     1174 2023-03-26 16:44:44.959697 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/common/logging.py
+-rw-r--r--   0        0        0     3012 2023-03-10 11:34:33.523871 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/errors.py
+-rw-r--r--   0        0        0       93 2023-03-08 21:22:30.582973 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/models/__init__.py
+-rw-r--r--   0        0        0     1467 2023-03-08 10:34:32.551495 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/models/v1b1.py
+-rw-r--r--   0        0        0     1400 2023-03-26 16:47:51.434956 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/proxy_api.py
+-rw-r--r--   0        0        0        0 2023-03-14 12:46:32.223933 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/specs/__init__.py
+-rw-r--r--   0        0        0     3825 2023-04-16 08:57:33.887474 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/specs/tenant_mappings-input.json
+-rw-r--r--   0        0        0     2936 2023-04-16 08:53:27.770521 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/tenant_mappings/__init__.py
+-rw-r--r--   0        0        0      414 2023-03-10 12:11:17.799028 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/tenant_mappings/exceptions.py
+-rw-r--r--   0        0        0      800 2023-03-26 16:00:22.879474 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/tools/__init__.py
+-rw-r--r--   0        0        0    10915 2023-04-16 08:57:33.593470 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/tools/import_tenants_mappings.py
+-rw-r--r--   0        0        0     2430 2023-04-16 08:58:42.448296 cdk_proxy_api_client-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5902 1970-01-01 00:00:00.000000 cdk_proxy_api_client-0.2.2/setup.py
+-rw-r--r--   0        0        0     6035 1970-01-01 00:00:00.000000 cdk_proxy_api_client-0.2.2/PKG-INFO
```

### Comparing `cdk_proxy_api_client-0.2.1/LICENSE` & `cdk_proxy_api_client-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.1/README.md` & `cdk_proxy_api_client-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/admin_auth/__init__.py` & `cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/admin_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/cli/__init__.py` & `cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/cli/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import yaml
 
 try:
     from yaml import Dumper
 except ImportError:
     from yaml import CDumper as Dumper
 
-from compose_x_common.compose_x_common import set_else_none
+from compose_x_common.compose_x_common import keyisset, set_else_none
 
 from cdk_proxy_api_client.admin_auth import AdminAuth
 from cdk_proxy_api_client.cli.main_parser import set_parser
 from cdk_proxy_api_client.common.logging import LOG
 from cdk_proxy_api_client.proxy_api import ApiClient, Multitenancy, ProxyClient
 from cdk_proxy_api_client.tenant_mappings import TenantTopicMappings
 from cdk_proxy_api_client.tools import load_config_file
@@ -55,14 +55,21 @@
     tenant_name = set_else_none("tenant_name", kwargs)
     if action == "list":
         return tenants_mappings.list_tenant_topics_mappings(tenant_name).json()
     elif action == "import-from-tenants-config":
         content = load_config_file(path.abspath(kwargs["import_config_file"]))
         topics_mappings = import_tenants_mappings(proxy, content, tenant_name)
         return topics_mappings
+    elif action == "create":
+        tenants_mappings.create_tenant_topic_mapping(
+            tenant_name,
+            kwargs["logical_topic_name"],
+            kwargs["physical_topic_name"],
+            keyisset("ReadWrite", kwargs),
+        )
     elif action == "import-from-tenant":
         source_tenant = kwargs.pop("source_tenant")
         content = {
             "tenant_name": tenant_name,
             "mappings": [],
             "ignore_duplicates_conflict": True,
             "import_from_tenant": {"include_regex": [rf"^{source_tenant}$"]},
@@ -115,15 +122,19 @@
         "tenant-topic-mappings": tenant_mappings_actions,
         "auth": auth_actions,
     }
     dest_function = _categories_mappings[_category]
     response = dest_function(_proxy, _action, **_vars)
     if not response:
         return
-    if _args.output_format == "json":
-        print(json.dumps(response, indent=2))
-    else:
-        print(yaml.dump(response, Dumper=Dumper))
+    try:
+        if _args.output_format == "json":
+            print(json.dumps(response, indent=2))
+        else:
+            print(yaml.dump(response, Dumper=Dumper))
+    except Exception as error:
+        print(error)
+        print(response)
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/cli/main_parser.py` & `cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/cli/main_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,19 +34,29 @@
         dest="action", help="Mappings management"
     )
     mappings_subparser.add_parser(
         name="list",
         help="List tenant mappings",
         parents=[TENANT_PARSER],
     )
-    mappings_subparser.add_parser(
+    create_parser = mappings_subparser.add_parser(
         name="create",
         help="Create a new tenant mapping",
         parents=[TENANT_PARSER],
     )
+    create_parser.add_argument("--logical-topic-name", type=str, required=True)
+    create_parser.add_argument("--physical-topic-name", type=str, required=True)
+    create_parser.add_argument(
+        "--read-write",
+        required=False,
+        default=False,
+        dest="ReadWrite",
+        action="store_true",
+        help="Creates mapping in Read-Write (defaults to Read Only)",
+    )
     import_from_tenants_parser = mappings_subparser.add_parser(
         name="import-from-tenants-config",
         help="Create topic mappings from existing tenants",
     )
     import_from_tenants_parser.add_argument(
         "-f",
         "--import-config-file",
```

### Comparing `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/client_wrapper.py` & `cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/common/__init__.py` & `cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/common/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/common/logging.py` & `cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/common/logging.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/errors.py` & `cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/errors.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/models/v1b1.py` & `cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/models/v1b1.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/proxy_api.py` & `cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/proxy_api.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/specs/tenant_mappings-input.json` & `cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/specs/tenant_mappings-input.json`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/tenant_mappings/__init__.py` & `cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/tenant_mappings/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,20 @@
     app_path: str = f"{Multitenancy.app_path}"
 
     def create_tenant_topic_mapping(
         self,
         tenant_id: str,
         logical_topic_name: str,
         physical_topic_name: str,
-        read_only: bool = False,
+        read_write: bool = False,
     ) -> Response:
         """Create a new logical to physical topic mapping for tenant"""
         payload: dict = {
             "physicalTopicName": physical_topic_name,
-            "readOnly": read_only,
+            "readOnly": not read_write,
         }
         _path: str = f"{self.base_path}/tenants/{tenant_id}/topics/{logical_topic_name}"
         LOG.debug(f"create_tenant_topic_mapping path {_path}")
         req = self.proxy.client.post(
             _path,
             headers=self.proxy.client.json_headers,
             json=payload,
```

### Comparing `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/tools/__init__.py` & `cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.1/cdk_proxy_api_client/tools/import_tenants_mappings.py` & `cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/tools/import_tenants_mappings.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,33 +2,24 @@
 #   Copyright 2023 John Mille <john@ews-network.net>
 
 """Wrapper to configure mappings for a given tenant"""
 
 from __future__ import annotations
 
 import re
-import sys
 from copy import deepcopy
-
-import yaml
-
-try:
-    from yaml import Dumper
-except ImportError:
-    from yaml import CDumper as Dumper
-
 from json import loads
 
 from compose_x_common.compose_x_common import keyisset, set_else_none
 from importlib_resources import files as pkg_files
 from jsonschema import validate
 
 from cdk_proxy_api_client.common.logging import LOG
 from cdk_proxy_api_client.errors import ProxyApiException, ProxyGenericException
-from cdk_proxy_api_client.proxy_api import ApiClient, Multitenancy, ProxyClient
+from cdk_proxy_api_client.proxy_api import Multitenancy, ProxyClient
 from cdk_proxy_api_client.tenant_mappings import TenantTopicMappings
 
 DEFAULT_SCHEMA_PATH = pkg_files("cdk_proxy_api_client").joinpath(
     "specs/tenant_mappings-input.json"
 )
 
 
@@ -81,15 +72,15 @@
             else:
                 tenant_topics: list[dict] = get_tenant_logical_topics(proxy, _tenant)
                 for _import_tenant_topic in tenant_topics:
                     tenant_mappings.create_tenant_topic_mapping(
                         tenant_name,
                         _import_tenant_topic["logicalTopicName"],
                         _import_tenant_topic["physicalTopicName"],
-                        True,
+                        read_write=False,
                     )
                 processed_tenants.append(_tenant)
 
 
 def import_from_tenants_include_dict(
     proxy: ProxyClient,
     mapping_import_config: dict,
@@ -184,15 +175,15 @@
         grant_write_access = keyisset("grant_write_access", mapping_import_config)
         for topic_mapping in final_topics_import:
             try:
                 tenant_mappings.create_tenant_topic_mapping(
                     tenant_name,
                     topic_mapping["logicalTopicName"],
                     topic_mapping["physicalTopicName"],
-                    read_only=not grant_write_access,
+                    read_write=grant_write_access,
                 )
                 if grant_write_access:
                     LOG.warn(
                         "{}:{} - Granting write access.".format(
                             _tenant, topic_mapping["physicalTopicName"]
                         )
                     )
@@ -261,15 +252,15 @@
 ) -> None:
     for mapping in mappings:
         try:
             tenant_mappings.create_tenant_topic_mapping(
                 tenant_name,
                 mapping["logicalTopicName"],
                 mapping["physicalTopicName"],
-                read_only=keyisset("readOnly", mapping),
+                read_write=not keyisset("readOnly", mapping),
             )
         except ProxyGenericException as error:
             if error.code == 409 and ignore_conflicts:
                 pass
 
 
 def import_tenants_mappings(
```

### Comparing `cdk_proxy_api_client-0.2.1/pyproject.toml` & `cdk_proxy_api_client-0.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cdk-proxy-api-client"
 description = "Conduktor Proxy API Client"
-version = "0.2.1"
+version = "0.2.2"
 authors = ["John \"Preston\" Mille <john@ews-network.net>"]
 readme = "README.md"
 license = "LICENSE"
 packages = [{include = "cdk_proxy_api_client"}]
 keywords = ["compose-x", "conduktor", "kafka", "proxy"]
 classifiers = [
   "Development Status :: 2 - Pre-Alpha",
@@ -55,15 +55,15 @@
 cdk-cli = "cdk_proxy_api_client.cli:main"
 
 
 [tool.tbump]
 github_url = "https://codeberg.org/JohnPreston/cdk-proxy-api-client"
 
 [tool.tbump.version]
-current = "0.2.1"
+current = "0.2.2"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?:(?P<rc>[\S]+))?
```

### Comparing `cdk_proxy_api_client-0.2.1/setup.py` & `cdk_proxy_api_client-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
            'importlib-resources>=5.12.0,<6.0.0']}
 
 entry_points = \
 {'console_scripts': ['cdk-cli = cdk_proxy_api_client.cli:main']}
 
 setup_kwargs = {
     'name': 'cdk-proxy-api-client',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'Conduktor Proxy API Client',
     'long_description': '# cdk-proxy-api-client\n\nAPI Client library to interact with Conduktor Proxy\n\nCurrent version: v1beta1\n\n\n## Getting started\n\nFirst, create a Proxy Client\n\n```python\nfrom cdk_proxy_api_client.proxy_api import ApiClient, ProxyClient\n\napi = ApiClient("localhost", port=8888, username="superUser", password="superUser")\nproxy_client = ProxyClient(api)\n```\n\n### Features\n\nNote: we assume you are re-using the ``proxy_client`` as shown above.\n\n* Create new Token for a tenant\n\n```python\nfrom cdk_proxy_api_client.admin_auth import AdminAuth\n\nadmin = AdminAuth(proxy_client)\nadmin.create_tenant_credentials("a_tenant_name")\n```\n\n* List all topic mappings for a tenant\n\n```python\nfrom cdk_proxy_api_client.proxy_api import Multitenancy\n\ntenants_mgmt = Multitenancy(proxy_client)\ntenants = tenants_mgmt.list_tenants(as_list=True)\n```\n\n* Create a new mapping for a tenant\n* Delete a tenant - topic mapping\n* Delete all topic mappings for a tenant\n\n```python\nfrom cdk_proxy_api_client.tenant_mappings import TenantTopicMappings\n\ntenant_mappings_mgmt = TenantTopicMappings(proxy_client)\ntenant_mappings_mgmt.create_tenant_topic_mapping(\n    "tenant_name", "logical_name", "real_name"\n)\ntenant_mappings_mgmt.delete_tenant_topic_mapping("tenant_name", "logical_name")\n```\n\n## Testing\nThe testing is for now very manual. See ``e2e_testing.py``\n\nPytest will be added later on\n\n\n## Tools & CLI\n\nTo simplify the usage of the client, you can use some CLI commands\n\n```shell\nusage: CDK Proxy CLI [-h] [--format OUTPUT_FORMAT] --username USERNAME --password PASSWORD --url URL {auth,tenant-topic-mappings,tenants} ...\n\npositional arguments:\n  {auth,tenant-topic-mappings,tenants}\n                        Resources to manage\n    auth                Manages proxy tenant token\n    tenant-topic-mappings\n                        Manages tenant mappings\n    tenants             Manage tenants\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --format OUTPUT_FORMAT, --output-format OUTPUT_FORMAT\n                        output format\n  --username USERNAME\n  --password PASSWORD\n  --url URL\n\n```\n\n### cdk-cli tenant-topic-mappings\n\n```shell\nusage: CDK Proxy CLI tenant-topic-mappings [-h] {list,create,import-from-tenants-config,import-from-tenant,delete-all-mappings,delete-topic-mapping} ...\n\npositional arguments:\n  {list,create,import-from-tenants-config,import-from-tenant,delete-all-mappings,delete-topic-mapping}\n                        Mappings management\n    list                List tenant mappings\n    create              Create a new tenant mapping\n    import-from-tenants-config\n                        Create topic mappings from existing tenants\n    import-from-tenant  Import all topics from a existing tenant\n    delete-all-mappings\n                        Delete all topics mappings for a given tenant\n    delete-topic-mapping\n                        Delete a topic mapping for a given tenant\n\noptional arguments:\n  -h, --help            show this help message and exit\n```\n\n#### import-from-tenants-config\n\nThis command uses a configuration file that will be used to propagate mappings from one/multiple existing tenants to another.\n\nexample file:\n\n```yaml\n---\n# example.config.yaml\n\ntenant_name: application-01\nignore_duplicates_conflict: true\nmappings:\n  - logicalTopicName: data.stock\n    physicalTopicName: data.stock\n    readOnly: true\n```\n\n```shell\ncdk-cli --username ${PROXY_USERNAME} \\\n        --password ${PROXY_PASSWORD} \\\n        --url ${PROXY_URL} \\\n        tenant-topic-mappings import-from-tenants-config -f example.config.yaml\n```\n\n### cdk-cli auth\n\n```shell\ncdk-cli auth --help\nusage: CDK Proxy CLI auth [-h] {create} ...\n\npositional arguments:\n  {create}    Token actions to execute\n    create    Create a new tenant proxy JWT Token\n\noptional arguments:\n  -h, --help  show this help message and exit\n```\n\n#### cdk-cli-create-tenant-token\n\nCreate a new user tenant token\n\n```shell\ncdk-cli \\\n        --username ${PROXY_USERNAME} \\\n        --password ${PROXY_PASSWORD} \\\n        --url ${PROXY_URL} \\\n        auth create \\\n        --lifetime-in-seconds 3600  \\\n        --tenant-name js-fin-panther-stg\n```\n\n### cdk-cli tenants\n\nManage tenants\n\n```shell\ncdk-cli tenants --help\nusage: CDK Proxy CLI tenants [-h] {list} ...\n\npositional arguments:\n  {list}      Manage tenants\n    list      List tenants\n\noptional arguments:\n  -h, --help  show this help message and exit\n```\n',
     'author': 'John "Preston" Mille',
     'author_email': 'john@ews-network.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `cdk_proxy_api_client-0.2.1/PKG-INFO` & `cdk_proxy_api_client-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-proxy-api-client
-Version: 0.2.1
+Version: 0.2.2
 Summary: Conduktor Proxy API Client
 License: LICENSE
 Keywords: compose-x,conduktor,kafka,proxy
 Author: John "Preston" Mille
 Author-email: john@ews-network.net
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

