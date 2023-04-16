# Comparing `tmp/buildarr_prowlarr-0.1.1.tar.gz` & `tmp/buildarr_prowlarr-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildarr_prowlarr-0.1.1.tar", max compression
+gzip compressed data, was "buildarr_prowlarr-0.2.0.tar", max compression
```

## Comparing `buildarr_prowlarr-0.1.1.tar` & `buildarr_prowlarr-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    35149 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/LICENSE
--rw-r--r--   0        0        0    11795 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/README.md
--rw-r--r--   0        0        0      975 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/__init__.py
--rw-r--r--   0        0        0     3830 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/api.py
--rw-r--r--   0        0        0     2548 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/cli.py
--rw-r--r--   0        0        0     5261 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/__init__.py
--rw-r--r--   0        0        0     3913 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/__init__.py
--rw-r--r--   0        0        0     1055 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/apps/__init__.py
--rw-r--r--   0        0        0    25596 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/apps/applications.py
--rw-r--r--   0        0        0     8237 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/apps/sync_profiles.py
--rw-r--r--   0        0        0    10178 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/download_clients/__init__.py
--rw-r--r--   0        0        0     8611 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/download_clients/base.py
--rw-r--r--   0        0        0    32335 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/download_clients/torrent.py
--rw-r--r--   0        0        0    14416 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/download_clients/usenet.py
--rw-r--r--   0        0        0    20465 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/general.py
--rw-r--r--   0        0        0     2117 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/indexers/__init__.py
--rw-r--r--   0        0        0    30713 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/indexers/indexers.py
--rw-r--r--   0        0        0    15858 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/indexers/proxies.py
--rw-r--r--   0        0        0    42999 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/notifications.py
--rw-r--r--   0        0        0     3384 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/tags.py
--rw-r--r--   0        0        0     7231 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/ui.py
--rw-r--r--   0        0        0     1034 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/types.py
--rw-r--r--   0        0        0     1396 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/exceptions.py
--rw-r--r--   0        0        0      950 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/manager.py
--rw-r--r--   0        0        0     1189 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/plugin.py
--rw-r--r--   0        0        0        0 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/py.typed
--rw-r--r--   0        0        0     3841 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/secrets.py
--rw-r--r--   0        0        0     1162 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/types.py
--rw-r--r--   0        0        0     1465 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/util.py
--rw-r--r--   0        0        0     2332 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    13157 1970-01-01 00:00:00.000000 buildarr_prowlarr-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-16 05:15:50.971702 buildarr_prowlarr-0.2.0/LICENSE
+-rw-r--r--   0        0        0    11795 2023-04-16 05:15:50.971702 buildarr_prowlarr-0.2.0/README.md
+-rw-r--r--   0        0        0      975 2023-04-16 05:15:50.971702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/__init__.py
+-rw-r--r--   0        0        0     3820 2023-04-16 05:15:50.971702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/api.py
+-rw-r--r--   0        0        0     2548 2023-04-16 05:15:50.971702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/cli.py
+-rw-r--r--   0        0        0     5261 2023-04-16 05:15:50.971702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/__init__.py
+-rw-r--r--   0        0        0     4912 2023-04-16 05:15:50.971702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/__init__.py
+-rw-r--r--   0        0        0     1055 2023-04-16 05:15:50.971702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/apps/__init__.py
+-rw-r--r--   0        0        0    25970 2023-04-16 05:15:50.971702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/apps/applications.py
+-rw-r--r--   0        0        0     8821 2023-04-16 05:15:50.971702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/apps/sync_profiles.py
+-rw-r--r--   0        0        0    10900 2023-04-16 05:15:50.971702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/download_clients/__init__.py
+-rw-r--r--   0        0        0     8509 2023-04-16 05:15:50.975702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/download_clients/base.py
+-rw-r--r--   0        0        0    32333 2023-04-16 05:15:50.975702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/download_clients/torrent.py
+-rw-r--r--   0        0        0    14416 2023-04-16 05:15:50.975702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/download_clients/usenet.py
+-rw-r--r--   0        0        0    20465 2023-04-16 05:15:50.975702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/general.py
+-rw-r--r--   0        0        0     2318 2023-04-16 05:15:50.975702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/indexers/__init__.py
+-rw-r--r--   0        0        0    31215 2023-04-16 05:15:50.975702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/indexers/indexers.py
+-rw-r--r--   0        0        0    16437 2023-04-16 05:15:50.975702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/indexers/proxies.py
+-rw-r--r--   0        0        0    43584 2023-04-16 05:15:50.975702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/notifications.py
+-rw-r--r--   0        0        0     2928 2023-04-16 05:15:50.975702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/tags.py
+-rw-r--r--   0        0        0     7231 2023-04-16 05:15:50.975702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/ui.py
+-rw-r--r--   0        0        0     1034 2023-04-16 05:15:50.975702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/types.py
+-rw-r--r--   0        0        0     1396 2023-04-16 05:15:50.975702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/exceptions.py
+-rw-r--r--   0        0        0      950 2023-04-16 05:15:50.975702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/manager.py
+-rw-r--r--   0        0        0     1189 2023-04-16 05:15:50.975702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/plugin.py
+-rw-r--r--   0        0        0        0 2023-04-16 05:15:50.975702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/py.typed
+-rw-r--r--   0        0        0     3841 2023-04-16 05:15:50.975702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/secrets.py
+-rw-r--r--   0        0        0     1162 2023-04-16 05:15:50.975702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/types.py
+-rw-r--r--   0        0        0     1465 2023-04-16 05:15:50.975702 buildarr_prowlarr-0.2.0/buildarr_prowlarr/util.py
+-rw-r--r--   0        0        0     2332 2023-04-16 05:15:50.975702 buildarr_prowlarr-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    13157 1970-01-01 00:00:00.000000 buildarr_prowlarr-0.2.0/PKG-INFO
```

### Comparing `buildarr_prowlarr-0.1.1/LICENSE` & `buildarr_prowlarr-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.1/README.md` & `buildarr_prowlarr-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.1/buildarr_prowlarr/__init__.py` & `buildarr_prowlarr-0.2.0/buildarr_prowlarr/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.1/buildarr_prowlarr/api.py` & `buildarr_prowlarr-0.2.0/buildarr_prowlarr/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,32 +86,38 @@
         api_key (str): Prowlarr instance API key, if required. Defaults to `None`.
 
     Returns:
         Session initialisation metadata
     """
 
     url = f"{host_url}/initialize.js"
+
     logger.debug("GET %s", url)
+
     res = requests.get(
         url,
         headers={"X-Api-Key": api_key} if api_key else None,
-        timeout=state.config.buildarr.request_timeout,
+        timeout=state.request_timeout,
         allow_redirects=False,
     )
+
     if res.status_code != HTTPStatus.OK:
         logger.debug("GET %s -> status_code=%i res=%s", url, res.status_code, res.text)
         if res.status_code in (HTTPStatus.UNAUTHORIZED, HTTPStatus.FOUND):
             status_code: int = HTTPStatus.UNAUTHORIZED
             error_message = "Unauthorized"
         else:
             status_code = res.status_code
             error_message = f"Unexpected response with error code {res.status_code}: {res.text}"
         raise ProwlarrAPIError(
             f"Unable to retrieve 'initialize.js': {error_message}",
             status_code=status_code,
         )
+
     res_match = re.match(INITIALIZE_JS_RES_PATTERN, res.text)
     if not res_match:
         raise RuntimeError(f"No matches for 'initialize.js' parsing: {res.text}")
     res_json = json5.loads(res_match.group(1))
+
     logger.debug("GET %s -> status_code=%i res=%s", url, res.status_code, repr(res_json))
+
     return res_json
```

### Comparing `buildarr_prowlarr-0.1.1/buildarr_prowlarr/cli.py` & `buildarr_prowlarr-0.2.0/buildarr_prowlarr/cli.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/__init__.py` & `buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/apps/__init__.py` & `buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/apps/applications.py` & `buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/apps/applications.py`

 * *Files 5% similar despite different names*

```diff
@@ -236,24 +236,18 @@
                 prowlarr.ApplicationApi(api_client).update_applications(
                     id=str(api_application.id),
                     application_resource=prowlarr.ApplicationResource.from_dict(remote_attrs),
                 )
             return True
         return False
 
-    def _delete_remote(self, tree: str, secrets: ProwlarrSecrets, application_id: int) -> None:
-        logger.info("%s: (...) -> (deleted)", tree)
+    def _delete_remote(self, secrets: ProwlarrSecrets, application_id: int) -> None:
         with prowlarr_api_client(secrets=secrets) as api_client:
             prowlarr.ApplicationApi(api_client).delete_applications(id=application_id)
 
-    class Config(ProwlarrConfigBase.Config):
-        # Ensure in-place assignments of attributes are always validated,
-        # since this class performs such modifications in certain cases.
-        validate_assignment = True
-
 
 class LazylibrarianApplication(Application):
     """
     Add a [LazyLibrarian](https://lazylibrarian.gitlab.io) instance to sync with Prowlarr.
     """
 
     type: Literal["lazylibrarian", "lazylibrary"] = "lazylibrarian"
@@ -722,26 +716,38 @@
                 remote=remote.definitions[application_name],  # type: ignore[arg-type]
                 api_application_schemas=api_application_schemas,
                 category_ids=category_ids,
                 tag_ids=tag_ids,
                 api_application=api_applications[application_name],
             ):
                 changed = True
+        # Return whether or not the remote instance was changed.
+        return changed
+
+    def delete_remote(self, tree: str, secrets: ProwlarrSecrets, remote: Self) -> bool:
+        # Track whether or not any changes have been made on the remote instance.
+        changed = False
+        # Pull API objects and metadata required during the update operation.
+        with prowlarr_api_client(secrets=secrets) as api_client:
+            application_ids: Dict[str, int] = {
+                api_application.name: api_application.id
+                for api_application in prowlarr.ApplicationApi(api_client).list_applications()
+            }
         # Traverse the remote definitions, and see if there are any remote definitions
         # that do not exist in the local configuration.
         # If `delete_unmanaged` is enabled, delete it from the remote.
         # If `delete_unmanaged` is disabled, just add a log entry acknowledging
         # the existence of the unmanaged definition.
         for application_name, application in remote.definitions.items():
             if application_name not in self.definitions:
                 application_tree = f"{tree}.definitions[{repr(application_name)}]"
                 if self.delete_unmanaged:
+                    logger.info("%s: (...) -> (deleted)", application_tree)
                     application._delete_remote(
-                        tree=application_tree,
                         secrets=secrets,
-                        application_id=api_applications[application_name].id,
+                        application_id=application_ids[application_name],
                     )
                     changed = True
                 else:
                     logger.debug("%s: (...) (unmanaged)", application_tree)
         # Return whether or not the remote instance was changed.
         return changed
```

### Comparing `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/apps/sync_profiles.py` & `buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/apps/sync_profiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,16 +105,15 @@
                 prowlarr.AppProfileApi(api_client).update_app_profile(
                     id=str(api_profile.id),
                     app_profile_resource=prowlarr.AppProfileResource.from_dict(remote_attrs),
                 )
             return True
         return False
 
-    def _delete_remote(self, tree: str, secrets: ProwlarrSecrets, profile_id: int) -> None:
-        logger.info("%s: (...) -> (deleted)", tree)
+    def _delete_remote(self, secrets: ProwlarrSecrets, profile_id: int) -> None:
         with prowlarr_api_client(secrets=secrets) as api_client:
             prowlarr.AppProfileApi(api_client).delete_app_profile(id=profile_id)
 
 
 class SyncProfilesSettings(ProwlarrConfigBase):
     """
     App sync profiles are used to set application syncing configuration
@@ -203,26 +202,38 @@
             elif profile._update_remote(
                 tree=profile_tree,
                 secrets=secrets,
                 remote=remote.definitions[profile_name],  # type: ignore[arg-type]
                 api_profile=api_profiles[profile_name],
             ):
                 changed = True
+        # Return whether or not the remote instance was changed.
+        return changed
+
+    def delete_remote(self, tree: str, secrets: ProwlarrSecrets, remote: Self) -> bool:
+        # Track whether or not any changes have been made on the remote instance.
+        changed = False
+        # Pull API objects and metadata required during the update operation.
+        with prowlarr_api_client(secrets=secrets) as api_client:
+            profile_ids: Dict[str, int] = {
+                api_profile.name: api_profile.id
+                for api_profile in prowlarr.AppProfileApi(api_client).list_app_profile()
+            }
         # Traverse the remote definitions, and see if there are any remote definitions
         # that do not exist in the local configuration.
         # If `delete_unmanaged` is enabled, delete it from the remote.
         # If `delete_unmanaged` is disabled, just add a log entry acknowledging
         # the existence of the unmanaged definition.
         for profile_name, profile in remote.definitions.items():
             if profile_name not in self.definitions:
                 profile_tree = f"{tree}.definitions[{repr(profile_name)}]"
                 if self.delete_unmanaged:
+                    logger.info("%s: (...) -> (deleted)", profile_tree)
                     profile._delete_remote(
-                        tree=profile_tree,
                         secrets=secrets,
-                        profile_id=api_profiles[profile_name].id,
+                        profile_id=profile_ids[profile_name],
                     )
                     changed = True
                 else:
                     logger.debug("%s: (...) (unmanaged)", profile_tree)
         # Return whether or not the remote instance was changed.
         return changed
```

### Comparing `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/download_clients/__init__.py` & `buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/download_clients/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -248,26 +248,40 @@
                 remote=remote.definitions[downloadclient_name],  # type: ignore[arg-type]
                 api_downloadclient_schemas=api_downloadclient_schemas,
                 category_ids=category_ids,
                 tag_ids=tag_ids,
                 api_downloadclient=api_downloadclients[downloadclient_name],
             ):
                 changed = True
