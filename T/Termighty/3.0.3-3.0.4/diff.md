# Comparing `tmp/Termighty-3.0.3.tar.gz` & `tmp/Termighty-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Termighty-3.0.3.tar", last modified: Thu Apr 13 17:18:56 2023, max compression
+gzip compressed data, was "Termighty-3.0.4.tar", last modified: Sun Apr 16 13:54:54 2023, max compression
```

## Comparing `Termighty-3.0.3.tar` & `Termighty-3.0.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 17:18:56.151046 Termighty-3.0.3/
--rw-rw-rw-   0        0        0    35823 2022-09-11 20:43:48.000000 Termighty-3.0.3/LICENSE
--rw-rw-rw-   0        0        0      634 2023-04-13 17:18:56.151546 Termighty-3.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       78 2022-09-11 20:43:48.000000 Termighty-3.0.3/README.md
--rw-rw-rw-   0        0        0      105 2022-09-18 20:12:03.000000 Termighty-3.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      130 2023-04-13 17:18:56.153046 Termighty-3.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1043 2023-04-13 17:18:35.000000 Termighty-3.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:18:56.087046 Termighty-3.0.3/source/
-drwxrwxrwx   0        0        0        0 2023-04-13 17:18:56.107546 Termighty-3.0.3/source/Termighty.egg-info/
--rw-rw-rw-   0        0        0      634 2023-04-13 17:18:56.000000 Termighty-3.0.3/source/Termighty.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      900 2023-04-13 17:18:56.000000 Termighty-3.0.3/source/Termighty.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 17:18:56.000000 Termighty-3.0.3/source/Termighty.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-13 17:18:56.000000 Termighty-3.0.3/source/Termighty.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-13 17:18:56.000000 Termighty-3.0.3/source/Termighty.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 17:18:56.111046 Termighty-3.0.3/source/termighty/
--rw-rw-rw-   0        0        0      115 2022-09-11 20:43:48.000000 Termighty-3.0.3/source/termighty/__init__.py
--rw-rw-rw-   0        0        0      403 2022-09-17 22:33:08.000000 Termighty-3.0.3/source/termighty/config.ini
-drwxrwxrwx   0        0        0        0 2023-04-13 17:18:56.118546 Termighty-3.0.3/source/termighty/data/
--rw-rw-rw-   0        0        0     7971 2022-09-17 14:02:53.000000 Termighty-3.0.3/source/termighty/data/keymaps.json
--rw-rw-rw-   0        0        0    66090 2022-09-11 20:43:48.000000 Termighty-3.0.3/source/termighty/data/rgb.json
--rw-rw-rw-   0        0        0      216 2022-09-11 20:43:48.000000 Termighty-3.0.3/source/termighty/data/styles.json
-drwxrwxrwx   0        0        0        0 2023-04-13 17:18:56.124546 Termighty-3.0.3/source/termighty/obj/
--rw-rw-rw-   0        0        0       54 2022-09-11 20:43:48.000000 Termighty-3.0.3/source/termighty/obj/__init__.py
--rw-rw-rw-   0        0        0    15095 2022-09-18 18:49:31.000000 Termighty-3.0.3/source/termighty/obj/color.py
--rw-rw-rw-   0        0        0    17757 2022-09-18 14:21:27.000000 Termighty-3.0.3/source/termighty/obj/string.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:18:56.133047 Termighty-3.0.3/source/termighty/settings/
--rw-rw-rw-   0        0        0       80 2022-09-11 20:43:48.000000 Termighty-3.0.3/source/termighty/settings/__init__.py
--rw-rw-rw-   0        0        0     1737 2022-09-17 22:33:43.000000 Termighty-3.0.3/source/termighty/settings/config.py
--rw-rw-rw-   0        0        0     1010 2022-09-18 14:22:15.000000 Termighty-3.0.3/source/termighty/settings/data.py
--rw-rw-rw-   0        0        0     1458 2023-04-13 13:51:49.000000 Termighty-3.0.3/source/termighty/settings/system.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:18:56.141546 Termighty-3.0.3/source/termighty/utils/
--rw-rw-rw-   0        0        0       97 2022-09-18 19:41:57.000000 Termighty-3.0.3/source/termighty/utils/__init__.py
--rw-rw-rw-   0        0        0    45163 2023-04-13 14:59:33.000000 Termighty-3.0.3/source/termighty/utils/key_processor.py
--rw-rw-rw-   0        0        0    10100 2023-04-13 14:40:44.000000 Termighty-3.0.3/source/termighty/utils/listener.py
--rw-rw-rw-   0        0        0     5463 2023-04-13 14:00:48.000000 Termighty-3.0.3/source/termighty/utils/term.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:18:56.148046 Termighty-3.0.3/source/termighty/widgets/
--rw-rw-rw-   0        0        0       68 2022-09-12 19:41:55.000000 Termighty-3.0.3/source/termighty/widgets/__init__.py
--rw-rw-rw-   0        0        0    16902 2023-04-13 14:19:25.000000 Termighty-3.0.3/source/termighty/widgets/text_box.py
--rw-rw-rw-   0        0        0    15848 2023-04-13 15:25:28.000000 Termighty-3.0.3/source/termighty/widgets/text_editor.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:54:54.928257 Termighty-3.0.4/
+-rw-rw-rw-   0        0        0    35823 2022-09-11 20:43:48.000000 Termighty-3.0.4/LICENSE
+-rw-rw-rw-   0        0        0    21213 2023-04-16 13:54:54.928758 Termighty-3.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    20657 2023-04-16 13:48:14.000000 Termighty-3.0.4/README.md
+-rw-rw-rw-   0        0        0       93 2023-04-13 17:22:56.000000 Termighty-3.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      130 2023-04-16 13:54:54.931256 Termighty-3.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      929 2023-04-16 12:50:11.000000 Termighty-3.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:54:54.859757 Termighty-3.0.4/source/
+drwxrwxrwx   0        0        0        0 2023-04-16 13:54:54.883757 Termighty-3.0.4/source/Termighty.egg-info/
+-rw-rw-rw-   0        0        0    21213 2023-04-16 13:54:54.000000 Termighty-3.0.4/source/Termighty.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      900 2023-04-16 13:54:54.000000 Termighty-3.0.4/source/Termighty.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 13:54:54.000000 Termighty-3.0.4/source/Termighty.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-16 13:54:54.000000 Termighty-3.0.4/source/Termighty.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-16 13:54:54.000000 Termighty-3.0.4/source/Termighty.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 13:54:54.887256 Termighty-3.0.4/source/termighty/
+-rw-rw-rw-   0        0        0      115 2022-09-11 20:43:48.000000 Termighty-3.0.4/source/termighty/__init__.py
+-rw-rw-rw-   0        0        0      403 2022-09-17 22:33:08.000000 Termighty-3.0.4/source/termighty/config.ini
+drwxrwxrwx   0        0        0        0 2023-04-16 13:54:54.894757 Termighty-3.0.4/source/termighty/data/
+-rw-rw-rw-   0        0        0     7971 2022-09-17 14:02:53.000000 Termighty-3.0.4/source/termighty/data/keymaps.json
+-rw-rw-rw-   0        0        0    66090 2022-09-11 20:43:48.000000 Termighty-3.0.4/source/termighty/data/rgb.json
+-rw-rw-rw-   0        0        0      216 2022-09-11 20:43:48.000000 Termighty-3.0.4/source/termighty/data/styles.json
+drwxrwxrwx   0        0        0        0 2023-04-16 13:54:54.901257 Termighty-3.0.4/source/termighty/obj/
+-rw-rw-rw-   0        0        0       54 2022-09-11 20:43:48.000000 Termighty-3.0.4/source/termighty/obj/__init__.py
+-rw-rw-rw-   0        0        0    15095 2022-09-18 18:49:31.000000 Termighty-3.0.4/source/termighty/obj/color.py
+-rw-rw-rw-   0        0        0    17757 2022-09-18 14:21:27.000000 Termighty-3.0.4/source/termighty/obj/string.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:54:54.909257 Termighty-3.0.4/source/termighty/settings/
+-rw-rw-rw-   0        0        0       80 2022-09-11 20:43:48.000000 Termighty-3.0.4/source/termighty/settings/__init__.py
+-rw-rw-rw-   0        0        0     1737 2022-09-17 22:33:43.000000 Termighty-3.0.4/source/termighty/settings/config.py
+-rw-rw-rw-   0        0        0     1010 2022-09-18 14:22:15.000000 Termighty-3.0.4/source/termighty/settings/data.py
+-rw-rw-rw-   0        0        0     1458 2023-04-13 13:51:49.000000 Termighty-3.0.4/source/termighty/settings/system.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:54:54.918757 Termighty-3.0.4/source/termighty/utils/
+-rw-rw-rw-   0        0        0       97 2022-09-18 19:41:57.000000 Termighty-3.0.4/source/termighty/utils/__init__.py
+-rw-rw-rw-   0        0        0    45164 2023-04-15 22:32:49.000000 Termighty-3.0.4/source/termighty/utils/key_processor.py
+-rw-rw-rw-   0        0        0    10100 2023-04-13 14:40:44.000000 Termighty-3.0.4/source/termighty/utils/listener.py
+-rw-rw-rw-   0        0        0     5463 2023-04-13 14:00:48.000000 Termighty-3.0.4/source/termighty/utils/term.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:54:54.925257 Termighty-3.0.4/source/termighty/widgets/
+-rw-rw-rw-   0        0        0       68 2022-09-12 19:41:55.000000 Termighty-3.0.4/source/termighty/widgets/__init__.py
+-rw-rw-rw-   0        0        0    18807 2023-04-16 13:27:48.000000 Termighty-3.0.4/source/termighty/widgets/text_box.py
+-rw-rw-rw-   0        0        0    16942 2023-04-16 12:49:28.000000 Termighty-3.0.4/source/termighty/widgets/text_editor.py
```

### Comparing `Termighty-3.0.3/LICENSE` & `Termighty-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.3/setup.py` & `Termighty-3.0.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from setuptools import setup, find_packages
-# from Cython.Build import cythonize
 
 dependencies = ["numpy"]
 
 url = "https://github.com/GabrielSCabrera/Termighty"
 
