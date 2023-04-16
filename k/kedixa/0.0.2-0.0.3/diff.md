# Comparing `tmp/kedixa-0.0.2-py3-none-any.whl.zip` & `tmp/kedixa-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,39 +1,45 @@
-Zip file size: 31877 bytes, number of entries: 37
+Zip file size: 39214 bytes, number of entries: 43
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-28 08:01 kedixa/__init__.py
 -rw-r--r--  2.0 unx       46 b- defN 23-Mar-12 13:18 kedixa/compat.py
 -rw-r--r--  2.0 unx      877 b- defN 23-Feb-28 08:01 kedixa/file_loader.py
 -rw-r--r--  2.0 unx     3828 b- defN 23-Feb-28 08:01 kedixa/mprocess.py
--rw-r--r--  2.0 unx      145 b- defN 23-Apr-07 13:12 kedixa/version.py
--rw-r--r--  2.0 unx      286 b- defN 23-Apr-07 13:09 kedixa/comm/__init__.py
+-rw-r--r--  2.0 unx      145 b- defN 23-Apr-16 12:58 kedixa/version.py
+-rw-r--r--  2.0 unx      312 b- defN 23-Apr-16 11:42 kedixa/comm/__init__.py
 -rw-r--r--  2.0 unx     1623 b- defN 23-Mar-25 08:13 kedixa/comm/address.py
 -rw-r--r--  2.0 unx     6678 b- defN 23-Apr-07 10:56 kedixa/comm/basic.py
--rw-r--r--  2.0 unx     1525 b- defN 23-Apr-07 10:56 kedixa/comm/bridge.py
--rw-r--r--  2.0 unx     2043 b- defN 23-Apr-07 10:57 kedixa/comm/connection.py
+-rw-r--r--  2.0 unx     1537 b- defN 23-Apr-16 12:25 kedixa/comm/bridge.py
+-rw-r--r--  2.0 unx     2328 b- defN 23-Apr-16 12:38 kedixa/comm/connection.py
 -rw-r--r--  2.0 unx     1082 b- defN 23-Mar-18 17:04 kedixa/comm/debug_filter.py
--rw-r--r--  2.0 unx     1107 b- defN 23-Apr-07 10:57 kedixa/comm/debug_transformer.py
+-rw-r--r--  2.0 unx     1132 b- defN 23-Apr-09 03:30 kedixa/comm/debug_transformer.py
 -rw-r--r--  2.0 unx      771 b- defN 23-Apr-07 10:58 kedixa/comm/exception.py
 -rw-r--r--  2.0 unx     1162 b- defN 23-Mar-12 13:18 kedixa/comm/file_adaptor.py
 -rw-r--r--  2.0 unx     1929 b- defN 23-Mar-12 13:18 kedixa/comm/read_until_filter.py
 -rw-r--r--  2.0 unx     1969 b- defN 23-Apr-07 10:58 kedixa/comm/read_until_transformer.py
 -rw-r--r--  2.0 unx     3439 b- defN 23-Mar-25 08:01 kedixa/comm/socket_adaptor.py
 -rw-r--r--  2.0 unx     5294 b- defN 23-Feb-26 14:05 kedixa/comm/socks5_filter.py
 -rw-r--r--  2.0 unx     5310 b- defN 23-Apr-07 11:12 kedixa/comm/socks5_updater.py
+-rw-r--r--  2.0 unx     5311 b- defN 23-Apr-07 14:32 kedixa/comm/socks5_upgrader.py
 -rw-r--r--  2.0 unx     3487 b- defN 23-Mar-26 14:20 kedixa/comm/speed_limit_filter.py
 -rw-r--r--  2.0 unx     3507 b- defN 23-Apr-07 10:58 kedixa/comm/speed_limit_transformer.py
 -rw-r--r--  2.0 unx     2151 b- defN 23-Mar-12 13:18 kedixa/comm/ssl_filter.py
