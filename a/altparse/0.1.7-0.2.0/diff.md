# Comparing `tmp/altparse-0.1.7.tar.gz` & `tmp/altparse-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altparse-0.1.7.tar", last modified: Thu Mar 30 03:32:54 2023, max compression
+gzip compressed data, was "altparse-0.2.0.tar", last modified: Sun Apr 16 00:48:49 2023, max compression
```

## Comparing `altparse-0.1.7.tar` & `altparse-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 03:32:54.945007 altparse-0.1.7/
--rw-rw-rw-   0        0        0       66 2022-05-23 21:26:59.000000 altparse-0.1.7/.gitattributes
--rw-rw-rw-   0        0        0     1447 2022-06-03 19:24:20.000000 altparse-0.1.7/.gitignore
--rw-rw-rw-   0        0        0        0 2022-11-30 22:58:46.000000 altparse-0.1.7/CHANGES.md
--rw-rw-rw-   0        0        0     1086 2022-05-23 21:26:59.000000 altparse-0.1.7/LICENSE.txt
--rw-rw-rw-   0        0        0        0 2022-11-30 22:59:45.000000 altparse-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2429 2023-03-30 03:32:54.944008 altparse-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-02-26 04:17:54.000000 altparse-0.1.7/README.md
--rw-rw-rw-   0        0        0     1018 2023-03-30 03:32:29.000000 altparse-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-30 03:32:54.945007 altparse-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0       71 2022-12-01 01:01:54.000000 altparse-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-30 03:32:54.872508 altparse-0.1.7/src/
-drwxrwxrwx   0        0        0        0 2023-03-30 03:32:54.898006 altparse-0.1.7/src/altparse/
--rw-rw-rw-   0        0        0      155 2022-12-06 02:28:59.000000 altparse-0.1.7/src/altparse/__init__.py
--rw-rw-rw-   0        0        0    12655 2023-03-30 03:02:15.000000 altparse-0.1.7/src/altparse/core.py
--rw-rw-rw-   0        0        0      615 2023-03-28 23:48:04.000000 altparse-0.1.7/src/altparse/errors.py
--rw-rw-rw-   0        0        0     3101 2022-12-06 07:19:15.000000 altparse-0.1.7/src/altparse/helpers.py
-drwxrwxrwx   0        0        0        0 2023-03-30 03:32:54.931007 altparse-0.1.7/src/altparse/ipautil/
--rw-rw-rw-   0        0        0      156 2022-12-06 07:29:32.000000 altparse-0.1.7/src/altparse/ipautil/__init__.py
--rw-rw-rw-   0        0        0     3345 2022-12-06 07:29:06.000000 altparse-0.1.7/src/altparse/ipautil/core.py
--rw-rw-rw-   0        0        0      603 2022-12-06 07:12:17.000000 altparse-0.1.7/src/altparse/ipautil/errors.py
--rw-rw-rw-   0        0        0     4519 2022-12-06 07:28:58.000000 altparse-0.1.7/src/altparse/ipautil/helpers.py
--rw-rw-rw-   0        0        0     4051 2022-12-06 07:28:01.000000 altparse-0.1.7/src/altparse/ipautil/model.py
--rw-rw-rw-   0        0        0    26925 2023-03-30 01:29:08.000000 altparse-0.1.7/src/altparse/model.py
--rw-rw-rw-   0        0        0    14145 2023-02-26 04:13:40.000000 altparse-0.1.7/src/altparse/parsers.py
-drwxrwxrwx   0        0        0        0 2023-03-30 03:32:54.922504 altparse-0.1.7/src/altparse.egg-info/
--rw-rw-rw-   0        0        0     2429 2023-03-30 03:32:54.000000 altparse-0.1.7/src/altparse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      720 2023-03-30 03:32:54.000000 altparse-0.1.7/src/altparse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 03:32:54.000000 altparse-0.1.7/src/altparse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-03-30 03:32:54.000000 altparse-0.1.7/src/altparse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-30 03:32:54.000000 altparse-0.1.7/src/altparse.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-30 03:32:54.942508 altparse-0.1.7/tests/
--rw-rw-rw-   0        0        0   357189 2022-12-06 04:50:45.000000 altparse-0.1.7/tests/XPatcher_2.2.ipa
--rw-rw-rw-   0        0        0        1 2022-12-01 07:44:32.000000 altparse-0.1.7/tests/__init__.py
--rw-rw-rw-   0        0        0      987 2022-12-06 07:11:28.000000 altparse-0.1.7/tests/example_ipa_upload.py
--rw-rw-rw-   0        0        0     6175 2023-01-06 17:13:00.000000 altparse-0.1.7/tests/example_update.py
--rw-rw-rw-   0        0        0   210229 2023-01-06 17:51:30.000000 altparse-0.1.7/tests/quantumsource.json
--rw-rw-rw-   0        0        0      623 2022-12-06 07:31:59.000000 altparse-0.1.7/tests/test_create_altsource_obj.py
+drwxrwxrwx   0        0        0        0 2023-04-16 00:48:49.798894 altparse-0.2.0/
+-rw-rw-rw-   0        0        0       66 2022-05-23 21:26:59.000000 altparse-0.2.0/.gitattributes
+-rw-rw-rw-   0        0        0     1447 2022-06-03 19:24:20.000000 altparse-0.2.0/.gitignore
+-rw-rw-rw-   0        0        0        0 2022-11-30 22:58:46.000000 altparse-0.2.0/CHANGES.md
+-rw-rw-rw-   0        0        0     1086 2022-05-23 21:26:59.000000 altparse-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0        0 2022-11-30 22:59:45.000000 altparse-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2429 2023-04-16 00:48:49.798392 altparse-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-02-26 04:17:54.000000 altparse-0.2.0/README.md
+-rw-rw-rw-   0        0        0     1018 2023-04-16 00:48:22.000000 altparse-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 00:48:49.798894 altparse-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0       71 2022-12-01 01:01:54.000000 altparse-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 00:48:49.548035 altparse-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 00:48:49.664393 altparse-0.2.0/src/altparse/
+-rw-rw-rw-   0        0        0      155 2022-12-06 02:28:59.000000 altparse-0.2.0/src/altparse/__init__.py
+-rw-rw-rw-   0        0        0    13592 2023-04-16 00:40:47.000000 altparse-0.2.0/src/altparse/core.py
+-rw-rw-rw-   0        0        0      615 2023-03-28 23:48:04.000000 altparse-0.2.0/src/altparse/errors.py
+-rw-rw-rw-   0        0        0     3101 2022-12-06 07:19:15.000000 altparse-0.2.0/src/altparse/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-16 00:48:49.728892 altparse-0.2.0/src/altparse/ipautil/
+-rw-rw-rw-   0        0        0      156 2022-12-06 07:29:32.000000 altparse-0.2.0/src/altparse/ipautil/__init__.py
+-rw-rw-rw-   0        0        0     3493 2023-04-15 22:08:19.000000 altparse-0.2.0/src/altparse/ipautil/core.py
+-rw-rw-rw-   0        0        0      603 2022-12-06 07:12:17.000000 altparse-0.2.0/src/altparse/ipautil/errors.py
+-rw-rw-rw-   0        0        0     4857 2023-04-15 19:21:16.000000 altparse-0.2.0/src/altparse/ipautil/helpers.py
+-rw-rw-rw-   0        0        0     4150 2023-04-15 22:11:00.000000 altparse-0.2.0/src/altparse/ipautil/model.py
+-rw-rw-rw-   0        0        0    27352 2023-04-16 00:42:44.000000 altparse-0.2.0/src/altparse/model.py
+-rw-rw-rw-   0        0        0    14163 2023-04-15 23:54:41.000000 altparse-0.2.0/src/altparse/parsers.py
+drwxrwxrwx   0        0        0        0 2023-04-16 00:48:49.691393 altparse-0.2.0/src/altparse.egg-info/
+-rw-rw-rw-   0        0        0     2429 2023-04-16 00:48:49.000000 altparse-0.2.0/src/altparse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      720 2023-04-16 00:48:49.000000 altparse-0.2.0/src/altparse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 00:48:49.000000 altparse-0.2.0/src/altparse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-16 00:48:49.000000 altparse-0.2.0/src/altparse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-16 00:48:49.000000 altparse-0.2.0/src/altparse.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 00:48:49.796893 altparse-0.2.0/tests/
+-rw-rw-rw-   0        0        0   357189 2022-12-06 04:50:45.000000 altparse-0.2.0/tests/XPatcher_2.2.ipa
+-rw-rw-rw-   0        0        0        1 2022-12-01 07:44:32.000000 altparse-0.2.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      987 2022-12-06 07:11:28.000000 altparse-0.2.0/tests/example_ipa_upload.py
+-rw-rw-rw-   0        0        0     6199 2023-04-16 00:40:19.000000 altparse-0.2.0/tests/example_update.py
+-rw-rw-rw-   0        0        0   210229 2023-04-16 00:44:35.000000 altparse-0.2.0/tests/quantumsource.json
+-rw-rw-rw-   0        0        0      623 2022-12-06 07:31:59.000000 altparse-0.2.0/tests/test_create_altsource_obj.py
```

### Comparing `altparse-0.1.7/.gitignore` & `altparse-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `altparse-0.1.7/LICENSE.txt` & `altparse-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `altparse-0.1.7/PKG-INFO` & `altparse-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altparse
-Version: 0.1.7
+Version: 0.2.0
 Summary: Designed to aid in creating and maintaining AltSources
 Author-email: Noah Keck <noahkeck@mindspring.com>
 License: MIT License
         
         Copyright (c) 2022 Noah Keck
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `altparse-0.1.7/pyproject.toml` & `altparse-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "altparse"
-version = "0.1.7"
+version = "0.2.0"
 authors = [
     {name = "Noah Keck", email="noahkeck@mindspring.com"}
 ]
 license = {file = "LICENSE.txt"}
 description = "Designed to aid in creating and maintaining AltSources"
 readme = "README.md"
 keywords = ["altstore", "altsource", "ios", "developer"]
```

