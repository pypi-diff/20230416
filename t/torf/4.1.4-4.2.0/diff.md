# Comparing `tmp/torf-4.1.4.tar.gz` & `tmp/torf-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torf-4.1.4.tar", last modified: Thu Jan 26 10:17:30 2023, max compression
+gzip compressed data, was "torf-4.2.0.tar", last modified: Sun Apr 16 12:04:20 2023, max compression
```

## Comparing `torf-4.1.4.tar` & `torf-4.2.0.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwx------   0 ich       (1000) ich       (1000)        0 2023-01-26 10:17:30.873764 torf-4.1.4/
--rw-------   0 ich       (1000) ich       (1000)    35149 2020-04-02 09:42:44.000000 torf-4.1.4/LICENSE
--rw-------   0 ich       (1000) ich       (1000)     3002 2023-01-26 10:17:30.873764 torf-4.1.4/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)     2135 2022-04-26 14:13:06.000000 torf-4.1.4/README.rst
--rw-------   0 ich       (1000) ich       (1000)       38 2023-01-26 10:17:30.873764 torf-4.1.4/setup.cfg
--rw-------   0 ich       (1000) ich       (1000)     1575 2022-11-09 17:40:17.000000 torf-4.1.4/setup.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-01-26 10:17:30.869764 torf-4.1.4/tests/
--rw-------   0 ich       (1000) ich       (1000)    19972 2022-04-21 17:08:25.000000 torf-4.1.4/tests/__init__.py
--rw-------   0 ich       (1000) ich       (1000)    23891 2022-11-24 15:38:20.000000 torf-4.1.4/tests/conftest.py
--rw-------   0 ich       (1000) ich       (1000)    61359 2023-01-07 16:09:57.000000 torf-4.1.4/tests/test_attributes.py
--rw-------   0 ich       (1000) ich       (1000)     1925 2020-06-20 13:29:35.000000 torf-4.1.4/tests/test_convert.py
--rw-------   0 ich       (1000) ich       (1000)    11832 2020-08-10 16:19:53.000000 torf-4.1.4/tests/test_exclude.py
--rw-------   0 ich       (1000) ich       (1000)     1638 2020-06-20 13:29:35.000000 torf-4.1.4/tests/test_fuzzy.py
--rw-------   0 ich       (1000) ich       (1000)     9854 2022-11-24 15:38:58.000000 torf-4.1.4/tests/test_generate.py
--rw-------   0 ich       (1000) ich       (1000)    24994 2020-06-20 13:29:35.000000 torf-4.1.4/tests/test_magnet.py
--rw-------   0 ich       (1000) ich       (1000)     3918 2020-06-20 13:29:35.000000 torf-4.1.4/tests/test_partial_size.py
--rw-------   0 ich       (1000) ich       (1000)     9711 2020-06-20 13:29:35.000000 torf-4.1.4/tests/test_read.py
--rw-------   0 ich       (1000) ich       (1000)    29610 2022-05-17 13:56:01.000000 torf-4.1.4/tests/test_utils.py
--rw-------   0 ich       (1000) ich       (1000)    16049 2020-06-20 13:29:35.000000 torf-4.1.4/tests/test_validate.py
--rw-------   0 ich       (1000) ich       (1000)    29245 2022-04-26 14:16:31.000000 torf-4.1.4/tests/test_verify_content.py
--rw-------   0 ich       (1000) ich       (1000)    20528 2022-04-20 10:54:04.000000 torf-4.1.4/tests/test_verify_filesize.py
--rw-------   0 ich       (1000) ich       (1000)     2844 2020-06-20 13:29:35.000000 torf-4.1.4/tests/test_write.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-01-26 10:17:30.869764 torf-4.1.4/torf/
--rw-------   0 ich       (1000) ich       (1000)      891 2023-01-25 18:08:41.000000 torf-4.1.4/torf/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     9945 2023-01-07 16:09:57.000000 torf-4.1.4/torf/_errors.py
--rw-------   0 ich       (1000) ich       (1000)    20636 2023-01-09 11:27:27.000000 torf-4.1.4/torf/_generate.py
--rw-------   0 ich       (1000) ich       (1000)    13957 2022-07-05 14:26:08.000000 torf-4.1.4/torf/_magnet.py
--rw-------   0 ich       (1000) ich       (1000)     7132 2023-01-16 10:29:01.000000 torf-4.1.4/torf/_reuse.py
--rw-------   0 ich       (1000) ich       (1000)    30268 2023-01-25 17:51:42.000000 torf-4.1.4/torf/_stream.py
--rw-------   0 ich       (1000) ich       (1000)    68623 2023-01-09 10:58:49.000000 torf-4.1.4/torf/_torrent.py
--rw-------   0 ich       (1000) ich       (1000)    26007 2022-05-17 13:56:01.000000 torf-4.1.4/torf/_utils.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-01-26 10:17:30.873764 torf-4.1.4/torf.egg-info/
--rw-------   0 ich       (1000) ich       (1000)     3002 2023-01-26 10:17:30.000000 torf-4.1.4/torf.egg-info/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)      633 2023-01-26 10:17:30.000000 torf-4.1.4/torf.egg-info/SOURCES.txt
--rw-------   0 ich       (1000) ich       (1000)        1 2023-01-26 10:17:30.000000 torf-4.1.4/torf.egg-info/dependency_links.txt
--rw-------   0 ich       (1000) ich       (1000)       19 2023-01-26 10:17:30.000000 torf-4.1.4/torf.egg-info/requires.txt
--rw-------   0 ich       (1000) ich       (1000)        5 2023-01-26 10:17:30.000000 torf-4.1.4/torf.egg-info/top_level.txt
+drwx------   0 ich       (1000) ich       (1000)        0 2023-04-16 12:04:20.671871 torf-4.2.0/
+-rw-------   0 ich       (1000) ich       (1000)    35149 2020-04-02 09:42:44.000000 torf-4.2.0/LICENSE
+-rw-------   0 ich       (1000) ich       (1000)     3002 2023-04-16 12:04:20.671871 torf-4.2.0/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)     2135 2022-04-26 14:13:06.000000 torf-4.2.0/README.rst
+-rw-------   0 ich       (1000) ich       (1000)       38 2023-04-16 12:04:20.671871 torf-4.2.0/setup.cfg
+-rw-------   0 ich       (1000) ich       (1000)     1575 2022-11-09 17:40:17.000000 torf-4.2.0/setup.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-04-16 12:04:20.663871 torf-4.2.0/tests/
+-rw-------   0 ich       (1000) ich       (1000)    19972 2022-04-21 17:08:25.000000 torf-4.2.0/tests/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)    23891 2022-11-24 15:38:20.000000 torf-4.2.0/tests/conftest.py
+-rw-------   0 ich       (1000) ich       (1000)    61584 2023-04-13 10:06:18.000000 torf-4.2.0/tests/test_attributes.py
+-rw-------   0 ich       (1000) ich       (1000)     1925 2020-06-20 13:29:35.000000 torf-4.2.0/tests/test_convert.py
+-rw-------   0 ich       (1000) ich       (1000)    11832 2020-08-10 16:19:53.000000 torf-4.2.0/tests/test_exclude.py
+-rw-------   0 ich       (1000) ich       (1000)     1638 2020-06-20 13:29:35.000000 torf-4.2.0/tests/test_fuzzy.py
+-rw-------   0 ich       (1000) ich       (1000)     9854 2022-11-24 15:38:58.000000 torf-4.2.0/tests/test_generate.py
+-rw-------   0 ich       (1000) ich       (1000)    24994 2020-06-20 13:29:35.000000 torf-4.2.0/tests/test_magnet.py
+-rw-------   0 ich       (1000) ich       (1000)     3918 2020-06-20 13:29:35.000000 torf-4.2.0/tests/test_partial_size.py
+-rw-------   0 ich       (1000) ich       (1000)     9712 2023-04-13 10:06:18.000000 torf-4.2.0/tests/test_read.py
+-rw-------   0 ich       (1000) ich       (1000)    29898 2023-01-09 14:33:59.000000 torf-4.2.0/tests/test_reuse.py
+-rw-------   0 ich       (1000) ich       (1000)    90416 2023-01-25 18:04:55.000000 torf-4.2.0/tests/test_stream.py
+-rw-------   0 ich       (1000) ich       (1000)    30054 2023-04-13 10:16:39.000000 torf-4.2.0/tests/test_utils.py
+-rw-------   0 ich       (1000) ich       (1000)    16381 2023-04-13 10:06:18.000000 torf-4.2.0/tests/test_validate.py
+-rw-------   0 ich       (1000) ich       (1000)    29451 2023-04-16 11:50:39.000000 torf-4.2.0/tests/test_verify_content.py
+-rw-------   0 ich       (1000) ich       (1000)    20528 2022-04-20 10:54:04.000000 torf-4.2.0/tests/test_verify_filesize.py
+-rw-------   0 ich       (1000) ich       (1000)     2844 2020-06-20 13:29:35.000000 torf-4.2.0/tests/test_write.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-04-16 12:04:20.671871 torf-4.2.0/torf/
+-rw-------   0 ich       (1000) ich       (1000)      891 2023-04-16 11:50:39.000000 torf-4.2.0/torf/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     9952 2023-04-13 10:06:18.000000 torf-4.2.0/torf/_errors.py
+-rw-------   0 ich       (1000) ich       (1000)    20636 2023-01-09 11:27:27.000000 torf-4.2.0/torf/_generate.py
+-rw-------   0 ich       (1000) ich       (1000)    13957 2022-07-05 14:26:08.000000 torf-4.2.0/torf/_magnet.py
+-rw-------   0 ich       (1000) ich       (1000)     7132 2023-03-12 14:07:48.000000 torf-4.2.0/torf/_reuse.py
+-rw-------   0 ich       (1000) ich       (1000)    30268 2023-01-25 17:51:42.000000 torf-4.2.0/torf/_stream.py
+-rw-------   0 ich       (1000) ich       (1000)    68659 2023-04-13 10:06:18.000000 torf-4.2.0/torf/_torrent.py
+-rw-------   0 ich       (1000) ich       (1000)    25915 2023-04-16 11:21:14.000000 torf-4.2.0/torf/_utils.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-04-16 12:04:20.671871 torf-4.2.0/torf.egg-info/
+-rw-------   0 ich       (1000) ich       (1000)     3002 2023-04-16 12:04:20.000000 torf-4.2.0/torf.egg-info/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)      674 2023-04-16 12:04:20.000000 torf-4.2.0/torf.egg-info/SOURCES.txt
+-rw-------   0 ich       (1000) ich       (1000)        1 2023-04-16 12:04:20.000000 torf-4.2.0/torf.egg-info/dependency_links.txt
+-rw-------   0 ich       (1000) ich       (1000)       19 2023-04-16 12:04:20.000000 torf-4.2.0/torf.egg-info/requires.txt
+-rw-------   0 ich       (1000) ich       (1000)        5 2023-04-16 12:04:20.000000 torf-4.2.0/torf.egg-info/top_level.txt
```

### Comparing `torf-4.1.4/LICENSE` & `torf-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torf-4.1.4/PKG-INFO` & `torf-4.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torf
-Version: 4.1.4
+Version: 4.2.0
 Summary: Python 3 module for creating and parsing torrent files and magnet URIs
 Home-page: https://github.com/rndusr/torf
 Author: Random User
 Author-email: rndusr@posteo.de
 License: GPLv3+
 Keywords: bittorrent torrent magnet
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `torf-4.1.4/README.rst` & `torf-4.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `torf-4.1.4/setup.py` & `torf-4.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `torf-4.1.4/tests/__init__.py` & `torf-4.2.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `torf-4.1.4/tests/conftest.py` & `torf-4.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `torf-4.1.4/tests/test_attributes.py` & `torf-4.2.0/tests/test_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -742,29 +742,30 @@
 
 def test_piece_size_is_set_to_wrong_type(create_torrent):
     torrent = create_torrent()
     with pytest.raises(ValueError) as excinfo:
         torrent.piece_size = 'hello'
     assert str(excinfo.value) == "piece_size must be int, not str: 'hello'"
 
-def test_piece_size_is_set_manually_to_not_power_of_two(create_torrent):
+@pytest.mark.parametrize('piece_size_', (-1, 0, 16385))
+def test_piece_size_is_set_manually_to_number_not_divisible_by_16_kib(piece_size_, create_torrent):
     torrent = create_torrent()
     with pytest.raises(torf.PieceSizeError) as excinfo:
-        torrent.piece_size = 123 * 1000
-    assert str(excinfo.value) == 'Piece size must be a power of 2: 123000'
+        torrent.piece_size = piece_size_
+    assert str(excinfo.value) == f'Piece size must be divisible by 16 KiB: {piece_size_}'
 
 def test_piece_size_can_be_invalid_in_metainfo(create_torrent):
     torrent = create_torrent()
     torrent.metainfo['info']['piece length'] = 123
     torrent.metainfo['info']['piece length'] = 'foo'
     torrent.metainfo['info']['piece length'] = -12
 
 
-PIECE_SIZE_MIN_DEFAULT = torf.Torrent.piece_size_min_default
-PIECE_SIZE_MAX_DEFAULT = torf.Torrent.piece_size_max_default
+PIECE_SIZE_MIN_DEFAULT = 32768
+PIECE_SIZE_MAX_DEFAULT = 163840
 
 # "piece_size_" because "piece_size" is already used for --piece-size
 # (see conftest.py)
 @pytest.mark.parametrize('with_path', (True, False), ids=['with path', 'without path'])
 @pytest.mark.parametrize(
     argnames='piece_size_, piece_size_min, piece_size_max, exp_piece_size_min, exp_piece_size_max, exp_exception',
     argvalues=(
@@ -823,15 +824,18 @@
             id='Invalid custom piece_size_max',
         ),
     ),
     ids=lambda v: repr(v),
 )
 def test_piece_size_min_max(piece_size_, piece_size_min, piece_size_max,
                             exp_piece_size_max, exp_piece_size_min, exp_exception,
-                            with_path, singlefile_content):
+                            with_path, singlefile_content, mocker):
+    mocker.patch.object(torf.Torrent, 'piece_size_min_default', PIECE_SIZE_MIN_DEFAULT)
+    mocker.patch.object(torf.Torrent, 'piece_size_max_default', PIECE_SIZE_MAX_DEFAULT)
+
     if exp_exception:
         with pytest.raises(type(exp_exception), match=rf'^{re.escape(str(exp_exception))}$'):
             torf.Torrent(
                 path=singlefile_content.path if with_path else None,
                 piece_size=piece_size_,
                 piece_size_min=piece_size_min,
                 piece_size_max=piece_size_max,
```

