# Comparing `tmp/arkdriver-1.0.1.tar.gz` & `tmp/arkdriver-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkdriver-1.0.1.tar", last modified: Sat Apr 15 23:09:04 2023, max compression
+gzip compressed data, was "arkdriver-1.0.2.tar", last modified: Sat Apr 15 23:34:03 2023, max compression
```

## Comparing `arkdriver-1.0.1.tar` & `arkdriver-1.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 23:09:04.386896 arkdriver-1.0.1/
--rw-rw-rw-   0        0        0     1095 2023-03-25 16:35:50.000000 arkdriver-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2088 2023-04-15 23:09:04.386896 arkdriver-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1305 2023-03-25 16:35:50.000000 arkdriver-1.0.1/README.md
--rw-rw-rw-   0        0        0      698 2023-04-11 00:25:28.000000 arkdriver-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1329 2023-04-15 23:09:04.391896 arkdriver-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 23:09:04.362897 arkdriver-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 23:09:04.368896 arkdriver-1.0.1/src/arkdriver/
--rw-rw-rw-   0        0        0      128 2023-04-06 04:15:05.000000 arkdriver-1.0.1/src/arkdriver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 23:09:04.382897 arkdriver-1.0.1/src/arkdriver/driver/
--rw-rw-rw-   0        0        0      137 2023-03-31 17:34:17.000000 arkdriver-1.0.1/src/arkdriver/driver/__init__.py
--rw-rw-rw-   0        0        0    10696 2023-04-14 00:06:06.000000 arkdriver-1.0.1/src/arkdriver/driver/application.py
--rw-rw-rw-   0        0        0     2830 2023-03-31 21:05:16.000000 arkdriver-1.0.1/src/arkdriver/driver/driver.py
--rw-rw-rw-   0        0        0        0 2023-04-13 23:37:23.000000 arkdriver-1.0.1/src/arkdriver/driver/integrity.py
--rw-rw-rw-   0        0        0     6305 2023-04-14 06:18:29.000000 arkdriver-1.0.1/src/arkdriver/main.py
-drwxrwxrwx   0        0        0        0 2023-04-15 23:09:04.383897 arkdriver-1.0.1/src/arkdriver/presentation/
--rw-rw-rw-   0        0        0        0 2023-03-31 07:17:37.000000 arkdriver-1.0.1/src/arkdriver/presentation/__init__.py
--rw-rw-rw-   0        0        0    12071 2023-04-02 00:47:11.000000 arkdriver-1.0.1/src/arkdriver/presentation/presentation.py
--rw-rw-rw-   0        0        0        0 2023-03-25 16:35:50.000000 arkdriver-1.0.1/src/arkdriver/py.typed
-drwxrwxrwx   0        0        0        0 2023-04-15 23:09:04.379902 arkdriver-1.0.1/src/arkdriver.egg-info/
--rw-rw-rw-   0        0        0     2088 2023-04-15 23:09:04.000000 arkdriver-1.0.1/src/arkdriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2023-04-15 23:09:04.000000 arkdriver-1.0.1/src/arkdriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 23:09:04.000000 arkdriver-1.0.1/src/arkdriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      178 2023-04-15 23:09:04.000000 arkdriver-1.0.1/src/arkdriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-15 23:09:04.000000 arkdriver-1.0.1/src/arkdriver.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 23:09:04.385898 arkdriver-1.0.1/tests/
--rw-rw-rw-   0        0        0      342 2023-03-25 16:35:50.000000 arkdriver-1.0.1/tests/test_lib.py
--rw-rw-rw-   0        0        0      580 2023-03-25 16:35:50.000000 arkdriver-1.0.1/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2023-04-15 23:34:03.586219 arkdriver-1.0.2/
+-rw-rw-rw-   0        0        0     1095 2023-03-25 16:35:50.000000 arkdriver-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1986 2023-04-15 23:34:03.586219 arkdriver-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1305 2023-03-25 16:35:50.000000 arkdriver-1.0.2/README.md
+-rw-rw-rw-   0        0        0      695 2023-04-15 23:30:02.000000 arkdriver-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1246 2023-04-15 23:34:03.592217 arkdriver-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-15 23:34:03.555219 arkdriver-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 23:34:03.562218 arkdriver-1.0.2/src/arkdriver/
+-rw-rw-rw-   0        0        0      128 2023-04-06 04:15:05.000000 arkdriver-1.0.2/src/arkdriver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 23:34:03.582221 arkdriver-1.0.2/src/arkdriver/driver/
+-rw-rw-rw-   0        0        0      137 2023-03-31 17:34:17.000000 arkdriver-1.0.2/src/arkdriver/driver/__init__.py
+-rw-rw-rw-   0        0        0    10696 2023-04-14 00:06:06.000000 arkdriver-1.0.2/src/arkdriver/driver/application.py
+-rw-rw-rw-   0        0        0     2830 2023-03-31 21:05:16.000000 arkdriver-1.0.2/src/arkdriver/driver/driver.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 23:37:23.000000 arkdriver-1.0.2/src/arkdriver/driver/integrity.py
+-rw-rw-rw-   0        0        0     6305 2023-04-14 06:18:29.000000 arkdriver-1.0.2/src/arkdriver/main.py
+drwxrwxrwx   0        0        0        0 2023-04-15 23:34:03.584217 arkdriver-1.0.2/src/arkdriver/presentation/
+-rw-rw-rw-   0        0        0        0 2023-03-31 07:17:37.000000 arkdriver-1.0.2/src/arkdriver/presentation/__init__.py
+-rw-rw-rw-   0        0        0    12071 2023-04-02 00:47:11.000000 arkdriver-1.0.2/src/arkdriver/presentation/presentation.py
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:35:50.000000 arkdriver-1.0.2/src/arkdriver/py.typed
+drwxrwxrwx   0        0        0        0 2023-04-15 23:34:03.579216 arkdriver-1.0.2/src/arkdriver.egg-info/
+-rw-rw-rw-   0        0        0     1986 2023-04-15 23:34:03.000000 arkdriver-1.0.2/src/arkdriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2023-04-15 23:34:03.000000 arkdriver-1.0.2/src/arkdriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 23:34:03.000000 arkdriver-1.0.2/src/arkdriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      175 2023-04-15 23:34:03.000000 arkdriver-1.0.2/src/arkdriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-15 23:34:03.000000 arkdriver-1.0.2/src/arkdriver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 23:34:03.585217 arkdriver-1.0.2/tests/
+-rw-rw-rw-   0        0        0      342 2023-03-25 16:35:50.000000 arkdriver-1.0.2/tests/test_lib.py
+-rw-rw-rw-   0        0        0      580 2023-03-25 16:35:50.000000 arkdriver-1.0.2/tests/test_main.py
```

### Comparing `arkdriver-1.0.1/LICENSE` & `arkdriver-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.1/PKG-INFO` & `arkdriver-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: arkdriver
-Version: 1.0.1
+Version: 1.0.2
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/mjlomeli/arkdriver
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/arkdriver/issues
 Platform: win32
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `arkdriver-1.0.1/README.md` & `arkdriver-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.1/pyproject.toml` & `arkdriver-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = [
     "setuptools>=42",
     "wheel",
     "requests>=2.28.1",
-    "arklibrary>=0.0.62",
+    "arklibrary==1.*",
     "arkclient>=0.0.35",
     "pywinauto",
     "pywin32",
     "six",
     "comtypes",
     "numpy>=1.24.2"
 ]
```

