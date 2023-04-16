# Comparing `tmp/nif-dumper-1.0.1.tar.gz` & `tmp/nif-dumper-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nif-dumper-1.0.1.tar", last modified: Thu Jul 21 12:09:25 2022, max compression
+gzip compressed data, was "nif-dumper-1.0.2.tar", last modified: Sun Apr 16 21:01:50 2023, max compression
```

## Comparing `nif-dumper-1.0.1.tar` & `nif-dumper-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-07-21 12:09:25.726317 nif-dumper-1.0.1/
--rw-rw-rw-   0        0        0    35817 2022-07-21 11:25:37.000000 nif-dumper-1.0.1/LICENSE.md
--rw-rw-rw-   0        0        0     2508 2022-07-21 12:09:25.727319 nif-dumper-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1574 2022-07-21 11:25:37.000000 nif-dumper-1.0.1/README.md
--rw-rw-rw-   0        0        0       86 2022-07-21 11:25:37.000000 nif-dumper-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1251 2022-07-21 12:09:25.740318 nif-dumper-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-07-21 12:09:25.637789 nif-dumper-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2022-07-21 12:09:25.658794 nif-dumper-1.0.1/src/nif_dumper/
--rw-rw-rw-   0        0        0        0 2022-07-21 11:25:37.000000 nif-dumper-1.0.1/src/nif_dumper/__init__.py
--rw-rw-rw-   0        0        0     7247 2022-07-21 12:03:08.000000 nif-dumper-1.0.1/src/nif_dumper/dumper.py
-drwxrwxrwx   0        0        0        0 2022-07-21 12:09:25.723320 nif-dumper-1.0.1/src/nif_dumper.egg-info/
--rw-rw-rw-   0        0        0     2508 2022-07-21 12:09:25.000000 nif-dumper-1.0.1/src/nif_dumper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2022-07-21 12:09:25.000000 nif-dumper-1.0.1/src/nif_dumper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-21 12:09:25.000000 nif-dumper-1.0.1/src/nif_dumper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2022-07-21 12:09:25.000000 nif-dumper-1.0.1/src/nif_dumper.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       91 2022-07-21 12:09:25.000000 nif-dumper-1.0.1/src/nif_dumper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-07-21 12:09:25.000000 nif-dumper-1.0.1/src/nif_dumper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:01:50.650758 nif-dumper-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-16 21:01:50.650758 nif-dumper-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-16 21:01:39.000000 nif-dumper-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-16 21:01:39.000000 nif-dumper-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-16 21:01:50.650758 nif-dumper-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:01:50.646758 nif-dumper-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:01:50.650758 nif-dumper-1.0.2/src/nif_dumper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:01:39.000000 nif-dumper-1.0.2/src/nif_dumper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-04-16 21:01:39.000000 nif-dumper-1.0.2/src/nif_dumper/dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:01:50.650758 nif-dumper-1.0.2/src/nif_dumper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-16 21:01:50.000000 nif-dumper-1.0.2/src/nif_dumper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-16 21:01:50.000000 nif-dumper-1.0.2/src/nif_dumper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 21:01:50.000000 nif-dumper-1.0.2/src/nif_dumper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-16 21:01:50.000000 nif-dumper-1.0.2/src/nif_dumper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-16 21:01:50.000000 nif-dumper-1.0.2/src/nif_dumper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-16 21:01:50.000000 nif-dumper-1.0.2/src/nif_dumper.egg-info/top_level.txt
```

### Comparing `nif-dumper-1.0.1/README.md` & `nif-dumper-1.0.2/README.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-# NIF Dumper
-
-<p align="center"><img src="https://raw.githubusercontent.com/LightDestory/NIF-Dumper/master/.github/assets/preview.gif" alt="Preview" width=600px/></p>
-
-A simple Python CLI tool to search and download NIF (Naruto Italian Forum) releases.
-
-_This utility aims to make easier the download of a whole series due to missing pack downloads_
-
-If you like NIF releases, support the team!
-
-__This project is in no way affiliated with, supported or offered by NIF Team__
-
-
-## Install and Usage
-
-__Make sure to have Python 3.7+ and aria2 installed on your system.__
-
-You can install this tool as a Python Module using pip
-or using the script directly. The dumper provide a wizard that will help you download the releases.
-
-- If you want to install the tool as a Python Module:
-   - Install the module using pip: `pip install nif-dumper`
-   - You can run the tool using: `nif-dumper`
-- If you want to use the script directly:
-  - Clone the repository anywhere on your pc:
-  
-     `git clone https://github.com/LightDestory/NIF-Dumper`
-
-  - Install the requirements using pip:
-
-     `pip install .`
-
-  - Run the dumper:
-
-     `python ./src/nif_dumper/dumper.py`
-
-## Support
-
-<p align="center">
-    <a href="https://coindrop.to/lightdestory" target="__blank"><img alt="Coindrop" title="Support me with a donation!"
-            src="https://img.shields.io/badge/-Support me with coindrop.to-yellowgreen?style=for-the-badge&logo=paypal&logoColor=white" /></a>
-</p>
-
-## ⚠️ License
-
+# NIF Dumper
+
+<p align="center"><img src="https://raw.githubusercontent.com/LightDestory/NIF-Dumper/master/.github/assets/preview.gif" alt="Preview" width=600px/></p>
+
+A simple Python CLI tool to search and download NIF (Naruto Italian Forum) releases.
+
+_This utility aims to make easier the download of a whole series due to missing pack downloads_
+
+If you like NIF releases, support the team!
+
+__This project is in no way affiliated with, supported or offered by NIF Team__
+
+
+## Install and Usage
+
+__Make sure to have Python 3.7+ and aria2 installed on your system.__
+
+You can install this tool as a Python Module using pip
+or using the script directly. The dumper provide a wizard that will help you download the releases.
+
+- If you want to install the tool as a Python Module:
+   - Install the module using pip: `pip install nif-dumper`
+   - You can run the tool using: `nif-dumper`
+- If you want to use the script directly:
+  - Clone the repository anywhere on your pc:
+  
+     `git clone https://github.com/LightDestory/NIF-Dumper`
+
+  - Install the requirements using pip:
+
+     `pip install .`
+
+  - Run the dumper:
+
+     `python ./src/nif_dumper/dumper.py`
+
+## Support
+
+<p align="center">
+    <a href="https://coindrop.to/lightdestory" target="__blank"><img alt="Coindrop" title="Support me with a donation!"
+            src="https://img.shields.io/badge/-Support me with coindrop.to-yellowgreen?style=for-the-badge&logo=paypal&logoColor=white" /></a>
+</p>
+
+## ⚠️ License
+
 This collection is under GNU GPL-3.0 License.
