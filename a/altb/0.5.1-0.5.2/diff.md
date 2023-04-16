# Comparing `tmp/altb-0.5.1.tar.gz` & `tmp/altb-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altb-0.5.1.tar", max compression
+gzip compressed data, was "altb-0.5.2.tar", max compression
```

## Comparing `altb-0.5.1.tar` & `altb-0.5.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1541 2023-04-11 19:07:53.402512 altb-0.5.1/README.md
--rw-r--r--   0        0        0        0 2023-04-11 19:07:53.402512 altb-0.5.1/altb/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 19:07:53.402512 altb-0.5.1/altb/common/__init__.py
--rw-r--r--   0        0        0      109 2023-04-11 19:07:53.402512 altb-0.5.1/altb/common/console.py
--rw-r--r--   0        0        0      378 2023-04-11 19:07:53.402512 altb-0.5.1/altb/common/constants.py
--rw-r--r--   0        0        0     1148 2023-04-11 19:07:53.402512 altb-0.5.1/altb/common/rich.py
--rw-r--r--   0        0        0     3336 2023-04-11 19:07:53.402512 altb-0.5.1/altb/common/selector.py
--rw-r--r--   0        0        0      275 2023-04-11 19:07:53.402512 altb-0.5.1/altb/common/utils.py
--rw-r--r--   0        0        0    10799 2023-04-11 19:07:53.402512 altb-0.5.1/altb/main.py
--rw-r--r--   0        0        0        0 2023-04-11 19:07:53.402512 altb-0.5.1/altb/model/__init__.py
--rw-r--r--   0        0        0      739 2023-04-11 19:07:53.402512 altb-0.5.1/altb/model/config.py
--rw-r--r--   0        0        0     1021 2023-04-11 19:07:53.402512 altb-0.5.1/altb/model/settings.py
--rw-r--r--   0        0        0     1548 2023-04-11 19:07:53.402512 altb-0.5.1/altb/model/tags.py
--rw-r--r--   0        0        0     2680 2023-04-11 19:07:53.402512 altb-0.5.1/altb/options.py
--rw-r--r--   0        0        0    10849 2023-04-11 19:07:53.402512 altb-0.5.1/altb/service.py
--rw-r--r--   0        0        0     1805 2023-04-11 19:07:53.402512 altb-0.5.1/altb/track.py
--rw-r--r--   0        0        0       18 2023-04-11 19:08:01.882676 altb-0.5.1/altb/version_file.py
--rw-r--r--   0        0        0      898 2023-04-11 19:08:01.846675 altb-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 altb-0.5.1/setup.py
--rw-r--r--   0        0        0     2398 1970-01-01 00:00:00.000000 altb-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1660 2023-04-16 11:56:27.600811 altb-0.5.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-16 11:56:27.600811 altb-0.5.2/altb/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 11:56:27.600811 altb-0.5.2/altb/common/__init__.py
+-rw-r--r--   0        0        0      109 2023-04-16 11:56:27.600811 altb-0.5.2/altb/common/console.py
+-rw-r--r--   0        0        0      378 2023-04-16 11:56:27.600811 altb-0.5.2/altb/common/constants.py
+-rw-r--r--   0        0        0     1148 2023-04-16 11:56:27.600811 altb-0.5.2/altb/common/rich.py
+-rw-r--r--   0        0        0     3336 2023-04-16 11:56:27.600811 altb-0.5.2/altb/common/selector.py
+-rw-r--r--   0        0        0      275 2023-04-16 11:56:27.600811 altb-0.5.2/altb/common/utils.py
+-rw-r--r--   0        0        0    10819 2023-04-16 11:56:27.600811 altb-0.5.2/altb/main.py
+-rw-r--r--   0        0        0        0 2023-04-16 11:56:27.600811 altb-0.5.2/altb/model/__init__.py
+-rw-r--r--   0        0        0      739 2023-04-16 11:56:27.600811 altb-0.5.2/altb/model/config.py
+-rw-r--r--   0        0        0     1021 2023-04-16 11:56:27.600811 altb-0.5.2/altb/model/settings.py
+-rw-r--r--   0        0        0     1548 2023-04-16 11:56:27.600811 altb-0.5.2/altb/model/tags.py
+-rw-r--r--   0        0        0     2680 2023-04-16 11:56:27.600811 altb-0.5.2/altb/options.py
+-rw-r--r--   0        0        0    10849 2023-04-16 11:56:27.600811 altb-0.5.2/altb/service.py
+-rw-r--r--   0        0        0     1805 2023-04-16 11:56:27.600811 altb-0.5.2/altb/track.py
+-rw-r--r--   0        0        0       18 2023-04-16 11:56:36.808729 altb-0.5.2/altb/version_file.py
+-rw-r--r--   0        0        0      898 2023-04-16 11:56:36.776729 altb-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2609 1970-01-01 00:00:00.000000 altb-0.5.2/setup.py
+-rw-r--r--   0        0        0     2513 1970-01-01 00:00:00.000000 altb-0.5.2/PKG-INFO
```

### Comparing `altb-0.5.1/README.md` & `altb-0.5.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -50,7 +50,12 @@
 ```bash
 altb track command special_command@latest "echo This is a command"
 ```
 this especially useful for latest developments, example:
 ```bash
 altb track command special_command@latest "go run ./cmd/special_command" --working-directory "$HOME/special_command"
 ```
