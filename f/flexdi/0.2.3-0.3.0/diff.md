# Comparing `tmp/flexdi-0.2.3.tar.gz` & `tmp/flexdi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexdi-0.2.3.tar", last modified: Sat Mar 11 00:31:47 2023, max compression
+gzip compressed data, was "flexdi-0.3.0.tar", last modified: Sun Apr 16 06:16:59 2023, max compression
```

## Comparing `flexdi-0.2.3.tar` & `flexdi-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-03-11 00:31:47.383259 flexdi-0.2.3/
--rw-rw-rw-   0        0        0     1087 2023-02-19 00:02:09.000000 flexdi-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     8062 2023-03-11 00:31:47.384260 flexdi-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     7565 2023-03-10 23:07:43.000000 flexdi-0.2.3/README.rst
--rw-rw-rw-   0        0        0      267 2023-02-20 19:54:06.000000 flexdi-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0      765 2023-03-11 00:31:47.389260 flexdi-0.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-11 00:31:47.328149 flexdi-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2023-03-11 00:31:47.349260 flexdi-0.2.3/src/flexdi/
--rw-rw-rw-   0        0        0      205 2023-03-10 23:17:08.000000 flexdi-0.2.3/src/flexdi/__init__.py
--rw-rw-rw-   0        0        0     4280 2023-03-11 00:21:49.000000 flexdi-0.2.3/src/flexdi/_bindable.py
--rw-rw-rw-   0        0        0     1946 2023-03-11 00:06:12.000000 flexdi-0.2.3/src/flexdi/_entrypoint.py
--rw-rw-rw-   0        0        0     2647 2023-03-11 00:21:49.000000 flexdi-0.2.3/src/flexdi/_graph.py
--rw-rw-rw-   0        0        0     1128 2023-03-10 23:17:08.000000 flexdi-0.2.3/src/flexdi/_implicit.py
--rw-rw-rw-   0        0        0      511 2023-03-11 00:06:12.000000 flexdi-0.2.3/src/flexdi/_openable.py
--rw-rw-rw-   0        0        0     1568 2023-03-11 00:06:12.000000 flexdi-0.2.3/src/flexdi/_resolvable.py
--rw-rw-rw-   0        0        0     6213 2023-03-11 00:21:49.000000 flexdi-0.2.3/src/flexdi/_rules.py
--rw-rw-rw-   0        0        0     5063 2023-03-11 00:21:49.000000 flexdi-0.2.3/src/flexdi/_scope.py
--rw-rw-rw-   0        0        0     1820 2023-03-10 23:17:08.000000 flexdi-0.2.3/src/flexdi/_store.py
--rw-rw-rw-   0        0        0      352 2023-03-11 00:06:12.000000 flexdi-0.2.3/src/flexdi/_types.py
--rw-rw-rw-   0        0        0     2620 2023-03-11 00:21:49.000000 flexdi-0.2.3/src/flexdi/_util.py
--rw-rw-rw-   0        0        0      183 2023-03-11 00:21:49.000000 flexdi-0.2.3/src/flexdi/errors.py
-drwxrwxrwx   0        0        0        0 2023-03-11 00:31:47.376259 flexdi-0.2.3/src/flexdi/fastapi/
--rw-rw-rw-   0        0        0     1495 2023-03-11 00:06:12.000000 flexdi-0.2.3/src/flexdi/fastapi/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-18 17:47:12.000000 flexdi-0.2.3/src/flexdi/py.typed
-drwxrwxrwx   0        0        0        0 2023-03-11 00:31:47.374260 flexdi-0.2.3/src/flexdi.egg-info/
--rw-rw-rw-   0        0        0     8062 2023-03-11 00:31:47.000000 flexdi-0.2.3/src/flexdi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      711 2023-03-11 00:31:47.000000 flexdi-0.2.3/src/flexdi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-11 00:31:47.000000 flexdi-0.2.3/src/flexdi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-03-11 00:31:47.000000 flexdi-0.2.3/src/flexdi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-11 00:31:47.000000 flexdi-0.2.3/src/flexdi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-11 00:31:47.383259 flexdi-0.2.3/tests/
--rw-rw-rw-   0        0        0      781 2023-02-25 07:13:33.000000 flexdi-0.2.3/tests/test_app_fastapi.py
--rw-rw-rw-   0        0        0     1056 2023-02-25 02:57:18.000000 flexdi-0.2.3/tests/test_app_override.py
--rw-rw-rw-   0        0        0     3315 2023-03-03 01:43:26.000000 flexdi-0.2.3/tests/test_fastapi.py
--rw-rw-rw-   0        0        0    19837 2023-03-11 00:06:12.000000 flexdi-0.2.3/tests/test_graph.py
--rw-rw-rw-   0        0        0       61 2023-02-20 18:11:50.000000 flexdi-0.2.3/tests/test_module.py
--rw-rw-rw-   0        0        0     1876 2023-03-03 01:43:26.000000 flexdi-0.2.3/tests/test_scope.py
--rw-rw-rw-   0        0        0     1796 2023-03-10 23:17:08.000000 flexdi-0.2.3/tests/test_util.py
+drwxrwxrwx   0        0        0        0 2023-04-16 06:16:59.159244 flexdi-0.3.0/
+-rw-rw-rw-   0        0        0     1087 2023-02-19 00:02:09.000000 flexdi-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     8084 2023-04-16 06:16:59.160245 flexdi-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7565 2023-03-10 23:07:43.000000 flexdi-0.3.0/README.rst
+-rw-rw-rw-   0        0        0      267 2023-02-20 19:54:06.000000 flexdi-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0      880 2023-04-16 06:16:59.165245 flexdi-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 06:16:59.115244 flexdi-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 06:16:59.131246 flexdi-0.3.0/src/flexdi/
+-rw-rw-rw-   0        0        0      205 2023-03-10 23:17:08.000000 flexdi-0.3.0/src/flexdi/__init__.py
+-rw-rw-rw-   0        0        0     4276 2023-03-11 20:20:32.000000 flexdi-0.3.0/src/flexdi/_bindable.py
+-rw-rw-rw-   0        0        0     1946 2023-03-11 00:06:12.000000 flexdi-0.3.0/src/flexdi/_entrypoint.py
+-rw-rw-rw-   0        0        0     2814 2023-03-11 20:20:32.000000 flexdi-0.3.0/src/flexdi/_graph.py
+-rw-rw-rw-   0        0        0     1128 2023-03-10 23:17:08.000000 flexdi-0.3.0/src/flexdi/_implicit.py
+-rw-rw-rw-   0        0        0      511 2023-03-11 00:06:12.000000 flexdi-0.3.0/src/flexdi/_openable.py
+-rw-rw-rw-   0        0        0     1725 2023-03-11 20:20:32.000000 flexdi-0.3.0/src/flexdi/_resolvable.py
+-rw-rw-rw-   0        0        0     6213 2023-03-11 00:21:49.000000 flexdi-0.3.0/src/flexdi/_rules.py
+-rw-rw-rw-   0        0        0     5935 2023-03-11 20:20:32.000000 flexdi-0.3.0/src/flexdi/_scope.py
+-rw-rw-rw-   0        0        0     1820 2023-03-10 23:17:08.000000 flexdi-0.3.0/src/flexdi/_store.py
+-rw-rw-rw-   0        0        0      352 2023-03-11 00:06:12.000000 flexdi-0.3.0/src/flexdi/_types.py
+-rw-rw-rw-   0        0        0     2620 2023-03-11 00:21:49.000000 flexdi-0.3.0/src/flexdi/_util.py
+-rw-rw-rw-   0        0        0      183 2023-03-11 00:21:49.000000 flexdi-0.3.0/src/flexdi/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-16 06:16:59.150249 flexdi-0.3.0/src/flexdi/fastapi/
+-rw-rw-rw-   0        0        0     1495 2023-03-11 00:06:12.000000 flexdi-0.3.0/src/flexdi/fastapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 06:16:59.151243 flexdi-0.3.0/src/flexdi/flask/
+-rw-rw-rw-   0        0        0     1096 2023-03-11 20:20:32.000000 flexdi-0.3.0/src/flexdi/flask/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 06:16:59.152246 flexdi-0.3.0/src/flexdi/grpc/
+-rw-rw-rw-   0        0        0      844 2023-04-16 06:15:17.000000 flexdi-0.3.0/src/flexdi/grpc/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-18 17:47:12.000000 flexdi-0.3.0/src/flexdi/py.typed
+drwxrwxrwx   0        0        0        0 2023-04-16 06:16:59.149246 flexdi-0.3.0/src/flexdi.egg-info/
+-rw-rw-rw-   0        0        0     8084 2023-04-16 06:16:59.000000 flexdi-0.3.0/src/flexdi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      815 2023-04-16 06:16:59.000000 flexdi-0.3.0/src/flexdi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 06:16:59.000000 flexdi-0.3.0/src/flexdi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-16 06:16:59.000000 flexdi-0.3.0/src/flexdi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-16 06:16:59.000000 flexdi-0.3.0/src/flexdi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 06:16:59.159244 flexdi-0.3.0/tests/
+-rw-rw-rw-   0        0        0      781 2023-02-25 07:13:33.000000 flexdi-0.3.0/tests/test_app_fastapi.py
+-rw-rw-rw-   0        0        0     1280 2023-04-16 06:15:17.000000 flexdi-0.3.0/tests/test_app_flask.py
+-rw-rw-rw-   0        0        0     1097 2023-04-16 06:15:17.000000 flexdi-0.3.0/tests/test_app_grpc.py
+-rw-rw-rw-   0        0        0     1088 2023-04-16 06:15:17.000000 flexdi-0.3.0/tests/test_app_override.py
+-rw-rw-rw-   0        0        0     3315 2023-03-03 01:43:26.000000 flexdi-0.3.0/tests/test_fastapi.py
+-rw-rw-rw-   0        0        0    19837 2023-03-11 00:06:12.000000 flexdi-0.3.0/tests/test_graph.py
+-rw-rw-rw-   0        0        0       61 2023-02-20 18:11:50.000000 flexdi-0.3.0/tests/test_module.py
+-rw-rw-rw-   0        0        0     1876 2023-03-03 01:43:26.000000 flexdi-0.3.0/tests/test_scope.py
+-rw-rw-rw-   0        0        0     1796 2023-03-10 23:17:08.000000 flexdi-0.3.0/tests/test_util.py
```

### Comparing `flexdi-0.2.3/LICENSE` & `flexdi-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flexdi-0.2.3/PKG-INFO` & `flexdi-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: flexdi
-Version: 0.2.3
+Version: 0.3.0
 Summary: A flexible dependency injection tool for typed Python projects.
 Home-page: https://github.com/cal-pratt/flexdi
 Author: Cal Pratt
 Author-email: ccpratt4@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Provides-Extra: grpc
 License-File: LICENSE
 
 
 Flex DI
 =======
 
 .. image:: https://img.shields.io/pypi/v/flexdi.svg
