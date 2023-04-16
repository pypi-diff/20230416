# Comparing `tmp/sphere_base-0.0.1.tar.gz` & `tmp/sphere_base-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphere_base-0.0.1.tar", last modified: Thu Mar 16 15:00:45 2023, max compression
+gzip compressed data, was "sphere_base-0.1.0.tar", last modified: Sun Apr 16 14:57:09 2023, max compression
```

## Comparing `sphere_base-0.0.1.tar` & `sphere_base-0.1.0.tar`

### file list

```diff
@@ -1,92 +1,155 @@
-drwxrwxrwx   0        0        0        0 2023-03-16 15:00:45.625550 sphere_base-0.0.1/
--rw-rw-rw-   0        0        0      101 2023-03-15 12:30:50.000000 sphere_base-0.0.1/HISTORY.rst
--rw-rw-rw-   0        0        0     1540 2023-03-15 11:59:22.000000 sphere_base-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      252 2023-03-15 14:22:33.000000 sphere_base-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2307 2023-03-16 15:00:45.624550 sphere_base-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1502 2023-03-16 14:07:49.000000 sphere_base-0.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-16 15:00:45.121521 sphere_base-0.0.1/docs/
--rw-rw-rw-   0        0        0      638 2023-03-15 17:55:12.000000 sphere_base-0.0.1/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-03-16 15:00:45.038516 sphere_base-0.0.1/docs/build/
-drwxrwxrwx   0        0        0        0 2023-03-16 15:00:45.039516 sphere_base-0.0.1/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-03-16 15:00:45.135522 sphere_base-0.0.1/docs/build/html/_static/
--rw-rw-rw-   0        0        0      286 2023-03-15 17:53:40.000000 sphere_base-0.0.1/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.0.1/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.0.1/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      804 2023-03-15 17:55:12.000000 sphere_base-0.0.1/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-03-16 15:00:45.160523 sphere_base-0.0.1/docs/source/
--rw-rw-rw-   0        0        0     1003 2023-03-15 18:08:16.000000 sphere_base-0.0.1/docs/source/conf.py
--rw-rw-rw-   0        0        0      469 2023-03-15 17:55:12.000000 sphere_base-0.0.1/docs/source/index.rst
--rw-rw-rw-   0        0        0      127 2023-03-15 17:49:53.000000 sphere_base-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-16 15:00:45.626550 sphere_base-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1473 2023-03-15 17:15:22.000000 sphere_base-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-16 15:00:45.166524 sphere_base-0.0.1/sphere_base/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.0.1/sphere_base/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 15:00:45.248528 sphere_base-0.0.1/sphere_base/model/
--rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.0.1/sphere_base/model/__init__.py
--rw-rw-rw-   0        0        0     3517 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/model/mesh.py
--rw-rw-rw-   0        0        0     5703 2023-03-16 10:58:58.000000 sphere_base-0.0.1/sphere_base/model/model.py
--rw-rw-rw-   0        0        0     8678 2023-03-16 10:58:58.000000 sphere_base-0.0.1/sphere_base/model/models.py
--rw-rw-rw-   0        0        0    17693 2023-03-16 10:58:59.000000 sphere_base-0.0.1/sphere_base/model/obj_file_loader.py
-drwxrwxrwx   0        0        0        0 2023-03-16 15:00:45.329533 sphere_base-0.0.1/sphere_base/shader/
--rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.0.1/sphere_base/shader/__init__.py
--rw-rw-rw-   0        0        0    10075 2023-03-16 10:58:59.000000 sphere_base-0.0.1/sphere_base/shader/uv_base_shader.py
--rw-rw-rw-   0        0        0     1851 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/shader/uv_circle_shader.py
--rw-rw-rw-   0        0        0     1841 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/shader/uv_cross_shader.py
--rw-rw-rw-   0        0        0      527 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/shader/uv_default_shader.py
--rw-rw-rw-   0        0        0      777 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/shader/uv_flat_shader.py
--rw-rw-rw-   0        0        0     1325 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/shader/uv_holo_sphere_shader.py
--rw-rw-rw-   0        0        0     1030 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/shader/uv_node_shader.py
--rw-rw-rw-   0        0        0     2154 2023-03-16 10:58:34.000000 sphere_base-0.0.1/sphere_base/shader/uv_skybox_shader.py
--rw-rw-rw-   0        0        0     1119 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/shader/uv_socket_shader.py
--rw-rw-rw-   0        0        0     1368 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/shader/uv_sphere_edge_shader.py
--rw-rw-rw-   0        0        0     1551 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/shader/uv_sphere_shader.py
--rw-rw-rw-   0        0        0     1219 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/shader/uv_sphere_small_shader.py
--rw-rw-rw-   0        0        0     1703 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/shader/uv_square_shader.py
-drwxrwxrwx   0        0        0        0 2023-03-16 15:00:45.417538 sphere_base-0.0.1/sphere_base/sphere_overlay/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.0.1/sphere_base/sphere_overlay/__init__.py
--rw-rw-rw-   0        0        0     1871 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/sphere_overlay/sov_conf.py
--rw-rw-rw-   0        0        0      543 2021-04-13 07:49:18.000000 sphere_base-0.0.1/sphere_base/sphere_overlay/sov_edge.py
--rw-rw-rw-   0        0        0     2206 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/sphere_overlay/sov_sphere.py
--rw-rw-rw-   0        0        0     1589 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/sphere_overlay/sov_sphere_node_base.py
--rw-rw-rw-   0        0        0      871 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/sphere_overlay/sov_uv_widget.py
-drwxrwxrwx   0        0        0        0 2023-03-16 15:00:45.459540 sphere_base-0.0.1/sphere_base/sphere_overlay/sphere_nodes/
--rw-rw-rw-   0        0        0      248 2021-03-02 15:18:12.000000 sphere_base-0.0.1/sphere_base/sphere_overlay/sphere_nodes/__init__.py
--rw-rw-rw-   0        0        0      566 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/sphere_overlay/sphere_nodes/edge_sphere_item.py
--rw-rw-rw-   0        0        0     1006 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py
--rw-rw-rw-   0        0        0      922 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py
-drwxrwxrwx   0        0        0        0 2023-03-16 15:00:45.617550 sphere_base-0.0.1/sphere_base/sphere_universe_base/
--rw-rw-rw-   0        0        0       23 2021-03-11 14:37:00.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/__init__.py
--rw-rw-rw-   0        0        0     5795 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_calc.py
--rw-rw-rw-   0        0        0     7282 2023-03-16 10:58:58.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_cam.py
--rw-rw-rw-   0        0        0     4886 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_cam_movement.py
--rw-rw-rw-   0        0        0     5399 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_clipboard.py
--rw-rw-rw-   0        0        0     4036 2023-03-16 13:20:23.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_config.py
--rw-rw-rw-   0        0        0     7594 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_constants.py
--rw-rw-rw-   0        0        0     6521 2023-03-16 10:58:58.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_edge_drag.py
--rw-rw-rw-   0        0        0     7218 2023-03-16 10:58:58.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_graphic_disc.py
--rw-rw-rw-   0        0        0     4859 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_graphic_edge.py
--rw-rw-rw-   0        0        0      367 2021-03-16 19:38:36.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_graphic_item.py
--rw-rw-rw-   0        0        0     2726 2023-03-16 10:58:59.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_graphic_node.py
--rw-rw-rw-   0        0        0     2499 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_graphic_socket.py
--rw-rw-rw-   0        0        0     8853 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_history.py
--rw-rw-rw-   0        0        0    17083 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_mouse_ray.py
--rw-rw-rw-   0        0        0    11756 2023-03-16 10:58:58.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_node.py
--rw-rw-rw-   0        0        0     7343 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_rubber_band.py
--rw-rw-rw-   0        0        0     1657 2021-03-16 20:04:16.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_serializable.py
--rw-rw-rw-   0        0        0     6113 2023-03-16 12:32:57.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_skybox.py
--rw-rw-rw-   0        0        0     8677 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_socket.py
--rw-rw-rw-   0        0        0    35649 2023-03-16 10:58:58.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_sphere.py
--rw-rw-rw-   0        0        0     1892 2023-03-13 10:54:30.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_sphere_edge.py
--rw-rw-rw-   0        0        0    10112 2023-03-15 10:44:30.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_surface_edge.py
--rw-rw-rw-   0        0        0    13949 2023-03-16 12:21:36.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_universe.py
--rw-rw-rw-   0        0        0     1494 2021-03-18 13:39:18.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_utils.py
--rw-rw-rw-   0        0        0    15926 2023-03-15 15:36:32.000000 sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_widget.py
-drwxrwxrwx   0        0        0        0 2023-03-16 15:00:45.210526 sphere_base-0.0.1/sphere_base.egg-info/
--rw-rw-rw-   0        0        0     2307 2023-03-16 15:00:44.000000 sphere_base-0.0.1/sphere_base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2965 2023-03-16 15:00:44.000000 sphere_base-0.0.1/sphere_base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-16 15:00:44.000000 sphere_base-0.0.1/sphere_base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-16 15:00:44.000000 sphere_base-0.0.1/sphere_base.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      119 2023-03-16 15:00:44.000000 sphere_base-0.0.1/sphere_base.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-16 15:00:44.000000 sphere_base-0.0.1/sphere_base.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-16 15:00:45.623550 sphere_base-0.0.1/tests/
--rw-rw-rw-   0        0        0      530 2023-03-15 14:00:41.000000 sphere_base-0.0.1/tests/test_000_import.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.201292 sphere_base-0.1.0/
+-rw-rw-rw-   0        0        0      978 2023-04-16 07:19:30.000000 sphere_base-0.1.0/HISTORY.rst
+-rw-rw-rw-   0        0        0     1105 2023-04-16 08:54:46.000000 sphere_base-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      252 2023-03-15 14:22:33.000000 sphere_base-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      737 2023-04-16 14:57:09.201292 sphere_base-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1090 2023-04-16 14:27:52.000000 sphere_base-0.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-16 14:57:08.989280 sphere_base-0.1.0/docs/
+-rw-rw-rw-   0        0        0      638 2023-03-15 17:55:12.000000 sphere_base-0.1.0/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-04-16 14:57:08.964278 sphere_base-0.1.0/docs/build/
+drwxrwxrwx   0        0        0        0 2023-04-16 14:57:08.965278 sphere_base-0.1.0/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-04-16 14:57:08.994280 sphere_base-0.1.0/docs/build/html/_static/
+-rw-rw-rw-   0        0        0      286 2023-03-15 17:53:40.000000 sphere_base-0.1.0/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.0/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.0/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      804 2023-03-15 17:55:12.000000 sphere_base-0.1.0/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-16 14:57:08.997280 sphere_base-0.1.0/docs/source/
+-rw-rw-rw-   0        0        0     1175 2023-03-16 20:29:33.000000 sphere_base-0.1.0/docs/source/conf.py
+-rw-rw-rw-   0        0        0      489 2023-03-16 21:15:47.000000 sphere_base-0.1.0/docs/source/index.rst
+drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.094286 sphere_base-0.1.0/docs/source/rst/
+-rw-rw-rw-   0        0        0      163 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.model.mesh.rst
+-rw-rw-rw-   0        0        0      166 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.model.model.rst
+-rw-rw-rw-   0        0        0      169 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.model.models.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.model.obj_file_loader.rst
+-rw-rw-rw-   0        0        0      369 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.model.rst
+-rw-rw-rw-   0        0        0      196 2023-03-16 21:18:48.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.rst
+-rw-rw-rw-   0        0        0      780 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_base_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_circle_shader.rst
+-rw-rw-rw-   0        0        0      203 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_cross_shader.rst
+-rw-rw-rw-   0        0        0      209 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_default_shader.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_flat_shader.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_holo_sphere_shader.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_node_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_skybox_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_socket_shader.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_sphere_edge_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_sphere_shader.rst
+-rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_sphere_small_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_square_shader.rst
+-rw-rw-rw-   0        0        0      602 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_overlay.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_overlay.sov_conf.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_overlay.sov_edge.rst
+-rw-rw-rw-   0        0        0      212 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_overlay.sov_sphere.rst
+-rw-rw-rw-   0        0        0      246 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_overlay.sov_sphere_node_base.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_overlay.sov_uv_widget.rst
+-rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.edge_sphere_item.rst
+-rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.item_sphere_node.rst
+-rw-rw-rw-   0        0        0      279 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.person_sphere_node.rst
+-rw-rw-rw-   0        0        0      502 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.rst
+-rw-rw-rw-   0        0        0     1563 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.rst
+-rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_calc.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_cam.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_cam_movement.rst
+-rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_clipboard.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_config.rst
+-rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_constants.rst
+-rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_edge_drag.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_disc.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_edge.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_item.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_node.rst
+-rw-rw-rw-   0        0        0      258 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_socket.rst
+-rw-rw-rw-   0        0        0      235 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_history.rst
+-rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_mouse_ray.rst
+-rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_node.rst
+-rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_rubber_band.rst
+-rw-rw-rw-   0        0        0      250 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_serializable.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_skybox.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_socket.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere.rst
+-rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere_edge.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_surface_edge.rst
+-rw-rw-rw-   0        0        0      238 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_universe.rst
+-rw-rw-rw-   0        0        0      229 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_utils.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_widget.rst
+-rw-rw-rw-   0        0        0      127 2023-03-15 17:49:53.000000 sphere_base-0.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 14:57:09.201292 sphere_base-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1507 2023-04-16 14:57:02.000000 sphere_base-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.107287 sphere_base-0.1.0/sphere_base/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.0/sphere_base/__init__.py
+-rw-rw-rw-   0        0        0     8514 2023-04-14 08:27:37.000000 sphere_base-0.1.0/sphere_base/calc.py
+-rw-rw-rw-   0        0        0     6909 2023-04-15 10:13:03.000000 sphere_base-0.1.0/sphere_base/clipboard.py
+-rw-rw-rw-   0        0        0     5078 2023-04-14 08:50:15.000000 sphere_base-0.1.0/sphere_base/config.py
+-rw-rw-rw-   0        0        0     5372 2023-04-15 11:21:35.000000 sphere_base-0.1.0/sphere_base/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.137288 sphere_base-0.1.0/sphere_base/edge/
+-rw-rw-rw-   0        0        0        0 2023-03-30 07:32:40.000000 sphere_base-0.1.0/sphere_base/edge/__init__.py
+-rw-rw-rw-   0        0        0     6609 2023-04-14 08:50:15.000000 sphere_base-0.1.0/sphere_base/edge/edge_drag.py
+-rw-rw-rw-   0        0        0     4771 2023-04-14 17:26:15.000000 sphere_base-0.1.0/sphere_base/edge/graphic_edge.py
+-rw-rw-rw-   0        0        0      365 2023-04-15 20:38:35.000000 sphere_base-0.1.0/sphere_base/edge/graphic_line.py
+-rw-rw-rw-   0        0        0     1859 2023-04-04 08:07:28.000000 sphere_base-0.1.0/sphere_base/edge/inter_sphere_edge.py
+-rw-rw-rw-   0        0        0    14064 2023-04-15 09:49:56.000000 sphere_base-0.1.0/sphere_base/edge/surface_edge.py
+-rw-rw-rw-   0        0        0     9835 2023-04-08 12:55:07.000000 sphere_base-0.1.0/sphere_base/history.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.143289 sphere_base-0.1.0/sphere_base/model/
+-rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.0/sphere_base/model/__init__.py
+-rw-rw-rw-   0        0        0     4398 2023-04-04 14:50:05.000000 sphere_base-0.1.0/sphere_base/model/mesh.py
+-rw-rw-rw-   0        0        0     6060 2023-04-11 18:27:52.000000 sphere_base-0.1.0/sphere_base/model/model.py
+-rw-rw-rw-   0        0        0     3318 2023-04-04 11:04:51.000000 sphere_base-0.1.0/sphere_base/model/models.py
+-rw-rw-rw-   0        0        0    23013 2023-04-07 13:30:04.000000 sphere_base-0.1.0/sphere_base/model/obj_file_loader.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.153289 sphere_base-0.1.0/sphere_base/node/
+-rw-rw-rw-   0        0        0        0 2023-03-30 07:35:09.000000 sphere_base-0.1.0/sphere_base/node/__init__.py
+-rw-rw-rw-   0        0        0     8018 2023-04-03 06:31:17.000000 sphere_base-0.1.0/sphere_base/node/graphic_disc.py
+-rw-rw-rw-   0        0        0     2676 2023-04-03 06:31:17.000000 sphere_base-0.1.0/sphere_base/node/graphic_node.py
+-rw-rw-rw-   0        0        0     2449 2023-04-03 06:31:16.000000 sphere_base-0.1.0/sphere_base/node/graphic_socket.py
+-rw-rw-rw-   0        0        0    13284 2023-04-14 09:24:59.000000 sphere_base-0.1.0/sphere_base/node/node.py
+-rw-rw-rw-   0        0        0     8797 2023-04-13 12:16:43.000000 sphere_base-0.1.0/sphere_base/node/socket.py
+-rw-rw-rw-   0        0        0     1737 2023-03-30 07:13:13.000000 sphere_base-0.1.0/sphere_base/serializable.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.173290 sphere_base-0.1.0/sphere_base/shader/
+-rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.0/sphere_base/shader/__init__.py
+-rw-rw-rw-   0        0        0    10547 2023-04-14 08:50:15.000000 sphere_base-0.1.0/sphere_base/shader/base_shader.py
+-rw-rw-rw-   0        0        0     1956 2023-03-30 12:23:24.000000 sphere_base-0.1.0/sphere_base/shader/circle_shader.py
+-rw-rw-rw-   0        0        0     1946 2023-03-30 12:23:24.000000 sphere_base-0.1.0/sphere_base/shader/cross_shader.py
+-rw-rw-rw-   0        0        0      572 2023-03-30 09:23:40.000000 sphere_base-0.1.0/sphere_base/shader/default_shader.py
+-rw-rw-rw-   0        0        0     1174 2023-04-15 09:19:58.000000 sphere_base-0.1.0/sphere_base/shader/edge_shader.py
+-rw-rw-rw-   0        0        0      886 2023-03-30 12:22:23.000000 sphere_base-0.1.0/sphere_base/shader/flat_shader.py
+-rw-rw-rw-   0        0        0     1447 2023-03-30 12:22:23.000000 sphere_base-0.1.0/sphere_base/shader/holo_sphere_shader.py
+-rw-rw-rw-   0        0        0     1160 2023-03-30 12:22:23.000000 sphere_base-0.1.0/sphere_base/shader/node_shader.py
+-rw-rw-rw-   0        0        0     2150 2023-03-30 12:20:38.000000 sphere_base-0.1.0/sphere_base/shader/skybox_shader.py
+-rw-rw-rw-   0        0        0     1238 2023-03-30 12:20:38.000000 sphere_base-0.1.0/sphere_base/shader/socket_shader.py
+-rw-rw-rw-   0        0        0     3109 2023-03-31 17:56:46.000000 sphere_base-0.1.0/sphere_base/shader/sphere_edge_shader.py
+-rw-rw-rw-   0        0        0     1631 2023-03-30 12:18:39.000000 sphere_base-0.1.0/sphere_base/shader/sphere_shader.py
+-rw-rw-rw-   0        0        0     1232 2023-03-30 12:18:13.000000 sphere_base-0.1.0/sphere_base/shader/sphere_small_shader.py
+-rw-rw-rw-   0        0        0     1808 2023-03-30 12:18:13.000000 sphere_base-0.1.0/sphere_base/shader/square_shader.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.176290 sphere_base-0.1.0/sphere_base/sphere/
+-rw-rw-rw-   0        0        0        0 2023-03-28 18:59:07.000000 sphere_base-0.1.0/sphere_base/sphere/__init__.py
+-rw-rw-rw-   0        0        0    28219 2023-04-16 07:14:28.000000 sphere_base-0.1.0/sphere_base/sphere/sphere.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.182291 sphere_base-0.1.0/sphere_base/sphere_overlay/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.0/sphere_base/sphere_overlay/__init__.py
+-rw-rw-rw-   0        0        0     1875 2023-03-28 18:59:36.000000 sphere_base-0.1.0/sphere_base/sphere_overlay/sov_conf.py
+-rw-rw-rw-   0        0        0     2468 2023-04-13 17:50:12.000000 sphere_base-0.1.0/sphere_base/sphere_overlay/sov_sphere.py
+-rw-rw-rw-   0        0        0     1598 2023-04-13 12:14:08.000000 sphere_base-0.1.0/sphere_base/sphere_overlay/sov_sphere_node_base.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.186291 sphere_base-0.1.0/sphere_base/sphere_overlay/sphere_nodes/
+-rw-rw-rw-   0        0        0      248 2021-03-02 15:18:12.000000 sphere_base-0.1.0/sphere_base/sphere_overlay/sphere_nodes/__init__.py
+-rw-rw-rw-   0        0        0      460 2023-04-04 13:53:39.000000 sphere_base-0.1.0/sphere_base/sphere_overlay/sphere_nodes/edge_sphere_item.py
+-rw-rw-rw-   0        0        0     1084 2023-04-13 12:16:43.000000 sphere_base-0.1.0/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py
+-rw-rw-rw-   0        0        0     1002 2023-04-13 12:14:08.000000 sphere_base-0.1.0/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.198292 sphere_base-0.1.0/sphere_base/sphere_universe_base/
+-rw-rw-rw-   0        0        0       23 2021-03-11 14:37:00.000000 sphere_base-0.1.0/sphere_base/sphere_universe_base/__init__.py
+-rw-rw-rw-   0        0        0     7829 2023-04-15 12:02:34.000000 sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_cam.py
+-rw-rw-rw-   0        0        0     3434 2023-04-15 11:53:42.000000 sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_cam_movement.py
+-rw-rw-rw-   0        0        0      365 2023-03-28 18:59:36.000000 sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_graphic_item.py
+-rw-rw-rw-   0        0        0    15874 2023-04-14 08:50:15.000000 sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_mouse_ray.py
+-rw-rw-rw-   0        0        0     7211 2023-04-14 09:13:08.000000 sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_rubber_band.py
+-rw-rw-rw-   0        0        0     5392 2023-03-28 18:59:36.000000 sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_skybox.py
+-rw-rw-rw-   0        0        0    14026 2023-04-14 08:50:15.000000 sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_universe.py
+-rw-rw-rw-   0        0        0    17879 2023-04-16 07:15:30.000000 sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_widget.py
+-rw-rw-rw-   0        0        0     1494 2023-03-30 07:18:00.000000 sphere_base-0.1.0/sphere_base/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.129288 sphere_base-0.1.0/sphere_base.egg-info/
+-rw-rw-rw-   0        0        0      737 2023-04-16 14:57:08.000000 sphere_base-0.1.0/sphere_base.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6024 2023-04-16 14:57:08.000000 sphere_base-0.1.0/sphere_base.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 14:57:08.000000 sphere_base-0.1.0/sphere_base.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-16 07:34:46.000000 sphere_base-0.1.0/sphere_base.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      119 2023-04-16 14:57:08.000000 sphere_base-0.1.0/sphere_base.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-16 14:57:08.000000 sphere_base-0.1.0/sphere_base.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.199292 sphere_base-0.1.0/tests/
+-rw-rw-rw-   0        0        0      530 2023-03-15 14:00:41.000000 sphere_base-0.1.0/tests/test_000_import.py
```

### Comparing `sphere_base-0.0.1/docs/Makefile` & `sphere_base-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphere_base-0.0.1/docs/make.bat` & `sphere_base-0.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sphere_base-0.0.1/setup.py` & `sphere_base-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,39 +9,40 @@
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 with open('requirements.txt') as requirements_file:
     requirements = requirements_file.read()
 
-setup_requirements = [ ]
+setup_requirements = []
 
