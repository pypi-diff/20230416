# Comparing `tmp/stress_injector-0.5-py3-none-any.whl.zip` & `tmp/stress_injector-0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 13033 bytes, number of entries: 12
--rw-r--r--  2.0 unx      248 b- defN 23-Apr-16 17:33 stressinjector/__init__.py
--rw-r--r--  2.0 unx     4788 b- defN 23-Apr-16 17:33 stressinjector/cpu.py
--rw-r--r--  2.0 unx     2997 b- defN 23-Apr-16 17:33 stressinjector/echo.py
--rw-r--r--  2.0 unx     4586 b- defN 23-Apr-16 17:33 stressinjector/memory.py
--rw-r--r--  2.0 unx     1285 b- defN 23-Apr-16 17:33 stressinjector/models.py
--rw-r--r--  2.0 unx       49 b- defN 23-Apr-16 17:33 stressinjector/requirements.txt
--rw-r--r--  2.0 unx     5442 b- defN 23-Apr-16 17:33 stressinjector/url.py
--rw-r--r--  2.0 unx     1078 b- defN 23-Apr-16 17:34 stress_injector-0.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     8520 b- defN 23-Apr-16 17:34 stress_injector-0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-16 17:34 stress_injector-0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Apr-16 17:34 stress_injector-0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      981 b- defN 23-Apr-16 17:34 stress_injector-0.5.dist-info/RECORD
-12 files, 30081 bytes uncompressed, 11383 bytes compressed:  62.2%
+Zip file size: 12735 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      248 b- defN 23-Apr-16 19:29 stressinjector/__init__.py
+-rw-r--r--  2.0 unx     4968 b- defN 23-Apr-16 19:29 stressinjector/cpu.py
+-rw-r--r--  2.0 unx      614 b- defN 23-Apr-16 19:29 stressinjector/helper.py
+-rw-r--r--  2.0 unx     4832 b- defN 23-Apr-16 19:29 stressinjector/memory.py
+-rw-r--r--  2.0 unx     1388 b- defN 23-Apr-16 19:29 stressinjector/models.py
+-rw-r--r--  2.0 unx       49 b- defN 23-Apr-16 19:29 stressinjector/requirements.txt
+-rw-r--r--  2.0 unx     5495 b- defN 23-Apr-16 19:29 stressinjector/url.py
+-rw-r--r--  2.0 unx     1078 b- defN 23-Apr-16 19:29 stress_injector-0.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8973 b- defN 23-Apr-16 19:29 stress_injector-0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-16 19:29 stress_injector-0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Apr-16 19:29 stress_injector-0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      982 b- defN 23-Apr-16 19:29 stress_injector-0.7.dist-info/RECORD
+12 files, 28734 bytes uncompressed, 11081 bytes compressed:  61.4%
```

## zipnote {}

```diff
@@ -1,37 +1,37 @@
 Filename: stressinjector/__init__.py
 Comment: 
 
 Filename: stressinjector/cpu.py
 Comment: 
 
-Filename: stressinjector/echo.py
+Filename: stressinjector/helper.py
 Comment: 
 
 Filename: stressinjector/memory.py
 Comment: 
 
 Filename: stressinjector/models.py
 Comment: 
 
 Filename: stressinjector/requirements.txt
 Comment: 
 
 Filename: stressinjector/url.py
 Comment: 
 
-Filename: stress_injector-0.5.dist-info/LICENSE
+Filename: stress_injector-0.7.dist-info/LICENSE
 Comment: 
 
-Filename: stress_injector-0.5.dist-info/METADATA
+Filename: stress_injector-0.7.dist-info/METADATA
 Comment: 
 
-Filename: stress_injector-0.5.dist-info/WHEEL
+Filename: stress_injector-0.7.dist-info/WHEEL
 Comment: 
 
-Filename: stress_injector-0.5.dist-info/top_level.txt
+Filename: stress_injector-0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: stress_injector-0.5.dist-info/RECORD
+Filename: stress_injector-0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## stressinjector/__init__.py

```diff
@@ -1,6 +1,6 @@
 from stressinjector.cpu import CPUStress  # noqa: F401
 from stressinjector.memory import MemoryStress  # noqa: F401
 from stressinjector.models import RequestType  # noqa: F401
 from stressinjector.url import URLStress  # noqa: F401
 
-version = "0.5"
+version = "0.7"
```

## stressinjector/cpu.py

```diff
@@ -1,46 +1,50 @@
+import logging
 import os
-import sys
 import time
 from multiprocessing import Process
 from threading import Thread
 from typing import List
 
 import psutil
 
-from .echo import echo
+from .helper import flush_screen, write_screen
+from .models import LOGGER
 
 
 class CPUStress:
     """`Controller <https://git.io/J9cXV>`__ for CPU stress using multiprocessing. Gets duration as user input.
 
     >>> CPUStress
 
     CPU is stressed using `multiprocessing.Process <https://docs.python.org/3/library/multiprocessing.html#
     the-process-class>`__ to run the infinite loop on each process.
 
-    Args:
-        seconds:
-            - The number of seconds for which the CPU has to be stressed. Defaults to five times the number of cores.
-
     Warnings:
         - CPU stress is induced in real time.
         - A relatively low performing machine may stall when stress is induced for a long duration.
 
     References:
         >>> CPUStress._infinite()
             Triggers an infinite loop for the number of logical cores.
 
         >>> CPUStress._measure_cpu()
             Measures the impact on each logical core in a dedicated thread.
     """
 
     CORES = os.cpu_count()
 
-    def __init__(self, seconds: int = CORES * 5):
+    def __init__(self, seconds: int = CORES * 5, logger: logging.Logger = None):
+        """Instantiates the members of the class.
+
+        Args:
+            seconds: The number of seconds CPU has to be stressed. Defaults to five times the number of cores.
+            logger: Custom logger.
+        """
+        self.LOGGER = logger or LOGGER
         self.seconds = seconds
         self.start_time = None
         self._run()
 
     def _infinite(self) -> None:
         """Infinite loop to stress each core on the CPU for the number of logical cores available.
 
@@ -64,31 +68,30 @@
         processors = []
         while True:
             cpu_util: List[float] = psutil.cpu_percent(interval=1, percpu=True)  # noqa
             processors.append(cpu_util)  # stores the list of usage % as a list within a list
             output = ''
             for index, percent in enumerate(cpu_util):
                 output += f'Core {index + 1}: {percent}%\t'
-            sys.stdout.write(f'\r{output.strip()}')
+            write_screen(output.strip())
             if stop_thread:
                 break
-        sys.stdout.flush()
-        sys.stdout.write('\r')
+        flush_screen()
         processors = map(list, zip(*processors))
         processors = [max(processor) for processor in processors]
         processors = list(enumerate(processors))
         processors = sorted(processors, key=lambda x: x[1], reverse=True)
 
         if self.start_time and (run_time := round(time.time() - self.start_time)):
             if (stop_when := self.seconds - run_time) and stop_when > 0:
-                echo.warning(f'Actual runtime: {run_time} seconds. Stopped {stop_when} seconds early.')
+                self.LOGGER.warning('Actual runtime: %d seconds. Stopped %d seconds early.', run_time, stop_when)
         else:
-            echo.warning('Stress Test was stopped before it began.')
+            self.LOGGER.warning('Stress Test was stopped before it began.')
 
-        echo.info('CPU Usage Report:')
+        self.LOGGER.info('CPU Usage Report:')
         [print(f'Core {processor + 1} - {self._format_number(usage)}%') for processor, usage in processors]
 
     @classmethod
     def _format_number(cls, n: float) -> int:
         """Converts numbers with float value .0 to integers.
 
         Args:
@@ -106,15 +109,15 @@
         Methods:
             infinite: To kick off stress injector.
             measure: To measure the usage in the background running in a dedicated thread.
         """
         # noinspection PyGlobalUndefined
         global stop_thread
         try:
-            sys.stdout.write(f'\rStressing CPU cores for {self.seconds} seconds')
+            self.LOGGER.info('Stressing CPU cores for %d seconds', self.seconds)
             processes = []
             for n in range(self.CORES):
                 processes.append(Process(target=self._infinite))
             stop_thread = False
             measure = Thread(target=self._measure_cpu)
             measure.start()
             time.sleep(1)
@@ -123,9 +126,9 @@
             time.sleep(self.seconds)
             [each_core.terminate() for each_core in processes]
             [each_core.join() for each_core in processes]
             time.sleep(1)
             stop_thread = True
             measure.join()
         except KeyboardInterrupt:
-            sys.stdout.write('\rManual interrupt received. Stopping stress.')
+            self.LOGGER.warning('Manual interrupt received. Stopping stress.')
             stop_thread = True
```

## stressinjector/memory.py

```diff
@@ -1,19 +1,19 @@
+import logging
 import math
 import resource
-import sys
 import time
 from typing import Union
 
 import psutil
 from numpy.random import bytes
 from tqdm import tqdm
 
-from .echo import echo
-from .models import operating_system, settings
+from .helper import flush_screen
+from .models import LOGGER, operating_system, settings
 
 
 def _size_converter(byte_size: Union[int, float]) -> str:
     """Gets the current memory consumed and converts it to human friendly format.
 
     Args:
         byte_size: Receives byte size as argument.
@@ -52,15 +52,22 @@
         >>> _size_converter()
 
             Converts ``bytes`` to human-readable size format.
     """
 
     MAX_DEFAULT = round(float(_size_converter(psutil.virtual_memory().total).split()[0]) * 2)
 
-    def __init__(self, gigabytes: int = MAX_DEFAULT):
+    def __init__(self, gigabytes: int = MAX_DEFAULT, logger: logging.Logger = None):
+        """Instantiates the members of the class.
+
+        Args:
+            gigabytes: The number of gigabytes, memory has to be stressed. Defaults to twice the physical memory.
+            logger: Custom logger.
+        """
+        self.LOGGER = logger or LOGGER
         self.gigabytes = gigabytes
         self._run()
 
     @classmethod
     def _stress(cls, mb: int) -> str:
         """Generates `random bytes <https://numpy.org/doc/stable/reference/random/generated/numpy.random.bytes.html>`__.
 
@@ -110,18 +117,16 @@
 
         Methods:
             stress: To kick off stress injector with the desired bytes converted from user input.
             memory_util_check: To measure the usage post completion.
         """
         megabytes = int(self.gigabytes) * 1024  # gigabytes to megabytes
         try:
-            sys.stdout.write(f'\rStressing Memory with {self.gigabytes} GB')
+            self.LOGGER.info('Stressing Memory with %d GB', self.gigabytes)
             time.sleep(1)
-            sys.stdout.flush()
-            sys.stdout.write('\r')
-            sys.stdout.write(self._stress(mb=megabytes) + '\n')
+            flush_screen()
+            self.LOGGER.info(self._stress(mb=megabytes) + '\n')
         except KeyboardInterrupt:
-            sys.stdout.write('\rManual interrupt received. Stopping stress.\n')
+            self.LOGGER.warning('Manual interrupt received. Stopping stress.')
             time.sleep(1)
-            sys.stdout.flush()
-            sys.stdout.write('\r')
-        echo.info(f'Actual memory Consumed: {_size_converter(self._memory_util_check())}')
+            flush_screen()
+        self.LOGGER.info('Actual memory Consumed: %s', _size_converter(self._memory_util_check()))
```

## stressinjector/models.py

```diff
@@ -1,10 +1,11 @@
 import logging
 import os
 import platform
