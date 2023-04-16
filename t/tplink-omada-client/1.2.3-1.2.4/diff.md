# Comparing `tmp/tplink_omada_client-1.2.3.tar.gz` & `tmp/tplink_omada_client-1.2.4.tar.gz`

## Comparing `tplink_omada_client-1.2.3.tar` & `tplink_omada_client-1.2.4.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/.pylintrc
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/Dockerfile.dev
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/requirements.txt
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/requirements_test.txt
--rwxr-xr-x   0        0        0     3375 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/sample_client.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/.vscode/launch.json
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/__init__.py
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/definitions.py
--rw-r--r--   0        0        0    14103 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/devices.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/exceptions.py
--rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/omadaapiconnection.py
--rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/omadaclient.py
--rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/omadasiteclient.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/py.typed
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/cli/__init__.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/cli/__main__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/cli/command_default.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/cli/command_devices.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/cli/command_switch.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/cli/command_switches.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/cli/command_target.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/cli/command_targets.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/cli/config.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/src/tplink_omada_client/cli/util.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/tests/conftest.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/LICENSE
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/README.md
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/.pylintrc
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/Dockerfile.dev
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/requirements.txt
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/requirements_test.txt
+-rwxr-xr-x   0        0        0     3375 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/sample_client.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/.vscode/launch.json
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/__init__.py
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/definitions.py
+-rw-r--r--   0        0        0    18473 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/devices.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/exceptions.py
+-rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/omadaapiconnection.py
+-rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/omadaclient.py
+-rw-r--r--   0        0        0    11606 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/omadasiteclient.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/py.typed
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/cli/__init__.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/cli/__main__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_default.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_devices.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_gateway.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_switch.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_switches.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_target.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_targets.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/cli/config.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/cli/util.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/tests/conftest.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/LICENSE
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/README.md
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/PKG-INFO
```

### Comparing `tplink_omada_client-1.2.3/Dockerfile.dev` & `tplink_omada_client-1.2.4/Dockerfile.dev`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.3/sample_client.py` & `tplink_omada_client-1.2.4/sample_client.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.3/.devcontainer/devcontainer.json` & `tplink_omada_client-1.2.4/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.3/.github/workflows/python-package.yml` & `tplink_omada_client-1.2.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.3/.github/workflows/python-publish.yml` & `tplink_omada_client-1.2.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.3/.vscode/launch.json` & `tplink_omada_client-1.2.4/.vscode/launch.json`

 * *Files 10% similar despite different names*

```diff
@@ -31,10 +31,19 @@
         {
             "name": "CLI: Get Switch",
             "type": "python",
             "request": "launch",
             "module": "tplink_omada_client.cli",
             "justMyCode": true,
             "args": ["switch", "Main Switch", "--dump"]
+        },
+        {
+            "name": "CLI: Get Gateway",
+            "type": "python",
+            "request": "launch",
+            "module": "tplink_omada_client.cli",
+            "justMyCode": true,
+            "args": ["gateway", "--dump"]
         }
+
     ]
 }
```

### Comparing `tplink_omada_client-1.2.3/src/tplink_omada_client/definitions.py` & `tplink_omada_client-1.2.4/src/tplink_omada_client/definitions.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,14 +45,26 @@
 class PortType(IntEnum):
     """Known types of switch port."""
 
     COPPER = 1
     COMBO = 2
     SFP = 3
 
+class GatewayPortType(IntEnum):
+    """Known types of gateway port."""
+    WAN = 0
+    WAN_LAN = 1
+    LAN = 2
+    SFP_WAN = 3
+
+class GatewayPortMode(IntEnum):
+    """Modes of gateway port."""
+    DISABLED = -1
+    WAN = 0
+    LAN = 1
 
 class LinkStatus(IntEnum):
     """Known link statuses."""
 
     LINK_UP = 0
     LINK_DOWN = 2
```

### Comparing `tplink_omada_client-1.2.3/src/tplink_omada_client/devices.py` & `tplink_omada_client-1.2.4/src/tplink_omada_client/devices.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """
 Definitions for Omada device objects
 
 APs, Switches and Routers
 """
