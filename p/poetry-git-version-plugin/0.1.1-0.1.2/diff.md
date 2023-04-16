# Comparing `tmp/poetry_git_version_plugin-0.1.1.tar.gz` & `tmp/poetry_git_version_plugin-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_git_version_plugin-0.1.1.tar", max compression
+gzip compressed data, was "poetry_git_version_plugin-0.1.2.tar", max compression
```

## Comparing `poetry_git_version_plugin-0.1.1.tar` & `poetry_git_version_plugin-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1055 2023-04-11 19:28:21.273926 poetry_git_version_plugin-0.1.1/LICENSE
--rw-r--r--   0        0        0        0 2023-04-12 18:36:34.455778 poetry_git_version_plugin-0.1.1/poetry_git_version_plugin/__init__.py
--rw-r--r--   0        0        0      310 2023-04-11 19:28:21.273926 poetry_git_version_plugin-0.1.1/poetry_git_version_plugin/commands.py
--rw-r--r--   0        0        0     1002 2023-04-12 18:36:34.375778 poetry_git_version_plugin-0.1.1/poetry_git_version_plugin/config.py
--rw-r--r--   0        0        0      781 2023-04-11 19:28:21.273926 poetry_git_version_plugin-0.1.1/poetry_git_version_plugin/exceptions.py
--rw-r--r--   0        0        0     1535 2023-04-11 19:28:21.273926 poetry_git_version_plugin-0.1.1/poetry_git_version_plugin/plugins.py
--rw-r--r--   0        0        0     4295 2023-04-12 18:36:34.375778 poetry_git_version_plugin-0.1.1/poetry_git_version_plugin/services.py
--rw-r--r--   0        0        0     2172 2023-04-11 19:28:21.273926 poetry_git_version_plugin-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1075 2023-04-11 19:28:21.273926 poetry_git_version_plugin-0.1.1/readme.md
--rw-r--r--   0        0        0     2721 1970-01-01 00:00:00.000000 poetry_git_version_plugin-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-04-16 19:45:04.526406 poetry_git_version_plugin-0.1.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-16 19:48:08.369382 poetry_git_version_plugin-0.1.2/poetry_git_version_plugin/__init__.py
+-rw-r--r--   0        0        0      310 2023-04-16 19:45:04.530406 poetry_git_version_plugin-0.1.2/poetry_git_version_plugin/commands.py
+-rw-r--r--   0        0        0     1250 2023-04-16 19:45:04.530406 poetry_git_version_plugin-0.1.2/poetry_git_version_plugin/config.py
+-rw-r--r--   0        0        0      758 2023-04-16 19:45:04.530406 poetry_git_version_plugin-0.1.2/poetry_git_version_plugin/exceptions.py
+-rw-r--r--   0        0        0     1461 2023-04-16 19:45:04.530406 poetry_git_version_plugin-0.1.2/poetry_git_version_plugin/plugins.py
+-rw-r--r--   0        0        0     4506 2023-04-16 19:45:04.530406 poetry_git_version_plugin-0.1.2/poetry_git_version_plugin/services.py
+-rw-r--r--   0        0        0     2228 2023-04-16 19:45:04.530406 poetry_git_version_plugin-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1077 2023-04-16 19:45:04.530406 poetry_git_version_plugin-0.1.2/readme.md
+-rw-r--r--   0        0        0     2723 1970-01-01 00:00:00.000000 poetry_git_version_plugin-0.1.2/PKG-INFO
```

### Comparing `poetry_git_version_plugin-0.1.1/LICENSE` & `poetry_git_version_plugin-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.1/poetry_git_version_plugin/config.py` & `poetry_git_version_plugin-0.1.2/poetry_git_version_plugin/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,29 +8,35 @@
 class PluginConfig(object):
     """Обертка над конфигурацией pyproject"""
 
     pyproject: PyProjectTOML
 
     _default_setting = {
         # Игнорирование отсутствия тега
-        'ignore_exception': True,
+        'ignore_errors': True,
         # Использование ref без тега
-        'use_last_tag': True,
+        'make_alpha_version': True,
+        # Использование ref без тега
+        'format_alpha_version': '{version}.a{distance}+{commit_hash}',
     }
 
     def __init__(self, pyproject: PyProjectTOML) -> None:
         self.pyproject = pyproject
 
     @property
     def settings(self):
         settings = self.pyproject.data.get('tool', {}).get(PLUGIN_NAME, {})
         new_settings = deepcopy(self._default_setting)
         new_settings.update(settings)
         return new_settings
 
     @property
