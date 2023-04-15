# Comparing `tmp/structio-1.1.4.tar.gz` & `tmp/structio-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structio-1.1.4.tar", last modified: Thu Apr 13 19:42:08 2023, max compression
+gzip compressed data, was "structio-1.1.5.tar", last modified: Sat Apr 15 22:29:42 2023, max compression
```

## Comparing `structio-1.1.4.tar` & `structio-1.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:42:08.826329 structio-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-04-13 19:42:08.826329 structio-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13356 2023-04-13 19:41:52.000000 structio-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-13 19:41:52.000000 structio-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 19:42:08.826329 structio-1.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:42:08.826329 structio-1.1.4/structio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-04-13 19:42:08.000000 structio-1.1.4/structio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-13 19:42:08.000000 structio-1.1.4/structio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:42:08.000000 structio-1.1.4/structio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 19:42:08.000000 structio-1.1.4/structio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-04-13 19:41:52.000000 structio-1.1.4/structio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 22:29:42.965475 structio-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-04-15 22:29:42.965475 structio-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-04-15 22:29:23.000000 structio-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-15 22:29:23.000000 structio-1.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 22:29:42.965475 structio-1.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 22:29:42.965475 structio-1.1.5/structio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-04-15 22:29:42.000000 structio-1.1.5/structio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-15 22:29:42.000000 structio-1.1.5/structio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 22:29:42.000000 structio-1.1.5/structio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 22:29:42.000000 structio-1.1.5/structio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11670 2023-04-15 22:29:23.000000 structio-1.1.5/structio.py
```

### Comparing `structio-1.1.4/PKG-INFO` & `structio-1.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structio
-Version: 1.1.4
+Version: 1.1.5
 Summary: A Library for unparsing, parsing, and editing binary files
 Project-URL: Homepage, https://github.com/lingeringwillx/StructIO
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 
 A small Python library based on the BytesIO object from the standard library, designed to make parsing and editing binary files easier.
 
@@ -108,33 +108,33 @@
 
 Convert bytes object *b* into a string.
 
 **pack_str(string)**
 
 Converts *string* into a bytes object.
 
-**unpack_cstr(b, start=0, ret_end=False)**
+**unpack_cstr(b, start=0, ret_len=False)**
 
-Convert bytes object *b* into a string up to the null termination. If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_end* is True, then a tuple is returned containing both the value and the end position of the type.
+Convert bytes object *b* into a string up to the null termination. If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_len* is True, then a tuple is returned containing both the value and the length of the type.
 
 **pack_cstr(string)**
 
 Converts *string* into a bytes object representing a null-terminated string.
 
-**unpack_pstr(b, numbytes, endian=None, start=0, ret_end=False)**
+**unpack_pstr(b, numbytes, endian=None, start=0, ret_len=False)**
 
-Converts bytes object *b* into a Pascal string. *numbytes* is used to specify how many bytes are used for the string's length in the object. The endian of the length of the string is specified with the *endian* argument. *b* will only be converted up to the length specified in the bytes object. If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_end* is True, then a tuple is returned containing both the value and the end position of the type.
+Converts bytes object *b* into a Pascal string. *numbytes* is used to specify how many bytes are used for the string's length in the object. The endian of the length of the string is specified with the *endian* argument. *b* will only be converted up to the length specified in the bytes object. If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_len* is True, then a tuple is returned containing both the value and the length of the type.
 
 **pack_pstr(string, numbytes, endian=None)**
 
 Converts *string* into a bytes object in the Pascal string format. *numbytes* is used to specify how many bytes are used for the string's length. The endian of the length of the string is specified with the *endian* argument.
 
-**unpack_7bint(b, start=0, ret_end=False)**
+**unpack_7bint(b, start=0, ret_len=False)**
 
-Converts bytes representing a 7 bit integer (Variable Length Quantity) into an integer.  If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_end* is True, then a tuple is returned containing both the value and the end position of the type.
+Converts bytes representing a 7 bit integer (Variable Length Quantity) into an integer.  If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_len* is True, then a tuple is returned containing both the value and the length of the type.
 
 **pack_7bint(number)**
 
 Converts *number* into a 7 bit integer.
 
 -----
 
