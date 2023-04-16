# Comparing `tmp/aiosignald-0.3.6.tar.gz` & `tmp/aiosignald-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosignald-0.3.6.tar", max compression
+gzip compressed data, was "aiosignald-0.3.7.tar", max compression
```

## Comparing `aiosignald-0.3.6.tar` & `aiosignald-0.3.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    34523 2023-01-19 17:11:03.019209 aiosignald-0.3.6/LICENSE
--rw-r--r--   0        0        0     2642 2023-01-19 17:11:03.019209 aiosignald-0.3.6/README.md
--rw-r--r--   0        0        0      159 2023-01-19 17:11:03.019209 aiosignald-0.3.6/aiosignald/__init__.py
--rw-r--r--   0        0        0      410 2023-01-19 17:11:03.019209 aiosignald-0.3.6/aiosignald/error.py
--rw-r--r--   0        0        0     6032 2023-01-19 17:11:03.019209 aiosignald-0.3.6/aiosignald/exc.py
--rw-r--r--   0        0        0    72429 2023-01-19 17:11:03.019209 aiosignald-0.3.6/aiosignald/generated.py
--rw-r--r--   0        0        0     9988 2023-01-19 17:11:03.022543 aiosignald-0.3.6/aiosignald/util.py
--rw-r--r--   0        0        0      572 2023-01-19 17:12:17.429242 aiosignald-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     3279 1970-01-01 00:00:00.000000 aiosignald-0.3.6/setup.py
--rw-r--r--   0        0        0     3277 1970-01-01 00:00:00.000000 aiosignald-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-16 08:06:26.974300 aiosignald-0.3.7/LICENSE
+-rw-r--r--   0        0        0     2642 2023-04-16 08:06:26.974300 aiosignald-0.3.7/README.md
+-rw-r--r--   0        0        0      159 2023-04-16 08:06:26.974300 aiosignald-0.3.7/aiosignald/__init__.py
+-rw-r--r--   0        0        0      410 2023-04-16 08:06:26.974300 aiosignald-0.3.7/aiosignald/error.py
+-rw-r--r--   0        0        0     6043 2023-04-16 08:06:26.974300 aiosignald-0.3.7/aiosignald/exc.py
+-rw-r--r--   0        0        0    72953 2023-04-16 08:06:26.977634 aiosignald-0.3.7/aiosignald/generated.py
+-rw-r--r--   0        0        0        0 2023-04-16 08:06:26.977634 aiosignald-0.3.7/aiosignald/py.typed
+-rw-r--r--   0        0        0    10668 2023-04-16 08:06:26.977634 aiosignald-0.3.7/aiosignald/util.py
+-rw-r--r--   0        0        0      641 2023-04-16 08:07:12.681484 aiosignald-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     3277 1970-01-01 00:00:00.000000 aiosignald-0.3.7/PKG-INFO
```

### Comparing `aiosignald-0.3.6/LICENSE` & `aiosignald-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aiosignald-0.3.6/README.md` & `aiosignald-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `aiosignald-0.3.6/aiosignald/exc.py` & `aiosignald-0.3.7/aiosignald/exc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
 Generated using https://signald.org/protocol.json
-Version: '0.23.1'=
+Version: '0.23.2-7-1583b4df'=
 """
 
 from .error import SignaldException
 from .generated import *
 
 
 class IllegalArgumentException(SignaldException):
     message: str
 
 
-class DuplicateMessageError(SignaldException):
-    timestamp: int
-    message: str
-
-
 class UntrustedIdentityError(SignaldException):
     identifier: str
     message: str
     identity_key: "IdentityKeyv1"
 
 
-class NetworkError(SignaldException):
-    message: str
-
-
 class ProtocolInvalidKeyIdError(SignaldException):
     sender: str
     timestamp: int
     message: str
     sender_device: int
     content_hint: int
     group_id: str
 
 
+class DuplicateMessageError(SignaldException):
+    timestamp: int
+    message: str
+
+
+class NetworkError(SignaldException):
+    message: str
+
+
 class ProtocolInvalidMessageError(SignaldException):
     sender: str
     timestamp: int
     message: str
     sender_device: int
     content_hint: int
     group_id: str
@@ -235,18 +235,18 @@
 
 class GroupLinkNotActiveError(SignaldException):
     message: str
 
 
 __all__ = [
     "SignaldException",
-    "DuplicateMessageError",
     "UntrustedIdentityError",
-    "NetworkError",
     "ProtocolInvalidKeyIdError",
+    "DuplicateMessageError",
+    "NetworkError",
     "ProtocolInvalidMessageError",
     "ProtocolNoSessionError",
     "NoSuchAccountError",
     "ServerNotFoundError",
     "InvalidProxyError",
     "NoSendPermissionError",
     "InvalidAttachmentError",
```

