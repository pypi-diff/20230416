# Comparing `tmp/danielutils-0.8.0.tar.gz` & `tmp/danielutils-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danielutils-0.8.0.tar", last modified: Tue Apr 11 11:33:08 2023, max compression
+gzip compressed data, was "danielutils-0.8.1.tar", last modified: Sun Apr 16 09:32:56 2023, max compression
```

## Comparing `danielutils-0.8.0.tar` & `danielutils-0.8.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 11:33:08.969068 danielutils-0.8.0/
--rw-rw-rw-   0        0        0      834 2023-04-11 11:33:08.968062 danielutils-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-04-11 11:33:08.000000 danielutils-0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 11:33:08.938437 danielutils-0.8.0/danielutils/
-drwxrwxrwx   0        0        0        0 2023-04-11 11:33:08.959109 danielutils-0.8.0/danielutils/Classes/
--rw-rw-rw-   0        0        0      103 2023-04-02 21:16:20.000000 danielutils-0.8.0/danielutils/Classes/Convenience.py
--rw-rw-rw-   0        0        0     1694 2023-04-02 21:17:25.000000 danielutils-0.8.0/danielutils/Classes/DataStructures.py
--rw-rw-rw-   0        0        0     3569 2023-04-03 13:58:33.000000 danielutils-0.8.0/danielutils/Classes/TypedBuiltins.py
--rw-rw-rw-   0        0        0      117 2023-03-30 21:30:39.000000 danielutils-0.8.0/danielutils/Classes/__init__.py
--rw-rw-rw-   0        0        0      904 2023-03-30 21:22:39.000000 danielutils-0.8.0/danielutils/Classes/frange.py
--rw-rw-rw-   0        0        0     2159 2023-04-03 13:58:33.000000 danielutils-0.8.0/danielutils/Colors.py
-drwxrwxrwx   0        0        0        0 2023-04-11 11:33:08.960561 danielutils-0.8.0/danielutils/Conversions/
--rw-rw-rw-   0        0        0     2032 2023-04-03 13:58:33.000000 danielutils-0.8.0/danielutils/Conversions/MainConversions.py
-drwxrwxrwx   0        0        0        0 2023-04-11 11:33:08.963162 danielutils-0.8.0/danielutils/Conversions/SpecializedConversions/
--rw-rw-rw-   0        0        0       46 2022-10-14 16:36:49.000000 danielutils-0.8.0/danielutils/Conversions/SpecializedConversions/__init__.py
--rw-rw-rw-   0        0        0      454 2022-10-14 16:32:03.000000 danielutils-0.8.0/danielutils/Conversions/SpecializedConversions/to_hex.py
--rw-rw-rw-   0        0        0      389 2022-10-28 08:08:26.000000 danielutils-0.8.0/danielutils/Conversions/SpecializedConversions/to_int.py
--rw-rw-rw-   0        0        0       71 2022-10-14 16:31:17.000000 danielutils-0.8.0/danielutils/Conversions/__init__.py
--rw-rw-rw-   0        0        0      308 2023-04-03 13:58:33.000000 danielutils-0.8.0/danielutils/Data.py
-drwxrwxrwx   0        0        0        0 2023-04-11 11:33:08.964565 danielutils-0.8.0/danielutils/DataStructures/
--rw-rw-rw-   0        0        0     2587 2023-04-03 13:58:33.000000 danielutils-0.8.0/danielutils/DataStructures/Graph.py
--rw-rw-rw-   0        0        0     2653 2023-04-03 13:58:33.000000 danielutils-0.8.0/danielutils/DataStructures/MarkovChain.py
--rw-rw-rw-   0        0        0       50 2022-10-28 07:57:32.000000 danielutils-0.8.0/danielutils/DataStructures/__init__.py
--rw-rw-rw-   0        0        0    19685 2023-04-03 14:10:10.000000 danielutils-0.8.0/danielutils/Decorators.py
--rw-rw-rw-   0        0        0     1122 2023-04-03 14:02:27.000000 danielutils-0.8.0/danielutils/Exceptions.py
--rw-rw-rw-   0        0        0     8193 2023-04-03 11:53:26.000000 danielutils-0.8.0/danielutils/Functions.py
--rw-rw-rw-   0        0        0     7484 2023-04-03 20:39:45.000000 danielutils-0.8.0/danielutils/IO.py
--rw-rw-rw-   0        0        0     1324 2023-04-03 13:58:33.000000 danielutils-0.8.0/danielutils/Internet.py
-drwxrwxrwx   0        0        0        0 2023-04-11 11:33:08.967059 danielutils-0.8.0/danielutils/Math/
--rw-rw-rw-   0        0        0     6036 2022-10-28 20:26:06.000000 danielutils-0.8.0/danielutils/Math/Constants.py
--rw-rw-rw-   0        0        0      237 2023-04-03 13:58:33.000000 danielutils-0.8.0/danielutils/Math/Functions.py
--rw-rw-rw-   0        0        0      860 2023-04-03 18:56:27.000000 danielutils-0.8.0/danielutils/Math/MathPrint.py
--rw-rw-rw-   0        0        0     6485 2023-04-02 21:11:12.000000 danielutils-0.8.0/danielutils/Math/MathSymbols.py
--rw-rw-rw-   0        0        0       80 2023-04-03 18:56:40.000000 danielutils-0.8.0/danielutils/Math/__init__.py
--rw-rw-rw-   0        0        0     1006 2023-01-12 01:01:37.000000 danielutils-0.8.0/danielutils/Path.py
--rw-rw-rw-   0        0        0     2681 2023-04-11 11:31:36.000000 danielutils-0.8.0/danielutils/Print.py
--rw-rw-rw-   0        0        0     1357 2023-01-05 22:01:09.000000 danielutils-0.8.0/danielutils/Serialization.py
--rw-rw-rw-   0        0        0     4907 2023-04-03 13:58:33.000000 danielutils-0.8.0/danielutils/System.py
--rw-rw-rw-   0        0        0     6785 2023-04-03 13:58:33.000000 danielutils-0.8.0/danielutils/Testing.py
--rw-rw-rw-   0        0        0     3183 2023-04-03 13:58:33.000000 danielutils-0.8.0/danielutils/Text.py
--rw-rw-rw-   0        0        0      330 2022-10-28 08:07:45.000000 danielutils-0.8.0/danielutils/Threading.py
--rw-rw-rw-   0        0        0      251 2022-10-07 22:49:20.000000 danielutils-0.8.0/danielutils/Time.py
--rw-rw-rw-   0        0        0      649 2023-01-18 20:34:53.000000 danielutils-0.8.0/danielutils/Typing.py
--rw-rw-rw-   0        0        0     1248 2023-04-02 14:10:39.000000 danielutils-0.8.0/danielutils/Windows.py
--rw-rw-rw-   0        0        0      480 2023-04-03 18:57:22.000000 danielutils-0.8.0/danielutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 11:33:08.956109 danielutils-0.8.0/danielutils.egg-info/
--rw-rw-rw-   0        0        0      834 2023-04-11 11:33:08.000000 danielutils-0.8.0/danielutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1309 2023-04-11 11:33:08.000000 danielutils-0.8.0/danielutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 11:33:08.000000 danielutils-0.8.0/danielutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-11 11:33:08.000000 danielutils-0.8.0/danielutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-11 11:33:08.000000 danielutils-0.8.0/danielutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      728 2023-04-11 11:33:08.000000 danielutils-0.8.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-11 11:33:08.969068 danielutils-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1340 2023-04-11 11:33:08.000000 danielutils-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 09:32:56.416437 danielutils-0.8.1/
+-rw-rw-rw-   0        0        0      939 2023-04-16 09:32:56.416437 danielutils-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-04-16 09:32:55.000000 danielutils-0.8.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 09:32:56.385174 danielutils-0.8.1/danielutils/
+drwxrwxrwx   0        0        0        0 2023-04-16 09:32:56.400813 danielutils-0.8.1/danielutils/Classes/
+-rw-rw-rw-   0        0        0      103 2023-04-11 14:27:34.000000 danielutils-0.8.1/danielutils/Classes/Convenience.py
+-rw-rw-rw-   0        0        0     1694 2023-04-11 14:27:34.000000 danielutils-0.8.1/danielutils/Classes/DataStructures.py
+-rw-rw-rw-   0        0        0     3489 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/Classes/TypedBuiltins.py
+-rw-rw-rw-   0        0        0      117 2023-04-11 14:27:34.000000 danielutils-0.8.1/danielutils/Classes/__init__.py
+-rw-rw-rw-   0        0        0      904 2023-04-11 14:27:34.000000 danielutils-0.8.1/danielutils/Classes/frange.py
+-rw-rw-rw-   0        0        0     1968 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/Colors.py
+drwxrwxrwx   0        0        0        0 2023-04-16 09:32:56.400813 danielutils-0.8.1/danielutils/Conversions/
+-rw-rw-rw-   0        0        0     1797 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/Conversions/MainConversions.py
+drwxrwxrwx   0        0        0        0 2023-04-16 09:32:56.400813 danielutils-0.8.1/danielutils/Conversions/SpecializedConversions/
+-rw-rw-rw-   0        0        0       46 2022-10-25 07:33:55.000000 danielutils-0.8.1/danielutils/Conversions/SpecializedConversions/__init__.py
+-rw-rw-rw-   0        0        0      454 2022-10-25 07:33:55.000000 danielutils-0.8.1/danielutils/Conversions/SpecializedConversions/to_hex.py
+-rw-rw-rw-   0        0        0      389 2022-10-31 15:04:29.000000 danielutils-0.8.1/danielutils/Conversions/SpecializedConversions/to_int.py
+-rw-rw-rw-   0        0        0       71 2022-10-25 07:33:55.000000 danielutils-0.8.1/danielutils/Conversions/__init__.py
+-rw-rw-rw-   0        0        0      270 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/Data.py
+drwxrwxrwx   0        0        0        0 2023-04-16 09:32:56.416437 danielutils-0.8.1/danielutils/DataStructures/
+-rw-rw-rw-   0        0        0     2503 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/DataStructures/Graph.py
+-rw-rw-rw-   0        0        0     2564 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/DataStructures/MarkovChain.py
+-rw-rw-rw-   0        0        0       50 2022-10-26 11:35:28.000000 danielutils-0.8.1/danielutils/DataStructures/__init__.py
+-rw-rw-rw-   0        0        0    19824 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/Decorators.py
+-rw-rw-rw-   0        0        0     1122 2023-04-11 14:27:34.000000 danielutils-0.8.1/danielutils/Exceptions.py
+-rw-rw-rw-   0        0        0     8193 2023-04-11 14:27:34.000000 danielutils-0.8.1/danielutils/Functions.py
+-rw-rw-rw-   0        0        0     7503 2023-04-16 09:29:30.000000 danielutils-0.8.1/danielutils/IO.py
+-rw-rw-rw-   0        0        0     1259 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/Internet.py
+drwxrwxrwx   0        0        0        0 2023-04-16 09:32:56.416437 danielutils-0.8.1/danielutils/Math/
+-rw-rw-rw-   0        0        0     6036 2022-10-31 15:04:29.000000 danielutils-0.8.1/danielutils/Math/Constants.py
+-rw-rw-rw-   0        0        0      205 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/Math/Functions.py
+-rw-rw-rw-   0        0        0      860 2023-04-11 14:27:34.000000 danielutils-0.8.1/danielutils/Math/MathPrint.py
+-rw-rw-rw-   0        0        0     6485 2023-04-11 14:27:34.000000 danielutils-0.8.1/danielutils/Math/MathSymbols.py
+-rw-rw-rw-   0        0        0       80 2023-04-11 14:27:34.000000 danielutils-0.8.1/danielutils/Math/__init__.py
+-rw-rw-rw-   0        0        0     1006 2023-01-19 11:44:27.000000 danielutils-0.8.1/danielutils/Path.py
+-rw-rw-rw-   0        0        0     2686 2023-04-11 14:28:24.000000 danielutils-0.8.1/danielutils/Print.py
+-rw-rw-rw-   0        0        0     1357 2023-01-11 17:24:17.000000 danielutils-0.8.1/danielutils/Serialization.py
+-rw-rw-rw-   0        0        0     4801 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/System.py
+-rw-rw-rw-   0        0        0     6699 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/Testing.py
+-rw-rw-rw-   0        0        0     2895 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/Text.py
+-rw-rw-rw-   0        0        0      137 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/Threading.py
+-rw-rw-rw-   0        0        0      426 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/Time.py
+-rw-rw-rw-   0        0        0      649 2023-01-19 11:44:27.000000 danielutils-0.8.1/danielutils/Typing.py
+-rw-rw-rw-   0        0        0     1248 2023-04-11 14:27:34.000000 danielutils-0.8.1/danielutils/Windows.py
+-rw-rw-rw-   0        0        0      480 2023-04-11 14:27:34.000000 danielutils-0.8.1/danielutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 09:32:56.400813 danielutils-0.8.1/danielutils.egg-info/
+-rw-rw-rw-   0        0        0      939 2023-04-16 09:32:56.000000 danielutils-0.8.1/danielutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1309 2023-04-16 09:32:56.000000 danielutils-0.8.1/danielutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 09:32:56.000000 danielutils-0.8.1/danielutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-16 09:32:56.000000 danielutils-0.8.1/danielutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-16 09:32:56.000000 danielutils-0.8.1/danielutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      728 2023-04-16 09:32:55.000000 danielutils-0.8.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 09:32:56.416437 danielutils-0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     1340 2023-04-16 09:32:55.000000 danielutils-0.8.1/setup.py
```

### Comparing `danielutils-0.8.0/PKG-INFO` & `danielutils-0.8.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.8.0
+Version: 0.8.1
 Summary: A python utils library for things I find useful
 Home-page: https://github.com/danielnachumdev/danielutils
 Author: danielnachumdev
