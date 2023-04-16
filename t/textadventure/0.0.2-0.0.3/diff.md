# Comparing `tmp/textadventure-0.0.2.tar.gz` & `tmp/textadventure-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textadventure-0.0.2.tar", last modified: Sun Apr 16 11:48:25 2023, max compression
+gzip compressed data, was "textadventure-0.0.3.tar", last modified: Sun Apr 16 11:56:37 2023, max compression
```

## Comparing `textadventure-0.0.2.tar` & `textadventure-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 11:48:25.624158 textadventure-0.0.2/
--rw-rw-rw-   0        0        0    12438 2023-04-16 09:59:23.000000 textadventure-0.0.2/LICENSE.md
--rw-rw-rw-   0        0        0     5448 2023-04-16 11:48:25.623158 textadventure-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4986 2023-04-16 11:43:36.000000 textadventure-0.0.2/README.md
--rw-rw-rw-   0        0        0      568 2023-04-16 11:47:46.000000 textadventure-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-16 11:48:25.624158 textadventure-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-16 11:48:25.600153 textadventure-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 11:48:25.608154 textadventure-0.0.2/src/textadventure/
--rw-rw-rw-   0        0        0       21 2023-04-16 11:46:17.000000 textadventure-0.0.2/src/textadventure/__init__.py
--rw-rw-rw-   0        0        0     6194 2023-04-16 11:32:58.000000 textadventure-0.0.2/src/textadventure/__main__.py
--rw-rw-rw-   0        0        0     2409 2023-04-16 11:17:09.000000 textadventure-0.0.2/src/textadventure/input.py
--rw-rw-rw-   0        0        0      697 2023-04-16 07:11:59.000000 textadventure-0.0.2/src/textadventure/menu.py
--rw-rw-rw-   0        0        0      255 2023-04-16 06:46:12.000000 textadventure-0.0.2/src/textadventure/output.py
--rw-rw-rw-   0        0        0      238 2023-04-16 05:25:27.000000 textadventure-0.0.2/src/textadventure/timing.py
-drwxrwxrwx   0        0        0        0 2023-04-16 11:48:25.622158 textadventure-0.0.2/src/textadventure.egg-info/
--rw-rw-rw-   0        0        0     5448 2023-04-16 11:48:25.000000 textadventure-0.0.2/src/textadventure.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2023-04-16 11:48:25.000000 textadventure-0.0.2/src/textadventure.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 11:48:25.000000 textadventure-0.0.2/src/textadventure.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-16 11:48:25.000000 textadventure-0.0.2/src/textadventure.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-16 11:48:25.000000 textadventure-0.0.2/src/textadventure.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 11:56:37.743970 textadventure-0.0.3/
+-rw-rw-rw-   0        0        0    12438 2023-04-16 09:59:23.000000 textadventure-0.0.3/LICENSE.md
+-rw-rw-rw-   0        0        0     5448 2023-04-16 11:56:37.743970 textadventure-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4986 2023-04-16 11:43:36.000000 textadventure-0.0.3/README.md
+-rw-rw-rw-   0        0        0      568 2023-04-16 11:55:20.000000 textadventure-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 11:56:37.743970 textadventure-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 11:56:37.722546 textadventure-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 11:56:37.728546 textadventure-0.0.3/src/textadventure/
+-rw-rw-rw-   0        0        0     6495 2023-04-16 11:56:03.000000 textadventure-0.0.3/src/textadventure/__init__.py
+-rw-rw-rw-   0        0        0     2409 2023-04-16 11:17:09.000000 textadventure-0.0.3/src/textadventure/input.py
+-rw-rw-rw-   0        0        0      697 2023-04-16 07:11:59.000000 textadventure-0.0.3/src/textadventure/menu.py
+-rw-rw-rw-   0        0        0      255 2023-04-16 06:46:12.000000 textadventure-0.0.3/src/textadventure/output.py
+-rw-rw-rw-   0        0        0      238 2023-04-16 05:25:27.000000 textadventure-0.0.3/src/textadventure/timing.py
+drwxrwxrwx   0        0        0        0 2023-04-16 11:56:37.742964 textadventure-0.0.3/src/textadventure.egg-info/
+-rw-rw-rw-   0        0        0     5448 2023-04-16 11:56:37.000000 textadventure-0.0.3/src/textadventure.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-04-16 11:56:37.000000 textadventure-0.0.3/src/textadventure.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 11:56:37.000000 textadventure-0.0.3/src/textadventure.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-16 11:56:37.000000 textadventure-0.0.3/src/textadventure.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-16 11:56:37.000000 textadventure-0.0.3/src/textadventure.egg-info/top_level.txt
```

### Comparing `textadventure-0.0.2/LICENSE.md` & `textadventure-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `textadventure-0.0.2/PKG-INFO` & `textadventure-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textadventure
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small package to make creating your own text adventure games easy!
 Author-email: Matthew James <mattdestroyerpro@gmail.com>
 Project-URL: Homepage, https://github.com/Matt-DESTROYER/TextAdventures
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `textadventure-0.0.2/README.md` & `textadventure-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `textadventure-0.0.2/pyproject.toml` & `textadventure-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "textadventure"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Matthew James", email="mattdestroyerpro@gmail.com" }
 ]
 description = "A small package to make creating your own text adventure games easy!"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `textadventure-0.0.2/src/textadventure/__main__.py` & `textadventure-0.0.3/src/textadventure/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,276 +1,278 @@