--rw-r--r--  2.0 unx     2171 b- defN 23-Apr-07 10:58 kedixa/comm/ssl_transformer.py
--rw-r--r--  2.0 unx      129 b- defN 23-Apr-07 13:09 kedixa/comm/http/__init__.py
+-rw-r--r--  2.0 unx     2348 b- defN 23-Apr-14 17:44 kedixa/comm/ssl_transformer.py
+-rw-r--r--  2.0 unx     3077 b- defN 23-Apr-16 11:43 kedixa/comm/tcp_server.py
+-rw-r--r--  2.0 unx      130 b- defN 23-Apr-07 14:42 kedixa/comm/http/__init__.py
 -rw-r--r--  2.0 unx     1996 b- defN 23-Apr-01 02:16 kedixa/comm/http/http_chunk_filter.py
--rw-r--r--  2.0 unx     2046 b- defN 23-Apr-07 10:59 kedixa/comm/http/http_chunk_transformer.py
+-rw-r--r--  2.0 unx     2066 b- defN 23-Apr-15 17:30 kedixa/comm/http/http_chunk_transformer.py
 -rw-r--r--  2.0 unx     2011 b- defN 23-Mar-18 06:37 kedixa/comm/http/http_code_map.py
 -rw-r--r--  2.0 unx    12688 b- defN 23-Apr-07 11:00 kedixa/comm/http/http_message.py
 -rw-r--r--  2.0 unx     2356 b- defN 23-Apr-01 02:17 kedixa/comm/http/http_proxy_filter.py
 -rw-r--r--  2.0 unx     2435 b- defN 23-Apr-07 11:10 kedixa/comm/http/http_proxy_updater.py
--rw-r--r--  2.0 unx       65 b- defN 23-Apr-06 10:25 kedixa/comm/websocket/__init__.py
--rw-r--r--  2.0 unx     6842 b- defN 23-Apr-06 10:37 kedixa/comm/websocket/websocket_client.py
+-rw-r--r--  2.0 unx     2437 b- defN 23-Apr-07 14:31 kedixa/comm/http/http_proxy_upgrader.py
+-rw-r--r--  2.0 unx      135 b- defN 23-Apr-08 15:33 kedixa/comm/websocket/__init__.py
+-rw-r--r--  2.0 unx     4524 b- defN 23-Apr-08 08:17 kedixa/comm/websocket/websocket_client.py
+-rw-r--r--  2.0 unx     4903 b- defN 23-Apr-09 03:17 kedixa/comm/websocket/websocket_handler.py
 -rw-r--r--  2.0 unx     3860 b- defN 23-Apr-01 03:14 kedixa/comm/websocket/websocket_message.py
--rw-r--r--  2.0 unx      227 b- defN 23-Apr-07 13:12 kedixa-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-07 13:12 kedixa-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-07 13:12 kedixa-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3117 b- defN 23-Apr-07 13:12 kedixa-0.0.2.dist-info/RECORD
-37 files, 88301 bytes uncompressed, 26885 bytes compressed:  69.6%
+-rw-r--r--  2.0 unx     6166 b- defN 23-Apr-15 08:48 kedixa/comm/websocket/websocket_processor.py
+-rw-r--r--  2.0 unx     2603 b- defN 23-Apr-09 02:01 kedixa/comm/websocket/websocket_upgrader.py
+-rw-r--r--  2.0 unx      227 b- defN 23-Apr-16 12:59 kedixa-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-16 12:59 kedixa-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-16 12:59 kedixa-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3683 b- defN 23-Apr-16 12:59 kedixa-0.0.3.dist-info/RECORD
+43 files, 111662 bytes uncompressed, 33320 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -51,26 +51,32 @@
 
 Filename: kedixa/comm/socks5_filter.py
 Comment: 
 
 Filename: kedixa/comm/socks5_updater.py
 Comment: 
 
+Filename: kedixa/comm/socks5_upgrader.py
+Comment: 
+
 Filename: kedixa/comm/speed_limit_filter.py
 Comment: 
 
 Filename: kedixa/comm/speed_limit_transformer.py
 Comment: 
 
 Filename: kedixa/comm/ssl_filter.py
 Comment: 
 
 Filename: kedixa/comm/ssl_transformer.py
 Comment: 
 