### Comparing `aiosignald-0.3.6/aiosignald/generated.py` & `aiosignald-0.3.7/aiosignald/generated.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Generated using https://signald.org/protocol.json
-Version: '0.23.1'=
+Version: '0.23.2-7-1583b4df'=
 """
 from typing import Optional, TYPE_CHECKING
 from dataclasses import dataclass, field
 
 from .util import JSONProtocol, locals_to_request, dict_to_nested_dataclass
 
 if TYPE_CHECKING:
@@ -408,14 +408,15 @@
     data_message: Optional["JsonDataMessagev1"] = None
     sync_message: Optional["JsonSyncMessagev1"] = None
     call_message: Optional["CallMessagev1"] = None
     receipt_message: Optional["ReceiptMessagev1"] = None
     typing_message: Optional["TypingMessagev1"] = None
     story_message: Optional["StoryMessagev1"] = None
     server_guid: Optional[str] = None
+    decryption_error_message: Optional["DecryptionErrorMessagev1"] = None
 
 
 @dataclass
 class ListenerStatev1:
     """
     prior attempt to indicate signald connectivity state. WebSocketConnectionState messages will be delivered at the  same time as well as in other parts of the websocket lifecycle.
     """
@@ -725,14 +726,21 @@
     group: Optional["JsonGroupV2Infov1"] = None
     file: Optional["JsonAttachmentv1"] = None
     text: Optional["TextAttachmentv1"] = None
     allow_replies: Optional[bool] = None
 
 
 @dataclass
+class DecryptionErrorMessagev1:
+    timestamp: Optional[int] = None
+    device_id: Optional[int] = None
+    ratchet_key: Optional[str] = None
+
+
+@dataclass
 class JsonAttachmentv1:
     """
     represents a file attached to a message. When sending, only `filename` is required.
     """
 
     contentType: Optional[str] = None
     id: Optional[str] = None
@@ -1099,14 +1107,17 @@
 class SharedContactAvatarv1:
     attachment: Optional["JsonAttachmentv1"] = None
     is_profile: Optional[bool] = None
 
 
 @dataclass
 class Gradientv1:
+    colors: list[str] = field(default_factory=list)
+    angle: Optional[int] = None
+    positions: list[float] = field(default_factory=list)
     start_color: Optional[str] = None
     end_color: Optional[str] = None
 
 
 class SignaldGeneratedAPI(JSONProtocol):
     async def send(
         self,
@@ -1117,14 +1128,15 @@
         messageBody: Optional[str] = None,
         attachments: Optional[list["JsonAttachmentv1"]] = None,
         quote: Optional["JsonQuotev1"] = None,
         timestamp: Optional[int] = None,
         mentions: Optional[list["JsonMentionv1"]] = None,
         previews: Optional[list["JsonPreviewv1"]] = None,
         members: Optional[list["JsonAddressv1"]] = None,
+        is_for_story: Optional[bool] = None,
     ) -> SendResponsev1:
         """
 
 
         :param username: Example: "+12024561414"
         :param account: Example: "0cc10e61-d64c-4dbc-b51c-334f7dd45a4a"
         :param recipientAddress:
@@ -1132,14 +1144,15 @@
         :param messageBody: Example: "hello"
         :param attachments:
         :param quote:
         :param timestamp:
         :param mentions:
         :param previews:
         :param members: Optionally set to a sub-set of group members. Ignored if recipientGroupId isn't specified
