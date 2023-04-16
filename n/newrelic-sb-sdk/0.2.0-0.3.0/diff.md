# Comparing `tmp/newrelic_sb_sdk-0.2.0.tar.gz` & `tmp/newrelic_sb_sdk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newrelic_sb_sdk-0.2.0.tar", max compression
+gzip compressed data, was "newrelic_sb_sdk-0.3.0.tar", max compression
```

## Comparing `newrelic_sb_sdk-0.2.0.tar` & `newrelic_sb_sdk-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0      490 2023-03-12 12:21:39.786341 newrelic_sb_sdk-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2023-03-04 19:28:34.334390 newrelic_sb_sdk-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     2407 2023-03-10 03:56:51.412939 newrelic_sb_sdk-0.2.0/README.md
--rw-r--r--   0        0        0     2613 2023-03-12 12:21:39.786341 newrelic_sb_sdk-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-03-12 12:21:39.786341 newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/__init__.py
--rw-r--r--   0        0        0   380313 2023-03-12 12:21:33.158306 newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/_modidx.py
--rw-r--r--   0        0        0     4872 2023-03-12 12:21:33.158306 newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/alerts/__init__.py
--rw-r--r--   0        0        0     1541 2023-03-12 12:21:33.158306 newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/alerts/enums.py
--rw-r--r--   0        0        0      769 2023-03-12 12:21:33.158306 newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/alerts/utils.py
--rw-r--r--   0        0        0     2016 2023-03-12 12:21:33.158306 newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/client/__init__.py
--rw-r--r--   0        0        0        0 2023-03-12 12:17:42.328835 newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/core/__init__.py
--rw-r--r--   0        0        0      372 2023-03-12 12:18:04.377000 newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/core/base.py
--rw-r--r--   0        0        0      747 2023-03-12 12:18:04.377000 newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/core/encoders.py
--rw-r--r--   0        0        0     2183 2023-03-12 12:18:04.377000 newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/core/mixins.py
--rw-r--r--   0        0        0     1236 2023-03-12 12:18:04.377000 newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/dashboards/__init__.py
--rw-r--r--   0        0        0     1095 2023-03-12 12:18:04.377000 newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/dashboards/enums.py
--rw-r--r--   0        0        0      969 2023-03-12 12:18:04.377000 newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/dashboards/pages.py
--rw-r--r--   0        0        0      562 2023-03-12 12:18:04.377000 newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/dashboards/utils.py
--rw-r--r--   0        0        0     3456 2023-03-12 12:18:04.377000 newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/dashboards/widgets.py
--rw-r--r--   0        0        0      200 2023-03-12 12:18:04.377000 newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/graphql/__init__.py
--rw-r--r--   0        0        0   163843 2023-03-12 12:18:04.381000 newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/graphql/enums.py
--rw-r--r--   0        0        0   233611 2023-03-12 12:18:04.381000 newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/graphql/input_objects.py
--rw-r--r--   0        0        0   419485 2023-03-12 12:18:04.385000 newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/graphql/objects.py
--rw-r--r--   0        0        0     6331 2023-03-12 12:18:04.385000 newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/graphql/scalars.py
--rw-r--r--   0        0        0        0 2023-03-12 12:17:42.328835 newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/utils/__init__.py
--rw-r--r--   0        0        0      279 2023-03-12 12:21:33.158306 newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/utils/query.py
--rw-r--r--   0        0        0      729 2023-03-12 12:21:33.158306 newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/utils/response.py
--rw-r--r--   0        0        0     1901 2023-03-12 12:18:04.385000 newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/utils/text.py
--rw-r--r--   0        0        0     3554 1970-01-01 00:00:00.000000 newrelic_sb_sdk-0.2.0/setup.py
--rw-r--r--   0        0        0     4085 1970-01-01 00:00:00.000000 newrelic_sb_sdk-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      602 2023-04-16 17:39:09.459229 newrelic_sb_sdk-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2023-03-04 19:28:34.334390 newrelic_sb_sdk-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     1619 2023-04-16 17:22:47.206977 newrelic_sb_sdk-0.3.0/README.md
+-rw-r--r--   0        0        0     2652 2023-04-16 17:39:09.455229 newrelic_sb_sdk-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-16 17:39:13.975248 newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/__init__.py
+-rw-r--r--   0        0        0   380313 2023-04-16 17:35:33.162296 newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/_modidx.py
+-rw-r--r--   0        0        0     4872 2023-04-16 17:35:33.162296 newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/alerts/__init__.py
+-rw-r--r--   0        0        0     1541 2023-04-16 17:35:33.162296 newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/alerts/enums.py
+-rw-r--r--   0        0        0      769 2023-04-16 17:35:33.158296 newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/alerts/utils.py
+-rw-r--r--   0        0        0     2016 2023-04-16 17:35:33.158296 newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 17:35:33.162296 newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/core/__init__.py
+-rw-r--r--   0        0        0      372 2023-04-16 17:35:33.158296 newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/core/base.py
+-rw-r--r--   0        0        0      747 2023-04-16 17:35:33.158296 newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/core/encoders.py
+-rw-r--r--   0        0        0     2183 2023-04-16 17:35:33.158296 newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/core/mixins.py
+-rw-r--r--   0        0        0     1236 2023-04-16 17:35:33.158296 newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/dashboards/__init__.py
+-rw-r--r--   0        0        0     1095 2023-04-16 17:35:33.162296 newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/dashboards/enums.py
+-rw-r--r--   0        0        0      969 2023-04-16 17:35:33.158296 newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/dashboards/pages.py
+-rw-r--r--   0        0        0      562 2023-04-16 17:35:33.158296 newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/dashboards/utils.py
+-rw-r--r--   0        0        0     3456 2023-04-16 17:35:33.158296 newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/dashboards/widgets.py
+-rw-r--r--   0        0        0      200 2023-04-16 17:35:33.162296 newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/graphql/__init__.py
+-rw-r--r--   0        0        0   163843 2023-04-16 17:35:33.162296 newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/graphql/enums.py
+-rw-r--r--   0        0        0   233611 2023-04-16 17:35:33.158296 newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/graphql/input_objects.py
+-rw-r--r--   0        0        0   419485 2023-04-16 17:35:33.166296 newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/graphql/objects.py
+-rw-r--r--   0        0        0     6331 2023-04-16 17:35:33.162296 newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/graphql/scalars.py
+-rw-r--r--   0        0        0        0 2023-04-16 17:35:33.158296 newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/utils/__init__.py
+-rw-r--r--   0        0        0      279 2023-04-16 17:35:33.158296 newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/utils/query.py
+-rw-r--r--   0        0        0      729 2023-04-16 17:35:33.158296 newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/utils/response.py
+-rw-r--r--   0        0        0     1901 2023-04-16 17:35:33.158296 newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/utils/text.py
+-rw-r--r--   0        0        0     3327 1970-01-01 00:00:00.000000 newrelic_sb_sdk-0.3.0/PKG-INFO
```

### Comparing `newrelic_sb_sdk-0.2.0/LICENSE.txt` & `newrelic_sb_sdk-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.2.0/pyproject.toml` & `newrelic_sb_sdk-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 [tool.poetry]
 name = "newrelic-sb-sdk"
