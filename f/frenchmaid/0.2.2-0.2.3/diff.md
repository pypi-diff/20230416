# Comparing `tmp/frenchmaid-0.2.2.tar.gz` & `tmp/frenchmaid-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frenchmaid-0.2.2.tar", last modified: Sun Aug 21 21:01:46 2022, max compression
+gzip compressed data, was "frenchmaid-0.2.3.tar", last modified: Sun Apr 16 14:51:24 2023, max compression
```

## Comparing `frenchmaid-0.2.2.tar` & `frenchmaid-0.2.3.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2022-08-21 21:01:46.317179 frenchmaid-0.2.2/
--rw-rw-rw-   0        0        0      593 2022-04-24 12:32:05.000000 frenchmaid-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     8052 2022-08-21 21:01:46.316177 frenchmaid-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     7038 2022-08-21 21:00:58.000000 frenchmaid-0.2.2/README.md
--rw-rw-rw-   0        0        0       86 2022-04-19 21:04:21.000000 frenchmaid-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-08-21 21:01:46.317179 frenchmaid-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1548 2022-08-21 20:59:04.000000 frenchmaid-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-21 21:01:46.268177 frenchmaid-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2022-08-21 21:01:46.281178 frenchmaid-0.2.2/src/frenchmaid/
--rw-rw-rw-   0        0        0      225 2022-08-21 20:58:57.000000 frenchmaid-0.2.2/src/frenchmaid/__init__.py
--rw-rw-rw-   0        0        0      136 2022-08-10 05:23:52.000000 frenchmaid-0.2.2/src/frenchmaid/__main__.py
--rw-rw-rw-   0        0        0     1218 2022-08-12 18:10:09.000000 frenchmaid-0.2.2/src/frenchmaid/cli.py
-drwxrwxrwx   0        0        0        0 2022-08-21 21:01:46.309177 frenchmaid-0.2.2/src/frenchmaid/modules/
--rw-rw-rw-   0        0        0        0 2022-08-10 05:53:15.000000 frenchmaid-0.2.2/src/frenchmaid/modules/__init__.py
--rw-rw-rw-   0        0        0     4396 2022-08-11 04:07:55.000000 frenchmaid-0.2.2/src/frenchmaid/modules/clean.py
--rw-rw-rw-   0        0        0     2987 2022-08-21 20:54:59.000000 frenchmaid-0.2.2/src/frenchmaid/modules/ignore.py
-drwxrwxrwx   0        0        0        0 2022-08-21 21:01:46.314179 frenchmaid-0.2.2/src/frenchmaid/switches/
--rw-rw-rw-   0        0        0        0 2022-08-12 14:58:07.000000 frenchmaid-0.2.2/src/frenchmaid/switches/__init__.py
--rw-rw-rw-   0        0        0      631 2022-08-11 05:13:32.000000 frenchmaid-0.2.2/src/frenchmaid/switches/cleanSwitch.py
--rw-rw-rw-   0        0        0      777 2022-08-11 05:13:51.000000 frenchmaid-0.2.2/src/frenchmaid/switches/ignoreSwitch.py
-drwxrwxrwx   0        0        0        0 2022-08-21 21:01:46.304179 frenchmaid-0.2.2/src/frenchmaid.egg-info/
--rw-rw-rw-   0        0        0     8052 2022-08-21 21:01:46.000000 frenchmaid-0.2.2/src/frenchmaid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      562 2022-08-21 21:01:46.000000 frenchmaid-0.2.2/src/frenchmaid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-21 21:01:46.000000 frenchmaid-0.2.2/src/frenchmaid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2022-08-21 21:01:46.000000 frenchmaid-0.2.2/src/frenchmaid.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2022-08-21 21:01:46.000000 frenchmaid-0.2.2/src/frenchmaid.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-08-21 21:01:46.000000 frenchmaid-0.2.2/src/frenchmaid.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 14:51:24.398642 frenchmaid-0.2.3/
+-rw-rw-rw-   0        0        0      593 2023-04-16 14:39:33.000000 frenchmaid-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     8601 2023-04-16 14:51:24.397668 frenchmaid-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7611 2023-04-16 14:48:32.000000 frenchmaid-0.2.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-16 14:39:33.000000 frenchmaid-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 14:51:24.399640 frenchmaid-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1524 2023-04-16 14:46:59.000000 frenchmaid-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:51:24.345643 frenchmaid-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 14:51:24.361640 frenchmaid-0.2.3/src/frenchmaid/
+-rw-rw-rw-   0        0        0      225 2023-04-16 14:47:20.000000 frenchmaid-0.2.3/src/frenchmaid/__init__.py
+-rw-rw-rw-   0        0        0      138 2023-04-16 14:39:33.000000 frenchmaid-0.2.3/src/frenchmaid/__main__.py
+-rw-rw-rw-   0        0        0     1227 2023-04-16 14:39:33.000000 frenchmaid-0.2.3/src/frenchmaid/cli.py
+-rw-rw-rw-   0        0        0     2564 2023-04-16 14:39:33.000000 frenchmaid-0.2.3/src/frenchmaid/delcache.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:51:24.391643 frenchmaid-0.2.3/src/frenchmaid/modules/
+-rw-rw-rw-   0        0        0        0 2023-04-16 14:39:33.000000 frenchmaid-0.2.3/src/frenchmaid/modules/__init__.py
+-rw-rw-rw-   0        0        0     4421 2023-04-16 14:39:33.000000 frenchmaid-0.2.3/src/frenchmaid/modules/clean.py
+-rw-rw-rw-   0        0        0     3012 2023-04-16 14:39:33.000000 frenchmaid-0.2.3/src/frenchmaid/modules/ignore.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:51:24.395640 frenchmaid-0.2.3/src/frenchmaid/switches/
+-rw-rw-rw-   0        0        0        0 2023-04-16 14:39:33.000000 frenchmaid-0.2.3/src/frenchmaid/switches/__init__.py
+-rw-rw-rw-   0        0        0      631 2023-04-16 14:39:33.000000 frenchmaid-0.2.3/src/frenchmaid/switches/cleanSwitch.py
+-rw-rw-rw-   0        0        0      777 2023-04-16 14:39:33.000000 frenchmaid-0.2.3/src/frenchmaid/switches/ignoreSwitch.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:51:24.387672 frenchmaid-0.2.3/src/frenchmaid.egg-info/
+-rw-rw-rw-   0        0        0     8601 2023-04-16 14:51:24.000000 frenchmaid-0.2.3/src/frenchmaid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      589 2023-04-16 14:51:24.000000 frenchmaid-0.2.3/src/frenchmaid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 14:51:24.000000 frenchmaid-0.2.3/src/frenchmaid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-16 14:51:24.000000 frenchmaid-0.2.3/src/frenchmaid.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-04-16 14:51:24.000000 frenchmaid-0.2.3/src/frenchmaid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-16 14:51:24.000000 frenchmaid-0.2.3/src/frenchmaid.egg-info/top_level.txt
```

### Comparing `frenchmaid-0.2.2/LICENSE` & `frenchmaid-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `frenchmaid-0.2.2/PKG-INFO` & `frenchmaid-0.2.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: frenchmaid
-Version: 0.2.2
+Version: 0.2.3
 Summary: Remove all pests from your project! frenchmaid is a lightweight all platform cli package that will delete all pycache and other folders (contents included) in your project directory. Are you tired of doing it manually each time? Fear not, the frenchmaid will do it for you!
 Home-page: https://github.com/lewisjr/frenchmaid.git
-Author: Techtronics Solutions Limited | Lewis Mosho Jr
-Author-email: lmosho@techtronicsltd.com
+Author: Cerebrus Inc | Lewis Mosho Jr
+Author-email: lewis@cerebrus.dev
 Project-URL: Bug Tracker, https://github.com/lewisjr/frenchmaid/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -18,15 +18,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
     <img src="https://static.wixstatic.com/media/916fb4_88bd4d4d46e14f0c90f64213970c3a2d~mv2.png/v1/fill/w_750,h_750,al_c,q_90,usm_0.66_1.00_0.01,enc_auto/916fb4_88bd4d4d46e14f0c90f64213970c3a2d~mv2.png" alt="frenchmaid logo" width="250" height="250" />
 </p>
 
-# frenchmaid v0.2.2
+# frenchmaid v0.2.3
 
 Are you a python developer who also/only uses windows and are sick and tired of constantly deteting those pesky `__pycache__` directories? Fear not, **frenchmaid** is here to help! frenchmaid is a CLI app written in pure python that will search your entire project directory and delete any `__pycache__` or other folders (and the files within) in your root directory. Now it can also add these folders to your ignore files!
 
 **Supported Folders**
 
 - \_\_pycache\_\_
 - .mypy_cache
@@ -106,21 +106,21 @@
 
 <br />
 It's really that simple, just ensure that you are in your project's root directory! For clarity, the above example assumes that your project structure is something like this for example:
 <br />
 <br />
 
     example-app
-    ├── main.py
+    ├── LICENSE
     ├── requirements.txt
     └── src
          └── __init__.py
          └── app.py
 
-If the root is `example-app` then you can see that the terminal should be in that folder.
+If the root is `example-app` then you can see that the terminal should be in that dir.
 
 ## Commands
 
 ### clean
 
 Run `frenchmaid clean` in your project's root directory without any arguments to remove all instances of supported folders. If you want to delete all instances of one type of folder and not any others, run the command with an option; For example, `frenchmaid clean mypy`.
 
@@ -159,15 +159,15 @@
 
 or
 
     frenchmaid --version
 
 will return (for example):
 
-    frenchmaid v0.2.2
+    frenchmaid v0.2.3
 
 ### Help
 
 In any terminal in any directory:
 
     frenchmaid --help
 
@@ -189,52 +189,74 @@
 
 Note that this option can also be used in tandem with any command.
 
 ## Support and Reporting
 
 You can report any bugs or improvements [here](https://github.com/lewisjr/home-app/issues), I will try to address them as soon as possible. Feel free to suggest any other files or folders you think it should delete (e.g .pytest_cache) with all context on how they appear. I will happily make it a possibility without breaking the current format! To the best of my abilities of course, and the github page will be updated on any changes.
 
-# Version History
+# Changelog
 
-## v0.2.2
+## v0.2.x
 
-**Minor Patch 2**
+<details open>
+<summary><strong>v0.2.3</strong></summary>
 
-- Updated README version history to include v0.2.1 updates
+- Codebase improvements
+- Full parity between `windows` and `linux` systems; **Full Stability**
+- Added .gitignore
+- README structure changed
+- Note added to v0.2.0 to denote it's instability
+</details>
 
-## v0.2.1
+<details>
+<summary><strong>v0.2.2</strong></summary>
 
-**Minor Patch 1**
+- Updated README version history to include v0.2.1 updates
+</details>
 
-- Fixed ignore format for \_\_pycache\_\_ in git
+<details>
+<summary><strong>v0.2.1</strong></summary>
 
-## v0.2.0
+- Fixed ignore format for **pycache** in git
+</details>
 
-**Major Patch**
+<details>
+<summary><strong>v0.2.0</strong></summary>
 
 - Added a logo to the README
 - Added instructions for a Linux PATH error
 - Added ignore command and arguments
 - Added support for mypy cache folders
 - Added arguments to the clean command
 - Added `--help` context to all commands
 - Moved all functions to a modules folder
 - Added a class switch
 - Typed modules
+- Unstable on linux bases systems
+
+</details>
+<br />
 
-## v0.1.2
+## v0.1.x
 
-**Minor patch 2**
+<details>
+<summary><strong>v0.1.2</strong></summary>
 
 - License has been updated to Apache from MIT effective from the date of this release
 - Notes on potential path problems that can arise from installation on Windows have been added to the README
 
-## v0.1.1
+</details>
 
-**Minor patch**
+<details>
+<summary><strong>v0.1.1</strong></summary>
 
 - Issue on linux machines fixed with directory name post pycache delete
   - The package no longer displays the root directory's full absolute path (e.g Documents/example-app), but rather just the root directory's name (e.g example-app) on linux machines.
 
-## v0.1.0
+</details>
+
+<details>
+<summary><strong>v0.1.0</strong></summary>
+
+- Initial Release; Stable version for use on all platforms
 
-Initial Release; Stable version for use on all platforms.
+</details>
```

