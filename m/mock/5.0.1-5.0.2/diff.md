# Comparing `tmp/mock-5.0.1.tar.gz` & `tmp/mock-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mock-5.0.1.tar", last modified: Mon Jan  9 17:49:20 2023, max compression
+gzip compressed data, was "mock-5.0.2.tar", last modified: Sun Apr 16 11:26:52 2023, max compression
```

## Comparing `mock-5.0.1.tar` & `mock-5.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-01-09 17:49:20.416427 mock-5.0.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16634 2023-01-09 17:49:14.000000 mock-5.0.1/CHANGELOG.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1342 2023-01-09 17:49:14.000000 mock-5.0.1/LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-01-09 17:49:14.000000 mock-5.0.1/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2812 2023-01-09 17:49:20.416427 mock-5.0.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1475 2023-01-09 17:49:14.000000 mock-5.0.1/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-01-09 17:49:20.416427 mock-5.0.1/mock/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      334 2023-01-09 17:49:14.000000 mock-5.0.1/mock/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2808 2023-01-09 17:49:14.000000 mock-5.0.1/mock/backports.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   105498 2023-01-09 17:49:14.000000 mock-5.0.1/mock/mock.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-01-09 17:49:20.416427 mock-5.0.1/mock/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-01-09 17:49:14.000000 mock-5.0.1/mock/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      974 2023-01-09 17:49:14.000000 mock-5.0.1/mock/tests/support.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    38696 2023-01-09 17:49:14.000000 mock-5.0.1/mock/tests/testasync.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4263 2023-01-09 17:49:14.000000 mock-5.0.1/mock/tests/testcallable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33857 2023-01-09 17:49:14.000000 mock-5.0.1/mock/tests/testhelpers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16261 2023-01-09 17:49:14.000000 mock-5.0.1/mock/tests/testmagicmethods.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    77314 2023-01-09 17:49:14.000000 mock-5.0.1/mock/tests/testmock.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    58990 2023-01-09 17:49:14.000000 mock-5.0.1/mock/tests/testpatch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7391 2023-01-09 17:49:14.000000 mock-5.0.1/mock/tests/testsealable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1316 2023-01-09 17:49:14.000000 mock-5.0.1/mock/tests/testsentinel.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12208 2023-01-09 17:49:14.000000 mock-5.0.1/mock/tests/testwith.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-01-09 17:49:20.416427 mock-5.0.1/mock.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2812 2023-01-09 17:49:20.000000 mock-5.0.1/mock.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      531 2023-01-09 17:49:20.000000 mock-5.0.1/mock.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-01-09 17:49:20.000000 mock-5.0.1/mock.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-01-09 17:49:20.000000 mock-5.0.1/mock.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2023-01-09 17:49:20.000000 mock-5.0.1/mock.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1410 2023-01-09 17:49:20.420427 mock-5.0.1/setup.cfg
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      246 2023-01-09 17:49:14.000000 mock-5.0.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 11:26:52.041844 mock-5.0.2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16940 2023-04-16 11:26:45.000000 mock-5.0.2/CHANGELOG.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1342 2023-04-16 11:26:45.000000 mock-5.0.2/LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-04-16 11:26:45.000000 mock-5.0.2/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2812 2023-04-16 11:26:52.041844 mock-5.0.2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1475 2023-04-16 11:26:45.000000 mock-5.0.2/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 11:26:52.037844 mock-5.0.2/mock/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      334 2023-04-16 11:26:45.000000 mock-5.0.2/mock/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2808 2023-04-16 11:26:45.000000 mock-5.0.2/mock/backports.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   105795 2023-04-16 11:26:45.000000 mock-5.0.2/mock/mock.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 11:26:52.041844 mock-5.0.2/mock/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-16 11:26:45.000000 mock-5.0.2/mock/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      974 2023-04-16 11:26:45.000000 mock-5.0.2/mock/tests/support.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    38696 2023-04-16 11:26:45.000000 mock-5.0.2/mock/tests/testasync.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4263 2023-04-16 11:26:45.000000 mock-5.0.2/mock/tests/testcallable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    34990 2023-04-16 11:26:45.000000 mock-5.0.2/mock/tests/testhelpers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16261 2023-04-16 11:26:45.000000 mock-5.0.2/mock/tests/testmagicmethods.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    77314 2023-04-16 11:26:45.000000 mock-5.0.2/mock/tests/testmock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    60095 2023-04-16 11:26:45.000000 mock-5.0.2/mock/tests/testpatch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7391 2023-04-16 11:26:45.000000 mock-5.0.2/mock/tests/testsealable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1316 2023-04-16 11:26:45.000000 mock-5.0.2/mock/tests/testsentinel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12208 2023-04-16 11:26:45.000000 mock-5.0.2/mock/tests/testwith.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 11:26:52.037844 mock-5.0.2/mock.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2812 2023-04-16 11:26:52.000000 mock-5.0.2/mock.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      531 2023-04-16 11:26:52.000000 mock-5.0.2/mock.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-16 11:26:52.000000 mock-5.0.2/mock.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-04-16 11:26:52.000000 mock-5.0.2/mock.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2023-04-16 11:26:52.000000 mock-5.0.2/mock.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1410 2023-04-16 11:26:52.041844 mock-5.0.2/setup.cfg
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      246 2023-04-16 11:26:45.000000 mock-5.0.2/setup.py
```

### Comparing `mock-5.0.1/CHANGELOG.rst` & `mock-5.0.2/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+5.0.2
+-----
+
+- gh-102978: Fixes :func:`unittest.mock.patch` not enforcing function
+  signatures for methods decorated with ``@classmethod`` or
+  ``@staticmethod`` when patch is called with ``autospec=True``.
+
+- gh-103329: Regression tests for the behaviour of
+  ``unittest.mock.PropertyMock`` were added.
+
 5.0.1
 -----
 
 - gh-100740: Fix ``unittest.mock.Mock`` not respecting the spec for
   attribute names prefixed with ``assert``.
 
 - gh-100690: ``Mock`` objects which are not unsafe will now raise an
