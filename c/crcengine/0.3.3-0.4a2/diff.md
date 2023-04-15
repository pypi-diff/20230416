# Comparing `tmp/crcengine-0.3.3.tar.gz` & `tmp/crcengine-0.4a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crcengine-0.3.3.tar", last modified: Sun Jun 26 19:09:10 2022, max compression
+gzip compressed data, was "crcengine-0.4a2.tar", max compression
```

## Comparing `crcengine-0.3.3.tar` & `crcengine-0.4a2.tar`

### file list

```diff
@@ -1,76 +1,12 @@
-drwxrwxrwx   0        0        0        0 2022-06-26 19:09:10.141931 crcengine-0.3.3/
--rw-rw-rw-   0        0        0    17687 2020-02-13 21:49:38.000000 crcengine-0.3.3/.pylintrc
--rw-rw-rw-   0        0        0     1130 2022-06-26 19:03:50.000000 crcengine-0.3.3/CHANGES.rst
--rw-rw-rw-   0        0        0    35149 2019-11-20 00:22:26.000000 crcengine-0.3.3/LICENSE
--rw-rw-rw-   0        0        0      431 2021-04-11 18:09:19.000000 crcengine-0.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0     5856 2022-06-26 19:09:10.141931 crcengine-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     4704 2021-04-11 18:09:19.000000 crcengine-0.3.3/README.rst
--rw-rw-rw-   0        0        0        7 2022-06-26 18:39:40.000000 crcengine-0.3.3/VERSION.txt
-drwxrwxrwx   0        0        0        0 2022-06-26 19:09:10.057920 crcengine-0.3.3/docs/
--rw-rw-rw-   0        0        0      610 2020-01-30 21:52:01.000000 crcengine-0.3.3/docs/Makefile
-drwxrwxrwx   0        0        0        0 2022-06-26 19:09:10.025717 crcengine-0.3.3/docs/build/
-drwxrwxrwx   0        0        0        0 2022-06-26 19:09:10.077921 crcengine-0.3.3/docs/build/_static/
--rw-rw-rw-   0        0        0      673 2020-01-29 20:54:02.000000 crcengine-0.3.3/docs/build/_static/ajax-loader.gif
--rw-rw-rw-   0        0        0      756 2020-01-29 20:54:02.000000 crcengine-0.3.3/docs/build/_static/comment-bright.png
--rw-rw-rw-   0        0        0      829 2020-01-29 20:54:02.000000 crcengine-0.3.3/docs/build/_static/comment-close.png
--rw-rw-rw-   0        0        0      641 2020-01-29 20:54:02.000000 crcengine-0.3.3/docs/build/_static/comment.png
--rw-rw-rw-   0        0        0      222 2020-01-29 20:54:02.000000 crcengine-0.3.3/docs/build/_static/down-pressed.png
--rw-rw-rw-   0        0        0      202 2020-01-29 20:54:02.000000 crcengine-0.3.3/docs/build/_static/down.png
--rw-rw-rw-   0        0        0      286 2020-01-29 20:54:02.000000 crcengine-0.3.3/docs/build/_static/file.png
--rw-rw-rw-   0        0        0       90 2020-01-29 20:54:02.000000 crcengine-0.3.3/docs/build/_static/minus.png
--rw-rw-rw-   0        0        0       90 2020-01-29 20:54:02.000000 crcengine-0.3.3/docs/build/_static/plus.png
--rw-rw-rw-   0        0        0      214 2020-01-29 20:54:02.000000 crcengine-0.3.3/docs/build/_static/up-pressed.png
--rw-rw-rw-   0        0        0      203 2020-01-29 20:54:02.000000 crcengine-0.3.3/docs/build/_static/up.png
-drwxrwxrwx   0        0        0        0 2022-06-26 19:09:10.025717 crcengine-0.3.3/docs/build/html/
-drwxrwxrwx   0        0        0        0 2022-06-26 19:09:10.093923 crcengine-0.3.3/docs/build/html/_static/
--rw-rw-rw-   0        0        0      673 2020-01-29 21:11:19.000000 crcengine-0.3.3/docs/build/html/_static/ajax-loader.gif
--rw-rw-rw-   0        0        0      756 2020-01-29 21:11:19.000000 crcengine-0.3.3/docs/build/html/_static/comment-bright.png
--rw-rw-rw-   0        0        0      829 2020-01-29 21:11:19.000000 crcengine-0.3.3/docs/build/html/_static/comment-close.png
--rw-rw-rw-   0        0        0      641 2020-01-29 21:11:19.000000 crcengine-0.3.3/docs/build/html/_static/comment.png
--rw-rw-rw-   0        0        0      222 2020-01-29 21:11:19.000000 crcengine-0.3.3/docs/build/html/_static/down-pressed.png
--rw-rw-rw-   0        0        0      202 2020-01-29 21:11:19.000000 crcengine-0.3.3/docs/build/html/_static/down.png
--rw-rw-rw-   0        0        0      286 2020-01-29 21:11:19.000000 crcengine-0.3.3/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2020-01-29 21:11:19.000000 crcengine-0.3.3/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2020-01-29 21:11:19.000000 crcengine-0.3.3/docs/build/html/_static/plus.png
--rw-rw-rw-   0        0        0      214 2020-01-29 21:11:19.000000 crcengine-0.3.3/docs/build/html/_static/up-pressed.png
--rw-rw-rw-   0        0        0      203 2020-01-29 21:11:19.000000 crcengine-0.3.3/docs/build/html/_static/up.png
--rwxrwxrwx   0        0        0      817 2020-03-06 00:27:21.000000 crcengine-0.3.3/docs/make.bat
-drwxrwxrwx   0        0        0        0 2022-06-26 19:09:10.105925 crcengine-0.3.3/docs/source/
--rw-rw-rw-   0        0        0     5279 2021-04-11 18:09:19.000000 crcengine-0.3.3/docs/source/conf.py
--rw-rw-rw-   0        0        0      778 2021-04-11 18:09:19.000000 crcengine-0.3.3/docs/source/crcengine.rst
--rw-rw-rw-   0        0        0       32 2021-04-11 18:09:19.000000 crcengine-0.3.3/docs/source/history.rst
--rw-rw-rw-   0        0        0      500 2021-04-11 18:09:19.000000 crcengine-0.3.3/docs/source/index.rst
--rw-rw-rw-   0        0        0       71 2021-04-11 18:09:19.000000 crcengine-0.3.3/docs/source/modules.rst
--rw-rw-rw-   0        0        0       37 2021-04-11 18:09:19.000000 crcengine-0.3.3/docs/source/readme.rst
-drwxrwxrwx   0        0        0        0 2022-06-26 19:09:10.105925 crcengine-0.3.3/examples/
--rw-rw-rw-   0        0        0      704 2021-04-11 18:09:19.000000 crcengine-0.3.3/examples/example.py
-drwxrwxrwx   0        0        0        0 2022-06-26 19:09:10.113926 crcengine-0.3.3/examples/out/
--rw-rw-rw-   0        0        0     2879 2020-01-30 22:39:41.000000 crcengine-0.3.3/examples/out/crc16_xmodem.c
--rw-rw-rw-   0        0        0      205 2020-01-30 22:39:41.000000 crcengine-0.3.3/examples/out/crc16_xmodem.h
--rw-rw-rw-   0        0        0     4040 2020-01-30 22:39:41.000000 crcengine-0.3.3/examples/out/crc32.c
--rw-rw-rw-   0        0        0      177 2020-01-30 22:39:41.000000 crcengine-0.3.3/examples/out/crc32.h
--rw-rw-rw-   0        0        0      151 2022-04-09 09:52:26.000000 crcengine-0.3.3/pyproject.toml
--rw-rw-rw-   0        0        0      158 2021-04-11 18:09:19.000000 crcengine-0.3.3/requirements.in
--rw-rw-rw-   0        0        0     3389 2022-04-09 09:54:32.000000 crcengine-0.3.3/requirements.txt
--rw-rw-rw-   0        0        0     1503 2022-06-26 19:09:10.145932 crcengine-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      186 2021-04-11 18:09:19.000000 crcengine-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-26 19:09:10.033720 crcengine-0.3.3/src/
-drwxrwxrwx   0        0        0        0 2022-06-26 19:09:10.121939 crcengine-0.3.3/src/crcengine/
--rw-rw-rw-   0        0        0     1282 2021-04-11 18:09:19.000000 crcengine-0.3.3/src/crcengine/__init__.py
--rw-rw-rw-   0        0        0     4853 2021-04-11 18:09:19.000000 crcengine-0.3.3/src/crcengine/__main__.py
--rw-rw-rw-   0        0        0     6448 2021-04-11 18:09:19.000000 crcengine-0.3.3/src/crcengine/algorithms.py
--rw-rw-rw-   0        0        0    14130 2022-06-26 18:39:30.000000 crcengine-0.3.3/src/crcengine/calc.py
--rw-rw-rw-   0        0        0     8214 2021-04-11 18:09:19.000000 crcengine-0.3.3/src/crcengine/codegen.py
-drwxrwxrwx   0        0        0        0 2022-06-26 19:09:10.141931 crcengine-0.3.3/src/crcengine/templates/
--rw-rw-rw-   0        0        0     1298 2021-04-11 18:09:19.000000 crcengine-0.3.3/src/crcengine/templates/c_template
--rw-rw-rw-   0        0        0      291 2020-01-30 21:41:28.000000 crcengine-0.3.3/src/crcengine/templates/h_template
--rw-rw-rw-   0        0        0      458 2021-04-11 18:09:19.000000 crcengine-0.3.3/src/crcengine/templates/test_template
-drwxrwxrwx   0        0        0        0 2022-06-26 19:09:10.137928 crcengine-0.3.3/src/crcengine.egg-info/
--rw-rw-rw-   0        0        0     5856 2022-06-26 19:09:09.000000 crcengine-0.3.3/src/crcengine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1674 2022-06-26 19:09:10.000000 crcengine-0.3.3/src/crcengine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-26 19:09:09.000000 crcengine-0.3.3/src/crcengine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2022-06-26 19:09:09.000000 crcengine-0.3.3/src/crcengine.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-06-26 19:09:09.000000 crcengine-0.3.3/src/crcengine.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       36 2022-06-26 19:09:09.000000 crcengine-0.3.3/src/crcengine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-06-26 19:09:09.000000 crcengine-0.3.3/src/crcengine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      332 2021-04-11 18:09:19.000000 crcengine-0.3.3/tox.ini
+-rw-r--r--   0        0        0    35149 2019-11-13 08:29:00.381942 crcengine-0.4a2/LICENSE
+-rw-r--r--   0        0        0     1570 2023-04-15 23:37:54.480008 crcengine-0.4a2/pyproject.toml
+-rw-r--r--   0        0        0     4709 2023-04-15 23:26:27.574057 crcengine-0.4a2/README.rst
+-rw-r--r--   0        0        0     1972 2023-04-15 23:26:27.589686 crcengine-0.4a2/src/crcengine/__init__.py
+-rw-r--r--   0        0        0     4841 2023-04-15 23:26:27.589686 crcengine-0.4a2/src/crcengine/__main__.py
+-rw-r--r--   0        0        0     9245 2023-04-15 23:26:27.589686 crcengine-0.4a2/src/crcengine/algorithms.py
+-rw-r--r--   0        0        0    23912 2023-04-15 23:26:27.589686 crcengine-0.4a2/src/crcengine/calc.py
+-rw-r--r--   0        0        0     7979 2023-04-15 23:26:27.589686 crcengine-0.4a2/src/crcengine/codegen.py
+-rw-r--r--   0        0        0     1300 2023-04-15 23:26:27.589686 crcengine-0.4a2/src/crcengine/templates/c_template
+-rw-r--r--   0        0        0      291 2019-12-21 11:49:25.832968 crcengine-0.4a2/src/crcengine/templates/h_template
+-rw-r--r--   0        0        0      458 2021-04-05 22:32:42.944797 crcengine-0.4a2/src/crcengine/templates/test_template
+-rw-r--r--   0        0        0     5835 1970-01-01 00:00:00.000000 crcengine-0.4a2/PKG-INFO
```

### Comparing `crcengine-0.3.3/LICENSE` & `crcengine-0.4a2/LICENSE`

 * *Files identical despite different names*

### Comparing `crcengine-0.3.3/PKG-INFO` & `crcengine-0.4a2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,158 +1,163 @@
-Metadata-Version: 2.1
-Name: crcengine
-Version: 0.3.3
-Summary: A library for CRC calculation and code generation
-Home-page: https://github.com/GardenTools/crcengine
-Author: Garden Tools
-Author-email: gardensofdorwinion@gmail.com
-License: GNU General Public License v3
-Project-URL: Changelog, https://github.com/GardenTools/CrcEngine/blob/master/CHANGES.rst
-Project-URL: Documentation, https://crcengine.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/GardenTools/CrcEngine
-Keywords: crcengine crc cyclic redundancy check checksum code-generation Castagnoli CRC32 CRC16-CCITT
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-.. image:: https://img.shields.io/pypi/v/crcengine.svg
-        :target: https://pypi.python.org/pypi/crcengine
-
-..  image:: https://img.shields.io/github/workflow/status/GardenTools/CrcEngine/Python%20package/master
-        :target: https://github.com/GardenTools/CrcEngine/actions?query=branch%3Amaster
-
-.. image:: https://img.shields.io/pypi/pyversions/CrcEngine.svg
-        :target: https://pypi.python.org/pypi/crcengine
-
-.. image:: https://img.shields.io/pypi/format/CrcEngine.svg
-        :target: https://pypi.python.org/pypi/crcengine
-
-.. image:: https://readthedocs.org/projects/crcengine/badge/?version=latest
-        :target: https://crcengine.readthedocs.io/en/latest/?badge=latest
-        :alt: Documentation Status
-
-=========
-CrcEngine
-=========
-A python library for CRC calculation providing table-based as well as
-bit-bashing implementations (for reference).
-
-* Free software: GNU General Public License v3
-* Documentation: https://crcengine.readthedocs.io.
-
-Installing
-----------
-CrcEngine can be installing using pip with
-
-.. code-block:: python
-
-    pip install crcengine
-
-Usage
------
-Pre-defined algorithms such as CRC32 are available. Tailored algorithms can
-be created by calling CrcEngine.create() and other related methods.
-
-A calculation engine for a specific named algorithm can be obtained using
-CrcEngine.new(). Algorithms which are not pre-defined can be created using
-CrcEngine.create() 
-
-A list of pre-defined algorithms can be obtained using crcengine.algorithms_available()
-
-.. code-block:: python
-
-   >>> list(crcengine.algorithms_available())
-   ['crc8', 'crc8-autosar', 'crc8-bluetooth', 'crc8-ccitt', 'crc8-gsm-b', 'crc8-sae-j1850', 'crc15-can', 'crc16-kermit', 'crc16-ccitt-true', 'crc16-xmodem', 'crc16-autosar', 'crc16-ccitt-false', 'crc16-cdma2000', 'crc16-ibm', 'crc16-modbus', 'crc16-profibus', 'crc24-flexray16-a', 'crc24-flexray16-b', 'crc32', 'crc32-bzip2', 'crc32-c', 'crc64-ecma']
-
-
-Built-in algorithms
-~~~~~~~~~~~~~~~~~~~
-crc8, crc8-autosar, crc8-bluetooth, crc8-ccitt, crc8-gsm-b, crc8-sae-j1850, crc15-can, crc16-kermit, crc16-ccitt-true, crc16-xmodem, crc16-autosar, crc16-ccitt-false, crc16-cdma2000, crc16-ibm, crc16-modbus, crc16-profibus, crc24-flexray16-a, crc24-flexray16-b, crc32, crc32-bzip2, crc32-c, crc64-ecma
-
-Examples
---------
-Using a pre-defined algorithm
-
-.. code-block:: python
-
-  import crcengine
-  crc_algorithm = crcengine.new('crc32-bzip2')
-  result = crc_algorithm(b'123456789')
-  print('CRC=0x{:08x}'.format(result))
-
-Output:
-> CRC=0xfc891918
-
-Defining an algorithm
-
-.. code-block:: python
-
-  import crcengine
-  crc_openpgp = crcengine.create(0x864cfb, 24, 0xb704ce, ref_in=False,
-                                 ref_out=False, xor_out=0,
-                                 name='crc-24-openpgp')
-
-Code Generation
----------------
-The library can generate C code for a given table-algorithm. The code produced
-is intended to be a reasonable compromise between size, complexity and speed
-without requiring allocation of memory for table generation at runtime.
-
-Faster implementations of specific algorithms can be achieved in software which
-unroll loops and pipeline the operations different bytes to introduce
-parallelism in the calculation see intel_soft_src_ for example. Some processors
-also include instructions specifically for crc calculation.
-
-.. _intel_soft_src: https://github.com/intel/soft-crc
-
-Code Generation Example usage:
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Generating code into a directory named "out" by passing CRC parameters
-
-.. code-block:: python
-
-    params = crcengine.get_algorithm_params('crc32')
-    crcengine.generate_code(params, 'out/')
-
-or referencing the algorithm by name
-
-.. code-block:: python
-
-    crcengine.generate_code('crc16-xmodem', 'out/')
-
-
-Downloading
------------
-- The source is available on github_
-- Git clone crcengine.git_
-- On pypi.org_
-
-.. _github: https://github.com/GardenTools/crcengine
-.. _crcengine.git: https://github.com/GardenTools/crcengine.git
-.. _pypi.org: https://pypi.org/project/crcengine/
-
-Running the tests
--------------------------
-Tests can be performed directly by executing pytest in the "tests" directory
-
-Running the Codegen tests
--------------------------
-The codegen tests make use of ceedling_ which is expected to be installed as a ruby gem.
-The unit tests are configured to compile with gcc.
-
-.. _ceedling: https://github.com/ThrowTheSwitch/Ceedling
-
--------
-
-With thanks to Greg Cook for providing such a thoroughly collated list of
-`CRC definitions`_
-
-.. _CRC definitions: http://reveng.sourceforge.net/crc-catalogue/all.htm
+Metadata-Version: 2.1
+Name: crcengine
+Version: 0.4a2
+Summary: A library for CRC calculation and code generation
+Home-page: https://github.com/GardenTools/crcengine
+License: GPL-3.0-only
+Keywords: crcengine,CRC,cyclic,redundancy,check,checksum,code-generation,Castagnoli,CRC32,CRC16-CCITT
+Author: Garden Tools
+Author-email: gardensofdorwinion@gmail.com
+Requires-Python: >=3.7.2,<4.0.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: C
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Communications
+Classifier: Topic :: System :: Networking
+Classifier: Topic :: Utilities
+Requires-Dist: importlib-metadata (>=3.6) ; python_version < "3.8"
+Requires-Dist: jinja2 (>=2.7)
+Project-URL: Documentation, https://crcengine.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/GardenTools/crcengine
+Description-Content-Type: text/x-rst
+
+.. image:: https://img.shields.io/pypi/v/crcengine.svg
+        :target: https://pypi.python.org/pypi/crcengine
+
+..  image:: https://img.shields.io/github/actions/workflow/status/GardenTools/CrcEngine/python-package.yml
+        :target: https://github.com/GardenTools/CrcEngine/actions?query=branch%3Amaster
+
+.. image:: https://img.shields.io/pypi/pyversions/CrcEngine.svg
+        :target: https://pypi.python.org/pypi/crcengine
+
+.. image:: https://img.shields.io/pypi/format/CrcEngine.svg
+        :target: https://pypi.python.org/pypi/crcengine
+
+.. image:: https://readthedocs.org/projects/crcengine/badge/?version=latest
+        :target: https://crcengine.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+==========
+CrcEngine
+==========
+A python library for CRC calculation providing table-based as well as
+bit-bashing implementations (for reference).
+
+* Free software: GNU General Public License v3
+* Documentation: https://crcengine.readthedocs.io.
+
+Installing
+----------
+CrcEngine can be installing using pip with
+
+.. code-block:: python
+
+    pip install crcengine
+
+Usage
+-----
+Pre-defined algorithms such as CRC32 are available. Tailored algorithms can
+be created by calling CrcEngine.create() and other related methods.
+
+A calculation engine for a specific named algorithm can be obtained using
+CrcEngine.new(). Algorithms which are not pre-defined can be created using
+CrcEngine.create() 
+
+A list of pre-defined algorithms can be obtained using crcengine.algorithms_available()
+
+.. code-block:: python
+
+   >>> list(crcengine.algorithms_available())
+   ['crc8', 'crc8-autosar', 'crc8-bluetooth', 'crc8-ccitt', 'crc8-gsm-b', 'crc8-sae-j1850', 'crc15-can', 'crc16-kermit', 'crc16-ccitt-true', 'crc16-xmodem', 'crc16-autosar', 'crc16-ccitt-false', 'crc16-cdma2000', 'crc16-ibm', 'crc16-modbus', 'crc16-profibus', 'crc24-flexray16-a', 'crc24-flexray16-b', 'crc32', 'crc32-bzip2', 'crc32-c', 'crc64-ecma']
+
+
+Built-in algorithms
+~~~~~~~~~~~~~~~~~~~
+crc8, crc8-autosar, crc8-bluetooth, crc8-ccitt, crc8-gsm-b, crc8-sae-j1850, crc15-can, crc16-kermit, crc16-ccitt-true, crc16-xmodem, crc16-autosar, crc16-ccitt-false, crc16-cdma2000, crc16-ibm, crc16-modbus, crc16-profibus, crc24-flexray16-a, crc24-flexray16-b, crc32, crc32-bzip2, crc32-c, crc64-ecma
+
+Examples
+--------
+Using a pre-defined algorithm
+
+.. code-block:: python
+
+  import crcengine
+  crc_algorithm = crcengine.new('crc32-bzip2')
+  result = crc_algorithm(b'123456789')
+  print('CRC=0x{:08x}'.format(result))
+
+Output:
+> CRC=0xfc891918
+
+Defining an algorithm
+
+.. code-block:: python
+
+  import crcengine
+  crc_openpgp = crcengine.create(0x864cfb, 24, 0xb704ce, ref_in=False,
+                                 ref_out=False, xor_out=0,
+                                 name='crc-24-openpgp')
+
+Code Generation
+---------------
+The library can generate C code for a given table-algorithm. The code produced
+is intended to be a reasonable compromise between size, complexity and speed
+without requiring allocation of memory for table generation at runtime.
+
+Faster implementations of specific algorithms can be achieved in software which
+unroll loops and pipeline the operations different bytes to introduce
+parallelism in the calculation see intel_soft_src_ for example. Some processors
+also include instructions specifically for crc calculation.
+
+.. _intel_soft_src: https://github.com/intel/soft-crc
+
+Code Generation Example usage:
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Generating code into a directory named "out" by passing CRC parameters
+
+.. code-block:: python
+
+    params = crcengine.get_algorithm_params('crc32')
+    crcengine.generate_code(params, 'out/')
+
+or referencing the algorithm by name
+
+.. code-block:: python
+
+    crcengine.generate_code('crc16-xmodem', 'out/')
+
+
+Downloading
+-----------
+- The source is available on github_
+- Git clone crcengine.git_
+- On pypi.org_
+
+.. _github: https://github.com/GardenTools/crcengine
+.. _crcengine.git: https://github.com/GardenTools/crcengine.git
+.. _pypi.org: https://pypi.org/project/crcengine/
+
+Running the tests
+-------------------------
+Tests can be performed directly by executing pytest in the "tests" directory
+
+Running the Codegen tests
+-------------------------
+The codegen tests make use of ceedling_ which is expected to be installed as a ruby gem.
+The unit tests are configured to compile with gcc.
+
+.. _ceedling: https://github.com/ThrowTheSwitch/Ceedling
+
+-------
+
+With thanks to Greg Cook for providing such a thoroughly collated list of
+`CRC definitions`_
+
+.. _CRC definitions: http://reveng.sourceforge.net/crc-catalogue/all.htm
+
```

### Comparing `crcengine-0.3.3/README.rst` & `crcengine-0.4a2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 .. image:: https://img.shields.io/pypi/v/crcengine.svg
         :target: https://pypi.python.org/pypi/crcengine
 
