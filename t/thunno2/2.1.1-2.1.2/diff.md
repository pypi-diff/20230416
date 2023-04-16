# Comparing `tmp/thunno2-2.1.1.tar.gz` & `tmp/thunno2-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunno2-2.1.1.tar", last modified: Sun Apr 16 13:01:09 2023, max compression
+gzip compressed data, was "thunno2-2.1.2.tar", last modified: Sun Apr 16 13:16:53 2023, max compression
```

## Comparing `thunno2-2.1.1.tar` & `thunno2-2.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-16 13:01:09.413257 thunno2-2.1.1/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-16 13:01:09.413145 thunno2-2.1.1/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)       38 2023-04-16 13:01:09.413291 thunno2-2.1.1/setup.cfg
--rw-r--r--   0 nayak      (501) staff       (20)     1354 2023-04-12 09:58:27.000000 thunno2-2.1.1/setup.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-16 13:01:09.412470 thunno2-2.1.1/thunno2/
--rw-r--r--   0 nayak      (501) staff       (20)       22 2023-04-03 16:07:07.000000 thunno2-2.1.1/thunno2/__init__.py
--rw-r--r--   0 nayak      (501) staff       (20)     1412 2023-04-03 16:27:37.000000 thunno2-2.1.1/thunno2/codepage.py
--rw-r--r--   0 nayak      (501) staff       (20)    46724 2023-04-16 13:00:29.000000 thunno2-2.1.1/thunno2/commands.py
--rw-r--r--   0 nayak      (501) staff       (20)     2971 2023-04-15 15:28:56.000000 thunno2-2.1.1/thunno2/constants.py
--rw-r--r--   0 nayak      (501) staff       (20)   245513 2023-04-14 08:28:09.000000 thunno2-2.1.1/thunno2/dictionary.py
--rw-r--r--   0 nayak      (501) staff       (20)     6066 2023-04-14 19:12:18.000000 thunno2-2.1.1/thunno2/flags.py
--rw-r--r--   0 nayak      (501) staff       (20)    48173 2023-04-16 11:06:19.000000 thunno2-2.1.1/thunno2/helpers.py
--rw-r--r--   0 nayak      (501) staff       (20)    25876 2023-04-15 15:28:56.000000 thunno2-2.1.1/thunno2/interpreter.py
--rw-r--r--   0 nayak      (501) staff       (20)    22512 2023-04-15 17:55:44.000000 thunno2-2.1.1/thunno2/lexer.py
--rw-r--r--   0 nayak      (501) staff       (20)     1675 2023-04-15 17:55:44.000000 thunno2-2.1.1/thunno2/run.py
--rw-r--r--   0 nayak      (501) staff       (20)    62659 2023-04-16 13:00:29.000000 thunno2-2.1.1/thunno2/tests.py
--rw-r--r--   0 nayak      (501) staff       (20)     3274 2023-04-15 17:55:44.000000 thunno2-2.1.1/thunno2/tokens.py
--rw-r--r--   0 nayak      (501) staff       (20)       97 2023-04-16 13:00:43.000000 thunno2-2.1.1/thunno2/version.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-16 13:01:09.412998 thunno2-2.1.1/thunno2.egg-info/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-16 13:01:09.000000 thunno2-2.1.1/thunno2.egg-info/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)      414 2023-04-16 13:01:09.000000 thunno2-2.1.1/thunno2.egg-info/SOURCES.txt
--rw-r--r--   0 nayak      (501) staff       (20)        1 2023-04-16 13:01:09.000000 thunno2-2.1.1/thunno2.egg-info/dependency_links.txt
--rw-r--r--   0 nayak      (501) staff       (20)       54 2023-04-16 13:01:09.000000 thunno2-2.1.1/thunno2.egg-info/entry_points.txt
--rw-r--r--   0 nayak      (501) staff       (20)        8 2023-04-16 13:01:09.000000 thunno2-2.1.1/thunno2.egg-info/top_level.txt
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-16 13:16:53.900194 thunno2-2.1.2/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-16 13:16:53.900065 thunno2-2.1.2/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)       38 2023-04-16 13:16:53.900233 thunno2-2.1.2/setup.cfg
+-rw-r--r--   0 nayak      (501) staff       (20)     1354 2023-04-12 09:58:27.000000 thunno2-2.1.2/setup.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-16 13:16:53.899308 thunno2-2.1.2/thunno2/
+-rw-r--r--   0 nayak      (501) staff       (20)       22 2023-04-03 16:07:07.000000 thunno2-2.1.2/thunno2/__init__.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1412 2023-04-03 16:27:37.000000 thunno2-2.1.2/thunno2/codepage.py
+-rw-r--r--   0 nayak      (501) staff       (20)    46724 2023-04-16 13:00:29.000000 thunno2-2.1.2/thunno2/commands.py
+-rw-r--r--   0 nayak      (501) staff       (20)     2971 2023-04-15 15:28:56.000000 thunno2-2.1.2/thunno2/constants.py
+-rw-r--r--   0 nayak      (501) staff       (20)   245338 2023-04-16 13:14:34.000000 thunno2-2.1.2/thunno2/dictionary.py
+-rw-r--r--   0 nayak      (501) staff       (20)     6066 2023-04-14 19:12:18.000000 thunno2-2.1.2/thunno2/flags.py
+-rw-r--r--   0 nayak      (501) staff       (20)    48354 2023-04-16 13:14:16.000000 thunno2-2.1.2/thunno2/helpers.py
+-rw-r--r--   0 nayak      (501) staff       (20)    25876 2023-04-15 15:28:56.000000 thunno2-2.1.2/thunno2/interpreter.py
+-rw-r--r--   0 nayak      (501) staff       (20)    22512 2023-04-15 17:55:44.000000 thunno2-2.1.2/thunno2/lexer.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1675 2023-04-15 17:55:44.000000 thunno2-2.1.2/thunno2/run.py
+-rw-r--r--   0 nayak      (501) staff       (20)    62753 2023-04-16 13:14:34.000000 thunno2-2.1.2/thunno2/tests.py
+-rw-r--r--   0 nayak      (501) staff       (20)     3274 2023-04-15 17:55:44.000000 thunno2-2.1.2/thunno2/tokens.py
+-rw-r--r--   0 nayak      (501) staff       (20)       97 2023-04-16 13:16:42.000000 thunno2-2.1.2/thunno2/version.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-16 13:16:53.899897 thunno2-2.1.2/thunno2.egg-info/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-16 13:16:53.000000 thunno2-2.1.2/thunno2.egg-info/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)      414 2023-04-16 13:16:53.000000 thunno2-2.1.2/thunno2.egg-info/SOURCES.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        1 2023-04-16 13:16:53.000000 thunno2-2.1.2/thunno2.egg-info/dependency_links.txt
+-rw-r--r--   0 nayak      (501) staff       (20)       54 2023-04-16 13:16:53.000000 thunno2-2.1.2/thunno2.egg-info/entry_points.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        8 2023-04-16 13:16:53.000000 thunno2-2.1.2/thunno2.egg-info/top_level.txt
```

### Comparing `thunno2-2.1.1/PKG-INFO` & `thunno2-2.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.1.1
+Version: 2.1.2
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.1.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.2.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `thunno2-2.1.1/setup.py` & `thunno2-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.1/thunno2/codepage.py` & `thunno2-2.1.2/thunno2/codepage.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.1/thunno2/commands.py` & `thunno2-2.1.2/thunno2/commands.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.1/thunno2/constants.py` & `thunno2-2.1.2/thunno2/constants.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.1/thunno2/dictionary.py` & `thunno2-2.1.2/thunno2/dictionary.py`

 * *Files 0% similar despite different names*

