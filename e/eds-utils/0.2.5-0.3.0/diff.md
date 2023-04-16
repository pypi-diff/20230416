# Comparing `tmp/eds-utils-0.2.5.tar.gz` & `tmp/eds-utils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eds-utils-0.2.5.tar", last modified: Tue Apr 11 03:17:38 2023, max compression
+gzip compressed data, was "eds-utils-0.3.0.tar", last modified: Sun Apr 16 16:33:08 2023, max compression
```

## Comparing `eds-utils-0.2.5.tar` & `eds-utils-0.3.0.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:17:38.703668 eds-utils-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 03:17:28.000000 eds-utils-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-11 03:17:38.703668 eds-utils-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-11 03:17:28.000000 eds-utils-0.2.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:17:38.691668 eds-utils-0.2.5/eds_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:17:38.695668 eds-utils-0.2.5/eds_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12689 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/core/eds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:17:38.695668 eds-utils-0.2.5/eds_utils/core/file_io/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/core/file_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22994 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/core/file_io/read_eds.py
--rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/core/file_io/write_canopennode.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/core/file_io/write_eds.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/core/file_io/write_md.py
--rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/core/file_io/write_rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/core/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds2dcf.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds2md.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds2rst.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_autofix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:17:38.699668 eds-utils-0.2.5/eds_utils/eds_editor/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:17:38.699668 eds-utils-0.2.5/eds_utils/eds_editor/dialogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/dialogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/dialogs/add_mapped_object_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/dialogs/add_object_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/dialogs/copy_object_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/dialogs/errors_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/dialogs/open_tmp_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/eds_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:17:38.703668 eds-utils-0.2.5/eds_utils/eds_editor/pages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/pages/_object_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/pages/device_commissioning_page.py
--rw-r--r--   0 runner    (1001) docker     (123)    13499 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/pages/general_info_page.py
--rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/pages/object_dictionary_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/pages/page.py
--rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/pages/pdo_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/window.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:17:38.695668 eds-utils-0.2.5/eds_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-11 03:17:38.000000 eds-utils-0.2.5/eds_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-11 03:17:38.000000 eds-utils-0.2.5/eds_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 03:17:38.000000 eds-utils-0.2.5/eds_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-11 03:17:38.000000 eds-utils-0.2.5/eds_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 03:17:38.000000 eds-utils-0.2.5/eds_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 03:17:38.000000 eds-utils-0.2.5/eds_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-11 03:17:28.000000 eds-utils-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-11 03:17:38.703668 eds-utils-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:17:38.703668 eds-utils-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:17:28.000000 eds-utils-0.2.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-11 03:17:28.000000 eds-utils-0.2.5/tests/test_eds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-11 03:17:28.000000 eds-utils-0.2.5/tests/test_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:33:08.263846 eds-utils-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 16:32:56.000000 eds-utils-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-16 16:33:08.263846 eds-utils-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-16 16:32:56.000000 eds-utils-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:33:08.259847 eds-utils-0.3.0/eds_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:33:08.259847 eds-utils-0.3.0/eds_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12779 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/core/eds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:33:08.259847 eds-utils-0.3.0/eds_utils/core/file_io/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/core/file_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23363 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/core/file_io/read_eds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/core/file_io/write_canopennode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/core/file_io/write_eds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/core/file_io/write_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9072 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/core/file_io/write_rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/core/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds2dcf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds2md.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds2rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_autofix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:33:08.259847 eds-utils-0.3.0/eds_utils/eds_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:33:08.259847 eds-utils-0.3.0/eds_utils/eds_editor/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/dialogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/dialogs/add_mapped_object_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/dialogs/add_object_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/dialogs/copy_object_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/dialogs/errors_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/dialogs/open_tmp_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/eds_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:33:08.263846 eds-utils-0.3.0/eds_utils/eds_editor/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12753 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/pages/_object_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/pages/device_commissioning_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13499 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/pages/general_info_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/pages/object_dictionary_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/pages/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/pages/pdo_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:33:08.259847 eds-utils-0.3.0/eds_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-16 16:33:08.000000 eds-utils-0.3.0/eds_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-16 16:33:08.000000 eds-utils-0.3.0/eds_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 16:33:08.000000 eds-utils-0.3.0/eds_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-16 16:33:08.000000 eds-utils-0.3.0/eds_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-16 16:33:08.000000 eds-utils-0.3.0/eds_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-16 16:33:08.000000 eds-utils-0.3.0/eds_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-16 16:32:56.000000 eds-utils-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-16 16:33:08.263846 eds-utils-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:33:08.263846 eds-utils-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:32:56.000000 eds-utils-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-16 16:32:56.000000 eds-utils-0.3.0/tests/test_eds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-16 16:32:56.000000 eds-utils-0.3.0/tests/test_objects.py
```

### Comparing `eds-utils-0.2.5/LICENSE` & `eds-utils-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.5/PKG-INFO` & `eds-utils-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eds-utils
-Version: 0.2.5
+Version: 0.3.0
 Summary: Utilities for editing CANopen EDS/DCF files
 Home-page: https://github.com/oresat/eds-utils
 Author: psas
 Author-email: oresat@pdx.edu
 Maintainer: psas
 Maintainer-email: oresat@pdx.edu
 License: GPL-3.0
