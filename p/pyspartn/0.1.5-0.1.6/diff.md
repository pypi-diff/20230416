# Comparing `tmp/pyspartn-0.1.5.tar.gz` & `tmp/pyspartn-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspartn-0.1.5.tar", last modified: Thu Apr 13 08:00:53 2023, max compression
+gzip compressed data, was "pyspartn-0.1.6.tar", last modified: Sun Apr 16 08:50:16 2023, max compression
```

## Comparing `pyspartn-0.1.5.tar` & `pyspartn-0.1.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-13 08:00:53.161810 pyspartn-0.1.5/
--rw-r--r--   0 steve      (501) staff       (20)     1613 2023-03-28 07:19:43.000000 pyspartn-0.1.5/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)       64 2023-03-28 07:19:43.000000 pyspartn-0.1.5/MANIFEST.in
--rw-r--r--   0 steve      (501) staff       (20)    14144 2023-04-13 08:00:53.161676 pyspartn-0.1.5/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)    11020 2023-03-28 07:19:43.000000 pyspartn-0.1.5/README.md
--rw-r--r--   0 steve      (501) staff       (20)     2292 2023-04-13 07:59:47.000000 pyspartn-0.1.5/pyproject.toml
--rw-r--r--   0 steve      (501) staff       (20)       38 2023-04-13 08:00:53.161843 pyspartn-0.1.5/setup.cfg
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-13 08:00:53.158642 pyspartn-0.1.5/src/
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-13 08:00:53.160422 pyspartn-0.1.5/src/pyspartn/
--rw-r--r--   0 steve      (501) staff       (20)      600 2023-03-28 07:19:43.000000 pyspartn-0.1.5/src/pyspartn/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      162 2023-04-13 07:54:16.000000 pyspartn-0.1.5/src/pyspartn/_version.py
--rw-r--r--   0 steve      (501) staff       (20)      671 2023-03-28 07:19:43.000000 pyspartn-0.1.5/src/pyspartn/exceptions.py
--rw-r--r--   0 steve      (501) staff       (20)     2465 2023-03-28 07:19:43.000000 pyspartn-0.1.5/src/pyspartn/socket_stream.py
--rw-r--r--   0 steve      (501) staff       (20)     6051 2023-03-28 07:19:43.000000 pyspartn-0.1.5/src/pyspartn/spartnhelpers.py
--rw-r--r--   0 steve      (501) staff       (20)    17631 2023-04-13 07:54:16.000000 pyspartn-0.1.5/src/pyspartn/spartnmessage.py
--rw-r--r--   0 steve      (501) staff       (20)     9161 2023-04-13 07:54:16.000000 pyspartn-0.1.5/src/pyspartn/spartnreader.py
--rw-r--r--   0 steve      (501) staff       (20)      222 2023-03-28 07:19:43.000000 pyspartn-0.1.5/src/pyspartn/spartntables.py
--rw-r--r--   0 steve      (501) staff       (20)     8642 2023-04-13 07:54:16.000000 pyspartn-0.1.5/src/pyspartn/spartntypes_core.py
--rw-r--r--   0 steve      (501) staff       (20)    18776 2023-04-13 07:54:16.000000 pyspartn-0.1.5/src/pyspartn/spartntypes_get.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-13 08:00:53.161111 pyspartn-0.1.5/src/pyspartn.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)    14144 2023-04-13 08:00:53.000000 pyspartn-0.1.5/src/pyspartn.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      576 2023-04-13 08:00:53.000000 pyspartn-0.1.5/src/pyspartn.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2023-04-13 08:00:53.000000 pyspartn-0.1.5/src/pyspartn.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)      120 2023-04-13 08:00:53.000000 pyspartn-0.1.5/src/pyspartn.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)        9 2023-04-13 08:00:53.000000 pyspartn-0.1.5/src/pyspartn.egg-info/top_level.txt
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-13 08:00:53.161462 pyspartn-0.1.5/tests/
--rw-r--r--   0 steve      (501) staff       (20)     4043 2023-03-28 07:19:43.000000 pyspartn-0.1.5/tests/test_socket.py
--rw-r--r--   0 steve      (501) staff       (20)     5437 2023-03-28 07:19:43.000000 pyspartn-0.1.5/tests/test_static.py
--rw-r--r--   0 steve      (501) staff       (20)    54361 2023-04-13 07:54:16.000000 pyspartn-0.1.5/tests/test_stream.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 08:50:16.872215 pyspartn-0.1.6/
+-rw-r--r--   0 steve      (501) staff       (20)     1613 2023-03-28 07:19:43.000000 pyspartn-0.1.6/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)       64 2023-03-28 07:19:43.000000 pyspartn-0.1.6/MANIFEST.in
+-rw-r--r--   0 steve      (501) staff       (20)    14408 2023-04-16 08:50:16.872049 pyspartn-0.1.6/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)    11288 2023-04-16 08:49:28.000000 pyspartn-0.1.6/README.md
+-rw-r--r--   0 steve      (501) staff       (20)     2292 2023-04-16 08:49:28.000000 pyspartn-0.1.6/pyproject.toml
+-rw-r--r--   0 steve      (501) staff       (20)       38 2023-04-16 08:50:16.872260 pyspartn-0.1.6/setup.cfg
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 08:50:16.868595 pyspartn-0.1.6/src/
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 08:50:16.870468 pyspartn-0.1.6/src/pyspartn/
+-rw-r--r--   0 steve      (501) staff       (20)      600 2023-03-28 07:19:43.000000 pyspartn-0.1.6/src/pyspartn/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      162 2023-04-16 08:49:28.000000 pyspartn-0.1.6/src/pyspartn/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)      671 2023-03-28 07:19:43.000000 pyspartn-0.1.6/src/pyspartn/exceptions.py
+-rw-r--r--   0 steve      (501) staff       (20)     2465 2023-03-28 07:19:43.000000 pyspartn-0.1.6/src/pyspartn/socket_stream.py
+-rw-r--r--   0 steve      (501) staff       (20)     6594 2023-04-16 08:49:28.000000 pyspartn-0.1.6/src/pyspartn/spartnhelpers.py
+-rw-r--r--   0 steve      (501) staff       (20)    17675 2023-04-16 08:49:28.000000 pyspartn-0.1.6/src/pyspartn/spartnmessage.py
+-rw-r--r--   0 steve      (501) staff       (20)     9161 2023-04-13 12:24:53.000000 pyspartn-0.1.6/src/pyspartn/spartnreader.py
+-rw-r--r--   0 steve      (501) staff       (20)      222 2023-03-28 07:19:43.000000 pyspartn-0.1.6/src/pyspartn/spartntables.py
+-rw-r--r--   0 steve      (501) staff       (20)     8642 2023-04-13 07:54:16.000000 pyspartn-0.1.6/src/pyspartn/spartntypes_core.py
+-rw-r--r--   0 steve      (501) staff       (20)    18776 2023-04-13 11:21:41.000000 pyspartn-0.1.6/src/pyspartn/spartntypes_get.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 08:50:16.871188 pyspartn-0.1.6/src/pyspartn.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)    14408 2023-04-16 08:50:16.000000 pyspartn-0.1.6/src/pyspartn.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      576 2023-04-16 08:50:16.000000 pyspartn-0.1.6/src/pyspartn.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2023-04-16 08:50:16.000000 pyspartn-0.1.6/src/pyspartn.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)      120 2023-04-16 08:50:16.000000 pyspartn-0.1.6/src/pyspartn.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)        9 2023-04-16 08:50:16.000000 pyspartn-0.1.6/src/pyspartn.egg-info/top_level.txt
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 08:50:16.871789 pyspartn-0.1.6/tests/
+-rw-r--r--   0 steve      (501) staff       (20)     4043 2023-03-28 07:19:43.000000 pyspartn-0.1.6/tests/test_socket.py
+-rw-r--r--   0 steve      (501) staff       (20)     6054 2023-04-16 08:49:28.000000 pyspartn-0.1.6/tests/test_static.py
+-rw-r--r--   0 steve      (501) staff       (20)    28728 2023-04-16 08:49:28.000000 pyspartn-0.1.6/tests/test_stream.py
```

### Comparing `pyspartn-0.1.5/LICENSE` & `pyspartn-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.5/PKG-INFO` & `pyspartn-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspartn
-Version: 0.1.5
+Version: 0.1.6
 Summary: SPARTN protocol parser
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2023, SEMU Consulting
         All rights reserved.
