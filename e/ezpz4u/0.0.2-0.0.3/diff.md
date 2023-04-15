# Comparing `tmp/ezpz4u-0.0.2.tar.gz` & `tmp/ezpz4u-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezpz4u-0.0.2.tar", last modified: Sat Apr 15 21:38:51 2023, max compression
+gzip compressed data, was "ezpz4u-0.0.3.tar", last modified: Sat Apr 15 23:48:57 2023, max compression
```

## Comparing `ezpz4u-0.0.2.tar` & `ezpz4u-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 steam     (1001) steam     (1001)        0 2023-04-15 21:38:51.653621 ezpz4u-0.0.2/
--rw-rw-r--   0 steam     (1001) steam     (1001)      263 2023-04-15 21:38:51.653621 ezpz4u-0.0.2/PKG-INFO
--rw-rw-r--   0 steam     (1001) steam     (1001)      737 2023-04-15 21:21:16.000000 ezpz4u-0.0.2/README.md
-drwxrwxr-x   0 steam     (1001) steam     (1001)        0 2023-04-15 21:38:51.653621 ezpz4u-0.0.2/ezpz4u.egg-info/
--rw-rw-r--   0 steam     (1001) steam     (1001)      263 2023-04-15 21:38:51.000000 ezpz4u-0.0.2/ezpz4u.egg-info/PKG-INFO
--rw-rw-r--   0 steam     (1001) steam     (1001)      254 2023-04-15 21:38:51.000000 ezpz4u-0.0.2/ezpz4u.egg-info/SOURCES.txt
--rw-rw-r--   0 steam     (1001) steam     (1001)        1 2023-04-15 21:38:51.000000 ezpz4u-0.0.2/ezpz4u.egg-info/dependency_links.txt
--rw-rw-r--   0 steam     (1001) steam     (1001)       48 2023-04-15 21:38:51.000000 ezpz4u-0.0.2/ezpz4u.egg-info/entry_points.txt
--rw-rw-r--   0 steam     (1001) steam     (1001)      102 2023-04-15 21:38:51.000000 ezpz4u-0.0.2/ezpz4u.egg-info/requires.txt
--rw-rw-r--   0 steam     (1001) steam     (1001)        3 2023-04-15 21:38:51.000000 ezpz4u-0.0.2/ezpz4u.egg-info/top_level.txt
--rw-rw-r--   0 steam     (1001) steam     (1001)      497 2023-04-15 21:38:42.000000 ezpz4u-0.0.2/pyproject.toml
-drwxrwxr-x   0 steam     (1001) steam     (1001)        0 2023-04-15 21:38:51.653621 ezpz4u-0.0.2/pz/
--rw-rw-r--   0 steam     (1001) steam     (1001)        0 2023-04-15 17:07:26.000000 ezpz4u-0.0.2/pz/__init__.py
--rw-rw-r--   0 steam     (1001) steam     (1001)      398 2023-04-15 17:26:12.000000 ezpz4u-0.0.2/pz/config.py
--rw-rw-r--   0 steam     (1001) steam     (1001)     2415 2023-04-15 21:21:16.000000 ezpz4u-0.0.2/pz/main.py
--rw-rw-r--   0 steam     (1001) steam     (1001)     2731 2023-04-15 21:21:16.000000 ezpz4u-0.0.2/pz/pz.py
--rw-rw-r--   0 steam     (1001) steam     (1001)       38 2023-04-15 21:38:51.653621 ezpz4u-0.0.2/setup.cfg
+drwxrwxr-x   0 steam     (1001) steam     (1001)        0 2023-04-15 23:48:57.060429 ezpz4u-0.0.3/
+-rw-rw-r--   0 steam     (1001) steam     (1001)      263 2023-04-15 23:48:57.060429 ezpz4u-0.0.3/PKG-INFO
+-rw-rw-r--   0 steam     (1001) steam     (1001)     1336 2023-04-15 23:38:03.000000 ezpz4u-0.0.3/README.md
+drwxrwxr-x   0 steam     (1001) steam     (1001)        0 2023-04-15 23:48:57.056429 ezpz4u-0.0.3/ezpz4u.egg-info/
+-rw-rw-r--   0 steam     (1001) steam     (1001)      263 2023-04-15 23:48:57.000000 ezpz4u-0.0.3/ezpz4u.egg-info/PKG-INFO
+-rw-rw-r--   0 steam     (1001) steam     (1001)      254 2023-04-15 23:48:57.000000 ezpz4u-0.0.3/ezpz4u.egg-info/SOURCES.txt
+-rw-rw-r--   0 steam     (1001) steam     (1001)        1 2023-04-15 23:48:57.000000 ezpz4u-0.0.3/ezpz4u.egg-info/dependency_links.txt
+-rw-rw-r--   0 steam     (1001) steam     (1001)       48 2023-04-15 23:48:57.000000 ezpz4u-0.0.3/ezpz4u.egg-info/entry_points.txt
+-rw-rw-r--   0 steam     (1001) steam     (1001)      102 2023-04-15 23:48:57.000000 ezpz4u-0.0.3/ezpz4u.egg-info/requires.txt
+-rw-rw-r--   0 steam     (1001) steam     (1001)        3 2023-04-15 23:48:57.000000 ezpz4u-0.0.3/ezpz4u.egg-info/top_level.txt
+-rw-rw-r--   0 steam     (1001) steam     (1001)      497 2023-04-15 22:38:36.000000 ezpz4u-0.0.3/pyproject.toml
+drwxrwxr-x   0 steam     (1001) steam     (1001)        0 2023-04-15 23:48:57.060429 ezpz4u-0.0.3/pz/
+-rw-rw-r--   0 steam     (1001) steam     (1001)        0 2023-04-15 22:07:56.000000 ezpz4u-0.0.3/pz/__init__.py
+-rw-rw-r--   0 steam     (1001) steam     (1001)      319 2023-04-15 22:38:36.000000 ezpz4u-0.0.3/pz/config.py
+-rw-rw-r--   0 steam     (1001) steam     (1001)     2242 2023-04-15 23:38:03.000000 ezpz4u-0.0.3/pz/main.py
+-rw-rw-r--   0 steam     (1001) steam     (1001)     3067 2023-04-15 23:47:55.000000 ezpz4u-0.0.3/pz/pz.py
+-rw-rw-r--   0 steam     (1001) steam     (1001)       38 2023-04-15 23:48:57.060429 ezpz4u-0.0.3/setup.cfg
```

### Comparing `ezpz4u-0.0.2/pz/main.py` & `ezpz4u-0.0.3/pz/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -54,19 +54,14 @@
         return pz.restart_server()
 
 @app.get("/server/update_mods")
 def stop_server(username: Annotated[str, Depends(get_current_username)]):
     if username == "admin":
         return pz.update_server_mods()
 
-@app.get("/server/update_server")
-def update_server(username: Annotated[str, Depends(get_current_username)]):
-    if username == "admin":
-        return pz.update_server()
-
 @app.get("/server/stats")
 def update_server():
     return pz.get_stats_server()
 
 def start_server():
     uvicorn.run(
         app,
```