-..  image:: https://img.shields.io/github/workflow/status/GardenTools/CrcEngine/Python%20package/master
+..  image:: https://img.shields.io/github/actions/workflow/status/GardenTools/CrcEngine/python-package.yml
         :target: https://github.com/GardenTools/CrcEngine/actions?query=branch%3Amaster
 
 .. image:: https://img.shields.io/pypi/pyversions/CrcEngine.svg
         :target: https://pypi.python.org/pypi/crcengine
 
 .. image:: https://img.shields.io/pypi/format/CrcEngine.svg
         :target: https://pypi.python.org/pypi/crcengine
 
 .. image:: https://readthedocs.org/projects/crcengine/badge/?version=latest
         :target: https://crcengine.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
-=========
+==========
 CrcEngine
-=========
+==========
 A python library for CRC calculation providing table-based as well as
 bit-bashing implementations (for reference).
 
 * Free software: GNU General Public License v3
 * Documentation: https://crcengine.readthedocs.io.
 
 Installing
```

### Comparing `crcengine-0.3.3/src/crcengine/__main__.py` & `crcengine-0.4a2/src/crcengine/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Command line invocation for crcengine to either generate code or run on a file"""
 
 # This file is part of CrcEngine, a python library for CRC calculation
 #
 # Copyright 2021 Garden Tools software
 #
-# crcengine is free software: you can redistribute it an d /or modify
+# crcengine is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # crcengine is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -17,15 +17,15 @@
 # You should have received a copy of the GNU General Public License
 # along with crcengine.  If not, see <https://www.gnu.org/licenses/>.
 
 import argparse
 import sys
 
 import crcengine
-import crcengine.codegen as codegen
+from crcengine import codegen
 
 
 def main():
     """Main entry point for command line"""
     parser = make_arg_parser()
     process_cmdline(parser)
 
@@ -139,20 +139,20 @@
     """
     algo = crcengine.new(args.algorithm)
     prefix = "0x" if args.hex_prefix else ""
     if args.string:
         data = args.string.encode()
     elif args.file:
         # This is a bit stupid for now just to get it working, ideally calculation would be chunked
