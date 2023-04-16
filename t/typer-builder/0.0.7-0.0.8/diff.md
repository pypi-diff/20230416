# Comparing `tmp/typer_builder-0.0.7.tar.gz` & `tmp/typer_builder-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_builder-0.0.7.tar", max compression
+gzip compressed data, was "typer_builder-0.0.8.tar", max compression
```

## Comparing `typer_builder-0.0.7.tar` & `typer_builder-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      998 2023-03-05 04:09:53.796929 typer_builder-0.0.7/LICENSE
--rw-r--r--   0        0        0     1279 2023-04-16 10:19:38.985826 typer_builder-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3348 2023-04-16 10:20:13.900839 typer_builder-0.0.7/readme.md
--rw-r--r--   0        0        0      273 2023-04-01 00:05:47.241262 typer_builder-0.0.7/src/typer_builder/__init__.py
--rw-r--r--   0        0        0     4984 2023-03-26 00:18:10.619884 typer_builder-0.0.7/src/typer_builder/_build.py
--rw-r--r--   0        0        0      658 2023-04-16 10:21:00.319527 typer_builder-0.0.7/src/typer_builder/_build_test.py
--rw-r--r--   0        0        0     6158 2023-03-23 10:04:44.887366 typer_builder-0.0.7/src/typer_builder/_injector.py
--rw-r--r--   0        0        0        0 2023-03-05 04:09:53.800929 typer_builder-0.0.7/src/typer_builder/py.typed
--rw-r--r--   0        0        0     4036 1970-01-01 00:00:00.000000 typer_builder-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      998 2023-03-05 04:09:53.796929 typer_builder-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1602 2023-04-16 14:13:46.762430 typer_builder-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3623 2023-04-16 14:11:14.594706 typer_builder-0.0.8/readme.md
+-rw-r--r--   0        0        0    10293 2023-04-16 14:07:29.485030 typer_builder-0.0.8/src/typer_builder/Dependencies.py
+-rw-r--r--   0        0        0     2496 2023-04-16 14:04:36.241894 typer_builder-0.0.8/src/typer_builder/Dependencies_test.py
+-rw-r--r--   0        0        0      330 2023-04-16 14:13:46.762430 typer_builder-0.0.8/src/typer_builder/__init__.py
+-rw-r--r--   0        0        0     4964 2023-04-16 14:04:06.414731 typer_builder-0.0.8/src/typer_builder/build_app.py
+-rw-r--r--   0        0        0      661 2023-04-16 14:04:16.258455 typer_builder-0.0.8/src/typer_builder/build_app_test.py
+-rw-r--r--   0        0        0        0 2023-03-05 04:09:53.800929 typer_builder-0.0.8/src/typer_builder/py.typed
+-rw-r--r--   0        0        0     4520 1970-01-01 00:00:00.000000 typer_builder-0.0.8/PKG-INFO
```

### Comparing `typer_builder-0.0.7/LICENSE` & `typer_builder-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `typer_builder-0.0.7/readme.md` & `typer_builder-0.0.8/readme.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,42 @@
 # typer-builder
 
   [Typer]: https://typer.tiangolo.com/
+  [pep585]: https://www.python.org/dev/peps/pep-0585/
+  [pep604]: https://www.python.org/dev/peps/pep-0604/
+  [typeapi]: https://github.com/NiklasRosenstein/python-typeapi
 
-This package allows you to easily build a [Typer][] CLI application from a Python module hierarchy.
+A framework for simplifying the development of [Typer][] based CLIs supporting modern type hints and hierarchical
+dependency injection. 
 
-### Quickstart
+__Table of Contents__
+
+* [Introduction](#introduction)
+  * [Example](#example)
+* [Documentation](#documentation)
+  * [New-style type hint support](#new-style-type-hint-support)
+  * [Dependency injection](#dependency-injection)
+
+
+## Introduction
+
+The `build_app_from_module()` inspect a hierarchy of Python modules to build a Typer command and group structure.
+Packages are treated as command groups and may define a `callback()` member. Modules are treated commands and must
+define a `main()` member. Modules and packages prefixed with an underscore ( `_` ) are ignored. Help text is extracted
+from the `main()` docstring or the module docstring.
+
+In addition, we provide support for new-style type hints ([PEP 585 - Type Hinting Generics in Standard Collections][pep585]
+and [PEP 604 - Union Operators][pep604]) in older versions of Python as well as adapt it for Typer (e.g. `list[str]`
+and `str | None`), as well as a method of injecting dependencies to functions that are not sourced from the command-line.
+
+
+### Example
 
 ```
