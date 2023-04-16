# Comparing `tmp/jsonrpc-py-2.5.1.tar.gz` & `tmp/jsonrpc-py-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonrpc-py-2.5.1.tar", last modified: Wed Feb  1 17:28:57 2023, max compression
+gzip compressed data, was "jsonrpc-py-3.0.0.tar", last modified: Sun Apr 16 09:15:16 2023, max compression
```

## Comparing `jsonrpc-py-2.5.1.tar` & `jsonrpc-py-3.0.0.tar`

### file list

```diff
@@ -1,41 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:28:57.111777 jsonrpc-py-2.5.1/
--rw-rw-rw-   0 root         (0) root         (0)    10174 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3154 2023-02-01 17:28:57.111777 jsonrpc-py-2.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1527 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:28:57.106777 jsonrpc-py-2.5.1/jsonrpc/
--rw-rw-rw-   0 root         (0) root         (0)     1201 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/jsonrpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1705 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/jsonrpc/_concurrency.py
--rw-rw-rw-   0 root         (0) root         (0)     5024 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/jsonrpc/_dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2882 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/jsonrpc/_errors.py
--rw-rw-rw-   0 root         (0) root         (0)     6453 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/jsonrpc/_request.py
--rw-rw-rw-   0 root         (0) root         (0)     4719 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/jsonrpc/_response.py
--rw-rw-rw-   0 root         (0) root         (0)     4511 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/jsonrpc/_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     1700 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/jsonrpc/_typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1933 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/jsonrpc/_utilities.py
--rw-rw-rw-   0 root         (0) root         (0)     8807 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/jsonrpc/_wsgi.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/jsonrpc/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:28:57.107777 jsonrpc-py-2.5.1/jsonrpc_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3154 2023-02-01 17:28:57.000000 jsonrpc-py-2.5.1/jsonrpc_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      774 2023-02-01 17:28:57.000000 jsonrpc-py-2.5.1/jsonrpc_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-01 17:28:57.000000 jsonrpc-py-2.5.1/jsonrpc_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-01 17:28:57.000000 jsonrpc-py-2.5.1/jsonrpc_py.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      122 2023-02-01 17:28:57.000000 jsonrpc-py-2.5.1/jsonrpc_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-02-01 17:28:57.000000 jsonrpc-py-2.5.1/jsonrpc_py.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)     1640 2023-02-01 17:28:57.112777 jsonrpc-py-2.5.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)       61 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:28:57.110777 jsonrpc-py-2.5.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)      661 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:28:57.111777 jsonrpc-py-2.5.1/tests/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)      661 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/tests/fixtures/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1335 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/tests/fixtures/dummy_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/tests/test_concurrency.py
--rw-rw-rw-   0 root         (0) root         (0)     4197 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/tests/test_dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2593 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/tests/test_errors.py
--rw-rw-rw-   0 root         (0) root         (0)     8825 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/tests/test_request.py
--rw-rw-rw-   0 root         (0) root         (0)     6426 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/tests/test_response.py
--rw-rw-rw-   0 root         (0) root         (0)     3078 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/tests/test_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2434 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/tests/test_utilities.py
--rw-rw-rw-   0 root         (0) root         (0)    12575 2023-02-01 17:28:45.000000 jsonrpc-py-2.5.1/tests/test_wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:15:16.005010 jsonrpc-py-3.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2937 2023-04-16 09:15:16.005010 jsonrpc-py-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1453 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:15:15.998010 jsonrpc-py-3.0.0/jsonrpc/
+-rw-rw-rw-   0 root         (0) root         (0)      501 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/jsonrpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8885 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/jsonrpc/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     4355 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/jsonrpc/dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2219 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/jsonrpc/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/jsonrpc/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     5746 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/jsonrpc/request.py
+-rw-rw-rw-   0 root         (0) root         (0)     4055 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/jsonrpc/response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/jsonrpc/serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2877 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/jsonrpc/typedefs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/jsonrpc/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:15:16.002010 jsonrpc-py-3.0.0/jsonrpc_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2937 2023-04-16 09:15:15.000000 jsonrpc-py-3.0.0/jsonrpc_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      658 2023-04-16 09:15:15.000000 jsonrpc-py-3.0.0/jsonrpc_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 09:15:15.000000 jsonrpc-py-3.0.0/jsonrpc_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 09:15:15.000000 jsonrpc-py-3.0.0/jsonrpc_py.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      134 2023-04-16 09:15:15.000000 jsonrpc-py-3.0.0/jsonrpc_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-16 09:15:15.000000 jsonrpc-py-3.0.0/jsonrpc_py.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      389 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1572 2023-04-16 09:15:16.005010 jsonrpc-py-3.0.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)       61 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:15:16.005010 jsonrpc-py-3.0.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13845 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/tests/test_asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     3580 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/tests/test_dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     1917 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/tests/test_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     8121 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/tests/test_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     5721 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/tests/test_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/tests/test_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2439 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/tests/test_utilities.py
```

### Comparing `jsonrpc-py-2.5.1/PKG-INFO` & `jsonrpc-py-3.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,80 +1,78 @@
 Metadata-Version: 2.1
 Name: jsonrpc-py
-Version: 2.5.1
+Version: 3.0.0
 Summary: Pure zero-dependency JSON-RPC 2.0 implementation
 Home-page: https://docs.jsonrpc.ru
 Author: Andrew Malchuk
 Author-email: andrew.malchuk@yandex.ru
 Maintainer: JSON-RPC Development Group
 Maintainer-email: dev@jsonrpc.ru
-License: Apache-2.0
+License: BSD-3-Clause
 Project-URL: Source Code, https://gitlab.com/jsonrpc/jsonrpc-py
 Project-URL: Documentation, https://docs.jsonrpc.ru
 Project-URL: Change Log, https://docs.jsonrpc.ru/changelog.html
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
+Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
-Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 JSON-RPC Python
 ===============
 [![pipeline status][pipeline]][homepage]
 [![coverage report][coverage]][homepage]
 [![latest release][version]][pypi]
 [![pypi downloads][downloads]][pypi]
 
-**JSON-RPC Python** is a lightweight WSGI micro framework for building web applications.
+**JSON-RPC Python** is a lightweight ASGI micro framework for building web applications.
 
 Features
 --------
 * Pure zero-dependency JSON-RPC 2.0 implementation.
 * Simple and user-friendly API interface.
 * 100% type annotated codebase.
 * 100% test coverage, so it's production-ready.
 
 Requirements
 ------------
-Python 3.10 and above.
+Python 3.11 and above.
 
 Installation
 ------------
 ```
 $ pip install jsonrpc-py
 ```
 
 Distribution
 ------------
-This project is licensed under the terms of the [Apache License 2.0](LICENSE).
+This project is licensed under the terms of the [BSD 3-Clause License](LICENSE).
 
 Links
 -----
 * Documentation: <https://docs.jsonrpc.ru>
 * PyPI Releases: <https://pypi.org/project/jsonrpc-py>
 * Source Code: <https://gitlab.com/jsonrpc/jsonrpc-py>
 
 [homepage]: <https://gitlab.com/jsonrpc/jsonrpc-py>
-[pipeline]: <https://img.shields.io/gitlab/pipeline-status/jsonrpc/jsonrpc-py?branch=development&logo=gitlab&style=flat-square&cacheSeconds=86400>
-[coverage]: <https://img.shields.io/gitlab/pipeline-coverage/jsonrpc/jsonrpc-py?branch=development&logo=gitlab&style=flat-square&cacheSeconds=86400>
+[pipeline]: <https://img.shields.io/gitlab/pipeline-status/jsonrpc/jsonrpc-py?branch=development&logo=gitlab&style=flat-square>
+[coverage]: <https://img.shields.io/gitlab/pipeline-coverage/jsonrpc/jsonrpc-py?branch=development&logo=gitlab&style=flat-square>
 [pypi]: <https://pypi.org/project/jsonrpc-py>
