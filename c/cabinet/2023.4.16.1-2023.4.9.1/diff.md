# Comparing `tmp/cabinet-2023.4.16.1.tar.gz` & `tmp/cabinet-2023.4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cabinet-2023.4.16.1.tar", last modified: Sun Apr 16 07:16:11 2023, max compression
+gzip compressed data, was "cabinet-2023.4.9.1.tar", last modified: Mon Apr 10 04:09:49 2023, max compression
```

## Comparing `cabinet-2023.4.16.1.tar` & `cabinet-2023.4.9.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-16 07:16:11.903584 cabinet-2023.4.16.1/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11357 2023-03-06 03:35:41.000000 cabinet-2023.4.16.1/LICENSE
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6160 2023-04-16 07:16:11.903584 cabinet-2023.4.16.1/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     5808 2023-04-16 07:10:22.000000 cabinet-2023.4.16.1/README.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2023-03-06 04:41:10.000000 cabinet-2023.4.16.1/pyproject.toml
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      750 2023-04-16 07:16:11.903584 cabinet-2023.4.16.1/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-16 07:16:11.903584 cabinet-2023.4.16.1/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-16 07:16:11.903584 cabinet-2023.4.16.1/src/cabinet/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    23710 2023-04-16 07:14:49.000000 cabinet-2023.4.16.1/src/cabinet/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       69 2023-03-25 22:04:50.000000 cabinet-2023.4.16.1/src/cabinet/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2737 2023-03-25 22:04:50.000000 cabinet-2023.4.16.1/src/cabinet/mail.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-16 07:16:11.903584 cabinet-2023.4.16.1/src/cabinet.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6160 2023-04-16 07:16:11.000000 cabinet-2023.4.16.1/src/cabinet.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      288 2023-04-16 07:16:11.000000 cabinet-2023.4.16.1/src/cabinet.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-04-16 07:16:11.000000 cabinet-2023.4.16.1/src/cabinet.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2023-04-16 07:16:11.000000 cabinet-2023.4.16.1/src/cabinet.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2023-04-16 07:16:11.000000 cabinet-2023.4.16.1/src/cabinet.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-10 04:09:49.754821 cabinet-2023.4.9.1/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11357 2023-03-06 03:35:41.000000 cabinet-2023.4.9.1/LICENSE
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     4365 2023-04-10 04:09:49.754821 cabinet-2023.4.9.1/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     4014 2023-03-25 22:04:50.000000 cabinet-2023.4.9.1/README.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2023-03-06 04:41:10.000000 cabinet-2023.4.9.1/pyproject.toml
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      750 2023-04-10 04:09:49.754821 cabinet-2023.4.9.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-10 04:09:49.754821 cabinet-2023.4.9.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-10 04:09:49.754821 cabinet-2023.4.9.1/src/cabinet/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    20802 2023-03-25 22:04:50.000000 cabinet-2023.4.9.1/src/cabinet/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       69 2023-03-25 22:04:50.000000 cabinet-2023.4.9.1/src/cabinet/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2737 2023-03-25 22:04:50.000000 cabinet-2023.4.9.1/src/cabinet/mail.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-10 04:09:49.754821 cabinet-2023.4.9.1/src/cabinet.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     4365 2023-04-10 04:09:49.000000 cabinet-2023.4.9.1/src/cabinet.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      288 2023-04-10 04:09:49.000000 cabinet-2023.4.9.1/src/cabinet.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-04-10 04:09:49.000000 cabinet-2023.4.9.1/src/cabinet.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2023-04-10 04:09:49.000000 cabinet-2023.4.9.1/src/cabinet.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2023-04-10 04:09:49.000000 cabinet-2023.4.9.1/src/cabinet.egg-info/top_level.txt
```

### Comparing `cabinet-2023.4.16.1/LICENSE` & `cabinet-2023.4.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cabinet-2023.4.16.1/PKG-INFO` & `cabinet-2023.4.9.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2023.4.16.1
+Version: 2023.4.9.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cabinet
 A Python library to easily store data across multiple projects in one or more JSON files.
 
-Supports a cli, email, and event logging.
+Supports email and event logging.
 
 ## Features
 
 - Read and write data in the JSON files of your choice
 - Log to a file/directory of your choice without having to configure `logger` each time
 - Send/receive mail using `cabinet.Cabinet().mail()`
 
