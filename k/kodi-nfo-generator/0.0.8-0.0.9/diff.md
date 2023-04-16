# Comparing `tmp/kodi-nfo-generator-0.0.8.tar.gz` & `tmp/kodi-nfo-generator-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodi-nfo-generator-0.0.8.tar", last modified: Wed Jan  4 03:54:49 2023, max compression
+gzip compressed data, was "kodi-nfo-generator-0.0.9.tar", last modified: Thu Jan  5 23:26:01 2023, max compression
```

## Comparing `kodi-nfo-generator-0.0.8.tar` & `kodi-nfo-generator-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-01-04 03:54:49.392583 kodi-nfo-generator-0.0.8/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2021 2023-01-04 03:54:20.000000 kodi-nfo-generator-0.0.8/CHANGES.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      687 2021-08-14 06:43:50.000000 kodi-nfo-generator-0.0.8/DESCRIPTION.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    35149 2021-08-14 06:43:50.000000 kodi-nfo-generator-0.0.8/LICENSE
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:43:50.000000 kodi-nfo-generator-0.0.8/MANIFEST.in
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3286 2023-01-04 03:54:49.392583 kodi-nfo-generator-0.0.8/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    11532 2023-01-04 03:00:18.000000 kodi-nfo-generator-0.0.8/README.md
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2023-01-04 03:54:49.392583 kodi-nfo-generator-0.0.8/setup.cfg
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2085 2023-01-04 03:54:20.000000 kodi-nfo-generator-0.0.8/setup.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-01-04 03:54:49.388584 kodi-nfo-generator-0.0.8/src/
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-01-04 03:54:49.392583 kodi-nfo-generator-0.0.8/src/kodi/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2021-08-14 06:43:50.000000 kodi-nfo-generator-0.0.8/src/kodi/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6254 2021-08-14 06:43:50.000000 kodi-nfo-generator-0.0.8/src/kodi/exports.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     8253 2023-01-03 01:27:07.000000 kodi-nfo-generator-0.0.8/src/kodi/generator.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5537 2023-01-04 03:49:00.000000 kodi-nfo-generator-0.0.8/src/kodi/guess.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    12051 2023-01-04 03:46:20.000000 kodi-nfo-generator-0.0.8/src/kodi/imdb.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6575 2021-11-07 19:42:11.000000 kodi-nfo-generator-0.0.8/src/kodi/imdb_series.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     7999 2021-08-14 06:43:50.000000 kodi-nfo-generator-0.0.8/src/kodi/imports.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3974 2021-08-14 06:43:50.000000 kodi-nfo-generator-0.0.8/src/kodi/io_utils.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2308 2023-01-02 21:09:11.000000 kodi-nfo-generator-0.0.8/src/kodi/xml_utils.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-01-04 03:54:49.392583 kodi-nfo-generator-0.0.8/src/kodi_nfo_generator.egg-info/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3286 2023-01-04 03:54:49.000000 kodi-nfo-generator-0.0.8/src/kodi_nfo_generator.egg-info/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      529 2023-01-04 03:54:49.000000 kodi-nfo-generator-0.0.8/src/kodi_nfo_generator.egg-info/SOURCES.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2023-01-04 03:54:49.000000 kodi-nfo-generator-0.0.8/src/kodi_nfo_generator.egg-info/dependency_links.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      174 2023-01-04 03:54:49.000000 kodi-nfo-generator-0.0.8/src/kodi_nfo_generator.egg-info/entry_points.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       31 2023-01-04 03:54:49.000000 kodi-nfo-generator-0.0.8/src/kodi_nfo_generator.egg-info/requires.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        5 2023-01-04 03:54:49.000000 kodi-nfo-generator-0.0.8/src/kodi_nfo_generator.egg-info/top_level.txt
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-01-05 23:26:01.948165 kodi-nfo-generator-0.0.9/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2572 2023-01-05 23:25:31.000000 kodi-nfo-generator-0.0.9/CHANGES.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      687 2021-08-14 06:43:50.000000 kodi-nfo-generator-0.0.9/DESCRIPTION.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    35149 2021-08-14 06:43:50.000000 kodi-nfo-generator-0.0.9/LICENSE
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:43:50.000000 kodi-nfo-generator-0.0.9/MANIFEST.in
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3837 2023-01-05 23:26:01.948165 kodi-nfo-generator-0.0.9/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    13534 2023-01-05 22:57:30.000000 kodi-nfo-generator-0.0.9/README.md
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2023-01-05 23:26:01.948165 kodi-nfo-generator-0.0.9/setup.cfg
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2137 2023-01-05 23:25:31.000000 kodi-nfo-generator-0.0.9/setup.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-01-05 23:26:01.944165 kodi-nfo-generator-0.0.9/src/
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-01-05 23:26:01.948165 kodi-nfo-generator-0.0.9/src/kodi/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2021-08-14 06:43:50.000000 kodi-nfo-generator-0.0.9/src/kodi/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6254 2021-08-14 06:43:50.000000 kodi-nfo-generator-0.0.9/src/kodi/exports.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     9307 2023-01-05 22:49:51.000000 kodi-nfo-generator-0.0.9/src/kodi/generator.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     5537 2023-01-04 03:49:00.000000 kodi-nfo-generator-0.0.9/src/kodi/guess.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    13098 2023-01-05 22:41:44.000000 kodi-nfo-generator-0.0.9/src/kodi/imdb.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     7072 2023-01-05 22:52:27.000000 kodi-nfo-generator-0.0.9/src/kodi/imdb_series.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     7999 2021-08-14 06:43:50.000000 kodi-nfo-generator-0.0.9/src/kodi/imports.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4628 2023-01-05 02:47:13.000000 kodi-nfo-generator-0.0.9/src/kodi/io_utils.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4461 2023-01-05 22:16:44.000000 kodi-nfo-generator-0.0.9/src/kodi/rename.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2437 2023-01-05 02:52:21.000000 kodi-nfo-generator-0.0.9/src/kodi/xml_utils.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-01-05 23:26:01.948165 kodi-nfo-generator-0.0.9/src/kodi_nfo_generator.egg-info/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3837 2023-01-05 23:26:01.000000 kodi-nfo-generator-0.0.9/src/kodi_nfo_generator.egg-info/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      548 2023-01-05 23:26:01.000000 kodi-nfo-generator-0.0.9/src/kodi_nfo_generator.egg-info/SOURCES.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2023-01-05 23:26:01.000000 kodi-nfo-generator-0.0.9/src/kodi_nfo_generator.egg-info/dependency_links.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      213 2023-01-05 23:26:01.000000 kodi-nfo-generator-0.0.9/src/kodi_nfo_generator.egg-info/entry_points.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       31 2023-01-05 23:26:01.000000 kodi-nfo-generator-0.0.9/src/kodi_nfo_generator.egg-info/requires.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        5 2023-01-05 23:26:01.000000 kodi-nfo-generator-0.0.9/src/kodi_nfo_generator.egg-info/top_level.txt
```

### Comparing `kodi-nfo-generator-0.0.8/DESCRIPTION.rst` & `kodi-nfo-generator-0.0.9/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `kodi-nfo-generator-0.0.8/LICENSE` & `kodi-nfo-generator-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kodi-nfo-generator-0.0.8/PKG-INFO` & `kodi-nfo-generator-0.0.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodi-nfo-generator
-Version: 0.0.8
+Version: 0.0.9
 Summary:  Simple Python-based command-line tool to generate .nfo files for movies and TV shows for Kodi. 
 Home-page: https://github.com/fracpete/kodi-nfo-generator
 Author: Peter "fracpete" Reutemann
 Author-email: fracpete@gmail.com
 License: GNU General Public License version 3.0 (GPLv3)
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -22,14 +22,27 @@
 the default is `*.imdb`, containing the unique IMDB movie ID (or full IMDB movie URL).
 The tool will then scour the movie directories for these files and pull in the
 information and create the `.nfo` files in the same location.
 
 Changelog
 =========
 
+0.0.9 (2023-01-06)
+------------------
+
+- using `download-missing` no longer generates `Ignoring unhandled fanart type: download-missing`
+  message when fanart already present (just an output bug).
+- improved checks for existing `.nfo` files to reduce IMDB requests
+- added `kodi-nfo-rename` tool for renaming files using regular expressions
+  (e.g., files of TV shows)
+- the `kodi-nfo-gen` tool now has additional options for matching episode files
+  rather than using hardcoded defaults: `--episode_pattern`, `--season_group`,
+  `--episode_group`.
+
+
 0.0.8 (2023-01-04)
 ------------------
 
 - added `kodi-nfo-guess` tool that performs online database searches for directories
   that miss meta-files, like `.imdb`, which the `kodi-nfo-gen` tool uses as input.
```