### Comparing `frenchmaid-0.2.2/README.md` & `frenchmaid-0.2.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <p align="center">
     <img src="https://static.wixstatic.com/media/916fb4_88bd4d4d46e14f0c90f64213970c3a2d~mv2.png/v1/fill/w_750,h_750,al_c,q_90,usm_0.66_1.00_0.01,enc_auto/916fb4_88bd4d4d46e14f0c90f64213970c3a2d~mv2.png" alt="frenchmaid logo" width="250" height="250" />
 </p>
 
-# frenchmaid v0.2.2
+# frenchmaid v0.2.3
 
 Are you a python developer who also/only uses windows and are sick and tired of constantly deteting those pesky `__pycache__` directories? Fear not, **frenchmaid** is here to help! frenchmaid is a CLI app written in pure python that will search your entire project directory and delete any `__pycache__` or other folders (and the files within) in your root directory. Now it can also add these folders to your ignore files!
 
 **Supported Folders**
 
 - \_\_pycache\_\_
 - .mypy_cache
@@ -86,21 +86,21 @@
 
 <br />
 It's really that simple, just ensure that you are in your project's root directory! For clarity, the above example assumes that your project structure is something like this for example:
 <br />
 <br />
 
     example-app
-    ├── main.py
+    ├── LICENSE
     ├── requirements.txt
     └── src
          └── __init__.py
          └── app.py
 