-[version]: <https://img.shields.io/pypi/v/jsonrpc-py?color=steelblue&logo=python&logoColor=steelblue&style=flat-square&cacheSeconds=86400>
-[downloads]: <https://img.shields.io/pypi/dm/jsonrpc-py?color=steelblue&logo=python&logoColor=steelblue&style=flat-square&cacheSeconds=86400>
+[version]: <https://img.shields.io/pypi/v/jsonrpc-py?color=steelblue&logo=python&logoColor=steelblue&style=flat-square>
+[downloads]: <https://img.shields.io/pypi/dm/jsonrpc-py?color=steelblue&logo=python&logoColor=steelblue&style=flat-square>
```

### Comparing `jsonrpc-py-2.5.1/README.md` & `jsonrpc-py-3.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 JSON-RPC Python
 ===============
 [![pipeline status][pipeline]][homepage]
 [![coverage report][coverage]][homepage]
 [![latest release][version]][pypi]
 [![pypi downloads][downloads]][pypi]
 
-**JSON-RPC Python** is a lightweight WSGI micro framework for building web applications.
+**JSON-RPC Python** is a lightweight ASGI micro framework for building web applications.
 
 Features
 --------
 * Pure zero-dependency JSON-RPC 2.0 implementation.
 * Simple and user-friendly API interface.
 * 100% type annotated codebase.
 * 100% test coverage, so it's production-ready.
 
 Requirements
 ------------
-Python 3.10 and above.
+Python 3.11 and above.
 
 Installation
 ------------
 ```
 $ pip install jsonrpc-py
 ```
 
 Distribution
 ------------
-This project is licensed under the terms of the [Apache License 2.0](LICENSE).
+This project is licensed under the terms of the [BSD 3-Clause License](LICENSE).
 
 Links
 -----
 * Documentation: <https://docs.jsonrpc.ru>
 * PyPI Releases: <https://pypi.org/project/jsonrpc-py>
 * Source Code: <https://gitlab.com/jsonrpc/jsonrpc-py>
 
 [homepage]: <https://gitlab.com/jsonrpc/jsonrpc-py>
-[pipeline]: <https://img.shields.io/gitlab/pipeline-status/jsonrpc/jsonrpc-py?branch=development&logo=gitlab&style=flat-square&cacheSeconds=86400>
-[coverage]: <https://img.shields.io/gitlab/pipeline-coverage/jsonrpc/jsonrpc-py?branch=development&logo=gitlab&style=flat-square&cacheSeconds=86400>
+[pipeline]: <https://img.shields.io/gitlab/pipeline-status/jsonrpc/jsonrpc-py?branch=development&logo=gitlab&style=flat-square>
+[coverage]: <https://img.shields.io/gitlab/pipeline-coverage/jsonrpc/jsonrpc-py?branch=development&logo=gitlab&style=flat-square>
 [pypi]: <https://pypi.org/project/jsonrpc-py>
-[version]: <https://img.shields.io/pypi/v/jsonrpc-py?color=steelblue&logo=python&logoColor=steelblue&style=flat-square&cacheSeconds=86400>
-[downloads]: <https://img.shields.io/pypi/dm/jsonrpc-py?color=steelblue&logo=python&logoColor=steelblue&style=flat-square&cacheSeconds=86400>
+[version]: <https://img.shields.io/pypi/v/jsonrpc-py?color=steelblue&logo=python&logoColor=steelblue&style=flat-square>
+[downloads]: <https://img.shields.io/pypi/dm/jsonrpc-py?color=steelblue&logo=python&logoColor=steelblue&style=flat-square>
```

### Comparing `jsonrpc-py-2.5.1/jsonrpc/_dispatcher.py` & `jsonrpc-py-3.0.0/jsonrpc/dispatcher.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,125 +1,105 @@
-# Pure zero-dependency JSON-RPC 2.0 implementation.
-# Copyright © 2022-2023 Andrew Malchuk. All rights reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     https://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
+from asyncio import CancelledError
 from collections import UserDict
 from collections.abc import Callable
 from functools import partial
 from inspect import BoundArguments, isfunction, signature
 from typing import Any, Final, TypeAlias, TypeVar, overload
 
-from ._errors import Error, ErrorEnum
+from .errors import Error, ErrorEnum
+from .utilities import wrap_coroutine
 
-__all__: Final[tuple[str, ...]] = ("Dispatcher",)
+__all__: Final[tuple[str, ...]] = ("AsyncDispatcher",)
 
-_AnyCallable: TypeAlias = Callable[..., Any]
-_Func = TypeVar("_Func", bound=_AnyCallable)
+AnyCallable: TypeAlias = Callable[..., Any]
+Func = TypeVar("Func", bound=AnyCallable)
 
 
-class Dispatcher(UserDict[str, _AnyCallable]):
+class AsyncDispatcher(UserDict[str, AnyCallable]):
     """
     The :py:class:`collections.UserDict` subclass representing the storage of user-defined functions.
-
-    For example::
-
-        >>> dispatcher = Dispatcher()
-        >>> dispatcher["func"] = lambda: True
-        >>> dispatcher["func"]
-        <function <lambda> at 0x\u2026>
     """
 
     __slots__: tuple[str, ...] = ()
 
     def __repr__(self) -> str:
-        return f"{self.__class__.__qualname__}({self.data!r})"
+        return f"{self.__class__.__qualname__}()"
 
     @overload
-    def register(self, user_function: _Func, /) -> _Func:
+    def register(self, user_function: Func, /) -> Func:
         ...
 
     @overload
-    def register(self, user_function: _Func, *, function_name: str | None = ...) -> _Func:
+    def register(self, user_function: Func, *, function_name: str | None = ...) -> Func:
         ...
 
     @overload
-    def register(self, *, function_name: str | None = ...) -> Callable[[_Func], _Func]:
+    def register(self, *, function_name: str | None = ...) -> Callable[[Func], Func]:
         ...
 
-    def register(self, user_function: _Func | None = None, *, function_name: str | None = None) -> Any:
+    def register(self, user_function: Func | None = None, *, function_name: str | None = None) -> Any:
         """
         Adds a user-defined function to the dispatcher.
 
         Example usage::
 
             >>> @dispatcher.register
             ... def truediv(a: float, b: float) -> float:
             ...     return a / b
 
         Also you can pass the different function's name::
 
-            >>> @dispatcher.register(function_name="sum")
-            ... def _(a: float, b: float) -> float:
-            ...     return a + b
+            >>> @dispatcher.register(function_name="slow_greetings")
+            ... async def _(name: str) -> str:
+            ...     return await sleep(3600.0, f"Greetings, {name} !!")
 
         :param user_function: The :py:data:`types.FunctionType` object representing the user-defined function.
         :param function_name: An optional function's name. If it is omitted, attribute ``__name__`` will be used instead.
         :raises RuntimeError: If the ``user_function`` isn't passed by the :py:func:`inspect.isfunction` method,
-            or function with the provided name is already defined in the :class:`jsonrpc.Dispatcher` class.
+            or function with the provided name is already defined in the :class:`jsonrpc.AsyncDispatcher` class.
         :returns: The unmodified ``user_function`` object, passed in the parameters.
         """
         if user_function is None:
             return partial(self.register, function_name=function_name)
 
         if not isfunction(user_function):
             raise RuntimeError(f"{type(user_function).__name__!r} isn't a user-defined function")
 
         if (function_name := user_function.__name__ if function_name is None else function_name) in self:
             raise RuntimeError(f"{function_name!r} is already defined in {self[function_name].__module__!r}")
 
         self[function_name] = user_function
         return user_function
 
-    def dispatch(self, function_name: str, /, *args: Any, **kwargs: Any) -> Any:
+    async def dispatch(self, function_name: str, /, *args: Any, **kwargs: Any) -> Any:
         """
         Invoke the user-defined function by passed in parameters function's name.
 
         Example usage::
 
-            >>> dispatcher = Dispatcher()
-            >>> dispatcher.dispatch("sum", a=12, b=34)
+            >>> dispatcher = AsyncDispatcher()
+            >>> await dispatcher.dispatch("sum", a=12, b=34)
             46
 
         :param function_name: The user-defined function's name.
         :param args: Positional arguments for the provided function.
         :param kwargs: Keyword arguments for the provided function.
-        :raises jsonrpc.Error: If the function doesn't exists in the :class:`jsonrpc.Dispatcher` class,
+        :raises jsonrpc.Error: If the function doesn't exists in the :class:`jsonrpc.AsyncDispatcher` class,
             passed invalid parameters or unexpected internal error has raised. See also :class:`jsonrpc.ErrorEnum`.
         :returns: Result of execution the user-defined function.
         """
         try:
