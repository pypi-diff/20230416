# Comparing `tmp/xata-0.9.0.tar.gz` & `tmp/xata-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xata-0.9.0.tar", max compression
+gzip compressed data, was "xata-0.9.1.tar", max compression
```

## Comparing `xata-0.9.0.tar` & `xata-0.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11357 2023-04-15 14:30:22.160620 xata-0.9.0/LICENSE
--rw-r--r--   0        0        0     1156 2023-04-15 14:30:22.160620 xata-0.9.0/README.md
--rw-r--r--   0        0        0      749 2023-04-15 14:30:22.188621 xata-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      858 2023-04-15 14:30:22.188621 xata-0.9.0/xata/__init__.py
--rw-r--r--   0        0        0    31957 2023-04-15 14:30:22.188621 xata-0.9.0/xata/client.py
--rw-r--r--   0        0        0     1715 2023-04-15 14:30:22.188621 xata-0.9.0/xata/errors.py
--rw-r--r--   0        0        0    10836 2023-04-15 14:30:22.188621 xata-0.9.0/xata/helpers.py
--rw-r--r--   0        0        0     2115 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespace.py
--rw-r--r--   0        0        0      769 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/__init__.py
--rw-r--r--   0        0        0      769 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/core/__init__.py
--rw-r--r--   0        0        0     2666 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/core/authentication.py
--rw-r--r--   0        0        0     6182 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/core/databases.py
--rw-r--r--   0        0        0     6204 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/core/invites.py
--rw-r--r--   0        0        0     2554 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/core/users.py
--rw-r--r--   0        0        0     7419 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/core/workspaces.py
--rw-r--r--   0        0        0      769 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/workspace/__init__.py
--rw-r--r--   0        0        0    12315 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/workspace/branch.py
--rw-r--r--   0        0        0    10143 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/workspace/migrations.py
--rw-r--r--   0        0        0    12491 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/workspace/records.py
--rw-r--r--   0        0        0    29615 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/workspace/search_and_filter.py
--rw-r--r--   0        0        0    12792 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/workspace/table.py
--rw-r--r--   0        0        0     1867 1970-01-01 00:00:00.000000 xata-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-16 10:15:31.921430 xata-0.9.1/LICENSE
+-rw-r--r--   0        0        0     1156 2023-04-16 10:15:31.921430 xata-0.9.1/README.md
+-rw-r--r--   0        0        0      749 2023-04-16 10:15:31.949431 xata-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      858 2023-04-16 10:15:31.949431 xata-0.9.1/xata/__init__.py
+-rw-r--r--   0        0        0    31957 2023-04-16 10:15:31.949431 xata-0.9.1/xata/client.py
+-rw-r--r--   0        0        0     1715 2023-04-16 10:15:31.949431 xata-0.9.1/xata/errors.py
+-rw-r--r--   0        0        0    11020 2023-04-16 10:15:31.949431 xata-0.9.1/xata/helpers.py
+-rw-r--r--   0        0        0     2114 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespace.py
+-rw-r--r--   0        0        0      769 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/__init__.py
+-rw-r--r--   0        0        0      769 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/core/__init__.py
+-rw-r--r--   0        0        0     2666 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/core/authentication.py
+-rw-r--r--   0        0        0     6182 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/core/databases.py
+-rw-r--r--   0        0        0     6204 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/core/invites.py
+-rw-r--r--   0        0        0     2554 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/core/users.py
+-rw-r--r--   0        0        0     7419 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/core/workspaces.py
+-rw-r--r--   0        0        0      769 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/workspace/__init__.py
+-rw-r--r--   0        0        0    12315 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/workspace/branch.py
+-rw-r--r--   0        0        0    10143 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/workspace/migrations.py
+-rw-r--r--   0        0        0    12491 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/workspace/records.py
+-rw-r--r--   0        0        0    29615 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/workspace/search_and_filter.py
+-rw-r--r--   0        0        0    12792 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/workspace/table.py
+-rw-r--r--   0        0        0     1867 1970-01-01 00:00:00.000000 xata-0.9.1/PKG-INFO
```

### Comparing `xata-0.9.0/LICENSE` & `xata-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xata-0.9.0/README.md` & `xata-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `xata-0.9.0/pyproject.toml` & `xata-0.9.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xata"
-version = "0.9.0"
+version = "0.9.1"
 description = "Python client for Xata.io"
 authors = ["Xata <support@xata.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 documentation = "https://xata-py.readthedocs.io"
 
 [tool.poetry.dependencies]
```

### Comparing `xata-0.9.0/xata/__init__.py` & `xata-0.9.1/xata/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.0/xata/client.py` & `xata-0.9.1/xata/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 from .namespaces.workspace.migrations import Migrations
 from .namespaces.workspace.records import Records
 from .namespaces.workspace.search_and_filter import Search_and_filter
 from .namespaces.workspace.table import Table
 
 # TODO this is a manual task, to keep in sync with pyproject.toml
 # could/should be automated to keep in sync
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 PERSONAL_API_KEY_LOCATION = "~/.config/xata/key"
 DEFAULT_DATA_PLANE_DOMAIN = "xata.sh"
 DEFAULT_CONTROL_PLANE_DOMAIN = "api.xata.io"
 DEFAULT_REGION = "us-east-1"
 DEFAULT_BRANCH_NAME = "main"
 CONFIG_LOCATION = ".xatarc"
