# Comparing `tmp/aiooss2-0.2.3.tar.gz` & `tmp/aiooss2-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiooss2-0.2.3.tar", last modified: Wed Oct  5 03:53:57 2022, max compression
+gzip compressed data, was "aiooss2-0.2.4.tar", last modified: Sun Apr 16 09:51:58 2023, max compression
```

## Comparing `aiooss2-0.2.3.tar` & `aiooss2-0.2.4.tar`

### file list

```diff
@@ -1,44 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 03:53:57.961289 aiooss2-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 03:53:57.957289 aiooss2-0.2.3/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      737 2022-10-05 03:53:32.000000 aiooss2-0.2.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 03:53:57.957289 aiooss2-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1680 2022-10-05 03:53:32.000000 aiooss2-0.2.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-10-05 03:53:32.000000 aiooss2-0.2.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-05 03:53:32.000000 aiooss2-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      954 2022-10-05 03:53:32.000000 aiooss2-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-05 03:53:32.000000 aiooss2-0.2.3/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11345 2022-10-05 03:53:32.000000 aiooss2-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-10-05 03:53:32.000000 aiooss2-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2667 2022-10-05 03:53:57.961289 aiooss2-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2063 2022-10-05 03:53:32.000000 aiooss2-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 03:53:57.957289 aiooss2-0.2.3/aiooss2/
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-10-05 03:53:32.000000 aiooss2-0.2.3/aiooss2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7033 2022-10-05 03:53:32.000000 aiooss2-0.2.3/aiooss2/adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)    26228 2022-10-05 03:53:32.000000 aiooss2-0.2.3/aiooss2/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      596 2022-10-05 03:53:32.000000 aiooss2-0.2.3/aiooss2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4883 2022-10-05 03:53:32.000000 aiooss2-0.2.3/aiooss2/http.py
--rw-r--r--   0 runner    (1001) docker     (121)     4644 2022-10-05 03:53:32.000000 aiooss2-0.2.3/aiooss2/iterators.py
--rw-r--r--   0 runner    (1001) docker     (121)     5938 2022-10-05 03:53:32.000000 aiooss2-0.2.3/aiooss2/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     2586 2022-10-05 03:53:32.000000 aiooss2-0.2.3/aiooss2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 03:53:57.957289 aiooss2-0.2.3/aiooss2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2667 2022-10-05 03:53:57.000000 aiooss2-0.2.3/aiooss2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-10-05 03:53:57.000000 aiooss2-0.2.3/aiooss2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 03:53:57.000000 aiooss2-0.2.3/aiooss2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 03:53:57.000000 aiooss2-0.2.3/aiooss2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-10-05 03:53:57.000000 aiooss2-0.2.3/aiooss2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-05 03:53:57.000000 aiooss2-0.2.3/aiooss2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 03:53:57.957289 aiooss2-0.2.3/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1397 2022-10-05 03:53:32.000000 aiooss2-0.2.3/examples/simple.py
--rw-r--r--   0 runner    (1001) docker     (121)     1649 2022-10-05 03:53:32.000000 aiooss2-0.2.3/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-10-05 03:53:32.000000 aiooss2-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1791 2022-10-05 03:53:57.961289 aiooss2-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 03:53:57.957289 aiooss2-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 03:53:32.000000 aiooss2-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3052 2022-10-05 03:53:32.000000 aiooss2-0.2.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 03:53:57.957289 aiooss2-0.2.3/tests/func/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 03:53:32.000000 aiooss2-0.2.3/tests/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-10-05 03:53:32.000000 aiooss2-0.2.3/tests/func/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (121)     8965 2022-10-05 03:53:32.000000 aiooss2-0.2.3/tests/func/test_object.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 03:53:57.957289 aiooss2-0.2.3/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 03:53:32.000000 aiooss2-0.2.3/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3573 2022-10-05 03:53:32.000000 aiooss2-0.2.3/tests/unit/test_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:58.547588 aiooss2-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-16 09:51:35.000000 aiooss2-0.2.4/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-16 09:51:35.000000 aiooss2-0.2.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:58.539588 aiooss2-0.2.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-16 09:51:35.000000 aiooss2-0.2.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:58.543588 aiooss2-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-16 09:51:35.000000 aiooss2-0.2.4/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-16 09:51:35.000000 aiooss2-0.2.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-16 09:51:35.000000 aiooss2-0.2.4/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-16 09:51:35.000000 aiooss2-0.2.4/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-16 09:51:35.000000 aiooss2-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-16 09:51:35.000000 aiooss2-0.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-16 09:51:35.000000 aiooss2-0.2.4/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-16 09:51:35.000000 aiooss2-0.2.4/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-16 09:51:35.000000 aiooss2-0.2.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-16 09:51:35.000000 aiooss2-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-16 09:51:35.000000 aiooss2-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-16 09:51:58.547588 aiooss2-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-16 09:51:35.000000 aiooss2-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-16 09:51:35.000000 aiooss2-0.2.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:58.543588 aiooss2-0.2.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:58.543588 aiooss2-0.2.4/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-16 09:51:35.000000 aiooss2-0.2.4/docs/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-16 09:51:35.000000 aiooss2-0.2.4/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-16 09:51:35.000000 aiooss2-0.2.4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:58.543588 aiooss2-0.2.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-16 09:51:35.000000 aiooss2-0.2.4/examples/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-16 09:51:35.000000 aiooss2-0.2.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-16 09:51:35.000000 aiooss2-0.2.4/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-16 09:51:35.000000 aiooss2-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-16 09:51:58.547588 aiooss2-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:58.539588 aiooss2-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:58.543588 aiooss2-0.2.4/src/aiooss2/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-16 09:51:35.000000 aiooss2-0.2.4/src/aiooss2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-16 09:51:35.000000 aiooss2-0.2.4/src/aiooss2/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29416 2023-04-16 09:51:35.000000 aiooss2-0.2.4/src/aiooss2/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-16 09:51:35.000000 aiooss2-0.2.4/src/aiooss2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-04-16 09:51:35.000000 aiooss2-0.2.4/src/aiooss2/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-04-16 09:51:35.000000 aiooss2-0.2.4/src/aiooss2/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-04-16 09:51:35.000000 aiooss2-0.2.4/src/aiooss2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-04-16 09:51:35.000000 aiooss2-0.2.4/src/aiooss2/multipart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19767 2023-04-16 09:51:35.000000 aiooss2-0.2.4/src/aiooss2/resumable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-16 09:51:35.000000 aiooss2-0.2.4/src/aiooss2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:58.543588 aiooss2-0.2.4/src/aiooss2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-16 09:51:58.000000 aiooss2-0.2.4/src/aiooss2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-16 09:51:58.000000 aiooss2-0.2.4/src/aiooss2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 09:51:58.000000 aiooss2-0.2.4/src/aiooss2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 09:51:58.000000 aiooss2-0.2.4/src/aiooss2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-16 09:51:58.000000 aiooss2-0.2.4/src/aiooss2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-16 09:51:58.000000 aiooss2-0.2.4/src/aiooss2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:58.543588 aiooss2-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-16 09:51:35.000000 aiooss2-0.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-16 09:51:35.000000 aiooss2-0.2.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:58.543588 aiooss2-0.2.4/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:35.000000 aiooss2-0.2.4/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-16 09:51:35.000000 aiooss2-0.2.4/tests/func/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-04-16 09:51:35.000000 aiooss2-0.2.4/tests/func/test_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-16 09:51:35.000000 aiooss2-0.2.4/tests/func/test_resumable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-16 09:51:35.000000 aiooss2-0.2.4/tests/test_aiooss2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:58.547588 aiooss2-0.2.4/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:35.000000 aiooss2-0.2.4/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-16 09:51:35.000000 aiooss2-0.2.4/tests/unit/test_adapter.py
```

### Comparing `aiooss2-0.2.3/.github/dependabot.yml` & `aiooss2-0.2.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.3/.github/workflows/release.yml` & `aiooss2-0.2.4/.github/workflows/release.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 name: Release
 
 on:
   release:
     types: [published]
