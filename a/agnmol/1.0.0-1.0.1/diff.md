# Comparing `tmp/agnmol-1.0.0.tar.gz` & `tmp/agnmol-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agnmol-1.0.0.tar", last modified: Sat Apr 15 15:34:34 2023, max compression
+gzip compressed data, was "agnmol-1.0.1.tar", last modified: Sun Apr 16 15:14:37 2023, max compression
```

## Comparing `agnmol-1.0.0.tar` & `agnmol-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 15:34:34.668901 agnmol-1.0.0/
--rw-rw-rw-   0        0        0     1091 2023-04-15 15:33:58.000000 agnmol-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0      458 2023-04-15 15:34:34.665905 agnmol-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       69 2023-04-15 15:33:51.000000 agnmol-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 15:34:34.652898 agnmol-1.0.0/agnmol/
--rw-rw-rw-   0        0        0        0 2023-04-15 14:55:12.000000 agnmol-1.0.0/agnmol/__init__.py
--rw-rw-rw-   0        0        0      764 2023-04-15 15:17:57.000000 agnmol-1.0.0/agnmol/motion.py
-drwxrwxrwx   0        0        0        0 2023-04-15 15:34:34.662900 agnmol-1.0.0/agnmol.egg-info/
--rw-rw-rw-   0        0        0      458 2023-04-15 15:34:34.000000 agnmol-1.0.0/agnmol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-04-15 15:34:34.000000 agnmol-1.0.0/agnmol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 15:34:34.000000 agnmol-1.0.0/agnmol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-15 15:34:34.000000 agnmol-1.0.0/agnmol.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      461 2023-04-15 15:32:43.000000 agnmol-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 15:34:34.669900 agnmol-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 15:14:37.690675 agnmol-1.0.1/
+-rw-rw-rw-   0        0        0     1091 2023-04-15 15:33:58.000000 agnmol-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1367 2023-04-16 15:14:37.689674 agnmol-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      978 2023-04-16 15:09:05.000000 agnmol-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 15:14:37.664683 agnmol-1.0.1/agnmol/
+-rw-rw-rw-   0        0        0        0 2023-04-15 14:55:12.000000 agnmol-1.0.1/agnmol/__init__.py
+-rw-rw-rw-   0        0        0      823 2023-04-16 15:13:05.000000 agnmol-1.0.1/agnmol/motion.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:14:37.688673 agnmol-1.0.1/agnmol.egg-info/
+-rw-rw-rw-   0        0        0     1367 2023-04-16 15:14:37.000000 agnmol-1.0.1/agnmol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-04-16 15:14:37.000000 agnmol-1.0.1/agnmol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 15:14:37.000000 agnmol-1.0.1/agnmol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-16 15:14:37.000000 agnmol-1.0.1/agnmol.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      461 2023-04-16 15:13:35.000000 agnmol-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 15:14:37.690675 agnmol-1.0.1/setup.cfg
```

### Comparing `agnmol-1.0.0/LICENSE.txt` & `agnmol-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `agnmol-1.0.0/agnmol/motion.py` & `agnmol-1.0.1/agnmol/motion.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import math
+
+
 def acceleration(v_delta, t, vf, vi):
     if v_delta and t:
         return v_delta / t
     elif vi and vf and t:
         return (vf - vi) / t
     else:
         return 0
@@ -10,22 +13,22 @@
     if x_delta and t:
         return x_delta / t
     elif vi and vf:
         return (vf - vi) / 2
     else:
         return 0
 
-def v_final(vi, a, t, x_delta):
+def v_final(vi, a, t=math.inf, x_delta=math.inf):
     if not vi or not a:
         return 0
 
-    if t:
+    if t != math.inf:
         return vi + a * t
 
-    if x_delta:
+    if x_delta != math.inf:
         return vi ** 2 + 2 * a * x_delta
 
     return 0
 
 def change_in_position(vi, t, a):
     if vi and t and a:
         return vi * t + 0.5 * a * (t ** 2)
```

