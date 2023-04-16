# Comparing `tmp/lazyfunc-0.1.0.tar.gz` & `tmp/lazyfunc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyfunc-0.1.0.tar", last modified: Sun Jan 22 17:44:18 2023, max compression
+gzip compressed data, was "lazyfunc-0.2.0.tar", last modified: Sun Apr 16 19:22:43 2023, max compression
```

## Comparing `lazyfunc-0.1.0.tar` & `lazyfunc-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:44:18.537053 lazyfunc-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:44:18.533053 lazyfunc-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:44:18.537053 lazyfunc-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-01-22 17:44:08.000000 lazyfunc-0.1.0/.github/workflows/deploy_docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-01-22 17:44:08.000000 lazyfunc-0.1.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-01-22 17:44:08.000000 lazyfunc-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-01-22 17:44:08.000000 lazyfunc-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-01-22 17:44:08.000000 lazyfunc-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-01-22 17:44:18.537053 lazyfunc-0.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:44:18.537053 lazyfunc-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-01-22 17:44:08.000000 lazyfunc-0.1.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-01-22 17:44:08.000000 lazyfunc-0.1.0/docs/explanation.md
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-22 17:44:08.000000 lazyfunc-0.1.0/docs/reference.md
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-01-22 17:44:08.000000 lazyfunc-0.1.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-01-22 17:44:08.000000 lazyfunc-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-22 17:44:18.537053 lazyfunc-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:44:18.537053 lazyfunc-0.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-22 17:44:18.000000 lazyfunc-0.1.0/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:44:18.537053 lazyfunc-0.1.0/src/lazyfunc/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-01-22 17:44:08.000000 lazyfunc-0.1.0/src/lazyfunc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-01-22 17:44:08.000000 lazyfunc-0.1.0/src/lazyfunc/lazy_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-01-22 17:44:08.000000 lazyfunc-0.1.0/src/lazyfunc/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-01-22 17:44:08.000000 lazyfunc-0.1.0/src/lazyfunc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:44:18.537053 lazyfunc-0.1.0/src/lazyfunc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-01-22 17:44:18.000000 lazyfunc-0.1.0/src/lazyfunc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-01-22 17:44:18.000000 lazyfunc-0.1.0/src/lazyfunc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-22 17:44:18.000000 lazyfunc-0.1.0/src/lazyfunc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-22 17:44:18.000000 lazyfunc-0.1.0/src/lazyfunc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-22 17:44:18.000000 lazyfunc-0.1.0/src/lazyfunc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:44:18.537053 lazyfunc-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-01-22 17:44:08.000000 lazyfunc-0.1.0/tests/test_equations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-01-22 17:44:08.000000 lazyfunc-0.1.0/tests/test_lazy_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-01-22 17:44:08.000000 lazyfunc-0.1.0/tests/test_lazy_func_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-01-22 17:44:08.000000 lazyfunc-0.1.0/tests/test_lazy_func_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:22:43.325459 lazyfunc-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-16 19:22:29.000000 lazyfunc-0.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:22:43.321459 lazyfunc-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:22:43.325459 lazyfunc-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-16 19:22:29.000000 lazyfunc-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-16 19:22:29.000000 lazyfunc-0.2.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-16 19:22:29.000000 lazyfunc-0.2.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-16 19:22:29.000000 lazyfunc-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-16 19:22:29.000000 lazyfunc-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-16 19:22:29.000000 lazyfunc-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-16 19:22:43.325459 lazyfunc-0.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:22:43.325459 lazyfunc-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-16 19:22:29.000000 lazyfunc-0.2.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-16 19:22:29.000000 lazyfunc-0.2.0/docs/reference.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:22:43.321459 lazyfunc-0.2.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:22:43.325459 lazyfunc-0.2.0/examples/photometrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-16 19:22:29.000000 lazyfunc-0.2.0/examples/photometrics/data.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-16 19:22:29.000000 lazyfunc-0.2.0/examples/photometrics/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-16 19:22:29.000000 lazyfunc-0.2.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-16 19:22:29.000000 lazyfunc-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 19:22:43.329460 lazyfunc-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:22:43.325459 lazyfunc-0.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-16 19:22:43.000000 lazyfunc-0.2.0/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:22:43.325459 lazyfunc-0.2.0/src/lazyfunc/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-16 19:22:29.000000 lazyfunc-0.2.0/src/lazyfunc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-16 19:22:29.000000 lazyfunc-0.2.0/src/lazyfunc/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9831 2023-04-16 19:22:29.000000 lazyfunc-0.2.0/src/lazyfunc/lazy_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-16 19:22:29.000000 lazyfunc-0.2.0/src/lazyfunc/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-16 19:22:29.000000 lazyfunc-0.2.0/src/lazyfunc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:22:43.325459 lazyfunc-0.2.0/src/lazyfunc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-16 19:22:43.000000 lazyfunc-0.2.0/src/lazyfunc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-16 19:22:43.000000 lazyfunc-0.2.0/src/lazyfunc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 19:22:43.000000 lazyfunc-0.2.0/src/lazyfunc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-16 19:22:43.000000 lazyfunc-0.2.0/src/lazyfunc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-16 19:22:43.000000 lazyfunc-0.2.0/src/lazyfunc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:22:43.325459 lazyfunc-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-16 19:22:29.000000 lazyfunc-0.2.0/tests/test_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-16 19:22:29.000000 lazyfunc-0.2.0/tests/test_equations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-16 19:22:29.000000 lazyfunc-0.2.0/tests/test_lazy_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-16 19:22:29.000000 lazyfunc-0.2.0/tests/test_lazy_func_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-04-16 19:22:29.000000 lazyfunc-0.2.0/tests/test_lazy_func_operators.py
```

### Comparing `lazyfunc-0.1.0/.gitignore` & `lazyfunc-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lazyfunc-0.1.0/LICENSE` & `lazyfunc-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lazyfunc-0.1.0/PKG-INFO` & `lazyfunc-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: lazyfunc
-Version: 0.1.0
-Summary: Wrapper for callables in Python, enabling many operations between them, with lazy evaluation.
+Version: 0.2.0
+Summary: Operations between callables, with lazy evaluation.
 Author-email: Josh Read <joshua-read@hotmail.co.uk>
 Project-URL: Documentation, https://josh-read.github.io/lazyfunc/
 Project-URL: Issues, https://github.com/josh-read/lazyfunc/issues
 Project-URL: Source, https://github.com/josh-read/lazyfunc
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: tests
+Provides-Extra: examples
+Provides-Extra: dev
 Provides-Extra: docs