### Comparing `torf-4.1.4/tests/test_convert.py` & `torf-4.2.0/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `torf-4.1.4/tests/test_exclude.py` & `torf-4.2.0/tests/test_exclude.py`

 * *Files identical despite different names*

### Comparing `torf-4.1.4/tests/test_fuzzy.py` & `torf-4.2.0/tests/test_fuzzy.py`

 * *Files identical despite different names*

### Comparing `torf-4.1.4/tests/test_generate.py` & `torf-4.2.0/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `torf-4.1.4/tests/test_magnet.py` & `torf-4.2.0/tests/test_magnet.py`

 * *Files identical despite different names*

### Comparing `torf-4.1.4/tests/test_partial_size.py` & `torf-4.2.0/tests/test_partial_size.py`

 * *Files identical despite different names*

### Comparing `torf-4.1.4/tests/test_read.py` & `torf-4.2.0/tests/test_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
     with pytest.raises(torf.MetainfoError) as excinfo:
         torf.Torrent.read_stream(io.BytesIO(bencode.encode(data)), validate=False)
     assert excinfo.match(r"^Invalid metainfo: \['info'\] must be dict, not int: 1$")
 
 def test_validate_missing_pieces():
     data = OrderedDict([(b'info', {b'name': b'Foo',
-                                   b'piece length': 1024})])
+                                   b'piece length': 16384})])
     fo = io.BytesIO(bencode.encode(data))
     with pytest.raises(torf.MetainfoError) as excinfo:
         torf.Torrent.read_stream(fo, validate=True)
     assert excinfo.match(r"^Invalid metainfo: Missing 'pieces' in \['info'\]$")
 
 
 def test_read_nonstandard_data_without_validation():
