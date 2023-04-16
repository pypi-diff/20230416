# Comparing `tmp/oai_tools-0.1.1.tar.gz` & `tmp/oai_tools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oai_tools-0.1.1.tar", last modified: Fri Apr 14 18:05:42 2023, max compression
+gzip compressed data, was "oai_tools-0.1.2.tar", last modified: Sun Apr 16 06:42:43 2023, max compression
```

## Comparing `oai_tools-0.1.1.tar` & `oai_tools-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:42.607755 oai_tools-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-14 18:05:33.000000 oai_tools-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-14 18:05:42.603754 oai_tools-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-14 18:05:33.000000 oai_tools-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:42.603754 oai_tools-0.1.1/oai_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-14 18:05:33.000000 oai_tools-0.1.1/oai_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-04-14 18:05:33.000000 oai_tools-0.1.1/oai_tools/cligpt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:42.603754 oai_tools-0.1.1/oai_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-14 18:05:42.000000 oai_tools-0.1.1/oai_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-14 18:05:42.000000 oai_tools-0.1.1/oai_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:05:42.000000 oai_tools-0.1.1/oai_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-14 18:05:42.000000 oai_tools-0.1.1/oai_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-14 18:05:42.000000 oai_tools-0.1.1/oai_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 18:05:42.000000 oai_tools-0.1.1/oai_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-14 18:05:33.000000 oai_tools-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:05:42.607755 oai_tools-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-14 18:05:33.000000 oai_tools-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:42:43.434271 oai_tools-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-16 06:42:29.000000 oai_tools-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-16 06:42:43.434271 oai_tools-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-16 06:42:29.000000 oai_tools-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:42:43.434271 oai_tools-0.1.2/oai_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-16 06:42:29.000000 oai_tools-0.1.2/oai_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-16 06:42:29.000000 oai_tools-0.1.2/oai_tools/cligpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:42:43.434271 oai_tools-0.1.2/oai_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-16 06:42:43.000000 oai_tools-0.1.2/oai_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-16 06:42:43.000000 oai_tools-0.1.2/oai_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 06:42:43.000000 oai_tools-0.1.2/oai_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-16 06:42:43.000000 oai_tools-0.1.2/oai_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-16 06:42:43.000000 oai_tools-0.1.2/oai_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-16 06:42:43.000000 oai_tools-0.1.2/oai_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-16 06:42:29.000000 oai_tools-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 06:42:43.434271 oai_tools-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-16 06:42:29.000000 oai_tools-0.1.2/setup.py
```

### Comparing `oai_tools-0.1.1/LICENSE` & `oai_tools-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oai_tools-0.1.1/PKG-INFO` & `oai_tools-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: oai_tools
-Version: 0.1.1
+Version: 0.1.2
 Summary: Collection of useful tools built on top of OpenAI's API
 Home-page: https://github.com/filipgrano/oai_tools/tree/main
 Author: Filip Granö
 Author-email: filip-accounts@grano.me
 License: UNKNOWN
 Description: # OAI Tools
         
         This repository contains a collection of useful tools built on top of OpenAI's API. These tools can help automate various tasks and provide assistance through natural language processing.
         
-        ## Installation
-        `pip install .`
+        ## Installation or Upgrade
+        `pip install --upgrade oai-tools`
         
         ## Tools
         
         1. **cligpt**: A command-line helper that takes a user prompt and returns shell commands, along with explanations of what they do. See [cligpt.md](doc/cligpt.md) for more details.
         
         ## Configuration
         Configuration file is read from `~/.config/oai_tools/config.yaml` file. See the [config-example.yaml](doc/config-example.yaml) file for more details.
```

### Comparing `oai_tools-0.1.1/README.md` & `oai_tools-0.1.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # OAI Tools
 
 This repository contains a collection of useful tools built on top of OpenAI's API. These tools can help automate various tasks and provide assistance through natural language processing.
 
-## Installation
-`pip install .`
+## Installation or Upgrade
+`pip install --upgrade oai-tools`
 
 ## Tools
 
 1. **cligpt**: A command-line helper that takes a user prompt and returns shell commands, along with explanations of what they do. See [cligpt.md](doc/cligpt.md) for more details.
 
 ## Configuration
 Configuration file is read from `~/.config/oai_tools/config.yaml` file. See the [config-example.yaml](doc/config-example.yaml) file for more details.
