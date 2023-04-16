# Comparing `tmp/ohmyi3-0.1.0.tar.gz` & `tmp/ohmyi3-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohmyi3-0.1.0.tar", max compression
+gzip compressed data, was "ohmyi3-0.1.1.tar", max compression
```

## Comparing `ohmyi3-0.1.0.tar` & `ohmyi3-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,39 @@
--rw-r--r--   0        0        0     1082 2023-04-15 19:45:51.088364 ohmyi3-0.1.0/LICENSE
--rw-r--r--   0        0        0       43 2023-04-15 22:50:07.408756 ohmyi3-0.1.0/README.md
--rw-r--r--   0        0        0     1980 2023-04-16 06:37:20.784772 ohmyi3-0.1.0/ohmyi3/app.py
--rw-r--r--   0        0        0     1131 2023-04-16 01:52:38.895592 ohmyi3-0.1.0/ohmyi3/commands/entrypoint.py
--rw-r--r--   0        0        0     3058 2023-04-16 15:58:45.569141 ohmyi3-0.1.0/ohmyi3/commands/generate.py
--rw-r--r--   0        0        0      344 2023-04-16 01:50:57.498737 ohmyi3-0.1.0/ohmyi3/commands/info.py
--rw-r--r--   0        0        0     1205 2023-04-16 05:47:31.632014 ohmyi3-0.1.0/ohmyi3/commands/init.py
--rw-r--r--   0        0        0      591 2023-04-16 02:01:06.406276 ohmyi3-0.1.0/ohmyi3/config/app.py
--rw-r--r--   0        0        0     2384 2023-04-16 05:45:45.284535 ohmyi3-0.1.0/ohmyi3/config/package.py
--rw-r--r--   0        0        0      814 2023-04-15 19:45:51.085030 ohmyi3-0.1.0/ohmyi3/services/bootstrap.py
--rw-r--r--   0        0        0     2372 2023-04-16 01:49:15.905195 ohmyi3-0.1.0/ohmyi3/services/ohmyi3.py
--rw-r--r--   0        0        0      810 2023-04-16 01:34:15.198801 ohmyi3-0.1.0/ohmyi3/stubs/config.d/00-header.conf
--rw-r--r--   0        0        0      588 2023-04-16 01:18:24.775431 ohmyi3-0.1.0/ohmyi3/stubs/settings.py
--rw-r--r--   0        0        0      524 2023-04-16 17:34:39.272085 ohmyi3-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 ohmyi3-0.1.0/setup.py
--rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 ohmyi3-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-04-15 19:45:51.088364 ohmyi3-0.1.1/LICENSE
+-rw-r--r--   0        0        0       43 2023-04-15 22:50:07.408756 ohmyi3-0.1.1/README.md
+-rw-r--r--   0        0        0     1659 2023-04-16 19:21:21.603562 ohmyi3-0.1.1/ohmyi3/app.py
+-rw-r--r--   0        0        0     1131 2023-04-16 01:52:38.895592 ohmyi3-0.1.1/ohmyi3/commands/entrypoint.py
+-rw-r--r--   0        0        0     2867 2023-04-16 19:17:23.069039 ohmyi3-0.1.1/ohmyi3/commands/generate.py
+-rw-r--r--   0        0        0      582 2023-04-16 19:17:41.632714 ohmyi3-0.1.1/ohmyi3/commands/info.py
+-rw-r--r--   0        0        0     1221 2023-04-16 19:02:29.594220 ohmyi3-0.1.1/ohmyi3/commands/init.py
+-rw-r--r--   0        0        0      591 2023-04-16 02:01:06.406276 ohmyi3-0.1.1/ohmyi3/config/app.py
+-rw-r--r--   0        0        0     2384 2023-04-16 05:45:45.284535 ohmyi3-0.1.1/ohmyi3/config/package.py
+-rw-r--r--   0        0        0     1141 2023-04-16 19:18:58.080807 ohmyi3-0.1.1/ohmyi3/configurator.py
+-rw-r--r--   0        0        0      814 2023-04-15 19:45:51.085030 ohmyi3-0.1.1/ohmyi3/services/bootstrap.py
+-rw-r--r--   0        0        0     2529 2023-04-16 19:40:39.743720 ohmyi3-0.1.1/ohmyi3/services/ohmyi3.py
+-rw-r--r--   0        0        0      188 2023-04-16 20:00:12.022854 ohmyi3-0.1.1/ohmyi3/stubs/README.md
+-rw-r--r--   0        0        0      810 2023-04-16 19:50:22.554902 ohmyi3-0.1.1/ohmyi3/stubs/config.d/00-header.conf
+-rw-r--r--   0        0        0     1734 2023-04-16 19:50:22.558236 ohmyi3-0.1.1/ohmyi3/stubs/config.d/05-system.conf
+-rw-r--r--   0        0        0     2014 2023-04-16 19:50:22.561569 ohmyi3-0.1.1/ohmyi3/stubs/config.d/10-autostart.conf
+-rw-r--r--   0        0        0      552 2023-04-16 19:50:22.561569 ohmyi3-0.1.1/ohmyi3/stubs/config.d/15-borders.conf
+-rw-r--r--   0        0        0     6209 2023-04-16 19:50:22.564903 ohmyi3-0.1.1/ohmyi3/stubs/config.d/20-navigation.conf
+-rw-r--r--   0        0        0     2962 2023-04-16 19:50:22.564903 ohmyi3-0.1.1/ohmyi3/stubs/config.d/80-applications.conf
+-rw-r--r--   0        0        0     6686 2023-04-16 19:50:22.568236 ohmyi3-0.1.1/ohmyi3/stubs/config.d/85-windows.conf
+-rw-r--r--   0        0        0     3141 2023-04-16 19:50:22.571569 ohmyi3-0.1.1/ohmyi3/stubs/config.d/90-gaps.conf
+-rw-r--r--   0        0        0     6361 2023-04-16 19:57:35.033223 ohmyi3-0.1.1/ohmyi3/stubs/configurator.py
+-rw-r--r--   0        0        0       29 2023-04-16 19:50:30.758322 ohmyi3-0.1.1/ohmyi3/stubs/plugins/archey3/__init__.py
+-rw-r--r--   0        0        0      962 2023-04-16 19:50:30.761655 ohmyi3-0.1.1/ohmyi3/stubs/plugins/archey3/archey3.py
+-rw-r--r--   0        0        0       31 2023-04-16 19:50:30.761655 ohmyi3-0.1.1/ohmyi3/stubs/plugins/nitrogen/__init__.py
+-rw-r--r--   0        0        0     1607 2023-04-16 19:50:30.764989 ohmyi3-0.1.1/ohmyi3/stubs/plugins/nitrogen/nitrogen.py
+-rw-r--r--   0        0        0   385109 2023-04-16 19:50:38.535071 ohmyi3-0.1.1/ohmyi3/stubs/themes/amber/background.jpg
+-rw-r--r--   0        0        0     1841 2023-04-16 19:50:38.535071 ohmyi3-0.1.1/ohmyi3/stubs/themes/amber/theme.conf
+-rw-r--r--   0        0        0   198158 2023-04-16 19:50:38.538404 ohmyi3-0.1.1/ohmyi3/stubs/themes/archlinux/background.jpg
+-rw-r--r--   0        0        0     1882 2023-04-16 19:50:38.541738 ohmyi3-0.1.1/ohmyi3/stubs/themes/archlinux/theme.conf
+-rw-r--r--   0        0        0     1869 2023-04-16 19:50:38.541738 ohmyi3-0.1.1/ohmyi3/stubs/themes/i3status.conf
+-rw-r--r--   0        0        0   108928 2023-04-16 19:50:38.545071 ohmyi3-0.1.1/ohmyi3/stubs/themes/manjaro/background.jpg
+-rw-r--r--   0        0        0     1901 2023-04-16 19:50:38.545071 ohmyi3-0.1.1/ohmyi3/stubs/themes/manjaro/theme.conf
+-rw-r--r--   0        0        0   514555 2023-04-16 19:50:38.548405 ohmyi3-0.1.1/ohmyi3/stubs/themes/pink/background.jpg
+-rw-r--r--   0        0        0     2389 2023-04-16 19:50:38.548405 ohmyi3-0.1.1/ohmyi3/stubs/themes/pink/theme.conf
+-rw-r--r--   0        0        0     1660 2023-04-16 19:32:43.375019 ohmyi3-0.1.1/ohmyi3/util.py
+-rw-r--r--   0        0        0      703 2023-04-16 20:01:27.091497 ohmyi3-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1182 1970-01-01 00:00:00.000000 ohmyi3-0.1.1/setup.py
+-rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 ohmyi3-0.1.1/PKG-INFO
```

### Comparing `ohmyi3-0.1.0/LICENSE` & `ohmyi3-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.0/ohmyi3/app.py` & `ohmyi3-0.1.1/ohmyi3/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,50 @@
 import os
 import sys
 import shutil
 import uvicore
 from uvicore.typing import Dict
 from uvicore.support.dumper import dump, dd
