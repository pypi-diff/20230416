# Comparing `tmp/wg_utilities-3.4.0.tar.gz` & `tmp/wg_utilities-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wg_utilities-3.4.0.tar", max compression
+gzip compressed data, was "wg_utilities-3.4.1.tar", max compression
```

## Comparing `wg_utilities-3.4.0.tar` & `wg_utilities-3.4.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1069 2023-04-16 12:36:50.156112 wg_utilities-3.4.0/LICENSE
--rw-r--r--   0        0        0     2297 2023-04-16 12:36:50.156112 wg_utilities-3.4.0/README.md
--rw-r--r--   0        0        0     4825 2023-04-16 12:36:50.160112 wg_utilities-3.4.0/pyproject.toml
--rw-r--r--   0        0        0      280 2023-04-16 12:36:50.236112 wg_utilities-3.4.0/wg_utilities/__init__.py
--rw-r--r--   0        0        0      140 2023-04-16 12:36:50.236112 wg_utilities-3.4.0/wg_utilities/api/__init__.py
--rw-r--r--   0        0        0     7384 2023-04-16 12:36:50.236112 wg_utilities-3.4.0/wg_utilities/api/temp_auth_server.py
--rw-r--r--   0        0        0      685 2023-04-16 12:36:50.236112 wg_utilities-3.4.0/wg_utilities/clients/__init__.py
--rw-r--r--   0        0        0     4305 2023-04-16 12:36:50.236112 wg_utilities-3.4.0/wg_utilities/clients/_google.py
--rw-r--r--   0        0        0    10390 2023-04-16 12:36:50.236112 wg_utilities-3.4.0/wg_utilities/clients/_spotify_types.py
--rw-r--r--   0        0        0    24119 2023-04-16 12:36:50.236112 wg_utilities-3.4.0/wg_utilities/clients/google_calendar.py
--rw-r--r--   0        0        0    56540 2023-04-16 12:36:50.236112 wg_utilities-3.4.0/wg_utilities/clients/google_drive.py
--rw-r--r--   0        0        0     7566 2023-04-16 12:36:50.236112 wg_utilities-3.4.0/wg_utilities/clients/google_fit.py
--rw-r--r--   0        0        0    13531 2023-04-16 12:36:50.236112 wg_utilities-3.4.0/wg_utilities/clients/google_photos.py
--rw-r--r--   0        0        0    15632 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/clients/monzo.py
--rw-r--r--   0        0        0    26578 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/clients/oauth_client.py
--rw-r--r--   0        0        0    49179 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/clients/spotify.py
--rw-r--r--   0        0        0    21832 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/clients/truelayer.py
--rw-r--r--   0        0        0      126 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/devices/__init__.py
--rw-r--r--   0        0        0      119 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/devices/dht22/__init__.py
--rwxr-xr-x   0        0        0     6642 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/devices/dht22/dht22_lib.py
--rw-r--r--   0        0        0     1129 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/devices/epd/__init__.py
--rw-r--r--   0        0        0     7042 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/devices/epd/epd7in5_v2.py
--rw-r--r--   0        0        0     6041 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/devices/epd/epdconfig.py
--rw-r--r--   0        0        0      138 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/devices/yamaha_yas_209/__init__.py
--rw-r--r--   0        0        0    36374 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py
--rw-r--r--   0        0        0     5401 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/exceptions/__init__.py
--rw-r--r--   0        0        0      803 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/functions/__init__.py
--rw-r--r--   0        0        0     4595 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/functions/_functions.py
--rw-r--r--   0        0        0     1287 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/functions/datetime_helpers.py
--rw-r--r--   0        0        0     2024 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/functions/file_management.py
--rw-r--r--   0        0        0     8877 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/functions/json.py
--rw-r--r--   0        0        0     1386 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/functions/processes.py
--rw-r--r--   0        0        0     1106 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/functions/string_manipulation.py
--rw-r--r--   0        0        0     1586 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/functions/xml.py
--rw-r--r--   0        0        0     7258 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/loggers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/py.typed
--rw-r--r--   0        0        0      167 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/testing/__init__.py
--rw-r--r--   0        0        0     5257 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/testing/_custom_mocks.py
--rw-r--r--   0        0        0     4113 1970-01-01 00:00:00.000000 wg_utilities-3.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-16 21:52:36.053445 wg_utilities-3.4.1/LICENSE
+-rw-r--r--   0        0        0     2297 2023-04-16 21:52:36.053445 wg_utilities-3.4.1/README.md
+-rw-r--r--   0        0        0     4825 2023-04-16 21:52:36.053445 wg_utilities-3.4.1/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/__init__.py
+-rw-r--r--   0        0        0      140 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/api/__init__.py
+-rw-r--r--   0        0        0     7384 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/api/temp_auth_server.py
+-rw-r--r--   0        0        0      685 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/clients/__init__.py
+-rw-r--r--   0        0        0     4305 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/clients/_google.py
+-rw-r--r--   0        0        0    10390 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/clients/_spotify_types.py
+-rw-r--r--   0        0        0    24119 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/clients/google_calendar.py
+-rw-r--r--   0        0        0    56540 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/clients/google_drive.py
+-rw-r--r--   0        0        0     7566 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/clients/google_fit.py
+-rw-r--r--   0        0        0    13531 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/clients/google_photos.py
+-rw-r--r--   0        0        0    15632 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/clients/monzo.py
+-rw-r--r--   0        0        0    26578 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/clients/oauth_client.py
+-rw-r--r--   0        0        0    49179 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/clients/spotify.py
+-rw-r--r--   0        0        0    22151 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/clients/truelayer.py
+-rw-r--r--   0        0        0      126 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/devices/__init__.py
+-rw-r--r--   0        0        0      119 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/devices/dht22/__init__.py
+-rwxr-xr-x   0        0        0     6642 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/devices/dht22/dht22_lib.py
+-rw-r--r--   0        0        0     1129 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/devices/epd/__init__.py
+-rw-r--r--   0        0        0     7042 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/devices/epd/epd7in5_v2.py
+-rw-r--r--   0        0        0     6041 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/devices/epd/epdconfig.py
+-rw-r--r--   0        0        0      138 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/devices/yamaha_yas_209/__init__.py
+-rw-r--r--   0        0        0    36374 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py
+-rw-r--r--   0        0        0     5401 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/exceptions/__init__.py
+-rw-r--r--   0        0        0      803 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/functions/__init__.py
+-rw-r--r--   0        0        0     4595 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/functions/_functions.py
+-rw-r--r--   0        0        0     1287 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/functions/datetime_helpers.py
+-rw-r--r--   0        0        0     2024 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/functions/file_management.py
+-rw-r--r--   0        0        0     8877 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/functions/json.py
+-rw-r--r--   0        0        0     1386 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/functions/processes.py
+-rw-r--r--   0        0        0     1106 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/functions/string_manipulation.py
+-rw-r--r--   0        0        0     1586 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/functions/xml.py
+-rw-r--r--   0        0        0     7258 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/loggers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/py.typed
+-rw-r--r--   0        0        0      167 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/testing/__init__.py
+-rw-r--r--   0        0        0     5257 2023-04-16 21:52:36.125445 wg_utilities-3.4.1/wg_utilities/testing/_custom_mocks.py
+-rw-r--r--   0        0        0     4113 1970-01-01 00:00:00.000000 wg_utilities-3.4.1/PKG-INFO
```

### Comparing `wg_utilities-3.4.0/LICENSE` & `wg_utilities-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/README.md` & `wg_utilities-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/pyproject.toml` & `wg_utilities-3.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wg-utilities"
-version = "3.4.0"
+version = "3.4.1"
 description = "Loads of useful stuff for the things I do :)"
 
 authors = ["Will Garside <worgarside@gmail.com>"]
 include = ["wg_utilities/py.typed"]
 license = "MIT"
 maintainers = ["Will Garside <worgarside@gmail.com>"]
 packages = [{ include = "wg_utilities" }]
