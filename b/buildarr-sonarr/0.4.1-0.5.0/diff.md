# Comparing `tmp/buildarr_sonarr-0.4.1.tar.gz` & `tmp/buildarr_sonarr-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildarr_sonarr-0.4.1.tar", max compression
+gzip compressed data, was "buildarr_sonarr-0.5.0.tar", max compression
```

## Comparing `buildarr_sonarr-0.4.1.tar` & `buildarr_sonarr-0.5.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    35149 2023-04-08 09:23:52.591184 buildarr_sonarr-0.4.1/LICENSE
--rw-r--r--   0        0        0    19787 2023-04-08 09:23:52.591184 buildarr_sonarr-0.4.1/README.md
--rw-r--r--   0        0        0      971 2023-04-08 09:23:52.591184 buildarr_sonarr-0.4.1/buildarr_sonarr/__init__.py
--rw-r--r--   0        0        0     9767 2023-04-08 09:23:52.591184 buildarr_sonarr-0.4.1/buildarr_sonarr/api.py
--rw-r--r--   0        0        0     2536 2023-04-08 09:23:52.591184 buildarr_sonarr-0.4.1/buildarr_sonarr/cli.py
--rw-r--r--   0        0        0    12804 2023-04-08 09:23:52.591184 buildarr_sonarr-0.4.1/buildarr_sonarr/config/__init__.py
--rw-r--r--   0        0        0    49054 2023-04-08 09:23:52.591184 buildarr_sonarr-0.4.1/buildarr_sonarr/config/connect.py
--rw-r--r--   0        0        0     9322 2023-04-08 09:23:52.591184 buildarr_sonarr-0.4.1/buildarr_sonarr/config/download_clients/__init__.py
--rw-r--r--   0        0        0    48166 2023-04-08 09:23:52.591184 buildarr_sonarr-0.4.1/buildarr_sonarr/config/download_clients/download_clients.py
--rw-r--r--   0        0        0     8956 2023-04-08 09:23:52.591184 buildarr_sonarr-0.4.1/buildarr_sonarr/config/download_clients/remote_path_mappings.py
--rw-r--r--   0        0        0    18803 2023-04-08 09:23:52.591184 buildarr_sonarr-0.4.1/buildarr_sonarr/config/general.py
--rw-r--r--   0        0        0    48134 2023-04-08 09:23:52.591184 buildarr_sonarr-0.4.1/buildarr_sonarr/config/import_lists.py
--rw-r--r--   0        0        0    32600 2023-04-08 09:23:52.591184 buildarr_sonarr-0.4.1/buildarr_sonarr/config/indexers.py
--rw-r--r--   0        0        0    19051 2023-04-08 09:23:52.595185 buildarr_sonarr-0.4.1/buildarr_sonarr/config/media_management.py
--rw-r--r--   0        0        0    11024 2023-04-08 09:23:52.595185 buildarr_sonarr-0.4.1/buildarr_sonarr/config/metadata.py
--rw-r--r--   0        0        0     1527 2023-04-08 09:23:52.595185 buildarr_sonarr-0.4.1/buildarr_sonarr/config/profiles/__init__.py
--rw-r--r--   0        0        0    13160 2023-04-08 09:23:52.595185 buildarr_sonarr-0.4.1/buildarr_sonarr/config/profiles/delay.py
--rw-r--r--   0        0        0    12657 2023-04-08 09:23:52.595185 buildarr_sonarr-0.4.1/buildarr_sonarr/config/profiles/language.py
--rw-r--r--   0        0        0    16529 2023-04-08 09:23:52.595185 buildarr_sonarr-0.4.1/buildarr_sonarr/config/profiles/quality.py
--rw-r--r--   0        0        0    17741 2023-04-08 09:23:52.595185 buildarr_sonarr-0.4.1/buildarr_sonarr/config/profiles/release.py
--rw-r--r--   0        0        0     9026 2023-04-08 09:23:52.595185 buildarr_sonarr-0.4.1/buildarr_sonarr/config/quality.py
--rw-r--r--   0        0        0     3164 2023-04-08 09:23:52.595185 buildarr_sonarr-0.4.1/buildarr_sonarr/config/tags.py
--rw-r--r--   0        0        0     1229 2023-04-08 09:23:52.595185 buildarr_sonarr-0.4.1/buildarr_sonarr/config/types.py
--rw-r--r--   0        0        0     6150 2023-04-08 09:23:52.595185 buildarr_sonarr-0.4.1/buildarr_sonarr/config/ui.py
--rw-r--r--   0        0        0     1537 2023-04-08 09:23:52.595185 buildarr_sonarr-0.4.1/buildarr_sonarr/config/util.py
--rw-r--r--   0        0        0     1184 2023-04-08 09:23:52.595185 buildarr_sonarr-0.4.1/buildarr_sonarr/exceptions.py
--rw-r--r--   0        0        0      938 2023-04-08 09:23:52.595185 buildarr_sonarr-0.4.1/buildarr_sonarr/manager.py
--rw-r--r--   0        0        0     1165 2023-04-08 09:23:52.595185 buildarr_sonarr-0.4.1/buildarr_sonarr/plugin.py
--rw-r--r--   0        0        0        0 2023-04-08 09:23:52.595185 buildarr_sonarr-0.4.1/buildarr_sonarr/py.typed
--rw-r--r--   0        0        0     2673 2023-04-08 09:23:52.595185 buildarr_sonarr-0.4.1/buildarr_sonarr/secrets.py
--rw-r--r--   0        0        0      980 2023-04-08 09:23:52.595185 buildarr_sonarr-0.4.1/buildarr_sonarr/types.py
--rw-r--r--   0        0        0     1924 2023-04-08 09:23:52.595185 buildarr_sonarr-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    20944 1970-01-01 00:00:00.000000 buildarr_sonarr-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-16 04:55:27.923625 buildarr_sonarr-0.5.0/LICENSE
+-rw-r--r--   0        0        0    19787 2023-04-16 04:55:27.923625 buildarr_sonarr-0.5.0/README.md
+-rw-r--r--   0        0        0      971 2023-04-16 04:55:27.923625 buildarr_sonarr-0.5.0/buildarr_sonarr/__init__.py
+-rw-r--r--   0        0        0     9799 2023-04-16 04:55:27.923625 buildarr_sonarr-0.5.0/buildarr_sonarr/api.py
+-rw-r--r--   0        0        0     2536 2023-04-16 04:55:27.923625 buildarr_sonarr-0.5.0/buildarr_sonarr/cli.py
+-rw-r--r--   0        0        0    11938 2023-04-16 04:55:27.923625 buildarr_sonarr-0.5.0/buildarr_sonarr/config/__init__.py
+-rw-r--r--   0        0        0    49245 2023-04-16 04:55:27.923625 buildarr_sonarr-0.5.0/buildarr_sonarr/config/connect.py
+-rw-r--r--   0        0        0    10057 2023-04-16 04:55:27.923625 buildarr_sonarr-0.5.0/buildarr_sonarr/config/download_clients/__init__.py
+-rw-r--r--   0        0        0    48064 2023-04-16 04:55:27.923625 buildarr_sonarr-0.5.0/buildarr_sonarr/config/download_clients/download_clients.py
+-rw-r--r--   0        0        0     9009 2023-04-16 04:55:27.923625 buildarr_sonarr-0.5.0/buildarr_sonarr/config/download_clients/remote_path_mappings.py
+-rw-r--r--   0        0        0    18803 2023-04-16 04:55:27.923625 buildarr_sonarr-0.5.0/buildarr_sonarr/config/general.py
+-rw-r--r--   0        0        0    45264 2023-04-16 04:55:27.923625 buildarr_sonarr-0.5.0/buildarr_sonarr/config/import_lists.py
+-rw-r--r--   0        0        0    32740 2023-04-16 04:55:27.923625 buildarr_sonarr-0.5.0/buildarr_sonarr/config/indexers.py
+-rw-r--r--   0        0        0    19672 2023-04-16 04:55:27.923625 buildarr_sonarr-0.5.0/buildarr_sonarr/config/media_management.py
+-rw-r--r--   0        0        0    11024 2023-04-16 04:55:27.923625 buildarr_sonarr-0.5.0/buildarr_sonarr/config/metadata.py
+-rw-r--r--   0        0        0     1527 2023-04-16 04:55:27.923625 buildarr_sonarr-0.5.0/buildarr_sonarr/config/profiles/__init__.py
+-rw-r--r--   0        0        0    13160 2023-04-16 04:55:27.923625 buildarr_sonarr-0.5.0/buildarr_sonarr/config/profiles/delay.py
+-rw-r--r--   0        0        0    12858 2023-04-16 04:55:27.923625 buildarr_sonarr-0.5.0/buildarr_sonarr/config/profiles/language.py
+-rw-r--r--   0        0        0    16729 2023-04-16 04:55:27.923625 buildarr_sonarr-0.5.0/buildarr_sonarr/config/profiles/quality.py
+-rw-r--r--   0        0        0    17233 2023-04-16 04:55:27.923625 buildarr_sonarr-0.5.0/buildarr_sonarr/config/profiles/release.py
+-rw-r--r--   0        0        0     8322 2023-04-16 04:55:27.923625 buildarr_sonarr-0.5.0/buildarr_sonarr/config/quality.py
+-rw-r--r--   0        0        0     2710 2023-04-16 04:55:27.923625 buildarr_sonarr-0.5.0/buildarr_sonarr/config/tags.py
+-rw-r--r--   0        0        0     1229 2023-04-16 04:55:27.923625 buildarr_sonarr-0.5.0/buildarr_sonarr/config/types.py
+-rw-r--r--   0        0        0     6150 2023-04-16 04:55:27.923625 buildarr_sonarr-0.5.0/buildarr_sonarr/config/ui.py
+-rw-r--r--   0        0        0     1537 2023-04-16 04:55:27.923625 buildarr_sonarr-0.5.0/buildarr_sonarr/config/util.py
+-rw-r--r--   0        0        0     1372 2023-04-16 04:55:27.927625 buildarr_sonarr-0.5.0/buildarr_sonarr/exceptions.py
+-rw-r--r--   0        0        0      938 2023-04-16 04:55:27.927625 buildarr_sonarr-0.5.0/buildarr_sonarr/manager.py
+-rw-r--r--   0        0        0     1165 2023-04-16 04:55:27.927625 buildarr_sonarr-0.5.0/buildarr_sonarr/plugin.py
+-rw-r--r--   0        0        0        0 2023-04-16 04:55:27.927625 buildarr_sonarr-0.5.0/buildarr_sonarr/py.typed
+-rw-r--r--   0        0        0     3408 2023-04-16 04:55:27.927625 buildarr_sonarr-0.5.0/buildarr_sonarr/secrets.py
+-rw-r--r--   0        0        0      980 2023-04-16 04:55:27.927625 buildarr_sonarr-0.5.0/buildarr_sonarr/types.py
+-rw-r--r--   0        0        0     1898 2023-04-16 04:55:27.927625 buildarr_sonarr-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    20944 1970-01-01 00:00:00.000000 buildarr_sonarr-0.5.0/PKG-INFO
```

### Comparing `buildarr_sonarr-0.4.1/LICENSE` & `buildarr_sonarr-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `buildarr_sonarr-0.4.1/README.md` & `buildarr_sonarr-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/__init__.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/api.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,31 +15,29 @@
 """
 Sonarr plugin API functions.
 """
 
 
 from __future__ import annotations
 
-import json
 import re
 
-from datetime import datetime, timezone
 from http import HTTPStatus
 from logging import getLogger
 from typing import TYPE_CHECKING
 
 import json5  # type: ignore[import]
 import requests
 
 from buildarr.state import state
 
 from .exceptions import SonarrAPIError
 
 if TYPE_CHECKING:
-    from typing import Any, Dict, Mapping, Optional
+    from typing import Any, Dict, Optional, Union
 
     from .secrets import SonarrSecrets
 
 
 logger = getLogger(__name__)
 
 INITIALIZE_JS_RES_PATTERN = re.compile(r"(?s)^window\.Sonarr = ({.*});$")
@@ -54,141 +52,228 @@
         api_key (str): Sonarr instance API key, if required. Defaults to `None`.
 
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
+        allow_redirects=False,
     )
+
+    if res.status_code != HTTPStatus.OK:
+        logger.debug("GET %s -> status_code=%i res=%s", url, res.status_code, res.text)
+        if res.status_code in (HTTPStatus.UNAUTHORIZED, HTTPStatus.FOUND):
+            status_code: int = HTTPStatus.UNAUTHORIZED
+            error_message = "Unauthorized"
+        else:
+            status_code = res.status_code
+            error_message = f"Unexpected response with error code {res.status_code}: {res.text}"
+        raise SonarrAPIError(
+            f"Unable to retrieve 'initialize.js': {error_message}",
+            status_code=status_code,
+        )
+
     res_match = re.match(INITIALIZE_JS_RES_PATTERN, res.text)
     if not res_match:
-        raise RuntimeError(f"No matches for initialize.js parsing: {res.text}")
+        raise RuntimeError(f"No matches for 'initialize.js' parsing: {res.text}")
     res_json = json5.loads(res_match.group(1))
+
     logger.debug("GET %s -> status_code=%i res=%s", url, res.status_code, repr(res_json))
+
     return res_json
 
 
-def api_get(secrets: SonarrSecrets, api_url: str) -> Any:
+def api_get(
+    secrets: Union[SonarrSecrets, str],
+    api_url: str,
+    session: Optional[requests.Session] = None,
+    use_api_key: bool = True,
+    expected_status_code: HTTPStatus = HTTPStatus.OK,
+) -> Any:
     """
     Send a `GET` request to a Sonarr instance.
 
     Args:
-        secrets (SonarrSecrets): Sonarr secrets metadata
-        api_url (str): Sonarr API command
+        secrets (Union[SonarrSecrets, str]): Sonarr secrets metadata, or host URL.
+        api_url (str): Sonarr API command.
+        expected_status_code (HTTPStatus): Expected response status. Defaults to `200 OK`.
 
     Returns:
         Response object
     """
 
-    url = f"{secrets.host_url}/{api_url.lstrip('/')}"
+    if isinstance(secrets, str):
+        host_url = secrets
+        api_key = None
+    else:
+        host_url = secrets.host_url
+        api_key = secrets.api_key.get_secret_value() if use_api_key else None
+    url = f"{host_url}/{api_url.lstrip('/')}"
+
     logger.debug("GET %s", url)
-    res = requests.get(
+
+    if not session:
+        session = requests.Session()
+    res = session.get(
         url,
-        headers={"X-Api-Key": secrets.api_key.get_secret_value()},
-        timeout=state.config.buildarr.request_timeout,
+        headers={"X-Api-Key": api_key} if api_key else None,
+        timeout=state.request_timeout,
     )
     res_json = res.json()
+
     logger.debug("GET %s -> status_code=%i res=%s", url, res.status_code, repr(res_json))
-    if res.status_code != HTTPStatus.OK:
+
+    if res.status_code != expected_status_code:
         api_error(method="GET", url=url, response=res)
+
     return res_json
 
 
-def api_post(secrets: SonarrSecrets, api_url: str, req: Any) -> Any:
+def api_post(
+    secrets: Union[SonarrSecrets, str],
+    api_url: str,
+    req: Any = None,
+    session: Optional[requests.Session] = None,
+    use_api_key: bool = True,
+    expected_status_code: HTTPStatus = HTTPStatus.CREATED,
+) -> Any:
     """
     Send a `POST` request to a Sonarr instance.
 
     Args:
-        secrets (SonarrSecrets): Sonarr secrets metadata
-        api_url (str): Sonarr API command
-        req (Any): Request (JSON-serialisable)
+        secrets (Union[SonarrSecrets, str]): Sonarr secrets metadata, or host URL.
+        api_url (str): Sonarr API command.
+        req (Any): Request (JSON-serialisable).
+        expected_status_code (HTTPStatus): Expected response status. Defaults to `201 Created`.
 
     Returns:
         Response object
     """
 
-    url = f"{secrets.host_url}/{api_url.lstrip('/')}"
-    logger.debug("POST %s <- req=%s", url, repr(req))
-    headers = {"X-Api-Key": secrets.api_key.get_secret_value()}
-    if not state.dry_run:
-        res = requests.post(
-            url,
-            headers=headers,
-            json=req,
-            timeout=state.config.buildarr.request_timeout,
-        )
+    if isinstance(secrets, str):
+        host_url = secrets
+        api_key = None
     else:
-        res = _create_dryrun_response("POST", url, content=json.dumps(req))
+        host_url = secrets.host_url
+        api_key = secrets.api_key.get_secret_value() if use_api_key else None
+    url = f"{host_url}/{api_url.lstrip('/')}"
+
+    logger.debug("POST %s <- req=%s", url, repr(req))
+
+    if not session:
+        session = requests.Session()
+    res = session.post(
+        url,
+        headers={"X-Api-Key": api_key} if api_key else None,
+        timeout=state.request_timeout,
+        **({"json": req} if req is not None else {}),
+    )
     res_json = res.json()
+
     logger.debug("POST %s -> status_code=%i res=%s", url, res.status_code, repr(res_json))
-    if res.status_code != HTTPStatus.CREATED:
+
+    if res.status_code != expected_status_code:
         api_error(method="POST", url=url, response=res)
+
     return res_json
 
 
-def api_put(secrets: SonarrSecrets, api_url: str, req: Any) -> Any:
+def api_put(
+    secrets: Union[SonarrSecrets, str],
+    api_url: str,
+    req: Any,
+    session: Optional[requests.Session] = None,
+    use_api_key: bool = True,
+    expected_status_code: HTTPStatus = HTTPStatus.ACCEPTED,
+) -> Any:
     """
     Send a `PUT` request to a Sonarr instance.
 
     Args:
-        secrets (SonarrSecrets): Sonarr secrets metadata
-        api_url (str): Sonarr API command
-        req (Any): Request (JSON-serialisable)
+        secrets (Union[SonarrSecrets, str]): Sonarr secrets metadata, or host URL.
+        api_url (str): Sonarr API command.
+        req (Any): Request (JSON-serialisable).
+        expected_status_code (HTTPStatus): Expected response status. Defaults to `200 OK`.
 
     Returns:
         Response object
     """
 
-    url = f"{secrets.host_url}/{api_url.lstrip('/')}"
-    logger.debug("PUT %s <- req=%s", url, repr(req))
-    headers = {"X-Api-Key": secrets.api_key.get_secret_value()}
-    if not state.dry_run:
-        res = requests.put(
-            url,
-            headers=headers,
-            json=req,
-            timeout=state.config.buildarr.request_timeout,
-        )
+    if isinstance(secrets, str):
+        host_url = secrets
+        api_key = None
     else:
-        res = _create_dryrun_response("PUT", url, content=json.dumps(req))
+        host_url = secrets.host_url
+        api_key = secrets.api_key.get_secret_value() if use_api_key else None
+    url = f"{host_url}/{api_url.lstrip('/')}"
+
+    logger.debug("PUT %s <- req=%s", url, repr(req))
+
+    if not session:
+        session = requests.Session()
+    res = session.put(
+        url,
+        headers={"X-Api-Key": api_key} if api_key else None,
+        json=req,
+        timeout=state.request_timeout,
+    )
     res_json = res.json()
+
     logger.debug("PUT %s -> status_code=%i res=%s", url, res.status_code, repr(res_json))
-    if res.status_code != HTTPStatus.ACCEPTED:
+
+    if res.status_code != expected_status_code:
         api_error(method="PUT", url=url, response=res)
+
     return res_json
 
 
-def api_delete(secrets: SonarrSecrets, api_url: str) -> None:
+def api_delete(
+    secrets: Union[SonarrSecrets, str],
+    api_url: str,
+    session: Optional[requests.Session] = None,
+    use_api_key: bool = True,
+    expected_status_code: HTTPStatus = HTTPStatus.OK,
+) -> None:
     """
     Send a `DELETE` request to a Sonarr instance.
 
     Args:
-        secrets (SonarrSecrets): Sonarr secrets metadata
-        api_url (str): Sonarr API command
+        secrets (Union[SonarrSecrets, str]): Sonarr secrets metadata, or host URL.
+        api_url (str): Sonarr API command.
+        expected_status_code (HTTPStatus): Expected response status. Defaults to `200 OK`.
     """
 
-    url = f"{secrets.host_url}/{api_url.lstrip('/')}"
+    if isinstance(secrets, str):
+        host_url = secrets
+        api_key = None
+    else:
+        host_url = secrets.host_url
+        api_key = secrets.api_key.get_secret_value() if use_api_key else None
+    url = f"{host_url}/{api_url.lstrip('/')}"
+
     logger.debug("DELETE %s", url)
-    headers = {"X-Api-Key": secrets.api_key.get_secret_value()}
-    res = (
-        requests.delete(
-            url,
-            headers=headers,
-            timeout=state.config.buildarr.request_timeout,
-        )
-        if not state.dry_run
-        else _create_dryrun_response("DELETE", url)
+
+    if not session:
+        session = requests.Session()
+    res = session.delete(
+        url,
+        headers={"X-Api-Key": api_key} if api_key else None,
+        timeout=state.request_timeout,
     )
+
     logger.debug("DELETE %s -> status_code=%i", url, res.status_code)
-    if res.status_code != HTTPStatus.OK:
+
+    if res.status_code != expected_status_code:
         api_error(method="DELETE", url=url, response=res, parse_response=False)
 
 
 def api_error(
     method: str,
     url: str,
     response: requests.Response,
@@ -215,15 +300,15 @@
         try:
             error_message += f" {_api_error(res_json)}"
         except TypeError:
             for error in res_json:
                 error_message += f"\n{_api_error(error)}"
         except KeyError:
             error_message += f" {res_json}"
-    raise SonarrAPIError(error_message, response=response)
+    raise SonarrAPIError(error_message, status_code=response.status_code)
 
 
 def _api_error(res_json: Any) -> str:
     """
     Generate an error message from a response object.
 
     Args:
@@ -246,68 +331,7 @@
         try:
             return f"{res_json['message']}\n{res_json['description']}"
         except KeyError:
             pass
         return res_json["message"]
     except KeyError:
         return f"(Unsupported error JSON format) {res_json}"
-
-
-def _create_dryrun_response(
-    method: str,
-    url: str,
-    headers: Optional[Mapping[str, str]] = None,
-    status_code: Optional[int] = None,
-    content_type: str = "application/json",
-    charset: str = "utf-8",
-    content: str = "{}",
-) -> requests.Response:
-    """
-    A utility function for generating `requests.Response` objects in dry-run mode.
-
-    Args:
-        method (str): HTTP method of the response to simulate.
-        url (str): URL of the request.
-        status_code (Optional[int], optional): Status code for the response. Default: auto-detect
-        content_type (str, optional): MIME type of response content. Default: `application/json`
-        charset (str, optional): Encoding of response content. Default: `utf-8`
-        content (str, optional): Response content. Default: `{}`
-
-    Raises:
-        ValueError: When an unsupported HTTP method is used
-
-    Returns:
-        Generated `requests.Response` object
-    """
-
-    method = method.upper()
-
-    response = requests.Response()
-    response.url = url
-    response.headers["Vary"] = "Accept"
-    response.headers["Cache-Control"] = "no-cache, no-store, must-revalidate, max-age=0"
-    response.headers["Pragma"] = "no-cache"
-    response.headers["Expires"] = "0"
-    response.headers["Access-Control-Allow-Origin"] = "*"
-    response.headers["Content-Type"] = f"{content_type}; charset={charset}"
-    response.headers["Server"] = "Mono-HTTPAPI/1.0"
-    response.headers["Date"] = datetime.now(tz=timezone.utc).strftime("%a, %d %b %Y %H:%M:%S %Z")
-    response.headers["Transfer-Encoding"] = "chunked"
-    if headers:
-        response.headers.update(headers)
-    if status_code is not None:
-        response.status_code = status_code
-    elif method == "POST":
-        response.status_code = int(HTTPStatus.CREATED)
-    elif method == "PUT":
-        response.status_code = int(HTTPStatus.ACCEPTED)
-    elif method == "DELETE":
-        response.status_code = int(HTTPStatus.OK)
-    else:
-        raise ValueError(
-            f"Unsupported HTTP method for creating dry-run response: {str(method)}",
-        )
-    response.encoding = charset
-    if content is not None:
-        response._content = content.encode("UTF-8")
-
-    return response
```

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/cli.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/cli.py`

 * *Files identical despite different names*

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/config/__init__.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/config/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 """
 Sonarr plugin configuration.
 """
 
 
 from __future__ import annotations
 
-from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, Optional
 
 from buildarr.config import ConfigPlugin
 from buildarr.types import NonEmptyStr, Port
 from typing_extensions import Self
 
 from ..api import api_get
@@ -54,60 +53,38 @@
 
 
 class SonarrSettingsConfig(SonarrConfigBase):
     """
     Sonarr settings, used to configure a remote Sonarr instance.
     """
 
-    #: Media management settings.
     media_management = SonarrMediaManagementSettingsConfig()
-
-    #: Profile settings (quality, language, delay, release profiles).
     profiles = SonarrProfilesSettingsConfig()
-
-    #: Quality definition settings.
     quality = SonarrQualitySettingsConfig()
-
-    #: Usenet/BitTorrent indexer settings.
     indexers = SonarrIndexersSettingsConfig()
-
-    #: Usenet/BitTorrent download client settings.
     download_clients = SonarrDownloadClientsSettingsConfig()
-
-    #: Import list settings.
     import_lists = SonarrImportListsSettingsConfig()
-
-    #: Notification connection settings.
     connect = SonarrConnectSettingsConfig()
-
-    #: Metadata file settings.
     metadata = SonarrMetadataSettingsConfig()
-
-    #: Tag settings.
     tags = SonarrTagsSettingsConfig()
-
-    #: General instance settings.
     general = SonarrGeneralSettingsConfig()
-
-    #: User interface settings.
     ui = SonarrUISettingsConfig()
 
     def update_remote(
         self,
         tree: str,
         secrets: SonarrSecrets,
         remote: Self,
         check_unmanaged: bool = False,
     ) -> bool:
         # Overload base function to guarantee execution order of section updates.
-        # 1. Tags must be created before everything else, and destroyed after they
-        #    are no longer referenced elsewhere.
+        # 1. Tags must be created before everything else.
         # 2. Qualities must be updated before quality profiles.
-        # 3. Indexers must be created before release profiles, and destroyed after they
-        #    are no longer referenced by them.
+        # 3. Download clients must be created before indexers.
+        # 4. Indexers must be created before release profiles.
         return any(
             [
                 self.tags.update_remote(
                     f"{tree}.tags",
                     secrets,
                     remote.tags,
                     check_unmanaged=check_unmanaged,
@@ -168,16 +145,46 @@
                 ),
                 self.ui.update_remote(
                     f"{tree}.ui",
                     secrets,
                     remote.ui,
                     check_unmanaged=check_unmanaged,
                 ),
-                # TODO: destroy indexers
-                # TODO: destroy tags
+            ],
+        )
+
+    def delete_remote(self, tree: str, secrets: SonarrSecrets, remote: Self) -> bool:
+        # Overload base function to guarantee execution order of section deletions.
+        # 1. Release profiles must be deleted before indexers.
+        # 2. Indexers must be deleted before download clients.
+        return any(
+            [
+                self.profiles.delete_remote(f"{tree}.profiles", secrets, remote.profiles),
+                self.indexers.delete_remote(f"{tree}.indexers", secrets, remote.indexers),
+                self.download_clients.delete_remote(
+                    f"{tree}.download_clients",
+                    secrets,
+                    remote.download_clients,
+                ),
+                self.media_management.delete_remote(
+                    f"{tree}.media_management",
+                    secrets,
+                    remote.media_management,
+                ),
+                self.import_lists.delete_remote(
+                    f"{tree}.import_lists",
+                    secrets,
+                    remote.import_lists,
+                ),
+                self.connect.delete_remote(f"{tree}.connect", secrets, remote.connect),
+                self.tags.delete_remote(f"{tree}.tags", secrets, remote.tags),
+                self.quality.delete_remote(f"{tree}.quality", secrets, remote.quality),
+                self.metadata.delete_remote(f"{tree}.metadata", secrets, remote.metadata),
+                self.general.delete_remote(f"{tree}.general", secrets, remote.general),
+                self.ui.delete_remote(f"{tree}.ui", secrets, remote.ui),
             ],
         )
 
 
 class SonarrInstanceConfig(_SonarrInstanceConfig):
     """
     By default, Buildarr will look for a single instance at `http://sonarr:8989`.