```

### Comparing `flexdi-0.2.3/README.rst` & `flexdi-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `flexdi-0.2.3/setup.cfg` & `flexdi-0.3.0/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2066 6c65 7864 690d 0a76 6572 7369   = flexdi..versi
-00000020: 6f6e 203d 2030 2e32 2e33 0d0a 6465 7363  on = 0.2.3..desc
+00000020: 6f6e 203d 2030 2e33 2e30 0d0a 6465 7363  on = 0.3.0..desc
 00000030: 7269 7074 696f 6e20 3d20 4120 666c 6578  ription = A flex
 00000040: 6962 6c65 2064 6570 656e 6465 6e63 7920  ible dependency 
 00000050: 696e 6a65 6374 696f 6e20 746f 6f6c 2066  injection tool f
 00000060: 6f72 2074 7970 6564 2050 7974 686f 6e20  or typed Python 
 00000070: 7072 6f6a 6563 7473 2e0d 0a6c 6f6e 675f  projects...long_
 00000080: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
 00000090: 6c65 3a20 5245 4144 4d45 2e72 7374 0d0a  le: README.rst..
@@ -32,17 +32,24 @@
 000001f0: 5f64 6972 203d 200d 0a09 3d73 7263 0d0a  _dir = ...=src..
 00000200: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
 00000210: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
 00000220: 6573 203d 200d 0a09 7479 7069 6e67 2d65  es = ...typing-e
 00000230: 7874 656e 7369 6f6e 7320 3e3d 2034 0d0a  xtensions >= 4..
 00000240: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
 00000250: 3d20 3e3d 332e 380d 0a0d 0a5b 6f70 7469  = >=3.8....[opti
-00000260: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
-00000270: 645d 0d0a 7768 6572 6520 3d20 7372 630d  d]..where = src.
-00000280: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
-00000290: 6167 655f 6461 7461 5d0d 0a66 6c65 7864  age_data]..flexd
-000002a0: 6920 3d20 7079 2e74 7970 6564 0d0a 0d0a  i = py.typed....
-000002b0: 5b66 6c61 6b65 385d 0d0a 6d61 782d 6c69  [flake8]..max-li
-000002c0: 6e65 2d6c 656e 6774 6820 3d20 3130 300d  ne-length = 100.
-000002d0: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-000002e0: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-000002f0: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+00000260: 6f6e 732e 6578 7472 6173 5f72 6571 7569  ons.extras_requi
+00000270: 7265 5d0d 0a67 7270 6320 3d20 0d0a 0967  re]..grpc = ...g
+00000280: 7270 632d 696e 7465 7263 6570 746f 7220  rpc-interceptor 
+00000290: 3e3d 2030 2e31 350d 0a09 6772 7063 696f  >= 0.15...grpcio
+000002a0: 203e 3d20 312e 3434 0d0a 0d0a 5b6f 7074   >= 1.44....[opt
+000002b0: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
+000002c0: 6e64 5d0d 0a77 6865 7265 203d 2073 7263  nd]..where = src
+000002d0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
+000002e0: 6b61 6765 5f64 6174 615d 0d0a 666c 6578  kage_data]..flex
+000002f0: 6469 203d 2070 792e 7479 7065 640d 0a0d  di = py.typed...
+00000300: 0a5b 666c 616b 6538 5d0d 0a6d 6178 2d6c  .[flake8]..max-l
+00000310: 696e 652d 6c65 6e67 7468 203d 2031 3030  ine-length = 100
+00000320: 0d0a 6578 636c 7564 6520 3d20 2a5f 7062  ..exclude = *_pb
+00000330: 322e 7079 2c2a 5f70 6232 5f67 7270 632e  2.py,*_pb2_grpc.
+00000340: 7079 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  py....[egg_info]
+00000350: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+00000360: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

### Comparing `flexdi-0.2.3/src/flexdi/_bindable.py` & `flexdi-0.3.0/src/flexdi/_bindable.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,9 +122,9 @@
         :return: The unedited value supplied.
         """
 
         if self.opened:
             raise FlexError("FlexGraph opened. Cannot be bound.")
 
         self._rules.add_binding(func := lambda: value, resolves or type(value))
-        self._rules.add_policy(func, scope="application", eager=True)
+        self._rules.add_policy(func, scope="request", eager=True)
         return value
```

### Comparing `flexdi-0.2.3/src/flexdi/_entrypoint.py` & `flexdi-0.3.0/src/flexdi/_entrypoint.py`

 * *Files identical despite different names*

### Comparing `flexdi-0.2.3/src/flexdi/_graph.py` & `flexdi-0.3.0/src/flexdi/_graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from contextlib import contextmanager
-from typing import Iterator, TypeVar
+from typing import Any, Dict, Iterator, TypeVar
 
 from ._bindable import BindableMixin
 from ._entrypoint import EntrypointMixin
 from ._rules import FlexRules
 from ._scope import ApplicationScope
 from ._types import Func, Instance
 
@@ -44,14 +44,17 @@
 
     def application_scope(self) -> ApplicationScope:
         return ApplicationScope(self._rules.clone())
 
     async def _resolve(self, func: Func) -> Instance:
         return await self.application_scope().resolve(func)
 
+    async def resolve_args(self, func: Func, **extra: Any) -> Dict[str, Any]:
+        return await self.application_scope().resolve_args(func, **extra)
+
     @contextmanager
     def override(self) -> Iterator["FlexGraph"]:
         """
         This context manager is primarily intended for testing use-cases.
 
         An override allow users to override dependency bindings a temporary way
         which will be reverted when the override is closed. This prevents making