+        # Return whether or not the remote instance was changed.
+        return changed
+
+    def delete_remote(self, tree: str, secrets: ProwlarrSecrets, remote: Self) -> bool:
+        # Track whether or not any changes have been made on the remote instance.
+        changed = False
+        # Pull API objects and metadata required during the update operation.
+        with prowlarr_api_client(secrets=secrets) as api_client:
+            downloadclient_ids: Dict[str, int] = {
+                api_downloadclient.name: api_downloadclient.id
+                for api_downloadclient in prowlarr.DownloadClientApi(
+                    api_client,
+                ).list_download_client()
+            }
         # Traverse the remote definitions, and see if there are any remote definitions
         # that do not exist in the local configuration.
         # If `delete_unmanaged` is enabled, delete it from the remote.
         # If `delete_unmanaged` is disabled, just add a log entry acknowledging
         # the existence of the unmanaged definition.
         for downloadclient_name, downloadclient in remote.definitions.items():
             if downloadclient_name not in self.definitions:
                 downloadclient_tree = f"{tree}.definitions[{repr(downloadclient_name)}]"
                 if self.delete_unmanaged:
+                    logger.info("%s: (...) -> (deleted)", downloadclient_tree)
                     downloadclient._delete_remote(
-                        tree=downloadclient_tree,
                         secrets=secrets,
-                        downloadclient_id=api_downloadclients[downloadclient_name].id,
+                        downloadclient_id=downloadclient_ids[downloadclient_name],
                     )
                     changed = True
                 else:
                     logger.debug("%s: (...) (unmanaged)", downloadclient_tree)
         # Return whether or not the remote instance was changed.
         return changed