-from typing import Any, List, Optional
+from typing import Any, List, Optional, Union
 from .definitions import (
     BandwidthControl,
     DeviceStatus,
     DeviceStatusCategory,
     Eth802Dot1X,
+    GatewayPortMode,
+    GatewayPortType,
+    LinkDuplex,
     LinkSpeed,
     LinkStatus,
     PoEMode,
     PortType,
 )
 
 class OmadaApiData:
@@ -51,32 +54,40 @@
     def model_display_name(self) -> str:
         """Model description for front-end display."""
         return self._data["showModel"]
 
     @property
     def status(self) -> DeviceStatus:
         """The status of the device."""
-        return self._data["status"]
+        return DeviceStatus(self._data["status"])
 
     @property
     def status_category(self) -> DeviceStatusCategory:
         """The high-level status of the device."""
-        return self._data["statusCategory"]
+        return DeviceStatusCategory(self._data["statusCategory"])
 
     @property
     def ip_address(self) -> str:
         """IP address of the device."""
         return self._data["ip"]
 
     @property
     def display_uptime(self) -> str:
         """Uptime of the device, as a display string"""
         return self._data["uptime"]
 
     @property
+    def cpu_usage(self) -> int:
+        return self._data["cpuUtil"]
+        
+    @property
+    def mem_usage(self) -> int:
+        return self._data["memUtil"]
+
+    @property
     def uptime(self) -> int:
         """Uptime of the device, as a display string"""
         return self._data["uptimeLong"]
 
     @property
     def firmware_version(self) -> str:
         """Firmware version of the device"""
@@ -141,20 +152,20 @@
 
 class OmadaPortStatus(OmadaApiData):
     """Status information for a switch port."""
 
     @property
     def link_status(self) -> LinkStatus:
         """Port's link status."""
-        return self._data["linkStatus"]
+        return LinkStatus(self._data["linkStatus"])
 
     @property
     def link_speed(self) -> LinkSpeed:
         """Port's link speed."""
-        return self._data["linkSpeed"]
+        return LinkSpeed(self._data["linkSpeed"])
 
     @property
     def poe_active(self) -> bool:
         """Is the port powering a PoE device?"""
         return self._data["poe"]
 
     @property
@@ -363,15 +374,15 @@
     def port_id(self) -> str:
         """The ID of the port"""
         return self._data["id"]
 
     @property
     def max_speed(self) -> LinkSpeed:
         """The max speed of the port."""
-        return self._data["maxSpeed"]
+        return LinkSpeed(self._data["maxSpeed"])
 
     @property
     def profile_name(self) -> str:
         """Name of the port's config profile"""
         return self._data["profileName"]
 
     @property
@@ -383,15 +394,15 @@
     def poe_mode(self) -> PoEMode:
         """PoE config for this port."""
         return self._data["poe"]
 
     @property
     def bandwidth_limit_mode(self) -> BandwidthControl:
         """Type of bandwidth control applied."""
-        return self._data["bandWidthCtrlType"]
+        return BandwidthControl(self._data["bandWidthCtrlType"])
 
     # "bandCtrl": {
     #     "egressEnable": false,
     #     "egressLimit": 0,
     #     "egressUnit": 1,
     #     "ingressEnable": false,
     #     "ingressLimit": 0,
@@ -407,15 +418,15 @@
     #     "action": 0,
     #     "recoverTime": 3600
     # },
 
     @property
     def eth_802_1x_control(self) -> Eth802Dot1X:
         """802.1x Auth mode"""
-        return self._data["dot1x"]
+        return Eth802Dot1X(self._data["dot1x"])
 
     @property
     def lldp_med_enabled(self) -> bool:
         """LLDP Mode"""
         return self._data["lldpMedEnable"]
 
     @property
@@ -456,25 +467,25 @@
     def name(self) -> str:
         """Name of the profile."""
         return self._data["name"]
 
     @property
     def poe_mode(self) -> PoEMode:
         """PoE mode."""
