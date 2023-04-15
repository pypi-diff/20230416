# Comparing `tmp/buildarr-0.4.2.tar.gz` & `tmp/buildarr-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildarr-0.4.2.tar", max compression
+gzip compressed data, was "buildarr-0.5.0.tar", max compression
```

## Comparing `buildarr-0.4.2.tar` & `buildarr-0.5.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0    35149 2023-04-14 10:03:59.115044 buildarr-0.4.2/LICENSE
--rw-r--r--   0        0        0    14660 2023-04-14 10:03:59.115044 buildarr-0.4.2/README.md
--rw-r--r--   0        0        0      946 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/__init__.py
--rw-r--r--   0        0        0     1783 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/cli/__init__.py
--rw-r--r--   0        0        0    11235 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/cli/compose.py
--rw-r--r--   0        0        0    17974 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/cli/daemon.py
--rw-r--r--   0        0        0     2521 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/cli/exceptions.py
--rw-r--r--   0        0        0     1254 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/cli/main.py
--rw-r--r--   0        0        0    15480 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/cli/run.py
--rw-r--r--   0        0        0     9627 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/cli/test_config.py
--rw-r--r--   0        0        0     1402 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/config/__init__.py
--rw-r--r--   0        0        0    34135 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/config/base.py
--rw-r--r--   0        0        0     5429 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/config/buildarr.py
--rw-r--r--   0        0        0     1071 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/config/exceptions.py
--rw-r--r--   0        0        0     7213 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/config/load.py
--rw-r--r--   0        0        0    10724 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/config/models.py
--rw-r--r--   0        0        0     2006 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/config/render_instance_configs.py
--rw-r--r--   0        0        0     5338 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/config/resolve_instance_dependencies.py
--rw-r--r--   0        0        0     2164 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/config/types.py
--rw-r--r--   0        0        0      827 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/exceptions.py
--rw-r--r--   0        0        0     3046 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/logging.py
--rw-r--r--   0        0        0     9394 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/manager/__init__.py
--rw-r--r--   0        0        0      877 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/manager/exceptions.py
--rw-r--r--   0        0        0      872 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/dummy/__init__.py
--rw-r--r--   0        0        0     8838 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/dummy/api.py
--rw-r--r--   0        0        0     2922 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/dummy/cli.py
--rw-r--r--   0        0        0     7264 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/dummy/config/__init__.py
--rw-r--r--   0        0        0     7783 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/dummy/config/settings.py
--rw-r--r--   0        0        0     1184 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/dummy/config/types.py
--rw-r--r--   0        0        0     1178 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/dummy/exceptions.py
--rw-r--r--   0        0        0      932 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/dummy/manager.py
--rw-r--r--   0        0        0     1160 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/dummy/plugin.py
--rw-r--r--   0        0        0     3570 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/dummy/secrets.py
--rw-r--r--   0        0        0     5934 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/dummy/server.py
--rw-r--r--   0        0        0     1386 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/dummy/types.py
--rw-r--r--   0        0        0     2236 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/load.py
--rw-r--r--   0        0        0     3728 2023-04-14 10:03:59.119044 buildarr-0.4.2/buildarr/plugins/models.py
--rw-r--r--   0        0        0     1239 2023-04-14 10:03:59.119044 buildarr-0.4.2/buildarr/plugins/types.py
--rw-r--r--   0        0        0        0 2023-04-14 10:03:59.119044 buildarr-0.4.2/buildarr/py.typed
--rw-r--r--   0        0        0      925 2023-04-14 10:03:59.119044 buildarr-0.4.2/buildarr/secrets/__init__.py
--rw-r--r--   0        0        0     2807 2023-04-14 10:03:59.119044 buildarr-0.4.2/buildarr/secrets/base.py
--rw-r--r--   0        0        0     2466 2023-04-14 10:03:59.119044 buildarr-0.4.2/buildarr/secrets/load.py
--rw-r--r--   0        0        0     3723 2023-04-14 10:03:59.119044 buildarr-0.4.2/buildarr/secrets/models.py
--rw-r--r--   0        0        0     7334 2023-04-14 10:03:59.119044 buildarr-0.4.2/buildarr/state.py
--rw-r--r--   0        0        0     5321 2023-04-14 10:03:59.119044 buildarr-0.4.2/buildarr/trash.py
--rw-r--r--   0        0        0    15383 2023-04-14 10:03:59.119044 buildarr-0.4.2/buildarr/types.py
--rw-r--r--   0        0        0     4183 2023-04-14 10:03:59.119044 buildarr-0.4.2/buildarr/util.py
--rw-r--r--   0        0        0     2326 2023-04-14 10:03:59.119044 buildarr-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    16162 1970-01-01 00:00:00.000000 buildarr-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-15 22:02:11.338667 buildarr-0.5.0/LICENSE
+-rw-r--r--   0        0        0    14526 2023-04-15 22:02:11.338667 buildarr-0.5.0/README.md
+-rw-r--r--   0        0        0      946 2023-04-15 22:02:11.338667 buildarr-0.5.0/buildarr/__init__.py
+-rw-r--r--   0        0        0     1783 2023-04-15 22:02:11.338667 buildarr-0.5.0/buildarr/cli/__init__.py
+-rw-r--r--   0        0        0    11235 2023-04-15 22:02:11.338667 buildarr-0.5.0/buildarr/cli/compose.py
+-rw-r--r--   0        0        0    17974 2023-04-15 22:02:11.338667 buildarr-0.5.0/buildarr/cli/daemon.py
+-rw-r--r--   0        0        0     2521 2023-04-15 22:02:11.338667 buildarr-0.5.0/buildarr/cli/exceptions.py
+-rw-r--r--   0        0        0     1254 2023-04-15 22:02:11.338667 buildarr-0.5.0/buildarr/cli/main.py
+-rw-r--r--   0        0        0    14761 2023-04-15 22:02:11.338667 buildarr-0.5.0/buildarr/cli/run.py
+-rw-r--r--   0        0        0     8847 2023-04-15 22:02:11.338667 buildarr-0.5.0/buildarr/cli/test_config.py
+-rw-r--r--   0        0        0     1402 2023-04-15 22:02:11.338667 buildarr-0.5.0/buildarr/config/__init__.py
+-rw-r--r--   0        0        0    34077 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/config/base.py
+-rw-r--r--   0        0        0     5429 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/config/buildarr.py
+-rw-r--r--   0        0        0     1071 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/config/exceptions.py
+-rw-r--r--   0        0        0     7213 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/config/load.py
+-rw-r--r--   0        0        0    10224 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/config/models.py
+-rw-r--r--   0        0        0     2006 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/config/render_instance_configs.py
+-rw-r--r--   0        0        0     5338 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/config/resolve_instance_dependencies.py
+-rw-r--r--   0        0        0     2164 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/config/types.py
+-rw-r--r--   0        0        0      827 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/exceptions.py
+-rw-r--r--   0        0        0     3046 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/logging.py
+-rw-r--r--   0        0        0     8828 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/manager/__init__.py
+-rw-r--r--   0        0        0      877 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/manager/exceptions.py
+-rw-r--r--   0        0        0      872 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/plugins/dummy/__init__.py
+-rw-r--r--   0        0        0     9319 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/plugins/dummy/api.py
+-rw-r--r--   0        0        0     2922 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/plugins/dummy/cli.py
+-rw-r--r--   0        0        0     5814 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/plugins/dummy/config/__init__.py
+-rw-r--r--   0        0        0     7504 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/plugins/dummy/config/settings.py
+-rw-r--r--   0        0        0     1186 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/plugins/dummy/config/types.py
+-rw-r--r--   0        0        0     1360 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/plugins/dummy/exceptions.py
+-rw-r--r--   0        0        0      932 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/plugins/dummy/manager.py
+-rw-r--r--   0        0        0     1160 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/plugins/dummy/plugin.py
+-rw-r--r--   0        0        0     4047 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/plugins/dummy/secrets.py
+-rw-r--r--   0        0        0     5934 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/plugins/dummy/server.py
+-rw-r--r--   0        0        0     1386 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/plugins/dummy/types.py
+-rw-r--r--   0        0        0     2236 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/plugins/load.py
+-rw-r--r--   0        0        0     3728 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/plugins/models.py
+-rw-r--r--   0        0        0     1239 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/plugins/types.py
+-rw-r--r--   0        0        0        0 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/py.typed
+-rw-r--r--   0        0        0      925 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/secrets/__init__.py
+-rw-r--r--   0        0        0     2663 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/secrets/base.py
+-rw-r--r--   0        0        0     2466 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/secrets/load.py
+-rw-r--r--   0        0        0     3723 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/secrets/models.py
+-rw-r--r--   0        0        0     7653 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/state.py
+-rw-r--r--   0        0        0     3725 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/trash.py
+-rw-r--r--   0        0        0    14582 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/types.py
+-rw-r--r--   0        0        0     4183 2023-04-15 22:02:11.342667 buildarr-0.5.0/buildarr/util.py
+-rw-r--r--   0        0        0     2326 2023-04-15 22:02:11.342667 buildarr-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    16028 1970-01-01 00:00:00.000000 buildarr-0.5.0/PKG-INFO
```

### Comparing `buildarr-0.4.2/LICENSE` & `buildarr-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/README.md` & `buildarr-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,14 @@
 2023-02-22 21:21:27,223 buildarr:1 buildarr.main [INFO] Buildarr ready.
 ```
 
 For more information on how to interfact with Buildarr, check the [usage documentation](https://buildarr.github.io/usage).
 
 ## To-do list
 
-* Add a dry-run mode for testing configurations (added in [version 0.4.0](https://buildarr.github.io/release-notes/#v040-2023-03-31))
 * Test updates for all available attributes in the existing Sonarr plugin
 * Unit tests and code coverage
 * Split Sonarr plugin to its own repository (completed in [version 0.4.0](https://buildarr.github.io/release-notes/#v040-2023-03-31))
 * Create plugins for the following applications:
     * Sonarr V4
     * Radarr
     * Prowlarr (now available as [`buildarr-prowlarr`](https://buildarr.github.io/plugins/prowlarr))
```