```

### Comparing `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/download_clients/base.py` & `buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/download_clients/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -230,16 +230,10 @@
                     download_client_resource=prowlarr.DownloadClientResource.from_dict(
                         remote_attrs,
                     ),
                 )
             return True
         return False
 
-    def _delete_remote(
-        self,
-        tree: str,
-        secrets: ProwlarrSecrets,
-        downloadclient_id: int,
-    ) -> None:
-        logger.info("%s: (...) -> (deleted)", tree)
+    def _delete_remote(self, secrets: ProwlarrSecrets, downloadclient_id: int) -> None:
         with prowlarr_api_client(secrets=secrets) as api_client:
             prowlarr.DownloadClientApi(api_client).delete_download_client(id=downloadclient_id)
```

### Comparing `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/download_clients/torrent.py` & `buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/download_clients/torrent.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from __future__ import annotations
 
 from logging import getLogger
 from typing import Any, Dict, List, Literal, Mapping, Optional, Set
 
 from buildarr.config import RemoteMapEntry
-from buildarr.types import BaseEnum, BaseIntEnum, NonEmptyStr, Password, Port
+from buildarr.types import BaseEnum, NonEmptyStr, Password, Port
 from pydantic import validator
 
 from ....types import LowerCaseNonEmptyStr
 from .base import DownloadClient
 
 logger = getLogger(__name__)
 
