# Comparing `tmp/winerp-1.4.0.tar.gz` & `tmp/winerp-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winerp-1.4.0.tar", last modified: Sat May  7 03:49:44 2022, max compression
+gzip compressed data, was "winerp-1.5.0.tar", last modified: Sun Apr 16 08:15:00 2023, max compression
```

## Comparing `winerp-1.4.0.tar` & `winerp-1.5.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2022-05-07 03:49:44.725467 winerp-1.4.0/
--rw-rw-rw-   0        0        0     1091 2022-04-05 17:51:02.000000 winerp-1.4.0/LICENSE
--rw-rw-rw-   0        0        0       20 2022-04-06 14:33:55.000000 winerp-1.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4039 2022-05-07 03:49:44.725467 winerp-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     3253 2022-05-07 03:48:11.000000 winerp-1.4.0/README.md
--rw-rw-rw-   0        0        0       42 2022-05-07 03:49:44.725467 winerp-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1536 2022-05-07 03:39:44.000000 winerp-1.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-05-07 03:49:44.685493 winerp-1.4.0/winerp/
--rw-rw-rw-   0        0        0      264 2022-05-07 03:37:08.000000 winerp-1.4.0/winerp/__init__.py
--rw-rw-rw-   0        0        0      826 2022-05-07 03:37:08.000000 winerp-1.4.0/winerp/__main__.py
--rw-rw-rw-   0        0        0    24063 2022-05-07 03:39:15.000000 winerp-1.4.0/winerp/client.py
-drwxrwxrwx   0        0        0        0 2022-05-07 03:49:44.717471 winerp-1.4.0/winerp/lib/
--rw-rw-rw-   0        0        0      807 2022-05-07 03:37:08.000000 winerp-1.4.0/winerp/lib/errors.py
--rw-rw-rw-   0        0        0     3074 2022-05-07 03:37:08.000000 winerp-1.4.0/winerp/lib/message.py
--rw-rw-rw-   0        0        0     8200 2022-05-07 03:37:08.000000 winerp-1.4.0/winerp/lib/payload.py
--rw-rw-rw-   0        0        0     8313 2022-05-07 03:37:08.000000 winerp-1.4.0/winerp/server.py
-drwxrwxrwx   0        0        0        0 2022-05-07 03:49:44.717471 winerp-1.4.0/winerp.egg-info/
--rw-rw-rw-   0        0        0     4039 2022-05-07 03:49:43.000000 winerp-1.4.0/winerp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2022-05-07 03:49:44.000000 winerp-1.4.0/winerp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-07 03:49:44.000000 winerp-1.4.0/winerp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2022-05-07 03:49:44.000000 winerp-1.4.0/winerp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       35 2022-05-07 03:49:44.000000 winerp-1.4.0/winerp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-05-07 03:49:44.000000 winerp-1.4.0/winerp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 08:15:00.698513 winerp-1.5.0/
+-rw-rw-rw-   0        0        0     1070 2023-04-15 20:26:38.000000 winerp-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0       20 2023-04-15 20:26:38.000000 winerp-1.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3695 2023-04-16 08:15:00.697515 winerp-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-15 20:26:38.000000 winerp-1.5.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-16 08:15:00.698662 winerp-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     4336 2023-04-16 08:13:49.000000 winerp-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 08:15:00.609434 winerp-1.5.0/winerp/
+-rw-rw-rw-   0        0        0      290 2023-04-16 08:06:31.000000 winerp-1.5.0/winerp/__init__.py
+-rw-rw-rw-   0        0        0      826 2023-04-16 08:06:31.000000 winerp-1.5.0/winerp/__main__.py
+-rw-rw-rw-   0        0        0    23547 2023-04-16 08:06:31.000000 winerp-1.5.0/winerp/client.py
+drwxrwxrwx   0        0        0        0 2023-04-16 08:15:00.695520 winerp-1.5.0/winerp/lib/
+-rw-rw-rw-   0        0        0      807 2023-04-15 20:26:38.000000 winerp-1.5.0/winerp/lib/errors.py
+-rw-rw-rw-   0        0        0     3570 2023-04-15 20:26:38.000000 winerp-1.5.0/winerp/lib/events.py
+-rw-rw-rw-   0        0        0     3070 2023-04-15 20:26:38.000000 winerp-1.5.0/winerp/lib/message.py
+-rw-rw-rw-   0        0        0     8201 2023-04-15 20:26:38.000000 winerp-1.5.0/winerp/lib/payload.py
+-rw-rw-rw-   0        0        0     8605 2023-04-16 08:06:31.000000 winerp-1.5.0/winerp/server.py
+drwxrwxrwx   0        0        0        0 2023-04-16 08:15:00.639311 winerp-1.5.0/winerp.egg-info/
+-rw-rw-rw-   0        0        0     3695 2023-04-16 08:15:00.000000 winerp-1.5.0/winerp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2023-04-16 08:15:00.000000 winerp-1.5.0/winerp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 08:15:00.000000 winerp-1.5.0/winerp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-16 08:15:00.000000 winerp-1.5.0/winerp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       35 2023-04-16 08:15:00.000000 winerp-1.5.0/winerp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-16 08:15:00.000000 winerp-1.5.0/winerp.egg-info/top_level.txt
```

### Comparing `winerp-1.4.0/PKG-INFO` & `winerp-1.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,30 @@
 Metadata-Version: 2.1
 Name: winerp
-Version: 1.4.0
+Version: 1.5.0
 Summary: Websocket based IPC for discord.py bots
