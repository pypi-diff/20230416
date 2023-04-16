# Comparing `tmp/async-http-requests-0.0.0.tar.gz` & `tmp/async-http-requests-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async-http-requests-0.0.0.tar", last modified: Fri Apr 14 16:26:22 2023, max compression
+gzip compressed data, was "async-http-requests-0.0.1.tar", last modified: Sun Apr 16 17:04:52 2023, max compression
```

## Comparing `async-http-requests-0.0.0.tar` & `async-http-requests-0.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 andreasergi  (1000) andreasergi  (1000)        0 2023-04-14 16:26:22.113147 async-http-requests-0.0.0/
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     1078 2023-04-13 10:12:28.000000 async-http-requests-0.0.0/LICENSE
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)       17 2023-04-14 15:28:46.000000 async-http-requests-0.0.0/MANIFEST.in
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     5102 2023-04-14 16:26:22.109147 async-http-requests-0.0.0/PKG-INFO
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     3347 2023-04-14 15:50:08.000000 async-http-requests-0.0.0/README.md
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      854 2023-04-14 16:25:59.000000 async-http-requests-0.0.0/pyproject.toml
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)       38 2023-04-14 16:26:22.113147 async-http-requests-0.0.0/setup.cfg
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)       38 2023-04-13 22:04:33.000000 async-http-requests-0.0.0/setup.py
-drwxrwxr-x   0 andreasergi  (1000) andreasergi  (1000)        0 2023-04-14 16:26:22.109147 async-http-requests-0.0.0/src/
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     5068 2023-04-14 14:30:41.000000 async-http-requests-0.0.0/src/AsyncRequests.py
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      608 2023-04-14 09:22:32.000000 async-http-requests-0.0.0/src/RequestObject.py
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      476 2023-04-14 10:05:37.000000 async-http-requests-0.0.0/src/RequestsType.py
-drwxrwxr-x   0 andreasergi  (1000) andreasergi  (1000)        0 2023-04-14 16:26:22.109147 async-http-requests-0.0.0/src/async_http_requests.egg-info/
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     5102 2023-04-14 16:26:22.000000 async-http-requests-0.0.0/src/async_http_requests.egg-info/PKG-INFO
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      376 2023-04-14 16:26:22.000000 async-http-requests-0.0.0/src/async_http_requests.egg-info/SOURCES.txt
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)        1 2023-04-14 16:26:22.000000 async-http-requests-0.0.0/src/async_http_requests.egg-info/dependency_links.txt
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      144 2023-04-14 16:26:22.000000 async-http-requests-0.0.0/src/async_http_requests.egg-info/requires.txt
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)       48 2023-04-14 16:26:22.000000 async-http-requests-0.0.0/src/async_http_requests.egg-info/top_level.txt
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      459 2023-04-13 16:22:15.000000 async-http-requests-0.0.0/src/helper.py
-drwxrwxr-x   0 andreasergi  (1000) andreasergi  (1000)        0 2023-04-14 16:26:22.109147 async-http-requests-0.0.0/test/
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     1213 2023-04-14 16:02:07.000000 async-http-requests-0.0.0/test/test.py
+drwxrwxr-x   0 andreasergi  (1000) andreasergi  (1000)        0 2023-04-16 17:04:52.731696 async-http-requests-0.0.1/
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     1078 2023-04-13 10:12:28.000000 async-http-requests-0.0.1/LICENSE
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)       17 2023-04-14 15:28:46.000000 async-http-requests-0.0.1/MANIFEST.in
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     5168 2023-04-16 17:04:52.731696 async-http-requests-0.0.1/PKG-INFO
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     3413 2023-04-16 16:58:44.000000 async-http-requests-0.0.1/README.md
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      854 2023-04-16 17:01:18.000000 async-http-requests-0.0.1/pyproject.toml
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)       38 2023-04-16 17:04:52.731696 async-http-requests-0.0.1/setup.cfg
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)       38 2023-04-13 22:04:33.000000 async-http-requests-0.0.1/setup.py
+drwxrwxr-x   0 andreasergi  (1000) andreasergi  (1000)        0 2023-04-16 17:04:52.731696 async-http-requests-0.0.1/src/
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     5226 2023-04-16 16:18:11.000000 async-http-requests-0.0.1/src/AsyncRequests.py
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      608 2023-04-14 09:22:32.000000 async-http-requests-0.0.1/src/RequestObject.py
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      476 2023-04-14 10:05:37.000000 async-http-requests-0.0.1/src/RequestsType.py
+drwxrwxr-x   0 andreasergi  (1000) andreasergi  (1000)        0 2023-04-16 17:04:52.731696 async-http-requests-0.0.1/src/async_http_requests.egg-info/
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     5168 2023-04-16 17:04:52.000000 async-http-requests-0.0.1/src/async_http_requests.egg-info/PKG-INFO
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      376 2023-04-16 17:04:52.000000 async-http-requests-0.0.1/src/async_http_requests.egg-info/SOURCES.txt
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)        1 2023-04-16 17:04:52.000000 async-http-requests-0.0.1/src/async_http_requests.egg-info/dependency_links.txt
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      144 2023-04-16 17:04:52.000000 async-http-requests-0.0.1/src/async_http_requests.egg-info/requires.txt
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)       48 2023-04-16 17:04:52.000000 async-http-requests-0.0.1/src/async_http_requests.egg-info/top_level.txt
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      459 2023-04-13 16:22:15.000000 async-http-requests-0.0.1/src/helper.py
+drwxrwxr-x   0 andreasergi  (1000) andreasergi  (1000)        0 2023-04-16 17:04:52.731696 async-http-requests-0.0.1/test/
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     1213 2023-04-14 16:02:07.000000 async-http-requests-0.0.1/test/test.py
```

### Comparing `async-http-requests-0.0.0/LICENSE` & `async-http-requests-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `async-http-requests-0.0.0/PKG-INFO` & `async-http-requests-0.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-http-requests
-Version: 0.0.0
+Version: 0.0.1
 Summary: Asynchronous HTTP requests
 Author-email: Andrea Sergi <andrea.serg1@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 sclash - Andrea Sergi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,21 +35,24 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # Async Requests
 
 Python library to handle asynchronous http requests, built on top of the [requests](https://requests.readthedocs.io/en/latest/) library 
 
+
 - [Installation](#installation)
 - [Usage](#usage)
 
 ## Installation
 
+[PyPI page](https://pypi.org/project/async-http-requests/)
+
 ```bash
