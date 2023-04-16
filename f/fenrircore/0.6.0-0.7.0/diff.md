# Comparing `tmp/fenrircore-0.6.0.tar.gz` & `tmp/fenrircore-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenrircore-0.6.0.tar", last modified: Wed Apr 12 19:41:59 2023, max compression
+gzip compressed data, was "fenrircore-0.7.0.tar", last modified: Sun Apr 16 10:05:11 2023, max compression
```

## Comparing `fenrircore-0.6.0.tar` & `fenrircore-0.7.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-12 19:41:59.361579 fenrircore-0.6.0/
--rw-r--r--   0 hannes    (1000) users      (100)    18092 2023-02-17 12:58:30.000000 fenrircore-0.6.0/LICENSE
--rw-r--r--   0 hannes    (1000) users      (100)      492 2023-04-12 19:41:59.361579 fenrircore-0.6.0/PKG-INFO
--rw-r--r--   0 hannes    (1000) users      (100)     1673 2023-04-10 18:38:00.000000 fenrircore-0.6.0/README.md
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-12 19:41:59.361579 fenrircore-0.6.0/fenrircore/
--rw-r--r--   0 hannes    (1000) users      (100)       22 2023-04-12 19:39:27.000000 fenrircore-0.6.0/fenrircore/__init__.py
--rw-r--r--   0 hannes    (1000) users      (100)       65 2023-04-10 17:56:19.000000 fenrircore-0.6.0/fenrircore/__main__.py
--rw-r--r--   0 hannes    (1000) users      (100)    11033 2023-04-10 18:38:00.000000 fenrircore-0.6.0/fenrircore/arper.py
--rw-r--r--   0 hannes    (1000) users      (100)     6868 2023-04-10 18:38:00.000000 fenrircore-0.6.0/fenrircore/fenrir.py
--rw-r--r--   0 hannes    (1000) users      (100)     7516 2023-04-12 19:39:27.000000 fenrircore-0.6.0/fenrircore/filehandler.py
--rw-r--r--   0 hannes    (1000) users      (100)     4923 2023-04-10 18:38:00.000000 fenrircore-0.6.0/fenrircore/firewall.py
--rw-r--r--   0 hannes    (1000) users      (100)     2019 2023-04-10 18:38:00.000000 fenrircore-0.6.0/fenrircore/getmacvendors.py
--rw-r--r--   0 hannes    (1000) users      (100)     8258 2023-04-10 18:38:00.000000 fenrircore-0.6.0/fenrircore/scanner.py
--rw-r--r--   0 hannes    (1000) users      (100)    11909 2023-04-12 19:39:27.000000 fenrircore-0.6.0/fenrircore/vpn.py
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-12 19:41:59.361579 fenrircore-0.6.0/fenrircore.egg-info/
--rw-r--r--   0 hannes    (1000) users      (100)      492 2023-04-12 19:41:59.000000 fenrircore-0.6.0/fenrircore.egg-info/PKG-INFO
--rw-r--r--   0 hannes    (1000) users      (100)      469 2023-04-12 19:41:59.000000 fenrircore-0.6.0/fenrircore.egg-info/SOURCES.txt
--rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-12 19:41:59.000000 fenrircore-0.6.0/fenrircore.egg-info/dependency_links.txt
--rw-r--r--   0 hannes    (1000) users      (100)       50 2023-04-12 19:41:59.000000 fenrircore-0.6.0/fenrircore.egg-info/entry_points.txt
--rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-02 11:09:58.000000 fenrircore-0.6.0/fenrircore.egg-info/not-zip-safe
--rw-r--r--   0 hannes    (1000) users      (100)       54 2023-04-12 19:41:59.000000 fenrircore-0.6.0/fenrircore.egg-info/requires.txt
--rw-r--r--   0 hannes    (1000) users      (100)       11 2023-04-12 19:41:59.000000 fenrircore-0.6.0/fenrircore.egg-info/top_level.txt
--rw-r--r--   0 hannes    (1000) users      (100)       38 2023-04-12 19:41:59.361579 fenrircore-0.6.0/setup.cfg
--rw-r--r--   0 hannes    (1000) users      (100)      897 2023-04-12 19:39:27.000000 fenrircore-0.6.0/setup.py
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-16 10:05:11.745950 fenrircore-0.7.0/
+-rw-r--r--   0 hannes    (1000) users      (100)    18092 2023-02-17 12:58:30.000000 fenrircore-0.7.0/LICENSE
+-rw-r--r--   0 hannes    (1000) users      (100)      492 2023-04-16 10:05:11.745950 fenrircore-0.7.0/PKG-INFO
+-rw-r--r--   0 hannes    (1000) users      (100)     1673 2023-04-10 18:38:00.000000 fenrircore-0.7.0/README.md
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-16 10:05:11.741950 fenrircore-0.7.0/fenrircore/
+-rw-r--r--   0 hannes    (1000) users      (100)       22 2023-04-16 09:57:58.000000 fenrircore-0.7.0/fenrircore/__init__.py
+-rw-r--r--   0 hannes    (1000) users      (100)       65 2023-04-10 17:56:19.000000 fenrircore-0.7.0/fenrircore/__main__.py
+-rw-r--r--   0 hannes    (1000) users      (100)    11033 2023-04-10 18:38:00.000000 fenrircore-0.7.0/fenrircore/arper.py
+-rw-r--r--   0 hannes    (1000) users      (100)     6868 2023-04-10 18:38:00.000000 fenrircore-0.7.0/fenrircore/fenrir.py
+-rw-r--r--   0 hannes    (1000) users      (100)     7516 2023-04-12 19:39:27.000000 fenrircore-0.7.0/fenrircore/filehandler.py
+-rw-r--r--   0 hannes    (1000) users      (100)     4923 2023-04-10 18:38:00.000000 fenrircore-0.7.0/fenrircore/firewall.py
+-rw-r--r--   0 hannes    (1000) users      (100)     2019 2023-04-10 18:38:00.000000 fenrircore-0.7.0/fenrircore/getmacvendors.py
+-rw-r--r--   0 hannes    (1000) users      (100)     8383 2023-04-14 08:38:02.000000 fenrircore-0.7.0/fenrircore/scanner.py
+-rw-r--r--   0 hannes    (1000) users      (100)    11909 2023-04-12 19:39:27.000000 fenrircore-0.7.0/fenrircore/vpn.py
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-16 10:05:11.745950 fenrircore-0.7.0/fenrircore.egg-info/
+-rw-r--r--   0 hannes    (1000) users      (100)      492 2023-04-16 10:05:11.000000 fenrircore-0.7.0/fenrircore.egg-info/PKG-INFO
+-rw-r--r--   0 hannes    (1000) users      (100)      469 2023-04-16 10:05:11.000000 fenrircore-0.7.0/fenrircore.egg-info/SOURCES.txt
+-rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-16 10:05:11.000000 fenrircore-0.7.0/fenrircore.egg-info/dependency_links.txt
+-rw-r--r--   0 hannes    (1000) users      (100)       50 2023-04-16 10:05:11.000000 fenrircore-0.7.0/fenrircore.egg-info/entry_points.txt
+-rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-02 11:09:58.000000 fenrircore-0.7.0/fenrircore.egg-info/not-zip-safe
+-rw-r--r--   0 hannes    (1000) users      (100)       54 2023-04-16 10:05:11.000000 fenrircore-0.7.0/fenrircore.egg-info/requires.txt
+-rw-r--r--   0 hannes    (1000) users      (100)       11 2023-04-16 10:05:11.000000 fenrircore-0.7.0/fenrircore.egg-info/top_level.txt
+-rw-r--r--   0 hannes    (1000) users      (100)       38 2023-04-16 10:05:11.745950 fenrircore-0.7.0/setup.cfg
+-rw-r--r--   0 hannes    (1000) users      (100)      897 2023-04-12 19:39:27.000000 fenrircore-0.7.0/setup.py
```

### Comparing `fenrircore-0.6.0/LICENSE` & `fenrircore-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fenrircore-0.6.0/README.md` & `fenrircore-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `fenrircore-0.6.0/fenrircore/arper.py` & `fenrircore-0.7.0/fenrircore/arper.py`

 * *Files identical despite different names*

