# Comparing `tmp/connpy-3.0.5.tar.gz` & `tmp/connpy-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connpy-3.0.5.tar", last modified: Fri Apr 14 21:32:13 2023, max compression
+gzip compressed data, was "connpy-3.0.6.tar", last modified: Sun Apr 16 01:41:45 2023, max compression
```

## Comparing `connpy-3.0.5.tar` & `connpy-3.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:32:13.171288 connpy-3.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-14 21:31:58.000000 connpy-3.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-04-14 21:32:13.171288 connpy-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-04-14 21:31:58.000000 connpy-3.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:32:13.171288 connpy-3.0.5/connpy/
--rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-04-14 21:31:58.000000 connpy-3.0.5/connpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 21:31:58.000000 connpy-3.0.5/connpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 21:31:58.000000 connpy-3.0.5/connpy/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-14 21:31:58.000000 connpy-3.0.5/connpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-14 21:31:58.000000 connpy-3.0.5/connpy/completion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11869 2023-04-14 21:31:58.000000 connpy-3.0.5/connpy/configfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47220 2023-04-14 21:31:58.000000 connpy-3.0.5/connpy/connapp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27894 2023-04-14 21:31:58.000000 connpy-3.0.5/connpy/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:32:13.171288 connpy-3.0.5/connpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-04-14 21:32:13.000000 connpy-3.0.5/connpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-14 21:32:13.000000 connpy-3.0.5/connpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:32:13.000000 connpy-3.0.5/connpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 21:32:13.000000 connpy-3.0.5/connpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 21:32:13.000000 connpy-3.0.5/connpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 21:32:13.000000 connpy-3.0.5/connpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-14 21:32:13.171288 connpy-3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-14 21:31:58.000000 connpy-3.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 01:41:45.301464 connpy-3.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-16 01:41:34.000000 connpy-3.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-16 01:41:45.301464 connpy-3.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-04-16 01:41:34.000000 connpy-3.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 01:41:45.301464 connpy-3.0.6/connpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-04-16 01:41:34.000000 connpy-3.0.6/connpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-16 01:41:34.000000 connpy-3.0.6/connpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-16 01:41:34.000000 connpy-3.0.6/connpy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-04-16 01:41:34.000000 connpy-3.0.6/connpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-04-16 01:41:34.000000 connpy-3.0.6/connpy/completion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11869 2023-04-16 01:41:34.000000 connpy-3.0.6/connpy/configfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47695 2023-04-16 01:41:34.000000 connpy-3.0.6/connpy/connapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27894 2023-04-16 01:41:34.000000 connpy-3.0.6/connpy/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 01:41:45.301464 connpy-3.0.6/connpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-16 01:41:45.000000 connpy-3.0.6/connpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-16 01:41:45.000000 connpy-3.0.6/connpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 01:41:45.000000 connpy-3.0.6/connpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-16 01:41:45.000000 connpy-3.0.6/connpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-16 01:41:45.000000 connpy-3.0.6/connpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-16 01:41:45.000000 connpy-3.0.6/connpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-16 01:41:45.301464 connpy-3.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-16 01:41:34.000000 connpy-3.0.6/setup.py
```

### Comparing `connpy-3.0.5/LICENSE` & `connpy-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `connpy-3.0.5/PKG-INFO` & `connpy-3.0.6/connpy/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,80 +1,177 @@
-Metadata-Version: 2.1
-Name: connpy
-Version: 3.0.5
-Summary: Connpy is a SSH/Telnet connection manager and automation module
-Home-page: https://github.com/fluzzi/connpy
-Author: Federico Luzzi
-Author-email: fluzzi@gmail.com
-License: MIT License
-Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
-Project-URL: Documentation, https://fluzzi.github.io/connpy/
-Keywords: networking,automation,ssh,telnet,connection manager
-Classifier: Development Status :: 4 - Beta
-Classifier: Topic :: System :: Networking
-Classifier: Intended Audience :: Telecommunications Industry
-Classifier: Programming Language :: Python :: 3
-Classifier: Natural Language :: English
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Unix
-Description-Content-Type: text/markdown
-Provides-Extra: fuzzysearch
-License-File: LICENSE
-
-# Conn
-[![](https://img.shields.io/pypi/v/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
-[![](https://img.shields.io/pypi/pyversions/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
-[![](https://img.shields.io/pypi/l/connpy.svg?style=flat-square)](https://github.com/fluzzi/connpy/blob/main/LICENSE)
-[![](https://img.shields.io/pypi/dm/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
+#!/usr/bin/env python3
+'''
+## Connection manager
 
-Connpy is a ssh and telnet connection manager and automation module
+Connpy is a connection manager that allows you to store nodes to connect them fast and password free.
 
-## Installation
+### Features
+    - You can generate profiles and reference them from nodes using @profilename 
+      so you dont need to edit multiple nodes when changing password or other 
+      information.
+    - Nodes can be stored on @folder or @subfolder@folder to organize your 
+      devices. Then can be referenced using node@subfolder@folder or node@folder
+    - If you have too many nodes. Get completion script using: conn config 
+      --completion, or use fzf installing pyfzf and running conn config --fzf true
+    - Much more!
+
+### Usage
+```
+usage: conn [-h] [--add | --del | --mod | --show | --debug] [node|folder]
+       conn {profile,move,mv,copy,cp,list,ls,bulk,config} ...
+
+positional arguments:
+  node|folder    node[@subfolder][@folder]
+                 Connect to specific node or show all matching nodes
+                 [@subfolder][@folder]
+                 Show all available connections globaly or in specified path
+Options:
+  -h, --help         show this help message and exit
+  -v, --version      Show version
+  -a, --add          Add new node[@subfolder][@folder] or [@subfolder]@folder
+  -r, --del, --rm    Delete node[@subfolder][@folder] or [@subfolder]@folder
+  -e, --mod, --edit  Modify node[@subfolder][@folder]
+  -s, --show         Show node[@subfolder][@folder]
+  -d, --debug        Display all conections steps
+
+Commands:
+  profile        Manage profiles
+  move (mv)      Move node
+  copy (cp)      Copy node
+  list (ls)      List profiles, nodes or folders
+  bulk           Add nodes in bulk
+  run            Run scripts or commands on nodes
+  config         Manage app config
+  api            Start and stop connpy api
+```
+
+###   Manage profiles
+```
+usage: conn profile [-h] (--add | --del | --mod | --show) profile
+
+positional arguments:
+  profile        Name of profile to manage
+
+options:
+  -h, --help         show this help message and exit
+  -a, --add          Add new profile
+  -r, --del, --rm    Delete profile
+  -e, --mod, --edit  Modify profile
+  -s, --show         Show profile
+
+```
+
+###   Examples
+```
+   conn profile --add office-user
+   conn --add @office
+   conn --add @datacenter@office
+   conn --add server@datacenter@office
+   conn --add pc@office
+   conn --show server@datacenter@office
+   conn pc@office
+   conn server
+``` 
+## http API
+With the Connpy API you can run commands on devices using http requests
+
+### 1. List Nodes
+
+**Endpoint**: `/list_nodes`
+
+**Method**: `POST`
+
+**Description**: This route returns a list of nodes. It can also filter the list based on a given keyword.
+
+#### Request Body:
+
+```json
+{
+  "filter": "<keyword>"
+}
+```
+
+* `filter` (optional): A keyword to filter the list of nodes. It returns only the nodes that contain the keyword. If not provided, the route will return the entire list of nodes.
+
+#### Response:
+
+- A JSON array containing the filtered list of nodes.
+
+---
+
+### 2. Run Commands
+
+**Endpoint**: `/run_commands`
 
-pip install connpy
+**Method**: `POST`
+
+**Description**: This route runs commands on selected nodes based on the provided action, nodes, and commands. It also supports executing tests by providing expected results.
+
+#### Request Body:
+
+```json
+{
+  "action": "<action>",
+  "nodes": "<nodes>",
+  "commands": "<commands>",
+  "expected": "<expected>",
+  "options": "<options>"
+}
+```
+
+* `action` (required): The action to be performed. Possible values: `run` or `test`.
+* `nodes` (required): A list of nodes or a single node on which the commands will be executed. The nodes can be specified as individual node names or a node group with the `@` prefix. Node groups can also be specified as arrays with a list of nodes inside the group.
+* `commands` (required): A list of commands to be executed on the specified nodes.
+* `expected` (optional, only used when the action is `test`): A single expected result for the test.
+* `options` (optional): Array to pass options to the run command, options are: `prompt`, `parallel`, `timeout`  
+
+#### Response:
+
+- A JSON object with the results of the executed commands on the nodes.
+## Automation module
+the automation module
 
-## Automation module usage
 ### Standalone module
 ```
 import connpy
