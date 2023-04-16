# Comparing `tmp/tuneflow-py-0.5.1.tar.gz` & `tmp/tuneflow-py-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneflow-py-0.5.1.tar", last modified: Mon Apr 10 18:45:31 2023, max compression
+gzip compressed data, was "tuneflow-py-0.6.0.tar", last modified: Sun Apr 16 21:26:52 2023, max compression
```

## Comparing `tuneflow-py-0.5.1.tar` & `tuneflow-py-0.6.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 18:45:31.446440 tuneflow-py-0.5.1/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1065 2023-01-10 14:03:44.000000 tuneflow-py-0.5.1/LICENSE
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-04-10 18:45:31.446440 tuneflow-py-0.5.1/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)     3809 2023-03-06 23:39:23.000000 tuneflow-py-0.5.1/README.md
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1288 2023-04-10 18:44:50.000000 tuneflow-py-0.5.1/pyproject.toml
--rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-04-10 18:45:31.446440 tuneflow-py-0.5.1/setup.cfg
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 18:45:31.446440 tuneflow-py-0.5.1/src/
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 18:45:31.446440 tuneflow-py-0.5.1/src/tuneflow_py/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1155 2023-04-10 06:26:06.000000 tuneflow-py-0.5.1/src/tuneflow_py/__init__.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1987 2023-02-28 00:04:43.000000 tuneflow-py-0.5.1/src/tuneflow_py/base_plugin.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 18:45:31.446440 tuneflow-py-0.5.1/src/tuneflow_py/descriptors/
--rw-r--r--   0 panacea   (1000) panacea   (1000)      922 2023-03-30 21:40:36.000000 tuneflow-py-0.5.1/src/tuneflow_py/descriptors/audio_plugin_descriptor.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1579 2023-03-30 21:53:02.000000 tuneflow-py-0.5.1/src/tuneflow_py/descriptors/clip_descriptor.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)      439 2023-03-30 21:53:05.000000 tuneflow-py-0.5.1/src/tuneflow_py/descriptors/common.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4221 2023-03-30 21:53:07.000000 tuneflow-py-0.5.1/src/tuneflow_py/descriptors/param.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4407 2023-03-30 21:53:10.000000 tuneflow-py-0.5.1/src/tuneflow_py/descriptors/plugin.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)       71 2023-03-30 21:53:12.000000 tuneflow-py-0.5.1/src/tuneflow_py/descriptors/text.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     5575 2023-03-31 22:25:01.000000 tuneflow-py-0.5.1/src/tuneflow_py/descriptors/widget.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 18:45:31.446440 tuneflow-py-0.5.1/src/tuneflow_py/models/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     3128 2023-03-01 03:02:02.000000 tuneflow-py-0.5.1/src/tuneflow_py/models/audio_plugin.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    17158 2023-03-31 07:33:41.000000 tuneflow-py-0.5.1/src/tuneflow_py/models/automation.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    23875 2023-03-31 07:45:07.000000 tuneflow-py-0.5.1/src/tuneflow_py/models/clip.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1305 2023-04-10 18:15:27.000000 tuneflow-py-0.5.1/src/tuneflow_py/models/marker.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     5275 2023-02-22 00:50:28.000000 tuneflow-py-0.5.1/src/tuneflow_py/models/note.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 18:45:31.446440 tuneflow-py-0.5.1/src/tuneflow_py/models/protos/
--rw-r--r--   0 panacea   (1000) panacea   (1000)    70682 2023-04-10 18:11:02.000000 tuneflow-py-0.5.1/src/tuneflow_py/models/protos/song_pb2.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    25607 2023-04-10 18:24:50.000000 tuneflow-py-0.5.1/src/tuneflow_py/models/song.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)      873 2023-03-01 22:09:14.000000 tuneflow-py-0.5.1/src/tuneflow_py/models/tempo.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1093 2023-02-22 00:28:50.000000 tuneflow-py-0.5.1/src/tuneflow_py/models/time_signature.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    16387 2023-03-31 16:53:25.000000 tuneflow-py-0.5.1/src/tuneflow_py/models/track.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     6210 2023-03-29 01:48:05.000000 tuneflow-py-0.5.1/src/tuneflow_py/utils.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 18:45:31.446440 tuneflow-py-0.5.1/src/tuneflow_py.egg-info/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-04-10 18:45:31.000000 tuneflow-py-0.5.1/src/tuneflow_py.egg-info/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1113 2023-04-10 18:45:31.000000 tuneflow-py-0.5.1/src/tuneflow_py.egg-info/SOURCES.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-04-10 18:45:31.000000 tuneflow-py-0.5.1/src/tuneflow_py.egg-info/dependency_links.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)       96 2023-04-10 18:45:31.000000 tuneflow-py-0.5.1/src/tuneflow_py.egg-info/requires.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)       12 2023-04-10 18:45:31.000000 tuneflow-py-0.5.1/src/tuneflow_py.egg-info/top_level.txt
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 18:45:31.446440 tuneflow-py-0.5.1/test/
--rw-r--r--   0 panacea   (1000) panacea   (1000)    21690 2023-02-24 04:10:42.000000 tuneflow-py-0.5.1/test/test_audio_clip.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    24170 2023-03-31 07:02:16.000000 tuneflow-py-0.5.1/test/test_automation.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     8001 2023-04-10 18:37:18.000000 tuneflow-py-0.5.1/test/test_marker.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    33568 2023-03-09 18:17:16.000000 tuneflow-py-0.5.1/test/test_midi_clip.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    24300 2023-02-22 00:33:25.000000 tuneflow-py-0.5.1/test/test_note.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    14091 2023-03-31 16:54:59.000000 tuneflow-py-0.5.1/test/test_song.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     3583 2023-03-31 08:05:14.000000 tuneflow-py-0.5.1/test/test_track.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2071 2023-02-16 23:10:13.000000 tuneflow-py-0.5.1/test/test_utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-16 21:26:52.732991 tuneflow-py-0.6.0/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1065 2023-01-10 14:03:44.000000 tuneflow-py-0.6.0/LICENSE
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-04-16 21:26:52.732991 tuneflow-py-0.6.0/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     3809 2023-03-06 23:39:23.000000 tuneflow-py-0.6.0/README.md
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1288 2023-04-16 21:26:20.000000 tuneflow-py-0.6.0/pyproject.toml
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-04-16 21:26:52.732991 tuneflow-py-0.6.0/setup.cfg
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-16 21:26:52.722991 tuneflow-py-0.6.0/src/
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-16 21:26:52.722991 tuneflow-py-0.6.0/src/tuneflow_py/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1155 2023-04-10 06:26:06.000000 tuneflow-py-0.6.0/src/tuneflow_py/__init__.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1987 2023-02-28 00:04:43.000000 tuneflow-py-0.6.0/src/tuneflow_py/base_plugin.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-16 21:26:52.722991 tuneflow-py-0.6.0/src/tuneflow_py/descriptors/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      922 2023-03-30 21:40:36.000000 tuneflow-py-0.6.0/src/tuneflow_py/descriptors/audio_plugin_descriptor.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1857 2023-04-16 06:53:45.000000 tuneflow-py-0.6.0/src/tuneflow_py/descriptors/clip_descriptor.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      439 2023-03-30 21:53:05.000000 tuneflow-py-0.6.0/src/tuneflow_py/descriptors/common.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4221 2023-03-30 21:53:07.000000 tuneflow-py-0.6.0/src/tuneflow_py/descriptors/param.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4407 2023-03-30 21:53:10.000000 tuneflow-py-0.6.0/src/tuneflow_py/descriptors/plugin.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       71 2023-03-30 21:53:12.000000 tuneflow-py-0.6.0/src/tuneflow_py/descriptors/text.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     5575 2023-03-31 22:25:01.000000 tuneflow-py-0.6.0/src/tuneflow_py/descriptors/widget.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-16 21:26:52.722991 tuneflow-py-0.6.0/src/tuneflow_py/models/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     3128 2023-03-01 03:02:02.000000 tuneflow-py-0.6.0/src/tuneflow_py/models/audio_plugin.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    17158 2023-03-31 07:33:41.000000 tuneflow-py-0.6.0/src/tuneflow_py/models/automation.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    33694 2023-04-16 21:13:50.000000 tuneflow-py-0.6.0/src/tuneflow_py/models/clip.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1305 2023-04-10 18:15:27.000000 tuneflow-py-0.6.0/src/tuneflow_py/models/marker.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     5275 2023-02-22 00:50:28.000000 tuneflow-py-0.6.0/src/tuneflow_py/models/note.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-16 21:26:52.722991 tuneflow-py-0.6.0/src/tuneflow_py/models/protos/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    71614 2023-04-15 03:58:44.000000 tuneflow-py-0.6.0/src/tuneflow_py/models/protos/song_pb2.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    25607 2023-04-10 18:24:50.000000 tuneflow-py-0.6.0/src/tuneflow_py/models/song.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      873 2023-03-01 22:09:14.000000 tuneflow-py-0.6.0/src/tuneflow_py/models/tempo.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1093 2023-02-22 00:28:50.000000 tuneflow-py-0.6.0/src/tuneflow_py/models/time_signature.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    16387 2023-03-31 16:53:25.000000 tuneflow-py-0.6.0/src/tuneflow_py/models/track.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     6210 2023-03-29 01:48:05.000000 tuneflow-py-0.6.0/src/tuneflow_py/utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-16 21:26:52.722991 tuneflow-py-0.6.0/src/tuneflow_py.egg-info/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-04-16 21:26:52.000000 tuneflow-py-0.6.0/src/tuneflow_py.egg-info/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1113 2023-04-16 21:26:52.000000 tuneflow-py-0.6.0/src/tuneflow_py.egg-info/SOURCES.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-04-16 21:26:52.000000 tuneflow-py-0.6.0/src/tuneflow_py.egg-info/dependency_links.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       96 2023-04-16 21:26:52.000000 tuneflow-py-0.6.0/src/tuneflow_py.egg-info/requires.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       12 2023-04-16 21:26:52.000000 tuneflow-py-0.6.0/src/tuneflow_py.egg-info/top_level.txt
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-16 21:26:52.732991 tuneflow-py-0.6.0/test/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    26849 2023-04-16 07:54:00.000000 tuneflow-py-0.6.0/test/test_audio_clip.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    24170 2023-03-31 07:02:16.000000 tuneflow-py-0.6.0/test/test_automation.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     8001 2023-04-10 18:37:18.000000 tuneflow-py-0.6.0/test/test_marker.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    33568 2023-03-09 18:17:16.000000 tuneflow-py-0.6.0/test/test_midi_clip.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    24300 2023-02-22 00:33:25.000000 tuneflow-py-0.6.0/test/test_note.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    14091 2023-03-31 16:54:59.000000 tuneflow-py-0.6.0/test/test_song.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     3583 2023-03-31 08:05:14.000000 tuneflow-py-0.6.0/test/test_track.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2071 2023-02-16 23:10:13.000000 tuneflow-py-0.6.0/test/test_utils.py
```

### Comparing `tuneflow-py-0.5.1/LICENSE` & `tuneflow-py-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.1/PKG-INFO` & `tuneflow-py-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-py
-Version: 0.5.1
+Version: 0.6.0
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: TuneFlow <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-py-0.5.1/README.md` & `tuneflow-py-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.1/pyproject.toml` & `tuneflow-py-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "tuneflow-py"
-version = "0.5.1"
+version = "0.6.0"
 authors = [{ name = "TuneFlow", email = "contact@info.tuneflow.com" }]
 description = "Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = [
   "AI",
   "music",
