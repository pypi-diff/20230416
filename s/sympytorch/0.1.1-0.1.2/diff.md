# Comparing `tmp/sympytorch-0.1.1.tar.gz` & `tmp/sympytorch-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sympytorch-0.1.1.tar", last modified: Mon May 31 20:42:14 2021, max compression
+gzip compressed data, was "sympytorch-0.1.2.tar", last modified: Sun Apr 16 17:52:13 2023, max compression
```

## Comparing `sympytorch-0.1.1.tar` & `sympytorch-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 kidger   (22469) kidger   (22469)        0 2021-05-31 20:42:14.000000 sympytorch-0.1.1/
--rw-rw-r--   0 kidger   (22469) kidger   (22469)    11357 2021-02-23 22:15:35.000000 sympytorch-0.1.1/LICENSE
--rw-rw-r--   0 kidger   (22469) kidger   (22469)       28 2021-05-31 20:29:06.000000 sympytorch-0.1.1/MANIFEST.in
--rw-rw-r--   0 kidger   (22469) kidger   (22469)     3612 2021-05-31 20:42:14.000000 sympytorch-0.1.1/PKG-INFO
--rw-rw-r--   0 kidger   (22469) kidger   (22469)     2167 2021-05-31 20:24:55.000000 sympytorch-0.1.1/README.md
--rw-rw-r--   0 kidger   (22469) kidger   (22469)       38 2021-05-31 20:42:14.000000 sympytorch-0.1.1/setup.cfg
--rw-rw-r--   0 kidger   (22469) kidger   (22469)     2136 2021-05-31 20:39:34.000000 sympytorch-0.1.1/setup.py
-drwxrwxr-x   0 kidger   (22469) kidger   (22469)        0 2021-05-31 20:42:14.000000 sympytorch-0.1.1/sympytorch/
--rw-rw-r--   0 kidger   (22469) kidger   (22469)      101 2021-05-31 20:24:55.000000 sympytorch-0.1.1/sympytorch/__init__.py
--rw-rw-r--   0 kidger   (22469) kidger   (22469)      851 2021-05-31 20:24:55.000000 sympytorch-0.1.1/sympytorch/hide_floats_m.py
--rw-rw-r--   0 kidger   (22469) kidger   (22469)     5603 2021-05-31 20:24:55.000000 sympytorch-0.1.1/sympytorch/sympy_module.py
-drwxrwxr-x   0 kidger   (22469) kidger   (22469)        0 2021-05-31 20:42:14.000000 sympytorch-0.1.1/sympytorch.egg-info/
--rw-rw-r--   0 kidger   (22469) kidger   (22469)     3612 2021-05-31 20:42:13.000000 sympytorch-0.1.1/sympytorch.egg-info/PKG-INFO
--rw-rw-r--   0 kidger   (22469) kidger   (22469)      318 2021-05-31 20:42:13.000000 sympytorch-0.1.1/sympytorch.egg-info/SOURCES.txt
--rw-rw-r--   0 kidger   (22469) kidger   (22469)        1 2021-05-31 20:42:13.000000 sympytorch-0.1.1/sympytorch.egg-info/dependency_links.txt
--rw-rw-r--   0 kidger   (22469) kidger   (22469)        1 2021-02-23 22:34:13.000000 sympytorch-0.1.1/sympytorch.egg-info/not-zip-safe
--rw-rw-r--   0 kidger   (22469) kidger   (22469)       26 2021-05-31 20:42:13.000000 sympytorch-0.1.1/sympytorch.egg-info/requires.txt
--rw-rw-r--   0 kidger   (22469) kidger   (22469)       11 2021-05-31 20:42:13.000000 sympytorch-0.1.1/sympytorch.egg-info/top_level.txt
+drwxr-xr-x   0 kidger    (1000) kidger    (1000)        0 2023-04-16 17:52:13.898434 sympytorch-0.1.2/
+-rw-r--r--   0 kidger    (1000) kidger    (1000)    11357 2023-04-16 17:42:44.000000 sympytorch-0.1.2/LICENSE
+-rw-r--r--   0 kidger    (1000) kidger    (1000)       28 2023-04-16 17:42:44.000000 sympytorch-0.1.2/MANIFEST.in
+-rw-r--r--   0 kidger    (1000) kidger    (1000)     3227 2023-04-16 17:52:13.898434 sympytorch-0.1.2/PKG-INFO
+-rw-r--r--   0 kidger    (1000) kidger    (1000)     2223 2023-04-16 17:42:44.000000 sympytorch-0.1.2/README.md
+-rw-r--r--   0 kidger    (1000) kidger    (1000)       38 2023-04-16 17:52:13.898434 sympytorch-0.1.2/setup.cfg
+-rw-r--r--   0 kidger    (1000) kidger    (1000)     2136 2023-04-16 17:42:44.000000 sympytorch-0.1.2/setup.py
+drwxr-xr-x   0 kidger    (1000) kidger    (1000)        0 2023-04-16 17:52:13.896433 sympytorch-0.1.2/sympytorch/
+-rw-r--r--   0 kidger    (1000) kidger    (1000)      101 2023-04-16 17:42:44.000000 sympytorch-0.1.2/sympytorch/__init__.py
+-rw-r--r--   0 kidger    (1000) kidger    (1000)      851 2023-04-16 17:42:44.000000 sympytorch-0.1.2/sympytorch/hide_floats_m.py
+-rw-r--r--   0 kidger    (1000) kidger    (1000)     6501 2023-04-16 17:50:40.000000 sympytorch-0.1.2/sympytorch/sympy_module.py
+drwxr-xr-x   0 kidger    (1000) kidger    (1000)        0 2023-04-16 17:52:13.897434 sympytorch-0.1.2/sympytorch.egg-info/
+-rw-r--r--   0 kidger    (1000) kidger    (1000)     3227 2023-04-16 17:52:13.000000 sympytorch-0.1.2/sympytorch.egg-info/PKG-INFO
+-rw-r--r--   0 kidger    (1000) kidger    (1000)      318 2023-04-16 17:52:13.000000 sympytorch-0.1.2/sympytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 kidger    (1000) kidger    (1000)        1 2023-04-16 17:52:13.000000 sympytorch-0.1.2/sympytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 kidger    (1000) kidger    (1000)        1 2023-04-16 17:43:02.000000 sympytorch-0.1.2/sympytorch.egg-info/not-zip-safe
+-rw-r--r--   0 kidger    (1000) kidger    (1000)       26 2023-04-16 17:52:13.000000 sympytorch-0.1.2/sympytorch.egg-info/requires.txt
+-rw-r--r--   0 kidger    (1000) kidger    (1000)       11 2023-04-16 17:52:13.000000 sympytorch-0.1.2/sympytorch.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sympytorch-0.1.1/LICENSE` & `sympytorch-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sympytorch-0.1.1/PKG-INFO` & `sympytorch-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,82 @@
 Metadata-Version: 2.1
 Name: sympytorch