### Comparing `buildarr-0.4.2/buildarr/__init__.py` & `buildarr-0.5.0/buildarr/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/cli/__init__.py` & `buildarr-0.5.0/buildarr/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/cli/compose.py` & `buildarr-0.5.0/buildarr/cli/compose.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/cli/daemon.py` & `buildarr-0.5.0/buildarr/cli/daemon.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/cli/exceptions.py` & `buildarr-0.5.0/buildarr/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/cli/main.py` & `buildarr-0.5.0/buildarr/cli/main.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/cli/run.py` & `buildarr-0.5.0/buildarr/cli/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     render_instance_configs,
     resolve_instance_dependencies,
 )
 from ..logging import get_log_level
 from ..manager import load_managers
 from ..secrets import load_secrets
 from ..state import state
-from ..trash import fetch_trash_metadata, render_trash_metadata, trash_metadata_used
+from ..trash import fetch_trash_metadata, trash_metadata_used
 from ..util import get_resolved_path
 from . import cli
 from .exceptions import RunInstanceConnectionTestFailedError, RunNoPluginsDefinedError
 
 if TYPE_CHECKING:
     from typing import Dict, Optional, Set
 
@@ -88,22 +88,14 @@
     help=(
         "Read secrets metadata from (and write back to) the specified JSON file. "
         "If unspecified, use the value from the configuration file, "
         "and if undefined there, default to `secrets.json'."
     ),
 )
 @click.option(
-    "-D",
-    "--dry-run",
-    "dry_run",
-    is_flag=True,
-    default=False,
-    help="Enable dry-run mode. Update runs are executed, but instances are not modified.",
-)
-@click.option(
     "-p",
     "--plugin",
     "use_plugins",
     metavar="PLUGIN",
     type=str,
     callback=lambda ctx, params, plugins: set(plugins),
     multiple=True,
@@ -111,34 +103,26 @@
         "Use only the specified Buildarr plugin. Default is to use all installed plugins. "
         "(can be defined multiple times)"
     ),
 )
 def run(
     config_path: Path,
     secrets_file_path: Optional[Path],
-    dry_run: bool,
     use_plugins: Set[str],
 ) -> None:
     """
     `buildarr run` main routine.
 
     Args:
         config_path (Path): Configuration file to load.
-        dry_run (bool): If set to `True`, run in dry-run mode.
         plugins (Set[str]): Plugins to load. If empty, use all plugins.
     """
 
     logger.info("Buildarr version %s (log level: %s)", __version__, get_log_level())
 
-    if dry_run:
-        logger.info(
-            "Dry-run mode enabled: executing update runs, but will not modify instances",
-        )
-        state.dry_run = True
-
     logger.info("Loading configuration file '%s'", config_path)
     load_config(path=config_path, use_plugins=use_plugins)
     logger.info("Finished loading configuration file")
 
     if not secrets_file_path:
         secrets_file_path = state.config.buildarr.secrets_file_path
 
@@ -201,20 +185,16 @@
     logger.info("Finished resolving instance dependencies")
 
     # Render dynamically populated attributes in instance configurations,
     # with the TRaSH-Guides metadata directory available in the global state
     # only if at least one instance configuration requires it.
     if trash_metadata_used():
         logger.info("Fetching TRaSH metadata")
-        with fetch_trash_metadata() as trash_metadata_dir:
-            # TODO: Remove `render_trash_metadata` in Buildarr v0.5.0.
+        with fetch_trash_metadata():
             logger.info("Finished fetching TRaSH metadata")
-            logger.info("Rendering TRaSH metadata")
-            render_trash_metadata(trash_metadata_dir)
-            logger.info("Finished rendering TRaSH metadata")
             logger.info("Rendering instance configuration dynamic attributes")
             render_instance_configs()
             logger.info("Finished rendering instance configuration dynamic attributes")
     else:
         logger.info("Rendering instance configuration dynamic attributes")
         render_instance_configs()
         logger.info("Finished rendering instance configuration dynamic attributes")
```

### Comparing `buildarr-0.4.2/buildarr/cli/test_config.py` & `buildarr-0.5.0/buildarr/cli/test_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     load_instance_configs,
     render_instance_configs,
     resolve_instance_dependencies,
 )
 from ..logging import get_log_level
 from ..manager import load_managers
 from ..state import state
-from ..trash import fetch_trash_metadata, render_trash_metadata
+from ..trash import fetch_trash_metadata
 from ..util import get_resolved_path
 from . import cli
 from .exceptions import TestConfigNoPluginsDefinedError
 
 if TYPE_CHECKING:
     from typing import Set
 