+import sys
 from enum import Enum
 
 LOGGER = logging.getLogger(__name__)
 DEFAULT_LOG_FORM = '%(asctime)s - %(levelname)s - [%(processName)s:%(module)s:%(lineno)d] - %(funcName)s - %(message)s'
 DEFAULT_FORMATTER = logging.Formatter(datefmt='%b-%d-%Y %I:%M:%S %p', fmt=DEFAULT_LOG_FORM)
 HANDLER = logging.StreamHandler()
 HANDLER.setFormatter(fmt=DEFAULT_FORMATTER)
@@ -28,14 +29,18 @@
 
 
 class Settings:
     """Wrapper for settings."""
 
     pid: int = os.getpid()
     os: str = platform.system()
+    if sys.stdin.isatty():
+        interactive = True
+    else:
+        interactive = False
 
 
 settings = Settings
 
 
 class RequestType(str, Enum):
     """Wrapper for request types."""
```

## stressinjector/url.py

```diff
@@ -6,25 +6,25 @@
 from threading import Event
 from typing import NoReturn, Union
 
 import requests
 
 from .models import LOGGER, RequestType
 
-RESULT = {'success': 0, 'errors': 0}
-event = Event()
-
 
 class URLStress:
     """Controller for URL stress using threadpool. Gets url as input.
 
     >>> URLStress
 
     """
 