@@ -35,14 +35,15 @@
 - **eds-editor:** GTK4-based GUI to edit EDS / DCF files.
 - **eds-validate:** CLI to validate EDS / DCF files. Will print all errors to stderr.
 - **eds2c:** CLI to convert a EDS / DCF file to CANopenNode OD.[c/h] files.
 - **eds2dcf:** CLI to convert a EDS to a DCF.
 - **eds2md:** CLI to convert a EDS / DCF file to a md (Markdown) file.
 - **eds2rst:** CLI to convert a EDS / DCF file to a rst (reStructuredText) file.
 - **eds-autofix:** CLI to autofix errors in EDS / DCF files.
+- **eds-merge:** CLI to merge two EDS / DCF files.
 
 
 How To Install
 ==============
 
 Linux
 -----
```

### Comparing `eds-utils-0.2.5/README.rst` & `eds-utils-0.3.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 - **eds-editor:** GTK4-based GUI to edit EDS / DCF files.
 - **eds-validate:** CLI to validate EDS / DCF files. Will print all errors to stderr.
 - **eds2c:** CLI to convert a EDS / DCF file to CANopenNode OD.[c/h] files.
 - **eds2dcf:** CLI to convert a EDS to a DCF.
 - **eds2md:** CLI to convert a EDS / DCF file to a md (Markdown) file.
 - **eds2rst:** CLI to convert a EDS / DCF file to a rst (reStructuredText) file.
 - **eds-autofix:** CLI to autofix errors in EDS / DCF files.
+- **eds-merge:** CLI to merge two EDS / DCF files.
 
 
 How To Install
 ==============
 
 Linux
 -----
```

### Comparing `eds-utils-0.2.5/eds_utils/__main__.py` & `eds-utils-0.3.0/eds_utils/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 from .eds_validate import eds_validate, EDS_VALIDATE_DESCRIPTION
 from .eds_editor.main import eds_editor, EDS_EDITOR_DESCRIPTION
 from .eds2dcf import eds2dcf, EDS2DCF_DESCRIPTION
 from .eds2md import eds2md, EDS2MD_DESCRIPTION
 from .eds2rst import eds2rst, EDS2RST_DESCRIPTION
 from .eds2c import eds2c, EDS2C_DESCRIPTION
 from .eds_autofix import eds_autofix, EDS_AUTOFIX_DESCRIPTION
+from .eds_merge import eds_merge, EDS_MERGE_DESCRIPTION
 
 
 PROGRAMS = {
     'eds-validate': EDS_VALIDATE_DESCRIPTION,
     'eds-editor  ': EDS_EDITOR_DESCRIPTION,
     'eds2dcf     ': EDS2DCF_DESCRIPTION,
     'eds2md      ': EDS2MD_DESCRIPTION,
     'eds2rst     ': EDS2RST_DESCRIPTION,
     'eds2c       ': EDS2C_DESCRIPTION,
     'eds-autofix ': EDS_AUTOFIX_DESCRIPTION,
+    'eds-merge   ': EDS_MERGE_DESCRIPTION,
 }
 
 
 def eds_utils():
     print('eds-utils v' + __version__)
     print('')
 