-Home-page: https://github.com/BlackThunder01001/winerp
+Home-page: https://github.com/nouman0103/winerp
 Author: BlackThunder
 Author-email: nouman0103@gmail.com
 License: MIT
-Project-URL: Bug Tracker, https://github.com/BlackThunder01001/winerp/issues
+Project-URL: Bug Tracker, https://github.com/nouman0103/winerp/issues
 Project-URL: Documentation, https://winerp.readthedocs.io/en/latest/
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: OS Independent
 Classifier: Typing :: Typed
-Requires-Python: >=3.7, !=3.10.*, !=3.11.*
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # winerp
 An IPC based on Websockets. Fast, Stable, and easy-to-use, for inter-communication between your processes or discord.py bots.
 
-> **BREAKING CHANGES (1.4.0):**  
-The message source name is passed to all registered routes.
-Instead of:
-> ```py
-> @ipc.route() # < v1.4.0
-> async def route_name():
->     ...
-> ```
-> Use: 
-> ```py
-> @ipc.route() # >= v1.4.0
-> async def route_name(source):
->     ...
-> ```
 
 ### Key Features
 
  - **Fast** with minimum recorded response time being `< 2ms`
  - Lightweight, Stable and Easy to integrate.
  - No limitation on number of connected clients. 
 
@@ -145,9 +130,7 @@
     return "You are very cool"
 
 
 bot.loop.create_task(bot.ipc.start())
 bot.run("TOKEN")
 ```
 
-
-
```

### Comparing `winerp-1.4.0/winerp/__main__.py` & `winerp-1.5.0/winerp/__main__.py`

 * *Files identical despite different names*

### Comparing `winerp-1.4.0/winerp/client.py` & `winerp-1.5.0/winerp/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,258 +1,334 @@
+"""
+Winerp- An IPC based on Websockets. Fast, Stable, and easy-to-use,
+for inter-communication between your processes or discord.py bots. 
+"""
+# pylint: disable=E0401,W0718,C0301
 import asyncio
-from types import FunctionType
-import websockets
-import orjson
 import logging
-from .lib.message import WsMessage
-from .lib.payload import Payloads, MessagePayload, winerpObject, responseObject
-from .lib.errors import *
-import uuid
 import traceback
+import typing
+import uuid
+from types import FunctionType
 from typing import (
     Any,
     Callable,
     Coroutine,
     TypeVar,
     Union,
-    Dict,
 )
 
+import orjson
+import websockets
+
+from .lib.errors import (
+    ClientNotReadyError,
+    ClientRuntimeError,
+    InvalidRouteType,
+    UnauthorizedError,
+    MissingUUIDError,
+    UUIDNotFoundError,
+)
+from .lib.events import Events
+from .lib.message import WsMessage
+from .lib.payload import Payloads, MessagePayload, winerpObject, responseObject
+
 logger = logging.getLogger(__name__)
 Coro = TypeVar('Coro', bound=Callable[..., Coroutine[Any, Any, Any]])
 
+
 class Client:
     r"""Represents a winerp Client.
     This class is used to interact with the Server
 
     Parameters
     -----------
     local_name: :class:`str`
         The name which will be used to refer to this client.
         This should be unique to all the clients.
+    host: Optional[:class:`str`]
+        The port on which the server is running. Defaults to localhost.
     port: Optional[:class:`int`]
         The port on which the server is running. Defaults to 13254.
     reconnect: Optional[:class:`bool`]
         If set to True, the client will automatically try to reconnect to the winerp server
         every 60 seconds (default). This option is set to True by default.
     """
+
     def __init__(
-        self,
-        local_name: str,
-        port: int = 13254,
-        reconnect: bool = True
+            self,
+            local_name: str,
+            host: str = "localhost",
+            port: int = 13254,
+            reconnect: bool = True
     ):
-        self.uri: str = f"ws://localhost:{port}"        
+        self.uri: str = f"ws://{host}:{port}"
         self.local_name: str = local_name
         self.reconnect: bool = reconnect
         self.reconnect_threshold: int = 60
-        self.max_data_size: float = 2 #MiB
+        self.max_data_size: float = 2  # MiB
         self.websocket = None
         self.__routes = {}
         self.__sub_routes = {}
         self.listeners = {}
-        self.event_listeners: Dict[str, asyncio.Future] = {}
+
         self._authorized: bool = False
         self._on_hold = False
-        self.events = [
-            "on_winerp_connect",
-            "on_winerp_ready",
-            "on_winerp_disconnect",
-            "on_winerp_request",
-            "on_winerp_response",
-            "on_winerp_information",
-            "on_winerp_error"
-        ]
-    
+        self.__events = Events(logger)
+        self.event = self.__events.event
+
     @property
     def authorized(self) -> bool:
-        '''
+        """
         :class:`bool`: Returns if the client is authorized by the server.
-        '''
+        """
         return self._authorized
-    
+
     @property
     def on_hold(self) -> bool:
-        '''
-        :class:`bool`: Returns True if the client is on hold by the server. A client is put on hold if a client of same local name is already connected to the server.
-        '''
+        """
+        :class:`bool`: Returns True if the client is on hold by the server.
+        A client is put on hold if a client of same local name is already connected to the server.
+        """
         return self._on_hold
 
     async def send_message(self, data: Union[Any, WsMessage]):
+        """Send a message to the server."""
         if not isinstance(data, WsMessage):
             data = data.__dict__
         logger.debug(data)
         await self.websocket.send(orjson.dumps(data).decode("utf-8"))
-    
+
     def __send_message(self, data):
         asyncio.create_task(self.send_message(data))
-    
+
     async def __verify_client(self):
         payload = MessagePayload(
-            type = Payloads.verification,
-            id = self.local_name,
-            uuid = str(uuid.uuid4())
+            type=Payloads.verification,
+            id=self.local_name,
+            uuid=str(uuid.uuid4())
         )
         await self.send_message(payload)
         logger.info("Verification request sent")
 
     async def __connect(self) -> None:
         if self.websocket is None or self.websocket.closed:
             logger.info("Connecting to Websocket")
             self.websocket = await websockets.connect(
-                self.uri, close_timeout=0, ping_interval=None, max_size=int(self.max_data_size*1048576)
+                self.uri,
+                close_timeout=0,
+                ping_interval=None,
+                max_size=int(self.max_data_size * 1048576)
             )
             self._authorized = False
-            self._dispatch_event('winerp_connect')
+            self.__events.dispatch_event('winerp_connect')
             logger.info("Connected to Websocket")
 
     async def __reconnect_client(self) -> bool:
         while True:
             try:
                 await self.__connect()
                 await self.__verify_client()
                 return True
-            except:
-                logger.debug(f"Failed to reconnect. Retrying in {self.reconnect_threshold}s")
+            except Exception as error:
+                logger.debug("Failed to reconnect. Retrying in %ss.", self.reconnect_threshold)
+                logger.error("While trying to reconnect there has been an error. %s", str(error))
                 await asyncio.sleep(self.reconnect_threshold)
-        
+
     async def start(self) -> None:
-        '''|coro|
+        """|coro|
 
         Connects the client to the server.
 
         Raises
         -------
             ConnectionError
                 If the websocket is already connected.
         
         Returns
         -------
             :class:`None`
-        '''
+        """
         if self.websocket is None or self.websocket.closed:
             await self.__connect()
             await self.__verify_client()
             asyncio.create_task(self.__on_message())
         else:
             raise ConnectionError("Websocket is already connected!")
 
     def route(self, name: str = None):
-        '''
+        """
         A decorator to register your route. The route name should be unique.
 
         Raises
         -------
             ValueError
                 Route name already exists.
             InvalidRouteType
                 The function passed is not a coro.
-        '''
-        def route_decorator(func):
-            if (name is None and func.__name__ in self.__routes) or (name is not None and name in self.__routes):
+        """
+
+        def route_decorator(_route_func):
+            if (name is None and _route_func.__name__ in self.__routes) or (name is not None and name in self.__routes):
                 raise ValueError("Route name is already registered!")
-            
-            if not asyncio.iscoroutinefunction(func):
+
+            if not asyncio.iscoroutinefunction(_route_func):
                 raise InvalidRouteType("Route function must be a coro.")
-            
-            self.__routes[name or func.__name__] = func
-            return func
-            
+
+            self.__routes[name or _route_func.__name__] = _route_func
+            return _route_func
+
         if isinstance(name, FunctionType):
-            func = name
+            _route_func = name
             name = name.__name__
-            return route_decorator(func)
+            return route_decorator(_route_func)
         else:
             return route_decorator
 
-    async def __purge_sub_routes(self, timeout, uuid):
+    async def add_route(self, callback: typing.Callable, name: str = None):
+        """|coro|
+        A function to register a route. Either a decorator or this function can be used
+        to register a route.
+
+        Parameters
+        ----------
+        callback
+        name
+
+        Returns
+        -------
+        typing.Callable
+
+        Raises
+        -------
+            KeyError
+                Route name already exists.
+            InvalidRouteType
+                The function passed is not a coro.
+
+        """
+        if (name in self.__routes) or (callback.__name__ in self.__routes):
+            raise KeyError(f"Route name is already registered!\nRoutes: {self.__routes}")
+        if not asyncio.iscoroutinefunction(callback):
+            raise InvalidRouteType('Route callback must be an asyncio coro.')
+
+        self.__routes[name or callback.__name__] = callback
+        return callback
+
+    def remove_route(self, name: str):
+        """
+        Removes a route from the registered routes.
+        
+        Parameters
+        ----------
+        name
+            The name of the route to be removed.
+
+        Returns
+        -------
+        None
+
+        Raises
+        -------
+            KeyError
+                Route name does not exist.
+        """
+        if name in self.__routes:
+            del self.__routes[name]
+        else:
+            raise KeyError(f"Route name {name} does not exist!")
+
+    async def __purge_sub_routes(self, timeout, _uuid):
         await asyncio.sleep(timeout)
-        del self.__sub_routes[uuid]
+        del self.__sub_routes[_uuid]
+
     def __register_object_funcs(self, winerp_object: winerpObject):
         self.__sub_routes[winerp_object.uuid] = {}
         for function_name, function_object in winerp_object.functions.items():
             self.__sub_routes[winerp_object.uuid][function_name] = function_object
-        asyncio.create_task(self.__purge_sub_routes(winerp_object.object_expiry, winerp_object.uuid))
+        asyncio.create_task(self.__purge_sub_routes(
+            winerp_object.object_expiry, winerp_object.uuid
+        ))
 
