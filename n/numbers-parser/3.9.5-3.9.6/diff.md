# Comparing `tmp/numbers_parser-3.9.5.tar.gz` & `tmp/numbers_parser-3.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numbers_parser-3.9.5.tar", max compression
+gzip compressed data, was "numbers_parser-3.9.6.tar", max compression
```

## Comparing `numbers_parser-3.9.5.tar` & `numbers_parser-3.9.6.tar`

### file list

```diff
@@ -1,56 +1,55 @@
--rw-r--r--   0        0        0     1050 2022-06-23 17:13:17.000000 numbers_parser-3.9.5/LICENSE.rst
--rw-r--r--   0        0        0    15682 2022-11-20 14:32:10.876841 numbers_parser-3.9.5/README.md
--rw-r--r--   0        0        0     1998 2023-01-15 20:54:02.534909 numbers_parser-3.9.5/pyproject.toml
--rw-r--r--   0        0        0     2021 2023-01-15 19:12:02.043556 numbers_parser-3.9.5/src/numbers_parser/__init__.py
--rw-r--r--   0        0        0     3627 2022-10-30 11:23:27.394347 numbers_parser-3.9.5/src/numbers_parser/_cat_numbers.py
--rw-r--r--   0        0        0     5364 2022-11-20 13:34:31.176334 numbers_parser-3.9.5/src/numbers_parser/_unpack_numbers.py
--rw-r--r--   0        0        0     2616 2022-07-21 08:13:02.000000 numbers_parser-3.9.5/src/numbers_parser/bullets.py
--rw-r--r--   0        0        0    10419 2022-11-19 17:07:46.000000 numbers_parser-3.9.5/src/numbers_parser/cell.py
--rw-r--r--   0        0        0    27190 2022-11-20 14:19:53.651081 numbers_parser-3.9.5/src/numbers_parser/cell_storage.py
--rw-r--r--   0        0        0     1518 2022-11-20 13:23:02.021105 numbers_parser-3.9.5/src/numbers_parser/constants.py
--rw-r--r--   0        0        0     4541 2022-11-19 16:45:32.000000 numbers_parser-3.9.5/src/numbers_parser/containers.py
--rwxr-xr-x   0        0        0   134819 2022-07-21 08:13:02.000000 numbers_parser-3.9.5/src/numbers_parser/data/empty.numbers
--rw-r--r--   0        0        0    15684 2022-12-21 15:02:45.301004 numbers_parser-3.9.5/src/numbers_parser/document.py
--rw-r--r--   0        0        0      663 2022-10-17 17:39:14.019486 numbers_parser-3.9.5/src/numbers_parser/exceptions.py
--rw-r--r--   0        0        0     3807 2022-11-06 09:49:04.857258 numbers_parser-3.9.5/src/numbers_parser/file.py
--rw-r--r--   0        0        0     8908 2022-11-20 14:11:44.897207 numbers_parser-3.9.5/src/numbers_parser/formula.py
--rw-r--r--   0        0        0     6082 2022-10-27 16:53:49.111770 numbers_parser-3.9.5/src/numbers_parser/functionmap.py
--rw-r--r--   0        0        0    15834 2022-10-28 15:05:31.311960 numbers_parser-3.9.5/src/numbers_parser/generated/TNArchives_pb2.py
--rw-r--r--   0        0        0     1215 2022-10-28 15:05:31.312792 numbers_parser-3.9.5/src/numbers_parser/generated/TNArchives_sos_pb2.py
--rw-r--r--   0        0        0    18271 2022-10-28 15:05:31.313777 numbers_parser-3.9.5/src/numbers_parser/generated/TNCommandArchives_pb2.py
--rw-r--r--   0        0        0     1857 2022-10-28 15:05:31.314123 numbers_parser-3.9.5/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py
--rw-r--r--   0        0        0    17112 2022-10-28 15:05:31.314488 numbers_parser-3.9.5/src/numbers_parser/generated/TSAArchives_pb2.py
--rw-r--r--   0        0        0     2033 2022-10-28 15:05:31.314709 numbers_parser-3.9.5/src/numbers_parser/generated/TSAArchives_sos_pb2.py
--rw-r--r--   0        0        0     3907 2022-10-28 15:05:31.315065 numbers_parser-3.9.5/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py
--rw-r--r--   0        0        0    64758 2022-10-28 15:05:31.316694 numbers_parser-3.9.5/src/numbers_parser/generated/TSCEArchives_pb2.py
--rw-r--r--   0        0        0    11162 2022-10-28 15:05:31.317198 numbers_parser-3.9.5/src/numbers_parser/generated/TSCH3DArchives_pb2.py
--rw-r--r--   0        0        0     8655 2022-10-28 15:05:31.317798 numbers_parser-3.9.5/src/numbers_parser/generated/TSCHArchives_Common_pb2.py
--rw-r--r--   0        0        0    44225 2022-10-28 15:05:31.318754 numbers_parser-3.9.5/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py
--rw-r--r--   0        0        0    21748 2022-10-28 15:05:31.319146 numbers_parser-3.9.5/src/numbers_parser/generated/TSCHArchives_pb2.py
--rw-r--r--   0        0        0    62194 2022-10-28 15:05:31.320026 numbers_parser-3.9.5/src/numbers_parser/generated/TSCHArchives_sos_pb2.py
--rw-r--r--   0        0        0    27446 2022-10-28 15:05:31.320498 numbers_parser-3.9.5/src/numbers_parser/generated/TSCHCommandArchives_pb2.py
--rw-r--r--   0        0        0    30051 2022-10-28 15:05:31.320887 numbers_parser-3.9.5/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py
--rw-r--r--   0        0        0    39023 2022-10-28 15:05:31.321415 numbers_parser-3.9.5/src/numbers_parser/generated/TSDArchives_pb2.py
--rw-r--r--   0        0        0     6022 2022-10-28 15:05:31.321645 numbers_parser-3.9.5/src/numbers_parser/generated/TSDArchives_sos_pb2.py
--rw-r--r--   0        0        0    29192 2022-10-28 15:05:31.322062 numbers_parser-3.9.5/src/numbers_parser/generated/TSDCommandArchives_pb2.py
--rw-r--r--   0        0        0    53111 2022-10-28 15:05:31.322747 numbers_parser-3.9.5/src/numbers_parser/generated/TSKArchives_pb2.py
--rw-r--r--   0        0        0     1941 2022-10-28 15:05:31.322986 numbers_parser-3.9.5/src/numbers_parser/generated/TSKArchives_sos_pb2.py
--rw-r--r--   0        0        0    17950 2022-10-28 15:05:31.323544 numbers_parser-3.9.5/src/numbers_parser/generated/TSPArchiveMessages_pb2.py
--rw-r--r--   0        0        0     2024 2022-10-28 15:05:31.324346 numbers_parser-3.9.5/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py
--rw-r--r--   0        0        0    11780 2022-10-28 15:05:31.324724 numbers_parser-3.9.5/src/numbers_parser/generated/TSPMessages_pb2.py
--rw-r--r--   0        0        0     9543 2022-10-28 15:05:31.325086 numbers_parser-3.9.5/src/numbers_parser/generated/TSSArchives_pb2.py
--rw-r--r--   0        0        0     2842 2022-10-28 15:05:31.325441 numbers_parser-3.9.5/src/numbers_parser/generated/TSSArchives_sos_pb2.py
--rw-r--r--   0        0        0    88138 2022-10-28 15:05:31.326390 numbers_parser-3.9.5/src/numbers_parser/generated/TSTArchives_pb2.py
--rw-r--r--   0        0        0    12597 2022-10-28 15:05:31.326802 numbers_parser-3.9.5/src/numbers_parser/generated/TSTArchives_sos_pb2.py
--rw-r--r--   0        0        0    59523 2022-10-28 15:05:31.328559 numbers_parser-3.9.5/src/numbers_parser/generated/TSTCommandArchives_pb2.py
--rw-r--r--   0        0        0    12415 2022-10-28 15:05:31.328963 numbers_parser-3.9.5/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py
--rw-r--r--   0        0        0    54693 2022-10-28 15:05:31.329694 numbers_parser-3.9.5/src/numbers_parser/generated/TSWPArchives_pb2.py
--rw-r--r--   0        0        0    28840 2022-10-28 15:05:31.330420 numbers_parser-3.9.5/src/numbers_parser/generated/TSWPArchives_sos_pb2.py
--rw-r--r--   0        0        0    25441 2022-10-28 15:05:31.330922 numbers_parser-3.9.5/src/numbers_parser/generated/TSWPCommandArchives_pb2.py
--rw-r--r--   0        0        0        0 2022-10-28 15:05:31.335174 numbers_parser-3.9.5/src/numbers_parser/generated/__init__.py
--rw-r--r--   0        0        0    11751 2022-11-19 16:45:01.039682 numbers_parser-3.9.5/src/numbers_parser/iwafile.py
--rw-r--r--   0        0        0    31987 2022-10-30 11:05:25.564931 numbers_parser-3.9.5/src/numbers_parser/mapping.py
--rw-r--r--   0        0        0    54060 2022-12-21 15:03:07.294819 numbers_parser-3.9.5/src/numbers_parser/model.py
--rw-r--r--   0        0        0     2690 2022-11-06 16:05:56.811266 numbers_parser-3.9.5/src/numbers_parser/numbers_uuid.py
--rw-r--r--   0        0        0    17200 1970-01-01 00:00:00.000000 numbers_parser-3.9.5/setup.py
--rw-r--r--   0        0        0    16859 1970-01-01 00:00:00.000000 numbers_parser-3.9.5/PKG-INFO
+-rw-r--r--   0        0        0     1050 2022-06-23 17:13:17.000000 numbers_parser-3.9.6/LICENSE.rst
+-rw-r--r--   0        0        0    15603 2023-04-16 12:31:58.218386 numbers_parser-3.9.6/README.md
+-rw-r--r--   0        0        0     2019 2023-04-16 11:37:58.545418 numbers_parser-3.9.6/pyproject.toml
+-rw-r--r--   0        0        0     2033 2023-04-16 12:36:29.639119 numbers_parser-3.9.6/src/numbers_parser/__init__.py
+-rw-r--r--   0        0        0     3627 2022-10-30 11:23:27.394347 numbers_parser-3.9.6/src/numbers_parser/_cat_numbers.py
+-rw-r--r--   0        0        0     5364 2022-11-20 13:34:31.176334 numbers_parser-3.9.6/src/numbers_parser/_unpack_numbers.py
+-rw-r--r--   0        0        0     2616 2022-07-21 08:13:02.000000 numbers_parser-3.9.6/src/numbers_parser/bullets.py
+-rw-r--r--   0        0        0    10419 2022-11-19 17:07:46.000000 numbers_parser-3.9.6/src/numbers_parser/cell.py
+-rw-r--r--   0        0        0    27190 2022-11-20 14:19:53.651081 numbers_parser-3.9.6/src/numbers_parser/cell_storage.py
+-rw-r--r--   0        0        0     1518 2022-11-20 13:23:02.021105 numbers_parser-3.9.6/src/numbers_parser/constants.py
+-rw-r--r--   0        0        0     4541 2022-11-19 16:45:32.000000 numbers_parser-3.9.6/src/numbers_parser/containers.py
+-rwxr-xr-x   0        0        0   134819 2022-07-21 08:13:02.000000 numbers_parser-3.9.6/src/numbers_parser/data/empty.numbers
+-rw-r--r--   0        0        0    15684 2023-04-16 12:29:24.617353 numbers_parser-3.9.6/src/numbers_parser/document.py
+-rw-r--r--   0        0        0      663 2022-10-17 17:39:14.019486 numbers_parser-3.9.6/src/numbers_parser/exceptions.py
+-rw-r--r--   0        0        0     3807 2022-11-06 09:49:04.857258 numbers_parser-3.9.6/src/numbers_parser/file.py
+-rw-r--r--   0        0        0     8908 2022-11-20 14:11:44.897207 numbers_parser-3.9.6/src/numbers_parser/formula.py
+-rw-r--r--   0        0        0     6082 2023-04-16 11:48:38.802281 numbers_parser-3.9.6/src/numbers_parser/functionmap.py
+-rw-r--r--   0        0        0    15834 2023-04-16 12:18:42.484479 numbers_parser-3.9.6/src/numbers_parser/generated/TNArchives_pb2.py
+-rw-r--r--   0        0        0     1215 2023-04-16 12:18:42.485145 numbers_parser-3.9.6/src/numbers_parser/generated/TNArchives_sos_pb2.py
+-rw-r--r--   0        0        0    18271 2023-04-16 12:18:42.486105 numbers_parser-3.9.6/src/numbers_parser/generated/TNCommandArchives_pb2.py
+-rw-r--r--   0        0        0     1857 2023-04-16 12:18:42.486434 numbers_parser-3.9.6/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py
+-rw-r--r--   0        0        0    17112 2023-04-16 12:18:42.487255 numbers_parser-3.9.6/src/numbers_parser/generated/TSAArchives_pb2.py
+-rw-r--r--   0        0        0     2033 2023-04-16 12:18:28.770572 numbers_parser-3.9.6/src/numbers_parser/generated/TSAArchives_sos_pb2.py
+-rw-r--r--   0        0        0     3907 2023-04-16 12:18:28.771273 numbers_parser-3.9.6/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py
+-rw-r--r--   0        0        0    64758 2023-04-16 12:18:28.772399 numbers_parser-3.9.6/src/numbers_parser/generated/TSCEArchives_pb2.py
+-rw-r--r--   0        0        0    11162 2023-04-16 12:18:28.773082 numbers_parser-3.9.6/src/numbers_parser/generated/TSCH3DArchives_pb2.py
+-rw-r--r--   0        0        0     8655 2023-04-16 12:18:28.773314 numbers_parser-3.9.6/src/numbers_parser/generated/TSCHArchives_Common_pb2.py
+-rw-r--r--   0        0        0    44225 2023-04-16 12:18:28.773624 numbers_parser-3.9.6/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py
+-rw-r--r--   0        0        0    21748 2023-04-16 12:18:28.774422 numbers_parser-3.9.6/src/numbers_parser/generated/TSCHArchives_pb2.py
+-rw-r--r--   0        0        0    62194 2023-04-16 12:18:28.774761 numbers_parser-3.9.6/src/numbers_parser/generated/TSCHArchives_sos_pb2.py
+-rw-r--r--   0        0        0    27446 2023-04-16 12:18:28.774990 numbers_parser-3.9.6/src/numbers_parser/generated/TSCHCommandArchives_pb2.py
+-rw-r--r--   0        0        0    30051 2023-04-16 12:18:28.775455 numbers_parser-3.9.6/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py
+-rw-r--r--   0        0        0    39023 2023-04-16 12:18:28.776119 numbers_parser-3.9.6/src/numbers_parser/generated/TSDArchives_pb2.py
+-rw-r--r--   0        0        0     6022 2023-04-16 12:18:28.776316 numbers_parser-3.9.6/src/numbers_parser/generated/TSDArchives_sos_pb2.py
+-rw-r--r--   0        0        0    29192 2023-04-16 12:18:28.776803 numbers_parser-3.9.6/src/numbers_parser/generated/TSDCommandArchives_pb2.py
+-rw-r--r--   0        0        0    53111 2023-04-16 12:18:28.777475 numbers_parser-3.9.6/src/numbers_parser/generated/TSKArchives_pb2.py
+-rw-r--r--   0        0        0     1941 2023-04-16 12:18:28.777869 numbers_parser-3.9.6/src/numbers_parser/generated/TSKArchives_sos_pb2.py
+-rw-r--r--   0        0        0    17950 2023-04-16 12:18:28.778300 numbers_parser-3.9.6/src/numbers_parser/generated/TSPArchiveMessages_pb2.py
+-rw-r--r--   0        0        0     2024 2023-04-16 12:18:28.778448 numbers_parser-3.9.6/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py
+-rw-r--r--   0        0        0    11780 2023-04-16 12:18:28.778935 numbers_parser-3.9.6/src/numbers_parser/generated/TSPMessages_pb2.py
+-rw-r--r--   0        0        0     9543 2023-04-16 12:18:28.779250 numbers_parser-3.9.6/src/numbers_parser/generated/TSSArchives_pb2.py
+-rw-r--r--   0        0        0     2842 2023-04-16 12:18:28.779605 numbers_parser-3.9.6/src/numbers_parser/generated/TSSArchives_sos_pb2.py
+-rw-r--r--   0        0        0    88138 2023-04-16 12:18:18.612839 numbers_parser-3.9.6/src/numbers_parser/generated/TSTArchives_pb2.py
+-rw-r--r--   0        0        0    12597 2023-04-16 12:18:18.613908 numbers_parser-3.9.6/src/numbers_parser/generated/TSTArchives_sos_pb2.py
+-rw-r--r--   0        0        0    59523 2023-04-16 12:18:18.615150 numbers_parser-3.9.6/src/numbers_parser/generated/TSTCommandArchives_pb2.py
+-rw-r--r--   0        0        0    12415 2023-04-16 12:18:18.615351 numbers_parser-3.9.6/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py
+-rw-r--r--   0        0        0    54693 2023-04-16 12:18:06.523946 numbers_parser-3.9.6/src/numbers_parser/generated/TSWPArchives_pb2.py
+-rw-r--r--   0        0        0    28840 2023-04-16 12:18:09.712539 numbers_parser-3.9.6/src/numbers_parser/generated/TSWPArchives_sos_pb2.py
+-rw-r--r--   0        0        0    25441 2023-04-16 12:18:18.616163 numbers_parser-3.9.6/src/numbers_parser/generated/TSWPCommandArchives_pb2.py
+-rw-r--r--   0        0        0        0 2023-04-16 12:18:50.290394 numbers_parser-3.9.6/src/numbers_parser/generated/__init__.py
+-rw-r--r--   0        0        0    11751 2022-11-19 16:45:01.039682 numbers_parser-3.9.6/src/numbers_parser/iwafile.py
+-rw-r--r--   0        0        0    31987 2022-10-30 11:05:25.564931 numbers_parser-3.9.6/src/numbers_parser/mapping.py
+-rw-r--r--   0        0        0    54055 2023-04-16 11:16:34.696239 numbers_parser-3.9.6/src/numbers_parser/model.py
+-rw-r--r--   0        0        0     2690 2022-11-06 16:05:56.811266 numbers_parser-3.9.6/src/numbers_parser/numbers_uuid.py
+-rw-r--r--   0        0        0    16780 1970-01-01 00:00:00.000000 numbers_parser-3.9.6/PKG-INFO
```

### Comparing `numbers_parser-3.9.5/LICENSE.rst` & `numbers_parser-3.9.6/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/README.md` & `numbers_parser-3.9.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -42,21 +42,27 @@
 And on Apple Silicon:
 
 ``` bash
 brew install snappy python3
 CPPFLAGS="-I/opt/homebrew/include -L/opt/homebrew/lib" python3 -m pip install python-snappy
 ```
 