### Comparing `kodi-nfo-generator-0.0.8/README.md` & `kodi-nfo-generator-0.0.9/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -35,16 +35,19 @@
 The following parameters can be supplied to the tool:
 
 ```
 usage: kodi-nfo-gen [-h] --dir DIR [--type {imdb}] [--recursive]
                     [--pattern GLOB] [--delay SECONDS]
                     [--preferred_language LANG]
                     [--fanart {none,download,download-missing,use-existing}]
-                    [--fanart_file FILE] [--episodes] [--dry_run]
-                    [--overwrite] [--verbose] [--debug] [--interactive]
+                    [--fanart_file FILE] [--episodes]
+                    [--episode_pattern EPISODE_PATTERN]
+                    [--season_group SEASON_GROUP]
+                    [--episode_group EPISODE_GROUP] [--dry_run] [--overwrite]
+                    [--verbose] [--debug] [--interactive]
                     [--user-agent USER_AGENT]
 
 Generates Kodi .nfo files with information retrieved from IMDB using local
 files containing the unique IMDB movie ID.
 
 optional arguments:
   -h, --help            show this help message and exit
@@ -61,16 +64,25 @@
                         the preferred language for the titles (ISO 639-1, see
                         https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes)
                         (default: en)
   --fanart {none,download,download-missing,use-existing}
                         how to deal with fan-art (default: none)
   --fanart_file FILE    when downloading or using existing fanart, use this
                         filename (default: folder.jpg)
-  --episodes            whether to generte .nfo files for episodes as well
+  --episodes            whether to generate .nfo files for episodes as well
                         (default: False)
+  --episode_pattern EPISODE_PATTERN
+                        the shell pattern to use for locating episode files
+                        (default: *S??E??*.*)
+  --season_group SEASON_GROUP
+                        the regular expression to extract the season (first
+                        group) (default: .*S([0-9]?[0-9])E.*)
+  --episode_group EPISODE_GROUP
+                        the regular expression to extract the episode (first
+                        group) (default: .*E([0-9]?[0-9]).*)
   --dry_run             whether to perform a 'dry-run', ie only outputting the
                         .nfo content to stdout but not saving it to files
                         (default: False)
   --overwrite           whether to overwrite existing .nfo files, ie
                         recreating them with freshly retrieved data (default:
                         False)
   --verbose             whether to output logging information (default: False)
@@ -124,14 +136,45 @@
   --debug               whether to output debugging information (default:
                         False)
   --user-agent USER_AGENT, --ua USER_AGENT
                         User agent for HTTP requests (default: Mozilla)
 ```
 
 