@@ -270,55 +277,35 @@
 
     settings: SonarrSettingsConfig = SonarrSettingsConfig()
     """
     Sonarr settings.
     Configuration options for Sonarr itself are set within this structure.
     """
 
-    @property
     def uses_trash_metadata(self) -> bool:
-        """
-        A flag determining whether or not this configuration uses TRaSH-Guides metadata.
-
-        Returns:
-            `True` if TRaSH-Guides metadata is used, otherwise `False`
-        """
-        if self.settings.quality.uses_trash_metadata:
+        if self.settings.quality.uses_trash_metadata():
             return True
         for release_profile in self.settings.profiles.release_profiles.definitions.values():
-            if release_profile.uses_trash_metadata:
+            if release_profile.uses_trash_metadata():
                 return True
         return False
 
-    def render_trash_metadata(self, trash_metadata_dir: Path) -> Self:
-        """
-        Read TRaSH-Guides metadata, and return a configuration object with all templates rendered.
-
-        Args:
-            trash_metadata_dir (Path): TRaSH-Guides metadata directory.
-
-        Returns:
-            Rendered configuration object
-        """
+    def render(self) -> Self:
+        if not self.uses_trash_metadata():
+            return self
         copy = self.copy(deep=True)
-        copy._render_trash_metadata(trash_metadata_dir)
+        copy._render()
         return copy
 