```

### Comparing `oai_tools-0.1.1/oai_tools/__init__.py` & `oai_tools-0.1.2/oai_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `oai_tools-0.1.1/oai_tools/cligpt.py` & `oai_tools-0.1.2/oai_tools/cligpt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import logging
 import os
 import platform
-import selectors
-import subprocess
 import sys
 
 import openai
 
 from oai_tools import get_api_key, read_config
 
 openai.api_key = get_api_key()
@@ -14,15 +12,15 @@
 config = read_config()
 cligpt_config = config.get("cligpt", {})
 
 LOG_LEVEL = cligpt_config.get("loglevel", "INFO")
 logging.basicConfig(level=logging.getLevelName(LOG_LEVEL))
 
 MODEL = cligpt_config.get("model", "gpt-3.5-turbo")
-AUTO_EXPLAIN = cligpt_config.get("auto_explain", True)
+AUTO_EXPLAIN = cligpt_config.get("auto_explain", False)
 MAX_TOKENS_COMMAND = cligpt_config.get("max_tokens", {}).get("command", 100)
 MAX_TOKENS_EXPLANATION = cligpt_config.get("max_tokens", {}).get("explanation", 100)
 TEMPERATURE_COMMAND = cligpt_config.get("temperature", {}).get("command", 0.9)
 TEMPERATURE_EXPLANATION = cligpt_config.get("temperature", {}).get("explanation", 0.9)
 
 
 def get_shell() -> str:
@@ -75,53 +73,19 @@
 
 
 def execute_command(command: str) -> None:
     """Execute a shell command and print its output and errors as they are produced."""
     shell = get_shell()
     logging.debug("Executing shell command in shell %s: %s", shell, command)
 
-    with subprocess.Popen(
-        command,
-        shell=True,
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
-        text=True,
-        bufsize=1,
-        executable=shell,
-    ) as process:
-        selector = selectors.DefaultSelector()
-        if process.stdout:
-            selector.register(process.stdout, selectors.EVENT_READ)
-        if process.stderr:
-            selector.register(process.stderr, selectors.EVENT_READ)
-
-        while process.poll() is None:
-            for key, _ in selector.select():
-                line = None
-                if key.fileobj is process.stdout and process.stdout:
-                    line = process.stdout.readline()
-                elif key.fileobj is process.stderr and process.stderr:
-                    line = process.stderr.readline()
-
-                if line is not None:
-                    if key.fileobj is process.stdout:
-                        print(line, end="")
-                    elif key.fileobj is process.stderr:
-                        print(line, end="", file=sys.stderr)
-
-        return_code = process.returncode
-        logging.debug("Shell command results -- return code: %s", return_code)
-
-        # Clean up
-        if process.stdout:
-            selector.unregister(process.stdout)
-            process.stdout.close()
-        if process.stderr:
-            selector.unregister(process.stderr)
-            process.stderr.close()
+    command = command.replace('"', r"\"")
+    command = f'{shell} -c "{command}" '
+    return_code = os.system(command)
+
+    logging.debug("Shell command results -- return code: %s", return_code)
 
 
 def main():
     try:
         prompt = " ".join(sys.argv[1:])
         logging.debug("Prompt: %s", prompt)
```

### Comparing `oai_tools-0.1.1/oai_tools.egg-info/PKG-INFO` & `oai_tools-0.1.2/oai_tools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: oai-tools
-Version: 0.1.1
+Version: 0.1.2
 Summary: Collection of useful tools built on top of OpenAI's API
 Home-page: https://github.com/filipgrano/oai_tools/tree/main
 Author: Filip Granö
 Author-email: filip-accounts@grano.me
 License: UNKNOWN
 Description: # OAI Tools
         
         This repository contains a collection of useful tools built on top of OpenAI's API. These tools can help automate various tasks and provide assistance through natural language processing.
         
-        ## Installation
-        `pip install .`
+        ## Installation or Upgrade
+        `pip install --upgrade oai-tools`
         
         ## Tools
         
         1. **cligpt**: A command-line helper that takes a user prompt and returns shell commands, along with explanations of what they do. See [cligpt.md](doc/cligpt.md) for more details.
         
         ## Configuration
         Configuration file is read from `~/.config/oai_tools/config.yaml` file. See the [config-example.yaml](doc/config-example.yaml) file for more details.
```

### Comparing `oai_tools-0.1.1/pyproject.toml` & `oai_tools-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oai_tools-0.1.1/setup.py` & `oai_tools-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="oai_tools",
-    version="0.1.1",
+    version="0.1.2",
     author="Filip Granö",
     author_email="filip-accounts@grano.me",
     description="Collection of useful tools built on top of OpenAI's API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/filipgrano/oai_tools/tree/main",
     packages=find_packages(),
```

