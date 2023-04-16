# Comparing `tmp/doji_core-0.1.1.tar.gz` & `tmp/doji_core-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doji_core-0.1.1.tar", max compression
+gzip compressed data, was "doji_core-0.1.2.tar", max compression
```

## Comparing `doji_core-0.1.1.tar` & `doji_core-0.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1069 2023-04-16 10:49:32.941115 doji_core-0.1.1/LICENSE
--rw-r--r--   0        0        0       78 2023-04-16 10:49:32.941115 doji_core-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.941115 doji_core-0.1.1/doji/core/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.941115 doji_core-0.1.1/doji/core/api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.941115 doji_core-0.1.1/doji/core/api/classes/__init__.py
--rw-r--r--   0        0        0     6102 2023-04-16 12:39:02.353036 doji_core-0.1.1/doji/core/api/classes/api.py
--rw-r--r--   0        0        0     4137 2023-04-16 10:49:32.945115 doji_core-0.1.1/doji/core/api/classes/response.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.1/doji/core/api/mixins/__init__.py
--rw-r--r--   0        0        0     3303 2023-04-16 10:49:32.945115 doji_core-0.1.1/doji/core/api/mixins/api_mixin.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.1/doji/core/asset/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.1/doji/core/asset/classes/__init__.py
--rw-r--r--   0        0        0     3050 2023-04-16 14:02:21.510452 doji_core-0.1.1/doji/core/asset/classes/asset.py
--rw-r--r--   0        0        0     2603 2023-04-16 15:07:54.310882 doji_core-0.1.1/doji/core/asset/classes/asset_instances.py
--rw-r--r--   0        0        0     4519 2023-04-16 14:09:13.680598 doji_core-0.1.1/doji/core/asset/classes/asset_pair.py
--rw-r--r--   0        0        0     2641 2023-04-16 15:37:29.236623 doji_core-0.1.1/doji/core/asset/classes/asset_pair_instances.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.1/doji/core/asset/mixins/__init__.py
--rw-r--r--   0        0        0     6993 2023-04-16 15:19:48.797600 doji_core-0.1.1/doji/core/asset/mixins/asset_pairs_mixin.py
--rw-r--r--   0        0        0     9416 2023-04-16 15:23:35.086566 doji_core-0.1.1/doji/core/asset/mixins/assets_mixin.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.1/doji/core/currency/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.1/doji/core/currency/classes/__init__.py
--rw-r--r--   0        0        0     1210 2023-04-16 10:49:32.945115 doji_core-0.1.1/doji/core/currency/classes/currency.py
--rw-r--r--   0        0        0     1348 2023-04-16 10:49:32.945115 doji_core-0.1.1/doji/core/currency/classes/currency_instances.py
--rw-r--r--   0        0        0     1303 2023-04-16 10:49:32.945115 doji_core-0.1.1/doji/core/currency/classes/currency_pair.py
--rw-r--r--   0        0        0     1388 2023-04-16 10:49:32.945115 doji_core-0.1.1/doji/core/currency/classes/currency_pair_instances.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.1/doji/core/currency/mixins/__init__.py
--rw-r--r--   0        0        0    14713 2023-04-16 15:41:11.805369 doji_core-0.1.1/doji/core/currency/mixins/currencies_mixin.py
--rw-r--r--   0        0        0    10188 2023-04-16 15:47:25.691429 doji_core-0.1.1/doji/core/currency/mixins/currency_pairs_mixin.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.1/doji/core/exchange/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.1/doji/core/exchange/classes/__init__.py
--rw-r--r--   0        0        0     1586 2023-04-16 14:51:14.088258 doji_core-0.1.1/doji/core/exchange/classes/currency_exchange.py
--rw-r--r--   0        0        0     4870 2023-04-16 14:51:38.852483 doji_core-0.1.1/doji/core/exchange/classes/exchange.py
--rw-r--r--   0        0        0        0 2023-04-16 16:03:32.948981 doji_core-0.1.1/doji/core/py.typed
--rw-r--r--   0        0        0     1914 2023-04-16 10:49:32.945115 doji_core-0.1.1/doji/core/types/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.1/doji/core/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.1/doji/core/utils/classes/__init__.py
--rw-r--r--   0        0        0     1470 2023-04-16 14:01:48.390107 doji_core-0.1.1/doji/core/utils/classes/instance.py
--rw-r--r--   0        0        0     9168 2023-04-16 15:40:46.253260 doji_core-0.1.1/doji/core/utils/classes/instances.py
--rw-r--r--   0        0        0      544 2023-04-16 16:04:14.964892 doji_core-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 doji_core-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-16 10:49:32.941115 doji_core-0.1.2/LICENSE
+-rw-r--r--   0        0        0       78 2023-04-16 10:49:32.941115 doji_core-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.941115 doji_core-0.1.2/doji/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.941115 doji_core-0.1.2/doji/core/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.941115 doji_core-0.1.2/doji/core/api/classes/__init__.py
+-rw-r--r--   0        0        0     6102 2023-04-16 12:39:02.353036 doji_core-0.1.2/doji/core/api/classes/api.py
+-rw-r--r--   0        0        0     4137 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/api/classes/response.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/api/mixins/__init__.py
+-rw-r--r--   0        0        0     3303 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/api/mixins/api_mixin.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/asset/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/asset/classes/__init__.py
+-rw-r--r--   0        0        0     3050 2023-04-16 14:02:21.510452 doji_core-0.1.2/doji/core/asset/classes/asset.py
+-rw-r--r--   0        0        0     2603 2023-04-16 15:07:54.310882 doji_core-0.1.2/doji/core/asset/classes/asset_instances.py
+-rw-r--r--   0        0        0     4519 2023-04-16 14:09:13.680598 doji_core-0.1.2/doji/core/asset/classes/asset_pair.py
+-rw-r--r--   0        0        0     2641 2023-04-16 15:37:29.236623 doji_core-0.1.2/doji/core/asset/classes/asset_pair_instances.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/asset/mixins/__init__.py
+-rw-r--r--   0        0        0     6993 2023-04-16 15:19:48.797600 doji_core-0.1.2/doji/core/asset/mixins/asset_pairs_mixin.py
+-rw-r--r--   0        0        0     9416 2023-04-16 15:23:35.086566 doji_core-0.1.2/doji/core/asset/mixins/assets_mixin.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/currency/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/currency/classes/__init__.py
+-rw-r--r--   0        0        0     1210 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/currency/classes/currency.py
+-rw-r--r--   0        0        0     1348 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/currency/classes/currency_instances.py
+-rw-r--r--   0        0        0     1303 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/currency/classes/currency_pair.py
+-rw-r--r--   0        0        0     1388 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/currency/classes/currency_pair_instances.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/currency/mixins/__init__.py
+-rw-r--r--   0        0        0    14713 2023-04-16 15:41:11.805369 doji_core-0.1.2/doji/core/currency/mixins/currencies_mixin.py
+-rw-r--r--   0        0        0    10188 2023-04-16 15:47:25.691429 doji_core-0.1.2/doji/core/currency/mixins/currency_pairs_mixin.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/exchange/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/exchange/classes/__init__.py
+-rw-r--r--   0        0        0     1586 2023-04-16 14:51:14.088258 doji_core-0.1.2/doji/core/exchange/classes/currency_exchange.py
+-rw-r--r--   0        0        0     4870 2023-04-16 14:51:38.852483 doji_core-0.1.2/doji/core/exchange/classes/exchange.py
+-rw-r--r--   0        0        0        0 2023-04-16 16:03:32.948981 doji_core-0.1.2/doji/core/py.typed
+-rw-r--r--   0        0        0     2071 2023-04-16 16:30:03.427132 doji_core-0.1.2/doji/core/types/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/utils/classes/__init__.py
+-rw-r--r--   0        0        0     1470 2023-04-16 14:01:48.390107 doji_core-0.1.2/doji/core/utils/classes/instance.py
+-rw-r--r--   0        0        0     9168 2023-04-16 15:40:46.253260 doji_core-0.1.2/doji/core/utils/classes/instances.py
+-rw-r--r--   0        0        0      544 2023-04-16 16:30:21.175045 doji_core-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 doji_core-0.1.2/PKG-INFO
```

### Comparing `doji_core-0.1.1/LICENSE` & `doji_core-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.1/doji/core/api/classes/api.py` & `doji_core-0.1.2/doji/core/api/classes/api.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.1/doji/core/api/classes/response.py` & `doji_core-0.1.2/doji/core/api/classes/response.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.1/doji/core/api/mixins/api_mixin.py` & `doji_core-0.1.2/doji/core/api/mixins/api_mixin.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.1/doji/core/asset/classes/asset.py` & `doji_core-0.1.2/doji/core/asset/classes/asset.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.1/doji/core/asset/classes/asset_instances.py` & `doji_core-0.1.2/doji/core/asset/classes/asset_instances.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.1/doji/core/asset/classes/asset_pair.py` & `doji_core-0.1.2/doji/core/asset/classes/asset_pair.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.1/doji/core/asset/classes/asset_pair_instances.py` & `doji_core-0.1.2/doji/core/asset/classes/asset_pair_instances.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.1/doji/core/asset/mixins/asset_pairs_mixin.py` & `doji_core-0.1.2/doji/core/asset/mixins/asset_pairs_mixin.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.1/doji/core/asset/mixins/assets_mixin.py` & `doji_core-0.1.2/doji/core/asset/mixins/assets_mixin.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.1/doji/core/currency/classes/currency.py` & `doji_core-0.1.2/doji/core/currency/classes/currency.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.1/doji/core/currency/classes/currency_instances.py` & `doji_core-0.1.2/doji/core/currency/classes/currency_instances.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.1/doji/core/currency/classes/currency_pair.py` & `doji_core-0.1.2/doji/core/currency/classes/currency_pair.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.1/doji/core/currency/classes/currency_pair_instances.py` & `doji_core-0.1.2/doji/core/currency/classes/currency_pair_instances.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.1/doji/core/currency/mixins/currencies_mixin.py` & `doji_core-0.1.2/doji/core/currency/mixins/currencies_mixin.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.1/doji/core/currency/mixins/currency_pairs_mixin.py` & `doji_core-0.1.2/doji/core/currency/mixins/currency_pairs_mixin.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.1/doji/core/exchange/classes/currency_exchange.py` & `doji_core-0.1.2/doji/core/exchange/classes/currency_exchange.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.1/doji/core/exchange/classes/exchange.py` & `doji_core-0.1.2/doji/core/exchange/classes/exchange.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.1/doji/core/types/__init__.py` & `doji_core-0.1.2/doji/core/types/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,9 +18,15 @@
 # ┌─────────────────────────────────────────────────────────────────────────────────────
 # │ JSON
 # └─────────────────────────────────────────────────────────────────────────────────────
 
 # Define a generic JSON value type
 JSONValue = str | int | float | bool | None
 