### Comparing `fenrircore-0.6.0/fenrircore/fenrir.py` & `fenrircore-0.7.0/fenrircore/fenrir.py`

 * *Files identical despite different names*

### Comparing `fenrircore-0.6.0/fenrircore/filehandler.py` & `fenrircore-0.7.0/fenrircore/filehandler.py`

 * *Files identical despite different names*

### Comparing `fenrircore-0.6.0/fenrircore/firewall.py` & `fenrircore-0.7.0/fenrircore/firewall.py`

 * *Files identical despite different names*

### Comparing `fenrircore-0.6.0/fenrircore/getmacvendors.py` & `fenrircore-0.7.0/fenrircore/getmacvendors.py`

 * *Files identical despite different names*

### Comparing `fenrircore-0.6.0/fenrircore/scanner.py` & `fenrircore-0.7.0/fenrircore/scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ipaddress import ip_network
 from . getmacvendors import getvendorformac
 from . arper import getmydefaultgws
 from socket import AF_INET
 from datetime import datetime
 from time import time, sleep
 from sqlite3 import connect, OperationalError, Cursor
-from logging import info, debug, basicConfig, INFO, DEBUG
+from logging import info, debug, basicConfig, getLogger, INFO, DEBUG
 from sys import stdout
 from argparse import ArgumentParser
 from signal import signal, SIGINT, SIGTERM
 
 
 class Scanner:
     """ class to handle MACAddress/IP scanning
@@ -159,14 +159,15 @@
         :param singleshot: abort scan after 1 scan if set to True
         :param debug: set logging to debug if true
 
         initialize logging and map singals to doend method
         start scanning with given parameters
         """
         basicConfig(stream=stdout, level=DEBUG if debuglog else INFO)