@@ -319,46 +319,47 @@
 -----
 
 ### Extending StructIO
 
 You can add your own types by inheriting from the two base objects:
 
 ```python
+from structio import Struct, StructIO
+
 class ExtendedStruct(Struct):
-    def _get_7bstr_end(self, b, start=0):
-        length, int_end = self.unpack_7bint(b, start=0, ret_end=True)
-        return int_end + length
+    def _get_7bstr_len(self, b, start=0):
+        str_len, int_len = self.unpack_7bint(b, start, ret_len=True)
+        return int_len + str_len
         
-    def unpack_7bstr(self, b, start=0, ret_end=False):
-        length, int_end = self.unpack_7bint(b, start, ret_end=True)
-        str_end = int_end + length
-        string = self.unpack_str(b[int_end:str_end])
+    def unpack_7bstr(self, b, start=0, ret_len=False):
+        str_len, int_len = self.unpack_7bint(b, start, ret_len=True)
+        string = self.unpack_str(b[(start + int_len):(start + int_len + str_len)])
         
-        if ret_end:
-            return string, str_end
+        if ret_len:
+            return string, int_len + str_len
         else:
             return string
             
     def pack_7bstr(self, string):
         b = self.pack_str(string)
         return self.pack_7bint(len(b)) + b
         
 class ExtendedStructIO(StructIO):
     def __init__(self, b=b'', endian='little', struct=ExtendedStruct):
         super().__init__(b, endian, struct=struct)
         
     def read_7bstr(self):
-        string, end = self._struct.unpack_7bstr(self.getvalue(), start=self.tell(), ret_end=True)
-        self.seek(end)
+        string, length = self._struct.unpack_7bstr(self.getvalue(), start=self.tell(), ret_len=True)
+        self.seek(length, 1)
         return string
         
     def write_7bstr(self, string):
         return self.write(self._struct.pack_7bstr(string))
         
     def append_7bstr(self, string):
         return self.append(self._struct.pack_7bstr(string))
         
     def overwrite_7bstr(self, string):
         start = self.tell()
-        end = self._struct._get_7bstr_end(self.getvalue(), start)
-        return self.overwrite(start, end, self._struct.pack_7bstr(string))
+        length = self._struct._get_7bstr_len(self.getvalue(), start)
+        return self.overwrite(start, start + length, self._struct.pack_7bstr(string))
 ```
```

### Comparing `structio-1.1.4/README.md` & `structio-1.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -100,33 +100,33 @@
 
 Convert bytes object *b* into a string.
 
 **pack_str(string)**
 
 Converts *string* into a bytes object.
 
-**unpack_cstr(b, start=0, ret_end=False)**
+**unpack_cstr(b, start=0, ret_len=False)**
 
-Convert bytes object *b* into a string up to the null termination. If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_end* is True, then a tuple is returned containing both the value and the end position of the type.
+Convert bytes object *b* into a string up to the null termination. If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_len* is True, then a tuple is returned containing both the value and the length of the type.
 
 **pack_cstr(string)**
 
 Converts *string* into a bytes object representing a null-terminated string.
 
-**unpack_pstr(b, numbytes, endian=None, start=0, ret_end=False)**
+**unpack_pstr(b, numbytes, endian=None, start=0, ret_len=False)**
 
-Converts bytes object *b* into a Pascal string. *numbytes* is used to specify how many bytes are used for the string's length in the object. The endian of the length of the string is specified with the *endian* argument. *b* will only be converted up to the length specified in the bytes object. If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_end* is True, then a tuple is returned containing both the value and the end position of the type.
+Converts bytes object *b* into a Pascal string. *numbytes* is used to specify how many bytes are used for the string's length in the object. The endian of the length of the string is specified with the *endian* argument. *b* will only be converted up to the length specified in the bytes object. If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_len* is True, then a tuple is returned containing both the value and the length of the type.
 
 **pack_pstr(string, numbytes, endian=None)**
 
 Converts *string* into a bytes object in the Pascal string format. *numbytes* is used to specify how many bytes are used for the string's length. The endian of the length of the string is specified with the *endian* argument.
 
-**unpack_7bint(b, start=0, ret_end=False)**
+**unpack_7bint(b, start=0, ret_len=False)**
 
-Converts bytes representing a 7 bit integer (Variable Length Quantity) into an integer.  If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_end* is True, then a tuple is returned containing both the value and the end position of the type.
+Converts bytes representing a 7 bit integer (Variable Length Quantity) into an integer.  If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_len* is True, then a tuple is returned containing both the value and the length of the type.
 
 **pack_7bint(number)**
 
 Converts *number* into a 7 bit integer.
 
 -----
 