```

### Comparing `flexdi-0.2.3/src/flexdi/_implicit.py` & `flexdi-0.3.0/src/flexdi/_implicit.py`

 * *Files identical despite different names*

### Comparing `flexdi-0.2.3/src/flexdi/_resolvable.py` & `flexdi-0.3.0/src/flexdi/_resolvable.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from abc import ABC, abstractmethod
 from typing import (
     Any,
     AsyncIterator,
     Awaitable,
     Callable,
+    Dict,
     Iterator,
     Type,
     TypeVar,
     cast,
     overload,
 )
 
@@ -56,7 +57,13 @@
         """
 
         return cast(T, await self._resolve(func))
 
     @abstractmethod
     async def _resolve(self, func: Callable[..., Any]) -> Any:
         pass
+
+    @abstractmethod
+    async def resolve_args(
+        self, func: Callable[..., Any], **extra: Any
+    ) -> Dict[str, Any]:
+        pass
```

### Comparing `flexdi-0.2.3/src/flexdi/_rules.py` & `flexdi-0.3.0/src/flexdi/_rules.py`

 * *Files identical despite different names*

### Comparing `flexdi-0.2.3/src/flexdi/_scope.py` & `flexdi-0.3.0/src/flexdi/_scope.py`

 * *Files 15% similar despite different names*

```diff
@@ -87,22 +87,28 @@
                 raise FlexError(
                     "Could not resolve scope for func "
                     f"{func} in scope {policy.scope}"
                 )
 
         async with self._store.lock(func):
             if func not in self._store:
-                args: Dict[str, Any] = {}
-                for name, clazz in parse_signature(func).items():
-                    args[name] = await self._scope_resolve(clazz)
-
+                args = await self._scope_resolve_args(func)
                 await self._store.create(func, args)
 
         return self._store[func]
 
+    async def _scope_resolve_args(self, func: Func, **extra: Any) -> Dict[str, Any]:
+        args: Dict[str, Any] = dict(extra)
+        for name, clazz in parse_signature(func).items():
+            if name not in args:
+                # Note that the extra args are not propagated.
+                # You can only enhance the first level of resolution.
+                args[name] = await self._scope_resolve(clazz)
+        return args
+
 
 class RequestScope(FlexScope, BindableMixin, ResolvableMixin):
     """
     The request scope is the storage for all request or unmarked scoped dependencies.
     If already opened, it can be called repeatedly to have cached calls.
     """
 
@@ -111,14 +117,20 @@
 
     async def _resolve(self, func: Func) -> Instance:
         if self.opened:
             return await self._scope_resolve(func)
         async with self:
             return await self._scope_resolve(func)
 
+    async def resolve_args(self, func: Func, **extra: Any) -> Dict[str, Any]:
+        if self.opened:
+            return await self._scope_resolve_args(func, **extra)
+        async with self:
+            return await self._scope_resolve_args(func, **extra)
+
 
 class ApplicationScope(FlexScope, BindableMixin, ResolvableMixin):
     """
     The application scope is the storage for all application scoped dependencies.
     For higher stricter scoped dependencies it will defer to the request scope.
     """
 
@@ -131,7 +143,13 @@
         return RequestScope(self._rules.clone(), self)
 
     async def _resolve(self, func: Func) -> Instance:
         if self.opened:
             return await self.request_scope().resolve(func)
         async with self:
             return await self.request_scope().resolve(func)
+
+    async def resolve_args(self, func: Func, **extra: Any) -> Dict[str, Any]:
+        if self.opened:
+            return await self.request_scope().resolve_args(func, **extra)
+        async with self:
+            return await self.request_scope().resolve_args(func, **extra)
```

### Comparing `flexdi-0.2.3/src/flexdi/_store.py` & `flexdi-0.3.0/src/flexdi/_store.py`

 * *Files identical despite different names*

### Comparing `flexdi-0.2.3/src/flexdi/_util.py` & `flexdi-0.3.0/src/flexdi/_util.py`

 * *Files identical despite different names*

### Comparing `flexdi-0.2.3/src/flexdi/fastapi/__init__.py` & `flexdi-0.3.0/src/flexdi/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `flexdi-0.2.3/src/flexdi.egg-info/PKG-INFO` & `flexdi-0.3.0/src/flexdi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: flexdi
-Version: 0.2.3
+Version: 0.3.0
 Summary: A flexible dependency injection tool for typed Python projects.
 Home-page: https://github.com/cal-pratt/flexdi
 Author: Cal Pratt
 Author-email: ccpratt4@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Provides-Extra: grpc
 License-File: LICENSE
 
 
 Flex DI
 =======
 
 .. image:: https://img.shields.io/pypi/v/flexdi.svg
```

### Comparing `flexdi-0.2.3/src/flexdi.egg-info/SOURCES.txt` & `flexdi-0.3.0/src/flexdi.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,18 @@
 src/flexdi/py.typed
 src/flexdi.egg-info/PKG-INFO
 src/flexdi.egg-info/SOURCES.txt
 src/flexdi.egg-info/dependency_links.txt
 src/flexdi.egg-info/requires.txt
 src/flexdi.egg-info/top_level.txt
 src/flexdi/fastapi/__init__.py
+src/flexdi/flask/__init__.py
+src/flexdi/grpc/__init__.py
 tests/test_app_fastapi.py
+tests/test_app_flask.py
+tests/test_app_grpc.py
 tests/test_app_override.py
 tests/test_fastapi.py
 tests/test_graph.py
 tests/test_module.py
 tests/test_scope.py
 tests/test_util.py
```

### Comparing `flexdi-0.2.3/tests/test_app_fastapi.py` & `flexdi-0.3.0/tests/test_app_fastapi.py`

 * *Files identical despite different names*

### Comparing `flexdi-0.2.3/tests/test_app_override.py` & `flexdi-0.3.0/tests/test_app_override.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 from typing import Iterator
 
 import pytest
 from _pytest.capture import CaptureFixture
 
 from flexdi import FlexGraph
 
-from .test_app import app
+from .test_app import app_cli
 
 
 class MockClient:
     def foo(self) -> str:
         return "bar"
 
 
 @pytest.fixture
 def graph() -> Iterator[FlexGraph]:
-    with app.graph.override():
-        yield app.graph
+    with app_cli.graph.override():
+        yield app_cli.graph
 
 
 @pytest.fixture
 def mock_client(graph: FlexGraph) -> MockClient:
-    return graph.bind_instance(MockClient(), resolves=app.ApiClient)
+    return graph.bind_instance(MockClient(), resolves=app_cli.ApiClient)
 
 
 def test_main_normal(capsys: CaptureFixture[str]) -> None:
-    app.main()
+    app_cli.main()
     assert capsys.readouterr().out == "foo\n"
 
 
 def test_main_override(mock_client: MockClient, capsys: CaptureFixture[str]) -> None:
-    app.main()
+    app_cli.main()
     assert capsys.readouterr().out == "bar\n"
 
 
 def test_main_again(capsys: CaptureFixture[str]) -> None:
-    app.main()
+    app_cli.main()
     assert capsys.readouterr().out == "foo\n"
 
 
 @pytest.mark.asyncio
 async def test_main_again_async(capsys: CaptureFixture[str]) -> None:
-    await app.main.aio()
+    await app_cli.main.aio()
     assert capsys.readouterr().out == "foo\n"
```

### Comparing `flexdi-0.2.3/tests/test_fastapi.py` & `flexdi-0.3.0/tests/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `flexdi-0.2.3/tests/test_graph.py` & `flexdi-0.3.0/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `flexdi-0.2.3/tests/test_scope.py` & `flexdi-0.3.0/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `flexdi-0.2.3/tests/test_util.py` & `flexdi-0.3.0/tests/test_util.py`

 * *Files identical despite different names*

