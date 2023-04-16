# Comparing `tmp/oaas_sdk_py-0.1.0.tar.gz` & `tmp/oaas_sdk_py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oaas_sdk_py-0.1.0.tar", last modified: Mon Feb 27 22:47:48 2023, max compression
+gzip compressed data, was "oaas_sdk_py-0.1.1.tar", last modified: Sun Apr 16 04:31:48 2023, max compression
```

## Comparing `oaas_sdk_py-0.1.0.tar` & `oaas_sdk_py-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-02-27 22:47:48.833699 oaas_sdk_py-0.1.0/
--rw-rw-rw-   0        0        0    11557 2023-02-10 20:57:09.000000 oaas_sdk_py-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      258 2023-02-27 22:47:48.833176 oaas_sdk_py-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-02-10 20:52:55.000000 oaas_sdk_py-0.1.0/README.md
--rw-rw-rw-   0        0        0      495 2023-02-27 22:47:37.000000 oaas_sdk_py-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-27 22:47:48.833699 oaas_sdk_py-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-27 22:47:48.821271 oaas_sdk_py-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-02-27 22:47:48.825672 oaas_sdk_py-0.1.0/src/oaas_sdk_py/
--rw-rw-rw-   0        0        0     8160 2023-02-27 22:45:46.000000 oaas_sdk_py-0.1.0/src/oaas_sdk_py/__init__.py
--rw-rw-rw-   0        0        0     1740 2023-02-27 22:42:20.000000 oaas_sdk_py-0.1.0/src/oaas_sdk_py/model.py
-drwxrwxrwx   0        0        0        0 2023-02-27 22:47:48.831539 oaas_sdk_py-0.1.0/src/oaas_sdk_py.egg-info/
--rw-rw-rw-   0        0        0      258 2023-02-27 22:47:48.000000 oaas_sdk_py-0.1.0/src/oaas_sdk_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-02-27 22:47:48.000000 oaas_sdk_py-0.1.0/src/oaas_sdk_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-27 22:47:48.000000 oaas_sdk_py-0.1.0/src/oaas_sdk_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-02-27 22:47:48.000000 oaas_sdk_py-0.1.0/src/oaas_sdk_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-02-27 22:47:48.000000 oaas_sdk_py-0.1.0/src/oaas_sdk_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 04:31:48.006533 oaas_sdk_py-0.1.1/
+-rw-rw-rw-   0        0        0    11557 2023-02-10 20:57:09.000000 oaas_sdk_py-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      258 2023-04-16 04:31:48.006533 oaas_sdk_py-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-02-10 20:52:55.000000 oaas_sdk_py-0.1.1/README.md
+-rw-rw-rw-   0        0        0      495 2023-04-16 04:29:04.000000 oaas_sdk_py-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 04:31:48.008094 oaas_sdk_py-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 04:31:47.976139 oaas_sdk_py-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 04:31:47.995860 oaas_sdk_py-0.1.1/src/oaas_sdk_py/
+-rw-rw-rw-   0        0        0     8754 2023-04-16 04:29:04.000000 oaas_sdk_py-0.1.1/src/oaas_sdk_py/__init__.py
+-rw-rw-rw-   0        0        0     1740 2023-04-14 09:02:39.000000 oaas_sdk_py-0.1.1/src/oaas_sdk_py/model.py
+drwxrwxrwx   0        0        0        0 2023-04-16 04:31:48.005514 oaas_sdk_py-0.1.1/src/oaas_sdk_py.egg-info/
+-rw-rw-rw-   0        0        0      258 2023-04-16 04:31:47.000000 oaas_sdk_py-0.1.1/src/oaas_sdk_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-04-16 04:31:47.000000 oaas_sdk_py-0.1.1/src/oaas_sdk_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 04:31:47.000000 oaas_sdk_py-0.1.1/src/oaas_sdk_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-16 04:31:47.000000 oaas_sdk_py-0.1.1/src/oaas_sdk_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-16 04:31:47.000000 oaas_sdk_py-0.1.1/src/oaas_sdk_py.egg-info/top_level.txt
```

### Comparing `oaas_sdk_py-0.1.0/LICENSE` & `oaas_sdk_py-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oaas_sdk_py-0.1.0/src/oaas_sdk_py/__init__.py` & `oaas_sdk_py-0.1.1/src/oaas_sdk_py/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,14 +104,27 @@
         url = self.allocate_url_dict[key]
         if url is None:
             raise OaasException(f"The output object not accept '{key}' as key")
         resp = await session.put(url, data=data)
         if not resp.ok:
             raise OaasException("Got error when put the data to S3")
 
+    async def upload_main_byte_data(self,
+                               session: ClientSession,
+                               key: str,
+                               data: bytearray) -> None:
+        if self.allocate_main_url_dict is None:
+            await self.allocate_file(session)
+        url = self.allocate_main_url_dict[key]
+        if url is None:
+            raise OaasException(f"The main object not accept '{key}' as key")
+        resp = await session.put(url, data=data)
+        if not resp.ok:
+            raise OaasException("Got error when put the data to S3")
+
     async def upload_file(self,
                           session: ClientSession,
                           key: str,
                           path: str) -> None:
         if self.allocate_url_dict is None:
             await self.allocate_file(session)
         url = self.allocate_url_dict[key]
```

### Comparing `oaas_sdk_py-0.1.0/src/oaas_sdk_py/model.py` & `oaas_sdk_py-0.1.1/src/oaas_sdk_py/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 class OaasObjectOrigin:
     def __init__(self, json_dict):
         self.json_dict = json_dict
 
     @property
     def args(self):
         if 'args' not in self.json_dict or self.json_dict['args'] is None:
-            self.json_dict['args'] = {}
+            self.json_dict['args'] = []
         return self.json_dict['args']
 
     @property
     def func(self):
         return self.json_dict['funcName']
```

