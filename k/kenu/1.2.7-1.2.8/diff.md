# Comparing `tmp/kenu-1.2.7.tar.gz` & `tmp/kenu-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kenu-1.2.7.tar", last modified: Sun Apr 16 16:15:48 2023, max compression
+gzip compressed data, was "kenu-1.2.8.tar", last modified: Sun Apr 16 16:22:36 2023, max compression
```

## Comparing `kenu-1.2.7.tar` & `kenu-1.2.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 16:15:48.561185 kenu-1.2.7/
--rw-rw-rw-   0        0        0      122 2023-04-16 16:15:48.559190 kenu-1.2.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 16:15:48.516305 kenu-1.2.7/kenu/
--rw-rw-rw-   0        0        0     5025 2023-03-24 18:10:30.000000 kenu-1.2.7/kenu/__init__.py
--rw-rw-rw-   0        0        0     8177 2023-03-31 17:35:51.000000 kenu-1.2.7/kenu/__main__.py
--rw-rw-rw-   0        0        0     4125 2023-04-16 16:15:29.000000 kenu-1.2.7/kenu/connect.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:15:48.556203 kenu-1.2.7/kenu.egg-info/
--rw-rw-rw-   0        0        0      122 2023-04-16 16:15:48.000000 kenu-1.2.7/kenu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-04-16 16:15:48.000000 kenu-1.2.7/kenu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 16:15:48.000000 kenu-1.2.7/kenu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-04-16 16:15:48.000000 kenu-1.2.7/kenu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-04-16 16:15:48.000000 kenu-1.2.7/kenu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-16 16:15:48.000000 kenu-1.2.7/kenu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 16:15:48.561185 kenu-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0      423 2023-04-16 16:15:41.000000 kenu-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:22:36.619826 kenu-1.2.8/
+-rw-rw-rw-   0        0        0      122 2023-04-16 16:22:36.618830 kenu-1.2.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 16:22:36.575942 kenu-1.2.8/kenu/
+-rw-rw-rw-   0        0        0     5025 2023-03-24 18:10:30.000000 kenu-1.2.8/kenu/__init__.py
+-rw-rw-rw-   0        0        0     8177 2023-03-31 17:35:51.000000 kenu-1.2.8/kenu/__main__.py
+-rw-rw-rw-   0        0        0     4106 2023-04-16 16:22:16.000000 kenu-1.2.8/kenu/connect.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:22:36.614839 kenu-1.2.8/kenu.egg-info/
+-rw-rw-rw-   0        0        0      122 2023-04-16 16:22:36.000000 kenu-1.2.8/kenu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-04-16 16:22:36.000000 kenu-1.2.8/kenu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 16:22:36.000000 kenu-1.2.8/kenu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-04-16 16:22:36.000000 kenu-1.2.8/kenu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-04-16 16:22:36.000000 kenu-1.2.8/kenu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-16 16:22:36.000000 kenu-1.2.8/kenu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 16:22:36.620822 kenu-1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      423 2023-04-16 16:22:30.000000 kenu-1.2.8/setup.py
```

### Comparing `kenu-1.2.7/kenu/__init__.py` & `kenu-1.2.8/kenu/__init__.py`

 * *Files identical despite different names*

### Comparing `kenu-1.2.7/kenu/__main__.py` & `kenu-1.2.8/kenu/__main__.py`

 * *Files identical despite different names*

### Comparing `kenu-1.2.7/kenu/connect.py` & `kenu-1.2.8/kenu/connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
                 sys.exit()
             except:
                 client.close()
                 sys.exit()
 
     
 
-    def connectserver(servername, server):
-        print("Connecting to the server. - " + server)
-        connectserverld()
-        start_client(server)
+def connectserver(servername, server):
+    print("Connecting to the server. - " + servername)
+    connectserverld()
+    main.start_client(server)
 
-    @loadwave.process
-    def connectserverld():
-        time.sleep(3.5)
+@loadwave.process
+def connectserverld():
+    time.sleep(3.5)
```

