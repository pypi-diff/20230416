# Comparing `tmp/nitrado-0.0.9.tar.gz` & `tmp/nitrado-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitrado-0.0.9.tar", last modified: Mon Aug 15 04:36:23 2022, max compression
+gzip compressed data, was "nitrado-1.0.1.tar", last modified: Sun Apr 16 09:35:14 2023, max compression
```

## Comparing `nitrado-0.0.9.tar` & `nitrado-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,31 @@
-drwxrwxrwx   0        0        0        0 2022-08-15 04:36:23.544632 nitrado-0.0.9/
--rw-rw-rw-   0        0        0     1093 2022-07-31 22:27:45.000000 nitrado-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     4509 2022-08-15 04:36:23.544632 nitrado-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     3555 2022-07-31 22:27:45.000000 nitrado-0.0.9/README.md
--rw-rw-rw-   0        0        0      533 2022-07-31 22:27:45.000000 nitrado-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0     1200 2022-08-15 04:36:23.545632 nitrado-0.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-15 04:36:23.519631 nitrado-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2022-08-15 04:36:23.527633 nitrado-0.0.9/src/nitrado/
--rw-rw-rw-   0        0        0      338 2022-07-31 22:27:45.000000 nitrado-0.0.9/src/nitrado/__init__.py
--rw-rw-rw-   0        0        0     2272 2022-07-31 22:27:45.000000 nitrado-0.0.9/src/nitrado/client.py
--rw-rw-rw-   0        0        0    25129 2022-07-31 22:27:45.000000 nitrado-0.0.9/src/nitrado/game_server.py
--rw-rw-rw-   0        0        0     2523 2022-07-31 22:27:45.000000 nitrado-0.0.9/src/nitrado/nitrado_api.py
--rw-rw-rw-   0        0        0        0 2022-07-31 22:27:45.000000 nitrado-0.0.9/src/nitrado/py.typed
--rw-rw-rw-   0        0        0     5968 2022-07-31 22:27:45.000000 nitrado-0.0.9/src/nitrado/service.py
-drwxrwxrwx   0        0        0        0 2022-08-15 04:36:23.543631 nitrado-0.0.9/src/nitrado.egg-info/
--rw-rw-rw-   0        0        0     4509 2022-08-15 04:36:23.000000 nitrado-0.0.9/src/nitrado.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2022-08-15 04:36:23.000000 nitrado-0.0.9/src/nitrado.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-15 04:36:23.000000 nitrado-0.0.9/src/nitrado.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2022-08-15 04:36:23.000000 nitrado-0.0.9/src/nitrado.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-08-15 04:36:23.000000 nitrado-0.0.9/src/nitrado.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 09:35:14.264843 nitrado-1.0.1/
+-rw-rw-rw-   0        0        0     1093 2023-03-25 00:21:47.000000 nitrado-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     4401 2023-04-16 09:35:14.265847 nitrado-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3600 2023-03-25 00:21:47.000000 nitrado-1.0.1/README.md
+-rw-rw-rw-   0        0        0      555 2023-04-16 01:48:34.000000 nitrado-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1135 2023-04-16 09:35:14.266848 nitrado-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 09:35:14.231401 nitrado-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 09:35:14.240427 nitrado-1.0.1/src/nitrado/
+-rw-rw-rw-   0        0        0      236 2023-03-25 08:45:32.000000 nitrado-1.0.1/src/nitrado/__init__.py
+-rw-rw-rw-   0        0        0       30 2023-03-25 08:45:32.000000 nitrado-1.0.1/src/nitrado/ark_server.py
+drwxrwxrwx   0        0        0        0 2023-04-16 09:35:14.259326 nitrado-1.0.1/src/nitrado/lib/
+-rw-rw-rw-   0        0        0       91 2023-03-25 00:51:09.000000 nitrado-1.0.1/src/nitrado/lib/__init__.py
+-rw-rw-rw-   0        0        0     1347 2023-04-16 03:40:10.000000 nitrado-1.0.1/src/nitrado/lib/errors.py
+-rw-rw-rw-   0        0        0    21890 2023-04-16 09:32:56.000000 nitrado-1.0.1/src/nitrado/lib/game_server.py
+-rw-rw-rw-   0        0        0     3919 2023-04-16 09:31:37.000000 nitrado-1.0.1/src/nitrado/lib/service.py
+-rw-rw-rw-   0        0        0     2823 2023-04-16 05:06:33.000000 nitrado-1.0.1/src/nitrado/nitrado_api.py
+-rw-rw-rw-   0        0        0        0 2023-03-25 00:21:47.000000 nitrado-1.0.1/src/nitrado/py.typed
+drwxrwxrwx   0        0        0        0 2023-04-16 09:35:14.260325 nitrado-1.0.1/src/nitrado/tools/
+-rw-rw-rw-   0        0        0       43 2023-03-25 00:37:24.000000 nitrado-1.0.1/src/nitrado/tools/__init__.py
+-rw-rw-rw-   0        0        0     1564 2023-04-16 05:08:15.000000 nitrado-1.0.1/src/nitrado/tools/client.py
+drwxrwxrwx   0        0        0        0 2023-04-16 09:35:14.255327 nitrado-1.0.1/src/nitrado.egg-info/
+-rw-rw-rw-   0        0        0     4401 2023-04-16 09:35:14.000000 nitrado-1.0.1/src/nitrado.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      583 2023-04-16 09:35:14.000000 nitrado-1.0.1/src/nitrado.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 09:35:14.000000 nitrado-1.0.1/src/nitrado.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-04-16 09:35:14.000000 nitrado-1.0.1/src/nitrado.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-16 09:35:14.000000 nitrado-1.0.1/src/nitrado.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 09:35:14.264843 nitrado-1.0.1/tests/
+-rw-rw-rw-   0        0        0     2251 2023-04-16 05:41:31.000000 nitrado-1.0.1/tests/test_connection.py
+-rw-rw-rw-   0        0        0    19592 2023-04-16 09:33:34.000000 nitrado-1.0.1/tests/test_game_server.py
+-rw-rw-rw-   0        0        0      106 2023-03-25 08:45:33.000000 nitrado-1.0.1/tests/test_nitrado_api.py
+-rw-rw-rw-   0        0        0     2511 2023-03-25 08:45:33.000000 nitrado-1.0.1/tests/test_service.py
```

### Comparing `nitrado-0.0.9/LICENSE` & `nitrado-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nitrado-0.0.9/PKG-INFO` & `nitrado-1.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 Metadata-Version: 2.1
 Name: nitrado