-        with open(args.file, "rb") as f:
-            data = f.read()
+        with open(args.file, "rb") as file:
+            data = file.read()
     else:
         data = sys.stdin.read().encode()
     result = algo.calculate(data)
-    print("{}{:x}".format(prefix, result))
+    print(f"{prefix}{result:x}")
 
 
 def do_generate(args):
     """Perform the generate command
 
     :param args:  arguments as produced by parse_args()
     :return:
```

### Comparing `crcengine-0.3.3/src/crcengine/codegen.py` & `crcengine-0.4a2/src/crcengine/codegen.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,109 +3,107 @@
 Generation of C code for CRC calculation
 """
 
 # This file is part of CrcEngine, a python library for CRC calculation
 #
 # Copyright 2021 Garden Tools software
 #
-# crcengine is free software: you can redistribute it an d /or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+#   This program is free software: you can redistribute it and/or modify
+#   it under the terms of the GNU General Public License as published by
+#   the Free Software Foundation, either version 3 of the License, or
+#   (at your option) any later version.
 #
-# crcengine is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+#   This program is distributed in the hope that it will be useful,
+#   but WITHOUT ANY WARRANTY; without even the implied warranty of
+#   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#   GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
-# along with crcengine.  If not, see <https://www.gnu.org/licenses/>.
+#   You should have received a copy of the GNU General Public License
+#   along with crcengine.  If not, see <https://www.gnu.org/licenses/>.
 
 from __future__ import generator_stop
 
 import os
 import pathlib
 import textwrap
 from collections import namedtuple
 
 from jinja2 import Environment, FileSystemLoader
 
 from .algorithms import get_algorithm_params
