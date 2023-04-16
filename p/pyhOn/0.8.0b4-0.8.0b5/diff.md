# Comparing `tmp/pyhOn-0.8.0b4.tar.gz` & `tmp/pyhOn-0.8.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhOn-0.8.0b4.tar", last modified: Sat Apr 15 20:28:26 2023, max compression
+gzip compressed data, was "pyhOn-0.8.0b5.tar", last modified: Sun Apr 16 11:59:58 2023, max compression
```

## Comparing `pyhOn-0.8.0b4.tar` & `pyhOn-0.8.0b5.tar`

### file list

```diff
@@ -1,40 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:28:26.199605 pyhOn-0.8.0b4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-15 20:28:26.199605 pyhOn-0.8.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:28:26.195605 pyhOn-0.8.0b4/pyhOn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-15 20:28:26.000000 pyhOn-0.8.0b4/pyhOn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-15 20:28:26.000000 pyhOn-0.8.0b4/pyhOn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 20:28:26.000000 pyhOn-0.8.0b4/pyhOn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-15 20:28:26.000000 pyhOn-0.8.0b4/pyhOn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 20:28:26.000000 pyhOn-0.8.0b4/pyhOn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-15 20:28:26.000000 pyhOn-0.8.0b4/pyhOn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:28:26.195605 pyhOn-0.8.0b4/pyhon/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3251 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/appliance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:28:26.199605 pyhOn-0.8.0b4/pyhon/appliances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/appliances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/appliances/ov.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/appliances/td.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/appliances/wd.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/appliances/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:28:26.199605 pyhOn-0.8.0b4/pyhon/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/connection/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/connection/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/connection/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:28:26.199605 pyhOn-0.8.0b4/pyhon/connection/handler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/connection/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/connection/handler/anonym.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/connection/handler/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/connection/handler/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/connection/handler/hon.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/hon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 20:28:26.199605 pyhOn-0.8.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:59:58.600005 pyhOn-0.8.0b5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-16 11:59:58.600005 pyhOn-0.8.0b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:59:58.596005 pyhOn-0.8.0b5/pyhOn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-16 11:59:58.000000 pyhOn-0.8.0b5/pyhOn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-16 11:59:58.000000 pyhOn-0.8.0b5/pyhOn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 11:59:58.000000 pyhOn-0.8.0b5/pyhOn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 11:59:58.000000 pyhOn-0.8.0b5/pyhOn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-16 11:59:58.000000 pyhOn-0.8.0b5/pyhOn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 11:59:58.000000 pyhOn-0.8.0b5/pyhOn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:59:58.596005 pyhOn-0.8.0b5/pyhon/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3251 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/appliance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:59:58.596005 pyhOn-0.8.0b5/pyhon/appliances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/appliances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/appliances/dw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/appliances/td.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/appliances/wd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/appliances/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:59:58.596005 pyhOn-0.8.0b5/pyhon/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/connection/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/connection/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/connection/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:59:58.596005 pyhOn-0.8.0b5/pyhon/connection/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/connection/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/connection/handler/anonym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/connection/handler/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/connection/handler/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/connection/handler/hon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/hon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:59:58.600005 pyhOn-0.8.0b5/pyhon/parameter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/parameter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/parameter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/parameter/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/parameter/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/parameter/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/parameter/range.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 11:59:58.600005 pyhOn-0.8.0b5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/setup.py
```

### Comparing `pyhOn-0.8.0b4/LICENSE` & `pyhOn-0.8.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b4/PKG-INFO` & `pyhOn-0.8.0b5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.8.0b4
+Version: 0.8.0b5
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.8.0b4/README.md` & `pyhOn-0.8.0b5/README.md`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b4/pyhOn.egg-info/PKG-INFO` & `pyhOn-0.8.0b5/pyhOn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.8.0b4
+Version: 0.8.0b5
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.8.0b4/pyhon/__main__.py` & `pyhOn-0.8.0b5/pyhon/__main__.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b4/pyhon/appliance.py` & `pyhOn-0.8.0b5/pyhon/appliance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import importlib
 from contextlib import suppress
 from typing import Optional, Dict, Any
 from typing import TYPE_CHECKING
 
 from pyhon import helper
 from pyhon.commands import HonCommand
-from pyhon.parameter import HonParameterFixed
+from pyhon.parameter.fixed import HonParameterFixed
 
 if TYPE_CHECKING:
     from pyhon import HonAPI
 
 
 class HonAppliance:
     def __init__(
@@ -120,16 +120,16 @@
                     if d.get("command", {}).get("commandName") == name
                 ),
                 None,
             )
             if last is None:
                 continue
             parameters = command_history[last].get("command", {}).get("parameters", {})
-            if command._multi and parameters.get("program"):
-                command.set_program(parameters.pop("program").split(".")[-1].lower())
+            if command.programs and parameters.get("program"):
+                command.program = parameters.pop("program").split(".")[-1].lower()
                 command = self.commands[name]
             for key, data in command.settings.items():
                 if (
                     not isinstance(data, HonParameterFixed)
                     and parameters.get(key) is not None
                 ):
                     with suppress(ValueError):
@@ -145,15 +145,20 @@
             if "parameters" in attr:
                 commands[command] = HonCommand(command, attr, self._api, self)
             elif "parameters" in attr[list(attr)[0]]:
                 multi = {}
                 for program, attr2 in attr.items():
                     program = program.split(".")[-1].lower()
                     cmd = HonCommand(
-                        command, attr2, self._api, self, multi=multi, program=program
+                        command,
+                        attr2,
+                        self._api,
+                        self,
+                        programs=multi,
+                        program_name=program,
                     )
                     multi[program] = cmd
                     commands[command] = cmd
         self._commands = commands
         await self._recover_last_command_states(commands)
 
     @property
@@ -166,15 +171,17 @@
             return self._extra.settings(result)
         return result
 
     @property
     def parameters(self):
         result = {}
         for name, command in self._commands.items():
-            for key, parameter in command.parameters.items():
+            for key, parameter in (
+                command.parameters | command.ancillary_parameters
+            ).items():
                 result.setdefault(name, {})[key] = parameter.value
         return result
 
     async def load_attributes(self):
         self._attributes = await self._api.load_attributes(self)
         for name, values in self._attributes.pop("shadow").get("parameters").items():
             self._attributes.setdefault("parameters", {})[name] = values["parNewVal"]
```