@@ -94,22 +94,19 @@
 ![Build](https://img.shields.io/github/actions/workflow/status/semuconsulting/pyspartn/main.yml?branch=main)
 ![Codecov](https://img.shields.io/codecov/c/github/semuconsulting/pyspartn)
 ![Release Date](https://img.shields.io/github/release-date-pre/semuconsulting/pyspartn)
 ![Last Commit](https://img.shields.io/github/last-commit/semuconsulting/pyspartn)
 ![Contributors](https://img.shields.io/github/contributors/semuconsulting/pyspartn.svg)
 ![Open Issues](https://img.shields.io/github/issues-raw/semuconsulting/pyspartn)
 
-The `SPARTNReader` class is fully functional and is capable of parsing individual SPARTN transport-layer messages from a binary data stream containing *solely* SPARTN data.
+The `SPARTNReader` class is fully functional and is capable of parsing individual SPARTN transport-layer messages from a binary data stream containing *solely* SPARTN data, with their associated metadata (message type/subtype, payload length, encryption parameters, etc.).
 
-The `SPARTNMessage` class does not currently perform a full decrypt and decode of SPARTN payloads; it decodes the transport layer to identify message type/subtype, payload length and other key metadata. Full payload decode will be added in due course as and when voluntary development time permits - contributions welcome!
-
-**NB:** Decryption of SPARTN payloads requires a 128-bit AES Initialisation Vector (IV) derived from various fields in the message's transport layer. This in turn requires a `gnssTimeTag` value in 32-bit format (representing total seconds from the SPARTN time origin of 2010-01-01 00:00:00). If `timeTagtype = 1`, this can be derived directly from the message's transport layer. If `timeTagtype = 0`, however, it is necessary to convert an ambiguous 16-bit (half-days) timetag to 32-bit format. The [SPARTN 2.01 protocol specification](https://www.spartnformat.org/download/) provides *no details* on how to do this, but it appears to be necessary to use the 32-bit timetag or GPS Timestamp from an external concurrent SPARTN or UBX message from the same data source and stream. In other words, it appears SPARTN messages with `timeTagtype = 0` *cannot* be reliably decrypted in isolation.
-
-See https://portal.u-blox.com/s/question/0D52p0000CimfsOCQQ/spartn-initialization-vector-iv-details for discussion.
+The `SPARTNMessage` class implements a provisional decrypt and decode for OCB, HPAC and GAD message types but it has not yet been fully tested (*appears to be working OK for HPAC messages*).
 
+There are some additional complexities for messages where `timeTagtype` = 0. See https://portal.u-blox.com/s/question/0D52p0000CimfsOCQQ/spartn-initialization-vector-iv-details for discussion.
 
 Sphinx API Documentation in HTML format is available at [https://www.semuconsulting.com/pyspartn](https://www.semuconsulting.com/pyspartn).
 
 Contributions welcome - please refer to [CONTRIBUTING.MD](https://github.com/semuconsulting/pyspartn/blob/master/CONTRIBUTING.md).
 
 [Bug reports](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided.
 
@@ -150,15 +147,15 @@
 class pyspartn.spartnreader.SPARTNReader(stream, **kwargs)
 ```
 
 You can create a `SPARTNReader` object by calling the constructor with an active stream object. 
 The stream object can be any data stream which supports a `read(n) -> bytes` method (e.g. File or Serial, with 
 or without a buffer wrapper). `pyspartn` implements an internal `SocketStream` class to allow sockets to be read in the same way as other streams (see example below).
 
-Individual SPARTN messages can then be read using the `SPARTNReader.read()` function, which returns both the raw binary data (as bytes) and the parsed data (as a `SPARTNMMessage`, via the `parse()` method). The function is thread-safe in so far as the incoming data stream object is thread-safe. `SPARTNReader` also implements an iterator.
+Individual SPARTN messages can then be read using the `SPARTNReader.read()` function, which returns both the raw binary data (as bytes) and the parsed data (as a `SPARTNMessage`, via the `parse()` method). The function is thread-safe in so far as the incoming data stream object is thread-safe. `SPARTNReader` also implements an iterator.
 
 Example -  Serial input:
 ```python
 >>> from serial import Serial
 >>> from pyspartn import SPARTNReader
 >>> stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
 >>>spr = SPARTNReader(stream)
@@ -185,35 +182,42 @@
 >>> spr = SPARTNReader(stream)
 >>> for (raw_data, parsed_data) in spr: print(parsed_data)
 ```
 
 ---
 ## <a name="parsing">Parsing</a>
 
-You can parse individual SPARTN messages using the static `SPARTNReader.parse(data)` function, which takes a bytes array containing a binary SPARTN message and returns a `SPARTNMessage` object.
+You can parse individual SPARTN messages using the static `SPARTNReader.parse(data)` function, which takes a bytes array containing a binary SPARTN message and returns a `SPARTNMessage` object. The optional `decode` keyword argument signifies whether to decrypt and decode the full payload (default = `False`). If `decode` is set to `True` and the message is encrypted (`eaf=1`), the decryption key must be provided via the `key` keyword argument - see example below.
 
 **NB:** Once instantiated, a `SPARTNMMessage` object is immutable.
 
-Example:
+Examples:
+
 ```python
 >>> from pyspartn import SPARTNReader
->>> msg = SPARTNReader.parse(b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad")
+>>> msg = SPARTNReader.parse(b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad", decode=False)
 >>> print(msg)
 <SPARTN(SPARTN-1X-OCB-GPS, msgType=0, msgSubtype=0, nData=37, eaf=1, crcType=2, frameCrc=2, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11)>
 ```
 
-The `SPARTNMessage` object exposes different public attributes depending on its message type or 'identity':
+The `SPARTNMessage` object exposes different public attributes depending on its message type or 'identity'. SPARTN data fields are denoted `SFnnn` - use the `datadesc()` helper method to obtain a more user-friendly text description of the data field.
 
 ```python
+>>> from pyspartn import SPARTNReader, datadesc
+>>> msg = SPARTNReader.parse(b'\x73\x03\x35\xec\x08\xc7\xd4\x20\x70\x5b\x1f\xc ... \x1e\xbe\x18\x43\x2d\x57\xe7\xa7', decode=True, key="00112233445566778899aabbccddeeff")
 >>> print(msg)
-<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, msgSubtype=0, nData=37, eaf=1, crcType=2, frameCrc=2, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11)>
+<SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=619, eaf=1, crcType=2, frameCrc=12, msgSubtype=0, timeTagtype=1, gnssTimeTag=419070990, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=63, authInd=1, embAuthLen=0, crc=5760935, SF005=508, SF068=1, SF069=0, SF030=9, SF031_01=0, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=2, SF043_01=127, SF044_01=1, SF048_01=213, SF049a_01=257, SF049b_01=253, SF054_01=1, SatBitmaskLen_01=0, SF011_01=70263185, SF055_01_01=6, SF056_01_01=1, SF060_01_01=8944, ... SF061b_09_08=8287)>
 >>> msg.identity
-'SPARTN-1X-OCB-GPS'
+'SPARTN-1X-HPAC-GPS'
 >>> msg.gnssTimeTag
-3970
+419070990
+>>> msg.SF005
+508
+datadesc("SF005")
+'Solution issue of update (SIOU)'
 ```
 
 The `payload` attribute always contains the raw payload as bytes.
 
 ---
 ## <a name="generating">Generating</a>
```

### Comparing `pyspartn-0.1.5/README.md` & `pyspartn-0.1.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -33,22 +33,19 @@
 ![Build](https://img.shields.io/github/actions/workflow/status/semuconsulting/pyspartn/main.yml?branch=main)
 ![Codecov](https://img.shields.io/codecov/c/github/semuconsulting/pyspartn)
 ![Release Date](https://img.shields.io/github/release-date-pre/semuconsulting/pyspartn)
 ![Last Commit](https://img.shields.io/github/last-commit/semuconsulting/pyspartn)
 ![Contributors](https://img.shields.io/github/contributors/semuconsulting/pyspartn.svg)
 ![Open Issues](https://img.shields.io/github/issues-raw/semuconsulting/pyspartn)
 
-The `SPARTNReader` class is fully functional and is capable of parsing individual SPARTN transport-layer messages from a binary data stream containing *solely* SPARTN data.
+The `SPARTNReader` class is fully functional and is capable of parsing individual SPARTN transport-layer messages from a binary data stream containing *solely* SPARTN data, with their associated metadata (message type/subtype, payload length, encryption parameters, etc.).
 
-The `SPARTNMessage` class does not currently perform a full decrypt and decode of SPARTN payloads; it decodes the transport layer to identify message type/subtype, payload length and other key metadata. Full payload decode will be added in due course as and when voluntary development time permits - contributions welcome!
-
-**NB:** Decryption of SPARTN payloads requires a 128-bit AES Initialisation Vector (IV) derived from various fields in the message's transport layer. This in turn requires a `gnssTimeTag` value in 32-bit format (representing total seconds from the SPARTN time origin of 2010-01-01 00:00:00). If `timeTagtype = 1`, this can be derived directly from the message's transport layer. If `timeTagtype = 0`, however, it is necessary to convert an ambiguous 16-bit (half-days) timetag to 32-bit format. The [SPARTN 2.01 protocol specification](https://www.spartnformat.org/download/) provides *no details* on how to do this, but it appears to be necessary to use the 32-bit timetag or GPS Timestamp from an external concurrent SPARTN or UBX message from the same data source and stream. In other words, it appears SPARTN messages with `timeTagtype = 0` *cannot* be reliably decrypted in isolation.
-
-See https://portal.u-blox.com/s/question/0D52p0000CimfsOCQQ/spartn-initialization-vector-iv-details for discussion.
+The `SPARTNMessage` class implements a provisional decrypt and decode for OCB, HPAC and GAD message types but it has not yet been fully tested (*appears to be working OK for HPAC messages*).
 
+There are some additional complexities for messages where `timeTagtype` = 0. See https://portal.u-blox.com/s/question/0D52p0000CimfsOCQQ/spartn-initialization-vector-iv-details for discussion.
 
 Sphinx API Documentation in HTML format is available at [https://www.semuconsulting.com/pyspartn](https://www.semuconsulting.com/pyspartn).
 
 Contributions welcome - please refer to [CONTRIBUTING.MD](https://github.com/semuconsulting/pyspartn/blob/master/CONTRIBUTING.md).
 
 [Bug reports](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided.
 
@@ -89,15 +86,15 @@
 class pyspartn.spartnreader.SPARTNReader(stream, **kwargs)
 ```
 
 You can create a `SPARTNReader` object by calling the constructor with an active stream object. 
 The stream object can be any data stream which supports a `read(n) -> bytes` method (e.g. File or Serial, with 
 or without a buffer wrapper). `pyspartn` implements an internal `SocketStream` class to allow sockets to be read in the same way as other streams (see example below).
 
-Individual SPARTN messages can then be read using the `SPARTNReader.read()` function, which returns both the raw binary data (as bytes) and the parsed data (as a `SPARTNMMessage`, via the `parse()` method). The function is thread-safe in so far as the incoming data stream object is thread-safe. `SPARTNReader` also implements an iterator.
+Individual SPARTN messages can then be read using the `SPARTNReader.read()` function, which returns both the raw binary data (as bytes) and the parsed data (as a `SPARTNMessage`, via the `parse()` method). The function is thread-safe in so far as the incoming data stream object is thread-safe. `SPARTNReader` also implements an iterator.
 
 Example -  Serial input:
 ```python
 >>> from serial import Serial
 >>> from pyspartn import SPARTNReader
 >>> stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
 >>>spr = SPARTNReader(stream)
@@ -124,35 +121,42 @@
 >>> spr = SPARTNReader(stream)
 >>> for (raw_data, parsed_data) in spr: print(parsed_data)
 ```
 
 ---
 ## <a name="parsing">Parsing</a>
 
-You can parse individual SPARTN messages using the static `SPARTNReader.parse(data)` function, which takes a bytes array containing a binary SPARTN message and returns a `SPARTNMessage` object.
+You can parse individual SPARTN messages using the static `SPARTNReader.parse(data)` function, which takes a bytes array containing a binary SPARTN message and returns a `SPARTNMessage` object. The optional `decode` keyword argument signifies whether to decrypt and decode the full payload (default = `False`). If `decode` is set to `True` and the message is encrypted (`eaf=1`), the decryption key must be provided via the `key` keyword argument - see example below.
 
 **NB:** Once instantiated, a `SPARTNMMessage` object is immutable.
 
-Example:
+Examples:
+
 ```python
 >>> from pyspartn import SPARTNReader
->>> msg = SPARTNReader.parse(b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad")
+>>> msg = SPARTNReader.parse(b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad", decode=False)
 >>> print(msg)
 <SPARTN(SPARTN-1X-OCB-GPS, msgType=0, msgSubtype=0, nData=37, eaf=1, crcType=2, frameCrc=2, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11)>
 ```
 
-The `SPARTNMessage` object exposes different public attributes depending on its message type or 'identity':
+The `SPARTNMessage` object exposes different public attributes depending on its message type or 'identity'. SPARTN data fields are denoted `SFnnn` - use the `datadesc()` helper method to obtain a more user-friendly text description of the data field.
 
 ```python
+>>> from pyspartn import SPARTNReader, datadesc
+>>> msg = SPARTNReader.parse(b'\x73\x03\x35\xec\x08\xc7\xd4\x20\x70\x5b\x1f\xc ... \x1e\xbe\x18\x43\x2d\x57\xe7\xa7', decode=True, key="00112233445566778899aabbccddeeff")
 >>> print(msg)
-<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, msgSubtype=0, nData=37, eaf=1, crcType=2, frameCrc=2, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11)>
+<SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=619, eaf=1, crcType=2, frameCrc=12, msgSubtype=0, timeTagtype=1, gnssTimeTag=419070990, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=63, authInd=1, embAuthLen=0, crc=5760935, SF005=508, SF068=1, SF069=0, SF030=9, SF031_01=0, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=2, SF043_01=127, SF044_01=1, SF048_01=213, SF049a_01=257, SF049b_01=253, SF054_01=1, SatBitmaskLen_01=0, SF011_01=70263185, SF055_01_01=6, SF056_01_01=1, SF060_01_01=8944, ... SF061b_09_08=8287)>
 >>> msg.identity
-'SPARTN-1X-OCB-GPS'
+'SPARTN-1X-HPAC-GPS'
 >>> msg.gnssTimeTag
-3970
+419070990
+>>> msg.SF005
+508
+datadesc("SF005")
+'Solution issue of update (SIOU)'
 ```
 
 The `payload` attribute always contains the raw payload as bytes.
 
 ---
 ## <a name="generating">Generating</a>
```

### Comparing `pyspartn-0.1.5/pyproject.toml` & `pyspartn-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = [
     {name = "semuadmin", email = "semuadmin@semuconsulting.com"},
 ]
 maintainers = [
   {name = "semuadmin", email = "semuadmin@semuconsulting.com"}
 ]
 description = "SPARTN protocol parser"
-version = "0.1.5"
+version = "0.1.6"
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Operating System :: OS Independent",
     "Development Status :: 2 - Pre-Alpha",
     "Environment :: MacOS X",
@@ -74,12 +74,12 @@
     useless-suppression,
     deprecated-pragma,
     use-symbolic-message-instead,
 """
 
 [tool.pytest.ini_options]
 minversion = "7.0"
-addopts = "--cov --cov-report term-missing --cov-fail-under 60"
+addopts = "--cov --cov-report term-missing --cov-fail-under 80"
 pythonpath = ["src"]
 
 [tool.coverage.run]
 source = ["src"]
```

### Comparing `pyspartn-0.1.5/src/pyspartn/__init__.py` & `pyspartn-0.1.6/src/pyspartn/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.5/src/pyspartn/exceptions.py` & `pyspartn-0.1.6/src/pyspartn/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.5/src/pyspartn/socket_stream.py` & `pyspartn-0.1.6/src/pyspartn/socket_stream.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.5/src/pyspartn/spartnhelpers.py` & `pyspartn-0.1.6/src/pyspartn/spartnhelpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 :copyright: SEMU Consulting © 2023
 :license: BSD 3-Clause
 """
 # pylint: disable=invalid-name
 
 from datetime import datetime
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
-from pyspartn.spartntypes_core import TIMEBASE
+from pyspartn.spartntypes_core import TIMEBASE, SPARTN_DATA_FIELDS
+from pyspartn.exceptions import SPARTNMessageError
 
 
 def att2idx(att: str) -> int:
     """
     Get integer index corresponding to grouped attribute.
     e.g. SF019_04 -> 4; SF019_23 -> 23
 
@@ -45,26 +46,29 @@
         return att[: att.rindex("_")]
     except ValueError:
         return att
 
 
 def bitsval(bitfield: bytes, position: int, length: int) -> int:
     """
-    Get unisgned integer value of masked bits in bitfield.
+    Get unisgned integer value of masked bits in bytes.
 
     :param bytes bitfield: bytes
     :param int position: position in bitfield, from leftmost bit
     :param int length: length of masked bits
     :return: value
     :rtype: int
+    :raises: SPARTNMessageError if end of bitfield
     """
 
     lbb = len(bitfield) * 8
     if position + length > lbb:
-        return None
+        raise SPARTNMessageError(
+            f"Attribute size {length} exceeds remaining payload length {lbb - position}"
+        )
 
     return (
         int.from_bytes(bitfield, "big") >> (lbb - position - length) & 2**length - 1
     )
 
 
 def numbitsset(val: int) -> int:
@@ -219,7 +223,20 @@
     if timetag32 is None:
         time32 = (datetime.now() - TIMEBASE).total_seconds()
     else:
         time32 = timetag32
     basis32 = time32 - (time32 % 43200)
     timetag32 = timetag16 + basis32
     return int(timetag32)
+
+
+def datadesc(datafield: str) -> str:
+    """
+    Get description of data field.
+
+    :param str datafield: datafield e.g. 'SF054'
+    :return: datafield description e.g. "Ionosphere equation type"
+    :rtype: str
+    """
+
+    (_, _, desc) = SPARTN_DATA_FIELDS[datafield[0:5]]
+    return desc
```

### Comparing `pyspartn-0.1.5/src/pyspartn/spartnmessage.py` & `pyspartn-0.1.6/src/pyspartn/spartnmessage.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,17 +150,17 @@
 
         offset = 0  # payload offset in bits
         index = []  # array of (nested) group indices
 
         # decrypt payload if encrypted
         if self.eaf and self._decode:
             iv = self._get_iv()
-            self.payload = decrypt(payload, self._key, iv)
+            self._payload = decrypt(payload, self._key, iv)
         else:
-            self.payload = payload
+            self._payload = payload
 
         key = ""
         try:
             if self._decode:
                 pdict = (
                     self._get_dict()
                 )  # get payload definition dict for this message identity
@@ -215,30 +215,28 @@
         """
 
         keyr = key
         keyl = NESTED_DEPTH[key]
         for i in range(keyl + 1):
             n = index[i]
             keyr += f"_{n:02d}"
-        # print(f"DEBUG _set_attribute_group nested depth {key} {keyl} {keyr}")
         return keyr
 
     def _set_attribute(self, offset: int, pdict: dict, key: str, index: list) -> tuple:
         """
         Recursive routine to set individual, optional or grouped payload attributes.
 
         :param int offset: payload offset in bits
         :param dict pdict: dict representing payload definition
         :param str key: attribute keyword
         :param list index: repeating group index array
         :return: (offset, index[])
         :rtype: tuple
         """
 
-        # print(f"DEBUG set_attribute {self} index {index} key {key}")
         att = pdict[key]  # get attribute type
         if isinstance(att, tuple):  # attribute group
             siz, _ = att
             if isinstance(siz, tuple):  # conditional group of attributes
                 (offset, index) = self._set_attribute_optional(att, offset, index)
             else:  # repeating group of attributes
                 (offset, index) = self._set_attribute_group(att, offset, index)
@@ -348,15 +346,15 @@
         # get value of required number of bits at current payload offset
         # (attribute length, resolution, description)
         attlen, res, _ = SPARTN_DATA_FIELDS[key]
         if isinstance(attlen, str):  # variable length attribute
             attlen = self._getvarlen(key, index)
         if not self._scaling:
             res = 0
-        val = bitsval(self.payload, offset, attlen)
+        val = bitsval(self._payload, offset, attlen)
 
         setattr(self, keyr, val)
 
         offset += attlen
 
         return offset
 
@@ -380,15 +378,15 @@
         value of preceeding bits.
 
         :param str keyr: name of attribute
         :param list index: nested group index
         :return: length of attribute in bits
         :rtype: int
         """
-        # pylint: disable=no-member
+        # pylint: disable=no-member, too-many-branches
 
         # if within repeating group, append nested index
         if len(index) > 0:
             sfx = f"_{index[-1]:02d}"
         else:
             sfx = ""
         attl = 0
@@ -512,7 +510,18 @@
         Return message identity.
 
         :return: message identity e.g. "SPARTN_1X_OCB_GPS"
         :rtype: str
         """
 
         return SPARTN_MSGIDS.get((self.msgType, self.msgSubtype), "UNKNOWN")
+
+    @property
+    def payload(self) -> bytes:
+        """
+        Return payload.
+
+        :return: payload
+        :rtype: bytes
+        """
+
+        return self._payload
```

### Comparing `pyspartn-0.1.5/src/pyspartn/spartnreader.py` & `pyspartn-0.1.6/src/pyspartn/spartnreader.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.5/src/pyspartn/spartntypes_core.py` & `pyspartn-0.1.6/src/pyspartn/spartntypes_core.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.5/src/pyspartn/spartntypes_get.py` & `pyspartn-0.1.6/src/pyspartn/spartntypes_get.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.5/src/pyspartn.egg-info/PKG-INFO` & `pyspartn-0.1.6/src/pyspartn.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspartn
-Version: 0.1.5
+Version: 0.1.6
 Summary: SPARTN protocol parser
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2023, SEMU Consulting
         All rights reserved.
@@ -94,22 +94,19 @@
 ![Build](https://img.shields.io/github/actions/workflow/status/semuconsulting/pyspartn/main.yml?branch=main)
 ![Codecov](https://img.shields.io/codecov/c/github/semuconsulting/pyspartn)
 ![Release Date](https://img.shields.io/github/release-date-pre/semuconsulting/pyspartn)
 ![Last Commit](https://img.shields.io/github/last-commit/semuconsulting/pyspartn)
 ![Contributors](https://img.shields.io/github/contributors/semuconsulting/pyspartn.svg)
 ![Open Issues](https://img.shields.io/github/issues-raw/semuconsulting/pyspartn)
 
-The `SPARTNReader` class is fully functional and is capable of parsing individual SPARTN transport-layer messages from a binary data stream containing *solely* SPARTN data.
+The `SPARTNReader` class is fully functional and is capable of parsing individual SPARTN transport-layer messages from a binary data stream containing *solely* SPARTN data, with their associated metadata (message type/subtype, payload length, encryption parameters, etc.).
 
-The `SPARTNMessage` class does not currently perform a full decrypt and decode of SPARTN payloads; it decodes the transport layer to identify message type/subtype, payload length and other key metadata. Full payload decode will be added in due course as and when voluntary development time permits - contributions welcome!
-
-**NB:** Decryption of SPARTN payloads requires a 128-bit AES Initialisation Vector (IV) derived from various fields in the message's transport layer. This in turn requires a `gnssTimeTag` value in 32-bit format (representing total seconds from the SPARTN time origin of 2010-01-01 00:00:00). If `timeTagtype = 1`, this can be derived directly from the message's transport layer. If `timeTagtype = 0`, however, it is necessary to convert an ambiguous 16-bit (half-days) timetag to 32-bit format. The [SPARTN 2.01 protocol specification](https://www.spartnformat.org/download/) provides *no details* on how to do this, but it appears to be necessary to use the 32-bit timetag or GPS Timestamp from an external concurrent SPARTN or UBX message from the same data source and stream. In other words, it appears SPARTN messages with `timeTagtype = 0` *cannot* be reliably decrypted in isolation.
-
-See https://portal.u-blox.com/s/question/0D52p0000CimfsOCQQ/spartn-initialization-vector-iv-details for discussion.
+The `SPARTNMessage` class implements a provisional decrypt and decode for OCB, HPAC and GAD message types but it has not yet been fully tested (*appears to be working OK for HPAC messages*).
 
+There are some additional complexities for messages where `timeTagtype` = 0. See https://portal.u-blox.com/s/question/0D52p0000CimfsOCQQ/spartn-initialization-vector-iv-details for discussion.
 
 Sphinx API Documentation in HTML format is available at [https://www.semuconsulting.com/pyspartn](https://www.semuconsulting.com/pyspartn).
 
 Contributions welcome - please refer to [CONTRIBUTING.MD](https://github.com/semuconsulting/pyspartn/blob/master/CONTRIBUTING.md).
 
 [Bug reports](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided.
 
@@ -150,15 +147,15 @@
 class pyspartn.spartnreader.SPARTNReader(stream, **kwargs)
 ```
 
 You can create a `SPARTNReader` object by calling the constructor with an active stream object. 
 The stream object can be any data stream which supports a `read(n) -> bytes` method (e.g. File or Serial, with 
 or without a buffer wrapper). `pyspartn` implements an internal `SocketStream` class to allow sockets to be read in the same way as other streams (see example below).
 
-Individual SPARTN messages can then be read using the `SPARTNReader.read()` function, which returns both the raw binary data (as bytes) and the parsed data (as a `SPARTNMMessage`, via the `parse()` method). The function is thread-safe in so far as the incoming data stream object is thread-safe. `SPARTNReader` also implements an iterator.
+Individual SPARTN messages can then be read using the `SPARTNReader.read()` function, which returns both the raw binary data (as bytes) and the parsed data (as a `SPARTNMessage`, via the `parse()` method). The function is thread-safe in so far as the incoming data stream object is thread-safe. `SPARTNReader` also implements an iterator.
 
 Example -  Serial input:
 ```python
 >>> from serial import Serial
 >>> from pyspartn import SPARTNReader
 >>> stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
 >>>spr = SPARTNReader(stream)
@@ -185,35 +182,42 @@
 >>> spr = SPARTNReader(stream)
 >>> for (raw_data, parsed_data) in spr: print(parsed_data)
 ```
 
 ---
 ## <a name="parsing">Parsing</a>
 
-You can parse individual SPARTN messages using the static `SPARTNReader.parse(data)` function, which takes a bytes array containing a binary SPARTN message and returns a `SPARTNMessage` object.
+You can parse individual SPARTN messages using the static `SPARTNReader.parse(data)` function, which takes a bytes array containing a binary SPARTN message and returns a `SPARTNMessage` object. The optional `decode` keyword argument signifies whether to decrypt and decode the full payload (default = `False`). If `decode` is set to `True` and the message is encrypted (`eaf=1`), the decryption key must be provided via the `key` keyword argument - see example below.
 
 **NB:** Once instantiated, a `SPARTNMMessage` object is immutable.
 
-Example:
+Examples:
+
 ```python
 >>> from pyspartn import SPARTNReader
->>> msg = SPARTNReader.parse(b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad")
+>>> msg = SPARTNReader.parse(b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad", decode=False)
 >>> print(msg)
 <SPARTN(SPARTN-1X-OCB-GPS, msgType=0, msgSubtype=0, nData=37, eaf=1, crcType=2, frameCrc=2, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11)>
 ```
 
-The `SPARTNMessage` object exposes different public attributes depending on its message type or 'identity':
+The `SPARTNMessage` object exposes different public attributes depending on its message type or 'identity'. SPARTN data fields are denoted `SFnnn` - use the `datadesc()` helper method to obtain a more user-friendly text description of the data field.
 
 ```python
+>>> from pyspartn import SPARTNReader, datadesc
+>>> msg = SPARTNReader.parse(b'\x73\x03\x35\xec\x08\xc7\xd4\x20\x70\x5b\x1f\xc ... \x1e\xbe\x18\x43\x2d\x57\xe7\xa7', decode=True, key="00112233445566778899aabbccddeeff")
 >>> print(msg)
-<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, msgSubtype=0, nData=37, eaf=1, crcType=2, frameCrc=2, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11)>
+<SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=619, eaf=1, crcType=2, frameCrc=12, msgSubtype=0, timeTagtype=1, gnssTimeTag=419070990, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=63, authInd=1, embAuthLen=0, crc=5760935, SF005=508, SF068=1, SF069=0, SF030=9, SF031_01=0, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=2, SF043_01=127, SF044_01=1, SF048_01=213, SF049a_01=257, SF049b_01=253, SF054_01=1, SatBitmaskLen_01=0, SF011_01=70263185, SF055_01_01=6, SF056_01_01=1, SF060_01_01=8944, ... SF061b_09_08=8287)>
 >>> msg.identity
-'SPARTN-1X-OCB-GPS'
+'SPARTN-1X-HPAC-GPS'
 >>> msg.gnssTimeTag
-3970
+419070990
+>>> msg.SF005
+508
+datadesc("SF005")
+'Solution issue of update (SIOU)'
 ```
 
 The `payload` attribute always contains the raw payload as bytes.
 
 ---
 ## <a name="generating">Generating</a>
```

### Comparing `pyspartn-0.1.5/src/pyspartn.egg-info/SOURCES.txt` & `pyspartn-0.1.6/src/pyspartn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.5/tests/test_socket.py` & `pyspartn-0.1.6/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.5/tests/test_static.py` & `pyspartn-0.1.6/tests/test_static.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,35 +18,44 @@
     bitsval,
     valid_crc,
     escapeall,
     encrypt,
     decrypt,
     convert_timetag,
     numbitsset,
+    datadesc,
 )
 from pyspartn.spartntypes_core import TIMEBASE
+from pyspartn.exceptions import SPARTNMessageError
 
 
 class StaticTest(unittest.TestCase):
     def setUp(self):
         self.maxDiff = None
         dirname = os.path.dirname(__file__)
 
     def tearDown(self):
         pass
 
     def testbitsval(self):
-        bits = [(7, 1), (8, 8), (22, 2), (24, 4), (40, 16)]
-        EXPECTED_RESULT = [1, 8, 3, 15, None]
+        bits = [(7, 1), (8, 8), (22, 2), (24, 4)]
+        EXPECTED_RESULT = [1, 8, 3, 15]
 
         bm = b"\x01\x08\x03\xf0\xff"
         for i, (ps, ln) in enumerate(bits):
             res = bitsval(bm, ps, ln)
             self.assertEqual(res, EXPECTED_RESULT[i])
 
+    def testbitsvalerr(self):
+        EXPECTED_ERROR = "Attribute size 16 exceeds remaining payload length 2"
+        bm = b"\x01\x08\x03\xf0\xff"
+        # print(f"Length bitfield = {len(bm) * 8}")
+        with self.assertRaisesRegex(SPARTNMessageError, EXPECTED_ERROR):
+            res = bitsval(bm, 38, 16)
+
     def testnumbitsset(self):
         vals = [7, 8, 22, 24, 4167, 234876]
         EXPECTED_RESULT = [3, 1, 3, 2, 5, 11]
 
         for i, val in enumerate(vals):
             res = numbitsset(val)
             self.assertEqual(res, EXPECTED_RESULT[i])
@@ -156,11 +165,16 @@
         EXPECTED_RESULT = ["svid", "gnssId", "cno", "gmsLon"]
         atts = ["svid_04", "gnssId_16", "cno_101", "gmsLon"]
         for i, att in enumerate(atts):
             res = att2name(att)
             # print(res)
             self.assertEqual(res, EXPECTED_RESULT[i])
 
+    def testdatadesc(self):  # test datadesc
+        res = datadesc("SF054")
+        self.assertEqual(res, "Ionosphere equation type")
+        res = datadesc("SF043_01")
+        self.assertEqual(res, "Area average vertical hydrostatic delay")
 
 if __name__ == "__main__":
     # import sys;sys.argv = ['', 'Test.testName']
     unittest.main()
```