-    def _render_trash_metadata(self, trash_metadata_dir: Path) -> None:
-        """
-        Render configuration attributes obtained from TRaSH-Guides, in-place.
-
-        Args:
-            trash_metadata_dir (Path): TRaSH-Guides metadata directory.
-        """
+    def _render(self) -> None:
         for rp in self.settings.profiles.release_profiles.definitions.values():
-            if rp.uses_trash_metadata:
-                rp._render_trash_metadata(trash_metadata_dir)
-        if self.settings.quality.uses_trash_metadata:
-            self.settings.quality._render_trash_metadata(trash_metadata_dir)
+            if rp.uses_trash_metadata():
+                rp._render()
+        if self.settings.quality.uses_trash_metadata():
+            self.settings.quality._render()
 
     @classmethod
     def from_remote(cls, secrets: SonarrSecrets) -> Self:
         """
         Read configuration from a remote instance and return it as a configuration object.
 
         Args:
@@ -353,38 +340,7 @@
     Instance-specific Sonarr configuration.
 
     Can only be defined on the global `sonarr` configuration block.
 
     Globally specified configuration values apply to all instances.
     Configuration values specified on an instance-level take precedence at runtime.
     """
-
-    @property
-    def uses_trash_metadata(self) -> bool:
-        """
-        A flag determining whether or not this configuration uses TRaSH-Guides metadata.
-
-        Returns:
-            `True` if TRaSH-Guides metadata is used, otherwise `False`
-        """
-        for instance in self.instances.values():
-            if instance.uses_trash_metadata:
-                return True
-        return super().uses_trash_metadata
-
-    def render_trash_metadata(self, trash_metadata_dir: Path) -> Self:
-        """
-        Read TRaSH-Guides metadata, and return a configuration object with all templates rendered.
-
-        Args:
-            trash_metadata_dir (Path): TRaSH-Guides metadata directory.
-
-        Returns:
-            Rendered configuration object
-        """
-        copy = self.copy(deep=True)
-        for instance in copy.instances.values():
-            if instance.uses_trash_metadata:
-                instance._render_trash_metadata(trash_metadata_dir)
-        if self.uses_trash_metadata:
-            copy._render_trash_metadata(trash_metadata_dir)
-        return copy
```

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/config/connect.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/config/connect.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,27 +20,27 @@
 from __future__ import annotations
 
 from datetime import datetime
 from logging import getLogger
 from typing import Any, Dict, List, Literal, Mapping, Optional, Set, Tuple, Type, Union
 
 from buildarr.config import RemoteMapEntry
-from buildarr.types import BaseEnum, BaseIntEnum, NonEmptyStr, Password, Port
+from buildarr.types import BaseEnum, NonEmptyStr, Password, Port
 from pydantic import AnyHttpUrl, ConstrainedInt, Field, NameEmail, SecretStr
 from typing_extensions import Annotated, Self
 
 from ..api import api_delete, api_get, api_post, api_put
 from ..secrets import SonarrSecrets
 from .types import SonarrConfigBase, TraktAuthUser
 from .util import trakt_expires_encoder
 
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
@@ -373,16 +373,15 @@
                     **triggers_remote_attrs,
                     **base_remote_attrs,
                 },
             )
             return True
         return False
 
-    def _delete_remote(self, tree: str, secrets: SonarrSecrets, connection_id: int) -> None:
-        logger.info("%s: (...) -> (deleted)", tree)
+    def _delete_remote(self, secrets: SonarrSecrets, connection_id: int) -> None:
         api_delete(secrets, f"/api/v3/notification/{connection_id}")
 
 
 class BoxcarConnection(Connection):
     """
     Receive media update and health alert push notifications via Boxcar.
 
@@ -1750,57 +1749,58 @@
     def update_remote(
         self,
         tree: str,
         secrets: SonarrSecrets,
         remote: Self,
         check_unmanaged: bool = False,
     ) -> bool:
-        #
         changed = False
-        #
         connection_ids: Dict[str, int] = {
             connection_json["name"]: connection_json["id"]
             for connection_json in api_get(secrets, "/api/v3/notification")
         }
         tag_ids: Dict[str, int] = (
             {tag["label"]: tag["id"] for tag in api_get(secrets, "/api/v3/tag")}
             if any(connection.tags for connection in self.definitions.values())
             or any(connection.tags for connection in remote.definitions.values())
             else {}
         )
-        #
         for connection_name, connection in self.definitions.items():
             connection_tree = f"{tree}.definitions[{repr(connection_name)}]"
-            #
             if connection_name not in remote.definitions:
                 connection._create_remote(
                     tree=connection_tree,
                     secrets=secrets,
                     tag_ids=tag_ids,
                     connection_name=connection_name,
                 )
                 changed = True
-            #
             elif connection._update_remote(
                 tree=connection_tree,
                 secrets=secrets,
                 remote=remote.definitions[connection_name],  # type: ignore[arg-type]
                 tag_ids=tag_ids,
                 connection_id=connection_ids[connection_name],
                 connection_name=connection_name,
             ):
                 changed = True
-        #
+        return changed
+
+    def delete_remote(self, tree: str, secrets: SonarrSecrets, remote: Self) -> bool:
+        changed = False
+        connection_ids: Dict[str, int] = {
+            connection_json["name"]: connection_json["id"]
+            for connection_json in api_get(secrets, "/api/v3/notification")
+        }
         for connection_name, connection in remote.definitions.items():
             if connection_name not in self.definitions:
                 connection_tree = f"{tree}.definitions[{repr(connection_name)}]"
                 if self.delete_unmanaged:
+                    logger.info("%s: (...) -> (deleted)", connection_tree)
                     connection._delete_remote(
-                        tree=connection_tree,
                         secrets=secrets,
                         connection_id=connection_ids[connection_name],
                     )
                     changed = True
                 else:
                     logger.debug("%s: (...) (unmanaged)", connection_tree)
-        #
         return changed
```

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/config/download_clients/__init__.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/config/download_clients/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -220,16 +220,14 @@
         }
         tag_ids: Dict[str, int] = (
             {tag["label"]: tag["id"] for tag in api_get(secrets, "/api/v3/tag")}
             if any(downloadclient.tags for downloadclient in local.values())
             or any(downloadclient.tags for downloadclient in remote.values())
             else {}
         )
