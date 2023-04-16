# Comparing `tmp/arkdriver-1.0.3.tar.gz` & `tmp/arkdriver-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkdriver-1.0.3.tar", last modified: Sat Apr 15 23:36:49 2023, max compression
+gzip compressed data, was "arkdriver-1.0.4.tar", last modified: Sun Apr 16 02:11:45 2023, max compression
```

## Comparing `arkdriver-1.0.3.tar` & `arkdriver-1.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 23:36:49.385340 arkdriver-1.0.3/
--rw-rw-rw-   0        0        0     1095 2023-03-25 16:35:50.000000 arkdriver-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     1935 2023-04-15 23:36:49.385340 arkdriver-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1305 2023-03-25 16:35:50.000000 arkdriver-1.0.3/README.md
--rw-rw-rw-   0        0        0      695 2023-04-15 23:30:02.000000 arkdriver-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0     1206 2023-04-15 23:36:49.387338 arkdriver-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 23:36:49.356407 arkdriver-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 23:36:49.363404 arkdriver-1.0.3/src/arkdriver/
--rw-rw-rw-   0        0        0      128 2023-04-06 04:15:05.000000 arkdriver-1.0.3/src/arkdriver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 23:36:49.381338 arkdriver-1.0.3/src/arkdriver/driver/
--rw-rw-rw-   0        0        0      137 2023-03-31 17:34:17.000000 arkdriver-1.0.3/src/arkdriver/driver/__init__.py
--rw-rw-rw-   0        0        0    10696 2023-04-14 00:06:06.000000 arkdriver-1.0.3/src/arkdriver/driver/application.py
--rw-rw-rw-   0        0        0     2830 2023-03-31 21:05:16.000000 arkdriver-1.0.3/src/arkdriver/driver/driver.py
--rw-rw-rw-   0        0        0        0 2023-04-13 23:37:23.000000 arkdriver-1.0.3/src/arkdriver/driver/integrity.py
--rw-rw-rw-   0        0        0     6305 2023-04-14 06:18:29.000000 arkdriver-1.0.3/src/arkdriver/main.py
-drwxrwxrwx   0        0        0        0 2023-04-15 23:36:49.383340 arkdriver-1.0.3/src/arkdriver/presentation/
--rw-rw-rw-   0        0        0        0 2023-03-31 07:17:37.000000 arkdriver-1.0.3/src/arkdriver/presentation/__init__.py
--rw-rw-rw-   0        0        0    12071 2023-04-02 00:47:11.000000 arkdriver-1.0.3/src/arkdriver/presentation/presentation.py
--rw-rw-rw-   0        0        0        0 2023-03-25 16:35:50.000000 arkdriver-1.0.3/src/arkdriver/py.typed
-drwxrwxrwx   0        0        0        0 2023-04-15 23:36:49.378342 arkdriver-1.0.3/src/arkdriver.egg-info/
--rw-rw-rw-   0        0        0     1935 2023-04-15 23:36:49.000000 arkdriver-1.0.3/src/arkdriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2023-04-15 23:36:49.000000 arkdriver-1.0.3/src/arkdriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 23:36:49.000000 arkdriver-1.0.3/src/arkdriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      175 2023-04-15 23:36:49.000000 arkdriver-1.0.3/src/arkdriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-15 23:36:49.000000 arkdriver-1.0.3/src/arkdriver.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 23:36:49.384339 arkdriver-1.0.3/tests/
--rw-rw-rw-   0        0        0      342 2023-03-25 16:35:50.000000 arkdriver-1.0.3/tests/test_lib.py
--rw-rw-rw-   0        0        0      580 2023-03-25 16:35:50.000000 arkdriver-1.0.3/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2023-04-16 02:11:45.040204 arkdriver-1.0.4/
+-rw-rw-rw-   0        0        0     1095 2023-03-25 16:35:50.000000 arkdriver-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1935 2023-04-16 02:11:45.040204 arkdriver-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1305 2023-03-25 16:35:50.000000 arkdriver-1.0.4/README.md
+-rw-rw-rw-   0        0        0      669 2023-04-16 02:10:28.000000 arkdriver-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1186 2023-04-16 02:11:45.042205 arkdriver-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 02:11:45.012205 arkdriver-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 02:11:45.019208 arkdriver-1.0.4/src/arkdriver/
+-rw-rw-rw-   0        0        0      128 2023-04-06 04:15:05.000000 arkdriver-1.0.4/src/arkdriver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 02:11:45.036206 arkdriver-1.0.4/src/arkdriver/driver/
+-rw-rw-rw-   0        0        0      137 2023-03-31 17:34:17.000000 arkdriver-1.0.4/src/arkdriver/driver/__init__.py
+-rw-rw-rw-   0        0        0    10696 2023-04-14 00:06:06.000000 arkdriver-1.0.4/src/arkdriver/driver/application.py
+-rw-rw-rw-   0        0        0     2830 2023-03-31 21:05:16.000000 arkdriver-1.0.4/src/arkdriver/driver/driver.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 23:37:23.000000 arkdriver-1.0.4/src/arkdriver/driver/integrity.py
+-rw-rw-rw-   0        0        0     6305 2023-04-14 06:18:29.000000 arkdriver-1.0.4/src/arkdriver/main.py
+drwxrwxrwx   0        0        0        0 2023-04-16 02:11:45.038204 arkdriver-1.0.4/src/arkdriver/presentation/
+-rw-rw-rw-   0        0        0        0 2023-03-31 07:17:37.000000 arkdriver-1.0.4/src/arkdriver/presentation/__init__.py
+-rw-rw-rw-   0        0        0    12071 2023-04-02 00:47:11.000000 arkdriver-1.0.4/src/arkdriver/presentation/presentation.py
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:35:50.000000 arkdriver-1.0.4/src/arkdriver/py.typed
+drwxrwxrwx   0        0        0        0 2023-04-16 02:11:45.033208 arkdriver-1.0.4/src/arkdriver.egg-info/
+-rw-rw-rw-   0        0        0     1935 2023-04-16 02:11:44.000000 arkdriver-1.0.4/src/arkdriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2023-04-16 02:11:45.000000 arkdriver-1.0.4/src/arkdriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 02:11:44.000000 arkdriver-1.0.4/src/arkdriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      157 2023-04-16 02:11:44.000000 arkdriver-1.0.4/src/arkdriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-16 02:11:44.000000 arkdriver-1.0.4/src/arkdriver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 02:11:45.039206 arkdriver-1.0.4/tests/
+-rw-rw-rw-   0        0        0      342 2023-03-25 16:35:50.000000 arkdriver-1.0.4/tests/test_lib.py
+-rw-rw-rw-   0        0        0      580 2023-03-25 16:35:50.000000 arkdriver-1.0.4/tests/test_main.py
```

### Comparing `arkdriver-1.0.3/LICENSE` & `arkdriver-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.3/PKG-INFO` & `arkdriver-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkdriver
-Version: 1.0.3
+Version: 1.0.4
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/mjlomeli/arkdriver
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/arkdriver/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `arkdriver-1.0.3/README.md` & `arkdriver-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.3/pyproject.toml` & `arkdriver-1.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [build-system]
 requires = [
     "setuptools>=42",
     "wheel",
     "requests>=2.28.1",
     "arklibrary==1.*",
-    "arkclient>=0.0.35",
     "pywinauto",
     "pywin32",
     "six",
     "comtypes",
     "numpy>=1.24.2"
 ]
 build-backend = "setuptools.build_meta"
```