-router = connpy.node("unique name","ip/hostname", user="username", password="password")
+router = connpy.node("unique name","ip/hostname", user="user", password="pass")
 router.run(["term len 0","show run"])
 print(router.output)
 hasip = router.test("show ip int brief","1.1.1.1")
 if hasip:
     print("Router has ip 1.1.1.1")
 else:
     print("router does not have ip 1.1.1.1")
 ```
 
 ### Using manager configuration
 ```
 import connpy
 conf = connpy.configfile()
-device = conf.getitem("router@office")
-router = connpy.node("unique name", **device, config=conf)
-result = router.run("show ip int brief")
+device = conf.getitem("server@office")
+server = connpy.node("unique name", **device, config=conf)
+result = server.run(["cd /", "ls -la"])
 print(result)
 ```
-### Running parallel tasks on multiple devices 
+### Running parallel tasks 
 ```
 import connpy
 conf = connpy.configfile()
 #You can get the nodes from the config from a folder and fitlering in it
 nodes = conf.getitem("@office", ["router1", "router2", "router3"])
 #You can also get each node individually:
 nodes = {}
 nodes["router1"] = conf.getitem("router1@office")
 nodes["router2"] = conf.getitem("router2@office")
 nodes["router10"] = conf.getitem("router10@datacenter")
 #Also, you can create the nodes manually:
 nodes = {}