@@ -68,15 +68,15 @@
     language = 2
     release_group = 3
     year = 4
     indexer = 5
     network = 6
 
 
-class FreeboxPriority(BaseIntEnum):
+class FreeboxPriority(BaseEnum):
     last = 0
     first = 1
 
 
 class QbittorrentPriority(BaseEnum):
     """
     qBittorrent queue priority.
@@ -561,15 +561,15 @@
     """
     Default category to classify downloads under if no category mappings apply to it.
 
     This will create a `[category]` subdirectory in the output directory.
     Adding a category specific to Prowlarr avoids conflicts with unrelated non-Prowlarr downloads.
     """
 
-    priority: FreeboxPriority = FreeboxPriority.last
+    client_priority: FreeboxPriority = FreeboxPriority.last
     """
     Priority to use when adding a download to the client.
     """
 
     add_paused: bool = False
     """
     Add media to the download client in the Paused state.
@@ -603,15 +603,15 @@
                 {"is_field": True, "decoder": lambda v: v or None, "encoder": lambda v: v or ""},
             ),
             (
                 "category",
                 "category",
                 {"is_field": True, "decoder": lambda v: v or None, "encoder": lambda v: v or ""},
             ),
-            ("priority", "priority", {"is_field": True}),
+            ("client_priority", "priority", {"is_field": True}),
             ("add_paused", "addPaused", {"is_field": True}),
             (
                 "category_mappings",
                 "categories",
                 {
                     "decoder": lambda v: cls._category_mappings_decoder(category_ids, v),
                     "encoder": lambda v: cls._category_mappings_encoder(category_ids, v),
```

### Comparing `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/download_clients/usenet.py` & `buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/download_clients/usenet.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/general.py` & `buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/general.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/indexers/__init__.py` & `buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/indexers/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,27 +39,32 @@
         self,
         tree: str,
         secrets: ProwlarrSecrets,
         remote: Self,
         check_unmanaged: bool = False,
     ) -> bool:
         # Overload base function to guarantee execution order of section updates.
-        # 1. Tags must be created before everything else, and destroyed after they
-        #    are no longer referenced elsewhere.
         return any(
             [
                 self.proxies.update_remote(
                     f"{tree}.proxies",
                     secrets,
                     remote.proxies,
                     check_unmanaged=check_unmanaged,
                 ),
                 self.indexers.update_remote(
                     f"{tree}.indexers",
                     secrets,
                     remote.indexers,
                     check_unmanaged=check_unmanaged,
                 ),
-                # TODO: destroy indexers
-                # TODO: destroy tags
+            ],
+        )
+
+    def delete_remote(self, tree: str, secrets: ProwlarrSecrets, remote: Self) -> bool:
+        # Overload base function to guarantee execution order of section deletions.
+        return any(
+            [
+                self.indexers.delete_remote(f"{tree}.indexers", secrets, remote.indexers),
+                self.proxies.delete_remote(f"{tree}.proxies", secrets, remote.proxies),
             ],
         )
```

### Comparing `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/indexers/indexers.py` & `buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/indexers/indexers.py`

 * *Files 3% similar despite different names*

```diff
@@ -581,16 +581,15 @@
                             "fields": fields,
                         },
                     ),
                 )
             return True
         return False
 
