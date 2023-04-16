# Comparing `tmp/scikit-robot-0.0.8.tar.gz` & `tmp/scikit-robot-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scikit-robot-0.0.8.tar", last modified: Sun Aug  2 09:13:38 2020, max compression
+gzip compressed data, was "dist/scikit-robot-0.0.9.tar", last modified: Fri Oct 16 01:50:19 2020, max compression
```

## Comparing `scikit-robot-0.0.8.tar` & `scikit-robot-0.0.9.tar`

### file list

```diff
@@ -1,93 +1,97 @@
-drwxrwxr-x   0 iory      (1000) iory      (1000)        0 2020-08-02 09:13:38.000000 scikit-robot-0.0.8/
--rw-rw-r--   0 iory      (1000) iory      (1000)      286 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/requirements.txt
--rw-rw-r--   0 iory      (1000) iory      (1000)     1471 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/README.md
-drwxrwxr-x   0 iory      (1000) iory      (1000)        0 2020-08-02 09:13:38.000000 scikit-robot-0.0.8/scikit_robot.egg-info/
--rw-rw-r--   0 iory      (1000) iory      (1000)        1 2020-08-02 09:13:38.000000 scikit-robot-0.0.8/scikit_robot.egg-info/not-zip-safe
--rw-rw-r--   0 iory      (1000) iory      (1000)        8 2020-08-02 09:13:38.000000 scikit-robot-0.0.8/scikit_robot.egg-info/top_level.txt
--rw-rw-r--   0 iory      (1000) iory      (1000)      226 2020-08-02 09:13:38.000000 scikit-robot-0.0.8/scikit_robot.egg-info/requires.txt
--rw-rw-r--   0 iory      (1000) iory      (1000)       69 2020-08-02 09:13:38.000000 scikit-robot-0.0.8/scikit_robot.egg-info/entry_points.txt
--rw-rw-r--   0 iory      (1000) iory      (1000)     2798 2020-08-02 09:13:38.000000 scikit-robot-0.0.8/scikit_robot.egg-info/SOURCES.txt
--rw-rw-r--   0 iory      (1000) iory      (1000)        1 2020-08-02 09:13:38.000000 scikit-robot-0.0.8/scikit_robot.egg-info/dependency_links.txt
--rw-rw-r--   0 iory      (1000) iory      (1000)     2578 2020-08-02 09:13:38.000000 scikit-robot-0.0.8/scikit_robot.egg-info/PKG-INFO
-drwxrwxr-x   0 iory      (1000) iory      (1000)        0 2020-08-02 09:13:38.000000 scikit-robot-0.0.8/skrobot/
--rw-rw-r--   0 iory      (1000) iory      (1000)     7734 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/interpolator.py
-drwxrwxr-x   0 iory      (1000) iory      (1000)        0 2020-08-02 09:13:38.000000 scikit-robot-0.0.8/skrobot/utils/
--rw-rw-r--   0 iory      (1000) iory      (1000)       52 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/utils/__init__.py
--rw-rw-r--   0 iory      (1000) iory      (1000)    96734 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/utils/urdf.py
--rw-rw-r--   0 iory      (1000) iory      (1000)      127 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/utils/listify.py
--rw-rw-r--   0 iory      (1000) iory      (1000)      399 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/__init__.py
-drwxrwxr-x   0 iory      (1000) iory      (1000)        0 2020-08-02 09:13:38.000000 scikit-robot-0.0.8/skrobot/models/
--rw-rw-r--   0 iory      (1000) iory      (1000)      531 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/models/__init__.py
--rw-rw-r--   0 iory      (1000) iory      (1000)     1259 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/models/panda.py
--rw-rw-r--   0 iory      (1000) iory      (1000)     2285 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/models/kuka.py
--rw-rw-r--   0 iory      (1000) iory      (1000)     5122 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/models/primitives.py
--rw-rw-r--   0 iory      (1000) iory      (1000)      616 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/models/urdf.py
--rw-rw-r--   0 iory      (1000) iory      (1000)     8164 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/models/pr2.py
--rw-rw-r--   0 iory      (1000) iory      (1000)     2598 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/models/fetch.py
-drwxrwxr-x   0 iory      (1000) iory      (1000)        0 2020-08-02 09:13:38.000000 scikit-robot-0.0.8/skrobot/coordinates/
--rw-rw-r--   0 iory      (1000) iory      (1000)      548 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/coordinates/__init__.py
--rw-rw-r--   0 iory      (1000) iory      (1000)     4609 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/coordinates/geo.py
--rw-rw-r--   0 iory      (1000) iory      (1000)    14379 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/coordinates/dual_quaternion.py
--rw-rw-r--   0 iory      (1000) iory      (1000)    42532 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/coordinates/math.py
--rw-rw-r--   0 iory      (1000) iory      (1000)    39713 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/coordinates/base.py
--rw-rw-r--   0 iory      (1000) iory      (1000)    12063 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/coordinates/quaternion.py
--rw-rw-r--   0 iory      (1000) iory      (1000)     1617 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/optimizer.py
-drwxrwxr-x   0 iory      (1000) iory      (1000)        0 2020-08-02 09:13:38.000000 scikit-robot-0.0.8/skrobot/data/
--rw-rw-r--   0 iory      (1000) iory      (1000)     1327 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/__init__.py
-drwxrwxr-x   0 iory      (1000) iory      (1000)        0 2020-08-02 09:13:38.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/
-drwxrwxr-x   0 iory      (1000) iory      (1000)        0 2020-08-02 09:13:38.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/
--rwxrwxr-x   0 iory      (1000) iory      (1000)    10084 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/finger_base_right.stl
--rw-rw-r--   0 iory      (1000) iory      (1000)    77434 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_4.stl
--rw-rw-r--   0 iory      (1000) iory      (1000)   115751 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_3.obj
--rw-rw-r--   0 iory      (1000) iory      (1000)      137 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_1.mtl
--rwxrwxr-x   0 iory      (1000) iory      (1000)     6984 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/finger_tip_right.stl
--rw-rw-r--   0 iory      (1000) iory      (1000)    93414 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_4.obj
--rw-rw-r--   0 iory      (1000) iory      (1000)      137 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_6.mtl
--rwxrwxr-x   0 iory      (1000) iory      (1000)    10084 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/finger_base_left.stl
--rw-rw-r--   0 iory      (1000) iory      (1000)      137 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_5.mtl
--rw-rw-r--   0 iory      (1000) iory      (1000)   185365 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_0.obj
--rw-rw-r--   0 iory      (1000) iory      (1000)    76096 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_5.obj
--rw-rw-r--   0 iory      (1000) iory      (1000)    68485 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_6.obj
--rw-rw-r--   0 iory      (1000) iory      (1000)      137 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_3.mtl
--rw-rw-r--   0 iory      (1000) iory      (1000)    57934 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_6.stl
--rw-rw-r--   0 iory      (1000) iory      (1000)   138034 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_1.stl
--rw-rw-r--   0 iory      (1000) iory      (1000)      137 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_0.mtl
--rw-rw-r--   0 iory      (1000) iory      (1000)   170199 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_1.obj
--rw-rw-r--   0 iory      (1000) iory      (1000)    92888 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_7.obj
--rw-rw-r--   0 iory      (1000) iory      (1000)      137 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_2.mtl
--rw-rw-r--   0 iory      (1000) iory      (1000)   151984 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_0.stl
--rw-rw-r--   0 iory      (1000) iory      (1000)    86691 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_2.obj
--rw-rw-r--   0 iory      (1000) iory      (1000)    96984 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_3.stl
--rw-rw-r--   0 iory      (1000) iory      (1000)      137 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_4.mtl
--rw-rw-r--   0 iory      (1000) iory      (1000)    75684 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_7.stl
--rwxrwxr-x   0 iory      (1000) iory      (1000)     6984 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/finger_tip_left.stl
--rw-rw-r--   0 iory      (1000) iory      (1000)      137 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_7.mtl
--rw-rw-r--   0 iory      (1000) iory      (1000)    72534 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_2.stl
--rw-rw-r--   0 iory      (1000) iory      (1000)    67984 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_5.stl
--rw-rw-r--   0 iory      (1000) iory      (1000)    16001 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/data/kuka_description/kuka.urdf
--rw-rw-r--   0 iory      (1000) iory      (1000)    99440 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/model.py
-drwxrwxr-x   0 iory      (1000) iory      (1000)        0 2020-08-02 09:13:38.000000 scikit-robot-0.0.8/skrobot/optimizers/
--rw-rw-r--   0 iory      (1000) iory      (1000)      697 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/optimizers/cvxopt_solver.py
--rw-rw-r--   0 iory      (1000) iory      (1000)      108 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/optimizers/__init__.py
--rw-rw-r--   0 iory      (1000) iory      (1000)     1732 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/optimizers/quadprog_solver.py
-drwxrwxr-x   0 iory      (1000) iory      (1000)        0 2020-08-02 09:13:38.000000 scikit-robot-0.0.8/skrobot/viewers/
--rw-rw-r--   0 iory      (1000) iory      (1000)      428 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/viewers/__init__.py
--rw-rw-r--   0 iory      (1000) iory      (1000)     4306 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/viewers/_trimesh.py
-drwxrwxr-x   0 iory      (1000) iory      (1000)        0 2020-08-02 09:13:38.000000 scikit-robot-0.0.8/skrobot/apps/
--rw-rw-r--   0 iory      (1000) iory      (1000)        0 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/apps/__init__.py
--rw-rw-r--   0 iory      (1000) iory      (1000)      537 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/apps/visualize_urdf.py
-drwxrwxr-x   0 iory      (1000) iory      (1000)        0 2020-08-02 09:13:38.000000 scikit-robot-0.0.8/skrobot/interfaces/
--rw-rw-r--   0 iory      (1000) iory      (1000)      254 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/interfaces/__init__.py
-drwxrwxr-x   0 iory      (1000) iory      (1000)        0 2020-08-02 09:13:38.000000 scikit-robot-0.0.8/skrobot/interfaces/ros/
--rw-rw-r--   0 iory      (1000) iory      (1000)       96 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/interfaces/ros/__init__.py
--rw-rw-r--   0 iory      (1000) iory      (1000)     4484 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/interfaces/ros/transform_listener.py
--rw-rw-r--   0 iory      (1000) iory      (1000)      634 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/interfaces/ros/panda.py
--rw-rw-r--   0 iory      (1000) iory      (1000)     3371 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/interfaces/ros/tf_utils.py
--rw-rw-r--   0 iory      (1000) iory      (1000)     6667 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/interfaces/ros/pr2.py
--rw-rw-r--   0 iory      (1000) iory      (1000)    23810 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/interfaces/ros/base.py
--rw-rw-r--   0 iory      (1000) iory      (1000)    21819 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/interfaces/ros/move_base.py
--rw-rw-r--   0 iory      (1000) iory      (1000)    14764 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/skrobot/interfaces/_pybullet.py
--rw-rw-r--   0 iory      (1000) iory      (1000)      103 2020-08-02 09:13:38.000000 scikit-robot-0.0.8/setup.cfg
--rw-rw-r--   0 iory      (1000) iory      (1000)       76 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/MANIFEST.in
--rw-rw-r--   0 iory      (1000) iory      (1000)     2578 2020-08-02 09:13:38.000000 scikit-robot-0.0.8/PKG-INFO
--rw-rw-r--   0 iory      (1000) iory      (1000)     2948 2020-08-02 09:13:23.000000 scikit-robot-0.0.8/setup.py
+drwxr-xr-x   0 iory      (1000) iory      (1000)        0 2020-10-16 01:50:19.000000 scikit-robot-0.0.9/
+-rw-r--r--   0 iory      (1000) iory      (1000)       76 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/MANIFEST.in
+-rw-r--r--   0 iory      (1000) iory      (1000)     2578 2020-10-16 01:50:19.000000 scikit-robot-0.0.9/PKG-INFO
+-rw-r--r--   0 iory      (1000) iory      (1000)     1471 2020-08-01 19:48:45.000000 scikit-robot-0.0.9/README.md
+-rw-r--r--   0 iory      (1000) iory      (1000)      286 2020-06-18 07:04:32.000000 scikit-robot-0.0.9/requirements.txt
+drwxr-xr-x   0 iory      (1000) iory      (1000)        0 2020-10-16 01:50:19.000000 scikit-robot-0.0.9/scikit_robot.egg-info/
+-rw-r--r--   0 iory      (1000) iory      (1000)     2578 2020-10-16 01:50:19.000000 scikit-robot-0.0.9/scikit_robot.egg-info/PKG-INFO
+-rw-r--r--   0 iory      (1000) iory      (1000)     2922 2020-10-16 01:50:19.000000 scikit-robot-0.0.9/scikit_robot.egg-info/SOURCES.txt
+-rw-r--r--   0 iory      (1000) iory      (1000)        1 2020-10-16 01:50:19.000000 scikit-robot-0.0.9/scikit_robot.egg-info/dependency_links.txt
+-rw-r--r--   0 iory      (1000) iory      (1000)       69 2020-10-16 01:50:19.000000 scikit-robot-0.0.9/scikit_robot.egg-info/entry_points.txt
+-rw-r--r--   0 iory      (1000) iory      (1000)        1 2020-01-28 14:42:43.000000 scikit-robot-0.0.9/scikit_robot.egg-info/not-zip-safe
+-rw-r--r--   0 iory      (1000) iory      (1000)      226 2020-10-16 01:50:19.000000 scikit-robot-0.0.9/scikit_robot.egg-info/requires.txt
+-rw-r--r--   0 iory      (1000) iory      (1000)        8 2020-10-16 01:50:19.000000 scikit-robot-0.0.9/scikit_robot.egg-info/top_level.txt
+-rw-r--r--   0 iory      (1000) iory      (1000)      103 2020-10-16 01:50:19.000000 scikit-robot-0.0.9/setup.cfg
+-rw-r--r--   0 iory      (1000) iory      (1000)     3093 2020-10-16 01:45:11.000000 scikit-robot-0.0.9/setup.py
+drwxr-xr-x   0 iory      (1000) iory      (1000)        0 2020-10-16 01:50:19.000000 scikit-robot-0.0.9/skrobot/
+-rw-r--r--   0 iory      (1000) iory      (1000)      399 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/__init__.py
+drwxr-xr-x   0 iory      (1000) iory      (1000)        0 2020-10-16 01:50:19.000000 scikit-robot-0.0.9/skrobot/apps/
+-rw-r--r--   0 iory      (1000) iory      (1000)        0 2020-03-27 17:25:49.000000 scikit-robot-0.0.9/skrobot/apps/__init__.py
+-rw-r--r--   0 iory      (1000) iory      (1000)      537 2020-03-27 17:25:49.000000 scikit-robot-0.0.9/skrobot/apps/visualize_urdf.py
+drwxr-xr-x   0 iory      (1000) iory      (1000)        0 2020-10-16 01:50:19.000000 scikit-robot-0.0.9/skrobot/coordinates/
+-rw-r--r--   0 iory      (1000) iory      (1000)      548 2020-08-01 19:48:45.000000 scikit-robot-0.0.9/skrobot/coordinates/__init__.py
+-rw-r--r--   0 iory      (1000) iory      (1000)    39713 2020-06-18 07:04:48.000000 scikit-robot-0.0.9/skrobot/coordinates/base.py
+-rw-r--r--   0 iory      (1000) iory      (1000)    14379 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/coordinates/dual_quaternion.py
+-rw-r--r--   0 iory      (1000) iory      (1000)     4609 2020-08-01 19:48:45.000000 scikit-robot-0.0.9/skrobot/coordinates/geo.py
+-rw-r--r--   0 iory      (1000) iory      (1000)    42544 2020-10-16 01:44:53.000000 scikit-robot-0.0.9/skrobot/coordinates/math.py
+-rw-r--r--   0 iory      (1000) iory      (1000)    12063 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/coordinates/quaternion.py
+drwxr-xr-x   0 iory      (1000) iory      (1000)        0 2020-10-16 01:50:19.000000 scikit-robot-0.0.9/skrobot/data/
+-rw-r--r--   0 iory      (1000) iory      (1000)     1327 2020-02-27 15:05:42.000000 scikit-robot-0.0.9/skrobot/data/__init__.py
+-rw-r--r--   0 iory      (1000) iory      (1000)     1916 2020-01-28 14:43:01.000000 scikit-robot-0.0.9/skrobot/data/__init__.pyc
+drwxr-xr-x   0 iory      (1000) iory      (1000)        0 2020-10-16 01:50:19.000000 scikit-robot-0.0.9/skrobot/data/__pycache__/
+-rw-r--r--   0 iory      (1000) iory      (1000)     1560 2020-02-27 21:17:12.000000 scikit-robot-0.0.9/skrobot/data/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 iory      (1000) iory      (1000)     1566 2020-03-27 16:07:58.000000 scikit-robot-0.0.9/skrobot/data/__pycache__/__init__.cpython-37.pyc
+drwxr-xr-x   0 iory      (1000) iory      (1000)        0 2020-10-16 01:50:19.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/
+-rw-r--r--   0 iory      (1000) iory      (1000)    16001 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/kuka.urdf
+drwxr-xr-x   0 iory      (1000) iory      (1000)        0 2020-10-16 01:50:19.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/
+-rwxr-xr-x   0 iory      (1000) iory      (1000)    10084 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/finger_base_left.stl
+-rwxr-xr-x   0 iory      (1000) iory      (1000)    10084 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/finger_base_right.stl
+-rwxr-xr-x   0 iory      (1000) iory      (1000)     6984 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/finger_tip_left.stl
+-rwxr-xr-x   0 iory      (1000) iory      (1000)     6984 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/finger_tip_right.stl
+-rw-r--r--   0 iory      (1000) iory      (1000)      137 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_0.mtl
+-rw-r--r--   0 iory      (1000) iory      (1000)   185365 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_0.obj
+-rw-r--r--   0 iory      (1000) iory      (1000)   151984 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_0.stl
+-rw-r--r--   0 iory      (1000) iory      (1000)      137 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_1.mtl
+-rw-r--r--   0 iory      (1000) iory      (1000)   170199 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_1.obj
+-rw-r--r--   0 iory      (1000) iory      (1000)   138034 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_1.stl
+-rw-r--r--   0 iory      (1000) iory      (1000)      137 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_2.mtl
+-rw-r--r--   0 iory      (1000) iory      (1000)    86691 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_2.obj
+-rw-r--r--   0 iory      (1000) iory      (1000)    72534 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_2.stl
+-rw-r--r--   0 iory      (1000) iory      (1000)      137 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_3.mtl
+-rw-r--r--   0 iory      (1000) iory      (1000)   115751 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_3.obj
+-rw-r--r--   0 iory      (1000) iory      (1000)    96984 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_3.stl
+-rw-r--r--   0 iory      (1000) iory      (1000)      137 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_4.mtl
+-rw-r--r--   0 iory      (1000) iory      (1000)    93414 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_4.obj
+-rw-r--r--   0 iory      (1000) iory      (1000)    77434 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_4.stl
+-rw-r--r--   0 iory      (1000) iory      (1000)      137 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_5.mtl
+-rw-r--r--   0 iory      (1000) iory      (1000)    76096 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_5.obj
+-rw-r--r--   0 iory      (1000) iory      (1000)    67984 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_5.stl
+-rw-r--r--   0 iory      (1000) iory      (1000)      137 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_6.mtl
+-rw-r--r--   0 iory      (1000) iory      (1000)    68485 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_6.obj
+-rw-r--r--   0 iory      (1000) iory      (1000)    57934 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_6.stl
+-rw-r--r--   0 iory      (1000) iory      (1000)      137 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_7.mtl
+-rw-r--r--   0 iory      (1000) iory      (1000)    92888 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_7.obj
+-rw-r--r--   0 iory      (1000) iory      (1000)    75684 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_7.stl
+drwxr-xr-x   0 iory      (1000) iory      (1000)        0 2020-10-16 01:50:19.000000 scikit-robot-0.0.9/skrobot/interfaces/
+-rw-r--r--   0 iory      (1000) iory      (1000)      254 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/interfaces/__init__.py
+-rw-r--r--   0 iory      (1000) iory      (1000)    14764 2020-08-01 19:48:45.000000 scikit-robot-0.0.9/skrobot/interfaces/_pybullet.py
+drwxr-xr-x   0 iory      (1000) iory      (1000)        0 2020-10-16 01:50:19.000000 scikit-robot-0.0.9/skrobot/interfaces/ros/
+-rw-r--r--   0 iory      (1000) iory      (1000)       96 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/interfaces/ros/__init__.py
+-rw-r--r--   0 iory      (1000) iory      (1000)    23810 2020-08-01 19:48:45.000000 scikit-robot-0.0.9/skrobot/interfaces/ros/base.py
+-rw-r--r--   0 iory      (1000) iory      (1000)    21824 2020-10-16 01:44:53.000000 scikit-robot-0.0.9/skrobot/interfaces/ros/move_base.py
+-rw-r--r--   0 iory      (1000) iory      (1000)      634 2020-02-27 15:05:42.000000 scikit-robot-0.0.9/skrobot/interfaces/ros/panda.py
+-rw-r--r--   0 iory      (1000) iory      (1000)     6667 2020-05-25 00:55:00.000000 scikit-robot-0.0.9/skrobot/interfaces/ros/pr2.py
+-rw-r--r--   0 iory      (1000) iory      (1000)     3371 2020-08-01 19:48:45.000000 scikit-robot-0.0.9/skrobot/interfaces/ros/tf_utils.py
+-rw-r--r--   0 iory      (1000) iory      (1000)     4484 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/interfaces/ros/transform_listener.py
+-rw-r--r--   0 iory      (1000) iory      (1000)     7734 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/interpolator.py
+-rw-r--r--   0 iory      (1000) iory      (1000)    99568 2020-10-16 01:44:53.000000 scikit-robot-0.0.9/skrobot/model.py
+drwxr-xr-x   0 iory      (1000) iory      (1000)        0 2020-10-16 01:50:19.000000 scikit-robot-0.0.9/skrobot/models/
+-rw-r--r--   0 iory      (1000) iory      (1000)      584 2020-10-16 01:44:53.000000 scikit-robot-0.0.9/skrobot/models/__init__.py
+-rw-r--r--   0 iory      (1000) iory      (1000)     2598 2020-02-05 20:22:34.000000 scikit-robot-0.0.9/skrobot/models/fetch.py
+-rw-r--r--   0 iory      (1000) iory      (1000)     2285 2020-02-05 20:22:34.000000 scikit-robot-0.0.9/skrobot/models/kuka.py
+-rw-r--r--   0 iory      (1000) iory      (1000)     1259 2020-02-05 20:22:34.000000 scikit-robot-0.0.9/skrobot/models/panda.py
+-rw-r--r--   0 iory      (1000) iory      (1000)     8164 2020-06-18 07:04:32.000000 scikit-robot-0.0.9/skrobot/models/pr2.py
+-rw-r--r--   0 iory      (1000) iory      (1000)     5522 2020-10-16 01:44:53.000000 scikit-robot-0.0.9/skrobot/models/primitives.py
+-rw-r--r--   0 iory      (1000) iory      (1000)      616 2020-02-05 20:22:34.000000 scikit-robot-0.0.9/skrobot/models/urdf.py
+-rw-r--r--   0 iory      (1000) iory      (1000)     1617 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/optimizer.py
+drwxr-xr-x   0 iory      (1000) iory      (1000)        0 2020-10-16 01:50:19.000000 scikit-robot-0.0.9/skrobot/optimizers/
+-rw-r--r--   0 iory      (1000) iory      (1000)      108 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/optimizers/__init__.py
+-rw-r--r--   0 iory      (1000) iory      (1000)      697 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/optimizers/cvxopt_solver.py
+-rw-r--r--   0 iory      (1000) iory      (1000)     1732 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/optimizers/quadprog_solver.py
+drwxr-xr-x   0 iory      (1000) iory      (1000)        0 2020-10-16 01:50:19.000000 scikit-robot-0.0.9/skrobot/utils/
+-rw-r--r--   0 iory      (1000) iory      (1000)       52 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/utils/__init__.py
+-rw-r--r--   0 iory      (1000) iory      (1000)      127 2020-01-28 14:42:38.000000 scikit-robot-0.0.9/skrobot/utils/listify.py
+-rw-r--r--   0 iory      (1000) iory      (1000)    96734 2020-05-25 00:55:00.000000 scikit-robot-0.0.9/skrobot/utils/urdf.py
+drwxr-xr-x   0 iory      (1000) iory      (1000)        0 2020-10-16 01:50:19.000000 scikit-robot-0.0.9/skrobot/viewers/
+-rw-r--r--   0 iory      (1000) iory      (1000)      428 2020-02-27 15:05:42.000000 scikit-robot-0.0.9/skrobot/viewers/__init__.py
+-rw-r--r--   0 iory      (1000) iory      (1000)     4306 2020-02-27 15:05:42.000000 scikit-robot-0.0.9/skrobot/viewers/_trimesh.py
```

### Comparing `scikit-robot-0.0.8/README.md` & `scikit-robot-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/scikit_robot.egg-info/SOURCES.txt` & `scikit-robot-0.0.9/scikit_robot.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 skrobot/coordinates/__init__.py
 skrobot/coordinates/base.py
 skrobot/coordinates/dual_quaternion.py
 skrobot/coordinates/geo.py
 skrobot/coordinates/math.py
 skrobot/coordinates/quaternion.py
 skrobot/data/__init__.py
