# Comparing `tmp/cupcake-0.1.2.tar.gz` & `tmp/cupcake-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cupcake-0.1.2.tar", max compression
+gzip compressed data, was "cupcake-0.1.3.tar", max compression
```

## Comparing `cupcake-0.1.2.tar` & `cupcake-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      761 2023-03-01 17:58:55.790012 cupcake-0.1.2/LICENSE
--rw-r--r--   0        0        0      568 2023-04-05 17:14:13.173286 cupcake-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       73 2023-03-13 22:19:09.065654 cupcake-0.1.2/src/cupcake/__init__.py
--rw-r--r--   0        0        0     4023 2023-03-13 20:49:00.721516 cupcake-0.1.2/src/cupcake/cascade.py
--rw-r--r--   0        0        0     2345 2023-03-24 13:54:18.178294 cupcake-0.1.2/src/cupcake/confee.py
--rw-r--r--   0        0        0       35 2023-03-08 23:12:26.626449 cupcake-0.1.2/src/cupcake/data/new/.gitignore
--rw-r--r--   0        0        0      446 2023-04-05 14:08:12.001491 cupcake-0.1.2/src/cupcake/data/new/CMakeLists.txt
--rw-r--r--   0        0        0     1534 2023-04-04 16:25:50.085034 cupcake-0.1.2/src/cupcake/data/new/conanfile.py
--rw-r--r--   0        0        0      177 2022-04-07 22:23:03.400195 cupcake-0.1.2/src/cupcake/data/new/include/{{name}}/{{name}}.hpp
--rw-r--r--   0        0        0       87 2022-04-07 22:23:55.073837 cupcake-0.1.2/src/cupcake/data/new/src/lib{{name}}.cpp
--rw-r--r--   0        0        0      143 2022-04-07 22:49:53.297481 cupcake-0.1.2/src/cupcake/data/new/src/{{name}}.cpp
--rw-r--r--   0        0        0      177 2023-03-10 21:15:53.093370 cupcake-0.1.2/src/cupcake/data/new/tests/CMakeLists.txt
--rw-r--r--   0        0        0      169 2022-04-07 22:20:24.683135 cupcake-0.1.2/src/cupcake/data/new/tests/{{name}}.cpp
--rw-r--r--   0        0        0      177 2023-03-01 15:12:58.048397 cupcake-0.1.2/src/cupcake/data/query/CMakeLists.txt
--rw-r--r--   0        0        0    23745 2023-04-05 16:41:40.778666 cupcake-0.1.2/src/cupcake/main.py
--rw-r--r--   0        0        0     6725 2023-03-08 20:46:34.258683 cupcake-0.1.2/src/cupcake/scratch.py
--rw-r--r--   0        0        0     1030 2023-04-05 17:14:20.219830 cupcake-0.1.2/setup.py
--rw-r--r--   0        0        0      618 2023-04-05 17:14:20.220043 cupcake-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      761 2023-03-01 17:58:55.790012 cupcake-0.1.3/LICENSE
+-rw-r--r--   0        0        0      549 2023-04-16 13:36:58.104474 cupcake-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-03-13 22:19:09.065654 cupcake-0.1.3/src/cupcake/__init__.py
+-rw-r--r--   0        0        0     4023 2023-03-13 20:49:00.721516 cupcake-0.1.3/src/cupcake/cascade.py
+-rw-r--r--   0        0        0     2345 2023-03-24 13:54:18.178294 cupcake-0.1.3/src/cupcake/confee.py
+-rw-r--r--   0        0        0       35 2023-03-08 23:12:26.626449 cupcake-0.1.3/src/cupcake/data/new/.gitignore
+-rw-r--r--   0        0        0      446 2023-04-05 14:08:12.001491 cupcake-0.1.3/src/cupcake/data/new/CMakeLists.txt
+-rw-r--r--   0        0        0     1534 2023-04-04 16:25:50.085034 cupcake-0.1.3/src/cupcake/data/new/conanfile.py
+-rw-r--r--   0        0        0      177 2022-04-07 22:23:03.400195 cupcake-0.1.3/src/cupcake/data/new/include/{{name}}/{{name}}.hpp
+-rw-r--r--   0        0        0       87 2022-04-07 22:23:55.073837 cupcake-0.1.3/src/cupcake/data/new/src/lib{{name}}.cpp
+-rw-r--r--   0        0        0      143 2022-04-07 22:49:53.297481 cupcake-0.1.3/src/cupcake/data/new/src/{{name}}.cpp
+-rw-r--r--   0        0        0      177 2023-03-10 21:15:53.093370 cupcake-0.1.3/src/cupcake/data/new/tests/CMakeLists.txt
+-rw-r--r--   0        0        0      169 2022-04-07 22:20:24.683135 cupcake-0.1.3/src/cupcake/data/new/tests/{{name}}.cpp
+-rw-r--r--   0        0        0      177 2023-03-01 15:12:58.048397 cupcake-0.1.3/src/cupcake/data/query/CMakeLists.txt
+-rw-r--r--   0        0        0    27445 2023-04-16 01:37:02.469659 cupcake-0.1.3/src/cupcake/main.py
+-rw-r--r--   0        0        0     6725 2023-03-08 20:46:34.258683 cupcake-0.1.3/src/cupcake/scratch.py
+-rw-r--r--   0        0        0     1004 2023-04-16 13:37:27.791882 cupcake-0.1.3/setup.py
+-rw-r--r--   0        0        0      578 2023-04-16 13:37:27.792074 cupcake-0.1.3/PKG-INFO
```

### Comparing `cupcake-0.1.2/LICENSE` & `cupcake-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cupcake-0.1.2/pyproject.toml` & `cupcake-0.1.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "cupcake"
-version = "0.1.2"
+version = "0.1.3"
 description = "Make C++ a piece of cake."
 authors = ["John Freeman <jfreeman08@gmail.com>"]
 packages = [{include = "cupcake", from = "src"}]
 
 [tool.poetry.scripts]
 cupcake = 'cupcake.main:main'
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.0.4"
 click-option-group = "^0.5.3"
 tomlkit = "^0.10.1"
 jinja2 = "^3.1.1"