### Comparing `arkdriver-1.0.3/setup.cfg` & `arkdriver-1.0.4/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 726b 6472 6976 6572 0d0a 7665   = arkdriver..ve
-00000020: 7273 696f 6e20 3d20 312e 302e 330d 0a74  rsion = 1.0.3..t
+00000020: 7273 696f 6e20 3d20 312e 302e 340d 0a74  rsion = 1.0.4..t
 00000030: 6573 745f 7665 7273 696f 6e20 3d20 312e  est_version = 1.
-00000040: 302e 340d 0a70 726f 6475 6374 696f 6e5f  0.4..production_
-00000050: 7665 7273 696f 6e20 3d20 312e 302e 330d  version = 1.0.3.
+00000040: 302e 350d 0a70 726f 6475 6374 696f 6e5f  0.5..production_
+00000050: 7665 7273 696f 6e20 3d20 312e 302e 340d  version = 1.0.4.
 00000060: 0a61 7574 686f 7220 3d20 4d61 7572 6963  .author = Mauric
 00000070: 696f 0d0a 6175 7468 6f72 5f65 6d61 696c  io..author_email
 00000080: 203d 2064 6576 2e6d 6175 7269 6369 6f2e   = dev.mauricio.
 00000090: 6c6f 6d65 6c69 4067 6d61 696c 2e63 6f6d  lomeli@gmail.com
 000000a0: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 000000b0: 5468 6973 2061 7070 6c69 6361 7469 6f6e  This application
 000000c0: 2061 6363 6573 7365 7320 7468 6520 4172   accesses the Ar