+        getLogger('pyroute2').propagate = False
         signal(SIGINT, self.doend)
         signal(SIGTERM, self.doend)
         info('statring device scanning...')
         self.continousupdate(singleshot=singleshot)
         info('device scanning stoped.')
 
 
@@ -197,20 +198,18 @@
 def main() -> None:
     """ main method
 
     parse given commandline arguments
     start Firewall
     """
     parser = ArgumentParser()
-    parser.add_argument(
-        '--singleshot', help='exit after first completed scan', action='store_true')
-    parser.add_argument(
-        '--print', help='print found devices int network (implies --singleshot)', action='store_true')
-    parser.add_argument(
-        '--interface', help='interface for device scanning', default='eth0')
+    parser.add_argument('--singleshot', help='exit after first completed scan', action='store_true')
+    parser.add_argument('--print', help='print found devices int network (implies --singleshot)', action='store_true')
+    parser.add_argument('--interface', help='interface for device scanning', default='eth0')
+    parser.add_argument('--interface', help='interface for device scanning', default='eth0')
     parser.add_argument('--debug', help='activate debug logging', action='store_true')
     args = parser.parse_args()
     if args.print:
         return printresults(args.interface)
     scan(interface=args.interface, singleshot=args.singleshot, debug=args.debug)
```

### Comparing `fenrircore-0.6.0/fenrircore/vpn.py` & `fenrircore-0.7.0/fenrircore/vpn.py`

 * *Files identical despite different names*

### Comparing `fenrircore-0.6.0/setup.py` & `fenrircore-0.7.0/setup.py`

 * *Files identical despite different names*