+        :param is_for_story: set to true when replying to a story
         """
 
         return dict_to_nested_dataclass(
             SendResponsev1,
             await self.get_response(
                 {"type": "send", "version": "v1", **locals_to_request(locals())}
             ),
@@ -2287,14 +2300,15 @@
     "IdentityKeyv1",
     "JsonDataMessagev1",
     "JsonSyncMessagev1",
     "CallMessagev1",
     "ReceiptMessagev1",
     "TypingMessagev1",
     "StoryMessagev1",
+    "DecryptionErrorMessagev1",
     "JsonAttachmentv1",
     "JsonQuotev1",
     "JsonMentionv1",
     "JsonPreviewv1",
     "JsonReactionv1",
     "GroupAccessControlv1",
     "GroupMemberv1",
```

### Comparing `aiosignald-0.3.6/aiosignald/util.py` & `aiosignald-0.3.7/aiosignald/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass, is_dataclass, asdict
 import asyncio
 import dataclasses
 import json
 import logging
-import random
 import typing
 import types
+from uuid import uuid4
 
 from . import generated
 from . import exc
 
 
 class SignaldException(Exception):
     """
@@ -113,56 +113,79 @@
                     "Received payload:"
                     + "\n"
                     + json.dumps(payload, indent=4, sort_keys=True)
                 )
 
             for handler in self.specific_handlers:
                 if handler.validate(payload):
-                    self.logger.debug(f"Found a specific handler")
+                    self.logger.debug("Found a specific handler")
                     self.specific_handlers.remove(handler)
                     handler.callback(payload)
                     return
 
             id_ = payload.get("id")
             if id_ is None:
                 type_ = payload.get("type")
                 try:
                     generic_handler: typing.Callable = getattr(self, f"handle_{type_}")
                 except AttributeError:
                     self.logger.info(f"No method to handle {type_}, ignoring")
                     return
                 self.logger.debug(
-                    f"Method found to handle '%s': %s", type_, generic_handler
+                    "Method found to handle '%s': %s", type_, generic_handler
                 )
 
                 try:
                     attr = getattr(generated, type_ + self.PROTOCOL_VERSION)
                 except AttributeError:
                     self.logger.warning(
-                        f"No dataclass for: %s, passing raw JSON payload", type_
+                        "No dataclass for: %s, passing raw JSON payload", type_
                     )
                     data = payload
                 else:
-                    self.logger.debug(f"Found: %s", attr)
+                    self.logger.debug("Found: %s", attr)
                     data = dict_to_nested_dataclass(attr, payload["data"])
 
-                if asyncio.iscoroutinefunction(generic_handler):
-                    asyncio.create_task(generic_handler(data, payload))
-                else:
-                    generic_handler(data, payload)
+                try:
+                    if asyncio.iscoroutinefunction(generic_handler):
+                        asyncio.create_task(self.__wrap(generic_handler, data, payload))
+                    else:
+                        generic_handler(data, payload)
+                except Exception as e:
+                    self.exception(generic_handler, e)
             else:
                 callback = self.callbacks.pop(id_, None)
                 if callback is None:
                     self.logger.warning(
-                        f"Received payload with id but no callbacks were"
+                        "Received payload with id but no callbacks were"
                         "registered for it, ignoring"
                     )
                 else:
                     callback(payload)
 
+    async def __wrap(
+        self,
+        handler: typing.Callable[[typing.Any, dict], typing.Awaitable[None]],
+        data: typing.Any,
+        payload: dict,
+    ):
+        try:
+            await handler(data, payload)
+        except Exception as e:
+            self.exception(handler, e)
+
+    def exception(self, handler: typing.Callable, e: Exception):
+        """
+        Handle exceptions in generic handlers
+
+        Override this function or set the attribute to customize the default
+        behaviour, which is to just log the exception
+        """
+        self.logger.exception("Exception in %s", handler, exc_info=e)
+
     def send_request(
         self,
         payload: dict,
         id_: typing.Optional[str] = None,
         callback: typing.Optional[typing.Callable] = None,
     ):
         """
@@ -173,15 +196,15 @@
         :param callback: a Callable that will be called with the response payload
         """
         if self.transport is None:
             self.logger.warning("No transport, cannot send payload")
             return
 
         if id_ is None:
-            id_ = random_id()
+            id_ = str(uuid4())
         payload["id"] = id_
         payload["version"] = self.PROTOCOL_VERSION
 
         if callback is not None:
             self.callbacks[id_] = callback
 
         if self.logger.isEnabledFor(logging.DEBUG):
@@ -207,26 +230,22 @@
             return response
         else:
             return response.get("data", dict())
 
     def handle_version(self, _data, payload):
         # special case where the event type does not correspond to the proper structure
         # version vs JsonVersionMessage