+Filename: kedixa/comm/tcp_server.py
+Comment: 
+
 Filename: kedixa/comm/http/__init__.py
 Comment: 
 
 Filename: kedixa/comm/http/http_chunk_filter.py
 Comment: 
 
 Filename: kedixa/comm/http/http_chunk_transformer.py
@@ -84,29 +90,41 @@
 
 Filename: kedixa/comm/http/http_proxy_filter.py
 Comment: 
 
 Filename: kedixa/comm/http/http_proxy_updater.py
 Comment: 
 
+Filename: kedixa/comm/http/http_proxy_upgrader.py
+Comment: 
+
 Filename: kedixa/comm/websocket/__init__.py
 Comment: 
 
 Filename: kedixa/comm/websocket/websocket_client.py
 Comment: 
 
+Filename: kedixa/comm/websocket/websocket_handler.py
+Comment: 
+
 Filename: kedixa/comm/websocket/websocket_message.py
 Comment: 
 
-Filename: kedixa-0.0.2.dist-info/METADATA
+Filename: kedixa/comm/websocket/websocket_processor.py
+Comment: 
+
+Filename: kedixa/comm/websocket/websocket_upgrader.py
+Comment: 
+
+Filename: kedixa-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: kedixa-0.0.2.dist-info/WHEEL
+Filename: kedixa-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: kedixa-0.0.2.dist-info/top_level.txt
+Filename: kedixa-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: kedixa-0.0.2.dist-info/RECORD
+Filename: kedixa-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kedixa/version.py

```diff
@@ -1,4 +1,4 @@
 __major_version__ = 0
 __minor_version__ = 0
-__bugfix_version__ = 2
+__bugfix_version__ = 3
 __version__ = f'{__major_version__}.{__minor_version__}.{__bugfix_version__}'
```

## kedixa/comm/__init__.py

```diff
@@ -7,7 +7,8 @@
 from .file_adaptor import *
 
 from .read_until_transformer import *
 from .ssl_transformer import *
 from .speed_limit_transformer import *
 
 from .bridge import *
+from .tcp_server import *
```

## kedixa/comm/bridge.py

```diff
@@ -45,12 +45,11 @@
 
             try:
                 nread: int = await self._from.read(rlen, buffer=buf)
             except (AdaptorEofError, TransformerEofError):
                 break
 
             with memoryview(buf) as view:
-                await self._to.write_all(view[:nread])
+                await self._to.write_all(view[:nread], flush=False)
 
             self._total_read += nread
             rlen = self._next_read_size()
-
```

## kedixa/comm/connection.py

```diff
@@ -14,25 +14,29 @@
 
 
 class Connection:
     def __init__(self, adaptor: BasicAdaptor, *,
             prepared: bool = False):
         self._adaptor: BasicAdaptor = adaptor
         self._comms: List[CommunicateBase] = []
-        self._opened: bool = prepared
+        self._closed: bool = not prepared
 
         self._c: CommunicateBase = self._adaptor
         self._lock: asyncio.Lock = asyncio.Lock()
         self._context = None
 
     @property
     def c(self) -> CommunicateBase:
         return self._c
 
     @property
+    def adaptor(self) -> BasicAdaptor:
+        return self._adaptor
+
+    @property
     def lock(self) -> asyncio.Lock:
         return self._lock
 
     @property
     def info(self) -> str:
         return 'TODO'
 
@@ -40,31 +44,38 @@
     def context(self):
         return self._context
 
     @context.setter
     def context(self, context):
         self._context = context
 
+    def closed(self) -> bool:
+        return self._closed
+
     async def open(self):
-        if not self._opened:
+        if self._closed:
             await self._adaptor.prepare()
-            self._opened = True
+            self._closed = False
 
     async def close(self):
-        if self._opened:
-            self._opened = False
+        if not self._closed:
+            self._closed = True
             try:
                 for comm in self._comms[::-1]:
                     await comm.finish()
+                self._comms.clear()
             except:
                 # force close if gracefully finish failed
                 self._comms.clear()
                 self._c = self._adaptor
                 await self._adaptor.finish()
                 raise
+            else:
+                self._c = self._adaptor
+                await self._adaptor.finish()
 
     async def bind(self, next: BasicTransformer):
         if len(self._comms) == 0:
             next.bind_next(self._adaptor)
         else:
             next.bind_next(self._comms[-1])
```

