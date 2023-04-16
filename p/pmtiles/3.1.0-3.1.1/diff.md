# Comparing `tmp/pmtiles-3.1.0.tar.gz` & `tmp/pmtiles-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmtiles-3.1.0.tar", last modified: Thu Dec 22 16:16:13 2022, max compression
+gzip compressed data, was "pmtiles-3.1.1.tar", last modified: Sun Apr 16 11:41:33 2023, max compression
```

## Comparing `pmtiles-3.1.0.tar` & `pmtiles-3.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 bdon       (501) staff       (20)        0 2022-12-22 16:16:13.527126 pmtiles-3.1.0/
--rw-r--r--   0 bdon       (501) staff       (20)       54 2022-09-15 23:32:51.000000 pmtiles-3.1.0/.gitignore
--rw-r--r--   0 bdon       (501) staff       (20)      495 2022-12-22 16:16:13.526994 pmtiles-3.1.0/PKG-INFO
--rw-r--r--   0 bdon       (501) staff       (20)        0 2022-01-20 15:34:15.000000 pmtiles-3.1.0/README.md
-drwxr-xr-x   0 bdon       (501) staff       (20)        0 2022-12-22 16:16:13.524172 pmtiles-3.1.0/bin/
--rwxr-xr-x   0 bdon       (501) staff       (20)     1423 2022-11-21 14:51:38.000000 pmtiles-3.1.0/bin/pmtiles-convert
--rwxr-xr-x   0 bdon       (501) staff       (20)      142 2022-11-21 14:51:38.000000 pmtiles-3.1.0/bin/pmtiles-serve
--rwxr-xr-x   0 bdon       (501) staff       (20)      557 2022-11-21 14:51:38.000000 pmtiles-3.1.0/bin/pmtiles-show
-drwxr-xr-x   0 bdon       (501) staff       (20)        0 2022-12-22 16:16:13.524298 pmtiles-3.1.0/examples/
--rw-r--r--   0 bdon       (501) staff       (20)     1525 2022-11-21 14:51:38.000000 pmtiles-3.1.0/examples/create_raster_example.py
-drwxr-xr-x   0 bdon       (501) staff       (20)        0 2022-12-22 16:16:13.525607 pmtiles-3.1.0/pmtiles/
--rw-r--r--   0 bdon       (501) staff       (20)      111 2022-05-30 02:55:23.000000 pmtiles-3.1.0/pmtiles/__init__.py
--rw-r--r--   0 bdon       (501) staff       (20)     5477 2022-11-21 14:51:38.000000 pmtiles-3.1.0/pmtiles/convert.py
--rw-r--r--   0 bdon       (501) staff       (20)     2451 2022-11-21 14:51:38.000000 pmtiles-3.1.0/pmtiles/reader.py
--rw-r--r--   0 bdon       (501) staff       (20)     7237 2022-12-22 13:54:08.000000 pmtiles-3.1.0/pmtiles/tile.py
--rw-r--r--   0 bdon       (501) staff       (20)     3078 2022-11-21 14:51:38.000000 pmtiles-3.1.0/pmtiles/v2.py
--rw-r--r--   0 bdon       (501) staff       (20)     4474 2022-11-21 14:51:38.000000 pmtiles-3.1.0/pmtiles/writer.py
-drwxr-xr-x   0 bdon       (501) staff       (20)        0 2022-12-22 16:16:13.526109 pmtiles-3.1.0/pmtiles.egg-info/
--rw-r--r--   0 bdon       (501) staff       (20)      495 2022-12-22 16:16:13.000000 pmtiles-3.1.0/pmtiles.egg-info/PKG-INFO
--rw-r--r--   0 bdon       (501) staff       (20)      443 2022-12-22 16:16:13.000000 pmtiles-3.1.0/pmtiles.egg-info/SOURCES.txt
--rw-r--r--   0 bdon       (501) staff       (20)        1 2022-12-22 16:16:13.000000 pmtiles-3.1.0/pmtiles.egg-info/dependency_links.txt
--rw-r--r--   0 bdon       (501) staff       (20)       13 2022-12-22 16:16:13.000000 pmtiles-3.1.0/pmtiles.egg-info/top_level.txt
--rw-r--r--   0 bdon       (501) staff       (20)       38 2022-12-22 16:16:13.527158 pmtiles-3.1.0/setup.cfg
--rw-r--r--   0 bdon       (501) staff       (20)      813 2022-12-22 16:15:59.000000 pmtiles-3.1.0/setup.py
-drwxr-xr-x   0 bdon       (501) staff       (20)        0 2022-12-22 16:16:13.526793 pmtiles-3.1.0/test/
--rw-r--r--   0 bdon       (501) staff       (20)        0 2022-05-30 02:55:23.000000 pmtiles-3.1.0/test/__init__.py
--rw-r--r--   0 bdon       (501) staff       (20)     3157 2022-11-21 14:51:38.000000 pmtiles-3.1.0/test/test_convert.py
--rw-r--r--   0 bdon       (501) staff       (20)     1206 2022-11-21 14:51:38.000000 pmtiles-3.1.0/test/test_reader.py
--rw-r--r--   0 bdon       (501) staff       (20)     7692 2022-12-22 13:50:50.000000 pmtiles-3.1.0/test/test_tile.py
--rw-r--r--   0 bdon       (501) staff       (20)       16 2022-11-21 14:51:38.000000 pmtiles-3.1.0/test/test_writer.py
+drwxr-xr-x   0 bdon       (501) staff       (20)        0 2023-04-16 11:41:33.049441 pmtiles-3.1.1/
+-rw-r--r--   0 bdon       (501) staff       (20)       54 2022-09-15 23:32:51.000000 pmtiles-3.1.1/.gitignore
+-rw-r--r--   0 bdon       (501) staff       (20)      495 2023-04-16 11:41:33.049313 pmtiles-3.1.1/PKG-INFO
+-rw-r--r--   0 bdon       (501) staff       (20)        0 2022-01-20 15:34:15.000000 pmtiles-3.1.1/README.md
+drwxr-xr-x   0 bdon       (501) staff       (20)        0 2023-04-16 11:41:33.046278 pmtiles-3.1.1/bin/
+-rwxr-xr-x   0 bdon       (501) staff       (20)     1423 2022-11-21 14:51:38.000000 pmtiles-3.1.1/bin/pmtiles-convert
+-rwxr-xr-x   0 bdon       (501) staff       (20)      142 2022-11-21 14:51:38.000000 pmtiles-3.1.1/bin/pmtiles-serve
+-rwxr-xr-x   0 bdon       (501) staff       (20)      557 2022-11-21 14:51:38.000000 pmtiles-3.1.1/bin/pmtiles-show
+drwxr-xr-x   0 bdon       (501) staff       (20)        0 2023-04-16 11:41:33.046436 pmtiles-3.1.1/examples/
+-rw-r--r--   0 bdon       (501) staff       (20)     1525 2022-11-21 14:51:38.000000 pmtiles-3.1.1/examples/create_raster_example.py
+drwxr-xr-x   0 bdon       (501) staff       (20)        0 2023-04-16 11:41:33.047732 pmtiles-3.1.1/pmtiles/
+-rw-r--r--   0 bdon       (501) staff       (20)      111 2022-05-30 02:55:23.000000 pmtiles-3.1.1/pmtiles/__init__.py
+-rw-r--r--   0 bdon       (501) staff       (20)     5570 2023-03-12 05:15:04.000000 pmtiles-3.1.1/pmtiles/convert.py
+-rw-r--r--   0 bdon       (501) staff       (20)     2451 2022-11-21 14:51:38.000000 pmtiles-3.1.1/pmtiles/reader.py
+-rw-r--r--   0 bdon       (501) staff       (20)     7238 2023-02-01 10:17:57.000000 pmtiles-3.1.1/pmtiles/tile.py
+-rw-r--r--   0 bdon       (501) staff       (20)     3090 2023-02-01 10:17:57.000000 pmtiles-3.1.1/pmtiles/v2.py
+-rw-r--r--   0 bdon       (501) staff       (20)     4474 2022-11-21 14:51:38.000000 pmtiles-3.1.1/pmtiles/writer.py
+drwxr-xr-x   0 bdon       (501) staff       (20)        0 2023-04-16 11:41:33.048273 pmtiles-3.1.1/pmtiles.egg-info/
+-rw-r--r--   0 bdon       (501) staff       (20)      495 2023-04-16 11:41:32.000000 pmtiles-3.1.1/pmtiles.egg-info/PKG-INFO
+-rw-r--r--   0 bdon       (501) staff       (20)      443 2023-04-16 11:41:32.000000 pmtiles-3.1.1/pmtiles.egg-info/SOURCES.txt
+-rw-r--r--   0 bdon       (501) staff       (20)        1 2023-04-16 11:41:32.000000 pmtiles-3.1.1/pmtiles.egg-info/dependency_links.txt
+-rw-r--r--   0 bdon       (501) staff       (20)       13 2023-04-16 11:41:32.000000 pmtiles-3.1.1/pmtiles.egg-info/top_level.txt
+-rw-r--r--   0 bdon       (501) staff       (20)       38 2023-04-16 11:41:33.049479 pmtiles-3.1.1/setup.cfg
+-rw-r--r--   0 bdon       (501) staff       (20)      813 2023-04-16 11:40:58.000000 pmtiles-3.1.1/setup.py
+drwxr-xr-x   0 bdon       (501) staff       (20)        0 2023-04-16 11:41:33.049096 pmtiles-3.1.1/test/
+-rw-r--r--   0 bdon       (501) staff       (20)        0 2022-05-30 02:55:23.000000 pmtiles-3.1.1/test/__init__.py
+-rw-r--r--   0 bdon       (501) staff       (20)     3157 2022-11-21 14:51:38.000000 pmtiles-3.1.1/test/test_convert.py
+-rw-r--r--   0 bdon       (501) staff       (20)     1206 2022-11-21 14:51:38.000000 pmtiles-3.1.1/test/test_reader.py
+-rw-r--r--   0 bdon       (501) staff       (20)     7871 2023-02-01 09:15:14.000000 pmtiles-3.1.1/test/test_tile.py
+-rw-r--r--   0 bdon       (501) staff       (20)       16 2022-11-21 14:51:38.000000 pmtiles-3.1.1/test/test_writer.py
```

### Comparing `pmtiles-3.1.0/bin/pmtiles-convert` & `pmtiles-3.1.1/bin/pmtiles-convert`

 * *Files identical despite different names*

### Comparing `pmtiles-3.1.0/bin/pmtiles-show` & `pmtiles-3.1.1/bin/pmtiles-show`

 * *Files identical despite different names*

### Comparing `pmtiles-3.1.0/examples/create_raster_example.py` & `pmtiles-3.1.1/examples/create_raster_example.py`

 * *Files identical despite different names*

### Comparing `pmtiles-3.1.0/pmtiles/convert.py` & `pmtiles-3.1.1/pmtiles/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,16 @@
             metadata["center"] = f"{center_lon},{center_lat},{center_zoom}"
 
         if "format" not in metadata:
             if header["tile_type"] == TileType.MVT:
                 metadata["format"] = "pbf"
 
         for k, v in metadata.items():