### Comparing `arkdriver-1.0.1/setup.cfg` & `arkdriver-1.0.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 726b 6472 6976 6572 0d0a 7665   = arkdriver..ve
-00000020: 7273 696f 6e20 3d20 312e 302e 310d 0a74  rsion = 1.0.1..t
+00000020: 7273 696f 6e20 3d20 312e 302e 320d 0a74  rsion = 1.0.2..t
 00000030: 6573 745f 7665 7273 696f 6e20 3d20 312e  est_version = 1.
-00000040: 302e 310d 0a70 726f 6475 6374 696f 6e5f  0.1..production_
-00000050: 7665 7273 696f 6e20 3d20 312e 302e 310d  version = 1.0.1.
+00000040: 302e 330d 0a70 726f 6475 6374 696f 6e5f  0.3..production_
+00000050: 7665 7273 696f 6e20 3d20 312e 302e 320d  version = 1.0.2.
 00000060: 0a61 7574 686f 7220 3d20 4d61 7572 6963  .author = Mauric
 00000070: 696f 0d0a 6175 7468 6f72 5f65 6d61 696c  io..author_email
 00000080: 203d 2064 6576 2e6d 6175 7269 6369 6f2e   = dev.mauricio.
 00000090: 6c6f 6d65 6c69 4067 6d61 696c 2e63 6f6d  lomeli@gmail.com
 000000a0: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 000000b0: 5468 6973 2061 7070 6c69 6361 7469 6f6e  This application
 000000c0: 2061 6363 6573 7365 7320 7468 6520 4172   accesses the Ar
@@ -25,60 +25,54 @@
 00000180: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d6a  ://github.com/mj
 00000190: 6c6f 6d65 6c69 2f61 726b 6472 6976 6572  lomeli/arkdriver
 000001a0: 2f69 7373 7565 730d 0a70 6c61 7466 6f72  /issues..platfor
 000001b0: 6d73 203d 2077 696e 3332 0d0a 636c 6173  ms = win32..clas
 000001c0: 7369 6669 6572 7320 3d20 0d0a 0950 726f  sifiers = ...Pro
 000001d0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
 000001e0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000001f0: 2e36 0d0a 0950 726f 6772 616d 6d69 6e67  .6...Programming
