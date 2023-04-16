# Comparing `tmp/bitstring-4.0.1.tar.gz` & `tmp/bitstring-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitstring-4.0.1.tar", last modified: Wed Nov 16 14:22:00 2022, max compression
+gzip compressed data, was "bitstring-4.0.2.tar", last modified: Sun Apr 16 13:50:10 2023, max compression
```

## Comparing `bitstring-4.0.1.tar` & `bitstring-4.0.2.tar`

### file list

```diff
@@ -1,17 +1,26 @@
-drwxr-xr-x   0 scottg     (501) staff       (20)        0 2022-11-16 14:22:00.546977 bitstring-4.0.1/
--rw-r--r--   0 scottg     (501) staff       (20)     1106 2022-11-16 14:19:45.000000 bitstring-4.0.1/LICENSE
--rw-r--r--   0 scottg     (501) staff       (20)      121 2022-11-16 14:19:45.000000 bitstring-4.0.1/MANIFEST.in
--rw-r--r--   0 scottg     (501) staff       (20)     5368 2022-11-16 14:22:00.546430 bitstring-4.0.1/PKG-INFO
--rw-r--r--   0 scottg     (501) staff       (20)     4611 2022-11-16 14:21:36.000000 bitstring-4.0.1/README.md
-drwxr-xr-x   0 scottg     (501) staff       (20)        0 2022-11-16 14:22:00.541386 bitstring-4.0.1/bitstring.egg-info/
--rw-r--r--   0 scottg     (501) staff       (20)     5368 2022-11-16 14:22:00.000000 bitstring-4.0.1/bitstring.egg-info/PKG-INFO
--rw-r--r--   0 scottg     (501) staff       (20)      242 2022-11-16 14:22:00.000000 bitstring-4.0.1/bitstring.egg-info/SOURCES.txt
--rw-r--r--   0 scottg     (501) staff       (20)        1 2022-11-16 14:22:00.000000 bitstring-4.0.1/bitstring.egg-info/dependency_links.txt
--rw-r--r--   0 scottg     (501) staff       (20)       10 2022-11-16 14:22:00.000000 bitstring-4.0.1/bitstring.egg-info/top_level.txt
--rw-r--r--   0 scottg     (501) staff       (20)   200386 2022-11-16 14:21:36.000000 bitstring-4.0.1/bitstring.py
--rw-r--r--   0 scottg     (501) staff       (20)      735 2022-11-16 14:21:36.000000 bitstring-4.0.1/pyproject.toml
--rw-r--r--   0 scottg     (501) staff       (20)    58047 2022-11-16 14:21:36.000000 bitstring-4.0.1/release_notes.txt
--rw-r--r--   0 scottg     (501) staff       (20)       38 2022-11-16 14:22:00.547559 bitstring-4.0.1/setup.cfg
-drwxr-xr-x   0 scottg     (501) staff       (20)        0 2022-11-16 14:22:00.543511 bitstring-4.0.1/tests/
--rw-r--r--   0 scottg     (501) staff       (20)        8 2022-11-16 14:19:45.000000 bitstring-4.0.1/tests/smalltestfile
--rw-r--r--   0 scottg     (501) staff       (20)   125300 2022-11-16 14:19:45.000000 bitstring-4.0.1/tests/test.m1v
+drwxr-xr-x   0 scottg     (501) staff       (20)        0 2023-04-16 13:50:10.654277 bitstring-4.0.2/
+-rw-r--r--   0 scottg     (501) staff       (20)     1106 2021-07-17 21:23:45.000000 bitstring-4.0.2/LICENSE
+-rw-r--r--   0 scottg     (501) staff       (20)      174 2023-04-16 13:48:24.000000 bitstring-4.0.2/MANIFEST.in
+-rw-r--r--   0 scottg     (501) staff       (20)     6263 2023-04-16 13:50:10.653685 bitstring-4.0.2/PKG-INFO
+-rw-r--r--   0 scottg     (501) staff       (20)     5507 2023-04-16 13:48:24.000000 bitstring-4.0.2/README.md
+drwxr-xr-x   0 scottg     (501) staff       (20)        0 2023-04-16 13:50:10.640687 bitstring-4.0.2/bitstring/
+-rw-r--r--   0 scottg     (501) staff       (20)   200454 2023-04-16 13:48:24.000000 bitstring-4.0.2/bitstring/__init__.py
+-rw-r--r--   0 scottg     (501) staff       (20)        0 2023-04-16 13:48:24.000000 bitstring-4.0.2/bitstring/py.typed
+drwxr-xr-x   0 scottg     (501) staff       (20)        0 2023-04-16 13:50:10.643530 bitstring-4.0.2/bitstring.egg-info/
+-rw-r--r--   0 scottg     (501) staff       (20)     6263 2023-04-16 13:50:10.000000 bitstring-4.0.2/bitstring.egg-info/PKG-INFO
+-rw-r--r--   0 scottg     (501) staff       (20)      430 2023-04-16 13:50:10.000000 bitstring-4.0.2/bitstring.egg-info/SOURCES.txt
+-rw-r--r--   0 scottg     (501) staff       (20)        1 2023-04-16 13:50:10.000000 bitstring-4.0.2/bitstring.egg-info/dependency_links.txt
+-rw-r--r--   0 scottg     (501) staff       (20)       10 2023-04-16 13:50:10.000000 bitstring-4.0.2/bitstring.egg-info/top_level.txt
+-rw-r--r--   0 scottg     (501) staff       (20)      864 2023-04-16 13:48:24.000000 bitstring-4.0.2/pyproject.toml
+-rw-r--r--   0 scottg     (501) staff       (20)    58558 2023-04-16 13:48:24.000000 bitstring-4.0.2/release_notes.txt
+-rw-r--r--   0 scottg     (501) staff       (20)       38 2023-04-16 13:50:10.654487 bitstring-4.0.2/setup.cfg
+drwxr-xr-x   0 scottg     (501) staff       (20)        0 2023-04-16 13:50:10.652637 bitstring-4.0.2/tests/
+-rw-r--r--   0 scottg     (501) staff       (20)        0 2023-04-14 20:44:35.000000 bitstring-4.0.2/tests/__init__.py
+-rw-r--r--   0 scottg     (501) staff       (20)        8 2022-11-13 10:43:27.000000 bitstring-4.0.2/tests/smalltestfile
+-rw-r--r--   0 scottg     (501) staff       (20)   125300 2022-11-13 10:43:27.000000 bitstring-4.0.2/tests/test.m1v
+-rw-r--r--   0 scottg     (501) staff       (20)    24765 2023-04-16 13:48:24.000000 bitstring-4.0.2/tests/test_bitarray.py
+-rw-r--r--   0 scottg     (501) staff       (20)    26826 2023-04-16 13:48:24.000000 bitstring-4.0.2/tests/test_bits.py
+-rw-r--r--   0 scottg     (501) staff       (20)     1115 2022-11-13 10:43:27.000000 bitstring-4.0.2/tests/test_bitstore.py
+-rw-r--r--   0 scottg     (501) staff       (20)   144643 2023-04-16 13:48:24.000000 bitstring-4.0.2/tests/test_bitstream.py
+-rw-r--r--   0 scottg     (501) staff       (20)     4501 2023-04-16 13:48:24.000000 bitstring-4.0.2/tests/test_bitstring.py
+-rw-r--r--   0 scottg     (501) staff       (20)     6806 2023-04-16 13:48:24.000000 bitstring-4.0.2/tests/test_constbitstream.py
```

### Comparing `bitstring-4.0.1/LICENSE` & `bitstring-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bitstring-4.0.1/PKG-INFO` & `bitstring-4.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,121 +1,73 @@
-Metadata-Version: 2.1
-Name: bitstring
-Version: 4.0.1
-Summary: Simple construction, analysis and modification of binary data.
-Author-email: Scott Griffiths <dr.scottgriffiths@gmail.com>
-Project-URL: homepage, https://github.com/scott-griffiths/bitstring
-Project-URL: documentation, https://bitstring.readthedocs.io/
-Keywords: binary,bitarray,bitvector
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
 
 
-
-![bitstring](https://github.com/scott-griffiths/bitstring/blob/d85c22504882d93b8c0cec373ef03b375e9ea7f8/doc/bitstring_logo_small.png?raw=true "bitstring")
+![bitstring](https://raw.githubusercontent.com/scott-griffiths/bitstring/main/doc/bitstring_logo_small.png "bitstring")
 
 **bitstring** is a pure Python module designed to help make
 the creation and analysis of binary data as simple and natural as possible.
 
-It has been maintained since 2006 and now has about [20 million downloads](https://pypistats.org/packages/bitstring) per year.
-
-> **Note** \
-> \
-> Version 4.0 of bitstring only supports Python 3.7 and later. \
-> Use bitstring version 3.1 if you're using Python 2.7 or 3.6 or earlier.
-
-New in version 4.0
-------------------
-
-* New Python 3.7 minimum requirement. The code has been updated with type hints and legacy code removed.
-* Shorter and more versative properties are available.
-
-      >>> a = BitArray('u8=20')
-      >>> a += '0b0011, f16=5.52'
-      >>> a[12:].f16
-      5.51953125
-
-* A useful new pretty printing method. Gives a formatted view of a singe or two interpretations of the
-  binary data.
-
-      >>> a = Bits(bytes=b'hello world!!')
-      >>> a.pp('bin, hex', width=40)
-        0: 01101000 01100101   68 65
-       16: 01101100 01101100   6c 6c
-       32: 01101111 00100000   6f 20
-       48: 01110111 01101111   77 6f
-       64: 01110010 01101100   72 6c
-       80: 01100100 00100001   64 21
-       96: 00100001            21   
+It has been maintained since 2006 and now has about 20 million downloads per year.
 
-* LSB0 option (beta). This indexes the bits with the least significant bit being bit zero. This is the
-  opposite way to the standard Python containers but is usual in some relevant fields.
-      
-      >>> bitstring.lsb0 = True
-      >>> s = BitArray('0b00000')
-      >>> s[0] = 1
-      >>> s.bin
-      '00001'
 
-  This feature is still considered a beta as there may be issues with edge cases, especially around the
-  interaction with the 'stream' features of the `BitStream` and `ConstBitStream` classes. For most usage
-  cases it should be solid though, so please report any bugs in the issue tracker.
-      
-* Command line usage. Useful for quick interpretations of binary data.
+You can try out the interactive walkthrough notebook on [binder](https://mybinder.org/v2/gh/scott-griffiths/bitstring/main?labpath=doc%2Fwalkthrough.ipynb), or take a look at the [static version](https://github.com/scott-griffiths/bitstring/blob/main/doc/walkthrough.ipynb).
 
-        $ python -m bitstring int:16=-400
-        0xfe70
 
-* Support for 16 bit floating point types (both IEEE and bfloat).
+[![CI badge](https://github.com/scott-griffiths/bitstring/actions/workflows/.github/workflows/ci.yml/badge.svg)](https://github.com/scott-griffiths/bitstring/actions/workflows/ci.yml)
+[![Docs](https://img.shields.io/readthedocs/bitstring)](https://bitstring.readthedocs.io/en/latest/)
+[![Downloads](https://img.shields.io/pypi/dm/bitstring?color=blue)](https://pypistats.org/packages/bitstring) &nbsp; &nbsp; 
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/scott-griffiths/bitstring/main?labpath=doc%2Fwalkthrough.ipynb)
 
 
 Overview
 --------
 
 * Create bitstrings from hex, octal, binary, files, formatted strings, bytes, integers and floats of different endiannesses.
 * Powerful binary packing and unpacking functions.
 * Bit-level slicing, joining, searching, replacing and more.
 * Read from and interpret bitstrings as streams of binary data.
 * Rich API - chances are that whatever you want to do there's a simple and elegant way of doing it.
 * Open source software, released under the MIT licence.
 
 
+> **Note** \
+> Version 4.0 of bitstring only supports Python 3.7 and later. \
+> Use bitstring version 3.1 if you're using Python 2.7 or 3.6 or earlier.
+
+
 Documentation
 -------------
 The manual for the bitstring module is available at [Read the Docs](https://bitstring.readthedocs.org).
 It contains a walk-through of all the features and a complete [reference section](https://bitstring.readthedocs.io/en/stable/quick_ref.html).
 
 
-Simple Examples
----------------
+Examples
+--------
+
+### Installation
+
+    $ pip install bitstring
 
 ### [Creation](https://bitstring.readthedocs.io/en/stable/creation.html)
 
+     >>> from bitstring import Bits, BitArray, BitStream, pack
      >>> a = BitArray(bin='00101')
      >>> b = Bits(a_file_object)
      >>> c = BitArray('0xff, 0b101, 0o65, uint6=22')
      >>> d = pack('intle16, hex=a, 0b1', 100, a='0x34f')
      >>> e = pack('<16h', *range(16))
 
 ### [Different interpretations, slicing and concatenation](https://bitstring.readthedocs.io/en/stable/interpretation.html)
 
-     >>> a = BitArray('0x1af')
-     >>> a.hex, a.bin, a.uint
-     ('1af', '000110101111', 431)
+     >>> a = BitArray('0x3348')
+     >>> a.hex, a.bin, a.uint, a.float, a.bytes
+     ('3348', '0011001101001000', 13128, 0.2275390625, b'3H')
      >>> a[10:3:-1].bin
-     '1110101'
+     '0101100'
      >>> '0b100' + 3*a
-     BitArray('0x835e35e35, 0b111')
+     BitArray('0x866906690669, 0b000')
 
 ### [Reading data sequentially](https://bitstring.readthedocs.io/en/stable/reading.html)
 
      >>> b = BitStream('0x160120f')
      >>> b.read(12).hex
      '160'
      >>> b.pos = 0
@@ -129,14 +81,60 @@
      >>> c = BitArray('0b00010010010010001111')   # c.hex == '0x1248f'
      >>> c.find('0x48')
      (8,)
      >>> c.replace('0b001', '0xabc')
      >>> c.insert('0b0000', pos=3)
      >>> del c[12:16]
 
+
+New in version 4.0
+------------------
+
+* New Python 3.7 minimum requirement. The code has been updated with type hints and legacy code removed.
+* Shorter and more versative properties are available.
+
+      >>> a = BitArray('u8=20')
+      >>> a += '0b0011, f16=5.52'
+      >>> a[12:].f16
+      5.51953125
+
+* A useful new pretty printing method. Gives a formatted view of a singe or two interpretations of the
+  binary data.
+
+      >>> a = Bits(bytes=b'hello world!!')
+      >>> a.pp('bin, hex', width=40)
+        0: 01101000 01100101   68 65
+       16: 01101100 01101100   6c 6c
+       32: 01101111 00100000   6f 20
+       48: 01110111 01101111   77 6f
+       64: 01110010 01101100   72 6c
+       80: 01100100 00100001   64 21
+       96: 00100001            21   
+
+* LSB0 option (beta). This indexes the bits with the least significant bit being bit zero. This is the
+  opposite way to the standard Python containers but is usual in some relevant fields.
+      
+      >>> bitstring.lsb0 = True
+      >>> s = BitArray('0b00000')
+      >>> s[0] = 1
+      >>> s.bin
+      '00001'
+
+  This feature is still considered a beta as there may be issues with edge cases, especially around the
+  interaction with the 'stream' features of the `BitStream` and `ConstBitStream` classes. For most usage
+  cases it should be solid though, so please report any bugs in the issue tracker.
+      
+* Command line usage. Useful for quick interpretations of binary data.
+
+        $ python -m bitstring int:16=-400
+        0xfe70
+
+* Support for 16 bit floating point types (both IEEE and bfloat).
+
+
 Unit Tests
 ----------
 
 The 600+ unit tests should all pass. They can be run from the root of the project with
 
      python -m unittest
 
@@ -145,8 +143,8 @@
 -------
 
 Created by Scott Griffiths in 2006 to help with ad hoc parsing and creation of compressed video files.
 Maintained and expanded ever since as it became unexpectedly popular. Thanks to all those who have contributed ideas
 and code (and bug reports) over the years.
 
 
-<sub>Copyright (c) 2006 - 2022 Scott Griffiths</sub>
+<sub>Copyright (c) 2006 - 2023 Scott Griffiths</sub>
```

### Comparing `bitstring-4.0.1/README.md` & `bitstring-4.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,103 +1,91 @@
+Metadata-Version: 2.1
+Name: bitstring
+Version: 4.0.2
+Summary: Simple construction, analysis and modification of binary data.
+Author-email: Scott Griffiths <dr.scottgriffiths@gmail.com>
+Project-URL: homepage, https://github.com/scott-griffiths/bitstring
+Project-URL: documentation, https://bitstring.readthedocs.io/
+Keywords: binary,bitarray,bitvector
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
 
-![bitstring](https://github.com/scott-griffiths/bitstring/blob/d85c22504882d93b8c0cec373ef03b375e9ea7f8/doc/bitstring_logo_small.png?raw=true "bitstring")
+
+![bitstring](https://raw.githubusercontent.com/scott-griffiths/bitstring/main/doc/bitstring_logo_small.png "bitstring")
 
 **bitstring** is a pure Python module designed to help make
 the creation and analysis of binary data as simple and natural as possible.
 
-It has been maintained since 2006 and now has about [20 million downloads](https://pypistats.org/packages/bitstring) per year.
-
-> **Note** \
-> \
-> Version 4.0 of bitstring only supports Python 3.7 and later. \
-> Use bitstring version 3.1 if you're using Python 2.7 or 3.6 or earlier.
-
-New in version 4.0
-------------------
-
-* New Python 3.7 minimum requirement. The code has been updated with type hints and legacy code removed.
-* Shorter and more versative properties are available.
-
-      >>> a = BitArray('u8=20')
-      >>> a += '0b0011, f16=5.52'
-      >>> a[12:].f16
-      5.51953125
-
-* A useful new pretty printing method. Gives a formatted view of a singe or two interpretations of the
-  binary data.
-
-      >>> a = Bits(bytes=b'hello world!!')
-      >>> a.pp('bin, hex', width=40)
-        0: 01101000 01100101   68 65
-       16: 01101100 01101100   6c 6c
-       32: 01101111 00100000   6f 20
-       48: 01110111 01101111   77 6f
-       64: 01110010 01101100   72 6c
-       80: 01100100 00100001   64 21
-       96: 00100001            21   
+It has been maintained since 2006 and now has about 20 million downloads per year.
 
-* LSB0 option (beta). This indexes the bits with the least significant bit being bit zero. This is the
-  opposite way to the standard Python containers but is usual in some relevant fields.
-      
-      >>> bitstring.lsb0 = True
-      >>> s = BitArray('0b00000')
-      >>> s[0] = 1
-      >>> s.bin
-      '00001'
 
-  This feature is still considered a beta as there may be issues with edge cases, especially around the
-  interaction with the 'stream' features of the `BitStream` and `ConstBitStream` classes. For most usage
-  cases it should be solid though, so please report any bugs in the issue tracker.
-      
-* Command line usage. Useful for quick interpretations of binary data.
+You can try out the interactive walkthrough notebook on [binder](https://mybinder.org/v2/gh/scott-griffiths/bitstring/main?labpath=doc%2Fwalkthrough.ipynb), or take a look at the [static version](https://github.com/scott-griffiths/bitstring/blob/main/doc/walkthrough.ipynb).
 
-        $ python -m bitstring int:16=-400
-        0xfe70
 
-* Support for 16 bit floating point types (both IEEE and bfloat).
+[![CI badge](https://github.com/scott-griffiths/bitstring/actions/workflows/.github/workflows/ci.yml/badge.svg)](https://github.com/scott-griffiths/bitstring/actions/workflows/ci.yml)
+[![Docs](https://img.shields.io/readthedocs/bitstring)](https://bitstring.readthedocs.io/en/latest/)
+[![Downloads](https://img.shields.io/pypi/dm/bitstring?color=blue)](https://pypistats.org/packages/bitstring) &nbsp; &nbsp; 
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/scott-griffiths/bitstring/main?labpath=doc%2Fwalkthrough.ipynb)
 
 
 Overview
 --------
 
 * Create bitstrings from hex, octal, binary, files, formatted strings, bytes, integers and floats of different endiannesses.
 * Powerful binary packing and unpacking functions.
 * Bit-level slicing, joining, searching, replacing and more.
 * Read from and interpret bitstrings as streams of binary data.
 * Rich API - chances are that whatever you want to do there's a simple and elegant way of doing it.
 * Open source software, released under the MIT licence.
 
 
+> **Note** \
+> Version 4.0 of bitstring only supports Python 3.7 and later. \
+> Use bitstring version 3.1 if you're using Python 2.7 or 3.6 or earlier.
+
+
 Documentation
 -------------
 The manual for the bitstring module is available at [Read the Docs](https://bitstring.readthedocs.org).
 It contains a walk-through of all the features and a complete [reference section](https://bitstring.readthedocs.io/en/stable/quick_ref.html).
 
 
-Simple Examples
----------------
+Examples
+--------
+
+### Installation
+
+    $ pip install bitstring
 
 ### [Creation](https://bitstring.readthedocs.io/en/stable/creation.html)
 
+     >>> from bitstring import Bits, BitArray, BitStream, pack
      >>> a = BitArray(bin='00101')
      >>> b = Bits(a_file_object)
      >>> c = BitArray('0xff, 0b101, 0o65, uint6=22')
      >>> d = pack('intle16, hex=a, 0b1', 100, a='0x34f')
      >>> e = pack('<16h', *range(16))
 
 ### [Different interpretations, slicing and concatenation](https://bitstring.readthedocs.io/en/stable/interpretation.html)
 
-     >>> a = BitArray('0x1af')
-     >>> a.hex, a.bin, a.uint
-     ('1af', '000110101111', 431)
+     >>> a = BitArray('0x3348')
+     >>> a.hex, a.bin, a.uint, a.float, a.bytes
+     ('3348', '0011001101001000', 13128, 0.2275390625, b'3H')
      >>> a[10:3:-1].bin
-     '1110101'
+     '0101100'
      >>> '0b100' + 3*a
-     BitArray('0x835e35e35, 0b111')
+     BitArray('0x866906690669, 0b000')
 
 ### [Reading data sequentially](https://bitstring.readthedocs.io/en/stable/reading.html)
 
      >>> b = BitStream('0x160120f')
      >>> b.read(12).hex
      '160'
      >>> b.pos = 0
@@ -111,14 +99,60 @@
      >>> c = BitArray('0b00010010010010001111')   # c.hex == '0x1248f'
      >>> c.find('0x48')
      (8,)
      >>> c.replace('0b001', '0xabc')
      >>> c.insert('0b0000', pos=3)
      >>> del c[12:16]
 
+
+New in version 4.0
+------------------
+
+* New Python 3.7 minimum requirement. The code has been updated with type hints and legacy code removed.
+* Shorter and more versative properties are available.
+
+      >>> a = BitArray('u8=20')
+      >>> a += '0b0011, f16=5.52'
+      >>> a[12:].f16
+      5.51953125
+
+* A useful new pretty printing method. Gives a formatted view of a singe or two interpretations of the
+  binary data.
+
+      >>> a = Bits(bytes=b'hello world!!')
+      >>> a.pp('bin, hex', width=40)
+        0: 01101000 01100101   68 65
+       16: 01101100 01101100   6c 6c
+       32: 01101111 00100000   6f 20
+       48: 01110111 01101111   77 6f
+       64: 01110010 01101100   72 6c
+       80: 01100100 00100001   64 21
+       96: 00100001            21   
+
+* LSB0 option (beta). This indexes the bits with the least significant bit being bit zero. This is the
+  opposite way to the standard Python containers but is usual in some relevant fields.
+      
+      >>> bitstring.lsb0 = True
+      >>> s = BitArray('0b00000')
+      >>> s[0] = 1
+      >>> s.bin
+      '00001'
+
+  This feature is still considered a beta as there may be issues with edge cases, especially around the
+  interaction with the 'stream' features of the `BitStream` and `ConstBitStream` classes. For most usage
+  cases it should be solid though, so please report any bugs in the issue tracker.
+      
+* Command line usage. Useful for quick interpretations of binary data.
+
+        $ python -m bitstring int:16=-400
+        0xfe70
+
+* Support for 16 bit floating point types (both IEEE and bfloat).
+
+
 Unit Tests
 ----------
 
 The 600+ unit tests should all pass. They can be run from the root of the project with
 
      python -m unittest
 
@@ -127,8 +161,8 @@
 -------
 
 Created by Scott Griffiths in 2006 to help with ad hoc parsing and creation of compressed video files.
 Maintained and expanded ever since as it became unexpectedly popular. Thanks to all those who have contributed ideas
 and code (and bug reports) over the years.
 
 
-<sub>Copyright (c) 2006 - 2022 Scott Griffiths</sub>
+<sub>Copyright (c) 2006 - 2023 Scott Griffiths</sub>
```

### Comparing `bitstring-4.0.1/bitstring.egg-info/PKG-INFO` & `bitstring-4.0.2/bitstring.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitstring
-Version: 4.0.1
+Version: 4.0.2
 Summary: Simple construction, analysis and modification of binary data.
 Author-email: Scott Griffiths <dr.scottgriffiths@gmail.com>
 Project-URL: homepage, https://github.com/scott-griffiths/bitstring
 Project-URL: documentation, https://bitstring.readthedocs.io/
 Keywords: binary,bitarray,bitvector
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -14,108 +14,78 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 
-![bitstring](https://github.com/scott-griffiths/bitstring/blob/d85c22504882d93b8c0cec373ef03b375e9ea7f8/doc/bitstring_logo_small.png?raw=true "bitstring")
+![bitstring](https://raw.githubusercontent.com/scott-griffiths/bitstring/main/doc/bitstring_logo_small.png "bitstring")
 
 **bitstring** is a pure Python module designed to help make
 the creation and analysis of binary data as simple and natural as possible.
 
-It has been maintained since 2006 and now has about [20 million downloads](https://pypistats.org/packages/bitstring) per year.
+It has been maintained since 2006 and now has about 20 million downloads per year.
 
-> **Note** \
-> \
-> Version 4.0 of bitstring only supports Python 3.7 and later. \
-> Use bitstring version 3.1 if you're using Python 2.7 or 3.6 or earlier.
 
-New in version 4.0
-------------------
+You can try out the interactive walkthrough notebook on [binder](https://mybinder.org/v2/gh/scott-griffiths/bitstring/main?labpath=doc%2Fwalkthrough.ipynb), or take a look at the [static version](https://github.com/scott-griffiths/bitstring/blob/main/doc/walkthrough.ipynb).
 
-* New Python 3.7 minimum requirement. The code has been updated with type hints and legacy code removed.
-* Shorter and more versative properties are available.
 
-      >>> a = BitArray('u8=20')
-      >>> a += '0b0011, f16=5.52'
-      >>> a[12:].f16
-      5.51953125
-
-* A useful new pretty printing method. Gives a formatted view of a singe or two interpretations of the
-  binary data.
-
-      >>> a = Bits(bytes=b'hello world!!')
-      >>> a.pp('bin, hex', width=40)
-        0: 01101000 01100101   68 65
-       16: 01101100 01101100   6c 6c
-       32: 01101111 00100000   6f 20
-       48: 01110111 01101111   77 6f
-       64: 01110010 01101100   72 6c
-       80: 01100100 00100001   64 21
-       96: 00100001            21   
-
-* LSB0 option (beta). This indexes the bits with the least significant bit being bit zero. This is the
-  opposite way to the standard Python containers but is usual in some relevant fields.
-      
-      >>> bitstring.lsb0 = True
-      >>> s = BitArray('0b00000')
-      >>> s[0] = 1
-      >>> s.bin
-      '00001'
-
-  This feature is still considered a beta as there may be issues with edge cases, especially around the
-  interaction with the 'stream' features of the `BitStream` and `ConstBitStream` classes. For most usage
-  cases it should be solid though, so please report any bugs in the issue tracker.
-      
-* Command line usage. Useful for quick interpretations of binary data.
-
-        $ python -m bitstring int:16=-400
-        0xfe70
-
-* Support for 16 bit floating point types (both IEEE and bfloat).
+[![CI badge](https://github.com/scott-griffiths/bitstring/actions/workflows/.github/workflows/ci.yml/badge.svg)](https://github.com/scott-griffiths/bitstring/actions/workflows/ci.yml)
+[![Docs](https://img.shields.io/readthedocs/bitstring)](https://bitstring.readthedocs.io/en/latest/)
+[![Downloads](https://img.shields.io/pypi/dm/bitstring?color=blue)](https://pypistats.org/packages/bitstring) &nbsp; &nbsp; 
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/scott-griffiths/bitstring/main?labpath=doc%2Fwalkthrough.ipynb)
 
 
 Overview
 --------
 
 * Create bitstrings from hex, octal, binary, files, formatted strings, bytes, integers and floats of different endiannesses.
 * Powerful binary packing and unpacking functions.
 * Bit-level slicing, joining, searching, replacing and more.
 * Read from and interpret bitstrings as streams of binary data.
 * Rich API - chances are that whatever you want to do there's a simple and elegant way of doing it.
 * Open source software, released under the MIT licence.
 
 
+> **Note** \
+> Version 4.0 of bitstring only supports Python 3.7 and later. \
+> Use bitstring version 3.1 if you're using Python 2.7 or 3.6 or earlier.
+
+
 Documentation
 -------------
 The manual for the bitstring module is available at [Read the Docs](https://bitstring.readthedocs.org).
 It contains a walk-through of all the features and a complete [reference section](https://bitstring.readthedocs.io/en/stable/quick_ref.html).
 
 
-Simple Examples
----------------
+Examples
+--------
+
+### Installation
+
+    $ pip install bitstring
 
 ### [Creation](https://bitstring.readthedocs.io/en/stable/creation.html)
 
+     >>> from bitstring import Bits, BitArray, BitStream, pack
      >>> a = BitArray(bin='00101')
      >>> b = Bits(a_file_object)
      >>> c = BitArray('0xff, 0b101, 0o65, uint6=22')
      >>> d = pack('intle16, hex=a, 0b1', 100, a='0x34f')
      >>> e = pack('<16h', *range(16))
 
 ### [Different interpretations, slicing and concatenation](https://bitstring.readthedocs.io/en/stable/interpretation.html)
 
-     >>> a = BitArray('0x1af')
-     >>> a.hex, a.bin, a.uint
-     ('1af', '000110101111', 431)
+     >>> a = BitArray('0x3348')
+     >>> a.hex, a.bin, a.uint, a.float, a.bytes
+     ('3348', '0011001101001000', 13128, 0.2275390625, b'3H')
      >>> a[10:3:-1].bin
-     '1110101'
+     '0101100'
      >>> '0b100' + 3*a
-     BitArray('0x835e35e35, 0b111')
+     BitArray('0x866906690669, 0b000')
 
 ### [Reading data sequentially](https://bitstring.readthedocs.io/en/stable/reading.html)
 
      >>> b = BitStream('0x160120f')
      >>> b.read(12).hex
      '160'
      >>> b.pos = 0
@@ -129,14 +99,60 @@
      >>> c = BitArray('0b00010010010010001111')   # c.hex == '0x1248f'
      >>> c.find('0x48')
      (8,)
      >>> c.replace('0b001', '0xabc')
      >>> c.insert('0b0000', pos=3)
      >>> del c[12:16]
 
+
+New in version 4.0
+------------------
+
+* New Python 3.7 minimum requirement. The code has been updated with type hints and legacy code removed.
+* Shorter and more versative properties are available.
+
+      >>> a = BitArray('u8=20')
+      >>> a += '0b0011, f16=5.52'
+      >>> a[12:].f16
+      5.51953125
+
+* A useful new pretty printing method. Gives a formatted view of a singe or two interpretations of the
+  binary data.
+
+      >>> a = Bits(bytes=b'hello world!!')
+      >>> a.pp('bin, hex', width=40)
+        0: 01101000 01100101   68 65
+       16: 01101100 01101100   6c 6c
+       32: 01101111 00100000   6f 20
+       48: 01110111 01101111   77 6f
+       64: 01110010 01101100   72 6c
+       80: 01100100 00100001   64 21
+       96: 00100001            21   
+
+* LSB0 option (beta). This indexes the bits with the least significant bit being bit zero. This is the
+  opposite way to the standard Python containers but is usual in some relevant fields.
+      
+      >>> bitstring.lsb0 = True
+      >>> s = BitArray('0b00000')
+      >>> s[0] = 1
+      >>> s.bin
+      '00001'
+
+  This feature is still considered a beta as there may be issues with edge cases, especially around the
+  interaction with the 'stream' features of the `BitStream` and `ConstBitStream` classes. For most usage
+  cases it should be solid though, so please report any bugs in the issue tracker.
+      
+* Command line usage. Useful for quick interpretations of binary data.
+
+        $ python -m bitstring int:16=-400
+        0xfe70
+
+* Support for 16 bit floating point types (both IEEE and bfloat).
+
+
 Unit Tests
 ----------
 
 The 600+ unit tests should all pass. They can be run from the root of the project with
 
      python -m unittest
 
@@ -145,8 +161,8 @@
 -------
 
 Created by Scott Griffiths in 2006 to help with ad hoc parsing and creation of compressed video files.
 Maintained and expanded ever since as it became unexpectedly popular. Thanks to all those who have contributed ideas
 and code (and bug reports) over the years.
 
 
-<sub>Copyright (c) 2006 - 2022 Scott Griffiths</sub>
+<sub>Copyright (c) 2006 - 2023 Scott Griffiths</sub>
```

### Comparing `bitstring-4.0.1/bitstring.py` & `bitstring-4.0.2/bitstring/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
-__version__ = "4.0.1"
+__version__ = "4.0.2"
 
 __author__ = "Scott Griffiths"
 
 import copy
 import pathlib
 import sys
 import re
@@ -161,35 +161,44 @@
 
     Used internally - not part of public interface.
     """
 
     @classmethod
     def _setlsb0methods(cls, lsb0: bool) -> None:
         if lsb0:
-            cls.getbit = cls._getbit_lsb0
-            cls.setbit = cls._setbit_lsb0
-            cls.unsetbit = cls._unsetbit_lsb0
-            cls.invertbit = cls._invertbit_lsb0
-        else:
-            cls.getbit = cls._getbit_msb0
-            cls.setbit = cls._setbit_msb0
-            cls.unsetbit = cls._unsetbit_msb0
-            cls.invertbit = cls._invertbit_msb0
+            cls.getbit = cls._getbit_lsb0  # type: ignore
+            cls.setbit = cls._setbit_lsb0  # type: ignore
+            cls.unsetbit = cls._unsetbit_lsb0  # type: ignore
+            cls.invertbit = cls._invertbit_lsb0  # type: ignore
+            cls.__iter__ = cls._iter_lsb0  # type: ignore
+        else:
+            cls.getbit = cls._getbit_msb0  # type: ignore
+            cls.setbit = cls._setbit_msb0  # type: ignore
+            cls.unsetbit = cls._unsetbit_msb0  # type: ignore
+            cls.invertbit = cls._invertbit_msb0  # type: ignore
+            cls.__iter__ = cls._iter_msb0  # type: ignore
 
     __slots__ = ('offset', 'rawarray', 'bitlength')
 
     def __init__(self, data: Union[bytearray, MmapByteArray],
                  bitlength: Optional[int] = None, offset: int = 0) -> None:
         self.rawarray = data
         if bitlength is None:
             bitlength = 8 * len(data) - offset
         self.offset = offset
         self.bitlength = bitlength
 
-    def __iter__(self) -> Iterator[bool]:
+    def _iter_lsb0(self) -> Iterator[bool]:
+        # TODO: Rewrite like _iter_msb0
+        # A rather slow but simple version
+        for p in range(0, self.bitlength):
+            yield self._getbit_lsb0(p)
+        return
+
+    def _iter_msb0(self) -> Iterator[bool]:
         start_byte, start_bit = divmod(self.offset, 8)
         end_byte, end_bit = divmod(self.offset + self.bitlength, 8)
 
         try:
             byte = self.rawarray[start_byte]
         except IndexError:
             return  # Empty
@@ -332,46 +341,45 @@
 
 def offsetcopy(s: ByteStore, newoffset: int) -> ByteStore:
     """Return a copy of a ByteStore with the newoffset.
 
     Not part of public interface.
     """
     assert 0 <= newoffset < 8
-    if not s.bitlength:
+    if s.bitlength == 0:
         return copy.copy(s)
+    if newoffset == s.offset % 8:
+        return type(s)(s.getbyteslice(s.byteoffset, s.byteoffset + s.bytelength), s.bitlength, newoffset)
+
+    if isinstance(s.rawarray, MmapByteArray):
+        # Need to make a copy in memory first
+        v = int.from_bytes(s.rawarray[:], 'big')
     else:
-        if newoffset == s.offset % 8:
-            return type(s)(s.getbyteslice(s.byteoffset, s.byteoffset + s.bytelength), s.bitlength, newoffset)
-        newdata = []
-        d = s.rawarray
-        assert newoffset != s.offset % 8
-        if newoffset < s.offset % 8:
-            # We need to shift everything left
-            shiftleft = s.offset % 8 - newoffset
-            # First deal with everything except for the final byte
-            for x in range(s.byteoffset, s.byteoffset + s.bytelength - 1):
-                newdata.append(((d[x] << shiftleft) & 0xff) + (d[x + 1] >> (8 - shiftleft)))
-            bits_in_last_byte = (s.offset + s.bitlength) % 8
-            if not bits_in_last_byte:
-                bits_in_last_byte = 8
-            if bits_in_last_byte > shiftleft:
-                newdata.append((d[s.byteoffset + s.bytelength - 1] << shiftleft) & 0xff)
-        else:  # newoffset > s._offset % 8
-            shiftright = newoffset - s.offset % 8
-            newdata.append(s.getbyte(0) >> shiftright)
-            for x in range(s.byteoffset + 1, s.byteoffset + s.bytelength):
-                newdata.append(((d[x - 1] << (8 - shiftright)) & 0xff) + (d[x] >> shiftright))
-            bits_in_last_byte = (s.offset + s.bitlength) % 8
-            if not bits_in_last_byte:
-                bits_in_last_byte = 8
-            if bits_in_last_byte + shiftright > 8:
-                newdata.append((d[s.byteoffset + s.bytelength - 1] << (8 - shiftright)) & 0xff)
-        new_s = type(s)(bytearray(newdata), s.bitlength, newoffset)
-        assert new_s.offset == newoffset
-        return new_s
+        v = int.from_bytes(s.rawarray, 'big')
+    if newoffset < s.offset % 8:
+        # We need to shift everything left
+        shiftleft = s.offset % 8 - newoffset
+        v <<= shiftleft
+        v &= (1 << 8 * len(s.rawarray)) - 1
+        newdata = v.to_bytes(len(s.rawarray), 'big')
+    else:
+        # Shifting right, but we use a left shift as we don't want to lose any data
+        shiftleft = 8 - newoffset + s.offset % 8
+        v <<= shiftleft
+        newdata = v.to_bytes(len(s.rawarray) + 1, 'big')
+
+    bits_remaining_in_last_byte = (s.offset + s.bitlength) % 8
+    if bits_remaining_in_last_byte == 0:
+        bits_remaining_in_last_byte = 8
+    bits_remaining_in_last_byte -= shiftleft
+    if bits_remaining_in_last_byte <= 0 and len(newdata) > 1:
+        newdata = newdata[:-1]
+
+    new_s = type(s)(bytearray(newdata), s.bitlength, newoffset)
+    return new_s
 
 
 def equal(a: ByteStore, b: ByteStore) -> bool:
     """Return True if ByteStores a == b.
 
     Not part of public interface.
     """
@@ -519,18 +527,18 @@
     def __len__(self) -> int:
         return self.bytelength
 
     # These methods shouldn't ever get called
     def pop(self, __index: int = ...) -> int:
         raise NotImplementedError
     
-    def append(self, __item: Sequence) -> None:
+    def append(self, __item: Union[Sequence, int]) -> None:
         raise NotImplementedError
 
-    def extend(self, __iterable_of_ints: Iterable[Sequence]) -> None:
+    def extend(self, __iterable_of_ints: Union[Iterable[Sequence], bytearray]) -> None:
         raise NotImplementedError
 
     def __iter__(self):
         raise NotImplementedError
     
     def __setitem__(self, key: Union[slice, int], value: Any) -> None:
         raise NotImplementedError
@@ -823,39 +831,34 @@
     len -- Length of the bitstring in bits.
 
     """
 
     @classmethod
     def _setlsb0methods(cls, lsb0: bool) -> None:
         if lsb0:
-            cls._find = cls._find_lsb0
-            cls._rfind = cls._rfind_lsb0
-            cls._findall = cls._findall_lsb0
-            cls._slice = cls._slice_lsb0
-            cls._readuint = cls._readuint_lsb0
-            cls._truncatestart = cls._truncateright
-            cls._truncateend = cls._truncateleft
-            cls._validate_slice = cls._validate_slice_lsb0
-        else:
-            cls._find = cls._find_msb0
-            cls._rfind = cls._rfind_msb0
-            cls._findall = cls._findall_msb0
-            cls._slice = cls._slice_msb0
-            cls._readuint = cls._readuint_msb0
-            cls._truncatestart = cls._truncateleft
-            cls._truncateend = cls._truncateright
-            cls._validate_slice = cls._validate_slice_msb0
+            cls._find = cls._find_lsb0  # type: ignore
+            cls._rfind = cls._rfind_lsb0  # type: ignore
+            cls._findall = cls._findall_lsb0  # type: ignore
+            cls._slice = cls._slice_lsb0  # type: ignore
+            cls._truncatestart = cls._truncateright  # type: ignore
+            cls._truncateend = cls._truncateleft  # type: ignore
+            cls._validate_slice = cls._validate_slice_lsb0  # type: ignore
+        else:
+            cls._find = cls._find_msb0  # type: ignore
+            cls._rfind = cls._rfind_msb0  # type: ignore
+            cls._findall = cls._findall_msb0  # type: ignore
+            cls._slice = cls._slice_msb0  # type: ignore
+            cls._truncatestart = cls._truncateleft  # type: ignore
+            cls._truncateend = cls._truncateright  # type: ignore
+            cls._validate_slice = cls._validate_slice_msb0  # type: ignore
 
     __slots__ = ('_datastore', '_pos')
     # This converts a single octal digit to 3 bits.
     _octToBits: List[str] = ['{0:03b}'.format(i) for i in range(8)]
 
-    # A dictionary of number of 1 bits contained in binary representation of any byte
-    _bitCount: Dict[int, int] = dict(zip(range(0x100), [bin(i).count('1') for i in range(0x100)]))
-
     # Creates dictionaries to quickly reverse single bytes
     _int8ReversalDict: Dict[int, int] = {i: int("{0:08b}".format(i)[::-1], 2) for i in range(0x100)}
     _byteReversalDict: Dict[int, bytes] = {i: bytes([int("{0:08b}".format(i)[::-1], 2)]) for i in range(0x100)}
 
     def __init__(self, auto: Optional[BitsType] = None, length: Optional[int] = None,
                  offset: Optional[int] = None, **kwargs) -> None:
         """Either specify an 'auto' initialiser:
@@ -896,73 +899,15 @@
                   initialising using 'bytes' or 'filename'.
 
         """
         pass
 
     def __new__(cls, auto: Optional[BitsType] = None, length: Optional[int] = None,
                 offset: Optional[int] = None, _cache={}, **kwargs) -> Bits:
-        # Mapping token names to the methods used to set them
-        cls._setfunc = {'bin': cls._setbin_safe,
-                        'hex': cls._sethex,
-                        'oct': cls._setoct,
-                        'ue': cls._setue,
-                        'se': cls._setse,
-                        'uie': cls._setuie,
-                        'sie': cls._setsie,
-                        'bool': cls._setbool,
-                        'uint': cls._setuint,
-                        'int': cls._setint,
-                        'float': cls._setfloatbe,
-                        'bfloat': cls._setbfloatbe,
-                        'bfloatbe': cls._setbfloatbe,
-                        'bfloatle': cls._setbfloatle,
-                        'bfloatne': cls._setbfloatne,
-                        'uintbe': cls._setuintbe,
-                        'intbe': cls._setintbe,
-                        'floatbe': cls._setfloatbe,
-                        'uintle': cls._setuintle,
-                        'intle': cls._setintle,
-                        'floatle': cls._setfloatle,
-                        'uintne': cls._setuintne,
-                        'intne': cls._setintne,
-                        'floatne': cls._setfloatne,
-                        'bytes': cls._setbytes_safe,
-                        'filename': cls._setfile}
-
-        # Dictionary that maps token names to the function that reads them
-        cls._name_to_read = {'uint': Bits._readuint,
-                             'uintle': Bits._readuintle,
-                             'uintbe': Bits._readuintbe,
-                             'uintne': Bits._readuintne,
-                             'int': Bits._readint,
-                             'intle': Bits._readintle,
-                             'intbe': Bits._readintbe,
-                             'intne': Bits._readintne,
-                             'float': Bits._readfloatbe,
-                             'floatbe': Bits._readfloatbe,  # floatbe is a synonym for float
-                             'floatle': Bits._readfloatle,
-                             'floatne': Bits._readfloatne,
-                             'bfloat': Bits._readbfloatbe,
-                             'bfloatbe': Bits._readbfloatbe,
-                             'bfloatle': Bits._readbfloatle,
-                             'bfloatne': Bits._readbfloatne,
-                             'hex': Bits._readhex,
-                             'oct': Bits._readoct,
-                             'bin': Bits._readbin,
-                             'bits': Bits._readbits,
-                             'bytes': Bits._readbytes,
-                             'ue': Bits._readue,
-                             'se': Bits._readse,
-                             'uie': Bits._readuie,
-                             'sie': Bits._readsie,
-                             'bool': Bits._readbool,
-                             'pad': Bits._readpad}
-
-        # For instances auto-initialised with a string we intern the
-        # instance for re-use.
+        # For instances auto-initialised with a string we intern the instance for re-use.
         if isinstance(auto, str):
             try:
                 return _cache[auto]
             except KeyError:
                 x = object.__new__(Bits)
                 try:
                     _, tokens = tokenparser(auto)
@@ -1191,17 +1136,17 @@
         length = self.len
         pos_string = "" if self._pos in (0, None) else f", pos={self._pos}"
         if isinstance(self._datastore.rawarray, MmapByteArray):
             offsetstring = ''
             if self._datastore.byteoffset or self._offset:
                 offsetstring = ", offset=%d" % (self._datastore.rawarray.byteoffset * 8 + self._offset)
             lengthstring = ", length=%d" % length
-            return "{0}(filename='{1}'{2}{3}{4})".format(self.__class__.__name__,
-                                                         self._datastore.rawarray.source.name,
-                                                         lengthstring, offsetstring, pos_string)
+            return "{0}(filename={1}{2}{3}{4})".format(self.__class__.__name__,
+                                                       repr(str(self._datastore.rawarray.source.name)),
+                                                       lengthstring, offsetstring, pos_string)
         else:
             s = self.__str__()
             lengthstring = ''
             if s.endswith('...'):
                 lengthstring = "  # length={0}".format(length)
             return "{0}('{1}'{2}){3}".format(self.__class__.__name__, s, pos_string, lengthstring)
 
@@ -1246,15 +1191,15 @@
 
         """
         if n < 0:
             raise ValueError("Cannot shift by a negative amount.")
         if not self.len:
             raise ValueError("Cannot shift an empty bitstring.")
         n = min(n, self.len)
-        s = self._slice(n, self.len)
+        s = self._absolute_slice(n, self.len)
         s._addright(Bits(n))
         return s
 
     def __rshift__(self, n: int) -> Bits:
         """Return bitstring with bits shifted by n to the right.
 
         n -- the number of bits to shift. Must be >= 0.
@@ -1263,15 +1208,16 @@
         if n < 0:
             raise ValueError("Cannot shift by a negative amount.")
         if not self.len:
             raise ValueError("Cannot shift an empty bitstring.")
         if not n:
             return self._copy()
         s = self.__class__(length=min(n, self.len))
-        s._addright(self[:-n])
+        n = min(n, self.len)
+        s._addright(self._absolute_slice(0, self.len - n))
         return s
 
     def __mul__(self, n: int) -> Bits:
         """Return bitstring consisting of n concatenations of self.
 
         Called for expression of the form 'a = b*3'.
         n -- The number of concatenations. Must be >= 0.
@@ -1290,90 +1236,90 @@
 
         Called for expressions of the form 'a = 3*b'.
         n -- The number of concatenations. Must be >= 0.
 
         """
         return self.__mul__(n)
 
-    def __and__(self, bs: Any) -> Bits:
+    def __and__(self, bs: BitsType) -> Bits:
         """Bit-wise 'and' between two bitstrings. Returns new bitstring.
 
         bs -- The bitstring to '&' with.
 
         Raises ValueError if the two bitstrings have differing lengths.
 
         """
         bs = Bits(bs)
         if self.len != bs.len:
             raise ValueError("Bitstrings must have the same length for & operator.")
         s = self._copy()
         s._iand(bs)
         return s
 
-    def __rand__(self, bs: Any) -> Bits:
+    def __rand__(self, bs: BitsType) -> Bits:
         """Bit-wise 'and' between two bitstrings. Returns new bitstring.
 
         bs -- the bitstring to '&' with.
 
         Raises ValueError if the two bitstrings have differing lengths.
 
         """
         return self.__and__(bs)
 
-    def __or__(self, bs: Any) -> Bits:
+    def __or__(self, bs: BitsType) -> Bits:
         """Bit-wise 'or' between two bitstrings. Returns new bitstring.
 
         bs -- The bitstring to '|' with.
 
         Raises ValueError if the two bitstrings have differing lengths.
 
         """
         bs = Bits(bs)
         if self.len != bs.len:
             raise ValueError("Bitstrings must have the same length for | operator.")
         s = self._copy()
         s._ior(bs)
         return s
 
-    def __ror__(self, bs: Any) -> Bits:
+    def __ror__(self, bs: BitsType) -> Bits:
         """Bit-wise 'or' between two bitstrings. Returns new bitstring.
 
         bs -- The bitstring to '|' with.
 
         Raises ValueError if the two bitstrings have differing lengths.
 
         """
         return self.__or__(bs)
 
-    def __xor__(self, bs: Any) -> Bits:
+    def __xor__(self, bs: BitsType) -> Bits:
         """Bit-wise 'xor' between two bitstrings. Returns new bitstring.
 
         bs -- The bitstring to '^' with.
 
         Raises ValueError if the two bitstrings have differing lengths.
 
         """
         bs = Bits(bs)
         if self.len != bs.len:
             raise ValueError("Bitstrings must have the same length for ^ operator.")
         s = self._copy()
         s._ixor(bs)
         return s
 
-    def __rxor__(self, bs: Any) -> Bits:
+    def __rxor__(self, bs: BitsType) -> Bits:
         """Bit-wise 'xor' between two bitstrings. Returns new bitstring.
 
         bs -- The bitstring to '^' with.
 
         Raises ValueError if the two bitstrings have differing lengths.
 
         """
         return self.__xor__(bs)
 
-    def __contains__(self, bs: Any) -> bool:
+    def __contains__(self, bs: BitsType) -> bool:
         """Return whether bs is contained in the current bitstring.
 
         bs -- The bitstring to search for.
 
         """
         # Don't want to change pos
         pos = self._pos
@@ -1584,14 +1530,21 @@
         data = int.to_bytes(uint, (length + 7) // 8, 'big')
 
         offset = 8 - (length % 8)
         if offset == 8:
             offset = 0
         self._setbytes_unsafe(bytearray(data), length, offset)
 
+    def _readuint(self, start: int, length: int) -> int:
+        # TODO: This needs to be refactored again.
+        if _lsb0:
+            return self._readuint_lsb0(start, length)
+        else:
+            return self._readuint_msb0(start, length)
+
     def _readuint_lsb0(self, start: int, length: int) -> int:
         return self._readuint_msb0(self.len - start - length, length)
 
     def _readuint_msb0(self, start: int, length: int) -> int:
         """Read bits and interpret as an unsigned int."""
         if length == 0:
             raise InterpretError("Cannot interpret a zero length bitstring as an integer.")
@@ -1735,27 +1688,30 @@
             raise CreationError("A non-zero length must be specified with a float initialiser.")
         try:
             b = struct.pack(struct_dict[length], f)
             self._setbytes_unsafe(bytearray(b), length, 0)
         except KeyError:
             raise CreationError(f"Floats can only be 16, 32 or 64 bits long, not {length} bits")
         except (OverflowError, struct.error):
-            if length == 16:
-                # Not sure why only f16 overflows. Other types go to 'inf'. Could do the same here?
-                raise CreationError(f"Overflow trying to create float16 from {f}.")
+            # If float64 doesn't fit it automatically goes to 'inf'. This reproduces that behaviour for other types.
+            if length in [16, 32]:
+                b = struct.pack(struct_dict[length], float('inf') if f > 0 else float('-inf'))
+                self._setbytes_unsafe(bytearray(b), length, 0)
 
     def _readfloat(self, start: int, length: int, struct_dict: Dict[int, str]) -> float:
         """Read bits and interpret as a float."""
         try:
             fmt = struct_dict[length]
         except KeyError:
             raise InterpretError(f"Floats can only be 16, 32 or 64 bits long, not {length} bits")
 
+        if _lsb0:
+            start = self._getlength() - start - length
         startbyte, offset = divmod(start + self._offset, 8)
-        if not offset:
+        if offset == 0:
             return struct.unpack(fmt, bytes(self._datastore.getbyteslice(startbyte, startbyte + length // 8)))[0]
         else:
             return struct.unpack(fmt, self._readbytes(start, length))[0]
 
     def _setfloatbe(self, f: float, length: Optional[int] = None, _offset: None = None) -> None:
         self._setfloat(f, {16: '>e', 32: '>f', 64: '>d'}, length)
 
@@ -1780,30 +1736,30 @@
 
     def _getbfloatbe(self) -> float:
         return self._readbfloatbe(0, self.len)
 
     def _readbfloatbe(self, start: int, _length: int) -> float:
         if _length != 16:
             raise InterpretError(f"bfloats must be length 16, received a length of {_length} bits.")
-        two_bytes = self._readbits(start, 16)
+        two_bytes = self._slice(start, start + 16)
         zero_padded = two_bytes + Bits(16)
         return zero_padded._getfloatbe()
 
     def _setbfloatbe(self, f: Union[float, str], length: Optional[int] = None, _offset: None = None) -> None:
         if length is not None and length != 16:
             raise CreationError(f"bfloats must be length 16, received a length of {length} bits.")
         f = float(f)
         four_byte_float = Bits(float=f, length=32)
         self._setbytes_unsafe(four_byte_float._datastore.rawarray[0:2], 16, 0)
 
     def _getbfloatle(self) -> float:
         return self._readbfloatle(0, self.len)
 
     def _readbfloatle(self, start: int, _length: int) -> float:
-        two_bytes = self._readbits(start, 16)
+        two_bytes = self._slice(start, start + 16)
         zero_padded = Bits(16) + two_bytes
         return zero_padded._getfloatle()
 
     def _setbfloatle(self, f: Union[float, str], length: Optional[int] = None, _offset: None = None) -> None:
         if length is not None and length != 16:
             raise CreationError(f"bfloats must be length 16, received a length of {length} bits.")
         f = float(f)
@@ -2021,51 +1977,46 @@
         if self.length != 1:
             raise InterpretError(f"For a bool interpretation a bitstring must be 1 bit long, not {self.length} bits.")
         return self[0]
 
     def _readbool(self, pos: int, _length: None = None) -> Tuple[int, int]:
         return self[pos], pos + 1
 
-    @staticmethod
-    def _readpad(_self, _pos, _length) -> None:
+    def _readpad(self, _pos, _length) -> None:
         return None
 
     def _setbin_safe(self, binstring: str, _length: None = None, _offset: None = None) -> None:
         """Reset the bitstring to the value given in binstring."""
         binstring = tidy_input_string(binstring)
         # remove any 0b if present
         binstring = binstring.replace('0b', '')
         self._setbin_unsafe(binstring)
 
     def _setbin_unsafe(self, binstring: str, _length: None = None, _offset: None = None) -> None:
         """Same as _setbin_safe, but input isn't sanity checked. binstring mustn't start with '0b'."""
-        length = len(binstring)
-        # pad with zeros up to byte boundary if needed
-        boundary = ((length + 7) // 8) * 8
-        padded_binstring = binstring + '0' * (boundary - length) if len(binstring) < boundary else binstring
+        if binstring == '':
+            self._setbytes_unsafe(bytearray(), 0, 0)
+            return
         try:
-            bytelist = [int(padded_binstring[x:x + 8], 2)
-                        for x in range(0, len(padded_binstring), 8)]
+            i = int(binstring, 2)
         except ValueError:
             raise CreationError(f"Invalid character in bin initialiser {binstring}.")
-        self._setbytes_unsafe(bytearray(bytelist), length, 0)
+        if len(binstring) % 8 != 0:
+            i <<= 8 - (len(binstring) % 8)
+        b = i.to_bytes((len(binstring) + 7) // 8, 'big')
+        self._setbytes_unsafe(bytearray(b), len(binstring), 0)
 
     def _readbin(self, start: int, length: int) -> str:
         """Read bits and interpret as a binary string."""
-        if not length:
+        if length == 0:
             return ''
-        # Get the byte slice containing our bit slice
-        startbyte, startoffset = divmod(start + self._offset, 8)
-        endbyte, endbit = divmod(start + self._offset + length - 1, 8)
-        b = self._datastore.getbyteslice(startbyte, endbyte + 1)
-        # Convert to a string of '0' and '1's
+        b = self._slice(start, start + length).tobytes()
         integer = int.from_bytes(b, 'big')
         c = "{:0{}b}".format(integer, 8*len(b))
-        # Finally chop off any extra bits.
-        return c[startoffset:startoffset + length]
+        return c[0:length]
 
     def _getbin(self) -> str:
         """Return interpretation as a binary string."""
         return self._readbin(0, self.len)
 
     def _setoct(self, octstring: str, _length: None = None, _offset: None = None) -> None:
         """Reset the bitstring to have the value given in octstring."""
@@ -2174,18 +2125,23 @@
         s_copy = self.__class__()
         s_copy._setbytes_unsafe(self._datastore.getbyteslice(0, self._datastore.bytelength),
                                 self.len, self._offset)
         return s_copy
 
     def _slice_lsb0(self, start: int, end: int) -> Bits:
         """Used internally to get a slice, without error checking (LSB0)."""
-        return self._slice_msb0(self.length - end, self.length - start)
+        return self._absolute_slice(self.length - end, self.length - start)
 
     def _slice_msb0(self, start: int, end: int) -> Bits:
-        """Used internally to get a slice, without error checking."""
+        """Used internally to get a slice, without error checking (MSB0)."""
+        return self._absolute_slice(start, end)
+
+    def _absolute_slice(self, start: int, end: int) -> Bits:
+        """Used internally to get a slice, without error checking.
+        Uses MSB0 bit numbering even if LSB0 is set."""
         if end == start:
             return self.__class__()
         assert start < end, f"start={start}, end={end}"
         offset = self._offset
         startbyte, newoffset = divmod(start + offset, 8)
         endbyte = (end + offset - 1) // 8
         bs = self.__class__()
@@ -2228,29 +2184,29 @@
         self._setbytes_unsafe(bytearray().join(n), self.length, newoffset)
 
     def _truncateleft(self, bits: int) -> Bits:
         """Truncate bits from the start of the bitstring. Return the truncated bits."""
         assert 0 <= bits <= self.len
         if not bits:
             return Bits()
-        truncated_bits = self._slice_msb0(0, bits)
+        truncated_bits = self._absolute_slice(0, bits)
         if bits == self.len:
             self._clear()
             return truncated_bits
         bytepos, offset = divmod(self._offset + bits, 8)
         self._setbytes_unsafe(self._datastore.getbyteslice(bytepos, self._datastore.bytelength), self.len - bits,
                               offset)
         return truncated_bits
 
     def _truncateright(self, bits: int) -> Bits:
         """Truncate bits from the end of the bitstring. Return the truncated bits."""
         assert 0 <= bits <= self.len
         if not bits:
             return Bits()
-        truncated_bits = self._slice_lsb0(0, bits)
+        truncated_bits = self._absolute_slice(self.length - bits, self.length)
         if bits == self.len:
             self._clear()
             return truncated_bits
         newlength_in_bytes = (self._offset + self.len - bits + 7) // 8
         self._setbytes_unsafe(self._datastore.getbyteslice(0, newlength_in_bytes), self.len - bits,
                               self._offset)
         return truncated_bits
@@ -2569,44 +2525,63 @@
                 p += pos
                 break
             p += increment
         if not found:
             return ()
         return (p * 8,)
 
-    def _findregex(self, reg_ex: Pattern[str], start: int, end: int, bytealigned: bool) -> Union[Tuple[int], Tuple[()]]:
-        """Find first occurrence of a compiled regular expression.
-
-        Note that this doesn't support arbitrary regexes, in particular they
-        must match a known length.
-
-        """
+    def _findbin(self, binstr: str, start: int, end: int, bytealigned: bool) -> Union[Tuple[int], Tuple[()]]:
+        """Find first occurrence of a binary string."""
         p = start
-        length = len(reg_ex.pattern)
+        length = len(binstr)
         # We grab overlapping chunks of the binary representation and
         # do an ordinary string search within that.
-        increment = max(4096, length * 10)
+        increment = max(4096, length * 64)
         buffersize = increment + length
         while p < end:
             buf = self._readbin(p, min(buffersize, end - p))
-            # Test using regular expressions...
-            m = reg_ex.search(buf)
-            if m:
-                pos = m.start()
-                # if bytealigned then we only accept byte aligned positions.
-                if not bytealigned or (p + pos) % 8 == 0:
+            pos = buf.find(binstr)
+            if pos != -1:
+                if not bytealigned:
                     return (p + pos,)
-                if bytealigned:
-                    # Advance to just beyond the non-byte-aligned match and try again...
-                    p += pos + 1
-                    continue
+                if (p + pos) % 8 == 0:  # TODO: Is this logic only right for MSB0?
+                    return (p + pos,)
+                # Advance to just beyond the non-byte-aligned match and try again...
+                p += pos + 1
+                continue
             p += increment
         # Not found, return empty tuple
         return ()
 
+    def _rfindbin(self, binstr: str, start: int, end: int, bytealigned: bool) -> Union[Tuple[int], Tuple[()]]:
+        """Find final occurrence of a binary string."""
+        p = end
+        # We grab overlapping chunks of the binary representation and
+        # do an ordinary string search within that.
+        increment = max(4096, len(binstr) * 64)
+        buffersize = increment + len(binstr)
+        while p > start:
+            start_pos = max(start, p - buffersize)
+            if not _lsb0:
+                buf = self._readbin(start_pos, p - start_pos)
+            else:
+                buf = self._readbin(self.len - p, p - start_pos)
+            pos = buf.rfind(binstr)
+            if pos != -1:
+                if not bytealigned:
+                    return (pos + start_pos,)
+                if (pos + start_pos) % 8 == 0:
+                    return (pos + start_pos,)
+                # Advance to just beyond the non-byte-aligned match and try again...
+                p = pos + start_pos + len(binstr) - 1
+                continue
+            p -= increment
+        # Not found, return empty tuple
+        return ()
+
     def find(self, bs: BitsType, start: Optional[int] = None, end: Optional[int] = None,
              bytealigned: Optional[bool] = None) -> Union[Tuple[int], Tuple[()]]:
         """Find first occurrence of substring bs.
 
         Returns a single item tuple with the bit position if found, or an
         empty tuple if not found. The bit position (pos property) will
         also be set to the start of the substring if it is found.
@@ -2625,33 +2600,34 @@
         (6,)
 
         """
         bs = Bits(bs)
         if bs.len == 0:
             raise ValueError("Cannot find an empty bitstring.")
         start, end = self._validate_slice(start, end)
-        ba = globals()['_bytealigned'] if bytealigned is None else bytealigned
+        ba = _bytealigned if bytealigned is None else bytealigned
         return self._find(bs, start, end, ba)
 
     def _find_lsb0(self, bs: Bits, start: int, end: int, bytealigned: bool) -> Union[Tuple[int], Tuple[()]]:
-        # A find in lsb0 is very like a reverse find in msb0.
-        p = self._rfind_msb0(bs, start, end, bytealigned)
+        assert start <= end
+        p = self._rfindbin(bs._getbin(), start, end, bytealigned)
+
         if p:
-            newpos = self.len - p[0] - bs.length
+            newpos = self.length - p[0] - bs.length
             if self._pos is not None:
                 self._pos = newpos
             return (newpos,)
         else:
             return ()
 
     def _find_msb0(self, bs: Bits, start: int, end: int, bytealigned: bool) -> Union[Tuple[int], Tuple[()]]:
         if bytealigned and not bs.len % 8 and not self._datastore.offset:
             p = self._findbytes(bs.bytes, start, end)
         else:
-            p = self._findregex(re.compile(bs._getbin()), start, end, bytealigned)
+            p = self._findbin(bs._getbin(), start, end, bytealigned)
         # If called from a class that has a pos, set it
         if p and self._pos is not None:
             self._pos = p[0]
         return p
 
     def findall(self, bs: Any, start: Optional[int] = None, end: Optional[int] = None, count: Optional[int] = None,
                 bytealigned: Optional[bool] = None) -> Generator[int, None, None]:
@@ -2671,25 +2647,25 @@
         Note that all occurrences of bs are found, even if they overlap.
 
         """
         if count is not None and count < 0:
             raise ValueError("In findall, count must be >= 0.")
         bs = Bits(bs)
         start, end = self._validate_slice(start, end)
-        ba = globals()['_bytealigned'] if bytealigned is None else bytealigned
+        ba = _bytealigned if bytealigned is None else bytealigned
         return self._findall(bs, start, end, count, ba)
 
     def _findall_msb0(self, bs: Bits, start: int, end: int, count: Optional[int],
                       bytealigned: bool) -> Generator[int, None, None]:
         c = 0
         if bytealigned and not bs.len % 8 and not self._datastore.offset:
             # Use the quick find method
             f = functools.partial(self._findbytes, bytes_=bs._getbytes())
         else:
-            f = functools.partial(self._findregex, reg_ex=re.compile(bs._getbin()), bytealigned=bytealigned)
+            f = functools.partial(self._findbin, binstr=bs._getbin(), bytealigned=bytealigned)
         while True:
             if count is not None and c >= count:
                 return
             p = f(start=start, end=end)
             if not p:
                 break
             c += 1
@@ -2702,14 +2678,15 @@
                 start = p[0] + 1
             if start >= end:
                 break
         return
 
     def _findall_lsb0(self, bs: Bits, start: int, end: int, count: Optional[int],
                       bytealigned: bool) -> Generator[int, None, None]:
+        assert start <= end
         # Search chunks starting near the end and then moving back.
         c = 0
         increment = max(8192, bs.len * 80)
         buffersize = min(increment + bs.len, end - start)
         pos = max(start, end - buffersize)
         while True:
             found = list(self._findall_msb0(bs, start=pos, end=pos + buffersize, count=None,
@@ -2745,34 +2722,25 @@
 
         Raises ValueError if bs is empty, if start < 0, if end > len(self) or
         if end < start.
 
         """
         bs = Bits(bs)
         start, end = self._validate_slice(start, end)
-        ba = globals()['_bytealigned'] if bytealigned is None else bytealigned
+        ba = _bytealigned if bytealigned is None else bytealigned
         if not bs.len:
             raise ValueError("Cannot find an empty bitstring.")
-        return self._rfind(bs, start, end, ba)
+        p = self._rfind(bs, start, end, ba)
+        # If called from a class that has a pos, set it
+        if p and self._pos is not None:
+            self._pos = p[0]
+        return p
 
     def _rfind_msb0(self, bs: Bits, start: int, end: int, bytealigned: bool) -> Union[Tuple[int], Tuple[()]]:
-        # Search chunks starting near the end and then moving back
-        # until we find bs.
-        increment = max(8192, bs.len * 80)
-        buffersize = min(increment + bs.len, end - start)
-        pos = max(start, end - buffersize)
-        while True:
-            found = list(self._findall_msb0(bs, start=pos, end=pos + buffersize, count=None,
-                                            bytealigned=bytealigned))
-            if not found:
-                if pos == start:
-                    return ()
-                pos = max(start, pos - increment)
-                continue
-            return (found[-1],)
+        return self._rfindbin(bs.bin, start, end, bytealigned)
 
     def _rfind_lsb0(self, bs: Bits, start: int, end: int, bytealigned: bool) -> Union[Tuple[int], Tuple[()]]:
         # A reverse find in lsb0 is very like a forward find in msb0.
         p = self._find_msb0(bs, start, end, bytealigned)
         if p:
             newpos = self.len - p[0] - bs.length
             if self._pos is not None:
@@ -2828,24 +2796,24 @@
         Raises ValueError if the delimiter is empty.
 
         """
         delimiter = Bits(delimiter)
         if not delimiter.len:
             raise ValueError("split delimiter cannot be empty.")
         start, end = self._validate_slice(start, end)
-        bytealigned_: bool = globals()['_bytealigned'] if bytealigned is None else bytealigned
+        bytealigned_: bool = _bytealigned if bytealigned is None else bytealigned
         if count is not None and count < 0:
             raise ValueError("Cannot split - count must be >= 0.")
         if count == 0:
             return
         if bytealigned_ and not delimiter.len % 8 and not self._datastore.offset:
             # Use the quick find method
             f = functools.partial(self._findbytes, bytes_=delimiter._getbytes())
         else:
-            f = functools.partial(self._findregex, reg_ex=re.compile(delimiter._getbin()), bytealigned=bytealigned_)
+            f = functools.partial(self._findbin, binstr=delimiter._getbin(), bytealigned=bytealigned_)
         found = f(start=start, end=end)
         if not found:
             # Initial bits are the whole bitstring being searched
             yield self._slice(start, end)
             return
         # yield the bytes before the first occurrence of the delimiter, even if empty
         yield self._slice(start, found[0])
@@ -3009,25 +2977,16 @@
         value -- If bool(value) is True then bits set to 1 are counted, otherwise bits set
                  to 0 are counted.
 
         >>> Bits('0xef').count(1)
         7
 
         """
-        if not self.len:
-            return 0
         # count the number of 1s (from which it's easy to work out the 0s).
-        # Don't count the final byte yet.
-        count = sum(Bits._bitCount[self._datastore.getbyte(i)] for i in range(self._datastore.bytelength - 1))
-        # adjust for bits at start that aren't part of the bitstring
-        if self._offset:
-            count -= Bits._bitCount[self._datastore.getbyte(0) >> (8 - self._offset)]
-        # and count the last 1 - 8 bits at the end.
-        endbits = self._datastore.bytelength * 8 - (self._offset + self.len)
-        count += Bits._bitCount[self._datastore.getbyte(self._datastore.bytelength - 1) >> endbits]
+        count = (self._getbin()).count('1')
         return count if value else self.len - count
 
     def pp(self, fmt: str = 'bin', width: int = 120, sep: Optional[str] = ' ',
            show_offset: bool = True, stream: TextIO = sys.stdout) -> None:
         """Pretty print the bitstring's value.
 
         fmt -- Printed data format. One of 'bin', 'oct', 'hex' or 'bytes'. Defaults to 'bin'.
@@ -3305,14 +3264,77 @@
     i = int
     u = uint
     f = float
     b = bin
     o = oct
     h = hex
 
+    # Dictionary that maps token names to the function that reads them
+    _name_to_read = {'uint': _readuint,
+                     'u': _readuint,
+                     'uintle': _readuintle,
+                     'uintbe': _readuintbe,
+                     'uintne': _readuintne,
+                     'int': _readint,
+                     'i': _readint,
+                     'intle': _readintle,
+                     'intbe': _readintbe,
+                     'intne': _readintne,
+                     'float': _readfloatbe,
+                     'f': _readfloatbe,
+                     'floatbe': _readfloatbe,  # floatbe is a synonym for float
+                     'floatle': _readfloatle,
+                     'floatne': _readfloatne,
+                     'bfloat': _readbfloatbe,
+                     'bfloatbe': _readbfloatbe,
+                     'bfloatle': _readbfloatle,
+                     'bfloatne': _readbfloatne,
+                     'hex': _readhex,
+                     'h': _readhex,
+                     'oct': _readoct,
+                     'o': _readoct,
+                     'bin': _readbin,
+                     'b': _readbin,
+                     'bits': _readbits,
+                     'bytes': _readbytes,
+                     'ue': _readue,
+                     'se': _readse,
+                     'uie': _readuie,
+                     'sie': _readsie,
+                     'bool': _readbool,
+                     'pad': _readpad}
+
+    # Mapping token names to the methods used to set them
+    _setfunc = {'bin': _setbin_safe,
+                'hex': _sethex,
+                'oct': _setoct,
+                'ue': _setue,
+                'se': _setse,
+                'uie': _setuie,
+                'sie': _setsie,
+                'bool': _setbool,
+                'uint': _setuint,
+                'int': _setint,
+                'float': _setfloatbe,
+                'bfloat': _setbfloatbe,
+                'bfloatbe': _setbfloatbe,
+                'bfloatle': _setbfloatle,
+                'bfloatne': _setbfloatne,
+                'uintbe': _setuintbe,
+                'intbe': _setintbe,
+                'floatbe': _setfloatbe,
+                'uintle': _setuintle,
+                'intle': _setintle,
+                'floatle': _setfloatle,
+                'uintne': _setuintne,
+                'intne': _setintne,
+                'floatne': _setfloatne,
+                'bytes': _setbytes_safe,
+                'filename': _setfile}
+
 
 class BitArray(Bits):
     """A container holding a mutable sequence of bits.
 
     Subclass of the immutable Bits class. Inherits all of its
     methods (except __hash__) and adds mutating methods.
 
@@ -3384,29 +3406,30 @@
     len -- Length of the bitstring in bits.
 
     """
 
     @classmethod
     def _setlsb0methods(cls, lsb0: bool) -> None:
         if lsb0:
-            cls._overwrite = cls._overwrite_lsb0
-            cls._insert = cls._insert_lsb0
-            cls._delete = cls._delete_lsb0
-            cls._ror = cls._rol_msb0
-            cls._rol = cls._ror_msb0
-            cls._append = cls._append_lsb0
-            cls._prepend = cls._append_msb0  # An LSB0 prepend is an MSB0 append
-        else:
-            cls._overwrite = cls._overwrite_msb0
-            cls._insert = cls._insert_msb0
-            cls._delete = cls._delete_msb0
-            cls._ror = cls._ror_msb0
-            cls._rol = cls._rol_msb0
-            cls._append = cls._append_msb0
-            cls._prepend = cls._append_lsb0
+            cls._overwrite = cls._overwrite_lsb0  # type: ignore
+            cls._insert = cls._insert_lsb0  # type: ignore
+            cls._delete = cls._delete_lsb0  # type: ignore
+            cls._ror = cls._rol_msb0  # type: ignore
+            cls._rol = cls._ror_msb0  # type: ignore
+            cls._append = cls._append_lsb0  # type: ignore
+            # An LSB0 prepend is an MSB0 append
+            cls._prepend = cls._append_msb0  # type: ignore
+        else:
+            cls._overwrite = cls._overwrite_msb0  # type: ignore
+            cls._insert = cls._insert_msb0  # type: ignore
+            cls._delete = cls._delete_msb0  # type: ignore
+            cls._ror = cls._ror_msb0  # type: ignore
+            cls._rol = cls._rol_msb0  # type: ignore
+            cls._append = cls._append_msb0  # type: ignore
+            cls._prepend = cls._append_lsb0  # type: ignore
 
     __slots__ = ()
 
     # As BitArray objects are mutable, we shouldn't allow them to be hashed.
     __hash__: None = None
 
     def __init__(self, auto: Optional[BitsType] = None, length: Optional[int] = None,
@@ -3759,15 +3782,15 @@
         """
         old = Bits(old)
         new = Bits(new)
         if not old.len:
             raise ValueError("Empty bitstring cannot be replaced.")
         start, end = self._validate_slice(start, end)
         if bytealigned is None:
-            bytealigned = globals()['_bytealigned']
+            bytealigned = _bytealigned
         # Adjust count for use in split()
         if count is not None:
             count += 1
         sections = self.split(old, start, end, count, bytealigned)
         lengths = [s.len for s in sections]
         if len(lengths) == 1:
             # Didn't find anything to replace.
@@ -3902,17 +3925,19 @@
         pos -- Either a single bit position or an iterable of bit positions.
                Negative numbers are treated in the same way as slice indices.
                Defaults to the entire bitstring.
 
         Raises IndexError if pos < -len(self) or pos >= len(self).
 
         """
-        f = self._set if value else self._unset
         if pos is None:
-            pos = range(self.len)
+            # Set all bits to either 1 or 0
+            self._setint(-1 if value else 0)
+            return
+        f = self._set if value else self._unset
         if not isinstance(pos, abc.Iterable):
             pos = (pos,)
         length = self.len
         for p in pos:
             if p < 0:
                 p += length
             if not 0 <= p < length:
@@ -4001,18 +4026,18 @@
                whole bitstring.
         start -- Start bit position, defaults to 0.
         end -- End bit position, defaults to len(self).
         repeat -- If True (the default) the byte swapping pattern is repeated
                   as much as possible.
 
         """
-        start, end = self._validate_slice(start, end)
+        start_v, end_v = self._validate_slice(start, end)
         if fmt is None or fmt == 0:
             # reverse all of the whole bytes.
-            bytesizes = [(end - start) // 8]
+            bytesizes = [(end_v - start_v) // 8]
         elif isinstance(fmt, int):
             if fmt < 0:
                 raise ValueError(f"Improper byte length {fmt}.")
             bytesizes = [fmt]
         elif isinstance(fmt, str):
             m = STRUCT_PACK_RE.match(fmt)
             if not m:
@@ -4031,24 +4056,24 @@
             for bytesize in bytesizes:
                 if not isinstance(bytesize, int) or bytesize < 0:
                     raise ValueError(f"Improper byte length {bytesize}.")
         else:
             raise TypeError("Format must be an integer, string or iterable.")
 
         repeats = 0
-        totalbitsize = 8 * sum(bytesizes)
+        totalbitsize: int = 8 * sum(bytesizes)
         if not totalbitsize:
             return 0
         if repeat:
             # Try to repeat up to the end of the bitstring.
-            finalbit = end
+            finalbit = end_v
         else:
             # Just try one (set of) byteswap(s).
-            finalbit = start + totalbitsize
-        for patternend in range(start + totalbitsize, finalbit + 1, totalbitsize):
+            finalbit = start_v + totalbitsize
+        for patternend in range(start_v + totalbitsize, finalbit + 1, totalbitsize):
             bytestart = patternend - totalbitsize
             for bytesize in bytesizes:
                 byteend = bytestart + bytesize * 8
                 self._reversebytes(bytestart, byteend)
                 bytestart += bytesize * 8
             repeats += 1
         return repeats
@@ -4682,15 +4707,15 @@
                 s._append(kwargs[name])
                 continue
             if length is not None:
                 length = int(length)
             if value is None and name != 'pad':
                 # Take the next value from the ones provided
                 value = next(value_iter)
-            s._addright(BitStream._init_with_token(name, length, value))
+            s._append(BitStream._init_with_token(name, length, value))
     except StopIteration:
         raise CreationError(f"Not enough parameters present to pack according to the "
                             "format. {len(tokens)} values are needed.")
     try:
         next(value_iter)
     except StopIteration:
         # Good, we've used up all the *values.
@@ -4737,15 +4762,16 @@
 $ python -m bitstring float:32=0.2 bin
 00111110010011001100110011001101
 $ python -m bitstring 0xff 3*0b01,0b11 uint
 65367
 $ python -m bitstring hex=01, uint:12=352.hex
 01160
         """)
-    elif fp in dummy._name_to_read.keys():
+        return
+    if fp in dummy._name_to_read.keys():
         # concatenate all other parameters and interpret using the final one
         b1 = Bits(','.join(sys.argv[1: -1]))
         print(b1._readtoken(fp, 0, b1.__len__())[0])
     else:
         # does final parameter end with a dot then an interpretation string?
         interp = fp[fp.rfind('.') + 1:]
         if interp in dummy._name_to_read.keys():
```

### Comparing `bitstring-4.0.1/pyproject.toml` & `bitstring-4.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,29 @@
+[build-system]
+requires = ["setuptools>=61"]
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "bitstring"
-version = "4.0.1"
+version = "4.0.2"
 authors = [
   { name="Scott Griffiths", email="dr.scottgriffiths@gmail.com" },
 ]
 description = "Simple construction, analysis and modification of binary data."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-
 keywords = ["binary", "bitarray", "bitvector"]
 
 [project.urls]
 homepage = "https://github.com/scott-griffiths/bitstring"
-documentation = "https://bitstring.readthedocs.io/"
+documentation = "https://bitstring.readthedocs.io/"
+
+[tool.setuptools]
+packages = ["bitstring"]
```

### Comparing `bitstring-4.0.1/release_notes.txt` & `bitstring-4.0.2/release_notes.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 --------------------------------
 bitstring module version history
 --------------------------------
 
+----------------------------------
+April 2023: version 4.0.2 released
+----------------------------------
+A maintenance release.
+
+* Added py.typed file and converted the module to a package to let mypy find type
+  annotations. Bug 248.
+* Fix to shifting operations when using LSB0 mode. Bug 251.
+* A few more fixes for LSB0 mode.
+* Improved LSB0 documentation.
+* Added build-system section to pyproject.toml. Bug 243.
+* Rewrote the walkthrough documentation as a jupyter notebook.
+* Updated the project's logo.
+
 -------------------------------------
 November 2022: version 4.0.1 released
 -------------------------------------
 
 This is a major release which drops support for Python 2.7 and has a new minimum
 requirement of Python 3.7. Around 95% of downloads satisfy this - users of
 older versions can continue to use bitstring 3.1, which will still be supported
```

### Comparing `bitstring-4.0.1/tests/test.m1v` & `bitstring-4.0.2/tests/test.m1v`

 * *Files identical despite different names*