-$ tree src/mypackage/commands/
+$ tree src/mypackage/
 src/mypackage/
 ├── __init__.py
 ├── __main__.py
 └── commands
     ├── __init__.py
     ├── hello.py
     └── bye.py
@@ -28,73 +53,45 @@
 from typer_builder import build_app_from_module
 
 if __name__ == "__main__":
     app = build_app_from_module("mypackage.commands")
     app()
 ```
 
-### Features
 
-* Packages are treated as command groups and _may_ define a `def callback(): ...` (see `Typer.add_callback()`).
-* Modules are treated as commands and _must_ define a `def main(): ...` (see `Typer.command()`).
-* Underscores in package or module names are normalized to hyphens (e.g `my_command` -> `my-command`).
-* Command(-group) help text is extracted from the package or module docstring, or from the `main()` docstring.
-* [WIP] Improved and dynamic dependency injection.
-* Support for new-style type hints in older versions of Python and Typer (e.g. `str | None`).
-
-### Dependency Injection
-
-The `typer_builder.DependencyInjector` is essentially a mapping of types to a corresponding implementation. It allows
-you to bind any function to the given dependencies based on the function signature.
-
-The `build_app_from_module()` takes a `dependencies` argument which populates a `DependencyInjector`. All `callback()`
-and `main()` functions encountered and added to a `typer.Typer` object are first bound to the dependencies that can be
-served by the injector.
-
-The types for which injection can take place must be known in advance. If the implementation is not known in advance,
-a `callback()` can accept the `DependencyInjector` as an argument and inform about the dependencies that will be
-provided by the callback, allowing any of its subcommands to resolve it.
+## Documentation
 
-```py
-# src/mypackages/commands/__init__.py
-"""
-This is a cool CLI that uses typer-builder.
-"""
-
-from mypackage.config import CliConfig
-from pathlib import Path
-from typer_builder import DependencyInjector, DelayedBinding
-from typer import Option
-
-def callback(
-    config_file: Path = Option(Path("~/.config/mypackage.ini"), help="Path to the configuration file."),
-    dependencies: DependencyInjector = DelayedBinding(CliConfig),
-) -> None:
-    dependencies.register_supplier(CliConfig, lambda: CliConfig.load(config_file))
-```
+### New-style type hint support
+
+Through [`typeapi`][typeapi], we can convert new-tyle type hints such as `str | None` or `list[int]` to their corresponding
+representation using `typing` before the function signature is parsed by [Typer][].
 
 ```py
-# src/mypackage/commands/hello.py
-from mypackage.config import CliConfig
+# src/mypackage/commands/create_user.py
+from ___future__ import annotations
 