@@ -44,9 +46,11 @@
         eds2md(sys.argv[2:])
     elif sys.argv[1] == 'eds2rst':
         eds2rst(sys.argv[2:])
     elif sys.argv[1] == 'eds2c':
         eds2c(sys.argv[2:])
     elif sys.argv[1] == 'eds-autofix':
         eds_autofix(sys.argv[2:])
+    elif sys.argv[1] == 'eds-merge':
+        eds_merge(sys.argv[2:])
     else:
         eds_utils()
```

### Comparing `eds-utils-0.2.5/eds_utils/core/__init__.py` & `eds-utils-0.3.0/eds_utils/core/__init__.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.5/eds_utils/core/eds.py` & `eds-utils-0.3.0/eds_utils/core/eds.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 @dataclass
 class FileInfo:
 
     file_name: str = 'new_file.eds'
     file_version: int = 0
     file_revision: int = 0
+    last_eds: int = ''  # DCF only
     eds_version: str = '4.0'
     description: str = ''
     creation_dt: datetime = datetime.now()
     created_by: str = ''
     modification_dt: datetime = datetime.now()
     modified_by: str = ''
 
@@ -160,14 +161,16 @@
             raise EDSError(f'index 0x{index:X} already exist')
 
         if item.storage_location == '' and self._storage_locations:
             item.storage_location = self._storage_locations[0]
 
         self._data[index] = item
 
+        self._data = dict(sorted(self._data.items()))
+
     def __delitem__(self, index: int):
         del self._data[index]
 
     def insert(self, index: int, subindex: int, item):
         '''Insert a object into the object dictionary'''
 
         if subindex is None:
```

### Comparing `eds-utils-0.2.5/eds_utils/core/file_io/read_eds.py` & `eds-utils-0.3.0/eds_utils/core/file_io/read_eds.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,15 +284,16 @@
         access_type = lines['AccessType']
         var.access_type = AccessType.from_str(access_type)
     except KeyError:
         errors.append(f'{_LEVEL}: AccessType was missing from {header}')
     except ValueError:
         errors.append(f'{_LEVEL}: AccessType value of {access_type} is invalid in {header}')
 
-    list_data_types = [DataType.VISIBLE_STRING, DataType.OCTET_STRING, DataType.UNICODE_STRING]
+    list_data_types = [DataType.VISIBLE_STRING, DataType.OCTET_STRING, DataType.UNICODE_STRING,
+                       DataType.DOMAIN]
 
     if 'DefaultValue' in lines:  # optional
         if var.data_type == DataType.OCTET_STRING:
             value = lines['DefaultValue']
             value_ns = value.replace(' ', '')
 
             # format OCTET_STRING's default value
@@ -453,14 +454,20 @@
         errors.append(f'{_LEVEL}: {exc}')
 
     try:
         file_info.file_revision = _read_int_value(header, lines, 'FileRevision')
     except ValueError as exc:
         errors.append(f'{_LEVEL}: {exc}')
 
+    if file_info.file_name.endswith('.dcf'):  # only in DCFs
+        try:
+            file_info.last_eds = lines['LastEDS']
+        except KeyError:
+            errors.append(f'{_LEVEL}: LastEDS was missing from {header}')
+
     try:
         file_info.eds_version = lines['EDSVersion']
     except KeyError:
         # optional, if missing it's v3.0
         file_info.eds_version = '3.0'
 
     try:
@@ -621,15 +628,18 @@
 
     try:
         device_comm.node_name = lines['NodeName']
     except KeyError:
         errors.append(f'{_LEVEL}: NodeName was missing from {header}')
 
     try:
-        temp = _read_int_value(header, lines, 'Baudrate')
+        try:
+            temp = _read_int_value(header, lines, 'Baudrate')
+        except Exception:
+            temp = _read_int_value(header, lines, 'BaudRate')
         if temp in BAUD_RATE:
             device_comm.baud_rate = temp
         else:
             errors.append(f'{_LEVEL}: Baudrate in {header} was not a valid CANopen baud rate')
     except ValueError as exc:
         errors.append(f'{_LEVEL}: {exc}')
```

### Comparing `eds-utils-0.2.5/eds_utils/core/file_io/write_canopennode.py` & `eds-utils-0.3.0/eds_utils/core/file_io/write_canopennode.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.5/eds_utils/core/file_io/write_eds.py` & `eds-utils-0.3.0/eds_utils/core/file_io/write_eds.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,21 +24,24 @@
 
     if not file_path:  # use value from file info
         file_path = eds.file_info.file_name
 
     if not dcf and file_path.endswith('.dcf'):
         dcf = True
     elif dcf and file_path.endswith('.eds'):  # force eds to dcf