```

### Comparing `torf-4.1.4/tests/test_utils.py` & `torf-4.2.0/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,37 @@
 import pytest
 
 import torf
 from torf import _errors as errors
 from torf import _utils as utils
 
 
-def test_is_power_of_2():
-    assert utils.is_power_of_2(0) is False
-    for n in range(1, 30):
-        assert utils.is_power_of_2(2**n) is True
-        assert utils.is_power_of_2(-2**n) is True
-        assert utils.is_power_of_2(3**n) is False
-        assert utils.is_power_of_2(-5**n) is False
+@pytest.mark.parametrize(
+    argnames='num, exp_return_value',
+    argvalues=(
+        (-16 * 3 * 1024 + 1, False),
+        (-16 * 3 * 1024 + 0, False),
+        (-16 * 3 * 1024 - 1, False),
+        (-16 * 1 * 1024 + 1, False),
+        (-16 * 1 * 1024 + 0, False),
+        (-16 * 1 * 1024 - 1, False),
+        (-1, False),
+        (0, False),
+        (1, False),
+        (16 * 1 * 1024 + 1, False),
+        (16 * 1 * 1024 + 0, True),
+        (16 * 1 * 1024 - 1, False),
+        (16 * 3 * 1024 + 1, False),
+        (16 * 3 * 1024 + 0, True),
+        (16 * 3 * 1024 - 1, False),
+
+    ),
+)
+def test_is_divisible_by_16_kib(num, exp_return_value):
+    assert utils.is_divisible_by_16_kib(num) is exp_return_value
 
 
 def test_iterable_startswith():
     a = ['a', 'b', 'c', 'd']
     b = ['a', 'b', 'c']
     assert utils.iterable_startswith(a, b)
     assert not utils.iterable_startswith(b, a)
