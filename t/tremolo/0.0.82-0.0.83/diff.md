# Comparing `tmp/tremolo-0.0.82.tar.gz` & `tmp/tremolo-0.0.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tremolo-0.0.82.tar", last modified: Wed Apr 12 23:55:57 2023, max compression
+gzip compressed data, was "dist/tremolo-0.0.83.tar", last modified: Sun Apr 16 13:38:25 2023, max compression
```

## Comparing `tremolo-0.0.82.tar` & `tremolo-0.0.83.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 23:55:57.000000 tremolo-0.0.82/
--rw-r--r--   0 tux       (1000) users      (100)     3487 2023-04-12 23:55:57.000000 tremolo-0.0.82/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)     2202 2023-04-12 13:07:35.000000 tremolo-0.0.82/README.md
--rw-r--r--   0 tux       (1000) users      (100)       38 2023-04-12 23:55:57.000000 tremolo-0.0.82/setup.cfg
--rwxr-xr-x   0 tux       (1000) users      (100)      973 2023-04-12 23:52:43.000000 tremolo-0.0.82/setup.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 23:55:57.000000 tremolo-0.0.82/tremolo/
--rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-04-12 13:07:35.000000 tremolo-0.0.82/tremolo/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)      321 2023-04-12 13:07:35.000000 tremolo-0.0.82/tremolo/exceptions.py
--rw-r--r--   0 tux       (1000) users      (100)    11749 2023-04-12 23:50:45.000000 tremolo-0.0.82/tremolo/http_server.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 23:55:57.000000 tremolo-0.0.82/tremolo/lib/
--rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 13:07:35.000000 tremolo-0.0.82/tremolo/lib/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)      846 2023-04-12 13:07:35.000000 tremolo-0.0.82/tremolo/lib/connection_pool.py
--rw-r--r--   0 tux       (1000) users      (100)     1665 2023-04-12 13:07:35.000000 tremolo-0.0.82/tremolo/lib/http_exception.py
--rwxr-xr-x   0 tux       (1000) users      (100)    13717 2023-04-12 23:43:31.000000 tremolo-0.0.82/tremolo/lib/http_protocol.py
--rwxr-xr-x   0 tux       (1000) users      (100)     8527 2023-04-12 13:07:35.000000 tremolo-0.0.82/tremolo/lib/http_request.py
--rwxr-xr-x   0 tux       (1000) users      (100)    10732 2023-04-12 13:07:35.000000 tremolo-0.0.82/tremolo/lib/http_response.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 23:55:57.000000 tremolo-0.0.82/tremolo/lib/parsed/
--rw-r--r--   0 tux       (1000) users      (100)       31 2023-04-12 13:07:35.000000 tremolo-0.0.82/tremolo/lib/parsed/__init__.py
--rwxr-xr-x   0 tux       (1000) users      (100)     5466 2023-04-12 13:07:35.000000 tremolo-0.0.82/tremolo/lib/parsed/parse.py
--rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-04-12 13:07:35.000000 tremolo-0.0.82/tremolo/lib/request.py
--rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-04-12 13:07:35.000000 tremolo-0.0.82/tremolo/lib/response.py
--rwxr-xr-x   0 tux       (1000) users      (100)    13754 2023-04-12 13:07:35.000000 tremolo-0.0.82/tremolo/tremolo.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 23:55:57.000000 tremolo-0.0.82/tremolo.egg-info/
--rw-r--r--   0 tux       (1000) users      (100)     3487 2023-04-12 23:55:57.000000 tremolo-0.0.82/tremolo.egg-info/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)      503 2023-04-12 23:55:57.000000 tremolo-0.0.82/tremolo.egg-info/SOURCES.txt
--rw-r--r--   0 tux       (1000) users      (100)        1 2023-04-12 23:55:57.000000 tremolo-0.0.82/tremolo.egg-info/dependency_links.txt
--rw-r--r--   0 tux       (1000) users      (100)        8 2023-04-12 23:55:57.000000 tremolo-0.0.82/tremolo.egg-info/top_level.txt
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-16 13:38:25.000000 tremolo-0.0.83/
+-rw-r--r--   0 tux       (1000) users      (100)     3487 2023-04-16 13:38:25.000000 tremolo-0.0.83/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)     2202 2023-04-12 13:07:35.000000 tremolo-0.0.83/README.md
+-rw-r--r--   0 tux       (1000) users      (100)       38 2023-04-16 13:38:25.000000 tremolo-0.0.83/setup.cfg
+-rwxr-xr-x   0 tux       (1000) users      (100)      973 2023-04-16 13:32:51.000000 tremolo-0.0.83/setup.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-16 13:38:25.000000 tremolo-0.0.83/tremolo/
+-rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-04-12 13:07:35.000000 tremolo-0.0.83/tremolo/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)      321 2023-04-12 13:07:35.000000 tremolo-0.0.83/tremolo/exceptions.py
+-rw-r--r--   0 tux       (1000) users      (100)    11749 2023-04-14 02:53:18.000000 tremolo-0.0.83/tremolo/http_server.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-16 13:38:25.000000 tremolo-0.0.83/tremolo/lib/
+-rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 13:07:35.000000 tremolo-0.0.83/tremolo/lib/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)      846 2023-04-12 13:07:35.000000 tremolo-0.0.83/tremolo/lib/connection_pool.py
+-rw-r--r--   0 tux       (1000) users      (100)     1665 2023-04-12 13:07:35.000000 tremolo-0.0.83/tremolo/lib/http_exception.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    13717 2023-04-12 23:43:31.000000 tremolo-0.0.83/tremolo/lib/http_protocol.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     8522 2023-04-16 13:13:40.000000 tremolo-0.0.83/tremolo/lib/http_request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    10732 2023-04-14 02:53:02.000000 tremolo-0.0.83/tremolo/lib/http_response.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-16 13:38:25.000000 tremolo-0.0.83/tremolo/lib/parsed/
+-rw-r--r--   0 tux       (1000) users      (100)       31 2023-04-12 13:07:35.000000 tremolo-0.0.83/tremolo/lib/parsed/__init__.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     4962 2023-04-16 13:30:48.000000 tremolo-0.0.83/tremolo/lib/parsed/parse.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-04-12 13:07:35.000000 tremolo-0.0.83/tremolo/lib/request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-04-12 13:07:35.000000 tremolo-0.0.83/tremolo/lib/response.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    13754 2023-04-12 13:07:35.000000 tremolo-0.0.83/tremolo/tremolo.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-16 13:38:25.000000 tremolo-0.0.83/tremolo.egg-info/
+-rw-r--r--   0 tux       (1000) users      (100)     3487 2023-04-16 13:38:25.000000 tremolo-0.0.83/tremolo.egg-info/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)      503 2023-04-16 13:38:25.000000 tremolo-0.0.83/tremolo.egg-info/SOURCES.txt
+-rw-r--r--   0 tux       (1000) users      (100)        1 2023-04-16 13:38:25.000000 tremolo-0.0.83/tremolo.egg-info/dependency_links.txt
+-rw-r--r--   0 tux       (1000) users      (100)        8 2023-04-16 13:38:25.000000 tremolo-0.0.83/tremolo.egg-info/top_level.txt
```

### Comparing `tremolo-0.0.82/PKG-INFO` & `tremolo-0.0.83/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.82
+Version: 0.0.83
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Description: # Tremolo
```

### Comparing `tremolo-0.0.82/README.md` & `tremolo-0.0.83/README.md`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.82/setup.py` & `tremolo-0.0.83/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='tremolo',
     packages=['tremolo'],
     package_data={'': ['lib/*', 'lib/parsed/*']},
-    version='0.0.82',
+    version='0.0.83',
     license='MIT',
     author='nggit',
     author_email='contact@anggit.com',
     description='Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nggit/tremolo',
```

