# Comparing `tmp/wg_utilities-3.3.0.tar.gz` & `tmp/wg_utilities-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wg_utilities-3.3.0.tar", max compression
+gzip compressed data, was "wg_utilities-3.4.0.tar", max compression
```

## Comparing `wg_utilities-3.3.0.tar` & `wg_utilities-3.4.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1069 2023-04-15 20:24:04.024161 wg_utilities-3.3.0/LICENSE
--rw-r--r--   0        0        0     2297 2023-04-15 20:24:04.024161 wg_utilities-3.3.0/README.md
--rw-r--r--   0        0        0     4825 2023-04-15 20:24:04.028161 wg_utilities-3.3.0/pyproject.toml
--rw-r--r--   0        0        0      280 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/__init__.py
--rw-r--r--   0        0        0      140 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/api/__init__.py
--rw-r--r--   0        0        0     7384 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/api/temp_auth_server.py
--rw-r--r--   0        0        0      560 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/clients/__init__.py
--rw-r--r--   0        0        0     4305 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/clients/_google.py
--rw-r--r--   0        0        0    10390 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/clients/_spotify_types.py
--rw-r--r--   0        0        0    24119 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/clients/google_calendar.py
--rw-r--r--   0        0        0    56745 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/clients/google_drive.py
--rw-r--r--   0        0        0     7441 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/clients/google_fit.py
--rw-r--r--   0        0        0    13531 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/clients/google_photos.py
--rw-r--r--   0        0        0    15632 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/clients/monzo.py
--rw-r--r--   0        0        0    26324 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/clients/oauth_client.py
--rw-r--r--   0        0        0    49179 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/clients/spotify.py
--rw-r--r--   0        0        0    21707 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/clients/truelayer.py
--rw-r--r--   0        0        0      126 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/devices/__init__.py
--rw-r--r--   0        0        0      119 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/devices/dht22/__init__.py
--rwxr-xr-x   0        0        0     6642 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/devices/dht22/dht22_lib.py
--rw-r--r--   0        0        0     1129 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/devices/epd/__init__.py
--rw-r--r--   0        0        0     7042 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/devices/epd/epd7in5_v2.py
--rw-r--r--   0        0        0     6041 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/devices/epd/epdconfig.py
--rw-r--r--   0        0        0      138 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/devices/yamaha_yas_209/__init__.py
--rw-r--r--   0        0        0    36374 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py
--rw-r--r--   0        0        0     5401 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/exceptions/__init__.py
--rw-r--r--   0        0        0      803 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/functions/__init__.py
--rw-r--r--   0        0        0     4595 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/functions/_functions.py
--rw-r--r--   0        0        0     1287 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/functions/datetime_helpers.py
--rw-r--r--   0        0        0     2024 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/functions/file_management.py
--rw-r--r--   0        0        0     8877 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/functions/json.py
--rw-r--r--   0        0        0     1386 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/functions/processes.py
--rw-r--r--   0        0        0     1106 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/functions/string_manipulation.py
--rw-r--r--   0        0        0     1586 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/functions/xml.py
--rw-r--r--   0        0        0     7258 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/loggers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/py.typed
--rw-r--r--   0        0        0      167 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/testing/__init__.py
--rw-r--r--   0        0        0     5257 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/testing/_custom_mocks.py
--rw-r--r--   0        0        0     4113 1970-01-01 00:00:00.000000 wg_utilities-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-16 12:36:50.156112 wg_utilities-3.4.0/LICENSE
+-rw-r--r--   0        0        0     2297 2023-04-16 12:36:50.156112 wg_utilities-3.4.0/README.md
+-rw-r--r--   0        0        0     4825 2023-04-16 12:36:50.160112 wg_utilities-3.4.0/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-04-16 12:36:50.236112 wg_utilities-3.4.0/wg_utilities/__init__.py
+-rw-r--r--   0        0        0      140 2023-04-16 12:36:50.236112 wg_utilities-3.4.0/wg_utilities/api/__init__.py
+-rw-r--r--   0        0        0     7384 2023-04-16 12:36:50.236112 wg_utilities-3.4.0/wg_utilities/api/temp_auth_server.py
+-rw-r--r--   0        0        0      685 2023-04-16 12:36:50.236112 wg_utilities-3.4.0/wg_utilities/clients/__init__.py
+-rw-r--r--   0        0        0     4305 2023-04-16 12:36:50.236112 wg_utilities-3.4.0/wg_utilities/clients/_google.py
+-rw-r--r--   0        0        0    10390 2023-04-16 12:36:50.236112 wg_utilities-3.4.0/wg_utilities/clients/_spotify_types.py
+-rw-r--r--   0        0        0    24119 2023-04-16 12:36:50.236112 wg_utilities-3.4.0/wg_utilities/clients/google_calendar.py
+-rw-r--r--   0        0        0    56540 2023-04-16 12:36:50.236112 wg_utilities-3.4.0/wg_utilities/clients/google_drive.py
+-rw-r--r--   0        0        0     7566 2023-04-16 12:36:50.236112 wg_utilities-3.4.0/wg_utilities/clients/google_fit.py
+-rw-r--r--   0        0        0    13531 2023-04-16 12:36:50.236112 wg_utilities-3.4.0/wg_utilities/clients/google_photos.py
+-rw-r--r--   0        0        0    15632 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/clients/monzo.py
+-rw-r--r--   0        0        0    26578 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/clients/oauth_client.py
+-rw-r--r--   0        0        0    49179 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/clients/spotify.py
+-rw-r--r--   0        0        0    21832 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/clients/truelayer.py
+-rw-r--r--   0        0        0      126 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/devices/__init__.py
+-rw-r--r--   0        0        0      119 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/devices/dht22/__init__.py
+-rwxr-xr-x   0        0        0     6642 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/devices/dht22/dht22_lib.py
+-rw-r--r--   0        0        0     1129 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/devices/epd/__init__.py
+-rw-r--r--   0        0        0     7042 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/devices/epd/epd7in5_v2.py
+-rw-r--r--   0        0        0     6041 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/devices/epd/epdconfig.py
+-rw-r--r--   0        0        0      138 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/devices/yamaha_yas_209/__init__.py
+-rw-r--r--   0        0        0    36374 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py
+-rw-r--r--   0        0        0     5401 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/exceptions/__init__.py
+-rw-r--r--   0        0        0      803 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/functions/__init__.py
+-rw-r--r--   0        0        0     4595 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/functions/_functions.py
+-rw-r--r--   0        0        0     1287 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/functions/datetime_helpers.py
+-rw-r--r--   0        0        0     2024 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/functions/file_management.py
+-rw-r--r--   0        0        0     8877 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/functions/json.py
+-rw-r--r--   0        0        0     1386 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/functions/processes.py
+-rw-r--r--   0        0        0     1106 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/functions/string_manipulation.py
+-rw-r--r--   0        0        0     1586 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/functions/xml.py
+-rw-r--r--   0        0        0     7258 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/loggers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/py.typed
+-rw-r--r--   0        0        0      167 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/testing/__init__.py
+-rw-r--r--   0        0        0     5257 2023-04-16 12:36:50.240112 wg_utilities-3.4.0/wg_utilities/testing/_custom_mocks.py
+-rw-r--r--   0        0        0     4113 1970-01-01 00:00:00.000000 wg_utilities-3.4.0/PKG-INFO
```

### Comparing `wg_utilities-3.3.0/LICENSE` & `wg_utilities-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.3.0/README.md` & `wg_utilities-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.3.0/pyproject.toml` & `wg_utilities-3.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wg-utilities"
-version = "3.3.0"
+version = "3.4.0"
 description = "Loads of useful stuff for the things I do :)"
 
 authors = ["Will Garside <worgarside@gmail.com>"]
 include = ["wg_utilities/py.typed"]
 license = "MIT"
 maintainers = ["Will Garside <worgarside@gmail.com>"]
 packages = [{ include = "wg_utilities" }]