+            if not isinstance(v, str):
+                v = json.dumps(v, ensure_ascii=False)
             cursor.execute("INSERT INTO metadata VALUES(?,?)", (k, v))
 
         for zxy, tile_data in all_tiles(source):
             flipped_y = (1 << zxy[0]) - 1 - zxy[2]
             cursor.execute(
                 "INSERT INTO tiles VALUES(?,?,?,?)",
                 (zxy[0], zxy[1], flipped_y, tile_data),
```

### Comparing `pmtiles-3.1.0/pmtiles/reader.py` & `pmtiles-3.1.1/pmtiles/reader.py`

 * *Files identical despite different names*

### Comparing `pmtiles-3.1.0/pmtiles/tile.py` & `pmtiles-3.1.1/pmtiles/tile.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         acc += num_tiles
     raise OverflowError("tile zoom exceeds 64-bit limit")
 
 
 def find_tile(entries, tile_id):
     m = 0
     n = len(entries) - 1
-    while m < n:
+    while m <= n:
         k = (n + m) >> 1
         c = tile_id - entries[k].tile_id
         if c > 0:
             m = k + 1
         elif c < 0:
             n = k - 1
         else:
```

### Comparing `pmtiles-3.1.0/pmtiles/v2.py` & `pmtiles-3.1.1/pmtiles/v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from collections import namedtuple
 
 
 def load_directory(data_bytes, offset, num_entries):
     tile_entries = {}
     leaves = {}
     for i in range(offset, offset + num_entries * 17, 17):
```

### Comparing `pmtiles-3.1.0/pmtiles/writer.py` & `pmtiles-3.1.1/pmtiles/writer.py`

 * *Files identical despite different names*

### Comparing `pmtiles-3.1.0/setup.py` & `pmtiles-3.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pmtiles",
-    version="3.1.0",
+    version="3.1.1",
     author="Brandon Liu",
     author_email="brandon@protomaps.com",
     description="Library and utilities to write and read PMTiles files - cloud-optimized archives of map tiles.",
     license="BSD-3-Clause",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/protomaps/pmtiles",
```

### Comparing `pmtiles-3.1.0/test/test_convert.py` & `pmtiles-3.1.1/test/test_convert.py`

 * *Files identical despite different names*

### Comparing `pmtiles-3.1.0/test/test_reader.py` & `pmtiles-3.1.1/test/test_reader.py`

 * *Files identical despite different names*

### Comparing `pmtiles-3.1.0/test/test_tile.py` & `pmtiles-3.1.1/test/test_tile.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,14 +82,19 @@
 
     def test_find_tile_first(self):
         entries = [Entry(100, 1, 1, 1)]
         result = find_tile(entries, 100)
         self.assertEqual(result.offset, 1)
         self.assertEqual(result.length, 1)
 
+    def test_find_tile_runlength(self):
+        entries = [Entry(3, 3, 1, 2),Entry(5, 5, 1, 2)]
+        result = find_tile(entries, 4)
+        self.assertEqual(result.offset, 3)
+
     def test_find_tile_multiple(self):
         entries = [Entry(100, 1, 1, 2)]
         result = find_tile(entries, 101)
         self.assertEqual(result.offset, 1)
         self.assertEqual(result.length, 1)
         entries = [Entry(100, 1, 1, 2), Entry(150, 2, 2, 2)]
         result = find_tile(entries, 151)
```