-nodes["router1"] = {"host": "1.1.1.1", "user": "username", "password": "password1"}
-nodes["router2"] = {"host": "1.1.1.2", "user": "username", "password": "password2"}
-nodes["router3"] = {"host": "1.1.1.2", "user": "username", "password": "password3"}
+nodes["router1"] = {"host": "1.1.1.1", "user": "username", "password": "pass1"}
+nodes["router2"] = {"host": "1.1.1.2", "user": "username", "password": "pass2"}
+nodes["router3"] = {"host": "1.1.1.2", "user": "username", "password": "pass3"}
 #Finally you run some tasks on the nodes
 mynodes = connpy.nodes(nodes, config = conf)
 result = mynodes.test(["show ip int br"], "1.1.1.2")
 for i in result:
     print("---" + i + "---")
     print(result[i])
     print()
@@ -100,79 +197,21 @@
 expected = "!"
 routers = connpy.nodes(nodes, config = config)
 routers.run(commands, variables)
 routers.test("ping {ip}", expected, variables)
 for key in routers.result:
     print(key, ' ---> ', ("pass" if routers.result[key] else "fail"))
 ```
-
-## Connection manager 
-### Features
-    - You can generate profiles and reference them from nodes using @profilename so you dont
-      need to edit multiple nodes when changing password or other information.
-    - Nodes can be stored on @folder or @subfolder@folder to organize your devices. Then can 
-      be referenced using node@subfolder@folder or node@folder
-    - If you have too many nodes. Get completion script using: conn config --completion.
-      Or use fzf installing pyfzf and running conn config --fzf true
-    - Much more!
-
-### Usage:
-```
-usage: conn [-h] [--add | --del | --mod | --show | --debug] [node|folder]
-       conn {profile,move,mv,copy,cp,list,ls,bulk,config} ...
-
-positional arguments:
-  node|folder    node[@subfolder][@folder]
-                 Connect to specific node or show all matching nodes
-                 [@subfolder][@folder]
-                 Show all available connections globaly or in specified path
-```
-
-### Options:
-```
-  -h, --help         show this help message and exit
-  -v, --version      Show version
-  -a, --add          Add new node[@subfolder][@folder] or [@subfolder]@folder
-  -r, --del, --rm    Delete node[@subfolder][@folder] or [@subfolder]@folder
-  -e, --mod, --edit  Modify node[@subfolder][@folder]
-  -s, --show         Show node[@subfolder][@folder]
-  -d, --debug        Display all conections steps
-```
-
-### Commands:
-```
-  profile        Manage profiles
-  move (mv)      Move node
-  copy (cp)      Copy node
-  list (ls)      List profiles, nodes or folders
-  bulk           Add nodes in bulk
-  run            Run scripts or commands on nodes
-  config         Manage app config
-```
-
-### Manage profiles:
-```
-usage: conn profile [-h] (--add | --del | --mod | --show) profile
-
-positional arguments:
-  profile        Name of profile to manage
-
-options:
-  -h, --help         show this help message and exit
-  -a, --add          Add new profile
-  -r, --del, --rm    Delete profile
-  -e, --mod, --edit  Modify profile
-  -s, --show         Show profile
-
-```
-
-### Examples:
-```
-   conn profile --add office-user
-   conn --add @office
-   conn --add @datacenter@office
-   conn --add server@datacenter@office
-   conn --add pc@office
-   conn --show server@datacenter@office
-   conn pc@office
-   conn server
-``` 
+'''
+from .core import node,nodes
+from .configfile import configfile
+from .connapp import connapp
+from ._version import __version__
+from pkg_resources import get_distribution
+
+__all__ = ["node", "nodes", "configfile", "connapp"]
+__author__ = "Federico Luzzi"
+__pdoc__ = {
+    'core': False,
+    'completion': False,
+    'api': False
+}
```