-    async def ping(self, client = None, timeout: int = 60) -> bool:
-        '''|coro|
+    async def ping(self, client=None, timeout: int = 60) -> bool:
+        """|coro|
 
         Pings the client and returns back if the ping was successful.
 
         Raises
         -------
             ClientNotReadyError
                 The client is currently not ready to send or accept requests.
             UnauthorizedError
                 The client isn't authorized by the server.
         
         Returns
         --------
             :class:`bool`
                 If the ping is successful, it returns True.
-        '''
+        """
         if self._on_hold or self.websocket is None or not self.websocket.open:
             raise ClientNotReadyError("The client is currently not ready to send or accept requests.")
         if not self._authorized:
             raise UnauthorizedError("Client is not authorized!")
         logger.debug("Pinging IPC Server")
-        
+
         _uuid = str(uuid.uuid4())
         payload = MessagePayload(
-            type = Payloads.ping,
-            id = self.local_name,
-            destination = client,
-            uuid = _uuid
+            type=Payloads.ping,
+            id=self.local_name,
+            destination=client,
+            uuid=_uuid
         )
         await self.send_message(payload)
         resp = await self.__get_response(_uuid, asyncio.get_event_loop(), timeout=timeout)
         return resp.get("success", False)
 
-    async def call_function(self, destination, object_identifier, func_name, *args, **kwargs) -> bool:
+    async def _call_function(self, destination, object_identifier, func_name, *args, **kwargs) -> bool:
         if self._on_hold or self.websocket is None or not self.websocket.open:
             raise ClientNotReadyError("The client is currently not ready to send or accept requests.")
         if not self._authorized:
             raise UnauthorizedError("Client is not authorized!")
         logger.debug("Calling a function IPC Server")
-        
+
         _uuid = str(uuid.uuid4())
         payload = MessagePayload(
-            type = Payloads.function_call,
-            id = self.local_name,
-            destination = destination,
-            uuid = _uuid,
+            type=Payloads.function_call,
+            id=self.local_name,
+            destination=destination,
+            uuid=_uuid,
             data={
                 "__uuid__": object_identifier,
                 "__func__": func_name,
                 "__args__": list(args),
                 "__kwargs__": dict(kwargs)
             }
         )
         await self.send_message(payload)
         recv = await self.__get_response(_uuid, asyncio.get_event_loop(), timeout=30)
         return recv
 
     def __get_response(
-        self,
-        _uuid: str,
-        loop: asyncio.AbstractEventLoop,
-        timeout: int = 60
+            self,
+            _uuid: str,
+            loop: asyncio.AbstractEventLoop,
+            timeout: int = 60
     ):
         future = loop.create_future()
         self.listeners[_uuid] = future
-        return asyncio.wait_for(future, timeout, loop=loop)
+        return asyncio.wait_for(future, timeout)
 
     async def request(
-        self,
-        route: str,
-        source: str,
-        timeout: int = 60,
-        **kwargs
-    ) -> any:
-        '''|coro|
+            self,
+            route: str,
+            source: str,
+            timeout: int = 60,
+            **kwargs
+    ) -> Any:
+        """|coro|
 
         Requests the server for a response.
         Resolves when the response is received matching the UUID.
 
         Parameters
         -----------
         route: :class:`str`
@@ -273,122 +349,121 @@
             RuntimeError
                 If the UUID is not found.
             asyncio.TimeoutError
                 If the response is not received within the timeout.
         
         Returns
         --------
-            :class:`any`
+            :class:`Any`
                 The data associated with the message.
-        '''
+        """
         if self.websocket is not None and self.websocket.open:
             if self._on_hold:
                 raise ClientNotReadyError("The client is currently not ready to send or accept requests.")
             if not self._authorized:
                 raise UnauthorizedError("Client is not authorized!")
-            
+
             if not route or not source:
                 raise ValueError("Missing required information for this request")
 
             logger.info("Requesting IPC Server for %r", route)
-        
+
             _uuid = str(uuid.uuid4())
             payload = MessagePayload(
-                type = Payloads.request,
-                id = self.local_name,
-                destination = source,
-                route = route,
-                data = kwargs,
-                uuid = _uuid
+                type=Payloads.request,
+                id=self.local_name,
+                destination=source,
+                route=route,
+                data=kwargs,
+                uuid=_uuid
             )
 
             await self.send_message(payload)
             recv = await self.__get_response(_uuid, asyncio.get_event_loop(), timeout=timeout)
             return recv
-        
+
         else:
             raise ClientNotReadyError("The client has not been started or has disconnected")
 
     async def inform(
-        self,
-        data: any,
-        destinations: list
+            self,
+            data: Any,
+            destinations: list
     ):
-        '''|coro|
+        """|coro|
 
-        Sends data to other connected clients. There is no tracking of the data so there won't be any error
-        if it doesn't reach its specified destination.
+        Sends data to other connected clients. There is no tracking of the data so there 
+        won't be any error if it doesn't reach its specified destination.
 
         The data is sent to all connected clients if the destinations list is empty.
 
         Parameters
         -----------
         data: :class:`Any`
             The data to redirect.
-        destination: :class:`list`
+        destinations: :class:`list`
             The list of destinations.
 
         Raises
         -------
             ClientNotReadyError
                 The client is currently not ready to send or accept requests.
             UnauthorizedError
                 The client isn't authorized by the server.
         
         Returns
         --------
             :class:`None`
-        '''
+        """
         if self.websocket is not None and self.websocket.open:
             if self._on_hold:
                 raise ClientNotReadyError("The client is currently not ready to send or accept requests.")
             if not self._authorized:
                 raise UnauthorizedError("Client is not authorized!")
 
