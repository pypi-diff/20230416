# Comparing `tmp/cs_events-0.4.0.tar.gz` & `tmp/cs_events-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs_events-0.4.0.tar", max compression
+gzip compressed data, was "cs_events-0.4.1.tar", max compression
```

## Comparing `cs_events-0.4.0.tar` & `cs_events-0.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1090 2023-03-27 01:32:35.282886 cs_events-0.4.0/LICENSE
--rw-r--r--   0        0        0     1323 2023-03-28 18:01:28.007044 cs_events-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6756 2023-03-27 01:05:01.123372 cs_events-0.4.0/README.md
--rw-r--r--   0        0        0      495 2023-03-28 18:01:28.007044 cs_events-0.4.0/src/events/__init__.py
--rw-r--r--   0        0        0     3664 2023-03-27 01:05:01.125380 cs_events-0.4.0/src/events/_collections.py
--rw-r--r--   0        0        0     7137 2023-03-28 18:02:22.196045 cs_events-0.4.0/src/events/_event.py
--rw-r--r--   0        0        0     6962 2023-03-27 01:05:01.126383 cs_events-0.4.0/src/events/_events.py
--rw-r--r--   0        0        0     7739 1970-01-01 00:00:00.000000 cs_events-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-03-27 01:32:35.282886 cs_events-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1323 2023-04-16 14:04:20.620131 cs_events-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6756 2023-03-27 01:05:01.123372 cs_events-0.4.1/README.md
+-rw-r--r--   0        0        0      495 2023-04-16 14:04:20.626131 cs_events-0.4.1/src/events/__init__.py
+-rw-r--r--   0        0        0     3655 2023-04-01 15:38:35.471687 cs_events-0.4.1/src/events/_collections.py
+-rw-r--r--   0        0        0     7134 2023-04-01 15:37:38.747157 cs_events-0.4.1/src/events/_event.py
+-rw-r--r--   0        0        0     6948 2023-04-16 14:01:05.944034 cs_events-0.4.1/src/events/_events.py
+-rw-r--r--   0        0        0     7739 1970-01-01 00:00:00.000000 cs_events-0.4.1/PKG-INFO
```

### Comparing `cs_events-0.4.0/LICENSE` & `cs_events-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cs_events-0.4.0/pyproject.toml` & `cs_events-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cs-events"
-version = "0.4.0"
+version = "0.4.1"
 description = "C#-style event handling mechanism for Python"
 authors = ["Daniel Jeong <wise0704@outlook.com>"]
 keywords = ["python", "event", "c#"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/wise0704/python-cs-events"
 classifiers = [
```

### Comparing `cs_events-0.4.0/README.md` & `cs_events-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `cs_events-0.4.0/src/events/_collections.py` & `cs_events-0.4.1/src/events/_collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from collections.abc import Callable
-from typing import TYPE_CHECKING, Any, Protocol, Union, runtime_checkable
+from typing import TYPE_CHECKING, Protocol, Union, runtime_checkable
 
 from ._event import Event
 
 
 __all__ = [
     "EventHandlerCollection",
     "EventHandlerList",
     "EventHandlerDict",
 ]
 
 
-void = None | Any
+void = object
 
 
 @runtime_checkable
 class EventHandlerCollection(Protocol):
     """
     Provides a collection of event handler delegates.
     """
```

### Comparing `cs_events-0.4.0/src/events/_event.py` & `cs_events-0.4.1/src/events/_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 from collections.abc import Callable, Collection, Iterator
-from typing import Any, Generic, ParamSpec, final, overload
+from typing import Generic, ParamSpec, final, overload
 
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
@@ -18,19 +18,19 @@
 
 
 # Python does not provide a void type, which is a useful feature in callbacks,
 # and is clearly different from None.
 # Comparison with TS:
 #     function foo(): void {} <==> def foo() -> None: pass
 #     let bar: () => void;    <==> bar: Callable[[], Any]
-void = None | Any
+void = object
 P = ParamSpec("P")
 
 EventHandler = Callable[P, void]
-accessors = tuple[Callable[[Any, EventHandler[P]], void], Callable[[Any, EventHandler[P]], void]]
+accessors = tuple[Callable[[object, EventHandler[P]], void], Callable[[object, EventHandler[P]], void]]
 
 
 class Event(Collection[EventHandler[P]]):
     """
     Represents an event delegate that handlers can subscribe to.
 
     The type argument specifies the event data parameters::
```

### Comparing `cs_events-0.4.0/src/events/_events.py` & `cs_events-0.4.1/src/events/_events.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,27 +109,27 @@
     return _events(cls, collection)
 
 
 def _events(cls: T, collection: str | None, /) -> T:
     if not isinstance(cls, type):
         raise TypeError("Argument 'cls' must be a class.")
 
-    if collection is not None and collection.startswith("__") and not collection.endswith("__"):
+    if collection and collection.startswith("__") and not collection.endswith("__"):
         collection = f"_{cls.__name__.lstrip('_')}{collection}"
 
     fields: list[str] = [None]  # type: ignore
     properties: list[str] = []
 
     for (attr, T) in get_type_hints(cls).items():
         T = get_origin(T) or T
         if T is Event:
             fields.append(f"self.{attr} = Event()")
         elif T is event:
             properties.append(attr)
-        elif collection is None and isinstance(T, type) and issubclass(T, EventHandlerCollection):
+        elif not collection and isinstance(T, type) and issubclass(T, EventHandlerCollection):
             collection = attr
 
     if len(fields) > 1:
         _fields(cls, fields)
 
     if properties:
         _properties(cls, properties, collection)
@@ -209,8 +209,9 @@
 
     Args:
      - key (object): A key for the event handler collection to use.
 
     Returns:
         (event[...]): A hint for the ``@events`` decorator to use the specified key instead.
     """
+
     return key  # type: ignore
```

### Comparing `cs_events-0.4.0/PKG-INFO` & `cs_events-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs-events
-Version: 0.4.0
+Version: 0.4.1
 Summary: C#-style event handling mechanism for Python
 Home-page: https://github.com/wise0704/python-cs-events
 License: MIT
 Keywords: python,event,c#
 Author: Daniel Jeong
 Author-email: wise0704@outlook.com
 Requires-Python: >=3.10,<4.0
```

