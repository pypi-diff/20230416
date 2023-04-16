# Comparing `tmp/textadventure-0.0.1.tar.gz` & `tmp/textadventure-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textadventure-0.0.1.tar", last modified: Sun Apr 16 11:41:44 2023, max compression
+gzip compressed data, was "textadventure-0.0.2.tar", last modified: Sun Apr 16 11:48:25 2023, max compression
```

## Comparing `textadventure-0.0.1.tar` & `textadventure-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 11:41:44.605528 textadventure-0.0.1/
--rw-rw-rw-   0        0        0    12438 2023-04-16 09:59:23.000000 textadventure-0.0.1/LICENSE.md
--rw-rw-rw-   0        0        0     4513 2023-04-16 11:41:44.605528 textadventure-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4124 2023-04-16 11:13:56.000000 textadventure-0.0.1/README.md
--rw-rw-rw-   0        0        0      460 2023-04-16 11:41:03.000000 textadventure-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-16 11:41:44.606536 textadventure-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-16 11:41:44.586501 textadventure-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 11:41:44.593525 textadventure-0.0.1/src/textadventure/
--rw-rw-rw-   0        0        0       21 2023-04-16 11:34:32.000000 textadventure-0.0.1/src/textadventure/__init__.py
--rw-rw-rw-   0        0        0     6194 2023-04-16 11:32:58.000000 textadventure-0.0.1/src/textadventure/__main__.py
--rw-rw-rw-   0        0        0     2409 2023-04-16 11:17:09.000000 textadventure-0.0.1/src/textadventure/input.py
--rw-rw-rw-   0        0        0      697 2023-04-16 07:11:59.000000 textadventure-0.0.1/src/textadventure/menu.py
--rw-rw-rw-   0        0        0      255 2023-04-16 06:46:12.000000 textadventure-0.0.1/src/textadventure/output.py
--rw-rw-rw-   0        0        0      238 2023-04-16 05:25:27.000000 textadventure-0.0.1/src/textadventure/timing.py
-drwxrwxrwx   0        0        0        0 2023-04-16 11:41:44.604527 textadventure-0.0.1/src/textadventure.egg-info/
--rw-rw-rw-   0        0        0     4513 2023-04-16 11:41:44.000000 textadventure-0.0.1/src/textadventure.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      368 2023-04-16 11:41:44.000000 textadventure-0.0.1/src/textadventure.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 11:41:44.000000 textadventure-0.0.1/src/textadventure.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-16 11:41:44.000000 textadventure-0.0.1/src/textadventure.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 11:48:25.624158 textadventure-0.0.2/
+-rw-rw-rw-   0        0        0    12438 2023-04-16 09:59:23.000000 textadventure-0.0.2/LICENSE.md
+-rw-rw-rw-   0        0        0     5448 2023-04-16 11:48:25.623158 textadventure-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4986 2023-04-16 11:43:36.000000 textadventure-0.0.2/README.md
+-rw-rw-rw-   0        0        0      568 2023-04-16 11:47:46.000000 textadventure-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 11:48:25.624158 textadventure-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 11:48:25.600153 textadventure-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 11:48:25.608154 textadventure-0.0.2/src/textadventure/
+-rw-rw-rw-   0        0        0       21 2023-04-16 11:46:17.000000 textadventure-0.0.2/src/textadventure/__init__.py
+-rw-rw-rw-   0        0        0     6194 2023-04-16 11:32:58.000000 textadventure-0.0.2/src/textadventure/__main__.py
+-rw-rw-rw-   0        0        0     2409 2023-04-16 11:17:09.000000 textadventure-0.0.2/src/textadventure/input.py
+-rw-rw-rw-   0        0        0      697 2023-04-16 07:11:59.000000 textadventure-0.0.2/src/textadventure/menu.py
+-rw-rw-rw-   0        0        0      255 2023-04-16 06:46:12.000000 textadventure-0.0.2/src/textadventure/output.py
+-rw-rw-rw-   0        0        0      238 2023-04-16 05:25:27.000000 textadventure-0.0.2/src/textadventure/timing.py
+drwxrwxrwx   0        0        0        0 2023-04-16 11:48:25.622158 textadventure-0.0.2/src/textadventure.egg-info/
+-rw-rw-rw-   0        0        0     5448 2023-04-16 11:48:25.000000 textadventure-0.0.2/src/textadventure.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2023-04-16 11:48:25.000000 textadventure-0.0.2/src/textadventure.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 11:48:25.000000 textadventure-0.0.2/src/textadventure.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-16 11:48:25.000000 textadventure-0.0.2/src/textadventure.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-16 11:48:25.000000 textadventure-0.0.2/src/textadventure.egg-info/top_level.txt
```

### Comparing `textadventure-0.0.1/LICENSE.md` & `textadventure-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `textadventure-0.0.1/PKG-INFO` & `textadventure-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,42 @@
-Metadata-Version: 2.1
-Name: textadventure
-Version: 0.0.1
-Summary: A small package to make creating your own text adventure games easy!
-Author-email: Matthew James <mattdestroyerpro@gmail.com>
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-# Text Adventures
+# Text Adventure
 
 This library aims to enable you to easily create your own text adventure games!
 
 ## Getting started
 Simply install the library using `pip` or your package manager:
 ```shell
