# Comparing `tmp/spotify_dl-8.6.0.tar.gz` & `tmp/spotify_dl-8.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify_dl-8.6.0.tar", last modified: Tue Mar 14 22:50:51 2023, max compression
+gzip compressed data, was "spotify_dl-8.7.0.tar", last modified: Sun Apr 16 08:58:03 2023, max compression
```

## Comparing `spotify_dl-8.6.0.tar` & `spotify_dl-8.7.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:50:51.135841 spotify_dl-8.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-14 22:50:42.000000 spotify_dl-8.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-14 22:50:42.000000 spotify_dl-8.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-03-14 22:50:51.135841 spotify_dl-8.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-03-14 22:50:42.000000 spotify_dl-8.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-14 22:50:42.000000 spotify_dl-8.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 22:50:51.135841 spotify_dl-8.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-03-14 22:50:42.000000 spotify_dl-8.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:50:51.135841 spotify_dl-8.6.0/spotify_dl/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-14 22:50:42.000000 spotify_dl-8.6.0/spotify_dl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-14 22:50:42.000000 spotify_dl-8.6.0/spotify_dl/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-03-14 22:50:42.000000 spotify_dl-8.6.0/spotify_dl/scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-03-14 22:50:42.000000 spotify_dl-8.6.0/spotify_dl/spotify.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6196 2023-03-14 22:50:42.000000 spotify_dl-8.6.0/spotify_dl/spotify_dl.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-14 22:50:42.000000 spotify_dl-8.6.0/spotify_dl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-03-14 22:50:42.000000 spotify_dl-8.6.0/spotify_dl/youtube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:50:51.135841 spotify_dl-8.6.0/spotify_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-03-14 22:50:51.000000 spotify_dl-8.6.0/spotify_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-14 22:50:51.000000 spotify_dl-8.6.0/spotify_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 22:50:51.000000 spotify_dl-8.6.0/spotify_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-14 22:50:51.000000 spotify_dl-8.6.0/spotify_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-14 22:50:51.000000 spotify_dl-8.6.0/spotify_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-14 22:50:51.000000 spotify_dl-8.6.0/spotify_dl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:58:03.095536 spotify_dl-8.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-16 08:57:48.000000 spotify_dl-8.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-16 08:57:48.000000 spotify_dl-8.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-16 08:58:03.095536 spotify_dl-8.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-04-16 08:57:48.000000 spotify_dl-8.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-16 08:57:48.000000 spotify_dl-8.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 08:58:03.095536 spotify_dl-8.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-16 08:57:48.000000 spotify_dl-8.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:58:03.095536 spotify_dl-8.7.0/spotify_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-16 08:57:48.000000 spotify_dl-8.7.0/spotify_dl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-16 08:57:48.000000 spotify_dl-8.7.0/spotify_dl/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-16 08:57:48.000000 spotify_dl-8.7.0/spotify_dl/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-04-16 08:57:48.000000 spotify_dl-8.7.0/spotify_dl/spotify.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6196 2023-04-16 08:57:48.000000 spotify_dl-8.7.0/spotify_dl/spotify_dl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-16 08:57:48.000000 spotify_dl-8.7.0/spotify_dl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-04-16 08:57:48.000000 spotify_dl-8.7.0/spotify_dl/youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:58:03.095536 spotify_dl-8.7.0/spotify_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-16 08:58:03.000000 spotify_dl-8.7.0/spotify_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-16 08:58:03.000000 spotify_dl-8.7.0/spotify_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 08:58:03.000000 spotify_dl-8.7.0/spotify_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-16 08:58:03.000000 spotify_dl-8.7.0/spotify_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-16 08:58:03.000000 spotify_dl-8.7.0/spotify_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-16 08:58:03.000000 spotify_dl-8.7.0/spotify_dl.egg-info/top_level.txt
```

### Comparing `spotify_dl-8.6.0/LICENSE` & `spotify_dl-8.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spotify_dl-8.6.0/PKG-INFO` & `spotify_dl-8.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify_dl
-Version: 8.6.0
+Version: 8.7.0
 Summary: Downloads songs from a Spotify Playlist/Track/Album that you provide
 Home-page: https://github.com/SathyaBhat/spotify-dl/
 Author: Sathya Bhat
 Author-email: sathya@sathyasays.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `spotify_dl-8.6.0/README.md` & `spotify_dl-8.7.0/README.md`

 * *Files identical despite different names*

### Comparing `spotify_dl-8.6.0/setup.py` & `spotify_dl-8.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `spotify_dl-8.6.0/spotify_dl/scaffold.py` & `spotify_dl-8.7.0/spotify_dl/scaffold.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,12 +44,12 @@
             $env:SPOTIPY_CLIENT_SECRET='your-spotify-client-secret'
 
             Windows CMD:
             set SPOTIPY_CLIENT_ID=your-spotify-client-id
             set SPOTIPY_CLIENT_SECRET=your-spotify-client-secret
 
             Get your credentials at
-                https://developer.spotify.com/my-applications
+                https://developer.spotify.com/dashboard
         """
         )
         return None
     return CLIENT_ID, CLIENT_SECRET
```

### Comparing `spotify_dl-8.6.0/spotify_dl/spotify.py` & `spotify_dl-8.7.0/spotify_dl/spotify.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,15 @@
     :param url: URL to be parsed
 
     :return tuple indicating the type and id of the item
     """
     if url.startswith("spotify:"):
         log.error("Spotify URI was provided instead of a playlist/album/track URL.")
         sys.exit(1)
-    parsed_url = url.replace("https://open.spotify.com/", "")
+    parsed_url = url.replace("https://open.spotify.com/", "").split("?")[0]
     item_type = parsed_url.split("/")[0]
     item_id = parsed_url.split("/")[1]
     return item_type, item_id
 
 
 def get_item_name(sp, item_type, item_id):
     """
```

### Comparing `spotify_dl-8.6.0/spotify_dl/spotify_dl.py` & `spotify_dl-8.7.0/spotify_dl/spotify_dl.py`

 * *Files identical despite different names*

### Comparing `spotify_dl-8.6.0/spotify_dl/youtube.py` & `spotify_dl-8.7.0/spotify_dl/youtube.py`

 * *Files identical despite different names*

### Comparing `spotify_dl-8.6.0/spotify_dl.egg-info/PKG-INFO` & `spotify_dl-8.7.0/spotify_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-dl
-Version: 8.6.0
+Version: 8.7.0
 Summary: Downloads songs from a Spotify Playlist/Track/Album that you provide
 Home-page: https://github.com/SathyaBhat/spotify-dl/
 Author: Sathya Bhat
 Author-email: sathya@sathyasays.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

