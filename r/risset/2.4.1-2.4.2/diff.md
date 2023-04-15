# Comparing `tmp/risset-2.4.1.tar.gz` & `tmp/risset-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "risset-2.4.1.tar", last modified: Thu Apr 13 23:01:23 2023, max compression
+gzip compressed data, was "risset-2.4.2.tar", last modified: Sat Apr 15 23:15:34 2023, max compression
```

## Comparing `risset-2.4.1.tar` & `risset-2.4.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-13 23:01:23.052319 risset-2.4.1/
--rw-rw-r--   0 em        (1000) em        (1000)     5627 2023-04-13 23:01:23.052319 risset-2.4.1/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)     5349 2023-04-13 00:18:38.000000 risset-2.4.1/README.md
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-13 23:01:23.051319 risset-2.4.1/risset.egg-info/
--rw-rw-r--   0 em        (1000) em        (1000)     5627 2023-04-13 23:01:23.000000 risset-2.4.1/risset.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)      210 2023-04-13 23:01:23.000000 risset-2.4.1/risset.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-13 23:01:23.000000 risset-2.4.1/risset.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)       39 2023-04-13 23:01:23.000000 risset-2.4.1/risset.egg-info/entry_points.txt
--rw-rw-r--   0 em        (1000) em        (1000)       26 2023-04-13 23:01:23.000000 risset-2.4.1/risset.egg-info/requires.txt
--rw-rw-r--   0 em        (1000) em        (1000)        7 2023-04-13 23:01:23.000000 risset-2.4.1/risset.egg-info/top_level.txt
--rwxrwxr-x   0 em        (1000) em        (1000)   107887 2023-04-13 23:01:14.000000 risset-2.4.1/risset.py
--rw-rw-r--   0 em        (1000) em        (1000)       38 2023-04-13 23:01:23.052319 risset-2.4.1/setup.cfg
--rw-rw-r--   0 em        (1000) em        (1000)      897 2023-04-12 12:16:30.000000 risset-2.4.1/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-15 23:15:34.655872 risset-2.4.2/
+-rw-rw-r--   0 em        (1000) em        (1000)     5664 2023-04-15 23:15:34.654872 risset-2.4.2/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)     5349 2023-04-13 00:18:38.000000 risset-2.4.2/README.md
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-15 23:15:34.654872 risset-2.4.2/risset.egg-info/
+-rw-rw-r--   0 em        (1000) em        (1000)     5664 2023-04-15 23:15:34.000000 risset-2.4.2/risset.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)      210 2023-04-15 23:15:34.000000 risset-2.4.2/risset.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-15 23:15:34.000000 risset-2.4.2/risset.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       40 2023-04-15 23:15:34.000000 risset-2.4.2/risset.egg-info/entry_points.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       26 2023-04-15 23:15:34.000000 risset-2.4.2/risset.egg-info/requires.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        7 2023-04-15 23:15:34.000000 risset-2.4.2/risset.egg-info/top_level.txt
+-rwxrwxr-x   0 em        (1000) em        (1000)   108080 2023-04-15 23:08:22.000000 risset-2.4.2/risset.py
+-rw-rw-r--   0 em        (1000) em        (1000)       38 2023-04-15 23:15:34.655872 risset-2.4.2/setup.cfg
+-rw-rw-r--   0 em        (1000) em        (1000)      897 2023-04-12 12:16:30.000000 risset-2.4.2/setup.py
```

### Comparing `risset-2.4.1/PKG-INFO` & `risset-2.4.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: risset
-Version: 2.4.1
-Summary: A package manager for csound
-Home-page: https://github.com/csound-plugins/risset
-Author: Eduardo Moguillansky
-Author-email: eduardo.moguillansky@gmail.com
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 ![risset](assets/risset-title.png)
 
 # risset: a package manager for csound
 
 This is the repository of risset, a package manager for csound external
 plugins and user-defined-opcodes. The index aggregating all available packages is kept 
 at [risset-data](https://github.com/csound-plugins/risset-data).
```

### Comparing `risset-2.4.1/README.md` & `risset-2.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: risset
+Version: 2.4.2
+Summary: A package manager for csound
+Home-page: https://github.com/csound-plugins/risset
+Author: Eduardo Moguillansky
+Author-email: eduardo.moguillansky@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 ![risset](assets/risset-title.png)
 
 # risset: a package manager for csound
 
 This is the repository of risset, a package manager for csound external
 plugins and user-defined-opcodes. The index aggregating all available packages is kept 
 at [risset-data](https://github.com/csound-plugins/risset-data).
@@ -194,7 +206,9 @@
 
 ## Manifest
 
 Each plugin has an accompanying manifest in the .json format. The name of this file
 is always `risset.json`
 See one of the examples in https://github.com/csound-plugins/csound-plugins/tree/master/src for
 more information about the manifest
+
+
```

### Comparing `risset-2.4.1/risset.egg-info/PKG-INFO` & `risset-2.4.2/risset.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: risset
-Version: 2.4.1
+Version: 2.4.2
 Summary: A package manager for csound
 Home-page: https://github.com/csound-plugins/risset
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ![risset](assets/risset-title.png)
 
 # risset: a package manager for csound
 
@@ -204,7 +206,9 @@
 
 ## Manifest
 
 Each plugin has an accompanying manifest in the .json format. The name of this file
 is always `risset.json`
 See one of the examples in https://github.com/csound-plugins/csound-plugins/tree/master/src for
 more information about the manifest
+
+
```

### Comparing `risset-2.4.1/risset.py` & `risset-2.4.2/risset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
-__version__ = "2.4.1"
+__version__ = "2.4.2"
 
 import sys
 
 if (sys.version_info.major, sys.version_info.minor) < (3, 8):
     print("Python 3.8 or higher is needed", file=sys.stderr)
     sys.exit(-1)
 
@@ -515,16 +515,22 @@
         Returns:
             a Plugin
 
         Raises: PluginDefinitionError if there is an error
         """
         manifest = self.manifest_path()
         assert manifest.exists() and manifest.suffix == '.json'
-        plugin = _read_plugindef(manifest.as_posix(), url=self.url,
-                                 manifest_relative_path=self.path)
+        try:
+            plugin = _read_plugindef(manifest.as_posix(), url=self.url,
+                                     manifest_relative_path=self.path)
+        except Exception as e:
+            self.update()
+            plugin = _read_plugindef(manifest.as_posix(), url=self.url,
+                                     manifest_relative_path=self.path)
+
         plugin.cloned_path = _git_local_path(self.url)
         return plugin
 
 
 @dataclass
 class Plugin:
     """
@@ -620,15 +626,15 @@
         besides the manifest
         """
         root = self.local_manifest_path().parent
         doc_folder = _resolve_path(self.doc_folder or "doc", root)
         if not doc_folder.exists():
             raise OSError(f"No doc folder found (declared as {doc_folder}")
         return doc_folder
-    
+
     def find_binary(self, platform: str = None, csound_version: int = 0) -> Optional[Binary]:
         """
         Find a binary for the platform and csound versions given / current
 
         Returns:
             a Binary which matches the given platform and csound version, or None
             if no match possible
@@ -1903,18 +1909,18 @@
         Args:
             plugin: the plugin to install
             check: if True, check that the opcodes defined in plugin are present
                 after installation
 
         Returns:
             None if ok, an ErrorMsg if failed
-            
+
         Example
         =======
-        
+
             >>> import risset
             >>> idx = risset.MainIndex(update=True)
             >>> pluginpoly = idx.plugins['poly']
             >>> idx.install_plugin(pluginpoly)
         """
         assert isinstance(plugin, Plugin)
         platform = _get_platform()
@@ -2269,15 +2275,15 @@
     os.chdir(currentdir)
 
 
 def _is_mkdocs_installed() -> bool:
     return _is_package_installed("mkdocs") or shutil.which("mkdocs") is not None
 
 
-def _generate_documentation(index: MainIndex, dest: Path = None, 
+def _generate_documentation(index: MainIndex, dest: Path = None,
                             buildhtml=True, onlyinstalled=False,
                             opcodesxml: Path = None
                             ) -> Path:
     """
     Generate documentation for the plugins
 
     Args:
@@ -2859,15 +2865,15 @@
     update_cmd = subparsers.add_parser("update", help="Update repository. Updates the metadata about available"
                                                       "packages, their versions, etc.")
 
     # list-opcodes
     listopcodes_cmd = subparsers.add_parser("listopcodes", help="List installed opcodes")
     listopcodes_cmd.add_argument("-l", "--long", action="store_true", help="Long format")
     listopcodes_cmd.set_defaults(func=cmd_list_installed_opcodes)
-    
+
     # reset
     reset_cmd = subparsers.add_parser("resetcache", help="Remove local clones of plugin's repositories")
 
     # info
     info_cmd = subparsers.add_parser("info", help="Outputs information about risset itself in json format")
     info_cmd.add_argument("--outfile", default=None, help="Save output to this path")
     info_cmd.add_argument("--full", action="store_true", help="Include all available information")
```

### Comparing `risset-2.4.1/setup.py` & `risset-2.4.2/setup.py`

 * *Files identical despite different names*

