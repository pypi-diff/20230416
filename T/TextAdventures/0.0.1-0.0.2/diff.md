# Comparing `tmp/TextAdventures-0.0.1.tar.gz` & `tmp/TextAdventures-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TextAdventures-0.0.1.tar", last modified: Sun Apr 16 11:04:39 2023, max compression
+gzip compressed data, was "TextAdventures-0.0.2.tar", last modified: Sun Apr 16 11:25:49 2023, max compression
```

## Comparing `TextAdventures-0.0.1.tar` & `TextAdventures-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 11:04:39.368659 TextAdventures-0.0.1/
--rw-rw-rw-   0        0        0    12438 2023-04-16 09:59:23.000000 TextAdventures-0.0.1/LICENSE.md
--rw-rw-rw-   0        0        0     4514 2023-04-16 11:04:39.368659 TextAdventures-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4124 2023-04-16 10:17:21.000000 TextAdventures-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 11:04:39.363562 TextAdventures-0.0.1/TextAdventures.egg-info/
--rw-rw-rw-   0        0        0     4514 2023-04-16 11:04:39.000000 TextAdventures-0.0.1/TextAdventures.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-04-16 11:04:39.000000 TextAdventures-0.0.1/TextAdventures.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 11:04:39.000000 TextAdventures-0.0.1/TextAdventures.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-16 11:04:39.000000 TextAdventures-0.0.1/TextAdventures.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      461 2023-04-16 10:58:02.000000 TextAdventures-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-16 11:04:39.368659 TextAdventures-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-16 11:04:39.353057 TextAdventures-0.0.1/textadventures/
-drwxrwxrwx   0        0        0        0 2023-04-16 11:04:39.367653 TextAdventures-0.0.1/textadventures/src/
--rw-rw-rw-   0        0        0       21 2023-04-16 07:21:16.000000 TextAdventures-0.0.1/textadventures/src/__init__.py
--rw-rw-rw-   0        0        0     6181 2023-04-16 10:41:19.000000 TextAdventures-0.0.1/textadventures/src/__main__.py
--rw-rw-rw-   0        0        0     2196 2023-04-16 05:47:15.000000 TextAdventures-0.0.1/textadventures/src/input.py
--rw-rw-rw-   0        0        0      697 2023-04-16 07:11:59.000000 TextAdventures-0.0.1/textadventures/src/menu.py
--rw-rw-rw-   0        0        0      255 2023-04-16 06:46:12.000000 TextAdventures-0.0.1/textadventures/src/output.py
--rw-rw-rw-   0        0        0      238 2023-04-16 05:25:27.000000 TextAdventures-0.0.1/textadventures/src/timing.py
+drwxrwxrwx   0        0        0        0 2023-04-16 11:25:49.287671 TextAdventures-0.0.2/
+-rw-rw-rw-   0        0        0    12438 2023-04-16 09:59:23.000000 TextAdventures-0.0.2/LICENSE.md
+-rw-rw-rw-   0        0        0     4514 2023-04-16 11:25:49.287671 TextAdventures-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4124 2023-04-16 11:13:56.000000 TextAdventures-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 11:25:49.282213 TextAdventures-0.0.2/TextAdventures.egg-info/
+-rw-rw-rw-   0        0        0     4514 2023-04-16 11:25:49.000000 TextAdventures-0.0.2/TextAdventures.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-04-16 11:25:49.000000 TextAdventures-0.0.2/TextAdventures.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 11:25:49.000000 TextAdventures-0.0.2/TextAdventures.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-16 11:25:49.000000 TextAdventures-0.0.2/TextAdventures.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      461 2023-04-16 11:25:09.000000 TextAdventures-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 11:25:49.287671 TextAdventures-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 11:25:49.267926 TextAdventures-0.0.2/textadventures/
+drwxrwxrwx   0        0        0        0 2023-04-16 11:25:49.286662 TextAdventures-0.0.2/textadventures/src/
+-rw-rw-rw-   0        0        0       21 2023-04-16 11:25:20.000000 TextAdventures-0.0.2/textadventures/src/__init__.py
+-rw-rw-rw-   0        0        0     6198 2023-04-16 11:17:28.000000 TextAdventures-0.0.2/textadventures/src/__main__.py
+-rw-rw-rw-   0        0        0     2409 2023-04-16 11:17:09.000000 TextAdventures-0.0.2/textadventures/src/input.py
+-rw-rw-rw-   0        0        0      697 2023-04-16 07:11:59.000000 TextAdventures-0.0.2/textadventures/src/menu.py
+-rw-rw-rw-   0        0        0      255 2023-04-16 06:46:12.000000 TextAdventures-0.0.2/textadventures/src/output.py
+-rw-rw-rw-   0        0        0      238 2023-04-16 05:25:27.000000 TextAdventures-0.0.2/textadventures/src/timing.py
```

### Comparing `TextAdventures-0.0.1/LICENSE.md` & `TextAdventures-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `TextAdventures-0.0.1/PKG-INFO` & `TextAdventures-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TextAdventures
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small package to make creating your own text adventure games easy!
 Author-email: Matthew James <mattdestroyerpro@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -12,42 +12,42 @@
 # Text Adventures
 
 This library aims to enable you to easily create your own text adventure games!
 
 ## Getting started
 Simply install the library using `pip` or your package manager:
 ```shell