-test_requirements = [ ]
+test_requirements = []
 
 setup(
     author="Richard Boltze",
     author_email='rboltze@protonmail.com',
     python_requires='>=3.6',
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
+        'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
-    description="Python Boilerplate contains all the boilerplate you need to create a Python package.",
+    description="The library was created to be used as a building block for applications were information"
+                "should appear on the surface of a sphere.",
     install_requires=requirements,
-    license="BSD license",
-    long_description=readme + '\n\n' + history,
+    license="MIT license",
+    long_description="",
     include_package_data=True,
     keywords='sphere_base',
     name='sphere_base',
     packages=find_packages(include=['sphere_base*'], exclude=['examples*', 'test*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
-    url='https://github.com/rboltze/sphere_base',
-    version='0.0.1',
+    url='https://github.com/rboltze/spherebase',
+    version='0.1.0',
     zip_safe=False,
 )
```

### Comparing `sphere_base-0.0.1/sphere_base/model/model.py` & `sphere_base-0.1.0/sphere_base/model/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,42 @@
 # -*- coding: utf-8 -*-
 
-"""
-- **model** - :class:`~sphere_iot.uv_models.Model`
-"""
+# Do not remove these!!!
+# -------------- these will be dynamically late loaded! -----------------------
+from sphere_base.shader.skybox_shader import SkyboxShader
+from sphere_base.shader.sphere_shader import SphereShader
+from sphere_base.shader.node_shader import NodeShader
+from sphere_base.shader.socket_shader import SocketShader
+from sphere_base.shader.flat_shader import FlatShader
+from sphere_base.shader.default_shader import DefaultShader
+from sphere_base.shader.circle_shader import CircleShader
+from sphere_base.shader.square_shader import SquareShader
+from sphere_base.shader.sphere_edge_shader import SphereEdgeShader
+from sphere_base.shader.cross_shader import CrossShader
+from sphere_base.shader.holo_sphere_shader import HoloSphereShader
+from sphere_base.shader.sphere_small_shader import SphereSmallShader
+from sphere_base.shader.edge_shader import EdgeShader
+# -----------------------------------------------------------------------
 
 from sphere_base.sphere_universe_base.suv_graphic_item import GraphicItem
 from sphere_base.model.mesh import Mesh
 from sphere_base.model.obj_file_loader import ObjectFileLoader
 import pathlib
 
 DEBUG = True
 
+
 class Model(GraphicItem):
     Mesh_class = Mesh
 
     """
     Class representing a ``Model``. 
     """
 
-    def __init__(self, models, model_id, model_name, obj_file=None, shader=None, vertex_shader=None,
+    def __init__(self, models, model_id=None, model_name=None, obj_file=None, shader=None, vertex_shader=None,
                  fragment_shader=None, geometry_shader=None):
         """
 
         Contructor of the ``Model`` class. Creates a new model from data received.
 
         :param models: Instance of :class:`~sphere_iot.uv_models.Models`
         :type models: :class:`~sphere_iot.uv_models.Models`
@@ -42,15 +56,15 @@
         :Instance Variables:
 
             - **config** - :class:`~sphere_iot.uv_config.UvConfig`
             - **uv** - :class:`~sphere_iot.uv_universe.Universe`
             - **models** - :class:`~sphere_iot.uv_models.Models`
             - **model_id** - ``int`` id of this ``Model``
             - **shader** - specific class inherited from :class:`~sphere_iot.shader.uv_base_shader.Shader`
-            - **model** - ``model`` loaded from ``Pyassimp``
+            - **model** - ``model`` loaded
 
         .. note::
 
             Each ``Model`` has its own shader.
 
             The shader name is stored with the data that is used to load the Model.
             In this implementation of the library there can be only one shader per model.
@@ -59,28 +73,31 @@
 
         """
         super().__init__(self, model_name)
 
         self.config = models.config
         self.uv = models.uv
         self.models = models
-        self.model_id = model_id
+        self.model_id = model_id if model_id else self.id
         self.name = model_name
 
         self.meshes = []  # list holding instances of mesh class
         self.texture_coordinates = []
 
         # passing shader source file names to the shader
         self.shader = eval(shader)(self, vertex_shader, fragment_shader, geometry_shader)
 
         if ".obj" == pathlib.Path(obj_file).suffix:
-            self.loader = ObjectFileLoader(self)
+            self.loader = ObjectFileLoader(self, config=self.config)
             self.meshes = self.loader.get_meshes(obj_file)
         else:
-            print("not a .obj file")
+            pass
+            # No object file passed, meshes need to be loaded later.
+            self.loader = ObjectFileLoader(self, config=self.config)
+            self.meshes = self.loader.create_empty_mesh()
 
     def get_number_of_meshes_in_model(self) -> int:
         """
         Returns the number of ``Meshes`` in this ``Model``
         """
         return len(self.meshes)
 
@@ -97,15 +114,15 @@
         :type switch: ``int``
         :param scale: ``list`` used for scaling the model
         :type scale:   ``list``
 
         """
 
         # draws all meshes
-        color = color if color else [1.0, 1.0, 1.0, 1.0]
+        color = color if color else [0.0, 0.0, 0.0, 0.5]
         for mesh in self.meshes:
             mesh.draw(self.shader,
                       model_id=self.model_id,
                       position=parent.xyz,
                       orientation=parent.orientation,
                       scale=scale if scale else parent.scale,
                       texture_id=texture_id,
@@ -122,20 +139,7 @@
 # from sphere_base.shader.uv_default_shader import DefaultShader
 # from sphere_base.shader.uv_circle_shader import CircleShader
 # from sphere_base.shader.uv_square_shader import SquareShader
 # from sphere_base.shader.uv_sphere_edge_shader import SphereEdgeShader
 # from sphere_base.shader.uv_cross_shader import CrossShader
 # from sphere_base.shader.uv_holo_sphere_shader import HoloSphereShader
 # from sphere_base.shader.uv_sphere_small_shader import SphereSmallShader
-
-from sphere_base.shader.uv_skybox_shader import SkyboxShader
-from sphere_base.shader.uv_sphere_shader import SphereShader
-from sphere_base.shader.uv_node_shader import NodeShader
-from sphere_base.shader.uv_socket_shader import SocketShader
-from sphere_base.shader.uv_flat_shader import FlatShader
-from sphere_base.shader.uv_default_shader import DefaultShader
-from sphere_base.shader.uv_circle_shader import CircleShader
-from sphere_base.shader.uv_square_shader import SquareShader
-from sphere_base.shader.uv_sphere_edge_shader import SphereEdgeShader
-from sphere_base.shader.uv_cross_shader import CrossShader
-from sphere_base.shader.uv_holo_sphere_shader import HoloSphereShader
-from sphere_base.shader.uv_sphere_small_shader import SphereSmallShader
```

### Comparing `sphere_base-0.0.1/sphere_base/shader/uv_base_shader.py` & `sphere_base-0.1.0/sphere_base/shader/base_shader.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 
 """
 
 from OpenGL.GL import *
 from pyrr import Vector3, matrix44
 import pyrr
 from OpenGL.GL.shaders import compileProgram, compileShader
+from sphere_base.constants import *
 
-from sphere_base.sphere_universe_base.suv_constants import *
+DEBUG = False
 
 
 class BaseShader:
 
     def __init__(self, parent, vertex_shader=None, fragment_shader=None, geometry_shader=None, *args, **kwargs):
         """
         Constructor of the ``BaseShader`` class.
@@ -31,14 +32,16 @@
 
         """
 
         self.config = parent.config
         self.width = self.config.view.view_width
         self.height = self.config.view.view_height
 
+        self.projection_matrix = None
+
         self.vertex_shader = vertex_shader
         self.fragment_shader = fragment_shader
         self.geometry_shader = geometry_shader
 
         self._init_values()
         self.shader_id = self.compile_shader()
         self._init_locations()
@@ -59,26 +62,29 @@
         self.view = None
         self.fov = FOV  # Field of View
         self.near_val = NEAR_VAL
         self.far_val = FAR_VAL
         self.a_color = []
         self.light_id = None
 
+        self.projection_matrix = None
+
     def _init_locations(self):
         """
         can be partially or completely overridden.
 
         """
         self.model_loc = glGetUniformLocation(self.shader_id, "model")
         self.view_loc = glGetUniformLocation(self.shader_id, "view")
         self.proj_loc = glGetUniformLocation(self.shader_id, "projection")
         self.a_color = glGetUniformLocation(self.shader_id, "a_color")
         self.transform_loc = glGetUniformLocation(self.shader_id, "transform")
 
-    def shader_from_file(self, file_name):
+    @staticmethod
+    def shader_from_file(file_name):
         """
         Retrieve shader from .glsl file
         :param file_name: Name of the shader to use
         :param file_name: ``str``
         :returns: the content of the shader to use
 
         """
@@ -94,32 +100,29 @@
         return output
 
     def compile_shader(self):
         """
         compiling the OpenGL shaders
 
         """
-        geometry_source = ""
+
         vertex_source = self.shader_from_file(self.vertex_shader)
         fragment_source = self.shader_from_file(self.fragment_shader)
-        if self.geometry_shader:
-            geometry_source = self.shader_from_file(self.geometry_shader)
 
         if self.geometry_shader:
+            geometry_source = self.shader_from_file(self.geometry_shader)
             shader_id = compileProgram(compileShader(vertex_source, GL_VERTEX_SHADER),
                                        compileShader(fragment_source, GL_FRAGMENT_SHADER),
                                        compileShader(geometry_source, GL_GEOMETRY_SHADER))
         else:
             shader_id = compileProgram(compileShader(vertex_source, GL_VERTEX_SHADER),
                                        compileShader(fragment_source, GL_FRAGMENT_SHADER))
 
         return shader_id
 
-
-
     def set_environment(self):
         """
         Set OpenGL environment
 
         """
         self.set_window_size()
         self.create_light_source()
@@ -135,14 +138,17 @@
             glUniform3f(self.light_id, light_pos.x, light_pos.y, light_pos.z)
 
     def set_buffer_bits(self):
         """
         Set OpenGL buffer bits
 
         """
+        glHint(GL_LINE_SMOOTH_HINT, GL_NICEST)
+        glHint(GL_POLYGON_SMOOTH_HINT, GL_NICEST)
+
         if self.switcher_loc:
 
             glUniform1i(self.switcher_loc, 1)
 
             # background black-ish
             glClearColor(0, 0.1, 0.1, 1)
             glClearStencil(0)
@@ -199,32 +205,33 @@
         if scale is None:
             scale = Vector3([1.0, 1.0, 1.0])
         else:
             scale = Vector3(scale)
 
         return matrix44.create_from_scale(scale)
 
-    def draw(self, object_index: int = 0, object_type: str = "", mesh_index: int = 0, indices: list = None,
-             vertices: list = None, position: 'Vector3' = None, orientation: 'Quaternion' = None,
-             scale: 'Vector3' = None, texture_id: int = 0, color: 'Vector4' = None, switch: int = 0):
+    def draw(self, object_index: int = 0, object_type: str = "", mesh_index: int = 0, indices_len=0,
+             position: 'Vector3' = None, orientation: 'Quaternion' = None,
+             scale: 'Vector3' = None, texture_id: int = 0, color: 'Vector4' = None,
+             switch: int = 0, ):
 
         """
 
         Needs to be extended
 
         Rendering and preparing the OpenGL shader
 
         :param object_index: ID of the object
         :type object_index: ``int``
         :param object_type: Object type name
         :type object_type: ``str``
         :param mesh_index: ID of the Mesh
         :type mesh_index: ``int``
-        :param indices: List of Indices
-        :type indices: ``list``
+        :param indices_len: length of Indices
+        :type indices_len: ``int``
         :param vertices: List of vertex coordinates
         :type indices: ``list``
         :param position: Position of the object
         :type position: ``Vector3``
         :param orientation: Orientation of the object
         :type orientation: ``Quaternion``
         :param scale: object scaling factor
@@ -233,20 +240,29 @@
         :type texture_id: ``int``
         :param color: color to apply
         :type color: ``Vector4``
         :param switch: OpenGL shader switch
         :type switch: ``int``
         """
 
+        if DEBUG:
+            if object_type == "edge1":
+                print("-------------- DRAW MESH -----------")
+                print("mesh_id", mesh_index)
+                print("position", position)
+                print("orientation", orientation)
+                print("scale", scale)
+                print("texture_id", texture_id, "\n")
+
         glUseProgram(self.shader_id)
         glBindVertexArray(self.config.VAO[mesh_index])
 
-        if texture_id > 0:
-            glActiveTexture(GL_TEXTURE0)
-            glBindTexture(GL_TEXTURE_2D, self.config.textures[texture_id])
+        # if texture_id > 0:
+        glActiveTexture(GL_TEXTURE0)
+        glBindTexture(GL_TEXTURE_2D, self.config.textures[texture_id])
 
         obj_pos = matrix44.create_from_translation(Vector3(position))
         glUniformMatrix4fv(self.model_loc, 1, GL_FALSE, obj_pos)
 
         if color:
             glUniform4f(self.a_color, *color)
 
@@ -300,10 +316,9 @@
             # reset to normal
             glDisable(GL_LINE_STIPPLE)
 
         glBegin(GL_LINE_STRIP)
         for point in points:
             glVertex3f(point[0], point[1], point[2])
         glEnd()
-        glDisable(GL_LINE_STIPPLE)  # just in case
+        glDisable(GL_LINE_STIPPLE)  # just in case ....
         glLineWidth(1)
-
```

### Comparing `sphere_base-0.0.1/sphere_base/shader/uv_circle_shader.py` & `sphere_base-0.1.0/sphere_base/shader/circle_shader.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 the circle shader uses an OpenGL geometry shader to draw circles around node discs and sockets.
 
 """
 
 from OpenGL.GL import *
 from OpenGL.GLU import *
-from sphere_base.shader.uv_base_shader import BaseShader
+from sphere_base.shader.base_shader import BaseShader
 from pyrr import matrix44
 
 
 class CircleShader(BaseShader):
     """
     Class representing the circle shader.
 
@@ -33,27 +33,28 @@
             - **scale** - scaling of the circle
 
         """
 
         self.line_width = 1
         self.scale = [1.0, 1.0, 1.0]
 
-    def draw(self, object_index=0, object_type="", mesh_index=0, indices=None,
-             vertices=None, position=None, orientation=None, scale=None,
+    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0,
+             position=None, orientation=None, scale=None,
              texture_id=0, color=None, switch: int = 0):
 
-        super().draw(object_index, object_type, mesh_index, indices, vertices,
-                     position, orientation, scale, texture_id, color)
+        super().draw(object_index=object_index, object_type=object_type, mesh_index=mesh_index, indices_len=indices_len,
+                     position=position, orientation=orientation, scale=scale, texture_id=texture_id,
+                     color=color, switch=switch)
 
         glLineWidth(self.line_width)
 
         rm = matrix44.create_from_inverse_of_quaternion(orientation)
         sm = self.create_scale_matrix(scale)
 
         # combined transformation matrix
         tm = matrix44.multiply(sm, rm)
 
         glUniformMatrix4fv(self.transform_loc, 1, GL_FALSE, tm)
 
-        glDrawElements(GL_POINTS, len(indices) * 3, GL_UNSIGNED_INT, ctypes.c_void_p(0))
+        glDrawElements(GL_POINTS, indices_len * 3, GL_UNSIGNED_INT, ctypes.c_void_p(0))
         glStencilFunc(GL_ALWAYS, object_index, -1)
         glLineWidth(1)
```

### Comparing `sphere_base-0.0.1/sphere_base/shader/uv_cross_shader.py` & `sphere_base-0.1.0/sphere_base/shader/cross_shader.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 the circle shader uses an OpenGL geometry shader to draw circles around node discs and sockets.
 
 """
 
 from OpenGL.GL import *
 from OpenGL.GLU import *
-from sphere_base.shader.uv_base_shader import BaseShader
+from sphere_base.shader.base_shader import BaseShader
 from pyrr import matrix44
 
 
 class CrossShader(BaseShader):
     """
     Class representing the circle shader.
 
@@ -32,27 +32,28 @@
             - **scale** - scaling of the circle
 
         """
 
         self.line_width = 1
         self.scale = [1.0, 1.0, 1.0]
 
-    def draw(self, object_index=0, object_type="", mesh_index=0, indices=None,
-             vertices=None, position=None, orientation=None, scale=None,
+    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0,
+             position=None, orientation=None, scale=None,
              texture_id=0, color=None, switch=0):
 
-        super().draw(object_index, object_type, mesh_index, indices, vertices,
-                     position, orientation, scale, texture_id, color)
+        super().draw(object_index=object_index, object_type=object_type, mesh_index=mesh_index, indices_len=indices_len,
+                     position=position, orientation=orientation, scale=scale, texture_id=texture_id,
+                     color=color, switch=switch)
 
         glLineWidth(self.line_width)
 
         rm = matrix44.create_from_inverse_of_quaternion(orientation)
         sm = self.create_scale_matrix(scale)
 
         # combined transformation matrix
         tm = matrix44.multiply(sm, rm)
 
         glUniformMatrix4fv(self.transform_loc, 1, GL_FALSE, tm)
 
-        glDrawElements(GL_POINTS, len(indices) * 3, GL_UNSIGNED_INT, ctypes.c_void_p(0))
+        glDrawElements(GL_POINTS, indices_len * 3, GL_UNSIGNED_INT, ctypes.c_void_p(0))
         glStencilFunc(GL_ALWAYS, object_index, -1)
         glLineWidth(1)
```

### Comparing `sphere_base-0.0.1/sphere_base/shader/uv_default_shader.py` & `sphere_base-0.1.0/sphere_base/shader/default_shader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # -*- coding: utf-8 -*-
 
 """
 Default shader. This module contains the Default shader class.
 
 """
 
-from sphere_base.shader.uv_base_shader import BaseShader
+from sphere_base.shader.base_shader import BaseShader
 
 DEBUG = False
 
 
 class DefaultShader(BaseShader):
 
     def __init__(self, parent, vertex_shader="vert_default.glsl", fragment_shader="frag_default.glsl", geometry_shader=None):
-        super().__init__(parent, vertex_shader, fragment_shader, geometry_shader)
+
+        super().__init__(parent, vertex_shader=vertex_shader, fragment_shader=fragment_shader, geometry_shader=geometry_shader)
 
     def set_view(self):
         # overriding base class function avoid crash
         pass
```

### Comparing `sphere_base-0.0.1/sphere_base/shader/uv_flat_shader.py` & `sphere_base-0.1.0/sphere_base/shader/flat_shader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # -*- coding: utf-8 -*-
 
 
 from OpenGL.GL import *
 from OpenGL.GLU import *
-from sphere_base.shader.uv_base_shader import BaseShader
+from sphere_base.shader.base_shader import BaseShader
 
 
 class FlatShader(BaseShader):
 
-    def draw(self, object_index=0, object_type="", mesh_index=0, indices=None,
-             vertices: list = None, position=None, orientation=None, scale=None, texture_id=0, color=None, switch=0):
+    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0,
+             position=None, orientation=None, scale=None, texture_id=0,
+             color=None, switch=0):
 
         scale = [scale[0] * .97, scale[1] * .97, scale[2]]
-        super().draw(object_index, object_type, mesh_index, indices, vertices,
-                     position, orientation, scale, texture_id, color)
+
+        super().draw(object_index=object_index, object_type=object_type, mesh_index=mesh_index, indices_len=indices_len,
+                     position=position, orientation=orientation, scale=scale, texture_id=texture_id,
+                     color=color, switch=switch)
 
         if object_type == "rubber_band":
             glUniform4f(self.a_color, *color)
 
-        glDrawElements(GL_TRIANGLES, len(indices) * 3, GL_UNSIGNED_INT, ctypes.c_void_p(0))
-
-
+        glDrawElements(GL_TRIANGLES, indices_len * 3, GL_UNSIGNED_INT, ctypes.c_void_p(0))
```

### Comparing `sphere_base-0.0.1/sphere_base/shader/uv_holo_sphere_shader.py` & `sphere_base-0.1.0/sphere_base/shader/sphere_small_shader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,35 @@
 # -*- coding: utf-8 -*-
 
 """
-Node shader module. This module contains the Node shader class which inherits from the base shader class.
-It is used to render nodes
+This class contains the class that colors the small overview spheres. It inherits from the base shader class.
 
 """
 
 from OpenGL.GL import *
-from sphere_base.shader.uv_base_shader import BaseShader
+from OpenGL.GLU import *
+from sphere_base.shader.base_shader import BaseShader
 
 
-class HoloSphereShader(BaseShader):
+class SphereSmallShader(BaseShader):
 
     def _init_locations(self):
         """
         Initiates the OpenGL locations
 
         """
         super()._init_locations()
         self.switcher_loc = glGetUniformLocation(self.shader_id, "switcher")
 
-    def draw(self, object_index=0, object_type="", mesh_index=0, indices=None, vertices=None,
-             position=None, orientation=None, scale=None, texture_id=0, color=None, switch=0):
+    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0, vertices=None, position=None,
+             orientation=None, scale=None, texture_id=0, color=None, switch=0):
 
-        super().draw(object_index, object_type, mesh_index, indices, vertices,
-                     position, orientation, scale, texture_id, color)
+        super().draw(object_index=object_index, object_type=object_type, mesh_index=mesh_index, indices_len=indices_len,
+                     position=position, orientation=orientation, scale=scale, texture_id=texture_id,
+                     color=color, switch=switch)
 
-        glUniform1i(self.switcher_loc, switch)
-        glUniform4f(self.a_color, *color)
+        glUniform1i(self.switcher_loc, 2)
 
-        # One way to draw with indexes
+        glUniform4f(self.a_color, *color)
         glEnable(GL_CULL_FACE)
-        glDrawElements(GL_TRIANGLES, len(indices) * 3, GL_UNSIGNED_INT, ctypes.c_void_p(0))
-
-        # alternative possibility drawing arrays.....
-        # glDrawArrays(GL_TRIANGLES, 0, len(vertices))
+        glDrawElements(GL_TRIANGLES, indices_len * 3, GL_UNSIGNED_INT, ctypes.c_void_p(0))
         glDisable(GL_CULL_FACE)
-        glStencilFunc(GL_ALWAYS, object_index, -1)
-
-
-
```

### Comparing `sphere_base-0.0.1/sphere_base/shader/uv_node_shader.py` & `sphere_base-0.1.0/sphere_base/shader/socket_shader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 # -*- coding: utf-8 -*-
 
 """
-Node shader module. This module contains the Node shader class which inherits from the base shader class.
+Socket shader module. This module contains the Socket shader class which inherits from the base shader class.
 It is used to render nodes
 
 """
 
 from OpenGL.GL import *
 from OpenGL.GLU import *
-from sphere_base.shader.uv_base_shader import BaseShader
+from sphere_base.shader.base_shader import BaseShader
 
 
-class NodeShader(BaseShader):
+class SocketShader(BaseShader):
 
     def _init_locations(self):
         """
         Initiates the OpenGL locations
 
         """
         super()._init_locations()
         self.switcher_loc = glGetUniformLocation(self.shader_id, "switcher")
 
-    def draw(self, object_index=0, object_type="", mesh_index=0, indices=None,
-             vertices=None, position=None, orientation=None, scale=None, texture_id=0, color=None, switch=0):
+    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0,
+             position=None, orientation=None, scale=None, texture_id=0,
+             color=None, switch=0):
 
-        super().draw(object_index, object_type, mesh_index, indices, vertices,
-                     position, orientation, scale, texture_id, color)
-
-        glUniform1i(self.switcher_loc, switch)
-        glDrawElements(GL_TRIANGLES, len(indices) * 3, GL_UNSIGNED_INT, ctypes.c_void_p(0))
+        super().draw(object_index=object_index, object_type=object_type, mesh_index=mesh_index, indices_len=indices_len,
+                     position=position, orientation=orientation, scale=scale, texture_id=texture_id,
+                     color=color, switch=switch)
 
+        # switch = SHADER_SWITCH[object_type]
+        glUniform1i(self.switcher_loc, 2)
 
+        glUniform4f(self.a_color, *color)
 
+        glDrawElements(GL_TRIANGLES, indices_len * 3, GL_UNSIGNED_INT, ctypes.c_void_p(0))
```

### Comparing `sphere_base-0.0.1/sphere_base/shader/uv_skybox_shader.py` & `sphere_base-0.1.0/sphere_base/shader/skybox_shader.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     This shader is used to render the skybox
 
 """
 
 from OpenGL.GL import *
 from pyrr import Vector3, matrix44
-from sphere_base.shader.uv_base_shader import BaseShader
+from sphere_base.shader.base_shader import BaseShader
 
 
 class SkyboxShader(BaseShader):
 
     def _init_locations(self):
         """
         Initiates the OpenGL locations
@@ -40,25 +40,26 @@
 
         glTexParameteri(GL_TEXTURE_CUBE_MAP, GL_TEXTURE_MIN_FILTER, GL_LINEAR)
         glTexParameteri(GL_TEXTURE_CUBE_MAP, GL_TEXTURE_MAG_FILTER, GL_LINEAR)
         glTexParameteri(GL_TEXTURE_CUBE_MAP, GL_TEXTURE_WRAP_S, GL_CLAMP_TO_EDGE)
         glTexParameteri(GL_TEXTURE_CUBE_MAP, GL_TEXTURE_WRAP_T, GL_CLAMP_TO_EDGE)
         glTexParameteri(GL_TEXTURE_CUBE_MAP, GL_TEXTURE_WRAP_R, GL_CLAMP_TO_EDGE)
 
-    def draw(self, object_index=0, object_type="", mesh_index=0, indices=None,
-             vertices=None, position=None, orientation=None, scale=None, texture_id=0, color=None, switch=0):
+    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0,
+             position=None, orientation=None, scale=None, texture_id=0,
+             color=None, switch=0):
 
         glUseProgram(self.shader_id)
         # glUniformMatrix4fv(self.view_loc, 1, GL_FALSE, self.config.view_loc)
 
         glBindVertexArray(self.config.VAO[mesh_index])
 
         obj_pos = matrix44.create_from_translation(Vector3(self.config.uv.cam.xyz))
         glUniformMatrix4fv(self.model_loc, 1, GL_FALSE, obj_pos)
 
         glDepthMask(GL_FALSE)
-        glDrawElements(GL_TRIANGLES, len(indices) * 3, GL_UNSIGNED_INT, ctypes.c_void_p(0))
+        glDrawElements(GL_TRIANGLES, indices_len * 3, GL_UNSIGNED_INT, ctypes.c_void_p(0))
 
         # clean up code
         glDepthMask(GL_TRUE)
```

### Comparing `sphere_base-0.0.1/sphere_base/shader/uv_socket_shader.py` & `sphere_base-0.1.0/sphere_base/shader/node_shader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 # -*- coding: utf-8 -*-
 
 """
-Socket shader module. This module contains the Socket shader class which inherits from the base shader class.
+Node shader module. This module contains the Node shader class which inherits from the base shader class.
 It is used to render nodes
 
 """
 
 from OpenGL.GL import *
 from OpenGL.GLU import *
-from sphere_base.shader.uv_base_shader import BaseShader
+from sphere_base.shader.base_shader import BaseShader
 
 
-class SocketShader(BaseShader):
+class NodeShader(BaseShader):
 
     def _init_locations(self):
         """
         Initiates the OpenGL locations
 
         """
         super()._init_locations()
         self.switcher_loc = glGetUniformLocation(self.shader_id, "switcher")
 
-    def draw(self, object_index=0, object_type="", mesh_index=0, indices=None,
-             vertices=None, position=None, orientation=None, scale=None, texture_id=0, color=None, switch=0):
+    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0,
+             position=None, orientation=None, scale=None, texture_id=0, texture_file="",
+             color=None, switch=0):
+
+        super().draw(object_index=object_index, object_type=object_type, mesh_index=mesh_index, indices_len=indices_len,
+                     position=position, orientation=orientation, scale=scale, texture_id=texture_id,
+                     color=color, switch=switch)
 
-        super().draw(object_index, object_type, mesh_index, indices, vertices,
-                     position, orientation, scale, texture_id, color)
-
-        # switch = SHADER_SWITCH[object_type]
-        glUniform1i(self.switcher_loc, 2)
-
-        glUniform4f(self.a_color, *color)
-
-        glDrawElements(GL_TRIANGLES, len(indices) * 3, GL_UNSIGNED_INT, ctypes.c_void_p(0))
+        glUniform1i(self.switcher_loc, switch)
+        glDrawElements(GL_TRIANGLES, indices_len * 3, GL_UNSIGNED_INT, ctypes.c_void_p(0))
```

### Comparing `sphere_base-0.0.1/sphere_base/shader/uv_sphere_shader.py` & `sphere_base-0.1.0/sphere_base/shader/sphere_shader.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 Sphere shader module. This module contains the Sphere shader class which inherits from the base shader class.
 It is used to render Sphere
 
 """
 
 from OpenGL.GL import *
 from OpenGL.GLU import *
-from sphere_base.shader.uv_base_shader import BaseShader
+from sphere_base.shader.base_shader import BaseShader
 
-from sphere_base.sphere_universe_base.suv_constants import *
+from sphere_base.constants import *
 
 
 class SphereShader(BaseShader):
     def _init_locations(self):
         """
         Initiates the OpenGL locations
 
@@ -22,25 +22,26 @@
         super()._init_locations()
         self.light_id = glGetUniformLocation(self.shader_id, "LightPosition_world_space")
         self.switcher_loc = glGetUniformLocation(self.shader_id, "switcher")
 
     def set_buffer_bits(self):
         super().set_buffer_bits()
 
-    def draw(self, object_index=0, object_type="", mesh_index=0, indices=None,
-             vertices=None, position=None, orientation=None, scale=None, texture_id=0, color=None, switch=0):
+    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0, position=None,
+             orientation=None, scale=None, texture_id=0, color=None, switch=0):
 
-        super().draw(object_index, object_type, mesh_index, indices, vertices,
-                     position, orientation, scale, texture_id, color)
+        super().draw(object_index=object_index, object_type=object_type, mesh_index=mesh_index, indices_len=indices_len,
+                     position=position, orientation=orientation, scale=scale, texture_id=texture_id,
+                     color=color, switch=switch)
 
         # switch between shaders per object_type
         switch = SHADER_SWITCH[object_type]
         glUniform1i(self.switcher_loc, switch)
 
         # Using element arrays
-        glDrawElements(GL_TRIANGLES, len(indices) * 3, GL_UNSIGNED_INT, ctypes.c_void_p(0))
+        glDrawElements(GL_TRIANGLES, indices_len * 3, GL_UNSIGNED_INT, ctypes.c_void_p(0))
 
         # alternative possibility drawing arrays.....
         # glDrawArrays(GL_TRIANGLES, 0, len(vertices))
 
         glStencilFunc(GL_ALWAYS, object_index, -1)
```

### Comparing `sphere_base-0.0.1/sphere_base/shader/uv_sphere_small_shader.py` & `sphere_base-0.1.0/sphere_base/shader/square_shader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 # -*- coding: utf-8 -*-
 
 """
-This class contains the class that colors the small overview spheres. It inherits from the base shader class.
+Square shader module. This module contains the Node shader class which inherits from the base shader class.
+It is used to render squares like the one used in the rubber band selection box.
 
 """
 
 from OpenGL.GL import *
 from OpenGL.GLU import *
-from sphere_base.shader.uv_base_shader import BaseShader
-from sphere_base.sphere_universe_base.suv_constants import *
+from sphere_base.shader.base_shader import BaseShader
 
 
-class SphereSmallShader(BaseShader):
+class SquareShader(BaseShader):
+    def __init__(self, parent, vertex_shader=None, fragment_shader=None, geometry_shader=None):
+        super().__init__(parent, vertex_shader, fragment_shader, geometry_shader)
+        """
+        Square shader constructor calls the constructor of the base shader
+
+        """
+
+        self.line_width = 1
+        self.scale = [1.0, 1.0, 1.0]
 
     def _init_locations(self):
         """
-        Initiates the OpenGL locations
+        Adds a scale location to the geometric shader to. This scale is the fraction used to
+        correctly scale the border box of size 1 by 1
 
         """
         super()._init_locations()
-        self.switcher_loc = glGetUniformLocation(self.shader_id, "switcher")
+        self.scale_loc = glGetUniformLocation(self.shader_id, "scale")
 
-    def draw(self, object_index=0, object_type="", mesh_index=0, indices=None,
-             vertices=None, position=None, orientation=None, scale=None, texture_id=0, color=None, switch=0):
+    def draw(self, object_index=0, object_type="", mesh_index=0, indices_len=0, position=None,
+             orientation=None, scale=None, texture_id=0, color=None, switch=0):
 
-        super().draw(object_index, object_type, mesh_index, indices, vertices,
-                     position, orientation, scale, texture_id, color)
+        super().draw(object_index=object_index, object_type=object_type, mesh_index=mesh_index, indices_len=indices_len,
+                     position=position, orientation=orientation, scale=scale, texture_id=texture_id,
+                     color=color, switch=switch)
 
-        switch = SHADER_SWITCH[object_type]
-        glUniform1i(self.switcher_loc, 2)
+        glLineWidth(self.line_width)
+        glUniform3f(self.scale_loc, *scale)  # sending the size of the box to the geometric shader
 
-        glUniform4f(self.a_color, *color)
-        glEnable(GL_CULL_FACE)
-        glDrawElements(GL_TRIANGLES, len(indices) * 3, GL_UNSIGNED_INT, ctypes.c_void_p(0))
-        glDisable(GL_CULL_FACE)
+        glDrawElements(GL_POINTS, indices_len * 3, GL_UNSIGNED_INT, ctypes.c_void_p(0))
+        glStencilFunc(GL_ALWAYS, object_index, -1)
+        glLineWidth(1)
```

### Comparing `sphere_base-0.0.1/sphere_base/sphere_overlay/sov_conf.py` & `sphere_base-0.1.0/sphere_base/sphere_overlay/sov_conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 DICTIONARY_SPHERE_NODE_ICONS = \
     {
         "Female": "woman_icon", "LGBT": "lgbt_icon", "Male": "man_icon",
         "Type": "item_icon", "landline": "landline_icon", "laptop": "laptop_icon",
         "mobile": "mobile_icon", "passport": "passport_icon", "pc": "pc_icon",
         "rfid tag": "rfid_tag_icon", "smart card": "smart_card_icon", "smart tv": "smart_tv_icon",
         "smart phone": "smart_phone_icon", "smart watch": "smart_watch_icon", "tablet": "tablet_icon",
-        "webcam": "webcam_icon", "wifi": "wifi_icon"
+        "webcam": "webcam_icon", "wifi": "icon_wifi.png"
     }
 
 
 class ConfException(Exception): pass
 class InvalidNodeRegistration(ConfException): pass
 class OpCodeNotRegistered(ConfException): pass
```

### Comparing `sphere_base-0.0.1/sphere_base/sphere_overlay/sov_sphere.py` & `sphere_base-0.1.0/sphere_base/sphere_overlay/sov_sphere.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,74 @@
 # -*- coding: utf-8 -*-
 
 """
 This is the implementation for the detail sphere_base
 """
 
-from sphere_base.sphere_universe_base.suv_sphere import Sphere
+from sphere_base.sphere.sphere import Sphere
 from sphere_base.sphere_overlay.sov_conf import *
 from sphere_base.sphere_overlay.sphere_nodes.edge_sphere_item import SphereEdge
 import random
