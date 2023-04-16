# Comparing `tmp/kenu-1.2.5.tar.gz` & `tmp/kenu-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kenu-1.2.5.tar", last modified: Sun Apr 16 14:11:21 2023, max compression
+gzip compressed data, was "kenu-1.2.6.tar", last modified: Sun Apr 16 14:15:25 2023, max compression
```

## Comparing `kenu-1.2.5.tar` & `kenu-1.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 14:11:21.491537 kenu-1.2.5/
--rw-rw-rw-   0        0        0      122 2023-04-16 14:11:21.489542 kenu-1.2.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 14:11:21.457627 kenu-1.2.5/kenu/
--rw-rw-rw-   0        0        0     5025 2023-03-24 18:10:30.000000 kenu-1.2.5/kenu/__init__.py
--rw-rw-rw-   0        0        0     8177 2023-03-31 17:35:51.000000 kenu-1.2.5/kenu/__main__.py
--rw-rw-rw-   0        0        0     4027 2023-04-16 14:03:32.000000 kenu-1.2.5/kenu/connect.py
-drwxrwxrwx   0        0        0        0 2023-04-16 14:11:21.487547 kenu-1.2.5/kenu.egg-info/
--rw-rw-rw-   0        0        0      122 2023-04-16 14:11:21.000000 kenu-1.2.5/kenu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-04-16 14:11:21.000000 kenu-1.2.5/kenu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 14:11:21.000000 kenu-1.2.5/kenu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-04-16 14:11:21.000000 kenu-1.2.5/kenu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-04-16 14:11:21.000000 kenu-1.2.5/kenu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-16 14:11:21.000000 kenu-1.2.5/kenu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 14:11:21.492536 kenu-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0      423 2023-04-16 14:11:13.000000 kenu-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:15:25.817033 kenu-1.2.6/
+-rw-rw-rw-   0        0        0      122 2023-04-16 14:15:25.815052 kenu-1.2.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 14:15:25.768163 kenu-1.2.6/kenu/
+-rw-rw-rw-   0        0        0     5025 2023-03-24 18:10:30.000000 kenu-1.2.6/kenu/__init__.py
+-rw-rw-rw-   0        0        0     8177 2023-03-31 17:35:51.000000 kenu-1.2.6/kenu/__main__.py
+-rw-rw-rw-   0        0        0     4043 2023-04-16 14:15:17.000000 kenu-1.2.6/kenu/connect.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:15:25.811048 kenu-1.2.6/kenu.egg-info/
+-rw-rw-rw-   0        0        0      122 2023-04-16 14:15:25.000000 kenu-1.2.6/kenu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-04-16 14:15:25.000000 kenu-1.2.6/kenu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 14:15:25.000000 kenu-1.2.6/kenu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-04-16 14:15:25.000000 kenu-1.2.6/kenu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-04-16 14:15:25.000000 kenu-1.2.6/kenu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-16 14:15:25.000000 kenu-1.2.6/kenu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 14:15:25.817033 kenu-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      423 2023-04-16 14:15:09.000000 kenu-1.2.6/setup.py
```

### Comparing `kenu-1.2.5/kenu/__init__.py` & `kenu-1.2.6/kenu/__init__.py`

 * *Files identical despite different names*

### Comparing `kenu-1.2.5/kenu/__main__.py` & `kenu-1.2.6/kenu/__main__.py`

 * *Files identical despite different names*

### Comparing `kenu-1.2.5/kenu/connect.py` & `kenu-1.2.6/kenu/connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 def main():
     arg = sys.argv[1]
     if(arg == "kenu-1"):
         connectserver(arg)
     else:
         print("This server is invalid.")
+        exit()
     HOST = "20.238.119.193"
     PORT = 5050
     try:
         client_id = '1085214791771111485'
         RPC = pypresence.Presence(client_id)
         RPC.connect()
     except Exception as e:
```