@@ -311,46 +311,47 @@
 -----
 
 ### Extending StructIO
 
 You can add your own types by inheriting from the two base objects:
 
 ```python
+from structio import Struct, StructIO
+
 class ExtendedStruct(Struct):
-    def _get_7bstr_end(self, b, start=0):
-        length, int_end = self.unpack_7bint(b, start=0, ret_end=True)
-        return int_end + length
+    def _get_7bstr_len(self, b, start=0):
+        str_len, int_len = self.unpack_7bint(b, start, ret_len=True)
+        return int_len + str_len
         
-    def unpack_7bstr(self, b, start=0, ret_end=False):
-        length, int_end = self.unpack_7bint(b, start, ret_end=True)
-        str_end = int_end + length
-        string = self.unpack_str(b[int_end:str_end])
+    def unpack_7bstr(self, b, start=0, ret_len=False):
+        str_len, int_len = self.unpack_7bint(b, start, ret_len=True)
+        string = self.unpack_str(b[(start + int_len):(start + int_len + str_len)])
         
-        if ret_end:
-            return string, str_end
+        if ret_len:
+            return string, int_len + str_len
         else:
             return string
             
     def pack_7bstr(self, string):
         b = self.pack_str(string)
         return self.pack_7bint(len(b)) + b
         
 class ExtendedStructIO(StructIO):
     def __init__(self, b=b'', endian='little', struct=ExtendedStruct):
         super().__init__(b, endian, struct=struct)
         
     def read_7bstr(self):
-        string, end = self._struct.unpack_7bstr(self.getvalue(), start=self.tell(), ret_end=True)
-        self.seek(end)
+        string, length = self._struct.unpack_7bstr(self.getvalue(), start=self.tell(), ret_len=True)
+        self.seek(length, 1)
         return string
         
     def write_7bstr(self, string):
         return self.write(self._struct.pack_7bstr(string))
         
     def append_7bstr(self, string):
         return self.append(self._struct.pack_7bstr(string))
         
     def overwrite_7bstr(self, string):
         start = self.tell()
-        end = self._struct._get_7bstr_end(self.getvalue(), start)
-        return self.overwrite(start, end, self._struct.pack_7bstr(string))
+        length = self._struct._get_7bstr_len(self.getvalue(), start)
+        return self.overwrite(start, start + length, self._struct.pack_7bstr(string))
 ```
```

### Comparing `structio-1.1.4/structio.egg-info/PKG-INFO` & `structio-1.1.5/structio.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structio
-Version: 1.1.4
+Version: 1.1.5
 Summary: A Library for unparsing, parsing, and editing binary files
 Project-URL: Homepage, https://github.com/lingeringwillx/StructIO
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 
 A small Python library based on the BytesIO object from the standard library, designed to make parsing and editing binary files easier.
 
@@ -108,33 +108,33 @@
 
 Convert bytes object *b* into a string.
 
 **pack_str(string)**
 
 Converts *string* into a bytes object.
 
-**unpack_cstr(b, start=0, ret_end=False)**
+**unpack_cstr(b, start=0, ret_len=False)**
 
-Convert bytes object *b* into a string up to the null termination. If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_end* is True, then a tuple is returned containing both the value and the end position of the type.
+Convert bytes object *b* into a string up to the null termination. If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_len* is True, then a tuple is returned containing both the value and the length of the type.
 
 **pack_cstr(string)**
 
 Converts *string* into a bytes object representing a null-terminated string.
 
-**unpack_pstr(b, numbytes, endian=None, start=0, ret_end=False)**
+**unpack_pstr(b, numbytes, endian=None, start=0, ret_len=False)**
 
-Converts bytes object *b* into a Pascal string. *numbytes* is used to specify how many bytes are used for the string's length in the object. The endian of the length of the string is specified with the *endian* argument. *b* will only be converted up to the length specified in the bytes object. If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_end* is True, then a tuple is returned containing both the value and the end position of the type.
+Converts bytes object *b* into a Pascal string. *numbytes* is used to specify how many bytes are used for the string's length in the object. The endian of the length of the string is specified with the *endian* argument. *b* will only be converted up to the length specified in the bytes object. If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_len* is True, then a tuple is returned containing both the value and the length of the type.
 
 **pack_pstr(string, numbytes, endian=None)**
 
 Converts *string* into a bytes object in the Pascal string format. *numbytes* is used to specify how many bytes are used for the string's length. The endian of the length of the string is specified with the *endian* argument.
 
-**unpack_7bint(b, start=0, ret_end=False)**
+**unpack_7bint(b, start=0, ret_len=False)**
 