@@ -50,16 +50,14 @@
 
 @cli.command(
     help=(
         "Test a Buildarr configuration file for correctness.\n\n"
         "This loads the configuration file and performs a number of checks on it. "
         "If all tests pass, the file is pretty much guaranteed to work properly "
         "in a Buildarr run, incorrect values for a remote instance notwithstanding.\n\n"
-        "To validate the configuration against remote instances without modifying them, "
-        "use `buildarr run --dry-run'.\n\n"
         "If CONFIG-PATH is not defined, use `buildarr.yml' from the current directory."
     ),
 )
 @click.argument(
     "config_path",
     metavar="[CONFIG-PATH]",
     type=click.Path(
@@ -177,28 +175,18 @@
     # with the TRaSH-Guides metadata available.
     # If the configuration reports that TRaSH-Guides metadata is not required,
     # run the test without fetching it.
     if uses_trash_metadata:
         fetching_metadata = True
         try:
             logger.debug("Fetching TRaSH metadata")
-            with fetch_trash_metadata() as trash_metadata_dir:
+            with fetch_trash_metadata():
                 logger.debug("Finished fetching TRaSH metadata")
                 logger.info("Fetching TRaSH-Guides metadata: PASSED")
                 fetching_metadata = False
-                # TODO: Remove `render_trash_metadata` in Buildarr v0.5.0.
-                try:
-                    logger.debug("Rendering TRaSH metadata")
-                    render_trash_metadata(trash_metadata_dir)
-                    logger.debug("Finished rendering TRaSH metadata")
-                except Exception:
-                    logger.error("Rendering TRaSH-Guides metadata: FAILED")
-                    raise
-                else:
-                    logger.info("Rendering TRaSH-Guides metadata: PASSED")
                 try:
                     logger.debug("Rendering instance configuration dynamic attributes")
                     render_instance_configs()
                     logger.debug("Finished rendering instance configuration dynamic attributes")
                 except Exception:
                     logger.error("Rendering instance configuration dynamic attributes: FAILED")
                     raise
@@ -206,15 +194,14 @@
                     logger.info("Rendering instance configuration dynamic attributes: PASSED")
         except Exception:
             if fetching_metadata:
                 logger.error("Fetching TRaSH-Guides metadata: FAILED")
             raise
     else:
         logger.info("Fetching TRaSH-Guides metadata: SKIPPED (not required)")
-        logger.info("Rendering TRaSH-Guides metadata: SKIPPED (not required)")
         try:
             logger.debug("Rendering instance configuration dynamic attributes")
             render_instance_configs()
             logger.debug("Finished rendering instance configuration dynamic attributes")
         except Exception:
             logger.error("Rendering instance configuration dynamic attributes: FAILED")
             raise
```

### Comparing `buildarr-0.4.2/buildarr/config/__init__.py` & `buildarr-0.5.0/buildarr/config/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/config/base.py` & `buildarr-0.5.0/buildarr/config/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 import yaml
 
 from pydantic import AnyUrl, BaseModel, SecretStr
 from pydantic.validators import _VALIDATORS
 from typing_extensions import Self
 
 from ..plugins import Secrets
-from ..types import BaseEnum, BaseIntEnum, ModelConfigBase
+from ..types import BaseEnum, ModelConfigBase
 from .types import RemoteMapEntry
 
 logger = getLogger(__name__)
 
 OPTIONAL_TYPE_UNION_SIZE = 2
 
 
@@ -677,15 +677,15 @@
 
         Args:
             value (Any): Value to format
 
         Returns:
             The value to pass to the logging function
         """
-        if isinstance(value, (BaseEnum, BaseIntEnum)):
+        if isinstance(value, BaseEnum):
             return value.to_name_str()
         elif isinstance(value, AnyUrl):
             return str(value)
         elif isinstance(value, SecretStr):
             return str(value)
         elif isinstance(value, Path):
             return str(value)
@@ -730,30 +730,30 @@
                 and type(None) in attr_union_types
                 and value is not None
             ):
                 return cls._decode_attr(
                     [t for t in attr_union_types if t is not type(None)][0],
                     value,
                 )
-        elif issubclass(type_tree[-1], (BaseEnum, BaseIntEnum)):
+        elif issubclass(type_tree[-1], BaseEnum):
             return type_tree[-1](value)
         return value
 
     @classmethod
     def _encode_attr(cls, value: Any) -> Any:
         """
         Default local-to-remote instance attribute encoding function.
 
         Args:
             value (Any): Local attribute value
 
         Returns:
             Remote attribute value
         """
-        if isinstance(value, (BaseEnum, BaseIntEnum)):
+        if isinstance(value, BaseEnum):
             return value.value
         elif isinstance(value, AnyUrl):
             return str(value)
         elif isinstance(value, SecretStr):
             return value.get_secret_value()
         elif isinstance(value, UUID):
             return str(value)
```

### Comparing `buildarr-0.4.2/buildarr/config/buildarr.py` & `buildarr-0.5.0/buildarr/config/buildarr.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/config/exceptions.py` & `buildarr-0.5.0/buildarr/config/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/config/load.py` & `buildarr-0.5.0/buildarr/config/load.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/config/models.py` & `buildarr-0.5.0/buildarr/config/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 """
 Buildarr plugin configuration object models.
 """
 
 
 from __future__ import annotations
 
-from pathlib import Path
 from typing import Any, Dict, Type, cast
 
 from pydantic import root_validator
 from typing_extensions import Self
 
 from ..plugins import Secrets
 from ..types import NonEmptyStr, Port
@@ -123,22 +122,22 @@
     @property
     def host_url(self) -> str:
         """
         Fully qualified URL for the instance.
         """
         return f"{self.protocol}://{self.hostname}:{self.port}"
 
-    @property
     def uses_trash_metadata(self) -> bool:
         """
-        A flag determining whether or not this configuration uses TRaSH-Guides metadata.
+        Return whether or not this instance configuration uses TRaSH-Guides metadata.
 
-        Configuration plugins should implement this property if TRaSH-Guides metadata is used.
+        Configuration plugins should implement this function if TRaSH-Guides metadata is used.
 
-        This property is checked by the `ManagerPlugin.uses_trash_metadata()` function.
+        Returns:
+            `True` if TRaSH-Guides metadata is used, otherwise `False`
         """
         return False
 
     @property
     def has_instance_configs(self) -> bool:
         """
         Whether or not this plugin has instance-specific configurations defined.
@@ -180,28 +179,14 @@
                 self.instances[instance_name].dict(  # type: ignore[attr-defined]
                     exclude=set(["instances"]),
                     exclude_unset=True,
                 ),
             ),
         )
 
-    def render_trash_metadata(self, trash_metadata_dir: Path) -> Self:
-        """
-        Read TRaSH-Guides metadata, and return a configuration object with all templates rendered.
-
-        Configuration plugins should implement this function if TRaSH-Guides metadata is used.
-
-        Args:
-            trash_metadata_dir (Path): TRaSH-Guides metadata directory.
-
-        Returns:
-            Rendered configuration object
-        """
-        return self
-
     def render(self) -> Self:
         """
         Render any dynamically populated attributes in this instance configuration.
 
         Configuration plugins should implement this function if there are any attributes
         that get dynamically populated, e.g. TRaSH-Guides metadata.
```

### Comparing `buildarr-0.4.2/buildarr/config/render_instance_configs.py` & `buildarr-0.5.0/buildarr/config/render_instance_configs.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/config/resolve_instance_dependencies.py` & `buildarr-0.5.0/buildarr/config/resolve_instance_dependencies.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/config/types.py` & `buildarr-0.5.0/buildarr/config/types.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/exceptions.py` & `buildarr-0.5.0/buildarr/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/logging.py` & `buildarr-0.5.0/buildarr/logging.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/manager/__init__.py` & `buildarr-0.5.0/buildarr/manager/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from logging import getLogger
 from typing import TYPE_CHECKING, Generic
 
 from ..plugins import Config, Secrets
 from ..state import state
 
 if TYPE_CHECKING:
-    from pathlib import Path
     from typing import Any, Dict, Optional, Set
 
 
 logger = getLogger(__name__)
 
 
 class ManagerPlugin(Generic[Config, Secrets]):
@@ -83,29 +82,15 @@
 
         Args:
             instance_config (Config): Instance configuration object to check.
 
         Returns:
             `True` if TRaSH-Guides metadata is used, otherwise `False`
         """