-            logger.info("Informing IPC Server to redirect to routes %s" % destinations)
+            logger.info("Informing IPC Server to redirect to routes %s", destinations)
             if not isinstance(destinations, list):
                 destinations = [destinations]
 
             payload = MessagePayload(
-                type = Payloads.information,
-                id = self.local_name,
-                route = destinations,
-                data = data,
+                type=Payloads.information,
+                id=self.local_name,
+                route=destinations,
+                data=data,
             )
 
             await self.send_message(payload)
         else:
             raise ClientNotReadyError("The client has not been started or has disconnected")
-    
 
     async def wait_until_ready(self):
-        '''|coro|
+        """|coro|
 
         Waits until the client is ready to send or accept requests.        
-        '''
+        """
         await self.wait_for('winerp_ready', None)
 
     async def wait_until_disconnected(self):
-        '''|coro|
+        """|coro|
         
         Waits until the client is disconnected.
-        '''
+        """
         await self.wait_for('winerp_disconnect', None)
 
     def wait_for(
-        self,
-        event: str,
-        timeout: int = 60,
+            self,
+            event: str,
+            timeout: Union[int, None] = None,
     ):
-        '''|coro|
+        """|coro|
 
         Waits for a WebSocket event to be dispatched.
 
         The timeout parameter is passed onto asyncio.wait_for().
-        By default, it does not timeout.
+        By default, it does not have timeout.
 
         In case the event returns multiple arguments, a tuple containing those arguments is returned instead.
         Please check the documentation for a list of events and their parameters.
 
         This function returns the **first event that meets the requirements.**
 
         Parameters
@@ -403,179 +478,176 @@
             asyncio.TimeoutError
                 If the event is not received within the timeout.
         
         Returns
         --------
             :class:`Any`
                 The payload for the event that meets the requirements.
-        '''
+        """
         future = asyncio.get_event_loop().create_future()
 
-        ev = event.lower()
+        _event = event.lower()
         try:
-            listeners = self.event_listeners[ev]
+            listeners = self.__events.listeners[_event]
         except KeyError:
             listeners = []
-            self.event_listeners[ev] = listeners
+            self.__events.listeners[_event] = listeners
 
         listeners.append(future)
         return asyncio.wait_for(future, timeout)
 
-
     async def __on_message(self):
         logger.info("Listening to messages")
+        message = None
         while True:
             try:
                 message = WsMessage(orjson.loads(await self.websocket.recv()))
             except websockets.exceptions.ConnectionClosedError:
-                self._dispatch_event('winerp_disconnect')
+                self.__events.dispatch_event('winerp_disconnect')
                 if self.reconnect:
                     if not await self.__reconnect_client():
                         break
                 else:
                     break
 
             if message.type.success and not self._authorized:
                 logger.info("Authorized Successfully")
-                self._dispatch_event('winerp_ready')
+                self.__events.dispatch_event('winerp_ready')
                 self._authorized = True
                 self._on_hold = False
 
             elif message.type.ping:
                 logger.debug("Received a ping from server")
                 asyncio.create_task(self._dispatch(message))
 
             elif message.type.request:
                 if message.route not in self.__routes:
                     logger.info("Failed to fulfill request, route not found")
                     payload = MessagePayload(
-                        type = Payloads.error,
-                        id = self.local_name,
-                        data = "Route not found",
-                        traceback = "Route not found",
-                        destination = message.id,
-                        uuid = message.uuid
+                        type=Payloads.error,
+                        id=self.local_name,
+                        data="Route not found",
+                        traceback="Route not found",
+                        destination=message.id,
+                        uuid=message.uuid
                     )
                     self.__send_message(payload)
                     return
-                logger.info("Fulfilling request @ route: %s" % message.route)
+                logger.info("Fulfilling request @ route: %s", message.route)
                 asyncio.create_task(self._fulfill_request(message))
-                self._dispatch_event('winerp_request')
-            
+                self.__events.dispatch_event('winerp_request')
+
             elif message.type.response:
-                logger.info("Received a response from server @ uuid: %s" % message.uuid)
+                logger.info("Received a response from server @ uuid: %s", message.uuid)
                 asyncio.create_task(self._dispatch(message))
-                self._dispatch_event('winerp_response')
+                self.__events.dispatch_event('winerp_response')
 
             elif message.type.error:
                 if message.data == "Already authorized.":
                     self._on_hold = True
-                    logger.warn("Another client is already connected. Requests will be enabled when the other is disconnected.")
+                    logger.warning(
+                        "Another client is already connected. Requests will be enabled when the other is disconnected.")
                 else:
-                    logger.debug("Failed to fulfill request: %s" % message.data)
-                    self._dispatch_event('winerp_error', message.data)
+                    logger.debug("Failed to fulfill request: %s", message.data)
+                    self.__events.dispatch_event('winerp_error', message.data)
 
                 if message.uuid is not None:
                     asyncio.create_task(self._dispatch(message))
 
             elif message.type.information:
                 if message.data:
-                    logger.debug("Received an information bit from client: %s" % message.id)
-                    self._dispatch_event('winerp_information', message.data, message.id)
+                    logger.debug("Received an information bit from client: %s", message.id)
+                    self.__events.dispatch_event('winerp_information', message.data, message.id)
 
             elif message.type.function_call:
                 logger.debug("Received an object function call.")
                 logger.debug(message.data)
                 payload = MessagePayload(
-                    type = Payloads.response,
-                    id = self.local_name,
-                    destination = message.id,
-                    uuid = message.uuid
+                    type=Payloads.response,
+                    id=self.local_name,
+                    destination=message.id,
+                    uuid=message.uuid
                 )
                 try:
                     called_function = self.__sub_routes[message.data["__uuid__"]][message.data["__func__"]]
                     asyncio.create_task(
-                    self._fulfil_callback(
-                        payload,
-                        called_function,
-                        *message.data["__args__"],
-                        **message.data["__kwargs__"]
+                        self._fulfil_callback(
+                            payload,
+                            called_function,
+                            *message.data["__args__"],
+                            **message.data["__kwargs__"]
+                        )
                     )
-                )
                 except KeyError:
                     payload = MessagePayload(
-                        type = Payloads.error,
-                        id = self.local_name,
-                        data = "The called function has either expired or has never been registered",
-                        traceback = "The called function has either expired or has never been registered",
-                        destination = message.id,
-                        uuid = message.uuid
+                        type=Payloads.error,
+                        id=self.local_name,
+                        data="The called function has either expired or has never been registered",
+                        traceback="The called function has either expired or has never been registered",
+                        destination=message.id,
+                        uuid=message.uuid
                     )
                     self.__send_message(payload)
 
-                
-
     def __parse_object(self, payload):
         payload.pseudo_object = True
         dummy_object = payload.data
         payload.data = dummy_object.serialize()
         self.__register_object_funcs(dummy_object)
 
     async def _fulfil_callback(self, payload, function, *args, **kwargs):
         try:
             payload.data = await function(*args, **kwargs)
             if not isinstance(payload.data, (int, float, str, bool, type(None), list, tuple, dict)):
                 payload.data = winerpObject(payload.data)
 
-            if type(payload.data) == winerpObject:
+            if isinstance(payload.data, winerpObject):
                 self.__parse_object(payload)
-            
+
             self.__send_message(payload)
         except Exception as error:
             logger.exception("Failed to run the registered method")
-            self._dispatch_event('winerp_error', error)
+            self.__events.dispatch_event('winerp_error', error)
             payload.type = Payloads.error
             payload.data = str(error)
             payload.traceback = ''.join(
                 traceback.format_exception(
                     TypeError, error, error.__traceback__
                 )
             )
-        
-    
+
     async def _fulfill_request(self, message: WsMessage):
         route = message.route
         func = self.__routes[route]
         data = message.data
         payload = MessagePayload().from_message(message)
         payload.type = Payloads.response
         payload.id = self.local_name
 
-
         try:
-            payload.data = await func(message.id, **data)
-            if type(payload.data) == winerpObject:
+            payload.data = await func(message.destination, **data)
+            if isinstance(payload.data, winerpObject):
                 self.__parse_object(payload)
         except Exception as error:
             logger.exception(error)
-            self._dispatch_event('winerp_error', error)
+            self.__events.dispatch_event('winerp_error', error)
             etype = type(error)
             trace = error.__traceback__
             lines = traceback.format_exception(etype, error, trace)
             traceback_text = ''.join(lines)
 
             payload.type = Payloads.error
             payload.data = str(error)
             payload.traceback = traceback_text
         finally:
             try:
                 await self.send_message(payload)
             except TypeError as error:
                 logger.exception("Failed to convert data to json")
