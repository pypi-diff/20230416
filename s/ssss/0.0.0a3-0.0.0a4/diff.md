# Comparing `tmp/ssss-0.0.0a3.tar.gz` & `tmp/ssss-0.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssss-0.0.0a3.tar", max compression
+gzip compressed data, was "ssss-0.0.0a4.tar", max compression
```

## Comparing `ssss-0.0.0a3.tar` & `ssss-0.0.0a4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2023-04-15 07:46:56.462384 ssss-0.0.0a3/LICENSE
--rw-r--r--   0        0        0      640 2023-04-15 16:24:04.382517 ssss-0.0.0a3/README.md
--rw-r--r--   0        0        0      563 2023-04-15 19:34:18.873058 ssss-0.0.0a3/pyproject.toml
--rw-r--r--   0        0        0      457 2023-04-15 07:46:56.471383 ssss-0.0.0a3/ssss/__init__.py
--rw-r--r--   0        0        0       90 2023-04-15 07:46:56.466384 ssss-0.0.0a3/ssss/common/__init__.py
--rw-r--r--   0        0        0      119 2023-04-15 07:46:56.467383 ssss-0.0.0a3/ssss/common/application/__init__.py
--rw-r--r--   0        0        0     1646 2023-04-15 16:15:47.286603 ssss-0.0.0a3/ssss/common/application/variables.py
--rw-r--r--   0        0        0      187 2023-04-15 07:46:56.467383 ssss-0.0.0a3/ssss/common/fs/__init__.py
--rw-r--r--   0        0        0      933 2023-04-15 12:27:22.411863 ssss-0.0.0a3/ssss/common/fs/directory.py
--rw-r--r--   0        0        0     1152 2023-04-15 12:40:52.829570 ssss-0.0.0a3/ssss/common/fs/file.py
--rw-r--r--   0        0        0       52 2023-04-15 07:46:56.463384 ssss-0.0.0a3/ssss/common/md/__init__.py
--rw-r--r--   0        0        0      799 2023-04-15 11:29:22.866819 ssss-0.0.0a3/ssss/common/md/info.py
--rw-r--r--   0        0        0     1418 2023-04-15 12:32:53.750536 ssss-0.0.0a3/ssss/common/md/render.py
--rw-r--r--   0        0        0       75 2023-04-15 07:46:56.471383 ssss-0.0.0a3/ssss/configuration/__init__.py
--rw-r--r--   0        0        0     4700 2023-04-15 16:23:17.484279 ssss-0.0.0a3/ssss/configuration/application.py
--rw-r--r--   0        0        0      470 2023-04-15 07:59:41.196054 ssss-0.0.0a3/ssss/configuration/arguments.py
--rw-r--r--   0        0        0      381 2023-04-15 07:46:56.469384 ssss-0.0.0a3/ssss/configuration/default.py
--rw-r--r--   0        0        0       31 2023-04-15 07:46:56.471383 ssss-0.0.0a3/ssss/generate/__init__.py
--rw-r--r--   0        0        0      371 2023-04-15 07:46:56.476383 ssss-0.0.0a3/ssss/generate/site.py
--rw-r--r--   0        0        0     1335 1970-01-01 00:00:00.000000 ssss-0.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-15 07:46:56.462384 ssss-0.0.0a4/LICENSE
+-rw-r--r--   0        0        0      941 2023-04-16 07:29:37.964974 ssss-0.0.0a4/README.md
+-rw-r--r--   0        0        0      631 2023-04-16 07:33:55.505795 ssss-0.0.0a4/pyproject.toml
+-rw-r--r--   0        0        0      457 2023-04-15 07:46:56.471383 ssss-0.0.0a4/ssss/__init__.py
+-rw-r--r--   0        0        0       90 2023-04-15 07:46:56.466384 ssss-0.0.0a4/ssss/common/__init__.py
+-rw-r--r--   0        0        0      119 2023-04-15 07:46:56.467383 ssss-0.0.0a4/ssss/common/application/__init__.py
+-rw-r--r--   0        0        0     1646 2023-04-15 16:15:47.286603 ssss-0.0.0a4/ssss/common/application/variables.py
+-rw-r--r--   0        0        0      187 2023-04-15 07:46:56.467383 ssss-0.0.0a4/ssss/common/fs/__init__.py
+-rw-r--r--   0        0        0      933 2023-04-15 12:27:22.411863 ssss-0.0.0a4/ssss/common/fs/directory.py
+-rw-r--r--   0        0        0     1152 2023-04-15 12:40:52.829570 ssss-0.0.0a4/ssss/common/fs/file.py
+-rw-r--r--   0        0        0       52 2023-04-15 07:46:56.463384 ssss-0.0.0a4/ssss/common/md/__init__.py
+-rw-r--r--   0        0        0      799 2023-04-15 11:29:22.866819 ssss-0.0.0a4/ssss/common/md/info.py
+-rw-r--r--   0        0        0     1418 2023-04-15 12:32:53.750536 ssss-0.0.0a4/ssss/common/md/render.py
+-rw-r--r--   0        0        0       75 2023-04-15 07:46:56.471383 ssss-0.0.0a4/ssss/configuration/__init__.py
+-rw-r--r--   0        0        0     4700 2023-04-15 16:23:17.484279 ssss-0.0.0a4/ssss/configuration/application.py
+-rw-r--r--   0        0        0      470 2023-04-15 07:59:41.196054 ssss-0.0.0a4/ssss/configuration/arguments.py
+-rw-r--r--   0        0        0      381 2023-04-15 07:46:56.469384 ssss-0.0.0a4/ssss/configuration/default.py
+-rw-r--r--   0        0        0       31 2023-04-15 07:46:56.471383 ssss-0.0.0a4/ssss/generate/__init__.py
+-rw-r--r--   0        0        0      371 2023-04-15 07:46:56.476383 ssss-0.0.0a4/ssss/generate/site.py
+-rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 ssss-0.0.0a4/PKG-INFO
```

### Comparing `ssss-0.0.0a3/LICENSE` & `ssss-0.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `ssss-0.0.0a3/ssss/common/application/variables.py` & `ssss-0.0.0a4/ssss/common/application/variables.py`

 * *Files identical despite different names*

### Comparing `ssss-0.0.0a3/ssss/common/fs/directory.py` & `ssss-0.0.0a4/ssss/common/fs/directory.py`

 * *Files identical despite different names*

### Comparing `ssss-0.0.0a3/ssss/common/fs/file.py` & `ssss-0.0.0a4/ssss/common/fs/file.py`

 * *Files identical despite different names*

### Comparing `ssss-0.0.0a3/ssss/common/md/info.py` & `ssss-0.0.0a4/ssss/common/md/info.py`

 * *Files identical despite different names*

### Comparing `ssss-0.0.0a3/ssss/common/md/render.py` & `ssss-0.0.0a4/ssss/common/md/render.py`

 * *Files identical despite different names*

### Comparing `ssss-0.0.0a3/ssss/configuration/application.py` & `ssss-0.0.0a4/ssss/configuration/application.py`

 * *Files identical despite different names*