-        return self.handle_JsonVersionMessage(generated.JsonVersionMessagev1(**payload["data"]))
+        return self.handle_JsonVersionMessage(
+            generated.JsonVersionMessagev1(**payload["data"])
+        )
 
     def handle_JsonVersionMessage(self, version):
         self.logger.info("Signald version: %s", version)
 
 
-def random_id(length=20):
-    return "".join(
-        random.choice("abcdefghijklmnopqrstuvwxyz0123456789") for _ in range(length)
-    )
-
-
 def locals_to_request(d: dict):
     """
     Helper for the generated bindings.
     """
     request: dict[str, typing.Any] = {}
     for k, v in d.items():
         if v is None or k == "self":
@@ -253,15 +272,15 @@
         return t._evaluate(generated.__dict__, locals(), frozenset())  # type:ignore
     else:
         return t
 
 
 def dict_to_nested_dataclass(cls: typing.Type[T], dikt) -> T:
     kwargs = {}
-    for field in dataclasses.fields(cls):
+    for field in dataclasses.fields(cls):  # type:ignore
         name = field.name
 
         dict_value = dikt.get(name)
         if dict_value is None:
             continue
 
         if isinstance(field.type, types.GenericAlias):
```

### Comparing `aiosignald-0.3.6/pyproject.toml` & `aiosignald-0.3.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 [tool.poetry]
 name = "aiosignald"
-version = "0.3.6"
+version = "0.3.7"
 description = "Python bindings for signald"
 authors = ["Nicolas Cedilnik <nicoco@nicoco.fr>"]
 readme = "README.md"
 homepage = "https://git.sr.ht/~nicoco/aiosignald"
 license = "AGPL-3.0-or-later"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <4"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^7.1"
 pytest-asyncio = "^0.19.0"
 Sphinx = "^4.5.0"
 requests = "^2.28.1"
 sphinx-rtd-theme = "^1.0.0"
 sphinx-autoapi = "^1.9.0"
-mypy = "^0.971"
+mypy = "^1.2"
+ruff = "^0.0.261"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.ruff]
+ignore = ["E501", "F403", "F405"]
```

### Comparing `aiosignald-0.3.6/setup.py` & `aiosignald-0.3.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,93 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: aiosignald
+Version: 0.3.7
+Summary: Python bindings for signald
+Home-page: https://git.sr.ht/~nicoco/aiosignald
+License: AGPL-3.0-or-later
+Author: Nicolas Cedilnik
+Author-email: nicoco@nicoco.fr
+Requires-Python: >=3.8,<4
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
 
-packages = \
-['aiosignald']
+Signald python bindings
+=======================
 
-package_data = \
-{'': ['*']}
 
