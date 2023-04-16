# Comparing `tmp/email_validator-2.0.0.dev3.tar.gz` & `tmp/email_validator-2.0.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "email_validator-2.0.0.dev3.tar", last modified: Fri Mar 10 18:17:18 2023, max compression
+gzip compressed data, was "email_validator-2.0.0.dev4.tar", last modified: Mon Mar 13 12:56:33 2023, max compression
```

## Comparing `email_validator-2.0.0.dev3.tar` & `email_validator-2.0.0.dev4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-10 18:17:18.958727 email_validator-2.0.0.dev3/
--rw-rw-r--   0 user      (1000) user      (1000)     7048 2021-11-17 12:22:14.000000 email_validator-2.0.0.dev3/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       53 2021-11-17 12:22:14.000000 email_validator-2.0.0.dev3/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)    22815 2023-03-10 18:17:18.962727 email_validator-2.0.0.dev3/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    21857 2023-03-10 16:29:14.000000 email_validator-2.0.0.dev3/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-10 18:17:18.958727 email_validator-2.0.0.dev3/email_validator/
--rw-rw-r--   0 user      (1000) user      (1000)     3887 2023-02-04 18:41:25.000000 email_validator-2.0.0.dev3/email_validator/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1516 2023-03-10 16:29:14.000000 email_validator-2.0.0.dev3/email_validator/__main__.py
--rw-rw-r--   0 user      (1000) user      (1000)     5749 2023-03-10 16:29:23.000000 email_validator-2.0.0.dev3/email_validator/deliverability.py
--rw-rw-r--   0 user      (1000) user      (1000)     4992 2023-03-10 16:29:23.000000 email_validator-2.0.0.dev3/email_validator/exceptions_types.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-03-10 16:29:23.000000 email_validator-2.0.0.dev3/email_validator/py.typed
--rw-rw-r--   0 user      (1000) user      (1000)     1802 2023-03-10 16:29:14.000000 email_validator-2.0.0.dev3/email_validator/rfc_constants.py
--rw-rw-r--   0 user      (1000) user      (1000)    17571 2023-03-10 16:29:23.000000 email_validator-2.0.0.dev3/email_validator/syntax.py
--rw-rw-r--   0 user      (1000) user      (1000)     6201 2023-03-10 16:29:23.000000 email_validator-2.0.0.dev3/email_validator/validate_email.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-10 18:17:18.958727 email_validator-2.0.0.dev3/email_validator.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    22815 2023-03-10 18:17:18.000000 email_validator-2.0.0.dev3/email_validator.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      543 2023-03-10 18:17:18.000000 email_validator-2.0.0.dev3/email_validator.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-03-10 18:17:18.000000 email_validator-2.0.0.dev3/email_validator.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       57 2023-03-10 18:17:18.000000 email_validator-2.0.0.dev3/email_validator.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       29 2023-03-10 18:17:18.000000 email_validator-2.0.0.dev3/email_validator.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       16 2023-03-10 18:17:18.000000 email_validator-2.0.0.dev3/email_validator.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       96 2023-02-04 18:50:03.000000 email_validator-2.0.0.dev3/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)     1367 2023-03-10 18:17:18.962727 email_validator-2.0.0.dev3/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)       37 2021-11-17 12:22:14.000000 email_validator-2.0.0.dev3/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-13 12:56:33.965168 email_validator-2.0.0.dev4/
+-rw-rw-r--   0 user      (1000) user      (1000)     7048 2021-11-17 12:22:14.000000 email_validator-2.0.0.dev4/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       53 2021-11-17 12:22:14.000000 email_validator-2.0.0.dev4/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)    22815 2023-03-13 12:56:33.965168 email_validator-2.0.0.dev4/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    21857 2023-03-10 16:29:14.000000 email_validator-2.0.0.dev4/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-13 12:56:33.961168 email_validator-2.0.0.dev4/email_validator/
+-rw-rw-r--   0 user      (1000) user      (1000)     4133 2023-03-13 12:54:36.000000 email_validator-2.0.0.dev4/email_validator/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1516 2023-03-10 16:29:14.000000 email_validator-2.0.0.dev4/email_validator/__main__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5749 2023-03-10 16:29:23.000000 email_validator-2.0.0.dev4/email_validator/deliverability.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4835 2023-03-13 12:53:03.000000 email_validator-2.0.0.dev4/email_validator/exceptions_types.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-03-10 16:29:23.000000 email_validator-2.0.0.dev4/email_validator/py.typed
+-rw-rw-r--   0 user      (1000) user      (1000)     1802 2023-03-10 16:29:14.000000 email_validator-2.0.0.dev4/email_validator/rfc_constants.py
+-rw-rw-r--   0 user      (1000) user      (1000)    17571 2023-03-10 16:29:23.000000 email_validator-2.0.0.dev4/email_validator/syntax.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6201 2023-03-10 16:29:23.000000 email_validator-2.0.0.dev4/email_validator/validate_email.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-13 12:56:33.965168 email_validator-2.0.0.dev4/email_validator.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    22815 2023-03-13 12:56:33.000000 email_validator-2.0.0.dev4/email_validator.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      543 2023-03-13 12:56:33.000000 email_validator-2.0.0.dev4/email_validator.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-03-13 12:56:33.000000 email_validator-2.0.0.dev4/email_validator.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       57 2023-03-13 12:56:33.000000 email_validator-2.0.0.dev4/email_validator.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       29 2023-03-13 12:56:33.000000 email_validator-2.0.0.dev4/email_validator.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       16 2023-03-13 12:56:33.000000 email_validator-2.0.0.dev4/email_validator.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       96 2023-02-04 18:50:03.000000 email_validator-2.0.0.dev4/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)     1367 2023-03-13 12:56:33.965168 email_validator-2.0.0.dev4/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)       37 2021-11-17 12:22:14.000000 email_validator-2.0.0.dev4/setup.py
```

### Comparing `email_validator-2.0.0.dev3/LICENSE` & `email_validator-2.0.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `email_validator-2.0.0.dev3/PKG-INFO` & `email_validator-2.0.0.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: email_validator
-Version: 2.0.0.dev3
+Version: 2.0.0.dev4
 Summary: A robust email address syntax and deliverability validation library.
 Home-page: https://github.com/JoshData/python-email-validator
 Author: Joshua Tauberer
 Author-email: jt@occams.info
 License: CC0 (copyright waived)
 Keywords: email address validator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `email_validator-2.0.0.dev3/README.md` & `email_validator-2.0.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `email_validator-2.0.0.dev3/email_validator/__init__.py` & `email_validator-2.0.0.dev4/email_validator/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 # -*- coding: utf-8 -*-
 
 # Export the main method, helper methods, and the public data types.
-from .exceptions_types import *  # noqa: F401,F403
-from .validate_email import validate_email  # noqa: F401
+from .exceptions_types import ValidatedEmail, EmailNotValidError, \
+                              EmailSyntaxError, EmailUndeliverableError
+from .validate_email import validate_email
+
+
+__all__ = ["validate_email",
+           "ValidatedEmail", "EmailNotValidError",
+           "EmailSyntaxError", "EmailUndeliverableError",
+           "caching_resolver"]
 
 
 def caching_resolver(*args, **kwargs):
     # Lazy load `deliverability` as it is slow to import (due to dns.resolver)
     from .deliverability import caching_resolver
 
     return caching_resolver(*args, **kwargs)
```

