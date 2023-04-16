# Comparing `tmp/plainlog-0.1.1.tar.gz` & `tmp/plainlog-0.1.3.tar.gz`

## Comparing `plainlog-0.1.1.tar` & `plainlog-0.1.3.tar`

### file list

```diff
@@ -1,62 +1,30 @@
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 plainlog-0.1.1/.pdm.toml
--rw-r--r--   0        0        0    10611 2020-02-02 00:00:00.000000 plainlog-0.1.1/hello.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 plainlog-0.1.1/immod.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 plainlog-0.1.1/tasks.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 plainlog-0.1.1/.github/workflows/test.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/.gitignore
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/.update-informer
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/10e84d17b86234ee
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/263286bccf0b0787
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/26dc59c54d87f4db
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/2abaa79b4e523ee2
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/2c43b14d0410b017
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/38ff43c1e137a084
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/431978924f5542c0
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/483ad389044e5f19
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/4c57face63c9d03a
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/54b2e4d67f4cdb86
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/5823987a91c4bec
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/5ab26d91046ed93e
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/5be073268caeef17
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/5e9e9be0d3601fd4
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/63cca12c1153aeb2
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/73caa4191fa489cb
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/74fba163336ab6f3
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/76e02d9e1923d9b5
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/79dfcb16bebe6942
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/7f7a48c0641916e3
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/83c8f249d7b569c0
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/99be8d3ce5137152
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/9c3ed1114cd064ce
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/aa25d461a11656e7
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/afc6447828d60548
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/b9e567d856ab6cbc
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/cbc8ce83f20d816
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/dd02e01df8e132c6
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 plainlog-0.1.1/.ruff_cache/content/e2c3c13a6bcbd665
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 plainlog-0.1.1/.vscode/launch.json
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 plainlog-0.1.1/src/plainlog/__init__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 plainlog-0.1.1/src/plainlog/__version__.py
--rw-r--r--   0        0        0     9359 2020-02-02 00:00:00.000000 plainlog-0.1.1/src/plainlog/_dev.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 plainlog-0.1.1/src/plainlog/_env.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 plainlog-0.1.1/src/plainlog/_frames.py
--rw-r--r--   0        0        0    14627 2020-02-02 00:00:00.000000 plainlog-0.1.1/src/plainlog/_logger.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 plainlog-0.1.1/src/plainlog/_recattrs.py
--rw-r--r--   0        0        0     6631 2020-02-02 00:00:00.000000 plainlog-0.1.1/src/plainlog/configure.py
--rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 plainlog-0.1.1/src/plainlog/formatters.py
--rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 plainlog-0.1.1/src/plainlog/handlers.py
--rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 plainlog-0.1.1/src/plainlog/processors.py
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 plainlog-0.1.1/src/plainlog/utils.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 plainlog-0.1.1/src/plainlog/warnings.py
--rw-r--r--   0        0        0    11431 2020-02-02 00:00:00.000000 plainlog-0.1.1/src/plainlog_extensions/_rich_handler.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 plainlog-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 plainlog-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 plainlog-0.1.1/tests/test_bind.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 plainlog-0.1.1/tests/test_import.py
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 plainlog-0.1.1/.gitignore
--rw-r--r--   0        0        0     6656 2020-02-02 00:00:00.000000 plainlog-0.1.1/README.md
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 plainlog-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 plainlog-0.1.1/LICENSES/Apache-2.0.txt
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 plainlog-0.1.1/LICENSES/MIT.txt
--rw-r--r--   0        0        0     8066 2020-02-02 00:00:00.000000 plainlog-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 plainlog-0.1.3/Makefile
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 plainlog-0.1.3/std_hello.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 plainlog-0.1.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 plainlog-0.1.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0    11431 2020-02-02 00:00:00.000000 plainlog-0.1.3/scripts/plainlog_extensions/_rich_handler.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 plainlog-0.1.3/src/plainlog/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 plainlog-0.1.3/src/plainlog/__version__.py
+-rw-r--r--   0        0        0     9051 2020-02-02 00:00:00.000000 plainlog-0.1.3/src/plainlog/_dev.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 plainlog-0.1.3/src/plainlog/_env.py
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 plainlog-0.1.3/src/plainlog/_frames.py
+-rw-r--r--   0        0        0    16539 2020-02-02 00:00:00.000000 plainlog-0.1.3/src/plainlog/_logger.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 plainlog-0.1.3/src/plainlog/_recattrs.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 plainlog-0.1.3/src/plainlog/_utils.py
+-rw-r--r--   0        0        0     6632 2020-02-02 00:00:00.000000 plainlog-0.1.3/src/plainlog/configure.py
+-rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 plainlog-0.1.3/src/plainlog/formatters.py
+-rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 plainlog-0.1.3/src/plainlog/handlers.py
+-rw-r--r--   0        0        0     7344 2020-02-02 00:00:00.000000 plainlog-0.1.3/src/plainlog/processors.py
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 plainlog-0.1.3/src/plainlog/std.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 plainlog-0.1.3/src/plainlog/warnings.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 plainlog-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 plainlog-0.1.3/tests/conftest.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 plainlog-0.1.3/tests/test_bind.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 plainlog-0.1.3/tests/test_import.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 plainlog-0.1.3/tests/test_utils.py
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 plainlog-0.1.3/.gitignore
+-rw-r--r--   0        0        0     6656 2020-02-02 00:00:00.000000 plainlog-0.1.3/README.md
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 plainlog-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 plainlog-0.1.3/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 plainlog-0.1.3/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     8066 2020-02-02 00:00:00.000000 plainlog-0.1.3/PKG-INFO
```