### Comparing `tremolo-0.0.82/tremolo/http_server.py` & `tremolo-0.0.83/tremolo/http_server.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.82/tremolo/lib/connection_pool.py` & `tremolo-0.0.83/tremolo/lib/connection_pool.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.82/tremolo/lib/http_exception.py` & `tremolo-0.0.83/tremolo/lib/http_exception.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.82/tremolo/lib/http_protocol.py` & `tremolo-0.0.83/tremolo/lib/http_protocol.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.82/tremolo/lib/http_request.py` & `tremolo-0.0.83/tremolo/lib/http_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .request import Request
 
 class HTTPRequest(Request):
     def __init__(self, protocol):
         super().__init__(protocol)
 
         self.is_valid = protocol.header.is_valid_request
-        self.headers = protocol.header.getheaders()
+        self.headers = protocol.header.headers
         self.host = protocol.header.gethost()
 
         if isinstance(self.host, list):
             self.host = self.host[0]
 
         self.method = protocol.header.getmethod().upper()
         self.path = protocol.header.getpath()
```

### Comparing `tremolo-0.0.82/tremolo/lib/http_response.py` & `tremolo-0.0.83/tremolo/lib/http_response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.82/tremolo/lib/parsed/parse.py` & `tremolo-0.0.83/tremolo/lib/parsed/parse.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     def parse(self, data, header_size=None, excludes=[]):
         self.is_request = False
         self.is_response = False
         self.is_valid_request = False
         self.is_valid_response = False
 
         self._data = data