-            user_function: Final[_AnyCallable] = self[function_name]
+            user_function: AnyCallable = self[function_name]
         except KeyError as exc:
             raise Error(code=ErrorEnum.METHOD_NOT_FOUND, message=f"Function {function_name!r} isn't found") from exc
 
         try:
-            params: Final[BoundArguments] = signature(user_function).bind(*args, **kwargs)
+            params: BoundArguments = signature(user_function).bind(*args, **kwargs)
         except TypeError as exc:
             raise Error(code=ErrorEnum.INVALID_PARAMETERS, message=f"Invalid parameters: {exc!s}") from exc
 
         try:
-            return user_function(*params.args, **params.kwargs)
-        except Error:
+            return await wrap_coroutine(user_function, *params.args, **params.kwargs)
+        except (TimeoutError, CancelledError, Error):
             raise
         except Exception as exc:
             raise Error(code=ErrorEnum.INTERNAL_ERROR, message=f"Unexpected internal error: {exc!s}") from exc
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `jsonrpc-py-2.5.1/jsonrpc/_errors.py` & `jsonrpc-py-3.0.0/jsonrpc/errors.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,12 @@
-# Pure zero-dependency JSON-RPC 2.0 implementation.
-# Copyright © 2022-2023 Andrew Malchuk. All rights reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     https://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from dataclasses import dataclass
 from enum import IntEnum
 from typing import Any, Final
 
-from ._utilities import Undefined, UndefinedType, make_hashable
+from .utilities import Undefined, UndefinedType, make_hashable
 
 __all__: Final[tuple[str, ...]] = (
     "Error",
     "ErrorEnum",
 )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `jsonrpc-py-2.5.1/jsonrpc/_request.py` & `jsonrpc-py-3.0.0/jsonrpc/request.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,16 @@
-# Pure zero-dependency JSON-RPC 2.0 implementation.
-# Copyright © 2022-2023 Andrew Malchuk. All rights reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     https://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from collections import UserList
 from collections.abc import Iterable, MutableMapping, MutableSequence
 from dataclasses import dataclass
 from numbers import Number
-from re import match as _regex_match
-from typing import Any, Final, Union
+from re import match as regex_match
+from typing import Any, Final, Self
 
-from ._errors import Error, ErrorEnum
-from ._utilities import Undefined, UndefinedType, make_hashable
+from .errors import Error, ErrorEnum
+from .utilities import Undefined, UndefinedType, make_hashable
 
 __all__: Final[tuple[str, ...]] = (
     "BatchRequest",
     "Request",
 )
 
 
@@ -50,15 +35,15 @@
         self._validate_params()
         self._validate_request_id()
 
     def __hash__(self) -> int:
         return hash((self.method, make_hashable(self.params), self.request_id))
 
     def _validate_method(self) -> None:
-        if not isinstance(self.method, str) or _regex_match("\x5E\x72\x70\x63\x5C\x2E", self.method):
+        if not isinstance(self.method, str) or regex_match("\x5e\x72\x70\x63\x5c\x2e", self.method):
             raise Error(
                 code=ErrorEnum.INVALID_REQUEST,
                 message="Request method must be a string and should not have a 'rpc.' prefix",
             )
 
     def _validate_params(self) -> None:
         if not isinstance(self.params, MutableSequence | MutableMapping | UndefinedType):
@@ -91,38 +76,38 @@
     @property
     def is_notification(self) -> bool:
         """
         Returns :py:data:`True` if the identifier of the request is omitted, :py:data:`False` elsewise.
         """
         return isinstance(self.request_id, UndefinedType)
 
-    @staticmethod
-    def from_json(obj: dict[str, Any], /) -> Union["Request", Error]:
+    @classmethod
+    def from_json(cls, obj: dict[str, Any], /) -> Self | Error:
         """
-        The static method for creating the :class:`jsonrpc.Request` object from :py:class:`dict` object.
+        The class method for creating the :class:`jsonrpc.Request` object from :py:class:`dict` object.
         Unlike the :class:`jsonrpc.Request` constructor, doesn't raises any exceptions by validations,
         it returns the :class:`jsonrpc.Error` as is.
 
         Example usage::
 
             >>> Request.from_json({"jsonrpc": "2.0", "method": "foobar", "id": 1})
             Request(method="foobar", params=Undefined, request_id=1)
             >>> Request.from_json({"not_jsonrpc": True})
             Error(code=-32600, message="Invalid request object", data={"not_jsonrpc": True})
         """
         try:
             match obj:
                 case {"jsonrpc": "2.0", "method": method, "params": params, "id": request_id}:
-                    return Request(method=method, params=params, request_id=request_id)
+                    return cls(method=method, params=params, request_id=request_id)
                 case {"jsonrpc": "2.0", "method": method, "params": params}:
-                    return Request(method=method, params=params)
+                    return cls(method=method, params=params)
                 case {"jsonrpc": "2.0", "method": method, "id": request_id}:
-                    return Request(method=method, request_id=request_id)
+                    return cls(method=method, request_id=request_id)
                 case {"jsonrpc": "2.0", "method": method}:
-                    return Request(method=method)
+                    return cls(method=method)
                 case _ as data:
                     raise Error(code=ErrorEnum.INVALID_REQUEST, message="Invalid request object", data=data)
         except Error as error:
             return error
 
 
 class BatchRequest(UserList[Request | Error]):
@@ -135,23 +120,23 @@
 
     def __repr__(self) -> str:
         return f"{self.__class__.__qualname__}({self.data!r})"
 
     def __hash__(self) -> int:
         return hash(tuple(self.data))
 
-    @staticmethod
-    def from_json(iterable: Iterable[dict[str, Any]], /) -> "BatchRequest":
+    @classmethod
+    def from_json(cls, iterable: Iterable[dict[str, Any]], /) -> Self:
         """
-        The static method for creating the :class:`jsonrpc.BatchRequest` object from :py:class:`collections.abc.Iterable`
+        The class method for creating the :class:`jsonrpc.BatchRequest` object from :py:class:`collections.abc.Iterable`
         of :py:class:`dict` objects.
         Similar to :func:`jsonrpc.Request.from_json` function it doesn't raises any exceptions.
 
         Example usage::
 
             >>> BatchRequest.from_json([
             ...     {"jsonrpc": "2.0", "method": "foobar", "id": 1},
             ...     {"not_jsonrpc": True}
             ... ])
             BatchRequest([Request(\u2026), Error(\u2026)])
         """
-        return BatchRequest(map(Request.from_json, iterable))
+        return cls(map(Request.from_json, iterable))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `jsonrpc-py-2.5.1/jsonrpc/_response.py` & `jsonrpc-py-3.0.0/jsonrpc/response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,15 @@
-# Pure zero-dependency JSON-RPC 2.0 implementation.
-# Copyright © 2022-2023 Andrew Malchuk. All rights reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     https://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from collections import UserList
 from dataclasses import dataclass
 from numbers import Number
 from types import NoneType
 from typing import Any, Final
 
-from ._errors import Error
-from ._utilities import Undefined, UndefinedType, make_hashable
+from .errors import Error
+from .utilities import Undefined, UndefinedType, make_hashable
 
 __all__: Final[tuple[str, ...]] = (
     "BatchResponse",
     "Response",
 )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `jsonrpc-py-2.5.1/jsonrpc/_utilities.py` & `jsonrpc-py-3.0.0/jsonrpc/utilities.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,71 @@