-Author-email: <danielnachumdev@gmail.com>
+Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
+Project-URL: Homepage, https://github.com/danielnachumdev/danielutils
+Project-URL: Bug Tracker, https://github.com/danielnachumdev/danielutils/issues
 Keywords: functions,decorators,methods
 Platform: All
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.10.5
 Description-Content-Type: text/markdown
 
-# danielutils v=0.8.0
+# danielutils v=0.8.1
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
-
```

### Comparing `danielutils-0.8.0/danielutils/Classes/DataStructures.py` & `danielutils-0.8.1/danielutils/Classes/DataStructures.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.0/danielutils/Classes/TypedBuiltins.py` & `danielutils-0.8.1/danielutils/Classes/TypedBuiltins.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 from ..Typing import Any, Union, Iterable
-from ..Decorators import validate_explicit, overload
+from ..Decorators import validate, overload
 from ..Functions import isoftype
 
 
 class tlist(list):
     """tlist is same as builtin python list but with added type restriction
 
     Args:
         type (type): the allowed type, can be nested type
         iterable (Iterable, optional): the value to create the tlist from. Defaults to None.
     """
 
     def get_type_error_msg(self, v: Any):
         return f"A value is of the wrong type:\n'{v}' is of type '{type(v)}' but should be of type '{self.type}'"
 