+# Define a generic JSON dict type
+JSONDict = dict[str, JSONValue | "JSON" | list["JSON"]]
+
+# Define a generic JSON array type
+JSONArray = list[JSONValue | "JSON" | JSONDict]
+
 # Define a generic JSON type
-JSON = dict[str, JSONValue] | list[JSONValue] | JSONValue
+JSON = JSONValue | JSONDict | JSONArray
```

### Comparing `doji_core-0.1.1/doji/core/utils/classes/instance.py` & `doji_core-0.1.2/doji/core/utils/classes/instance.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.1/doji/core/utils/classes/instances.py` & `doji_core-0.1.2/doji/core/utils/classes/instances.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.1/pyproject.toml` & `doji_core-0.1.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "doji-core"
-version = "0.1.1"
+version = "0.1.2"
 description = "A repository for Doji, a trade analytics suite written in Python."
 authors = ["Sean O'Leary <seamicole@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "doji"}]
 
 [tool.poetry.dependencies]
```

### Comparing `doji_core-0.1.1/PKG-INFO` & `doji_core-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doji-core
-Version: 0.1.1
+Version: 0.1.2
 Summary: A repository for Doji, a trade analytics suite written in Python.
 License: MIT
 Author: Sean O'Leary
 Author-email: seamicole@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

