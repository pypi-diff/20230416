# Comparing `tmp/triple-quote-clean-1.0.0.tar.gz` & `tmp/triple-quote-clean-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triple-quote-clean-1.0.0.tar", last modified: Sat Apr  8 22:38:29 2023, max compression
+gzip compressed data, was "triple-quote-clean-1.1.0.tar", last modified: Sun Apr 16 12:36:07 2023, max compression
```

## Comparing `triple-quote-clean-1.0.0.tar` & `triple-quote-clean-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 22:38:29.201810 triple-quote-clean-1.0.0/
--rw-rw-rw-   0        0        0     1132 2023-03-26 11:43:35.000000 triple-quote-clean-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     3099 2023-04-08 22:38:29.200810 triple-quote-clean-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2312 2023-04-08 21:59:47.000000 triple-quote-clean-1.0.0/README.md
--rw-rw-rw-   0        0        0      898 2023-04-08 22:37:23.000000 triple-quote-clean-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-08 22:38:29.201810 triple-quote-clean-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-08 22:38:29.145796 triple-quote-clean-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-08 22:38:29.163802 triple-quote-clean-1.0.0/src/triple_quote_clean/
--rw-rw-rw-   0        0        0     1575 2023-03-26 11:43:35.000000 triple-quote-clean-1.0.0/src/triple_quote_clean/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 22:38:29.179806 triple-quote-clean-1.0.0/src/triple_quote_clean.egg-info/
--rw-rw-rw-   0        0        0     3099 2023-04-08 22:38:29.000000 triple-quote-clean-1.0.0/src/triple_quote_clean.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      368 2023-04-08 22:38:29.000000 triple-quote-clean-1.0.0/src/triple_quote_clean.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 22:38:29.000000 triple-quote-clean-1.0.0/src/triple_quote_clean.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-08 22:38:29.000000 triple-quote-clean-1.0.0/src/triple_quote_clean.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-08 22:38:29.196810 triple-quote-clean-1.0.0/tests/
--rw-rw-rw-   0        0        0      456 2023-03-26 11:43:35.000000 triple-quote-clean-1.0.0/tests/test_exponent.py
--rw-rw-rw-   0        0        0      517 2023-03-26 11:43:35.000000 triple-quote-clean-1.0.0/tests/test_guide_character.py
--rw-rw-rw-   0        0        0      399 2023-03-26 11:43:35.000000 triple-quote-clean-1.0.0/tests/test_query.py
--rw-rw-rw-   0        0        0      328 2023-03-26 11:43:35.000000 triple-quote-clean-1.0.0/tests/test_rshift.py
--rw-rw-rw-   0        0        0      533 2023-03-26 11:43:35.000000 triple-quote-clean-1.0.0/tests/test_tabs.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:36:07.293804 triple-quote-clean-1.1.0/
+-rw-rw-rw-   0        0        0     1132 2023-04-16 11:43:01.000000 triple-quote-clean-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     3894 2023-04-16 12:36:07.292804 triple-quote-clean-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3151 2023-04-16 12:31:51.000000 triple-quote-clean-1.1.0/README.md
+-rw-rw-rw-   0        0        0      875 2023-04-16 12:34:36.000000 triple-quote-clean-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 12:36:07.294799 triple-quote-clean-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 12:36:07.233137 triple-quote-clean-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 12:36:07.257787 triple-quote-clean-1.1.0/src/triple_quote_clean/
+-rw-rw-rw-   0        0        0      171 2023-04-16 12:22:53.000000 triple-quote-clean-1.1.0/src/triple_quote_clean/__init__.py
+-rw-rw-rw-   0        0        0      757 2023-04-16 12:26:22.000000 triple-quote-clean-1.1.0/src/triple_quote_clean/_jinja_pipe.py
+-rw-rw-rw-   0        0        0      937 2023-04-16 11:51:07.000000 triple-quote-clean-1.1.0/src/triple_quote_clean/_pipe.py
+-rw-rw-rw-   0        0        0      919 2023-04-16 11:46:39.000000 triple-quote-clean-1.1.0/src/triple_quote_clean/_triple_quote_clean.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:36:07.273791 triple-quote-clean-1.1.0/src/triple_quote_clean.egg-info/
+-rw-rw-rw-   0        0        0     3894 2023-04-16 12:36:07.000000 triple-quote-clean-1.1.0/src/triple_quote_clean.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      529 2023-04-16 12:36:07.000000 triple-quote-clean-1.1.0/src/triple_quote_clean.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 12:36:07.000000 triple-quote-clean-1.1.0/src/triple_quote_clean.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-16 12:36:07.000000 triple-quote-clean-1.1.0/src/triple_quote_clean.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-16 12:36:07.000000 triple-quote-clean-1.1.0/src/triple_quote_clean.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 12:36:07.288797 triple-quote-clean-1.1.0/tests/
+-rw-rw-rw-   0        0        0      456 2023-04-16 11:43:01.000000 triple-quote-clean-1.1.0/tests/test_exponent.py
+-rw-rw-rw-   0        0        0      517 2023-04-16 11:43:01.000000 triple-quote-clean-1.1.0/tests/test_guide_character.py
+-rw-rw-rw-   0        0        0      399 2023-04-16 11:43:01.000000 triple-quote-clean-1.1.0/tests/test_query.py
+-rw-rw-rw-   0        0        0      328 2023-04-16 11:43:01.000000 triple-quote-clean-1.1.0/tests/test_rshift.py
+-rw-rw-rw-   0        0        0      533 2023-04-16 11:43:01.000000 triple-quote-clean-1.1.0/tests/test_tabs.py
```

### Comparing `triple-quote-clean-1.0.0/LICENSE.txt` & `triple-quote-clean-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `triple-quote-clean-1.0.0/PKG-INFO` & `triple-quote-clean-1.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,16 @@
-Metadata-Version: 2.1
-Name: triple-quote-clean
-Version: 1.0.0
-Summary: clean up triple quotes
-Author-email: Chris <chrisam1993@live.com>
-Project-URL: Homepage, https://github.com/Chr1sC0de/triple-quote-clean
-Project-URL: Bug Tracker, https://github.com/Chr1sC0de/triple-quote-clean/issues
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # triple-quote-clean
 
+- [triple-quote-clean](#triple-quote-clean)
+  - [Usage](#usage)
+    - [Basic Usage](#basic-usage)
+    - [Indentation](#indentation)
+    - [Guide Characters](#guide-characters)
+    - [Jinja Pipe](#jinja-pipe)
+
 TripleQuoteCleaner is a Python class that can be used to clean triple-quoted
 strings in a variety of ways. It's designed to be used in cases where you want
 to remove extraneous whitespace and/or add indentation to a triple-quoted
 string. This is useful when dealing with extensions/code that require some
 extraneous metadata in the string.
 
 To use TripleQuoteCleaner, simply import it into your Python script:
@@ -101,7 +89,45 @@
 In this example, tqc.guide_character is set to "$$" so that the 4 beginning
 spaces will be maintained . The output of this code will be:
 
 ```sql
     select *
     from some_database
 ```
+
+### Jinja Pipe
+
+A jinja pipe is a simple wrapper over a jinja string render. For example
+
+```python
+tqc = TripleQuoteCleaner(skip_top_lines=1)
+ (
+    JinjaPipe(columns=["hello", "these", "are", "some", "columns"])
+    << tqc
+    ** """--sql
+    select
+    {% for item in columns %}
+        {% if loop.last%}
+            nvl({{item}}, -1)
+        {% else %}
+            nvl({{item}}, -1),
+        {% endif %}
+    {% endfor %}
+    from
+        some.table
+    """
+)
+```
+
+will produce
+
+```sql
+select
+    hello,
+    these,
+    are,
+    some,
+    columns,
+    world
+from
+    some.table
+```
```

### Comparing `triple-quote-clean-1.0.0/pyproject.toml` & `triple-quote-clean-1.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 readme          = "README.md"
 requires-python = ">=3.7"
 keywords        = []
 authors         = [
   { name = "Chris", email = "chrisam1993@live.com" },
 ]
 classifiers = [
-  "Development Status :: 4 - Beta",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
-dependencies = []
-version = "1.0.0"
+dependencies = [
+  "jinja2"
+]
+version = "1.1.0"
 
 [project.urls]
 "Homepage" = "https://github.com/Chr1sC0de/triple-quote-clean"
 "Bug Tracker" = "https://github.com/Chr1sC0de/triple-quote-clean/issues"
```

### Comparing `triple-quote-clean-1.0.0/tests/test_guide_character.py` & `triple-quote-clean-1.1.0/tests/test_guide_character.py`

 * *Files identical despite different names*

### Comparing `triple-quote-clean-1.0.0/tests/test_tabs.py` & `triple-quote-clean-1.1.0/tests/test_tabs.py`

 * *Files identical despite different names*