-    @validate_explicit(None, [type, type(Union[Any, Any])], Iterable)
-    def __init__(self, type: type, iterable: Iterable = None):
+    @validate
+    def __init__(self: Any, type: type, iterable: Iterable = None):
         """_summary_
 
         Args:
             type (type): the allowed type, can be nested type
         ietrable (Iterable, optional): the value to create the tlist from. Defaults to None.
 
         Raises:
@@ -39,16 +39,16 @@
         super()[index] = value
 
     def append(self, value: Any) -> None:
         if not isoftype(value, self.type):
             raise TypeError(self.get_type_error_msg(value))
         super().append(value)
 
-    @validate_explicit(None, Iterable)
-    def extend(self, iterable: Iterable) -> None:
+    @validate
+    def extend(self: Any, iterable: Iterable) -> None:
         for v in iterable:
             self.append(v)
 
     def __add__(self, other) -> tlist:
         pass
```

### Comparing `danielutils-0.8.0/danielutils/Classes/frange.py` & `danielutils-0.8.1/danielutils/Classes/frange.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.0/danielutils/Colors.py` & `danielutils-0.8.1/danielutils/Colors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-from .Decorators import validate_explicit
+from .Decorators import validate
 
 
 class ColoredText:
-    __rgb_validation = [int, lambda v: 0 <=
-                        v <= 255, "rgb value must be in [0,255]"]
-
     @staticmethod
-    @validate_explicit(__rgb_validation, __rgb_validation, __rgb_validation, str)
+    @validate
     def from_rgb(r: int, g: int, b: int, text: str):
         return f"\033[38;2;{r};{g};{b}m{text}\033[38;2;255;255;255m"
 
     @staticmethod
     def green(text: str):
         return ColoredText.from_rgb(0, 255, 0, text)
```

### Comparing `danielutils-0.8.0/danielutils/Conversions/MainConversions.py` & `danielutils-0.8.1/danielutils/Conversions/MainConversions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-from ..Decorators import validate_explicit, overload
+from ..Decorators import validate
 
 
-@validate_explicit([str, lambda s:len(s) == 1, "len(s) must be 1"])
+@validate
 def char_to_int(c: str) -> int:
     """convert char to its representing int value
 
     Args:
         c (str): char to convert
 
     Returns:
         int: int value
     """
     return ord(c)
 
 
-@validate_explicit(int)
+@validate
 def int_to_char(num: int) -> str:
     """convert int to its corresponding char
 
     Args:
         num (int): number to convert
 
     Returns:
         str: result character
     """
     return chr(num)
 
 
-@validate_explicit(str)
+@validate
 def hex_to_char(h: str) -> str:
     """convert hex number to char
 
     Args:
         h (str): number to convert
 
     Returns:
         str: result char
     """
     return int_to_char(hex_to_dec(h))
 
 
-@validate_explicit(str)
+@validate
 def hex_to_dec(h: str) -> int:
     """convert hex to dec
 
     Args:
         h (str): converts base 16 to base 10
 
     Returns:
         int: decimal value for hex number
     """
     return int(h, 16)
 
 
-@validate_explicit([str, lambda s:len(s) == 1, "len(s) must be 1"])
+@validate
 def char_to_hex(c: str) -> str:
     """convert char to hex
 
     Args:
         c (str): char to convert
 
     Returns:
         str: hex representation
     """
     return int_to_hex(char_to_int(c))
 
 
-@validate_explicit(int)
+@validate
 def dec_to_hex(num: int) -> str:
     """convert decimal number to hex
 
     Args:
         num (int): number to convert
 
     Returns:
         str: _description_
     """
     return int_to_hex(num)
 
 
-@validate_explicit(int)
+@validate
 def int_to_hex(num: int) -> str:
     return hex(num)
 
 
-@validate_explicit(bytes)
+@validate
 def bytes_to_str(b: bytes) -> str:
     return b.decode("utf-8")
 
 
-@validate_explicit(str)
+@validate
 def str_to_bytes(s: str) -> bytes:
     return bytes(s, encoding='utf-8')
 
 
 __all__ = [
     "char_to_int",
     "int_to_char",
```

### Comparing `danielutils-0.8.0/danielutils/DataStructures/Graph.py` & `danielutils-0.8.1/danielutils/DataStructures/Graph.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from __future__ import annotations
 from ..Typing import Any, Sequence, Union, TypeVar
-from ..Decorators import overload, validate_explicit
+from ..Decorators import overload, validate
 
 
 class GraphNode:
     def __init__(self, value: Any):
         self.value = value
 
     def __str__(self) -> str:
         return f"GN(V={self.value})"
 
     def __repr__(self) -> str:
         return str(self)
 
 
 class Connection:
-    @validate_explicit(None, GraphNode, GraphNode, Any)
+    @validate
     def __init__(self, node1: GraphNode, node2: GraphNode, weight: Any):
         self.node1 = node1
         self.node2 = node2
         self.weight = weight
 
 
 class Graph:
     @classmethod
-    @validate_explicit(None, list, list, list)
+    @validate
     def from_lists(cls, values: list[Any], connections: list[list[int]]) -> Graph:
         nodes = [GraphNode(v) for v in values]
         parsed_connections = []
         for i1, i_connections in enumerate(connections):
             for i2 in i_connections:
                 parsed_connections.append(Connection(nodes[i1], nodes[i2]))
         return cls(
```

### Comparing `danielutils-0.8.0/danielutils/DataStructures/MarkovChain.py` & `danielutils-0.8.1/danielutils/DataStructures/MarkovChain.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..Decorators import validate_explicit, overload
+from ..Decorators import validate, overload
 from ..Typing import Any, Iterable, Union
 import random
 INDEX_INDEX = 0
 OCCUPANCE_INDEX = 1
 
 
 class MarkovNode:
@@ -46,23 +46,23 @@
         return str(self)
 
     def has_children(self) -> bool:
         return len(self.occurrences) > 0
 
 
 class MarkovChain:
-    @validate_explicit(None, list[MarkovNode])
+    @validate
     def __init__(self, nodes: list[MarkovNode] = None) -> None:
         self.nodes = nodes if nodes is not None else []
 
-    @validate_explicit(None, int)
+    @validate
     def __getitem__(self, index: int) -> MarkovNode:
         return self.nodes[index]
 
-    @validate_explicit(None, MarkovNode)
+    @validate
     def append(self, node: MarkovNode) -> None:
         self.nodes.append(node)
 
     def __iter__(self) -> Iterable:
         return iter(self.nodes)
 
     def __str__(self) -> str:
```

### Comparing `danielutils-0.8.0/danielutils/Decorators.py` & `danielutils-0.8.1/danielutils/Decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,20 @@
 import functools
 import threading
 import inspect
 from .Functions import areoneof, isoneof, isoneof_strict, isoftype
 from .Exceptions import *
 
 
-def __get_function_return_type(func) -> type:
-    return_annotation = inspect.signature(func).return_annotation
-    if "inspect._empty" in str(return_annotation) or return_annotation is None:
-        return type(None)
-    return return_annotation
-
-
 def validate(func: Callable) -> Callable:
     """A decorator that validates the annotations and types of the arguments and return value of a function.
 
