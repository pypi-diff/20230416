# Comparing `tmp/scsm-0.2.7.tar.gz` & `tmp/scsm-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scsm-0.2.7.tar", last modified: Sun Dec 12 05:52:03 2021, max compression
+gzip compressed data, was "scsm-0.2.8.tar", max compression
```

## Comparing `scsm-0.2.7.tar` & `scsm-0.2.8.tar`

### file list

```diff
@@ -1,25 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-12 05:52:03.362256 scsm-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-12-12 05:51:52.000000 scsm-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       75 2021-12-12 05:51:52.000000 scsm-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2097 2021-12-12 05:52:03.362256 scsm-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1251 2021-12-12 05:51:52.000000 scsm-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-12 05:52:03.362256 scsm-0.2.7/scsm/
--rw-r--r--   0 runner    (1001) docker     (121)      334 2021-12-12 05:51:52.000000 scsm-0.2.7/scsm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20833 2021-12-12 05:51:52.000000 scsm-0.2.7/scsm/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2392 2021-12-12 05:51:52.000000 scsm-0.2.7/scsm/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    16682 2021-12-12 05:51:52.000000 scsm-0.2.7/scsm/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-12 05:52:03.362256 scsm-0.2.7/scsm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2097 2021-12-12 05:52:03.000000 scsm-0.2.7/scsm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      369 2021-12-12 05:52:03.000000 scsm-0.2.7/scsm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-12 05:52:03.000000 scsm-0.2.7/scsm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2021-12-12 05:52:03.000000 scsm-0.2.7/scsm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2021-12-12 05:52:03.000000 scsm-0.2.7/scsm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-12-12 05:52:03.000000 scsm-0.2.7/scsm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2021-12-12 05:52:03.366256 scsm-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1284 2021-12-12 05:51:52.000000 scsm-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-12 05:52:03.362256 scsm-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-12 05:51:52.000000 scsm-0.2.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1541 2021-12-12 05:51:52.000000 scsm-0.2.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     6076 2021-12-12 05:51:52.000000 scsm-0.2.7/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      183 2021-12-12 05:51:52.000000 scsm-0.2.7/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     4798 2021-12-12 05:51:52.000000 scsm-0.2.7/tests/test_core.py
+-rw-r--r--   0        0        0    35149 2023-04-16 03:40:26.778482 scsm-0.2.8/LICENSE
+-rw-r--r--   0        0        0     1019 2023-04-16 03:40:26.778482 scsm-0.2.8/README.md
+-rw-r--r--   0        0        0     1201 2023-04-16 03:40:26.778482 scsm-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      334 2023-04-16 03:40:26.778482 scsm-0.2.8/scsm/__init__.py
+-rw-r--r--   0        0        0    20847 2023-04-16 03:40:26.778482 scsm-0.2.8/scsm/cli.py
+-rw-r--r--   0        0        0     2286 2023-04-16 03:40:26.778482 scsm-0.2.8/scsm/config.py
+-rw-r--r--   0        0        0    17701 2023-04-16 03:40:26.778482 scsm-0.2.8/scsm/core.py
+-rw-r--r--   0        0        0       37 2023-04-16 03:40:27.246479 scsm-0.2.8/scsm/data/.git
+-rw-r--r--   0        0        0    35149 2023-04-16 03:40:27.982474 scsm-0.2.8/scsm/data/LICENSE
+-rw-r--r--   0        0        0       43 2023-04-16 03:40:27.982474 scsm-0.2.8/scsm/data/README.md
+-rw-r--r--   0        0        0      370 2023-04-16 03:40:27.982474 scsm-0.2.8/scsm/data/apps/105600.yaml
+-rw-r--r--   0        0        0      534 2023-04-16 03:40:27.982474 scsm-0.2.8/scsm/data/apps/111710.yaml
+-rw-r--r--   0        0        0      556 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/17505.yaml
+-rw-r--r--   0        0        0      545 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/17515.yaml
+-rw-r--r--   0        0        0      554 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/17575.yaml
+-rw-r--r--   0        0        0      285 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/211820.yaml
+-rw-r--r--   0        0        0      363 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/215350.yaml
+-rw-r--r--   0        0        0      363 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/215360.yaml
+-rw-r--r--   0        0        0      538 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/222840.yaml
+-rw-r--r--   0        0        0      534 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/222860.yaml
+-rw-r--r--   0        0        0      328 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/223249.yaml
+-rw-r--r--   0        0        0      328 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/223250.yaml
+-rw-r--r--   0        0        0      504 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/228780.yaml
+-rw-r--r--   0        0        0      529 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/232250.yaml
+-rw-r--r--   0        0        0      542 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/232290.yaml
+-rw-r--r--   0        0        0      521 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/232330.yaml
+-rw-r--r--   0        0        0      550 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/232370.yaml
+-rw-r--r--   0        0        0      257 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/233780.yaml
+-rw-r--r--   0        0        0      547 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/237410.yaml
+-rw-r--r--   0        0        0      238 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/244310.yaml
+-rw-r--r--   0        0        0      553 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/255470.yaml
+-rw-r--r--   0        0        0      543 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/258550.yaml
+-rw-r--r--   0        0        0      311 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/261140.yaml
+-rw-r--r--   0        0        0      232 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/270150.yaml
+-rw-r--r--   0        0        0      252 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/294420.yaml
+-rw-r--r--   0        0        0      533 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/295230.yaml
+-rw-r--r--   0        0        0      235 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/310.yaml
+-rw-r--r--   0        0        0      198 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/312070.yaml
+-rw-r--r--   0        0        0      398 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/313900.yaml
+-rw-r--r--   0        0        0      565 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/317670.yaml
+-rw-r--r--   0        0        0      563 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/317800.yaml
+-rw-r--r--   0        0        0      242 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/332670.yaml
+-rw-r--r--   0        0        0      241 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/332850.yaml
+-rw-r--r--   0        0        0      271 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/338440.yaml
+-rw-r--r--   0        0        0      430 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/343050.yaml
+-rw-r--r--   0        0        0      450 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/346680.yaml
+-rw-r--r--   0        0        0      272 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/349090.yaml
+-rw-r--r--   0        0        0      601 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/376030.yaml
+-rw-r--r--   0        0        0      283 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/380840.yaml
+-rw-r--r--   0        0        0      244 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/380870.yaml
+-rw-r--r--   0        0        0      409 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/383410.yaml
+-rw-r--r--   0        0        0      563 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/4020.yaml
+-rw-r--r--   0        0        0      306 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/403240.yaml
+-rw-r--r--   0        0        0      333 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/405100.yaml
+-rw-r--r--   0        0        0      495 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/41080.yaml
+-rw-r--r--   0        0        0      270 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/416880.yaml
+-rw-r--r--   0        0        0      560 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/427520.yaml
+-rw-r--r--   0        0        0      285 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/443030.yaml
+-rw-r--r--   0        0        0      457 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/460040.yaml
+-rw-r--r--   0        0        0      469 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/462310.yaml
+-rw-r--r--   0        0        0      471 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/475370.yaml
+-rw-r--r--   0        0        0      400 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/4940.yaml
+-rw-r--r--   0        0        0      239 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/497110.yaml
+-rw-r--r--   0        0        0      523 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/581330.yaml
+-rw-r--r--   0        0        0      384 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/629800.yaml
+-rw-r--r--   0        0        0      259 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/739590.yaml
+-rw-r--r--   0        0        0      629 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/740.yaml
+-rw-r--r--   0        0        0     3050 2023-04-16 03:40:27.986474 scsm-0.2.8/scsm/data/apps/90.yaml
+-rw-r--r--   0        0        0      232 2023-04-16 03:40:26.778482 scsm-0.2.8/scsm/scsm-complete.sh
+-rw-r--r--   0        0        0     1913 1970-01-01 00:00:00.000000 scsm-0.2.8/setup.py
+-rw-r--r--   0        0        0     2330 1970-01-01 00:00:00.000000 scsm-0.2.8/PKG-INFO
```

### Comparing `scsm-0.2.7/LICENSE` & `scsm-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `scsm-0.2.7/README.md` & `scsm-0.2.8/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # SteamCMD Server Manager ( SCSM )
 [![PyPi version](https://img.shields.io/pypi/v/scsm.svg)](https://pypi.org/project/scsm/)
 [![Actions Status: CI](https://github.com/bubylou/scsm/actions/workflows/tests.yml/badge.svg)](https://github.com/bubylou/scsm/actions?query=workflow)
-[![Codecov coverage](https://img.shields.io/codecov/c/github/bubylou/scsm.svg)](https://codecov.io/gh/bubylou/scsm)
-[![PyUp status](https://pyup.io/repos/github/bubylou/scsm/shield.svg)](https://pyup.io/repos/github/bubylou/scsm)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 SCSM is a python program used to manage SteamCMD servers. It includes a core library, basic configuration file management, and a command line interface.
 
 ## Features
 
 - Backup / Restore
 - Install / Update / Validate
 - Start / Stop / Restart / Kill
 - Monitor running servers
 - Multiple server support
 
 ## Requirments
 
-- python (3.6+)
+- python (3.9+)
 - pip
-- screen
 - steamcmd
+- tmux
 
 If SteamCMD is not available in your repository you can install it through SCSM itself by using the `scsm install steamcmd` command.
 
 ## Install
 
 Install using pip.
 ```
