# Comparing `tmp/stress_injector-0.4a0-py3-none-any.whl.zip` & `tmp/stress_injector-0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 12493 bytes, number of entries: 12
--rw-r--r--  2.0 unx      189 b- defN 23-Apr-14 02:34 stressinjector/__init__.py
--rw-r--r--  2.0 unx     4767 b- defN 23-Apr-14 02:34 stressinjector/cpu.py
--rw-r--r--  2.0 unx     2997 b- defN 23-Apr-14 02:34 stressinjector/echo.py
--rw-r--r--  2.0 unx     4565 b- defN 23-Apr-14 02:34 stressinjector/memory.py
--rw-r--r--  2.0 unx      838 b- defN 23-Apr-14 02:34 stressinjector/models.py
--rw-r--r--  2.0 unx       40 b- defN 23-Apr-14 02:34 stressinjector/requirements.txt
--rw-r--r--  2.0 unx     4664 b- defN 23-Apr-14 02:34 stressinjector/url.py
--rw-r--r--  2.0 unx     1078 b- defN 23-Apr-14 02:34 stress_injector-0.4a0.dist-info/LICENSE
--rw-r--r--  2.0 unx     7808 b- defN 23-Apr-14 02:34 stress_injector-0.4a0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 02:34 stress_injector-0.4a0.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Apr-14 02:34 stress_injector-0.4a0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      990 b- defN 23-Apr-14 02:34 stress_injector-0.4a0.dist-info/RECORD
-12 files, 28043 bytes uncompressed, 10823 bytes compressed:  61.4%
+Zip file size: 13033 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      248 b- defN 23-Apr-16 17:33 stressinjector/__init__.py
+-rw-r--r--  2.0 unx     4788 b- defN 23-Apr-16 17:33 stressinjector/cpu.py
+-rw-r--r--  2.0 unx     2997 b- defN 23-Apr-16 17:33 stressinjector/echo.py
+-rw-r--r--  2.0 unx     4586 b- defN 23-Apr-16 17:33 stressinjector/memory.py
+-rw-r--r--  2.0 unx     1285 b- defN 23-Apr-16 17:33 stressinjector/models.py
+-rw-r--r--  2.0 unx       49 b- defN 23-Apr-16 17:33 stressinjector/requirements.txt
+-rw-r--r--  2.0 unx     5442 b- defN 23-Apr-16 17:33 stressinjector/url.py
+-rw-r--r--  2.0 unx     1078 b- defN 23-Apr-16 17:34 stress_injector-0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8520 b- defN 23-Apr-16 17:34 stress_injector-0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-16 17:34 stress_injector-0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Apr-16 17:34 stress_injector-0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      981 b- defN 23-Apr-16 17:34 stress_injector-0.5.dist-info/RECORD
+12 files, 30081 bytes uncompressed, 11383 bytes compressed:  62.2%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: stressinjector/requirements.txt
 Comment: 
 
 Filename: stressinjector/url.py
 Comment: 
 
-Filename: stress_injector-0.4a0.dist-info/LICENSE
+Filename: stress_injector-0.5.dist-info/LICENSE
 Comment: 
 
-Filename: stress_injector-0.4a0.dist-info/METADATA
+Filename: stress_injector-0.5.dist-info/METADATA
 Comment: 
 
-Filename: stress_injector-0.4a0.dist-info/WHEEL
+Filename: stress_injector-0.5.dist-info/WHEEL
 Comment: 
 
-Filename: stress_injector-0.4a0.dist-info/top_level.txt
+Filename: stress_injector-0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: stress_injector-0.4a0.dist-info/RECORD
+Filename: stress_injector-0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## stressinjector/__init__.py

```diff
@@ -1,5 +1,6 @@
 from stressinjector.cpu import CPUStress  # noqa: F401
 from stressinjector.memory import MemoryStress  # noqa: F401
+from stressinjector.models import RequestType  # noqa: F401
 from stressinjector.url import URLStress  # noqa: F401
 
-version = "0.4a"
+version = "0.5"
```

## stressinjector/cpu.py