+### kodi-nfo-rename
+
+Simple renaming tool, e.g., to be used for renaming episodes of TV shows
+to a format that kodi recognizes.
+
+The following parameters can be supplied to the tool:
+
+```
+usage: kodi-nfo-rename [-h] --dir DIR --find REGEXP --replace PATTERN
+                       [--recursive] [--dry_run] [--verbose] [--debug]
+
+Simple renaming tool using regular expressions.
+
+optional arguments:
+  -h, --help         show this help message and exit
+  --dir DIR          the directory to traverse (default: None)
+  --find REGEXP      the regular expression that files must match in order to
+                     be renamed (excluding path; must specify groups to
+                     identify season, episode and extension) (default:
+                     ([0-9]?[0-9])x([0-9][0-9]).(.*))
+  --replace PATTERN  the pattern for assembling the new file name (default:
+                     S\1E\2.\3)
+  --recursive        whether to traverse the directory recursively (default:
+                     False)
+  --dry_run          whether to perform a 'dry-run', ie only outputting the
+                     .nfo content to stdout but not saving it to files
+                     (default: False)
+  --verbose          whether to output logging information (default: False)
+  --debug            whether to output debugging information (default: False)
+```
+
 ### kodi-nfo-export
 
 Using the `kodi-nfo-export` tool, you can export your ID files in a CSV file, 
 associating them with the directory that they were located in. The tool also
 looks for `.nfo` files, in case you already have meta-data stored for your movies.  
 
 The following parameters can be supplied to the tool:
```

### Comparing `kodi-nfo-generator-0.0.8/setup.py` & `kodi-nfo-generator-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,23 +44,24 @@
     license='GNU General Public License version 3.0 (GPLv3)',
     package_dir={
         '': 'src'
     },
     packages=[
         "kodi",
     ],
-    version="0.0.8",
+    version="0.0.9",
     author='Peter "fracpete" Reutemann',
     author_email='fracpete@gmail.com',
     install_requires=[
         "requests",
         "beautifulsoup4!=4.9.*",
     ],
     entry_points={
         "console_scripts": [
             "kodi-nfo-gen=kodi.generator:sys_main",
             "kodi-nfo-guess=kodi.guess:sys_main",
+            "kodi-nfo-rename=kodi.rename:sys_main",
             "kodi-nfo-export=kodi.exports:sys_main",
             "kodi-nfo-import=kodi.imports:sys_main",
         ]
     }
 )
```

### Comparing `kodi-nfo-generator-0.0.8/src/kodi/exports.py` & `kodi-nfo-generator-0.0.9/src/kodi/exports.py`

 * *Files identical despite different names*

### Comparing `kodi-nfo-generator-0.0.8/src/kodi/generator.py` & `kodi-nfo-generator-0.0.9/src/kodi/imports.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,154 +7,161 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-# generator.py
-# Copyright (C) 2020-2023 Fracpete (fracpete at gmail dot com)
+# imports.py
+# Copyright (C) 2020 Fracpete (fracpete at gmail dot com)
 
 import argparse
-import fnmatch
+import csv
 import logging
 import os
-import time
 import traceback
-from kodi.imdb import generate_imdb
-from kodi.io_utils import determine_dirs, read_id, skip, proceed
+from kodi.io_utils import guess_file_name, skip, proceed
 
 # logging setup
-logger = logging.getLogger("kodi.generator")
+logger = logging.getLogger("kodi.import")
 
 
-def generate(dir, idtype="imdb", recursive=True, pattern="*.imdb", delay=1, dry_run=False, overwrite=False,
-             language="en", fanart="none", fanart_file="folder.jpg", interactive=False, episodes=False,
-             ua="Mozilla"):
+def import_ids(input, dir, idtype="imdb", cols=dict(), dry_run=False, overwrite=False, interactive=False):
     """
-    Traverses the directory and generates the .nfo files.
+    Imports the IDs from the CSV file.
 
-    :param dir: the directory to traverse
+    :param input: the input CSV file to read from
+    :type input: str
+    :param dir: the top-level movie directory, in case relative paths are stored in the CSV file
     :type dir: str
-    :param idtype: how to interpret the ID files (choices: 'imdb')
+    :param idtype: what type of ID files to generate (choices: 'imdb')
     :type idtype: str
-    :param recursive: whether to search recursively
-    :type recursive: bool
-    :param pattern: the file pattern (glob) to use for identifying the files with the IDs
-    :type pattern: str
-    :param delay: the delay in seconds between web queries
-    :type delay: int
-    :param dry_run: whether to perform a 'dry-run', ie generating .nfo content but not saving them (only outputting them to stdout)
+    :param cols: the dictionary with the columns (name or 1-based index)
+    :type cols: dict
+    :param dry_run: whether to perform a 'dry-run', ie only outputting the content of the ID files but not writing them to disk
     :type dry_run: bool
-    :param overwrite: whether to overwrite existing .nfo files (ie recreating them)
+    :param overwrite: whether to overwrite existing ID files or skip them
     :type overwrite: bool
-    :param language: the preferred language for the titles
-    :type language: str
-    :param fanart: how to deal with fanart
-    :type fanart: str
-    :param fanart_file: the fanart filename to use (when downloading or re-using existing)
-    :type fanart_file: str
     :param interactive: whether to use interactive mode
     :type interactive: bool
-    :param episodes: whether to generate episode information as well
-    :type episodes: bool
-    :param ua: User agent for requests
-    :type ua: str
     """
 
