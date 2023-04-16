# Comparing `tmp/clevertouch-0.3.0.tar.gz` & `tmp/clevertouch-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clevertouch-0.3.0.tar", last modified: Mon Mar 13 13:22:50 2023, max compression
+gzip compressed data, was "clevertouch-0.4.0.tar", last modified: Sun Apr 16 12:47:19 2023, max compression
```

## Comparing `clevertouch-0.3.0.tar` & `clevertouch-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1064 2023-01-24 14:28:50.216215 clevertouch-0.3.0/LICENSE
--rw-r--r--   0        0        0     5073 2023-03-13 13:06:21.888575 clevertouch-0.3.0/README.md
--rw-r--r--   0        0        0     1022 2023-03-13 13:13:09.610364 clevertouch-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      183 2023-01-31 10:59:22.202682 clevertouch-0.3.0/src/clevertouch/__init__.py
--rw-r--r--   0        0        0     6679 2023-03-13 13:06:21.888575 clevertouch-0.3.0/src/clevertouch/api.py
--rw-r--r--   0        0        0      206 2023-03-09 11:16:19.367070 clevertouch-0.3.0/src/clevertouch/devices/__init__.py
--rw-r--r--   0        0        0      373 2023-03-13 13:06:21.888575 clevertouch-0.3.0/src/clevertouch/devices/const.py
--rw-r--r--   0        0        0     1193 2023-03-09 11:33:26.233110 clevertouch-0.3.0/src/clevertouch/devices/device.py
--rw-r--r--   0        0        0      900 2023-03-13 13:06:21.888575 clevertouch-0.3.0/src/clevertouch/devices/factory.py
--rw-r--r--   0        0        0     2023 2023-03-09 11:13:52.013655 clevertouch-0.3.0/src/clevertouch/devices/onoff.py
--rw-r--r--   0        0        0     7800 2023-03-09 11:25:33.806268 clevertouch-0.3.0/src/clevertouch/devices/radiator.py
--rw-r--r--   0        0        0     1522 2023-01-31 10:59:22.206682 clevertouch-0.3.0/src/clevertouch/info.py
--rw-r--r--   0        0        0     4214 2023-03-13 13:06:21.888575 clevertouch-0.3.0/src/clevertouch/objects.py
--rw-r--r--   0        0        0      836 2023-01-31 10:59:22.206682 clevertouch-0.3.0/src/clevertouch/util.py
--rw-r--r--   0        0        0       37 2023-01-24 22:11:22.095324 clevertouch-0.3.0/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-01-24 22:11:22.095324 clevertouch-0.3.0/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2023-01-24 22:11:22.095324 clevertouch-0.3.0/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0      103 2023-01-24 22:34:04.437950 clevertouch-0.3.0/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      128 2023-01-24 22:34:04.437950 clevertouch-0.3.0/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-01-24 22:34:04.437950 clevertouch-0.3.0/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     1109 2023-01-31 10:59:22.206682 clevertouch-0.3.0/tests/authenticate_test.py
--rw-r--r--   0        0        0     5684 1970-01-01 00:00:00.000000 clevertouch-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-01-24 14:28:50.216215 clevertouch-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5073 2023-03-13 13:06:21.888575 clevertouch-0.4.0/README.md
+-rw-r--r--   0        0        0     1022 2023-04-16 12:46:43.653638 clevertouch-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-01-31 10:59:22.202682 clevertouch-0.4.0/src/clevertouch/__init__.py
+-rw-r--r--   0        0        0     6679 2023-03-13 13:06:21.888575 clevertouch-0.4.0/src/clevertouch/api.py
+-rw-r--r--   0        0        0      206 2023-03-09 11:16:19.367070 clevertouch-0.4.0/src/clevertouch/devices/__init__.py
+-rw-r--r--   0        0        0      373 2023-03-13 13:06:21.888575 clevertouch-0.4.0/src/clevertouch/devices/const.py
+-rw-r--r--   0        0        0     1193 2023-03-09 11:33:26.233110 clevertouch-0.4.0/src/clevertouch/devices/device.py
+-rw-r--r--   0        0        0      900 2023-03-13 13:06:21.888575 clevertouch-0.4.0/src/clevertouch/devices/factory.py
+-rw-r--r--   0        0        0     2023 2023-03-09 11:13:52.013655 clevertouch-0.4.0/src/clevertouch/devices/onoff.py
+-rw-r--r--   0        0        0    11703 2023-04-15 06:05:19.193436 clevertouch-0.4.0/src/clevertouch/devices/radiator.py
+-rw-r--r--   0        0        0     1522 2023-01-31 10:59:22.206682 clevertouch-0.4.0/src/clevertouch/info.py
+-rw-r--r--   0        0        0     4214 2023-03-13 13:06:21.888575 clevertouch-0.4.0/src/clevertouch/objects.py
+-rw-r--r--   0        0        0      836 2023-01-31 10:59:22.206682 clevertouch-0.4.0/src/clevertouch/util.py
+-rw-r--r--   0        0        0       37 2023-01-24 22:11:22.095324 clevertouch-0.4.0/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2023-01-24 22:11:22.095324 clevertouch-0.4.0/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2023-01-24 22:11:22.095324 clevertouch-0.4.0/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0      103 2023-01-24 22:34:04.437950 clevertouch-0.4.0/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      128 2023-01-24 22:34:04.437950 clevertouch-0.4.0/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2023-01-24 22:34:04.437950 clevertouch-0.4.0/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0     1109 2023-01-31 10:59:22.206682 clevertouch-0.4.0/tests/authenticate_test.py
+-rw-r--r--   0        0        0     5684 1970-01-01 00:00:00.000000 clevertouch-0.4.0/PKG-INFO
```

### Comparing `clevertouch-0.3.0/LICENSE` & `clevertouch-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clevertouch-0.3.0/README.md` & `clevertouch-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `clevertouch-0.3.0/pyproject.toml` & `clevertouch-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 [tool.pytest.ini_options]
 log_cli = 1
 log_cli_level = "DEBUG"
 
 [project]
 name = "clevertouch"
-version = "0.3.0"
+version = "0.4.0"
 description = "A Python API for interacting with LVI/Purmo Touch E3-connected radiators"
 keywords = [
     "LVI",
     "home automation",
     "heating",
 ]
 authors = [
```