## kedixa/comm/debug_transformer.py

```diff
@@ -11,14 +11,15 @@
     'DebugTransformer',
 ]
 
 
 class DebugTransformer(BasicTransformer):
     def __init__(self, size_limit: int = 128):
         super().__init__()
+        # TODO self._log
         self._limit: int = size_limit
 
     async def write(self, buffer: ReadableBuffer) -> int:
         ret = await self._nxt.write(buffer)
         x = min(ret, self._limit)
         _log.debug('write len:%d data:%s', ret, buffer[:x])
         return ret
```

## kedixa/comm/ssl_transformer.py

```diff
@@ -5,14 +5,18 @@
     BasicTransformer,
     ReadableBuffer,
     ReadRetType,
     WritableBuffer,
     DEFAULT_MAX_READ_SIZE,
 )
 
+from .exception import (
+    TransformerEofError,
+)
+
 __all__ = [
     'SslTransformer',
 ]
 
 # _logger = logging.getLogger('kedixa.comm')
 
 
@@ -65,13 +69,17 @@
                 await self._do_want_read()
             except ssl.SSLWantWriteError:
                 await self._do_want_write()
             else:
                 break
 
         await self._do_want_write()
+
+        if not ret:
+            # the ssl is shutdown by remote
+            raise TransformerEofError('SslTransformerEof')
         return ret
 
     async def write(self, buffer: ReadableBuffer) -> int:
         wsz = self._ssl_obj.write(buffer)
         await self._do_want_write()
         return wsz
```

## kedixa/comm/http/__init__.py

```diff
@@ -1,4 +1,4 @@
 from .http_chunk_transformer import *
 from .http_code_map import *
 from .http_message import *
-from .http_proxy_updater import *
+from .http_proxy_upgrader import *
```

## kedixa/comm/http/http_chunk_transformer.py

```diff
@@ -55,16 +55,16 @@
         buf[:nread] = self._buf[:nread]
         del self._buf[:nread]
         self._buflen -= nread
         return buf if buffer is None else nread
 
     async def write(self, buffer: ReadableBuffer) -> int:
         blen = len(buffer)
-        buf = bytearray(str(blen).encode())
+        buf = bytearray(hex(blen).lstrip('0x').encode())
         buf.extend(b'\r\n')
         buf.extend(buffer)
         buf.extend(b'\r\n')
-        await self._nxt.write_all(buf)
+        return await self._nxt.write_all(buf)
 
     async def flush(self):
         await self._nxt.write(b'0\r\n\r\n')
         await self._nxt.flush()
```

## kedixa/comm/websocket/__init__.py

```diff
@@ -1,2 +1,4 @@
 from .websocket_message import *
-from .websocket_client import *
+from .websocket_upgrader import *
+from .websocket_processor import *
+from .websocket_handler import *
```

## kedixa/comm/websocket/websocket_client.py