-    dirs = []
-    determine_dirs(dir, recursive, dirs)
-    dirs.sort()
-    logger.info("# dirs: %d" % len(dirs))
-    if interactive:
-        delay = 0
-
-    for d in dirs:
-        logger.info("Current dir: %s" % d)
-        id_filenames = fnmatch.filter(os.listdir(d), pattern)
-
-        for id_filename in id_filenames:
-            id_path = os.path.join(d, id_filename)
-            xml_path = os.path.join(d, os.path.splitext(id_filename)[0] + ".nfo")
-            logger.info("ID file: %s" % id_path)
-
-            id = read_id(id_path)
-            logger.info("ID: %s" % id)
-
-            if interactive and skip():
-                if proceed():
+    indices = {}
+    indices["id"] = -1
+    indices["dir"] = -1
+    indices["file"] = -1
+    first = True
+    with open(input, newline='') as csv_file:
+        csv_reader = csv.reader(csv_file)
+        for row in csv_reader:
+            if first:
+                first = False
+                # determine column indices
+                for i, name in enumerate(row):
+                    for k in cols:
+                        if cols[k] == name:
+                            indices[k] = i
+                        else:
+                            try:
+                                if int(cols[k]) - 1 == i:
+                                    indices[k] = i
+                            except:
+                                pass
+                logger.info("Indices (0-based): %s" % str(indices))
+                if indices["id"] == -1:
+                    raise Exception("ID column not found ('%s')!" % cols["id"])
+                if indices["dir"] == -1:
+                    raise Exception("Dir column not found ('%s')!" % cols["dir"])
+            else:
+                # read values
+                r_id = row[indices["id"]]
+                if r_id is None or len(r_id) == 0:
+                    logger.warning("No ID, skipping row: %s" % str(row))
                     continue
-                else:
-                    break
-
-            if os.path.exists(xml_path) and not overwrite:
-                logger.info(".nfo file already exists, skipping: %s" % xml_path)
+                r_dir = row[indices["dir"]]
+                if r_dir is None or len(r_dir) == 0:
+                    logger.warning("No directory, skipping row: %s" % str(row))
+                    continue
+                r_file = None
+                if indices["file"] != -1:
+                    r_file = row[indices["file"]]
+                if not os.path.isabs(r_dir):
+                    r_dir = os.path.join(dir, r_dir)
+                logger.info("id|dir|file: %s|%s|%s" % (r_id, r_dir, r_file))
+
+                if interactive and skip():
+                    if proceed():
+                        continue
+                    else:
+                        break
 
-            if overwrite or not os.path.exists(xml_path):
-                try:
-                    if idtype == "imdb":
-                        generate_imdb(id, language=language, fanart=fanart, fanart_file=fanart_file,
-                                      xml_path=xml_path, episodes=episodes, path=d, overwrite=overwrite,
-                                      dry_run=dry_run, ua=ua)
+                # output ID file
+                if dry_run:
+                    if r_file is not None:
+                        print("%s -> %s" % (os.path.join(r_dir, r_file), r_id))
+                    else:
+                        print("%s -> %s" % (r_dir, r_id))
+                else:
+                    if r_file is not None and len(r_file) > 0:
+                        id_path = os.path.join(r_dir, r_file + "." + idtype)
+                    else:
+                        id_path = os.path.join(r_dir, guess_file_name(r_dir) + "." + idtype)
+                    logger.info("ID file: %s" % id_path)
+                    if not overwrite and os.path.exists(id_path):
+                        logger.info("Already exists, skipping")
                     else:
-                        logger.critical("Unhandled ID type: %s" % idtype)
-                        return
-                except Exception:
-                    logger.info(traceback.format_exc())
+                        with open(id_path, "w") as id_file:
+                            id_file.write(r_id)
 
                 if interactive and not proceed():
                     break
