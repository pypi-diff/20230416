# Comparing `tmp/safeoutput-2.0.tar.gz` & `tmp/safeoutput-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/safeoutput-2.0.tar", last modified: Mon Dec 23 06:57:42 2019, max compression
+gzip compressed data, was "safeoutput-2.1.tar", last modified: Sun Apr 16 20:12:57 2023, max compression
```

## Comparing `safeoutput-2.0.tar` & `safeoutput-2.1.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 andrewthomson   (501) staff       (20)        0 2019-12-23 06:57:42.000000 safeoutput-2.0/
--rw-r--r--   0 andrewthomson   (501) staff       (20)     1316 2019-12-23 06:57:42.000000 safeoutput-2.0/PKG-INFO
--rw-r--r--   0 andrewthomson   (501) staff       (20)     1075 2019-03-16 02:10:04.000000 safeoutput-2.0/README.md
--rw-r--r--   0 andrewthomson   (501) staff       (20)     1648 2019-12-23 06:48:55.000000 safeoutput-2.0/setup.py
--rw-r--r--   0 andrewthomson   (501) staff       (20)       59 2019-12-23 06:57:42.000000 safeoutput-2.0/setup.cfg
-drwxr-xr-x   0 andrewthomson   (501) staff       (20)        0 2019-12-23 06:57:42.000000 safeoutput-2.0/safeoutput.egg-info/
--rw-r--r--   0 andrewthomson   (501) staff       (20)     1316 2019-12-23 06:57:42.000000 safeoutput-2.0/safeoutput.egg-info/PKG-INFO
--rw-r--r--   0 andrewthomson   (501) staff       (20)        1 2019-03-06 19:42:40.000000 safeoutput-2.0/safeoutput.egg-info/zip-safe
--rw-r--r--   0 andrewthomson   (501) staff       (20)      276 2019-12-23 06:57:42.000000 safeoutput-2.0/safeoutput.egg-info/SOURCES.txt
--rw-r--r--   0 andrewthomson   (501) staff       (20)       48 2019-12-23 06:57:42.000000 safeoutput-2.0/safeoutput.egg-info/entry_points.txt
--rw-r--r--   0 andrewthomson   (501) staff       (20)       26 2019-12-23 06:57:42.000000 safeoutput-2.0/safeoutput.egg-info/requires.txt
--rw-r--r--   0 andrewthomson   (501) staff       (20)       11 2019-12-23 06:57:42.000000 safeoutput-2.0/safeoutput.egg-info/top_level.txt
--rw-r--r--   0 andrewthomson   (501) staff       (20)        1 2019-12-23 06:57:42.000000 safeoutput-2.0/safeoutput.egg-info/dependency_links.txt
-drwxr-xr-x   0 andrewthomson   (501) staff       (20)        0 2019-12-23 06:57:42.000000 safeoutput-2.0/safeoutput/
--rw-r--r--   0 andrewthomson   (501) staff       (20)     2629 2019-12-23 06:54:01.000000 safeoutput-2.0/safeoutput/__init__.py
+drwxr-xr-x   0 andrewthomson   (501) staff       (20)        0 2023-04-16 20:12:57.663931 safeoutput-2.1/
+-rw-r--r--   0 andrewthomson   (501) staff       (20)     1082 2020-04-08 21:45:47.000000 safeoutput-2.1/LICENSE
+-rw-r--r--   0 andrewthomson   (501) staff       (20)     1329 2023-04-16 20:12:57.663574 safeoutput-2.1/PKG-INFO
+-rw-r--r--   0 andrewthomson   (501) staff       (20)     1075 2020-04-08 21:45:47.000000 safeoutput-2.1/README.md
+drwxr-xr-x   0 andrewthomson   (501) staff       (20)        0 2023-04-16 20:12:57.659388 safeoutput-2.1/safeoutput/
+-rw-r--r--   0 andrewthomson   (501) staff       (20)     2822 2023-04-16 20:09:50.000000 safeoutput-2.1/safeoutput/__init__.py
+drwxr-xr-x   0 andrewthomson   (501) staff       (20)        0 2023-04-16 20:12:57.662043 safeoutput-2.1/safeoutput.egg-info/
+-rw-r--r--   0 andrewthomson   (501) staff       (20)     1329 2023-04-16 20:12:57.000000 safeoutput-2.1/safeoutput.egg-info/PKG-INFO
+-rw-r--r--   0 andrewthomson   (501) staff       (20)      309 2023-04-16 20:12:57.000000 safeoutput-2.1/safeoutput.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewthomson   (501) staff       (20)        1 2023-04-16 20:12:57.000000 safeoutput-2.1/safeoutput.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewthomson   (501) staff       (20)       47 2023-04-16 20:12:57.000000 safeoutput-2.1/safeoutput.egg-info/entry_points.txt
+-rw-r--r--   0 andrewthomson   (501) staff       (20)       26 2023-04-16 20:12:57.000000 safeoutput-2.1/safeoutput.egg-info/requires.txt
+-rw-r--r--   0 andrewthomson   (501) staff       (20)       11 2023-04-16 20:12:57.000000 safeoutput-2.1/safeoutput.egg-info/top_level.txt
+-rw-r--r--   0 andrewthomson   (501) staff       (20)        1 2020-05-09 05:41:27.000000 safeoutput-2.1/safeoutput.egg-info/zip-safe
+-rw-r--r--   0 andrewthomson   (501) staff       (20)       38 2023-04-16 20:12:57.664032 safeoutput-2.1/setup.cfg
+-rw-r--r--   0 andrewthomson   (501) staff       (20)     1648 2023-04-16 20:10:28.000000 safeoutput-2.1/setup.py
+drwxr-xr-x   0 andrewthomson   (501) staff       (20)        0 2023-04-16 20:12:57.663061 safeoutput-2.1/tests/
+-rw-r--r--   0 andrewthomson   (501) staff       (20)     2933 2020-04-08 21:45:47.000000 safeoutput-2.1/tests/test_safeoutput.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `safeoutput-2.0/PKG-INFO` & `safeoutput-2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: safeoutput
-Version: 2.0
+Version: 2.1
 Summary: Tempfile wrapper to ensure output files are either complete, or empty. Also handles stdout, which gives no truncation guarantees.
 Home-page: http://github.com/andrewguy9/safeoutput
 Author: andrew thomson
 Author-email: athomsonguy@gmail.com
 License: MIT
-Description: Tool to facilitate console script output redirection. When scripts run, often they have an output file option. If no output option is specified, its common to write to stdout. Its common to use tempfiles as output, and then rename the tempfile to the output name as the last step of the program so that the flip of output is atomic and partial/truncated/corrupt output is not confused as successful output. This is especially true when dealing with make, as exiting with error will stop make, but subsequent runs will assume that partial output files left in the workspace are complete. Writing to stdout gives no guarantees about partial results due to truncation.
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Filesystems
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 2.7
+Provides-Extra: test
+License-File: LICENSE
+
+Tool to facilitate console script output redirection. When scripts run, often they have an output file option. If no output option is specified, its common to write to stdout. Its common to use tempfiles as output, and then rename the tempfile to the output name as the last step of the program so that the flip of output is atomic and partial/truncated/corrupt output is not confused as successful output. This is especially true when dealing with make, as exiting with error will stop make, but subsequent runs will assume that partial output files left in the workspace are complete. Writing to stdout gives no guarantees about partial results due to truncation.
```