-def main(name: str, config: CliConfig) -> None:
+def main(name: str | None = None, groups: list[str] | None = None) -> None:
     # ...
 ```
 
-In the above example, the `config` parameter is not passed by [Typer][], but instead by the `DependencyInjector` per the implementation in the previous `callback()` snippet.
+[`typeapi`][typeapi] also allows us to convert `list[str]` to `List[str]` and `dict[str, int]` to `Dict[str, int]` for
+Python versions prior to 3.9. This is necessary because [Typer][] does not support the new-style type hints.
 
-__Known caveats__
+### Dependency injection
 
-* Only concrete types are supported (no `Optional[CliConfig]` or vice versa).
+The `typer_builder.Dependencies` object is used to map types to concrete values or functions that provide them.
+Functions wrapped with `Dependencies.bind()` will have their arguments resolved by the injector based on type
+annotations. Every `build_app_from_module()` call creates a new `Dependencies` instance. Dependencies can be
+injected from the outside by passing a `Dependencies` instance to `build_app_from_module()` or by providing
+additional dependencies via a `callback()` function on the command group.
 
-## New-style type hint support
+Note that the `Dependencies` does not understand generics with different type parameters. For example, it makes
+no distinction between `MyGeneric[int]` and `MyGeneric[str]`. This is a limitation of the current implementation as well
+as the Python type system.
 
-Through `typeapi`, we can convert new-tyle type hints such as `str | None` or `list[int]` to their corresponding
-representation using `typing` before the function signature is parsed by [Typer][]. Usually, ty
+The most common use case for dependency injection is to inject configuration managers or clients into subcommands. For
+an example, you should check out the [examples/dependency-injection](./examples/dependency-injection) directory.
 
-```py
-# src/mypackage/commands/hello.py
-from mypackage.config import CliConfig
 
-def main(name: str | None = None) -> None:
-    # ...
-```
+## License
+
+This project is licensed under the terms of the MIT license.
```

### Comparing `typer_builder-0.0.7/src/typer_builder/_build.py` & `typer_builder-0.0.8/src/typer_builder/build_app.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 from pathlib import Path
 from pkgutil import iter_modules
 from typing import Any, Callable, Coroutine, Mapping, Sequence
 
 from typeapi import get_annotations
 from typer import Exit, Typer
 
-from ._injector import DependencyInjector
+from .Dependencies import Dependencies
 
 
 def build_app_from_module(
     module_name: str,
     name: str | None = None,
     typer_options: Mapping[str, Any] | None = None,
-    dependencies: DependencyInjector | Sequence[Any] = (),
+    dependencies: Dependencies | Sequence[Any] = (),
     event_loop: asyncio.AbstractEventLoop | None = None,
 ) -> Typer:
     """
     Looks at the module given with *module_name* and adds subcommand groups or commands to the Typer *app* based on
     the contents. Packages with an `__init__.py` will create a subcommand group, where the docstring of that module
     is the help of the group. Python modules that don't start with an underscore will create a command in the current
     subcommand group.
@@ -34,16 +34,16 @@
         function signature.
     """
 
     if event_loop is None:
         event_loop = asyncio.new_event_loop()
         asyncio.set_event_loop(event_loop)
 
-    if not isinstance(dependencies, DependencyInjector):
-        dependencies = DependencyInjector(*dependencies)
+    if not isinstance(dependencies, Dependencies):
+        dependencies = Dependencies(*dependencies)
 
     module = import_module(module_name)
     assert module.__file__, f"module {module_name!r} has no __file__"
     assert Path(module.__file__).stem == "__init__", f"expected a package for {module_name!r}"
 
     name = name or module_name.rpartition(".")[-1]
     app = Typer(name=name, help=module.__doc__, **(typer_options or {}))
@@ -59,15 +59,15 @@
         assert module_spec is not None, f"unable to find module spec of {submodule_info.name!r}"
         assert module_spec.origin is not None, f"module spec of {submodule_info.name!r} has no origin"
 
         if Path(module_spec.origin).stem == "__init__":
             sub_app = build_app_from_module(
                 submodule_info.name,
                 typer_options=typer_options,
-                dependencies=dependencies,
+                dependencies=dependencies.fork(),
                 event_loop=event_loop,
             )
             app.add_typer(sub_app)
 
         elif not submodule_name.startswith("_"):
             func = _prepare_typer_func(submodule.main, dependencies, event_loop)
             app.command(
@@ -75,15 +75,15 @@
                 help=func.__doc__ or submodule.__doc__,
             )(func)
 
     return app
 
 
 def _prepare_typer_func(
-    func: Callable[..., int | None], dependencies: DependencyInjector, event_loop: asyncio.AbstractEventLoop
+    func: Callable[..., int | None], dependencies: Dependencies, event_loop: asyncio.AbstractEventLoop
 ) -> Callable[..., None]:
     func = _evaluate_type_hints(func)
     if iscoroutinefunction(func):
         func = _deasyncify(func, event_loop)
     func = dependencies.bind(func, allow_unresolved=True)
     func = _raise_non_zero_exit_code_as_exit(func)
     return func
