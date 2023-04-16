# Comparing `tmp/searchlix-1.0.5.tar.gz` & `tmp/searchlix-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\searchlix-1.0.5.tar", last modified: Sat Apr 15 19:50:02 2023, max compression
+gzip compressed data, was "dist\searchlix-1.0.6.tar", last modified: Sat Apr 15 19:59:08 2023, max compression
```

## Comparing `searchlix-1.0.5.tar` & `searchlix-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 19:50:02.000000 searchlix-1.0.5/
--rw-rw-rw-   0        0        0     2465 2023-04-15 19:50:02.000000 searchlix-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1545 2023-04-15 19:49:33.000000 searchlix-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 19:50:02.000000 searchlix-1.0.5/searchlix/
--rw-rw-rw-   0        0        0        0 2023-04-14 00:19:50.000000 searchlix-1.0.5/searchlix/__init__.py
--rw-rw-rw-   0        0        0     3559 2023-04-15 19:48:19.000000 searchlix-1.0.5/searchlix/searchlix.py
-drwxrwxrwx   0        0        0        0 2023-04-15 19:50:02.000000 searchlix-1.0.5/searchlix.egg-info/
--rw-rw-rw-   0        0        0     2465 2023-04-15 19:50:02.000000 searchlix-1.0.5/searchlix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-04-15 19:50:02.000000 searchlix-1.0.5/searchlix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 19:50:02.000000 searchlix-1.0.5/searchlix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-15 19:50:02.000000 searchlix-1.0.5/searchlix.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-15 19:50:02.000000 searchlix-1.0.5/searchlix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 19:50:02.000000 searchlix-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      662 2023-04-15 19:49:39.000000 searchlix-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:59:08.000000 searchlix-1.0.6/
+-rw-rw-rw-   0        0        0     2479 2023-04-15 19:59:08.000000 searchlix-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1559 2023-04-15 19:58:47.000000 searchlix-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 19:59:08.000000 searchlix-1.0.6/searchlix/
+-rw-rw-rw-   0        0        0        0 2023-04-14 00:19:50.000000 searchlix-1.0.6/searchlix/__init__.py
+-rw-rw-rw-   0        0        0     3559 2023-04-15 19:48:19.000000 searchlix-1.0.6/searchlix/searchlix.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:59:08.000000 searchlix-1.0.6/searchlix.egg-info/
+-rw-rw-rw-   0        0        0     2479 2023-04-15 19:59:07.000000 searchlix-1.0.6/searchlix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-04-15 19:59:08.000000 searchlix-1.0.6/searchlix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 19:59:07.000000 searchlix-1.0.6/searchlix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-15 19:59:07.000000 searchlix-1.0.6/searchlix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-15 19:59:08.000000 searchlix-1.0.6/searchlix.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 19:59:08.000000 searchlix-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      690 2023-04-15 19:58:17.000000 searchlix-1.0.6/setup.py
```

### Comparing `searchlix-1.0.5/PKG-INFO` & `searchlix-1.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchlix
-Version: 1.0.5
+Version: 1.0.6
 Summary: A package for extract data from websites and text
 Home-page: UNKNOWN
 Author: Hashem
 Author-email: hashem.a.muhammad@gmail.com
 License: UNKNOWN
 Description: # Searchlix
         ## _powerful python pakage to search in text and websites_
@@ -12,20 +12,20 @@
         
         
         ## Features
         
         - Search for page name in website
         - Extract emails from website page
         - Extract phone number from website page
-        - check if domain has a valid mail server
-        - check if domain is valid
+        - check if a domain has a valid mail server
+        - check if a domain is valid
         - Pattern search in text
         - Search for word in text
-        - Extract phone number in text / Phone number validation
-        - Extract emails in text / Email validation
+        - Extract a phone number from a text / Phone number validation
+        - Extract emails from a text / Email validation
         
         
         
         
         
         
         ## Installation
```

### Comparing `searchlix-1.0.5/README.md` & `searchlix-1.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 
 ## Features
 
 - Search for page name in website
 - Extract emails from website page
 - Extract phone number from website page
-- check if domain has a valid mail server
-- check if domain is valid
+- check if a domain has a valid mail server
+- check if a domain is valid
 - Pattern search in text
 - Search for word in text
-- Extract phone number in text / Phone number validation
-- Extract emails in text / Email validation
+- Extract a phone number from a text / Phone number validation
+- Extract emails from a text / Email validation
 
 
 
 
 
 
 ## Installation
```

### Comparing `searchlix-1.0.5/searchlix/searchlix.py` & `searchlix-1.0.6/searchlix/searchlix.py`

 * *Files identical despite different names*

### Comparing `searchlix-1.0.5/searchlix.egg-info/PKG-INFO` & `searchlix-1.0.6/searchlix.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchlix
-Version: 1.0.5
+Version: 1.0.6
 Summary: A package for extract data from websites and text
 Home-page: UNKNOWN
 Author: Hashem
 Author-email: hashem.a.muhammad@gmail.com
 License: UNKNOWN
 Description: # Searchlix
         ## _powerful python pakage to search in text and websites_
@@ -12,20 +12,20 @@
         
         
         ## Features
         
         - Search for page name in website
         - Extract emails from website page
         - Extract phone number from website page
-        - check if domain has a valid mail server
-        - check if domain is valid
+        - check if a domain has a valid mail server
+        - check if a domain is valid
         - Pattern search in text
         - Search for word in text
-        - Extract phone number in text / Phone number validation
-        - Extract emails in text / Email validation
+        - Extract a phone number from a text / Phone number validation
+        - Extract emails from a text / Email validation
         
         
         
         
         
         
         ## Installation
```

