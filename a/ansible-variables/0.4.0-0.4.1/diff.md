# Comparing `tmp/ansible-variables-0.4.0.tar.gz` & `tmp/ansible-variables-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-variables-0.4.0.tar", last modified: Fri Apr 14 14:16:13 2023, max compression
+gzip compressed data, was "ansible-variables-0.4.1.tar", last modified: Sun Apr 16 19:09:22 2023, max compression
```

## Comparing `ansible-variables-0.4.0.tar` & `ansible-variables-0.4.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:13.224984 ansible-variables-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 14:16:00.000000 ansible-variables-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-04-14 14:16:13.224984 ansible-variables-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-14 14:16:00.000000 ansible-variables-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:13.220984 ansible-variables-0.4.0/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:13.224984 ansible-variables-0.4.0/lib/ansible_variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:00.000000 ansible-variables-0.4.0/lib/ansible_variables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:13.224984 ansible-variables-0.4.0/lib/ansible_variables/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:00.000000 ansible-variables-0.4.0/lib/ansible_variables/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-14 14:16:00.000000 ansible-variables-0.4.0/lib/ansible_variables/cli/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:13.224984 ansible-variables-0.4.0/lib/ansible_variables/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:00.000000 ansible-variables-0.4.0/lib/ansible_variables/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-04-14 14:16:00.000000 ansible-variables-0.4.0/lib/ansible_variables/utils/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:13.224984 ansible-variables-0.4.0/lib/ansible_variables.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-04-14 14:16:13.000000 ansible-variables-0.4.0/lib/ansible_variables.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-14 14:16:13.000000 ansible-variables-0.4.0/lib/ansible_variables.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:16:13.000000 ansible-variables-0.4.0/lib/ansible_variables.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-14 14:16:13.000000 ansible-variables-0.4.0/lib/ansible_variables.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:16:13.000000 ansible-variables-0.4.0/lib/ansible_variables.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 14:16:13.000000 ansible-variables-0.4.0/lib/ansible_variables.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 14:16:13.000000 ansible-variables-0.4.0/lib/ansible_variables.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-14 14:16:00.000000 ansible-variables-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-14 14:16:13.224984 ansible-variables-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-14 14:16:00.000000 ansible-variables-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:13.224984 ansible-variables-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-14 14:16:00.000000 ansible-variables-0.4.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-14 14:16:00.000000 ansible-variables-0.4.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-14 14:16:00.000000 ansible-variables-0.4.0/tests/test_variablesource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:09:22.641183 ansible-variables-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 19:09:11.000000 ansible-variables-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-04-16 19:09:22.641183 ansible-variables-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-16 19:09:11.000000 ansible-variables-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:09:22.637183 ansible-variables-0.4.1/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:09:22.641183 ansible-variables-0.4.1/lib/ansible_variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:09:11.000000 ansible-variables-0.4.1/lib/ansible_variables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:09:22.641183 ansible-variables-0.4.1/lib/ansible_variables/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:09:11.000000 ansible-variables-0.4.1/lib/ansible_variables/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-16 19:09:11.000000 ansible-variables-0.4.1/lib/ansible_variables/cli/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:09:22.641183 ansible-variables-0.4.1/lib/ansible_variables/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:09:11.000000 ansible-variables-0.4.1/lib/ansible_variables/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-04-16 19:09:11.000000 ansible-variables-0.4.1/lib/ansible_variables/utils/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:09:22.641183 ansible-variables-0.4.1/lib/ansible_variables.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-04-16 19:09:22.000000 ansible-variables-0.4.1/lib/ansible_variables.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-16 19:09:22.000000 ansible-variables-0.4.1/lib/ansible_variables.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 19:09:22.000000 ansible-variables-0.4.1/lib/ansible_variables.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-16 19:09:22.000000 ansible-variables-0.4.1/lib/ansible_variables.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 19:09:22.000000 ansible-variables-0.4.1/lib/ansible_variables.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-16 19:09:22.000000 ansible-variables-0.4.1/lib/ansible_variables.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-16 19:09:22.000000 ansible-variables-0.4.1/lib/ansible_variables.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-16 19:09:11.000000 ansible-variables-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-16 19:09:22.641183 ansible-variables-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-16 19:09:11.000000 ansible-variables-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:09:22.641183 ansible-variables-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-16 19:09:11.000000 ansible-variables-0.4.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-16 19:09:11.000000 ansible-variables-0.4.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-16 19:09:11.000000 ansible-variables-0.4.1/tests/test_variablesource.py
```

### Comparing `ansible-variables-0.4.0/LICENSE` & `ansible-variables-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.4.0/PKG-INFO` & `ansible-variables-0.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-variables
-Version: 0.4.0
+Version: 0.4.1
 Summary: Keep track of Ansible host context variables
 Home-page: https://github.com/hille721/ansible-variables
 Author: Christoph Hille
 Author-email: hille721@gmail.com
 License: GPLv3+
 Project-URL: Bug Tracker, https://github.com/hille721/ansible-variables/issues
 Project-URL: Documentation, https://github.com/hille721/ansible-variables/blob/main/README.md