```

### Comparing `wg_utilities-3.4.0/wg_utilities/api/temp_auth_server.py` & `wg_utilities-3.4.1/wg_utilities/api/temp_auth_server.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/clients/__init__.py` & `wg_utilities-3.4.1/wg_utilities/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/clients/_google.py` & `wg_utilities-3.4.1/wg_utilities/clients/_google.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/clients/_spotify_types.py` & `wg_utilities-3.4.1/wg_utilities/clients/_spotify_types.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/clients/google_calendar.py` & `wg_utilities-3.4.1/wg_utilities/clients/google_calendar.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/clients/google_drive.py` & `wg_utilities-3.4.1/wg_utilities/clients/google_drive.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/clients/google_fit.py` & `wg_utilities-3.4.1/wg_utilities/clients/google_fit.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/clients/google_photos.py` & `wg_utilities-3.4.1/wg_utilities/clients/google_photos.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/clients/monzo.py` & `wg_utilities-3.4.1/wg_utilities/clients/monzo.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/clients/oauth_client.py` & `wg_utilities-3.4.1/wg_utilities/clients/oauth_client.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/clients/spotify.py` & `wg_utilities-3.4.1/wg_utilities/clients/spotify.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/clients/truelayer.py` & `wg_utilities-3.4.1/wg_utilities/clients/truelayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -544,34 +544,41 @@
         creds_cache_path: Path | None = None,
         scopes: list[str] | None = None,
         oauth_login_redirect_host: str = "localhost",
         oauth_redirect_uri_override: str | None = None,
         headless_auth_link_callback: Callable[[str], None] | None = None,
         bank: Bank,
     ):
