# Comparing `tmp/pymstodo-0.0.8.tar.gz` & `tmp/pymstodo-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymstodo-0.0.8.tar", last modified: Sun Apr  4 12:02:41 2021, max compression
+gzip compressed data, was "dist/pymstodo-0.0.9.tar", last modified: Mon May  3 10:14:51 2021, max compression
```

## Comparing `pymstodo-0.0.8.tar` & `pymstodo-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-04 12:02:41.000000 pymstodo-0.0.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2354 2021-04-04 12:02:41.000000 pymstodo-0.0.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1382 2021-04-04 12:02:23.000000 pymstodo-0.0.8/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-04 12:02:41.000000 pymstodo-0.0.8/pymstodo/
--rw-rw-r--   0 travis    (2000) travis    (2000)       51 2021-04-04 12:02:23.000000 pymstodo-0.0.8/pymstodo/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10313 2021-04-04 12:02:23.000000 pymstodo-0.0.8/pymstodo/client.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-04 12:02:41.000000 pymstodo-0.0.8/pymstodo.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2354 2021-04-04 12:02:41.000000 pymstodo-0.0.8/pymstodo.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      217 2021-04-04 12:02:41.000000 pymstodo-0.0.8/pymstodo.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-04-04 12:02:41.000000 pymstodo-0.0.8/pymstodo.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       25 2021-04-04 12:02:41.000000 pymstodo-0.0.8/pymstodo.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2021-04-04 12:02:41.000000 pymstodo-0.0.8/pymstodo.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-04-04 12:02:41.000000 pymstodo-0.0.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1297 2021-04-04 12:02:23.000000 pymstodo-0.0.8/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-03 10:14:51.000000 pymstodo-0.0.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35149 2021-05-03 10:14:34.000000 pymstodo-0.0.9/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2354 2021-05-03 10:14:51.000000 pymstodo-0.0.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1382 2021-05-03 10:14:34.000000 pymstodo-0.0.9/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-03 10:14:51.000000 pymstodo-0.0.9/pymstodo/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       51 2021-05-03 10:14:34.000000 pymstodo-0.0.9/pymstodo/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11016 2021-05-03 10:14:34.000000 pymstodo-0.0.9/pymstodo/client.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-03 10:14:51.000000 pymstodo-0.0.9/pymstodo.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2354 2021-05-03 10:14:51.000000 pymstodo-0.0.9/pymstodo.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      225 2021-05-03 10:14:51.000000 pymstodo-0.0.9/pymstodo.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-05-03 10:14:51.000000 pymstodo-0.0.9/pymstodo.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       25 2021-05-03 10:14:51.000000 pymstodo-0.0.9/pymstodo.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2021-05-03 10:14:51.000000 pymstodo-0.0.9/pymstodo.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-05-03 10:14:51.000000 pymstodo-0.0.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1297 2021-05-03 10:14:34.000000 pymstodo-0.0.9/setup.py
```

### Comparing `pymstodo-0.0.8/PKG-INFO` & `pymstodo-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymstodo
-Version: 0.0.8
+Version: 0.0.9
 Summary: Microsoft To Do API client
 Home-page: https://github.com/inbalboa/pymstodo
 Author: Sergey Shlyapugin
 Author-email: shlyapugin@gmail.com
 License: GPLv3
 Description: # pymstodo ✔️
         [![PyPI](https://img.shields.io/pypi/v/pymstodo.svg)](https://pypi.org/project/pymstodo/) [![Build Status](https://travis-ci.org/inbalboa/pymstodo.svg?branch=master)](https://travis-ci.org/inbalboa/pymstodo) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
```

### Comparing `pymstodo-0.0.8/README.md` & `pymstodo-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pymstodo-0.0.8/pymstodo/client.py` & `pymstodo-0.0.9/pymstodo/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -143,19 +143,19 @@
         if now >= expire_time:
             token_url = f'{ToDoConnection._authority}{ToDoConnection._token_endpoint}'
             oa_sess = OAuth2Session(self.client_id, scope=ToDoConnection._scope,
                                     token=self.token, redirect_uri=ToDoConnection._redirect)
             new_token = oa_sess.refresh_token(token_url, client_id=self.client_id, client_secret=self.client_secret)
             self.token = new_token
 
-    def get_lists(self) -> Optional[List[TaskList]]:
+    def get_lists(self, limit: Optional[int] = 99) -> Optional[List[TaskList]]:
         """Get all task lists."""
         self._refresh_token()
         oa_sess = OAuth2Session(self.client_id, scope=ToDoConnection._scope, token=self.token)
-        resp = oa_sess.get(f'{ToDoConnection._base_api_url}lists?top=99')
+        resp = oa_sess.get(f'{ToDoConnection._base_api_url}lists?$top={limit}')
         if not resp.ok:
             raise PymstodoError(f'Error {resp.status_code}: {resp.reason}')
 
         contents = json.loads(resp.content.decode())['value']
         lists = [TaskList(**list_data) for list_data in contents]
 
         return lists
@@ -202,19 +202,29 @@
         oa_sess = OAuth2Session(self.client_id, scope=ToDoConnection._scope, token=self.token)
         resp = oa_sess.delete(f'{ToDoConnection._base_api_url}lists/{list_id}')
         if not resp.ok:
             raise PymstodoError(f'Error {resp.status_code}: {resp.reason}')
 
         return resp.ok
 
-    def get_tasks(self, list_id: str) -> Optional[List[Task]]:
-        """Get all uncompleted tasks for the list."""
+    def get_tasks(self, list_id: str, limit: Optional[int] = 99, status: Optional[str] = None) -> Optional[List[Task]]:
+        """Get all tasks for the list."""
         self._refresh_token()
         oa_sess = OAuth2Session(self.client_id, scope=ToDoConnection._scope, token=self.token)
-        resp = oa_sess.get(f"{ToDoConnection._base_api_url}lists/{list_id}/tasks?top=99&$filter=status ne 'completed'")
+        if status:
+            if status=='all':
+                resp = oa_sess.get(f"{ToDoConnection._base_api_url}lists/{list_id}/tasks?$top={limit}")
+            elif status=='completed':
+                resp = oa_sess.get(f"{ToDoConnection._base_api_url}lists/{list_id}/tasks?$top={limit}&$filter=status eq 'completed'")
+            elif status=='notCompleted':
+                resp = oa_sess.get(f"{ToDoConnection._base_api_url}lists/{list_id}/tasks?$top={limit}&$filter=status ne 'completed'")
+            else:
+                raise PymstodoError(f'{status} is an unexpected status parameter')
+        else:
+            resp = oa_sess.get(f"{ToDoConnection._base_api_url}lists/{list_id}/tasks?$top={limit}&$filter=status ne 'completed'")
         if not resp.ok:
             raise PymstodoError(f'Error {resp.status_code}: {resp.reason}')
 
         contents = json.loads(resp.content.decode())['value']
         tasks = [Task(**task_data) for task_data in contents]
 
         return tasks
```

### Comparing `pymstodo-0.0.8/pymstodo.egg-info/PKG-INFO` & `pymstodo-0.0.9/pymstodo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymstodo
-Version: 0.0.8
+Version: 0.0.9
 Summary: Microsoft To Do API client
 Home-page: https://github.com/inbalboa/pymstodo
 Author: Sergey Shlyapugin
 Author-email: shlyapugin@gmail.com
 License: GPLv3
 Description: # pymstodo ✔️
         [![PyPI](https://img.shields.io/pypi/v/pymstodo.svg)](https://pypi.org/project/pymstodo/) [![Build Status](https://travis-ci.org/inbalboa/pymstodo.svg?branch=master)](https://travis-ci.org/inbalboa/pymstodo) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
```

### Comparing `pymstodo-0.0.8/setup.py` & `pymstodo-0.0.9/setup.py`

 * *Files identical despite different names*

