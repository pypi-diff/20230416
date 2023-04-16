# Comparing `tmp/aiomonitor-ng-0.7.0.tar.gz` & `tmp/aiomonitor-ng-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiomonitor-ng-0.7.0.tar", last modified: Wed Oct 19 08:30:18 2022, max compression
+gzip compressed data, was "aiomonitor-ng-0.7.1.tar", last modified: Sun Apr 16 12:14:52 2023, max compression
```

## Comparing `aiomonitor-ng-0.7.0.tar` & `aiomonitor-ng-0.7.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 joongi     (501) staff       (20)        0 2022-10-19 08:30:18.077906 aiomonitor-ng-0.7.0/
--rw-r--r--   0 joongi     (501) staff       (20)     2667 2022-10-19 08:29:32.000000 aiomonitor-ng-0.7.0/CHANGES.txt
--rw-r--r--   0 joongi     (501) staff       (20)    11311 2022-08-25 07:44:15.000000 aiomonitor-ng-0.7.0/LICENSE
--rw-r--r--   0 joongi     (501) staff       (20)       99 2022-08-25 07:44:15.000000 aiomonitor-ng-0.7.0/MANIFEST.in
--rw-r--r--   0 joongi     (501) staff       (20)     8980 2022-10-19 08:30:18.077667 aiomonitor-ng-0.7.0/PKG-INFO
--rw-r--r--   0 joongi     (501) staff       (20)     5530 2022-09-26 08:49:08.000000 aiomonitor-ng-0.7.0/README.rst
-drwxr-xr-x   0 joongi     (501) staff       (20)        0 2022-10-19 08:30:18.076787 aiomonitor-ng-0.7.0/aiomonitor/
--rw-r--r--   0 joongi     (501) staff       (20)      822 2022-10-19 08:29:43.000000 aiomonitor-ng-0.7.0/aiomonitor/__init__.py
--rw-r--r--   0 joongi     (501) staff       (20)      955 2022-09-23 09:34:54.000000 aiomonitor-ng-0.7.0/aiomonitor/cli.py
--rw-r--r--   0 joongi     (501) staff       (20)     4818 2022-09-25 16:39:01.000000 aiomonitor-ng-0.7.0/aiomonitor/console.py
--rw-r--r--   0 joongi     (501) staff       (20)    30953 2022-10-19 08:27:30.000000 aiomonitor-ng-0.7.0/aiomonitor/monitor.py
--rw-r--r--   0 joongi     (501) staff       (20)     3499 2022-10-19 08:27:30.000000 aiomonitor-ng-0.7.0/aiomonitor/task.py
--rw-r--r--   0 joongi     (501) staff       (20)     9250 2022-09-25 16:39:01.000000 aiomonitor-ng-0.7.0/aiomonitor/telnet.py
--rw-r--r--   0 joongi     (501) staff       (20)      556 2022-10-19 08:27:30.000000 aiomonitor-ng-0.7.0/aiomonitor/types.py
--rw-r--r--   0 joongi     (501) staff       (20)     7894 2022-10-19 08:27:30.000000 aiomonitor-ng-0.7.0/aiomonitor/utils.py
-drwxr-xr-x   0 joongi     (501) staff       (20)        0 2022-10-19 08:30:18.077482 aiomonitor-ng-0.7.0/aiomonitor_ng.egg-info/
--rw-r--r--   0 joongi     (501) staff       (20)     8980 2022-10-19 08:30:18.000000 aiomonitor-ng-0.7.0/aiomonitor_ng.egg-info/PKG-INFO
--rw-r--r--   0 joongi     (501) staff       (20)      415 2022-10-19 08:30:18.000000 aiomonitor-ng-0.7.0/aiomonitor_ng.egg-info/SOURCES.txt
--rw-r--r--   0 joongi     (501) staff       (20)        1 2022-10-19 08:30:18.000000 aiomonitor-ng-0.7.0/aiomonitor_ng.egg-info/dependency_links.txt
--rw-r--r--   0 joongi     (501) staff       (20)       99 2022-10-19 08:30:18.000000 aiomonitor-ng-0.7.0/aiomonitor_ng.egg-info/requires.txt
--rw-r--r--   0 joongi     (501) staff       (20)       11 2022-10-19 08:30:18.000000 aiomonitor-ng-0.7.0/aiomonitor_ng.egg-info/top_level.txt
--rw-r--r--   0 joongi     (501) staff       (20)      122 2022-09-23 09:34:54.000000 aiomonitor-ng-0.7.0/pyproject.toml
--rw-r--r--   0 joongi     (501) staff       (20)       38 2022-10-19 08:30:18.077942 aiomonitor-ng-0.7.0/setup.cfg
--rw-r--r--   0 joongi     (501) staff       (20)     1991 2022-10-19 08:27:30.000000 aiomonitor-ng-0.7.0/setup.py
+drwxr-xr-x   0 joongi     (501) staff       (20)        0 2023-04-16 12:14:52.192699 aiomonitor-ng-0.7.1/
+-rw-r--r--   0 joongi     (501) staff       (20)    11311 2022-08-25 07:44:15.000000 aiomonitor-ng-0.7.1/LICENSE
+-rw-r--r--   0 joongi     (501) staff       (20)       99 2022-08-25 07:44:15.000000 aiomonitor-ng-0.7.1/MANIFEST.in
+-rw-r--r--   0 joongi     (501) staff       (20)     9393 2023-04-16 12:14:52.192547 aiomonitor-ng-0.7.1/PKG-INFO
+-rw-r--r--   0 joongi     (501) staff       (20)     5706 2022-10-19 08:55:38.000000 aiomonitor-ng-0.7.1/README.rst
+drwxr-xr-x   0 joongi     (501) staff       (20)        0 2023-04-16 12:14:52.191676 aiomonitor-ng-0.7.1/aiomonitor/
+-rw-r--r--   0 joongi     (501) staff       (20)      822 2023-04-16 12:11:12.000000 aiomonitor-ng-0.7.1/aiomonitor/__init__.py
+-rw-r--r--   0 joongi     (501) staff       (20)      955 2022-09-23 09:34:54.000000 aiomonitor-ng-0.7.1/aiomonitor/cli.py
+-rw-r--r--   0 joongi     (501) staff       (20)     4818 2022-09-25 16:39:01.000000 aiomonitor-ng-0.7.1/aiomonitor/console.py
+-rw-r--r--   0 joongi     (501) staff       (20)    31248 2023-04-16 08:39:53.000000 aiomonitor-ng-0.7.1/aiomonitor/monitor.py
+-rw-r--r--   0 joongi     (501) staff       (20)     3488 2022-10-19 09:10:28.000000 aiomonitor-ng-0.7.1/aiomonitor/task.py
+-rw-r--r--   0 joongi     (501) staff       (20)     9250 2022-09-25 16:39:01.000000 aiomonitor-ng-0.7.1/aiomonitor/telnet.py
+-rw-r--r--   0 joongi     (501) staff       (20)      556 2022-10-19 08:27:30.000000 aiomonitor-ng-0.7.1/aiomonitor/types.py
+-rw-r--r--   0 joongi     (501) staff       (20)     7894 2022-10-19 08:27:30.000000 aiomonitor-ng-0.7.1/aiomonitor/utils.py
+drwxr-xr-x   0 joongi     (501) staff       (20)        0 2023-04-16 12:14:52.192247 aiomonitor-ng-0.7.1/aiomonitor_ng.egg-info/
+-rw-r--r--   0 joongi     (501) staff       (20)     9393 2023-04-16 12:14:52.000000 aiomonitor-ng-0.7.1/aiomonitor_ng.egg-info/PKG-INFO
+-rw-r--r--   0 joongi     (501) staff       (20)      425 2023-04-16 12:14:52.000000 aiomonitor-ng-0.7.1/aiomonitor_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 joongi     (501) staff       (20)        1 2023-04-16 12:14:52.000000 aiomonitor-ng-0.7.1/aiomonitor_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 joongi     (501) staff       (20)       99 2023-04-16 12:14:52.000000 aiomonitor-ng-0.7.1/aiomonitor_ng.egg-info/requires.txt
+-rw-r--r--   0 joongi     (501) staff       (20)       11 2023-04-16 12:14:52.000000 aiomonitor-ng-0.7.1/aiomonitor_ng.egg-info/top_level.txt
+-rw-r--r--   0 joongi     (501) staff       (20)      122 2022-09-23 09:34:54.000000 aiomonitor-ng-0.7.1/pyproject.toml
+-rw-r--r--   0 joongi     (501) staff       (20)       38 2023-04-16 12:14:52.192735 aiomonitor-ng-0.7.1/setup.cfg
+-rw-r--r--   0 joongi     (501) staff       (20)     1991 2022-10-19 09:00:47.000000 aiomonitor-ng-0.7.1/setup.py
+drwxr-xr-x   0 joongi     (501) staff       (20)        0 2023-04-16 12:14:52.192366 aiomonitor-ng-0.7.1/tests/
+-rw-r--r--   0 joongi     (501) staff       (20)     5676 2023-04-16 08:39:53.000000 aiomonitor-ng-0.7.1/tests/test_monitor.py
```

### Comparing `aiomonitor-ng-0.7.0/LICENSE` & `aiomonitor-ng-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiomonitor-ng-0.7.0/PKG-INFO` & `aiomonitor-ng-0.7.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiomonitor-ng
-Version: 0.7.0
+Version: 0.7.1
 Summary: aiomonitor-ng adds monitor and python REPL capabilities for asyncio application
 Home-page: https://github.com/achimnol/aiomonitor-ng
 Download-URL: https://pypi.python.org/pypi/aiomonitor-ng
 Author: Nikolay Novik
 Author-email: nickolainovik@gmail.com
 License: Apache 2
 Platform: POSIX
