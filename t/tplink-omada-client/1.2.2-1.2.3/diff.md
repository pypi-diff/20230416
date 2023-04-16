# Comparing `tmp/tplink_omada_client-1.2.2.tar.gz` & `tmp/tplink_omada_client-1.2.3.tar.gz`

## Comparing `tplink_omada_client-1.2.2.tar` & `tplink_omada_client-1.2.3.tar`

### file list

```diff
@@ -1,35 +1,34 @@
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/.pylintrc
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/Dockerfile.dev
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/package_constraints.txt
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/requirements.txt
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/requirements_test.txt
--rwxr-xr-x   0        0        0     3375 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/sample_client.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/.vscode/launch.json
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/__init__.py
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/definitions.py
--rw-r--r--   0        0        0    14103 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/devices.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/exceptions.py
--rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/omadaapiconnection.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/omadaclient.py
--rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/omadasiteclient.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/py.typed
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/cli/__init__.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/cli/__main__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/cli/command_default.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/cli/command_devices.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/cli/command_switch.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/cli/command_switches.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/cli/command_target.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/cli/command_targets.py
--rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/cli/config.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/cli/util.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/tests/conftest.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/LICENSE
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/README.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/.pylintrc
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/Dockerfile.dev
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/requirements.txt
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/requirements_test.txt
+-rwxr-xr-x   0        0        0     3375 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/sample_client.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/.vscode/launch.json
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/__init__.py
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/definitions.py
+-rw-r--r--   0        0        0    14103 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/devices.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/exceptions.py
+-rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/omadaapiconnection.py
+-rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/omadaclient.py
+-rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/omadasiteclient.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/py.typed
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/cli/__init__.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/cli/__main__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/cli/command_default.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/cli/command_devices.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/cli/command_switch.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/cli/command_switches.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/cli/command_target.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/cli/command_targets.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/cli/config.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/cli/util.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/tests/conftest.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/LICENSE
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/README.md
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/PKG-INFO
```