-        # Create download clients that don't exist yet on the remote,
-        # and update in-place ones that do.
         for downloadclient_name, downloadclient in local.items():
             downloadclient_tree = f"{tree}[{repr(downloadclient_name)}]"
             if downloadclient_name not in remote:
                 downloadclient._create_remote(
                     tree=downloadclient_tree,
                     secrets=secrets,
                     tag_ids=tag_ids,
@@ -241,24 +239,48 @@
                 secrets=secrets,
                 remote=remote[downloadclient_name],  # type: ignore[arg-type]
                 tag_ids=tag_ids,
                 downloadclient_id=downloadclient_ids[downloadclient_name],
                 downloadclient_name=downloadclient_name,
             ):
                 changed = True
-        # If `delete_unmanaged` is `True`, remove any download clients on the remote
-        # that aren't managed by Buildarr.
-        # Otherwise, just log them.
+        return changed
+
+    def delete_remote(self, tree: str, secrets: SonarrSecrets, remote: Self) -> bool:
+        definitions_changed = self._delete_remote_definitions(
+            tree=f"{tree}.definitions",
+            secrets=secrets,
+            local=self.definitions,
+            remote=remote.definitions,
+        )
+        rpms_changed = self.remote_path_mappings._delete_remote(
+            tree=f"{tree}.remote_path_mappings",
+            secrets=secrets,
+            remote=remote.remote_path_mappings,
+        )
+        return any([definitions_changed, rpms_changed])
+
+    def _delete_remote_definitions(
+        self,
+        tree: str,
+        secrets: SonarrSecrets,
+        local: Mapping[str, DownloadClientType],
+        remote: Mapping[str, DownloadClientType],
+    ) -> bool:
+        changed = False
+        downloadclient_ids: Dict[str, int] = {
+            downloadclient_json["name"]: downloadclient_json["id"]
+            for downloadclient_json in api_get(secrets, "/api/v3/downloadclient")
+        }
         for downloadclient_name, downloadclient in remote.items():
             if downloadclient_name not in local:
                 downloadclient_tree = f"{tree}[{repr(downloadclient_name)}]"
                 if self.delete_unmanaged:
+                    logger.info("%s: (...) -> (deleted)", downloadclient_tree)
                     downloadclient._delete_remote(
-                        tree=downloadclient_tree,
                         secrets=secrets,
                         downloadclient_id=downloadclient_ids[downloadclient_name],
                     )
                     changed = True
                 else:
                     logger.debug("%s: (...) (unmanaged)", downloadclient_tree)
-        # Return the resource changed status.
         return changed
```

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/config/download_clients/download_clients.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/config/download_clients/download_clients.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,21 +376,15 @@
                     "configContract": self._config_contract,
                     **remote_attrs,
                 },
             )
             return True
         return False
 
-    def _delete_remote(
-        self,
-        tree: str,
-        secrets: SonarrSecrets,
-        downloadclient_id: int,
-    ) -> None:
-        logger.info("%s: (...) -> (deleted)", tree)
+    def _delete_remote(self, secrets: SonarrSecrets, downloadclient_id: int) -> None:
         api_delete(secrets, f"/api/v3/downloadclient/{downloadclient_id}")
 
 
 class UsenetDownloadClient(DownloadClient):
     """
     Usenet-based download client.
     """
```

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/config/download_clients/remote_path_mappings.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/config/download_clients/remote_path_mappings.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,21 +118,15 @@
                 secrets,
                 f"/api/v3/remotepathmapping/{remotepathmapping_id}",
                 {"id": remotepathmapping_id, **remote_attrs},
             )
             return True
         return False
 
