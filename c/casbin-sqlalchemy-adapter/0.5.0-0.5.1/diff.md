# Comparing `tmp/casbin_sqlalchemy_adapter-0.5.0.tar.gz` & `tmp/casbin_sqlalchemy_adapter-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casbin_sqlalchemy_adapter-0.5.0.tar", last modified: Sun Jul 17 07:08:15 2022, max compression
+gzip compressed data, was "casbin_sqlalchemy_adapter-0.5.1.tar", last modified: Sun Apr 16 01:48:19 2023, max compression
```

## Comparing `casbin_sqlalchemy_adapter-0.5.0.tar` & `casbin_sqlalchemy_adapter-0.5.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-17 07:08:15.226640 casbin_sqlalchemy_adapter-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-07-17 07:07:42.000000 casbin_sqlalchemy_adapter-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2951 2022-07-17 07:08:15.226640 casbin_sqlalchemy_adapter-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2248 2022-07-17 07:07:42.000000 casbin_sqlalchemy_adapter-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-17 07:08:15.226640 casbin_sqlalchemy_adapter-0.5.0/casbin_sqlalchemy_adapter/
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-07-17 07:07:42.000000 casbin_sqlalchemy_adapter-0.5.0/casbin_sqlalchemy_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9641 2022-07-17 07:07:42.000000 casbin_sqlalchemy_adapter-0.5.0/casbin_sqlalchemy_adapter/adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-17 07:08:15.226640 casbin_sqlalchemy_adapter-0.5.0/casbin_sqlalchemy_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2951 2022-07-17 07:08:15.000000 casbin_sqlalchemy_adapter-0.5.0/casbin_sqlalchemy_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-07-17 07:08:15.000000 casbin_sqlalchemy_adapter-0.5.0/casbin_sqlalchemy_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-17 07:08:15.000000 casbin_sqlalchemy_adapter-0.5.0/casbin_sqlalchemy_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-07-17 07:08:15.000000 casbin_sqlalchemy_adapter-0.5.0/casbin_sqlalchemy_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-07-17 07:08:15.000000 casbin_sqlalchemy_adapter-0.5.0/casbin_sqlalchemy_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-07-17 07:08:15.226640 casbin_sqlalchemy_adapter-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1443 2022-07-17 07:07:42.000000 casbin_sqlalchemy_adapter-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 01:48:19.460608 casbin_sqlalchemy_adapter-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-16 01:47:39.000000 casbin_sqlalchemy_adapter-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-16 01:48:19.464608 casbin_sqlalchemy_adapter-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-16 01:47:39.000000 casbin_sqlalchemy_adapter-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 01:48:19.460608 casbin_sqlalchemy_adapter-0.5.1/casbin_sqlalchemy_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 01:47:39.000000 casbin_sqlalchemy_adapter-0.5.1/casbin_sqlalchemy_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-04-16 01:47:39.000000 casbin_sqlalchemy_adapter-0.5.1/casbin_sqlalchemy_adapter/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 01:48:19.460608 casbin_sqlalchemy_adapter-0.5.1/casbin_sqlalchemy_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-16 01:48:19.000000 casbin_sqlalchemy_adapter-0.5.1/casbin_sqlalchemy_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-16 01:48:19.000000 casbin_sqlalchemy_adapter-0.5.1/casbin_sqlalchemy_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 01:48:19.000000 casbin_sqlalchemy_adapter-0.5.1/casbin_sqlalchemy_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-16 01:48:19.000000 casbin_sqlalchemy_adapter-0.5.1/casbin_sqlalchemy_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-16 01:48:19.000000 casbin_sqlalchemy_adapter-0.5.1/casbin_sqlalchemy_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-16 01:48:19.464608 casbin_sqlalchemy_adapter-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-16 01:47:39.000000 casbin_sqlalchemy_adapter-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 01:48:19.460608 casbin_sqlalchemy_adapter-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    16896 2023-04-16 01:47:39.000000 casbin_sqlalchemy_adapter-0.5.1/tests/test_adapter.py
```

### Comparing `casbin_sqlalchemy_adapter-0.5.0/LICENSE` & `casbin_sqlalchemy_adapter-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `casbin_sqlalchemy_adapter-0.5.0/PKG-INFO` & `casbin_sqlalchemy_adapter-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin_sqlalchemy_adapter
-Version: 0.5.0
+Version: 0.5.1
 Summary: SQLAlchemy Adapter for PyCasbin
 Home-page: https://github.com/pycasbin/sqlalchemy-adapter
 Author: TechLee
 Author-email: techlee@qq.com
 License: Apache 2.0
 Keywords: casbin,SQLAlchemy,casbin-adapter,rbac,access control,abac,acl,permission
 Classifier: Programming Language :: Python :: 3.5
@@ -51,22 +51,22 @@
 
 ```python
 import casbin_sqlalchemy_adapter
 import casbin
 
 adapter = casbin_sqlalchemy_adapter.Adapter('sqlite:///test.db')
 