-                if delay > 0:
-                    time.sleep(delay)
 
 
 def main(args=None):
     """
-    Runs the .nfo generation.
-    Use -h/--help to see all options.
+    Performs the import.
+    Use -h to see all options.
 
     :param args: the command-line arguments to use, uses sys.argv if None
     :type args: list
     """
 
     parser = argparse.ArgumentParser(
-        description='Generates Kodi .nfo files with information retrieved from IMDB using local files containing the unique IMDB movie ID.',
+        description='Imports IDs from CSV, storing ID files in the associated directories.',
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-        prog="kodi-nfo-gen")
-    parser.add_argument("--dir", metavar="DIR", dest="dir", required=True, help="the directory to traverse")
-    parser.add_argument("--type", dest="type", choices=["imdb"], default="imdb", required=False, help="what type of ID the movie ID files represent, ie the website they are from")
-    parser.add_argument("--recursive", action="store_true", dest="recursive", required=False, help="whether to traverse the directory recursively")
-    parser.add_argument("--pattern", metavar="GLOB", dest="pattern", required=False, default="*.imdb", help="the pattern for the files that contain the movie IDs")
-    parser.add_argument("--delay", metavar="SECONDS", dest="delay", type=int, required=False, default=1, help="the delay in seconds between web queries (to avoid blacklisting)")
-    parser.add_argument("--preferred_language", metavar="LANG", dest="language", required=False, default="en", help="the preferred language for the titles (ISO 639-1, see https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes)")
-    parser.add_argument("--fanart", dest="fanart", choices=["none", "download", "download-missing", "use-existing"], default="none", required=False, help="how to deal with fan-art")
-    parser.add_argument("--fanart_file", metavar="FILE", dest="fanart_file", default="folder.jpg", required=False, help="when downloading or using existing fanart, use this filename")
-    parser.add_argument("--episodes", action="store_true", dest="episodes", required=False, help="whether to generte .nfo files for episodes as well")
-    parser.add_argument("--dry_run", action="store_true", dest="dry_run", required=False, help="whether to perform a 'dry-run', ie only outputting the .nfo content to stdout but not saving it to files")
-    parser.add_argument("--overwrite", action="store_true", dest="overwrite", required=False, help="whether to overwrite existing .nfo files, ie recreating them with freshly retrieved data")
+        prog="kodi-nfo-import")
+    parser.add_argument("--input", metavar="CSV", dest="input", required=True, help="the CSV output file to store the collected information in")
+    parser.add_argument("--dir", metavar="DIR", dest="dir", required=True, help="the top-level directory of the movies if relative directories are used in the CSV file")
+    parser.add_argument("--type", dest="type", choices=["imdb"], default="imdb", required=False, help="what type of ID to create, ie what website the IDs are from")
+    parser.add_argument("--col_id", metavar="COL", dest="col_id", required=True, help="the column that contains the ID (name or 1-based index)")
+    parser.add_argument("--col_dir", metavar="COL", dest="col_dir", required=True, help="the column that contains the directory (name or 1-based index)")
+    parser.add_argument("--col_file", metavar="COL", dest="col_file", required=False, default=None, help="the column that contains the file name (name or 1-based index)")
+    parser.add_argument("--dry_run", action="store_true", dest="dry_run", required=False, help="whether to perform a 'dry-run', ie only outputting the ID file content to stdout but not saving them to files")
+    parser.add_argument("--overwrite", action="store_true", dest="overwrite", required=False, help="whether to overwrite any existing ID files or leave them be")
     parser.add_argument("--verbose", action="store_true", dest="verbose", required=False, help="whether to output logging information")
     parser.add_argument("--debug", action="store_true", dest="debug", required=False, help="whether to output debugging information")
     parser.add_argument("--interactive", action="store_true", dest="interactive", required=False, help="for enabling interactive mode")
-    parser.add_argument("--user-agent", "--ua", type=str, required=False, default="Mozilla", help="User agent for HTTP requests")
     parsed = parser.parse_args(args=args)
     # interactive mode turns on verbose mode
     if parsed.interactive and not (parsed.verbose or parsed.debug):
         parsed.verbose = True
     # configure loggin
     if parsed.debug:
         logging.basicConfig(level=logging.DEBUG)
     elif parsed.verbose:
         logging.basicConfig(level=logging.INFO)
     logger.debug(parsed)
     if parsed.interactive:
         logger.info("Entering interactive mode")
-    generate(dir=parsed.dir, idtype=parsed.type, recursive=parsed.recursive, pattern=parsed.pattern,
-             dry_run=parsed.dry_run, overwrite=parsed.overwrite, language=parsed.language,
-             fanart=parsed.fanart, fanart_file=parsed.fanart_file, interactive=parsed.interactive,
-             episodes=parsed.episodes, ua=parsed.user_agent)
+    cols = {}
+    cols["id"] = parsed.col_id
+    cols["dir"] = parsed.col_dir
+    cols["file"] = parsed.col_file
+    import_ids(input=parsed.input, dir=parsed.dir, idtype=parsed.type, dry_run=parsed.dry_run,
+               overwrite=parsed.overwrite, cols=cols, interactive=parsed.interactive)
 
 
 def sys_main():
     """
     Runs the main function using the system cli arguments, and
     returns a system error code.
```

### Comparing `kodi-nfo-generator-0.0.8/src/kodi/guess.py` & `kodi-nfo-generator-0.0.9/src/kodi/guess.py`

 * *Files identical despite different names*

### Comparing `kodi-nfo-generator-0.0.8/src/kodi/imdb.py` & `kodi-nfo-generator-0.0.9/src/kodi/imdb.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,55 +17,69 @@
 from bs4 import BeautifulSoup
 import fnmatch
 import json
 import logging
 import os
 import requests
 from xml.dom import minidom
-from kodi.io_utils import determine_dirs, prompt, read_id
+from kodi.io_utils import determine_dirs, prompt, read_id, TAG_MOVIE, TAG_TVSHOW, FILENAME_TVSHOW, get_nfo_file
 from kodi.xml_utils import add_node, output_xml
 from kodi.imdb_series import has_episodes, create_episodes_url, extract_seasons, extract_episodes, episode_to_xml, \
     extract_season_episode
 
 # logging setup
 logger = logging.getLogger("kodi.imdb")
 
-TAG_MOVIE = "movie"
-TAG_TVSHOW = "tvshow"
-FILENAME_TVSHOW = "tvshow.nfo"
 
-
-def generate_imdb(id, language="en", fanart="none", fanart_file="folder.jpg", xml_path=None, episodes=False, path=None,
-                  overwrite=False, dry_run=False, ua="Mozilla"):
+def generate_imdb(id, language="en", fanart="none", fanart_file="folder.jpg", path=None, overwrite=False, dry_run=False,
+                  episodes=False, episode_pattern="*S??E??*.*",
+                  season_group=".*S([0-9]?[0-9])E.*", episode_group=".*E([0-9]?[0-9]).*",
+                  ua="Mozilla"):
     """
     Generates the XML for the specified IMDB ID.
 
     :param id: the IMDB ID to use
     :type id: str
     :param language: the preferred language for the titles
     :type language: str
     :param fanart: how to deal with fanart
     :type fanart: str
     :param fanart_file: the fanart filename to use (when downloading or re-using existing)
     :type fanart_file: str
