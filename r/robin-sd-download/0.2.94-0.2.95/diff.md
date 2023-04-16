# Comparing `tmp/robin_sd_download-0.2.94.tar.gz` & `tmp/robin_sd_download-0.2.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/robin_sd_download-0.2.94.tar", last modified: Thu Apr  6 13:14:08 2023, max compression
+gzip compressed data, was "dist/robin_sd_download-0.2.95.tar", last modified: Sun Apr 16 09:07:45 2023, max compression
```

## Comparing `robin_sd_download-0.2.94.tar` & `robin_sd_download-0.2.95.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 13:14:08.000000 robin_sd_download-0.2.94/
--rw-r--r--   0 root         (0) root         (0)      650 2023-04-06 13:14:08.000000 robin_sd_download-0.2.94/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-04-06 13:13:54.000000 robin_sd_download-0.2.94/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 13:14:08.000000 robin_sd_download-0.2.94/robin_sd_download/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-06 13:13:54.000000 robin_sd_download-0.2.94/robin_sd_download/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-04-06 13:13:54.000000 robin_sd_download-0.2.94/robin_sd_download/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-04-06 13:13:54.000000 robin_sd_download-0.2.94/robin_sd_download/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 13:14:08.000000 robin_sd_download-0.2.94/robin_sd_download/api_interaction/
--rw-rw-rw-   0 root         (0) root         (0)       48 2023-04-06 13:13:54.000000 robin_sd_download-0.2.94/robin_sd_download/api_interaction/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1722 2023-04-06 13:13:54.000000 robin_sd_download-0.2.94/robin_sd_download/api_interaction/get_bearer_token.py
--rw-rw-rw-   0 root         (0) root         (0)     4907 2023-04-06 13:13:54.000000 robin_sd_download-0.2.94/robin_sd_download/api_interaction/get_software.py
--rw-rw-rw-   0 root         (0) root         (0)     4729 2023-04-06 13:13:54.000000 robin_sd_download-0.2.94/robin_sd_download/api_interaction/get_software_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 13:14:08.000000 robin_sd_download-0.2.94/robin_sd_download/apt_interaction/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-06 13:13:54.000000 robin_sd_download-0.2.94/robin_sd_download/apt_interaction/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1895 2023-04-06 13:13:54.000000 robin_sd_download-0.2.94/robin_sd_download/apt_interaction/ensure_hook.py
--rw-rw-rw-   0 root         (0) root         (0)     3851 2023-04-06 13:13:54.000000 robin_sd_download-0.2.94/robin_sd_download/apt_interaction/ensure_local_repo.py
--rw-rw-rw-   0 root         (0) root         (0)    15269 2023-04-06 13:13:54.000000 robin_sd_download-0.2.94/robin_sd_download/apt_interaction/offline_install.py
--rw-rw-rw-   0 root         (0) root         (0)     4768 2023-04-06 13:13:54.000000 robin_sd_download-0.2.94/robin_sd_download/apt_interaction/prepare_install.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 13:14:08.000000 robin_sd_download-0.2.94/robin_sd_download/slack_interaction/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-06 13:13:54.000000 robin_sd_download-0.2.94/robin_sd_download/slack_interaction/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2952 2023-04-06 13:13:54.000000 robin_sd_download-0.2.94/robin_sd_download/slack_interaction/slack_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 13:14:08.000000 robin_sd_download-0.2.94/robin_sd_download/supportive_scripts/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-06 13:13:54.000000 robin_sd_download-0.2.94/robin_sd_download/supportive_scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3426 2023-04-06 13:13:54.000000 robin_sd_download-0.2.94/robin_sd_download/supportive_scripts/arg_parse.py
--rw-rw-rw-   0 root         (0) root         (0)     2126 2023-04-06 13:13:54.000000 robin_sd_download-0.2.94/robin_sd_download/supportive_scripts/logger.py
--rw-rw-rw-   0 root         (0) root         (0)     1574 2023-04-06 13:13:54.000000 robin_sd_download-0.2.94/robin_sd_download/supportive_scripts/sudo_file.py
--rw-rw-rw-   0 root         (0) root         (0)     1396 2023-04-06 13:13:54.000000 robin_sd_download-0.2.94/robin_sd_download/supportive_scripts/version_checker.py
--rw-rw-rw-   0 root         (0) root         (0)     3537 2023-04-06 13:13:54.000000 robin_sd_download-0.2.94/robin_sd_download/supportive_scripts/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 13:14:08.000000 robin_sd_download-0.2.94/robin_sd_download.egg-info/
--rw-r--r--   0 root         (0) root         (0)      650 2023-04-06 13:14:08.000000 robin_sd_download-0.2.94/robin_sd_download.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1254 2023-04-06 13:14:08.000000 robin_sd_download-0.2.94/robin_sd_download.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 13:14:08.000000 robin_sd_download-0.2.94/robin_sd_download.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-04-06 13:14:08.000000 robin_sd_download-0.2.94/robin_sd_download.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-04-06 13:14:08.000000 robin_sd_download-0.2.94/robin_sd_download.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-06 13:14:08.000000 robin_sd_download-0.2.94/robin_sd_download.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-06 13:14:08.000000 robin_sd_download-0.2.94/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-04-06 13:13:54.000000 robin_sd_download-0.2.94/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 13:14:08.000000 robin_sd_download-0.2.94/tests/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-06 13:13:54.000000 robin_sd_download-0.2.94/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3747 2023-04-06 13:13:54.000000 robin_sd_download-0.2.94/tests/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:07:45.000000 robin_sd_download-0.2.95/
+-rw-r--r--   0 root         (0) root         (0)      650 2023-04-16 09:07:45.000000 robin_sd_download-0.2.95/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-04-16 09:07:27.000000 robin_sd_download-0.2.95/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:07:45.000000 robin_sd_download-0.2.95/robin_sd_download/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-16 09:07:27.000000 robin_sd_download-0.2.95/robin_sd_download/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-04-16 09:07:27.000000 robin_sd_download-0.2.95/robin_sd_download/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-04-16 09:07:27.000000 robin_sd_download-0.2.95/robin_sd_download/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:07:45.000000 robin_sd_download-0.2.95/robin_sd_download/api_interaction/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2023-04-16 09:07:27.000000 robin_sd_download-0.2.95/robin_sd_download/api_interaction/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1722 2023-04-16 09:07:27.000000 robin_sd_download-0.2.95/robin_sd_download/api_interaction/get_bearer_token.py
+-rw-rw-rw-   0 root         (0) root         (0)     5452 2023-04-16 09:07:27.000000 robin_sd_download-0.2.95/robin_sd_download/api_interaction/get_software.py
+-rw-rw-rw-   0 root         (0) root         (0)     4729 2023-04-16 09:07:27.000000 robin_sd_download-0.2.95/robin_sd_download/api_interaction/get_software_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:07:45.000000 robin_sd_download-0.2.95/robin_sd_download/apt_interaction/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-16 09:07:27.000000 robin_sd_download-0.2.95/robin_sd_download/apt_interaction/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1895 2023-04-16 09:07:27.000000 robin_sd_download-0.2.95/robin_sd_download/apt_interaction/ensure_hook.py
+-rw-rw-rw-   0 root         (0) root         (0)     3851 2023-04-16 09:07:27.000000 robin_sd_download-0.2.95/robin_sd_download/apt_interaction/ensure_local_repo.py
+-rw-rw-rw-   0 root         (0) root         (0)    15269 2023-04-16 09:07:27.000000 robin_sd_download-0.2.95/robin_sd_download/apt_interaction/offline_install.py
+-rw-rw-rw-   0 root         (0) root         (0)     4768 2023-04-16 09:07:27.000000 robin_sd_download-0.2.95/robin_sd_download/apt_interaction/prepare_install.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:07:45.000000 robin_sd_download-0.2.95/robin_sd_download/slack_interaction/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-16 09:07:27.000000 robin_sd_download-0.2.95/robin_sd_download/slack_interaction/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2952 2023-04-16 09:07:27.000000 robin_sd_download-0.2.95/robin_sd_download/slack_interaction/slack_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:07:45.000000 robin_sd_download-0.2.95/robin_sd_download/supportive_scripts/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-16 09:07:27.000000 robin_sd_download-0.2.95/robin_sd_download/supportive_scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3426 2023-04-16 09:07:27.000000 robin_sd_download-0.2.95/robin_sd_download/supportive_scripts/arg_parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     2220 2023-04-16 09:07:27.000000 robin_sd_download-0.2.95/robin_sd_download/supportive_scripts/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1574 2023-04-16 09:07:27.000000 robin_sd_download-0.2.95/robin_sd_download/supportive_scripts/sudo_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2023-04-16 09:07:27.000000 robin_sd_download-0.2.95/robin_sd_download/supportive_scripts/version_checker.py
+-rw-rw-rw-   0 root         (0) root         (0)     3537 2023-04-16 09:07:27.000000 robin_sd_download-0.2.95/robin_sd_download/supportive_scripts/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:07:45.000000 robin_sd_download-0.2.95/robin_sd_download.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      650 2023-04-16 09:07:45.000000 robin_sd_download-0.2.95/robin_sd_download.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1254 2023-04-16 09:07:45.000000 robin_sd_download-0.2.95/robin_sd_download.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 09:07:45.000000 robin_sd_download-0.2.95/robin_sd_download.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-04-16 09:07:45.000000 robin_sd_download-0.2.95/robin_sd_download.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-04-16 09:07:45.000000 robin_sd_download-0.2.95/robin_sd_download.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-16 09:07:45.000000 robin_sd_download-0.2.95/robin_sd_download.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 09:07:45.000000 robin_sd_download-0.2.95/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-04-16 09:07:27.000000 robin_sd_download-0.2.95/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:07:45.000000 robin_sd_download-0.2.95/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-16 09:07:27.000000 robin_sd_download-0.2.95/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3747 2023-04-16 09:07:27.000000 robin_sd_download-0.2.95/tests/test.py
```

### Comparing `robin_sd_download-0.2.94/PKG-INFO` & `robin_sd_download-0.2.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robin_sd_download
-Version: 0.2.94
+Version: 0.2.95
 Summary: Package to download files to the Robin Radar API
 Home-page: https://bitbucket.org/robin-radar-systems/sd-api-download-pip-package.git
 Author: Robin Radar Systems
 Author-email: it-team@robinradar.com
 License: MIT
 Description: # robin-sd-download
