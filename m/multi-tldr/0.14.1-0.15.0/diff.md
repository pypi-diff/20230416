# Comparing `tmp/multi-tldr-0.14.1.tar.gz` & `tmp/multi-tldr-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/multi-tldr-0.14.1.tar", last modified: Wed Oct 21 22:39:50 2020, max compression
+gzip compressed data, was "multi-tldr-0.15.0.tar", last modified: Sun Apr 16 16:14:46 2023, max compression
```

## Comparing `multi-tldr-0.14.1.tar` & `multi-tldr-0.15.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 shen       (501) staff       (20)        0 2020-10-21 22:39:50.508538 multi-tldr-0.14.1/
--rw-r--r--   0 shen       (501) staff       (20)     1099 2020-10-07 21:10:51.000000 multi-tldr-0.14.1/LICENSE
--rw-r--r--   0 shen       (501) staff       (20)       29 2020-10-07 19:16:53.000000 multi-tldr-0.14.1/MANIFEST.in
--rw-r--r--   0 shen       (501) staff       (20)      813 2020-10-21 22:39:50.508685 multi-tldr-0.14.1/PKG-INFO
--rw-r--r--   0 shen       (501) staff       (20)      127 2020-10-09 22:28:51.000000 multi-tldr-0.14.1/Readme.PyPI.md
--rw-r--r--   0 shen       (501) staff       (20)     9715 2020-10-16 13:36:17.000000 multi-tldr-0.14.1/Readme.md
-drwxr-xr-x   0 shen       (501) staff       (20)        0 2020-10-21 22:39:50.508317 multi-tldr-0.14.1/multi_tldr.egg-info/
--rw-r--r--   0 shen       (501) staff       (20)      813 2020-10-21 22:39:50.000000 multi-tldr-0.14.1/multi_tldr.egg-info/PKG-INFO
--rw-r--r--   0 shen       (501) staff       (20)      277 2020-10-21 22:39:50.000000 multi-tldr-0.14.1/multi_tldr.egg-info/SOURCES.txt
--rw-r--r--   0 shen       (501) staff       (20)        1 2020-10-21 22:39:50.000000 multi-tldr-0.14.1/multi_tldr.egg-info/dependency_links.txt
--rw-r--r--   0 shen       (501) staff       (20)       37 2020-10-21 22:39:50.000000 multi-tldr-0.14.1/multi_tldr.egg-info/entry_points.txt
--rw-r--r--   0 shen       (501) staff       (20)       11 2020-10-21 22:39:50.000000 multi-tldr-0.14.1/multi_tldr.egg-info/requires.txt
--rw-r--r--   0 shen       (501) staff       (20)        5 2020-10-21 22:39:50.000000 multi-tldr-0.14.1/multi_tldr.egg-info/top_level.txt
--rw-r--r--   0 shen       (501) staff       (20)      112 2020-10-21 22:39:50.509219 multi-tldr-0.14.1/setup.cfg
--rw-r--r--   0 shen       (501) staff       (20)     1084 2020-10-21 22:27:55.000000 multi-tldr-0.14.1/setup.py
--rwxr-xr-x   0 shen       (501) staff       (20)    18837 2020-10-21 22:29:05.000000 multi-tldr-0.14.1/tldr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:14:46.649850 multi-tldr-0.15.0/
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-04-16 16:14:41.000000 multi-tldr-0.15.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-16 16:14:41.000000 multi-tldr-0.15.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      780 2023-04-16 16:14:46.649850 multi-tldr-0.15.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      127 2023-04-16 16:14:41.000000 multi-tldr-0.15.0/Readme.PyPI.md
+-rw-r--r--   0 root         (0) root         (0)     9636 2023-04-16 16:14:41.000000 multi-tldr-0.15.0/Readme.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:14:46.649850 multi-tldr-0.15.0/multi_tldr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      780 2023-04-16 16:14:46.000000 multi-tldr-0.15.0/multi_tldr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      277 2023-04-16 16:14:46.000000 multi-tldr-0.15.0/multi_tldr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 16:14:46.000000 multi-tldr-0.15.0/multi_tldr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-04-16 16:14:46.000000 multi-tldr-0.15.0/multi_tldr.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-16 16:14:46.000000 multi-tldr-0.15.0/multi_tldr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-16 16:14:46.000000 multi-tldr-0.15.0/multi_tldr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2023-04-16 16:14:46.649850 multi-tldr-0.15.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1083 2023-04-16 16:14:41.000000 multi-tldr-0.15.0/setup.py
+-rwxr-xr-x   0 root         (0) root         (0)    18575 2023-04-16 16:14:41.000000 multi-tldr-0.15.0/tldr.py
```

### Comparing `multi-tldr-0.14.1/LICENSE` & `multi-tldr-0.15.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multi-tldr-0.14.1/PKG-INFO` & `multi-tldr-0.15.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: multi-tldr
-Version: 0.14.1
+Version: 0.15.0
 Summary: Yet another python client for tldr-pages/tldr. View tldr pages in multi repo, multi platform, any language at the same time.
 Home-page: https://github.com/Phuker/multi-tldr
 Author: Phuker
 Author-email: Phuker@users.noreply.github.com
 License: MIT