-# Pure zero-dependency JSON-RPC 2.0 implementation.
-# Copyright © 2022-2023 Andrew Malchuk. All rights reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     https://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from collections.abc import Iterable, MutableMapping
-from typing import Any, Final, Literal, TypeGuard, final
+from asyncio import AbstractEventLoop, Future, get_running_loop
+from collections.abc import Callable, Iterable, MutableMapping
+from contextvars import Context, copy_context
+from functools import partial
+from inspect import iscoroutinefunction
+from typing import Any, Final, Literal, ParamSpec, TypeGuard, final
 
 __all__: Final[tuple[str, ...]] = (
     "is_iterable",
     "make_hashable",
     "Undefined",
     "UndefinedType",
+    "wrap_coroutine",
 )
 
+P = ParamSpec("P")
+
 
 def is_iterable(obj: Any, /) -> TypeGuard[Iterable[Any]]:
     try:
         iter(obj)
     except TypeError:
         return False
     else:
         return True
 
 
 def make_hashable(obj: Any, /) -> Any:
     if isinstance(obj, MutableMapping):
         return tuple((key, make_hashable(value)) for key, value in sorted(obj.items()))
-
-    # Try hash to avoid converting a hashable iterable (e.g. string, frozenset)
-    # to a tuple:
+    #: ---
+    #: Try hash to avoid converting a hashable iterable (e.g. string, frozenset)
+    #: to a tuple:
     try:
         hash(obj)
     except TypeError:
         if is_iterable(obj):
             return tuple(map(make_hashable, obj))
-        # Non-hashable, non-iterable:
+        #: ---
+        #: Non-hashable, non-iterable:
         raise
 
     return obj
 
 
+def wrap_coroutine(user_function: Callable[P, Any], /, *args: P.args, **kwargs: P.kwargs) -> Future[Any]:
+    loop: AbstractEventLoop = get_running_loop()
+    context: Context = copy_context()
+
+    if iscoroutinefunction(callback := partial(user_function, *args, **kwargs)):
+        return loop.create_task(callback(), context=context)
+    else:
+        return loop.run_in_executor(None, context.run, callback)
+
+
 @final
 class UndefinedType:
     __slots__: tuple[str, ...] = ()
 
     def __repr__(self) -> Literal["Undefined"]:
         return "Undefined"
 
-    def __hash__(self) -> Literal[0xDEADBEEF]:
-        return 0xDEADBEEF
+    def __hash__(self) -> Literal[0xBAADF00D]:
+        return 0xBAADF00D
 
     def __eq__(self, obj: Any) -> bool:
         return isinstance(obj, self.__class__)
 
     def __bool__(self) -> Literal[False]:
         return False
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `jsonrpc-py-2.5.1/jsonrpc_py.egg-info/PKG-INFO` & `jsonrpc-py-3.0.0/jsonrpc_py.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,80 +1,78 @@
 Metadata-Version: 2.1
 Name: jsonrpc-py
-Version: 2.5.1
+Version: 3.0.0
 Summary: Pure zero-dependency JSON-RPC 2.0 implementation
 Home-page: https://docs.jsonrpc.ru
 Author: Andrew Malchuk
 Author-email: andrew.malchuk@yandex.ru
 Maintainer: JSON-RPC Development Group
 Maintainer-email: dev@jsonrpc.ru
-License: Apache-2.0
+License: BSD-3-Clause
 Project-URL: Source Code, https://gitlab.com/jsonrpc/jsonrpc-py
 Project-URL: Documentation, https://docs.jsonrpc.ru
 Project-URL: Change Log, https://docs.jsonrpc.ru/changelog.html
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
+Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
-Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 JSON-RPC Python
 ===============
 [![pipeline status][pipeline]][homepage]
 [![coverage report][coverage]][homepage]
 [![latest release][version]][pypi]
 [![pypi downloads][downloads]][pypi]
 
-**JSON-RPC Python** is a lightweight WSGI micro framework for building web applications.
+**JSON-RPC Python** is a lightweight ASGI micro framework for building web applications.
 
 Features
 --------
 * Pure zero-dependency JSON-RPC 2.0 implementation.
 * Simple and user-friendly API interface.
 * 100% type annotated codebase.
 * 100% test coverage, so it's production-ready.
 
 Requirements
 ------------
-Python 3.10 and above.
+Python 3.11 and above.
 
 Installation
 ------------
 ```
 $ pip install jsonrpc-py
 ```
 
 Distribution
 ------------
-This project is licensed under the terms of the [Apache License 2.0](LICENSE).
+This project is licensed under the terms of the [BSD 3-Clause License](LICENSE).
 
 Links
 -----
 * Documentation: <https://docs.jsonrpc.ru>
 * PyPI Releases: <https://pypi.org/project/jsonrpc-py>
 * Source Code: <https://gitlab.com/jsonrpc/jsonrpc-py>
 
 [homepage]: <https://gitlab.com/jsonrpc/jsonrpc-py>
-[pipeline]: <https://img.shields.io/gitlab/pipeline-status/jsonrpc/jsonrpc-py?branch=development&logo=gitlab&style=flat-square&cacheSeconds=86400>
-[coverage]: <https://img.shields.io/gitlab/pipeline-coverage/jsonrpc/jsonrpc-py?branch=development&logo=gitlab&style=flat-square&cacheSeconds=86400>
+[pipeline]: <https://img.shields.io/gitlab/pipeline-status/jsonrpc/jsonrpc-py?branch=development&logo=gitlab&style=flat-square>
+[coverage]: <https://img.shields.io/gitlab/pipeline-coverage/jsonrpc/jsonrpc-py?branch=development&logo=gitlab&style=flat-square>
 [pypi]: <https://pypi.org/project/jsonrpc-py>
-[version]: <https://img.shields.io/pypi/v/jsonrpc-py?color=steelblue&logo=python&logoColor=steelblue&style=flat-square&cacheSeconds=86400>
-[downloads]: <https://img.shields.io/pypi/dm/jsonrpc-py?color=steelblue&logo=python&logoColor=steelblue&style=flat-square&cacheSeconds=86400>
+[version]: <https://img.shields.io/pypi/v/jsonrpc-py?color=steelblue&logo=python&logoColor=steelblue&style=flat-square>
+[downloads]: <https://img.shields.io/pypi/dm/jsonrpc-py?color=steelblue&logo=python&logoColor=steelblue&style=flat-square>
```

### Comparing `jsonrpc-py-2.5.1/setup.cfg` & `jsonrpc-py-3.0.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -5,50 +5,52 @@
 author_email = andrew.malchuk@yandex.ru
 maintainer = JSON-RPC Development Group
 maintainer_email = dev@jsonrpc.ru
 description = Pure zero-dependency JSON-RPC 2.0 implementation
 url = https://docs.jsonrpc.ru
 long_description = file:README.md
 long_description_content_type = text/markdown
-license = Apache-2.0
+license = BSD-3-Clause
 license_files = LICENSE
 platforms = any
 project_urls = 
 	Source Code = https://gitlab.com/jsonrpc/jsonrpc-py
 	Documentation = https://docs.jsonrpc.ru
 	Change Log = https://docs.jsonrpc.ru/changelog.html
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Web Environment
+	Framework :: AsyncIO
 	Intended Audience :: Developers
-	License :: OSI Approved :: Apache Software License
+	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
-	Topic :: Internet :: WWW/HTTP :: WSGI
-	Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 	Topic :: Software Development :: Libraries :: Application Frameworks
 	Topic :: Software Development :: Libraries :: Python Modules
 	Typing :: Typed
 
 [options]
 packages = jsonrpc
-python_requires = >=3.10
+python_requires = >=3.11
 zip_safe = off
 
 [options.package_data]
 jsonrpc = py.typed
 
 [options.extras_require]
 dev = file:requirements-dev.txt
 