-with open("README.md", 'r') as fs:
+with open("README.md", "r") as fs:
     long_description = fs.read()
 
 setup(
     name="Termighty",
     packages=find_packages(where="source"),
     package_dir={"": "source"},
     include_package_data=True,
     package_data={"": ["data/*.json", "config.ini"]},
-    version="3.0.3",
+    version="3.0.4",
     description="Cross-Platform Terminal Coloring, Formatting, and Management Utilities.",
     long_description=long_description,
     author="Gabriel S. Cabrera",
     author_email="gabriel.sigurd.cabrera@gmail.com",
     url=url,
-    download_url=url + "archive/v3.0.3.tar.gz",
+    download_url=url + "archive/v3.0.4.tar.gz",
     keywords=["terminal", "xterm", "gui", "windows", "linux"],
     install_requires=dependencies,
-    # ext_modules=cythonize(["source/termighty/utils/key_processor.pyx"]),
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3.10",
     ],
 )
```

### Comparing `Termighty-3.0.3/source/Termighty.egg-info/SOURCES.txt` & `Termighty-3.0.4/source/Termighty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.3/source/termighty/data/keymaps.json` & `Termighty-3.0.4/source/termighty/data/keymaps.json`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.3/source/termighty/data/rgb.json` & `Termighty-3.0.4/source/termighty/data/rgb.json`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.3/source/termighty/obj/color.py` & `Termighty-3.0.4/source/termighty/obj/color.py`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.3/source/termighty/obj/string.py` & `Termighty-3.0.4/source/termighty/obj/string.py`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.3/source/termighty/settings/config.py` & `Termighty-3.0.4/source/termighty/settings/config.py`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.3/source/termighty/settings/data.py` & `Termighty-3.0.4/source/termighty/settings/data.py`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.3/source/termighty/settings/system.py` & `Termighty-3.0.4/source/termighty/settings/system.py`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.3/source/termighty/utils/key_processor.py` & `Termighty-3.0.4/source/termighty/utils/key_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -718,15 +718,15 @@
     def process_key(
         cls,
         raw_text: list[str, ...],
         cursor_position: tuple[int, int],
         selected: list[tuple[int, int], ...],
         shape: tuple[int, int],
         key: str,
-        ignore_keys: Optional[Union[str, tuple[str,...]]] = None,
+        ignore_keys: Optional[Union[str, tuple[str, ...]]] = None,
     ) -> tuple[bool, list[str, ...], tuple[int, int], list[tuple[int, int], ...]]:
         """
         Take the current text and cursor position, and modify them using the given key input.
         """
         # By default, the text will be updated.  Is set to False if a key without a binding is detected.
         call = True
```