-If the root is `example-app` then you can see that the terminal should be in that folder.
+If the root is `example-app` then you can see that the terminal should be in that dir.
 
 ## Commands
 
 ### clean
 
 Run `frenchmaid clean` in your project's root directory without any arguments to remove all instances of supported folders. If you want to delete all instances of one type of folder and not any others, run the command with an option; For example, `frenchmaid clean mypy`.
 
@@ -139,15 +139,15 @@
 
 or
 
     frenchmaid --version
 
 will return (for example):
 
-    frenchmaid v0.2.2
+    frenchmaid v0.2.3
 
 ### Help
 
 In any terminal in any directory:
 
     frenchmaid --help
 
@@ -169,52 +169,74 @@
 
 Note that this option can also be used in tandem with any command.
 
 ## Support and Reporting
 
 You can report any bugs or improvements [here](https://github.com/lewisjr/home-app/issues), I will try to address them as soon as possible. Feel free to suggest any other files or folders you think it should delete (e.g .pytest_cache) with all context on how they appear. I will happily make it a possibility without breaking the current format! To the best of my abilities of course, and the github page will be updated on any changes.
 
-# Version History
+# Changelog
 
-## v0.2.2
+## v0.2.x
 
-**Minor Patch 2**
+<details open>
+<summary><strong>v0.2.3</strong></summary>
 
-- Updated README version history to include v0.2.1 updates
+- Codebase improvements
+- Full parity between `windows` and `linux` systems; **Full Stability**
+- Added .gitignore
+- README structure changed
+- Note added to v0.2.0 to denote it's instability
+</details>
 
-## v0.2.1
+<details>
+<summary><strong>v0.2.2</strong></summary>
 
-**Minor Patch 1**
+- Updated README version history to include v0.2.1 updates
+</details>
 
-- Fixed ignore format for \_\_pycache\_\_ in git
+<details>
+<summary><strong>v0.2.1</strong></summary>
 
-## v0.2.0
+- Fixed ignore format for **pycache** in git
+</details>
 
-**Major Patch**
+<details>
+<summary><strong>v0.2.0</strong></summary>
 
 - Added a logo to the README
 - Added instructions for a Linux PATH error
 - Added ignore command and arguments
 - Added support for mypy cache folders
 - Added arguments to the clean command
 - Added `--help` context to all commands
 - Moved all functions to a modules folder
 - Added a class switch
 - Typed modules
+- Unstable on linux bases systems
+
+</details>
+<br />
 
-## v0.1.2
+## v0.1.x
 
-**Minor patch 2**
+<details>
+<summary><strong>v0.1.2</strong></summary>
 
 - License has been updated to Apache from MIT effective from the date of this release
 - Notes on potential path problems that can arise from installation on Windows have been added to the README
 
-## v0.1.1
+</details>
 
-**Minor patch**
+<details>
+<summary><strong>v0.1.1</strong></summary>
 
 - Issue on linux machines fixed with directory name post pycache delete
   - The package no longer displays the root directory's full absolute path (e.g Documents/example-app), but rather just the root directory's name (e.g example-app) on linux machines.
 
-## v0.1.0
+</details>
+
+<details>
+<summary><strong>v0.1.0</strong></summary>
+
+- Initial Release; Stable version for use on all platforms
 
-Initial Release; Stable version for use on all platforms.
+</details>
```

### Comparing `frenchmaid-0.2.2/setup.py` & `frenchmaid-0.2.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="frenchmaid",
-    version="0.2.2",
+    version="0.2.3",
     description="Remove all pests from your project! frenchmaid is a lightweight all platform cli package that will delete all pycache and other folders (contents included) in your project directory. Are you tired of doing it manually each time? Fear not, the frenchmaid will do it for you!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lewisjr/frenchmaid.git",
     project_urls={
         "Bug Tracker": "https://github.com/lewisjr/frenchmaid/issues",
     },
-    author = "Techtronics Solutions Limited | Lewis Mosho Jr",
-    author_email = "lmosho@techtronicsltd.com",
+    author = "Cerebrus Inc | Lewis Mosho Jr",
+    author_email = "lewis@cerebrus.dev",
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "Topic :: Utilities",
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
```

### Comparing `frenchmaid-0.2.2/src/frenchmaid/cli.py` & `frenchmaid-0.2.3/src/frenchmaid/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import typer
 
 from typing import Optional
-from frenchmaid import __app_name__, __version__
+from . import __app_name__, __version__
 
 from .switches import cleanSwitch as clS, ignoreSwitch as igS
 
 app = typer.Typer(help="A handy tool to delete all junk!", no_args_is_help=True)
 
 ignoreSwitch = igS.IgnoreSwitch()
 cleanSwitch = clS.CleanSwitch()
@@ -26,17 +26,17 @@
         callback=_version_callback,
         is_eager=True
     )
 ) -> None: return
 
 @app.command(help="Delete all instances of junk folders")
 def clean(folder: Optional[str] = typer.Argument(None, help="pycache, mypy")) -> None:
-    if (folder):
+    if folder:
         cleanSwitch.indirect(folder)
     else:
         cleanSwitch.indirect("all")
     raise typer.Exit()
 
 @app.command(help="Add junk folders to ignore files", no_args_is_help=True)
 def ignore(platform: Optional[str] = typer.Argument(..., help="git, docker")) -> None:
-    ignoreSwitch.indirect(platform)
+    ignoreSwitch.indirect(platform if platform else "")
     raise typer.Exit()
```

### Comparing `frenchmaid-0.2.2/src/frenchmaid/modules/clean.py` & `frenchmaid-0.2.3/src/frenchmaid/modules/clean.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import os, shutil, sys
+from typing import List
 
 platf: str = sys.platform
 
 def delDir(dir_select: str) -> bool:
     try:
         shutil.rmtree(dir_select)
         return True
     except:
         return False
 
-def loopDirsOne(main_dir: str, dir_arr: list[str], num_pycache: int, dir_arr_used: list[str], dir_to_delete: str) -> list[str]:
+def loopDirsOne(main_dir: str, dir_arr: List[str], num_pycache: int, dir_arr_used: List[str], dir_to_delete: str) -> List[str]:
     iterats: int = num_pycache
-    arr: list[str] = dir_arr_used
-    arr2: list[str] = dir_arr_used
+    arr: List[str] = dir_arr_used
+    arr2: List[str] = dir_arr_used
 
     if "pyvenv.cfg" not in dir_arr:
         for dir in dir_arr:
             if (dir in dir_arr_used) == False:
                 if str(dir) == dir_to_delete:
 
                     if platf == "win32":
