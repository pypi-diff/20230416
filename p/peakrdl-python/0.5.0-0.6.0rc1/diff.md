# Comparing `tmp/peakrdl-python-0.5.0.tar.gz` & `tmp/peakrdl-python-0.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakrdl-python-0.5.0.tar", last modified: Sun Mar 12 17:45:10 2023, max compression
+gzip compressed data, was "peakrdl-python-0.6.0rc1.tar", last modified: Sun Apr 16 18:46:48 2023, max compression
```

## Comparing `peakrdl-python-0.5.0.tar` & `peakrdl-python-0.6.0rc1.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:45:10.964576 peakrdl-python-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-03-12 17:45:10.964576 peakrdl-python-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-12 17:45:10.964576 peakrdl-python-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:45:10.960576 peakrdl-python-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:45:10.960576 peakrdl-python-0.5.0/src/peakrdl_python/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/src/peakrdl_python/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/src/peakrdl_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/src/peakrdl_python/__peakrdl__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/src/peakrdl_python/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:45:10.964576 peakrdl-python-0.5.0/src/peakrdl_python/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/src/peakrdl_python/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/src/peakrdl_python/lib/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/src/peakrdl_python/lib/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    27632 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/src/peakrdl_python/lib/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    27934 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/src/peakrdl_python/lib/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    31302 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/src/peakrdl_python/lib/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/src/peakrdl_python/peakpython.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/src/peakrdl_python/safe_name_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/src/peakrdl_python/systemrdl_node_utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:45:10.964576 peakrdl-python-0.5.0/src/peakrdl_python/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/src/peakrdl_python/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21835 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/src/peakrdl_python/templates/addrmap.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/src/peakrdl_python/templates/addrmap_field.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/src/peakrdl_python/templates/addrmap_memory.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/src/peakrdl_python/templates/addrmap_register.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/src/peakrdl_python/templates/addrmap_simulation.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/src/peakrdl_python/templates/addrmap_simulation_tb.jinja
--rw-r--r--   0 runner    (1001) docker     (123)    78053 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/src/peakrdl_python/templates/addrmap_tb.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/src/peakrdl_python/templates/header.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/src/peakrdl_python/templates/header_tb.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-03-12 17:45:09.000000 peakrdl-python-0.5.0/src/peakrdl_python/templates/reg_definitions.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:45:10.960576 peakrdl-python-0.5.0/src/peakrdl_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-03-12 17:45:10.000000 peakrdl-python-0.5.0/src/peakrdl_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-03-12 17:45:10.000000 peakrdl-python-0.5.0/src/peakrdl_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 17:45:10.000000 peakrdl-python-0.5.0/src/peakrdl_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-12 17:45:10.000000 peakrdl-python-0.5.0/src/peakrdl_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-12 17:45:10.000000 peakrdl-python-0.5.0/src/peakrdl_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-12 17:45:10.000000 peakrdl-python-0.5.0/src/peakrdl_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:46:48.203227 peakrdl-python-0.6.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-16 18:46:48.203227 peakrdl-python-0.6.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 18:46:48.203227 peakrdl-python-0.6.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:46:48.199227 peakrdl-python-0.6.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:46:48.199227 peakrdl-python-0.6.0rc1/src/peakrdl_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/__peakrdl__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/_node_walkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17790 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:46:48.199227 peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27632 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27934 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31302 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/peakpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/safe_name_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/systemrdl_node_utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:46:48.203227 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21835 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_field.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_memory.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_register.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_simulation.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_simulation_tb.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)    72721 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_tb.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/baseclass_tb.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/header.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/header_tb.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/reg_definitions.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:46:48.199227 peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-16 18:46:48.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-16 18:46:48.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 18:46:48.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-16 18:46:48.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-16 18:46:48.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-16 18:46:48.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/top_level.txt
```

### Comparing `peakrdl-python-0.5.0/LICENSE` & `peakrdl-python-0.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.5.0/PKG-INFO` & `peakrdl-python-0.6.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakrdl-python
-Version: 0.5.0
+Version: 0.6.0rc1
 Summary: Generate python wrapper for a register model compiled SystemRDL input
 Home-page: https://github.com/krcb197/PeakRDL-python
 Author: Keith Brady
 License: UNKNOWN
 Project-URL: Source, https://github.com/krcb197/PeakRDL-python
 Project-URL: Tracker, https://github.com/krcb197/PeakRDL-python/issues
 Project-URL: Documentation, https://peakrdl-python.readthedocs.io/
```

### Comparing `peakrdl-python-0.5.0/setup.py` & `peakrdl-python-0.6.0rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     include_package_data = True,
     entry_points= { 'console_scripts' : ['peakrdl_python=peakrdl_python.peakpython:main_function'],
                     "peakrdl.exporters": [
                         'python = peakrdl_python.__peakrdl__:Exporter'
                     ]
                     },
     install_requires=[
-        "systemrdl-compiler>=1.21.0",
+        "systemrdl-compiler>=1.24.0",
         "autopep8",
         "pylint",
         "coverage",
         "jinja2",
         "asynctest;python_version<'3.8'",
         "peakrdl-ipxact"
     ],
```

### Comparing `peakrdl-python-0.5.0/src/peakrdl_python/__peakrdl__.py` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/__peakrdl__.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.5.0/src/peakrdl_python/exporter.py` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/exporter.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pathlib import Path
 from shutil import copyfile
 from typing import List, NoReturn, Iterable, Tuple
 from glob import glob
 
 import autopep8 # type: ignore
 import jinja2 as jj
+from systemrdl import RDLWalker # type: ignore
 
 from systemrdl.node import RootNode, Node, RegNode, AddrmapNode, RegfileNode # type: ignore
 from systemrdl.node import FieldNode, MemNode, AddressableNode # type: ignore
 from systemrdl.node import SignalNode # type: ignore
 from systemrdl.rdltypes import OnReadType, OnWriteType, PropertyReference  # type: ignore
 from systemrdl.rdltypes.user_enum import UserEnumMeta  # type: ignore
 
@@ -24,14 +25,16 @@
     get_memory_max_entry_value_hex_string, get_memory_width_bytes, \
     get_field_default_value, get_enum_values
 
 from .lib import get_array_typecode
 
 from .safe_name_utility import get_python_path_segments, safe_node_name
 
+from ._node_walkers import AddressMaps, OwnedbyAddressMap
+
 from .__about__ import __version__
 
 file_path = os.path.dirname(__file__)
 
 class PythonExportTemplateError(Exception):
     """
     Exception for hading errors in the templating
@@ -111,95 +114,162 @@
         Returns:
             List[str] : modules that have been exported:
         """
         # pylint: disable=too-many-locals
 
         # If it is the root node, skip to top addrmap
         if isinstance(node, RootNode):
-            node = node.top
+            top_block = node.top
+        else:
+            top_block = node
 
         package_path = os.path.join(path, node.inst_name)
         self._create_empty_package(package_path=package_path,
                                    skip_test_case_generation=skip_test_case_generation)
 