-pip install textadventures
+pip install TextAdventures
 ```
 
 Import the package in your code:
 ```python
-import textadventures
+import TextAdventures
 ```
 
 And you're good to go!
 
 ## Loading and running scenes
 The scene language enables you to create your own text adventure games with almost zero code!
 
 To load scenes from a file, use the `load_scenes` method:
 ```python
-import textadventures
+import TextAdventures
 
-textadventures.load_scene("Scenes.txt")
+TextAdventures.load_scene("Scenes.txt")
 ```
 You can load scenes from any generic text file.
 You can load scenes from as many files as you want, the only thing to remember is that the first scene in the first file you load will become the starting scene.
 
 To run your game using those scenes, call the `start_game` method:
 ```python
 import textadventures
 
-textadventures.load_scene("Scenes.txt")
-textadventures.start_game()
+TextAdventures.load_scene("Scenes.txt")
+TextAdventures.start_game()
 ```
 
 And that's all the code you will need to run your text adventure games!
 
 ## Getting to know Scene
 Scene is the mini 'language' I created to remove all the coding from making a text adventure game.
 The Scene language is very basic and should be relatively easy to get your head around.
```

### Comparing `TextAdventures-0.0.1/README.md` & `TextAdventures-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # Text Adventures
 
 This library aims to enable you to easily create your own text adventure games!
 
 ## Getting started
 Simply install the library using `pip` or your package manager:
 ```shell
-pip install textadventures
+pip install TextAdventures
 ```
 
 Import the package in your code:
 ```python
-import textadventures
+import TextAdventures
 ```
 
 And you're good to go!
 
 ## Loading and running scenes
 The scene language enables you to create your own text adventure games with almost zero code!
 
 To load scenes from a file, use the `load_scenes` method:
 ```python
-import textadventures
+import TextAdventures
 
-textadventures.load_scene("Scenes.txt")
+TextAdventures.load_scene("Scenes.txt")
 ```
 You can load scenes from any generic text file.
 You can load scenes from as many files as you want, the only thing to remember is that the first scene in the first file you load will become the starting scene.
 
 To run your game using those scenes, call the `start_game` method:
 ```python
 import textadventures
 
-textadventures.load_scene("Scenes.txt")
-textadventures.start_game()
+TextAdventures.load_scene("Scenes.txt")
+TextAdventures.start_game()
 ```
 
 And that's all the code you will need to run your text adventure games!
 
 ## Getting to know Scene
 Scene is the mini 'language' I created to remove all the coding from making a text adventure game.
 The Scene language is very basic and should be relatively easy to get your head around.