@@ -31,15 +32,15 @@
 
                     if platf == "win32":
                         other_dir = f"{main_dir}\\{dir}"
                     else:
                         other_dir = f"{main_dir}/{dir}"
 
                     try:
-                        other_dirs: list[str] = os.listdir(other_dir)
+                        other_dirs: List[str] = os.listdir(other_dir)
 
                         if platf == "win32":
                             iterats_two = loopDirsOne(other_dir, other_dirs, iterats, arr, dir_to_delete)
                         else:
                             iterats_two = loopDirsOne(other_dir, other_dirs, iterats, arr2, dir_to_delete)
 
                         iterats = iterats + len(iterats_two)
@@ -48,18 +49,18 @@
 
 
     if platf == "win32":
         return arr
     else:
         return arr2
 
-def loopDirsAll(main_dir: str, dir_arr: list[str], num_pycache: int, dir_arr_used: list[str]) -> list[str]:
+def loopDirsAll(main_dir: str, dir_arr: List[str], num_pycache: int, dir_arr_used: List[str]) -> List[str]:
     iterats: int = num_pycache
-    arr: list[str] = dir_arr_used
-    arr2: list[str] = dir_arr_used
+    arr: List[str] = dir_arr_used
+    arr2: List[str] = dir_arr_used
 
     if "pyvenv.cfg" not in dir_arr:
         for dir in dir_arr:
             if (dir in dir_arr_used) == False:
                 if str(dir) == "__pycache__" or str(dir) == '.mypy_cache':
 
                     if platf == "win32":
