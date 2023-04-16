# Comparing `tmp/igbpyutils-0.0.2.tar.gz` & `tmp/igbpyutils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igbpyutils-0.0.2.tar", last modified: Sat Apr 15 09:03:03 2023, max compression
+gzip compressed data, was "igbpyutils-0.0.3.tar", last modified: Sun Apr 16 11:34:01 2023, max compression
```

## Comparing `igbpyutils-0.0.2.tar` & `igbpyutils-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwx------   0 haukex    (1000) haukex    (1000)        0 2023-04-15 09:03:03.567283 igbpyutils-0.0.2/
--rw-------   0 haukex    (1000) haukex    (1000)    35149 2023-04-14 17:49:50.000000 igbpyutils-0.0.2/LICENSE.txt
--rw-------   0 haukex    (1000) haukex    (1000)     2222 2023-04-15 09:03:03.567283 igbpyutils-0.0.2/PKG-INFO
--rw-------   0 haukex    (1000) haukex    (1000)     1496 2023-04-15 09:00:42.000000 igbpyutils-0.0.2/README.md
-drwx------   0 haukex    (1000) haukex    (1000)        0 2023-04-15 09:03:03.567283 igbpyutils-0.0.2/igbpyutils/
--rw-------   0 haukex    (1000) haukex    (1000)        0 2023-04-14 19:16:14.000000 igbpyutils-0.0.2/igbpyutils/__init__.py
--rw-------   0 haukex    (1000) haukex    (1000)     5263 2023-04-15 08:15:49.000000 igbpyutils-0.0.2/igbpyutils/error.py
--rw-------   0 haukex    (1000) haukex    (1000)     9115 2023-04-14 17:49:50.000000 igbpyutils-0.0.2/igbpyutils/file.py
--rw-------   0 haukex    (1000) haukex    (1000)     5456 2023-04-14 17:49:50.000000 igbpyutils-0.0.2/igbpyutils/iter.py
--rw-------   0 haukex    (1000) haukex    (1000)     1429 2023-04-14 19:21:32.000000 igbpyutils-0.0.2/igbpyutils/test.py
-drwx------   0 haukex    (1000) haukex    (1000)        0 2023-04-15 09:03:03.567283 igbpyutils-0.0.2/igbpyutils.egg-info/
--rw-------   0 haukex    (1000) haukex    (1000)     2222 2023-04-15 09:03:03.000000 igbpyutils-0.0.2/igbpyutils.egg-info/PKG-INFO
--rw-------   0 haukex    (1000) haukex    (1000)      349 2023-04-15 09:03:03.000000 igbpyutils-0.0.2/igbpyutils.egg-info/SOURCES.txt
--rw-------   0 haukex    (1000) haukex    (1000)        1 2023-04-15 09:03:03.000000 igbpyutils-0.0.2/igbpyutils.egg-info/dependency_links.txt
--rw-------   0 haukex    (1000) haukex    (1000)       11 2023-04-15 09:03:03.000000 igbpyutils-0.0.2/igbpyutils.egg-info/top_level.txt
--rw-------   0 haukex    (1000) haukex    (1000)      767 2023-04-15 08:41:35.000000 igbpyutils-0.0.2/pyproject.toml
--rw-------   0 haukex    (1000) haukex    (1000)       38 2023-04-15 09:03:03.567283 igbpyutils-0.0.2/setup.cfg
-drwx------   0 haukex    (1000) haukex    (1000)        0 2023-04-15 09:03:03.567283 igbpyutils-0.0.2/tests/
--rwx------   0 haukex    (1000) haukex    (1000)     6413 2023-04-15 08:58:04.000000 igbpyutils-0.0.2/tests/test_error.py
--rwx------   0 haukex    (1000) haukex    (1000)    11316 2023-04-15 08:18:39.000000 igbpyutils-0.0.2/tests/test_file.py
--rwx------   0 haukex    (1000) haukex    (1000)     9021 2023-04-14 19:25:57.000000 igbpyutils-0.0.2/tests/test_iter.py
--rwx------   0 haukex    (1000) haukex    (1000)     1606 2023-04-14 19:26:01.000000 igbpyutils-0.0.2/tests/test_test.py
+drwx------   0 haukex    (1000) haukex    (1000)        0 2023-04-16 11:34:01.813254 igbpyutils-0.0.3/
+-rw-------   0 haukex    (1000) haukex    (1000)    35149 2023-04-14 17:49:50.000000 igbpyutils-0.0.3/LICENSE.txt
+-rw-------   0 haukex    (1000) haukex    (1000)     2374 2023-04-16 11:34:01.813254 igbpyutils-0.0.3/PKG-INFO
+-rw-------   0 haukex    (1000) haukex    (1000)     1496 2023-04-15 09:00:42.000000 igbpyutils-0.0.3/README.md
+drwx------   0 haukex    (1000) haukex    (1000)        0 2023-04-16 11:34:01.809254 igbpyutils-0.0.3/igbpyutils/
+-rw-------   0 haukex    (1000) haukex    (1000)        0 2023-04-14 19:16:14.000000 igbpyutils-0.0.3/igbpyutils/__init__.py
+-rw-------   0 haukex    (1000) haukex    (1000)     1528 2023-04-16 11:28:55.000000 igbpyutils-0.0.3/igbpyutils/dt.py
+-rw-------   0 haukex    (1000) haukex    (1000)     5263 2023-04-15 08:15:49.000000 igbpyutils-0.0.3/igbpyutils/error.py
+-rw-------   0 haukex    (1000) haukex    (1000)     9181 2023-04-15 10:48:14.000000 igbpyutils-0.0.3/igbpyutils/file.py
+-rw-------   0 haukex    (1000) haukex    (1000)     5432 2023-04-15 10:48:14.000000 igbpyutils-0.0.3/igbpyutils/iter.py
+-rw-------   0 haukex    (1000) haukex    (1000)     1429 2023-04-14 19:21:32.000000 igbpyutils-0.0.3/igbpyutils/test.py
+drwx------   0 haukex    (1000) haukex    (1000)        0 2023-04-16 11:34:01.813254 igbpyutils-0.0.3/igbpyutils.egg-info/
+-rw-------   0 haukex    (1000) haukex    (1000)     2374 2023-04-16 11:34:01.000000 igbpyutils-0.0.3/igbpyutils.egg-info/PKG-INFO
+-rw-------   0 haukex    (1000) haukex    (1000)      383 2023-04-16 11:34:01.000000 igbpyutils-0.0.3/igbpyutils.egg-info/SOURCES.txt
+-rw-------   0 haukex    (1000) haukex    (1000)        1 2023-04-16 11:34:01.000000 igbpyutils-0.0.3/igbpyutils.egg-info/dependency_links.txt
+-rw-------   0 haukex    (1000) haukex    (1000)       11 2023-04-16 11:34:01.000000 igbpyutils-0.0.3/igbpyutils.egg-info/top_level.txt
+-rw-------   0 haukex    (1000) haukex    (1000)      904 2023-04-16 11:23:07.000000 igbpyutils-0.0.3/pyproject.toml
+-rw-------   0 haukex    (1000) haukex    (1000)       38 2023-04-16 11:34:01.813254 igbpyutils-0.0.3/setup.cfg
+drwx------   0 haukex    (1000) haukex    (1000)        0 2023-04-16 11:34:01.813254 igbpyutils-0.0.3/tests/
+-rwxr-xr-x   0 haukex    (1000) haukex    (1000)     2023 2023-04-16 11:23:30.000000 igbpyutils-0.0.3/tests/test_dt.py
+-rwx------   0 haukex    (1000) haukex    (1000)     6413 2023-04-15 08:58:04.000000 igbpyutils-0.0.3/tests/test_error.py
+-rwx------   0 haukex    (1000) haukex    (1000)    11396 2023-04-15 10:48:14.000000 igbpyutils-0.0.3/tests/test_file.py
+-rwx------   0 haukex    (1000) haukex    (1000)     9018 2023-04-16 11:21:31.000000 igbpyutils-0.0.3/tests/test_iter.py
+-rwx------   0 haukex    (1000) haukex    (1000)     1606 2023-04-14 19:26:01.000000 igbpyutils-0.0.3/tests/test_test.py
```

### Comparing `igbpyutils-0.0.2/LICENSE.txt` & `igbpyutils-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `igbpyutils-0.0.2/PKG-INFO` & `igbpyutils-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: igbpyutils
-Version: 0.0.2
+Version: 0.0.3
 Summary: Various Python Utilities
 Author-email: Hauke D <haukex@zero-g.net>
 Project-URL: Homepage, https://github.com/haukex/igbpyutils
 Project-URL: Bug Tracker, https://github.com/haukex/igbpyutils/issues
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.9
```

