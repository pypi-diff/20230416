# Comparing `tmp/altparse-0.2.0.tar.gz` & `tmp/altparse-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altparse-0.2.0.tar", last modified: Sun Apr 16 00:48:49 2023, max compression
+gzip compressed data, was "altparse-0.2.1.tar", last modified: Sun Apr 16 01:28:10 2023, max compression
```

## Comparing `altparse-0.2.0.tar` & `altparse-0.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 00:48:49.798894 altparse-0.2.0/
--rw-rw-rw-   0        0        0       66 2022-05-23 21:26:59.000000 altparse-0.2.0/.gitattributes
--rw-rw-rw-   0        0        0     1447 2022-06-03 19:24:20.000000 altparse-0.2.0/.gitignore
--rw-rw-rw-   0        0        0        0 2022-11-30 22:58:46.000000 altparse-0.2.0/CHANGES.md
--rw-rw-rw-   0        0        0     1086 2022-05-23 21:26:59.000000 altparse-0.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0        0 2022-11-30 22:59:45.000000 altparse-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2429 2023-04-16 00:48:49.798392 altparse-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-02-26 04:17:54.000000 altparse-0.2.0/README.md
--rw-rw-rw-   0        0        0     1018 2023-04-16 00:48:22.000000 altparse-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-16 00:48:49.798894 altparse-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0       71 2022-12-01 01:01:54.000000 altparse-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 00:48:49.548035 altparse-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 00:48:49.664393 altparse-0.2.0/src/altparse/
--rw-rw-rw-   0        0        0      155 2022-12-06 02:28:59.000000 altparse-0.2.0/src/altparse/__init__.py
--rw-rw-rw-   0        0        0    13592 2023-04-16 00:40:47.000000 altparse-0.2.0/src/altparse/core.py
--rw-rw-rw-   0        0        0      615 2023-03-28 23:48:04.000000 altparse-0.2.0/src/altparse/errors.py
--rw-rw-rw-   0        0        0     3101 2022-12-06 07:19:15.000000 altparse-0.2.0/src/altparse/helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-16 00:48:49.728892 altparse-0.2.0/src/altparse/ipautil/
--rw-rw-rw-   0        0        0      156 2022-12-06 07:29:32.000000 altparse-0.2.0/src/altparse/ipautil/__init__.py
--rw-rw-rw-   0        0        0     3493 2023-04-15 22:08:19.000000 altparse-0.2.0/src/altparse/ipautil/core.py
--rw-rw-rw-   0        0        0      603 2022-12-06 07:12:17.000000 altparse-0.2.0/src/altparse/ipautil/errors.py
--rw-rw-rw-   0        0        0     4857 2023-04-15 19:21:16.000000 altparse-0.2.0/src/altparse/ipautil/helpers.py
--rw-rw-rw-   0        0        0     4150 2023-04-15 22:11:00.000000 altparse-0.2.0/src/altparse/ipautil/model.py
--rw-rw-rw-   0        0        0    27352 2023-04-16 00:42:44.000000 altparse-0.2.0/src/altparse/model.py
--rw-rw-rw-   0        0        0    14163 2023-04-15 23:54:41.000000 altparse-0.2.0/src/altparse/parsers.py
-drwxrwxrwx   0        0        0        0 2023-04-16 00:48:49.691393 altparse-0.2.0/src/altparse.egg-info/
--rw-rw-rw-   0        0        0     2429 2023-04-16 00:48:49.000000 altparse-0.2.0/src/altparse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      720 2023-04-16 00:48:49.000000 altparse-0.2.0/src/altparse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 00:48:49.000000 altparse-0.2.0/src/altparse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-16 00:48:49.000000 altparse-0.2.0/src/altparse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-16 00:48:49.000000 altparse-0.2.0/src/altparse.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-16 00:48:49.796893 altparse-0.2.0/tests/
--rw-rw-rw-   0        0        0   357189 2022-12-06 04:50:45.000000 altparse-0.2.0/tests/XPatcher_2.2.ipa
--rw-rw-rw-   0        0        0        1 2022-12-01 07:44:32.000000 altparse-0.2.0/tests/__init__.py
--rw-rw-rw-   0        0        0      987 2022-12-06 07:11:28.000000 altparse-0.2.0/tests/example_ipa_upload.py
--rw-rw-rw-   0        0        0     6199 2023-04-16 00:40:19.000000 altparse-0.2.0/tests/example_update.py
--rw-rw-rw-   0        0        0   210229 2023-04-16 00:44:35.000000 altparse-0.2.0/tests/quantumsource.json
--rw-rw-rw-   0        0        0      623 2022-12-06 07:31:59.000000 altparse-0.2.0/tests/test_create_altsource_obj.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:28:10.168700 altparse-0.2.1/
+-rw-rw-rw-   0        0        0       66 2022-05-23 21:26:59.000000 altparse-0.2.1/.gitattributes
+-rw-rw-rw-   0        0        0     1447 2022-06-03 19:24:20.000000 altparse-0.2.1/.gitignore
+-rw-rw-rw-   0        0        0        0 2022-11-30 22:58:46.000000 altparse-0.2.1/CHANGES.md
+-rw-rw-rw-   0        0        0     1086 2022-05-23 21:26:59.000000 altparse-0.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0        0 2022-11-30 22:59:45.000000 altparse-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2429 2023-04-16 01:28:10.168198 altparse-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-02-26 04:17:54.000000 altparse-0.2.1/README.md
+-rw-rw-rw-   0        0        0     1018 2023-04-16 01:26:48.000000 altparse-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 01:28:10.169200 altparse-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0       71 2022-12-01 01:01:54.000000 altparse-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:28:10.063699 altparse-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 01:28:10.095699 altparse-0.2.1/src/altparse/
+-rw-rw-rw-   0        0        0      155 2022-12-06 02:28:59.000000 altparse-0.2.1/src/altparse/__init__.py
+-rw-rw-rw-   0        0        0    13618 2023-04-16 01:10:40.000000 altparse-0.2.1/src/altparse/core.py
+-rw-rw-rw-   0        0        0      615 2023-03-28 23:48:04.000000 altparse-0.2.1/src/altparse/errors.py
+-rw-rw-rw-   0        0        0     3101 2022-12-06 07:19:15.000000 altparse-0.2.1/src/altparse/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:28:10.131697 altparse-0.2.1/src/altparse/ipautil/
+-rw-rw-rw-   0        0        0      156 2022-12-06 07:29:32.000000 altparse-0.2.1/src/altparse/ipautil/__init__.py
+-rw-rw-rw-   0        0        0     3493 2023-04-15 22:08:19.000000 altparse-0.2.1/src/altparse/ipautil/core.py
+-rw-rw-rw-   0        0        0      603 2022-12-06 07:12:17.000000 altparse-0.2.1/src/altparse/ipautil/errors.py
+-rw-rw-rw-   0        0        0     5074 2023-04-16 01:16:54.000000 altparse-0.2.1/src/altparse/ipautil/helpers.py
+-rw-rw-rw-   0        0        0     4150 2023-04-15 22:11:00.000000 altparse-0.2.1/src/altparse/ipautil/model.py
+-rw-rw-rw-   0        0        0    27402 2023-04-16 01:19:43.000000 altparse-0.2.1/src/altparse/model.py
+-rw-rw-rw-   0        0        0    14271 2023-04-16 01:26:02.000000 altparse-0.2.1/src/altparse/parsers.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:28:10.122698 altparse-0.2.1/src/altparse.egg-info/
+-rw-rw-rw-   0        0        0     2429 2023-04-16 01:28:09.000000 altparse-0.2.1/src/altparse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      720 2023-04-16 01:28:10.000000 altparse-0.2.1/src/altparse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 01:28:09.000000 altparse-0.2.1/src/altparse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-16 01:28:09.000000 altparse-0.2.1/src/altparse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-16 01:28:09.000000 altparse-0.2.1/src/altparse.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 01:28:10.166198 altparse-0.2.1/tests/
+-rw-rw-rw-   0        0        0   357189 2022-12-06 04:50:45.000000 altparse-0.2.1/tests/XPatcher_2.2.ipa
+-rw-rw-rw-   0        0        0        1 2022-12-01 07:44:32.000000 altparse-0.2.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      987 2022-12-06 07:11:28.000000 altparse-0.2.1/tests/example_ipa_upload.py
+-rw-rw-rw-   0        0        0     6199 2023-04-16 00:40:19.000000 altparse-0.2.1/tests/example_update.py
+-rw-rw-rw-   0        0        0   210229 2023-04-16 00:44:35.000000 altparse-0.2.1/tests/quantumsource.json
+-rw-rw-rw-   0        0        0      623 2022-12-06 07:31:59.000000 altparse-0.2.1/tests/test_create_altsource_obj.py
```

### Comparing `altparse-0.2.0/.gitignore` & `altparse-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `altparse-0.2.0/LICENSE.txt` & `altparse-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `altparse-0.2.0/PKG-INFO` & `altparse-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altparse
-Version: 0.2.0
+Version: 0.2.1
 Summary: Designed to aid in creating and maintaining AltSources
 Author-email: Noah Keck <noahkeck@mindspring.com>
 License: MIT License
         
         Copyright (c) 2022 Noah Keck
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `altparse-0.2.0/pyproject.toml` & `altparse-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "altparse"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     {name = "Noah Keck", email="noahkeck@mindspring.com"}
 ]
 license = {file = "LICENSE.txt"}
 description = "Designed to aid in creating and maintaining AltSources"
 readme = "README.md"
 keywords = ["altstore", "altsource", "ios", "developer"]
```