+from ohmyi3.util import path
 
-class App(Dict):
+class Application(Dict):
 
     def __init__(self, must_exist = True):
+
         # Ohmyi3 main folder (~/.config/ohmyi3)
-        # Override with env OHMYI3_CONFIG_PATH
-        self.config_folder = self.path(uvicore.config('ohmyi3.config_path'), must_exist,
-            message="Perhpas you havent run 'i3ctl init' yet??")
-
-        # config.d folder (~/.config/ohmyi3/config.d)
-        self.configd_folder = self.path(self.config_folder + '/config.d', must_exist)
-
-        # themes.d folder (~/.config/ohmyi3/themes.d)
-        self.theme_folder = self.path(self.config_folder + '/themes.d')
-
-        # i3 config path (~/.config/i3) and file
-        # Override with env OHMYI3_I3CONFIG_PATH
-        self.i3config_folder = self.path(uvicore.config('ohmyi3.i3config_path'))
+        self.config_folder = path(uvicore.config('ohmyi3.config_path'), must_exist,
+            notfound_message="Perhpas you havent run 'i3ctl init' yet??")
+
+        # Ohmyi3 i3 configs folder (~/.config/ohmyi3/configs)
+        self.configd_folder = path([self.config_folder, 'config.d'], must_exist)
+
+        # Ohmyi3 i3 themes folder (~/.config/ohmyi3/themes)
+        self.themes_folder = path([self.config_folder, 'themes'])
 
