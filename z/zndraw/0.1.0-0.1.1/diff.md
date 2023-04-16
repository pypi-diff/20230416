# Comparing `tmp/zndraw-0.1.0.tar.gz` & `tmp/zndraw-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zndraw-0.1.0.tar", max compression
+gzip compressed data, was "zndraw-0.1.1.tar", max compression
```

## Comparing `zndraw-0.1.0.tar` & `zndraw-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    13576 2023-04-12 16:10:14.508402 zndraw-0.1.0/LICENSE
--rw-r--r--   0        0        0      757 2023-04-15 19:00:54.346499 zndraw-0.1.0/README.md
--rw-r--r--   0        0        0      499 2023-04-15 19:00:54.356499 zndraw-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       46 2023-04-15 19:00:54.356499 zndraw-0.1.0/zndraw/__init__.py
--rw-r--r--   0        0        0     2328 2023-04-15 19:00:54.356499 zndraw-0.1.0/zndraw/app.py
--rw-r--r--   0        0        0     2616 2023-04-15 19:00:54.356499 zndraw-0.1.0/zndraw/cli.py
--rw-r--r--   0        0        0     1204 2023-04-15 19:00:54.356499 zndraw-0.1.0/zndraw/globals.py
--rw-r--r--   0        0        0     1006 2023-04-15 19:00:54.356499 zndraw-0.1.0/zndraw/io.py
--rw-r--r--   0        0        0     9189 2023-04-15 19:00:54.356499 zndraw-0.1.0/zndraw/static/main.js
--rw-r--r--   0        0        0      798 2023-04-15 19:00:54.366499 zndraw-0.1.0/zndraw/templates/index.html
--rw-r--r--   0        0        0     1329 1970-01-01 00:00:00.000000 zndraw-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    13576 2023-04-12 16:10:14.508402 zndraw-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1054 2023-04-16 15:12:56.780430 zndraw-0.1.1/README.md
+-rw-r--r--   0        0        0      646 2023-04-15 20:56:07.240790 zndraw-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      125 2023-04-15 20:56:00.080869 zndraw-0.1.1/zndraw/__init__.py
+-rw-r--r--   0        0        0     2403 2023-04-16 13:08:44.451924 zndraw-0.1.1/zndraw/app.py
+-rw-r--r--   0        0        0     2184 2023-04-16 13:36:29.983571 zndraw-0.1.1/zndraw/cli.py
+-rw-r--r--   0        0        0     1222 2023-04-16 12:56:04.890308 zndraw-0.1.1/zndraw/globals.py
+-rw-r--r--   0        0        0     1074 2023-04-15 22:53:05.753961 zndraw-0.1.1/zndraw/io.py
+-rw-r--r--   0        0        0     4398 2023-04-16 11:38:33.242164 zndraw-0.1.1/zndraw/static/main.css
+-rw-r--r--   0        0        0    14752 2023-04-16 14:54:27.672532 zndraw-0.1.1/zndraw/static/main.js
+-rw-r--r--   0        0        0     9431 2023-04-16 14:55:41.771724 zndraw-0.1.1/zndraw/templates/index.html
+-rw-r--r--   0        0        0     1691 1970-01-01 00:00:00.000000 zndraw-0.1.1/PKG-INFO
```

### Comparing `zndraw-0.1.0/LICENSE` & `zndraw-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.0/README.md` & `zndraw-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 [![zincware](https://img.shields.io/badge/Powered%20by-zincware-darkcyan)](https://github.com/zincware)
+[![PyPI version](https://badge.fury.io/py/zndraw.svg)](https://badge.fury.io/py/zndraw)
+!['Threejs](https://img.shields.io/badge/threejs-black?style=for-the-badge&logo=three.js&logoColor=white)
+
 
 # ZnDraw
 
 Install via ``pip install zndraw``.
 
 ## CLI
 
@@ -10,14 +13,17 @@
 For a full list of arguments use `zndraw --help`.
 
 To interface with ``zndraw --update-function module.function`` you need to be able to import via ``from module import function``.
 
 The ZnDraw function expects as inputs
 - atom_ids: list[int], the ids of the currently selected atoms
 - atoms: ase.Atoms, the configuration as `ase.Atoms` file where atom_ids where selected.
+
 and as an output:
 - list[ase.Atoms], a list of ase Atoms objects to display.
 
 ```python
 def function(atom_ids: list[int], atoms: ase.Atoms) -> list[ase.Atoms]:
     ...
-```
+```
+
+![Alt text](https://raw.githubusercontent.com/zincware/ZnDraw/main/misc/zndraw_ui.png "ZnDraw UI")
```

### Comparing `zndraw-0.1.0/zndraw/app.py` & `zndraw-0.1.1/zndraw/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-from flask import Flask
-from flask import render_template
-from flask import session, request
+import dataclasses
 import uuid
+
+from flask import Flask, render_template, request, session
+
 from zndraw import globals, io
-import dataclasses
 
 app = Flask(__name__)
 app.secret_key = str(uuid.uuid4())
 
 
 @app.route("/")
 def index():
     session["key"] = str(uuid.uuid4())  # TODO use session key e.g. for atoms cache
-    return render_template("index.html")
+    return render_template("index.html", config=dataclasses.asdict(globals.config))
 
 
 @app.route("/config")
 def config():
-    return dataclasses.asdict(globals.config)
+    return dataclasses.asdict(globals.config) | {
+        "total_frames": len(globals._atoms_cache) - 1
+    }
 
 
 @app.route("/atoms")
 def atoms():
     atoms = globals.config.get_atoms(step=0)
     graph = io.get_graph(atoms)
     return [graph.nodes[idx] | {"id": idx} for idx in graph.nodes]
@@ -35,23 +37,23 @@
         return [graph.nodes[idx] | {"id": idx} for idx in graph.nodes]
     except (KeyError, IndexError):
         return []
 
 
 @app.route("/atoms/<start>&<stop>")
 def atoms_steps(start, stop):
+    result = []
     try:
-        result = []
         for step in range(int(start), int(stop)):
             atoms = globals.config.get_atoms(step=int(step))
             graph = io.get_graph(atoms)
             result.append([graph.nodes[idx] | {"id": idx} for idx in graph.nodes])
         return result
     except (KeyError, IndexError):
-        return []
+        return result
 
 
 @app.route("/atoms/<step>/<atom_id>")
 def atom_step(step, atom_id):
     return {}
```

### Comparing `zndraw-0.1.0/zndraw/cli.py` & `zndraw-0.1.1/zndraw/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,79 +1,63 @@
+import pathlib
+import sys
+import webbrowser
+
 import typer
-from zndraw import app, globals
+
+from zndraw import __version__, app, globals
 
 cli = typer.Typer()
 
 
-# @app.command()
-# def main(
-#     file: str,
-#     select_canvas: bool = typer.Option(True),
-#     select_atoms: bool = typer.Option(False),
-#     bonds: bool = typer.Option(False),
-# ) -> None:
-#     """ZnDraw: Visualize Molecules
-
-#     With 'zndraw molecule.xyz' you can visualize the molecule in your browser.
-
-#     Attributes
-#     ----------
-#     file : str
-#         Path to the xyz file.
-#     select_canvas : bool
-#         Add a canvas that helps to select points in space.
-#     select_atoms : bool
-#         Allow selection of atoms.
-#     """
-#     graph = io.read_file(file)
-
-#     app = viewer.DashApp(
-#         graph=graph, select_canvas=select_canvas, select_atoms=select_atoms
-#     )
-#     app.update_layout()
-#     app.add_canvas_slider()
-#     app.plot_atoms()
-#     if bonds:
-#         app.plot_bonds()
-#     app.run_dash_server_click()
+def version_callback():
+    typer.echo(f"ZnDraw {__version__}")
+    raise typer.Exit()
 
 
 @cli.command()
 def main(
     file: str = typer.Argument(..., help="Trajectory File"),
     port: int = typer.Option(5123, help="Port to run the server on"),
     animate: bool = typer.Option(False, help="Animate the trajectory"),
     sphere_size: float = typer.Option(1.0, help="size of the hydrogen sphere"),
     bond_size: float = typer.Option(1.0, help="size of a bond"),
-    max_fps: int = typer.Option(1000, help="Maximum frames per second"),
+    max_fps: int = typer.Option(100, help="Maximum frames per second"),
     update_function: str = typer.Option(
         None, help="Path to a python file with an update function 'module.function'."
     ),
     repeat: int = typer.Option(1, help="Repeat the trajectory n times"),
     frame_buffer: int = typer.Option(
         100,
         help="Buffer size. Must be smaller than the total number of frames.",
     ),
     resolution: int = typer.Option(5, help="Proportional to the number of polygons."),
     restart_animation: bool = typer.Option(
         False, help="run the animation in an endless loop."
     ),
     frames_per_post: int = typer.Option(10, help="Number of frames to send per POST."),
+    browser: bool = typer.Option(True, help="Open the browser automatically."),
 ):
-    """
-    ZnDraw: Visualize Molecules
+    """ZnDraw: Visualize Molecules
 
-    CLI for the ZnDraw visualizer.
+    The ZnDraw CLI. Use 'zndraw version' to get the current version.
     """
+    sys.path.insert(1, pathlib.Path.cwd().as_posix())
+
+    if file == "version":
+        version_callback()
+
     globals.config.file = file
     globals.config.animate = animate
     globals.config.sphere_size = sphere_size
     globals.config.bond_size = bond_size
     globals.config.max_fps = max_fps
     globals.config.update_function = update_function
     globals.config.frame_buffer = frame_buffer
     globals.config.resolution = resolution
     globals.config.frames_per_post = frames_per_post
     globals.config.restart_animation = restart_animation
     globals.config.repeat = (repeat, repeat, repeat)
 
+    if browser:
+        webbrowser.open(f"http://localhost:{port}")
     app.run(port=port)
```

### Comparing `zndraw-0.1.0/zndraw/globals.py` & `zndraw-0.1.1/zndraw/globals.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import dataclasses
 import importlib
+
 import ase.io
 
 
 @dataclasses.dataclass
 class Config:
     file: str = None
     animate: bool = None
@@ -24,20 +25,21 @@
         module = importlib.import_module(module_name)
         return getattr(module, function_name)
 
     def get_atoms(self, step=0) -> ase.Atoms:
         try:
             return _atoms_cache[step]
         except KeyError:
-            if not self.animate and step != 0:
+            if self.update_function is not None and step != 0:
                 raise
             for idx, atoms in enumerate(ase.io.iread(self.file)):
                 _atoms_cache[idx] = atoms.copy().repeat(self.repeat)
                 if step == 0:
                     break
+
         return _atoms_cache[step]
 
 
 # TODO set defaults here and load in typer?
 
 _atoms_cache: dict = {}
 config = Config()
```

### Comparing `zndraw-0.1.0/PKG-INFO` & `zndraw-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: zndraw
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: Apache-2.0
 Author: zincwarecode
 Author-email: zincwarecode@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ase (>=3.22.1,<4.0.0)
 Requires-Dist: flask (>=2.2.3,<3.0.0)
 Requires-Dist: networkx (>=3.1,<4.0)
-Requires-Dist: typer (>=0.7.0,<0.8.0)
+Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Project-URL: repository, https://github.com/zincware/ZnDraw
 Description-Content-Type: text/markdown
 
 [![zincware](https://img.shields.io/badge/Powered%20by-zincware-darkcyan)](https://github.com/zincware)
+[![PyPI version](https://badge.fury.io/py/zndraw.svg)](https://badge.fury.io/py/zndraw)
+!['Threejs](https://img.shields.io/badge/threejs-black?style=for-the-badge&logo=three.js&logoColor=white)
+
 
 # ZnDraw
 
 Install via ``pip install zndraw``.
 
 ## CLI
 
@@ -28,14 +32,18 @@
 For a full list of arguments use `zndraw --help`.
 
 To interface with ``zndraw --update-function module.function`` you need to be able to import via ``from module import function``.
 
 The ZnDraw function expects as inputs
 - atom_ids: list[int], the ids of the currently selected atoms
 - atoms: ase.Atoms, the configuration as `ase.Atoms` file where atom_ids where selected.
+
 and as an output:
 - list[ase.Atoms], a list of ase Atoms objects to display.
 
 ```python
 def function(atom_ids: list[int], atoms: ase.Atoms) -> list[ase.Atoms]:
     ...
 ```
+
+![Alt text](https://raw.githubusercontent.com/zincware/ZnDraw/main/misc/zndraw_ui.png "ZnDraw UI")
+
```