-    def ignore_exception(self) -> bool:
-        return self.settings['ignore_exception']
+    def ignore_errors(self) -> bool:
+        return self.settings['ignore_errors']
+
+    @property
+    def make_alpha_version(self) -> bool:
+        return self.settings['make_alpha_version']
 
     @property
-    def use_last_tag(self) -> bool:
-        return self.settings['use_last_tag']
+    def format_alpha_version(self) -> str:
+        return self.settings['format_alpha_version']
```

### Comparing `poetry_git_version_plugin-0.1.1/poetry_git_version_plugin/exceptions.py` & `poetry_git_version_plugin-0.1.2/poetry_git_version_plugin/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class PluginException(RuntimeError):
     def __str__(self) -> str:
         if isinstance(self.args[0], BaseException):
             ex = self.args[0]
             message = ex.__class__.__name__
             if ex.args:
-                message = '{0}: {1}'.format(message, '; '.join(ex.args))
+                message = f'{message}: {ex.args}'
 
         else:
             message = '; '.join(self.args)
 
         return f'<b>{config.PLUGIN_NAME}</b>: {message}'
```

### Comparing `poetry_git_version_plugin-0.1.1/poetry_git_version_plugin/plugins.py` & `poetry_git_version_plugin-0.1.2/poetry_git_version_plugin/plugins.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,32 +15,30 @@
 class PoetryGitVersionPlugin(Plugin):
     """Плагин определения версии по гит тегу"""
 
     @plugin_exception_wrapper
     def activate(self, poetry: Poetry, io: IO):
         io.write_line(f'<b>{config.PLUGIN_NAME}</b>: Init', Verbosity.VERBOSE)
 
-        self.plugin_config = config.PluginConfig(poetry.pyproject)
+        plugin_config = config.PluginConfig(poetry.pyproject)
 
         try:
-            tag = GitVersionService(io, self.plugin_config).get_tag()
+            tag = GitVersionService(io, plugin_config).get_version()
 
         except Exception as ex:
-            if self.plugin_config.ignore_exception:
+            if plugin_config.ignore_errors:
                 if not isinstance(ex, PluginException):
                     ex = PluginException(ex)
 
-                text = f'{ex}. Ignore Exception\n'
+                io.write_error(f'{ex}. Ignore Exception\n', Verbosity.VERBOSE)
 
-                io.write_error(text, Verbosity.VERBOSE)
                 return
 
             raise ex
 
-        if tag is not None:
-            poetry.package.version = tag
+        poetry.package.version = tag
 
         io.write_line(f'<b>{config.PLUGIN_NAME}</b>: Finished\n', Verbosity.VERBOSE)
 
 
 class PoetryGitVersionApplicationPlugin(ApplicationPlugin):
     commands = [GitVersionCommand]
```

### Comparing `poetry_git_version_plugin-0.1.1/poetry_git_version_plugin/services.py` & `poetry_git_version_plugin-0.1.2/poetry_git_version_plugin/services.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
         for tag in tags:
             if tag.commit == self.repo.head.commit:
                 return tag
 
         return None
 