-
   workflow_dispatch:
 
 env:
   FORCE_COLOR: "1"
 
 jobs:
   release:
@@ -28,11 +27,11 @@
         pip install --upgrade pip nox
         pip --version
         nox --version
     - name: Build package
       run: nox -s build
 
     - name: Upload package
-      uses: pypa/gh-action-pypi-publish@master
+      if: github.event_name == 'release'
+      uses: pypa/gh-action-pypi-publish@release/v1
       with:
-        user: __token__
-        password: ${{ secrets.PYPI_TOKEN }}
+        password: ${{ secrets.PYPI_TOKEN }}
```

### Comparing `aiooss2-0.2.3/LICENSE` & `aiooss2-0.2.4/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -174,23 +174,23 @@
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
 
    APPENDIX: How to apply the Apache License to your work.
 
       To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
+      boilerplate notice, with the fields enclosed by brackets "{}"
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2021 Iterative, Inc.
+   Copyright 2023 Yanxiang Gao.
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `aiooss2-0.2.3/PKG-INFO` & `aiooss2-0.2.4/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,29 @@
-Metadata-Version: 2.1
-Name: aiooss2
-Version: 0.2.3
-Summary: Async client for aliyun OSS
-Home-page: https://github.com/karajan1001/aiooss2
-Maintainer-email: mishanyo1001@gmail.com
-License: Apache-2.0
-Keywords: "oss,aio"
-Platform: any
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: dev
-License-File: LICENSE
-
 # aiooss2
 
 Async client for aliyun OSS(Object Storage Service) using oss2 and aiohttp_/asyncio_.
 
 The main purpose of this library is to support aliyun OSS async api, but other services
 should work (but maybe with minor fixes). For now, we have tested
 only upload/download/delete/list api for OSS. More functionality will be coming soon.
 
 # Install
 
 ```bash
-pip install aiooss22
+pip install aiooss2
 ```
 
 ## Basic Example
 -------------
 
 ```python
 import asyncio
 import os
 
-from aiooss22 import AioBucket, AioObjectIterator, Auth
+from aiooss2 import AioBucket, AioObjectIterator, Auth
 
 OSS_ACCESS_KEY_ID = os.environ.get('OSS_ACCESS_KEY_ID')
 OSS_SECRET_ACCESS_KEY = os.environ.get('OSS_SECRET_ACCESS_KEY')
 BUCKET_NAME = os.environ.get("OSS_TEST_BUCKET_NAME")
 
 
 async def async_go():
```

### Comparing `aiooss2-0.2.3/aiooss2/adapter.py` & `aiooss2-0.2.4/src/aiooss2/adapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Adapter (crc check and progress bar call backs) for data types
 """
 # pylint: disable=unnecessary-dunder-call
 import inspect
 import logging
 import os
 from abc import ABC, abstractmethod
-from typing import IO, AsyncIterator, Awaitable, Callable, Optional, Union
+from typing import IO, AsyncIterator, Callable, Optional, Union
 
 from aiohttp.abc import AbstractStreamWriter
 from aiohttp.payload import PAYLOAD_REGISTRY, TOO_LARGE_BYTES_BODY, Payload
 from oss2.compat import to_bytes
 from oss2.utils import (
     _CHUNK_SIZE,
     _invoke_cipher_callback,
@@ -53,25 +53,25 @@
         self.offset = 0
         self.size = size
         self.discard = discard
 
     def __aiter__(self) -> AsyncIterator:
         return self
 
-    async def __anext__(self) -> Awaitable[bytes]:
+    async def __anext__(self) -> bytes:
         content = await self.read(_CHUNK_SIZE)
         if content:
             return content
         raise StopAsyncIteration
 
-    def __len__(self) -> int:
+    def __len__(self) -> Optional[int]:
         return self.size
 
     @abstractmethod
-    async def read(self, amt=-1) -> Awaitable[bytes]:
+    async def read(self, amt=-1) -> bytes:
         """async api to read a chunk from the data
 
         Args:
             amt (int): batch size of the data to read, -1 to read all
         """
 
     @property
@@ -88,21 +88,17 @@
         real_discard = 0
         if self.offset < self.discard:
             real_discard = (
                 len(content) if len(content) <= self.discard else self.discard
             )
         self.discard -= real_discard
 
-        _invoke_progress_callback(
-            self.progress_callback, self.offset, self.size
-        )
+        _invoke_progress_callback(self.progress_callback, self.offset, self.size)
         _invoke_crc_callback(self.crc_callback, content, real_discard)
-        content = _invoke_cipher_callback(
-            self.cipher_callback, content, real_discard
-        )
+        content = _invoke_cipher_callback(self.cipher_callback, content, real_discard)
 
         return content
 
 
 class SliceableAdapter(StreamAdapter):
     """Adapter for data can get a slice via `stream[a:b]`"""
 
@@ -113,23 +109,23 @@
     ):
         """
         Args:
             size (Optional[int]):
                 size of the data stream.
         """
         super().__init__(stream, **kwargs)
-        self.size = self.size or len(stream)
+        self.size: int = self.size or len(stream)
 
     def _length_to_read(self, amt: int) -> int:
         length_to_read = self.size - self.offset
         if amt > 0:
             length_to_read = min(amt, length_to_read)
         return length_to_read
 
-    async def read(self, amt: int = -1) -> Awaitable[bytes]:
+    async def read(self, amt: int = -1) -> bytes:
         if self.offset >= self.size:
             return b""
         length_to_read = self._length_to_read(amt)
         content = self.stream[self.offset : self.offset + length_to_read]
         return self._invoke_callbacks(content)
 
 
@@ -144,24 +140,34 @@
                 position = self.stream.tell()
                 end = self.stream.seek(0, os.SEEK_END)
                 self.stream.seek(position)
                 self.size = end - position
             except AttributeError:
                 pass
 
-    async def read(self, amt: int = -1) -> Awaitable[bytes]:
-        if self._read_all:
+    def _length_to_read(self, amt: int) -> int:
+        if self.size is None:
+            return amt
+        length_to_read = self.size - self.offset
+        if amt > 0:
+            length_to_read = min(amt, length_to_read)
+        return length_to_read
+
+    async def read(self, amt: int = -1) -> bytes:
+        if self._read_all or (self.size and self.offset >= self.size):
             return b""
         if self.offset < self.discard and amt:
             amt += self.discard - self.offset
 
+        length_to_read = self._length_to_read(amt)
+
         if inspect.iscoroutinefunction(self.stream.read):
-            content = await self.stream.read(amt)
+            content = await self.stream.read(length_to_read)
         else:
-            content = self.stream.read(amt)
+            content = self.stream.read(length_to_read)
         if not content:
             self._read_all = True
         return self._invoke_callbacks(content)
 
 
 class IterableAdapter(StreamAdapter):
     """Adapter for Async Iterable data"""
@@ -170,19 +176,18 @@
         if hasattr(stream, "__aiter__"):
             stream = stream.__aiter__()
         elif hasattr(stream, "__iter__"):
             stream = iter(stream)
         super().__init__(stream, **kwargs)
         if discard:
             raise ValueError(
-                "discard not supported in Async "
-                f"Iterable input {self.stream}"
+                "discard not supported in Async " f"Iterable input {self.stream}"
             )
 
-    async def read(self, amt: int = -1) -> Awaitable[bytes]:
+    async def read(self, amt: int = -1) -> bytes:
         try:
             if hasattr(self.stream, "__anext__"):
                 content = await self.stream.__anext__()
             elif hasattr(self.stream, "__next__"):
                 content = next(self.stream)
             else:
                 raise AttributeError(
@@ -199,21 +204,18 @@
 
     _value: StreamAdapter
 
     async def write(self, writer: AbstractStreamWriter) -> None:
         chunk = await self._value.read()
         while chunk:
             if len(chunk) > TOO_LARGE_BYTES_BODY:
-                kwargs = {"source": self}
                 logger.warning(
                     "Sending a large body directly with raw bytes might"
                     " lock the event loop. You should probably pass an "
-                    "io.BytesIO object instead",
-                    ResourceWarning,
-                    **kwargs,
+                    "io.BytesIO object instead.",
                 )
             await writer.write(chunk)
             chunk = await self._value.read()
 
 
 PAYLOAD_REGISTRY.register(
     AsyncPayload, (SliceableAdapter, FilelikeObjectAdapter, IterableAdapter)
```

### Comparing `aiooss2-0.2.3/aiooss2/api.py` & `aiooss2-0.2.4/src/aiooss2/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Module for Bucket and Service
 """
 # pylint: disable=too-many-arguments
 # pylint: disable=too-many-instance-attributes
 
 import logging