### Comparing `tplink_omada_client-1.2.2/Dockerfile.dev` & `tplink_omada_client-1.2.3/Dockerfile.dev`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,13 @@
     && rm -rf /var/lib/apt/lists/*
 
 WORKDIR /workspaces
 
 # Install Python dependencies from requirements
 COPY requirements.txt ./
 COPY requirements_test.txt ./
-COPY package_constraints.txt ./
 RUN pip3 install -r requirements.txt
 RUN pip3 install -r requirements_test.txt 
-RUN rm -f requirements.txt requirements_test.txt package_constraints.txt
+RUN rm -f requirements.txt requirements_test.txt
 
 # Set the default shell to bash instead of sh
 ENV SHELL /bin/bash
```

### Comparing `tplink_omada_client-1.2.2/sample_client.py` & `tplink_omada_client-1.2.3/sample_client.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.2/.devcontainer/devcontainer.json` & `tplink_omada_client-1.2.3/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.2/.github/workflows/python-package.yml` & `tplink_omada_client-1.2.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.2/.github/workflows/python-publish.yml` & `tplink_omada_client-1.2.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.2/.vscode/launch.json` & `tplink_omada_client-1.2.3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.2/src/tplink_omada_client/definitions.py` & `tplink_omada_client-1.2.3/src/tplink_omada_client/definitions.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.2/src/tplink_omada_client/devices.py` & `tplink_omada_client-1.2.3/src/tplink_omada_client/devices.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.2/src/tplink_omada_client/exceptions.py` & `tplink_omada_client-1.2.3/src/tplink_omada_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.2/src/tplink_omada_client/omadaapiconnection.py` & `tplink_omada_client-1.2.3/src/tplink_omada_client/omadaapiconnection.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import time
 from typing import Any, Optional, Tuple
 
 import re
 from urllib.parse import urlsplit, urljoin
 from aiohttp import client_exceptions, CookieJar
 from aiohttp.client import ClientSession
+from awesomeversion  import AwesomeVersion
 
 from .exceptions import (
     BadControllerUrl,
     ConnectionFailed,
     LoginFailed,
     LoginSessionClosed,
     RequestFailed,
@@ -89,16 +90,15 @@
 
         Calls to login are optional, as the API will automatically authenticate as necessary.
         However, you may want to attempt a login to check connectivity.
         """
 
         version, controller_id = await self._get_controller_info()
 
-        # Alphabetical is good enough for now
-        if version < "5.0.0":
+        if AwesomeVersion(version) < AwesomeVersion("5.1.0"):
             raise UnsupportedControllerVersion(self._controller_version)
 
         self._controller_id = controller_id
         self._controller_version = version
 
         auth = {"username": self._username, "password": self._password}
         response = await self._do_request(
@@ -171,24 +171,24 @@
                 headers=headers,
                 json=payload,
                 ssl=self._verify_ssl,
             ) as response:
 
                 if response.status != 200:
                     if response.content_type == "application/json":
-                        content = await response.json()
+                        content = await response.json(encoding="utf-8")
                         self._check_application_errors(content)
 
                     raise RequestFailed(response.status, "HTTP Request Error")
 
                 # If something goes wrong with the login session, Omada requests return "success", and a login page. :/
                 if response.content_type != "application/json":
                     raise LoginSessionClosed()
 
-                content = await response.json()
+                content = await response.json(encoding="utf-8")
                 self._check_application_errors(content)
 
                 # Unpack response data
                 if "result" in content:
                     return content["result"]
                 return content
```

### Comparing `tplink_omada_client-1.2.2/src/tplink_omada_client/omadaclient.py` & `tplink_omada_client-1.2.3/src/tplink_omada_client/omadaclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
         await self._api.__aenter__()
         return self
 
     async def __aexit__(self, *args) -> bool:
         """Call when the client is disposed."""
         # Close the web session, if we created it (i.e. it was not passed in)
         return await self._api.__aexit__(*args)
-        
 
     async def login(self) -> str:
         """
         Log in to the controller and returns the controller's unique ID.
 
         Calls to login are optional, as the API will automatically authenticate as necessary.
         However, you may want to attempt a login to check connectivity.
```

### Comparing `tplink_omada_client-1.2.2/src/tplink_omada_client/omadasiteclient.py` & `tplink_omada_client-1.2.3/src/tplink_omada_client/omadasiteclient.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.2/src/tplink_omada_client/cli/__init__.py` & `tplink_omada_client-1.2.3/src/tplink_omada_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.2/src/tplink_omada_client/cli/command_default.py` & `tplink_omada_client-1.2.3/src/tplink_omada_client/cli/command_default.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.2/src/tplink_omada_client/cli/command_devices.py` & `tplink_omada_client-1.2.3/src/tplink_omada_client/cli/command_devices.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.2/src/tplink_omada_client/cli/command_switch.py` & `tplink_omada_client-1.2.3/src/tplink_omada_client/cli/command_switch.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.2/src/tplink_omada_client/cli/command_switches.py` & `tplink_omada_client-1.2.3/src/tplink_omada_client/cli/command_switches.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.2/src/tplink_omada_client/cli/command_target.py` & `tplink_omada_client-1.2.3/src/tplink_omada_client/cli/command_target.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.2/src/tplink_omada_client/cli/command_targets.py` & `tplink_omada_client-1.2.3/src/tplink_omada_client/cli/command_targets.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.2/src/tplink_omada_client/cli/config.py` & `tplink_omada_client-1.2.3/src/tplink_omada_client/cli/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     config_parser.remove_section(stored_name)
     config_parser.add_section(stored_name)
     config_parser.set(stored_name, "url", config.url)
     config_parser.set(stored_name, "username", config.username)
     config_parser.set(stored_name, "password", config.password)
     config_parser.set(stored_name, "site", config.site)
     if set_default:
-        if not config_parser[_CLI_SECTION]:
+        if _CLI_SECTION not in config_parser:
             config_parser[_CLI_SECTION] = {}
         config_parser[_CLI_SECTION][_DEFAULT_TARGET] = name
 
     _write_config_file(config_parser)
 
 def set_default_target(name: str) -> None:
     config_parser = _read_config_file()
```

### Comparing `tplink_omada_client-1.2.2/src/tplink_omada_client/cli/util.py` & `tplink_omada_client-1.2.3/src/tplink_omada_client/cli/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,9 +28,9 @@
     if not device:
         raise argparse.ArgumentError(None, f"Device with name {mac_or_name} not found")
     return device.mac
 
 def dump_raw_data(args: dict[str, Any], data: OmadaApiData):
     if args['dump']:
         print("--- BEGIN RAW DATA ---")
-        print(json.dumps(data.raw_data, indent=2))
+        print(json.dumps(data.raw_data, indent=2,ensure_ascii=False))
         print("---  END RAW DATA  ---")
```

### Comparing `tplink_omada_client-1.2.2/LICENSE` & `tplink_omada_client-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.2/README.md` & `tplink_omada_client-1.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     * List Devices (APs, Gateways and Switches)
     * Basic device information
     * Get firmware information and initiating automatic updates
     * Port status and configuraton for Switches
     * Lan port configuration for Access Points
 
 Tested with OC200 on Omada Controller Version 5.5.7 - 5.7.6. Other versions may not be fully compatible.
+Version 5.0.x is definitely not compatible.
 
 ## CLI
 
 This package provides a simple CLI for interacting with one or more Omada Controllers. To start using the
 CLI, you must first target a Controller.
 
 ```sh
```

### Comparing `tplink_omada_client-1.2.2/pyproject.toml` & `tplink_omada_client-1.2.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tplink_omada_client"
-version = "1.2.2"
+version = "1.2.3"
 authors = [
   { name="Mark Godwin", email="author@example.com" },
 ]
 description = "Python wrapper for TP-Link Omada SDN Controller API (OC200/OC300/Software Controller)"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
   "Programming Language :: Python :: 3.9",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 dependencies = [
-  "aiohttp >= 3.8.1, <4"
+  "aiohttp >= 3.8.1, <4",
+  "awesomeversion >= 22.9.0"
 ]
 
 [project.scripts]
 omada = "tplink_omada_client.cli:main"
 
 [project.urls]
 "Homepage" = "https://github.com/MarkGodwin/tplink-omada-api"
```

### Comparing `tplink_omada_client-1.2.2/PKG-INFO` & `tplink_omada_client-1.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: tplink_omada_client
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python wrapper for TP-Link Omada SDN Controller API (OC200/OC300/Software Controller)
 Project-URL: Homepage, https://github.com/MarkGodwin/tplink-omada-api
 Project-URL: Bug Tracker, https://github.com/MarkGodwin/tplink-omada-api/issues
 Author-email: Mark Godwin <author@example.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Requires-Dist: aiohttp<4,>=3.8.1
+Requires-Dist: awesomeversion>=22.9.0
 Description-Content-Type: text/markdown
 
 # What's this?
 
 A basic Python client for calling the TP-Link Omada controller API.
 
 ## Installation
@@ -33,14 +34,15 @@
     * List Devices (APs, Gateways and Switches)
     * Basic device information
     * Get firmware information and initiating automatic updates
     * Port status and configuraton for Switches
     * Lan port configuration for Access Points
 
 Tested with OC200 on Omada Controller Version 5.5.7 - 5.7.6. Other versions may not be fully compatible.
+Version 5.0.x is definitely not compatible.
 
 ## CLI
 
 This package provides a simple CLI for interacting with one or more Omada Controllers. To start using the
 CLI, you must first target a Controller.
 
 ```sh
```