-pip install TextAdventures
+pip install textadventures
 ```
 
 Import the package in your code:
 ```python
-import TextAdventures
+import textadventures
 ```
 
 And you're good to go!
 
 ## Loading and running scenes
 The scene language enables you to create your own text adventure games with almost zero code!
 
 To load scenes from a file, use the `load_scenes` method:
 ```python
-import TextAdventures
+import textadventures
 
-TextAdventures.load_scene("Scenes.txt")
+textadventures.load_scene("Scenes.txt")
 ```
 You can load scenes from any generic text file.
 You can load scenes from as many files as you want, the only thing to remember is that the first scene in the first file you load will become the starting scene.
 
 To run your game using those scenes, call the `start_game` method:
 ```python
 import textadventures
 
-TextAdventures.load_scene("Scenes.txt")
-TextAdventures.start_game()
+textadventures.load_scene("Scenes.txt")
+textadventures.start_game()
 ```
 
 And that's all the code you will need to run your text adventure games!
 
 ## Getting to know Scene
 Scene is the mini 'language' I created to remove all the coding from making a text adventure game.
 The Scene language is very basic and should be relatively easy to get your head around.
@@ -65,8 +54,77 @@
 - `[INTERACTION]` - This indicates an interaction must occur from the player. The subsequent two space separated 'words' must be the ASCII key which the user must press followed by the number of seconds the user has to press this key (in that order).
 - `[SUCCESS]` - This is a conditional statement indicating the user completed the above interaction action successully. This can **only** follow an `[INTERACTION]` action or a `[FAIL]` action and can **only** be followed by a `[GOTO]` action.
 - `[FAIL]` - This is a conditional statement indicating the user did not complete the above interaction action successully. This can **only** follow an `[INTERACTION]` action or a `[SUCCESS]` action and can **only** be followed by a `[GOTO]` action.
 
 More information:
 > The Scene language is currently a very basic prototype, it is my intention to make this into a full-fledged custom programming language which can be run using this module or transpiled to C++ and compiled using a tool I will create when the language is much more complete.
 
-<a rel="license" href="http://creativecommons.org/licenses/by-nd/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nd/4.0/">Creative Commons Attribution-NoDerivatives 4.0 International License</a>.
+## A basic demo
+`main.scn`:
+```
+[SCENE] Generic Scene
+
+[TEXT] Multiline
+description!
+
+[OPTIONS] Pick an option:
+[OPTION] A
+[GOTO] Scene A
+[OPTION] B
+[GOTO] Scene B
+[OPTION] C
+[GOTO] Scene C
+
+[SCENE] Interactive Scene
+
+[TEXT]
+Quick! Press the space key within two seconds!
+
+[INTERACTION] SPACE 2
+[SUCCESS]
+[GOTO] Interaction Success
+[FAIL]
+[GOTO] Interaction Fail
+
+[SCENE] Scene A
+
+[TEXT]
+This is Scene A!
+
+[GOTO] Interactive Scene
+
+[SCENE] Scene B
+
+[TEXT]
+This is Scene B!
+
+[GOTO] Interactive Scene
+
+[SCENE] Scene C
+
+[TEXT]
+This is Scene C!
+
+[GOTO] Interactive Scene
+
+[SCENE] Interaction Success
+
+[TEXT]
+You did it!
+
+[GOTO] Final Scene
+
+[SCENE] Interaction Fail
+
+[TEXT]
+Oh no! You didn't interact in time...
+
+[GOTO] Final Scene
+
+[SCENE] Final Scene
+
+[TEXT]
+That's all for now folks!
+
+[END]
+```
+<a rel="license" href="http://creativecommons.org/licenses/by-nd/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nd/4.0/">Creative Commons Attribution-NoDerivatives 4.0 International License</a>.
```

### Comparing `textadventure-0.0.1/src/textadventure/__main__.py` & `textadventure-0.0.2/src/textadventure/__main__.py`

 * *Files identical despite different names*

