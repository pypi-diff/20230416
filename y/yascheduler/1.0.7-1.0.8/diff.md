# Comparing `tmp/yascheduler-1.0.7.tar.gz` & `tmp/yascheduler-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yascheduler-1.0.7.tar", last modified: Thu Mar  2 20:55:54 2023, max compression
+gzip compressed data, was "yascheduler-1.0.8.tar", last modified: Sun Apr 16 16:14:21 2023, max compression
```

## Comparing `yascheduler-1.0.7.tar` & `yascheduler-1.0.8.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 20:55:54.947363 yascheduler-1.0.7/
--rw-r--r--   0 root         (0) root         (0)     1134 2023-03-02 20:55:54.947363 yascheduler-1.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10229 2022-12-16 20:27:02.000000 yascheduler-1.0.7/README.md
--rw-r--r--   0 root         (0) root         (0)      102 2023-03-02 20:55:54.947363 yascheduler-1.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1972 2022-08-17 12:59:28.000000 yascheduler-1.0.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 20:55:54.939363 yascheduler-1.0.7/yascheduler/
--rw-r--r--   0 root         (0) root         (0)      228 2022-07-30 22:43:35.000000 yascheduler-1.0.7/yascheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)       22 2022-08-17 12:59:28.000000 yascheduler-1.0.7/yascheduler/__version__.py
--rw-r--r--   0 root         (0) root         (0)     4747 2022-09-26 15:10:05.000000 yascheduler-1.0.7/yascheduler/aiida_plugin.py
--rw-r--r--   0 root         (0) root         (0)     2695 2022-08-01 14:38:59.000000 yascheduler-1.0.7/yascheduler/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 20:55:54.943363 yascheduler-1.0.7/yascheduler/clouds/
--rw-r--r--   0 root         (0) root         (0)      170 2022-07-30 22:43:35.000000 yascheduler-1.0.7/yascheduler/clouds/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2981 2022-08-02 17:38:08.000000 yascheduler-1.0.7/yascheduler/clouds/adapters.py
--rw-r--r--   0 root         (0) root         (0)     8736 2022-08-02 17:38:08.000000 yascheduler-1.0.7/yascheduler/clouds/az.py
--rw-r--r--   0 root         (0) root         (0)     6867 2022-08-16 14:53:47.000000 yascheduler-1.0.7/yascheduler/clouds/cloud_api.py
--rw-r--r--   0 root         (0) root         (0)     6821 2022-08-16 14:53:47.000000 yascheduler-1.0.7/yascheduler/clouds/cloud_api_manager.py
--rw-r--r--   0 root         (0) root         (0)     3282 2022-08-02 17:38:08.000000 yascheduler-1.0.7/yascheduler/clouds/hetzner.py
--rw-r--r--   0 root         (0) root         (0)     5802 2022-08-16 14:53:47.000000 yascheduler-1.0.7/yascheduler/clouds/protocols.py
--rw-r--r--   0 root         (0) root         (0)     2831 2022-08-02 17:38:08.000000 yascheduler-1.0.7/yascheduler/clouds/upcloud.py
--rw-r--r--   0 root         (0) root         (0)      763 2022-08-02 17:38:08.000000 yascheduler-1.0.7/yascheduler/clouds/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 20:55:54.943363 yascheduler-1.0.7/yascheduler/config/
--rw-r--r--   0 root         (0) root         (0)      731 2022-07-30 22:43:35.000000 yascheduler-1.0.7/yascheduler/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6408 2022-08-01 13:33:43.000000 yascheduler-1.0.7/yascheduler/config/cloud.py
--rw-r--r--   0 root         (0) root         (0)     2438 2022-08-17 12:59:28.000000 yascheduler-1.0.7/yascheduler/config/config.py
--rw-r--r--   0 root         (0) root         (0)      807 2022-07-30 22:43:35.000000 yascheduler-1.0.7/yascheduler/config/db.py
--rw-r--r--   0 root         (0) root         (0)     4917 2022-08-01 15:25:53.000000 yascheduler-1.0.7/yascheduler/config/engine.py
--rw-r--r--   0 root         (0) root         (0)     2635 2022-07-30 22:43:35.000000 yascheduler-1.0.7/yascheduler/config/engine_repository.py
--rw-r--r--   0 root         (0) root         (0)     2844 2022-08-02 17:38:08.000000 yascheduler-1.0.7/yascheduler/config/local.py
--rw-r--r--   0 root         (0) root         (0)     1294 2022-07-30 22:43:35.000000 yascheduler-1.0.7/yascheduler/config/remote.py
--rw-r--r--   0 root         (0) root         (0)      484 2022-07-30 22:43:35.000000 yascheduler-1.0.7/yascheduler/config/utils.py
--rw-r--r--   0 root         (0) root         (0)      200 2022-07-30 22:43:26.000000 yascheduler-1.0.7/yascheduler/daemon_systemd.py
--rw-r--r--   0 root         (0) root         (0)      864 2022-08-01 13:33:43.000000 yascheduler-1.0.7/yascheduler/daemon_sysv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 20:55:54.947363 yascheduler-1.0.7/yascheduler/data/
--rw-r--r--   0 root         (0) root         (0)      360 2023-02-09 18:58:39.000000 yascheduler-1.0.7/yascheduler/data/schema.sql
--rw-r--r--   0 root         (0) root         (0)     1493 2022-07-30 22:43:26.000000 yascheduler-1.0.7/yascheduler/data/yascheduler.conf
--rw-r--r--   0 root         (0) root         (0)      664 2022-07-30 22:43:35.000000 yascheduler-1.0.7/yascheduler/data/yascheduler.service
--rwxr-xr-x   0 root         (0) root         (0)     1832 2022-07-30 22:43:35.000000 yascheduler-1.0.7/yascheduler/data/yascheduler.sh
--rw-r--r--   0 root         (0) root         (0)    12108 2022-08-01 13:33:43.000000 yascheduler-1.0.7/yascheduler/db.py
--rw-r--r--   0 root         (0) root         (0)     1651 2022-08-01 13:33:43.000000 yascheduler-1.0.7/yascheduler/queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 20:55:54.947363 yascheduler-1.0.7/yascheduler/remote_machine/
--rw-r--r--   0 root         (0) root         (0)      417 2022-07-30 22:43:35.000000 yascheduler-1.0.7/yascheduler/remote_machine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3271 2022-08-17 12:59:28.000000 yascheduler-1.0.7/yascheduler/remote_machine/adapters.py
--rw-r--r--   0 root         (0) root         (0)     2338 2022-08-17 12:59:28.000000 yascheduler-1.0.7/yascheduler/remote_machine/checks.py
--rw-r--r--   0 root         (0) root         (0)     1213 2022-07-30 22:43:35.000000 yascheduler-1.0.7/yascheduler/remote_machine/common.py
--rw-r--r--   0 root         (0) root         (0)       72 2022-07-30 22:43:26.000000 yascheduler-1.0.7/yascheduler/remote_machine/exc.py
--rw-r--r--   0 root         (0) root         (0)     6980 2022-08-03 22:43:25.000000 yascheduler-1.0.7/yascheduler/remote_machine/linux_methods.py
--rw-r--r--   0 root         (0) root         (0)     8641 2022-08-16 21:24:49.000000 yascheduler-1.0.7/yascheduler/remote_machine/protocol.py
--rw-r--r--   0 root         (0) root         (0)    13264 2022-08-17 15:28:14.000000 yascheduler-1.0.7/yascheduler/remote_machine/remote_machine.py
--rw-r--r--   0 root         (0) root         (0)     2655 2022-07-30 22:43:35.000000 yascheduler-1.0.7/yascheduler/remote_machine/remote_machine_repository.py
--rw-r--r--   0 root         (0) root         (0)     7288 2022-08-03 22:43:25.000000 yascheduler-1.0.7/yascheduler/remote_machine/windows_methods.py
--rwxr-xr-x   0 root         (0) root         (0)    26280 2022-09-23 17:45:29.000000 yascheduler-1.0.7/yascheduler/scheduler.py
--rw-r--r--   0 root         (0) root         (0)      435 2022-08-01 13:33:43.000000 yascheduler-1.0.7/yascheduler/time.py
--rw-r--r--   0 root         (0) root         (0)    15681 2022-09-26 15:02:04.000000 yascheduler-1.0.7/yascheduler/utils.py
--rw-r--r--   0 root         (0) root         (0)      263 2022-08-01 13:33:43.000000 yascheduler-1.0.7/yascheduler/variables.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 20:55:54.939363 yascheduler-1.0.7/yascheduler.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1134 2023-03-02 20:55:54.000000 yascheduler-1.0.7/yascheduler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1621 2023-03-02 20:55:54.000000 yascheduler-1.0.7/yascheduler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-02 20:55:54.000000 yascheduler-1.0.7/yascheduler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      323 2023-03-02 20:55:54.000000 yascheduler-1.0.7/yascheduler.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      235 2023-03-02 20:55:54.000000 yascheduler-1.0.7/yascheduler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-03-02 20:55:54.000000 yascheduler-1.0.7/yascheduler.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:14:21.667817 yascheduler-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-04-16 16:14:21.667817 yascheduler-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10424 2023-03-08 16:11:57.000000 yascheduler-1.0.8/README.md
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-16 16:14:21.667817 yascheduler-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1972 2022-08-17 12:59:28.000000 yascheduler-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:14:21.659817 yascheduler-1.0.8/yascheduler/
+-rw-r--r--   0 root         (0) root         (0)      228 2022-07-30 22:43:35.000000 yascheduler-1.0.8/yascheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-03-10 23:58:05.000000 yascheduler-1.0.8/yascheduler/__version__.py
+-rw-r--r--   0 root         (0) root         (0)     4747 2022-09-26 15:10:05.000000 yascheduler-1.0.8/yascheduler/aiida_plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2022-08-01 14:38:59.000000 yascheduler-1.0.8/yascheduler/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:14:21.659817 yascheduler-1.0.8/yascheduler/clouds/
+-rw-r--r--   0 root         (0) root         (0)      170 2022-07-30 22:43:35.000000 yascheduler-1.0.8/yascheduler/clouds/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2981 2022-08-02 17:38:08.000000 yascheduler-1.0.8/yascheduler/clouds/adapters.py
+-rw-r--r--   0 root         (0) root         (0)     8736 2022-08-02 17:38:08.000000 yascheduler-1.0.8/yascheduler/clouds/az.py
+-rw-r--r--   0 root         (0) root         (0)     6867 2022-08-16 14:53:47.000000 yascheduler-1.0.8/yascheduler/clouds/cloud_api.py
+-rw-r--r--   0 root         (0) root         (0)     6821 2022-08-16 14:53:47.000000 yascheduler-1.0.8/yascheduler/clouds/cloud_api_manager.py
+-rw-r--r--   0 root         (0) root         (0)     3282 2022-08-02 17:38:08.000000 yascheduler-1.0.8/yascheduler/clouds/hetzner.py
+-rw-r--r--   0 root         (0) root         (0)     5802 2022-08-16 14:53:47.000000 yascheduler-1.0.8/yascheduler/clouds/protocols.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2022-08-02 17:38:08.000000 yascheduler-1.0.8/yascheduler/clouds/upcloud.py
+-rw-r--r--   0 root         (0) root         (0)      763 2022-08-02 17:38:08.000000 yascheduler-1.0.8/yascheduler/clouds/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:14:21.663817 yascheduler-1.0.8/yascheduler/config/
+-rw-r--r--   0 root         (0) root         (0)      731 2022-07-30 22:43:35.000000 yascheduler-1.0.8/yascheduler/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6408 2022-08-01 13:33:43.000000 yascheduler-1.0.8/yascheduler/config/cloud.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2022-08-17 12:59:28.000000 yascheduler-1.0.8/yascheduler/config/config.py
+-rw-r--r--   0 root         (0) root         (0)      807 2022-07-30 22:43:35.000000 yascheduler-1.0.8/yascheduler/config/db.py
+-rw-r--r--   0 root         (0) root         (0)     4917 2022-08-01 15:25:53.000000 yascheduler-1.0.8/yascheduler/config/engine.py
+-rw-r--r--   0 root         (0) root         (0)     2635 2022-07-30 22:43:35.000000 yascheduler-1.0.8/yascheduler/config/engine_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2844 2022-08-02 17:38:08.000000 yascheduler-1.0.8/yascheduler/config/local.py
+-rw-r--r--   0 root         (0) root         (0)     1294 2022-07-30 22:43:35.000000 yascheduler-1.0.8/yascheduler/config/remote.py
+-rw-r--r--   0 root         (0) root         (0)      484 2022-07-30 22:43:35.000000 yascheduler-1.0.8/yascheduler/config/utils.py
+-rw-r--r--   0 root         (0) root         (0)      200 2022-07-30 22:43:26.000000 yascheduler-1.0.8/yascheduler/daemon_systemd.py
+-rw-r--r--   0 root         (0) root         (0)      864 2022-08-01 13:33:43.000000 yascheduler-1.0.8/yascheduler/daemon_sysv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:14:21.663817 yascheduler-1.0.8/yascheduler/data/
+-rw-r--r--   0 root         (0) root         (0)      360 2023-02-09 18:58:39.000000 yascheduler-1.0.8/yascheduler/data/schema.sql
+-rw-r--r--   0 root         (0) root         (0)     1493 2022-07-30 22:43:26.000000 yascheduler-1.0.8/yascheduler/data/yascheduler.conf
+-rw-r--r--   0 root         (0) root         (0)      664 2022-07-30 22:43:35.000000 yascheduler-1.0.8/yascheduler/data/yascheduler.service
+-rwxr-xr-x   0 root         (0) root         (0)     1832 2022-07-30 22:43:35.000000 yascheduler-1.0.8/yascheduler/data/yascheduler.sh
+-rw-r--r--   0 root         (0) root         (0)    12108 2022-08-01 13:33:43.000000 yascheduler-1.0.8/yascheduler/db.py
+-rw-r--r--   0 root         (0) root         (0)     1651 2022-08-01 13:33:43.000000 yascheduler-1.0.8/yascheduler/queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:14:21.667817 yascheduler-1.0.8/yascheduler/remote_machine/
+-rw-r--r--   0 root         (0) root         (0)      417 2022-07-30 22:43:35.000000 yascheduler-1.0.8/yascheduler/remote_machine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3271 2022-08-17 12:59:28.000000 yascheduler-1.0.8/yascheduler/remote_machine/adapters.py
+-rw-r--r--   0 root         (0) root         (0)     2338 2022-08-17 12:59:28.000000 yascheduler-1.0.8/yascheduler/remote_machine/checks.py
+-rw-r--r--   0 root         (0) root         (0)     1213 2022-07-30 22:43:35.000000 yascheduler-1.0.8/yascheduler/remote_machine/common.py
+-rw-r--r--   0 root         (0) root         (0)       72 2022-07-30 22:43:26.000000 yascheduler-1.0.8/yascheduler/remote_machine/exc.py
+-rw-r--r--   0 root         (0) root         (0)     6980 2022-08-03 22:43:25.000000 yascheduler-1.0.8/yascheduler/remote_machine/linux_methods.py
+-rw-r--r--   0 root         (0) root         (0)     8641 2022-08-16 21:24:49.000000 yascheduler-1.0.8/yascheduler/remote_machine/protocol.py
+-rw-r--r--   0 root         (0) root         (0)    13207 2023-03-10 23:58:05.000000 yascheduler-1.0.8/yascheduler/remote_machine/remote_machine.py
+-rw-r--r--   0 root         (0) root         (0)     2655 2022-07-30 22:43:35.000000 yascheduler-1.0.8/yascheduler/remote_machine/remote_machine_repository.py
+-rw-r--r--   0 root         (0) root         (0)     7288 2022-08-03 22:43:25.000000 yascheduler-1.0.8/yascheduler/remote_machine/windows_methods.py
+-rwxr-xr-x   0 root         (0) root         (0)    26345 2023-03-10 23:59:11.000000 yascheduler-1.0.8/yascheduler/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)      435 2022-08-01 13:33:43.000000 yascheduler-1.0.8/yascheduler/time.py
+-rw-r--r--   0 root         (0) root         (0)    15688 2023-03-08 16:11:57.000000 yascheduler-1.0.8/yascheduler/utils.py
+-rw-r--r--   0 root         (0) root         (0)      263 2022-08-01 13:33:43.000000 yascheduler-1.0.8/yascheduler/variables.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:14:21.659817 yascheduler-1.0.8/yascheduler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-04-16 16:14:21.000000 yascheduler-1.0.8/yascheduler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-04-16 16:14:21.000000 yascheduler-1.0.8/yascheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 16:14:21.000000 yascheduler-1.0.8/yascheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      323 2023-04-16 16:14:21.000000 yascheduler-1.0.8/yascheduler.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      235 2023-04-16 16:14:21.000000 yascheduler-1.0.8/yascheduler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-16 16:14:21.000000 yascheduler-1.0.8/yascheduler.egg-info/top_level.txt
```

### Comparing `yascheduler-1.0.7/PKG-INFO` & `yascheduler-1.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: yascheduler
-Version: 1.0.7
+Version: 1.0.8
 Summary: Yet another computing scheduler and cloud orchestration engine
 Home-page: https://github.com/tilde-lab/yascheduler
 Author: Sergey Korolev, Evgeny Blokhin, Andrey Sobolev
 Author-email: eb@tilde.pro
 License: MIT
 Description: *Yascheduler* is a job scheduler designed for submitting scientific simulations to the VM clouds and copying back their results.
 Platform: UNKNOWN