+Provides-Extra: all
 License-File: LICENSE
```

### Comparing `lazyfunc-0.1.0/pyproject.toml` & `lazyfunc-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools_scm[toml]"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lazyfunc"
-description = "Wrapper for callables in Python, enabling many operations between them, with lazy evaluation."
+description = "Operations between callables, with lazy evaluation."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE.txt"}
 keywords = []
 authors = [
   { name = "Josh Read", email = "joshua-read@hotmail.co.uk" },
 ]
@@ -32,24 +32,36 @@
 Source = "https://github.com/josh-read/lazyfunc"
 
 
 [dirs.env]
 virtual = ".venv"
 
 [project.optional-dependencies]
-tests = [
+examples = [
+  "numpy",
+  "scipy",
+  "matplotlib",
+]
+dev = [
   "pytest",
-  "pytest-cov",
   "numpy",
+  "black",
+  "flake8",
+  "pre-commit",
 ]
 docs = [
   "mkdocs",
   "mkdocstrings-python-legacy",
   "mkdocs-material",
 ]
+all = [
+  "lazyfunc[examples]",
+  "lazyfunc[dev]",
+  "lazyfunc[docs]",
+]
 
 [tool.coverage.run]
 branch = true
 parallel = true
 omit = [
   "src/lazyfunc/__about__.py",
 ]
```

### Comparing `lazyfunc-0.1.0/src/lazyfunc/lazy_func.py` & `lazyfunc-0.2.0/src/lazyfunc/lazy_func.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,111 +1,149 @@
-import numbers
+import inspect
 from warnings import warn
 
-from lazyfunc.utils import callable_name, add_parentheses, insert
+from lazyfunc.arguments import ARGUMENT_ORDER
 from lazyfunc.operators import operators
+from lazyfunc.utils import callable_name, add_parentheses, insert
 
 
-def function_from_operator(operator, *instances):
-    """Returns a function by combining self and other through a specified operation.
-    Self must be of type LazyFunc, other may be a scalar value or any callable including LazyFunc"""
-    if operator.number_of_operands == 1:
-        self, = instances
-        return lambda *x: operator.func(self(*x))
-    elif operator.number_of_operands == 2:
-        self, other = instances
-        if callable(other):
-            return lambda *x: operator.func(self(*x), other(*x))
-        elif isinstance(other, numbers.Real):
-            return lambda *x: operator.func(self(*x), other)
-        else:
-            msg = f"Cannot call {operator.name} on LazyFunc and type {type(other)}. " \
-                  f"Must be either callable or a scalar value."
-            raise TypeError(msg)
-    else:
-        msg = 'Handling of ternary operators not yet implemented!'
-        raise NotImplementedError(msg)
-
-
-def _get_desc(instance, operator_precedence):
-    if callable(instance):
-        desc = callable_name(instance)
-    else:
-        desc = str(instance)
-
-    precedence = getattr(instance, '_precedence', None)
-    if precedence is None:
-        pass
-    elif precedence < operator_precedence:
-        desc = add_parentheses(desc)
-
-    return desc
-
-
-def description_from_operator(operator, *instances, reverse):
-    """Returns a string describing the function resulting from combining self and other through
-    the specified operation. The precedence of the operation is compared to the precedence of the last operation
-    on self and other to determine whether parentheses are required."""
-    descriptions = [_get_desc(instance, operator.precedence) for instance in instances]
-
-    if reverse:
-        descriptions = reversed(descriptions)
-    return operator.format(*descriptions)
-
-
-def lazy_func_method_factory(operator, reverse=False):
-    """Function factory which produces the functions for operations which are bound
-    to LazyFunc."""
-
-    def inner(*instances):
-        new_func = function_from_operator(operator, *instances)
-        new_desc = description_from_operator(operator, *instances, reverse=reverse)
-        mf = LazyFunc(func=new_func, description=new_desc)
-        mf._precedence = operator.precedence
-        return mf
-
-    if operator.number_of_operands == 1:
-        operation_description = operator.format('self')
-    elif operator.number_of_operands == 2:
-        if reverse:
-            operation_description = operator.format('other', 'self')
-        else:
-            operation_description = operator.format('self', 'other')
+class LazyFuncMeta(type):
+    def __new__(mcs, name, bases, attrs):
+        for operator in operators:
+            attrs[operator.name] = mcs.lazy_func_method_factory(operator)
+            if operator.has_reverse:
+                reverse_operator_name = insert(operator.name, "r", index=2)
+                attrs[reverse_operator_name] = mcs.lazy_func_method_factory(
+                    operator, reverse=True
+                )
+        return super().__new__(mcs, name, bases, attrs)
+
+    @staticmethod
+    def lazy_func_method_factory(operator, reverse=False):
+        """Function factory which produces the functions for operations which are bound
+        to LazyFunc."""
+
+        def inner(*instances):
+            new_func = LazyFuncMeta.new_function(operator, *instances)
+            new_func.__signature__ = LazyFuncMeta.build_new_signature(instances)
+            new_desc = LazyFuncMeta.description_from_operator(
+                operator, *instances, reverse=reverse
+            )
+            mf = LazyFunc(func=new_func, description=new_desc)
+            mf._precedence = operator.precedence
+            return mf
 
-    inner.__name__ = operator.name
-    inner.__doc__ = f"Return new instance LazyFunc({operation_description}), " \
-                    "where other may be a scalar value or any other callable including another LazyFunc instance."
-    return inner
+        if operator.number_of_operands == 1:
+            operation_description = operator.format("self")
+        elif operator.number_of_operands == 2:
+            if reverse:
+                operation_description = operator.format("other", "self")
+            else:
+                operation_description = operator.format("self", "other")
+
+        inner.__name__ = operator.name
+        inner.__doc__ = (
+            f"Return new instance LazyFunc({operation_description}), "
+            "where other may be a scalar value or any other callable "
+            "including another LazyFunc instance."
+        )
+        return inner
+
+    @staticmethod
+    def new_function(operator, *instances):
+        def inner(*args, **kwargs):
+            operator_args = []
+            for obj in instances:
+                if not callable(obj):
+                    operator_args.append(obj)
+                else:
+                    callable_kwargs = {}
+                    for key in kwargs:
+                        if key in inspect.signature(obj).parameters:
+                            callable_kwargs[key] = kwargs[key]
+                    operator_args.append(obj(*args, **callable_kwargs))
+            return operator.func(*operator_args)
+
+        return inner
+
+    @staticmethod
+    def description_from_operator(operator, *instances, reverse):
+        """Returns a string describing the function resulting from combining self and
+        other through the specified operation. The precedence of the operation is
+        compared to the precedence of the last operation on self and other to determine
+        whether parentheses are required."""
+        descriptions = [
+            LazyFuncMeta._get_desc(instance, operator.precedence)
+            for instance in instances
+        ]
+
+        if reverse:
+            descriptions = reversed(descriptions)
+        return operator.format(*descriptions)
 
+    @staticmethod
+    def _get_desc(instance, operator_precedence):
+        if callable(instance):
+            desc = callable_name(instance)
+        else:
+            desc = str(instance)
 
-def lazy_func_meta(name, bases, attrs):
-    """Metaclass over class decorator as special operator behaviour needs to persist through inheritance."""
-    for operator in operators:
-        attrs[operator.name] = lazy_func_method_factory(operator)
-        if operator.has_reverse:
-            reverse_operator_name = insert(operator.name, 'r', index=2)
-            attrs[reverse_operator_name] = lazy_func_method_factory(operator, reverse=True)
-    return type(name, bases, attrs)
+        precedence = getattr(instance, "_precedence", None)
+        if precedence is None:
+            pass
+        elif precedence < operator_precedence:
+            desc = add_parentheses(desc)
+
+        return desc
+
+    @staticmethod
+    def build_new_signature(instances):
+        callables = [obj for obj in instances if callable(obj)]
+        if len(callables) == 1:
+            return instances[0].__signature__
+        else:  # build new signature merging any duplicated arguments
+            combined_params = {}
+            instance_parameters = [
+                inspect.signature(obj).parameters for obj in callables
+            ]
+            for (
+                kind
+            ) in (
+                ARGUMENT_ORDER
+            ):  # positional arguments must come first, default arguments must come last
+                for (
+                    params
+                ) in (
+                    instance_parameters
+                ):  # arguments of same kind from first instance come before last
+                    # instance
+                    for name, param in params.items():
+                        if param.kind == kind and name not in combined_params:
+                            combined_params[name] = param
+            return inspect.Signature(parameters=combined_params.values())
 
 
-class LazyFunc(metaclass=lazy_func_meta):
-    """Wrap a callable object enabling arithmetic operations between it and scalar values or any other callables,
-    including LazyFunc instances."""
+class LazyFunc(metaclass=LazyFuncMeta):
+    """Operations between callables, with lazy evaluation."""
 
-    def __init__(self, func, *args, description=None, **kwargs):
+    def __init__(self, func, description=None, **kwargs):
         self.func = func
-        self.args = args
-        self.kwargs = kwargs
         self._description = description
+        self._kwargs = self._default_kwargs = kwargs
         self._precedence = None
 
     @property
+    def __signature__(self):
+        return inspect.signature(self.func)
+
+    @property
     def description(self) -> str:
-        """Defaults to the name of the wrapped callable, but can be set by the user at object initialisation. Also
-        updated when operations are applied with other callables.
+        """Defaults to the name of the wrapped callable, but can be set by the user at
+        object initialisation. Also updated when operations are applied with other
+        callables.
 
         Examples:
             >>> def my_function(x):
             ...     return x
             >>> lf_auto = LazyFunc(my_function)
             >>> lf_auto.description
             'my_function'
@@ -126,62 +164,85 @@
         """Alias of the LazyFunc description."""
         return self.description
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self.description})"
 
     def __call__(self, *args, **kwargs) -> object:
-        """Either calls the wrapped function with the provided args and kwargs, or if the first argument is a callable,
-        returns a new LazyFunc object of LazyFunc(args[0](self)).
+        """Either calls the wrapped function with the provided args and kwargs, or if
+        the first argument is a callable, returns a new LazyFunc object of
+        LazyFunc(args[0](self)).
+
+        When calling a LazyFunc instance, if the first argument is NOT a callable, it
+        behaves exactly as the unwrapped callable.
 
-        When calling a LazyFunc instance, if the first argument is NOT a callable, it behaves exactly as the unwrapped
-        callable.
         Examples:
             >>> @LazyFunc
             ... def my_function(x):
             ...     return 2 * x
             ...
             >>> my_function('foo')  # first argument is not callable
             'foofoo'
             >>> import builtins
             >>> builtin_min = builtins.min
             >>> min = LazyFunc(min)
             >>> min([3, 1, 4, 1, 5, 9])  # first argument is not callable
             1
-            >>> min('lazy', 'function', key=lambda s: s[1])  # first argument is not callable
+            >>> min('lazy', 'function', key=lambda s: s[1])  # first argument is
+            ...                                              # not callable
             'lazy'
             >>> min_of_my_function = min(my_function)  # first argument is callable
             >>> min_of_my_function
             LazyFunc(min(my_function))
 
         Args:
             args: Positional arguments to be passed to wrapped function.
             kwargs: Keyword arguments to be passed to wrapped function.
 