```diff
@@ -35,14 +35,15 @@
     """
 
     CORES = os.cpu_count()
 
     def __init__(self, seconds: int = CORES * 5):
         self.seconds = seconds
         self.start_time = None
+        self._run()
 
     def _infinite(self) -> None:
         """Infinite loop to stress each core on the CPU for the number of logical cores available.
 
         See Also:
             The loop runs on each core as this function is triggered by ``processing.Process`` that runs as a loop.
         """
@@ -95,15 +96,15 @@
 
         Returns:
             int:
             Processed integers without any float value extensions in it.
         """
         return int(n) if isinstance(n, float) and n.is_integer() else n
 
-    def run(self) -> None:
+    def _run(self) -> None:
         """Initiator for stress injector.
 
         Methods:
             infinite: To kick off stress injector.
             measure: To measure the usage in the background running in a dedicated thread.
         """
         # noinspection PyGlobalUndefined
```

## stressinjector/memory.py

```diff
@@ -54,14 +54,15 @@
             Converts ``bytes`` to human-readable size format.
     """
 
     MAX_DEFAULT = round(float(_size_converter(psutil.virtual_memory().total).split()[0]) * 2)
 
     def __init__(self, gigabytes: int = MAX_DEFAULT):
         self.gigabytes = gigabytes
+        self._run()
 
     @classmethod
     def _stress(cls, mb: int) -> str:
         """Generates `random bytes <https://numpy.org/doc/stable/reference/random/generated/numpy.random.bytes.html>`__.
 
         Bytes are generated with the multiple of 1024 ~ 1GB. Uses tqdm module to show a progress bar.
 
@@ -100,15 +101,15 @@
         if settings.os == operating_system.macOS:
             return resource.getrusage(resource.RUSAGE_SELF).ru_maxrss
         if settings.os == operating_system.linux:
             return resource.getrusage(resource.RUSAGE_SELF).ru_maxrss * 1e+3
         if settings.os == operating_system.windows:
             return psutil.Process(settings.pid).memory_info().peak_wset
 
-    def run(self) -> None:
+    def _run(self) -> None:
         """Initiator for stress injector. Converts GigaBytes to Bytes.
 
         Methods:
             stress: To kick off stress injector with the desired bytes converted from user input.
             memory_util_check: To measure the usage post completion.
         """
         megabytes = int(self.gigabytes) * 1024  # gigabytes to megabytes
```

## stressinjector/models.py

```diff
@@ -1,15 +1,19 @@
 import logging
 import os
 import platform
 from enum import Enum
 
 LOGGER = logging.getLogger(__name__)
-LOGGER.addHandler(logging.StreamHandler())
-LOGGER.setLevel(logging.DEBUG)
+DEFAULT_LOG_FORM = '%(asctime)s - %(levelname)s - [%(processName)s:%(module)s:%(lineno)d] - %(funcName)s - %(message)s'
+DEFAULT_FORMATTER = logging.Formatter(datefmt='%b-%d-%Y %I:%M:%S %p', fmt=DEFAULT_LOG_FORM)
+HANDLER = logging.StreamHandler()
+HANDLER.setFormatter(fmt=DEFAULT_FORMATTER)
+LOGGER.addHandler(hdlr=HANDLER)
+LOGGER.setLevel(level=logging.DEBUG)
 
 
 class UnsupportedOS(OSError):
     """Custom OSError for unsupported operating system."""
 
 
 class OperatingSystem(str, Enum):
@@ -29,11 +33,20 @@
     pid: int = os.getpid()
     os: str = platform.system()
 
 
 settings = Settings
 
 
+class RequestType(str, Enum):
+    """Wrapper for request types."""
+
+    get: str = "get"
+    put: str = "put"
+    post: str = "post"
+    delete: str = "delete"
+
+
 _supported_systems = (operating_system.macOS, operating_system.linux, operating_system.windows)
 
 if settings.os not in _supported_systems:
     raise UnsupportedOS(f"\n\ncurrently supported only on {', '.join(_supported_systems)}\n")
```

## stressinjector/requirements.txt

```diff
@@ -1,3 +1,4 @@
 numpy>=1.20.0
 psutil>=5.9.0