-    def _delete_remote(self, tree: str, secrets: ProwlarrSecrets, indexer_id: int) -> None:
-        logger.info("%s: (...) -> (deleted)", tree)
+    def _delete_remote(self, secrets: ProwlarrSecrets, indexer_id: int) -> None:
         with prowlarr_api_client(secrets=secrets) as api_client:
             prowlarr.IndexerApi(api_client).delete_indexer(id=indexer_id)
 
 
 class IndexersSettings(ProwlarrConfigBase):
     """
     Indexers are used to monitor for new releases of media on external trackers.
@@ -666,16 +665,16 @@
     ) -> bool:
         # Track whether or not any changes have been made on the remote instance.
         changed = False
         # Pull API objects and metadata required during the update operation.
         with prowlarr_api_client(secrets=secrets) as api_client:
             indexer_api = prowlarr.IndexerApi(api_client)
             api_indexer_schemas = indexer_api.list_indexer_schema()
-            indexer_api_objs: Dict[str, prowlarr.IndexerResource] = {
-                indexer.name: indexer for indexer in indexer_api.list_indexer()
+            api_indexers: Dict[str, prowlarr.IndexerResource] = {
+                api_indexer.name: api_indexer for api_indexer in indexer_api.list_indexer()
             }
             sync_profile_ids: Dict[str, int] = {
                 profile.name: profile.id
                 for profile in prowlarr.AppProfileApi(api_client).list_app_profile()
             }
             tag_ids: Dict[str, int] = (
                 {tag.label: tag.id for tag in prowlarr.TagApi(api_client).list_tag()}
@@ -702,31 +701,40 @@
             elif indexer._update_remote(
                 tree=indexer_tree,
                 secrets=secrets,
                 remote=remote.definitions[indexer_name],  # type: ignore[arg-type]
                 api_indexer_schemas=api_indexer_schemas,
                 sync_profile_ids=sync_profile_ids,
                 tag_ids=tag_ids,
-                indexer_id=indexer_api_objs[indexer_name].id,
+                indexer_id=api_indexers[indexer_name].id,
                 indexer_name=indexer_name,
-                indexer_added=indexer_api_objs[indexer_name].added,
+                indexer_added=api_indexers[indexer_name].added,
             ):
                 changed = True
+        # Return whether or not the remote instance was changed.
+        return changed
+
+    def delete_remote(self, tree: str, secrets: ProwlarrSecrets, remote: Self) -> bool:
+        # Track whether or not any changes have been made on the remote instance.
+        changed = False
+        # Pull API objects and metadata required during the update operation.
+        with prowlarr_api_client(secrets=secrets) as api_client:
+            indexer_ids: Dict[str, int] = {
+                api_indexer.name: api_indexer.id
+                for api_indexer in prowlarr.IndexerApi(api_client).list_indexer()
+            }
         # Traverse the remote definitions, and see if there are any remote definitions
         # that do not exist in the local configuration.
         # If `delete_unmanaged` is enabled, delete it from the remote.
         # If `delete_unmanaged` is disabled, just add a log entry acknowledging
         # the existence of the unmanaged definition.
         for indexer_name, indexer in remote.definitions.items():
             if indexer_name not in self.definitions:
                 indexer_tree = f"{tree}.definitions[{repr(indexer_name)}]"
                 if self.delete_unmanaged:
-                    indexer._delete_remote(
-                        tree=indexer_tree,
-                        secrets=secrets,
-                        indexer_id=indexer_api_objs[indexer_name].id,
-                    )
+                    logger.info("%s: (...) -> (deleted)", indexer_tree)
+                    indexer._delete_remote(secrets=secrets, indexer_id=indexer_ids[indexer_name])
                     changed = True
                 else:
                     logger.debug("%s: (...) (unmanaged)", indexer_tree)
         # Return whether or not the remote instance was changed.
         return changed
```

### Comparing `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/indexers/proxies.py` & `buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/indexers/proxies.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,16 +165,15 @@
                 prowlarr.IndexerProxyApi(api_client).update_indexer_proxy(
                     id=str(api_proxy.id),
                     indexer_proxy_resource=prowlarr.IndexerProxyResource.from_dict(remote_attrs),
                 )
             return True
         return False
 
-    def _delete_remote(self, tree: str, secrets: ProwlarrSecrets, proxy_id: int) -> None:
-        logger.info("%s: (...) -> (deleted)", tree)
+    def _delete_remote(self, secrets: ProwlarrSecrets, proxy_id: int) -> None:
         with prowlarr_api_client(secrets=secrets) as api_client:
             prowlarr.IndexerProxyApi(api_client).delete_indexer_proxy(id=proxy_id)
 
 
 class FlaresolverrProxy(Proxy):
     """
     Bypass CloudFlare and DDoS-GUARD protection using FlareSolverr.