+from sphere_base.utils import dump_exception
 
 
-class SplitSphere(Sphere):
+class OverlaySphere(Sphere):
     Edge_class = SphereEdge
 
     def __init__(self, universe, position=None, texture_id=None):
         super().__init__(universe, position, texture_id)
 
         self.set_node_class_selector(self.get_node_class_from_data)
         self._close_event_listeners = []
         self.billboard_id = random.randint(30, 31)
 
+
     def get_model(self):
-        self.cube = self.uv.models.get_model('cube') #model in the middle of the globe
+        # self.cube = self.uv.models.get_model('cube') #model in the middle of the globe
         self.model_h = self.uv.models.get_model('holo_sphere')
         self.model = self.uv.models.get_model('sphere_base')
         self.shader = self.model.shader
 
     def get_node_class_from_data(self, data):
         if 'op_code' not in data:
             return self.Node
         return get_class_from_type(data['op_code'], SPHERE_NODE_EDITOR)
 
-    def create_new_node(self, node_type=0, mouse_x=0, mouse_y=0, abs_pos=None):
+    def create_new_node(self, node_type=0, mouse_ray_collision_point=None):
         # create new node at the mouse pointer
 
         # calculate the cumulative angle based on the mouse position
-        orientation = self.calc_mouse_position_in_angles(mouse_x, mouse_y)
+        orientation = self.calc.find_angle(mouse_ray_collision_point, self.orientation)
 
         # create new node at the cumulative angle
-        if node_type:
 
-            node = get_class_from_type(node_type, SPHERE_NODE_EDITOR)(self, orientation)
-        else:
-            node = self.Node(self, orientation)
+        try:
+
+            if node_type:
+
+                node = get_class_from_type(node_type, SPHERE_NODE_EDITOR)(self, orientation_offset=orientation)
+            else:
+                node = self.Node(self, orientation)
+
+        except Exception as e:
+            dump_exception(e)
 
         self.history.store_history("node created", True)
         return node
 
     def draw(self):
         """
         Render the sphere_base and all the items on it.
         """
-        self.cube.draw(self, self.billboard_id, scale=[0.5, 0.5, 0.5])
-        self.model_h.draw(self, texture_id=1, color=self.color)
+
+        if self.animation != 0:
+            self.rotate_sphere(self.animation)
+
+        # self.cube.draw(self, self.billboard_id, scale=[0.5, 0.5, 0.5])
+        self.model_h.draw(self, texture_id=self.texture_id, color=self.color)
 
         for item in self.items:
             if item.type == "node":
                 item.draw()
             elif item.type == "edge":
                 item.draw()
```

### Comparing `sphere_base-0.0.1/sphere_base/sphere_overlay/sov_sphere_node_base.py` & `sphere_base-0.1.0/sphere_base/sphere_overlay/sov_sphere_node_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 
 
-from sphere_base.sphere_universe_base.suv_node import SphereNode
-from sphere_base.sphere_universe_base.suv_graphic_node import GraphicNode
+from sphere_base.node.node import Node
+from sphere_base.node.graphic_node import GraphicNode
 from sphere_base.sphere_overlay.sov_conf import *
 
 
 class GraphicSphereNode(GraphicNode):
     """ probably needed to add project specific imaging"""
     def __init__(self, node):
         super().__init__(node)
 
 
-class SphereNodeBase(SphereNode):
+class SphereNodeBase(Node):
     GraphicNode_class = GraphicSphereNode
     op_code = OP_SPHERE_NODE_BASE
 
-    def __init__(self, target_sphere, orientation_offset=None):
-        super().__init__(target_sphere, orientation_offset, "node")
+    def __init__(self, target_sphere, orientation_offset=None, yaw_degrees=0, pitch_degrees=0,):
+        super().__init__(target_sphere, orientation_offset, yaw_degrees, pitch_degrees, "node")
         self.node_type_name = "sphere_node_base"
 
     def serialize(self):
         res = super().serialize()
         res['op_code'] = self.__class__.op_code
         return res
```

### Comparing `sphere_base-0.0.1/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py` & `sphere_base-0.1.0/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # -*- coding: utf-8 -*-
 
 
 from sphere_base.sphere_overlay.sov_sphere_node_base import SphereNodeBase
-from sphere_base.sphere_universe_base.suv_graphic_node import GraphicNode
+from sphere_base.node.graphic_node import GraphicNode
 from sphere_base.sphere_overlay.sov_conf import *
 
-# GENDER = ["Male", "Female", "LGBT"]
 
-
-class ItemGraphicNode(GraphicNode):
+class PersonGraphicNode(GraphicNode):
     def __init__(self, node):
         super().__init__(node)
+        self.node_disc_radius = 0.08
 
     def init_assets(self):
         super().init_assets()
-        self.set_icon_by_name("item_icon")
-        self.set_background_color([0.17, 0.07, 0.4, 0.05])
-        self.scale = [2.0, 2.0, 2.0]
-        self.circle_scale = [0.27, 0.30, 0.27]
-
-@register_node(OP_SPHERE_NODE_ITEM, SPHERE_NODE_EDITOR)
-class ItemSphereNode(SphereNodeBase):
-    GraphicNode_class = ItemGraphicNode
-    op_code = OP_SPHERE_NODE_ITEM
-    op_title = "ItemNode"
-
-    def __init__(self, target_sphere, orientation_offset=None):
-        super().__init__(target_sphere, orientation_offset)
-        self.node_type_name = "item_sphere_node"
+        self.set_icon_by_name("icon_man")
+        self.set_background_color([0.07, 0.0, 0.4, 0.1])
+
+@register_node(OP_SPHERE_NODE_PERSON, SPHERE_NODE_EDITOR)
+class PersonSphereNode(SphereNodeBase):
+    GraphicNode_class = PersonGraphicNode
+    op_code = OP_SPHERE_NODE_PERSON
+    op_title = "PersonNode"
+
+    def __init__(self, target_sphere, orientation_offset=None, yaw_degrees=0, pitch_degrees=0):
+
+        super().__init__(target_sphere, orientation_offset, yaw_degrees, pitch_degrees)
+        self.node_type_name = "person_sphere_node"
+        self.gender = None
+
+
```

### Comparing `sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_cam.py` & `sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_cam.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 camera module. Contains the camera class. Is used to create a camera object for the implementation. In the
 current implementation there is only need for a single camera object.
 
 """
 
 from pyrr import Vector3, Vector4, vector, matrix44
 from sphere_base.sphere_universe_base.suv_cam_movement import CameraMovement
-from sphere_base.sphere_universe_base.suv_constants import *
+from sphere_base.utils import dump_exception
 
 MOUSE_SENSITIVITY = .1
-TARGET = Vector3([0.0, 0.0, 0.0])
+DEFAULT_TARGET = Vector3([0.0, 0.0, 0.0])
 DEFAULT_POS = Vector3([0.0, 0.0, 3.0])
 
 
 class Camera:
     CameraMovement_class = CameraMovement
     """
     Class representing the camera. 
@@ -38,78 +38,76 @@
         - **config** - Instance of :class:`~sphere_iot.uv_config.UvConfig` from universe
 
 
         :Instance Variables:
 
         - **target** - ``Vector`` xyz position of the target sphere_base.
         - **distance_to_target** - distance between camera and center of the target sphere_base. (``Vector3``).
-        - **camera_direction** - normalized ``vector3`` pointing away from the center of the target sphere_base through the center of the camera.
+        - **camera_direction** - normalized ``vector3`` pointing away from the center of the target sphere_base
+          through the center of the camera.
         - **camera_up** - ``Vector3`` with the ``up`` position of the camera.
         - **xyz** - position of the camera (``Vector3``).
         - **mouse_sensitivity** - ``float`` modifier to adjust the sensitivity of the mouse when moving the camera.
 
         """
 
-        self._init_variables()
+        # camera target pointing at origin
+        self.target = DEFAULT_TARGET
+        self.xyz = DEFAULT_POS
+        self.distance_to_target = None
+        self.camera_direction = None
+        self.camera_up = None
+
+        self.mouse_sensitivity = MOUSE_SENSITIVITY
+        self.movement_stack = []
+        self.target_stack = []
 
+        self.uv = parent
+        self.target_sphere = None
         self.shader = parent.shader
         self.config = parent.config
 
         self._set_view()
 
         # has the calculations for camera movement
         self.cm = self.__class__.CameraMovement_class(self)
-        self.set_movement_values()
 
         view = self.get_view_matrix()
         self.config.set_view_loc(view)
 
-    def _init_variables(self):
-        # camera target pointing at origin
-        self.target = TARGET
-        self.set_position()
-        self.distance_to_target = None
-        self.camera_direction = None
-        self.camera_up = None
-
-        self.mouse_sensitivity = MOUSE_SENSITIVITY
-        self.movement_stack = []
-        self.target_stack = []
-
     def _set_view(self):
+        sphere_xyz = self.target_sphere.xyz if self.target_sphere else DEFAULT_TARGET
+
         # distance to target
         self.distance_to_target = self.get_distance_to_target()
 
         # direction vector, points away from target
-        self.camera_direction = vector.normalize(Vector3(self.xyz) - Vector3(self.target))
+        self.camera_direction = vector.normalize(Vector3(self.xyz) - Vector3(sphere_xyz))
 
         # right vector that represents the positive x-axis of the camera space
         up = Vector3([0.0, 1.0, 0.0])
         camera_right = vector.normalize(Vector3.cross(up, self.camera_direction))
         self.camera_up = Vector3.cross(Vector3(self.camera_direction), Vector3(camera_right))
 
-    def set_position(self):
-        self.xyz = DEFAULT_POS
-
-    def set_movement_values(self, min_radius=MIN_RADIUS, cam_movement_steps=CAM_MOVEMENT_STEPS):
-        self.cm.set_minimum_values(min_radius, cam_movement_steps)
-
-    def reset_to_default_view(self, target_sphere, default_pos= DEFAULT_POS):
+    def reset_to_default_view(self, target_sphere, offset=None):
         """
         Resetting the camera view to the default view on the sphere_base, without any rotation.
-
+        :param offset: Default position
         :param target_sphere: The target :class:`~sphere_iot.uv_sphere.Sphere` the camera is looking at
         :type target_sphere:  :class:`~sphere_iot.uv_sphere.Sphere`
 
         """
+        pass
 
-        # used when de-serializing
-        self.target = target_sphere.xyz
-        self.xyz = self.target + default_pos
+        offset = Vector3([0.0, 0.0, target_sphere.radius * 2]) if not offset else offset
+        offset = Vector3([0.0, 0.0, target_sphere.radius * 3]) if target_sphere.radius == 1 else offset
+        offset = Vector3([0.0, 0.0, target_sphere.radius * 2.7]) if target_sphere.radius == 2 else offset
 
+        # used when de-serializing
+        self.xyz = target_sphere.xyz + offset
         self.move_to_new_target_sphere(target_sphere)
         self.cm.reset()
         self._set_view()
 
     def get_view_matrix(self) -> 'matrix44':
         """
         Set view and get the look at matrix
@@ -117,49 +115,53 @@
         """
 
         self._set_view()
         m = matrix44.create_look_at(self.xyz, self.target, self.camera_up)
         self.config.set_view_loc(m)
         return m
 
-    def process_mouse_movement(self, target_sphere: 'sphere_base', x_offset: int, y_offset: int):
+    def process_mouse_movement(self, target_sphere, x_offset: int, y_offset: int):
         """
         :param target_sphere: The :class:`~sphere_iot.uv_sphere.Sphere` the camera is looking at
         :type target_sphere: :class:`~sphere_iot.uv_sphere.Sphere`
         :param x_offset: used for rotation
         :type x_offset: ``int``
         :param y_offset: used for up and down (yaw) movement
         :type y_offset: ``int``
 
         """
+
         x_offset *= self.mouse_sensitivity
         y_offset *= self.mouse_sensitivity
 
         self.process_movement(target_sphere, rotation=x_offset, angle_up=y_offset)
 
-    def process_movement(self, target_sphere: 'sphere_base' = None, rotation: int = 0, angle_up: int = 0, radius: int = 0):
+    def process_movement(self, target_sphere=None, rotation: float = 0, angle_up: float = 0,
+                         radius: float = 0):
+
         """
         Moves the camera around the target sphere_base based on received angles.
 
         :param target_sphere: The :class:`~sphere_iot.uv_sphere.Sphere` the camera is looking at
         :type target_sphere: :class:`~sphere_iot.uv_sphere.Sphere`
         :param rotation: rotation angle
         :type rotation: ``int``
         :param angle_up: yaw or angle up or down
         :type angle_up: ``int``
         :param radius: distance to the center of the target sphere_base
         :type radius: ``float``
 
         """
+
         xyzw = self.cm.orbit_around_target(target_sphere, rotation, angle_up, radius)
         self.xyz = Vector3(Vector4(xyzw).xyz)
         view = self.get_view_matrix()
         self.config.set_view_loc(view)
 
-    def move_to_new_target_sphere(self, target_sphere: 'Sphere'):
+    def move_to_new_target_sphere(self, target_sphere):
         """
         Moves the camera from its current location to the new target sphere_base.
 
         :param target_sphere: The new :class:`~sphere_iot.uv_sphere.Sphere` to move to.
         :type target_sphere: :class:`~sphere_iot.uv_sphere.Sphere`
 
         """
@@ -174,30 +176,33 @@
         return self.cm.rotation, self.cm.yaw
 
     def get_distance_to_target(self):
         return vector.length(Vector3(self.target) - Vector3(self.xyz))
 
     def draw(self):
         """
-        Sets the camera view for use with all shaders. If a new sphere_base target is _selected move the camera
+        Sets the camera view for use with all shaders. If a new sphere target is _selected move the camera
         to the new position.
 
         """
 
-        # if a sphere_base has been clicked (_selected) then move the camera to the new sphere_base
+        # if a sphere has been on_current_row_changed (_selected) then move the camera to the new sphere
         if len(self.movement_stack) > 0:
             self.xyz = Vector3(self.movement_stack[0])
             self.target = Vector3(self.target_stack[0])
             del self.movement_stack[0]
             del self.target_stack[0]
 
         # The view needs to be updated before drawing. This is because OpenGL is a state machine that listens to
         # changes program wide spanning instances!
         self.get_view_matrix()
 
-
-
-
-
-
-
+    def get_cam_collision_point(self):
+        #  the collision point on the surface of the sphere with the camera
+        try:
+            p1 = (self.xyz[0], self.xyz[1], self.xyz[2])
+            angle = self.uv.target_sphere.calc.find_angle(p1, self.uv.target_sphere.orientation)
+            # angle, print yaw degrees, pitch degrees
+            print(angle)
+        except Exception as e:
+            dump_exception(e)
```

### Comparing `sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_clipboard.py` & `sphere_base-0.1.0/sphere_base/edge/graphic_edge.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,161 +1,139 @@
 # -*- coding: utf-8 -*-
 
 """
-Clipboard module. Contains the clipboard class.
+Module Graphic Edge. The graphics edge is used with edges.
 
 """
 
-from collections import OrderedDict
-from pyrr import quaternion, Quaternion
-from sphere_base.sphere_universe_base.suv_surface_edge import SphereSurfaceEdge
+from pyrr import quaternion
+from sphere_base.calc import Calc
+import math
 
-DEBUG = False
 
-
-class Clipboard:
+class GraphicEdge:
     """
-    This class deals with serializing and deserializing form and to the clipboard.
-
+    Base class for Graphics Edge
     """
-    def __init__(self, universe):
-        """
-        Constructor of the clipboard class.
 
-        :param universe: The ``Universe``
-        :type universe: reference the :class:`~sphere_iot.uv_universe.Universe`
+    calc_class = Calc
 
+    def __init__(self, parent=None):
         """
+        Constructor of the ``Graphic Edge`` class .
 
-        self.uv = universe
+        :param parent: reference to  :class:`~sphere_iot.uv_edge.SphereSurfaceEdge` or
+        :class:`~sphere_iot.uv_edge_drag.EdgeDrag`.
+        :type parent:  :class:`~sphere_iot.uv_edge.SphereSurfaceEdge` or :class:`~sphere_iot.uv_edge_drag.EdgeDrag`.
 
-    def serialize_selected(self, delete: bool = False) -> 'OrderedDict':
-        """
-        Copy to clipboard
+        :Instance Variables:
 
-        :param delete: when ``cutting`` the _selected items
-        :type delete: ``bool``
-        :returns: ``serialized data`` as a ``OrderedDict``
+            - **edge** - :class:`~sphere_iot.uv_edge.SphereSurfaceEdge` or :class:`~sphere_iot.uv_edge_drag.EdgeDrag`.
+            - **sphere_base** - reference of :class:`~sphere_iot.uv_sphere.Sphere`
+            - **calc** - instance of :class:`~sphere_iot.uv_calc.UvCalc`
 
         """
+        self.edge = parent
+        self.sphere = parent.sphere
+        self.calc = self.__class__.calc_class()
 
-        if DEBUG: print("-- COPY TO CLIPBOARD ---")
-
-        selected_nodes, selected_sockets_ids, selected_edges = [], [], []
-
-        # sort edges and nodes
-        for item in self.uv.target_sphere.items_selected:
-            if item.type == 'node':
-                selected_nodes.append(item.serialize())
-                selected_sockets_ids.append(item.socket.id)
-            elif item.type == 'edge':
-                selected_edges.append(item)
+        self._init_variables()
+        self._init_flags()
+        self._init_assets()
 
-        # debug
-        if DEBUG:
-            print("   NODES\n      ", selected_nodes)
-            print("   EDGES\n      ", selected_edges)
+    def _init_flags(self):
+        self._hover = False
 
-        # remove all edges in the list that are not connected on both sides with _selected nodes
-        edges_to_remove = []
-        for edge in selected_edges:
-             if edge.start_socket.id in selected_sockets_ids and edge.end_socket.id in selected_sockets_ids:
-                 if DEBUG:
-                     print(" edge is ok, connected at both sides with _selected nodes")
-                 pass
-             else:
-                if DEBUG:
-                    print("edge", edge, "is not connected on both sides with _selected nodes")
-                edges_to_remove.append(edge)
-        for edge in edges_to_remove:
-            selected_edges.remove(edge)
+    def _init_variables(self):
+        self._selected = False
+        self._current_color = None
 
-        # make final list of edges
-        edges_final = []
-        for edge in selected_edges:
-            edges_final.append(edge.serialize())
+        self.unit_length = 0.05
+        self.color = [0, 0, 0, .5]
 
-        if DEBUG:
-            print("our final list of edges:", edges_final)
+    def _init_assets(self):
+        """Initialize ``QObjects`` like ``QColor``, ``QPen`` and ``QBrush``"""
+        self.default_color = [0, 0, 0, .5]  # black
+        self.selected_color = [0.9, 0.0, 0.0, 0.4]
+        self.hover_color = [191, 255, 0, 1]
 
-        data = OrderedDict([
-            ('nodes', selected_nodes),
-            ('edges', edges_final),
-            ])
-
-        # if CUT (aka delete) remove _selected items from the sphere_base
-        if delete:
-            self.uv.target_sphere.delete_selected_items()
-            self.uv.target_sphere.history.store_history("Cut out elements from scene", set_modified=True)
+    def count_vertices(self, start_xyz: 'Vector3', end_xyz: 'Vector3', radius: float, unit_length: float):
+        """
+        Returns the number of vertices on the edge.
 
-        return data
+        :param start_xyz: start position
+        :type start_xyz: ``Vector3``
+        :param end_xyz: end position
+        :type end_xyz: ``Vector3``
+        :param radius: radius of the sphere_base
+        :type radius: ``float``
+        :param unit_length: length of each unit
+        :type unit_length: ``float``
+        :returns: ``int`` number of edge elements
 
-    def deserialize_from_clipboard(self, data: 'OrderedDict') -> list:
         """
-        Paste data from clipboard to the target sphere_base.
-
-        :param data: Data to deserialize
-        :type data: ``OrderedDict``
-        :return: list with nodes
+        # shortest distance over the surface of the globe between start socket and edge-end
+        length = self.calc.get_distance_on_sphere(end_xyz, start_xyz, radius)
+        return int(math.ceil(length / unit_length))
 
-        .. warning::
+    def get_position(self, pos_orientation_offset: 'Quaternion', radius=None) -> 'Vector3':
+        """
+        Returns xyz vector based on degree offset (position orientation offset)
 
-            Pasting a group of sphere_base nodes does locate the nodes in the expected position. The nodes are pasted
-            inverse of what is expected. The top node is pasted at the bottom and the bottom node is pasted at the top.
+        :param pos_orientation_offset: degree offset from the zero-position of the ``Sphere``.
+        :param pos_orientation_offset: ``Quaternion``
+        :returns: ``Vector3`` xyz-position
 
-            Also the connected edges are not copied and pasted.
+        """
+        cumulative_orientation = self.get_cumulative_rotation(pos_orientation_offset)
 
-            This needs to be looked into in a future iteration.
+        # get the position of the edge vertex on the sphere_base, calculated from the cumulative rotation
+        xyz = self.calc.move_to_position(cumulative_orientation, self.sphere)
+        return xyz
 
+    def get_cumulative_rotation(self, pos_orientation_offset: 'Quaternion') -> 'Quaternion':
         """
-        hashmap = {}
-
-        # # create each node
-        created_nodes = []
+        Returns the cumulative rotation of the pos_orientation_offset with the sphere rotation.
 
-        length = len(data['nodes'])
+        :param pos_orientation_offset: degree offset from the zero-position of the ``Sphere``.
+        :type pos_orientation_offset: ``Quaternion``
+        :returns: ``Quaternion`` cumulative offset
+        """
+        # rotation of the sphere with rotation offset of the pointer rotation
+        return quaternion.cross(pos_orientation_offset, quaternion.inverse(self.sphere.orientation))
 
-        for i, node_data in enumerate(data['nodes']):
-            q = Quaternion(node_data['orientation_offset'])
+    def on_selected_event(self, event):
+        """
+        Changing the color of the edge when selected.
 
-            if i == 0:
-                a = q
-                middle = q
-            else:
-                middle = quaternion.slerp(a, q, .5)
+        :returns: ``Vector4`` color
 
-        for i, node_data in enumerate(data['nodes']):
+        """
+        self._selected = event
+        if event:
+            self._current_color = self.selected_color
+        else:
+            self._current_color = self.default_color
+        return self._current_color
 
-            new_node = self.uv.target_sphere.get_node_class_from_data(node_data)(self.uv.target_sphere)
-            new_node.deserialize(node_data, hashmap, restore_id=False)
-            created_nodes.append(new_node)
+    def on_hover_event(self, event=False):
+        """
+        Changing the color of the edge when hovered.
 
-            new_node.on_selected_event(True)
-            self.uv.target_sphere.select_item(new_node, False if i == 0 else True)
+        :returns: ``Vector4`` color
 
-            diff = quaternion.cross(quaternion.inverse(new_node.pos_orientation_offset), middle)
+        """
+        if self._hover and event:
+            return self._current_color
 
-            if length == 1:
-                new_center = self.uv.target_sphere.calc_mouse_position_in_angles(self.uv.mouse_x, self.uv.mouse_y)
-                new_node.pos_orientation_offset = new_center
-                new_node.update_position()
+        elif self._hover and not event:
+            if self._selected:
+                self._current_color = self.selected_color
             else:
-                new_center = self.uv.target_sphere.calc_mouse_position_in_angles(self.uv.mouse_x, self.uv.mouse_y)
-                new_node.pos_orientation_offset = quaternion.cross(new_center, diff)
-                new_node.update_position()
-
-        # create each edge
-        if 'edges' in data:
-            for edge_data in data['edges']:
-                new_edge = SphereSurfaceEdge(self.uv.target_sphere)
-                new_edge.deserialize(edge_data, hashmap, restore_id=False)
-
-        # store history
-        self.uv.target_sphere.history.store_history("Pasted elements in scene", set_modified=True)
-
-        return created_nodes
-
-
-
-
+                self._current_color = self.default_color
+            self._hover = False
 
+        elif event:
+            self._hover = True
+            self._current_color = self.hover_color
 
+        return self._current_color
```

### Comparing `sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_config.py` & `sphere_base-0.1.0/sphere_base/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # -*- coding: utf-8 -*-
 
 """
 A module containing the Configuration class.
 
 """
 
-from sphere_base.sphere_universe_base.suv_constants import *
+from sphere_base.constants import *
 import os
 
+
 class UvConfig:
     """
     The configuration class contains project wide variables which can be easily shared between modules and classes.
 
     """
-    def __init__(self, universe, skybox_img_directory=""):
+    def __init__(self, universe, skybox_img_dir="", sphere_texture_dir=""):
         """
         Constructor of the sphere_base class.
 
         :param universe: reference to the :class:`~sphere_iot.uv_universe.Universe`
         :type universe: :class:`~sphere_iot.uv_universe.Universe`
 
         :Instance Variables:
@@ -28,65 +29,88 @@
         """
 
         self.uv = universe
         self.view = self.uv.view
         self.view_loc = None
 
         # project wide opengl buffers
-        self.VAO = None  # Vertex arrays objects indexes
-        self.VBO = None  # Vertex buffers objects indexes
-        self.EBO = None  # Element array buffer object indexes
+        self.VAO = []  # Vertex arrays objects indexes
+        self.VBO = []  # Vertex buffers objects indexes
+        self.EBO = []  # Element array buffer object indexes
 
         self.mesh_id_counter = 0  # used in creating new indexes for meshes
 
-        self.textures = []
-        self._textures = {}
         self._win_size_changed_listeners = []
         self._view_changed_listeners = []
 
-        self.skybox_sets = self.create_skybox_set(skybox_img_directory)
+        self.skybox_sets = self.create_skybox_set(skybox_img_dir)
+        self.sphere_textures = self.create_texture_set(SPHERE_TEXTURE_DIR, sphere_texture_dir)
+        self.all_textures = self.create_texture_dict(SPHERE_TEXTURE_DIR, sphere_texture_dir, TEXTURES_DIR, ICONS_DIR)
 
     @staticmethod
     def create_skybox_set(skybox_dir=""):
-        # find all directories that hold skybox images and add them to a list
-
         set0 = [None]
         set2 = []
-
         set1 = [SKYBOX_IMG_DIR + name for name in os.listdir(SKYBOX_IMG_DIR) if
                 os.path.isdir(os.path.join(SKYBOX_IMG_DIR, name))]
         if skybox_dir:
             set2 = [skybox_dir + name for name in os.listdir(skybox_dir) if
                     os.path.isdir(os.path.join(skybox_dir, name))]
 
-        sets = set0 + set1 + set2
+        return set0 + set1 + set2
 
-        return sets
+    def create_texture_dict(self, dir1, dir2, dir3, dir4):
+        # Get all textures from the 3 directories in a dictionary
+        textures = self.create_texture_set(dir1, dir2, dir3, dir4)
+        _dict = {}
+
+        for index, file_name in enumerate(textures):
+            key = os.path.basename(file_name)
+            _type = os.path.split(os.path.dirname(file_name))[1]
+            if key in _dict:
+                continue
+            if os.path.isfile(file_name):
+                if file_name.endswith('.jpg') or file_name.endswith('.png'):
+                    _dict[key] = {}
+                    _dict[key]['file_name'] = key
+                    _dict[key]['img_id'] = index
+                    _dict[key]['file_dir_name'] = file_name
+                    _dict[key]['type'] = _type[:-1]  # removing the 's'
+        return _dict
 
-    def set_view_loc(self, view: 'matrix'):
+    @staticmethod
+    def create_texture_set(*args):
+        # puts all the files of all the directories in a list
+        _set = []
+        for directory in args:
+            s = [directory + file_name for file_name in os.listdir(directory)]
+            _set += s
+        return _set
+
+    def set_view_loc(self, view):
         """
         Setting the view matrix to be used in OpenGL
 
         :param view: The view matrix
         :type view: ``Matrix``
 
         """
         self.view_loc = view
         self.on_view_changed()
 
-    def add_win_size_changed_listener(self, callback: 'function'):
+    def add_win_size_changed_listener(self, callback):
         """
         Register callback for 'win size changed' event.
 
         :param callback: callback function
 
         """
         self._win_size_changed_listeners.append(callback)
 
-    def add_view_changed_listener(self, callback: 'function'):
+    def add_view_changed_listener(self, callback):
         """
         Register callback for 'view changed' event.
 
         :param callback: callback function
 
         """
         self._view_changed_listeners.append(callback)
@@ -103,39 +127,32 @@
         """
         Handles 'view changed', calls registered listeners.
 
         """
         for callback in self._view_changed_listeners:
             callback()
 
-    def create_texture_by_name_dictionary(self):
-        """
-        Creating a texture dictionary indexed by name
-
-        """
-        for texture in TEXTURES:
-            texture_id, texture_name = texture[0], texture[1]
-            self._textures[texture_name] = texture_id
-
     def get_img_id(self, img_name) -> int:
         """
         Returns texture id of the texture name received.
 
         :param img_name: name of the texture/image/icon to retrieve
         :type img_name: str
 
         """
-        if img_name in self._textures:
-            return self._textures[img_name]
-        return None
+
+        image_id = None
+        for index, _item in enumerate(self.uv.config.all_textures.values()):
+            if _item['file_name'] == img_name or _item['file_name'][:-4] == img_name:
+                image_id = _item['img_id']
+                continue
+        return image_id
 
     def get_mesh_id(self) -> int:
         """
         Returns a new 'mesh id' and increases the mesh id counter
 
         """
 
         mesh_id = self.mesh_id_counter
         self.mesh_id_counter += 1
         return mesh_id
-
-
```

### Comparing `sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_edge_drag.py` & `sphere_base-0.1.0/sphere_base/edge/edge_drag.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,33 +2,36 @@
 
 """
 Edge_drag module. contains the EdgeDraw class which is responsible for drawing a new edge.
 
 """
 
 from pyrr import quaternion
-from sphere_base.sphere_universe_base.suv_socket import *
-from sphere_base.sphere_universe_base.suv_graphic_edge import GraphicEdge
+from sphere_base.node.socket import *
+from sphere_base.edge.graphic_edge import GraphicEdge
+from sphere_base.shader.sphere_shader import SphereShader
 
 
 class EdgeDrag:
+
     GraphicsEdge_class = GraphicEdge
+    Shader_class = SphereShader
+
     """
     This class takes care of dragging a new edge. SLERP-ing Quaternions to determine the angle 
     with the center of the sphere_base.
     
     """
 
-    def __init__(self, Sphere):
+    def __init__(self, sphere):
         """
         Constructor of the edge dragg class.
 