-semver = "^2.13.0"
 libcst = "^0.4.9"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.1"
 pytest-xdist = "^3.2.1"
 
 [build-system]
```

### Comparing `cupcake-0.1.2/src/cupcake/cascade.py` & `cupcake-0.1.3/src/cupcake/cascade.py`

 * *Files identical despite different names*

### Comparing `cupcake-0.1.2/src/cupcake/confee.py` & `cupcake-0.1.3/src/cupcake/confee.py`

 * *Files identical despite different names*

### Comparing `cupcake-0.1.2/src/cupcake/data/new/conanfile.py` & `cupcake-0.1.3/src/cupcake/data/new/conanfile.py`

 * *Files identical despite different names*

### Comparing `cupcake-0.1.2/src/cupcake/main.py` & `cupcake-0.1.3/src/cupcake/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 import hashlib
 from importlib import resources
 import itertools
 import jinja2
 import json
 import libcst as cst
 import libcst.matchers
+import operator
 import os
 import pathlib
 import re
-import semver
 import shlex
 import shutil
 import subprocess
 import tempfile
+import urllib.parse
 
 from cupcake import cascade, confee
 
 def run(command, *args, **kwargs):
     # TODO: Print this in a special color.
     print(' '.join(shlex.quote(str(arg)) for arg in command), flush=True)
     proc = subprocess.run(command, *args, **kwargs)
@@ -43,20 +44,105 @@
 FLAVORS = {
     'release': 'Release',
     'debug': 'Debug',
 }
 
 PATTERN_INDEX_FILENAME = re.compile(r'^index-.*\.json$')
 