-    def _delete_remote(
-        self,
-        tree: str,
-        secrets: SonarrSecrets,
-        remotepathmapping_id: int,
-    ) -> None:
-        logger.info("%s: (...) -> (deleted)", tree)
+    def _delete_remote(self, secrets: SonarrSecrets, remotepathmapping_id: int) -> None:
         api_delete(secrets, f"/api/v3/remotepathmapping/{remotepathmapping_id}")
 
 
 class SonarrRemotePathMappingsSettingsConfig(SonarrConfigBase):
     """
     Remote path mappings are used to associate a path on a download client remote host
     with its associated path on the local Sonarr instance.
@@ -201,17 +195,14 @@
         changed = False
         # Get required resource IDs from the remote, and create
         # data structures.
         remote_rpm_ids: Dict[Tuple[str, str, str], int] = {
             (rpm["host"], rpm["remotePath"], rpm["localPath"]): rpm["id"]
             for rpm in api_get(secrets, "/api/v3/remotepathmapping")
         }
-        local_rpms: Dict[Tuple[str, str, str], RemotePathMapping] = {
-            (rpm.host, rpm.remote_path, rpm.local_path): rpm for rpm in self.definitions
-        }
         remote_rpms: Dict[Tuple[str, str, str], RemotePathMapping] = {
             (rpm.host, rpm.remote_path, rpm.local_path): rpm for rpm in remote.definitions
         }
         # Handle managed remote path mappings.
         for i, rpm in enumerate(self.definitions):
             rpm_tree = f"{tree}.definitions[{i}]"
             rpm_tuple = (rpm.host, rpm.remote_path, rpm.local_path)
@@ -225,34 +216,41 @@
                     rpm._create_remote(tree=rpm_tree, secrets=secrets)
                     changed = True
             # If the remote path mapping should not exist, check that it does not
             # exist in the remote, and if it does, delete it.
             elif rpm_tuple in remote_rpms:
                 logger.info("%s: %s -> (deleted)", rpm_tree, repr(rpm))
                 rpm._delete_remote(
-                    tree=rpm_tree,
                     secrets=secrets,
                     remotepathmapping_id=remote_rpm_ids[rpm_tuple],
                 )
                 changed = True
             else:
                 logger.debug("%s: %s (does not exist)", rpm_tree, repr(rpm))
-        # Handle unmanaged remote path mappings.
-        # If `delete_unmanaged` is `True`, automatically delete them.
-        j = -1
+        # Return changed status.
+        return changed
+
+    def _delete_remote(self, tree: str, secrets: SonarrSecrets, remote: Self) -> bool:
+        changed = False
+        remote_rpm_ids: Dict[Tuple[str, str, str], int] = {
+            (rpm["host"], rpm["remotePath"], rpm["localPath"]): rpm["id"]
+            for rpm in api_get(secrets, "/api/v3/remotepathmapping")
+        }
+        local_rpms: Dict[Tuple[str, str, str], RemotePathMapping] = {
+            (rpm.host, rpm.remote_path, rpm.local_path): rpm for rpm in self.definitions
+        }
+        i = -1
         for rpm in remote.definitions:
             rpm_tuple = (rpm.host, rpm.remote_path, rpm.local_path)
             if rpm_tuple not in local_rpms:
-                rpm_tree = f"{tree}.definitions[{j}]"
+                rpm_tree = f"{tree}.definitions[{i}]"
                 if self.delete_unmanaged:
                     logger.info("%s: %s -> (deleted)", rpm_tree, repr(rpm))
                     rpm._delete_remote(
-                        tree=rpm_tree,
                         secrets=secrets,
                         remotepathmapping_id=remote_rpm_ids[rpm_tuple],
                     )
                     changed = True
                 else:
                     logger.debug("%s: %s (unmanaged)", rpm_tree, repr(rpm))
-                j -= 1
-        # Return changed status.
+                i -= 1
         return changed
```

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/config/general.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/config/general.py`

 * *Files identical despite different names*

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/config/import_lists.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/config/import_lists.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from __future__ import annotations
 
 import re
 
 from datetime import datetime
 from logging import getLogger
 from typing import (
-    TYPE_CHECKING,
     Any,
     Dict,
     Iterable,
     List,
     Literal,
     Mapping,
     Optional,
@@ -47,20 +46,14 @@
 
 from ..api import api_delete, api_get, api_post, api_put
 from ..secrets import SonarrSecrets
 from ..types import SonarrApiKey
 from .types import SonarrConfigBase, TraktAuthUser
 from .util import trakt_expires_encoder
 
-if TYPE_CHECKING:
-    from typing import Collection
-
-    from ..config import SonarrInstanceConfig
-
-
 logger = getLogger(__name__)
 
 
 class YearRange(ConstrainedStr):
     """
     Constrained string type for a singular year or range of years.
     """
@@ -422,24 +415,23 @@
                     "configContract": self._config_contract,
                     **remote_attrs,
                 },
             )
             return True
         return False
 
-    def _delete_remote(self, tree: str, secrets: SonarrSecrets, importlist_id: int) -> None:
+    def _delete_remote(self, secrets: SonarrSecrets, importlist_id: int) -> None:
         """
         Delete this import list from the remote Sonarr instance.
 
         Args:
             tree (str): Configuration tree. Used for logging.
             secrets (SonarrSecrets): Secrets metadata for the remote instance.
             importlist_id (int): ID associated with this import list on the remote instance.
         """
-        logger.info("%s: (...) -> (deleted)", tree)
         api_delete(secrets, f"/api/v3/importlist/{importlist_id}")
 
 
 class ProgramImportList(ImportList):
     """
     Base class for program-based import lists.
     """
@@ -879,45 +871,32 @@
                 if not isinstance(resource, int):
                     raise RuntimeError(
                         f"{resource_type} reference should be of type int here: {resource}",
                     )
                 resource_ids.add(resource)
             return sorted(resource_ids)
         source_resource_ids: Optional[Dict[str, int]] = None
-        for i, resource in enumerate(resources):
+        for resource in resources:
             if isinstance(resource, int):
                 resource_ids.add(resource)
             else:
                 if source_resource_ids is None:
                     source_resource_ids = {
                         p[name_key]: p["id"]
                         for p in cls._get_resources(
                             instance_name,
                             resource_type,
                         )
                     }
                 try:
                     resource_ids.add(source_resource_ids[resource])
                 except KeyError as err:
-                    # If this is a dry-run, then a non-existent resource name was passed from
-                    # the instance reference resolver.
-                    # Generate a fake ID based on the maximum existing resource ID
-                    # and the index of the resource name being currently processed, and
-                    # add it to the result.
-                    # (Since this is a dry-run, it's fine that it's fake.)
-                    if state.dry_run:
-                        max_id = max(source_resource_ids.values()) if resource_ids else 1
-                        resource_ids.add(max_id + i)
-                    # If this is **not** a dry-run, then a non-existent resource name
-                    # somehow made it past all the validation being done.
-                    # Raise a runtime error and report back to the user.
-                    else:
-                        raise RuntimeError(
-                            f"Unable to find ID for {resource_type} '{err.args[0]}'",
-                        ) from None
+                    raise RuntimeError(
+                        f"Unable to find ID for {resource_type} '{err.args[0]}'",
+                    ) from None
         return sorted(resource_ids)
 
     def _resolve_from_local(
         self,
         name: str,
         local: Self,
         ignore_nonexistent_ids: bool = False,
@@ -1025,62 +1004,29 @@
                         raise ValueError(
                             f"Source {resource_description} ID {resource} "
                             f"not found on target instance '{instance_name}",
                         ) from None
             elif resource in resource_ids:
                 resolved_source_resources.add(resource)
             else:
-                # If dry-run mode is enabled, then there is a very good chance
-                # the resource does not yet exist on the target Sonarr instance.
-                # Since the instance is also managed by Buildarr, go into its configuration
-                # and check if the resource name is defined.
-                #
-                # If the resource is defined, continue as normal, and a fake ID will be assigned
-                # when encoding the request, so the dry run will complete as expected.
-                #
-                # If the resource is **not** defined, raise an error as it would
-                # in the non-dry-run case, but set `available_resources` so that
-                # the error message will be accurate.
-                if state.dry_run:
-                    target_instance_config: SonarrInstanceConfig = state.instance_configs["sonarr"][
-                        instance_name
-                    ]  # type: ignore[assignment]
-                    settings = target_instance_config.settings
-                    definitions: Collection[str] = getattr(
-                        settings.profiles if resource_type_int.endswith("_profile") else settings,
-                        f"{resource_type_int}s",
-                    ).definitions
-                    if resource in definitions:
-                        resolved_source_resources.add(resource)
-                        continue
-                    available_resources = list(definitions)
-                # If this is not a dry-run, then either the user has not defined the
-                # resource on the target instance, or for some reason it wasn't created.
-                # Either way, raise an error.
-                else:
-                    available_resources = list(resource_ids.keys())
+                available_resources = list(resource_ids.keys())
                 _resources_str = (
                     ", ".join(repr(p) for p in available_resources)
                     if available_resources
                     else "(none)"
                 )
                 error_message = (
                     f"Source {resource_description} '{resource}' "
                     f"not found on target Sonarr instance '{instance_name}' "
                     f"in import list '{name}' "
                     f"(available {resource_description}s: {_resources_str})"
                 )
                 raise ValueError(error_message)
         return resolved_source_resources
 
-    class Config(SonarrConfigBase.Config):
-        # Ensure in-place assignments of attributes are always validated,
-        # since this class performs such modifications in certain cases.
-        validate_assignment = True
-
 
 class PlexWatchlistImportList(PlexImportList):
     """
     Import items from a Plex watchlist.
     """
 
     type: Literal["plex-watchlist"] = "plex-watchlist"
@@ -1348,23 +1294,29 @@
                 quality_profile_ids=quality_profile_ids,
                 language_profile_ids=language_profile_ids,
                 tag_ids=tag_ids,
                 importlist_id=importlist_ids[importlist_name],
                 importlist_name=importlist_name,
             ):
                 changed = True
-        # Find import list definitions on the remote that aren't configured locally.
-        # If `delete_unmanaged` is `True`, delete them. If not, just log them as unmanaged.
+        # We're done!
+        return changed
+
+    def delete_remote(self, tree: str, secrets: SonarrSecrets, remote: Self) -> bool:
+        changed = False
+        importlist_ids: Dict[str, int] = {
+            importlist_json["name"]: importlist_json["id"]
+            for importlist_json in api_get(secrets, "/api/v3/importlist")
+        }
         for importlist_name, importlist in remote.definitions.items():
             if importlist_name not in self.definitions:
                 importlist_tree = f"{tree}.definitions[{repr(importlist_name)}]"
                 if self.delete_unmanaged:
+                    logger.info("%s: (...) -> (deleted)", importlist_tree)
                     importlist._delete_remote(
-                        tree=importlist_tree,
                         secrets=secrets,
                         importlist_id=importlist_ids[importlist_name],
                     )
                     changed = True
                 else:
                     logger.debug("%s: (...) (unmanaged)", importlist_tree)
-        # We're done!
         return changed
```

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/config/indexers.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/config/indexers.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,26 +19,26 @@
 
 from __future__ import annotations
 
 from logging import getLogger
 from typing import Any, Dict, List, Literal, Mapping, Optional, Set, Tuple, Type, Union
 
 from buildarr.config import RemoteMapEntry
-from buildarr.types import BaseEnum, BaseIntEnum, NonEmptyStr, Password, RssUrl
+from buildarr.types import BaseEnum, NonEmptyStr, Password, RssUrl
 from pydantic import AnyHttpUrl, Field, PositiveInt
 from typing_extensions import Annotated, Self
 
 from ..api import api_delete, api_get, api_post, api_put
 from ..secrets import SonarrSecrets
 from .types import SonarrConfigBase
 
 logger = getLogger(__name__)
 
 
-class NabCategory(BaseIntEnum):
+class NabCategory(BaseEnum):
     """
     Newznab/Torznab category enumeration.
     """
 
     TV_WEBDL = 5010
     TV_FOREIGN = 5020
     TV_SD = 5030
@@ -245,16 +245,15 @@
                     "configContract": self._config_contract,
                     **remote_attrs,
                 },
             )
             return True
         return False
 
-    def _delete_remote(self, tree: str, secrets: SonarrSecrets, indexer_id: int) -> None:
-        logger.info("%s: (...) -> (deleted)", tree)
+    def _delete_remote(self, secrets: SonarrSecrets, indexer_id: int) -> None:
         api_delete(secrets, f"/api/v3/indexer/{indexer_id}")
 
 
 class UsenetIndexer(Indexer):
     """
     Usenet indexer base class.
     """
@@ -1079,17 +1078,15 @@
     def update_remote(
         self,
         tree: str,
         secrets: SonarrSecrets,
         remote: Self,
         check_unmanaged: bool = False,
     ) -> bool:
-        #
         changed = False
-        #
         indexer_ids: Dict[str, int] = {
             indexer["name"]: indexer["id"] for indexer in api_get(secrets, "/api/v3/indexer")
         }
         download_client_ids: Dict[str, int] = (
             {dc["name"]: dc["id"] for dc in api_get(secrets, "/api/v3/downloadclient")}
             if any(indexer.download_client for indexer in self.definitions.values())
             or any(indexer.download_client for indexer in remote.definitions.values())
@@ -1097,60 +1094,61 @@
         )
         tag_ids: Dict[str, int] = (
             {tag["label"]: tag["id"] for tag in api_get(secrets, "/api/v3/tag")}
             if any(indexer.tags for indexer in self.definitions.values())
             or any(indexer.tags for indexer in remote.definitions.values())
             else {}
         )
-        #
         config_changed, config_remote_attrs = self.get_update_remote_attrs(
             tree,
             remote,
             self._remote_map,
             check_unmanaged=check_unmanaged,
         )
         if config_changed:
             api_put(
                 secrets,
                 f"/api/v3/config/indexer/{api_get(secrets, '/api/v3/config/indexer')['id']}",
                 config_remote_attrs,
             )
             changed = True
-        #
         for indexer_name, indexer in self.definitions.items():
             indexer_tree = f"{tree}.definitions[{repr(indexer_name)}]"
-            #
             if indexer_name not in remote.definitions:
                 indexer._create_remote(
                     tree=indexer_tree,
                     secrets=secrets,
                     download_client_ids=download_client_ids,
                     tag_ids=tag_ids,
                     indexer_name=indexer_name,
                 )
                 changed = True
-            #
             elif indexer._update_remote(
                 tree=indexer_tree,
                 secrets=secrets,
                 remote=remote.definitions[indexer_name],  # type: ignore[arg-type]
                 download_client_ids=download_client_ids,
                 tag_ids=tag_ids,
                 indexer_id=indexer_ids[indexer_name],
                 indexer_name=indexer_name,
             ):
                 changed = True
-        #
+        return changed
+
+    def delete_remote(self, tree: str, secrets: SonarrSecrets, remote: Self) -> bool:
+        changed = False
+        indexer_ids: Dict[str, int] = {
+            indexer["name"]: indexer["id"] for indexer in api_get(secrets, "/api/v3/indexer")
+        }
         for indexer_name, indexer in remote.definitions.items():
             if indexer_name not in self.definitions:
                 indexer_tree = f"{tree}.definitions[{repr(indexer_name)}]"
                 if self.delete_unmanaged:
+                    logger.info("%s: (...) -> (deleted)", indexer_tree)
                     indexer._delete_remote(
-                        tree=indexer_tree,
                         secrets=secrets,
                         indexer_id=indexer_ids[indexer_name],
                     )
                     changed = True
                 else:
                     logger.debug("%s: (...) (unmanaged)", indexer_tree)
-        #
         return changed
```

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/config/media_management.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/config/media_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -535,15 +535,15 @@
                     tree=tree,
                     secrets=secrets,
                     remote=remote,
                     check_unmanaged=check_unmanaged,
                 ),
                 # Root Folders
                 self._update_remote_rootfolder(
-                    tree,
+                    tree=f"{tree}.root_folders",
                     secrets=secrets,
                     remote=remote,
                     check_unmanaged=check_unmanaged,
                 ),
             ],
         )
 
@@ -598,29 +598,44 @@
     def _update_remote_rootfolder(
         self,
         tree: str,
         secrets: SonarrSecrets,
         remote: Self,
         check_unmanaged: bool = False,
     ) -> bool:
-        tree = f"{tree}.root_folders"
         changed = False
         current_root_folders: Dict[str, int] = {
             rf["path"]: rf["id"] for rf in api_get(secrets, "/api/v3/rootfolder")
         }
-        expected_root_folders = set(self.root_folders)
-        if self.delete_unmanaged_root_folders:
-            i = -1
-            for root_folder, root_folder_id in current_root_folders.items():
-                if root_folder not in expected_root_folders:
-                    logger.info("%s[%i]: %s -> (deleted)", tree, i, repr(str(root_folder)))
-                    api_delete(secrets, f"/api/v3/rootfolder/{root_folder_id}")
-                    changed = True
-                    i -= 1
         for i, root_folder in enumerate(self.root_folders):
             if root_folder in current_root_folders:
                 logger.debug("%s[%i]: %s (exists)", tree, i, repr(str(root_folder)))
             else:
                 logger.info("%s[%i]: %s -> (created)", tree, i, repr(str(root_folder)))
                 api_post(secrets, "/api/v3/rootfolder", {"path": str(root_folder)})
                 changed = True
         return changed
+
+    def delete_remote(self, tree: str, secrets: SonarrSecrets, remote: Self) -> bool:
+        return self._update_remote_rootfolder(
+            tree=f"{tree}.root_folders",
+            secrets=secrets,
+            remote=remote,
+        )
+
+    def _delete_remote_rootfolder(self, tree: str, secrets: SonarrSecrets, remote: Self) -> bool:
+        changed = False
+        current_root_folders: Dict[str, int] = {
+            rf["path"]: rf["id"] for rf in api_get(secrets, "/api/v3/rootfolder")
+        }
+        expected_root_folders = set(self.root_folders)
+        i = -1
+        for root_folder, root_folder_id in current_root_folders.items():
+            if root_folder not in expected_root_folders:
+                if self.delete_unmanaged_root_folders:
+                    logger.info("%s[%i]: %s -> (deleted)", tree, i, repr(str(root_folder)))
+                    api_delete(secrets, f"/api/v3/rootfolder/{root_folder_id}")
+                    changed = True
+                else:
+                    logger.info("%s[%i]: %s -> (unmanaged)", tree, i, repr(str(root_folder)))
+                i -= 1
+        return changed
```

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/config/metadata.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/config/metadata.py`

 * *Files identical despite different names*

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/config/profiles/__init__.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/config/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/config/profiles/delay.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/config/profiles/delay.py`

 * *Files identical despite different names*

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/config/profiles/language.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/config/profiles/language.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,16 +300,15 @@
                 secrets,
                 f"/api/v3/languageprofile/{profile_id}",
                 {"id": profile_id, "name": profile_name, **remote_attrs},
             )
             return True
         return False
 
-    def _delete_remote(self, tree: str, secrets: SonarrSecrets, profile_id: int) -> None:
-        logger.info("%s: (...) -> (deleted)", tree)
+    def _delete_remote(self, secrets: SonarrSecrets, profile_id: int) -> None:
         api_delete(secrets, f"/api/v3/languageprofile/{profile_id}")
 
 
 class SonarrLanguageProfilesSettingsConfig(SonarrConfigBase):
     """
     Configuration parameters for controlling how Buildarr handles language profiles.
     """
@@ -344,17 +343,15 @@
     def update_remote(
         self,
         tree: str,
         secrets: SonarrSecrets,
         remote: Self,
         check_unmanaged: bool = False,
     ) -> bool:
-        #
         changed = False
-        #
         profile_ids: Dict[str, int] = {
             profile_json["name"]: profile_json["id"]
             for profile_json in api_get(secrets, "/api/v3/languageprofile")
         }
         language_ids = {
             Language(language["language"]["name"]): language["language"]["id"]
             for language in api_get(secrets, "/api/v3/languageprofile/schema")["languages"]
@@ -367,44 +364,47 @@
         #     }
         # # Compatible with Sonarr V3, deprecated on Sonarr V4
         # except SonarrAPIError as err:
         #     if err.response.status_code == 404:
         #         ...
         #     else:
         #         raise
-        #
         for profile_name, profile in self.definitions.items():
             profile_tree = f"{tree}.definitions[{repr(profile_name)}]"
-            #
             if profile_name not in remote.definitions:
                 profile._create_remote(
                     tree=profile_tree,
                     secrets=secrets,
                     profile_name=profile_name,
                     language_ids=language_ids,
                 )
                 changed = True
-            #
             elif profile._update_remote(
                 tree=profile_tree,
                 secrets=secrets,
                 remote=remote.definitions[profile_name],
                 profile_id=profile_ids[profile_name],
                 profile_name=profile_name,
                 language_ids=language_ids,
             ):
                 changed = True
-        #
+        return changed
+
+    def delete_remote(self, tree: str, secrets: SonarrSecrets, remote: Self) -> bool:
+        changed = False
+        profile_ids: Dict[str, int] = {
+            profile_json["name"]: profile_json["id"]
+            for profile_json in api_get(secrets, "/api/v3/languageprofile")
+        }
         for profile_name, profile in remote.definitions.items():
             if profile_name not in self.definitions:
                 profile_tree = f"{tree}.definitions[{repr(profile_name)}]"
                 if self.delete_unmanaged:
+                    logger.info("%s: (...) -> (deleted)", profile_tree)
                     profile._delete_remote(
-                        tree=profile_tree,
                         secrets=secrets,
                         profile_id=profile_ids[profile_name],
                     )
                     changed = True
                 else:
                     logger.debug("%s: (...) (unmanaged)", profile_tree)
-        #
         return changed
```

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/config/profiles/quality.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/config/profiles/quality.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,16 +320,15 @@
                 secrets,
                 f"/api/v3/qualityprofile/{profile_id}",
                 {"id": profile_id, "name": profile_name, **remote_attrs},
             )
             return True
         return False
 
-    def _delete_remote(self, tree: str, secrets: SonarrSecrets, profile_id: int) -> None:
-        logger.info("%s: (...) -> (deleted)", tree)
+    def _delete_remote(self, secrets: SonarrSecrets, profile_id: int) -> None:
         api_delete(secrets, f"/api/v3/qualityprofile/{profile_id}")
 
 
 class SonarrQualityProfilesSettingsConfig(SonarrConfigBase):
     """
     Configuration parameters for controlling how Buildarr handles quality profiles.
     """
@@ -363,65 +362,66 @@
     def update_remote(
         self,
         tree: str,
         secrets: SonarrSecrets,
         remote: Self,
         check_unmanaged: bool = False,
     ) -> bool:
-        #
         changed = False
-        #
         profile_ids: Dict[str, int] = {
             profile_json["name"]: profile_json["id"]
             for profile_json in api_get(secrets, "/api/v3/qualityprofile")
         }
         quality_definitions: Dict[str, Dict[str, Any]] = {
             quality_json["title"]: quality_json["quality"]
             for quality_json in sorted(
                 api_get(secrets, "/api/v3/qualitydefinition"),
                 key=lambda q: q["weight"],
                 reverse=True,
             )
         }
-        #
         for profile_name, profile in self.definitions.items():
             profile_tree = f"{tree}.definitions[{repr(profile_name)}]"
-            #
             if profile_name not in remote.definitions:
                 profile._create_remote(
                     tree=profile_tree,
                     secrets=secrets,
                     profile_name=profile_name,
                     quality_definitions=quality_definitions,
                 )
                 changed = True
-            #
             elif profile._update_remote(
                 tree=profile_tree,
                 secrets=secrets,
                 remote=remote.definitions[profile_name],
                 profile_id=profile_ids[profile_name],
                 profile_name=profile_name,
                 quality_definitions=quality_definitions,
             ):
                 changed = True
-        #
+        return changed
+
+    def delete_remote(self, tree: str, secrets: SonarrSecrets, remote: Self) -> bool:
+        changed = False
+        profile_ids: Dict[str, int] = {
+            profile_json["name"]: profile_json["id"]
+            for profile_json in api_get(secrets, "/api/v3/qualityprofile")
+        }
         for profile_name, profile in remote.definitions.items():
             if profile_name not in self.definitions:
                 profile_tree = f"{tree}.definitions[{repr(profile_name)}]"
                 if self.delete_unmanaged:
+                    logger.info("%s: (...) -> (deleted)", profile_tree)
                     profile._delete_remote(
-                        tree=profile_tree,
                         secrets=secrets,
                         profile_id=profile_ids[profile_name],
                     )
                     changed = True
                 else:
                     logger.debug("%s: (...) (unmanaged)", profile_tree)
-        #
         return changed
 
 
 def _decode_qualities(value: Sequence[Mapping[str, Any]]) -> List[Union[str, QualityGroup]]:
     return [
         (
             QualityGroup(
```

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/config/profiles/release.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/config/profiles/release.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 
 
 from __future__ import annotations
 
 import json
 
 from logging import getLogger
-from pathlib import Path
 from typing import Any, Dict, Iterable, List, Mapping, Optional, Set, cast
 
 from buildarr.config import ConfigTrashIDNotFoundError, RemoteMapEntry
+from buildarr.state import state
 from buildarr.types import NonEmptyStr, TrashID
 from pydantic import validator
 from typing_extensions import Self
 
 from ...api import api_delete, api_get, api_post, api_put
 from ...secrets import SonarrSecrets
 from ..types import SonarrConfigBase
@@ -116,16 +116,14 @@
     filter: TrashFilter = TrashFilter()
     """
     ###### ::: buildarr_sonarr.config.profiles.release.TrashFilter
         options:
           members:
             - include
             - exclude