-        Returns:
-            Either the result of the wrapped function evaluated with the supplied args and kwargs, or a new LazyFunc
-            instance.
+        Returns: Either the result of the wrapped function evaluated with the
+        supplied args and _kwargs, or a new LazyFunc instance.
         """
         if callable(args[0]):
             operator_precedence = 17
             other_func, *args = args
-            new_func = lambda *y: self.func(other_func(*y), *args, **kwargs)
-            new_desc = _get_desc(self, operator_precedence) + '(' + callable_name(other_func) + ')'
+
+            def new_func(*x):
+                return self.func(other_func(*x), *args, **kwargs)
+
+            new_desc = (
+                LazyFuncMeta._get_desc(self, operator_precedence)
+                + "("
+                + callable_name(other_func)
+                + ")"
+            )
             mf = LazyFunc(func=new_func, description=new_desc)
             mf._precedence = operator_precedence
             return mf
-        else:
-            return self.func(*args, *self.args, **kwargs, **self.kwargs)
+        else:  # when the function is called the kwargs supplied to the call take
+            # precedence over those set elsewhere
+            final_kwargs = self._kwargs | kwargs
+            return self.func(*args, **final_kwargs)
+
+    def set_kwargs(self, **kwargs):
+        self._kwargs = kwargs
+        return self
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self._kwargs = self._default_kwargs
 
     def is_equal(self, other: callable) -> bool:
         """Checks for equality between self and other.
 
