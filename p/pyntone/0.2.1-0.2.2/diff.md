# Comparing `tmp/pyntone-0.2.1.tar.gz` & `tmp/pyntone-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyntone-0.2.1.tar", last modified: Tue Apr 11 15:04:10 2023, max compression
+gzip compressed data, was "pyntone-0.2.2.tar", last modified: Sun Apr 16 13:06:07 2023, max compression
```

## Comparing `pyntone-0.2.1.tar` & `pyntone-0.2.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 15:04:10.517274 pyntone-0.2.1/
--rw-rw-rw-   0        0        0     1083 2022-10-20 13:41:34.000000 pyntone-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      435 2023-04-11 15:04:10.517274 pyntone-0.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-11 15:04:10.471290 pyntone-0.2.1/pyntone/
--rw-rw-rw-   0        0        0       91 2023-04-11 15:02:11.000000 pyntone-0.2.1/pyntone/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 15:04:10.503274 pyntone-0.2.1/pyntone/client/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:31:49.000000 pyntone-0.2.1/pyntone/client/__init__.py
--rw-rw-rw-   0        0        0     1924 2023-04-11 15:00:31.000000 pyntone-0.2.1/pyntone/client/bulk_request_client.py
--rw-rw-rw-   0        0        0    19740 2023-04-10 13:44:05.000000 pyntone-0.2.1/pyntone/client/record_client.py
-drwxrwxrwx   0        0        0        0 2023-04-11 15:04:10.506274 pyntone-0.2.1/pyntone/http/
--rw-rw-rw-   0        0        0        0 2022-02-26 06:27:39.000000 pyntone-0.2.1/pyntone/http/__init__.py
--rw-rw-rw-   0        0        0     1769 2023-04-11 15:00:54.000000 pyntone-0.2.1/pyntone/http/http_client.py
--rw-rw-rw-   0        0        0     6251 2023-04-11 15:00:14.000000 pyntone-0.2.1/pyntone/kintone_request_config_builder.py
--rw-rw-rw-   0        0        0     1262 2023-04-11 15:01:21.000000 pyntone-0.2.1/pyntone/kintone_rest_api_client.py
-drwxrwxrwx   0        0        0        0 2023-04-11 15:04:10.511275 pyntone-0.2.1/pyntone/types/
--rw-rw-rw-   0        0        0      136 2023-04-07 07:20:19.000000 pyntone-0.2.1/pyntone/types/__init__.py
--rw-rw-rw-   0        0        0      488 2023-04-11 14:59:57.000000 pyntone-0.2.1/pyntone/types/auth.py
--rw-rw-rw-   0        0        0      972 2023-04-11 15:01:15.000000 pyntone-0.2.1/pyntone/types/record.py
--rw-rw-rw-   0        0        0      340 2023-04-11 15:01:27.000000 pyntone-0.2.1/pyntone/url.py
-drwxrwxrwx   0        0        0        0 2023-04-11 15:04:10.497278 pyntone-0.2.1/pyntone.egg-info/
--rw-rw-rw-   0        0        0      435 2023-04-11 15:04:10.000000 pyntone-0.2.1/pyntone.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      554 2023-04-11 15:04:10.000000 pyntone-0.2.1/pyntone.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 15:04:10.000000 pyntone-0.2.1/pyntone.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-11 15:04:10.000000 pyntone-0.2.1/pyntone.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-11 15:04:10.000000 pyntone-0.2.1/pyntone.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2023-04-09 12:28:30.000000 pyntone-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0      536 2023-04-11 15:04:10.523274 pyntone-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-11 15:04:10.515274 pyntone-0.2.1/tests/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:21:21.000000 pyntone-0.2.1/tests/__init__.py
--rw-rw-rw-   0        0        0     6260 2023-04-10 13:36:36.000000 pyntone-0.2.1/tests/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:06:07.101910 pyntone-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-16 13:05:50.000000 pyntone-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-16 13:06:07.101910 pyntone-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-16 13:05:50.000000 pyntone-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:06:07.101910 pyntone-0.2.2/pyntone/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyntone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:06:07.101910 pyntone-0.2.2/pyntone/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyntone/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyntone/client/bulk_request_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19169 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyntone/client/record_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:06:07.101910 pyntone-0.2.2/pyntone/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyntone/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyntone/http/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyntone/kintone_request_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyntone/kintone_rest_api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:06:07.101910 pyntone-0.2.2/pyntone/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyntone/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyntone/types/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyntone/types/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyntone/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:06:07.101910 pyntone-0.2.2/pyntone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-16 13:06:07.000000 pyntone-0.2.2/pyntone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-16 13:06:07.000000 pyntone-0.2.2/pyntone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 13:06:07.000000 pyntone-0.2.2/pyntone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-16 13:06:07.000000 pyntone-0.2.2/pyntone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-16 13:06:07.000000 pyntone-0.2.2/pyntone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-16 13:06:07.101910 pyntone-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:06:07.101910 pyntone-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:05:50.000000 pyntone-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-04-16 13:05:50.000000 pyntone-0.2.2/tests/test_record.py
```

### Comparing `pyntone-0.2.1/LICENSE` & `pyntone-0.2.2/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 kashi03
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2022 kashi03
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `pyntone-0.2.1/pyntone/client/bulk_request_client.py` & `pyntone-0.2.2/pyntone/client/bulk_request_client.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-from typing import Literal, TypedDict, Union
-
-from pyntone.http.http_client import HttpClent, KintoneRequestParams
-from pyntone.url import build_path
-
-EndpointName = Literal[
-    'record',
-    'records',
-    'record/status',
-    'records/status',
-    'record/assignees',
-]
-
-HttpMethod = Literal[
-    'POST',
-    'PUT',
-    'DELETE'
-]
-
-class ApiRequestParameter(TypedDict):
-    method: HttpMethod
-    api: str
-    payload: dict
-
-class EndopintRequestParameter(TypedDict):
-    method: HttpMethod
-    endpoint_name: EndpointName
-    payload: dict
-
-class BulkRequestClient:
-    def __init__(
-        self,
-        client: HttpClent,
-        guest_space_id: Union[int, str, None] = None,
-    ) -> None:
-        self.client = client
-        self.guest_space_id = guest_space_id
-        self.REQUESTS_LENGTH_LIMIT = 20
-    
-    def send(
-        self,
-        requests: Union[list[ApiRequestParameter], list[EndopintRequestParameter], list[Union[ApiRequestParameter, EndopintRequestParameter]]]
-    ):
-        request_list = []
-        for request in requests:
-            endpoint_name = request.get('endpoint_name')
-            if endpoint_name is not None:
-                request_list.append({
-                    'method': request['method'],
-                    'api': self.__build_path_with_guest_space_id(endpoint_name),
-                    'payload': request['payload']
-                })
-            else:
-                request_list.append(request)
-        
-        path = self.__build_path_with_guest_space_id('bulkRequest')
-        params = KintoneRequestParams(
-            requests=request_list
-        )
-        return self.client.post(path, params)
-
-    def __build_path_with_guest_space_id(self, endpoint_name: str) -> str:
-        return build_path(
-            endpoint_name=endpoint_name,
-            guest_space_id=self.guest_space_id
+from typing import Literal, TypedDict, Union
+
+from pyntone.http.http_client import HttpClent, KintoneRequestParams
+from pyntone.url import build_path
+
+EndpointName = Literal[
+    'record',
+    'records',
+    'record/status',
+    'records/status',
+    'record/assignees',
+]
+
+HttpMethod = Literal[
+    'POST',
+    'PUT',
+    'DELETE'
+]
+
+class ApiRequestParameter(TypedDict):
+    method: HttpMethod
+    api: str
+    payload: dict
+
+class EndopintRequestParameter(TypedDict):
+    method: HttpMethod
+    endpoint_name: EndpointName
+    payload: dict
+
+class BulkRequestClient:
+    def __init__(
+        self,
+        client: HttpClent,
+        guest_space_id: Union[int, str, None] = None,
+    ) -> None:
+        self.client = client
+        self.guest_space_id = guest_space_id
+        self.REQUESTS_LENGTH_LIMIT = 20
+    
+    def send(
+        self,
+        requests: Union[list[ApiRequestParameter], list[EndopintRequestParameter], list[Union[ApiRequestParameter, EndopintRequestParameter]]]
+    ):
+        request_list = []
+        for request in requests:
+            endpoint_name = request.get('endpoint_name')
+            if endpoint_name is not None:
+                request_list.append({
+                    'method': request['method'],
+                    'api': self.__build_path_with_guest_space_id(endpoint_name),
+                    'payload': request['payload']
+                })
+            else:
+                request_list.append(request)
+        
+        path = self.__build_path_with_guest_space_id('bulkRequest')
+        params = KintoneRequestParams(
+            requests=request_list
+        )
+        return self.client.post(path, params)
+
+    def __build_path_with_guest_space_id(self, endpoint_name: str) -> str:
+        return build_path(
+            endpoint_name=endpoint_name,
+            guest_space_id=self.guest_space_id
         )
```