+On Windows, you will need to either arrange for snappy to be found for VSC++ or you can install python binary libraries compiled by [Christoph Gohlke](https://www.lfd.uci.edu/~gohlke/pythonlibs/#python-snappy). You must select the correct python version for your installation. For example for python 3.11:
+
+``` text
+C:\Users\Jon>pip install C:\Users\Jon\Downloads\python_snappy-0.6.1-cp311-cp311-win_amd64.whl
+```
+
 ## Usage
 
 Reading documents:
 
 ``` python
 from numbers_parser import Document
-doc = Document("my-spreasdsheet.numbers")
+doc = Document("my-spreadsheet.numbers")
 sheets = doc.sheets
 tables = sheets[0].tables
 rows = tables[0].rows()
 ```
 
 ### Referring to sheets and tables
 
@@ -89,15 +95,15 @@
 Cells are objects with a common base class of `Cell`. All cell types have a property `value` which returns the contents of the cell in as a native Python datatype. `DurationCell` object values are `datetime.timedelta` objects which are additionally available as a formatted value matching that stored in the Numbers spreadsheet. The formatted value is returned using the `formatted_value` property.
 
 ### Cell references
 
 In addition to extracting all data at once, individual cells can be referred to as methods
 
 ``` python
-doc = Document("my-spreasdsheet.numbers")
+doc = Document("my-spreadsheet.numbers")
 sheets = doc.sheets
 tables = sheets["Sheet 1"].tables
 table = tables["Table 1"]
 
 # row, column syntax
 print("Cell A1 contains", table.cell(0, 0))
 # Excel/Numbers-style cell references
@@ -108,15 +114,15 @@
 
 When extracting data using ```rows()``` merged cells are ignored since only text values
 are returned. The ```cell()``` method of ```Table``` objects returns a ```Cell``` type
 object which is typed by the type of cell in the Numbers table. ```MergeCell``` objects
 indicates cells removed in a merge.
 
 ``` python
-doc = Document("my-spreasdsheet.numbers")
+doc = Document("my-spreadsheet.numbers")
 sheets = doc.sheets
 tables = sheets["Sheet 1"].tables
 table = tables["Table 1"]
 
 cell = table.cell("A1")
 print(cell.merge_range)
 print(f"Cell A1 merge size is {cell.size[0]},{cell.size[1]})
@@ -307,37 +313,21 @@
 [Protobuf](https://github.com/protocolbuffers/protobuf) `.iwa` files containing
 metadata, text, and all other definitions used in the spreadsheet.
 
 ### Protobuf updates
 
 As `numbers-parser` includes private Protobuf definitions extracted from a copy of Numbers, new versions of Numbers will inevitably create `.numbers` files that cannot be read by `numbers-parser`. As new versions of Numbers are released, running `make bootstrap` will perform all the steps necessary to recreate the protobuf files used `numbers-parser` to read Numbers spreadsheets.
 
-On Apple Silicon Macs, the default protobuf package installation does not include the C++ optimised version which is required by the bootstrapping scripts to extract protobufs. You will receive the following error during build if this is the case:
+The default protobuf package installation may not include the C++ optimised version which is required by the bootstrapping scripts to extract protobufs. You will receive the following error during build if this is the case:
 
  `This script requires the Protobuf installation to use the C++ implementation. Please reinstall Protobuf with C++ support.`
 
  To include the C++ support, download a released version of Google protobuf [from github](https://github.com/protocolbuffers/protobuf). Build instructions are in the [`src/README.md`](https://github.com/protocolbuffers/protobuf/blob/main/src/README.md) in the distribution but for macOS with [Homebrew](https://brew.sh) the two steps are, firstly to install the native protobuf libraries, which must be on your `LD_LIBRARY_PATH`:
 
-``` bash
-brew install autoconf automake libtool
-./autogen.sh
-./configure --prefix=/usr/local
-make check -j`sysctl -n hw.ncpu`
-sudo make install
-```
-
-And then to install the Python libraries with C++ support. If you already have protobuf install via Homebrew, you will need to `brew unlink` the installation.
 
-``` bash
-cd python
-python3 setup.py build --cpp_implementation
-python3 setup.py test --cpp_implementation
-python3 setup.py install --cpp_implementation
-```
-  
   This will install protobuf in a folder above the source installation which can then be used by `make bootstrap` in the `numbers-parser` source tree.
 
 ## Credits
 
 `numbers-parser` was built by [Jon Connell](http://github.com/masaccio) but relies heavily on from [prior work](https://github.com/psobot/keynote-parser) by [Peter Sobot](https://petersobot.com) to read the IWA format archives used by Apple's iWork family of applications, and to regenerate the mapping files required for Python. Both modules are derived from [previous work](https://github.com/obriensp/iWorkFileFormat/blob/master/Docs/index.md) by [Sean Patrick O'Brien](http://www.obriensp.com).
 
 Decoding the data structures inside Numbers files was helped greatly by [Stingray-Reader](https://github.com/slott56/Stingray-Reader) by [Steven Lott](https://github.com/slott56).
```

### Comparing `numbers_parser-3.9.5/pyproject.toml` & `numbers_parser-3.9.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 description = "Read and write Apple Numbers spreadsheets"
 documentation = "https://github.com/masaccio/numbers-parser/blob/main/README.md"
 license = "MIT"
 name = "numbers-parser"
 packages = [{include = "numbers_parser", from = "src"}]
 readme = "README.md"
 repository = "https://github.com/masaccio/numbers-parser"
-version = "3.9.5"
+version = "3.9.6"
 
 [tool.poetry.scripts]
 cat-numbers = "numbers_parser._cat_numbers:main"
 unpack-numbers = "numbers_parser._unpack_numbers:main"
 
 [tool.poetry.dependencies]
 compact-json = "^1.1.3"
@@ -32,14 +32,15 @@
 pylama = "^8.4.1"
 pytest = "^7.2.0"
 pytest-check = "^1.0.10"
 pytest-console-scripts = "^1.3.1"
 pytest-cov = "^4.0.0"
 pytest-profiling = "^1.7.0"
 python-magic = "^0.4.27"
+termcolor = "^2.2.0"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 [tool.coverage.run]
 branch = true
```

### Comparing `numbers_parser-3.9.5/src/numbers_parser/__init__.py` & `numbers_parser-3.9.6/src/numbers_parser/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     "11.0",
     "11.1",
     "11.2",
     "12.0",
     "12.1",
     "12.2",
     "12.2.1",
+    "13.0",
 ]
 
 # Don't print the source line
 old_warn_f = warnings.formatwarning
 warnings.formatwarning = (
     lambda msg, catg, fname, lineno, line=None: old_warn_f(  # pragma: no cover
         msg, catg, fname, lineno, line=""
```

### Comparing `numbers_parser-3.9.5/src/numbers_parser/_cat_numbers.py` & `numbers_parser-3.9.6/src/numbers_parser/_cat_numbers.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/_unpack_numbers.py` & `numbers_parser-3.9.6/src/numbers_parser/_unpack_numbers.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/bullets.py` & `numbers_parser-3.9.6/src/numbers_parser/bullets.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/cell.py` & `numbers_parser-3.9.6/src/numbers_parser/cell.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/cell_storage.py` & `numbers_parser-3.9.6/src/numbers_parser/cell_storage.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/constants.py` & `numbers_parser-3.9.6/src/numbers_parser/constants.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/containers.py` & `numbers_parser-3.9.6/src/numbers_parser/containers.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/data/empty.numbers` & `numbers_parser-3.9.6/src/numbers_parser/data/empty.numbers`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/document.py` & `numbers_parser-3.9.6/src/numbers_parser/document.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/exceptions.py` & `numbers_parser-3.9.6/src/numbers_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/file.py` & `numbers_parser-3.9.6/src/numbers_parser/file.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/formula.py` & `numbers_parser-3.9.6/src/numbers_parser/formula.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/functionmap.py` & `numbers_parser-3.9.6/src/numbers_parser/functionmap.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TNArchives_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TNArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TNArchives_sos_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TNArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TNCommandArchives_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TNCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSAArchives_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSAArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSAArchives_sos_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSAArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSCEArchives_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSCEArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSCH3DArchives_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSCH3DArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSCHArchives_Common_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSCHArchives_Common_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSCHArchives_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSCHArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSCHArchives_sos_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSCHArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSCHCommandArchives_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSCHCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSDArchives_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSDArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSDArchives_sos_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSDArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSDCommandArchives_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSDCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSKArchives_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSKArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSKArchives_sos_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSKArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSPArchiveMessages_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSPArchiveMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSPMessages_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSPMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSSArchives_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSSArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSSArchives_sos_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSSArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSTArchives_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSTArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSTArchives_sos_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSTArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSTCommandArchives_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSTCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSWPArchives_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSWPArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSWPArchives_sos_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSWPArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/generated/TSWPCommandArchives_pb2.py` & `numbers_parser-3.9.6/src/numbers_parser/generated/TSWPCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/iwafile.py` & `numbers_parser-3.9.6/src/numbers_parser/iwafile.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/mapping.py` & `numbers_parser-3.9.6/src/numbers_parser/mapping.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/src/numbers_parser/model.py` & `numbers_parser-3.9.6/src/numbers_parser/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1341,16 +1341,16 @@
         while len(obj) > 0:
             _ = obj.pop()
 
 
 def pack_decimal128(value: float) -> bytearray:
     buffer = bytearray(16)
     exp = math.floor(math.log10(math.e) * math.log(abs(value))) if value != 0.0 else 0
-    exp = int(exp) + 0x1820 - 16
-    mantissa = int(value / math.pow(10, exp - 0x1820))
+    exp += 0x1820 - 16
+    mantissa = abs(int(value / math.pow(10, exp - 0x1820)))
     buffer[15] |= exp >> 7
     buffer[14] |= (exp & 0x7F) << 1
     i = 0
     while mantissa >= 1:
         buffer[i] = mantissa & 0xFF
         i += 1
         mantissa = int(mantissa / 256)
```

### Comparing `numbers_parser-3.9.5/src/numbers_parser/numbers_uuid.py` & `numbers_parser-3.9.6/src/numbers_parser/numbers_uuid.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-3.9.5/setup.py` & `numbers_parser-3.9.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,372 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: numbers-parser
+Version: 3.9.6
+Summary: Read and write Apple Numbers spreadsheets
+Home-page: https://github.com/masaccio/numbers-parser
+License: MIT
+Author: Jon Connell
+Author-email: python@figsandfudge.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Office/Business :: Financial :: Spreadsheet
+Requires-Dist: compact-json (>=1.1.3,<2.0.0)
+Requires-Dist: pendulum (>=2.1.2,<3.0.0)
+Requires-Dist: protobuf (>=4.21.1,<5.0.0)
+Requires-Dist: python-snappy (>=0.6.1,<0.7.0)
+Requires-Dist: regex (>=2022.9.13,<2023.0.0)
+Requires-Dist: roman (>=3.3,<4.0)
+Project-URL: Documentation, https://github.com/masaccio/numbers-parser/blob/main/README.md
+Project-URL: Repository, https://github.com/masaccio/numbers-parser
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# numbers-parser
 
-packages = \
-['numbers_parser', 'numbers_parser.generated']
+[![build:](https://github.com/masaccio/numbers-parser/actions/workflows/run-all-tests.yml/badge.svg)](https://github.com/masaccio/numbers-parser/actions/workflows/run-all-tests.yml)
+[![build:](https://github.com/masaccio/numbers-parser/actions/workflows/codeql.yml/badge.svg)](https://github.com/masaccio/numbers-parser/actions/workflows/codeql.yml)
+[![codecov](https://codecov.io/gh/masaccio/numbers-parser/branch/main/graph/badge.svg?token=EKIUFGT05E)](https://codecov.io/gh/masaccio/numbers-parser)
 
-package_data = \
-{'': ['*'], 'numbers_parser': ['data/*']}
-
-install_requires = \
-['compact-json>=1.1.3,<2.0.0',
- 'pendulum>=2.1.2,<3.0.0',
- 'protobuf>=4.21.1,<5.0.0',
- 'python-snappy>=0.6.1,<0.7.0',
- 'regex>=2022.9.13,<2023.0.0',
- 'roman>=3.3,<4.0']
-
-entry_points = \
-{'console_scripts': ['cat-numbers = numbers_parser._cat_numbers:main',
-                     'unpack-numbers = numbers_parser._unpack_numbers:main']}
-
-setup_kwargs = {
-    'name': 'numbers-parser',
-    'version': '3.9.5',
-    'description': 'Read and write Apple Numbers spreadsheets',
-    'long_description': '# numbers-parser\n\n[![build:](https://github.com/masaccio/numbers-parser/actions/workflows/run-all-tests.yml/badge.svg)](https://github.com/masaccio/numbers-parser/actions/workflows/run-all-tests.yml)\n[![build:](https://github.com/masaccio/numbers-parser/actions/workflows/codeql.yml/badge.svg)](https://github.com/masaccio/numbers-parser/actions/workflows/codeql.yml)\n[![codecov](https://codecov.io/gh/masaccio/numbers-parser/branch/main/graph/badge.svg?token=EKIUFGT05E)](https://codecov.io/gh/masaccio/numbers-parser)\n\n`numbers-parser` is a Python module for parsing [Apple Numbers](https://www.apple.com/numbers/)\n`.numbers` files. It supports Numbers files generated by Numbers version 10.3, and up with the latest tested version being 12.2\n(current as of October 2022).\n\nIt supports and is tested against Python versions from 3.8 onwards. It is not compatible with earlier versions of Python.\n\nCurrently supported features of Numbers files are:\n\n* Multiple sheets per document\n* Multiple tables per sheet\n* Text, numeric, date, currency, duration, percentage cell types\n\nFormulas rely on Numbers storing current values which should usually be\nthe case. Formulas themselves rather than the computed values can optionally\nbe extracted. Styles are not supported.\n\nAs of version 3.0, `numbers-parser` has limited support for creating Numbers files.\n\n## Installation\n\n``` bash\npython3 -m pip install numbers-parser\n```\n\nA pre-requisite for this package is [python-snappy](https://pypi.org/project/python-snappy/) which will be installed by Python automatically, but python-snappy also requires that the binary libraries for snappy compression are present.\n\nThe most straightforward way to install the binary dependencies is to use [Homebrew](https://brew.sh) and source Python from Homebrew rather than from macOS as described in the [python-snappy github](https://github.com/andrix/python-snappy):\n\nFor Intel Macs:\n\n``` bash\nbrew install snappy python3\nCPPFLAGS="-I/usr/local/include -L/usr/local/lib" python3 -m pip install python-snappy\n```\n\nAnd on Apple Silicon:\n\n``` bash\nbrew install snappy python3\nCPPFLAGS="-I/opt/homebrew/include -L/opt/homebrew/lib" python3 -m pip install python-snappy\n```\n\n## Usage\n\nReading documents:\n\n``` python\nfrom numbers_parser import Document\ndoc = Document("my-spreasdsheet.numbers")\nsheets = doc.sheets\ntables = sheets[0].tables\nrows = tables[0].rows()\n```\n\n### Referring to sheets and tables\n\nBoth sheets and names can be accessed from lists of these objects using an integer index (`list` syntax) and using the name\nof the sheet/table (`dict` syntax):\n\n``` python\n# list access method\nsheet_1 = doc.sheets[0]\nprint("Opened sheet", sheet_1.name)\n\n# dict access method\ntable_1 = sheets["Table 1"]\nprint("Opened table", table_1.name)\n```\n\nAs of version 3.0, the `Document.sheets()` and `Sheet.tables()` methods are deprecated and will issue a `DeprecationWarning` if used. Instead of these functions, you should use the properties as demonstrated above. The legacy methods will be removed in a future version of `numbers-parser`.\n\n### Accessing data\n\n`Table` objects have a `rows` method which contains a nested list with an entry for each row of the table. Each row is\nitself a list of the column values. Empty cells in Numbers are returned as `None` values.\n\n``` python\ndata = sheets["Table 1"].rows()\nprint("Cell A1 contains", data[0][0])\nprint("Cell C2 contains", data[2][1])\n```\n\nCells are objects with a common base class of `Cell`. All cell types have a property `value` which returns the contents of the cell in as a native Python datatype. `DurationCell` object values are `datetime.timedelta` objects which are additionally available as a formatted value matching that stored in the Numbers spreadsheet. The formatted value is returned using the `formatted_value` property.\n\n### Cell references\n\nIn addition to extracting all data at once, individual cells can be referred to as methods\n\n``` python\ndoc = Document("my-spreasdsheet.numbers")\nsheets = doc.sheets\ntables = sheets["Sheet 1"].tables\ntable = tables["Table 1"]\n\n# row, column syntax\nprint("Cell A1 contains", table.cell(0, 0))\n# Excel/Numbers-style cell references\nprint("Cell C2 contains", table.cell("C2"))\n```\n\n### Merged cells\n\nWhen extracting data using ```rows()``` merged cells are ignored since only text values\nare returned. The ```cell()``` method of ```Table``` objects returns a ```Cell``` type\nobject which is typed by the type of cell in the Numbers table. ```MergeCell``` objects\nindicates cells removed in a merge.\n\n``` python\ndoc = Document("my-spreasdsheet.numbers")\nsheets = doc.sheets\ntables = sheets["Sheet 1"].tables\ntable = tables["Table 1"]\n\ncell = table.cell("A1")\nprint(cell.merge_range)\nprint(f"Cell A1 merge size is {cell.size[0]},{cell.size[1]})\n```\n\n### Row and column iterators\n\nTables have iterators for row-wise and column-wise iteration with each iterator\nreturning a list of the cells in that row or column\n\n``` python\nfor row in table.iter_rows(min_row=2, max_row=7, values_only=True):\n    sum += row\nfor col in table.iter_cols(min_row=2, max_row=7):\n    sum += col.value\n```\n\n### Pandas\n\nSince the return value of `data()` is a list of lists, you can pass this directly to pandas. Assuming you have a Numbers table with a single header which contains the names of the pandas series you want to create you can construct a pandas dataframe using:\n\n``` python\nimport pandas as pd\n\ndoc = Document("simple.numbers")\nsheets = doc.sheets\ntables = sheets[0].tables\ndata = tables[0].rows(values_only=True)\ndf = pd.DataFrame(data[1:], columns=data[0])\n```\n\n### Bullets and lists\n\nCells that contain bulleted or numbered lists can be identified by the `is_bulleted` property. Data from such cells is returned using the `value` property as with other cells, but can additionally extracted using the `bullets` property. `bullets` returns a list of the paragraphs in the cell without the bullet or numbering character. Newlines are not included when bullet lists are extracted using `bullets`.\n\n``` python\ndoc = Document("bullets.numbers")\nsheets = doc.sheets\ntables = sheets[0].tables\ntable = tables[0]\nif not table.cell(0, 1).is_bulleted:\n    print(table.cell(0, 1).value)\nelse:\n    bullets = ["* " + s for s in table.cell(0, 1).bullets]\n    print("\\n".join(bullets))\n```\n\nBulleted and numbered data can also be extracted with the bullet or number characters present in the text for each line in the cell in the same way as above but using the `formatted_bullets` property. A single space is inserted between the bullet character and the text string and in the case of bullets, this will be the Unicode character seen in Numbers, for example `"• some text"`.\n\n### \xa0Cell images\n\nQuerying cell formats is currently limited to image backrgounds only. If a cell has no background image, `None` is returned for all calls.\n\n``` python\ncell = table.cell("B1")\nwith open (cell.image_filename, "wb") as f:\n    f.write(cell.image_data)\nprint("Wrote file of type", cell.image_type)\n```\n\n## Writing Numbers files\n\n*This is considered experimental*: you are highly recommened not to overwrite working Numbers files and instead save data to a new file.\n\n### Limitations\n\nSince version 3.4.0, adding tables and sheets is supported. Known limitations to write support are:\n\n* Creating cells of type `BulletedTextCell` is not supported\n* Formats cannot be defined for `DurationCell` or `DateCell`\n* New tables are inserted with a fixed offset below the last table in a worksheet which does not take into account title or caption size\n* New sheets insert tables with formats copied from the first table in the previous sheet rather than default table formats\n\n### Editing cells\n\n`numbers-parser` will automatically empty rows and columns for any cell references that are out of range of the current table. The `write` method accepts the same cell numbering notation as `cell` plus an additional argument representing the new cell value. The type of the new value will be used to determine the cell type.\n\n``` python\ndoc = Document("old-sheet.numbers")\nsheets = doc.sheets\ntables = sheets[0].tables\ntable = tables[0]\ntable.write(1, 1, "This is new text")\ntable.write("B7", datetime(2020, 12, 25))\ndoc.save("new-sheet.numbers")\n```\n\nSheet names and table names can be changed by assigning a new value to the `name` of each:\n\n```python\nsheets[0].name = "My new sheet"\ntables[0].name = "Edited table"\n````\n\n### Adding tables and sheets\n\nAdditional tables and worksheets can be added to a `Document` before saving. If no sheet name or table name is supplied, `numbers-parser` will use `Sheet 1`, `Sheet 2`, etc.\n\n```python\ndoc = Document()\ndoc.add_sheet("New Sheet", "New Table")\nsheet = doc.sheets["New Sheet"]\ntable = sheet.tables["New Table"]\ntable.write(1, 1, 1000)\ntable.write(1, 2, 2000)\ntable.write(1, 3, 3000)\n\ndoc.save("sheet.numbers")\n```\n\n## Table geometries\n\n`numbers-parser` can query and change the position and size of tables. Changes made to a table\'s row height or column width is retained when files are saved.\n\n### \xa0Row and column sizes\n\nRow heights and column widths are queried and set using the `row_height` and `col_width` methods:\n\n```python\ndoc = Document("sheet.numbers")\ntable = doc.sheets[0].tables[0]\nprint(f"Table size is {table.height} x {table.width}")\nprint(f"Table row 1 height is {table.row_height(0)}")\ntable.row_height(0, 40)\nprint(f"Table row 1 height is now {table.row_height(0)}")\nprint(f"Table column A width is {table.col_width(0)}")\ntable.col_width(0, 200)\nprint(f"Table column A width is {table.col_width(0)}")\n```\n\n### \xa0Header row and columns\n\nWhen new tables are created, `numbers-parser` follows the Numbers convention of creating a table with one row header and one column header. You can change the number of headers by modifying the appopriate property:\n\n```python\ndoc = Document("sheet.numbers")\ntable = doc.sheets[0].tables[0]\ntable.num_header_rows = 2\ntable.num_header_cols = 0\ndoc.save("saved.numbers")\n```\n\nA zero header count will remove the headers from the table. Attempting to set a negative number of headers, or using more headers that rows or columns in the table will raise a `ValueError` exception.\n\n### Positioning tables\n\nBy default, new tables are positioned at a fixed offset below the last table vertically in a sheet and on the left side of the sheet. Large table headers and captions may result in new tables overlapping existing ones. The `add_table` method takes optional coordinates for positioning a table. A table\'s height and coordinates can also be queried to help aligning new tables:\n\n```python\n(x, y) = sheet.table[0].coordinates\ny += sheet.table[0].height + 200.0\nnew_table = sheet.add_table("Offset Table", x, y)\n```\n\n## Command-line scripts\n\nWhen installed from [PyPI](https://pypi.org/project/numbers-parser/), a command-like script `cat-numbers` is installed in Python\'s scripts folder. This script dumps Numbers spreadsheets into Excel-compatible CSV format, iterating through all the spreadsheets passed on the command-line.\n\n``` text\nusage: cat-numbers [-h] [-T | -S | -b] [-V] [--debug] [--formulas]\n                   [--formatting] [-s SHEET] [-t TABLE] [document ...]\n\nExport data from Apple Numbers spreadsheet tables\n\npositional arguments:\n  document                 Document(s) to export\n\noptional arguments:\n  -h, --help               show this help message and exit\n  -T, --list-tables        List the names of tables and exit\n  -S, --list-sheets        List the names of sheets and exit\n  -b, --brief              Don\'t prefix data rows with name of sheet/table (default: false)\n  -V, --version\n  --debug                  Enable debug output\n  --formulas               Dump formulas instead of formula results\n  --formatting             Dump formatted cells (durations) as they appear in Numbers\n  -s SHEET, --sheet SHEET  Names of sheet(s) to include in export\n  -t TABLE, --table TABLE  Names of table(s) to include in export\n```\n\nNote: `--formatting` will return different capitalisation for 12-hour times due to differences between Numbers\' representation of these dates and `datetime.strftime`. Numbers in English locales displays 12-hour times with \'am\' and \'pm\', but `datetime.strftime` on macOS at least cannot return lower-case versions of AM/PM.\n\n## Numbers File Formats\n\nNumbers uses a proprietary, compressed binary format to store its tables.\nThis format is comprised of a zip file containing images, as well as\n[Snappy](https://github.com/google/snappy)-compressed\n[Protobuf](https://github.com/protocolbuffers/protobuf) `.iwa` files containing\nmetadata, text, and all other definitions used in the spreadsheet.\n\n### Protobuf updates\n\nAs `numbers-parser` includes private Protobuf definitions extracted from a copy of Numbers, new versions of Numbers will inevitably create `.numbers` files that cannot be read by `numbers-parser`. As new versions of Numbers are released, running `make bootstrap` will perform all the steps necessary to recreate the protobuf files used `numbers-parser` to read Numbers spreadsheets.\n\nOn Apple Silicon Macs, the default protobuf package installation does not include the C++ optimised version which is required by the bootstrapping scripts to extract protobufs. You will receive the following error during build if this is the case:\n\n `This script requires the Protobuf installation to use the C++ implementation. Please reinstall Protobuf with C++ support.`\n\n To include the C++ support, download a released version of Google protobuf [from github](https://github.com/protocolbuffers/protobuf). Build instructions are in the [`src/README.md`](https://github.com/protocolbuffers/protobuf/blob/main/src/README.md) in the distribution but for macOS with [Homebrew](https://brew.sh) the two steps are, firstly to install the native protobuf libraries, which must be on your `LD_LIBRARY_PATH`:\n\n``` bash\nbrew install autoconf automake libtool\n./autogen.sh\n./configure --prefix=/usr/local\nmake check -j`sysctl -n hw.ncpu`\nsudo make install\n```\n\nAnd then to install the Python libraries with C++ support. If you already have protobuf install via Homebrew, you will need to `brew unlink` the installation.\n\n``` bash\ncd python\npython3 setup.py build --cpp_implementation\npython3 setup.py test --cpp_implementation\npython3 setup.py install --cpp_implementation\n```\n  \n  This will install protobuf in a folder above the source installation which can then be used by `make bootstrap` in the `numbers-parser` source tree.\n\n## Credits\n\n`numbers-parser` was built by [Jon Connell](http://github.com/masaccio) but relies heavily on from [prior work](https://github.com/psobot/keynote-parser) by [Peter Sobot](https://petersobot.com) to read the IWA format archives used by Apple\'s iWork family of applications, and to regenerate the mapping files required for Python. Both modules are derived from [previous work](https://github.com/obriensp/iWorkFileFormat/blob/master/Docs/index.md) by [Sean Patrick O\'Brien](http://www.obriensp.com).\n\nDecoding the data structures inside Numbers files was helped greatly by [Stingray-Reader](https://github.com/slott56/Stingray-Reader) by [Steven Lott](https://github.com/slott56).\n\nFormula tests were adapted from JavaScript tests used in\n[fast-formula-parser](https://github.com/LesterLyu/fast-formula-parser).\n\nDecimal128 conversion to and from byte storage was adapted from work done by the\n[SheetsJS project](https://github.com/SheetJS/sheetjs). SheetJS also helped greatly with some of the steps required to successfully save a Numbers spreadsheet.\n\n## License\n\nAll code in this repository is licensed under the [MIT License](https://github.com/masaccio/numbers-parser/blob/master/LICENSE.rst)\n',
-    'author': 'Jon Connell',
-    'author_email': 'python@figsandfudge.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/masaccio/numbers-parser',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+`numbers-parser` is a Python module for parsing [Apple Numbers](https://www.apple.com/numbers/)
+`.numbers` files. It supports Numbers files generated by Numbers version 10.3, and up with the latest tested version being 12.2
+(current as of October 2022).
 
+It supports and is tested against Python versions from 3.8 onwards. It is not compatible with earlier versions of Python.
+
+Currently supported features of Numbers files are:
+
+* Multiple sheets per document
+* Multiple tables per sheet
+* Text, numeric, date, currency, duration, percentage cell types
+
+Formulas rely on Numbers storing current values which should usually be
+the case. Formulas themselves rather than the computed values can optionally
+be extracted. Styles are not supported.
+
+As of version 3.0, `numbers-parser` has limited support for creating Numbers files.
+
+## Installation
+
+``` bash
+python3 -m pip install numbers-parser
+```
+
+A pre-requisite for this package is [python-snappy](https://pypi.org/project/python-snappy/) which will be installed by Python automatically, but python-snappy also requires that the binary libraries for snappy compression are present.
+
+The most straightforward way to install the binary dependencies is to use [Homebrew](https://brew.sh) and source Python from Homebrew rather than from macOS as described in the [python-snappy github](https://github.com/andrix/python-snappy):
+
+For Intel Macs:
+
+``` bash
+brew install snappy python3
+CPPFLAGS="-I/usr/local/include -L/usr/local/lib" python3 -m pip install python-snappy
+```
+
+And on Apple Silicon:
+
+``` bash
+brew install snappy python3
+CPPFLAGS="-I/opt/homebrew/include -L/opt/homebrew/lib" python3 -m pip install python-snappy
+```
+
+On Windows, you will need to either arrange for snappy to be found for VSC++ or you can install python binary libraries compiled by [Christoph Gohlke](https://www.lfd.uci.edu/~gohlke/pythonlibs/#python-snappy). You must select the correct python version for your installation. For example for python 3.11:
+
+``` text
+C:\Users\Jon>pip install C:\Users\Jon\Downloads\python_snappy-0.6.1-cp311-cp311-win_amd64.whl
+```
+
+## Usage
+
+Reading documents:
+
+``` python
+from numbers_parser import Document
+doc = Document("my-spreadsheet.numbers")
+sheets = doc.sheets
+tables = sheets[0].tables
+rows = tables[0].rows()
+```
+
+### Referring to sheets and tables
+
+Both sheets and names can be accessed from lists of these objects using an integer index (`list` syntax) and using the name
+of the sheet/table (`dict` syntax):
+
+``` python
+# list access method
+sheet_1 = doc.sheets[0]
+print("Opened sheet", sheet_1.name)
+
+# dict access method
+table_1 = sheets["Table 1"]
+print("Opened table", table_1.name)
+```
+
+As of version 3.0, the `Document.sheets()` and `Sheet.tables()` methods are deprecated and will issue a `DeprecationWarning` if used. Instead of these functions, you should use the properties as demonstrated above. The legacy methods will be removed in a future version of `numbers-parser`.
+
+### Accessing data
+
+`Table` objects have a `rows` method which contains a nested list with an entry for each row of the table. Each row is
+itself a list of the column values. Empty cells in Numbers are returned as `None` values.
+
+``` python
+data = sheets["Table 1"].rows()
+print("Cell A1 contains", data[0][0])
+print("Cell C2 contains", data[2][1])
+```
+
+Cells are objects with a common base class of `Cell`. All cell types have a property `value` which returns the contents of the cell in as a native Python datatype. `DurationCell` object values are `datetime.timedelta` objects which are additionally available as a formatted value matching that stored in the Numbers spreadsheet. The formatted value is returned using the `formatted_value` property.
+
+### Cell references
+
+In addition to extracting all data at once, individual cells can be referred to as methods
+
+``` python
+doc = Document("my-spreadsheet.numbers")
+sheets = doc.sheets
+tables = sheets["Sheet 1"].tables
+table = tables["Table 1"]
+
+# row, column syntax
+print("Cell A1 contains", table.cell(0, 0))
+# Excel/Numbers-style cell references
+print("Cell C2 contains", table.cell("C2"))
+```
+
+### Merged cells
+
+When extracting data using ```rows()``` merged cells are ignored since only text values
+are returned. The ```cell()``` method of ```Table``` objects returns a ```Cell``` type
+object which is typed by the type of cell in the Numbers table. ```MergeCell``` objects
+indicates cells removed in a merge.
+
+``` python
+doc = Document("my-spreadsheet.numbers")
+sheets = doc.sheets
+tables = sheets["Sheet 1"].tables
+table = tables["Table 1"]
+
+cell = table.cell("A1")
+print(cell.merge_range)
+print(f"Cell A1 merge size is {cell.size[0]},{cell.size[1]})
+```
+
+### Row and column iterators
+
+Tables have iterators for row-wise and column-wise iteration with each iterator
+returning a list of the cells in that row or column
+
+``` python
+for row in table.iter_rows(min_row=2, max_row=7, values_only=True):
+    sum += row
+for col in table.iter_cols(min_row=2, max_row=7):
+    sum += col.value
+```
+
+### Pandas
+
+Since the return value of `data()` is a list of lists, you can pass this directly to pandas. Assuming you have a Numbers table with a single header which contains the names of the pandas series you want to create you can construct a pandas dataframe using:
+
+``` python
+import pandas as pd
+
+doc = Document("simple.numbers")
+sheets = doc.sheets
+tables = sheets[0].tables
+data = tables[0].rows(values_only=True)
+df = pd.DataFrame(data[1:], columns=data[0])
+```
+
+### Bullets and lists
+
+Cells that contain bulleted or numbered lists can be identified by the `is_bulleted` property. Data from such cells is returned using the `value` property as with other cells, but can additionally extracted using the `bullets` property. `bullets` returns a list of the paragraphs in the cell without the bullet or numbering character. Newlines are not included when bullet lists are extracted using `bullets`.
+
+``` python
+doc = Document("bullets.numbers")
+sheets = doc.sheets
+tables = sheets[0].tables
+table = tables[0]
+if not table.cell(0, 1).is_bulleted:
+    print(table.cell(0, 1).value)
+else:
+    bullets = ["* " + s for s in table.cell(0, 1).bullets]
+    print("\n".join(bullets))
+```
+
+Bulleted and numbered data can also be extracted with the bullet or number characters present in the text for each line in the cell in the same way as above but using the `formatted_bullets` property. A single space is inserted between the bullet character and the text string and in the case of bullets, this will be the Unicode character seen in Numbers, for example `"• some text"`.
+
+###  Cell images
+
+Querying cell formats is currently limited to image backrgounds only. If a cell has no background image, `None` is returned for all calls.
+
+``` python
+cell = table.cell("B1")
+with open (cell.image_filename, "wb") as f:
+    f.write(cell.image_data)
+print("Wrote file of type", cell.image_type)
+```
+
+## Writing Numbers files
+
+*This is considered experimental*: you are highly recommened not to overwrite working Numbers files and instead save data to a new file.
+
+### Limitations
+
+Since version 3.4.0, adding tables and sheets is supported. Known limitations to write support are:
+
+* Creating cells of type `BulletedTextCell` is not supported
+* Formats cannot be defined for `DurationCell` or `DateCell`
+* New tables are inserted with a fixed offset below the last table in a worksheet which does not take into account title or caption size
+* New sheets insert tables with formats copied from the first table in the previous sheet rather than default table formats
+
+### Editing cells
+
+`numbers-parser` will automatically empty rows and columns for any cell references that are out of range of the current table. The `write` method accepts the same cell numbering notation as `cell` plus an additional argument representing the new cell value. The type of the new value will be used to determine the cell type.
+
+``` python
+doc = Document("old-sheet.numbers")
+sheets = doc.sheets
+tables = sheets[0].tables
+table = tables[0]
+table.write(1, 1, "This is new text")
+table.write("B7", datetime(2020, 12, 25))
+doc.save("new-sheet.numbers")
+```
+
+Sheet names and table names can be changed by assigning a new value to the `name` of each:
+
+```python
+sheets[0].name = "My new sheet"
+tables[0].name = "Edited table"
+````
+
+### Adding tables and sheets
+
+Additional tables and worksheets can be added to a `Document` before saving. If no sheet name or table name is supplied, `numbers-parser` will use `Sheet 1`, `Sheet 2`, etc.
+
+```python
+doc = Document()
+doc.add_sheet("New Sheet", "New Table")
+sheet = doc.sheets["New Sheet"]
+table = sheet.tables["New Table"]
+table.write(1, 1, 1000)
+table.write(1, 2, 2000)
+table.write(1, 3, 3000)
+
+doc.save("sheet.numbers")
+```
+
+## Table geometries
+
+`numbers-parser` can query and change the position and size of tables. Changes made to a table's row height or column width is retained when files are saved.
+
+###  Row and column sizes
+
+Row heights and column widths are queried and set using the `row_height` and `col_width` methods:
+
+```python
+doc = Document("sheet.numbers")
+table = doc.sheets[0].tables[0]
+print(f"Table size is {table.height} x {table.width}")
+print(f"Table row 1 height is {table.row_height(0)}")
+table.row_height(0, 40)
+print(f"Table row 1 height is now {table.row_height(0)}")
+print(f"Table column A width is {table.col_width(0)}")
+table.col_width(0, 200)
+print(f"Table column A width is {table.col_width(0)}")
+```
+
+###  Header row and columns
+
+When new tables are created, `numbers-parser` follows the Numbers convention of creating a table with one row header and one column header. You can change the number of headers by modifying the appopriate property:
+
+```python
+doc = Document("sheet.numbers")
+table = doc.sheets[0].tables[0]
+table.num_header_rows = 2
+table.num_header_cols = 0
+doc.save("saved.numbers")
+```
+
+A zero header count will remove the headers from the table. Attempting to set a negative number of headers, or using more headers that rows or columns in the table will raise a `ValueError` exception.
+
+### Positioning tables
+
+By default, new tables are positioned at a fixed offset below the last table vertically in a sheet and on the left side of the sheet. Large table headers and captions may result in new tables overlapping existing ones. The `add_table` method takes optional coordinates for positioning a table. A table's height and coordinates can also be queried to help aligning new tables:
+
+```python
+(x, y) = sheet.table[0].coordinates
+y += sheet.table[0].height + 200.0
+new_table = sheet.add_table("Offset Table", x, y)
+```
+
+## Command-line scripts
+
+When installed from [PyPI](https://pypi.org/project/numbers-parser/), a command-like script `cat-numbers` is installed in Python's scripts folder. This script dumps Numbers spreadsheets into Excel-compatible CSV format, iterating through all the spreadsheets passed on the command-line.
+
+``` text
+usage: cat-numbers [-h] [-T | -S | -b] [-V] [--debug] [--formulas]
+                   [--formatting] [-s SHEET] [-t TABLE] [document ...]
+
+Export data from Apple Numbers spreadsheet tables
+
+positional arguments:
+  document                 Document(s) to export
+
+optional arguments:
+  -h, --help               show this help message and exit
+  -T, --list-tables        List the names of tables and exit
+  -S, --list-sheets        List the names of sheets and exit
+  -b, --brief              Don't prefix data rows with name of sheet/table (default: false)
+  -V, --version
+  --debug                  Enable debug output
+  --formulas               Dump formulas instead of formula results
+  --formatting             Dump formatted cells (durations) as they appear in Numbers
+  -s SHEET, --sheet SHEET  Names of sheet(s) to include in export
+  -t TABLE, --table TABLE  Names of table(s) to include in export
+```
+
+Note: `--formatting` will return different capitalisation for 12-hour times due to differences between Numbers' representation of these dates and `datetime.strftime`. Numbers in English locales displays 12-hour times with 'am' and 'pm', but `datetime.strftime` on macOS at least cannot return lower-case versions of AM/PM.
+
+## Numbers File Formats
+
+Numbers uses a proprietary, compressed binary format to store its tables.
+This format is comprised of a zip file containing images, as well as
+[Snappy](https://github.com/google/snappy)-compressed
+[Protobuf](https://github.com/protocolbuffers/protobuf) `.iwa` files containing
+metadata, text, and all other definitions used in the spreadsheet.
+
+### Protobuf updates
+
+As `numbers-parser` includes private Protobuf definitions extracted from a copy of Numbers, new versions of Numbers will inevitably create `.numbers` files that cannot be read by `numbers-parser`. As new versions of Numbers are released, running `make bootstrap` will perform all the steps necessary to recreate the protobuf files used `numbers-parser` to read Numbers spreadsheets.
+
+The default protobuf package installation may not include the C++ optimised version which is required by the bootstrapping scripts to extract protobufs. You will receive the following error during build if this is the case:
+
+ `This script requires the Protobuf installation to use the C++ implementation. Please reinstall Protobuf with C++ support.`
+
+ To include the C++ support, download a released version of Google protobuf [from github](https://github.com/protocolbuffers/protobuf). Build instructions are in the [`src/README.md`](https://github.com/protocolbuffers/protobuf/blob/main/src/README.md) in the distribution but for macOS with [Homebrew](https://brew.sh) the two steps are, firstly to install the native protobuf libraries, which must be on your `LD_LIBRARY_PATH`:
+
+
+  This will install protobuf in a folder above the source installation which can then be used by `make bootstrap` in the `numbers-parser` source tree.
+
+## Credits
+
+`numbers-parser` was built by [Jon Connell](http://github.com/masaccio) but relies heavily on from [prior work](https://github.com/psobot/keynote-parser) by [Peter Sobot](https://petersobot.com) to read the IWA format archives used by Apple's iWork family of applications, and to regenerate the mapping files required for Python. Both modules are derived from [previous work](https://github.com/obriensp/iWorkFileFormat/blob/master/Docs/index.md) by [Sean Patrick O'Brien](http://www.obriensp.com).
+
+Decoding the data structures inside Numbers files was helped greatly by [Stingray-Reader](https://github.com/slott56/Stingray-Reader) by [Steven Lott](https://github.com/slott56).
+
+Formula tests were adapted from JavaScript tests used in
+[fast-formula-parser](https://github.com/LesterLyu/fast-formula-parser).
+
+Decimal128 conversion to and from byte storage was adapted from work done by the
+[SheetsJS project](https://github.com/SheetJS/sheetjs). SheetJS also helped greatly with some of the steps required to successfully save a Numbers spreadsheet.
+
+## License
+
+All code in this repository is licensed under the [MIT License](https://github.com/masaccio/numbers-parser/blob/master/LICENSE.rst)
 
-setup(**setup_kwargs)
```

