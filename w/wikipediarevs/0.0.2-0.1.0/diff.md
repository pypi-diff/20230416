# Comparing `tmp/wikipediarevs-0.0.2.tar.gz` & `tmp/wikipediarevs-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikipediarevs-0.0.2.tar", last modified: Sun Oct 23 13:38:39 2022, max compression
+gzip compressed data, was "wikipediarevs-0.1.0.tar", last modified: Sun Apr 16 12:52:22 2023, max compression
```

## Comparing `wikipediarevs-0.0.2.tar` & `wikipediarevs-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2022-10-23 13:38:39.701184 wikipediarevs-0.0.2/
--rw-r--r--   0 edsummers   (505) staff       (20)    51063 2022-10-23 13:38:39.701369 wikipediarevs-0.0.2/PKG-INFO
--rw-r--r--   0 edsummers   (505) staff       (20)    50788 2022-10-22 21:13:23.000000 wikipediarevs-0.0.2/README.md
--rw-r--r--   0 edsummers   (505) staff       (20)       63 2022-10-23 13:38:39.701850 wikipediarevs-0.0.2/setup.cfg
--rw-r--r--   0 edsummers   (505) staff       (20)      889 2022-10-23 13:37:34.000000 wikipediarevs-0.0.2/setup.py
-drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2022-10-23 13:38:39.700636 wikipediarevs-0.0.2/wikipediarevs.egg-info/
--rw-r--r--   0 edsummers   (505) staff       (20)    51063 2022-10-23 13:38:39.000000 wikipediarevs-0.0.2/wikipediarevs.egg-info/PKG-INFO
--rw-r--r--   0 edsummers   (505) staff       (20)      301 2022-10-23 13:38:39.000000 wikipediarevs-0.0.2/wikipediarevs.egg-info/SOURCES.txt
--rw-r--r--   0 edsummers   (505) staff       (20)        1 2022-10-23 13:38:39.000000 wikipediarevs-0.0.2/wikipediarevs.egg-info/dependency_links.txt
--rw-r--r--   0 edsummers   (505) staff       (20)       53 2022-10-23 13:38:39.000000 wikipediarevs-0.0.2/wikipediarevs.egg-info/entry_points.txt
--rw-r--r--   0 edsummers   (505) staff       (20)        9 2022-10-23 13:38:39.000000 wikipediarevs-0.0.2/wikipediarevs.egg-info/requires.txt
--rw-r--r--   0 edsummers   (505) staff       (20)       14 2022-10-23 13:38:39.000000 wikipediarevs-0.0.2/wikipediarevs.egg-info/top_level.txt
--rw-r--r--   0 edsummers   (505) staff       (20)        1 2022-10-22 19:17:22.000000 wikipediarevs-0.0.2/wikipediarevs.egg-info/zip-safe
--rwxr-xr-x   0 edsummers   (505) staff       (20)     4289 2022-10-23 13:37:26.000000 wikipediarevs-0.0.2/wikipediarevs.py
+drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-04-16 12:52:22.630381 wikipediarevs-0.1.0/
+-rw-r--r--   0 edsummers   (505) staff       (20)    51063 2023-04-16 12:52:22.630684 wikipediarevs-0.1.0/PKG-INFO
+-rw-r--r--   0 edsummers   (505) staff       (20)    50788 2023-04-16 12:51:46.000000 wikipediarevs-0.1.0/README.md
+-rw-r--r--   0 edsummers   (505) staff       (20)       63 2023-04-16 12:52:22.631199 wikipediarevs-0.1.0/setup.cfg
+-rw-r--r--   0 edsummers   (505) staff       (20)      889 2023-04-16 12:49:01.000000 wikipediarevs-0.1.0/setup.py
+drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-04-16 12:52:22.630084 wikipediarevs-0.1.0/wikipediarevs.egg-info/
+-rw-r--r--   0 edsummers   (505) staff       (20)    51063 2023-04-16 12:52:22.000000 wikipediarevs-0.1.0/wikipediarevs.egg-info/PKG-INFO
+-rw-r--r--   0 edsummers   (505) staff       (20)      301 2023-04-16 12:52:22.000000 wikipediarevs-0.1.0/wikipediarevs.egg-info/SOURCES.txt
+-rw-r--r--   0 edsummers   (505) staff       (20)        1 2023-04-16 12:52:22.000000 wikipediarevs-0.1.0/wikipediarevs.egg-info/dependency_links.txt
+-rw-r--r--   0 edsummers   (505) staff       (20)       53 2023-04-16 12:52:22.000000 wikipediarevs-0.1.0/wikipediarevs.egg-info/entry_points.txt
+-rw-r--r--   0 edsummers   (505) staff       (20)        9 2023-04-16 12:52:22.000000 wikipediarevs-0.1.0/wikipediarevs.egg-info/requires.txt
+-rw-r--r--   0 edsummers   (505) staff       (20)       14 2023-04-16 12:52:22.000000 wikipediarevs-0.1.0/wikipediarevs.egg-info/top_level.txt
+-rw-r--r--   0 edsummers   (505) staff       (20)        1 2022-10-22 19:17:22.000000 wikipediarevs-0.1.0/wikipediarevs.egg-info/zip-safe
+-rwxr-xr-x   0 edsummers   (505) staff       (20)     5042 2023-04-16 12:38:59.000000 wikipediarevs-0.1.0/wikipediarevs.py
```

### Comparing `wikipediarevs-0.0.2/PKG-INFO` & `wikipediarevs-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikipediarevs
-Version: 0.0.2
+Version: 0.1.0
 Summary: Download all the revisions for a set of Wikipedia articles
 Home-page: https://github.com/edsu/wikipediarevs
 Author: Ed Summers
 Author-email: ehs@pobox.com
 License: MIT
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wikipediarevs Version: 0.0.2 Summary: Download all
+Metadata-Version: 2.1 Name: wikipediarevs Version: 0.1.0 Summary: Download all
 the revisions for a set of Wikipedia articles Home-page: https://github.com/
 edsu/wikipediarevs Author: Ed Summers Author-email: ehs@pobox.com License: MIT
 Description-Content-Type: text/markdown # wikipediarevs [![Build Status](https:
 //github.com/edsu/wikipediarevs/workflows/tests/badge.svg)](https://github.com/
 edsu/wikipediarevs/actions/workflows/main.yml) If you have a file of Wikipedia
 article URLs wikipediarevs will get the page revisions for all of them (one
 JSON file per revision). ## Install First you will need to install it: pip3
