# Comparing `tmp/webslides-0.5.5.tar.gz` & `tmp/webslides-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webslides-0.5.5.tar", last modified: Sun Apr 16 19:01:51 2023, max compression
+gzip compressed data, was "webslides-0.5.6.tar", last modified: Sun Apr 16 19:12:19 2023, max compression
```

## Comparing `webslides-0.5.5.tar` & `webslides-0.5.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 19:01:51.956523 webslides-0.5.5/
--rw-rw-rw-   0        0        0      193 2023-04-16 18:43:46.000000 webslides-0.5.5/MANIFEST.in
--rw-rw-rw-   0        0        0     6621 2023-04-16 19:01:51.955523 webslides-0.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     6275 2023-04-16 18:40:55.000000 webslides-0.5.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-16 19:01:51.957521 webslides-0.5.5/setup.cfg
--rw-rw-rw-   0        0        0      537 2023-04-16 19:01:49.000000 webslides-0.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 19:01:51.871523 webslides-0.5.5/webslides/
--rw-rw-rw-   0        0        0       56 2023-04-16 16:05:42.000000 webslides-0.5.5/webslides/__init__.py
--rw-rw-rw-   0        0        0     5017 2023-04-16 18:37:59.000000 webslides-0.5.5/webslides/main.py
-drwxrwxrwx   0        0        0        0 2023-04-16 19:01:51.952523 webslides-0.5.5/webslides/modules/
--rw-rw-rw-   0        0        0     9881 2023-04-16 18:36:21.000000 webslides-0.5.5/webslides/modules/demo.py
--rw-rw-rw-   0        0        0     3800 2023-04-15 17:59:58.000000 webslides-0.5.5/webslides/modules/generate.py
--rw-rw-rw-   0        0        0     2383 2023-04-16 15:35:26.000000 webslides-0.5.5/webslides/modules/hello_world.py
--rw-rw-rw-   0        0        0     2824 2023-04-16 17:57:26.000000 webslides-0.5.5/webslides/modules/input_validations.py
--rw-rw-rw-   0        0        0     1724 2023-04-16 16:39:50.000000 webslides-0.5.5/webslides/modules/other.py
--rw-rw-rw-   0        0        0     2998 2023-04-16 18:40:55.000000 webslides-0.5.5/webslides/modules/pagination.py
--rw-rw-rw-   0        0        0     7774 2023-04-16 18:40:55.000000 webslides-0.5.5/webslides/modules/tohtml.py
-drwxrwxrwx   0        0        0        0 2023-04-16 19:01:51.921523 webslides-0.5.5/webslides.egg-info/
--rw-rw-rw-   0        0        0     6621 2023-04-16 19:01:51.000000 webslides-0.5.5/webslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2023-04-16 19:01:51.000000 webslides-0.5.5/webslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 19:01:51.000000 webslides-0.5.5/webslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-16 19:01:51.000000 webslides-0.5.5/webslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-16 19:01:51.000000 webslides-0.5.5/webslides.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 19:12:19.534754 webslides-0.5.6/
+-rw-rw-rw-   0        0        0      193 2023-04-16 18:43:46.000000 webslides-0.5.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     6621 2023-04-16 19:12:19.532754 webslides-0.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6275 2023-04-16 18:40:55.000000 webslides-0.5.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-16 19:12:19.535756 webslides-0.5.6/setup.cfg
+-rw-rw-rw-   0        0        0      537 2023-04-16 19:12:16.000000 webslides-0.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 19:12:19.463756 webslides-0.5.6/webslides/
+-rw-rw-rw-   0        0        0       56 2023-04-16 16:05:42.000000 webslides-0.5.6/webslides/__init__.py
+-rw-rw-rw-   0        0        0     5017 2023-04-16 18:37:59.000000 webslides-0.5.6/webslides/main.py
+drwxrwxrwx   0        0        0        0 2023-04-16 19:12:19.521757 webslides-0.5.6/webslides/modules/
+-rw-rw-rw-   0        0        0     9881 2023-04-16 19:12:16.000000 webslides-0.5.6/webslides/modules/demo.py
+-rw-rw-rw-   0        0        0     3800 2023-04-15 17:59:58.000000 webslides-0.5.6/webslides/modules/generate.py
+-rw-rw-rw-   0        0        0     2383 2023-04-16 15:35:26.000000 webslides-0.5.6/webslides/modules/hello_world.py
+-rw-rw-rw-   0        0        0     2824 2023-04-16 17:57:26.000000 webslides-0.5.6/webslides/modules/input_validations.py
+-rw-rw-rw-   0        0        0     1724 2023-04-16 16:39:50.000000 webslides-0.5.6/webslides/modules/other.py
+-rw-rw-rw-   0        0        0     2998 2023-04-16 18:40:55.000000 webslides-0.5.6/webslides/modules/pagination.py
+-rw-rw-rw-   0        0        0     7774 2023-04-16 18:40:55.000000 webslides-0.5.6/webslides/modules/tohtml.py
+drwxrwxrwx   0        0        0        0 2023-04-16 19:12:19.495757 webslides-0.5.6/webslides.egg-info/
+-rw-rw-rw-   0        0        0     6621 2023-04-16 19:12:19.000000 webslides-0.5.6/webslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2023-04-16 19:12:19.000000 webslides-0.5.6/webslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 19:12:19.000000 webslides-0.5.6/webslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-16 19:12:19.000000 webslides-0.5.6/webslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-16 19:12:19.000000 webslides-0.5.6/webslides.egg-info/top_level.txt
```

### Comparing `webslides-0.5.5/PKG-INFO` & `webslides-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webslides
-Version: 0.5.5
+Version: 0.5.6
 Summary: Creates powerpoint like slides in HTML format. Including title page, index page and page navigation.
 Home-page: UNKNOWN
 Author: Derk-Jan Woltjer
 Author-email: derkjan.woltjer@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `webslides-0.5.5/README.md` & `webslides-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `webslides-0.5.5/setup.py` & `webslides-0.5.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="webslides",