+skrobot/data/__init__.pyc
+skrobot/data/__pycache__/__init__.cpython-36.pyc
+skrobot/data/__pycache__/__init__.cpython-37.pyc
 skrobot/data/kuka_description/kuka.urdf
 skrobot/data/kuka_description/meshes/finger_base_left.stl
 skrobot/data/kuka_description/meshes/finger_base_right.stl
 skrobot/data/kuka_description/meshes/finger_tip_left.stl
 skrobot/data/kuka_description/meshes/finger_tip_right.stl
 skrobot/data/kuka_description/meshes/link_0.mtl
 skrobot/data/kuka_description/meshes/link_0.obj
```

### Comparing `scikit-robot-0.0.8/scikit_robot.egg-info/PKG-INFO` & `scikit-robot-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-robot
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Flexible Framework for Robot Control in Python
 Home-page: https://github.com/iory/scikit-robot
 Author: iory
 Author-email: ab.ioryz@gmail.com
 License: MIT
 Description: # scikit-robot: A Flexible Framework for Robot Control in Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scikit-robot Version: 0.0.8 Summary: A Flexible
+Metadata-Version: 2.1 Name: scikit-robot Version: 0.0.9 Summary: A Flexible
 Framework for Robot Control in Python Home-page: https://github.com/iory/
 scikit-robot Author: iory Author-email: ab.ioryz@gmail.com License: MIT
 Description: # scikit-robot: A Flexible Framework for Robot Control in Python
 [![Build Status](https://travis-ci.com/iory/scikit-
 robot.svg?token=zM5rExyvuRoJThsnqHAF&branch=master)](https://travis-ci.com/
 iory/scikit-robot)
 *** Documentation | Installation | Quick_Start | Python_API | Contribute ***
