# Comparing `tmp/murfey-0.7.7.tar.gz` & `tmp/murfey-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "murfey-0.7.7.tar", last modified: Fri Apr 14 14:47:34 2023, max compression
+gzip compressed data, was "murfey-0.7.8.tar", last modified: Sun Apr 16 20:50:50 2023, max compression
```

## Comparing `murfey-0.7.7.tar` & `murfey-0.7.8.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.259859 murfey-0.7.7/
--rw-r--r--   0 vsts      (1001) docker     (122)     1481 2023-04-14 14:47:27.000000 murfey-0.7.7/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      179 2023-04-14 14:47:27.000000 murfey-0.7.7/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     2463 2023-04-14 14:47:34.259859 murfey-0.7.7/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1698 2023-04-14 14:47:27.000000 murfey-0.7.7/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      206 2023-04-14 14:47:27.000000 murfey-0.7.7/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     1647 2023-04-14 14:47:34.259859 murfey-0.7.7/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-04-14 14:47:27.000000 murfey-0.7.7/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.247859 murfey-0.7.7/src/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.251859 murfey-0.7.7/src/murfey/
--rw-r--r--   0 vsts      (1001) docker     (122)       97 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.251859 murfey-0.7.7/src/murfey/bootstrap/
--rw-r--r--   0 vsts      (1001) docker     (122)     4237 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/bootstrap/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.251859 murfey-0.7.7/src/murfey/cli/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/cli/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      919 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/cli/dummy.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2621 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/cli/transfer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.251859 murfey-0.7.7/src/murfey/client/
--rw-r--r--   0 vsts      (1001) docker     (122)    10265 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12051 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/analyser.py
--rw-r--r--   0 vsts      (1001) docker     (122)    45471 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/context.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.255859 murfey-0.7.7/src/murfey/client/contexts/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/contexts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2476 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/contexts/tomo.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1466 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/customlogging.py
--rw-r--r--   0 vsts      (1001) docker     (122)      546 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/gain_ref.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7058 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/instance_environment.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11696 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/rsync.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.255859 murfey-0.7.7/src/murfey/client/tui/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/tui/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      127 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/tui/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19403 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/tui/app.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5094 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/tui/controller.css
--rw-r--r--   0 vsts      (1001) docker     (122)      678 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/tui/forms.py
--rw-r--r--   0 vsts      (1001) docker     (122)      318 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/tui/launcher.css
--rw-r--r--   0 vsts      (1001) docker     (122)     5280 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/tui/progress.py
--rw-r--r--   0 vsts      (1001) docker     (122)    26660 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/tui/screens.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2188 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/tui/status_bar.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2594 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/update.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9178 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/watchdir.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2204 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/watchdir_multigrid.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4895 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/client/websocket.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.255859 murfey-0.7.7/src/murfey/server/
--rw-r--r--   0 vsts      (1001) docker     (122)    17866 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/server/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18289 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/server/api.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8109 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/server/bootstrap.py
--rw-r--r--   0 vsts      (1001) docker     (122)      946 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/server/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11850 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/server/demo_api.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1875 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/server/gain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7596 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/server/ispyb.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1085 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/server/main.py
--rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/server/run.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4265 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/server/websocket.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.255859 murfey-0.7.7/src/murfey/templates/
--rw-r--r--   0 vsts      (1001) docker     (122)      671 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/templates/activevisits.html
--rw-r--r--   0 vsts      (1001) docker     (122)      891 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/templates/base.html
--rw-r--r--   0 vsts      (1001) docker     (122)     1148 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/templates/bootstrap.html
--rw-r--r--   0 vsts      (1001) docker     (122)      242 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/templates/home.html
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.259859 murfey-0.7.7/src/murfey/templates/images/
--rw-r--r--   0 vsts      (1001) docker     (122)   131288 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/templates/images/diamond.png
--rw-r--r--   0 vsts      (1001) docker     (122)    14468 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/templates/images/icon_268.png
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.259859 murfey-0.7.7/src/murfey/templates/static/
--rw-r--r--   0 vsts      (1001) docker     (122)     1420 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/templates/static/styles.css
--rw-r--r--   0 vsts      (1001) docker     (122)      726 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/templates/visit.html
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.259859 murfey-0.7.7/src/murfey/util/
--rw-r--r--   0 vsts      (1001) docker     (122)     3390 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3262 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/util/dummy_setup.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1309 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/util/file_monitor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1133 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/util/mdoc.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3682 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/util/models.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6530 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/util/rsync.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3210 2023-04-14 14:47:27.000000 murfey-0.7.7/src/murfey/util/state.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 14:47:34.251859 murfey-0.7.7/src/murfey.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     2463 2023-04-14 14:47:34.000000 murfey-0.7.7/src/murfey.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1947 2023-04-14 14:47:34.000000 murfey-0.7.7/src/murfey.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-14 14:47:34.000000 murfey-0.7.7/src/murfey.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      160 2023-04-14 14:47:34.000000 murfey-0.7.7/src/murfey.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-14 14:47:34.000000 murfey-0.7.7/src/murfey.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      252 2023-04-14 14:47:34.000000 murfey-0.7.7/src/murfey.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        7 2023-04-14 14:47:34.000000 murfey-0.7.7/src/murfey.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.841428 murfey-0.7.8/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1481 2023-04-16 20:50:45.000000 murfey-0.7.8/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      179 2023-04-16 20:50:45.000000 murfey-0.7.8/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     2463 2023-04-16 20:50:50.841428 murfey-0.7.8/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1698 2023-04-16 20:50:45.000000 murfey-0.7.8/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      206 2023-04-16 20:50:45.000000 murfey-0.7.8/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1647 2023-04-16 20:50:50.841428 murfey-0.7.8/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-04-16 20:50:45.000000 murfey-0.7.8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.825428 murfey-0.7.8/src/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.829428 murfey-0.7.8/src/murfey/
+-rw-r--r--   0 vsts      (1001) docker     (122)       97 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.829428 murfey-0.7.8/src/murfey/bootstrap/
+-rw-r--r--   0 vsts      (1001) docker     (122)     4237 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/bootstrap/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.829428 murfey-0.7.8/src/murfey/cli/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      919 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/cli/dummy.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2621 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/cli/transfer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.833428 murfey-0.7.8/src/murfey/client/
+-rw-r--r--   0 vsts      (1001) docker     (122)    10265 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12896 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/analyser.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    44190 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/context.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.833428 murfey-0.7.8/src/murfey/client/contexts/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/contexts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2476 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/contexts/tomo.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1466 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/customlogging.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      546 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/gain_ref.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7084 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/instance_environment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11696 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/rsync.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.837428 murfey-0.7.8/src/murfey/client/tui/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/tui/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      127 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/tui/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19676 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/tui/app.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5101 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/tui/controller.css
+-rw-r--r--   0 vsts      (1001) docker     (122)      179 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/tui/forms.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      318 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/tui/launcher.css
+-rw-r--r--   0 vsts      (1001) docker     (122)     5280 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/tui/progress.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    32434 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/tui/screens.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2188 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/tui/status_bar.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2594 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/update.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9178 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/watchdir.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2204 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/watchdir_multigrid.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4895 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/websocket.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.837428 murfey-0.7.8/src/murfey/server/
+-rw-r--r--   0 vsts      (1001) docker     (122)    18740 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/server/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18416 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/server/api.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8109 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/server/bootstrap.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      978 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/server/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11850 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/server/demo_api.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1875 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/server/gain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7596 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/server/ispyb.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1085 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/server/main.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/server/run.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4265 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/server/websocket.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.837428 murfey-0.7.8/src/murfey/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)      671 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/templates/activevisits.html
+-rw-r--r--   0 vsts      (1001) docker     (122)      891 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/templates/base.html
+-rw-r--r--   0 vsts      (1001) docker     (122)     1148 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/templates/bootstrap.html
+-rw-r--r--   0 vsts      (1001) docker     (122)      242 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/templates/home.html
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.837428 murfey-0.7.8/src/murfey/templates/images/
+-rw-r--r--   0 vsts      (1001) docker     (122)   131288 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/templates/images/diamond.png
+-rw-r--r--   0 vsts      (1001) docker     (122)    14468 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/templates/images/icon_268.png
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.837428 murfey-0.7.8/src/murfey/templates/static/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1420 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/templates/static/styles.css
+-rw-r--r--   0 vsts      (1001) docker     (122)      726 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/templates/visit.html
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.841428 murfey-0.7.8/src/murfey/util/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3390 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3262 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/util/dummy_setup.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1309 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/util/file_monitor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1133 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/util/mdoc.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4128 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/util/models.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6530 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/util/rsync.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3210 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/util/state.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.829428 murfey-0.7.8/src/murfey.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2463 2023-04-16 20:50:50.000000 murfey-0.7.8/src/murfey.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1947 2023-04-16 20:50:50.000000 murfey-0.7.8/src/murfey.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-16 20:50:50.000000 murfey-0.7.8/src/murfey.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      160 2023-04-16 20:50:50.000000 murfey-0.7.8/src/murfey.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-16 20:50:50.000000 murfey-0.7.8/src/murfey.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      252 2023-04-16 20:50:50.000000 murfey-0.7.8/src/murfey.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        7 2023-04-16 20:50:50.000000 murfey-0.7.8/src/murfey.egg-info/top_level.txt
```

### Comparing `murfey-0.7.7/LICENSE` & `murfey-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/PKG-INFO` & `murfey-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: murfey
-Version: 0.7.7
+Version: 0.7.8
 Summary: Client-Server architecture hauling Cryo-EM data
 License: BSD
 Project-URL: Bug-Tracker, https://github.com/DiamondLightSource/python-murfey/issues
 Project-URL: Documentation, https://github.com/DiamondLightSource/python-murfey
 Project-URL: GitHub, https://github.com/DiamondLightSource/python-murfey
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `murfey-0.7.7/README.md` & `murfey-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/setup.cfg` & `murfey-0.7.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = murfey
 description = Client-Server architecture hauling Cryo-EM data
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 0.7.7
+version = 0.7.8
 license = BSD
 license_file = LICENSE
 classifiers = 
 	Development Status :: 3 - Alpha
 	Environment :: Console
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: BSD License
@@ -46,15 +46,15 @@
 	jinja2
 	packaging
 	uvicorn[standard]
 	werkzeug
 	zocalo
 client = 
 	procrunner
-	textual ==0.16.0
+	textual ==0.17.0
 	websocket-client
 	xmltodict
 
 [options.packages.find]
 where = src
 
 [options.package_data]
```