+        eds.file_info.last_eds = basename(file_path)
         file_path = splitext(file_path)[0] + '.dcf'
 
     # file info seciton
     lines.append('[FileInfo]')
     lines.append(f'FileName={basename(file_path)}')
     lines.append(f'FileVersion={eds.file_info.file_version}')
     lines.append(f'FileRevision={eds.file_info.file_revision}')
+    if dcf:
+        lines.append(f'LastEDS={eds.file_info.last_eds}')
     lines.append(f'EDSVersion={eds.file_info.eds_version}')
     lines.append(f'Description={eds.file_info.description}')
     lines.append('CreationTime=' + eds.file_info.creation_dt.strftime('%I:%M%p'))
     lines.append('CreationDate=' + eds.file_info.creation_dt.strftime('%m-%d-%Y'))
     lines.append(f'CreatedBy={eds.file_info.created_by}')
     lines.append('ModificationTime=' + eds.file_info.modification_dt.strftime('%I:%M%p'))
     lines.append('ModificationDate=' + eds.file_info.modification_dt.strftime('%m-%d-%Y'))
@@ -65,19 +68,19 @@
     lines.append(f'LSS_Supported={int(eds.device_info.lss_supported)}')
     lines.append('')
 
     if dcf:
         lines.append('[DeviceComissioning]')  # only one 'm' in header
         lines.append(f'NodeID=0x{eds.device_commissioning.node_id:X}')
         lines.append(f'NodeName={eds.device_commissioning.node_name}')
-        lines.append(f'Baudrate={eds.device_commissioning.baud_rate}')
+        lines.append(f'BaudRate={eds.device_commissioning.baud_rate}')
         lines.append(f'NetNumber={eds.device_commissioning.net_number}')
         lines.append(f'NetworkName={eds.device_commissioning.network_name}')
         lines.append(f'CANopenManager={int(eds.device_commissioning.canopen_manager)}')
-        lines.append(f'LSS_SerialNumber={eds.device_commissioning.lss_serialnumber}')
+        lines.append(f'LSS_SerialNumber={int(eds.device_commissioning.lss_serialnumber)}')
         lines.append('')
 
     # TODO dummy usage
     lines.append('[DummyUsage]')
     for i in range(8):
         lines.append(f'Dummy000{i}=1')
     lines.append('')
```

### Comparing `eds-utils-0.2.5/eds_utils/core/file_io/write_md.py` & `eds-utils-0.3.0/eds_utils/core/file_io/write_md.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     lines.append('## File Info')
     lines.append('')
     lines.append('Item|Value')
     lines.append('---|---')
     lines.append(f'File Name|{basename(eds.file_info.file_name)}')
     lines.append(f'File Version|{eds.file_info.file_version}')
     lines.append(f'File Revision|{eds.file_info.file_revision}')
+    if dcf:
+        lines.append(f'Last EDS|{eds.file_info.last_eds}')
     lines.append(f'EDS Version|{eds.file_info.eds_version}')
     lines.append(f'Description|{eds.file_info.description}')
     lines.append('Creation Time|' + eds.file_info.creation_dt.strftime('%I:%M%p'))
     lines.append('Creation Date|' + eds.file_info.creation_dt.strftime('%m-%d-%Y'))
     lines.append(f'Created By|{eds.file_info.created_by}')
     lines.append('Modification Time|' + eds.file_info.modification_dt.strftime('%I:%M%p'))
     lines.append('Modification Date|' + eds.file_info.modification_dt.strftime('%m-%d-%Y'))
```

### Comparing `eds-utils-0.2.5/eds_utils/core/file_io/write_rst.py` & `eds-utils-0.3.0/eds_utils/core/file_io/write_rst.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     lines.append('#########')
     lines.append('')
     lines.append('.. csv-table::')
     lines.append('')
     lines.append(f'{INDENT3}"File Name", "{basename(eds.file_info.file_name)}"')
     lines.append(f'{INDENT3}"File Version", "{eds.file_info.file_version}"')
     lines.append(f'{INDENT3}"File Revision", "{eds.file_info.file_revision}"')