```

### Comparing `typer_builder-0.0.7/src/typer_builder/_build_test.py` & `typer_builder-0.0.8/src/typer_builder/build_app_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import List, Optional
 
 from pytest import raises
 from typer import Typer
 
-from typer_builder._build import _evaluate_type_hints
+from typer_builder.build_app import _evaluate_type_hints
 
 
 def test__evaluate_type_hints() -> None:
     def func(value: str | None) -> list[str]:
         assert value == "foo"
         return [value]
```

### Comparing `typer_builder-0.0.7/PKG-INFO` & `typer_builder-0.0.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,65 @@
 Metadata-Version: 2.1
 Name: typer-builder
-Version: 0.0.7
+Version: 0.0.8
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: deprecated (>=1.2.13,<2.0.0)
 Requires-Dist: nr-stream (>=1.1.5,<2.0.0)
 Requires-Dist: typeapi (>=1.4.1,<2.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
+Project-URL: Bug Tracker, https://github.com/NiklasRosenstein/python-typer-builder/issues
+Project-URL: Repository, https://github.com/NiklasRosenstein/typer-builder
 Description-Content-Type: text/markdown
 
 # typer-builder
 
   [Typer]: https://typer.tiangolo.com/
+  [pep585]: https://www.python.org/dev/peps/pep-0585/
+  [pep604]: https://www.python.org/dev/peps/pep-0604/
+  [typeapi]: https://github.com/NiklasRosenstein/python-typeapi
 
-This package allows you to easily build a [Typer][] CLI application from a Python module hierarchy.
+A framework for simplifying the development of [Typer][] based CLIs supporting modern type hints and hierarchical
+dependency injection. 
 
-### Quickstart
+__Table of Contents__
+
+* [Introduction](#introduction)
+  * [Example](#example)
+* [Documentation](#documentation)
+  * [New-style type hint support](#new-style-type-hint-support)
+  * [Dependency injection](#dependency-injection)
+
+
+## Introduction
+
+The `build_app_from_module()` inspect a hierarchy of Python modules to build a Typer command and group structure.
+Packages are treated as command groups and may define a `callback()` member. Modules are treated commands and must
+define a `main()` member. Modules and packages prefixed with an underscore ( `_` ) are ignored. Help text is extracted
+from the `main()` docstring or the module docstring.
+
+In addition, we provide support for new-style type hints ([PEP 585 - Type Hinting Generics in Standard Collections][pep585]
+and [PEP 604 - Union Operators][pep604]) in older versions of Python as well as adapt it for Typer (e.g. `list[str]`
+and `str | None`), as well as a method of injecting dependencies to functions that are not sourced from the command-line.
+
+
+### Example
 
 ```
-$ tree src/mypackage/commands/
+$ tree src/mypackage/
 src/mypackage/
 ├── __init__.py
 ├── __main__.py
 └── commands
     ├── __init__.py
     ├── hello.py
     └── bye.py
@@ -48,74 +76,46 @@
 from typer_builder import build_app_from_module
 
 if __name__ == "__main__":
     app = build_app_from_module("mypackage.commands")
     app()
 ```
 
-### Features
 
-* Packages are treated as command groups and _may_ define a `def callback(): ...` (see `Typer.add_callback()`).
-* Modules are treated as commands and _must_ define a `def main(): ...` (see `Typer.command()`).
-* Underscores in package or module names are normalized to hyphens (e.g `my_command` -> `my-command`).
-* Command(-group) help text is extracted from the package or module docstring, or from the `main()` docstring.
-* [WIP] Improved and dynamic dependency injection.
-* Support for new-style type hints in older versions of Python and Typer (e.g. `str | None`).
-
-### Dependency Injection
-
-The `typer_builder.DependencyInjector` is essentially a mapping of types to a corresponding implementation. It allows
-you to bind any function to the given dependencies based on the function signature.
-
-The `build_app_from_module()` takes a `dependencies` argument which populates a `DependencyInjector`. All `callback()`
-and `main()` functions encountered and added to a `typer.Typer` object are first bound to the dependencies that can be
-served by the injector.
-
-The types for which injection can take place must be known in advance. If the implementation is not known in advance,
-a `callback()` can accept the `DependencyInjector` as an argument and inform about the dependencies that will be
-provided by the callback, allowing any of its subcommands to resolve it.
+## Documentation
 
-```py
-# src/mypackages/commands/__init__.py
-"""
-This is a cool CLI that uses typer-builder.
-"""
-
-from mypackage.config import CliConfig
-from pathlib import Path
-from typer_builder import DependencyInjector, DelayedBinding
-from typer import Option
-
-def callback(
-    config_file: Path = Option(Path("~/.config/mypackage.ini"), help="Path to the configuration file."),
-    dependencies: DependencyInjector = DelayedBinding(CliConfig),
-) -> None:
-    dependencies.register_supplier(CliConfig, lambda: CliConfig.load(config_file))
-```
+### New-style type hint support
+
+Through [`typeapi`][typeapi], we can convert new-tyle type hints such as `str | None` or `list[int]` to their corresponding
+representation using `typing` before the function signature is parsed by [Typer][].
 
 ```py
-# src/mypackage/commands/hello.py
-from mypackage.config import CliConfig
+# src/mypackage/commands/create_user.py
+from ___future__ import annotations
 
-def main(name: str, config: CliConfig) -> None:
+def main(name: str | None = None, groups: list[str] | None = None) -> None:
     # ...
 ```
 
-In the above example, the `config` parameter is not passed by [Typer][], but instead by the `DependencyInjector` per the implementation in the previous `callback()` snippet.
+[`typeapi`][typeapi] also allows us to convert `list[str]` to `List[str]` and `dict[str, int]` to `Dict[str, int]` for
+Python versions prior to 3.9. This is necessary because [Typer][] does not support the new-style type hints.
 
-__Known caveats__
+### Dependency injection
 
-* Only concrete types are supported (no `Optional[CliConfig]` or vice versa).
+The `typer_builder.Dependencies` object is used to map types to concrete values or functions that provide them.
+Functions wrapped with `Dependencies.bind()` will have their arguments resolved by the injector based on type
+annotations. Every `build_app_from_module()` call creates a new `Dependencies` instance. Dependencies can be
+injected from the outside by passing a `Dependencies` instance to `build_app_from_module()` or by providing
+additional dependencies via a `callback()` function on the command group.
 
-## New-style type hint support
+Note that the `Dependencies` does not understand generics with different type parameters. For example, it makes
+no distinction between `MyGeneric[int]` and `MyGeneric[str]`. This is a limitation of the current implementation as well
+as the Python type system.
 
-Through `typeapi`, we can convert new-tyle type hints such as `str | None` or `list[int]` to their corresponding
-representation using `typing` before the function signature is parsed by [Typer][]. Usually, ty
+The most common use case for dependency injection is to inject configuration managers or clients into subcommands. For
+an example, you should check out the [examples/dependency-injection](./examples/dependency-injection) directory.
 
-```py
-# src/mypackage/commands/hello.py
-from mypackage.config import CliConfig
 
-def main(name: str | None = None) -> None:
-    # ...
-```
+## License
+
+This project is licensed under the terms of the MIT license.
```