### Comparing `Termighty-3.0.3/source/termighty/utils/listener.py` & `Termighty-3.0.4/source/termighty/utils/listener.py`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.3/source/termighty/utils/term.py` & `Termighty-3.0.4/source/termighty/utils/term.py`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.3/source/termighty/widgets/text_box.py` & `Termighty-3.0.4/source/termighty/widgets/text_box.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from termighty.settings.config import Config
 from termighty.settings.data import Data
 from termighty.settings.system import System
 from termighty.utils.term import Term
 
 import threading
 import time
+from textwrap import TextWrapper
 
 from typing import Optional, Union, Literal
 
 
 class TextBox:
 
     """
@@ -25,104 +26,127 @@
     def __init__(
         self,
         row_start: int,
         col_start: int,
         row_end: int,
         col_end: int,
         wrap_text: bool = False,
+        wrap_subsequent_indent: str = "",
+        wrap_text_break_on_hyphens: bool = True,
+        wrap_text_break_long_words: bool = True,
         background: Optional[Union[str, Color]] = None,
         foreground: Optional[Union[str, Color]] = None,
         style: Optional[str] = None,
         alignment: Literal["left", "right", "center"] = "left",
         view: tuple[int, int] = (0, 0),
     ):
         """
         Return a new instance of class `TextBox` at the specified coordinates.  If negative coordinates are given, they
         will be set dynamically relative to the size of the terminal; a thread will loop in the background keeping
         track of the terminal dimensions and resizing the TextBox if its coordinates are dynamic.
         """
         # Create a new instance of class Term, which is used to perform writing and cursor operations to the terminal.
-        self._term = Term()
+        self._term: Term = Term()
 
         # Initialize the terminal dimension attributes.
         self._init_spacial_attributes(
             row_start=row_start, col_start=col_start, row_end=row_end, col_end=col_end, view=view
         )
 
-        # Whether the text should wrap to the next line if a line exceeds the width of the underlying TextBox.
-        self._wrap_text: bool = wrap_text
         # Text alignment set to "left" by default. "right" and "center" are other alternatives.
         self._alignment: Literal["left", "right", "center"] = alignment
 
         self._set_shape()
 
-        background, foreground, style = self._prep_arguments(
+        background, foreground, style = self._init_arguments(
             background=background,
             foreground=foreground,
             style=style,
             defaults=(Config.background_color, Config.foreground_color, Config.style),
             argnames=("background", "foreground", "style"),
         )
 
         self._init_color_attributes(background=background, foreground=foreground, style=style)
 
-        self._active = False
-        self._view_changed = False
-        self._text = None
+        self._active: bool = False
+        self._view_changed: bool = False
+        self._text: list[str, ...] = None  # [""]
+
+        # Whether the text should wrap to the next line if a line exceeds the width of the underlying TextBox.
+        self._wrap_text: bool = wrap_text
+        self._wrap_text_width: int = self._shape[1]
+        self._wrap_subsequent_indent: str = wrap_subsequent_indent
+        self._wrap_text_break_on_hyphens: bool = wrap_text_break_on_hyphens
+        self._wrap_text_break_long_words: bool = wrap_text_break_long_words
+        self._process_text_wrapper()
 
     """MAGIC METHODS"""
 
     def __call__(self, text: Union[str, list[str, ...]]) -> None:
         """
         Modify the current state of the TextBox by replacing its contents with the given text. Accepts a single string,
         or a list of strings -- if a list is given, will place each element in its own row within the TextBox.
 
         Does not support the use of strings containing ANSI escape sequences!
         """
         if isinstance(text, str):
-            text = [text]
+            text: list[str, ...] = [text]
         elif not isinstance(text, list) and any(not isinstance(i, str) for i in text):
             error_message: str = (
                 f"\n\nArgument `text` in calling of {self._type} instance must be a list containing <class 'str'>."
             )
             System.kill_all = True
             raise TypeError(error_message)
 
-        self._text = text
-        self._text_prep()
+        self._text: list[str, ...] = text
+        self._process_text()
         self._set_view()
 
-    def _text_prep(self):
+    def _process_text(self):
         """
         Justify the raw text given to the __call__ method such that all lines of text are equally-sized, and wide enough
         to allow for the view of the text to be moved left, right, up, and down, until the text is just out of view.
 
         Takes the `self._alignment` attribute into account, aligning the text either to the left, right, or center of
         the TextBox.
         """
-        rows = len(self._text)
-        cols = max(len(row) for row in self._text)
+        self._process_text_wrapper()
+        if self._wrap_text:
+            self._new_line: list[bool, ...] = [
+                i == 0 for row in self._text for i in range(len(self._text_wrapper.wrap(row)))
+            ]
+            text: list[str, ...] = [line for row in self._text for line in self._text_wrapper.wrap(row)]
+        else:
+            self._new_line: list[bool] = [True for i in range(self._shape[0])]
+            text: list[str, ...] = self._text
+
+        rows: int = len(text)
+        cols: int = max(len(row) for row in text) if len(text) > 0 else 0
 
         if self._alignment == "left":
-            pad_char = "<"
+            pad_char: str = "<"
         elif self._alignment == "right":
-            pad_char = ">"
+            pad_char: str = ">"
         elif self._alignment == "center":
-            pad_char = "^"
+            pad_char: str = "^"
 
-        vertical_pad = [" " * (cols + 2 * self._shape[1])] * self._shape[0]
-        text = [f"{line:{pad_char}{self._shape[1]}s}" for line in self._text]
-        text = [line.ljust(cols + self._shape[1]) for line in text]
-        text = [line.rjust(cols + 2 * self._shape[1]) for line in text]
-        text = vertical_pad + text + vertical_pad
-
-        dimensions = (2 * self._shape[0] + rows, 2 * self._shape[1] + cols)
-
-        self._text_grid = np.zeros(dimensions, dtype="<U1")
-        self._text_grid = np.array([list(row) for row in text])
+        vertical_pad: list[str, ...] = [" " * (cols + 2 * self._shape[1])] * self._shape[0]
+        text: list[str, ...] = [f"{line:{pad_char}{self._shape[1]}s}" for line in text]
+        text: list[str, ...] = [line.ljust(cols + self._shape[1]) for line in text]
+        text: list[str, ...] = [line.rjust(cols + 2 * self._shape[1]) for line in text]
+        text: list[str, ...] = vertical_pad + text + vertical_pad
+
+        vertical_pad: list[str, ...] = [False] * self._shape[0]
+        new_line: list[str, ...] = vertical_pad + self._new_line + vertical_pad
+
+        dimensions: tuple[int, int] = (2 * self._shape[0] + rows, 2 * self._shape[1] + cols)
+
+        self._text_grid: np.ndarray = np.zeros(dimensions, dtype="<U1")
+        self._text_grid: np.ndarray = np.array([list(row) for row in text])
+        self._new_line_grid: np.npdarray = np.array(new_line)
         self._text_shape: tuple[int, int] = self._text_grid.shape
         self._text_size: int = self._text_grid.size
 
     """PRIVATE METHODS"""
 
     def _init_color_attributes(
         self,
@@ -131,17 +155,17 @@
         style: str,
     ):
         """
         Prepare all the required instance attributes, such as colors, style, and the resulting ANSI sequences that will
         be used to correctly display the text with these colors and styles.
 
         """
-        self._background = background
-        self._foreground = foreground
-        self._style = style
+        self._background: Color = background
+        self._foreground: Color = foreground
+        self._style: Color = style
 
         self._back_fmt: str = "48;2;{};{};{}".format(*self._background._rgb)
         self._fore_fmt: str = "38;2;{};{};{}".format(*self._foreground._rgb)
         self._style_fmt: str = f"{Data.styles[self._style.lower()]};"
 
         self._ANSI_format: str = f"\033[{self._style_fmt}{self._fore_fmt};{self._back_fmt}m"
 
@@ -167,18 +191,26 @@
         self._ref_col_start: int = col_start
         self._ref_row_end: int = row_end
         self._ref_col_end: int = col_end
 
         # Terminal dimensions in row major order (rows, cols).
         self._terminal_size: tuple[int, int] = System.terminal_size
 
-        self._origin = view
-        self._current_output = None
+        self._origin: tuple[int, int] = view
+        self._current_output: list[str, ...] = None
+
+    def _process_text_wrapper(self):
+        self._text_wrapper = TextWrapper(
+            width=self._wrap_text_width,
+            subsequent_indent=self._wrap_subsequent_indent,
+            break_on_hyphens=self._wrap_text_break_on_hyphens,
+            break_long_words=self._wrap_text_break_long_words,
+        )
 
-    def _prep_arguments(
+    def _init_arguments(
         self,
         background: Union[str, Color, tuple[int, int, int]],
         foreground: Union[str, Color, tuple[int, int, int]],
         style: str,
         defaults: tuple[Color, Color, str],
         argnames: tuple[str, str, str],
     ) -> tuple[Color, Color, str]:
@@ -193,29 +225,29 @@
 
         # Check that `row_end` is greater than `row_start`, and that `col_end` is greater than `col_start`.
         for i, j in zip(self._shape, (("row_end", "row_start"), ("col_end", "col_start"))):
             if i <= 0:
                 error_message: str = (
                     f"\n\nArgument `{j[0]}` must be larger than argument `{j[1]}` in the instantiation of {self._type}."
                 )
-                System.kill_all = True
+                System.kill_all: bool = True
                 raise ValueError(error_message)
 
         # Detailed exception in case an invalid color option is given. Contains string formatting curly braces so that
         # information on the specific problem is given to the user.
         color_error_message: str = (
             f"\n\nArgument `{{}}` in instantiation of {self._type} is invalid! Cannot recognize the user-provided "
             f"color: `{{}}` -- valid options are:\n"
             f"\n* The name of a known color (<class 'str'>) -- hint: print `termighty.Color.list_colors()`,"
             f"\n* A sequence containing 3 integers in range [0, 255],"
             f"\n* An instance of <class 'Color'>.\n"
         )
 
         # Will contain the final background and foreground colors, respectively.
-        args = []
+        args: list = []
         # Performs the checking and processing for both the background and foreground colors.
         for arg, default, name in zip((background, foreground), defaults[:2], argnames[:2]):
             # If the arg is None, falls back to the color name in argument `default` and uses `Color.palette`.
             if arg is None:
                 args.append(Color.palette(default))
             # If the arg is a string and a known color by name, uses `Color.palette`.
             elif isinstance(arg, str) and Color.is_color(arg.lower()):
@@ -248,26 +280,26 @@
         return *args, style
 
     def _run_thread(self, dt: float) -> None:
         """
         Keep updating the window every `dt` seconds, and account for changes in the terminal size (useful when dealing
         with relative coordinates on initialization).
         """
-        self._active = True
+        self._active: bool = True
         while self._active and not System.kill_all:
             # Reformat the contents of the TextBox due to a change in terminal dimensions.
             if self._terminal_size != (terminal_size := System.terminal_size):
-                self._terminal_size = terminal_size
+                self._terminal_size: tuple[int, int] = terminal_size
                 # Repeat the reset process three times in order to account for lag in the terminal as it is resized.
                 # Two iterations usually is enough, but three seems to always prevent issues.
                 for i in range(3):
                     time.sleep(0.01)
                     self._set_shape()
                     self._set_view()
-                    self._text_prep()
+                    self._process_text()
 
             if self._view_changed:
                 self._view_changed: bool = False
                 self.write()
             time.sleep(dt)
 
     def _set_shape(self) -> None:
@@ -289,16 +321,16 @@
         self._size: int = self._shape[0] * self._shape[1]
 
     def _set_view(self) -> None:
         """
         Backend for method `set_view` -- limits the view to prevent out of bounds errors by using commands `min` and
         `max` with the TextBox dimensions.
         """
-        row = max(min(self._origin[0] + self._shape[0], self._text_shape[0]), 0)
-        col = max(min(self._origin[1] + self._shape[1], self._text_shape[1]), 0)
+        row: int = max(min(self._origin[0] + self._shape[0], self._text_shape[0]), 0)
+        col: int = max(min(self._origin[1] + self._shape[1], self._text_shape[1]), 0)
 
         self._view: np.ndarray = self._text_grid[row : row + self._shape[0], col : col + self._shape[1]]
         self._view_changed: bool = True
 
     """PUBLIC METHODS"""
 
     @property
@@ -310,37 +342,37 @@
 
     @alignment.setter
     def alignment(self, mode: str) -> None:
         """
         Set the TextBox text alignment mode.  Set to "left" by default, but can also be set to "right" or "center".
         """
         if (mode := mode.lower()) not in ["left", "right", "center"]:
-            error_message = (
+            error_message: str = (
                 f'\n\nInvalid text alignment option selected in TextBox method `alignment`.  Valid options are "left", '
                 f'"right", or "center".'
             )
             System.kill_all = True
             raise ValueError(error_message)
 
-        self._alignment = mode
+        self._alignment: str = mode
 
     def start(self, dt: float = 0.005):
         """
         Activate a thread that runs the method self._run_thread.
         """
         if self._text is None:
             self.__call__([""])
-        self._thread = threading.Thread(target=self._run_thread, args=(dt,), daemon=False)
+        self._thread: threading.Thread = threading.Thread(target=self._run_thread, args=(dt,), daemon=False)
         self._thread.start()
 
     def stop(self) -> None:
         """
         Kill the active thread.
         """
-        self._active = False
+        self._active: bool = False
         self._thread.join()
 
     def set_view(self, row: Optional[int] = 0, col: Optional[int] = 0) -> None:
         """
         Set the current view on the text to the given coordinates. For example, given a TextBox with shape (rows=1,
         cols=10) the string
 
