# Comparing `tmp/oaas_sdk_py-0.1.2.tar.gz` & `tmp/oaas_sdk_py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oaas_sdk_py-0.1.2.tar", last modified: Sun Apr 16 05:01:48 2023, max compression
+gzip compressed data, was "oaas_sdk_py-0.1.3.tar", last modified: Sun Apr 16 05:43:08 2023, max compression
```

## Comparing `oaas_sdk_py-0.1.2.tar` & `oaas_sdk_py-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 05:01:48.783461 oaas_sdk_py-0.1.2/
--rw-rw-rw-   0        0        0    11557 2023-02-10 20:57:09.000000 oaas_sdk_py-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      258 2023-04-16 05:01:48.783461 oaas_sdk_py-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-02-10 20:52:55.000000 oaas_sdk_py-0.1.2/README.md
--rw-rw-rw-   0        0        0      495 2023-04-16 05:01:01.000000 oaas_sdk_py-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-16 05:01:48.784969 oaas_sdk_py-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-16 05:01:48.771404 oaas_sdk_py-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 05:01:48.775684 oaas_sdk_py-0.1.2/src/oaas_sdk_py/
--rw-rw-rw-   0        0        0     8784 2023-04-16 05:01:01.000000 oaas_sdk_py-0.1.2/src/oaas_sdk_py/__init__.py
--rw-rw-rw-   0        0        0     1740 2023-04-14 09:02:39.000000 oaas_sdk_py-0.1.2/src/oaas_sdk_py/model.py
-drwxrwxrwx   0        0        0        0 2023-04-16 05:01:48.782455 oaas_sdk_py-0.1.2/src/oaas_sdk_py.egg-info/
--rw-rw-rw-   0        0        0      258 2023-04-16 05:01:48.000000 oaas_sdk_py-0.1.2/src/oaas_sdk_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-04-16 05:01:48.000000 oaas_sdk_py-0.1.2/src/oaas_sdk_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 05:01:48.000000 oaas_sdk_py-0.1.2/src/oaas_sdk_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-16 05:01:48.000000 oaas_sdk_py-0.1.2/src/oaas_sdk_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-16 05:01:48.000000 oaas_sdk_py-0.1.2/src/oaas_sdk_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 05:43:08.674819 oaas_sdk_py-0.1.3/
+-rw-rw-rw-   0        0        0    11557 2023-02-10 20:57:09.000000 oaas_sdk_py-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      258 2023-04-16 05:43:08.673820 oaas_sdk_py-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-02-10 20:52:55.000000 oaas_sdk_py-0.1.3/README.md
+-rw-rw-rw-   0        0        0      495 2023-04-16 05:42:49.000000 oaas_sdk_py-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 05:43:08.674819 oaas_sdk_py-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 05:43:08.661110 oaas_sdk_py-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 05:43:08.666970 oaas_sdk_py-0.1.3/src/oaas_sdk_py/
+-rw-rw-rw-   0        0        0     8789 2023-04-16 05:42:49.000000 oaas_sdk_py-0.1.3/src/oaas_sdk_py/__init__.py
+-rw-rw-rw-   0        0        0     1740 2023-04-14 09:02:39.000000 oaas_sdk_py-0.1.3/src/oaas_sdk_py/model.py
+drwxrwxrwx   0        0        0        0 2023-04-16 05:43:08.672810 oaas_sdk_py-0.1.3/src/oaas_sdk_py.egg-info/
+-rw-rw-rw-   0        0        0      258 2023-04-16 05:43:08.000000 oaas_sdk_py-0.1.3/src/oaas_sdk_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-04-16 05:43:08.000000 oaas_sdk_py-0.1.3/src/oaas_sdk_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 05:43:08.000000 oaas_sdk_py-0.1.3/src/oaas_sdk_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-16 05:43:08.000000 oaas_sdk_py-0.1.3/src/oaas_sdk_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-16 05:43:08.000000 oaas_sdk_py-0.1.3/src/oaas_sdk_py.egg-info/top_level.txt
```

### Comparing `oaas_sdk_py-0.1.2/LICENSE` & `oaas_sdk_py-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oaas_sdk_py-0.1.2/src/oaas_sdk_py/__init__.py` & `oaas_sdk_py-0.1.3/src/oaas_sdk_py/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             raise OaasException("Got error when put the data to S3")
 
     async def upload_main_byte_data(self,
                                session: ClientSession,
                                key: str,
                                data: bytearray) -> None:
         if self.allocate_main_url_dict is None:
-            await self.allocate_file(session)
+            await self.allocate_main_file(session)
         url = self.allocate_main_url_dict[key]
         if url is None:
             raise OaasException(f"The main object not accept '{key}' as key")
         resp = await session.put(url, data=data)
         if not resp.ok:
             raise OaasException("Got error when put the data to S3")
```

### Comparing `oaas_sdk_py-0.1.2/src/oaas_sdk_py/model.py` & `oaas_sdk_py-0.1.3/src/oaas_sdk_py/model.py`

 * *Files identical despite different names*