-    :param xml_path: the current nfo full file path
-    :type xml_path: str
-    :param episodes: whether to generate episode information as well
-    :type episodes: bool
     :param path: the current directory (used for determining episode files)
     :type path: str
     :param overwrite: whether to overwrite existing .nfo files (ie recreating them)
     :type overwrite: bool
     :param dry_run: whether to perform a 'dry-run', ie generating .nfo content but not saving them (only outputting them to stdout)
     :type dry_run: bool
+    :param episodes: whether to generate episode information as well
+    :type episodes: bool
+    :param episode_pattern: the pattern to use for locating episode files
+    :type episode_pattern: str
+    :param season_group: the regular expression to extract the season (first group)
+    :type season_group: str
+    :param episode_group: the regular expression to extract the episode (first group)
+    :type episode_group: str
     :param ua: the user agent to use, ignore if empty string or None
     :type ua: str
+    :return: whether a file was generated
+    :rtype: bool
     """
     id = id.strip()
 
+    # can we skip?
+    if not overwrite:
+        f = get_nfo_file(path)
+        if f is not None:
+            logger.info(".nfo file already exists, skipping: %s" % f)
+            return False
+
+    # default movie .nfo
+    xml_path = os.path.join(path, os.path.basename(path) + ".nfo")
+
     # generate URL
     if id.startswith("http"):
         url = id
     else:
         url = "https://www.imdb.com/title/%s/" % id
     logger.info("IMDB URL: " + url)
 
@@ -84,14 +98,15 @@
 
     widget = soup.find("div", id="star-rating-widget")
     if widget is None:
         preflang_title = None
     else:
         preflang_title = widget["data-title"]
 
+    output_generated = False
     for script in soup.findAll("script", type="application/ld+json"):
         j = json.loads(script.text)
         logger.debug(j)
 
         root = add_node(doc, doc, TAG_MOVIE)
         add_node(doc, root, "title", j['name'] if preflang_title is None else preflang_title)
         add_node(doc, root, "originaltitle", j["name"])
@@ -121,16 +136,22 @@
             xratings = add_node(doc, root, "ratings")
             xrating = add_node(doc, xratings, "rating")
             xrating.setAttribute("name", "imdb")
             xrating.setAttribute("max", "10")
             add_node(doc, xrating, "value", str(j["aggregateRating"]["ratingValue"]))
 
         # fanart
-        fanart_path = os.path.join(os.path.dirname(xml_path), fanart_file)
-        if (fanart == "download") or ((fanart == "download-missing") and not os.path.exists(fanart_path)):
+        fanart_path = os.path.join(path, fanart_file)
+        fanart_act = fanart
+        if fanart_act == "download-missing":
+            if os.path.exists(fanart_path):
+                fanart_act = "use-existing"
+            else:
+                fanart_act = "download"
+        if fanart_act == "download":
             if "image" in j:
                 logger.info("Downloading fanart: %s" % j["image"])
                 if (ua is not None) and (ua != ""):
                     r = requests.get(j["image"], headers={'user-agent': ua}, stream=True)
                 else:
                     r = requests.get(j["image"], stream=True)
                 if r.status_code == 200:
@@ -139,27 +160,27 @@
                             f.write(chunk)
                     xthumb = add_node(doc, root, "thumb", fanart_file)
                     xthumb.setAttribute("aspect", "poster")
                 else:
                     logger.critical("Failed to download fanart, status code: " % r.status_code)
             else:
                 logger.warning("No image associated, cannot download!")
-        elif fanart == "use-existing":
+        elif fanart_act == "use-existing":
             xthumb = add_node(doc, root, "thumb", fanart_file)
             xthumb.setAttribute("aspect", "poster")
-        elif fanart == "none":
+        elif fanart_act == "none":
             pass
         else:
-            logger.critical("Ignoring unhandled fanart type: %s" % fanart)
+            logger.critical("Ignoring unhandled fanart type: %s" % fanart_act)
 
         if has_episodes(soup):
             logger.info("Has episode data")
 
-            # use special name rather than ID-based one
-            xml_path = os.path.join(os.path.dirname(xml_path), FILENAME_TVSHOW)
+            # use special name rather than name-based one
+            xml_path = os.path.join(path, FILENAME_TVSHOW)
 
             # update root tag
             root.tagName = TAG_TVSHOW
 
             if episodes:
                 # determine seasons
                 url = create_episodes_url(id)
@@ -188,28 +209,32 @@
                         xml = episode_to_xml(episodes_data[k])
                         season_data[season][k] = xml
 
                 # locate files and output XML
                 dirs = []
                 determine_dirs(path, True, dirs)
                 for d in dirs:
-                    files = fnmatch.filter(os.listdir(d), "*S??E??*.*")
+                    files = fnmatch.filter(os.listdir(d), episode_pattern)
                     for f in files:
                         if f.endswith(".nfo"):
                             continue
-                        parts = extract_season_episode(f)
+                        parts = extract_season_episode(f, season_group=season_group, episode_group=episode_group)
                         if parts is None:
                             continue
                         s, e = parts
                         if (s in season_data) and (e in season_data[s]):
                             xml_path_ep = os.path.join(d, os.path.splitext(f)[0] + ".nfo")
-                            output_xml(season_data[s][e], xml_path_ep, dry_run=dry_run, overwrite=overwrite, logger=logger)
+                            if output_xml(season_data[s][e], xml_path_ep, dry_run=dry_run, overwrite=overwrite, logger=logger):
+                                output_generated = True
 
         # output .nfo
-        output_xml(doc, xml_path, dry_run=dry_run, overwrite=overwrite, logger=logger)
+        if output_xml(doc, xml_path, dry_run=dry_run, overwrite=overwrite, logger=logger):
+            output_generated = True
+
+        return output_generated
 
 
 def guess_imdb(title, meta_path, language="en", dry_run=False, ua="Mozilla"):
     """
     Generates .imdb files using the user's selection of IMDB search results for the title.
 
     :param title: the title to look for