-Version: 0.0.9
+Version: 1.0.1
 Summary: This application accesses the Nitrado API.
 Home-page: https://github.com/mjlomeli/NitradoAPI
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/NitradoAPI/issues
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # Python Nitrado SDK
-[![Testing](https://github.com/mjlomeli/NitradoAPI/actions/workflows/tests.yml/badge.svg)](#)
+
+[![Testing](https://github.com/mjlomeli/NitradoAPI/actions/workflows/tests.yml/badge.svg)](#) tests need a Nitrado subscription account 
 
 
 A Python based SDK for the [Nitrado RESTful API](https://doc.nitrado.net/) published at [PyPI](https://pypi.org/project/nitrado/).
 
 
 # Overview
```

### Comparing `nitrado-0.0.9/README.md` & `nitrado-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Python Nitrado SDK
-[![Testing](https://github.com/mjlomeli/NitradoAPI/actions/workflows/tests.yml/badge.svg)](#)
+
+[![Testing](https://github.com/mjlomeli/NitradoAPI/actions/workflows/tests.yml/badge.svg)](#) tests need a Nitrado subscription account 
 
 
 A Python based SDK for the [Nitrado RESTful API](https://doc.nitrado.net/) published at [PyPI](https://pypi.org/project/nitrado/).
 
 
 # Overview
```

### Comparing `nitrado-0.0.9/pyproject.toml` & `nitrado-1.0.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [build-system]
 requires = [
     "setuptools>=42",
-    "wheel"
+    "wheel",
+    "requests==2.*"
 ]
 build-backend = "setuptools.build_meta"
 
 
 [too.pytest.ini_options]
 addopts = "--cov=nitrado"
 testpaths = [
```

### Comparing `nitrado-0.0.9/setup.cfg` & `nitrado-1.0.1/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,75 +1,71 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6974 7261 646f 0d0a 7665 7273   = nitrado..vers
-00000020: 696f 6e20 3d20 302e 302e 390d 0a61 7574  ion = 0.0.9..aut
-00000030: 686f 7220 3d20 4d61 7572 6963 696f 0d0a  hor = Mauricio..
-00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2064  author_email = d
-00000050: 6576 2e6d 6175 7269 6369 6f2e 6c6f 6d65  ev.mauricio.lome
-00000060: 6c69 4067 6d61 696c 2e63 6f6d 0d0a 6465  li@gmail.com..de
-00000070: 7363 7269 7074 696f 6e20 3d20 5468 6973  scription = This
-00000080: 2061 7070 6c69 6361 7469 6f6e 2061 6363   application acc
-00000090: 6573 7365 7320 7468 6520 4e69 7472 6164  esses the Nitrad
-000000a0: 6f20 4150 492e 0d0a 6c6f 6e67 5f64 6573  o API...long_des
-000000b0: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
-000000c0: 2052 4541 444d 452e 6d64 0d0a 6c6f 6e67   README.md..long
-000000d0: 5f64 6573 6372 6970 7469 6f6e 5f63 6f6e  _description_con
-000000e0: 7465 6e74 5f74 7970 6520 3d20 7465 7874  tent_type = text
-000000f0: 2f6d 6172 6b64 6f77 6e0d 0a75 726c 203d  /markdown..url =
-00000100: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000110: 636f 6d2f 6d6a 6c6f 6d65 6c69 2f4e 6974  com/mjlomeli/Nit
-00000120: 7261 646f 4150 490d 0a70 726f 6a65 6374  radoAPI..project
-00000130: 5f75 726c 7320 3d20 0d0a 0942 7567 2054  _urls = ...Bug T
-00000140: 7261 636b 6572 203d 2068 7474 7073 3a2f  racker = https:/
-00000150: 2f67 6974 6875 622e 636f 6d2f 6d6a 6c6f  /github.com/mjlo
-00000160: 6d65 6c69 2f4e 6974 7261 646f 4150 492f  meli/NitradoAPI/
-00000170: 6973 7375 6573 0d0a 706c 6174 666f 726d  issues..platform
-00000180: 7320 3d20 756e 6978 2c20 6c69 6e75 782c  s = unix, linux,
-00000190: 206f 7378 2c20 6379 6777 696e 2c20 7769   osx, cygwin, wi
-000001a0: 6e33 320d 0a63 6c61 7373 6966 6965 7273  n32..classifiers
-000001b0: 203d 200d 0a09 5072 6f67 7261 6d6d 696e   = ...Programmin
-000001c0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000001d0: 7468 6f6e 203a 3a20 330d 0a09 5072 6f67  thon :: 3...Prog
-000001e0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000001f0: 203a 3a20 5079 7468 6f6e 203a 3a20 3320   :: Python :: 3 
-00000200: 3a3a 204f 6e6c 790d 0a09 5072 6f67 7261  :: Only...Progra
-00000210: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000220: 3a20 5079 7468 6f6e 203a 3a20 332e 360d  : Python :: 3.6.
-00000230: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000240: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000250: 203a 3a20 332e 370d 0a09 5072 6f67 7261   :: 3.7...Progra
-00000260: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000270: 3a20 5079 7468 6f6e 203a 3a20 332e 380d  : Python :: 3.8.
-00000280: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000290: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000002a0: 203a 3a20 332e 390d 0a09 5072 6f67 7261   :: 3.9...Progra
-000002b0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000002c0: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
-000002d0: 0d0a 090d 0a09 4c69 6365 6e73 6520 3a3a  ......License ::
-000002e0: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
-000002f0: 204d 4954 204c 6963 656e 7365 0d0a 094f   MIT License...O
-00000300: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000310: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-00000320: 740d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  t....[options]..
-00000330: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
-00000340: 093d 2073 7263 0d0a 7061 636b 6167 6573  .= src..packages
-00000350: 203d 2066 696e 643a 0d0a 7079 7468 6f6e   = find:..python
-00000360: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
-00000370: 360d 0a69 6e73 7461 6c6c 5f72 6571 7569  6..install_requi
-00000380: 7265 7320 3d20 0d0a 0977 6865 656c 0d0a  res = ...wheel..
-00000390: 0972 6571 7565 7374 730d 0a0d 0a5b 6f70  .requests....[op
-000003a0: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
-000003b0: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
-000003c0: 630d 0a0d 0a5b 6f70 7469 6f6e 732e 6578  c....[options.ex
-000003d0: 7472 6173 5f72 6571 7569 7265 5d0d 0a74  tras_require]..t
-000003e0: 6573 7469 6e67 203d 200d 0a09 7079 7465  esting = ...pyte
-000003f0: 7374 3e3d 362e 300d 0a09 7079 7465 7374  st>=6.0...pytest
-00000400: 2d63 6f76 3e3d 322e 300d 0a09 6d79 7079  -cov>=2.0...mypy
-00000410: 3e3d 302e 3931 300d 0a09 666c 616b 6538  >=0.910...flake8
-00000420: 3e3d 332e 390d 0a09 746f 783e 3d33 2e32  >=3.9...tox>=3.2
-00000430: 340d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  4....[options.pa
-00000440: 636b 6167 655f 6461 7461 5d0d 0a6e 6974  ckage_data]..nit
-00000450: 7261 646f 203d 2070 792e 7479 7065 640d  rado = py.typed.
-00000460: 0a0d 0a5b 666c 616b 6538 5d0d 0a6d 6178  ...[flake8]..max
-00000470: 2d6c 696e 652d 6c65 6e67 7468 203d 2031  -line-length = 1
-00000480: 3630 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  60....[egg_info]
-00000490: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-000004a0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+00000020: 696f 6e20 3d20 312e 302e 310d 0a74 6573  ion = 1.0.1..tes
+00000030: 745f 7665 7273 696f 6e20 3d20 312e 302e  t_version = 1.0.
+00000040: 320d 0a70 726f 6475 6374 696f 6e5f 7665  2..production_ve
+00000050: 7273 696f 6e20 3d20 312e 302e 310d 0a61  rsion = 1.0.1..a
+00000060: 7574 686f 7220 3d20 4d61 7572 6963 696f  uthor = Mauricio
+00000070: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
+00000080: 2064 6576 2e6d 6175 7269 6369 6f2e 6c6f   dev.mauricio.lo
+00000090: 6d65 6c69 4067 6d61 696c 2e63 6f6d 0d0a  meli@gmail.com..
+000000a0: 6465 7363 7269 7074 696f 6e20 3d20 5468  description = Th
+000000b0: 6973 2061 7070 6c69 6361 7469 6f6e 2061  is application a
+000000c0: 6363 6573 7365 7320 7468 6520 4e69 7472  ccesses the Nitr
+000000d0: 6164 6f20 4150 492e 0d0a 6c6f 6e67 5f64  ado API...long_d
+000000e0: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
+000000f0: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
+00000100: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
+00000110: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
+00000120: 7874 2f6d 6172 6b64 6f77 6e0d 0a75 726c  xt/markdown..url
+00000130: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
+00000140: 622e 636f 6d2f 6d6a 6c6f 6d65 6c69 2f4e  b.com/mjlomeli/N
+00000150: 6974 7261 646f 4150 490d 0a70 726f 6a65  itradoAPI..proje
+00000160: 6374 5f75 726c 7320 3d20 0d0a 0942 7567  ct_urls = ...Bug
+00000170: 2054 7261 636b 6572 203d 2068 7474 7073   Tracker = https
+00000180: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d6a  ://github.com/mj
+00000190: 6c6f 6d65 6c69 2f4e 6974 7261 646f 4150  lomeli/NitradoAP
+000001a0: 492f 6973 7375 6573 0d0a 706c 6174 666f  I/issues..platfo
+000001b0: 726d 7320 3d20 756e 6978 2c20 6c69 6e75  rms = unix, linu
+000001c0: 782c 206f 7378 2c20 6379 6777 696e 2c20  x, osx, cygwin, 
+000001d0: 7769 6e33 320d 0a63 6c61 7373 6966 6965  win32..classifie
+000001e0: 7273 203d 200d 0a09 5072 6f67 7261 6d6d  rs = ...Programm
+000001f0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000200: 5079 7468 6f6e 203a 3a20 330d 0a09 5072  Python :: 3...Pr
+00000210: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000220: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000230: 3320 3a3a 204f 6e6c 790d 0a09 5072 6f67  3 :: Only...Prog
+00000240: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000250: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000260: 390d 0a09 5072 6f67 7261 6d6d 696e 6720  9...Programming 
+00000270: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000280: 6f6e 203a 3a20 332e 3130 0d0a 090d 0a09  on :: 3.10......
+00000290: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+000002a0: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
+000002b0: 6963 656e 7365 0d0a 094f 7065 7261 7469  icense...Operati
+000002c0: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
+000002d0: 496e 6465 7065 6e64 656e 740d 0a0d 0a5b  Independent....[
+000002e0: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
+000002f0: 655f 6469 7220 3d20 0d0a 093d 2073 7263  e_dir = ...= src
+00000300: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
+00000310: 643a 0d0a 7079 7468 6f6e 5f72 6571 7569  d:..python_requi
+00000320: 7265 7320 3d20 3e3d 332e 390d 0a69 6e73  res = >=3.9..ins
+00000330: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
+00000340: 0d0a 0977 6865 656c 0d0a 0972 6571 7565  ...wheel...reque
+00000350: 7374 733d 3d32 2e2a 0d0a 0d0a 5b6f 7074  sts==2.*....[opt
+00000360: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
+00000370: 6e64 5d0d 0a77 6865 7265 203d 2073 7263  nd]..where = src
+00000380: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 7874  ....[options.ext
+00000390: 7261 735f 7265 7175 6972 655d 0d0a 7465  ras_require]..te
+000003a0: 7374 696e 6720 3d20 0d0a 0970 7974 6573  sting = ...pytes
+000003b0: 743e 3d36 2e30 0d0a 0970 7974 6573 742d  t>=6.0...pytest-
+000003c0: 636f 763e 3d32 2e30 0d0a 096d 7970 793e  cov>=2.0...mypy>
+000003d0: 3d30 2e39 3130 0d0a 0966 6c61 6b65 383e  =0.910...flake8>
+000003e0: 3d33 2e39 0d0a 0974 6f78 3e3d 332e 3234  =3.9...tox>=3.24
+000003f0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
+00000400: 6b61 6765 5f64 6174 615d 0d0a 6e69 7472  kage_data]..nitr
+00000410: 6164 6f20 3d20 7079 2e74 7970 6564 0d0a  ado = py.typed..
+00000420: 0d0a 5b66 6c61 6b65 385d 0d0a 6d61 782d  ..[flake8]..max-
+00000430: 6c69 6e65 2d6c 656e 6774 6820 3d20 3136  line-length = 16
+00000440: 300d 0a0d 0a5b 6567 675f 696e 666f 5d0d  0....[egg_info].
+00000450: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
+00000460: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
```

### Comparing `nitrado-0.0.9/src/nitrado.egg-info/PKG-INFO` & `nitrado-1.0.1/src/nitrado.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 Metadata-Version: 2.1
 Name: nitrado
-Version: 0.0.9
+Version: 1.0.1
 Summary: This application accesses the Nitrado API.
 Home-page: https://github.com/mjlomeli/NitradoAPI
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/NitradoAPI/issues
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # Python Nitrado SDK
-[![Testing](https://github.com/mjlomeli/NitradoAPI/actions/workflows/tests.yml/badge.svg)](#)
+
+[![Testing](https://github.com/mjlomeli/NitradoAPI/actions/workflows/tests.yml/badge.svg)](#) tests need a Nitrado subscription account 
 
 
 A Python based SDK for the [Nitrado RESTful API](https://doc.nitrado.net/) published at [PyPI](https://pypi.org/project/nitrado/).
 
 
 # Overview
```