```diff
@@ -15292,54 +15292,43 @@
 0003bbb0: 0a20 2020 2020 2020 2020 2020 2072 202b  .            r +
 0003bbc0: 3d20 275c 5c27 202b 2063 0a20 2020 2020  = '\\' + c.     
 0003bbd0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
 0003bbe0: 2020 2020 2072 202b 3d20 630a 2020 2020       r += c.    
 0003bbf0: 7265 7475 726e 2072 0a0a 0a64 6566 206f  return r...def o
 0003bc00: 7074 696d 616c 5f64 6963 7469 6f6e 6172  ptimal_dictionar
 0003bc10: 795f 636f 6d70 7265 7373 696f 6e28 7329  y_compression(s)
-0003bc20: 3a0a 2020 2020 776f 7264 7320 3d20 7265  :.    words = re
-0003bc30: 2e66 696e 6461 6c6c 2827 285b 612d 7a5d  .findall('([a-z]
-0003bc40: 2b29 285b 5e61 2d7a 5d2b 2927 2c20 7374  +)([^a-z]+)', st
-0003bc50: 7228 7329 2e6c 6f77 6572 2829 290a 2020  r(s).lower()).  
-0003bc60: 2020 7265 7420 3d20 2727 0a20 2020 2066    ret = ''.    f
-0003bc70: 6f72 2077 6f72 642c 206f 7468 6572 5f73  or word, other_s
-0003bc80: 7475 6666 2069 6e20 776f 7264 733a 0a20  tuff in words:. 
-0003bc90: 2020 2020 2020 2069 6620 6e6f 7420 2877         if not (w
-0003bca0: 6f72 6420 2b20 6f74 6865 725f 7374 7566  ord + other_stuf
-0003bcb0: 6629 3a0a 2020 2020 2020 2020 2020 2020  f):.            
-0003bcc0: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
-0003bcd0: 2063 6f6d 7072 6573 7369 6f6e 7320 3d20   compressions = 
-0003bce0: 5b5d 0a20 2020 2020 2020 2066 6f72 206c  [].        for l
-0003bcf0: 2069 6e20 6865 6c70 6572 732e 696e 7465   in helpers.inte
-0003bd00: 6765 725f 7061 7274 6974 696f 6e73 286c  ger_partitions(l
-0003bd10: 656e 2877 6f72 6429 295b 3a3a 2d31 5d3a  en(word))[::-1]:
-0003bd20: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
-0003bd30: 5f77 6f72 6420 3d20 776f 7264 0a20 2020  _word = word.   
-0003bd40: 2020 2020 2020 2020 2078 203d 205b 5d0a           x = [].
-0003bd50: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0003bd60: 6920 696e 206c 3a0a 2020 2020 2020 2020  i in l:.        
-0003bd70: 2020 2020 2020 2020 782e 6170 7065 6e64          x.append
-0003bd80: 286e 6577 5f77 6f72 645b 3a69 5d29 0a20  (new_word[:i]). 
-0003bd90: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0003bda0: 6577 5f77 6f72 6420 3d20 6e65 775f 776f  ew_word = new_wo
-0003bdb0: 7264 5b69 3a5d 0a20 2020 2020 2020 2020  rd[i:].         
-0003bdc0: 2020 2063 6f6d 7072 6573 7369 6f6e 732e     compressions.
-0003bdd0: 6170 7065 6e64 280a 2020 2020 2020 2020  append(.        
-0003bde0: 2020 2020 2020 2020 2727 2e6a 6f69 6e28          ''.join(
-0003bdf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0003be00: 2020 2020 2064 6963 7469 6f6e 6172 795f       dictionary_
-0003be10: 636f 6d70 7265 7373 5f77 6f72 6428 7729  compress_word(w)
-0003be20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0003be30: 2020 2020 2069 6620 6469 6374 696f 6e61       if dictiona
-0003be40: 7279 5f63 6f6d 7072 6573 735f 776f 7264  ry_compress_word
-0003be50: 2877 2920 213d 202d 310a 2020 2020 2020  (w) != -1.      
-0003be60: 2020 2020 2020 2020 2020 2020 2020 656c                el
-0003be70: 7365 2077 0a20 2020 2020 2020 2020 2020  se w.           
-0003be80: 2020 2020 2020 2020 2066 6f72 2077 2069           for w i
-0003be90: 6e20 780a 2020 2020 2020 2020 2020 2020  n x.            
-0003bea0: 2020 2020 2920 2b20 6261 636b 736c 6173      ) + backslas
-0003beb0: 6869 6679 286f 7468 6572 5f73 7475 6666  hify(other_stuff
-0003bec0: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
-0003bed0: 2020 2020 2020 2020 7265 7420 2b3d 206d          ret += m
-0003bee0: 696e 2863 6f6d 7072 6573 7369 6f6e 732c  in(compressions,
-0003bef0: 206b 6579 3d6c 656e 290a 2020 2020 7265   key=len).    re
-0003bf00: 7475 726e 2072 6574 0a                   turn ret.
+0003bc20: 3a0a 2020 2020 7773 203d 2072 652e 6669  :.    ws = re.fi
+0003bc30: 6e64 616c 6c28 2728 5b61 2d7a 5d2a 2928  ndall('([a-z]*)(
+0003bc40: 5b5e 612d 7a5d 2a29 272c 2073 7472 2873  [^a-z]*)', str(s
+0003bc50: 292e 6c6f 7765 7228 2929 0a20 2020 2072  ).lower()).    r
+0003bc60: 6574 203d 2027 270a 2020 2020 666f 7220  et = ''.    for 
+0003bc70: 776f 7264 2c20 6f74 6865 725f 7374 7566  word, other_stuf
+0003bc80: 6620 696e 2077 733a 0a20 2020 2020 2020  f in ws:.       
+0003bc90: 2069 6620 6e6f 7420 2877 6f72 6420 2b20   if not (word + 
+0003bca0: 6f74 6865 725f 7374 7566 6629 3a0a 2020  other_stuff):.  
+0003bcb0: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+0003bcc0: 7565 0a20 2020 2020 2020 2063 6f6d 7072  ue.        compr
+0003bcd0: 6573 7369 6f6e 7320 3d20 5b5d 0a20 2020  essions = [].   
+0003bce0: 2020 2020 2066 6f72 2078 2069 6e20 6865       for x in he
+0003bcf0: 6c70 6572 732e 616c 6c5f 736c 6963 6573  lpers.all_slices
+0003bd00: 2877 6f72 6429 3a0a 2020 2020 2020 2020  (word):.        
+0003bd10: 2020 2020 636f 6d70 7265 7373 696f 6e73      compressions
+0003bd20: 2e61 7070 656e 6428 0a20 2020 2020 2020  .append(.       
+0003bd30: 2020 2020 2020 2020 2027 272e 6a6f 696e           ''.join
+0003bd40: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0003bd50: 2020 2020 2020 6469 6374 696f 6e61 7279        dictionary
+0003bd60: 5f63 6f6d 7072 6573 735f 776f 7264 2877  _compress_word(w
+0003bd70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0003bd80: 2020 2020 2020 6966 2064 6963 7469 6f6e        if diction
+0003bd90: 6172 795f 636f 6d70 7265 7373 5f77 6f72  ary_compress_wor
+0003bda0: 6428 7729 2021 3d20 2d31 0a20 2020 2020  d(w) != -1.     
+0003bdb0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0003bdc0: 6c73 6520 770a 2020 2020 2020 2020 2020  lse w.          
+0003bdd0: 2020 2020 2020 2020 2020 666f 7220 7720            for w 
+0003bde0: 696e 2078 0a20 2020 2020 2020 2020 2020  in x.           
+0003bdf0: 2020 2020 2029 202b 2062 6163 6b73 6c61       ) + backsla
+0003be00: 7368 6966 7928 6f74 6865 725f 7374 7566  shify(other_stuf
+0003be10: 6629 0a20 2020 2020 2020 2020 2020 2029  f).            )
+0003be20: 0a20 2020 2020 2020 2072 6574 202b 3d20  .        ret += 
+0003be30: 6d69 6e28 636f 6d70 7265 7373 696f 6e73  min(compressions
+0003be40: 2c20 6b65 793d 6c65 6e29 0a20 2020 2072  , key=len).    r
+0003be50: 6574 7572 6e20 7265 740a                 eturn ret.
```