```

### Comparing `kodi-nfo-generator-0.0.8/src/kodi/imdb_series.py` & `kodi-nfo-generator-0.0.9/src/kodi/imdb_series.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 # imdb_series.py
-# Copyright (C) 2021 Fracpete (fracpete at gmail dot com)
+# Copyright (C) 2021-2023 Fracpete (fracpete at gmail dot com)
 
 import re
 import logging
 from bs4 import BeautifulSoup
 from datetime import datetime
 from xml.dom import minidom
 from kodi.xml_utils import add_node
@@ -192,25 +192,32 @@
         rating.setAttribute("default", "true")
         add_node(doc, rating, "value", str(episode_data["_rating"]["value"]))
         add_node(doc, rating, "votes", str(episode_data["_rating"]["votes"]))
 
     return doc
 
 
-def extract_season_episode(path):
+def extract_season_episode(path, season_group=".*S([0-9]?[0-9])E.*", episode_group=".*E([0-9]?[0-9]).*"):
     """
     Extracts season and episode from the file path (format: *S??E??*).
 
     :param path: the path to extract the season/episode from
     :type path: str
+    :param season_group: the regular expression to extract the season (first group)
+    :type season_group: str
+    :param episode_group: the regular expression to extract the episode (first group)
+    :type episode_group: str
     :return: the list of season/episode, None if no match
     :rtype: list
     """
-    p = re.compile(".*S([0-9][0-9]?)E([0-9][0-9]?).*")
-    m = p.match(path)
-    if m is None:
+    pattern_s = re.compile(season_group)
+    pattern_e = re.compile(episode_group)
+    match_s = pattern_s.match(path)
+    match_e = pattern_e.match(path)
+    if (match_s is None) or (match_e is None):
         return None
-    result = m.groups()
-    if len(result) == 2:
-        return [str(int(x)) for x in result]
+    result_s = match_s.groups()
+    result_e = match_e.groups()
+    if (len(result_s) == 1) and (len(result_e) == 1):
+        return [str(int(result_s[0])), str(int(result_e[0]))]
     else:
         return None
```

### Comparing `kodi-nfo-generator-0.0.8/src/kodi/io_utils.py` & `kodi-nfo-generator-0.0.9/src/kodi/io_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,38 +8,42 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 # io_utils.py
-# Copyright (C) 2020 Fracpete (fracpete at gmail dot com)
+# Copyright (C) 2020-2023 Fracpete (fracpete at gmail dot com)
 
 import fnmatch
 import os
 from xml.dom import minidom
 
+TAG_MOVIE = "movie"
+TAG_TVSHOW = "tvshow"
+FILENAME_TVSHOW = "tvshow.nfo"
 
-def determine_dirs(dir, recursive, result):
+
+def determine_dirs(path, recursive, result):
     """
     Determines all the directories to inspect.
 
-    :param dir: the top-level directory
-    :type dir: str
+    :param path: the top-level directory
+    :type path: str
     :param recursive: whether to look for directories recursively
     :type recursive: bool
     :param result: for storing the located dirs
     :type param: list
     """
 
-    result.append(dir)
+    result.append(path)
     if recursive:
-        files = os.listdir(dir)
+        files = os.listdir(path)
         for f in files:
-            full = os.path.join(dir, f)
+            full = os.path.join(path, f)
             if os.path.isdir(full):
                 determine_dirs(full, True, result)
 
 
 def read_id(id_path):
     """
     Reads the ID from the specified ID file.
@@ -73,39 +77,39 @@
         if "type" in item.attributes and item.attributes["type"].value == idtype:
             id = item.firstChild.data
             break
 
     return id.strip()
 
 
-def guess_file_name(dir):
+def guess_file_name(path):
     """
     Tries to determine the filename (excl extension) for the specified directory.
     Looks for .nfo file, then video files (mp4, mkv, avi) and finally the base name
     of the directory itself.
 