```

### Comparing `scsm-0.2.7/scsm/cli.py` & `scsm-0.2.8/scsm/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -666,13 +666,13 @@
     message('Status', 'SteamCMD installing')
 
     steamcmd = SteamCMD()
     steamcmd.install()
     message('Status', 'SteamCMD installed')
 
     message('Status', 'SteamCMD updating')
-    exit_code, text = steamcmd.update()
+    exit_code = steamcmd.update()
 
     if exit_code == 0:
         message('Status', 'SteamCMD updated')
     else:
-        message('Error', text)
+        message('Error', 'SteamCMD update failed')
```

### Comparing `scsm-0.2.7/scsm/config.py` & `scsm-0.2.8/scsm/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
+import yaml
 import platform
 from pathlib import Path
-from pkg_resources import resource_filename
-from ruamel.yaml import YAML
+import scsm
 
 
 if platform.system() != 'Windows':
     if os.geteuid() == 0:
         BASE_DIR = Path('/opt/scsm')
     else:
         BASE_DIR = Path('~/.local/share/scsm').expanduser()
@@ -27,32 +27,31 @@
         username: anonymous
         password:
     """
 
 
 class Config():
     system_wide = False
-    data_dir = resource_filename(__name__, 'data')
+    data_dir = Path(scsm.__path__[0], 'data')
 
     if platform.system() != 'Windows':
         config_dir = Path('~/.config/scsm').expanduser()
         if not config_dir.exists() and Path('/etc/scsm').exists():
             system_wide = True
             config_dir = Path('/etc/scsm')
     else:
         config_dir = Path(os.getenv('APPDATA'), 'scsm')
 
-    _yaml = YAML(typ='safe')
     config_f = Path(config_dir, 'config.yaml')
 
     if config_f.exists():
         with open(config_f, 'r') as _f:
-            data = _yaml.load(_f)
+            data = yaml.safe_load(_f)
     else:
-        data = _yaml.load(DEFAULTS)
+        data = yaml.safe_load(DEFAULTS)
 
     compression = str(data['general']['compression'])
     steam_guard = str(data['general']['steam_guard'])
     max_backups = int(data['general']['max_backups'])
     wait_time = int(data['general']['wait_time'])
     app_dir = Path(data['directories']['app_dir'])
     backup_dir = Path(data['directories']['backup_dir'])
@@ -70,13 +69,12 @@
             config_dir = Path(os.getenv('APPDATA'), 'scsm')
 
         Path(config_dir, 'apps').mkdir(parents=True, exist_ok=True)
         Config.config_dir = config_dir
         Config.config_f = Path(config_dir, 'config.yaml')
 
         with open(Path(config_dir, 'config.yaml'), 'w') as f:
-            yaml = YAML(typ='safe')
-            yaml.dump(yaml.load(DEFAULTS), f)
+            yaml.dump(yaml.safe_load(DEFAULTS), f)
 
     @staticmethod
     def remove():
         Config.config_f.unlink()
```

### Comparing `scsm-0.2.7/scsm/core.py` & `scsm-0.2.8/scsm/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from datetime import datetime
 from pathlib import Path
 from urllib.request import urlretrieve
 from zipfile import ZipFile
 
 import libtmux
 import vdf
-from ruamel.yaml import YAML
+import yaml
 
 from .config import Config
 
 
 class App():
     def __init__(self, app, app_dir, backup_dir=None, platform=None):
         self.app_id, self.app_name, self.server_name = Index.search(app)
@@ -27,16 +27,15 @@
         # check for user app config file
         d = Path(Config.config_dir, 'apps')
         if d.exists() and Path(d, f).is_file():
             self.config_f = Path(d, f)
             self.config_is_default = False
 
         with open(self.config_f, 'r') as f:
-            yaml = YAML(typ='safe')
-            data = yaml.load(f)
+            data = yaml.safe_load(f)
 
         self.app_names = list(data['apps'].keys())
         if not self.app_name:
             self.app_name = self.app_names[0]
 
         self.server_names = list(data['apps'][self.app_name]['servers'].keys())
 
@@ -157,15 +156,28 @@
         app_dir = self.app_dir.parent
         if not os.listdir(app_dir):
             app_dir.rmdir()
 
     def restore(self, backup):
         '''Restore specified backup file'''
         with tarfile.open(Path(self.backup_dir, backup)) as tar:
-            tar.extractall(self.app_dir.parent)
+            def is_within_directory(directory, target):
+                abs_directory = os.path.abspath(directory)
+                abs_target = os.path.abspath(target)
+                prefix = os.path.commonprefix([abs_directory, abs_target])
+                return prefix == abs_directory
+
+            def safe_extract(tar, path=".", members=None, *, numeric_owner=False):
+                for member in tar.getmembers():
+                    member_path = os.path.join(path, member.name)
+                    if not is_within_directory(path, member_path):
+                        raise Exception("Attempted Path Traversal in Tar File")
+                tar.extractall(path, members, numeric_owner=numeric_owner) 
+
+            safe_extract(tar, self.app_dir.parent)
 
         if self.config_is_default:
             self.copy_config()
 
     def update(self, username='anonymous', password='',
                steam_guard='', validate=False):
         '''Update app using steamcmd'''
@@ -196,30 +208,28 @@
     def list(directory):
         '''Return appid or app_name if not only app for app_id'''
         directory = Path(directory)
         if not directory.exists():
             return
 
         with open(Index.f, 'r') as f:
-            yaml = YAML(typ='safe')
-            data = yaml.load(f)
+            data = yaml.safe_load(f)
 
         for app_id in directory.iterdir():
             if len(data[int(app_id.name)].keys()) > 1:
                 for app_name in Path(directory, app_id).iterdir():
                     yield app_name.name
             else:
                 yield app_id.name
 
     @staticmethod
     def list_all():
         '''Return generator of all app_id's in index'''
         with open(Index.f, 'r') as f:
-            yaml = YAML(typ='safe')
-            data = yaml.load(f)
+            data = yaml.safe_load(f)
 
         for app_id in data.keys():
             app_names = data[app_id].keys()
 
             if len(app_names) > 1:
                 for app_name in app_names:
                     yield app_name
@@ -231,16 +241,15 @@
         '''Search index for app and return app_id, app_name, and server_name'''
         try:
             app = int(app)
         except ValueError:
             pass
 
         with open(Index.f, 'r') as f:
-            yaml = YAML(typ='safe')
-            data = yaml.load(f)
+            data = yaml.safe_load(f)
 
         if app in data.keys():
             return app, None, None
 
         for app_id in data.keys():
             if app in data[app_id].keys():
                 if app in data[app_id][app]:
@@ -255,38 +264,36 @@
     def update():
         '''Update index with latst app config files'''
         app_index = {}
         for d in Index.config_dirs():
             for f in d.iterdir():
                 if Path(f).suffix == '.yaml':
                     with open(Path(d, f), 'r') as config_f:
-                        yaml = YAML(typ='safe')
-                        data = yaml.load(config_f)
+                        data = yaml.safe_load(config_f)
 
                     for app in data['apps'].keys():
                         app_index[data['app_id']] = {app: list(data['apps'][app]
                                                                ['servers'].keys())}
 
         with open(Index.f, 'w') as f:
-            yaml = YAML(typ='safe')
             yaml.dump(app_index, f)
 
 
 class Server(App):
     def __init__(self, app, app_dir, backup_dir=None,  platform=None):
         super(Server, self).__init__(app, app_dir, backup_dir, platform)
         if not self.server_name:
             self.server_name = self.server_names[0]
 
         self.tmux = libtmux.Server()
         self.session_name = f'{self.app_name}-{self.server_name}'
 
         try:
-            self.session = self.tmux.find_where({'session_name': self.session_name})
-        except libtmux.exc.LibTmuxException:
+            self.session = self.tmux.sessions.filter(session_name=self.session_name)[0]
+        except IndexError:
             self.session = None
 
     @property
     def running(self):
         '''Return True if app is running'''
         if self.server_name == self.app_name:
             return Server.running_check(self.app_name)
@@ -303,35 +310,31 @@
     @staticmethod
     def running_check(app_name, server_name=None):
         '''Check if server or app is running'''
         tmux = libtmux.Server()
 
         if server_name:
             try:
-                session = tmux.find_where({'session_name': f'{app_name}-{server_name}'})
+                session = tmux.sessions.filter(f'{app_name}-{server_name}')[0]
                 if session:
                     return True
                 return False
-            except libtmux.exc.LibTmuxException:
+            except IndexError:
                 return False
         else:
-            # tmux.find_where does not work with partial names
-            try:
-                for session in tmux.list_sessions():
-                    if session.name.startswith(f'{app_name}-'):
-                        return True
-            except libtmux.exc.LibTmuxException:
-                return False
+            for session in tmux.sessions:
+                if session.name.startswith(f'{app_name}-'):
+                    return True
+            return False
 
     def send(self, command):
         '''Send command to tmux session'''
-        window = self.session.list_windows()[0]
-        pane = window.list_panes()[0]
+        pane = self.session.windows[0].panes[0]
         # suppress_history and literal must be false for c-c to work
-        pane.send_keys(command, enter=True, suppress_history=False, literal=False, )
+        pane.send_keys(command, enter=True, suppress_history=False, literal=False)
 
     def start(self, debug=False):
         '''Start server'''
         if self.library:
             cmd = f'LD_LIBRARY_PATH={self.library} {self.exe} '
         else:
             cmd = f'{self.exe} '
@@ -382,16 +385,16 @@
             return True
         return self.directory.exists() and self.exe.is_file()
 
     def app_update(self, app_id, app_dir, beta=None, beta_password=None,
                    config=None, platform=None, validate=False,
                    username='anonymous', password='', steam_guard='',):
         '''+app_update wrapper'''
-        cmd = ['+login', username, password, steam_guard, '+force_install_dir',
-               app_dir, '+app_update', str(app_id), '+quit']
+        cmd = ['+force_install_dir', app_dir, '+login', username, password,
+               steam_guard, '+app_update', str(app_id), '+quit']
 
         if config:
             cmd.insert(-3, f'+app_set_config {app_id} {config}')
         if beta:
             cmd.insert(-1, f'-beta {beta}')
         if beta_password:
             cmd.insert(-1, f'-betapassword {beta_password}')
@@ -454,15 +457,28 @@
         url = f'{base_url}/{f}'
 
         self.directory.mkdir(parents=True, exist_ok=True)
         urlretrieve(url, Path(self.directory, f))
 
         if pf.system() != 'Windows':
             with tarfile.open(Path(self.directory, f)) as tar:
-                tar.extractall(self.directory)
+                def is_within_directory(directory, target):
+                    abs_directory = os.path.abspath(directory)
+                    abs_target = os.path.abspath(target)
+                    prefix = os.path.commonprefix([abs_directory, abs_target])
+                    return prefix == abs_directory
+
+                def safe_extract(tar, path=".", members=None, *, numeric_owner=False):
+                    for member in tar.getmembers():
+                        member_path = os.path.join(path, member.name)
+                        if not is_within_directory(path, member_path):
+                            raise Exception("Attempted Path Traversal in Tar File")
+                    tar.extractall(path, members, numeric_owner=numeric_owner) 
+
+                safe_extract(tar, self.directory)
         else:
             with ZipFile(Path(self.directory, f)) as zipf:
                 zipf.extractall(self.directory)
 
     def license(self, app_id, username='anonymous', password='', steam_guard=''):
         '''Check if user has a license for app_id'''
         cmd = [self.exe, '+login', username, password, steam_guard,
```