-    def get_git_last_tag(self) -> git.Tag:
+    def get_alpha_version(self) -> git.Tag:
         """Получение последнего тега нынешней ветки"""
 
         commits = set(self.commits)
         tags = self.tags
 
         for tag in tags:
             if tag.commit in commits:
@@ -96,54 +96,55 @@
 
     def __init__(self, io: IO, plugin_config: config.PluginConfig) -> None:
         self.io = io
         self.plugin_config = plugin_config
 
         self.git_service = GitService()
 
-    def get_git_tag(self):
-        self.io.write(f'<b>{config.PLUGIN_NAME}</b>: Find git <b>current tag</b>... ', verbosity=Verbosity.VERBOSE)
+    def construct_alpha_version(self, version: str, distance: str, commit_hash: str):
+        return self.plugin_config.format_alpha_version.format(
+            version=version,
+            distance=distance,
+            commit_hash=commit_hash,
+        )
 
+    def get_main_version(self) -> str:
         tag = self.git_service.get_git_current_tag()
+        return tag.name if tag is not None else None
 
-        if tag is None:
-            self.io.write_line('fail', Verbosity.VERBOSE)
-            return None
+    def get_alpha_version(self):
+        tag = self.git_service.get_alpha_version()
 
-        self.io.write_line(f'success, setting dynamic version to: {tag.name}', Verbosity.VERBOSE)
+        version = '0.0.0'
+        distance_from_commit = self.git_service.commits[-1]
 
-        return tag.name
+        if tag is not None:
+            distance_from_commit = tag.commit
+            version = str(tag)
 
-    def get_git_last_tag(self):
-        self.io.write(f'<b>{config.PLUGIN_NAME}</b>: Find git <b>last tag</b>... ', verbosity=Verbosity.VERBOSE)
+        distance = self.git_service.get_distance(distance_from_commit, self.git_service.current_commit)
+        commit_hash = self.git_service.get_current_short_rev()
 
-        tag = self.git_service.get_git_last_tag()
+        return self.construct_alpha_version(version, distance, commit_hash)
 
-        if tag is None:
-            first_commit = self.git_service.commits[-1]
-            distance = self.git_service.get_distance(first_commit, self.git_service.current_commit)
+    @validate_version_decorator
+    def get_version(self) -> str:
+        self.io.write(f'<b>{config.PLUGIN_NAME}</b>: Find git <b>current tag</b>... ', verbosity=Verbosity.VERBOSE)
 
-            tag = f'0.0.1+{distance}-{self.git_service.get_current_short_rev()}'
+        version = self.get_main_version()
 
-        else:
-            distance = self.git_service.get_distance(tag.commit, self.git_service.current_commit)
+        if version is not None:
+            self.io.write_line(f'success, setting dynamic version to: {version}', Verbosity.VERBOSE)
+            return version
 
-            tag = f'{tag}+{distance}-{self.git_service.get_current_short_rev()}'
+        self.io.write_line('fail', Verbosity.VERBOSE)
 
-        self.io.write_line(f'success, setting dynamic version to: {tag}', Verbosity.VERBOSE)
+        if not self.plugin_config.make_alpha_version:
+            raise PluginException('No Git version found, not extracting dynamic version')
 
-        return tag
+        self.io.write(f'<b>{config.PLUGIN_NAME}</b>: Make <b>alpha version</b>... ', verbosity=Verbosity.VERBOSE)
 
-    @validate_version_decorator
-    def get_tag(self) -> str:
-        tag = self.get_git_tag()
+        tag = self.get_alpha_version()
 
-        if tag is not None:
-            return tag
-
-        if self.plugin_config.use_last_tag:
-            tag = self.get_git_last_tag()
-
-        if tag is not None:
-            return tag
+        self.io.write_line(f'success, setting dynamic version to: {tag}', Verbosity.VERBOSE)
 