-from .calc import create_lsb_table, create_msb_table
-from crcengine import __version__ as crcengine_version
+from .calc import bit_reverse_n, create_lsb_table, create_msb_table
 
 # Generated file information
-_GenFile = namedtuple("GenFile", ["template", "output"])
+_GenFile = namedtuple("_GenFile", ["template", "output"])
 
 
 def generate_code(
-    crc_params, output_dir="out/", language="C", seed_parameter=False, func_name=None
+    crc_name_params, output_dir="out/", language="C", seed_parameter=False, func_name=None
 ):
     """Generate code implementing a specific CRC. Currently only language=C is
     supported"""
-    if isinstance(crc_params, str):
+    if isinstance(crc_name_params, str):
         # crc_params is an algorithm name, so replace it with the parameters
-        crc_params = get_algorithm_params(crc_params)
+        crc_name_params = get_algorithm_params(crc_name_params)
 
     env = _get_jinja_environment()
     template_params = _get_template_params(
-        crc_params, output_dir, seed_parameter, func_name, language
+        crc_name_params, output_dir, seed_parameter, func_name, language
     )
     _generate_output_files(env, template_params)
 
 
 def _get_template_params(crc_params, output_dir, seed_parameter, func_name, language):
     datatype_bits = _get_datatype_bits(crc_params["width"])