-tqdm>=4.56.0
+tqdm>=4.56.0
+requests
```

## stressinjector/url.py

```diff
@@ -1,113 +1,130 @@
-import http.client
 import logging
 import time
-import urllib.error
 import urllib.parse
-import urllib.request
 import warnings
 from concurrent.futures import ThreadPoolExecutor, as_completed
+from threading import Event
 from typing import NoReturn, Union
 
-from .models import LOGGER
+import requests
+
+from .models import LOGGER, RequestType
 
 RESULT = {'success': 0, 'errors': 0}
+event = Event()
 
 
 class URLStress:
     """Controller for URL stress using threadpool. Gets url as input.
 
     >>> URLStress
 
     """
 
-    def __init__(self, url: str, rate: int = 1e+5, timeout: Union[int, float] = 5e-1,
-                 retry_limit: Union[int, float] = 5, circuit_break: Union[int, float] = 5,
-                 logger: logging.Logger = None, **kwargs):
+    def __init__(self, url: str, rate: int = 1e+5, timeout: Union[int, float] = None,
+                 logger: logging.Logger = None, request_type: str = RequestType.get,
+                 **kwargs):
         """Instantiate the object, parse and validate the URL.
 
         Args:
             url: URL to inject stress.
             rate: Number of calls to make.
             timeout: Timeout for each request.
             retry_limit: Retry limit if the system is unable to spinup more threads.
             circuit_break: Wait time in seconds between retries.
+            logger: Custom logger.
+            request_type: Function from ``requests`` module.
             kwargs: Keyword arguments to use in the request.
         """
         self.parsed = urllib.parse.urlparse(url=url, allow_fragments=True)
-        if self.parsed.scheme not in ('http', 'https', 'ws'):
+        if self.parsed.scheme not in ('http', 'https', 'ws', 'ftp', 'tcp', 'udp', 'ssh',
+                                      'gopher', 'mailto', 'news', 'telnet', 'file', 'nntp', 'wais'):
             raise ValueError(
                 f"\n\nbad url: {url}\n{self.parsed.scheme}"
             )
+        if request_type not in RequestType.__members__.keys():
+            raise ValueError(
+                f"\n\nbad request type: {request_type}\n\nallowed: {', '.join(RequestType.__members__.keys())}"
+            )
         self.LOGGER = logger or LOGGER
         self.request_url = url
         self.request_rate = int(rate)
         self.timeout = timeout
-        self.retry_limit = retry_limit
-        self.circuit_break = circuit_break
         self.kwargs = kwargs or {}
+        self.request_type = request_type
+        self._run()
 
     def make_request(self, sample: bool = False) -> NoReturn:
         """Makes a GET request to the endpoint.
 
         Args:
             sample: Boolean flag to indicate if the request is sample.
         """
+        if event.is_set():
+            return
         if sample:
-            response: http.client.HTTPResponse = urllib.request.urlopen(url=self.request_url, timeout=self.timeout,
-                                                                        **self.kwargs)
+            response = requests.request(method=self.request_type.lower(), url=self.request_url, **self.kwargs)
         else:
-            response: http.client.HTTPResponse = urllib.request.urlopen(url=self.request_url, **self.kwargs)
-        response_code = response.getcode()
-        if 200 <= response_code <= 399:
+            response = requests.request(method=self.request_type.lower(), url=self.request_url,
+                                        timeout=self.timeout, **self.kwargs)
+        if response.ok:
             return
         else:
-            raise urllib.error.HTTPError(code=response_code, url=response.geturl(),
-                                         msg=response.msg.__str__(), hdrs=response.headers, fp=response.fp)
+            response.raise_for_status()
+
+    def initiate_injection(self) -> bool:
+        """Initiates injection in a thread pool.
 
-    def initiate_injection(self) -> NoReturn:
-        """Initiates injection in a thread pool."""
+        Returns:
+            bool:
+            Returns a boolean flag based on successful completion.
+        """
         futures = {}
-        retries = 0
         executor = ThreadPoolExecutor(max_workers=self.request_rate)
         with executor:
             for iterator in range(1, int(self.request_rate) + 1):
                 try:
                     future = executor.submit(self.make_request)
