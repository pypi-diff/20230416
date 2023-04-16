# Comparing `tmp/chope-0.1.1.tar.gz` & `tmp/chope-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chope-0.1.1.tar", last modified: Fri Apr 14 12:38:51 2023, max compression
+gzip compressed data, was "chope-0.1.2.tar", last modified: Sun Apr 16 07:30:00 2023, max compression
```

## Comparing `chope-0.1.1.tar` & `chope-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 johantjuatja   (501) staff       (20)        0 2023-04-14 12:38:51.326882 chope-0.1.1/
--rw-r--r--   0 johantjuatja   (501) staff       (20)     1065 2023-04-08 07:11:52.000000 chope-0.1.1/LICENSE
--rw-r--r--   0 johantjuatja   (501) staff       (20)     3298 2023-04-14 12:38:51.326524 chope-0.1.1/PKG-INFO
--rw-r--r--   0 johantjuatja   (501) staff       (20)     2600 2023-04-14 12:14:13.000000 chope-0.1.1/README.md
-drwxr-xr-x   0 johantjuatja   (501) staff       (20)        0 2023-04-14 12:38:51.323890 chope-0.1.1/chope/
--rw-r--r--   0 johantjuatja   (501) staff       (20)     3958 2023-04-09 14:42:26.000000 chope-0.1.1/chope/__init__.py
--rw-r--r--   0 johantjuatja   (501) staff       (20)     1677 2023-04-10 13:16:55.000000 chope-0.1.1/chope/css.py
--rw-r--r--   0 johantjuatja   (501) staff       (20)     2248 2023-04-12 14:25:39.000000 chope-0.1.1/chope/element.py
-drwxr-xr-x   0 johantjuatja   (501) staff       (20)        0 2023-04-14 12:38:51.325047 chope-0.1.1/chope.egg-info/
--rw-r--r--   0 johantjuatja   (501) staff       (20)     3298 2023-04-14 12:38:51.000000 chope-0.1.1/chope.egg-info/PKG-INFO
--rw-r--r--   0 johantjuatja   (501) staff       (20)      282 2023-04-14 12:38:51.000000 chope-0.1.1/chope.egg-info/SOURCES.txt
--rw-r--r--   0 johantjuatja   (501) staff       (20)        1 2023-04-14 12:38:51.000000 chope-0.1.1/chope.egg-info/dependency_links.txt
--rw-r--r--   0 johantjuatja   (501) staff       (20)        7 2023-04-14 12:38:51.000000 chope-0.1.1/chope.egg-info/requires.txt
--rw-r--r--   0 johantjuatja   (501) staff       (20)        6 2023-04-14 12:38:51.000000 chope-0.1.1/chope.egg-info/top_level.txt
--rw-r--r--   0 johantjuatja   (501) staff       (20)      833 2023-04-14 12:38:26.000000 chope-0.1.1/pyproject.toml
--rw-r--r--   0 johantjuatja   (501) staff       (20)       38 2023-04-14 12:38:51.326951 chope-0.1.1/setup.cfg
-drwxr-xr-x   0 johantjuatja   (501) staff       (20)        0 2023-04-14 12:38:51.326000 chope-0.1.1/tests/
--rw-r--r--   0 johantjuatja   (501) staff       (20)        0 2023-04-08 07:53:38.000000 chope-0.1.1/tests/__init__.py
--rw-r--r--   0 johantjuatja   (501) staff       (20)      761 2023-04-10 13:07:47.000000 chope-0.1.1/tests/test_css.py
--rw-r--r--   0 johantjuatja   (501) staff       (20)     1641 2023-04-12 14:01:22.000000 chope-0.1.1/tests/test_element.py
+drwxr-xr-x   0 johantjuatja   (501) staff       (20)        0 2023-04-16 07:30:00.329008 chope-0.1.2/
+-rw-r--r--   0 johantjuatja   (501) staff       (20)     1065 2023-04-08 07:11:52.000000 chope-0.1.2/LICENSE
+-rw-r--r--   0 johantjuatja   (501) staff       (20)     6098 2023-04-16 07:30:00.328629 chope-0.1.2/PKG-INFO
+-rw-r--r--   0 johantjuatja   (501) staff       (20)     5401 2023-04-16 07:11:01.000000 chope-0.1.2/README.md
+drwxr-xr-x   0 johantjuatja   (501) staff       (20)        0 2023-04-16 07:30:00.325956 chope-0.1.2/chope/
+-rw-r--r--   0 johantjuatja   (501) staff       (20)     3958 2023-04-09 14:42:26.000000 chope-0.1.2/chope/__init__.py
+-rw-r--r--   0 johantjuatja   (501) staff       (20)     1677 2023-04-10 13:16:55.000000 chope-0.1.2/chope/css.py
+-rw-r--r--   0 johantjuatja   (501) staff       (20)     2404 2023-04-16 07:25:48.000000 chope-0.1.2/chope/element.py
+drwxr-xr-x   0 johantjuatja   (501) staff       (20)        0 2023-04-16 07:30:00.327256 chope-0.1.2/chope.egg-info/
+-rw-r--r--   0 johantjuatja   (501) staff       (20)     6098 2023-04-16 07:30:00.000000 chope-0.1.2/chope.egg-info/PKG-INFO
+-rw-r--r--   0 johantjuatja   (501) staff       (20)      282 2023-04-16 07:30:00.000000 chope-0.1.2/chope.egg-info/SOURCES.txt
+-rw-r--r--   0 johantjuatja   (501) staff       (20)        1 2023-04-16 07:30:00.000000 chope-0.1.2/chope.egg-info/dependency_links.txt
+-rw-r--r--   0 johantjuatja   (501) staff       (20)        7 2023-04-16 07:30:00.000000 chope-0.1.2/chope.egg-info/requires.txt
+-rw-r--r--   0 johantjuatja   (501) staff       (20)        6 2023-04-16 07:30:00.000000 chope-0.1.2/chope.egg-info/top_level.txt
+-rw-r--r--   0 johantjuatja   (501) staff       (20)      833 2023-04-16 07:26:46.000000 chope-0.1.2/pyproject.toml
+-rw-r--r--   0 johantjuatja   (501) staff       (20)       38 2023-04-16 07:30:00.329087 chope-0.1.2/setup.cfg
+drwxr-xr-x   0 johantjuatja   (501) staff       (20)        0 2023-04-16 07:30:00.328059 chope-0.1.2/tests/
+-rw-r--r--   0 johantjuatja   (501) staff       (20)        0 2023-04-08 07:53:38.000000 chope-0.1.2/tests/__init__.py
+-rw-r--r--   0 johantjuatja   (501) staff       (20)      761 2023-04-10 13:07:47.000000 chope-0.1.2/tests/test_css.py
+-rw-r--r--   0 johantjuatja   (501) staff       (20)     1673 2023-04-16 07:22:38.000000 chope-0.1.2/tests/test_element.py
```

### Comparing `chope-0.1.1/LICENSE` & `chope-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chope-0.1.1/chope/__init__.py` & `chope-0.1.2/chope/__init__.py`

 * *Files identical despite different names*

### Comparing `chope-0.1.1/chope/css.py` & `chope-0.1.2/chope/css.py`

 * *Files identical despite different names*

### Comparing `chope-0.1.1/chope/element.py` & `chope-0.1.2/chope/element.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,27 +46,31 @@
     def render(self, indent: int = 2) -> str:
         nl = '\n'
         indented = indent > 0
 
         comp_str = nl * indented
         for comp in self._components:
             if isinstance(comp, str):
