# Comparing `tmp/Liara-2.5.3.tar.gz` & `tmp/Liara-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Liara-2.5.3.tar", last modified: Sun Apr 16 11:43:25 2023, max compression
+gzip compressed data, was "Liara-2.5.4.tar", last modified: Sun Apr 16 12:43:42 2023, max compression
```

## Comparing `Liara-2.5.3.tar` & `Liara-2.5.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-16 11:43:25.966311 Liara-2.5.3/
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1332 2023-01-02 13:55:30.000000 Liara-2.5.3/LICENSE.txt
-drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-16 11:43:25.966311 Liara-2.5.3/Liara.egg-info/
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1395 2023-04-16 11:43:25.000000 Liara-2.5.3/Liara.egg-info/PKG-INFO
--rw-r--r--   0 anteru    (1000) anteru    (1000)      729 2023-04-16 11:43:25.000000 Liara-2.5.3/Liara.egg-info/SOURCES.txt
--rw-r--r--   0 anteru    (1000) anteru    (1000)        1 2023-04-16 11:43:25.000000 Liara-2.5.3/Liara.egg-info/dependency_links.txt
--rw-r--r--   0 anteru    (1000) anteru    (1000)       45 2023-04-16 11:43:25.000000 Liara-2.5.3/Liara.egg-info/entry_points.txt
--rw-r--r--   0 anteru    (1000) anteru    (1000)      376 2023-04-16 11:43:25.000000 Liara-2.5.3/Liara.egg-info/requires.txt
--rw-r--r--   0 anteru    (1000) anteru    (1000)        6 2023-04-16 11:43:25.000000 Liara-2.5.3/Liara.egg-info/top_level.txt
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1395 2023-04-16 11:43:25.966311 Liara-2.5.3/PKG-INFO
--rw-r--r--   0 anteru    (1000) anteru    (1000)      441 2023-01-01 11:59:39.000000 Liara-2.5.3/README.md
-drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-16 11:43:25.966311 Liara-2.5.3/liara/
--rwxr-xr-x   0 anteru    (1000) anteru    (1000)    29291 2023-04-16 11:43:18.000000 Liara-2.5.3/liara/__init__.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     4975 2023-01-01 11:59:39.000000 Liara-2.5.3/liara/actions.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     9328 2023-02-11 11:15:23.000000 Liara-2.5.3/liara/cache.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)    10367 2023-04-15 11:41:10.000000 Liara-2.5.3/liara/cmdline.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     2675 2023-02-11 11:15:23.000000 Liara-2.5.3/liara/config.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     4540 2023-01-01 11:59:39.000000 Liara-2.5.3/liara/feeds.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)    12347 2023-04-16 11:43:18.000000 Liara-2.5.3/liara/md.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)    31982 2023-02-11 11:15:23.000000 Liara-2.5.3/liara/nodes.py
-drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-16 11:43:25.966311 Liara-2.5.3/liara/plugins/
--rw-r--r--   0 anteru    (1000) anteru    (1000)      132 2023-01-01 11:59:39.000000 Liara-2.5.3/liara/plugins/__init__.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)      889 2023-04-15 11:41:10.000000 Liara-2.5.3/liara/plugins/has_pending_document.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1326 2023-04-15 11:41:10.000000 Liara-2.5.3/liara/plugins/series_schedule.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     5349 2023-02-11 11:15:23.000000 Liara-2.5.3/liara/publish.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     8046 2023-02-11 11:15:23.000000 Liara-2.5.3/liara/query.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)    11574 2023-01-01 11:59:39.000000 Liara-2.5.3/liara/quickstart.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     5236 2023-01-22 13:57:52.000000 Liara-2.5.3/liara/server.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1953 2023-02-11 11:15:23.000000 Liara-2.5.3/liara/signals.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)    28210 2023-04-15 11:41:10.000000 Liara-2.5.3/liara/site.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)    11215 2023-01-01 11:59:39.000000 Liara-2.5.3/liara/template.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     4116 2023-01-01 11:59:39.000000 Liara-2.5.3/liara/util.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)      888 2023-01-01 11:59:39.000000 Liara-2.5.3/liara/yaml.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)      190 2023-01-01 11:59:39.000000 Liara-2.5.3/pyproject.toml
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1457 2023-04-16 11:43:25.966311 Liara-2.5.3/setup.cfg
--rw-r--r--   0 anteru    (1000) anteru    (1000)       38 2023-01-01 11:59:39.000000 Liara-2.5.3/setup.py
-drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-16 11:43:25.966311 Liara-2.5.3/test/
--rw-r--r--   0 anteru    (1000) anteru    (1000)      141 2023-01-01 11:59:39.000000 Liara-2.5.3/test/test_cache.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     3708 2023-04-16 11:43:18.000000 Liara-2.5.3/test/test_md.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1363 2023-02-11 11:15:23.000000 Liara-2.5.3/test/test_nodes.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     2498 2023-02-11 11:15:23.000000 Liara-2.5.3/test/test_query.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     6064 2023-01-01 11:59:39.000000 Liara-2.5.3/test/test_site.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     2391 2023-01-01 11:59:39.000000 Liara-2.5.3/test/test_template.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1031 2023-01-01 11:59:39.000000 Liara-2.5.3/test/test_util.py
+drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-16 12:43:42.778083 Liara-2.5.4/
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1332 2023-01-02 13:55:30.000000 Liara-2.5.4/LICENSE.txt
+drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-16 12:43:42.778083 Liara-2.5.4/Liara.egg-info/
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1395 2023-04-16 12:43:42.000000 Liara-2.5.4/Liara.egg-info/PKG-INFO
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      729 2023-04-16 12:43:42.000000 Liara-2.5.4/Liara.egg-info/SOURCES.txt
+-rw-r--r--   0 anteru    (1000) anteru    (1000)        1 2023-04-16 12:43:42.000000 Liara-2.5.4/Liara.egg-info/dependency_links.txt
+-rw-r--r--   0 anteru    (1000) anteru    (1000)       45 2023-04-16 12:43:42.000000 Liara-2.5.4/Liara.egg-info/entry_points.txt
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      376 2023-04-16 12:43:42.000000 Liara-2.5.4/Liara.egg-info/requires.txt
+-rw-r--r--   0 anteru    (1000) anteru    (1000)        6 2023-04-16 12:43:42.000000 Liara-2.5.4/Liara.egg-info/top_level.txt
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1395 2023-04-16 12:43:42.778083 Liara-2.5.4/PKG-INFO
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      441 2023-01-01 11:59:39.000000 Liara-2.5.4/README.md
+drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-16 12:43:42.778083 Liara-2.5.4/liara/
+-rwxr-xr-x   0 anteru    (1000) anteru    (1000)    29291 2023-04-16 12:43:28.000000 Liara-2.5.4/liara/__init__.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     4975 2023-01-01 11:59:39.000000 Liara-2.5.4/liara/actions.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     9328 2023-02-11 11:15:23.000000 Liara-2.5.4/liara/cache.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)    10367 2023-04-15 11:41:10.000000 Liara-2.5.4/liara/cmdline.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     2675 2023-02-11 11:15:23.000000 Liara-2.5.4/liara/config.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     4540 2023-01-01 11:59:39.000000 Liara-2.5.4/liara/feeds.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)    12471 2023-04-16 12:43:28.000000 Liara-2.5.4/liara/md.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)    32036 2023-04-16 12:43:28.000000 Liara-2.5.4/liara/nodes.py
+drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-16 12:43:42.778083 Liara-2.5.4/liara/plugins/
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      132 2023-01-01 11:59:39.000000 Liara-2.5.4/liara/plugins/__init__.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      889 2023-04-15 11:41:10.000000 Liara-2.5.4/liara/plugins/has_pending_document.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1326 2023-04-15 11:41:10.000000 Liara-2.5.4/liara/plugins/series_schedule.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     5349 2023-02-11 11:15:23.000000 Liara-2.5.4/liara/publish.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     8046 2023-02-11 11:15:23.000000 Liara-2.5.4/liara/query.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)    11574 2023-01-01 11:59:39.000000 Liara-2.5.4/liara/quickstart.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     5236 2023-01-22 13:57:52.000000 Liara-2.5.4/liara/server.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1953 2023-02-11 11:15:23.000000 Liara-2.5.4/liara/signals.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)    28210 2023-04-15 11:41:10.000000 Liara-2.5.4/liara/site.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)    11215 2023-01-01 11:59:39.000000 Liara-2.5.4/liara/template.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     4116 2023-01-01 11:59:39.000000 Liara-2.5.4/liara/util.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      888 2023-01-01 11:59:39.000000 Liara-2.5.4/liara/yaml.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      190 2023-01-01 11:59:39.000000 Liara-2.5.4/pyproject.toml
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1457 2023-04-16 12:43:42.778083 Liara-2.5.4/setup.cfg
+-rw-r--r--   0 anteru    (1000) anteru    (1000)       38 2023-01-01 11:59:39.000000 Liara-2.5.4/setup.py
+drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-16 12:43:42.778083 Liara-2.5.4/test/
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      141 2023-01-01 11:59:39.000000 Liara-2.5.4/test/test_cache.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     3708 2023-04-16 11:43:18.000000 Liara-2.5.4/test/test_md.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1363 2023-02-11 11:15:23.000000 Liara-2.5.4/test/test_nodes.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     2498 2023-02-11 11:15:23.000000 Liara-2.5.4/test/test_query.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     6064 2023-01-01 11:59:39.000000 Liara-2.5.4/test/test_site.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     2391 2023-01-01 11:59:39.000000 Liara-2.5.4/test/test_template.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1031 2023-01-01 11:59:39.000000 Liara-2.5.4/test/test_util.py
```

### Comparing `Liara-2.5.3/LICENSE.txt` & `Liara-2.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Liara-2.5.3/Liara.egg-info/PKG-INFO` & `Liara-2.5.4/Liara.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Liara
-Version: 2.5.3
+Version: 2.5.4
 Summary: Static page generator
 Home-page: http://shelter13.net/projects/Liara
 Author: Matthäus G. Chajdas
 Author-email: dev@anteru.net
 License: BSD 2-Clause License
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Liara-2.5.3/Liara.egg-info/SOURCES.txt` & `Liara-2.5.4/Liara.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Liara-2.5.3/PKG-INFO` & `Liara-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Liara
-Version: 2.5.3
+Version: 2.5.4
 Summary: Static page generator
 Home-page: http://shelter13.net/projects/Liara
 Author: Matthäus G. Chajdas
 Author-email: dev@anteru.net
 License: BSD 2-Clause License
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Liara-2.5.3/liara/__init__.py` & `Liara-2.5.4/liara/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     _process_node_sync
 )
 
 from .cache import Cache, FilesystemCache, NullCache, Sqlite3Cache, RedisCache
 from .util import FilesystemWalker, flatten_dictionary
 from .yaml import load_yaml
 