@@ -476,26 +475,38 @@
                 secrets=secrets,
                 remote=remote.definitions[proxy_name],  # type: ignore[arg-type]
                 api_proxy_schemas=api_proxy_schemas,
                 tag_ids=tag_ids,
                 api_proxy=api_proxies[proxy_name],
             ):
                 changed = True
+        # Return whether or not the remote instance was changed.
+        return changed
+
+    def delete_remote(self, tree: str, secrets: ProwlarrSecrets, remote: Self) -> bool:
+        # Track whether or not any changes have been made on the remote instance.
+        changed = False
+        # Pull API objects and metadata required during the update operation.
+        with prowlarr_api_client(secrets=secrets) as api_client:
+            proxy_ids: Dict[str, int] = {
+                api_proxy.name: api_proxy.id
+                for api_proxy in prowlarr.IndexerProxyApi(api_client).list_indexer_proxy()
+            }
         # Traverse the remote definitions, and see if there are any remote definitions
         # that do not exist in the local configuration.
         # If `delete_unmanaged` is enabled, delete it from the remote.
         # If `delete_unmanaged` is disabled, just add a log entry acknowledging
         # the existence of the unmanaged definition.
         for proxy_name, proxy in remote.definitions.items():
             if proxy_name not in self.definitions:
                 proxy_tree = f"{tree}.definitions[{repr(proxy_name)}]"
                 if self.delete_unmanaged:
+                    logger.info("%s: (...) -> (deleted)", proxy_tree)
                     proxy._delete_remote(
-                        tree=proxy_tree,
                         secrets=secrets,
-                        proxy_id=api_proxies[proxy_name].id,
+                        proxy_id=proxy_ids[proxy_name],
                     )
                     changed = True
                 else:
                     logger.debug("%s: (...) (unmanaged)", proxy_tree)
         # Return whether or not the remote instance was changed.
         return changed
```

### Comparing `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/notifications.py` & `buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/notifications.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 
 from logging import getLogger
 from typing import Any, Dict, List, Literal, Mapping, Optional, Set, Tuple, Type, Union
 
 import prowlarr
 
 from buildarr.config import RemoteMapEntry