### Comparing `connpy-3.0.5/connpy/__init__.py` & `connpy-3.0.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,138 @@
-#!/usr/bin/env python3
-'''
-## Connection manager
+# Conn
+[![](https://img.shields.io/pypi/v/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
+[![](https://img.shields.io/pypi/pyversions/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
+[![](https://img.shields.io/pypi/l/connpy.svg?style=flat-square)](https://github.com/fluzzi/connpy/blob/main/LICENSE)
+[![](https://img.shields.io/pypi/dm/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
 
-Connpy is a connection manager that allows you to store nodes to connect them fast and password free.
+Connpy is a ssh and telnet connection manager and automation module
 
+## Installation
+
+pip install connpy
+
+## Automation module usage
+### Standalone module
+```
+import connpy
+router = connpy.node("unique name","ip/hostname", user="username", password="password")
+router.run(["term len 0","show run"])
+print(router.output)
+hasip = router.test("show ip int brief","1.1.1.1")
+if hasip:
+    print("Router has ip 1.1.1.1")
+else:
+    print("router does not have ip 1.1.1.1")
+```
+
+### Using manager configuration
+```
+import connpy
+conf = connpy.configfile()
+device = conf.getitem("router@office")
+router = connpy.node("unique name", **device, config=conf)
+result = router.run("show ip int brief")
+print(result)
+```
+### Running parallel tasks on multiple devices 
+```
+import connpy
+conf = connpy.configfile()
+#You can get the nodes from the config from a folder and fitlering in it
+nodes = conf.getitem("@office", ["router1", "router2", "router3"])
+#You can also get each node individually:
+nodes = {}
+nodes["router1"] = conf.getitem("router1@office")
+nodes["router2"] = conf.getitem("router2@office")
+nodes["router10"] = conf.getitem("router10@datacenter")
+#Also, you can create the nodes manually:
+nodes = {}
+nodes["router1"] = {"host": "1.1.1.1", "user": "username", "password": "password1"}
+nodes["router2"] = {"host": "1.1.1.2", "user": "username", "password": "password2"}
+nodes["router3"] = {"host": "1.1.1.2", "user": "username", "password": "password3"}
+#Finally you run some tasks on the nodes
+mynodes = connpy.nodes(nodes, config = conf)
+result = mynodes.test(["show ip int br"], "1.1.1.2")
+for i in result:
+    print("---" + i + "---")
+    print(result[i])
+    print()
+# Or for one specific node
+mynodes.router1.run(["term len 0". "show run"], folder = "/home/user/logs")
+```
+### Using variables
+```
+import connpy
+config = connpy.configfile()
+nodes = config.getitem("@office", ["router1", "router2", "router3"])
+commands = []
+commands.append("config t")
+commands.append("interface lo {id}")
+commands.append("ip add {ip} {mask}")
+commands.append("end")
+variables = {}
+variables["router1@office"] = {"ip": "10.57.57.1"}
+variables["router2@office"] = {"ip": "10.57.57.2"}
+variables["router3@office"] = {"ip": "10.57.57.3"}
+variables["__global__"] = {"id": "57"}
+variables["__global__"]["mask"] =  "255.255.255.255"
+expected = "!"
+routers = connpy.nodes(nodes, config = config)
+routers.run(commands, variables)
+routers.test("ping {ip}", expected, variables)
+for key in routers.result:
+    print(key, ' ---> ', ("pass" if routers.result[key] else "fail"))
+```
+
+## Connection manager 
 ### Features
-    - You can generate profiles and reference them from nodes using @profilename 
-      so you dont need to edit multiple nodes when changing password or other 
-      information.
-    - Nodes can be stored on @folder or @subfolder@folder to organize your 
-      devices. Then can be referenced using node@subfolder@folder or node@folder
-    - If you have too many nodes. Get completion script using: conn config 
-      --completion, or use fzf installing pyfzf and running conn config --fzf true
+    - You can generate profiles and reference them from nodes using @profilename so you dont
+      need to edit multiple nodes when changing password or other information.
+    - Nodes can be stored on @folder or @subfolder@folder to organize your devices. Then can 
+      be referenced using node@subfolder@folder or node@folder
+    - If you have too many nodes. Get completion script using: conn config --completion.
+      Or use fzf installing pyfzf and running conn config --fzf true
     - Much more!
 
-### Usage
+### Usage:
 ```
 usage: conn [-h] [--add | --del | --mod | --show | --debug] [node|folder]
        conn {profile,move,mv,copy,cp,list,ls,bulk,config} ...
 
 positional arguments:
   node|folder    node[@subfolder][@folder]
                  Connect to specific node or show all matching nodes
                  [@subfolder][@folder]
                  Show all available connections globaly or in specified path
-Options:
+```
+
+### Options:
+```
   -h, --help         show this help message and exit
   -v, --version      Show version
   -a, --add          Add new node[@subfolder][@folder] or [@subfolder]@folder
   -r, --del, --rm    Delete node[@subfolder][@folder] or [@subfolder]@folder
   -e, --mod, --edit  Modify node[@subfolder][@folder]
   -s, --show         Show node[@subfolder][@folder]
   -d, --debug        Display all conections steps
+```
 
-Commands:
+### Commands:
+```
   profile        Manage profiles
   move (mv)      Move node
   copy (cp)      Copy node
   list (ls)      List profiles, nodes or folders
   bulk           Add nodes in bulk
   run            Run scripts or commands on nodes
   config         Manage app config
   api            Start and stop connpy api
 ```
 
-###   Manage profiles
+### Manage profiles:
 ```
 usage: conn profile [-h] (--add | --del | --mod | --show) profile
 
 positional arguments:
   profile        Name of profile to manage
 
 options:
@@ -56,15 +140,15 @@
   -a, --add          Add new profile
   -r, --del, --rm    Delete profile
   -e, --mod, --edit  Modify profile
   -s, --show         Show profile
 
 ```
 
-###   Examples
+### Examples:
 ```
    conn profile --add office-user
    conn --add @office
    conn --add @datacenter@office
    conn --add server@datacenter@office
    conn --add pc@office
    conn --show server@datacenter@office
@@ -123,95 +207,7 @@
 * `commands` (required): A list of commands to be executed on the specified nodes.
 * `expected` (optional, only used when the action is `test`): A single expected result for the test.
 * `options` (optional): Array to pass options to the run command, options are: `prompt`, `parallel`, `timeout`  
 
 #### Response:
 
 - A JSON object with the results of the executed commands on the nodes.
-## Automation module
-the automation module
-
-### Standalone module
-```
-import connpy
-router = connpy.node("unique name","ip/hostname", user="user", password="pass")
-router.run(["term len 0","show run"])
-print(router.output)
-hasip = router.test("show ip int brief","1.1.1.1")
-if hasip:
-    print("Router has ip 1.1.1.1")
-else:
-    print("router does not have ip 1.1.1.1")
-```
-
-### Using manager configuration
-```
-import connpy
-conf = connpy.configfile()
-device = conf.getitem("server@office")
-server = connpy.node("unique name", **device, config=conf)
-result = server.run(["cd /", "ls -la"])
-print(result)
-```
-### Running parallel tasks 
-```
-import connpy
-conf = connpy.configfile()
-#You can get the nodes from the config from a folder and fitlering in it
-nodes = conf.getitem("@office", ["router1", "router2", "router3"])
-#You can also get each node individually:
-nodes = {}
-nodes["router1"] = conf.getitem("router1@office")
-nodes["router2"] = conf.getitem("router2@office")
-nodes["router10"] = conf.getitem("router10@datacenter")
-#Also, you can create the nodes manually:
-nodes = {}
-nodes["router1"] = {"host": "1.1.1.1", "user": "username", "password": "pass1"}
-nodes["router2"] = {"host": "1.1.1.2", "user": "username", "password": "pass2"}
-nodes["router3"] = {"host": "1.1.1.2", "user": "username", "password": "pass3"}
-#Finally you run some tasks on the nodes
-mynodes = connpy.nodes(nodes, config = conf)
-result = mynodes.test(["show ip int br"], "1.1.1.2")
-for i in result:
-    print("---" + i + "---")
-    print(result[i])
-    print()
-# Or for one specific node
-mynodes.router1.run(["term len 0". "show run"], folder = "/home/user/logs")
-```
-### Using variables
-```
-import connpy
-config = connpy.configfile()
-nodes = config.getitem("@office", ["router1", "router2", "router3"])
-commands = []
-commands.append("config t")
-commands.append("interface lo {id}")
-commands.append("ip add {ip} {mask}")
-commands.append("end")
-variables = {}
-variables["router1@office"] = {"ip": "10.57.57.1"}
-variables["router2@office"] = {"ip": "10.57.57.2"}
-variables["router3@office"] = {"ip": "10.57.57.3"}
-variables["__global__"] = {"id": "57"}
-variables["__global__"]["mask"] =  "255.255.255.255"
-expected = "!"
-routers = connpy.nodes(nodes, config = config)
-routers.run(commands, variables)
-routers.test("ping {ip}", expected, variables)
-for key in routers.result:
-    print(key, ' ---> ', ("pass" if routers.result[key] else "fail"))
-```
-'''
-from .core import node,nodes
-from .configfile import configfile
-from .connapp import connapp
-from ._version import __version__
-from pkg_resources import get_distribution
-
-__all__ = ["node", "nodes", "configfile", "connapp"]
-__author__ = "Federico Luzzi"
-__pdoc__ = {
-    'core': False,
-    'completion': False,
-    'api': False
-}
```

### Comparing `connpy-3.0.5/connpy/api.py` & `connpy-3.0.6/connpy/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -98,48 +98,54 @@
         return({"DataError": error})
     return output
 
 def stop_api():
     # Read the process ID (pid) from the file
     try:
         with open(PID_FILE1, "r") as f:
-            pid = int(f.read().strip())
+            pid = int(f.readline().strip())
+            port = int(f.readline().strip())
         PID_FILE=PID_FILE1
     except:
         try:
             with open(PID_FILE2, "r") as f:
-                pid = int(f.read().strip())
+                pid = int(f.readline().strip())
+                port = int(f.readline().strip())
             PID_FILE=PID_FILE2
         except:
             print("Connpy api server is not running.")
             return 
     # Send a SIGTERM signal to the process
     os.kill(pid, signal.SIGTERM)
     # Delete the PID file
     os.remove(PID_FILE)
-
     print(f"Server with process ID {pid} stopped.")
+    return port
+
+def debug_api(port=8048):
+    app.custom_config = configfile()
+    app.run(debug=True, port=port)
 
-def start_server():
+def start_server(port=8048):
     app.custom_config = configfile()
-    serve(app, host='0.0.0.0', port=8048)
+    serve(app, host='0.0.0.0', port=port)
 
-def start_api():
+def start_api(port=8048):
     if os.path.exists(PID_FILE1) or os.path.exists(PID_FILE2):
         print("Connpy server is already running.")
         return
     pid = os.fork()
     if pid == 0:
-        start_server()
+        start_server(port)
     else:
         try:
             with open(PID_FILE1, "w") as f:
-                f.write(str(pid))
+                f.write(str(pid) + "\n" + str(port))
         except:
             try:
                 with open(PID_FILE2, "w") as f:
-                    f.write(str(pid))
+                    f.write(str(pid) + "\n" + str(port))
             except:
                 print("Cound't create PID file")
                 return
-        print(f'Server is running with process ID {pid}.')
+        print(f'Server is running with process ID {pid} in port {port}')
```

### Comparing `connpy-3.0.5/connpy/completion.py` & `connpy-3.0.6/connpy/completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     elif wordsnumber == 3:
         strings=[]
         if words[0] == "profile":
             strings=["--add", "--rm", "--del", "--edit", "--mod", "--show", "--help"]
         if words[0] == "config":
             strings=["--allow-uppercase", "--keepalive", "--completion", "--fzf", "--configfolder", "--help"]
         if words[0] == "api":
-            strings=["--start", "--stop", "--restart", "--help"]
+            strings=["--start", "--stop", "--restart", "--debug", "--help"]
         if words[0] in ["--mod", "--edit", "-e", "--show", "-s", "--add", "-a", "--rm", "--del", "-r"]:
             strings=["profile"]
         if words[0] in ["list", "ls"]:
             strings=["profiles", "nodes", "folders"]
         if words[0] in ["bulk", "mv", "cp", "copy", "run"]:
             strings=["--help"]
         if words[0] in ["--rm", "--del", "-r"]:
```

### Comparing `connpy-3.0.5/connpy/configfile.py` & `connpy-3.0.6/connpy/configfile.py`

 * *Files identical despite different names*

### Comparing `connpy-3.0.5/connpy/connapp.py` & `connpy-3.0.6/connpy/connapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,17 +102,18 @@
         runparser = subparsers.add_parser("run", help="Run scripts or commands on nodes", formatter_class=argparse.RawTextHelpFormatter) 
         runparser.add_argument("run", nargs='+', action=self._store_type, help=self._help("run"), default="run")
         runparser.add_argument("-g","--generate", dest="action", action="store_const", help="Generate yaml file template", const="generate", default="run")
         runparser.set_defaults(func=self._func_run)
         #APIPARSER
         apiparser = subparsers.add_parser("api", help="Start and stop connpy api") 
         apicrud = apiparser.add_mutually_exclusive_group(required=True)
-        apicrud.add_argument("--start", dest="start", nargs=0, action=self._store_type, help="Start conppy api")
-        apicrud.add_argument("--restart", dest="restart", nargs=0, action=self._store_type, help="Restart conppy api")
-        apicrud.add_argument("--stop", dest="stop", nargs=0, action=self._store_type, help="Stop conppy api")
+        apicrud.add_argument("-s","--start", dest="start", nargs="?", action=self._store_type, help="Start conppy api", type=int, default=8048, metavar="PORT")
+        apicrud.add_argument("-r","--restart", dest="restart", nargs=0, action=self._store_type, help="Restart conppy api")
+        apicrud.add_argument("-x","--stop", dest="stop", nargs=0, action=self._store_type, help="Stop conppy api")
+        apicrud.add_argument("-d", "--debug", dest="debug", nargs="?", action=self._store_type, help="Run connpy server on debug mode", type=int, default=8048, metavar="PORT")
         apiparser.set_defaults(func=self._func_api)
         #CONFIGPARSER
         configparser = subparsers.add_parser("config", help="Manage app config") 
         configcrud = configparser.add_mutually_exclusive_group(required=True)
         configcrud.add_argument("--allow-uppercase", dest="case", nargs=1, action=self._store_type, help="Allow case sensitive names", choices=["true","false"])
         configcrud.add_argument("--fzf", dest="fzf", nargs=1, action=self._store_type, help="Use fzf for lists", choices=["true","false"])
         configcrud.add_argument("--keepalive", dest="idletime", nargs=1, action=self._store_type, help="Set keepalive time in seconds, 0 to disable", type=int, metavar="INT")
@@ -496,17 +497,25 @@
         if len(args.data) > 1:
             args.action = "noderun"
         actions = {"noderun": self._node_run, "generate": self._yaml_generate, "run": self._yaml_run}
         return actions.get(args.action)(args)
 
     def _func_api(self, args):
         if args.command == "stop" or args.command == "restart":
-            stop_api()
+            args.data = stop_api()
         if args.command == "start" or args.command == "restart":
-            start_api()
+            if args.data:
+                start_api(args.data)
+            else:
+                start_api()
+        if args.command == "debug":
+            if args.data:
+                debug_api(args.data)
+            else:
+                debug_api()
         return
 
     def _node_run(self, args):
         command = " ".join(args.data[1:])
         command = command.split("-")
         matches = list(filter(lambda k: k == args.data[0], self.nodes))
         if len(matches) == 0:
```

### Comparing `connpy-3.0.5/connpy/core.py` & `connpy-3.0.6/connpy/core.py`

 * *Files identical despite different names*

### Comparing `connpy-3.0.5/setup.cfg` & `connpy-3.0.6/setup.cfg`

 * *Files identical despite different names*