```

### Comparing `mock-5.0.1/LICENSE.txt` & `mock-5.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mock-5.0.1/PKG-INFO` & `mock-5.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mock
-Version: 5.0.1
+Version: 5.0.2
 Summary: Rolling backport of unittest.mock for all Pythons
 Home-page: http://mock.readthedocs.org/en/latest/
 Author: Testing Cabal
 Author-email: testing-in-python@lists.idyll.org
 License: UNKNOWN
 Project-URL: Source, https://github.com/testing-cabal/mock
 Platform: UNKNOWN
```

### Comparing `mock-5.0.1/README.rst` & `mock-5.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `mock-5.0.1/mock/backports.py` & `mock-5.0.2/mock/backports.py`

 * *Files identical despite different names*

### Comparing `mock-5.0.1/mock/mock.py` & `mock-5.0.2/mock/mock.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,20 @@
     Return a (reduced func, signature) tuple, or None.
     """
     if isinstance(func, type) and not as_instance:
         # If it's a type and should be modelled as a type, use __init__.
         func = func.__init__
         # Skip the `self` argument in __init__
         eat_self = True
+    elif isinstance(func, (classmethod, staticmethod)):
+        if isinstance(func, classmethod):
+            # Skip the `cls` argument of a class method
+            eat_self = True
+        # Use the original decorated method to extract the correct function signature
+        func = func.__func__
     elif not isinstance(func, FunctionTypes):
         # If we really want to model an instance of the passed type,
         # __call__ should be looked up, not __init__.
         try:
             func = func.__call__
         except AttributeError:
             return None
```

### Comparing `mock-5.0.1/mock/tests/support.py` & `mock-5.0.2/mock/tests/support.py`

 * *Files identical despite different names*

### Comparing `mock-5.0.1/mock/tests/testasync.py` & `mock-5.0.2/mock/tests/testasync.py`

 * *Files identical despite different names*

### Comparing `mock-5.0.1/mock/tests/testcallable.py` & `mock-5.0.2/mock/tests/testcallable.py`

 * *Files identical despite different names*

### Comparing `mock-5.0.1/mock/tests/testhelpers.py` & `mock-5.0.2/mock/tests/testhelpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -957,14 +957,32 @@
                 return partial(lambda name: name, attribute)
 
         proxy = Foo()
         autospec = create_autospec(proxy)
         self.assertFalse(hasattr(autospec, '__name__'))
 
 
+    def test_autospec_signature_staticmethod(self):
+        class Foo:
+            @staticmethod
+            def static_method(a, b=10, *, c): pass
+
+        mock = create_autospec(Foo.__dict__['static_method'])
+        self.assertEqual(inspect.signature(Foo.static_method), inspect.signature(mock))
+
+
+    def test_autospec_signature_classmethod(self):
+        class Foo:
+            @classmethod
+            def class_method(cls, a, b=10, *, c): pass
+
+        mock = create_autospec(Foo.__dict__['class_method'])
+        self.assertEqual(inspect.signature(Foo.class_method), inspect.signature(mock))
+
+
     def test_spec_inspect_signature(self):
 
         def myfunc(x, y): pass
 
         mock = create_autospec(myfunc)
         mock(1, 2)
         mock(x=1, y=2)
@@ -1082,25 +1100,46 @@
 
             s.one = 3
             self.assertEqual(mock.mock_calls, [call(), call(), call(3)])
         finally:
             p.stop()
 
 
-    def test_propertymock_returnvalue(self):
+    def test_propertymock_bare(self):
         m = MagicMock()
         p = PropertyMock()
         type(m).foo = p
 
         returned = m.foo
         p.assert_called_once_with()
         self.assertIsInstance(returned, MagicMock)
         self.assertNotIsInstance(returned, PropertyMock)
 
 
+    def test_propertymock_returnvalue(self):
+        m = MagicMock()
+        p = PropertyMock(return_value=42)
+        type(m).foo = p
+
+        returned = m.foo
+        p.assert_called_once_with()
+        self.assertEqual(returned, 42)
+        self.assertNotIsInstance(returned, PropertyMock)
+
+
+    def test_propertymock_side_effect(self):
+        m = MagicMock()
+        p = PropertyMock(side_effect=ValueError)
+        type(m).foo = p
+
+        with self.assertRaises(ValueError):
+            m.foo
+        p.assert_called_once_with()
+
+
 class TestCallablePredicate(unittest.TestCase):
 
     def test_type(self):
         for obj in [str, bytes, int, list, tuple, SomeClass]:
             self.assertTrue(_callable(obj))
 
     def test_call_magic_method(self):
```

### Comparing `mock-5.0.1/mock/tests/testmagicmethods.py` & `mock-5.0.2/mock/tests/testmagicmethods.py`

 * *Files identical despite different names*

### Comparing `mock-5.0.1/mock/tests/testmock.py` & `mock-5.0.2/mock/tests/testmock.py`

 * *Files identical despite different names*

### Comparing `mock-5.0.1/mock/tests/testpatch.py` & `mock-5.0.2/mock/tests/testpatch.py`

 * *Files 4% similar despite different names*

```diff
@@ -992,14 +992,44 @@
 
     def test_autospec_classmethod(self):
         with patch('%s.Foo.class_method' % __name__, autospec=True) as method:
             Foo.class_method()
             method.assert_called_once_with()
 
 
+    def test_autospec_staticmethod_signature(self):
+        # Patched methods which are decorated with @staticmethod should have the same signature
+        class Foo:
+            @staticmethod
+            def static_method(a, b=10, *, c): pass
+
+        Foo.static_method(1, 2, c=3)
+
+        with patch.object(Foo, 'static_method', autospec=True) as method:
+            method(1, 2, c=3)
+            self.assertRaises(TypeError, method)
+            self.assertRaises(TypeError, method, 1)
+            self.assertRaises(TypeError, method, 1, 2, 3, c=4)
+
+
+    def test_autospec_classmethod_signature(self):
+        # Patched methods which are decorated with @classmethod should have the same signature
+        class Foo:
+            @classmethod
+            def class_method(cls, a, b=10, *, c): pass
+
+        Foo.class_method(1, 2, c=3)
+
+        with patch.object(Foo, 'class_method', autospec=True) as method:
+            method(1, 2, c=3)
+            self.assertRaises(TypeError, method)
+            self.assertRaises(TypeError, method, 1)
+            self.assertRaises(TypeError, method, 1, 2, 3, c=4)
+
+
     def test_autospec_with_new(self):
         patcher = patch('%s.function' % __name__, new=3, autospec=True)
         self.assertRaises(TypeError, patcher.start)
 
         module = sys.modules[__name__]
         patcher = patch.object(module, 'function', new=3, autospec=True)
         self.assertRaises(TypeError, patcher.start)
```

### Comparing `mock-5.0.1/mock/tests/testsealable.py` & `mock-5.0.2/mock/tests/testsealable.py`

 * *Files identical despite different names*

### Comparing `mock-5.0.1/mock/tests/testsentinel.py` & `mock-5.0.2/mock/tests/testsentinel.py`

 * *Files identical despite different names*

### Comparing `mock-5.0.1/mock/tests/testwith.py` & `mock-5.0.2/mock/tests/testwith.py`

 * *Files identical despite different names*

### Comparing `mock-5.0.1/mock.egg-info/PKG-INFO` & `mock-5.0.2/mock.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mock
-Version: 5.0.1
+Version: 5.0.2
 Summary: Rolling backport of unittest.mock for all Pythons
 Home-page: http://mock.readthedocs.org/en/latest/
 Author: Testing Cabal
 Author-email: testing-in-python@lists.idyll.org
 License: UNKNOWN
 Project-URL: Source, https://github.com/testing-cabal/mock
 Platform: UNKNOWN
```

### Comparing `mock-5.0.1/mock.egg-info/SOURCES.txt` & `mock-5.0.2/mock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mock-5.0.1/setup.cfg` & `mock-5.0.2/setup.cfg`

 * *Files identical despite different names*

