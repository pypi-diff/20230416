# Comparing `tmp/pysymbolcheck-2.7.4.tar.gz` & `tmp/pysymbolcheck-2.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysymbolcheck-2.7.4.tar", last modified: Wed Mar 15 07:09:26 2023, max compression
+gzip compressed data, was "pysymbolcheck-2.7.5.tar", last modified: Sun Apr 16 10:13:31 2023, max compression
```

## Comparing `pysymbolcheck-2.7.4.tar` & `pysymbolcheck-2.7.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:09:26.043810 pysymbolcheck-2.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-03-15 07:09:11.000000 pysymbolcheck-2.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-15 07:09:11.000000 pysymbolcheck-2.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-03-15 07:09:26.043810 pysymbolcheck-2.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-03-15 07:09:11.000000 pysymbolcheck-2.7.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-03-15 07:09:11.000000 pysymbolcheck-2.7.4/basic_rules.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:09:26.043810 pysymbolcheck-2.7.4/pysymbolcheck/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 07:09:11.000000 pysymbolcheck-2.7.4/pysymbolcheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-03-15 07:09:11.000000 pysymbolcheck-2.7.4/pysymbolcheck/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:09:26.043810 pysymbolcheck-2.7.4/pysymbolcheck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-03-15 07:09:26.000000 pysymbolcheck-2.7.4/pysymbolcheck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-15 07:09:26.000000 pysymbolcheck-2.7.4/pysymbolcheck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 07:09:26.000000 pysymbolcheck-2.7.4/pysymbolcheck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-15 07:09:26.000000 pysymbolcheck-2.7.4/pysymbolcheck.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-15 07:09:26.000000 pysymbolcheck-2.7.4/pysymbolcheck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-15 07:09:26.000000 pysymbolcheck-2.7.4/pysymbolcheck.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-15 07:09:11.000000 pysymbolcheck-2.7.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-15 07:09:26.047809 pysymbolcheck-2.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-03-15 07:09:25.000000 pysymbolcheck-2.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:13:31.227715 pysymbolcheck-2.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-16 10:13:18.000000 pysymbolcheck-2.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-16 10:13:18.000000 pysymbolcheck-2.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-16 10:13:31.227715 pysymbolcheck-2.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-16 10:13:18.000000 pysymbolcheck-2.7.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-16 10:13:18.000000 pysymbolcheck-2.7.5/basic_rules.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:13:31.227715 pysymbolcheck-2.7.5/pysymbolcheck/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 10:13:18.000000 pysymbolcheck-2.7.5/pysymbolcheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-04-16 10:13:18.000000 pysymbolcheck-2.7.5/pysymbolcheck/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:13:31.227715 pysymbolcheck-2.7.5/pysymbolcheck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-16 10:13:31.000000 pysymbolcheck-2.7.5/pysymbolcheck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-16 10:13:31.000000 pysymbolcheck-2.7.5/pysymbolcheck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 10:13:31.000000 pysymbolcheck-2.7.5/pysymbolcheck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-16 10:13:31.000000 pysymbolcheck-2.7.5/pysymbolcheck.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-16 10:13:31.000000 pysymbolcheck-2.7.5/pysymbolcheck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-16 10:13:31.000000 pysymbolcheck-2.7.5/pysymbolcheck.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-16 10:13:18.000000 pysymbolcheck-2.7.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-16 10:13:31.227715 pysymbolcheck-2.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-16 10:13:30.000000 pysymbolcheck-2.7.5/setup.py
```

### Comparing `pysymbolcheck-2.7.4/LICENSE` & `pysymbolcheck-2.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pysymbolcheck-2.7.4/PKG-INFO` & `pysymbolcheck-2.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysymbolcheck
-Version: 2.7.4
+Version: 2.7.5
 Summary: ELF symbol check
 Home-page: https://github.com/priv-kweihmann/pysymcheck
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pysymbolcheck-2.7.4/README.md` & `pysymbolcheck-2.7.5/README.md`

 * *Files identical despite different names*

### Comparing `pysymbolcheck-2.7.4/basic_rules.json` & `pysymbolcheck-2.7.5/basic_rules.json`

 * *Files identical despite different names*

### Comparing `pysymbolcheck-2.7.4/pysymbolcheck/__main__.py` & `pysymbolcheck-2.7.5/pysymbolcheck/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         sys.stderr.write(
             "Rule {rule} is not well-formed: {e}\n".format(rule=item["rule"], e=e))
         return False
     return True
 
 
 def eval_rules(rules):
-    return all([parse_rules(x) for x in rules])
+    return all(parse_rules(x) for x in rules)
 
 
 def create_argparses():
     parser = argparse.ArgumentParser(
         description='Eval symbols of a binary against given rules')
     parser.add_argument('rules', help='Path to a rule file')
     parser.add_argument("file", help="File to parse")
```

### Comparing `pysymbolcheck-2.7.4/pysymbolcheck.egg-info/PKG-INFO` & `pysymbolcheck-2.7.5/pysymbolcheck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysymbolcheck
-Version: 2.7.4
+Version: 2.7.5
 Summary: ELF symbol check
 Home-page: https://github.com/priv-kweihmann/pysymcheck
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pysymbolcheck-2.7.4/setup.py` & `pysymbolcheck-2.7.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 requirements = []
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="pysymbolcheck",
-    version="2.7.4",
+    version="2.7.5",
     author="Konrad Weihmann",
     author_email="kweihmann@outlook.com",
     description="ELF symbol check",
     long_description=_long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/priv-kweihmann/pysymcheck",
     packages=setuptools.find_packages(),
```