-        return self._data["poe"]
+        return PoEMode(self._data["poe"])
 
     @property
     def bandwidth_limit_mode(self) -> BandwidthControl:
         """Type of bandwidth control applied."""
-        return self._data["bandWidthCtrlType"]
+        return BandwidthControl(self._data["bandWidthCtrlType"])
 
     @property
     def eth_802_1x_control(self) -> Eth802Dot1X:
         """802.1x Auth mode"""
-        return self._data["dot1x"]
+        return Eth802Dot1X(self._data["dot1x"])
 
     @property
     def lldp_med_enabled(self) -> bool:
         """LLDP Mode"""
         return self._data["lldpMedEnable"]
 
     @property
@@ -520,7 +531,133 @@
         """Latest firmware version available."""
         return self._data["lastFwVer"]
 
     @property
     def release_notes(self) -> str:
         """Release notes for the new firmware."""
         return self._data["fwReleaseLog"]
+
+class OmadaGatewayPort(OmadaApiData):
+
+    
+    @property
+    def port_number(self) -> int:
+        return self._data["port"]
+
+    @property
+    def name(self) -> str:
+        """Port name"""
+        return self._data["name"]
+
+    @property
+    def type(self) -> GatewayPortType:
+        """Type of the port - SFP, WAN, WAN/LAN or LAN only."""
+        return GatewayPortType(self._data["type"])
+
+    @property
+    def mode(self) -> GatewayPortMode:
+        """Whether the port is operating in WAN or LAN mode"""
+        return GatewayPortMode(self._data["mode"])
+
+    @property
+    def link_status(self) -> LinkStatus:
+        """Low level connectivity status of the link."""
+        # Defined differently to switches, so mangle the values to match
+        return LinkStatus.LINK_UP if self._data["status"] == 1 else LinkStatus.LINK_DOWN
+
+    @property
+    def wan_connected(self) -> bool:
+        """True if the port is connected to the internet/WAN"""
+        return self._data.get("internetState", 0) != 0
+
+    @property
+    def ip(self) -> Union[str, None]:
+        """The WAN IP of the port (for WAN ports only)"""
+        return self._data.get("ip")
+
+    @property
+    def link_speed(self) -> LinkSpeed:
+        """The established link speed of the port"""
+        return LinkSpeed(self._data.get("speed", LinkSpeed.SPEED_10_MBPS))
+
+    @property
+    def link_duplex(self) -> LinkDuplex:
+        """Actual duplex mode of the port"""
+        return LinkDuplex(self._data.get("duplex", LinkDuplex.FULL))
+
+    @property
+    def wan_protocol(self) -> Union[str, None]:
+        """May be: static, dhcp, pppoe, l2tp, pptp """
+        return self._data.get("proto")
+
+    # For connected ports
+    #"rxPkt":217028151,"rxPktRate":35,"rxRate":6,"tx":15157457326,"txPkt":60843861,"txPktRate":24,"txRate":5,
+    # "mirroredPorts":[]
+
+    # FOR WAN PORTS:
+    # "wanPortIpv6Config":{"enable":0,"addr":"","gateway":"","priDns":"","sndDns":"","internetState":0},
+    # "wanPortIpv4Config":{"ip":"x.x.x.x","gateway":"x.x.x.x","gateway2":"0.0.0.0","priDns":"194.168.4.100","sndDns":"194.168.8.100","priDns2":"0.0.0.0","sndDns2":"0.0.0.0"}
+
+
+class OmadaGatewayPortConfig(OmadaApiData):
+    @property
+    def port_number(self) -> int:
+        """Port number"""
+        return self._data["port"]
+
+    @property
+    def duplex(self) -> LinkDuplex:
+        """Configured duplex mode for the port."""
+        return self._data.get("duplex", LinkDuplex.AUTO)
+
+    @property
+    def link_speed(self) -> LinkSpeed:
+        """Configured link speed for the port."""
+        return self._data.get("linkSpeed", LinkSpeed.SPEED_AUTO)
+
+    @property
+    def mirror_enable(self) -> bool:
+        """True if port mirroring is enabled"""
+        return self._data.get("mirrorEnable", False)
+
+    @property
+    def port_status(self) -> OmadaGatewayPort:
+        """Full status of the port"""
+        return OmadaGatewayPort(self._data["portStat"])
+
+class OmadaGateway(OmadaDevice):
+
+    @property
+    def number_of_ports(self) -> int:
+        """The number of ports on the switch."""
+        return self._data.get("portNum", 0)
+
+    @property
+    def supports_poe(self) -> bool:
+        """True if the device supports PoE."""
+        return self._data["supportPoe"]
+
+    @property
+    def ip(self) -> str:
+        """Gateway's LAN IP address."""
+        return self._data["ip"]
+        
+    @property
+    def port_status(self) -> List[OmadaGatewayPort]:
+        """Status of the gateway's ports."""
+        return [
+            OmadaGatewayPort(p) for p in self._data["portStats"]
+        ]
+
+    @property 
+    def port_configs(self) -> List[OmadaGatewayPortConfig]:
+        """Configuration of the gateway's ports. Also includes status..."""
+        return [
+            OmadaGatewayPortConfig(p) for p in self._data["portConfigs"]
+        ]
+
+    @property
+    def is_combined_gateway(self) -> bool:
+        """True if this is a combined gateway/switch."""
+        return self._data.get("combinedGateway", False)
+
+
```

### Comparing `tplink_omada_client-1.2.3/src/tplink_omada_client/exceptions.py` & `tplink_omada_client-1.2.4/src/tplink_omada_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.3/src/tplink_omada_client/omadaapiconnection.py` & `tplink_omada_client-1.2.4/src/tplink_omada_client/omadaapiconnection.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.3/src/tplink_omada_client/omadaclient.py` & `tplink_omada_client-1.2.4/src/tplink_omada_client/omadaclient.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.3/src/tplink_omada_client/omadasiteclient.py` & `tplink_omada_client-1.2.4/src/tplink_omada_client/omadasiteclient.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import List, Optional, Union
 from .omadaapiconnection import OmadaApiConnection
 
 from .devices import (
     OmadaAccessPoint,
     OmadaDevice,
     OmadaFirmwareUpdate,
+    OmadaGateway,
     OmadaListDevice,
     OmadaPortProfile,
     OmadaSwitch,
     OmadaSwitchPort,
     OmadaSwitchPortDetails,
     OmadaAccesPointLanPortSettings,
 )