+[flake8]
+extend-ignore = E203
+max-line-length = 140
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `jsonrpc-py-2.5.1/tests/test_dispatcher.py` & `jsonrpc-py-3.0.0/tests/test_dispatcher.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,20 @@
-# Pure zero-dependency JSON-RPC 2.0 implementation.
-# Copyright © 2022-2023 Andrew Malchuk. All rights reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     https://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from collections.abc import Callable, MutableMapping
 from types import FunctionType, LambdaType
 from typing import NoReturn, TypeVar
-from unittest.case import TestCase
+from unittest import IsolatedAsyncioTestCase
 
-from jsonrpc._dispatcher import Dispatcher
-from jsonrpc._errors import Error, ErrorEnum
+from jsonrpc import AsyncDispatcher, Error, ErrorEnum
 
-_T = TypeVar("_T")
+T = TypeVar("T")
 
 
-class TestDispatcher(TestCase):
+class TestDispatcher(IsolatedAsyncioTestCase):
     def setUp(self) -> None:
-        self.dispatcher: Dispatcher = Dispatcher()
+        self.dispatcher: AsyncDispatcher = AsyncDispatcher()
 
     def test_inheritance(self) -> None:
         self.assertIsInstance(self.dispatcher, MutableMapping)
 
     def test_register_not_function(self) -> None:
         with self.assertRaises(RuntimeError) as context:
             self.dispatcher.register(print)
@@ -45,55 +29,55 @@
         self.assertEqual(self.dispatcher["test_lambda"], test_lambda)
 
         with self.assertRaises(RuntimeError) as context:
             self.dispatcher.register(test_lambda, function_name="test_lambda")
 
         self.assertIn("is already defined", str(context.exception))
 
-    def test_dispatch_non_existent_function(self) -> None:
+    async def test_dispatch_non_existent_function(self) -> None:
         with self.assertRaises(Error) as context:
-            self.dispatcher.dispatch("non_existent_function")
+            await self.dispatcher.dispatch("non_existent_function")
 
         self.assertEqual(context.exception.code, ErrorEnum.METHOD_NOT_FOUND)
 
-    def test_dispatch_non_existent_parameter(self) -> None:
-        test_lambda: Callable[[_T], _T] = lambda obj: obj
+    async def test_dispatch_non_existent_parameter(self) -> None:
+        test_lambda: Callable[[T], T] = lambda obj: obj
         self.dispatcher.register(test_lambda, function_name="test_lambda")
         self.assertIn("test_lambda", self.dispatcher)
         self.assertIsInstance(self.dispatcher["test_lambda"], LambdaType)
         self.assertEqual(self.dispatcher["test_lambda"], test_lambda)
 
         with self.assertRaises(Error) as context:
-            self.dispatcher.dispatch("test_lambda", non_existent_parameter="non_existent_parameter")
+            await self.dispatcher.dispatch("test_lambda", non_existent_parameter="non_existent_parameter")
 
         self.assertEqual(context.exception.code, ErrorEnum.INVALID_PARAMETERS)
 
-    def test_dispatch_division(self) -> None:
+    async def test_dispatch_division(self) -> None:
         @self.dispatcher.register(function_name="my_div")
         def div(a: float, b: float) -> float:
             return a / b
 
         self.assertNotIn("div", self.dispatcher)
         self.assertIn("my_div", self.dispatcher)
         self.assertIsInstance(self.dispatcher["my_div"], FunctionType)
         self.assertEqual(self.dispatcher["my_div"], div)
 
         with self.assertRaises(Error) as context:
-            self.dispatcher.dispatch("my_div", 10, 0)
+            await self.dispatcher.dispatch("my_div", 10, 0)
 
         self.assertEqual(context.exception.code, ErrorEnum.INTERNAL_ERROR)
         self.assertIn("division by zero", context.exception.message)
 
-    def test_dispatch_raising(self) -> None:
+    async def test_dispatch_raising(self) -> None:
         @self.dispatcher.register
         def raising(*, code: int, message: str) -> NoReturn:
             raise Error(code=code, message=message)
 
         self.assertIn("raising", self.dispatcher)
         self.assertIsInstance(self.dispatcher["raising"], FunctionType)
         self.assertEqual(self.dispatcher["raising"], raising)
 
         with self.assertRaises(Error) as context:
-            self.dispatcher.dispatch("raising", code=ErrorEnum.INTERNAL_ERROR, message="for testing purposes")
+            await self.dispatcher.dispatch("raising", code=ErrorEnum.INTERNAL_ERROR, message="for testing purposes")
 
         self.assertEqual(context.exception.code, ErrorEnum.INTERNAL_ERROR)
         self.assertEqual(context.exception.message, "for testing purposes")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `jsonrpc-py-2.5.1/tests/test_errors.py` & `jsonrpc-py-3.0.0/tests/test_errors.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,13 @@
-# Pure zero-dependency JSON-RPC 2.0 implementation.
-# Copyright © 2022-2023 Andrew Malchuk. All rights reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     https://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from dataclasses import is_dataclass
 from typing import Final
-from unittest.case import TestCase
+from unittest import TestCase
 
-from jsonrpc._errors import Error, ErrorEnum
-from jsonrpc._utilities import Undefined
+from jsonrpc import Error, ErrorEnum
+from jsonrpc.utilities import Undefined
 
 
 class TestError(TestCase):
     def test_inheritance(self) -> None:
         error: Final[Error] = Error(code=ErrorEnum.INTERNAL_ERROR, message="Internal Error")
         self.assertTrue(is_dataclass(error))
         self.assertIsInstance(error, Exception)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `jsonrpc-py-2.5.1/tests/test_request.py` & `jsonrpc-py-3.0.0/tests/test_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,17 @@
-# Pure zero-dependency JSON-RPC 2.0 implementation.
-# Copyright © 2022-2023 Andrew Malchuk. All rights reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     https://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from collections.abc import MutableSequence
 from dataclasses import is_dataclass
 from functools import partial
 from types import NoneType
 from typing import Any, Final
-from unittest.case import TestCase
+from unittest import TestCase
 from uuid import UUID, uuid4
 
-from jsonrpc._errors import Error, ErrorEnum
-from jsonrpc._request import BatchRequest, Request
-from jsonrpc._utilities import Undefined
+from jsonrpc import BatchRequest, Error, ErrorEnum, Request
+from jsonrpc.utilities import Undefined
 
 
 class TestRequest(TestCase):
     @property
     def random_id(self) -> int:
         uuid: Final[UUID] = uuid4()
         return int(uuid)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `jsonrpc-py-2.5.1/tests/test_response.py` & `jsonrpc-py-3.0.0/tests/test_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,16 @@
-# Pure zero-dependency JSON-RPC 2.0 implementation.
-# Copyright © 2022-2023 Andrew Malchuk. All rights reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     https://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from collections.abc import MutableSequence
 from dataclasses import is_dataclass
 from functools import partial
 from typing import Final
-from unittest.case import TestCase
+from unittest import TestCase
 from uuid import UUID, uuid4
 
-from jsonrpc._errors import Error, ErrorEnum
-from jsonrpc._response import BatchResponse, Response
-from jsonrpc._utilities import Undefined
+from jsonrpc import BatchResponse, Error, ErrorEnum, Response
+from jsonrpc.utilities import Undefined
 
 
 class TestResponse(TestCase):
     @property
     def random_id(self) -> str:
         uuid: Final[UUID] = uuid4()
         return str(uuid)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `jsonrpc-py-2.5.1/tests/test_utilities.py` & `jsonrpc-py-3.0.0/tests/test_utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,13 @@
-# Pure zero-dependency JSON-RPC 2.0 implementation.
-# Copyright © 2022-2023 Andrew Malchuk. All rights reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     https://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
+from asyncio import Future
 from typing import Any, Literal
-from unittest.case import TestCase
+from unittest import IsolatedAsyncioTestCase, TestCase
+from unittest.mock import AsyncMock, MagicMock, sentinel
 
-from jsonrpc._utilities import Undefined, UndefinedType, make_hashable
+from jsonrpc.utilities import Undefined, UndefinedType, make_hashable, wrap_coroutine
 
 
 class TestHashable(TestCase):
     def test_equality(self) -> None:
         tests: tuple[tuple[Any, Any], ...] = (
             ([], ()),
             (["a", 1], ("a", 1)),
@@ -53,15 +40,28 @@
             make_hashable(Unhashable())
 
         self.assertIn("unhashable type", str(context.exception))
 
 
 class TestUndefined(TestCase):
     def test_hash(self) -> None:
-        self.assertEqual(hash(Undefined), 0xDEADBEEF)
+        self.assertEqual(hash(Undefined), 0xBAADF00D)
 
     def test_equality(self) -> None:
         self.assertEqual(Undefined, UndefinedType())
         self.assertNotEqual(Undefined, None)
 
     def test_is_truth(self) -> None:
         self.assertFalse(Undefined)
+
+
+class TestUtilities(IsolatedAsyncioTestCase):
+    async def test_wrap_coroutine(self) -> None:
+        for mock in (
+            MagicMock(return_value=sentinel.sync_def),
+            AsyncMock(return_value=sentinel.async_def),
+        ):
+            with self.subTest(mock=mock):
+                future: Future[Any] = wrap_coroutine(mock, 1, 2, 3, key="value")
+                self.assertIsInstance(future, Future)
+                self.assertIs(await future, mock.return_value)
+                mock.assert_called_once_with(1, 2, 3, key="value")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `jsonrpc-py-2.5.1/tests/test_wsgi.py` & `jsonrpc-py-3.0.0/tests/test_asgi.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,290 +1,172 @@
-# Pure zero-dependency JSON-RPC 2.0 implementation.
-# Copyright © 2022-2023 Andrew Malchuk. All rights reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     https://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
+from asyncio import Event, Queue, get_running_loop, sleep, wait_for
 from collections.abc import MutableMapping
