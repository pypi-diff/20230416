# Comparing `tmp/TheengsGateway-0.9.0.tar.gz` & `tmp/TheengsGateway-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TheengsGateway-0.9.0.tar", last modified: Tue Mar 28 13:04:16 2023, max compression
+gzip compressed data, was "TheengsGateway-1.0.0.tar", last modified: Sun Apr 16 19:18:07 2023, max compression
```

## Comparing `TheengsGateway-0.9.0.tar` & `TheengsGateway-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:04:16.466234 TheengsGateway-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-03-28 13:04:09.000000 TheengsGateway-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-03-28 13:04:09.000000 TheengsGateway-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-03-28 13:04:16.466234 TheengsGateway-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-03-28 13:04:09.000000 TheengsGateway-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:04:16.466234 TheengsGateway-0.9.0/TheengsGateway/
--rw-r--r--   0 runner    (1001) docker     (122)     8954 2023-03-28 13:04:09.000000 TheengsGateway-0.9.0/TheengsGateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-03-28 13:04:09.000000 TheengsGateway-0.9.0/TheengsGateway/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16967 2023-03-28 13:04:09.000000 TheengsGateway-0.9.0/TheengsGateway/ble_gateway.py
--rw-r--r--   0 runner    (1001) docker     (122)     4513 2023-03-28 13:04:09.000000 TheengsGateway-0.9.0/TheengsGateway/diagnose.py
--rw-r--r--   0 runner    (1001) docker     (122)     5026 2023-03-28 13:04:09.000000 TheengsGateway-0.9.0/TheengsGateway/discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:04:16.466234 TheengsGateway-0.9.0/TheengsGateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-03-28 13:04:16.000000 TheengsGateway-0.9.0/TheengsGateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-03-28 13:04:16.000000 TheengsGateway-0.9.0/TheengsGateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-28 13:04:16.000000 TheengsGateway-0.9.0/TheengsGateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-03-28 13:04:16.000000 TheengsGateway-0.9.0/TheengsGateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-03-28 13:04:16.000000 TheengsGateway-0.9.0/TheengsGateway.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:04:16.466234 TheengsGateway-0.9.0/bin/
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-03-28 13:04:09.000000 TheengsGateway-0.9.0/bin/TheengsGateway
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-03-28 13:04:09.000000 TheengsGateway-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-28 13:04:16.466234 TheengsGateway-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      863 2023-03-28 13:04:15.000000 TheengsGateway-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 19:18:07.320083 TheengsGateway-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-04-16 19:17:57.000000 TheengsGateway-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-16 19:17:57.000000 TheengsGateway-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-04-16 19:18:07.320083 TheengsGateway-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-04-16 19:17:57.000000 TheengsGateway-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 19:18:07.320083 TheengsGateway-1.0.0/TheengsGateway/
+-rw-r--r--   0 runner    (1001) docker     (122)     9286 2023-04-16 19:17:57.000000 TheengsGateway-1.0.0/TheengsGateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-04-16 19:17:57.000000 TheengsGateway-1.0.0/TheengsGateway/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17892 2023-04-16 19:17:57.000000 TheengsGateway-1.0.0/TheengsGateway/ble_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4522 2023-04-16 19:17:57.000000 TheengsGateway-1.0.0/TheengsGateway/diagnose.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5026 2023-04-16 19:17:57.000000 TheengsGateway-1.0.0/TheengsGateway/discovery.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 19:18:07.320083 TheengsGateway-1.0.0/TheengsGateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-04-16 19:18:07.000000 TheengsGateway-1.0.0/TheengsGateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-04-16 19:18:07.000000 TheengsGateway-1.0.0/TheengsGateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-16 19:18:07.000000 TheengsGateway-1.0.0/TheengsGateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-04-16 19:18:07.000000 TheengsGateway-1.0.0/TheengsGateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-16 19:18:07.000000 TheengsGateway-1.0.0/TheengsGateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 19:18:07.320083 TheengsGateway-1.0.0/bin/
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-04-16 19:17:57.000000 TheengsGateway-1.0.0/bin/TheengsGateway
+-rw-r--r--   0 runner    (1001) docker     (122)      242 2023-04-16 19:17:57.000000 TheengsGateway-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-16 19:18:07.320083 TheengsGateway-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      893 2023-04-16 19:18:04.000000 TheengsGateway-1.0.0/setup.py
```

### Comparing `TheengsGateway-0.9.0/LICENSE` & `TheengsGateway-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TheengsGateway-0.9.0/PKG-INFO` & `TheengsGateway-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TheengsGateway
-Version: 0.9.0
+Version: 1.0.0
 Home-page: https://github.com/theengs/gateway
 Author: Theengs
 License: GPL-3.0 License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 **Theengs Gateway** is a multi platforms, multi devices BLE to MQTT gateway that leverages the [Theengs Decoder library](https://github.com/theengs/decoder).
```

### Comparing `TheengsGateway-0.9.0/README.md` & `TheengsGateway-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `TheengsGateway-0.9.0/TheengsGateway/__init__.py` & `TheengsGateway-1.0.0/TheengsGateway/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,19 +40,22 @@
     "presence": 0,
     "publish_all": 1,
     "log_level": "WARNING",
     "discovery": 1,
     "hass_discovery": 1,
     "discovery_topic": "homeassistant/sensor",
     "discovery_device_name": "TheengsGateway",
-    "discovery_filter": ["IBEACON", "GAEN", "MS-CDP"],
+    "discovery_filter": [
+        "IBEACON",
+    ],
     "adapter": "",
     "scanning_mode": "active",
     "time_sync": [],
     "time_format": 0,
+    "publish_advdata": 0,
 }
 
 conf_path = os.path.expanduser("~") + "/theengsgw.conf"
 
 
 def main():
     parser = argparse.ArgumentParser()
@@ -196,14 +199,22 @@
         "-tf",
         "--time_format",
         dest="time_format",
         type=int,
         help="Use 12-hour (1) or 24-hour (0) time format for clocks "
         "(default: 0)",
     )
+    parser.add_argument(
+        "-padv",
+        "--publish_advdata",
+        dest="publish_advdata",
+        type=int,
+        help="Publish advertising and advanced data (1) or not (0) (default: 0)",
+    )
+
     args = parser.parse_args()
 
     try:
         with open(conf_path, encoding="utf-8") as config_file:
             config = json.load(config_file)
     except Exception:
         config = default_config
@@ -286,14 +297,17 @@
                 config["time_sync"].append(item)
     elif "time_sync" not in config.keys():
         config["time_sync"] = default_config["time_sync"]
 
     if args.time_format is not None:
         config["time_format"] = args.time_format
 
+    if args.publish_advdata is not None:
+        config["publish_advdata"] = args.publish_advdata
+
     if not config["host"]:
         sys.exit("Invalid MQTT host")
 
     try:
         with open(conf_path, mode="w", encoding="utf-8") as config_file:
             config_file.write(json.dumps(config, sort_keys=True, indent=4))
     except Exception as exception:
```

### Comparing `TheengsGateway-0.9.0/TheengsGateway/ble_gateway.py` & `TheengsGateway-1.0.0/TheengsGateway/ble_gateway.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 from bluetooth_clocks.exceptions import UnsupportedDeviceError
 from bluetooth_clocks.scanners import find_clock
 from bluetooth_numbers import company
 from bluetooth_numbers.exceptions import UnknownCICError
 from paho.mqtt import client as mqtt_client
 from TheengsDecoder import decodeBLE
 
+from .diagnose import diagnostics
+
 if platform.system() == "Linux":
     from bleak.assigned_numbers import AdvertisementDataType
     from bleak.backends.bluezdbus.advertisement_monitor import OrPattern
     from bleak.backends.bluezdbus.scanner import BlueZScannerArgs
 
 SECONDS_IN_DAY = 86400
 
@@ -317,43 +319,60 @@
         if data_json:
             data_json["id"] = device.address
             data_json["rssi"] = advertisement_data.rssi
             decoded_json = decodeBLE(json.dumps(data_json))
 
             if decoded_json:
                 decoded_json = json.loads(decoded_json)
-                # Only add manufacturer if device is compliant and no beacon
-                if decoded_json.get("cidc", True) and decoded_json[
-                    "model_id"
-                ] not in ("ABTemp", "IBEACON", "MS-CDP", "RDL52832"):
-                    try:
-                        decoded_json["mfr"] = company[company_id]
-                    except (UnboundLocalError, UnknownCICError):
-                        # Ignore when there's no manufacturer data
-                        # or when the company ID is unknown
-                        pass
+                # Only process if the device is not a random mac address
+                if decoded_json["type"] != "RMAC":
+                    # Only add manufacturer if device is compliant and no beacon
+                    if decoded_json.get("cidc", True) and decoded_json[
+                        "model_id"
+                    ] not in ("ABTemp", "IBEACON", "RDL52832"):
+                        try:
+                            decoded_json["mfr"] = company[company_id]
+                        except (UnboundLocalError, UnknownCICError):
+                            # Ignore when there's no manufacturer data
+                            # or when the company ID is unknown
+                            pass
 
-                if gw.presence:
-                    self.hass_presence(decoded_json)
-
-                if gw.discovery:
-                    gw.publish_device_info(
-                        decoded_json
-                    )  # Publish sensor data to Home Assistant MQTT discovery
-                else:
-                    msg = json.dumps(decoded_json)
-                    gw.publish(
-                        msg,
-                        gw.pub_topic + "/" + device.address.replace(":", ""),
-                    )
                     if gw.presence:
+                        self.hass_presence(decoded_json)
+
+                    # Remove advanced data
+                    if not gw.pubadvdata:
+                        for key in (
+                            "servicedatauuid",
+                            "servicedata",
+                            "manufacturerdata",
+                            "cidc",
+                            "acts",
+                            "cont",
+                            "track",
+                        ):
+                            decoded_json.pop(key, None)
+
+                    if gw.discovery:
+                        gw.publish_device_info(
+                            decoded_json
+                        )  # Publish sensor data to Home Assistant MQTT discovery
+                    else:
+                        msg = json.dumps(decoded_json)
                         gw.publish(
                             msg,
-                            gw.presence_topic,
+                            gw.pub_topic
+                            + "/"
+                            + device.address.replace(":", ""),
                         )
+                        if gw.presence:
+                            gw.publish(
+                                msg,
+                                gw.presence_topic,
+                            )
             elif gw.publish_all:
                 try:
                     data_json["mfr"] = company[company_id]
                 except (UnboundLocalError, UnknownCICError):
                     # Ignore when there's no manufacturer data
                     # or when the company ID is unknown
                     pass
@@ -425,19 +444,23 @@
     gw.pub_topic = config.get("publish_topic", "gateway_pub")
     gw.lwt_topic = config["lwt_topic"]
     gw.presence_topic = config["presence_topic"]
     gw.presence = config["presence"]
     gw.publish_all = config["publish_all"]
     gw.time_sync = config["time_sync"]
     gw.time_format = bool(config["time_format"])
+    gw.pubadvdata = bool(config["publish_advdata"])
 
     logging.basicConfig()
     logger.setLevel(log_level)
 
     loop = asyncio.get_event_loop()
+
+    if log_level == logging.DEBUG:
+        asyncio.run(diagnostics())
     thread = Thread(target=loop.run_forever, daemon=True)
     thread.start()
     asyncio.run_coroutine_threadsafe(gw.ble_scan_loop(), loop)
 
     gw.connect_mqtt()
 
     try:
```

### Comparing `TheengsGateway-0.9.0/TheengsGateway/diagnose.py` & `TheengsGateway-1.0.0/TheengsGateway/diagnose.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     for field in fields:
         if field in config:
             config[field] = "***"
 
 
 def _anonymize_address(address) -> str:
     addr_parts = _ADDR_RE.match(address)
-    try:
+    if addr_parts:
         return f"{addr_parts.group(1)}XX:XX:XX"
-    except AttributeError:
+    else:
         return "INVALID ADDRESS"
 
 
 def _anonymize_addresses(field, config) -> None:
     try:
         config[field] = [
             _anonymize_address(address) for address in config[field]
@@ -38,21 +38,21 @@
 def _section(title, values) -> None:
     """Print a collection of named values within a titled section.
     Args:
         title: The title for the section.
         values: The values to print out.
     """
     max_name = max(map(len, values.keys()))
-    max_value = max(map(len, values.values()))
+    max_value = max(map(len, [str(value) for value in values.values()]))
     print(f"## {title}")
     print()
     print(f"| {'Name':{max_name}} | {'Value':{max_value}} |")
     print(f"|-{'-' * max_name}-|-{'-'*max_value}-|")
     for name, value in values.items():
-        print(f"| {name:{max_name}} | {value:{max_value}} |")
+        print(f"| {name:{max_name}} | {str(value):{max_value}} |")
     print()
 
 
 def _versions() -> None:
     """Print useful version numbers."""
     try:
         packages = {
@@ -97,15 +97,15 @@
 def _os() -> None:
     os_parameters = {
         "System": platform.system(),
         "Release": platform.release(),
         "Version": platform.version(),
         "Machine type": platform.machine(),
     }
-    if platform.system() == "Linux":
+    if platform.system() == "Linux" and sys.version_info[:2] >= (3, 10):
         os_parameters["Distribution"] = platform.freedesktop_os_release()[
             "PRETTY_NAME"
         ]
 
     _section("Operating System", os_parameters)
 
 
@@ -113,15 +113,17 @@
     print("## Configuration")
     print()
     try:
         with open(_conf_path, encoding="utf-8") as config_file:
             config = json.load(config_file)
             _anonymize_strings(["user", "pass"], config)
             _anonymize_addresses("time_sync", config)
+        print("```")
         print(json.dumps(config, sort_keys=True, indent=4))
+        print("```")
         print()
     except FileNotFoundError:
         print(f"Configuration file not found: {_conf_path}")
         print()
 
 
 async def _adapters() -> None:
@@ -133,16 +135,14 @@
         bluetooth_adapters = get_adapters()
         await bluetooth_adapters.refresh()
         print(f"Default adapter: {bluetooth_adapters.default_adapter}")
         print()
 
         for adapter, properties in sorted(bluetooth_adapters.adapters.items()):
             properties["address"] = _anonymize_address(properties["address"])
-            for prop in properties:
-                properties[prop] = str(properties[prop])
             print("#", end="")
             _section(adapter, properties)
 
 
 async def diagnostics():
     print("# Theengs Gateway Diagnostics")
     print()
```

### Comparing `TheengsGateway-0.9.0/TheengsGateway/discovery.py` & `TheengsGateway-1.0.0/TheengsGateway/discovery.py`

 * *Files identical despite different names*

### Comparing `TheengsGateway-0.9.0/TheengsGateway.egg-info/PKG-INFO` & `TheengsGateway-1.0.0/TheengsGateway.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TheengsGateway
-Version: 0.9.0
+Version: 1.0.0
 Home-page: https://github.com/theengs/gateway
 Author: Theengs
 License: GPL-3.0 License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 **Theengs Gateway** is a multi platforms, multi devices BLE to MQTT gateway that leverages the [Theengs Decoder library](https://github.com/theengs/decoder).
```

### Comparing `TheengsGateway-0.9.0/setup.py` & `TheengsGateway-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 from setuptools import setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="TheengsGateway",
-    version="v0.9.0",
+    version="v1.0.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Theengs",
     url="https://github.com/theengs/gateway",
     license="GPL-3.0 License",
     package_dir={"TheengsGateway": "TheengsGateway"},
     packages=["TheengsGateway"],
     scripts=["bin/TheengsGateway"],
     include_package_data=True,
     install_requires=[
         "bleak>=0.19.0",
         'bluetooth-adapters>=0.15.3; python_version>="3.9"',
         "bluetooth-clocks<1.0",
         "bluetooth-numbers>=1.0,<2.0",
+        "importlib-metadata",
         "paho-mqtt>=1.6.1",
-        "TheengsDecoder>=1.3.0",
+        "TheengsDecoder>=1.4.0",
     ],
 )
```