@@ -313,7 +314,37 @@
         await self._api.request(
             "post",
             self._api.format_url(f"cmd/devices/{mac}/onlineUpgrade", self._site_id),
             payload=payload,
         )
 
         return True
+
+    async def get_gateways(self) -> List[OmadaGateway]:
+        """Get the list of gateways (routers) on the site. (Zero or one!)"""
+
+        return [
+            await self.get_gateway(d)
+            for d in await self.get_devices()
+            if d.type == "gateway"
+        ]
+
+    async def get_gateway(self, mac_or_device: Union[str, OmadaDevice, None]) -> OmadaGateway:
+        """Get the gatway (router) for the site by Mac address or Omada device. (There can be only one!)"""
+
+        if mac_or_device is None:
+            mac_or_device = next((d for d in await self.get_devices() if d.type == "gateway"), None)
+            if mac_or_device is None:
+                raise InvalidDevice("No gateways found in site")
+
+        if isinstance(mac_or_device, OmadaDevice):
+            if mac_or_device.type != "gateway":
+                raise InvalidDevice()
+            mac = mac_or_device.mac
+        else:
+            mac = mac_or_device
+
+        result = await self._api.request(
+            "get", self._api.format_url(f"gateways/{mac}", self._site_id)
+        )
+
+        return OmadaGateway(result)
```

### Comparing `tplink_omada_client-1.2.3/src/tplink_omada_client/cli/__init__.py` & `tplink_omada_client-1.2.4/src/tplink_omada_client/cli/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 from . import (
     command_devices,
     command_switch,
     command_switches,
     command_target,
     command_targets,
-    command_default
+    command_default,
+    command_gateway
 )
 
 def main(argv: Union[Sequence[str], None] = None) -> int:
     """Entry point for Omada CLI"""
     if argv is None:
         argv = sys.argv[1:]
     parser = argparse.ArgumentParser()