@@ -242,15 +258,15 @@
             'four': 'baz',
             'five': [{'a': [1, 2, 3], 'b': 4}],
         }
     }
     assert utils.decode_dict(encoded) == decoded
 
 def test_decoding_invalid_unicode():
-    assert utils.decode_value(b'\xed') == b'\xed'
+    assert utils.decode_value(b'\xed') == '\uFFFD'  # REPLACEMENT CHARACTER: �'
 
 
 def test_encoding():
     class SillyStr(str):
         def __str__(self):
             return f'This is silly: {super().__str__()}'
         __repr__ = __str__
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `torf-4.1.4/tests/test_validate.py` & `torf-4.2.0/tests/test_validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,20 +34,28 @@
     t = generated_singlefile_torrent
     t.metainfo['info']['piece length'] = [700]
     with pytest.raises(torf.MetainfoError) as excinfo:
         t.validate()
     assert str(excinfo.value) == ("Invalid metainfo: ['info']['piece length'] "
                                   "must be int, not list: [700]")
 
-def test_piece_length_not_power_of_two(generated_singlefile_torrent):
+@pytest.mark.parametrize(
+    argnames='piece_length, exp_exception',
+    argvalues=(
+        (-1, torf.MetainfoError("['info']['piece length'] is invalid: -1")),
+        (0, torf.MetainfoError("['info']['piece length'] is invalid: 0")),
+        (16385, torf.MetainfoError("['info']['piece length'] is invalid: 16385")),
+    ),
+)
+def test_piece_length_not_divisible_by_16_kib(piece_length, exp_exception, generated_singlefile_torrent):
     t = generated_singlefile_torrent
-    t.metainfo['info']['piece length'] = 1023
-    with pytest.raises(torf.MetainfoError) as excinfo:
+    t.metainfo['info']['piece length'] = piece_length
+    with pytest.raises(type(exp_exception)) as excinfo:
         t.validate()
-    assert str(excinfo.value) == "Invalid metainfo: ['info']['piece length'] is invalid: 1023"
+    assert str(excinfo.value) == str(exp_exception)
 
 def test_wrong_pieces_type(generated_singlefile_torrent):
     t = generated_singlefile_torrent
     t.metainfo['info']['pieces'] = 'many'
     with pytest.raises(torf.MetainfoError) as excinfo:
         t.validate()
     assert str(excinfo.value) == ("Invalid metainfo: ['info']['pieces'] "
```