-        return instance_config.uses_trash_metadata
-
-    def render_trash_metadata(self, instance_config: Config, trash_metadata_dir: Path) -> Config:
-        """
-        Read TRaSH-Guides metadata, and return an instance configuration object
-        with all templates rendered.
-
-        Args:
-            instance_config (Config): Instance configuration object to render.
-            trash_metadata_dir (Path): TRaSH-Guides metadata directory.
-
-        Returns:
-            Rendered configuration object
-        """
-        return instance_config.render_trash_metadata(trash_metadata_dir)
+        return instance_config.uses_trash_metadata()
 
     def render(self, instance_config: Config) -> Config:
         """
         Render dynamically populated attributes on the given instance configuration.
 
         If the instance configuration returned `True` for `uses_trash_metadata`,
         the filepath to the downloaded metadata directory will be available as
```

### Comparing `buildarr-0.4.2/buildarr/manager/exceptions.py` & `buildarr-0.5.0/buildarr/manager/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/plugins/__init__.py` & `buildarr-0.5.0/buildarr/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/plugins/dummy/api.py` & `buildarr-0.5.0/buildarr/plugins/dummy/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,28 +18,27 @@
 
 
 from __future__ import annotations
 
 import json
 import re
 
-from datetime import datetime, timezone
 from http import HTTPStatus
 from logging import getLogger
 from typing import TYPE_CHECKING
 
 import json5  # type: ignore[import]
 import requests
 
 from buildarr.state import state
 
 from .exceptions import DummyAPIError
 
 if TYPE_CHECKING:
-    from typing import Any, Dict, Mapping, Optional
+    from typing import Any, Dict, Optional, Union
 
     from .secrets import DummySecrets
 
 
 logger = getLogger(__name__)
 
 INITIALIZE_JS_RES_PATTERN = re.compile(r"(?s)^window\.Dummy = ({.*});$")
@@ -54,141 +53,228 @@
         api_key (str): Dummy instance API key, if required. Defaults to `None`.
 
     Returns:
         Session initialisation metadata
     """
 
     url = f"{host_url}/initialize.js"
+
     logger.debug("GET %s", url)
+
     res = requests.get(
         url,
         headers={"X-Api-Key": api_key} if api_key else None,
         timeout=state.config.buildarr.request_timeout,
+        allow_redirects=False,
     )
+
+    if res.status_code != HTTPStatus.OK:
+        logger.debug("GET %s -> status_code=%i res=%s", url, res.status_code, res.text)
+        if res.status_code in (HTTPStatus.UNAUTHORIZED, HTTPStatus.FOUND):
+            status_code: int = HTTPStatus.UNAUTHORIZED
+            error_message = "Unauthorized"
+        else:
+            status_code = res.status_code
+            error_message = f"Unexpected response with error code {res.status_code}: {res.text}"
+        raise DummyAPIError(
+            f"Unable to retrieve 'initialize.js': {error_message}",
+            status_code=status_code,
+        )
+
     res_match = re.match(INITIALIZE_JS_RES_PATTERN, res.text)
     if not res_match:
-        raise RuntimeError(f"No matches for initialize.js parsing: {res.text}")
+        raise RuntimeError(f"No matches for 'initialize.js' parsing: {res.text}")
     res_json = json5.loads(res_match.group(1))
+
     logger.debug("GET %s -> status_code=%i res=%s", url, res.status_code, repr(res_json))
+
     return res_json
 
 
-def api_get(secrets: DummySecrets, api_url: str) -> Any:
+def api_get(
+    secrets: Union[DummySecrets, str],
+    api_url: str,
+    session: Optional[requests.Session] = None,
+    use_api_key: bool = True,
+    expected_status_code: HTTPStatus = HTTPStatus.OK,
+) -> Any:
     """
     Send a `GET` request to a Dummy instance.
 
     Args:
-        secrets (DummySecrets): Dummy secrets metadata
-        api_url (str): Dummy API command
+        secrets (Union[DummySecrets, str]): Dummy secrets metadata, or host URL.
+        api_url (str): Dummy API command.
+        expected_status_code (HTTPStatus): Expected response status. Defaults to `200 OK`.
 
     Returns:
         Response object
     """
 
-    url = f"{secrets.host_url}/{api_url.lstrip('/')}"
+    if isinstance(secrets, str):
+        host_url = secrets
+        api_key = None
+    else:
+        host_url = secrets.host_url
+        api_key = secrets.api_key.get_secret_value() if use_api_key else None
+    url = f"{host_url}/{api_url.lstrip('/')}"
+
     logger.debug("GET %s", url)