-          show_root_heading: false
-          show_source: false
     """
 
     strict_negative_scores: bool = False
     """
     Enables preferred term scores less than 0 to be instead treated
     as "Must Not Contain" (ignored) terms.
 
@@ -250,34 +248,23 @@
         cls,
         indexer_ids: Mapping[str, int],
         tag_ids: Mapping[str, int],
         remote_attrs: Mapping[str, Any],
     ) -> Self:
         return cls(**cls.get_local_attrs(cls._get_remote_map(indexer_ids, tag_ids), remote_attrs))
 
-    @property
     def uses_trash_metadata(self) -> bool:
-        """
-        A flag determining whether or not this configuration uses TRaSH-Guides metadata.
-
-        Returns:
-            `True` if TRaSH-Guides metadata is used, otherwise `False`
-        """
         return bool(self.trash_id)
 
-    def _render_trash_metadata(self, trash_metadata_dir: Path) -> None:
-        """
-        Render configuration attributes obtained from TRaSH-Guides, in-place.
-
-        Args:
-            trash_metadata_dir (Path): TRaSH-Guides metadata directory.
-        """
+    def _render(self) -> None:
         if not self.trash_id:
             return
-        for profile_file in (trash_metadata_dir / "docs" / "json" / "sonarr" / "rp").iterdir():
+        for profile_file in (
+            state.trash_metadata_dir / "docs" / "json" / "sonarr" / "rp"
+        ).iterdir():
             with profile_file.open() as f:
                 profile: Dict[str, Any] = json.load(f)
                 if cast(str, profile["trash_id"]).lower() == self.trash_id:
                     #
                     must_contain: Set[str] = set()
                     must_not_contain: Set[str] = set()
                     preferred: List[PreferredWord] = []