@@ -125,22 +125,24 @@
 
     monitor >>> help
     Usage: help [OPTIONS] COMMAND [ARGS]...
     
       To see the usage of each command, run them with "--help" option.
     
     Commands:
-      cancel                 Cancel an indicated task
-      console                Switch to async Python REPL
-      exit (q,quit)          Leave the monitor client session
-      help (?,h)             Show the list of commands
-      ps (p)                 Show task table
-      signal                 Send a Unix signal
-      stacktrace (st,stack)  Print a stack trace from the event loop thread
-      where (w)              Show stack frames and its task creation chain of a task
+      cancel                  Cancel an indicated task
+      console                 Switch to async Python REPL
+      exit (q,quit)           Leave the monitor client session
+      help (?,h)              Show the list of commands
+      ps (p)                  Show task table
+      ps-terminated (pst,pt)  List recently terminated/cancelled tasks
+      signal                  Send a Unix signal
+      stacktrace (st,stack)   Print a stack trace from the event loop thread
+      where (w)               Show stack frames and the task creation chain of a task
+      where-terminated (wt)   Show stack frames and the termination/cancellation chain of a task
 
 ``aiomonitor`` also supports async python console inside a running event loop
 so you can explore the state of your application::
 
     monitor >>> console
     Python 3.10.7 (main, Sep  9 2022, 12:31:20) [Clang 13.1.6 (clang-1316.0.21.2.5)] on darwin
     Type "help", "copyright", "credits" or "license" for more information.