+
+
+## Docs
+### Migrations
+- [Migrate to v0.5.0 and above from lower versions](./docs/migrations/migrate_to_0_5_0.md)
```

### Comparing `altb-0.5.1/altb/common/rich.py` & `altb-0.5.2/altb/common/rich.py`

 * *Files identical despite different names*

### Comparing `altb-0.5.1/altb/common/selector.py` & `altb-0.5.2/altb/common/selector.py`

 * *Files identical despite different names*

### Comparing `altb-0.5.1/altb/main.py` & `altb-0.5.2/altb/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from altb.common.constants import TYPE_TO_COLOR, PACKAGE_NAME
 from altb.options import (app_name_option,
                           is_short_option,
                           is_current_option,
                           all_tags_option,
                           full_app_name_option, should_force_option)
 
-
 app = typer.Typer(pretty_exceptions_enable=False)
 
 app.add_typer(track, name="track")
 
 
 @app.command()
 def config(ctx: typer.Context, is_json: bool = typer.Option(False, '-j', '--json', help='Output in json format')):
@@ -52,17 +51,17 @@
         typer.echo(to_print)
 
 
 @app.command(name="list")
 def list_applications(
         ctx: typer.Context,
         app_name=app_name_option,
-        is_short=is_short_option,
-        all_tags=all_tags_option,
-        current_only=is_current_option,
+        is_short: bool = is_short_option,
+        all_tags: bool = all_tags_option,
+        current_only: bool = is_current_option,
 ):
     """List all applications tracked."""
     settings = ctx.ensure_object(Settings)
     service = AltbService(settings)
 
     if len(service.config.binaries) == 0:
         error_console.print(f'No binaries currently tracked, please use "{PACKAGE_NAME} track" command to start')
@@ -195,15 +194,15 @@
         return tag
 
 
 @app.command()
 def use(
         ctx: typer.Context,
         app_details=full_app_name_option,
-        force=should_force_option,
+        force: bool = should_force_option,
 ):
     """Select which tag to run of a given app."""
     settings = ctx.ensure_object(Settings)
     service = AltbService(settings)
     app_name, tag = app_details
     if not tag:
         tag = get_tag_dynamic(service.config, app_name)
@@ -255,15 +254,15 @@
         service.select(app_name, tag=None)
 
 
 @app.command()
 def schema(
         ctx: typer.Context,
         model: Optional[str] = typer.Argument(None),
-        dump_all: Optional[bool] = typer.Option(False, '-a', '--all', help='Dump all scheme')
+        dump_all: bool = typer.Option(False, '-a', '--all', help='Dump all scheme')
 ):
     settings = ctx.ensure_object(Settings)
     service = AltbService(settings)
     schema = service.config.schema()
 
     if model is not None:
         if model not in schema['definitions']:
```

### Comparing `altb-0.5.1/altb/model/config.py` & `altb-0.5.2/altb/model/config.py`

 * *Files identical despite different names*

### Comparing `altb-0.5.1/altb/model/settings.py` & `altb-0.5.2/altb/model/settings.py`

 * *Files identical despite different names*

### Comparing `altb-0.5.1/altb/model/tags.py` & `altb-0.5.2/altb/model/tags.py`

 * *Files identical despite different names*

### Comparing `altb-0.5.1/altb/options.py` & `altb-0.5.2/altb/options.py`

 * *Files identical despite different names*

### Comparing `altb-0.5.1/altb/service.py` & `altb-0.5.2/altb/service.py`

 * *Files identical despite different names*

### Comparing `altb-0.5.1/altb/track.py` & `altb-0.5.2/altb/track.py`

 * *Files identical despite different names*

### Comparing `altb-0.5.1/pyproject.toml` & `altb-0.5.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "altb"
-version = "0.5.1"  # this means version is development
+version = "0.5.2"  # this means version is development
 description = "Cli tool for tracking over binaries and easily swapping between them"
 readme = "README.md"
 authors = ["Elran Shefer <elran777@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Utilities",
```

### Comparing `altb-0.5.1/setup.py` & `altb-0.5.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,17 @@
  'typer>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['altb = altb.main:main']}
 
 setup_kwargs = {
     'name': 'altb',
-    'version': '0.5.1',
+    'version': '0.5.2',
     'description': 'Cli tool for tracking over binaries and easily swapping between them',
-    'long_description': '# altb\naltb is a cli utility influenced by `update-alternatives` of ubuntu.  \nLinked paths are added to `$HOME/.local/bin` according to [XDG Base Directory Specification](https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html).  \nConfig file is located at `$HOME/.config/altb/config.yaml`.\n\n### How to start?\n\n**Must use Python > 3.9**\nexecute:\n```bash\npipx install altb\n```\n\nto track new binary use:\n```bash\naltb track path <app_name>@<app_tag> /path/to/binary\n```\nfor example:\n```bash\naltb track path python@2.7 /bin/python2.7\naltb track path python@3.8 /bin/python3.8\n# altb track path python ~/Downloads/python # will also work and generate a new hash for it\n```\n\nList all tracked versions:\n```bash\n$ altb list -a\npython\n|----   2.7 - /bin/python2.7\n|----   3.8 - /bin/python3.8\n```\n\nUse specific version:\n```bash\naltb use <app_name>[@<app_tag>]\n```\n\nexample:\n```bash\naltb use python@2.7\n```\nthis will link the tracked path to `~/.local/bin/<app_name>` in this case - `~/.local/bin/python`\n\nCopy specific standalone binary automatically to `~/.local/share/altb/versions/<app_name>/<app_name>_<tag>`\n```bash\naltb track path helm@3 ~/Downloads/helm --copy\n```\n\nYou can run custom commands using:\n```bash\naltb track command special_command@latest "echo This is a command"\n```\nthis especially useful for latest developments, example:\n```bash\naltb track command special_command@latest "go run ./cmd/special_command" --working-directory "$HOME/special_command"\n```\n',
+    'long_description': '# altb\naltb is a cli utility influenced by `update-alternatives` of ubuntu.  \nLinked paths are added to `$HOME/.local/bin` according to [XDG Base Directory Specification](https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html).  \nConfig file is located at `$HOME/.config/altb/config.yaml`.\n\n### How to start?\n\n**Must use Python > 3.9**\nexecute:\n```bash\npipx install altb\n```\n\nto track new binary use:\n```bash\naltb track path <app_name>@<app_tag> /path/to/binary\n```\nfor example:\n```bash\naltb track path python@2.7 /bin/python2.7\naltb track path python@3.8 /bin/python3.8\n# altb track path python ~/Downloads/python # will also work and generate a new hash for it\n```\n\nList all tracked versions:\n```bash\n$ altb list -a\npython\n|----   2.7 - /bin/python2.7\n|----   3.8 - /bin/python3.8\n```\n\nUse specific version:\n```bash\naltb use <app_name>[@<app_tag>]\n```\n\nexample:\n```bash\naltb use python@2.7\n```\nthis will link the tracked path to `~/.local/bin/<app_name>` in this case - `~/.local/bin/python`\n\nCopy specific standalone binary automatically to `~/.local/share/altb/versions/<app_name>/<app_name>_<tag>`\n```bash\naltb track path helm@3 ~/Downloads/helm --copy\n```\n\nYou can run custom commands using:\n```bash\naltb track command special_command@latest "echo This is a command"\n```\nthis especially useful for latest developments, example:\n```bash\naltb track command special_command@latest "go run ./cmd/special_command" --working-directory "$HOME/special_command"\n```\n\n\n## Docs\n### Migrations\n- [Migrate to v0.5.0 and above from lower versions](./docs/migrations/migrate_to_0_5_0.md)',
     'author': 'Elran Shefer',
     'author_email': 'elran777@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/IamShobe/altb',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `altb-0.5.1/PKG-INFO` & `altb-0.5.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altb
-Version: 0.5.1
+Version: 0.5.2
 Summary: Cli tool for tracking over binaries and easily swapping between them
 Home-page: https://github.com/IamShobe/altb
 License: MIT
 Author: Elran Shefer
 Author-email: elran777@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -76,7 +76,11 @@
 altb track command special_command@latest "echo This is a command"
 ```
 this especially useful for latest developments, example:
 ```bash
 altb track command special_command@latest "go run ./cmd/special_command" --working-directory "$HOME/special_command"
 ```
 
+
+## Docs
+### Migrations
+- [Migrate to v0.5.0 and above from lower versions](./docs/migrations/migrate_to_0_5_0.md)
```