-Version: 0.1.1
+Version: 0.1.2
 Summary: Turning SymPy expressions into PyTorch modules.
 Home-page: https://github.com/patrick-kidger/sympytorch
 Author: Patrick Kidger
 Author-email: contact@kidger.site
 Maintainer: Patrick Kidger
 Maintainer-email: contact@kidger.site
 License: Apache-2.0
-Description: # sympytorch
-        
-        A micro-library as a convenience for turning SymPy expressions into PyTorch Modules.
-        
-        SymPy floats (optionally) become trainable parameters. SymPy symbols are inputs to the Module.
-        
-        ## Installation
-        
-        ```bash
-        pip install git+https://github.com/patrick-kidger/sympytorch.git
-        ```
-        
-        ## Example
-        
-        ```python
-        import sympy, torch, sympytorch
-        
-        x = sympy.symbols('x_name')
-        cosx = 1.0 * sympy.cos(x)
-        sinx = 2.0 * sympy.sin(x)
-        mod = sympytorch.SymPyModule(expressions=[cosx, sinx])
-        
-        x_ = torch.rand(3)
-        out = mod(x_name=x_)  # out has shape (3, 2)
-        
-        assert torch.equal(out[:, 0], x_.cos())
-        assert torch.equal(out[:, 1], 2 * x_.sin())
-        assert out.requires_grad  # from the two Parameters initialised as 1.0 and 2.0
-        assert {x.item() for x in mod.parameters()} == {1.0, 2.0}
-        ```
-        
-        ## API
-        
-        ```python
-        sympytorch.SymPyModule(*, expressions, extra_funcs=None)
-        ```
-        Where:
-        - `expressions` is a list of SymPy expressions.
-        - `extra_funcs` is a dictionary mapping from custom `sympy.Function`s to their PyTorch implementation. Defaults to no extra functions.
-        
-        Instances of `SymPyModule` can be called, passing the values of the symbols as in the above example.
-        
-        `SymPyModule` has a method `.sympy()`, which returns the corresponding list of SymPy expressions. (Which may not be the same as the expressions it was initialised with, if the values of its Parameters have been changed, i.e. have been learnt.)
-        
-        Wrapping floats in `sympy.UnevaluatedExpr` will cause them not to be trained, by registering them as buffers rather than parameters.
-        
-        ```python
-        sympytorch.hide_floats(expression)
-        ```
-        As a convenience, `hide_floats` will take an expression and return a new expression with every float wrapped in a `sympy.UnevaluatedExpr`, so that it is interpreted as a buffer rather than a parameter.
-        
-        ## Extensions
-        
-        Not every PyTorch or SymPy operation is supported -- just the ones that I found I've needed! There's a dictionary [here](./sympytorch/sympy_module.py#L12) that lists the supported operations. Feel free to submit PRs for any extra operations you think should be in by default. You can also use the `extra_funcs` argument to specify extra functions, including custom functions.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align="center">sympytorch</h1>
+
+Turn SymPy expressions into PyTorch Modules.
+
+SymPy floats (optionally) become trainable parameters. SymPy symbols are inputs to the Module.
+
+Optimise your symbolic expressions via gradient descent!
+
+## Installation
+
+```bash
+pip install sympytorch
+```
+Requires Python 3.7+ and PyTorch 1.6.0+ and SymPy 1.7.1+.
+
+## Example
+
+```python
+import sympy, torch, sympytorch
+
+x = sympy.symbols('x_name')
+cosx = 1.0 * sympy.cos(x)
+sinx = 2.0 * sympy.sin(x)
+mod = sympytorch.SymPyModule(expressions=[cosx, sinx])
+
+x_ = torch.rand(3)
+out = mod(x_name=x_)  # out has shape (3, 2)
+
+assert torch.equal(out[:, 0], x_.cos())
+assert torch.equal(out[:, 1], 2 * x_.sin())
+assert out.requires_grad  # from the two Parameters initialised as 1.0 and 2.0
+assert {x.item() for x in mod.parameters()} == {1.0, 2.0}
+```
+
+## API
+
+```python
+sympytorch.SymPyModule(*, expressions, extra_funcs=None)
+```
+Where:
+- `expressions` is a list of SymPy expressions.
+- `extra_funcs` is a dictionary mapping from custom `sympy.Function`s to their PyTorch implementation. Defaults to no extra functions.
+
+Instances of `SymPyModule` can be called, passing the values of the symbols as in the above example.
+
+`SymPyModule` has a method `.sympy()`, which returns the corresponding list of SymPy expressions. (Which may not be the same as the expressions it was initialised with, if the values of its Parameters have been changed, i.e. have been learnt.)
+
+Wrapping floats in `sympy.UnevaluatedExpr` will cause them not to be trained, by registering them as buffers rather than parameters.
+
+```python
+sympytorch.hide_floats(expression)
+```
+As a convenience, `hide_floats` will take an expression and return a new expression with every float wrapped in a `sympy.UnevaluatedExpr`, so that it is interpreted as a buffer rather than a parameter.
+
+## Extensions
+
+Not every PyTorch or SymPy operation is supported -- just the ones that I found I've needed! There's a dictionary [here](./sympytorch/sympy_module.py#L12) that lists the supported operations. Feel free to submit PRs for any extra operations you think should be in by default. You can also use the `extra_funcs` argument to specify extra functions, including custom functions.
```

### Comparing `sympytorch-0.1.1/README.md` & `sympytorch-0.1.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-# sympytorch
+<h1 align="center">sympytorch</h1>
 
-A micro-library as a convenience for turning SymPy expressions into PyTorch Modules.
+Turn SymPy expressions into PyTorch Modules.
 
 SymPy floats (optionally) become trainable parameters. SymPy symbols are inputs to the Module.
 
+Optimise your symbolic expressions via gradient descent!
+
 ## Installation
 
 ```bash
-pip install git+https://github.com/patrick-kidger/sympytorch.git
+pip install sympytorch
 ```
+Requires Python 3.7+ and PyTorch 1.6.0+ and SymPy 1.7.1+.
 
 ## Example
 
 ```python
 import sympy, torch, sympytorch
 
 x = sympy.symbols('x_name')
```

### Comparing `sympytorch-0.1.1/setup.py` & `sympytorch-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `sympytorch-0.1.1/sympytorch/hide_floats_m.py` & `sympytorch-0.1.2/sympytorch/hide_floats_m.py`

 * *Files identical despite different names*

### Comparing `sympytorch-0.1.1/sympytorch/sympy_module.py` & `sympytorch-0.1.2/sympytorch/sympy_module.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 
 def _reduce(fn):
     def fn_(*args):
         return ft.reduce(fn, args)
     return fn_
 
+def _I(*args):
+    return torch.tensor(1j)
 
 _global_func_lookup = {
     sympy.Mul: _reduce(torch.mul),
     sympy.Add: _reduce(torch.add),
     sympy.div: torch.div,
     sympy.Abs: torch.abs,
     sympy.sign: torch.sign,
@@ -56,39 +58,45 @@
     sympy.Min: torch.min,
     # Matrices
     sympy.MatAdd: torch.add,
     sympy.HadamardProduct: torch.mul,
     sympy.Trace: torch.trace,
     # Note: May raise error for integer matrices.
     sympy.Determinant: torch.det,
+    sympy.core.numbers.ImaginaryUnit: _I,
+    sympy.conjugate: torch.conj,
+
 }
 
 
 class _Node(torch.nn.Module):
     def __init__(self, *, expr, _memodict, _func_lookup, **kwargs):
         super().__init__(**kwargs)
 
         self._sympy_func = expr.func
 
         if issubclass(expr.func, sympy.Float):
             self._value = torch.nn.Parameter(torch.tensor(float(expr)))
             self._torch_func = lambda: self._value
             self._args = ()
+        elif issubclass(expr.func, sympy.Integer):
+            self._value = int(expr)
+            self._torch_func = lambda: self._value
+            self._args = ()
+        elif issubclass(expr.func, sympy.Rational):
+            self.register_buffer('_numerator', torch.tensor(expr.p, dtype=torch.get_default_dtype()))
+            self.register_buffer('_denominator', torch.tensor(expr.q, dtype=torch.get_default_dtype()))
+            self._torch_func = lambda: self._numerator / self._denominator
+            self._args = ()
         elif issubclass(expr.func, sympy.UnevaluatedExpr):
             if len(expr.args) != 1 or not issubclass(expr.args[0].func, sympy.Float):
                 raise ValueError("UnevaluatedExpr should only be used to wrap floats.")
             self.register_buffer('_value', torch.tensor(float(expr.args[0])))
             self._torch_func = lambda: self._value
             self._args = ()
-        elif issubclass(expr.func, sympy.Integer):
-            # Can get here if expr is one of the Integer special cases,
-            # e.g. NegativeOne
-            self._value = int(expr)
-            self._torch_func = lambda: self._value
-            self._args = ()
         elif issubclass(expr.func, sympy.Symbol):
             self._name = expr.name
             self._torch_func = lambda value: value
             self._args = ((lambda memodict: memodict[expr.name]),)
         else:
             self._torch_func = _func_lookup[expr.func]
             args = []
@@ -102,18 +110,27 @@
             self._args = torch.nn.ModuleList(args)
 
     def sympy(self, _memodict):
         if issubclass(self._sympy_func, sympy.Float):
             return self._sympy_func(self._value.item())
         elif issubclass(self._sympy_func, sympy.UnevaluatedExpr):
             return self._sympy_func(self._value.item())
+        elif issubclass(self._sympy_func, (type(sympy.S.NegativeOne), type(sympy.S.One), type(sympy.S.Zero))):
+            return self._sympy_func()
         elif issubclass(self._sympy_func, sympy.Integer):
             return self._sympy_func(self._value)
+        elif issubclass(self._sympy_func, sympy.Rational):
+            if issubclass(self._sympy_func, type(sympy.S.Half)):
+                return sympy.S.Half
+            else:
+                return self._sympy_func(self._numerator.item(), self._denominator.item())
         elif issubclass(self._sympy_func, sympy.Symbol):
             return self._sympy_func(self._name)
+        elif issubclass(self._sympy_func, sympy.core.numbers.ImaginaryUnit):
+            return sympy.I
         else:
             if issubclass(self._sympy_func, (sympy.Min, sympy.Max)):
                 evaluate = False
             else:
                 evaluate = True
             args = []
             for arg in self._args:
```

### Comparing `sympytorch-0.1.1/sympytorch.egg-info/PKG-INFO` & `sympytorch-0.1.2/sympytorch.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,82 @@
 Metadata-Version: 2.1
 Name: sympytorch
-Version: 0.1.1
+Version: 0.1.2
 Summary: Turning SymPy expressions into PyTorch modules.
 Home-page: https://github.com/patrick-kidger/sympytorch
 Author: Patrick Kidger
 Author-email: contact@kidger.site
 Maintainer: Patrick Kidger
 Maintainer-email: contact@kidger.site
 License: Apache-2.0
-Description: # sympytorch
-        
-        A micro-library as a convenience for turning SymPy expressions into PyTorch Modules.
-        
-        SymPy floats (optionally) become trainable parameters. SymPy symbols are inputs to the Module.
-        
-        ## Installation
-        
-        ```bash
-        pip install git+https://github.com/patrick-kidger/sympytorch.git
-        ```
-        
-        ## Example
-        
-        ```python
-        import sympy, torch, sympytorch
-        
-        x = sympy.symbols('x_name')
-        cosx = 1.0 * sympy.cos(x)
-        sinx = 2.0 * sympy.sin(x)
-        mod = sympytorch.SymPyModule(expressions=[cosx, sinx])
-        
-        x_ = torch.rand(3)
-        out = mod(x_name=x_)  # out has shape (3, 2)
-        
-        assert torch.equal(out[:, 0], x_.cos())
-        assert torch.equal(out[:, 1], 2 * x_.sin())
-        assert out.requires_grad  # from the two Parameters initialised as 1.0 and 2.0
-        assert {x.item() for x in mod.parameters()} == {1.0, 2.0}
-        ```
-        
-        ## API
-        
-        ```python
-        sympytorch.SymPyModule(*, expressions, extra_funcs=None)
-        ```
-        Where:
-        - `expressions` is a list of SymPy expressions.
-        - `extra_funcs` is a dictionary mapping from custom `sympy.Function`s to their PyTorch implementation. Defaults to no extra functions.
-        
-        Instances of `SymPyModule` can be called, passing the values of the symbols as in the above example.
-        
-        `SymPyModule` has a method `.sympy()`, which returns the corresponding list of SymPy expressions. (Which may not be the same as the expressions it was initialised with, if the values of its Parameters have been changed, i.e. have been learnt.)
-        
-        Wrapping floats in `sympy.UnevaluatedExpr` will cause them not to be trained, by registering them as buffers rather than parameters.
-        
-        ```python
-        sympytorch.hide_floats(expression)
-        ```
-        As a convenience, `hide_floats` will take an expression and return a new expression with every float wrapped in a `sympy.UnevaluatedExpr`, so that it is interpreted as a buffer rather than a parameter.
-        
-        ## Extensions
-        
-        Not every PyTorch or SymPy operation is supported -- just the ones that I found I've needed! There's a dictionary [here](./sympytorch/sympy_module.py#L12) that lists the supported operations. Feel free to submit PRs for any extra operations you think should be in by default. You can also use the `extra_funcs` argument to specify extra functions, including custom functions.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align="center">sympytorch</h1>
+
+Turn SymPy expressions into PyTorch Modules.
+
+SymPy floats (optionally) become trainable parameters. SymPy symbols are inputs to the Module.
+
+Optimise your symbolic expressions via gradient descent!
+
+## Installation
+
+```bash
+pip install sympytorch
+```
+Requires Python 3.7+ and PyTorch 1.6.0+ and SymPy 1.7.1+.
+
+## Example
+
+```python
+import sympy, torch, sympytorch
+
+x = sympy.symbols('x_name')
+cosx = 1.0 * sympy.cos(x)
+sinx = 2.0 * sympy.sin(x)
+mod = sympytorch.SymPyModule(expressions=[cosx, sinx])
+
+x_ = torch.rand(3)
+out = mod(x_name=x_)  # out has shape (3, 2)
+
+assert torch.equal(out[:, 0], x_.cos())
+assert torch.equal(out[:, 1], 2 * x_.sin())
+assert out.requires_grad  # from the two Parameters initialised as 1.0 and 2.0
+assert {x.item() for x in mod.parameters()} == {1.0, 2.0}
+```
+
+## API
+
+```python
+sympytorch.SymPyModule(*, expressions, extra_funcs=None)
+```
+Where:
+- `expressions` is a list of SymPy expressions.
+- `extra_funcs` is a dictionary mapping from custom `sympy.Function`s to their PyTorch implementation. Defaults to no extra functions.
+
+Instances of `SymPyModule` can be called, passing the values of the symbols as in the above example.
+
+`SymPyModule` has a method `.sympy()`, which returns the corresponding list of SymPy expressions. (Which may not be the same as the expressions it was initialised with, if the values of its Parameters have been changed, i.e. have been learnt.)
+
+Wrapping floats in `sympy.UnevaluatedExpr` will cause them not to be trained, by registering them as buffers rather than parameters.
+
+```python
+sympytorch.hide_floats(expression)
+```
+As a convenience, `hide_floats` will take an expression and return a new expression with every float wrapped in a `sympy.UnevaluatedExpr`, so that it is interpreted as a buffer rather than a parameter.
+
+## Extensions
+
+Not every PyTorch or SymPy operation is supported -- just the ones that I found I've needed! There's a dictionary [here](./sympytorch/sympy_module.py#L12) that lists the supported operations. Feel free to submit PRs for any extra operations you think should be in by default. You can also use the `extra_funcs` argument to specify extra functions, including custom functions.
```