### Comparing `igbpyutils-0.0.2/README.md` & `igbpyutils-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `igbpyutils-0.0.2/igbpyutils/error.py` & `igbpyutils-0.0.3/igbpyutils/error.py`

 * *Files identical despite different names*

### Comparing `igbpyutils-0.0.2/igbpyutils/file.py` & `igbpyutils-0.0.3/igbpyutils/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,29 +69,29 @@
             # If a *NIX glob doesn't match anything, it isn't expanded,
             # while glob() returns an empty list, so we emulate *NIX.
             if g: yield from g
             else: yield f
     else:
         yield from files
 
-class Pushd:  # cover-not-3.11
+class Pushd:  # cover-not-ge3.11
     """A context manager that temporarily changes the current working directory."""
     def __init__(self, newdir :Filename):
         self.newdir = newdir
     def __enter__(self):
         self.prevdir = os.getcwd()
         os.chdir(self.newdir)
         return
     def __exit__(self, exc_type, exc_val, exc_tb):
         os.chdir(self.prevdir)
         return False  # raise exception if any
-if sys.hexversion>=0x030B00F0:  # cover-not-3.9 cover-not-3.10
+if sys.hexversion>=0x030B00F0:  # cover-not-le3.10
     import contextlib
     Pushd = contextlib.chdir