-        modules = [node]
+        self._build_node_type_table(top_block)
 
-        for block in modules:
+        context = {
+            'print': print,
+            'type': type,
+            'top_node': top_block,
+            'systemrdlFieldNode': FieldNode,
+            'systemrdlRegNode': RegNode,
+            'systemrdlRegfileNode': RegfileNode,
+            'systemrdlAddrmapNode': AddrmapNode,
+            'systemrdlMemNode': MemNode,
+            'systemrdlAddressableNode': AddressableNode,
+            'systemrdlSignalNode': SignalNode,
+            'asyncoutput': asyncoutput,
+            'OnWriteType': OnWriteType,
+            'OnReadType': OnReadType,
+            'PropertyReference': PropertyReference,
+            'isinstance': isinstance,
+            'uses_enum' : uses_enum(top_block),
+            'uses_memory' : uses_memory(top_block),
+            'get_fully_qualified_type_name': self._lookup_type_name,
+            'get_array_dim': get_array_dim,
+            'get_dependent_component': get_dependent_component,
+            'get_dependent_enum': self._get_dependent_enum,
+            'get_enum_values': get_enum_values,
+            'get_fully_qualified_enum_type': self._fully_qualified_enum_type,
+            'get_field_bitmask_hex_string': get_field_bitmask_hex_string,
+            'get_field_inv_bitmask_hex_string': get_field_inv_bitmask_hex_string,
+            'get_field_max_value_hex_string': get_field_max_value_hex_string,
+            'get_reg_max_value_hex_string': get_reg_max_value_hex_string,
+            'get_table_block': get_table_block,
+            'get_reg_writable_fields': get_reg_writable_fields,
+            'get_reg_readable_fields': get_reg_readable_fields,
+            'get_memory_max_entry_value_hex_string': get_memory_max_entry_value_hex_string,
+            'get_array_typecode': get_array_typecode,
+            'get_memory_width_bytes': get_memory_width_bytes,
+            'get_field_default_value': get_field_default_value,
+            'raise_template_error' : self._raise_template_error,
+            'get_python_path_segments' : get_python_path_segments,
+            'safe_node_name' : safe_node_name,
+            'version' : __version__
+        }
+
+        context.update(self.user_template_context)
+
+        template = self.jj_env.get_template("addrmap.py.jinja")
+        module_fqfn = os.path.join(package_path,
+                                   'reg_model',
+                                   top_block.inst_name + '.py')
+        if autoformatoutputs is True:
+            module_code_str = autopep8.fix_code(template.render(context))
+            with open(module_fqfn, "w", encoding='utf-8') as fid:
+                fid.write(module_code_str)
+        else:
+            stream = template.stream(context)
+            stream.dump(module_fqfn, encoding='utf-8')
 
-            self._build_node_type_table(block)
+        if not skip_test_case_generation:
+
+            # make the top level base class for all the other test, this is what instantes
+            # the register model
+            template = self.jj_env.get_template("baseclass_tb.py.jinja")
+            module_tb_fqfn = os.path.join(package_path,
+                                          'tests',
+                                          '_' + top_block.inst_name + '_test_base.py')
 
             context = {
-                'print': print,
-                'type': type,
-                'top_node': block,
-                'systemrdlFieldNode': FieldNode,
-                'systemrdlRegNode': RegNode,
-                'systemrdlRegfileNode': RegfileNode,
-                'systemrdlAddrmapNode': AddrmapNode,
-                'systemrdlMemNode': MemNode,
-                'systemrdlAddressableNode': AddressableNode,
-                'systemrdlSignalNode': SignalNode,
+                'top_node': top_block,
                 'asyncoutput': asyncoutput,
-                'OnWriteType': OnWriteType,
-                'OnReadType': OnReadType,
-                'PropertyReference': PropertyReference,
-                'isinstance': isinstance,
-                'uses_enum' : uses_enum(block),
-                'uses_memory' : uses_memory(block),
-                'get_fully_qualified_type_name': self._lookup_type_name,
-                'get_array_dim': get_array_dim,
-                'get_dependent_component': get_dependent_component,
-                'get_dependent_enum': self._get_dependent_enum,
-                'get_enum_values': get_enum_values,
-                'get_fully_qualified_enum_type': self._fully_qualified_enum_type,
-                'get_field_bitmask_hex_string': get_field_bitmask_hex_string,
-                'get_field_inv_bitmask_hex_string': get_field_inv_bitmask_hex_string,
-                'get_field_max_value_hex_string': get_field_max_value_hex_string,
-                'get_reg_max_value_hex_string': get_reg_max_value_hex_string,
-                'get_table_block': get_table_block,
-                'get_reg_writable_fields': get_reg_writable_fields,
-                'get_reg_readable_fields': get_reg_readable_fields,
-                'get_memory_max_entry_value_hex_string': get_memory_max_entry_value_hex_string,
-                'get_array_typecode': get_array_typecode,
-                'get_memory_width_bytes': get_memory_width_bytes,
-                'get_field_default_value': get_field_default_value,
-                'raise_template_error' : self._raise_template_error,
-                'get_python_path_segments' : get_python_path_segments,
-                'safe_node_name' : safe_node_name,
-                'version' : __version__
+                'version': __version__
             }
 
-            context.update(self.user_template_context)
-
-            template = self.jj_env.get_template("addrmap.py.jinja")
-            module_fqfn = os.path.join(package_path,
-                                       'reg_model',
-                                       block.inst_name + '.py')
             if autoformatoutputs is True:
-                module_code_str = autopep8.fix_code(template.render(context))
-                with open(module_fqfn, "w", encoding='utf-8') as fid:
-                    fid.write(module_code_str)
+                module_tb_code_str = autopep8.fix_code(template.render(context))
+                with open(module_tb_fqfn, "w", encoding='utf-8') as fid:
+                    fid.write(module_tb_code_str)
             else:
                 stream = template.stream(context)
-                stream.dump(module_fqfn, encoding='utf-8')
+                stream.dump(module_tb_fqfn, encoding='utf-8')
+
+            # make the tests themselves
+            template = self.jj_env.get_template("addrmap_tb.py.jinja")
+
+            blocks = AddressMaps()
+            # running the walker populated the blocks with all the address maps in within the
+            # top block, including the top_block itself
+            RDLWalker(unroll=True).walk(top_block, blocks, skip_top=False)
+
+            for block in blocks:
+                owned_elements = OwnedbyAddressMap()
+                # running the walker populated the blocks with all the address maps in within the
+                # top block, including the top_block itself
+                RDLWalker(unroll=True).walk(block, owned_elements, skip_top=True)
+
+                fq_block_name = '_'.join(block.get_path_segments(array_suffix = '_{index:d}_'))
 
