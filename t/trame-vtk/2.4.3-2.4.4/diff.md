# Comparing `tmp/trame-vtk-2.4.3.tar.gz` & `tmp/trame-vtk-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-vtk-2.4.3.tar", last modified: Fri Apr  7 19:04:12 2023, max compression
+gzip compressed data, was "trame-vtk-2.4.4.tar", last modified: Sun Apr 16 17:37:00 2023, max compression
```

## Comparing `trame-vtk-2.4.3.tar` & `trame-vtk-2.4.4.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.016879 trame-vtk-2.4.3/
--rw-r--r--   0 root         (0) root         (0)     1504 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       63 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    13038 2023-04-07 19:04:12.016879 trame-vtk-2.4.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12303 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/README.rst
--rw-r--r--   0 root         (0) root         (0)      878 2023-04-07 19:04:12.016879 trame-vtk-2.4.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.004878 trame-vtk-2.4.3/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.004878 trame-vtk-2.4.3/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       39 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame/modules/paraview.py
--rw-r--r--   0 root         (0) root         (0)       39 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame/modules/vtk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.004878 trame-vtk-2.4.3/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      182 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame/widgets/paraview.py
--rw-r--r--   0 root         (0) root         (0)      172 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame/widgets/vtk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.004878 trame-vtk-2.4.3/trame_vtk/
--rw-r--r--   0 root         (0) root         (0)     1504 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/LICENSE
--rw-r--r--   0 root         (0) root         (0)       91 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.004878 trame-vtk-2.4.3/trame_vtk/modules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.004878 trame-vtk-2.4.3/trame_vtk/modules/common/
--rw-r--r--   0 root         (0) root         (0)      354 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.004878 trame-vtk-2.4.3/trame_vtk/modules/common/serve/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/common/serve/.gitignore
--rw-r--r--   0 root         (0) root         (0)  1626752 2023-04-07 19:04:08.000000 trame-vtk-2.4.3/trame_vtk/modules/common/serve/trame-vtk.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.008879 trame-vtk-2.4.3/trame_vtk/modules/paraview/
--rw-r--r--   0 root         (0) root         (0)     7623 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/paraview/__init__.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/paraview/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.008879 trame-vtk-2.4.3/trame_vtk/modules/paraview/protocols/
--rw-r--r--   0 root         (0) root         (0)      363 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/paraview/protocols/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5356 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/paraview/protocols/local_rendering.py
--rw-r--r--   0 root         (0) root         (0)     2233 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/paraview/protocols/mouse_handler.py
--rw-r--r--   0 root         (0) root         (0)    23952 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/paraview/protocols/publish_image_delivery.py
--rw-r--r--   0 root         (0) root         (0)     3565 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/paraview/protocols/view_port.py
--rw-r--r--   0 root         (0) root         (0)     4170 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/paraview/protocols/web_protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.008879 trame-vtk-2.4.3/trame_vtk/modules/vtk/
--rw-r--r--   0 root         (0) root         (0)     7518 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2624 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.012879 trame-vtk-2.4.3/trame_vtk/modules/vtk/protocols/
--rw-r--r--   0 root         (0) root         (0)      322 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/protocols/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5574 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/protocols/local_rendering.py
--rw-r--r--   0 root         (0) root         (0)     3981 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/protocols/mouse_handler.py
--rw-r--r--   0 root         (0) root         (0)    12797 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/protocols/publish_image_delivery.py
--rw-r--r--   0 root         (0) root         (0)     1973 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/protocols/view_port.py
--rw-r--r--   0 root         (0) root         (0)     1787 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/protocols/web_protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.012879 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/
--rw-r--r--   0 root         (0) root         (0)      726 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11702 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/actors.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/data.py
--rw-r--r--   0 root         (0) root         (0)      796 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/export.py
--rw-r--r--   0 root         (0) root         (0)     5785 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/helpers.py
--rw-r--r--   0 root         (0) root         (0)     4666 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/initialize.py
--rw-r--r--   0 root         (0) root         (0)     1354 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/lights.py
--rw-r--r--   0 root         (0) root         (0)     5724 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/lookup_tables.py
--rw-r--r--   0 root         (0) root         (0)     5093 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/mappers.py
--rw-r--r--   0 root         (0) root         (0)     6041 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/mesh.py
--rw-r--r--   0 root         (0) root         (0)     3272 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/properties.py
--rw-r--r--   0 root         (0) root         (0)      378 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/registry.py
--rw-r--r--   0 root         (0) root         (0)     4978 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/render_windows.py
--rw-r--r--   0 root         (0) root         (0)      914 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/serialize.py
--rw-r--r--   0 root         (0) root         (0)     3541 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/synchronization_context.py
--rw-r--r--   0 root         (0) root         (0)     1337 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/textures.py
--rw-r--r--   0 root         (0) root         (0)     1946 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/utils.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/widgets.py
--rw-r--r--   0 root         (0) root         (0)     4551 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.012879 trame-vtk-2.4.3/trame_vtk/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.012879 trame-vtk-2.4.3/trame_vtk/widgets/vtk/
--rw-r--r--   0 root         (0) root         (0)      645 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/widgets/vtk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32816 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/widgets/vtk/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.004878 trame-vtk-2.4.3/trame_vtk.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13038 2023-04-07 19:04:11.000000 trame-vtk-2.4.3/trame_vtk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2295 2023-04-07 19:04:11.000000 trame-vtk-2.4.3/trame_vtk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 19:04:11.000000 trame-vtk-2.4.3/trame_vtk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-07 19:04:11.000000 trame-vtk-2.4.3/trame_vtk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-07 19:04:11.000000 trame-vtk-2.4.3/trame_vtk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 17:37:00.206477 trame-vtk-2.4.4/
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    13038 2023-04-16 17:37:00.206477 trame-vtk-2.4.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12303 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/README.rst
+-rw-r--r--   0 root         (0) root         (0)      878 2023-04-16 17:37:00.206477 trame-vtk-2.4.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 17:37:00.194477 trame-vtk-2.4.4/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 17:37:00.194477 trame-vtk-2.4.4/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       39 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame/modules/paraview.py
+-rw-r--r--   0 root         (0) root         (0)       39 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame/modules/vtk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 17:37:00.194477 trame-vtk-2.4.4/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame/widgets/paraview.py
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame/widgets/vtk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 17:37:00.198477 trame-vtk-2.4.4/trame_vtk/
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       91 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 17:37:00.198477 trame-vtk-2.4.4/trame_vtk/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 17:37:00.198477 trame-vtk-2.4.4/trame_vtk/modules/common/
+-rw-r--r--   0 root         (0) root         (0)      354 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 17:37:00.198477 trame-vtk-2.4.4/trame_vtk/modules/common/serve/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/common/serve/.gitignore
+-rw-r--r--   0 root         (0) root         (0)  1626752 2023-04-16 17:36:57.000000 trame-vtk-2.4.4/trame_vtk/modules/common/serve/trame-vtk.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 17:37:00.198477 trame-vtk-2.4.4/trame_vtk/modules/paraview/
+-rw-r--r--   0 root         (0) root         (0)     7755 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/paraview/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/paraview/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 17:37:00.202477 trame-vtk-2.4.4/trame_vtk/modules/paraview/protocols/
+-rw-r--r--   0 root         (0) root         (0)      363 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/paraview/protocols/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5356 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/paraview/protocols/local_rendering.py
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/paraview/protocols/mouse_handler.py
+-rw-r--r--   0 root         (0) root         (0)    23952 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/paraview/protocols/publish_image_delivery.py
+-rw-r--r--   0 root         (0) root         (0)     3565 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/paraview/protocols/view_port.py
+-rw-r--r--   0 root         (0) root         (0)     4170 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/paraview/protocols/web_protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 17:37:00.202477 trame-vtk-2.4.4/trame_vtk/modules/vtk/
+-rw-r--r--   0 root         (0) root         (0)     7518 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2624 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 17:37:00.202477 trame-vtk-2.4.4/trame_vtk/modules/vtk/protocols/
+-rw-r--r--   0 root         (0) root         (0)      322 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/protocols/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5574 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/protocols/local_rendering.py
+-rw-r--r--   0 root         (0) root         (0)     3981 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/protocols/mouse_handler.py
+-rw-r--r--   0 root         (0) root         (0)    12797 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/protocols/publish_image_delivery.py
+-rw-r--r--   0 root         (0) root         (0)     1973 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/protocols/view_port.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/protocols/web_protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 17:37:00.206477 trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/
+-rw-r--r--   0 root         (0) root         (0)      726 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11702 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/actors.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/data.py
+-rw-r--r--   0 root         (0) root         (0)      926 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/export.py
+-rw-r--r--   0 root         (0) root         (0)     5785 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     4666 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1354 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/lights.py
+-rw-r--r--   0 root         (0) root         (0)     5724 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/lookup_tables.py
+-rw-r--r--   0 root         (0) root         (0)     5093 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/mappers.py
+-rw-r--r--   0 root         (0) root         (0)     6041 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/mesh.py
+-rw-r--r--   0 root         (0) root         (0)     3272 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/properties.py
+-rw-r--r--   0 root         (0) root         (0)      378 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/registry.py
+-rw-r--r--   0 root         (0) root         (0)     4978 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/render_windows.py
+-rw-r--r--   0 root         (0) root         (0)      914 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     3541 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/synchronization_context.py
+-rw-r--r--   0 root         (0) root         (0)     1337 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/textures.py
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/widgets.py
+-rw-r--r--   0 root         (0) root         (0)     4551 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/modules/vtk/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 17:37:00.206477 trame-vtk-2.4.4/trame_vtk/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 17:37:00.206477 trame-vtk-2.4.4/trame_vtk/widgets/vtk/
+-rw-r--r--   0 root         (0) root         (0)      645 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/widgets/vtk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32816 2023-04-16 17:36:55.000000 trame-vtk-2.4.4/trame_vtk/widgets/vtk/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 17:37:00.198477 trame-vtk-2.4.4/trame_vtk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13038 2023-04-16 17:37:00.000000 trame-vtk-2.4.4/trame_vtk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2295 2023-04-16 17:37:00.000000 trame-vtk-2.4.4/trame_vtk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 17:37:00.000000 trame-vtk-2.4.4/trame_vtk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-16 17:37:00.000000 trame-vtk-2.4.4/trame_vtk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-16 17:37:00.000000 trame-vtk-2.4.4/trame_vtk.egg-info/top_level.txt
```

### Comparing `trame-vtk-2.4.3/LICENSE` & `trame-vtk-2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/PKG-INFO` & `trame-vtk-2.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-vtk
-Version: 2.4.3
+Version: 2.4.4
 Summary: VTK widgets for trame
 Author: Kitware Inc.
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `trame-vtk-2.4.3/README.rst` & `trame-vtk-2.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/setup.cfg` & `trame-vtk-2.4.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-vtk
-version = 2.4.3
+version = 2.4.4
 description = VTK widgets for trame
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = BSD License
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-vtk-2.4.3/trame_vtk/LICENSE` & `trame-vtk-2.4.4/trame_vtk/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/common/serve/trame-vtk.js` & `trame-vtk-2.4.4/trame_vtk/modules/common/serve/trame-vtk.js`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/paraview/__init__.py` & `trame-vtk-2.4.4/trame_vtk/modules/paraview/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         tmp = view_proxy.SuppressRendering
         view_proxy.SuppressRendering = 1
         try:
             view_proxy.StillRender()
         finally:
             view_proxy.SuppressRendering = tmp
 