```

### Comparing `scikit-robot-0.0.8/skrobot/interpolator.py` & `scikit-robot-0.0.9/skrobot/interpolator.py`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/utils/urdf.py` & `scikit-robot-0.0.9/skrobot/utils/urdf.py`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/models/__init__.py` & `scikit-robot-0.0.9/skrobot/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,13 +3,14 @@
 from skrobot.models.primitives import Annulus
 from skrobot.models.primitives import Axis
 from skrobot.models.primitives import Box
 from skrobot.models.primitives import CameraMarker
 from skrobot.models.primitives import Cone
 from skrobot.models.primitives import Cylinder
 from skrobot.models.primitives import MeshLink
+from skrobot.models.primitives import PointCloudLink
 from skrobot.models.primitives import Sphere
 
 from skrobot.models.fetch import Fetch
 from skrobot.models.kuka import Kuka
 from skrobot.models.panda import Panda
 from skrobot.models.pr2 import PR2
```

### Comparing `scikit-robot-0.0.8/skrobot/models/panda.py` & `scikit-robot-0.0.9/skrobot/models/panda.py`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/models/kuka.py` & `scikit-robot-0.0.9/skrobot/models/kuka.py`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/models/primitives.py` & `scikit-robot-0.0.9/skrobot/models/primitives.py`

 * *Files 6% similar despite different names*

```diff
@@ -154,7 +154,20 @@
                  visual_mesh=None,
                  pos=(0, 0, 0), rot=np.eye(3), name=None):
         if name is None:
             name = 'meshlink_{}'.format(str(uuid.uuid1()).replace('-', '_'))
 
         super(MeshLink, self).__init__(pos=pos, rot=rot, name=name)
         self.visual_mesh = visual_mesh