+000001f0: 2e38 0d0a 0950 726f 6772 616d 6d69 6e67  .8...Programming
 00000200: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000210: 686f 6e20 3a3a 2033 2e37 0d0a 0950 726f  hon :: 3.7...Pro
+00000210: 686f 6e20 3a3a 2033 2e39 0d0a 0950 726f  hon :: 3.9...Pro
 00000220: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
 00000230: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000240: 2e38 0d0a 0950 726f 6772 616d 6d69 6e67  .8...Programming
-00000250: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000260: 686f 6e20 3a3a 2033 2e39 0d0a 0950 726f  hon :: 3.9...Pro
-00000270: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000280: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000290: 2e31 300d 0a09 0d0a 094c 6963 656e 7365  .10......License
-000002a0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-000002b0: 203a 3a20 4d49 5420 4c69 6365 6e73 650d   :: MIT License.
-000002c0: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
-000002d0: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
-000002e0: 6465 6e74 0d0a 0d0a 5b6f 7074 696f 6e73  dent....[options
-000002f0: 5d0d 0a70 6163 6b61 6765 5f64 6972 203d  ]..package_dir =
-00000300: 200d 0a09 3d20 7372 630d 0a70 6163 6b61   ...= src..packa
-00000310: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
-00000320: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-00000330: 3d33 2e36 0d0a 696e 7374 616c 6c5f 7265  =3.6..install_re
-00000340: 7175 6972 6573 203d 200d 0a09 7768 6565  quires = ...whee
-00000350: 6c0d 0a09 7265 7175 6573 7473 3e3d 322e  l...requests>=2.
-00000360: 3238 2e31 0d0a 0961 726b 6c69 6272 6172  28.1...arklibrar
-00000370: 793e 3d30 2e30 2e36 320d 0a09 6172 6b63  y>=0.0.62...arkc
-00000380: 6c69 656e 743e 3d30 2e30 2e33 350d 0a09  lient>=0.0.35...
-00000390: 7079 7769 6e61 7574 6f0d 0a09 7079 7769  pywinauto...pywi
-000003a0: 6e33 320d 0a09 7369 780d 0a09 636f 6d74  n32...six...comt
-000003b0: 7970 6573 0d0a 096e 756d 7079 3e3d 312e  ypes...numpy>=1.
-000003c0: 3234 2e32 0d0a 0d0a 5b6f 7074 696f 6e73  24.2....[options
-000003d0: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
-000003e0: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
-000003f0: 5b6f 7074 696f 6e73 2e65 7874 7261 735f  [options.extras_
-00000400: 7265 7175 6972 655d 0d0a 7465 7374 696e  require]..testin
-00000410: 6720 3d20 0d0a 0970 7974 6573 743e 3d36  g = ...pytest>=6
-00000420: 2e30 0d0a 0970 7974 6573 742d 636f 763e  .0...pytest-cov>
-00000430: 3d32 2e30 0d0a 096d 7970 793e 3d30 2e39  =2.0...mypy>=0.9
-00000440: 3731 0d0a 0966 6c61 6b65 383e 3d33 2e39  71...flake8>=3.9
-00000450: 0d0a 0974 6f78 3e3d 332e 3234 0d0a 0d0a  ...tox>=3.24....
-00000460: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-00000470: 5f64 6174 615d 0d0a 6172 6b64 7269 7665  _data]..arkdrive
-00000480: 7220 3d20 7079 2e74 7970 6564 2c20 6172  r = py.typed, ar
-00000490: 6b2e 6c6e 6b2c 2063 6f6e 6669 672e 696e  k.lnk, config.in
-000004a0: 692c 2070 7977 696e 3332 2d33 3034 2e77  i, pywin32-304.w
-000004b0: 696e 3332 2d70 7933 2e39 2e65 7865 2c20  in32-py3.9.exe, 
-000004c0: 7079 7769 6e33 322d 3330 342e 7769 6e2d  pywin32-304.win-
-000004d0: 616d 6436 342d 7079 332e 3130 2e65 7865  amd64-py3.10.exe
-000004e0: 0d0a 0d0a 5b66 6c61 6b65 385d 0d0a 6d61  ....[flake8]..ma
-000004f0: 782d 6c69 6e65 2d6c 656e 6774 6820 3d20  x-line-length = 
-00000500: 3136 300d 0a0d 0a5b 6567 675f 696e 666f  160....[egg_info
-00000510: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-00000520: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-00000530: 0a                                       .
+00000240: 2e31 300d 0a09 0d0a 094c 6963 656e 7365  .10......License
+00000250: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+00000260: 203a 3a20 4d49 5420 4c69 6365 6e73 650d   :: MIT License.
+00000270: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
+00000280: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
+00000290: 6465 6e74 0d0a 0d0a 5b6f 7074 696f 6e73  dent....[options
+000002a0: 5d0d 0a70 6163 6b61 6765 5f64 6972 203d  ]..package_dir =
+000002b0: 200d 0a09 3d20 7372 630d 0a70 6163 6b61   ...= src..packa
+000002c0: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
+000002d0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+000002e0: 3d33 2e36 0d0a 696e 7374 616c 6c5f 7265  =3.6..install_re
+000002f0: 7175 6972 6573 203d 200d 0a09 7768 6565  quires = ...whee
+00000300: 6c0d 0a09 7265 7175 6573 7473 3e3d 322e  l...requests>=2.
+00000310: 3238 2e31 0d0a 0961 726b 6c69 6272 6172  28.1...arklibrar
+00000320: 793d 3d31 2e2a 0d0a 0961 726b 636c 6965  y==1.*...arkclie
+00000330: 6e74 3e3d 302e 302e 3335 0d0a 0970 7977  nt>=0.0.35...pyw
+00000340: 696e 6175 746f 0d0a 0970 7977 696e 3332  inauto...pywin32
+00000350: 0d0a 0973 6978 0d0a 0963 6f6d 7479 7065  ...six...comtype
+00000360: 730d 0a09 6e75 6d70 793e 3d31 2e32 342e  s...numpy>=1.24.
+00000370: 320d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  2....[options.pa
+00000380: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
+00000390: 6572 6520 3d20 7372 630d 0a0d 0a5b 6f70  ere = src....[op
+000003a0: 7469 6f6e 732e 6578 7472 6173 5f72 6571  tions.extras_req
+000003b0: 7569 7265 5d0d 0a74 6573 7469 6e67 203d  uire]..testing =
+000003c0: 200d 0a09 7079 7465 7374 3e3d 362e 300d   ...pytest>=6.0.
+000003d0: 0a09 7079 7465 7374 2d63 6f76 3e3d 322e  ..pytest-cov>=2.
+000003e0: 300d 0a09 6d79 7079 3e3d 302e 3937 310d  0...mypy>=0.971.
+000003f0: 0a09 666c 616b 6538 3e3d 332e 390d 0a09  ..flake8>=3.9...
+00000400: 746f 783e 3d33 2e32 340d 0a0d 0a5b 6f70  tox>=3.24....[op
+00000410: 7469 6f6e 732e 7061 636b 6167 655f 6461  tions.package_da
+00000420: 7461 5d0d 0a61 726b 6472 6976 6572 203d  ta]..arkdriver =
+00000430: 2070 792e 7479 7065 642c 2061 726b 2e6c   py.typed, ark.l
+00000440: 6e6b 2c20 636f 6e66 6967 2e69 6e69 2c20  nk, config.ini, 
+00000450: 7079 7769 6e33 322d 3330 342e 7769 6e33  pywin32-304.win3
+00000460: 322d 7079 332e 392e 6578 652c 2070 7977  2-py3.9.exe, pyw
+00000470: 696e 3332 2d33 3034 2e77 696e 2d61 6d64  in32-304.win-amd
+00000480: 3634 2d70 7933 2e31 302e 6578 650d 0a0d  64-py3.10.exe...
+00000490: 0a5b 666c 616b 6538 5d0d 0a6d 6178 2d6c  .[flake8]..max-l
+000004a0: 696e 652d 6c65 6e67 7468 203d 2031 3630  ine-length = 160
+000004b0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+000004c0: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+000004d0: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

### Comparing `arkdriver-1.0.1/src/arkdriver/driver/application.py` & `arkdriver-1.0.2/src/arkdriver/driver/application.py`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.1/src/arkdriver/driver/driver.py` & `arkdriver-1.0.2/src/arkdriver/driver/driver.py`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.1/src/arkdriver/main.py` & `arkdriver-1.0.2/src/arkdriver/main.py`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.1/src/arkdriver/presentation/presentation.py` & `arkdriver-1.0.2/src/arkdriver/presentation/presentation.py`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.1/src/arkdriver.egg-info/PKG-INFO` & `arkdriver-1.0.2/src/arkdriver.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: arkdriver
-Version: 1.0.1
+Version: 1.0.2
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/mjlomeli/arkdriver
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/arkdriver/issues
 Platform: win32
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `arkdriver-1.0.1/src/arkdriver.egg-info/SOURCES.txt` & `arkdriver-1.0.2/src/arkdriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.1/tests/test_main.py` & `arkdriver-1.0.2/tests/test_main.py`

 * *Files identical despite different names*