-        return self._app.protocol_call(
+        return self._trame_server.protocol_call(
             "viewport.geometry.view.get.state",
             self.id(view_proxy),
             new_state,
             widgets=widgets,
             orientation_axis=orientation_axis,
         )
 
@@ -212,16 +212,24 @@
     return HELPER.object(vtk_id)
 
 
 def mesh(dataset, field_to_keep=None, point_arrays=None, cell_arrays=None):
     return HELPER.mesh(dataset, field_to_keep, point_arrays, cell_arrays)
 
 
-def scene(render_window, reset_camera=False, new_state=True):
-    scene_state = HELPER.scene(render_window, new_state)
+def scene(
+    render_window,
+    reset_camera=False,
+    new_state=True,
+    widgets=None,
+    orientation_axis=0,
+):
+    scene_state = HELPER.scene(
+        render_window, new_state, widgets=widgets, orientation_axis=orientation_axis
+    )
     if reset_camera:
         scene_state.setdefault("extra", {})["resetCamera"] = 1
     return scene_state
 
 
 def export(render_window, widgets=None, orientation_axis=0):
     return HELPER.export(
```

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/paraview/core.py` & `trame-vtk-2.4.4/trame_vtk/modules/paraview/core.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/paraview/protocols/local_rendering.py` & `trame-vtk-2.4.4/trame_vtk/modules/paraview/protocols/local_rendering.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/paraview/protocols/mouse_handler.py` & `trame-vtk-2.4.4/trame_vtk/modules/paraview/protocols/mouse_handler.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/paraview/protocols/publish_image_delivery.py` & `trame-vtk-2.4.4/trame_vtk/modules/paraview/protocols/publish_image_delivery.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/paraview/protocols/view_port.py` & `trame-vtk-2.4.4/trame_vtk/modules/paraview/protocols/view_port.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/paraview/protocols/web_protocol.py` & `trame-vtk-2.4.4/trame_vtk/modules/paraview/protocols/web_protocol.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/vtk/__init__.py` & `trame-vtk-2.4.4/trame_vtk/modules/vtk/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/vtk/core.py` & `trame-vtk-2.4.4/trame_vtk/modules/vtk/core.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/vtk/protocols/local_rendering.py` & `trame-vtk-2.4.4/trame_vtk/modules/vtk/protocols/local_rendering.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/vtk/protocols/mouse_handler.py` & `trame-vtk-2.4.4/trame_vtk/modules/vtk/protocols/mouse_handler.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/vtk/protocols/publish_image_delivery.py` & `trame-vtk-2.4.4/trame_vtk/modules/vtk/protocols/publish_image_delivery.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/vtk/protocols/view_port.py` & `trame-vtk-2.4.4/trame_vtk/modules/vtk/protocols/view_port.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/vtk/protocols/web_protocol.py` & `trame-vtk-2.4.4/trame_vtk/modules/vtk/protocols/web_protocol.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/__init__.py` & `trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/actors.py` & `trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/actors.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/data.py` & `trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/data.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/export.py` & `trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/export.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 def handle_property(hash_list, prop_value):
+    if isinstance(prop_value, list):
+        for item in prop_value:
+            handle_property(hash_list, item)
+        return
+
     if not isinstance(prop_value, dict):
         return
 
     if "vtkClass" in prop_value and "hash" in prop_value:
         hash_list.append(
             dict(
                 hash=prop_value.get("hash"),
```

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/helpers.py` & `trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/helpers.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/initialize.py` & `trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/initialize.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/lights.py` & `trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/lights.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/lookup_tables.py` & `trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/lookup_tables.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/mappers.py` & `trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/mappers.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/mesh.py` & `trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/mesh.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/properties.py` & `trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/properties.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/render_windows.py` & `trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/render_windows.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/serialize.py` & `trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/serialize.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/synchronization_context.py` & `trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/synchronization_context.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/textures.py` & `trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/textures.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/utils.py` & `trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/utils.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/widgets.py` & `trame-vtk-2.4.4/trame_vtk/modules/vtk/serializers/widgets.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/modules/vtk/widget.py` & `trame-vtk-2.4.4/trame_vtk/modules/vtk/widget.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/widgets/vtk/__init__.py` & `trame-vtk-2.4.4/trame_vtk/widgets/vtk/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk/widgets/vtk/common.py` & `trame-vtk-2.4.4/trame_vtk/widgets/vtk/common.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.3/trame_vtk.egg-info/PKG-INFO` & `trame-vtk-2.4.4/trame_vtk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-vtk
-Version: 2.4.3
+Version: 2.4.4
 Summary: VTK widgets for trame
 Author: Kitware Inc.
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `trame-vtk-2.4.3/trame_vtk.egg-info/SOURCES.txt` & `trame-vtk-2.4.4/trame_vtk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

