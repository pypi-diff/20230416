# Comparing `tmp/pdm_conda-0.8.1b1.tar.gz` & `tmp/pdm_conda-0.8.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_conda-0.8.1b1.tar", last modified: Sat Apr 15 17:38:01 2023, max compression
+gzip compressed data, was "pdm_conda-0.8.1b2.tar", last modified: Sun Apr 16 20:38:06 2023, max compression
```

## Comparing `pdm_conda-0.8.1b1.tar` & `pdm_conda-0.8.1b2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1065 2022-12-16 23:52:20.043514 pdm_conda-0.8.1b1/LICENSE
--rw-r--r--   0        0        0     4832 2023-04-09 20:29:55.601420 pdm_conda-0.8.1b1/README.md
--rw-r--r--   0        0        0     2021 2023-04-15 17:38:01.598644 pdm_conda-0.8.1b1/pyproject.toml
--rw-r--r--   0        0        0      595 2023-04-15 17:37:37.531424 pdm_conda-0.8.1b1/src/pdm_conda/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:28.238706 pdm_conda-0.8.1b1/src/pdm_conda/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:59.837399 pdm_conda-0.8.1b1/src/pdm_conda/cli/commands/__init__.py
--rw-r--r--   0        0        0     3219 2023-04-09 20:29:55.603310 pdm_conda-0.8.1b1/src/pdm_conda/cli/commands/add.py
--rw-r--r--   0        0        0     1681 2023-04-09 20:29:55.604146 pdm_conda-0.8.1b1/src/pdm_conda/cli/commands/remove.py
--rw-r--r--   0        0        0     2183 2023-04-09 20:29:55.604925 pdm_conda-0.8.1b1/src/pdm_conda/cli/utils.py
--rw-r--r--   0        0        0    11223 2023-04-15 17:34:37.904070 pdm_conda-0.8.1b1/src/pdm_conda/conda.py
--rw-r--r--   0        0        0        0 2023-01-05 20:40:25.652497 pdm_conda-0.8.1b1/src/pdm_conda/installers/__init__.py
--rw-r--r--   0        0        0     2482 2023-04-09 20:29:55.606525 pdm_conda-0.8.1b1/src/pdm_conda/installers/manager.py
--rw-r--r--   0        0        0     2162 2023-04-14 22:24:14.370967 pdm_conda-0.8.1b1/src/pdm_conda/installers/synchronizers.py
--rw-r--r--   0        0        0     3132 2023-01-17 17:44:51.337923 pdm_conda-0.8.1b1/src/pdm_conda/mapping.py
--rw-r--r--   0        0        0        0 2023-01-02 22:45:44.891129 pdm_conda-0.8.1b1/src/pdm_conda/models/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 01:53:52.844040 pdm_conda-0.8.1b1/src/pdm_conda/models/__pycache__/candidates.cpython-310.pyc.281473776611248
--rw-r--r--   0        0        0     6776 2023-04-09 20:29:55.608074 pdm_conda-0.8.1b1/src/pdm_conda/models/candidates.py
--rw-r--r--   0        0        0     1818 2023-04-15 01:10:11.358619 pdm_conda-0.8.1b1/src/pdm_conda/models/conda.py
--rw-r--r--   0        0        0     7145 2023-04-10 20:13:29.271209 pdm_conda-0.8.1b1/src/pdm_conda/models/config.py
--rw-r--r--   0        0        0     3234 2023-04-09 20:29:55.609532 pdm_conda-0.8.1b1/src/pdm_conda/models/environment.py
--rw-r--r--   0        0        0     3863 2023-04-09 20:29:55.610491 pdm_conda-0.8.1b1/src/pdm_conda/models/repositories.py
--rw-r--r--   0        0        0    10806 2023-04-15 17:37:15.580889 pdm_conda-0.8.1b1/src/pdm_conda/models/requirements.py
--rw-r--r--   0        0        0      900 2023-04-09 20:29:55.611942 pdm_conda-0.8.1b1/src/pdm_conda/models/setup.py
--rw-r--r--   0        0        0     8413 2023-04-14 22:23:45.622217 pdm_conda-0.8.1b1/src/pdm_conda/project.py
--rw-r--r--   0        0        0        0 2023-02-18 20:09:32.663574 pdm_conda-0.8.1b1/src/pdm_conda/resolver/__init__.py
--rw-r--r--   0        0        0     1134 2023-02-23 00:47:35.312247 pdm_conda-0.8.1b1/src/pdm_conda/resolver/providers.py
--rw-r--r--   0        0        0     5455 2023-04-15 17:36:44.693219 pdm_conda-0.8.1b1/src/pdm_conda/resolvers.py
--rw-r--r--   0        0        0      784 2023-01-10 16:37:32.674613 pdm_conda-0.8.1b1/src/pdm_conda/utils.py
--rw-r--r--   0        0        0     6628 1970-01-01 00:00:00.000000 pdm_conda-0.8.1b1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-12-16 23:52:20.043514 pdm_conda-0.8.1b2/LICENSE
+-rw-r--r--   0        0        0     4832 2023-04-09 20:29:55.601420 pdm_conda-0.8.1b2/README.md
+-rw-r--r--   0        0        0     2020 2023-04-16 20:38:07.194508 pdm_conda-0.8.1b2/pyproject.toml
+-rw-r--r--   0        0        0      595 2023-04-15 20:17:55.377949 pdm_conda-0.8.1b2/src/pdm_conda/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-06 20:52:28.238706 pdm_conda-0.8.1b2/src/pdm_conda/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-06 20:52:59.837399 pdm_conda-0.8.1b2/src/pdm_conda/cli/commands/__init__.py
+-rw-r--r--   0        0        0     3219 2023-04-09 20:29:55.603310 pdm_conda-0.8.1b2/src/pdm_conda/cli/commands/add.py
+-rw-r--r--   0        0        0     1681 2023-04-09 20:29:55.604146 pdm_conda-0.8.1b2/src/pdm_conda/cli/commands/remove.py
+-rw-r--r--   0        0        0     2183 2023-04-09 20:29:55.604925 pdm_conda-0.8.1b2/src/pdm_conda/cli/utils.py
+-rw-r--r--   0        0        0    11223 2023-04-15 17:34:37.904070 pdm_conda-0.8.1b2/src/pdm_conda/conda.py
+-rw-r--r--   0        0        0        0 2023-01-05 20:40:25.652497 pdm_conda-0.8.1b2/src/pdm_conda/installers/__init__.py
+-rw-r--r--   0        0        0     2482 2023-04-09 20:29:55.606525 pdm_conda-0.8.1b2/src/pdm_conda/installers/manager.py
+-rw-r--r--   0        0        0     2311 2023-04-15 20:38:24.832128 pdm_conda-0.8.1b2/src/pdm_conda/installers/synchronizers.py
+-rw-r--r--   0        0        0     3132 2023-01-17 17:44:51.337923 pdm_conda-0.8.1b2/src/pdm_conda/mapping.py
+-rw-r--r--   0        0        0        0 2023-01-02 22:45:44.891129 pdm_conda-0.8.1b2/src/pdm_conda/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-30 01:53:52.844040 pdm_conda-0.8.1b2/src/pdm_conda/models/__pycache__/candidates.cpython-310.pyc.281473776611248
+-rw-r--r--   0        0        0     6776 2023-04-09 20:29:55.608074 pdm_conda-0.8.1b2/src/pdm_conda/models/candidates.py
+-rw-r--r--   0        0        0     1818 2023-04-15 01:10:11.358619 pdm_conda-0.8.1b2/src/pdm_conda/models/conda.py
+-rw-r--r--   0        0        0     7145 2023-04-10 20:13:29.271209 pdm_conda-0.8.1b2/src/pdm_conda/models/config.py
+-rw-r--r--   0        0        0     3492 2023-04-15 19:31:29.818151 pdm_conda-0.8.1b2/src/pdm_conda/models/environment.py
+-rw-r--r--   0        0        0     3863 2023-04-09 20:29:55.610491 pdm_conda-0.8.1b2/src/pdm_conda/models/repositories.py
+-rw-r--r--   0        0        0    10806 2023-04-15 17:37:15.580889 pdm_conda-0.8.1b2/src/pdm_conda/models/requirements.py
+-rw-r--r--   0        0        0      900 2023-04-09 20:29:55.611942 pdm_conda-0.8.1b2/src/pdm_conda/models/setup.py
+-rw-r--r--   0        0        0     8413 2023-04-14 22:23:45.622217 pdm_conda-0.8.1b2/src/pdm_conda/project.py
+-rw-r--r--   0        0        0        0 2023-02-18 20:09:32.663574 pdm_conda-0.8.1b2/src/pdm_conda/resolver/__init__.py
+-rw-r--r--   0        0        0     1134 2023-02-23 00:47:35.312247 pdm_conda-0.8.1b2/src/pdm_conda/resolver/providers.py
+-rw-r--r--   0        0        0     5455 2023-04-15 17:36:44.693219 pdm_conda-0.8.1b2/src/pdm_conda/resolvers.py
+-rw-r--r--   0        0        0      784 2023-01-10 16:37:32.674613 pdm_conda-0.8.1b2/src/pdm_conda/utils.py
+-rw-r--r--   0        0        0     6627 1970-01-01 00:00:00.000000 pdm_conda-0.8.1b2/PKG-INFO
```

### Comparing `pdm_conda-0.8.1b1/LICENSE` & `pdm_conda-0.8.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b1/README.md` & `pdm_conda-0.8.1b2/README.md`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b1/pyproject.toml` & `pdm_conda-0.8.1b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 dynamic = []
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = [
-    "prefect",
+    "pytest",
 ]
-version = "0.8.1b1"
+version = "0.8.1b2"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/macro128/pdm-conda"
 Changelog = "https://github.com/macro128/pdm-conda/blob/main/CHANGELOG.md"
```