### Comparing `murfey-0.7.7/src/murfey/bootstrap/__main__.py` & `murfey-0.7.8/src/murfey/bootstrap/__main__.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/cli/dummy.py` & `murfey-0.7.8/src/murfey/cli/dummy.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/cli/transfer.py` & `murfey-0.7.8/src/murfey/cli/transfer.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/client/__init__.py` & `murfey-0.7.8/src/murfey/client/__init__.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/client/analyser.py` & `murfey-0.7.8/src/murfey/client/analyser.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,20 +5,36 @@
 import threading
 from pathlib import Path
 from typing import Type
 
 from murfey.client.context import Context, SPAContext, TomographyContext
 from murfey.client.instance_environment import MurfeyInstanceEnvironment
 from murfey.client.rsync import RSyncerUpdate
-from murfey.client.tui.forms import TUIFormValue
+from murfey.client.tui.forms import FormDependency
 from murfey.util import Observer, get_machine_config
 from murfey.util.models import DCParametersSPA, DCParametersTomo
 
 logger = logging.getLogger("murfey.client.analyser")
 
+spa_form_dependencies: dict = {
+    "use_cryolo": FormDependency(
+        dependencies={"estimate_particle_diameter": False}, trigger_value=False
+    ),
+    "estimate_particle_diameter": FormDependency(
+        dependencies={
+            "use_cryolo": True,
+            "boxsize": "None",
+            "small_boxsize": "None",
+            "mask_diameter": "None",
+            "particle_diameter": "None",
+        },
+        trigger_value=True,
+    ),
+}
+
 
 class Analyser(Observer):
     def __init__(
         self,
         basepath_local: Path,
         environment: MurfeyInstanceEnvironment | None = None,
         force_mdoc_metadata: bool = False,
@@ -106,15 +122,14 @@
         return False
 
     def _analyse(self):
         logger.info("Analyser thread started")
         mdoc_for_reading = None
         while not self._halt_thread:
             transferred_file = self.queue.get()
-            logger.info(f"analysing file {transferred_file}")
             if not transferred_file:
                 self._halt_thread = True
                 continue
             dc_metadata = {}
             if (
                 self._force_mdoc_metadata
                 and transferred_file.suffix == ".mdoc"
@@ -157,23 +172,28 @@
                             except NotImplementedError:
                                 dc_metadata = {}
                         if not dc_metadata or not self._force_mdoc_metadata:
                             self._unseen_xml.append(transferred_file)
                         else:
                             self._unseen_xml = []
                             if dc_metadata.get("file_extension"):
-                                self._extension = dc_metadata["file_extension"].data
+                                self._extension = dc_metadata["file_extension"]
                             else:
-                                dc_metadata["file_extension"] = TUIFormValue(
-                                    self._extension
-                                )
-                            dc_metadata["acquisition_software"] = TUIFormValue(
-                                self._context._acquisition_software
+                                dc_metadata["file_extension"] = self._extension
+                            dc_metadata[
+                                "acquisition_software"
+                            ] = self._context._acquisition_software
+                            self.notify(
+                                {
+                                    "form": dc_metadata,
+                                    "dependencies": spa_form_dependencies
+                                    if isinstance(self._context, SPAContext)
+                                    else {},
+                                }
                             )
-                            self.notify({"form": dc_metadata})
             elif not self._extension or self._unseen_xml:
                 self._find_extension(transferred_file)
                 if self._extension:
                     logger.info(
                         f"Context found successfully: {self._role}, {transferred_file}"
                     )
                     try:
@@ -191,23 +211,28 @@
                                 environment=self._environment,
                             )
                         if not dc_metadata or not self._force_mdoc_metadata:
                             self._unseen_xml.append(transferred_file)
                         if dc_metadata:
                             self._unseen_xml = []
                             if dc_metadata.get("file_extension"):
-                                self._extension = dc_metadata["file_extension"].data
+                                self._extension = dc_metadata["file_extension"]
                             else:
-                                dc_metadata["file_extension"] = TUIFormValue(
-                                    self._extension
-                                )
-                            dc_metadata["acquisition_software"] = TUIFormValue(
-                                self._context._acquisition_software
+                                dc_metadata["file_extension"] = self._extension
+                            dc_metadata[
+                                "acquisition_software"
+                            ] = self._context._acquisition_software
+                            self.notify(
+                                {
+                                    "form": dc_metadata,
+                                    "dependencies": spa_form_dependencies
+                                    if isinstance(self._context, SPAContext)
+                                    else {},
+                                }
                             )
-                            self.notify({"form": dc_metadata})
             elif isinstance(self._context, TomographyContext):
                 _tilt_series = set(self._context._tilt_series.keys())
                 self._context.post_transfer(
                     transferred_file, role=self._role, environment=self._environment
                 )
                 if (
                     len(self._context._tilt_series.keys()) > len(_tilt_series)
```

### Comparing `murfey-0.7.7/src/murfey/client/context.py` & `murfey-0.7.8/src/murfey/client/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from murfey.client.instance_environment import (
     MovieID,
     MovieTracker,
     MurfeyID,
     MurfeyInstanceEnvironment,
     global_env_lock,
 )
-from murfey.client.tui.forms import TUIFormValue
 from murfey.util import get_machine_config
 from murfey.util.mdoc import get_block, get_global_data, get_num_blocks
 
 logger = logging.getLogger("murfey.client.context")
 
 
 class FutureRequest(NamedTuple):
@@ -79,41 +78,41 @@
 
 
 class SPAContext(Context):
     user_params = [
         ProcessingParameter(
             "dose_per_frame", "Dose Per Frame (e- / Angstrom^2 / frame)"
         ),
+        ProcessingParameter(
+            "estimate_particle_diameter",
+            "Use crYOLO to Estimate Particle Diameter",
+            default=True,
+        ),
+        ProcessingParameter(
+            "particle_diameter", "Particle Diameter (Angstroms)", default=0
+        ),
         ProcessingParameter("use_cryolo", "Use crYOLO Autopicking", default=True),
         ProcessingParameter("symmetry", "Symmetry Group", default="C1"),
-        ProcessingParameter("boxsize", "Box Size", default=256),
         ProcessingParameter("eer_grouping", "EER Grouping", default=20),
         ProcessingParameter(
             "mask_diameter", "Mask Diameter (2D classification)", default=190
         ),
+        ProcessingParameter("boxsize", "Box Size", default=256),
         ProcessingParameter("downscale", "Downscale Extracted Particles", default=True),
         ProcessingParameter(
             "small_boxsize", "Downscaled Extracted Particle Size (pixels)", default=128
         ),
-        ProcessingParameter(
-            "estimate_particle_diameter",
-            "Use crYOLO to Estimate Particle Diameter",
-            default=True,
-        ),
-        ProcessingParameter(
-            "particle_diameter", "Particle Diameter (Angstroms)", default=0
-        ),
+        ProcessingParameter("gain_ref", "Gain Reference"),
     ]
     metadata_params = [
         ProcessingParameter("voltage", "Voltage"),
         ProcessingParameter("image_size_x", "Image Size X"),
         ProcessingParameter("image_size_y", "Image Size Y"),
         ProcessingParameter("pixel_size_on_image", "Pixel Size"),
         ProcessingParameter("motion_corr_binning", "Motion Correction Binning"),
-        ProcessingParameter("gain_ref", "Gain Reference"),
     ]
 
     def __init__(self, acquisition_software: str, basepath: Path):
         super().__init__(acquisition_software)
         self._basepath = basepath
         self._processing_job_stash: dict = {}
         self._preprocessing_triggers: dict = {}
@@ -123,21 +122,15 @@
         tag: str,
         url: str,
         data: dict,
         environment: MurfeyInstanceEnvironment,
     ):
         logger.info(f"registering data collection with data {data}")
         environment.id_tag_registry["data_collection"].append(tag)
-        machine_config = get_machine_config(
-            str(environment.url.geturl()), demo=environment.demo
-        )
-        image_directory = str(
-            Path(machine_config.get("rsync_basepath", "."))
-            / environment.default_destinations[Path(tag)]
-        )
+        image_directory = str(environment.default_destinations[Path(tag)])
         json = {
             "voltage": data["voltage"],
             "pixel_size_on_image": data["pixel_size_on_image"],
             "experiment_type": data["experiment_type"],
             "image_size_x": data["image_size_x"],
             "image_size_y": data["image_size_y"],
             "file_extension": data["file_extension"],
@@ -236,118 +229,104 @@
                 for_parsing = xml.read()
             except Exception:
                 logger.warning(f"Failed to parse file {metadata_file}")
                 return OrderedDict({})
             data = xmltodict.parse(for_parsing)
         magnification = 0
         metadata: OrderedDict = OrderedDict({})
-        metadata["experiment_type"] = TUIFormValue("SPA")
+        metadata["experiment_type"] = "SPA"
         if data.get("Acquisition"):
-            metadata["voltage"] = TUIFormValue(300)
-            metadata["image_size_x"] = TUIFormValue(
-                data["Acquisition"]["Info"]["ImageSize"]["Width"]
-            )
-            metadata["image_size_y"] = TUIFormValue(
-                data["Acquisition"]["Info"]["ImageSize"]["Height"]
-            )
-            metadata["pixel_size_on_image"] = TUIFormValue(
-                float(data["Acquisition"]["Info"]["SensorPixelSize"]["Height"])
+            metadata["voltage"] = 300
+            metadata["image_size_x"] = data["Acquisition"]["Info"]["ImageSize"]["Width"]
+            metadata["image_size_y"] = data["Acquisition"]["Info"]["ImageSize"][
+                "Height"
+            ]
+            metadata["pixel_size_on_image"] = float(
+                data["Acquisition"]["Info"]["SensorPixelSize"]["Height"]
             )
         elif data.get("MicroscopeImage"):
-            metadata["voltage"] = TUIFormValue(
+            metadata["voltage"] = (
                 float(
                     data["MicroscopeImage"]["microscopeData"]["gun"][
                         "AccelerationVoltage"
                     ]
                 )
                 / 1000
             )
-            metadata["image_size_x"] = TUIFormValue(
-                data["MicroscopeImage"]["microscopeData"]["acquisition"]["camera"][
-                    "ReadoutArea"
-                ]["a:width"]
-            )
-            metadata["image_size_y"] = TUIFormValue(
-                data["MicroscopeImage"]["microscopeData"]["acquisition"]["camera"][
-                    "ReadoutArea"
-                ]["a:height"]
-            )
-            metadata["pixel_size_on_image"] = TUIFormValue(
-                data["MicroscopeImage"]["SpatialScale"]["pixelSize"]["x"][
-                    "numericValue"
-                ]
-            )
+            metadata["image_size_x"] = data["MicroscopeImage"]["microscopeData"][
+                "acquisition"
+            ]["camera"]["ReadoutArea"]["a:width"]
+            metadata["image_size_y"] = data["MicroscopeImage"]["microscopeData"][
+                "acquisition"
+            ]["camera"]["ReadoutArea"]["a:height"]
+            metadata["pixel_size_on_image"] = data["MicroscopeImage"]["SpatialScale"][
+                "pixelSize"
+            ]["x"]["numericValue"]
             magnification = data["MicroscopeImage"]["microscopeData"]["optics"][
                 "TemMagnification"
             ]["NominalMagnification"]
-            metadata["magnification"] = TUIFormValue(magnification)
-            metadata["total_exposed_dose"] = TUIFormValue(
-                data["MicroscopeImage"]["CustomData"]["a:KeyValueOfstringanyType"][0][
-                    "a:Value"
-                ]["#text"]
-            )
-            metadata["c2aperture"] = TUIFormValue(
-                data["MicroscopeImage"]["CustomData"]["a:KeyValueOfstringanyType"][3][
-                    "a:Value"
-                ]["#text"]
-            )
-            metadata["exposure_time"] = TUIFormValue(
-                data["MicroscopeImage"]["microscopeData"]["acquisition"]["camera"][
-                    "ExposureTime"
-                ]
-            )
-            metadata["slit_width"] = TUIFormValue(
-                data["MicroscopeImage"]["microscopeData"]["optics"]["EnergyFilter"][
-                    "EnergySelectionSlitWidth"
-                ]
-            )
-            metadata["phase_plate"] = TUIFormValue(
+            metadata["magnification"] = magnification
+            metadata["total_exposed_dose"] = data["MicroscopeImage"]["CustomData"][
+                "a:KeyValueOfstringanyType"
+            ][0]["a:Value"]["#text"]
+            metadata["c2aperture"] = data["MicroscopeImage"]["CustomData"][
+                "a:KeyValueOfstringanyType"
+            ][3]["a:Value"]["#text"]
+            metadata["exposure_time"] = data["MicroscopeImage"]["microscopeData"][
+                "acquisition"
+            ]["camera"]["ExposureTime"]
+            metadata["slit_width"] = data["MicroscopeImage"]["microscopeData"][
+                "optics"
+            ]["EnergyFilter"]["EnergySelectionSlitWidth"]
+            metadata["phase_plate"] = (
                 1
                 if data["MicroscopeImage"]["CustomData"]["a:KeyValueOfstringanyType"][
                     11
                 ]["a:Value"]["#text"]
                 == "true"
                 else 0
             )
         else:
             logger.warning("Metadata file format is not recognised")
             return OrderedDict({})
-        if environment and magnification:
+        binning_factor = 1
+        if environment:
             server_config = requests.get(
                 f"{str(environment.url.geturl())}/machine/"
             ).json()
-            ps_from_mag = (
-                server_config.get("calibrations", {})
-                .get("magnification", {})
-                .get(int(magnification))
-            )
-            if ps_from_mag:
-                metadata["pixel_size_on_image"] = TUIFormValue(
-                    float(ps_from_mag) * 1e-10
-                )
-        metadata["motion_corr_binning"] = TUIFormValue(1)
-        metadata["gain_ref"] = TUIFormValue(None, top=True)
-        metadata["dose_per_frame"] = TUIFormValue(
+            if server_config.get("superres") and environment.superres:
+                binning_factor = 2
+            if magnification:
+                ps_from_mag = (
+                    server_config.get("calibrations", {})
+                    .get("magnification", {})
+                    .get(int(magnification))
+                )
+                if ps_from_mag:
+                    metadata["pixel_size_on_image"] = float(ps_from_mag) * 1e-10
+        metadata["pixel_size_on_image"] = (
+            metadata["pixel_size_on_image"] / binning_factor
+        )
+        metadata["motion_corr_binning"] = binning_factor
+        metadata["gain_ref"] = None
+        metadata["dose_per_frame"] = (
             environment.data_collection_parameters.get("dose_per_frame")
             if environment
-            else None,
-            top=True,
+            else None
         )
-        metadata["use_cryolo"] = TUIFormValue(True)
-        metadata["symmetry"] = TUIFormValue("C1")
-        metadata["mask_diameter"] = TUIFormValue(190)
-        metadata["boxsize"] = TUIFormValue(256)
-        metadata["downscale"] = TUIFormValue(False)
-        metadata["small_boxsize"] = TUIFormValue(128)
-        metadata["eer_grouping"] = TUIFormValue(20)
-        metadata["source"] = TUIFormValue(str(self._basepath))
-        metadata["particle_diameter"] = TUIFormValue(0)
-        metadata["estimate_particle_diameter"] = TUIFormValue(True)
-        metadata.move_to_end("gain_ref", last=False)
-        metadata.move_to_end("dose_per_frame", last=False)
+        metadata["use_cryolo"] = True
+        metadata["symmetry"] = "C1"
+        metadata["mask_diameter"] = 190
+        metadata["boxsize"] = 256
+        metadata["downscale"] = False
+        metadata["small_boxsize"] = 128
+        metadata["eer_grouping"] = 20
+        metadata["source"] = str(self._basepath)
+        metadata["particle_diameter"] = 0
+        metadata["estimate_particle_diameter"] = True
         return metadata
 
 
 class ProcessFileIncomplete(BaseModel):
     dest: Path
     source: Path
     image_number: int
@@ -357,23 +336,23 @@
 
 
 class TomographyContext(Context):
     user_params = [
         ProcessingParameter(
             "dose_per_frame", "Dose Per Frame (e- / Angstrom^2 / frame)"
         ),
-        ProcessingParameter("manual_tilt_offset", "Tilt Offset"),
+        ProcessingParameter("manual_tilt_offset", "Tilt Offset", default=0),
+        ProcessingParameter("gain_ref", "Gain Reference"),
     ]
     metadata_params = [
         ProcessingParameter("voltage", "Voltage"),
         ProcessingParameter("image_size_x", "Image Size X"),
         ProcessingParameter("image_size_y", "Image Size Y"),
         ProcessingParameter("pixel_size_on_image", "Pixel Size"),
         ProcessingParameter("motion_corr_binning", "Motion Correction Binning"),
-        ProcessingParameter("gain_ref", "Gain Reference"),
     ]
 
     def __init__(self, acquisition_software: str, basepath: Path):
         super().__init__(acquisition_software)
         self._basepath = basepath
         self._tilt_series: Dict[str, List[Path]] = {}
         self._tilt_series_sizes: Dict[str, int | None] = {}
@@ -612,15 +591,18 @@
                                     file_path.parent, file_path.parent
                                 )
                             ).resolve()
                         ),
                         "tag": tilt_series,
                         "source": str(self._basepath),
                     }
-                    if environment.data_collection_parameters:
+                    if (
+                        environment.data_collection_parameters
+                        and environment.data_collection_parameters.get("voltage")
+                    ):
                         data.update(
                             {
                                 "voltage": environment.data_collection_parameters[
                                     "voltage"
                                 ],
                                 "pixel_size_on_image": environment.data_collection_parameters[
                                     "pixel_size_on_image"
@@ -659,15 +641,15 @@
                             json={"tag": tilt_series, "recipe": "em-tomo-preprocess"},
                         )
                         requests.post(
                             proc_url,
                             json={"tag": tilt_series, "recipe": "em-tomo-align"},
                         )
             except Exception as e:
-                logger.error(f"ERROR {e}")
+                logger.error(f"ERROR {e}, {environment.data_collection_parameters}")
         else:
             if file_path not in self._tilt_series[tilt_series]:
                 for p in self._tilt_series[tilt_series]:
                     if tilt_angle == extract_tilt_angle(p):
                         break
                 else:
                     self._tilt_series[tilt_series].append(file_path)
@@ -969,84 +951,79 @@
                     for_parsing = xml.read()
                 except Exception:
                     logger.warning(f"Failed to parse file {metadata_file}")
                     return OrderedDict({})
                 data = xmltodict.parse(for_parsing)
             try:
                 metadata: OrderedDict = OrderedDict({})
-                metadata["experiment_type"] = TUIFormValue("tomography")
-                metadata["voltage"] = TUIFormValue(300)
-                metadata["image_size_x"] = TUIFormValue(
-                    data["Acquisition"]["Info"]["ImageSize"]["Width"]
-                )
-                metadata["image_size_y"] = TUIFormValue(
-                    data["Acquisition"]["Info"]["ImageSize"]["Height"]
-                )
-                metadata["pixel_size_on_image"] = TUIFormValue(
-                    float(data["Acquisition"]["Info"]["SensorPixelSize"]["Height"])
+                metadata["experiment_type"] = "tomography"
+                metadata["voltage"] = 300
+                metadata["image_size_x"] = data["Acquisition"]["Info"]["ImageSize"][
+                    "Width"
+                ]
+                metadata["image_size_y"] = data["Acquisition"]["Info"]["ImageSize"][
+                    "Height"
+                ]
+                metadata["pixel_size_on_image"] = float(
+                    data["Acquisition"]["Info"]["SensorPixelSize"]["Height"]
                 )
-                metadata["motion_corr_binning"] = TUIFormValue(1)
-                metadata["gain_ref"] = TUIFormValue(None, top=True)
-                metadata["dose_per_frame"] = TUIFormValue(
+                metadata["motion_corr_binning"] = 1
+                metadata["gain_ref"] = None
+                metadata["dose_per_frame"] = (
                     environment.data_collection_parameters.get("dose_per_frame")
                     if environment
-                    else None,
-                    top=True,
-                    colour="dark_orange",
+                    else None
                 )
-                metadata["manual_tilt_offset"] = TUIFormValue(0, top=True)
-                metadata["source"] = TUIFormValue(str(self._basepath))
-                metadata.move_to_end("gain_ref", last=False)
-                metadata.move_to_end("dose_per_frame", last=False)
+                metadata["manual_tilt_offset"] = 0
+                metadata["source"] = str(self._basepath)
             except KeyError:
                 return OrderedDict({})
             return metadata
         with open(metadata_file, "r") as md:
             mdoc_data = get_global_data(md)
             mdoc_data_block = get_block(md)
         if not mdoc_data:
             return OrderedDict({})
         mdoc_metadata: OrderedDict = OrderedDict({})
-        mdoc_metadata["experiment_type"] = TUIFormValue("tomography")
-        mdoc_metadata["voltage"] = TUIFormValue(float(mdoc_data["Voltage"]))
-        mdoc_metadata["image_size_x"] = TUIFormValue(int(mdoc_data["ImageSize"][0]))
-        mdoc_metadata["image_size_y"] = TUIFormValue(int(mdoc_data["ImageSize"][1]))
-        mdoc_metadata["magnification"] = TUIFormValue(
-            int(mdoc_data_block["Magnification"])
-        )
+        mdoc_metadata["experiment_type"] = "tomography"
+        mdoc_metadata["voltage"] = float(mdoc_data["Voltage"])
+        mdoc_metadata["image_size_x"] = int(mdoc_data["ImageSize"][0])
+        mdoc_metadata["image_size_y"] = int(mdoc_data["ImageSize"][1])
+        mdoc_metadata["magnification"] = int(mdoc_data_block["Magnification"])
         superres_binning = int(mdoc_data_block["Binning"])
         binning_factor = 1
         if environment:
             server_config = requests.get(
                 f"{str(environment.url.geturl())}/machine/"
             ).json()
-            if server_config.get("superres") and superres_binning == 1:
+            if (
+                server_config.get("superres")
+                and superres_binning == 1
+                and environment.superres
+            ):
                 binning_factor = 2
             ps_from_mag = (
                 server_config.get("calibrations", {})
                 .get("magnification", {})
                 .get(int(mdoc_data_block["Magnification"]))
             )
             if ps_from_mag:
-                mdoc_metadata["pixel_size_on_image"] = TUIFormValue(
+                mdoc_metadata["pixel_size_on_image"] = (
                     float(ps_from_mag) * 1e-10 / binning_factor
                 )
         if mdoc_metadata.get("pixel_size_on_image") is None:
-            mdoc_metadata["pixel_size_on_image"] = TUIFormValue(
+            mdoc_metadata["pixel_size_on_image"] = (
                 float(mdoc_data["PixelSpacing"]) * 1e-10 / binning_factor
             )
-        mdoc_metadata["motion_corr_binning"] = TUIFormValue(binning_factor)
-        mdoc_metadata["gain_ref"] = TUIFormValue(None, top=True)
-        mdoc_metadata["dose_per_frame"] = TUIFormValue(
+        mdoc_metadata["motion_corr_binning"] = binning_factor
+        mdoc_metadata["gain_ref"] = None
+        mdoc_metadata["dose_per_frame"] = (
             environment.data_collection_parameters.get("dose_per_frame")
             if environment
-            else None,
-            top=True,
-        )
-        mdoc_metadata["manual_tilt_offset"] = TUIFormValue(0, top=True)
-        mdoc_metadata["source"] = TUIFormValue(str(self._basepath))
-        mdoc_metadata.move_to_end("gain_ref", last=False)
-        mdoc_metadata.move_to_end("dose_per_frame", last=False)
-        mdoc_metadata["file_extension"] = TUIFormValue(
-            f".{mdoc_data_block['SubFramePath'].split('.')[-1]}"
+            else None
         )
+        mdoc_metadata["manual_tilt_offset"] = 0
+        mdoc_metadata["source"] = str(self._basepath)
+        mdoc_metadata[
+            "file_extension"
+        ] = f".{mdoc_data_block['SubFramePath'].split('.')[-1]}"
         return mdoc_metadata
```

### Comparing `murfey-0.7.7/src/murfey/client/contexts/tomo.py` & `murfey-0.7.8/src/murfey/client/contexts/tomo.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/client/customlogging.py` & `murfey-0.7.8/src/murfey/client/customlogging.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/client/gain_ref.py` & `murfey-0.7.8/src/murfey/client/gain_ref.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/client/instance_environment.py` & `murfey-0.7.8/src/murfey/client/instance_environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     motion_corrected_movies: Dict[Path, List[str]] = {}
     listeners: Dict[str, Set[Callable]] = {}
     movie_tilt_pair: Dict[Path, str] = {}
     tilt_angles: Dict[str, List[List[str]]] = {}
     visit: str = ""
     processing_only_mode: bool = False
     gain_ref: Optional[Path] = None
+    superres: bool = True
 
     class Config:
         validate_assignment: bool = True
         arbitrary_types_allowed: bool = True
 
     def clear(self):
         self.sources = []
```

### Comparing `murfey-0.7.7/src/murfey/client/rsync.py` & `murfey-0.7.8/src/murfey/client/rsync.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/client/tui/app.py` & `murfey-0.7.8/src/murfey/client/tui/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     ProcessingForm,
     VisitSelection,
     determine_default_destination,
 )
 from murfey.client.tui.status_bar import StatusBar
 from murfey.client.watchdir import DirWatcher
 from murfey.client.watchdir_multigrid import MultigridDirWatcher
-from murfey.util import _get_visit_list
+from murfey.util import _get_visit_list, get_machine_config
 
 log = logging.getLogger("murfey.tui.app")
 
 ReactiveType = TypeVar("ReactiveType")
 
 
 class MurfeyTUI(App):
@@ -41,14 +41,15 @@
     processing_btn: Button
     processing_form: ProcessingForm
     hover: List[str]
     visits: List[str]
     rsync_processes: Dict[Path, RSyncer] = {}
     analysers: Dict[Path, Analyser] = {}
     _form_values: dict = reactive({})
+    _form_dependencies: dict = {}
 
     def __init__(
         self,
         environment: MurfeyInstanceEnvironment | None = None,
         visits: List[str] | None = None,
         queues: Dict[str, Queue] | None = None,
         status_bar: StatusBar | None = None,
@@ -249,19 +250,18 @@
             return
         if self._register_dc and response.get("form"):
             self._form_values = {k: str(v) for k, v in response.get("form", {}).items()}
             log.info(
                 f"gain reference is set to {self._form_values.get('gain_ref')}, {self._environment.data_collection_parameters.get('gain_ref')}"
             )
             if self._form_values.get("gain_ref") in (None, "None"):
-                log.info(self._form_values)
                 self._form_values[
                     "gain_ref"
                 ] = self._environment.data_collection_parameters.get("gain_ref")
-            log.info(self._form_values)
+            self._form_dependencies = response.get("dependencies", {})
             self.processing_btn.disabled = False
             self._data_collection_form_complete = True
         elif self._register_dc is None:
             self._tmp_responses.append(response)
             self._data_collection_form_complete = True
 
     def _start_dc_confirm_prompt(self, json: dict):
@@ -348,15 +348,17 @@
 
     async def on_load(self, event):
         self.bind("q", "quit", description="Quit", show=True)
         self.bind("c", "clear", description="Remove copied data and quit", show=True)
         self.bind("p", "process", description="Allow processing", show=True)
 
     def _install_processing_form(self):
-        self.processing_form = ProcessingForm(self._form_values)
+        self.processing_form = ProcessingForm(
+            self._form_values, dependencies=self._form_dependencies
+        )
         self.install_screen(self.processing_form, "processing-form")
 
     def on_input_submitted(self, event: Input.Submitted):
         event.input.has_focus = False
         self.screen.focused = None
 
     def on_button_pressed(self, event: Button.Pressed):
@@ -433,15 +435,18 @@
         if self._multigrid_watcher:
             self._multigrid_watcher.stop()
         self._clear_state()
         self.exit()
         exit()
 
     async def action_clear(self) -> None:
-        if self.rsync_processes:
+        machine_config = get_machine_config(
+            str(self._environment.url.geturl()), demo=self._environment.demo
+        )
+        if self.rsync_processes and machine_config.get("allow_removal"):
             sources = "\n".join(str(k) for k in self.rsync_processes.keys())
             prompt = f"Remove files from the following: {sources}"
             self.install_screen(
                 ConfirmScreen(
                     prompt,
                     pressed_callback=self._remove_data,
                     button_names={"launch": "Yes", "quit": "No"},
```

### Comparing `murfey-0.7.7/src/murfey/client/tui/controller.css` & `murfey-0.7.8/src/murfey/client/tui/controller.css`

 * *Files 2% similar despite different names*

```diff
@@ -280,33 +280,33 @@
     height: 100%;
     column-span: 4;
     row-span: 3;
     content-align: left top;
     background: gray;
 }
 
+#modality-select {
+    width: 100%;
+    height: 10%;
+}
+
 #selected-directories {
     width: 100%;
-    height:75%;
+    height:65%;
     column-span: 1;
     row-span: 2;
 }
 
 #switch-directory {
     width: 100%;
     height: 100%;
     column-span: 3;
     row-span: 1;
 }
 
-#superres {
-    width: 50%;
-    height: 10fr;
-}
-
 #label-directory {
     width: 100%;
     height: 100%;
     column-span: 1;
     row-span: 1;
     content-align: center middle;
     text-style: bold;
```

### Comparing `murfey-0.7.7/src/murfey/client/tui/progress.py` & `murfey-0.7.8/src/murfey/client/tui/progress.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/client/tui/screens.py` & `murfey-0.7.8/src/murfey/client/tui/screens.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 from __future__ import annotations
 
 # import contextlib
 import logging
 from datetime import datetime
 from pathlib import Path
-from typing import Callable, Dict, List, NamedTuple, OrderedDict, TypeVar
+from typing import Any, Callable, Dict, List, NamedTuple, OrderedDict, Type, TypeVar
 
 import procrunner
 import requests
 from pydantic import BaseModel, ValidationError
 from rich.box import SQUARE
 from rich.panel import Panel
 from textual.app import ScreenStackError
-from textual.containers import Vertical
+from textual.containers import VerticalScroll
 from textual.message import Message
 from textual.reactive import reactive
 from textual.screen import Screen
 from textual.widget import Widget
 from textual.widgets import (
     Button,
     DataTable,
     DirectoryTree,
     Footer,
     Header,
     Input,
     Label,
+    OptionList,
     Static,
     Switch,
     TextLog,
     Tree,
 )
 
-from murfey.client.analyser import Analyser
-from murfey.client.context import SPAContext
+from murfey.client.analyser import Analyser, spa_form_dependencies
+from murfey.client.context import SPAContext, TomographyContext
 from murfey.client.gain_ref import determine_gain_ref
 from murfey.client.instance_environment import (
     MurfeyInstanceEnvironment,
     global_env_lock,
 )
-from murfey.client.tui.forms import TUIFormValue
+from murfey.client.tui.forms import FormDependency
+from murfey.util import get_machine_config
+from murfey.util.models import DCParametersSPA, DCParametersTomo
 
 log = logging.getLogger("murfey.tui.screens")
 
 ReactiveType = TypeVar("ReactiveType")
 
 
 def determine_default_destination(
@@ -113,15 +116,15 @@
 class InputResponse(NamedTuple):
     question: str
     allowed_responses: List[str] | None = None
     default: str = ""
     callback: Callable | None = None
     key_change_callback: Callable | None = None
     kwargs: dict | None = None
-    form: OrderedDict[str, TUIFormValue] | None = None
+    form: OrderedDict[str, Any] | None = None
     model: BaseModel | None = None
 
 
 class LogBook(TextLog):
     class Log(Message):
         def __init__(self, log_renderable):
             self.renderable = log_renderable
@@ -160,22 +163,23 @@
     def __iter__(self):
         return iter(self._options)
 
     def __bool__(self):
         return bool(self._text)
 
 
-def validate_form(form: dict, model: BaseModel) -> dict:
+def validate_form(form: dict, model: BaseModel) -> bool:
     try:
-        validated = model(**form)
+        convert = lambda x: None if x == "None" else x
+        validated = model(**{k: convert(v) for k, v in form.items()})
         log.info(validated.dict())
-        return validated.dict()
+        return True
     except (AttributeError, ValidationError) as e:
         log.warning(f"Form validation failed: {str(e)}")
-        return {}
+        return False
 
 
 class _DirectoryTree(DirectoryTree):
     valid_selection = reactive(False)
 
     def __init__(self, *args, data_directories: dict | None = None, **kwargs):
         super().__init__(*args, **kwargs)
@@ -226,14 +230,15 @@
 
     def __init__(
         self, *args, basepath: Path = Path("."), add_basepath: bool = False, **kwargs
     ):
         super().__init__(*args, **kwargs)
         self._selected_dir = basepath
         self._add_basepath = add_basepath
+        self._context = SPAContext
 
     def compose(self):
         machine_data = requests.get(
             f"{self.app._environment.url.geturl()}/machine/"
         ).json()
         self._dir_tree = _DirectoryTree(
             str(self._selected_dir),
@@ -241,17 +246,19 @@
             if self.app._strict
             else {},
             id="dir-select",
         )
 
         yield self._dir_tree
         text_log = TextLog(id="selected-directories")
-        text_log_block = Vertical(
-            text_log, Button("Clear", id="clear"), id="selected-directories-vert"
-        )
+        widgets = [text_log, Button("Clear", id="clear")]
+        if self.app._multigrid:
+            widgets.append(Label("Data collection modality:"))
+            widgets.append(OptionList("SPA", "Tomography", id="modality-select"))
+        text_log_block = VerticalScroll(*widgets, id="selected-directories-vert")
         yield text_log_block
 
         text_log.write("Selected directories:\n")
         btn_disabled = True
         for d in machine_data.get("data_directories", {}).keys():
             if Path(self._dir_tree._selected_path).resolve().is_relative_to(d):
                 btn_disabled = False
@@ -284,14 +291,22 @@
             self.app._default_destinations[
                 source
             ] = f"{machine_data.get('rsync_module') or 'data'}/{datetime.now().year}"
         if self._launch_btn:
             self._launch_btn.disabled = False
         self.query_one("#selected-directories").write(str(source) + "\n")
 
+    def on_option_list_option_selected(self, event):
+        log.info(f"option selected: {event.option}")
+        if event.option.prompt == "Tomography":
+            log.info("switching context to tomo")
+            self._context = TomographyContext
+        elif event.option.prompt == "SPA":
+            self._context = SPAContext
+
     def on_button_pressed(self, event: Button.Pressed) -> None:
         if event.button.id == "quit":
             self.app.exit()
             exit()
         elif event.button.id == "add":
             self._add_directory(self._dir_tree._selected_path)
         elif event.button.id == "launch":
@@ -307,25 +322,29 @@
                     self.app.analysers,
                 )
                 visit_path = defd + f"/{text}"
                 if self.app._environment.processing_only_mode:
                     self.app._start_rsyncer(_default, visit_path=visit_path)
                 transfer_routes[s] = _default
             self.app.install_screen(
-                DestinationSelect(transfer_routes), "destination-select-screen"
+                DestinationSelect(
+                    transfer_routes, self._context, dependencies=spa_form_dependencies
+                ),
+                "destination-select-screen",
             )
             self.app.pop_screen()
             self.app.push_screen("destination-select-screen")
         elif event.button.id == "clear":
             sel_dir = self.query_one("#selected-directories")
             for line in sel_dir.lines[1:]:
                 source = Path(line.text)
                 if source in self.app._environment.sources:
                     self.app._environment.sources.remove(source)
-                    del self.app._default_destinations[source]
+                    if self.app._default_destinations.get(source):
+                        del self.app._default_destinations[source]
             sel_dir.clear()
             sel_dir.write("Selected directories:\n")
 
 
 class ConfirmScreen(Screen):
     def __init__(
         self,
@@ -372,66 +391,105 @@
             self._callback(params=self._params)
 
 
 class ProcessingForm(Screen):
     _form = reactive({})
     _vert = None
 
-    def __init__(self, form: dict, *args, **kwargs):
+    def __init__(
+        self,
+        form: dict,
+        *args,
+        dependencies: Dict[str, FormDependency] | None = None,
+        **kwargs,
+    ):
         super().__init__(*args, **kwargs)
         self._form = form
         self._inputs: Dict[Input, str] = {}
+        self._dependencies = dependencies or {}
 
     def compose(self):
         inputs = []
         analyser = list(self.app.analysers.values())[0]
         for k in analyser._context.user_params + analyser._context.metadata_params:
             t = k.label
             inputs.append(Label(t, classes="label"))
-            i = Input(placeholder=t, classes="input", id=f"input_{k.name}")
+            if self._form.get(k.name) in ("true", "True", True):
+                i = Switch(value=True, classes="input", id=f"switch_{k.name}")
+            elif self._form.get(k.name) in ("false", "False", False):
+                i = Switch(value=False, classes="input", id=f"switch_{k.name}")
+            else:
+                i = Input(placeholder=t, classes="input", id=f"input_{k.name}")
+                default = self._form.get(k.name)
+                i.value = "None" if default is None else default
             self._inputs[i] = k.name
-            default = self._form.get(k.name)
-            i.value = "None" if default is None else default
             inputs.append(i)
+        for i, k in self._inputs.items():
+            self._check_dependency(k, i.value)
         confirm_btn = Button("Confirm", id="confirm-btn")
         if self._form.get("motion_corr_binning") == "2":
-            self._vert = Vertical(
+            self._vert = VerticalScroll(
                 *inputs,
-                Label("Collected in super resoultion mode:"),
-                Switch(id="superres", value=True),
+                Label("Collected in super resoultion mode unbinned:"),
+                Switch(id="superres", value=True, classes="input"),
                 confirm_btn,
                 id="input-form",
             )
         else:
-            self._vert = Vertical(*inputs, confirm_btn, id="input-form")
+            self._vert = VerticalScroll(*inputs, confirm_btn, id="input-form")
         yield self._vert
-        # yield confirm_btn
 
     def _write_params(self, params: dict | None = None):
         if params:
             analyser = list(self.app.analysers.values())[0]
             for k in analyser._context.user_params + analyser._context.metadata_params:
                 self.app.query_one("#info").write(f"{k.label}: {params.get(k.name)}")
             self.app._start_dc(params)
 
     def on_switch_changed(self, event):
-        pix_size = self.query_one("#input_pixel_size_on_image")
-        motion_corr_binning = self.query_one("#input_motion_corr_binning")
-        if event.value:
-            pix_size.value = str(float(pix_size.value) / 2)
-            motion_corr_binning.value = "2"
+        if event.switch.id == "superres":
+            pix_size = self.query_one("#input_pixel_size_on_image")
+            motion_corr_binning = self.query_one("#input_motion_corr_binning")
+            if event.value:
+                pix_size.value = str(float(pix_size.value) / 2)
+                motion_corr_binning.value = "2"
+            else:
+                pix_size.value = str(float(pix_size.value) * 2)
+                motion_corr_binning.value = "1"
         else:
-            pix_size.value = str(float(pix_size.value) * 2)
-            motion_corr_binning.value = "1"
+            k = self._inputs[event.switch]
+            self._form[k] = event.value
+            self._check_dependency(k, event.value)
+
+    def _check_dependency(self, key: str, value: Any):
+        if x := self._dependencies.get(key):
+            for d, v in x.dependencies.items():
+                if value == x.trigger_value:
+                    self._form[d] = v
+                    for i, dk in self._inputs.items():
+                        if dk == d:
+                            i.value = v
+                            i.disabled = True
+                            break
+                else:
+                    for i, dk in self._inputs.items():
+                        if dk == d:
+                            i.disabled = False
+                            break
 
     def on_input_changed(self, event):
         k = self._inputs[event.input]
         self._form[k] = event.value
 
     def on_button_pressed(self, event):
+        if self.app.analysers.get(Path(self._form.get("source", ""))):
+            if model := self.app.analysers[Path(self._form["source"])].parameters_model:
+                valid = validate_form(self._form, model)
+                if not valid:
+                    return
         if "confirm" not in self.app._installed_screens:
             self.app.install_screen(
                 ConfirmScreen(
                     "Launch processing?",
                     params=self._form,
                     pressed_callback=self._write_params,
                 ),
@@ -461,15 +519,15 @@
             [
                 Button(e, id=f"btn-{self._name}-{e}", classes=f"btn-{self._name}")
                 for e in self._elements
             ]
             if self._elements
             else [Button("No elements found")]
         )
-        yield Vertical(*hovers, id=f"select-{self._name}")
+        yield VerticalScroll(*hovers, id=f"select-{self._name}")
         yield Static(self._switch_label, id=f"label-{self._name}")
         yield Switch(id=f"switch-{self._name}", value=self._switch_status)
 
     def on_switch_changed(self, event):
         self._switch_status = event.value
 
 
@@ -559,60 +617,76 @@
                 log.info(f"Would perform {' '.join(cmd)}")
             else:
                 gain_rsync = procrunner.run(cmd)
                 if gain_rsync.returncode:
                     log.warning(
                         f"Gain reference file {self._dir_tree._gain_reference} was not successfully transferred to {visit_path}/processing"
                     )
-        process_gain_response = requests.post(
-            url=f"{str(self.app._environment.url.geturl())}/visits/{self.app._environment.visit}/process_gain",
-            json={
-                "gain_ref": str(self._dir_tree._gain_reference),
-            },
-        )
-        if str(process_gain_response.status_code).startswith("4"):
-            log.warning(
-                f"Gain processing failed: status code {process_gain_response.status_code}"
-            )
-        else:
-            log.info(
-                f"Gain reference file {process_gain_response.json().get('gain_ref')}"
+            process_gain_response = requests.post(
+                url=f"{str(self.app._environment.url.geturl())}/visits/{self.app._environment.visit}/process_gain",
+                json={
+                    "gain_ref": str(self._dir_tree._gain_reference),
+                },
             )
-            self.app._environment.data_collection_parameters[
-                "gain_ref"
-            ] = process_gain_response.json().get("gain_ref")
+            if str(process_gain_response.status_code).startswith("4"):
+                log.warning(
+                    f"Gain processing failed: status code {process_gain_response.status_code}"
+                )
+            else:
+                log.info(
+                    f"Gain reference file {process_gain_response.json().get('gain_ref')}"
+                )
+                self.app._environment.data_collection_parameters[
+                    "gain_ref"
+                ] = process_gain_response.json().get("gain_ref")
         if self._switch_status:
             self.app.push_screen("directory-select")
         else:
             self.app.install_screen(LaunchScreen(basepath=Path("./")), "launcher")
             self.app.push_screen("launcher")
 
 
 class DirectorySelection(SwitchSelection):
     def __init__(self, directories: List[str], *args, **kwargs):
-        super().__init__("directory", directories, "Multigrid", *args, **kwargs)
+        super().__init__(
+            "directory",
+            directories,
+            "Automatically transfer and trigger processing for new directories (recommended for multigrid)",
+            *args,
+            **kwargs,
+        )
 
     def on_button_pressed(self, event: Button.Pressed):
         self.app._multigrid = self._switch_status
         visit_dir = Path(str(event.button.label)) / self.app._visit
         visit_dir.mkdir(exist_ok=True)
         (visit_dir / "atlas").mkdir(exist_ok=True)
         self.app.install_screen(
             LaunchScreen(basepath=visit_dir, add_basepath=True), "launcher"
         )
         self.app.pop_screen()
         self.app.push_screen("launcher")
 
 
 class DestinationSelect(Screen):
-    def __init__(self, transfer_routes: Dict[Path, str], *args, **kwargs):
+    def __init__(
+        self,
+        transfer_routes: Dict[Path, str],
+        context: Type[SPAContext] | Type[TomographyContext],
+        *args,
+        dependencies: Dict[str, FormDependency] | None = None,
+        **kwargs,
+    ):
         super().__init__(*args, **kwargs)
         self._transfer_routes = transfer_routes
         self._destination_overrides: Dict[Path, str] = {}
         self._user_params: Dict[str, str] = {}
+        self._dependencies = dependencies or {}
+        self._inputs: Dict[Input, str] = {}
+        self._context = context
 
     def compose(self):
         bulk = []
         if self.app._multigrid:
             for s in self._transfer_routes.keys():
                 for d in s.glob("*"):
                     if d.is_dir() and d.name != "atlas":
@@ -639,42 +713,98 @@
             for s, d in self._transfer_routes.items():
                 bulk.append(Label(f"Copy the source {s} to:"))
                 bulk.append(
                     Input(
                         value=d, id=f"destination-{str(s)}", classes="input-destination"
                     )
                 )
-        yield Vertical(*bulk, id="destination-holder")
+        yield VerticalScroll(*bulk, id="destination-holder")
         params_bulk = []
         if self.app._multigrid:
-            for k in SPAContext.user_params:
+            for k in self._context.user_params:
                 params_bulk.append(Label(k.label))
+                val = self.app._environment.data_collection_parameters.get(
+                    k.name
+                ) or str(k.default)
+                self._user_params[k.name] = val
+                if val in ("true", "True", True):
+                    i = Switch(value=True, id=k.name, classes="input-destination")
+                elif val in ("false", "False", False):
+                    i = Switch(value=False, id=k.name, classes="input-destination")
+                else:
+                    i = Input(value=val, id=k.name, classes="input-destination")
+                params_bulk.append(i)
+                self._inputs[i] = k.name
+            machine_config = get_machine_config(
+                str(self.app._environment.url.geturl()), demo=self.app._environment.demo
+            )
+            if machine_config.get("superres"):
                 params_bulk.append(
-                    Input(value=str(k.default), id=k.name, classes="input-destination")
+                    Label("Collected in super resoultion mode unbinned:")
+                )
+                params_bulk.append(
+                    Switch(
+                        value=False,
+                        id="superres-multigrid",
+                        classes="input-destination",
+                    )
                 )
-        yield Vertical(
+                self.app._environment.superres = False
+            for i, k in self._inputs.items():
+                self._check_dependency(k, i.value)
+        yield VerticalScroll(
             *params_bulk,
             id="user-params",
         )
         yield Button("Confirm", id="destination-btn")
 
+    def _check_dependency(self, key: str, value: Any):
+        if x := self._dependencies.get(key):
+            for d, v in x.dependencies.items():
+                if value == x.trigger_value:
+                    self._user_params[d] = str(v)
+                    for i, dk in self._inputs.items():
+                        if dk == d:
+                            i.value = v
+                            i.disabled = True
+                            break
+                else:
+                    for i, dk in self._inputs.items():
+                        if dk == d:
+                            i.disabled = False
+                            break
+
+    def on_switch_changed(self, event):
+        if event.switch.id == "superres-multigrid":
+            self.app._environment.superres = event.value
+        else:
+            for k in self._context.user_params:
+                if event.switch.id == k.name:
+                    self._user_params[k.name] = event.value
+                    self._check_dependency(k.name, event.value)
+
     def on_input_changed(self, event):
         if event.input.id.startswith("destination-"):
             if not self.app._multigrid:
                 self._transfer_routes[Path(event.input.id[12:])] = event.value
             else:
                 self._destination_overrides[Path(event.input.id[12:])] = event.value
         else:
-            for k in SPAContext.user_params:
+            for k in self._context.user_params:
                 if event.input.id == k.name:
                     self._user_params[k.name] = event.value
 
     def on_button_pressed(self, event):
-        if any(v == "None" for v in self._user_params.values()):
-            return
+        if self.app._multigrid:
+            if self._context == TomographyContext:
+                valid = validate_form(self._user_params, DCParametersTomo.Base)
+            else:
+                valid = validate_form(self._user_params, DCParametersSPA.Base)
+            if not valid:
+                return
         for s, d in self._transfer_routes.items():
             self.app._default_destinations[s] = d
             self.app._register_dc = True
             if self.app._multigrid:
                 for k, v in self._destination_overrides.items():
                     self.app._environment.destination_registry[k.name] = v
                 self.app._launch_multigrid_watcher(
@@ -706,15 +836,17 @@
             self.app._redirected_logger.text_log = self.app.log_book
             log.info("logger connected")
         self.app.hovers = (
             [Button(v, id="visit-btn") for v in self.app.visits]
             if len(self.app.visits)
             else [Button("No ongoing visits found")]
         )
-        self.app.processing_form = ProcessingForm(self.app._form_values)
+        self.app.processing_form = ProcessingForm(
+            self.app._form_values, dependencies=self.app._form_dependencies
+        )
         yield Header()
         info_widget = TextLog(id="info", markup=True)
         yield info_widget
         yield self.app.log_book
         info_widget.write("[bold]Welcome to Murfey[/bold]")
         self.app.processing_btn = Button(
             "Request processing",
```

### Comparing `murfey-0.7.7/src/murfey/client/tui/status_bar.py` & `murfey-0.7.8/src/murfey/client/tui/status_bar.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/client/update.py` & `murfey-0.7.8/src/murfey/client/update.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/client/watchdir.py` & `murfey-0.7.8/src/murfey/client/watchdir.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/client/watchdir_multigrid.py` & `murfey-0.7.8/src/murfey/client/watchdir_multigrid.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/client/websocket.py` & `murfey-0.7.8/src/murfey/client/websocket.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/server/__init__.py` & `murfey-0.7.8/src/murfey/server/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,148 +312,161 @@
                             message.get("movie_id"),
                         ]
                     },
                 )
 
 
 def feedback_callback(header: dict, message: dict) -> None:
-    record = None
-    if "environment" in message:
-        message = message["payload"]
-    if message["register"] == "motion_corrected":
-        global_state.update(
-            "motion_corrected_movies",
-            {
-                message.get("movie"): [
-                    message.get("mrc_out"),
-                    message.get("movie_id"),
-                ]
-            },
-            perform_state_update=False,
-        )
+    try:
+        record = None
+        if "environment" in message:
+            message = message["payload"]
+        if message["register"] == "motion_corrected":
+            global_state.update(
+                "motion_corrected_movies",
+                {
+                    message.get("movie"): [
+                        message.get("mrc_out"),
+                        message.get("movie_id"),
+                    ]
+                },
+                perform_state_update=False,
+            )
 
-        if _transport_object:
-            _transport_object.transport.ack(header)
-        return None
-    elif message["register"] == "data_collection_group":
-        record = DataCollectionGroup(
-            sessionId=message["session_id"],
-            experimentType=message["experiment_type"],
-            experimentTypeId=message["experiment_type_id"],
-        )
-        dcgid = _register(record, header)
-        if _transport_object:
+            if _transport_object:
+                _transport_object.transport.ack(header)
+            return None
+        elif message["register"] == "data_collection_group":
+            record = DataCollectionGroup(
+                sessionId=message["session_id"],
+                experimentType=message["experiment_type"],
+                experimentTypeId=message["experiment_type_id"],
+            )
+            dcgid = _register(record, header)
+            if _transport_object:
+                if dcgid is None:
+                    _transport_object.transport.nack(header)
+                    return None
+                if global_state.get("data_collection_group_ids") and isinstance(
+                    global_state["data_collection_group_ids"], dict
+                ):
+                    global_state["data_collection_group_ids"] = {
+                        **global_state["data_collection_group_ids"],
+                        message.get("tag"): dcgid,
+                    }
+                else:
+                    global_state["data_collection_group_ids"] = {
+                        message.get("tag"): dcgid
+                    }
+                _transport_object.transport.ack(header)
+            return None
+        elif message["register"] == "data_collection":
+            dcgid = global_state.get("data_collection_group_ids", {}).get(  # type: ignore
+                message["source"]
+            )
             if dcgid is None:
+                raise ValueError(
+                    f"No data collection group ID was found for image directory {message['image_directory']}"
+                )
+            record = DataCollection(
+                SESSIONID=message["session_id"],
+                experimenttype=message["experiment_type"],
+                imageDirectory=message["image_directory"],
+                imageSuffix=message["image_suffix"],
+                voltage=message["voltage"],
+                dataCollectionGroupId=dcgid,
+                pixelSizeOnImage=message["pixel_size"],
+                imageSizeX=message["image_size_x"],
+                imageSizeY=message["image_size_y"],
+                slitGapHorizontal=message.get("slit_width"),
+                magnification=message.get("magnification"),
+                exposureTime=message.get("exposure_time"),
+                totalExposedDose=message.get("total_exposed_dose"),
+                c2aperture=message.get("c2aperture"),
+                phasePlate=int(message.get("phase_plate", 0)),
+            )
+            dcid = _register(
+                record,
+                header,
+                tag=message.get("tag")
+                if message["experiment_type"] == "tomography"
+                else "",
+            )
+            if dcid is None and _transport_object:
                 _transport_object.transport.nack(header)
                 return None
-            if global_state.get("data_collection_group_ids") and isinstance(
-                global_state["data_collection_group_ids"], dict
+            logger.debug(f"registered: {message.get('tag')}")
+            if global_state.get("data_collection_ids") and isinstance(
+                global_state["data_collection_ids"], dict
             ):
-                global_state["data_collection_group_ids"] = {
-                    **global_state["data_collection_group_ids"],
-                    message.get("tag"): dcgid,
+                global_state["data_collection_ids"] = {
+                    **global_state["data_collection_ids"],
+                    message.get("tag"): dcid,
                 }
             else:
-                global_state["data_collection_group_ids"] = {message.get("tag"): dcgid}
-            _transport_object.transport.ack(header)
-        return None
-    elif message["register"] == "data_collection":
-        dcgid = global_state.get("data_collection_group_ids", {}).get(  # type: ignore
-            message["tag"]
-        )
-        if dcgid is None:
-            raise ValueError(
-                f"No data collection group ID was found for image directory {message['image_directory']}"
-            )
-        record = DataCollection(
-            SESSIONID=message["session_id"],
-            experimenttype=message["experiment_type"],
-            imageDirectory=message["image_directory"],
-            imageSuffix=message["image_suffix"],
-            voltage=message["voltage"],
-            dataCollectionGroupId=dcgid,
-            pixelSizeOnImage=message["pixel_size"],
-            imageSizeX=message["image_size_x"],
-            imageSizeY=message["image_size_y"],
-            slitGapHorizontal=message.get("slit_width"),
-            magnification=message.get("magnification"),
-            exposureTime=message.get("exposure_time"),
-            totalExposedDose=message.get("total_exposed_dose"),
-            c2aperture=message.get("c2aperture"),
-            phasePlate=int(message.get("phase_plate", 0)),
-        )
-        dcid = _register(record, header, tag=message.get("tag"))
-        if dcid is None and _transport_object:
-            _transport_object.transport.nack(header)
-            return None
-        logger.debug(f"registered: {message.get('tag')}")
-        if global_state.get("data_collection_ids") and isinstance(
-            global_state["data_collection_ids"], dict
-        ):
-            global_state["data_collection_ids"] = {
-                **global_state["data_collection_ids"],
-                message.get("tag"): dcid,
-            }
-        else:
-            global_state["data_collection_ids"] = {message.get("tag"): dcid}
-        if _transport_object:
-            _transport_object.transport.ack(header)
-        return None
-    elif message["register"] == "processing_job":
-        assert isinstance(global_state["data_collection_ids"], dict)
-        _dcid = global_state["data_collection_ids"][message["tag"]]
-        record = ProcessingJob(dataCollectionId=_dcid, recipe=message["recipe"])
-        if message.get("job_parameters"):
-            job_parameters = [
-                ProcessingJobParameter(parameterKey=k, parameterValue=v)
-                for k, v in message["job_parameters"].items()
-            ]
-            pid = _register(ExtendedRecord(record, job_parameters), header)
-        else:
-            pid = _register(record, header)
-        if pid is None and _transport_object:
-            _transport_object.transport.nack(header)
+                global_state["data_collection_ids"] = {message.get("tag"): dcid}
+            if _transport_object:
+                _transport_object.transport.ack(header)
             return None
-        if global_state.get("processing_job_ids"):
-            global_state["processing_job_ids"] = {
-                **global_state["processing_job_ids"],  # type: ignore
-                message.get("tag"): {
-                    **global_state["processing_job_ids"].get(message.get("tag"), {}),  # type: ignore
-                    message["recipe"]: pid,
-                },
-            }
-        else:
-            prids = {message["tag"]: {message["recipe"]: pid}}
-            global_state["processing_job_ids"] = prids
-        if message.get("job_parameters"):
-            return None
-        record = AutoProcProgram(processingJobId=pid)
-        appid = _register(record, header)
-        if appid is None and _transport_object:
-            _transport_object.transport.nack(header)
+        elif message["register"] == "processing_job":
+            assert isinstance(global_state["data_collection_ids"], dict)
+            _dcid = global_state["data_collection_ids"][message["tag"]]
+            record = ProcessingJob(dataCollectionId=_dcid, recipe=message["recipe"])
+            if message.get("job_parameters"):
+                job_parameters = [
+                    ProcessingJobParameter(parameterKey=k, parameterValue=v)
+                    for k, v in message["job_parameters"].items()
+                ]
+                pid = _register(ExtendedRecord(record, job_parameters), header)
+            else:
+                pid = _register(record, header)
+            if pid is None and _transport_object:
+                _transport_object.transport.nack(header)
+                return None
+            if global_state.get("processing_job_ids"):
+                global_state["processing_job_ids"] = {
+                    **global_state["processing_job_ids"],  # type: ignore
+                    message.get("tag"): {
+                        **global_state["processing_job_ids"].get(message.get("tag"), {}),  # type: ignore
+                        message["recipe"]: pid,
+                    },
+                }
+            else:
+                prids = {message["tag"]: {message["recipe"]: pid}}
+                global_state["processing_job_ids"] = prids
+            if message.get("job_parameters"):
+                return None
+            record = AutoProcProgram(processingJobId=pid)
+            appid = _register(record, header)
+            if appid is None and _transport_object:
+                _transport_object.transport.nack(header)
+                return None
+            if global_state.get("autoproc_program_ids"):
+                assert isinstance(global_state["autoproc_program_ids"], dict)
+                global_state["autoproc_program_ids"] = {
+                    **global_state["autoproc_program_ids"],
+                    message.get("tag"): {
+                        **global_state["processing_job_ids"].get(message.get("tag"), {}),  # type: ignore
+                        message["recipe"]: appid,
+                    },
+                }
+            else:
+                global_state["autoproc_program_ids"] = {
+                    message["tag"]: {message["recipe"]: appid}
+                }
+            if _transport_object:
+                _transport_object.transport.ack(header)
             return None
-        if global_state.get("autoproc_program_ids"):
-            assert isinstance(global_state["autoproc_program_ids"], dict)
-            global_state["autoproc_program_ids"] = {
-                **global_state["autoproc_program_ids"],
-                message.get("tag"): {
-                    **global_state["processing_job_ids"].get(message.get("tag"), {}),  # type: ignore
-                    message["recipe"]: appid,
-                },
-            }
-        else:
-            global_state["autoproc_program_ids"] = {
-                message["tag"]: {message["recipe"]: appid}
-            }
         if _transport_object:
-            _transport_object.transport.ack(header)
+            _transport_object.transport.nack(header, requeue=False)
         return None
-    if _transport_object:
-        _transport_object.transport.nack(header, requeue=False)
-    return None
+    except Exception:
+        logger.warning(
+            "Exception encountered in server RabbitMQ callback", exc_info=True
+        )
 
 
 @singledispatch
 def _register(record, header: dict, **kwargs):
     raise NotImplementedError(f"Not method to register {record} or type {type(record)}")
```

### Comparing `murfey-0.7.7/src/murfey/server/api.py` & `murfey-0.7.8/src/murfey/server/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,19 @@
     conn.close()
     return {
         "ispyb_connection": True,
         "rabbitmq_connection": _transport_object.transport.is_connected(),
     }
 
 
+@router.get("/connections/")
+def connections_check():
+    return {"connections": list(ws.manager.active_connections.keys())}
+
+
 @lru_cache(maxsize=1)
 @router.get("/machine/")
 def machine_info():
     if settings.murfey_machine_configuration:
         microscope = get_microscope()
         print(from_file(settings.murfey_machine_configuration, microscope))
         return from_file(settings.murfey_machine_configuration, microscope)
@@ -416,15 +421,15 @@
         "image_size_x": dc_params.image_size_x,
         "image_size_y": dc_params.image_size_y,
         "acquisition_software": dc_params.acquisition_software,
         "tag": dc_params.tag,
         "source": dc_params.source,
         "magnification": dc_params.magnification,
         "total_exposed_dose": dc_params.total_exposed_dose,
-        "c2paerture": dc_params.c2aperture,
+        "c2aperture": dc_params.c2aperture,
         "exposure_time": dc_params.exposure_time,
         "slit_width": dc_params.slit_width,
         "phase_plate": dc_params.phase_plate,
     }
 
     if _transport_object:
         log.debug(
```

### Comparing `murfey-0.7.7/src/murfey/server/bootstrap.py` & `murfey-0.7.8/src/murfey/server/bootstrap.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/server/config.py` & `murfey-0.7.8/src/murfey/server/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,13 +17,14 @@
     rsync_module: str = ""
     gain_reference_directory: Optional[Path] = None
     processed_directory_name: str = "processed"
     feedback_queue: str = "murfey_feedback"
     superres: bool = False
     camera: str = "FALCON"
     data_required_substrings: Dict[str, List[str]] = {}
+    allow_removal: bool = False
 
 
 def from_file(config_file_path: Path, microscope: str) -> MachineConfig:
     with open(config_file_path, "r") as config_stream:
         config = yaml.safe_load(config_stream)
     return MachineConfig(**config.get(microscope, {}))
```

### Comparing `murfey-0.7.7/src/murfey/server/demo_api.py` & `murfey-0.7.8/src/murfey/server/demo_api.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/server/gain.py` & `murfey-0.7.8/src/murfey/server/gain.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/server/ispyb.py` & `murfey-0.7.8/src/murfey/server/ispyb.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/server/main.py` & `murfey-0.7.8/src/murfey/server/main.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/server/websocket.py` & `murfey-0.7.8/src/murfey/server/websocket.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/templates/activevisits.html` & `murfey-0.7.8/src/murfey/templates/activevisits.html`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/templates/base.html` & `murfey-0.7.8/src/murfey/templates/base.html`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/templates/bootstrap.html` & `murfey-0.7.8/src/murfey/templates/bootstrap.html`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/templates/images/diamond.png` & `murfey-0.7.8/src/murfey/templates/images/diamond.png`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/templates/images/icon_268.png` & `murfey-0.7.8/src/murfey/templates/images/icon_268.png`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/templates/static/styles.css` & `murfey-0.7.8/src/murfey/templates/static/styles.css`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/templates/visit.html` & `murfey-0.7.8/src/murfey/templates/visit.html`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/util/__init__.py` & `murfey-0.7.8/src/murfey/util/__init__.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/util/dummy_setup.py` & `murfey-0.7.8/src/murfey/util/dummy_setup.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/util/file_monitor.py` & `murfey-0.7.8/src/murfey/util/file_monitor.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/util/mdoc.py` & `murfey-0.7.8/src/murfey/util/mdoc.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/util/models.py` & `murfey-0.7.8/src/murfey/util/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,40 +118,56 @@
     image_size_y: int
     pixel_size_on_image: str
     motion_corr_binning: int
     manual_tilt_offset: float
     file_extension: str
     acquisition_software: str
 
+    class Base(BaseModel):
+        dose_per_frame: float
+        gain_ref: Optional[str]
+        manual_tilt_offset: float
+
 
 class DCParametersSPA(BaseModel):
     dose_per_frame: float
     gain_ref: Optional[str]
     experiment_type: str
     voltage: float
     image_size_x: int
     image_size_y: int
     pixel_size_on_image: str
     motion_corr_binning: int
     file_extension: str
     acquisition_software: str
     use_cryolo: bool
     symmetry: str
-    mask_diameter: int
-    boxsize: int
+    mask_diameter: Optional[int]
+    boxsize: Optional[int]
     downscale: bool
-    small_boxsize: int
+    small_boxsize: Optional[int]
     eer_grouping: int
     magnification: Optional[int] = None
     total_exposed_dose: Optional[float] = None
     c2aperture: Optional[float] = None
     exposure_time: Optional[float] = None
     slit_width: Optional[float] = None
     phase_plate: bool = False
 
+    class Base(BaseModel):
+        dose_per_frame: float
+        gain_ref: Optional[str]
+        use_cryolo: bool
+        symmetry: str
+        mask_diameter: Optional[int]
+        boxsize: Optional[int]
+        downscale: bool
+        small_boxsize: Optional[int]
+        eer_grouping: int
+
 
 class ProcessingJobParameters(BaseModel):
     tag: str
     recipe: str
     parameters: Dict[str, Any] = {}
```

### Comparing `murfey-0.7.7/src/murfey/util/rsync.py` & `murfey-0.7.8/src/murfey/util/rsync.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey/util/state.py` & `murfey-0.7.8/src/murfey/util/state.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.7/src/murfey.egg-info/PKG-INFO` & `murfey-0.7.8/src/murfey.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: murfey
-Version: 0.7.7
+Version: 0.7.8
 Summary: Client-Server architecture hauling Cryo-EM data
 License: BSD
 Project-URL: Bug-Tracker, https://github.com/DiamondLightSource/python-murfey/issues
 Project-URL: Documentation, https://github.com/DiamondLightSource/python-murfey
 Project-URL: GitHub, https://github.com/DiamondLightSource/python-murfey
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `murfey-0.7.7/src/murfey.egg-info/SOURCES.txt` & `murfey-0.7.8/src/murfey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

