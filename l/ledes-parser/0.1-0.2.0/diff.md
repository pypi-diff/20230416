# Comparing `tmp/ledes-parser-0.1.tar.gz` & `tmp/ledes-parser-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ledes-parser-0.1.tar", last modified: Sun Apr 16 00:00:29 2023, max compression
+gzip compressed data, was "ledes-parser-0.2.0.tar", last modified: Sun Apr 16 01:57:17 2023, max compression
```

## Comparing `ledes-parser-0.1.tar` & `ledes-parser-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 00:00:29.027109 ledes-parser-0.1/
--rw-rw-rw-   0        0        0     1091 2023-04-15 23:55:26.000000 ledes-parser-0.1/LICENSE
--rw-rw-rw-   0        0        0      300 2023-04-16 00:00:29.003105 ledes-parser-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       58 2023-04-15 23:55:26.000000 ledes-parser-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 00:00:28.991106 ledes-parser-0.1/ledes-parser/
--rw-rw-rw-   0        0        0        0 2023-04-15 23:47:09.000000 ledes-parser-0.1/ledes-parser/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-15 23:47:20.000000 ledes-parser-0.1/ledes-parser/ledes_1998_parser.py
-drwxrwxrwx   0        0        0        0 2023-04-16 00:00:28.998105 ledes-parser-0.1/ledes_parser.egg-info/
--rw-rw-rw-   0        0        0      300 2023-04-16 00:00:28.000000 ledes-parser-0.1/ledes_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-04-16 00:00:28.000000 ledes-parser-0.1/ledes_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 00:00:28.000000 ledes-parser-0.1/ledes_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-16 00:00:28.000000 ledes-parser-0.1/ledes_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 00:00:29.028104 ledes-parser-0.1/setup.cfg
--rw-rw-rw-   0        0        0      406 2023-04-15 23:50:05.000000 ledes-parser-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 00:00:29.001107 ledes-parser-0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-04-15 23:47:44.000000 ledes-parser-0.1/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-15 23:47:37.000000 ledes-parser-0.1/tests/test_ledes_1998_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 01:57:17.075103 ledes-parser-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-16 01:57:01.000000 ledes-parser-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-16 01:57:17.075103 ledes-parser-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-16 01:57:01.000000 ledes-parser-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 01:57:17.071103 ledes-parser-0.2.0/ledes_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-16 01:57:17.000000 ledes-parser-0.2.0/ledes_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-16 01:57:17.000000 ledes-parser-0.2.0/ledes_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 01:57:17.000000 ledes-parser-0.2.0/ledes_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-16 01:57:17.000000 ledes-parser-0.2.0/ledes_parser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 01:57:17.075103 ledes-parser-0.2.0/ledes_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-16 01:57:01.000000 ledes-parser-0.2.0/ledes_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-16 01:57:01.000000 ledes-parser-0.2.0/ledes_parsers/base_ledes_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-16 01:57:01.000000 ledes-parser-0.2.0/ledes_parsers/ledes_1998BI_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-16 01:57:01.000000 ledes-parser-0.2.0/ledes_parsers/ledes_1998B_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-16 01:57:01.000000 ledes-parser-0.2.0/ledes_parsers/ledes_1998_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-16 01:57:01.000000 ledes-parser-0.2.0/ledes_parsers/ledes_dynamic_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 01:57:17.075103 ledes-parser-0.2.0/ledes_parsers/typings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 01:57:01.000000 ledes-parser-0.2.0/ledes_parsers/typings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-16 01:57:01.000000 ledes-parser-0.2.0/ledes_parsers/typings/invoice_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 01:57:17.075103 ledes-parser-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-16 01:57:01.000000 ledes-parser-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 01:57:17.075103 ledes-parser-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 01:57:01.000000 ledes-parser-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-16 01:57:01.000000 ledes-parser-0.2.0/tests/test_ledes_1998_parser.py
```