-                self._dispatch_event('winerp_error', error)
+                self.__events.dispatch_event('winerp_error', error)
                 payload.type = Payloads.error
                 payload.data = str(error)
                 payload.traceback = ''.join(
                     traceback.format_exception(
                         TypeError,
                         error,
                         error.__traceback__
@@ -586,90 +658,18 @@
     async def _dispatch(self, msg: WsMessage):
         data = msg.data
         _uuid = msg.uuid
         if _uuid is None:
             raise MissingUUIDError('UUID is missing.')
         if _uuid not in self.listeners:
             raise UUIDNotFoundError(f"UUID {_uuid} not found in listeners.")
-        
+
         future: asyncio.Future = self.listeners[_uuid]
         if not msg.type.error:
             if msg.pseudo_object:
                 future.set_result(responseObject(self, msg.id, data))
             else:
                 future.set_result(data)
         else:
             future.set_exception(
                 ClientRuntimeError(msg.data)
             )
-
-    def event(self, func: Coro, /) -> Coro:
-        '''
-        Registers a function for the event.
-
-        The available events are:
-            | ``on_winerp_connect``: The client has successfully connected to the server.
-            | ``on_winerp_ready``: The client is ready to recieve and send requests.
-            | ``on_winerp_disconnect``: The client has disconnected from the server.
-            | ``on_winerp_request``: The server sent new request.
-            | ``on_winerp_response``: The server sent back a response to a previous request.
-            | ``on_winerp_information``: The server sent some data sourced by a client.
-            | ``on_winerp_error``: An error occured during request processing.
-        
-        Raises
-        -------
-            NameError
-                Invalid winerp event name.
-            TypeError
-                The event function is not a coro.
-        '''
-        if func.__name__ not in self.events:
-            raise NameError("Invalid winerp event")
-        
-        if not asyncio.iscoroutinefunction(func):
-            raise TypeError("Event function must be a coro.")
-
-        setattr(self, func.__name__, func)
-        logger.debug(('%s has successfully been registered as an event', func.__name__))
-        return func
-
-    def _dispatch_event(self, event_name: str, *args, **kwargs):
-        logger.debug('Event Dispatch -> %r', event_name)
-        try:
-            for future in self.event_listeners[event_name]:
-                future.set_result(None)
-                logger.debug('Event %r has been dispatched', event_name)
-        except KeyError:
-            ...
-
-        try:
-            coro = getattr(self, f'on_{event_name}')
-        except AttributeError:
-            pass
-        else:
-            self._schedule_event(coro, f'on_{event_name}', *args, **kwargs)
-
-    
-    def _schedule_event(
-        self,
-        coro: Callable[..., Coroutine[Any, Any, Any]],
-        event_name: str,
-        *args: Any,
-        **kwargs: Any,
-    ) -> asyncio.Task:
-        wrapped = self._run_event(coro, event_name, *args, **kwargs)
-        # Schedules the task
-        return asyncio.create_task(wrapped, name=f'winerp: {event_name}')
-    
-
-    async def _run_event(
-        self,
-        coro: Callable[..., Coroutine[Any, Any, Any]],
-        event_name: str,
-        *args: Any,
-        **kwargs: Any,
-    ) -> None:
-        try:
-            await coro(*args, **kwargs)
-        except Exception:
-            # TODO
-            traceback.print_exc()
```

### Comparing `winerp-1.4.0/winerp/lib/message.py` & `winerp-1.5.0/winerp/lib/message.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,101 +11,101 @@
         return f'<winerp.WsMessage uuid={self.uuid} type={self.type.__repr__()}>'
     
     def __dict__(self) -> dict:
         return self.to_dict()
     
     @property
     def type(self) -> PayloadTypes:
-        '''
+        """
         :class:`~winerp.lib.payload.PayloadTypes`: Returns the type of the message.
-        '''
+        """
         return PayloadTypes(self._message["type"])
     
     @property
     def id(self) -> int:
-        '''
+        """
         :class:`int`: Returns the id of the bot.
-        '''
+        """
         return self._message.get("id")
     
     @property
     def destination(self) -> str:
-        '''
+        """
         :class:`str`: Returns the destination of the message.
-        '''
+        """
         return self._message.get("destination")
     
     @property
     def route(self) -> str:
-        '''
+        """
         :class:`str`: Returns the route of the message.
-        '''
+        """
         return self._message.get("route")
     
     @property
     def uuid(self) -> str:
-        '''
+        """
         :class:`str`: Returns the unique id associated with this message.
-        '''
+        """
         return self._message.get("uuid")
     
     @property
     def data(self) -> any:
-        '''
+        """
         :class:`Any`: Returns the data associated with the message.
-        '''
+        """
         return self._message.get("data")
     
     @property
     def error(self) -> str:
-        '''
+        """
         :class:`str`: Returns the error associated with the message.
-        '''
+        """
         return self._message.get("error")
     
     @error.setter
     def error(self, error: str):
-        '''
+        """
         Sets the error associated with the message.
-        '''
+        """
         self._message["error"] = error
     
     @property
     def traceback(self) -> str:
-        '''
+        """
         :class:`str`: Returns the error associated with the message.
-        '''
+        """
         return self._message.get("traceback")
     
     @traceback.setter
     def traceback(self, traceback: str):
-        '''
+        """
         Sets the error associated with the message.
-        '''
+        """
         self._message["traceback"] = traceback
 
     @property
     def pseudo_object(self) -> bool:
-        '''
+        """
         :class:`str`: Returns the error associated with the message.
-        '''
+        """
         return self._message.get("pseudo_object")
-    
+
 
     @pseudo_object.setter
     def pseudo_object(self, pseudo_object: bool):
-        '''
+        """
         Sets the error associated with the message.
-        '''
+        """
         self._message["pseudo_object"] = pseudo_object
 
     def to_dict(self) -> dict:
-        '''
+        """
         :class:`dict`: Returns the message as a `dict` type.
-        '''
+        """
         return {
             'type': self.type,
             'id': self.id,
             'destination': self.destination,
             'route': self.route,
             'uuid': self.uuid,
             'data': self.data,
```

### Comparing `winerp-1.4.0/winerp/lib/payload.py` & `winerp-1.5.0/winerp/lib/payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
                 return await self.__function_call(each_function, is_it_coro, *args, **kwargs)
 
             self.__setattr__(each_function, __async_fakeFunc)
 
     
 
     async def __function_call(self, function_name, is_it_coro, *args, **kwargs):
-        return await self.__ipc.call_function(self.__source, self.__uuid__, function_name, *args, **kwargs)
+        return await self.__ipc._call_function(self.__source, self.__uuid__, function_name, *args, **kwargs)
 
 
 
 class winerpObject:
     def __init__(self, object, required_functions = [], object_expiry=30, process_iters = True):
         """Creates a fake object which can be transferred to another client
         Whenever a fake object is sent to another client, the required functions are registered in the memory until the object expiry timeout.
```

### Comparing `winerp-1.4.0/winerp/server.py` & `winerp-1.5.0/winerp/server.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,62 @@
+def noop(*args, **kwargs):
+    pass
+    
+import logging
+original_basicConfig = logging.basicConfig
+logging.basicConfig = noop
+
 from websocket_server import WebsocketServer
+logging.basicConfig = original_basicConfig
+
+import orjson
 from .lib.message import WsMessage
 from .lib.payload import Payloads, MessagePayload
-from .lib.errors import *
-import orjson
 
-import logging
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
+handler = logging.StreamHandler()
+handler.setLevel(logging.INFO)
+logger.addHandler(handler)
+
 class Server:
     """
     Represents a winerp Server.
     This class is used as the central communication center for all connected clients.
     All requests and responses pass through the server
 
     If the library is installed using PyPi, you can also use terminal to start server using `winerp --port 1234`
     
     Parameters
     -----------
+    host: Optional[:class:`str`]
+        The host on which the server is running. Defaults to 127.0.0.1.
     port: Optional[:class:`int`]
         The port on which the server is running. Defaults to 13254.
     """
+
     def __init__(
-        self,
-        port: int = 13254
+            self,
+            host: str = "127.0.0.1",
+            port: int = 13254
     ):
-        self.websocket = WebsocketServer(host='127.0.0.1', port=port)
+        self.websocket = WebsocketServer(host=host, port=port)
         self.websocket.set_fn_new_client(self.__on_client_connect)
         self.websocket.set_fn_message_received(self.__on_message)
         self.websocket.set_fn_client_left(self.__on_client_disconnect)
         self.active_clients = {}
         self.pending_verification = {}
         self.on_hold_connections = {}
-    
+
     @property
     def client_count(self) -> int:
-        '''
+        """
         :class:`int`: Returns the number of connected clients
-        '''
+        """
         return len(self.active_clients)
 
     def __on_client_connect(self, client, _):
         logger.info("Client connected with id %s" % client['address'][1])
         self.pending_verification[client["address"][1]] = client
 
     def __on_client_disconnect(self, client, _):
@@ -55,25 +70,23 @@
                     self.__send_message(
                         self.on_hold_connections[cid]["client"],
                         MessagePayload(type=Payloads.success, data="Authorized.")
                     )
                     del self.pending_verification[self.on_hold_connections[cid]["id"]]
                     del self.on_hold_connections[cid]
                 return
-        
+
         for cid, each_client in self.on_hold_connections.items():
             if each_client["id"] == client["address"][1]:
                 del self.on_hold_connections[cid]
                 return
 
         if client["address"][1] in self.pending_verification:
             del self.pending_verification[client["address"][1]]
 
-        
-    
     def __send_message(self, client, message):
         if not isinstance(message, dict):
             message = message.to_dict()
         self.websocket.send_message(
             client,
             orjson.dumps(message)
         )
@@ -111,15 +124,15 @@
             if client["address"][1] in self.pending_verification:
                 logger.info('Unverified client tried to send message')
                 payload.type = Payloads.error
                 payload.data = "Not authorized."
                 payload.traceback = "Not authorized."
                 self.__send_error(client, payload)
                 return
-        
+
         if msg.type.information:
             logger.debug("Received Information Message from client %s" % client['address'][1])
             payload.type = Payloads.information
             if msg.route:
                 for destination in msg.route:
                     if destination in self.active_clients:
                         payload.destination = destination
@@ -133,15 +146,15 @@
         if msg.type.ping:
             logger.debug("Received Ping Message from client %s" % client['address'][1])
             payload.type = Payloads.ping
             if (msg.destination is not None and msg.destination in self.active_clients) or msg.destination is None:
                 payload.data = {"success": True}
             else:
                 payload.data = {"success": False}
-                
+
             self.__send_message(
                 client,
                 payload
             )
 
         if msg.type.request:
             logger.debug("Received Request Message from client %s" % client['address'][1])
@@ -179,15 +192,14 @@
                 Payloads.function_call if msg.type.function_call else Payloads.error)
 
             self.__send_message(
                 self.active_clients[msg.destination]["client"],
                 payload
             )
             logger.debug("Response forwarded to %s" % self.active_clients[msg.destination]["client"]['address'][1])
-            
-            
+
     def start(self):
-        '''
+        """
         Starts the server on the given port.
-        '''
+        """
         logger.info("Started Websocket Server")
         self.websocket.run_forever()
```

### Comparing `winerp-1.4.0/winerp.egg-info/PKG-INFO` & `winerp-1.5.0/winerp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,30 @@
 Metadata-Version: 2.1
 Name: winerp
-Version: 1.4.0
+Version: 1.5.0
 Summary: Websocket based IPC for discord.py bots
-Home-page: https://github.com/BlackThunder01001/winerp
+Home-page: https://github.com/nouman0103/winerp
 Author: BlackThunder
 Author-email: nouman0103@gmail.com
 License: MIT
-Project-URL: Bug Tracker, https://github.com/BlackThunder01001/winerp/issues
+Project-URL: Bug Tracker, https://github.com/nouman0103/winerp/issues
 Project-URL: Documentation, https://winerp.readthedocs.io/en/latest/
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: OS Independent
 Classifier: Typing :: Typed
-Requires-Python: >=3.7, !=3.10.*, !=3.11.*
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # winerp
 An IPC based on Websockets. Fast, Stable, and easy-to-use, for inter-communication between your processes or discord.py bots.
 
-> **BREAKING CHANGES (1.4.0):**  
-The message source name is passed to all registered routes.
-Instead of:
-> ```py
-> @ipc.route() # < v1.4.0
-> async def route_name():
->     ...
-> ```
-> Use: 
-> ```py
-> @ipc.route() # >= v1.4.0
-> async def route_name(source):
->     ...
-> ```
 
 ### Key Features
 
  - **Fast** with minimum recorded response time being `< 2ms`
  - Lightweight, Stable and Easy to integrate.
  - No limitation on number of connected clients. 
 
@@ -145,9 +130,7 @@
     return "You are very cool"
 
 
 bot.loop.create_task(bot.ipc.start())
 bot.run("TOKEN")
 ```
 
-
-
```

