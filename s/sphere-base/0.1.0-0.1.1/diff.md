# Comparing `tmp/sphere_base-0.1.0.tar.gz` & `tmp/sphere_base-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphere_base-0.1.0.tar", last modified: Sun Apr 16 14:57:09 2023, max compression
+gzip compressed data, was "sphere_base-0.1.1.tar", last modified: Sun Apr 16 15:11:20 2023, max compression
```

## Comparing `sphere_base-0.1.0.tar` & `sphere_base-0.1.1.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.201292 sphere_base-0.1.0/
--rw-rw-rw-   0        0        0      978 2023-04-16 07:19:30.000000 sphere_base-0.1.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1105 2023-04-16 08:54:46.000000 sphere_base-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      252 2023-03-15 14:22:33.000000 sphere_base-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      737 2023-04-16 14:57:09.201292 sphere_base-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1090 2023-04-16 14:27:52.000000 sphere_base-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-16 14:57:08.989280 sphere_base-0.1.0/docs/
--rw-rw-rw-   0        0        0      638 2023-03-15 17:55:12.000000 sphere_base-0.1.0/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-04-16 14:57:08.964278 sphere_base-0.1.0/docs/build/
-drwxrwxrwx   0        0        0        0 2023-04-16 14:57:08.965278 sphere_base-0.1.0/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-04-16 14:57:08.994280 sphere_base-0.1.0/docs/build/html/_static/
--rw-rw-rw-   0        0        0      286 2023-03-15 17:53:40.000000 sphere_base-0.1.0/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.0/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.0/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      804 2023-03-15 17:55:12.000000 sphere_base-0.1.0/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-04-16 14:57:08.997280 sphere_base-0.1.0/docs/source/
--rw-rw-rw-   0        0        0     1175 2023-03-16 20:29:33.000000 sphere_base-0.1.0/docs/source/conf.py
--rw-rw-rw-   0        0        0      489 2023-03-16 21:15:47.000000 sphere_base-0.1.0/docs/source/index.rst
-drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.094286 sphere_base-0.1.0/docs/source/rst/
--rw-rw-rw-   0        0        0      163 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.model.mesh.rst
--rw-rw-rw-   0        0        0      166 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.model.model.rst
--rw-rw-rw-   0        0        0      169 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.model.models.rst
--rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.model.obj_file_loader.rst
--rw-rw-rw-   0        0        0      369 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.model.rst
--rw-rw-rw-   0        0        0      196 2023-03-16 21:18:48.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.rst
--rw-rw-rw-   0        0        0      780 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.rst
--rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_base_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_circle_shader.rst
--rw-rw-rw-   0        0        0      203 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_cross_shader.rst
--rw-rw-rw-   0        0        0      209 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_default_shader.rst
--rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_flat_shader.rst
--rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_holo_sphere_shader.rst
--rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_node_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_skybox_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_socket_shader.rst
--rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_sphere_edge_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_sphere_shader.rst
--rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_sphere_small_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.shader.uv_square_shader.rst
--rw-rw-rw-   0        0        0      602 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_overlay.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_overlay.sov_conf.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_overlay.sov_edge.rst
--rw-rw-rw-   0        0        0      212 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_overlay.sov_sphere.rst
--rw-rw-rw-   0        0        0      246 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_overlay.sov_sphere_node_base.rst
--rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_overlay.sov_uv_widget.rst
--rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.edge_sphere_item.rst
--rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.item_sphere_node.rst
--rw-rw-rw-   0        0        0      279 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.person_sphere_node.rst
--rw-rw-rw-   0        0        0      502 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.rst
--rw-rw-rw-   0        0        0     1563 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.rst
--rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_calc.rst
--rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_cam.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_cam_movement.rst
--rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_clipboard.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_config.rst
--rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_constants.rst
--rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_edge_drag.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_disc.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_edge.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_item.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_node.rst
--rw-rw-rw-   0        0        0      258 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_socket.rst
--rw-rw-rw-   0        0        0      235 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_history.rst
--rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_mouse_ray.rst
--rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_node.rst
--rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_rubber_band.rst
--rw-rw-rw-   0        0        0      250 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_serializable.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_skybox.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_socket.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere.rst
--rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere_edge.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_surface_edge.rst
--rw-rw-rw-   0        0        0      238 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_universe.rst
--rw-rw-rw-   0        0        0      229 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_utils.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.suv_widget.rst
--rw-rw-rw-   0        0        0      127 2023-03-15 17:49:53.000000 sphere_base-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 14:57:09.201292 sphere_base-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1507 2023-04-16 14:57:02.000000 sphere_base-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.107287 sphere_base-0.1.0/sphere_base/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.0/sphere_base/__init__.py
--rw-rw-rw-   0        0        0     8514 2023-04-14 08:27:37.000000 sphere_base-0.1.0/sphere_base/calc.py
--rw-rw-rw-   0        0        0     6909 2023-04-15 10:13:03.000000 sphere_base-0.1.0/sphere_base/clipboard.py
--rw-rw-rw-   0        0        0     5078 2023-04-14 08:50:15.000000 sphere_base-0.1.0/sphere_base/config.py
--rw-rw-rw-   0        0        0     5372 2023-04-15 11:21:35.000000 sphere_base-0.1.0/sphere_base/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.137288 sphere_base-0.1.0/sphere_base/edge/
--rw-rw-rw-   0        0        0        0 2023-03-30 07:32:40.000000 sphere_base-0.1.0/sphere_base/edge/__init__.py
--rw-rw-rw-   0        0        0     6609 2023-04-14 08:50:15.000000 sphere_base-0.1.0/sphere_base/edge/edge_drag.py
--rw-rw-rw-   0        0        0     4771 2023-04-14 17:26:15.000000 sphere_base-0.1.0/sphere_base/edge/graphic_edge.py
--rw-rw-rw-   0        0        0      365 2023-04-15 20:38:35.000000 sphere_base-0.1.0/sphere_base/edge/graphic_line.py
--rw-rw-rw-   0        0        0     1859 2023-04-04 08:07:28.000000 sphere_base-0.1.0/sphere_base/edge/inter_sphere_edge.py
--rw-rw-rw-   0        0        0    14064 2023-04-15 09:49:56.000000 sphere_base-0.1.0/sphere_base/edge/surface_edge.py
--rw-rw-rw-   0        0        0     9835 2023-04-08 12:55:07.000000 sphere_base-0.1.0/sphere_base/history.py
-drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.143289 sphere_base-0.1.0/sphere_base/model/
--rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.0/sphere_base/model/__init__.py
--rw-rw-rw-   0        0        0     4398 2023-04-04 14:50:05.000000 sphere_base-0.1.0/sphere_base/model/mesh.py
--rw-rw-rw-   0        0        0     6060 2023-04-11 18:27:52.000000 sphere_base-0.1.0/sphere_base/model/model.py
--rw-rw-rw-   0        0        0     3318 2023-04-04 11:04:51.000000 sphere_base-0.1.0/sphere_base/model/models.py
--rw-rw-rw-   0        0        0    23013 2023-04-07 13:30:04.000000 sphere_base-0.1.0/sphere_base/model/obj_file_loader.py
-drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.153289 sphere_base-0.1.0/sphere_base/node/
--rw-rw-rw-   0        0        0        0 2023-03-30 07:35:09.000000 sphere_base-0.1.0/sphere_base/node/__init__.py
--rw-rw-rw-   0        0        0     8018 2023-04-03 06:31:17.000000 sphere_base-0.1.0/sphere_base/node/graphic_disc.py
--rw-rw-rw-   0        0        0     2676 2023-04-03 06:31:17.000000 sphere_base-0.1.0/sphere_base/node/graphic_node.py
--rw-rw-rw-   0        0        0     2449 2023-04-03 06:31:16.000000 sphere_base-0.1.0/sphere_base/node/graphic_socket.py
--rw-rw-rw-   0        0        0    13284 2023-04-14 09:24:59.000000 sphere_base-0.1.0/sphere_base/node/node.py
--rw-rw-rw-   0        0        0     8797 2023-04-13 12:16:43.000000 sphere_base-0.1.0/sphere_base/node/socket.py
--rw-rw-rw-   0        0        0     1737 2023-03-30 07:13:13.000000 sphere_base-0.1.0/sphere_base/serializable.py
-drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.173290 sphere_base-0.1.0/sphere_base/shader/
--rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.0/sphere_base/shader/__init__.py
--rw-rw-rw-   0        0        0    10547 2023-04-14 08:50:15.000000 sphere_base-0.1.0/sphere_base/shader/base_shader.py
--rw-rw-rw-   0        0        0     1956 2023-03-30 12:23:24.000000 sphere_base-0.1.0/sphere_base/shader/circle_shader.py
--rw-rw-rw-   0        0        0     1946 2023-03-30 12:23:24.000000 sphere_base-0.1.0/sphere_base/shader/cross_shader.py
--rw-rw-rw-   0        0        0      572 2023-03-30 09:23:40.000000 sphere_base-0.1.0/sphere_base/shader/default_shader.py
--rw-rw-rw-   0        0        0     1174 2023-04-15 09:19:58.000000 sphere_base-0.1.0/sphere_base/shader/edge_shader.py
--rw-rw-rw-   0        0        0      886 2023-03-30 12:22:23.000000 sphere_base-0.1.0/sphere_base/shader/flat_shader.py
--rw-rw-rw-   0        0        0     1447 2023-03-30 12:22:23.000000 sphere_base-0.1.0/sphere_base/shader/holo_sphere_shader.py
--rw-rw-rw-   0        0        0     1160 2023-03-30 12:22:23.000000 sphere_base-0.1.0/sphere_base/shader/node_shader.py
--rw-rw-rw-   0        0        0     2150 2023-03-30 12:20:38.000000 sphere_base-0.1.0/sphere_base/shader/skybox_shader.py
--rw-rw-rw-   0        0        0     1238 2023-03-30 12:20:38.000000 sphere_base-0.1.0/sphere_base/shader/socket_shader.py
--rw-rw-rw-   0        0        0     3109 2023-03-31 17:56:46.000000 sphere_base-0.1.0/sphere_base/shader/sphere_edge_shader.py
--rw-rw-rw-   0        0        0     1631 2023-03-30 12:18:39.000000 sphere_base-0.1.0/sphere_base/shader/sphere_shader.py
--rw-rw-rw-   0        0        0     1232 2023-03-30 12:18:13.000000 sphere_base-0.1.0/sphere_base/shader/sphere_small_shader.py
--rw-rw-rw-   0        0        0     1808 2023-03-30 12:18:13.000000 sphere_base-0.1.0/sphere_base/shader/square_shader.py
-drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.176290 sphere_base-0.1.0/sphere_base/sphere/
--rw-rw-rw-   0        0        0        0 2023-03-28 18:59:07.000000 sphere_base-0.1.0/sphere_base/sphere/__init__.py
--rw-rw-rw-   0        0        0    28219 2023-04-16 07:14:28.000000 sphere_base-0.1.0/sphere_base/sphere/sphere.py
-drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.182291 sphere_base-0.1.0/sphere_base/sphere_overlay/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.0/sphere_base/sphere_overlay/__init__.py
--rw-rw-rw-   0        0        0     1875 2023-03-28 18:59:36.000000 sphere_base-0.1.0/sphere_base/sphere_overlay/sov_conf.py
--rw-rw-rw-   0        0        0     2468 2023-04-13 17:50:12.000000 sphere_base-0.1.0/sphere_base/sphere_overlay/sov_sphere.py
--rw-rw-rw-   0        0        0     1598 2023-04-13 12:14:08.000000 sphere_base-0.1.0/sphere_base/sphere_overlay/sov_sphere_node_base.py
-drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.186291 sphere_base-0.1.0/sphere_base/sphere_overlay/sphere_nodes/
--rw-rw-rw-   0        0        0      248 2021-03-02 15:18:12.000000 sphere_base-0.1.0/sphere_base/sphere_overlay/sphere_nodes/__init__.py
--rw-rw-rw-   0        0        0      460 2023-04-04 13:53:39.000000 sphere_base-0.1.0/sphere_base/sphere_overlay/sphere_nodes/edge_sphere_item.py
--rw-rw-rw-   0        0        0     1084 2023-04-13 12:16:43.000000 sphere_base-0.1.0/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py
--rw-rw-rw-   0        0        0     1002 2023-04-13 12:14:08.000000 sphere_base-0.1.0/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py
-drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.198292 sphere_base-0.1.0/sphere_base/sphere_universe_base/
--rw-rw-rw-   0        0        0       23 2021-03-11 14:37:00.000000 sphere_base-0.1.0/sphere_base/sphere_universe_base/__init__.py
--rw-rw-rw-   0        0        0     7829 2023-04-15 12:02:34.000000 sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_cam.py
--rw-rw-rw-   0        0        0     3434 2023-04-15 11:53:42.000000 sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_cam_movement.py
--rw-rw-rw-   0        0        0      365 2023-03-28 18:59:36.000000 sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_graphic_item.py
--rw-rw-rw-   0        0        0    15874 2023-04-14 08:50:15.000000 sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_mouse_ray.py
--rw-rw-rw-   0        0        0     7211 2023-04-14 09:13:08.000000 sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_rubber_band.py
--rw-rw-rw-   0        0        0     5392 2023-03-28 18:59:36.000000 sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_skybox.py
--rw-rw-rw-   0        0        0    14026 2023-04-14 08:50:15.000000 sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_universe.py
--rw-rw-rw-   0        0        0    17879 2023-04-16 07:15:30.000000 sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_widget.py
--rw-rw-rw-   0        0        0     1494 2023-03-30 07:18:00.000000 sphere_base-0.1.0/sphere_base/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.129288 sphere_base-0.1.0/sphere_base.egg-info/
--rw-rw-rw-   0        0        0      737 2023-04-16 14:57:08.000000 sphere_base-0.1.0/sphere_base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6024 2023-04-16 14:57:08.000000 sphere_base-0.1.0/sphere_base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 14:57:08.000000 sphere_base-0.1.0/sphere_base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-16 07:34:46.000000 sphere_base-0.1.0/sphere_base.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      119 2023-04-16 14:57:08.000000 sphere_base-0.1.0/sphere_base.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-16 14:57:08.000000 sphere_base-0.1.0/sphere_base.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-16 14:57:09.199292 sphere_base-0.1.0/tests/
--rw-rw-rw-   0        0        0      530 2023-03-15 14:00:41.000000 sphere_base-0.1.0/tests/test_000_import.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.799001 sphere_base-0.1.1/
+-rw-rw-rw-   0        0        0      978 2023-04-16 07:19:30.000000 sphere_base-0.1.1/HISTORY.rst
+-rw-rw-rw-   0        0        0     1105 2023-04-16 08:54:46.000000 sphere_base-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      252 2023-03-15 14:22:33.000000 sphere_base-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1968 2023-04-16 15:11:20.799001 sphere_base-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1074 2023-04-16 15:08:33.000000 sphere_base-0.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.578988 sphere_base-0.1.1/docs/
+-rw-rw-rw-   0        0        0      638 2023-03-15 17:55:12.000000 sphere_base-0.1.1/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.542986 sphere_base-0.1.1/docs/build/
+drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.542986 sphere_base-0.1.1/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.583988 sphere_base-0.1.1/docs/build/html/_static/
+-rw-rw-rw-   0        0        0      286 2023-03-15 17:53:40.000000 sphere_base-0.1.1/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.1/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.1/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      804 2023-03-15 17:55:12.000000 sphere_base-0.1.1/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.586988 sphere_base-0.1.1/docs/source/
+-rw-rw-rw-   0        0        0     1175 2023-03-16 20:29:33.000000 sphere_base-0.1.1/docs/source/conf.py
+-rw-rw-rw-   0        0        0      489 2023-03-16 21:15:47.000000 sphere_base-0.1.1/docs/source/index.rst
+drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.688994 sphere_base-0.1.1/docs/source/rst/
+-rw-rw-rw-   0        0        0      163 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.model.mesh.rst
+-rw-rw-rw-   0        0        0      166 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.model.model.rst
+-rw-rw-rw-   0        0        0      169 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.model.models.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.model.obj_file_loader.rst
+-rw-rw-rw-   0        0        0      369 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.model.rst
+-rw-rw-rw-   0        0        0      196 2023-03-16 21:18:48.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.rst
+-rw-rw-rw-   0        0        0      780 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_base_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_circle_shader.rst
+-rw-rw-rw-   0        0        0      203 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_cross_shader.rst
+-rw-rw-rw-   0        0        0      209 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_default_shader.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_flat_shader.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_holo_sphere_shader.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_node_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_skybox_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_socket_shader.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_sphere_edge_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_sphere_shader.rst
+-rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_sphere_small_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.shader.uv_square_shader.rst
+-rw-rw-rw-   0        0        0      602 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_overlay.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_overlay.sov_conf.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_overlay.sov_edge.rst
+-rw-rw-rw-   0        0        0      212 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_overlay.sov_sphere.rst
+-rw-rw-rw-   0        0        0      246 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_overlay.sov_sphere_node_base.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_overlay.sov_uv_widget.rst
+-rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.edge_sphere_item.rst
+-rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.item_sphere_node.rst
+-rw-rw-rw-   0        0        0      279 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.person_sphere_node.rst
+-rw-rw-rw-   0        0        0      502 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.rst
+-rw-rw-rw-   0        0        0     1563 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.rst
+-rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_calc.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_cam.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_cam_movement.rst
+-rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_clipboard.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_config.rst
+-rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_constants.rst
+-rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_edge_drag.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_disc.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_edge.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_item.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_node.rst
+-rw-rw-rw-   0        0        0      258 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_socket.rst
+-rw-rw-rw-   0        0        0      235 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_history.rst
+-rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_mouse_ray.rst
+-rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_node.rst
+-rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_rubber_band.rst
+-rw-rw-rw-   0        0        0      250 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_serializable.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_skybox.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_socket.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere.rst
+-rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere_edge.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_surface_edge.rst
+-rw-rw-rw-   0        0        0      238 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_universe.rst
+-rw-rw-rw-   0        0        0      229 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_utils.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.suv_widget.rst
+-rw-rw-rw-   0        0        0      127 2023-03-15 17:49:53.000000 sphere_base-0.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 15:11:20.799001 sphere_base-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1781 2023-04-16 15:10:58.000000 sphere_base-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.700995 sphere_base-0.1.1/sphere_base/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.1/sphere_base/__init__.py
+-rw-rw-rw-   0        0        0     8514 2023-04-14 08:27:37.000000 sphere_base-0.1.1/sphere_base/calc.py
+-rw-rw-rw-   0        0        0     6909 2023-04-15 10:13:03.000000 sphere_base-0.1.1/sphere_base/clipboard.py
+-rw-rw-rw-   0        0        0     5078 2023-04-14 08:50:15.000000 sphere_base-0.1.1/sphere_base/config.py
+-rw-rw-rw-   0        0        0     5372 2023-04-15 11:21:35.000000 sphere_base-0.1.1/sphere_base/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.720996 sphere_base-0.1.1/sphere_base/edge/
+-rw-rw-rw-   0        0        0        0 2023-03-30 07:32:40.000000 sphere_base-0.1.1/sphere_base/edge/__init__.py
+-rw-rw-rw-   0        0        0     6609 2023-04-14 08:50:15.000000 sphere_base-0.1.1/sphere_base/edge/edge_drag.py
+-rw-rw-rw-   0        0        0     4771 2023-04-14 17:26:15.000000 sphere_base-0.1.1/sphere_base/edge/graphic_edge.py
+-rw-rw-rw-   0        0        0      365 2023-04-15 20:38:35.000000 sphere_base-0.1.1/sphere_base/edge/graphic_line.py
+-rw-rw-rw-   0        0        0     1859 2023-04-04 08:07:28.000000 sphere_base-0.1.1/sphere_base/edge/inter_sphere_edge.py
+-rw-rw-rw-   0        0        0    14064 2023-04-15 09:49:56.000000 sphere_base-0.1.1/sphere_base/edge/surface_edge.py
+-rw-rw-rw-   0        0        0     9835 2023-04-08 12:55:07.000000 sphere_base-0.1.1/sphere_base/history.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.726997 sphere_base-0.1.1/sphere_base/model/
+-rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.1/sphere_base/model/__init__.py
+-rw-rw-rw-   0        0        0     4398 2023-04-04 14:50:05.000000 sphere_base-0.1.1/sphere_base/model/mesh.py
+-rw-rw-rw-   0        0        0     6060 2023-04-11 18:27:52.000000 sphere_base-0.1.1/sphere_base/model/model.py
+-rw-rw-rw-   0        0        0     3318 2023-04-04 11:04:51.000000 sphere_base-0.1.1/sphere_base/model/models.py
+-rw-rw-rw-   0        0        0    23013 2023-04-07 13:30:04.000000 sphere_base-0.1.1/sphere_base/model/obj_file_loader.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.734997 sphere_base-0.1.1/sphere_base/node/
+-rw-rw-rw-   0        0        0        0 2023-03-30 07:35:09.000000 sphere_base-0.1.1/sphere_base/node/__init__.py
+-rw-rw-rw-   0        0        0     8018 2023-04-03 06:31:17.000000 sphere_base-0.1.1/sphere_base/node/graphic_disc.py
+-rw-rw-rw-   0        0        0     2676 2023-04-03 06:31:17.000000 sphere_base-0.1.1/sphere_base/node/graphic_node.py
+-rw-rw-rw-   0        0        0     2449 2023-04-03 06:31:16.000000 sphere_base-0.1.1/sphere_base/node/graphic_socket.py
+-rw-rw-rw-   0        0        0    13284 2023-04-14 09:24:59.000000 sphere_base-0.1.1/sphere_base/node/node.py
+-rw-rw-rw-   0        0        0     8797 2023-04-13 12:16:43.000000 sphere_base-0.1.1/sphere_base/node/socket.py
+-rw-rw-rw-   0        0        0     1737 2023-03-30 07:13:13.000000 sphere_base-0.1.1/sphere_base/serializable.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.770999 sphere_base-0.1.1/sphere_base/shader/
+-rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.1/sphere_base/shader/__init__.py
+-rw-rw-rw-   0        0        0    10547 2023-04-14 08:50:15.000000 sphere_base-0.1.1/sphere_base/shader/base_shader.py
+-rw-rw-rw-   0        0        0     1956 2023-03-30 12:23:24.000000 sphere_base-0.1.1/sphere_base/shader/circle_shader.py
+-rw-rw-rw-   0        0        0     1946 2023-03-30 12:23:24.000000 sphere_base-0.1.1/sphere_base/shader/cross_shader.py
+-rw-rw-rw-   0        0        0      572 2023-03-30 09:23:40.000000 sphere_base-0.1.1/sphere_base/shader/default_shader.py
+-rw-rw-rw-   0        0        0     1174 2023-04-15 09:19:58.000000 sphere_base-0.1.1/sphere_base/shader/edge_shader.py
+-rw-rw-rw-   0        0        0      886 2023-03-30 12:22:23.000000 sphere_base-0.1.1/sphere_base/shader/flat_shader.py
+-rw-rw-rw-   0        0        0     1447 2023-03-30 12:22:23.000000 sphere_base-0.1.1/sphere_base/shader/holo_sphere_shader.py
+-rw-rw-rw-   0        0        0     1160 2023-03-30 12:22:23.000000 sphere_base-0.1.1/sphere_base/shader/node_shader.py
+-rw-rw-rw-   0        0        0     2150 2023-03-30 12:20:38.000000 sphere_base-0.1.1/sphere_base/shader/skybox_shader.py
+-rw-rw-rw-   0        0        0     1238 2023-03-30 12:20:38.000000 sphere_base-0.1.1/sphere_base/shader/socket_shader.py
+-rw-rw-rw-   0        0        0     3109 2023-03-31 17:56:46.000000 sphere_base-0.1.1/sphere_base/shader/sphere_edge_shader.py
+-rw-rw-rw-   0        0        0     1631 2023-03-30 12:18:39.000000 sphere_base-0.1.1/sphere_base/shader/sphere_shader.py
+-rw-rw-rw-   0        0        0     1232 2023-03-30 12:18:13.000000 sphere_base-0.1.1/sphere_base/shader/sphere_small_shader.py
+-rw-rw-rw-   0        0        0     1808 2023-03-30 12:18:13.000000 sphere_base-0.1.1/sphere_base/shader/square_shader.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.773999 sphere_base-0.1.1/sphere_base/sphere/
+-rw-rw-rw-   0        0        0        0 2023-03-28 18:59:07.000000 sphere_base-0.1.1/sphere_base/sphere/__init__.py
+-rw-rw-rw-   0        0        0    28219 2023-04-16 07:14:28.000000 sphere_base-0.1.1/sphere_base/sphere/sphere.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.779999 sphere_base-0.1.1/sphere_base/sphere_overlay/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.1/sphere_base/sphere_overlay/__init__.py
+-rw-rw-rw-   0        0        0     1875 2023-03-28 18:59:36.000000 sphere_base-0.1.1/sphere_base/sphere_overlay/sov_conf.py
+-rw-rw-rw-   0        0        0     2468 2023-04-13 17:50:12.000000 sphere_base-0.1.1/sphere_base/sphere_overlay/sov_sphere.py
+-rw-rw-rw-   0        0        0     1598 2023-04-13 12:14:08.000000 sphere_base-0.1.1/sphere_base/sphere_overlay/sov_sphere_node_base.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.785000 sphere_base-0.1.1/sphere_base/sphere_overlay/sphere_nodes/
+-rw-rw-rw-   0        0        0      248 2021-03-02 15:18:12.000000 sphere_base-0.1.1/sphere_base/sphere_overlay/sphere_nodes/__init__.py
+-rw-rw-rw-   0        0        0      460 2023-04-04 13:53:39.000000 sphere_base-0.1.1/sphere_base/sphere_overlay/sphere_nodes/edge_sphere_item.py
+-rw-rw-rw-   0        0        0     1084 2023-04-13 12:16:43.000000 sphere_base-0.1.1/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py
+-rw-rw-rw-   0        0        0     1002 2023-04-13 12:14:08.000000 sphere_base-0.1.1/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.796000 sphere_base-0.1.1/sphere_base/sphere_universe_base/
+-rw-rw-rw-   0        0        0       23 2021-03-11 14:37:00.000000 sphere_base-0.1.1/sphere_base/sphere_universe_base/__init__.py
+-rw-rw-rw-   0        0        0     7829 2023-04-15 12:02:34.000000 sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_cam.py
+-rw-rw-rw-   0        0        0     3434 2023-04-15 11:53:42.000000 sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_cam_movement.py
+-rw-rw-rw-   0        0        0      365 2023-03-28 18:59:36.000000 sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_graphic_item.py
+-rw-rw-rw-   0        0        0    15874 2023-04-14 08:50:15.000000 sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_mouse_ray.py
+-rw-rw-rw-   0        0        0     7211 2023-04-14 09:13:08.000000 sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_rubber_band.py
+-rw-rw-rw-   0        0        0     5392 2023-03-28 18:59:36.000000 sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_skybox.py
+-rw-rw-rw-   0        0        0    14026 2023-04-14 08:50:15.000000 sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_universe.py
+-rw-rw-rw-   0        0        0    17879 2023-04-16 07:15:30.000000 sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_widget.py
+-rw-rw-rw-   0        0        0     1494 2023-03-30 07:18:00.000000 sphere_base-0.1.1/sphere_base/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.711995 sphere_base-0.1.1/sphere_base.egg-info/
+-rw-rw-rw-   0        0        0     1968 2023-04-16 15:11:20.000000 sphere_base-0.1.1/sphere_base.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6024 2023-04-16 15:11:20.000000 sphere_base-0.1.1/sphere_base.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 15:11:20.000000 sphere_base-0.1.1/sphere_base.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-16 07:34:46.000000 sphere_base-0.1.1/sphere_base.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      119 2023-04-16 15:11:20.000000 sphere_base-0.1.1/sphere_base.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-16 15:11:20.000000 sphere_base-0.1.1/sphere_base.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 15:11:20.797001 sphere_base-0.1.1/tests/
+-rw-rw-rw-   0        0        0      530 2023-03-15 14:00:41.000000 sphere_base-0.1.1/tests/test_000_import.py
```

### Comparing `sphere_base-0.1.0/HISTORY.rst` & `sphere_base-0.1.1/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/LICENSE` & `sphere_base-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/README.rst` & `sphere_base-0.1.1/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,52 @@
 Sphere Base