+
+
+class PointCloudLink(model_module.Link):
+
+    def __init__(self,
+                 visual_mesh=None,
+                 pos=(0, 0, 0), rot=np.eye(3), name=None):
+        if name is None:
+            name = 'pointcloudlink_{}'.format(
+                str(uuid.uuid1()).replace('-', '_'))
+
+        super(PointCloudLink, self).__init__(pos=pos, rot=rot, name=name)
+        self.visual_mesh = visual_mesh
```

### Comparing `scikit-robot-0.0.8/skrobot/models/urdf.py` & `scikit-robot-0.0.9/skrobot/models/urdf.py`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/models/pr2.py` & `scikit-robot-0.0.9/skrobot/models/pr2.py`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/models/fetch.py` & `scikit-robot-0.0.9/skrobot/models/fetch.py`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/coordinates/__init__.py` & `scikit-robot-0.0.9/skrobot/coordinates/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/coordinates/geo.py` & `scikit-robot-0.0.9/skrobot/coordinates/geo.py`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/coordinates/dual_quaternion.py` & `scikit-robot-0.0.9/skrobot/coordinates/dual_quaternion.py`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/coordinates/math.py` & `scikit-robot-0.0.9/skrobot/coordinates/math.py`

 * *Files 1% similar despite different names*