@@ -33,14 +34,15 @@
 
     command_devices.arg_parser(subparsers)
     command_switch.arg_parser(subparsers)
     command_switches.arg_parser(subparsers)
     command_target.arg_parser(subparsers)
     command_targets.arg_parser(subparsers)
     command_default.arg_parser(subparsers)
+    command_gateway.arg_parser(subparsers)
 
     try:
         args = parser.parse_args(args=argv)
         if "func" in args:
             return asyncio.run(args.func(vars(args)))
         parser.print_help()
         return 1
```

### Comparing `tplink_omada_client-1.2.3/src/tplink_omada_client/cli/command_default.py` & `tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_default.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.3/src/tplink_omada_client/cli/command_devices.py` & `tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_devices.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     """Executes 'devices' command"""
     controller = get_target_argument(args)
     config = get_target_config(controller)
 
     async with to_omada_connection(config) as client:
         site_client = await client.get_site_client(config.site)
         for device in await site_client.get_devices():
-            print(f"{device.mac} {device.ip_address:>15} {device.type:>7}  {device.name:20} {device.model_display_name}")
+            print(f"{device.mac} {device.ip_address:>15} {device.type:>7} {device.status_category.name:16} {device.name:20} {device.model_display_name}")
             dump_raw_data(args, device)
     return 0
 
 def arg_parser(subparsers: _SubParsersAction) -> None:
     """Configures arguments parser for 'devices' command"""
     devices_parser = subparsers.add_parser(
         "devices",
```

### Comparing `tplink_omada_client-1.2.3/src/tplink_omada_client/cli/command_switch.py` & `tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_switch.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
     async with to_omada_connection(config) as client:
         site_client = await client.get_site_client(config.site)
         mac = await get_mac(site_client, args['mac'])
         switch = await site_client.get_switch(mac)
         print(f"Name: {switch.name}")
         print(f"Address: {switch.mac} ({switch.ip_address})")
+        print(f"Status: {switch.status.name} ({switch.status_category.name})")
         print(f"Ports: {switch.number_of_ports}")
         print(f"Supports PoE: {switch.device_capabilities.supports_poe}")
         if switch.device_capabilities.supports_poe:
             print(f"PoE ports: {switch.device_capabilities.poe_ports}")
         print(f"Model: {switch.model_display_name}")
         switch.status_category
         print(f"Uptime: {switch.display_uptime}")
```

### Comparing `tplink_omada_client-1.2.3/src/tplink_omada_client/cli/command_switches.py` & `tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_switches.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.3/src/tplink_omada_client/cli/command_target.py` & `tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_target.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.3/src/tplink_omada_client/cli/command_targets.py` & `tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_targets.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.3/src/tplink_omada_client/cli/config.py` & `tplink_omada_client-1.2.4/src/tplink_omada_client/cli/config.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.3/src/tplink_omada_client/cli/util.py` & `tplink_omada_client-1.2.4/src/tplink_omada_client/cli/util.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.3/LICENSE` & `tplink_omada_client-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.3/README.md` & `tplink_omada_client-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.3/pyproject.toml` & `tplink_omada_client-1.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tplink_omada_client"
-version = "1.2.3"
+version = "1.2.4"
 authors = [
   { name="Mark Godwin", email="author@example.com" },
 ]
 description = "Python wrapper for TP-Link Omada SDN Controller API (OC200/OC300/Software Controller)"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `tplink_omada_client-1.2.3/PKG-INFO` & `tplink_omada_client-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tplink_omada_client
-Version: 1.2.3
+Version: 1.2.4
 Summary: Python wrapper for TP-Link Omada SDN Controller API (OC200/OC300/Software Controller)
 Project-URL: Homepage, https://github.com/MarkGodwin/tplink-omada-api
 Project-URL: Bug Tracker, https://github.com/MarkGodwin/tplink-omada-api/issues
 Author-email: Mark Godwin <author@example.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