-Converts bytes representing a 7 bit integer (Variable Length Quantity) into an integer.  If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_end* is True, then a tuple is returned containing both the value and the end position of the type.
+Converts bytes representing a 7 bit integer (Variable Length Quantity) into an integer.  If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_len* is True, then a tuple is returned containing both the value and the length of the type.
 
 **pack_7bint(number)**
 
 Converts *number* into a 7 bit integer.
 
 -----
 
@@ -319,46 +319,47 @@
 -----
 
 ### Extending StructIO
 
 You can add your own types by inheriting from the two base objects:
 
 ```python
+from structio import Struct, StructIO
+
 class ExtendedStruct(Struct):
-    def _get_7bstr_end(self, b, start=0):
-        length, int_end = self.unpack_7bint(b, start=0, ret_end=True)
-        return int_end + length
+    def _get_7bstr_len(self, b, start=0):
+        str_len, int_len = self.unpack_7bint(b, start, ret_len=True)
+        return int_len + str_len
         
-    def unpack_7bstr(self, b, start=0, ret_end=False):
-        length, int_end = self.unpack_7bint(b, start, ret_end=True)
-        str_end = int_end + length
-        string = self.unpack_str(b[int_end:str_end])
+    def unpack_7bstr(self, b, start=0, ret_len=False):
+        str_len, int_len = self.unpack_7bint(b, start, ret_len=True)
+        string = self.unpack_str(b[(start + int_len):(start + int_len + str_len)])
         
-        if ret_end:
-            return string, str_end
+        if ret_len:
+            return string, int_len + str_len
         else:
             return string
             
     def pack_7bstr(self, string):
         b = self.pack_str(string)
         return self.pack_7bint(len(b)) + b
         
 class ExtendedStructIO(StructIO):
     def __init__(self, b=b'', endian='little', struct=ExtendedStruct):
         super().__init__(b, endian, struct=struct)
         
     def read_7bstr(self):
-        string, end = self._struct.unpack_7bstr(self.getvalue(), start=self.tell(), ret_end=True)
-        self.seek(end)
+        string, length = self._struct.unpack_7bstr(self.getvalue(), start=self.tell(), ret_len=True)
+        self.seek(length, 1)
         return string
         
     def write_7bstr(self, string):
         return self.write(self._struct.pack_7bstr(string))
         
     def append_7bstr(self, string):
         return self.append(self._struct.pack_7bstr(string))
         
     def overwrite_7bstr(self, string):
         start = self.tell()
-        end = self._struct._get_7bstr_end(self.getvalue(), start)
-        return self.overwrite(start, end, self._struct.pack_7bstr(string))
+        length = self._struct._get_7bstr_len(self.getvalue(), start)
+        return self.overwrite(start, start + length, self._struct.pack_7bstr(string))
 ```
```

### Comparing `structio-1.1.4/structio.py` & `structio-1.1.5/structio.py`

 * *Files 13% similar despite different names*

```diff
@@ -61,73 +61,73 @@
         
     def unpack_str(self, b):
         return b.decode(self.encoding, errors=self.errors)
         
     def pack_str(self, string):
         return string.encode(self.encoding, errors=self.errors)
         
-    def _get_cstr_end(self, b, start=0):
+    def _get_cstr_len(self, b, start=0):
         end = b.find(b'\x00', start)
         
         if end == -1:
             raise ValueError('null termination not found')
             
-        return end + 1
+        return end - start + 1
         
-    def unpack_cstr(self, b, start=0, ret_end=False):
-        end = self._get_cstr_end(b, start)
-        string = self.unpack_str(b[start:(end - 1)])
+    def unpack_cstr(self, b, start=0, ret_len=False):
+        length = self._get_cstr_len(b, start)
+        string = self.unpack_str(b[start:(start + length - 1)])
         
-        if ret_end:
-            return string, end
+        if ret_len:
+            return string, length
         else:
             return string
             
     def pack_cstr(self, string):
         return self.pack_str(string) + b'\x00'
         
-    def _get_pstr_end(self, b, numbytes, endian=None, start=0):
-        return start + numbytes + self.unpack_int(b[start:(start + numbytes)], endian)
+    def _get_pstr_len(self, b, numbytes, endian=None, start=0):
+        return numbytes + self.unpack_int(b[start:(start + numbytes)], endian)
         
-    def unpack_pstr(self, b, numbytes, endian=None, start=0, ret_end=False):
-        end = self._get_pstr_end(b, numbytes, endian, start)
-        string = self.unpack_str(b[(start + numbytes):end])
+    def unpack_pstr(self, b, numbytes, endian=None, start=0, ret_len=False):
+        length = self._get_pstr_len(b, numbytes, endian, start)
+        string = self.unpack_str(b[(start + numbytes):(start + length)])
         