@@ -28,191 +28,131 @@
   - this can be changed on a per-log basis
 
 ## Installation and Setup
 
 ```bash
   python3 -m pip install cabinet
 
-  cabinet --config
-```
-
-## CLI usage
-```
-Usage: cabinet [OPTIONS]
-
-Options:
-  -h, --help              Show this help message and exit
-  --configure, -config    Configure
-  --edit, -e              Edit the settings.json file
-  --edit-file, -ef        Edit a specific file
-  --no-create             (for -ef) Do not create file if it does not exist
-  --get, -g [GET ...]     Get a property from settings.json
-  --put PUT [PUT ...]     Put a property into settings.json
-  --get-file GET_FILE     Get file
-  --strip                 (for --get-file) Whether to strip file content whitespace
-  --log, -l               Log a message to the default location
-  --level LOG_LEVEL       (for -l) Log level [debug, info, warn, error, critical]
-  -v, --version           show version number and exit
+  cabinet config
 ```
 
 ## Configuration
 
-- Upon first launch, will prompt you to choose a location for `settings.json`. You can change this at any time with `cabinet --config`.
+- Upon first launch, will prompt you to choose a location for `settings.json`. You can change this at any time with `cabinet config`.
 
-### edit_file() shortcuts
-- see example below to enable something like
-  - `cabinet -ef shopping` from the terminal
-    - rather than `cabinet -ef "/home/{username}/path/to/shopping_list.md"`
-  - or `cabinet.Cabinet().edit("shopping")`
-    - rather than `cabinet.Cabinet().edit("/home/{username}/path/to/whatever.md")`
+### edit() shortcuts
+- see example below to enable something like `cabinet edit shopping` from the terminal
+  - or `cabinet.Cabinet().edit("shopping")`, rather than `cabinet.Cabinet().edit("/home/{username}/path/to/shopping.md")`
 
-file:
 ```
 # example only; these commands will be unique to your setup
 
 {
   "path": {
     "edit": {
       "shopping": {
-        "value": "/home/{username}/path/to/whatever.md",
+        "value": "/home/{username}/path/to/shopping.md",
       },
       "todo": {
-        "value": "/home/{username}/path/to/whatever.md",
+        "value": "/home/{username}/path/to/todo.md",
       }
     }
   }
 }
 ```
 
-set from terminal:
-```
-cabinet -p edit shopping value "/home/{username}/path/to/whatever.md"
-cabinet -p edit todo value "/home/{username}/path/to/whatever.md"
-```
-
 ### mail
 
 - It is NEVER a good idea to store your password in plaintext; for this reason, I strongly recommend a "throwaway" account that is only used for sending emails
 - Gmail (as of May 2022) and most other mainstream email providers won't work with this; for support, search for sending mail from your email provider with `smtplib`.
 - In `settings.json`, add the `email` object to make your settings file look like this example:
 
-file:
 ```
 {
     "email": {
         "from": "throwaway@example.com",
         "from_pw": "example",
         "from_name": "Raspberry Pi",
         "to": "destination@protonmail.com",
         "smtp_server": "example.com",
         "imap_server": "example.com",
         "port": 123
     }
 }
 ```
 
-set from terminal:
-```
-cabinet -p email from throwaway@example.com
-cabinet -p email from_pw example
-...
-```
-
 ## Examples
 
-### `put`
+### `set`
 
-python:
 ```
 from cabinet import Cabinet
 
 cab = Cabinet()
 
-cab.put("employee", "Tyler", "salary", 7.25)
-```
-
-or terminal:
-```
-# warning - from the terminal, numeric values in cabinet are stored as strings
-cabinet -p employer Tyler salary 7.25
+cab.set("employee", "Tyler", "salary", 7.25)
 ```
 
 results in this structure in settings.json:
+
 ```
 {
     "employee": {
         "Tyler": {
-            "salary": 7.25 # or "7.25" if done from terminal
+            "salary": 7.25
         }
     }
 }
 ```
 
 ### `get`
 
-python:
 ```
 from cabinet import Cabinet
 
 cab = Cabinet()
 
 print(cab.get("employee", "Tyler", "salary"))
 ```
 
-or terminal:
-```
-cabinet -g employee Tyler salary
-```
-
-results in:
 ```
-7.25
+> python3 test.py
+> 7.25
 ```
 