+    if dcf:
+        lines.append(f'{INDENT3}"Last EDS", "{eds.file_info.last_eds}"')
     lines.append(f'{INDENT3}"EDS Version", "{eds.file_info.eds_version}"')
     lines.append(f'{INDENT3}"Description", "{eds.file_info.description}"')
     time_str = eds.file_info.creation_dt.strftime('%I:%M%p')
     lines.append(f'{INDENT3}"Creation Time", "{time_str}"')
     date_str = eds.file_info.creation_dt.strftime('%m-%d-%Y')
     lines.append(f'{INDENT3}"Creation Date", "{date_str}"')
     lines.append(f'{INDENT3}"Created By", "{eds.file_info.created_by}"')
```

### Comparing `eds-utils-0.2.5/eds_utils/core/objects.py` & `eds-utils-0.3.0/eds_utils/core/objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     comments: str = ''
     parameter_name: str = 'New Variable'
     denotation: str = ''
     data_type: DataType = DataType.UNSIGNED32
     low_limit: str = ''
     high_limit: str = ''
-    default_value: str = '0'
+    default_value: str = ''
     access_type: AccessType = AccessType.RW
     pdo_mapping: bool = False
     object_type: ObjectType = ObjectType.VAR
     storage_location: str = ''  # for CANopenNode support
 
     def __hash__(self):
         return hash((self.parameter_name, self.data_type, self.comments))
@@ -85,16 +85,19 @@
             self._data[subindex].access_type = variable.access_type
         elif subindex in self._data:  # add subindex
             raise ValueError('Subindex already exists')
         else:
             variable.storage_location = self.storage_location
             self._data[subindex] = variable
 
-            # update record size subindex
-            self._data[0].default_value = f'0x{len(self._data) - 1:02X}'
+            # make sure the subindexes are ordered
+            self._data = dict(sorted(self._data.items()))
+
+            # update record highest subindex
+            self._data[0].default_value = f'0x{list(self._data)[-1]:02X}'
 
     def __delitem__(self, subindex: int):
         '''Remove a subindex from the record'''
 
         if subindex == 0:
             raise ValueError('Cannot remove subindex 0')
         if subindex not in self._data:
@@ -105,15 +108,15 @@
         # update record size subindex
         self._data[0].default_value = f'0x{len(self._data) - 1:02X}'
 
     @property
     def subindexes(self) -> list:
         '''Get the list of subindexes'''
 
-        return sorted(self._data.keys())
+        return self._data.keys()
 
     @property
     def storage_location(self) -> str:
         '''The storage location of object'''
 
         return self._storage_location
 
@@ -167,16 +170,19 @@
             variable.storage_location = self.storage_location
             self._data[subindex] = variable
 
             # set the data_type if not set
             if not self._data_type:
                 self._data_type = variable.data_type
 
-            # update record size subindex
-            self._data[0].default_value = f'0x{len(self._data) - 1:02X}'
+            # make sure the subindexes are ordered
+            self._data = dict(sorted(self._data.items()))
+
+            # update record highest subindex
+            self._data[0].default_value = f'0x{list(self._data)[-1]:02X}'
 
     @property
     def data_type(self) -> DataType:
         '''DataType: Get the data type for all items in array'''
         return self._data_type
 
     @data_type.setter
```

### Comparing `eds-utils-0.2.5/eds_utils/eds2c.py` & `eds-utils-0.3.0/eds_utils/eds2c.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.5/eds_utils/eds2dcf.py` & `eds-utils-0.3.0/eds_utils/eds2dcf.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,8 +41,10 @@
     eds.device_commissioning.network_name = args.network_name
     eds.device_commissioning.canopen_manager = args.canopen_manager
     eds.device_commissioning.lss_serialnumber = args.lss_serial_number
 
     if args.output:
         write_eds(eds, file_path=args.output, dcf=True)
     else:
-        write_eds(eds, file_path=os.path.dirname(os.path.abspath(args.filepath)), dcf=True)
+        path = os.path.dirname(os.path.abspath(args.filepath))
+        file_name = os.path.basename(args.filepath)
+        write_eds(eds, file_path=f'{path}/{file_name}', dcf=True)
```

### Comparing `eds-utils-0.2.5/eds_utils/eds2md.py` & `eds-utils-0.3.0/eds_utils/eds_autofix.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-import os
 import sys
 import argparse
 
 from .core.file_io.read_eds import read_eds