@@ -350,29 +382,29 @@
         representing the upper left part of the view into the text.
 
         If we were to run set_view(row=0, col=10), then the TextBox would instead display "trangers t". Or if we run
         set_view(row=1, col=15), we would get "les and so".
 
         The view may exceed the text's boundary, as it is automatically padded.
         """
-        self._origin = (row, col)
+        self._origin: tuple[int, int] = (row, col)
         self._set_view()
 
     def write(self) -> None:
         """
         Write the text to its designated coordinates with the view taken into account.
         """
         # Saving the cursor position.
         self._term.cursor_save()
         # Iterate through each row of the text.
         for m, line in enumerate(self._view):
-            row = self._row_start + m
+            row: int = self._row_start + m
             # Iterate through each column in the current row of the text.
             for n, char in enumerate(line):
-                col = self._col_start + n
-                char = f"{self._ANSI_format}{char}\033[m"
+                col: int = self._col_start + n
+                char: str = f"{self._ANSI_format}{char}\033[m"
                 # Write to the buffer, without flushing to the terminal.
                 self._term.write(row, col, char, flush=False)
         # Restoring the cursor position.
         self._term.cursor_load()
         # Flushing the results to the terminal.  Waiting to flush improves efficienty significantly.
         self._term.flush()
```

### Comparing `Termighty-3.0.3/source/termighty/widgets/text_editor.py` & `Termighty-3.0.4/source/termighty/widgets/text_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from termighty.settings.data import Data
 from termighty.utils.listener import Listener
 from termighty.utils import KeyProcessor
 from termighty.widgets.text_box import TextBox
 
 import textwrap
 import threading
+from textwrap import TextWrapper
 
 from typing import Optional, Union
 
 
 class TextEditor(TextBox):
     """
     A subclass of `TextBox` that uses class `Listener` to detect keyboard inputs, and emulate a fully-functional word