-###########
+############
 
 Introduction
-============
+=============
 
 This library was created as a building block for use in applications were information should be displayed as nodes or
 labels on a sphere. These nodes are interactive so they can be moved by dragging and connecting them to other nodes.
 
 This package is created in python using a pyqt5 window.
 
 * Development Status :: 4 - Beta
 * Free software: MIT license
 
 
 Features
-========
+=========
 
 - Customizable spheres with textures and colors
 - Nodes, sockets and edges can be dragged over the surface of the sphere
 - Support for undo/redo, cut and paste using serialization
 - Hovering effects, dragging nodes, cutting edges
 - Example on how the library can be implemented
 
-
 Requirements
-============
+=============
 
 - Python 3.x
 - PyOpenGL
 - PyQt5
 
 
 Supported Environment
 ======================
 
 * Windows (Win32, x64)
 
-::
 
-The library is available from PyPI::
+The library is available from PyPI
 
     $ pip install sphere-base==0.0.1
 
 
-::
-
-
-Or download the source code from github::
+Or download the source code from github
 
     git clone https://github.com/rboltze/sphere_base.git
 
 
-::
+
```

### Comparing `sphere_base-0.1.0/docs/Makefile` & `sphere_base-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/docs/make.bat` & `sphere_base-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/docs/source/conf.py` & `sphere_base-0.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/docs/source/rst/sphere_base.shader.rst` & `sphere_base-0.1.1/docs/source/rst/sphere_base.shader.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_overlay.rst` & `sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_overlay.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/docs/source/rst/sphere_base.sphere_universe_base.rst` & `sphere_base-0.1.1/docs/source/rst/sphere_base.sphere_universe_base.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/setup.py` & `sphere_base-0.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,22 +27,25 @@
         'License :: OSI Approved :: BSD License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
     description="The library was created to be used as a building block for applications were information"
