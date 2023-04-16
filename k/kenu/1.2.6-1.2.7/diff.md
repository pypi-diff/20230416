# Comparing `tmp/kenu-1.2.6.tar.gz` & `tmp/kenu-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kenu-1.2.6.tar", last modified: Sun Apr 16 14:15:25 2023, max compression
+gzip compressed data, was "kenu-1.2.7.tar", last modified: Sun Apr 16 16:15:48 2023, max compression
```

## Comparing `kenu-1.2.6.tar` & `kenu-1.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 14:15:25.817033 kenu-1.2.6/
--rw-rw-rw-   0        0        0      122 2023-04-16 14:15:25.815052 kenu-1.2.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 14:15:25.768163 kenu-1.2.6/kenu/
--rw-rw-rw-   0        0        0     5025 2023-03-24 18:10:30.000000 kenu-1.2.6/kenu/__init__.py
--rw-rw-rw-   0        0        0     8177 2023-03-31 17:35:51.000000 kenu-1.2.6/kenu/__main__.py
--rw-rw-rw-   0        0        0     4043 2023-04-16 14:15:17.000000 kenu-1.2.6/kenu/connect.py
-drwxrwxrwx   0        0        0        0 2023-04-16 14:15:25.811048 kenu-1.2.6/kenu.egg-info/
--rw-rw-rw-   0        0        0      122 2023-04-16 14:15:25.000000 kenu-1.2.6/kenu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-04-16 14:15:25.000000 kenu-1.2.6/kenu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 14:15:25.000000 kenu-1.2.6/kenu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-04-16 14:15:25.000000 kenu-1.2.6/kenu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-04-16 14:15:25.000000 kenu-1.2.6/kenu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-16 14:15:25.000000 kenu-1.2.6/kenu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 14:15:25.817033 kenu-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0      423 2023-04-16 14:15:09.000000 kenu-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:15:48.561185 kenu-1.2.7/
+-rw-rw-rw-   0        0        0      122 2023-04-16 16:15:48.559190 kenu-1.2.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 16:15:48.516305 kenu-1.2.7/kenu/
+-rw-rw-rw-   0        0        0     5025 2023-03-24 18:10:30.000000 kenu-1.2.7/kenu/__init__.py
+-rw-rw-rw-   0        0        0     8177 2023-03-31 17:35:51.000000 kenu-1.2.7/kenu/__main__.py
+-rw-rw-rw-   0        0        0     4125 2023-04-16 16:15:29.000000 kenu-1.2.7/kenu/connect.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:15:48.556203 kenu-1.2.7/kenu.egg-info/
+-rw-rw-rw-   0        0        0      122 2023-04-16 16:15:48.000000 kenu-1.2.7/kenu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-04-16 16:15:48.000000 kenu-1.2.7/kenu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 16:15:48.000000 kenu-1.2.7/kenu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-04-16 16:15:48.000000 kenu-1.2.7/kenu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-04-16 16:15:48.000000 kenu-1.2.7/kenu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-16 16:15:48.000000 kenu-1.2.7/kenu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 16:15:48.561185 kenu-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      423 2023-04-16 16:15:41.000000 kenu-1.2.7/setup.py
```

### Comparing `kenu-1.2.6/kenu/__init__.py` & `kenu-1.2.7/kenu/__init__.py`

 * *Files identical despite different names*

### Comparing `kenu-1.2.6/kenu/__main__.py` & `kenu-1.2.7/kenu/__main__.py`

 * *Files identical despite different names*

### Comparing `kenu-1.2.6/kenu/connect.py` & `kenu-1.2.7/kenu/connect.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,21 +9,23 @@
 import ctypes
 from plyer import notification
 import os
 import loadwave
 
 def main():
     arg = sys.argv[1]
+    PORT = 5050
     if(arg == "kenu-1"):
-        connectserver(arg)
+        HOST = "20.238.119.193"
+        connectserver(arg, HOST)
     else:
         print("This server is invalid.")
         exit()
-    HOST = "20.238.119.193"
-    PORT = 5050
+    
+    
     try:
         client_id = '1085214791771111485'
         RPC = pypresence.Presence(client_id)
         RPC.connect()
     except Exception as e:
         pass
 
@@ -87,19 +89,19 @@
             rpcupdate("in lobby")
 
                     
             return True
         else:
             return False
 
-    def start_client():
+    def start_client(server):
         try:
             global client
             client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-            client.connect((HOST, PORT))
+            client.connect((server, PORT))
             signin()
             if login() == False:
                 print("Try again. \n")
                 signin()
             receive_thread = threading.Thread(target=handle_receive)
             receive_thread.start()
         except Exception as e:
@@ -115,16 +117,17 @@
                 print("Closing connection...")
                 client.close()
                 sys.exit()
             except:
                 client.close()
                 sys.exit()
 
-    start_client()
+    
 
-def connectserver(server):
-    print("Connecting to the server. - " + server)
-    connectserverld()
-
-@loadwave.process
-def connectserverld():
-    time.sleep(3.5)
+    def connectserver(servername, server):
+        print("Connecting to the server. - " + server)
+        connectserverld()
+        start_client(server)
+
+    @loadwave.process
+    def connectserverld():
+        time.sleep(3.5)
```