-        raise PluginException('No Git version found, not extracting dynamic version')
+        return tag
```

### Comparing `poetry_git_version_plugin-0.1.1/pyproject.toml` & `poetry_git_version_plugin-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 poetry-git-version-plugin = "poetry_git_version_plugin.plugins:PoetryGitVersionPlugin"
 
 [tool.poetry.plugins."poetry.application.plugin"]
 poetry-git-version-plugin = "poetry_git_version_plugin.plugins:PoetryGitVersionApplicationPlugin"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-poetry = "^1.3.2"
+poetry = "^1.2.2"
 gitpython = "^3.1.29"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 ruff = "^0.0.260"
 black = "^23.3.0"
@@ -66,8 +66,11 @@
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "def __repr__",
     "raise AssertionError",
     "raise NotImplementedError",
     "if __name__ == .__main__.:",
-]
+]
+
+[tool.poetry-git-version-plugin]
+ignore_errors = false
```

### Comparing `poetry_git_version_plugin-0.1.1/readme.md` & `poetry_git_version_plugin-0.1.2/readme.md`

 * *Files 24% similar despite different names*

```diff
@@ -17,29 +17,29 @@
 poetry -v git-version # print process
 ```
 
 ## Dependencies
 
 ```toml
 [tool.poetry.dependencies]
-python = ">=3.10"
+python = ">=3.7"
 poetry = ">=1.2.0"
 ```
 
 ## Setup
 
 ```toml
 [tool.poetry-git-version-plugin]
 # Ignore "tag missing" errors
-ignore_exception = true
+ignore_errors = true
 
 # If the tag is missing.
 # Returns a version, computed from the latest version tag.
 # It takes the version tag, increases the version tag by the number of commits since, adds a local label specifying the git commit hash and the dirty status.
 # Example: 1.3.2+5-5babef6
-use_last_tag = true
+make_alpha_version = true
 ```
 
 ## Contribute
 
 Issue Tracker: <https://gitlab.com/rocshers/python/poetry-git-version-plugin/-/issues>  
 Source Code: <https://gitlab.com/rocshers/python/poetry-git-version-plugin>
```

### Comparing `poetry_git_version_plugin-0.1.1/PKG-INFO` & `poetry_git_version_plugin-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-git-version-plugin
-Version: 0.1.1
+Version: 0.1.2
 Summary: Poetry plugin to get package version from git
 Home-page: https://gitlab.com/rocshers/python/poetry-git-version-plugin
 License: MIT
 Author: irocshers
 Author-email: develop.iam@rocshers.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -26,15 +26,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Software Distribution
 Requires-Dist: gitpython (>=3.1.29,<4.0.0)
-Requires-Dist: poetry (>=1.3.2,<2.0.0)
+Requires-Dist: poetry (>=1.2.2,<2.0.0)
 Project-URL: Repository, https://gitlab.com/rocshers/python/poetry-git-version-plugin
 Description-Content-Type: text/markdown
 
 # Poetry Git Version Plugin
 
 Poetry plugin to get package version from git.
 
@@ -53,30 +53,30 @@
 poetry -v git-version # print process
 ```
 
 ## Dependencies
 
 ```toml
 [tool.poetry.dependencies]
-python = ">=3.10"
+python = ">=3.7"
 poetry = ">=1.2.0"
 ```
 
 ## Setup
 
 ```toml
 [tool.poetry-git-version-plugin]
 # Ignore "tag missing" errors
-ignore_exception = true
+ignore_errors = true
 
 # If the tag is missing.
 # Returns a version, computed from the latest version tag.
 # It takes the version tag, increases the version tag by the number of commits since, adds a local label specifying the git commit hash and the dirty status.
 # Example: 1.3.2+5-5babef6
-use_last_tag = true
+make_alpha_version = true
 ```
 
 ## Contribute
 
 Issue Tracker: <https://gitlab.com/rocshers/python/poetry-git-version-plugin/-/issues>  
 Source Code: <https://gitlab.com/rocshers/python/poetry-git-version-plugin>
```