-from .core.file_io.write_md import write_md
+from .core.file_io.write_eds import write_eds
 
-EDS2MD_DESCRIPTION = 'Convert a EDS/DCF file to a md (Markdown) file'
+EDS_AUTOFIX_DESCRIPTION = 'Autofix errors in a EDS/DCF file'
 
 
-def eds2md(sys_args=None):
+def eds_autofix(sys_args=None):
     if sys_args is None:
         sys_args = sys.argv[1:]
 
-    parser = argparse.ArgumentParser(description=EDS2MD_DESCRIPTION, prog='eds2md')
-    parser.add_argument('filepath', metavar='FILEPATH', help='file path to EDS file')
-    parser.add_argument('-o', '--output', metavar='OUTPUT', help='output file path')
+    parser = argparse.ArgumentParser(description=EDS_AUTOFIX_DESCRIPTION, prog='eds-autofix')
+    parser.add_argument('filepath', metavar='FILEPATH', help='file path to EDS/DCF file')
+    parser.add_argument('-s', '--silence', action='store_true', help='silence prints to stdout')
     args = parser.parse_args(sys_args)
 
     try:
         eds, errors = read_eds(args.filepath)
+        write_eds(eds, args.filepath)
     except FileNotFoundError as exc:
         print(exc)
         sys.exit(1)
 
-    if args.output:
-        write_md(eds, file_path=args.output)
-    else:
-        write_md(eds, file_path=os.path.dirname(os.path.abspath(args.filepath)))
+    if not args.silence:
+        for i in errors:
+            print(i)
```

### Comparing `eds-utils-0.2.5/eds_utils/eds2rst.py` & `eds-utils-0.3.0/eds_utils/eds2rst.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,8 +22,10 @@
     except FileNotFoundError as exc:
         print(exc)
         sys.exit(1)
 
     if args.output:
         write_rst(eds, file_path=args.output)
     else:
-        write_rst(eds, file_path=os.path.dirname(os.path.abspath(args.filepath)))
+        path = os.path.dirname(os.path.abspath(args.filepath))
+        file_name = os.path.basename(args.filepath)[:-4] + '.rst'
+        write_rst(eds, file_path=f'{path}/{file_name}')
```

### Comparing `eds-utils-0.2.5/eds_utils/eds_autofix.py` & `eds-utils-0.3.0/eds_utils/eds_validate.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import sys
 import argparse
 
 from .core.file_io.read_eds import read_eds
-from .core.file_io.write_eds import write_eds
 
-EDS_AUTOFIX_DESCRIPTION = 'Autofix errors in a EDS/DCF file'
+EDS_VALIDATE_DESCRIPTION = 'Validate a EDS/DCF file'
 
 
-def eds_autofix(sys_args=None):
+def eds_validate(sys_args=None):
     if sys_args is None:
         sys_args = sys.argv[1:]
 
-    name = 'eds-autofix'
-    parser = argparse.ArgumentParser(description=EDS_AUTOFIX_DESCRIPTION, prog=name)
+    parser = argparse.ArgumentParser(description=EDS_VALIDATE_DESCRIPTION, prog='eds-validate')
     parser.add_argument('filepath', metavar='FILEPATH', help='file path to EDS/DCF file')
-    parser.add_argument('-s', '--silence', action='store_true', help='silence prints to stdout')
+    parser.add_argument('-s', '--silence', action='store_true', help='silence prints to stderr')
     args = parser.parse_args(sys_args)
 
     try:
-        eds, errors = read_eds(args.filepath)
-        write_eds(eds, args.filepath)
+        _, errors = read_eds(args.filepath)
     except FileNotFoundError as exc:
         print(exc)
         sys.exit(1)
 
     if not args.silence:
         for i in errors:
-            print(i)
+            print(i, file=sys.stderr)
+
+    if len(errors) > 0:
+        sys.exit(1)
```

### Comparing `eds-utils-0.2.5/eds_utils/eds_editor/app.py` & `eds-utils-0.3.0/eds_utils/eds_editor/app.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.5/eds_utils/eds_editor/dialogs/add_mapped_object_dialog.py` & `eds-utils-0.3.0/eds_utils/eds_editor/dialogs/add_mapped_object_dialog.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.5/eds_utils/eds_editor/dialogs/add_object_dialog.py` & `eds-utils-0.3.0/eds_utils/eds_editor/dialogs/add_object_dialog.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.5/eds_utils/eds_editor/dialogs/copy_object_dialog.py` & `eds-utils-0.3.0/eds_utils/eds_editor/dialogs/copy_object_dialog.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.5/eds_utils/eds_editor/dialogs/errors_dialog.py` & `eds-utils-0.3.0/eds_utils/eds_editor/dialogs/errors_dialog.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.5/eds_utils/eds_editor/dialogs/open_tmp_dialog.py` & `eds-utils-0.3.0/eds_utils/eds_editor/dialogs/open_tmp_dialog.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.5/eds_utils/eds_editor/eds_notebook.py` & `eds-utils-0.3.0/eds_utils/eds_editor/eds_notebook.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.5/eds_utils/eds_editor/main.py` & `eds-utils-0.3.0/eds_utils/eds_editor/main.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.5/eds_utils/eds_editor/pages/_object_grid.py` & `eds-utils-0.3.0/eds_utils/eds_editor/pages/_object_grid.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,17 @@
         self.attach(self._obj_parameter_name, column=1, row=0, width=3, height=1)
 
         label = Gtk.Label.new('Denotation (DCF only):')
         label.set_halign(Gtk.Align.START)
         self._obj_denotation = Gtk.Entry()
         self._obj_denotation.set_max_length(241)
         self._obj_denotation.connect('changed', self._on_obj_denotation_changed)
+        if self._eds.file_info.file_name.endswith('.eds'):
+            label.hide()
+            self._obj_denotation.hide()
         self.attach(label, column=0, row=1, width=1, height=1)
         self.attach(self._obj_denotation, column=1, row=1, width=3, height=1)
 
         label = Gtk.Label.new('Object Type:')
         label.set_halign(Gtk.Align.START)
         self._obj_type = Gtk.DropDown()
         self._obj_type.set_sensitive(False)
@@ -136,21 +139,21 @@
         self._selected_obj = self._eds[index] if subindex is None else self._eds[index][subindex]
 
         # reset these
         self._obj_data_type.set_sensitive(True)
         self._obj_storage_loc.set_sensitive(True)
         self._obj_default_value_len_label.hide()
 
-        if subindex is None:
-            self._obj_data_type.set_sensitive(False)
-        elif self._eds[index].object_type == ObjectType.ARRAY:
+        # data_type set sensitivity
+        if self._eds[index].object_type in [ObjectType.ARRAY, ObjectType.RECORD]:
+            if subindex == 0:
+                self._obj_data_type.set_sensitive(False)
             self._obj_storage_loc.set_sensitive(False)
+        if self._eds[index].object_type == ObjectType.ARRAY:
             self._obj_data_type.set_sensitive(False)
-        else:
-            self._obj_storage_loc.set_sensitive(False)
 
         if self._selected_obj.object_type == ObjectType.ARRAY:
             self._obj_data_type.show()
             self._obj_access_type.hide()
             self._obj_pdo_mapping.hide()
             self._obj_default_value.hide()
             self._obj_low_limit.hide()
```

### Comparing `eds-utils-0.2.5/eds_utils/eds_editor/pages/device_commissioning_page.py` & `eds-utils-0.3.0/eds_utils/eds_editor/pages/device_commissioning_page.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.5/eds_utils/eds_editor/pages/general_info_page.py` & `eds-utils-0.3.0/eds_utils/eds_editor/pages/general_info_page.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.5/eds_utils/eds_editor/pages/object_dictionary_page.py` & `eds-utils-0.3.0/eds_utils/eds_editor/pages/object_dictionary_page.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.5/eds_utils/eds_editor/pages/pdo_page.py` & `eds-utils-0.3.0/eds_utils/eds_editor/pages/pdo_page.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.5/eds_utils/eds_editor/window.py` & `eds-utils-0.3.0/eds_utils/eds_editor/window.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.5/eds_utils.egg-info/PKG-INFO` & `eds-utils-0.3.0/eds_utils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eds-utils
-Version: 0.2.5
+Version: 0.3.0
 Summary: Utilities for editing CANopen EDS/DCF files
 Home-page: https://github.com/oresat/eds-utils
 Author: psas
 Author-email: oresat@pdx.edu
 Maintainer: psas
 Maintainer-email: oresat@pdx.edu
 License: GPL-3.0