@@ -74,15 +75,15 @@
 
                     if platf == "win32":
                         other_dir = f"{main_dir}\\{dir}"
                     else:
                         other_dir = f"{main_dir}/{dir}"
 
                     try:
-                        other_dirs: list[str] = os.listdir(other_dir)
+                        other_dirs: List[str] = os.listdir(other_dir)
 
                         if platf == "win32":
                             iterats_two = loopDirsAll(other_dir, other_dirs, iterats, arr)
                         else:
                             iterats_two = loopDirsAll(other_dir, other_dirs, iterats, arr2)
 
                         iterats = iterats + len(iterats_two)
@@ -99,18 +100,18 @@
         dir_name: str = ''
         
         if platf == "win32":
             dir_name = dir_main[str(dir_main).rfind("\\")+1:len(dir_main)]
         else:
             dir_name = dir_main[str(dir_main).rfind("/")+1:len(dir_main)]
             
-        dirs: list[str] = os.listdir(dir_main)
+        dirs: List[str] = os.listdir(dir_main)
         num_dirs: int = len(dirs)
-        arr: list[str] = []
-        array_thing: list[str] = []
+        arr: List[str] = []
+        array_thing: List[str] = []
 
         if folder == 'all':
             array_thing = loopDirsAll(dir_main, dirs, 0, arr)
         else:
            array_thing = loopDirsOne(dir_main, dirs, 0, arr, folder)
 
         res: int = len(array_thing)