-Description: [Project homepage](https://github.com/Phuker/multi-tldr)
-        
-        [Readme](https://github.com/Phuker/multi-tldr/blob/master/Readme.md)
-        
 Keywords: tldr cli man command usage
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[Project homepage](https://github.com/Phuker/multi-tldr)
+
+[Readme](https://github.com/Phuker/multi-tldr/blob/master/Readme.md)
```

### Comparing `multi-tldr-0.14.1/Readme.md` & `multi-tldr-0.15.0/Readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,15 @@
     "color_output": "auto",
     "colors": {
         "description": "bright_yellow",
         "usage": "green",
         "command": "white",
         "param": "cyan"
     },
+    "command_indent_size": 4,
     "platform_list": [
         "common",
         "osx",
         "linux"
     ],
     "compact_output": false
 }
@@ -139,15 +140,15 @@
 tldr --help
 ```
 
 ### Show version info
 
 ```console
 $ tldr --version
-multi-tldr, by Phuker, version 0.13.1
+multi-tldr, by Phuker, version 0.15.0
 Homepage: https://github.com/Phuker/multi-tldr
 This tldr client is designed based on the tldr-pages client specification 1.4, but not 100% implemented.
 ```
 
 ### Look up a command usage
 
 ```bash
@@ -233,16 +234,14 @@
 
 **Q: How to auto update tldr pages?**
 
 A: This program will neither update tldr pages when loop up a command, nor create a daemon or service to update tldr pages periodically. Updating is totally up to you. You can run `tldr --update` manually at any time you want, or use `crontab`, Windows `Task Scheduler` or any tool else to automatically update.
 
 ## Contributing
 
-- It sucks? Why not help me improve it? Let me know the bad things.
-- Want a new feature? Feel free to file an issue for a feature request.
-- Find a bug? Open an issue please, or it's better if you can send me a pull request.
+It sucks? Want a new feature? Find a bug?
 
-Contributions are always welcome at any time!
+Please open an issue, and let me know the bad things and your opinion. After our discussion, a pull request is welcomed.
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for the full license text.
```

### Comparing `multi-tldr-0.14.1/multi_tldr.egg-info/PKG-INFO` & `multi-tldr-0.15.0/multi_tldr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: multi-tldr
-Version: 0.14.1
+Version: 0.15.0
 Summary: Yet another python client for tldr-pages/tldr. View tldr pages in multi repo, multi platform, any language at the same time.
 Home-page: https://github.com/Phuker/multi-tldr
 Author: Phuker
 Author-email: Phuker@users.noreply.github.com
 License: MIT
-Description: [Project homepage](https://github.com/Phuker/multi-tldr)
-        
-        [Readme](https://github.com/Phuker/multi-tldr/blob/master/Readme.md)
-        
 Keywords: tldr cli man command usage
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[Project homepage](https://github.com/Phuker/multi-tldr)
+
+[Readme](https://github.com/Phuker/multi-tldr/blob/master/Readme.md)
```

### Comparing `multi-tldr-0.14.1/setup.py` & `multi-tldr-0.15.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     py_modules = ['tldr'],
     install_requires=[
         'click>=5.0',
     ],
     include_package_data=True,
     entry_points={
         'console_scripts': [
-            'tldr=tldr:_main'
+            'tldr=tldr:main'
         ]
     },
     classifiers=[
         'Environment :: Console',
         'Operating System :: POSIX',
         'Operating System :: POSIX :: Linux',
         'License :: OSI Approved :: MIT License',
```

### Comparing `multi-tldr-0.14.1/tldr.py` & `multi-tldr-0.15.0/tldr.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,54 +5,124 @@
 multi-tldr
 
 Yet another python client for tldr-pages/tldr. View tldr pages in multi repo, multi platform, any language at the same time.
 
 https://github.com/Phuker/multi-tldr
 """
 
-
 import os
 import sys
+import argparse
+import logging
 import re
 import json
-import logging
-import argparse
 import subprocess
 import functools
 
-import click
+# buggy: https://github.com/pallets/click/issues/665
+# import readline
 
+import click
 
-__title__ = "multi-tldr"
-__version__ = "0.14.1"
-__author__ = "Phuker"
-__homepage__ = "https://github.com/Phuker/multi-tldr"
-__license__ = "MIT"
-__copyright__ = "Copyright (c) 2020 Phuker, Copyright (c) 2015 lord63"
-__specification__ = "This tldr client is designed based on the tldr-pages client specification 1.4, but not 100% implemented."
 
+__title__ = 'multi-tldr'
+__version__ = '0.15.0'
+__author__ = 'Phuker'
+__homepage__ = 'https://github.com/Phuker/multi-tldr'
+__license__ = 'MIT'
+__copyright__ = 'Copyright (c) 2020 Phuker, Copyright (c) 2015 lord63'
+__specification__ = 'This tldr client is designed based on the tldr-pages client specification 1.4, but not 100% implemented.'
 
 # High coupling
 # make things just work at a minimal level, or can not even --init
 DEFAULT_CONFIG = {
     'repo_directory_list': [],
     'color_output': 'never',
     'colors': {
         'description': 'bright_yellow',
         'usage': 'green',
         'command': 'white',
         'param': 'cyan',
     },
+    'command_indent_size': 4,
     'platform_list': [],
     'compact_output': False,
 }
 
-if sys.flags.optimize > 0:
-    print('Error: Do not run with "-O", assert require no optimize', file=sys.stderr)
-    sys.exit(1)
+logger = logging.getLogger(__name__)
+shell_args = None
+
+
+def _assert(expr, msg=''):
+    if not expr:
+        raise AssertionError(msg)
+
+
+def _init_logging():
+    logging_stream = sys.stderr
+    logging_format = '%(asctime)s [%(levelname)s]:%(message)s'
+    logging_level = logging.INFO
+
+    if logging_stream.isatty():
+        logging_date_format = '%H:%M:%S'
+    else:
+        logging_date_format = '%Y-%m-%d %H:%M:%S %z'
+
+    logging.basicConfig(
+        level=logging_level,
+        format=logging_format,
+        datefmt=logging_date_format,
+        stream=logging_stream,
+    )
+
+
+def _parse_args(args=sys.argv[1:]):
+    parser = argparse.ArgumentParser(
+        description='Yet another python client for tldr-pages/tldr. View tldr pages in multi repo, multi platform, any language at the same time.',
+        epilog='https://github.com/Phuker/multi-tldr',
+        add_help=True
+    )
+    group = parser.add_mutually_exclusive_group(required=False)
+    group.add_argument('-i', '--init', action='store_true', help='Interactively gererate config file')
+    group.add_argument('-l', '--list', action='store_true', help='Print all tldr page files path (of a command if specified) in all repo on all/specified platform')
+    group.add_argument('-u', '--update', action='store_true', help='Pull all git repo')
+    
+    parser.add_argument('command', help='Command to query', nargs='*')
+    parser.add_argument('-p', '--platform', help="Specify platform. Special virtual platform options are 'all' and 'default'", choices=['common', 'linux', 'osx', 'sunos', 'windows', 'all', 'default'])
+
+    parser.add_argument('-V', '--version', action='store_true', help='Show version and exit')
+    parser.add_argument('-v', '--verbose', action='count', default=0, help='Increase verbosity level (use -vv or more for greater effect)')
+
+    result = parser.parse_args(args)
+
+    if result.verbose >= 1:
+        logging.root.setLevel(logging.DEBUG)
+    
+    if result.command:
+        result.command = '-'.join(result.command)
+    else:
+        result.command = None
+    
+    ctrl_group_set = result.init or result.list or result.update
+    ok_conditions = [
+        result.version,
+        result.init and result.command is None and result.platform is None,
+        result.list,
+        result.update and result.command is None and result.platform is None,
+        not ctrl_group_set and result.command is not None,
+    ]
+
+    if not any(ok_conditions):
+        logger.error('Bad command line arguments')
+        parser.print_help()
+        sys.exit(1)
+
+    logger.debug('Command line arguments: %r', result)
+
+    return result
 
 
 def get_config_dir_path():
     sub_dir_name = 'multi-tldr'
     if 'TLDR_CONFIG_DIR' in os.environ:
         config_dir_path = os.environ.get('TLDR_CONFIG_DIR')
     elif 'XDG_CONFIG_HOME' in os.environ:
@@ -66,107 +136,101 @@
 
 
 def get_config_path():
     return os.path.join(get_config_dir_path(), 'tldr.config.json')
 
 
 def check_config(config):
-    assert type(config) == dict, 'type(config) != dict'
-    assert type(config['color_output']) == str, 'type(color_output) != str'
-    assert type(config['colors']) == dict, 'type(colors) != dict'
-    assert type(config['platform_list']) == list, 'type(platform_list) != list'
-    assert type(config['repo_directory_list']) == list, 'type(repo_directory_list) != list'
-    assert type(config['compact_output']) == bool, 'type(compact_output) != bool'
+    _assert(isinstance(config, dict), 'Invalid config')
+    _assert(isinstance(config['color_output'], str), 'Invalid color_output')
+    _assert(isinstance(config['colors'], dict), 'Invalid colors')
+    _assert(isinstance(config['platform_list'], list), 'Invalid platform_list')
+    _assert(isinstance(config['repo_directory_list'], list), 'Invalid repo_directory_list')
+    _assert(isinstance(config['compact_output'], bool), 'Invalid compact_output')
+    _assert(isinstance(config['command_indent_size'], int), 'Invalid command_indent_size')
 
-    supported_color_output = ('always', 'auto', 'never')
-    assert config['color_output'] in supported_color_output
+    _assert(config['color_output'] in ('always', 'auto', 'never'))
+    _assert(config['command_indent_size'] >= 0, 'Invalid command_indent_size')
     
     supported_colors = ('black', 'red', 'green', 'yellow', 'blue', 'magenta', 'cyan', 'white', 'bright_black', 'bright_red', 'bright_green', 'bright_yellow', 'bright_blue', 'bright_magenta', 'bright_cyan', 'bright_white')
     if not set(config['colors'].values()).issubset(set(supported_colors)):
         bad_colors = set(config['colors'].values()) - set(supported_colors)
         bad_colors_str = ', '.join([repr(_) for _ in bad_colors])
         raise ValueError(f'Unsupported colors in config file: {bad_colors_str}')
 
     for platform in config['platform_list']:
-        assert type(platform) == str, f'Bad item in platform_list: {platform!r}'
+        _assert(isinstance(platform, str), 'Invalid platform_list')
     
     for _repo_dir in config['repo_directory_list']:
-        assert type(_repo_dir) == str, f'Bad item in repo_directory_list: {_repo_dir!r}'
-        if not os.path.exists(_repo_dir):
-            raise ValueError(f"Path in repo_directory_list not exist: {_repo_dir!r}")
+        _assert(isinstance(_repo_dir, str), 'Invalid repo_directory_list')
+        _assert(os.path.exists(os.path.abspath(os.path.expanduser(_repo_dir))), f'Path in repo_directory_list not exist: {_repo_dir!r}')
 
 
 def load_json(file_path):
-    assert type(file_path) == str
-
-    log = logging.getLogger(__name__)
+    _assert(isinstance(file_path, str))
 
     try:
         with open(file_path, 'r', encoding='utf-8') as f:
-            result = json.load(f)
-            return result
+            return json.load(f)
     except Exception as e:
-        log.error('Error when load json file %r: %r %r', file_path, type(e), e)
+        logger.error('Error when load json file %r: %r %r', file_path, type(e), e)
         sys.exit(1)
 
 
 @functools.lru_cache
 def get_config():
     """Get the configurations and return it as a dict."""
 
-    log = logging.getLogger(__name__)
-
     config_path = get_config_path()
     if not os.path.exists(config_path):
-        log.error("Can't find config file at: %r.", config_path)
-        log.error('You may use `tldr --init` to init the config file.')
+        logger.error("Can't find config file at: %r", config_path)
+        logger.error('You may use `tldr --init` to init the config file')
         return DEFAULT_CONFIG
 
-    log.debug('Reading file: %r', config_path) # os.debug() won't output until a handler is inited
+    logger.debug('Reading config file: %r', config_path)
     config = load_json(config_path)
 
     try:
         check_config(config)
-        return config
     except Exception as e:
-        log.error('Check config failed: %r.', e)
-        log.error('You may use `tldr --init` to init the config file.')
+        logger.error('Check config failed: %r', e)
+        logger.error('You may use `tldr --init` to init the config file')
         return DEFAULT_CONFIG
 
+    config['repo_directory_list'] = [os.path.abspath(os.path.expanduser(_)) for _ in config['repo_directory_list']]
+
+    return config
+
 
 def style(text, *args, **kwargs):
     """Wrapper of click.style()"""
 
     color_output = get_config()['color_output']
 
-    if color_output == 'always':
+    if color_output == 'always' or (color_output == 'auto' and sys.stdout.isatty() and 'TERM' in os.environ):
         return click.style(text, *args, **kwargs)
-    elif color_output == 'auto':
-        if sys.stdout.isatty() and 'TERM' in os.environ:
-            return click.style(text, *args, **kwargs)
-        else:
-            return text
-    else: # 'never'
+    else:
         return text
 
 
 @functools.lru_cache
 def get_escape_str(*args, **kwargs):
     """Wrapper of style(), get escape string without reset string at the end"""
 
     if 'reset' not in kwargs:
         kwargs['reset'] = False
+    
     return style('', *args, **kwargs)
 
 
 @functools.lru_cache
 def get_escape_str_by_type(_type):
     """Get escape string by type"""
 
-    assert _type is None or type(_type) == str
+    _assert(_type is None or isinstance(_type, str))
 
     colors = get_config()['colors']
 
     if _type is None:
         return ''
     elif _type in ('description', 'usage', 'command'):
         return get_escape_str(fg=colors[_type], underline=False)
@@ -209,19 +273,18 @@
     result += get_escape_str(reset=True)
     return result
 
 
 def parse_page(page_file_path):
     """Parse the command man page."""
 
-    log = logging.getLogger(__name__)
-
     compact_output = get_config()['compact_output']
+    command_indent_size = get_config()['command_indent_size']
 
-    log.debug('Reading file: %r', page_file_path)
+    logger.debug('Reading file: %r', page_file_path)
     with open(page_file_path, 'r', encoding='utf-8') as f:
         lines = f.readlines() # with '\n' end
     
     output_lines = []
     for line in lines:
         line = line.strip('\n')
         if line.startswith('# '): # h1
@@ -231,15 +294,15 @@
             output_lines.append(line)
         elif line.startswith('- '): # usage
             line = parse_inline_md(line[2:], 'usage')
             output_lines.append(line)
         elif line.startswith('`'): # code example
             line = line.strip('`')
             line = parse_inline_md(line, 'command')
-            line = '    ' + line
+            line = (' ' * command_indent_size) + line
             output_lines.append(line)
         elif line == '':
             if not compact_output:
                 # default: reset = True, add reset string at the end
                 output_lines.append(style(line))
             else:
                 pass
@@ -253,36 +316,34 @@
 
 @functools.lru_cache
 def get_index(repo_directory):
     """Generate index in the pages directory.
     Return: [(platform, command), ]
     """
 
-    assert type(repo_directory) == str
-
-    log = logging.getLogger(__name__)
+    _assert(isinstance(repo_directory, str))
 
     index = []
 
-    log.debug('os.walk() in %r', repo_directory)
+    logger.debug('os.walk() in %r', repo_directory)
     tree_generator = os.walk(repo_directory)
     platforms = next(tree_generator)[1]
     
     for platform in platforms:
         pages = next(tree_generator)[2]
         index += [(platform, page[:-3]) for page in pages if page.endswith('.md')] # there is no .MD uppercase
     
     return index
 
 
 def get_page_path_list(command=None, platform='default'):
     """Get page_path_list in all repo"""
 
-    assert command is None or type(command) == str
-    assert type(platform) == str
+    _assert(command is None or isinstance(command, str))
+    _assert(isinstance(platform, str))
 
     repo_directory_list = get_config()['repo_directory_list']
     default_platform_set = set(get_config()['platform_list'])
 
     page_path_list = []
     for repo_directory in repo_directory_list:
         index = get_index(repo_directory)
@@ -302,130 +363,129 @@
     
     return page_path_list
 
 
 def action_init():
     """Interactively gererate config file"""
 
-    log = logging.getLogger(__name__)
-
     config_path = get_config_path()
     if os.path.exists(config_path):
-        log.warning("A config file already exists: %r", config_path)
+        logger.warning('A config file already exists: %r', config_path)
         if click.prompt('Are you sure want to overwrite it? (yes/no)', default='no') != 'yes':
             return
     
     repo_path_list = []
-    log.info('Please input repo path line by line, to "pages/" level, empty line to end.')
+    logger.info('Please input repo path line by line, to "pages/" level, empty line to end.')
     while True:
-        repo_path = click.prompt("Input 1 tldr repo path", default='')
+        repo_path = click.prompt('Input 1 tldr repo path', default='')
         if len(repo_path) == 0:
             break
         repo_path = os.path.abspath(os.path.expanduser(repo_path))
         if not os.path.exists(repo_path):
-            log.error("Repo path not exist, clone it first.")
+            logger.error('Repo path not exist, clone it first.')
         elif repo_path not in repo_path_list:
             repo_path_list.append(repo_path)
 
     platform_list = []
-    platform_choice = click.Choice(('common', 'linux', 'osx', 'sunos', 'windows'))
-    log.info('Please input default platforms line by line, empty line to end.')
+    platform_choice = click.Choice(('common', 'linux', 'osx', 'sunos', 'windows', ''))
+    logger.info('Please input default platforms line by line, empty line to end.')
     while True:
-        platform = click.prompt("Input 1 platform", type=platform_choice, default='')
+        platform = click.prompt('Input 1 platform', type=platform_choice, default='')
         if len(platform) == 0:
             break
         elif platform not in platform_list:
             platform_list.append(platform)
 
-    log.info('Please input colors, empty to use default.')
+    logger.info('Please input colors, empty to use default.')
     colors_choice = click.Choice(('black', 'red', 'green', 'yellow', 'blue', 'magenta', 'cyan', 'white', 'bright_black', 'bright_red', 'bright_green', 'bright_yellow', 'bright_blue', 'bright_magenta', 'bright_cyan', 'bright_white'))
     colors = {
-        "description": click.prompt('Input color for description', type=colors_choice, default='bright_yellow'),
-        "usage": click.prompt('Input color for usage', type=colors_choice, default='green'),
-        "command": click.prompt('Input color for command', type=colors_choice, default='white'),
-        "param": click.prompt('Input color for param', type=colors_choice, default='cyan'),
+        'description': click.prompt('Input color for description', type=colors_choice, default='bright_yellow'),
+        'usage': click.prompt('Input color for usage', type=colors_choice, default='green'),
+        'command': click.prompt('Input color for command', type=colors_choice, default='white'),
+        'param': click.prompt('Input color for param', type=colors_choice, default='cyan'),
     }
 
     color_output_choice = click.Choice(('always', 'auto', 'never'))
     color_output = click.prompt('When output with color?', type=color_output_choice, default='auto')
 
+    command_indent_size = click.prompt('Command indent size?', type=int, default=4)
+    if command_indent_size < 0:
+        command_indent_size = 0
+
     compact_output = click.prompt('Enable compact output (not output empty lines)? (yes/no)', default='no') == 'yes'
 
     config = {
         'repo_directory_list': repo_path_list,
         'color_output': color_output,
         'colors': colors,
+        'command_indent_size': command_indent_size,
         'platform_list': platform_list,
         'compact_output': compact_output,
     }
 
     config_dir_path = get_config_dir_path()
     if not os.path.exists(config_dir_path):
-        log.info('Make dir: %r', config_dir_path)
+        logger.info('Make dir: %r', config_dir_path)
         os.makedirs(config_dir_path)
 
-    log.info("Write to config file %r", config_path)
+    logger.info('Write to config file %r', config_path)
     with open(config_path, 'w') as f:
         f.write(json.dumps(config, ensure_ascii=True, indent=4))
 
 
 def action_update():
     """Update all tldr pages repo."""
 
-    log = logging.getLogger(__name__)
-
     repo_directory_list = get_config()['repo_directory_list']
     command = ['git', 'pull', '--stat']
     command_str = ' '.join(command)
 
     for repo_directory in repo_directory_list:
         os.chdir(repo_directory)
-        log.info("Check for updates in %r ...", repo_directory)
+        logger.info('Check for updates in %r ...', repo_directory)
         try:
             return_code = subprocess.call(command)
             return_code_color = 'green' if return_code == 0 else 'bright_red'
             return_code_str = style(str(return_code), fg=return_code_color)
 
-            log.info('Command %r return code %s', command_str, return_code_str)
+            logger.info('Command %r return code %s', command_str, return_code_str)
         except Exception as e:
-            log.error('Error when run %r in %r: %r %r', command_str, repo_directory, type(e), e)
+            logger.error('Error when run %r in %r: %r %r', command_str, repo_directory, type(e), e)
 
 
 def action_find(command, platform):
     """Find and display the tldr pages of a command."""
 
-    assert type(command) == str
-    assert platform is None or type(platform) == str
-
-    log = logging.getLogger(__name__)
+    _assert(isinstance(command, str))
+    _assert(platform is None or isinstance(platform, str))
 
     if platform:
         page_path_list = get_page_path_list(command, platform)
     else:
         page_path_list = get_page_path_list(command, 'default')
     
     if len(page_path_list) == 0:
-        log.error("Command not found: %r", command)
-        log.error("You can try to find a page on all platforms by run %r.", f'tldr -p all {command}')
-        log.error("If still nothing, you can create a new issue against the tldr-pages/tldr GitHub repository: %r,", f'https://github.com/tldr-pages/tldr/issues/new?title=page%20request:%20{command}')
-        log.error("or create a Pull Request on GitHub.")
+        logger.error('Command not found: %r', command)
+        logger.error('You can try to find a page on all platforms by run %r.', f'tldr -p all {command}')
+        logger.error('If still nothing, you can create a new issue against the tldr-pages/tldr GitHub repository: %r,', f'https://github.com/tldr-pages/tldr/issues/new?title=page%20request:%20{command}')
+        logger.error('or create a Pull Request on GitHub.')
         sys.exit(1)
     else:
         for page_path in page_path_list:
-            print(style(command + ' - ' + page_path, underline=True, bold=True))
+            print(style(command, underline=True, bold=True) + ' - ' + style(page_path, underline=True, bold=True))
             output_lines = parse_page(page_path)
             for line in output_lines:
                 print(line)
 
 
 def action_list_command(command, platform):
     """Locate all tldr page files path of the command."""
     
-    assert command is None or type(command) == str
-    assert platform is None or type(platform) == str
+    _assert(command is None or isinstance(command, str))
+    _assert(platform is None or isinstance(platform, str))
 
     if platform:
         page_path_list = get_page_path_list(command, platform)
     else:
         page_path_list = get_page_path_list(command, 'all')
     
     for page_path in page_path_list:
@@ -434,118 +494,42 @@
 
 def action_version():
     print(f'{__title__}, by {__author__}, version {__version__}')
     print(f'Homepage: {__homepage__}')
     print(__specification__)
 
 
-def parse_args(args=sys.argv[1:]):
-    log = logging.getLogger(__name__)
-
-    parser = argparse.ArgumentParser(
-        description='Yet another python client for tldr-pages/tldr. View tldr pages in multi repo, multi platform, any language at the same time.',
-        epilog='https://github.com/Phuker/multi-tldr',
-        add_help=True
-    )
-    group = parser.add_mutually_exclusive_group(required=False)
-    group.add_argument('-i', '--init', action="store_true", help="Interactively gererate config file")
-    group.add_argument('-l', '--list', action='store_true', help="Print all tldr page files path (of a command if specified) in all repo on all/specified platform")
-    group.add_argument('-u', '--update', action="store_true", help="Pull all git repo")
-    
-    parser.add_argument('command', help="Command to query", nargs='*')
-    parser.add_argument('-p', '--platform', help="Specify platform. Special virtual platform options are 'all' and 'default'", choices=['common', 'linux', 'osx', 'sunos', 'windows', 'all', 'default'])
-
-    parser.add_argument('-v', '--version', action="store_true", help="Show version and exit")
-
-    args = parser.parse_args(args)
-
-    if len(args.command) > 0:
-        args.command = '-'.join(args.command)
-    else:
-        args.command = None
-
-    ctrl_group_set = args.init or args.list or args.update
-    ok_conditions = [
-        args.version,
-        args.init and args.command is None and args.platform is None,
-        args.list,
-        args.update and args.command is None and args.platform is None,
-        not ctrl_group_set and args.command is not None,
-    ]
-
-    if not any(ok_conditions):
-        log.error('Bad arguments')
-        parser.print_help()
-        sys.exit(1)
-    
-    return args
-
-
-def init_logging():
-    escape_bold = get_escape_str(bold=True)
-    escape_reset = get_escape_str(reset=True)
-    escape_fg_default = get_escape_str(fg='reset')
-    escape_fg_red = get_escape_str(fg='red')
-    escape_fg_yellow = get_escape_str(fg='yellow')
-    escape_fg_cyan = get_escape_str(fg='cyan')
-
-    logging_stream = sys.stderr
-    logging_format = f'{escape_bold}%(asctime)s [%(levelname)s]:{escape_reset}%(message)s'
-
-    if 'DEBUG' in os.environ:
-        logging_level = logging.DEBUG
-    else:
-        logging_level = logging.INFO
-
-    if logging_stream.isatty():
-        logging_date_format = '%H:%M:%S'
-    else:
-        print('', file=logging_stream)
-        logging_date_format = '%Y-%m-%d %H:%M:%S'
-
-    logging.basicConfig(
-        level=logging_level,
-        format=logging_format,
-        datefmt=logging_date_format,
-        stream=logging_stream,
-    )
+def broken_pipe_error_wrapper(func):
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs):
+        # https://docs.python.org/3/library/signal.html#note-on-sigpipe
+        try:
+            return func(*args, **kwargs)
+        except BrokenPipeError:
+            devnull = os.open(os.devnull, os.O_WRONLY)
+            os.dup2(devnull, sys.stdout.fileno())
+            sys.exit(1)
 
-    logging.addLevelName(logging.CRITICAL, f'{escape_fg_red}{logging.getLevelName(logging.CRITICAL)}{escape_fg_default}')
-    logging.addLevelName(logging.ERROR, f'{escape_fg_red}{logging.getLevelName(logging.ERROR)}{escape_fg_default}')
-    logging.addLevelName(logging.WARNING, f'{escape_fg_yellow}{logging.getLevelName(logging.WARNING)}{escape_fg_default}')
-    logging.addLevelName(logging.INFO, f'{escape_fg_cyan}{logging.getLevelName(logging.INFO)}{escape_fg_default}')
-    logging.addLevelName(logging.DEBUG, f'{escape_fg_cyan}{logging.getLevelName(logging.DEBUG)}{escape_fg_default}')
+    return wrapper
 
 
+@broken_pipe_error_wrapper
 def main():
-    """Real entry point"""
-
-    init_logging()
-    args = parse_args()
+    _init_logging()
+    shell_args = _parse_args()
 
-    if args.version:
+    if shell_args.version:
         action_version()
-    elif args.init:
+    elif shell_args.init:
         action_init()
-    elif args.list:
-        action_list_command(args.command, args.platform)
-    elif args.update:
+    elif shell_args.list:
+        action_list_command(shell_args.command, shell_args.platform)
+    elif shell_args.update:
         action_update()
     else:
-        action_find(args.command, args.platform)
-
-
-def _main():
-    """Entry point wrapper"""
-
-    # https://docs.python.org/3/library/signal.html#note-on-sigpipe
-    try:
-        main()
-        sys.stdout.flush()
-    except BrokenPipeError:
-        devnull = os.open(os.devnull, os.O_WRONLY)
-        os.dup2(devnull, sys.stdout.fileno())
-        sys.exit(1)
+        action_find(shell_args.command, shell_args.platform)
+    
+    sys.stdout.flush()
 
 
-if __name__ == "__main__":
-    _main()
+if __name__ == '__main__':
+    main()
```