+        if not creds_cache_path:
+            if self.DEFAULT_CACHE_DIR:
+                creds_cache_path = Path(self.DEFAULT_CACHE_DIR).joinpath(
+                    type(self).__name__, client_id, f"{bank.name.lower()}.json"
+                )
+            else:
+                creds_cache_path = user_data_dir(
+                    file_name=sep.join(
+                        [
+                            "oauth_credentials",
+                            type(self).__name__,
+                            client_id,
+                            f"{bank.name.lower()}.json",
+                        ]
+                    )
+                )
+
         super().__init__(
             base_url=self.BASE_URL,
             access_token_endpoint=self.ACCESS_TOKEN_ENDPOINT,
             auth_link_base=self.AUTH_LINK_BASE,
             client_id=client_id,
             client_secret=client_secret,
             log_requests=log_requests,
             # TrueLayer shares the same Client ID for all banks, so override the
             # default to separate by bank
-            creds_cache_path=creds_cache_path
-            or user_data_dir(
-                file_name=sep.join(
-                    [
-                        "oauth_credentials",
-                        type(self).__name__,
-                        client_id,
-                        f"{bank.name.lower()}.json",
-                    ]
-                )
-            ),
+            creds_cache_path=creds_cache_path,
             scopes=scopes or self.DEFAULT_SCOPES,
             oauth_login_redirect_host=oauth_login_redirect_host,
             oauth_redirect_uri_override=oauth_redirect_uri_override,
             headless_auth_link_callback=headless_auth_link_callback,
         )
 
         self.bank = bank
```

### Comparing `wg_utilities-3.4.0/wg_utilities/devices/dht22/dht22_lib.py` & `wg_utilities-3.4.1/wg_utilities/devices/dht22/dht22_lib.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/devices/epd/__init__.py` & `wg_utilities-3.4.1/wg_utilities/devices/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/devices/epd/epd7in5_v2.py` & `wg_utilities-3.4.1/wg_utilities/devices/epd/epd7in5_v2.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/devices/epd/epdconfig.py` & `wg_utilities-3.4.1/wg_utilities/devices/epd/epdconfig.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py` & `wg_utilities-3.4.1/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/exceptions/__init__.py` & `wg_utilities-3.4.1/wg_utilities/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/functions/__init__.py` & `wg_utilities-3.4.1/wg_utilities/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/functions/_functions.py` & `wg_utilities-3.4.1/wg_utilities/functions/_functions.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/functions/datetime_helpers.py` & `wg_utilities-3.4.1/wg_utilities/functions/datetime_helpers.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/functions/file_management.py` & `wg_utilities-3.4.1/wg_utilities/functions/file_management.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/functions/json.py` & `wg_utilities-3.4.1/wg_utilities/functions/json.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/functions/processes.py` & `wg_utilities-3.4.1/wg_utilities/functions/processes.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/functions/string_manipulation.py` & `wg_utilities-3.4.1/wg_utilities/functions/string_manipulation.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/functions/xml.py` & `wg_utilities-3.4.1/wg_utilities/functions/xml.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/loggers/__init__.py` & `wg_utilities-3.4.1/wg_utilities/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/wg_utilities/testing/_custom_mocks.py` & `wg_utilities-3.4.1/wg_utilities/testing/_custom_mocks.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.4.0/PKG-INFO` & `wg_utilities-3.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wg-utilities
-Version: 3.4.0
+Version: 3.4.1
 Summary: Loads of useful stuff for the things I do :)
 Home-page: https://github.com/worgarside/wg-utilities
 License: MIT
 Author: Will Garside
 Author-email: worgarside@gmail.com
 Maintainer: Will Garside
 Maintainer-email: worgarside@gmail.com
```