```

### Comparing `robin_sd_download-0.2.94/robin_sd_download/api_interaction/get_bearer_token.py` & `robin_sd_download-0.2.95/robin_sd_download/api_interaction/get_bearer_token.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.2.94/robin_sd_download/api_interaction/get_software.py` & `robin_sd_download-0.2.95/robin_sd_download/api_interaction/get_software.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 # -*- coding: utf-8 -*-
 
 import requests
 import os
 import zipfile
 import datetime
 import glob
+import re
 
 from robin_sd_download.api_interaction import get_bearer_token
 from robin_sd_download.supportive_scripts import yaml_parser
 from robin_sd_download.supportive_scripts import logger
 
-import itertools
-from contextlib import closing
-
 
 def generate_response_content(response, chunk_size=8192):
     try:
         for chunk in response.iter_content(chunk_size=chunk_size):
             if chunk:
                 yield chunk
     except KeyboardInterrupt:
@@ -52,95 +50,118 @@
         while len(backup_files) > 3:
             oldest_file = backup_files.pop()
             os.remove(oldest_file)
             logger.log(
                 message=f"Removed old backup: {oldest_file}", log_level="info", to_terminal=True)
 
 
+def extract_version(file_name):
+    version_pattern = re.compile(r'\d+\.\d+\.\d+')
+    match = version_pattern.search(file_name)
+
+    if match:
+        return match.group(0)
+    else:
+        return None
+
+
+def get_local_version(file_location):
+    local_software_files = glob.glob(os.path.join(file_location, "*"))
+    local_software_files.sort(key=os.path.getctime, reverse=True)
+
+    if local_software_files:
+        return extract_version(local_software_files[0])
+    else:
+        return None
+
+
+def get_server_version(response):
+    file_name = response.headers.get("Content-Disposition").split("=")[1]
+    file_name = file_name.replace('"', '').replace('.zip', '')
+    return extract_version(file_name), file_name
+
+
+def download_file(response, file_location, file_name):
+    write_file = os.path.join(file_location, f"{file_name}.zip")
+
+    with open(write_file, 'wb') as f:
+        try:
+            for chunk in generate_response_content(response, chunk_size=8192):
+                f.write(chunk)
+        except KeyboardInterrupt:
+            logger.log(
+                message="Download interrupted by user, cleaning up...",
+                log_level="warning", to_terminal=True)
+            f.close()
+            os.remove(write_file)
+            return 1
+
+    logger.log(message="Downloaded to " + write_file,
+               log_level="info", to_terminal=True)
+
+    return write_file
+
+
+def extract_and_cleanup(file_location, file_name, write_file):
+    extracted_folder_path = os.path.join(file_location, f"{file_name}")
+
+    try:
+        create_backup_if_exists(extracted_folder_path)
+
+        with zipfile.ZipFile(write_file, "r") as zip_ref:
+            zip_ref.extractall(extracted_folder_path)
+    except zipfile.BadZipFile:
+        logger.log(message="The downloaded file is not a valid zip file",
+                   log_level="error", to_terminal=True)
+        return 1
+
+    os.remove(write_file)
+    return 0
+
+
 def get_software():
     config = yaml_parser.parse_config()