### Comparing `torf-4.1.4/tests/test_verify_content.py` & `torf-4.2.0/tests/test_verify_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,21 @@
                calc_piece_indexes, calc_pieces_done, change_file_size,
                display_filespecs, file_piece_indexes, file_range, fuzzylist,
                pos2file, pos2files, random_positions, round_down_to_multiple)
 
 import logging  # isort:skip
 debug = logging.getLogger('test').debug
 
+
+# Allow arbitrary small piece sizes to make debugging easier.
+@pytest.fixture(autouse=True)
+def ignore_piece_size_check(mocker):
+    mocker.patch('torf._utils.is_divisible_by_16_kib', return_value=True)
+
+
 class CollectingCallback():
     """Collect call arguments and make basic assertions"""
     def __init__(self, torrent):
         super().__init__()
         self.torrent = torrent
         self.seen_pieces_done = []
         self._seen_piece_indexes = collections.defaultdict(lambda: fuzzylist())  # noqa: F405
```

### Comparing `torf-4.1.4/tests/test_verify_filesize.py` & `torf-4.2.0/tests/test_verify_filesize.py`

 * *Files identical despite different names*

### Comparing `torf-4.1.4/tests/test_write.py` & `torf-4.2.0/tests/test_write.py`

 * *Files identical despite different names*

### Comparing `torf-4.1.4/torf/__init__.py` & `torf-4.2.0/torf/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 
 # flake8: noqa
 
 """
 Create and parse torrent files and magnet URIs
 """
 