@@ -372,23 +359,17 @@
                 secrets,
                 f"/api/v3/releaseprofile/{profile_id}",
                 {"id": profile_id, "name": profile_name, **remote_attrs},
             )
             return True
         return False
 
-    def _delete_remote(self, tree: str, secrets: SonarrSecrets, profile_id: int) -> None:
-        logger.info("%s: (...) -> (deleted)", tree)
+    def _delete_remote(self, secrets: SonarrSecrets, profile_id: int) -> None:
         api_delete(secrets, f"/api/v3/releaseprofile/{profile_id}")
 
-    # Tell Pydantic to validate in-place assignments of attributes.
-    # This ensures that any validators that parse attributes to consistent values run.
-    class Config(SonarrConfigBase.Config):
-        validate_assignment = True
-
 
 class SonarrReleaseProfilesSettingsConfig(SonarrConfigBase):
     """
     Configuration parameters for controlling how Buildarr handles release profiles.
     """
 
     delete_unmanaged: bool = False
@@ -428,17 +409,15 @@
     def update_remote(
         self,
         tree: str,
         secrets: SonarrSecrets,
         remote: Self,
         check_unmanaged: bool = False,
     ) -> bool:
-        #
         changed = False
-        #
         profile_ids: Dict[str, int] = {
             profile_json["name"]: profile_json["id"]
             for profile_json in api_get(secrets, "/api/v3/releaseprofile")
         }
         indexer_ids: Dict[str, int] = (
             {tag["name"]: tag["id"] for tag in api_get(secrets, "/api/v3/indexer")}
             if any(p.indexer for p in self.definitions.values())
@@ -447,46 +426,49 @@
         )
         tag_ids: Dict[str, int] = (
             {tag["label"]: tag["id"] for tag in api_get(secrets, "/api/v3/tag")}
             if any(profile.tags for profile in self.definitions.values())
             or any(profile.tags for profile in remote.definitions.values())
             else {}
         )
-        #
         for profile_name, profile in self.definitions.items():
             profile_tree = f"{tree}.definitions[{repr(profile_name)}]"
-            #
             if profile_name not in remote.definitions:
                 profile._create_remote(
                     tree=profile_tree,
                     secrets=secrets,
                     profile_name=profile_name,
                     indexer_ids=indexer_ids,
                     tag_ids=tag_ids,
                 )
                 changed = True
-            #
             elif profile._update_remote(
                 tree=profile_tree,
                 secrets=secrets,
                 remote=remote.definitions[profile_name],
                 profile_id=profile_ids[profile_name],
                 profile_name=profile_name,
                 indexer_ids=indexer_ids,
                 tag_ids=tag_ids,
             ):
                 changed = True
-        #
+        return changed
+
+    def delete_remote(self, tree: str, secrets: SonarrSecrets, remote: Self) -> bool:
+        changed = False
+        profile_ids: Dict[str, int] = {
+            profile_json["name"]: profile_json["id"]
+            for profile_json in api_get(secrets, "/api/v3/releaseprofile")
+        }
         for profile_name, profile in remote.definitions.items():
             if profile_name not in self.definitions:
                 profile_tree = f"{tree}.definitions[{repr(profile_name)}]"
                 if self.delete_unmanaged:
+                    logger.info("%s: (...) -> (deleted)", profile_tree)
                     profile._delete_remote(
-                        tree=profile_tree,
                         secrets=secrets,
                         profile_id=profile_ids[profile_name],
                     )
                     changed = True
                 else:
                     logger.debug("%s: (...) (unmanaged)", profile_tree)
-        #
         return changed
