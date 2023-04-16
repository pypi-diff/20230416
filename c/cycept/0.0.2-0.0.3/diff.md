# Comparing `tmp/cycept-0.0.2.tar.gz` & `tmp/cycept-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycept-0.0.2.tar", last modified: Wed Apr 12 16:35:50 2023, max compression
+gzip compressed data, was "cycept-0.0.3.tar", last modified: Sun Apr 16 18:27:27 2023, max compression
```

## Comparing `cycept-0.0.2.tar` & `cycept-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-04-12 16:35:50.130908 cycept-0.0.2/
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     1068 2023-04-01 21:39:01.000000 cycept-0.0.2/LICENSE
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     5571 2023-04-12 16:35:50.130908 cycept-0.0.2/PKG-INFO
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     4236 2023-04-12 12:45:01.000000 cycept-0.0.2/README.md
-drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-04-12 16:35:50.126908 cycept-0.0.2/cycept/
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)       77 2023-04-11 00:49:17.000000 cycept-0.0.2/cycept/__init__.py
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    26018 2023-04-12 15:49:06.000000 cycept-0.0.2/cycept/call.py
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     2282 2023-04-12 12:46:27.000000 cycept-0.0.2/cycept/compile.py
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    24974 2023-04-12 14:06:13.000000 cycept-0.0.2/cycept/core.py
-drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-04-12 16:35:50.130908 cycept-0.0.2/cycept/tests/
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)      618 2023-04-12 15:50:45.000000 cycept-0.0.2/cycept/tests/__init__.py
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     9385 2023-04-12 14:15:20.000000 cycept-0.0.2/cycept/tests/test_cycept.py
-drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-04-12 16:35:50.130908 cycept-0.0.2/cycept.egg-info/
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     5571 2023-04-12 16:35:50.000000 cycept-0.0.2/cycept.egg-info/PKG-INFO
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)      301 2023-04-12 16:35:50.000000 cycept-0.0.2/cycept.egg-info/SOURCES.txt
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)        1 2023-04-12 16:35:50.000000 cycept-0.0.2/cycept.egg-info/dependency_links.txt
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)       99 2023-04-12 16:35:50.000000 cycept-0.0.2/cycept.egg-info/requires.txt
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)        7 2023-04-12 16:35:50.000000 cycept-0.0.2/cycept.egg-info/top_level.txt
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     1581 2023-04-12 16:17:29.000000 cycept-0.0.2/pyproject.toml
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)       38 2023-04-12 16:35:50.130908 cycept-0.0.2/setup.cfg
+drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-04-16 18:27:27.419529 cycept-0.0.3/
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     1068 2023-04-01 21:39:01.000000 cycept-0.0.3/LICENSE
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     6196 2023-04-16 18:27:27.419529 cycept-0.0.3/PKG-INFO
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     4840 2023-04-16 18:25:44.000000 cycept-0.0.3/README.md
+drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-04-16 18:27:27.419529 cycept-0.0.3/cycept/
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)       84 2023-04-15 21:05:00.000000 cycept-0.0.3/cycept/__init__.py
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    26554 2023-04-16 00:23:56.000000 cycept-0.0.3/cycept/call.py
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     4767 2023-04-16 17:37:25.000000 cycept-0.0.3/cycept/compile.py
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    22931 2023-04-15 18:33:58.000000 cycept-0.0.3/cycept/core.py
+drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-04-16 18:27:27.419529 cycept-0.0.3/cycept/tests/
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)      998 2023-04-16 12:40:48.000000 cycept-0.0.3/cycept/tests/__init__.py
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    11614 2023-04-15 22:47:01.000000 cycept-0.0.3/cycept/tests/test_cycept.py
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    14083 2023-04-16 17:40:47.000000 cycept-0.0.3/cycept/tests/test_perf.py
+drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-04-16 18:27:27.419529 cycept-0.0.3/cycept.egg-info/
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     6196 2023-04-16 18:27:27.000000 cycept-0.0.3/cycept.egg-info/PKG-INFO
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)      327 2023-04-16 18:27:27.000000 cycept-0.0.3/cycept.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)        1 2023-04-16 18:27:27.000000 cycept-0.0.3/cycept.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)      185 2023-04-16 18:27:27.000000 cycept-0.0.3/cycept.egg-info/requires.txt
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)        7 2023-04-16 18:27:27.000000 cycept-0.0.3/cycept.egg-info/top_level.txt
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     1712 2023-04-16 18:26:29.000000 cycept-0.0.3/pyproject.toml
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)       38 2023-04-16 18:27:27.419529 cycept-0.0.3/setup.cfg
```

### Comparing `cycept-0.0.2/LICENSE` & `cycept-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cycept-0.0.2/PKG-INFO` & `cycept-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycept
-Version: 0.0.2
+Version: 0.0.3
 Summary: Effortless just-in-time compilation of Python functions, powered by Cython
 Author-email: Jeppe Dakin <jeppe_dakin@hotmail.com>
 Project-URL: Download, https://pypi.python.org/pypi/cycept
 Project-URL: Changelog, https://github.com/jmd-dk/cycept/blob/main/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/jmd-dk/cycept/issues
 Project-URL: Source code, https://github.com/jmd-dk/cycept
 Classifier: Intended Audience :: Developers
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Cython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: repl
 Provides-Extra: test
 License-File: LICENSE
 
 # Cycept
 Effortless just-in-time compilation of Python functions,
 powered by [Cython](https://cython.org/).
 
@@ -38,17 +39,22 @@
 python -m pip install cycept
 ```
 
 Cycept requires Python 3.9 or later.
 
 To run Cycept a C compiler needs to be installed on the system.
 
-* On **Linux** you may install [GCC](https://gcc.gnu.org/) (Debian-like distros: `sudo apt install build-essential`).
-* On **macOS** you may install [Xcode](https://developer.apple.com/xcode/).
-* On **Windows** you may install [MSVC](https://visualstudio.microsoft.com/visual-cpp-build-tools/).
+* On **Linux** you may install [GCC](https://gcc.gnu.org/)
+  (Debian-like distros: `sudo apt install build-essential`).
+* On **macOS** you may install [Clang](https://clang.llvm.org/)
+  (available through [Xcode](https://developer.apple.com/xcode/)).
+* On **Windows** you may install
+  [MSVC](https://en.wikipedia.org/wiki/Microsoft_Visual_C%2B%2B)
+  (available through
+  [Microsoft C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/)).
 
 
 ## Quick demo
 ```python
 """Comparison of Python function JITs
 
 Below we implement the sample function sum((a - b)**2) where a and b
@@ -154,26 +160,36 @@
 
 See the help info on `cycept.jit` for optional arguments:
 ```bash
 python -c 'import cycept; help(cycept.jit)'
 ```
 
 
-## Test suite
+## Tests
 The code contains a unit test suite which may be run as
-```
-python -c "import cycept; cycept.test()"
+```bash
+python -c "import cycept; cycept.test('cycept')"
 ```
 This requires [pytest](https://docs.pytest.org/) to be installed
 (`python -m pip install pytest`).
 
+If `cycept.test()` is called without an argument it will further run a
+performance test suite, though showing only whether each test passes or not.
+To display the actual performance benchmarks, run the performance test suite
+by itself using
+```bash
+python -c "import cycept; cycept.bench(show_func=True)"
+```
+
 
 ## What's up with the name?
 'Cycept' is an amalgamation of '[Cython](https://cython.org/)' and
 '[CO*N*CEPT](https://github.com/jmd-dk/concept)', the latter of which is a
 cosmological simulation code that makes heavy use of code transformation,
 both custom and through Cython. As the author of both projects, Cycept is my
 attempt to extract some of the code transformation ideas buried within
 CO*N*CEPT, making them available within an easy-to-use library.
 Though no code is shared between the projects, in many respects Cycept
 can be considered a spiritual descendant of CO*N*CEPT.
+Furthermore, 'Cy*cept*' has a nice in*cept*ion ring to it,
+which seems fitting for a piece of code that generates code.
```

### Comparing `cycept-0.0.2/README.md` & `cycept-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,17 +9,22 @@
 python -m pip install cycept
 ```
 
 Cycept requires Python 3.9 or later.
 
 To run Cycept a C compiler needs to be installed on the system.
 
-* On **Linux** you may install [GCC](https://gcc.gnu.org/) (Debian-like distros: `sudo apt install build-essential`).
-* On **macOS** you may install [Xcode](https://developer.apple.com/xcode/).
-* On **Windows** you may install [MSVC](https://visualstudio.microsoft.com/visual-cpp-build-tools/).
+* On **Linux** you may install [GCC](https://gcc.gnu.org/)
+  (Debian-like distros: `sudo apt install build-essential`).
+* On **macOS** you may install [Clang](https://clang.llvm.org/)
+  (available through [Xcode](https://developer.apple.com/xcode/)).
+* On **Windows** you may install
+  [MSVC](https://en.wikipedia.org/wiki/Microsoft_Visual_C%2B%2B)
+  (available through
+  [Microsoft C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/)).
 
 
 ## Quick demo
 ```python
 """Comparison of Python function JITs
 
 Below we implement the sample function sum((a - b)**2) where a and b
@@ -125,26 +130,36 @@
 
 See the help info on `cycept.jit` for optional arguments:
 ```bash
 python -c 'import cycept; help(cycept.jit)'
 ```
 
 
-## Test suite
+## Tests
 The code contains a unit test suite which may be run as
-```
-python -c "import cycept; cycept.test()"
+```bash
+python -c "import cycept; cycept.test('cycept')"
 ```
 This requires [pytest](https://docs.pytest.org/) to be installed
 (`python -m pip install pytest`).
 
+If `cycept.test()` is called without an argument it will further run a
+performance test suite, though showing only whether each test passes or not.
+To display the actual performance benchmarks, run the performance test suite
+by itself using
+```bash
+python -c "import cycept; cycept.bench(show_func=True)"
+```
+
 
 ## What's up with the name?
 'Cycept' is an amalgamation of '[Cython](https://cython.org/)' and
 '[CO*N*CEPT](https://github.com/jmd-dk/concept)', the latter of which is a
 cosmological simulation code that makes heavy use of code transformation,
 both custom and through Cython. As the author of both projects, Cycept is my
 attempt to extract some of the code transformation ideas buried within
 CO*N*CEPT, making them available within an easy-to-use library.
 Though no code is shared between the projects, in many respects Cycept
 can be considered a spiritual descendant of CO*N*CEPT.
+Furthermore, 'Cy*cept*' has a nice in*cept*ion ring to it,
+which seems fitting for a piece of code that generates code.
```

### Comparing `cycept-0.0.2/cycept/call.py` & `cycept-0.0.3/cycept/call.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # various aspects of the function call to be jitted.
 class FunctionCall:
 
     class Compiled(typing.NamedTuple):
         func: object
         module: object
         source: str
+        source_ext: str
         html: str
 
     class Time(typing.NamedTuple):
         compile: float
         total: float
 
     def __init__(self, func, args, kwargs):
@@ -363,30 +364,32 @@
                         tp = self.call.types[node.id]
                         if tp.startswith('cython.') and '[' not in tp:
                             return True
                     elif isinstance(node, ast.Constant):
                         if isinstance(node.value, int):
                             return True
                     return False
-                n_nested_subscripts = 0
+                nodes_subscript = []
                 while isinstance(node, ast.Subscript):
-                    n_nested_subscripts += 1
-                    node_subscript = node
+                    nodes_subscript.append(node)
                     node = node.value
                 if not isinstance(node, ast.Name) or node.id not in self.names:
                     return
-                if n_nested_subscripts == 1:
-                    # Memoryview/array indexing arr[x].
-                    # If we can prove that x is a scalar
+                if nodes_subscript:
+                    # Memoryview/array indexing arr[x0][x1, x2][...].
+                    # If we can prove that all x are scalars
                     # we use the memoryview as is.
-                    if isinstance(node_subscript.slice, ast.Tuple):
-                        if all(is_scalar(el) for el in node_subscript.slice.elts):
-                            return node
-                    elif is_scalar(node_subscript.slice):
-                        return node
+                    for node_subscript in nodes_subscript:
+                        if isinstance(node_subscript.slice, ast.Tuple):
+                            if not all(is_scalar(el) for el in node_subscript.slice.elts):
+                                break
+                        elif not is_scalar(node_subscript.slice):
+                            break
+                    else:
+                        return
                 # Wrap node
                 self.wrapped_any = True
                 if kind == 0:
                     node.id = f'{self.wrapper_func}({node.id})'
                 elif kind == 1:
                     self.tmp_any = True
                     node.id = f'{self.tmp_name} = {self.wrapper_func}({node.id}); {self.tmp_name}'
@@ -543,28 +546,29 @@
                 self._contains_closure = True
         if ClosureVisitor(self).contains_closure():
             return False
         # No violations found
         return True
 
     # Method for handling Cythonization and C compilation
-    def compile(self, optimizations, html, silent):
+    def compile(self, optimizations, c_lang, html, silent):
         # Cythonize and compile extension module within temporary directory.
         # The compiled module is then imported (through hacking of sys.path)
         # before it is removed from disk.
         @contextlib.contextmanager
         def hack_sys_path():
             sys.path.append(dir_name)
             yield
             sys.path.remove(dir_name)
         module_name = f'_cycept_module_{self.hash}'
         namespace = {}
+        source_c = None
         html_annotation = None
         tempfile_kwargs = {}
-        if sys.version_info[:2] >= (3, 10):
+        if sys.version_info >= (3, 10):
             tempfile_kwargs |= {'ignore_cleanup_errors': True}
         with (
             tempfile.TemporaryDirectory(**tempfile_kwargs) as dir_name,
             hack_sys_path(),
         ):
             # Write Cython source to file
             module_path = pathlib.Path(dir_name) / module_name
@@ -576,14 +580,15 @@
                 '-c',
                 '; '.join([
                     'import cycept.compile',
                     'cycept.compile.compile({})'
                     .format(', '.join([
                         f'{str(module_path)!r}',
                         f'{optimizations!r}',
+                        f'{c_lang!r}',
                         f'{html!r}',
                     ]))
                 ]),
             ]
             run_kwargs = {}
             if silent:
                 run_kwargs |= {
@@ -602,17 +607,21 @@
                 msg = ['Cythonization failed.']
                 if silent:
                     msg += ['Subprocess output:', cproc.stdout]
                 raise OSError('\n'.join(msg))
             # Import function from compiled module into temporary namespace
             exec(f'import {module_name}', namespace)
             # Read in C source and annotated HTML
-            source_c = module_path.with_suffix('.c').read_text('utf-8')
-            path_html = module_path.with_suffix('.html')
-            if path_html.is_file():
+            for ext in ['c', 'cc', 'cpp', 'cxx']:
+                if (path_c := module_path.with_suffix(f'.{ext}')).is_file():
+                    source_c = path_c.read_text('utf-8')
+                    break
+            else:
+                ext = None
+            if (path_html := module_path.with_suffix('.html')).is_file():
                 html_annotation = path_html.read_text('utf-8')
         # Extract compiled function
         module_compiled = namespace[module_name]
         module_compiled_dict = module_compiled.__dict__
         func_compiled = module_compiled_dict[self.func_name]
         # Replace fake globals and non-locals with actual
         # globals and non-locals within extension module.
@@ -621,28 +630,33 @@
                 continue
             module_compiled_dict[name] = val
         # Store compilation products
         self.compiled = self.Compiled(
             func_compiled,
             module_compiled,
             source_c,
+            ext,
             html_annotation,
         )
         # Return compilation time (in seconds)
         return toc - tic
 
     # Method for viewing the annotated HTML
     def __call__(self, dir_name=None):
         if self.compiled is None or self.compiled.html is None:
             print(f'No Cython HTML annotation generated for {self.func_name}()')
             return
         if dir_name is None:
             dir_name = tempfile.mkdtemp()  # not cleaned up
         module_path = pathlib.Path(dir_name) / self.compiled.module.__name__
-        module_path.with_suffix('.c').write_text(self.compiled.source, 'utf-8')
+        if self.compiled.source is not None and self.compiled.source_ext is not None:
+            module_path.with_suffix(f'.{self.compiled.source_ext}').write_text(
+                self.compiled.source,
+                'utf-8',
+             )
         path_html = module_path.with_suffix('.html')
         path_html.write_text(self.compiled.html, 'utf-8')
         webbrowser.open_new_tab(str(path_html.as_uri()))
         return dir_name
 
     # Method for pretty printing (showing types)
     def __repr__(self):
```

### Comparing `cycept-0.0.2/cycept/core.py` & `cycept-0.0.3/cycept/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -78,14 +78,20 @@
 
 
             silent: bool
                 Set to False to display compilation messages.
                 Default value is True.
 
 
+            c_lang: str
+                Set this to 'c' or 'c++' to select the language to which the
+                Python function will be transpiled.
+                Default value is 'c'.
+
+
             html: bool
                 Set to True to produce HTML annotations of the compiled code.
                 View the HTMl using func.__cycept__().
                 Default value is False.
 
 
             checks: bool
@@ -131,65 +137,37 @@
                 passing them as memoryviews instead of NumPy arrays may not
                 work. To be safe, all memoryview variables are thus converted
                 back to NumPy arrays before used as arguments. Set this option
                 to False to prevent the conversion back to NumPy arrays.
                 Default value is True.
 
 
-            directives: None | dict
+            directives: dict[str, bool]
                 Allows for adding Cython directives to the transpiled
                 function, typically in order to achieve further speedup.
                 To e.g. disable boundschecking of indexing operations:
 
                     @jit(directives={'boundscheck': False})
 
                 You can read about the different directives here:
                 https://cython.readthedocs.io/en/latest/src/userguide/source_files_and_compilation.html#compiler-directives
 
 
-            optimizations: None | str | list |  dict | int | bool
-                Specifies which optimizations to use with the C compiler
-                (given as CFLAGS).
-                If not provided or None, default (aggressive) optimizations
-                are used. One or more optimizations can be given as a str
-                or list of strs, overwriting the defaults, e.g.
-
-                    @jit(optimizations='-O2')
-
-                If not supplied, default optimizations include
-                    * -O3
-                    * -ffast-math
-                    * -march=native
-                To remove e.g. -ffast-math while keeping the remaining
-                default optimizations, use
-
-                    @jit(optimizations={'-ffast-math': False})
-
-                If the value within the dict is True rather than False,
-                the given optimization is added on top of the default
-                optimizations rather than being removed.
-
-                Specifying the optimizations argument as an int 'n'
-                is equivalent to passing just the overall optimization level
-                (which disables all defaults):
-
-                    @jit(optimizations=n)  # equivalent to the below
-                    @jit(optimizations=f'-O{n}')
+            optimizations: dict[str, bool]
+                Specifies which compiler optimizations to enable/disable.
+                Cycept defines the following optimizations, here written with
+                their GCC equivalent to their right:
+                    * base: -O3 -funroll-loops
+                    * fastmath: -ffast-math
+                    * native: -march=native
+                To disable e.g. fastmath, use
 
-                If the optimizations argument is given as a bool,
-                all optimizations are enabled/disabled. That is,
+                    @jit(optimizations={'fastmath': False})
 
-                    @jit(optimizations=True)
-
-                is equivalent to not passing the optimizations argument
-                at all, making use of the defaults. Using
-
-                    @jit(optimizations=False)
-
-                replaces all of the default optimizations with -O0.
+                The default value for all optimizations is True.
 
 
             integral: type | str
                 By default, Python ints are replaced with cython.Py_ssize_t.
                 These are not fully equivalent: while cython.Py_ssize_t is
                 typically 64-bit, Python ints are unbounded. If you prefer
                 to e.g. use 32-bit ints, set this option to e.g. np.int32:
@@ -275,14 +253,15 @@
     func,
     wrapper,
     args,
     kwargs,
     *,
     compile=True,
     silent=True,
+    c_lang=None,
     html=False,
     checks=False,
     clike=False,
     array_args=True,
     directives=None,
     optimizations=None,
     integral=None,
@@ -320,16 +299,15 @@
     result = record_locals(call)
     # Make sure that NumPy arrays are treated as such when necessary
     call.protect_arrays(array_args)
     # Convert Python function source into Cython module source
     directives = get_directives(directives, checks, clike)
     call.to_cython(directives)
     # Cythonize and compile
-    optimizations = get_optimizations(optimizations)
-    time_compile = call.compile(optimizations, html, silent)
+    time_compile = call.compile(optimizations, c_lang, html, silent)
     # Store the function call object on the wrapper function
     wrapper.__cycept__[call.arguments_types] = call
     # End and store time measurements
     toc = time.perf_counter()
     time_total = toc - tic
     call.time = call.Time(time_compile, time_total)
     if not silent:
@@ -341,22 +319,33 @@
 
 # Function used to fetch FunctionCall instance from the global
 # cache or instantiating a new one if not found in the cache.
 def fetch_function_call(func, args=None, kwargs=None):
     if isinstance(func, int):
         # Called with function call hash
         return cache[func]
+    # Fast lookup if called with the same objects as last time
+    ids = (
+        id(func),
+        *(id(arg) for arg in args),
+        *kwargs.keys(),
+        *(id(kwarg) for kwarg in kwargs.values()),
+    )
+    loot = cache.get('last')
+    if loot is not None and loot[1] == ids:
+        return loot[0]
     # We need to instantiate a fresh instance to obtain the hash
     call = FunctionCall(func, args, kwargs)
     call_cached = cache.get(call.hash)
     if call_cached is not None:
         # Found in cache. Disregard the freshly created instance.
         return call_cached
     # Not found in cache. Cache and return the freshly created instance.
     cache[call.hash] = call
+    cache['last'] = call, ids  # special additional store
     return call
 cache = {}
 
 
 # Function for setting up Cython directives
 def get_directives(directives, checks, clike):
     def set_directive(directives, directive, val):
@@ -385,52 +374,14 @@
             warnings.warn(
                 f'Cython directive {directive!r} does not seem to exist',
                 RuntimeWarning,
             )
     return directives
 
 
-# Function for setting up compiler optimizations (CFLAGS)
-def get_optimizations(optimizations):
-    get_defaults = lambda: optimizations_default.copy()
-    if optimizations is None:
-        # No optimizations provided. Use defaults.
-        optimizations = get_defaults()
-    elif isinstance(optimizations, (bool, int)):
-        # Enable or disable all optimizations
-        if optimizations is True:
-            optimizations = get_defaults()
-        else:
-            level = abs(int(optimizations))
-            optimizations = [f'-O{level}']
-    elif isinstance(optimizations, str):
-        # Transform str of optimizations to list
-        optimizations = optimizations.split(' ')
-    elif isinstance(optimizations, dict):
-        # Use defaults with amendments
-        optimizations_ammended = get_defaults()
-        for optimization, enable in optimizations.items():
-            if enable and optimization not in optimizations_ammended:
-                optimizations_ammended.append(optimization)
-            elif not enable and optimization in optimizations_ammended:
-                optimizations_ammended.remove(optimization)
-        optimizations = optimizations_ammended
-    else:
-        # Use supplied optimizations as is
-        optimizations = list(optimizations)
-    return optimizations
-optimizations_default = [
-    '-DNDEBUG',
-    '-O3',
-    '-funroll-loops',
-    '-ffast-math',
-    '-march=native',
-]
-
-
 # Function for extracting the Python/NumPy type off of a value
 def get_type(val):
     tp = construct_ndarray_type_info(val)
     if tp is not None:
         return tp
     return type(val)
```

### Comparing `cycept-0.0.2/cycept/tests/test_cycept.py` & `cycept-0.0.3/cycept/tests/test_cycept.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,64 +10,70 @@
 
 def test_pass():
     @jit
     def f():
         pass
     assert f() is None
 
+
 def test_object():
     @jit
     def f(a):
         return a
     a = object()
     assert f(a) is a
 
+
 def test_type_arg():
     @jit
     def f(a):
         pass
     tps = [int, dict]
     for tp in tps:
         f(tp())
     for tp, key in zip(tps, f.__cycept__.keys()):
         assert key[0] is tp
 
+
 def test_type_local():
     @jit
     def f(a):
         b = a
     tps = [float, str]
     for tp in tps:
         f(tp())
     for tp, call in zip(tps, f.__cycept__.values()):
         assert call.locals_types['b'] is tp
 
+
 def test_type_return():
     @jit
     def f(a):
         return a
     tps = [bool, set]
     for tp in tps:
         f(tp())
     for tp, call in zip(tps, f.__cycept__.values()):
         assert call.locals_types['return'] is tp
 
+
 def test_type_cython():
     @jit
     def f(a):
         b = [a]
         return 2*b.pop()
     f(True)
     call = next(iter(f.__cycept__.values()))
     assert call.types == {
         'a': 'cython.bint',
         'b': 'list',
         'return': 'cython.Py_ssize_t',
     }
 
+
 def test_type_array():
     @jit
     def f(a):
         b = a**0.5
         return b + 1j
     f(np.arange(3, dtype=np.int64))
     key = next(iter(f.__cycept__))
@@ -78,66 +84,85 @@
     assert call.locals_types['return'].dtype is np.complex128
     assert call.types == {
         'a': 'cython.longlong[::1]',
         'b': 'cython.double[::1]',
         'return': 'cython.doublecomplex[::1]',
     }
 
+
 def test_type_annotation():
     @jit
     def f(a: int) -> float:
         b : object = [a]
         return 2*b.pop()
     f(True)
     call = next(iter(f.__cycept__.values()))
     assert call.types == {
         'a': 'cython.Py_ssize_t',
         'b': 'object',
         'return': 'cython.double',
     }
 
+
 def test_manual():
     def f(a):
         return 2*a
     g = jit(f)
     assert f(1) == g(1)
     call = next(iter(g.__cycept__.values()))
     assert call.types['return'] == 'cython.Py_ssize_t'
 
+
 def test_lambda():
     def test(f):
         g = jit(f)
         assert f(1) == g(1)
         call = next(iter(g.__cycept__.values()))
         assert call.types['return'] == 'cython.Py_ssize_t'
     f = lambda a: 2*a
     test(f)
     test(lambda a: 2*a)
 
+
 def test_closure():
     @jit
     def f(a):
         def g(a):
             return 2*a
         return 1 + g(a)
     for _ in range(2):
         assert f(3) == 7
 
+
+def test_method():
+    class Adder:
+        def __init__(self, a):
+            self.a = a
+        @jit
+        def f(self, b):
+            return self.a + b
+    a, b = 2, 3
+    adder = Adder(a)
+    for _ in range(2):
+        assert adder.f(b) == 5
+
+
 def test_arg_default():
     @jit
     def f(a, b=3):
         return a + 2*b
     f(1)
     assert f(1) == 7
     assert f(1, 3) == 7
     assert f(1, 5) == 11
     assert f(1, b=5) == 11
     assert f(a=1, b=5) == 11
     assert f(b=5, a=1) == 11
 
+
 def test_arg_posonly():
     @jit
     def f(a, /, b):
         return a + 2*b
     f(1, 3)
     assert f(1, 3) == 7
     assert f(1, b=3) == 7
@@ -145,14 +170,15 @@
     def g(a, /, b=3):
         return a + 2*b
     g(1)
     assert g(1) == 7
     assert g(1, 5) == 11
     assert g(1, b=5) == 11
 
+
 def test_arg_kwonly():
     @jit
     def f(a, *, b):
         return a + 2*b
     f(1, b=3)
     assert f(1, b=3) == 7
     assert f(a=1, b=3) == 7
@@ -161,14 +187,15 @@
     def g(a, *, b=3):
         return a + 2*b
     g(1)
     assert g(1) == 7
     assert g(1, b=5) == 11
     assert g(b=5, a=1) == 11
 
+
 def test_arg_starargs():
     @jit
     def f(a, *args):
         return a + sum(args)
     f(1)
     call = next(iter(f.__cycept__.values()))
     assert call.locals_types['args'] is tuple
@@ -181,14 +208,15 @@
     g()
     call = next(iter(g.__cycept__.values()))
     assert call.locals_types['args'] is tuple
     assert g() == 1
     assert g(2, 3, 4) == 10
     assert g(2, 3, 4, a=0) == 9
 
+
 def test_arg_starstarkwargs():
     @jit
     def f(a, **kwargs):
         return a + kwargs.get('b', 0) + kwargs.get('c', 0)
     f(1)
     call = next(iter(f.__cycept__.values()))
     assert call.locals_types['kwargs'] is dict
@@ -201,161 +229,238 @@
     g()
     call = next(iter(g.__cycept__.values()))
     assert call.locals_types['kwargs'] is dict
     assert g() == 1
     assert g(b=2, c=3) == 6
     assert g(b=2, c=3, a=0) == 5
 
+
 def test_option_none():
     @jit()
     def f():
         pass
     assert f() is None
 
+
 def test_option_compile():
-    for compile in (False, True):
+    for compile in [False, True]:
         @jit(compile=compile)
         def f():
             return cython.compiled
         f()  # to compile
         assert f() is compile
 
+
 def test_option_silent(capfd):
-    for silent in (False, True):
+    for silent in [False, True]:
         @jit(silent=silent)
         def f(a):
             pass
         f(np.linspace(0, 1, 3, dtype=np.float64))
-        out, err = capfd.readouterr()
+        captured = capfd.readouterr()
         if silent:
-            assert out == ''
+            assert captured.out == ''
         else:
-            assert 'Jitting f(a: double[::1])' in out       # Cycept
-            assert 'Compilation time' in out                # Cycept
-            assert 'Compiling' in out                       # Cython
-            assert re.search(r'cycept_module_\d+\.o', out)  # C compiler
+            assert 'Jitting f(a: double[::1])' in captured.out       # Cycept
+            assert 'Compilation time' in captured.out                # Cycept
+            assert 'Compiling' in captured.out                       # Cython
+            assert re.search(r'cycept_module_\d+\.o', captured.out)  # C compiler
+
+
+def test_option_c_lang():
+    for c_lang in [None, 'c', 'c++']:
+        @jit(c_lang=c_lang)
+        def f():
+            pass
+        f()
+        call = next(iter(f.__cycept__.values()))
+        assert re.match('c' + '.'*(c_lang == 'c++'), call.compiled.source_ext)
+        if c_lang == 'c++':
+            assert len(re.findall('template', call.compiled.source))
+
 
 def test_option_html():
-    for html in (False, True):
+    for html in [False, True]:
         @jit(html=html)
         def f():
             a = 1234
             pass
         f()
         html_annotation = f.__cycept__[()].compiled.html
         if html:
             assert '1234' in html_annotation
         else:
             assert html_annotation is None
 
+
 def test_option_checks():
-    for checks in (False, True):
+    for checks in [False, True]:
         @jit(checks=checks)
         def f(a, i):
             return a[i]
         f(np.arange(3), 2)
         source = next(iter(f.__cycept__.values())).source
         deactivated_boundscheck = '@cython.boundscheck(False)' in source
         deactivated_initializedcheck = '@cython.initializedcheck(False)' in source
         assert deactivated_boundscheck is not checks
         assert deactivated_initializedcheck is not checks
 
+
 def test_option_clike():
-    for clike in (False, True):
+    for clike in [False, True]:
         @jit(clike=clike)
         def f(a, b):
             return a//b
         for _ in range(2):  # twice in order to use compiled function
             result = f(-1, 2)
         source = next(iter(f.__cycept__.values())).source
         deactivated_wraparoundcheck = '@cython.wraparound(False)' in source
         deactivated_pydivisioncheck = '@cython.cdivision(True)' in source
         assert deactivated_wraparoundcheck is clike
         assert deactivated_pydivisioncheck is clike
         assert result == (0 if clike else -1)
 
+
 def test_option_array_args():
     def g(a):
         try:
             a *= 2
         except TypeError:
             # Augmented assignment fails for memoryviews
             a[:] = 0
         return a
-    for array_args in (False, True):
+    for array_args in [False, True]:
         @jit(array_args=array_args)
         def f(a):
             return g(a)
         for _ in range(2):  # twice in order to use compiled function
             result = f(np.arange(3))
         assert result.sum() == 6*array_args
 
+
 def test_option_directives():
-    for cdivision in (False, True):
+    for cdivision in [False, True]:
         @jit(directives={'cdivision': cdivision})
         def f(a, b):
             return a//b
         for _ in range(2):  # twice in order to use compiled function
             result = f(-1, 2)
         assert result == (0 if cdivision else -1)
 
-@pytest.mark.skipif(
-    re.search(r'(?<!dar)win', sys.platform.lower()),
-    reason=(
-        'CFLAGS optimizations does not work with MSVC, '
-        'which is probably the compiler used on Windows'
-    ),
-)
+
 def test_option_optimizations(capfd):
-    for level, optimizations in enumerate([False, 1, '-O2', {'-O3': True}]):
-        @jit(optimizations=optimizations, silent=False)
+    for fastmath in [False, True]:
+        @jit(optimizations={'fastmath': fastmath}, silent=False)
         def f():
             pass
         f()
-        out, err = capfd.readouterr()
-        assert f'-O{level}' in out
+        captured = capfd.readouterr()
+        output = captured.out + captured.err
+        if fastmath:
+            assert '-ffast-math' in output or '/fp:fast' in output
+        else:
+            assert '-ffast-math' not in output and '/fp:fast' not in output
+
+
+def test_option_integral():
+    for integral in [None, object, 'int', np.int8, np.int32, np.int64]:
+        @jit(integral=integral)
+        def f(a):
+            return a + 1
+        f(0)
+        if integral in {None, 'int'}:
+            for size in [8, 16, 32, 64, 128]:
+                a = 2**(size - 1) - 1
+                result = f(a)
+                assert result in {-2**(size - 1), a + 1}
+                if result < 0:
+                    break
+            assert result < 0
+        elif integral is object:
+            size = 1024
+            a = 2**(size - 1) - 1
+            assert f(a) == a + 1
+        else:
+            size = 8*integral().itemsize
+            assert f(2**(size - 1) - 1) == -2**(size - 1)
+
+
+def test_option_floating():
+    for floating in [None, 'double', np.float32, np.float64]:
+        @jit(floating=floating)
+        def f(a):
+            return 2*a
+        f(0.0)
+        dtype = floating
+        if dtype in {None, 'double'}:
+            dtype = np.float64
+        a = float(np.finfo(dtype).max)
+        assert f(a) == float('inf')
+        assert f(a/2) == a
+
+
+def test_option_floating_complex():
+    for floating_complex in [None, np.complex64, np.complex128]:
+        @jit(floating_complex=floating_complex)
+        def f(a):
+            return 2*a
+        f(0.0j)
+        dtype = floating_complex
+        if dtype is None:
+            dtype = np.complex128
+        a = float(np.finfo(dtype).max)
+        a -= a*1j
+        result = f(a)
+        assert result.real == +float('inf')
+        assert result.imag == -float('inf')
+        assert f(a/2) == a
+
 
 def test_array_mutability():
     @jit
     def f(a):
         a[0] += 1
     a = np.zeros(3, dtype=int)
     n = 3
     for _ in range(n):
         f(a)
     assert a[0] == n
 
+
 def test_array_operations():
     @jit
     def f(a):
         b = a + 1
         return b
     a = np.zeros(3, dtype=int)
     for _ in range(2):
         b = f(a)
         assert b.sum() == 3
 
+
 def test_array_augmentation():
     @jit
     def f(a):
         a += 1
     a = np.zeros(3, dtype=int)
     for _ in range(2):
         f(a)
     assert a.sum() == 6
 
+
 def test_array_slice_augmentation():
     @jit
     def f(a):
         a[1:] += 1
     a = np.zeros(3, dtype=int)
     for _ in range(2):
         f(a)
     assert a.sum() == 4
 
+
 def test_array_element_augmentation():
     @jit
     def f(a, b):
         a[b] += 1
     a = np.zeros(3, dtype=int)
     b = np.zeros(3, dtype=bool)
     b[2] = True
@@ -365,14 +470,15 @@
     assert (a == [0, 2, 2]).all()
     sourcelengths = [
         len(call.compiled.source)
         for call in f.__cycept__.values()
     ]
     assert sourcelengths[0] < sourcelengths[1]
 
+
 def test_array_comparison():
     @jit
     def f(a):
         b = a < 2
         return a >= b[0]
     a = np.arange(3, dtype=int)
     for _ in range(2):
```

### Comparing `cycept-0.0.2/cycept.egg-info/PKG-INFO` & `cycept-0.0.3/cycept.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycept
-Version: 0.0.2
+Version: 0.0.3
 Summary: Effortless just-in-time compilation of Python functions, powered by Cython
 Author-email: Jeppe Dakin <jeppe_dakin@hotmail.com>
 Project-URL: Download, https://pypi.python.org/pypi/cycept
 Project-URL: Changelog, https://github.com/jmd-dk/cycept/blob/main/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/jmd-dk/cycept/issues
 Project-URL: Source code, https://github.com/jmd-dk/cycept
 Classifier: Intended Audience :: Developers
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Cython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: repl
 Provides-Extra: test
 License-File: LICENSE
 
 # Cycept
 Effortless just-in-time compilation of Python functions,
 powered by [Cython](https://cython.org/).
 
@@ -38,17 +39,22 @@
 python -m pip install cycept
 ```
 
 Cycept requires Python 3.9 or later.
 
 To run Cycept a C compiler needs to be installed on the system.
 
-* On **Linux** you may install [GCC](https://gcc.gnu.org/) (Debian-like distros: `sudo apt install build-essential`).
-* On **macOS** you may install [Xcode](https://developer.apple.com/xcode/).
-* On **Windows** you may install [MSVC](https://visualstudio.microsoft.com/visual-cpp-build-tools/).
+* On **Linux** you may install [GCC](https://gcc.gnu.org/)
+  (Debian-like distros: `sudo apt install build-essential`).
+* On **macOS** you may install [Clang](https://clang.llvm.org/)
+  (available through [Xcode](https://developer.apple.com/xcode/)).
+* On **Windows** you may install
+  [MSVC](https://en.wikipedia.org/wiki/Microsoft_Visual_C%2B%2B)
+  (available through
+  [Microsoft C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/)).
 
 
 ## Quick demo
 ```python
 """Comparison of Python function JITs
 
 Below we implement the sample function sum((a - b)**2) where a and b
@@ -154,26 +160,36 @@
 
 See the help info on `cycept.jit` for optional arguments:
 ```bash
 python -c 'import cycept; help(cycept.jit)'
 ```
 
 
-## Test suite
+## Tests
 The code contains a unit test suite which may be run as
-```
-python -c "import cycept; cycept.test()"
+```bash
+python -c "import cycept; cycept.test('cycept')"
 ```
 This requires [pytest](https://docs.pytest.org/) to be installed
 (`python -m pip install pytest`).
 
+If `cycept.test()` is called without an argument it will further run a
+performance test suite, though showing only whether each test passes or not.
+To display the actual performance benchmarks, run the performance test suite
+by itself using
+```bash
+python -c "import cycept; cycept.bench(show_func=True)"
+```
+
 
 ## What's up with the name?
 'Cycept' is an amalgamation of '[Cython](https://cython.org/)' and
 '[CO*N*CEPT](https://github.com/jmd-dk/concept)', the latter of which is a
 cosmological simulation code that makes heavy use of code transformation,
 both custom and through Cython. As the author of both projects, Cycept is my
 attempt to extract some of the code transformation ideas buried within
 CO*N*CEPT, making them available within an easy-to-use library.
 Though no code is shared between the projects, in many respects Cycept
 can be considered a spiritual descendant of CO*N*CEPT.
+Furthermore, 'Cy*cept*' has a nice in*cept*ion ring to it,
+which seems fitting for a piece of code that generates code.
```

### Comparing `cycept-0.0.2/pyproject.toml` & `cycept-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = [
-    "setuptools>=61.0",
+    "setuptools >= 65.6.0, < 68",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cycept"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     {name="Jeppe Dakin", email="jeppe_dakin@hotmail.com"},
 ]
 description = "Effortless just-in-time compilation of Python functions, powered by Cython"
 readme = "README.md"
 requires-python = ">= 3.9"
 dependencies = [
-    "cython >= 3.0.0b1",
-    "numpy >= 1.20",
-    "dill >= 0.3",
-    "tomli >= 1.1.0; python_version < '3.11'",
+    "cython >= 3.0.0b1, < 3.1",
+    "numpy >= 1.21.0, < 1.25",
+    "setuptools >= 65.6.0, < 68",
+    "tomli >= 1.1.0, < 2.1; python_version < '3.11'",
 ]
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
@@ -40,16 +40,20 @@
 [project.urls]
 "Download" = "https://pypi.python.org/pypi/cycept"
 "Changelog" = "https://github.com/jmd-dk/cycept/blob/main/CHANGELOG.md"
 "Bug Tracker" = "https://github.com/jmd-dk/cycept/issues"
 "Source code" = "https://github.com/jmd-dk/cycept"
 
 [project.optional-dependencies]
+repl = [
+    "dill >= 0.2.0, < 0.4",
+]
 test = [
-    "pytest ~= 7.3",
+    "pytest >= 7.3.0, < 7.4",
+    "numba >= 0.57.0rc1, < 0.58",
 ]
 
 [tool.setuptools]
 packages = [
     "cycept", "cycept.tests",
 ]
```