@@ -195,14 +197,22 @@
 .. _prompt_toolkit: https://python-prompt-toolkit.readthedocs.io
 .. _uvloop: https://github.com/MagicStack/uvloop
 .. _cmd: http://docs.python.org/3/library/cmd.html
 
 CHANGES
 =======
 
+0.7.1 (2023-04-16)
+------------------
+
+* Support Python 3.11 properly by allowing the optional `name` and `context` kwargs passed to `asyncio.create_task()` in the hooked task factory function (#10)
+
+* Update development dependencies
+
+
 0.7.0 (2022-10-19)
 ------------------
 
 * Selective persistent termination logs (#9)
 
 * Implement cancellation chain tracker (#8)
 
@@ -230,14 +240,15 @@
 
 
 0.5.1 (2022-08-29)
 ------------------
 
 * Fix the task creation location in the 'ps' command output
 
+
 0.5.0 (2022-08-26)
 ------------------
 
 * Made it compatible with Python 3.10
 
 * Added the task creation stack chain display to the 'where' command by setting a custom task factory (#1)
```

### Comparing `aiomonitor-ng-0.7.0/README.rst` & `aiomonitor-ng-0.7.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -104,22 +104,24 @@
 
     monitor >>> help
     Usage: help [OPTIONS] COMMAND [ARGS]...
     
       To see the usage of each command, run them with "--help" option.
     
     Commands:
-      cancel                 Cancel an indicated task
-      console                Switch to async Python REPL
-      exit (q,quit)          Leave the monitor client session
-      help (?,h)             Show the list of commands
-      ps (p)                 Show task table
-      signal                 Send a Unix signal
-      stacktrace (st,stack)  Print a stack trace from the event loop thread
-      where (w)              Show stack frames and its task creation chain of a task
+      cancel                  Cancel an indicated task
+      console                 Switch to async Python REPL
+      exit (q,quit)           Leave the monitor client session
+      help (?,h)              Show the list of commands
+      ps (p)                  Show task table
+      ps-terminated (pst,pt)  List recently terminated/cancelled tasks
+      signal                  Send a Unix signal
+      stacktrace (st,stack)   Print a stack trace from the event loop thread
+      where (w)               Show stack frames and the task creation chain of a task
+      where-terminated (wt)   Show stack frames and the termination/cancellation chain of a task
 
 ``aiomonitor`` also supports async python console inside a running event loop
 so you can explore the state of your application::
 
     monitor >>> console
     Python 3.10.7 (main, Sep  9 2022, 12:31:20) [Clang 13.1.6 (clang-1316.0.21.2.5)] on darwin
     Type "help", "copyright", "credits" or "license" for more information.
```

### Comparing `aiomonitor-ng-0.7.0/aiomonitor/__init__.py` & `aiomonitor-ng-0.7.1/aiomonitor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,8 +33,8 @@
     "Monitor",
     "monitor_cli",
     "start_monitor",
     "MONITOR_HOST",
     "MONITOR_PORT",
     "CONSOLE_PORT",
 )
-__version__ = "0.7.0"
+__version__ = "0.7.1"
```

### Comparing `aiomonitor-ng-0.7.0/aiomonitor/cli.py` & `aiomonitor-ng-0.7.1/aiomonitor/cli.py`

 * *Files identical despite different names*

### Comparing `aiomonitor-ng-0.7.0/aiomonitor/console.py` & `aiomonitor-ng-0.7.1/aiomonitor/console.py`

 * *Files identical despite different names*

### Comparing `aiomonitor-ng-0.7.0/aiomonitor/monitor.py` & `aiomonitor-ng-0.7.1/aiomonitor/monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import asyncio
+import contextvars
 import functools
 import logging
 import os
 import shlex
 import signal
 import sys
 import threading
@@ -14,24 +15,26 @@
 from asyncio.coroutines import _format_coroutine  # type: ignore
 from contextvars import ContextVar, copy_context
 from datetime import timedelta
 from types import TracebackType
 from typing import (
     Any,
     Awaitable,
+    Coroutine,
     Dict,
     Final,
     Generator,
     Iterable,
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
+    cast,
 )
 
 import click
 import janus
 from click.parser import split_arg_string
 from click.shell_completion import CompletionItem, _resolve_context, _resolve_incomplete
 from prompt_toolkit import PromptSession
@@ -311,30 +314,35 @@
         except BaseException as e:
             myself._termination_stack = _extract_stack_from_exception(e)[:-1]
             raise
 
     def _create_task(
         self,
         loop: asyncio.AbstractEventLoop,
-        coro: Generator[Any, Any, T_co],
+        coro: Coroutine[Any, Any, T_co] | Generator[Any, None, T_co],
+        *,
+        name: str | None = None,
+        context: contextvars.Context | None = None,
     ) -> asyncio.Future[T_co]:
         assert loop is self._monitored_loop
         try:
             parent_task = asyncio.current_task()
         except RuntimeError:
             parent_task = None
         persistent = coro in persistent_coro
         task = TracedTask(
             self._coro_wrapper(coro),  # type: ignore
             termination_info_queue=self._termination_info_queue.sync_q,
             cancellation_chain_queue=self._cancellation_chain_queue.sync_q,
             persistent=persistent,
             loop=self._monitored_loop,
+            name=name,  # since Python 3.8
+            context=context,  # since Python 3.11
         )
-        task._orig_coro = coro
+        task._orig_coro = cast(Coroutine[Any, Any, T_co], coro)
         self._created_tracebacks[task] = _extract_stack_from_frame(sys._getframe())[
             :-1
         ]  # strip this wrapper method
         if parent_task is not None:
             self._created_traceback_chains[task] = weakref.ref(parent_task)
         return task
```

### Comparing `aiomonitor-ng-0.7.0/aiomonitor/task.py` & `aiomonitor-ng-0.7.1/aiomonitor/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import functools
 import struct
 import sys
 import time
 import traceback
 import weakref
 from asyncio.coroutines import _format_coroutine  # type: ignore
-from typing import Any, Callable, Coroutine, Generator, List, Optional, TypeVar
+from typing import Any, Callable, Coroutine, List, Optional, TypeVar
 
 import janus
 from typing_extensions import ParamSpec
 
 from .types import CancellationChain, TerminatedTaskInfo
 from .utils import _extract_stack_from_frame
 
@@ -24,15 +24,15 @@
 persistent_coro: weakref.WeakSet[Coroutine] = weakref.WeakSet()
 
 T = TypeVar("T")
 P = ParamSpec("P")
 
 
 class TracedTask(asyncio.Task):
-    _orig_coro: Generator[Any, Any, Any]
+    _orig_coro: Coroutine[Any, Any, Any]
     _termination_stack: Optional[List[traceback.FrameSummary]]
 
     def __init__(
         self,
         *args,
         termination_info_queue: janus._SyncQueueProxy[TerminatedTaskInfo],
         cancellation_chain_queue: janus._SyncQueueProxy[CancellationChain],
```

### Comparing `aiomonitor-ng-0.7.0/aiomonitor/telnet.py` & `aiomonitor-ng-0.7.1/aiomonitor/telnet.py`

 * *Files identical despite different names*

### Comparing `aiomonitor-ng-0.7.0/aiomonitor/types.py` & `aiomonitor-ng-0.7.1/aiomonitor/types.py`

 * *Files identical despite different names*

### Comparing `aiomonitor-ng-0.7.0/aiomonitor/utils.py` & `aiomonitor-ng-0.7.1/aiomonitor/utils.py`

 * *Files identical despite different names*

### Comparing `aiomonitor-ng-0.7.0/aiomonitor_ng.egg-info/PKG-INFO` & `aiomonitor-ng-0.7.1/aiomonitor_ng.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiomonitor-ng
-Version: 0.7.0
+Version: 0.7.1
 Summary: aiomonitor-ng adds monitor and python REPL capabilities for asyncio application
 Home-page: https://github.com/achimnol/aiomonitor-ng
 Download-URL: https://pypi.python.org/pypi/aiomonitor-ng
 Author: Nikolay Novik
 Author-email: nickolainovik@gmail.com
 License: Apache 2
 Platform: POSIX
@@ -125,22 +125,24 @@
 
     monitor >>> help
     Usage: help [OPTIONS] COMMAND [ARGS]...
     
       To see the usage of each command, run them with "--help" option.
     
     Commands:
-      cancel                 Cancel an indicated task
-      console                Switch to async Python REPL
-      exit (q,quit)          Leave the monitor client session
-      help (?,h)             Show the list of commands
-      ps (p)                 Show task table
-      signal                 Send a Unix signal
-      stacktrace (st,stack)  Print a stack trace from the event loop thread
-      where (w)              Show stack frames and its task creation chain of a task
+      cancel                  Cancel an indicated task
+      console                 Switch to async Python REPL
+      exit (q,quit)           Leave the monitor client session
+      help (?,h)              Show the list of commands
+      ps (p)                  Show task table
+      ps-terminated (pst,pt)  List recently terminated/cancelled tasks
+      signal                  Send a Unix signal
+      stacktrace (st,stack)   Print a stack trace from the event loop thread
+      where (w)               Show stack frames and the task creation chain of a task
+      where-terminated (wt)   Show stack frames and the termination/cancellation chain of a task
 
 ``aiomonitor`` also supports async python console inside a running event loop
 so you can explore the state of your application::
 
     monitor >>> console
     Python 3.10.7 (main, Sep  9 2022, 12:31:20) [Clang 13.1.6 (clang-1316.0.21.2.5)] on darwin
     Type "help", "copyright", "credits" or "license" for more information.
@@ -195,14 +197,22 @@
 .. _prompt_toolkit: https://python-prompt-toolkit.readthedocs.io
 .. _uvloop: https://github.com/MagicStack/uvloop
 .. _cmd: http://docs.python.org/3/library/cmd.html
 
 CHANGES
 =======
 
+0.7.1 (2023-04-16)
+------------------
+
+* Support Python 3.11 properly by allowing the optional `name` and `context` kwargs passed to `asyncio.create_task()` in the hooked task factory function (#10)
+
+* Update development dependencies
+
+
 0.7.0 (2022-10-19)
 ------------------
 
 * Selective persistent termination logs (#9)
 
 * Implement cancellation chain tracker (#8)
 
@@ -230,14 +240,15 @@
 
 
 0.5.1 (2022-08-29)
 ------------------
 
 * Fix the task creation location in the 'ps' command output
 
+
 0.5.0 (2022-08-26)
 ------------------
 
 * Made it compatible with Python 3.10
 
 * Added the task creation stack chain display to the 'where' command by setting a custom task factory (#1)
```

### Comparing `aiomonitor-ng-0.7.0/setup.py` & `aiomonitor-ng-0.7.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 setup(
     name="aiomonitor-ng",
     version=read_version(),
     description=(
         "aiomonitor-ng adds monitor and python REPL "
         "capabilities for asyncio application"
     ),
-    long_description="\n\n".join((read("README.rst"), read("CHANGES.txt"))),
+    long_description="\n\n".join((read("README.rst"), read("CHANGES.rst"))),
     classifiers=classifiers,
     platforms=["POSIX"],
     author="Nikolay Novik",
     author_email="nickolainovik@gmail.com",
     url="https://github.com/achimnol/aiomonitor-ng",
     download_url="https://pypi.python.org/pypi/aiomonitor-ng",
     license="Apache 2",
```