### Comparing `email_validator-2.0.0.dev3/email_validator/__main__.py` & `email_validator-2.0.0.dev4/email_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `email_validator-2.0.0.dev3/email_validator/deliverability.py` & `email_validator-2.0.0.dev4/email_validator/deliverability.py`

 * *Files identical despite different names*

### Comparing `email_validator-2.0.0.dev3/email_validator/exceptions_types.py` & `email_validator-2.0.0.dev4/email_validator/exceptions_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,18 +59,14 @@
     mx_fallback_type: str
 
     """Tests use this constructor."""
     def __init__(self, **kwargs):
         for k, v in kwargs.items():
             setattr(self, k, v)
 
-    """As a convenience, str(...) on instances of this class return the normalized address."""
-    def __self__(self):
-        return self.normalized_email
-
     def __repr__(self):
         return f"<ValidatedEmail {self.email}>"
 
     """For backwards compatibility, some fields are also exposed through a dict-like interface. Note
     that some of the names changed when they became attributes."""
     def __getitem__(self, key):
         if key == "email":
```

### Comparing `email_validator-2.0.0.dev3/email_validator/rfc_constants.py` & `email_validator-2.0.0.dev4/email_validator/rfc_constants.py`

 * *Files identical despite different names*

### Comparing `email_validator-2.0.0.dev3/email_validator/syntax.py` & `email_validator-2.0.0.dev4/email_validator/syntax.py`

 * *Files identical despite different names*

### Comparing `email_validator-2.0.0.dev3/email_validator/validate_email.py` & `email_validator-2.0.0.dev4/email_validator/validate_email.py`

 * *Files identical despite different names*

### Comparing `email_validator-2.0.0.dev3/email_validator.egg-info/PKG-INFO` & `email_validator-2.0.0.dev4/email_validator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: email-validator
-Version: 2.0.0.dev3
+Version: 2.0.0.dev4
 Summary: A robust email address syntax and deliverability validation library.
 Home-page: https://github.com/JoshData/python-email-validator
 Author: Joshua Tauberer
 Author-email: jt@occams.info
 License: CC0 (copyright waived)
 Keywords: email address validator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `email_validator-2.0.0.dev3/email_validator.egg-info/SOURCES.txt` & `email_validator-2.0.0.dev4/email_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `email_validator-2.0.0.dev3/setup.cfg` & `email_validator-2.0.0.dev4/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = email_validator
-version = 2.0.0-dev3
+version = 2.0.0-dev4
 description = A robust email address syntax and deliverability validation library.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/JoshData/python-email-validator
 author = Joshua Tauberer
 author_email = jt@occams.info
 license = CC0 (copyright waived)
```