### Comparing `pdm_conda-0.8.1b1/src/pdm_conda/__init__.py` & `pdm_conda-0.8.1b2/src/pdm_conda/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
     core.register_command(AddCommand)
     core.register_command(RemoveCommand)
 
     for name, config in CONFIGS:
         core.add_config(name, config)
 
 
-__version__ = "0.8.1b1"
+__version__ = "0.8.1b2"
```

### Comparing `pdm_conda-0.8.1b1/src/pdm_conda/cli/commands/add.py` & `pdm_conda-0.8.1b2/src/pdm_conda/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b1/src/pdm_conda/cli/commands/remove.py` & `pdm_conda-0.8.1b2/src/pdm_conda/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b1/src/pdm_conda/cli/utils.py` & `pdm_conda-0.8.1b2/src/pdm_conda/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b1/src/pdm_conda/conda.py` & `pdm_conda-0.8.1b2/src/pdm_conda/conda.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b1/src/pdm_conda/installers/manager.py` & `pdm_conda-0.8.1b2/src/pdm_conda/installers/manager.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b1/src/pdm_conda/installers/synchronizers.py` & `pdm_conda-0.8.1b2/src/pdm_conda/installers/synchronizers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Collection, cast
 
 from pdm.installers import Synchronizer
 from pdm.models.candidates import Candidate
 
 from pdm_conda.models.candidates import CondaCandidate
 from pdm_conda.models.environment import CondaEnvironment, Environment