-__version__ = '4.1.4'
+__version__ = '4.2.0'
 
 from ._errors import *
 from ._magnet import Magnet
 from ._stream import TorrentFileStream
 from ._torrent import Torrent
 from ._utils import File, Filepath
```

### Comparing `torf-4.1.4/torf/_errors.py` & `torf-4.2.0/torf/_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         self._size = size
         self._min = min
         self._max = max
         if min is not None and max is not None:
             super().__init__(f'Piece size must be between {min} and {max}: {size}',
                              size, min=min, max=max)
         else:
-            super().__init__(f'Piece size must be a power of 2: {size}',
+            super().__init__(f'Piece size must be divisible by 16 KiB: {size}',
                              size)
 
     @property
     def size(self):
         """The invalid piece size"""
         return self._size
```

### Comparing `torf-4.1.4/torf/_generate.py` & `torf-4.2.0/torf/_generate.py`

 * *Files identical despite different names*

### Comparing `torf-4.1.4/torf/_magnet.py` & `torf-4.2.0/torf/_magnet.py`

 * *Files identical despite different names*

### Comparing `torf-4.1.4/torf/_reuse.py` & `torf-4.2.0/torf/_reuse.py`

 * *Files identical despite different names*

### Comparing `torf-4.1.4/torf/_stream.py` & `torf-4.2.0/torf/_stream.py`

 * *Files identical despite different names*

### Comparing `torf-4.1.4/torf/_torrent.py` & `torf-4.2.0/torf/_torrent.py`

 * *Files 0% similar despite different names*

```diff
@@ -619,15 +619,15 @@
                 )
 
         try:
             piece_length = int(value)
         except (TypeError, ValueError):
             raise ValueError(f'piece_size must be int, not {type(value).__name__}: {value!r}')
         else:
-            if not utils.is_power_of_2(piece_length):
+            if not utils.is_divisible_by_16_kib(piece_length):
                 raise error.PieceSizeError(piece_length)
             elif not self.piece_size_min <= piece_length <= self.piece_size_max:
                 raise error.PieceSizeError(piece_length,
                                            min=self.piece_size_min,
                                            max=self.piece_size_max)
             self.metainfo['info']['piece length'] = piece_length
 
@@ -641,15 +641,15 @@
         """
         return self._piece_size_min
 
     @piece_size_min.setter
     def piece_size_min(self, piece_size_min):
         if piece_size_min is None:
             self._piece_size_min = type(self).piece_size_min_default
-        elif not utils.is_power_of_2(piece_size_min):
+        elif not utils.is_divisible_by_16_kib(piece_size_min):
             raise error.PieceSizeError(piece_size_min)
         else:
             self._piece_size_min = int(piece_size_min)
 
     @property
     def piece_size_max(self):
         """
