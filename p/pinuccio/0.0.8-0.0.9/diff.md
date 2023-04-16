# Comparing `tmp/pinuccio-0.0.8.tar.gz` & `tmp/pinuccio-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinuccio-0.0.8.tar", last modified: Wed Mar 22 19:37:40 2023, max compression
+gzip compressed data, was "pinuccio-0.0.9.tar", last modified: Wed Mar 22 20:53:08 2023, max compression
```

## Comparing `pinuccio-0.0.8.tar` & `pinuccio-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-22 19:37:40.040326 pinuccio-0.0.8/
--rw-rw-r--   0 user      (1000) user      (1000)      182 2023-03-22 19:37:40.040326 pinuccio-0.0.8/PKG-INFO
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-22 19:37:40.040326 pinuccio-0.0.8/pinuccio/
--rw-rw-r--   0 user      (1000) user      (1000)      443 2023-03-22 15:39:18.850335 pinuccio-0.0.8/pinuccio/SThread.py
--rw-rw-r--   0 user      (1000) user      (1000)       54 2023-03-22 15:39:18.850335 pinuccio-0.0.8/pinuccio/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      887 2023-03-22 15:39:18.850335 pinuccio-0.0.8/pinuccio/client.py
--rw-rw-r--   0 user      (1000) user      (1000)     2246 2023-03-22 15:39:18.850335 pinuccio-0.0.8/pinuccio/interface.py
--rw-rw-r--   0 user      (1000) user      (1000)     5586 2023-03-22 19:29:31.323104 pinuccio-0.0.8/pinuccio/server.py
--rw-rw-r--   0 user      (1000) user      (1000)      389 2023-03-22 15:39:18.850335 pinuccio-0.0.8/pinuccio/status.py
--rw-rw-r--   0 user      (1000) user      (1000)      117 2023-03-22 19:33:51.227219 pinuccio-0.0.8/pinuccio/utils.py
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-03-22 19:25:09.410284 pinuccio-0.0.8/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      135 2023-03-22 19:37:32.375597 pinuccio-0.0.8/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-22 20:53:08.872790 pinuccio-0.0.9/
+-rw-rw-r--   0 user      (1000) user      (1000)      182 2023-03-22 20:53:08.872790 pinuccio-0.0.9/PKG-INFO
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-22 20:53:08.872790 pinuccio-0.0.9/pinuccio/
+-rw-rw-r--   0 user      (1000) user      (1000)      443 2023-03-22 15:39:18.850335 pinuccio-0.0.9/pinuccio/SThread.py
+-rw-rw-r--   0 user      (1000) user      (1000)       54 2023-03-22 15:39:18.850335 pinuccio-0.0.9/pinuccio/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1067 2023-03-22 20:52:03.774853 pinuccio-0.0.9/pinuccio/client.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2246 2023-03-22 15:39:18.850335 pinuccio-0.0.9/pinuccio/interface.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5586 2023-03-22 19:29:31.323104 pinuccio-0.0.9/pinuccio/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)      389 2023-03-22 15:39:18.850335 pinuccio-0.0.9/pinuccio/status.py
+-rw-rw-r--   0 user      (1000) user      (1000)      117 2023-03-22 19:33:51.227219 pinuccio-0.0.9/pinuccio/utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-03-22 19:25:09.410284 pinuccio-0.0.9/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      135 2023-03-22 20:52:54.272351 pinuccio-0.0.9/setup.py
```

### Comparing `pinuccio-0.0.8/pinuccio/interface.py` & `pinuccio-0.0.9/pinuccio/interface.py`

 * *Files identical despite different names*

### Comparing `pinuccio-0.0.8/pinuccio/server.py` & `pinuccio-0.0.9/pinuccio/server.py`

 * *Files identical despite different names*