```diff
@@ -1,57 +1,36 @@
 import asyncio
 import random
-import base64
-import hashlib
 import ssl
 from urllib.parse import urlparse
 from typing import (
     List,
     Tuple,
     Callable,
     Awaitable,
 )
 
 from .. import (
     Connection,
     TcpAdaptor,
-    SslFilter,
-    ReadUntilFilter,
+    SslTransformer,
+    ReadUntilTransformer,
 
     getaddrinfo,
 )
-from ..http import (
-    HttpRequest,
-    HttpResponse,
-)
 from .websocket_message import (
     WebSocketFrame,
     WebSocketOpcode,
 )
+from .websocket_upgrader import WebSocketUpgrader
 
 __all__ = [
-    'SEC_WS_APPEND',
-    'get_sec_ws_accept',
-    'get_sec_ws_pair',
     'WebSocketClient',
 ]
 
-SEC_WS_APPEND = '258EAFA5-E914-47DA-95CA-C5AB0DC85B11'
-
-def get_sec_ws_accept(key: str) -> str:
-    accept = key + SEC_WS_APPEND
-    accept = hashlib.sha1(accept.encode()).digest()
-    accept = base64.b64encode(accept).decode()
-    return accept
-
-def get_sec_ws_pair() -> Tuple[str, str]:
-    key = bytes(random.choices(range(0, 256), k=16))
-    key: str = base64.b64encode(key).decode()
-    return key, get_sec_ws_accept(key)
-
 def _ws_parse_url(url: str):
     u = urlparse(url)
     scheme = u.scheme.lower()
     assert scheme in ['ws', 'wss']
 
     host, port = u.hostname, u.port
     assert host is not None
@@ -64,130 +43,86 @@
 
     req_url: str = '/' if len(u.path) == 0 else u.path
     if len(u.query) > 0:
         req_url += '?' + u.query
 
     return scheme, host, port, req_url
 
-WsTextHandlerType = Callable[['WebSocketClient', str], Awaitable[None]]
-WsBinaryHandlerType = Callable[['WebSocketClient', bytes], Awaitable[None]]
-WsFramesHandlerType = Callable[['WebSocketClient', List[WebSocketFrame]], Awaitable[None]]
+
+class WebSocketHandlerBase:
+    async def on_frame(self, cli: 'WebSocketClient', frame: WebSocketFrame):
+        pass
+
 
 class WebSocketClient:
     def __init__(self, url: str, *,
             ssl_ctx: ssl.SSLContext = None,
             upgrade_headers: List[Tuple[str, str]] = None,
-            on_text: WsTextHandlerType = None,
-            on_binary: WsBinaryHandlerType = None,
-            on_frames: WsFramesHandlerType = None,
+            frame_handler: WebSocketHandlerBase,
             ):
         self._url : str = url
         self._ssl_ctx: ssl.SSLContext = ssl_ctx
-        self._on_text: WsTextHandlerType = on_text
-        self._on_binary: WsBinaryHandlerType = on_binary
-        self._on_frames: WsFramesHandlerType = on_frames
+        self._hdl: WebSocketHandlerBase = frame_handler
+
+        if self._hdl is None:
+            self._hdl = WebSocketHandlerBase()
 
         self._conn: Connection = None
         self._closed: bool = True
         self._recv_task: asyncio.Task = None
         self._context = None
+        self._lock = asyncio.Lock()
 
-        self._ex_hdrs: List[Tuple[str, str]] = \
-            upgrade_headers if upgrade_headers is not None else []
+        self._ex_hdrs: List[Tuple[str, str]] = upgrade_headers
+        if self._ex_hdrs is None:
+            self._ex_hdrs = []
 
     @property
     def context(self):
         return self._context
 
     @context.setter
     def context(self, context):
         self._context = context
 
     def closed(self) -> bool:
         return self._closed
 
-    async def _receive_msgs(self) -> List[WebSocketFrame]:
-        msgs = []
-        while True:
-            msg = WebSocketFrame()
-            await self._conn.request(None, msg)
-            msgs.append(msg)
-            if msg.fin:
-                break
-
-        return msgs
-
-    async def _handle_msg(self, msgs: List[WebSocketFrame]):
-        opcode = msgs[0].opcode
-        if opcode == WebSocketOpcode.TextFrame and self._on_text:
-            data = bytes().join([m.payload for m in msgs])
-            try:
-                data = data.decode()
-            except UnicodeDecodeError:
-                pass
-            await self._on_text(self, data)
-        elif opcode == WebSocketOpcode.BinaryFrame and self._on_binary:
-            data = bytes().join([m.payload for m in msgs])
-            await self._on_binary(self, data)
-        elif self._on_frames:
-            await self._on_frames(self, msgs)
-        else:
-            pass
-
     async def _process_msg(self):
         try:
             while not self.closed():
-                msgs = await self._receive_msgs()
-                if len(msgs) == 0:
-                    continue
-
-                await self._handle_msg(msgs)
+                msg = WebSocketFrame()
+                await self._conn.request(None, msg)
+                await self._hdl.on_frame(self, msg)
         except asyncio.CancelledError:
             return
+        except Exception as e:
+            # TODO close on exception
+            print(e)
+            pass
 
     async def _open(self):
         scheme, host, port, req_url = _ws_parse_url(self._url)
         addrs = await getaddrinfo(host, port)
 
         # TODO assert(len(addrs) > 0)
         self._conn = Connection(TcpAdaptor(addrs[0]))
 
         try:
             await self._conn.open()
 
             if scheme == 'wss':
                 if self._ssl_ctx is None:
                     self._ssl_ctx = ssl.create_default_context()
-                s = SslFilter(self._ssl_ctx, host)
+                s = SslTransformer(self._ssl_ctx, host)
                 await self._conn.bind(s)
 
-            await self._conn.bind(ReadUntilFilter())
-
-            sec_key, sec_accept = get_sec_ws_pair()
-            http_req = HttpRequest(req_url=req_url)
-            http_resp = HttpResponse()
-
-            for exhdr in self._ex_hdrs:
-                http_req.set_header(exhdr[0], exhdr[1])
-
-            http_req.set_header('Host', host, overwrite=False)
-            http_req.set_header('Connection', 'Upgrade')
-            http_req.set_header('Upgrade', 'websocket')
-            http_req.set_header('Sec-WebSocket-Version', '13')
-            http_req.set_header('Sec-WebSocket-Key', sec_key)
-
-
-            await self._conn.request(http_req, http_resp)
-            if http_resp.get_status_code() != 101:
-                print(http_resp)
-                raise Exception('TODO upgrade failed')
-
-            resp_accept = http_resp.get_header('Sec-WebSocket-Accept')
-            if len(resp_accept) != 1 or sec_accept != resp_accept[0]:
-                raise Exception('TODO upgrade failed')
+            await self._conn.bind(ReadUntilTransformer())
+            up = WebSocketUpgrader(host, req_url, upgrade_headers=self._ex_hdrs)
+            await self._conn.bind(up)
 
             proc = self._process_msg()
             self._recv_task = asyncio.ensure_future(proc)
         except:
             self._recv_task = None
             await self._conn.close()
             self._conn = None
@@ -214,21 +149,23 @@
             finally:
                 self._conn = None
                 self._recv_task = None
 
     async def send(self, type: int, data: bytes):
         mask = random.randint(0, 2**32-1)
         msg = WebSocketFrame(opcode=type, mask=mask, payload=data)
-        async with self._conn.lock:
+        async with self._lock:
+            if self.closed():
+                raise Exception('TODO')
             await self._conn.request(msg, None)
 
     async def send_text(self, text: str):
         await self.send(WebSocketOpcode.TextFrame, text.encode())
 
     async def send_binary(self, data: bytes):
         await self.send(WebSocketOpcode.BinaryFrame, data)
 
     async def send_ping(self):
         await self.send(WebSocketOpcode.Ping, bytes())
 
     async def send_pong(self):
-        await self.send(WebSocketOpcode.Pong, bytes())
+        await self.send(WebSocketOpcode.Pong, bytes())
```

