# Comparing `tmp/httpx-socks-0.7.5.tar.gz` & `tmp/httpx-socks-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/httpx-socks-0.7.5.tar", last modified: Tue Nov 22 14:22:01 2022, max compression
+gzip compressed data, was "dist/httpx-socks-0.7.6.tar", last modified: Sun Apr 16 05:43:39 2023, max compression
```

## Comparing `httpx-socks-0.7.5.tar` & `httpx-socks-0.7.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2022-11-22 14:22:01.000000 httpx-socks-0.7.5/
--rw-rw-r--   0 roman     (1000) roman     (1000)    11357 2020-11-30 04:28:18.000000 httpx-socks-0.7.5/LICENSE.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)       47 2020-11-30 04:28:18.000000 httpx-socks-0.7.5/MANIFEST.in
--rw-rw-r--   0 roman     (1000) roman     (1000)     2828 2022-11-22 14:22:01.000000 httpx-socks-0.7.5/PKG-INFO
--rw-rw-r--   0 roman     (1000) roman     (1000)     2409 2022-02-12 08:51:18.000000 httpx-socks-0.7.5/README.md
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2022-11-22 14:22:01.000000 httpx-socks-0.7.5/httpx_socks/
--rw-rw-r--   0 roman     (1000) roman     (1000)      448 2022-11-22 14:00:52.000000 httpx-socks-0.7.5/httpx_socks/__init__.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     8125 2021-11-25 11:27:42.000000 httpx-socks-0.7.5/httpx_socks/_async_proxy.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     3400 2021-11-25 11:17:09.000000 httpx-socks-0.7.5/httpx_socks/_async_transport.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     6195 2021-11-25 11:29:34.000000 httpx-socks-0.7.5/httpx_socks/_sync_proxy.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     1420 2021-11-25 12:08:29.000000 httpx-socks-0.7.5/httpx_socks/_sync_stream.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     3265 2021-11-25 11:27:33.000000 httpx-socks-0.7.5/httpx_socks/_sync_transport.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2022-11-22 14:22:01.000000 httpx-socks-0.7.5/httpx_socks.egg-info/
--rw-rw-r--   0 roman     (1000) roman     (1000)     2828 2022-11-22 14:22:00.000000 httpx-socks-0.7.5/httpx_socks.egg-info/PKG-INFO
--rw-rw-r--   0 roman     (1000) roman     (1000)      401 2022-11-22 14:22:00.000000 httpx-socks-0.7.5/httpx_socks.egg-info/SOURCES.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)        1 2022-11-22 14:22:00.000000 httpx-socks-0.7.5/httpx_socks.egg-info/dependency_links.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)      120 2022-11-22 14:22:00.000000 httpx-socks-0.7.5/httpx_socks.egg-info/requires.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)       12 2022-11-22 14:22:00.000000 httpx-socks-0.7.5/httpx_socks.egg-info/top_level.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)      209 2022-02-06 06:27:51.000000 httpx-socks-0.7.5/pyproject.toml
--rw-rw-r--   0 roman     (1000) roman     (1000)       38 2022-11-22 14:22:01.000000 httpx-socks-0.7.5/setup.cfg
--rw-rw-r--   0 roman     (1000) roman     (1000)     1330 2022-11-22 13:59:48.000000 httpx-socks-0.7.5/setup.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-04-16 05:43:39.000000 httpx-socks-0.7.6/
+-rw-rw-r--   0 roman     (1000) roman     (1000)    11357 2020-11-30 04:28:18.000000 httpx-socks-0.7.6/LICENSE.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)       47 2020-11-30 04:28:18.000000 httpx-socks-0.7.6/MANIFEST.in
+-rw-rw-r--   0 roman     (1000) roman     (1000)     2828 2023-04-16 05:43:39.000000 httpx-socks-0.7.6/PKG-INFO
+-rw-rw-r--   0 roman     (1000) roman     (1000)     2409 2022-02-12 08:51:18.000000 httpx-socks-0.7.6/README.md
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-04-16 05:43:39.000000 httpx-socks-0.7.6/httpx_socks/
+-rw-rw-r--   0 roman     (1000) roman     (1000)      448 2023-04-16 05:31:37.000000 httpx-socks-0.7.6/httpx_socks/__init__.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     8125 2021-11-25 11:27:42.000000 httpx-socks-0.7.6/httpx_socks/_async_proxy.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     3400 2021-11-25 11:17:09.000000 httpx-socks-0.7.6/httpx_socks/_async_transport.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     6195 2021-11-25 11:29:34.000000 httpx-socks-0.7.6/httpx_socks/_sync_proxy.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1420 2021-11-25 12:08:29.000000 httpx-socks-0.7.6/httpx_socks/_sync_stream.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     3265 2021-11-25 11:27:33.000000 httpx-socks-0.7.6/httpx_socks/_sync_transport.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-04-16 05:43:39.000000 httpx-socks-0.7.6/httpx_socks.egg-info/
+-rw-rw-r--   0 roman     (1000) roman     (1000)     2828 2023-04-16 05:43:38.000000 httpx-socks-0.7.6/httpx_socks.egg-info/PKG-INFO
+-rw-rw-r--   0 roman     (1000) roman     (1000)      401 2023-04-16 05:43:38.000000 httpx-socks-0.7.6/httpx_socks.egg-info/SOURCES.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)        1 2023-04-16 05:43:38.000000 httpx-socks-0.7.6/httpx_socks.egg-info/dependency_links.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)      120 2023-04-16 05:43:38.000000 httpx-socks-0.7.6/httpx_socks.egg-info/requires.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)       12 2023-04-16 05:43:38.000000 httpx-socks-0.7.6/httpx_socks.egg-info/top_level.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)      209 2022-02-06 06:27:51.000000 httpx-socks-0.7.6/pyproject.toml
+-rw-rw-r--   0 roman     (1000) roman     (1000)       38 2023-04-16 05:43:39.000000 httpx-socks-0.7.6/setup.cfg
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1330 2023-04-16 05:29:16.000000 httpx-socks-0.7.6/setup.py
```

### Comparing `httpx-socks-0.7.5/LICENSE.txt` & `httpx-socks-0.7.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `httpx-socks-0.7.5/PKG-INFO` & `httpx-socks-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpx-socks
-Version: 0.7.5
+Version: 0.7.6
 Summary: Proxy (HTTP, SOCKS) transports for httpx
 Home-page: https://github.com/romis2012/httpx-socks
 Author: Roman Snegirev
 Author-email: snegiryev@gmail.com
 License: Apache 2
 Keywords: httpx asyncio socks socks5 socks4 http proxy
 Platform: UNKNOWN
```