### Comparing `plainlog-0.1.1/.github/workflows/test.yml` & `plainlog-0.1.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `plainlog-0.1.1/src/plainlog/_dev.py` & `plainlog-0.1.3/src/plainlog/_dev.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,41 +8,36 @@
 
 import sys
 
 from io import StringIO
 from typing import Any, Iterable, TextIO, Type, Union
 
 from ._frames import _format_exception
+from .formatters import format_message
 
 from typing import Protocol
 
 try:
     import colorama
 except ImportError:
-    colorama = None
-
-try:
-    import better_exceptions
-except ImportError:
-    better_exceptions = None
+    colorama = None  # type: ignore[assignment]
 
 try:
     import rich
 
     from rich.console import Console
     from rich.traceback import Traceback
 except ImportError:
     rich = None  # type: ignore[assignment]
 
 
 __all__ = [
     "ConsoleRenderer",
     "plain_traceback",
     "rich_traceback",
-    "better_traceback",
 ]
 
 _IS_WINDOWS = sys.platform == "win32"
 
 _MISSING = "{who} requires the {package} package installed.  "
 _EVENT_WIDTH = 40  # pad the event name to so many characters
 
@@ -149,32 +144,25 @@
 def plain_traceback(sio: TextIO, exc_info) -> None:
     sio.write("\n" + _format_exception(exc_info))
 
 
 def rich_traceback(sio: TextIO, exc_info) -> None:
     sio.write("\n")
     Console(file=sio, color_system="truecolor").print(
-        Traceback.from_exception(*exc_info, show_locals=True)
+        Traceback.from_exception(*exc_info, show_locals=True)  # noqa
     )
 
 
-def better_traceback(sio: TextIO, exc_info) -> None:
-    sio.write("\n" + "".join(better_exceptions.format_exception(*exc_info)))
-
-
 if rich is not None:
     default_exception_formatter = rich_traceback
-elif better_exceptions is not None:
-    default_exception_formatter = better_traceback
 else:
     default_exception_formatter = plain_traceback
 
 
 class ConsoleRenderer:
-
     def __init__(
         self,
         pad_event: int = _EVENT_WIDTH,
         colors: bool = _use_colors,
         force_colors: bool = False,
         repr_native_str: bool = False,
         level_styles: Styles | None = None,
@@ -235,15 +223,14 @@
 
         if isinstance(val, str):
             return val
         else:
             return repr(val)
 
     def __call__(self, record) -> str:
-
         sio = StringIO()
 
         ts = record.get("datetime", None)
         if ts is not None:
             sio.write(
                 # can be a number if timestamp is UNIXy
                 self._styles.timestamp
@@ -262,16 +249,15 @@
                 level = level.name
                 sio.write(
                     self._level_to_color.get(level, "")
                     + _pad(level, self._longest_level + 1)
                     + self._styles.reset
                 )
 
-        event = record.get("message", "")
-        # event = record.get("message_fmt", event)
+        event = format_message(record)
         if not isinstance(event, str):
             event = str(event)
 
         extra = record.get("extra")
         logger_name = record.get("name", None)
         if not self._log_name:
             logger_name = None
```

### Comparing `plainlog-0.1.1/src/plainlog/_frames.py` & `plainlog-0.1.3/src/plainlog/_frames.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SPDX-FileCopyrightText: 2023 Wolfgang Langner <tds333@mailbox.org>
 #
 # SPDX-License-Identifier: Apache-2.0 OR MIT
 from __future__ import annotations
 
 import sys
 import traceback
+from typing import Tuple
 
 from io import StringIO
 from types import FrameType
 
 
 def get_frame_fallback(n):
     try:
@@ -46,15 +47,15 @@
         s = s[:-1]
 
     return s
 
 
 def _find_first_app_frame_and_name(
     additional_ignores: list[str] | None = None,
-) -> tuple[FrameType, str]:
+) -> Tuple[FrameType, str]:
     """
     Remove all intra-plainlog calls and return the relevant app frame.
 
     :param additional_ignores: Additional names with which the first frame must
         not start.
 
     :returns: tuple of (frame, name)
```

### Comparing `plainlog-0.1.1/src/plainlog/_logger.py` & `plainlog-0.1.3/src/plainlog/_logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 from threading import Thread, Event
 from queue import SimpleQueue
 from enum import Enum
 import atexit
 import traceback
 from functools import partial
 from multiprocessing import current_process
+from typing import Union, Optional, Callable, Iterable, Any, Generator, Tuple, Dict
 
 from . import _env
 from ._recattrs import Level, HandlerRecord, Options
 from ._frames import get_frame
 
 
 get_now_utc = partial(datetime.now, timezone.utc)
-start_time = get_now_utc()
-context = ContextVar("plainlog_context", default={})
+context: ContextVar = ContextVar("plainlog_context", default={})
 logger_process = current_process()
 
 # predefined for performance reason
 LEVEL_DEBUG = Level(logging.DEBUG, "DEBUG")
 LEVEL_INFO = Level(logging.INFO, "INFO")
 LEVEL_WARNING = Level(logging.WARNING, "WARNING")
 LEVEL_ERROR = Level(logging.ERROR, "ERROR")
@@ -40,15 +40,22 @@
     ADD_HANDLER = "ADD_HANDLER"
     REMOVE_HANDLER = "REMOVE_HANDLER"
     OPTIONS = "OPTIONS"
     UPDATE_LEVELS = "UPDATE_LEVELS"
     EVENT = "EVENT"
 
 
-def _validate_callables(callables, name="Callable"):
+LevelInput = Union[int, str, Level]
+Levels = Dict[LevelInput, Level]
+Callables = Union[Callable, Iterable[Callable]]
+
+
+def _validate_callables(
+    callables: Optional[Union[Callable, Iterable[Callable]]], name: str = "Callable"
+) -> Tuple[Callable, ...]:
     if callables is not None:
         if isinstance(callables, collections.abc.Iterable):
             callables = tuple(callables)
         else:
             callables = (callables,)
 
         for c in callables:
@@ -56,120 +63,145 @@
                 raise ValueError(f"{name} '{c}' must be a callable object.")
     else:
         callables = ()
 
     return callables
 
 
-def _validate_extra(extra):
+def _validate_extra(extra: Optional[Dict[str, Any]]) -> Dict[str, Any]:
     if extra is None:
         extra = {}
     else:
         if not isinstance(extra, collections.abc.Mapping):
             raise ValueError("Extra must be a Mapping (dict like) object.")
         extra = deepcopy(extra)
 
     return extra
 
 
-def _validate_name(name):
+def _validate_name(name: str) -> str:
     if not isinstance(name, str):
         raise ValueError("Name must be a string.")
 
     return name
 
 
-def _get_levels():
-    levels = {}
+def _get_levels() -> Levels:
+    levels: Levels = {}
     for no, name in logging._levelToName.items():
         level = Level(no, name)
         levels[no] = level
         levels[name] = level
         levels[level] = level
         levels[name[0]] = level
 
     return levels
 
 
 class Core:
-    def __init__(self):
-        self._max_level_no = sys.maxsize
-        self.min_level_no = self._max_level_no
-        self._levels = _get_levels()
-        self._handlers = {}
-        self._options = Options("CORE", (), (), {})
-        self._queue = SimpleQueue()
-        self._thread = Thread(target=self._worker, daemon=True, name="plainlog-worker")
+    def __init__(self) -> None:
+        self._max_level_no: int = sys.maxsize
+        self._min_level_no: int = self._max_level_no
+        self._levels: Levels = _get_levels()
+        self._handlers: Dict[str, HandlerRecord] = {}
+        self._options: Options = Options("CORE", (), (), {})
+        self._queue: SimpleQueue = SimpleQueue()
+        self._thread: Thread = Thread(target=self._worker, daemon=True, name="plainlog-worker")
         self._thread.start()
 
     def __getstate__(self):
         state = self.__dict__.copy()
         state["_queue"] = None
+        state["_thread"] = None
         return state
 
     def __setstate__(self, state):
         self.__dict__.update(state)
         self._queue = SimpleQueue()
+        self._thread = Thread(target=self._worker, daemon=True, name="plainlog-worker")
+        self._thread.start()
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         handlers = list(self._handlers.values())
         return f"<plainlog.Core handlers={handlers!r}>"
 
-    def put(self, message, command=Command.LOG):
+    @property
+    def options(self) -> Options:
+        return self._options
+
+    @property
+    def min_level_no(self) -> int:
+        return self._min_level_no
+
+    def _put(self, command: Command, message: Any = None):
         self._queue.put((command, message))
 
-    def stop(self):
-        self.put(None, Command.STOP)
+    def log(self, log_record: Dict[str, Any], processors: Callables) -> None:
+        self._queue.put((Command.LOG, (log_record, processors)))
+
+    def stop(self) -> None:
+        self._put(Command.STOP)
 
-    def join(self):
+    def join(self) -> None:
         self._thread.join()
 
-    def is_alive(self):
+    def is_alive(self) -> bool:
         return self._thread.is_alive()
 
-    def level(self, level):
+    def level(self, level: Union[str, int, Level]) -> Level:
         ret = self._levels.get(level)
 
         if ret is None:
             raise ValueError(f"Invalid level {level!r}. Does not exist.")
 
         return ret
 
     def configure(
-        self, *, handlers=None, extra=None, preprocessors=None, processors=None, update_levels=False
+        self,
+        *,
+        handlers=None,
+        extra: Optional[Dict[str, Any]] = None,
+        preprocessors: Optional[Callables] = None,
+        processors: Optional[Callables] = None,
+        update_levels: bool = False,
     ):
         if handlers is not None:
             self.remove()
         else:
             handlers = []
 
         if update_levels:
-            self.put((None, Command.UPDATE_LEVELS))
+            self._put(Command.UPDATE_LEVELS)
 
         extra = _validate_extra(extra)
         preprocessors = _validate_callables(preprocessors, "Preprocessor")
         processors = _validate_callables(processors, "Processor")
         options = Options("CORE", preprocessors, processors, extra)
-        self.put(options, Command.OPTIONS)
+        self._put(Command.OPTIONS, options)
+
+        added = []
+        for params in handlers:
+            added.append(self.add(**params))
+        if not added:
+            self.wait_for_processed(_env.DEFAULT_WAIT_TIMEOUT)
 
-        return [self.add(**params) for params in handlers]
+        return added
 
-    def wait_for_processed(self, timeout=None):
+    def wait_for_processed(self, timeout: Optional[float] = None) -> None:
         event = Event()
-        self.put(event, Command.EVENT)
+        self._put(Command.EVENT, event)
         event.wait(timeout)
 
     def add(
         self,
-        handler,
-        name=None,
-        level=None,
-        print_errors=True,
-    ):
-
+        handler: Callable,
+        name: Optional[str] = None,
+        level: Optional[Union[str, int, Level]] = None,
+        print_errors: bool = True,
+    ) -> HandlerRecord:
         if not callable(handler):
             raise TypeError(
                 "Cannot log to objects of type '%s'. Object must be a callable."
                 % type(handler).__name__
             )
 
         if name is None:
@@ -179,41 +211,48 @@
                 name = handler.__class__.__name__
 
         level = _env.PLAINLOG_LEVEL if level is None else level
         level = self.level(level)
 
         handler_record = HandlerRecord(name, level, print_errors, handler)
 
-        self.put(handler_record, Command.ADD_HANDLER)
-        self.wait_for_processed()
+        self._put(Command.ADD_HANDLER, handler_record)
+        self.wait_for_processed(_env.DEFAULT_WAIT_TIMEOUT)
 
         return handler_record
 
-    def remove(self, name=None):
+    def remove(self, name: Optional[str] = None) -> None:
         if not (name is None or isinstance(name, str)):
             raise TypeError(
                 "Invalid handler name, it should be an string " "or None, not: '%s'" % type(name)
             )
 
-        self.put(name, Command.REMOVE_HANDLER)
-        self.wait_for_processed()
+        self._put(Command.REMOVE_HANDLER, name)
+        self.wait_for_processed(_env.DEFAULT_WAIT_TIMEOUT)
+
+    def has_handlers(self) -> bool:
+        return bool(self._handlers)
 
-    def close(self):
+    def close(self) -> None:
         if self.is_alive():
+            self.wait_for_processed(_env.DEFAULT_WAIT_TIMEOUT)
             self.remove()
             self.stop()
             self.join()
 
-    def _worker(self):
+    def _worker(self) -> None:
         queue = self._queue
 
         while True:
-            command, message = None, None
-            with contextlib.suppress(Exception):
+            # command, message = None, None
+            # with contextlib.suppress(Exception):
+            try:
                 command, message = queue.get()
+            except Exception:
+                continue
 
             if command is Command.LOG:
                 log_record, processors = message
 
                 stop = False
                 for p in (*processors, *self._options.processors):
                     with contextlib.suppress(Exception):
@@ -237,35 +276,32 @@
 
             elif command is Command.ADD_HANDLER:
                 handlers = self._handlers.copy()
                 handler_record = message
                 name = handler_record.name
                 if name not in self._handlers:
                     handlers[name] = handler_record
-                    self.min_level_no = min(self.min_level_no, handler_record.level.no)
+                    self._min_level_no = min(self._min_level_no, handler_record.level.no)
                     self._handlers = handlers
 
             elif command is Command.REMOVE_HANDLER:
                 handlers = self._handlers.copy()
                 name_ = message
                 handler_names = list(handlers.keys())
                 if name_ is not None:
                     handler_names = [name_]
 
                 for handler_name in handler_names:
-                    name, level, print_errors, handler = handlers.pop(
-                        handler_name, (None, None, None, None)
-                    )
-
-                    if name is None:
+                    if handler_name not in handlers:
                         continue
+                    else:
+                        name, level, print_erros, handler = handlers.pop(handler_name)
 
                     levelnos = (h.level.no for h in handlers.values())
-                    self.min_level_no = min(levelnos, default=self._max_level_no)
-                    # self._handlers = handlers
+                    self._min_level_no = min(levelnos, default=self._max_level_no)
 
                     if hasattr(handler, "close") and callable(handler.close):
                         try:
                             handler.close()
                         except Exception as ex:
                             if print_errors:
                                 print(
@@ -282,15 +318,15 @@
                 self._levels = _get_levels()
 
             elif command is Command.EVENT:
                 event = message
                 event.set()
 
     @staticmethod
-    def _print_error(record, handler_name, exception=None):
+    def _print_error(record: dict, handler_name: str, exception=None):
         if not sys.stderr or sys.stderr.closed:
             return
 
         if exception is None:
             type_, value, traceback_ = sys.exc_info()
         else:
             type_, value, traceback_ = (type(exception), exception, exception.__traceback__)
@@ -307,146 +343,150 @@
         except OSError:
             pass
         finally:
             del type_, value, traceback_
 
 
 class Logger:
-
     # core should be the same for every logger, options change per logger
-    def __init__(self, core, name, preprocessors, processors, extra):
+    def __init__(
+        self,
+        core: Core,
+        name: str,
+        preprocessors: Optional[Callables],
+        processors: Optional[Callables],
+        extra: Optional[Dict[str, Any]],
+    ):
         self._core = core
         name = _validate_name(name)
         preprocessors = _validate_callables(preprocessors, "Preprocessor")
         processors = _validate_callables(processors, "Processor")
         extra = _validate_extra(extra)
         self._options = Options(name, preprocessors, processors, extra)
 
     def __repr__(self):
         name = self._options.name
         core = repr(self._core)
         return f"<plainlog.Logger name={name!r} core={core}>"
 
-    def new(self, name=None, preprocessors=None, processors=None, extra=None):
+    def new(self, name: Optional[str] = None, preprocessors=None, processors=None, extra=None):
         name_, preprocessors_, processors_, extra_ = self._options
         # special handling to autodetect name, only for empty new
         if name is None and preprocessors is None and processors is None and extra is None:
             names = []
             frame = get_frame(1)
             with contextlib.suppress(KeyError):
                 module_name = frame.f_globals["__name__"]
                 names.append(module_name)
                 code = frame.f_code
                 qualname = code.co_name
-                file_name = code.co_filename
+                # file_name = code.co_filename
                 with contextlib.suppress(AttributeError):
                     qualname = code.co_qualname  # from 3.11 on available
                 if qualname and qualname != "<module>":
                     names.append(qualname)
             name = ".".join(names)  # TODO: finish impl to handle all cases and asign names correct
 
         name = name_ if name is None else name
         preprocessors = preprocessors_ if preprocessors is None else preprocessors
         processors = processors_ if processors is None else processors
         extra = extra_ if extra is None else extra
 
         return self.__class__(self._core, name, preprocessors, processors, extra)
 
-    def bind(self, **kwargs):  # noqa: N805
-        *options, extra = self._options
-        return self.__class__(self._core, *options, {**extra, **kwargs})
-
-    def unbind(self, *args):  # noqa: N805
-        *options, old_extra = self._options
-        extra = old_extra.copy()
+    def bind(self, **kwargs) -> "Logger":
+        name, preprocessors, processors, extra = self._options
+        return self.__class__(self._core, name, preprocessors, processors, {**extra, **kwargs})
+
+    def unbind(self, *args) -> "Logger":
+        name, preprocessors, processors, old_extra = self._options
+        extra: Dict[str, Any] = old_extra.copy()
         for key in args:
             extra.pop(key, None)
 
-        return self.__class__(self._core, *options, extra)
+        return self.__class__(self._core, name, preprocessors, processors, extra)
 
     @staticmethod
     def context(**kwargs):
         new_context = {**context.get(), **kwargs}
         token = context.set(new_context)
 
         return token
 
     @staticmethod
-    def reset_context(token):
+    def reset_context(token) -> None:
         context.reset(token)
 
     @staticmethod
     @contextlib.contextmanager
-    def contextualize(**kwargs):  # noqa: N805
+    def contextualize(**kwargs) -> Generator:  # noqa: N805
         token = Logger.context(**kwargs)
         try:
             yield token
         finally:
             Logger.reset_context(token)
 
-    def _log(self, level, msg, args, kwargs):
+    def _log(self, level: Level, msg: str, args: Tuple[Any, ...], kwargs: dict) -> None:
         level_no, _ = level
         core = self._core
 
         if level_no < core.min_level_no:
             return
 
         current_datetime = get_now_utc()
-        elapsed = current_datetime - start_time
 
-        _, core_preprocessors, __, core_extra = core._options
+        _, core_preprocessors, __, core_extra = core.options
         name, preprocessors, processors, extra = self._options
 
         log_record = {
-            "elapsed": elapsed,
             "level": level,
             "msg": msg,  # raw message as in std logging
             "message": str(msg),
             "name": name,
             "datetime": current_datetime,
-            "process_id" : logger_process.ident,
-            "process_name" : logger_process.name,
+            "process_id": logger_process.ident,
+            "process_name": logger_process.name,
             "context": {**context.get()},
             "extra": {**core_extra, **extra},
             "args": args,
             "kwargs": kwargs,
         }
 
         stop = False
         for preprocessor in (*preprocessors, *core_preprocessors):
             stop = preprocessor(log_record)
             if stop:
                 return
 
-        core.put((log_record, processors))
+        core.log(log_record, processors)
 
-    def debug(self, msg, *args, **kwargs):  # noqa: N805
+    def debug(self, msg: str, *args, **kwargs) -> None:  # noqa: N805
         self._log(LEVEL_DEBUG, msg, args, kwargs)
 
-    def info(self, msg, *args, **kwargs):  # noqa: N805
+    def info(self, msg: str, *args, **kwargs) -> None:  # noqa: N805
         self._log(LEVEL_INFO, msg, args, kwargs)
 
-    def warning(self, msg, *args, **kwargs):  # noqa: N805
+    def warning(self, msg: str, *args, **kwargs) -> None:  # noqa: N805
         self._log(LEVEL_WARNING, msg, args, kwargs)
 
-    def error(self, msg, *args, **kwargs):  # noqa: N805
+    def error(self, msg: str, *args, **kwargs) -> None:  # noqa: N805
         self._log(LEVEL_ERROR, msg, args, kwargs)
 
-    def critical(self, msg, *args, **kwargs):  # noqa: N805
+    def critical(self, msg: str, *args, **kwargs) -> None:  # noqa: N805
         self._log(LEVEL_CRITICAL, msg, args, kwargs)
 
-    def exception(self, msg, *args, **kwargs):  # noqa: N805
+    def exception(self, msg: str, *args, **kwargs) -> None:  # noqa: N805
         kwargs["exc_info"] = True
         self._log(LEVEL_ERROR, msg, args, kwargs)
 
-    def log(self, level, msg, *args, **kwargs):  # noqa: N805
+    def log(self, level: LevelInput, msg: str, *args, **kwargs) -> None:
         level = self._core.level(level)
         self._log(level, msg, args, kwargs)
 
-    def __call__(self, level=LEVEL_DEBUG, msg="", *args, **kwargs):  # noqa: N805
+    def __call__(self, level: LevelInput = LEVEL_DEBUG, msg="", *args, **kwargs) -> None:
         level = self._core.level(level)
         self._log(level, msg, args, kwargs)
 
 
 logger_core = Core()
 atexit.register(logger_core.close)
```

### Comparing `plainlog-0.1.1/src/plainlog/configure.py` & `plainlog-0.1.3/src/plainlog/configure.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,14 +216,15 @@
     "fingerscrossed_file": _fingerscrossed_file,
     "console_no_color": _console_no_color,
     "fast": _fast,
     "empty": _empty,
     "no_init": _no_init,
 }
 
+
 def add_profile(name, function):
     if name in _profiles:
         return False
     _profiles[name] = function
 
 
 def configure_log(name=None, level=None, extra=None, **kwargs):
```

### Comparing `plainlog-0.1.1/src/plainlog/formatters.py` & `plainlog-0.1.3/src/plainlog/formatters.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 # SPDX-FileCopyrightText: 2023 Wolfgang Langner <tds333@mailbox.org>
 #
 # SPDX-License-Identifier: Apache-2.0 OR MIT
 import json
-from ._dev import ConsoleRenderer
+from ._utils import eval_format
 
 
 def format_message(record):
     preformatted = record.get("preformatted", False)
     message = record.get("message", "")
     if preformatted:
         return message
     msg = record.get("msg", "")
     args = record.get("args", [])
     kwargs = record.get("kwargs", {})
     if msg and (args or kwargs):
-        message = msg.format(*args, **kwargs)
+        message = eval_format(msg, args, kwargs)
 
     return message
 
 
 class SimpleFormatter:
-
     DEFAULT_FORMAT = "{datetime} {level.name:<8} [{name}] {message}"
 
     def __init__(self, fmt=None):
         self._fmt = fmt if fmt is not None else self.DEFAULT_FORMAT
 
     def __call__(self, record):
-        message = format_message(record)
         data = record.copy()
-        data["message"] = message
+        data["message"] = format_message(record)
         message = self._fmt.format_map(data)
 
         return message
 
 
 class DefaultFormatter:
-
     DEFAULT_FORMAT = "{datetime:%H:%M:%S.%f} {level.name:<8} [{name}] {message} {extra}"
 
     def __init__(self):
         self._fmt = DefaultFormatter.DEFAULT_FORMAT
 
     def __call__(self, record):
         message = format_message(record)
@@ -67,15 +64,14 @@
     # message = _DEFAULT_FORMAT.format_map(data)
     message = fmt.format_map(data)
 
     return message
 
 
 class JsonFormatter:
-
     DEFAULT_ADDITIONAL_KEYS = (
         "file_name",
         "file_path",
         "function",
         "line",
         "module",
         "process_id",
@@ -108,28 +104,23 @@
 
         message = format_message(record)
 
         serializable = {
             "message": message,
             "name": record["name"],
             "datetime": record["datetime"].isoformat(),
-            "level": {
-                "name": record["level"].name,
-                "no": record["level"].no,
-            },
+            "timestamp": record["datetime"].timestamp(),
+            "level_name": record["level"].name,
+            "level_no": record["level"].no,
             "extra": record["extra"],
-            "elapsed": {
-                "repr": record["elapsed"],
-                "seconds": record["elapsed"].total_seconds(),
-            },
             "process_id": record["process_id"],
             "process_name": record["process_name"],
-            # "time": {"repr": record["time"], "timestamp": record["time"].timestamp()},
         }
-        if exception: serializable["exception"] = exception
+        if exception:
+            serializable["exception"] = exception
         for key in self._additional_keys:
             value = record.get(key)
             if value is not None:
                 serializable[key] = value
 
         return json.dumps(
             serializable,
```

### Comparing `plainlog-0.1.1/src/plainlog/handlers.py` & `plainlog-0.1.3/src/plainlog/handlers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 # SPDX-FileCopyrightText: 2023 Wolfgang Langner <tds333@mailbox.org>
 #
 # SPDX-License-Identifier: Apache-2.0 OR MIT
 import os
 import stat
 import sys
 import logging
+import asyncio
 from collections import deque
 import pathlib
+from typing import Protocol, Dict, Any
+
 from .formatters import (
     SimpleFormatter,
-    ConsoleRenderer,
     JsonFormatter,
     default_formatter,
 )
+from . import _env
+from ._dev import ConsoleRenderer
+
+
+class HandlerProtocol(Protocol):
+    def __call__(self, record: Dict[str, Any]) -> None:
+        ...
 
 
 class StreamHandler:
     def __init__(self, stream=None, formatter=None):
         if stream is None:
             stream = sys.stderr
         self._stream = stream
@@ -49,15 +58,14 @@
     def __init__(self, stream=None, colors=True):
         if stream is None:
             stream = sys.stdout
         super().__init__(stream, ConsoleRenderer(colors=colors))
 
 
 class WrapStandardHandler:
-
     factory = logging.getLogRecordFactory()
 
     def __init__(self, handler):
         self._handler = handler
 
     def __repr__(self):
         return f"{self.__class__.__name__}(handler={self._handler!r})"
@@ -224,7 +232,30 @@
         if (
             not result
             or result[stat.ST_DEV] != self._file_dev
             or result[stat.ST_INO] != self._file_ino
         ):
             self._close_file()
             self._create_file()
+
+
+class AsyncHandler:
+    def __init__(self, loop=None, formatter=None):
+        self.loop = asyncio.get_running_loop() if loop is None else loop
+        self._formatter = SimpleFormatter() if formatter is None else formatter
+        self.terminator = "\n"
+        self.last_future = None
+
+    def __call__(self, record):
+        message = self._formatter(record)
+        if self.loop.is_running():
+            self.last_future = asyncio.run_coroutine_threadsafe(self.write(message), self.loop)
+
+    async def write(self, message):
+        pass
+
+    def close(self):
+        if self.last_future is not None:
+            self.last_future.result(_env.DEFAULT_WAIT_TIMEOUT)
+
+    def __repr__(self):
+        return f"{self.__class__.__name__}(formatter={self._formatter.__class__.__name__})"
```

### Comparing `plainlog-0.1.1/src/plainlog/processors.py` & `plainlog-0.1.3/src/plainlog/processors.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,23 +11,33 @@
 import sys
 import contextlib
 from threading import current_thread
 from multiprocessing import current_process
 from os.path import basename, splitext
 from pathlib import Path
 import time
+from datetime import datetime, timezone
 from functools import lru_cache
+from typing import Protocol, Dict, Any, Optional
 
 from ._recattrs import RecordException
 from ._frames import get_frame
+from ._utils import eval_lambda_dict, eval_lambda_list, eval_dict, eval_list, eval_format
 
 
 STOP_PROCESSING = True
 CONTINUE_PROCESSING = False
 
+start_time = datetime.now(timezone.utc)
+
+
+class ProcessorProtocol(Protocol):
+    def __call__(self, record: Dict[str, Any]) -> Optional[bool]:
+        ...
+
 
 def add_caller_info(record, level=3):
     frame = get_frame(level)
     # name = frame.f_globals["__name__"]
     code = frame.f_code
     file_path = code.co_filename
     file_name = basename(file_path)
@@ -49,28 +59,34 @@
     frame = get_frame(3)
     name = frame.f_globals["__name__"]
     if name:
         record["name"] = name
 
 
 def eval_args(record):
-    eval_args = []
     args = record.get("args", [])
+    record["args"] = eval_list(args)
+
+
+def eval_kwargs(record):
+    kwargs = record.get("kwargs", {})
+    eval_dict(kwargs)
+
+
+def eval_lambda(record):
+    args = record.get("args", [])
+    record["args"] = eval_lambda_list(args)
+
     kwargs = record.get("kwargs", {})
-    for arg in args:
-        if callable(arg):
-            with contextlib.suppress(Exception):
-                arg_result = arg()
-                eval_args.append(arg_result)
-                func_name = arg.__name__
-                if func_name != "<lambda>" and func_name not in kwargs:
-                    kwargs[func_name] = arg_result
-        else:
-            eval_args.append(arg)
-    record["args"] = eval_args
+    eval_lambda_dict(kwargs)
+
+
+def eval_extra(record):
+    extra = record.get("extra", {})
+    eval_lambda_dict(extra)
 
 
 def preprocess_exc_info(record):
     kwargs = record.get("kwargs", {})
     exc_info = kwargs.pop("exc_info", False)
     if exc_info:
         type_, value, traceback = sys.exc_info()
@@ -90,20 +106,23 @@
     context = record.get("context", {})
     if context:
         extra = record.get("extra", {})
         extra.update(context)
 
 
 def preformat_message(record):
+    preformatted = record.get("preformatted", False)
+    if preformatted:
+        return
     msg = record.get("msg", "")
     args = record.get("args", [])
     kwargs = record.get("kwargs", {})
     if msg and (args or kwargs):
         with contextlib.suppress(Exception):
-            record["message"] = msg.format(*args, **kwargs)
+            record["message"] = eval_format(msg, args, kwargs)
             record["preformatted"] = True
 
 
 def remove_items(*args):
     def remover(record):
         for arg in args:
             arg = str(arg)
@@ -231,10 +250,15 @@
                 # kwargs["duration_key"] = stop
                 kwargs["duration"] = duration
                 if not message and self._add_message:
                     message = f"Stop {stop!r}. Duration: {duration:.6f} seconds."
                     record["message"] = message
 
 
+def elapsed(record):
+    record["elapsed"] = datetime.now(timezone.utc) - start_time
+
+
 # defaults used for core configuration
 DEFAULT_PREPROCESSORS = (preprocess_exc_info,)
-DEFAULT_PROCESSORS = (eval_args, context_to_extra, kwargs_to_extra, preformat_message)
+# DEFAULT_PROCESSORS = (eval_lambda, context_to_extra, kwargs_to_extra, preformat_message)
+DEFAULT_PROCESSORS = (context_to_extra, kwargs_to_extra, eval_extra)
```

### Comparing `plainlog-0.1.1/src/plainlog/warnings.py` & `plainlog-0.1.3/src/plainlog/warnings.py`

 * *Files identical despite different names*

### Comparing `plainlog-0.1.1/src/plainlog_extensions/_rich_handler.py` & `plainlog-0.1.3/scripts/plainlog_extensions/_rich_handler.py`

 * *Files identical despite different names*

### Comparing `plainlog-0.1.1/tests/conftest.py` & `plainlog-0.1.3/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,32 +15,48 @@
 #         )
 #         plainlog._logger.context.set({})
 
 #     reset()
 #     yield
 #     reset()
 
+class DummyHandler:
+
+    def __init__(self):
+        self._records = []
+
+    def __call__(self, record):
+        self._records.append(record)
+
+    @property
+    def records(self):
+        plainlog.logger_core.wait_for_processed() 
+        return self._records
+        
+
+    def first(self):
+        plainlog.logger_core.wait_for_processed()
+        return self._records[0]
+
+    def clear(self):
+        self._records.clear()
+
 
 @pytest.fixture
-def writer():
-    records = []
-    
-    def w(record):
-        records.append(record)
-
-    w.records = records
-    w.first = lambda: records[0]
-    w.clear = lambda: records.clear()
+def thandler():
+    dh = DummyHandler()
+    name = "testhandler"
 
-    plainlog.logger_core.add(w, name="writer")
+    plainlog.logger_core.configure(handlers=[dict(handler=dh, name=name)])
+    #plainlog.logger_core.add(dh, name="writer")
 
-    yield w
+    yield dh
 
-    plainlog.logger_core.remove("writer")
-    del records
+    plainlog.logger_core.remove(name)
+    dh.clear()
 
 
 @contextlib.contextmanager
 def make_logging_logger(name, handler, fmt="%(message)s", level="DEBUG"):
     logging_logger = logging.getLogger(name)
     logging_logger.setLevel(level)
     formatter = logging.Formatter(fmt)
```

### Comparing `plainlog-0.1.1/tests/test_bind.py` & `plainlog-0.1.3/tests/test_bind.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,64 @@
 import pytest
 
 from plainlog import logger, logger_core
 
 
-def test_bind_after_add(writer):
-    logger_core.add(writer)
+def test_bind_after_add(thandler):
     logger_bound = logger.bind(a=0)
     logger_bound.debug("A")
-    logger_core.wait_for_processed()
 
-    record = writer.first()
+    record = thandler.first()
 
     assert record["extra"].get("a") == 0
     assert record["msg"] == "A"
 
 
-def test_bind_before_add(writer):
+def test_bind_before_add(thandler):
     logger_bound = logger.bind(a=0)
-    logger_core.add(writer)
     logger_bound.debug("A")
-    logger_core.wait_for_processed()
 
-    record = writer.first()
+    record = thandler.first()
 
     assert record["extra"].get("a") == 0
     assert record["msg"] == "A"
 
 
-def test_add_using_bound(writer):
+def test_add_using_bound(thandler):
     logger_core.configure(extra={"a": -1})
     logger_bound = logger.bind(a=0)
-    logger_core.add(writer)
     logger.debug("A")
     logger_bound.debug("B")
-    logger_core.wait_for_processed()
 
-    record = writer.records[0]
+    assert thandler.records
+
+    record = thandler.records[0]
 
     assert record["extra"].get("a") == -1
     assert record["msg"] == "A"
     
-    record = writer.records[1]
+    record = thandler.records[1]
+
+    assert record["extra"].get("a") == 0
+    assert record["msg"] == "B"
 
+
+def test_unbind(thandler):
+    lb = logger.bind(a=0)
+    lb.debug("A")
+    lb = lb.unbind("a")
+    lb.debug("B")
+    
+    assert thandler.records
+    record = thandler.records[0]
     assert record["extra"].get("a") == 0
+    assert record["msg"] == "A"
+    
+    record = thandler.records[1]
+    assert record["extra"].get("a") == None
     assert record["msg"] == "B"
 
 
 # def test_not_override_parent_logger(writer):
 #     logger_1 = logger.bind(a="a")
 #     logger_2 = logger_1.bind(a="A")
 #     logger.add(writer, format="{extra[a]} {message}")
```

### Comparing `plainlog-0.1.1/.gitignore` & `plainlog-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `plainlog-0.1.1/README.md` & `plainlog-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `plainlog-0.1.1/pyproject.toml` & `plainlog-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -74,21 +74,31 @@
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
+[tool.coverage.paths]
+source = ["src"]
+
 
 [tool.pytest.ini_options]
 pythonpath = ["src"]
 testpaths = ["tests"]
 
 [tool.black]
 line-length = 100
+extend-exclude = '''
+/(
+  | .env
+  | .venv
+  | venv
+)/
+'''
 
 [tool.ruff]
 select = [
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
     "F",  # pyflakes
     # "I",  # isort
@@ -96,7 +106,9 @@
     "B",  # flake8-bugbear
 ]
 ignore = [
     "E501",  # line too long, handled by black
     "B008",  # do not perform function calls in argument defaults
     "C901",  # too complex
 ]
+exclude = [".env", ".venv", "venv"]
+#show-source = true
```

### Comparing `plainlog-0.1.1/LICENSES/Apache-2.0.txt` & `plainlog-0.1.3/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `plainlog-0.1.1/LICENSES/MIT.txt` & `plainlog-0.1.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `plainlog-0.1.1/PKG-INFO` & `plainlog-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plainlog
-Version: 0.1.1
+Version: 0.1.3
 Summary: Logging made simple and easy.
 Project-URL: Documentation, https://github.com/tds333/plainlog#readme
 Project-URL: Issues, https://github.com/tds333/plainlog/issues
 Project-URL: Source, https://github.com/tds333/plainlog
 Author-email: Wolfgang Langner <tds333@mailbox.org>
 License-Expression: Apache-2.0 OR MIT
 License-File: LICENSES/Apache-2.0.txt
```