### Comparing `altparse-0.1.7/src/altparse/core.py` & `altparse-0.2.0/src/altparse/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,15 @@
                 ipa_path = Path(ipa_path)
             metadata = extract_altstore_metadata(ipa_path)
             
             # create initial version
             new_ver = {
                 "date": fmt_github_datetime(datetime.utcnow()),
                 "size": metadata.get("size"),
+                "sha256": metadata.get("sha256"),
                 "version": metadata.get("version"),
                 "downloadURL": download_url
             }
             new_ver = AltSource.App.Version(new_ver)
             
             # then create the overall app
             metadata = {**metadata,
@@ -116,17 +117,18 @@
                     apps = parser.parse_apps(None if data.get("getAllApps") else data.get("ids"))
                     for app in apps:
                         bundleID = app.appID
                         if bundleID in existingAppIDs:
                             # save the old versions property to ensure old versions aren't lost even if the other AltSource isn't tracking them
                             old_app = self.src.apps[existingAppIDs.index(bundleID)]
                             # version.parse() will be a lower value if the version is 'older'
-                            if version.parse(app.latest_version().version) > version.parse(self.src.apps[existingAppIDs.index(bundleID)].latest_version().version):
+                            new_ver = app.latest_version()
+                            if version.parse(new_ver.version) > version.parse(self.src.apps[existingAppIDs.index(bundleID)].latest_version().version):
                                 updatedAppsCount += 1
-                                old_app.add_version(app.latest_version())
+                                old_app.add_version(new_ver)
                             app._src = old_app._src # use the _src property to avoid overwrite warnings
                             self.src.apps[existingAppIDs.index(bundleID)] = app # note that this actually updates the app regardless of whether the version is newer
                         else:
                             addedAppsCount += 1
                             self.src.apps.append(app)
 
                     if not data.get("ignoreNews"):
@@ -165,14 +167,15 @@
                             metadata = parser.get_asset_metadata()
                             
                             new_ver = {
                                 "absoluteVersion": parser.version,
                                 "date": parser.versionDate,
                                 "localizedDescription": parser.versionDescription,
                                 "size": metadata.get("size"),
+                                "sha256": metadata.get("sha256"),
                                 "version": metadata.get("version") or parser.version,
                                 "downloadURL": metadata.get("downloadURL")
                             }
                             
                             new_ver = AltSource.App.Version(new_ver)
                             
                             if not metadata.get("bundleIdentifier"):
@@ -204,14 +207,31 @@
                 continue
             
             # end of for loop
             
         logging.info(f"{updatedAppsCount} app(s) updated.")
         logging.info(f"{addedAppsCount} app(s) added, {addedNewsCount} news article(s) added.")
 
+    def update_hashes(self, only_latest: bool = True, force_update: bool = False):
+        """Updates the sha256 hashes for 
+
+        Args:
+            only_latest (bool, optional): Only updates missing hashes for the latest version. Defaults to True.
+            force_update (bool, optional): Forces every app, every version to update its hash. Defaults to False.
+        """
+        for app in self.src.apps:
+            if only_latest:
+                latest_ver = app.latest_version()
+                if force_update or latest_ver.sha256 is None:
+                    latest_ver.calculate_sha256()
+            else:
+                for ver in app.versions:
+                    if force_update or ver.sha256 is None:
+                        ver.calculate_sha256()
+
     def alter_app_info(self, alternate_data: dict[str, dict[str, any]]):
         """Uses the provided alternate source info to automatically modify the data in the json.
         
         Caution: this method bypasses the built-in safety and formatting checks.
         
         alternate_data (dict | None, optional): A dictionary containing preferred AltStore app metadata using the bundleID as the key. Defaults to None.
         """
```

### Comparing `altparse-0.1.7/src/altparse/errors.py` & `altparse-0.2.0/src/altparse/errors.py`

 * *Files identical despite different names*

### Comparing `altparse-0.1.7/src/altparse/helpers.py` & `altparse-0.2.0/src/altparse/helpers.py`

 * *Files identical despite different names*

### Comparing `altparse-0.1.7/src/altparse/ipautil/core.py` & `altparse-0.2.0/src/altparse/ipautil/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from pathlib import Path
 
 from github3 import login
 from github3.exceptions import GitHubError
 from github3.repos.release import Release
 
 from altparse.ipautil.model import IPA_Info
+from altparse.ipautil.helpers import extract_sha256
 
 
 def get_or_create_github_release(github_token: str, repo_id: int | None = None, repo_name: str | None = None) -> Release:
     """Gets the github3.py Release object required to upload assets to.
     
     If neither a repo_id or repo_name is provided, a repository will be automatically generated. And if the selected repository does not contain any releases, one will be automatically generated.
 
@@ -67,12 +68,14 @@
     Returns:
         dict[str, Any]: Returns a dictionary containing the bundleID, version, and more
     """
     plist = IPA_Info(ipa_path=ipa_path, plist_path=plist_path)
     
     metadata = {
         "bundleIdentifier": plist.Identifier,
-        "version": plist.ShortVersion
+        "version": plist.ShortVersion,
+        "buildVersion": plist.Version
     }
     if ipa_path is not None:
         metadata["size"] = ipa_path.stat().st_size
+        metadata["sha256"] = extract_sha256(ipa_path)
     return metadata
```

### Comparing `altparse-0.1.7/src/altparse/ipautil/errors.py` & `altparse-0.2.0/src/altparse/ipautil/errors.py`

 * *Files identical despite different names*

### Comparing `altparse-0.1.7/src/altparse/ipautil/helpers.py` & `altparse-0.2.0/src/altparse/ipautil/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 :------------------------------------------------------------------------------:
 MIT License
 Copyright (c) 2022
 :------------------------------------------------------------------------------:
 """
 
 import atexit
+import hashlib
 import logging
 import os
 import re
 import shutil
 from pathlib import Path
 from tempfile import mkdtemp
 from zipfile import ZipFile
@@ -48,14 +49,22 @@
     atexit.register(cleanup_tempdir, tempdir)
     filename = "temp"
     r = requests.get(download_url)
     with open(tempdir / filename, "wb") as file:
         file.write(r.content)
     return tempdir / filename
 
+def extract_sha256(ipa_path: Path) -> str:
+    sha256_hash = hashlib.sha256()
+    with open(ipa_path,"rb") as f:
+        # Read and update hash string value in blocks of 4K
+        for byte_block in iter(lambda: f.read(4096),b""):
+            sha256_hash.update(byte_block)
+        return sha256_hash.hexdigest()
+
 def extract_ipa(ipa_path: Path, extract_twice: bool = False, use_temp_dir: bool = False) -> Path | Path:
     """Extracts the ipa data into a directory.
 
     If you are extracting twice, the normal .ipa file will be located in the parent directory of the returned path with the name "temp2.ipa".
     
     Args:
         ipa_path (Path): The Path to the ipa file.
```

### Comparing `altparse-0.1.7/src/altparse/ipautil/model.py` & `altparse-0.2.0/src/altparse/ipautil/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,25 +70,25 @@
         
     @property 
     def Name(self) -> str:
         return self._plist.get("CFBundleName")
         
     @property 
     def ShortVersion(self) -> str:
-        """The most commonly used and more accurate version.
+        """The most commonly used and more accurate version designed for display to end users.
         """
         return self._plist.get("CFBundleShortVersionString").lstrip("v")
         
     @property 
     def SupportedPlatforms(self) -> list[str]:
         return self._plist.get("CFBundleSupportedPlatforms")
         
     @property 
     def Version(self) -> str:
-        """Version that sometimes only contains the major version point.
+        """Version that is designed to indicate the internal build version, sometimes only contains one digit or the full version string.
         """
         return self._plist.get("CFBundleVersion")
     
     @property 
     def MinimumOSVersion(self) -> str:
         return self._plist.get("MinimumOSVersion")
```

### Comparing `altparse-0.1.7/src/altparse/model.py` & `altparse-0.2.0/src/altparse/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 import json
 import logging
 from pathlib import Path
 
 from altparse.errors import *
 from altparse.helpers import fmt_github_datetime, utcnow, parse_github_datetime
+from altparse.ipautil.helpers import extract_sha256, download_tempfile
 
 # Create a helper class in the namespace that acts as an intermediary to the logging.info to optionally silence the AltSource creation help text
 # OR remove the info help text from the model entirely and place in the cli instead
 
 class AltSource:
     class App:
         class Permission:
@@ -123,14 +124,21 @@
                 """Checks to see if the AltSource.App.Permission is valid and contains all the required information.
 
                 Returns:
                     bool: True if the `Permission` is a valid AltSource.App.Permission.
                 """
                 return not self.missing_keys()
             
+            def calculate_sha256(self):
+                """Calculates the sha256 hash based on the downloadURL object and sets the property.
+                """
+                if self.downloadURL is not None:
+                    ipa_path = download_tempfile(self.downloadURL)
+                    self.sha256 = extract_sha256(ipa_path)
+            
             @property 
             def version(self) -> str:
                 return self._src.get("version")
             @version.setter
             def version(self, value: str):
                 self._src["version"] = value
                 
@@ -193,15 +201,15 @@
             if src is None:
                 logging.info(f"Brand new AltSource.App created. Please remember to set the following properties: {self._requiredKeys}")
                 self._src = {
                     "name": "Example App", 
                     "bundleIdentifier": "com.example.app", 
                     "developerName": "Example.com", 
                     "versions": [],
-                    "localizedDescription": "An app that is an example.", 
+                    "localizedDescription": "An app that is an example.",
                     "iconURL": "https://example.com/icon.png"
                     }
             else:
                 self._src = src
                 if "permissions" in src.keys():
                     self._src["permissions"] = [self.Permission(perm) for perm in src["permissions"]]
                 if "versions" in src.keys():
```

### Comparing `altparse-0.1.7/src/altparse/parsers.py` & `altparse-0.2.0/src/altparse/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
             release["asset"] = asset # set asset in the release to only be most recently IPA found
             
         def alter_tag_names(releases: list):
             for index, release in enumerate(releases):
                 alter_tag_name(release)
                 ver = version.parse(release["tag_name"])
                 if isinstance(ver, version.LegacyVersion):
-                    logging.warning(f"Invalid version removed: {ver.base_version}")
+                    logging.warning(f"Invalid GitHub tag version not considered: {ver.base_version}")
                     releases.pop(index)
 
         def alter_tag_name(release: dict):
             release["tag_name"] = ver_parse(release["tag_name"])
         
         #### Parse the correct release ####
         if not include_pre:
```

### Comparing `altparse-0.1.7/src/altparse.egg-info/PKG-INFO` & `altparse-0.2.0/src/altparse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altparse
-Version: 0.1.7
+Version: 0.2.0
 Summary: Designed to aid in creating and maintaining AltSources
 Author-email: Noah Keck <noahkeck@mindspring.com>
 License: MIT License
         
         Copyright (c) 2022 Noah Keck
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `altparse-0.1.7/src/altparse.egg-info/SOURCES.txt` & `altparse-0.2.0/src/altparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `altparse-0.1.7/tests/XPatcher_2.2.ipa` & `altparse-0.2.0/tests/XPatcher_2.2.ipa`

 * *Files identical despite different names*

### Comparing `altparse-0.1.7/tests/example_ipa_upload.py` & `altparse-0.2.0/tests/example_ipa_upload.py`

 * *Files identical despite different names*

### Comparing `altparse-0.1.7/tests/example_update.py` & `altparse-0.2.0/tests/example_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,9 +141,10 @@
     }
 }
 
 src = altsource_from_file("quantumsource.json")
 srcmgr = AltSourceManager(src, sourcesData)
 
 srcmgr.update()
+srcmgr.update_hashes()
 srcmgr.alter_app_info(alternateAppData)
 srcmgr.save(prettify=True) # if prettify is true, output will have indents and newlines
```

### Comparing `altparse-0.1.7/tests/quantumsource.json` & `altparse-0.2.0/tests/quantumsource.json`

 * *Files identical despite different names*

### Comparing `altparse-0.1.7/tests/test_create_altsource_obj.py` & `altparse-0.2.0/tests/test_create_altsource_obj.py`

 * *Files identical despite different names*