-
     radar_id = config['radar_id']
     request_url = config['api_url']
+    file_location = config['static']['download_location']
 
-    # current_date = datetime.datetime.now().strftime("%d%m%Y%H%M%S")
-
+    # Get bearer_token
     try:
         bearer_token = str(get_bearer_token.get_bearer_token())
-    except KeyboardInterrupt:
-        logger.log(
-            message="Aborted by user.", log_level="error", to_terminal=True)
-        return 1
     except Exception as e:
-
         logger.log(
             message=f"Failed to get bearer token: {str(e)}", log_level="error", to_terminal=True)
         return 1
 
     headers = {
         'Content-Type': 'application/json',
         'Authorization': 'Bearer ' + bearer_token,
     }
 
     api_endpoint = '/api/radars/' + radar_id + '/software'
 
+    # Get server response
     try:
         response = requests.get(
             request_url + api_endpoint, allow_redirects=True, headers=headers, stream=True)
         response.raise_for_status()
     except requests.exceptions.HTTPError as e:
         logger.log(
             message=f"Failed to get software: {str(e)}", log_level="error", to_terminal=True)
         return 1
 
-    # Get the name of the file
-    file_name = response.headers.get("Content-Disposition").split("=")[1]
-    file_name = file_name.replace('"', '')
-    file_name = file_name.replace('.zip', '')
-
-    # Define the location to save the file
-    file_location = config['static']['download_location']
+    server_version, file_name = get_server_version(response)
+    local_version = get_local_version(file_location)
 