### Comparing `altparse-0.2.0/src/altparse/core.py` & `altparse-0.2.1/src/altparse/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
             
             # end of for loop
             
         logging.info(f"{updatedAppsCount} app(s) updated.")
         logging.info(f"{addedAppsCount} app(s) added, {addedNewsCount} news article(s) added.")
 
     def update_hashes(self, only_latest: bool = True, force_update: bool = False):
-        """Updates the sha256 hashes for 
+        """Updates the sha256 hashes for the apps in the AltSource.
 
         Args:
             only_latest (bool, optional): Only updates missing hashes for the latest version. Defaults to True.
             force_update (bool, optional): Forces every app, every version to update its hash. Defaults to False.
         """
         for app in self.src.apps:
             if only_latest:
```

### Comparing `altparse-0.2.0/src/altparse/errors.py` & `altparse-0.2.1/src/altparse/errors.py`

 * *Files identical despite different names*

### Comparing `altparse-0.2.0/src/altparse/helpers.py` & `altparse-0.2.1/src/altparse/helpers.py`

 * *Files identical despite different names*

### Comparing `altparse-0.2.0/src/altparse/ipautil/core.py` & `altparse-0.2.1/src/altparse/ipautil/core.py`

 * *Files identical despite different names*

### Comparing `altparse-0.2.0/src/altparse/ipautil/errors.py` & `altparse-0.2.1/src/altparse/ipautil/errors.py`

 * *Files identical despite different names*

### Comparing `altparse-0.2.0/src/altparse/ipautil/helpers.py` & `altparse-0.2.1/src/altparse/ipautil/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,29 +32,34 @@
         else:
             os.remove(fp.as_posix())
     except FileNotFoundError as err:
         logging.debug(f"File not found in temporary directory: {str(fp)}")
     except Exception as err:
         logging.warning(f"Unable to cleanup files in temporary directory: {str(fp)} due to {err.__class__}")
 
-def download_tempfile(download_url: str) -> Path:
-    """Downloads file to a temporary directory.
+def download_tempfile(download_url: str) -> Path | None:
+    """Downloads file to a temporary directory. If a file cannot be downloaded, it returns None.
 
     Args:
         download_url (str): The url of the file to be downloaded.
 
     Returns:
         Path: The Path obj pointing to the downloaded file.
     """
     tempdir = Path(mkdtemp())
     atexit.register(cleanup_tempdir, tempdir)
     filename = "temp"
     r = requests.get(download_url)
     with open(tempdir / filename, "wb") as file:
         file.write(r.content)