@@ -25,40 +25,41 @@
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![PyPI version](https://badge.fury.io/py/ansible-variables.svg)](https://badge.fury.io/py/ansible-variables)
-
 # ansible-variables
 
+[![PyPI version][pypi-version]][pypi-link]
+[![PyPI platforms][pypi-platforms]][pypi-link]
+
 The Ansible inventory provides a very powerful framework to declare variables in a hierarchical manner.
-There a lof of differnt places where a variable can be definied (inventory, host_vars, groups_vars, ...) and Ansible will merge them in a specific order ([variable precedence](https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_variables.html#understanding-variable-precedence)).
+There a lof of different places where a variable can be defined (inventory, host_vars, groups_vars, ...) and Ansible will merge them in a specific order ([variable precedence](https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_variables.html#understanding-variable-precedence)).
 
 `ansible-variables` will help to keep track of your host context variables:
 
 * inventory file or script group vars
 * inventory group_vars/all
 * inventory group_vars/*
 * inventory file or script host vars
 * inventory host_vars/*
 
-Based on one host it will retun a list with all variables, values and variable type.
+Based on one host it will return a list with all variables, values and variable type.
 
 ## Installation
 
 ```bash
 pip install ansible-variables
 ```
 
 ## Usage
 
-The command line usage is simmilar to the official Ansible CLI tools, especially like ansible-inventory, thus to see all possible commands and options run
+The command line usage is similar to the official Ansible CLI tools, especially like ansible-inventory, thus to see all possible commands and options run
 
 ```plain
 ansible-variables --help
 ```
 
 ### Get all variables for a host
 
@@ -67,16 +68,15 @@
 ```plain
 ansible-variables mywebserver
 ```
 
 This results in following simple rich formatted output
 ![command_simple](https://github.com/hille721/ansible-variables/raw/main/docs/img/command_simple.png)
 
-
-The vervosity can be increased Ansible like with `-v`, `-vvv`, ...
+The verbosity can be increased Ansible like with `-v`, `-vvv`, ...
 
 With `-v` the inventory files where the variable is defined, will be printed. The last file wins.
 
 ![command_simple_verbose](https://github.com/hille721/ansible-variables/raw/main/docs/img/command_simple_verbose.png)
 
 With `-vvv` it will also print all files which were considered to look for the variable.
 
@@ -88,35 +88,37 @@
 ansible-variables mywebserver --var foo
 ```
 
 Same es above, the verbosity can also increase here.
 
 ### More customization
 
-With `--help` you will see which furhter arguments are possible, e.g. you can set the path to your inventory with `-i`
+With `--help` you will see which further arguments are possible, e.g. you can set the path to your inventory with `-i`
 
 ```plain
 ansible-variables mywebserver -i /path/to/inventory
 ```
 
 ## Implementation
 
 This tool is tightly coupled to the Ansible library (`ansible-core`) and simple reuses what is already there.
-The whole structure and implemntation was inspired and oriented by the implementation of [`ansible-inventory`](https://github.com/ansible/ansible/blob/devel/lib/ansible/cli/inventory.py).
+The whole structure and implementation was inspired and oriented by the implementation of [`ansible-inventory`](https://github.com/ansible/ansible/blob/devel/lib/ansible/cli/inventory.py).
 
 To get the source and the inventory files in which Ansible will look for a variable, we are using a [debug flag](https://github.com/ansible/ansible/blob/devel/lib/ansible/vars/manager.py#L187) in Ansible's `get_vars` method.
 
 As as result, the output of `ansible-variables` can be fully trusted as it uses the same methods as Ansible to get the variable precedence.
 
 ## Limitations
 
-* as written in the description, this tool shows only host context varialbe and there does not know anything about playbook or role variables or command line options.
+* as written in the description, this tool only shows host context variables and does not know anything about playbook or role variables or command line options.
 
 ## Credits
 
-I would like to thank the termshot project for their excellent tool that allowed me to easily create the screenshots used in this README.md file.
-
-If you're interested in learning more about the termshot project, you can visit their website at <https://termshot.app/> or check out their GitHub repository at <https://github.com/nickolasburr/termshot>.
+* the screenshots used  in this README where created with [termshot](https://github.com/homeport/termshot)
 
 ## License
 
 This project is licensed under the [GNU General Public License v3.0](https://github.com/hille721/ansible-variables/blob/main/LICENSE)
+
+[pypi-link]:                https://pypi.org/project/ansible-variables/
+[pypi-platforms]:           https://img.shields.io/pypi/pyversions/ansible-variables
+[pypi-version]:             https://badge.fury.io/py/ansible-variables.svg
```

### Comparing `ansible-variables-0.4.0/README.md` & `ansible-variables-0.4.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-[![PyPI version](https://badge.fury.io/py/ansible-variables.svg)](https://badge.fury.io/py/ansible-variables)
-
 # ansible-variables
 
+[![PyPI version][pypi-version]][pypi-link]
+[![PyPI platforms][pypi-platforms]][pypi-link]
+
 The Ansible inventory provides a very powerful framework to declare variables in a hierarchical manner.
-There a lof of differnt places where a variable can be definied (inventory, host_vars, groups_vars, ...) and Ansible will merge them in a specific order ([variable precedence](https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_variables.html#understanding-variable-precedence)).
+There a lof of different places where a variable can be defined (inventory, host_vars, groups_vars, ...) and Ansible will merge them in a specific order ([variable precedence](https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_variables.html#understanding-variable-precedence)).
 
 `ansible-variables` will help to keep track of your host context variables:
 
 * inventory file or script group vars
 * inventory group_vars/all
 * inventory group_vars/*
 * inventory file or script host vars
 * inventory host_vars/*
 
-Based on one host it will retun a list with all variables, values and variable type.
+Based on one host it will return a list with all variables, values and variable type.
 
 ## Installation
 
 ```bash
 pip install ansible-variables
 ```
 
 ## Usage
 
-The command line usage is simmilar to the official Ansible CLI tools, especially like ansible-inventory, thus to see all possible commands and options run
+The command line usage is similar to the official Ansible CLI tools, especially like ansible-inventory, thus to see all possible commands and options run
 
 ```plain
 ansible-variables --help
 ```
 
 ### Get all variables for a host
 
@@ -36,16 +37,15 @@
 ```plain
 ansible-variables mywebserver
 ```
 
 This results in following simple rich formatted output
 ![command_simple](https://github.com/hille721/ansible-variables/raw/main/docs/img/command_simple.png)
 
-
-The vervosity can be increased Ansible like with `-v`, `-vvv`, ...
+The verbosity can be increased Ansible like with `-v`, `-vvv`, ...
 
 With `-v` the inventory files where the variable is defined, will be printed. The last file wins.
 
 ![command_simple_verbose](https://github.com/hille721/ansible-variables/raw/main/docs/img/command_simple_verbose.png)
 
 With `-vvv` it will also print all files which were considered to look for the variable.
 
@@ -57,35 +57,37 @@
 ansible-variables mywebserver --var foo
 ```
 
 Same es above, the verbosity can also increase here.
 
 ### More customization
 
-With `--help` you will see which furhter arguments are possible, e.g. you can set the path to your inventory with `-i`
+With `--help` you will see which further arguments are possible, e.g. you can set the path to your inventory with `-i`
 
 ```plain
 ansible-variables mywebserver -i /path/to/inventory
 ```
 
 ## Implementation
 
 This tool is tightly coupled to the Ansible library (`ansible-core`) and simple reuses what is already there.
-The whole structure and implemntation was inspired and oriented by the implementation of [`ansible-inventory`](https://github.com/ansible/ansible/blob/devel/lib/ansible/cli/inventory.py).
+The whole structure and implementation was inspired and oriented by the implementation of [`ansible-inventory`](https://github.com/ansible/ansible/blob/devel/lib/ansible/cli/inventory.py).
 
 To get the source and the inventory files in which Ansible will look for a variable, we are using a [debug flag](https://github.com/ansible/ansible/blob/devel/lib/ansible/vars/manager.py#L187) in Ansible's `get_vars` method.
 
 As as result, the output of `ansible-variables` can be fully trusted as it uses the same methods as Ansible to get the variable precedence.
 
 ## Limitations
 
-* as written in the description, this tool shows only host context varialbe and there does not know anything about playbook or role variables or command line options.
+* as written in the description, this tool only shows host context variables and does not know anything about playbook or role variables or command line options.
 
 ## Credits
 
-I would like to thank the termshot project for their excellent tool that allowed me to easily create the screenshots used in this README.md file.
-
-If you're interested in learning more about the termshot project, you can visit their website at <https://termshot.app/> or check out their GitHub repository at <https://github.com/nickolasburr/termshot>.
+* the screenshots used  in this README where created with [termshot](https://github.com/homeport/termshot)
 
 ## License
 
 This project is licensed under the [GNU General Public License v3.0](https://github.com/hille721/ansible-variables/blob/main/LICENSE)
+
+[pypi-link]:                https://pypi.org/project/ansible-variables/
+[pypi-platforms]:           https://img.shields.io/pypi/pyversions/ansible-variables
+[pypi-version]:             https://badge.fury.io/py/ansible-variables.svg
```

### Comparing `ansible-variables-0.4.0/lib/ansible_variables/cli/variables.py` & `ansible-variables-0.4.1/lib/ansible_variables/cli/variables.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         "omit",
         "playbook_dir",
     ]
 )
 
 
 class VariablesCLI(CLI):
-    """used to display from where a variable value is comming from"""
+    """used to display from where a variable value is coming from"""
 
     name = "ansible-variables"
 
     def __init__(self, args):
         super().__init__(args)
         self.loader = None
         self.inventory = None
```

### Comparing `ansible-variables-0.4.0/lib/ansible_variables/utils/vars.py` & `ansible-variables-0.4.1/lib/ansible_variables/utils/vars.py`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.4.0/lib/ansible_variables.egg-info/PKG-INFO` & `ansible-variables-0.4.1/lib/ansible_variables.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-variables
-Version: 0.4.0
+Version: 0.4.1
 Summary: Keep track of Ansible host context variables
 Home-page: https://github.com/hille721/ansible-variables
 Author: Christoph Hille
 Author-email: hille721@gmail.com
 License: GPLv3+
 Project-URL: Bug Tracker, https://github.com/hille721/ansible-variables/issues
 Project-URL: Documentation, https://github.com/hille721/ansible-variables/blob/main/README.md
@@ -25,40 +25,41 @@
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![PyPI version](https://badge.fury.io/py/ansible-variables.svg)](https://badge.fury.io/py/ansible-variables)
-
 # ansible-variables
 
+[![PyPI version][pypi-version]][pypi-link]
+[![PyPI platforms][pypi-platforms]][pypi-link]
+
 The Ansible inventory provides a very powerful framework to declare variables in a hierarchical manner.
-There a lof of differnt places where a variable can be definied (inventory, host_vars, groups_vars, ...) and Ansible will merge them in a specific order ([variable precedence](https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_variables.html#understanding-variable-precedence)).
+There a lof of different places where a variable can be defined (inventory, host_vars, groups_vars, ...) and Ansible will merge them in a specific order ([variable precedence](https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_variables.html#understanding-variable-precedence)).
 
 `ansible-variables` will help to keep track of your host context variables:
 
 * inventory file or script group vars
 * inventory group_vars/all
 * inventory group_vars/*
 * inventory file or script host vars
 * inventory host_vars/*
 
-Based on one host it will retun a list with all variables, values and variable type.
+Based on one host it will return a list with all variables, values and variable type.
 
 ## Installation
 
 ```bash
 pip install ansible-variables
 ```
 
 ## Usage
 
-The command line usage is simmilar to the official Ansible CLI tools, especially like ansible-inventory, thus to see all possible commands and options run
+The command line usage is similar to the official Ansible CLI tools, especially like ansible-inventory, thus to see all possible commands and options run
 
 ```plain
 ansible-variables --help
 ```
 
 ### Get all variables for a host
 
@@ -67,16 +68,15 @@
 ```plain
 ansible-variables mywebserver
 ```
 
 This results in following simple rich formatted output
 ![command_simple](https://github.com/hille721/ansible-variables/raw/main/docs/img/command_simple.png)
 
-
-The vervosity can be increased Ansible like with `-v`, `-vvv`, ...
+The verbosity can be increased Ansible like with `-v`, `-vvv`, ...
 
 With `-v` the inventory files where the variable is defined, will be printed. The last file wins.
 
 ![command_simple_verbose](https://github.com/hille721/ansible-variables/raw/main/docs/img/command_simple_verbose.png)
 
 With `-vvv` it will also print all files which were considered to look for the variable.
 
@@ -88,35 +88,37 @@
 ansible-variables mywebserver --var foo
 ```
 
 Same es above, the verbosity can also increase here.
 
 ### More customization
 
-With `--help` you will see which furhter arguments are possible, e.g. you can set the path to your inventory with `-i`
+With `--help` you will see which further arguments are possible, e.g. you can set the path to your inventory with `-i`
 
 ```plain
 ansible-variables mywebserver -i /path/to/inventory
 ```
 
 ## Implementation
 
 This tool is tightly coupled to the Ansible library (`ansible-core`) and simple reuses what is already there.
-The whole structure and implemntation was inspired and oriented by the implementation of [`ansible-inventory`](https://github.com/ansible/ansible/blob/devel/lib/ansible/cli/inventory.py).
+The whole structure and implementation was inspired and oriented by the implementation of [`ansible-inventory`](https://github.com/ansible/ansible/blob/devel/lib/ansible/cli/inventory.py).
 
 To get the source and the inventory files in which Ansible will look for a variable, we are using a [debug flag](https://github.com/ansible/ansible/blob/devel/lib/ansible/vars/manager.py#L187) in Ansible's `get_vars` method.
 
 As as result, the output of `ansible-variables` can be fully trusted as it uses the same methods as Ansible to get the variable precedence.
 
 ## Limitations
 
-* as written in the description, this tool shows only host context varialbe and there does not know anything about playbook or role variables or command line options.
+* as written in the description, this tool only shows host context variables and does not know anything about playbook or role variables or command line options.
 
 ## Credits
 
-I would like to thank the termshot project for their excellent tool that allowed me to easily create the screenshots used in this README.md file.
-
-If you're interested in learning more about the termshot project, you can visit their website at <https://termshot.app/> or check out their GitHub repository at <https://github.com/nickolasburr/termshot>.
+* the screenshots used  in this README where created with [termshot](https://github.com/homeport/termshot)
 
 ## License
 
 This project is licensed under the [GNU General Public License v3.0](https://github.com/hille721/ansible-variables/blob/main/LICENSE)
+
+[pypi-link]:                https://pypi.org/project/ansible-variables/
+[pypi-platforms]:           https://img.shields.io/pypi/pyversions/ansible-variables
+[pypi-version]:             https://badge.fury.io/py/ansible-variables.svg
```

### Comparing `ansible-variables-0.4.0/lib/ansible_variables.egg-info/SOURCES.txt` & `ansible-variables-0.4.1/lib/ansible_variables.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.4.0/setup.cfg` & `ansible-variables-0.4.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ansible-variables
-version = 0.4.0
+version = 0.4.1
 description = Keep track of Ansible host context variables
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Christoph Hille
 author_email = hille721@gmail.com
 url = https://github.com/hille721/ansible-variables
 project_urls =
```

### Comparing `ansible-variables-0.4.0/tests/test_cli.py` & `ansible-variables-0.4.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.4.0/tests/test_utils.py` & `ansible-variables-0.4.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.4.0/tests/test_variablesource.py` & `ansible-variables-0.4.1/tests/test_variablesource.py`

 * *Files identical despite different names*