-                except RuntimeError:
-                    retries += 1
-                    if retries > self.retry_limit:
-                        self.LOGGER.error("Retry limit reached.")
-                        break
-                    self.LOGGER.warning("Hit rate limit. Awaiting 5 seconds before retry.")
-                    time.sleep(self.circuit_break)
-                    continue
-                futures[future] = iterator
+                    futures[future] = iterator
+                except RuntimeError as error:
+                    self.LOGGER.error(error)
+                    self.LOGGER.warning("cancelling future tasks")
+                    future.cancel()
+                    event.set()
+                    total = len(futures)
+                    returned = sum(RESULT.values())
+                    self.LOGGER.warning("calls made: %d", f'{total:,}')
+                    self.LOGGER.warning("calls completed: %d", f'{returned:,}')
+                    self.LOGGER.warning("calls pending: %d", f'{total - returned:,}')
+                    self.LOGGER.warning("awaiting pending tasks to complete")
+                    return False
         for future in as_completed(futures):
             if future.exception():
-                self.LOGGER.error(f'Thread processing for {iterator!r} received an exception: {future.exception()}')
+                self.LOGGER.error("thread processing for '%s' received an exception: '%s'",
+                                  iterator, future.exception())
                 RESULT['errors'] += 1
             else:
                 RESULT['success'] += 1
+        return True
 
-    def run(self) -> NoReturn:
+    def _run(self) -> NoReturn:
         """Runs initiate request injection and prints success and error count."""
         try:
+            self.LOGGER.info("Initiating sample call")
             self.make_request(sample=True)  # at least one request should pass before initiating request injection
+            self.LOGGER.info("Sample call successful")
         except Exception as error:
             warnings.warn(
                 f"\n{error.__str__()}\n\ntest call failed, cannot proceed stress testing\n"
             )
             return
         self.LOGGER.info("Running request injection on '%s' with rate %s", self.parsed.netloc, f'{self.request_rate:,}')
-        time.sleep(3)
         start = time.time()
-        self.initiate_injection()
+        run_assert = self.initiate_injection()
         self.LOGGER.info("Request injection completed in %f seconds", round(float(time.time() - start), 2))
-        assert RESULT['success'] + RESULT['errors'] == self.request_rate, "Not all request trails were successful"
         self.LOGGER.info("Total number of requests passed: %d", RESULT['success'])
         self.LOGGER.warning("Total number of requests failed: %d", RESULT['errors'])
-
-
-if __name__ == '__main__':
-    injector = URLStress(url="http://0.0.0.0:5002")
-    injector.run()
+        if run_assert:
+            assert sum(RESULT.values()) == self.request_rate, "Not all request trails were successful"
+        else:
+            self.LOGGER.warning("Total number of requests abandoned: %d", self.request_rate - sum(RESULT.values()))
```

## Comparing `stress_injector-0.4a0.dist-info/LICENSE` & `stress_injector-0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `stress_injector-0.4a0.dist-info/METADATA` & `stress_injector-0.5.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stress-injector
-Version: 0.4a0
+Version: 0.5
 Summary: Python module, to inject memory and CPU stress, and URL load test
 Author-email: Vignesh Sivanandha Rao <svignesh1793@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Vignesh Sivanandha Rao
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,14 +42,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy (>=1.20.0)
 Requires-Dist: psutil (>=5.9.0)
 Requires-Dist: tqdm (>=4.56.0)
+Requires-Dist: requests
 Provides-Extra: dev
 Requires-Dist: pre-commit ; extra == 'dev'
 
 [![Pypi-version](https://img.shields.io/pypi/v/stress-injector)](https://pypi.org/project/stress-injector)
 [![Pypi-py-version](https://img.shields.io/pypi/pyversions/stress-injector)](https://pypi.org/project/stress-injector)
 
 ![docs](https://github.com/thevickypedia/stress-injector/actions/workflows/docs.yml/badge.svg)
@@ -86,36 +87,62 @@
 * I have then used `getrusage` (get resource usage) for `SELF` to get the memory consumed only by the current script.
 * The `size_converter` converts the bytes from resource usage to a human understandable format.
 </details>
 <br>
 <details>
 <summary><strong>Insights about <a href="https://github.com/thevickypedia/stress-injector/blob/main/stressinjector/onus.py">URL Stress</a></strong></summary>
 
-* In this script, I have used threadpools to make concurrent GET requests.
-* The script uses builtin library `urllib` to make the GET calls.
+* In this script, I have used threadpools to make concurrent requests.
+* The script uses `requests` module to make calls.
 * Takes arguments
   * **rate**: Number of calls to make. _Defaults to 100K_
   * **timeout**: Timeout for each request. _Defaults to 0.5_
   * **retry_limit**: Retry limit if the system is unable to spinup more threads. _Defaults to 5_
   * **circuit_break**: Wait time in seconds between retries. _Defaults to 5_
+  * **request_type**: Function from `requests` module.
 
 </details>
 
 ### Usage
 `pip install stress-injector`
 
 [CPU Stress](https://github.com/thevickypedia/stress-injector/blob/main/stressinjector/cpu.py)
 ```python
 import stressinjector as injector
 
 
 if __name__ == '__main__':