-
-        :param Sphere: This class is instantiated from the :class:`~sphere_iot.uv_sphere.Sphere`
-        :type Sphere: :class:`~sphere_iot.uv_sphere.Sphere`
+        :param sphere: This class is instantiated from the :class:`~sphere_iot.uv_sphere.Sphere`
+        :type sphere: :class:`~sphere_iot.uv_sphere.Sphere`
 
         :Instance Attributes:
 
         - **gr_edge** - Instance of :class:`~sphere_iot.uv_edge.SphereSurfaceEdge`
         - **calc** - Instance of :class:`~sphere_iot.uv_calc.UvCalc` from universe
 
         :Instance Variables:
@@ -36,39 +39,41 @@
         - **uv** - reference to :class:`~sphere_iot.uv_universe.Universe`
         - **sphere_base** - reference to :class:`~sphere_iot.uv_sphere.Sphere`
         - **config** - reference to :class:`~sphere_iot.uv_config.UvConfig`
         - **shader** - reference to :class:`~sphere_iot.shader.uv_base_shader.BaseShader`
         - **radius** - radius of the sphere_base this node is on.
         - **start_socket** - reference to :class:`~sphere_iot.uv_socket.Socket`
         - **xyz** - ``Vector`` location of the loose edge end.
-        - **pos_orientation_offset** - quaternion position of the edge end relative to the zero rotation of the sphere_base.
+        - **pos_orientation_offset** - quaternion position of the edge end relative to the
+          zero rotation of the sphere_base.
 
         : Properties:
             - **dragging** - property flag indicating whether the edge being dragged
 
         """
-        self.sphere = Sphere
-        self.config = Sphere.config
+        self.sphere = sphere
+        self.config = sphere.config
         self._init_variables()
 
     def _init_variables(self):
         self.uv = self.sphere.uv
         self.shader = self.sphere.shader
+        # self.shader = self.__class__.Shader_class(self)
 
         self.radius = self.sphere.radius
         self.start_socket = None
         self.xyz = None
         self.pos_orientation_offset = None
         self._dragging = False
 
         self.unit_length = 0.04
         self.pos_array = []
 
         self.gr_edge = self.__class__.GraphicsEdge_class(self)
-        self.calc = UvCalc()
+        self.calc = Calc()
 
     def _init_start_dragging(self, start_socket: 'Socket'):
         # dragging start point is the start socket
         self.start_socket = start_socket
         self.xyz = start_socket.xyz  # position of the mouse at start
         self.pos_orientation_offset = self.start_socket.node.pos_orientation_offset
 
@@ -89,24 +94,22 @@
         return self._dragging
 
     @dragging.setter
     def dragging(self, value: bool):
         if not self._dragging and value:
             self._dragging = value
 
-    def drag(self, start_socket: 'socket', x_offset: float, y_offset: float, dragging: bool):
+    def drag(self, start_socket: 'socket', dragging: bool, mouse_ray_collision_point=None):
         """
         Dragging an edge
 
         :param start_socket:
         :type start_socket: :class:`~sphere_iot.uv_socket.Socket`
-        :param x_offset: mouse x-offset
-        :type x_offset: ``float``
-        :param y_offset: mouse y-offset
-        :type y_offset: ``float``
+        :param mouse_ray_collision_point: mouse x-offset
+        :type mouse_ray_collision_point: ``float``
         :param dragging: ``True`` when dragging
         :type dragging: ``bool``
 
         """
 
         if not dragging:
             self._stop_dragging()
@@ -114,22 +117,24 @@
         else:
             self._dragging = True
 
         if not self.start_socket:
             self._init_start_dragging(start_socket)
             return
 
-        # the location of the point under the mouse pointer
-        self.xyz = self.drag_to(x_offset, y_offset)
+        # we recalculate the xyz from the angles as there is a discrepancy with the collision point
+        self.xyz = self.drag_to(mouse_ray_collision_point)
+
+        # self.xyz = Vector3(mouse_ray_collision_point)  # we could use this if there would have been no difference
         self.snap_to_socket()
 
         # number of points this edge is made off
-        n = self.gr_edge.get_number_of_points(self.start_socket.xyz, self.xyz, self.radius, self.unit_length)
+        n = self.gr_edge.count_vertices(self.start_socket.xyz, self.xyz, self.radius, self.unit_length)
 
-        if n > 0:
+        if n:
             step = 1 / n
             self.update_edge(n, step)
 
     def snap_to_socket(self):
         """
         When an edge end get close to a socket it 'snaps' to the socket.
         
@@ -156,30 +161,28 @@
 
         """
         self.pos_array = [[self.xyz[0], self.xyz[1], self.xyz[2]]]  # first point
         for i in range(1, number_of_elements):
             pos_orientation_offset = quaternion.slerp(
                 self.pos_orientation_offset, self.start_socket.pos_orientation_offset, step * i)
 
-            # take the position of each point and add to array
-            pos = self.gr_edge.get_position(pos_orientation_offset)
+            # get the position of each point and add to array
+            pos = self.gr_edge.get_position(pos_orientation_offset, self.sphere.radius)
             self.pos_array.append([pos[0], pos[1], pos[2]])
 
-    def drag_to(self, pitch_degrees: int, yaw_degrees: int) -> 'Vector3':
+    def drag_to(self, mouse_abs_pos):
         """
+        Used to Drag a line on the globe to the mouse_ray collision point.
 
-        :param pitch_degrees: horizontal rotation
-        :param yaw_degrees: vertical yaw
+        :param mouse_abs_pos: mouse_ray collision point
         :returns: xyz 'Vector3'
         """
-        # get the new position orientation offset angle based on pitch and yaw
-        self.pos_orientation_offset = self.calc.get_pos_orientation_offset(pitch_degrees, yaw_degrees,
-                                                                           self.pos_orientation_offset)
-        return self.gr_edge.get_position(self.pos_orientation_offset)
+        self.pos_orientation_offset = self.calc.find_angle(mouse_abs_pos, self.sphere.orientation)
+        return self.gr_edge.get_position(self.pos_orientation_offset, self.sphere.radius)
 
     def draw(self):
         """
         Drawing the edge with dotted lines.
 
         """
         if self._dragging:
-            self.shader.draw_edge(self.pos_array, width=3, color=[0, 0, 0, 1], dotted=True)
+            self.shader.draw_edge(self.pos_array, width=2, color=[0, 0, 0, 1], dotted=True)
```

### Comparing `sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_graphic_disc.py` & `sphere_base-0.1.0/sphere_base/node/graphic_disc.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,50 +2,59 @@
 
 """
 Module Graphic Disc. The graphics disc class is used in all nodes and sockets.
 
 """
 
 
-
-class EditorGraphicDisc:
-    def __init__(self, node: 'SphereNode'):
+class GraphicDisc:
+    def __init__(self, node: 'Node'):
         """
         Constructor of the ``Editor Graphic Disc`` class. Contains graphic elements.
 
-        :param node: reference to  :class:`~sphere_iot.uv_node.SphereNode`.
-        :type node:  :class:`~sphere_iot.uv_node.SphereNode`
+        :param node: reference to  :class:`~sphere_iot.uv_node.Node`.
+        :type node:  :class:`~sphere_iot.uv_node.Node`
 
         :Instance Variables:
 
-            - **node** - :class:`~sphere_iot.uv_node.SphereNode`.
+            - **node** - :class:`~sphere_iot.uv_node.Node`.
             - **current_img_id** - id of the current active image.
             - **last_img_id** - id of the last active image.
             - **default_img_id** - id of the default image
             - **selected_img_id** - id of the image when the item is _selected.
             - **hover_img_id** - id of the image when the item is hovered with the mouse pointer.
             - **default_background_color** - ``list``
             - **selected_background_color** - ``list``
             - **hover_background_color** - ``list``
             - **current_background_color** - ``list``
 
         """
 
         self.node = node
-        self._init_flags()
-        self._init_variables()
-        self.init_assets()
-
-    def _init_flags(self):
         self._hover = False
         self._selected = False
-
-    def _init_variables(self):
         self.current_img_id = None
         self.last_img_id = None
+        self.default_img_id, self.selected_img_id, self.hover_img_id = None, None, None
+        self.current_img_id, self.last_img_id = None, None
+
+        self.scale, self.circle_scale, self.default_img_id, self.selected_img_id = None, None, None, None
+        self.hover_img_id, self.main_image_color, self.default_background_color = None, None, None
+
+        self.selected_background_color, self.hover_background_color, self.default_border_color = None, None, None
+        self.selected_border_color, self.hover_border_color, self.default_border_width = None, None, None
+        self.selected_border_width, self.hover_border_width = None, None
+
+        self.current_img_id = self.default_img_id
+        self.current_background_color = self.default_background_color
+        self.current_border_color = self.default_border_color
+        self.current_border_width = self.default_border_width
+
+        self.last_img_id = self.default_img_id
+        self.init_assets()
 
     def _init_unified_icons(self, img_id: int) -> int:
         """
         This function sets all icons the same, independent of its state. Therefore
         there is no difference between hovered, _selected and default.
 
         .. Warning::
```

### Comparing `sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_graphic_edge.py` & `sphere_base-0.1.0/sphere_base/model/mesh.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,142 +1,109 @@
 # -*- coding: utf-8 -*-
 
 """
-Module Graphic Edge. The graphics edge is used with edges.
-
+**mesh** - Instance of :class:`~sphere_iot.uv_models.Mesh`
 """
 
-from pyrr import quaternion
-from sphere_base.sphere_universe_base.suv_calc import UvCalc
-
+import numpy as np
+from sphere_base.utils import dump_exception
 
-class GraphicEdge:
-    """
-    Base class for Graphics Edge
-    """
+DEBUG = False
 
-    calc_class = UvCalc
 
-    def __init__(self, parent=None):
+class Mesh:
+    def __init__(self, model, mesh_id, vertices, indices, buffer):
         """
-        Constructor of the ``Graphic Edge`` class .
-
-        :param parent: reference to  :class:`~sphere_iot.uv_edge.SphereSurfaceEdge` or :class:`~sphere_iot.uv_edge_drag.EdgeDrag`.
-        :type parent:  :class:`~sphere_iot.uv_edge.SphereSurfaceEdge` or :class:`~sphere_iot.uv_edge_drag.EdgeDrag`.
+        Constructor of the ``Mesh`` class. Holds and draws a single mesh.
+
+        :param model: the :class:`~sphere_iot.uv_models.Model` this ``Mesh`` belongs to.
+        :type model: :class:`~sphere_iot.uv_models.Model`
+        :param mesh_id: id of this mesh.
+        :type mesh_id: ``int``
+        :param vertices: Array of Vertex positions
+        :type vertices: ``np.array``
+        :param indices: Indices array
+        :type indices: ``np.array``
+        :param buffer: Buffer array
+        :type buffer: ``np.array``
 
         :Instance Variables:
 
-            - **edge** - :class:`~sphere_iot.uv_edge.SphereSurfaceEdge` or :class:`~sphere_iot.uv_edge_drag.EdgeDrag`.
-            - **sphere_base** - reference of :class:`~sphere_iot.uv_sphere.Sphere`
-            - **calc** - instance of :class:`~sphere_iot.uv_calc.UvCalc`
-
-        """
-        self.edge = parent
-        self.sphere = parent.sphere
-        self.calc = self.__class__.calc_class()
-
-        self._init_variables()
-        self._init_flags()
-        self._init_assets()
-
-    def _init_flags(self):
-        self._hover = False
-
-    def _init_variables(self):
-        self._selected = False
-        self._current_color = None
-
-        self.unit_length = 0.1
-        self.color = [0, 0, 0, .5]
-
-    def _init_assets(self):
-        """Initialize ``QObjects`` like ``QColor``, ``QPen`` and ``QBrush``"""
-        self.default_color = [0, 0, 0, .5]  # black
-        self.selected_color = [255, 0, 0, 1]
-        self.hover_color = [191, 255, 0, 1]
-
-    def get_number_of_points(self, start_xyz: 'Vector3', end_xyz: 'Vector3', radius: float, unit_length: float):
-        """
-        Returns the number of vertices on the edge.
-
-        :param start_xyz: start position
-        :type start_xyz: ``Vector3``
-        :param end_xyz: end position
-        :type end_xyz: ``Vector3``
-        :param radius: radius of the sphere_base
-        :type radius: ``float``
-        :param unit_length: length of each unit
-        :type unit_length: ``float``
-        :returns: ``int`` number of edge elements
-
-        """
-        # shortest distance over the surface of the globe between start socket and edge-end
-        length = self.calc.get_distance_on_sphere(end_xyz, start_xyz, radius)
-
-        # calculate how many edge_elements fit on the edge length.
-        return int(length / unit_length)
-
-    def get_position(self, pos_orientation_offset: 'Quaternion') -> 'Vector3':
-        """
-        Returns xyz vector based on degree offset (position orientation offset)
-
-        :param pos_orientation_offset: degree offset from the zero-position of the ``Sphere``.
-        :param pos_orientation_offset: ``Quaternion``
-        :returns: ``Vector3`` xyz-position
-
-        """
-        cumulative_orientation = self.get_cumulative_rotation(pos_orientation_offset)
-
-        # get the position of the edge vertex on the sphere_base, calculated from the cumulative rotation
-        xyz = self.calc.move_to_position(cumulative_orientation, self.sphere, self.sphere.radius)
-        return xyz
-
-    def get_cumulative_rotation(self, pos_orientation_offset: 'Quaternion') -> 'Quaternion':
-        """
-        Returns the cumulative rotation of the pos_orientation_offset with the sphere_base rotation.
-
-        :param pos_orientation_offset: degree offset from the zero-position of the ``Sphere``.
-        :type pos_orientation_offset: ``Quaternion``
-        :returns: ``Quaternion`` cumulative offset
-        """
-        # rotation of the sphere_base with rotation offset of the pointer rotation
-        return quaternion.cross(pos_orientation_offset, quaternion.inverse(self.sphere.orientation))
-
-    def on_selected_event(self, event):
-        """
-        Changing the color of the edge when selected.
-
-        :returns: ``Vector4`` color
-
-        """
-        self._selected = event
-        if event:
-            self._current_color = self.selected_color
-        else:
-            self._current_color = self.default_color
-        return self._current_color
-
-    def on_hover_event(self, event=False):
-        """
-        Changing the color of the edge when hovered.
-
-        :returns: ``Vector4`` color
-
-        """
-        if self._hover and event:
-            return self._current_color
-
-        elif self._hover and not event:
-            if self._selected:
-                self._current_color = self.selected_color
-            else:
-                self._current_color = self.default_color
-            self._hover = False
-
-        elif event:
-            self._hover = True
-            self._current_color = self.hover_color
-
-        return self._current_color
-
-
-
+            - **model** - The :class:`~sphere_iot.uv_models.Model` this ``Mesh`` belongs to.
+            - **models** - :class:`~sphere_iot.uv_models.Models`.
+            - **shader** - A dedicated shader for this ``Mesh``.
+            - **model_id** - id of the `:class:`~sphere_iot.uv_models.Model` this ``Mesh`` belongs to.
+            - **mesh_id** - id of the Mesh.
+
+        """
+        self.model = model
+        self.shader = model.shader
+        self.mesh_id = mesh_id
+
+        self.vertices = np.array(vertices, dtype=np.float32)  # vertex coordinates
+        self.indices = np.array(indices, dtype='uint32')
+        self.buffer = np.array(buffer, dtype=np.float32)
+        self.indices_len = len(self.indices)
+
+    def save_memory(self):
+        """
+        During setup static model meshes are stored in the VBO,
+        after that the memory can be released as it is not used anymore.
+
+        Dynamic models will need these variables as the model will change and needs to be reloaded
+        in the VBO.
+
+        :return:
+        """
+        self.vertices = None
+        self.indices = None
+        self.buffer = None
+
+    def draw(self, shader: 'Shader', model_id: int, position: 'Vector3', orientation: 'Quaternion', scale: list = None,
+             texture_id: int = 0, color: list = None, switch: int = 0):
+        """
+        Sending the ``Mesh`` with all the parameters to the dedicated shader.
+
+        :param shader: Each ``Model`` gets its own ``Shader`` allocated.
+        :type shader: :class:`~sphere_iot.shader.uv_base_shader.BaseShader`.
+        :param model_id: The id of :class:`~sphere_iot.uv_models.Model` this ``Mesh`` is on.
+        :type model_id: ``int``
+        :param position: Position of the :class:`~sphere_iot.uv_models.Model`
+        :type position: ``Vector3``
+        :param orientation: The direction the :class:`~sphere_iot.uv_models.Model` is pointing at
+        :type orientation: ``Quaternion``
+        :param scale: ``vector`` used to scale the :class:`~sphere_iot.uv_models.Model`
+        :type scale: ``Vector3`` scale of the Mesh
+        :param texture_id: The ``id`` of the texture to put on the ``Mesh``.
+        :type texture_id: ``int``
+        :param color: ``rbg array``
+        :type color: ``Array``
+        :param switch: Switch used in the shader to switch from one behaviour to another.
+        :type switch: ``int``
+        """
+
+        if DEBUG:
+            if self.model.type == "edge1":
+                print("-------------- DRAW MESH -----------")
+                print("model, model_type", model_id, self.model.type)
+                print("mesh_id", self.mesh_id)
+                print("indices_len", self.indices_len)
+                print("position", position)
+                print("orientation", orientation)
+                print("scale", scale)
+                print("texture_id", texture_id, "\n")
+
+        try:
+            shader.draw(
+                         object_index=model_id,
+                         object_type=self.model.type,
+                         mesh_index=self.mesh_id,
+                         indices_len=self.indices_len,
+                         position=position,
+                         orientation=orientation,
+                         scale=scale,
+                         texture_id=texture_id,
+                         color=color,
+                         switch=switch
+                         )
+        except Exception as e:
+            dump_exception(e)
```

### Comparing `sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_graphic_node.py` & `sphere_base-0.1.0/sphere_base/node/graphic_socket.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,75 +1,65 @@
 # -*- coding: utf-8 -*-
 
 """
-Module Graphic Node. The graphics node is used in all nodes and sockets.
+Module Graphic Socket. The graphics socket initializes the graphic assets for the sockets
 
 """
 
-from sphere_base.sphere_universe_base.suv_graphic_disc import EditorGraphicDisc
+from sphere_base.node.graphic_disc import GraphicDisc
 
 
-class GraphicNode(EditorGraphicDisc):
+class GraphicSocket(GraphicDisc):
     def __init__(self, node):
         """
-        Constructor of the ``Editor Graphic Node`` class. Contains graphic elements.
+        Constructor of the ``Graphic Socket`` class. Contains graphic elements.
 
-        :param node: reference to any inherited class of :class:`~sphere_iot.uv_node.SphereNode`.
-        :type node:  :class:`~sphere_iot.uv_node.SphereNode`
+        :param node: reference to any inherited class of :class:`~sphere_iot.uv_node.Node`.
+        :type node:  :class:`~sphere_iot.uv_node.Node`
 
         :Instance Variables:
 
-            - **node** - :class:`~sphere_iot.uv_node.SphereNode`.
+            - **node** - :class:`~sphere_iot.uv_node.Node`.
             - **scale** - ``Vector3`` for scaling the node.
             - **circle_scale** - ``Vector3`` for scaling the outside circle.
             - **default_img_id** - id of the default image
             - **selected_img** - id of the image when the item is _selected.
             - **hover_img_id** - id of the image when the item is hovered with the mouse pointer.
             - **default_background_color** - ``Vector4``
             - **selected_background_color** - ``Vector4``
             - **hover_background_color** - ``Vector4``
             - **current_background_color** - ``Vector4``
 
         """
-        self.node = node
-        super().__init__(self.node)
 
-        # this is used to determine how close an edge can get to the disc
-        self.node_disc_radius = 0.08
+        super().__init__(node)
 
     def init_assets(self):
         """
         initializing the graphic assets. Can be partially or fully overridden.
 
         """
-        self.scale = [3.0, 3.0, 3.0]
-        self.circle_scale = [0.41, 0.44, 0.41]
-
-        img_id = self.node.config.get_img_id("question_mark_icon")
-        self.default_img_id = img_id
-        self.selected_img = img_id
-        self.hover_img_id = img_id
+        self.scale = [.5, .5, .5]
+        self.circle_scale = [0.05, 0.05, 0.05]
+        self.default_img_id = 4
+        self.selected_img_id = 2
+        self.hover_img_id = 2
         self.main_image_color = [1.0, 1.0, 1.0, 1.0]  # black image
 
-        self.default_background_color = [0.0, 0.07, 0.4, 0.1]
-        self.selected_background_color = [0.0, 0.07, 0.4, 0.1]  # [0.89, 0.15, 0.21, 0.1]
-        self.hover_background_color = [0.0, 0.07, 0.4, 0.1]
+        self.default_background_color = [0.0, 0.0, 0.0, 1.0]
+        self.selected_background_color = [0.9, 0.0, 0.0, 0.9]  # [0.89, 0.15, 0.21, 0.1]
+        self.hover_background_color = [0.9, 0.0, 0.0, 0.9]
 
-        self.default_border_color = [0.0, 0.0, 1.0, 0.3]
+        self.default_border_color = [0.0, 0.07, 0.4, 0.0]
         self.selected_border_color = [0.9, 0.0, 0.0, 0.4]
         self.hover_border_color = [0.9, 0.0, 0.0, 0.4]
 
         self.default_border_width = 1
         self.selected_border_width = 2
         self.hover_border_width = 3
 
         self.current_img_id = self.default_img_id
         self.current_background_color = self.default_background_color
         self.current_border_color = self.default_border_color
         self.current_border_width = self.default_border_width
 
         self.last_img_id = self.default_img_id
-
-
-
-
-
```

### Comparing `sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_graphic_socket.py` & `sphere_base-0.1.0/sphere_base/node/graphic_node.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,75 @@
 # -*- coding: utf-8 -*-
 
 """
-Module Graphic Socket. The graphics socket initializes the graphic assets for the sockets
+Module Graphic Node. The graphics node is used in all nodes and sockets.
 
 """
 
-from sphere_base.sphere_universe_base.suv_graphic_disc import EditorGraphicDisc
+from sphere_base.node.graphic_disc import GraphicDisc
 
 
-class GraphicSocket(EditorGraphicDisc):
+class GraphicNode(GraphicDisc):
     def __init__(self, node):
         """
-        Constructor of the ``Graphic Socket`` class. Contains graphic elements.
+        Constructor of the ``Editor Graphic Node`` class. Contains graphic elements.
 
-        :param node: reference to any inherited class of :class:`~sphere_iot.uv_node.SphereNode`.
-        :type node:  :class:`~sphere_iot.uv_node.SphereNode`
+        :param node: reference to any inherited class of :class:`~sphere_iot.uv_node.Node`.
+        :type node:  :class:`~sphere_iot.uv_node.Node`
 
         :Instance Variables:
 
-            - **node** - :class:`~sphere_iot.uv_node.SphereNode`.
+            - **node** - :class:`~sphere_iot.uv_node.Node`.
             - **scale** - ``Vector3`` for scaling the node.
             - **circle_scale** - ``Vector3`` for scaling the outside circle.
             - **default_img_id** - id of the default image
             - **selected_img** - id of the image when the item is _selected.
             - **hover_img_id** - id of the image when the item is hovered with the mouse pointer.
             - **default_background_color** - ``Vector4``
             - **selected_background_color** - ``Vector4``
             - **hover_background_color** - ``Vector4``
             - **current_background_color** - ``Vector4``
 
         """
+        self.node = node
+        super().__init__(self.node)
 
-        super().__init__(node)
+        # this is used to determine how close an edge can get to the disc
+        self.node_disc_radius = 0.08
 
     def init_assets(self):
         """
         initializing the graphic assets. Can be partially or fully overridden.
 
         """
-        self.scale = [.5, .5, .5]
-        self.circle_scale = [0.05, 0.05, 0.05]
-        self.default_img_id = 4
-        self.selected_img_id = 2
-        self.hover_img_id = 2
+        self.scale = [3.0, 3.0, 3.0]
+        self.circle_scale = [0.41, 0.44, 0.41]
+
+        img_id = self.node.config.get_img_id("icon_question_mark")
+        self.default_img_id = img_id
+        self.selected_img = img_id
+        self.hover_img_id = img_id
         self.main_image_color = [1.0, 1.0, 1.0, 1.0]  # black image
 
-        self.default_background_color = [0.0, 0.0, 0.0, 1.0]
-        self.selected_background_color = [0.9, 0.0, 0.0, 0.9]  # [0.89, 0.15, 0.21, 0.1]
-        self.hover_background_color = [0.9, 0.0, 0.0, 0.9]
+        self.default_background_color = [0.0, 0.07, 0.4, 0.1]
+        self.selected_background_color = [0.0, 0.07, 0.4, 0.1]  # [0.89, 0.15, 0.21, 0.1]
+        self.hover_background_color = [0.0, 0.07, 0.4, 0.1]
 
-        self.default_border_color = [0.0, 0.07, 0.4, 0.0]
+        self.default_border_color = [0.0, 0.0, 1.0, 0.3]
         self.selected_border_color = [0.9, 0.0, 0.0, 0.4]
         self.hover_border_color = [0.9, 0.0, 0.0, 0.4]
 
         self.default_border_width = 1
         self.selected_border_width = 2
         self.hover_border_width = 3
 
         self.current_img_id = self.default_img_id
         self.current_background_color = self.default_background_color
         self.current_border_color = self.default_border_color
         self.current_border_width = self.default_border_width
 
         self.last_img_id = self.default_img_id
+
+
+
+
+
```

### Comparing `sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_history.py` & `sphere_base-0.1.0/sphere_base/history.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 
 """
-A module containing all code for working with history on a single sphere_base (Undo/Redo)
+A module containing all the code for working with history on a single sphere (Undo/Redo)
 """
 
-from sphere_base.sphere_universe_base.suv_utils import dump_exception
+from sphere_base.utils import dump_exception
 
-DEBUG = False
-DEBUG_SELECTION = False
+DEBUG_STORE = False
+DEBUG_RESTORE = False
 
 
 class History:
     """ Class contains all the code for undo/redo operations on a single sphere_base """
 
     def __init__(self, sphere: 'Sphere'):
         """
@@ -33,203 +33,217 @@
             - **hover_background_color** - ``list``
             - **current_background_color** - ``list``
 
         """
 
         self.sphere = sphere
 
-        self.clear()
-
         # history limit pere Sphere
         self.history_limit = 32
 
         self.undo_selection_has_changed = False
 
         # listeners
         self._history_modified_listeners = []
         self._history_stored_listeners = []
         self._history_restored_listeners = []
+        self.history_stack = []
+
+        self.history_current_step = -1
 
     def clear(self):
         """
         Reset the history stack
-
         """
         self.history_stack = []
         self.history_current_step = -1
 
     def store_initial_history_stamp(self):
         """
         Helper function usually used when new or open file requested
-
         """
+        self.clear()
         self.store_history("Initial history stamp")
 
     def add_history_modified_listener(self, callback: 'function'):
         """
         Register callback for 'history modified' event.
-
         :param callback: callback function
-
         """
         self._history_modified_listeners.append(callback)
 
     def add_history_stored_listener(self, callback):
         """
         Register callback for 'history stored' event.
-
         :param callback: callback function
-
         """
         self._history_stored_listeners.append(callback)
 
     def add_history_restored_listener(self, callback: 'function'):
         """
         Register callback for 'history restored' event.
-
         :param callback: callback function
-
         """
         self._history_restored_listeners.append(callback)
 
     def can_undo(self) -> bool:
         """
         True if possible to un-do history.
-
         :returns: ``bool``
-
         """
         return self.history_current_step > 0
 
     def can_redo(self) -> bool:
         """
         True if possible to un-do history.
-
         :returns: ``bool``
-
         """
         return self.history_current_step + 1 < len(self.history_stack)
 
     def undo(self):
         """
         Undo operation
-
         """
-        if DEBUG:
+        if DEBUG_RESTORE:
             print("UNDO")
 
         if self.can_undo():
             self.history_current_step -= 1
             self.restore_history()
             self.sphere.has_been_modified = True
 
     def redo(self):
         """
         Redo operation
 
         """
-        if DEBUG:
+        if DEBUG_STORE:
             print("REDO")
         if self.can_redo():
             self.history_current_step += 1
             self.restore_history()
             self.sphere.has_been_modified = True
 
-    def restore_history(self):
-        """
-        Restore `History Stamp` from `History stack`
-
-        """
-        if DEBUG:
-            print("Restoring history",
-                  ".... current_step: @%d" % self.history_current_step,
-                  "(%d)" % len(self.history_stack))
-
-        self.restore_history_stamp(self.history_stack[self.history_current_step])
-        for callback in self._history_modified_listeners: callback()
-        for callback in self._history_restored_listeners: callback()
-
     def store_history(self, description: str, set_modified: bool = False):
         """
         Store History Stamp into History Stack. Set modified flag if set_modified is True
 
         :param description: description
         :type description: ``str``
         :param set_modified: set modified flag
         :type set_modified: ``bool``
 
         """
 
         if set_modified:
             self.sphere.has_been_modified = True
 