```

### Comparing `wikipediarevs-0.0.2/README.md` & `wikipediarevs-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `wikipediarevs-0.0.2/setup.py` & `wikipediarevs-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-__version__ = "0.0.2"
+__version__ = "0.1.0"
 
 def load_requirements(filename):
     with open(filename, "rt") as fh:
         return fh.read().rstrip().split("\n")
 
 def long_description():
     with open("README.md") as f:
```

### Comparing `wikipediarevs-0.0.2/wikipediarevs.egg-info/PKG-INFO` & `wikipediarevs-0.1.0/wikipediarevs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikipediarevs
-Version: 0.0.2
+Version: 0.1.0
 Summary: Download all the revisions for a set of Wikipedia articles
 Home-page: https://github.com/edsu/wikipediarevs
 Author: Ed Summers
 Author-email: ehs@pobox.com
 License: MIT
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wikipediarevs Version: 0.0.2 Summary: Download all
+Metadata-Version: 2.1 Name: wikipediarevs Version: 0.1.0 Summary: Download all
 the revisions for a set of Wikipedia articles Home-page: https://github.com/
 edsu/wikipediarevs Author: Ed Summers Author-email: ehs@pobox.com License: MIT
 Description-Content-Type: text/markdown # wikipediarevs [![Build Status](https:
 //github.com/edsu/wikipediarevs/workflows/tests/badge.svg)](https://github.com/
 edsu/wikipediarevs/actions/workflows/main.yml) If you have a file of Wikipedia
 article URLs wikipediarevs will get the page revisions for all of them (one
 JSON file per revision). ## Install First you will need to install it: pip3
```

### Comparing `wikipediarevs-0.0.2/wikipediarevs.py` & `wikipediarevs-0.1.0/wikipediarevs.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,24 +9,28 @@
 import argparse
 import requests
 
 from urllib.parse import urlparse
 
 def main():
     parser = argparse.ArgumentParser(description="Download Wikipedia article revisions")
-    parser.add_argument("input", type=str, help="A Wikipedia article URL or a file that contains Wikipedia URLs.")
+    parser.add_argument("input", type=str, help="A Wikipedia article URL or a UTF-8 encoded file that contains lines of Wikipedia URLs")
     parser.add_argument("--output-dir", default="revisions", type=str, help="The path to a directory where to write results.")
     parser.add_argument("--log", type=str, default="wikipediarevs.log", help="Where to write a log file.")
     parser.add_argument("--quiet", action="store_true", help="Don't print progress to the console.")
+    parser.add_argument("--encoding", type=str, default="utf-8-sig", help="The input file character encoding.")
     opts = parser.parse_args()
     logging.basicConfig(filename=opts.log, level=logging.INFO)
 
     # get the input URL
     if os.path.isfile(opts.input):
-        urls = open(opts.input).read().splitlines()
+        try:
+            urls = open(opts.input, encoding=opts.encoding).read().splitlines()
+        except ValueError:
+            sys.exit(f"Unable to read {opts.input} using the {opts.encoding} character encoding, consider using the --encoding option to set it.")
     else:
         urls = [opts.input]
 
     revd = RevisionDownloader(urls, output_dir=opts.output_dir, quiet=opts.quiet)
     revd.run()
 
 
@@ -37,19 +41,27 @@
         self.quiet = quiet
         self.output_dir = pathlib.Path(output_dir)
         if not self.output_dir.is_dir():
             self.output_dir.mkdir(parents=True)
 
     def run(self):
         for article_url in self.urls:
-            self.download(article_url)
+            try:
+                self.download(article_url)
+            except ValueError as e:
+                logging.error(e)
+            except requests.exceptions.RequestException as e:
+                logging.error("HTTP error when fetching revisions for %s: %s", article_url, e)
 
     def download(self, article_url):
         logging.info("downloading revisions for %s", article_url)
         url = urlparse(article_url)
+        if url.netloc == '':
+            raise ValueError(f"Invalid URL {article_url}")
+
         host = url.netloc
         api_url = f"https://{host}/w/api.php"
 
         # the article title
         title =  os.path.basename(url.path)
 
         # The properties to request for each revision:
@@ -123,11 +135,14 @@
             if not self.quiet:
                 print(path)
 
     def latest_rev_id(self, article_dir):
         if not article_dir.is_dir():
             return None
         revs = sorted(map(lambda d: int(d.name.replace(".json", "")), article_dir.iterdir()))
-        return revs[-1]
+        if len(revs) > 0:
+            return revs[-1]
+        else:
+            return None
 
 if __name__ == "__main__":
     main()
```

