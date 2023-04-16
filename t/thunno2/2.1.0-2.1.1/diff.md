# Comparing `tmp/thunno2-2.1.0.tar.gz` & `tmp/thunno2-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunno2-2.1.0.tar", last modified: Sat Apr 15 17:56:38 2023, max compression
+gzip compressed data, was "thunno2-2.1.1.tar", last modified: Sun Apr 16 13:01:09 2023, max compression
```

## Comparing `thunno2-2.1.0.tar` & `thunno2-2.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-15 17:56:38.680179 thunno2-2.1.0/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-15 17:56:38.680056 thunno2-2.1.0/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)       38 2023-04-15 17:56:38.680237 thunno2-2.1.0/setup.cfg
--rw-r--r--   0 nayak      (501) staff       (20)     1354 2023-04-12 09:58:27.000000 thunno2-2.1.0/setup.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-15 17:56:38.679022 thunno2-2.1.0/thunno2/
--rw-r--r--   0 nayak      (501) staff       (20)       22 2023-04-03 16:07:07.000000 thunno2-2.1.0/thunno2/__init__.py
--rw-r--r--   0 nayak      (501) staff       (20)     1412 2023-04-03 16:27:37.000000 thunno2-2.1.0/thunno2/codepage.py
--rw-r--r--   0 nayak      (501) staff       (20)    46735 2023-04-15 17:10:04.000000 thunno2-2.1.0/thunno2/commands.py
--rw-r--r--   0 nayak      (501) staff       (20)     2971 2023-04-15 15:28:56.000000 thunno2-2.1.0/thunno2/constants.py
--rw-r--r--   0 nayak      (501) staff       (20)   245513 2023-04-14 08:28:09.000000 thunno2-2.1.0/thunno2/dictionary.py
--rw-r--r--   0 nayak      (501) staff       (20)     6066 2023-04-14 19:12:18.000000 thunno2-2.1.0/thunno2/flags.py
--rw-r--r--   0 nayak      (501) staff       (20)    48088 2023-04-15 17:10:04.000000 thunno2-2.1.0/thunno2/helpers.py
--rw-r--r--   0 nayak      (501) staff       (20)    25876 2023-04-15 15:28:56.000000 thunno2-2.1.0/thunno2/interpreter.py
--rw-r--r--   0 nayak      (501) staff       (20)    22512 2023-04-15 17:55:44.000000 thunno2-2.1.0/thunno2/lexer.py
--rw-r--r--   0 nayak      (501) staff       (20)     1675 2023-04-15 17:55:44.000000 thunno2-2.1.0/thunno2/run.py
--rw-r--r--   0 nayak      (501) staff       (20)    62680 2023-04-15 17:10:04.000000 thunno2-2.1.0/thunno2/tests.py
--rw-r--r--   0 nayak      (501) staff       (20)     3274 2023-04-15 17:55:44.000000 thunno2-2.1.0/thunno2/tokens.py
--rw-r--r--   0 nayak      (501) staff       (20)       97 2023-04-15 17:55:44.000000 thunno2-2.1.0/thunno2/version.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-15 17:56:38.679848 thunno2-2.1.0/thunno2.egg-info/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-15 17:56:38.000000 thunno2-2.1.0/thunno2.egg-info/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)      414 2023-04-15 17:56:38.000000 thunno2-2.1.0/thunno2.egg-info/SOURCES.txt
--rw-r--r--   0 nayak      (501) staff       (20)        1 2023-04-15 17:56:38.000000 thunno2-2.1.0/thunno2.egg-info/dependency_links.txt
--rw-r--r--   0 nayak      (501) staff       (20)       54 2023-04-15 17:56:38.000000 thunno2-2.1.0/thunno2.egg-info/entry_points.txt
--rw-r--r--   0 nayak      (501) staff       (20)        8 2023-04-15 17:56:38.000000 thunno2-2.1.0/thunno2.egg-info/top_level.txt
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-16 13:01:09.413257 thunno2-2.1.1/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-16 13:01:09.413145 thunno2-2.1.1/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)       38 2023-04-16 13:01:09.413291 thunno2-2.1.1/setup.cfg
+-rw-r--r--   0 nayak      (501) staff       (20)     1354 2023-04-12 09:58:27.000000 thunno2-2.1.1/setup.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-16 13:01:09.412470 thunno2-2.1.1/thunno2/
+-rw-r--r--   0 nayak      (501) staff       (20)       22 2023-04-03 16:07:07.000000 thunno2-2.1.1/thunno2/__init__.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1412 2023-04-03 16:27:37.000000 thunno2-2.1.1/thunno2/codepage.py
+-rw-r--r--   0 nayak      (501) staff       (20)    46724 2023-04-16 13:00:29.000000 thunno2-2.1.1/thunno2/commands.py
+-rw-r--r--   0 nayak      (501) staff       (20)     2971 2023-04-15 15:28:56.000000 thunno2-2.1.1/thunno2/constants.py
+-rw-r--r--   0 nayak      (501) staff       (20)   245513 2023-04-14 08:28:09.000000 thunno2-2.1.1/thunno2/dictionary.py
+-rw-r--r--   0 nayak      (501) staff       (20)     6066 2023-04-14 19:12:18.000000 thunno2-2.1.1/thunno2/flags.py
+-rw-r--r--   0 nayak      (501) staff       (20)    48173 2023-04-16 11:06:19.000000 thunno2-2.1.1/thunno2/helpers.py
+-rw-r--r--   0 nayak      (501) staff       (20)    25876 2023-04-15 15:28:56.000000 thunno2-2.1.1/thunno2/interpreter.py
+-rw-r--r--   0 nayak      (501) staff       (20)    22512 2023-04-15 17:55:44.000000 thunno2-2.1.1/thunno2/lexer.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1675 2023-04-15 17:55:44.000000 thunno2-2.1.1/thunno2/run.py
+-rw-r--r--   0 nayak      (501) staff       (20)    62659 2023-04-16 13:00:29.000000 thunno2-2.1.1/thunno2/tests.py
+-rw-r--r--   0 nayak      (501) staff       (20)     3274 2023-04-15 17:55:44.000000 thunno2-2.1.1/thunno2/tokens.py
+-rw-r--r--   0 nayak      (501) staff       (20)       97 2023-04-16 13:00:43.000000 thunno2-2.1.1/thunno2/version.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-16 13:01:09.412998 thunno2-2.1.1/thunno2.egg-info/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-16 13:01:09.000000 thunno2-2.1.1/thunno2.egg-info/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)      414 2023-04-16 13:01:09.000000 thunno2-2.1.1/thunno2.egg-info/SOURCES.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        1 2023-04-16 13:01:09.000000 thunno2-2.1.1/thunno2.egg-info/dependency_links.txt
+-rw-r--r--   0 nayak      (501) staff       (20)       54 2023-04-16 13:01:09.000000 thunno2-2.1.1/thunno2.egg-info/entry_points.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        8 2023-04-16 13:01:09.000000 thunno2-2.1.1/thunno2.egg-info/top_level.txt
```

### Comparing `thunno2-2.1.0/PKG-INFO` & `thunno2-2.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.1.0
+Version: 2.1.1
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.0.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.1.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `thunno2-2.1.0/setup.py` & `thunno2-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.0/thunno2/codepage.py` & `thunno2-2.1.1/thunno2/codepage.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.0/thunno2/commands.py` & `thunno2-2.1.1/thunno2/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -526,15 +526,15 @@
     'U': Overload(1, {
         Number: uniquify_num,
         str: uniquify_str,
         list: uniquify_lst
     }, 0, ('uniquify',)),
 
     'V': Overload(1, {
-        Number: indices_where_truthy_num,
+        Number: round,
         str: rot_13,
         list: indices_where_truthy
     }, 0, ('where_truthy', 'rot13')),
 
     'W': Overload(1, {
         Any: wrap
     }, 0, ('wrap',)),
@@ -658,17 +658,17 @@
 
     'v': Overload(3, {
         (Any[0], Any[0], list): list_replace,
         (Any[0], Any[0], Any[0]): string_replace
     }, 0, ('replace',)),
 
     'w': Overload(1, {
-        Number: round,
+        Number: factorial,
         str: remove_whitespace
-    }, 1, ('round', 'remove_whitespace')),
+    }, 1, ('factorial', 'remove_whitespace')),
 
     # x is defined in the run function
 
     # y is defined in the run function
 
     'z': Overload(1, {
         Number: num_uninterleave,
```