-            if not skip_test_case_generation:
-                template = self.jj_env.get_template("addrmap_tb.py.jinja")
                 module_tb_fqfn = os.path.join(package_path,
                                               'tests',
-                                              'test_' + block.inst_name + '.py')
+                                              'test_' + fq_block_name + '.py')
+
+                context = {
+                    'top_node': top_block,
+                    'block' : block,
+                    'fq_block_name' : fq_block_name,
+                    'owned_elements': owned_elements,
+                    'systemrdlFieldNode': FieldNode,
+                    'systemrdlSignalNode': SignalNode,
+                    'systemrdlRegNode': RegNode,
+                    'systemrdlMemNode': MemNode,
+                    'systemrdlRegfileNode': RegfileNode,
+                    'systemrdlAddrmapNode': AddrmapNode,
+                    'isinstance': isinstance,
+                    'get_python_path_segments': get_python_path_segments,
+                    'safe_node_name': safe_node_name,
+                    'uses_memory': (len(owned_elements.memories) > 0),
+                    'get_field_bitmask_hex_string': get_field_bitmask_hex_string,
+                    'get_field_inv_bitmask_hex_string': get_field_inv_bitmask_hex_string,
+                    'get_field_max_value_hex_string': get_field_max_value_hex_string,
+                    'get_field_default_value': get_field_default_value,
+                    'get_reg_max_value_hex_string': get_reg_max_value_hex_string,
+                    'get_reg_writable_fields': get_reg_writable_fields,
+                    'get_reg_readable_fields': get_reg_readable_fields,
+                    'get_memory_max_entry_value_hex_string': get_memory_max_entry_value_hex_string,
+                    'get_enum_values': get_enum_values,
+                    'get_array_typecode': get_array_typecode,
+                    'get_memory_width_bytes': get_memory_width_bytes,
+                    'asyncoutput': asyncoutput,
+                    'uses_enum': uses_enum(block),
+                    'version': __version__
+                }
+
                 if autoformatoutputs is True:
                     module_tb_code_str = autopep8.fix_code(template.render(context))
                     with open(module_tb_fqfn, "w", encoding='utf-8') as fid:
                         fid.write(module_tb_code_str)
                 else:
                     stream = template.stream(context)
                     stream.dump(module_tb_fqfn, encoding='utf-8')
 
-        return [m.inst_name for m in modules]
+        return top_block.inst_name
 
     def _lookup_type_name(self, node: Node) -> str:
         """
         Retreive the unique type name from the current lookup list
 
         Args:
             node: node to lookup
```

### Comparing `peakrdl-python-0.5.0/src/peakrdl_python/lib/__init__.py` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.5.0/src/peakrdl_python/lib/base.py` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/base.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.5.0/src/peakrdl_python/lib/callbacks.py` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/callbacks.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.5.0/src/peakrdl_python/lib/fields.py` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/fields.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.5.0/src/peakrdl_python/lib/memory.py` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/memory.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.5.0/src/peakrdl_python/lib/register.py` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/register.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.5.0/src/peakrdl_python/peakpython.py` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/peakpython.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.5.0/src/peakrdl_python/safe_name_utility.py` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/safe_name_utility.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.5.0/src/peakrdl_python/systemrdl_node_utility_functions.py` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/systemrdl_node_utility_functions.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.5.0/src/peakrdl_python/templates/addrmap.py.jinja` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.5.0/src/peakrdl_python/templates/addrmap_field.py.jinja` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_field.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.5.0/src/peakrdl_python/templates/addrmap_memory.py.jinja` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_memory.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.5.0/src/peakrdl_python/templates/addrmap_register.py.jinja` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_register.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.5.0/src/peakrdl_python/templates/addrmap_tb.py.jinja` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_tb.py.jinja`

 * *Files 7% similar despite different names*

```diff
@@ -16,20 +16,14 @@
 {% endif %}
 import random
 from itertools import combinations
 import math
 from enum import IntEnum
 
 from ..lib import RegisterWriteVerifyError
-{% if asyncoutput %}
-from ..lib import AsyncCallbackSet
-{% else %}
-from ..lib import NormalCallbackSet
-{% endif %}
-
 
 from ..reg_model.{{top_node.type_name}} import {{top_node.type_name}}_cls
 {% if asyncoutput %}
 from ..lib import FieldAsyncReadOnly, FieldAsyncWriteOnly, FieldAsyncReadWrite
 from ..lib import WritableAsyncRegister, ReadableAsyncRegister, RegAsyncReadWrite, RegAsyncReadOnly, RegAsyncWriteOnly
 from ..lib import MemoryAsyncReadOnly, MemoryAsyncWriteOnly, MemoryAsyncReadWrite
 {% else %}
@@ -38,156 +32,65 @@
 from ..lib import MemoryReadOnly, MemoryWriteOnly, MemoryReadWrite
 {% endif %}
 from ..lib import AddressMap, RegFile
 from ..lib import Memory
 from ..lib import Field
 from ..lib import Reg
 
-# dummy functions to support the test cases, note that these are not used as
-# they get patched
-{% if asyncoutput %}async {% endif %}def read_addr_space(addr: int, width: int, accesswidth: int) -> int:
-    assert isinstance(addr, int)
-    assert isinstance(width, int)
-    assert isinstance(accesswidth, int)
-    {% if asyncoutput %}await asyncio.sleep(1) {% endif %}
-    return 0
-
-{% if asyncoutput %}async {% endif %}def write_addr_space(addr: int, width: int, accesswidth: int,  data: int) -> None:
-    assert isinstance(addr, int)
-    assert isinstance(width, int)
-    assert isinstance(accesswidth, int)
-    assert isinstance(data, int)
-    {% if asyncoutput %}await asyncio.sleep(1) {% endif %}
-
-{% if asyncoutput %}async {% endif %}def read_callback(addr: int, width: int, accesswidth: int) -> int:
-    return {% if asyncoutput %}await {% endif %}read_addr_space(addr=addr, width=width, accesswidth=accesswidth)
-
-{% if asyncoutput %}async {%endif %}def read_block_addr_space(addr: int, width: int, accesswidth: int, length:int) -> Array:
-    assert isinstance(addr, int)
-    assert isinstance(width, int)
-    assert isinstance(accesswidth, int)
-    assert isinstance(length, int)
-
-    if width == 32:
-        typecode = 'L'
-    elif width == 64:
-        typecode = 'Q'
-    elif width == 16:
-        typecode = 'I'
-    elif width == 8:
-        typecode = 'B'
-    else:
-        raise ValueError('unhandled memory width')
-
-    {% if asyncoutput %}await asyncio.sleep(1) {% endif %}
-    return Array(typecode, [0 for x in range(length)])
-
-{% if asyncoutput %}async {%endif %}def read_block_callback(addr: int, width: int, accesswidth: int, length: int) -> Array:
-    return {% if asyncoutput %}await {% endif %}read_block_addr_space(addr=addr, width=width, accesswidth=accesswidth, length=length)
-
-{% if asyncoutput %}async {%endif %}def write_callback(addr: int, width: int, accesswidth: int,  data: int) -> None:
-    {% if asyncoutput %}await {% endif %}write_addr_space(addr=addr, width=width, accesswidth=accesswidth, data=data)
-
-{% if asyncoutput %}async {%endif %}def write_block_addr_space(addr: int, width: int, accesswidth: int,  data: Array) -> None:
-    assert isinstance(addr, int)
-    assert isinstance(width, int)
-    assert isinstance(accesswidth, int)
-    assert isinstance(data, Array)
-    {% if asyncoutput %}await asyncio.sleep(1) {% endif %}
-
-{% if asyncoutput %}async {%endif %}def write_block_callback(addr: int, width: int, accesswidth: int,  data: Array) -> None:
-    {% if asyncoutput %}await {% endif %}write_block_addr_space(addr=addr, width=width, accesswidth=accesswidth, data=data)
-
-{% if asyncoutput %}
-if sys.version_info < (3, 8):
-    TestCaseBase = asynctest.TestCase
-else:
-    TestCaseBase = unittest.IsolatedAsyncioTestCase
-{% else %}
-TestCaseBase = unittest.TestCase
-{% endif %}
-
-class {{top_node.type_name}}_TestCase(TestCaseBase): # type: ignore[valid-type,misc]
-
-    def setUp(self) -> None:
-        self.dut = {{top_node.type_name}}_cls({% if asyncoutput %}AsyncCallbackSet{% else %}NormalCallbackSet{% endif %}(read_callback=read_callback,
-                                                          write_callback=write_callback))
-
-    @staticmethod
-    def _reverse_bits(value: int, number_bits: int) -> int:
-        """
+from ._{{top_node.inst_name}}_test_base import {{top_node.type_name}}_TestCase, {{top_node.type_name}}_TestCase_BlockAccess
+from ._{{top_node.inst_name}}_test_base import __name__ as base_name
 
