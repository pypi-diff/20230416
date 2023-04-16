# Comparing `tmp/pytreeclass-0.2.7.tar.gz` & `tmp/pytreeclass-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytreeclass-0.2.7.tar", last modified: Thu Apr 13 18:00:40 2023, max compression
+gzip compressed data, was "pytreeclass-0.2.8.tar", last modified: Sun Apr 16 20:46:40 2023, max compression
```

## Comparing `pytreeclass-0.2.7.tar` & `pytreeclass-0.2.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:40.145738 pytreeclass-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29181 2023-04-13 18:00:40.145738 pytreeclass-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28305 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:40.141738 pytreeclass-0.2.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:40.141738 pytreeclass-0.2.7/pytreeclass/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/pytreeclass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:40.141738 pytreeclass-0.2.7/pytreeclass/_src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/pytreeclass/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23535 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/pytreeclass/_src/tree_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/pytreeclass/_src/tree_freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)    25696 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/pytreeclass/_src/tree_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    31282 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/pytreeclass/_src/tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    13138 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/pytreeclass/_src/tree_trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:40.141738 pytreeclass-0.2.7/pytreeclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29181 2023-04-13 18:00:40.000000 pytreeclass-0.2.7/pytreeclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-13 18:00:40.000000 pytreeclass-0.2.7/pytreeclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:00:40.000000 pytreeclass-0.2.7/pytreeclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:00:40.000000 pytreeclass-0.2.7/pytreeclass.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 18:00:40.000000 pytreeclass-0.2.7/pytreeclass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 18:00:40.000000 pytreeclass-0.2.7/pytreeclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 18:00:40.145738 pytreeclass-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:40.145738 pytreeclass-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17904 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/tests/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10220 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/tests/test_tree_freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/tests/test_tree_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/tests/test_tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/tests/test_tree_viz_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    17430 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/tests/test_treeclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/tests/test_under_jit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:46:40.528353 pytreeclass-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29188 2023-04-16 20:46:40.524353 pytreeclass-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28312 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:46:40.524353 pytreeclass-0.2.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:46:40.524353 pytreeclass-0.2.8/pytreeclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/pytreeclass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:46:40.524353 pytreeclass-0.2.8/pytreeclass/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/pytreeclass/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18680 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/pytreeclass/_src/tree_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/pytreeclass/_src/tree_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19421 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/pytreeclass/_src/tree_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31487 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/pytreeclass/_src/tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/pytreeclass/_src/tree_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:46:40.524353 pytreeclass-0.2.8/pytreeclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29188 2023-04-16 20:46:40.000000 pytreeclass-0.2.8/pytreeclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-16 20:46:40.000000 pytreeclass-0.2.8/pytreeclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 20:46:40.000000 pytreeclass-0.2.8/pytreeclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 20:46:40.000000 pytreeclass-0.2.8/pytreeclass.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-16 20:46:40.000000 pytreeclass-0.2.8/pytreeclass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-16 20:46:40.000000 pytreeclass-0.2.8/pytreeclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 20:46:40.528353 pytreeclass-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:46:40.524353 pytreeclass-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18439 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/tests/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10220 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/tests/test_tree_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/tests/test_tree_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/tests/test_tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/tests/test_tree_viz_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17379 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/tests/test_treeclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-04-16 20:46:31.000000 pytreeclass-0.2.8/tests/test_under_jit.py
```

### Comparing `pytreeclass-0.2.7/LICENSE` & `pytreeclass-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.7/PKG-INFO` & `pytreeclass-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytreeclass
-Version: 0.2.7
+Version: 0.2.8
 Summary: JAX compatible dataclass.
 Home-page: https://github.com/ASEM000/pytreeclass
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: Apache-2.0
 Keywords: python machine-learning pytorch jax
 Classifier: Development Status :: 5 - Production/Stable
@@ -461,15 +461,15 @@
 
 </details>
 
 ## ➕ More<a id="more"></a>
 
 <details><summary>[Advanced] Register custom user-defined classes to work with visualization and indexing tools. </summary>
 