@@ -660,15 +660,15 @@
         """
         return self._piece_size_max
 
     @piece_size_max.setter
     def piece_size_max(self, piece_size_max):
         if piece_size_max is None:
             self._piece_size_max = type(self).piece_size_max_default
-        elif not utils.is_power_of_2(piece_size_max):
+        elif not utils.is_divisible_by_16_kib(piece_size_max):
             raise error.PieceSizeError(piece_size_max)
         else:
             self._piece_size_max = int(piece_size_max)
 
     piece_size_min_default = 16 * 1024  # 16 KiB
     """
     Smallest allowed piece size (default value)
@@ -1350,15 +1350,15 @@
         md = self.metainfo
         info = md['info']
 
         # Check values shared by singlefile and multifile torrents
         utils.assert_type(md, ('info',), (dict,), must_exist=True)
         utils.assert_type(md, ('info', 'name'), (str,), must_exist=True)
         utils.assert_type(md, ('info', 'piece length'), (int,), must_exist=True,
-                          check=utils.is_power_of_2)
+                          check=utils.is_divisible_by_16_kib)
         utils.assert_type(md, ('info', 'pieces'), (abc.ByteString,), must_exist=True)
         utils.assert_type(md, ('info', 'private'), (bool, int), must_exist=False)
         utils.assert_type(md, ('announce',), (str,), must_exist=False, check=utils.is_url)
         utils.assert_type(md, ('announce-list',), (utils.Iterable,), must_exist=False)
         for i,_ in enumerate(md.get('announce-list', ())):
             utils.assert_type(md, ('announce-list', i), (utils.Iterable,))
             for j,_ in enumerate(md['announce-list'][i]):
```

### Comparing `torf-4.1.4/torf/_utils.py` & `torf-4.2.0/torf/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,20 +31,19 @@
 import urllib.request
 from datetime import datetime
 from urllib.parse import quote_plus as urlquote  # noqa: F401
 
 from . import _errors as error
 
 
-def is_power_of_2(num):
-    """Return whether `num` is a power of two"""
-    if num == 0:
+def is_divisible_by_16_kib(num):
+    """Return whether `num` is divisible by 16384 and positive"""
+    if num <= 0:
         return False
-    log = math.log2(abs(num))
-    return int(log) == float(log)
+    return num % 16384 == 0
 
 def iterable_startswith(a, b):
     a_len = len(a)
     for i, b_item in enumerate(b):
         if i >= a_len:
             # a can't start with b if b is longer than a
             return False
@@ -727,20 +726,17 @@
 
     elif check is not None and not check(obj[key]):
         raise error.MetainfoError(f"{keychain_str}[{key!r}] is invalid: {obj[key]!r}")
 
 
 def decode_value(value):
     if isinstance(value, collections.abc.ByteString):
-        # Torrents can contain binary data in non-standard fields. There is no
-        # way to tell if a field is supposed to be decoded as a string or not.
-        try:
-            return bytes.decode(value, encoding='utf-8', errors='strict')
-        except UnicodeDecodeError:
-            return value
+        # WARNING: Torrents can contain binary data (e.g. "pieces" field). You
+        #          should handle and remove those separately beforehand.
+        return bytes.decode(value, encoding='utf-8', errors='replace')
     elif isinstance(value, collections.abc.Sequence):
         return decode_list(value)
     elif isinstance(value, collections.abc.Mapping):
         return decode_dict(value)
     else:
         return value
```

### Comparing `torf-4.1.4/torf.egg-info/PKG-INFO` & `torf-4.2.0/torf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torf
-Version: 4.1.4
+Version: 4.2.0
 Summary: Python 3 module for creating and parsing torrent files and magnet URIs
 Home-page: https://github.com/rndusr/torf
 Author: Random User
 Author-email: rndusr@posteo.de
 License: GPLv3+
 Keywords: bittorrent torrent magnet
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `torf-4.1.4/torf.egg-info/SOURCES.txt` & `torf-4.2.0/torf.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 tests/test_convert.py
 tests/test_exclude.py
 tests/test_fuzzy.py
 tests/test_generate.py
 tests/test_magnet.py
 tests/test_partial_size.py
 tests/test_read.py
+tests/test_reuse.py
+tests/test_stream.py
 tests/test_utils.py
 tests/test_validate.py
 tests/test_verify_content.py
 tests/test_verify_filesize.py
 tests/test_write.py
 torf/__init__.py
 torf/_errors.py
```