-        # i3status path (~/.config/i3status/config)
-        self.i3status_folder = self.path(uvicore.config('ohmyi3.i3status_path'))
+        # i3 config folder (~/.config/i3)
+        self.i3config_folder = path(uvicore.config('ohmyi3.i3config_path'))
+
+        # i3status path (~/.config/i3status)
+        self.i3status_folder = path(uvicore.config('ohmyi3.i3status_path'))
 
         # Stubs folder
-        self.app_folder = self.path(uvicore.app.package(main=True).path, True)
-        self.stubs_folder = self.path(self.app_folder + '/stubs', True)
+        self.app_folder = path(uvicore.app.package(main=True).path, True)
+        self.stubs_folder = path([self.app_folder, 'stubs'], True)
 
         # Import user settings (~/.config/ohmyi3/settings.py)
         if must_exist:
-            self.settings = self._import_settings();
-
-    def path(self, location, must_exist=False, message=None):
-        real = os.path.realpath(os.path.expanduser(location))
-        if must_exist:
-            if not os.path.exists(real):
-                print(f"{real} not found")
-                if message: print(message)
-                exit(1)
-        return real
+            self.configurator = self._import_configurator();
 
 
     def _cleanup(self):
-        pycache = self.path(self.config_folder + '/__pycache__')
+        pycache = path([self.config_folder, '__pycache__'])
         if os.path.exists(pycache):
             shutil.rmtree(pycache)
 
 
-    def _import_settings(self):
+    def _import_configurator(self):
+        """Dynamically import the users ~/.config/ohmyi3/configurator.py"""
         sys.path.append(os.path.realpath(self.config_folder))
-        from settings import Settings
-        return Settings(self)
+        from configurator import Ohmyi3
+        return Ohmyi3(self)
```

### Comparing `ohmyi3-0.1.0/ohmyi3/commands/entrypoint.py` & `ohmyi3-0.1.1/ohmyi3/commands/entrypoint.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.0/ohmyi3/commands/generate.py` & `ohmyi3-0.1.1/ohmyi3/commands/generate.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,86 +1,81 @@
 import os
 import sys
-import uvicore
 import shutil
+import uvicore
 from glob import glob
