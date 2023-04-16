# Comparing `tmp/srf_weather-0.1.0.tar.gz` & `tmp/srf_weather-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srf_weather-0.1.0.tar", max compression
+gzip compressed data, was "srf_weather-0.1.1.tar", max compression
```

## Comparing `srf_weather-0.1.0.tar` & `srf_weather-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-04-16 06:54:49.835032 srf_weather-0.1.0/LICENSE
--rw-r--r--   0        0        0     1137 2023-04-16 07:20:21.787885 srf_weather-0.1.0/README.md
--rw-r--r--   0        0        0      777 2023-04-16 07:22:48.451313 srf_weather-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-16 06:45:43.691653 srf_weather-0.1.0/srf_weather/__init__.py
--rw-r--r--   0        0        0      409 2023-04-16 06:45:08.564095 srf_weather-0.1.0/srf_weather/main.py
--rw-r--r--   0        0        0     4140 2023-04-16 07:11:44.586288 srf_weather-0.1.0/srf_weather/weather.py
--rw-r--r--   0        0        0     1721 1970-01-01 00:00:00.000000 srf_weather-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-16 06:54:49.835032 srf_weather-0.1.1/LICENSE
+-rw-r--r--   0        0        0      303 2023-04-16 12:03:26.631518 srf_weather-0.1.1/README.rst
+-rw-r--r--   0        0        0     1033 2023-04-16 15:27:54.013689 srf_weather-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-16 13:58:48.945899 srf_weather-0.1.1/srf_weather/__init__.py
+-rw-r--r--   0        0        0      420 2023-04-16 15:30:22.052551 srf_weather-0.1.1/srf_weather/main.py
+-rw-r--r--   0        0        0     4651 2023-04-16 15:32:38.839517 srf_weather-0.1.1/srf_weather/weather.py
+-rw-r--r--   0        0        0     1072 1970-01-01 00:00:00.000000 srf_weather-0.1.1/PKG-INFO
```

### Comparing `srf_weather-0.1.0/LICENSE` & `srf_weather-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `srf_weather-0.1.0/pyproject.toml` & `srf_weather-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 [tool.poetry]
 name = "srf-weather"
-version = "0.1.0"
+version = "0.1.1"
 description = "A weather app for SRF"
 authors = ["Andreas Weier <andreas.weier.open.source@gmail.com>"]
-readme = "README.md"
+homepage = "https://github.com/weieran/SRF-Weather"
+repository = "https://github.com/weieran/SRF-Weather"
+documentation = "https://srf-weather.readthedocs.io/en/latest/"
+readme = "README.rst"
 packages = [{include = "srf_weather"}]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ["^3.10", "^3.8"]
 requests = "^2.28.2"
 
 [tool.poetry.scripts]
 srf-weather = "srf_weater.main:main"
 
+[tool.poetry.group.dev.dependencies]
+sphinx = "^6.1.3"
+sphinx-rtd-theme = "^1.2.0"
+
 [tool.coverage.run]
 branch = true
 source = ["srf_weather"]
 
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.tox.coverage.report]
 exclude_lines = [
     "pragma: no cover",
```

### Comparing `srf_weather-0.1.0/srf_weather/weather.py` & `srf_weather-0.1.1/srf_weather/weather.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 from enum import Enum
 import requests
 from datetime import datetime, timedelta
+import urllib.parse
 
 
 class InvalidTokenException(Exception):
     """Raised when the received access token is invalid """
     pass
 
 
@@ -42,29 +43,30 @@
         self.headers = None
         self.geo_location_id = self.get_geo_location_id(location)
 
     def _get_headers(self):
         if self.last_header_update is None or self.last_header_update + self.TOKEN_VALIDITY_DAY < datetime.now():
             self.logger.debug("Updating token, as it is older than 7 days")
             self.last_header_update = datetime.now()
-            access_token = self.get_access_token()
+            access_token = self.get_access_token(self.logger, self.client_id, self.client_secret)
             self.headers = {'Authorization': f"Bearer {access_token}"}
         return self.headers
 
-    def get_access_token(self):
+    @staticmethod
+    def get_access_token(logger: logging.Logger = None, client_id: str = None, client_secret: str = None):
         # Define the authentication API endpoint URL and parameters
         url = "https://api.srgssr.ch/oauth/v1/accesstoken"
         params = {
             "grant_type": "client_credentials"
         }
 
         # Send a POST request to the authentication API endpoint
-        response = requests.post(url, params=params, auth=(self.client_id, self.client_secret))
+        response = requests.post(url, params=params, auth=(client_id, client_secret))
         if not response.ok:
-            self.logger.error(f"Invalid token, response: {response.status_code}  ")
+            logger.error(f"Invalid token, response: {response.status_code}  ")
             raise InvalidTokenException
 
         # Parse the JSON response data
         data = response.json()
 
         # Extract the access token from the response data
         return data["access_token"]
@@ -90,16 +92,21 @@
         return geo_location_id
 
     class ForecastDuration(Enum):
         minutes60 = "60minutes"
         hour = "hour"
         day = "day"
 
+    @staticmethod
+    def get_weather_forcast_url(location_id: str):
+        url = f"https://api.srgssr.ch/srf-meteo/forecast/{urllib.parse.quote(location_id)}"
+        return url
+
     def get_weather_forecast(self, forcast_duration: ForecastDuration):
-        url = f"https://api.srgssr.ch/srf-meteo/forecast/{self.geo_location_id}"
+        url = self.get_weather_forcast_url(self.geo_location_id)
         params = {"type": forcast_duration.value}
 
         # Send a GET request to the API endpoint
         response = requests.get(url, params=params, headers=self._get_headers())
 
         if response.status_code != 200:
             self.logger.error(f"Invalid weather, response: {response.status_code}  ")
@@ -108,7 +115,13 @@
         # Parse the JSON response data
         data = response.json()
 
         # Extract the forecast data from the response data
         forecast = data["forecast"]
 
         return forecast
+
+    @staticmethod
+    def get_hours_of_sun(forecast):
+        sun_h_today = forecast["day"][0]["SUN_H"]
+        sun_h_tomorrow = forecast["day"][1]["SUN_H"]
+        return sun_h_today, sun_h_tomorrow
```