@@ -28,14 +29,15 @@
     def __init__(
         self,
         row_start: int,
         col_start: int,
         row_end: int,
         col_end: int,
         wrap_text: bool = False,
+        wrap_subsequent_indent: str = "",
         line_numbers: bool = False,
         background: Union[str, Color, tuple[int, int, int]] = None,
         foreground: Union[str, Color, tuple[int, int, int]] = None,
         style: Optional[str] = None,
         select_background: Union[str, Color, tuple[int, int, int]] = None,
         select_foreground: Union[str, Color, tuple[int, int, int]] = None,
         select_style: Optional[str] = None,
@@ -46,43 +48,46 @@
         horizontal_scroll_buffer: Optional[int] = None,
         cursor_position: tuple[int, int] = (0, 0),
         frozen: bool = False,
     ):
         """
         Creates an instance of TextEditor, and initializes its attributes and those of its inherited `TextBox`.
         """
+        self._line_numbers = line_numbers
+
         # Performing the initialization of the TextBox base class.
         super().__init__(
             row_start=row_start,
             col_start=col_start,
             row_end=row_end,
             col_end=col_end,
             wrap_text=wrap_text,
+            wrap_subsequent_indent=wrap_subsequent_indent,
             background=background,
             foreground=foreground,
             style=style,
         )
 
         # Confirming that the style, background color, and foreground color of the selected text are valid, and
         # processing them if they are not `Color` instances.