-        if DEBUG: print("Storing history", '"%s"' % description,
-                        ".... current_step: @%d" % self.history_current_step,
-                        "(%d)" % len(self.history_stack))
+        if DEBUG_STORE:
+            print("\n .....................Storing history....................")
+            print("Storing history", '"%s"' % description,
+                  ".... current_step: @%d" % self.history_current_step,
+                  "(%d)" % len(self.history_stack))
 
         # if the pointer (history_current_step) is not at the end of history_stack
         if self.history_current_step + 1 < len(self.history_stack):
             self.history_stack = self.history_stack[0:self.history_current_step + 1]
 
         # history is outside of the limits
         if self.history_current_step + 1 >= self.history_limit:
             self.history_stack = self.history_stack[1:]
             self.history_current_step -= 1
 
-        hs = self.create_history_stamp(description)
+        history_stamp = self.create_history_stamp(description)
 
-        self.history_stack.append(hs)
+        self.history_stack.append(history_stamp)
         self.history_current_step += 1
-        if DEBUG: print("  -- setting step to:", self.history_current_step)
+
+        if DEBUG_STORE:
+            print("  -- setting step to:", self.history_current_step)
 
         # always trigger history modified (for i.e. update_edit_menu)
-        for callback in self._history_modified_listeners: callback()
-        for callback in self._history_stored_listeners: callback()
+        for callback in self._history_modified_listeners:
+            callback()
+        for callback in self._history_stored_listeners:
+            callback()
 
     def capture_current_selection(self) -> dict:
         """
         Create dictionary with list of _selected nodes and list of _selected edges
 
         """
 
+        if DEBUG_STORE:
+            print("  -- capturing current selection ")
+
         sel_obj = {
             'nodes': [],
             'edges': [],
         }
+
         for item in self.sphere.items_selected:
             if item.type == 'node':
                 sel_obj['nodes'].append(item.id)
-            elif item.type == 'node':
+            elif item.type == 'edge':
                 sel_obj['edges'].append(item.id)
+
+        if DEBUG_STORE:
+            print("  -- current selection: ", sel_obj)
         return sel_obj
 
     def create_history_stamp(self, description: str) -> dict:
         """
-        Create History Stamp. Internally serialize whole scene and current selection.
-
+        Create History Stamp. Internally serialize whole sphere and current selection.
+        :param description: Descriptive label for the History Stamp
+        :return: History stamp serializing state of `Sphere` and current selection
+        :rtype: ``dict``
         """
+        if DEBUG_STORE:
+            print("  -- create history time stamp")
         history_stamp = {
             'description': description,
             'snapshot': self.sphere.serialize(),
             'selection': self.capture_current_selection(),
         }
 
         return history_stamp
 
+    def restore_history(self):
+        """
+        Restore `History Stamp` from `History stack`
+
+        """
+        if DEBUG_RESTORE:
+            print("Restoring history",
+                  ".... current_step: @%d" % self.history_current_step,
+                  "(%d)" % len(self.history_stack))
+
+        self.restore_history_stamp(self.history_stack[self.history_current_step])
+        for callback in self._history_modified_listeners:
+            callback()
+        for callback in self._history_restored_listeners:
+            callback()
+
     def restore_history_stamp(self, history_stamp: dict):
         """
         Restore History Stamp to current `Scene` with selection of items included
 
+        :param history_stamp: History Stamp to restore
+        :type history_stamp: ``dict``
+
         """
-        if DEBUG: print("restore_history_stamp: ", history_stamp['description'])
+        if DEBUG_RESTORE:
+            print("restore_history_stamp: ", history_stamp['description'])
 
         try:
             self.undo_selection_has_changed = False
             previous_selection = self.capture_current_selection()
-            if DEBUG_SELECTION: print("_selected nodes before restore:", previous_selection['nodes'])
+            if DEBUG_RESTORE:
+                print("_selected nodes before restore:", previous_selection['nodes'])
+                print("_selected edges before restore:", previous_selection['edges'])
 
             self.sphere.deserialize(history_stamp['snapshot'])
 
             # restore selection
 
             # first clear all selection on all items
             for item in self.sphere.items_selected:
@@ -246,20 +260,23 @@
             for node_id in history_stamp['selection']['nodes']:
                 for item in self.sphere.items:
                     if item.id == node_id:
                         self.sphere.select_item(item, True)
                         break
 
             current_selection = self.capture_current_selection()
-            if DEBUG_SELECTION: print("_selected nodes after restore:", current_selection['nodes'])
+            if DEBUG_RESTORE:
+                print("_selected nodes after restore:", current_selection['nodes'])
+                print("_selected edges after restore:", current_selection['edges'])
 
             # reset the last_selected_items - since we're comparing change to the last_selected state
-            # self.sphere_base._last_selected_items = self.sphere_base.items_selected
+            self.sphere._last_selected_items = self.sphere.items_selected
 
             # if the selection of nodes differ before and after restoration, set flag
             if current_selection['nodes'] != previous_selection['nodes'] or current_selection['edges'] != \
                     previous_selection['edges']:
-                if DEBUG_SELECTION: print("\nSCENE: Selection has changed")
+                if DEBUG_RESTORE:
+                    print("\nSCENE: Selection has changed")
                 self.undo_selection_has_changed = True
 
         except Exception as e:
             dump_exception(e)
```

### Comparing `sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_mouse_ray.py` & `sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_mouse_ray.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,265 +1,214 @@
 # -*- coding: utf-8 -*-
 
 """
-This is the ``MouseRay`` module. This module is used for determining which object is clicked by the mouse pointer.
+This is the ``MouseRay`` module. This module is used for determining which object is on_current_row_changed
+by the mouse pointer.
 It uses the ``PyBullet`` library to shoot a ray into the ``PyBullet`` physics simulation
-which is a copy of the :class:`~sphere_iot.uv_universe.Universe` with all its ``Model`` objects. It returns the collision
-object the mouse ray hits.
+which is a copy of the :class:`~sphere_iot.uv_universe.Universe` with all its ``Model`` objects.
+It returns the collision object the mouse ray hits.
 
 This module also creates all collision objects in the ``PyBullet`` simulation world for all the models used in the
 :class:`~sphere_iot.uv_universe.Universe` implementation.
 
 """
 
 import pybullet as p
 from pyrr import Vector3, Vector4, vector, matrix44
-from sphere_base.sphere_universe_base.suv_constants import *
-from sphere_base.sphere_universe_base.suv_utils import dump_exception
+from sphere_base.constants import *
+from sphere_base.utils import dump_exception
 from pybullet_utils import bullet_client as bc
 
 DEBUG = False
 DEBUG_SHOW_GUI = False
+DEBUG_MOUSE_RAY = False
+
+COLLISION_SHAPES = {
+    "sphere_base": {"type": p.GEOM_SPHERE, "radius": SPHERE_RADIUS, "height": 0, "base_mass": 0,
+                    "baseVisualShapeIndex": -1},
+    "node": {"type": p.GEOM_SPHERE, "radius": NODE_DISC_RADIUS, "height": 0, "base_mass": 0,
+             "baseVisualShapeIndex": -1},
+    "socket": {"type": p.GEOM_CYLINDER, "radius": SOCKET_RADIUS, "height": 0, "base_mass": 0,
+               "baseVisualShapeIndex": -1},
+    "edge": {"type": p.GEOM_MESH, "height": .025, "base_mass": 0, "baseVisualShapeIndex": -1},
+    "sphere_small": {"type": p.GEOM_CYLINDER, "radius": SPHERE_SMALL_RADIUS, "height": .026, "base_mass": 0,
+                     "baseVisualShapeIndex": -1},
+          }
 
 
 class MouseRay:
     """
     This class maintains a parallel PyBullet physics reality of the :class:`~sphere_iot.uv_universe.Universe`.
     For this it creates, places and maintains collision object shapes for all models which can be hit
     by a ray emitted from the mouse pointer.
 
     """
 
-    def __init__(self, universe: 'Universe', pybullet_key=None):
+    def __init__(self, universe, pybullet_key=None):
 
         """
-        Constructor of the ``MousRay`` class.
+        Constructor of the ``MouseRay`` class.
 
         :param universe: The 'PyBullet' physics simulation is a copy of the :class:`~sphere_iot.uv_universe.Universe`
         :type universe:  :class:`~sphere_iot.uv_universe.Universe`
 
         :Instance Attributes:
 
             - **camera** - Instance of :class:`~sphere_iot.uv_cam.camera`
             - **uv** - Instance of :class:`~sphere_iot.uv_universe.Universe`
 
         """
 
-        # Uses pybullet to detect what the mouse is clicking on
-
         self.uv = universe
         self.cam = universe.cam
-        self._collision_objects = {}
-        self.pybullet_key = pybullet_key
-        self.client_id = 0
 
-        if DEBUG_SHOW_GUI:
-            p.connect(p.GUI)
-        elif pybullet_key:
-            try:
-
-                self.bullet = bc.BulletClient(connection_mode=p.DIRECT)
-                self.client_id = self.bullet._client
+        self.client_id = 0
+        self.pybullet_key = pybullet_key
+        self.abs_pos = [0.0, 0.0, 0.0]  # position of mouse ray collision point in world space
 
-            except:
-                dump_exception()
+        self._collision_objects = {}
+        self._collision_shapes = {}
 
-        else:
-            p.connect(p.DIRECT)
+        self._open_bullet_client(self.pybullet_key)
         self._create_collision_shapes()
 
-    def _create_collision_shapes(self):
-        """
-        Creates. collision shapes used for all models used in the implementation.
-
-        """
-        self.c_shape_sphere_small = self.bullet.createCollisionShape(p.GEOM_SPHERE, radius=SPHERE_SMALL_RADIUS)
-        self.c_shape_sphere = self.bullet.createCollisionShape(p.GEOM_SPHERE, radius=SPHERE_RADIUS)
-        self.c_shape_node_disc = self.bullet.createCollisionShape(p.GEOM_CYLINDER, radius=COLLISION_NODE_DISC_RADIUS, height=.025)
-        self.c_shape_socket = self.bullet.createCollisionShape(p.GEOM_CYLINDER, radius=COLLISION_SOCKET_RADIUS, height=.026)
-
-    def create_collision_object(self, item: ('Sphere', 'Node', 'Socket', 'Edge'), vertices: list = None):
-        """
-        Allocates the correct collision object.
-
-        :param item: Each item has a type.
-        :param item: Can be: :class:`~sphere_iot.uv_sphere.Sphere`, :class:`~sphere_iot.uv_node.SphereNode`, :class:`~sphere_iot.uv_socket.Socket`, :class:`~sphere_iot.uv_edge.SphereSurfaceEdge``
-        :param vertices: when lines are drawn, the vertices determine the collision shape
-        :param vertices: ``list``
-        """
-
-        if item.type == "sphere_base":
-            return self.create_sphere_collision_object(item)
-        if item.type == "node":
-            return self.create_node_collision_object(item)
-        if item.type == "socket":
-            return self.create_socket_collision_object(item)
-        if item.type == "edge":
-            return self.create_edge_element_collision_object(item, vertices)
-        if item.type == "sphere_small":
-            return self.create_sphere_small_collision_object(item)
-
-
-    def create_sphere_collision_object(self, sphere: 'Sphere'):
-        """
-        Creating the ``Sphere`` collision object
-
-        :param sphere: The model that the collision object belongs to.
-        :type sphere: :class:`~sphere_iot.uv_sphere.Sphere`
-
-        """
-        mass = 0
-        visual_shape_id = -1
-
-        object_id = self.bullet.createMultiBody(baseMass=mass,
-                                                baseCollisionShapeIndex=self.c_shape_sphere,
-                                                baseVisualShapeIndex=visual_shape_id,
-                                                basePosition=[sphere.xyz[0], sphere.xyz[1], sphere.xyz[2]],
-                                                baseOrientation=[0, 0, 0, 1],
-                                                physicsClientId=0)
-
-        self._collision_objects[object_id] = sphere.id
-        return object_id
-
-    def create_sphere_small_collision_object(self, sphere: 'Sphere'):
-        """
-        Creating the ``Sphere_small`` collision object
-
-        :param sphere: The model that the collision object belongs to.
-        :type sphere: :class:`~sphere_iot.uv_sphere.Sphere`
-
-        """
-
-        mass = 0
-        visual_shape_id = -1
+    def _open_bullet_client(self, pybullet_key):
+        try:
+            if DEBUG_SHOW_GUI:
 
-        object_id = self.bullet.createMultiBody(baseMass=mass,
-                                                baseCollisionShapeIndex=self.c_shape_sphere_small,
-                                                baseVisualShapeIndex=visual_shape_id,
-                                                basePosition=[sphere.xyz[0], sphere.xyz[1], sphere.xyz[2]],
-                                                baseOrientation=[0, 0, 0, 1],
-                                                physicsClientId=self.client_id)
+                self.bullet = bc.BulletClient(connection_mode=p.GUI)
+                self.client_id = self.bullet._client
 
-        self._collision_objects[object_id] = sphere.id
-        # print("creating small collision object", self.client_id, object_id)
-        return object_id
+            else:
 
-    def create_node_collision_object(self, node: 'Node'):
-        """
-        Creating the ``node`` collision object
+                self.bullet = bc.BulletClient(connection_mode=p.DIRECT)
+                self.client_id = self.bullet._client
 
-        :param Node: The model that the collision object belongs to.
-        :type Node: :class:`~sphere_iot.uv_node.SphereNode`
+        except Exception as e:
+            dump_exception(e)
+        else:
+            p.connect(p.DIRECT)
 
+    def _create_collision_shapes(self):
         """
+        Creates a dictionary with collision shapes used for all models used in the implementation.
 
-        mass = 0
-        visual_shape_id = -1
-
-        collision_object_id = self.bullet.createMultiBody(baseMass=mass,
-                                                          baseCollisionShapeIndex=self.c_shape_node_disc,
-                                                          baseVisualShapeIndex=visual_shape_id,
-                                                          basePosition=[node.xyz[0], node.xyz[1], node.xyz[2]],
-                                                          baseOrientation=node.orientation,
-                                                          physicsClientId=self.client_id)
-
-        self._collision_objects[collision_object_id] = node.id
-        if DEBUG and collision_object_id == 1:
-            self.debug_collision_object(collision_object_id, node)
-        return collision_object_id
-
-    def create_socket_collision_object(self, socket: 'Socket'):
         """
-        Creating the ``Socket`` collision object
-
-        :param socket: The model that the collision object belongs to.
-        :type socket: :class:`~sphere_iot.uv_socket.Socket`
 
-        """
-        mass = 0
-        visual_shape_id = -1
+        self._collision_shapes = {
+            'sphere_small': self.bullet.createCollisionShape(p.GEOM_SPHERE, radius=SPHERE_SMALL_RADIUS, height=0),
+            'sphere_base': self.bullet.createCollisionShape(p.GEOM_SPHERE, radius=SPHERE_RADIUS, height=0),
+            'node': self.bullet.createCollisionShape(p.GEOM_CYLINDER, radius=NODE_DISC_RADIUS, height=0.025),
+            'socket': self.bullet.createCollisionShape(p.GEOM_CYLINDER, radius=SOCKET_RADIUS, height=0.027),
 
-        collision_object_id = self.bullet.createMultiBody(baseMass=mass,
-                                                          baseCollisionShapeIndex=self.c_shape_socket,
-                                                          baseVisualShapeIndex=visual_shape_id,
-                                                          basePosition=[socket.xyz[0], socket.xyz[1], socket.xyz[2]],
-                                                          baseOrientation=socket.orientation,
-                                                          physicsClientId=self.client_id)
+        }
 
-        self._collision_objects[collision_object_id] = socket.id
-        if DEBUG and collision_object_id == 1:
-            self.debug_collision_object(collision_object_id, socket)
-        return collision_object_id
+    def get_collision_shape(self, obj):
+        shape_id = None
+        if obj.type.startswith('sphere'):
+            shape_id = self.bullet.createCollisionShape(p.GEOM_SPHERE, radius=obj.radius, height=0)
+        elif obj.type == 'node':
+            shape_id = self.bullet.createCollisionShape(p.GEOM_CYLINDER, radius=obj.radius, height=0.025)
+        elif obj.type == 'socket':
+            shape_id = self.bullet.createCollisionShape(p.GEOM_CYLINDER, radius=obj.radius, height=0.026)
+        return shape_id
 
-    def create_edge_element_collision_object(self, edge, vertices):
+    def create_collision_object(self, obj, vertices: list = None):
         """
-        Creating an ``Edge`` collision object
-
-        :param edge: The edge that this collision object belongs to.
-        :type edge: :class:`~sphere_iot.uv_surface_edge.SphereSurfaceEdge`
-        :param vertices: The vertices of this edge.
-        :type vertices: ``list``
+        Allocates the correct collision object.
 
+        :param obj: Each item has a type.
+        :param obj: Can be: :class:`~sphere_iot.uv_sphere.Sphere`, :class:`~sphere_iot.uv_node.Node`,
+        :class:`~sphere_iot.uv_socket.Socket`, :class:`~sphere_iot.uv_edge.SphereSurfaceEdge``
+        :param vertices: when lines are drawn, the vertices determine the collision shape
+        :param vertices: ``list``
         """
-        mass = 0
-        visual_shape_id = -1
-
-        if edge.collision_object_id:
-            self.bullet.removeBody(edge.collision_object_id)
+        cs = COLLISION_SHAPES
 
-        self.c_shape_edge_element = self.bullet.createCollisionShape(p.GEOM_MESH, vertices=vertices)
+        for key in cs.keys():
+            if key == obj.type:
 
-        collision_object_id = self.bullet.createMultiBody(baseMass=mass,
-                                                          baseCollisionShapeIndex=self.c_shape_edge_element,
-                                                          baseVisualShapeIndex=visual_shape_id,
-                                                          physicsClientId=self.client_id)
+                if key == "edge":
+                    collision_shape_id = self.bullet.createCollisionShape(p.GEOM_MESH, vertices=vertices,
+                                                                          flags=p.GEOM_FORCE_CONCAVE_TRIMESH)
+                    # print(obj.type, collision_shape_id)
+                    object_id = self.bullet.createMultiBody(baseMass=cs[key]["base_mass"],
+                                                            baseCollisionShapeIndex=collision_shape_id,
+                                                            baseVisualShapeIndex=cs[key]["baseVisualShapeIndex"],
+                                                            baseOrientation=obj.orientation,
+                                                            physicsClientId=self.client_id)
+                elif key == "sphere_base":
+                    object_id = self.bullet.createMultiBody(baseMass=cs[key]["base_mass"],
+                                                            baseCollisionShapeIndex=obj.collision_shape_id,
+                                                            baseVisualShapeIndex=cs[key]["baseVisualShapeIndex"],
+                                                            basePosition=[obj.xyz[0], obj.xyz[1], obj.xyz[2]],
+                                                            baseOrientation=obj.orientation,
+                                                            physicsClientId=self.client_id)
+                else:
+
+                    object_id = self.bullet.createMultiBody(baseMass=cs[key]["base_mass"],
+                                                            baseCollisionShapeIndex=self._collision_shapes[key],
+                                                            baseVisualShapeIndex=cs[key]["baseVisualShapeIndex"],
+                                                            basePosition=[obj.xyz[0], obj.xyz[1], obj.xyz[2]],
+                                                            baseOrientation=obj.orientation,
+                                                            physicsClientId=self.client_id)
 
-        self._collision_objects[collision_object_id] = edge.id
-        if DEBUG and collision_object_id == 1:
-            self.debug_collision_object(collision_object_id, edge)
-        return collision_object_id
+                self._collision_objects[object_id] = obj.id
+                return object_id
 
-    def delete_collision_object(self, item: ('Sphere', 'Node', 'Socket', 'Edge')):
+    def delete_collision_object(self, item):
         """
         Delete the collision object of the item
 
         :param item: The model the collision object belongs to.
-        :param item: :class:`~sphere_iot.uv_sphere.Sphere`, :class:`~sphere_iot.uv_node.SphereNode`, :class:`~sphere_iot.uv_socket.Socket`, :class:`~sphere_iot.uv_edge.SphereSurfaceEdge`
+        :param item: :class:`~sphere_iot.uv_sphere.Sphere`, :class:`~sphere_iot.uv_node.Node`,
+        :class:`~sphere_iot.uv_socket.Socket`, :class:`~sphere_iot.uv_edge.SphereSurfaceEdge`
         """
         self.bullet.removeBody(item.collision_object_id, physicsClientId=self.client_id)
 
-    def reset_position_collision_object(self, item: ('Sphere', 'Node', 'Socket', 'Edge')):
+    def reset_position_collision_object(self, item, vertices=None):
         """
         Reset the collision object of the item
 
+        :param vertices: The vertices of the model.
         :param item: The model the collision object belongs to.
-        :param item: :class:`~sphere_iot.uv_sphere.Sphere`, :class:`~sphere_iot.uv_node.SphereNode`, :class:`~sphere_iot.uv_socket.Socket`, :class:`~sphere_iot.uv_edge.SphereSurfaceEdge`
+        :param item: :class:`~sphere_iot.uv_sphere.Sphere`, :class:`~sphere_iot.uv_node.Node`,
+        :class:`~sphere_iot.uv_socket.Socket`, :class:`~sphere_iot.uv_edge.SphereSurfaceEdge`
 
         .. warning::
 
             The build in 'reset method' of PyBullet does not not give the desired result. It did not work for me.
             The work around is to delete the current collision object and create a new one. This is likely
             more expensive.
 
             It is also executed quite often and more than is strictly needed. When the position
             of the model changes the position of the collision object is updated too. This might be changed in
             an update that only takes place when dragging stops or when a button is released.
 
         """
-        # TODO: resetting does not work correctly and we are using a work round of destroying
-        #  the current collision object and re-creating it
-        # This does not work correctly
-        # self.p0.resetBasePositionAndOrientation(bodyUniqueId=node_disc.collision_object_id,
-        #                                   posObj=[node_disc.xyz[0], node_disc.xyz[1], node_disc.xyz[2]],
-        #                                   ornObj=node_disc.orientation)
+        # TODO: resetting does not work correctly and we are using a workaround: destroying
+        #       the current collision object and re-creating it
+        #
 
-        # this seems to work....
+        try:
+            # This does not work:
+            # self.bullet.resetBasePositionAndOrientation(bodyUniqueId=item.collision_object_id,
+            #                                   posObj=[item.xyz[0], item.xyz[1], item.xyz[2]],
+            #                                   ornObj=item.orientation,
+            #                                   physicsClientId=self.client_id)
+
+            # the below works for now.... But I imagine it will to have too much overhead. Instead of moving an
+            # object we are destroying and then recreating it.
+
+            if item.collision_object_id:
+                self.bullet.removeBody(item.collision_object_id, physicsClientId=self.client_id)
+            self.create_collision_object(item, vertices)
 
-        self.bullet.removeBody(item.collision_object_id, physicsClientId=self.client_id)
-        self.create_collision_object(item)
+        except Exception as e:
+            dump_exception(e)
 
         if DEBUG and item.collision_object_id == 1:
             self.debug_collision_object(item.collision_object_id, item)
 
         return item.id, item.xyz
 
     def check_mouse_ray(self, mouse_x: float, mouse_y: float) -> (int, list):
@@ -270,29 +219,32 @@
         :type mouse_x: ``float``
         :param mouse_y: mouse y position
         :type mouse_y: ``float``
         :returns: id of the collision object id and its position
         """
         ray_world = self.get_mouse_point(mouse_x, mouse_y)
 
-        point_at = self.bullet.rayTest(self.cam.xyz, self.cam.xyz + (ray_world * 100), physicsClientId=self.client_id)
-        object_id = point_at[0][0]
-        # print(object_id)
+        intersection = self.bullet.rayTest(self.cam.xyz, self.cam.xyz + (ray_world * 100),
+                                           physicsClientId=self.client_id)
+        object_id = intersection[0][0]
 
         try:
             if object_id >= 0:
-                return self._collision_objects[object_id], point_at[0][3]
+                if DEBUG_MOUSE_RAY:
+                    self.debug_mouse_ray(intersection)
+                self.abs_pos = intersection[0][3]
+                return self._collision_objects[object_id], self.abs_pos
             else:
                 return None, None
         except Exception as e:
-            print(mouse_x, mouse_y, point_at)
+            print(mouse_x, mouse_y, intersection)
             dump_exception(e)
             return None, None
 
-    def check_mouse_ray_batch(self, sphere: 'Sphere', ray_array_start: 'Vector3', ray_array_end: 'Vector3') -> list:
+    def check_mouse_ray_batch(self, sphere, ray_array_start: 'Vector3', ray_array_end: 'Vector3') -> list:
         """
         Returns a ``list`` of object id`s of the collision objects in the path of the mouse ray.
 
         :param sphere:
         :type sphere: :class:`~sphere_iot.uv_sphere.Sphere`
         :param ray_array_start: The mouse ray starting point
         :type ray_array_start: ``Vector3``
@@ -364,22 +316,33 @@
         """
         Resetting the physics simulation and recreating all collision shapes
 
         """
         self.bullet.resetSimulation(physicsClientId=self.client_id)
         self._create_collision_shapes()
 
-    def debug_collision_object(self, collision_object_id: int, item: ('Sphere', 'Node', 'Socket', 'Edge')):
+    def debug_collision_object(self, collision_object_id: int, item):
         """
         Method used for debugging.
 
         :param collision_object_id: ìd of the collision object
         :param collision_object_id: ``int``
-        :type item: :class:`~sphere_iot.uv_sphere.Sphere`, :class:`~sphere_iot.uv_node.SphereNode`, :class:`~sphere_iot.uv_socket.Socket, :class:`~sphere_iot.uv_edge.SphereSurfaceEdge``
+        :type item: :class:`~sphere_iot.uv_sphere.Sphere`, :class:`~sphere_iot.uv_node.Node`,
+        :class:`~sphere_iot.uv_socket.Socket, :class:`~sphere_iot.uv_edge.SphereSurfaceEdge``
 
         :return:
         """
         print("\n---------------------------")
         print("Node id and collision object id  :             ", item.id, collision_object_id)
         print("Node id and position and rotation :            ", item.xyz, item.orientation)
-        print("Collision object id, position and rotation :   ", self.bullet.getBasePositionAndOrientation(collision_object_id, physicsClientId=self.client_id))
-        print("Collision shape data :                          ", self.bullet.getCollisionShapeData(collision_object_id, -1, physicsClientId=self.client_id))
+        print("Collision object id, position and rotation :   ",
+              self.bullet.getBasePositionAndOrientation(collision_object_id, physicsClientId=self.client_id))
+        print("Collision shape data :                          ",
+              self.bullet.getCollisionShapeData(collision_object_id, -1, physicsClientId=self.client_id))
+
+    def debug_mouse_ray(self, intersection):
+        print("objectUniqueId:", intersection[0][0])
+        print("global collision object id:", self._collision_objects[intersection[0][0]])
+        print("linkIndex:", intersection[0][1])
+        print("hit fraction:", intersection[0][2])
+        print("hit position:", intersection[0][3])
+        print("hit normal:", intersection[0][4])
```

### Comparing `sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_node.py` & `sphere_base-0.1.0/sphere_base/node/node.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 # -*- coding: utf-8 -*-
 
 """
-Module Node. A node is the basis for all nodes. Further nodes are derived from SphereNode
+Module Node. A node is the basis for all nodes. Further nodes are derived from Node
 """
 
-from pyrr import quaternion
-from sphere_base.sphere_universe_base.suv_serializable import Serializable
+from pyrr import quaternion, Vector3, Quaternion
+from sphere_base.serializable import Serializable
 from collections import OrderedDict
-from sphere_base.sphere_universe_base.suv_graphic_node import GraphicNode
-from sphere_base.sphere_universe_base.suv_socket import Socket
-from sphere_base.sphere_universe_base.suv_constants import *
-# from sphere_iot.uv_calc import UvCalc
+from sphere_base.node.graphic_node import GraphicNode
+from sphere_base.node.socket import Socket
+from sphere_base.constants import *
+from sphere_base.utils import dump_exception
 import numpy as np
+import math
 
 
-class SphereNode(Serializable):
+class Node(Serializable):
     """
     Class representing a ``Node`` on a ``Sphere``. Each node can represent a person, an object or any entity.
     ``Sphere Nodes`` are sphere_base items like ``Sphere Edges`` and ``Sphere Sockets``.
     """
 
     GraphicNode_class = GraphicNode
     NodeContent_class = None
     Socket_class = Socket
 