```

### Comparing `xata-0.9.0/xata/errors.py` & `xata-0.9.1/xata/errors.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.0/xata/helpers.py` & `xata-0.9.1/xata/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,41 +100,42 @@
                 self.flush_interval,
                 self.processing_timeout,
             )
         )
         while True:
             batch = self.records.next_batch()
             if "table" in batch and len(batch["records"]) > 0:
-                r = self.client.records().bulkInsertTableRecords(batch["table"], {"records": batch["records"]})
-                if r.status_code != 200:
-                    self.logger.error(
-                        "thread #%d: unable to process batch for table '%s', with error: %d - %s"
-                        % (id, batch["table"], r.status_code, r.json())
-                    )
-                    # Add to failed queue
-                    self.failed_batches_queue.append(
-                        {
-                            "timestamp": datetime.utcnow(),
-                            "records": batch["records"],
-                            "table": batch["table"],
-                            "response": r,
-                        }
-                    )
-                    self.stats["failed_batches"] += 1
-                    if self.throw_exception:
-                        raise Exception(r.json())
+                try:
+                    r = self.client.records().bulkInsertTableRecords(batch["table"], {"records": batch["records"]})
+                    if r.status_code != 200:
+                        self.logger.error(
+                            "thread #%d: unable to process batch for table '%s', with error: %d - %s"
+                            % (id, batch["table"], r.status_code, r.json())
+                        )
+                        # Add to failed queue
+                        self.failed_batches_queue.append(
+                            {
+                                "timestamp": datetime.utcnow(),
+                                "records": batch["records"],
+                                "table": batch["table"],
+                                "response": r,
+                            }
+                        )
+                        self.stats["failed_batches"] += 1
+                        if self.throw_exception:
+                            raise Exception(r.json())
 
-                self.logger.debug(
-                    "thread #%d: pushed a batch of %d records to table %s" % (id, len(batch["records"]), batch["table"])
-                )
-                self.stats["total"] += len(batch["records"])
-                self.stats["queue"] = self.records.size()
-                if batch["table"] not in self.stats["tables"]:
-                    self.stats["tables"][batch["table"]] = 0
-                self.stats["tables"][batch["table"]] += len(batch["records"])
+                    self.logger.debug("thread #%d: pushed a batch of %d records to table %s" % (id, len(batch["records"]), batch["table"]))
+                    self.stats["total"] += len(batch["records"])
+                    self.stats["queue"] = self.records.size()
+                    if batch["table"] not in self.stats["tables"]:
+                        self.stats["tables"][batch["table"]] = 0
+                    self.stats["tables"][batch["table"]] += len(batch["records"])
+                except Exception as exc:
+                    logging.error("thread #%d: %s" % (id, exc))
             time.sleep(self.processing_timeout)
 
     def put_record(self, table_name: str, record: dict):
         """
         Put a record to the processing queue
 
         :param table_name: str
```

### Comparing `xata-0.9.0/xata/namespace.py` & `xata-0.9.1/xata/namespace.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 
     def request(self, http_method: str, url_path: str, headers: dict = {}, payload: dict = None) -> Response:
         headers = {
             **headers,
             **self.client.get_headers(),
         }  # TODO use "|" when client py min version >= 3.9
         url = "%s/%s" % (self.get_base_url(), url_path.lstrip("/"))
-
         if payload is None:
             resp = request(http_method, url, headers=headers)
         else:
             resp = request(http_method, url, headers=headers, json=payload)
 
         if resp.status_code == 429:
             raise RateLimitException(f"Rate limited: {resp.json()}")
```

### Comparing `xata-0.9.0/xata/namespaces/__init__.py` & `xata-0.9.1/xata/namespaces/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.0/xata/namespaces/core/__init__.py` & `xata-0.9.1/xata/namespaces/core/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.0/xata/namespaces/core/authentication.py` & `xata-0.9.1/xata/namespaces/core/authentication.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.0/xata/namespaces/core/databases.py` & `xata-0.9.1/xata/namespaces/core/databases.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.0/xata/namespaces/core/invites.py` & `xata-0.9.1/xata/namespaces/core/invites.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.0/xata/namespaces/core/users.py` & `xata-0.9.1/xata/namespaces/core/users.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.0/xata/namespaces/core/workspaces.py` & `xata-0.9.1/xata/namespaces/core/workspaces.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.0/xata/namespaces/workspace/__init__.py` & `xata-0.9.1/xata/namespaces/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.0/xata/namespaces/workspace/branch.py` & `xata-0.9.1/xata/namespaces/workspace/branch.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.0/xata/namespaces/workspace/migrations.py` & `xata-0.9.1/xata/namespaces/workspace/migrations.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.0/xata/namespaces/workspace/records.py` & `xata-0.9.1/xata/namespaces/workspace/records.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.0/xata/namespaces/workspace/search_and_filter.py` & `xata-0.9.1/xata/namespaces/workspace/search_and_filter.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.0/xata/namespaces/workspace/table.py` & `xata-0.9.1/xata/namespaces/workspace/table.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.0/PKG-INFO` & `xata-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xata
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python client for Xata.io
 License: Apache-2.0
 Author: Xata
 Author-email: support@xata.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