```

### Comparing `wg_utilities-3.3.0/wg_utilities/api/temp_auth_server.py` & `wg_utilities-3.4.0/wg_utilities/api/temp_auth_server.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.3.0/wg_utilities/clients/_google.py` & `wg_utilities-3.4.0/wg_utilities/clients/_google.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.3.0/wg_utilities/clients/_spotify_types.py` & `wg_utilities-3.4.0/wg_utilities/clients/_spotify_types.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.3.0/wg_utilities/clients/google_calendar.py` & `wg_utilities-3.4.0/wg_utilities/clients/google_calendar.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.3.0/wg_utilities/clients/google_drive.py` & `wg_utilities-3.4.0/wg_utilities/clients/google_drive.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,15 +189,15 @@
                 parent.add_child(instance)
             elif host_drive is not None and host_drive.id == instance.parents[0]:
                 instance.parent_ = host_drive
                 host_drive.add_child(instance)
 
         if (
             not _block_describe_call
-            and google_client.item_metadata_retrieval == ItemMetadataRetrieval.ON_INIT
+            and google_client.item_metadata_retrieval == IMR.ON_INIT
             and hasattr(instance, "describe")
         ):
             instance.describe()
 
         return instance
 
     def dict(
@@ -452,16 +452,15 @@
                 for child in self.all_known_children:
                     if child.name == directory_name:
                         return child.navigate("/".join(rest))
 
                 try:
                     file_fields = (
                         "*"
-                        if self.google_client.item_metadata_retrieval
-                        == ItemMetadataRetrieval.ON_INIT
+                        if self.google_client.item_metadata_retrieval == IMR.ON_INIT
                         else "id, name, parents, mimeType, kind"
                     )
 
                     item = self.google_client.get_items(
                         "/files",
                         list_key="files",
                         params={
@@ -618,16 +617,15 @@
             list: the directories contained within this directory
         """
 
         if self._directories_loaded is not True:
             # TODO replace these with a `file_fields` property
             file_fields = (
                 "*"
-                if self.google_client.item_metadata_retrieval
-                == ItemMetadataRetrieval.ON_INIT
+                if self.google_client.item_metadata_retrieval == IMR.ON_INIT
                 else "id, name, parents, mimeType, kind"
             )
 
             # TODO: this needs to be changed to only get *new* folders - currently this
             #   will overwrite any known children, including all metadata ad further
             #   descendents
             self._set_private_attr(
@@ -665,16 +663,15 @@
 
         Returns:
             list: the list of files contained within this directory
         """
         if self._files_loaded is not True:
             file_fields = (
                 "*"
-                if self.google_client.item_metadata_retrieval
-                == ItemMetadataRetrieval.ON_INIT
+                if self.google_client.item_metadata_retrieval == IMR.ON_INIT
                 else "id, name, parents, mimeType, kind"
             )
 
             self._set_private_attr(
                 "_files",
                 [
                     File.from_json_response(
@@ -802,18 +799,15 @@
             or name not in self.__fields__
             or self.__fields__[name].field_info.exclude is True
         ):
             return super().__getattribute__(name)
 
         if name not in self.__fields_set__ or not super().__getattribute__(name):
             # If IMR is enabled, load all metadata
-            if (
-                self.google_client.item_metadata_retrieval
-                == ItemMetadataRetrieval.ON_FIRST_REQUEST
-            ):
+            if self.google_client.item_metadata_retrieval == IMR.ON_FIRST_REQUEST:
                 self.describe()
                 return super().__getattribute__(name)
 
             # Otherwise just get the single field
             google_key = self.__fields__[name].alias or name
 
             res = self.google_client.get_json_response(
@@ -1132,16 +1126,15 @@
 
         Args:
             cls (type): The class of the entity to get.
             entity_id (str): The ID of the entity to get.
         """
         file_fields = (
             "*"
-            if self.google_client.item_metadata_retrieval
-            == ItemMetadataRetrieval.ON_INIT
+            if self.google_client.item_metadata_retrieval == IMR.ON_INIT
             else "id, name, parents, mimeType, kind"
         )
 
         return cls.from_json_response(
             self.google_client.get_json_response(
                 f"/files/{entity_id}",
                 params={
@@ -1205,16 +1198,15 @@
         ):
             return
 
         # May as well get all fields in initial request if we're going to do it per
         # item anyway
         file_fields = (
             "*"
-            if self.google_client.item_metadata_retrieval
-            == ItemMetadataRetrieval.ON_INIT
+            if self.google_client.item_metadata_retrieval == IMR.ON_INIT
             else "id, name, parents, mimeType, kind"
         )
 
         params = {
             "pageSize": 1000,
             "fields": f"nextPageToken, files({file_fields})",
         }
@@ -1334,16 +1326,15 @@
 
         Raises:
             ValueError: if the given entity type is not supported
         """
 
         file_fields = (
             "*"
-            if self.google_client.item_metadata_retrieval
-            == ItemMetadataRetrieval.ON_INIT
+            if self.google_client.item_metadata_retrieval == IMR.ON_INIT
             else "id, name, parents, mimeType, kind"
         )
 
         params = {
             "pageSize": 1 if exact_match else min(max_results, 1000),
             "fields": f"nextPageToken, files({file_fields})",
         }
@@ -1442,14 +1433,17 @@
     """
 
     ON_DEMAND = "on_demand"
     ON_FIRST_REQUEST = "on_first_request"
     ON_INIT = "on_init"
 
 
+IMR = ItemMetadataRetrieval
+
+
 class GoogleDriveClient(GoogleClient[JSONObj]):
     """Custom client specifically for Google's Drive API.
 
     Args:
         scopes (list): a list of scopes the client can be given
         creds_cache_path (str): file path for where to cache credentials
     """
@@ -1471,27 +1465,28 @@
         *,
         client_id: str,
         client_secret: str,
         log_requests: bool = False,
         creds_cache_path: Path | None = None,
         scopes: list[str] | None = None,
         oauth_login_redirect_host: str = "localhost",
-        # pylint: disable=line-too-long
-        item_metadata_retrieval: ItemMetadataRetrieval = ItemMetadataRetrieval.ON_FIRST_REQUEST,
+        oauth_redirect_uri_override: str | None = None,
         headless_auth_link_callback: Callable[[str], None] | None = None,
+        item_metadata_retrieval: IMR = IMR.ON_FIRST_REQUEST,
     ):
         super().__init__(
             client_id=client_id,
             client_secret=client_secret,
             log_requests=log_requests,
             creds_cache_path=creds_cache_path,
             scopes=scopes or self.DEFAULT_SCOPES,
             oauth_login_redirect_host=oauth_login_redirect_host,
-            base_url=self.BASE_URL,
+            oauth_redirect_uri_override=oauth_redirect_uri_override,
             headless_auth_link_callback=headless_auth_link_callback,
+            base_url=self.BASE_URL,
         )
 
         self._my_drive: Drive
         self.item_metadata_retrieval = item_metadata_retrieval
 
     @property
     def my_drive(self) -> Drive:
```

### Comparing `wg_utilities-3.3.0/wg_utilities/clients/google_fit.py` & `wg_utilities-3.4.0/wg_utilities/clients/google_fit.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,25 +199,27 @@
         *,
         client_id: str,
         client_secret: str,
         log_requests: bool = False,
         creds_cache_path: Path | None = None,
         scopes: list[str] | None = None,
         oauth_login_redirect_host: str = "localhost",
+        oauth_redirect_uri_override: str | None = None,
         headless_auth_link_callback: Callable[[str], None] | None = None,
     ):
         super().__init__(
             client_id=client_id,
             client_secret=client_secret,
             log_requests=log_requests,
             creds_cache_path=creds_cache_path,
             scopes=scopes or self.DEFAULT_SCOPES,
             oauth_login_redirect_host=oauth_login_redirect_host,
-            base_url=self.BASE_URL,
+            oauth_redirect_uri_override=oauth_redirect_uri_override,
             headless_auth_link_callback=headless_auth_link_callback,
+            base_url=self.BASE_URL,
         )
 
         self.data_sources: dict[str, DataSource] = {}
 
     def get_data_source(self, data_source_id: str) -> DataSource:
         """Get a data source based on its UID.
```

### Comparing `wg_utilities-3.3.0/wg_utilities/clients/google_photos.py` & `wg_utilities-3.4.0/wg_utilities/clients/google_photos.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.3.0/wg_utilities/clients/monzo.py` & `wg_utilities-3.4.0/wg_utilities/clients/monzo.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.3.0/wg_utilities/clients/oauth_client.py` & `wg_utilities-3.4.0/wg_utilities/clients/oauth_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,27 +238,29 @@
         *,
         client_id: str | None = None,
         client_secret: str | None = None,
         log_requests: bool = False,
         creds_cache_path: Path | None = None,
         scopes: list[str] | None = None,
         oauth_login_redirect_host: str = "localhost",
+        oauth_redirect_uri_override: str | None = None,
+        headless_auth_link_callback: Callable[[str], None] | None = None,
         access_token_endpoint: str | None = None,
         auth_link_base: str | None = None,
         base_url: str | None = None,
-        headless_auth_link_callback: Callable[[str], None] | None = None,
     ):
         self._client_id = client_id
         self._client_secret = client_secret
         self.base_url = base_url or self.BASE_URL
         self.access_token_endpoint = access_token_endpoint or self.ACCESS_TOKEN_ENDPOINT
         self.auth_link_base = auth_link_base or self.AUTH_LINK_BASE
         self.log_requests = log_requests
         self._creds_cache_path = creds_cache_path
         self.oauth_login_redirect_host = oauth_login_redirect_host
+        self.oauth_redirect_uri_override = oauth_redirect_uri_override
         self.headless_auth_link_callback = headless_auth_link_callback
 
         self.scopes = scopes or self.DEFAULT_SCOPES
 
         self._credentials: OAuthCredentials
         self._temp_auth_server: TempAuthServer
 
@@ -577,16 +579,19 @@
         """
         LOGGER.info("Performing first time login")
 
         state_token = "".join(choice(ascii_letters) for _ in range(32))
 
         self.temp_auth_server.start_server()
 
-        # pylint: disable=line-too-long
-        redirect_uri = f"http://{self.oauth_login_redirect_host}:{self.temp_auth_server.port}/get_auth_code"
+        if self.oauth_redirect_uri_override:
+            redirect_uri = self.oauth_redirect_uri_override
+        else:
+            # pylint: disable=line-too-long
+            redirect_uri = f"http://{self.oauth_login_redirect_host}:{self.temp_auth_server.port}/get_auth_code"
 
         auth_link_params = {
             "client_id": self._client_id,
             "redirect_uri": redirect_uri,
             "response_type": "code",
             "state": state_token,
             "access_type": "offline",
```

### Comparing `wg_utilities-3.3.0/wg_utilities/clients/spotify.py` & `wg_utilities-3.4.0/wg_utilities/clients/spotify.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.3.0/wg_utilities/clients/truelayer.py` & `wg_utilities-3.4.0/wg_utilities/clients/truelayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -540,14 +540,15 @@
         *,
         client_id: str,
         client_secret: str,
         log_requests: bool = False,
         creds_cache_path: Path | None = None,
         scopes: list[str] | None = None,
         oauth_login_redirect_host: str = "localhost",
+        oauth_redirect_uri_override: str | None = None,
         headless_auth_link_callback: Callable[[str], None] | None = None,
         bank: Bank,
     ):
         super().__init__(
             base_url=self.BASE_URL,
             access_token_endpoint=self.ACCESS_TOKEN_ENDPOINT,
             auth_link_base=self.AUTH_LINK_BASE,
@@ -565,14 +566,15 @@
                         client_id,
                         f"{bank.name.lower()}.json",
                     ]
                 )
             ),
             scopes=scopes or self.DEFAULT_SCOPES,
             oauth_login_redirect_host=oauth_login_redirect_host,
+            oauth_redirect_uri_override=oauth_redirect_uri_override,
             headless_auth_link_callback=headless_auth_link_callback,
         )
 
         self.bank = bank
 
     def _get_entity_by_id(
         self,
```

### Comparing `wg_utilities-3.3.0/wg_utilities/devices/dht22/dht22_lib.py` & `wg_utilities-3.4.0/wg_utilities/devices/dht22/dht22_lib.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.3.0/wg_utilities/devices/epd/__init__.py` & `wg_utilities-3.4.0/wg_utilities/devices/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.3.0/wg_utilities/devices/epd/epd7in5_v2.py` & `wg_utilities-3.4.0/wg_utilities/devices/epd/epd7in5_v2.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.3.0/wg_utilities/devices/epd/epdconfig.py` & `wg_utilities-3.4.0/wg_utilities/devices/epd/epdconfig.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.3.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py` & `wg_utilities-3.4.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.3.0/wg_utilities/exceptions/__init__.py` & `wg_utilities-3.4.0/wg_utilities/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.3.0/wg_utilities/functions/__init__.py` & `wg_utilities-3.4.0/wg_utilities/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.3.0/wg_utilities/functions/_functions.py` & `wg_utilities-3.4.0/wg_utilities/functions/_functions.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.3.0/wg_utilities/functions/datetime_helpers.py` & `wg_utilities-3.4.0/wg_utilities/functions/datetime_helpers.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.3.0/wg_utilities/functions/file_management.py` & `wg_utilities-3.4.0/wg_utilities/functions/file_management.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.3.0/wg_utilities/functions/json.py` & `wg_utilities-3.4.0/wg_utilities/functions/json.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.3.0/wg_utilities/functions/processes.py` & `wg_utilities-3.4.0/wg_utilities/functions/processes.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.3.0/wg_utilities/functions/string_manipulation.py` & `wg_utilities-3.4.0/wg_utilities/functions/string_manipulation.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.3.0/wg_utilities/functions/xml.py` & `wg_utilities-3.4.0/wg_utilities/functions/xml.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.3.0/wg_utilities/loggers/__init__.py` & `wg_utilities-3.4.0/wg_utilities/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.3.0/wg_utilities/testing/_custom_mocks.py` & `wg_utilities-3.4.0/wg_utilities/testing/_custom_mocks.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.3.0/PKG-INFO` & `wg_utilities-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wg-utilities
-Version: 3.3.0
+Version: 3.4.0
 Summary: Loads of useful stuff for the things I do :)
 Home-page: https://github.com/worgarside/wg-utilities
 License: MIT
 Author: Will Garside
 Author-email: worgarside@gmail.com
 Maintainer: Will Garside
 Maintainer-email: worgarside@gmail.com
```