```

### Comparing `yascheduler-1.0.7/README.md` & `yascheduler-1.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Yet another computing scheduler & cloud orchestration engine
 
+[![DOI](https://zenodo.org/badge/222936146.svg)](https://doi.org/10.5281/zenodo.7693555)
+[![PyPI](https://img.shields.io/pypi/v/yascheduler.svg?style=flat)](https://pypi.org/project/yascheduler)
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Ftilde-lab%2Fyascheduler.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Ftilde-lab%2Fyascheduler?ref=badge_shield)
 
 **Yascheduler** is a simple job scheduler designed for submitting scientific
 calculations and copying back the results from the computing clouds.
 
 Currently it supports several scientific simulation codes in chemistry
 and solid state physics.
```

### Comparing `yascheduler-1.0.7/setup.py` & `yascheduler-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/aiida_plugin.py` & `yascheduler-1.0.8/yascheduler/aiida_plugin.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/client.py` & `yascheduler-1.0.8/yascheduler/client.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/clouds/adapters.py` & `yascheduler-1.0.8/yascheduler/clouds/adapters.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/clouds/az.py` & `yascheduler-1.0.8/yascheduler/clouds/az.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/clouds/cloud_api.py` & `yascheduler-1.0.8/yascheduler/clouds/cloud_api.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/clouds/cloud_api_manager.py` & `yascheduler-1.0.8/yascheduler/clouds/cloud_api_manager.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/clouds/hetzner.py` & `yascheduler-1.0.8/yascheduler/clouds/hetzner.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/clouds/protocols.py` & `yascheduler-1.0.8/yascheduler/clouds/protocols.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/clouds/upcloud.py` & `yascheduler-1.0.8/yascheduler/clouds/upcloud.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/clouds/utils.py` & `yascheduler-1.0.8/yascheduler/clouds/utils.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/config/__init__.py` & `yascheduler-1.0.8/yascheduler/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/config/cloud.py` & `yascheduler-1.0.8/yascheduler/config/cloud.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/config/config.py` & `yascheduler-1.0.8/yascheduler/config/config.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/config/db.py` & `yascheduler-1.0.8/yascheduler/config/db.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/config/engine.py` & `yascheduler-1.0.8/yascheduler/config/engine.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/config/engine_repository.py` & `yascheduler-1.0.8/yascheduler/config/engine_repository.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/config/local.py` & `yascheduler-1.0.8/yascheduler/config/local.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/config/remote.py` & `yascheduler-1.0.8/yascheduler/config/remote.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/daemon_sysv.py` & `yascheduler-1.0.8/yascheduler/daemon_sysv.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/data/yascheduler.conf` & `yascheduler-1.0.8/yascheduler/data/yascheduler.conf`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/data/yascheduler.service` & `yascheduler-1.0.8/yascheduler/data/yascheduler.service`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/data/yascheduler.sh` & `yascheduler-1.0.8/yascheduler/data/yascheduler.sh`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/db.py` & `yascheduler-1.0.8/yascheduler/db.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/queue.py` & `yascheduler-1.0.8/yascheduler/queue.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/remote_machine/adapters.py` & `yascheduler-1.0.8/yascheduler/remote_machine/adapters.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/remote_machine/checks.py` & `yascheduler-1.0.8/yascheduler/remote_machine/checks.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/remote_machine/common.py` & `yascheduler-1.0.8/yascheduler/remote_machine/common.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/remote_machine/linux_methods.py` & `yascheduler-1.0.8/yascheduler/remote_machine/linux_methods.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/remote_machine/protocol.py` & `yascheduler-1.0.8/yascheduler/remote_machine/protocol.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/remote_machine/remote_machine.py` & `yascheduler-1.0.8/yascheduler/remote_machine/remote_machine.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,21 +397,19 @@
         """
         Start occupancy checker for engine.
         """
         # remove old tasks
         self.jobs.difference_update([t for t in self.jobs if t.done()])
 
         async def occupancy_checker():
-            while not self.cancellation_event.is_set() and self.meta.busy:
+            while not self.cancellation_event.is_set() and self.meta.busy is not False:
                 try:
-                    busy = await asyncio.wait_for(
+                    self.meta.busy = await asyncio.wait_for(
                         self.occupancy_check(engine), timeout=engine.sleep_interval
                     )
-                    if not busy:
-                        self.meta.busy = False
                 except asyncio.TimeoutError:
                     t = "Engine {} busy check timeouted on {}"
                     self.log.warning(t.format(engine.name, self.hostname))
                 except Exception as err:
                     self.log.warning(err)
                 await asyncio.sleep(engine.sleep_interval)
```

### Comparing `yascheduler-1.0.7/yascheduler/remote_machine/remote_machine_repository.py` & `yascheduler-1.0.8/yascheduler/remote_machine/remote_machine_repository.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/remote_machine/windows_methods.py` & `yascheduler-1.0.8/yascheduler/remote_machine/windows_methods.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.7/yascheduler/scheduler.py` & `yascheduler-1.0.8/yascheduler/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,16 +236,16 @@
         self,
         machine: PRemoteMachine,
         engine: Engine,
         task: TaskModel,
     ) -> bool:
         "Run task on remote machine"
         self.log.info(
-            "Submitting task_id=%s %s to %s"
-            % (task.task_id, task.label, machine.hostname)
+            "Submitting task_id=%s %s with %s to %s"
+            % (task.task_id, task.label, engine.name, machine.hostname)
         )
         assert task.metadata.get("remote_folder")
         machine.meta.busy = True
         remote_folder = machine.path(task.metadata["remote_folder"])
 
         async with machine.sftp() as sftp:
             try:
@@ -375,15 +375,17 @@
                         sftp_errors.append((out_file, err))
                         self.log.warning(
                             "Cannot download file for task_id=%s from %s: %s",
                             task.task_id,
                             out_file,
                             err,
                         )
-                await sftp.rmtree(machine.path(remote_folder)) # uncomment to keep raw files
+                await sftp.rmtree(
+                    machine.path(remote_folder)
+                )  # uncomment to keep raw files
 
         try:
             await sftp_get_retry(job)()
         except Exception as err:
             self.log.warning("Cannot scp from %s: %s" % (remote_folder, err))
             sftp_errors.append((remote_folder, err))
 
@@ -527,15 +529,15 @@
             return
         # if machine state is unknown
         if machine.meta.busy is None:
             engine = self.config.engines.get(task.metadata["engine"])
             if engine:
                 await machine.start_occupancy_check(engine)
         # consume
-        if not machine.meta.busy:
+        if machine.meta.busy is False:
             self.log.debug(f"machine {machine.hostname} is free for task {task_id}")
             await self.consume_task(machine, task)
 
     async def deallocator_producer(
         self,
     ) -> AsyncGenerator[UMessage[str, NodeModel], None]:
         """Produce messages with nodes for deallocation"""
```

### Comparing `yascheduler-1.0.7/yascheduler/utils.py` & `yascheduler-1.0.8/yascheduler/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,15 +326,15 @@
 
 def show_nodes():
     asyncio.run(_show_nodes())
 
 
 async def _manage_node():
     parser = argparse.ArgumentParser(description="Add nodes to yascheduler daemon")
-    parser.add_argument("host", help="IP[~ncpus]")
+    parser.add_argument("host", help="[user@]IP[~ncpus]")
     parser.add_argument(
         "--skip-setup",
         required=False,
         default=False,
         nargs="?",
         type=bool,
         const=True,
```

### Comparing `yascheduler-1.0.7/yascheduler.egg-info/PKG-INFO` & `yascheduler-1.0.8/yascheduler.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: yascheduler
-Version: 1.0.7
+Version: 1.0.8
 Summary: Yet another computing scheduler and cloud orchestration engine
 Home-page: https://github.com/tilde-lab/yascheduler
 Author: Sergey Korolev, Evgeny Blokhin, Andrey Sobolev
 Author-email: eb@tilde.pro
 License: MIT
 Description: *Yascheduler* is a job scheduler designed for submitting scientific simulations to the VM clouds and copying back their results.
 Platform: UNKNOWN
```

### Comparing `yascheduler-1.0.7/yascheduler.egg-info/SOURCES.txt` & `yascheduler-1.0.8/yascheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