+        * 'None' is allowed as default value for everything
+        * Because of their use in classes, the generally accepted keywords 'self' and 'cls' are not validated to not break intellisense when using 'Any'
+
     Args:
         func (Callable): The function to be decorated.
 
     Raises:
         TypeError: if the decorated object is nto a Callable
         EmptyAnnotationException: If an argument is not annotated.
         InvalidDefaultValueException: If an argument's default value is not of the annotated type.
@@ -31,23 +27,27 @@
     """
     if not isinstance(func, Callable):
         raise TypeError("The validate decorator must only decorate a function")
     func_name = f"{func.__module__}.{func.__qualname__}"
     # get the signature of the function
     signature = inspect.signature(func)
     for arg_name, arg_param in signature.parameters.items():
-        arg_type = arg_param.annotation
-        # check if an annotation is missing
-        if arg_type == inspect.Parameter.empty:
-            raise EmptyAnnotationException(
-                f"In {func_name}, argument '{arg_name}' is not annotated")
+        if arg_name not in {"self", "cls"}:
+            arg_type = arg_param.annotation
+            # check if an annotation is missing
+            if arg_type == inspect.Parameter.empty:
+                raise EmptyAnnotationException(
+                    f"In {func_name}, argument '{arg_name}' is not annotated")
 
         # check if the argument has a default value
         default_value = signature.parameters[arg_name].default
         if default_value != inspect.Parameter.empty:
+            # allow everything to be set to None as default
+            if default_value is None:
+                continue
             # if it does, check the type of the default value
             if not isoftype(default_value, arg_type):
                 raise InvalidDefaultValueException(
                     f"In {func_name}, argument '{arg_name}'s default value is annotated as {arg_type} but got '{default_value}' which is {type(default_value)}")
 
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
@@ -62,126 +62,127 @@
                 raise ValidationException(
                     f"In {func_name}, argument '{variable_name}' is annotated as {annotated_type} but got '{variable_value}' which is {type(variable_value)}")
 
         # call the function
         result = func(*args, **kwargs)
 
         # check the return type
-        return_type = __get_function_return_type(func)
+        return_type = type(None) if ("inspect._empty" in str(signature.return_annotation)
+                                     or signature.return_annotation is None) else signature.return_annotation
         if not isoftype(result, return_type):
             raise InvalidReturnValueException(
                 f"In function {func_name}, the return type is annotated as {return_type} but got '{result}' which is {type(result)}")
         return result
     return wrapper
 
 
-__validation_set = set()
-__validation_instantiation_rule = dict()
-
+# __validation_set = set()
+# __validation_instantiation_rule = dict()
 
-def __validate_type(func: Callable, v: Any, T: type, validation_func: Callable[[Any], bool] = isoftype, msg: str = None) -> None:
-    if not validation_func(v, T):
-        raise ValidationTypeError(
-            msg or f"In {func.__module__}.{func.__qualname__}(...)\nThe argument is: '{ v.__qualname__ if hasattr(v, '__qualname__') else v}'\nIt has the type of '{type(v)}'\nIt is marked as type(s): '{T}'")
-
-
-def __validate_condition(func: Callable, v: Any, constraint: Callable[[Any], bool], msg: str = None) -> None:
-    if not constraint(v):
-        raise ValidationValueError(
-            msg or f"In {func.__module__}.{func.__qualname__}(...)\nThe argument '{str(v)}' has failed provided constraint\nConstraint in {constraint.__module__}.{constraint.__qualname__}")
-
-
-def __validate_arg(func: Callable, curr_arg: Any, curr_inner_arg: Any) -> None:
-    if isoneof(curr_arg, [list, tuple]):
-        # multiple type only:
-        if areoneof(curr_arg, [type]):
-            __validate_type(func, curr_inner_arg, curr_arg, isoneof)
-
-        else:  # maybe with condition:
-            class_type, constraint = curr_arg[0], curr_arg[1]
-
-            # Type validation
-            if isoneof(class_type, [list, tuple]):
-                __validate_type(func, curr_inner_arg, class_type, isoneof)
-            else:
-                __validate_type(func, curr_inner_arg, class_type, isinstance)
-
-            # constraints validation
-            if constraint is not None:
-                message = curr_arg[2] if len(curr_arg) > 2 else None
-                __validate_condition(func, curr_inner_arg, constraint, message)
-    else:
-        __validate_type(func, curr_inner_arg, curr_arg)
-
-
-def validate_explicit(*args, return_type=None, can_instantiate_multiple_times: bool = False) -> Callable:
-    """validate decorator
-
-        Is passed types of variables to perform type checking over\n
-        The arguments must be passed in the same order\n
-
-    for each parameter respectively you can choose one of four options:\n
-        1. None - to skip\n
-        2. Type - a type to check \n
-        3. Sequence of Type to check if the type is contained in the sequence\n
-        4. Sequence that contains three arguments:\n
-            4.1 a Type or Sequence[Type]\n
-            4.2 a function to call on argument\n
-            4.3 a str to display in a ValueError iff the condition from 4.2 fails\n
-    In addition you can use keyword 'return_type' for the returned value same as specified in 1,2,3
-    """
-    from .Exceptions import ValidationDuplicationError, ValidationTypeError, ValidationValueError, ValidationReturnTypeError
-
-    def deco(func: Callable) -> Callable:
-        if not isinstance(func, Callable):
-            raise ValueError("validate decorator must decorate a callable")
-        global __validation_set, __validation_instantiation_rule
-        func_id = f"{func.__module__}.{func.__qualname__}"
-
-        if func_id not in __validation_instantiation_rule:
-            __validation_instantiation_rule[func_id] = can_instantiate_multiple_times
-        assert can_instantiate_multiple_times == __validation_instantiation_rule[
-            func_id], "can't change instantiation status on runtime"
-
-        if func_id not in __validation_set:
-            __validation_set.add(func_id)
-        else:
-            if not __validation_instantiation_rule[func_id]:
-                raise ValidationDuplicationError(
-                    "validate decorator is being used on two functions in the same module with the same name\nmaybe use @overload instead")
 
-        @ functools.wraps(func)
-        def wrapper(*inner_args, **inner_kwargs) -> Any:
-            for i in range(min(len(args), len(inner_args))):
-                if args[i] is not None:
-                    __validate_arg(func, args[i], inner_args[i])
-            res = func(*inner_args, **inner_kwargs)
-            if return_type is not None:
-                msg = f"In {func.__module__}.{func.__qualname__}(...)\nThe returned value is: '{ res.__qualname__ if hasattr(res, '__qualname__') else res}'\nIt has the type of '{type(res)}'\nIt is marked as type(s): '{return_type}'"
-                __validate_type(func, res, return_type, msg=msg)
-            return res
-        return wrapper
-    return deco
+# def __validate_type(func: Callable, v: Any, T: type, validation_func: Callable[[Any], bool] = isoftype, msg: str = None) -> None:
+#     if not validation_func(v, T):
+#         raise ValidationTypeError(
+#             msg or f"In {func.__module__}.{func.__qualname__}(...)\nThe argument is: '{ v.__qualname__ if hasattr(v, '__qualname__') else v}'\nIt has the type of '{type(v)}'\nIt is marked as type(s): '{T}'")
+
+
+# def __validate_condition(func: Callable, v: Any, constraint: Callable[[Any], bool], msg: str = None) -> None:
+#     if not constraint(v):
+#         raise ValidationValueError(
+#             msg or f"In {func.__module__}.{func.__qualname__}(...)\nThe argument '{str(v)}' has failed provided constraint\nConstraint in {constraint.__module__}.{constraint.__qualname__}")
+
+
+# def __validate_arg(func: Callable, curr_arg: Any, curr_inner_arg: Any) -> None:
+#     if isoneof(curr_arg, [list, tuple]):
+#         # multiple type only:
+#         if areoneof(curr_arg, [type]):
+#             __validate_type(func, curr_inner_arg, curr_arg, isoneof)
+
+#         else:  # maybe with condition:
+#             class_type, constraint = curr_arg[0], curr_arg[1]
+
+#             # Type validation
+#             if isoneof(class_type, [list, tuple]):
+#                 __validate_type(func, curr_inner_arg, class_type, isoneof)
+#             else:
+#                 __validate_type(func, curr_inner_arg, class_type, isinstance)
+
+#             # constraints validation
+#             if constraint is not None:
+#                 message = curr_arg[2] if len(curr_arg) > 2 else None
+#                 __validate_condition(func, curr_inner_arg, constraint, message)
+#     else:
+#         __validate_type(func, curr_inner_arg, curr_arg)
+
+
+# def validate_explicit(*args, return_type=None, can_instantiate_multiple_times: bool = False) -> Callable:
+#     """validate decorator
+
+#         Is passed types of variables to perform type checking over\n
+#         The arguments must be passed in the same order\n
+
+#     for each parameter respectively you can choose one of four options:\n
+#         1. None - to skip\n
+#         2. Type - a type to check \n
+#         3. Sequence of Type to check if the type is contained in the sequence\n
+#         4. Sequence that contains three arguments:\n
+#             4.1 a Type or Sequence[Type]\n
+#             4.2 a function to call on argument\n
+#             4.3 a str to display in a ValueError iff the condition from 4.2 fails\n
+#     In addition you can use keyword 'return_type' for the returned value same as specified in 1,2,3
+#     """
+#     from .Exceptions import ValidationDuplicationError, ValidationTypeError, ValidationValueError, ValidationReturnTypeError
+
+#     def deco(func: Callable) -> Callable:
+#         if not isinstance(func, Callable):
+#             raise ValueError("validate decorator must decorate a callable")
+#         global __validation_set, __validation_instantiation_rule
+#         func_id = f"{func.__module__}.{func.__qualname__}"
+
+#         if func_id not in __validation_instantiation_rule:
+#             __validation_instantiation_rule[func_id] = can_instantiate_multiple_times
+#         assert can_instantiate_multiple_times == __validation_instantiation_rule[
+#             func_id], "can't change instantiation status on runtime"
+
+#         if func_id not in __validation_set:
+#             __validation_set.add(func_id)
+#         else:
+#             if not __validation_instantiation_rule[func_id]:
+#                 raise ValidationDuplicationError(
+#                     "validate decorator is being used on two functions in the same module with the same name\nmaybe use @overload instead")
+
+#         @ functools.wraps(func)
+#         def wrapper(*inner_args, **inner_kwargs) -> Any:
+#             for i in range(min(len(args), len(inner_args))):
+#                 if args[i] is not None:
+#                     __validate_arg(func, args[i], inner_args[i])
+#             res = func(*inner_args, **inner_kwargs)
+#             if return_type is not None:
+#                 msg = f"In {func.__module__}.{func.__qualname__}(...)\nThe returned value is: '{ res.__qualname__ if hasattr(res, '__qualname__') else res}'\nIt has the type of '{type(res)}'\nIt is marked as type(s): '{return_type}'"
+#                 __validate_type(func, res, return_type, msg=msg)
+#             return res
+#         return wrapper
+#     return deco
 
 
-@ validate_explicit(Callable)
+@validate
 def NotImplemented(func: Callable) -> Callable:
     """decorator to mark function as not implemented for development purposes
 
     Args:
         func (Callable): the function to decorate
     """
     @ functools.wraps(func)
     def wrapper(*args, **kwargs) -> Any:
         raise NotImplementedError(
             f"As marked by the developer {func.__module__}.{func.__qualname__} is not implemented yet..")
     return wrapper
 
 