@@ -42,35 +42,34 @@
 00000290: 630d 0a70 6163 6b61 6765 7320 3d20 6669  c..packages = fi
 000002a0: 6e64 3a0d 0a70 7974 686f 6e5f 7265 7175  nd:..python_requ
 000002b0: 6972 6573 203d 203e 3d33 2e39 0d0a 696e  ires = >=3.9..in
 000002c0: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
 000002d0: 200d 0a09 7768 6565 6c0d 0a09 7265 7175   ...wheel...requ
 000002e0: 6573 7473 3e3d 322e 3238 2e31 0d0a 0961  ests>=2.28.1...a
 000002f0: 726b 6c69 6272 6172 793d 3d31 2e2a 0d0a  rklibrary==1.*..
-00000300: 0961 726b 636c 6965 6e74 3e3d 302e 302e  .arkclient>=0.0.
-00000310: 3335 0d0a 0970 7977 696e 6175 746f 0d0a  35...pywinauto..
-00000320: 0970 7977 696e 3332 0d0a 0973 6978 0d0a  .pywin32...six..
-00000330: 0963 6f6d 7479 7065 730d 0a09 6e75 6d70  .comtypes...nump
-00000340: 793e 3d31 2e32 342e 320d 0a0d 0a5b 6f70  y>=1.24.2....[op
-00000350: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
-00000360: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
-00000370: 630d 0a0d 0a5b 6f70 7469 6f6e 732e 6578  c....[options.ex
-00000380: 7472 6173 5f72 6571 7569 7265 5d0d 0a74  tras_require]..t
-00000390: 6573 7469 6e67 203d 200d 0a09 7079 7465  esting = ...pyte
-000003a0: 7374 3e3d 362e 300d 0a09 7079 7465 7374  st>=6.0...pytest
-000003b0: 2d63 6f76 3e3d 322e 300d 0a09 6d79 7079  -cov>=2.0...mypy
-000003c0: 3e3d 302e 3937 310d 0a09 666c 616b 6538  >=0.971...flake8
-000003d0: 3e3d 332e 390d 0a09 746f 783e 3d33 2e32  >=3.9...tox>=3.2
-000003e0: 340d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  4....[options.pa
-000003f0: 636b 6167 655f 6461 7461 5d0d 0a61 726b  ckage_data]..ark
-00000400: 6472 6976 6572 203d 2070 792e 7479 7065  driver = py.type
-00000410: 642c 2061 726b 2e6c 6e6b 2c20 636f 6e66  d, ark.lnk, conf
-00000420: 6967 2e69 6e69 2c20 7079 7769 6e33 322d  ig.ini, pywin32-
-00000430: 3330 342e 7769 6e33 322d 7079 332e 392e  304.win32-py3.9.
-00000440: 6578 652c 2070 7977 696e 3332 2d33 3034  exe, pywin32-304
-00000450: 2e77 696e 2d61 6d64 3634 2d70 7933 2e31  .win-amd64-py3.1
-00000460: 302e 6578 650d 0a0d 0a5b 666c 616b 6538  0.exe....[flake8
-00000470: 5d0d 0a6d 6178 2d6c 696e 652d 6c65 6e67  ]..max-line-leng
-00000480: 7468 203d 2031 3630 0d0a 0d0a 5b65 6767  th = 160....[egg
-00000490: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-000004a0: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-000004b0: 2030 0d0a 0d0a                            0....
+00000300: 0970 7977 696e 6175 746f 0d0a 0970 7977  .pywinauto...pyw
+00000310: 696e 3332 0d0a 0973 6978 0d0a 0963 6f6d  in32...six...com
+00000320: 7479 7065 730d 0a09 6e75 6d70 793e 3d31  types...numpy>=1
+00000330: 2e32 342e 320d 0a0d 0a5b 6f70 7469 6f6e  .24.2....[option
+00000340: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+00000350: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
+00000360: 0a5b 6f70 7469 6f6e 732e 6578 7472 6173  .[options.extras
+00000370: 5f72 6571 7569 7265 5d0d 0a74 6573 7469  _require]..testi
+00000380: 6e67 203d 200d 0a09 7079 7465 7374 3e3d  ng = ...pytest>=
+00000390: 362e 300d 0a09 7079 7465 7374 2d63 6f76  6.0...pytest-cov
+000003a0: 3e3d 322e 300d 0a09 6d79 7079 3e3d 302e  >=2.0...mypy>=0.
+000003b0: 3937 310d 0a09 666c 616b 6538 3e3d 332e  971...flake8>=3.
+000003c0: 390d 0a09 746f 783e 3d33 2e32 340d 0a0d  9...tox>=3.24...
+000003d0: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
+000003e0: 655f 6461 7461 5d0d 0a61 726b 6472 6976  e_data]..arkdriv
+000003f0: 6572 203d 2070 792e 7479 7065 642c 2061  er = py.typed, a
+00000400: 726b 2e6c 6e6b 2c20 636f 6e66 6967 2e69  rk.lnk, config.i
+00000410: 6e69 2c20 7079 7769 6e33 322d 3330 342e  ni, pywin32-304.
+00000420: 7769 6e33 322d 7079 332e 392e 6578 652c  win32-py3.9.exe,
+00000430: 2070 7977 696e 3332 2d33 3034 2e77 696e   pywin32-304.win
+00000440: 2d61 6d64 3634 2d70 7933 2e31 302e 6578  -amd64-py3.10.ex
+00000450: 650d 0a0d 0a5b 666c 616b 6538 5d0d 0a6d  e....[flake8]..m
+00000460: 6178 2d6c 696e 652d 6c65 6e67 7468 203d  ax-line-length =
+00000470: 2031 3630 0d0a 0d0a 5b65 6767 5f69 6e66   160....[egg_inf
+00000480: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
+00000490: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
+000004a0: 0d0a                                     ..
```

### Comparing `arkdriver-1.0.3/src/arkdriver/driver/application.py` & `arkdriver-1.0.4/src/arkdriver/driver/application.py`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.3/src/arkdriver/driver/driver.py` & `arkdriver-1.0.4/src/arkdriver/driver/driver.py`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.3/src/arkdriver/main.py` & `arkdriver-1.0.4/src/arkdriver/main.py`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.3/src/arkdriver/presentation/presentation.py` & `arkdriver-1.0.4/src/arkdriver/presentation/presentation.py`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.3/src/arkdriver.egg-info/PKG-INFO` & `arkdriver-1.0.4/src/arkdriver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkdriver
-Version: 1.0.3
+Version: 1.0.4
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/mjlomeli/arkdriver
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/arkdriver/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `arkdriver-1.0.3/src/arkdriver.egg-info/SOURCES.txt` & `arkdriver-1.0.4/src/arkdriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.3/tests/test_main.py` & `arkdriver-1.0.4/tests/test_main.py`

 * *Files identical despite different names*