-        select_background, select_foreground, select_style = self._prep_arguments(
+        select_background, select_foreground, select_style = self._init_arguments(
             background=select_background,
             foreground=select_foreground,
             style=select_style,
             defaults=(
                 Config.selected_background_color,
                 Config.selected_foreground_color,
                 Config.selected_style,
             ),
             argnames=("select_background", "select_foreground", "select_style"),
         )
 
         # Confirming that the style, background color, and foreground color of the line numbers are valid, and
         # processing them if they are not `Color` instances.
-        line_number_background, line_number_foreground, line_number_style = self._prep_arguments(
+        line_number_background, line_number_foreground, line_number_style = self._init_arguments(
             background=line_number_background,
             foreground=line_number_foreground,
             style=line_number_style,
             defaults=(
                 Config.line_numbers_background_color,
                 Config.line_numbers_foreground_color,
                 Config.line_numbers_style,
@@ -135,16 +140,14 @@
         self._prev_cursor_position = self._cursor_position
 
         # Whether the TextEditor should be locked and all inputs ignored.
         self._frozen = frozen
 
         # Whether line numbers should be displayed on the left side of the text.
         self._line_numbers = line_numbers
-        # The default minimum width of the column containing line numbers.
-        self._line_numbers_width = Config.line_numbers_width
 
         # Saving the selected text color and style settings to instance attributes.
         self._select_background = select_background
         self._select_foreground = select_foreground
         self._select_style = select_style
 
         # ANSI escape sequences for the background color, foreground color, and text style of selected text.
@@ -167,14 +170,30 @@
         self._line_number_style_fmt: str = f"{Data.styles[self._line_number_style.lower()]};"
 
         # The full ANSI escape sequence that combines all the above three into one statement.
         self._line_number_ANSI_format: str = (
             f"\033[{self._line_number_style_fmt}{self._line_number_fore_fmt};{self._line_number_back_fmt}m"
         )
 
+    def _process_text_wrapper(self):
+        if not self._line_numbers or self._text is None:
+            w = 0
+        else:
+            w = max(Config.line_numbers_width, int(np.log10(len(self._text))) + 2)
+        self._text_wrapper = TextWrapper(
+            width=self._wrap_text_width - w,
+            expand_tabs=False,
+            replace_whitespace=False,
+            fix_sentence_endings=False,
+            break_long_words=False,
+            drop_whitespace=False,
+            break_on_hyphens=False,
+            subsequent_indent=self._wrap_subsequent_indent,
+        )
+
     def _run_getch_thread(self) -> None:
         """
         Keeps updating the window every set number of seconds (given by `dt`) and accounts for changes in the terminal
         size (useful when dealing with relative coordinates on initializiation).
         """
         self._raw_text = self._text
         getch_iterator = Listener.getch_iterator()
@@ -186,32 +205,31 @@
                     raw_text=self._raw_text,
                     cursor_position=self._cursor_position,
                     selected=self._selected,
                     shape=self._shape,
                     key=key,
                 )
                 if call:
-                    if self._wrap_text:
-                        self.__call__([i for i in self._raw_text for j in textwrap.wrap(i, self._shape[1])])
-                    else:
-                        self.__call__(self._raw_text)
+                    self.__call__(self._raw_text)
 
     def _set_scroll_buffer(self) -> None:
         """
         If the vertical and/or horizontal scroll buffers are dynamic, changes them based on the current terminal
         dimensions.
         """
         scroll_buffer = [self._scroll_buffer[0], self._scroll_buffer[1]]
 
         # How close (in rows) the cursor must get to the top or bottom of the TextBox before scrolling vertically.
         if self._dynamic_scroll_buffer[0]:
             scroll_buffer[0] = max(self._shape[0] // 10, 2)
 
         # How close (in columns) the cursor must get to the left or right TextBox edge before scrolling horizontally.
-        if self._dynamic_scroll_buffer[1]:
+        if self._wrap_text:
+            scroll_buffer[1] = 0
+        elif self._dynamic_scroll_buffer[1]:
             scroll_buffer[1] = max(self._shape[1] // 10, 4)
 
         self._scroll_buffer = (scroll_buffer[0], scroll_buffer[1])
 
     def _set_view(self) -> None:
         """ """
 
@@ -226,45 +244,57 @@
             col + self._ref_col_start - self._origin[1],
         )
 
         self._set_scroll_buffer()
 
         # Number of columns reserved for displaying line numbers -- accounts for the number of lines in the text.
         if self._line_numbers:
-            w = max(self._line_numbers_width, int(np.log10(len(self._text))) + 2)
+            w = max(Config.line_numbers_width, int(np.log10(len(self._text))) + 2)
         else:
             w = 0
 
+        # Vertically scrolls the view of the text based on the cursor position.
+        if (diff := cursor_position[0] - self._shape[0] + self._scroll_buffer[0]) >= 0:
+            self._origin = (self._origin[0] + diff, self._origin[1])
+        elif (diff := cursor_position[0] - self._scroll_buffer[0]) < 0:
+            self._origin = (max(0, self._origin[0] + diff - self._row_start), self._origin[1])
+
         if self._wrap_text:
-            pass
-        else:
 
-            # Vertically scrolls the view of the text based on the cursor position.
-            if (diff := cursor_position[0] - self._shape[0] + self._scroll_buffer[0]) >= 0:
-                self._origin = (self._origin[0] + diff, self._origin[1])
-            elif (diff := cursor_position[0] - self._scroll_buffer[0]) < 0:
-                self._origin = (max(0, self._origin[0] + diff - self._row_start), self._origin[1])
+            cursor_position = (
+                row + (col // (self._shape[1] - w)) + self._row_start - self._origin[0],
+                col % (self._shape[1] - w) + self._col_start - self._origin[1] + w,
+            )
+
+            self._selected_processed = [
+                (position[0] + self._row_start - self._origin[0], position[1] + self._col_start - self._origin[1])
+                for position in self._selected
+            ]
+            self._prev_cursor_position = self._cursor_position
+            self._term.cursor_move(*cursor_position, flush=True)
+
+        else:
 
             # Horizontally scrolls the view of the text based on the cursor position.
             if (diff := cursor_position[1] - self._shape[1] + self._scroll_buffer[1]) >= 0:
                 self._origin = (self._origin[0], self._origin[1] + diff)
             elif (diff := cursor_position[1] - self._scroll_buffer[1]) < 0:
                 self._origin = (self._origin[0], max(0, self._origin[1] + diff - self._col_start))
 
             cursor_position = (
                 row + self._row_start - self._origin[0],
                 col + self._col_start - self._origin[1] + w,
             )
 
-        self._selected_processed = [
-            (position[0] + self._row_start - self._origin[0], position[1] + self._col_start - self._origin[1])
-            for position in self._selected
-        ]
-        self._prev_cursor_position = self._cursor_position
-        self._term.cursor_move(*cursor_position, flush=True)
+            self._selected_processed = [
+                (position[0] + self._row_start - self._origin[0], position[1] + self._col_start - self._origin[1])
+                for position in self._selected
+            ]
+            self._prev_cursor_position = self._cursor_position
+            self._term.cursor_move(*cursor_position, flush=True)
 
         super()._set_view()
 
     def start(self):
         """
         Main loop which runs on one thread, while a listener runs on another and provides commands to be read by
         this method.
@@ -292,15 +322,15 @@
 
     def write(self) -> None:
         """
         Write the text to its designated coordinates with the view taken into account.
         """
         if self._line_numbers:
             # Number of columns reserved for displaying line numbers -- accounts for the number of lines in the text.
-            w = max(self._line_numbers_width, int(np.log10(len(self._text))) + 2)
+            w = max(Config.line_numbers_width, int(np.log10(len(self._text))) + 2)
             # Checking the shape the terminal had when this method was last called.
             expected_shape = (self._view.shape[0], self._view.shape[1] + w)
         else:
             w = 0
             expected_shape = self._view.shape
 
         # Clearing the current_output attribute if the terminal had a different shape when last writing to the terminal.
```