-@ validate_explicit(Callable)
+@validate
 def PartiallyImplemented(func: Callable) -> Callable:
     """decorator to mark function as not fully implemented for development purposes
 
     Args:
         func (Callable): the function to decorate
     """
     from .Colors import warning
@@ -190,15 +191,15 @@
     def wrapper(*args, **kwargs) -> Any:
         warning(
             f"As marked by the developer, {func.__module__}.{func.__qualname__} may not be fully implemented and might not work properly")
         return func(*args, **kwargs)
     return wrapper
 
 
-@ validate_explicit(Callable)
+@validate
 def memo(func: Callable) -> Callable:
     """decorator to memorize function calls in order to improve performance by using more memory
 
     Args:
         func (Callable): function to memorize
     """
     cache: dict[tuple, Any] = {}
@@ -299,33 +300,31 @@
             raise OverloadNotFound(
                 f"function {func.__module__}.{func.__qualname__} is not overloaded with {[type(v) for v in args]}")
 
         return wrapper
     return deco
 
 
-@ validate_explicit(Callable)
+@validate
 def abstractmethod(func: Callable) -> Callable:
     """A decorator to mark a function to be 'pure virtual' / 'abstract'
 
     Args:
         func (Callable): the function to mark
 
     Raises:
         NotImplementedError: the error that will rise when the marked function will be called if not overridden in a derived class
     """
     @ functools.wraps(func)
     def wrapper(*args, **kwargs):
         raise NotImplementedError(
-            f"{func.__module__}.{func.__qualname__} MUST be overrided in a child class")
+            f"{func.__module__}.{func.__qualname__} MUST be overridden in a child class")
     return wrapper
 
 
-purevirtual = abstractmethod
-
 # __virtualization_tables = dict()
 
 
 # @NotImplemented
 # def virtual(func: Callable) -> Callable:
 #     def wrapper(*args, **kwargs):
 #         return func(*args, **kwargs)
@@ -335,68 +334,67 @@
 # @NotImplemented
 # def override(func: Callable) -> Callable:
 #     def wrapper(*args, **kwargs):
 #         return func(*args, **kwargs)
 #     return wrapper
 
 