### Comparing `thunno2-2.1.1/thunno2/flags.py` & `thunno2-2.1.2/thunno2/flags.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.1/thunno2/helpers.py` & `thunno2-2.1.2/thunno2/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -2560,7 +2560,17 @@
     return x.replace(y, '')
 
 
 def factorial(n):
     if n < 1:
         return 1
     return math.factorial(int(n))
+
+
+def all_slices(s):
+    if not s:
+        return [[]]
+    r = []
+    for i in one_range(len(s)):
+        for x in all_slices(s[i:]):
+            r.append([s[:i]] + x)
+    return r
```

### Comparing `thunno2-2.1.1/thunno2/interpreter.py` & `thunno2-2.1.2/thunno2/interpreter.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.1/thunno2/lexer.py` & `thunno2-2.1.2/thunno2/lexer.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.1/thunno2/run.py` & `thunno2-2.1.2/thunno2/run.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.1/thunno2/tests.py` & `thunno2-2.1.2/thunno2/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1907,14 +1907,16 @@
 
 assert_eq(call('ẓ', 2, [123, 456, 789]), [123])
 assert_eq(call('ẓ', ['abc', 'def', 'ghi', 'jkl', 'mno'], 3), ['abc', 'def'])
 
 # øD
 
 assert_eq(call('øD', 'Hello, World!'), 'Ƙ¥, «ʋ!')
+assert_eq(call('øD', 'thunnobest'), 'thunnoÇ&')
+assert_eq(call('øD', 'withree'), 'wiċŀ')
 
 # After all the tests
 
 untested_commands = sorted({*commands} - {*tested_commands} - {*UNTESTABLE}, key=[*commands].index)
 if untested_commands:
     print(f'\u001b[33mUntested commands: {", ".join(untested_commands)}')
```

### Comparing `thunno2-2.1.1/thunno2/tokens.py` & `thunno2-2.1.2/thunno2/tokens.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.1/thunno2.egg-info/PKG-INFO` & `thunno2-2.1.2/thunno2.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.1.1
+Version: 2.1.2
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.1.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.2.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