## Comparing `kedixa-0.0.2.dist-info/RECORD` & `kedixa-0.0.3.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 kedixa/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kedixa/compat.py,sha256=G87n6iIZ0Xbvt87mnYLymfrZxluXYYL7lxjC99a4CTo,46
 kedixa/file_loader.py,sha256=2wfU05ozidmTn9LD7zdxljlLJbIFroBvk58RUltEQ-A,877
 kedixa/mprocess.py,sha256=wi1v4D0PdKheQtZaRfWoFyiOh19kfeO5uWb9s_dQMqk,3828
-kedixa/version.py,sha256=lr_Y4v_7NhPcZNhqqUh6iAMEbXueOQAI3IlETAprxo4,145
-kedixa/comm/__init__.py,sha256=lSDOwQWo6vJeyMh1NOV_o-qjcBoo7hkR9KvW9UK9pVw,286
+kedixa/version.py,sha256=VkGNrQe89lDmcMy5XfnXMkZEzOJNjwmwIx2-2wNgqlk,145
+kedixa/comm/__init__.py,sha256=2fdXCUd0V9jZswFs2hXfTJB2K3rEmlSDU1Ew7bQDYD8,312
 kedixa/comm/address.py,sha256=dOdqjGR2WFDsm_To2SKr-6x9a_bSgahvqXkOC8t0bIQ,1623
 kedixa/comm/basic.py,sha256=HOVBqA1o0mFVz-2eQPaRrwSp-YjD9Eo_QXQVUyV_v1A,6678
