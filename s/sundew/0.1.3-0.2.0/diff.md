# Comparing `tmp/sundew-0.1.3.tar.gz` & `tmp/sundew-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sundew-0.1.3.tar", max compression
+gzip compressed data, was "sundew-0.2.0.tar", max compression
```

## Comparing `sundew-0.1.3.tar` & `sundew-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1068 2023-03-27 00:42:45.376292 sundew-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0     1129 2023-03-27 00:42:45.376292 sundew-0.1.3/README.md
--rw-r--r--   0        0        0     1067 2023-03-27 00:42:59.644667 sundew-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       44 2023-03-27 00:42:45.460294 sundew-0.1.3/sundew/__init__.py
--rw-r--r--   0        0        0       29 2023-03-27 00:42:45.460294 sundew-0.1.3/sundew/__main__.py
--rw-r--r--   0        0        0      250 2023-03-27 00:42:45.460294 sundew-0.1.3/sundew/config.py
--rw-r--r--   0        0        0     1384 2023-03-27 00:42:45.460294 sundew-0.1.3/sundew/graph.py
--rw-r--r--   0        0        0     3013 2023-03-27 00:42:45.460294 sundew-0.1.3/sundew/main.py
--rw-r--r--   0        0        0     2931 2023-03-27 00:42:45.464294 sundew-0.1.3/sundew/side_effects.py
--rw-r--r--   0        0        0    12572 2023-03-27 00:42:45.464294 sundew-0.1.3/sundew/test_runner.py
--rw-r--r--   0        0        0     8322 2023-03-27 00:42:45.464294 sundew-0.1.3/sundew/test_writer.py
--rw-r--r--   0        0        0     5160 2023-03-27 00:42:45.464294 sundew-0.1.3/sundew/types.py
--rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 sundew-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-16 17:39:06.711212 sundew-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1129 2023-04-16 17:39:06.711212 sundew-0.2.0/README.md
+-rw-r--r--   0        0        0     1801 2023-04-16 17:39:17.003381 sundew-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-04-16 17:39:06.787213 sundew-0.2.0/sundew/__init__.py
+-rw-r--r--   0        0        0       29 2023-04-16 17:39:06.787213 sundew-0.2.0/sundew/__main__.py
+-rw-r--r--   0        0        0      250 2023-04-16 17:39:06.787213 sundew-0.2.0/sundew/config.py
+-rw-r--r--   0        0        0     1384 2023-04-16 17:39:06.787213 sundew-0.2.0/sundew/graph.py
+-rw-r--r--   0        0        0     3077 2023-04-16 17:39:06.787213 sundew-0.2.0/sundew/main.py
+-rw-r--r--   0        0        0     2931 2023-04-16 17:39:06.787213 sundew-0.2.0/sundew/side_effects.py
+-rw-r--r--   0        0        0    13524 2023-04-16 17:39:06.787213 sundew-0.2.0/sundew/test_runner.py
+-rw-r--r--   0        0        0     7113 2023-04-16 17:39:06.787213 sundew-0.2.0/sundew/test_writer.py
+-rw-r--r--   0        0        0     5326 2023-04-16 17:39:06.787213 sundew-0.2.0/sundew/types.py
+-rw-r--r--   0        0        0     1326 2023-04-16 17:39:06.787213 sundew-0.2.0/sundew/utils.py
+-rw-r--r--   0        0        0     2041 1970-01-01 00:00:00.000000 sundew-0.2.0/PKG-INFO
```

### Comparing `sundew-0.1.3/LICENSE.txt` & `sundew-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sundew-0.1.3/README.md` & `sundew-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sundew-0.1.3/sundew/graph.py` & `sundew-0.2.0/sundew/graph.py`

 * *Files identical despite different names*

### Comparing `sundew-0.1.3/sundew/main.py` & `sundew-0.2.0/sundew/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import glob
 import importlib
 import importlib.util
 import os
 import sys
 from importlib.machinery import ModuleSpec
 from pathlib import Path
@@ -89,8 +90,12 @@
         if spec.loader:
             spec.loader.exec_module(imported_module)
         else:
             ...
     else:
         ...
 