-import shutil
 from typing import (
     TYPE_CHECKING,
     Callable,
     Dict,
     List,
+    Mapping,
     Optional,
     Sequence,
     Type,
     Union,
 )
 
 from oss2 import Bucket, defaults, models
@@ -24,38 +24,52 @@
 from oss2.headers import OSS_COPY_OBJECT_SOURCE
 from oss2.http import CaseInsensitiveDict
 from oss2.models import (
     AppendObjectResult,
     BatchDeleteObjectsResult,
     GetBucketInfoResult,
     GetObjectMetaResult,
+    HeadObjectResult,
+    InitMultipartUploadResult,
     ListBucketsResult,
+    ListMultipartUploadsResult,
     ListObjectsResult,
+    ListPartsResult,
     PutObjectResult,
     RequestResult,
 )
 from oss2.utils import (
     check_crc,
     content_md5,
     is_valid_bucket_name,
     is_valid_endpoint,
     set_content_type,
 )
 from oss2.xml_utils import (
     parse_batch_delete_objects,
+    parse_dummy_result,
     parse_get_bucket_info,
     parse_list_buckets,
     parse_list_objects,
     to_batch_delete_objects_request,
 )
 
 from .exceptions import make_exception
 from .http import AioSession, Request
 from .models import AioGetObjectResult
-from .utils import copyfileobj_and_verify, make_adapter
+from .multipart import (
+    abort_multipart_upload,
+    complete_multipart_upload,
+    init_multipart_upload,
+    list_multipart_uploads,
+    list_parts,
+    upload_part,
+    upload_part_copy,
+)
+from .utils import copyfileobj, copyfileobj_and_verify, make_adapter
 
 if TYPE_CHECKING:
     from oss2 import AnonymousAuth, Auth, StsAuth
 
     from .http import AioResponse
 
 logger = logging.getLogger(__name__)
@@ -73,31 +87,30 @@
         enable_crc: bool = True,
         proxies=None,
     ):
         """_summary_
 
         Args:
             auth (Union[Auth, AnonymousAuth, StsAuth]): Auth class.
-            endpoint (str): enpoint address or CNAME.
+            endpoint (str): endpoint address or CNAME.
             is_cname (bool): Whether the endpoint is a CNAME.
             session (Optional[AioSession], optional): reuse a custom session.
             connect_timeout (int): connection.
             app_name (str, optional): app name.
             enable_crc (bool, optional): enable crc check or not.
             proxies (_type_, optional): proxies settings.
 
         Raises:
             ClientError: _description_
         """
         self.auth = auth
         self.endpoint = _normalize_endpoint(endpoint.strip())
         if is_valid_endpoint(self.endpoint) is not True:
             raise ClientError(
-                "The endpoint you has specified is not valid, "
-                f"endpoint: {endpoint}"
+                "The endpoint you has specified is not valid, " f"endpoint: {endpoint}"
             )
         self.session = session
         self.timeout = connect_timeout or defaults.connect_timeout
         self.app_name = app_name
         self.enable_crc = enable_crc
         self.proxies = proxies
 
@@ -112,33 +125,30 @@
             enable_crc,
             proxies,
         )
 
     async def _do(
         self, method: str, bucket_name: str, key: Union[bytes, str], **kwargs
     ) -> "AioResponse":
-
         key = to_string(key)
         req = Request(
             method,
             self._make_url(bucket_name, key),
             app_name=self.app_name,
             **kwargs,
         )
         self.auth._sign_request(  # pylint: disable=protected-access
             req, bucket_name, key
         )
 
         assert self.session
-        resp: "AioResponse" = await self.session.do_request(
-            req, timeout=self.timeout
-        )
+        resp: "AioResponse" = await self.session.do_request(req, timeout=self.timeout)
 
         logger.debug(
-            "Responsed from the server, req_id: %s, status_code: %d",
+            "Responses from the server, req_id: %s, status_code: %d",
             resp.request_id,
             resp.status,
         )
 
         if resp.status // 100 != 2:
             err = await make_exception(resp)
             logger.info("Exception: %s", err)
@@ -156,34 +166,30 @@
         req = Request(
             method,
             sign_url,
             app_name=self.app_name,
             proxies=self.proxies,
             **kwargs,
         )
-        resp: "AioResponse" = await self.session.do_request(
-            req, timeout=self.timeout
-        )
+        resp: "AioResponse" = await self.session.do_request(req, timeout=self.timeout)
         if resp.status // 100 != 2:
             err = await make_exception(resp)
             logger.info("Exception: %s", err)
             raise err
 
         content_length = models._hget(  # pylint: disable=protected-access
             resp.headers, "content-length", int
         )
         if content_length is not None and content_length == 0:
             await resp.read()
 
         return resp
 
     @staticmethod
-    async def _parse_result(
-        resp: "AioResponse", parse_func: Callable, klass: Type
-    ):
+    async def _parse_result(resp: "AioResponse", parse_func: Callable, klass: Type):
         result = klass(resp)
         parse_func(result, await resp.read())
         return result
 
     async def __aenter__(self):
         if self.session is None:
             self.session = AioSession()
@@ -192,15 +198,15 @@
         return self
 
     async def __aexit__(self, *args):
         await self.session.close()
 
 
 class AioBucket(_AioBase):
-    """Used for Bucket and Object opertions, creating、deleting Bucket,
+    """Used for Bucket and Object operations, creating、deleting Bucket,
     uploading、downloading Object, etc。
     use case (bucket in HangZhou area)::
 
     >>> import oss2
     >>> import aiooss2
     >>> import asyncio
     >>> auth = oss2.Auth('your-access-key-id', 'your-access-key-secret')
@@ -228,63 +234,65 @@
     ):
         """
         Args:
             bucket_name (str): the bucket name to operate
         """
         self.bucket_name = bucket_name.strip()
         if is_valid_bucket_name(self.bucket_name) is not True:
-            raise ClientError("The bucket_name is invalid, please check it.")
+            raise ClientError(
+                f"The bucket_name '{self.bucket_name}' is invalid, please check it."
+            )
         super().__init__(
             auth,
             endpoint,
             is_cname,
             **kwargs,
         )
 