-from http import HTTPStatus
-from io import StringIO
-from os import urandom
-from typing import Final, Literal
-from unittest.case import TestCase
-from unittest.mock import patch
+from http import HTTPMethod, HTTPStatus
+from typing import Any, Final, Literal
+from unittest import IsolatedAsyncioTestCase, TestCase
+from unittest.mock import AsyncMock
 from uuid import UUID, uuid4
 
-from werkzeug.test import Client, EnvironBuilder, TestResponse
-
-from jsonrpc._concurrency import set_executor
-from jsonrpc._errors import ErrorEnum
-from jsonrpc._wsgi import WSGIHandler
+from httpx import AsyncClient, Response
 
-from .fixtures.dummy_executor import DummyExecutor
+from jsonrpc import ASGIHandler, ErrorEnum
 
 
 class AnyNonEmptyString:
     __slots__: tuple[str, ...] = ("test_case",)
 
     def __init__(self, test_case: TestCase) -> None:
         self.test_case: TestCase = test_case
 
     def __eq__(self, string: str) -> Literal[True]:
         self.test_case.assertIsInstance(string, str)
         self.test_case.assertGreater(len(string), 0)
         return True
 
 
-class TestWSGIHandler(TestCase):
-    @property
-    def random_id(self) -> str:
-        uuid: Final[UUID] = uuid4()
-        return str(uuid)
-
-    @classmethod
-    def setUpClass(cls) -> None:
-        dummy_executor: Final[DummyExecutor] = DummyExecutor()
-        set_executor(dummy_executor)
-
+class TestASGIHandler(IsolatedAsyncioTestCase):
     def setUp(self) -> None:
-        self.application: WSGIHandler = WSGIHandler()
-        self.client: Client = Client(self.application, use_cookies=False)
-        self.collection: list[str] = list()
-
-        @self.application.dispatcher.register(function_name="sum")
-        def _(a: float, b: float) -> float:
-            return a + b
-
-        @self.application.dispatcher.register
-        def div(*, a: float, b: float) -> float:
-            return a / b
-
-        @self.application.dispatcher.register
-        def append(obj: str) -> None:
-            self.collection.append(obj)
+        self.app: ASGIHandler = ASGIHandler()
+        self.receive_channel: AsyncMock = AsyncMock()
+        self.send_channel: AsyncMock = AsyncMock()
 
     def test_inheritance(self) -> None:
-        self.assertIsInstance(self.application, MutableMapping)
+        self.assertIsInstance(self.app, MutableMapping)
 
-    def test_handle_request_runtime_error(self) -> None:
-        with StringIO() as raw_buffer:
-            request: EnvironBuilder = EnvironBuilder(
-                method="POST",
-                errors_stream=raw_buffer,
-                json={"jsonrpc": "2.0", "method": "print"},
-            )
-
-            with patch.object(WSGIHandler, "_read_request_body") as mock:
-                mock.side_effect = RuntimeError("for testing purposes")
-
-                with self.assertRaises(RuntimeError) as context:
-                    self.client.open(request)
-
-            self.assertIsInstance(context.exception, RuntimeError)
-            self.assertEqual(str(context.exception), "for testing purposes")
-            self.assertIn("RuntimeError: for testing purposes", raw_buffer.getvalue())
-
-    def test_forbidden_methods(self) -> None:
-        responses: tuple[TestResponse, ...] = (
-            self.client.head("/testHead/"),
-            self.client.get("/testGet/"),
-            self.client.patch(data=b""),
-            self.client.delete(data=b""),
-            self.client.options("/testOptions/"),
-            self.client.trace("/testTrace/"),
-        )
-        for response in responses:
-            with self.subTest(response=response):
-                self.assertEqual(response.status_code, HTTPStatus.METHOD_NOT_ALLOWED)
-                self.assertIn("POST", response.allow)
-                self.assertIn("PUT", response.allow)
-                self.assertEqual(response.data, b"")
-
-    def test_empty_request(self) -> None:
-        responses: tuple[TestResponse, ...] = (
-            self.client.post(data=b""),
-            self.client.put(data=b""),
-        )
-        for response in responses:
-            with self.subTest(response=response):
-                self.assertEqual(response.status_code, HTTPStatus.BAD_REQUEST)
-                self.assertEqual(response.data, b"")
-
-    def test_positional_parameters(self) -> None:
-        uuid: str = self.random_id
-        response: TestResponse = self.client.post(json={"jsonrpc": "2.0", "method": "sum", "params": [8192, 1024], "id": uuid})
-        self.assertEqual(response.status_code, HTTPStatus.OK)
-        self.assertTrue(response.is_json)
-        self.assertDictEqual(response.json, {"jsonrpc": "2.0", "result": 9216, "id": uuid})
+    async def test_supported_scopes(self) -> None:
+        for scope in {"type": "websocket"}, {"type": "lifespan"}:
+            with self.subTest(scope=scope):
+                with self.assertRaises(ValueError) as context:
+                    await self.app(scope, self.receive_channel, self.send_channel)
 
-    def test_named_parameters(self) -> None:
-        uuid: str = self.random_id
-        response: TestResponse = self.client.post(json={"jsonrpc": "2.0", "method": "div", "params": {"a": 8192, "b": 1024}, "id": uuid})
-        self.assertEqual(response.status_code, HTTPStatus.OK)
-        self.assertTrue(response.is_json)
-        self.assertDictEqual(response.json, {"jsonrpc": "2.0", "result": 8.0, "id": uuid})
+                self.assertEqual(str(context.exception), "Only ASGI/HTTP connections are allowed.")
+                self.receive_channel.assert_not_called()
+                self.send_channel.assert_not_called()
 
-    def test_notification(self) -> None:
-        self.assertEqual(len(self.collection), 0)
 
-        response: TestResponse = self.client.put(json={"jsonrpc": "2.0", "method": "append", "params": ["hello world"]})
-        self.assertEqual(response.status_code, HTTPStatus.NO_CONTENT)
-        self.assertEqual(response.data, b"")
-        self.assertIn("hello world", self.collection)
+class TestHTTPHandler(IsolatedAsyncioTestCase):
+    @property
+    def random_id(self) -> str:
+        uuid: Final[UUID] = uuid4()
+        return str(uuid)
 