-    injector.CPUStress(seconds=300).run()
+    injector.CPUStress(seconds=300)
+```
+
+[Memory Stress](https://github.com/thevickypedia/stress-injector/blob/main/stressinjector/memory.py)
+```python
+import stressinjector as injector
+
+
+if __name__ == '__main__':
     injector.MemoryStress(gigabytes=2_000).run()
-    injector.URLStress(url='http://0.0.0.0:5002/').run()
+```
+
+[URL Stress](https://github.com/thevickypedia/stress-injector/blob/main/stressinjector/url.py)
+```python
+import os
+import stressinjector as injector
+
+
+if __name__ == '__main__':
+    injector.URLStress(url='http://0.0.0.0:5002/')  # Stress test GET calls
+
+    # Stress test POST calls, also supports PUT, and DELETE
+    sample_data = {'headers': {'Authorization': 'Bearer %s' % os.environ.get('TOKEN')}}
+    injector.URLStress(
+      url='http://0.0.0.0:5002/',
+      request_type=injector.RequestType.post,
+      **sample_data
+    )
 ```
 
 #### Coding Standards
 Docstring format: [`Google`](https://google.github.io/styleguide/pyguide.html#38-comments-and-docstrings) <br>
 Styling conventions: [`PEP 8`](https://www.python.org/dev/peps/pep-0008/) <br>
 Clean code with pre-commit hooks: [`flake8`](https://flake8.pycqa.org/en/latest/) and 
 [`isort`](https://pycqa.github.io/isort/)
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: stress-injector Version: 0.4a0 Summary: Python
+Metadata-Version: 2.1 Name: stress-injector Version: 0.5 Summary: Python
 module, to inject memory and CPU stress, and URL load test Author-email:
 Vignesh Sivanandha Rao
 gmail.com> License: MIT License Copyright (c) 2021 Vignesh Sivanandha Rao
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
@@ -27,19 +27,19 @@
 Classifier: Intended Audience :: Information Technology Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: numpy (>=1.20.0) Requires-
-Dist: psutil (>=5.9.0) Requires-Dist: tqdm (>=4.56.0) Provides-Extra: dev
-Requires-Dist: pre-commit ; extra == 'dev' [![Pypi-version](https://
-img.shields.io/pypi/v/stress-injector)](https://pypi.org/project/stress-
-injector) [![Pypi-py-version](https://img.shields.io/pypi/pyversions/stress-
-injector)](https://pypi.org/project/stress-injector) ![docs](https://
+Dist: psutil (>=5.9.0) Requires-Dist: tqdm (>=4.56.0) Requires-Dist: requests
+Provides-Extra: dev Requires-Dist: pre-commit ; extra == 'dev' [![Pypi-version]
+(https://img.shields.io/pypi/v/stress-injector)](https://pypi.org/project/
+stress-injector) [![Pypi-py-version](https://img.shields.io/pypi/pyversions/
+stress-injector)](https://pypi.org/project/stress-injector) ![docs](https://
 github.com/thevickypedia/stress-injector/actions/workflows/docs.yml/badge.svg)
 ![pypi](https://github.com/thevickypedia/stress-injector/actions/workflows/
 python-publish.yml/badge.svg) [![Pypi-format](https://img.shields.io/pypi/
 format/stress-injector)](https://pypi.org/project/stress-injector/#files) [!
 [Pypi-status](https://img.shields.io/pypi/status/stress-injector)](https://
 pypi.org/project/stress-injector) ![Maintained](https://img.shields.io/
 maintenance/yes/2023) [![GitHub Repo created](https://img.shields.io/date/
@@ -61,26 +61,35 @@
  Insights about Memory_Stress * In this script, I have used
 `numpy.random.bytes` which are sampled from uniform distribution. * Generating
 these random bytes induces a stress on the machine's memory usage. * I have
 then used `getrusage` (get resource usage) for `SELF` to get the memory
 consumed only by the current script. * The `size_converter` converts the bytes
 from resource usage to a human understandable format.
  Insights about URL_Stress * In this script, I have used threadpools to make
-concurrent GET requests. * The script uses builtin library `urllib` to make the
-GET calls. * Takes arguments * **rate**: Number of calls to make. _Defaults to
-100K_ * **timeout**: Timeout for each request. _Defaults to 0.5_ *
-**retry_limit**: Retry limit if the system is unable to spinup more threads.
-_Defaults to 5_ * **circuit_break**: Wait time in seconds between retries.
-_Defaults to 5_  ### Usage `pip install stress-injector` [CPU Stress](https://
-github.com/thevickypedia/stress-injector/blob/main/stressinjector/cpu.py)
-```python import stressinjector as injector if __name__ == '__main__':
-injector.CPUStress(seconds=300).run() injector.MemoryStress
-(gigabytes=2_000).run() injector.URLStress(url='http://0.0.0.0:5002/').run()
-``` #### Coding Standards Docstring format: [`Google`](https://
-google.github.io/styleguide/pyguide.html#38-comments-and-docstrings)
+concurrent requests. * The script uses `requests` module to make calls. * Takes
+arguments * **rate**: Number of calls to make. _Defaults to 100K_ *
+**timeout**: Timeout for each request. _Defaults to 0.5_ * **retry_limit**:
+Retry limit if the system is unable to spinup more threads. _Defaults to 5_ *
+**circuit_break**: Wait time in seconds between retries. _Defaults to 5_ *
+**request_type**: Function from `requests` module.  ### Usage `pip install
+stress-injector` [CPU Stress](https://github.com/thevickypedia/stress-injector/
+blob/main/stressinjector/cpu.py) ```python import stressinjector as injector if
+__name__ == '__main__': injector.CPUStress(seconds=300) ``` [Memory Stress]
+(https://github.com/thevickypedia/stress-injector/blob/main/stressinjector/
+memory.py) ```python import stressinjector as injector if __name__ ==
+'__main__': injector.MemoryStress(gigabytes=2_000).run() ``` [URL Stress]
+(https://github.com/thevickypedia/stress-injector/blob/main/stressinjector/
+url.py) ```python import os import stressinjector as injector if __name__ ==
+'__main__': injector.URLStress(url='http://0.0.0.0:5002/') # Stress test GET
+calls # Stress test POST calls, also supports PUT, and DELETE sample_data =
+{'headers': {'Authorization': 'Bearer %s' % os.environ.get('TOKEN')}}
+injector.URLStress( url='http://0.0.0.0:5002/',
+request_type=injector.RequestType.post, **sample_data ) ``` #### Coding
+Standards Docstring format: [`Google`](https://google.github.io/styleguide/
+pyguide.html#38-comments-and-docstrings)
 Styling conventions: [`PEP 8`](https://www.python.org/dev/peps/pep-0008/)
 Clean code with pre-commit hooks: [`flake8`](https://flake8.pycqa.org/en/
 latest/) and [`isort`](https://pycqa.github.io/isort/) #### [Release Notes]
 (https://github.com/thevickypedia/stress-injector/blob/main/release_notes.rst)
 **Requirement** ```shell python -m pip install changelog-generator ```
 **Usage** ```shell changelog reverse -f release_notes.rst -t 'Release Notes'
 ``` #### Linting `PreCommit` will ensure linting, and the doc creation are run
```