-        Args:
-            value: value to reverse
-            number_bits: number of bits used in the value
-
-        Returns:
-            reversed valued
-        """
-        result = 0
-        for i in range(number_bits):
-            if (value >> i) & 1:
-                result |= 1 << (number_bits - 1 - i)
-        return result
+class {{fq_block_name}}_single_access({{top_node.type_name}}_TestCase): # type: ignore[valid-type,misc]
 
     def test_inst_name(self)  -> None:
         """
         Walk the address map and check the inst name has been correctly populated
         """
-        {% for node in top_node.descendants(unroll=True) -%}
-        {% if isinstance(node, systemrdlSignalNode) %}
-        # doing nothing with signal node: {{node.inst_name}}
-        {% else %}
+        {% for node in owned_elements.nodes -%}
         with self.subTest(msg='node: {{'.'.join(node.get_path_segments())}}'):
             self.assertEqual(self.dut.{{'.'.join(get_python_path_segments(node))}}.inst_name, '{{node.get_path_segments()[-1]}}') # type: ignore[union-attr]
             self.assertEqual(self.dut.{{'.'.join(get_python_path_segments(node))}}.full_inst_name, '{{'.'.join(node.get_path_segments())}}')  # type: ignore[union-attr]
-        {% endif %}
         {% endfor %}
 
     def test_register_properties(self)  -> None:
         """
         Walk the address map and check the address, size and accesswidth of every register is
         correct
         """
-        {%- for node in top_node.descendants(unroll=True) -%}
-            {%- if isinstance(node, systemrdlRegNode) %}
+        {% for node in owned_elements.registers -%}
         with self.subTest(msg='register: {{'.'.join(node.get_path_segments())}}'):
             self.assertEqual(self.dut.{{'.'.join(get_python_path_segments(node))}}.address, {{node.absolute_address}}) # type: ignore[union-attr]
             self.assertEqual(self.dut.{{'.'.join(get_python_path_segments(node))}}.width, {{node.size * 8}}) # type: ignore[union-attr]
             {% if 'accesswidth' in node.list_properties() -%}self.assertEqual(self.dut.{{'.'.join(get_python_path_segments(node))}}.accesswidth, {{node.get_property('accesswidth')}}){%- else -%} self.assertEqual(self.dut.{{'.'.join(get_python_path_segments(node))}}.accesswidth, self.dut.{{'.'.join(get_python_path_segments(node))}}.accesswidth){%- endif %} # type: ignore[union-attr]
-            {%- endif %}
-        {%- endfor %}
+        {% endfor %}
 
     def test_memory_properties(self)  -> None:
         """
         Walk the address map and check the address, size and accesswidth of every memory is
         correct
         """
         mut: Memory
-        {%- for node in top_node.descendants(unroll=True) -%}
-            {%- if isinstance(node, systemrdlMemNode) %}
+        {% for node in owned_elements.memories -%}
         with self.subTest(msg='memory: {{'.'.join(node.get_path_segments())}}'):
             mut = self.dut.{{'.'.join(get_python_path_segments(node))}} # type: ignore[union-attr,assignment]
             self.assertIsInstance(mut, Memory)
             self.assertEqual(mut.address, {{node.absolute_address}})
             self.assertEqual(mut.width, {{node.get_property('memwidth')}})
             self.assertEqual(mut.entries, {{node.get_property('mementries')}})
             {% if 'accesswidth' in node.list_properties() -%}self.assertEqual(mut.accesswidth, {{node.get_property('accesswidth')}}){%- else -%}self.assertEqual(mut.accesswidth, mut.accesswidth){%- endif %}
-            {%- endif %}
-        {%- endfor %}
+        {% endfor %}
 
     def test_field_properties(self)  -> None:
         """
         walk the address map and check:
         - that the lsb and msb of every field is correct
         - that where default values are provided they are applied correctly
         """
         fut:Field
-        {%- for node in top_node.descendants(unroll=True) -%}
-            {%- if isinstance(node, systemrdlFieldNode) %}
+        {% for node in owned_elements.fields -%}
         with self.subTest(msg='field: {{'.'.join(node.get_path_segments())}}'):
             # test properties of field: {{'.'.join(node.get_path_segments())}}
             fut = self.dut.{{'.'.join(get_python_path_segments(node))}} # type: ignore[union-attr]
             if not isinstance(fut, Field):
                 raise TypeError('This test relies on node being of type Field')
             self.assertEqual(fut.lsb,{{node.lsb}})
             self.assertEqual(fut.msb,{{node.msb}})
@@ -203,30 +106,28 @@
                     {% else %}
             self.assertIsNone(fut.default)
                     {% endif %}
                 {% else %}
             self.assertEqual(fut.default,{{get_field_default_value(node)}})
                 {% endif %}
             self.assertEqual(fut.is_volatile,{{node.is_hw_writable}})
-            {%- endif -%}
-        {%- endfor %}
+        {% endfor %}
 
     {% if asyncoutput %}async {% endif %}def test_register_read_and_write(self) -> None:
         """
         Walk the register map and check every register can be read and written to correctly
         """
         rut: Reg
-        {%- for node in top_node.descendants(unroll=True) -%}
-            {%- if isinstance(node, systemrdlRegNode) %}
+        {% for node in owned_elements.registers -%}
         # test access operations (read and/or write) to register:
         # {{'.'.join(node.get_path_segments())}}
         with self.subTest(msg='register: {{'.'.join(node.get_path_segments())}}'):
             rut=self.dut.{{'.'.join(get_python_path_segments(node))}} # type: ignore[union-attr,assignment]
-            with patch(__name__ + '.' + 'write_addr_space') as write_callback_mock, \
-                patch(__name__ + '.' + 'read_addr_space', return_value=1) as read_callback_mock:
+            with patch(base_name + '.write_addr_space') as write_callback_mock, \
+                patch(base_name + '.read_addr_space', return_value=1) as read_callback_mock:
 
                 {% if node.has_sw_readable -%}
                 {% if asyncoutput %}
                 if not isinstance(rut, (RegAsyncReadOnly, RegAsyncReadWrite)):
                     raise TypeError('Register is not a Readable Async Type')
                 {% else %}
                 if not isinstance(rut, (RegReadOnly, RegReadWrite)):
@@ -319,32 +220,30 @@
                 # test that a non-writable register has no write method and attempting one generates and error
                 with self.assertRaises(AttributeError):
                     {% if asyncoutput %}await {%endif %}rut.write(0) # type: ignore[attr-defined]
                 {%- endif %}
 
                 # check the read has not been called in the write test
                 read_callback_mock.assert_not_called()
-            {%- endif %}
-        {%- endfor %}
+        {% endfor %}
 
     {% if asyncoutput %}async {% endif %}def test_int_field_read_and_write(self) -> None:
         """
         Check the ability to read and write to integer (non-eumn) fields
         """
         fut:Field
-    {%- for node in top_node.descendants(unroll=True) -%}
-        {%- if isinstance(node, systemrdlFieldNode) %}
+        {% for node in owned_elements.fields -%}
         {%- if 'encode' not in node.list_properties() %}
 
         # test access operations (read and/or write) to field:
         # {{'.'.join(node.get_path_segments())}}
         with self.subTest(msg='field: {{'.'.join(node.get_path_segments())}}'):
             fut = self.dut.{{'.'.join(get_python_path_segments(node))}} # type: ignore[union-attr]
-            with patch(__name__ + '.' + 'write_addr_space') as write_callback_mock,\
-                patch(__name__ + '.' + 'read_addr_space', return_value=0) as read_callback_mock:
+            with patch(base_name + '.write_addr_space') as write_callback_mock,\
+                patch(base_name + '.read_addr_space', return_value=0) as read_callback_mock:
 
                 {% if node.is_sw_readable %}
                 {% if asyncoutput %}
                 if not isinstance(fut, (FieldAsyncReadOnly, FieldAsyncReadWrite)):
                     raise TypeError('Test can not proceed as the fut is not a readable async field')
                 {% else %}
                 if not isinstance(fut, (FieldReadOnly, FieldReadWrite)):
@@ -458,31 +357,29 @@
                     {% if asyncoutput %}await {%endif %}fut.write({{ get_field_max_value_hex_string(node) }} + 1)
 
                 with self.assertRaises(ValueError):
                     {% if asyncoutput %}await {%endif %}fut.write(-1)
                 {%- endif %}
 
         {%- endif %}
-        {%- endif %}
     {%- endfor %}
 
     {% if uses_enum %}
     {% if asyncoutput %}async {% endif %}def test_enum_field_read_and_write(self) -> None:
         """
         Check the ability to read and write to enum fields
         """
-    {%- for node in top_node.descendants(unroll=True) -%}
-        {%- if isinstance(node, systemrdlFieldNode) %}
+    {% for node in owned_elements.fields -%}
         {%- if 'encode' in node.list_properties() %}
 
         # test access operations (read and/or write) to field:
         # {{'.'.join(node.get_path_segments())}}
         with self.subTest(msg='field: {{'.'.join(node.get_path_segments())}}'):
-            with patch(__name__ + '.' + 'write_addr_space') as write_callback_mock,\
-                patch(__name__ + '.' + 'read_addr_space', return_value=0) as read_callback_mock:
+            with patch(base_name + '.write_addr_space') as write_callback_mock,\
+                patch(base_name + '.read_addr_space', return_value=0) as read_callback_mock:
 
                 {% if node.is_sw_readable %}
                 # read back test
                 {%- for value_of_enum_needed in node.get_property('encode') -%}
                 # set the simulated read_back value to {{value_of_enum_needed.name.upper()}}
                 random_reg_value = random.randrange(0, {{get_reg_max_value_hex_string(node.parent)}} + 1)
                 read_callback_mock.reset_mock()
@@ -574,25 +471,23 @@
                 {% endif -%}
                 {% endif %}
 
                 {% endfor %}
                 {% endif %}
 
         {%- endif %}
-        {%- endif %}
     {%- endfor %}
     {%- endif %}
 
     {% if asyncoutput %}async {% endif %}def test_register_read_fields(self) -> None:
         """
         Walk the register map and check every register read_fields method
         """
         reference_read_fields: Dict[str, Union[bool, IntEnum, int]]
-        {%- for node in top_node.descendants(unroll=True) -%}
-        {%- if isinstance(node, systemrdlRegNode) %}
+        {% for node in owned_elements.registers -%}
         {% if node.has_sw_readable %}
         with self.subTest(msg='register: {{'.'.join(node.get_path_segments())}}'):
             # test read_fields to register:
             # {{'.'.join(node.get_path_segments())}}
             # build up the register value with a random base value, overlaid with
             # a random value for each field
             rand_reg_value = random.randrange(0, {{get_reg_max_value_hex_string(node)}} + 1)
@@ -612,16 +507,16 @@
             rand_reg_value = (rand_reg_value & {{get_field_inv_bitmask_hex_string(child_node)}}) | (self._reverse_bits(value=rand_field_value, number_bits={{child_node.width}}) << {{ child_node.low }})
                          {% endif %}
                     {% endif %}
                 {% else %}
             {{ raise_template_error('unexpected type') }}
                 {% endif %}
             {% endfor %}
-            with patch(__name__ + '.' + 'write_addr_space') as write_callback_mock, \
-                 patch(__name__ + '.' + 'read_addr_space', return_value=rand_reg_value) as read_callback_mock:
+            with patch(base_name + '.write_addr_space') as write_callback_mock, \
+                 patch(base_name + '.read_addr_space', return_value=rand_reg_value) as read_callback_mock:
                 # the read_fields method gets a dictionary back
                 # from the object with all the read back field
                 # values
                 reference_read_fields = { {% for child_node in node.children() -%}
                                             {% if isinstance(child_node, systemrdlFieldNode) %}
                                                 {%- if child_node.is_sw_readable %}
                                           '{{ child_node.inst_name }}' : {% if asyncoutput %}await {%endif %}self.dut.{{'.'.join(get_python_path_segments(child_node))}}.read(){%- if not loop.last -%}, {%- endif %} # type: ignore[union-attr]
@@ -634,24 +529,22 @@
 
                 self.assertDictEqual({% if asyncoutput %}await {% endif %}self.dut.{{'.'.join(get_python_path_segments(node))}}.read_fields(), # type: ignore[union-attr]
                                      reference_read_fields)
                 read_callback_mock.assert_called_once()
                 write_callback_mock.assert_not_called()
 
         {%- endif %}
-        {%- endif %}
         {%- endfor %}
 
     {% if asyncoutput %}async {% endif %}def test_register_read_context_manager(self) -> None:
         """
         Walk the register map and check every register read_fields method
         """
         reference_read_fields: Dict[str, Union[bool, IntEnum, int]]
-        {%- for node in top_node.descendants(unroll=True) -%}
-        {%- if isinstance(node, systemrdlRegNode) %}
+        {% for node in owned_elements.registers -%}
         {% if node.has_sw_readable %}
         # test context manager to register:
         # {{'.'.join(node.get_path_segments())}}
         # build up the register value with a random base value, overlaid with
         # a random value for each field
         with self.subTest(msg='register: {{'.'.join(node.get_path_segments())}}'):
             rand_reg_value = random.randrange(0, {{get_reg_max_value_hex_string(node)}} + 1)
@@ -669,16 +562,16 @@
             rand_reg_value = (rand_reg_value & {{get_field_inv_bitmask_hex_string(field)}}) | (self._reverse_bits(value=rand_field_value, number_bits={{field.width}}) << {{ field.low }})
                         {% endif %}
                     {% endif %}
                 {% else %}
                 # skipping {{field.inst_name}}
                 {% endif %}
             {% endfor %}
-            with patch(__name__ + '.' + 'write_addr_space') as write_callback_mock, \
-                 patch(__name__ + '.' + 'read_addr_space', return_value=rand_reg_value) as read_callback_mock:
+            with patch(base_name + '.write_addr_space') as write_callback_mock, \
+                 patch(base_name + '.read_addr_space', return_value=rand_reg_value) as read_callback_mock:
 
                 # first read the fields using the "normal" method, then compare the result to reading
                 # via the context manager
                 reference_read_fields = { {% for field in node.children() -%}
                                           {%- if isinstance(field, systemrdlFieldNode) -%}
                                           {%- if field.is_sw_readable %}
                                           '{{ field.inst_name }}' : {%if asyncoutput %}await {% endif %}self.dut.{{'.'.join(get_python_path_segments(field))}}.read(){%- if not loop.last -%}, {%- endif %}  # type: ignore[union-attr]
@@ -702,25 +595,24 @@
                     {%- endif -%}
                     {%- endfor %}
 
                 read_callback_mock.assert_called_once()
                 write_callback_mock.assert_not_called()
 
         {%- endif %}
-        {%- endif %}
         {%- endfor %}
 
     {% if asyncoutput %}async {% endif %}def test_register_write_context_manager(self) -> None:
         """
         Test the read modify write context manager
         """
         rut:Reg{% if asyncoutput %}Async{% endif %}ReadWrite
         {% if asyncoutput %}async {% endif %}def write_field_cominbinations(reg: Reg{% if asyncoutput %}Async{% endif %}ReadWrite, writable_fields:List[str]) -> None:
-            with patch(__name__ + '.' + 'write_addr_space') as write_callback_mock, \
-                patch(__name__ + '.' + 'read_addr_space', return_value=0) as read_callback_mock:
+            with patch(base_name + '.write_addr_space') as write_callback_mock, \
+                patch(base_name + '.read_addr_space', return_value=0) as read_callback_mock:
                 for num_parm in range(1, len(writable_fields) + 1):
                     for fields_to_write in combinations(writable_fields, num_parm):
                         field_values = {}
                         expected_value = 0
                         for field_str in fields_to_write:
                             field = getattr(reg, field_str)
                             if hasattr(field, 'enum_cls'):
@@ -777,38 +669,36 @@
                                     field = getattr(reg_session, field_name)
                                     {% if asyncoutput %}await {% endif %}field.write(field_value)
                                 read_callback_mock.return_value = expected_value ^ reg_session.max_value
 
                         write_callback_mock.reset_mock()
                         read_callback_mock.reset_mock()
 
-        {%- for node in top_node.descendants(unroll=True) -%}
-        {%- if isinstance(node, systemrdlRegNode) %}
+        {% for node in owned_elements.registers -%}
         {% if node.has_sw_writable and node.has_sw_readable %}
         with self.subTest(msg='register: {{'.'.join(node.get_path_segments())}}'):
             rut = self.dut.{{'.'.join(get_python_path_segments(node))}} # type: ignore[union-attr,assignment]
             if not isinstance(rut, Reg{% if asyncoutput %}Async{% endif %}ReadWrite):
                 raise TypeError('Failed to find read/write register')
             {% if asyncoutput %}await {% endif %}write_field_cominbinations(reg=rut,
                                writable_fields = [ {% for field in get_reg_writable_fields(node) -%}
                                                    '{{ safe_node_name(field) }}' {%- if not loop.last -%},{%- endif %}
                                                    {% endfor -%} ])
         {%- endif %}
-        {%- endif %}
         {%- endfor %}
 
     {% if asyncoutput %}async {% endif %}def test_register_write_fields(self) -> None:
         """
         Walk the register map and check every register write_fields method
         """
         rut:Reg{% if asyncoutput %}Async{% endif %}ReadWrite
         rand_enum_value:IntEnum
         {% if asyncoutput %}async {% endif %}def write_field_cominbinations(reg: Reg{% if asyncoutput %}Async{% endif %}ReadWrite, writable_fields:List[str]) -> None:
-            with patch(__name__ + '.' + 'write_addr_space') as write_callback_mock, \
-                patch(__name__ + '.' + 'read_addr_space', return_value=0) as read_callback_mock:
+            with patch(base_name + '.write_addr_space') as write_callback_mock, \
+                patch(base_name + '.read_addr_space', return_value=0) as read_callback_mock:
                 for num_parm in range(1, len(writable_fields) + 1):
                     for fields_to_write in combinations(writable_fields, num_parm):
                         kwargs = {}
                         expected_value = 0
                         for field_str in fields_to_write:
                             field = getattr(reg, field_str)
                             if hasattr(field, 'enum_cls'):
@@ -833,16 +723,15 @@
                                 accesswidth=reg.accesswidth,
                                 data=expected_value)
                         read_callback_mock.assert_called_once()
                         write_callback_mock.reset_mock()
                         read_callback_mock.reset_mock()
 
 
-        {%- for node in top_node.descendants(unroll=True) -%}
-        {%- if isinstance(node, systemrdlRegNode) %}
+        {% for node in owned_elements.registers -%}
         {% if node.has_sw_writable %}
         with self.subTest(msg='register: {{'.'.join(node.get_path_segments())}}'):
             # test read_fields to register:
             # {{'.'.join(node.get_path_segments())}}
 
 
             {% if node.has_sw_readable %}
@@ -863,46 +752,44 @@
             kwargs['{{field.inst_name}}'] = rand_enum_value
             {%- else %}
             rand_field_value = random.randrange(0, {{ get_field_max_value_hex_string(field) }} + 1)
             kwargs['{{field.inst_name}}'] = rand_field_value
             {%- endif  %}
             expected_value = ( expected_value & {{get_field_inv_bitmask_hex_string(field)}} ) | (rand_field_value << {{ field.low }})
             {% endfor %}
-            with patch(__name__ + '.' + 'write_addr_space') as write_callback_mock, \
-                patch(__name__ + '.' + 'read_addr_space', return_value=0) as read_callback_mock:
+            with patch(base_name + '.write_addr_space') as write_callback_mock, \
+                patch(base_name + '.read_addr_space', return_value=0) as read_callback_mock:
                 {% if asyncoutput %}await {% endif %}self.dut.{{'.'.join(get_python_path_segments(node))}}.write_fields(**kwargs)  # type: ignore[union-attr]
                 write_callback_mock.assert_called_once_with(
                                     addr={{node.absolute_address}},
                                     width={{node.size * 8}},
                                     accesswidth=self.dut.{{'.'.join(get_python_path_segments(node))}}.accesswidth, # type: ignore[union-attr]
                                     data=expected_value)
                 read_callback_mock.assert_not_called()
                 write_callback_mock.reset_mock()
                 read_callback_mock.reset_mock()
 
             {% endif %}
 
 
         {%- endif %}
-        {%- endif %}
         {%- endfor %}
 
     {% if uses_memory %}
     {% if asyncoutput %}async {% endif %}def test_memory_read_and_write(self) -> None:
         """
         Walk the register map and check every register can be read and written to correctly
         """
-        {%- for node in top_node.descendants(unroll=True) -%}
-            {%- if isinstance(node, systemrdlMemNode) %}
+        {% for node in owned_elements.memories -%}
 
         # test access operations (read and/or write) to register:
         # {{'.'.join(node.get_path_segments())}}
         with self.subTest(msg='memory: {{'.'.join(node.get_path_segments())}}'):
-            with patch(__name__ + '.' + 'write_addr_space') as write_callback_mock, \
-                patch(__name__ + '.' + 'read_addr_space', return_value=1) as read_callback_mock:
+            with patch(base_name + '.write_addr_space') as write_callback_mock, \
+                patch(base_name + '.read_addr_space', return_value=1) as read_callback_mock:
 
                 {% if node.is_sw_readable -%}
                 # checks single unit accesses at the first entry, the last entry and a random entry in
                 # in each case check a 0, max value and random value being read
                 for entry in [0, random.randint(0,{{node.get_property('mementries')-1}}), {{node.get_property('mementries')-1}}]:
                     for value in [0, random.randint(0,{{get_memory_max_entry_value_hex_string(node)}}), {{get_memory_max_entry_value_hex_string(node)}}]:
                         read_callback_mock.reset_mock()
@@ -968,37 +855,32 @@
                                           data=random_data[x]))
 
                 read_callback_mock.assert_not_called()
                 write_callback_mock.reset_mock()
 
                 {%- endif %}
 
-        {%- endif %}
         {%- endfor %}
     {%- endif %}
 
     def test_adding_attributes(self) -> None:
         """
         Walk the address map and attempt to set a new value on each node
 
         The attribute name: cppkbrgmgeloagvfgjjeiiushygirh was randomly generated to be unlikely to
         every be a attribute name
 
         """
-        {%- for node in top_node.descendants(unroll=True) %}
-        {% if isinstance(node, systemrdlSignalNode) %}
-        # doing nothing with signal node: {{node.inst_name}}
-        {% else %}
+        {% for node in owned_elements.nodes -%}
         with self.subTest(msg='node: {{'.'.join(node.get_path_segments())}}'):
             with self.assertRaises(AttributeError):
                 # this line is trying to set an illegal value so by definition should fail the type
                 # checks
                 self.dut.{{'.'.join(get_python_path_segments(node))}}.cppkbrgmgeloagvfgjjeiiushygirh = 1 # type: ignore[attr-defined,union-attr]
-        {% endif %}
-        {%- endfor %}
+        {% endfor %}
 
     {% macro check_readable_register_iterators(node) %}
         {# check the unrolled case first #}
         expected_readable_regs = [ {%- for child_node in node.children(unroll=True) %}
                                     {%- if isinstance(child_node, systemrdlRegNode) %}{% if child_node.has_sw_readable %}self.dut.{{'.'.join(get_python_path_segments(child_node))}}, # type: ignore[union-attr,list-item] {% endif %}{% endif %}
                                     {% endfor %} ]
         readable_regs = []
@@ -1088,16 +970,16 @@
         expected_readable_fields: List[Union[FieldReadOnly, FieldReadWrite]]
         expected_writable_regs: List[WritableRegister]
         expected_readable_regs: List[ReadableRegister]
         expected_memories:List[Union[MemoryReadOnly, MemoryWriteOnly, MemoryReadWrite]]
         {% endif %}
         expected_sections : List[Union[AddressMap, RegFile]]
 
-        {%- for node in top_node.descendants(unroll=True) %}
-            {%- if isinstance(node, systemrdlRegNode) %}
+        # test all the registers
+        {% for node in owned_elements.registers -%}
         with self.subTest(msg='register: {{'.'.join(node.get_path_segments())}}'):
                 {# a register can only have fields beneath it #}
                 {% if node.has_sw_writable %}
             expected_writable_fields = [ {%- for child_node in node.children(unroll=True) -%}
                                          {% if child_node.is_sw_writable %}self.dut.{{'.'.join(get_python_path_segments(child_node))}}, # type: ignore[union-attr,list-item] {% endif %}
                                          {% endfor %}
                                          ]
@@ -1118,78 +1000,78 @@
             for readable_field in self.dut.{{'.'.join(get_python_path_segments(node))}}.readable_fields: # type: ignore[union-attr]
                 readable_fields.append(readable_field)
             self.assertCountEqual(expected_readable_fields, readable_fields)
                     {% else %}
             # register should not have readable_fields attribute
             self.assertFalse(hasattr(self.dut.{{'.'.join(get_python_path_segments(node))}}, 'readable_fields')) # type: ignore[union-attr]
                     {% endif %}
-            {%- elif isinstance(node, systemrdlMemNode) %}
+        {% endfor %}
+        # test all the memories
+        {% for node in owned_elements.memories -%}
+
         with self.subTest(msg='memory: {{'.'.join(node.get_path_segments())}}'):
                     {% if node.is_sw_writable %}
                         {{ check_writable_register_iterators(node) | indent }}
                     {% else %}
             self.assertFalse(hasattr(self.dut.{{'.'.join(get_python_path_segments(node))}}, 'get_writeable_registers')) # type: ignore[union-attr]
                     {% endif %}
                     {% if node.is_sw_readable %}
                         {{ check_readable_register_iterators(node) | indent}}
                     {% else %}
             self.assertFalse(hasattr(self.dut.{{'.'.join(get_python_path_segments(node))}}, 'get_readable_registers')) # type: ignore[union-attr]
                     {% endif %}
-            {%- elif isinstance(node, systemrdlAddrmapNode) %}
+        {% endfor %}
+        # test all the address maps
+        {% for node in owned_elements.addr_maps -%}
         with self.subTest(msg='addrmap: {{'.'.join(node.get_path_segments())}}'):
             {{ check_readable_register_iterators(node) | indent }}
             {{ check_writable_register_iterators(node) | indent}}
             {{ check_section_iterators(node) | indent }}
             {{ check_memory_iterators(node) | indent}}
-            {%- elif isinstance(node, systemrdlRegfileNode) %}
+        {% endfor %}
+        # test all the register files
+        {% for node in owned_elements.reg_files -%}
         with self.subTest(msg='regfile: {{'.'.join(node.get_path_segments())}}'):
             {{ check_readable_register_iterators(node) | indent }}
             {{ check_writable_register_iterators(node)  | indent}}
             {{ check_section_iterators(node) | indent }}
             self.assertFalse(hasattr(self.dut.{{'.'.join(get_python_path_segments(node))}}, 'get_memories')) # type: ignore[union-attr]
-            {% endif %}
-        {%- endfor %}
+        {% endfor %}
 
     def test_name_map(self) -> None:
         """
         Check that the function for getting a node by its original systemRDL name works
         """
-        {% for node in top_node.descendants(unroll=True) -%}
-        {% if not isinstance(node, (systemrdlFieldNode, systemrdlSignalNode)) %}
+        {% for node in owned_elements.nodes -%}
         {% for child_node in node.children(unroll=False) %}
         {% if not isinstance(child_node, systemrdlSignalNode) %}
         self.assertEqual(self.dut.{{'.'.join(get_python_path_segments(node))}}.get_child_by_system_rdl_name('{{child_node.inst_name}}').inst_name, '{{child_node.inst_name}}')  # type: ignore[union-attr]
         {% endif %}
         {% endfor %}
-        {% endif %}
         {% endfor %}
 
-class {{top_node.type_name}}_TestCase_BlockAccess(TestCaseBase): # type: ignore[valid-type,misc]
-
-    def setUp(self) -> None:
-        self.dut = {{top_node.type_name}}_cls({% if asyncoutput %}AsyncCallbackSet{% else %}NormalCallbackSet{% endif %}(read_callback=read_callback,
-                                                          write_callback=write_callback,
-                                                          read_block_callback=read_block_callback,
-                                                          write_block_callback=write_block_callback))
+class {{fq_block_name}}_block_access({{top_node.type_name}}_TestCase_BlockAccess): # type: ignore[valid-type,misc]
+    """
+    tests for all the block access methods
+    """
 
     {% if uses_memory %}
     {% if asyncoutput %}async {% endif %}def test_memory_read_and_write(self) -> None:
         """
         Walk the register map and check every register can be read and written to correctly
         """
-        {%- for node in top_node.descendants(unroll=True) -%}
-            {%- if isinstance(node, systemrdlMemNode) %}
+        {% for node in owned_elements.memories -%}
 
         # test access operations (read and/or write) to register:
         # {{'.'.join(node.get_path_segments())}}
-        with patch(__name__ + '.' + 'write_addr_space') as write_callback_mock,\
-                            patch(__name__ + '.' + 'read_addr_space', return_value=1) as read_callback_mock, \
-                            patch(__name__ + '.' + 'read_block_addr_space',
+        with patch(base_name + '.write_addr_space') as write_callback_mock,\
+                            patch(base_name + '.read_addr_space', return_value=1) as read_callback_mock, \
+                            patch(base_name + '.read_block_addr_space',
                                   return_value=Array('{{get_array_typecode(node.get_property('memwidth'))}}', [0])) as read_block_callback_mock , \
-                            patch(__name__ + '.' + 'write_block_addr_space') as write_block_callback_mock:
+                            patch(base_name + '.write_block_addr_space') as write_block_callback_mock:
 
             {% if node.is_sw_readable -%}
             # checks single unit accesses at the first entry, the last entry and a random entry in
             # in each case check a 0, max value and random value being read
             for entry in [0, random.randint(0,{{node.get_property('mementries')-1}}), {{node.get_property('mementries')-1}}]:
                 for value in [0, random.randint(0,{{get_memory_max_entry_value_hex_string(node)}}), {{get_memory_max_entry_value_hex_string(node)}}]:
                     read_block_callback_mock.reset_mock()
@@ -1256,15 +1138,14 @@
             read_callback_mock.assert_not_called()
             write_callback_mock.assert_not_called()
             read_block_callback_mock.assert_not_called()
             write_block_callback_mock.reset_mock()
 
             {%- endif %}
 
-        {%- endif %}
         {%- endfor %}
     {%- endif %}
 
 
 if __name__ == '__main__':
 {% if asyncoutput %}
     if sys.version_info < (3, 8):
```

### Comparing `peakrdl-python-0.5.0/src/peakrdl_python/templates/reg_definitions.py.jinja` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/reg_definitions.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.5.0/src/peakrdl_python.egg-info/PKG-INFO` & `peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakrdl-python
-Version: 0.5.0
+Version: 0.6.0rc1
 Summary: Generate python wrapper for a register model compiled SystemRDL input
 Home-page: https://github.com/krcb197/PeakRDL-python
 Author: Keith Brady
 License: UNKNOWN
 Project-URL: Source, https://github.com/krcb197/PeakRDL-python
 Project-URL: Tracker, https://github.com/krcb197/PeakRDL-python/issues
 Project-URL: Documentation, https://peakrdl-python.readthedocs.io/
```

### Comparing `peakrdl-python-0.5.0/src/peakrdl_python.egg-info/SOURCES.txt` & `peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 src/peakrdl_python/__about__.py
 src/peakrdl_python/__init__.py
 src/peakrdl_python/__peakrdl__.py
+src/peakrdl_python/_node_walkers.py
 src/peakrdl_python/exporter.py
 src/peakrdl_python/peakpython.py
 src/peakrdl_python/safe_name_utility.py
 src/peakrdl_python/systemrdl_node_utility_functions.py
 src/peakrdl_python.egg-info/PKG-INFO
 src/peakrdl_python.egg-info/SOURCES.txt
 src/peakrdl_python.egg-info/dependency_links.txt
@@ -25,10 +26,11 @@
 src/peakrdl_python/templates/addrmap.py.jinja
 src/peakrdl_python/templates/addrmap_field.py.jinja
 src/peakrdl_python/templates/addrmap_memory.py.jinja
 src/peakrdl_python/templates/addrmap_register.py.jinja
 src/peakrdl_python/templates/addrmap_simulation.py.jinja
 src/peakrdl_python/templates/addrmap_simulation_tb.jinja
 src/peakrdl_python/templates/addrmap_tb.py.jinja
+src/peakrdl_python/templates/baseclass_tb.py.jinja
 src/peakrdl_python/templates/header.py.jinja
 src/peakrdl_python/templates/header_tb.py.jinja
 src/peakrdl_python/templates/reg_definitions.py.jinja
```