-kedixa/comm/bridge.py,sha256=yNfH1uJHT3S9vsr024PeRr6Ave3OMuP_d6Vru5w1ZUA,1525
-kedixa/comm/connection.py,sha256=FXMmiaLD2DuRwBFot0TaQ0naBNTS2jkp01yjGYJjLO8,2043
+kedixa/comm/bridge.py,sha256=p02zNymVowJOL3lU_NKXQuPfRkeBjLnyCjC1_bKHabo,1537
+kedixa/comm/connection.py,sha256=6pM_505bjsW4R4IC-o3YyXc0i9bK-pnUleYrQxYR7js,2328
 kedixa/comm/debug_filter.py,sha256=SdCROn1CACYZjlO_ZDiDgwHSg09DHb-0qlUaTUAdWYw,1082
-kedixa/comm/debug_transformer.py,sha256=Y0blu6SFfFJiYWJ_TkOV9IHhW_lqHFXc02wzrneDn5w,1107
+kedixa/comm/debug_transformer.py,sha256=KA9e0k3Wjnk6Ynr5-ajFQtzaElhSpaDqdcayEdZgzfc,1132
 kedixa/comm/exception.py,sha256=Yo-EAo4Mc_YGkeRAlMcsl7Bvj79rowgIedvE8UFuzsM,771
 kedixa/comm/file_adaptor.py,sha256=T14VRpmfaybVnP9_vbpYKM_q-XjSG3ompwE75tEMg78,1162
 kedixa/comm/read_until_filter.py,sha256=0_UHqswKfBhiFJ9A-lEUkHbmPVE8zOUBKaQmpHyXf2o,1929
 kedixa/comm/read_until_transformer.py,sha256=cUL6tqAYfnpAxgQW2vrdOm4_9HbC3SOMidgPEeVbhjE,1969
 kedixa/comm/socket_adaptor.py,sha256=OMwh8pk0OJOn9Mcsm186cwbgHAOAtLfZgZigSvStq_4,3439
 kedixa/comm/socks5_filter.py,sha256=Irf8Op5Gy64TAxXSkYShWnb_RkU-r3RcDvnDqEuHvRc,5294
 kedixa/comm/socks5_updater.py,sha256=yVV7M3aSNzY8oGtjOy4cyj8LHKGZpRlWLcQZa_6EnnE,5310
+kedixa/comm/socks5_upgrader.py,sha256=0WdJv1ze6WFAXEZrP5uENXQ3tlY9bqQ0KVpH8j92BsA,5311
 kedixa/comm/speed_limit_filter.py,sha256=3obGCuvvMiA-hPq8w3NFuLPOPHn8WfFHWWLdlEh7pRI,3487
 kedixa/comm/speed_limit_transformer.py,sha256=PXGNVh8Xs2awjw8dk7MhCLZ0b6vMjJZjItyeIfqRpzo,3507
 kedixa/comm/ssl_filter.py,sha256=clE9qwJBoDhXotQLuGjSraVPnjFkLrt7TVEcs_LTWOE,2151