-    version="0.5.5",
+    version="0.5.6",
     author="Derk-Jan Woltjer",
     author_email="derkjan.woltjer@gmail.com",
     description="Creates powerpoint like slides in HTML format. Including title page, index page and page navigation.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     licence="MIT License",
     packages=find_packages(),
```

### Comparing `webslides-0.5.5/webslides/main.py` & `webslides-0.5.6/webslides/main.py`

 * *Files identical despite different names*

### Comparing `webslides-0.5.5/webslides/modules/demo.py` & `webslides-0.5.6/webslides/modules/demo.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,9 +194,8 @@
            , open_in_browser=True
            , show_index_page=True
            , show_highlights_page=True
            , show_highlights_only=False)
 
     return None
 
-
-demo()
+# demo()
```

### Comparing `webslides-0.5.5/webslides/modules/generate.py` & `webslides-0.5.6/webslides/modules/generate.py`

 * *Files identical despite different names*

### Comparing `webslides-0.5.5/webslides/modules/hello_world.py` & `webslides-0.5.6/webslides/modules/hello_world.py`

 * *Files identical despite different names*

### Comparing `webslides-0.5.5/webslides/modules/input_validations.py` & `webslides-0.5.6/webslides/modules/input_validations.py`

 * *Files identical despite different names*

### Comparing `webslides-0.5.5/webslides/modules/other.py` & `webslides-0.5.6/webslides/modules/other.py`

 * *Files identical despite different names*

### Comparing `webslides-0.5.5/webslides/modules/pagination.py` & `webslides-0.5.6/webslides/modules/pagination.py`

 * *Files identical despite different names*

### Comparing `webslides-0.5.5/webslides/modules/tohtml.py` & `webslides-0.5.6/webslides/modules/tohtml.py`

 * *Files identical despite different names*

### Comparing `webslides-0.5.5/webslides.egg-info/PKG-INFO` & `webslides-0.5.6/webslides.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webslides
-Version: 0.5.5
+Version: 0.5.6
 Summary: Creates powerpoint like slides in HTML format. Including title page, index page and page navigation.
 Home-page: UNKNOWN
 Author: Derk-Jan Woltjer
 Author-email: derkjan.woltjer@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