### Comparing `thunno2-2.1.0/thunno2/constants.py` & `thunno2-2.1.1/thunno2/constants.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.0/thunno2/dictionary.py` & `thunno2-2.1.1/thunno2/dictionary.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.0/thunno2/flags.py` & `thunno2-2.1.1/thunno2/flags.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.0/thunno2/helpers.py` & `thunno2-2.1.1/thunno2/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -2554,7 +2554,13 @@
 
 def replace_with_nothing(x, y):
     return y.replace(x, '')
 
 
 def replace_with_nothing2(x, y):
     return x.replace(y, '')
+
+
+def factorial(n):
+    if n < 1:
+        return 1
+    return math.factorial(int(n))
```

### Comparing `thunno2-2.1.0/thunno2/interpreter.py` & `thunno2-2.1.1/thunno2/interpreter.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.0/thunno2/lexer.py` & `thunno2-2.1.1/thunno2/lexer.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.0/thunno2/run.py` & `thunno2-2.1.1/thunno2/run.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.0/thunno2/tests.py` & `thunno2-2.1.1/thunno2/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,17 +369,17 @@
 
 assert_eq(call('U', [1, 2, 3, 2, 1]), [1, 2, 3])
 assert_eq(call('U', [123, 'abc', 123, 'abc']), [123, 'abc'])
 assert_eq(call('U', []), [])
 
 # V
 