```diff
@@ -930,15 +930,15 @@
         third_axis = np.cross(e2, e1)
     e3 = normalize_vector(
         third_axis - np.dot(third_axis, e1) * e1 - np.dot(third_axis, e2) * e2)
     first_index = ord(axes[0]) - ord('x')
     second_index = ord(axes[1]) - ord('x')
     third_index = ((first_index + 1) ^ (second_index + 1)) - 1
     indices = [first_index, second_index, third_index]
-    return np.vstack([e1, e2, e3])[indices].T
+    return np.vstack([e1, e2, e3])[np.argsort(indices)].T
 
 
 def rodrigues(axis, theta=None):
     """Rodrigues formula.
 
     See: `Rodrigues' rotation formula - Wikipedia
     <https://en.wikipedia.org/wiki/Rodrigues%27_rotation_formula>`_.
```

### Comparing `scikit-robot-0.0.8/skrobot/coordinates/base.py` & `scikit-robot-0.0.9/skrobot/coordinates/base.py`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/coordinates/quaternion.py` & `scikit-robot-0.0.9/skrobot/coordinates/quaternion.py`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/optimizer.py` & `scikit-robot-0.0.9/skrobot/optimizer.py`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/data/__init__.py` & `scikit-robot-0.0.9/skrobot/data/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/finger_base_right.stl` & `scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/finger_base_right.stl`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_4.stl` & `scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_4.stl`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_3.obj` & `scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_3.obj`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/finger_tip_right.stl` & `scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/finger_tip_right.stl`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_4.obj` & `scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_4.obj`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/finger_base_left.stl` & `scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/finger_base_left.stl`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_0.obj` & `scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_0.obj`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_5.obj` & `scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_5.obj`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_6.obj` & `scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_6.obj`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_6.stl` & `scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_6.stl`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_1.stl` & `scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_1.stl`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_1.obj` & `scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_1.obj`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_7.obj` & `scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_7.obj`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_0.stl` & `scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_0.stl`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_2.obj` & `scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_2.obj`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_3.stl` & `scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_3.stl`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_7.stl` & `scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_7.stl`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/finger_tip_left.stl` & `scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/finger_tip_left.stl`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_2.stl` & `scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_2.stl`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/data/kuka_description/meshes/link_5.stl` & `scikit-robot-0.0.9/skrobot/data/kuka_description/meshes/link_5.stl`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/data/kuka_description/kuka.urdf` & `scikit-robot-0.0.9/skrobot/data/kuka_description/kuka.urdf`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/model.py` & `scikit-robot-0.0.9/skrobot/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -600,26 +600,28 @@
 
     @visual_mesh.setter
     def visual_mesh(self, mesh):
         """Setter of visual mesh
 
         Parameters
         ----------
-        mesh : None, trimesh.Trimesh, sequence of trimesh.Trimesh, or str
+        mesh : None, trimesh.Trimesh, sequence of trimesh.Trimesh,
+               trimesh.points.PointCloud or str
             A set of visual meshes for the link in the link frame.
         """
         if not (mesh is None
                 or isinstance(mesh, trimesh.Trimesh)
                 or (isinstance(mesh, collections.Sequence)
                     and all(isinstance(m, trimesh.Trimesh) for m in mesh))
+                or isinstance(mesh, trimesh.points.PointCloud)
                 or isinstance(mesh, str)):
             raise TypeError(
                 'mesh must be None, trimesh.Trimesh, sequence of '
-                'trimesh.Trimesh, or path of mesh file, but got: {}'.format(
-                    type(mesh)))
+                'trimesh.Trimesh, trimesh.points.PointCloud '
+                'or path of mesh file, but got: {}'.format(type(mesh)))
         if isinstance(mesh, str):
             mesh = trimesh.load(mesh)
         self._visual_mesh = mesh
 
 
 class CascadedLink(CascadedCoords):