-    crc_id = crc_params["name"].replace("-", "_")
+    crc_id = crc_params["name"].replace("-", "_").replace("/", "_")
+    result_mask = (1 << crc_params["width"]) - 1
     if not func_name:
         func_name = crc_id
     template_params = {
         "after_table": "",
-        "crc_datatype": "uint{datatype_bits}_t".format(datatype_bits=datatype_bits),
+        "crc_datatype": f"uint{datatype_bits}_t",
         "comment_begin": "/*",
         "comment_end": "*/",
         "datatype_bits": datatype_bits,
         "before_table": "",
         "byte_type": "uint8_t",
         "function_name": func_name,
         "language": language,
-        "table_name": "{crc_id}_table".format(crc_id=crc_id),
+        "table_name": f"{crc_id}_table",
         "value_rows": _generate_table_text(crc_params, datatype_bits),
         "output_dir": output_dir,
         "reflect": crc_params["ref_in"],
         "includes": ["#include <stdint.h>"],
         "c_includes": [],
-        "preamble": "/* Auto-generated by CrcEngine {crcengine_version} */".format(
-            crcengine_version=crcengine_version
-        ),
-        "result_mask": "0x{:x}".format((1 << crc_params["width"]) - 1),
+        "preamble": "/* Auto-generated by CrcEngine */",
+        "result_mask": f"0x{result_mask:x}",
         "requires_result_mask": crc_params["width"] != datatype_bits,
-        "header_macro": "{}_H".format(crc_id.upper()),
+        "header_macro": f"{crc_id.upper()}_H",
         "msb_shift": crc_params["width"] - 8,
         "gen_files": [
-            _GenFile("c_template", "{crc_id}.c".format(crc_id=crc_id)),
-            _GenFile("h_template", "{crc_id}.h".format(crc_id=crc_id)),
+            _GenFile("c_template", f"{crc_id}.c"),
+            _GenFile("h_template", f"{crc_id}.h"),
         ],
         # The header file is required here so that it can be included in the C
         # file
-        "header_file": "{crc_id}.h".format(crc_id=crc_id),
+        "header_file": f"{crc_id}.h",
     }
     # suffix for numeric literals of the same type as the CRC
     lit_sufx = "u"
     # These are optional parameters which are checked with 'is defined' in the
     # template, if they are not defined it means that the operation the value
     # is relevant for should not be performed
     if not seed_parameter:
-        template_params["seed"] = "0x{crc_param:0x}{lit_sufx}".format(
-            crc_param=crc_params["seed"], lit_sufx=lit_sufx
-        )
+        # If the input is reflected, we need to also reflect the seed hard-coded
+        # into the C file
+        seed = (bit_reverse_n(crc_params["seed"], crc_params["width"]) if crc_params["ref_in"] else
+                crc_params["seed"])
+        template_params["seed"] = f"0x{seed:0x}{lit_sufx}"
     if crc_params["xor_out"]:
-        template_params["xor_out"] = "0x{crc_param:0x}{lit_sufx}".format(
-            crc_param=crc_params["xor_out"], lit_sufx=lit_sufx
-        )
+        template_params["xor_out"] = f"0x{crc_params['xor_out']:0x}{lit_sufx}"
     return template_params
 
 
 def generate_test(name, output_dir):
     """Generate a Ceedling C-test wrapper for a given algorithm's generated code
 
     :param name: name of algorithm
@@ -115,43 +113,41 @@
     crc_params = get_algorithm_params(name, include_check=True)
     jinja_env = _get_jinja_environment()
     template_params = _get_template_params(crc_params, output_dir, False, None, "C")
     crc_id = crc_params["name"].replace("-", "_")
     template_params["test_name"] = crc_id
     template_params["check_string"] = '"123456789"'
     template_params["crc_function"] = crc_id
-    template_params["comparison"] = "TEST_ASSERT_EQUAL_HEX{}".format(
-        template_params["datatype_bits"]
-    )
-    template_params["expected_value"] = "0x{:x}".format(crc_params["check"])
+    template_params["comparison"] = f"TEST_ASSERT_EQUAL_HEX{template_params['datatype_bits']}"
+    template_params["expected_value"] = f"0x{crc_params['check']:x}"
     _ensure_directory(output_dir)
     template_file = jinja_env.get_template("test_template")
     output_text = template_file.render(template_params)
 
-    output_filename = "test_" + "{crc_id}.c".format(crc_id=crc_id)
+    output_filename = "test_" + f"{crc_id}.c"
     output_file_path = os.path.join(output_dir, output_filename)
 
-    with open(output_file_path, "w") as f:
-        f.write(output_text)
+    with open(output_file_path, "w", encoding='utf-8') as file:
+        file.write(output_text)
 
 
 def _get_jinja_environment():
     templates_dir = _get_templates_dir()
     env = Environment(loader=FileSystemLoader(templates_dir), trim_blocks=True)
     return env
 
 
 def _generate_output_files(env, template_params):
     _ensure_directory(template_params["output_dir"])
     for gen_file in template_params["gen_files"]:
         template_file = env.get_template(gen_file.template)
         output_text = template_file.render(template_params)
         output_file_path = os.path.join(template_params["output_dir"], gen_file.output)
-        with open(output_file_path, "w") as f:
-            f.write(output_text)
+        with open(output_file_path, "w", encoding="utf-8") as file_obj:
+            file_obj.write(output_text)
 
 
 def _get_templates_dir():
     package_dir = os.path.dirname(__file__)
     templates_dir = os.path.join(package_dir, "templates")
     return templates_dir
 
@@ -203,20 +199,15 @@
 
     :param table:
     :return: list of rows of table entry strings
     """
     spacer = ", "
     indent = indent_width * " "
     elements = [
-        "{number_prefix}{value:0{value_width}x}{number_suffix}".format(
-            number_prefix=number_prefix,
-            value=value,
-            value_width=value_width,
-            number_suffix=number_suffix,
-        )
+        f"{number_prefix}{value:0{value_width}x}{number_suffix}"
         for value in table
     ]
     txt = spacer.join(elements)
     wrapper = textwrap.TextWrapper(
         width=max_width,
         initial_indent=indent,
         subsequent_indent=indent,
```

### Comparing `crcengine-0.3.3/src/crcengine/templates/c_template` & `crcengine-0.4a2/src/crcengine/templates/c_template`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 {{include}}
 {% endfor %}
 #include <stdio.h>
 #include "{{header_file}}"
 
 {% if xor_out is defined -%}
 #define RESULT_XOR_MASK {{xor_out}}
+
 {% set return_expression = 'crc ^ RESULT_XOR_MASK' %}
 {% else %}
 {% set return_expression = 'crc' %}
 {% endif %}
 
 {%- if reflect %}
 {% set shift_op = '>>' %}
```