### Comparing `textadventure-0.0.1/src/textadventure/input.py` & `textadventure-0.0.2/src/textadventure/input.py`

 * *Files identical despite different names*

### Comparing `textadventure-0.0.1/src/textadventure/menu.py` & `textadventure-0.0.2/src/textadventure/menu.py`

 * *Files identical despite different names*

### Comparing `textadventure-0.0.1/src/textadventure.egg-info/PKG-INFO` & `textadventure-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 Metadata-Version: 2.1
 Name: textadventure
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small package to make creating your own text adventure games easy!
 Author-email: Matthew James <mattdestroyerpro@gmail.com>
+Project-URL: Homepage, https://github.com/Matt-DESTROYER/TextAdventures
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# Text Adventures
+# Text Adventure
 
 This library aims to enable you to easily create your own text adventure games!
 
 ## Getting started
 Simply install the library using `pip` or your package manager:
 ```shell
-pip install TextAdventures
+pip install textadventures
 ```
 
 Import the package in your code:
 ```python
-import TextAdventures
+import textadventures
 ```
 
 And you're good to go!
 
 ## Loading and running scenes
 The scene language enables you to create your own text adventure games with almost zero code!
 
 To load scenes from a file, use the `load_scenes` method:
 ```python
-import TextAdventures
+import textadventures
 
-TextAdventures.load_scene("Scenes.txt")
+textadventures.load_scene("Scenes.txt")
 ```
 You can load scenes from any generic text file.
 You can load scenes from as many files as you want, the only thing to remember is that the first scene in the first file you load will become the starting scene.
 
 To run your game using those scenes, call the `start_game` method:
 ```python
 import textadventures
 
-TextAdventures.load_scene("Scenes.txt")
-TextAdventures.start_game()
+textadventures.load_scene("Scenes.txt")
+textadventures.start_game()
 ```
 
 And that's all the code you will need to run your text adventure games!
 
 ## Getting to know Scene
 Scene is the mini 'language' I created to remove all the coding from making a text adventure game.
 The Scene language is very basic and should be relatively easy to get your head around.
@@ -65,8 +66,77 @@
 - `[INTERACTION]` - This indicates an interaction must occur from the player. The subsequent two space separated 'words' must be the ASCII key which the user must press followed by the number of seconds the user has to press this key (in that order).
 - `[SUCCESS]` - This is a conditional statement indicating the user completed the above interaction action successully. This can **only** follow an `[INTERACTION]` action or a `[FAIL]` action and can **only** be followed by a `[GOTO]` action.
 - `[FAIL]` - This is a conditional statement indicating the user did not complete the above interaction action successully. This can **only** follow an `[INTERACTION]` action or a `[SUCCESS]` action and can **only** be followed by a `[GOTO]` action.
 
 More information:
 > The Scene language is currently a very basic prototype, it is my intention to make this into a full-fledged custom programming language which can be run using this module or transpiled to C++ and compiled using a tool I will create when the language is much more complete.
 
+## A basic demo
+`main.scn`:
+```
+[SCENE] Generic Scene
+
+[TEXT] Multiline
+description!
+
+[OPTIONS] Pick an option:
+[OPTION] A
+[GOTO] Scene A
+[OPTION] B
+[GOTO] Scene B
+[OPTION] C
+[GOTO] Scene C
+
+[SCENE] Interactive Scene
+
+[TEXT]
+Quick! Press the space key within two seconds!
+
+[INTERACTION] SPACE 2
+[SUCCESS]
+[GOTO] Interaction Success
+[FAIL]
+[GOTO] Interaction Fail
+
+[SCENE] Scene A
+
+[TEXT]
+This is Scene A!
+
+[GOTO] Interactive Scene
+
+[SCENE] Scene B
+
+[TEXT]
+This is Scene B!
+
+[GOTO] Interactive Scene
+
+[SCENE] Scene C
+
+[TEXT]
+This is Scene C!
+
+[GOTO] Interactive Scene
+
+[SCENE] Interaction Success
+
+[TEXT]
+You did it!
+
+[GOTO] Final Scene
+
+[SCENE] Interaction Fail
+
+[TEXT]
+Oh no! You didn't interact in time...
+
+[GOTO] Final Scene
+
+[SCENE] Final Scene
+
+[TEXT]
+That's all for now folks!
+
+[END]
+```
 <a rel="license" href="http://creativecommons.org/licenses/by-nd/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nd/4.0/">Creative Commons Attribution-NoDerivatives 4.0 International License</a>.
```