-                "should appear on the surface of a sphere.",
+                "should appear on the surface of a sphere. It allows for creating spheres with nodes"
+                "and edges that can be dragged on its surface. Nodes and edges can be placed and removed "
+                "from the sphere surface. \n"
+                "This library is written in Python, PyOpenGL and PyQT5",
     install_requires=requirements,
     license="MIT license",
-    long_description="",
+    long_description=readme,
     include_package_data=True,
     keywords='sphere_base',
     name='sphere_base',
     packages=find_packages(include=['sphere_base*'], exclude=['examples*', 'test*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/rboltze/spherebase',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

### Comparing `sphere_base-0.1.0/sphere_base/calc.py` & `sphere_base-0.1.1/sphere_base/calc.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/clipboard.py` & `sphere_base-0.1.1/sphere_base/clipboard.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/config.py` & `sphere_base-0.1.1/sphere_base/config.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/constants.py` & `sphere_base-0.1.1/sphere_base/constants.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/edge/edge_drag.py` & `sphere_base-0.1.1/sphere_base/edge/edge_drag.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/edge/graphic_edge.py` & `sphere_base-0.1.1/sphere_base/edge/graphic_edge.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/edge/inter_sphere_edge.py` & `sphere_base-0.1.1/sphere_base/edge/inter_sphere_edge.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/edge/surface_edge.py` & `sphere_base-0.1.1/sphere_base/edge/surface_edge.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/history.py` & `sphere_base-0.1.1/sphere_base/history.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/model/mesh.py` & `sphere_base-0.1.1/sphere_base/model/mesh.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/model/model.py` & `sphere_base-0.1.1/sphere_base/model/model.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/model/models.py` & `sphere_base-0.1.1/sphere_base/model/models.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/model/obj_file_loader.py` & `sphere_base-0.1.1/sphere_base/model/obj_file_loader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/node/graphic_disc.py` & `sphere_base-0.1.1/sphere_base/node/graphic_disc.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/node/graphic_node.py` & `sphere_base-0.1.1/sphere_base/node/graphic_node.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/node/graphic_socket.py` & `sphere_base-0.1.1/sphere_base/node/graphic_socket.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/node/node.py` & `sphere_base-0.1.1/sphere_base/node/node.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/node/socket.py` & `sphere_base-0.1.1/sphere_base/node/socket.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/serializable.py` & `sphere_base-0.1.1/sphere_base/serializable.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/shader/base_shader.py` & `sphere_base-0.1.1/sphere_base/shader/base_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/shader/circle_shader.py` & `sphere_base-0.1.1/sphere_base/shader/circle_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/shader/cross_shader.py` & `sphere_base-0.1.1/sphere_base/shader/cross_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/shader/default_shader.py` & `sphere_base-0.1.1/sphere_base/shader/default_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/shader/edge_shader.py` & `sphere_base-0.1.1/sphere_base/shader/edge_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/shader/flat_shader.py` & `sphere_base-0.1.1/sphere_base/shader/flat_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/shader/holo_sphere_shader.py` & `sphere_base-0.1.1/sphere_base/shader/holo_sphere_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/shader/node_shader.py` & `sphere_base-0.1.1/sphere_base/shader/node_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/shader/skybox_shader.py` & `sphere_base-0.1.1/sphere_base/shader/skybox_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/shader/socket_shader.py` & `sphere_base-0.1.1/sphere_base/shader/socket_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/shader/sphere_edge_shader.py` & `sphere_base-0.1.1/sphere_base/shader/sphere_edge_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/shader/sphere_shader.py` & `sphere_base-0.1.1/sphere_base/shader/sphere_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/shader/sphere_small_shader.py` & `sphere_base-0.1.1/sphere_base/shader/sphere_small_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/shader/square_shader.py` & `sphere_base-0.1.1/sphere_base/shader/square_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/sphere/sphere.py` & `sphere_base-0.1.1/sphere_base/sphere/sphere.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/sphere_overlay/sov_conf.py` & `sphere_base-0.1.1/sphere_base/sphere_overlay/sov_conf.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/sphere_overlay/sov_sphere.py` & `sphere_base-0.1.1/sphere_base/sphere_overlay/sov_sphere.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/sphere_overlay/sov_sphere_node_base.py` & `sphere_base-0.1.1/sphere_base/sphere_overlay/sov_sphere_node_base.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py` & `sphere_base-0.1.1/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py` & `sphere_base-0.1.1/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_cam.py` & `sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_cam.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_cam_movement.py` & `sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_cam_movement.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_mouse_ray.py` & `sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_mouse_ray.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_rubber_band.py` & `sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_rubber_band.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_skybox.py` & `sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_skybox.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_universe.py` & `sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_universe.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/sphere_universe_base/suv_widget.py` & `sphere_base-0.1.1/sphere_base/sphere_universe_base/suv_widget.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base/utils.py` & `sphere_base-0.1.1/sphere_base/utils.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/sphere_base.egg-info/SOURCES.txt` & `sphere_base-0.1.1/sphere_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.0/tests/test_000_import.py` & `sphere_base-0.1.1/tests/test_000_import.py`

 * *Files identical despite different names*