```

### Comparing `frenchmaid-0.2.2/src/frenchmaid/modules/ignore.py` & `frenchmaid-0.2.3/src/frenchmaid/modules/ignore.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+from typing import List
 
 def git(directory: str) -> None:
     try:
         f = open(".gitignore", "x")
         f.write("__pycache__/\n.mypy_cache/")
         f.close()
         print(f'\nSuccessfully created a ".gitignore" in your "{directory}" folder. It now ignores all pycache and mypy cache folders!')
         return
     except:
         f_read = open(".gitignore", "r")
         f_write = open(".gitignore", "a")
         f_data = f_read.read()
-        array: list[str] = []
+        array: List[str] = []
 
         if "__pycache__/" not in f_data:
             f_write.write("\n__pycache__/")
             array.append('pycache')
 
         if ".mypy_cache/" not in f_data:
             f_write.write("\n.mypy_cache/")
@@ -41,15 +42,15 @@
         f.close()
         print(f'\nSuccessfully created a ".dockerignore" in your "{directory}" folder. It now ignores all pycache and mypy cache folders!')
         return
     except:
         f_read = open(".dockerignore", "r")
         f_write = open(".dockerignore", "a")
         f_data = f_read.read()
-        array: list[str] = []
+        array: List[str] = []
 
         if "*__pycache__*" not in f_data:
             f_write.write("\n*__pycache__*")
             array.append('pycache')
 
         if ".mypy_cache" not in f_data:
             f_write.write("\n.mypy_cache")
```

### Comparing `frenchmaid-0.2.2/src/frenchmaid/switches/cleanSwitch.py` & `frenchmaid-0.2.3/src/frenchmaid/switches/cleanSwitch.py`

 * *Files identical despite different names*

### Comparing `frenchmaid-0.2.2/src/frenchmaid/switches/ignoreSwitch.py` & `frenchmaid-0.2.3/src/frenchmaid/switches/ignoreSwitch.py`

 * *Files identical despite different names*

### Comparing `frenchmaid-0.2.2/src/frenchmaid.egg-info/PKG-INFO` & `frenchmaid-0.2.3/src/frenchmaid.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: frenchmaid
-Version: 0.2.2
+Version: 0.2.3
 Summary: Remove all pests from your project! frenchmaid is a lightweight all platform cli package that will delete all pycache and other folders (contents included) in your project directory. Are you tired of doing it manually each time? Fear not, the frenchmaid will do it for you!
 Home-page: https://github.com/lewisjr/frenchmaid.git
-Author: Techtronics Solutions Limited | Lewis Mosho Jr
-Author-email: lmosho@techtronicsltd.com
+Author: Cerebrus Inc | Lewis Mosho Jr
+Author-email: lewis@cerebrus.dev
 Project-URL: Bug Tracker, https://github.com/lewisjr/frenchmaid/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -18,15 +18,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
     <img src="https://static.wixstatic.com/media/916fb4_88bd4d4d46e14f0c90f64213970c3a2d~mv2.png/v1/fill/w_750,h_750,al_c,q_90,usm_0.66_1.00_0.01,enc_auto/916fb4_88bd4d4d46e14f0c90f64213970c3a2d~mv2.png" alt="frenchmaid logo" width="250" height="250" />
 </p>
 
-# frenchmaid v0.2.2
+# frenchmaid v0.2.3
 
 Are you a python developer who also/only uses windows and are sick and tired of constantly deteting those pesky `__pycache__` directories? Fear not, **frenchmaid** is here to help! frenchmaid is a CLI app written in pure python that will search your entire project directory and delete any `__pycache__` or other folders (and the files within) in your root directory. Now it can also add these folders to your ignore files!
 
 **Supported Folders**
 
 - \_\_pycache\_\_
 - .mypy_cache
@@ -106,21 +106,21 @@
 
 <br />
 It's really that simple, just ensure that you are in your project's root directory! For clarity, the above example assumes that your project structure is something like this for example:
 <br />
 <br />
 
     example-app
-    ├── main.py
+    ├── LICENSE
     ├── requirements.txt
     └── src
          └── __init__.py
          └── app.py
 