-    async def __do_object(
+    async def _do_object(
         self, method: str, key: Union[bytes, str], **kwargs
     ) -> "AioResponse":
         return await self._do(method, self.bucket_name, key, **kwargs)
 
-    async def __do_bucket(self, method: str, **kwargs) -> "AioResponse":
+    async def _do_bucket(self, method: str, **kwargs) -> "AioResponse":
         return await self._do(method, self.bucket_name, "", **kwargs)
 
     async def put_object(
         self,
         key: str,
         data,
-        headers: Optional[Dict] = None,
+        headers: Optional[Mapping] = None,
         progress_callback: Optional[Callable] = None,
     ) -> "PutObjectResult":
         """upload some contents to an object
 
         (use case) ::
             >>> await bucket.put_object('readme.txt', 'content of readme.txt')
             >>> with open(u'local_file.txt', 'rb') as f:
             >>>     await bucket.put_object('remote_file.txt', f)
 
         Args:
             key (str): object name to upload
             data (Union[str, bytes, IO, Iterable]): contents to upload
-            headers (Optional[Dict], optional): HTTP headers to specify.
+            headers (Optional[Mapping], optional): HTTP headers to specify.
             progress_callback (Optional[Callable], optional): callback function
                 for progress bar.
 
         Returns:
             PutObjectResult:
         """
         headers = set_content_type(CaseInsensitiveDict(headers), key)
 
         data = make_adapter(
             data,
             progress_callback=progress_callback,
             enable_crc=self.enable_crc,
         )
 
-        resp: "AioResponse" = await self.__do_object(
+        resp: "AioResponse" = await self._do_object(
             "PUT", key, data=data, headers=headers
         )
         logger.debug("Put object done")
         result = PutObjectResult(resp)
 
         if self.enable_crc and result.crc is not None:
             check_crc("put object", data.crc, result.crc, result.request_id)
@@ -294,15 +302,15 @@
     async def get_object(  # pylint: disable=too-many-arguments
         self,
         key: str,
         byte_range: Optional[Sequence[Optional[int]]] = None,
         headers: Optional[dict] = None,
         progress_callback: Optional[Callable] = None,
         process=None,
-        params: Optional[Dict] = None,
+        params: Optional[Union[Dict, CaseInsensitiveDict]] = None,
     ) -> AioGetObjectResult:
         """download the contents of an object
 
         (use case) ::
             >>> async with await bucket.get_object("helloword") as result
             >>>     print(await result.read())
             'hello world'
@@ -311,33 +319,31 @@
             key (str): object name to download.
             byte_range (Optional[Sequence[Optional[int]]], optional):
                 Range to download.
             headers (Optional[dict], optional): HTTP headers to specify.
             progress_callback (Optional[Callable], optional): callback function
                 for progress bar.
             process (_type_, optional): oss file process method.
-            params (Optional[Dict], optional):
+            params (Optional[Union[Dict, CaseInsensitiveDict]], optional):
 
         Returns:
             AioGetObjectResult:
         """
 
         headers_dict: CaseInsensitiveDict = CaseInsensitiveDict(headers)
 
         range_string = _make_range_string(byte_range)
         if range_string:
             headers_dict["range"] = range_string
 
         params = {} if params is None else params
         if process:
-            params.update({Bucket.PROCESS: process})
+            params[Bucket.PROCESS] = process
 
-        resp = await self.__do_object(
-            "GET", key, headers=headers_dict, params=params
-        )
+        resp = await self._do_object("GET", key, headers=headers_dict, params=params)
         logger.debug("Get object done")
 
         return AioGetObjectResult(resp, progress_callback, self.enable_crc)
 
     async def delete_object(
         self,
         key: str,
@@ -361,17 +367,15 @@
             headers (Optional[Dict], optional): HTTP headers to specify.
             params (Union[Dict, CaseInsensitiveDict], optional):
 
         Returns:
             RequestResult:
         """
 
-        resp = await self.__do_object(
-            "DELETE", key, params=params, headers=headers
-        )
+        resp = await self._do_object("DELETE", key, params=params, headers=headers)
         logger.debug("Delete object done")
         return RequestResult(resp)
 
     async def list_objects(  # pylint: disable=too-many-arguments
         self,
         prefix: str = "",
         delimiter: str = "",
@@ -394,30 +398,28 @@
             max_keys (int, optional): numbers of objects for one page.
             headers (Optional[Dict], optional): HTTP headers to specify.
 
         Returns:
             ListObjectsResult:
         """
         headers = CaseInsensitiveDict(headers)
-        resp = await self.__do_object(
+        resp = await self._do_object(
             "GET",
             "",
             params={
                 "prefix": prefix,
                 "delimiter": delimiter,
                 "marker": marker,
                 "max-keys": str(max_keys),
                 "encoding-type": "url",
             },
             headers=headers,
         )
         logger.debug("List objects done")
-        return await self._parse_result(
-            resp, parse_list_objects, ListObjectsResult
-        )
+        return await self._parse_result(resp, parse_list_objects, ListObjectsResult)
 
     async def get_object_meta(
         self,
         key: str,
         params: Optional[Union[dict, CaseInsensitiveDict]] = None,
         headers: Optional[Dict] = None,
     ) -> "GetObjectMetaResult":
@@ -440,23 +442,19 @@
 
         if params is None:
             params = {}
 
         if Bucket.OBJECTMETA not in params:
             params[Bucket.OBJECTMETA] = ""
 
-        resp = await self.__do_object(
-            "GET", key, params=params, headers=headers
-        )
+        resp = await self._do_object("GET", key, params=params, headers=headers)
         logger.debug("Get object metadata done")
         return GetObjectMetaResult(resp)
 
-    async def object_exists(
-        self, key: str, headers: Optional[Dict] = None
-    ) -> bool:
+    async def object_exists(self, key: str, headers: Optional[Dict] = None) -> bool:
         """Return True if key exists, False otherwise. raise Exception
         for other exceptions.
 
         (use case) ::
             >>> result = await bucket.object_exists('object1')
             >>> print(result)
             True
@@ -474,25 +472,25 @@
             await self.get_object_meta(key, headers=headers)
         except NoSuchKey:
             return False
 
         return True
 
     async def get_bucket_info(self) -> GetBucketInfoResult:
-        """Get bucket infomation, `Create time`, `Endpoint`, `Owner`, `ACL`
+        """Get bucket information, `Create time`, `Endpoint`, `Owner`, `ACL`
 
         (use case) ::
             >>> resp = await aiobucket.get_bucket_info()
             >>> print(resp.name)
             'bucket_name'
 
         Returns:
             GetBucketInfoResult
         """
-        resp = await self.__do_bucket("GET", params={Bucket.BUCKET_INFO: ""})
+        resp = await self._do_bucket("GET", params={Bucket.BUCKET_INFO: ""})
         logger.debug("Get bucket info done")
         return await self._parse_result(
             resp, parse_get_bucket_info, GetBucketInfoResult
         )
 
     async def append_object(
         self,
@@ -530,15 +528,15 @@
 
         data = make_adapter(
             data,
             progress_callback=progress_callback,
             enable_crc=self.enable_crc,
         )
 
-        resp = await self.__do_object(
+        resp = await self._do_object(
             "POST",
             key,
             data=data,
             headers=headers,
             params={"append": "", "position": str(position)},
         )
         logger.debug("Append object done")
@@ -549,33 +547,33 @@
 
         return result
 
     async def put_object_from_file(
         self,
         key: str,
         filename: str,
-        headers: Optional[Dict] = None,
+        headers: Optional[Mapping] = None,
         progress_callback: Optional[Callable] = None,
     ) -> "PutObjectResult":
         """Upload a local file to a oss key
 
         (use case) ::
             >>> with open("file") as f:
             >>>     print(f.read())
-            "hellow world"
+            "hello world"
             >>> result = await aiobucket.put_object_from_file("object1",
                 "file")
             >>> async with await bucket.get_object("object1") as result
             >>>     print(await result.read())
             'hello world'
 
         Args:
             key (str): key of the oss
             filename (str): filename to upload
-            headers (Optional[Dict], optional): HTTP headers to specify.
+            headers (Optional[Mapping], optional): HTTP headers to specify.
             progress_callback (Optional[Callable], optional): callback function
                 for progress bar.
 
         Returns:
             _type_: _description_
         """
         headers = set_content_type(CaseInsensitiveDict(headers), filename)
@@ -591,34 +589,34 @@
         self,
         key: str,
         filename: str,
         byte_range: Optional[Sequence[int]] = None,
         headers: Optional[Union[Dict, CaseInsensitiveDict]] = None,
         progress_callback: Optional[Callable] = None,
         process: Optional[Callable] = None,
-        params: Optional[Dict] = None,
+        params: Optional[Union[Dict, CaseInsensitiveDict]] = None,
     ) -> AioGetObjectResult:
         """Download contents of object to file.
 
         (use case) ::
             >>> result = await aiobucket.get_object_to_file("object1", "file")
             >>> with open("file") as f:
             >>>     print(f.read())
-            "hellow world"
+            "hello world"
 
         Args:
             key (str): object name to download.
             filename (str): filename to save the data downloaded.
             byte_range (Optional[Sequence[Optional[int]]], optional):
                 Range to download.
             headers (Optional[dict], optional): HTTP headers to specify.
             progress_callback (Optional[Callable], optional): callback function
                 for progress bar.
             process (_type_, optional): oss file process method.
-            params (Optional[Dict], optional):
+            params (Optional[Union[Dict, CaseInsensitiveDict]], optional):
 
         Returns:
             AioGetObjectResult:
         """
         with open(to_unicode(filename), "wb") as f_w:
             result = await self.get_object(
                 key,
@@ -626,15 +624,15 @@
                 headers=headers,
                 progress_callback=progress_callback,
                 process=process,
                 params=params,
             )
 
             if result.content_length is None:
-                shutil.copyfileobj(result, f_w)
+                copyfileobj(result, f_w)
             else:
                 await copyfileobj_and_verify(
                     result,
                     f_w,
                     result.content_length,
                     request_id=result.request_id,
                 )
@@ -687,23 +685,23 @@
             BatchDeleteObjectResult:
         """
         if not key_list:
             raise ClientError("key_list should not be empty")
 
         data = to_batch_delete_objects_request(key_list, False)
 
-        headers = CaseInsensitiveDict(headers)
-        headers["Content-MD5"] = content_md5(data)
+        header_dict: CaseInsensitiveDict = CaseInsensitiveDict(headers)
+        header_dict["Content-MD5"] = content_md5(data)
 
-        resp = await self.__do_object(
+        resp = await self._do_object(
             "POST",
             "",
             data=data,
             params={"delete": "", "encoding-type": "url"},
-            headers=headers,
+            headers=header_dict,
         )
         return await self._parse_result(
             resp, parse_batch_delete_objects, BatchDeleteObjectsResult
         )
 
     async def copy_object(
         self,
@@ -749,18 +747,97 @@
                 + params[Bucket.VERSIONID]
             )
         else:
             headers[OSS_COPY_OBJECT_SOURCE] = (
                 "/" + source_bucket_name + "/" + urlquote(source_key, "")
             )
 
-        resp = await self.__do_object("PUT", target_key, headers=headers)
+        resp = await self._do_object("PUT", target_key, headers=headers)
 
         return PutObjectResult(resp)
 
+    async def head_object(
+        self,
+        key: str,
+        headers: Optional[Union[Dict, CaseInsensitiveDict]] = None,
+        params: Optional[Mapping] = None,
+    ) -> "HeadObjectResult":
+        """Get object metadata
+
+            >>> result = bucket.head_object('readme.txt')
+            >>> print(result.content_type)
+            text/plain
+
+        Args:
+            key (str): object key
+            headers (Optional[Union[Dict, CaseInsensitiveDict]], optional):
+                HTTP headers to specify.
+            params (Optional[Mapping], optional):
+
+        Returns:
+            HeadObjectResult:
+
+        Raises:
+            `NotFound <oss2.exceptions.NotFound>` if object does not exist.
+        """
+
+        logger.debug(
+            "Start to head object, bucket: %s, key: %s, headers: %s",
+            self.bucket_name,
+            to_string(key),
+            headers,
+        )
+
+        resp = await self._do_object("HEAD", key, headers=headers, params=params)
+
+        logger.debug(
+            "Head object done, req_id: %s, status_code: %s",
+            resp.request_id,
+            resp.status,
+        )
+        return await self._parse_result(resp, parse_dummy_result, HeadObjectResult)
+
+    async def abort_multipart_upload(
+        self: "AioBucket", *args, **kwargs
+    ) -> RequestResult:
+        """abort multipart uploading process"""
+        return await abort_multipart_upload(self, *args, **kwargs)
+
+    async def complete_multipart_upload(
+        self: "AioBucket", *args, **kwargs
+    ) -> PutObjectResult:
+        """Complete multipart uploading process create a new file."""
+        return await complete_multipart_upload(self, *args, **kwargs)
+
+    async def init_multipart_upload(
+        self: "AioBucket", *args, **kwargs
+    ) -> InitMultipartUploadResult:
+        """initialize multipart uploading
+        The returning upload id, bucket name and object name together
+        defines this uploading event."""
+        return await init_multipart_upload(self, *args, **kwargs)
+
+    async def list_multipart_uploads(
+        self: "AioBucket", *args, **kwargs
+    ) -> ListMultipartUploadsResult:
+        """List multipart uploading process"""
+        return await list_multipart_uploads(self, *args, **kwargs)
+
+    async def list_parts(self: "AioBucket", *args, **kwargs) -> ListPartsResult:
+        """list uploaded parts in a part uploading progress."""
+        return await list_parts(self, *args, **kwargs)
+
+    async def upload_part(self: "AioBucket", *args, **kwargs) -> PutObjectResult:
+        """upload single part."""
+        return await upload_part(self, *args, **kwargs)
+
+    async def upload_part_copy(self: "AioBucket", *args, **kwargs) -> PutObjectResult:
+        """copy part or whole of a source file to a slice of a target file."""
+        return await upload_part_copy(self, *args, **kwargs)
+
 
 # pylint: disable=too-few-public-methods
 class AioService(_AioBase):
     """Service class used for operations like list all bucket"""
 
     def __init__(
         self,
@@ -771,15 +848,15 @@
         app_name: str = "",
         proxies=None,
     ):
         """_summary_
 
         Args:
             auth (Union[Auth, AnonymousAuth, StsAuth]): Auth class.
-            endpoint (str): enpoint address or CNAME.
+            endpoint (str): endpoint address or CNAME.
             session (Optional[AioSession], optional): reuse a custom session.
             connect_timeout (int): connection.
             app_name (str, optional): app name.
             proxies (_type_, optional): proxies settings.
         """
         super().__init__(
             auth,
@@ -826,10 +903,8 @@
             if "tag-key" in params:
                 list_param["tag-key"] = params["tag-key"]
             if "tag-value" in params:
                 list_param["tag-value"] = params["tag-value"]
 
         resp = await self._do("GET", "", "", params=list_param)
         logger.debug("List buckets done")
-        return await self._parse_result(
-            resp, parse_list_buckets, ListBucketsResult
-        )
+        return await self._parse_result(resp, parse_list_buckets, ListBucketsResult)
```

### Comparing `aiooss2-0.2.3/aiooss2/http.py` & `aiooss2-0.2.4/src/aiooss2/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,16 @@
         self.proxies = proxies
 
         if not isinstance(headers, CaseInsensitiveDict):
             self.headers = CaseInsensitiveDict(headers)
         else:
             self.headers = headers
 
-        self.headers["Content-Type"] = "application/octet-stream"
+        if "Content-Type" not in self.headers:
+            self.headers["Content-Type"] = "application/octet-stream"
         if "User-Agent" not in self.headers:
             if app_name:
                 self.headers["User-Agent"] = USER_AGENT + "/" + app_name
             else:
                 self.headers["User-Agent"] = USER_AGENT
 
         logger.debug(
```

### Comparing `aiooss2-0.2.3/aiooss2/iterators.py` & `aiooss2-0.2.4/src/aiooss2/iterators.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 """
 Contains some useful iteraotrs, can be used to iterate buckets、
 files or file parts etc.
 """
 # pylint: disable=too-many-arguments
-from typing import TYPE_CHECKING, Dict, Optional
+from typing import TYPE_CHECKING, Dict, List, Optional
 
 from oss2 import defaults, http
 from oss2.models import ListObjectsResult, SimplifiedObjectInfo
 
 from .exceptions import ServerError
 
 if TYPE_CHECKING:
+    from oss2.models import SimplifiedBucketInfo
+    from oss2.resumable import PartInfo
+
     from .api import AioBucket, AioService
 
 
 class _AioBaseIterator:
-    def __init__(self, marker: str, max_retries: Optional[str]):
+    def __init__(self, marker: str, max_retries: Optional[int]):
         self.is_truncated = True
         self.next_marker = marker
 
         max_retries = max_retries or defaults.request_retries
         self.max_retries = max_retries if max_retries > 0 else 1
 
-        self.entries = []
+        self.entries: List = []
 
     async def _fetch(self):
         raise NotImplementedError
 
     def __aiter__(self):
         return self
 
@@ -93,23 +96,22 @@
         self.bucket = bucket
         self.prefix = prefix
         self.delimiter = delimiter
         self.max_keys = max_keys
         self.headers = http.CaseInsensitiveDict(headers)
 
     async def _fetch(self):
-
         result: ListObjectsResult = await self.bucket.list_objects(
             prefix=self.prefix,
             delimiter=self.delimiter,
             marker=self.next_marker,
             max_keys=self.max_keys,
             headers=self.headers,
         )
-        self.entries = result.object_list + [
+        self.entries: List["SimplifiedObjectInfo"] = result.object_list + [
             SimplifiedObjectInfo(prefix, None, None, None, None, None)
             for prefix in result.prefix_list
         ]
         self.entries.sort(key=lambda obj: obj.key)
         return result.is_truncated, result.next_marker
 
 
@@ -141,10 +143,55 @@
         self.prefix = prefix
         self.max_keys = max_keys
 
     async def _fetch(self):
         result = await self.service.list_buckets(
             prefix=self.prefix, marker=self.next_marker, max_keys=self.max_keys
         )
-        self.entries = result.buckets
+        self.entries: List["SimplifiedBucketInfo"] = result.buckets
+
+        return result.is_truncated, result.next_marker
+
+
+class AioPartIterator(_AioBaseIterator):
+    """Iterator over all parts from a partial upload session"""
+
+    def __init__(
+        self,
+        bucket: "AioBucket",
+        key: str,
+        upload_id: str,
+        marker: str = "0",
+        max_parts: int = 1000,
+        max_retries: Optional[int] = None,
+        headers: Optional[Dict] = None,
+    ):
+        """
+
+        Args:
+            bucket (AioBucket): bucket to operate.
+            key (str): key of the object.
+            upload_id (str): upload id of the partial upload session.
+            marker (str, optional): paginate separator.
+            max_parts (int, optional): key number returns from `list_parts`
+            max_retries (Optional[int], optional): max retry count.
+            headers (Optional[Dict], optional): HTTP header.
+        """
+        super().__init__(marker, max_retries)
+
+        self.bucket = bucket
+        self.key = key
+        self.upload_id = upload_id
+        self.max_parts = max_parts
+        self.headers = http.CaseInsensitiveDict(headers)
+
+    async def _fetch(self):
+        result = await self.bucket.list_parts(
+            self.key,
+            self.upload_id,
+            marker=self.next_marker,
+            max_parts=self.max_parts,
+            headers=self.headers,
+        )
+        self.entries: List["PartInfo"] = result.parts
 
         return result.is_truncated, result.next_marker
```

### Comparing `aiooss2-0.2.3/aiooss2/models.py` & `aiooss2-0.2.4/src/aiooss2/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Module for all input and output classes for the Python SDK API
 """
 import copy
 import logging
-from typing import TYPE_CHECKING, Awaitable, Optional
+from typing import TYPE_CHECKING
 
 from oss2.exceptions import ClientError
 from oss2.headers import (
     DEPRECATED_CLIENT_SIDE_ENCRYPTION_KEY,
     KMS_ALI_WRAP_ALGORITHM,
     OSS_CLIENT_SIDE_ENCRYPTION_KEY,
 )
@@ -67,37 +67,29 @@
         content_crypto_material = ContentCryptoMaterial(
             self.__crypto_provider.cipher, self.__crypto_provider.wrap_alg
         )
         content_crypto_material.from_object_meta(self.resp.headers)
 
         if content_crypto_material.is_unencrypted():
             logger.info(
-                "The object is not encrypted, "
-                "use crypto provider is not recommended"
+                "The object is not encrypted, use crypto provider is not recommended"
             )
         else:
             crypto_provider = self.__crypto_provider
-            if (
-                content_crypto_material.mat_desc
-                != self.__crypto_provider.mat_desc
-            ):
+            if content_crypto_material.mat_desc != self.__crypto_provider.mat_desc:
                 logger.warning(
                     "The material description of the object "
                     "and the provider is inconsistent"
                 )
-                encryption_materials = (
-                    self.__crypto_provider.get_encryption_materials(
-                        content_crypto_material.mat_desc
-                    )
+                encryption_materials = self.__crypto_provider.get_encryption_materials(
+                    content_crypto_material.mat_desc
                 )
                 if encryption_materials:
-                    crypto_provider = (
-                        self.__crypto_provider.reset_encryption_materials(
-                            encryption_materials
-                        )
+                    crypto_provider = self.__crypto_provider.reset_encryption_materials(
+                        encryption_materials
                     )
                 else:
                     raise ClientError(
                         "There is no encryption materials "
                         "match the material description of the object"
                     )
 
@@ -120,17 +112,15 @@
             else:
                 plain_iv = crypto_provider.decrypt_encrypted_iv(
                     content_crypto_material.encrypted_iv
                 )
 
             offset = 0
             if self.content_range:
-                start, _ = crypto_provider.adjust_range(
-                    byte_range[0], byte_range[1]
-                )
+                start, _ = crypto_provider.adjust_range(byte_range[0], byte_range[1])
                 offset = content_crypto_material.cipher.calc_offset(start)
 
             cipher = copy.copy(content_crypto_material.cipher)
             if content_crypto_material.deprecated:
                 cipher.initial_by_counter(plain_key, plain_counter + offset)
             else:
                 cipher.initialize(plain_key, plain_iv, offset)
@@ -162,17 +152,17 @@
     @property
     def client_crc(self):
         """the client crc"""
         if self.__crc_enabled:
             return self.stream.crc
         return None
 
-    async def read(self, amt: Optional[int] = None) -> Awaitable[bytes]:
+    async def read(self, amt: int = -1) -> bytes:
         """async read data from stream
 
         Args:
-            amt (int, optional): batch size of the data to read
+            amt int: batch size of the data to read
 
         Returns:
         Awaitable[bytes]:
         """
         return await self.stream.read(amt)
```

### Comparing `aiooss2-0.2.3/aiooss2/utils.py` & `aiooss2-0.2.4/src/aiooss2/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """
 Utils used in project.
 """
 import logging
+import os
 from typing import Callable, Optional
 
 from oss2.compat import to_bytes
 from oss2.exceptions import ClientError, InconsistentError
 from oss2.utils import Crc64
 
 from aiooss2.adapter import (
     FilelikeObjectAdapter,
     IterableAdapter,
     SliceableAdapter,
     StreamAdapter,
 )
 
+COPY_BUFSIZE = 1024 * 1024 if os.name == "nt" else 64 * 1024
+
 logger = logging.getLogger(__name__)
 
 
 async def copyfileobj_and_verify(
     fsrc, fdst, expected_len, chunk_size=16 * 1024, request_id=""
 ):
     """copy data from file-like object fsrc to file-like object fdst,
@@ -77,23 +80,34 @@
         "progress_callback": progress_callback,
         "crc_callback": crc_callback,
         "discard": discard,
         "size": size,
     }
 
     if isinstance(stream, (bytes, bytearray, memoryview)):
-        adapter = SliceableAdapter(**params)
-    elif hasattr(stream, "read"):
-        adapter = FilelikeObjectAdapter(**params)
-    elif (
+        return SliceableAdapter(**params)
+    if hasattr(stream, "read"):
+        return FilelikeObjectAdapter(**params)
+    if (
         hasattr(stream, "__aiter__")
         or hasattr(stream, "__iter__")
         or hasattr(stream, "__next__")
         or hasattr(stream, "__anext__")
     ):
-        adapter = IterableAdapter(**params)
-    else:
-        raise ClientError(
-            f"{stream.__class__.__name__} is neither a string nor bytes "
-            "nor a file object nor an iterator"
-        )
-    return adapter
+        return IterableAdapter(**params)
+    raise ClientError(
+        f"{stream.__class__.__name__} is neither a string nor bytes "
+        "nor a file object nor an iterator"
+    )
+
+
+async def copyfileobj(fsrc, fdst, length=0):
+    """copy data from file-like object fsrc to file-like object fdst"""
+    if not length:
+        length = COPY_BUFSIZE
+    fsrc_read = fsrc.read
+    fdst_write = fdst.write
+    while True:
+        buf = await fsrc_read(length)
+        if not buf:
+            break
+        fdst_write(buf)
```

### Comparing `aiooss2-0.2.3/examples/simple.py` & `aiooss2-0.2.4/examples/simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     folder = "readme"
     data_obj = f"{folder}/{obj_name}"
 
     auth = Auth(OSS_ACCESS_KEY_ID, OSS_SECRET_ACCESS_KEY)
     async with AioBucket(
         auth, "http://oss-cn-hangzhou.aliyuncs.com", BUCKET_NAME
     ) as bucket:
-
         # upload object to oss
         data = b"\x01" * 1024
         resp = await bucket.put_object(data_obj, data)
 
         # download object to oss
         async with await bucket.get_object(data_obj) as resp:
             assert await resp.read() == data
```

### Comparing `aiooss2-0.2.3/noxfile.py` & `aiooss2-0.2.4/noxfile.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,53 @@
 """Automation using nox."""
-# pylint: disable=missing-function-docstring
 import glob
 import os
 
 import nox
 
 nox.options.reuse_existing_virtualenvs = True
 nox.options.sessions = "lint", "tests"
 locations = "src", "tests"
 
 
-@nox.session(python=["3.7", "3.8", "3.9", "3.10", "pypy-3.8", "pypy-3.9"])
+@nox.session
+def docs(session: nox.Session) -> None:
+    session.install(".[docs]")
+    session.run("mkdocs", "build")
+
+
+@nox.session(python=["3.8", "3.9", "3.10", "3.11", "pypy3.8", "pypy3.9"])
 def tests(session: nox.Session) -> None:
     session.install(".[tests]")
     session.run(
         "pytest",
-        "tests",
+        "--cov",
+        "--cov-config=pyproject.toml",
+        "--durations",
+        "100",
         *session.posargs,
+        env={"COVERAGE_FILE": f".coverage.{session.python}"},
     )
 
 
 @nox.session
 def lint(session: nox.Session) -> None:
     session.install("pre-commit")
     session.install("-e", ".[dev]")
 
     args = *(session.posargs or ("--show-diff-on-failure",)), "--all-files"
     session.run("pre-commit", "run", *args)
+    session.run("python", "-m", "mypy")
+    session.run("python", "-m", "pylint", *locations)
 
 
 @nox.session
 def safety(session: nox.Session) -> None:
     """Scan dependencies for insecure packages."""
-    session.install(".")
+    session.install(".[dev]")
     session.install("safety")
     session.run("safety", "check", "--full-report")
 
 
 @nox.session
 def build(session: nox.Session) -> None:
     session.install("build", "setuptools", "twine")
```

### Comparing `aiooss2-0.2.3/tests/conftest.py` & `aiooss2-0.2.4/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,24 @@
 Pytest setup
 """
 # pylint: disable=missing-function-docstring
 # pylint: disable=redefined-outer-name
 import os
 import pathlib
 import subprocess
-import time
 import uuid
 
 import pytest
 import requests
 from oss2 import Bucket, Service
 
 from aiooss2 import AioBucket, AioService, Auth
 
 PORT = 5555
-LICENSE_PATH = os.path.join(
-    pathlib.Path(__file__).parent.parent.resolve(), "LICENSE"
-)
+LICENSE_PATH = os.path.join(pathlib.Path(__file__).parent.parent.resolve(), "LICENSE")
 NUMBERS = b"1234567890\n"
 
 
 @pytest.fixture(scope="session")
 def access_key_id():
     return os.environ.get("OSS_ACCESS_KEY_ID", "")
 
@@ -41,15 +38,15 @@
 def bucket_name():
     return os.environ.get("OSS_TEST_BUCKET_NAME")
 
 
 @pytest.fixture(scope="session")
 def test_directory():
     test_id = uuid.uuid4()
-    return f"ossfs_test/{test_id}"
+    return f"aiooss2_test/{test_id}"
 
 
 @pytest.fixture(scope="session")
 def test_full_path(bucket_name, test_directory):
     return f"/{bucket_name}/{test_directory}"
 
 
@@ -60,26 +57,20 @@
 
 @pytest.fixture()
 def oss_emulator_server_start(emulator_endpoint):
     """
     Start a local emulator server
     """
     with subprocess.Popen(f"ruby bin/emulator -r store -p {PORT}"):
-
-        timeout = 5
-        while timeout > 0:
-            try:
-                result = requests.get(emulator_endpoint)
-                if result.ok:
-                    break
-            except Exception as err:
-                raise Exception("emulator start timeout") from err
-            timeout -= 0.1
-            time.sleep(0.1)
-        yield
+        try:
+            result = requests.get(emulator_endpoint, timeout=5)
+            if result.ok:
+                yield
+        except TimeoutError as err:
+            raise Exception("emulator start timeout") from err
 
 
 @pytest.fixture(scope="session")
 def auth(access_key_id, access_key_secret):
     return Auth(access_key_id, access_key_secret)
```

### Comparing `aiooss2-0.2.3/tests/func/test_bucket.py` & `aiooss2-0.2.4/tests/func/test_bucket.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 """
-Basic tests for aiooss2
+Basic tests for bucket operations.
 """
 # pylint: disable=missing-function-docstring
 import asyncio
 from typing import TYPE_CHECKING
 
 from oss2 import BucketIterator
 
 from aiooss2 import AioBucketIterator
 
 if TYPE_CHECKING:
-
     from oss2 import Service
 
     from aiooss2 import AioService
 
 
-def test_list_bucket(
-    service: "AioService", oss2_service: "Service", bucket_name
-):
+def test_list_bucket(service: "AioService", oss2_service: "Service", bucket_name):
     async def list_bucket():
         async with service as aioservice:
             result = []
             async for obj in AioBucketIterator(aioservice):
                 result.append(obj.name)
             return result
```

### Comparing `aiooss2-0.2.3/tests/func/test_object.py` & `aiooss2-0.2.4/tests/func/test_object.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Basic tests for aiooss2
+Functional tests for object operations.
 """
 # pylint: disable=missing-function-docstring
 import asyncio
 import inspect
 import os
 from typing import TYPE_CHECKING
 
@@ -36,30 +36,28 @@
 
     async def put(object_name, data):
         async with bucket as aiobucket:
             return await aiobucket.put_object(object_name, data)
 
     bucket.enable_crc = enable_crc
     result = asyncio.run(put(object_name, data))
-    bucket.enable_crc = not enable_crc
     assert result.resp.status == 200
     assert oss2_bucket.get_object(object_name).read() == data
 
 
 @pytest.mark.parametrize("enable_crc", [True, False])
 def test_get_object(bucket: "AioBucket", number_file, enable_crc: bool):
     async def get(object_name):
         async with bucket as aiobucket:
             resp = await aiobucket.get_object(object_name)
             async with resp as result:
                 return await result.read()
 
     bucket.enable_crc = enable_crc
     result = asyncio.run(get(number_file))
-    bucket.enable_crc = not enable_crc
     assert result == NUMBERS
 
 
 def test_list_objects(bucket: "AioBucket", oss2_bucket: "Bucket", test_path):
     data = b"\x01" * 2
     function_name = inspect.stack()[0][0].f_code.co_name
     object_path = f"{test_path}/{function_name}"
@@ -82,34 +80,28 @@
 
 def test_delete_object(bucket: "AioBucket", oss2_bucket: "Bucket", test_path):
     data = b"\x01" * 1024
     function_name = inspect.stack()[0][0].f_code.co_name
     object_name = f"{test_path}/{function_name}"
 
     oss2_bucket.put_object(object_name, data)
-    file_list = [
-        obj.key for obj in ObjectIterator(oss2_bucket, prefix=object_name)
-    ]
+    file_list = [obj.key for obj in ObjectIterator(oss2_bucket, prefix=object_name)]
     assert object_name in file_list
 
     async def delete_obj(object_name):
         async with bucket as aiobucket:
             return await aiobucket.delete_object(object_name)
 
     asyncio.run(delete_obj(object_name))
 
-    file_list = [
-        obj.key for obj in ObjectIterator(oss2_bucket, prefix=object_name)
-    ]
+    file_list = [obj.key for obj in ObjectIterator(oss2_bucket, prefix=object_name)]
     assert object_name not in file_list
 
 
-def test_get_object_meta(
-    bucket: "AioBucket", oss2_bucket: "Bucket", number_file
-):
+def test_get_object_meta(bucket: "AioBucket", oss2_bucket: "Bucket", number_file):
     async def get_object_meta(object_name):
         async with bucket as aiobucket:
             return await aiobucket.get_object_meta(object_name)
 
     result = asyncio.run(get_object_meta(number_file))
     expected = oss2_bucket.get_object_meta(number_file)
     assert expected.content_length == result.content_length
@@ -177,15 +169,14 @@
 
     async def put_object_from_file(object_name, file):
         async with bucket as aiobucket:
             return await aiobucket.put_object_from_file(object_name, file)
 
     bucket.enable_crc = enable_crc
     result = asyncio.run(put_object_from_file(object_name, str(file)))
-    bucket.enable_crc = not enable_crc
     assert result.resp.status == 200
     assert oss2_bucket.get_object(object_name).read() == data
 
 
 @pytest.mark.parametrize("enable_crc", [True, False])
 def test_get_object_to_file(
     tmpdir: "local", bucket: "AioBucket", number_file, enable_crc: bool
@@ -196,21 +187,18 @@
         async with bucket as aiobucket:
             resp = await aiobucket.get_object_to_file(object_name, file)
             async with resp as result:
                 return await result.read()
 
     bucket.enable_crc = enable_crc
     asyncio.run(get_object_to_file(number_file, str(file)))
-    bucket.enable_crc = not enable_crc
     assert file.read_binary() == NUMBERS
 
 
-def test_batch_delete_objects(
-    bucket: "AioBucket", oss2_bucket: "Bucket", test_path
-):
+def test_batch_delete_objects(bucket: "AioBucket", oss2_bucket: "Bucket", test_path):
     data = b"\x01" * 2
     function_name = inspect.stack()[0][0].f_code.co_name
     object_path = f"{test_path}/{function_name}"
     deleted = []
     expected = []
     for i in range(10):
         obj = f"{object_path}/{i}"
@@ -242,17 +230,17 @@
     object_path = f"{test_path}/{function_name}"
 
     async def copy_objects(file_from, file_to):
         async with bucket as aiobucket:
             return await aiobucket.copy_object(bucket_name, file_from, file_to)
 
     asyncio.run(copy_objects(number_file, object_path))
-    assert [
-        obj.key for obj in ObjectIterator(oss2_bucket, prefix=object_path)
-    ] == [object_path]
+    assert [obj.key for obj in ObjectIterator(oss2_bucket, prefix=object_path)] == [
+        object_path
+    ]
     assert oss2_bucket.get_object(object_path).read() == NUMBERS
 
 
 def test_put_object_from_middle_of_file(
     tmpdir: "local", bucket: "AioBucket", oss2_bucket: "Bucket", test_path
 ):
     data = b"1234567890\n"
@@ -266,10 +254,23 @@
             return await aiobucket.put_object(object_name, data)
 
     with open(file, "rb") as f_r:
         assert f_r.readline() == data.strip() + os.linesep.encode()
         result = asyncio.run(put(object_name, f_r))
     assert result.resp.status == 200
     assert (
-        oss2_bucket.get_object(object_name).read()
-        == data.strip() + os.linesep.encode()
+        oss2_bucket.get_object(object_name).read() == data.strip() + os.linesep.encode()
     )
+
+
+def test_head_object(bucket: "AioBucket", oss2_bucket: "Bucket", number_file):
+    async def head_object(object_name):
+        async with bucket as aiobucket:
+            return await aiobucket.head_object(object_name)
+
+    result = asyncio.run(head_object(number_file))
+    expected = oss2_bucket.head_object(number_file)
+    assert expected.content_length == result.content_length
+    assert expected.object_type == result.object_type
+    assert expected.content_type == result.content_type
+    assert expected.last_modified == result.last_modified
+    assert expected.etag == result.etag
```

### Comparing `aiooss2-0.2.3/tests/unit/test_adapter.py` & `aiooss2-0.2.4/tests/unit/test_adapter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 """Unit tests for contents in adapter.py"""
 # pylint: disable=too-many-arguments
 # pylint: disable=missing-function-docstring
 import asyncio
 import inspect
 import io
 import os
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Iterable
 from unittest.mock import Mock
 
 import pytest
-from _collections_abc import list_iterator
 from aiohttp.streams import StreamReader
 
-from aiooss2.adapter import (
-    FilelikeObjectAdapter,
-    IterableAdapter,
-    SliceableAdapter,
-)
+from aiooss2.adapter import FilelikeObjectAdapter, IterableAdapter, SliceableAdapter
 from aiooss2.utils import make_adapter
 
 if TYPE_CHECKING:
     from oss2 import Bucket
+    from py.path import local
 
     from aiooss2.api import AioBucket
 
 
 @pytest.fixture(scope="module", name="test_path")
 def file_level_path(test_directory):
     file_name = __file__.rsplit(os.sep, maxsplit=1)[-1]
@@ -110,15 +106,15 @@
 ):
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
 
     if callable(datastream):
         datastream = datastream()
 
-    if not enable_crc and isinstance(datastream, list_iterator):
+    if not enable_crc and isinstance(datastream, Iterable):
         pytest.skip("invalid combination")
 
     function_name = inspect.stack()[0][0].f_code.co_name
     adapter = make_adapter(datastream, enable_crc=enable_crc)
     object_name = f"{test_path}/{function_name}"
     if enable_crc:
         assert isinstance(adapter, adapter_obj)
@@ -133,10 +129,22 @@
     assert result.resp.status == 200
 
     assert oss2_bucket.get_object(object_name).read() == data_get
 
 
 def test_make_adapter_error():
     with pytest.raises(ValueError):
-        assert make_adapter(
-            ["data1", "data2", "data3"], discard=1, enable_crc=True
-        )
+        assert make_adapter(["data1", "data2", "data3"], discard=1, enable_crc=True)
+
+
+def test_adapter_read(
+    tmpdir: "local",
+):
+    data = b"123456789"
+    file = tmpdir / "file"
+    file.write(data)
+
+    with open(str(file), "rb") as f_r:
+        f_r.seek(3, os.SEEK_SET)
+        adaptor = FilelikeObjectAdapter(f_r, size=5)
+        result = asyncio.run(adaptor.read())
+        assert result == b"45678"
```