-    test_runner.run(function_name=function, enable_auto_test_writer=auto_test_writer)
+    asyncio.run(
+        test_runner.run(
+            function_name=function, enable_auto_test_writer=auto_test_writer
+        )
+    )
```

### Comparing `sundew-0.1.3/sundew/side_effects.py` & `sundew-0.2.0/sundew/side_effects.py`

 * *Files identical despite different names*

### Comparing `sundew-0.1.3/sundew/test_runner.py` & `sundew-0.2.0/sundew/test_runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import ast
-import asyncio
 import importlib
 import inspect
 import os
 import sys
-from collections.abc import Callable, Coroutine
-from contextlib import ExitStack, _GeneratorContextManager
-from functools import wraps
+from collections.abc import Callable
+from contextlib import (
+    AsyncExitStack,
+    _AsyncGeneratorContextManager,
+    _GeneratorContextManager,
+)
 from typing import Any, Optional, Union
-from unittest.mock import patch
+from unittest.mock import AsyncMock, patch
 
 from pydantic import BaseConfig, BaseModel, create_model
 from rich import print
 from rich.progress import (
     BarColumn,
     MofNCompleteColumn,
     Progress,
@@ -59,52 +61,39 @@
                             Function(declaration=fn),
                             Function(declaration=sub_function),
                         )
         else:
             print("Not sure how we get here yet.")
 
 