+    try:
+        open(tempdir / filename, "r")
+    except OSError as err:
+        logging.error("Could not find/open downloaded file.")
+        return None
     return tempdir / filename
 
 def extract_sha256(ipa_path: Path) -> str:
     sha256_hash = hashlib.sha256()
     with open(ipa_path,"rb") as f:
         # Read and update hash string value in blocks of 4K
         for byte_block in iter(lambda: f.read(4096),b""):
```

### Comparing `altparse-0.2.0/src/altparse/ipautil/model.py` & `altparse-0.2.1/src/altparse/ipautil/model.py`

 * *Files identical despite different names*

### Comparing `altparse-0.2.0/src/altparse/model.py` & `altparse-0.2.1/src/altparse/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,16 @@
                 return not self.missing_keys()
             
             def calculate_sha256(self):
                 """Calculates the sha256 hash based on the downloadURL object and sets the property.
                 """
                 if self.downloadURL is not None:
                     ipa_path = download_tempfile(self.downloadURL)
-                    self.sha256 = extract_sha256(ipa_path)
+                    if ipa_path is not None:
+                        self.sha256 = extract_sha256(ipa_path)
             
             @property 
             def version(self) -> str:
                 return self._src.get("version")
             @version.setter
             def version(self, value: str):
                 self._src["version"] = value
