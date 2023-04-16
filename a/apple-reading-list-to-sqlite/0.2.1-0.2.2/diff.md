# Comparing `tmp/apple_reading_list_to_sqlite-0.2.1.tar.gz` & `tmp/apple_reading_list_to_sqlite-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apple_reading_list_to_sqlite-0.2.1.tar", max compression
+gzip compressed data, was "apple_reading_list_to_sqlite-0.2.2.tar", max compression
```

## Comparing `apple_reading_list_to_sqlite-0.2.1.tar` & `apple_reading_list_to_sqlite-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-04-14 18:28:13.240358 apple_reading_list_to_sqlite-0.2.1/LICENSE
--rw-r--r--   0        0        0     1242 2023-04-16 17:46:52.351170 apple_reading_list_to_sqlite-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-04-15 11:08:11.395262 apple_reading_list_to_sqlite-0.2.1/apple_reading_list_to_sqlite/__init__.py
--rw-r--r--   0        0        0       22 2023-04-16 17:47:25.471787 apple_reading_list_to_sqlite-0.2.1/apple_reading_list_to_sqlite/__version__.py
--rw-r--r--   0        0        0     3939 2023-04-16 14:08:26.780118 apple_reading_list_to_sqlite-0.2.1/apple_reading_list_to_sqlite/cli.py
--rw-r--r--   0        0        0      750 2023-04-16 17:47:58.713604 apple_reading_list_to_sqlite-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1755 1970-01-01 00:00:00.000000 apple_reading_list_to_sqlite-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-14 18:28:13.240358 apple_reading_list_to_sqlite-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1185 2023-04-16 17:49:27.886546 apple_reading_list_to_sqlite-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 11:08:11.395262 apple_reading_list_to_sqlite-0.2.2/apple_reading_list_to_sqlite/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-16 17:49:41.581441 apple_reading_list_to_sqlite-0.2.2/apple_reading_list_to_sqlite/__version__.py
+-rw-r--r--   0        0        0     3939 2023-04-16 14:08:26.780118 apple_reading_list_to_sqlite-0.2.2/apple_reading_list_to_sqlite/cli.py
+-rw-r--r--   0        0        0      750 2023-04-16 17:49:41.584030 apple_reading_list_to_sqlite-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1698 1970-01-01 00:00:00.000000 apple_reading_list_to_sqlite-0.2.2/PKG-INFO
```

### Comparing `apple_reading_list_to_sqlite-0.2.1/LICENSE` & `apple_reading_list_to_sqlite-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apple_reading_list_to_sqlite-0.2.1/README.md` & `apple_reading_list_to_sqlite-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # apple-reading-list-to-sqlite
 
 Export Apple Reading List to SQLite
 
 ## Install
 
-    $pip install apple-reading-list-to-sqlite
+    $ pip install apple-reading-list-to-sqlite
 
 ## Usage
 
-            $ apple-reading-list-to-sqlite --help
-            Usage: apple-reading-list-to-sqlite [OPTIONS] [DB_PATH]
+    $ apple-reading-list-to-sqlite --help
+      Usage: apple-reading-list-to-sqlite [OPTIONS] [DB_PATH]
 
-            Export Apple Reading List to SQLite
+      Export Apple Reading List to SQLite
 
-            Arguments:
-            [DB_PATH]  Path to the SQLite database file.
+      Arguments:
+      [DB_PATH]  Path to the SQLite database file.
 
-            Options:
-            --version  Show the version and exit.
-            --help     Show this message and exit.
-            --fetch-content / --no-fetch-content try and retrive the content of the article
-            --dump / --no-dump Dump the reading list to stdout
-            --enable-fts / --no-enable-fts Enable full text search
+      Options:
+        --version  Show the version and exit.
+        --help     Show this message and exit.
+        --fetch-content / --no-fetch-content try and retrive the content of the article
+        --dump / --no-dump Dump the reading list to stdout
+        --enable-fts / --no-enable-fts Enable full text search
 
 ## Testing
 
 Right now, all tests only run on macOS. You can run them with:
 
     $ pytest
```

### Comparing `apple_reading_list_to_sqlite-0.2.1/apple_reading_list_to_sqlite/cli.py` & `apple_reading_list_to_sqlite-0.2.2/apple_reading_list_to_sqlite/cli.py`

 * *Files identical despite different names*

### Comparing `apple_reading_list_to_sqlite-0.2.1/pyproject.toml` & `apple_reading_list_to_sqlite-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apple-reading-list-to-sqlite"
-version = "0.2.1"
+version = "0.2.2"
 description = "Export Apple Reading List to SQLite"
 authors = ["ryanscott <ryscott@gmail.com>"]
 readme = "README.md"
 packages = [{include = "apple_reading_list_to_sqlite"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `apple_reading_list_to_sqlite-0.2.1/PKG-INFO` & `apple_reading_list_to_sqlite-0.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apple-reading-list-to-sqlite
-Version: 0.2.1
+Version: 0.2.2
 Summary: Export Apple Reading List to SQLite
 Author: ryanscott
 Author-email: ryscott@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -15,32 +15,32 @@
 
 # apple-reading-list-to-sqlite
 
 Export Apple Reading List to SQLite
 
 ## Install
 
-    $pip install apple-reading-list-to-sqlite
+    $ pip install apple-reading-list-to-sqlite
 
 ## Usage
 
-            $ apple-reading-list-to-sqlite --help
-            Usage: apple-reading-list-to-sqlite [OPTIONS] [DB_PATH]
+    $ apple-reading-list-to-sqlite --help
+      Usage: apple-reading-list-to-sqlite [OPTIONS] [DB_PATH]
 
-            Export Apple Reading List to SQLite
+      Export Apple Reading List to SQLite
 
-            Arguments:
-            [DB_PATH]  Path to the SQLite database file.
+      Arguments:
+      [DB_PATH]  Path to the SQLite database file.
 
-            Options:
-            --version  Show the version and exit.
-            --help     Show this message and exit.
-            --fetch-content / --no-fetch-content try and retrive the content of the article
-            --dump / --no-dump Dump the reading list to stdout
-            --enable-fts / --no-enable-fts Enable full text search
+      Options:
+        --version  Show the version and exit.
+        --help     Show this message and exit.
+        --fetch-content / --no-fetch-content try and retrive the content of the article
+        --dump / --no-dump Dump the reading list to stdout
+        --enable-fts / --no-enable-fts Enable full text search
 
 ## Testing
 
 Right now, all tests only run on macOS. You can run them with:
 
     $ pytest
```