-def get_test_function(fn: Callable) -> Callable:
-    @wraps(fn)
-    def sundew_test_wrapper(
-        *args: tuple[Any, ...],
-        **kwargs: dict[str, Any],
-    ) -> Callable:
-        return fn(*args, **kwargs)
-
-    @wraps(fn)
-    async def async_sundew_test_wrapper(
-        *args: tuple[Any, ...],
-        **kwargs: dict[str, Any],
-    ) -> Coroutine:
-        return await fn(*args, **kwargs)
-
-    if inspect.iscoroutinefunction(fn):
-        async_sundew_test_wrapper.__signature__ = inspect.signature(  # type: ignore[attr-defined]
-            fn
-        )
-        return async_sundew_test_wrapper
-    sundew_test_wrapper.__signature__ = inspect.signature(fn)  # type: ignore[attr-defined]
-    return sundew_test_wrapper
-
-
-def test(fn: Callable) -> Callable:
+def test(fn: Callable, proxy_fn: Union[Callable, None] = None) -> Callable:
     def add_test(
         cache: bool = False,  # noqa: FBT
-        setup: Optional[set[Callable[[], _GeneratorContextManager[Any]]]] = None,
+        setup: Optional[
+            set[
+                Callable[
+                    [],
+                    Union[
+                        _GeneratorContextManager[Any],
+                        _AsyncGeneratorContextManager[Any],
+                    ],
+                ]
+            ]
+        ] = None,
         kwargs: Optional[dict[str, Any]] = None,
         returns: Union[Any, Exception, None] = None,
         patches: Optional[dict[str, Any]] = None,
         side_effects: Optional[list[Callable]] = None,
     ) -> Callable:
         update_test_graph(fn)
 
         config.test_graph.add_test(
             FunctionTest(
-                function=get_test_function(fn),
+                function=fn,
+                proxy_function=proxy_fn,
                 kwargs=kwargs or {},
                 cache=cache,
                 location=f"{os.path.relpath(inspect.stack()[1][1])}:{inspect.stack()[1][2]}",
                 patches=patches or {},
                 returns=returns,
                 setup=setup or set(),
                 side_effects=side_effects or [],
@@ -112,33 +101,46 @@
         )
 
         return add_test
 
     return add_test
 
 
-def apply_patches(test: FunctionTest, stack: ExitStack) -> None:
+async def apply_patches(test: FunctionTest, stack: AsyncExitStack) -> None:
     if test.patches:
         for target, new in test.patches.items():
-            stack.enter_context(patch(target, new))
+            # If we are patching with a yield fixture, apply it
+            if inspect.isgeneratorfunction(inspect.unwrap(new)):
+                patch_fixture = stack.enter_context(new())
+                stack.enter_context(patch(target, patch_fixture))
+            elif inspect.isasyncgenfunction(inspect.unwrap(new)):
+                patch_fixture = await stack.enter_async_context(new())
+                stack.enter_context(patch(target, patch_fixture))
+            else:
+                stack.enter_context(patch(target, new))
 
 
-def apply_fixtures(test: FunctionTest, stack: ExitStack) -> dict[str, Any]:
+async def apply_fixtures(test: FunctionTest, stack: AsyncExitStack) -> dict[str, Any]:
     fixture_yields = {}
     if test.setup:
         for fixture in test.setup:
-            fixture_yield: Any = stack.enter_context(fixture())
+            fixture_yield: Any
+            if inspect.isasyncgenfunction(inspect.unwrap(fixture)):  # async fixture
+                fixture_yield = await stack.enter_async_context(fixture())  # type: ignore[arg-type]
+            else:  # normal fixture
+                fixture_yield = stack.enter_context(fixture())  # type: ignore[arg-type]
             fixture_yields[fixture.__name__] = fixture_yield
 
     return fixture_yields
 
 
 def copy_function_inputs(test: FunctionTest) -> dict[str, Any]:
+    function_under_test = test.proxy_function or test.function
     isolated_inputs: dict[str, Any] = {}
-    signature = inspect.signature(test.function)
+    signature = inspect.signature(function_under_test)
     isolated_inputs = {
         k: v.default
         for k, v in signature.parameters.items()
         if v.default is not inspect.Parameter.empty
     }
 
     for arg_name, input_value in test.kwargs.items():
@@ -150,49 +152,61 @@
                 result = input_value
         else:
             result = input_value
         isolated_inputs[arg_name] = result
     return isolated_inputs
 
 
-def run_function(
-    test: FunctionTest, isolated_input: dict[str, Any]
+async def run_function(
+    test: FunctionTest, isolated_input: dict[str, Any], stack: AsyncExitStack
 ) -> Any:  # noqa: ANN401
-    if test.cache and config.cache.contains(test.function, test.kwargs):
-        return config.cache.get_cached_value(test.function, test.kwargs)
+    # Run proxy_function if it exists, else function
+    function = test.proxy_function or test.function
+    if test.proxy_function is not None:
+        mock = stack.enter_context(
+            patch(test.name.qualified, AsyncMock(wraps=test.function))
+        )
+    if test.cache and config.cache.contains(function, test.kwargs):
+        return config.cache.get_cached_value(function, test.kwargs)
+
+    # Call function
+    if inspect.iscoroutinefunction(function):
+        actual_return = await function(**isolated_input)
+    else:
+        actual_return = function(**isolated_input)
 
-    if inspect.iscoroutinefunction(test.function):
-        return asyncio.run(test.function(**isolated_input))
-    return test.function(**isolated_input)
+    if test.proxy_function is not None:
+        mock.assert_awaited()
+
+    return actual_return
 
 
 def check_test_exception(test: FunctionTest, e: Exception) -> None:
     # If we get an exception, check to see if it was expected
-    if test.returns:
-        assert isinstance(e, test.returns)
+    if test.returns is not None and isinstance(test.returns, Exception):
+        assert isinstance(e, test.returns.__class__)
     else:
         raise e
 
 
 def check_test_output(test: FunctionTest, actual_return: Any) -> None:  # noqa: ANN401
     if isinstance(actual_return, ast.Module) and isinstance(test.returns, ast.Module):
         assert (
             ast.unparse(actual_return).strip() == ast.unparse(test.returns).strip()
         ), (
             f"Input {test.kwargs} returned AST for "
             + f"{ast.unparse(actual_return).strip()} "
             + "which does not match the expected AST for "
             + f"{ast.unparse(test.returns).strip()}"
         )
-    #     assert actual_return.__code__.co_code == test.returns.__code__.co_code, (
     else:
         assert actual_return == test.returns, (
-            f"Input {test.kwargs} returned {actual_return} "
+            f"Input {test.kwargs} returned {repr(actual_return)} "
             + "which does not match the expected return of "
-            + f"{test.returns}"
+            + f"{repr(test.returns)}"
         )
 
 
 def build_side_effect_vars(test_function: Callable) -> type[BaseModel]:
     # Parse function signature annotations
     funtion_arguments: dict[str, tuple[Any, Any]] = {}
     for name, parameter in inspect.signature(test_function).parameters.items():
@@ -229,49 +243,50 @@
             side_effect_arg_model = build_side_effect_vars(test.function)
             _ = side_effect_arg_model.construct(
                 patches=test.patches, returns=actual_return, **isolated_input
             )
             exec(side_effect_code)  # noqa: S102
 
 
-def run_test(
+async def run_test(
     test: FunctionTest,
-    stack: ExitStack,
+    stack: AsyncExitStack,
     tests_ran: TaskID,
     progress: Progress,
     enable_auto_test_writer: bool,  # noqa: FBT001
 ) -> None:
     try:
         # programmatically apply any patches defined
-        apply_patches(test, stack)
+        await apply_patches(test, stack)
         # programmatically apply any fixtures setup
-        apply_fixtures(test, stack)
+        await apply_fixtures(test, stack)
         try:
             # Isolate input arguments
             isolated_input = copy_function_inputs(test)
 
             # Mock dependent functions to be able to write regression tests
             mocks = mock_function_dependencies(test.function, stack)
 
             # Run the test function once for evaluation
-            actual_return = run_function(test, isolated_input)
+            actual_return = await run_function(test, isolated_input, stack)
 
             if enable_auto_test_writer:
                 # Write tests with mock data
                 generate_function_dependency_test_file(test.function, mocks)
 
         except Exception as e:  # noqa: BLE001
             # If we get an exception, check if it's expected
             check_test_exception(test, e)
         else:
             # If we didn't get an exception then check the output normally
-            if test.returns:
+            if test.returns is not None:
                 check_test_output(test, actual_return)
-        finally:
-            # Check if we have defined side effects
+
+        # Check if we have defined side effects
+        if test.side_effects is not None:
             check_test_side_effects(test, actual_return, isolated_input)
 
     except AssertionError as e:
         # Stop the progress bar
         progress.stop()
         # Log details of the failure
         print(f"\n[bold red1]FAILURE[/] {test.location} - {str(e)}")
@@ -331,15 +346,17 @@
         if function not in selected_functions:
             function_name = config.test_graph.functions[function].name
             missing_tests.append(function_name.qualified or function_name.simple)
 
     return missing_tests
 
 
-def run(function_name: str, enable_auto_test_writer: bool) -> None:  # noqa: FBT001
+async def run(
+    function_name: str, enable_auto_test_writer: bool  # noqa: FBT001
+) -> None:
     with Progress(
         TextColumn("{task.description}"),
         BarColumn(),
         MofNCompleteColumn(),
         TimeElapsedColumn(),
     ) as progress:
         total_num_tests = sum(
@@ -359,9 +376,11 @@
             f"Selected {len(sorted_tests)}/{total_num_tests} tests",
         )
 
         tests_ran = progress.add_task("Running tests...", total=len(sorted_tests))
 
         # Run all selected tests
         for test in sorted_tests:
-            with ExitStack() as stack:
-                run_test(test, stack, tests_ran, progress, enable_auto_test_writer)
+            async with AsyncExitStack() as stack:
+                await run_test(
+                    test, stack, tests_ran, progress, enable_auto_test_writer
+                )
```

### Comparing `sundew-0.1.3/sundew/test_writer.py` & `sundew-0.2.0/sundew/test_writer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,37 @@
 import inspect
 from collections.abc import Callable
-from contextlib import ExitStack
+from contextlib import AsyncExitStack
 from pathlib import Path
-from typing import Any
 from unittest.mock import patch
 
 import black
 
 from sundew.config import config
 from sundew.types import FunctionTest
-
-
-class DependentFunctionSpy:
-    def __init__(self, func: Callable) -> None:
-        self.func = func
-        self.calls: set[FunctionTest] = set()
-        self.__name__ = func.__name__
-        self.__qualname__ = func.__qualname__
-
-    def __call__(
-        self, *args: tuple[Any, ...], **kwargs: dict[str, Any]
-    ) -> Any:  # noqa: ANN401
-        generated_kwargs = inspect.getcallargs(self.func, *args, **kwargs)
-
-        # Check cache
-        if config.cache.contains(self.func, generated_kwargs):
-            return config.cache.get_cached_value(self.func, generated_kwargs)
-
-        answer = self.func(*args, **kwargs)
-        function_test = FunctionTest(
-            function=self.func,
-            kwargs=generated_kwargs,
-            returns=answer,
-            cache=True,
-        )
-        self.calls.add(function_test)
-        return answer
-
-    def __eq__(self, other: object) -> bool:
-        if not isinstance(other, DependentFunctionSpy):
-            # don't attempt to compare against unrelated types
-            return NotImplemented
-
-        return (
-            self.func.__code__.co_code == other.func.__code__.co_code
-            and self.calls == other.calls
-        )
+from sundew.utils import FunctionSpy
 
 
 def mock_function_dependencies(
-    fn: Callable, stack: ExitStack
-) -> dict[str, DependentFunctionSpy]:
-    mocks: dict[str, DependentFunctionSpy] = {}
+    fn: Callable, stack: AsyncExitStack
+) -> dict[str, FunctionSpy]:
+    mocks: dict[str, FunctionSpy] = {}
     for dep_func_simple_name in config.test_graph.functions[fn.__name__].deps:
         dep_func = config.test_graph.functions[dep_func_simple_name]
         # Recursively mock sub-dependent functions
         if (
             config.test_graph.functions[dep_func_simple_name].deps
             and dep_func_simple_name != "mock_function_dependencies"
         ):
             mocks.update(mock_function_dependencies(dep_func.declaration, stack))
         # Spy on all dependent functions
         mocks[dep_func_simple_name] = stack.enter_context(
             patch(
                 dep_func.name.qualified,
-                DependentFunctionSpy(dep_func.declaration),
+                FunctionSpy(dep_func.declaration),
             )
         )
     return mocks
 
 
 def check_kwargs_for_imports(test_fn: FunctionTest) -> list[list[str]]:
     imports = []
@@ -200,15 +163,15 @@
 
     file_path /= f"auto_test_{fn.__name__}.py"
 
     return file_path
 
 
 def generate_function_dependency_test_file(
-    fn: Callable, mocks: dict[str, DependentFunctionSpy]
+    fn: Callable, mocks: dict[str, FunctionSpy]
 ) -> None:
     generated_test_file_imports = set()
     mock_calls: set[FunctionTest] = set()
     # Build imports
     for mock_name, mock_fn in mocks.items():
         # Only add imports if we generated tests for the mocked function
         if mock_fn.calls:
```

### Comparing `sundew-0.1.3/sundew/types.py` & `sundew-0.2.0/sundew/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import inspect
 from collections.abc import Callable
-from contextlib import _GeneratorContextManager
+from contextlib import _AsyncGeneratorContextManager, _GeneratorContextManager
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import Any, Optional
+from typing import Any, Optional, Union
 
 
 def format_kwargs(kwargs: dict[str, Any]) -> str:
     formatted_kwargs = []
     for kwarg, kwval in kwargs.items():
         if isinstance(kwval, set):
             formatted_kwargs.append(f"{repr(kwarg)}: {kwval}")
@@ -23,20 +23,25 @@
     simple: str
     qualified: str
 
 
 @dataclass(eq=True)
 class FunctionTest:
     function: Callable
+    proxy_function: Union[Callable, None] = None
     location: str = ""
     cache: bool = False
     kwargs: dict[str, Any] = field(default_factory=dict)
     patches: dict[str, Any] = field(default_factory=dict)
     returns: Optional[Any] = None
-    setup: set[Callable[[], _GeneratorContextManager[Any]]] = field(default_factory=set)
+    setup: set[
+        Callable[
+            [], Union[_GeneratorContextManager[Any], _AsyncGeneratorContextManager[Any]]
+        ]
+    ] = field(default_factory=set)
     side_effects: list[Callable[[Any], bool]] = field(default_factory=list)
 
     @property
     def name(self) -> FunctionName:
         simple_name = self.function.__name__
         qualified_name = self.function.__qualname__
         if simple_name == qualified_name:
```

### Comparing `sundew-0.1.3/PKG-INFO` & `sundew-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 Metadata-Version: 2.1
 Name: sundew
-Version: 0.1.3
+Version: 0.2.0
 Summary: 
+Home-page: https://github.com/devenjarvis/sundew
 License: MIT
+Keywords: testing
 Author: devenjarvis
 Author-email: devenjarvis@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Testing
 Requires-Dist: black
 Requires-Dist: cachetools
+Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: poetry (>=1.4.0,<2.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Project-URL: Documentation, https://devenjarvis.github.io/sundew/#/
+Project-URL: Repository, https://github.com/devenjarvis/sundew
 Description-Content-Type: text/markdown
 
 # sundew ☀️
 A new kind of testing framework for Python.
 
 ## Here Be Dragons 🐉
 Not only does this project attempt a new approach to testing, it is also in _very_ early stages and thus still has alot of sharp edges. Early adopters are encouraged to try out sundew and report any issues or critical missing functionality in the form of a GitHub Issue.
```