```

### Comparing `nif-dumper-1.0.1/setup.cfg` & `nif-dumper-1.0.2/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,79 +1,76 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 206e 6966 2d64 756d 7065 720d 0a76   = nif-dumper..v
-00000020: 6572 7369 6f6e 203d 2061 7474 723a 206e  ersion = attr: n
-00000030: 6966 5f64 756d 7065 722e 6475 6d70 6572  if_dumper.dumper
-00000040: 2e56 4552 5349 4f4e 0d0a 6175 7468 6f72  .VERSION..author
-00000050: 203d 204c 6967 6874 4465 7374 6f72 790d   = LightDestory.
-00000060: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
-00000070: 6170 6232 3331 4067 6d61 696c 2e63 6f6d  apb231@gmail.com
-00000080: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
-00000090: 4120 7369 6d70 6c65 2050 7974 686f 6e20  A simple Python 
-000000a0: 434c 4920 746f 6f6c 2074 6f20 7365 6172  CLI tool to sear
-000000b0: 6368 2061 6e64 2064 6f77 6e6c 6f61 6420  ch and download 
-000000c0: 4e49 4620 284e 6172 7574 6f20 4974 616c  NIF (Naruto Ital
-000000d0: 6961 6e20 466f 7275 6d29 2072 656c 6561  ian Forum) relea
-000000e0: 7365 730d 0a6c 6f6e 675f 6465 7363 7269  ses..long_descri
-000000f0: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
-00000100: 4144 4d45 2e6d 640d 0a6c 6f6e 675f 6465  ADME.md..long_de
-00000110: 7363 7269 7074 696f 6e5f 636f 6e74 656e  scription_conten
-00000120: 745f 7479 7065 203d 2074 6578 742f 6d61  t_type = text/ma
-00000130: 726b 646f 776e 0d0a 6c69 6365 6e73 655f  rkdown..license_
-00000140: 6669 6c65 7320 3d20 4c49 4345 4e53 452e  files = LICENSE.
-00000150: 6d64 0d0a 7572 6c20 3d20 6874 7470 733a  md..url = https:
-00000160: 2f2f 6769 7468 7562 2e63 6f6d 2f4c 6967  //github.com/Lig
-00000170: 6874 4465 7374 6f72 792f 4e49 462d 4475  htDestory/NIF-Du
-00000180: 6d70 6572 0d0a 7072 6f6a 6563 745f 7572  mper..project_ur
-00000190: 6c73 203d 200d 0a09 4275 6720 5472 6163  ls = ...Bug Trac
-000001a0: 6b65 7220 3d20 6874 7470 733a 2f2f 6769  ker = https://gi
-000001b0: 7468 7562 2e63 6f6d 2f4c 6967 6874 4465  thub.com/LightDe
-000001c0: 7374 6f72 792f 4e49 462d 4475 6d70 6572  story/NIF-Dumper
-000001d0: 2f69 7373 7565 730d 0a63 6c61 7373 6966  /issues..classif
-000001e0: 6965 7273 203d 200d 0a09 4465 7665 6c6f  iers = ...Develo
-000001f0: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
-00000200: 3520 2d20 5072 6f64 7563 7469 6f6e 2f53  5 - Production/S
-00000210: 7461 626c 650d 0a09 456e 7669 726f 6e6d  table...Environm
-00000220: 656e 7420 3a3a 2043 6f6e 736f 6c65 0d0a  ent :: Console..
-00000230: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
-00000240: 4170 7072 6f76 6564 203a 3a20 474e 5520  Approved :: GNU 
-00000250: 4765 6e65 7261 6c20 5075 626c 6963 204c  General Public L
-00000260: 6963 656e 7365 2076 3320 2847 504c 7633  icense v3 (GPLv3
-00000270: 290d 0a09 4f70 6572 6174 696e 6720 5379  )...Operating Sy
-00000280: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
-00000290: 656e 6465 6e74 0d0a 0950 726f 6772 616d  endent...Program
-000002a0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000002b0: 2050 7974 686f 6e20 3a3a 2033 0d0a 0950   Python :: 3...P
-000002c0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000002d0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000002e0: 2033 2e37 0d0a 0950 726f 6772 616d 6d69   3.7...Programmi
-000002f0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000300: 7974 686f 6e20 3a3a 2033 2e38 0d0a 0950  ython :: 3.8...P
-00000310: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000320: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000330: 2033 2e39 0d0a 0950 726f 6772 616d 6d69   3.9...Programmi
-00000340: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000350: 7974 686f 6e20 3a3a 2033 2e31 300d 0a09  ython :: 3.10...
-00000360: 5479 7069 6e67 203a 3a20 5479 7065 640d  Typing :: Typed.
-00000370: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7061  ...[options]..pa
-00000380: 636b 6167 655f 6469 7220 3d20 0d0a 093d  ckage_dir = ...=
-00000390: 2073 7263 0d0a 7061 636b 6167 6573 203d   src..packages =
-000003a0: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
-000003b0: 6571 7569 7265 7320 3d20 3e3d 332e 370d  equires = >=3.7.
-000003c0: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
-000003d0: 7320 3d20 0d0a 0972 6571 7565 7374 737e  s = ...requests~
-000003e0: 3d32 2e32 372e 310d 0a09 696e 7175 6972  =2.27.1...inquir
-000003f0: 6572 7079 7e3d 302e 332e 330d 0a09 6265  erpy~=0.3.3...be
-00000400: 6175 7469 6675 6c73 6f75 7034 7e3d 342e  autifulsoup4~=4.
-00000410: 3130 2e30 0d0a 0963 6f6c 6f72 616d 617e  10.0...colorama~
-00000420: 3d30 2e34 2e34 0d0a 0974 6572 6d63 6f6c  =0.4.4...termcol
-00000430: 6f72 7e3d 312e 312e 300d 0a0d 0a5b 6f70  or~=1.1.0....[op
-00000440: 7469 6f6e 732e 656e 7472 795f 706f 696e  tions.entry_poin
-00000450: 7473 5d0d 0a63 6f6e 736f 6c65 5f73 6372  ts]..console_scr
-00000460: 6970 7473 203d 200d 0a09 6e69 662d 6475  ipts = ...nif-du
-00000470: 6d70 6572 203d 206e 6966 5f64 756d 7065  mper = nif_dumpe
-00000480: 722e 6475 6d70 6572 3a6d 6169 6e0d 0a0d  r.dumper:main...
-00000490: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-000004a0: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
-000004b0: 3d20 7372 630d 0a0d 0a5b 6567 675f 696e  = src....[egg_in
-000004c0: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-000004d0: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-000004e0: 0a0d 0a                                  ...
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6e69 662d 6475 6d70 6572 0a76 6572  = nif-dumper.ver
+00000020: 7369 6f6e 203d 2061 7474 723a 206e 6966  sion = attr: nif
+00000030: 5f64 756d 7065 722e 6475 6d70 6572 2e56  _dumper.dumper.V
+00000040: 4552 5349 4f4e 0a61 7574 686f 7220 3d20  ERSION.author = 
+00000050: 4c69 6768 7444 6573 746f 7279 0a61 7574  LightDestory.aut
+00000060: 686f 725f 656d 6169 6c20 3d20 6170 6232  hor_email = apb2
+00000070: 3331 4067 6d61 696c 2e63 6f6d 0a64 6573  31@gmail.com.des
+00000080: 6372 6970 7469 6f6e 203d 2041 2073 696d  cription = A sim
+00000090: 706c 6520 5079 7468 6f6e 2043 4c49 2074  ple Python CLI t
+000000a0: 6f6f 6c20 746f 2073 6561 7263 6820 616e  ool to search an
+000000b0: 6420 646f 776e 6c6f 6164 204e 4946 2028  d download NIF (
+000000c0: 4e61 7275 746f 2049 7461 6c69 616e 2046  Naruto Italian F
+000000d0: 6f72 756d 2920 7265 6c65 6173 6573 0a6c  orum) releases.l
+000000e0: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
+000000f0: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
+00000100: 640a 6c6f 6e67 5f64 6573 6372 6970 7469  d.long_descripti
+00000110: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
+00000120: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0a  = text/markdown.
+00000130: 6c69 6365 6e73 655f 6669 6c65 7320 3d20  license_files = 
+00000140: 4c49 4345 4e53 450a 7572 6c20 3d20 6874  LICENSE.url = ht
+00000150: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000160: 2f4c 6967 6874 4465 7374 6f72 792f 4e49  /LightDestory/NI
+00000170: 462d 4475 6d70 6572 0a70 726f 6a65 6374  F-Dumper.project
+00000180: 5f75 726c 7320 3d20 0a09 4275 6720 5472  _urls = ..Bug Tr
+00000190: 6163 6b65 7220 3d20 6874 7470 733a 2f2f  acker = https://
+000001a0: 6769 7468 7562 2e63 6f6d 2f4c 6967 6874  github.com/Light
+000001b0: 4465 7374 6f72 792f 4e49 462d 4475 6d70  Destory/NIF-Dump
+000001c0: 6572 2f69 7373 7565 730a 636c 6173 7369  er/issues.classi
+000001d0: 6669 6572 7320 3d20 0a09 4465 7665 6c6f  fiers = ..Develo
+000001e0: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
+000001f0: 3520 2d20 5072 6f64 7563 7469 6f6e 2f53  5 - Production/S
+00000200: 7461 626c 650a 0945 6e76 6972 6f6e 6d65  table..Environme
+00000210: 6e74 203a 3a20 436f 6e73 6f6c 650a 094c  nt :: Console..L
+00000220: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+00000230: 7072 6f76 6564 203a 3a20 474e 5520 4765  proved :: GNU Ge
+00000240: 6e65 7261 6c20 5075 626c 6963 204c 6963  neral Public Lic
+00000250: 656e 7365 2076 3320 2847 504c 7633 290a  ense v3 (GPLv3).
+00000260: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
+00000270: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+00000280: 656e 740a 0950 726f 6772 616d 6d69 6e67  ent..Programming
+00000290: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000002a0: 686f 6e20 3a3a 2033 0a09 5072 6f67 7261  hon :: 3..Progra
+000002b0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000002c0: 3a20 5079 7468 6f6e 203a 3a20 332e 370a  : Python :: 3.7.
+000002d0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+000002e0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000002f0: 3a3a 2033 2e38 0a09 5072 6f67 7261 6d6d  :: 3.8..Programm
+00000300: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000310: 5079 7468 6f6e 203a 3a20 332e 390a 0950  Python :: 3.9..P
+00000320: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000330: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000340: 2033 2e31 300a 0954 7970 696e 6720 3a3a   3.10..Typing ::
+00000350: 2054 7970 6564 0a0a 5b6f 7074 696f 6e73   Typed..[options
+00000360: 5d0a 7061 636b 6167 655f 6469 7220 3d20  ].package_dir = 
+00000370: 0a09 3d20 7372 630a 7061 636b 6167 6573  ..= src.packages
+00000380: 203d 2066 696e 643a 0a70 7974 686f 6e5f   = find:.python_
+00000390: 7265 7175 6972 6573 203d 203e 3d33 2e37  requires = >=3.7
+000003a0: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
+000003b0: 7320 3d20 0a09 7265 7175 6573 7473 7e3d  s = ..requests~=
+000003c0: 322e 3238 2e32 0a09 696e 7175 6972 6572  2.28.2..inquirer
+000003d0: 7079 7e3d 302e 332e 340a 0962 6561 7574  py~=0.3.4..beaut
+000003e0: 6966 756c 736f 7570 347e 3d34 2e31 322e  ifulsoup4~=4.12.
+000003f0: 320a 0963 6f6c 6f72 616d 617e 3d30 2e34  2..colorama~=0.4
+00000400: 2e36 0a09 7465 726d 636f 6c6f 727e 3d32  .6..termcolor~=2
+00000410: 2e32 2e30 0a0a 5b6f 7074 696f 6e73 2e65  .2.0..[options.e
+00000420: 6e74 7279 5f70 6f69 6e74 735d 0a63 6f6e  ntry_points].con
+00000430: 736f 6c65 5f73 6372 6970 7473 203d 200a  sole_scripts = .
+00000440: 096e 6966 2d64 756d 7065 7220 3d20 6e69  .nif-dumper = ni
+00000450: 665f 6475 6d70 6572 2e64 756d 7065 723a  f_dumper.dumper:
+00000460: 6d61 696e 0a0a 5b6f 7074 696f 6e73 2e70  main..[options.p
+00000470: 6163 6b61 6765 732e 6669 6e64 5d0a 7768  ackages.find].wh
+00000480: 6572 6520 3d20 7372 630a 0a5b 6567 675f  ere = src..[egg_
+00000490: 696e 666f 5d0a 7461 675f 6275 696c 6420  info].tag_build 
+000004a0: 3d20 0a74 6167 5f64 6174 6520 3d20 300a  = .tag_date = 0.
+000004b0: 0a                                       .
```

### Comparing `nif-dumper-1.0.1/src/nif_dumper/dumper.py` & `nif-dumper-1.0.2/src/nif_dumper/dumper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,172 +1,172 @@
-import os
-import re
-import shutil
-from typing import Union
-
-import requests
-from InquirerPy import inquirer
-from InquirerPy.base import Choice
-from InquirerPy.validator import EmptyInputValidator
-from bs4 import BeautifulSoup
-from colorama import init
-from requests import Response
-from termcolor import colored
-
-VERSION = "1.0.1"
-NIF_SCRAPE_TEMPLATE: str = "https://nifteam.info/Multimedia/?Anime=%key%"
-NIF_DL_TEMPLATE: str = "https://download.nifteam.info/Download/Anime/%episode%"
-NIF_HOME_KEY: str = "Homepage"
-SERIES_REGEX: str = r"//nifteam.info/Multimedia/\?Anime=.+"
-SERIES_EPISODES_REGEX: str = r"//nifteam.info/link.php\?file=.+"
-
-
-def make_soup(url: str) -> BeautifulSoup:
-    page_src: Response = requests.get(url)
-    if page_src.status_code != 200:
-        print(colored("NIF website is not reachable at the moment!", "red"))
-        exit(-1)
-    return BeautifulSoup(page_src.text, "html.parser")
-
-
-def a_to_dict(soup: BeautifulSoup, regex: str) -> dict[str, str]:
-    collection: dict[str, str] = {}
-    div = soup.find("div", attrs={'class': "nifteam0"})
-    for a_element in div.find_all("a", attrs={'href': re.compile(regex)}):
-        name: str = a_element.contents[0]
-        anime_path: str = a_element['href'].split("=")[1]
-        collection[name] = anime_path
-    return collection
-
-
-def get_series(soup: BeautifulSoup) -> [dict[str, str]]:
-    in_progress: dict[str, str] = {}
-    in_progress_div = soup.find("div", attrs={'id': "titoloepisodio"}).find_next('div')
-    for a_element in in_progress_div.find_all("a", attrs={'href': re.compile(SERIES_REGEX)}):
-        name: str = a_element.find("img")['alt']
-        anime_path: str = a_element['href'].split("=")[1]
-        in_progress[name] = anime_path
-    return [in_progress, a_to_dict(soup, SERIES_REGEX)]
-
-
-def get_series_episodes(soup: BeautifulSoup) -> dict[str, str]:
-    return a_to_dict(soup, SERIES_EPISODES_REGEX)
-
-
-def ask_selection(title: str, choices: [Choice]) -> int:
-    return inquirer.select(
-        message=title,
-        choices=choices,
-        default=0).execute()
-
-
-def ask_fuzzy(title: str, data: [str], episode_listing: bool = False) -> str:
-    choices: [Union[str, list['Choice']]] = [
-        Choice(value="dumper_goback", name="Go Back to Selection"),
-        Choice(value="dumper_exit", name="Exit")
-    ]
-    if episode_listing:
-        choices.append(Choice(value="dumper_download_all", name="Download All (Offset can be set)"))
-    choices = choices + data
-    return inquirer.fuzzy(
-        message=title,
-        choices=choices
-    ).execute()
-
-
-def ask_integer_parameter(title: str, min_value: int, max_value: int, default: int = 1) -> int:
-    return inquirer.number(
-        message=title,
-        min_allowed=min_value,
-        max_allowed=max_value,
-        validate=EmptyInputValidator(),
-        default=default
-    ).execute()
-
-
-def download(anime: str, download_action: str, episodes: dict[str, str]) -> None:
-    parallel_downloads: int = 1
-    current_path: str = "./"
-    subdir_needed: bool = True if os.path.isdir(anime) else inquirer.confirm(message=f'Create "{anime}" subfolder?',
-                                                                             default=False).execute()
-    if subdir_needed:
-        try:
-            os.makedirs(f'{current_path}{anime}', exist_ok=True)
-            current_path = f'{current_path}{anime}'
-        except OSError:
-            print(colored("Unable to create subfolder!", "red"))
-    if download_action != "dumper_download_all":
-        url: str = f'\"{NIF_DL_TEMPLATE.replace("%episode%", episodes[download_action])}\"'
-    else:
-        offset: int = 1
-        limit: int = len(episodes.values())
-        offset_needed: bool = inquirer.confirm(message="Do you want to set a offset?", default=False).execute()
-        if offset_needed:
-            offset = ask_integer_parameter("What episode should I start with?:", 1, limit)
-        more_parallel: bool = inquirer.confirm(message="Do you want to download more than 1 episode at once?",
-                                               default=False).execute()
-        if more_parallel:
-            parallel_downloads = ask_integer_parameter("How many parallel downloads do you want? (max 5):", 1, 5)
-        ep_list: [str] = list(episodes.keys())
-        url = ""
-        for i in range(int(offset) - 1, limit):
-            url: str = f'{url}\"{NIF_DL_TEMPLATE.replace("%episode%", episodes[ep_list[i]])}\" '
-    print(colored("\nRunning aria2, to interrupt download press CTRL+C...", "yellow"))
-    os.system(f'aria2c -d {current_path} -j {parallel_downloads} --download-result=hide --summary-interval=0 -x 15 -s '
-              f'15 -Z {url}')
-
-
-def runtime(series_list: [dict[str, str]]):
-    try:
-        while True:
-            os.system('cls' if os.name == 'nt' else 'clear')
-            series_type = ask_selection("Select anime's category:", [
-                Choice(value=0, name="Fansub WIP"),
-                Choice(value=1, name="Fansub Completed"),
-                Choice(value=-1, name="Exit")
-            ])
-            if series_type == -1:
-                break
-            selected_series: str = ask_fuzzy("Select an Anime:", list(series_list[series_type].keys()))
-            if selected_series == "dumper_exit":
-                break
-            elif selected_series == "dumper_goback":
-                continue
-            else:
-                print(colored("Fetching episodes...", "yellow"))
-                anime_path: str = series_list[series_type][selected_series]
-                episode_soup: BeautifulSoup = make_soup(NIF_SCRAPE_TEMPLATE.replace("%key%", anime_path))
-                print(colored("Fetch completed", "green"))
-                episodes: dict[str, str] = get_series_episodes(episode_soup)
-                download_action: str = ask_fuzzy("Select download item:", list(episodes.keys()), episode_listing=True)
-                if download_action == "dumper_exit":
-                    break
-                elif download_action == "dumper_goback":
-                    continue
-                download(anime_path, download_action, episodes)
-                print(colored("Download completed", "green"))
-                exit_confirm = ask_selection("Do you want to dump another anime?:", [
-                    Choice(value=0, name="Yes"),
-                    Choice(value=1, name="No")
-                ])
-                if exit_confirm:
-                    break
-    except KeyboardInterrupt:
-        print(colored("\nRuntime aborted by KeyboardInterrupt", "red"))
-        exit(-1)
-
-
-def main() -> None:
-    # colorama init
-    init()
-    if not shutil.which("aria2c"):
-        print(colored("aria2 is required to run the dumper!\nInstall it and put it in the PATH!", "red"))
-        exit(-1)
-    print(colored("Fetching NIF releases...", "yellow"))
-    soup: BeautifulSoup = make_soup(NIF_SCRAPE_TEMPLATE.replace("%key%", NIF_HOME_KEY))
-    print(colored("Fetch completed!", "green"))
-    runtime(get_series(soup))
-    print(colored("Thanks you, goodbye!", "cyan"))
-
-
-if __name__ == '__main__':
-    main()
+import os
+import re
+import shutil
+from typing import Union
+
+import requests
+from InquirerPy import inquirer
+from InquirerPy.base import Choice
+from InquirerPy.validator import EmptyInputValidator
+from bs4 import BeautifulSoup
+from colorama import init
+from requests import Response
+from termcolor import colored
+
+VERSION = "1.0.2"
+NIF_SCRAPE_TEMPLATE: str = "https://nifteam.info/Multimedia/?Anime=%key%"
+NIF_DL_TEMPLATE: str = "https://download.nifteam.info/Download/Anime/%episode%"
+NIF_HOME_KEY: str = "Homepage"
+SERIES_REGEX: str = r"//nifteam.info/Multimedia/\?Anime=.+"
+SERIES_EPISODES_REGEX: str = r"//nifteam.info/link.php\?file=.+"
+
+
+def make_soup(url: str) -> BeautifulSoup:
+    page_src: Response = requests.get(url)
+    if page_src.status_code != 200:
+        print(colored("NIF website is not reachable at the moment!", "red"))
+        exit(-1)
+    return BeautifulSoup(page_src.text, "html.parser")
+
+
+def a_to_dict(soup: BeautifulSoup, regex: str) -> dict[str, str]:
+    collection: dict[str, str] = {}
+    div = soup.find("div", attrs={'class': "nifteam0"})
+    for a_element in div.find_all("a", attrs={'href': re.compile(regex)}):
+        name: str = a_element.contents[0]
+        anime_path: str = a_element['href'].split("=")[1]
+        collection[name] = anime_path
+    return collection
+
+
+def get_series(soup: BeautifulSoup) -> [dict[str, str]]:
+    in_progress: dict[str, str] = {}
+    in_progress_div = soup.find("div", attrs={'id': "titoloepisodio"}).find_next('div')
+    for a_element in in_progress_div.find_all("a", attrs={'href': re.compile(SERIES_REGEX)}):
+        name: str = a_element.find("img")['alt']
+        anime_path: str = a_element['href'].split("=")[1]
+        in_progress[name] = anime_path
+    return [in_progress, a_to_dict(soup, SERIES_REGEX)]
+
+
+def get_series_episodes(soup: BeautifulSoup) -> dict[str, str]:
+    return a_to_dict(soup, SERIES_EPISODES_REGEX)
+
+
+def ask_selection(title: str, choices: [Choice]) -> int:
+    return inquirer.select(
+        message=title,
+        choices=choices,
+        default=0).execute()
+
+
+def ask_fuzzy(title: str, data: [str], episode_listing: bool = False) -> str:
+    choices: [Union[str, list['Choice']]] = [
+        Choice(value="dumper_goback", name="Go Back to Selection"),
+        Choice(value="dumper_exit", name="Exit")
+    ]
+    if episode_listing:
+        choices.append(Choice(value="dumper_download_all", name="Download All (Offset can be set)"))
+    choices = choices + data
+    return inquirer.fuzzy(
+        message=title,
+        choices=choices
+    ).execute()
+
+
+def ask_integer_parameter(title: str, min_value: int, max_value: int, default: int = 1) -> int:
+    return inquirer.number(
+        message=title,
+        min_allowed=min_value,
+        max_allowed=max_value,
+        validate=EmptyInputValidator(),
+        default=default
+    ).execute()
+
+
+def download(anime: str, download_action: str, episodes: dict[str, str]) -> None:
+    parallel_downloads: int = 1
+    current_path: str = "./"
+    subdir_needed: bool = True if os.path.isdir(anime) else inquirer.confirm(message=f'Create "{anime}" subfolder?',
+                                                                             default=False).execute()
+    if subdir_needed:
+        try:
+            os.makedirs(f'{current_path}{anime}', exist_ok=True)
+            current_path = f'{current_path}{anime}'
+        except OSError:
+            print(colored("Unable to create subfolder!", "red"))
+    if download_action != "dumper_download_all":
+        url: str = f'\"{NIF_DL_TEMPLATE.replace("%episode%", episodes[download_action])}\"'
+    else:
+        offset: int = 1
+        limit: int = len(episodes.values())
+        offset_needed: bool = inquirer.confirm(message="Do you want to set a offset?", default=False).execute()
+        if offset_needed:
+            offset = ask_integer_parameter("What episode should I start with?:", 1, limit)
+        more_parallel: bool = inquirer.confirm(message="Do you want to download more than 1 episode at once?",
+                                               default=False).execute()
+        if more_parallel:
+            parallel_downloads = ask_integer_parameter("How many parallel downloads do you want? (max 5):", 1, 5)
+        ep_list: [str] = list(episodes.keys())
+        url = ""
+        for i in range(int(offset) - 1, limit):
+            url: str = f'{url}\"{NIF_DL_TEMPLATE.replace("%episode%", episodes[ep_list[i]])}\" '
+    print(colored("\nRunning aria2, to interrupt download press CTRL+C...", "yellow"))
+    os.system(f'aria2c -d {current_path} -j {parallel_downloads} --download-result=hide --summary-interval=0 -x 15 -s '
+              f'15 -Z {url}')
+
+
+def runtime(series_list: [dict[str, str]]):
+    try:
+        while True:
+            os.system('cls' if os.name == 'nt' else 'clear')
+            series_type = ask_selection("Select anime's category:", [
+                Choice(value=0, name="Fansub WIP"),
+                Choice(value=1, name="Fansub Completed"),
+                Choice(value=-1, name="Exit")
+            ])
+            if series_type == -1:
+                break
+            selected_series: str = ask_fuzzy("Select an Anime:", list(series_list[series_type].keys()))
+            if selected_series == "dumper_exit":
+                break
+            elif selected_series == "dumper_goback":
+                continue
+            else:
+                print(colored("Fetching episodes...", "yellow"))
+                anime_path: str = series_list[series_type][selected_series]
+                episode_soup: BeautifulSoup = make_soup(NIF_SCRAPE_TEMPLATE.replace("%key%", anime_path))
+                print(colored("Fetch completed", "green"))
+                episodes: dict[str, str] = get_series_episodes(episode_soup)
+                download_action: str = ask_fuzzy("Select download item:", list(episodes.keys()), episode_listing=True)
+                if download_action == "dumper_exit":
+                    break
+                elif download_action == "dumper_goback":
+                    continue
+                download(anime_path, download_action, episodes)
+                print(colored("Download completed", "green"))
+                exit_confirm = ask_selection("Do you want to dump another anime?:", [
+                    Choice(value=0, name="Yes"),
+                    Choice(value=1, name="No")
+                ])
+                if exit_confirm:
+                    break
+    except KeyboardInterrupt:
+        print(colored("\nRuntime aborted by KeyboardInterrupt", "red"))
+        exit(-1)
+
+
+def main() -> None:
+    # colorama init
+    init()
+    if not shutil.which("aria2c"):
+        print(colored("aria2 is required to run the dumper!\nInstall it and put it in the PATH!", "red"))
+        exit(-1)
+    print(colored("Fetching NIF releases...", "yellow"))
+    soup: BeautifulSoup = make_soup(NIF_SCRAPE_TEMPLATE.replace("%key%", NIF_HOME_KEY))
+    print(colored("Fetch completed!", "green"))
+    runtime(get_series(soup))
+    print(colored("Thanks you, goodbye!", "cyan"))
+
+
+if __name__ == '__main__':
+    main()
```

