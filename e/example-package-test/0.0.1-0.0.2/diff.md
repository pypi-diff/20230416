# Comparing `tmp/example_package_test-0.0.1.tar.gz` & `tmp/example_package_test-0.0.2.tar.gz`

## Comparing `example_package_test-0.0.1.tar` & `example_package_test-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 example_package_test-0.0.1/src/example_package_test/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 example_package_test-0.0.1/src/example_package_test/example.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 example_package_test-0.0.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 example_package_test-0.0.1/LICENSE
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 example_package_test-0.0.1/README.md
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 example_package_test-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 example_package_test-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 example_package_test-0.0.2/.DS_Store
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 example_package_test-0.0.2/requirements.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 example_package_test-0.0.2/src/example_package_test/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 example_package_test-0.0.2/src/example_package_test/example.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 example_package_test-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 example_package_test-0.0.2/LICENSE
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 example_package_test-0.0.2/README.md
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 example_package_test-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 example_package_test-0.0.2/PKG-INFO
```

### Comparing `example_package_test-0.0.1/LICENSE` & `example_package_test-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `example_package_test-0.0.1/PKG-INFO` & `example_package_test-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: example_package_test
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Author-email: test <author@example.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