### Comparing `httpx-socks-0.7.5/README.md` & `httpx-socks-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `httpx-socks-0.7.5/httpx_socks/_async_proxy.py` & `httpx-socks-0.7.6/httpx_socks/_async_proxy.py`

 * *Files identical despite different names*

### Comparing `httpx-socks-0.7.5/httpx_socks/_async_transport.py` & `httpx-socks-0.7.6/httpx_socks/_async_transport.py`

 * *Files identical despite different names*

### Comparing `httpx-socks-0.7.5/httpx_socks/_sync_proxy.py` & `httpx-socks-0.7.6/httpx_socks/_sync_proxy.py`

 * *Files identical despite different names*

### Comparing `httpx-socks-0.7.5/httpx_socks/_sync_stream.py` & `httpx-socks-0.7.6/httpx_socks/_sync_stream.py`

 * *Files identical despite different names*

### Comparing `httpx-socks-0.7.5/httpx_socks/_sync_transport.py` & `httpx-socks-0.7.6/httpx_socks/_sync_transport.py`

 * *Files identical despite different names*

### Comparing `httpx-socks-0.7.5/httpx_socks.egg-info/PKG-INFO` & `httpx-socks-0.7.6/httpx_socks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpx-socks
-Version: 0.7.5
+Version: 0.7.6
 Summary: Proxy (HTTP, SOCKS) transports for httpx
 Home-page: https://github.com/romis2012/httpx-socks
 Author: Roman Snegirev
 Author-email: snegiryev@gmail.com
 License: Apache 2
 Keywords: httpx asyncio socks socks5 socks4 http proxy
 Platform: UNKNOWN
```

### Comparing `httpx-socks-0.7.5/setup.py` & `httpx-socks-0.7.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,16 +33,16 @@
     url='https://github.com/romis2012/httpx-socks',
     description='Proxy (HTTP, SOCKS) transports for httpx',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['httpx_socks'],
     keywords='httpx asyncio socks socks5 socks4 http proxy',
     install_requires=[
-        'httpx>=0.21.0,<0.24.0',
-        'httpcore>=0.14.0,<0.17.0',
+        'httpx>=0.21.0,<0.25.0',
+        'httpcore>=0.14.0,<0.18.0',
         'python-socks>=2.0.0',
     ],
     extras_require={
         'asyncio': ['async-timeout>=3.0.1'],
         'trio': ['trio>=0.16.0'],
     }
 )
```