-assert_eq(call('V', 102), [0, 2])
-assert_eq(call('V', -1.23), [1, 3, 4])
-assert_eq(call('V', 0.0), [])
+assert_eq(call('V', 123.456), 123)
+assert_eq(call('V', -1.23), -1)
+assert_eq(call('V', 456.789), 457)
 
 assert_eq(call('V', 'Abc, Def?'), 'Nop, Qrs?')
 assert_eq(call('V', '...'), '...')
 
 assert_eq(call('V', ['abc', 1.0, '', 'def', 0]), [0, 1, 3])
 
 # W
@@ -582,21 +582,21 @@
 assert_eq(call('v', '', 'a', 'abcbabcba'), 'bcbbcb')
 
 assert_eq(call('v', 0, 1, [1, 2, 1, 2, 1]), [0, 2, 0, 2, 0])
 assert_eq(call('v', 123, 'abc', [1, 2, 1, 2, 1]), [1, 2, 1, 2, 1])
 
 # w
 
-assert_eq(call('w', 1.234), 1)
-assert_eq(call('w', [-2.345, -1, 0.123, 1.234, 2]), [-2, -1, 0, 1, 2])
+assert_eq(call('w', 5), 120)
+assert_eq(call('w', [-1, 0, 1, 2, 3]), [1, 1, 1, 2, 6])
 
 assert_eq(call('w', 'a\t b\r\n c'), 'abc')
 assert_eq(call('w', ['a b \n c', 'd\t e\nf']), ['abc', 'def'])
 
-assert_eq(call('w', [-123.456, 'a b \n c \t d']), [-123, 'abcd'])
+assert_eq(call('w', [10, 'a b \n c \t d']), [3628800, 'abcd'])
 
 # z
 
 assert_eq(call('z', 12345), [[1, 3, 5], [2, 4]])
 assert_eq(call('z', -6.789), [[6, 8], [7, 9]])
 
 assert_eq(call('z', 'abcdef'), ['ace', 'bdf'])
```

### Comparing `thunno2-2.1.0/thunno2/tokens.py` & `thunno2-2.1.1/thunno2/tokens.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.0/thunno2.egg-info/PKG-INFO` & `thunno2-2.1.1/thunno2.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.1.0
+Version: 2.1.1
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.0.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.1.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

