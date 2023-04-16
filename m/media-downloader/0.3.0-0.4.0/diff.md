# Comparing `tmp/media_downloader-0.3.0-py2.py3-none-any.whl.zip` & `tmp/media_downloader-0.4.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6159 bytes, number of entries: 9
--rw-r--r--  2.0 unx      348 b- defN 22-Dec-23 19:04 media_downloader/__init__.py
--rw-r--r--  2.0 unx     8966 b- defN 22-Dec-23 19:04 media_downloader/media_downloader.py
--rw-r--r--  2.0 unx      116 b- defN 22-Dec-23 19:04 media_downloader/version.py
--rw-r--r--  2.0 unx     1210 b- defN 22-Dec-23 19:04 media_downloader-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2133 b- defN 22-Dec-23 19:04 media_downloader-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Dec-23 19:04 media_downloader-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       77 b- defN 22-Dec-23 19:04 media_downloader-0.3.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       17 b- defN 22-Dec-23 19:04 media_downloader-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      796 b- defN 22-Dec-23 19:04 media_downloader-0.3.0.dist-info/RECORD
-9 files, 13773 bytes uncompressed, 4765 bytes compressed:  65.4%
+Zip file size: 6158 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      348 b- defN 23-Apr-16 04:38 media_downloader/__init__.py
+-rw-r--r--  2.0 unx     8954 b- defN 23-Apr-16 04:38 media_downloader/media_downloader.py
+-rw-r--r--  2.0 unx      116 b- defN 23-Apr-16 04:38 media_downloader/version.py
+-rw-r--r--  2.0 unx     1210 b- defN 23-Apr-16 04:38 media_downloader-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2127 b- defN 23-Apr-16 04:38 media_downloader-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-16 04:38 media_downloader-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       77 b- defN 23-Apr-16 04:38 media_downloader-0.4.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-16 04:38 media_downloader-0.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      796 b- defN 23-Apr-16 04:38 media_downloader-0.4.0.dist-info/RECORD
+9 files, 13755 bytes uncompressed, 4764 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: media_downloader/media_downloader.py
 Comment: 
 
 Filename: media_downloader/version.py
 Comment: 
 
-Filename: media_downloader-0.3.0.dist-info/LICENSE
+Filename: media_downloader-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: media_downloader-0.3.0.dist-info/METADATA
+Filename: media_downloader-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: media_downloader-0.3.0.dist-info/WHEEL
+Filename: media_downloader-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: media_downloader-0.3.0.dist-info/entry_points.txt
+Filename: media_downloader-0.4.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: media_downloader-0.3.0.dist-info/top_level.txt
+Filename: media_downloader-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: media_downloader-0.3.0.dist-info/RECORD
+Filename: media_downloader-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## media_downloader/media_downloader.py

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 import os
 import sys
 import re
 import getopt
 import requests
-import youtube_dl
+import yt_dlp
 from multiprocessing import Pool
 
 
 class StdOutLogger(object):
     def debug(self, msg):
         print(f'{msg}')
 
@@ -96,15 +96,15 @@
             ydl_opts = {
                 'format': 'best',
                 'progress_with_newline': True,
                 'logger': StdOutLogger(),
                 'outtmpl': outtmpl
             }
         try:
-            with youtube_dl.YoutubeDL(ydl_opts) as ydl:
+            with yt_dlp.YoutubeDL(ydl_opts) as ydl:
                 print(ydl.download([link]))
         except Exception as e:
             try:
                 if self.audio:
                     outtmpl = f'{self.download_directory}/%(id)s.%(ext)s'
                     ydl_opts = {
                         'format': 'bestaudio/best',
@@ -120,15 +120,15 @@
                 else:
                     ydl_opts = {
                         'format': 'best',
                         'progress_with_newline': True,
                         'logger': StdOutLogger(),
                         'outtmpl': outtmpl
                     }
-                with youtube_dl.YoutubeDL(ydl_opts) as ydl:
+                with yt_dlp.YoutubeDL(ydl_opts) as ydl:
                     print(ydl.download([link]))
             except Exception as e:
                 print(f"Unable to download video: {link}")
 
     def get_channel_videos(self, channel, limit=-1):
         vids = None
         username = channel
```

## media_downloader/version.py

```diff
@@ -1,6 +1,6 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-__version__ = '0.3.0'
+__version__ = '0.4.0'
 __author__ = 'Audel Rouhi'
 __credits__ = 'Audel Rouhi'
```

## Comparing `media_downloader-0.3.0.dist-info/LICENSE` & `media_downloader-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `media_downloader-0.3.0.dist-info/METADATA` & `media_downloader-0.4.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: media-downloader
-Version: 0.3.0
+Version: 0.4.0
 Summary: Download audio/videos from the internet!
 Home-page: https://github.com/Knuckles-Team/media-downloader
 Author: Audel Rouhi
 Author-email: knucklessg1@gmail.com
 License: Unlicense
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,18 +14,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests (>=2.28.1)
-Requires-Dist: youtube-dl (>=2021.12.17)
+Requires-Dist: yt-dlp (>=2023.3.4)
 
 # Media Downloader
-*Version: 0.3.0*
+*Version: 0.4.0*
 
 Download videos and audio from the internet!
 
 ### Supports:
 - YouTube
 - Twitter
 - Rumble
```