```

### Comparing `scikit-robot-0.0.8/skrobot/optimizers/cvxopt_solver.py` & `scikit-robot-0.0.9/skrobot/optimizers/cvxopt_solver.py`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/optimizers/quadprog_solver.py` & `scikit-robot-0.0.9/skrobot/optimizers/quadprog_solver.py`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/viewers/_trimesh.py` & `scikit-robot-0.0.9/skrobot/viewers/_trimesh.py`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/apps/visualize_urdf.py` & `scikit-robot-0.0.9/skrobot/apps/visualize_urdf.py`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/interfaces/ros/transform_listener.py` & `scikit-robot-0.0.9/skrobot/interfaces/ros/transform_listener.py`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/interfaces/ros/panda.py` & `scikit-robot-0.0.9/skrobot/interfaces/ros/panda.py`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/interfaces/ros/tf_utils.py` & `scikit-robot-0.0.9/skrobot/interfaces/ros/tf_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/interfaces/ros/pr2.py` & `scikit-robot-0.0.9/skrobot/interfaces/ros/pr2.py`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/interfaces/ros/base.py` & `scikit-robot-0.0.9/skrobot/interfaces/ros/base.py`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/skrobot/interfaces/ros/move_base.py` & `scikit-robot-0.0.9/skrobot/interfaces/ros/move_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -440,15 +440,15 @@
         send-action [ send message to action server, it means robot will move ]
 
         """
         if len(trajectory_points) != len(time_list):
             raise ValueError
         while self.odom_msg is None:
             rospy.sleep(0.01)
-        odom_coords = geometry_pose_to_coords(self.odom_msg.pose)
+        odom_coords = geometry_pose_to_coords(self.odom_msg.pose.pose)
         goal = control_msgs.msg.FollowJointTrajectoryActionGoal()
         msg = trajectory_msgs.msg.JointTrajectory()
         msg.joint_names = self.move_base_trajectory_joint_names
         if start_time is not None:
             msg.header.stamp = start_time
         else:
             msg.header.stamp = rospy.Time.now()
```

### Comparing `scikit-robot-0.0.8/skrobot/interfaces/_pybullet.py` & `scikit-robot-0.0.9/skrobot/interfaces/_pybullet.py`

 * *Files identical despite different names*

### Comparing `scikit-robot-0.0.8/PKG-INFO` & `scikit-robot-0.0.9/scikit_robot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-robot
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Flexible Framework for Robot Control in Python
 Home-page: https://github.com/iory/scikit-robot
 Author: iory
 Author-email: ab.ioryz@gmail.com
 License: MIT
 Description: # scikit-robot: A Flexible Framework for Robot Control in Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scikit-robot Version: 0.0.8 Summary: A Flexible
+Metadata-Version: 2.1 Name: scikit-robot Version: 0.0.9 Summary: A Flexible
 Framework for Robot Control in Python Home-page: https://github.com/iory/
 scikit-robot Author: iory Author-email: ab.ioryz@gmail.com License: MIT
 Description: # scikit-robot: A Flexible Framework for Robot Control in Python
 [![Build Status](https://travis-ci.com/iory/scikit-
 robot.svg?token=zM5rExyvuRoJThsnqHAF&branch=master)](https://travis-ci.com/
 iory/scikit-robot)
 *** Documentation | Installation | Quick_Start | Python_API | Contribute ***
```

### Comparing `scikit-robot-0.0.8/setup.py` & `scikit-robot-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import print_function
 
 import distutils.spawn
 import os
+import platform
 import shlex
 import subprocess
 import sys
 
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = '0.0.8'
+version = '0.0.9'
 
 
 if sys.argv[-1] == 'release':
     if not distutils.spawn.find_executable('twine'):
         print(
             'Please install twine:\n\n\tpip install twine\n',
             file=sys.stderr,
@@ -59,14 +60,19 @@
     lock = [('pyglet', '1.4.10')]
     for name, version in lock:
         # remove version-free requirements
         install_requires.remove(name)
         # add working version locked requirements
         install_requires.append('{}=={}'.format(name, version))
 
+uname = platform.uname()[0]
+if uname == 'Darwin':
+    # python-fcl could not install.
+    install_requires.remove('python-fcl')
+
 setup(
     name='scikit-robot',
     version=version,
     description='A Flexible Framework for Robot Control in Python',
     author='iory',
     author_email='ab.ioryz@gmail.com',
     url='https://github.com/iory/scikit-robot',
```