-    def __init__(self, target_sphere: 'sphere_base', orientation_offset: 'quaternion' = None, node_type: str = "node"):
+    def __init__(self, target_sphere: 'sphere', orientation_offset: 'quaternion' = None,
+                 yaw_degrees=0, pitch_degrees=0, node_type: str = "node"):
         """
-        Constructor of the ``Node`` class. Creates a node and calculates where to place it on the sphere_base. Needs to be
-        overridden in the implementation to allow for other type of nodes.
+        Constructor of the ``Node`` class. Creates a node and calculates where to place it on the sphere_base.
+        Needs to be overridden in the implementation to allow for other type of nodes.
 
         :param target_sphere: The :class:`~sphere_iot.uv_sphere.Sphere` the ``node`` is on.
         :type target_sphere:  :class:`~sphere_iot.uv_sphere.Sphere`
-        :param orientation_offset: Quaternion representing the offset angle with the 0 position of the ``sphere_base``
+        :param orientation_offset: Quaternion representing the offset angle with the 0 position of
+         the ``sphere_base``
         :type orientation_offset: ``Quaternion``
         :param node_type: The type of the node to create
         :type node_type: ``str``
 
         :Instance Attributes:
 
             - **sphere_base** - Instance of :class:`~sphere_iot.uv_sphere.Sphere`
@@ -48,70 +51,69 @@
             - **shader** - Instance of :class:`~sphere_iot.shader.uv_node_shader.NodeShader`
 
         :Instance Variables:
 
             - **radius** - radius of the sphere_base this node is on.
             - **collision_object_id** - id of the collision cylinder pointing out.
             - **collision_object_radius** - radius of the node disc for pybullet collision object.
-            - **pos_orientation_offset** - quaternion position of the node relative to the zero rotation of the sphere_base.
-            - **orientation** - quaternion with the orientation of the disc pointing away from the center of the sphere_base.
+            - **pos_orientation_offset** - quaternion position of the node relative to the zero rotation of the
+              sphere_base.
+            - **orientation** - quaternion with the orientation of the disc pointing away from the center of the
+              sphere_base.
             - **scale** - scaling the node with the gr_node.scale value.
             - **texture_id** - ``int`` id of the current texture, image or icon applied to the node disc.
             - **serialized_detail_scene** - contains the ``json`` data of the detail node editor for this node.
             - **xyz** - ``Vector`` location of the ``node``.
 
         """
 
         super().__init__(node_type)
+
         self.node_type_name = "node"
         self.sphere = target_sphere
         self.config = self.sphere.config
         self.calc = self.sphere.calc
         self.node_disc = self.sphere.uv.models.get_model('node')
         self.circle = self.sphere.uv.models.get_model('circle')
+        self.ray = self.sphere.uv.mouse_ray
 
-        self.Socket = self.__class__.Socket_class  # initiate later
-
-        self._init_inner_classes()
-        self._init_variables()
-        self._init_flags()
-
-        self.collision_object_radius = COLLISION_NODE_DISC_RADIUS
-
-        # radius of the node to the center of the sphere_base. node can hover above surface of sphere_base
-        self.radius = target_sphere.radius - 0.01
-
-        # position_orientation (angle) of the node on the sphere_base relative to the zero rotation of the sphere_base
+        # (angle) of the node on the sphere_base relative to the zero rotation of the sphere_base
         self.pos_orientation_offset = np.array(
             [0.1, 0.1, 0.1, 1.0]) if orientation_offset is None else orientation_offset
+        self.yaw_degrees = yaw_degrees
+        self.pitch_degrees = pitch_degrees
 
-        # cumulative sphere_base rotation with position offset of node
-        cumulative_orientation = self.get_cumulative_rotation()
-        self.xyz = self.calc.move_to_position(cumulative_orientation, self.sphere, self.radius)
+        self.orientation = None
+        self.offset_with_collision_point = None  # difference center node with collision point
+        self.mouse_ray_collision_point = None
+        self.grNode = None
+        self.serialized_detail_scene = None
+        self._node_moved = False
+        self.xyz = None
+        self.collision_object_radius = NODE_DISC_RADIUS
 
+        self.Socket = self.__class__.Socket_class  # initiate later
+
+        self._init_inner_classes()
+        self.scale = self.gr_node.scale
+        self.texture_id = self.gr_node.default_img_id
+        self.radius = target_sphere.radius
+
+        self.xyz = self.get_position()  # the xyz position of the node on the surface of the sphere
         # get the orientation of the disc pointing away from the center of the sphere_base
-        self.orientation = self.calc.get_item_direction_pointing_outwards(self, self.sphere)
+        self.orientation = self.get_orientation()  # the normal for the node
+        self.cumulative_rotation = self.get_cumulative_rotation(self.pos_orientation_offset, self.sphere.orientation)
 
         # create a collision object (cylinder) pointing out
-        self.collision_object_id = self.sphere.uv.mouse_ray.create_collision_object(self)
+        self.collision_object_id = self.ray.create_collision_object(self)
         self.socket = self.Socket(self)
 
         self.sphere.add_item(self)
         self.sphere.add_item(self.socket)
 
-    def _init_variables(self):
-        self.scale = self.gr_node.scale
-        self.texture_id = self.gr_node.default_img_id
-        self.orientation = None
-
-        self.serialized_detail_scene = None
-
-    def _init_flags(self):
-        self._node_moved = False
-
     def _init_inner_classes(self):
         """
         Sets up graphic node and content class
         """
         node_content_class = self.get_node_content_class()
         graphics_node_class = self.get_graphic_node_class()
         if node_content_class:
@@ -127,73 +129,110 @@
 
     def get_graphic_node_class(self):
         """
         Helper function returns class representing GraphicNode.
         """
         return self.__class__.GraphicNode_class
 
-    def get_cumulative_rotation(self):
+    @staticmethod
+    def get_cumulative_rotation(angle1, angle2):
         """
-        Helper function returns a quaternion with a cumulative rotation of both the rotation
-        offset of the node with the rotation of the sphere_base.
+        Helper function returns a quaternion with a cumulative rotation of two rotations
+
         """
 
-        return quaternion.cross(self.pos_orientation_offset, quaternion.inverse(self.sphere.orientation))
+        return quaternion.cross(angle1, quaternion.inverse(angle2))
 
     def is_dragging(self, value: bool = False):
         """
         Returns the status of the _node_moved flag
         :return: ``bool``
         """
         if self._node_moved == value:
             # keep doing what you are doing
             return value
         elif self._node_moved and not value:
             # end dragging
             self._node_moved = False
-            self.sphere.history.store_history("node moved", True)
+            self.offset_with_collision_point = None
+            self.mouse_ray_collision_point = None
         elif not self._node_moved and value:
             # start dragging
             self._node_moved = True
         return self._node_moved
 
-    def drag_to(self, pitch_degrees, roll_degrees):
+    def drag_to(self, mouse_ray_collision_point=None):
         """
         Dragging the node_disc over the surface of the sphere_base
 
-        :param pitch_degrees: vertical degrees over the x as (while roll degrees is 0) in euler degrees
-        :type pitch_degrees: ``float``
-        :param roll_degrees: horizontal degrees following the equator in euler degrees
-        :type roll_degrees: ``float``
+        The difference between the mouse_ray collision point and the center of the disc is stored at the start of
+        the dragging. This difference is applied during the dragging and makes sure that the distance between the
+        collision point and the disc remains the same. This is very important when dragging groups of objects. Not
+        using this would mean that all objects would collect under the mouse pointer.
+
+        :param mouse_ray_collision_point: collision point of the mouse_ray with the target sphere
+        :type mouse_ray_collision_point: ``float``
 
         """
+        q = quaternion
+        try:
 
-        # get the new position orientation offset angle based on pitch and roll
-        self.pos_orientation_offset = self.calc.get_pos_orientation_offset(pitch_degrees, roll_degrees,
-                                                                           self.pos_orientation_offset)
-        self.update_position()
+            # first find the angle of the collision point
+            cp = self.calc.find_angle(mouse_ray_collision_point, self.sphere.orientation)
+
+            # print(mouse_ray_collision_point, self.sphere.orientation)
+            if self.offset_with_collision_point is None:
+
+                # store the difference between the node center and the collision point
+                self.offset_with_collision_point = q.cross(self.pos_orientation_offset, q.inverse(cp))
+
+            # Move the node center to the position of the collision point
+            self.pos_orientation_offset = cp
+
+            # correct the position of the node with the stored difference with the mouse pointer
+            self.pos_orientation_offset = q.cross(self.offset_with_collision_point, self.pos_orientation_offset)
+
+            self.update_position()
+            return self.pos_orientation_offset
+
+        except Exception as e:
+            print('collision_point', cp)
+            print('pos_orientation_offset', self.pos_orientation_offset)
+            print('offset_with_collision_point', self.offset_with_collision_point)
+            dump_exception(e)
+
+    def get_position(self):
+        # cumulative sphere_base rotation with position offset of node
+        cumulative_orientation = self.get_cumulative_rotation(self.pos_orientation_offset, self.sphere.orientation)
+
+        # get the position of the node on the sphere
+        xyz = self.calc.move_to_position(cumulative_orientation, self.sphere)
+
+        return xyz
+
+    def get_orientation(self):
+        # get the orientation of the disc pointing away from the center of the sphere_base
+        normal = self.calc.get_item_direction_pointing_outwards(self, self.sphere)
+        return normal
 
     def update_position(self):
         """
         update the position of the node_disc on the sphere_base. Calculate the position and the direction.
-        also update the position of the collision object for use with the mouse pointer ray.
         """
-        # update the position of the node_disc on the sphere_base
-        cumulative_orientation = self.get_cumulative_rotation()
 
-        # get the position of the node on the sphere_base
-        self.xyz = self.calc.move_to_position(cumulative_orientation, self.sphere, self.radius)
+        self.xyz = self.get_position()
+        self.orientation = self.get_orientation()
+        self.socket.update_position()
 
-        # get the orientation of the disc pointing away from the center of the sphere_base
-        self.orientation = self.calc.get_item_direction_pointing_outwards(self, self.sphere)
+        return self.xyz
 
+    def update_collision_object(self):
         # set the collision object for mouse pointer ray collision
-        self.sphere.uv.mouse_ray.reset_position_collision_object(self)
-
-        self.socket.update_position()
+        self.ray.reset_position_collision_object(self)
+        self.socket.update_collision_object()
 
     def update_content(self, texture_id: int, sphere_id: int):
         """
         Updates the content like icons and images
 
         :param texture_id: new texture, image or icon
         :type texture_id: ``int``
@@ -238,15 +277,15 @@
         self.sphere.remove_item(self)
 
     def draw(self):
         """
         Renders all the icons and circles of the node_disc.
         """
         self.socket.draw()
-        self.node_disc.draw(self, self.texture_id, self.gr_node.main_image_color, switch=0)
+        self.node_disc.draw(self, texture_id=self.texture_id, color=self.gr_node.main_image_color, switch=0)
         self.node_disc.draw(self, color=self.gr_node.current_background_color, switch=2)
 
         self.circle.shader.line_width = self.gr_node.current_border_width
         self.circle.draw(self, scale=self.gr_node.circle_scale, color=self.gr_node.current_border_color)
 
     def serialize(self):
         socket = self.socket.serialize()
@@ -258,24 +297,26 @@
             ('orientation_offset', self.pos_orientation_offset.tolist()),
             ('scene', self.serialized_detail_scene),
             ('socket_id', self.socket.id),
             ('socket', socket)
 
         ])
 
-    def deserialize(self, data: dict, hashmap: dict = {}, restore_id: bool = True) -> bool:
+    def deserialize(self, data: dict, hashmap: dict = None, restore_id: bool = True) -> bool:
         """
-        copy, cut paste also uses this. When pasting rtore id is false and new id's are created.
+        copy, cut paste also uses this. When pasting restore_id is false and new id's are created.
         """
+
+        # hashmap = {} if hashmap is None else hashmap
+
         if restore_id:
             self.id = data['id']
             self.socket.id = data['socket_id']
 
         self.node_type_name = data['node_type_name']
         self.pos_orientation_offset = np.array(data['orientation_offset'])
         self.serialized_detail_scene = data['scene']
         self.texture_id = data['texture_id']
         self.update_position()
+        self.update_collision_object()
 
         return True
-
-
```

### Comparing `sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_rubber_band.py` & `sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_rubber_band.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 
 """
 Module rubber band. The rubber band module contains the rubber band class. It is responsible
 for drawing a square selection box. Selecting all the items within the box.
 """
 
 from sphere_base.sphere_universe_base.suv_graphic_item import GraphicItem
-from pyrr import Vector4
 
-RAY_SEED = 20  # 10 creates 10 x 10 = 100 rays, x creates x**2 rays
+RAY_SEED = 13  # 10 creates 10 x 10 = 100 rays, x creates x**2 rays
 
 
 class RubberBand(GraphicItem):
     """
     This class represents a rubber band box used for selecting objects on a sphere_base.
     """
 
@@ -48,22 +47,19 @@
         """
         super().__init__(self, 'rubber_band_box')
         self.uv = universe
 
         self.inner_square = self.uv.models.get_model('rubber_band')
         self.outer_border = self.uv.models.get_model('square')  # the border of the rubber band
 
-        self._init_variables()
-
-    def _init_variables(self):
         self.xyz = None
         self.scale = None
         self.texture_id = 0
 
-        self._dragging = False  # Flag is also set from outside the class
+        self._dragging = False
 
         self.orientation = [0., 0., 0., 1.]
         self.color = [0.0, 0.5, 0.7, 0.05]
         self.border_color = [0.0, 0.5, 0.7, 0.5]
         self.mouse_start_point = [0.0, 0.0]
         self.mouse_end_point = [0.0, 0.0]
 
@@ -87,16 +83,16 @@
     @dragging.setter
     def dragging(self, value: bool):
         if not self._dragging and value:
             self._dragging = value
 
     def drag(self, start: bool, mouse_x: float, mouse_y: float):
         """
-        Size dragging the rubber band box. Start equals ``True`` when starting a new ``rubber band box`` and the starting
-        edge position is the current mouse position (mouse_x, mouse_y).
+        Size dragging the rubber band box. Start equals ``True`` when starting a new ``rubber band box``
+        and the starting edge position is the current mouse position (mouse_x, mouse_y).
 
         ``Start`` is ``False`` means we are already dragging a ``rubber band box`` and we just keep dragging the
         mouse position indicates the position of the opposite corner of the box.
 
         This means that the start attribute determines the meaning of (mouse_x, mouse_y)
 
         :param start: ``True`` when starting a new box. The mouse position is then the starting edge position.
@@ -118,15 +114,14 @@
 
     def set_pos(self):
         """
         finding the center position of the rubber band box based on the size of the box and the
         starting point. The shader uses ``xyz`` as the center of the square and ``scale`` as the scaling factor
 
         """
-
         self.xyz, self.scale = self.get_position_and_scale()
 
     def get_position_and_scale(self) -> (list, list):
         """
         The size of the rubber band box is determined by the distance between the mouse pointer starting
         position and its current mouse position in a two dimensional plane.
 
@@ -142,14 +137,15 @@
 
         x = (start[0] + diff[0] * .5)
         y = (start[1] + diff[1] * .5)
         z = 0
         center_position = [x, y, z]
 
         scaling_factor = [diff[0], diff[1], diff[2]]
+
         return center_position, scaling_factor
 
     def get_selection(self) -> list:
         """
         send out a collection of rays through the rubber band box.
         First create an array of "ray starting points" then a second array with ray ending points
         check for unique collisions that are not spheres. Select those items and deselect all other objects.
@@ -161,20 +157,21 @@
         ray_array_start = []
         ray_array_end = []
         selection = None
 
         if self._dragging:
             step_x = ((self.mouse_end_point[0] - self.mouse_start_point[0]) / RAY_SEED)
             step_y = ((self.mouse_end_point[1] - self.mouse_start_point[1]) / RAY_SEED)
+
             for x in range(RAY_SEED):
                 for y in range(RAY_SEED):
                     ray_start = self.uv.cam.xyz
                     ray_world = self.uv.mouse_ray.get_mouse_point(self.mouse_start_point[0] + x * step_x,
                                                                   self.mouse_start_point[1] + y * step_y)
-                    ray_end = self.uv.cam.xyz + ray_world * 3
+                    ray_end = self.uv.cam.xyz + ray_world * 30
                     ray_array_start.append(ray_start)
                     ray_array_end.append(ray_end)
 
             selection = self.uv.mouse_ray.check_mouse_ray_batch(self.uv.target_sphere, ray_array_start, ray_array_end)
 
         self._dragging = False
```

### Comparing `sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_serializable.py` & `sphere_base-0.1.0/sphere_base/serializable.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 """
 A module containing Serializable "Interface". We pretend its an abstract class
 
 """
 
 from collections import OrderedDict
 
-class Serializable():
+
+class Serializable:
     def __init__(self, item_type=None):
         """
         Default constructor automatically creates data which are common to any serializable object.
         In our case we create ``self.id`` which we use in every object in NodeEditor.
         """
         self.id = id(self)
         self.type = item_type
@@ -22,23 +23,25 @@
         in memory or file.
 
         :return: data serialized in ``OrderedDict``
         :rtype: ``OrderedDict``
         """
         raise NotImplemented()
 
-    def deserialize(self, data:dict, hashmap:dict={}, restore_id:bool=True) -> bool:
+    def deserialize(self, data: dict, hashmap: dict = None, restore_id: bool = True) -> bool:
+        hashmap = hashmap if hashmap else {}
+        print(hashmap)
         """
         Deserialization method which take data in python ``dict`` format with helping `hashmap` containing
         references to existing entities.
 
         :param data: Dictionary containing serialized data
         :type data: ``dict``
         :param hashmap: Helper dictionary containing references (by id == key) to existing objects
         :type hashmap: ``dict``
         :param restore_id: True if we are creating new Sockets. False is useful when loading existing
             Sockets of which we want to keep the existing object's `id`.
         :type restore_id: bool
         :return: ``True`` if deserialization was successful, otherwise ``False``
         :rtype: ``bool``
         """
-        raise NotImplemented()
+        return NotImplemented
```

### Comparing `sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_skybox.py` & `sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_skybox.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,25 +14,26 @@
 
 """
 
 from sphere_base.sphere_universe_base.suv_graphic_item import GraphicItem
 from collections import namedtuple
 from PIL import Image
 from random import randint
+import os
 
 
 class Skybox(GraphicItem):
     Face_texture = namedtuple("faces", "id, face_name, img_type, width, height, path, file_and_path, img_data")
 
     """
     Class creating and maintaining the ``background`` ``Skybox``
     
     """
 
-    def __init__(self, universe=None, skybox_set_name=None, skybox_img_directory=None):
+    def __init__(self, universe=None):
         """
         Constructor of the Skybox class.
 
         :param universe: reference to the :class:`~sphere_iot.uv_universe.Universe`
         :type universe: :class:`~sphere_iot.uv_universe.Universe`
 
         :Instance Attributes:
@@ -64,61 +65,38 @@
         self.xyz = self.uv.cam.xyz
         self.cf = self.uv.config
 
         # We get the shader from the model
         self.shader = self.model.shader
 
         self._init_variables()
-        self._init_skybox_image_set(skybox_set_name)
-        self.create_skybox_faces()
 
     def _init_variables(self):
         self.scale = None
         self.index = 0
         self.faces = []
         self.orientation = [0, 0, 0]
         self.paint_skybox = True
 
-    def get_random_skybox(self):
-        """
-        Change the skybox with a new random set of images
-        """
-        self._get_random_set()
-        self.create_skybox_faces()
+    def get_skybox_set(self, skybox_name=None, skybox_id=None, random=False):
 
-    def _init_skybox_image_set(self, skybox_set_name=None):
-        if skybox_set_name:
-            self.skb_id = self.get_skybox_id(skybox_set_name)
-        else:
-            self.skb_id = self._get_random_set()
-
-    def _get_random_set(self) -> int:
-        """
-        Returns the id of a random image set of all skybox sets stored. This happens at the beginning of the program.
-        If you want to allow the user to randomly jump to a new set during the program the new set should be
-        compared with the old set to avoid duplication.
-
-        """
+        if skybox_id == 0:  # Do not use a skybox
+            self.skb_id = skybox_id
+        elif not skybox_name and not skybox_id and not random:
+            random = True  # select a random skybox
+        elif skybox_name:
+            lst = ['None' if not txt else os.path.basename(txt) for txt in self.uv.config.skybox_sets]
+            self.skb_id = lst.index(skybox_name)  # choose a skybox by its name
+        elif skybox_id:
+            self.skb_id = skybox_id  # choose a skybox by its index
 
-        return randint(1, len(self.cf.skybox_sets) - 1)
+        if random:
+            self.skb_id = randint(1, len(self.cf.skybox_sets) - 1)  # select a random skybox
 
-
-    def get_skybox_id(self, skybox_name) -> int:
-        """
-        returns the id of a skybox based on its name.
-
-        :param skybox_name: Name of the ``Skybox`` set
-        :type skybox_name: ``string``
-        :returns: id of the skybox image set
-
-        """
-
-        for i, skybox in enumerate(self.cf.skybox_sets):
-            if skybox_name == skybox:
-                return i
+        self.create_skybox_faces()
 
     def get_next_set(self):
         """
         Activate next Skybox set in the id sequence.
 
         """
         _id = self.skb_id
@@ -147,21 +125,18 @@
         self.paint_skybox = True if path else False
         return path + "/" if path else path
 
     def create_skybox_faces(self):
         """
         Gets the six faces of the Skybox from the image path and adds them to the faces array.
 
-        :param path: path where the 6 images for the current skybox are located.
-        :type path: ``str``
         """
         path = self.get_skybox_path()
 
         if path:
-
             self.faces = []
             face_order = ["right", "left", "top", "bottom", "back", "front"]
             for i, face in enumerate(face_order):
                 img = Image.open(path + face + ".png")
                 img_data = img.convert("RGBA").tobytes()
                 face = self.Face_texture(i, face, "png", img.width, img.height, path,
                                          path + face + ".png", img_data)
```

### Comparing `sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_socket.py` & `sphere_base-0.1.0/sphere_base/node/socket.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 """
 Module Socket. Each sphere_base node has exactly one socket.
 The position of the socket is always is always in the center of the node disc it belongs to
 """
 
 
-from sphere_base.sphere_universe_base.suv_serializable import Serializable
-from sphere_base.sphere_universe_base.suv_graphic_socket import GraphicSocket
-from sphere_base.sphere_universe_base.suv_calc import UvCalc
-from sphere_base.sphere_universe_base.suv_constants import *
+from sphere_base.serializable import Serializable
+from sphere_base.node.graphic_socket import GraphicSocket
+from sphere_base.calc import Calc
+from sphere_base.constants import *
 from collections import OrderedDict
 
 DEBUG = False
 DEBUG_REMOVE_WARNINGS = False
 
 
 class Socket(Serializable):
@@ -27,15 +27,15 @@
 
     def __init__(self, node):
         """
         Constructor of the node class. Creates a node and calculates where to place it on the sphere_base. Needs to be
         overridden in the implementation to allow for other type of nodes.
 
         :param node: The ``node`` the ``socket`` belongs to.
-        :type node:  :class:`~sphere_iot.uv_node.SphereNode`
+        :type node:  :class:`~sphere_iot.uv_node.Node`
 
 
         :Instance Attributes:
 
             - **gr_socket** - Instance of :class:`~sphere_iot.uv_graphic_socket.GraphicSocket`
             - **calc** - Instance of :class:`~sphere_iot.uv_calc.UvCalc`
             - **socket_disc** - Instance of :class:`~sphere_iot.uv_models.Model`
@@ -45,73 +45,80 @@
         :Instance Variables:
 
             - **radius** - radius of the sphere_base this node is on.
             - **collision_object_radius** - radius of the socket for pybullet collision object.
             - **collision_object_id** - id of the collision cylinder pointing out.
             - **xyz** - ``Vector`` location of the ``Socket``.
             - **pos_orientation_offset** - copy from quaternion position of the node.
-            - **orientation** - quaternion with the orientation of the disc pointing away from the center of the sphere_base.
+            - **orientation** - quaternion with the orientation of the disc pointing away from the center of
+              the sphere_base.
             - **scale** - scaling the node with the gr_socket.scale value.
             - **texture_id** - ``int`` id of the current texture, image or icon applied to the node disc.
 
         """
         super().__init__('socket')
         self.node = node
 
         self.socket_disc = self.node.sphere.uv.models.get_model('socket')
         self.circle = self.node.sphere.uv.models.get_model('circle')
 
         self.gr_socket = self.__class__.GraphicSocket_class(self.node)
-        self.calc = UvCalc()
+        self.calc = Calc()
 
-        self._init_variables()
-
-        # create a collision object (cylinder) pointing out from the center of the sphere_base
-        self.collision_object_id = self.create_collision_object()
-
-        self.update_position()
-
-    def _init_variables(self):
         self.scale = self.gr_socket.scale
         self.texture_id = self.gr_socket.default_img_id
 
         self.radius = self.node.radius + 0.001
         self.orientation = self.node.orientation
+        self.cumulative_rotation = self.node.cumulative_rotation
         self.xyz = self.node.xyz
         self.pos_orientation_offset = self.node.pos_orientation_offset
 
         self.edges = []
         self.serialized_detail_scene = None
 
-        self.collision_object_radius = COLLISION_SOCKET_RADIUS
+        self.collision_object_radius = SOCKET_RADIUS
+
+        # create a collision object (cylinder) pointing out from the center of the sphere_base
+        self.collision_shape_id = self.node.sphere.uv.mouse_ray.get_collision_shape(self)
+        self.collision_object_id = self.create_collision_object()
+
+        self.update_position()
 
     def create_collision_object(self) -> int:
         """
         Creating a``pybullet`` collision object in the form of a cylinder with the same size
         as the ``Socket``. The cylinder is pointing out from the center of the ``Sphere``.
         """
         return self.node.sphere.uv.mouse_ray.create_collision_object(self)
 
-    def delete_collision_object(self) -> int:
+    def delete_collision_object(self) -> None:
         """
         Deleting the ``pybullet`` collision object.
         """
         self.node.sphere.uv.mouse_ray.delete_collision_object(self)
 
+    def update_collision_object(self):
+        # set the collision object for mouse pointer ray collision
+        self.node.sphere.uv.mouse_ray.reset_position_collision_object(self)
+        # find connected edges
+        edges = self.node.sphere.get_edges(self)
+        for edge in edges:
+            edge.update_collision_object()
+
     def update_position(self):
         """
         Updating the position of the ``Socket``. The socket is always located in the center of the
         Node Disc. The collision object and the connected edges are also updated.
         """
-        cumulative_orientation = self.node.get_cumulative_rotation()
-        self.xyz = self.calc.move_to_position(cumulative_orientation, self.node.sphere, self.radius)
 
+        self.xyz = self.node.xyz
         self.orientation = self.node.orientation  # same orientation as the node disc
         self.pos_orientation_offset = self.node.pos_orientation_offset
-        self.node.sphere.uv.mouse_ray.reset_position_collision_object(self)
+
         self.update_connected_edges()
 
     def update_connected_edges(self):
         """
         Update the connected edges
         """
 
@@ -211,15 +218,14 @@
         # not needed - not used, is part of the node
         return OrderedDict([
             ('id', self.id),
             ('type', self.type),
             ('scene', self.serialized_detail_scene),
         ])
 
-    def deserialize(self, data, hashmap={}, restore_id=True):
+    def deserialize(self, data, hashmap=None, restore_id=True):
         # not needed - not used, is included in node
         if restore_id:
             self.id = data['id']
 
         self.serialized_detail_scene = data['scene']
         return True
-
```

### Comparing `sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_sphere.py` & `sphere_base-0.1.0/sphere_base/sphere/sphere.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 # -*- coding: utf-8 -*-
 
 """
-Module Sphere. Each sphere_base represents a scene object for ``sphere_base items``. these items include nodes, edges and sockets.
+Module Sphere. Each sphere_base represents a scene object for ``sphere_base items``. these items include nodes,
+edges and sockets.
 One sphere_base at the time can become the 'target sphere_base'.
 
 """
 
 from random import *
-from sphere_base.sphere_universe_base.suv_serializable import Serializable
-from sphere_base.sphere_universe_base.suv_utils import dump_exception
+from sphere_base.serializable import Serializable
+from sphere_base.utils import dump_exception
 from collections import OrderedDict
-from sphere_base.sphere_universe_base.suv_node import SphereNode
-from sphere_base.sphere_universe_base.suv_edge_drag import EdgeDrag
-from sphere_base.sphere_universe_base.suv_surface_edge import SphereSurfaceEdge
-from sphere_base.sphere_universe_base.suv_constants import *
-
-from sphere_base.sphere_universe_base.suv_history import History
-from pyrr import quaternion, Vector3
+from sphere_base.node.node import Node
+from sphere_base.edge.edge_drag import EdgeDrag
+from sphere_base.edge.surface_edge import SurfaceEdge
+from sphere_base.history import History
+from pyrr import quaternion
 from math import pi
-from sphere_base.sphere_universe_base.suv_calc import UvCalc
+from sphere_base.calc import Calc
+from sphere_base.constants import *
 import numpy as np
 import pyperclip
 import json
 
 # for testing purposes a number of nodes can be _selected
 NUMBER_OF_TEST_NODES = 0
 
 
 class Sphere(Serializable):
     """
     Class representing a ``Sphere`` in the IOT ``Universe``. Each sphere_base represents a related group of people and
     or items. These `items` can include persons, entities or objects. They can have a relationship between each other.
     """
 
-    Node_class = SphereNode
-    Edge_class = SphereSurfaceEdge
-    Calc_class = UvCalc
+    Node_class = Node
+    Edge_class = SurfaceEdge
+    Calc_class = Calc
     Edge_drag_class = EdgeDrag
     History_class = History
 