-from ohmyi3.app import App
-from datetime import datetime
 from uvicore.typing import Dict
+from ohmyi3.app import Application
+from ohmyi3.util import path, now, template
 from uvicore.support.dumper import dump, dd
 from uvicore.exceptions import SmartException
-from jinja2 import FileSystemLoader, Environment
+
 from uvicore.console import command, argument, option
 
 @command()
 async def cli():
-    """Dynamically Generate the i3 config from config.d/*"""
+    """Dynamically Generate a new i3 config using Ohmyi3"""
 
     # Get the application instance
-    app = App()
+    app = Application()
+
+    # Shortcut to user configurator
+    configurator = app.configurator
 
     # Start the generation
     uvicore.log.header("Generating new i3 config using ohmyi3")
 
     # Fire off user defined before_generate_hook
     uvicore.log.item3("Firing user defined before_generate hook")
-    await app.settings.before_generate()
+    await configurator.before_generate()
 
     # If i3 config exists, back it up
     i3config_file = f"{app.i3config_folder}/config"
     if os.path.exists(i3config_file):
-        now = datetime.now().strftime('%Y-%m-%d_%H-%M-%S')
-        backup = os.path.realpath(f"{app.i3config_folder}/backup-{now}")
+        backup = path([app.i3config_folder, 'backup-' + now()])
         uvicore.log.item(f"Backing up {i3config_file} to {backup}")
         shutil.copy(i3config_file, backup)
 
     # Get all config.d/* files
     os.chdir(app.configd_folder)
     files = sorted(glob("*.conf"))
 
     # Append config.d/* and theme.d/theme to new i3 config
     with open(i3config_file, "w") as f:
         # Loop and merge each config and append to
         for file in files:
             uvicore.log.item2(f"Appending {file}")
-            f.write(template(app.configd_folder, file).render(**app.settings))
+            f.write(template(app.configd_folder, file, **configurator))
             f.write("\n\n\n")
 
         # Append the selected theme files
-        theme_folder = f"{app.theme_folder}/{app.settings.theme}"
-        theme_file = os.path.realpath(f"{theme_folder}/theme.conf")
+        theme_folder = f"{app.themes_folder}/{configurator.theme}"
+        theme_file = path([theme_folder, 'theme.conf'])
         if os.path.exists(theme_file):
-            uvicore.log.item(f"Appending THEME {app.settings.theme}")
-            f.write(template(theme_folder, 'theme.conf').render(**app.settings))
+            uvicore.log.item(f"Appending THEME {configurator.theme}")
+            f.write(template(theme_folder, 'theme.conf', **configurator))
 
     # Copy themed i3status or a default if no theme specific file exists
     i3status_folder = None
     if os.path.exists(f"{theme_folder}/i3status.conf"):
         # Use themed i3status.conf
         i3status_folder = f"{theme_folder}"
-    elif os.path.exists(f"{app.theme_folder}/i3status.conf"):
+    elif os.path.exists(f"{app.themes_folder}/i3status.conf"):
         # Use default i3status.conf
-        i3status_folder = f"{app.theme_folder}"
+        i3status_folder = f"{app.themes_folder}"
     if i3status_folder:
         uvicore.log.item(f"Copying {i3status_folder}/i3status.conf to {app.i3status_folder}/config")
         with open(f"{app.i3status_folder}/config", "w") as f:
-            f.write(template(i3status_folder, 'i3status.conf').render(**app.settings))
+            f.write(template(i3status_folder, 'i3status.conf', **configurator))
 
     # Fire off user defined afer_generate_hook
     uvicore.log.item3("Firing user defined after_generate hook")
-    await app.settings.after_generate()
+    await configurator.after_generate()
 
     # Cleanup
     app._cleanup()
 
     # Done
     uvicore.log.nl()
     uvicore.log("Done!")
     uvicore.log(f"New {i3config_file} generated!")
     uvicore.log("Please reload i3!")
-
-
-def template(path, file):
-    loader = FileSystemLoader(searchpath=path)
-    env = Environment(loader=loader)
-    return env.get_template(file)
-
```

### Comparing `ohmyi3-0.1.0/ohmyi3/commands/init.py` & `ohmyi3-0.1.1/ohmyi3/commands/init.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
 import shutil
 import uvicore