-        if ret_end:
-            return string, end
+        if ret_len:
+            return string, length
         else:
             return string
             
     def pack_pstr(self, string, numbytes, endian=None):
         b = self.pack_str(string)
         return self.pack_int(len(b), numbytes, endian) + b
         
-    def _get_7bint_end(self, b, start=0):
+    def _get_7bint_len(self, b, start=0):
         i = 0
-        while b[start + i] & 0b10000000 != 0:
+        while b[start + i] > 127:
             i += 1
             
-        return start + i + 1
+        return i + 1
         
-    def unpack_7bint(self, b, start=0, ret_end=False):
+    def unpack_7bint(self, b, start=0, ret_len=False):
         number = 0
         i = 0
         
         byte = b[start + i]
-        while byte & 0b10000000 != 0:
+        while byte > 127:
             number |= (byte & 0b01111111) << (7 * i)
             i += 1
             
             byte = b[start + i]
             
         number |= byte << (7 * i)
-        end = start + i + 1
+        length = i + 1
         
-        if ret_end:
-            return number, end
+        if ret_len:
+            return number, length
         else:
             return number
             
     def pack_7bint(self, number):
         b = bytearray()
         
         while number > 127:
@@ -293,53 +293,53 @@
         return self.append(self._struct.pack_str(string))
         
     def overwrite_str(self, string, length):
         start = self.tell()
         return self.overwrite(start, start + length, self._struct.pack_str(string))
         
     def read_cstr(self):
-        value, end = self._struct.unpack_cstr(self.getvalue(), start=self.tell(), ret_end=True)
-        self.seek(end)
+        value, length = self._struct.unpack_cstr(self.getvalue(), start=self.tell(), ret_len=True)
+        self.seek(length, 1)
         return value
         
     def write_cstr(self, string):
         return self.write(self._struct.pack_cstr(string))
         
     def append_cstr(self, string):
         return self.append(self._struct.pack_cstr(string))
         
     def overwrite_cstr(self, string):
         start = self.tell()
-        end = self._struct._get_cstr_end(self.getvalue(), start=start)
-        return self.overwrite(start, end, self._struct.pack_cstr(string))
+        length = self._struct._get_cstr_len(self.getvalue(), start=start)
+        return self.overwrite(start, start + length, self._struct.pack_cstr(string))
         
     def read_pstr(self, numbytes, endian=None):
-        value, end = self._struct.unpack_pstr(self.getvalue(), numbytes, endian, start=self.tell(), ret_end=True)
-        self.seek(end)
+        value, length = self._struct.unpack_pstr(self.getvalue(), numbytes, endian, start=self.tell(), ret_len=True)
+        self.seek(length, 1)
         return value
         
     def write_pstr(self, string, numbytes, endian=None):
         return self.write(self._struct.pack_pstr(string, numbytes, endian))
         
     def append_pstr(self, string, numbytes, endian=None):
         return self.append(self._struct.pack_pstr(string, numbytes, endian))
         
     def overwrite_pstr(self, string, numbytes, endian=None):
         start = self.tell()
-        end = self._struct._get_pstr_end(self.getvalue(), numbytes, endian, start=start)
-        return self.overwrite(start, end, self._struct.pack_pstr(string, numbytes, endian))
+        length = self._struct._get_pstr_len(self.getvalue(), numbytes, endian, start=start)
+        return self.overwrite(start, start + length, self._struct.pack_pstr(string, numbytes, endian))
         
     def read_7bint(self):
-        value, end = self._struct.unpack_7bint(self.getvalue(), start=self.tell(), ret_end=True)
-        self.seek(end)
+        value, length = self._struct.unpack_7bint(self.getvalue(), start=self.tell(), ret_len=True)
+        self.seek(length, 1)
         return value
         
     def write_7bint(self, number):
         return self.write(self._struct.pack_7bint(number))
         
     def append_7bint(self, number):
         return self.append(self._struct.pack_7bint(number))
         
     def overwrite_7bint(self, number):
         start = self.tell()
-        end = self._struct._get_7bint_end(self.getvalue(), start=start)
-        return self.overwrite(start, end, self._struct.pack_7bint(number))
+        length = self._struct._get_7bint_len(self.getvalue(), start=start)
+        return self.overwrite(start, start + length, self._struct.pack_7bint(number))
```