### Comparing `clevertouch-0.3.0/src/clevertouch/api.py` & `clevertouch-0.4.0/src/clevertouch/api.py`

 * *Files identical despite different names*

### Comparing `clevertouch-0.3.0/src/clevertouch/devices/device.py` & `clevertouch-0.4.0/src/clevertouch/devices/device.py`

 * *Files identical despite different names*

### Comparing `clevertouch-0.3.0/src/clevertouch/devices/factory.py` & `clevertouch-0.4.0/src/clevertouch/devices/factory.py`

 * *Files identical despite different names*

### Comparing `clevertouch-0.3.0/src/clevertouch/devices/onoff.py` & `clevertouch-0.4.0/src/clevertouch/devices/onoff.py`

 * *Files identical despite different names*

### Comparing `clevertouch-0.3.0/src/clevertouch/devices/radiator.py` & `clevertouch-0.4.0/src/clevertouch/devices/radiator.py`

 * *Files 26% similar despite different names*

```diff
@@ -58,17 +58,25 @@
     }
 
     _HEAT_MODE_TO_DEVICE: dict[str, str] = {
         HeatMode.ECO: "3",
         HeatMode.FROST: "2",
         HeatMode.COMFORT: "0",
         HeatMode.PROGRAM: "11",
+        HeatMode.BOOST: "4",
         HeatMode.OFF: "1",
     }
 
+    _HEAT_MODE_TO_WRITABLE_TEMP_TYPE: dict[str, str] = {
+        HeatMode.ECO: TempType.ECO,
+        HeatMode.FROST: TempType.FROST,
+        HeatMode.COMFORT: TempType.COMFORT,
+        HeatMode.BOOST: TempType.BOOST,
+    }
+
     _TEMP_TYPE_TO_DEVICE: dict[str, str] = {
         TempType.ECO: "consigne_eco",
         TempType.FROST: "consigne_hg",
         TempType.COMFORT: "consigne_confort",
         TempType.CURRENT: "temperature_air",
         TempType.MANUAL: "consigne_manuel",
         TempType.BOOST: "consigne_boost",
@@ -81,31 +89,40 @@
         TempType.CURRENT,
         TempType.BOOST,
     ]
 
     _READONLY_TEMP_TYPES: list[str] = [
         TempType.CURRENT,
         TempType.TARGET,
-        TempType.BOOST,
     ]
 
     _AVAILABLE_HEAT_MODES: list[str] = [
         HeatMode.COMFORT,
         HeatMode.ECO,
         HeatMode.FROST,
         HeatMode.PROGRAM,
+        HeatMode.BOOST,
         HeatMode.OFF,
     ]
 
     def __init__(self, session: ApiSession, home: HomeInfo, data: dict) -> None:
-        super().__init__(session, home, data, DeviceType.RADIATOR, DeviceTypeId.RADIATOR, do_update=False)
+        super().__init__(
+            session,
+            home,
+            data,
+            DeviceType.RADIATOR,
+            DeviceTypeId.RADIATOR,
+            do_update=False,
+        )
         self.modes: list[str] = self._AVAILABLE_HEAT_MODES
         self.active: bool = False
         self.heat_mode = HeatMode.OFF
         self.temp_type = TempType.NONE
+        self.boost_time: int = 0
+        self.boost_remaining: int = 0
         self.temperatures: dict[str, Temperature] = {}
         self.update(data)
 
     def update(self, data: dict[str, Any]):
         """Update the radiator from cloud API data."""
         super().update(data)
         mode_num = data["gv_mode"]
@@ -124,66 +141,151 @@
         self.temperatures[TempType.TARGET] = Temperature(
             None
             if self.temp_type == TempType.NONE
             else self.temperatures[self.temp_type].device,
             is_writable=False,
             name=TempType.TARGET,
         )
+        # Read boost settings
+        # 'boost_time' is the user writable boost time
+        try:
+            self.boost_time = int(data["time_boost"])
+        except KeyError:  # The key doesn't exist
+            self.boost_time = 0
+        except ValueError:  # The value can not be converted to an int
+            self.boost_time = 0
+        # 'time_boost_format_chrono' holds remaining boost time with higher resolution
+        try:
+            node = data["time_boost_format_chrono"]
+            self.boost_remaining = (
+                int(node["d"]) * 24 * 60 * 60
+                + int(node["h"]) * 60 * 60
+                + int(node["m"]) * 60
+                + int(node["s"])
+            )
+        except KeyError:
+            self.boost_remaining = 0
+        except ValueError:
+            self.boost_remaining = 0
 
     async def set_temperature(self, temp_type: str, temp_value: float, unit: str):
         """Set a specific temperature for a radiator"""
         if temp_type not in self._TEMP_TYPE_TO_DEVICE:
             raise ApiError(f"Temperature {temp_type} not available.")
         elif temp_type in self._READONLY_TEMP_TYPES:
             raise ApiError(f"Temperature {temp_type} is read-only.")
 
-        new_temp = Temperature(
-            temp_value,
-            unit,
-            is_writable=True,
-            name=temp_type)
+        new_temp = Temperature(temp_value, unit, is_writable=True, name=temp_type)
 
         query_params = {}
         query_params["id_device"] = self.id_local
         query_params[Radiator._TEMP_TYPE_TO_DEVICE[temp_type]] = new_temp.device
 
         await self._session.write_query(self.home.home_id, query_params)
 
         # This is debatable - for some scenarios it is reasonable to
         # update the value in the current object with the assumed
         # change, for others not
         self.temperatures[temp_type] = new_temp
 
         # To further complicate. If the temp_type set is the same type
         # that the object currently targets, that value should be updated as well
-        if temp_type==self.temp_type:
+        if temp_type == self.temp_type:
             self.temperatures[TempType.TARGET] = Temperature(
                 new_temp.device,
                 is_writable=False,
                 name=TempType.TARGET,
             )
 
-
     async def set_heat_mode(self, heat_mode: str):
         """Set a the heating mode for a radiator"""
         if heat_mode not in self._HEAT_MODE_TO_DEVICE:
             raise ApiError(f"Heating mode {heat_mode} not available.")
 
         query_params = {}
         query_params["id_device"] = self.id_local
         query_params["gv_mode"] = self._HEAT_MODE_TO_DEVICE[heat_mode]
         query_params["nv_mode"] = self._HEAT_MODE_TO_DEVICE[heat_mode]
 
         await self._session.write_query(self.home.home_id, query_params)
 
-        # This is debatable - for some scenarios it is reasonable to
-        # update the value in the current object with the assumed
-        # change, for others not
+        # Debatable - see set_temperature
         self.heat_mode = heat_mode
 
+    async def set_boost_time(self, boost_time: int) -> None:
+        """Set default boost time for subsequent activations of boost mode"""
+
+        query_params = {}
+        query_params["id_device"] = self.id_local
+        query_params["time_boost"] = boost_time
+
+        await self._session.write_query(self.home.home_id, query_params)
+
+        # Debatable - see set_temperature
+        self.boost_time = boost_time
+
+    async def activate_mode(
+        self,
+        heat_mode: str,
+        *,
+        temp_value: Optional[float] = None,
+        temp_unit: Optional[str] = None,
+        boost_time: Optional[int] = None,
+    ) -> None:
+        """
+        Set the heating mode, optionally adjusting parameters.
+
+        Parameters:
+        heat_mode : str
+            Heat mode to activate. Should be one of the `HeatMode` constants.
+        temp_value : float, optional
+            Temperature value. Must be used together with `temp_unit`.
+        temp_unit : str, optional
+            Unit of `temp_value`. Should be `celsius`, `farenheit` or `device`.
+        boost_time : int, optional
+            Length of period that boost mode should be active, in seconds.
+            Applicable to `HeatMode.Boost` only.
+
+        Raises:
+        ApiError
+            If any of the arguments are invalid or incompatible.
+        """
+
+        if heat_mode not in self._HEAT_MODE_TO_DEVICE:
+            raise ApiError(f"Heating mode {heat_mode} not available.")
+        if (temp_value or temp_unit) and (not temp_value or not temp_unit):
+            raise ApiError("Both temp value and unit must be set.")
+        if temp_value and heat_mode not in self._HEAT_MODE_TO_WRITABLE_TEMP_TYPE:
+            raise ApiError(f"Temperature can not be set for {heat_mode}.")
+        if boost_time and heat_mode != HeatMode.BOOST:
+            raise ApiError("Boost time can only be set for boost mode.")
+
+        query_params = {}
+        query_params["id_device"] = self.id_local
+        query_params["gv_mode"] = self._HEAT_MODE_TO_DEVICE[heat_mode]
+        query_params["nv_mode"] = self._HEAT_MODE_TO_DEVICE[heat_mode]
+
+        if temp_value:
+            temp_type = self._HEAT_MODE_TO_WRITABLE_TEMP_TYPE[heat_mode]
+            new_temp = Temperature(
+                temp_value, temp_unit, is_writable=True, name=temp_type
+            )
+            query_params[self._TEMP_TYPE_TO_DEVICE[temp_type]] = new_temp.device
+            # Debatable - see set_temperature
+            self.temperatures[temp_type] = new_temp
+            self.temperatures[TempType.TARGET] = new_temp
+
+        if boost_time:
+            query_params["time_boost"] = boost_time
+            # Debatable - see set_temperature
+            self.boost_time = boost_time
+            self.boost_remaining = boost_time
+
+        await self._session.write_query(self.home.home_id, query_params)
+
 
 class TempUnit(StrEnum):
     """Enum of available temperature units."""
 
     DEVICE = "device"
     CELSIUS = "celsius"
     FARENHEIT = "farenheit"
```

### Comparing `clevertouch-0.3.0/src/clevertouch/info.py` & `clevertouch-0.4.0/src/clevertouch/info.py`

 * *Files identical despite different names*

### Comparing `clevertouch-0.3.0/src/clevertouch/objects.py` & `clevertouch-0.4.0/src/clevertouch/objects.py`

 * *Files identical despite different names*

### Comparing `clevertouch-0.3.0/src/clevertouch/util.py` & `clevertouch-0.4.0/src/clevertouch/util.py`

 * *Files identical despite different names*

### Comparing `clevertouch-0.3.0/tests/authenticate_test.py` & `clevertouch-0.4.0/tests/authenticate_test.py`

 * *Files identical despite different names*

### Comparing `clevertouch-0.3.0/PKG-INFO` & `clevertouch-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevertouch
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Python API for interacting with LVI/Purmo Touch E3-connected radiators
 License: MIT
 Keywords: LVI,home automation,heating
 Author-email: hemphen <michael.hemph@gmail.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