-from buildarr.types import BaseEnum, BaseIntEnum, NonEmptyStr, Password, Port
+from buildarr.types import BaseEnum, NonEmptyStr, Password, Port
 from pydantic import AnyHttpUrl, ConstrainedInt, Field, NameEmail, SecretStr
 from typing_extensions import Annotated, Self
 
 from ...api import prowlarr_api_client
 from ...secrets import ProwlarrSecrets
 from ..types import ProwlarrConfigBase
 
 logger = getLogger(__name__)
 
 
-class OnGrabField(BaseIntEnum):
+class OnGrabField(BaseEnum):
     """
     Values for `on_grab_fields` for the Discord connection.
     """
 
     overview = 0
     rating = 1
     genres = 2
@@ -49,15 +49,15 @@
     size = 5
     links = 6
     release = 7
     poster = 8
     fanart = 9
 
 
-class OnImportField(BaseIntEnum):
+class OnImportField(BaseEnum):
     """
     Values for `on_import_fields` for the Discord connection.
     """
 
     overview = 0
     rating = 1
     genres = 2
@@ -92,15 +92,15 @@
     silent = -2
     quiet = -1
     normal = 0
     high = 1
     emergency = 2
 
 
-class NtfyshPriority(BaseIntEnum):
+class NtfyshPriority(BaseEnum):
     min = 1
     low = 2
     default = 3
     high = 4
     max = 5
 
 
@@ -359,16 +359,15 @@
                 prowlarr.NotificationApi(api_client).update_notification(
                     id=str(api_notification.id),
                     notification_resource=prowlarr.NotificationResource.from_dict(remote_attrs),
                 )
             return True
         return False
 
-    def _delete_remote(self, tree: str, secrets: ProwlarrSecrets, notification_id: int) -> None:
-        logger.info("%s: (...) -> (deleted)", tree)
+    def _delete_remote(self, secrets: ProwlarrSecrets, notification_id: int) -> None:
         with prowlarr_api_client(secrets=secrets) as api_client:
             prowlarr.NotificationApi(api_client).delete_notification(id=notification_id)
 
 
 class AppriseNotification(Notification):
     """
     Receive media update and health alert push notifications via an Apprise server.
@@ -1512,26 +1511,38 @@
                 secrets=secrets,
                 remote=remote.definitions[notification_name],  # type: ignore[arg-type]
                 api_notification_schemas=api_notification_schemas,
                 tag_ids=tag_ids,
                 api_notification=api_notifications[notification_name],
             ):
                 changed = True
+        # Return whether or not the remote instance was changed.
+        return changed
+
+    def delete_remote(self, tree: str, secrets: ProwlarrSecrets, remote: Self) -> bool:
+        # Track whether or not any changes have been made on the remote instance.
+        changed = False
+        # Pull API objects and metadata required during the update operation.
+        with prowlarr_api_client(secrets=secrets) as api_client:
+            notification_ids: Dict[str, int] = {
+                api_notification.name: api_notification.id
+                for api_notification in prowlarr.NotificationApi(api_client).list_notification()
+            }
         # Traverse the remote definitions, and see if there are any remote definitions
         # that do not exist in the local configuration.
         # If `delete_unmanaged` is enabled, delete it from the remote.
         # If `delete_unmanaged` is disabled, just add a log entry acknowledging
         # the existence of the unmanaged definition.
         for notification_name, notification in remote.definitions.items():
             if notification_name not in self.definitions:
                 notification_tree = f"{tree}.definitions[{repr(notification_name)}]"
                 if self.delete_unmanaged:
+                    logger.info("%s: (...) -> (deleted)", notification_tree)
                     notification._delete_remote(
-                        tree=notification_tree,
                         secrets=secrets,
-                        notification_id=api_notifications[notification_name].id,
+                        notification_id=notification_ids[notification_name],
                     )
                     changed = True
                 else:
                     logger.debug("%s: (...) (unmanaged)", notification_tree)
         # Return whether or not the remote instance was changed.
         return changed
```

### Comparing `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/tags.py` & `buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/tags.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,25 +47,14 @@
             - "example2"
     ```
 
     To be able to use those tags in Buildarr, they need to be defined
     in this configuration section.
     """
 
-    delete_unused: bool = False
-    """
-    Delete tags that are not used by any resource in Buildarr.
-
-    Note that tags not being used in Buildarr are not necessarily
-    unused by Prowlarr, so be careful about when to use this option.
-
-    Prowlarr appears to periodically clean up unused tags,
-    so in most cases there is no need to enable this option.
-    """
-
     definitions: Set[NonEmptyStr] = set()
     """
     Define tags that are used within Buildarr here.
 
     If they are not defined here, you may get errors resulting from non-existent
     tags from either Buildarr or Prowlarr.
     """