-@ PartiallyImplemented
-@ validate_explicit([str, Callable])
-def deprecate(obj: Union[str, Callable] = None) -> Callable:
-    """decorator to mark function as deprecated
-
-    Args:
-        obj (Union[str, None, Callable], optional): Defaults to None.
-
-        Can operate in two configurations:\n
-        1. obj is the function that you want to deprecate\n
-        \t@deprecate\n
-        \tdef foo(...):\n
-        \t\t...\n\n
-        2. obj is an advise message\n
-        \t@deprecate("instead use ...")\n
-        \tdef foo(...):
-        \t\t...
-    """
-    from .Colors import warning
-    # if callable(obj):
-    if isinstance(obj, Callable):
-        @ functools.wraps(obj)
-        def wrapper(*args, **kwargs) -> Any:
-            warning(
-                f"As marked by the developer, {obj.__module__}.{obj.__qualname__} is deprecated")
-            return obj(*args, **kwargs)
-        return wrapper
-
-    def deco(func: Callable) -> Callable:
-        @ functools.wraps(func)
-        def wrapper(*args, **kwargs) -> Any:
-            warning(
-                f"As marked by the developer, {func.__module__}.{func.__qualname__} is deprecated")
-            if obj:
-                print(obj)
-            return func(*args, **kwargs)
-        return wrapper
-    return deco
+# @ PartiallyImplemented
+# @validate
+# def deprecate(obj:  Callable) -> Callable:
+#     """decorator to mark function as deprecated
+
+#     Args:
+#         obj (Union[str, None, Callable], optional): Defaults to None.
+
+#         Can operate in two configurations:\n
+#         1. obj is the function that you want to deprecate\n
+#         \t@deprecate\n
+#         \tdef foo(...):\n
+#         \t\t...\n\n
+#         2. obj is an advise message\n
+#         \t@deprecate("instead use ...")\n
+#         \tdef foo(...):
+#         \t\t...
+#     """
+#     from .Colors import warning
+#     # if callable(obj):
+#     if isinstance(obj, Callable):
+#         @ functools.wraps(obj)
+#         def wrapper(*args, **kwargs) -> Any:
+#             warning(
+#                 f"As marked by the developer, {obj.__module__}.{obj.__qualname__} is deprecated")
+#             return obj(*args, **kwargs)
+#         return wrapper
+
+#     def deco(func: Callable) -> Callable:
+#         @ functools.wraps(func)
+#         def wrapper(*args, **kwargs) -> Any:
+#             warning(
+#                 f"As marked by the developer, {func.__module__}.{func.__qualname__} is deprecated")
+#             if obj:
+#                 print(obj)
+#             return func(*args, **kwargs)
+#         return wrapper
+#     return deco
 
 
-@ validate_explicit(Callable)
-def atomic(func):
-    import threading
+@validate
+def atomic(func: Callable) -> Callable:
     lock = threading.Lock()
 
     @ functools.wraps(func)
     def wrapper(*args, **kwargs):
         with lock:
             return func(*args, **kwargs)
     return wrapper
 
 
-@ validate_explicit([int, lambda d: d > 0, "limit_recursion's max_depth must be a positive integer"], None, bool)
-def limit_recursion(max_depth: int, return_value=None, quiet: bool = True):
+@validate
+def limit_recursion(max_depth: int, return_value: Any = None, quiet: bool = True):
     """decorator to limit recursion of functions
 
     Args:
         max_depth (int): max recursion depth which is allowed for this function
         return_value (_type_, optional): The value to return when the limit is reached. Defaults to None.
             if is None, will return the last (args, kwargs)
         quiet (bool, optional): whether to print a warning message. Defaults to True.
@@ -422,15 +420,15 @@
                     return return_value
                 return args, kwargs
             return func(*args, **kwargs)
         return wrapper
     return deco
 
 
-@validate_explicit([int, float])
+@validate
 def timeout(timeout: int | float) -> Callable:
     """A decorator to limit runtime for a function
 
     Args:
         timeout (int | float): allowed runtime duration
 
     Raises:
@@ -465,15 +463,15 @@
             if isinstance(res[0], BaseException):
                 raise res[0]
             return res[0]
         return wrapper
     return timeout_deco
 
 
-@validate_explicit(Callable, Callable)
+@validate
 def attach(before: Callable = None, after: Callable = None) -> Callable:
     if before is None and after is None:
         raise ValueError("You must supply at least one function")
 
     def attach_deco(func: Callable):
         if not isinstance(func, Callable):
             raise ValueError("attach must decorate a function")
@@ -488,23 +486,21 @@
             return res
         return wrapper
     return attach_deco
 
 
 __all__ = [
     "validate",
-    "validate_explicit",
     "NotImplemented",
     "PartiallyImplemented",
     "memo",
     "overload",
     "abstractmethod",
-    "purevirtual",
     # "virtual",
     # "override",
-    "deprecate",
+    # "deprecate",
     "atomic",
     "limit_recursion",
     "timeout",
     "attach"
 
 ]
```

### Comparing `danielutils-0.8.0/danielutils/Exceptions.py` & `danielutils-0.8.1/danielutils/Exceptions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.0/danielutils/Functions.py` & `danielutils-0.8.1/danielutils/Functions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.0/danielutils/IO.py` & `danielutils-0.8.1/danielutils/IO.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 from typing import IO
 import shutil
 import os
-from .Decorators import validate_explicit
+from .Decorators import validate
 from typing import Union
 from pathlib import Path
 
 
-@validate_explicit(str, list)
+@validate
 def write_to_file(path: str, lines: Union[list[str], list[bytes]], write_bytes: bool = False) -> None:
     """clear and then write data to file
 
     Args:
         path (str): path of file
         lines (list[str]): data to write
     """
@@ -26,65 +26,65 @@
     except Exception as e:
         if isinstance(e, TypeError):
             raise Exception(
                 "'lines' contains a 'bytes' object.\nTo use with bytes use: write_bytes = True ")
         raise e
 
 
-@validate_explicit(str)
+@validate
 def path_exists(path: str) -> bool:
     """checks whether a path exists
 
     Args:
         path (str): path to check
 
     Returns:
         bool: result of check
     """
     return os.path.exists(path)
 
 
-@validate_explicit(str)
+@validate
 def file_exists(path: str) -> bool:
     """checks whether a file exists at specified path
 
     Args:
         path (str): path to check
 
     Returns:
         bool: will return true iff the path exists and it is a path to a file
     """
     return path_exists(path) and is_file(path)
 
 
-@validate_explicit(str)
+@validate
 def directory_exists(path: str) -> bool:
     """checks whether a directory exists at specified path
 
     Args:
         path (str): path to check
 
     Returns:
         bool: will return true iff the path exists and it is a path to a directory
     """
     return path_exists(path) and is_directory(path)
 
 
-@validate_explicit(str)
+@validate
 def delete_file(path: str) -> None:
     """deletes a file if it exists
 
     Args:
         path (str): path of file
     """
     if file_exists(path):
         os.remove(path)
 
 