-else: pass  # cover-not-3.11
+else: pass  # cover-not-ge3.11
 
 def filetypestr(st :os.stat_result) -> str:
     """Return a string naming the file type reported by ``stat``."""
     if stat.S_ISDIR(st.st_mode): return "directory"
     elif stat.S_ISCHR(st.st_mode): return "character special device file"  # pragma: no cover
     elif stat.S_ISBLK(st.st_mode): return "block special device file"  # pragma: no cover
     elif stat.S_ISREG(st.st_mode): return "regular file"
@@ -185,16 +185,17 @@
         os.replace(tf, dst)
     except BaseException:
         os.unlink(tf)
         raise
 
 # noinspection PyPep8Naming
 @contextmanager
-def NamedTempFileDeleteLater(*args, **kwargs) -> Generator:
+def NamedTempFileDeleteLater(*args, **kwargs) -> Generator:  # cover-not-ge3.12
     """A ``NamedTemporaryFile`` that is unlinked on context manager exit, not on close."""
-    if sys.hexversion>=0x030C00F0:
-        # noinspection PyArgumentList
-        yield NamedTemporaryFile(*args, **kwargs, delete=True, delete_on_close=False)  # cover-not-3.9 cover-not-3.10 cover-not-3.11
-    else:
-        tf = NamedTemporaryFile(*args, **kwargs, delete=False)
-        try: yield tf
-        finally: os.unlink(tf.name)
+    tf = NamedTemporaryFile(*args, **kwargs, delete=False)
+    try: yield tf
+    finally: os.unlink(tf.name)
+#TODO Later: Once 3.12 is released, change the following to 0x030C00F0
+if sys.hexversion>=0x030C0000:  # cover-not-le3.11
+    from functools import partial
+    NamedTempFileDeleteLater = partial(NamedTemporaryFile, delete=True, delete_on_close=False)
+else: pass  # cover-not-ge3.12
```

### Comparing `igbpyutils-0.0.2/igbpyutils/iter.py` & `igbpyutils-0.0.3/igbpyutils/iter.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,24 +41,24 @@
 @overload
 def zip_strict(
     __iter1: Iterable[_T0],
     __iter2: Iterable[_T0],
     __iter3: Iterable[_T0],
     *iterables: Iterable[_T0],
 ) -> Iterator[tuple[_T0, ...]]: ...  # pragma: no cover
-def zip_strict(*iterables):  # cover-not-3.10 cover-not-3.11
+def zip_strict(*iterables):  # cover-not-ge3.10
     """Like Python's ``zip``, but requires all iterables to return the same number of items."""
     for combo in zip_longest(*iterables, fillvalue=_marker):
         if any( v is _marker for v in combo ):
             raise ValueError("Iterables have different lengths")
         yield combo
-if sys.hexversion>=0x030A00F0:  # cover-not-3.9
+if sys.hexversion>=0x030A00F0:  # cover-not-le3.9
     from functools import partial
     zip_strict = partial(zip, strict=True)
