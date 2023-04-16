# Comparing `tmp/nonebot-desktop-wing-0.2.1.tar.gz` & `tmp/nonebot-desktop-wing-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-desktop-wing-0.2.1.tar", last modified: Thu Apr 13 14:19:21 2023, max compression
+gzip compressed data, was "nonebot-desktop-wing-0.2.2.tar", last modified: Sun Apr 16 08:44:23 2023, max compression
```

## Comparing `nonebot-desktop-wing-0.2.1.tar` & `nonebot-desktop-wing-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:19:21.126456 nonebot-desktop-wing-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-13 14:19:11.000000 nonebot-desktop-wing-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-13 14:19:21.126456 nonebot-desktop-wing-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-13 14:19:11.000000 nonebot-desktop-wing-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:19:21.122456 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-13 14:19:11.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-13 14:19:11.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-13 14:19:11.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/hindsight.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-13 14:19:11.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/lazylib.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-13 14:19:11.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/lazylib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-13 14:19:11.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/molecules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-04-13 14:19:11.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-13 14:19:11.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:19:21.126456 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-13 14:19:21.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-13 14:19:21.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:19:21.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-13 14:19:21.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-13 14:19:21.000000 nonebot-desktop-wing-0.2.1/nonebot_desktop_wing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-13 14:19:11.000000 nonebot-desktop-wing-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 14:19:21.126456 nonebot-desktop-wing-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:44:23.440392 nonebot-desktop-wing-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-16 08:44:07.000000 nonebot-desktop-wing-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-16 08:44:23.440392 nonebot-desktop-wing-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-16 08:44:07.000000 nonebot-desktop-wing-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:44:23.440392 nonebot-desktop-wing-0.2.2/nonebot_desktop_wing/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-16 08:44:07.000000 nonebot-desktop-wing-0.2.2/nonebot_desktop_wing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-16 08:44:07.000000 nonebot-desktop-wing-0.2.2/nonebot_desktop_wing/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-16 08:44:07.000000 nonebot-desktop-wing-0.2.2/nonebot_desktop_wing/hindsight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-16 08:44:07.000000 nonebot-desktop-wing-0.2.2/nonebot_desktop_wing/lazylib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-16 08:44:07.000000 nonebot-desktop-wing-0.2.2/nonebot_desktop_wing/lazylib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-04-16 08:44:07.000000 nonebot-desktop-wing-0.2.2/nonebot_desktop_wing/molecules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-04-16 08:44:07.000000 nonebot-desktop-wing-0.2.2/nonebot_desktop_wing/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-16 08:44:07.000000 nonebot-desktop-wing-0.2.2/nonebot_desktop_wing/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:44:23.440392 nonebot-desktop-wing-0.2.2/nonebot_desktop_wing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-16 08:44:23.000000 nonebot-desktop-wing-0.2.2/nonebot_desktop_wing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-16 08:44:23.000000 nonebot-desktop-wing-0.2.2/nonebot_desktop_wing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 08:44:23.000000 nonebot-desktop-wing-0.2.2/nonebot_desktop_wing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 08:44:23.000000 nonebot-desktop-wing-0.2.2/nonebot_desktop_wing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-16 08:44:23.000000 nonebot-desktop-wing-0.2.2/nonebot_desktop_wing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-16 08:44:07.000000 nonebot-desktop-wing-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 08:44:23.440392 nonebot-desktop-wing-0.2.2/setup.cfg
```

### Comparing `nonebot-desktop-wing-0.2.1/LICENSE` & `nonebot-desktop-wing-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.1/PKG-INFO` & `nonebot-desktop-wing-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-desktop-wing
-Version: 0.2.1
+Version: 0.2.2
 Summary: Wings for NoneBot desktop applications.
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nonedesktop/nonebot-desktop-wing
 Project-URL: Repository, https://github.com/nonedesktop/nonebot-desktop-wing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `nonebot-desktop-wing-0.2.1/README.md` & `nonebot-desktop-wing-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/__init__.py` & `nonebot-desktop-wing-0.2.2/nonebot_desktop_wing/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/constants.py` & `nonebot-desktop-wing-0.2.2/nonebot_desktop_wing/constants.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/hindsight.py` & `nonebot-desktop-wing-0.2.2/nonebot_desktop_wing/hindsight.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from threading import Thread
-from typing import IO, Callable, Generic, List, Optional, ParamSpec, TypeVar
+from typing import IO, Callable, Generic, ParamSpec, TypeVar
 
 T = TypeVar("T")
 AnyStr_T = TypeVar("AnyStr_T", str, bytes)
 P = ParamSpec("P")
 
 
 class BackgroundObject(Generic[P, T]):
```

### Comparing `nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/lazylib.pyi` & `nonebot-desktop-wing-0.2.2/nonebot_desktop_wing/lazylib.pyi`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/molecules.py` & `nonebot-desktop-wing-0.2.2/nonebot_desktop_wing/molecules.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from shutil import which
 import subprocess
 from tempfile import mkstemp
 from threading import Lock
 from types import ModuleType
 from typing import List, Literal, Optional, Tuple, TypeVar, Union, overload
 
-
 from nonebot_desktop_wing.constants import LINUX_TERMINALS, WINDOWS
 
 _import_lock = Lock()
 T = TypeVar("T")
 
 
 def import_with_lock(
```

### Comparing `nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/project.py` & `nonebot-desktop-wing-0.2.2/nonebot_desktop_wing/project.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.1/nonebot_desktop_wing/resources.py` & `nonebot-desktop-wing-0.2.2/nonebot_desktop_wing/resources.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.1/nonebot_desktop_wing.egg-info/PKG-INFO` & `nonebot-desktop-wing-0.2.2/nonebot_desktop_wing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-desktop-wing
-Version: 0.2.1
+Version: 0.2.2
 Summary: Wings for NoneBot desktop applications.
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nonedesktop/nonebot-desktop-wing
 Project-URL: Repository, https://github.com/nonedesktop/nonebot-desktop-wing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `nonebot-desktop-wing-0.2.1/nonebot_desktop_wing.egg-info/SOURCES.txt` & `nonebot-desktop-wing-0.2.2/nonebot_desktop_wing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.2.1/pyproject.toml` & `nonebot-desktop-wing-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-desktop-wing"
-version = "0.2.1"
+version = "0.2.2"
 description = "Wings for NoneBot desktop applications."
 authors = [
     {name = "HivertMoZara", email = "worldmozara@163.com"},
 ]
 license = {text = "MIT"}
 dependencies = ["nb_cli~=1.0.0", "python-dotenv~=1.0.0", "httpx>=0.23"]
 requires-python = ">=3.8"
```