-version = "0.2.0"
+version = "0.3.0"
 description = "New Relic SDK to interact with API for data retrieving"
 authors = [
   "SoftButterfly Development Team <dev@softbutterfly.io>",
   "zodiacfireworks <martin.vuelta@gmail.com>"
 ]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface"
 repository = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface"
-documentation = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface/wiki"
-keywords = ["Softbutterfly", "New Relic", "SDK"]
+documentation = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface/-/wikis"
+keywords = [
+  "Softbutterfly",
+  "New Relic",
+  "SDK",
+]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Natural Language :: English",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
@@ -28,16 +32,16 @@
 ]
 include = [
   "LICENSE.txt",
   "CHANGELOG.md",
 ]
 
 [tool.poetry.urls]
-"Download" = "https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/archive/v0.2.0.tar.gz"
-"Bug Tracker" = "https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/issues"
+"Download" = "https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/archive/v0.3.0/newrelic-sb-sdk-v0.3.0.tar.gz"
+"Bug Tracker" = "https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/issues"
 
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
 enforce-typing = "^1.0.0.post1"
 python-dotenv = "^1.0.0"
 requests = "^2.28.2"
```

### Comparing `newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/_modidx.py` & `newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/_modidx.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/alerts/__init__.py` & `newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/alerts/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/alerts/enums.py` & `newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/alerts/enums.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/alerts/utils.py` & `newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/alerts/utils.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/client/__init__.py` & `newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/client/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/core/encoders.py` & `newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/core/encoders.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/core/mixins.py` & `newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/core/mixins.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/dashboards/__init__.py` & `newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/dashboards/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/dashboards/enums.py` & `newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/dashboards/enums.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/dashboards/pages.py` & `newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/dashboards/pages.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/dashboards/utils.py` & `newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/dashboards/utils.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/dashboards/widgets.py` & `newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/dashboards/widgets.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/graphql/enums.py` & `newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/graphql/enums.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/graphql/input_objects.py` & `newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/graphql/input_objects.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/graphql/objects.py` & `newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/graphql/objects.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/graphql/scalars.py` & `newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/graphql/scalars.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/utils/response.py` & `newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/utils/response.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.2.0/src/newrelic_sb_sdk/utils/text.py` & `newrelic_sb_sdk-0.3.0/src/newrelic_sb_sdk/utils/text.py`

 * *Files identical despite different names*