-If the root is `example-app` then you can see that the terminal should be in that folder.
+If the root is `example-app` then you can see that the terminal should be in that dir.
 
 ## Commands
 
 ### clean
 
 Run `frenchmaid clean` in your project's root directory without any arguments to remove all instances of supported folders. If you want to delete all instances of one type of folder and not any others, run the command with an option; For example, `frenchmaid clean mypy`.
 
@@ -159,15 +159,15 @@
 
 or
 
     frenchmaid --version
 
 will return (for example):
 
-    frenchmaid v0.2.2
+    frenchmaid v0.2.3
 
 ### Help
 
 In any terminal in any directory:
 
     frenchmaid --help
 
@@ -189,52 +189,74 @@
 
 Note that this option can also be used in tandem with any command.
 
 ## Support and Reporting
 
 You can report any bugs or improvements [here](https://github.com/lewisjr/home-app/issues), I will try to address them as soon as possible. Feel free to suggest any other files or folders you think it should delete (e.g .pytest_cache) with all context on how they appear. I will happily make it a possibility without breaking the current format! To the best of my abilities of course, and the github page will be updated on any changes.
 
-# Version History
+# Changelog
 
-## v0.2.2
+## v0.2.x
 
-**Minor Patch 2**
+<details open>
+<summary><strong>v0.2.3</strong></summary>
 
-- Updated README version history to include v0.2.1 updates
+- Codebase improvements
+- Full parity between `windows` and `linux` systems; **Full Stability**
+- Added .gitignore
+- README structure changed
+- Note added to v0.2.0 to denote it's instability
+</details>
 
-## v0.2.1
+<details>
+<summary><strong>v0.2.2</strong></summary>
 
-**Minor Patch 1**
+- Updated README version history to include v0.2.1 updates
+</details>
 
-- Fixed ignore format for \_\_pycache\_\_ in git
+<details>
+<summary><strong>v0.2.1</strong></summary>
 
-## v0.2.0
+- Fixed ignore format for **pycache** in git
+</details>
 
-**Major Patch**
+<details>
+<summary><strong>v0.2.0</strong></summary>
 
 - Added a logo to the README
 - Added instructions for a Linux PATH error
 - Added ignore command and arguments
 - Added support for mypy cache folders
 - Added arguments to the clean command
 - Added `--help` context to all commands
 - Moved all functions to a modules folder
 - Added a class switch
 - Typed modules
+- Unstable on linux bases systems
+
+</details>
+<br />
 
-## v0.1.2
+## v0.1.x
 
-**Minor patch 2**
+<details>
+<summary><strong>v0.1.2</strong></summary>
 
 - License has been updated to Apache from MIT effective from the date of this release
 - Notes on potential path problems that can arise from installation on Windows have been added to the README
 
-## v0.1.1
+</details>
 
-**Minor patch**
+<details>
+<summary><strong>v0.1.1</strong></summary>
 
 - Issue on linux machines fixed with directory name post pycache delete
   - The package no longer displays the root directory's full absolute path (e.g Documents/example-app), but rather just the root directory's name (e.g example-app) on linux machines.
 
-## v0.1.0
+</details>
+
+<details>
+<summary><strong>v0.1.0</strong></summary>
+
+- Initial Release; Stable version for use on all platforms
 
-Initial Release; Stable version for use on all platforms.
+</details>
```

### Comparing `frenchmaid-0.2.2/src/frenchmaid.egg-info/SOURCES.txt` & `frenchmaid-0.2.3/src/frenchmaid.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/frenchmaid/__init__.py
 src/frenchmaid/__main__.py
 src/frenchmaid/cli.py
+src/frenchmaid/delcache.py
 src/frenchmaid.egg-info/PKG-INFO
 src/frenchmaid.egg-info/SOURCES.txt
 src/frenchmaid.egg-info/dependency_links.txt
 src/frenchmaid.egg-info/entry_points.txt
 src/frenchmaid.egg-info/requires.txt
 src/frenchmaid.egg-info/top_level.txt
 src/frenchmaid/modules/__init__.py
```