-    res = requests.get(
+
+    if not session:
+        session = requests.Session()
+    res = session.get(
         url,
-        headers={"X-Api-Key": secrets.api_key.get_secret_value()},
-        timeout=state.config.buildarr.request_timeout,
+        headers={"X-Api-Key": api_key} if api_key else None,
+        timeout=state.request_timeout,
     )
     res_json = res.json()
+
     logger.debug("GET %s -> status_code=%i res=%s", url, res.status_code, repr(res_json))
-    if res.status_code != HTTPStatus.OK:
+
+    if res.status_code != expected_status_code:
         api_error(method="GET", url=url, response=res)
+
     return res_json
 
 
-def api_post(secrets: DummySecrets, api_url: str, req: Any) -> Any:
+def api_post(
+    secrets: Union[DummySecrets, str],
+    api_url: str,
+    req: Any = None,
+    session: Optional[requests.Session] = None,
+    use_api_key: bool = True,
+    expected_status_code: HTTPStatus = HTTPStatus.CREATED,
+) -> Any:
     """
     Send a `POST` request to a Dummy instance.
 
     Args:
-        secrets (DummySecrets): Dummy secrets metadata
-        api_url (str): Dummy API command
-        req (Any): Request (JSON-serialisable)
+        secrets (Union[DummySecrets, str]): Dummy secrets metadata, or host URL.
+        api_url (str): Dummy API command.
+        req (Any): Request (JSON-serialisable).
+        expected_status_code (HTTPStatus): Expected response status. Defaults to `201 Created`.
 
     Returns:
         Response object
     """
 
-    url = f"{secrets.host_url}/{api_url.lstrip('/')}"
-    logger.debug("POST %s <- req=%s", url, repr(req))
-    headers = {"X-Api-Key": secrets.api_key.get_secret_value()}
-    if not state.dry_run:
-        res = requests.post(
-            url,
-            headers=headers,
-            json=req,
-            timeout=state.config.buildarr.request_timeout,
-        )
+    if isinstance(secrets, str):
+        host_url = secrets
+        api_key = None
     else:
-        res = _create_dryrun_response("POST", url, content=json.dumps(req))
+        host_url = secrets.host_url
+        api_key = secrets.api_key.get_secret_value() if use_api_key else None
+    url = f"{host_url}/{api_url.lstrip('/')}"
+
+    logger.debug("POST %s <- req=%s", url, repr(req))
+
+    if not session:
+        session = requests.Session()
+    res = session.post(
+        url,
+        headers={"X-Api-Key": api_key} if api_key else None,
+        timeout=state.request_timeout,
+        **({"json": req} if req is not None else {}),
+    )
     res_json = res.json()
+
     logger.debug("POST %s -> status_code=%i res=%s", url, res.status_code, repr(res_json))
-    if res.status_code != HTTPStatus.CREATED:
+
+    if res.status_code != expected_status_code:
         api_error(method="POST", url=url, response=res)
+
     return res_json
 
 
-def api_put(secrets: DummySecrets, api_url: str, req: Any) -> Any:
+def api_put(
+    secrets: Union[DummySecrets, str],
+    api_url: str,
+    req: Any,
+    session: Optional[requests.Session] = None,
+    use_api_key: bool = True,
+    expected_status_code: HTTPStatus = HTTPStatus.OK,
+) -> Any:
     """
     Send a `PUT` request to a Dummy instance.
 
     Args:
-        secrets (DummySecrets): Dummy secrets metadata
-        api_url (str): Dummy API command
-        req (Any): Request (JSON-serialisable)
+        secrets (Union[DummySecrets, str]): Dummy secrets metadata, or host URL.
+        api_url (str): Dummy API command.
+        req (Any): Request (JSON-serialisable).
+        expected_status_code (HTTPStatus): Expected response status. Defaults to `200 OK`.
 
     Returns:
         Response object
     """
 
-    url = f"{secrets.host_url}/{api_url.lstrip('/')}"
-    logger.debug("PUT %s <- req=%s", url, repr(req))
-    headers = {"X-Api-Key": secrets.api_key.get_secret_value()}
-    if not state.dry_run:
-        res = requests.put(
-            url,
-            headers=headers,
-            json=req,
-            timeout=state.config.buildarr.request_timeout,
-        )
+    if isinstance(secrets, str):
+        host_url = secrets
+        api_key = None
     else:
-        res = _create_dryrun_response("PUT", url, content=json.dumps(req))
+        host_url = secrets.host_url
+        api_key = secrets.api_key.get_secret_value() if use_api_key else None
+    url = f"{host_url}/{api_url.lstrip('/')}"
+
+    logger.debug("PUT %s <- req=%s", url, repr(req))
+
+    if not session:
+        session = requests.Session()
+    res = session.put(
+        url,
+        headers={"X-Api-Key": api_key} if api_key else None,
+        json=req,
+        timeout=state.request_timeout,
+    )
     res_json = res.json()
+
     logger.debug("PUT %s -> status_code=%i res=%s", url, res.status_code, repr(res_json))
-    if res.status_code != HTTPStatus.ACCEPTED:
+
+    if res.status_code != expected_status_code:
         api_error(method="PUT", url=url, response=res)
+
     return res_json
 
 
-def api_delete(secrets: DummySecrets, api_url: str) -> None:
+def api_delete(
+    secrets: Union[DummySecrets, str],
+    api_url: str,
+    session: Optional[requests.Session] = None,
+    use_api_key: bool = True,
+    expected_status_code: HTTPStatus = HTTPStatus.OK,
+) -> None:
     """
     Send a `DELETE` request to a Dummy instance.
 
     Args:
-        secrets (DummySecrets): Dummy secrets metadata
-        api_url (str): Dummy API command
+        secrets (Union[DummySecrets, str]): Dummy secrets metadata, or host URL.
+        api_url (str): Dummy API command.
+        expected_status_code (HTTPStatus): Expected response status. Defaults to `200 OK`.
     """
 
-    url = f"{secrets.host_url}/{api_url.lstrip('/')}"
+    if isinstance(secrets, str):
+        host_url = secrets
+        api_key = None
+    else:
+        host_url = secrets.host_url
+        api_key = secrets.api_key.get_secret_value() if use_api_key else None
+    url = f"{host_url}/{api_url.lstrip('/')}"
+
     logger.debug("DELETE %s", url)
-    headers = {"X-Api-Key": secrets.api_key.get_secret_value()}
-    res = (
-        requests.delete(
-            url,
-            headers=headers,
-            timeout=state.config.buildarr.request_timeout,
-        )
-        if not state.dry_run
-        else _create_dryrun_response("DELETE", url)
+
+    if not session:
+        session = requests.Session()
+    res = session.delete(
+        url,
+        headers={"X-Api-Key": api_key} if api_key else None,
+        timeout=state.request_timeout,
     )
+
     logger.debug("DELETE %s -> status_code=%i", url, res.status_code)
-    if res.status_code != HTTPStatus.OK:
+
+    if res.status_code != expected_status_code:
         api_error(method="DELETE", url=url, response=res, parse_response=False)
 
 
 def api_error(
     method: str,
     url: str,
     response: requests.Response,
@@ -206,75 +292,26 @@
     Raises:
         Dummy API exception
     """
 
     error_message = (
         f"Unexpected response with status code {response.status_code} from from '{method} {url}'"
     )
+
     if parse_response:
-        res_json = response.json()
+        error_message += ": "
         try:
-            error_message += f": {res_json['message']}\n{res_json['description']}"
-        except KeyError:
-            error_message += f": {res_json}"
-    raise DummyAPIError(error_message, response=response)
-
-
-def _create_dryrun_response(
-    method: str,
-    url: str,
-    headers: Optional[Mapping[str, str]] = None,
-    status_code: Optional[int] = None,
-    content_type: str = "application/json",
-    charset: str = "utf-8",
-    content: str = "{}",
-) -> requests.Response:
-    """
-    A utility function for generating `requests.Response` objects in dry-run mode.
-
-    Args:
-        method (str): HTTP method of the response to simulate.
-        url (str): URL of the request.
-        status_code (Optional[int], optional): Status code for the response. Default: auto-detect
-        content_type (str, optional): MIME type of response content. Default: `application/json`
-        charset (str, optional): Encoding of response content. Default: `utf-8`
-        content (str, optional): Response content. Default: `{}`
-
-    Raises:
-        ValueError: When an unsupported HTTP method is used
-
-    Returns:
-        Generated `requests.Response` object
-    """
-
-    method = method.upper()
-
-    response = requests.Response()
-    response.url = url
-    response.headers["Vary"] = "Accept"
-    response.headers["Cache-Control"] = "no-cache, no-store, must-revalidate, max-age=0"
-    response.headers["Pragma"] = "no-cache"
-    response.headers["Expires"] = "0"
-    response.headers["Access-Control-Allow-Origin"] = "*"
-    response.headers["Content-Type"] = f"{content_type}; charset={charset}"
-    response.headers["Server"] = "Mono-HTTPAPI/1.0"
-    response.headers["Date"] = datetime.now(tz=timezone.utc).strftime("%a, %d %b %Y %H:%M:%S %Z")
-    response.headers["Transfer-Encoding"] = "chunked"
-    if headers:
-        response.headers.update(headers)
-    if status_code is not None:
-        response.status_code = status_code
-    elif method == "POST":
-        response.status_code = int(HTTPStatus.CREATED)
-    elif method == "PUT":
-        response.status_code = int(HTTPStatus.ACCEPTED)
-    elif method == "DELETE":
-        response.status_code = int(HTTPStatus.OK)
-    else:
-        raise ValueError(
-            f"Unsupported HTTP method for creating dry-run response: {str(method)}",
-        )
-    response.encoding = charset
-    if content is not None:
-        response._content = content.encode("UTF-8")
+            res_json = response.json()
+            try:
+                error_message += f"{res_json['message']}\n{res_json['description']}"
+            except KeyError:
+                try:
+                    error_message += res_json["message"]
+                except KeyError:
+                    try:
+                        error_message += res_json["error"]
+                    except KeyError:
+                        error_message += f"(Unsupported error JSON format) {res_json}"
+        except json.JSONDecodeError:
+            f"(Non-JSON error response)\n{response.text}"
 
-    return response
+    raise DummyAPIError(error_message, status_code=response.status_code)
```

### Comparing `buildarr-0.4.2/buildarr/plugins/dummy/cli.py` & `buildarr-0.5.0/buildarr/plugins/dummy/cli.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/plugins/dummy/config/__init__.py` & `buildarr-0.5.0/buildarr/plugins/dummy/config/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 """
 Dummy plugin configuration.
 """
 
 
 from __future__ import annotations
 
-from pathlib import Path
 from typing import TYPE_CHECKING, Dict, Optional
 
 from typing_extensions import Self
 
 from buildarr.config import ConfigPlugin
 from buildarr.types import NonEmptyStr, Port
 
@@ -135,47 +134,41 @@
 
     settings: DummySettingsConfig = DummySettingsConfig()
     """
     Dummy settings.
     Configuration options for Dummy itself are set within this structure.
     """
 
-    @property
     def uses_trash_metadata(self) -> bool:
         """
-        A flag determining whether or not this instance configuration uses TRaSH-Guides metadata.
+        Return whether or not this instance configuration uses TRaSH-Guides metadata.
 
         Returns:
             `True` if TRaSH-Guides metadata is used, otherwise `False`
         """
-        return self.settings.uses_trash_metadata
+        return self.settings.uses_trash_metadata()
 
-    def render_trash_metadata(self, trash_metadata_dir: Path) -> Self:
+    def render(self) -> Self:
         """
-        Read TRaSH-Guides metadata, and return a configuration object with all templates rendered.
-
-        Args:
-            trash_metadata_dir (Path): TRaSH-Guides metadata directory.
+        Render dynamic configuration attributes, and return the resulting configuration object.
 
         Returns:
             Rendered configuration object
         """
+        if not self.settings.uses_trash_metadata():
+            return self
         copy = self.copy(deep=True)
-        copy._render_trash_metadata(trash_metadata_dir)
+        copy._render()
         return copy
 
-    def _render_trash_metadata(self, trash_metadata_dir: Path) -> None:
+    def _render(self) -> None:
         """
-        Render configuration attributes obtained from TRaSH-Guides, in-place.
-
-        Args:
-            trash_metadata_dir (Path): TRaSH-Guides metadata directory.
+        Render dynamic configuration attributes in place.
         """
-        if self.settings.uses_trash_metadata:
-            self.settings._render_trash_metadata(trash_metadata_dir)
+        self.settings._render()
 
     @classmethod
     def from_remote(cls, secrets: DummySecrets) -> Self:
         """
         Read configuration from a remote instance and return it as a configuration object.
 
         Args:
@@ -207,38 +200,7 @@
     Instance-specific Dummy configuration.
 
     Can only be defined on the global `dummy` configuration block.
 
     Globally specified configuration values apply to all instances.
     Configuration values specified on an instance-level take precedence at runtime.
     """
-
-    @property
-    def uses_trash_metadata(self) -> bool:
-        """
-        A flag determining whether or not this configuration uses TRaSH-Guides metadata.
-
-        Returns:
-            `True` if TRaSH-Guides metadata is used, otherwise `False`
-        """
-        for instance in self.instances.values():
-            if instance.uses_trash_metadata:
-                return True
-        return super().uses_trash_metadata
-
-    def render_trash_metadata(self, trash_metadata_dir: Path) -> Self:
-        """
-        Read TRaSH-Guides metadata, and return a configuration object with all templates rendered.
-
-        Args:
-            trash_metadata_dir (Path): TRaSH-Guides metadata directory.
-
-        Returns:
-            Rendered configuration object
-        """
-        copy = self.copy(deep=True)
-        for instance in copy.instances.values():
-            if instance.uses_trash_metadata:
-                instance._render_trash_metadata(trash_metadata_dir)
-        if self.uses_trash_metadata:
-            copy._render_trash_metadata(trash_metadata_dir)
-        return copy
```

### Comparing `buildarr-0.4.2/buildarr/plugins/dummy/config/settings.py` & `buildarr-0.5.0/buildarr/plugins/dummy/config/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 """
 
 
 from __future__ import annotations
 
 import json
 
-from pathlib import Path
 from typing import Any, List, Mapping, Optional, Union, cast
 from uuid import UUID, uuid4
 
 from pydantic import Field
 from typing_extensions import Self
 
 from buildarr.config import ConfigTrashIDNotFoundError, RemoteMapEntry
@@ -105,38 +104,37 @@
     see the documentation for the following methods in `buildarr/config/__init__.py`:
 
     * `ConfigBase.get_local_attrs`
     * `ConfigBase.get_create_remote_attrs`
     * `ConfigBase.get_update_remote_attrs`
     """
 
-    @property
     def uses_trash_metadata(self) -> bool:
         """
-        A flag determining whether or not this instance configuration uses TRaSH-Guides metadata.
+        Return whether or not this instance configuration uses TRaSH-Guides metadata.
 
         Returns:
             `True` if TRaSH-Guides metadata is used, otherwise `False`
         """
         return bool(self.trash_id)
 
-    def _render_trash_metadata(self, sonarr_metadata_dir: Path) -> None:
+    def _render(self) -> None:
         """
-        Render configuration attributes obtained from TRaSH-Guides, in-place.
+        Render dynamic configuration attributes in place.
+
+        Specifically, this function reads a value from the TRaSH-Guides metadata
+        and populates the `trash_value` attribute with it.
 
         Set `trash_value` to the minimum data rate value for the
         `Bluray-1080p` quality definition in the profile.
-
-        Args:
-            trash_metadata_dir (Path): TRaSH-Guides metadata directory.
         """
         if not self.trash_id:
             return
         for quality_file in (
-            sonarr_metadata_dir / "docs" / "json" / "sonarr" / "quality-size"
+            state.trash_metadata_dir / "docs" / "json" / "sonarr" / "quality-size"
         ).iterdir():
             with quality_file.open() as f:
                 quality_json: Mapping[str, Any] = json.load(f)
                 if cast(str, quality_json["trash_id"]).lower() == self.trash_id:
                     for definition_json in quality_json["qualities"]:
                         if definition_json["quality"] == "Bluray-1080p":
                             self.trash_value = cast(float, definition_json["min"])
@@ -214,12 +212,7 @@
             check_unmanaged=check_unmanaged,
             set_unchanged=True,
         )
         if changed:
             api_post(secrets, "/api/v1/settings", remote_attrs)
             return True
         return False
-
-    class Config(DummyConfigBase.Config):
-        # Ensure in-place assignments of attributes are always validated,
-        # since this class performs such modifications in certain cases.
-        validate_assignment = True
```

### Comparing `buildarr-0.4.2/buildarr/plugins/dummy/config/types.py` & `buildarr-0.5.0/buildarr/plugins/dummy/config/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,13 +26,13 @@
 # Define the base class for Dummy configuration classes.
 # Subclassing this conditionally-created class allows Mypy to
 # properly resolve secrets type declarations.
 if TYPE_CHECKING:
     from ..secrets import DummySecrets
 
     class DummyConfigBase(ConfigBase[DummySecrets]):
-        ...
+        pass
 
 else:
 
     class DummyConfigBase(ConfigBase):
-        ...
+        pass
```

### Comparing `buildarr-0.4.2/buildarr/plugins/dummy/exceptions.py` & `buildarr-0.5.0/buildarr/plugins/dummy/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,31 +15,42 @@
 """
 Dummy plugin exception classes.
 """
 
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
-
 from buildarr.exceptions import BuildarrError
 
-if TYPE_CHECKING:
-    from requests import Response
-
 
 class DummyError(BuildarrError):
     """
     Dummy plugin exception base class.
     """
 
     pass
 
 
 class DummyAPIError(DummyError):
     """
     Dummy API exception class.
     """
 
-    def __init__(self, msg: str, response: Response) -> None:
-        self.response = response
+    def __init__(self, msg: str, status_code: int) -> None:
+        self.status_code = status_code
         super().__init__(msg)
+
+
+class DummySecretsError(DummyError):
+    """
+    Dummy plugin secrets exception base class.
+    """
+
+    pass
+
+
+class DummySecretsUnauthorizedError(DummySecretsError):
+    """
+    Error raised when the Dummy API key wasn't able to be retrieved.
+    """
+
+    pass
```

### Comparing `buildarr-0.4.2/buildarr/plugins/dummy/manager.py` & `buildarr-0.5.0/buildarr/plugins/dummy/manager.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/plugins/dummy/plugin.py` & `buildarr-0.5.0/buildarr/plugins/dummy/plugin.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/plugins/dummy/secrets.py` & `buildarr-0.5.0/buildarr/plugins/dummy/secrets.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,30 +23,30 @@
 from typing import TYPE_CHECKING
 from urllib.parse import urlparse
 
 from buildarr.secrets import SecretsPlugin
 from buildarr.types import NonEmptyStr, Port
 
 from .api import api_get, get_initialize_js
-from .exceptions import DummyAPIError
+from .exceptions import DummyAPIError, DummySecretsUnauthorizedError
 from .types import DummyApiKey, DummyProtocol
 
 # Allow Mypy to properly resolve configuration type declarations in secrets classes.
 if TYPE_CHECKING:
     from typing_extensions import Self
 
     from .config import DummyConfig
 
     class _DummySecrets(SecretsPlugin[DummyConfig]):
-        ...
+        pass
 
 else:
 
     class _DummySecrets(SecretsPlugin):
-        ...
+        pass
 
 
 class DummySecrets(_DummySecrets):
     """
     Dummy API secrets.
     """
 
@@ -94,31 +94,42 @@
 
         Args:
             config (DummyConfig): Instance configuration
 
         Returns:
             Secrets object
         """
-        return cls(
-            hostname=config.hostname,
-            port=config.port,
-            protocol=config.protocol,
-            api_key=(
-                config.api_key if config.api_key else get_initialize_js(config.host_url)["apiKey"]
-            ),
-        )
+        try:
+            return cls(
+                hostname=config.hostname,
+                port=config.port,
+                protocol=config.protocol,
+                api_key=(
+                    config.api_key
+                    if config.api_key
+                    else get_initialize_js(config.host_url)["apiKey"]
+                ),
+            )
+        except DummyAPIError as err:
+            if err.status_code == HTTPStatus.UNAUTHORIZED:
+                raise DummySecretsUnauthorizedError(
+                    "Unable to retrieve the API key for the Dummy instance "
+                    f"at '{config.host_url}': Authentication is enabled",
+                ) from None
+            else:
+                raise
 
     def test(self) -> bool:
         """
         Test whether or not the secrets metadata is valid for connecting to the instance.
 
         Returns:
             `True` if the test was successful, otherwise `False`
         """
         try:
             api_get(self, "/api/v1/settings")
             return True
         except DummyAPIError as err:
-            if err.response.status_code == HTTPStatus.UNAUTHORIZED:
+            if err.status_code == HTTPStatus.UNAUTHORIZED:
                 return False
             else:
                 raise
```

### Comparing `buildarr-0.4.2/buildarr/plugins/dummy/server.py` & `buildarr-0.5.0/buildarr/plugins/dummy/server.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/plugins/dummy/types.py` & `buildarr-0.5.0/buildarr/plugins/dummy/types.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/plugins/load.py` & `buildarr-0.5.0/buildarr/plugins/load.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/plugins/models.py` & `buildarr-0.5.0/buildarr/plugins/models.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/plugins/types.py` & `buildarr-0.5.0/buildarr/plugins/types.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/secrets/__init__.py` & `buildarr-0.5.0/buildarr/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/secrets/base.py` & `buildarr-0.5.0/buildarr/secrets/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,10 +88,8 @@
             ...
 
             class Config(_ExampleSecrets.Config):
                 ...  # Add model configuration attributes here.
         ```
         """
 
-        # Validate any values that have been modified in-place, to ensure the model
-        # still fits the constraints.
-        validate_assignment = True
+        pass
```

### Comparing `buildarr-0.4.2/buildarr/secrets/load.py` & `buildarr-0.5.0/buildarr/secrets/load.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/secrets/models.py` & `buildarr-0.5.0/buildarr/secrets/models.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/buildarr/state.py` & `buildarr-0.5.0/buildarr/state.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,23 +55,35 @@
     """
 
     testing: bool = bool(strtobool(os.environ.get("BUILDARR_TESTING", "false")))
     """
     Whether Buildarr is in testing mode or not.
     """
 
-    dry_run: bool = False
-    """
-    Whether Buildarr is in dry run mode or not.
-
-    When set to `True` under a CLI command that supports it, the command should not
-    perform any action that would change the state of any external instances.
-
-    Custom CLI commands can set this attribute to `True` if they support a dry-run mode.
-    """
+    @property
+    def dry_run(self) -> bool:
+        """
+        Whether Buildarr is in dry run mode or not.
+
+        **Note: As of Buildarr v0.5.0, this mode is no longer available,
+        and `state.dry_run` will always return `False`.**
+        """
+        return False
+
+    @property
+    def request_timeout(self) -> float:
+        """
+        Default timeout for HTTP requests, in seconds.
+
+        If the Buildarr configuration is loaded, the value defined there is used.
+        Otherwise, this is set to a default of 30 seconds.
+        """
+        if self.config is not None:
+            return self.config.buildarr.request_timeout
+        return 30.0
 
     plugins: Mapping[str, Plugin] = {}
     """
     The loaded Buildarr plugins, mapped to the plugin's unique name.
     """
 
     config: ConfigType = None  # type: ignore[assignment]
```

### Comparing `buildarr-0.4.2/buildarr/trash.py` & `buildarr-0.5.0/buildarr/trash.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,30 +15,27 @@
 """
 Buildarr TRaSH-Guides metadata functions.
 """
 
 
 from __future__ import annotations
 
-from collections import defaultdict
 from contextlib import contextmanager
 from logging import getLogger
 from pathlib import Path
 from shutil import move, rmtree
 from typing import TYPE_CHECKING
 from urllib.request import urlretrieve
 from zipfile import ZipFile
 
 from .state import state
 from .util import create_temp_dir
 
 if TYPE_CHECKING:
-    from typing import DefaultDict, Dict, Generator
-
-    from .config import ConfigPlugin
+    from typing import Generator
 
 
 logger = getLogger(__name__)
 
 
 def trash_metadata_used() -> bool:
     """
@@ -100,41 +97,7 @@
 
         state.trash_metadata_dir = temp_dir
         yield temp_dir
         state.trash_metadata_dir = None  # type: ignore[assignment]
 
         logger.debug("Deleting TRaSH metadata download temporary directory")
     logger.debug("Finished deleting TRaSH metadata download temporary directory")
-
-
-def render_trash_metadata(trash_metadata_dir: Path) -> None:
-    """
-    Render TRaSH-Guides metadata on any instance configurations where used,
-    and update the global state.
-
-    Plugins will parse the TRaSH-Guides metadata files in the given directory
-    and return new configuration objects with attributes populated from the metadata.
-
-    Instances that do not use TRaSH-Guides metadata will be left unchanged.
-
-    Args:
-        trash_metadata_dir (Path): Local folder containing TRaSH-Guides metadata files.
-    """
-
-    instance_configs: DefaultDict[str, Dict[str, ConfigPlugin]] = defaultdict(dict)
-
-    for plugin_name, instance_name in state._execution_order:
-        manager = state.managers[plugin_name]
-        instance_config = state.instance_configs[plugin_name][instance_name]
-        with state._with_context(plugin_name=plugin_name, instance_name=instance_name):
-            if manager.uses_trash_metadata(instance_config):
-                logger.debug("Rendering TRaSH-Guides metadata")
-                instance_configs[plugin_name][instance_name] = manager.render_trash_metadata(
-                    instance_config,
-                    trash_metadata_dir,
-                )
-                logger.debug("Finished rendering TRaSH-Guides metadata")
-            else:
-                logger.debug("Skipping rendering TRaSH-Guides metadata (not used)")
-                instance_configs[plugin_name][instance_name] = instance_config
-
-    state.instance_configs = instance_configs
```

### Comparing `buildarr-0.4.2/buildarr/types.py` & `buildarr-0.5.0/buildarr/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 Buildarr general purpose type hints, used in plugin models.
 """
 
 
 from __future__ import annotations
 
 import re
-import warnings
 
-from enum import Enum, IntEnum
+from enum import Enum
+from functools import total_ordering
 from pathlib import Path, PurePosixPath, PureWindowsPath
 from typing import TYPE_CHECKING, Any, Callable, Generator, Mapping
 
 from pydantic import AnyUrl, ConstrainedInt, ConstrainedStr, Field, SecretStr
 from pydantic.fields import ModelField
 from typing_extensions import Annotated, Self
 
@@ -214,114 +214,83 @@
                     return cls(str(value))
                 except ValueError:
                     return cls.from_name_str(value)
             except (TypeError, KeyError):
                 raise ValueError(f"Invalid {cls.__name__} name or value: {value}") from None
 
 
-class BaseIntEnum(IntEnum):
+@total_ordering
+class DayOfWeek(BaseEnum):
     """
-    Integer numeration base class for use in Buildarr configurations.
+    Sortable eumeration for the days in the week (Monday to Sunday).
+
+    Values (in ascending order):
 
-    Like `BaseEnum`, but as the enumeration values are guaranteed to be integer type,
-    it natively supports sorting functions such as `sorted`.
+    * `monday` (Monday)
+    * `tuesday` (Tuesday)
+    * `wednesday` (Wednesday)
+    * `thursday` (Thursday)
+    * `friday` (Friday)
+    * `saturday` (Saturday)
+    * `sunday` (Sunday)
     """
 
-    @classmethod
-    def from_name_str(cls, name_str: str) -> Self:
+    monday = 0
+    tuesday = 1
+    wednesday = 2
+    thursday = 3
+    friday = 4
+    saturday = 5
+    sunday = 6
+
+    def __eq__(self, other: Any) -> bool:
         """
-        Get the enumeration object corresponding to the given name case-insensitively.
+        Reimplement the `a == b` operator for `DayOfWeek`, so integers
+        of the same value also get evaluated as equal.
 
         Args:
-            name_str (str): Name of the enumeration value (case insensitive).
-
-        Raises:
-            KeyError: When the enumeration name is invalid (does not exist).
+            other (Any): Object to check is equal to this object.
 
         Returns:
-            The enumeration object for the given name
+            `True` if this object is equal to `other`, otherwise `False`
         """
-        warnings.warn(
-            (
-                "BaseIntEnum is deprecated, and will be removed in Buildarr version 0.5.0. "
-                "Please update your Buildarr plugin to use BaseEnum instead."
-            ),
-            DeprecationWarning,
-            stacklevel=1,
-        )
-        name = name_str.lower().replace("-", "_")
-        for obj in cls:
-            if obj.name.lower() == name:
-                return obj
-        raise KeyError(repr(name))
+        try:
+            other_obj = DayOfWeek(other)
+        except ValueError:
+            raise NotImplementedError() from None
+        return self.value == other_obj.value
 
-    def to_name_str(self) -> str:
+    def __hash__(self) -> int:
         """
-        Return the name for this enumaration object.
+        Implement the hash method for `DayOfWeek`.
+
+        Simply return the enumeration value, since it is an integer and always unique.
 
         Returns:
-            Enumeration name
+            `DayOfWeek` hash
         """
-        return self.name.replace("_", "-")
+        return self.value
 
-    @classmethod
-    def __get_validators__(cls) -> Generator[Callable[[Any], Self], None, None]:
+    def __lt__(self, other: Any) -> bool:
         """
-        Pass class validation functions to Pydantic.
+        Implement the `a < b` operator for `DayOfWeek`.
 
-        Yields:
-            Validation class functions
-        """
-        yield cls.validate
-
-    @classmethod
-    def validate(cls, value: Any) -> Self:
-        """
-        Validate and coerce the given value to an enumeration object.
+        The `total_ordering` decorator will declare the rest.
 
         Args:
-            value (Any): Object to validate and coerce
-
-        Raises:
-            ValueError: If a enumeration object corresponding with the value cannot be found
+            other (Any): Object to check is greater than this object.
 
         Returns:
-            Enumeration object corresponding to the given value
+            `True` if this object is less than `other`, otherwise `False`
         """
         try:
-            return cls(value)
+            other_obj = DayOfWeek(other)
         except ValueError:
-            try:
-                return cls.from_name_str(value)
-            except (TypeError, KeyError):
-                raise ValueError(f"Invalid {cls.__name__} name or value: {value}") from None
-
-
-class DayOfWeek(BaseIntEnum):
-    """
-    Sortable eumeration for the days in the week (Monday to Sunday).
-
-    Values (in ascending order):
-
-    * `monday` (Monday)
-    * `tuesday` (Tuesday)
-    * `wednesday` (Wednesday)
-    * `thursday` (Thursday)
-    * `friday` (Friday)
-    * `saturday` (Saturday)
-    * `sunday` (Sunday)
-    """
-
-    monday = 0
-    tuesday = 1
-    wednesday = 2
-    thursday = 3
-    friday = 4
-    saturday = 5
-    sunday = 6
+            raise NotImplementedError() from None
+        return self.value < other_obj.value
 
 
 class InstanceName(str):
     """
     A type for creating references to an instance in another plugin.
 
     When loading the instance-specific configurations, Buildarr will dereference
@@ -510,7 +479,11 @@
 
     # Validate all configuration attributes, even the default ones.
     # This is necessary because the default attributes sometimes need to
     # be validated for correctness in non-default contexts.
     # (For example, a normally optional attribute becoming required due to
     # another attribute being enabled.)
     validate_all = True
+
+    # Validate any values that have been modified in-place, to ensure the model
+    # still fits the constraints.
+    validate_assignment = True
```

### Comparing `buildarr-0.4.2/buildarr/util.py` & `buildarr-0.5.0/buildarr/util.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.2/pyproject.toml` & `buildarr-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.3.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "buildarr"
-version = "0.4.2"
+version = "0.5.0"
 description = "Constructs and configures Arr PVR stacks"
 authors = ["Callum Dickinson <callum.dickinson.nz@gmail.com>"]
 license = "GPL-3.0-or-later"
 homepage = "https://buildarr.github.io"
 repository = "https://github.com/buildarr/buildarr"
 documentation = "https://buildarr.github.io"
 keywords = ["buildarr", "sonarr", "radarr", "prowlarr"]
```

### Comparing `buildarr-0.4.2/PKG-INFO` & `buildarr-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildarr
-Version: 0.4.2
+Version: 0.5.0
 Summary: Constructs and configures Arr PVR stacks
 Home-page: https://buildarr.github.io
 License: GPL-3.0-or-later
 Keywords: buildarr,sonarr,radarr,prowlarr
 Author: Callum Dickinson
 Author-email: callum.dickinson.nz@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -211,15 +211,14 @@
 2023-02-22 21:21:27,223 buildarr:1 buildarr.main [INFO] Buildarr ready.
 ```
 
 For more information on how to interfact with Buildarr, check the [usage documentation](https://buildarr.github.io/usage).
 
 ## To-do list
 
-* Add a dry-run mode for testing configurations (added in [version 0.4.0](https://buildarr.github.io/release-notes/#v040-2023-03-31))
 * Test updates for all available attributes in the existing Sonarr plugin
 * Unit tests and code coverage
 * Split Sonarr plugin to its own repository (completed in [version 0.4.0](https://buildarr.github.io/release-notes/#v040-2023-03-31))
 * Create plugins for the following applications:
     * Sonarr V4
     * Radarr
     * Prowlarr (now available as [`buildarr-prowlarr`](https://buildarr.github.io/plugins/prowlarr))
```