-Similar to [`jax.tree_util.register_pytree_node`](https://jax.readthedocs.io/en/latest/pytrees.html#extending-pytrees), `PyTreeClass` register common data structures and `treeclass` wrapped classes to figure out how to define the names, types, index, and metadatas of certain leaf along its path.
+Similar to [`jax.tree_util.register_pytree_node`](https://jax.readthedocs.io/en/latest/pytrees.html#extending-pytrees), `PyTreeClass` register common data structures and `treeclass` wrapped classes to figure out how to define the names, types, and index of certain leaf along its path.
 
 Here is an example of registering
 
 ```python
 
 class Tree:
     def __init__(self, a, b):
@@ -486,19 +486,18 @@
 
 # jax unflatten rule
 def tree_unflatten(_, children):
     return Tree(*children)
 
 # PyTreeClass flatten rule
 def pytc_tree_flatten(tree):
-    names = ("a", "b")
+    names = ("a", "b") # or (`None`, `None`) if name is not defined
     types = (type(tree.a), type(tree.b))
-    indices = (0,1)
-    metadatas = (None, None)
-    return [*zip(names, types, indices, metadatas)]
+    indices = (0,1)  # or (`None`, `None`) if index is not defined
+    return [*zip(names, types, indices)]
 
 
 # Register with `jax`
 jax.tree_util.register_pytree_node(Tree, tree_flatten, tree_unflatten)
 
 # Register the `Tree` class trace function to support indexing
 pytc.register_pytree_node_trace(Tree, pytc_tree_flatten)
@@ -834,17 +833,16 @@
     @property
     def at(self):
         return pytc.tree_indexer(self)
 
 def pytc_flatten_rule(tree):
     names =("a","b","c")
     types = map(type, (tree.a, tree.b, tree.c))
-    indices = range(3)
-    metadatas= (None, None, None)
-    return [*zip(names, types, indices, metadatas)]
+    indices = range(3)  # make it indexable like namedtuple
+    return [*zip(names, types, indices)]
 
 pytc.register_pytree_node_trace(FlaxTree, pytc_flatten_rule)
 
 flax_tree = FlaxTree()
 
 print(f"{flax_tree!r}")
 # FlaxTree(a=1, b=(2.0, 3.0), c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00]))
@@ -905,15 +903,15 @@
 </details>
 
 <details> 
 <summary>Use tree_map_with_trace</summary>
 
 V0.2 of `PyTreeClass` register common python datatypes and `treeclass` wrapped class to `trace` registry.
 While `jax` uses `jax.tree_util.register_pytree_node` to define `flatten_rule` for leaves, `PyTreeClass` extends on this
-By registering the `flatten_rule` of (1) names, (2) types, (3) indexing, (4) metadata -if exists-
+By registering the `flatten_rule` of (1) names, (2) types, (3) indexing
 
 For demonstration , the following figure contains the 4 variants of the same `Tree` instance define
 
 ```python
 import jax
 import jax.numpy as jnp
 import pytreeclass as pytc
```

### Comparing `pytreeclass-0.2.7/README.md` & `pytreeclass-0.2.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -438,15 +438,15 @@
 
 </details>
 
 ## ➕ More<a id="more"></a>
 
 <details><summary>[Advanced] Register custom user-defined classes to work with visualization and indexing tools. </summary>
 
-Similar to [`jax.tree_util.register_pytree_node`](https://jax.readthedocs.io/en/latest/pytrees.html#extending-pytrees), `PyTreeClass` register common data structures and `treeclass` wrapped classes to figure out how to define the names, types, index, and metadatas of certain leaf along its path.
+Similar to [`jax.tree_util.register_pytree_node`](https://jax.readthedocs.io/en/latest/pytrees.html#extending-pytrees), `PyTreeClass` register common data structures and `treeclass` wrapped classes to figure out how to define the names, types, and index of certain leaf along its path.
 
 Here is an example of registering
 
 ```python
 
 class Tree:
     def __init__(self, a, b):
@@ -463,19 +463,18 @@
 
 # jax unflatten rule
 def tree_unflatten(_, children):
     return Tree(*children)
 
 # PyTreeClass flatten rule
 def pytc_tree_flatten(tree):
-    names = ("a", "b")
+    names = ("a", "b") # or (`None`, `None`) if name is not defined
     types = (type(tree.a), type(tree.b))
-    indices = (0,1)
-    metadatas = (None, None)
-    return [*zip(names, types, indices, metadatas)]
+    indices = (0,1)  # or (`None`, `None`) if index is not defined
+    return [*zip(names, types, indices)]
 
 
 # Register with `jax`
 jax.tree_util.register_pytree_node(Tree, tree_flatten, tree_unflatten)
 
 # Register the `Tree` class trace function to support indexing
 pytc.register_pytree_node_trace(Tree, pytc_tree_flatten)
@@ -811,17 +810,16 @@
     @property
     def at(self):
         return pytc.tree_indexer(self)
 
 def pytc_flatten_rule(tree):
     names =("a","b","c")
     types = map(type, (tree.a, tree.b, tree.c))
-    indices = range(3)
-    metadatas= (None, None, None)
-    return [*zip(names, types, indices, metadatas)]
+    indices = range(3)  # make it indexable like namedtuple
+    return [*zip(names, types, indices)]
 
 pytc.register_pytree_node_trace(FlaxTree, pytc_flatten_rule)
 
 flax_tree = FlaxTree()
 
 print(f"{flax_tree!r}")
 # FlaxTree(a=1, b=(2.0, 3.0), c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00]))
@@ -882,15 +880,15 @@
 </details>
 
 <details> 
 <summary>Use tree_map_with_trace</summary>
 
 V0.2 of `PyTreeClass` register common python datatypes and `treeclass` wrapped class to `trace` registry.
 While `jax` uses `jax.tree_util.register_pytree_node` to define `flatten_rule` for leaves, `PyTreeClass` extends on this
-By registering the `flatten_rule` of (1) names, (2) types, (3) indexing, (4) metadata -if exists-
+By registering the `flatten_rule` of (1) names, (2) types, (3) indexing
 
 For demonstration , the following figure contains the 4 variants of the same `Tree` instance define
 
 ```python
 import jax
 import jax.numpy as jnp
 import pytreeclass as pytc
```

### Comparing `pytreeclass-0.2.7/docs/conf.py` & `pytreeclass-0.2.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.7/pytreeclass/__init__.py` & `pytreeclass-0.2.8/pytreeclass/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,8 +43,8 @@
     "register_pytree_node_trace",
     "tree_map_with_trace",
     "tree_leaves_with_trace",
     "tree_flatten_with_trace",
     "tree_repr_with_trace",
 )
 
-__version__ = "0.2.7"
+__version__ = "0.2.8"
```

### Comparing `pytreeclass-0.2.7/pytreeclass/_src/tree_decorator.py` & `pytreeclass-0.2.8/pytreeclass/_src/tree_decorator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import functools as ft
 import sys
+from collections.abc import MutableMapping, MutableSequence
 from contextlib import suppress
 from types import FunctionType, MappingProxyType
 from typing import Any, Callable, NamedTuple, Sequence, TypeVar
 
 import jax.tree_util as jtu
 from typing_extensions import dataclass_transform
 
@@ -17,34 +18,33 @@
     is_tree_equal,
     tree_copy,
     tree_indexer,
 )
 from pytreeclass._src.tree_pprint import tree_repr, tree_str
 from pytreeclass._src.tree_trace import register_pytree_node_trace
 
-_NOT_SET = type("NOT_SET", (), {"__repr__": lambda _: "?"})()
-_MUTABLE_TYPES = (list, dict, set)
-_ANNOTATIONS = "__annotations__"
-_POST_INIT = "__post_init__"
-_FIELDS = "__fields__"
-T = TypeVar("T")
+
+class NOT_SET:
+    __repr__ = lambda _: "?"
 
 
 PyTree = Any
+T = TypeVar("T")
+_NOT_SET = NOT_SET()
+_FIELDS = "__fields__"
+_POST_INIT = "__post_init__"
+_MUTABLE_TYPES = (MutableSequence, MutableMapping, set)
+
 
 """Define a class decorator that is compatible with JAX's transformation."""
 
 
 def is_treeclass(node: Any) -> bool:
-    """Returns `True` if class or instance is a `treeclass`."""
-    # use `_setattr` as a proxy for `treeclass` as overriding `__setattr__
-    # or `__delattr__` is not allowed, this behavior is similar
-    # to `dataclasses.dataclass(frozen=True)` restriction.
-    klass = node if isinstance(node, type) else type(node)
-    return getattr(klass, "__setattr__", None) is _setattr
+    """Check if a node is a `treeclass`."""
+    return (node if isinstance(node, type) else type(node)).__setattr__ is _setattr
 
 
 class Field(NamedTuple):
     name: str | None = None
     type: type | None = None
     default: Any = _NOT_SET
     factory: Any = None
@@ -52,36 +52,32 @@
     repr: bool = True
     kw_only: bool = False
     pos_only: bool = False
     metadata: MappingProxyType[str, Any] | None = None
     callbacks: Sequence[Any] = ()
     alias: str | None = None
 
-    def __hash__(self) -> int:
-        # since `_generate_init_code` is caching the `fields`, then it is better
-        # only hash arguments that are used in generating the init code string
-        # this is avoid rewrtining the same final init code string multiple times.
-        return tree_hash(
-            (
-                self.name,
-                self.default,
-                self.factory,
-                self.init,
-                self.kw_only,
-                self.pos_only,
-                self.alias,
-            )
-        )
-
     def __eq__(self, other: Any) -> bool:
         return hash(self) == hash(other)
 
     def __repr__(self) -> str:
         return tree_repr(self)
 
+    def __hash__(self) -> int:
+        parameters = (
+            self.name,
+            self.default,
+            self.factory,
+            self.init,
+            self.kw_only,
+            self.pos_only,
+            self.alias,
+        )
+        return tree_hash(parameters)
+
 
 def field(
     *,
     default: Any = _NOT_SET,
     factory: Callable | None = None,
     init: bool = True,
     repr: bool = True,
@@ -134,44 +130,38 @@
     """
     if not isinstance(alias, (str, type(None))):
         msg = "`alias` must be a string or None, "
         msg += f"got type=`{type(alias).__name__}` instead."
         raise TypeError(msg)
 
     if default is not _NOT_SET and factory is not None:
-        # mutually exclusive arguments
-        # this is the similar behavior to `dataclasses`
         msg = "`default` and `factory` are mutually exclusive arguments."
         msg += f"got default={default} and factory={factory}"
         raise ValueError(msg)
 
     if kw_only is True and pos_only is True:
-        # mutually exclusive arguments
         msg = "`kw_only` and `pos_only` are mutually exclusive arguments."
         msg += f"got kw_only={kw_only} and pos_only={pos_only}"
         raise ValueError(msg)
 
     if isinstance(metadata, dict):
         metadata = MappingProxyType(metadata)  # type: ignore
     elif metadata is not None:
         raise TypeError("`metadata` must be a Mapping or None")
 
-    # check if `callbacks` is a Sequence of functions
     if not isinstance(callbacks, Sequence):
         msg = f"`callbacks` must be a Sequence of functions, got {type(callbacks)}"
         raise TypeError(msg)
 
-    # sanity check for callbacks
     for index, callback in enumerate(callbacks):
         if not isinstance(callback, Callable):  # type: ignore
             msg = "`callbacks` must be a Sequence of functions, "
             msg += f"got `{type(callbacks).__name__}` at index={index}"
             raise TypeError(msg)
 
-    # set name and type post initialization
     return Field(
         name=None,
         type=None,
         default=default,
         factory=factory,
         init=init,
         repr=repr,
@@ -189,140 +179,104 @@
         raise TypeError(f"Cannot get fields of {item!r}.")
 
     return tuple(vars(item)[_FIELDS].values())
 
 
 @ft.lru_cache
 def _generate_field_map(klass: type) -> dict[str, Field]:
-    # get all the fields of the class and its base classes
-    # get the fields of the class and its base classes
     field_map = dict()
 
     if klass is object:
-        # base case for recursion to stop
         return field_map
 
     for base in reversed(klass.__mro__[1:]):
-        # get the fields of the base class in the MRO
-        # in reverse order to ensure the correct order of the fields
-        # are preserved, i.e. the fields of the base class are added first
-        # and the fields of the derived class are added last so that
-        # in case of name collision, the derived class fields are preserved
+        # get the fields of the base class in the MRO in reverse order to ensure
+        # the correct order of the fields are preserved
         field_map.update(_generate_field_map(base))
 
-    # transform the annotated attributes of the class into Fields
-    # while assigning the default values of the Fields to the annotated attributes
     # TODO: use inspect to get annotations, once we are on minimum python version >3.9
-    if _ANNOTATIONS not in vars(klass):
+    if "__annotations__" not in vars(klass):
         return field_map
 
-    for name in (annotation_map := vars(klass)[_ANNOTATIONS]):
-        # get the value associated with the type hint
-        # in essence will skip any non type-hinted attributes
+    for name in (annotation_map := vars(klass)["__annotations__"]):
         value = vars(klass).get(name, _NOT_SET)
-        # at this point we stick to the type hint provided by the user
-        # inconsistency between the type hint and the value will be handled later
         type = annotation_map[name]
 
         if name == "self":
             # while `dataclasses` allows `self` as a field name, its confusing
             # and not recommended. so raise an error
             msg = "Field name cannot be `self`."
             raise ValueError(msg)
 
         if isinstance(value, Field):
-            # the annotated attribute is a `Field``
-            # example case: `x: Any = field(default=1)`
-            # assign the name and type to the Field from the annotation
+            # case: `x: Any = field(default=1)`
             if isinstance(value.default, _MUTABLE_TYPES):
                 # example case: `x: Any = field(default=[1, 2, 3])`
-                # https://github.com/ericvsmith/dataclasses/issues/3
                 msg = f"Mutable default value of field `{name}` is not allowed, use "
                 msg += f"`factory=lambda: {value.default}` instead."
                 raise TypeError(msg)
 
             field_map[name] = value._replace(name=name, type=type)
 
         elif isinstance(value, _MUTABLE_TYPES):
             # https://github.com/ericvsmith/dataclasses/issues/3
             # example case: `x: Any = [1, 2, 3]`
-            # this is the prime motivation for writing this decorator
-            # as from python 3.11, jax arrays `dataclasses` will raise an error if
-            # `JAX` arrays are used as default values.
-            # the `dataclasses` logic is flawed by using `__hash__` existence
-            # as a proxy for immutability, which is not the case for `JAX` arrays
-            # which are immutable but do not have a `__hash__` method
             msg = f"Mutable value= {(value)} is not allowed"
             msg += f" for field `{name}` in class `{klass.__name__}`.\n"
             msg += f" use `field(... ,factory=lambda:{value})` instead"
             raise TypeError(msg)
 
         elif value is _NOT_SET:
-            # nothing is assigned to the annotated attribute
-            # example case: `x: Any`
-            # create a Field and assign it to the class
+            # case: `x: Any`
             field_map[name] = Field(name=name, type=type)
 
         else:
-            # example case: `x: int = 1`
-            # create a Field and assign default value to the class
+            # case: `x: int = 1`
             field_map[name] = Field(name=name, type=type, default=value)
 
     return field_map
 
 
 @ft.lru_cache
-def _generate_init_code(fields: Sequence[Field]):
-    # generate the init method code string
-    # in here, we generate the function head and body and add `default`/`factory`
-    # for example, if we have a class with fields `x` and `y`
-    # then generated code will something like  `def __init__(self, x, y): self.x = x; self.y = y`
+def _generate_init_code(fields: Sequence[Field]) -> str:
     head = body = ""
 
     for field in fields:
         name = field.name  # name in body
         alias = field.alias or name  # name in constructor
 
         mark0 = f"field_map['{name}'].default"
         mark1 = f"field_map['{name}'].factory()"
         mark2 = f"self.{name}"
 
         if field.kw_only and "*" not in head and field.init:
-            # if the field is keyword only, and we have not added the `*` yet
             head += "*, "
 
         if field.default is not _NOT_SET:
-            # we add the default into the function head (def f(.. x= default_value))
-            # if the the field require initialization. if not, then omit it from head
+            # in head: def f(.. x= default_value)
             head += f"{alias}={mark0}, " if field.init else ""
-            # we then add self.x = x for the body function if field is initialized
-            # otherwise, define the default value inside the body ( self.x = default_value)
+            # in body:  self.x = default_value
             body += f"\t\t{mark2}=" + (f"{alias}\n " if field.init else f"{mark0}\n")
         elif field.factory is not None:
-            # same story for functions as above
             head += f"{alias}={mark1}, " if field.init else ""
             body += f"\t\t{mark2}=" + (f"{alias}\n" if field.init else f"{mark1}\n")
         else:
             # no defaults are added
             head += f"{alias}, " if field.init else ""
             body += f"\t\t{mark2}={alias}\n " if field.init else ""
 
         if field.pos_only and field.init:
-            # if the field is positional only, we add a "/" marker after it
             if "/" in head:
                 head = head.replace("/,", "")
 
             head += "/, "
 
-    # in case no field is initialized, we add a pass statement to the body
-    # to avoid syntax error in the generated code
+    # add pass to avoid syntax error if all fields are ignored
     body += "\t\tpass"
-    # add the body to the head
     body = "\tdef __init__(self, " + head[:-2] + "):\n" + body
-    # use closure to be able to reference default values of all types
     body = f"def closure(field_map):\n{body}\n\treturn __init__"
     return body.expandtabs(4)
 
 
 def _generate_init(klass: type) -> FunctionType:
     field_map = _generate_field_map(klass)
     local_namespace = dict()  # type: ignore
@@ -338,18 +292,15 @@
         argdefs=method.__defaults__,
         closure=method.__closure__,
     )
 
 
 @_conditional_mutable_method
 def _setattr(tree: PyTree, key: str, value: Any) -> None:
-    # setattr under `_mutable_context` context otherwise raise an error
     if key in (field_map := vars(tree)[_FIELDS]):
-        # apply the callbacks on setting the value
-        # check if the key is a field name
         for callback in field_map[key].callbacks:
             try:
                 # callback is a function that takes the value of the field
                 # and returns a modified value
                 value = callback(value)
             except Exception as e:
                 msg = f"Error for field=`{key}`:\n{e}"
@@ -394,96 +345,66 @@
             raise AttributeError(msg)
         return output
 
     return wrapper
 
 
 def _tree_unflatten(klass: type, treedef: Any, leaves: list[Any]):
-    """Unflatten rule for `treeclass` to use with `jax.tree_unflatten`."""
     tree = object.__new__(klass)
     # update through vars, to avoid calling the `setattr` method
     # that will check for callbacks.
-    # calling `setattr` will trigger any defined callbacks by the user
-    # on each unflattening which is not efficient.
-    # however it might be useful to constantly check if the updated value is
-    # satisfying the constraints defined by the user in the callbacks.
     vars(tree).update(treedef[1])
     vars(tree).update(zip(treedef[0], leaves))
     return tree
 
 
 def _tree_flatten(tree: PyTree):
-    """Flatten rule for `treeclass` to use with `jax.tree_flatten`."""
+    # Flatten rule for `treeclass` to use with `jax.tree_flatten`
     static, dynamic = dict(vars(tree)), dict()
     for key in static[_FIELDS]:
         dynamic[key] = static.pop(key)
     return list(dynamic.values()), (tuple(dynamic.keys()), static)
 
 
 def _tree_trace(tree: PyTree) -> list[tuple[Any, Any, Any, Any]]:
-    """Trace flatten rule to be used with the `tree_trace` module."""
+    # Trace flatten rule to be used with the `tree_trace` module
     leaves, (keys, _) = _tree_flatten(tree)
     names = (f"{key}" for key in keys)
     types = map(type, leaves)
     indices = range(len(leaves))
-    metadatas = (dict(repr=F.repr, id=id(getattr(tree, F.name))) for F in fields(tree))  # type: ignore
-    return [*zip(names, types, indices, metadatas)]
+    return [*zip(names, types, indices)]
 
 
 def _register_treeclass(klass: type[T]) -> type[T]:
     with suppress(ValueError):
         # `ValueError` is raised for duplicate registration.
         # there are two cases where a class is registered more than once:
         # first, when a class is decorated with `treeclass` more than once (e.g. `treeclass(treeclass(Class))`)
         # second when a class is decorated with `treeclass` and has a parent class that is decorated with `treeclass`
         # in that case `__init_subclass__` registers the class before the decorator registers it.
-        # this can be also be done using metaclass that registers the class on initialization
-        # but we are trying to stay away from deep magic.
         # register the trace flatten rule
         register_pytree_node_trace(klass, _tree_trace)
         # register the flatten/unflatten rules with jax
         jtu.register_pytree_node(klass, _tree_flatten, ft.partial(_tree_unflatten, klass))  # type: ignore
 
     return klass
 
 
 def _init_subclass_wrapper(init_subclass_method: Callable) -> Callable:
     # Non-decorated subclasses uses the base `treeclass` leaves only
-    # this behavior is aligned with `dataclasses` not registering non-decorated
-    # subclasses dataclass fields. for example:
-    # >>> @treeclass
-    # ... class A:
-    # ...   a:int=1
-    # >>> class B(A):
-    # ...    b:int=2
-    # >>> tree = B()
-    # >>> jax.tree_leaves(tree)
-    # [1]
-    # however if we decorate `B` with `treeclass` then the fields of `B` will be registered as leaves
-    # >>> @treeclass
-    # ... class B(A):
-    # ...    b:int=2
-    # >>> tree = B()
-    # >>> jax.tree_leaves(tree)
-    # [1, 2]
-    # this behavior is different from `flax.struct.dataclass`
-    # as it does not register non-decorated subclasses field that inherited from decorated subclasses.
     @classmethod  # type: ignore
     @ft.wraps(init_subclass_method)
     def wrapper(klass: type, *a, **k) -> None:
         init_subclass_method(*a, **k)
         _register_treeclass(klass)
 
     return wrapper
 
 
 def _treeclass_transform(klass: type[T]) -> type[T]:
-    # the method is called after registering the class with `_register_treeclass`
-    # cached to prevent wrapping the same class multiple times
-
     for key, method in (("__setattr__", _setattr), ("__delattr__", _delattr)):
         # basic required methods
         if key in vars(klass):
             if vars(klass)[key] is method:
                 return klass  # already transformed
             # the user defined a method that conflicts with the required method
             msg = f"Unable to transform the class `{klass.__name__}` with {key} method defined."
```

### Comparing `pytreeclass-0.2.7/pytreeclass/_src/tree_freeze.py` & `pytreeclass-0.2.8/pytreeclass/_src/tree_freeze.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.7/pytreeclass/_src/tree_indexer.py` & `pytreeclass-0.2.8/pytreeclass/_src/tree_indexer.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,26 +5,28 @@
 
 import copy
 import functools as ft
 import operator as op
 from collections.abc import Callable
 from contextlib import contextmanager
 from math import ceil, floor, trunc
-from typing import Any, NamedTuple, TypeVar
+from typing import Any, NamedTuple, Sequence, TypeVar
 
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import numpy as np
 
 from pytreeclass._src.tree_trace import tree_map_with_trace
 
-PyTree = Any
+EllipsisType = type(Ellipsis)
+TraceType = Any
 _no_initializer = object()
 _non_partial = object()
+PyTree = TypeVar("PyTree")
 T = TypeVar("T")
 
 # allow methods in mutable context to be called without raising an error
 # this is done by registering the instance id in a set before entering the
 # mutable context and removing it after exiting the context
 _mutable_instance_registry: set[int] = set()
 
@@ -46,407 +48,233 @@
 def _mutable_context(tree: PyTree, *, kopy: bool = False):
     tree = copy.copy(tree) if kopy else tree
     _mutable_instance_registry.add(id(tree))
     yield tree
     _mutable_instance_registry.discard(id(tree))
 
 
-def _is_leaf_bool(node: Any) -> bool:
-    if hasattr(node, "dtype"):
-        return node.dtype == "bool"
-    return isinstance(node, bool)
-
-
-def _check_valid_mask_leaf(where: Any):
-    if not _is_leaf_bool(where) and where is not None:
-        raise TypeError(f"All tree leaves must be boolean.Found {(where)}")
-    return where
-
-
-def _true_tree(tree: PyTree, is_leaf) -> PyTree:
-    return jtu.tree_map(lambda _: True, tree, is_leaf=is_leaf)
-
-
 # tree indexing by boolean PyTree
 
 
 def _get_at_mask(
     tree: PyTree, where: PyTree, is_leaf: Callable[[Any], bool] | None
 ) -> PyTree:
-    def lhs_get(lhs: Any, where: Any):
+    def leaf_get(leaf: Any, where: Any):
         # check if where is a boolean leaf inside the `tree_map`
         # to avoid extrachecks in `tree_map`
-        where = _check_valid_mask_leaf(where)
-        if isinstance(lhs, (jax.Array, np.ndarray)):
+        if isinstance(leaf, (jax.Array, np.ndarray)):
             # return empty array instead of None if condition is not met
             # not `jittable` as size of array changes
-            return lhs[jnp.where(where)]
-        return lhs if where else None
+            return leaf[jnp.where(where)]
+        return leaf if where else None
 
-    return jtu.tree_map(lhs_get, tree, where, is_leaf=is_leaf)
+    return jtu.tree_map(leaf_get, tree, where, is_leaf=is_leaf)
 
 
 def _set_at_mask(
     tree: PyTree,
     where: PyTree,
     set_value: Any,
     is_leaf: Callable[[Any], bool] | None,
 ) -> PyTree:
-    def lhs_set(lhs: Any, where: Any, set_value: Any):
+    def leaf_set(leaf: Any, where: Any, set_value: Any):
         # check if where is a boolean leaf inside the `tree_map`
         # to avoid extrachecks in `tree_map`
-        where = _check_valid_mask_leaf(where)
-        if isinstance(lhs, (jax.Array, np.ndarray)):
+        if isinstance(leaf, (jax.Array, np.ndarray)):
             if jnp.isscalar(set_value):
-                # apply scalar set_value to lhs array if condition is met
-                return jnp.where(where, set_value, lhs)
+                # apply scalar set_value to leaf array if condition is met
+                return jnp.where(where, set_value, leaf)
             # set_value is not scalar
-            return set_value if jnp.all(where) else lhs
-        # lhs is not an array and set_value, so we apply the set_value to the
-        # lhs if the condition is met
-        return set_value if (where is True) else lhs
+            return set_value if jnp.all(where) else leaf
+        # leaf is not an array and set_value, so we apply the set_value to the
+        # leaf if the condition is met
+        return set_value if (where is True) else leaf
 
     if isinstance(set_value, type(tree)) and (
         jtu.tree_structure(tree, is_leaf=is_leaf)
         == jtu.tree_structure(set_value, is_leaf=is_leaf)
     ):
         # do not broadcast set_value if it is a pytree of same structure
         # for example tree.at[where].set(tree2) will set all tree leaves to tree2 leaves
         # if tree2 is a pytree of same structure as tree
         # instead of making each leaf of tree a copy of tree2
         # is design is similar to `numpy` design `Array.at[...].set(Array)`
-        return jtu.tree_map(lhs_set, tree, where, set_value, is_leaf=is_leaf)
+        return jtu.tree_map(leaf_set, tree, where, set_value, is_leaf=is_leaf)
 
     # set_value is broadcasted to tree leaves
     # for example tree.at[where].set(1) will set all tree leaves to 1
-    partial_lhs_set = lambda lhs, where: lhs_set(lhs, where, set_value)
-    return jtu.tree_map(partial_lhs_set, tree, where, is_leaf=is_leaf)
+    partial_leaf_set = lambda leaf, where: leaf_set(leaf, where, set_value)
+    return jtu.tree_map(partial_leaf_set, tree, where, is_leaf=is_leaf)
 
 
 def _apply_at_mask(
     tree: PyTree,
     where: PyTree,
     func: Callable[[Any], Any],
     is_leaf: Callable[[Any], bool] | None,
 ) -> PyTree:
-    def lhs_apply(lhs: Any, where: bool):
+    def leaf_apply(leaf: Any, where: bool):
         # check if where is a boolean leaf inside the `tree_map`
         # to avoid extrachecks in `tree_map`
-        where, value = _check_valid_mask_leaf(where), func(lhs)
-        if isinstance(lhs, (jax.Array, np.ndarray)):
+        value = func(leaf)
+        if isinstance(leaf, (jax.Array, np.ndarray)):
             try:
-                # lhs is an array with scalar output
-                return jnp.where(where, value, lhs)
+                # leaf is an array with scalar output
+                return jnp.where(where, value, leaf)
             except TypeError:
                 # set_value is not `scalar` type
-                return value if jnp.all(where) else lhs
-        # lhs is not an array and value is not scalar
-        return value if (where is True) else lhs
+                return value if jnp.all(where) else leaf
+        # leaf is not an array and value is not scalar
+        return value if (where is True) else leaf
 
-    return jtu.tree_map(lhs_apply, tree, where, is_leaf=is_leaf)
+    return jtu.tree_map(leaf_apply, tree, where, is_leaf=is_leaf)
 
 
 def _reduce_at_mask(
     tree: PyTree,
     where: PyTree,
     func: Callable[[Any, Any], Any],
     initializer: Any = _no_initializer,
     is_leaf: Callable[[Any], bool] | None = None,
 ) -> Any:
-    # note: current `jax`` implementation of `tree_reduce`
-    # does not support `is_leaf` argument, but it is supported here
     tree = tree.at[where].get(is_leaf=is_leaf)
     if initializer is _no_initializer:
         return jtu.tree_reduce(func, tree)
     return jtu.tree_reduce(func, tree, initializer)
 
 
-class TreeAtMask(NamedTuple):
-    tree: PyTree
-    where: PyTree
-
-    def get(self, *, is_leaf: Callable[[Any], bool] | None = None) -> PyTree:
-        where = _true_tree(self.tree, is_leaf) if self.where is ... else self.where
-        return _get_at_mask(self.tree, where, is_leaf)
-
-    def set(
-        self, set_value: Any, *, is_leaf: Callable[[Any], bool] | None = None
-    ) -> PyTree:
-        where = _true_tree(self.tree, is_leaf) if self.where is ... else self.where
-        return _set_at_mask(self.tree, where, set_value, is_leaf)
-
-    def apply(
-        self,
-        func: Callable[[Any], Any],
-        *,
-        is_leaf: Callable[[Any], bool] | None = None,
-    ):
-        where = _true_tree(self.tree, is_leaf) if self.where is ... else self.where
-        return _apply_at_mask(self.tree, where, func, is_leaf)
-
-    def reduce(
-        self,
-        func: Callable[[Any, Any], Any],
-        initializer: Callable[[Any, Any], Any] | Any = _no_initializer,
-        *,
-        is_leaf: Callable[[Any], bool] | None = None,
-    ) -> Any:
-        where = _true_tree(self.tree, is_leaf) if self.where is ... else self.where
-        return _reduce_at_mask(self.tree, where, func, initializer, is_leaf)
-
-    def __getitem__(self, rhs_where: str | int | PyTree) -> TreeAtMask:
-        if isinstance(rhs_where, (str, int)):
-            # promote `rhs` path to boolean mask
-            mask = self.tree != self.tree
-            mask = mask.at[rhs_where].set(True)
-            rhs_where = mask
-
-        rhs_where = self.where & rhs_where
-        return TreeAtMask(tree=self.tree, where=rhs_where)
-
-    def __getattr__(self, name: str) -> TreeAtMask:
-        # support for nested `.at`
-        if name == "at":
-            # pass the current where condition to the next level
-            return TreeAtMask(tree=self.tree, where=self.where)
-
-        msg = f"{name} is not a valid attribute of {self}\n"
-        msg += f"Did you mean to use .at[{name!r}]?"
-        raise AttributeError(msg)
-
-
-# tree indexing by name or index  path
-
-
-def _get_at_trace(
+def _merge_where(
     tree: PyTree,
-    where: tuple[int | str, ...],
+    where: tuple[int | str | PyTree | EllipsisType, ...],
     is_leaf: Callable[[Any], bool] | None = None,
-) -> PyTree:
-    # canonicalize `where` to `tuple` to conform to leaf trace type
-    where = tuple(where)
+):
+    def merge_non_boolean_where(
+        where: tuple[int | str | EllipsisType, ...],
+        trace: Sequence[TraceType],
+        leaf: Any,
+    ):
+        names, _, indices = trace
+        is_array = isinstance(leaf, (jax.Array, np.ndarray))
 
-    def lhs_get(trace, leaf):
-        names, _, indices, __ = trace
+        if len(where) > len(indices):
+            return jnp.zeros_like(leaf, dtype=bool) if is_array else False
         for i, item in enumerate(where):
-            try:
-                if (isinstance(item, int) and indices[i] != item) or (
-                    isinstance(item, str) and names[i] != item
-                ):
-                    return None
-            except IndexError:
-                msg = f"Out of bounds path={where} for leaf={leaf}."
-                msg += f" Path length={len(where)} is longer than "
-                msg += f"leaf path levels={len(indices)-1}."
-                raise IndexError(msg)
-        return leaf
-
-    return tree_map_with_trace(lhs_get, tree, is_leaf=is_leaf)
-
-
-def _set_at_trace(
-    tree: PyTree,
-    where: tuple[int | str, ...],
-    set_value: Any,
-    is_leaf: Callable[[Any], bool] | None = None,
-) -> PyTree:
-    # canonicalize `where` to `tuple` to conform to leaf trace type
-    where = tuple(where)
+            if item is ... or indices[i] == item or names[i] == item:
+                # no mismatch in where and trace
+                continue
+            return jnp.zeros_like(leaf, dtype=bool) if is_array else False
+        return jnp.ones_like(leaf, dtype=bool) if is_array else True
+
+    def merge_boolean_where(*leaves):
+        def is_leaf_bool(leaf: Any) -> bool:
+            if hasattr(leaf, "dtype"):
+                return leaf.dtype == "bool"
+            return isinstance(leaf, bool)
+
+        verdict = True
+        for leaf in leaves:
+            if not is_leaf_bool(leaf):
+                msg = f"Expected boolean leaf, found {type(leaf).__name__}."
+                raise TypeError(msg)
+            verdict &= leaf
+        return verdict
 
-    def lhs_set(trace, leaf, set_value: Any):
-        names, _, indices, __ = trace
-        for i, item in enumerate(where):
-            try:
-                if (isinstance(item, int) and indices[i] != item) or (
-                    isinstance(item, str) and names[i] != item
-                ):
-                    return leaf
-            except IndexError:
-                msg = f"Out of bounds path={where} for leaf={leaf}."
-                msg += f" Path length={len(where)} is longer than "
-                msg += f"leaf path levels={len(indices)-1}."
-                raise IndexError(msg)
-        # consider the same structure PyTree case tree.at[...].set(tree)
-        return set_value
+    mask = None
 
-    # set_value is broadcasted to tree leaves
-    # for example tree.at[where].set(1) will set all tree leaves to 1
-    partial_lhs_set = lambda trace, lhs: lhs_set(trace, lhs, set_value)
-    return tree_map_with_trace(partial_lhs_set, tree, is_leaf=is_leaf)
+    if non_boolean_where := [i for i in where if isinstance(i, (int, str, type(...)))]:
+        func = ft.partial(merge_non_boolean_where, non_boolean_where)
+        mask = tree_map_with_trace(func, tree, is_leaf=is_leaf)
 
+    if boolean_where := [i for i in where if isinstance(i, type(tree))]:
+        args = (mask, *boolean_where) if mask else boolean_where
+        mask = jtu.tree_map(merge_boolean_where, *args)
 
-def _apply_at_trace(
-    tree: PyTree,
-    where: tuple[int | str, ...],
-    func: Callable,
-    is_leaf: Callable[[Any], bool] | None = None,
-) -> PyTree:
-    # canonicalize `where` to `tuple` to conform to leaf trace type
-    where = tuple(where)
+    return mask
 
-    def lhs_apply(trace, leaf):
-        names, _, indices, __ = trace
 
-        for i, item in enumerate(where):
-            try:
-                if (isinstance(item, int) and indices[i] != item) or (
-                    isinstance(item, str) and names[i] != item
-                ):
-                    return leaf
-            except IndexError:
-                msg = f"Out of bounds path={where} for leaf={leaf}."
-                msg += f" Path length={len(where)} is longer than "
-                msg += f"leaf path levels={len(indices)-1}."
-                raise IndexError(msg)
-        return func(leaf)
+def _recursive_getattr(tree: Any, where: tuple[str, ...]):
+    def step(tree: Any, where: tuple[str, ...]):
+        if len(where) == 1:
+            return getattr(tree, where[0])
+        return step(getattr(tree, where[0]), where[1:])
 
-    return tree_map_with_trace(lhs_apply, tree, is_leaf=is_leaf)
+    return step(tree, where)
 
 
-def _reduce_at_trace(
-    tree: PyTree,
-    where: tuple[str | int, ...],
-    func: Callable[[Any, Any], Any],
-    initializer: Any = _no_initializer,
-    is_leaf: Callable[[Any], bool] | None = None,
-) -> PyTree:
-    # note: current `jax`` implementation of tree_reduce does
-    # not support `is_leaf` argument using `tree_map_with_trace` with `is_leaf` argument
-    # achieves the same result
-    # canonicalize `where` to `tuple` to conform to leaf trace type
-    where = tuple(where)
-
-    def lhs_reduce(trace, leaf):
-        names, _, indices, __ = trace
-
-        for i, item in enumerate(where):
-            try:
-                if (isinstance(item, int) and indices[i] != item) or (
-                    isinstance(item, str) and names[i] != item
-                ):
-                    return None
-            except IndexError:
-                msg = f"Out of bounds path={where} for leaf={leaf}."
-                msg += f" Path length={len(where)} is more than "
-                msg += f"leaf path levels={len(indices)-1}."
-                raise IndexError(msg)
-        return leaf
-
-    tree = tree_map_with_trace(lhs_reduce, tree, is_leaf=is_leaf)
-    if initializer is _no_initializer:
-        return jtu.tree_reduce(func, tree)
-    return jtu.tree_reduce(func, tree, initializer=initializer)
+class AtIndexer(NamedTuple):
+    # base class for indexing with `.at`
+    tree: PyTree
+    where: tuple[str | int] | PyTree
 
+    def __getitem__(self, where: str | int | PyTree | EllipsisType) -> AtIndexer:
+        if isinstance(where, (type(self.tree), str, int, EllipsisType)):
+            return AtIndexer(self.tree, (*self.where, where))
 
-class TreeAtTrace(NamedTuple):
-    tree: PyTree
-    where: tuple[int | str]
+        raise NotImplementedError(
+            f"Indexing with {type(where).__name__} is not implemented.\n"
+            "Example of supported indexing:\n\n"
+            "@pytc.treeclass\n"
+            f"class {type(self.tree).__name__}:\n"
+            "    ...\n\n"
+            f">>> tree = {type(self.tree).__name__}(...)\n"
+            ">>> # indexing by boolean pytree\n"
+            ">>> tree.at[tree > 0].get()\n\n"
+            ">>> # indexing by attribute name\n"
+            ">>> tree.at[`attribute_name`].get()\n\n"
+            ">>> # indexing by attribute index\n"
+            ">>> tree.at[`attribute_index`].get()"
+        )
 
     def get(self, *, is_leaf: Callable[[Any], bool] | None = None) -> PyTree:
-        return _get_at_trace(self.tree, self.where, is_leaf)
+        where = _merge_where(self.tree, self.where, is_leaf)
+        return _get_at_mask(self.tree, where, is_leaf)
 
     def set(
         self,
         set_value: Any,
         *,
         is_leaf: Callable[[Any], bool] | None = None,
     ) -> PyTree:
-        return _set_at_trace(self.tree, self.where, set_value, is_leaf)
+        where = _merge_where(self.tree, self.where, is_leaf)
+        return _set_at_mask(self.tree, where, set_value, is_leaf)
 
     def apply(
         self,
         func: Callable[[Any], Any],
         *,
         is_leaf: Callable[[Any], bool] | None = None,
     ) -> PyTree:
-        return _apply_at_trace(self.tree, self.where, func, is_leaf)
+        where = _merge_where(self.tree, self.where, is_leaf)
+        return _apply_at_mask(self.tree, where, func, is_leaf)
 
     def reduce(
         self,
         func: Callable[[Any, Any], Any],
         *,
         initializer: Any = _no_initializer,
         is_leaf: Callable[[Any], bool] | None = None,
     ) -> Any:
-        return _reduce_at_trace(self.tree, self.where, func, initializer, is_leaf)
-
-    def __call__(self, *a, **k) -> tuple[Any, PyTree]:
-        # return the output of the method called on the attribute
-        # along with the new tree
-        # this method first creates a copy of the tree,
-        # next it unfreezes the tree then calls the method on the attribute
-        # and finally freezes the tree again
-        with _mutable_context(self.tree, kopy=True) as tree:
-            # check if the attribute is a string
-            (method_name,) = self.where
-            if not isinstance(method_name, str):
-                msg = "Expected method name to be a string, "
-                msg += f"Found method_name=`{method_name}` "
-                msg += f"of type={type(method_name).__name__}."
-                raise TypeError(msg)
-
-            method = getattr(tree, method_name)
-            value = method(*a, **k)
-        return value, tree
-
-    def __getitem__(self, rhs_where: tuple[str | int] | PyTree):
-        if isinstance(rhs_where, type(self.tree)):
-            # promote `lhs` name path to boolean mask
-            # and pass to `TreeAtMask`
-            lhs_mask = self.tree != self.tree
-            (lhs_where,) = self.where
-            lhs_mask = lhs_mask.at[lhs_where].set(True)
-            return TreeAtMask(tree=self.tree, where=lhs_mask & rhs_where)
-
-        # case for name/index path rhs
-        rhs_where = (*self.where, rhs_where)
-        return TreeAtTrace(tree=self.tree, where=rhs_where)
+        where = _merge_where(self.tree, self.where, is_leaf)
+        return _reduce_at_mask(self.tree, where, func, initializer, is_leaf)
 
-    def __getattr__(self, name: str) -> TreeAtTrace:
+    def __getattr__(self, name: str) -> AtIndexer:
         # support nested `.at``
         # for example `.at[A].at[B]` represents model.A.B
         if name == "at":
             # pass the current tree and the current path to the next `.at`
-            return TreeAtTrace(tree=self.tree, where=self.where)
+            return AtIndexer(tree=self.tree, where=self.where)
 
         msg = f"{name} is not a valid attribute of {self}\n"
         msg += f"Did you mean to use .at[{name!r}]?"
         raise AttributeError(msg)
 
-
-class AtIndexer(NamedTuple):
-    tree: PyTree
-
-    def __getitem__(self, where: Any) -> TreeAtTrace | TreeAtMask:
-        if isinstance(where, (str, int)):
-            # indexing by name or index
-            # name and index rules are defined using
-            # `register_pytree_node_trace_func`
-            return TreeAtTrace(tree=self.tree, where=(where,))
-
-        if isinstance(where, (type(self.tree), type(...))):
-            # indexing by boolean pytree
-            # Ellipsis as an alias for all elements
-            # model.at[model == model ] <--> model.at[...]
-            return TreeAtMask(tree=self.tree, where=where)
-
-        raise NotImplementedError(
-            f"Indexing with {type(where).__name__} is not implemented.\n"
-            "Example of supported indexing:\n\n"
-            "@pytc.treeclass\n"
-            f"class {type(self.tree).__name__}:\n"
-            "    ...\n\n"
-            f">>> tree = {type(self.tree).__name__}(...)\n"
-            ">>> # indexing by boolean pytree\n"
-            ">>> tree.at[tree > 0].get()\n\n"
-            ">>> # indexing by attribute name\n"
-            ">>> tree.at[`attribute_name`].get()\n\n"
-            ">>> # indexing by attribute index\n"
-            ">>> tree.at[`attribute_index`].get()"
-        )
+    def __call__(self, *a, **k) -> tuple[Any, PyTree]:
+        with _mutable_context(self.tree, kopy=True) as tree:
+            value = _recursive_getattr(tree, self.where)(*a, **k)
+        return value, tree
 
 
 def tree_indexer(tree: PyTree) -> AtIndexer:
     """Adds `.at` indexing abilities to a PyTree.
 
     Example:
         >>> import jax
@@ -468,37 +296,38 @@
         ...     def __repr__(self) -> str:
         ...         return f"{self.__class__.__name__}(a={self.a}, b={self.b})"
 
         >>> # Register the `Tree` class trace function to support indexing
         >>> def test_trace_func(tree):
         ...     names = ("a", "b")
         ...     types = (type(tree.a), type(tree.b))
-        ...     indices = (0, 1)
-        ...     metadatas = (None, None)
-        ...     return [*zip(names, types, indices, metadatas)]
+        ...     indices = (None, None) # use None to indicate that the attribute is not indexable
+        ...     return [*zip(names, types, indices)]
 
         >>> pytc.register_pytree_node_trace(Tree, test_trace_func)
 
         >>> Tree(1, 2).at["a"].get()
         Tree(a=1, b=None)
     """
-    return AtIndexer(tree=tree)
+    return AtIndexer(tree=tree, where=())
 
 
 class BroadcastablePartial(ft.partial):
     def __call__(self, *args, **keywords) -> Callable:
         # https://stackoverflow.com/a/7811270
         keywords = {**self.keywords, **keywords}
         iargs = iter(args)
         args = (next(iargs) if arg is _non_partial else arg for arg in self.args)  # type: ignore
         return self.func(*args, *iargs, **keywords)
 
 
 def bcmap(
-    func: Callable[..., Any], *, is_leaf: Callable[[Any], bool] | None = None
+    func: Callable[..., Any],
+    *,
+    is_leaf: Callable[[Any], bool] | None = None,
 ) -> Callable:
     """(map)s a function over pytrees leaves with automatic (b)road(c)asting for scalar arguments
 
     Args:
         func: the function to be mapped over the pytree
         is_leaf: a function that returns True if the argument is a leaf of the pytree
 
@@ -600,25 +429,25 @@
     def wrapper(self):
         return jtu.tree_map(func, self)
 
     return ft.wraps(func)(wrapper)
 
 
 def _binary_op(func):
-    def wrapper(lhs, rhs=None):
-        if isinstance(rhs, type(lhs)):
-            return jtu.tree_map(func, lhs, rhs)
-        return jtu.tree_map(lambda x: func(x, rhs), lhs)
+    def wrapper(leaf, rhs=None):
+        if isinstance(rhs, type(leaf)):
+            return jtu.tree_map(func, leaf, rhs)
+        return jtu.tree_map(lambda x: func(x, rhs), leaf)
 
     return ft.wraps(func)(wrapper)
 
 
 def _swop(func):
     # swaping the arguments of a two-arg function
-    return ft.wraps(func)(lambda lhs, rhs: func(rhs, lhs))
+    return ft.wraps(func)(lambda leaf, rhs: func(rhs, leaf))
 
 
 def _leafwise_transform(klass: type[T]) -> type[T]:
     # add leafwise transform methods to the class
     # that enable the user to apply a function to
     # all the leaves of the tree
     for key, method in (
@@ -668,24 +497,24 @@
         if key not in vars(klass):
             # do not override any user defined methods
             # this behavior similar is to `dataclasses.dataclass`
             setattr(klass, key, method)
     return klass
 
 
-def _is_lhs_rhs_equal(lhs, rhs) -> bool | jax.Array:
-    if hasattr(lhs, "shape") and hasattr(lhs, "dtype"):
+def _is_leaf_rhs_equal(leaf, rhs) -> bool | jax.Array:
+    if hasattr(leaf, "shape") and hasattr(leaf, "dtype"):
         if hasattr(rhs, "shape") and hasattr(rhs, "dtype"):
-            verdict = jnp.array_equal(lhs, rhs)
+            verdict = jnp.array_equal(leaf, rhs)
             try:
                 return bool(verdict)
             except Exception:
                 return verdict  # fail under `jit`
         return False
-    return lhs == rhs
+    return leaf == rhs
 
 
 def is_tree_equal(*trees: Any) -> bool | jax.Array:
     """Return `True` if all pytrees are equal.
 
     Note:
         trees are compared using their leaves and treedefs.
@@ -700,14 +529,14 @@
     leaves0, treedef0 = jtu.tree_flatten(tree0)
     verdict = True
 
     for tree in rest:
         leaves, treedef = jtu.tree_flatten(tree)
         if (treedef != treedef0) or verdict is False:
             return False
-        verdict = ft.reduce(op.and_, map(_is_lhs_rhs_equal, leaves0, leaves), verdict)
+        verdict = ft.reduce(op.and_, map(_is_leaf_rhs_equal, leaves0, leaves), verdict)
     return verdict
 
 
 def tree_copy(tree: T) -> T:
     """Return a copy of the tree."""
     return jtu.tree_unflatten(*jtu.tree_flatten(tree)[::-1])  # type: ignore
```

### Comparing `pytreeclass-0.2.7/pytreeclass/_src/tree_pprint.py` & `pytreeclass-0.2.8/pytreeclass/_src/tree_pprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import dataclasses as dc
 import functools as ft
 import inspect
 import math
 from collections import defaultdict
 from itertools import chain
 from types import FunctionType
-from typing import Any, Callable, Literal, Sequence
+from typing import Any, Callable, Literal
 
 import jax
 import numpy as np
 from jax._src.custom_derivatives import custom_jvp
 from jax.util import unzip2
 from jaxlib.xla_extension import PjitFunction
 
@@ -349,31 +349,33 @@
 
         >>> print(pytc.tree_str(tree, depth=2))
         {a:1, b:[2, 3], c:{d:4, e:5}, f:[6 7]}
     """
     return _node_pprint(tree, 0, "str", width, depth).expandtabs(tabwidth)
 
 
-def _resolve_names(names: Sequence[str], width: int) -> str:
+def _resolve_names(trace, width: int) -> str:
     # given a trace with a tuple of names, we resolve the names
     # to a single string
-    path, *paths = names
-    for name in paths:
-        path += "" if name.startswith("[") else "."
+    names, _, indices = trace
+    path = ""
+    for i, (name, index) in enumerate(zip(names, indices)):
+        name = f"[{index}]" if name is None else name
+        path += "" if name.startswith("[") else ("." if i > 0 else "")
         path += _node_pprint(name, 0, "str", width, float("inf"))
     return path
 
 
 def _is_trace_leaf_depth_factory(depth: int):
     # generate `is_trace_leaf` function to stop tracing at a certain `depth`
     # in essence, depth is the length of the trace entry
     def is_trace_leaf(trace) -> bool:
         # trace is a tuple of (names, leaves, tracers, aux_data)
         # done like this to ensure 4-tuple unpacking
-        names, _, __, ___ = trace
+        names, _, __ = trace
         # stop tracing if depth is reached
         return False if depth is None else (depth <= len(names))
 
     return is_trace_leaf
 
 
 def tree_indent(
@@ -413,21 +415,23 @@
     seen = set()
 
     for trace, leaf in pytc.tree_leaves_with_trace(
         tree=tree,
         is_leaf=is_leaf,
         is_trace_leaf=_is_trace_leaf_depth_factory(depth),
     ):
-        names, types = trace[0], trace[1]
+        names, types, indices = trace
 
-        for j, (name, type_) in enumerate(zip(names, types)):
-            if names[: j + 1] in seen:
-                continue  # skip printing the common parent node twice
-            seen.add(names[: j + 1])
+        for j, (name, type_, index) in enumerate(zip(names, types, indices)):
+            if (cur := (names[: j + 1], types[: j + 1], indices[: j + 1])) in seen:
+                # skip printing the common parent node twice
+                continue
+            seen.add(cur)
 
+            name = f"[{index}]" if name is None else name
             fmt += "\n" + "\t" * (j + 1)
             fmt += f"{_node_pprint(name,0,'str',width, depth )}"
             fmt += (
                 f"={_node_pprint(leaf,indent=j+1,kind='repr',width=width, depth=depth-1)}"
                 if j == len(names) - 1
                 else f":{type_.__name__}"
             )
@@ -865,20 +869,20 @@
         )
     )
 
     for trace, leaf in zip(traces, leaves):
         count = _calculate_count(leaf)
         COUNT += count
 
-        if trace == ((), (), (), ()):
+        if trace == ((), (), ()):
             # avoid printing the leaf trace (which is the root of the tree)
             # twice, once as a leaf and once as the root at the end
             continue
 
-        paths = _resolve_names(names=trace[0], width=60)
+        paths = _resolve_names(trace, width=60)
         types = _node_type_pprint(leaf, indent=0, kind="str", width=60, depth=depth)
         counts = f"{count:,}"
         ROWS += [[paths, types, counts]]
 
     paths = "Σ"
     types = _node_type_pprint(tree, indent=0, kind="str", width=60, depth=depth)
     counts = f"{COUNT:,}"
```

### Comparing `pytreeclass-0.2.7/pytreeclass/_src/tree_trace.py` & `pytreeclass-0.2.8/pytreeclass/_src/tree_trace.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,16 +22,15 @@
     # class in the `trace` registry
     # get leaves from the `jax` registry
     leaves, _ = _registry.get(type(tree)).to_iter(tree)  # type: ignore
     # TODO: fetch from `jax` key registry once min jax version>=0.4.6
     names = (f"leaf_{i}" for i in range(len(leaves)))
     types = map(type, leaves)
     indices = range(len(leaves))
-    metadatas = (dict(id=id(leaf)) for leaf in leaves)
-    return [*zip(names, types, indices, metadatas)]
+    return [*zip(names, types, indices)]
 
 
 class _TraceRegistryEntry(NamedTuple):
     to_iter: Callable[..., Any]
 
 
 _trace_registry = defaultdict(lambda: _TraceRegistryEntry(_jaxable_trace_func))
@@ -51,34 +50,34 @@
             # check if the trace has the correct format
             if not isinstance(trace, (list, tuple)):
                 msg = "Trace return type is not defined properly for "
                 msg += f"class=`{type(tree).__name__}`."
                 msg += f"Expected a list or tuple, got {trace}"
                 raise TypeError(msg)
 
-            if len(trace) != 4:
+            if len(trace) != 3:
                 msg = "Trace length is not defined properly for "
                 msg += f"class=`{type(tree).__name__}`."
-                msg += "Expected 4 entries, in the order of"
-                msg += f"(name, type, index, metadata), got {trace}"
+                msg += "Expected 3 entries, in the order of"
+                msg += f"(name, type, index), got {trace}"
                 raise ValueError(msg)
 
-            if not isinstance(trace[0], str):
+            if not isinstance(trace[0], (str, type(None))):
                 msg = "Trace name entry is not defined properly for "
                 msg += f"class=`{type(tree).__name__}`."
                 msg += f" Expected a string, got {trace[0]}"
                 raise TypeError(msg)
 
             if not isinstance(trace[1], type):
                 msg = "Trace type entry is not defined properly for "
                 msg += f"class=`{type(tree).__name__}`."
                 msg += f" Expected a type, got {trace[1]}"
                 raise TypeError(msg)
 
-            if not isinstance(trace[2], int):
+            if not isinstance(trace[2], (int, type(None))):
                 msg = "Trace index entry is not defined properly for "
                 msg += f"class=`{type(tree).__name__}`."
                 msg += f" Expected an integer, got {trace[2]}"
                 raise TypeError(msg)
 
         wrapper.has_run = True
         return traces
@@ -91,37 +90,35 @@
     klass: type,
     trace_func: Callable[[Any], list[tuple[str, Any, tuple[int, int], Any]]],
 ) -> None:
     """
     Args:
         klass: The class of the object to be traced.
         trace_func:A function that takes an instance of type `klass` and defines the flatten rule
-            for the object (name, type, index, metadata) for each leaf in the object.
+            for the object (name, type, index) for each leaf in the object.
 
     Example:
         >>> import jax
         >>> import pytreeclass as pytc
         >>> class UserList(list):
         ...     pass
         >>> def user_list_trace_func(tree:UserList):
-        ...     # (1) define name for each leaf
-        ...     names = (f"leaf{i}" for i in range(len(tree)))
+        ...     # (1) define name for each leaf if exists, `None` otherwise
+        ...     names = (None,) * len(tree)
         ...     # (2) define types for each leaf
         ...     types = (type(leaf) for leaf in tree)
-        ...     # (3) index for each leaf in the level
+        ...     # (3) index for each leaf in the level if exists, `None` otherwise
         ...     indices = range(len(tree))
-        ...     # (4) define metadatas (if any) for each leaf
-        ...     metadatas = (() for _ in range(len(tree)))
-        ...     # return a list of tuples (name, type, index, metadata)
-        ...     return [*zip(names, types, indices, metadatas)]
+        ...     # return a list of tuples (name, type, index)
+        ...     return [*zip(names, types, indices)]
         >>> pytc.register_pytree_node_trace(UserList, user_list_trace_func)
 
     Note:
         The `trace_func` should return a list of tuples in the order of
-        (name, type, index, metadata) for each leaf in the object.
+        (name, type, index) for each leaf in the object.
         The format of the trace is validated on the first call and will raise
         `TypeError` or `ValueError` if the format is not correct.
 
     Raises:
         TypeError: if input is not a type
         ValueError: if `klass` is already registered
     """
@@ -132,35 +129,32 @@
         msg = f"Node trace flatten function for {klass} is already registered."
         raise ValueError(msg)
     # register the node trace flatten function to the node trace registry
     _trace_registry[klass] = _TraceRegistryEntry(_validate_trace_func(trace_func))
 
 
 def _sequence_trace_func(tree: Sequence) -> list[TraceType]:
-    names = (f"[{i}]" for i in range(len(tree)))
+    names = (None,) * len(tree)
     types = map(type, tree)
     indices = range(len(tree))
-    metadatas = (dict(id=id(leaf)) for leaf in tree)
-    return [*zip(names, types, indices, metadatas)]
+    return [*zip(names, types, indices)]
 
 
 def _dict_trace_func(tree: dict) -> list[TraceType]:
     names = (f"['{k}']" for k in tree)
     types = (type(tree[key]) for key in tree)
-    indices = range(len(tree))
-    metadatas = (dict(repr=not k.startswith("_"), id=id(tree[k])) for k in tree)
-    return [*zip(names, types, indices, metadatas)]
+    indices = (None,) * len(tree)
+    return [*zip(names, types, indices)]
 
 
 def _namedtuple_trace_func(tree: Any) -> list[TraceType]:
-    names = (f"['{field}']" for field in tree._fields)
+    names = tree._fields
     types = (type(getattr(tree, field)) for field in tree._fields)
     indices = range(len(tree))
-    metadatas = (dict(id=id(getattr(tree, field))) for field in tree._fields)
-    return [*zip(names, types, indices, metadatas)]
+    return [*zip(names, types, indices)]
 
 
 # register trace functions for common types
 register_pytree_node_trace(tuple, _sequence_trace_func)
 register_pytree_node_trace(list, _sequence_trace_func)
 register_pytree_node_trace(dict, _dict_trace_func)
 register_pytree_node_trace(OrderedDict, _dict_trace_func)
@@ -197,15 +191,14 @@
         return
 
     for rhs_trace, leaf in zip(traces, leaves):
         leaf_trace = (
             (*tree_trace[0], rhs_trace[0]),  # names
             (*tree_trace[1], rhs_trace[1]),  # types
             (*tree_trace[2], rhs_trace[2]),  # indices
-            (*tree_trace[3], rhs_trace[3]),  # metadatas
         )
         yield from flatten_one_trace_level(leaf_trace, leaf, is_leaf, is_trace_leaf)
 
 
 def tree_leaves_with_trace(
     tree: PyTree,
     *,
@@ -222,37 +215,16 @@
     Returns:
         A list of (trace, leaf) pairs.
 
     Example:
         >>> import pytreeclass as pytc
         >>> tree = [1, [2, [3]]]
         >>> traces, _ = zip(*pytc.tree_leaves_with_trace(tree))
-        >>> # print(pytc.tree_repr(traces))
-        >>> # (
-        >>> # (('[0]'), (<class 'int'>), (0), ({id:4383785200})),
-        >>> # (
-        >>> #     ('[1]', '[0]'),
-        >>> #     (<class 'list'>, <class 'int'>),
-        >>> #     (1, 0),
-        >>> #     ({id:4558856448}, {id:4383785232})
-        >>> # ),
-        >>> # (
-        >>> #     ('[1]', '[1]', '[0]'),
-        >>> #     (<class 'list'>, <class 'list'>, <class 'int'>),
-        >>> #     (1, 1, 0),
-        >>> #     ({id:4558856448}, {id:4558857472}, {id:4383785264})
-        >>> # )
-        >>> # )
-
-    Note:
-        `metadata` path can hold any information about the object. PyTreeClass stores the object id
-        for the common data structures like `list`, `tuple`, `dict`, `set`, `namedtuple`, and `treeclass` wrapped
-        classes.
     """
-    trace = ((), (), (), ())
+    trace = ((), (), ())
     return list(flatten_one_trace_level(trace, tree, is_leaf, is_trace_leaf))
 
 
 def tree_flatten_with_trace(
     tree: PyTree,
     *,
     is_leaf: Callable[[Any], bool] | None = None,
@@ -291,67 +263,62 @@
 
     Example:
         >>> import jax
         >>> import pytreeclass as pytc
         >>> tree = {"a": [1, 2], "b": 4, "c": [5, 6]}
         >>> # the tree above is visualized as:
         >>> # value tree:
-        >>> #        tree
         >>> #          |
         >>> #    ---------------
         >>> #    |      |      |
         >>> #    |      |      |
         >>> #  ------   4   -------
         >>> #  |    |       |     |
         >>> #  1    2       5     6
 
         >>> # named tree:
-        >>> #        `dict`
         >>> #          |
         >>> #    ---------------
         >>> #    |      |      |
         >>> # `['a']` `['b']``['c']`
         >>> #    |             |
         >>> #  ------       -------
         >>> #  |    |       |     |
         >>> #`[0]``[1]`   `[0]` `[1]`
 
         >>> # type tree:
-        >>> #        <dict>
         >>> #          |
         >>> #    ---------------
         >>> #    |      |      |
         >>> #  <list> <int> <list>
         >>> #    |             |
         >>> #  ------       -------
         >>> #  |    |       |     |
         >>> # <int><int>   <int><int>
 
         >>> # index tree:
-        >>> #          0
         >>> #          |
         >>> #    ---------------
         >>> #    |      |      |
         >>> #    0      1      2
         >>> #    |             |
         >>> #  ------       -------
         >>> #  |    |       |     |
         >>> #  0    1       0     1
 
-
         >>> def map_func(trace, leaf):
-        ...    names, _, __, ___ = trace
+        ...    names, _, __ = trace
         ...    if "['a']" in names:
         ...        return leaf + 100
         ...    return leaf
         >>> pytc.tree_map_with_trace(map_func, tree)
         {'a': [101, 102], 'b': 4, 'c': [5, 6]}
 
         >>> def map_func(trace, leaf):
-        ...    _, types, __, ___ = trace
+        ...    _, types, __ = trace
         ...    if list in types:
         ...        return leaf + 100
         ...    return leaf
         >>> pytc.tree_map_with_trace(map_func, tree)
         {'a': [101, 102], 'b': 4, 'c': [105, 106]}
     """
     traces_leaves, treedef = tree_flatten_with_trace(tree, is_leaf=is_leaf)
```

### Comparing `pytreeclass-0.2.7/pytreeclass.egg-info/PKG-INFO` & `pytreeclass-0.2.8/pytreeclass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytreeclass
-Version: 0.2.7
+Version: 0.2.8
 Summary: JAX compatible dataclass.
 Home-page: https://github.com/ASEM000/pytreeclass
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: Apache-2.0
 Keywords: python machine-learning pytorch jax
 Classifier: Development Status :: 5 - Production/Stable
@@ -461,15 +461,15 @@
 
 </details>
 
 ## ➕ More<a id="more"></a>
 
 <details><summary>[Advanced] Register custom user-defined classes to work with visualization and indexing tools. </summary>
 
-Similar to [`jax.tree_util.register_pytree_node`](https://jax.readthedocs.io/en/latest/pytrees.html#extending-pytrees), `PyTreeClass` register common data structures and `treeclass` wrapped classes to figure out how to define the names, types, index, and metadatas of certain leaf along its path.
+Similar to [`jax.tree_util.register_pytree_node`](https://jax.readthedocs.io/en/latest/pytrees.html#extending-pytrees), `PyTreeClass` register common data structures and `treeclass` wrapped classes to figure out how to define the names, types, and index of certain leaf along its path.
 
 Here is an example of registering
 
 ```python
 
 class Tree:
     def __init__(self, a, b):
@@ -486,19 +486,18 @@
 
 # jax unflatten rule
 def tree_unflatten(_, children):
     return Tree(*children)
 
 # PyTreeClass flatten rule
 def pytc_tree_flatten(tree):
-    names = ("a", "b")
+    names = ("a", "b") # or (`None`, `None`) if name is not defined
     types = (type(tree.a), type(tree.b))
-    indices = (0,1)
-    metadatas = (None, None)
-    return [*zip(names, types, indices, metadatas)]
+    indices = (0,1)  # or (`None`, `None`) if index is not defined
+    return [*zip(names, types, indices)]
 
 
 # Register with `jax`
 jax.tree_util.register_pytree_node(Tree, tree_flatten, tree_unflatten)
 
 # Register the `Tree` class trace function to support indexing
 pytc.register_pytree_node_trace(Tree, pytc_tree_flatten)
@@ -834,17 +833,16 @@
     @property
     def at(self):
         return pytc.tree_indexer(self)
 
 def pytc_flatten_rule(tree):
     names =("a","b","c")
     types = map(type, (tree.a, tree.b, tree.c))
-    indices = range(3)
-    metadatas= (None, None, None)
-    return [*zip(names, types, indices, metadatas)]
+    indices = range(3)  # make it indexable like namedtuple
+    return [*zip(names, types, indices)]
 
 pytc.register_pytree_node_trace(FlaxTree, pytc_flatten_rule)
 
 flax_tree = FlaxTree()
 
 print(f"{flax_tree!r}")
 # FlaxTree(a=1, b=(2.0, 3.0), c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00]))
@@ -905,15 +903,15 @@
 </details>
 
 <details> 
 <summary>Use tree_map_with_trace</summary>
 
 V0.2 of `PyTreeClass` register common python datatypes and `treeclass` wrapped class to `trace` registry.
 While `jax` uses `jax.tree_util.register_pytree_node` to define `flatten_rule` for leaves, `PyTreeClass` extends on this
-By registering the `flatten_rule` of (1) names, (2) types, (3) indexing, (4) metadata -if exists-
+By registering the `flatten_rule` of (1) names, (2) types, (3) indexing
 
 For demonstration , the following figure contains the 4 variants of the same `Tree` instance define
 
 ```python
 import jax
 import jax.numpy as jnp
 import pytreeclass as pytc
```

### Comparing `pytreeclass-0.2.7/pytreeclass.egg-info/SOURCES.txt` & `pytreeclass-0.2.8/pytreeclass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.7/setup.py` & `pytreeclass-0.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.7/tests/test_indexing.py` & `pytreeclass-0.2.8/tests/test_indexing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import functools as ft
+from collections import namedtuple
 
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import numpy.testing as npt
 import pytest
 
@@ -448,23 +449,23 @@
         a: int = 1
         b: l0 = l0()
 
     t = Tree()
     assert pytc.is_tree_equal(t.at[0].get(), Tree(1, l0(None)))
     assert pytc.is_tree_equal(t.at[1].at[0].get(), Tree(None, l0(2)))
 
-    with pytest.raises(IndexError):
-        t.at[0].at[1].get()
+    # with pytest.raises(IndexError):
+    #     t.at[0].at[1].get()
 
-    with pytest.raises(IndexError):
-        t.at[0].at[1].set(10)
-    with pytest.raises(IndexError):
-        t.at[0].at[1].apply(lambda _: 10)
-    with pytest.raises(IndexError):
-        t.at[0].at[1].reduce(lambda _, __: 10)
+    # with pytest.raises(IndexError):
+    #     t.at[0].at[1].set(10)
+    # with pytest.raises(IndexError):
+    #     t.at[0].at[1].apply(lambda _: 10)
+    # with pytest.raises(IndexError):
+    #     t.at[0].at[1].reduce(lambda _, __: 10)
 
 
 def test_trace_set():
     @ft.partial(pytc.treeclass, leafwise=True)
     class l0:
         a: int = 2
 
@@ -524,16 +525,16 @@
         a: int = 1
         b: l0 = l0()
 
     t = Tree()
     assert pytc.is_tree_equal(t.at[1].at[t == 2].get(), Tree(None, l0(2, None)))
     assert pytc.is_tree_equal(t.at[t == 2].at[1].get(), Tree(None, l0(2, None)))
 
-    with pytest.raises(IndexError):
-        t.at[0].at[2].get()
+    # with pytest.raises(IndexError):
+    #     t.at[0].at[2].get()
 
 
 def test_mixed_set():
     @ft.partial(pytc.treeclass, leafwise=True)
     class l0:
         a: int = 2
         b: int = 1
@@ -547,16 +548,16 @@
 
     assert pytc.is_tree_equal(t.at["b"].at[t == 2].set(100), Tree(1, l0(100)))
     assert pytc.is_tree_equal(t.at[t == 2].at["b"].set(100), Tree(1, l0(100)))
     assert pytc.is_tree_equal(t.at[1].at[t == 2].set(100), Tree(1, l0(100)))
     assert pytc.is_tree_equal(t.at[t == 2].at[1].set(100), Tree(1, l0(100)))
     assert pytc.is_tree_equal(t.at["b"].at[0].set(100), Tree(1, l0(100)))
 
-    with pytest.raises(IndexError):
-        assert pytc.is_tree_equal(t.at[0].at["b"].set(100), Tree(1, l0(100, 2)))
+    # with pytest.raises(IndexError):
+    #     assert pytc.is_tree_equal(t.at[0].at["b"].set(100), Tree(1, l0(100, 2)))
 
 
 def test_mixed_apply():
     @ft.partial(pytc.treeclass, leafwise=True)
     class l0:
         a: int = 2
         b: int = 1
@@ -567,29 +568,37 @@
         b: l0 = l0()
 
     t = Tree()
 
     assert pytc.is_tree_equal(t.at[1].at[t == 2].apply(lambda _: 100), Tree(1, l0(100)))
     assert pytc.is_tree_equal(t.at["b"].at[0].apply(lambda _: 100), Tree(1, l0(100)))
 
-    with pytest.raises(IndexError):
-        t.at[0].at["a"].apply(lambda _: 100), Tree(1, l0(100))
+    # with pytest.raises(IndexError):
+    #     t.at[0].at["a"].apply(lambda _: 100), Tree(1, l0(100))
 
 
 def test_method_call():
     @ft.partial(pytc.treeclass, leafwise=True)
     class Tree:
         a: int = 1
 
         def increment(self):
             self.a += 1
 
+        def show(self):
+            return 1
+
     t = Tree()
 
+    @pytc.treeclass
+    class Tree2:
+        b: Tree = Tree()
+
     assert pytc.is_tree_equal(t.at["increment"]()[1], Tree(2))
+    assert pytc.is_tree_equal(Tree2().at["b"].at["show"]()[0], 1)
 
     with pytest.raises(AttributeError):
         t.at["bla"]()
 
     with pytest.raises(TypeError):
         t.at["a"]()
 
@@ -634,17 +643,17 @@
     @ft.partial(pytc.treeclass, leafwise=True)
     class Tree:
         a: int = 1
         b: int = 2
 
     t = Tree()
 
-    assert repr(t.at["a"]) == "TreeAtTrace(tree=Tree(a=1, b=2), where=('a',))"
-    assert str(t.at["a"]) == "TreeAtTrace(tree=Tree(a=1, b=2), where=('a',))"
-    assert repr(t.at[...]) == "TreeAtMask(tree=Tree(a=1, b=2), where=Ellipsis)"
+    assert repr(t.at["a"]) == "AtIndexer(tree=Tree(a=1, b=2), where=('a',))"
+    assert str(t.at["a"]) == "AtIndexer(tree=Tree(a=1, b=2), where=('a',))"
+    assert repr(t.at[...]) == "AtIndexer(tree=Tree(a=1, b=2), where=(Ellipsis,))"
 
 
 def test_not_equal():
     @ft.partial(pytc.treeclass, leafwise=True)
     class Tree:
         a: int = 1
         b: float = 1.0
@@ -705,7 +714,21 @@
 
 def test_register_pytree_node_trace():
     with pytest.raises(TypeError):
         pytc.register_pytree_node_trace(None, None)
 
     with pytest.raises(ValueError):
         pytc.register_pytree_node_trace(list, lambda x: x)
+
+
+def test_mixed_not_implemented():
+    @pytc.treeclass
+    class T:
+        a: tuple[int, ...] = namedtuple("a", ["x", "y"])(1, 2)
+
+    t = T()
+
+    with pytest.raises(NotImplementedError):
+        t.at["a"].at[[1]].get()
+
+    with pytest.raises(NotImplementedError):
+        t.at[0].at[[1]].get()
```

### Comparing `pytreeclass-0.2.7/tests/test_nn.py` & `pytreeclass-0.2.8/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.7/tests/test_tree_freeze.py` & `pytreeclass-0.2.8/tests/test_tree_freeze.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.7/tests/test_tree_operator.py` & `pytreeclass-0.2.8/tests/test_tree_operator.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.7/tests/test_tree_pprint.py` & `pytreeclass-0.2.8/tests/test_tree_pprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         == "┌────┬────────────┬─────┐\n│Name│Type        │Count│\n├────┼────────────┼─────┤\n│a   │int         │1    │\n├────┼────────────┼─────┤\n│b   │str         │1    │\n├────┼────────────┼─────┤\n│c   │float       │1    │\n├────┼────────────┼─────┤\n│d   │str         │1    │\n├────┼────────────┼─────┤\n│e   │list        │1    │\n├────┼────────────┼─────┤\n│f   │set         │1    │\n├────┼────────────┼─────┤\n│g   │dict        │1    │\n├────┼────────────┼─────┤\n│h   │f32[5,1]    │5    │\n├────┼────────────┼─────┤\n│i   │f32[1,6]    │6    │\n├────┼────────────┼─────┤\n│j   │f32[1,1,4,5]│20   │\n├────┼────────────┼─────┤\n│k   │tuple       │1    │\n├────┼────────────┼─────┤\n│l   │a           │1    │\n├────┼────────────┼─────┤\n│m   │f32[5,5]    │25   │\n├────┼────────────┼─────┤\n│n   │bool[0]     │1    │\n├────┼────────────┼─────┤\n│o   │c64[2]      │2    │\n├────┼────────────┼─────┤\n│Σ   │Repr1       │68   │\n└────┴────────────┴─────┘"
     )
 
     assert (
         tree_summary(r1, depth=2)
         == tree_summary(r1)
         # trunk-ignore(flake8/E501)
-        == "┌──────┬────────────┬─────┐\n│Name  │Type        │Count│\n├──────┼────────────┼─────┤\n│a     │int         │1    │\n├──────┼────────────┼─────┤\n│b     │str         │1    │\n├──────┼────────────┼─────┤\n│c     │float       │1    │\n├──────┼────────────┼─────┤\n│d     │str         │1    │\n├──────┼────────────┼─────┤\n│e[0]  │int         │1    │\n├──────┼────────────┼─────┤\n│e[1]  │int         │1    │\n├──────┼────────────┼─────┤\n│e[2]  │int         │1    │\n├──────┼────────────┼─────┤\n│e[3]  │int         │1    │\n├──────┼────────────┼─────┤\n│e[4]  │int         │1    │\n├──────┼────────────┼─────┤\n│f     │set         │1    │\n├──────┼────────────┼─────┤\n│g['a']│str         │1    │\n├──────┼────────────┼─────┤\n│g['b']│str         │1    │\n├──────┼────────────┼─────┤\n│g['c']│f32[5,5]    │25   │\n├──────┼────────────┼─────┤\n│h     │f32[5,1]    │5    │\n├──────┼────────────┼─────┤\n│i     │f32[1,6]    │6    │\n├──────┼────────────┼─────┤\n│j     │f32[1,1,4,5]│20   │\n├──────┼────────────┼─────┤\n│k[0]  │int         │1    │\n├──────┼────────────┼─────┤\n│k[1]  │int         │1    │\n├──────┼────────────┼─────┤\n│k[2]  │int         │1    │\n├──────┼────────────┼─────┤\n│l['b']│int         │1    │\n├──────┼────────────┼─────┤\n│l['c']│int         │1    │\n├──────┼────────────┼─────┤\n│m     │f32[5,5]    │25   │\n├──────┼────────────┼─────┤\n│n     │bool[0]     │1    │\n├──────┼────────────┼─────┤\n│o     │c64[2]      │2    │\n├──────┼────────────┼─────┤\n│Σ     │Repr1       │101  │\n└──────┴────────────┴─────┘"
+        == "┌──────┬────────────┬─────┐\n│Name  │Type        │Count│\n├──────┼────────────┼─────┤\n│a     │int         │1    │\n├──────┼────────────┼─────┤\n│b     │str         │1    │\n├──────┼────────────┼─────┤\n│c     │float       │1    │\n├──────┼────────────┼─────┤\n│d     │str         │1    │\n├──────┼────────────┼─────┤\n│e[0]  │int         │1    │\n├──────┼────────────┼─────┤\n│e[1]  │int         │1    │\n├──────┼────────────┼─────┤\n│e[2]  │int         │1    │\n├──────┼────────────┼─────┤\n│e[3]  │int         │1    │\n├──────┼────────────┼─────┤\n│e[4]  │int         │1    │\n├──────┼────────────┼─────┤\n│f     │set         │1    │\n├──────┼────────────┼─────┤\n│g['a']│str         │1    │\n├──────┼────────────┼─────┤\n│g['b']│str         │1    │\n├──────┼────────────┼─────┤\n│g['c']│f32[5,5]    │25   │\n├──────┼────────────┼─────┤\n│h     │f32[5,1]    │5    │\n├──────┼────────────┼─────┤\n│i     │f32[1,6]    │6    │\n├──────┼────────────┼─────┤\n│j     │f32[1,1,4,5]│20   │\n├──────┼────────────┼─────┤\n│k[0]  │int         │1    │\n├──────┼────────────┼─────┤\n│k[1]  │int         │1    │\n├──────┼────────────┼─────┤\n│k[2]  │int         │1    │\n├──────┼────────────┼─────┤\n│l.b   │int         │1    │\n├──────┼────────────┼─────┤\n│l.c   │int         │1    │\n├──────┼────────────┼─────┤\n│m     │f32[5,5]    │25   │\n├──────┼────────────┼─────┤\n│n     │bool[0]     │1    │\n├──────┼────────────┼─────┤\n│o     │c64[2]      │2    │\n├──────┼────────────┼─────┤\n│Σ     │Repr1       │101  │\n└──────┴────────────┴─────┘"
     )
 
 
 def _tree_to_indent(str):
     return str.replace("├── ", "    ").replace("└── ", "    ").replace("│", " ")
 
 
@@ -152,15 +152,15 @@
         tree_mermaid(r1, depth=1)
         # trunk-ignore(flake8/E501)
         == 'flowchart LR\n    id0(<b>Repr1</b>)\n    id0 --- id1("</b>a=1</b>")\n    id0 --- id2("</b>b=\'string\'</b>")\n    id0 --- id3("</b>c=1.0</b>")\n    id0 --- id4("</b>d=\'aaaaa\'</b>")\n    id0 --- id5("</b>e=[...]</b>")\n    id0 --- id6("</b>f={...}</b>")\n    id0 --- id7("</b>g={...}</b>")\n    id0 --- id8("</b>h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id9("</b>i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id10("</b>j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id11("</b>k=(...)</b>")\n    id0 --- id12("</b>l=a(...)</b>")\n    id0 --- id13("</b>m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id14("</b>n=bool[0]</b>")\n    id0 --- id15("</b>o=c64[2]</b>")\n'
     )
     assert (
         tree_mermaid(r1, depth=2)
         # trunk-ignore(flake8/E501)
-        == 'flowchart LR\n    id5 --- id6("</b>[0]=10</b>")\n    id5 --- id7("</b>[1]=10</b>")\n    id5 --- id8("</b>[2]=10</b>")\n    id5 --- id9("</b>[3]=10</b>")\n    id5 --- id10("</b>[4]=10</b>")\n    id12 --- id13("</b>[\'a\']=\'aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa\'</b>")\n    id12 --- id14("</b>[\'b\']=\'bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb\'</b>")\n    id12 --- id15("</b>[\'c\']=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id19 --- id20("</b>[0]=1</b>")\n    id19 --- id21("</b>[1]=2</b>")\n    id19 --- id22("</b>[2]=3</b>")\n    id23 --- id24("</b>[\'b\']=1</b>")\n    id23 --- id25("</b>[\'c\']=2</b>")\n    id0(<b>Repr1</b>)\n    id0 --- id1("</b>a=1</b>")\n    id0 --- id2("</b>b=\'string\'</b>")\n    id0 --- id3("</b>c=1.0</b>")\n    id0 --- id4("</b>d=\'aaaaa\'</b>")\n    id0 --- id5("</b>e:list</b>")\n    id0 --- id11("</b>f={1, 2, 3}</b>")\n    id0 --- id12("</b>g:dict</b>")\n    id0 --- id16("</b>h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id17("</b>i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id18("</b>j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id19("</b>k:tuple</b>")\n    id0 --- id23("</b>l:a</b>")\n    id0 --- id26("</b>m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id27("</b>n=bool[0]</b>")\n    id0 --- id28("</b>o=c64[2]</b>")\n'
+        == 'flowchart LR\n    id5 --- id6("</b>[0]=10</b>")\n    id5 --- id7("</b>[1]=10</b>")\n    id5 --- id8("</b>[2]=10</b>")\n    id5 --- id9("</b>[3]=10</b>")\n    id5 --- id10("</b>[4]=10</b>")\n    id12 --- id13("</b>[\'a\']=\'aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa\'</b>")\n    id12 --- id14("</b>[\'b\']=\'bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb\'</b>")\n    id12 --- id15("</b>[\'c\']=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id19 --- id20("</b>[0]=1</b>")\n    id19 --- id21("</b>[1]=2</b>")\n    id19 --- id22("</b>[2]=3</b>")\n    id23 --- id24("</b>b=1</b>")\n    id23 --- id25("</b>c=2</b>")\n    id0(<b>Repr1</b>)\n    id0 --- id1("</b>a=1</b>")\n    id0 --- id2("</b>b=\'string\'</b>")\n    id0 --- id3("</b>c=1.0</b>")\n    id0 --- id4("</b>d=\'aaaaa\'</b>")\n    id0 --- id5("</b>e:list</b>")\n    id0 --- id11("</b>f={1, 2, 3}</b>")\n    id0 --- id12("</b>g:dict</b>")\n    id0 --- id16("</b>h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id17("</b>i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id18("</b>j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id19("</b>k:tuple</b>")\n    id0 --- id23("</b>l:a</b>")\n    id0 --- id26("</b>m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id27("</b>n=bool[0]</b>")\n    id0 --- id28("</b>o=c64[2]</b>")\n'
     )
 
 
 def test_misc():
     x = (1, 2, 3)
     assert tree_repr(x) == tree_str(x) == "(1, 2, 3)"
```

### Comparing `pytreeclass-0.2.7/tests/test_tree_viz_util.py` & `pytreeclass-0.2.8/tests/test_tree_viz_util.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.7/tests/test_treeclass.py` & `pytreeclass-0.2.8/tests/test_treeclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -589,16 +589,15 @@
     class T:
         def __init__(self):
             self.a = 1
 
     def trace_func(tree):
         names = ("a",)
         types = (type(tree.a),)
-        indices = (0,)
-        return [*zip(names, types, indices)]
+        return [*zip(names, types)]
 
     flatten_func = lambda tree: ((tree.a,), None)
     unflatten_func = lambda _, x: T(x)
 
     jax.tree_util.register_pytree_node(T, flatten_func, unflatten_func)
 
     pytc.register_pytree_node_trace(T, trace_func)
@@ -611,16 +610,15 @@
         def __init__(self):
             self.a = 1
 
     def trace_func(tree):
         names = (1,)
         types = (type(tree.a),)
         indices = (0,)
-        metadatas = (None,)
-        return [*zip(names, types, indices, metadatas)]
+        return [*zip(names, types, indices)]
 
     flatten_func = lambda tree: ((tree.a,), None)
     unflatten_func = lambda _, x: T(x)
 
     jax.tree_util.register_pytree_node(T, flatten_func, unflatten_func)
 
     pytc.register_pytree_node_trace(T, trace_func)
@@ -633,16 +631,15 @@
         def __init__(self):
             self.a = 1
 
     def trace_func(tree):
         names = ("a",)
         types = (1,)
         indices = (0,)
-        metadatas = (None,)
-        return [*zip(names, types, indices, metadatas)]
+        return [*zip(names, types, indices)]
 
     flatten_func = lambda tree: ((tree.a,), None)
     unflatten_func = lambda _, x: T(x)
 
     jax.tree_util.register_pytree_node(T, flatten_func, unflatten_func)
 
     pytc.register_pytree_node_trace(T, trace_func)
@@ -655,16 +652,15 @@
         def __init__(self):
             self.a = 1
 
     def trace_func(tree):
         names = ("a",)
         types = (int,)
         indices = ("a",)
-        metadatas = (None,)
-        return [*zip(names, types, indices, metadatas)]
+        return [*zip(names, types, indices)]
 
     flatten_func = lambda tree: ((tree.a,), None)
     unflatten_func = lambda _, x: T(x)
 
     jax.tree_util.register_pytree_node(T, flatten_func, unflatten_func)
 
     pytc.register_pytree_node_trace(T, trace_func)
@@ -696,16 +692,15 @@
         def __init__(self):
             self.a = 1
 
     def trace_func(tree):
         names = ("a",)
         types = (int,)
         indices = (0,)
-        metadatas = (None,)
-        return [*zip(names, types, indices, metadatas)]
+        return [*zip(names, types, indices)]
 
     flatten_func = lambda tree: ((tree.a,), None)
     unflatten_func = lambda _, x: T(x)
 
     jax.tree_util.register_pytree_node(T, flatten_func, unflatten_func)
 
     pytc.register_pytree_node_trace(T, trace_func)
@@ -759,7 +754,15 @@
 
 def test_field_repr():
     assert (
         repr(pytc.field())
         # trunk-ignore(flake8/E501)
         == "Field(\n  name=None, \n  type=None, \n  default=?, \n  factory=None, \n  init=True, \n  repr=True, \n  kw_only=False, \n  pos_only=False, \n  metadata=None, \n  callbacks=(), \n  alias=None\n)"
     )
+
+
+def test_field_factory():
+    @pytc.treeclass
+    class Tree:
+        a: int = pytc.field(factory=lambda: 1)
+
+    assert Tree().a == 1
```

### Comparing `pytreeclass-0.2.7/tests/test_under_jit.py` & `pytreeclass-0.2.8/tests/test_under_jit.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 import pytreeclass as pytc
 
 
 def test_jit_freeze():
     @ft.partial(pytc.treeclass, leafwise=True)
     class Linear:
-        weight: jnp.ndarray
-        bias: jnp.ndarray
+        weight: jax.Array
+        bias: jax.Array
         name: str
 
         def __init__(self, key, in_dim, out_dim):
             self.weight = jax.random.normal(key, shape=(in_dim, out_dim)) * jnp.sqrt(
                 2 / in_dim
             )
             self.bias = jnp.ones((1, out_dim))
@@ -105,45 +105,47 @@
     for _ in range(2):
         value, model = train_step(x, y, epochs=20_000)
 
 
 def test_ops_with_jit():
     @ft.partial(pytc.treeclass, leafwise=True)
     class T0:
-        a: int = 1
-        b: int = 2
-        c: int = 3
+        a: jax.Array = jnp.array(1)
+        b: jax.Array = jnp.array(2)
+        c: jax.Array = jnp.array(3)
 
     @ft.partial(pytc.treeclass, leafwise=True)
     class T1:
-        a: int = 1
-        b: int = 2
-        c: int = 3
-        d: jnp.ndarray = pytc.field(factory=lambda: jnp.array([1, 2, 3]))
+        a: jax.Array = jnp.array(1)
+        b: jax.Array = jnp.array(2)
+        c: jax.Array = jnp.array(3)
+        d: jax.Array = jnp.array([1, 2, 3])
 
     @jax.jit
     def getter(tree):
         return tree.at[...].get()
 
     @jax.jit
     def setter(tree):
         return tree.at[...].set(0)
 
     @jax.jit
     def applier(tree):
         return tree.at[...].apply(lambda _: 0)
 
     with pytest.raises(jax.errors.ConcretizationTypeError):
-        getter(T0())
+        pytc.is_tree_equal(getter(T0()), T0())
 
     assert pytc.is_tree_equal(T0(0, 0, 0), setter(T0()))
 
     assert pytc.is_tree_equal(T0(0, 0, 0), applier(T0()))
 
     with pytest.raises(jax.errors.ConcretizationTypeError):
-        getter(T1())
+        pytc.is_tree_equal(getter(T1()), T1())
 
-    assert pytc.is_tree_equal(T1(0, 0, 0, jnp.array([0, 0, 0])), setter(T1()))
+    assert pytc.is_tree_equal(
+        T1(jnp.array(0), jnp.array(0), jnp.array(0), jnp.array([0, 0, 0])), setter(T1())
+    )
 
     assert pytc.is_tree_equal(T1(0, 0, 0, jnp.array([0, 0, 0])), applier(T1()))
 
     assert jax.jit(pytc.is_tree_equal)(T1(0, 0, 0, jnp.array([0, 0, 0])), applier(T1()))
```