```

### Comparing `tuneflow-py-0.5.1/src/tuneflow_py/__init__.py` & `tuneflow-py-0.6.0/src/tuneflow_py/__init__.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.1/src/tuneflow_py/base_plugin.py` & `tuneflow-py-0.6.0/src/tuneflow_py/base_plugin.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.1/src/tuneflow_py/descriptors/audio_plugin_descriptor.py` & `tuneflow-py-0.6.0/src/tuneflow_py/descriptors/audio_plugin_descriptor.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.1/src/tuneflow_py/descriptors/clip_descriptor.py` & `tuneflow-py-0.6.0/src/tuneflow_py/descriptors/clip_descriptor.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,7 +46,17 @@
     '''
     The duration of the audio content. You can get this value in the plugin
     by using `readApis.readAudioBuffer` to read the audio file content as `AudioBuffer`, and then
     get the duration from `audioBuffer.duration`.
     
     Duration needs to be updated whenever audio file (path or content) changes.
     '''
+
+    speed_ratio: NotRequired[float]
+    '''
+    How fast this audio plays, time-stretch is applied when this ratio is set and not 1, default to 1.
+    '''
+
+    pitch_offset: NotRequired[float]
+    '''
+    Pitch offset in semitones, ranging from -48 to 48, default to 0.
+    '''
```

### Comparing `tuneflow-py-0.5.1/src/tuneflow_py/descriptors/param.py` & `tuneflow-py-0.6.0/src/tuneflow_py/descriptors/param.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.1/src/tuneflow_py/descriptors/plugin.py` & `tuneflow-py-0.6.0/src/tuneflow_py/descriptors/plugin.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.1/src/tuneflow_py/descriptors/widget.py` & `tuneflow-py-0.6.0/src/tuneflow_py/descriptors/widget.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.1/src/tuneflow_py/models/audio_plugin.py` & `tuneflow-py-0.6.0/src/tuneflow_py/models/audio_plugin.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.1/src/tuneflow_py/models/automation.py` & `tuneflow-py-0.6.0/src/tuneflow_py/models/automation.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.1/src/tuneflow_py/models/clip.py` & `tuneflow-py-0.6.0/src/tuneflow_py/models/clip.py`

 * *Files 26% similar despite different names*

```diff
@@ -44,14 +44,18 @@
             if "audio_file_path" in audio_clip_data and audio_clip_data["audio_file_path"] is not None and audio_clip_data["audio_file_path"] != "":
                 self._proto.audio_clip_data.audio_file_path = audio_clip_data["audio_file_path"]
             if "audio_data" in audio_clip_data and audio_clip_data["audio_data"] is not None:
                 self._proto.audio_clip_data.audio_data.format = audio_clip_data["audio_data"]["format"]
                 self._proto.audio_clip_data.audio_data.data = audio_clip_data["audio_data"]["data"]
             self._proto.audio_clip_data.start_tick = audio_clip_data["start_tick"]
             self._proto.audio_clip_data.duration = audio_clip_data["duration"]
+            if "pitch_offset" in audio_clip_data:
+                self._proto.audio_clip_data.pitch_offset = audio_clip_data["pitch_offset"]
+            if "speed_ratio" in audio_clip_data:
+                self._proto.audio_clip_data.speed_ratio = audio_clip_data["speed_ratio"]
 
             clip_start_tick = max(
                 clip_start_tick, audio_clip_data["start_tick"]) if clip_start_tick is not None else audio_clip_data["start_tick"]
             audio_end_tick = self.get_audio_end_tick()
             if (clip_end_tick is None or audio_end_tick < clip_end_tick):  # type:ignore
                 clip_end_tick = audio_end_tick
 