-@validate_explicit(str, bool)
+@validate
 def read_file(path: str, read_bytes: bool = False) -> list[str]:
     """read all lines from a file
 
     Args:
         path (str): the path to the file
 
     Returns:
@@ -100,119 +100,119 @@
     except Exception as e:
         if isinstance(e, UnicodeDecodeError):
             raise Exception(
                 f"Can't read byte in file.\nTo use with bytes use: read_bytes = True ")
         raise e
 
 
-@validate_explicit(str)
+@validate
 def is_file(path: str) -> bool:
     """return whether a path represents a file
 
     Args:
         path (str): path to check
     """
     return os.path.isfile(path)
 
 
-@validate_explicit(str)
+@validate
 def is_directory(path: str) -> bool:
     """return whether a path represents a directory
 
     Args:
         path (str): path to check
     """
     return os.path.isdir(path)
 
 
-@validate_explicit(str)
+@validate
 def get_files(path: str) -> list[str]:
     """return a list of names of all files inside specified directory
 
     Args:
         path (str): directory
 
     Returns:
         list[str]: all files
     """
     files_and_directories = get_files_and_directories(path)
     return list(
         filter(lambda name: is_file(f"{path}\\{name}"), files_and_directories))
 
 
-@validate_explicit(str)
+@validate
 def get_files_and_directories(path: str) -> list[str]:
     """get a list of all files and directories in specified path
 
     Args:
         path (str): path to check
 
     Returns:
         list[str]: all files and directories
     """
     return os.listdir(path)
 
 
-@validate_explicit(str)
+@validate
 def get_directories(path: str) -> list[str]:
     """get all directories in specified path
 
     Args:
         path (str): path to check
 
     Returns:
         list[str]: all directories
     """
     files_and_directories = get_files_and_directories(path)
     return list(
         filter(lambda name: is_directory(f"{path}\\{name}"), files_and_directories))
 
 
-@ validate_explicit(str)
+@ validate
 def delete_directory(path: str) -> None:
     """delete a directory and all its contents
 
     Args:
         path (str): _description_
     """
     if is_directory(path):
         clear_directory(path)
         os.rmdir(path)
 
 
-@validate_explicit(str)
+@validate
 def clear_directory(path: str) -> None:
     for file in get_files(path):
         delete_file(f"{path}\\{file}")
     for dir in get_directories(path):
         delete_directory(f"{path}\\{dir}")
 
 
-@validate_explicit(str)
+@validate
 def create_directory(path: str) -> None:
     """create a directory at the specified path if it doesn't already exists
 
     Args:
         path (str): the path to create a directory at
     """
     if not directory_exists(path):
         os.makedirs(path)
 
 
-@validate_explicit(str, str)
+@validate
 def get_file_type_from_directory(path: str, file_type: str) -> list[str]:
     return list(
         filter(
             lambda name: Path(f"{path}\\{name}").suffix == file_type,
             get_files(path)
         )
     )
 
 
-@validate_explicit(str, str)
+@validate
 def get_file_type_from_directory_recursively(path: str, file_type: str):
     res = []
     for dir in get_directories(path):
         res.extend(f"{dir}\\{v}" for v in get_file_type_from_directory_recursively(
             f"{path}\\{dir}", file_type))
     res.extend(list(
         filter(
@@ -248,23 +248,29 @@
 
 
 def copy_directory(src: str, dest: str) -> None:
     shutil.copy(src, dest)
 
 
 class IndentedWriter:
-    def __init__(self, output_stream: IO, indent_char: str = "\t"):
+    def __init__(self, output_stream: IO = None, indent_char: str = "\t"):
         self.indent_level = 0
         self.output_stream: IO = output_stream
         self.indent_char = indent_char
 
     def write(self, *args, sep=" ", end="\n"):
+        if self.output_stream is None:
+            raise ValueError(
+                "Can't write to an empty stream. the stream must not be None either by set_stream or by initialization")
         self.output_stream.write(
             self.indent_level*self.indent_char + sep.join(args)+end)
 
+    def set_stream(self, stream):
+        self.output_stream = stream
+
     def indent(self):
         self.indent_level += 1
 
     def undent(self):
         self.indent_level = max(0, self.indent_level-1)
```

### Comparing `danielutils-0.8.0/danielutils/Internet.py` & `danielutils-0.8.1/danielutils/Internet.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import urllib.request
 import urllib.parse
 from urllib.parse import urlparse
 import urllib
-from .Decorators import validate_explicit
+from .Decorators import validate
 
 
 def prettify_html(html: str) -> str:
     return html
 
 
-@validate_explicit(str)
+@validate
 def get_html(url: str) -> str:
     user_agent = 'Mozilla/5.0 (Windows; U; Windows NT 5.1; en-US; rv:1.9.0.7) Gecko/2009021910 Firefox/3.0.7'
     headers = {'User-Agent': user_agent, }
     req = urllib.request.Request(url, headers=headers)
     html = urllib.request.urlopen(req).read().decode('UTF-8')
     # return bs4(html, 'html.parser').prettify()
     return html
 
 
-@validate_explicit(str)
+@validate
 def get_url_details(url: str) -> tuple[str, str, str, str, str]:
     scheme, netloc, path, params, query, fragment = urlparse(url)
     return scheme, netloc, path, params, query, fragment
 
 
-@validate_explicit(str)
+@validate
 def url_encode(s: str) -> str:
     return urllib.parse.quote(s)
 
 
-@validate_explicit(str)
+@validate
 def url_decode(s: str) -> str:
     return urllib.parse.unquote_plus(s)
 
 
 def get_elements(html: str, tag: str) -> list[str]:
     from bs4 import BeautifulSoup as bs4
     return [str(v) for v in bs4(html, 'html.parser').find_all(tag)]
```

### Comparing `danielutils-0.8.0/danielutils/Math/Constants.py` & `danielutils-0.8.1/danielutils/Math/Constants.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.0/danielutils/Math/MathPrint.py` & `danielutils-0.8.1/danielutils/Math/MathPrint.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.0/danielutils/Math/MathSymbols.py` & `danielutils-0.8.1/danielutils/Math/MathSymbols.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.0/danielutils/Path.py` & `danielutils-0.8.1/danielutils/Path.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.0/danielutils/Print.py` & `danielutils-0.8.1/danielutils/Print.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         *args: The arguments to print.
         sep (str, optional): The separator to use between the arguments. Defaults to " ".
         end (str, optional): The string to append to the end of the printed arguments. Defaults to "\n".
 
     Returns:
         None
     """
-    print(sep.join(args)+end)
+    print(*args, sep=sep, end=end)
 
 
 @atomic
 def bprint(*args, sep=" ", end="\n", stream=sys.stdout) -> None:
     """A function that writes a string representation of the given arguments to the specified stream.
 
     Args:
```

### Comparing `danielutils-0.8.0/danielutils/Serialization.py` & `danielutils-0.8.1/danielutils/Serialization.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.0/danielutils/System.py` & `danielutils-0.8.1/danielutils/System.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from math import inf
-from .Decorators import overload, timeout, validate_explicit
+from .Decorators import overload, timeout, validate
 from .Typing import IO
 from .Exceptions import TimeoutError
 from .Conversions import str_to_bytes
 from .Functions import areoneof
 from pathlib import Path
 import subprocess
 import time
@@ -31,33 +31,36 @@
     for i, arg in enumerate(args):
         if Path(args[i]).is_file() or Path(args[i]).is_dir():
             args = (*args[:i], f"\"{arg}\"", *args[i+1:])
     res = subprocess.run(" ".join(args), shell=shell, capture_output=True)
     return res.returncode, res.stdout, res.stderr
 
 
-@validate_explicit([int, float])
-def sleep(seconds: int | float):
+@validate
+def sleep(seconds: int | float) -> None:
     """make current thread sleep
 
     Args:
         seconds (float): number of seconds to sleep
+
+    Returns:
+        None
     """
     time.sleep(seconds)
 
 
 def __acm_write(*args, p: subprocess.Popen, sep=" ", end="\n") -> None:
     b_args = str_to_bytes(sep).join(str_to_bytes(v) for v in args)
     b_end = str_to_bytes(end)
     p.stdin.write(b_args+b_end)
     p.stdin.flush()
 
 
-@validate_explicit(str, [list, lambda l:areoneof(l, [str]), "inputs must be a list of strings"], [int, float], bool, bool, None, None,)
-def acm(command: str, inputs: list[str] = None, i_timeout: float = 0.01, shell: bool = False, use_write_helper: bool = True, cwd=None, env=None) -> tuple[int, list[bytes] | None, list[bytes] | None]:
+@validate
+def acm(command: str, inputs: list[str] = None, i_timeout: float = 0.01, shell: bool = False, use_write_helper: bool = True, cwd: str = None, env: str = None) -> tuple[int, list[bytes] | None, list[bytes] | None]:
     """Advanced command
 
     Args:
         command (str): The command to execute\n
         inputs (list[str]): the inputs to give to the program from the command. Defaults to None.\n
         i_timeout (float, optional): An individual timeout for every step of the execution. Defaults to 0.01.\n
         cwd (?, optional): Current working directory. Defaults to None.\n
```

### Comparing `danielutils-0.8.0/danielutils/Testing.py` & `danielutils-0.8.1/danielutils/Testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Sequence, Union, Any
 from collections.abc import Callable
-from .Decorators import validate_explicit
+from .Decorators import validate
 from .Colors import ColoredText
 from .Classes import DisablePytestDiscovery
 from .Functions import isoneof
 from .IO import read_file, write_to_file, file_exists
 from pathlib import Path
 import re
 