-    def test_large_request_body(self) -> None:
-        for payload in (
-            payload0 := urandom(10 * 1024 * 1024).hex(),
-            payload1 := urandom(10 * 1024 * 1024).hex(),
-            payload2 := urandom(10 * 1024 * 1024).hex(),
-            payload3 := urandom(10 * 1024 * 1024).hex(),
-            payload4 := urandom(10 * 1024 * 1024).hex(),
+    def setUp(self) -> None:
+        self.app: ASGIHandler = ASGIHandler()
+        self.client: AsyncClient = AsyncClient(
+            app=self.app,
+            base_url="http://testserver",
+            headers={"Content-Type": "application/json"},
+        )
+
+    async def asyncSetUp(self) -> None:
+        await self.enterAsyncContext(self.client)
+
+    async def test_negotiate_content_405(self) -> None:
+        for request in (
+            self.client.build_request(HTTPMethod.HEAD, "/testHead"),
+            self.client.build_request(HTTPMethod.GET, "/testGet"),
+            self.client.build_request(HTTPMethod.PATCH, "/testPatch", content=b""),
+            self.client.build_request(HTTPMethod.DELETE, "/testDelete", content=b""),
+            self.client.build_request(HTTPMethod.OPTIONS, "/testOptions"),
+            self.client.build_request(HTTPMethod.TRACE, "/testTrace"),
         ):
-            with self.subTest(payload=payload):
-                self.assertNotIn(payload, self.collection)
-
-        response: TestResponse = self.client.put(
-            json=[
-                {"jsonrpc": "2.0", "method": "append", "params": [payload0]},
-                {"jsonrpc": "2.0", "method": "append", "params": [payload1]},
-                {"jsonrpc": "2.0", "method": "append", "params": [payload2]},
-                {"jsonrpc": "2.0", "method": "append", "params": [payload3]},
-                {"jsonrpc": "2.0", "method": "append", "params": [payload4]},
-            ]
-        )
-        self.assertEqual(response.status_code, HTTPStatus.NO_CONTENT)
-        self.assertEqual(response.data, b"")
-
-        for payload in (payload0, payload1, payload2, payload3, payload4):
-            with self.subTest(payload=payload):
-                self.assertIn(payload, self.collection)
-
-    def test_unexpected_client_disconnected(self) -> None:
-        with StringIO() as raw_buffer:
-            request: EnvironBuilder = EnvironBuilder(
-                method="PUT",
-                errors_stream=raw_buffer,
-                environ_overrides={"CONTENT_LENGTH": "1000"},
-                json={
-                    "jsonrpc": "2.0",
-                    "method": "append",
-                    "params": ["Unexpected client disconnected"],
-                },
-            )
-
-            with self.assertRaises(EOFError) as context:
-                self.client.open(request)
-
-            self.assertNotIn("Unexpected client disconnected", self.collection)
-            self.assertIn("Client disconnected", str(context.exception))
-            self.assertIn("more bytes were expected", raw_buffer.getvalue())
+            with self.subTest(request=request):
+                response: Response = await self.client.send(request)
+                self.assertEqual(response.status_code, HTTPStatus.METHOD_NOT_ALLOWED)
+                self.assertEqual(response.headers["Allow"], HTTPMethod.POST)
+                self.assertEqual(response.content, b"")
 
-    def test_non_existent_method(self) -> None:
-        uuid: str = self.random_id
-        response: TestResponse = self.client.post(json={"jsonrpc": "2.0", "method": "foobar", "id": uuid})
-        self.assertEqual(response.status_code, HTTPStatus.OK)
-        self.assertTrue(response.is_json)
-        self.assertDictEqual(
-            response.json,
-            {
-                "jsonrpc": "2.0",
-                "error": {"code": ErrorEnum.METHOD_NOT_FOUND, "message": AnyNonEmptyString(self)},
-                "id": uuid,
-            },
-        )
+    async def test_negotiate_content_415(self) -> None:
+        for request in (
+            self.client.build_request(HTTPMethod.POST, "/", headers={"Content-Type": "multipart/form-data"}),
+            self.client.build_request(HTTPMethod.POST, "/", headers={"Content-Type": "text/plain"}),
+        ):
+            with self.subTest(request=request):
+                response: Response = await self.client.send(request)
+                self.assertEqual(response.status_code, HTTPStatus.UNSUPPORTED_MEDIA_TYPE)
+                self.assertEqual(response.content, b"")
+
+    async def test_request_aborted(self) -> None:
+        scope: dict[str, Any] = {
+            "type": "http",
+            "asgi": {"version": "3.0"},
+            "http_version": "1.1",
+            "method": "POST",
+            "scheme": "http",
+            "path": "/",
+            "headers": [],
+        }
+        receive_channel: Queue[Any] = Queue()
+        receive_channel.put_nowait({"type": "http.request", "body": b"", "more_body": True})
+        receive_channel.put_nowait({"type": "http.disconnect"})
+        send_channel: AsyncMock = AsyncMock()
+
+        await self.app(scope, receive_channel.get, send_channel)
+        send_channel.assert_not_called()
+
+    async def test_empty_request(self) -> None:
+        response: Response = await self.client.post("/", content=b"")
+        self.assertEqual(response.status_code, HTTPStatus.BAD_REQUEST)
+        self.assertEqual(response.content, b"")
 
-    def test_invalid_json(self) -> None:
-        response: TestResponse = self.client.post(data=b'{"jsonrpc": "2.0", "method": "foobar, "params": "bar", "baz]')
+    async def test_invalid_json(self) -> None:
+        response: Response = await self.client.post("/", content=b'{"jsonrpc": "2.0", "method": "foobar, "params": "bar", "baz]')
         self.assertEqual(response.status_code, HTTPStatus.OK)
-        self.assertTrue(response.is_json)
         self.assertDictEqual(
-            response.json,
+            response.json(),
             {
                 "jsonrpc": "2.0",
                 "error": {"code": ErrorEnum.PARSE_ERROR, "message": AnyNonEmptyString(self)},
                 "id": None,
             },
         )
 
-    def test_invalid_request_object(self) -> None:
-        response: TestResponse = self.client.post(json={"jsonrpc": "2.0", "method": 1, "params": "bar"})
+    async def test_invalid_request_object(self) -> None:
+        response: Response = await self.client.post("/", json={"jsonrpc": "2.0", "method": 1, "params": "bar"})
         self.assertEqual(response.status_code, HTTPStatus.OK)
-        self.assertTrue(response.is_json)
         self.assertDictEqual(
-            response.json,
+            response.json(),
             {
                 "jsonrpc": "2.0",
                 "error": {"code": ErrorEnum.INVALID_REQUEST, "message": AnyNonEmptyString(self)},
                 "id": None,
             },
         )
 
-    def test_batch_invalid_json(self) -> None:
-        response: TestResponse = self.client.post(
-            data=b"""
-        [
-            {"jsonrpc": "2.0", "method": "sum", "params": [8192, 1024], "id": 4}
-            {"jsonrpc": "2.0", "method"
-        ]
-        """
-        )
-        self.assertEqual(response.status_code, HTTPStatus.OK)
-        self.assertTrue(response.is_json)
-        self.assertDictEqual(
-            response.json,
-            {
-                "jsonrpc": "2.0",
-                "error": {"code": ErrorEnum.PARSE_ERROR, "message": AnyNonEmptyString(self)},
-                "id": None,
-            },
-        )
-
-    def test_empty_array(self) -> None:
-        response: TestResponse = self.client.post(json=[])
+    async def test_empty_array(self) -> None:
+        response: Response = await self.client.post("/", json=[])
         self.assertEqual(response.status_code, HTTPStatus.OK)
-        self.assertTrue(response.is_json)
         self.assertDictEqual(
-            response.json,
+            response.json(),
             {
                 "jsonrpc": "2.0",
                 "error": {"code": ErrorEnum.INVALID_REQUEST, "message": AnyNonEmptyString(self), "data": []},
                 "id": None,
             },
         )
 
-    def test_invalid_not_empty_batch(self) -> None:
-        response: TestResponse = self.client.post(json=[1])
+    async def test_invalid_not_empty_batch(self) -> None:
+        response: Response = await self.client.post("/", json=[1])
         self.assertEqual(response.status_code, HTTPStatus.OK)
-        self.assertTrue(response.is_json)
         self.assertCountEqual(
-            response.json,
+            response.json(),
             [
                 {
                     "jsonrpc": "2.0",
                     "error": {"code": ErrorEnum.INVALID_REQUEST, "message": AnyNonEmptyString(self), "data": 1},
                     "id": None,
                 }
             ],
         )
 
-    def test_invalid_batch(self) -> None:
-        response: TestResponse = self.client.post(json=[1, 2, 3])
+    async def test_invalid_batch(self) -> None:
+        response: Response = await self.client.post("/", json=[1, 2, 3])
         self.assertEqual(response.status_code, HTTPStatus.OK)
-        self.assertTrue(response.is_json)
         self.assertCountEqual(
-            response.json,
+            response.json(),
             [
                 {
                     "jsonrpc": "2.0",
                     "error": {"code": ErrorEnum.INVALID_REQUEST, "message": AnyNonEmptyString(self), "data": 1},
                     "id": None,
                 },
                 {
@@ -296,25 +178,183 @@
                     "jsonrpc": "2.0",
                     "error": {"code": ErrorEnum.INVALID_REQUEST, "message": AnyNonEmptyString(self), "data": 3},
                     "id": None,
                 },
             ],
         )
 
-    def test_invalid_json_response(self) -> None:
-        self.application.dispatcher.register(lambda: object(), function_name="lambda")
+    async def test_method_not_found(self) -> None:
+        uuid: str = self.random_id
+        response: Response = await self.client.post("/", json={"jsonrpc": "2.0", "method": "foobar", "id": uuid})
+        self.assertEqual(response.status_code, HTTPStatus.OK)
+        self.assertDictEqual(
+            response.json(),
+            {
+                "jsonrpc": "2.0",
+                "error": {"code": ErrorEnum.METHOD_NOT_FOUND, "message": AnyNonEmptyString(self)},
+                "id": uuid,
+            },
+        )
+
+    async def test_invalid_parameters_args(self) -> None:
+        mock: AsyncMock = AsyncMock()
 
-        response: TestResponse = self.client.post(json={"jsonrpc": "2.0", "method": "lambda", "id": self.random_id})
+        @self.app.dispatcher.register(function_name="args_only")
+        async def _(*args: Any) -> Any:
+            return await mock(*args)
+
+        uuid: str = self.random_id
+        response: Response = await self.client.post(
+            "/",
+            json={
+                "jsonrpc": "2.0",
+                "method": "args_only",
+                "params": {"a": 1, "b": 2},
+                "id": uuid,
+            },
+        )
+        self.assertEqual(response.status_code, HTTPStatus.OK)
+        self.assertDictEqual(
+            response.json(),
+            {
+                "jsonrpc": "2.0",
+                "error": {"code": ErrorEnum.INVALID_PARAMETERS, "message": AnyNonEmptyString(self)},
+                "id": uuid,
+            },
+        )
+        mock.assert_not_called()
+
+    async def test_invalid_parameters_kwargs(self) -> None:
+        mock: AsyncMock = AsyncMock()
+
+        @self.app.dispatcher.register(function_name="kwargs_only")
+        async def _(**kwargs: Any) -> Any:
+            return await mock(**kwargs)
+
+        uuid: str = self.random_id
+        response: Response = await self.client.post(
+            "/",
+            json={
+                "jsonrpc": "2.0",
+                "method": "kwargs_only",
+                "params": [1, 2, 3],
+                "id": uuid,
+            },
+        )
+        self.assertEqual(response.status_code, HTTPStatus.OK)
+        self.assertDictEqual(
+            response.json(),
+            {
+                "jsonrpc": "2.0",
+                "error": {"code": ErrorEnum.INVALID_PARAMETERS, "message": AnyNonEmptyString(self)},
+                "id": uuid,
+            },
+        )
+        mock.assert_not_called()
+
+    async def test_unexpected_internal_error(self) -> None:
+        mock: AsyncMock = AsyncMock(side_effect=Exception("for testing purposes"))
+
+        @self.app.dispatcher.register(function_name="exception")
+        async def _(**kwargs: Any) -> Any:
+            return await mock(**kwargs)
+
+        uuid: str = self.random_id
+        response: Response = await self.client.post("/", json={"jsonrpc": "2.0", "method": "exception", "id": uuid})
         self.assertEqual(response.status_code, HTTPStatus.OK)
-        self.assertTrue(response.is_json)
         self.assertDictEqual(
-            response.json,
+            response.json(),
+            {
+                "jsonrpc": "2.0",
+                "error": {"code": ErrorEnum.INTERNAL_ERROR, "message": AnyNonEmptyString(self)},
+                "id": uuid,
+            },
+        )
+        mock.assert_called_once()
+
+    async def test_positional_parameters(self) -> None:
+        mock: AsyncMock = AsyncMock(return_value=True)
+
+        @self.app.dispatcher.register(function_name="mock")
+        async def _(*args: Any, **kwargs: Any) -> bool:
+            return await mock(*args, **kwargs)
+
+        uuid: str = self.random_id
+        response: Response = await self.client.post(
+            "/",
+            json={
+                "jsonrpc": "2.0",
+                "method": "mock",
+                "params": [1, 2, 3],
+                "id": uuid,
+            },
+        )
+        self.assertEqual(response.status_code, HTTPStatus.OK)
+        self.assertDictEqual(response.json(), {"jsonrpc": "2.0", "result": True, "id": uuid})
+        mock.assert_awaited_once_with(1, 2, 3)
+
+    async def test_named_parameters(self) -> None:
+        mock: AsyncMock = AsyncMock(return_value=False)
+
+        @self.app.dispatcher.register(function_name="mock")
+        async def _(*args: Any, **kwargs: Any) -> bool:
+            return await mock(*args, **kwargs)
+
+        uuid: str = self.random_id
+        response: Response = await self.client.post(
+            "/",
+            json={
+                "jsonrpc": "2.0",
+                "method": "mock",
+                "params": {"a": 1, "b": 2, "c": 3},
+                "id": uuid,
+            },
+        )
+        self.assertEqual(response.status_code, HTTPStatus.OK)
+        self.assertDictEqual(response.json(), {"jsonrpc": "2.0", "result": False, "id": uuid})
+        mock.assert_awaited_once_with(a=1, b=2, c=3)
+
+    async def test_notification(self) -> None:
+        loop, mock, event = get_running_loop(), AsyncMock(), Event()
+
+        @self.app.dispatcher.register(function_name="mock")
+        async def _(*args: Any, **kwargs: Any) -> None:
+            try:
+                await mock(*args, **kwargs)
+            finally:
+                loop.call_soon(event.set)
+
+        response: Response = await self.client.post("/", json={"jsonrpc": "2.0", "method": "mock", "params": [1, 2, 3]})
+        await event.wait()
+        self.assertEqual(response.status_code, HTTPStatus.NO_CONTENT)
+        self.assertEqual(response.content, b"")
+        mock.assert_awaited_once_with(1, 2, 3)
+
+    async def test_invalid_json_response(self) -> None:
+        @self.app.dispatcher.register(function_name="object")
+        async def _() -> Any:
+            return object()
+
+        uuid: str = self.random_id
+        response: Response = await self.client.post("/", json={"jsonrpc": "2.0", "method": "object", "id": uuid})
+        self.assertEqual(response.status_code, HTTPStatus.OK)
+        self.assertDictEqual(
+            response.json(),
             {
                 "jsonrpc": "2.0",
                 "error": {"code": ErrorEnum.PARSE_ERROR, "message": AnyNonEmptyString(self)},
                 "id": None,
             },
         )
 
+    async def test_gateway_timeout(self) -> None:
+        @self.app.dispatcher.register(function_name="eternity")
+        async def _() -> None:
+            await wait_for(sleep(3600.0), timeout=0.001)
+
+        uuid: str = self.random_id
+        response: Response = await self.client.post("/", json={"jsonrpc": "2.0", "method": "eternity", "id": uuid})
+        self.assertEqual(response.status_code, HTTPStatus.GATEWAY_TIMEOUT)
+        self.assertEqual(response.content, b"")
+
     def tearDown(self) -> None:
-        self.application.dispatcher.clear()
-        self.collection.clear()
+        self.app.dispatcher.clear()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