@@ -85,28 +89,224 @@
             return None
 
         audio_start_time = self.song.tick_to_seconds(
             self._proto.audio_clip_data.start_tick)
         return self.song.seconds_to_tick(audio_start_time + duration)
 
     def get_duration(self):
+        '''
+        Duration from the clip start to clip end, in seconds.
+        '''
         return self.song.tick_to_seconds(
             self.get_clip_end_tick()) - self.song.tick_to_seconds(
             self.get_clip_start_tick())
 
     def get_audio_duration(self) -> float | None:
         '''
-        Gets the audio's duration if the clip is AUDIO_CLIP.
+        Gets the STRETCHED, FULL audio duration if the clip is AUDIO_CLIP, this takes speed ratio into consideration.
 
         Returns None if the clip is not AUDIO_CLIP or audio clip data is missing.
         '''
         if self.get_type() != ClipType.AUDIO_CLIP or not self.has_audio_clip_data():
             return None
+        return self._proto.audio_clip_data.duration / self.get_audio_speed_ratio()
+
+    def get_raw_audio_duration(self) -> float | None:
+        '''
+        Gets the UNSTRETCHED, FULL audio duration if the clip is AUDIO_CLIP, this DOES NOT consider speed ratio.
+
+        Returns undefined if the clip is not AUDIO_CLIP or audio clip data is missing.
+        '''
+        if self.get_type() != ClipType.AUDIO_CLIP or not self.has_audio_clip_data():
+            return None
         return self._proto.audio_clip_data.duration
 