-else: pass  # cover-not-3.10 cover-not-3.11
+else: pass  # cover-not-ge3.10
 
 _T = TypeVar('_T', covariant=True)
 class SizedCallbackIterator(Generic[_T], Sized, Iterator[_T]):
     """Wrapper to add ``len`` support to an iterator.
 
     For example, this can be used to wrap a generator which has a known output length
     (e.g. if it returns exactly one item per input item), so that it can then
```

### Comparing `igbpyutils-0.0.2/igbpyutils/test.py` & `igbpyutils-0.0.3/igbpyutils/test.py`

 * *Files identical despite different names*

### Comparing `igbpyutils-0.0.2/igbpyutils.egg-info/PKG-INFO` & `igbpyutils-0.0.3/igbpyutils.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: igbpyutils
-Version: 0.0.2
+Version: 0.0.3
 Summary: Various Python Utilities
 Author-email: Hauke D <haukex@zero-g.net>
 Project-URL: Homepage, https://github.com/haukex/igbpyutils
 Project-URL: Bug Tracker, https://github.com/haukex/igbpyutils/issues
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.9
```

### Comparing `igbpyutils-0.0.2/pyproject.toml` & `igbpyutils-0.0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "igbpyutils"
 description = "Various Python Utilities"
-version = "0.0.2"
+version = "0.0.3"
 authors = [ { name="Hauke D", email="haukex@zero-g.net" } ]
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: POSIX",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: MacOS :: MacOS X",
     "Development Status :: 5 - Production/Stable",
     "Topic :: Software Development :: Libraries",
 ]
```

### Comparing `igbpyutils-0.0.2/tests/test_error.py` & `igbpyutils-0.0.3/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `igbpyutils-0.0.2/tests/test_file.py` & `igbpyutils-0.0.3/tests/test_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,17 +54,17 @@
         self.assertTrue(len(files)>3)
         # this doesn't really test expanduser but that's ok
         self.assertEqual( files+[noglob], sorted(autoglob([testglob, noglob], force=True)) )
         self.assertEqual( files if sys.platform.startswith('win32') else [testglob], list(autoglob([testglob])) )
 
     def test_pushd(self):
         def realpath(pth):
-            if sys.hexversion>=0x030A00F0:  # cover-not-3.9
+            if sys.hexversion>=0x030A00F0:  # cover-not-le3.9
                 return os.path.realpath(pth, strict=True)
-            else:  # cover-not-3.10 cover-not-3.11
+            else:  # cover-not-ge3.10
                 return os.path.realpath(pth)
         prevwd = realpath(os.getcwd())
         with (TemporaryDirectory() as td1, TemporaryDirectory() as td2):
             # basic pushd
             with Pushd(td1):
                 self.assertEqual(realpath(os.getcwd()), realpath(td1))
                 with Pushd(td2):
@@ -236,17 +236,19 @@
             tf1.close()
             self.assertFalse( Path(tf1.name).exists() )
         with NamedTempFileDeleteLater() as tf2:
             tf2.write(b'Bar')
             tf2.close()
             self.assertTrue( Path(tf2.name).exists() )
         self.assertFalse( Path(tf2.name).exists() )
-        if sys.hexversion>=0x030C00F0:  # cover-not-3.9 cover-not-3.10 cover-not-3.11
+        #TODO Later: Once 3.12 is released, change the following to 0x030C00F0
+        if sys.hexversion>=0x030C0000:  # cover-not-le3.11
             # noinspection PyArgumentList
             with NamedTemporaryFile(delete=True, delete_on_close=False) as tf3:
                 tf3.write(b'Quz')
                 tf3.close()
                 self.assertTrue( Path(tf3.name).exists() )
             self.assertFalse( Path(tf3.name).exists() )
+        else: pass  # cover-not-ge3.12
 
 if __name__ == '__main__':  # pragma: no cover
     unittest.main()
```

### Comparing `igbpyutils-0.0.2/tests/test_iter.py` & `igbpyutils-0.0.3/tests/test_iter.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 along with this program. If not, see https://www.gnu.org/licenses/
 """
 import unittest
 from itertools import product
 from more_itertools import gray_product
 from igbpyutils.iter import no_duplicates, SizedCallbackIterator, is_unique_everseen, zip_strict
 
-class TestIgbItertools(unittest.TestCase):
+class TestIterTools(unittest.TestCase):
 
     def test_zip_strict(self):
         l2 = [0, 1]
         l3 = [2, 3, 4]
         l3b = [5, 6, 7]
         l4 = [8, 9, 10, 11]
         self.assertEqual( list(zip_strict(l3, l3b)), list(zip(l3, l3b)) )
```

### Comparing `igbpyutils-0.0.2/tests/test_test.py` & `igbpyutils-0.0.3/tests/test_test.py`

 * *Files identical despite different names*