-        self._headers = Headers()
-        self._header = {}
+        self.headers = Headers()
+        self._headers = []
         self._header_size = header_size
 
         if data == b'' or not isinstance(data, (bytearray, bytes)):
             return self
 
         if isinstance(data, bytes):
             self._data = bytearray(data)
@@ -62,109 +62,101 @@
                 name = line[:colon_pos]
                 name_lc = bytes(name.lower())
                 value = line[colon_pos + 1:]
 
                 if value.startswith(b' '):
                     value = value[1:]
 
-                if name_lc in self._headers and isinstance(self._headers[name_lc], list):
-                    self._headers[name_lc].append(value)
+                if name_lc in self.headers and isinstance(self.headers[name_lc], list):
+                    self.headers[name_lc].append(value)
                 else:
-                    if name_lc in self._headers:
-                        self._headers[name_lc] = [self._headers[name_lc], value]
+                    if name_lc in self.headers:
+                        self.headers[name_lc] = [self.headers[name_lc], value]
                     else:
-                        self._headers[name_lc] = value
+                        self.headers[name_lc] = value
 
                 if name_lc not in excludes:
-                    if name_lc in self._header and isinstance(self._header[name_lc], list):
-                        self._header[name_lc].append(name + b': ' + value)
-                    else:
-                        self._header[name_lc] = [name + b': ' + value]
+                    self._headers.append((name_lc, value))
             elif start == 0:
                 if line.startswith(b'HTTP/'):
                     self.is_response = True
 
                     try:
-                        _, self._headers[b'_version'], _status, self._headers[b'_message'] = line.replace(b'/', b' ').split(None, 3)
-                        self._headers[b'_status'] = int(_status)
+                        _, self.headers[b'_version'], _status, self.headers[b'_message'] = line.replace(b'/', b' ').split(None, 3)
+                        self.headers[b'_status'] = int(_status)
                         self.is_valid_response = True
                     except ValueError:
-                        self._headers[b'_version'] = b''
-                        self._headers[b'_status'] = 0
-                        self._headers[b'_message'] = b''
+                        self.headers[b'_version'] = b''
+                        self.headers[b'_status'] = 0
+                        self.headers[b'_message'] = b''
                 else:
                     path_end_pos = line.find(b' HTTP/')
 
                     if path_end_pos > 0:
                         self.is_request = True
 
                         try:
-                            self._headers[b'_method'], self._headers[b'_path'] = line[:path_end_pos].split(b' ', 1)
-                            self._headers[b'_version'] = line[path_end_pos + len(' HTTP/'):]
+                            self.headers[b'_method'], self.headers[b'_path'] = line[:path_end_pos].split(b' ', 1)
+                            self.headers[b'_version'] = line[path_end_pos + len(' HTTP/'):]
                             self.is_valid_request = True
                         except ValueError:
-                            self._headers[b'_method'] = b''
-                            self._headers[b'_path'] = b''
-                            self._headers[b'_version'] = b''
+                            self.headers[b'_method'] = b''
+                            self.headers[b'_path'] = b''
+                            self.headers[b'_version'] = b''
 
-                self._header[0] = [line]
+                self.headers[b'_line'] = line
             else:
                 self.is_valid_request = False
                 self.is_valid_response = False
 
                 break
 
             start = end + 2
 
-        if self.is_valid_request and self._headers[b'_version'] == b'1.1' and b'host' not in self._headers:
-            self._headers[b'host'] = b''
+        if self.is_valid_request and self.headers[b'_version'] == b'1.1' and b'host' not in self.headers:
+            self.headers[b'host'] = b''
             self.is_valid_request = False
 
         return self
 
-    def remove(self, remove=[]):
-        if remove == [] or not isinstance(remove, list):
+    def remove(self, *args):
+        if not args:
             return self
 
-        for value in remove:
-            if value in self._header:
-                del self._header[value]
+        for i, v in enumerate(self._headers):
+            if v[0] in args:
+                del self._headers[i]
 
         return self
 
-    def append(self, append={}):
-        if append == {} or not isinstance(append, dict):
-            return self
-
-        for name in append:
-            name_lc = name.lower()
-
-            if name_lc in self._header and isinstance(self._header[name_lc], list):
-                self._header[name_lc].append(name + b': ' + append[name])
-            else:
-                self._header[name_lc] = [name + b': ' + append[name]]
+    def append(self, *args):
+        for v in args:
+            if isinstance(v, tuple):
+                self._headers.append(v)
 
         return self
 
     def getheaders(self):
         return self._headers
 
     def gethost(self):
-        return self._headers.get(b'x-forwarded-host', self._headers.get(b'host'))
+        return self.headers.get(b'x-forwarded-host', self.headers.get(b'host'))
 
     def getmethod(self):
-        return self._headers.get(b'_method')
+        return self.headers.get(b'_method')
 
     def getpath(self):
-        return self._headers.get(b'_path')
+        return self.headers.get(b'_path')
 
     def getversion(self):
-        return self._headers.get(b'_version')
+        return self.headers.get(b'_version')
 
     def getstatus(self):
-        return self._headers.get(b'_status')
+        return self.headers.get(b'_status')
 
     def getmessage(self):
-        return self._headers.get(b'_message')
+        return self.headers.get(b'_message')
 
     def save(self):
-        return bytearray(b'\r\n').join([bytearray(b'\r\n').join(v) for v in self._header.values()]) + self._data[self._header_size:]
+        return bytearray(b'\r\n').join(
+                [self.headers.get(b'_line', b'')] + [bytearray(b': ').join(v) for v in self._headers]
+            ) + self._data[self._header_size:]
```

### Comparing `tremolo-0.0.82/tremolo/lib/request.py` & `tremolo-0.0.83/tremolo/lib/request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.82/tremolo/lib/response.py` & `tremolo-0.0.83/tremolo/lib/response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.82/tremolo/tremolo.py` & `tremolo-0.0.83/tremolo/tremolo.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.82/tremolo.egg-info/PKG-INFO` & `tremolo-0.0.83/tremolo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.82
+Version: 0.0.83
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Description: # Tremolo
```