-kedixa/comm/ssl_transformer.py,sha256=hHio54QpOSjgIAsFUGMhGVqUmfaJoY5z-UtoVeM9vUA,2171
-kedixa/comm/http/__init__.py,sha256=qpVySJc-aT54WSgv-8jSngjX4vKGX_TEFv8wTfhsnQE,129
+kedixa/comm/ssl_transformer.py,sha256=3-kgr34JNHyFcY8aeZzKXa9PvnLmqJRIe2C3kiA3Iek,2348
+kedixa/comm/tcp_server.py,sha256=yxieUMp93qAYHl4HUOL565l8i1lPX4kNJrt8FPHwclY,3077
+kedixa/comm/http/__init__.py,sha256=ChPXU-cEbVBK4GS5pMtHo3k-Ju5bcq8KH_0lEqdfqyA,130
 kedixa/comm/http/http_chunk_filter.py,sha256=iw_0B-7WWIO4NncHhTmGWVDs19EjC4xJOwsfwst65J0,1996
-kedixa/comm/http/http_chunk_transformer.py,sha256=P1Jq-4Hmk0fg-ajUXOkoJZOLmbw3-Rf0VTVPJwnsbXo,2046
+kedixa/comm/http/http_chunk_transformer.py,sha256=80ANjqMJa9yor303VA5djbj-2AkA-OOjV-ql89ONrPw,2066
 kedixa/comm/http/http_code_map.py,sha256=sEa5zuLjRUeoiDPL6eyTwH5GZICWgjCVwHBx-NigIkc,2011
 kedixa/comm/http/http_message.py,sha256=fexia7zJ8alaj1AR-x-5QlkCAhkNIf3EG2vBkxEZ2NU,12688
 kedixa/comm/http/http_proxy_filter.py,sha256=V39DlzOfXz-5M-_cuu9pVQZsC64vMD76su8L5q7oUWI,2356
 kedixa/comm/http/http_proxy_updater.py,sha256=ipj_OnlV9in63M3enF_FO2-jtljm2tn6wxMM_AKFbVk,2435
-kedixa/comm/websocket/__init__.py,sha256=K2iw5BRK4L7UrYJZGjujiwjIU9A06tULWEAYaif5tGk,65
-kedixa/comm/websocket/websocket_client.py,sha256=igxvsKM1mUIFC8G7opdas3ub-uIef5EpWpdAMy1kESw,6842
+kedixa/comm/http/http_proxy_upgrader.py,sha256=ZpMNLBDAcSvHOq-O8_YGObbPFTOM13f_1e4t-WxRo7s,2437
+kedixa/comm/websocket/__init__.py,sha256=ZCdKPpz9RuNMrgAAoILMI7EniexKVAYuHPfsLTI1f9s,135
+kedixa/comm/websocket/websocket_client.py,sha256=FrQtQ-vInrrqJ-B6oAtvzXr01Yqb2MZR1cIAqxLdWlA,4524
+kedixa/comm/websocket/websocket_handler.py,sha256=UmQ6MjBjz7vj3Oz5n5OmOgVeFGn2Gu5NcbiKNWehVY8,4903
 kedixa/comm/websocket/websocket_message.py,sha256=9GRqZLuHwDiNxhYF8vD8VfPjV-vsfQJ6GeDpzWZCDUM,3860
-kedixa-0.0.2.dist-info/METADATA,sha256=HnHnh-BIRLMTDSpAq3wIs_aRCEwzs04Bgl4KBfhq4CQ,227
-kedixa-0.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-kedixa-0.0.2.dist-info/top_level.txt,sha256=ONvTJADmljVaMUydvaC_uUZc5p_aUq5Z3GNuwTlhHpw,7
-kedixa-0.0.2.dist-info/RECORD,,
+kedixa/comm/websocket/websocket_processor.py,sha256=F_iM6TdCJlujFzUV3mBfhQirZL38uxKaNWAklkl_UZs,6166
+kedixa/comm/websocket/websocket_upgrader.py,sha256=SbGwmY-WV8keiW-Pk0oZtqvB3j1QCl1_Ejt-JO4llfo,2603
+kedixa-0.0.3.dist-info/METADATA,sha256=LJFEhSnAlbUgcVEQNnp4UUtQQF8nMgS_kVi1pHvOaIA,227
+kedixa-0.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+kedixa-0.0.3.dist-info/top_level.txt,sha256=ONvTJADmljVaMUydvaC_uUZc5p_aUq5Z3GNuwTlhHpw,7
+kedixa-0.0.3.dist-info/RECORD,,
```