```

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/config/quality.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/config/quality.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,19 +17,18 @@
 """
 
 
 from __future__ import annotations
 
 import json
 
-from pathlib import Path
 from typing import Any, Dict, Mapping, Optional, cast
 
-from buildarr.config import ConfigBase
-from buildarr.config.exceptions import ConfigTrashIDNotFoundError
+from buildarr.config import ConfigBase, ConfigTrashIDNotFoundError
+from buildarr.state import state
 from buildarr.types import TrashID
 from pydantic import Field, validator
 from typing_extensions import Self
 
 from ..api import api_get, api_put
 from ..secrets import SonarrSecrets
 from .types import SonarrConfigBase
@@ -148,35 +147,22 @@
     If `trash_id` is set, any values set here will override the default values provided
     from the TRaSH-Guides quality definition profile.
 
     If `trash_id` is not set, only explicitly defined quality definitions are managed,
     and quality definitions not set within Buildarr are left unmodified.
     """
 
-    @property
     def uses_trash_metadata(self) -> bool:
-        """
-        A flag determining whether or not this configuration uses TRaSH-Guides metadata.
-
-        Returns:
-            `True` if TRaSH-Guides metadata is used, otherwise `False`
-        """
         return bool(self.trash_id)
 
-    def _render_trash_metadata(self, trash_metadata_dir: Path) -> None:
-        """
-        Render configuration attributes obtained from TRaSH-Guides, in-place.
-
-        Args:
-            trash_metadata_dir (Path): TRaSH-Guides metadata directory.
-        """
+    def _render(self) -> None:
         if not self.trash_id:
             return
         for quality_file in (
-            trash_metadata_dir / "docs" / "json" / "sonarr" / "quality-size"
+            state.trash_metadata_dir / "docs" / "json" / "sonarr" / "quality-size"
         ).iterdir():
             with quality_file.open() as f:
                 quality_json = json.load(f)
                 if cast(str, quality_json["trash_id"]).lower() == self.trash_id:
                     for definition_json in quality_json["qualities"]:
                         definition_name = definition_json["quality"]
                         if definition_name not in self.definitions:
@@ -238,12 +224,7 @@
                 api_put(
                     secrets,
                     f"/api/v3/qualitydefinition/{definition_id}",
                     {**remote_definitions_json[definition_id], **remote_attrs},
                 )
                 changed = True
         return changed
-
-    # Tell Pydantic to validate in-place assignments of attributes.
-    # This ensures that any validators that parse attributes to consistent values run.
-    class Config(SonarrConfigBase.Config):
-        validate_assignment = True
```

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/config/tags.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/config/tags.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,25 +45,14 @@
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
-    unused by Sonarr, so be careful about when to use this option.
-
-    Sonarr appears to periodically clean up unused tags,
-    so in most cases there is no need to enable this option.
-    """
-
     definitions: List[NonEmptyStr] = []
     """
     Define tags that are used within Buildarr here.
 
     If they are not defined here, you may get errors resulting from non-existent
     tags from either Buildarr or Sonarr.
     """
@@ -77,17 +66,15 @@
     def update_remote(
         self,
         tree: str,
         secrets: SonarrSecrets,
         remote: Self,
         check_unmanaged: bool = False,
     ) -> bool:
-        # This only does creations and updates.
-        # Deletes (and empty tag list prints) are done AFTER all other modifications are made.
-        # TODO: Implement tag deletions.
+        # This only does creations and updates, as Sonarr automatically cleans up unused tags.
         changed = False
         current_tags: Dict[str, int] = {
             tag["label"]: tag["id"] for tag in api_get(secrets, "/api/v3/tag")
         }
         if self.definitions:
             for i, tag in enumerate(self.definitions):
                 if tag in current_tags:
```

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/config/types.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/config/types.py`

 * *Files identical despite different names*

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/config/ui.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/config/ui.py`

 * *Files identical despite different names*

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/config/util.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/config/util.py`

 * *Files identical despite different names*

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/exceptions.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,37 +9,21 @@
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with Buildarr.
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
-Sonarr plugin exception classes.
+Sonarr plugin manager class.
 """
 
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from buildarr.manager import ManagerPlugin
 
-from buildarr.exceptions import BuildarrError
+from .config import SonarrInstanceConfig
+from .secrets import SonarrSecrets
 
-if TYPE_CHECKING:
-    from requests import Response
-
-
-class SonarrError(BuildarrError):
-    """
-    Sonarr plugin exception base class.
-    """
 
+class SonarrManager(ManagerPlugin[SonarrInstanceConfig, SonarrSecrets]):
     pass
-
-
-class SonarrAPIError(SonarrError):
-    """
-    Sonarr API exception class.
-    """
-
-    def __init__(self, msg: str, response: Response) -> None:
-        self.response = response
-        super().__init__(msg)
```

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/manager.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,21 +9,32 @@
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with Buildarr.
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
-Sonarr plugin manager class.
+Sonarr plugin interface.
 """
 
 
 from __future__ import annotations
 
-from buildarr.manager import ManagerPlugin
+from buildarr.plugins import Plugin
 
-from .config import SonarrInstanceConfig
+from . import __version__
+from .cli import sonarr
+from .config import SonarrConfig
+from .manager import SonarrManager
 from .secrets import SonarrSecrets
 
 
-class SonarrManager(ManagerPlugin[SonarrInstanceConfig, SonarrSecrets]):
-    pass
+class SonarrPlugin(Plugin):
+    """
+    Sonarr plugin class that Buildarr reads to process Sonarr instances.
+    """
+
+    cli = sonarr
+    config = SonarrConfig
+    manager = SonarrManager
+    secrets = SonarrSecrets
+    version = __version__
```

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/secrets.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/secrets.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from typing import TYPE_CHECKING
 from urllib.parse import urlparse
 
 from buildarr.secrets import SecretsPlugin
 from buildarr.types import NonEmptyStr, Port
 
 from .api import api_get, get_initialize_js
-from .exceptions import SonarrAPIError
+from .exceptions import SonarrAPIError, SonarrSecretsUnauthorizedError
 from .types import SonarrApiKey, SonarrProtocol
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
     from .config import SonarrConfig
 
@@ -69,25 +69,39 @@
             if len(hostname_port) > 1
             else (443 if protocol == "https" else 80)
         )
         return cls(hostname=hostname, port=port, protocol=protocol, api_key=api_key)
 
     @classmethod
     def get(cls, config: SonarrConfig) -> Self:
-        return cls(
-            hostname=config.hostname,
-            port=config.port,
-            protocol=config.protocol,
-            api_key=(
-                config.api_key if config.api_key else get_initialize_js(config.host_url)["apiKey"]
-            ),
-        )
+        try:
+            return cls(
+                hostname=config.hostname,
+                port=config.port,
+                protocol=config.protocol,
+                api_key=(
+                    config.api_key
+                    if config.api_key
+                    else get_initialize_js(config.host_url)["apiKey"]
+                ),
+            )
+        except SonarrAPIError as err:
+            if err.status_code == HTTPStatus.UNAUTHORIZED:
+                raise SonarrSecretsUnauthorizedError(
+                    "Unable to retrieve the API key for the Sonarr instance "
+                    f"at '{config.host_url}': Authentication is enabled. "
+                    "Please set the 'Settings -> General -> Authentication' attribute to 'None', "
+                    "or if you do not wish to disable authentication, "
+                    "explicitly define the API key in the Buildarr configuration.",
+                ) from None
+            else:
+                raise
 
     def test(self) -> bool:
         try:
             api_get(self, "/api/v3/system/status")
             return True
         except SonarrAPIError as err:
-            if err.response.status_code == HTTPStatus.UNAUTHORIZED:
+            if err.status_code == HTTPStatus.UNAUTHORIZED:
                 return False
             else:
                 raise
```

### Comparing `buildarr_sonarr-0.4.1/buildarr_sonarr/types.py` & `buildarr_sonarr-0.5.0/buildarr_sonarr/types.py`

 * *Files identical despite different names*

### Comparing `buildarr_sonarr-0.4.1/pyproject.toml` & `buildarr_sonarr-0.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.3.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "buildarr-sonarr"
-version = "0.4.1"
+version = "0.5.0"
 description = "Sonarr PVR plugin for Buildarr"
 authors = ["Callum Dickinson <callum.dickinson.nz@gmail.com>"]
 license = "GPL-3.0-or-later"
 homepage = "https://buildarr.github.io/plugins/sonarr"
 repository = "https://github.com/buildarr/buildarr-sonarr"
 documentation = "https://buildarr.github.io/plugins/sonarr"
 keywords = ["buildarr", "sonarr"]
@@ -28,24 +28,23 @@
 packages = [{include = "buildarr_sonarr"}]
 
 [tool.poetry.plugins."buildarr.plugins"]
 "sonarr" = "buildarr_sonarr.plugin:SonarrPlugin"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
-buildarr = ">=0.4.0,<0.5.0"
+buildarr = ">=0.5.0,<0.6.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "23.1.0"
-mypy = "1.1.1"
-types-pyyaml = "6.0.12.8"
-types-requests = "2.28.11.15"
+black = "23.3.0"
+mypy = "1.2.0"
+types-requests = "2.28.11.17"
 mkdocs = "1.4.2"
-mkdocstrings = {extras = ["python"], version = "0.20.0"}
-ruff = "0.0.255"
+mkdocstrings = {extras = ["python"], version = "0.21.2"}
+ruff = "0.0.261"
 
 [tool.ruff]
 fix = true
 format = "grouped"
 target-version = "py38"
 line-length = 100
 select = [
```

### Comparing `buildarr_sonarr-0.4.1/PKG-INFO` & `buildarr_sonarr-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildarr-sonarr
-Version: 0.4.1
+Version: 0.5.0
 Summary: Sonarr PVR plugin for Buildarr
 Home-page: https://buildarr.github.io/plugins/sonarr
 License: GPL-3.0-or-later
 Keywords: buildarr,sonarr
 Author: Callum Dickinson
 Author-email: callum.dickinson.nz@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Systems Administration
 Classifier: Typing :: Typed
-Requires-Dist: buildarr (>=0.4.0,<0.5.0)
+Requires-Dist: buildarr (>=0.5.0,<0.6.0)
 Project-URL: Documentation, https://buildarr.github.io/plugins/sonarr
 Project-URL: Repository, https://github.com/buildarr/buildarr-sonarr
 Description-Content-Type: text/markdown
 
 # Buildarr Sonarr Plugin
 
 [![PyPI](https://img.shields.io/pypi/v/buildarr-sonarr)](https://pypi.org/project/buildarr-sonarr) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/buildarr-sonarr)  [![GitHub](https://img.shields.io/github/license/buildarr/buildarr-sonarr)](https://github.com/buildarr/buildarr-sonarr/blob/main/LICENSE) ![Pre-commit hooks](https://github.com/buildarr/buildarr-sonarr/actions/workflows/pre-commit.yml/badge.svg) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

