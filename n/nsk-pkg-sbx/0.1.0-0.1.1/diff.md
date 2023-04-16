# Comparing `tmp/nsk_pkg_sbx-0.1.0.tar.gz` & `tmp/nsk_pkg_sbx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsk_pkg_sbx-0.1.0.tar", max compression
+gzip compressed data, was "nsk_pkg_sbx-0.1.1.tar", max compression
```

## Comparing `nsk_pkg_sbx-0.1.0.tar` & `nsk_pkg_sbx-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-04-16 21:20:28.857783 nsk_pkg_sbx-0.1.0/LICENSE
--rw-r--r--   0        0        0       28 2023-04-16 21:20:28.857783 nsk_pkg_sbx-0.1.0/README.md
--rw-r--r--   0        0        0      425 2023-04-16 21:26:05.724448 nsk_pkg_sbx-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-16 21:21:02.081455 nsk_pkg_sbx-0.1.0/sbx/__init__.py
--rw-r--r--   0        0        0      157 2023-04-16 21:28:14.682345 nsk_pkg_sbx-0.1.0/sbx/cli.py
--rw-r--r--   0        0        0       72 2023-04-16 21:25:41.660883 nsk_pkg_sbx-0.1.0/sbx/hello.py
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 nsk_pkg_sbx-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-16 21:20:28.857783 nsk_pkg_sbx-0.1.1/LICENSE
+-rw-r--r--   0        0        0       28 2023-04-16 21:20:28.857783 nsk_pkg_sbx-0.1.1/README.md
+-rw-r--r--   0        0        0      425 2023-04-16 21:55:31.705509 nsk_pkg_sbx-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-16 21:21:02.081455 nsk_pkg_sbx-0.1.1/sbx/__init__.py
+-rw-r--r--   0        0        0      157 2023-04-16 21:28:14.682345 nsk_pkg_sbx-0.1.1/sbx/cli.py
+-rw-r--r--   0        0        0       72 2023-04-16 21:25:41.660883 nsk_pkg_sbx-0.1.1/sbx/hello.py
+-rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 nsk_pkg_sbx-0.1.1/PKG-INFO
```

### Comparing `nsk_pkg_sbx-0.1.0/LICENSE` & `nsk_pkg_sbx-0.1.1/LICENSE`

 * *Files identical despite different names*