-setup_kwargs = {
-    'name': 'aiosignald',
-    'version': '0.3.6',
-    'description': 'Python bindings for signald',
-    'long_description': 'Signald python bindings\n=======================\n\n\n[![pypi](https://badge.fury.io/py/aiosignald.svg)](https://pypi.org/project/aiosignald/)\n[![Documentation Status](https://readthedocs.org/projects/aiosignald/badge/?version=latest)](https://aiosignald.readthedocs.io/en/latest/)\n[![builds.sr.ht status](https://builds.sr.ht/~nicoco/aiosignald/commits/master/.build.yml.svg)](https://builds.sr.ht/~nicoco/aiosignald/commits/master/.build.yml?)\n\nInteract with the signal messaging network in python with sweet, sweet autocompletion.\n\nMost of the code is generated by the `generate.py` script that\nuses the schema available at <https://signald.org/protocol.json>.\n\nNo 3rd party dep, just the python standard lib.\n\nInstall\n-------\n\n`pip install aiosignald`\n\nHave signald running. See [their\ndocs](https://signald.org/articles/install/) about it.\n\nIssue tracker: https://todo.sr.ht/~nicoco/aiosignald\n\nPart of the [slidge project](https://sr.ht/~nicoco/slidge) (but can be used independently)\n\nUsage\n-----\n\n### Example: echo bot\n\n```py\nimport asyncio\n\nfrom aiosignald import SignaldAPI\nimport aiosignald.generated as api\n\nclass EchoBot(SignaldAPI):\n    async def handle_IncomingMessage(self, msg: api.IncomingMessagev1, _payload):\n        # hook to the incoming event by naming you function handle_EventName\n        # most stuff comes through an IncomingMessage anyway\n        print("Received: ", msg)\n        if (data_msg := msg.data_message) and (body := data_msg.body):\n            await self.send(\n                username=PHONE_NUMBER,\n                recipientAddress=msg.source,\n                messageBody=body\n            )\n\nasync def main():\n    loop = asyncio.get_running_loop()\n    _, signald = await loop.create_unix_connection(\n        EchoBot, path=SIGNALD_SOCKET_PATH)\n    if ACCOUNT_TYPE == "primary":\n        await signald.register(account=PHONE_NUMBER)\n        # Some async code to get the SMS code\n        code = await user_input("Enter your sms code?")\n        await signald.verify(account=PHONE_NUMBER, code=code)\n    else:\n        # linking to an existing account is also possible\n        resp = await signald.generate_linking_uri()\n        print("Make this a QR code and scan it on your primary signal device:", resp.uri)\n        await signald.finish_link(device_name="friendly-device-name", session_id=resp.session_id)\n    await signald.on_con_lost\n\n# See https://signald.org/articles/protocol/ for more info about this\nSIGNALD_SOCKET_PATH = "/var/run/signald/signald.sock"\nPHONE_NUMBER = "+XXXXXX"\nACCOUNT_TYPE = "primary"\n\nasyncio.run(main())\n```\n\nDocs are available on [readthedocs](https://aiosignald.readthedocs.org).\n',
-    'author': 'Nicolas Cedilnik',
-    'author_email': 'nicoco@nicoco.fr',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://git.sr.ht/~nicoco/aiosignald',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.8,<4',
-}
+[![pypi](https://badge.fury.io/py/aiosignald.svg)](https://pypi.org/project/aiosignald/)
+[![Documentation Status](https://readthedocs.org/projects/aiosignald/badge/?version=latest)](https://aiosignald.readthedocs.io/en/latest/)
+[![builds.sr.ht status](https://builds.sr.ht/~nicoco/aiosignald/commits/master/.build.yml.svg)](https://builds.sr.ht/~nicoco/aiosignald/commits/master/.build.yml?)
 
+Interact with the signal messaging network in python with sweet, sweet autocompletion.
+
+Most of the code is generated by the `generate.py` script that
+uses the schema available at <https://signald.org/protocol.json>.
+
+No 3rd party dep, just the python standard lib.
+
+Install
+-------
+
+`pip install aiosignald`
+
+Have signald running. See [their
+docs](https://signald.org/articles/install/) about it.
+
+Issue tracker: https://todo.sr.ht/~nicoco/aiosignald
+
+Part of the [slidge project](https://sr.ht/~nicoco/slidge) (but can be used independently)
+
+Usage
+-----
+
+### Example: echo bot
+
+```py
+import asyncio
+
+from aiosignald import SignaldAPI
+import aiosignald.generated as api
+
+class EchoBot(SignaldAPI):
+    async def handle_IncomingMessage(self, msg: api.IncomingMessagev1, _payload):
+        # hook to the incoming event by naming you function handle_EventName
+        # most stuff comes through an IncomingMessage anyway
+        print("Received: ", msg)
+        if (data_msg := msg.data_message) and (body := data_msg.body):
+            await self.send(
+                username=PHONE_NUMBER,
+                recipientAddress=msg.source,
+                messageBody=body
+            )
+
+async def main():
+    loop = asyncio.get_running_loop()
+    _, signald = await loop.create_unix_connection(
+        EchoBot, path=SIGNALD_SOCKET_PATH)
+    if ACCOUNT_TYPE == "primary":
+        await signald.register(account=PHONE_NUMBER)
+        # Some async code to get the SMS code
+        code = await user_input("Enter your sms code?")
+        await signald.verify(account=PHONE_NUMBER, code=code)
+    else:
+        # linking to an existing account is also possible
+        resp = await signald.generate_linking_uri()
+        print("Make this a QR code and scan it on your primary signal device:", resp.uri)
+        await signald.finish_link(device_name="friendly-device-name", session_id=resp.session_id)
+    await signald.on_con_lost
+
+# See https://signald.org/articles/protocol/ for more info about this
+SIGNALD_SOCKET_PATH = "/var/run/signald/signald.sock"
+PHONE_NUMBER = "+XXXXXX"
+ACCOUNT_TYPE = "primary"
+
+asyncio.run(main())
+```
+
+Docs are available on [readthedocs](https://aiosignald.readthedocs.org).
 
-setup(**setup_kwargs)
```