-    :param dir: the directory to guess the file name for
-    :type dir: str
+    :param path: the directory to guess the file name for
+    :type path: str
     :return: the guessed file name (excl path)
     :rtype: str
     """
 
     result = None
 
     # nfo or video file?
     exts = ["nfo", "mp4", "mkv", "avi"]
     for ext in exts:
-        filenames = fnmatch.filter(os.listdir(dir), "*." + ext)
+        filenames = fnmatch.filter(os.listdir(path), "*." + ext)
         if len(filenames) == 1:
             result = os.path.splitext(os.path.basename(filenames[0]))[0]
             break
 
     # directory
     if result is None:
-        result = os.path.basename(dir)
+        result = os.path.basename(path)
 
     return result
 
 
 def prompt(msg="Proceed (%s)? ", choices=["y", "n"]):
     """
     Prompts user in the console with a message with specific choices to select from.
@@ -146,7 +150,32 @@
     Prompts user whether to skip (y/n).
 
     :return: whether to skip
     :rtype: bool
     """
 
     return prompt(msg="Skip (%s)? ", choices=["y", "n"]) == "y"
+
+
+def get_nfo_file(path):
+    """
+    Checks whether an .nfo file is already present in the path and returns it.
+
+    :param path: the path to check for an existing .nfo file
+    :type path: str
+    :return: an existing .nfo file, otherwise None
+    :rtype: str
+    """
+    result = None
+
+    # movie
+    f = os.path.join(path, os.path.basename(path) + ".nfo")
+    if os.path.exists(f):
+        result = f
+
+    # tv show
+    if result is None:
+        f = os.path.join(path, FILENAME_TVSHOW)
+        if os.path.exists(f):
+            result = f
+
+    return result
```

### Comparing `kodi-nfo-generator-0.0.8/src/kodi/xml_utils.py` & `kodi-nfo-generator-0.0.9/src/kodi/xml_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,19 +50,24 @@
     :param xml_path: the file to (potentially) write to
     :type xml_path: str
     :param dry_run: whether this is just a test run
     :type dry_run: bool
     :param overwrite: whether to overwrite existing files
     :type overwrite: bool
     :param logger: the logger instance to use for outputting logging information
+    :return: whether a file was generated
+    :rtype: bool
     """
     xml_str = doc.toprettyxml(indent="  ")
     if dry_run:
         print(xml_str)
+        return False
     else:
         if os.path.exists(xml_path) and not overwrite:
             logger.info(".nfo file already exists, skipping: %s" % xml_path)
+            return False
         else:
             if logger is not None:
                 logger.info("Writing .nfo file: %s" % xml_path)
             with open(xml_path, "w") as xml_file:
                 xml_file.write(xml_str)
+            return True
```

### Comparing `kodi-nfo-generator-0.0.8/src/kodi_nfo_generator.egg-info/PKG-INFO` & `kodi-nfo-generator-0.0.9/src/kodi_nfo_generator.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodi-nfo-generator
-Version: 0.0.8
+Version: 0.0.9
 Summary:  Simple Python-based command-line tool to generate .nfo files for movies and TV shows for Kodi. 
 Home-page: https://github.com/fracpete/kodi-nfo-generator
 Author: Peter "fracpete" Reutemann
 Author-email: fracpete@gmail.com
 License: GNU General Public License version 3.0 (GPLv3)
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -22,14 +22,27 @@
 the default is `*.imdb`, containing the unique IMDB movie ID (or full IMDB movie URL).
 The tool will then scour the movie directories for these files and pull in the
 information and create the `.nfo` files in the same location.
 
 Changelog
 =========
 
+0.0.9 (2023-01-06)
+------------------
+
+- using `download-missing` no longer generates `Ignoring unhandled fanart type: download-missing`
+  message when fanart already present (just an output bug).
+- improved checks for existing `.nfo` files to reduce IMDB requests
+- added `kodi-nfo-rename` tool for renaming files using regular expressions
+  (e.g., files of TV shows)
+- the `kodi-nfo-gen` tool now has additional options for matching episode files
+  rather than using hardcoded defaults: `--episode_pattern`, `--season_group`,
+  `--episode_group`.
+
+
 0.0.8 (2023-01-04)
 ------------------
 
 - added `kodi-nfo-guess` tool that performs online database searches for directories
   that miss meta-files, like `.imdb`, which the `kodi-nfo-gen` tool uses as input.
```

### Comparing `kodi-nfo-generator-0.0.8/src/kodi_nfo_generator.egg-info/SOURCES.txt` & `kodi-nfo-generator-0.0.9/src/kodi_nfo_generator.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 src/kodi/exports.py
 src/kodi/generator.py
 src/kodi/guess.py
 src/kodi/imdb.py
 src/kodi/imdb_series.py
 src/kodi/imports.py
 src/kodi/io_utils.py
+src/kodi/rename.py
 src/kodi/xml_utils.py
 src/kodi_nfo_generator.egg-info/PKG-INFO
 src/kodi_nfo_generator.egg-info/SOURCES.txt
 src/kodi_nfo_generator.egg-info/dependency_links.txt
 src/kodi_nfo_generator.egg-info/entry_points.txt
 src/kodi_nfo_generator.egg-info/requires.txt
 src/kodi_nfo_generator.egg-info/top_level.txt
```