@@ -69,21 +69,21 @@
             else:
                 Test.failed(msg)
             return has_passed
 
 
 # @pytest.mark.filterwarnings("ignore:api v1")
 class TestFactory(DisablePytestDiscovery):
-    @validate_explicit(None, Callable, bool)
+    @validate
     def __init__(self, func: Callable, verbose: bool = False):
         self.func = func
         self.tests: list[Test] = []
         self.verbose = verbose
 
-    @validate_explicit(None, Test)
+    @validate
     def add_test(self, test: Test):
         self.tests.append(test)
         return self
 
     def add_tests(self, tests: Sequence[Test]):
         self.tests.extend(tests)
         return self
@@ -101,15 +101,15 @@
         print(f"PASSED {pass_count} / {count}".center(20, " ").center(40, "="))
         return pass_count == count
 
     def execute(self) -> bool:
         return self()
 
 
-@validate_explicit(str, str, bool)
+@validate
 def create_test_file(path: str, output_folder: str = None, overwrite: bool = False):
     filename = Path(path).stem
     output_path = f"./test_{filename.lower()}.py"
     if output_folder is not None:
         output_path = f"{output_folder}/test_{filename.lower()}.py"
     if output_folder is not None and file_exists(output_path) and not overwrite:
         return
```

### Comparing `danielutils-0.8.0/danielutils/Text.py` & `danielutils-0.8.1/danielutils/Text.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 # -*- coding: utf-8 -*-
-from .Decorators import validate_explicit
+from .Decorators import validate
 from .Functions import check_foreach
 from .Typing import Union, TypeGuard
 HEBREW_LETTERS = ['\u05D0', '\u2135', '\uFB21', '\uFB2E', '\uFB2F', '\uFB30', '\uFB4F', '\u05D1', '\u2136', '\uFB31', '\uFB4C', '\u05D2', '\u2137', '\uFB32', '\u05D3', '\u2138', '\uFB22', '\uFB33', '\u05D4', '\uFB23', '\uFB34', '\u05D5', '\uFB4B', '\uFB35', '\u05F0', '\u05F1', '\u05D6', '\uFB36', '\u05D7', '\u05D8', '\uFB38', '\u05D9', '\uFB1D', '\uFB39', '\u05EF', '\u05F2', '\uFB1F', '\u05DB', '\uFB24',
                   '\u05DA', '\uFB3B', '\uFB3A', '\uFB4D', '\u05DC', '\uFB25', '\uFB3C', '\u05DE', '\uFB26', '\u05DD', '\uFB3E', '\u05E0', '\u05DF', '\uFB40', '\u05E1', '\uFB41', '\u05E2', '\uFB20', '\u05E4', '\u05E3', '\uFB44', '\uFB43', '\uFB4E', '\u05E6', '\u05E5', '\uFB46', '\u05E7', '\uFB47', '\u05E8', '\uFB27', '\uFB48', '\u05E9', '\uFB2B', '\uFB2A', '\uFB49', '\uFB2D', '\uFB2C', '\u05EA', '\uFB28', '\uFB4A']
 HEBREW_LETTERS_DEC = [ord(v) for v in HEBREW_LETTERS]
 HEBREW_LETTERS_HEX = [hex(v) for v in HEBREW_LETTERS_DEC]
 ENGLISH_LETTERS = [chr(v) for v in range(65, 91)]+[chr(v)
                                                    for v in range(97, 123)]
 ENGLISH_LETTERS_DEC = [ord(v) for v in ENGLISH_LETTERS]
 ENGLISH_LETTERS_HEX = [hex(v) for v in ENGLISH_LETTERS_DEC]
 
 
-@validate_explicit(str, return_type=bool)
+@validate
 def is_english(s: str) -> TypeGuard[str]:
     return check_foreach(s, lambda c: c in ENGLISH_LETTERS)
     # try:
     #     s.encode(encoding='utf-8').decode('ascii')
     # except UnicodeDecodeError:
     #     return False
     # else:
     #     return True
 
 
-@validate_explicit(str, return_type=bool)
+@validate
 def is_str_number(text: str) -> bool:
     return text.isnumeric()
 
 
-@validate_explicit([int, float])
+@validate
 def is_int(num: Union[int, float]) -> TypeGuard[int]:
     if isinstance(num, int):
         return True
 
     return int(num) == num
 
 
-@validate_explicit(str, return_type=bool)
+@validate
 def is_float(text: str) -> TypeGuard[float]:
     try:
         float(text)
         return True
     except ValueError:
         return False
 
 
-@validate_explicit(str, return_type=bool)
+@validate
 def is_number(text: str) -> bool:
     return is_float(text)
 
 
-@validate_explicit(str, return_type=bool)
+@validate
 def is_hebrew(text: str) -> TypeGuard[str]:
     return check_foreach(text, lambda c: c in HEBREW_LETTERS)
 
 
-@validate_explicit(str, return_type=bool)
+@validate
 def is_binary(text: str) -> bool:
     return check_foreach(text, lambda c: c in [0, 1])
 
 
-@validate_explicit(str, return_type=bool)
+@validate
 def is_decimal(text: str) -> bool:
     return check_foreach(text, lambda c: c in range(10))
 
 
-@validate_explicit(str, return_type=bool)
+@validate
 def is_hex(h: str) -> bool:
     try:
         int(h, 16)
         return True
     except ValueError:
         return False
```

### Comparing `danielutils-0.8.0/danielutils/Typing.py` & `danielutils-0.8.1/danielutils/Typing.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.0/danielutils/Windows.py` & `danielutils-0.8.1/danielutils/Windows.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.0/danielutils.egg-info/PKG-INFO` & `danielutils-0.8.1/danielutils.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.8.0
+Version: 0.8.1
 Summary: A python utils library for things I find useful
 Home-page: https://github.com/danielnachumdev/danielutils
 Author: danielnachumdev
-Author-email: <danielnachumdev@gmail.com>
+Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
+Project-URL: Homepage, https://github.com/danielnachumdev/danielutils
+Project-URL: Bug Tracker, https://github.com/danielnachumdev/danielutils/issues
 Keywords: functions,decorators,methods
 Platform: All
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.10.5
 Description-Content-Type: text/markdown
 
-# danielutils v=0.8.0
+# danielutils v=0.8.1
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
-
```

### Comparing `danielutils-0.8.0/danielutils.egg-info/SOURCES.txt` & `danielutils-0.8.1/danielutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.0/pyproject.toml` & `danielutils-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "danielutils"
-version = "0.8.0"
+version = "0.8.1"
 authors = [
   { name="danielnachumdev", email="danielnachumdev@gmail.com" },
 ]
 description = "A python utils library for things I find useful"
 readme = "README.md"
 requires-python = ">=3.10.5"
 classifiers = [
```

### Comparing `danielutils-0.8.0/setup.py` & `danielutils-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 def read_file(path: str) -> "list[str]":
     with codecs.open(path, 'r', 'utf-8') as f:
         return [l.strip() for l in f.readlines()]
 
 
 README_PATH = 'README.md'
 DESCRIPTION = 'A python utils library for things I find useful'
-VERSION = "0.8.0"
+VERSION = "0.8.1"
 LONG_DESCRIPTION = '\n'.join(read_file(README_PATH))
 setup(
     name="danielutils",
     version=VERSION,
     author="danielnachumdev",
     author_email="<danielnachumdev@gmail.com>",
     description=DESCRIPTION,
```