+    def get_audio_speed_ratio(self) -> float:
+        if self.get_type() != ClipType.AUDIO_CLIP or not self.has_audio_clip_data() or self._proto.audio_clip_data.speed_ratio is None or self._proto.audio_clip_data.speed_ratio == 0:
+            return 1
+        return self._proto.audio_clip_data.speed_ratio
+
+    def time_stretch_from_clip_left(self, to_left_tick: int, resolve_clip_conflict=True):
+        '''
+        Time-stretch the clip by adjusting the start tick of the clip.
+
+        NOTE: This could delete the clip if the clip range becomes empty after
+        this call.
+
+        @param `to_left_tick` The new start tick to stretch the clip to.
+        '''
+        if (to_left_tick >= self.get_clip_end_tick()):
+            self.delete_from_parent(delete_associated_track_automation=True)
+            return
+        stretch_factor = (self.get_clip_end_tick(
+        ) - to_left_tick) / (self.get_clip_end_tick() - self.get_clip_start_tick())
+        # Resolve conflict before changing the clip's range
+        # to preserve the current order of clips.
+        if (resolve_clip_conflict and self.track is not None):
+            self.track._resolve_clip_conflict(
+                self.get_id(),
+                min(self.get_clip_start_tick(), to_left_tick),
+                self.get_clip_end_tick(),
+            )
+
+        if self.get_type() == ClipType.MIDI_CLIP:
+            self._time_stretch_midi_clip(stretch_factor=stretch_factor, reference_tick=self.get_clip_end_tick())
+            self.move_clip_to(to_left_tick, move_associated_track_automation_points=False)
+        elif (self.get_type() == ClipType.AUDIO_CLIP):
+            self._time_stretch_audio_clip(to_left_tick, self.get_clip_end_tick(), self.get_clip_end_tick())
+        # TODO: Scale the associated automation points accordingly.
+
+    def time_stretch_from_clip_right(self, to_right_tick: int, resolve_clip_conflict=True):
+        '''
+        Time-stretch the clip by adjusting the end tick of the clip.
+
+        NOTE: This could delete the clip if the range becomes empty after
+        this call.
+        @param to_right_tick The new end tick to stretch the clip to.
+        '''
+        if (to_right_tick <= self.get_clip_start_tick()):
+            self.delete_from_parent(delete_associated_track_automation=True)
+            return
+
+        # Resolve conflict before changing the clip's range
+        # to preserve the current order of clips.
+        if resolve_clip_conflict and self.track:
+            self.track._resolve_clip_conflict(
+                self.get_id(),
+                self.get_clip_start_tick(),
+                max(self.get_clip_end_tick(), to_right_tick),
+            )
+
+        if (self.get_type() == ClipType.MIDI_CLIP):
+            stretch_factor = (to_right_tick - self.get_clip_start_tick()
+                              ) / (self.get_clip_end_tick() - self.get_clip_start_tick())
+            self._time_stretch_midi_clip(stretch_factor=stretch_factor, reference_tick=self.get_clip_start_tick())
+        elif (self.get_type() == ClipType.AUDIO_CLIP):
+            self._time_stretch_audio_clip(self.get_clip_start_tick(), to_right_tick, self.get_clip_start_tick())
+
+        # TODO: Scale the associated automation points accordingly.
+
+    def _time_stretch_midi_clip(self, stretch_factor: float, reference_tick: int):
+        for note in self.get_raw_notes():
+            note.set_start_tick(
+                Clip._calculate_scaled_new_tick(
+                    note.get_start_tick(),
+                    reference_tick, stretch_factor))
+            note.set_end_tick(
+                Clip._calculate_scaled_new_tick(
+                    note.get_end_tick(),
+                    reference_tick, stretch_factor))
+
+        self._proto.clip_start_tick = Clip._calculate_scaled_new_tick(
+            self.get_clip_start_tick(),
+            reference_tick,
+            stretch_factor,
+        )
+        self._proto.clip_end_tick = Clip._calculate_scaled_new_tick(
+            self.get_clip_end_tick(), reference_tick, stretch_factor)
+
+    def _time_stretch_audio_clip(
+            self,
+        new_left_tick: int,
+        new_right_tick: int,
+        reference_tick: int,
+    ):
+        if (self.get_type() != ClipType.AUDIO_CLIP):
+            return
+
+        audio_clip_data = self.get_audio_clip_data()
+        if (audio_clip_data is None):
+            raise Exception(f"Audio clip data is missing for audio clip {self.get_id()}")
+        old_speed_ratio = audio_clip_data.speed_ratio if audio_clip_data.speed_ratio is not None and audio_clip_data.speed_ratio > 0 else 1
+        old_duratoin = self.song.tick_to_seconds(
+            self.get_clip_end_tick()) - self.song.tick_to_seconds(self.get_clip_start_tick())
+        new_duration = self.song.tick_to_seconds(new_right_tick) - self.song.tick_to_seconds(new_left_tick)
+        time_stretch_factor = new_duration / old_duratoin
+        speed_ratio = old_speed_ratio / time_stretch_factor
+        Clip.validate_audio_speed_ratio(speed_ratio)
+        old_audio_start_time = self.song.tick_to_seconds(audio_clip_data.start_tick)
+        reference_tick_time = self.song.tick_to_seconds(reference_tick)
+        new_audio_start_to_reference_distance_in_time = (
+            reference_tick_time - old_audio_start_time) * time_stretch_factor
+        new_audio_start_time = reference_tick_time - new_audio_start_to_reference_distance_in_time
+        new_audio_start_tick = self.song.seconds_to_tick(new_audio_start_time)
+        audio_clip_data.speed_ratio = speed_ratio
+        audio_clip_data.start_tick = new_audio_start_tick
+        self._proto.clip_start_tick = new_left_tick
+        self._proto.clip_end_tick = new_right_tick
+
+    @staticmethod
+    def validate_audio_speed_ratio(speed_ratio: float):
+        if (
+            speed_ratio is None or
+            speed_ratio < Clip.MIN_AUDIO_SPEED_RATIO or
+            speed_ratio > Clip.MAX_AUDIO_SPEED_RATIO
+        ):
+            raise Exception(
+                f'Speed ratio must be >= {Clip.MIN_AUDIO_SPEED_RATIO} and <= {Clip.MAX_AUDIO_SPEED_RATIO}, you are changing to {speed_ratio}',
+            )
+
+    @staticmethod
+    def _calculate_scaled_new_tick(
+        old_tick: int,
+        reference_tick: int,
+        scale_factor: float,
+    ):
+        distance = (reference_tick - old_tick) * scale_factor
+        return round(reference_tick - distance)
+
+    def get_audio_pitch_offset(self):
+        '''
+        @returns The pitch offset of this audio in semitones, comparing to the raw audio.
+        '''
+        if (
+            self.get_type() != ClipType.AUDIO_CLIP or
+            not self.has_audio_clip_data() or
+            self.get_audio_clip_data().pitch_offset is None  # type: ignore
+        ):
+            return 0
+        return self.get_audio_clip_data().pitch_offset  # type: ignore
+
+    def set_audio_pitch_offset(self, offset_in_semitones: float):
+        '''
+        Sets the pitch offset of this audio in semitones, the offset is compared to the raw audio.
+        * @param offset_in_semitones Ranging from `Clip.MIN_AUDIO_PITCH_OFFSET` to `Clip.MAX_AUDIO_PITCH_OFFSET`, step 1, inclusive.
+        * @returns
+        '''
+        if (self.get_type() != ClipType.AUDIO_CLIP):
+            return
+
+        Clip.validate_audio_pitch_offset(offset_in_semitones)
+        self.get_audio_clip_data().pitch_offset = offset_in_semitones  # type: ignore
+
+    @staticmethod
+    def validate_audio_pitch_offset(offset_in_semitones: float):
+        if (
+            offset_in_semitones is None or
+            offset_in_semitones < Clip.MIN_AUDIO_PITCH_OFFSET or
+            offset_in_semitones > Clip.MAX_AUDIO_PITCH_OFFSET
+        ):
+            raise Exception(
+                f'Pitch offset must be >= {Clip.MIN_AUDIO_PITCH_OFFSET} and <= {Clip.MAX_AUDIO_PITCH_OFFSET}, you are setting to {offset_in_semitones}',
+            )
+
+    def get_audio_start_tick(self):
+        '''
+        Gets the current clip audio's start tick.
+
+        Note that this differs from the clip's start tick in that the user can trim
+        the clip to only play part of the audio.
+
+        Returns None if the clip is not audio clip or audio clip data is missing.
+        '''
+        if (self.get_type() != ClipType.AUDIO_CLIP or not self.has_audio_clip_data()):
+            return None
+
+        return self.get_audio_clip_data().start_tick  # type: ignore
+
     def get_raw_note_count(self):
         return len(self._proto.notes)
 
     def get_raw_notes(self):
         '''
         @returns All notes contained by the clip, including those that
         are not within the clip's range.
@@ -191,19 +391,29 @@
 
     def get_clip_end_tick(self) -> int:
         return self._proto.clip_end_tick
 
     def has_audio_clip_data(self) -> bool:
         return self._proto.HasField("audio_clip_data")
 
-    def get_audio_clip_data(self):
+    def get_audio_clip_data(self) -> AudioClipData | None:
         if not self.has_audio_clip_data():
             return None
         return self._proto.audio_clip_data
 
+    def set_audio_file(self, file_path: str, start_tick: int, duration: float):
+        '''
+        Sets a new audio file.
+        '''
+        self._proto.audio_clip_data.audio_file_path = file_path
+        self._proto.audio_clip_data.start_tick = start_tick
+        self._proto.audio_clip_data.duration = duration
+        self._proto.audio_clip_data.speed_ratio = 1
+        self._proto.audio_clip_data.pitch_offset = 0
+
     def clear_notes(self):
         del self._proto.notes[:]
 
     def delete_from_parent(self, delete_associated_track_automation: bool):
         if self.track is not None:
             self.track.delete_clip(self, delete_associated_track_automation)
             self.track = None
@@ -579,7 +789,12 @@
             note_start_tick < clip_end_tick and
             note_end_tick > note_start_tick
         )
 
     @staticmethod
     def _generate_clip_id():
         return generate_nanoid(size=10)
+
+    MIN_AUDIO_SPEED_RATIO = 0.05
+    MAX_AUDIO_SPEED_RATIO = 20
+    MIN_AUDIO_PITCH_OFFSET = -24
+    MAX_AUDIO_PITCH_OFFSET = 24
```

### Comparing `tuneflow-py-0.5.1/src/tuneflow_py/models/marker.py` & `tuneflow-py-0.6.0/src/tuneflow_py/models/marker.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.1/src/tuneflow_py/models/note.py` & `tuneflow-py-0.6.0/src/tuneflow_py/models/note.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.1/src/tuneflow_py/models/protos/song_pb2.py` & `tuneflow-py-0.6.0/src/tuneflow_py/models/protos/song_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='song.proto',
   package='song',
   syntax='proto2',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\nsong.proto\x12\x04song\"\x7f\n\x04Note\x12\r\n\x05pitch\x18\x01 \x01(\x05\x12\x10\n\x08velocity\x18\x02 \x01(\x05\x12\x12\n\nstart_tick\x18\x03 \x01(\x05\x12\x12\n\nstart_time\x18\x04 \x01(\x02\x12\x10\n\x08\x65nd_tick\x18\x05 \x01(\x05\x12\x10\n\x08\x65nd_time\x18\x06 \x01(\x02\x12\n\n\x02id\x18\x07 \x01(\r\"6\n\nTempoEvent\x12\r\n\x05ticks\x18\x01 \x01(\x05\x12\x0b\n\x03\x62pm\x18\x02 \x01(\x02\x12\x0c\n\x04time\x18\x03 \x01(\x02\"K\n\x12TimeSignatureEvent\x12\r\n\x05ticks\x18\x01 \x01(\x05\x12\x11\n\tnumerator\x18\x02 \x01(\x05\x12\x13\n\x0b\x64\x65nominator\x18\x03 \x01(\x05\"2\n\x0eInstrumentInfo\x12\x0f\n\x07program\x18\x01 \x01(\x05\x12\x0f\n\x07is_drum\x18\x02 \x01(\x08\"f\n\x0f\x41udioPluginInfo\x12\r\n\x05tf_id\x18\x01 \x01(\t\x12\x12\n\nis_enabled\x18\x02 \x01(\x08\x12\x19\n\x11local_instance_id\x18\x03 \x01(\t\x12\x15\n\rbase64_states\x18\x04 \x01(\t\"\xb2\x01\n\x10\x41utomationTarget\x12/\n\x04type\x18\x01 \x01(\x0e\x32!.song.AutomationTarget.TargetType\x12\x17\n\x0f\x61udio_plugin_id\x18\x02 \x01(\t\x12\x10\n\x08param_id\x18\x03 \x01(\t\"B\n\nTargetType\x12\r\n\tUNDEFINED\x10\x00\x12\n\n\x06VOLUME\x10\x01\x12\x07\n\x03PAN\x10\x02\x12\x10\n\x0c\x41UDIO_PLUGIN\x10\x03\"\x8c\x01\n\x0f\x41utomationValue\x12\x30\n\x06points\x18\x01 \x03(\x0b\x32 .song.AutomationValue.ParamValue\x12\x10\n\x08\x64isabled\x18\x02 \x01(\x08\x1a\x35\n\nParamValue\x12\x0c\n\x04tick\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x02\x12\n\n\x02id\x18\x03 \x01(\x05\"\xc4\x01\n\x0e\x41utomationData\x12\'\n\x07targets\x18\x01 \x03(\x0b\x32\x16.song.AutomationTarget\x12=\n\rtarget_values\x18\x02 \x03(\x0b\x32&.song.AutomationData.TargetValuesEntry\x1aJ\n\x11TargetValuesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.song.AutomationValue:\x02\x38\x01\"\xef\x01\n\tTrackSend\x12\x17\n\x0foutput_bus_rank\x18\x01 \x01(\x05\x12\x12\n\ngain_level\x18\x02 \x01(\x02\x12\x33\n\x08position\x18\x03 \x01(\x0e\x32!.song.TrackSend.TrackSendPosition\x12\r\n\x05muted\x18\x04 \x01(\x08\"q\n\x11TrackSendPosition\x12!\n\x1dUNDEFINED_TRACK_SEND_POSITION\x10\x00\x12\x1b\n\x17SEND_POSITION_PRE_FADER\x10\x01\x12\x1c\n\x18SEND_POSITION_POST_FADER\x10\x02\"\xca\x01\n\x0bTrackOutput\x12/\n\x04type\x18\x01 \x01(\x0e\x32!.song.TrackOutput.TrackOutputType\x12\x10\n\x08track_id\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65vice_name\x18\x03 \x01(\t\"c\n\x0fTrackOutputType\x12\x1f\n\x1bUNDEFINED_TRACK_OUTPUT_TYPE\x10\x00\x12\x17\n\x13TRACK_OUTPUT_DEVICE\x10\x01\x12\x16\n\x12TRACK_OUTPUT_TRACK\x10\x02\"&\n\x0c\x41uxTrackData\x12\x16\n\x0einput_bus_rank\x18\x01 \x01(\x05\"\xe2\x05\n\x05Track\x12(\n\ninstrument\x18\x01 \x01(\x0b\x32\x14.song.InstrumentInfo\x12\x1d\n\x05notes\x18\x02 \x03(\x0b\x32\n.song.NoteB\x02\x18\x01\x12\x33\n\x15suggested_instruments\x18\x03 \x03(\x0b\x32\x14.song.InstrumentInfo\x12\x0c\n\x04uuid\x18\x04 \x01(\t\x12\x0e\n\x06volume\x18\x05 \x01(\x02\x12\x0c\n\x04solo\x18\x06 \x01(\x08\x12\r\n\x05muted\x18\x07 \x01(\x08\x12\x0c\n\x04rank\x18\x08 \x01(\x05\x12\x18\n\x10track_start_tick\x18\t \x01(\x05\x12\x16\n\x0etrack_end_tick\x18\n \x01(\x05\x12-\n\x0esampler_plugin\x18\x0b \x01(\x0b\x32\x15.song.AudioPluginInfo\x12\x32\n\x0c\x61udio_plugin\x18\x0c \x03(\x0b\x32\x1c.song.Track.AudioPluginEntry\x12\x19\n\x05\x63lips\x18\r \x03(\x0b\x32\n.song.Clip\x12\x0b\n\x03pan\x18\x0e \x01(\x05\x12\x0c\n\x04name\x18\x0f \x01(\t\x12(\n\nautomation\x18\x10 \x01(\x0b\x32\x14.song.AutomationData\x12\x1d\n\x04type\x18\x11 \x01(\x0e\x32\x0f.song.TrackType\x12*\n\x0e\x61ux_track_data\x18\x12 \x01(\x0b\x32\x12.song.AuxTrackData\x12%\n\x05sends\x18\x13 \x03(\x0b\x32\x16.song.Track.SendsEntry\x12!\n\x06output\x18\x14 \x01(\x0b\x32\x11.song.TrackOutput\x1aI\n\x10\x41udioPluginEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.song.AudioPluginInfo:\x02\x38\x01\x1a=\n\nSendsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.song.TrackSend:\x02\x38\x01\")\n\tAudioData\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12\x0e\n\x06\x66ormat\x18\x02 \x01(\t\"s\n\rAudioClipData\x12\x17\n\x0f\x61udio_file_path\x18\x01 \x01(\t\x12\x12\n\nstart_tick\x18\x02 \x01(\x05\x12\x10\n\x08\x64uration\x18\x03 \x01(\x01\x12#\n\naudio_data\x18\x04 \x01(\x0b\x32\x0f.song.AudioData\"\xb7\x01\n\x04\x43lip\x12\n\n\x02id\x18\x01 \x01(\t\x12\x17\n\x0f\x63lip_start_tick\x18\x02 \x01(\x05\x12\x15\n\rclip_end_tick\x18\x03 \x01(\x05\x12\x19\n\x05notes\x18\x04 \x03(\x0b\x32\n.song.Note\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x1c\n\x04type\x18\x06 \x01(\x0e\x32\x0e.song.ClipType\x12,\n\x0f\x61udio_clip_data\x18\x07 \x01(\x0b\x32\x13.song.AudioClipData\"\xf6\x01\n\x0fStructureMarker\x12\x0c\n\x04tick\x18\x01 \x01(\x05\x12\x31\n\x04type\x18\x02 \x01(\x0e\x32#.song.StructureMarker.StructureType\x12\x13\n\x0b\x63ustom_name\x18\x03 \x01(\t\"\x8c\x01\n\rStructureType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05INTRO\x10\x01\x12\t\n\x05VERSE\x10\x02\x12\n\n\x06\x43HORUS\x10\x03\x12\n\n\x06\x42RIDGE\x10\x04\x12\t\n\x05OUTRO\x10\x05\x12\x0e\n\nPRE_CHORUS\x10\x06\x12\x0f\n\x0bPOST_CHORUS\x10\x07\x12\x08\n\x04\x46ILL\x10\x08\x12\n\n\x06\x43USTOM\x10\t\"!\n\x03\x42us\x12\x0c\n\x04rank\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x92\x02\n\x04Song\x12\x0b\n\x03PPQ\x18\x01 \x01(\x05\x12 \n\x06tempos\x18\x02 \x03(\x0b\x32\x10.song.TempoEvent\x12\x31\n\x0ftime_signatures\x18\x03 \x03(\x0b\x32\x18.song.TimeSignatureEvent\x12\x11\n\tlast_tick\x18\x04 \x01(\x05\x12\x10\n\x08\x64uration\x18\x05 \x01(\x02\x12\x1b\n\x06tracks\x18\x06 \x03(\x0b\x32\x0b.song.Track\x12!\n\x0cmaster_track\x18\x07 \x01(\x0b\x32\x0b.song.Track\x12)\n\nstructures\x18\x08 \x03(\x0b\x32\x15.song.StructureMarker\x12\x18\n\x05\x62uses\x18\t \x03(\x0b\x32\t.song.Bus*b\n\tTrackType\x12\x13\n\x0fUNDEFINED_TRACK\x10\x00\x12\x0e\n\nMIDI_TRACK\x10\x01\x12\x0f\n\x0b\x41UDIO_TRACK\x10\x02\x12\x10\n\x0cMASTER_TRACK\x10\x03\x12\r\n\tAUX_TRACK\x10\x04*=\n\x08\x43lipType\x12\x12\n\x0eUNDEFINED_CLIP\x10\x00\x12\r\n\tMIDI_CLIP\x10\x01\x12\x0e\n\nAUDIO_CLIP\x10\x02'
+  serialized_pb=b'\n\nsong.proto\x12\x04song\"\x7f\n\x04Note\x12\r\n\x05pitch\x18\x01 \x01(\x05\x12\x10\n\x08velocity\x18\x02 \x01(\x05\x12\x12\n\nstart_tick\x18\x03 \x01(\x05\x12\x12\n\nstart_time\x18\x04 \x01(\x02\x12\x10\n\x08\x65nd_tick\x18\x05 \x01(\x05\x12\x10\n\x08\x65nd_time\x18\x06 \x01(\x02\x12\n\n\x02id\x18\x07 \x01(\r\"6\n\nTempoEvent\x12\r\n\x05ticks\x18\x01 \x01(\x05\x12\x0b\n\x03\x62pm\x18\x02 \x01(\x02\x12\x0c\n\x04time\x18\x03 \x01(\x02\"K\n\x12TimeSignatureEvent\x12\r\n\x05ticks\x18\x01 \x01(\x05\x12\x11\n\tnumerator\x18\x02 \x01(\x05\x12\x13\n\x0b\x64\x65nominator\x18\x03 \x01(\x05\"2\n\x0eInstrumentInfo\x12\x0f\n\x07program\x18\x01 \x01(\x05\x12\x0f\n\x07is_drum\x18\x02 \x01(\x08\"f\n\x0f\x41udioPluginInfo\x12\r\n\x05tf_id\x18\x01 \x01(\t\x12\x12\n\nis_enabled\x18\x02 \x01(\x08\x12\x19\n\x11local_instance_id\x18\x03 \x01(\t\x12\x15\n\rbase64_states\x18\x04 \x01(\t\"\xb2\x01\n\x10\x41utomationTarget\x12/\n\x04type\x18\x01 \x01(\x0e\x32!.song.AutomationTarget.TargetType\x12\x17\n\x0f\x61udio_plugin_id\x18\x02 \x01(\t\x12\x10\n\x08param_id\x18\x03 \x01(\t\"B\n\nTargetType\x12\r\n\tUNDEFINED\x10\x00\x12\n\n\x06VOLUME\x10\x01\x12\x07\n\x03PAN\x10\x02\x12\x10\n\x0c\x41UDIO_PLUGIN\x10\x03\"\x8c\x01\n\x0f\x41utomationValue\x12\x30\n\x06points\x18\x01 \x03(\x0b\x32 .song.AutomationValue.ParamValue\x12\x10\n\x08\x64isabled\x18\x02 \x01(\x08\x1a\x35\n\nParamValue\x12\x0c\n\x04tick\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x02\x12\n\n\x02id\x18\x03 \x01(\x05\"\xc4\x01\n\x0e\x41utomationData\x12\'\n\x07targets\x18\x01 \x03(\x0b\x32\x16.song.AutomationTarget\x12=\n\rtarget_values\x18\x02 \x03(\x0b\x32&.song.AutomationData.TargetValuesEntry\x1aJ\n\x11TargetValuesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.song.AutomationValue:\x02\x38\x01\"\xef\x01\n\tTrackSend\x12\x17\n\x0foutput_bus_rank\x18\x01 \x01(\x05\x12\x12\n\ngain_level\x18\x02 \x01(\x02\x12\x33\n\x08position\x18\x03 \x01(\x0e\x32!.song.TrackSend.TrackSendPosition\x12\r\n\x05muted\x18\x04 \x01(\x08\"q\n\x11TrackSendPosition\x12!\n\x1dUNDEFINED_TRACK_SEND_POSITION\x10\x00\x12\x1b\n\x17SEND_POSITION_PRE_FADER\x10\x01\x12\x1c\n\x18SEND_POSITION_POST_FADER\x10\x02\"\xca\x01\n\x0bTrackOutput\x12/\n\x04type\x18\x01 \x01(\x0e\x32!.song.TrackOutput.TrackOutputType\x12\x10\n\x08track_id\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65vice_name\x18\x03 \x01(\t\"c\n\x0fTrackOutputType\x12\x1f\n\x1bUNDEFINED_TRACK_OUTPUT_TYPE\x10\x00\x12\x17\n\x13TRACK_OUTPUT_DEVICE\x10\x01\x12\x16\n\x12TRACK_OUTPUT_TRACK\x10\x02\"&\n\x0c\x41uxTrackData\x12\x16\n\x0einput_bus_rank\x18\x01 \x01(\x05\"\xe2\x05\n\x05Track\x12(\n\ninstrument\x18\x01 \x01(\x0b\x32\x14.song.InstrumentInfo\x12\x1d\n\x05notes\x18\x02 \x03(\x0b\x32\n.song.NoteB\x02\x18\x01\x12\x33\n\x15suggested_instruments\x18\x03 \x03(\x0b\x32\x14.song.InstrumentInfo\x12\x0c\n\x04uuid\x18\x04 \x01(\t\x12\x0e\n\x06volume\x18\x05 \x01(\x02\x12\x0c\n\x04solo\x18\x06 \x01(\x08\x12\r\n\x05muted\x18\x07 \x01(\x08\x12\x0c\n\x04rank\x18\x08 \x01(\x05\x12\x18\n\x10track_start_tick\x18\t \x01(\x05\x12\x16\n\x0etrack_end_tick\x18\n \x01(\x05\x12-\n\x0esampler_plugin\x18\x0b \x01(\x0b\x32\x15.song.AudioPluginInfo\x12\x32\n\x0c\x61udio_plugin\x18\x0c \x03(\x0b\x32\x1c.song.Track.AudioPluginEntry\x12\x19\n\x05\x63lips\x18\r \x03(\x0b\x32\n.song.Clip\x12\x0b\n\x03pan\x18\x0e \x01(\x05\x12\x0c\n\x04name\x18\x0f \x01(\t\x12(\n\nautomation\x18\x10 \x01(\x0b\x32\x14.song.AutomationData\x12\x1d\n\x04type\x18\x11 \x01(\x0e\x32\x0f.song.TrackType\x12*\n\x0e\x61ux_track_data\x18\x12 \x01(\x0b\x32\x12.song.AuxTrackData\x12%\n\x05sends\x18\x13 \x03(\x0b\x32\x16.song.Track.SendsEntry\x12!\n\x06output\x18\x14 \x01(\x0b\x32\x11.song.TrackOutput\x1aI\n\x10\x41udioPluginEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.song.AudioPluginInfo:\x02\x38\x01\x1a=\n\nSendsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.song.TrackSend:\x02\x38\x01\")\n\tAudioData\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12\x0e\n\x06\x66ormat\x18\x02 \x01(\t\"\x9e\x01\n\rAudioClipData\x12\x17\n\x0f\x61udio_file_path\x18\x01 \x01(\t\x12\x12\n\nstart_tick\x18\x02 \x01(\x05\x12\x10\n\x08\x64uration\x18\x03 \x01(\x01\x12#\n\naudio_data\x18\x04 \x01(\x0b\x32\x0f.song.AudioData\x12\x13\n\x0bspeed_ratio\x18\x05 \x01(\x01\x12\x14\n\x0cpitch_offset\x18\x06 \x01(\x01\"\xb7\x01\n\x04\x43lip\x12\n\n\x02id\x18\x01 \x01(\t\x12\x17\n\x0f\x63lip_start_tick\x18\x02 \x01(\x05\x12\x15\n\rclip_end_tick\x18\x03 \x01(\x05\x12\x19\n\x05notes\x18\x04 \x03(\x0b\x32\n.song.Note\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x1c\n\x04type\x18\x06 \x01(\x0e\x32\x0e.song.ClipType\x12,\n\x0f\x61udio_clip_data\x18\x07 \x01(\x0b\x32\x13.song.AudioClipData\"\xf6\x01\n\x0fStructureMarker\x12\x0c\n\x04tick\x18\x01 \x01(\x05\x12\x31\n\x04type\x18\x02 \x01(\x0e\x32#.song.StructureMarker.StructureType\x12\x13\n\x0b\x63ustom_name\x18\x03 \x01(\t\"\x8c\x01\n\rStructureType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05INTRO\x10\x01\x12\t\n\x05VERSE\x10\x02\x12\n\n\x06\x43HORUS\x10\x03\x12\n\n\x06\x42RIDGE\x10\x04\x12\t\n\x05OUTRO\x10\x05\x12\x0e\n\nPRE_CHORUS\x10\x06\x12\x0f\n\x0bPOST_CHORUS\x10\x07\x12\x08\n\x04\x46ILL\x10\x08\x12\n\n\x06\x43USTOM\x10\t\"!\n\x03\x42us\x12\x0c\n\x04rank\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x92\x02\n\x04Song\x12\x0b\n\x03PPQ\x18\x01 \x01(\x05\x12 \n\x06tempos\x18\x02 \x03(\x0b\x32\x10.song.TempoEvent\x12\x31\n\x0ftime_signatures\x18\x03 \x03(\x0b\x32\x18.song.TimeSignatureEvent\x12\x11\n\tlast_tick\x18\x04 \x01(\x05\x12\x10\n\x08\x64uration\x18\x05 \x01(\x02\x12\x1b\n\x06tracks\x18\x06 \x03(\x0b\x32\x0b.song.Track\x12!\n\x0cmaster_track\x18\x07 \x01(\x0b\x32\x0b.song.Track\x12)\n\nstructures\x18\x08 \x03(\x0b\x32\x15.song.StructureMarker\x12\x18\n\x05\x62uses\x18\t \x03(\x0b\x32\t.song.Bus*b\n\tTrackType\x12\x13\n\x0fUNDEFINED_TRACK\x10\x00\x12\x0e\n\nMIDI_TRACK\x10\x01\x12\x0f\n\x0b\x41UDIO_TRACK\x10\x02\x12\x10\n\x0cMASTER_TRACK\x10\x03\x12\r\n\tAUX_TRACK\x10\x04*=\n\x08\x43lipType\x12\x12\n\x0eUNDEFINED_CLIP\x10\x00\x12\r\n\tMIDI_CLIP\x10\x01\x12\x0e\n\nAUDIO_CLIP\x10\x02'
 )
 
 _TRACKTYPE = _descriptor.EnumDescriptor(
   name='TrackType',
   full_name='song.TrackType',
   filename=None,
   file=DESCRIPTOR,
@@ -54,16 +54,16 @@
       name='AUX_TRACK', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=3096,
-  serialized_end=3194,
+  serialized_start=3140,
+  serialized_end=3238,
 )
 _sym_db.RegisterEnumDescriptor(_TRACKTYPE)
 
 TrackType = enum_type_wrapper.EnumTypeWrapper(_TRACKTYPE)
 _CLIPTYPE = _descriptor.EnumDescriptor(
   name='ClipType',
   full_name='song.ClipType',
@@ -85,16 +85,16 @@
       name='AUDIO_CLIP', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=3196,
-  serialized_end=3257,
+  serialized_start=3240,
+  serialized_end=3301,
 )
 _sym_db.RegisterEnumDescriptor(_CLIPTYPE)
 
 ClipType = enum_type_wrapper.EnumTypeWrapper(_CLIPTYPE)
 UNDEFINED_TRACK = 0
 MIDI_TRACK = 1
 AUDIO_TRACK = 2
@@ -256,16 +256,16 @@
       name='CUSTOM', index=9, number=9,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2642,
-  serialized_end=2782,
+  serialized_start=2686,
+  serialized_end=2826,
 )
 _sym_db.RegisterEnumDescriptor(_STRUCTUREMARKER_STRUCTURETYPE)
 
 
 _NOTE = _descriptor.Descriptor(
   name='Note',
   full_name='song.Note',
@@ -1177,28 +1177,42 @@
     _descriptor.FieldDescriptor(
       name='audio_data', full_name='song.AudioClipData.audio_data', index=3,
       number=4, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='speed_ratio', full_name='song.AudioClipData.speed_ratio', index=4,
+      number=5, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='pitch_offset', full_name='song.AudioClipData.pitch_offset', index=5,
+      number=6, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2232,
-  serialized_end=2347,
+  serialized_start=2233,
+  serialized_end=2391,
 )
 
 
 _CLIP = _descriptor.Descriptor(
   name='Clip',
   full_name='song.Clip',
   filename=None,
@@ -1263,16 +1277,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2350,
-  serialized_end=2533,
+  serialized_start=2394,
+  serialized_end=2577,
 )
 
 
 _STRUCTUREMARKER = _descriptor.Descriptor(
   name='StructureMarker',
   full_name='song.StructureMarker',
   filename=None,
@@ -1310,16 +1324,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2536,
-  serialized_end=2782,
+  serialized_start=2580,
+  serialized_end=2826,
 )
 
 
 _BUS = _descriptor.Descriptor(
   name='Bus',
   full_name='song.Bus',
   filename=None,
@@ -1349,16 +1363,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2784,
-  serialized_end=2817,
+  serialized_start=2828,
+  serialized_end=2861,
 )
 
 
 _SONG = _descriptor.Descriptor(
   name='Song',
   full_name='song.Song',
   filename=None,
@@ -1437,16 +1451,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2820,
-  serialized_end=3094,
+  serialized_start=2864,
+  serialized_end=3138,
 )
 
 _AUTOMATIONTARGET.fields_by_name['type'].enum_type = _AUTOMATIONTARGET_TARGETTYPE
 _AUTOMATIONTARGET_TARGETTYPE.containing_type = _AUTOMATIONTARGET
 _AUTOMATIONVALUE_PARAMVALUE.containing_type = _AUTOMATIONVALUE
 _AUTOMATIONVALUE.fields_by_name['points'].message_type = _AUTOMATIONVALUE_PARAMVALUE
 _AUTOMATIONDATA_TARGETVALUESENTRY.fields_by_name['value'].message_type = _AUTOMATIONVALUE
```

### Comparing `tuneflow-py-0.5.1/src/tuneflow_py/models/song.py` & `tuneflow-py-0.6.0/src/tuneflow_py/models/song.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.1/src/tuneflow_py/models/tempo.py` & `tuneflow-py-0.6.0/src/tuneflow_py/models/tempo.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.1/src/tuneflow_py/models/time_signature.py` & `tuneflow-py-0.6.0/src/tuneflow_py/models/time_signature.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.1/src/tuneflow_py/models/track.py` & `tuneflow-py-0.6.0/src/tuneflow_py/models/track.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.1/src/tuneflow_py/utils.py` & `tuneflow-py-0.6.0/src/tuneflow_py/utils.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.1/src/tuneflow_py.egg-info/PKG-INFO` & `tuneflow-py-0.6.0/src/tuneflow_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-py
-Version: 0.5.1
+Version: 0.6.0
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: TuneFlow <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-py-0.5.1/src/tuneflow_py.egg-info/SOURCES.txt` & `tuneflow-py-0.6.0/src/tuneflow_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.1/test/test_audio_clip.py` & `tuneflow-py-0.6.0/test/test_audio_clip.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-from tuneflow_py import Song, Clip, Track, TrackType, Note, ClipType
-from miditoolkit.midi import MidiFile
-from pathlib import PurePath, Path
-from io import BytesIO
-from typing import List
+from tuneflow_py import Song, TrackType, ClipType
 import unittest
+import pytest
 
 TEST_AUDIO_CLIP_DATA = {
     "audio_file_path": 'file1',
     "start_tick": 480,
     "duration": 1,
 }
 
@@ -129,14 +126,136 @@
         self.assertEqual(clip1.get_clip_start_tick(), 960)
         self.assertEqual(clip1.get_clip_end_tick(), 1000)
         self.assertEqual(clip1.get_audio_duration(), 1)
         self.assertEqual(clip1.get_audio_end_tick(), 1440)
         self.assertEqual(clip1.get_audio_clip_data().audio_file_path, TEST_AUDIO_CLIP_DATA["audio_file_path"])
         self.assertEqual(clip1.get_audio_clip_data().start_tick, TEST_AUDIO_CLIP_DATA["start_tick"])
         self.assertAlmostEqual(clip1.get_audio_clip_data().duration, TEST_AUDIO_CLIP_DATA["duration"])
+    
+    def test_get_optional_clip_audio_data_fields(self):
+        clip1 = self.audio_track.create_audio_clip(
+            clip_start_tick=960,
+            clip_end_tick=1440,
+            audio_clip_data={
+                "start_tick": 480,
+                "audio_file_path": 'file1',
+                "duration": 1,
+                "speed_ratio": 2,
+                "pitch_offset": 12
+            },
+        )
+        self.assertEqual(clip1.get_audio_speed_ratio(), 2)
+        self.assertEqual(clip1.get_audio_pitch_offset(), 12)
+        clip1.set_audio_pitch_offset(-13)
+        self.assertEqual(clip1.get_audio_pitch_offset(), -13)
+
+    def test_set_and_get_audio_pitch_offset(self):
+        clip1 = self.audio_track.create_audio_clip(
+            clip_start_tick=960,
+            clip_end_tick=1000,
+            audio_clip_data=TEST_AUDIO_CLIP_DATA,
+        )
+        self.assertEqual(clip1.get_audio_pitch_offset(), 0)
+        clip1.set_audio_pitch_offset(24)
+        self.assertEqual(clip1.get_audio_pitch_offset(), 24)
+        with pytest.raises(Exception) as e_info_1:
+            clip1.set_audio_pitch_offset(-99)
+
+        with pytest.raises(Exception) as e_info_2:
+            clip1.set_audio_pitch_offset(99)
+
+    def rejects_out_of_range_audio_speed_ratio(self):
+        clip1 = self.audio_track.create_audio_clip(
+            clip_start_tick=960,
+            clip_end_tick=1440,
+            audio_clip_data={
+                "start_tick": 480,
+                "audio_file_path": 'file1',
+                "duration": 1
+            },
+        )
+        with pytest.raises(Exception) as e_info_1:
+            clip1.time_stretch_from_clip_right(9999999)
+        with pytest.raises(Exception) as e_info_2:
+            clip1.time_stretch_from_clip_right(961)
+        with pytest.raises(Exception) as e_info_3:
+            clip1.time_stretch_from_clip_left(1439)
+        with pytest.raises(Exception) as e_info_4:
+            clip1.time_stretch_from_clip_left(-999999)
+
+    def test_time_stretch_from_clip_left(self):
+        clip1 = self.audio_track.create_audio_clip(
+            clip_start_tick=960,
+            clip_end_tick=1440,
+            audio_clip_data={
+                "start_tick": 480,
+                "audio_file_path": 'file1',
+                "duration": 1,
+            },
+        )
+        self.assertEqual(clip1.get_raw_audio_duration(), 1)
+        self.assertEqual(clip1.get_audio_duration(), 1)
+        self.assertEqual(clip1.get_audio_start_tick(), 480)
+        self.assertEqual(clip1.get_audio_end_tick(), 1440)
+        self.assertEqual(clip1.get_clip_start_tick(), 960)
+        self.assertEqual(clip1.get_clip_end_tick(), 1440)
+        self.assertEqual(clip1.get_audio_speed_ratio(), 1)
+
+        clip1.time_stretch_from_clip_left(480)
+        self.assertEqual(clip1.get_raw_audio_duration(), 1)
+        self.assertAlmostEqual(clip1.get_audio_duration(), 2.0)
+        self.assertEqual(clip1.get_audio_start_tick(), -480)
+        self.assertEqual(clip1.get_audio_end_tick(), 1440)
+        self.assertEqual(clip1.get_clip_start_tick(), 480)
+        self.assertEqual(clip1.get_clip_end_tick(), 1440)
+        self.assertAlmostEqual(clip1.get_audio_speed_ratio(), 0.5)
+
+        clip1.time_stretch_from_clip_left(1200)
+        self.assertEqual(clip1.get_raw_audio_duration(), 1)
+        self.assertEqual(clip1.get_audio_duration(), 0.5)
+        self.assertEqual(clip1.get_audio_start_tick(), 960)
+        self.assertEqual(clip1.get_audio_end_tick(), 1440)
+        self.assertEqual(clip1.get_clip_start_tick(), 1200)
+        self.assertEqual(clip1.get_clip_end_tick(), 1440)
+        self.assertAlmostEqual(clip1.get_audio_speed_ratio(), 2)
+
+    def test_time_stretch_from_clip_right(self):
+        clip1 = self.audio_track.create_audio_clip(
+            clip_start_tick=960,
+            clip_end_tick=1440,
+            audio_clip_data={
+                "start_tick": 480,
+                "audio_file_path": 'file1',
+                "duration": 1,
+            },
+        )
+        self.assertEqual(clip1.get_raw_audio_duration(), 1)
+        self.assertEqual(clip1.get_audio_duration(), 1)
+        self.assertEqual(clip1.get_audio_start_tick(), 480)
+        self.assertEqual(clip1.get_audio_end_tick(), 1440)
+        self.assertEqual(clip1.get_clip_start_tick(), 960)
+        self.assertEqual(clip1.get_clip_end_tick(), 1440)
+        self.assertEqual(clip1.get_audio_speed_ratio(), 1)
+
+        clip1.time_stretch_from_clip_right(1200)
+        self.assertEqual(clip1.get_audio_duration(), 0.5)
+        self.assertEqual(clip1.get_audio_start_tick(), 720)
+        self.assertEqual(clip1.get_audio_end_tick(), 1200)
+        self.assertEqual(clip1.get_clip_start_tick(), 960)
+        self.assertEqual(clip1.get_clip_end_tick(), 1200)
+        self.assertAlmostEqual(clip1.get_audio_speed_ratio(), 2.0)
+
+        clip1.time_stretch_from_clip_right(1680)
+        self.assertEqual(clip1.get_raw_audio_duration(), 1)
+        self.assertEqual(clip1.get_audio_duration(), 2)
+        self.assertEqual(clip1.get_audio_start_tick(), 0)
+        self.assertEqual(clip1.get_audio_end_tick(), 1680)
+        self.assertEqual(clip1.get_clip_start_tick(), 960)
+        self.assertEqual(clip1.get_clip_end_tick(), 1680)
+        self.assertAlmostEqual(clip1.get_audio_speed_ratio(), 0.5)
 
 
 class TestTrimLeftAndTrimRight(BaseTestCase):
     def test_trim_left_within_audio_range(self):
         clip1 = self.audio_track.create_audio_clip(
             clip_start_tick=960,
             clip_end_tick=1000,
```

### Comparing `tuneflow-py-0.5.1/test/test_automation.py` & `tuneflow-py-0.6.0/test/test_automation.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.1/test/test_marker.py` & `tuneflow-py-0.6.0/test/test_marker.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.1/test/test_midi_clip.py` & `tuneflow-py-0.6.0/test/test_midi_clip.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.1/test/test_note.py` & `tuneflow-py-0.6.0/test/test_note.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.1/test/test_song.py` & `tuneflow-py-0.6.0/test/test_song.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.1/test/test_track.py` & `tuneflow-py-0.6.0/test/test_track.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.1/test/test_utils.py` & `tuneflow-py-0.6.0/test/test_utils.py`

 * *Files identical despite different names*