@@ -79,17 +68,15 @@
     def update_remote(
         self,
         tree: str,
         secrets: ProwlarrSecrets,
         remote: Self,
         check_unmanaged: bool = False,
     ) -> bool:
-        # This only does creations and updates.
-        # Deletes (and empty tag list prints) are done AFTER all other modifications are made.
-        # TODO: Implement tag deletions.
+        # This only does creations and updates, as Prowlarr automatically cleans up unused tags.
         changed = False
         with prowlarr_api_client(secrets=secrets) as api_client:
             tag_api = prowlarr.TagApi(api_client)
             current_tags: Dict[str, int] = {tag.label: tag.id for tag in tag_api.list_tag()}
             if self.definitions:
                 for i, tag in enumerate(self.definitions):
                     if tag in current_tags:
```

### Comparing `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/ui.py` & `buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/settings/ui.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/types.py` & `buildarr_prowlarr-0.2.0/buildarr_prowlarr/config/types.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.1/buildarr_prowlarr/exceptions.py` & `buildarr_prowlarr-0.2.0/buildarr_prowlarr/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.1/buildarr_prowlarr/manager.py` & `buildarr_prowlarr-0.2.0/buildarr_prowlarr/manager.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.1/buildarr_prowlarr/plugin.py` & `buildarr_prowlarr-0.2.0/buildarr_prowlarr/plugin.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.1/buildarr_prowlarr/secrets.py` & `buildarr_prowlarr-0.2.0/buildarr_prowlarr/secrets.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.1/buildarr_prowlarr/types.py` & `buildarr_prowlarr-0.2.0/buildarr_prowlarr/types.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.1/buildarr_prowlarr/util.py` & `buildarr_prowlarr-0.2.0/buildarr_prowlarr/util.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.1/pyproject.toml` & `buildarr_prowlarr-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.3.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "buildarr-prowlarr"
-version = "0.1.1"
+version = "0.2.0"
 description = "Prowlarr indexer manager plugin for Buildarr"
 authors = ["Callum Dickinson <callum.dickinson.nz@gmail.com>"]
 license = "GPL-3.0-or-later"
 homepage = "https://buildarr.github.io/plugins/sonarr"
 repository = "https://github.com/buildarr/buildarr-sonarr"
 documentation = "https://buildarr.github.io/plugins/sonarr"
 keywords = [
@@ -39,16 +39,16 @@
 
 [tool.poetry.plugins."buildarr.plugins"]
 "prowlarr" = "buildarr_prowlarr.plugin:ProwlarrPlugin"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 prowlarr-py = ">=0.3.2,<0.4.0"
-buildarr = ">=0.4.0,<0.5.0"
-buildarr-sonarr = {version = ">=0.4.1", optional = true}
+buildarr = ">=0.5.0,<0.6.0"
+buildarr-sonarr = {version = ">=0.5.0", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 mypy = "1.2.0"
 types-requests = "2.28.11.17"
 mkdocs = "1.4.2"
 mkdocstrings = {extras = ["python"], version = "0.21.2"}
```

### Comparing `buildarr_prowlarr-0.1.1/PKG-INFO` & `buildarr_prowlarr-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildarr-prowlarr
-Version: 0.1.1
+Version: 0.2.0
 Summary: Prowlarr indexer manager plugin for Buildarr
 Home-page: https://buildarr.github.io/plugins/sonarr
 License: GPL-3.0-or-later
 Keywords: buildarr,prowlarr,lazylibrarian,lidarr,mylar,radarr,readarr,sonarr,whisparr
 Author: Callum Dickinson
 Author-email: callum.dickinson.nz@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -18,16 +18,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Systems Administration
 Classifier: Typing :: Typed
 Provides-Extra: sonarr
-Requires-Dist: buildarr (>=0.4.0,<0.5.0)
-Requires-Dist: buildarr-sonarr (>=0.4.1) ; extra == "sonarr"
+Requires-Dist: buildarr (>=0.5.0,<0.6.0)
+Requires-Dist: buildarr-sonarr (>=0.5.0) ; extra == "sonarr"
 Requires-Dist: prowlarr-py (>=0.3.2,<0.4.0)
 Project-URL: Documentation, https://buildarr.github.io/plugins/sonarr
 Project-URL: Repository, https://github.com/buildarr/buildarr-sonarr
 Description-Content-Type: text/markdown
 
 # Buildarr Prowlarr Plugin
```