+from pdm_conda.models.setup import CondaSetupDistribution
 
 
 class CondaSynchronizer(Synchronizer):
     def __init__(
         self,
         candidates: dict[str, Candidate],
         environment: Environment,
@@ -39,23 +40,25 @@
     def compare_with_working_set(self) -> tuple[list[str], list[str], list[str]]:
         to_add, to_update, to_remove = super().compare_with_working_set()
 
         # deactivate parallel execution if uninstall
         self.parallel = self.environment.project.config["install.parallel"]
         if to_remove:
             to_remove = [p for p in to_remove if p not in self.environment.python_dependencies]
-
-        if self.parallel and any(
-            True for d in to_remove + to_update if isinstance(self.candidates.get(d, None), CondaCandidate)
-        ):
+     
+        num_update, num_remove = (
+            len([p for p in pks if isinstance(self.working_set[p], CondaSetupDistribution)])
+            for pks in (to_update, to_remove)
+        )
+        if self.parallel and (num_update + num_remove > 0):
             self.environment.project.core.ui.echo("Deactivating parallel uninstall.")
             self.parallel = False
 
         if self.environment.project.conda_config.batched_commands:
+            num_adds = len([p for p in to_add if isinstance(self.candidates[p], CondaCandidate)])
+
             self.manager.prepare_batch_operations(
-                *(
-                    len([p for p in pkgs if isinstance(self.candidates[p], CondaCandidate)])
-                    for pkgs in (to_add + to_update, to_remove + to_update)
-                )
+                num_install=num_adds + num_update,
+                num_remove=num_remove + num_update
             )
 
         return to_add, to_update, to_remove
```

### Comparing `pdm_conda-0.8.1b1/src/pdm_conda/mapping.py` & `pdm_conda-0.8.1b2/src/pdm_conda/mapping.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b1/src/pdm_conda/models/candidates.py` & `pdm_conda-0.8.1b2/src/pdm_conda/models/candidates.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b1/src/pdm_conda/models/conda.py` & `pdm_conda-0.8.1b2/src/pdm_conda/models/conda.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b1/src/pdm_conda/models/config.py` & `pdm_conda-0.8.1b2/src/pdm_conda/models/config.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b1/src/pdm_conda/models/environment.py` & `pdm_conda-0.8.1b2/src/pdm_conda/models/environment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import functools
 import os
+import sysconfig
 from copy import copy
 from pathlib import Path
 from typing import cast
 
 from pdm.exceptions import NoPythonVersion, ProjectError
 from pdm.models.environment import Environment, PrefixEnvironment
 from pdm.models.requirements import Requirement
@@ -15,26 +16,36 @@
 from pdm_conda.models.candidates import CondaCandidate
 from pdm_conda.project import CondaProject
 from pdm_conda.utils import normalize_name
 
 _patched = False
 
 
+def ensure_conda_env():
+    if (packages_path := os.getenv("CONDA_PREFIX", None)) is None:
+        raise ProjectError("Conda environment not detected.")
+    return packages_path
+
+
 class CondaEnvironment(Environment):
     def __init__(self, project: Project) -> None:
         super().__init__(project)
         self.project = cast(CondaProject, project)
         self._python_dependencies: dict[str, Requirement] | None = None
         self._python_candidate: CondaCandidate | None = None
 
     @property
     def packages_path(self) -> Path:
-        if (packages_path := os.getenv("CONDA_PREFIX", None)) is None:
-            raise ProjectError("Conda environment not detected.")
-        return Path(packages_path)
+        return Path(ensure_conda_env())
+
+    def get_paths(self) -> dict[str, str]:
+        prefix = ensure_conda_env()
+        paths = sysconfig.get_paths(expand=True)
+        paths.setdefault("prefix", prefix)
+        return paths
 
     def get_working_set(self) -> WorkingSet:
         """
         Get the working set based on local packages directory, include Conda managed packages.
         """
         working_set = super().get_working_set()
         working_set._dist_map = conda_list(self.project) | {
```

### Comparing `pdm_conda-0.8.1b1/src/pdm_conda/models/repositories.py` & `pdm_conda-0.8.1b2/src/pdm_conda/models/repositories.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b1/src/pdm_conda/models/requirements.py` & `pdm_conda-0.8.1b2/src/pdm_conda/models/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b1/src/pdm_conda/models/setup.py` & `pdm_conda-0.8.1b2/src/pdm_conda/models/setup.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b1/src/pdm_conda/project.py` & `pdm_conda-0.8.1b2/src/pdm_conda/project.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b1/src/pdm_conda/resolver/providers.py` & `pdm_conda-0.8.1b2/src/pdm_conda/resolver/providers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b1/src/pdm_conda/resolvers.py` & `pdm_conda-0.8.1b2/src/pdm_conda/resolvers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b1/src/pdm_conda/utils.py` & `pdm_conda-0.8.1b2/src/pdm_conda/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b1/PKG-INFO` & `pdm_conda-0.8.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-conda
-Version: 0.8.1b1
+Version: 0.8.1b2
 Summary:  A PDM plugin to install project dependencies with Conda
 Keywords: pdm plugin conda
 Author: Marcos Pastorini
 License: MIT License
         
         Copyright (c) 2022 macro128
         
@@ -27,15 +27,15 @@
         SOFTWARE.
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Project-URL: Homepage, https://github.com/macro128/pdm-conda
 Project-URL: Changelog, https://github.com/macro128/pdm-conda/blob/main/CHANGELOG.md
 Requires-Python: >=3.10
-Requires-Dist: prefect
+Requires-Dist: pytest
 Description-Content-Type: text/markdown
 
 # pdm-conda
 
 A PDM plugin to install project dependencies with Conda.
 
 ## Configuration
```