-    def __init__(self, universe: 'universe', position: list = None, texture_id: int = None, sphere_type='sphere_base'):
+    def __init__(self, universe, position: list = None, texture_id: int = None, sphere_type='sphere_base'):
         """
         Constructor of the sphere_base class.
 
         :param universe: reference to the :class:`~sphere_iot.uv_universe.Universe`
         :type universe: :class:`~sphere_iot.uv_universe.Universe`
         :param position: position of the sphere_base in universe
         :type position: ``list`` with x, y, z values
         :param texture_id: number indicating which texture to use for the sphere_base
         :type texture_id: int
 
         :Instance Attributes:
 
-            - **node** - Instance of :class:`~sphere_iot.uv_node.SphereNode`
+            - **node** - Instance of :class:`~sphere_iot.uv_node.Node`
             - **edge** - Instance of :class:`~sphere_iot.uv_edge.SphereSurfaceEdge`
             - **calc** - Instance of :class:`~sphere_iot.uv_calc.UvCalc`
             - **config** - Instance of :class:`~sphere_iot.uv_config.UvConfig`
             - **edge_drag** - Instance of :class:`~sphere_iot.uv_edge_drag.EdgeDrag`
             - **history** - Instance of :class:`~sphere_iot.uv_history.History`
             - **shader** - Instance of :class:`~sphere_iot.shader.uv_sphere_shader.SphereShader`
 
@@ -76,92 +76,71 @@
         """
 
         super().__init__(sphere_type)
         self.uv = universe
         self.texture_id = texture_id
         self.config = universe.config
 
-        self._init_flags()
-        self._init_variables()
-        self._init_listeners()
+        self._has_been_modified = False
+        self._dragging = False
+        self.selected = False
+
+        # The sphere rotates
+        self.rotation_degrees = 0
+
+        self.index = 0
+        self.radius = SPHERE_RADIUS
+        self.scale = [self.radius, self.radius, self.radius]
+        self.color = [1, 1, 1, 1]
+        self.orientation = quaternion.create_from_eulers([0.0, self.radius, 0.0])
+        self.start_socket = None
+        self._hovered_item = None
+        self.animation = 0  # rotation speed
+        self.node_class_selector = None
 
+        self.selected_item = None
+        self._last_selected_items = None
+        # self.last_collision_point = None
+        self.items = []
+        self.items_selected = []
+        self.items_deselected = []
+        self._selection_changed_listeners = []
+        self._items_deselected_listeners = []
+        self._has_been_modified_listeners = []
+
+        self.model = None
         self.get_model()
 
         # instance attributes
         self.Node = self.__class__.Node_class
         self.Edge = self.__class__.Edge_class
         self.calc = self.__class__.Calc_class()
         self.edge_drag = self.__class__.Edge_drag_class(self)
         self.history = self.__class__.History_class(self)
 
         self.xyz = position if position else ([randint(-25, 25), randint(-25, 25), randint(-25, 25)])
         self.texture_id = texture_id if texture_id or texture_id == 0 else randint(1, 5)
 
-        self.collision_object_id = self.create_collision_object(self)
+        self.collision_shape_id = self.uv.mouse_ray.get_collision_shape(self)
+        self.collision_object_id = self.uv.mouse_ray.create_collision_object(self)
 
         # for testing purposes a number of random nodes can be created
-        self.create_test_node(NUMBER_OF_TEST_NODES)
+        # self.create_test_node(NUMBER_OF_TEST_NODES)
 
         # add the sphere_base to the universe
         self.uv.add_sphere(self)
         self.history.store_initial_history_stamp()
 
-    def _init_variables(self):
-        self.scale = None
-        self.index = 0
-        self.radius = 1.0
-        self.color = None
-        self.orientation = quaternion.create_from_eulers([0.0, 0.0, 0.0])
-        self._hovered_item = None
-        self.color_id = 0  # color id translates to a relevance color. Higher numbers are closer to red
-        self.color_id_per_lens = 12345  # Each digit represents a color to be selected by a lens
-
-        self.selected_item = None
-        self.items = []
-        self.items_selected = []
-        self.items_deselected = []
-
-
-    def _init_listeners(self):
-        self._selection_changed_listeners = []
-        self._items_deselected_listeners = []
-        self._has_been_modified_listeners = []
-
-    def _init_flags(self):
-        self._has_been_modified = False
-        self._dragging = False
-        self._selected = False
-
     def get_model(self):
         # likely to be overridden
         self.model = self.uv.models.get_model('sphere_base')
-        self.shader = self.model.shader
-
-    def create_collision_object(self, sphere):
-        return self.uv.mouse_ray.create_collision_object(sphere)
-
-    @property
-    def selected(self) -> bool:
-        """
-        Sets 'selected' value .
-
-        :getter: Returns current state
-        :setter: Sets _dragging value
-        :type: ``bool``
-        """
-        return self._selected
-
-    @selected.setter
-    def selected(self, value: bool):
-        self._selected = value
 
     @property
     def dragging(self) -> bool:
         """
-        Something on the sphere_base has been modified. Sets modified value and calls all registered listeners.
 
         :getter: Returns current state
         :setter: Sets _dragging value
         :type: ``bool``
         """
         return self._dragging
 
@@ -186,136 +165,121 @@
         if not self._has_been_modified and value:
             # set it now, because we will be reading it soon
             self._has_been_modified = value
 
             # call all registered listeners
             for callback in self._has_been_modified_listeners:
                 callback()
+        else:
+            self._has_been_modified = value
 
-        self._has_been_modified = value
-
-    def add_has_been_modified_listener(self, callback: 'function'):
+    def add_has_been_modified_listener(self, callback):
         """
         Register callback for 'has been modified' event.
-
         :param callback: callback function
         """
         self._has_been_modified_listeners.append(callback)
 
-    def add_selection_changed_listener(self, callback: 'function'):
+    def add_selection_changed_listener(self, callback):
         """
         Register callback for 'selection changed' event.
-
         :param callback: callback function
         """
         self._selection_changed_listeners.append(callback)
 
-    def add_item_deselected_listener(self, callback: 'function'):
+    def add_item_deselected_listener(self, callback):
         """
         Register callback for `deselected item` event.
-
         :param callback: callback function
         """
         self._items_deselected_listeners.append(callback)
 
-    def create_test_node(self, number_of_nodes: int = 0):
-        """
-        Creates a number_of_nodes at random positions on the target node.
-
-        :param number_of_nodes: number of tests nodes to create
-        :type number_of_nodes: ``int``
-        """
-
-        for i in range(number_of_nodes):
-            x = randint(-30, 30)  # 30º above and below the equator
-            roll = (pi / 180 * (90 + x))
-            y = randint(160, 200)
-            pitch = (pi / 180 * y)
-            yaw = 0.0  # no yaw
-
-            orientation_offset = quaternion.create_from_eulers([roll, pitch, yaw])
-            self.Node(self, orientation_offset)
-            self.history.store_history("node created", True)
-
-    def create_new_node(self, node_type: str = "person", mouse_x: int = 0, mouse_y: int = 0) -> 'node':
+    def create_new_node(self, node_type: str = "person", abs_pos=None):
         """
         Needs to be overridden.
         Can be used to create any type of node at the mouse pointer.
 
         :param node_type: can be ``person`` or ``item``
         :type node_type: ``string``
-        :param mouse_x: x position of the mouse
-        :type mouse_x: ``float``
-        :param mouse_y: y position of the mouse
-        :type mouse_y: ``float``
-        :return: :class:`~sphere_iot.uv_node.SphereNode`
-        """
-        # calculate the cumulative angle based on the mouse position
-        orientation = self.calc_mouse_position_in_angles(mouse_x, mouse_y)
-
-        # create new node at the cumulative angle
-        node = self.Node(self, orientation)
+        :return: :class:`~sphere_iot.uv_node.Node`
+        :param abs_pos: position in space
+        :type abs_pos:
+        """
+        # # calculate the cumulative angle based on the mouse position
+        # orientation = self.calc_mouse_position_in_angles(mouse_x, mouse_y)
+        #
+        # # create new node at the cumulative angle
+        # node = self.Node(self, orientation)
+        # self.history.store_history("node created", True)
+        # return node
 
-        self.history.store_history("node created", True)
-        return node
+        return NotImplemented
 
-    def on_item_selected(self, items_selected):
+    def on_item_selected(self, current_selected_items):
         """
         Handles item selection and triggers event `Item _selected`.
         """
-        if items_selected:
+
+        if current_selected_items != self._last_selected_items:
+            self._last_selected_items = current_selected_items
 
             for callback in self._selection_changed_listeners:
+                callback(self, current_selected_items)
 
-                callback(self, items_selected)
                 self.history.store_history("Selection Changed")
 
-
     def on_item_deselected(self, item: 'Node or Edge'):
         """
         Handles item deselection and triggers event `Items deselected`. Not used in the current implementation.
 
         :param item: Node or Edge
-        :type item: :class:`~sphere_iot.uv_node.SphereNode` or :class:`~sphere_iot.uv_surface_edge.SphereSurfaceEdge`
+        :type item: :class:`~sphere_iot.uv_node.Node` or :class:`~sphere_iot.uv_surface_edge.SphereSurfaceEdge`
         """
-        for callback in self._items_deselected_listeners:
-            callback(self, item)
-            self.history.store_history("Deselected Everything")
+        current_selected_items = self.items_selected
+        if current_selected_items == self._last_selected_items:
+            return
 
-    def get_item_by_id(self, item_id: int) -> 'item':
+        if not current_selected_items:
+            self._last_selected_items = []
+
+            for callback in self._items_deselected_listeners:
+                callback(self, item)
+                self.history.store_history("Deselected Everything")
+
+    def get_item_by_id(self, item_id: int):
         """
         Helper function returns an item of type `node` or `edge` based on id.
 
         :param item_id: The id of the item to be returned
         :type item_id: ``int``
-        :return: :class:`~sphere_iot.uv_node.SphereNode` or :class:`~sphere_iot.uv_edge.SphereSurfaceEdge`
+        :return: :class:`~sphere_iot.uv_node.Node` or :class:`~sphere_iot.uv_edge.SphereSurfaceEdge`
         """
         for item in self.items:
             if item.id == item_id:
                 return item
         return None
 
     def get_selected_item(self, selected_item_id: int, shift: bool = False):
         """
         Helper function returns an item of type `node` or `edge` based on _selected item id.
 
         :param selected_item_id: id of the item to return
         :type selected_item_id: ``int``
         :param shift: ``True`` means that the shift is hold down while selecting
         :type shift: ``bool``
-        :return: :class:`~sphere_iot.uv_node.SphereNode` or :class:`~sphere_iot.uv_edge.SphereSurfaceEdge`
+        :return: :class:`~sphere_iot.uv_node.Node` or :class:`~sphere_iot.uv_edge.SphereSurfaceEdge`
         """
 
         for item in self.items:
             if selected_item_id == item.id:
                 self.select_item(item, shift)
                 return item
         return None
 
-    def get_socket_edges(self, socket: 'socket') -> list:
+    def get_socket_edges(self, socket) -> list:
         """
         Helper function returns a list of all edges connected to a node socket.
 
         :param socket: _selected node socket
         :type socket: :class:`~sphere_iot.uv_socket.Socket`
         :return: returns a ``list`` with edges of type :class:`~sphere_iot.uv_edge.SphereSurfaceEdge`
         """
@@ -323,35 +287,38 @@
         edges = []
         for item in self.items:
             if item.type == "edge" and socket in [item.start_socket, item.end_socket]:
                 edges.append(item)
         return edges
 
     def add_item(self, item: 'Node or Edge or Socket'):
-        """Add :class:`~sphere_iot.uv_node.SphereNode` or :class:`~sphere_iot.uv_edge.SphereSurfaceEdge` to the `Sphere`.
+        """Add :class:`~sphere_iot.uv_node.Node` or :class:`~sphere_iot.uv_edge.SphereSurfaceEdge`
+        to the `Sphere`.
 
         :param item: Node or Edge
-        :type item: :class:`~sphere_iot.uv_node.SphereNode` or :class:`~sphere_iot.uv_edge.SphereSurfaceEdge`
+        :type item: :class:`~sphere_iot.uv_node.Node` or :class:`~sphere_iot.uv_edge.SphereSurfaceEdge`
                     or :class:`~sphere_iot.uv_socket.Socket`
         """
 
         # adding item to sphere_base
         self.items.append(item)
 
     def remove_item(self, item: 'Node or Edge or Socket'):
-        """Remove :class:`~sphere_iot.uv_node.SphereNode` or :class:`~sphere_iot.uv_edge.SphereEdge` from the target `Sphere`.
+        """Remove :class:`~sphere_iot.uv_node.Node` or :class:`~sphere_iot.uv_edge.SphereEdge`
+        from the target `Sphere`.
         :param item: Node or Edge to remove from this `Sphere`
-        :type item: :class:`~sphere_iot.uv_node.SphereNode` or :class:`~sphere_iot.uv_surface_edge.SphereSurfaceEdge` or :class:`~sphere_iot.uv_socket.Socket`
+        :type item: :class:`~sphere_iot.uv_node.Node` or :class:`~sphere_iot.uv_surface_edge.SphereSurfaceEdge`
+        or :class:`~sphere_iot.uv_socket.Socket`
 
         """
         # removing item from sphere_base
         if item in self.items:
             self.items.remove(item)
 
-    def has_edge(self, start_socket: 'socket', end_socket: 'socket') -> bool:
+    def has_edge(self, start_socket, end_socket) -> bool:
         """
         Helper function that checks whether an edge with the same start and end socket already exists
 
         :param start_socket: edge start socket
         :type start_socket: :class:`~sphere_iot.uv_socket.Socket`
         :param end_socket: edge end socket
         :type end_socket: :class:`~sphere_iot.uv_socket.Socket`
@@ -361,29 +328,28 @@
         # Could possibly be optimized by not checking all edges on the sphere_base
         for item in self.items:
             if item.type == "edge":
                 if item.start_socket in [start_socket, end_socket] and item.end_socket in [start_socket, end_socket]:
                     return True
         return False
 
-    def create_edge(self, end_socket: 'socket') -> 'edge':
+    def create_edge(self, end_socket):
         """
         Create an edge between the _selected start socket and the received end socket if it does not already exist.
 
         :param end_socket: the end socket where the edge has to be drawn to.
         :type end_socket: :class:`~sphere_iot.uv_socket.Socket`
         :return: return :class:`~sphere_iot.uv_edge.SphereSurfaceEdge` or ``None``
         """
 
         if not self.has_edge(self.start_socket, end_socket):
             edge = self.Edge(self, self.start_socket, end_socket)
             self.history.store_history("edge created", True)
             return edge
 
-        # print("edge already exist, not created")
         return None
 
     def get_edges(self, start_socket=None, end_socket=None):
         """
         find the edge that has the given start and end socket.
 
         :param start_socket: start socket for the edge.
@@ -429,205 +395,75 @@
         Update the orientation of all items on the sphere_base.
 
         .. note::
 
             This method only explicitly instructs nodes to update themselves.
             updating nodes will trickle down, causing the connected node socket and connected edges to update as well.
         """
+
         # update orientation of all nodes on sphere_base
         for item in self.items:
             if item.type == "node":
                 # updating the node trickles down to updating sockets and edges"
                 item.update_position()
 
     def rotate_sphere(self, offset_degrees: int):
         """
         Rotating the sphere_base over the y-axis as per the offset_degrees.
 
         :param offset_degrees: degrees that the sphere_base rotates over its y-axis
         :type offset_degrees: ``int``
         """
 
-        # rotating the sphere_base over the y-axis
+        self.rotation_degrees += offset_degrees
+
+        if self.rotation_degrees > 180:
+            self.rotation_degrees -= 360
+        elif self.rotation_degrees < -180:
+            self.rotation_degrees = self.rotation_degrees + 360
+
         pitch = (pi / 180 * offset_degrees)
         rotation = quaternion.create_from_eulers([0.0, pitch, 0.0])
-        self.orientation = quaternion.cross(self.orientation, rotation)
+        self.orientation = quaternion.normalize(quaternion.cross(self.orientation, rotation))
         self.update_item_positions()
 
-    def calc_mouse_position_in_angles(self, mouse_x: float, mouse_y: float) -> 'quaternion':
-        """
-        Calculates the angle of the mouse pointer with the center of the target sphere_base. It takes into account the
-        distance of the camera with the target sphere_base and the distance of the mouse from the center of the screen.
-
-        :param mouse_x: x-position of the mouse pointer
-        :type mouse_x: ``float``
-        :param mouse_y: y-position of the mouse pointer
-        :type mouse_y: ``float``
-        :return: orientation quaternion
-        """
-
-        # ratio offset from center
-        x_offset = (2.0 * mouse_x) / self.uv.view.view_width - 1.0
-        y_offset = 1.0 - (2.0 * mouse_y) / self.uv.view.view_height
-
-        # camera to center of target sphere_base modifier
-        m = self.get_distance_modifier(self.uv.cam.distance_to_target)
-        p_x = self.get_position_modifier(x_offset, True)
-        p_y = self.get_position_modifier(y_offset, False)
-
-        # mouse pointer offset in radians
-        mouse_pitch = -(pi / 180 * (x_offset * p_x * m))
-        mouse_roll = -(pi / 180 * (y_offset * p_y * m))
-
-        # mouse pointer offset quaternions
-        mouse_pitch = quaternion.create_from_eulers([0.0, mouse_pitch, 0.0])
-        mouse_roll = quaternion.create_from_eulers([mouse_roll, 0.0, 0.0])
-
-        # camera direction in radians
-        pitch, roll = self.uv.cam.get_angles()
-        cam_roll = (pi / 180 * (90 - roll))
-        cam_pitch = (pi / 180 * (pitch + 90))
-        yaw = 0.0  # no yaw
-
-        # camera direction offset quaternions
-        camera_pitch = quaternion.create_from_eulers([0.0, cam_pitch, yaw])
-        camera_roll = quaternion.create_from_eulers([cam_roll, 0.0, yaw])
-
-        # vertical angles first
-        roll = quaternion.cross(mouse_roll, camera_roll)
-
-        # horizontal adjustment
-        pitch = quaternion.cross(mouse_pitch, camera_pitch)
-
-        # join all offsets
-        orientation = quaternion.cross(roll, pitch)
-        orientation = quaternion.cross(orientation, self.orientation)
-
-        # return orientation quaternion
-        return orientation
-
-    def drag_items(self, x_offset: float, y_offset: float):
+    def drag_items(self, mouse_ray_collision_point=None):
         """
         Dragging all _selected items. The offset is the difference between the current and last stored location
         of the mouse pointer on the screen.
 
-        :param x_offset: x_position offset of the current mouse_position and the last stored mouse position.
-        :type x_offset: ``float``
-        :param y_offset: y_position offset of the current mouse_position and the last stored mouse position.
-        :type y_offset: ``float``
+        :param mouse_ray_collision_point:
+        :type mouse_ray_collision_point: ``float``
         :return:
 
         .. note::
 
-           This method uses a distance modifier. The dragging speed depends on the distance
-           of the camera to the center of the target sphere_base.
-
            Only existing nodes need to be dragged, as the position of sockets and edges are
            adjusted automatically. Updating the position of a node trickles down to adjusting the position of the
            center sockets of the _selected nodes and any connected edges.
-        """
 
-        # distance modifier
-        m = self.get_distance_modifier(self.uv.cam.distance_to_target)
-
-        x_offset *= .02 * m
-        y_offset *= .02 * m
+           It is important to maintain the distance to the mouse. So we need to calculate the difference between the
+           current mouse position and the center of the items we are dragging. Otherwise the node centers jumps to
+           the collision point.
 
+        """
         for item in self.items_selected:
-            # only drag any nodes in the _selected item list
             if item.type == "node":
-                item.drag_to(x_offset, y_offset)
+                # only drag any nodes in the _selected item list
+                item.drag_to(mouse_ray_collision_point)
+                item.mouse_ray_collision_point = mouse_ray_collision_point
                 self.dragging = item.is_dragging(True)
 
-    def drag_edge(self, start_socket: 'socket', x_offset: float, y_offset: float, dragging: bool = True):
-        """
-        This methods is the start of creating a new edge.
-        A new edge is dragged from the start socket and shown as a dashed line.
-        This method adds a distance modifier before handing over to the :class:`~sphere_iot.uv_edge_drag.EdgeDrag`
-
-        :param start_socket: starting socket
-        :type start_socket: :class:`~sphere_iot.uv_socket.Socket`
-        :param x_offset: x_position offset of the current mouse_position and the last stored mouse position.
-        :type x_offset: ``float``
-        :param y_offset: y_position offset of the current mouse_position and the last stored mouse position.
-        :type y_offset:  ``float``
-        :param dragging: ``True`` when dragging
-        :type dragging: ``bool``
-        """
-        self.start_socket = start_socket
-        m = self.get_distance_modifier(self.uv.cam.distance_to_target) * .02
-
-        x_offset *= m
-        y_offset *= m
-
-        self.edge_drag.drag(start_socket, x_offset, y_offset, dragging)
-
-    @staticmethod
-    def get_distance_modifier(distance: float) -> int:
-        """
-
-        This function returns a modifier based on the distance between the camera and the target sphere_base center.
-        It is used while dragging object and creating new objects. The modifier is larger when the distance is larger.
-
-        :param distance: Distance between camera position and the center of the target sphere_base
-        :type distance: ``float``
-        :return: distance modifier ``int``
-
-        .. note::
-
-           All spheres in the basic implementation use a radius of 1. The minimum workable distance after extensive
-           testing is 1.5. Getting closer to the sphere_base causes sometimes the camera to jump inside the sphere_base.
-           When keeping a minimum distance of 2 this does not happen.
-
-        """
-
-        distance_modifier = {2: 3, 3: 6, 4: 9, 5: 12, 6: 15, 7: 18, 8: 21, 9: 24, 10: 27}
-        d = int(distance)
-        if d in distance_modifier:
-            return distance_modifier[int(distance)]
-        elif d > 10:
-            return distance_modifier[10]
-        else:
-            return pow(distance, 2)
-
-    @staticmethod
-    def get_position_modifier(ratio: float, mod_x=True) -> int:
-        """
-
-        This is a modifier based on the distance between the mouse pointer and the center of the screen.
-        ratio is between 0 and 1. There are some differences between horizontal, vertical, positive and negative.
-
-        :param ratio: ratio modifier between -1.0 and 1.0
-        :type ratio: ``float``
-        :param mod_x: ``True`` if the modifier is meant for the x-axis
-        :type mod_x: ``bool``
-        :return: position modifier ``int``
-        """
-        position_modifier_x = {0: 9, 1: 8, 2: 7, 3: 7, 4: 7, 5: 7, 6: 7, 7: 7, 8: 7, 9: 7,
-                               -1: 7, -2: 6, -3: 6, -4: 6, -5: 6, -6: 6, -7: 6, -8: 6, -9: 7}
-        position_modifier_y = {0: 9, 1: 8, 2: 7, 3: 7, 4: 8, 5: 8, 6: 8, 7: 9, 8: 9, 9: 9,
-                               -1: 7, -2: 6, -3: 7, -4: 8, -5: 8, -6: 8, -7: 9, -8: 9, -9: 9}
-
-        position_modifier = position_modifier_x if mod_x else position_modifier_y
-
-        d = int(ratio * 10)
-        if d in position_modifier:
-            return position_modifier[d]
-        elif d > 10:
-            return position_modifier[10]
-        else:
-            return 9
-
     def select_item(self, item: 'node or edge', shift: bool = False):
         """
         Select an item by clicking on it. Holding shift down while clicking on an item, adds it to the _selected list.
         Sockets cannot be _selected.
 
         :param item: ``Node`` or ``Edge``
-        :type item: :class:`~sphere_iot.uv_node.SphereNode` or :class:`~sphere_iot.uv_surface_edge.SphereSurfaceEdge`
+        :type item: :class:`~sphere_iot.uv_node.Node` or :class:`~sphere_iot.uv_surface_edge.SphereSurfaceEdge`
         :param shift: ``bool``, ``True`` when shift is down while clicking on an item
         """
 
         if shift:
             if item:
                 self.items_deselected = []
                 if item not in self.items_selected:
@@ -643,29 +479,25 @@
 
         for item in self.items_selected:
             item.on_selected_event(True)
 
         for item in self.items_deselected:
             item.on_selected_event(False)
 
-
         self.on_item_selected(self.items_selected)
 
-
     def delete_selected_items(self):
         """
         Remove _selected items. If item is node then the socket and the connected edges are also removed.
         """
         for selected_item in self.items_selected:
             for i, item in enumerate(self.items):
                 if item.id == selected_item.id:
                     if item.type == "node":
-                        # remove node, socket and connected items
-                        item.remove(with_edges=True)
-
+                        item.remove(with_edges=True)  # remove node, socket and connected items
                     elif item.type == "edge":
                         self.remove_edges([item])
 
         self.items_selected = []
         self.on_item_selected(self.items_selected)
 
     def batch_selected_items(self, item_list=None):
@@ -683,30 +515,29 @@
             for selected in item_list:
                 for item in self.items:
                     if selected == item.id and item.type == 'node':
                         self.select_item(item, True)
                     if selected == item.id and item.type == 'edge':
                         self.select_item(item, True)
 
-
     def check_for_hover(self, mouse_x, mouse_y):
         """
         When the camera is close to the sphere_base hover checking is activated. If the mouse is above an item
         its hover flag is set. It also takes of the flag of items that are not anymore hovered.
 
         :param mouse_x: mouse position x
         :type mouse_x: ``float``
         :param mouse_y: mouse position y
         :type mouse_y: ``float``
         """
 
         # find the current item that is under the mouse pointer
         hovered_item, hovered_item_pos = self.uv.mouse_ray.check_mouse_ray(mouse_x, mouse_y)
 
-        # if there is no sphere_base item under the mouse pointer the id will be the id of the sphere_base
+        # if there is no sphere item under the mouse pointer the id will be the id of the sphere
         if hovered_item and self._hovered_item and hovered_item == self.id:
             # no hovered items
             self._hovered_item.set_hovered(False)
             self._hovered_item = None
 
         if hovered_item and hovered_item != self.id:
             for item in self.items:
@@ -714,14 +545,16 @@
                     # set hover
                     item.set_hovered(True)
                     self._hovered_item = item
                 else:
                     # remove hover
                     item.set_hovered(False)
 
+        return self._hovered_item
+
     def edit_cut(self):
         """
         Cut _selected sphere_base items to clipboard
         """
         data = self.uv.clipboard.serialize_selected(delete=True)
         str_data = json.dumps(data, indent=4)
 
@@ -734,15 +567,17 @@
         data = self.uv.clipboard.serialize_selected(delete=False)
         str_data = json.dumps(data, indent=4)
         pyperclip.copy(str_data)
 
     def edit_paste(self):
         """
         Paste _selected sphere_base items from clipboard to the target sphere_base
+        check that the mouse pointer is above the sphere and get the position of the mouse_ray collision point.
         """
+
         raw_data = pyperclip.paste()
 
         try:
             data = json.loads(raw_data)
         except ValueError as e:
             print("Pasting of not valid json data!", e)
             return
@@ -760,103 +595,96 @@
         """
         for item in self.items:
             item.remove()
 
         self.uv.mouse_ray.delete_collision_object(self)
         self.uv.remove_sphere(self)
 
-    def on_lens_index_changed(self):
-        # if the lens changes than the relevance colors change as well
-        # Each digit in the 'color_id_per_lens' represents a color_id
-        if self.color_id_per_lens > 0:
-            color_id = int(str(self.color_id_per_lens)[self.uv.lens_index])
-            self.color = RELEVANCE_COLORS[color_id]
-
-    def draw(self):
-        """
-        Render the sphere_base and all the items on it.
+    def set_radius(self, radius):
         """
+        setting the radius of the sphere
 