-from ohmyi3.app import App
+from ohmyi3.app import Application
 from uvicore.support.dumper import dump, dd
 from uvicore.exceptions import SmartException
 from uvicore.console import command, argument, option
 
 @command()
 async def cli():
     """Initialize a stock ~/.config/ohmyi3/* configuration"""
 
     # Get the application instance
-    app = App(must_exist=False);
+    app = Application(must_exist=False);
 
     uvicore.log.header('Initializing ohmyi3')
 
     # Create ~/.config/ohmyi3/ and copy stubs
     if not os.path.exists(app.config_folder):
         uvicore.log.item(f"Creating {app.config_folder} folder")
         #os.mkdir(app.config_folder)
```

### Comparing `ohmyi3-0.1.0/ohmyi3/config/app.py` & `ohmyi3-0.1.1/ohmyi3/config/app.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.0/ohmyi3/config/package.py` & `ohmyi3-0.1.1/ohmyi3/config/package.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.0/ohmyi3/services/bootstrap.py` & `ohmyi3-0.1.1/ohmyi3/services/bootstrap.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.0/ohmyi3/services/ohmyi3.py` & `ohmyi3-0.1.1/ohmyi3/services/ohmyi3.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,11 +43,14 @@
 
         # Or you can define commands as kwargs (multiple calls to self.commands() are appended)
         self.commands(
             group='i3ctl',
             help='Ohmyi3 i3ctl Commands and Setuptools Entrypoint',
             commands={
                 'generate': 'ohmyi3.commands.generate.cli',
+                'gen': 'ohmyi3.commands.generate.cli',
+                'g': 'ohmyi3.commands.generate.cli',
                 'init': 'ohmyi3.commands.init.cli',
                 'info': 'ohmyi3.commands.info.cli',
+                'i': 'ohmyi3.commands.info.cli',
             },
         )
```

### Comparing `ohmyi3-0.1.0/ohmyi3/stubs/config.d/00-header.conf` & `ohmyi3-0.1.1/ohmyi3/stubs/config.d/00-header.conf`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.0/setup.py` & `ohmyi3-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,35 +2,43 @@
 from setuptools import setup
 
 packages = \
 ['ohmyi3',
  'ohmyi3.commands',
  'ohmyi3.config',
  'ohmyi3.services',
- 'ohmyi3.stubs']
+ 'ohmyi3.stubs',
+ 'ohmyi3.stubs.plugins.archey3',
+ 'ohmyi3.stubs.plugins.nitrogen']
 
 package_data = \
-{'': ['*'], 'ohmyi3.stubs': ['config.d/*']}
+{'': ['*'],
+ 'ohmyi3.stubs': ['config.d/*',
+                  'themes/*',
+                  'themes/amber/*',
+                  'themes/archlinux/*',
+                  'themes/manjaro/*',
+                  'themes/pink/*']}
 
 install_requires = \
 ['jinja2>=3.1.0,<3.2.0', 'uvicore==0.1.25']
 
 entry_points = \
 {'console_scripts': ['i3ctl = ohmyi3.commands.entrypoint:cli']}
 
 setup_kwargs = {
     'name': 'ohmyi3',
-    'version': '0.1.0',
-    'description': '',
+    'version': '0.1.1',
+    'description': 'Dynamic i3 Configuration Manager ',
     'long_description': '# Ohmyi3\n\nDynamic i3 configuration manager\n',
     'author': 'Matthew Reschke',
     'author_email': 'mail@mreschke.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/ohmyi3/ohmyi3',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.7,<4.0',
 }
```

### Comparing `ohmyi3-0.1.0/PKG-INFO` & `ohmyi3-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: ohmyi3
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: Dynamic i3 Configuration Manager 
+Home-page: https://github.com/ohmyi3/ohmyi3
 License: MIT
 Author: Matthew Reschke
 Author-email: mail@mreschke.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jinja2 (>=3.1.0,<3.2.0)
 Requires-Dist: uvicore (==0.1.25)
+Project-URL: Documentation, https://github.com/ohmyi3/ohmyi3
+Project-URL: Repository, https://github.com/ohmyi3/ohmyi3
 Description-Content-Type: text/markdown
 
 # Ohmyi3
 
 Dynamic i3 configuration manager
```