-e = casbin.Enforcer('path/to/model.conf', adapter, True)
+e = casbin.Enforcer('path/to/model.conf', adapter)
 
 sub = "alice"  # the user that wants to access a resource.
 obj = "data1"  # the resource that is going to be accessed.
 act = "read"  # the operation that the user performs on the resource.
 
 if e.enforce(sub, obj, act):
-    # permit alice to read data1casbin_sqlalchemy_adapter
+    # permit alice to read data1
     pass
 else:
     # deny the request, show an error
     pass
 ```
```

### Comparing `casbin_sqlalchemy_adapter-0.5.0/README.md` & `casbin_sqlalchemy_adapter-0.5.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -31,22 +31,22 @@
 
 ```python
 import casbin_sqlalchemy_adapter
 import casbin
 
 adapter = casbin_sqlalchemy_adapter.Adapter('sqlite:///test.db')
 
-e = casbin.Enforcer('path/to/model.conf', adapter, True)
+e = casbin.Enforcer('path/to/model.conf', adapter)
 
 sub = "alice"  # the user that wants to access a resource.
 obj = "data1"  # the resource that is going to be accessed.
 act = "read"  # the operation that the user performs on the resource.
 
 if e.enforce(sub, obj, act):
-    # permit alice to read data1casbin_sqlalchemy_adapter
+    # permit alice to read data1
     pass
 else:
     # deny the request, show an error
     pass
 ```
```

### Comparing `casbin_sqlalchemy_adapter-0.5.0/casbin_sqlalchemy_adapter/adapter.py` & `casbin_sqlalchemy_adapter-0.5.1/casbin_sqlalchemy_adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `casbin_sqlalchemy_adapter-0.5.0/casbin_sqlalchemy_adapter.egg-info/PKG-INFO` & `casbin_sqlalchemy_adapter-0.5.1/casbin_sqlalchemy_adapter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin-sqlalchemy-adapter
-Version: 0.5.0
+Version: 0.5.1
 Summary: SQLAlchemy Adapter for PyCasbin
 Home-page: https://github.com/pycasbin/sqlalchemy-adapter
 Author: TechLee
 Author-email: techlee@qq.com
 License: Apache 2.0
 Keywords: casbin,SQLAlchemy,casbin-adapter,rbac,access control,abac,acl,permission
 Classifier: Programming Language :: Python :: 3.5
@@ -51,22 +51,22 @@
 
 ```python
 import casbin_sqlalchemy_adapter
 import casbin
 
 adapter = casbin_sqlalchemy_adapter.Adapter('sqlite:///test.db')
 
-e = casbin.Enforcer('path/to/model.conf', adapter, True)
+e = casbin.Enforcer('path/to/model.conf', adapter)
 
 sub = "alice"  # the user that wants to access a resource.
 obj = "data1"  # the resource that is going to be accessed.
 act = "read"  # the operation that the user performs on the resource.
 
 if e.enforce(sub, obj, act):
-    # permit alice to read data1casbin_sqlalchemy_adapter
+    # permit alice to read data1
     pass
 else:
     # deny the request, show an error
     pass
 ```
```

### Comparing `casbin_sqlalchemy_adapter-0.5.0/setup.py` & `casbin_sqlalchemy_adapter-0.5.1/setup.py`

 * *Files identical despite different names*