### Comparing `safeoutput-2.0/README.md` & `safeoutput-2.1/README.md`

 * *Files identical despite different names*

### Comparing `safeoutput-2.0/setup.py` & `safeoutput-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 tests_require = ['tox', 'pytest']
 
 setup(
     name='safeoutput',
-    version='2.0',
+    version='2.1',
     description='Tempfile wrapper to ensure output files are either complete, or empty. Also handles stdout, which gives no truncation guarantees.',
     long_description='Tool to facilitate console script output redirection. When scripts run, often they have an output file option. If no output option is specified, its common to write to stdout. Its common to use tempfiles as output, and then rename the tempfile to the output name as the last step of the program so that the flip of output is atomic and partial/truncated/corrupt output is not confused as successful output. This is especially true when dealing with make, as exiting with error will stop make, but subsequent runs will assume that partial output files left in the workspace are complete. Writing to stdout gives no guarantees about partial results due to truncation.',
     url='http://github.com/andrewguy9/safeoutput',
     author='andrew thomson',
     author_email='athomsonguy@gmail.com',
     license='MIT',
     packages=['safeoutput'],
```

### Comparing `safeoutput-2.0/safeoutput.egg-info/PKG-INFO` & `safeoutput-2.1/safeoutput.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: safeoutput
-Version: 2.0
+Version: 2.1
 Summary: Tempfile wrapper to ensure output files are either complete, or empty. Also handles stdout, which gives no truncation guarantees.
 Home-page: http://github.com/andrewguy9/safeoutput
 Author: andrew thomson
 Author-email: athomsonguy@gmail.com
 License: MIT
-Description: Tool to facilitate console script output redirection. When scripts run, often they have an output file option. If no output option is specified, its common to write to stdout. Its common to use tempfiles as output, and then rename the tempfile to the output name as the last step of the program so that the flip of output is atomic and partial/truncated/corrupt output is not confused as successful output. This is especially true when dealing with make, as exiting with error will stop make, but subsequent runs will assume that partial output files left in the workspace are complete. Writing to stdout gives no guarantees about partial results due to truncation.
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Filesystems
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 2.7
+Provides-Extra: test
+License-File: LICENSE
+
+Tool to facilitate console script output redirection. When scripts run, often they have an output file option. If no output option is specified, its common to write to stdout. Its common to use tempfiles as output, and then rename the tempfile to the output name as the last step of the program so that the flip of output is atomic and partial/truncated/corrupt output is not confused as successful output. This is especially true when dealing with make, as exiting with error will stop make, but subsequent runs will assume that partial output files left in the workspace are complete. Writing to stdout gives no guarantees about partial results due to truncation.
```

### Comparing `safeoutput-2.0/safeoutput/__init__.py` & `safeoutput-2.1/safeoutput/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 from builtins import object
 from os import rename
 from os.path import abspath, dirname
 from tempfile import NamedTemporaryFile
 
 LOG = logging.getLogger(__name__)
 
+def _sameDir(dst):
+    return dirname(abspath(dst))
 
-def open(dst=None, mode="w"):
+def open(dst=None, mode="w", useDir=_sameDir):
     if dst:
-        fd = NamedTemporaryFile(dir=dirname(abspath(dst)), mode=mode)
+        fd = NamedTemporaryFile(dir=useDir(dst), mode=mode)
     else:
         if mode == "w":
             fd = sys.stdout
         else:
             try:
                 fd = sys.stdout.buffer
             except AttributeError:
@@ -66,23 +68,24 @@
         # tempfile to delete the file.
         self.close(False)
 
 
 def main(args=None):
     """Buffer stdin and flush, and avoid incomplete files."""
     parser = argparse.ArgumentParser(description=main.__doc__)
-    parser.add_argument(
-        '--binary',
-        dest='mode',
-        action='store_const',
-        const="wb",
-        default="w",
-        help='write in binary mode')
-    parser.add_argument(
-        'output', metavar='FILE', type=unicode, help='Output file')
+    parser.add_argument('--binary',
+                        dest='mode',
+                        action='store_const',
+                        const="wb",
+                        default="w",
+                        help='write in binary mode')
+    parser.add_argument('output',
+                        metavar='FILE',
+                        type=unicode,
+                        help='Output file')
 
     logging.basicConfig(
         level=logging.DEBUG,
         stream=sys.stderr,
         format='[%(levelname)s elapsed=%(relativeCreated)dms] %(message)s')
 
     args = parser.parse_args(args or sys.argv[1:])
```