-### `edit_file`
+### `edit`
 
-python:
 ```
 from cabinet import Cabinet
 
 cab = Cabinet()
 
-# if put("path", "edit", "shopping", "/path/to/shopping.md") has been called, this will edit the file assigned to that shortcut.
+# if set("path", "edit", "shopping", "/path/to/shopping.md") has been called, this will edit the file assigned to that shortcut.
 
 # opens file in Vim, saves upon exit
 cab.edit("shopping")
 
 # or you can edit a file directly...
 cab.edit("/path/to/shopping.md")
 ```
 
-terminal:
-```
-# assumes path -> edit -> shopping -> path/to/shopping.md has been set
-cabinet -ef shoppping
-
-or 
-
-cabinet -ef "/path/to/shopping.md"
-```
-
 ### `mail`
 
 ```
 
 from cabinet import mail
 
 mail.send('Test Subject', 'Test Body')
 
 ```
 
 ### `log`
 
-python:
 ```
+
 from cabinet import Cabinet
 
 cab = Cabinet()
 
 # writes to a file named LOG_DAILY_YYYY-MM-DD in the default log folder (or cab.get('path', 'log')) inside a YYYY-MM-DD folder
 
 cab.log("Connection timed out") # defaults to 'info' if no level is set
@@ -229,34 +169,26 @@
 cab.log("30", logName="LOG_TEMPERATURE", filePath="/home/{username}/weather")
 
     # format
     # 2021-12-29 19:29:27,896 — INFO — 30
 
 ```
 
-terminal:
-```
-# defaults to 'info' if no level is set
-cab -l "Connection timed out" 
-
-# -l and --log are interchangeable
-cab --log "Connection timed out"
-
-# change levels with --level
-cab --log "Server is on fire" --level "critical"
-```
-
 ## Dependencies
 
 - Python >= 3.6
 - smtplib
 
 ## Disclaimers
 
 - Although I've done quite a bit of testing, I can't guarantee everything that works on my machine will work on yours. Always back up your data to multiple places to avoid data loss.
 - If you find any issues, please contact me... or get your hands dirty and raise a PR!
 