```

### Comparing `TextAdventures-0.0.1/TextAdventures.egg-info/PKG-INFO` & `TextAdventures-0.0.2/TextAdventures.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TextAdventures
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small package to make creating your own text adventure games easy!
 Author-email: Matthew James <mattdestroyerpro@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -12,42 +12,42 @@
 # Text Adventures
 
 This library aims to enable you to easily create your own text adventure games!
 
 ## Getting started
 Simply install the library using `pip` or your package manager:
 ```shell
-pip install textadventures
+pip install TextAdventures
 ```
 
 Import the package in your code:
 ```python
-import textadventures
+import TextAdventures
 ```
 
 And you're good to go!
 
 ## Loading and running scenes
 The scene language enables you to create your own text adventure games with almost zero code!
 
 To load scenes from a file, use the `load_scenes` method:
 ```python
-import textadventures
+import TextAdventures
 
-textadventures.load_scene("Scenes.txt")
+TextAdventures.load_scene("Scenes.txt")
 ```
 You can load scenes from any generic text file.
 You can load scenes from as many files as you want, the only thing to remember is that the first scene in the first file you load will become the starting scene.
 
 To run your game using those scenes, call the `start_game` method:
 ```python
 import textadventures
 
-textadventures.load_scene("Scenes.txt")
-textadventures.start_game()
+TextAdventures.load_scene("Scenes.txt")
+TextAdventures.start_game()
 ```
 
 And that's all the code you will need to run your text adventure games!
 
 ## Getting to know Scene
 Scene is the mini 'language' I created to remove all the coding from making a text adventure game.
 The Scene language is very basic and should be relatively easy to get your head around.
```

### Comparing `TextAdventures-0.0.1/textadventures/src/__main__.py` & `TextAdventures-0.0.2/textadventures/src/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,14 +261,15 @@
 			else:
 				InvalidActionError(action)
 		i += 1
 
 
 def start_game() -> None:
 	"""Starts the text adventure game using any already loaded scenes."""
+    init_input()
 	global game_running
 	global scenes
 	global current_scene
 	game_running = True
 	while game_running:
 		i = 0
 		while i < len(scenes[current_scene]):
```

### Comparing `TextAdventures-0.0.1/textadventures/src/input.py` & `TextAdventures-0.0.2/textadventures/src/input.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,33 +6,39 @@
 
 class InputThread(Thread):
 	def __init__(self, callback):
 		self.input_cbk = callback
 		super(InputThread, self).__init__(name="input-thread")
 		self.start()
 
-	def run(self):
+	def run(self) -> None:
 		while True:
 			self.input_cbk(getkey())
 
 
-_input_print = True
-_input_reading = True
-_input_buffer = ""
-_input_complete = False
+_input_thread: InputThread = None
+_input_print: bool = True
+_input_reading: bool = True
+_input_buffer: str = ""
+_input_complete: bool = False
 
 
 def _finish_condition(key):
 	pass
 
 
-def init_input():
+_input_initialised: bool = False
+def init_input() -> InputThread:
+    if _input_initialised:
+        return 
+    _input_initialised = True
+    
 	dont_print = [keys.LEFT, keys.RIGHT, keys.UP, keys.DOWN]
 
-	def key_press(key):
+	def key_press(key) -> None:
 		global _input_print
 		global _input_reading
 		global _input_buffer
 		global _input_complete
 		if _finish_condition(key):
 			_input_complete = True
 			if _input_print:
@@ -52,15 +58,15 @@
 					sys.stdout.flush()
 
 	input_thread = InputThread(key_press)
 
 	return input_thread
 
 
-def readLine(prompt: str = "", display: bool = True):
+def readLine(prompt: str = "", display: bool = True) -> str:
 	global _input_print
 	global _input_reading
 	global _input_buffer
 	global _input_complete
 	global _finish_condition
 	_input_print = display
 	_input_reading = True
@@ -78,15 +84,15 @@
 	result = _input_buffer
 	_input_reading = False
 	_input_buffer = ""
 	_input_complete = False
 	return result
 
 
-def readKey(prompt: str = "", display: bool = True):
+def readKey(prompt: str = "", display: bool = True) -> str:
 	global _input_print
 	global _input_reading
 	global _input_buffer
 	global _input_complete
 	global _finish_condition
 	_input_print = display
 	_input_reading = True
```

### Comparing `TextAdventures-0.0.1/textadventures/src/menu.py` & `TextAdventures-0.0.2/textadventures/src/menu.py`

 * *Files identical despite different names*