-                comp_str += f'{" " * indent}{comp}{nl * indented}'
+                _comp = comp.replace('\n', '<br>')
+                comp_str += f'{" " * indent}{_comp}{nl * indented}'
             else:
                 _comp_str = comp.render(indent).replace(
                     nl, f'{nl * indented}{" " * indent}')
                 comp_str += f'{" " * indent}{_comp_str}{nl * indented}'
 
         name = self.__class__.__name__
 
         attrs_str = f' id="{self._id}"' if self._id else ''
         attrs_str += f' class="{self._classes}"' if self._classes else ''
 
         for attr, val in self._attributes.items():
-            val = f'"{val}"' if isinstance(val, str) else str(val)
+            if isinstance(val, bool):
+                attrs_str += f' {attr}'
+            else:
+                val = f'"{val}"' if isinstance(val, str) else str(val)
 
-            attrs_str += f' {attr}={val}'
+                attrs_str += f' {attr}={val}'
 
         return f'<{name}{attrs_str}>{comp_str}</{name}>'
 
 
 Component = Union[str, Element, Css]
```

### Comparing `chope-0.1.1/pyproject.toml` & `chope-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chope"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     {name = "Johan Tjuatja", email = "hanstjua@yahoo.co.id"},
 ]
 description = "CSS & HTML on Python Easily"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `chope-0.1.1/tests/test_css.py` & `chope-0.1.2/tests/test_css.py`

 * *Files identical despite different names*

### Comparing `chope-0.1.1/tests/test_element.py` & `chope-0.1.2/tests/test_element.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pytest
 from chope import Element
 from chope.css import Css
 
 expected = \
-"""<e1 class="my-class" color="yellow" size=123>
+"""<e1 class="my-class" color="yellow" size=123 autofocus>
     text
     <e2>
-        word
+        word<br>
     </e2>
     <e3>
         letter
         space
     </e3>
 </e1>"""
 
@@ -21,18 +21,18 @@
 
     class e2(Element):
         pass
 
     class e3(Element):
         pass
 
-    component = e1(class_='my-class', color='yellow', size=123)[
+    component = e1(class_='my-class', color='yellow', size=123, autofocus=True)[
         'text',
         e2[
-            'word'
+            'word\n'
         ],
         e3[
             'letter',
             'space'
         ]
     ]
```