+def const(value):
+    def f(*args, **kwargs):
+        return value
+    return f
+
+def compare(a, b):
+    # Insane that Python does not have an efficient method for this.
+    # https://stackoverflow.com/q/50782317/618906
+    if a < b:
+        return -1
+    if a > b:
+        return 1
+    return 0
+
+nonet = type(None)
+compares = {
+    (int, int): operator.sub,
+    (str, str): compare,
+    (int, nonet): const(1),
+    (nonet, int): const(-1),
+    (int, str): const(1),
+    (str, int): const(-1),
+    (str, nonet): const(-1),
+    (nonet, str): const(1),
+}
+
+def print_call():
+    def decorate(f):
+        @functools.wraps(f)
+        def decorated(*args, **kwargs):
+            argss = ', '.join(map(str, args))
+            print(f'{f.__name__}({argss}) => ', end='')
+            value = f(*args, **kwargs)
+            print(value)
+            return value
+        return decorated
+    return decorate
+
+def compare_version(a, b):
+    # Not all Conan packages use Semantic Versioning.
+    # To be as flexible as possible,
+    # we treat version strings as non-digit-separated sequences of numbers.
+    # Sequences are compared item-by-item, in order.
+    # Numbers are compared numerically,
+    # non-numbers are compared lexicographically.
+    # Numbers are considered higher/later/younger versions than non-numbers.
+    # Numbers are considered higher/later/younger versions than nothing.
+    # Non-numbers are considered lower/earlier/older versions than nothing.
+    aa = re.split('(\D+)', a)
+    bb = re.split('(\D+)', b)
+    for aaa, bbb in itertools.zip_longest(aa, bb):
+        try:
+            aaa = int(aaa)
+            aaat = int
+        except (ValueError, TypeError):
+            aaat = type(aaa)
+        try:
+            bbb = int(bbb)
+            bbbt = int
+        except (ValueError, TypeError):
+            bbbt = type(bbb)
+        diff = compares[(aaat, bbbt)](aaa, bbb)
+        if diff:
+            return diff
+    return 0
+
+key = functools.cmp_to_key(
+    lambda a, b: compare_version(a, b)
+)
+
+PATTERN_GITHUB_PATH = r'/([^/]+)/([^/]+)(?:/tree/[^/]+(.+))?'
+
+@contextmanager
+def pack_directory(path):
+    yield path
+
+@contextmanager
+def pack_github(path):
+    """Return a path to a Conan package directory identified by _url_."""
+    with tempfile.TemporaryDirectory() as tmp:
+        user, project, suffix = re.match(PATTERN_GITHUB_PATH, path).groups()
+        if suffix is None:
+            suffix = '/'
+        run(['git', 'clone', f'https://github.com/{user}/{project}', tmp])
+        yield tmp + suffix
 
 class SearchResult:
     """Representation for a Conan package search result."""
 
     key = functools.cmp_to_key(
-        lambda a, b: semver.compare(a.version, b.version)
+        lambda a, b: compare_version(a.version, b.version)
     )
 
     def __init__(self, remote, reference):
         self.remote = remote
         match = re.match(f'^([^/]+)/([^@]+)(?:@(.*))?$', reference)
         self.package = match[1]
         self.version = match[2]
@@ -64,18 +150,14 @@
 
     def __str__(self):
         s = f'{self.package}/{self.version}@'
         if self.remainder:
             s += self.remainder
         return s
 
-    @staticmethod
-    def compare(a, b):
-        return semver.compare(a.version, b.version)
-
 class Conan:
     def __init__(self, CONAN):
         self.CONAN = CONAN
 
     def search(self, query):
         # TODO: Look into Conan Python API. Currently undocumented.
         # TODO: Implement version constraints like Python.
@@ -107,16 +189,15 @@
             results = [
                 SearchResult(result['remote'], item['recipe']['id'])
                 for result in results
                 for item in result['items']
             ]
             # They seem to be in ascending version order,
             # but I'm not sure we can rely on that.
