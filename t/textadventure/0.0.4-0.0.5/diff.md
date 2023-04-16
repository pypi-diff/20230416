# Comparing `tmp/textadventure-0.0.4.tar.gz` & `tmp/textadventure-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textadventure-0.0.4.tar", last modified: Sun Apr 16 21:04:18 2023, max compression
+gzip compressed data, was "textadventure-0.0.5.tar", last modified: Sun Apr 16 21:07:44 2023, max compression
```

## Comparing `textadventure-0.0.4.tar` & `textadventure-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 21:04:18.034556 textadventure-0.0.4/
--rw-rw-rw-   0        0        0    12438 2023-04-16 09:59:23.000000 textadventure-0.0.4/LICENSE.md
--rw-rw-rw-   0        0        0     5448 2023-04-16 21:04:18.034556 textadventure-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4986 2023-04-16 11:43:36.000000 textadventure-0.0.4/README.md
--rw-rw-rw-   0        0        0      568 2023-04-16 21:04:03.000000 textadventure-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-16 21:04:18.034556 textadventure-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-16 21:04:18.016416 textadventure-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 21:04:18.022772 textadventure-0.0.4/src/textadventure/
--rw-rw-rw-   0        0        0     6495 2023-04-16 21:03:53.000000 textadventure-0.0.4/src/textadventure/__init__.py
--rw-rw-rw-   0        0        0     2409 2023-04-16 11:17:09.000000 textadventure-0.0.4/src/textadventure/input.py
--rw-rw-rw-   0        0        0      697 2023-04-16 07:11:59.000000 textadventure-0.0.4/src/textadventure/menu.py
--rw-rw-rw-   0        0        0      255 2023-04-16 06:46:12.000000 textadventure-0.0.4/src/textadventure/output.py
--rw-rw-rw-   0        0        0      238 2023-04-16 05:25:27.000000 textadventure-0.0.4/src/textadventure/timing.py
-drwxrwxrwx   0        0        0        0 2023-04-16 21:04:18.033176 textadventure-0.0.4/src/textadventure.egg-info/
--rw-rw-rw-   0        0        0     5448 2023-04-16 21:04:18.000000 textadventure-0.0.4/src/textadventure.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      378 2023-04-16 21:04:18.000000 textadventure-0.0.4/src/textadventure.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 21:04:18.000000 textadventure-0.0.4/src/textadventure.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-16 21:04:18.000000 textadventure-0.0.4/src/textadventure.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-16 21:04:18.000000 textadventure-0.0.4/src/textadventure.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 21:07:44.920135 textadventure-0.0.5/
+-rw-rw-rw-   0        0        0    12438 2023-04-16 09:59:23.000000 textadventure-0.0.5/LICENSE.md
+-rw-rw-rw-   0        0        0     5448 2023-04-16 21:07:44.919116 textadventure-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4986 2023-04-16 11:43:36.000000 textadventure-0.0.5/README.md
+-rw-rw-rw-   0        0        0      568 2023-04-16 21:07:01.000000 textadventure-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 21:07:44.920135 textadventure-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 21:07:44.901618 textadventure-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 21:07:44.908060 textadventure-0.0.5/src/textadventure/
+-rw-rw-rw-   0        0        0     6477 2023-04-16 21:06:52.000000 textadventure-0.0.5/src/textadventure/__init__.py
+-rw-rw-rw-   0        0        0     2409 2023-04-16 11:17:09.000000 textadventure-0.0.5/src/textadventure/input.py
+-rw-rw-rw-   0        0        0      697 2023-04-16 07:11:59.000000 textadventure-0.0.5/src/textadventure/menu.py
+-rw-rw-rw-   0        0        0      255 2023-04-16 06:46:12.000000 textadventure-0.0.5/src/textadventure/output.py
+-rw-rw-rw-   0        0        0      238 2023-04-16 05:25:27.000000 textadventure-0.0.5/src/textadventure/timing.py
+drwxrwxrwx   0        0        0        0 2023-04-16 21:07:44.918096 textadventure-0.0.5/src/textadventure.egg-info/
+-rw-rw-rw-   0        0        0     5448 2023-04-16 21:07:44.000000 textadventure-0.0.5/src/textadventure.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-04-16 21:07:44.000000 textadventure-0.0.5/src/textadventure.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 21:07:44.000000 textadventure-0.0.5/src/textadventure.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-16 21:07:44.000000 textadventure-0.0.5/src/textadventure.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-16 21:07:44.000000 textadventure-0.0.5/src/textadventure.egg-info/top_level.txt
```

### Comparing `textadventure-0.0.4/LICENSE.md` & `textadventure-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `textadventure-0.0.4/PKG-INFO` & `textadventure-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textadventure
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small package to make creating your own text adventure games easy!
 Author-email: Matthew James <mattdestroyerpro@gmail.com>
 Project-URL: Homepage, https://github.com/Matt-DESTROYER/TextAdventures
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `textadventure-0.0.4/README.md` & `textadventure-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `textadventure-0.0.4/pyproject.toml` & `textadventure-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "textadventure"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Matthew James", email="mattdestroyerpro@gmail.com" }
 ]
 description = "A small package to make creating your own text adventure games easy!"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `textadventure-0.0.4/src/textadventure/__init__.py` & `textadventure-0.0.5/src/textadventure/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 from .input import readKey, readLine, keys, init_input
 from .menu import menu
 from .output import clear
 from .timing import timeEvent
 
 ACTIONS: list[str] = ["SCENE", "GOTO", "TEXT", "OPTIONS", "OPTION", "INTERACTION", "SUCCESS", "FAIL", "END"]
@@ -108,16 +108,15 @@
 class Interaction(Action):
 	key: str
 	timeout: float
 	success: Success
 	fail: Fail
 	__slots__ = ("key", "timeout", "success", "fail")
 
-	def __init__(self, key: str, timeout: float, success: Success,
-	             fail: Fail) -> None:
+	def __init__(self, key: str, timeout: float, success: Success, fail: Fail) -> None:
 		super().__init__()
 		self.key = key.upper()
 		self.timeout = timeout
 		self.success = success
 		self.fail = fail
 
 	def action(self) -> None:
@@ -260,15 +259,15 @@
 			else:
 				InvalidActionError(action)
 		i += 1
 
 
 def start_game() -> None:
 	"""Starts the text adventure game using any already loaded scenes."""
-    init_input()
+	init_input()
 	global game_running
 	global scenes
 	global current_scene
 	game_running = True
 	while game_running:
 		i = 0
 		while i < len(scenes[current_scene]):
```

### Comparing `textadventure-0.0.4/src/textadventure/input.py` & `textadventure-0.0.5/src/textadventure/input.py`

 * *Files identical despite different names*

### Comparing `textadventure-0.0.4/src/textadventure/menu.py` & `textadventure-0.0.5/src/textadventure/menu.py`

 * *Files identical despite different names*

### Comparing `textadventure-0.0.4/src/textadventure.egg-info/PKG-INFO` & `textadventure-0.0.5/src/textadventure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textadventure
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small package to make creating your own text adventure games easy!
 Author-email: Matthew James <mattdestroyerpro@gmail.com>
 Project-URL: Homepage, https://github.com/Matt-DESTROYER/TextAdventures
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