-pip install async-requests
+pip install async-http-requests
 ```
 
 ## Usage
 
 The library provide support for asynchronous http request, using the consumer-producer pattern.
 
 Instantiate the class `AsyncHTTP` specifying a list of `RequestObject`, (you can specify `N_PRODUCERS` and `N_CONSUMERS`: default values are `50` for both)
```

### Comparing `async-http-requests-0.0.0/README.md` & `async-http-requests-0.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # Async Requests
 
 Python library to handle asynchronous http requests, built on top of the [requests](https://requests.readthedocs.io/en/latest/) library 
 
+
 - [Installation](#installation)
 - [Usage](#usage)
 
 ## Installation
 
+[PyPI page](https://pypi.org/project/async-http-requests/)
+
 ```bash
-pip install async-requests
+pip install async-http-requests
 ```
 
 ## Usage
 
 The library provide support for asynchronous http request, using the consumer-producer pattern.
 
 Instantiate the class `AsyncHTTP` specifying a list of `RequestObject`, (you can specify `N_PRODUCERS` and `N_CONSUMERS`: default values are `50` for both)
```

### Comparing `async-http-requests-0.0.0/pyproject.toml` & `async-http-requests-0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "async-http-requests"
-version = "0.0.0"
+version = "0.0.1"
 description = "Asynchronous HTTP requests"
 readme = "README.md"
 authors = [{ name = "Andrea Sergi", email = "andrea.serg1@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `async-http-requests-0.0.0/src/AsyncRequests.py` & `async-http-requests-0.0.1/src/AsyncRequests.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,16 +56,20 @@
     async def __async_http_thread(self, r_obj: RequestObject, **fixed_kwargs):
         return await asyncio.to_thread(self.sync_http, r_obj , **fixed_kwargs)
     
     async def __produce(self, chunk: List[RequestObject], **fixed_kwargs):
         try:
             for r_obj in chunk:
                 r = await self.__async_http_thread(r_obj, **fixed_kwargs)
-                await self.queue.put(r)
+                if r:
+                    await self.queue.put(r)
+                else:
+                    await self.queue.put(None)
         except Exception as e:
+            self.error_response.append((r_obj, r.status_code))
             logger.error(f"PRODUCER ERROR: {r_obj}")
             print(e)
 
     async def __consume(self, callback: Optional[Callable] = None):
         while True:
             try:
                 data = await self.queue.get()
```

### Comparing `async-http-requests-0.0.0/src/RequestObject.py` & `async-http-requests-0.0.1/src/RequestObject.py`

 * *Files identical despite different names*

### Comparing `async-http-requests-0.0.0/src/async_http_requests.egg-info/PKG-INFO` & `async-http-requests-0.0.1/src/async_http_requests.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-http-requests
-Version: 0.0.0
+Version: 0.0.1
 Summary: Asynchronous HTTP requests
 Author-email: Andrea Sergi <andrea.serg1@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 sclash - Andrea Sergi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,21 +35,24 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # Async Requests
 
 Python library to handle asynchronous http requests, built on top of the [requests](https://requests.readthedocs.io/en/latest/) library 
 
+
 - [Installation](#installation)
 - [Usage](#usage)
 
 ## Installation
 
+[PyPI page](https://pypi.org/project/async-http-requests/)
+
 ```bash
-pip install async-requests
+pip install async-http-requests
 ```
 
 ## Usage
 
 The library provide support for asynchronous http request, using the consumer-producer pattern.
 
 Instantiate the class `AsyncHTTP` specifying a list of `RequestObject`, (you can specify `N_PRODUCERS` and `N_CONSUMERS`: default values are `50` for both)
```

### Comparing `async-http-requests-0.0.0/test/test.py` & `async-http-requests-0.0.1/test/test.py`

 * *Files identical despite different names*