-            key = functools.cmp_to_key(SearchResult.compare)
-            results = sorted(results, key=key, reverse=True)
+            results = sorted(results, key=SearchResult.key, reverse=True)
             return results
 
 
 class CMake:
     def __init__(self, CMAKE):
         self.CMAKE = CMAKE
 
@@ -675,17 +756,47 @@
             tree = cst.parse_module(conanfile_path_.read_bytes())
             tree = tree.visit(RemoveRequirement(package))
             recipe_out.write(tree.code)
             recipe_out.flush()
             shutil.copy(recipe_out.name, conanfile_path_)
 
     @cascade.command()
-    def pack(self, CONAN, source_dir_):
-        """Publish a Conan package."""
-        run([CONAN, 'create', source_dir_])
+    @cascade.argument('url', default='.')
+    def pack(self, CONAN, url):
+        """
+        Add a Conan package to your local cache.
+
+        For this command, it is important to understand the idea of a "Conan
+        package directory", which is a directory containing a `conanfile.py`
+        Conan recipe.
+        The URL argument must resolve to a Conan package directory.
+
+        The default URL is `.`, which is the package you are in,
+        but a few schemes are understood:
+
+        \b
+        - An absolute or relative path to a Conan package directory.
+        - A file:// URL for an absolute path to a Conan package directory.
+        - An http:// or https:// URL for the github.com domain pointing to
+          a Conan package directory.
+        - A gh://username/project[/path/to/directory] URL that identifies
+          a GitHub project and an optional path within that project to
+          a Conan package directory.
+        """
+        parts = urllib.parse.urlparse(url)
+        if parts.scheme in ('http', 'https'):
+            if parts.netloc != 'github.com':
+                raise ValueError('unknown URL')
+            context = pack_github(parts.path)
+        elif parts.scheme == 'gh':
+            context = pack_github(parts.path)
+        elif parts.scheme in ('', 'file'):
+            context = pack_directory(parts.path)
+        with context as path:
+            run([CONAN, 'export', path])
 
     @cascade.command()
     def clean(self, build_dir_path_):
         """Remove the build directory."""
         shutil.rmtree(build_dir_path_, ignore_errors=True)
 
 Cupcake()
```

### Comparing `cupcake-0.1.2/src/cupcake/scratch.py` & `cupcake-0.1.3/src/cupcake/scratch.py`

 * *Files identical despite different names*

### Comparing `cupcake-0.1.2/setup.py` & `cupcake-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,23 +13,22 @@
  'cupcake.data.new': ['include/{{name}}/*', 'src/*', 'tests/*']}
 
 install_requires = \
 ['click-option-group>=0.5.3,<0.6.0',
  'click>=8.0.4,<9.0.0',
  'jinja2>=3.1.1,<4.0.0',
  'libcst>=0.4.9,<0.5.0',
- 'semver>=2.13.0,<3.0.0',
  'tomlkit>=0.10.1,<0.11.0']
 
 entry_points = \
 {'console_scripts': ['cupcake = cupcake.main:main']}
 
 setup_kwargs = {
     'name': 'cupcake',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Make C++ a piece of cake.',
     'long_description': None,
     'author': 'John Freeman',
     'author_email': 'jfreeman08@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `cupcake-0.1.2/PKG-INFO` & `cupcake-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: cupcake
-Version: 0.1.2
+Version: 0.1.3
 Summary: Make C++ a piece of cake.
 Author: John Freeman
 Author-email: jfreeman08@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: click (>=8.0.4,<9.0.0)
 Requires-Dist: click-option-group (>=0.5.3,<0.6.0)
 Requires-Dist: jinja2 (>=3.1.1,<4.0.0)
 Requires-Dist: libcst (>=0.4.9,<0.5.0)
-Requires-Dist: semver (>=2.13.0,<3.0.0)
 Requires-Dist: tomlkit (>=0.10.1,<0.11.0)
```