-        To stay consistent with LazyFunc's other dunder methods, the `__eq__` method lazily compares equality
-        between the wrapped LazyFunc and other. Therefore, this method exists to check whether two unevaluated
-        LazyFunc objects are equal, without calling them and comparing the results.
+        To stay consistent with LazyFunc's other dunder methods, the `__eq__` method
+        lazily compares equality between the wrapped LazyFunc and other. Therefore,
+        this method exists to check whether two unevaluated LazyFunc objects are
+        equal, without calling them and comparing the results.
 
         Examples:
             >>> def my_function(x):
             ...     return x
             >>> lf_auto_1 = LazyFunc(my_function)
             >>> lf_auto_2 = LazyFunc(my_function)
             >>> lf_named = LazyFunc(my_function, description='my_named_function')
@@ -189,15 +250,18 @@
             True
             >>> lf_auto_1.is_equal(lf_named)
             False
         """
         try:
             equal = self.description == other.description
         except AttributeError:
-            msg = 'Can only compare a LazyFunc instance with another LazyFunc'
+            msg = "Can only compare a LazyFunc instance with another LazyFunc"
             raise TypeError(msg)
 
         if not equal:
-            msg = 'LazyFunc descriptions found to be not equal though may still be equivalent.'
+            msg = (
+                "LazyFunc descriptions found to be not equal though may still be "
+                "equivalent. "
+            )
             warn(msg)
 
         return equal
```

### Comparing `lazyfunc-0.1.0/src/lazyfunc/operators.py` & `lazyfunc-0.2.0/src/lazyfunc/operators.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 import operator
 from functools import cached_property
 from lazyfunc.utils import insert
 from string import ascii_lowercase
 
 
 def has_dunder(name):
-    return name.startswith('__') and name.endswith('__')
+    return name.startswith("__") and name.endswith("__")
 
 
-DUNDER_METHODS = [func_name for func_name, _ in inspect.getmembers(operator, inspect.isbuiltin) if
-                  has_dunder(func_name)]
+DUNDER_METHODS = [
+    func_name
+    for func_name, _ in inspect.getmembers(operator, inspect.isbuiltin)
+    if has_dunder(func_name)
+]
 
 
 class Operator:
-
     def __init__(self, name, precedence, has_reverse=None):
         self.name = name
         self.precedence = precedence
         self._has_reverse = has_reverse
 
     @cached_property
     def func(self):
@@ -28,52 +30,55 @@
     def number_of_operands(self):
         sig = inspect.signature(self.func)
         return len(sig.parameters)
 
     @property
     def has_reverse(self):
         if self._has_reverse is None:
-            return self.number_of_operands == 2  # most dyadic operators have reverse variants
+            return (
+                self.number_of_operands == 2
+            )  # most dyadic operators have reverse variants
         else:
             return self._has_reverse
 
     @property
     def has_inplace_variant(self):
-        inplace_name = insert(self.name, 'i', 2)
+        inplace_name = insert(self.name, "i", 2)
         return inplace_name in DUNDER_METHODS
 
     def format(self, *values):
-        doc_template = (self.func.__doc__
-                        .removeprefix('Same as ')
-                        .removesuffix('.')
-                        .removesuffix(', for a and b sequences')  # concat
-                        .removesuffix(' (note reversed operands)'))  # contains
+        doc_template = (
+            self.func.__doc__.removeprefix("Same as ")
+            .removesuffix(".")
+            .removesuffix(", for a and b sequences")  # concat
+            .removesuffix(" (note reversed operands)")
+        )  # contains
         for i, (char, _) in enumerate(zip(ascii_lowercase, values)):
-            doc_template = doc_template.replace(char, f'{{{i}}}')
+            doc_template = doc_template.replace(char, f"{{{i}}}")
         return doc_template.format(*values)
 
 
 # https://docs.python.org/3/reference/expressions.html#operator-precedence
 operators = [
-    Operator('__pow__', precedence=15),
-    Operator('__pos__', precedence=14),
-    Operator('__neg__', precedence=14),
-    Operator('__invert__', precedence=14),
-    Operator('__mul__', precedence=13),
-    Operator('__matmul__', precedence=13),
-    Operator('__truediv__', precedence=13),
-    Operator('__floordiv__', precedence=13),
-    Operator('__mod__', precedence=13),
-    Operator('__add__', precedence=12),
-    Operator('__sub__', precedence=12),
-    Operator('__rshift__', precedence=11),
-    Operator('__lshift__', precedence=11),
-    Operator('__and__', precedence=10),
-    Operator('__xor__', precedence=9),
-    Operator('__or__', precedence=8),
-    Operator('__lt__', precedence=7, has_reverse=False),
-    Operator('__le__', precedence=7, has_reverse=False),
-    Operator('__gt__', precedence=7, has_reverse=False),
-    Operator('__ge__', precedence=7, has_reverse=False),
-    Operator('__ne__', precedence=7, has_reverse=False),
-    Operator('__eq__', precedence=7, has_reverse=False),
+    Operator("__pow__", precedence=15),
+    Operator("__pos__", precedence=14),
+    Operator("__neg__", precedence=14),
+    Operator("__invert__", precedence=14),
+    Operator("__mul__", precedence=13),
+    Operator("__matmul__", precedence=13),
+    Operator("__truediv__", precedence=13),
+    Operator("__floordiv__", precedence=13),
+    Operator("__mod__", precedence=13),
+    Operator("__add__", precedence=12),
+    Operator("__sub__", precedence=12),
+    Operator("__rshift__", precedence=11),
+    Operator("__lshift__", precedence=11),
+    Operator("__and__", precedence=10),
+    Operator("__xor__", precedence=9),
+    Operator("__or__", precedence=8),
+    Operator("__lt__", precedence=7, has_reverse=False),
+    Operator("__le__", precedence=7, has_reverse=False),
+    Operator("__gt__", precedence=7, has_reverse=False),
+    Operator("__ge__", precedence=7, has_reverse=False),
+    Operator("__ne__", precedence=7, has_reverse=False),
+    Operator("__eq__", precedence=7, has_reverse=False),
 ]
```

### Comparing `lazyfunc-0.1.0/src/lazyfunc.egg-info/PKG-INFO` & `lazyfunc-0.2.0/src/lazyfunc.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: lazyfunc
-Version: 0.1.0
-Summary: Wrapper for callables in Python, enabling many operations between them, with lazy evaluation.
+Version: 0.2.0
+Summary: Operations between callables, with lazy evaluation.
 Author-email: Josh Read <joshua-read@hotmail.co.uk>
 Project-URL: Documentation, https://josh-read.github.io/lazyfunc/
 Project-URL: Issues, https://github.com/josh-read/lazyfunc/issues
 Project-URL: Source, https://github.com/josh-read/lazyfunc
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: tests
+Provides-Extra: examples
+Provides-Extra: dev
 Provides-Extra: docs
+Provides-Extra: all
 License-File: LICENSE
```

### Comparing `lazyfunc-0.1.0/tests/test_lazy_func.py` & `lazyfunc-0.2.0/tests/test_lazy_func.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,38 +9,38 @@
 
 
 def multi_parameter_function(x, y):
     return x + y
 
 
 class SingleParameterClass:
-
     def __call__(self, x):
         return x
 
 
 class MultiParameterClass:
-
     def __call__(self, x, y):
         return x + y
 
 
 def test_repr():
     mf_f = LazyFunc(single_parameter_function)
-    assert str(mf_f) == 'LazyFunc(single_parameter_function)'
-    mf_f_with_desc = LazyFunc(single_parameter_function, description='my_single_parameter_function')
-    assert str(mf_f_with_desc) == 'LazyFunc(my_single_parameter_function)'
+    assert str(mf_f) == "LazyFunc(single_parameter_function)"
+    mf_f_with_desc = LazyFunc(
+        single_parameter_function, description="my_single_parameter_function"
+    )
+    assert str(mf_f_with_desc) == "LazyFunc(my_single_parameter_function)"
     mf_j = LazyFunc(MultiParameterClass())
-    assert str(mf_j) == 'LazyFunc(MultiParameterClass)'
+    assert str(mf_j) == "LazyFunc(MultiParameterClass)"
 
     @LazyFunc
     def abc(x):
         return x
 
-    assert str(abc + abc) == 'LazyFunc(abc + abc)'
+    assert str(abc + abc) == "LazyFunc(abc + abc)"
 
 
 def test_call():
     x = np.array([1, 2, 3, 4])
     y = np.random.rand(4)
     print(y)
     mf_f = LazyFunc(single_parameter_function)
@@ -55,11 +55,13 @@
     assert mf_min_f(x) == min(x) * 2
 
 
 def test_equality():
     mf_single_parameter_function = LazyFunc(single_parameter_function)
     mf_single_parameter_class = LazyFunc(SingleParameterClass())
     assert (mf_single_parameter_function + mf_single_parameter_class).is_equal(
-        mf_single_parameter_function + mf_single_parameter_class)
+        mf_single_parameter_function + mf_single_parameter_class
+    )
     with pytest.warns(UserWarning):
         assert not (mf_single_parameter_function + mf_single_parameter_class).is_equal(
-             mf_single_parameter_class + mf_single_parameter_function)
+            mf_single_parameter_class + mf_single_parameter_function
+        )
```

### Comparing `lazyfunc-0.1.0/tests/test_lazy_func_operators.py` & `lazyfunc-0.2.0/tests/test_lazy_func_operators.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,82 +9,87 @@
 
 
 def multi_parameter_function(x, y):
     return x + y
 
 
 class SingleParameterClass:
-
     def __call__(self, x):
         return x
 
 
 class MultiParameterClass:
-
     def __call__(self, x, y):
         return x + y
 
 
 def test_mul():
     # test two LazyFunc objects
     x = np.random.rand(4)
     mf_f = LazyFunc(single_parameter_function)
     mf_h = LazyFunc(SingleParameterClass())
     mf_fh = mf_f * mf_h
-    assert str(mf_fh) == 'LazyFunc(single_parameter_function * SingleParameterClass)'
+    assert str(mf_fh) == "LazyFunc(single_parameter_function * SingleParameterClass)"
     assert np.allclose(mf_fh(x), x**2)
     # test a LazyFunc object with a normal function
     mf_g = LazyFunc(multi_parameter_function)
     mf_gj = mf_g * MultiParameterClass()
-    assert str(mf_gj) == 'LazyFunc(multi_parameter_function * MultiParameterClass)'
-    assert np.allclose(mf_gj(x, x), 4*x**2)
+    assert str(mf_gj) == "LazyFunc(multi_parameter_function * MultiParameterClass)"
+    assert np.allclose(mf_gj(x, x), 4 * x**2)
     # test a LazyFunc object with a scalar
     mf_f2 = mf_f * 2
-    assert str(mf_f2) == 'LazyFunc(single_parameter_function * 2)'
-    assert np.allclose(mf_f2(x), 2*x)
+    assert str(mf_f2) == "LazyFunc(single_parameter_function * 2)"
+    assert np.allclose(mf_f2(x), 2 * x)
     with pytest.raises(TypeError):
-        mf_f * 'foo'
+        mf_f_mul_foo = mf_f * "foo"
+        mf_f_mul_foo(0.0)
     # test LazyFunc operation name and docstring
-    assert LazyFunc.__mul__.__name__ == '__mul__'
-    assert LazyFunc.__mul__.__doc__ == 'Return new instance LazyFunc(self * other), where other may be a scalar value or any other callable including another LazyFunc instance.'
+    assert LazyFunc.__mul__.__name__ == "__mul__"
+    assert (
+        LazyFunc.__mul__.__doc__
+        == "Return new instance LazyFunc(self * other), where other may be a scalar "
+        "value or any other callable including another LazyFunc instance.".strip("\n")
+    )
 
 
 def test_add():
     # test two LazyFunc objects
     x = np.random.rand(4)
     mf_f = LazyFunc(single_parameter_function)
     mf_h = LazyFunc(SingleParameterClass())
     mf_fh = mf_f + mf_h
-    assert str(mf_fh) == 'LazyFunc(single_parameter_function + SingleParameterClass)'
-    assert np.allclose(mf_fh(x), 2*x)
+    assert str(mf_fh) == "LazyFunc(single_parameter_function + SingleParameterClass)"
+    assert np.allclose(mf_fh(x), 2 * x)
     # test a LazyFunc object with a normal function
     mf_g = LazyFunc(multi_parameter_function)
     mf_gj = mf_g + MultiParameterClass()
-    assert str(mf_gj) == 'LazyFunc(multi_parameter_function + MultiParameterClass)'
-    assert np.allclose(mf_gj(x, x), 4*x)
+    assert str(mf_gj) == "LazyFunc(multi_parameter_function + MultiParameterClass)"
+    assert np.allclose(mf_gj(x, x), 4 * x)
     # test a LazyFunc object with a scalar
     mf_f2 = mf_f + 2
-    assert str(mf_f2) == 'LazyFunc(single_parameter_function + 2)'
+    assert str(mf_f2) == "LazyFunc(single_parameter_function + 2)"
     assert np.allclose(mf_f2(x), x + 2)
     with pytest.raises(TypeError):
-        mf_f + 'foo'
+        mf_f_add_foo = mf_f + "foo"
+        mf_f_add_foo(0)
 
 
 def test_radd():
     # test two LazyFunc objects
     x = np.random.rand(4)
     mf_f = LazyFunc(single_parameter_function)
     mf_h = LazyFunc(SingleParameterClass())
     mf_fh = mf_f + mf_h
-    assert str(mf_fh) == 'LazyFunc(single_parameter_function + SingleParameterClass)'
-    assert np.allclose(mf_fh(x), 2*x)
+    assert str(mf_fh) == "LazyFunc(single_parameter_function + SingleParameterClass)"
+    assert np.allclose(mf_fh(x), 2 * x)
     # test a LazyFunc object with a normal function
     mf_g = LazyFunc(multi_parameter_function)
     mf_jg = MultiParameterClass() + mf_g
-    assert str(mf_jg) == 'LazyFunc(MultiParameterClass + multi_parameter_function)'
-    assert np.allclose(mf_jg(x, x), 4*x)
+    assert str(mf_jg) == "LazyFunc(MultiParameterClass + multi_parameter_function)"
+    assert np.allclose(mf_jg(x, x), 4 * x)
     # test a LazyFunc object with a scalar
     mf_2f = 2 + mf_f
-    assert str(mf_2f) == 'LazyFunc(2 + single_parameter_function)'
+    assert str(mf_2f) == "LazyFunc(2 + single_parameter_function)"
     assert np.allclose(mf_2f(x), x + 2)
     with pytest.raises(TypeError):
-        mf_f + 'foo'
+        foo_add_mf_f = "foo" + mf_f
+        foo_add_mf_f(0)
```