+```
+
+```
+
 ## Author
 
 - Tyler Woodfin
   - [GitHub](https://www.github.com/tylerjwoodfin)
   - [Website](http://tyler.cloud)
```

### Comparing `cabinet-2023.4.16.1/README.md` & `cabinet-2023.4.9.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # cabinet
 A Python library to easily store data across multiple projects in one or more JSON files.
 
-Supports a cli, email, and event logging.
+Supports email and event logging.
 
 ## Features
 
 - Read and write data in the JSON files of your choice
 - Log to a file/directory of your choice without having to configure `logger` each time
 - Send/receive mail using `cabinet.Cabinet().mail()`
 
@@ -16,191 +16,131 @@
   - this can be changed on a per-log basis
 
 ## Installation and Setup
 
 ```bash
   python3 -m pip install cabinet
 
-  cabinet --config
-```
-
-## CLI usage
-```
-Usage: cabinet [OPTIONS]
-
-Options:
-  -h, --help              Show this help message and exit
-  --configure, -config    Configure
-  --edit, -e              Edit the settings.json file
-  --edit-file, -ef        Edit a specific file
-  --no-create             (for -ef) Do not create file if it does not exist
-  --get, -g [GET ...]     Get a property from settings.json
-  --put PUT [PUT ...]     Put a property into settings.json
-  --get-file GET_FILE     Get file
-  --strip                 (for --get-file) Whether to strip file content whitespace
-  --log, -l               Log a message to the default location
-  --level LOG_LEVEL       (for -l) Log level [debug, info, warn, error, critical]
-  -v, --version           show version number and exit
+  cabinet config
 ```
 
 ## Configuration
 
-- Upon first launch, will prompt you to choose a location for `settings.json`. You can change this at any time with `cabinet --config`.
+- Upon first launch, will prompt you to choose a location for `settings.json`. You can change this at any time with `cabinet config`.
 
-### edit_file() shortcuts
-- see example below to enable something like
-  - `cabinet -ef shopping` from the terminal
-    - rather than `cabinet -ef "/home/{username}/path/to/shopping_list.md"`
-  - or `cabinet.Cabinet().edit("shopping")`
-    - rather than `cabinet.Cabinet().edit("/home/{username}/path/to/whatever.md")`
+### edit() shortcuts
+- see example below to enable something like `cabinet edit shopping` from the terminal
+  - or `cabinet.Cabinet().edit("shopping")`, rather than `cabinet.Cabinet().edit("/home/{username}/path/to/shopping.md")`
 
-file:
 ```
 # example only; these commands will be unique to your setup
 
 {
   "path": {
     "edit": {
       "shopping": {
-        "value": "/home/{username}/path/to/whatever.md",
+        "value": "/home/{username}/path/to/shopping.md",
       },
       "todo": {
-        "value": "/home/{username}/path/to/whatever.md",
+        "value": "/home/{username}/path/to/todo.md",
       }
     }
   }
 }
 ```
 
-set from terminal:
-```
-cabinet -p edit shopping value "/home/{username}/path/to/whatever.md"
-cabinet -p edit todo value "/home/{username}/path/to/whatever.md"
-```
-
 ### mail
 
 - It is NEVER a good idea to store your password in plaintext; for this reason, I strongly recommend a "throwaway" account that is only used for sending emails
 - Gmail (as of May 2022) and most other mainstream email providers won't work with this; for support, search for sending mail from your email provider with `smtplib`.
 - In `settings.json`, add the `email` object to make your settings file look like this example:
 
-file:
 ```
 {
     "email": {
         "from": "throwaway@example.com",
         "from_pw": "example",
         "from_name": "Raspberry Pi",
         "to": "destination@protonmail.com",
         "smtp_server": "example.com",
         "imap_server": "example.com",
         "port": 123
     }
 }
 ```
 
-set from terminal:
-```
-cabinet -p email from throwaway@example.com
-cabinet -p email from_pw example
-...
-```
-
 ## Examples
 
-### `put`
+### `set`
 
-python:
 ```
 from cabinet import Cabinet
 
 cab = Cabinet()
 
-cab.put("employee", "Tyler", "salary", 7.25)
-```
-
-or terminal:
-```
-# warning - from the terminal, numeric values in cabinet are stored as strings
-cabinet -p employer Tyler salary 7.25
+cab.set("employee", "Tyler", "salary", 7.25)
 ```
 
 results in this structure in settings.json:
+
 ```
 {
     "employee": {
         "Tyler": {
-            "salary": 7.25 # or "7.25" if done from terminal
+            "salary": 7.25
         }
     }
 }
 ```
 
 ### `get`
 
-python:
 ```
 from cabinet import Cabinet
 
 cab = Cabinet()
 
 print(cab.get("employee", "Tyler", "salary"))
 ```
 
-or terminal:
-```
-cabinet -g employee Tyler salary
-```
-
-results in:
 ```
-7.25
+> python3 test.py
+> 7.25
 ```
 
-### `edit_file`
+### `edit`
 
-python:
 ```
 from cabinet import Cabinet
 
 cab = Cabinet()
 
-# if put("path", "edit", "shopping", "/path/to/shopping.md") has been called, this will edit the file assigned to that shortcut.
+# if set("path", "edit", "shopping", "/path/to/shopping.md") has been called, this will edit the file assigned to that shortcut.
 
 # opens file in Vim, saves upon exit
 cab.edit("shopping")
 
 # or you can edit a file directly...
 cab.edit("/path/to/shopping.md")
 ```
 
-terminal:
-```
-# assumes path -> edit -> shopping -> path/to/shopping.md has been set
-cabinet -ef shoppping
-
-or 
-
-cabinet -ef "/path/to/shopping.md"
-```
-
 ### `mail`
 
 ```
 
 from cabinet import mail
 
 mail.send('Test Subject', 'Test Body')
 
 ```
 
 ### `log`
 
-python:
 ```
+
 from cabinet import Cabinet
 
 cab = Cabinet()
 
 # writes to a file named LOG_DAILY_YYYY-MM-DD in the default log folder (or cab.get('path', 'log')) inside a YYYY-MM-DD folder
 
 cab.log("Connection timed out") # defaults to 'info' if no level is set
@@ -217,34 +157,26 @@
 cab.log("30", logName="LOG_TEMPERATURE", filePath="/home/{username}/weather")
 
     # format
     # 2021-12-29 19:29:27,896 — INFO — 30
 
 ```
 
-terminal:
-```
-# defaults to 'info' if no level is set
-cab -l "Connection timed out" 
-
-# -l and --log are interchangeable
-cab --log "Connection timed out"
-
-# change levels with --level
-cab --log "Server is on fire" --level "critical"
-```
-
 ## Dependencies
 
 - Python >= 3.6
 - smtplib
 
 ## Disclaimers
 
 - Although I've done quite a bit of testing, I can't guarantee everything that works on my machine will work on yours. Always back up your data to multiple places to avoid data loss.
 - If you find any issues, please contact me... or get your hands dirty and raise a PR!
 
+```
+
+```
+
 ## Author
 
 - Tyler Woodfin
   - [GitHub](https://www.github.com/tylerjwoodfin)
   - [Website](http://tyler.cloud)
```

### Comparing `cabinet-2023.4.16.1/setup.cfg` & `cabinet-2023.4.9.1/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cabinet
-version = 2023.04.16.1
+version = 2023.04.09.1
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily manage data storage and logging across repos
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/cabinet
 project_urls =
```

### Comparing `cabinet-2023.4.16.1/src/cabinet/__init__.py` & `cabinet-2023.4.9.1/src/cabinet/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,18 +12,16 @@
 """
 
 import os
 import json
 import pathlib
 import logging
 import sys
-import argparse
 from datetime import date
 from typing import Optional
-import importlib.metadata
 
 
 class Cabinet:
     """
     The main class for Cabinet
     """
 
@@ -278,41 +276,28 @@
         file_handler = logging.FileHandler(
             f"{file_path}/{log_name}.log", mode='a')
         file_handler.setFormatter(log_format)
 
         logger.addHandler(file_handler)
         return logger
 
-    def _ifprint(self, message: str, is_print: bool):
-        """
-        Prints a string if `print` is true.
-        """
-        if is_print:
-            print(message)
-
     def configure(self):
         """
         Configures the Cabinet instance based on command line arguments or user input.
         """
 
         message = f"""
 Enter the full path of the directory where you want to store 
 all data (currently {self.path_cabinet}):\n"""
 
         self._put_config('path_cabinet', input(message))
 
-    def edit(self):
-        """
-        Edits and saves the settings file.
-        """
-        self.edit_file(self.path_settings_file)
-
     def edit_file(self, file_path: str = None, create_if_not_exist: bool = True) -> None:
         """
-        Edit and save a file in Vim.
+        Edit and save a file using Vim.
 
         Args:
             - file_path (str, optional): The path to the file to edit. 
                 Allows for shortcuts by setting paths in settings.json -> path -> edit
                 If unset, edit settings.json
 
             - create_if_not_exist (bool, optional): Whether to create the file if it does not exist.
@@ -363,15 +348,15 @@
 
         with open(file_path, "r", encoding="utf-8") as file:
             new_contents = file.readlines()
 
         if original_contents == new_contents:
             print("No changes.")
 
-    def get(self, *attributes, warn_missing=False, is_print=False):
+    def get(self, *attributes, warn_missing=False):
         """
         Returns a property in a JSON file based on the input attributes.
 
         Args:
             - attributes (str): the attributes to traverse in the JSON file
             - warn_missing (bool, optional): whether to warn if an attribute is missing
 
@@ -379,36 +364,32 @@
             - The value of the attribute if it exists in the JSON file, otherwise default.
 
         Usage:
             - get('person', 'tyler', 'salary') returns person -> tyler -> salary from self.settings
         """
 
         if self.settings_json is None:
-            self._ifprint("None", is_print)
             return None
 
         settings = self.settings_json
 
         for index, item in enumerate(attributes):
             if item in settings:
                 settings = settings[item]
             elif warn_missing and (len(attributes) < 2 or attributes[1] != "edit"):
-                is_print(
+                print(
                     f"Warning: {item} not found in \
                         {settings if index > 0 else f'{self.path_cabinet}/settings.json'}")
-                self._ifprint("None", is_print)
                 return None
             else:
-                self._ifprint("None", is_print)
                 return None
 
-        self._ifprint(settings, is_print)
         return settings
 
-    def put(self, *attribute, value=None, file_name='settings.json', is_print=False):
+    def put(self, *attribute, value=None, file_name='settings.json'):
         """
         Adds or replaces a property in a JSON file (default name: settings.json).
 
         Args:
             *attribute (str): A series of keys in the JSON object
                 to identify the location of the property.
             value (optional): The value to put into the property.
@@ -426,39 +407,33 @@
 
         _settings = self.settings_json if file_name == 'settings.json' else json.load(
             open(path_full, encoding="utf8"))
 
         # iterate through entire JSON object and replace 2nd to last attribute with value
 
         partition = _settings
-
         for index, item in enumerate(attribute[:-1]):
             if item not in partition:
-                try:
-                    partition[item] = value if index == len(attribute) - 2 else {}
-                    partition = partition[item]
-                    self.log(f"Adding new key '{item}' to {partition if index > 0 else path_full}",
-                             level="warn")
-                except TypeError as error:
-                    self.log(f"{error}\n\n{attribute[index-1]} is currently a string, so it cannot \
-be treated as an object with multiple properties.", level="error")
+                partition[item] = value if index == len(attribute) - 2 else {}
+                partition = partition[item]
+                print(
+                    f"Warning: Adding new key '{item}' to {partition if index > 0 else path_full}")
             else:
                 if index == len(attribute) - 2:
                     partition[item] = value
                 else:
                     partition = partition[item]
 
         with open(path_full, 'w+', encoding="utf8") as file:
             json.dump(_settings, file, indent=4)
 
-        self._ifprint(f"{' -> '.join(attribute[:-1])} set to {value}", is_print)
         return value
 
     def get_file_as_array(self, item: str, file_path=None, strip: bool = True,
-                          ignore_not_found: bool = False):
+                          ignore_not_found: bool = False) -> list[str]:
         """
         Reads a file and returns its contents as a list of lines.
         The file is assumed to be encoded in UTF-8.
 
         Args:
             - item (str): The filename to read.
             - file_path (str, optional): The path to the directory containing the file.
@@ -525,15 +500,15 @@
             if not is_quiet:
                 print(f"Wrote to '{file_path}/{file_name}'")
             return True
         except (OSError, IOError) as error:
             self.log(f"write_file: {error}", level="error")
             return False
 
-    def log(self, message: str = '', log_name: str = None, level: str = None,
+    def log(self, message: str = '', log_name: str = None, level: str = 'info',
             file_path: str = None, is_quiet: bool = False) -> None:
         """
         Logs a message using the specified log level
         and writes it to a file if a file path is provided.
 
         Args:
             message (str, optional): The message to log. Defaults to ''.
@@ -549,17 +524,14 @@
         Raises:
             ValueError: If an invalid log level is provided.
 
         Returns:
             None
         """
 
-        if level is None:
-            level = 'info'
-
         # validate log level
         valid_levels = {'debug', 'info', 'warn',
                         'warning', 'error', 'critical'}
         if level.lower() not in valid_levels:
             raise ValueError(
                 f"Invalid log level: {level}. Must be one of {', '.join(valid_levels)}.")
 
@@ -584,61 +556,21 @@
 
     Usage:
         (from the terminal)
         cabinet config
         cabinet edit <file path/name, optional; default: settings.json>
     """
 
-
-    cab = Cabinet()
-    package_name = sys.modules[__name__].__package__.split('.')[0]
-    version = importlib.metadata.version(package_name)
-
-    parser = argparse.ArgumentParser(
-        description=f"Cabinet ({version})")
-
-    parser.add_argument('--configure', '-config', dest='configure',
-                        action='store_true', help='Configure')
-    parser.add_argument('--edit', '-e', dest='edit', action='store_true',
-                        help='Edit the settings.json file')
-    parser.add_argument('--edit-file', '-ef', type=str, dest='edit_file',
-                        help='Edit a specific file')
-    parser.add_argument('--no-create', dest='create',
-                        action='store_false',
-                        help='(for -ef) Do not create file if it does not exist')
-    parser.add_argument('--get', '-g', dest='get', nargs='+',
-                        help='Get a property from settings.json')
-    parser.add_argument('--put', '-p', dest='put', nargs='+',
-                        help='Put a property into settings.json')
-    parser.add_argument('--get-file', dest='get_file',
-                        type=str, help='Get file')
-    parser.add_argument('--strip', dest='strip', action='store_false',
-                        help='(for --get-file) Whether to strip file content whitespace')
-    parser.add_argument('--log','-l', type=str,
-                        dest='log', help='Log a message to the default location')
-    parser.add_argument('--level', type=str, dest='log_level',
-                        help='(for -l) Log level [debug, info, warn, error, critical]')
-    parser.add_argument('-v', '--version',
-                        action='version', help='Show version number and exit', version=version)
-
-    args = parser.parse_args()
-
-    if args.configure:
-        cab.configure()
-    elif args.edit:
-        cab.edit()
-    elif args.edit_file:
-        cab.edit_file(file_path=args.edit_file, create_if_not_exist=args.create)
-    elif args.get:
-        cab.get(is_print=True, *args.get)
-    elif args.put:
-        attribute_values = args.put
-        cab.put(*attribute_values, is_print=True)
-    elif args.get_file:
-        cab.get_file_as_array(item=args.get_file,
-                              file_path=None, strip=args.strip)
-    elif args.log:
-        cab.log(message=args.log, level=args.log_level)
+    if len(sys.argv) < 2:
+        print("Cabinet is not intended to be directly run. See README.md.")
+        sys.exit(0)
+
+    if "cabinet" in sys.argv[0] and len(sys.argv) > 1:
+        if "config" == sys.argv[1]:
+            Cabinet().configure()
+        elif "edit" == sys.argv[1]:
+            path = None if len(sys.argv) < 3 else sys.argv[2]
+            Cabinet().edit_file(path)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `cabinet-2023.4.16.1/src/cabinet/mail.py` & `cabinet-2023.4.9.1/src/cabinet/mail.py`

 * *Files identical despite different names*

### Comparing `cabinet-2023.4.16.1/src/cabinet.egg-info/PKG-INFO` & `cabinet-2023.4.9.1/src/cabinet.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2023.4.16.1
+Version: 2023.4.9.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cabinet
 A Python library to easily store data across multiple projects in one or more JSON files.
 
-Supports a cli, email, and event logging.
+Supports email and event logging.
 
 ## Features
 
 - Read and write data in the JSON files of your choice
 - Log to a file/directory of your choice without having to configure `logger` each time
 - Send/receive mail using `cabinet.Cabinet().mail()`
 
@@ -28,191 +28,131 @@
   - this can be changed on a per-log basis
 
 ## Installation and Setup
 
 ```bash
   python3 -m pip install cabinet
 
-  cabinet --config
-```
-
-## CLI usage
-```
-Usage: cabinet [OPTIONS]
-
-Options:
-  -h, --help              Show this help message and exit
-  --configure, -config    Configure
-  --edit, -e              Edit the settings.json file
-  --edit-file, -ef        Edit a specific file
-  --no-create             (for -ef) Do not create file if it does not exist
-  --get, -g [GET ...]     Get a property from settings.json
-  --put PUT [PUT ...]     Put a property into settings.json
-  --get-file GET_FILE     Get file
-  --strip                 (for --get-file) Whether to strip file content whitespace
-  --log, -l               Log a message to the default location
-  --level LOG_LEVEL       (for -l) Log level [debug, info, warn, error, critical]
-  -v, --version           show version number and exit
+  cabinet config
 ```
 
 ## Configuration
 
-- Upon first launch, will prompt you to choose a location for `settings.json`. You can change this at any time with `cabinet --config`.
+- Upon first launch, will prompt you to choose a location for `settings.json`. You can change this at any time with `cabinet config`.
 
-### edit_file() shortcuts
-- see example below to enable something like
-  - `cabinet -ef shopping` from the terminal
-    - rather than `cabinet -ef "/home/{username}/path/to/shopping_list.md"`
-  - or `cabinet.Cabinet().edit("shopping")`
-    - rather than `cabinet.Cabinet().edit("/home/{username}/path/to/whatever.md")`
+### edit() shortcuts
+- see example below to enable something like `cabinet edit shopping` from the terminal
+  - or `cabinet.Cabinet().edit("shopping")`, rather than `cabinet.Cabinet().edit("/home/{username}/path/to/shopping.md")`
 
-file:
 ```
 # example only; these commands will be unique to your setup
 
 {
   "path": {
     "edit": {
       "shopping": {
-        "value": "/home/{username}/path/to/whatever.md",
+        "value": "/home/{username}/path/to/shopping.md",
       },
       "todo": {
-        "value": "/home/{username}/path/to/whatever.md",
+        "value": "/home/{username}/path/to/todo.md",
       }
     }
   }
 }
 ```
 
-set from terminal:
-```
-cabinet -p edit shopping value "/home/{username}/path/to/whatever.md"
-cabinet -p edit todo value "/home/{username}/path/to/whatever.md"
-```
-
 ### mail
 
 - It is NEVER a good idea to store your password in plaintext; for this reason, I strongly recommend a "throwaway" account that is only used for sending emails
 - Gmail (as of May 2022) and most other mainstream email providers won't work with this; for support, search for sending mail from your email provider with `smtplib`.
 - In `settings.json`, add the `email` object to make your settings file look like this example:
 
-file:
 ```
 {
     "email": {
         "from": "throwaway@example.com",
         "from_pw": "example",
         "from_name": "Raspberry Pi",
         "to": "destination@protonmail.com",
         "smtp_server": "example.com",
         "imap_server": "example.com",
         "port": 123
     }
 }
 ```
 
-set from terminal:
-```
-cabinet -p email from throwaway@example.com
-cabinet -p email from_pw example
-...
-```
-
 ## Examples
 
-### `put`
+### `set`
 
-python:
 ```
 from cabinet import Cabinet
 
 cab = Cabinet()
 
-cab.put("employee", "Tyler", "salary", 7.25)
-```
-
-or terminal:
-```
-# warning - from the terminal, numeric values in cabinet are stored as strings
-cabinet -p employer Tyler salary 7.25
+cab.set("employee", "Tyler", "salary", 7.25)
 ```
 
 results in this structure in settings.json:
+
 ```
 {
     "employee": {
         "Tyler": {
-            "salary": 7.25 # or "7.25" if done from terminal
+            "salary": 7.25
         }
     }
 }
 ```
 
 ### `get`
 
-python:
 ```
 from cabinet import Cabinet
 
 cab = Cabinet()
 
 print(cab.get("employee", "Tyler", "salary"))
 ```
 
-or terminal:
-```
-cabinet -g employee Tyler salary
-```
-
-results in:
 ```
-7.25
+> python3 test.py
+> 7.25
 ```
 
-### `edit_file`
+### `edit`
 
-python:
 ```
 from cabinet import Cabinet
 
 cab = Cabinet()
 
-# if put("path", "edit", "shopping", "/path/to/shopping.md") has been called, this will edit the file assigned to that shortcut.
+# if set("path", "edit", "shopping", "/path/to/shopping.md") has been called, this will edit the file assigned to that shortcut.
 
 # opens file in Vim, saves upon exit
 cab.edit("shopping")
 
 # or you can edit a file directly...
 cab.edit("/path/to/shopping.md")
 ```
 
-terminal:
-```
-# assumes path -> edit -> shopping -> path/to/shopping.md has been set
-cabinet -ef shoppping
-
-or 
-
-cabinet -ef "/path/to/shopping.md"
-```
-
 ### `mail`
 
 ```
 
 from cabinet import mail
 
 mail.send('Test Subject', 'Test Body')
 
 ```
 
 ### `log`
 
-python:
 ```
+
 from cabinet import Cabinet
 
 cab = Cabinet()
 
 # writes to a file named LOG_DAILY_YYYY-MM-DD in the default log folder (or cab.get('path', 'log')) inside a YYYY-MM-DD folder
 
 cab.log("Connection timed out") # defaults to 'info' if no level is set
@@ -229,34 +169,26 @@
 cab.log("30", logName="LOG_TEMPERATURE", filePath="/home/{username}/weather")
 
     # format
     # 2021-12-29 19:29:27,896 — INFO — 30
 
 ```
 
-terminal:
-```
-# defaults to 'info' if no level is set
-cab -l "Connection timed out" 
-
-# -l and --log are interchangeable
-cab --log "Connection timed out"
-
-# change levels with --level
-cab --log "Server is on fire" --level "critical"
-```
-
 ## Dependencies
 
 - Python >= 3.6
 - smtplib
 
 ## Disclaimers
 
 - Although I've done quite a bit of testing, I can't guarantee everything that works on my machine will work on yours. Always back up your data to multiple places to avoid data loss.
 - If you find any issues, please contact me... or get your hands dirty and raise a PR!
 
+```
+
+```
+
 ## Author
 
 - Tyler Woodfin
   - [GitHub](https://www.github.com/tylerjwoodfin)
   - [Website](http://tyler.cloud)
```