```

### Comparing `altparse-0.2.0/src/altparse/parsers.py` & `altparse-0.2.1/src/altparse/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,16 @@
         return "# " + self.data["name"] + "\n\n" + self.data["body"]
 
     def get_asset_metadata(self) -> dict[str]:
         """Returns a dictionary containing the downloadURL, size, bundleID, version
         """
         download_url = "https://unc0ver.dev" + self.data["browser_download_url"]
         ipa_path = download_tempfile(download_url)
-        metadata = extract_altstore_metadata(ipa_path)
+        if ipa_path is not None:
+            metadata = extract_altstore_metadata(ipa_path)
         metadata["downloadURL"] = download_url
         return metadata
 
 class GithubParser:
     def __init__(self, url: str | None = None, repo_author: str | None = None, repo_name: str | None = None, ver_parse: Callable = lambda x: x.lstrip("v"), include_pre: bool = False, prefer_date: bool = False, asset_regex: str = r".*\.ipa", extract_twice: bool = False, upload_ipa_repo: Release | None = None, **kwargs):
         """Create a new GithubParser object that can be used to generate an AltSource.App.
         
@@ -247,23 +248,24 @@
 
         Returns:
             dict: A dictionary containing the downloadURL, size, bundleID, version, and more.
         """
         download_url = self.data["asset"]["browser_download_url"]
 
         ipa_path = download_tempfile(download_url)
-        payload_path = extract_ipa(ipa_path, self.extract_twice)
-        if self.extract_twice:
-            ipa_path = payload_path.parent / "temp2.ipa"
-        plist_path = list(payload_path.rglob("Info.plist"))[0] # locate the Info.plist path within the extracted data
-        metadata = extract_altstore_metadata(ipa_path=ipa_path, plist_path=plist_path)
-        
-        # Uploads the ipa to a separate GitHub repository after its been processed
-        if self.upload_ipa_repo is not None:
-            download_url = upload_ipa_github(ipa_path, self.upload_ipa_repo, name=metadata["bundleIdentifier"], ver=metadata["version"])
+        if ipa_path is not None:
+            payload_path = extract_ipa(ipa_path, self.extract_twice)
+            if self.extract_twice:
+                ipa_path = payload_path.parent / "temp2.ipa"
+            plist_path = list(payload_path.rglob("Info.plist"))[0] # locate the Info.plist path within the extracted data
+            metadata = extract_altstore_metadata(ipa_path=ipa_path, plist_path=plist_path)
+            
+            # Uploads the ipa to a separate GitHub repository after its been processed
+            if self.upload_ipa_repo is not None:
+                download_url = upload_ipa_github(ipa_path, self.upload_ipa_repo, name=metadata["bundleIdentifier"], ver=metadata["version"])
         
         metadata["downloadURL"] = download_url
         return metadata
 
 class Parser(Enum):
     ALTSOURCE = AltSourceParser
     GITHUB = GithubParser
```

### Comparing `altparse-0.2.0/src/altparse.egg-info/PKG-INFO` & `altparse-0.2.1/src/altparse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altparse
-Version: 0.2.0
+Version: 0.2.1
 Summary: Designed to aid in creating and maintaining AltSources
 Author-email: Noah Keck <noahkeck@mindspring.com>
 License: MIT License
         
         Copyright (c) 2022 Noah Keck
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `altparse-0.2.0/src/altparse.egg-info/SOURCES.txt` & `altparse-0.2.1/src/altparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `altparse-0.2.0/tests/XPatcher_2.2.ipa` & `altparse-0.2.1/tests/XPatcher_2.2.ipa`

 * *Files identical despite different names*

### Comparing `altparse-0.2.0/tests/example_ipa_upload.py` & `altparse-0.2.1/tests/example_ipa_upload.py`

 * *Files identical despite different names*

### Comparing `altparse-0.2.0/tests/example_update.py` & `altparse-0.2.1/tests/example_update.py`

 * *Files identical despite different names*

### Comparing `altparse-0.2.0/tests/quantumsource.json` & `altparse-0.2.1/tests/quantumsource.json`

 * *Files identical despite different names*

### Comparing `altparse-0.2.0/tests/test_create_altsource_obj.py` & `altparse-0.2.1/tests/test_create_altsource_obj.py`

 * *Files identical despite different names*