-        self.model.draw(self, self.texture_id, color=self.color)
-        for item in self.items:
-            if item.type == "node":
-                item.draw()
-            elif item.type == "edge":
-                item.draw()
-
-        if self.edge_drag.dragging:
-            self.edge_drag.draw()
+        :param radius:
+        :return:
+        """
+        self.radius = radius
+        self.scale = [radius, radius, radius]
+        self.orientation = quaternion.create_from_eulers([0.0, radius, 0.0])
+        self.uv.cam.reset_to_default_view(self)
+        self.collision_shape_id = self.uv.mouse_ray.get_collision_shape(self)
 
-    def set_node_class_selector(self, class_selecting_function: 'function'):
+    def set_node_class_selector(self, class_selecting_function):
         """
         Helper method that sets the function which decides what `Node` class to instantiate when deserializing
         If not set, we will always instantiate :class:`~3dSphere.editor_node.Node` for each `Node` in the `UV`.
 
         :param class_selecting_function: node class
 
         """
         self.node_class_selector = class_selecting_function
 
     def get_node_class_from_data(self, data):
         """
         Takes `Node` serialized data and determines which `Node Class` to instantiate according to the description
         in the serialized Node.
         """
-        return SphereNode if self.node_class_selector is None else self.node_class_selector(data)
+        return Node if self.node_class_selector is None else self.node_class_selector(data)
 
-    def get_color_id_per_lens(self):
-        # returns a number with many digits, each digit represents a texture. Selecting a lens determines
-        # which digit to use
-        number = ""
-        if self.color_id_per_lens > 0:
-            number = self.color_id_per_lens
-        else:
-            for i in range(0, 21):
-                x = randint(1, 5)
-                number = int(str(number) + str(x))
+    def draw(self):
+        """
+        Render the sphere_base and all the items on it.
+        """
+
+        if self.animation != 0:
+            self.rotate_sphere(self.animation)
+
+        self.model.draw(self, texture_id=self.texture_id,  color=self.color)
+        for item in self.items:
+            if item.type == "node":
+                item.draw()
+            elif item.type == "edge":
+                item.draw()
 
-        return number
+        if self.edge_drag.dragging:
+            self.edge_drag.draw()
 
     def serialize(self):
         nodes, edges = [], []
         for item in self.items:
             if item.type == "node":
                 nodes.append(item.serialize())
             elif item.type == "edge":
                 edges.append(item.serialize())
 
         return OrderedDict([
             ('id', self.id),
             ('type', self.type),
             ('pos', self.xyz),
+            ('radius', self.radius),
             ('orientation', self.orientation.tolist()),
             ('texture_id', self.texture_id),
-            ('color_id', self.color_id),
-            ('color_id_per_lens', self.get_color_id_per_lens()),
+            ('color', self.color),
+            # ('color_id', self.color_id),
+            # ('color_id_per_lens', self.get_color_id_per_lens()),
             ('nodes', nodes),
             ('edges', edges),
         ])
 
     def deserialize(self, data: dict, hashmap: dict = {}, restore_id: bool = True) -> bool:
         if restore_id:
             self.id = data['id']
         hashmap[data['id']] = self
 
         self.xyz = data['pos']
         self.orientation = np.array(data['orientation'])
         self.texture_id = data['texture_id']
-        self.color_id = data['color_id']
-        self.color_id_per_lens = data['color_id_per_lens']
-
-        # Take the first color_id digit in the number
-        color_id = int(str(self.color_id_per_lens)[0])
-        c = RELEVANCE_COLORS[color_id]
-        # Create the color with the relevant transparency for the sphere_base
-        self.color = [c[0], c[1], c[2], TRANSPARENCY_DETAIL_SPHERE]
-
+        if 'color' in data:
+            self.color = data['color']
+        if 'radius' in data:
+            self.set_radius(data['radius'])
         self.uv.mouse_ray.reset_position_collision_object(self)
 
         # -- deserialize nodes on sphere_base
 
         # Instead of recreating all the nodes, reuse existing ones...
         all_items = self.items.copy()
 
@@ -873,22 +701,22 @@
                 if item.id == node_data['id']:
                     found = item
                     break
             if not found:
                 try:
                     new_node = self.get_node_class_from_data(node_data)(self)
                     new_node.deserialize(node_data, hashmap, restore_id)
-                except:
-                    dump_exception()
+                except Exception as e:
+                    dump_exception(e)
             else:
                 try:
                     found.deserialize(node_data, hashmap, restore_id)
                     all_items.remove(found)
-                except:
-                    dump_exception()
+                except Exception as e:
+                    dump_exception(e)
 
         # go through all deserialized edges:
         for edge_data in data['edges']:
             # can we find this edge in the data?
             found = None
             for item in all_items:
                 if item.id == edge_data['id']:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_sphere_edge.py` & `sphere_base-0.1.0/sphere_base/edge/inter_sphere_edge.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*-
 
 """
 Sphere Edge module. Contains the SphereEdge class. Edges are drawn between spheres.
 
 """
 
-from pyrr import quaternion, Vector3
+from pyrr import Vector3
 # from sphere_iot.uv_socket import *
-from sphere_universe_base.suv_graphic_edge import GraphicEdge
-from sphere_universe_base.suv_serializable import Serializable
+from sphere_base.edge.graphic_edge import GraphicEdge
+from sphere_base.serializable import Serializable
 from collections import OrderedDict
 
 
 DEBUG = False
 
 class SphereEdge(Serializable):
     """
```

### Comparing `sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_universe.py` & `sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_universe.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # -*- coding: utf-8 -*-
 
 """
 Module universe. The universe contains all the spheres.
 
 """
 
+from pyrr import quaternion, Quaternion
 from collections import OrderedDict
-from sphere_base.sphere_universe_base.suv_serializable import Serializable
-from sphere_base.sphere_universe_base.suv_sphere import Sphere
+from sphere_base.serializable import Serializable
+from sphere_base.sphere.sphere import Sphere
 from sphere_base.model.models import Models
 from sphere_base.sphere_universe_base.suv_mouse_ray import MouseRay
 from sphere_base.sphere_universe_base.suv_cam import Camera
 from sphere_base.sphere_universe_base.suv_skybox import Skybox
 from sphere_base.sphere_universe_base.suv_rubber_band import RubberBand
-from sphere_base.sphere_universe_base.suv_clipboard import Clipboard
-from sphere_base.sphere_universe_base.suv_config import UvConfig
-from sphere_base.shader.uv_default_shader import DefaultShader
+from sphere_base.clipboard import Clipboard
+from sphere_base.config import UvConfig
+from sphere_base.shader.default_shader import DefaultShader
+from sphere_base.calc import *
 import os.path
 
 DEBUG = False
-TEST_SPHERE_NUMBER = 25
+TEST_SPHERE_NUMBER = 1
 
 
 class Universe(Serializable):
     """
     This class represents the ``IOT universe``. It contains all the spheres
 
     """
@@ -33,22 +35,20 @@
     Shader_class = DefaultShader
     Ray_class = MouseRay
     Skybox_class = Skybox
     RubberBand_class = RubberBand
     Clipboard_class = Clipboard
     Config_class = UvConfig
 
-    def __init__(self, parent, skybox_img_directory=None, pybullet_key=None):
+    def __init__(self, parent, skybox_img_dir=None, sphere_texture_dir=None, pybullet_key=None):
         """
         Constructor of the ``Universe`` class
 
         :param parent: Reference to the universe class universe widget.
         :type parent: :class:`~sphere_iot.uv_widget.UV_Widget` or  :class:`~sphere_iot.uv_widget_glfw.UWidgetGLFW`.
-        :param skybox_set_name: The skybox set to instantiate
-        :type skybox_set_name: ``str``
         :param pybullet_key: Used to run the universe in its own physics engine
         :type pybullet_key: ``str``
 
         :Instance Attributes:
 
             - **target_sphere** - Instance of :class:`~sphere_iot.uv_sphere.Sphere`.
             - **config** - Instance of :class:`~sphere_iot.uv_config.UvConfig`.
@@ -70,59 +70,60 @@
 
         """
 
         super().__init__("sphere_iot")
 
         self.view = parent
 
-        self._init_variables()
+        self._spheres = []
+        self._edges = []
+        self._lens_index = 1  # variable to decide how to texture a sphere_base
+
+        self.mouse_last_x, self.mouse_last_y = self.view.view_width / 2, self.view.view_height / 2
+        self.mouse_x, self.mouse_y = self.mouse_last_x, self.mouse_last_y
+        self.mouse_offset = 0
+        self.target_sphere = None
+        self._has_been_modified = False
+
         self._init_listeners()
 
-        self.config = self.__class__.Config_class(self, skybox_img_directory)
+        self.config = self.__class__.Config_class(self, skybox_img_dir=skybox_img_dir,
+                                                  sphere_texture_dir=sphere_texture_dir)
         self.shader = self.__class__.Shader_class(self)
         self.cam = self.__class__.Camera_class(self)
         self.models = self.__class__.Models_class(self)
         self.Sphere = self.__class__.Sphere_class  # not instantiated here!
 
         self.mouse_ray = self.__class__.Ray_class(self, 1)
         self.skybox = self.__class__.Skybox_class(self)
         self.rubber_band_box = self.__class__.RubberBand_class(self)
         self.clipboard = self.__class__.Clipboard_class(self)
 
         if not os.path.exists("default.json"):
             self.create_test_spheres(TEST_SPHERE_NUMBER)
 
-    def _init_variables(self):
-        self._spheres = []
-        self._edges = []
-        self._lens_index = 1  # variable to decide how to texture a sphere_base
-
-        self.mouse_last_x, self.mouse_last_y = self.view.view_width / 2, self.view.view_height / 2
-        self.mouse_x, self.mouse_y = self.mouse_last_x, self.mouse_last_y
-        self.mouse_offset = 0
-        self.target_sphere = None
-        self._has_been_modified = False
-
     def _init_listeners(self):
         # initialize all listeners
         self._has_been_modified_listeners = []
         self._selection_changed_listeners = []
         self._items_deselected_listeners = []
 
     @property
     def lens_index(self):
         return self._lens_index
 
     @lens_index.setter
     def lens_index(self, value):
-        self._lens_index = value
+        pass
+        # self._lens_index = value
 
         # Change the relevance colors of all spheres
-        for sphere in self._spheres:
-            sphere.on_lens_index_changed()
+        # for sphere in self._spheres:
+        #     pass
+        # sphere.on_lens_index_changed()
 
     def clear(self):
         """
         Removes all spheres. This will then cascade down first removing all sphere_base items on each sphere_base.
         These items include nodes, sockets and edges.
 
         """
@@ -139,15 +140,14 @@
         """
         Re-create the sphere_iot universe
         :return:
 
         """
 
         self.clear()
-        self.skybox.get_random_skybox()
         self.create_test_spheres(TEST_SPHERE_NUMBER)
         self.cam.reset_to_default_view(self.target_sphere)
         self.on_selection_changed(None, None)
 
     def create_test_spheres(self, number: int = 0):
         """
         Create spheres for testing purposes
@@ -186,33 +186,31 @@
         :type sphere: :class:`~sphere_iot.uv_sphere.Sphere`
 
         """
 
         if sphere in self._spheres:
             self._spheres.remove(sphere)
 
-
     def add_edge(self, edge: 'Edge'):
         """
         Add a new edge to the internal list.
 
-        :param sphere_base: The ``edge`` that will be added to the ``Universe``
-        :type sphere_base: :class:`~sphere_iot.uv_sphere_edge.SphereEdge`
+        :param edge: The ``edge`` that will be added to the ``Universe``
+        :type edge: :class:`~sphere_iot.uv_sphere_edge.SphereEdge`
 
         """
 
         self._edges.append(edge)
 
-
     def remove_edge(self, edge: 'edge'):
         """
         Removing a sphere_base from the internal list.
 
-        :param sphere_base: The ``sphere_base`` that will be removed from the internal list``
-        :type sphere_base: :class:`~sphere_iot.uv_sphere.Sphere`
+        :param edge: The ``edge`` that will be removed from the internal list``
+        :type edge: :class:`~sphere_iot.uv_sphere_edge.SphereEdge`
 
         """
 
         if edge in self._edges:
             self._edges.remove(edge)
 
     def add_selection_changed_listener(self, callback: 'function'):
@@ -236,15 +234,16 @@
     def on_selection_changed(self, sphere: 'sphere_base', sphere_items: list):
         """
         Handles 'selection changed' and triggers event 'selection changed'.
 
         :param sphere: The target sphere_base that is _selected
         :type sphere: :class:`~sphere_iot.uv_sphere.Sphere`
         :param sphere_items: ``list`` of items on the sphere_base
-        :type sphere_items: list with items of type :class:`~sphere_iot.uv_node.SphereNode` or :class:`~sphere_iot.uv_edge.SphereSurfaceEdge`
+        :type sphere_items: list with items of type :class:`~sphere_iot.uv_node.Node` or
+        :class:`~sphere_iot.uv_edge.SphereSurfaceEdge`
 
         """
         for callback in self._selection_changed_listeners:
             callback(sphere, sphere_items)
 
     def on_modified(self):
         """
@@ -302,41 +301,41 @@
                 sphere.selected = True
                 self.target_sphere = sphere
                 self.cam.move_to_new_target_sphere(sphere)
                 is_sphere = True
                 self.on_selection_changed(self.target_sphere, None)
         return is_sphere
 
-    def rotate_target_sphere_with_mouse(self, offset: float = 0):
+    def rotate_target_sphere_with_mouse(self, offset: float = 0, collision_point=None):
         """
         Rotating the target sphere_base with the mouse y axis.
         Set the mouse offset here which will be picked up and used from the main loop and will be translated to rotation
 
         :param offset: mouse current x-position offset and last stored position.
         :type offset: ``float``
 
         .. note::
 
             This method only sets the mouse offset value which is then picked up from the main loop
 
         """
         # set the mouse offset here which will be picked up and used from the main loop
-        offset *= .05 * self.cam.distance_to_target
+
+        offset *= .05   # * self.cam.distance_to_target
         self.mouse_offset += offset
 
     def rotate_target_sphere(self):
         """
         Rotating the target sphere_base with the left and right arrows or dragging with the mouse.
         This method is called from the main loop
 
         """
-
         offset = 0
 
-        # rotating the target sphere_base with the left and right arrows
+        # rotating the target sphere with the left and right arrows
         if self.view.arrow_right:
             offset = 1.0  # degree
         if self.view.arrow_left:
             offset = -1.0  # degree
         if self.mouse_offset != 0:
             offset = self.mouse_offset
             self.mouse_offset = 0
@@ -366,14 +365,18 @@
         if self.view.down:
             angle_up = -.5
 
         # only process if there is movement
         if rotation or angle_up or radius:
             self.cam.process_movement(self.target_sphere, rotation, angle_up, radius=radius)
 
+    def get_mouse_pos(self):
+        # helper function to get the mouse variables
+        return self.view.get_mouse_pos()
+
     def draw(self):
         for sphere in self._spheres:
             sphere.draw()
         for edge in self._edges:
             edge.draw()
 
     def serialize(self):
@@ -386,17 +389,17 @@
             ('type', self.type),
             ('view_width', self.view.view_width),
             ('view_height', self.view.view_height),
             ('spheres', spheres),
             ('target_sphere_id', self.target_sphere.id)
         ])
 
-    def deserialize(self, data:dict, hashmap:dict={}, restore_id:bool=True) -> bool:
+    def deserialize(self, data: dict, hashmap: dict = None, restore_id: bool = True) -> bool:
         self.clear()
-        hashmap = {}
+        hashmap = hashmap if hashmap else {}
         self.id = data['id']
         self.mouse_ray.reset()
 
         # deserialize spheres
         for sphere_data in data['spheres']:
             self.Sphere(self, [0.0, 0.0, 0.0], 0).deserialize(sphere_data, hashmap)
```

### Comparing `sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_utils.py` & `sphere_base-0.1.0/sphere_base/utils.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.0.1/sphere_base/sphere_universe_base/suv_widget.py` & `sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_widget.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 Module UV_Widget. The layer on top of the universe.
 
 """
 
 from PyQt5.QtOpenGL import *
 from PyQt5.QtCore import *
 from PyQt5.QtWidgets import *
+from PyQt5.QtGui import QCursor
 
 import json
 
 from OpenGL.GL import *
 from sphere_base.sphere_universe_base.suv_universe import Universe
-from sphere_base.sphere_universe_base.suv_constants import *
-from sphere_base.sphere_universe_base.suv_utils import dump_exception
+from sphere_base.constants import *
+from sphere_base.utils import dump_exception
 
 
-class UV_Widget(QGLWidget):
+class UVWidget(QGLWidget):
     """
     This class represents the ``Universe Widget class`` its a pyqt5 wrapper around the OpenGL widget.
 
     """
 
     Universe_class = Universe
     keyPressed = pyqtSignal(int)
@@ -37,38 +38,34 @@
             - **view_width** - width of the view screen.
             - **view_height** - height of the view screen.
 
         """
         super().__init__(parent)
         self.setMinimumSize(640, 480)
 
-        self._init_flags()
-
         self.view_width, self.view_height = self.width(), self.height()
-        self._init_variables()
 
         self.setFocusPolicy(Qt.StrongFocus)
+
         self._delayed_init_listeners = []
         super().setMouseTracking(True)
 
-    def _init_variables(self):
-        self.pybullet_key = None
-
-    def _init_flags(self):
+        self.left, self.right, self.forward, self.back, self._shift = False, False, False, False, False
+        self.up, self.down, self.arrow_left, self.arrow_right = False, False, False, False
+        self._left_mouse_button_down, self._right_mouse_button_down = False, False
+        self._middle_mouse_button_down, self._mouse_button_down = False, False
         self._is_initialized = False
-        self._clicked_on_item = None
-        self._left_mouse_button_down = False
-        self._right_mouse_button_down = False
-        self._middle_mouse_button_down = False
-        self._shift = False
-        self._mouse_button_down = False
         self._first_mouse = False  # Is true ones after each mouse button press
-
-        self.left, self.right, self.forward, self.back = False, False, False, False
-        self.up, self.down, self.arrow_left, self.arrow_right = False, False, False, False
+        self.pybullet_key = None
+        self._clicked_on_item = None
+        self.mouse_ray_collision_point = None
+        self.mouse_x, self.mouse_y = None, None
+        self.uv = None
+        self.is_dragging = None
+        self.mouse_last_x, self.mouse_last_y = None, None
 
     def add_to_delayed_init(self, callback: 'function'):
         """
         Register callback for 'delayed init' event.
 
         :param callback: callback function
 
@@ -118,164 +115,172 @@
 
         :param event: xy-mouse position
         :type event: 'event'
         :return:
 
         """
         x, y = event.x(), event.y()
-        self._clicked_on_item, self.clicked_on_item_pos = self.uv.mouse_ray.check_mouse_ray(x, y)
+        self._clicked_on_item, self.mouse_ray_collision_point = self.uv.mouse_ray.check_mouse_ray(x, y)
 
         if self._clicked_on_item == self.uv.target_sphere.id:
-            self.handleContextMenu(event)
+            self.handle_context_menu(event)
         return super().contextMenuEvent(event)
 
-    def handleContextMenu(self, event: 'event'):
+    def get_mouse_pos(self):
         """
-        Handles context menu
-
-        :param event: Handles context menu
-        :type event: 'event
+        Helper function to get the object that the mouse is pointing at and to return the mouse ray collision
+        point coordinates.
 
         """
-        x, y = event.x(), event.y()
-        context_menu = QMenu(self)
-        create_person_node = context_menu.addAction("Person node")  # 1
-        create_item_node = context_menu.addAction("Item node")  # 2
-        create_entity_node = context_menu.addAction("Entity node")  # 3
-        action = context_menu.exec_(self.mapToGlobal(event.pos()))
-
-        if action == create_person_node:
-            self.uv.target_sphere.create_new_node(1, x, y, self.clicked_on_item_pos)
-        elif action == create_item_node:
-            self.uv.target_sphere.create_new_node(2, x, y, self.clicked_on_item_pos)
-        elif action == create_entity_node:
-            self.uv.target_sphere.create_new_node(1, x, y, self.clicked_on_item_pos)
+        self._clicked_on_item, self.mouse_ray_collision_point = self.uv.mouse_ray.check_mouse_ray(self.mouse_x,
+                                                                                                  self.mouse_y)
+        return self._clicked_on_item, self.mouse_ray_collision_point, self.mouse_x, self.mouse_y
 
     def mousePressEvent(self, event: 'event'):
         """
         Handles mouse press event
 
         :param event: contains the x and y mouse position
         :type event: 'event'
 
         """
 
         x, y = event.x(), event.y()
+        self.mouse_x = x
+        self.mouse_y = y
+        self.get_mouse_pos()
 
         if event.button() == Qt.LeftButton:
             self._first_mouse = True
             self._left_mouse_button_down = True
-            self._clicked_on_item, self.clicked_on_item_pos = self.uv.mouse_ray.check_mouse_ray(x, y)
 
             if not self._clicked_on_item:
                 return
 
             if self._clicked_on_item == self.uv.target_sphere.id:
 
-                # clicked on the target sphere_base (background). Release selection
+                # on_current_row_changed on the target sphere (background). Release selection
                 self.uv.target_sphere.selected_item = None
                 self.uv.target_sphere.select_item(None)
                 return
 
             is_sphere = self.uv.set_target_sphere(self._clicked_on_item)
 
-            # if it is not a sphere_base then get the _selected item
-
             if not is_sphere:
-                # set selected sphere_base item
+                # if it is not a sphere then get the _selected item, set selected sphere item
                 self.uv.target_sphere.get_selected_item(self._clicked_on_item, self._shift)
 
         if event.button() == Qt.RightButton:
             self._first_mouse = True
             self._right_mouse_button_down = True
-            self._clicked_on_item, self.clicked_on_item_pos = self.uv.mouse_ray.check_mouse_ray(x, y)
 
             if not self._clicked_on_item:
                 return
 
         if event.button() == Qt.MiddleButton:
             self._first_mouse = True
             self._middle_mouse_button_down = True
-            self._clicked_on_item, self.clicked_on_item_pos = self.uv.mouse_ray.check_mouse_ray(x, y)
+            self.uv.target_sphere.last_collision_point = self.mouse_ray_collision_point
 
     def _reset_mouse(self):
         """
         Reset the mouse flags
 
         """
         self._middle_mouse_button_down = False
         self._clicked_on_item = None
         self._left_mouse_button_down = False
         self._right_mouse_button_down = False
+        self.setCursor(QCursor(Qt.ArrowCursor))
 
     def mouseReleaseEvent(self, event):
         """
         Handles mouse release event
 
         :param event: contains the x and y mouse position
         :type event: 'event'
 
         """
-        self._reset_mouse()
-
-        if self.uv.target_sphere.dragging:
-            for item in self.uv.target_sphere.items_selected:
-                self.is_dragging = item.is_dragging(False)
 
         selection = self.uv.rubber_band_box.get_selection()
 
+        # if self.uv.target_sphere.dragging:
+        if self.is_dragging:
+
+            self.is_dragging = False
+            for item in self.uv.target_sphere.items_selected:
+                # Update the affected collision objects
+                item.update_collision_object()
+                item.is_dragging(False)
+            self.uv.target_sphere.history.store_history("node moved", set_modified=True)
+
         if selection:
             self.uv.target_sphere.batch_selected_items(selection)
+
         if self.uv.target_sphere.edge_drag.dragging:
-            self._clicked_on_item, self.clicked_on_item_pos = self.uv.mouse_ray.check_mouse_ray(self.mouse_x,
-                                                                                                self.mouse_y)
-            # self.target_sphere.edge_dragging.dragging = False
-            self.uv.target_sphere.edge_drag.drag(None, None, None, False)
+            try:
+                self.get_mouse_pos()
+                self.uv.target_sphere.edge_drag.drag(None, False, None)
 
-            is_sphere = self.uv.set_target_sphere(self._clicked_on_item)
+                is_sphere = self.uv.set_target_sphere(self._clicked_on_item)
 
-            # if it is not a sphere_base then get the _selected item
-            if not is_sphere:
-                item = self.uv.target_sphere.get_selected_item(self._clicked_on_item, self._shift)
-                if item and item.type == "socket":
-                    # if edge does not already exist, create it
-                    self.uv.target_sphere.create_edge(item)
-                elif item and item.type == "node":
-                    # if edge does not already exist, create it
-                    self.uv.target_sphere.create_edge(item.socket)
+                # if it is not a sphere then get the _selected item
+                if not is_sphere:
+                    item = self.uv.target_sphere.get_selected_item(self._clicked_on_item, self._shift)
+                    if item and item.type == "socket":
+                        # if edge does not already exist, create it
+                        self.uv.target_sphere.create_edge(item)
+                    elif item and item.type == "node":
+                        # if edge does not already exist, create it
+                        self.uv.target_sphere.create_edge(item.socket)
+            except Exception as e:
+                dump_exception(e)
+
+        if self._middle_mouse_button_down:
+            for item in self.uv.target_sphere.items:
+                item.update_collision_object()
+
+        self._reset_mouse()
 
     def mouseMoveEvent(self, event: 'event'):
         """
         Handles mouse release event
 
         :param event: contains the x and y mouse position
         :type event: 'event'
 
         """
-        x, y = event.x(), event.y()
-        self.mouse_x = x
-        self.mouse_y = y
 
+        x, y = event.x(), event.y()
+        self.mouse_x, self.mouse_y = x, y
+        self.get_mouse_pos()
 
         if self.uv.target_sphere and self.uv.cam.distance_to_target < HOVER_MIN_DISTANCE:
-            self.uv.target_sphere.check_for_hover(x, y)
+            hovered_item = self.uv.target_sphere.check_for_hover(x, y)
+            if hovered_item:
+                self.setCursor(QCursor(Qt.PointingHandCursor))
+            else:
+                self.setCursor(QCursor(Qt.ArrowCursor))
 
         if self._left_mouse_button_down:
 
             if self._clicked_on_item and self.uv.target_sphere.selected_item:
-
-                x_offset, y_offset = self.get_mouse_position_offset(x, y)
-
                 # dragging _selected items
-                if self.uv.target_sphere.selected_item.type == "node":
-                    self.uv.target_sphere.drag_items(x_offset, y_offset)
+                self.is_dragging = True
+                self.setCursor(QCursor(Qt.ClosedHandCursor))
+                # we are only looking at the first object in the selected objects.
+                # If it is node or edge then try to drag the whole selected group of items.
+                if self.uv.target_sphere.selected_item.type in ("node", "edge"):
+                    self.uv.target_sphere.drag_items(self.mouse_ray_collision_point)
                 elif self.uv.target_sphere.selected_item.type == "socket":
-                    # drag edge from socket
+                    # drag edge from socket to the mouse_ray collision point
                     start_socket = self.uv.target_sphere.selected_item
-                    self.uv.target_sphere.drag_edge(start_socket, x_offset, y_offset)
+                    self.uv.target_sphere.start_socket = start_socket
+                    self.uv.target_sphere.edge_drag.drag(start_socket, True,
+                                                         mouse_ray_collision_point=self.mouse_ray_collision_point)
 
             elif self._clicked_on_item and self._clicked_on_item == self.uv.target_sphere.id:
 
                 if self.uv.rubber_band_box.dragging:
                     # if already dragging a rubber_band_box keep dragging
                     self.uv.rubber_band_box.drag(start=False, mouse_x=x, mouse_y=y)
                 else:
@@ -283,23 +288,23 @@
                     self.uv.rubber_band_box.drag(start=True, mouse_x=x, mouse_y=y)
 
         elif self._middle_mouse_button_down:
 
             x_offset, y_offset = self.get_mouse_position_offset(x, y)
 
             if self._clicked_on_item and self._clicked_on_item == self.uv.target_sphere.id:
+                self.setCursor(QCursor(Qt.ClosedHandCursor))
+
                 # only rotate the sphere_base over the y axis
-                self.uv.rotate_target_sphere_with_mouse(x_offset)
+                self.uv.rotate_target_sphere_with_mouse(x_offset, self.mouse_ray_collision_point)
 
                 # rotation over the x axis are done through moving the camera
                 self.uv.cam.process_mouse_movement(self.uv.target_sphere, 0, -y_offset)
-            else:
-                self.uv.cam.process_mouse_movement(self.uv.target_sphere, x_offset, -y_offset)
 
-    def wheelEvent(self, event: 'event'):
+    def wheelEvent(self, event):
         """
         Handles mouse wheel event.
 
         :param event: contains mouse wheel rotation
 
         """
         step = 1 if event.angleDelta().y() > 0 else -1
@@ -341,19 +346,18 @@
             self.right = True
         elif event.key() == Qt.Key_Right:
             self.arrow_right = True
         elif event.key() == Qt.Key_Up:
             self.up = True
         elif event.key() == Qt.Key_Down:
             self.down = True
+        elif event.key() == Qt.Key_T:
+            self.uv.cam.get_cam_collision_point()
         elif event.key() == Qt.Key_P:
-            try:
-                self.uv.skybox.get_next_set()
-            except Exception as e:
-                dump_exception(e)
+            self.uv.skybox.get_next_set()
         elif event.key() == Qt.Key_O:
             self.uv.skybox.get_former_set()
         elif event.key() == Qt.Key_Delete:
             self.uv.target_sphere.delete_selected_items()
         elif event.key() == Qt.Key_Shift:
             self._shift = True
 
@@ -407,14 +411,50 @@
 
         # store the new mouse position as the last mouse position
         self.mouse_last_x = x_pos
         self.mouse_last_y = y_pos
 
         return x_offset, y_offset
 
+    def handle_context_menu(self, event: 'event'):
+        """
+        Handles context menu
+
+        :param event: Handles context menu
+        :type event: 'event
+
+        """
+
+        menuStyle = (
+            "QMenu::item{"
+            "background-color: lightGrey;"
+            "color: black;"
+            "}"
+            "QMenu::item:selected{"
+            "background-color: darkGrey;"
+            "color: rgb(255, 255, 255, 255);"
+            "}"
+        )
+
+        context_menu = QMenu(self)
+        context_menu.setStyleSheet(menuStyle)
+        context_menu.setGraphicsEffect(QGraphicsOpacityEffect(opacity=.8))
+        create_person_node = context_menu.addAction("Person node")  # 1
+        create_item_node = context_menu.addAction("Item node")  # 2
+
+        # create_entity_node = context_menu.addAction("Entity node")  # 3
+        action = context_menu.exec_(self.mapToGlobal(event.pos()))
+
+        if action == create_person_node:
+            self.uv.target_sphere.create_new_node(1, self.mouse_ray_collision_point)
+        elif action == create_item_node:
+            self.uv.target_sphere.create_new_node(2, self.mouse_ray_collision_point)
+        # elif action == create_entity_node:
+        #     self.uv.target_sphere.create_new_node(1, self.mouse_ray_collision_point)
+
     def save_to_file(self, file_name: str):
         """
         Save json to file
 
         :param file_name: path and name of the file to write to
         :type file_name: str
         :return:
@@ -432,14 +472,15 @@
 
         """
 
         with open(file_name, "r") as file:
             raw_data = file.read()
             data = json.loads(raw_data, encoding='utf-8')
             self.uv.deserialize(data)
+            self.uv.target_sphere.history.store_initial_history_stamp()
 
     def uv_new(self):
         """
         re-create the sphere_iot
 
         """
 
@@ -447,15 +488,18 @@
 
     def paintGL(self):
         """
         The main loop for rendering all objects
 
         """
 
+        # checking if the camera is moved with the keyboard
         self.uv.do_camera_movement()
+
+        # checking if the target sphere is rotated with the keyboard
         self.uv.rotate_target_sphere()
 
         glClear(GL_COLOR_BUFFER_BIT | GL_DEPTH_BUFFER_BIT | GL_STENCIL_BUFFER_BIT)
 
         self.uv.cam.draw()
         self.uv.skybox.draw()
```

### Comparing `sphere_base-0.0.1/tests/test_000_import.py` & `sphere_base-0.1.0/tests/test_000_import.py`

 * *Files identical despite different names*