-    try:
-        # Create the destination folder
-        os.makedirs(file_location, exist_ok=True)
-
-        # Write the file to disk
-        write_file = os.path.join(
-            file_location, f"{file_name}.zip")
-
-        with open(write_file, 'wb') as f:
-            try:
-                for chunk in generate_response_content(response, chunk_size=8192):
-                    f.write(chunk)
-            except KeyboardInterrupt:
-                logger.log(
-                    message="Download interrupted by user, cleaning up...",
-                    log_level="warning", to_terminal=True)
-                f.close()
-                os.remove(write_file)
-                return 1
-
-        logger.log(message="Downloaded to " + write_file,
-                   log_level="info", to_terminal=True)
-
-        # Extract the file
-        try:
-            extracted_folder_path = os.path.join(file_location, f"{file_name}")
-            create_backup_if_exists(extracted_folder_path)
-
-            with zipfile.ZipFile(write_file, "r") as zip_ref:
-                zip_ref.extractall(extracted_folder_path)
-        except zipfile.BadZipFile:
-            logger.log(message="The downloaded file is not a valid zip file",
-                       log_level="error", to_terminal=True)
-            return 1
+    if server_version and local_version and server_version == local_version:
+        logger.log(
+            message="The latest software version is already present. Skipping download.",
+            log_level="info", to_terminal=True)
+        return 0
 