-from .input import readKey, readLine, keys, init_input
-from .menu import menu
-from .output import clear
-from .timing import timeEvent
-
-ACTIONS: list[str] = ["SCENE", "GOTO", "TEXT", "OPTIONS", "OPTION", "INTERACTION", "SUCCESS", "FAIL", "END"]
-_ACTIONS: list[str] = ["[" + action + "]" for action in ACTIONS]
-
-game_running: bool = False
-scenes: dict[str, list] = {}
-current_scene: str = None
-
-
-class Action:
-	__slots__ = ()
-
-	def __init__(self) -> None:
-		pass
-
-	def action(self) -> None:
-		pass
-
-
-class InvalidActionError(Exception):
-	action: str
-	message: str
-	__slots__ = ("action", "message")
-
-	def __init__(self, action: str) -> None:
-		self.action = action
-		self.message = f"The action '{action}' is not a valid action."
-		super().__init__(self.message)
-
-
-class Goto(Action):
-	scene: str
-	__slots__ = ("scene")
-
-	def __init__(self, scene: str) -> None:
-		super().__init__()
-		self.scene = scene
-
-	def action(self) -> None:
-		global current_scene
-		current_scene = self.scene
-
-
-class Text(Action):
-	text: str
-	__slots__ = ("text")
-
-	def __init__(self, text: str) -> None:
-		super().__init__()
-		self.text = text
-
-	def action(self) -> None:
-		print(self.text)
-		readLine("> Continue <\n", False)
-
-
-class Options(Action):
-	text: str
-	options: list[str]
-	actions: list[str]
-	__slots__ = ("text", "options", "actions")
-
-	def __init__(self, text: str, options: list[str]) -> None:
-		super().__init__()
-		self.text = text
-		self.options = [_option[0] for _option in options]
-		self.actions = [_option[1] for _option in options]
-
-	def action(self) -> None:
-		action = self.actions[menu(self.text, self.options)]
-		if action[0:6].upper() == "[GOTO]":
-			global current_scene
-			current_scene = action[6:].strip()
-
-
-class Success(Action):
-	scene: str
-	__slots__ = ("scene")
-
-	def __init__(self, scene: str) -> None:
-		super().__init__()
-		self.scene = scene
-
-	def action(self) -> None:
-		global current_scene
-		current_scene = self.scene
-
-
-class Fail(Action):
-	scene: str
-	__slots__ = ("scene")
-
-	def __init__(self, scene: str) -> None:
-		super().__init__()
-		self.scene = scene
-
-	def action(self) -> None:
-		global current_scene
-		current_scene = self.scene
-
-
-class Interaction(Action):
-	key: str
-	timeout: float
-	success: Success
-	fail: Fail
-	__slots__ = ("key", "timeout", "success", "fail")
-
-	def __init__(self, key: str, timeout: float, success: Success,
-	             fail: Fail) -> None:
-		super().__init__()
-		self.key = key.upper()
-		self.timeout = timeout
-		self.success = success
-		self.fail = fail
-
-	def action(self) -> None:
-
-		def checkSuccess(target_key):
-			return readKey("", False) == getattr(keys, target_key)
-
-		result = timeEvent(checkSuccess, self.key)
-		if result[1]:
-			if result[0] < self.timeout:
-				self.success.action()
-			else:
-				self.fail.action()
-		else:
-			self.fail.action()
-
-
-class End(Action):
-	__slots__ = ()
-
-	def __init__(self) -> None:
-		super().__init__()
-
-	def action(self) -> None:
-		global game_running
-		game_running = False
-
-
-def index(_: list | tuple, item: any) -> int:
-	i = 0
-	while i < len(_):
-		if _[i] == item:
-			return i
-		i += 1
-	return -1
-
-
-def load_scenes(file: str) -> None:
-	"""Loads all the scenes from the input file based on it's name/path."""
-	global ACTIONS
-	global _ACTIONS
-	global scenes
-	global current_scene
-	lines = None
-	with open(file, "r") as _scenes:
-		lines = _scenes.read()
-	lines = lines.splitlines()
-	scene = None
-	i = 0
-	while i < len(lines):
-		line = lines[i]
-		action_idx = index(_ACTIONS, line.split(" ")[0].strip().upper())
-		if action_idx != -1:
-			action = ACTIONS[action_idx]
-			if action == "SCENE":
-				scene = line[7:]
-				i += 1
-				line = lines[i].strip()
-				while line != "" and line[0] != "[":
-					scene += "\n" + lines[i]
-					i += 1
-					line = lines[i].strip()
-				i -= 1
-				scene = scene.strip()
-				if current_scene == None:
-					current_scene = scene
-				scenes[scene] = []
-			elif action == "GOTO":
-				_scene = line[6:]
-				i += 1
-				line = lines[i].strip()
-				while line != "" and line[0] != "[":
-					_scene += "\n" + lines[i]
-					i += 1
-					line = lines[i].strip()
-				i -= 1
-				_scene = _scene.strip()
-				scenes[scene].append(Goto(_scene))
-			elif action == "TEXT":
-				text = line[6:]
-				i += 1
-				line = lines[i].strip()
-				while line != "" and line[0] != "[":
-					text += "\n" + lines[i]
-					i += 1
-					line = lines[i].strip()
-				scenes[scene].append(Text(text.strip()))
-				i -= 1
-			elif action == "OPTIONS":
-				text = line[9:].strip()
-				i += 1
-				line = lines[i].strip()
-				options = []
-				while line[0:8] == "[OPTION]":
-					print
-					option = line[9:]
-					i += 1
-					line = lines[i].strip()
-					while line != "" and line[0] != "[":
-						option += "\n" + lines[i]
-						i += 1
-						line = lines[i].strip()
-					goto = line
-					line = lines[i].strip()
-					while line != "" and line[0] != "[":
-						goto += "\n" + lines[i]
-						i += 1
-						line = lines[i].strip()
-					goto = goto.strip()
-					options.append([option, goto])
-					i += 1
-					line = lines[i].strip()
-				scenes[scene].append(Options(text, options))
-				i -= 1
-			elif action == "INTERACTION":
-				key, timeout = line[13:].strip().split(" ")
-				i += 1
-				command1 = lines[i].strip().upper()
-				i += 1
-				action1 = lines[i].strip()[6:].strip()
-				i += 1
-				command2 = lines[i].strip().upper()
-				i += 1
-				action2 = lines[i].strip()[6:].strip()
-				success: Success = None
-				fail: Fail = None
-				if command1 == "[SUCCESS]":
-					success = Success(action1)
-				elif command1 == "[FAIL]":
-					fail = Fail(action1)
-				if command2 == "[FAIL]":
-					fail = Fail(action2)
-				elif command2 == "[SUCCESS]":
-					success = Success(action2)
-				scenes[scene].append(Interaction(key, float(timeout), success, fail))
-			elif action == "END":
-				scenes[scene].append(End())
-			elif line == "":
-				continue
-			else:
-				InvalidActionError(action)
-		i += 1
-
-
-def start_game() -> None:
-	"""Starts the text adventure game using any already loaded scenes."""
-    init_input()
-	global game_running
-	global scenes
-	global current_scene
-	game_running = True
-	while game_running:
-		i = 0
-		while i < len(scenes[current_scene]):
-			clear()
-			scenes[current_scene][i].action()
-			i += 1
-	clear()
+__version__ = "0.0.3"
+
+from .input import readKey, readLine, keys, init_input
+from .menu import menu
+from .output import clear
+from .timing import timeEvent
+
+ACTIONS: list[str] = ["SCENE", "GOTO", "TEXT", "OPTIONS", "OPTION", "INTERACTION", "SUCCESS", "FAIL", "END"]
+_ACTIONS: list[str] = ["[" + action + "]" for action in ACTIONS]
+
+game_running: bool = False
+scenes: dict[str, list] = {}
+current_scene: str = None
+
+
+class Action:
+	__slots__ = ()
+
+	def __init__(self) -> None:
+		pass
+
+	def action(self) -> None:
+		pass
+
+
+class InvalidActionError(Exception):
+	action: str
+	message: str
+	__slots__ = ("action", "message")
+
+	def __init__(self, action: str) -> None:
+		self.action = action
+		self.message = f"The action '{action}' is not a valid action."
+		super().__init__(self.message)
+
+
+class Goto(Action):
+	scene: str
+	__slots__ = ("scene")
+
+	def __init__(self, scene: str) -> None:
+		super().__init__()
+		self.scene = scene
+
+	def action(self) -> None:
+		global current_scene
+		current_scene = self.scene
+
+
+class Text(Action):
+	text: str
+	__slots__ = ("text")
+
+	def __init__(self, text: str) -> None:
+		super().__init__()
+		self.text = text
+
+	def action(self) -> None:
+		print(self.text)
+		readLine("> Continue <\n", False)
+
+
+class Options(Action):
+	text: str
+	options: list[str]
+	actions: list[str]
+	__slots__ = ("text", "options", "actions")
+
+	def __init__(self, text: str, options: list[str]) -> None:
+		super().__init__()
+		self.text = text
+		self.options = [_option[0] for _option in options]
+		self.actions = [_option[1] for _option in options]
+
+	def action(self) -> None:
+		action = self.actions[menu(self.text, self.options)]
+		if action[0:6].upper() == "[GOTO]":
+			global current_scene
+			current_scene = action[6:].strip()
+
+
+class Success(Action):
+	scene: str
+	__slots__ = ("scene")
+
+	def __init__(self, scene: str) -> None:
+		super().__init__()
+		self.scene = scene
+
+	def action(self) -> None:
+		global current_scene
+		current_scene = self.scene
+
+
+class Fail(Action):
+	scene: str
+	__slots__ = ("scene")
+
+	def __init__(self, scene: str) -> None:
+		super().__init__()
+		self.scene = scene
+
+	def action(self) -> None:
+		global current_scene
+		current_scene = self.scene
+
+
+class Interaction(Action):
+	key: str
+	timeout: float
+	success: Success
+	fail: Fail
+	__slots__ = ("key", "timeout", "success", "fail")
+
+	def __init__(self, key: str, timeout: float, success: Success,
+	             fail: Fail) -> None:
+		super().__init__()
+		self.key = key.upper()
+		self.timeout = timeout
+		self.success = success
+		self.fail = fail
+
+	def action(self) -> None:
+
+		def checkSuccess(target_key):
+			return readKey("", False) == getattr(keys, target_key)
+
+		result = timeEvent(checkSuccess, self.key)
+		if result[1]:
+			if result[0] < self.timeout:
+				self.success.action()
+			else:
+				self.fail.action()
+		else:
+			self.fail.action()
+
+
+class End(Action):
+	__slots__ = ()
+
+	def __init__(self) -> None:
+		super().__init__()
+
+	def action(self) -> None:
+		global game_running
+		game_running = False
+
+
+def index(_: list | tuple, item: any) -> int:
+	i = 0
+	while i < len(_):
+		if _[i] == item:
+			return i
+		i += 1
+	return -1
+
+
+def load_scenes(file: str) -> None:
+	"""Loads all the scenes from the input file based on it's name/path."""
+	global ACTIONS
+	global _ACTIONS
+	global scenes
+	global current_scene
+	lines = None
+	with open(file, "r") as _scenes:
+		lines = _scenes.read()
+	lines = lines.splitlines()
+	scene = None
+	i = 0
+	while i < len(lines):
+		line = lines[i]
+		action_idx = index(_ACTIONS, line.split(" ")[0].strip().upper())
+		if action_idx != -1:
+			action = ACTIONS[action_idx]
+			if action == "SCENE":
+				scene = line[7:]
+				i += 1
+				line = lines[i].strip()
+				while line != "" and line[0] != "[":
+					scene += "\n" + lines[i]
+					i += 1
+					line = lines[i].strip()
+				i -= 1
+				scene = scene.strip()
+				if current_scene == None:
+					current_scene = scene
+				scenes[scene] = []
+			elif action == "GOTO":
+				_scene = line[6:]
+				i += 1
+				line = lines[i].strip()
+				while line != "" and line[0] != "[":
+					_scene += "\n" + lines[i]
+					i += 1
+					line = lines[i].strip()
+				i -= 1
+				_scene = _scene.strip()
+				scenes[scene].append(Goto(_scene))
+			elif action == "TEXT":
+				text = line[6:]
+				i += 1
+				line = lines[i].strip()
+				while line != "" and line[0] != "[":
+					text += "\n" + lines[i]
+					i += 1
+					line = lines[i].strip()
+				scenes[scene].append(Text(text.strip()))
+				i -= 1
+			elif action == "OPTIONS":
+				text = line[9:].strip()
+				i += 1
+				line = lines[i].strip()
+				options = []
+				while line[0:8] == "[OPTION]":
+					print
+					option = line[9:]
+					i += 1
+					line = lines[i].strip()
+					while line != "" and line[0] != "[":
+						option += "\n" + lines[i]
+						i += 1
+						line = lines[i].strip()
+					goto = line
+					line = lines[i].strip()
+					while line != "" and line[0] != "[":
+						goto += "\n" + lines[i]
+						i += 1
+						line = lines[i].strip()
+					goto = goto.strip()
+					options.append([option, goto])
+					i += 1
+					line = lines[i].strip()
+				scenes[scene].append(Options(text, options))
+				i -= 1
+			elif action == "INTERACTION":
+				key, timeout = line[13:].strip().split(" ")
+				i += 1
+				command1 = lines[i].strip().upper()
+				i += 1
+				action1 = lines[i].strip()[6:].strip()
+				i += 1
+				command2 = lines[i].strip().upper()
+				i += 1
+				action2 = lines[i].strip()[6:].strip()
+				success: Success = None
+				fail: Fail = None
+				if command1 == "[SUCCESS]":
+					success = Success(action1)
+				elif command1 == "[FAIL]":
+					fail = Fail(action1)
+				if command2 == "[FAIL]":
+					fail = Fail(action2)
+				elif command2 == "[SUCCESS]":
+					success = Success(action2)
+				scenes[scene].append(Interaction(key, float(timeout), success, fail))
+			elif action == "END":
+				scenes[scene].append(End())
+			elif line == "":
+				continue
+			else:
+				InvalidActionError(action)
+		i += 1
+
+
+def start_game() -> None:
+	"""Starts the text adventure game using any already loaded scenes."""
+    init_input()
+	global game_running
+	global scenes
+	global current_scene
+	game_running = True
+	while game_running:
+		i = 0
+		while i < len(scenes[current_scene]):
+			clear()
+			scenes[current_scene][i].action()
+			i += 1
+	clear()
```

### Comparing `textadventure-0.0.2/src/textadventure/input.py` & `textadventure-0.0.3/src/textadventure/input.py`

 * *Files identical despite different names*

### Comparing `textadventure-0.0.2/src/textadventure/menu.py` & `textadventure-0.0.3/src/textadventure/menu.py`

 * *Files identical despite different names*

### Comparing `textadventure-0.0.2/src/textadventure.egg-info/PKG-INFO` & `textadventure-0.0.3/src/textadventure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textadventure
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small package to make creating your own text adventure games easy!
 Author-email: Matthew James <mattdestroyerpro@gmail.com>
 Project-URL: Homepage, https://github.com/Matt-DESTROYER/TextAdventures
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