@@ -35,14 +35,15 @@
 - **eds-editor:** GTK4-based GUI to edit EDS / DCF files.
 - **eds-validate:** CLI to validate EDS / DCF files. Will print all errors to stderr.
 - **eds2c:** CLI to convert a EDS / DCF file to CANopenNode OD.[c/h] files.
 - **eds2dcf:** CLI to convert a EDS to a DCF.
 - **eds2md:** CLI to convert a EDS / DCF file to a md (Markdown) file.
 - **eds2rst:** CLI to convert a EDS / DCF file to a rst (reStructuredText) file.
 - **eds-autofix:** CLI to autofix errors in EDS / DCF files.
+- **eds-merge:** CLI to merge two EDS / DCF files.
 
 
 How To Install
 ==============
 
 Linux
 -----
```

### Comparing `eds-utils-0.2.5/eds_utils.egg-info/SOURCES.txt` & `eds-utils-0.3.0/eds_utils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 eds_utils/__init__.py
 eds_utils/__main__.py
 eds_utils/eds2c.py
 eds_utils/eds2dcf.py
 eds_utils/eds2md.py
 eds_utils/eds2rst.py
 eds_utils/eds_autofix.py
+eds_utils/eds_merge.py
 eds_utils/eds_validate.py
 eds_utils.egg-info/PKG-INFO
 eds_utils.egg-info/SOURCES.txt
 eds_utils.egg-info/dependency_links.txt
 eds_utils.egg-info/entry_points.txt
 eds_utils.egg-info/requires.txt
 eds_utils.egg-info/top_level.txt
```

### Comparing `eds-utils-0.2.5/setup.cfg` & `eds-utils-0.3.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -36,12 +36,13 @@
 	eds-editor = eds_utils.eds_editor.main:eds_editor
 	eds-validate = eds_utils.eds_validate:eds_validate
 	eds2c = eds_utils.eds2c:eds2c
 	eds2dcf = eds_utils.eds2dcf:eds2dcf
 	eds2md = eds_utils.eds2md:eds2md
 	eds2rst = eds_utils.eds2rstf:eds2rst
 	eds-autofix = eds_utils.eds_autofix:eds_autofix
+	eds-merge = eds_utils.eds_merge:eds_merge
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `eds-utils-0.2.5/tests/test_eds.py` & `eds-utils-0.3.0/tests/test_eds.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.5/tests/test_objects.py` & `eds-utils-0.3.0/tests/test_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         rec[2] = Variable()
         self.assertEqual(len(rec), 3)
         self.assertEqual(rec[0].default_value, '0x02')
 
         # empty space
         rec[4] = Variable()
         self.assertEqual(len(rec), 4)
-        self.assertEqual(rec[0].default_value, '0x03')
+        self.assertEqual(rec[0].default_value, '0x04')
 
     def test_remove(self):
 
         rec = Record()
 
         # add a var to an subindex
         rec[1] = Variable()
@@ -51,15 +51,15 @@
 
         # cannot remove an index that doesn't exist
         with self.assertRaises(ValueError):
             del rec[4]
 
         # remove a valid subindexes
         self.assertEqual(len(rec), 5)
-        self.assertEqual(rec[0].default_value, '0x04')
+        self.assertEqual(rec[0].default_value, '0x05')
         del rec[3]
         self.assertEqual(len(rec), 4)
         self.assertEqual(rec[0].default_value, '0x03')
         del rec[1]
         self.assertEqual(len(rec), 3)
         self.assertEqual(rec[0].default_value, '0x02')
         del rec[5]
@@ -90,15 +90,15 @@
             arr[1] = Variable(data_type=DataType.UNSIGNED16)
         self.assertEqual(len(arr), 2)
         self.assertEqual(arr[0].default_value, '0x01')
 
         # add a var to an subindex
         arr[10] = Variable(data_type=DataType.UNSIGNED8)
         self.assertEqual(len(arr), 3)
-        self.assertEqual(arr[0].default_value, '0x02')
+        self.assertEqual(arr[0].default_value, '0x0A')
 
         for i in arr.subindexes:
             self.assertEqual(arr[i].data_type, arr.data_type)
 
     def test_data_type(self):
 
         arr = Array(data_type=DataType.UNSIGNED32)
```