-        # Remove the zip file
-        os.remove(write_file)
+    os.makedirs(file_location, exist_ok=True)
 
-    except Exception as e:
-        logger.log(
-            message=f"Failed to download software: {str(e)}", log_level="error", to_terminal=True)
+    write_file = download_file(response, file_location, file_name)
+    if write_file == 1:
         return 1
 
-    return 0
+    return extract_and_cleanup(file_location, file_name, write_file)
```

### Comparing `robin_sd_download-0.2.94/robin_sd_download/api_interaction/get_software_info.py` & `robin_sd_download-0.2.95/robin_sd_download/api_interaction/get_software_info.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.2.94/robin_sd_download/apt_interaction/ensure_hook.py` & `robin_sd_download-0.2.95/robin_sd_download/apt_interaction/ensure_hook.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.2.94/robin_sd_download/apt_interaction/ensure_local_repo.py` & `robin_sd_download-0.2.95/robin_sd_download/apt_interaction/ensure_local_repo.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.2.94/robin_sd_download/apt_interaction/offline_install.py` & `robin_sd_download-0.2.95/robin_sd_download/apt_interaction/offline_install.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.2.94/robin_sd_download/apt_interaction/prepare_install.py` & `robin_sd_download-0.2.95/robin_sd_download/apt_interaction/prepare_install.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.2.94/robin_sd_download/slack_interaction/slack_handler.py` & `robin_sd_download-0.2.95/robin_sd_download/slack_interaction/slack_handler.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.2.94/robin_sd_download/supportive_scripts/arg_parse.py` & `robin_sd_download-0.2.95/robin_sd_download/supportive_scripts/arg_parse.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.2.94/robin_sd_download/supportive_scripts/logger.py` & `robin_sd_download-0.2.95/robin_sd_download/supportive_scripts/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,16 +16,19 @@
 log_dir = os.path.dirname(log_file)
 
 # Check if log_file or app_name is exist in config
 if log_file is None or app_name is None:
     raise Exception("log_file or app_name is not defined in config")
 
 # Create the log directory if it doesn't exist
-if not os.path.exists(log_dir):
-    os.makedirs(log_dir)
+try:
+    if not os.path.exists(log_dir):
+        os.makedirs(log_dir)
+except OSError as e:
+    raise Exception(f"Could not create log directory: {e}")
 
 # Set up logging
 amsterdam_tz = datetime.timezone(datetime.timedelta(hours=1), 'CET')
 logging.basicConfig(level=logging.DEBUG,
                     format='%(asctime)s - %(levelname)s - %(message)s',
                     datefmt='%Y-%m-%d %H:%M:%S %z',
                     filename=log_file,
```

### Comparing `robin_sd_download-0.2.94/robin_sd_download/supportive_scripts/sudo_file.py` & `robin_sd_download-0.2.95/robin_sd_download/supportive_scripts/sudo_file.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.2.94/robin_sd_download/supportive_scripts/version_checker.py` & `robin_sd_download-0.2.95/robin_sd_download/supportive_scripts/version_checker.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.2.94/robin_sd_download/supportive_scripts/yaml_parser.py` & `robin_sd_download-0.2.95/robin_sd_download/supportive_scripts/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.2.94/robin_sd_download.egg-info/PKG-INFO` & `robin_sd_download-0.2.95/robin_sd_download.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robin-sd-download
-Version: 0.2.94
+Version: 0.2.95
 Summary: Package to download files to the Robin Radar API
 Home-page: https://bitbucket.org/robin-radar-systems/sd-api-download-pip-package.git
 Author: Robin Radar Systems
 Author-email: it-team@robinradar.com
 License: MIT
 Description: # robin-sd-download
```

### Comparing `robin_sd_download-0.2.94/robin_sd_download.egg-info/SOURCES.txt` & `robin_sd_download-0.2.95/robin_sd_download.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.2.94/setup.py` & `robin_sd_download-0.2.95/setup.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.2.94/tests/test.py` & `robin_sd_download-0.2.95/tests/test.py`

 * *Files identical despite different names*