+    RESULT = {'success': 0, 'errors': 0}
+    EVENT = Event()
+
     def __init__(self, url: str, rate: int = 1e+5, timeout: Union[int, float] = None,
                  logger: logging.Logger = None, request_type: str = RequestType.get,
                  **kwargs):
         """Instantiate the object, parse and validate the URL.
 
         Args:
             url: URL to inject stress.
@@ -56,15 +56,15 @@
 
     def make_request(self, sample: bool = False) -> NoReturn:
         """Makes a GET request to the endpoint.
 
         Args:
             sample: Boolean flag to indicate if the request is sample.
         """
-        if event.is_set():
+        if self.EVENT.is_set():
             return
         if sample:
             response = requests.request(method=self.request_type.lower(), url=self.request_url, **self.kwargs)
         else:
             response = requests.request(method=self.request_type.lower(), url=self.request_url,
                                         timeout=self.timeout, **self.kwargs)
         if response.ok:
@@ -86,29 +86,29 @@
                 try:
                     future = executor.submit(self.make_request)
                     futures[future] = iterator
                 except RuntimeError as error:
                     self.LOGGER.error(error)
                     self.LOGGER.warning("cancelling future tasks")
                     future.cancel()
-                    event.set()
+                    self.EVENT.set()
                     total = len(futures)
-                    returned = sum(RESULT.values())
+                    returned = sum(self.RESULT.values())
                     self.LOGGER.warning("calls made: %d", f'{total:,}')
                     self.LOGGER.warning("calls completed: %d", f'{returned:,}')
                     self.LOGGER.warning("calls pending: %d", f'{total - returned:,}')
                     self.LOGGER.warning("awaiting pending tasks to complete")
                     return False
         for future in as_completed(futures):
             if future.exception():
                 self.LOGGER.error("thread processing for '%s' received an exception: '%s'",
                                   iterator, future.exception())
-                RESULT['errors'] += 1
+                self.RESULT['errors'] += 1
             else:
-                RESULT['success'] += 1
+                self.RESULT['success'] += 1
         return True
 
     def _run(self) -> NoReturn:
         """Runs initiate request injection and prints success and error count."""
         try:
             self.LOGGER.info("Initiating sample call")
             self.make_request(sample=True)  # at least one request should pass before initiating request injection
@@ -118,13 +118,13 @@
                 f"\n{error.__str__()}\n\ntest call failed, cannot proceed stress testing\n"
             )
             return
         self.LOGGER.info("Running request injection on '%s' with rate %s", self.parsed.netloc, f'{self.request_rate:,}')
         start = time.time()
         run_assert = self.initiate_injection()
         self.LOGGER.info("Request injection completed in %f seconds", round(float(time.time() - start), 2))
-        self.LOGGER.info("Total number of requests passed: %d", RESULT['success'])
-        self.LOGGER.warning("Total number of requests failed: %d", RESULT['errors'])
+        self.LOGGER.info("Total number of requests passed: %d", self.RESULT['success'])
+        self.LOGGER.warning("Total number of requests failed: %d", self.RESULT['errors'])
         if run_assert:
-            assert sum(RESULT.values()) == self.request_rate, "Not all request trails were successful"
+            assert sum(self.RESULT.values()) == self.request_rate, "Not all request trails were successful"
         else:
-            self.LOGGER.warning("Total number of requests abandoned: %d", self.request_rate - sum(RESULT.values()))
+            self.LOGGER.warning("Total number of requests abandoned: %d", self.request_rate - sum(self.RESULT.values()))
```

## Comparing `stress_injector-0.5.dist-info/LICENSE` & `stress_injector-0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `stress_injector-0.5.dist-info/METADATA` & `stress_injector-0.7.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7374 7265  : 2.1.Name: stre
 00000020: 7373 2d69 6e6a 6563 746f 720a 5665 7273  ss-injector.Vers
-00000030: 696f 6e3a 2030 2e35 0a53 756d 6d61 7279  ion: 0.5.Summary
+00000030: 696f 6e3a 2030 2e37 0a53 756d 6d61 7279  ion: 0.7.Summary
 00000040: 3a20 5079 7468 6f6e 206d 6f64 756c 652c  : Python module,
 00000050: 2074 6f20 696e 6a65 6374 206d 656d 6f72   to inject memor
 00000060: 7920 616e 6420 4350 5520 7374 7265 7373  y and CPU stress
 00000070: 2c20 616e 6420 5552 4c20 6c6f 6164 2074  , and URL load t
 00000080: 6573 740a 4175 7468 6f72 2d65 6d61 696c  est.Author-email
 00000090: 3a20 5669 676e 6573 6820 5369 7661 6e61  : Vignesh Sivana
 000000a0: 6e64 6861 2052 616f 203c 7376 6967 6e65  ndha Rao <svigne
@@ -179,355 +179,383 @@
 00000b20: 7079 2d76 6572 7369 6f6e 5d28 6874 7470  py-version](http
 00000b30: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
 00000b40: 696f 2f70 7970 692f 7079 7665 7273 696f  io/pypi/pyversio
 00000b50: 6e73 2f73 7472 6573 732d 696e 6a65 6374  ns/stress-inject
 00000b60: 6f72 295d 2868 7474 7073 3a2f 2f70 7970  or)](https://pyp
 00000b70: 692e 6f72 672f 7072 6f6a 6563 742f 7374  i.org/project/st
 00000b80: 7265 7373 2d69 6e6a 6563 746f 7229 0a0a  ress-injector)..
-00000b90: 215b 646f 6373 5d28 6874 7470 733a 2f2f  ![docs](https://
-00000ba0: 6769 7468 7562 2e63 6f6d 2f74 6865 7669  github.com/thevi
-00000bb0: 636b 7970 6564 6961 2f73 7472 6573 732d  ckypedia/stress-
-00000bc0: 696e 6a65 6374 6f72 2f61 6374 696f 6e73  injector/actions
-00000bd0: 2f77 6f72 6b66 6c6f 7773 2f64 6f63 732e  /workflows/docs.
-00000be0: 796d 6c2f 6261 6467 652e 7376 6729 0a21  yml/badge.svg).!
-00000bf0: 5b70 7970 695d 2868 7474 7073 3a2f 2f67  [pypi](https://g
-00000c00: 6974 6875 622e 636f 6d2f 7468 6576 6963  ithub.com/thevic
-00000c10: 6b79 7065 6469 612f 7374 7265 7373 2d69  kypedia/stress-i
-00000c20: 6e6a 6563 746f 722f 6163 7469 6f6e 732f  njector/actions/
-00000c30: 776f 726b 666c 6f77 732f 7079 7468 6f6e  workflows/python
-00000c40: 2d70 7562 6c69 7368 2e79 6d6c 2f62 6164  -publish.yml/bad
-00000c50: 6765 2e73 7667 290a 0a5b 215b 5079 7069  ge.svg)..[![Pypi
-00000c60: 2d66 6f72 6d61 745d 2868 7474 7073 3a2f  -format](https:/
-00000c70: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000c80: 7079 7069 2f66 6f72 6d61 742f 7374 7265  pypi/format/stre
-00000c90: 7373 2d69 6e6a 6563 746f 7229 5d28 6874  ss-injector)](ht
-00000ca0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-00000cb0: 726f 6a65 6374 2f73 7472 6573 732d 696e  roject/stress-in
-00000cc0: 6a65 6374 6f72 2f23 6669 6c65 7329 0a5b  jector/#files).[
-00000cd0: 215b 5079 7069 2d73 7461 7475 735d 2868  ![Pypi-status](h
-00000ce0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000cf0: 6473 2e69 6f2f 7079 7069 2f73 7461 7475  ds.io/pypi/statu
-00000d00: 732f 7374 7265 7373 2d69 6e6a 6563 746f  s/stress-injecto
-00000d10: 7229 5d28 6874 7470 733a 2f2f 7079 7069  r)](https://pypi
-00000d20: 2e6f 7267 2f70 726f 6a65 6374 2f73 7472  .org/project/str
-00000d30: 6573 732d 696e 6a65 6374 6f72 290a 0a21  ess-injector)..!
-00000d40: 5b4d 6169 6e74 6169 6e65 645d 2868 7474  [Maintained](htt
-00000d50: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000d60: 2e69 6f2f 6d61 696e 7465 6e61 6e63 652f  .io/maintenance/
-00000d70: 7965 732f 3230 3233 290a 5b21 5b47 6974  yes/2023).[![Git
-00000d80: 4875 6220 5265 706f 2063 7265 6174 6564  Hub Repo created
-00000d90: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000da0: 6965 6c64 732e 696f 2f64 6174 652f 3135  ields.io/date/15
-00000db0: 3939 3433 3233 3130 295d 2868 7474 7073  99432310)](https
-00000dc0: 3a2f 2f61 7069 2e67 6974 6875 622e 636f  ://api.github.co
-00000dd0: 6d2f 7265 706f 732f 7468 6576 6963 6b79  m/repos/thevicky
-00000de0: 7065 6469 612f 7374 7265 7373 2d69 6e6a  pedia/stress-inj
-00000df0: 6563 746f 7229 0a5b 215b 4769 7448 7562  ector).[![GitHub
-00000e00: 2063 6f6d 6d69 7420 6163 7469 7669 7479   commit activity
-00000e10: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000e20: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-00000e30: 636f 6d6d 6974 2d61 6374 6976 6974 792f  commit-activity/
-00000e40: 792f 7468 6576 6963 6b79 7065 6469 612f  y/thevickypedia/
-00000e50: 7374 7265 7373 2d69 6e6a 6563 746f 7229  stress-injector)
-00000e60: 5d28 6874 7470 733a 2f2f 6170 692e 6769  ](https://api.gi
-00000e70: 7468 7562 2e63 6f6d 2f72 6570 6f73 2f74  thub.com/repos/t
-00000e80: 6865 7669 636b 7970 6564 6961 2f73 7472  hevickypedia/str
-00000e90: 6573 732d 696e 6a65 6374 6f72 290a 5b21  ess-injector).[!
-00000ea0: 5b47 6974 4875 6220 6c61 7374 2063 6f6d  [GitHub last com
-00000eb0: 6d69 745d 2868 7474 7073 3a2f 2f69 6d67  mit](https://img
-00000ec0: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
-00000ed0: 7562 2f6c 6173 742d 636f 6d6d 6974 2f74  ub/last-commit/t
-00000ee0: 6865 7669 636b 7970 6564 6961 2f73 7472  hevickypedia/str
-00000ef0: 6573 732d 696e 6a65 6374 6f72 295d 2868  ess-injector)](h
-00000f00: 7474 7073 3a2f 2f61 7069 2e67 6974 6875  ttps://api.githu
-00000f10: 622e 636f 6d2f 7265 706f 732f 7468 6576  b.com/repos/thev
-00000f20: 6963 6b79 7065 6469 612f 7374 7265 7373  ickypedia/stress
-00000f30: 2d69 6e6a 6563 746f 7229 0a0a 2320 5374  -injector)..# St
-00000f40: 7265 7373 2049 6e6a 6563 746f 720a 5079  ress Injector.Py
-00000f50: 7468 6f6e 206d 6f64 756c 652c 2074 6f20  thon module, to 
-00000f60: 696e 6a65 6374 206d 656d 6f72 7920 616e  inject memory an
-00000f70: 6420 4350 5520 7374 7265 7373 0a0a 3c64  d CPU stress..<d
-00000f80: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
-00000f90: 3e3c 7374 726f 6e67 3e49 6e73 6967 6874  ><strong>Insight
-00000fa0: 7320 6162 6f75 7420 3c61 2068 7265 663d  s about <a href=
-00000fb0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00000fc0: 636f 6d2f 7468 6576 6963 6b79 7065 6469  com/thevickypedi
-00000fd0: 612f 7374 7265 7373 2d69 6e6a 6563 746f  a/stress-injecto
-00000fe0: 722f 626c 6f62 2f6d 6169 6e2f 7374 7265  r/blob/main/stre
-00000ff0: 7373 696e 6a65 6374 6f72 2f63 7075 2e70  ssinjector/cpu.p
-00001000: 7922 3e43 5055 2053 7472 6573 733c 2f61  y">CPU Stress</a
-00001010: 3e3c 2f73 7472 6f6e 673e 3c2f 7375 6d6d  ></strong></summ
-00001020: 6172 793e 0a0a 2a20 546f 2061 6368 6965  ary>..* To achie
-00001030: 7665 2043 5055 2073 7472 6573 732c 2049  ve CPU stress, I
-00001040: 2068 6176 6520 7573 6564 206d 756c 7469   have used multi
-00001050: 7072 6f63 6573 732c 206c 6f6f 7065 6420  process, looped 
-00001060: 666f 7220 7468 6520 6e75 6d62 6572 206f  for the number o
-00001070: 6620 6c6f 6769 6361 6c20 636f 7265 732c  f logical cores,
-00001080: 2074 7269 6767 6572 696e 6720 616e 2069   triggering an i
-00001090: 6e66 696e 6974 6520 6c6f 6f70 206f 6e0a  nfinite loop on.
-000010a0: 2020 6561 6368 2063 6f72 652e 0a2a 2054    each core..* T
-000010b0: 6865 2069 6e66 696e 6974 6520 6c6f 6f70  he infinite loop
-000010c0: 2077 696c 6c20 7275 6e20 666f 7220 6120   will run for a 
-000010d0: 6769 7665 6e20 6e75 6d62 6572 206f 6620  given number of 
-000010e0: 7365 636f 6e64 7320 7072 6f76 6964 6564  seconds provided
-000010f0: 2062 7920 7573 6572 2e0a 2a20 4d65 616e   by user..* Mean
-00001100: 2d77 6869 6c65 2074 6865 2060 6370 755f  -while the `cpu_
-00001110: 7065 7263 656e 7460 2066 726f 6d20 6070  percent` from `p
-00001120: 7375 7469 6c60 2072 756e 7320 2864 6564  sutil` runs (ded
-00001130: 6963 6174 6564 2074 6872 6561 6429 2069  icated thread) i
-00001140: 6e20 616e 2069 6e66 696e 6974 6520 6c6f  n an infinite lo
-00001150: 6f70 2063 616c 6375 6c61 7469 6e67 2074  op calculating t
-00001160: 6865 2063 7572 7265 6e74 2043 5055 200a  he current CPU .
-00001170: 2020 7574 696c 697a 6174 696f 6e20 6f6e    utilization on
-00001180: 2065 6163 6820 4350 5520 636f 7265 2e0a   each CPU core..
-00001190: 2a20 5468 6520 6465 6469 6361 7465 6420  * The dedicated 
-000011a0: 7468 7265 6164 2072 756e 7320 666f 7220  thread runs for 
-000011b0: 3320 7365 636f 6e64 7320 696e 2061 6464  3 seconds in add
-000011c0: 6974 696f 6e20 746f 2074 6865 206e 756d  ition to the num
-000011d0: 6265 7220 6f66 2073 6563 6f6e 6473 2070  ber of seconds p
-000011e0: 726f 7669 6465 6420 6279 2074 6865 2075  rovided by the u
-000011f0: 7365 722e 0a2a 204f 6e63 6520 7468 6520  ser..* Once the 
-00001200: 6769 7665 6e20 6e75 6d62 6572 206f 6620  given number of 
-00001210: 7365 636f 6e64 7320 6861 7665 2070 6173  seconds have pas
-00001220: 7365 642c 2074 6865 2060 6d75 6c74 6970  sed, the `multip
-00001230: 726f 6365 7373 6020 616e 6420 6074 6872  rocess` and `thr
-00001240: 6561 6460 2074 6861 7420 7761 7320 696e  ead` that was in
-00001250: 6974 6961 7465 6420 746f 206d 6f6e 6974  itiated to monit
-00001260: 6f72 2043 5055 2075 7361 6765 2061 7265  or CPU usage are
-00001270: 2073 746f 7070 6564 2e0a 3c2f 6465 7461   stopped..</deta
-00001280: 696c 733e 0a3c 6272 3e0a 3c64 6574 6169  ils>.<br>.<detai
-00001290: 6c73 3e0a 3c73 756d 6d61 7279 3e3c 7374  ls>.<summary><st
-000012a0: 726f 6e67 3e49 6e73 6967 6874 7320 6162  rong>Insights ab
-000012b0: 6f75 7420 3c61 2068 7265 663d 2268 7474  out <a href="htt
-000012c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000012d0: 7468 6576 6963 6b79 7065 6469 612f 7374  thevickypedia/st
-000012e0: 7265 7373 2d69 6e6a 6563 746f 722f 626c  ress-injector/bl
-000012f0: 6f62 2f6d 6169 6e2f 7374 7265 7373 696e  ob/main/stressin
-00001300: 6a65 6374 6f72 2f6d 656d 6f72 792e 7079  jector/memory.py
-00001310: 223e 4d65 6d6f 7279 2053 7472 6573 733c  ">Memory Stress<
-00001320: 2f61 3e3c 2f73 7472 6f6e 673e 3c2f 7375  /a></strong></su
-00001330: 6d6d 6172 793e 0a0a 2a20 496e 2074 6869  mmary>..* In thi
-00001340: 7320 7363 7269 7074 2c20 4920 6861 7665  s script, I have
-00001350: 2075 7365 6420 606e 756d 7079 2e72 616e   used `numpy.ran
-00001360: 646f 6d2e 6279 7465 7360 2077 6869 6368  dom.bytes` which
-00001370: 2061 7265 2073 616d 706c 6564 2066 726f   are sampled fro
-00001380: 6d20 756e 6966 6f72 6d20 6469 7374 7269  m uniform distri
-00001390: 6275 7469 6f6e 2e0a 2a20 4765 6e65 7261  bution..* Genera
-000013a0: 7469 6e67 2074 6865 7365 2072 616e 646f  ting these rando
-000013b0: 6d20 6279 7465 7320 696e 6475 6365 7320  m bytes induces 
-000013c0: 6120 7374 7265 7373 206f 6e20 7468 6520  a stress on the 
-000013d0: 6d61 6368 696e 6527 7320 6d65 6d6f 7279  machine's memory
-000013e0: 2075 7361 6765 2e0a 2a20 4920 6861 7665   usage..* I have
-000013f0: 2074 6865 6e20 7573 6564 2060 6765 7472   then used `getr
-00001400: 7573 6167 6560 2028 6765 7420 7265 736f  usage` (get reso
-00001410: 7572 6365 2075 7361 6765 2920 666f 7220  urce usage) for 
-00001420: 6053 454c 4660 2074 6f20 6765 7420 7468  `SELF` to get th
-00001430: 6520 6d65 6d6f 7279 2063 6f6e 7375 6d65  e memory consume
-00001440: 6420 6f6e 6c79 2062 7920 7468 6520 6375  d only by the cu
-00001450: 7272 656e 7420 7363 7269 7074 2e0a 2a20  rrent script..* 
-00001460: 5468 6520 6073 697a 655f 636f 6e76 6572  The `size_conver
-00001470: 7465 7260 2063 6f6e 7665 7274 7320 7468  ter` converts th
-00001480: 6520 6279 7465 7320 6672 6f6d 2072 6573  e bytes from res
-00001490: 6f75 7263 6520 7573 6167 6520 746f 2061  ource usage to a
-000014a0: 2068 756d 616e 2075 6e64 6572 7374 616e   human understan
-000014b0: 6461 626c 6520 666f 726d 6174 2e0a 3c2f  dable format..</
-000014c0: 6465 7461 696c 733e 0a3c 6272 3e0a 3c64  details>.<br>.<d
-000014d0: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
-000014e0: 3e3c 7374 726f 6e67 3e49 6e73 6967 6874  ><strong>Insight
-000014f0: 7320 6162 6f75 7420 3c61 2068 7265 663d  s about <a href=
-00001500: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00001510: 636f 6d2f 7468 6576 6963 6b79 7065 6469  com/thevickypedi
-00001520: 612f 7374 7265 7373 2d69 6e6a 6563 746f  a/stress-injecto
-00001530: 722f 626c 6f62 2f6d 6169 6e2f 7374 7265  r/blob/main/stre
-00001540: 7373 696e 6a65 6374 6f72 2f6f 6e75 732e  ssinjector/onus.
-00001550: 7079 223e 5552 4c20 5374 7265 7373 3c2f  py">URL Stress</
-00001560: 613e 3c2f 7374 726f 6e67 3e3c 2f73 756d  a></strong></sum
-00001570: 6d61 7279 3e0a 0a2a 2049 6e20 7468 6973  mary>..* In this
-00001580: 2073 6372 6970 742c 2049 2068 6176 6520   script, I have 
-00001590: 7573 6564 2074 6872 6561 6470 6f6f 6c73  used threadpools
-000015a0: 2074 6f20 6d61 6b65 2063 6f6e 6375 7272   to make concurr
-000015b0: 656e 7420 7265 7175 6573 7473 2e0a 2a20  ent requests..* 
-000015c0: 5468 6520 7363 7269 7074 2075 7365 7320  The script uses 
-000015d0: 6072 6571 7565 7374 7360 206d 6f64 756c  `requests` modul
-000015e0: 6520 746f 206d 616b 6520 6361 6c6c 732e  e to make calls.
-000015f0: 0a2a 2054 616b 6573 2061 7267 756d 656e  .* Takes argumen
-00001600: 7473 0a20 202a 202a 2a72 6174 652a 2a3a  ts.  * **rate**:
-00001610: 204e 756d 6265 7220 6f66 2063 616c 6c73   Number of calls
-00001620: 2074 6f20 6d61 6b65 2e20 5f44 6566 6175   to make. _Defau
-00001630: 6c74 7320 746f 2031 3030 4b5f 0a20 202a  lts to 100K_.  *
-00001640: 202a 2a74 696d 656f 7574 2a2a 3a20 5469   **timeout**: Ti
-00001650: 6d65 6f75 7420 666f 7220 6561 6368 2072  meout for each r
-00001660: 6571 7565 7374 2e20 5f44 6566 6175 6c74  equest. _Default
-00001670: 7320 746f 2030 2e35 5f0a 2020 2a20 2a2a  s to 0.5_.  * **
-00001680: 7265 7472 795f 6c69 6d69 742a 2a3a 2052  retry_limit**: R
-00001690: 6574 7279 206c 696d 6974 2069 6620 7468  etry limit if th
-000016a0: 6520 7379 7374 656d 2069 7320 756e 6162  e system is unab
-000016b0: 6c65 2074 6f20 7370 696e 7570 206d 6f72  le to spinup mor
-000016c0: 6520 7468 7265 6164 732e 205f 4465 6661  e threads. _Defa
-000016d0: 756c 7473 2074 6f20 355f 0a20 202a 202a  ults to 5_.  * *
-000016e0: 2a63 6972 6375 6974 5f62 7265 616b 2a2a  *circuit_break**
-000016f0: 3a20 5761 6974 2074 696d 6520 696e 2073  : Wait time in s
-00001700: 6563 6f6e 6473 2062 6574 7765 656e 2072  econds between r
-00001710: 6574 7269 6573 2e20 5f44 6566 6175 6c74  etries. _Default
-00001720: 7320 746f 2035 5f0a 2020 2a20 2a2a 7265  s to 5_.  * **re
-00001730: 7175 6573 745f 7479 7065 2a2a 3a20 4675  quest_type**: Fu
-00001740: 6e63 7469 6f6e 2066 726f 6d20 6072 6571  nction from `req
-00001750: 7565 7374 7360 206d 6f64 756c 652e 0a0a  uests` module...
-00001760: 3c2f 6465 7461 696c 733e 0a0a 2323 2320  </details>..### 
-00001770: 5573 6167 650a 6070 6970 2069 6e73 7461  Usage.`pip insta
-00001780: 6c6c 2073 7472 6573 732d 696e 6a65 6374  ll stress-inject
-00001790: 6f72 600a 0a5b 4350 5520 5374 7265 7373  or`..[CPU Stress
-000017a0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000017b0: 2e63 6f6d 2f74 6865 7669 636b 7970 6564  .com/thevickyped
-000017c0: 6961 2f73 7472 6573 732d 696e 6a65 6374  ia/stress-inject
-000017d0: 6f72 2f62 6c6f 622f 6d61 696e 2f73 7472  or/blob/main/str
-000017e0: 6573 7369 6e6a 6563 746f 722f 6370 752e  essinjector/cpu.
-000017f0: 7079 290a 6060 6070 7974 686f 6e0a 696d  py).```python.im
-00001800: 706f 7274 2073 7472 6573 7369 6e6a 6563  port stressinjec
-00001810: 746f 7220 6173 2069 6e6a 6563 746f 720a  tor as injector.
-00001820: 0a0a 6966 205f 5f6e 616d 655f 5f20 3d3d  ..if __name__ ==
-00001830: 2027 5f5f 6d61 696e 5f5f 273a 0a20 2020   '__main__':.   
-00001840: 2069 6e6a 6563 746f 722e 4350 5553 7472   injector.CPUStr
-00001850: 6573 7328 7365 636f 6e64 733d 3330 3029  ess(seconds=300)
-00001860: 0a60 6060 0a0a 5b4d 656d 6f72 7920 5374  .```..[Memory St
-00001870: 7265 7373 5d28 6874 7470 733a 2f2f 6769  ress](https://gi
-00001880: 7468 7562 2e63 6f6d 2f74 6865 7669 636b  thub.com/thevick
-00001890: 7970 6564 6961 2f73 7472 6573 732d 696e  ypedia/stress-in
-000018a0: 6a65 6374 6f72 2f62 6c6f 622f 6d61 696e  jector/blob/main
-000018b0: 2f73 7472 6573 7369 6e6a 6563 746f 722f  /stressinjector/
-000018c0: 6d65 6d6f 7279 2e70 7929 0a60 6060 7079  memory.py).```py
-000018d0: 7468 6f6e 0a69 6d70 6f72 7420 7374 7265  thon.import stre
-000018e0: 7373 696e 6a65 6374 6f72 2061 7320 696e  ssinjector as in
-000018f0: 6a65 6374 6f72 0a0a 0a69 6620 5f5f 6e61  jector...if __na
-00001900: 6d65 5f5f 203d 3d20 275f 5f6d 6169 6e5f  me__ == '__main_
-00001910: 5f27 3a0a 2020 2020 696e 6a65 6374 6f72  _':.    injector
-00001920: 2e4d 656d 6f72 7953 7472 6573 7328 6769  .MemoryStress(gi
-00001930: 6761 6279 7465 733d 325f 3030 3029 2e72  gabytes=2_000).r
-00001940: 756e 2829 0a60 6060 0a0a 5b55 524c 2053  un().```..[URL S
-00001950: 7472 6573 735d 2868 7474 7073 3a2f 2f67  tress](https://g
-00001960: 6974 6875 622e 636f 6d2f 7468 6576 6963  ithub.com/thevic
-00001970: 6b79 7065 6469 612f 7374 7265 7373 2d69  kypedia/stress-i
-00001980: 6e6a 6563 746f 722f 626c 6f62 2f6d 6169  njector/blob/mai
-00001990: 6e2f 7374 7265 7373 696e 6a65 6374 6f72  n/stressinjector
-000019a0: 2f75 726c 2e70 7929 0a60 6060 7079 7468  /url.py).```pyth
-000019b0: 6f6e 0a69 6d70 6f72 7420 6f73 0a69 6d70  on.import os.imp
-000019c0: 6f72 7420 7374 7265 7373 696e 6a65 6374  ort stressinject
-000019d0: 6f72 2061 7320 696e 6a65 6374 6f72 0a0a  or as injector..
-000019e0: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
-000019f0: 275f 5f6d 6169 6e5f 5f27 3a0a 2020 2020  '__main__':.    
-00001a00: 696e 6a65 6374 6f72 2e55 524c 5374 7265  injector.URLStre
-00001a10: 7373 2875 726c 3d27 6874 7470 3a2f 2f30  ss(url='http://0
-00001a20: 2e30 2e30 2e30 3a35 3030 322f 2729 2020  .0.0.0:5002/')  
-00001a30: 2320 5374 7265 7373 2074 6573 7420 4745  # Stress test GE
-00001a40: 5420 6361 6c6c 730a 0a20 2020 2023 2053  T calls..    # S
-00001a50: 7472 6573 7320 7465 7374 2050 4f53 5420  tress test POST 
-00001a60: 6361 6c6c 732c 2061 6c73 6f20 7375 7070  calls, also supp
-00001a70: 6f72 7473 2050 5554 2c20 616e 6420 4445  orts PUT, and DE
-00001a80: 4c45 5445 0a20 2020 2073 616d 706c 655f  LETE.    sample_
-00001a90: 6461 7461 203d 207b 2768 6561 6465 7273  data = {'headers
-00001aa0: 273a 207b 2741 7574 686f 7269 7a61 7469  ': {'Authorizati
-00001ab0: 6f6e 273a 2027 4265 6172 6572 2025 7327  on': 'Bearer %s'
-00001ac0: 2025 206f 732e 656e 7669 726f 6e2e 6765   % os.environ.ge
-00001ad0: 7428 2754 4f4b 454e 2729 7d7d 0a20 2020  t('TOKEN')}}.   
-00001ae0: 2069 6e6a 6563 746f 722e 5552 4c53 7472   injector.URLStr
-00001af0: 6573 7328 0a20 2020 2020 2075 726c 3d27  ess(.      url='
-00001b00: 6874 7470 3a2f 2f30 2e30 2e30 2e30 3a35  http://0.0.0.0:5
-00001b10: 3030 322f 272c 0a20 2020 2020 2072 6571  002/',.      req
-00001b20: 7565 7374 5f74 7970 653d 696e 6a65 6374  uest_type=inject
-00001b30: 6f72 2e52 6571 7565 7374 5479 7065 2e70  or.RequestType.p
-00001b40: 6f73 742c 0a20 2020 2020 202a 2a73 616d  ost,.      **sam
-00001b50: 706c 655f 6461 7461 0a20 2020 2029 0a60  ple_data.    ).`
-00001b60: 6060 0a0a 2323 2323 2043 6f64 696e 6720  ``..#### Coding 
-00001b70: 5374 616e 6461 7264 730a 446f 6373 7472  Standards.Docstr
-00001b80: 696e 6720 666f 726d 6174 3a20 5b60 476f  ing format: [`Go
-00001b90: 6f67 6c65 605d 2868 7474 7073 3a2f 2f67  ogle`](https://g
-00001ba0: 6f6f 676c 652e 6769 7468 7562 2e69 6f2f  oogle.github.io/
-00001bb0: 7374 796c 6567 7569 6465 2f70 7967 7569  styleguide/pygui
-00001bc0: 6465 2e68 746d 6c23 3338 2d63 6f6d 6d65  de.html#38-comme
-00001bd0: 6e74 732d 616e 642d 646f 6373 7472 696e  nts-and-docstrin
-00001be0: 6773 2920 3c62 723e 0a53 7479 6c69 6e67  gs) <br>.Styling
-00001bf0: 2063 6f6e 7665 6e74 696f 6e73 3a20 5b60   conventions: [`
-00001c00: 5045 5020 3860 5d28 6874 7470 733a 2f2f  PEP 8`](https://
-00001c10: 7777 772e 7079 7468 6f6e 2e6f 7267 2f64  www.python.org/d
-00001c20: 6576 2f70 6570 732f 7065 702d 3030 3038  ev/peps/pep-0008
-00001c30: 2f29 203c 6272 3e0a 436c 6561 6e20 636f  /) <br>.Clean co
-00001c40: 6465 2077 6974 6820 7072 652d 636f 6d6d  de with pre-comm
-00001c50: 6974 2068 6f6f 6b73 3a20 5b60 666c 616b  it hooks: [`flak
-00001c60: 6538 605d 2868 7474 7073 3a2f 2f66 6c61  e8`](https://fla
-00001c70: 6b65 382e 7079 6371 612e 6f72 672f 656e  ke8.pycqa.org/en
-00001c80: 2f6c 6174 6573 742f 2920 616e 6420 0a5b  /latest/) and .[
-00001c90: 6069 736f 7274 605d 2868 7474 7073 3a2f  `isort`](https:/
-00001ca0: 2f70 7963 7161 2e67 6974 6875 622e 696f  /pycqa.github.io
-00001cb0: 2f69 736f 7274 2f29 0a0a 2323 2323 205b  /isort/)..#### [
-00001cc0: 5265 6c65 6173 6520 4e6f 7465 735d 2868  Release Notes](h
-00001cd0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001ce0: 6d2f 7468 6576 6963 6b79 7065 6469 612f  m/thevickypedia/
-00001cf0: 7374 7265 7373 2d69 6e6a 6563 746f 722f  stress-injector/
-00001d00: 626c 6f62 2f6d 6169 6e2f 7265 6c65 6173  blob/main/releas
-00001d10: 655f 6e6f 7465 732e 7273 7429 0a2a 2a52  e_notes.rst).**R
-00001d20: 6571 7569 7265 6d65 6e74 2a2a 0a60 6060  equirement**.```
-00001d30: 7368 656c 6c0a 7079 7468 6f6e 202d 6d20  shell.python -m 
-00001d40: 7069 7020 696e 7374 616c 6c20 6368 616e  pip install chan
-00001d50: 6765 6c6f 672d 6765 6e65 7261 746f 720a  gelog-generator.
-00001d60: 6060 600a 0a2a 2a55 7361 6765 2a2a 0a60  ```..**Usage**.`
-00001d70: 6060 7368 656c 6c0a 6368 616e 6765 6c6f  ``shell.changelo
-00001d80: 6720 7265 7665 7273 6520 2d66 2072 656c  g reverse -f rel
-00001d90: 6561 7365 5f6e 6f74 6573 2e72 7374 202d  ease_notes.rst -
-00001da0: 7420 2752 656c 6561 7365 204e 6f74 6573  t 'Release Notes
-00001db0: 270a 6060 600a 0a23 2323 2320 4c69 6e74  '.```..#### Lint
-00001dc0: 696e 670a 6050 7265 436f 6d6d 6974 6020  ing.`PreCommit` 
-00001dd0: 7769 6c6c 2065 6e73 7572 6520 6c69 6e74  will ensure lint
-00001de0: 696e 672c 2061 6e64 2074 6865 2064 6f63  ing, and the doc
-00001df0: 2063 7265 6174 696f 6e20 6172 6520 7275   creation are ru
-00001e00: 6e20 6f6e 2065 7665 7279 2063 6f6d 6d69  n on every commi
-00001e10: 742e 0a0a 2a2a 5265 7175 6972 656d 656e  t...**Requiremen
-00001e20: 742a 2a0a 3c62 723e 0a60 6060 6261 7368  t**.<br>.```bash
-00001e30: 0a70 6970 2069 6e73 7461 6c6c 202d 2d6e  .pip install --n
-00001e40: 6f2d 6361 6368 6520 7370 6869 6e78 3d3d  o-cache sphinx==
-00001e50: 352e 312e 3120 7072 652d 636f 6d6d 6974  5.1.1 pre-commit
-00001e60: 2072 6563 6f6d 6d6f 6e6d 6172 6b0a 6060   recommonmark.``
-00001e70: 600a 0a2a 2a55 7361 6765 2a2a 0a3c 6272  `..**Usage**.<br
-00001e80: 3e0a 6060 6062 6173 680a 7072 652d 636f  >.```bash.pre-co
-00001e90: 6d6d 6974 2072 756e 202d 2d61 6c6c 2d66  mmit run --all-f
-00001ea0: 696c 6573 0a60 6060 0a0a 2323 2320 5079  iles.```..### Py
-00001eb0: 7069 2050 6163 6b61 6765 0a5b 215b 7079  pi Package.[![py
-00001ec0: 7069 2d6d 6f64 756c 655d 2868 7474 7073  pi-module](https
-00001ed0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00001ee0: 6f2f 6261 6467 652f 536f 6674 7761 7265  o/badge/Software
-00001ef0: 2532 3052 6570 6f73 6974 6f72 792d 7079  %20Repository-py
-00001f00: 7069 2d31 6634 3235 662e 7376 6729 5d28  pi-1f425f.svg)](
-00001f10: 6874 7470 733a 2f2f 7061 636b 6167 696e  https://packagin
-00001f20: 672e 7079 7468 6f6e 2e6f 7267 2f74 7574  g.python.org/tut
-00001f30: 6f72 6961 6c73 2f70 6163 6b61 6769 6e67  orials/packaging
-00001f40: 2d70 726f 6a65 6374 732f 290a 0a5b 6874  -projects/)..[ht
-00001f50: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-00001f60: 726f 6a65 6374 2f73 7472 6573 732d 696e  roject/stress-in
-00001f70: 6a65 6374 6f72 2f5d 2868 7474 7073 3a2f  jector/](https:/
-00001f80: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00001f90: 742f 7374 7265 7373 2d69 6e6a 6563 746f  t/stress-injecto
-00001fa0: 722f 290a 0a23 2323 2052 756e 626f 6f6b  r/)..### Runbook
-00001fb0: 0a5b 215b 6d61 6465 2d77 6974 682d 7370  .[![made-with-sp
-00001fc0: 6869 6e78 2d64 6f63 5d28 6874 7470 733a  hinx-doc](https:
-00001fd0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00001fe0: 2f62 6164 6765 2f43 6f64 6525 3230 446f  /badge/Code%20Do
-00001ff0: 6373 2d53 7068 696e 782d 3166 3432 3566  cs-Sphinx-1f425f
-00002000: 2e73 7667 295d 2868 7474 7073 3a2f 2f77  .svg)](https://w
-00002010: 7777 2e73 7068 696e 782d 646f 632e 6f72  ww.sphinx-doc.or
-00002020: 672f 656e 2f6d 6173 7465 722f 6d61 6e2f  g/en/master/man/
-00002030: 7370 6869 6e78 2d61 7574 6f67 656e 2e68  sphinx-autogen.h
-00002040: 746d 6c29 0a0a 5b68 7474 7073 3a2f 2f74  tml)..[https://t
-00002050: 6865 7669 636b 7970 6564 6961 2e67 6974  hevickypedia.git
-00002060: 6875 622e 696f 2f73 7472 6573 732d 696e  hub.io/stress-in
-00002070: 6a65 6374 6f72 2f5d 2868 7474 7073 3a2f  jector/](https:/
-00002080: 2f74 6865 7669 636b 7970 6564 6961 2e67  /thevickypedia.g
-00002090: 6974 6875 622e 696f 2f73 7472 6573 732d  ithub.io/stress-
-000020a0: 696e 6a65 6374 6f72 2f29 0a0a 2323 204c  injector/)..## L
-000020b0: 6963 656e 7365 2026 2063 6f70 7972 6967  icense & copyrig
-000020c0: 6874 0a0a 2663 6f70 793b 2056 6967 6e65  ht..&copy; Vigne
-000020d0: 7368 2053 6976 616e 616e 6468 6120 5261  sh Sivanandha Ra
-000020e0: 6f0a 0a4c 6963 656e 7365 6420 756e 6465  o..Licensed unde
-000020f0: 7220 7468 6520 5b4d 4954 204c 6963 656e  r the [MIT Licen
-00002100: 7365 5d28 6874 7470 733a 2f2f 6769 7468  se](https://gith
-00002110: 7562 2e63 6f6d 2f74 6865 7669 636b 7970  ub.com/thevickyp
-00002120: 6564 6961 2f73 7472 6573 732d 696e 6a65  edia/stress-inje
-00002130: 6374 6f72 2f62 6c6f 622f 6d61 696e 2f4c  ctor/blob/main/L
-00002140: 4943 454e 5345 290a                      ICENSE).
+00000b90: 5b21 5b70 6167 6573 2d62 7569 6c64 2d64  [![pages-build-d
+00000ba0: 6570 6c6f 796d 656e 745d 2868 7474 7073  eployment](https
+00000bb0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7468  ://github.com/th
+00000bc0: 6576 6963 6b79 7065 6469 612f 7374 7265  evickypedia/stre
+00000bd0: 7373 2d69 6e6a 6563 746f 722f 6163 7469  ss-injector/acti
+00000be0: 6f6e 732f 776f 726b 666c 6f77 732f 7061  ons/workflows/pa
+00000bf0: 6765 732f 7061 6765 732d 6275 696c 642d  ges/pages-build-
+00000c00: 6465 706c 6f79 6d65 6e74 2f62 6164 6765  deployment/badge
+00000c10: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
+00000c20: 6974 6875 622e 636f 6d2f 7468 6576 6963  ithub.com/thevic
+00000c30: 6b79 7065 6469 612f 7374 7265 7373 2d69  kypedia/stress-i
+00000c40: 6e6a 6563 746f 722f 6163 7469 6f6e 732f  njector/actions/
+00000c50: 776f 726b 666c 6f77 732f 7061 6765 732f  workflows/pages/
+00000c60: 7061 6765 732d 6275 696c 642d 6465 706c  pages-build-depl
+00000c70: 6f79 6d65 6e74 290a 5b21 5b70 7970 692d  oyment).[![pypi-
+00000c80: 7075 626c 6973 685d 2868 7474 7073 3a2f  publish](https:/
+00000c90: 2f67 6974 6875 622e 636f 6d2f 7468 6576  /github.com/thev
+00000ca0: 6963 6b79 7065 6469 612f 7374 7265 7373  ickypedia/stress
+00000cb0: 2d69 6e6a 6563 746f 722f 6163 7469 6f6e  -injector/action
+00000cc0: 732f 776f 726b 666c 6f77 732f 7079 7468  s/workflows/pyth
+00000cd0: 6f6e 2d70 7562 6c69 7368 2e79 6d6c 2f62  on-publish.yml/b
+00000ce0: 6164 6765 2e73 7667 295d 2868 7474 7073  adge.svg)](https
+00000cf0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7468  ://github.com/th
+00000d00: 6576 6963 6b79 7065 6469 612f 7374 7265  evickypedia/stre
+00000d10: 7373 2d69 6e6a 6563 746f 722f 6163 7469  ss-injector/acti
+00000d20: 6f6e 732f 776f 726b 666c 6f77 732f 7079  ons/workflows/py
+00000d30: 7468 6f6e 2d70 7562 6c69 7368 2e79 6d6c  thon-publish.yml
+00000d40: 290a 0a5b 215b 5079 7069 2d66 6f72 6d61  )..[![Pypi-forma
+00000d50: 745d 2868 7474 7073 3a2f 2f69 6d67 2e73  t](https://img.s
+00000d60: 6869 656c 6473 2e69 6f2f 7079 7069 2f66  hields.io/pypi/f
+00000d70: 6f72 6d61 742f 7374 7265 7373 2d69 6e6a  ormat/stress-inj
+00000d80: 6563 746f 7229 5d28 6874 7470 733a 2f2f  ector)](https://
+00000d90: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+00000da0: 2f73 7472 6573 732d 696e 6a65 6374 6f72  /stress-injector
+00000db0: 2f23 6669 6c65 7329 0a5b 215b 5079 7069  /#files).[![Pypi
+00000dc0: 2d73 7461 7475 735d 2868 7474 7073 3a2f  -status](https:/
+00000dd0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000de0: 7079 7069 2f73 7461 7475 732f 7374 7265  pypi/status/stre
+00000df0: 7373 2d69 6e6a 6563 746f 7229 5d28 6874  ss-injector)](ht
+00000e00: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+00000e10: 726f 6a65 6374 2f73 7472 6573 732d 696e  roject/stress-in
+00000e20: 6a65 6374 6f72 290a 0a21 5b4d 6169 6e74  jector)..![Maint
+00000e30: 6169 6e65 645d 2868 7474 7073 3a2f 2f69  ained](https://i
+00000e40: 6d67 2e73 6869 656c 6473 2e69 6f2f 6d61  mg.shields.io/ma
+00000e50: 696e 7465 6e61 6e63 652f 7965 732f 3230  intenance/yes/20
+00000e60: 3233 290a 5b21 5b47 6974 4875 6220 5265  23).[![GitHub Re
+00000e70: 706f 2063 7265 6174 6564 5d28 6874 7470  po created](http
+00000e80: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000e90: 696f 2f64 6174 652f 3135 3939 3433 3233  io/date/15994323
+00000ea0: 3130 295d 2868 7474 7073 3a2f 2f61 7069  10)](https://api
+00000eb0: 2e67 6974 6875 622e 636f 6d2f 7265 706f  .github.com/repo
+00000ec0: 732f 7468 6576 6963 6b79 7065 6469 612f  s/thevickypedia/
+00000ed0: 7374 7265 7373 2d69 6e6a 6563 746f 7229  stress-injector)
+00000ee0: 0a5b 215b 4769 7448 7562 2063 6f6d 6d69  .[![GitHub commi
+00000ef0: 7420 6163 7469 7669 7479 5d28 6874 7470  t activity](http
+00000f00: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000f10: 696f 2f67 6974 6875 622f 636f 6d6d 6974  io/github/commit
+00000f20: 2d61 6374 6976 6974 792f 792f 7468 6576  -activity/y/thev
+00000f30: 6963 6b79 7065 6469 612f 7374 7265 7373  ickypedia/stress
+00000f40: 2d69 6e6a 6563 746f 7229 5d28 6874 7470  -injector)](http
+00000f50: 733a 2f2f 6170 692e 6769 7468 7562 2e63  s://api.github.c
+00000f60: 6f6d 2f72 6570 6f73 2f74 6865 7669 636b  om/repos/thevick
+00000f70: 7970 6564 6961 2f73 7472 6573 732d 696e  ypedia/stress-in
+00000f80: 6a65 6374 6f72 290a 5b21 5b47 6974 4875  jector).[![GitHu
+00000f90: 6220 6c61 7374 2063 6f6d 6d69 745d 2868  b last commit](h
+00000fa0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000fb0: 6473 2e69 6f2f 6769 7468 7562 2f6c 6173  ds.io/github/las
+00000fc0: 742d 636f 6d6d 6974 2f74 6865 7669 636b  t-commit/thevick
+00000fd0: 7970 6564 6961 2f73 7472 6573 732d 696e  ypedia/stress-in
+00000fe0: 6a65 6374 6f72 295d 2868 7474 7073 3a2f  jector)](https:/
+00000ff0: 2f61 7069 2e67 6974 6875 622e 636f 6d2f  /api.github.com/
+00001000: 7265 706f 732f 7468 6576 6963 6b79 7065  repos/thevickype
+00001010: 6469 612f 7374 7265 7373 2d69 6e6a 6563  dia/stress-injec
+00001020: 746f 7229 0a0a 2320 5374 7265 7373 2049  tor)..# Stress I
+00001030: 6e6a 6563 746f 720a 5079 7468 6f6e 206d  njector.Python m
+00001040: 6f64 756c 652c 2074 6f20 696e 6a65 6374  odule, to inject
+00001050: 206d 656d 6f72 792c 2043 5055 2061 6e64   memory, CPU and
+00001060: 2055 524c 2073 7472 6573 732e 0a0a 3c64   URL stress...<d
+00001070: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
+00001080: 3e3c 7374 726f 6e67 3e49 6e73 6967 6874  ><strong>Insight
+00001090: 7320 6162 6f75 7420 3c61 2068 7265 663d  s about <a href=
+000010a0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+000010b0: 636f 6d2f 7468 6576 6963 6b79 7065 6469  com/thevickypedi
+000010c0: 612f 7374 7265 7373 2d69 6e6a 6563 746f  a/stress-injecto
+000010d0: 722f 626c 6f62 2f6d 6169 6e2f 7374 7265  r/blob/main/stre
+000010e0: 7373 696e 6a65 6374 6f72 2f63 7075 2e70  ssinjector/cpu.p
+000010f0: 7922 3e43 5055 2053 7472 6573 733c 2f61  y">CPU Stress</a
+00001100: 3e3c 2f73 7472 6f6e 673e 3c2f 7375 6d6d  ></strong></summ
+00001110: 6172 793e 0a0a 2a20 546f 2061 6368 6965  ary>..* To achie
+00001120: 7665 2043 5055 2073 7472 6573 732c 2049  ve CPU stress, I
+00001130: 2068 6176 6520 7573 6564 206d 756c 7469   have used multi
+00001140: 7072 6f63 6573 732c 206c 6f6f 7065 6420  process, looped 
+00001150: 666f 7220 7468 6520 6e75 6d62 6572 206f  for the number o
+00001160: 6620 6c6f 6769 6361 6c20 636f 7265 732c  f logical cores,
+00001170: 2074 7269 6767 6572 696e 6720 616e 2069   triggering an i
+00001180: 6e66 696e 6974 6520 6c6f 6f70 206f 6e0a  nfinite loop on.
+00001190: 2020 6561 6368 2063 6f72 652e 0a2a 2054    each core..* T
+000011a0: 6865 2069 6e66 696e 6974 6520 6c6f 6f70  he infinite loop
+000011b0: 2077 696c 6c20 7275 6e20 666f 7220 6120   will run for a 
+000011c0: 6769 7665 6e20 6e75 6d62 6572 206f 6620  given number of 
+000011d0: 7365 636f 6e64 7320 2870 726f 7669 6465  seconds (provide
+000011e0: 6420 6279 2074 6865 2075 7365 7229 0a2a  d by the user).*
+000011f0: 204d 6561 6e2d 7768 696c 6520 7468 6520   Mean-while the 
+00001200: 6063 7075 5f70 6572 6365 6e74 6020 6672  `cpu_percent` fr
+00001210: 6f6d 2060 7073 7574 696c 6020 7275 6e73  om `psutil` runs
+00001220: 2028 696e 2061 2064 6564 6963 6174 6564   (in a dedicated
+00001230: 2074 6872 6561 6429 2069 6e20 616e 2069   thread) in an i
+00001240: 6e66 696e 6974 6520 6c6f 6f70 2063 616c  nfinite loop cal
+00001250: 6375 6c61 7469 6e67 2074 6865 2063 7572  culating the cur
+00001260: 7265 6e74 2043 5055 200a 2020 7574 696c  rent CPU .  util
+00001270: 697a 6174 696f 6e20 6f6e 2065 6163 6820  ization on each 
+00001280: 4350 5520 636f 7265 2e0a 2a20 5468 6520  CPU core..* The 
+00001290: 6465 6469 6361 7465 6420 7468 7265 6164  dedicated thread
+000012a0: 2072 756e 7320 666f 7220 3320 7365 636f   runs for 3 seco
+000012b0: 6e64 7320 696e 2061 6464 6974 696f 6e20  nds in addition 
+000012c0: 746f 2074 6865 206e 756d 6265 7220 6f66  to the number of
+000012d0: 2073 6563 6f6e 6473 2070 726f 7669 6465   seconds provide
+000012e0: 6420 6279 2074 6865 2075 7365 722e 0a2a  d by the user..*
+000012f0: 204f 6e63 6520 7468 6520 6769 7665 6e20   Once the given 
+00001300: 6e75 6d62 6572 206f 6620 7365 636f 6e64  number of second
+00001310: 7320 6861 7665 2070 6173 7365 642c 2074  s have passed, t
+00001320: 6865 2060 7072 6f63 6573 7365 7360 2061  he `processes` a
+00001330: 6e64 2060 7468 7265 6164 7360 2069 6e69  nd `threads` ini
+00001340: 7469 6174 6564 2074 6f20 6d6f 6e69 746f  tiated to monito
+00001350: 7220 4350 5520 7573 6167 6520 6172 6520  r CPU usage are 
+00001360: 7374 6f70 7065 642e 0a3c 2f64 6574 6169  stopped..</detai
+00001370: 6c73 3e0a 3c62 723e 0a3c 6465 7461 696c  ls>.<br>.<detail
+00001380: 733e 0a3c 7375 6d6d 6172 793e 3c73 7472  s>.<summary><str
+00001390: 6f6e 673e 496e 7369 6768 7473 2061 626f  ong>Insights abo
+000013a0: 7574 203c 6120 6872 6566 3d22 6874 7470  ut <a href="http
+000013b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
+000013c0: 6865 7669 636b 7970 6564 6961 2f73 7472  hevickypedia/str
+000013d0: 6573 732d 696e 6a65 6374 6f72 2f62 6c6f  ess-injector/blo
+000013e0: 622f 6d61 696e 2f73 7472 6573 7369 6e6a  b/main/stressinj
+000013f0: 6563 746f 722f 6d65 6d6f 7279 2e70 7922  ector/memory.py"
+00001400: 3e4d 656d 6f72 7920 5374 7265 7373 3c2f  >Memory Stress</
+00001410: 613e 3c2f 7374 726f 6e67 3e3c 2f73 756d  a></strong></sum
+00001420: 6d61 7279 3e0a 0a2a 2049 6e20 7468 6973  mary>..* In this
+00001430: 2073 6372 6970 742c 2049 2068 6176 6520   script, I have 
+00001440: 7573 6564 2060 6e75 6d70 792e 7261 6e64  used `numpy.rand
+00001450: 6f6d 2e62 7974 6573 6020 7768 6963 6820  om.bytes` which 
+00001460: 6172 6520 7361 6d70 6c65 6420 6672 6f6d  are sampled from
+00001470: 2075 6e69 666f 726d 2064 6973 7472 6962   uniform distrib
+00001480: 7574 696f 6e2e 0a2a 2054 6865 7365 2072  ution..* These r
+00001490: 616e 646f 6d20 6279 7465 7320 6172 6520  andom bytes are 
+000014a0: 636f 6c6c 6563 7465 6420 6672 6f6d 2074  collected from t
+000014b0: 6865 206d 6163 6869 6e65 2773 2070 6879  he machine's phy
+000014c0: 7369 6361 6c20 6d65 6d6f 7279 2069 6e63  sical memory inc
+000014d0: 7265 6173 696e 6720 7468 6520 7072 6f67  reasing the prog
+000014e0: 7261 6d27 7320 7573 6167 652e 0a2a 2049  ram's usage..* I
+000014f0: 2068 6176 6520 7468 656e 2075 7365 6420   have then used 
+00001500: 6067 6574 7275 7361 6765 6020 2867 6574  `getrusage` (get
+00001510: 2072 6573 6f75 7263 6520 7573 6167 6529   resource usage)
+00001520: 2066 6f72 2060 5345 4c46 6020 746f 2067   for `SELF` to g
+00001530: 6574 2074 6865 206d 656d 6f72 7920 636f  et the memory co
+00001540: 6e73 756d 6564 206f 6e6c 7920 6279 2074  nsumed only by t
+00001550: 6865 2063 7572 7265 6e74 2073 6372 6970  he current scrip
+00001560: 742e 0a2a 2054 6865 2060 7369 7a65 5f63  t..* The `size_c
+00001570: 6f6e 7665 7274 6572 6020 636f 6e76 6572  onverter` conver
+00001580: 7473 2074 6865 2062 7974 6573 2066 726f  ts the bytes fro
+00001590: 6d20 7265 736f 7572 6365 2075 7361 6765  m resource usage
+000015a0: 2074 6f20 6120 6875 6d61 6e20 756e 6465   to a human unde
+000015b0: 7273 7461 6e64 6162 6c65 2066 6f72 6d61  rstandable forma
+000015c0: 742e 0a3c 2f64 6574 6169 6c73 3e0a 3c62  t..</details>.<b
+000015d0: 723e 0a3c 6465 7461 696c 733e 0a3c 7375  r>.<details>.<su
+000015e0: 6d6d 6172 793e 3c73 7472 6f6e 673e 496e  mmary><strong>In
+000015f0: 7369 6768 7473 2061 626f 7574 203c 6120  sights about <a 
+00001600: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00001610: 7468 7562 2e63 6f6d 2f74 6865 7669 636b  thub.com/thevick
+00001620: 7970 6564 6961 2f73 7472 6573 732d 696e  ypedia/stress-in
+00001630: 6a65 6374 6f72 2f62 6c6f 622f 6d61 696e  jector/blob/main
+00001640: 2f73 7472 6573 7369 6e6a 6563 746f 722f  /stressinjector/
+00001650: 6f6e 7573 2e70 7922 3e55 524c 2053 7472  onus.py">URL Str
+00001660: 6573 733c 2f61 3e3c 2f73 7472 6f6e 673e  ess</a></strong>
+00001670: 3c2f 7375 6d6d 6172 793e 0a0a 2a20 496e  </summary>..* In
+00001680: 2074 6869 7320 7363 7269 7074 2c20 4920   this script, I 
+00001690: 6861 7665 2075 7365 6420 7468 7265 6164  have used thread
+000016a0: 706f 6f6c 7320 746f 206d 616b 6520 636f  pools to make co
+000016b0: 6e63 7572 7265 6e74 2072 6571 7565 7374  ncurrent request
+000016c0: 732e 0a2a 2054 6865 2073 6372 6970 7420  s..* The script 
+000016d0: 7573 6573 2060 7265 7175 6573 7473 6020  uses `requests` 
+000016e0: 6d6f 6475 6c65 2074 6f20 6d61 6b65 2063  module to make c
+000016f0: 616c 6c73 2e0a 2a20 5461 6b65 7320 6172  alls..* Takes ar
+00001700: 6775 6d65 6e74 730a 2020 2a20 2a2a 7261  guments.  * **ra
+00001710: 7465 2a2a 3a20 4e75 6d62 6572 206f 6620  te**: Number of 
+00001720: 6361 6c6c 7320 746f 206d 616b 652e 205f  calls to make. _
+00001730: 4465 6661 756c 7473 2074 6f20 3130 304b  Defaults to 100K
+00001740: 5f0a 2020 2a20 2a2a 7469 6d65 6f75 742a  _.  * **timeout*
+00001750: 2a3a 2054 696d 656f 7574 2066 6f72 2065  *: Timeout for e
+00001760: 6163 6820 7265 7175 6573 742e 205f 4465  ach request. _De
+00001770: 6661 756c 7473 2074 6f20 302e 355f 0a20  faults to 0.5_. 
+00001780: 202a 202a 2a72 6574 7279 5f6c 696d 6974   * **retry_limit
+00001790: 2a2a 3a20 5265 7472 7920 6c69 6d69 7420  **: Retry limit 
+000017a0: 6966 2074 6865 2073 7973 7465 6d20 6973  if the system is
+000017b0: 2075 6e61 626c 6520 746f 2073 7069 6e75   unable to spinu
+000017c0: 7020 6d6f 7265 2074 6872 6561 6473 2e20  p more threads. 
+000017d0: 5f44 6566 6175 6c74 7320 746f 2035 5f0a  _Defaults to 5_.
+000017e0: 2020 2a20 2a2a 6369 7263 7569 745f 6272    * **circuit_br
+000017f0: 6561 6b2a 2a3a 2057 6169 7420 7469 6d65  eak**: Wait time
+00001800: 2069 6e20 7365 636f 6e64 7320 6265 7477   in seconds betw
+00001810: 6565 6e20 7265 7472 6965 732e 205f 4465  een retries. _De
+00001820: 6661 756c 7473 2074 6f20 355f 0a20 202a  faults to 5_.  *
+00001830: 202a 2a72 6571 7565 7374 5f74 7970 652a   **request_type*
+00001840: 2a3a 2046 756e 6374 696f 6e20 6672 6f6d  *: Function from
+00001850: 2060 7265 7175 6573 7473 6020 6d6f 6475   `requests` modu
+00001860: 6c65 2e0a 0a3c 2f64 6574 6169 6c73 3e0a  le...</details>.
+00001870: 0a23 2323 2055 7361 6765 0a60 7069 7020  .### Usage.`pip 
+00001880: 696e 7374 616c 6c20 7374 7265 7373 2d69  install stress-i
+00001890: 6e6a 6563 746f 7260 0a0a 5b43 5055 2053  njector`..[CPU S
+000018a0: 7472 6573 735d 2868 7474 7073 3a2f 2f67  tress](https://g
+000018b0: 6974 6875 622e 636f 6d2f 7468 6576 6963  ithub.com/thevic
+000018c0: 6b79 7065 6469 612f 7374 7265 7373 2d69  kypedia/stress-i
+000018d0: 6e6a 6563 746f 722f 626c 6f62 2f6d 6169  njector/blob/mai
+000018e0: 6e2f 7374 7265 7373 696e 6a65 6374 6f72  n/stressinjector
+000018f0: 2f63 7075 2e70 7929 0a60 6060 7079 7468  /cpu.py).```pyth
+00001900: 6f6e 0a69 6d70 6f72 7420 7374 7265 7373  on.import stress
+00001910: 696e 6a65 6374 6f72 2061 7320 696e 6a65  injector as inje
+00001920: 6374 6f72 0a0a 0a69 6620 5f5f 6e61 6d65  ctor...if __name
+00001930: 5f5f 203d 3d20 275f 5f6d 6169 6e5f 5f27  __ == '__main__'
+00001940: 3a0a 2020 2020 696e 6a65 6374 6f72 2e43  :.    injector.C
+00001950: 5055 5374 7265 7373 2873 6563 6f6e 6473  PUStress(seconds
+00001960: 3d33 3030 290a 6060 600a 0a5b 4d65 6d6f  =300).```..[Memo
+00001970: 7279 2053 7472 6573 735d 2868 7474 7073  ry Stress](https
+00001980: 3a2f 2f67 6974 6875 622e 636f 6d2f 7468  ://github.com/th
+00001990: 6576 6963 6b79 7065 6469 612f 7374 7265  evickypedia/stre
+000019a0: 7373 2d69 6e6a 6563 746f 722f 626c 6f62  ss-injector/blob
+000019b0: 2f6d 6169 6e2f 7374 7265 7373 696e 6a65  /main/stressinje
+000019c0: 6374 6f72 2f6d 656d 6f72 792e 7079 290a  ctor/memory.py).
+000019d0: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
+000019e0: 2073 7472 6573 7369 6e6a 6563 746f 7220   stressinjector 
+000019f0: 6173 2069 6e6a 6563 746f 720a 0a0a 6966  as injector...if
+00001a00: 205f 5f6e 616d 655f 5f20 3d3d 2027 5f5f   __name__ == '__
+00001a10: 6d61 696e 5f5f 273a 0a20 2020 2069 6e6a  main__':.    inj
+00001a20: 6563 746f 722e 4d65 6d6f 7279 5374 7265  ector.MemoryStre
+00001a30: 7373 2867 6967 6162 7974 6573 3d32 5f30  ss(gigabytes=2_0
+00001a40: 3030 290a 6060 600a 0a5b 5552 4c20 5374  00).```..[URL St
+00001a50: 7265 7373 5d28 6874 7470 733a 2f2f 6769  ress](https://gi
+00001a60: 7468 7562 2e63 6f6d 2f74 6865 7669 636b  thub.com/thevick
+00001a70: 7970 6564 6961 2f73 7472 6573 732d 696e  ypedia/stress-in
+00001a80: 6a65 6374 6f72 2f62 6c6f 622f 6d61 696e  jector/blob/main
+00001a90: 2f73 7472 6573 7369 6e6a 6563 746f 722f  /stressinjector/
+00001aa0: 7572 6c2e 7079 290a 6060 6070 7974 686f  url.py).```pytho
+00001ab0: 6e0a 696d 706f 7274 206f 730a 696d 706f  n.import os.impo
+00001ac0: 7274 2073 7472 6573 7369 6e6a 6563 746f  rt stressinjecto
+00001ad0: 7220 6173 2069 6e6a 6563 746f 720a 0a0a  r as injector...
+00001ae0: 6966 205f 5f6e 616d 655f 5f20 3d3d 2027  if __name__ == '
+00001af0: 5f5f 6d61 696e 5f5f 273a 0a20 2020 2069  __main__':.    i
+00001b00: 6e6a 6563 746f 722e 5552 4c53 7472 6573  njector.URLStres
+00001b10: 7328 7572 6c3d 2768 7474 703a 2f2f 302e  s(url='http://0.
+00001b20: 302e 302e 303a 3530 3032 2f27 2920 2023  0.0.0:5002/')  #
+00001b30: 2053 7472 6573 7320 7465 7374 2047 4554   Stress test GET
+00001b40: 2063 616c 6c73 0a0a 2020 2020 2320 5374   calls..    # St
+00001b50: 7265 7373 2074 6573 7420 504f 5354 2063  ress test POST c
+00001b60: 616c 6c73 2c20 616c 736f 2073 7570 706f  alls, also suppo
+00001b70: 7274 7320 5055 542c 2061 6e64 2044 454c  rts PUT, and DEL
+00001b80: 4554 450a 2020 2020 7361 6d70 6c65 5f64  ETE.    sample_d
+00001b90: 6174 6120 3d20 7b27 6865 6164 6572 7327  ata = {'headers'
+00001ba0: 3a20 7b27 4175 7468 6f72 697a 6174 696f  : {'Authorizatio
+00001bb0: 6e27 3a20 2742 6561 7265 7220 2573 2720  n': 'Bearer %s' 
+00001bc0: 2520 6f73 2e65 6e76 6972 6f6e 2e67 6574  % os.environ.get
+00001bd0: 2827 544f 4b45 4e27 297d 7d0a 2020 2020  ('TOKEN')}}.    
+00001be0: 696e 6a65 6374 6f72 2e55 524c 5374 7265  injector.URLStre
+00001bf0: 7373 280a 2020 2020 2020 7572 6c3d 2768  ss(.      url='h
+00001c00: 7474 703a 2f2f 302e 302e 302e 303a 3530  ttp://0.0.0.0:50
+00001c10: 3032 2f27 2c0a 2020 2020 2020 7265 7175  02/',.      requ
+00001c20: 6573 745f 7479 7065 3d69 6e6a 6563 746f  est_type=injecto
+00001c30: 722e 5265 7175 6573 7454 7970 652e 706f  r.RequestType.po
+00001c40: 7374 2c0a 2020 2020 2020 2a2a 7361 6d70  st,.      **samp
+00001c50: 6c65 5f64 6174 610a 2020 2020 290a 6060  le_data.    ).``
+00001c60: 600a 3e20 5468 6973 206d 6f64 756c 6520  `.> This module 
+00001c70: 6361 6e20 6f6e 6c79 2069 6e64 7563 6520  can only induce 
+00001c80: 7374 7265 7373 206f 6e20 6120 6769 7665  stress on a give
+00001c90: 6e20 5552 4c20 6279 206d 616b 696e 6720  n URL by making 
+00001ca0: 4e20 6e75 6d62 6572 206f 6620 6361 6c6c  N number of call
+00001cb0: 732e 2053 7569 7461 626c 6520 666f 7220  s. Suitable for 
+00001cc0: 4150 4973 2072 756e 6e69 6e67 206f 6e20  APIs running on 
+00001cd0: 6c6f 6361 6c68 6f73 742e 0a3e 200a 3e20  localhost..> .> 
+00001ce0: 546f 2070 6572 666f 726d 2061 2072 6561  To perform a rea
+00001cf0: 6c2d 7469 6d65 206c 6f61 6420 7465 7374  l-time load test
+00001d00: 2c20 7265 6665 7220 5b6c 6f63 7573 742e  , refer [locust.
+00001d10: 696f 5d28 6874 7470 733a 2f2f 6c6f 6375  io](https://locu
+00001d20: 7374 2e69 6f2f 290a 0a23 2323 2320 436f  st.io/)..#### Co
+00001d30: 6469 6e67 2053 7461 6e64 6172 6473 0a44  ding Standards.D
+00001d40: 6f63 7374 7269 6e67 2066 6f72 6d61 743a  ocstring format:
+00001d50: 205b 6047 6f6f 676c 6560 5d28 6874 7470   [`Google`](http
+00001d60: 733a 2f2f 676f 6f67 6c65 2e67 6974 6875  s://google.githu
+00001d70: 622e 696f 2f73 7479 6c65 6775 6964 652f  b.io/styleguide/
+00001d80: 7079 6775 6964 652e 6874 6d6c 2333 382d  pyguide.html#38-
+00001d90: 636f 6d6d 656e 7473 2d61 6e64 2d64 6f63  comments-and-doc
+00001da0: 7374 7269 6e67 7329 203c 6272 3e0a 5374  strings) <br>.St
+00001db0: 796c 696e 6720 636f 6e76 656e 7469 6f6e  yling convention
+00001dc0: 733a 205b 6050 4550 2038 605d 2868 7474  s: [`PEP 8`](htt
+00001dd0: 7073 3a2f 2f77 7777 2e70 7974 686f 6e2e  ps://www.python.
+00001de0: 6f72 672f 6465 762f 7065 7073 2f70 6570  org/dev/peps/pep
+00001df0: 2d30 3030 382f 2920 3c62 723e 0a43 6c65  -0008/) <br>.Cle
+00001e00: 616e 2063 6f64 6520 7769 7468 2070 7265  an code with pre
+00001e10: 2d63 6f6d 6d69 7420 686f 6f6b 733a 205b  -commit hooks: [
+00001e20: 6066 6c61 6b65 3860 5d28 6874 7470 733a  `flake8`](https:
+00001e30: 2f2f 666c 616b 6538 2e70 7963 7161 2e6f  //flake8.pycqa.o
+00001e40: 7267 2f65 6e2f 6c61 7465 7374 2f29 2061  rg/en/latest/) a
+00001e50: 6e64 200a 5b60 6973 6f72 7460 5d28 6874  nd .[`isort`](ht
+00001e60: 7470 733a 2f2f 7079 6371 612e 6769 7468  tps://pycqa.gith
+00001e70: 7562 2e69 6f2f 6973 6f72 742f 290a 0a23  ub.io/isort/)..#
+00001e80: 2323 2320 5b52 656c 6561 7365 204e 6f74  ### [Release Not
+00001e90: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
+00001ea0: 7562 2e63 6f6d 2f74 6865 7669 636b 7970  ub.com/thevickyp
+00001eb0: 6564 6961 2f73 7472 6573 732d 696e 6a65  edia/stress-inje
+00001ec0: 6374 6f72 2f62 6c6f 622f 6d61 696e 2f72  ctor/blob/main/r
+00001ed0: 656c 6561 7365 5f6e 6f74 6573 2e72 7374  elease_notes.rst
+00001ee0: 290a 2a2a 5265 7175 6972 656d 656e 742a  ).**Requirement*
+00001ef0: 2a0a 6060 6073 6865 6c6c 0a70 7974 686f  *.```shell.pytho
+00001f00: 6e20 2d6d 2070 6970 2069 6e73 7461 6c6c  n -m pip install
+00001f10: 2063 6861 6e67 656c 6f67 2d67 656e 6572   changelog-gener
+00001f20: 6174 6f72 0a60 6060 0a0a 2a2a 5573 6167  ator.```..**Usag
+00001f30: 652a 2a0a 6060 6073 6865 6c6c 0a63 6861  e**.```shell.cha
+00001f40: 6e67 656c 6f67 2072 6576 6572 7365 202d  ngelog reverse -
+00001f50: 6620 7265 6c65 6173 655f 6e6f 7465 732e  f release_notes.
+00001f60: 7273 7420 2d74 2027 5265 6c65 6173 6520  rst -t 'Release 
+00001f70: 4e6f 7465 7327 0a60 6060 0a0a 2323 2323  Notes'.```..####
+00001f80: 204c 696e 7469 6e67 0a60 5072 6543 6f6d   Linting.`PreCom
+00001f90: 6d69 7460 2077 696c 6c20 656e 7375 7265  mit` will ensure
+00001fa0: 206c 696e 7469 6e67 2c20 616e 6420 7468   linting, and th
+00001fb0: 6520 646f 6320 6372 6561 7469 6f6e 2061  e doc creation a
+00001fc0: 7265 2072 756e 206f 6e20 6576 6572 7920  re run on every 
+00001fd0: 636f 6d6d 6974 2e0a 0a2a 2a52 6571 7569  commit...**Requi
+00001fe0: 7265 6d65 6e74 2a2a 0a3c 6272 3e0a 6060  rement**.<br>.``
+00001ff0: 6062 6173 680a 7069 7020 696e 7374 616c  `bash.pip instal
+00002000: 6c20 2d2d 6e6f 2d63 6163 6865 2073 7068  l --no-cache sph
+00002010: 696e 783d 3d35 2e31 2e31 2070 7265 2d63  inx==5.1.1 pre-c
+00002020: 6f6d 6d69 7420 7265 636f 6d6d 6f6e 6d61  ommit recommonma
+00002030: 726b 0a60 6060 0a0a 2a2a 5573 6167 652a  rk.```..**Usage*
+00002040: 2a0a 3c62 723e 0a60 6060 6261 7368 0a70  *.<br>.```bash.p
+00002050: 7265 2d63 6f6d 6d69 7420 7275 6e20 2d2d  re-commit run --
+00002060: 616c 6c2d 6669 6c65 730a 6060 600a 0a23  all-files.```..#
+00002070: 2323 2050 7970 6920 5061 636b 6167 650a  ## Pypi Package.
+00002080: 5b21 5b70 7970 692d 6d6f 6475 6c65 5d28  [![pypi-module](
+00002090: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000020a0: 6c64 732e 696f 2f62 6164 6765 2f53 6f66  lds.io/badge/Sof
+000020b0: 7477 6172 6525 3230 5265 706f 7369 746f  tware%20Reposito
+000020c0: 7279 2d70 7970 692d 3166 3432 3566 2e73  ry-pypi-1f425f.s
+000020d0: 7667 295d 2868 7474 7073 3a2f 2f70 6163  vg)](https://pac
+000020e0: 6b61 6769 6e67 2e70 7974 686f 6e2e 6f72  kaging.python.or
+000020f0: 672f 7475 746f 7269 616c 732f 7061 636b  g/tutorials/pack
+00002100: 6167 696e 672d 7072 6f6a 6563 7473 2f29  aging-projects/)
+00002110: 0a0a 5b68 7474 7073 3a2f 2f70 7970 692e  ..[https://pypi.
+00002120: 6f72 672f 7072 6f6a 6563 742f 7374 7265  org/project/stre
+00002130: 7373 2d69 6e6a 6563 746f 722f 5d28 6874  ss-injector/](ht
+00002140: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+00002150: 726f 6a65 6374 2f73 7472 6573 732d 696e  roject/stress-in
+00002160: 6a65 6374 6f72 2f29 0a0a 2323 2320 5275  jector/)..### Ru
+00002170: 6e62 6f6f 6b0a 5b21 5b6d 6164 652d 7769  nbook.[![made-wi
+00002180: 7468 2d73 7068 696e 782d 646f 635d 2868  th-sphinx-doc](h
+00002190: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000021a0: 6473 2e69 6f2f 6261 6467 652f 436f 6465  ds.io/badge/Code
+000021b0: 2532 3044 6f63 732d 5370 6869 6e78 2d31  %20Docs-Sphinx-1
+000021c0: 6634 3235 662e 7376 6729 5d28 6874 7470  f425f.svg)](http
+000021d0: 733a 2f2f 7777 772e 7370 6869 6e78 2d64  s://www.sphinx-d
+000021e0: 6f63 2e6f 7267 2f65 6e2f 6d61 7374 6572  oc.org/en/master
+000021f0: 2f6d 616e 2f73 7068 696e 782d 6175 746f  /man/sphinx-auto
+00002200: 6765 6e2e 6874 6d6c 290a 0a5b 6874 7470  gen.html)..[http
+00002210: 733a 2f2f 7468 6576 6963 6b79 7065 6469  s://thevickypedi
+00002220: 612e 6769 7468 7562 2e69 6f2f 7374 7265  a.github.io/stre
+00002230: 7373 2d69 6e6a 6563 746f 722f 5d28 6874  ss-injector/](ht
+00002240: 7470 733a 2f2f 7468 6576 6963 6b79 7065  tps://thevickype
+00002250: 6469 612e 6769 7468 7562 2e69 6f2f 7374  dia.github.io/st
+00002260: 7265 7373 2d69 6e6a 6563 746f 722f 290a  ress-injector/).
+00002270: 0a23 2320 4c69 6365 6e73 6520 2620 636f  .## License & co
+00002280: 7079 7269 6768 740a 0a26 636f 7079 3b20  pyright..&copy; 
+00002290: 5669 676e 6573 6820 5369 7661 6e61 6e64  Vignesh Sivanand
+000022a0: 6861 2052 616f 0a0a 4c69 6365 6e73 6564  ha Rao..Licensed
+000022b0: 2075 6e64 6572 2074 6865 205b 4d49 5420   under the [MIT 
+000022c0: 4c69 6365 6e73 655d 2868 7474 7073 3a2f  License](https:/
+000022d0: 2f67 6974 6875 622e 636f 6d2f 7468 6576  /github.com/thev
+000022e0: 6963 6b79 7065 6469 612f 7374 7265 7373  ickypedia/stress
+000022f0: 2d69 6e6a 6563 746f 722f 626c 6f62 2f6d  -injector/blob/m
+00002300: 6169 6e2f 4c49 4345 4e53 4529 0a         ain/LICENSE).
```