-__version__ = '2.5.3'
+__version__ = '2.5.4'
 __all__ = [
     'actions',
     'cache',
     'cmdline',
     'config',
     'feeds',
     'md',
```

### Comparing `Liara-2.5.3/liara/actions.py` & `Liara-2.5.4/liara/actions.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.3/liara/cache.py` & `Liara-2.5.4/liara/cache.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.3/liara/cmdline.py` & `Liara-2.5.4/liara/cmdline.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.3/liara/config.py` & `Liara-2.5.4/liara/config.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.3/liara/feeds.py` & `Liara-2.5.4/liara/feeds.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.3/liara/md.py` & `Liara-2.5.4/liara/md.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from markdown.extensions import Extension
 from markdown.treeprocessors import Treeprocessor
 from markdown.preprocessors import Preprocessor
-from enum import Enum
 import re
 import logging
 from typing import (
     List, Optional
 )
 
 
@@ -263,17 +262,19 @@
       Instead, you'll have to use something like::
 
         <% alert message="This is important" blink=yes /%>
     """
 
     __log = logging.getLogger(f'{__name__}.{__qualname__}')
 
-    def __init__(self, md=None):
+    def __init__(self, md=None, node=None):
+        from .template import Page
         super().__init__(md)
         self.__functions = dict()
+        self.__page = Page(node)
 
     def register(self, name: str, function):
         """Register a new Markdown shortcode function.
 
         Shortcode function calls must accept all arguments as named arguments.
         Names (both function names and argument names) starting with ``$`` are
         reserved for built-in functions.
@@ -311,14 +312,16 @@
 
                 # Remove start from the current line
                 lines[i] = line[tag_start:]
 
                 parse_buffer = _ParseBuffer(i, lines)
                 shortcode_parser = _ShortcodeParser(parse_buffer)
                 rest, next_line, func_name, args = shortcode_parser.parse()
+
+                args['$page'] = self.__page
                 yield from self.__functions[func_name](**args).splitlines()
 
                 # Another shortcode in the same line, so we need to resume
                 # parsing there and cannot simply emit the rest
                 if '<%' in rest:
                     assert next_line >= 1
                     lines[next_line-1] = rest
@@ -330,23 +333,24 @@
                 i = next_line
             else:
                 yield line
                 i += 1
 
 
 class LiaraMarkdownExtensions(Extension):
-    """Markdown extension for the :py:class:`HeadingLevelFixupProcessor`.
+    """Register various markdown extensions.
     """
-    def __init__(self):
+    def __init__(self, node=None):
         super().__init__()
+        self.__node = node
 
     def extendMarkdown(self, md):
         from .signals import register_markdown_shortcodes
 
-        shortcode_preprocessor = ShortcodePreprocessor(md)
+        shortcode_preprocessor = ShortcodePreprocessor(md, self.__node)
 
         register_markdown_shortcodes.send(
             self,
             preprocessor=shortcode_preprocessor)
 
         md.treeprocessors.register(HeadingLevelFixupProcessor(md),
                                    'heading-level-fixup',
```

### Comparing `Liara-2.5.3/liara/nodes.py` & `Liara-2.5.4/liara/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -393,17 +393,32 @@
         self.content = self._raw_content
 
         self._apply_process_fixups()
 
 
 class MarkdownDocumentNode(DocumentNode):
     """A node representing a Markdown document."""
-    def __init__(self, md, **kwargs):
+    def __init__(self, configuration, **kwargs):
         super().__init__(**kwargs)
-        self.__md = md
+        self.__md = self._create_markdown_processor(configuration)
+
+    def _create_markdown_processor(self, configuration):
+        from markdown import Markdown
+        from .md import LiaraMarkdownExtensions
+
+        extensions = [
+            LiaraMarkdownExtensions(self)
+        ] + configuration['content.markdown.extensions']
+
+        extension_configs = configuration['content.markdown.config']
+        output = configuration['content.markdown.output']
+
+        return Markdown(extensions=extensions,
+                        extension_configs=extension_configs,
+                        output=output)
 
     def process(self, cache: Cache):
         import hashlib
         from .md import ShortcodeException
 
         byte_content = self._raw_content.encode('utf-8')
         content_hash = hashlib.sha256(byte_content).digest()
@@ -411,17 +426,18 @@
             self.content = content
             return
 
         # We re-raise shortcode exceptions to adjust the line number to
         # make debugging easier
         try:
             self.content = self.__md.convert(self._raw_content)
-            self.__md.reset()
         except ShortcodeException as sx:
             raise sx.with_line_offset(self._content_line_start) from sx
+        finally:
+            self.__md.reset()
 
         self._apply_process_fixups()
 
         cache.put(content_hash, self.content)
 
 
 class DataNode(Node):
@@ -781,40 +797,25 @@
         self.__process_fixups = []
 
         self.__setup_fixups(configuration)
 
         self.register_type(
             ['.md'], MarkdownDocumentNode,
             extra_args={
-                'md': self._create_markdown_processor(configuration)
+                'configuration': configuration
             })
         self.register_type(['.html'], HtmlDocumentNode)
 
     def _on_node_created(self, node):
         node.set_fixups(
             load_fixups=self.__load_fixups,
             process_fixups=self.__process_fixups)
         node.load()
         return node
 
-    def _create_markdown_processor(self, configuration):
-        from markdown import Markdown
-        from .md import LiaraMarkdownExtensions
-
-        extensions = [
-            LiaraMarkdownExtensions()
-        ] + configuration['content.markdown.extensions']
-
-        extension_configs = configuration['content.markdown.config']
-        output = configuration['content.markdown.output']
-
-        return Markdown(extensions=extensions,
-                        extension_configs=extension_configs,
-                        output=output)
-
 
 class StaticNode(Node):
     """A static data node.
 
     Static nodes are suitable for large static data which never changes, for
     instance, binary files, videos, images etc.
     """
```

### Comparing `Liara-2.5.3/liara/plugins/has_pending_document.py` & `Liara-2.5.4/liara/plugins/has_pending_document.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.3/liara/plugins/series_schedule.py` & `Liara-2.5.4/liara/plugins/series_schedule.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.3/liara/publish.py` & `Liara-2.5.4/liara/publish.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.3/liara/query.py` & `Liara-2.5.4/liara/query.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.3/liara/quickstart.py` & `Liara-2.5.4/liara/quickstart.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.3/liara/server.py` & `Liara-2.5.4/liara/server.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.3/liara/signals.py` & `Liara-2.5.4/liara/signals.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.3/liara/site.py` & `Liara-2.5.4/liara/site.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.3/liara/template.py` & `Liara-2.5.4/liara/template.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.3/liara/util.py` & `Liara-2.5.4/liara/util.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.3/liara/yaml.py` & `Liara-2.5.4/liara/yaml.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.3/setup.cfg` & `Liara-2.5.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `Liara-2.5.3/test/test_md.py` & `Liara-2.5.4/test/test_md.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.3/test/test_nodes.py` & `Liara-2.5.4/test/test_nodes.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.3/test/test_query.py` & `Liara-2.5.4/test/test_query.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.3/test/test_site.py` & `Liara-2.5.4/test/test_site.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.3/test/test_template.py` & `Liara-2.5.4/test/test_template.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.3/test/test_util.py` & `Liara-2.5.4/test/test_util.py`

 * *Files identical despite different names*