### Comparing `pyhOn-0.8.0b4/pyhon/connection/api.py` & `pyhOn-0.8.0b5/pyhon/connection/api.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import json
 import logging
 from datetime import datetime
 from typing import Dict, Optional
-from typing_extensions import Self
 
 from aiohttp import ClientSession
+from typing_extensions import Self
 
 from pyhon import const, exceptions
 from pyhon.appliance import HonAppliance
 from pyhon.connection.auth import HonAuth
-from pyhon.connection.handler.hon import HonConnectionHandler
 from pyhon.connection.handler.anonym import HonAnonymousConnectionHandler
+from pyhon.connection.handler.hon import HonConnectionHandler
 
 _LOGGER = logging.getLogger()
 
 
 class HonAPI:
     def __init__(
         self,
```

### Comparing `pyhOn-0.8.0b4/pyhon/connection/auth.py` & `pyhOn-0.8.0b5/pyhon/connection/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 import logging
 import re
 import secrets
 import urllib
 from contextlib import suppress
 from dataclasses import dataclass
 from datetime import datetime, timedelta
-from pprint import pformat
-from typing import Dict, Optional, List
+from typing import Dict, Optional
 from urllib import parse
 from urllib.parse import quote
 
 from aiohttp import ClientResponse
 from yarl import URL
 
 from pyhon import const, exceptions
```

### Comparing `pyhOn-0.8.0b4/pyhon/connection/device.py` & `pyhOn-0.8.0b5/pyhon/connection/device.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b4/pyhon/connection/handler/anonym.py` & `pyhOn-0.8.0b5/pyhon/connection/handler/anonym.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b4/pyhon/connection/handler/auth.py` & `pyhOn-0.8.0b5/pyhon/connection/handler/auth.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b4/pyhon/connection/handler/base.py` & `pyhOn-0.8.0b5/pyhon/connection/handler/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from collections.abc import AsyncIterator
 from contextlib import asynccontextmanager
-from typing import Optional, Callable, Dict, Any
+from typing import Optional, Callable, Dict
 
 import aiohttp
 from typing_extensions import Self
 
 from pyhon import const, exceptions
 
 _LOGGER = logging.getLogger(__name__)
```

### Comparing `pyhOn-0.8.0b4/pyhon/connection/handler/hon.py` & `pyhOn-0.8.0b5/pyhon/connection/handler/hon.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b4/pyhon/helper.py` & `pyhOn-0.8.0b5/pyhon/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 
 def create_command(commands, concat=False):
     result = {}
     for name, command in commands.items():
         if not concat:
             result[name] = {}
-        for parameter, data in command.parameters.items():
+        for parameter, data in command.settings.items():
             if data.typology == "enum":
                 value = data.values
             elif data.typology == "range":
                 value = {"min": data.min, "max": data.max, "step": data.step}
             else:
                 continue
             if not concat:
```

### Comparing `pyhOn-0.8.0b4/pyhon/hon.py` & `pyhOn-0.8.0b5/pyhon/hon.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 import asyncio
-import copy
-from typing import List, Optional, Dict, Any
-from typing_extensions import Self
+from types import TracebackType
+from typing import List, Optional, Dict, Any, Type
 
 from aiohttp import ClientSession
+from typing_extensions import Self
 
 from pyhon import HonAPI, exceptions
 from pyhon.appliance import HonAppliance
 
 
 class Hon:
     def __init__(self, email: str, password: str, session: ClientSession | None = None):
         self._email: str = email
         self._password: str = password
         self._session: ClientSession | None = session
         self._appliances: List[HonAppliance] = []
         self._api: Optional[HonAPI] = None
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> Self:
         return await self.create()
 
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
+    async def __aexit__(
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc: Optional[BaseException],
+        traceback: Optional[TracebackType],
+    ) -> None:
         await self.close()
 
     @property
     def api(self) -> HonAPI:
         if self._api is None:
             raise exceptions.NoAuthenticationException
         return self._api
@@ -49,16 +54,17 @@
                 appliance.load_attributes(),
                 appliance.load_commands(),
                 appliance.load_statistics(),
             ]
         )
         self._appliances.append(appliance)
 
-    async def setup(self):
+    async def setup(self) -> None:
         appliance: Dict
-        for appliance in (await self._api.load_appliances())["payload"]["appliances"]:
-            for zone in range(int(appliance.get("zone", "0"))):
-                await self._create_appliance(appliance.copy(), zone=zone + 1)
+        for appliance in (await self.api.load_appliances())["payload"]["appliances"]:
+            if (zones := int(appliance.get("zone", "0"))) > 1:
+                for zone in range(zones):
+                    await self._create_appliance(appliance.copy(), zone=zone + 1)
             await self._create_appliance(appliance)
 
-    async def close(self):
-        await self._api.close()
+    async def close(self) -> None:
+        await self.api.close()
```

### Comparing `pyhOn-0.8.0b4/setup.py` & `pyhOn-0.8.0b5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pyhOn",
-    version="0.8.0b4",
+    version="0.8.0b5",
     author="Andre Basche",
     description="Control hOn devices with python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         "GitHub": "https://github.com/Andre0512/pyhOn",
         "PyPI": "https://pypi.org/project/pyhOn",
```

