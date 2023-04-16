# Comparing `tmp/kenu-1.2.9.tar.gz` & `tmp/kenu-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kenu-1.2.9.tar", last modified: Sun Apr 16 16:24:53 2023, max compression
+gzip compressed data, was "kenu-1.3.4.tar", last modified: Sun Apr 16 16:25:55 2023, max compression
```

## Comparing `kenu-1.2.9.tar` & `kenu-1.3.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 16:24:53.038084 kenu-1.2.9/
--rw-rw-rw-   0        0        0      122 2023-04-16 16:24:53.036087 kenu-1.2.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 16:24:52.981232 kenu-1.2.9/kenu/
--rw-rw-rw-   0        0        0     5025 2023-03-24 18:10:30.000000 kenu-1.2.9/kenu/__init__.py
--rw-rw-rw-   0        0        0     8177 2023-03-31 17:35:51.000000 kenu-1.2.9/kenu/__main__.py
--rw-rw-rw-   0        0        0     3803 2023-04-16 16:24:44.000000 kenu-1.2.9/kenu/connect.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:24:53.032096 kenu-1.2.9/kenu.egg-info/
--rw-rw-rw-   0        0        0      122 2023-04-16 16:24:52.000000 kenu-1.2.9/kenu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-04-16 16:24:52.000000 kenu-1.2.9/kenu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 16:24:52.000000 kenu-1.2.9/kenu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-04-16 16:24:52.000000 kenu-1.2.9/kenu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-04-16 16:24:52.000000 kenu-1.2.9/kenu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-16 16:24:52.000000 kenu-1.2.9/kenu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 16:24:53.038084 kenu-1.2.9/setup.cfg
--rw-rw-rw-   0        0        0      423 2023-04-16 16:24:47.000000 kenu-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:25:55.805057 kenu-1.3.4/
+-rw-rw-rw-   0        0        0      122 2023-04-16 16:25:55.803063 kenu-1.3.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 16:25:55.761208 kenu-1.3.4/kenu/
+-rw-rw-rw-   0        0        0     5025 2023-03-24 18:10:30.000000 kenu-1.3.4/kenu/__init__.py
+-rw-rw-rw-   0        0        0     8177 2023-03-31 17:35:51.000000 kenu-1.3.4/kenu/__main__.py
+-rw-rw-rw-   0        0        0     3798 2023-04-16 16:25:44.000000 kenu-1.3.4/kenu/connect.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:25:55.799073 kenu-1.3.4/kenu.egg-info/
+-rw-rw-rw-   0        0        0      122 2023-04-16 16:25:55.000000 kenu-1.3.4/kenu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-04-16 16:25:55.000000 kenu-1.3.4/kenu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 16:25:55.000000 kenu-1.3.4/kenu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-04-16 16:25:55.000000 kenu-1.3.4/kenu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-04-16 16:25:55.000000 kenu-1.3.4/kenu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-16 16:25:55.000000 kenu-1.3.4/kenu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 16:25:55.806055 kenu-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      423 2023-04-16 16:25:51.000000 kenu-1.3.4/setup.py
```

### Comparing `kenu-1.2.9/kenu/__init__.py` & `kenu-1.3.4/kenu/__init__.py`

 * *Files identical despite different names*

### Comparing `kenu-1.2.9/kenu/__main__.py` & `kenu-1.3.4/kenu/__main__.py`

 * *Files identical despite different names*

### Comparing `kenu-1.2.9/kenu/connect.py` & `kenu-1.3.4/kenu/connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,12 +124,12 @@
             sys.exit()
 
     
 
 def connectserver(servername, server):
     print("Connecting to the server. - " + servername)
     connectserverld()
-    main.start_client(server)
+    start_client(server)
 
 @loadwave.process
 def connectserverld():
     time.sleep(3.5)
```