### Comparing `pyntone-0.2.1/pyntone/client/record_client.py` & `pyntone-0.2.2/pyntone/client/record_client.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,572 +1,572 @@
-from typing import Literal, Optional, Union
-
-from pyntone.client.bulk_request_client import (BulkRequestClient,
-                                                EndopintRequestParameter)
-from pyntone.http.http_client import HttpClent, KintoneRequestParams
-from pyntone.types import AppID, CommentID, RecordID, Revision
-from pyntone.types.record import (Comment, DeleteRecordParameter,
-                                  RecordForParameter, UpdateKey,
-                                  UpdateKeyRecordForParameter,
-                                  UpdateRecordForParameter,
-                                  UpdateRecordStatusParameter)
-from pyntone.url import build_path
-
-ADD_RECORDS_LIMIT = 100
-UPDATE_RECORDS_LIMIT = 100
-DELETE_RECORDS_LIMIT = 100
-GET_RECORDS_LIMIT = 500
-
-class RecordClient:
-    def __init__(
-        self,
-        client: HttpClent,
-        bulk_request_client: BulkRequestClient,
-        guest_space_id: Union[int, str, None]
-    ) -> None:
-        self.client = client
-        self.bulk_request_client = bulk_request_client
-        self.guest_space_id = guest_space_id
-        self.did_warn_maximum_offset_value = False
-    
-    def get_record(self, app: AppID, record_id: RecordID):
-        path = self.__build_path_with_guest_space_id(endpoint_name='record')
-        params = KintoneRequestParams(
-            app=app,
-            id=record_id
-        )
-        return self.client.get(path, params)
-
-    def add_record(self, app: AppID, record: Optional[RecordForParameter] = None):
-        path = self.__build_path_with_guest_space_id(endpoint_name='record')
-        params = KintoneRequestParams(
-            app=app,
-            record=record
-        )
-        return self.client.post(path, params)
-
-    def update_record(
-        self,
-        app: AppID,
-        record_id: Optional[RecordID] = None,
-        update_key: Optional[UpdateKey] = None,
-        record: Optional[RecordForParameter] = None,
-        revision: Optional[Revision] = None
-    ):
-        if record_id is None and update_key is None:
-            raise ValueError()
-        path = self.__build_path_with_guest_space_id(endpoint_name='record')
-        params = KintoneRequestParams(
-            app=app,
-            id=record_id,
-            update_key=update_key,
-            record=record,
-            revision=revision
-        )
-        return self.client.put(path, params)
-
-    def upsert_record(
-        self,
-        app: AppID,
-        update_key: UpdateKey,
-        record: Optional[RecordForParameter] = None,
-        revision: Optional[Revision] = None
-    ):
-        query = '{} = "{}"'.format(update_key['field'], update_key['value'])
-        records = self.get_records(app, query=query)['records']
-        if len(records) > 0:
-            if records[0]['$id']['type'] == '__ID__':
-                result = self.update_record(app, update_key=update_key, record=record, revision=revision)
-                return {
-                    'id': records[0]['$id']['value'],
-                    'revision': result['revision']
-                }
-            raise Exception('Missing `$id` in `getRecords` response.')
-        return self.add_record(
-            app,
-            {
-            f"{update_key['field']}": { 'value': update_key['value'] },
-            **({} if record is None else record)
-        }
-        )
-
-    def get_records(
-        self,
-        app: AppID,
-        fields: Optional[list[str]] = None,
-        query: Optional[str] = None,
-        total_count: Optional[bool] = None
-    ):
-        path = self.__build_path_with_guest_space_id(endpoint_name='records')
-        params = KintoneRequestParams(
-            app=app,
-            fields=fields,
-            query=query,
-            total_count=total_count
-        )
-        return self.client.get(path, params)
-
-    def add_records(self, app: AppID, records: list[RecordForParameter]):
-        path = self.__build_path_with_guest_space_id(endpoint_name='records')
-        params = KintoneRequestParams(
-            app=app,
-            records=records
-        )
-        return self.client.post(path, params)
-    
-    def update_records(
-        self,
-        app: AppID,
-        records: Union[list[UpdateRecordForParameter], list[UpdateKeyRecordForParameter], list[Union[UpdateRecordForParameter, UpdateKeyRecordForParameter]]]
-    ):
-        path = self.__build_path_with_guest_space_id(endpoint_name='records')
-        params = KintoneRequestParams(
-            app=app,
-            records=records
-        )
-        return self.client.put(path, params)
-    
-    def delete_records(self, app: AppID, ids: list[RecordID], revisions: Optional[list[Revision]]):
-        path = self.__build_path_with_guest_space_id(endpoint_name='records')
-        params = KintoneRequestParams(
-            app=app,
-            ids=ids,
-            revisions=revisions
-        )
-        return self.client.delete(path, params)
-    
-    def create_cursor(self,
-        app: AppID,
-        fields: Optional[list[str]] = None,
-        query: Optional[str] = None,
-        size: Union[int, str, None] = None
-    ):
-        path = self.__build_path_with_guest_space_id(endpoint_name='records/cursor')
-        params = KintoneRequestParams(
-            app=app,
-            fields=fields,
-            query=query,
-            size=size
-        )
-        return self.client.post(path, params)
-    
-    def get_records_by_cursor(self, cursor_id: str):
-        path = self.__build_path_with_guest_space_id(endpoint_name='records/cursor')
-        params = KintoneRequestParams(
-            id=cursor_id
-        )
-        return self.client.get(path, params)
-    
-    def delete_cursor(self, cursor_id: str):
-        path = self.__build_path_with_guest_space_id(endpoint_name='records/cursor')
-        params = KintoneRequestParams(
-            id=cursor_id
-        )
-        return self.client.delete(path, params)
-    
-    def get_all_records(
-        self,
-        app: AppID,
-        fields: Optional[list[str]] = None,
-        condition: Optional[str] = None,
-        order_by: Optional[str] = None,
-        with_cursor: bool = True
-    ):
-        if with_cursor:
-            condition_query = f'{condition} ' if condition is not None else ''
-            order_by_query = f'order by {order_by}' if order_by is not None else ''
-            query = f'{condition_query}{order_by_query}'
-            query = None if query == '' else query
-            return self.get_all_records_with_cursor(app, fields, query)
-        if order_by is None:
-            return self.get_all_records_with_id(app, fields, condition)
-        return self.get_all_records_with_offset(app, fields, condition, order_by)
-    
-    def get_all_records_with_id(
-        self,
-        app: AppID,
-        fields: Optional[list[str]] = None,
-        condition: Optional[str] = None
-    ):
-        if fields is not None and len(fields) > 0 and not '$id' in fields:
-            fields.append('$id')
-        return self.__get_all_records_recursive_with_id(app, fields, condition, '0', [])
-
-    def __get_all_records_recursive_with_id(
-        self,
-        app: AppID,
-        fields: Optional[list[str]],
-        condition: Optional[str],
-        id: str,
-        records: list
-    ):
-        condition_query = f'({condition}) and ' if condition is not None else ''
-        query = f'{condition_query}$id > {id} order by $id asc limit {GET_RECORDS_LIMIT}'
-        result = self.get_records(app, fields, query)
-        all_records = records + result['records']
-        if len(result['records']) < GET_RECORDS_LIMIT:
-            return all_records
-        last_record = result['records'][-1]
-        if last_record['$id']['type'] == '__ID__':
-            last_id = last_record['$id']['value']
-            return self.__get_all_records_recursive_with_id(app, fields, condition, last_id, all_records)
-        raise Exception('Missing `$id` in `getRecords` response.')
-    
-    def get_all_records_with_offset(
-        self,
-        app: AppID,
-        fields: Optional[list[str]] = None,
-        condition: Optional[str] = None,
-        order_by: Optional[str] = None,
-    ):
-        return self.__get_all_records_recursive_with_offset(app, fields, condition, order_by, 0, [])
-
-    def __get_all_records_recursive_with_offset(
-        self,
-        app: AppID,
-        fields: Optional[list[str]],
-        condition: Optional[str],
-        order_by: Optional[str],
-        offset: int,
-        records: list
-    ):
-        condition_query = f'{condition} ' if condition is not None else ''
-        order_by_query = f'order by {order_by} ' if order_by is not None else ''
-        query = f'{condition_query}{order_by_query}limit {GET_RECORDS_LIMIT} offset {offset}'
-        result = self.get_records(app, fields, query)
-        all_records = records + result['records']
-        if len(result['records']) < GET_RECORDS_LIMIT:
-            return all_records
-        return self.__get_all_records_recursive_with_offset(
-            app,
-            fields,
-            condition,
-            order_by,
-            offset + GET_RECORDS_LIMIT,
-            all_records
-        )
-
-    def get_all_records_with_cursor(
-        self,
-        app: AppID,
-        fields: Optional[list[str]] = None,
-        query: Optional[str] = None
-    ) -> list:
-        res = self.create_cursor(app, fields, query, size=500)
-        cursor_id = res['id']
-        try:
-            return self.__get_all_records_recursive_by_cursor(cursor_id, [])
-        except Exception as e:
-            self.delete_cursor(cursor_id)
-            raise e
-    
-    def __get_all_records_recursive_by_cursor(
-        self,
-        cursor_id: str,
-        records: list
-    ) -> list:
-        result = self.get_records_by_cursor(cursor_id)
-        all_records = records + result['records']
-        if result['next']:
-            return self.__get_all_records_recursive_by_cursor(cursor_id, all_records)
-        return all_records
-
-    def add_all_records(
-        self,
-        app: AppID,
-        records: list[RecordForParameter]
-    ):
-        if not all(not isinstance(record, list) and isinstance(record, dict) for record in records):
-            raise ValueError('the `records` parameter must be an array of object.')
-        return self.__add_all_records_recursive(app, records, len(records), [])
-    
-    def __add_all_records_recursive(
-        self,
-        app: AppID,
-        records: list[RecordForParameter],
-        num_of_all_records: int,
-        results: list
-    ) -> dict:
-        CHUNK_LENGTH = self.bulk_request_client.REQUESTS_LENGTH_LIMIT * ADD_RECORDS_LIMIT
-        records_chunk = records[:CHUNK_LENGTH]
-        if len(records_chunk) == 0:
-            return {
-                'records': results
-            }
-        new_results = []
-        try:
-            new_results = self.__add_all_records_with_bulk_request(
-                app,
-                records_chunk
-            )
-        except Exception as e:
-            # TODO
-            raise e
-        return self.__add_all_records_recursive(
-            app,
-            records[CHUNK_LENGTH:],
-            num_of_all_records,
-            results + new_results
-        )
-    
-    def __add_all_records_with_bulk_request(
-        self,
-        app: AppID,
-        records: list[RecordForParameter]
-    ):
-        separated_records = self.__separate_array_recursive(
-            ADD_RECORDS_LIMIT,
-            [],
-            records
-        )
-        requests: list[EndopintRequestParameter] = [
-            {
-                'method': 'POST',
-                'endpoint_name': 'records',
-                'payload': {
-                    'app': app,
-                    'records': records_
-                }
-            } for records_ in separated_records
-        ]
-        results = self.bulk_request_client.send(requests)['results']
-        return_value = []
-        for result in results:
-            ids = result['ids']
-            revisions = result['revisions']
-            return_value += [
-                {
-                    'id': val,
-                    'revision': revisions[num]
-                } for num, val in enumerate(ids)
-            ]
-        return return_value
-
-    def update_all_records(
-        self,
-        app: AppID,
-        records: Union[list[UpdateRecordForParameter], list[UpdateKeyRecordForParameter], list[Union[UpdateRecordForParameter, UpdateKeyRecordForParameter]]]
-    ):
-        return self.__update_all_records_recursive(app, records, len(records), [])
-    
-    def __update_all_records_recursive(
-        self,
-        app: AppID,
-        records: Union[list[UpdateRecordForParameter], list[UpdateKeyRecordForParameter], list[Union[UpdateRecordForParameter, UpdateKeyRecordForParameter]]],
-        num_of_all_records: int,
-        results: list
-    ):
-        CHUNK_LENGTH = self.bulk_request_client.REQUESTS_LENGTH_LIMIT * UPDATE_RECORDS_LIMIT
-        records_chunk = records[:CHUNK_LENGTH]
-        if len(records_chunk) == 0:
-            return {
-                'records': results
-            }
-        new_results = []
-        try:
-            new_results = self.__update_all_records_with_bulk_request(
-                app,
-                records_chunk
-            )
-        except Exception as e:
-            # TODO
-            raise e
-        return self.__update_all_records_recursive(
-            app,
-            records[CHUNK_LENGTH:],
-            num_of_all_records,
-            results + new_results
-        )
-    
-    def __update_all_records_with_bulk_request(
-        self,
-        app: AppID,
-        records: Union[list[UpdateRecordForParameter], list[UpdateKeyRecordForParameter], list[Union[UpdateRecordForParameter, UpdateKeyRecordForParameter]]],
-    ):
-        separated_records = self.__separate_array_recursive(
-            UPDATE_RECORDS_LIMIT,
-            [],
-            records
-        )
-        requests: list[EndopintRequestParameter] = [
-            {
-                'method': 'PUT',
-                'endpoint_name': 'records',
-                'payload': {
-                    'app': app,
-                    'records': records_,
-                }
-            } for records_ in separated_records
-        ]
-        results = self.bulk_request_client.send(requests)['results']
-        return_value = []
-        for result in results:
-            return_value += result['records']
-        return return_value
-    
-    def delete_all_reocrds(
-        self,
-        app: AppID,
-        records: list[DeleteRecordParameter]
-    ):
-        return self.__delete_all_records_recursive(app, records, len(records))
-    
-    def __delete_all_records_recursive(
-        self,
-        app: AppID,
-        records: list[DeleteRecordParameter],
-        num_of_all_records: int
-    ):
-        CHUNK_LENGTH = self.bulk_request_client.REQUESTS_LENGTH_LIMIT * DELETE_RECORDS_LIMIT
-        records_chunk = records[:CHUNK_LENGTH]
-        if len(records_chunk) == 0:
-            return {}
-        try:
-            self.__delete_all_records_with_bulk_request(
-                app,
-                records_chunk
-            )
-        except Exception as e:
-            # TODO
-            raise e
-        return self.__delete_all_records_recursive(
-            app,
-            records[CHUNK_LENGTH:],
-            num_of_all_records
-        )
-    
-    def __delete_all_records_with_bulk_request(
-        self,
-        app: AppID,
-        records: list[DeleteRecordParameter]
-    ):
-        separated_records = self.__separate_array_recursive(
-            DELETE_RECORDS_LIMIT,
-            [],
-            records
-        )
-        requests: list[EndopintRequestParameter] = [
-            {
-                'method': 'DELETE',
-                'endpoint_name': 'records',
-                'payload': {
-                    'app': app,
-                    'ids': [ record['id'] for record in records_ ],
-                    'revisions': [ record.get('revision', -1) for record in records_ ]
-                }
-            } for records_ in separated_records
-        ]
-        self.bulk_request_client.send(requests)['results']
-        return None
-    
-    def __separate_array_recursive(
-        self,
-        size: int,
-        separated: list[list],
-        array: list
-    ) -> list[list]:
-        chunk = array[:size]
-        if len(chunk) == 0:
-            return separated
-        return self.__separate_array_recursive(
-            size,
-            [*separated, chunk],
-            array[size:]
-        )
-    
-    def add_record_comment(
-        self,
-        app: AppID,
-        record: RecordID,
-        comment: Comment
-    ):
-        path = self.__build_path_with_guest_space_id('record/comment')
-        params = KintoneRequestParams(
-            app=app,
-            record=record,
-            comment=comment
-        )
-        return self.client.post(path, params)
-    
-    def delete_record_comment(
-        self,
-        app: AppID,
-        record: RecordID,
-        comment: CommentID
-    ):
-        path = self.__build_path_with_guest_space_id('record/comment')
-        params = KintoneRequestParams(
-            app=app,
-            record=record,
-            comment=comment
-        )
-        return self.client.delete(path, params)
-    
-    def get_record_comments(
-        self,
-        app: AppID,
-        record: RecordID,
-        order: Optional[Literal['asc', 'desc']] = None,
-        offset: Optional[int] = None,
-        limit: Optional[int] = None
-    ):
-        path = self.__build_path_with_guest_space_id('record/comments')
-        params = KintoneRequestParams(
-            app=app,
-            record=record,
-            order=order,
-            offset=offset,
-            limit=limit
-        )
-        return self.client.get(path, params)
-    
-    def update_record_assigness(
-        self,
-        app: AppID,
-        id: RecordID,
-        assignees: list[str],
-        revision: Optional[Revision] = None
-    ):
-        path = self.__build_path_with_guest_space_id('record/assignees')
-        params = KintoneRequestParams(
-            app=app,
-            id=id,
-            assignees=assignees,
-            revision=revision
-        )
-        return self.client.put(path, params)
-    
-    def update_record_status(
-        self,
-        app: AppID,
-        id: RecordID,
-        action: str,
-        assignees: Optional[list[str]] = None,
-        revision: Optional[Revision] = None
-    ):
-        path = self.__build_path_with_guest_space_id('record/status')
-        params = KintoneRequestParams(
-            app=app,
-            id=id,
-            action=action,
-            assignees=assignees,
-            revision=revision
-        )
-        return self.client.put(path, params)
-    
-    def update_records_status(
-        self,
-        app: AppID,
-        records: list[UpdateRecordStatusParameter]
-    ):
-        path = self.__build_path_with_guest_space_id('records/status')
-        params = KintoneRequestParams(
-            app=app,
-            records=records
-        )
-        return self.client.put(path, params)
-    
-    def __build_path_with_guest_space_id(self, endpoint_name: str) -> str:
-        return build_path(
-            endpoint_name=endpoint_name,
-            guest_space_id=self.guest_space_id
+from typing import Literal, Optional, Union
+
+from pyntone.client.bulk_request_client import (BulkRequestClient,
+                                                EndopintRequestParameter)
+from pyntone.http.http_client import HttpClent, KintoneRequestParams
+from pyntone.types import AppID, CommentID, RecordID, Revision
+from pyntone.types.record import (Comment, DeleteRecordParameter,
+                                  RecordForParameter, UpdateKey,
+                                  UpdateKeyRecordForParameter,
+                                  UpdateRecordForParameter,
+                                  UpdateRecordStatusParameter)
+from pyntone.url import build_path
+
+ADD_RECORDS_LIMIT = 100
+UPDATE_RECORDS_LIMIT = 100
+DELETE_RECORDS_LIMIT = 100
+GET_RECORDS_LIMIT = 500
+
+class RecordClient:
+    def __init__(
+        self,
+        client: HttpClent,
+        bulk_request_client: BulkRequestClient,
+        guest_space_id: Union[int, str, None]
+    ) -> None:
+        self.client = client
+        self.bulk_request_client = bulk_request_client
+        self.guest_space_id = guest_space_id
+        self.did_warn_maximum_offset_value = False
+    
+    def get_record(self, app: AppID, record_id: RecordID):
+        path = self.__build_path_with_guest_space_id(endpoint_name='record')
+        params = KintoneRequestParams(
+            app=app,
+            id=record_id
+        )
+        return self.client.get(path, params)
+
+    def add_record(self, app: AppID, record: Optional[RecordForParameter] = None):
+        path = self.__build_path_with_guest_space_id(endpoint_name='record')
+        params = KintoneRequestParams(
+            app=app,
+            record=record
+        )
+        return self.client.post(path, params)
+
+    def update_record(
+        self,
+        app: AppID,
+        record_id: Optional[RecordID] = None,
+        update_key: Optional[UpdateKey] = None,
+        record: Optional[RecordForParameter] = None,
+        revision: Optional[Revision] = None
+    ):
+        if record_id is None and update_key is None:
+            raise ValueError()
+        path = self.__build_path_with_guest_space_id(endpoint_name='record')
+        params = KintoneRequestParams(
+            app=app,
+            id=record_id,
+            update_key=update_key,
+            record=record,
+            revision=revision
+        )
+        return self.client.put(path, params)
+
+    def upsert_record(
+        self,
+        app: AppID,
+        update_key: UpdateKey,
+        record: Optional[RecordForParameter] = None,
+        revision: Optional[Revision] = None
+    ):
+        query = '{} = "{}"'.format(update_key['field'], update_key['value'])
+        records = self.get_records(app, query=query)['records']
+        if len(records) > 0:
+            if records[0]['$id']['type'] == '__ID__':
+                result = self.update_record(app, update_key=update_key, record=record, revision=revision)
+                return {
+                    'id': records[0]['$id']['value'],
+                    'revision': result['revision']
+                }
+            raise Exception('Missing `$id` in `getRecords` response.')
+        return self.add_record(
+            app,
+            {
+            f"{update_key['field']}": { 'value': update_key['value'] },
+            **({} if record is None else record)
+        }
+        )
+
+    def get_records(
+        self,
+        app: AppID,
+        fields: Optional[list[str]] = None,
+        query: Optional[str] = None,
+        total_count: Optional[bool] = None
+    ):
+        path = self.__build_path_with_guest_space_id(endpoint_name='records')
+        params = KintoneRequestParams(
+            app=app,
+            fields=fields,
+            query=query,
+            total_count=total_count
+        )
+        return self.client.get(path, params)
+
+    def add_records(self, app: AppID, records: list[RecordForParameter]):
+        path = self.__build_path_with_guest_space_id(endpoint_name='records')
+        params = KintoneRequestParams(
+            app=app,
+            records=records
+        )
+        return self.client.post(path, params)
+    
+    def update_records(
+        self,
+        app: AppID,
+        records: Union[list[UpdateRecordForParameter], list[UpdateKeyRecordForParameter], list[Union[UpdateRecordForParameter, UpdateKeyRecordForParameter]]]
+    ):
+        path = self.__build_path_with_guest_space_id(endpoint_name='records')
+        params = KintoneRequestParams(
+            app=app,
+            records=records
+        )
+        return self.client.put(path, params)
+    
+    def delete_records(self, app: AppID, ids: list[RecordID], revisions: Optional[list[Revision]]):
+        path = self.__build_path_with_guest_space_id(endpoint_name='records')
+        params = KintoneRequestParams(
+            app=app,
+            ids=ids,
+            revisions=revisions
+        )
+        return self.client.delete(path, params)
+    
+    def create_cursor(self,
+        app: AppID,
+        fields: Optional[list[str]] = None,
+        query: Optional[str] = None,
+        size: Union[int, str, None] = None
+    ):
+        path = self.__build_path_with_guest_space_id(endpoint_name='records/cursor')
+        params = KintoneRequestParams(
+            app=app,
+            fields=fields,
+            query=query,
+            size=size
+        )
+        return self.client.post(path, params)
+    
+    def get_records_by_cursor(self, cursor_id: str):
+        path = self.__build_path_with_guest_space_id(endpoint_name='records/cursor')
+        params = KintoneRequestParams(
+            id=cursor_id
+        )
+        return self.client.get(path, params)
+    
+    def delete_cursor(self, cursor_id: str):
+        path = self.__build_path_with_guest_space_id(endpoint_name='records/cursor')
+        params = KintoneRequestParams(
+            id=cursor_id
+        )
+        return self.client.delete(path, params)
+    
+    def get_all_records(
+        self,
+        app: AppID,
+        fields: Optional[list[str]] = None,
+        condition: Optional[str] = None,
+        order_by: Optional[str] = None,
+        with_cursor: bool = True
+    ):
+        if with_cursor:
+            condition_query = f'{condition} ' if condition is not None else ''
+            order_by_query = f'order by {order_by}' if order_by is not None else ''
+            query = f'{condition_query}{order_by_query}'
+            query = None if query == '' else query
+            return self.get_all_records_with_cursor(app, fields, query)
+        if order_by is None:
+            return self.get_all_records_with_id(app, fields, condition)
+        return self.get_all_records_with_offset(app, fields, condition, order_by)
+    
+    def get_all_records_with_id(
+        self,
+        app: AppID,
+        fields: Optional[list[str]] = None,
+        condition: Optional[str] = None
+    ):
+        if fields is not None and len(fields) > 0 and not '$id' in fields:
+            fields.append('$id')
+        return self.__get_all_records_recursive_with_id(app, fields, condition, '0', [])
+
+    def __get_all_records_recursive_with_id(
+        self,
+        app: AppID,
+        fields: Optional[list[str]],
+        condition: Optional[str],
+        id: str,
+        records: list
+    ):
+        condition_query = f'({condition}) and ' if condition is not None else ''
+        query = f'{condition_query}$id > {id} order by $id asc limit {GET_RECORDS_LIMIT}'
+        result = self.get_records(app, fields, query)
+        all_records = records + result['records']
+        if len(result['records']) < GET_RECORDS_LIMIT:
+            return all_records
+        last_record = result['records'][-1]
+        if last_record['$id']['type'] == '__ID__':
+            last_id = last_record['$id']['value']
+            return self.__get_all_records_recursive_with_id(app, fields, condition, last_id, all_records)
+        raise Exception('Missing `$id` in `getRecords` response.')
+    
+    def get_all_records_with_offset(
+        self,
+        app: AppID,
+        fields: Optional[list[str]] = None,
+        condition: Optional[str] = None,
+        order_by: Optional[str] = None,
+    ):
+        return self.__get_all_records_recursive_with_offset(app, fields, condition, order_by, 0, [])
+
+    def __get_all_records_recursive_with_offset(
+        self,
+        app: AppID,
+        fields: Optional[list[str]],
+        condition: Optional[str],
+        order_by: Optional[str],
+        offset: int,
+        records: list
+    ):
+        condition_query = f'{condition} ' if condition is not None else ''
+        order_by_query = f'order by {order_by} ' if order_by is not None else ''
+        query = f'{condition_query}{order_by_query}limit {GET_RECORDS_LIMIT} offset {offset}'
+        result = self.get_records(app, fields, query)
+        all_records = records + result['records']
+        if len(result['records']) < GET_RECORDS_LIMIT:
+            return all_records
+        return self.__get_all_records_recursive_with_offset(
+            app,
+            fields,
+            condition,
+            order_by,
+            offset + GET_RECORDS_LIMIT,
+            all_records
+        )
+
+    def get_all_records_with_cursor(
+        self,
+        app: AppID,
+        fields: Optional[list[str]] = None,
+        query: Optional[str] = None
+    ) -> list:
+        res = self.create_cursor(app, fields, query, size=500)
+        cursor_id = res['id']
+        try:
+            return self.__get_all_records_recursive_by_cursor(cursor_id, [])
+        except Exception as e:
+            self.delete_cursor(cursor_id)
+            raise e
+    
+    def __get_all_records_recursive_by_cursor(
+        self,
+        cursor_id: str,
+        records: list
+    ) -> list:
+        result = self.get_records_by_cursor(cursor_id)
+        all_records = records + result['records']
+        if result['next']:
+            return self.__get_all_records_recursive_by_cursor(cursor_id, all_records)
+        return all_records
+
+    def add_all_records(
+        self,
+        app: AppID,
+        records: list[RecordForParameter]
+    ):
+        if not all(not isinstance(record, list) and isinstance(record, dict) for record in records):
+            raise ValueError('the `records` parameter must be an array of object.')
+        return self.__add_all_records_recursive(app, records, len(records), [])
+    
+    def __add_all_records_recursive(
+        self,
+        app: AppID,
+        records: list[RecordForParameter],
+        num_of_all_records: int,
+        results: list
+    ) -> dict:
+        CHUNK_LENGTH = self.bulk_request_client.REQUESTS_LENGTH_LIMIT * ADD_RECORDS_LIMIT
+        records_chunk = records[:CHUNK_LENGTH]
+        if len(records_chunk) == 0:
+            return {
+                'records': results
+            }
+        new_results = []
+        try:
+            new_results = self.__add_all_records_with_bulk_request(
+                app,
+                records_chunk
+            )
+        except Exception as e:
+            # TODO
+            raise e
+        return self.__add_all_records_recursive(
+            app,
+            records[CHUNK_LENGTH:],
+            num_of_all_records,
+            results + new_results
+        )
+    
+    def __add_all_records_with_bulk_request(
+        self,
+        app: AppID,
+        records: list[RecordForParameter]
+    ):
+        separated_records = self.__separate_array_recursive(
+            ADD_RECORDS_LIMIT,
+            [],
+            records
+        )
+        requests: list[EndopintRequestParameter] = [
+            {
+                'method': 'POST',
+                'endpoint_name': 'records',
+                'payload': {
+                    'app': app,
+                    'records': records_
+                }
+            } for records_ in separated_records
+        ]
+        results = self.bulk_request_client.send(requests)['results']
+        return_value = []
+        for result in results:
+            ids = result['ids']
+            revisions = result['revisions']
+            return_value += [
+                {
+                    'id': val,
+                    'revision': revisions[num]
+                } for num, val in enumerate(ids)
+            ]
+        return return_value
+
+    def update_all_records(
+        self,
+        app: AppID,
+        records: Union[list[UpdateRecordForParameter], list[UpdateKeyRecordForParameter], list[Union[UpdateRecordForParameter, UpdateKeyRecordForParameter]]]
+    ):
+        return self.__update_all_records_recursive(app, records, len(records), [])
+    
+    def __update_all_records_recursive(
+        self,
+        app: AppID,
+        records: Union[list[UpdateRecordForParameter], list[UpdateKeyRecordForParameter], list[Union[UpdateRecordForParameter, UpdateKeyRecordForParameter]]],
+        num_of_all_records: int,
+        results: list
+    ):
+        CHUNK_LENGTH = self.bulk_request_client.REQUESTS_LENGTH_LIMIT * UPDATE_RECORDS_LIMIT
+        records_chunk = records[:CHUNK_LENGTH]
+        if len(records_chunk) == 0:
+            return {
+                'records': results
+            }
+        new_results = []
+        try:
+            new_results = self.__update_all_records_with_bulk_request(
+                app,
+                records_chunk
+            )
+        except Exception as e:
+            # TODO
+            raise e
+        return self.__update_all_records_recursive(
+            app,
+            records[CHUNK_LENGTH:],
+            num_of_all_records,
+            results + new_results
+        )
+    
+    def __update_all_records_with_bulk_request(
+        self,
+        app: AppID,
+        records: Union[list[UpdateRecordForParameter], list[UpdateKeyRecordForParameter], list[Union[UpdateRecordForParameter, UpdateKeyRecordForParameter]]],
+    ):
+        separated_records = self.__separate_array_recursive(
+            UPDATE_RECORDS_LIMIT,
+            [],
+            records
+        )
+        requests: list[EndopintRequestParameter] = [
+            {
+                'method': 'PUT',
+                'endpoint_name': 'records',
+                'payload': {
+                    'app': app,
+                    'records': records_,
+                }
+            } for records_ in separated_records
+        ]
+        results = self.bulk_request_client.send(requests)['results']
+        return_value = []
+        for result in results:
+            return_value += result['records']
+        return return_value
+    
+    def delete_all_reocrds(
+        self,
+        app: AppID,
+        records: list[DeleteRecordParameter]
+    ):
+        return self.__delete_all_records_recursive(app, records, len(records))
+    
+    def __delete_all_records_recursive(
+        self,
+        app: AppID,
+        records: list[DeleteRecordParameter],
+        num_of_all_records: int
+    ):
+        CHUNK_LENGTH = self.bulk_request_client.REQUESTS_LENGTH_LIMIT * DELETE_RECORDS_LIMIT
+        records_chunk = records[:CHUNK_LENGTH]
+        if len(records_chunk) == 0:
+            return {}
+        try:
+            self.__delete_all_records_with_bulk_request(
+                app,
+                records_chunk
+            )
+        except Exception as e:
+            # TODO
+            raise e
+        return self.__delete_all_records_recursive(
+            app,
+            records[CHUNK_LENGTH:],
+            num_of_all_records
+        )
+    
+    def __delete_all_records_with_bulk_request(
+        self,
+        app: AppID,
+        records: list[DeleteRecordParameter]
+    ):
+        separated_records = self.__separate_array_recursive(
+            DELETE_RECORDS_LIMIT,
+            [],
+            records
+        )
+        requests: list[EndopintRequestParameter] = [
+            {
+                'method': 'DELETE',
+                'endpoint_name': 'records',
+                'payload': {
+                    'app': app,
+                    'ids': [ record['id'] for record in records_ ],
+                    'revisions': [ record.get('revision', -1) for record in records_ ]
+                }
+            } for records_ in separated_records
+        ]
+        self.bulk_request_client.send(requests)['results']
+        return None
+    
+    def __separate_array_recursive(
+        self,
+        size: int,
+        separated: list[list],
+        array: list
+    ) -> list[list]:
+        chunk = array[:size]
+        if len(chunk) == 0:
+            return separated
+        return self.__separate_array_recursive(
+            size,
+            [*separated, chunk],
+            array[size:]
+        )
+    
+    def add_record_comment(
+        self,
+        app: AppID,
+        record: RecordID,
+        comment: Comment
+    ):
+        path = self.__build_path_with_guest_space_id('record/comment')
+        params = KintoneRequestParams(
+            app=app,
+            record=record,
+            comment=comment
+        )
+        return self.client.post(path, params)
+    
+    def delete_record_comment(
+        self,
+        app: AppID,
+        record: RecordID,
+        comment: CommentID
+    ):
+        path = self.__build_path_with_guest_space_id('record/comment')
+        params = KintoneRequestParams(
+            app=app,
+            record=record,
+            comment=comment
+        )
+        return self.client.delete(path, params)
+    
+    def get_record_comments(
+        self,
+        app: AppID,
+        record: RecordID,
+        order: Optional[Literal['asc', 'desc']] = None,
+        offset: Optional[int] = None,
+        limit: Optional[int] = None
+    ):
+        path = self.__build_path_with_guest_space_id('record/comments')
+        params = KintoneRequestParams(
+            app=app,
+            record=record,
+            order=order,
+            offset=offset,
+            limit=limit
+        )
+        return self.client.get(path, params)
+    
+    def update_record_assigness(
+        self,
+        app: AppID,
+        id: RecordID,
+        assignees: list[str],
+        revision: Optional[Revision] = None
+    ):
+        path = self.__build_path_with_guest_space_id('record/assignees')
+        params = KintoneRequestParams(
+            app=app,
+            id=id,
+            assignees=assignees,
+            revision=revision
+        )
+        return self.client.put(path, params)
+    
+    def update_record_status(
+        self,
+        app: AppID,
+        id: RecordID,
+        action: str,
+        assignees: Optional[list[str]] = None,
+        revision: Optional[Revision] = None
+    ):
+        path = self.__build_path_with_guest_space_id('record/status')
+        params = KintoneRequestParams(
+            app=app,
+            id=id,
+            action=action,
+            assignees=assignees,
+            revision=revision
+        )
+        return self.client.put(path, params)
+    
+    def update_records_status(
+        self,
+        app: AppID,
+        records: list[UpdateRecordStatusParameter]
+    ):
+        path = self.__build_path_with_guest_space_id('records/status')
+        params = KintoneRequestParams(
+            app=app,
+            records=records
+        )
+        return self.client.put(path, params)
+    
+    def __build_path_with_guest_space_id(self, endpoint_name: str) -> str:
+        return build_path(
+            endpoint_name=endpoint_name,
+            guest_space_id=self.guest_space_id
         )
```

### Comparing `pyntone-0.2.1/pyntone/http/http_client.py` & `pyntone-0.2.2/pyntone/http/http_client.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from typing import Any
-
-import requests
-
-from pyntone.kintone_request_config_builder import (
-    HttpMethod, KintoneRequestConfigBuilder, KintoneRequestParams)
-
-
-class KintoneError(Exception):
-    def __init__(self, message, text, json, status_code) -> None:
-        self.text = text
-        self.json = json
-        self.status_code = status_code
-        super().__init__(message)
-
-class HttpClent:
-    def __init__(self, config_builder: KintoneRequestConfigBuilder) -> None:
-        self.config_builder = config_builder
-    
-    def get(self, path: str, params: KintoneRequestParams) -> dict[str, Any]:
-        config = self.config_builder.build(HttpMethod.GET, path, params)
-        return self._send_request(config)
-
-    def post(self, path: str, params: KintoneRequestParams) -> dict[str, Any]:
-        config = self.config_builder.build(HttpMethod.POST, path, params)
-        return self._send_request(config)
-
-    def put(self, path: str, params: KintoneRequestParams) -> dict[str, Any]:
-        config = self.config_builder.build(HttpMethod.PUT, path, params)
-        return self._send_request(config)
-    
-    def delete(self, path: str, params: KintoneRequestParams) -> dict[str, Any]:
-        config = self.config_builder.build(HttpMethod.DELETE, path, params)
-        return self._send_request(config)
-    
-    def _send_request(self, config: dict[str, Any]) -> dict[str, Any]:
-        r = requests.request(**config)
-        self._is_success(r)
-        return r.json()
-
-    def _is_success(self, response: requests.Response) -> None:
-        if not (200 <= response.status_code < 300):
-            json = response.json()
-            raise KintoneError(json['message'], response.text, json, response.status_code)
+from typing import Any
+
+import requests
+
+from pyntone.kintone_request_config_builder import (
+    HttpMethod, KintoneRequestConfigBuilder, KintoneRequestParams)
+
+
+class KintoneError(Exception):
+    def __init__(self, message, text, json, status_code) -> None:
+        self.text = text
+        self.json = json
+        self.status_code = status_code
+        super().__init__(message)
+
+class HttpClent:
+    def __init__(self, config_builder: KintoneRequestConfigBuilder) -> None:
+        self.config_builder = config_builder
+    
+    def get(self, path: str, params: KintoneRequestParams) -> dict[str, Any]:
+        config = self.config_builder.build(HttpMethod.GET, path, params)
+        return self._send_request(config)
+
+    def post(self, path: str, params: KintoneRequestParams) -> dict[str, Any]:
+        config = self.config_builder.build(HttpMethod.POST, path, params)
+        return self._send_request(config)
+
+    def put(self, path: str, params: KintoneRequestParams) -> dict[str, Any]:
+        config = self.config_builder.build(HttpMethod.PUT, path, params)
+        return self._send_request(config)
+    
+    def delete(self, path: str, params: KintoneRequestParams) -> dict[str, Any]:
+        config = self.config_builder.build(HttpMethod.DELETE, path, params)
+        return self._send_request(config)
+    
+    def _send_request(self, config: dict[str, Any]) -> dict[str, Any]:
+        r = requests.request(**config)
+        self._is_success(r)
+        return r.json()
+
+    def _is_success(self, response: requests.Response) -> None:
+        if not (200 <= response.status_code < 300):
+            json = response.json()
+            raise KintoneError(json['message'], response.text, json, response.status_code)
```

### Comparing `pyntone-0.2.1/pyntone/kintone_rest_api_client.py` & `pyntone-0.2.2/pyntone/kintone_rest_api_client.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import re
-from typing import Optional, TypedDict, Union
-
-from pyntone.client.bulk_request_client import BulkRequestClient
-from pyntone.client.record_client import RecordClient
-from pyntone.http.http_client import HttpClent
-from pyntone.kintone_request_config_builder import KintoneRequestConfigBuilder
-from pyntone.types.auth import DiscriminatedAuth
-
-
-class FeatureFlags(TypedDict):
-    enableAbortSearchError: bool
-
-
-class KintoneRestAPIClient:
-    def __init__(
-        self,
-        base_url: str,
-        auth: DiscriminatedAuth,
-        guest_space_id: Union[int, str, None] = None,
-        basic_auth = None,
-        client_cert_auth = None,
-        proxy = None,
-        feature_flags = None,
-        user_agent: Optional[str] = None
-    ) -> None:
-        self.__base_url = re.sub('/+$', '', base_url)
-        
-        
-        request_config_builder = KintoneRequestConfigBuilder(auth=auth, base_url=self.__base_url)
-        httpClient = HttpClent(config_builder=request_config_builder)
-        
-        self.bulkRequest = BulkRequestClient(httpClient, guest_space_id)
-        self.record = RecordClient(httpClient, self.bulkRequest, guest_space_id)
-        # self.app = AppClient()
+import re
+from typing import Optional, TypedDict, Union
+
+from pyntone.client.bulk_request_client import BulkRequestClient
+from pyntone.client.record_client import RecordClient
+from pyntone.http.http_client import HttpClent
+from pyntone.kintone_request_config_builder import KintoneRequestConfigBuilder
+from pyntone.types.auth import DiscriminatedAuth
+
+
+class FeatureFlags(TypedDict):
+    enableAbortSearchError: bool
+
+
+class KintoneRestAPIClient:
+    def __init__(
+        self,
+        base_url: str,
+        auth: DiscriminatedAuth,
+        guest_space_id: Union[int, str, None] = None,
+        basic_auth = None,
+        client_cert_auth = None,
+        proxy = None,
+        feature_flags = None,
+        user_agent: Optional[str] = None
+    ) -> None:
+        self.__base_url = re.sub('/+$', '', base_url)
+        
+        
+        request_config_builder = KintoneRequestConfigBuilder(auth=auth, base_url=self.__base_url)
+        httpClient = HttpClent(config_builder=request_config_builder)
+        
+        self.bulkRequest = BulkRequestClient(httpClient, guest_space_id)
+        self.record = RecordClient(httpClient, self.bulkRequest, guest_space_id)
+        # self.app = AppClient()
         # self.file = FileClient()
```

### Comparing `pyntone-0.2.1/pyntone.egg-info/SOURCES.txt` & `pyntone-0.2.2/pyntone.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+README.md
 pyproject.toml
 setup.cfg
 pyntone/__init__.py
 pyntone/kintone_request_config_builder.py
 pyntone/kintone_rest_api_client.py
 pyntone/url.py
 pyntone.egg-info/PKG-INFO
@@ -15,8 +16,8 @@
 pyntone/client/record_client.py
 pyntone/http/__init__.py
 pyntone/http/http_client.py
 pyntone/types/__init__.py
 pyntone/types/auth.py
 pyntone/types/record.py
 tests/__init__.py
-tests/record.py
+tests/test_record.py
```

