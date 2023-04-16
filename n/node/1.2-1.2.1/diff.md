# Comparing `tmp/node-1.2.tar.gz` & `tmp/node-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "node-1.2.tar", last modified: Mon Dec  5 11:50:58 2022, max compression
+gzip compressed data, was "node-1.2.1.tar", last modified: Sun Apr 16 06:07:46 2023, max compression
```

## Comparing `node-1.2.tar` & `node-1.2.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 11:50:58.543705 node-1.2/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    17586 2022-12-05 11:50:58.000000 node-1.2/CHANGES.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1378 2022-12-05 11:50:58.000000 node-1.2/LICENSE.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       64 2022-12-05 11:50:58.000000 node-1.2/MANIFEST.in
--rw-r--r--   0 rnix      (1000) rnix      (1000)    47605 2022-12-05 11:50:58.543705 node-1.2/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)    17494 2022-12-05 11:50:58.000000 node-1.2/README.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       74 2022-12-05 11:50:58.543705 node-1.2/setup.cfg
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1616 2022-12-05 11:50:58.000000 node-1.2/setup.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 11:50:58.535705 node-1.2/src/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 11:50:58.539705 node-1.2/src/node/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       76 2022-12-05 11:50:58.000000 node-1.2/src/node/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2172 2022-12-05 11:50:58.000000 node-1.2/src/node/base.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 11:50:58.539705 node-1.2/src/node/behaviors/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3893 2022-12-05 11:50:58.000000 node-1.2/src/node/behaviors/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1854 2022-12-05 11:50:58.000000 node-1.2/src/node/behaviors/adopt.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4559 2022-12-05 11:50:58.000000 node-1.2/src/node/behaviors/alias.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2230 2022-12-05 11:50:58.000000 node-1.2/src/node/behaviors/attributes.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3108 2022-12-05 11:50:58.000000 node-1.2/src/node/behaviors/cache.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2193 2022-12-05 11:50:58.000000 node-1.2/src/node/behaviors/common.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2213 2022-12-05 11:50:58.000000 node-1.2/src/node/behaviors/constraints.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1528 2022-12-05 11:50:58.000000 node-1.2/src/node/behaviors/context.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     9895 2022-12-05 11:50:58.000000 node-1.2/src/node/behaviors/events.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6371 2022-12-05 11:50:58.000000 node-1.2/src/node/behaviors/factories.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1979 2022-12-05 11:50:58.000000 node-1.2/src/node/behaviors/fallback.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      767 2022-12-05 11:50:58.000000 node-1.2/src/node/behaviors/filter.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2714 2022-12-05 11:50:58.000000 node-1.2/src/node/behaviors/lifecycle.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6441 2022-12-05 11:50:58.000000 node-1.2/src/node/behaviors/mapping.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4964 2022-12-05 11:50:58.000000 node-1.2/src/node/behaviors/node.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2213 2022-12-05 11:50:58.000000 node-1.2/src/node/behaviors/nodespace.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7223 2022-12-05 11:50:58.000000 node-1.2/src/node/behaviors/order.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6127 2022-12-05 11:50:58.000000 node-1.2/src/node/behaviors/reference.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     9137 2022-12-05 11:50:58.000000 node-1.2/src/node/behaviors/schema.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4009 2022-12-05 11:50:58.000000 node-1.2/src/node/behaviors/sequence.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1939 2022-12-05 11:50:58.000000 node-1.2/src/node/behaviors/storage.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      594 2022-12-05 11:50:58.000000 node-1.2/src/node/compat.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1627 2022-12-05 11:50:58.000000 node-1.2/src/node/events.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    26740 2022-12-05 11:50:58.000000 node-1.2/src/node/interfaces.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      776 2022-12-05 11:50:58.000000 node-1.2/src/node/locking.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 11:50:58.539705 node-1.2/src/node/schema/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1615 2022-12-05 11:50:58.000000 node-1.2/src/node/schema/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    14949 2022-12-05 11:50:58.000000 node-1.2/src/node/schema/fields.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      764 2022-12-05 11:50:58.000000 node-1.2/src/node/schema/scope.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7638 2022-12-05 11:50:58.000000 node-1.2/src/node/schema/serializer.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     9349 2022-12-05 11:50:58.000000 node-1.2/src/node/serializer.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 11:50:58.539705 node-1.2/src/node/testing/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       63 2022-12-05 11:50:58.000000 node-1.2/src/node/testing/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2883 2022-12-05 11:50:58.000000 node-1.2/src/node/testing/base.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      625 2022-12-05 11:50:58.000000 node-1.2/src/node/testing/env.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     9562 2022-12-05 11:50:58.000000 node-1.2/src/node/testing/fullmapping.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      290 2022-12-05 11:50:58.000000 node-1.2/src/node/testing/profiling.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 11:50:58.543705 node-1.2/src/node/tests/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4603 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3656 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_adopt.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6280 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_alias.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2383 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_attributes.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    15962 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_base.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7834 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_cache.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3497 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_common.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3990 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_constraints.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3077 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_context.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    10023 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_events.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6101 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_factories.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7306 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_fallback.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1408 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_filter.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5454 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_lifecycle.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1565 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_locking.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     8647 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_mapping.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2832 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_node.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2302 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_nodespace.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    32587 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_order.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    20996 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_reference.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    31709 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_schema.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6430 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_sequence.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    18662 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_serializer.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3295 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_storage.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    39480 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_testing.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2864 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_tests.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7312 2022-12-05 11:50:58.000000 node-1.2/src/node/tests/test_utils.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     8033 2022-12-05 11:50:58.000000 node-1.2/src/node/utils.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 11:50:58.539705 node-1.2/src/node.egg-info/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    47605 2022-12-05 11:50:58.000000 node-1.2/src/node.egg-info/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2165 2022-12-05 11:50:58.000000 node-1.2/src/node.egg-info/SOURCES.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2022-12-05 11:50:58.000000 node-1.2/src/node.egg-info/dependency_links.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2022-12-05 11:50:58.000000 node-1.2/src/node.egg-info/namespace_packages.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      109 2022-12-05 11:50:58.000000 node-1.2/src/node.egg-info/requires.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2022-12-05 11:50:58.000000 node-1.2/src/node.egg-info/top_level.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2022-12-05 11:50:58.000000 node-1.2/src/node.egg-info/zip-safe
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-04-16 06:07:46.274876 node-1.2.1/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    17717 2023-04-16 06:07:46.000000 node-1.2.1/CHANGES.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1378 2023-04-16 06:07:46.000000 node-1.2.1/LICENSE.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       64 2023-04-16 06:07:46.000000 node-1.2.1/MANIFEST.in
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    37413 2023-04-16 06:07:46.274876 node-1.2.1/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    17494 2023-04-16 06:07:46.000000 node-1.2.1/README.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       74 2023-04-16 06:07:46.274876 node-1.2.1/setup.cfg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1618 2023-04-16 06:07:46.000000 node-1.2.1/setup.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-04-16 06:07:46.270876 node-1.2.1/src/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-04-16 06:07:46.270876 node-1.2.1/src/node/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       76 2023-04-16 06:07:46.000000 node-1.2.1/src/node/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2193 2023-04-16 06:07:46.000000 node-1.2.1/src/node/base.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-04-16 06:07:46.274876 node-1.2.1/src/node/behaviors/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3893 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1854 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/adopt.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4559 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/alias.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2230 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/attributes.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3108 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/cache.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2193 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/common.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2213 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/constraints.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1528 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/context.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     9895 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/events.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6371 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/factories.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1979 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/fallback.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      767 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/filter.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2714 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/lifecycle.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6441 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/mapping.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4964 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/node.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2213 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/nodespace.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7223 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/order.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6127 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/reference.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     9137 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/schema.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4009 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/sequence.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1939 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/storage.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      594 2023-04-16 06:07:46.000000 node-1.2.1/src/node/compat.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1627 2023-04-16 06:07:46.000000 node-1.2.1/src/node/events.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    26740 2023-04-16 06:07:46.000000 node-1.2.1/src/node/interfaces.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      776 2023-04-16 06:07:46.000000 node-1.2.1/src/node/locking.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-04-16 06:07:46.274876 node-1.2.1/src/node/schema/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1615 2023-04-16 06:07:46.000000 node-1.2.1/src/node/schema/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    14949 2023-04-16 06:07:46.000000 node-1.2.1/src/node/schema/fields.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      764 2023-04-16 06:07:46.000000 node-1.2.1/src/node/schema/scope.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7638 2023-04-16 06:07:46.000000 node-1.2.1/src/node/schema/serializer.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     9349 2023-04-16 06:07:46.000000 node-1.2.1/src/node/serializer.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-04-16 06:07:46.274876 node-1.2.1/src/node/testing/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       63 2023-04-16 06:07:46.000000 node-1.2.1/src/node/testing/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2883 2023-04-16 06:07:46.000000 node-1.2.1/src/node/testing/base.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      625 2023-04-16 06:07:46.000000 node-1.2.1/src/node/testing/env.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     9562 2023-04-16 06:07:46.000000 node-1.2.1/src/node/testing/fullmapping.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      290 2023-04-16 06:07:46.000000 node-1.2.1/src/node/testing/profiling.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-04-16 06:07:46.274876 node-1.2.1/src/node/tests/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4603 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3656 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_adopt.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6280 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_alias.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2383 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_attributes.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    15962 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_base.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7834 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_cache.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3497 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_common.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3990 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_constraints.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3077 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_context.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    10023 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_events.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6101 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_factories.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7306 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_fallback.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1408 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_filter.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5454 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_lifecycle.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1565 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_locking.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     8647 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_mapping.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2832 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_node.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2302 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_nodespace.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    32587 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_order.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    20996 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_reference.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    31709 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_schema.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6430 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_sequence.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    18662 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_serializer.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3295 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_storage.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    39480 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_testing.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2864 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_tests.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7312 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_utils.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     8033 2023-04-16 06:07:46.000000 node-1.2.1/src/node/utils.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-04-16 06:07:46.270876 node-1.2.1/src/node.egg-info/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    37413 2023-04-16 06:07:46.000000 node-1.2.1/src/node.egg-info/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2165 2023-04-16 06:07:46.000000 node-1.2.1/src/node.egg-info/SOURCES.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-04-16 06:07:46.000000 node-1.2.1/src/node.egg-info/dependency_links.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2023-04-16 06:07:46.000000 node-1.2.1/src/node.egg-info/namespace_packages.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      109 2023-04-16 06:07:46.000000 node-1.2.1/src/node.egg-info/requires.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2023-04-16 06:07:46.000000 node-1.2.1/src/node.egg-info/top_level.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-04-16 06:07:46.000000 node-1.2.1/src/node.egg-info/zip-safe
```

### Comparing `node-1.2/CHANGES.rst` & `node-1.2.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 
 Changes
 =======
 
+1.2.1 (2023-04-16)
+------------------
+
+- Replace deprecated import of ``Order`` with ``MappingOrder`` in ``node.base``.
+  [rnix]
+
+
 1.2 (2022-12-05)
 ----------------
 
 - Do not overwrite ``uuid`` in ``node.behaviors.UUIDAware.__init__`` if
   ``uuid`` already set.
   [rnix]
```

### Comparing `node-1.2/LICENSE.rst` & `node-1.2.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `node-1.2/PKG-INFO` & `node-1.2.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,1312 +1,1319 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: node
-Version: 1.2
+Version: 1.2.1
 Summary: Building data structures as node trees
 Home-page: http://github.com/conestack/node
 Author: Node Contributors
 Author-email: dev@conestack.org
 License: Simplified BSD
-Description: Node
-        ====
-        
-        .. image:: https://img.shields.io/pypi/v/node.svg
-            :target: https://pypi.python.org/pypi/node
-            :alt: Latest PyPI version
-        
-        .. image:: https://img.shields.io/pypi/dm/node.svg
-            :target: https://pypi.python.org/pypi/node
-            :alt: Number of PyPI downloads
-        
-        .. image:: https://github.com/conestack/node/actions/workflows/test.yaml/badge.svg
-            :target: https://github.com/conestack/node/actions/workflows/test.yaml
-            :alt: Test node
-        
-        
-        Overview
-        --------
-        
-        Node is a library to create nested data models and structures.
-        
-        These data models are described as trees of nodes, optionally with attributes
-        and schema definitions.
-        
-        They utilize:
-        
-        - Python's
-          `mapping and sequence API's <http://docs.python.org/reference/datamodel.html>`_
-          for accessing node members.
-        - The contract of
-          `zope.location.interfaces.ILocation <https://zopelocation.readthedocs.io/en/latest/api.html#zope.location.interfaces.ILocation>`_
-          for hierarchy information.
-        
-        One purpose of this package is to provide a unified API to different backend
-        storages. Specific storage related implementations are for example:
-        
-        - `node.ext.fs <https://pypi.org/project/node.ext.fs>`_
-        - `node.ext.ldap <https://pypi.org/project/node.ext.ldap>`_
-        - `node.ext.yaml <https://pypi.org/project/node.ext.yaml>`_
-        - `node.ext.zodb <https://pypi.org/project/node.ext.zodb>`_
-        
-        Another usecase is providing interfaces for specific application domains.
-        
-        E.g. for user and group management,
-        `node.ext.ugm <https://pypi.org/project/node.ext.ugm>`_ defines the interfaces.
-        Additional it implements a file based default implementation. Then there are
-        specific implementations of those interfaces in
-        `node.ext.ldap <https://pypi.org/project/node.ext.ldap>`_ and
-        `cone.sql <https://pypi.org/project/cone.sql>`_, to access users and groups in
-        LDAP and SQL databases.
-        
-        This package is also used to build in-memory models of all sorts.
-        
-        E.g.  `yafowil <https://pypi.org/project/yafowil>`_ is a HTML form processing
-        and rendering library. It uses node trees for declarative description of the
-        form model.
-        
-        Another one to mention is `cone.app <https://pypi.org/project/cone.app>`_,
-        a `Pyramid <https://pypi.org/project/pyramid>`_ based development environment
-        for web applications, which uses node trees to describe the application model.
-        
-        
-        Basic Usage
-        -----------
-        
-        There are two basic node types. Mapping nodes and sequence nodes. This
-        package provides some basic nodes to start from.
-        
-        
-        Mapping Nodes
-        ~~~~~~~~~~~~~
-        
-        Mapping nodes implement ``node.interfaces.IMappingNode``. A mapping in python
-        is a container object that supports arbitrary key lookups and implements the
-        methods specified in the ``MutableMapping`` of pythons abstract base classes
-        respective ``zope.interface.common.mapping.IFullMapping``.
-        
-        An unordered node. This can be used as base for trees where order of items
-        doesn't matter:
-        
-        .. code-block:: python
-        
-            from node.base import BaseNode
-        
-            root = BaseNode(name='root')
-            root['child'] = BaseNode()
-        
-        An ordered node. The order of items is preserved:
-        
-        .. code-block:: python
-        
-            from node.base import OrderedNode
-        
-            root = OrderedNode(name='orderedroot')
-            root['foo'] = OrderedNode()
-            root['bar'] = OrderedNode()
-        
-        With ``printtree`` we can do a quick inspection of our node tree:
-        
-        .. code-block:: pycon
-        
-            >>> root.printtree()
-            <class 'node.base.OrderedNode'>: orderedroot
-              <class 'node.base.OrderedNode'>: foo
-              <class 'node.base.OrderedNode'>: bar
-        
-        
-        Sequence Nodes
-        ~~~~~~~~~~~~~~
-        
-        Sequence nodes implement ``node.interfaces.ISequenceNode``. In the context
-        of this library, a sequence is an implementation of the methods
-        specified in the ``MutableSequence`` of pythons abstract base classes respective
-        ``zope.interface.common.collections.IMutableSequence``.
-        
-        Using a list node:
-        
-        .. code-block:: python
-        
-            from node.base import BaseNode
-            from node.base import ListNode
-        
-            root = ListNode(name='listroot')
-            root.insert(0, BaseNode())
-            root.insert(1, BaseNode())
-        
-        Check tree structure with ``printtree``:
-        
-        .. code-block:: pycon
-        
-            >>> root.printtree()
-            <class 'node.base.ListNode'>: listnode
-              <class 'node.base.BaseNode'>: 0
-              <class 'node.base.BaseNode'>: 1
-        
-        .. note::
-        
-            Sequence nodes are introduced as of node 1.0 and are not as feature rich
-            as mapping nodes (yet). If you find inconsistencies or missing features,
-            please file an issue or create a pull request at github.
-        
-        
-        Behaviors
-        ~~~~~~~~~
-        
-        ``node`` utilizes the `plumber <http://pypi.python.org/pypi/plumber>`_ package.
-        
-        The different functionalities of nodes are provided as plumbing behaviors:
-        
-        .. code-block:: python
-        
-            from node.behaviors import DefaultInit
-            from node.behaviors import MappingNode
-            from node.behaviors import OdictStorage
-            from plumber import plumbing
-        
-            @plumbing(
-                DefaultInit,
-                MappingNode,
-                OdictStorage)
-            class CustomNode:
-                pass
-        
-        When inspecting the ``CustomNode`` class, we can see it was plumbed using given
-        behaviors, now representing a complete node implementation:
-        
-        .. code-block:: pycon
-        
-            >>> dir(CustomNode)
-            ['__bool__', '__class__', '__contains__', '__delattr__', '__delitem__',
-            '__dict__', '__dir__', '__doc__', '__eq__', '__format__', '__ge__',
-            '__getattribute__', '__getitem__', '__gt__', '__hash__', '__implemented__',
-            '__init__', '__init_subclass__', '__iter__', '__le__', '__len__', '__lt__',
-            '__module__', '__name__', '__ne__', '__new__', '__nonzero__', '__parent__',
-            '__plumbing__', '__plumbing_stacks__', '__provides__', '__reduce__',
-            '__reduce_ex__', '__repr__', '__setattr__', '__setitem__', '__sizeof__',
-            '__str__', '__subclasshook__', '__weakref__', 'acquire', 'clear', 'copy',
-            'deepcopy', 'detach', 'filtereditems', 'filtereditervalues', 'filteredvalues',
-            'get', 'has_key', 'items', 'iteritems', 'iterkeys', 'itervalues', 'keys',
-            'name', 'noderepr', 'parent', 'path', 'pop', 'popitem', 'printtree', 'root',
-            'setdefault', 'storage', 'treerepr', 'update', 'values']
-        
-        Please read the documentation of ``plumber`` for detailed information about the
-        plumbing system.
-        
-        
-        Attributes
-        ~~~~~~~~~~
-        
-        While it is not strictly necessary, it's a good idea to separate the
-        hierarchical structure of a model from the node related attributes to avoid
-        naming conflicts. Attributes are provided via ``node.behaviors.Attributes``
-        plumbing behavior:
-        
-        .. code-block:: python
-        
-            from node.behaviors import Attributes
-            from node.behaviors import DefaultInit
-            from node.behaviors import DictStorage
-            from node.behaviors import MappingNode
-            from plumber import plumbing
-        
-            @plumbing(
-                Attributes,
-                DefaultInit,
-                MappingNode,
-                DictStorage)
-            class NodeWithAttributes:
-                pass
-        
-        The node now provides an ``attrs`` attribute. Node attributes are itself just
-        a node:
-        
-        .. code-block:: pycon
-        
-            >>> node = NodeWithAttributes()
-            >>> attrs = node.attrs
-            >>> attrs
-            <NodeAttributes object 'None' at ...>
-        
-            >>> attrs['foo'] = 'foo'
-        
-        If it's desired to access attribute members via python attribute access,
-        ``attribute_access_for_attrs`` must be set on node:
-        
-        .. code-block:: pycon
-        
-            >>> node.attribute_access_for_attrs = True
-            >>> attrs = node.attrs
-            >>> attrs.foo = 'bar'
-            >>> attrs.foo
-            'bar'
-        
-        A custom attributes implementation can be set by defining
-        ``attributes_factory`` on the node:
-        
-        .. code-block:: python
-        
-            from node.behaviors import NodeAttributes
-        
-            class CustomAttributes(NodeAttributes):
-                pass
-        
-            class CustomAttributesNode(NodeWithAttributes):
-                attributes_factory = CustomAttributes
-        
-        This factory is then used to instantiate the attributes:
-        
-        .. code-block:: pycon
-        
-            >>> node = CustomAttributesNode()
-            >>> node.attrs
-            <CustomAttributes object 'None' at ...>
-        
-        
-        Schema
-        ~~~~~~
-        
-        To describe the data types of node members, this package provides a mechanism
-        for defining schemata.
-        
-        This can happen in different ways. One is to define the schema for node members
-        directly. This is useful for nodes representing a leaf in the hierarchy or for
-        node attribute nodes:
-        
-        .. code-block:: python
-        
-            from node import schema
-            from node.base import BaseNode
-            from node.behaviors import DefaultInit
-            from node.behaviors import DictStorage
-            from node.behaviors import MappingNode
-            from node.behaviors import Schema
-            from plumber import plumbing
-        
-            @plumbing(
-                DefaultInit,
-                MappingNode,
-                DictStorage,
-                Schema)
-            class SchemaNode:
-                schema = {
-                    'int': schema.Int(),
-                    'float': schema.Float(default=1.),
-                    'str': schema.Str(),
-                    'bool': schema.Bool(default=False),
-                    'node': schema.Node(BaseNode)
-                }
-        
-        Children defined in the schema provide a default value. If not explicitely
-        defined, the default value is always ``node.utils.UNSET``:
-        
-        .. code-block:: pycon
-        
-            >>> node = SchemaNode()
-            >>> node['int']
-            <UNSET>
-        
-            >>> node['float']
-            1.0
-        
-            >>> node['bool']
-            False
-        
-        Children defined in the schema are validated against the defined type when
-        setting it's value:
-        
-        .. code-block:: pycon
-        
-            >>> node = SchemaNode()
-            >>> node['int'] = 'A'
-            Traceback (most recent call last):
-              ...
-            ValueError: A is no <class 'int'> type
-        
-        For accessing members defined in the schema as node attributes,
-        ``SchemaAsAttributes`` plumbing behavior can be used:
-        
-        .. code-block:: python
-        
-            from node.behaviors import SchemaAsAttributes
-        
-            @plumbing(SchemaAsAttributes)
-            class SchemaAsAttributesNode(BaseNode):
-                schema = {
-                    'int': schema.Int(default=1),
-                }
-        
-        Node ``attrs`` now provides access to the schema members:
-        
-        .. code-block:: pycon
-        
-            >>> node = SchemaAsAttributesNode()
-            >>> node.attrs['int']
-            1
-        
-        Schema members can also be defined as class attributes. This is syntactically
-        the most elegant way, but comes with the tradeoff of possible naming conflicts:
-        
-        .. code-block:: python
-        
-            from node.behaviors import SchemaProperties
-        
-            @plumbing(
-                DefaultInit,
-                MappingNode,
-                DictStorage,
-                SchemaProperties)
-            class SchemaPropertiesNode:
-                text = schema.Str(default='Text')
-        
-        Here we access ``text`` as class attribute:
-        
-        .. code-block:: pycon
-        
-            >>> node = SchemaPropertiesNode()
-            >>> node.text
-            'Text'
-        
-            >>> node.text = 1
-            Traceback (most recent call last):
-              ...
-            ValueError: 1 is no <class 'str'> type
-        
-        
-        Plumbing Behaviors
-        ------------------
-        
-        General Behaviors
-        ~~~~~~~~~~~~~~~~~
-        
-        **node.behaviors.DefaultInit**
-            Plumbing behavior providing default ``__init__`` function on node. This
-            behavior is going to be deprecated in future versions. Use
-            ``node.behaviors.NodeInit`` instead.
-            See ``node.interfaces.IDefaultInit``.
-        
-        **node.behaviors.NodeInit**
-            Plumbing behavior for transparent setting of ``__name__`` and ``__parent__``
-            at object initialization time.
-            See ``node.interfaces.INodeInit``.
-        
-        **node.behaviors.Node**
-            Fill in gaps for full INode API. See ``node.interfaces.INode``.
-        
-        **node.behaviors.ContentishNode**
-            A node which can contain children. See
-            ``node.interfaces.IContentishNode``. Concrete implementations are
-            ``node.behaviors.MappingNode`` and ``node.behaviors.SequenceNode``.
-        
-        **node.behaviors.Attributes**
-            Provide attributes on node. See ``node.interfaces.IAttributes``. If
-            ``node.behaviors.Nodespaces`` is applied on node, the attributes instance
-            gets stored internally in ``__attrs__`` nodespace, otherwise its set on
-            ``__attrs__`` attribute.
-        
-        **node.behaviors.Events**
-            Provide an event registration and dispatching mechanism.
-            See ``node.interfaces.IEvents``.
-        
-        **node.behaviors.BoundContext**
-            Mechanism for scoping objects to interfaces and classes.
-            See ``node.interfaces.IBoundContext``.
-        
-        **node.behaviors.NodeReference**
-            Plumbing behavior holding an index of nodes contained in the tree.
-            See ``node.interfaces.INodeReference``.
-        
-        **node.behaviors.WildcardFactory**
-            Plumbing behavior providing factories by wildcard patterns.
-            See ``node.interfaces.IWildcardFactory``.
-        
-        
-        Mapping Behaviors
-        ~~~~~~~~~~~~~~~~~
-        
-        **node.behaviors.MappingNode**
-            Turn an object into a mapping node. Extends ``node.behaviors.Node``.
-            See ``node.interfaces.IMappingNode``.
-        
-        **node.behaviors.MappingAdopt**
-            Plumbing behavior that provides ``__name__`` and ``__parent__`` attribute
-            adoption on child nodes of mapping.
-            See ``node.interfaces.IMappingAdopt``.
-        
-        **node.behaviors.MappingConstraints**
-            Plumbing behavior for constraints on mapping nodes.
-            See ``node.interfaces.IMappingConstraints``.
-        
-        **node.behaviors.UnicodeAware**
-            Plumbing behavior to ensure unicode for keys and string values.
-            See ``node.interfaces.IUnicodeAware``.
-        
-        **node.behaviors.Alias**
-            Plumbing behavior that provides aliasing of child keys.
-            See ``node.interfaces.IAlias``.
-        
-        **node.behaviors.AsAttrAccess**
-            Plumbing behavior to get node as IAttributeAccess implementation.
-            See ``node.interfaces.IAsAttrAccess``.
-        
-        **node.behaviors.ChildFactory**
-            Plumbing behavior providing child factories.
-            See ``node.interfaces.IChildFactory``.
-        
-        **node.behaviors.FixedChildren**
-            Plumbing Behavior that initializes a fixed dictionary as children.
-            See ``node.interfaces.IFixedChildren``.
-        
-        **node.behaviors.Nodespaces**
-            Plumbing behavior for providing nodespaces on node.
-            See ``node.interfaces.INodespaces``.
-        
-        **node.behaviors.Lifecycle**
-            Plumbing behavior taking care of lifecycle events.
-            See ``node.interfaces.ILifecycle``.
-        
-        **node.behaviors.AttributesLifecycle**
-            Plumbing behavior for handling lifecycle events on attribute manipulation.
-            See ``node.interfaces.IAttributesLifecycle``.
-        
-        **node.behaviors.Invalidate**
-            Plumbing behavior for node invalidation.
-            See ``node.interfaces.Invalidate``.
-        
-        **node.behaviors.VolatileStorageInvalidate**
-            Plumbing behavior for invalidating nodes using a volatile storage.
-            See ``node.interfaces.Invalidate``.
-        
-        **node.behaviors.Cache**
-            Plumbing behavior for caching.
-            See ``node.interfaces.ICache``.
-        
-        **node.behaviors.MappingOrder**
-            Plumbing behavior for ordering support on mapping nodes.
-            See ``node.interfaces.IMappingOrder``.
-        
-        **node.behaviors.UUIDAware**
-            Plumbing behavior providing a uuid on nodes.
-            See ``node.interfaces.IUUIDAware``.
-        
-        **node.behaviors.MappingReference**
-            Plumbing behavior to provide ``node.interfaces.INodeReference`` on mapping
-            nodes. See ``node.interfaces.IMappingReference``.
-        
-        **node.behaviors.MappingStorage**
-            Provide abstract mapping storage access.
-            See ``node.interfaces.IMappingStorage``.
-        
-        **node.behaviors.DictStorage**
-            Provide dictionary storage. Extends ``node.behaviors.MappingStorage``.
-            See ``node.interfaces.IMappingStorage``.
-        
-        **node.behaviors.OdictStorage**
-            Provide ordered dictionary storage. Extends
-            ``node.behaviors.MappingStorage``. See ``node.interfaces.IMappingStorage``.
-        
-        **node.behaviors.Fallback**
-            Provide a way to fall back to values by subpath stored on another node.
-            See ``node.interfaces.IFallback``.
-        
-        **node.behaviors.Schema**
-            Provide schema validation and value serialization on node values.
-            See ``node.interfaces.ISchema``.
-        
-        **node.behaviors.SchemaAsAttributes**
-            Provide schema validation and value serialization on node values via
-            dedicated attributes object.
-            See ``node.interfaces.ISchemaAsAttributes``.
-        
-        **node.behaviors.SchemaProperties**
-            Provide schema fields as class properties.
-            See ``node.interfaces.ISchemaProperties``.
-        
-        **node.behaviors.MappingFilter**
-            Filter mapping children by class or interface.
-            See ``node.interfaces.IChildFilter``.
-        
-        
-        Sequence Behaviors
-        ~~~~~~~~~~~~~~~~~~
-        
-        **node.behaviors.SequenceNode**
-            Turn an object into a sequence node. Extends ``node.behaviors.Node``.
-            See ``node.interfaces.IMappingNode``.
-        
-        **node.behaviors.SequenceAdopt**
-            Plumbing behavior that provides ``__name__`` and ``__parent__`` attribute
-            adoption on child nodes of sequence.
-            See ``node.interfaces.ISequenceAdopt``.
-        
-        **node.behaviors.SequenceConstraints**
-            Plumbing behavior for constraints on sequence nodes.
-            See ``node.interfaces.ISequenceConstraints``.
-        
-        **node.behaviors.SequenceStorage**
-            Provide abstract sequence storage access.
-            See ``node.interfaces.ISequenceStorage``.
-        
-        **node.behaviors.ListStorage**
-            Provide list storage. See ``node.interfaces.ISequenceStorage``.
-        
-        **node.behaviors.SequenceReference**
-            Plumbing behavior to provide ``node.interfaces.INodeReference`` on sequence
-            nodes. See ``node.interfaces.ISequenceReference``.
-        
-        **node.behaviors.SequenceFilter**
-            Filter sequence children by class or interface.
-            See ``node.interfaces.IChildFilter``.
-        
-        **node.behaviors.SequenceOrder**
-            Plumbing behavior for ordering support on sequence nodes.
-            See ``node.interfaces.ISequenceOrder``.
-        
-        
-        JSON Serialization
-        ------------------
-        
-        Nodes can be serialized to and deserialized from JSON:
-        
-        .. code-block:: pycon
-        
-            >>> from node.serializer import serialize
-            >>> json_dump = serialize(BaseNode(name='node'))
-        
-            >>> from node.serializer import deserialize
-            >>> deserialize(json_dump)
-            <BaseNode object 'node' at ...>
-        
-        For details on serialization API please read file in
-        ``docs/archive/serializer.rst``.
-        
-        
-        Python Versions
-        ---------------
-        
-        - Python 2.7, 3.7+
-        - May work with other versions (untested)
-        
-        
-        Contributors
-        ============
-        
-        - Robert Niederreiter
-        - Florian Friesdorf
-        - Jens Klein
-        
-        
-        
-        Changes
-        =======
-        
-        1.2 (2022-12-05)
-        ----------------
-        
-        - Do not overwrite ``uuid`` in ``node.behaviors.UUIDAware.__init__`` if
-          ``uuid`` already set.
-          [rnix]
-        
-        - Rename ``node.interfaces.IOrder`` to ``node.interfaces.IMappingOrder``
-          and ``node.behaviors.Order`` to ``node.behaviors.MappingOrder``.
-          B/C is kept.
-          [rnix]
-        
-        - Introduce ``node.behaviors.ISequenceOrder`` and
-          ``node.interfaces.SequenceOrder``.
-          [rnix]
-        
-        - Introduce ``node.interfaces.INodeOrder``. Used as base for
-          ``node.interfaces.IMappingOrder`` and ``node.interfaces.ISequenceOrder``.
-          [rnix]
-        
-        - Add rich comparison functions ``__lt__``, ``__le__``, ``__gt__`` and
-          ``__ge__`` to ``node.utils.Unset``.
-          [rnix]
-        
-        **Breaking changes**:
-        
-        - Importing B/C ``Order`` behavior from ``node.behaviors.order``
-          not works any more. Please import from ``node.behaviors``.
-          [rnix]
-        
-        
-        1.1 (2022-10-06)
-        ----------------
-        
-        - Add ``node.schema.DateTime``, ``node.schema.DateTimeSerializer`` and
-          ``node.schema.datetime_serializer``.
-          [rnix]
-        
-        - Subclass ``threading.local`` for
-          ``node.behaviors.lifecycle._lifecycle_context``,
-          ``node.behaviors.events._attribute_subscribers`` and
-          ``node.behaviors.schema._schema_property`` objects in order to safely provide
-          default values.
-          [rnix]
-        
-        - Introduce ``node.interfaces.IChildFilter``, ``node.behaviors.MappingFilter``
-          and ``node.behaviors.SequenceFilter``.
-          [rnix]
-        
-        - Introduce ``node.interfaces.IWildcardFactory`` and
-          ``node.behaviors.WildcardFactory``.
-          [rnix]
-        
-        - Introduce ``node.interfaces.INodeInit`` and ``node.behaviors.NodeInit``.
-          [rnix]
-        
-        - Deprecate ``IFixedChildren.fixed_children_factories`` Use
-          ``IFixedChildren.factories`` instead.
-          [rnix]
-        
-        - Introduce ``node.interfaces.IContentishNode`` and
-          ``node.behaviors.ContentishNode``. Use as base for mapping and sequence nodes.
-          [rnix]
-        
-        - ``insertbefore``, ``insertafter`` and ``swap`` in ``node.behaviors.Order``
-          alternatively accept node names as arguments where possible.
-          [rnix]
-        
-        - ``insertbefore``, ``insertafter``, and ``insertfirst`` and ``insertlast`` in
-          ``node.behaviors.Order`` internally use ``movebefore``, ``moveafter``,
-          ``movefirst`` and ``movelast`` of ``odict`` to avoid modifying the data
-          structure before ``__setitem__`` gets called.
-          [rnix]
-        
-        - Extend ``node.interfaces.IOrder``  respective ``node.behaviors.Order``
-          by ``movebefore``, ``moveafter``, ``movefirst`` and ``movelast``.
-          [rnix]
-        
-        - Reset ``__parent__`` in ``node.behaviors.Node.detach``. Node is no longer
-          contained in tree.
-          [rnix]
-        
-        - Introduce ``IndexViolationError`` which inherits from ``ValueError`` and
-          raise it in reference related behaviors instead of ``ValueError`` where
-          appropriate.
-          [rnix]
-        
-        - Introduce ``node.interfaces.INodeReference`` and
-          ``node.behaviors.NodeReference``.
-          [rnix]
-        
-        - Introduce ``node.interfaces.ISequenceReference`` and
-          ``node.behaviors.SequenceReference``.
-          [rnix]
-        
-        - Rename ``node.interfaces.IReference`` to ``node.interfaces.IMappingReference``
-          and ``node.behaviors.Reference`` to ``node.behaviors.MappingReference``.
-          B/C is kept.
-          [rnix]
-        
-        **Breaking changes**:
-        
-        - Remove ``_notify_suppress`` flag from ``Lifecycle`` behavior. Introduce
-          ``suppress_lifecycle_events`` contextmanager as substitute.
-          [rnix]
-        
-        - Importing ``ChildFactory`` and ``FixedChildren`` from
-          ``node.behaviors.common`` not works any more. Please import from
-          ``node.behaviors``.
-          [rnix]
-        
-        - Importing B/C ``Reference`` behavior from ``node.behaviors.reference``
-          not works any more. Please import from ``node.behaviors``.
-          [rnix]
-        
-        
-        1.0 (2022-03-17)
-        ----------------
-        
-        - Implement ``__copy__`` and ``__deepcopy__`` on ``node.utils.UNSET``.
-          [rnix]
-        
-        - Introduce ``node.interfaces.ISequenceConstraints`` and
-          ``node.behaviors.SequenceConstraints``.
-          [rnix]
-        
-        - Rename ``node.interfaces.INodeChildValidate`` to
-          ``node.interfaces.IMappingConstraints`` and
-          ``node.behaviors.NodeChildValidate`` to ``node.behaviors.MappingConstraints``.
-          ``MappingConstraints`` implementation moved from ``node.behaviors.common`` to
-          ``node.behaviors.constraints``. B/C is kept.
-          [rnix]
-        
-        - Introduce ``node.interfaces.ISequenceAdopt`` and
-          ``node.behaviors.SequenceAdopt``.
-          [rnix]
-        
-        - ``MappingAdopt`` now catches all exceptions instead of only
-          ``AttributeError``, ``KeyError`` and ``ValueError``.
-          [rnix]
-        
-        - Rename ``node.interfaces.IAdopt`` to ``node.interfaces.IMappingAdopt`` and
-          ``node.behaviors.Adopt`` to ``node.behaviors.MappingAdopt``. ``MappingAdopt``
-          implementation moved from ``node.behaviors.common`` to
-          ``node.behaviors.adopt``. B/C is kept.
-          [rnix]
-        
-        - ``node.behaviors.Attributes`` now also works if
-          ``node.behaviors.Nodespaces`` is not applied.
-          [rnix]
-        
-        - Introduce ``node.behaviors.Node`` which implements only
-          ``node.interfaces.INode`` contract. It is used as base for
-          ``node.behaviors.MappingNode`` and ``node.behaviors.SequcneNode``.
-          [rnix]
-        
-        - Do not inherit ``node.interfaces.INode`` from
-          ``zope.interfaces.common.mapping.IFullMapping`` any more. Data model specific
-          interfaces are added now via ``node.interfaces.IMappingNode`` and
-          ``node.interfaces.ISequenceNode``.
-          [rnix]
-        
-        - Introduce sequence nodes. Sequence nodes are implemented via
-          ``node.behaviors.SequcneNode`` and ``node.behaviors.ListStorage``.
-          [rnix]
-        
-        - Rename ``node.interfaces.INodify`` to ``node.interfaces.IMappingNode`` and
-          ``node.behaviors.Nodify`` to ``node.behaviors.MappingNode``. ``MappingNode``
-          implementation moved from ``node.behaviors.nodify`` to
-          ``node.behaviors.mapping``. B/C is kept.
-          [rnix]
-        
-        - Rename ``node.interfaces.IStorage`` to ``node.interfaces.IMappingStorage``
-          and ``node.behaviors.Storage`` to ``node.behaviors.Storage``. B/C is kept.
-          [rnix]
-        
-        - Add key and value type validation to schema fields where appropriate.
-          [rnix]
-        
-        - Introduce serializer support to schema fields. Add a couple of concrete field
-          serializer implementations to ``node.schema.serializer``.
-          [rnix]
-        
-        - Add ``ODict`` and ``Node`` schema fields to ``node.schema.fields``.
-          [rnix]
-        
-        - Add ``node.schema.fields.IterableField`` and use as base class for
-          ``List``, ``Tuple`` and ``Set`` schema fields.
-        
-        - Introduce ``node.behaviors.schema.SchemaProperties`` plumbing behavior.
-          [rnix]
-        
-        - Split up ``node.schema`` module into a package.
-          [rnix]
-        
-        - Introduce ``node.behaviors.context.BoundContext`` plumbing behavior.
-          [rnix]
-        
-        **Breaking changes**:
-        
-        - Remove ``node.behaviors.GetattrChildren``. See ``node.utils.AttributeAccess``
-          instead if you need to access node children via ``__getattr__``.
-          [rnix]
-        
-        - Importing B/C ``Adopt`` behavior from ``node.behaviors.common``
-          not works any more. Please import from ``node.behaviors``.
-          [rnix]
-        
-        - Importing B/C ``NodeChildValidate`` behavior from ``node.behaviors.common``
-          not works any more. Please import from ``node.behaviors``.
-          [rnix]
-        
-        - Importing B/C ``Nodify`` behavior from ``node.behaviors.nodify``
-          not works any more. Please import from ``node.behaviors``.
-          [rnix]
-        
-        - Remove deprecated B/C import location ``node.parts``.
-          [rnix]
-        
-        - ``node.behaviors.schema.Schema`` no longer considers wildcard fields.
-          [rnix]
-        
-        - ``node.behaviors.schema.Schema.__setitem__`` deletes value from related
-          storage for field if value is ``node.utils.UNSET``.
-          [rnix]
-        
-        - ``node.behaviors.schema.Schema.__getitem__`` always returns default value for
-          field instead of raising ``KeyError`` if no default is set.
-          [rnix]
-        
-        - Default value of ``node.schema.fields.Field.default`` is ``node.utils.UNSET``
-          now.
-          [rnix]
-        
-        - ``node.schema.fields.Field.validate`` raises exception if validation fails
-          instead of returning boolean.
-          [rnix]
-        
-        
-        0.9.28 (2021-11-08)
-        -------------------
-        
-        - Add missing ``node.interfaces.INodeAttributes`` interface.
-          [rnix]
-        
-        - Add missing ``attribute_access_for_attrs`` attribute to ``IAttributes``
-          interface.
-          [rnix]
-        
-        - Rename ``node.behaviors.common.NodeChildValidate.allow_non_node_childs``
-          to ``allow_non_node_children``. A Deprecation warning is printed if the
-          old attribute is used.
-          [rnix]
-        
-        - Introduce ``node.behaviors.schema.Schema``,
-          ``node.behaviors.schema.SchemaAsAttributes`` and related schema definitions
-          in ``node.schema``.
-          [rnix]
-        
-        
-        0.9.27 (2021-10-21)
-        -------------------
-        
-        - Expose ``first_key``, ``last_key``, ``next_key`` and ``prev_key`` from
-          odict storage on ``Order`` behavior.
-          [rnix, 2021-10-21]
-        
-        - Add basic serializer settings mechanism.
-          [rnix, 2021-07-20]
-        
-        
-        0.9.26 (2021-05-10)
-        -------------------
-        
-        - Use ``node.utils.safe_decode`` in ``node.behaviors.nodify.Nodify.treerepr``.
-          [rnix, 2021-05-04]
-        
-        - Add ``node.utils.safe_encode`` and ``node.utils.safe_decode``.
-          [rnix, 2021-05-04]
-        
-        
-        0.9.25 (2020-03-30)
-        -------------------
-        
-        - Introduce ``uuid_factory`` function on ``node.interfaces.IUUIDAware`` and
-          implement default function in ``node.behaviors.common.UUIDAware``.
-          [rnix, 2020-03-01]
-        
-        - Rename ``NodeTestCase.expect_error`` to ``NodeTestCase.expectError``.
-          [rnix, 2019-09-04]
-        
-        - Rename ``NodeTestCase.check_output`` to ``NodeTestCase.checkOutput``.
-          [rnix, 2019-09-04]
-        
-        - Introduce ``prefix`` keyword argument in ``Nodify.treerepr``.
-          [rnix, 2019-09-04]
-        
-        
-        0.9.24 (2019-07-10)
-        -------------------
-        
-        - Overhaul ``node.behaviors.Order``. Use related functions from ``odict`` where
-          appropriate.
-          [rnix, 2019-07-10]
-        
-        - Remove superfluous ``extra_require`` from ``setup.py``.
-          [rnix, 2019-04-25]
-        
-        - Drop Support for python < 2.7 and < 3.3.
-          [rnix, 2019-04-25]
-        
-        
-        0.9.23 (2018-11-07)
-        -------------------
-        
-        - Use property decorators for ``node.behaviors.reference.Reference.uuid``.
-          [rnix, 2017-12-15]
-        
-        
-        0.9.22 (2017-07-18)
-        -------------------
-        
-        - Add ``always_dispatch`` keyword argument to
-          ``node.behaviors.events.EventAttribute`` constructor which defines whether
-          events are always dispatched on ``__set__``, not only if attribute value
-          changes.
-          [rnix, 2017-06-20]
-        
-        - Use ``node.utils.UNSET`` as default ``default`` value in
-          ``node.behaviors.events.EventAttribute.__init__``.
-          [rnix, 2017-06-19]
-        
-        - Introduce ``node.behaviors.events.EventAttribute.subscriber`` decorator which
-          can be used to register attribute subscribers.
-          [rnix, 2017-06-19]
-        
-        - Move event dispatching related classes and functions from ``node.events``
-          to ``node.behaviors.events`` and import it from there in ``node.events``.
-          [rnix, 2017-06-16]
-        
-        - Introduce ``node.interfaces.IEvents`` and implement
-          ``node.behaviors.events.Events`` behavior. Contains business logic from
-          ``node.events.EventDispatcher``. Use new behavior on ``EventDispatcher``.
-          [rnix, 2017-06-16]
-        
-        - Create ``suppress_events`` context manager which can be used to
-          suppress event notification in conjunction with ``node.behaviors.Events``
-          behavior.
-          [rnix, 2017-06-15]
-        
-        - Create ``node.behaviors.fallback.fallback_processing`` context manager and
-          and use it in ``node.behaviors.fallback.Fallback.__getitem__`` to check
-          whether fallback processing is active.
-          [rnix, 2017-06-15]
-        
-        
-        0.9.21 (2017-06-15)
-        -------------------
-        
-        - Introduce ``node.events.EventDispatcher`` and ``node.events.EventAttribute``.
-          [rnix, 2017-06-15]
-        
-        - Use ``setattr`` in ``instance_property`` decorator instead of
-          ``object.__setattr__`` in order to avoid errors with custom low level
-          ``__setattr__`` implementations.
-          [rnix, 2017-06-14]
-        
-        
-        0.9.20 (2017-06-07)
-        -------------------
-        
-        - Type cast sort key to ``node.compat.UNICODE_TYPE`` in
-          ``node.behaviors.Nodify.treerepr`` to avoid unicode decode errors.
-          [rnix, 2017-06-07]
-        
-        
-        0.9.19 (2017-06-07)
-        -------------------
-        
-        - Python 3 and pypy compatibility.
-          [rnix, 2017-06-02]
-        
-        - Drop support for Python < 2.7.
-          [rnix, 2017-06-02]
-        
-        - Add ``__bool__`` to ``node.behaviors.Nodify``.
-          [rnix, 2017-06-02]
-        
-        - Add ``__bool__`` to ``node.utils.UNSET``.
-          [rnix, 2017-06-02]
-        
-        - Add ``treerepr`` in ``node.behaviors.nodify.Nodify`` and move code from
-          ``printtree`` to it. Returs tree representation as string instead of printing
-          it. ``printtree`` uses ``treerepr`` now. As enhancement ``treerepr`` sorts
-          children of node if it does not implement ``IOrdered`` in order to ensure
-          consistend output which can be used to write tests against.
-          [rnix, 2017-06-02]
-        
-        - Use ``object.__getattribute__`` explicitely in
-          ``node.utils.instance_property`` to check whether property value already has
-          been computed in order to avoid problems when oberwriting ``__getattr__``
-          on classes using ``instance_property`` decorator.
-          [rnix, 2017-06-02]
-        
-        
-        0.9.18.1 (2017-02-23)
-        ---------------------
-        
-        - Fix permissions.
-          [rnix, 2017-02-23]
-        
-        
-        0.9.18 (2017-02-14)
-        -------------------
-        
-        - Add ``node.utils.node_by_path``.
-          [rnix, 2017-02-07]
-        
-        - Do not depend on ``unittest2`` since its is not used.
-          [jensens, 2017-01-17]
-        
-        - Add ``node.behaviors.Fallback`` behavior.
-          [jensens, 2017-01-17]
-        
-        
-        0.9.17 (2017-01-17)
-        -------------------
-        
-        - Add basic JSON serializer and deserializer.
-          [rnix, 2016-12-03]
-        
-        
-        0.9.16 (2015-10-08)
-        -------------------
-        
-        - Only encode name in ``node.behaviors.nodify.Nodify.__repr__`` and
-          ``node.behaviors.nodify.Nodify.noderepr`` if name is unicode instance.
-          [rnix, 2015-10-03]
-        
-        - Improve ``node.behaviors.nodify.Nodify.printtree``. None node children are
-          printed with key.
-          [rnix, 2015-10-03]
-        
-        
-        0.9.15 (2014-12-17)
-        -------------------
-        
-        - Fix dependency declaration to ``odict`` in order to make setuptools 8.x+
-          happy; using ``>=`` instead of ``>`` now.
-          [jensens, 2014-12-17]
-        
-        
-        0.9.14
-        ------
-        
-        - use ``plumbing`` decorator instead of ``plumber`` metaclass.
-          [rnix, 2014-07-31]
-        
-        
-        0.9.13
-        ------
-        
-        - Introduce ``node.behaviors.cache.VolatileStorageInvalidate``.
-          [rnix, 2014-01-15]
-        
-        
-        0.9.12
-        ------
-        
-        - Add ``zope.component`` to install dependencies.
-          [rnix, 2013-12-09]
-        
-        
-        0.9.11
-        ------
-        
-        - Use ``node.utils.UNSET`` instance in
-          ``node.behaviors.mapping.ExtendedWriteMapping.pop``.
-          [rnix, 2013-02-10]
-        
-        - Improve ``node.utils.Unset``. Add ``Unset`` instance at
-          ``node.utils.UNSET``.
-          [rnix, 2013-02-10]
-        
-        
-        0.9.10
-        ------
-        
-        - Fix ``node.utils.StrCodec.encode`` to return value as is if str and decoding
-          failed.
-          [rnix, 2012-11-07]
-        
-        
-        0.9.9
-        -----
-        
-        - Python 2.7 compatibility.
-          [rnix, 2012-10-15]
-        
-        - Remove ``zope.component.event`` B/C.
-          [rnix, 2012-10-15]
-        
-        - Remove ``zope.location`` B/C.
-          [rnix, 2012-10-15]
-        
-        - Remove ``zope.lifecycleevent`` B/C.
-          [rnix, 2012-10-15]
-        
-        - Pep8.
-          [rnix, 2012-10-15]
-        
-        
-        0.9.8
-        -----
-        
-        - Deprecate the use of ``node.parts``. Use ``node.behaviors`` instead.
-          [rnix, 2012-07-28]
-        
-        - Adopt to ``plumber`` 1.2
-          [rnix, 2012-07-28]
-        
-        
-        0.9.7
-        -----
-        
-        - Introduce ``node.interfaces.IOrdered`` Marker interface. Set this interface
-          on ``node.parts.storage.OdictStorage``.
-          [rnix, 2012-05-21]
-        
-        - ``node.parts.mapping.ClonableMapping`` now supports ``deepcopy``.
-          [rnix, 2012-05-18]
-        
-        - Use ``zope.interface.implementer`` instead of ``zope.interface.implements``
-          all over the place.
-          [rnix, 2012-05-18]
-        
-        - Remove superfluos interfaces.
-          [rnix, 2012-05-18]
-        
-        - Remove ``Zodict`` from ``node.utils``.
-          [rnix, 2012-05-18]
-        
-        - Remove ``AliasedNodespace``, use ``Alias`` part instead.
-          [rnix, 2012-05-18]
-        
-        - Move aliaser objects from ``node.aliasing`` to ``node.parts.alias``.
-          [rnix, 2012-05-18]
-        
-        - Remove ``composition`` module.
-          [rnix, 2012-05-18]
-        
-        - Remove ``bbb`` module.
-          [rnix, 2012-05-18]
-        
-        
-        0.9.6
-        -----
-        
-        - Do not inherit ``node.parts.Reference`` from ``node.parts.UUIDAware``.
-          [rnix, 2012-01-30]
-        
-        - Set ``uuid`` in ``node.parts.Reference.__init__`` plumb.
-          [rnix, 2012-01-30]
-        
-        
-        0.9.5
-        -----
-        
-        - add ``node.parts.nodify.Nodify.acquire`` function.
-          [rnix, 2011-12-05]
-        
-        - add ``node.parts.ChildFactory`` plumbing part.
-          [rnix, 2011-12-04]
-        
-        - add ``node.parts.UUIDAware`` plumbing part.
-          [rnix, 2011-12-02]
-        
-        - fix ``node.parts.Order.swap`` in order to work with pickled nodes.
-          [rnix, 2011-11-28]
-        
-        - use ``node.name`` instead of ``node.__name__`` in
-          ``node.parts.nodify.Nodify.path``.
-          [rnix, 2011-11-17]
-        
-        - add ``swap`` to  ``node.parts.Order``.
-          [rnix, 2011-10-05]
-        
-        - add ``insertfirst`` and ``insertlast`` to ``node.parts.Order``.
-          [rnix, 2011-10-02]
-        
-        
-        0.9.4
-        -----
-        
-        - add ``node.utils.debug`` decorator.
-          [rnix, 2011-07-23]
-        
-        - remove non storage contract specific properties from
-          ``node.aliasing.AliasedNodespace``
-          [rnix, 2011-07-18]
-        
-        - ``node.aliasing`` test completion
-          [rnix, 2011-07-18]
-        
-        - Add non strict functionality to ``node.aliasing.DictAliaser`` for accessing
-          non aliased keys as is as fallback
-          [rnix, 2011-07-18]
-        
-        - Consider ``INode`` implementing objects in ``node.utils.StrCodec``
-          [rnix, 2011-07-16]
-        
-        - Remove duplicate implements in storage parts
-          [rnix, 2011-05-16]
-        
-        
-        0.9.3
-        -----
-        
-        - Increase test coverage
-          [rnix, 2011-05-09]
-        
-        - Add interfaces ``IFixedChildren`` and ``IGetattrChildren`` for related parts.
-          [rnix, 2011-05-09]
-        
-        - Rename ``Unicode`` part to ``UnicodeAware``.
-          [rnix, 2011-05-09]
-        
-        - Add ``node.utils.StrCodec``.
-          [rnix, 2011-05-09]
-        
-        - Inherit ``INodify`` interface from ``INode``.
-          [rnix, 2011-05-08]
-        
-        - Locking tests. Add ``time.sleep`` after thread start.
-          [rnix, 2011-05-08]
-        
-        - Cleanup ``BaseTester``, remove ``sorted_output`` flag (always sort), also
-          search class bases for detection in ``wherefrom``.
-          [rnix, 2011-05-08]
-        
-        - Remove useless try/except in ``utils.AttributeAccess``.
-          [rnix, 2011-05-08]
-        
-        - Add ``instance_property`` decorator to utils.
-          [rnix, 2011-05-06]
-        
-        - Add ``FixedChildren`` and ``GetattrChildren`` parts.
-          [chaoflow, 2011-04-22]
-        
-        
-        0.9.2
-        -----
-        
-        - Add ``__nonzero__`` on ``Nodifiy`` part always return True.
-          [rnix, 2011-03-15]
-        
-        
-        0.9.1
-        -----
-        
-        - Provide ``node.base.Node`` with same behavior like ``zodict.Node`` for
-          migration purposes.
-          [rnix, 2011-02-08]
-        
-        
-        0.9
-        ---
-        
-        - Make it work [rnix, chaoflow, et al]
-        
-        
-        License
-        =======
-        
-        Copyright (c) 2009-2021, BlueDynamics Alliance, Austria
-        Copyright (c) 2021-2022, Node Contributors
-        All rights reserved.
-        
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        * Redistributions of source code must retain the above copyright notice, this
-          list of conditions and the following disclaimer.
-        
-        * Redistributions in binary form must reproduce the above copyright notice, this
-          list of conditions and the following disclaimer in the documentation and/or
-          other materials provided with the distribution.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-        ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-        WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
-        ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-        (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-        LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
-        ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-        (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-        SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-        
 Keywords: node tree fullmapping dict
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE.rst
+
+Node
+====
+
+.. image:: https://img.shields.io/pypi/v/node.svg
+    :target: https://pypi.python.org/pypi/node
+    :alt: Latest PyPI version
+
+.. image:: https://img.shields.io/pypi/dm/node.svg
+    :target: https://pypi.python.org/pypi/node
+    :alt: Number of PyPI downloads
+
+.. image:: https://github.com/conestack/node/actions/workflows/test.yaml/badge.svg
+    :target: https://github.com/conestack/node/actions/workflows/test.yaml
+    :alt: Test node
+
+
+Overview
+--------
+
+Node is a library to create nested data models and structures.
+
+These data models are described as trees of nodes, optionally with attributes
+and schema definitions.
+
+They utilize:
+
+- Python's
+  `mapping and sequence API's <http://docs.python.org/reference/datamodel.html>`_
+  for accessing node members.
+- The contract of
+  `zope.location.interfaces.ILocation <https://zopelocation.readthedocs.io/en/latest/api.html#zope.location.interfaces.ILocation>`_
+  for hierarchy information.
+
+One purpose of this package is to provide a unified API to different backend
+storages. Specific storage related implementations are for example:
+
+- `node.ext.fs <https://pypi.org/project/node.ext.fs>`_
+- `node.ext.ldap <https://pypi.org/project/node.ext.ldap>`_
+- `node.ext.yaml <https://pypi.org/project/node.ext.yaml>`_
+- `node.ext.zodb <https://pypi.org/project/node.ext.zodb>`_
+
+Another usecase is providing interfaces for specific application domains.
+
+E.g. for user and group management,
+`node.ext.ugm <https://pypi.org/project/node.ext.ugm>`_ defines the interfaces.
+Additional it implements a file based default implementation. Then there are
+specific implementations of those interfaces in
+`node.ext.ldap <https://pypi.org/project/node.ext.ldap>`_ and
+`cone.sql <https://pypi.org/project/cone.sql>`_, to access users and groups in
+LDAP and SQL databases.
+
+This package is also used to build in-memory models of all sorts.
+
+E.g.  `yafowil <https://pypi.org/project/yafowil>`_ is a HTML form processing
+and rendering library. It uses node trees for declarative description of the
+form model.
+
+Another one to mention is `cone.app <https://pypi.org/project/cone.app>`_,
+a `Pyramid <https://pypi.org/project/pyramid>`_ based development environment
+for web applications, which uses node trees to describe the application model.
+
+
+Basic Usage
+-----------
+
+There are two basic node types. Mapping nodes and sequence nodes. This
+package provides some basic nodes to start from.
+
+
+Mapping Nodes
+~~~~~~~~~~~~~
+
+Mapping nodes implement ``node.interfaces.IMappingNode``. A mapping in python
+is a container object that supports arbitrary key lookups and implements the
+methods specified in the ``MutableMapping`` of pythons abstract base classes
+respective ``zope.interface.common.mapping.IFullMapping``.
+
+An unordered node. This can be used as base for trees where order of items
+doesn't matter:
+
+.. code-block:: python
+
+    from node.base import BaseNode
+
+    root = BaseNode(name='root')
+    root['child'] = BaseNode()
+
+An ordered node. The order of items is preserved:
+
+.. code-block:: python
+
+    from node.base import OrderedNode
+
+    root = OrderedNode(name='orderedroot')
+    root['foo'] = OrderedNode()
+    root['bar'] = OrderedNode()
+
+With ``printtree`` we can do a quick inspection of our node tree:
+
+.. code-block:: pycon
+
+    >>> root.printtree()
+    <class 'node.base.OrderedNode'>: orderedroot
+      <class 'node.base.OrderedNode'>: foo
+      <class 'node.base.OrderedNode'>: bar
+
+
+Sequence Nodes
+~~~~~~~~~~~~~~
+
+Sequence nodes implement ``node.interfaces.ISequenceNode``. In the context
+of this library, a sequence is an implementation of the methods
+specified in the ``MutableSequence`` of pythons abstract base classes respective
+``zope.interface.common.collections.IMutableSequence``.
+
+Using a list node:
+
+.. code-block:: python
+
+    from node.base import BaseNode
+    from node.base import ListNode
+
+    root = ListNode(name='listroot')
+    root.insert(0, BaseNode())
+    root.insert(1, BaseNode())
+
+Check tree structure with ``printtree``:
+
+.. code-block:: pycon
+
+    >>> root.printtree()
+    <class 'node.base.ListNode'>: listnode
+      <class 'node.base.BaseNode'>: 0
+      <class 'node.base.BaseNode'>: 1
+
+.. note::
+
+    Sequence nodes are introduced as of node 1.0 and are not as feature rich
+    as mapping nodes (yet). If you find inconsistencies or missing features,
+    please file an issue or create a pull request at github.
+
+
+Behaviors
+~~~~~~~~~
+
+``node`` utilizes the `plumber <http://pypi.python.org/pypi/plumber>`_ package.
+
+The different functionalities of nodes are provided as plumbing behaviors:
+
+.. code-block:: python
+
+    from node.behaviors import DefaultInit
+    from node.behaviors import MappingNode
+    from node.behaviors import OdictStorage
+    from plumber import plumbing
+
+    @plumbing(
+        DefaultInit,
+        MappingNode,
+        OdictStorage)
+    class CustomNode:
+        pass
+
+When inspecting the ``CustomNode`` class, we can see it was plumbed using given
+behaviors, now representing a complete node implementation:
+
+.. code-block:: pycon
+
+    >>> dir(CustomNode)
+    ['__bool__', '__class__', '__contains__', '__delattr__', '__delitem__',
+    '__dict__', '__dir__', '__doc__', '__eq__', '__format__', '__ge__',
+    '__getattribute__', '__getitem__', '__gt__', '__hash__', '__implemented__',
+    '__init__', '__init_subclass__', '__iter__', '__le__', '__len__', '__lt__',
+    '__module__', '__name__', '__ne__', '__new__', '__nonzero__', '__parent__',
+    '__plumbing__', '__plumbing_stacks__', '__provides__', '__reduce__',
+    '__reduce_ex__', '__repr__', '__setattr__', '__setitem__', '__sizeof__',
+    '__str__', '__subclasshook__', '__weakref__', 'acquire', 'clear', 'copy',
+    'deepcopy', 'detach', 'filtereditems', 'filtereditervalues', 'filteredvalues',
+    'get', 'has_key', 'items', 'iteritems', 'iterkeys', 'itervalues', 'keys',
+    'name', 'noderepr', 'parent', 'path', 'pop', 'popitem', 'printtree', 'root',
+    'setdefault', 'storage', 'treerepr', 'update', 'values']
+
+Please read the documentation of ``plumber`` for detailed information about the
+plumbing system.
+
+
+Attributes
+~~~~~~~~~~
+
+While it is not strictly necessary, it's a good idea to separate the
+hierarchical structure of a model from the node related attributes to avoid
+naming conflicts. Attributes are provided via ``node.behaviors.Attributes``
+plumbing behavior:
+
+.. code-block:: python
+
+    from node.behaviors import Attributes
+    from node.behaviors import DefaultInit
+    from node.behaviors import DictStorage
+    from node.behaviors import MappingNode
+    from plumber import plumbing
+
+    @plumbing(
+        Attributes,
+        DefaultInit,
+        MappingNode,
+        DictStorage)
+    class NodeWithAttributes:
+        pass
+
+The node now provides an ``attrs`` attribute. Node attributes are itself just
+a node:
+
+.. code-block:: pycon
+
+    >>> node = NodeWithAttributes()
+    >>> attrs = node.attrs
+    >>> attrs
+    <NodeAttributes object 'None' at ...>
+
+    >>> attrs['foo'] = 'foo'
+
+If it's desired to access attribute members via python attribute access,
+``attribute_access_for_attrs`` must be set on node:
+
+.. code-block:: pycon
+
+    >>> node.attribute_access_for_attrs = True
+    >>> attrs = node.attrs
+    >>> attrs.foo = 'bar'
+    >>> attrs.foo
+    'bar'
+
+A custom attributes implementation can be set by defining
+``attributes_factory`` on the node:
+
+.. code-block:: python
+
+    from node.behaviors import NodeAttributes
+
+    class CustomAttributes(NodeAttributes):
+        pass
+
+    class CustomAttributesNode(NodeWithAttributes):
+        attributes_factory = CustomAttributes
+
+This factory is then used to instantiate the attributes:
+
+.. code-block:: pycon
+
+    >>> node = CustomAttributesNode()
+    >>> node.attrs
+    <CustomAttributes object 'None' at ...>
+
+
+Schema
+~~~~~~
+
+To describe the data types of node members, this package provides a mechanism
+for defining schemata.
+
+This can happen in different ways. One is to define the schema for node members
+directly. This is useful for nodes representing a leaf in the hierarchy or for
+node attribute nodes:
+
+.. code-block:: python
+
+    from node import schema
+    from node.base import BaseNode
+    from node.behaviors import DefaultInit
+    from node.behaviors import DictStorage
+    from node.behaviors import MappingNode
+    from node.behaviors import Schema
+    from plumber import plumbing
+
+    @plumbing(
+        DefaultInit,
+        MappingNode,
+        DictStorage,
+        Schema)
+    class SchemaNode:
+        schema = {
+            'int': schema.Int(),
+            'float': schema.Float(default=1.),
+            'str': schema.Str(),
+            'bool': schema.Bool(default=False),
+            'node': schema.Node(BaseNode)
+        }
+
+Children defined in the schema provide a default value. If not explicitely
+defined, the default value is always ``node.utils.UNSET``:
+
+.. code-block:: pycon
+
+    >>> node = SchemaNode()
+    >>> node['int']
+    <UNSET>
+
+    >>> node['float']
+    1.0
+
+    >>> node['bool']
+    False
+
+Children defined in the schema are validated against the defined type when
+setting it's value:
+
+.. code-block:: pycon
+
+    >>> node = SchemaNode()
+    >>> node['int'] = 'A'
+    Traceback (most recent call last):
+      ...
+    ValueError: A is no <class 'int'> type
+
+For accessing members defined in the schema as node attributes,
+``SchemaAsAttributes`` plumbing behavior can be used:
+
+.. code-block:: python
+
+    from node.behaviors import SchemaAsAttributes
+
+    @plumbing(SchemaAsAttributes)
+    class SchemaAsAttributesNode(BaseNode):
+        schema = {
+            'int': schema.Int(default=1),
+        }
+
+Node ``attrs`` now provides access to the schema members:
+
+.. code-block:: pycon
+
+    >>> node = SchemaAsAttributesNode()
+    >>> node.attrs['int']
+    1
+
+Schema members can also be defined as class attributes. This is syntactically
+the most elegant way, but comes with the tradeoff of possible naming conflicts:
+
+.. code-block:: python
+
+    from node.behaviors import SchemaProperties
+
+    @plumbing(
+        DefaultInit,
+        MappingNode,
+        DictStorage,
+        SchemaProperties)
+    class SchemaPropertiesNode:
+        text = schema.Str(default='Text')
+
+Here we access ``text`` as class attribute:
+
+.. code-block:: pycon
+
+    >>> node = SchemaPropertiesNode()
+    >>> node.text
+    'Text'
+
+    >>> node.text = 1
+    Traceback (most recent call last):
+      ...
+    ValueError: 1 is no <class 'str'> type
+
+
+Plumbing Behaviors
+------------------
+
+General Behaviors
+~~~~~~~~~~~~~~~~~
+
+**node.behaviors.DefaultInit**
+    Plumbing behavior providing default ``__init__`` function on node. This
+    behavior is going to be deprecated in future versions. Use
+    ``node.behaviors.NodeInit`` instead.
+    See ``node.interfaces.IDefaultInit``.
+
+**node.behaviors.NodeInit**
+    Plumbing behavior for transparent setting of ``__name__`` and ``__parent__``
+    at object initialization time.
+    See ``node.interfaces.INodeInit``.
+
+**node.behaviors.Node**
+    Fill in gaps for full INode API. See ``node.interfaces.INode``.
+
+**node.behaviors.ContentishNode**
+    A node which can contain children. See
+    ``node.interfaces.IContentishNode``. Concrete implementations are
+    ``node.behaviors.MappingNode`` and ``node.behaviors.SequenceNode``.
+
+**node.behaviors.Attributes**
+    Provide attributes on node. See ``node.interfaces.IAttributes``. If
+    ``node.behaviors.Nodespaces`` is applied on node, the attributes instance
+    gets stored internally in ``__attrs__`` nodespace, otherwise its set on
+    ``__attrs__`` attribute.
+
+**node.behaviors.Events**
+    Provide an event registration and dispatching mechanism.
+    See ``node.interfaces.IEvents``.
+
+**node.behaviors.BoundContext**
+    Mechanism for scoping objects to interfaces and classes.
+    See ``node.interfaces.IBoundContext``.
+
+**node.behaviors.NodeReference**
+    Plumbing behavior holding an index of nodes contained in the tree.
+    See ``node.interfaces.INodeReference``.
+
+**node.behaviors.WildcardFactory**
+    Plumbing behavior providing factories by wildcard patterns.
+    See ``node.interfaces.IWildcardFactory``.
+
+
+Mapping Behaviors
+~~~~~~~~~~~~~~~~~
+
+**node.behaviors.MappingNode**
+    Turn an object into a mapping node. Extends ``node.behaviors.Node``.
+    See ``node.interfaces.IMappingNode``.
+
+**node.behaviors.MappingAdopt**
+    Plumbing behavior that provides ``__name__`` and ``__parent__`` attribute
+    adoption on child nodes of mapping.
+    See ``node.interfaces.IMappingAdopt``.
+
+**node.behaviors.MappingConstraints**
+    Plumbing behavior for constraints on mapping nodes.
+    See ``node.interfaces.IMappingConstraints``.
+
+**node.behaviors.UnicodeAware**
+    Plumbing behavior to ensure unicode for keys and string values.
+    See ``node.interfaces.IUnicodeAware``.
+
+**node.behaviors.Alias**
+    Plumbing behavior that provides aliasing of child keys.
+    See ``node.interfaces.IAlias``.
+
+**node.behaviors.AsAttrAccess**
+    Plumbing behavior to get node as IAttributeAccess implementation.
+    See ``node.interfaces.IAsAttrAccess``.
+
+**node.behaviors.ChildFactory**
+    Plumbing behavior providing child factories.
+    See ``node.interfaces.IChildFactory``.
+
+**node.behaviors.FixedChildren**
+    Plumbing Behavior that initializes a fixed dictionary as children.
+    See ``node.interfaces.IFixedChildren``.
+
+**node.behaviors.Nodespaces**
+    Plumbing behavior for providing nodespaces on node.
+    See ``node.interfaces.INodespaces``.
+
+**node.behaviors.Lifecycle**
+    Plumbing behavior taking care of lifecycle events.
+    See ``node.interfaces.ILifecycle``.
+
+**node.behaviors.AttributesLifecycle**
+    Plumbing behavior for handling lifecycle events on attribute manipulation.
+    See ``node.interfaces.IAttributesLifecycle``.
+
+**node.behaviors.Invalidate**
+    Plumbing behavior for node invalidation.
+    See ``node.interfaces.Invalidate``.
+
+**node.behaviors.VolatileStorageInvalidate**
+    Plumbing behavior for invalidating nodes using a volatile storage.
+    See ``node.interfaces.Invalidate``.
+
+**node.behaviors.Cache**
+    Plumbing behavior for caching.
+    See ``node.interfaces.ICache``.
+
+**node.behaviors.MappingOrder**
+    Plumbing behavior for ordering support on mapping nodes.
+    See ``node.interfaces.IMappingOrder``.
+
+**node.behaviors.UUIDAware**
+    Plumbing behavior providing a uuid on nodes.
+    See ``node.interfaces.IUUIDAware``.
+
+**node.behaviors.MappingReference**
+    Plumbing behavior to provide ``node.interfaces.INodeReference`` on mapping
+    nodes. See ``node.interfaces.IMappingReference``.
+
+**node.behaviors.MappingStorage**
+    Provide abstract mapping storage access.
+    See ``node.interfaces.IMappingStorage``.
+
+**node.behaviors.DictStorage**
+    Provide dictionary storage. Extends ``node.behaviors.MappingStorage``.
+    See ``node.interfaces.IMappingStorage``.
+
+**node.behaviors.OdictStorage**
+    Provide ordered dictionary storage. Extends
+    ``node.behaviors.MappingStorage``. See ``node.interfaces.IMappingStorage``.
+
+**node.behaviors.Fallback**
+    Provide a way to fall back to values by subpath stored on another node.
+    See ``node.interfaces.IFallback``.
+
+**node.behaviors.Schema**
+    Provide schema validation and value serialization on node values.
+    See ``node.interfaces.ISchema``.
+
+**node.behaviors.SchemaAsAttributes**
+    Provide schema validation and value serialization on node values via
+    dedicated attributes object.
+    See ``node.interfaces.ISchemaAsAttributes``.
+
+**node.behaviors.SchemaProperties**
+    Provide schema fields as class properties.
+    See ``node.interfaces.ISchemaProperties``.
+
+**node.behaviors.MappingFilter**
+    Filter mapping children by class or interface.
+    See ``node.interfaces.IChildFilter``.
+
+
+Sequence Behaviors
+~~~~~~~~~~~~~~~~~~
+
+**node.behaviors.SequenceNode**
+    Turn an object into a sequence node. Extends ``node.behaviors.Node``.
+    See ``node.interfaces.IMappingNode``.
+
+**node.behaviors.SequenceAdopt**
+    Plumbing behavior that provides ``__name__`` and ``__parent__`` attribute
+    adoption on child nodes of sequence.
+    See ``node.interfaces.ISequenceAdopt``.
+
+**node.behaviors.SequenceConstraints**
+    Plumbing behavior for constraints on sequence nodes.
+    See ``node.interfaces.ISequenceConstraints``.
+
+**node.behaviors.SequenceStorage**
+    Provide abstract sequence storage access.
+    See ``node.interfaces.ISequenceStorage``.
+
+**node.behaviors.ListStorage**
+    Provide list storage. See ``node.interfaces.ISequenceStorage``.
+
+**node.behaviors.SequenceReference**
+    Plumbing behavior to provide ``node.interfaces.INodeReference`` on sequence
+    nodes. See ``node.interfaces.ISequenceReference``.
+
+**node.behaviors.SequenceFilter**
+    Filter sequence children by class or interface.
+    See ``node.interfaces.IChildFilter``.
+
+**node.behaviors.SequenceOrder**
+    Plumbing behavior for ordering support on sequence nodes.
+    See ``node.interfaces.ISequenceOrder``.
+
+
+JSON Serialization
+------------------
+
+Nodes can be serialized to and deserialized from JSON:
+
+.. code-block:: pycon
+
+    >>> from node.serializer import serialize
+    >>> json_dump = serialize(BaseNode(name='node'))
+
+    >>> from node.serializer import deserialize
+    >>> deserialize(json_dump)
+    <BaseNode object 'node' at ...>
+
+For details on serialization API please read file in
+``docs/archive/serializer.rst``.
+
+
+Python Versions
+---------------
+
+- Python 2.7, 3.7+
+- May work with other versions (untested)
+
+
+Contributors
+============
+
+- Robert Niederreiter
+- Florian Friesdorf
+- Jens Klein
+
+
+
+Changes
+=======
+
+1.2.1 (2023-04-16)
+------------------
+
+- Replace deprecated import of ``Order`` with ``MappingOrder`` in ``node.base``.
+  [rnix]
+
+
+1.2 (2022-12-05)
+----------------
+
+- Do not overwrite ``uuid`` in ``node.behaviors.UUIDAware.__init__`` if
+  ``uuid`` already set.
+  [rnix]
+
+- Rename ``node.interfaces.IOrder`` to ``node.interfaces.IMappingOrder``
+  and ``node.behaviors.Order`` to ``node.behaviors.MappingOrder``.
+  B/C is kept.
+  [rnix]
+
+- Introduce ``node.behaviors.ISequenceOrder`` and
+  ``node.interfaces.SequenceOrder``.
+  [rnix]
+
+- Introduce ``node.interfaces.INodeOrder``. Used as base for
+  ``node.interfaces.IMappingOrder`` and ``node.interfaces.ISequenceOrder``.
+  [rnix]
+
+- Add rich comparison functions ``__lt__``, ``__le__``, ``__gt__`` and
+  ``__ge__`` to ``node.utils.Unset``.
+  [rnix]
+
+**Breaking changes**:
+
+- Importing B/C ``Order`` behavior from ``node.behaviors.order``
+  not works any more. Please import from ``node.behaviors``.
+  [rnix]
+
+
+1.1 (2022-10-06)
+----------------
+
+- Add ``node.schema.DateTime``, ``node.schema.DateTimeSerializer`` and
+  ``node.schema.datetime_serializer``.
+  [rnix]
+
+- Subclass ``threading.local`` for
+  ``node.behaviors.lifecycle._lifecycle_context``,
+  ``node.behaviors.events._attribute_subscribers`` and
+  ``node.behaviors.schema._schema_property`` objects in order to safely provide
+  default values.
+  [rnix]
+
+- Introduce ``node.interfaces.IChildFilter``, ``node.behaviors.MappingFilter``
+  and ``node.behaviors.SequenceFilter``.
+  [rnix]
+
+- Introduce ``node.interfaces.IWildcardFactory`` and
+  ``node.behaviors.WildcardFactory``.
+  [rnix]
+
+- Introduce ``node.interfaces.INodeInit`` and ``node.behaviors.NodeInit``.
+  [rnix]
+
+- Deprecate ``IFixedChildren.fixed_children_factories`` Use
+  ``IFixedChildren.factories`` instead.
+  [rnix]
+
+- Introduce ``node.interfaces.IContentishNode`` and
+  ``node.behaviors.ContentishNode``. Use as base for mapping and sequence nodes.
+  [rnix]
+
+- ``insertbefore``, ``insertafter`` and ``swap`` in ``node.behaviors.Order``
+  alternatively accept node names as arguments where possible.
+  [rnix]
+
+- ``insertbefore``, ``insertafter``, and ``insertfirst`` and ``insertlast`` in
+  ``node.behaviors.Order`` internally use ``movebefore``, ``moveafter``,
+  ``movefirst`` and ``movelast`` of ``odict`` to avoid modifying the data
+  structure before ``__setitem__`` gets called.
+  [rnix]
+
+- Extend ``node.interfaces.IOrder``  respective ``node.behaviors.Order``
+  by ``movebefore``, ``moveafter``, ``movefirst`` and ``movelast``.
+  [rnix]
+
+- Reset ``__parent__`` in ``node.behaviors.Node.detach``. Node is no longer
+  contained in tree.
+  [rnix]
+
+- Introduce ``IndexViolationError`` which inherits from ``ValueError`` and
+  raise it in reference related behaviors instead of ``ValueError`` where
+  appropriate.
+  [rnix]
+
+- Introduce ``node.interfaces.INodeReference`` and
+  ``node.behaviors.NodeReference``.
+  [rnix]
+
+- Introduce ``node.interfaces.ISequenceReference`` and
+  ``node.behaviors.SequenceReference``.
+  [rnix]
+
+- Rename ``node.interfaces.IReference`` to ``node.interfaces.IMappingReference``
+  and ``node.behaviors.Reference`` to ``node.behaviors.MappingReference``.
+  B/C is kept.
+  [rnix]
+
+**Breaking changes**:
+
+- Remove ``_notify_suppress`` flag from ``Lifecycle`` behavior. Introduce
+  ``suppress_lifecycle_events`` contextmanager as substitute.
+  [rnix]
+
+- Importing ``ChildFactory`` and ``FixedChildren`` from
+  ``node.behaviors.common`` not works any more. Please import from
+  ``node.behaviors``.
+  [rnix]
+
+- Importing B/C ``Reference`` behavior from ``node.behaviors.reference``
+  not works any more. Please import from ``node.behaviors``.
+  [rnix]
+
+
+1.0 (2022-03-17)
+----------------
+
+- Implement ``__copy__`` and ``__deepcopy__`` on ``node.utils.UNSET``.
+  [rnix]
+
+- Introduce ``node.interfaces.ISequenceConstraints`` and
+  ``node.behaviors.SequenceConstraints``.
+  [rnix]
+
+- Rename ``node.interfaces.INodeChildValidate`` to
+  ``node.interfaces.IMappingConstraints`` and
+  ``node.behaviors.NodeChildValidate`` to ``node.behaviors.MappingConstraints``.
+  ``MappingConstraints`` implementation moved from ``node.behaviors.common`` to
+  ``node.behaviors.constraints``. B/C is kept.
+  [rnix]
+
+- Introduce ``node.interfaces.ISequenceAdopt`` and
+  ``node.behaviors.SequenceAdopt``.
+  [rnix]
+
+- ``MappingAdopt`` now catches all exceptions instead of only
+  ``AttributeError``, ``KeyError`` and ``ValueError``.
+  [rnix]
+
+- Rename ``node.interfaces.IAdopt`` to ``node.interfaces.IMappingAdopt`` and
+  ``node.behaviors.Adopt`` to ``node.behaviors.MappingAdopt``. ``MappingAdopt``
+  implementation moved from ``node.behaviors.common`` to
+  ``node.behaviors.adopt``. B/C is kept.
+  [rnix]
+
+- ``node.behaviors.Attributes`` now also works if
+  ``node.behaviors.Nodespaces`` is not applied.
+  [rnix]
+
+- Introduce ``node.behaviors.Node`` which implements only
+  ``node.interfaces.INode`` contract. It is used as base for
+  ``node.behaviors.MappingNode`` and ``node.behaviors.SequcneNode``.
+  [rnix]
+
+- Do not inherit ``node.interfaces.INode`` from
+  ``zope.interfaces.common.mapping.IFullMapping`` any more. Data model specific
+  interfaces are added now via ``node.interfaces.IMappingNode`` and
+  ``node.interfaces.ISequenceNode``.
+  [rnix]
+
+- Introduce sequence nodes. Sequence nodes are implemented via
+  ``node.behaviors.SequcneNode`` and ``node.behaviors.ListStorage``.
+  [rnix]
+
+- Rename ``node.interfaces.INodify`` to ``node.interfaces.IMappingNode`` and
+  ``node.behaviors.Nodify`` to ``node.behaviors.MappingNode``. ``MappingNode``
+  implementation moved from ``node.behaviors.nodify`` to
+  ``node.behaviors.mapping``. B/C is kept.
+  [rnix]
+
+- Rename ``node.interfaces.IStorage`` to ``node.interfaces.IMappingStorage``
+  and ``node.behaviors.Storage`` to ``node.behaviors.Storage``. B/C is kept.
+  [rnix]
+
+- Add key and value type validation to schema fields where appropriate.
+  [rnix]
+
+- Introduce serializer support to schema fields. Add a couple of concrete field
+  serializer implementations to ``node.schema.serializer``.
+  [rnix]
+
+- Add ``ODict`` and ``Node`` schema fields to ``node.schema.fields``.
+  [rnix]
+
+- Add ``node.schema.fields.IterableField`` and use as base class for
+  ``List``, ``Tuple`` and ``Set`` schema fields.
+
+- Introduce ``node.behaviors.schema.SchemaProperties`` plumbing behavior.
+  [rnix]
+
+- Split up ``node.schema`` module into a package.
+  [rnix]
+
+- Introduce ``node.behaviors.context.BoundContext`` plumbing behavior.
+  [rnix]
+
+**Breaking changes**:
+
+- Remove ``node.behaviors.GetattrChildren``. See ``node.utils.AttributeAccess``
+  instead if you need to access node children via ``__getattr__``.
+  [rnix]
+
+- Importing B/C ``Adopt`` behavior from ``node.behaviors.common``
+  not works any more. Please import from ``node.behaviors``.
+  [rnix]
+
+- Importing B/C ``NodeChildValidate`` behavior from ``node.behaviors.common``
+  not works any more. Please import from ``node.behaviors``.
+  [rnix]
+
+- Importing B/C ``Nodify`` behavior from ``node.behaviors.nodify``
+  not works any more. Please import from ``node.behaviors``.
+  [rnix]
+
+- Remove deprecated B/C import location ``node.parts``.
+  [rnix]
+
+- ``node.behaviors.schema.Schema`` no longer considers wildcard fields.
+  [rnix]
+
+- ``node.behaviors.schema.Schema.__setitem__`` deletes value from related
+  storage for field if value is ``node.utils.UNSET``.
+  [rnix]
+
+- ``node.behaviors.schema.Schema.__getitem__`` always returns default value for
+  field instead of raising ``KeyError`` if no default is set.
+  [rnix]
+
+- Default value of ``node.schema.fields.Field.default`` is ``node.utils.UNSET``
+  now.
+  [rnix]
+
+- ``node.schema.fields.Field.validate`` raises exception if validation fails
+  instead of returning boolean.
+  [rnix]
+
+
+0.9.28 (2021-11-08)
+-------------------
+
+- Add missing ``node.interfaces.INodeAttributes`` interface.
+  [rnix]
+
+- Add missing ``attribute_access_for_attrs`` attribute to ``IAttributes``
+  interface.
+  [rnix]
+
+- Rename ``node.behaviors.common.NodeChildValidate.allow_non_node_childs``
+  to ``allow_non_node_children``. A Deprecation warning is printed if the
+  old attribute is used.
+  [rnix]
+
+- Introduce ``node.behaviors.schema.Schema``,
+  ``node.behaviors.schema.SchemaAsAttributes`` and related schema definitions
+  in ``node.schema``.
+  [rnix]
+
+
+0.9.27 (2021-10-21)
+-------------------
+
+- Expose ``first_key``, ``last_key``, ``next_key`` and ``prev_key`` from
+  odict storage on ``Order`` behavior.
+  [rnix, 2021-10-21]
+
+- Add basic serializer settings mechanism.
+  [rnix, 2021-07-20]
+
+
+0.9.26 (2021-05-10)
+-------------------
+
+- Use ``node.utils.safe_decode`` in ``node.behaviors.nodify.Nodify.treerepr``.
+  [rnix, 2021-05-04]
+
+- Add ``node.utils.safe_encode`` and ``node.utils.safe_decode``.
+  [rnix, 2021-05-04]
+
+
+0.9.25 (2020-03-30)
+-------------------
+
+- Introduce ``uuid_factory`` function on ``node.interfaces.IUUIDAware`` and
+  implement default function in ``node.behaviors.common.UUIDAware``.
+  [rnix, 2020-03-01]
+
+- Rename ``NodeTestCase.expect_error`` to ``NodeTestCase.expectError``.
+  [rnix, 2019-09-04]
+
+- Rename ``NodeTestCase.check_output`` to ``NodeTestCase.checkOutput``.
+  [rnix, 2019-09-04]
+
+- Introduce ``prefix`` keyword argument in ``Nodify.treerepr``.
+  [rnix, 2019-09-04]
+
+
+0.9.24 (2019-07-10)
+-------------------
+
+- Overhaul ``node.behaviors.Order``. Use related functions from ``odict`` where
+  appropriate.
+  [rnix, 2019-07-10]
+
+- Remove superfluous ``extra_require`` from ``setup.py``.
+  [rnix, 2019-04-25]
+
+- Drop Support for python < 2.7 and < 3.3.
+  [rnix, 2019-04-25]
+
+
+0.9.23 (2018-11-07)
+-------------------
+
+- Use property decorators for ``node.behaviors.reference.Reference.uuid``.
+  [rnix, 2017-12-15]
+
+
+0.9.22 (2017-07-18)
+-------------------
+
+- Add ``always_dispatch`` keyword argument to
+  ``node.behaviors.events.EventAttribute`` constructor which defines whether
+  events are always dispatched on ``__set__``, not only if attribute value
+  changes.
+  [rnix, 2017-06-20]
+
+- Use ``node.utils.UNSET`` as default ``default`` value in
+  ``node.behaviors.events.EventAttribute.__init__``.
+  [rnix, 2017-06-19]
+
+- Introduce ``node.behaviors.events.EventAttribute.subscriber`` decorator which
+  can be used to register attribute subscribers.
+  [rnix, 2017-06-19]
+
+- Move event dispatching related classes and functions from ``node.events``
+  to ``node.behaviors.events`` and import it from there in ``node.events``.
+  [rnix, 2017-06-16]
+
+- Introduce ``node.interfaces.IEvents`` and implement
+  ``node.behaviors.events.Events`` behavior. Contains business logic from
+  ``node.events.EventDispatcher``. Use new behavior on ``EventDispatcher``.
+  [rnix, 2017-06-16]
+
+- Create ``suppress_events`` context manager which can be used to
+  suppress event notification in conjunction with ``node.behaviors.Events``
+  behavior.
+  [rnix, 2017-06-15]
+
+- Create ``node.behaviors.fallback.fallback_processing`` context manager and
+  and use it in ``node.behaviors.fallback.Fallback.__getitem__`` to check
+  whether fallback processing is active.
+  [rnix, 2017-06-15]
+
+
+0.9.21 (2017-06-15)
+-------------------
+
+- Introduce ``node.events.EventDispatcher`` and ``node.events.EventAttribute``.
+  [rnix, 2017-06-15]
+
+- Use ``setattr`` in ``instance_property`` decorator instead of
+  ``object.__setattr__`` in order to avoid errors with custom low level
+  ``__setattr__`` implementations.
+  [rnix, 2017-06-14]
+
+
+0.9.20 (2017-06-07)
+-------------------
+
+- Type cast sort key to ``node.compat.UNICODE_TYPE`` in
+  ``node.behaviors.Nodify.treerepr`` to avoid unicode decode errors.
+  [rnix, 2017-06-07]
+
+
+0.9.19 (2017-06-07)
+-------------------
+
+- Python 3 and pypy compatibility.
+  [rnix, 2017-06-02]
+
+- Drop support for Python < 2.7.
+  [rnix, 2017-06-02]
+
+- Add ``__bool__`` to ``node.behaviors.Nodify``.
+  [rnix, 2017-06-02]
+
+- Add ``__bool__`` to ``node.utils.UNSET``.
+  [rnix, 2017-06-02]
+
+- Add ``treerepr`` in ``node.behaviors.nodify.Nodify`` and move code from
+  ``printtree`` to it. Returs tree representation as string instead of printing
+  it. ``printtree`` uses ``treerepr`` now. As enhancement ``treerepr`` sorts
+  children of node if it does not implement ``IOrdered`` in order to ensure
+  consistend output which can be used to write tests against.
+  [rnix, 2017-06-02]
+
+- Use ``object.__getattribute__`` explicitely in
+  ``node.utils.instance_property`` to check whether property value already has
+  been computed in order to avoid problems when oberwriting ``__getattr__``
+  on classes using ``instance_property`` decorator.
+  [rnix, 2017-06-02]
+
+
+0.9.18.1 (2017-02-23)
+---------------------
+
+- Fix permissions.
+  [rnix, 2017-02-23]
+
+
+0.9.18 (2017-02-14)
+-------------------
+
+- Add ``node.utils.node_by_path``.
+  [rnix, 2017-02-07]
+
+- Do not depend on ``unittest2`` since its is not used.
+  [jensens, 2017-01-17]
+
+- Add ``node.behaviors.Fallback`` behavior.
+  [jensens, 2017-01-17]
+
+
+0.9.17 (2017-01-17)
+-------------------
+
+- Add basic JSON serializer and deserializer.
+  [rnix, 2016-12-03]
+
+
+0.9.16 (2015-10-08)
+-------------------
+
+- Only encode name in ``node.behaviors.nodify.Nodify.__repr__`` and
+  ``node.behaviors.nodify.Nodify.noderepr`` if name is unicode instance.
+  [rnix, 2015-10-03]
+
+- Improve ``node.behaviors.nodify.Nodify.printtree``. None node children are
+  printed with key.
+  [rnix, 2015-10-03]
+
+
+0.9.15 (2014-12-17)
+-------------------
+
+- Fix dependency declaration to ``odict`` in order to make setuptools 8.x+
+  happy; using ``>=`` instead of ``>`` now.
+  [jensens, 2014-12-17]
+
+
+0.9.14
+------
+
+- use ``plumbing`` decorator instead of ``plumber`` metaclass.
+  [rnix, 2014-07-31]
+
+
+0.9.13
+------
+
+- Introduce ``node.behaviors.cache.VolatileStorageInvalidate``.
+  [rnix, 2014-01-15]
+
+
+0.9.12
+------
+
+- Add ``zope.component`` to install dependencies.
+  [rnix, 2013-12-09]
+
+
+0.9.11
+------
+
+- Use ``node.utils.UNSET`` instance in
+  ``node.behaviors.mapping.ExtendedWriteMapping.pop``.
+  [rnix, 2013-02-10]
+
+- Improve ``node.utils.Unset``. Add ``Unset`` instance at
+  ``node.utils.UNSET``.
+  [rnix, 2013-02-10]
+
+
+0.9.10
+------
+
+- Fix ``node.utils.StrCodec.encode`` to return value as is if str and decoding
+  failed.
+  [rnix, 2012-11-07]
+
+
+0.9.9
+-----
+
+- Python 2.7 compatibility.
+  [rnix, 2012-10-15]
+
+- Remove ``zope.component.event`` B/C.
+  [rnix, 2012-10-15]
+
+- Remove ``zope.location`` B/C.
+  [rnix, 2012-10-15]
+
+- Remove ``zope.lifecycleevent`` B/C.
+  [rnix, 2012-10-15]
+
+- Pep8.
+  [rnix, 2012-10-15]
+
+
+0.9.8
+-----
+
+- Deprecate the use of ``node.parts``. Use ``node.behaviors`` instead.
+  [rnix, 2012-07-28]
+
+- Adopt to ``plumber`` 1.2
+  [rnix, 2012-07-28]
+
+
+0.9.7
+-----
+
+- Introduce ``node.interfaces.IOrdered`` Marker interface. Set this interface
+  on ``node.parts.storage.OdictStorage``.
+  [rnix, 2012-05-21]
+
+- ``node.parts.mapping.ClonableMapping`` now supports ``deepcopy``.
+  [rnix, 2012-05-18]
+
+- Use ``zope.interface.implementer`` instead of ``zope.interface.implements``
+  all over the place.
+  [rnix, 2012-05-18]
+
+- Remove superfluos interfaces.
+  [rnix, 2012-05-18]
+
+- Remove ``Zodict`` from ``node.utils``.
+  [rnix, 2012-05-18]
+
+- Remove ``AliasedNodespace``, use ``Alias`` part instead.
+  [rnix, 2012-05-18]
+
+- Move aliaser objects from ``node.aliasing`` to ``node.parts.alias``.
+  [rnix, 2012-05-18]
+
+- Remove ``composition`` module.
+  [rnix, 2012-05-18]
+
+- Remove ``bbb`` module.
+  [rnix, 2012-05-18]
+
+
+0.9.6
+-----
+
+- Do not inherit ``node.parts.Reference`` from ``node.parts.UUIDAware``.
+  [rnix, 2012-01-30]
+
+- Set ``uuid`` in ``node.parts.Reference.__init__`` plumb.
+  [rnix, 2012-01-30]
+
+
+0.9.5
+-----
+
+- add ``node.parts.nodify.Nodify.acquire`` function.
+  [rnix, 2011-12-05]
+
+- add ``node.parts.ChildFactory`` plumbing part.
+  [rnix, 2011-12-04]
+
+- add ``node.parts.UUIDAware`` plumbing part.
+  [rnix, 2011-12-02]
+
+- fix ``node.parts.Order.swap`` in order to work with pickled nodes.
+  [rnix, 2011-11-28]
+
+- use ``node.name`` instead of ``node.__name__`` in
+  ``node.parts.nodify.Nodify.path``.
+  [rnix, 2011-11-17]
+
+- add ``swap`` to  ``node.parts.Order``.
+  [rnix, 2011-10-05]
+
+- add ``insertfirst`` and ``insertlast`` to ``node.parts.Order``.
+  [rnix, 2011-10-02]
+
+
+0.9.4
+-----
+
+- add ``node.utils.debug`` decorator.
+  [rnix, 2011-07-23]
+
+- remove non storage contract specific properties from
+  ``node.aliasing.AliasedNodespace``
+  [rnix, 2011-07-18]
+
+- ``node.aliasing`` test completion
+  [rnix, 2011-07-18]
+
+- Add non strict functionality to ``node.aliasing.DictAliaser`` for accessing
+  non aliased keys as is as fallback
+  [rnix, 2011-07-18]
+
+- Consider ``INode`` implementing objects in ``node.utils.StrCodec``
+  [rnix, 2011-07-16]
+
+- Remove duplicate implements in storage parts
+  [rnix, 2011-05-16]
+
+
+0.9.3
+-----
+
+- Increase test coverage
+  [rnix, 2011-05-09]
+
+- Add interfaces ``IFixedChildren`` and ``IGetattrChildren`` for related parts.
+  [rnix, 2011-05-09]
+
+- Rename ``Unicode`` part to ``UnicodeAware``.
+  [rnix, 2011-05-09]
+
+- Add ``node.utils.StrCodec``.
+  [rnix, 2011-05-09]
+
+- Inherit ``INodify`` interface from ``INode``.
+  [rnix, 2011-05-08]
+
+- Locking tests. Add ``time.sleep`` after thread start.
+  [rnix, 2011-05-08]
+
+- Cleanup ``BaseTester``, remove ``sorted_output`` flag (always sort), also
+  search class bases for detection in ``wherefrom``.
+  [rnix, 2011-05-08]
+
+- Remove useless try/except in ``utils.AttributeAccess``.
+  [rnix, 2011-05-08]
+
+- Add ``instance_property`` decorator to utils.
+  [rnix, 2011-05-06]
+
+- Add ``FixedChildren`` and ``GetattrChildren`` parts.
+  [chaoflow, 2011-04-22]
+
+
+0.9.2
+-----
+
+- Add ``__nonzero__`` on ``Nodifiy`` part always return True.
+  [rnix, 2011-03-15]
+
+
+0.9.1
+-----
+
+- Provide ``node.base.Node`` with same behavior like ``zodict.Node`` for
+  migration purposes.
+  [rnix, 2011-02-08]
+
+
+0.9
+---
+
+- Make it work [rnix, chaoflow, et al]
+
+
+License
+=======
+
+Copyright (c) 2009-2021, BlueDynamics Alliance, Austria
+Copyright (c) 2021-2022, Node Contributors
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice, this
+  list of conditions and the following disclaimer in the documentation and/or
+  other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
+ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
+ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `node-1.2/README.rst` & `node-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `node-1.2/setup.py` & `node-1.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def read_file(name):
     with open(os.path.join(os.path.dirname(__file__), name)) as f:
         return f.read()
 
 
-version = '1.2'
+version = '1.2.1'
 shortdesc = "Building data structures as node trees"
 longdesc = '\n\n'.join([read_file(name) for name in [
     'README.rst',
     'CHANGES.rst',
     'LICENSE.rst'
 ]])
```

### Comparing `node-1.2/src/node/base.py` & `node-1.2.1/src/node/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from node.behaviors import ListStorage
 from node.behaviors import MappingAdopt
 from node.behaviors import MappingConstraints
 from node.behaviors import MappingNode
 from node.behaviors import MappingReference
 from node.behaviors import Nodespaces
 from node.behaviors import OdictStorage
-from node.behaviors import Order
+from node.behaviors import MappingOrder
 from node.behaviors import SequenceAdopt
 from node.behaviors import SequenceConstraints
 from node.behaviors import SequenceNode
 from plumber import plumbing
 
 
 @plumbing(
@@ -71,29 +71,29 @@
 
 @plumbing(
     MappingConstraints,
     Nodespaces,
     MappingAdopt,
     Attributes,
     MappingReference,
-    Order,
+    MappingOrder,
     AsAttrAccess,
     DefaultInit,
     MappingNode,
     OdictStorage)
 class Node(object):
     """A node with original functionality from zodict.node.Node."""
 
 
 @plumbing(
     MappingConstraints,
     Nodespaces,
     MappingAdopt,
     Attributes,
     MappingReference,
-    Order,
+    MappingOrder,
     AsAttrAccess,
     DefaultInit,
     MappingNode,
     OdictStorage)
 class AttributedNode(object):
     """A node with original functionality from zodict.node.AttributedNode."""
```

### Comparing `node-1.2/src/node/behaviors/__init__.py` & `node-1.2.1/src/node/behaviors/__init__.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/behaviors/adopt.py` & `node-1.2.1/src/node/behaviors/adopt.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/behaviors/alias.py` & `node-1.2.1/src/node/behaviors/alias.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/behaviors/attributes.py` & `node-1.2.1/src/node/behaviors/attributes.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/behaviors/cache.py` & `node-1.2.1/src/node/behaviors/cache.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/behaviors/common.py` & `node-1.2.1/src/node/behaviors/common.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/behaviors/constraints.py` & `node-1.2.1/src/node/behaviors/constraints.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/behaviors/context.py` & `node-1.2.1/src/node/behaviors/context.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/behaviors/events.py` & `node-1.2.1/src/node/behaviors/events.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/behaviors/factories.py` & `node-1.2.1/src/node/behaviors/factories.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/behaviors/fallback.py` & `node-1.2.1/src/node/behaviors/fallback.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/behaviors/filter.py` & `node-1.2.1/src/node/behaviors/filter.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/behaviors/lifecycle.py` & `node-1.2.1/src/node/behaviors/lifecycle.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/behaviors/mapping.py` & `node-1.2.1/src/node/behaviors/mapping.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/behaviors/node.py` & `node-1.2.1/src/node/behaviors/node.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/behaviors/nodespace.py` & `node-1.2.1/src/node/behaviors/nodespace.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/behaviors/order.py` & `node-1.2.1/src/node/behaviors/order.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/behaviors/reference.py` & `node-1.2.1/src/node/behaviors/reference.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/behaviors/schema.py` & `node-1.2.1/src/node/behaviors/schema.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/behaviors/sequence.py` & `node-1.2.1/src/node/behaviors/sequence.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/behaviors/storage.py` & `node-1.2.1/src/node/behaviors/storage.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/compat.py` & `node-1.2.1/src/node/compat.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/events.py` & `node-1.2.1/src/node/events.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/interfaces.py` & `node-1.2.1/src/node/interfaces.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/locking.py` & `node-1.2.1/src/node/locking.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/schema/__init__.py` & `node-1.2.1/src/node/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/schema/fields.py` & `node-1.2.1/src/node/schema/fields.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/schema/scope.py` & `node-1.2.1/src/node/schema/scope.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/schema/serializer.py` & `node-1.2.1/src/node/schema/serializer.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/serializer.py` & `node-1.2.1/src/node/serializer.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/testing/base.py` & `node-1.2.1/src/node/testing/base.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/testing/env.py` & `node-1.2.1/src/node/testing/env.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/testing/fullmapping.py` & `node-1.2.1/src/node/testing/fullmapping.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/__init__.py` & `node-1.2.1/src/node/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_adopt.py` & `node-1.2.1/src/node/tests/test_adopt.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_alias.py` & `node-1.2.1/src/node/tests/test_alias.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_attributes.py` & `node-1.2.1/src/node/tests/test_attributes.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_base.py` & `node-1.2.1/src/node/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_cache.py` & `node-1.2.1/src/node/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_common.py` & `node-1.2.1/src/node/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_constraints.py` & `node-1.2.1/src/node/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_context.py` & `node-1.2.1/src/node/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_events.py` & `node-1.2.1/src/node/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_factories.py` & `node-1.2.1/src/node/tests/test_factories.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_fallback.py` & `node-1.2.1/src/node/tests/test_fallback.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_filter.py` & `node-1.2.1/src/node/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_lifecycle.py` & `node-1.2.1/src/node/tests/test_lifecycle.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_locking.py` & `node-1.2.1/src/node/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_mapping.py` & `node-1.2.1/src/node/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_node.py` & `node-1.2.1/src/node/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_nodespace.py` & `node-1.2.1/src/node/tests/test_nodespace.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_order.py` & `node-1.2.1/src/node/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_reference.py` & `node-1.2.1/src/node/tests/test_reference.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_schema.py` & `node-1.2.1/src/node/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_sequence.py` & `node-1.2.1/src/node/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_serializer.py` & `node-1.2.1/src/node/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_storage.py` & `node-1.2.1/src/node/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_testing.py` & `node-1.2.1/src/node/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_tests.py` & `node-1.2.1/src/node/tests/test_tests.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/tests/test_utils.py` & `node-1.2.1/src/node/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node/utils.py` & `node-1.2.1/src/node/utils.py`

 * *Files identical despite different names*

### Comparing `node-1.2/src/node.egg-info/PKG-INFO` & `node-1.2.1/src/node.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,1312 +1,1319 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: node
-Version: 1.2
+Version: 1.2.1
 Summary: Building data structures as node trees
 Home-page: http://github.com/conestack/node
 Author: Node Contributors
 Author-email: dev@conestack.org
 License: Simplified BSD
-Description: Node
-        ====
-        
-        .. image:: https://img.shields.io/pypi/v/node.svg
-            :target: https://pypi.python.org/pypi/node
-            :alt: Latest PyPI version
-        
-        .. image:: https://img.shields.io/pypi/dm/node.svg
-            :target: https://pypi.python.org/pypi/node
-            :alt: Number of PyPI downloads
-        
-        .. image:: https://github.com/conestack/node/actions/workflows/test.yaml/badge.svg
-            :target: https://github.com/conestack/node/actions/workflows/test.yaml
-            :alt: Test node
-        
-        
-        Overview
-        --------
-        
-        Node is a library to create nested data models and structures.
-        
-        These data models are described as trees of nodes, optionally with attributes
-        and schema definitions.
-        
-        They utilize:
-        
-        - Python's
-          `mapping and sequence API's <http://docs.python.org/reference/datamodel.html>`_
-          for accessing node members.
-        - The contract of
-          `zope.location.interfaces.ILocation <https://zopelocation.readthedocs.io/en/latest/api.html#zope.location.interfaces.ILocation>`_
-          for hierarchy information.
-        
-        One purpose of this package is to provide a unified API to different backend
-        storages. Specific storage related implementations are for example:
-        
-        - `node.ext.fs <https://pypi.org/project/node.ext.fs>`_
-        - `node.ext.ldap <https://pypi.org/project/node.ext.ldap>`_
-        - `node.ext.yaml <https://pypi.org/project/node.ext.yaml>`_
-        - `node.ext.zodb <https://pypi.org/project/node.ext.zodb>`_
-        
-        Another usecase is providing interfaces for specific application domains.
-        
-        E.g. for user and group management,
-        `node.ext.ugm <https://pypi.org/project/node.ext.ugm>`_ defines the interfaces.
-        Additional it implements a file based default implementation. Then there are
-        specific implementations of those interfaces in
-        `node.ext.ldap <https://pypi.org/project/node.ext.ldap>`_ and
-        `cone.sql <https://pypi.org/project/cone.sql>`_, to access users and groups in
-        LDAP and SQL databases.
-        
-        This package is also used to build in-memory models of all sorts.
-        
-        E.g.  `yafowil <https://pypi.org/project/yafowil>`_ is a HTML form processing
-        and rendering library. It uses node trees for declarative description of the
-        form model.
-        
-        Another one to mention is `cone.app <https://pypi.org/project/cone.app>`_,
-        a `Pyramid <https://pypi.org/project/pyramid>`_ based development environment
-        for web applications, which uses node trees to describe the application model.
-        
-        
-        Basic Usage
-        -----------
-        
-        There are two basic node types. Mapping nodes and sequence nodes. This
-        package provides some basic nodes to start from.
-        
-        
-        Mapping Nodes
-        ~~~~~~~~~~~~~
-        
-        Mapping nodes implement ``node.interfaces.IMappingNode``. A mapping in python
-        is a container object that supports arbitrary key lookups and implements the
-        methods specified in the ``MutableMapping`` of pythons abstract base classes
-        respective ``zope.interface.common.mapping.IFullMapping``.
-        
-        An unordered node. This can be used as base for trees where order of items
-        doesn't matter:
-        
-        .. code-block:: python
-        
-            from node.base import BaseNode
-        
-            root = BaseNode(name='root')
-            root['child'] = BaseNode()
-        
-        An ordered node. The order of items is preserved:
-        
-        .. code-block:: python
-        
-            from node.base import OrderedNode
-        
-            root = OrderedNode(name='orderedroot')
-            root['foo'] = OrderedNode()
-            root['bar'] = OrderedNode()
-        
-        With ``printtree`` we can do a quick inspection of our node tree:
-        
-        .. code-block:: pycon
-        
-            >>> root.printtree()
-            <class 'node.base.OrderedNode'>: orderedroot
-              <class 'node.base.OrderedNode'>: foo
-              <class 'node.base.OrderedNode'>: bar
-        
-        
-        Sequence Nodes
-        ~~~~~~~~~~~~~~
-        
-        Sequence nodes implement ``node.interfaces.ISequenceNode``. In the context
-        of this library, a sequence is an implementation of the methods
-        specified in the ``MutableSequence`` of pythons abstract base classes respective
-        ``zope.interface.common.collections.IMutableSequence``.
-        
-        Using a list node:
-        
-        .. code-block:: python
-        
-            from node.base import BaseNode
-            from node.base import ListNode
-        
-            root = ListNode(name='listroot')
-            root.insert(0, BaseNode())
-            root.insert(1, BaseNode())
-        
-        Check tree structure with ``printtree``:
-        
-        .. code-block:: pycon
-        
-            >>> root.printtree()
-            <class 'node.base.ListNode'>: listnode
-              <class 'node.base.BaseNode'>: 0
-              <class 'node.base.BaseNode'>: 1
-        
-        .. note::
-        
-            Sequence nodes are introduced as of node 1.0 and are not as feature rich
-            as mapping nodes (yet). If you find inconsistencies or missing features,
-            please file an issue or create a pull request at github.
-        
-        
-        Behaviors
-        ~~~~~~~~~
-        
-        ``node`` utilizes the `plumber <http://pypi.python.org/pypi/plumber>`_ package.
-        
-        The different functionalities of nodes are provided as plumbing behaviors:
-        
-        .. code-block:: python
-        
-            from node.behaviors import DefaultInit
-            from node.behaviors import MappingNode
-            from node.behaviors import OdictStorage
-            from plumber import plumbing
-        
-            @plumbing(
-                DefaultInit,
-                MappingNode,
-                OdictStorage)
-            class CustomNode:
-                pass
-        
-        When inspecting the ``CustomNode`` class, we can see it was plumbed using given
-        behaviors, now representing a complete node implementation:
-        
-        .. code-block:: pycon
-        
-            >>> dir(CustomNode)
-            ['__bool__', '__class__', '__contains__', '__delattr__', '__delitem__',
-            '__dict__', '__dir__', '__doc__', '__eq__', '__format__', '__ge__',
-            '__getattribute__', '__getitem__', '__gt__', '__hash__', '__implemented__',
-            '__init__', '__init_subclass__', '__iter__', '__le__', '__len__', '__lt__',
-            '__module__', '__name__', '__ne__', '__new__', '__nonzero__', '__parent__',
-            '__plumbing__', '__plumbing_stacks__', '__provides__', '__reduce__',
-            '__reduce_ex__', '__repr__', '__setattr__', '__setitem__', '__sizeof__',
-            '__str__', '__subclasshook__', '__weakref__', 'acquire', 'clear', 'copy',
-            'deepcopy', 'detach', 'filtereditems', 'filtereditervalues', 'filteredvalues',
-            'get', 'has_key', 'items', 'iteritems', 'iterkeys', 'itervalues', 'keys',
-            'name', 'noderepr', 'parent', 'path', 'pop', 'popitem', 'printtree', 'root',
-            'setdefault', 'storage', 'treerepr', 'update', 'values']
-        
-        Please read the documentation of ``plumber`` for detailed information about the
-        plumbing system.
-        
-        
-        Attributes
-        ~~~~~~~~~~
-        
-        While it is not strictly necessary, it's a good idea to separate the
-        hierarchical structure of a model from the node related attributes to avoid
-        naming conflicts. Attributes are provided via ``node.behaviors.Attributes``
-        plumbing behavior:
-        
-        .. code-block:: python
-        
-            from node.behaviors import Attributes
-            from node.behaviors import DefaultInit
-            from node.behaviors import DictStorage
-            from node.behaviors import MappingNode
-            from plumber import plumbing
-        
-            @plumbing(
-                Attributes,
-                DefaultInit,
-                MappingNode,
-                DictStorage)
-            class NodeWithAttributes:
-                pass
-        
-        The node now provides an ``attrs`` attribute. Node attributes are itself just
-        a node:
-        
-        .. code-block:: pycon
-        
-            >>> node = NodeWithAttributes()
-            >>> attrs = node.attrs
-            >>> attrs
-            <NodeAttributes object 'None' at ...>
-        
-            >>> attrs['foo'] = 'foo'
-        
-        If it's desired to access attribute members via python attribute access,
-        ``attribute_access_for_attrs`` must be set on node:
-        
-        .. code-block:: pycon
-        
-            >>> node.attribute_access_for_attrs = True
-            >>> attrs = node.attrs
-            >>> attrs.foo = 'bar'
-            >>> attrs.foo
-            'bar'
-        
-        A custom attributes implementation can be set by defining
-        ``attributes_factory`` on the node:
-        
-        .. code-block:: python
-        
-            from node.behaviors import NodeAttributes
-        
-            class CustomAttributes(NodeAttributes):
-                pass
-        
-            class CustomAttributesNode(NodeWithAttributes):
-                attributes_factory = CustomAttributes
-        
-        This factory is then used to instantiate the attributes:
-        
-        .. code-block:: pycon
-        
-            >>> node = CustomAttributesNode()
-            >>> node.attrs
-            <CustomAttributes object 'None' at ...>
-        
-        
-        Schema
-        ~~~~~~
-        
-        To describe the data types of node members, this package provides a mechanism
-        for defining schemata.
-        
-        This can happen in different ways. One is to define the schema for node members
-        directly. This is useful for nodes representing a leaf in the hierarchy or for
-        node attribute nodes:
-        
-        .. code-block:: python
-        
-            from node import schema
-            from node.base import BaseNode
-            from node.behaviors import DefaultInit
-            from node.behaviors import DictStorage
-            from node.behaviors import MappingNode
-            from node.behaviors import Schema
-            from plumber import plumbing
-        
-            @plumbing(
-                DefaultInit,
-                MappingNode,
-                DictStorage,
-                Schema)
-            class SchemaNode:
-                schema = {
-                    'int': schema.Int(),
-                    'float': schema.Float(default=1.),
-                    'str': schema.Str(),
-                    'bool': schema.Bool(default=False),
-                    'node': schema.Node(BaseNode)
-                }
-        
-        Children defined in the schema provide a default value. If not explicitely
-        defined, the default value is always ``node.utils.UNSET``:
-        
-        .. code-block:: pycon
-        
-            >>> node = SchemaNode()
-            >>> node['int']
-            <UNSET>
-        
-            >>> node['float']
-            1.0
-        
-            >>> node['bool']
-            False
-        
-        Children defined in the schema are validated against the defined type when
-        setting it's value:
-        
-        .. code-block:: pycon
-        
-            >>> node = SchemaNode()
-            >>> node['int'] = 'A'
-            Traceback (most recent call last):
-              ...
-            ValueError: A is no <class 'int'> type
-        
-        For accessing members defined in the schema as node attributes,
-        ``SchemaAsAttributes`` plumbing behavior can be used:
-        
-        .. code-block:: python
-        
-            from node.behaviors import SchemaAsAttributes
-        
-            @plumbing(SchemaAsAttributes)
-            class SchemaAsAttributesNode(BaseNode):
-                schema = {
-                    'int': schema.Int(default=1),
-                }
-        
-        Node ``attrs`` now provides access to the schema members:
-        
-        .. code-block:: pycon
-        
-            >>> node = SchemaAsAttributesNode()
-            >>> node.attrs['int']
-            1
-        
-        Schema members can also be defined as class attributes. This is syntactically
-        the most elegant way, but comes with the tradeoff of possible naming conflicts:
-        
-        .. code-block:: python
-        
-            from node.behaviors import SchemaProperties
-        
-            @plumbing(
-                DefaultInit,
-                MappingNode,
-                DictStorage,
-                SchemaProperties)
-            class SchemaPropertiesNode:
-                text = schema.Str(default='Text')
-        
-        Here we access ``text`` as class attribute:
-        
-        .. code-block:: pycon
-        
-            >>> node = SchemaPropertiesNode()
-            >>> node.text
-            'Text'
-        
-            >>> node.text = 1
-            Traceback (most recent call last):
-              ...
-            ValueError: 1 is no <class 'str'> type
-        
-        
-        Plumbing Behaviors
-        ------------------
-        
-        General Behaviors
-        ~~~~~~~~~~~~~~~~~
-        
-        **node.behaviors.DefaultInit**
-            Plumbing behavior providing default ``__init__`` function on node. This
-            behavior is going to be deprecated in future versions. Use
-            ``node.behaviors.NodeInit`` instead.
-            See ``node.interfaces.IDefaultInit``.
-        
-        **node.behaviors.NodeInit**
-            Plumbing behavior for transparent setting of ``__name__`` and ``__parent__``
-            at object initialization time.
-            See ``node.interfaces.INodeInit``.
-        
-        **node.behaviors.Node**
-            Fill in gaps for full INode API. See ``node.interfaces.INode``.
-        
-        **node.behaviors.ContentishNode**
-            A node which can contain children. See
-            ``node.interfaces.IContentishNode``. Concrete implementations are
-            ``node.behaviors.MappingNode`` and ``node.behaviors.SequenceNode``.
-        
-        **node.behaviors.Attributes**
-            Provide attributes on node. See ``node.interfaces.IAttributes``. If
-            ``node.behaviors.Nodespaces`` is applied on node, the attributes instance
-            gets stored internally in ``__attrs__`` nodespace, otherwise its set on
-            ``__attrs__`` attribute.
-        
-        **node.behaviors.Events**
-            Provide an event registration and dispatching mechanism.
-            See ``node.interfaces.IEvents``.
-        
-        **node.behaviors.BoundContext**
-            Mechanism for scoping objects to interfaces and classes.
-            See ``node.interfaces.IBoundContext``.
-        
-        **node.behaviors.NodeReference**
-            Plumbing behavior holding an index of nodes contained in the tree.
-            See ``node.interfaces.INodeReference``.
-        
-        **node.behaviors.WildcardFactory**
-            Plumbing behavior providing factories by wildcard patterns.
-            See ``node.interfaces.IWildcardFactory``.
-        
-        
-        Mapping Behaviors
-        ~~~~~~~~~~~~~~~~~
-        
-        **node.behaviors.MappingNode**
-            Turn an object into a mapping node. Extends ``node.behaviors.Node``.
-            See ``node.interfaces.IMappingNode``.
-        
-        **node.behaviors.MappingAdopt**
-            Plumbing behavior that provides ``__name__`` and ``__parent__`` attribute
-            adoption on child nodes of mapping.
-            See ``node.interfaces.IMappingAdopt``.
-        
-        **node.behaviors.MappingConstraints**
-            Plumbing behavior for constraints on mapping nodes.
-            See ``node.interfaces.IMappingConstraints``.
-        
-        **node.behaviors.UnicodeAware**
-            Plumbing behavior to ensure unicode for keys and string values.
-            See ``node.interfaces.IUnicodeAware``.
-        
-        **node.behaviors.Alias**
-            Plumbing behavior that provides aliasing of child keys.
-            See ``node.interfaces.IAlias``.
-        
-        **node.behaviors.AsAttrAccess**
-            Plumbing behavior to get node as IAttributeAccess implementation.
-            See ``node.interfaces.IAsAttrAccess``.
-        
-        **node.behaviors.ChildFactory**
-            Plumbing behavior providing child factories.
-            See ``node.interfaces.IChildFactory``.
-        
-        **node.behaviors.FixedChildren**
-            Plumbing Behavior that initializes a fixed dictionary as children.
-            See ``node.interfaces.IFixedChildren``.
-        
-        **node.behaviors.Nodespaces**
-            Plumbing behavior for providing nodespaces on node.
-            See ``node.interfaces.INodespaces``.
-        
-        **node.behaviors.Lifecycle**
-            Plumbing behavior taking care of lifecycle events.
-            See ``node.interfaces.ILifecycle``.
-        
-        **node.behaviors.AttributesLifecycle**
-            Plumbing behavior for handling lifecycle events on attribute manipulation.
-            See ``node.interfaces.IAttributesLifecycle``.
-        
-        **node.behaviors.Invalidate**
-            Plumbing behavior for node invalidation.
-            See ``node.interfaces.Invalidate``.
-        
-        **node.behaviors.VolatileStorageInvalidate**
-            Plumbing behavior for invalidating nodes using a volatile storage.
-            See ``node.interfaces.Invalidate``.
-        
-        **node.behaviors.Cache**
-            Plumbing behavior for caching.
-            See ``node.interfaces.ICache``.
-        
-        **node.behaviors.MappingOrder**
-            Plumbing behavior for ordering support on mapping nodes.
-            See ``node.interfaces.IMappingOrder``.
-        
-        **node.behaviors.UUIDAware**
-            Plumbing behavior providing a uuid on nodes.
-            See ``node.interfaces.IUUIDAware``.
-        
-        **node.behaviors.MappingReference**
-            Plumbing behavior to provide ``node.interfaces.INodeReference`` on mapping
-            nodes. See ``node.interfaces.IMappingReference``.
-        
-        **node.behaviors.MappingStorage**
-            Provide abstract mapping storage access.
-            See ``node.interfaces.IMappingStorage``.
-        
-        **node.behaviors.DictStorage**
-            Provide dictionary storage. Extends ``node.behaviors.MappingStorage``.
-            See ``node.interfaces.IMappingStorage``.
-        
-        **node.behaviors.OdictStorage**
-            Provide ordered dictionary storage. Extends
-            ``node.behaviors.MappingStorage``. See ``node.interfaces.IMappingStorage``.
-        
-        **node.behaviors.Fallback**
-            Provide a way to fall back to values by subpath stored on another node.
-            See ``node.interfaces.IFallback``.
-        
-        **node.behaviors.Schema**
-            Provide schema validation and value serialization on node values.
-            See ``node.interfaces.ISchema``.
-        
-        **node.behaviors.SchemaAsAttributes**
-            Provide schema validation and value serialization on node values via
-            dedicated attributes object.
-            See ``node.interfaces.ISchemaAsAttributes``.
-        
-        **node.behaviors.SchemaProperties**
-            Provide schema fields as class properties.
-            See ``node.interfaces.ISchemaProperties``.
-        
-        **node.behaviors.MappingFilter**
-            Filter mapping children by class or interface.
-            See ``node.interfaces.IChildFilter``.
-        
-        
-        Sequence Behaviors
-        ~~~~~~~~~~~~~~~~~~
-        
-        **node.behaviors.SequenceNode**
-            Turn an object into a sequence node. Extends ``node.behaviors.Node``.
-            See ``node.interfaces.IMappingNode``.
-        
-        **node.behaviors.SequenceAdopt**
-            Plumbing behavior that provides ``__name__`` and ``__parent__`` attribute
-            adoption on child nodes of sequence.
-            See ``node.interfaces.ISequenceAdopt``.
-        
-        **node.behaviors.SequenceConstraints**
-            Plumbing behavior for constraints on sequence nodes.
-            See ``node.interfaces.ISequenceConstraints``.
-        
-        **node.behaviors.SequenceStorage**
-            Provide abstract sequence storage access.
-            See ``node.interfaces.ISequenceStorage``.
-        
-        **node.behaviors.ListStorage**
-            Provide list storage. See ``node.interfaces.ISequenceStorage``.
-        
-        **node.behaviors.SequenceReference**
-            Plumbing behavior to provide ``node.interfaces.INodeReference`` on sequence
-            nodes. See ``node.interfaces.ISequenceReference``.
-        
-        **node.behaviors.SequenceFilter**
-            Filter sequence children by class or interface.
-            See ``node.interfaces.IChildFilter``.
-        
-        **node.behaviors.SequenceOrder**
-            Plumbing behavior for ordering support on sequence nodes.
-            See ``node.interfaces.ISequenceOrder``.
-        
-        
-        JSON Serialization
-        ------------------
-        
-        Nodes can be serialized to and deserialized from JSON:
-        
-        .. code-block:: pycon
-        
-            >>> from node.serializer import serialize
-            >>> json_dump = serialize(BaseNode(name='node'))
-        
-            >>> from node.serializer import deserialize
-            >>> deserialize(json_dump)
-            <BaseNode object 'node' at ...>
-        
-        For details on serialization API please read file in
-        ``docs/archive/serializer.rst``.
-        
-        
-        Python Versions
-        ---------------
-        
-        - Python 2.7, 3.7+
-        - May work with other versions (untested)
-        
-        
-        Contributors
-        ============
-        
-        - Robert Niederreiter
-        - Florian Friesdorf
-        - Jens Klein
-        
-        
-        
-        Changes
-        =======
-        
-        1.2 (2022-12-05)
-        ----------------
-        
-        - Do not overwrite ``uuid`` in ``node.behaviors.UUIDAware.__init__`` if
-          ``uuid`` already set.
-          [rnix]
-        
-        - Rename ``node.interfaces.IOrder`` to ``node.interfaces.IMappingOrder``
-          and ``node.behaviors.Order`` to ``node.behaviors.MappingOrder``.
-          B/C is kept.
-          [rnix]
-        
-        - Introduce ``node.behaviors.ISequenceOrder`` and
-          ``node.interfaces.SequenceOrder``.
-          [rnix]
-        
-        - Introduce ``node.interfaces.INodeOrder``. Used as base for
-          ``node.interfaces.IMappingOrder`` and ``node.interfaces.ISequenceOrder``.
-          [rnix]
-        
-        - Add rich comparison functions ``__lt__``, ``__le__``, ``__gt__`` and
-          ``__ge__`` to ``node.utils.Unset``.
-          [rnix]
-        
-        **Breaking changes**:
-        
-        - Importing B/C ``Order`` behavior from ``node.behaviors.order``
-          not works any more. Please import from ``node.behaviors``.
-          [rnix]
-        
-        
-        1.1 (2022-10-06)
-        ----------------
-        
-        - Add ``node.schema.DateTime``, ``node.schema.DateTimeSerializer`` and
-          ``node.schema.datetime_serializer``.
-          [rnix]
-        
-        - Subclass ``threading.local`` for
-          ``node.behaviors.lifecycle._lifecycle_context``,
-          ``node.behaviors.events._attribute_subscribers`` and
-          ``node.behaviors.schema._schema_property`` objects in order to safely provide
-          default values.
-          [rnix]
-        
-        - Introduce ``node.interfaces.IChildFilter``, ``node.behaviors.MappingFilter``
-          and ``node.behaviors.SequenceFilter``.
-          [rnix]
-        
-        - Introduce ``node.interfaces.IWildcardFactory`` and
-          ``node.behaviors.WildcardFactory``.
-          [rnix]
-        
-        - Introduce ``node.interfaces.INodeInit`` and ``node.behaviors.NodeInit``.
-          [rnix]
-        
-        - Deprecate ``IFixedChildren.fixed_children_factories`` Use
-          ``IFixedChildren.factories`` instead.
-          [rnix]
-        
-        - Introduce ``node.interfaces.IContentishNode`` and
-          ``node.behaviors.ContentishNode``. Use as base for mapping and sequence nodes.
-          [rnix]
-        
-        - ``insertbefore``, ``insertafter`` and ``swap`` in ``node.behaviors.Order``
-          alternatively accept node names as arguments where possible.
-          [rnix]
-        
-        - ``insertbefore``, ``insertafter``, and ``insertfirst`` and ``insertlast`` in
-          ``node.behaviors.Order`` internally use ``movebefore``, ``moveafter``,
-          ``movefirst`` and ``movelast`` of ``odict`` to avoid modifying the data
-          structure before ``__setitem__`` gets called.
-          [rnix]
-        
-        - Extend ``node.interfaces.IOrder``  respective ``node.behaviors.Order``
-          by ``movebefore``, ``moveafter``, ``movefirst`` and ``movelast``.
-          [rnix]
-        
-        - Reset ``__parent__`` in ``node.behaviors.Node.detach``. Node is no longer
-          contained in tree.
-          [rnix]
-        
-        - Introduce ``IndexViolationError`` which inherits from ``ValueError`` and
-          raise it in reference related behaviors instead of ``ValueError`` where
-          appropriate.
-          [rnix]
-        
-        - Introduce ``node.interfaces.INodeReference`` and
-          ``node.behaviors.NodeReference``.
-          [rnix]
-        
-        - Introduce ``node.interfaces.ISequenceReference`` and
-          ``node.behaviors.SequenceReference``.
-          [rnix]
-        
-        - Rename ``node.interfaces.IReference`` to ``node.interfaces.IMappingReference``
-          and ``node.behaviors.Reference`` to ``node.behaviors.MappingReference``.
-          B/C is kept.
-          [rnix]
-        
-        **Breaking changes**:
-        
-        - Remove ``_notify_suppress`` flag from ``Lifecycle`` behavior. Introduce
-          ``suppress_lifecycle_events`` contextmanager as substitute.
-          [rnix]
-        
-        - Importing ``ChildFactory`` and ``FixedChildren`` from
-          ``node.behaviors.common`` not works any more. Please import from
-          ``node.behaviors``.
-          [rnix]
-        
-        - Importing B/C ``Reference`` behavior from ``node.behaviors.reference``
-          not works any more. Please import from ``node.behaviors``.
-          [rnix]
-        
-        
-        1.0 (2022-03-17)
-        ----------------
-        
-        - Implement ``__copy__`` and ``__deepcopy__`` on ``node.utils.UNSET``.
-          [rnix]
-        
-        - Introduce ``node.interfaces.ISequenceConstraints`` and
-          ``node.behaviors.SequenceConstraints``.
-          [rnix]
-        
-        - Rename ``node.interfaces.INodeChildValidate`` to
-          ``node.interfaces.IMappingConstraints`` and
-          ``node.behaviors.NodeChildValidate`` to ``node.behaviors.MappingConstraints``.
-          ``MappingConstraints`` implementation moved from ``node.behaviors.common`` to
-          ``node.behaviors.constraints``. B/C is kept.
-          [rnix]
-        
-        - Introduce ``node.interfaces.ISequenceAdopt`` and
-          ``node.behaviors.SequenceAdopt``.
-          [rnix]
-        
-        - ``MappingAdopt`` now catches all exceptions instead of only
-          ``AttributeError``, ``KeyError`` and ``ValueError``.
-          [rnix]
-        
-        - Rename ``node.interfaces.IAdopt`` to ``node.interfaces.IMappingAdopt`` and
-          ``node.behaviors.Adopt`` to ``node.behaviors.MappingAdopt``. ``MappingAdopt``
-          implementation moved from ``node.behaviors.common`` to
-          ``node.behaviors.adopt``. B/C is kept.
-          [rnix]
-        
-        - ``node.behaviors.Attributes`` now also works if
-          ``node.behaviors.Nodespaces`` is not applied.
-          [rnix]
-        
-        - Introduce ``node.behaviors.Node`` which implements only
-          ``node.interfaces.INode`` contract. It is used as base for
-          ``node.behaviors.MappingNode`` and ``node.behaviors.SequcneNode``.
-          [rnix]
-        
-        - Do not inherit ``node.interfaces.INode`` from
-          ``zope.interfaces.common.mapping.IFullMapping`` any more. Data model specific
-          interfaces are added now via ``node.interfaces.IMappingNode`` and
-          ``node.interfaces.ISequenceNode``.
-          [rnix]
-        
-        - Introduce sequence nodes. Sequence nodes are implemented via
-          ``node.behaviors.SequcneNode`` and ``node.behaviors.ListStorage``.
-          [rnix]
-        
-        - Rename ``node.interfaces.INodify`` to ``node.interfaces.IMappingNode`` and
-          ``node.behaviors.Nodify`` to ``node.behaviors.MappingNode``. ``MappingNode``
-          implementation moved from ``node.behaviors.nodify`` to
-          ``node.behaviors.mapping``. B/C is kept.
-          [rnix]
-        
-        - Rename ``node.interfaces.IStorage`` to ``node.interfaces.IMappingStorage``
-          and ``node.behaviors.Storage`` to ``node.behaviors.Storage``. B/C is kept.
-          [rnix]
-        
-        - Add key and value type validation to schema fields where appropriate.
-          [rnix]
-        
-        - Introduce serializer support to schema fields. Add a couple of concrete field
-          serializer implementations to ``node.schema.serializer``.
-          [rnix]
-        
-        - Add ``ODict`` and ``Node`` schema fields to ``node.schema.fields``.
-          [rnix]
-        
-        - Add ``node.schema.fields.IterableField`` and use as base class for
-          ``List``, ``Tuple`` and ``Set`` schema fields.
-        
-        - Introduce ``node.behaviors.schema.SchemaProperties`` plumbing behavior.
-          [rnix]
-        
-        - Split up ``node.schema`` module into a package.
-          [rnix]
-        
-        - Introduce ``node.behaviors.context.BoundContext`` plumbing behavior.
-          [rnix]
-        
-        **Breaking changes**:
-        
-        - Remove ``node.behaviors.GetattrChildren``. See ``node.utils.AttributeAccess``
-          instead if you need to access node children via ``__getattr__``.
-          [rnix]
-        
-        - Importing B/C ``Adopt`` behavior from ``node.behaviors.common``
-          not works any more. Please import from ``node.behaviors``.
-          [rnix]
-        
-        - Importing B/C ``NodeChildValidate`` behavior from ``node.behaviors.common``
-          not works any more. Please import from ``node.behaviors``.
-          [rnix]
-        
-        - Importing B/C ``Nodify`` behavior from ``node.behaviors.nodify``
-          not works any more. Please import from ``node.behaviors``.
-          [rnix]
-        
-        - Remove deprecated B/C import location ``node.parts``.
-          [rnix]
-        
-        - ``node.behaviors.schema.Schema`` no longer considers wildcard fields.
-          [rnix]
-        
-        - ``node.behaviors.schema.Schema.__setitem__`` deletes value from related
-          storage for field if value is ``node.utils.UNSET``.
-          [rnix]
-        
-        - ``node.behaviors.schema.Schema.__getitem__`` always returns default value for
-          field instead of raising ``KeyError`` if no default is set.
-          [rnix]
-        
-        - Default value of ``node.schema.fields.Field.default`` is ``node.utils.UNSET``
-          now.
-          [rnix]
-        
-        - ``node.schema.fields.Field.validate`` raises exception if validation fails
-          instead of returning boolean.
-          [rnix]
-        
-        
-        0.9.28 (2021-11-08)
-        -------------------
-        
-        - Add missing ``node.interfaces.INodeAttributes`` interface.
-          [rnix]
-        
-        - Add missing ``attribute_access_for_attrs`` attribute to ``IAttributes``
-          interface.
-          [rnix]
-        
-        - Rename ``node.behaviors.common.NodeChildValidate.allow_non_node_childs``
-          to ``allow_non_node_children``. A Deprecation warning is printed if the
-          old attribute is used.
-          [rnix]
-        
-        - Introduce ``node.behaviors.schema.Schema``,
-          ``node.behaviors.schema.SchemaAsAttributes`` and related schema definitions
-          in ``node.schema``.
-          [rnix]
-        
-        
-        0.9.27 (2021-10-21)
-        -------------------
-        
-        - Expose ``first_key``, ``last_key``, ``next_key`` and ``prev_key`` from
-          odict storage on ``Order`` behavior.
-          [rnix, 2021-10-21]
-        
-        - Add basic serializer settings mechanism.
-          [rnix, 2021-07-20]
-        
-        
-        0.9.26 (2021-05-10)
-        -------------------
-        
-        - Use ``node.utils.safe_decode`` in ``node.behaviors.nodify.Nodify.treerepr``.
-          [rnix, 2021-05-04]
-        
-        - Add ``node.utils.safe_encode`` and ``node.utils.safe_decode``.
-          [rnix, 2021-05-04]
-        
-        
-        0.9.25 (2020-03-30)
-        -------------------
-        
-        - Introduce ``uuid_factory`` function on ``node.interfaces.IUUIDAware`` and
-          implement default function in ``node.behaviors.common.UUIDAware``.
-          [rnix, 2020-03-01]
-        
-        - Rename ``NodeTestCase.expect_error`` to ``NodeTestCase.expectError``.
-          [rnix, 2019-09-04]
-        
-        - Rename ``NodeTestCase.check_output`` to ``NodeTestCase.checkOutput``.
-          [rnix, 2019-09-04]
-        
-        - Introduce ``prefix`` keyword argument in ``Nodify.treerepr``.
-          [rnix, 2019-09-04]
-        
-        
-        0.9.24 (2019-07-10)
-        -------------------
-        
-        - Overhaul ``node.behaviors.Order``. Use related functions from ``odict`` where
-          appropriate.
-          [rnix, 2019-07-10]
-        
-        - Remove superfluous ``extra_require`` from ``setup.py``.
-          [rnix, 2019-04-25]
-        
-        - Drop Support for python < 2.7 and < 3.3.
-          [rnix, 2019-04-25]
-        
-        
-        0.9.23 (2018-11-07)
-        -------------------
-        
-        - Use property decorators for ``node.behaviors.reference.Reference.uuid``.
-          [rnix, 2017-12-15]
-        
-        
-        0.9.22 (2017-07-18)
-        -------------------
-        
-        - Add ``always_dispatch`` keyword argument to
-          ``node.behaviors.events.EventAttribute`` constructor which defines whether
-          events are always dispatched on ``__set__``, not only if attribute value
-          changes.
-          [rnix, 2017-06-20]
-        
-        - Use ``node.utils.UNSET`` as default ``default`` value in
-          ``node.behaviors.events.EventAttribute.__init__``.
-          [rnix, 2017-06-19]
-        
-        - Introduce ``node.behaviors.events.EventAttribute.subscriber`` decorator which
-          can be used to register attribute subscribers.
-          [rnix, 2017-06-19]
-        
-        - Move event dispatching related classes and functions from ``node.events``
-          to ``node.behaviors.events`` and import it from there in ``node.events``.
-          [rnix, 2017-06-16]
-        
-        - Introduce ``node.interfaces.IEvents`` and implement
-          ``node.behaviors.events.Events`` behavior. Contains business logic from
-          ``node.events.EventDispatcher``. Use new behavior on ``EventDispatcher``.
-          [rnix, 2017-06-16]
-        
-        - Create ``suppress_events`` context manager which can be used to
-          suppress event notification in conjunction with ``node.behaviors.Events``
-          behavior.
-          [rnix, 2017-06-15]
-        
-        - Create ``node.behaviors.fallback.fallback_processing`` context manager and
-          and use it in ``node.behaviors.fallback.Fallback.__getitem__`` to check
-          whether fallback processing is active.
-          [rnix, 2017-06-15]
-        
-        
-        0.9.21 (2017-06-15)
-        -------------------
-        
-        - Introduce ``node.events.EventDispatcher`` and ``node.events.EventAttribute``.
-          [rnix, 2017-06-15]
-        
-        - Use ``setattr`` in ``instance_property`` decorator instead of
-          ``object.__setattr__`` in order to avoid errors with custom low level
-          ``__setattr__`` implementations.
-          [rnix, 2017-06-14]
-        
-        
-        0.9.20 (2017-06-07)
-        -------------------
-        
-        - Type cast sort key to ``node.compat.UNICODE_TYPE`` in
-          ``node.behaviors.Nodify.treerepr`` to avoid unicode decode errors.
-          [rnix, 2017-06-07]
-        
-        
-        0.9.19 (2017-06-07)
-        -------------------
-        
-        - Python 3 and pypy compatibility.
-          [rnix, 2017-06-02]
-        
-        - Drop support for Python < 2.7.
-          [rnix, 2017-06-02]
-        
-        - Add ``__bool__`` to ``node.behaviors.Nodify``.
-          [rnix, 2017-06-02]
-        
-        - Add ``__bool__`` to ``node.utils.UNSET``.
-          [rnix, 2017-06-02]
-        
-        - Add ``treerepr`` in ``node.behaviors.nodify.Nodify`` and move code from
-          ``printtree`` to it. Returs tree representation as string instead of printing
-          it. ``printtree`` uses ``treerepr`` now. As enhancement ``treerepr`` sorts
-          children of node if it does not implement ``IOrdered`` in order to ensure
-          consistend output which can be used to write tests against.
-          [rnix, 2017-06-02]
-        
-        - Use ``object.__getattribute__`` explicitely in
-          ``node.utils.instance_property`` to check whether property value already has
-          been computed in order to avoid problems when oberwriting ``__getattr__``
-          on classes using ``instance_property`` decorator.
-          [rnix, 2017-06-02]
-        
-        
-        0.9.18.1 (2017-02-23)
-        ---------------------
-        
-        - Fix permissions.
-          [rnix, 2017-02-23]
-        
-        
-        0.9.18 (2017-02-14)
-        -------------------
-        
-        - Add ``node.utils.node_by_path``.
-          [rnix, 2017-02-07]
-        
-        - Do not depend on ``unittest2`` since its is not used.
-          [jensens, 2017-01-17]
-        
-        - Add ``node.behaviors.Fallback`` behavior.
-          [jensens, 2017-01-17]
-        
-        
-        0.9.17 (2017-01-17)
-        -------------------
-        
-        - Add basic JSON serializer and deserializer.
-          [rnix, 2016-12-03]
-        
-        
-        0.9.16 (2015-10-08)
-        -------------------
-        
-        - Only encode name in ``node.behaviors.nodify.Nodify.__repr__`` and
-          ``node.behaviors.nodify.Nodify.noderepr`` if name is unicode instance.
-          [rnix, 2015-10-03]
-        
-        - Improve ``node.behaviors.nodify.Nodify.printtree``. None node children are
-          printed with key.
-          [rnix, 2015-10-03]
-        
-        
-        0.9.15 (2014-12-17)
-        -------------------
-        
-        - Fix dependency declaration to ``odict`` in order to make setuptools 8.x+
-          happy; using ``>=`` instead of ``>`` now.
-          [jensens, 2014-12-17]
-        
-        
-        0.9.14
-        ------
-        
-        - use ``plumbing`` decorator instead of ``plumber`` metaclass.
-          [rnix, 2014-07-31]
-        
-        
-        0.9.13
-        ------
-        
-        - Introduce ``node.behaviors.cache.VolatileStorageInvalidate``.
-          [rnix, 2014-01-15]
-        
-        
-        0.9.12
-        ------
-        
-        - Add ``zope.component`` to install dependencies.
-          [rnix, 2013-12-09]
-        
-        
-        0.9.11
-        ------
-        
-        - Use ``node.utils.UNSET`` instance in
-          ``node.behaviors.mapping.ExtendedWriteMapping.pop``.
-          [rnix, 2013-02-10]
-        
-        - Improve ``node.utils.Unset``. Add ``Unset`` instance at
-          ``node.utils.UNSET``.
-          [rnix, 2013-02-10]
-        
-        
-        0.9.10
-        ------
-        
-        - Fix ``node.utils.StrCodec.encode`` to return value as is if str and decoding
-          failed.
-          [rnix, 2012-11-07]
-        
-        
-        0.9.9
-        -----
-        
-        - Python 2.7 compatibility.
-          [rnix, 2012-10-15]
-        
-        - Remove ``zope.component.event`` B/C.
-          [rnix, 2012-10-15]
-        
-        - Remove ``zope.location`` B/C.
-          [rnix, 2012-10-15]
-        
-        - Remove ``zope.lifecycleevent`` B/C.
-          [rnix, 2012-10-15]
-        
-        - Pep8.
-          [rnix, 2012-10-15]
-        
-        
-        0.9.8
-        -----
-        
-        - Deprecate the use of ``node.parts``. Use ``node.behaviors`` instead.
-          [rnix, 2012-07-28]
-        
-        - Adopt to ``plumber`` 1.2
-          [rnix, 2012-07-28]
-        
-        
-        0.9.7
-        -----
-        
-        - Introduce ``node.interfaces.IOrdered`` Marker interface. Set this interface
-          on ``node.parts.storage.OdictStorage``.
-          [rnix, 2012-05-21]
-        
-        - ``node.parts.mapping.ClonableMapping`` now supports ``deepcopy``.
-          [rnix, 2012-05-18]
-        
-        - Use ``zope.interface.implementer`` instead of ``zope.interface.implements``
-          all over the place.
-          [rnix, 2012-05-18]
-        
-        - Remove superfluos interfaces.
-          [rnix, 2012-05-18]
-        
-        - Remove ``Zodict`` from ``node.utils``.
-          [rnix, 2012-05-18]
-        
-        - Remove ``AliasedNodespace``, use ``Alias`` part instead.
-          [rnix, 2012-05-18]
-        
-        - Move aliaser objects from ``node.aliasing`` to ``node.parts.alias``.
-          [rnix, 2012-05-18]
-        
-        - Remove ``composition`` module.
-          [rnix, 2012-05-18]
-        
-        - Remove ``bbb`` module.
-          [rnix, 2012-05-18]
-        
-        
-        0.9.6
-        -----
-        
-        - Do not inherit ``node.parts.Reference`` from ``node.parts.UUIDAware``.
-          [rnix, 2012-01-30]
-        
-        - Set ``uuid`` in ``node.parts.Reference.__init__`` plumb.
-          [rnix, 2012-01-30]
-        
-        
-        0.9.5
-        -----
-        
-        - add ``node.parts.nodify.Nodify.acquire`` function.
-          [rnix, 2011-12-05]
-        
-        - add ``node.parts.ChildFactory`` plumbing part.
-          [rnix, 2011-12-04]
-        
-        - add ``node.parts.UUIDAware`` plumbing part.
-          [rnix, 2011-12-02]
-        
-        - fix ``node.parts.Order.swap`` in order to work with pickled nodes.
-          [rnix, 2011-11-28]
-        
-        - use ``node.name`` instead of ``node.__name__`` in
-          ``node.parts.nodify.Nodify.path``.
-          [rnix, 2011-11-17]
-        
-        - add ``swap`` to  ``node.parts.Order``.
-          [rnix, 2011-10-05]
-        
-        - add ``insertfirst`` and ``insertlast`` to ``node.parts.Order``.
-          [rnix, 2011-10-02]
-        
-        
-        0.9.4
-        -----
-        
-        - add ``node.utils.debug`` decorator.
-          [rnix, 2011-07-23]
-        
-        - remove non storage contract specific properties from
-          ``node.aliasing.AliasedNodespace``
-          [rnix, 2011-07-18]
-        
-        - ``node.aliasing`` test completion
-          [rnix, 2011-07-18]
-        
-        - Add non strict functionality to ``node.aliasing.DictAliaser`` for accessing
-          non aliased keys as is as fallback
-          [rnix, 2011-07-18]
-        
-        - Consider ``INode`` implementing objects in ``node.utils.StrCodec``
-          [rnix, 2011-07-16]
-        
-        - Remove duplicate implements in storage parts
-          [rnix, 2011-05-16]
-        
-        
-        0.9.3
-        -----
-        
-        - Increase test coverage
-          [rnix, 2011-05-09]
-        
-        - Add interfaces ``IFixedChildren`` and ``IGetattrChildren`` for related parts.
-          [rnix, 2011-05-09]
-        
-        - Rename ``Unicode`` part to ``UnicodeAware``.
-          [rnix, 2011-05-09]
-        
-        - Add ``node.utils.StrCodec``.
-          [rnix, 2011-05-09]
-        
-        - Inherit ``INodify`` interface from ``INode``.
-          [rnix, 2011-05-08]
-        
-        - Locking tests. Add ``time.sleep`` after thread start.
-          [rnix, 2011-05-08]
-        
-        - Cleanup ``BaseTester``, remove ``sorted_output`` flag (always sort), also
-          search class bases for detection in ``wherefrom``.
-          [rnix, 2011-05-08]
-        
-        - Remove useless try/except in ``utils.AttributeAccess``.
-          [rnix, 2011-05-08]
-        
-        - Add ``instance_property`` decorator to utils.
-          [rnix, 2011-05-06]
-        
-        - Add ``FixedChildren`` and ``GetattrChildren`` parts.
-          [chaoflow, 2011-04-22]
-        
-        
-        0.9.2
-        -----
-        
-        - Add ``__nonzero__`` on ``Nodifiy`` part always return True.
-          [rnix, 2011-03-15]
-        
-        
-        0.9.1
-        -----
-        
-        - Provide ``node.base.Node`` with same behavior like ``zodict.Node`` for
-          migration purposes.
-          [rnix, 2011-02-08]
-        
-        
-        0.9
-        ---
-        
-        - Make it work [rnix, chaoflow, et al]
-        
-        
-        License
-        =======
-        
-        Copyright (c) 2009-2021, BlueDynamics Alliance, Austria
-        Copyright (c) 2021-2022, Node Contributors
-        All rights reserved.
-        
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        * Redistributions of source code must retain the above copyright notice, this
-          list of conditions and the following disclaimer.
-        
-        * Redistributions in binary form must reproduce the above copyright notice, this
-          list of conditions and the following disclaimer in the documentation and/or
-          other materials provided with the distribution.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-        ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-        WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
-        ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-        (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-        LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
-        ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-        (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-        SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-        
 Keywords: node tree fullmapping dict
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE.rst
+
+Node
+====
+
+.. image:: https://img.shields.io/pypi/v/node.svg
+    :target: https://pypi.python.org/pypi/node
+    :alt: Latest PyPI version
+
+.. image:: https://img.shields.io/pypi/dm/node.svg
+    :target: https://pypi.python.org/pypi/node
+    :alt: Number of PyPI downloads
+
+.. image:: https://github.com/conestack/node/actions/workflows/test.yaml/badge.svg
+    :target: https://github.com/conestack/node/actions/workflows/test.yaml
+    :alt: Test node
+
+
+Overview
+--------
+
+Node is a library to create nested data models and structures.
+
+These data models are described as trees of nodes, optionally with attributes
+and schema definitions.
+
+They utilize:
+
+- Python's
+  `mapping and sequence API's <http://docs.python.org/reference/datamodel.html>`_
+  for accessing node members.
+- The contract of
+  `zope.location.interfaces.ILocation <https://zopelocation.readthedocs.io/en/latest/api.html#zope.location.interfaces.ILocation>`_
+  for hierarchy information.
+
+One purpose of this package is to provide a unified API to different backend
+storages. Specific storage related implementations are for example:
+
+- `node.ext.fs <https://pypi.org/project/node.ext.fs>`_
+- `node.ext.ldap <https://pypi.org/project/node.ext.ldap>`_
+- `node.ext.yaml <https://pypi.org/project/node.ext.yaml>`_
+- `node.ext.zodb <https://pypi.org/project/node.ext.zodb>`_
+
+Another usecase is providing interfaces for specific application domains.
+
+E.g. for user and group management,
+`node.ext.ugm <https://pypi.org/project/node.ext.ugm>`_ defines the interfaces.
+Additional it implements a file based default implementation. Then there are
+specific implementations of those interfaces in
+`node.ext.ldap <https://pypi.org/project/node.ext.ldap>`_ and
+`cone.sql <https://pypi.org/project/cone.sql>`_, to access users and groups in
+LDAP and SQL databases.
+
+This package is also used to build in-memory models of all sorts.
+
+E.g.  `yafowil <https://pypi.org/project/yafowil>`_ is a HTML form processing
+and rendering library. It uses node trees for declarative description of the
+form model.
+
+Another one to mention is `cone.app <https://pypi.org/project/cone.app>`_,
+a `Pyramid <https://pypi.org/project/pyramid>`_ based development environment
+for web applications, which uses node trees to describe the application model.
+
+
+Basic Usage
+-----------
+
+There are two basic node types. Mapping nodes and sequence nodes. This
+package provides some basic nodes to start from.
+
+
+Mapping Nodes
+~~~~~~~~~~~~~
+
+Mapping nodes implement ``node.interfaces.IMappingNode``. A mapping in python
+is a container object that supports arbitrary key lookups and implements the
+methods specified in the ``MutableMapping`` of pythons abstract base classes
+respective ``zope.interface.common.mapping.IFullMapping``.
+
+An unordered node. This can be used as base for trees where order of items
+doesn't matter:
+
+.. code-block:: python
+
+    from node.base import BaseNode
+
+    root = BaseNode(name='root')
+    root['child'] = BaseNode()
+
+An ordered node. The order of items is preserved:
+
+.. code-block:: python
+
+    from node.base import OrderedNode
+
+    root = OrderedNode(name='orderedroot')
+    root['foo'] = OrderedNode()
+    root['bar'] = OrderedNode()
+
+With ``printtree`` we can do a quick inspection of our node tree:
+
+.. code-block:: pycon
+
+    >>> root.printtree()
+    <class 'node.base.OrderedNode'>: orderedroot
+      <class 'node.base.OrderedNode'>: foo
+      <class 'node.base.OrderedNode'>: bar
+
+
+Sequence Nodes
+~~~~~~~~~~~~~~
+
+Sequence nodes implement ``node.interfaces.ISequenceNode``. In the context
+of this library, a sequence is an implementation of the methods
+specified in the ``MutableSequence`` of pythons abstract base classes respective
+``zope.interface.common.collections.IMutableSequence``.
+
+Using a list node:
+
+.. code-block:: python
+
+    from node.base import BaseNode
+    from node.base import ListNode
+
+    root = ListNode(name='listroot')
+    root.insert(0, BaseNode())
+    root.insert(1, BaseNode())
+
+Check tree structure with ``printtree``:
+
+.. code-block:: pycon
+
+    >>> root.printtree()
+    <class 'node.base.ListNode'>: listnode
+      <class 'node.base.BaseNode'>: 0
+      <class 'node.base.BaseNode'>: 1
+
+.. note::
+
+    Sequence nodes are introduced as of node 1.0 and are not as feature rich
+    as mapping nodes (yet). If you find inconsistencies or missing features,
+    please file an issue or create a pull request at github.
+
+
+Behaviors
+~~~~~~~~~
+
+``node`` utilizes the `plumber <http://pypi.python.org/pypi/plumber>`_ package.
+
+The different functionalities of nodes are provided as plumbing behaviors:
+
+.. code-block:: python
+
+    from node.behaviors import DefaultInit
+    from node.behaviors import MappingNode
+    from node.behaviors import OdictStorage
+    from plumber import plumbing
+
+    @plumbing(
+        DefaultInit,
+        MappingNode,
+        OdictStorage)
+    class CustomNode:
+        pass
+
+When inspecting the ``CustomNode`` class, we can see it was plumbed using given
+behaviors, now representing a complete node implementation:
+
+.. code-block:: pycon
+
+    >>> dir(CustomNode)
+    ['__bool__', '__class__', '__contains__', '__delattr__', '__delitem__',
+    '__dict__', '__dir__', '__doc__', '__eq__', '__format__', '__ge__',
+    '__getattribute__', '__getitem__', '__gt__', '__hash__', '__implemented__',
+    '__init__', '__init_subclass__', '__iter__', '__le__', '__len__', '__lt__',
+    '__module__', '__name__', '__ne__', '__new__', '__nonzero__', '__parent__',
+    '__plumbing__', '__plumbing_stacks__', '__provides__', '__reduce__',
+    '__reduce_ex__', '__repr__', '__setattr__', '__setitem__', '__sizeof__',
+    '__str__', '__subclasshook__', '__weakref__', 'acquire', 'clear', 'copy',
+    'deepcopy', 'detach', 'filtereditems', 'filtereditervalues', 'filteredvalues',
+    'get', 'has_key', 'items', 'iteritems', 'iterkeys', 'itervalues', 'keys',
+    'name', 'noderepr', 'parent', 'path', 'pop', 'popitem', 'printtree', 'root',
+    'setdefault', 'storage', 'treerepr', 'update', 'values']
+
+Please read the documentation of ``plumber`` for detailed information about the
+plumbing system.
+
+
+Attributes
+~~~~~~~~~~
+
+While it is not strictly necessary, it's a good idea to separate the
+hierarchical structure of a model from the node related attributes to avoid
+naming conflicts. Attributes are provided via ``node.behaviors.Attributes``
+plumbing behavior:
+
+.. code-block:: python
+
+    from node.behaviors import Attributes
+    from node.behaviors import DefaultInit
+    from node.behaviors import DictStorage
+    from node.behaviors import MappingNode
+    from plumber import plumbing
+
+    @plumbing(
+        Attributes,
+        DefaultInit,
+        MappingNode,
+        DictStorage)
+    class NodeWithAttributes:
+        pass
+
+The node now provides an ``attrs`` attribute. Node attributes are itself just
+a node:
+
+.. code-block:: pycon
+
+    >>> node = NodeWithAttributes()
+    >>> attrs = node.attrs
+    >>> attrs
+    <NodeAttributes object 'None' at ...>
+
+    >>> attrs['foo'] = 'foo'
+
+If it's desired to access attribute members via python attribute access,
+``attribute_access_for_attrs`` must be set on node:
+
+.. code-block:: pycon
+
+    >>> node.attribute_access_for_attrs = True
+    >>> attrs = node.attrs
+    >>> attrs.foo = 'bar'
+    >>> attrs.foo
+    'bar'
+
+A custom attributes implementation can be set by defining
+``attributes_factory`` on the node:
+
+.. code-block:: python
+
+    from node.behaviors import NodeAttributes
+
+    class CustomAttributes(NodeAttributes):
+        pass
+
+    class CustomAttributesNode(NodeWithAttributes):
+        attributes_factory = CustomAttributes
+
+This factory is then used to instantiate the attributes:
+
+.. code-block:: pycon
+
+    >>> node = CustomAttributesNode()
+    >>> node.attrs
+    <CustomAttributes object 'None' at ...>
+
+
+Schema
+~~~~~~
+
+To describe the data types of node members, this package provides a mechanism
+for defining schemata.
+
+This can happen in different ways. One is to define the schema for node members
+directly. This is useful for nodes representing a leaf in the hierarchy or for
+node attribute nodes:
+
+.. code-block:: python
+
+    from node import schema
+    from node.base import BaseNode
+    from node.behaviors import DefaultInit
+    from node.behaviors import DictStorage
+    from node.behaviors import MappingNode
+    from node.behaviors import Schema
+    from plumber import plumbing
+
+    @plumbing(
+        DefaultInit,
+        MappingNode,
+        DictStorage,
+        Schema)
+    class SchemaNode:
+        schema = {
+            'int': schema.Int(),
+            'float': schema.Float(default=1.),
+            'str': schema.Str(),
+            'bool': schema.Bool(default=False),
+            'node': schema.Node(BaseNode)
+        }
+
+Children defined in the schema provide a default value. If not explicitely
+defined, the default value is always ``node.utils.UNSET``:
+
+.. code-block:: pycon
+
+    >>> node = SchemaNode()
+    >>> node['int']
+    <UNSET>
+
+    >>> node['float']
+    1.0
+
+    >>> node['bool']
+    False
+
+Children defined in the schema are validated against the defined type when
+setting it's value:
+
+.. code-block:: pycon
+
+    >>> node = SchemaNode()
+    >>> node['int'] = 'A'
+    Traceback (most recent call last):
+      ...
+    ValueError: A is no <class 'int'> type
+
+For accessing members defined in the schema as node attributes,
+``SchemaAsAttributes`` plumbing behavior can be used:
+
+.. code-block:: python
+
+    from node.behaviors import SchemaAsAttributes
+
+    @plumbing(SchemaAsAttributes)
+    class SchemaAsAttributesNode(BaseNode):
+        schema = {
+            'int': schema.Int(default=1),
+        }
+
+Node ``attrs`` now provides access to the schema members:
+
+.. code-block:: pycon
+
+    >>> node = SchemaAsAttributesNode()
+    >>> node.attrs['int']
+    1
+
+Schema members can also be defined as class attributes. This is syntactically
+the most elegant way, but comes with the tradeoff of possible naming conflicts:
+
+.. code-block:: python
+
+    from node.behaviors import SchemaProperties
+
+    @plumbing(
+        DefaultInit,
+        MappingNode,
+        DictStorage,
+        SchemaProperties)
+    class SchemaPropertiesNode:
+        text = schema.Str(default='Text')
+
+Here we access ``text`` as class attribute:
+
+.. code-block:: pycon
+
+    >>> node = SchemaPropertiesNode()
+    >>> node.text
+    'Text'
+
+    >>> node.text = 1
+    Traceback (most recent call last):
+      ...
+    ValueError: 1 is no <class 'str'> type
+
+
+Plumbing Behaviors
+------------------
+
+General Behaviors
+~~~~~~~~~~~~~~~~~
+
+**node.behaviors.DefaultInit**
+    Plumbing behavior providing default ``__init__`` function on node. This
+    behavior is going to be deprecated in future versions. Use
+    ``node.behaviors.NodeInit`` instead.
+    See ``node.interfaces.IDefaultInit``.
+
+**node.behaviors.NodeInit**
+    Plumbing behavior for transparent setting of ``__name__`` and ``__parent__``
+    at object initialization time.
+    See ``node.interfaces.INodeInit``.
+
+**node.behaviors.Node**
+    Fill in gaps for full INode API. See ``node.interfaces.INode``.
+
+**node.behaviors.ContentishNode**
+    A node which can contain children. See
+    ``node.interfaces.IContentishNode``. Concrete implementations are
+    ``node.behaviors.MappingNode`` and ``node.behaviors.SequenceNode``.
+
+**node.behaviors.Attributes**
+    Provide attributes on node. See ``node.interfaces.IAttributes``. If
+    ``node.behaviors.Nodespaces`` is applied on node, the attributes instance
+    gets stored internally in ``__attrs__`` nodespace, otherwise its set on
+    ``__attrs__`` attribute.
+
+**node.behaviors.Events**
+    Provide an event registration and dispatching mechanism.
+    See ``node.interfaces.IEvents``.
+
+**node.behaviors.BoundContext**
+    Mechanism for scoping objects to interfaces and classes.
+    See ``node.interfaces.IBoundContext``.
+
+**node.behaviors.NodeReference**
+    Plumbing behavior holding an index of nodes contained in the tree.
+    See ``node.interfaces.INodeReference``.
+
+**node.behaviors.WildcardFactory**
+    Plumbing behavior providing factories by wildcard patterns.
+    See ``node.interfaces.IWildcardFactory``.
+
+
+Mapping Behaviors
+~~~~~~~~~~~~~~~~~
+
+**node.behaviors.MappingNode**
+    Turn an object into a mapping node. Extends ``node.behaviors.Node``.
+    See ``node.interfaces.IMappingNode``.
+
+**node.behaviors.MappingAdopt**
+    Plumbing behavior that provides ``__name__`` and ``__parent__`` attribute
+    adoption on child nodes of mapping.
+    See ``node.interfaces.IMappingAdopt``.
+
+**node.behaviors.MappingConstraints**
+    Plumbing behavior for constraints on mapping nodes.
+    See ``node.interfaces.IMappingConstraints``.
+
+**node.behaviors.UnicodeAware**
+    Plumbing behavior to ensure unicode for keys and string values.
+    See ``node.interfaces.IUnicodeAware``.
+
+**node.behaviors.Alias**
+    Plumbing behavior that provides aliasing of child keys.
+    See ``node.interfaces.IAlias``.
+
+**node.behaviors.AsAttrAccess**
+    Plumbing behavior to get node as IAttributeAccess implementation.
+    See ``node.interfaces.IAsAttrAccess``.
+
+**node.behaviors.ChildFactory**
+    Plumbing behavior providing child factories.
+    See ``node.interfaces.IChildFactory``.
+
+**node.behaviors.FixedChildren**
+    Plumbing Behavior that initializes a fixed dictionary as children.
+    See ``node.interfaces.IFixedChildren``.
+
+**node.behaviors.Nodespaces**
+    Plumbing behavior for providing nodespaces on node.
+    See ``node.interfaces.INodespaces``.
+
+**node.behaviors.Lifecycle**
+    Plumbing behavior taking care of lifecycle events.
+    See ``node.interfaces.ILifecycle``.
+
+**node.behaviors.AttributesLifecycle**
+    Plumbing behavior for handling lifecycle events on attribute manipulation.
+    See ``node.interfaces.IAttributesLifecycle``.
+
+**node.behaviors.Invalidate**
+    Plumbing behavior for node invalidation.
+    See ``node.interfaces.Invalidate``.
+
+**node.behaviors.VolatileStorageInvalidate**
+    Plumbing behavior for invalidating nodes using a volatile storage.
+    See ``node.interfaces.Invalidate``.
+
+**node.behaviors.Cache**
+    Plumbing behavior for caching.
+    See ``node.interfaces.ICache``.
+
+**node.behaviors.MappingOrder**
+    Plumbing behavior for ordering support on mapping nodes.
+    See ``node.interfaces.IMappingOrder``.
+
+**node.behaviors.UUIDAware**
+    Plumbing behavior providing a uuid on nodes.
+    See ``node.interfaces.IUUIDAware``.
+
+**node.behaviors.MappingReference**
+    Plumbing behavior to provide ``node.interfaces.INodeReference`` on mapping
+    nodes. See ``node.interfaces.IMappingReference``.
+
+**node.behaviors.MappingStorage**
+    Provide abstract mapping storage access.
+    See ``node.interfaces.IMappingStorage``.
+
+**node.behaviors.DictStorage**
+    Provide dictionary storage. Extends ``node.behaviors.MappingStorage``.
+    See ``node.interfaces.IMappingStorage``.
+
+**node.behaviors.OdictStorage**
+    Provide ordered dictionary storage. Extends
+    ``node.behaviors.MappingStorage``. See ``node.interfaces.IMappingStorage``.
+
+**node.behaviors.Fallback**
+    Provide a way to fall back to values by subpath stored on another node.
+    See ``node.interfaces.IFallback``.
+
+**node.behaviors.Schema**
+    Provide schema validation and value serialization on node values.
+    See ``node.interfaces.ISchema``.
+
+**node.behaviors.SchemaAsAttributes**
+    Provide schema validation and value serialization on node values via
+    dedicated attributes object.
+    See ``node.interfaces.ISchemaAsAttributes``.
+
+**node.behaviors.SchemaProperties**
+    Provide schema fields as class properties.
+    See ``node.interfaces.ISchemaProperties``.
+
+**node.behaviors.MappingFilter**
+    Filter mapping children by class or interface.
+    See ``node.interfaces.IChildFilter``.
+
+
+Sequence Behaviors
+~~~~~~~~~~~~~~~~~~
+
+**node.behaviors.SequenceNode**
+    Turn an object into a sequence node. Extends ``node.behaviors.Node``.
+    See ``node.interfaces.IMappingNode``.
+
+**node.behaviors.SequenceAdopt**
+    Plumbing behavior that provides ``__name__`` and ``__parent__`` attribute
+    adoption on child nodes of sequence.
+    See ``node.interfaces.ISequenceAdopt``.
+
+**node.behaviors.SequenceConstraints**
+    Plumbing behavior for constraints on sequence nodes.
+    See ``node.interfaces.ISequenceConstraints``.
+
+**node.behaviors.SequenceStorage**
+    Provide abstract sequence storage access.
+    See ``node.interfaces.ISequenceStorage``.
+
+**node.behaviors.ListStorage**
+    Provide list storage. See ``node.interfaces.ISequenceStorage``.
+
+**node.behaviors.SequenceReference**
+    Plumbing behavior to provide ``node.interfaces.INodeReference`` on sequence
+    nodes. See ``node.interfaces.ISequenceReference``.
+
+**node.behaviors.SequenceFilter**
+    Filter sequence children by class or interface.
+    See ``node.interfaces.IChildFilter``.
+
+**node.behaviors.SequenceOrder**
+    Plumbing behavior for ordering support on sequence nodes.
+    See ``node.interfaces.ISequenceOrder``.
+
+
+JSON Serialization
+------------------
+
+Nodes can be serialized to and deserialized from JSON:
+
+.. code-block:: pycon
+
+    >>> from node.serializer import serialize
+    >>> json_dump = serialize(BaseNode(name='node'))
+
+    >>> from node.serializer import deserialize
+    >>> deserialize(json_dump)
+    <BaseNode object 'node' at ...>
+
+For details on serialization API please read file in
+``docs/archive/serializer.rst``.
+
+
+Python Versions
+---------------
+
+- Python 2.7, 3.7+
+- May work with other versions (untested)
+
+
+Contributors
+============
+
+- Robert Niederreiter
+- Florian Friesdorf
+- Jens Klein
+
+
+
+Changes
+=======
+
+1.2.1 (2023-04-16)
+------------------
+
+- Replace deprecated import of ``Order`` with ``MappingOrder`` in ``node.base``.
+  [rnix]
+
+
+1.2 (2022-12-05)
+----------------
+
+- Do not overwrite ``uuid`` in ``node.behaviors.UUIDAware.__init__`` if
+  ``uuid`` already set.
+  [rnix]
+
+- Rename ``node.interfaces.IOrder`` to ``node.interfaces.IMappingOrder``
+  and ``node.behaviors.Order`` to ``node.behaviors.MappingOrder``.
+  B/C is kept.
+  [rnix]
+
+- Introduce ``node.behaviors.ISequenceOrder`` and
+  ``node.interfaces.SequenceOrder``.
+  [rnix]
+
+- Introduce ``node.interfaces.INodeOrder``. Used as base for
+  ``node.interfaces.IMappingOrder`` and ``node.interfaces.ISequenceOrder``.
+  [rnix]
+
+- Add rich comparison functions ``__lt__``, ``__le__``, ``__gt__`` and
+  ``__ge__`` to ``node.utils.Unset``.
+  [rnix]
+
+**Breaking changes**:
+
+- Importing B/C ``Order`` behavior from ``node.behaviors.order``
+  not works any more. Please import from ``node.behaviors``.
+  [rnix]
+
+
+1.1 (2022-10-06)
+----------------
+
+- Add ``node.schema.DateTime``, ``node.schema.DateTimeSerializer`` and
+  ``node.schema.datetime_serializer``.
+  [rnix]
+
+- Subclass ``threading.local`` for
+  ``node.behaviors.lifecycle._lifecycle_context``,
+  ``node.behaviors.events._attribute_subscribers`` and
+  ``node.behaviors.schema._schema_property`` objects in order to safely provide
+  default values.
+  [rnix]
+
+- Introduce ``node.interfaces.IChildFilter``, ``node.behaviors.MappingFilter``
+  and ``node.behaviors.SequenceFilter``.
+  [rnix]
+
+- Introduce ``node.interfaces.IWildcardFactory`` and
+  ``node.behaviors.WildcardFactory``.
+  [rnix]
+
+- Introduce ``node.interfaces.INodeInit`` and ``node.behaviors.NodeInit``.
+  [rnix]
+
+- Deprecate ``IFixedChildren.fixed_children_factories`` Use
+  ``IFixedChildren.factories`` instead.
+  [rnix]
+
+- Introduce ``node.interfaces.IContentishNode`` and
+  ``node.behaviors.ContentishNode``. Use as base for mapping and sequence nodes.
+  [rnix]
+
+- ``insertbefore``, ``insertafter`` and ``swap`` in ``node.behaviors.Order``
+  alternatively accept node names as arguments where possible.
+  [rnix]
+
+- ``insertbefore``, ``insertafter``, and ``insertfirst`` and ``insertlast`` in
+  ``node.behaviors.Order`` internally use ``movebefore``, ``moveafter``,
+  ``movefirst`` and ``movelast`` of ``odict`` to avoid modifying the data
+  structure before ``__setitem__`` gets called.
+  [rnix]
+
+- Extend ``node.interfaces.IOrder``  respective ``node.behaviors.Order``
+  by ``movebefore``, ``moveafter``, ``movefirst`` and ``movelast``.
+  [rnix]
+
+- Reset ``__parent__`` in ``node.behaviors.Node.detach``. Node is no longer
+  contained in tree.
+  [rnix]
+
+- Introduce ``IndexViolationError`` which inherits from ``ValueError`` and
+  raise it in reference related behaviors instead of ``ValueError`` where
+  appropriate.
+  [rnix]
+
+- Introduce ``node.interfaces.INodeReference`` and
+  ``node.behaviors.NodeReference``.
+  [rnix]
+
+- Introduce ``node.interfaces.ISequenceReference`` and
+  ``node.behaviors.SequenceReference``.
+  [rnix]
+
+- Rename ``node.interfaces.IReference`` to ``node.interfaces.IMappingReference``
+  and ``node.behaviors.Reference`` to ``node.behaviors.MappingReference``.
+  B/C is kept.
+  [rnix]
+
+**Breaking changes**:
+
+- Remove ``_notify_suppress`` flag from ``Lifecycle`` behavior. Introduce
+  ``suppress_lifecycle_events`` contextmanager as substitute.
+  [rnix]
+
+- Importing ``ChildFactory`` and ``FixedChildren`` from
+  ``node.behaviors.common`` not works any more. Please import from
+  ``node.behaviors``.
+  [rnix]
+
+- Importing B/C ``Reference`` behavior from ``node.behaviors.reference``
+  not works any more. Please import from ``node.behaviors``.
+  [rnix]
+
+
+1.0 (2022-03-17)
+----------------
+
+- Implement ``__copy__`` and ``__deepcopy__`` on ``node.utils.UNSET``.
+  [rnix]
+
+- Introduce ``node.interfaces.ISequenceConstraints`` and
+  ``node.behaviors.SequenceConstraints``.
+  [rnix]
+
+- Rename ``node.interfaces.INodeChildValidate`` to
+  ``node.interfaces.IMappingConstraints`` and
+  ``node.behaviors.NodeChildValidate`` to ``node.behaviors.MappingConstraints``.
+  ``MappingConstraints`` implementation moved from ``node.behaviors.common`` to
+  ``node.behaviors.constraints``. B/C is kept.
+  [rnix]
+
+- Introduce ``node.interfaces.ISequenceAdopt`` and
+  ``node.behaviors.SequenceAdopt``.
+  [rnix]
+
+- ``MappingAdopt`` now catches all exceptions instead of only
+  ``AttributeError``, ``KeyError`` and ``ValueError``.
+  [rnix]
+
+- Rename ``node.interfaces.IAdopt`` to ``node.interfaces.IMappingAdopt`` and
+  ``node.behaviors.Adopt`` to ``node.behaviors.MappingAdopt``. ``MappingAdopt``
+  implementation moved from ``node.behaviors.common`` to
+  ``node.behaviors.adopt``. B/C is kept.
+  [rnix]
+
+- ``node.behaviors.Attributes`` now also works if
+  ``node.behaviors.Nodespaces`` is not applied.
+  [rnix]
+
+- Introduce ``node.behaviors.Node`` which implements only
+  ``node.interfaces.INode`` contract. It is used as base for
+  ``node.behaviors.MappingNode`` and ``node.behaviors.SequcneNode``.
+  [rnix]
+
+- Do not inherit ``node.interfaces.INode`` from
+  ``zope.interfaces.common.mapping.IFullMapping`` any more. Data model specific
+  interfaces are added now via ``node.interfaces.IMappingNode`` and
+  ``node.interfaces.ISequenceNode``.
+  [rnix]
+
+- Introduce sequence nodes. Sequence nodes are implemented via
+  ``node.behaviors.SequcneNode`` and ``node.behaviors.ListStorage``.
+  [rnix]
+
+- Rename ``node.interfaces.INodify`` to ``node.interfaces.IMappingNode`` and
+  ``node.behaviors.Nodify`` to ``node.behaviors.MappingNode``. ``MappingNode``
+  implementation moved from ``node.behaviors.nodify`` to
+  ``node.behaviors.mapping``. B/C is kept.
+  [rnix]
+
+- Rename ``node.interfaces.IStorage`` to ``node.interfaces.IMappingStorage``
+  and ``node.behaviors.Storage`` to ``node.behaviors.Storage``. B/C is kept.
+  [rnix]
+
+- Add key and value type validation to schema fields where appropriate.
+  [rnix]
+
+- Introduce serializer support to schema fields. Add a couple of concrete field
+  serializer implementations to ``node.schema.serializer``.
+  [rnix]
+
+- Add ``ODict`` and ``Node`` schema fields to ``node.schema.fields``.
+  [rnix]
+
+- Add ``node.schema.fields.IterableField`` and use as base class for
+  ``List``, ``Tuple`` and ``Set`` schema fields.
+
+- Introduce ``node.behaviors.schema.SchemaProperties`` plumbing behavior.
+  [rnix]
+
+- Split up ``node.schema`` module into a package.
+  [rnix]
+
+- Introduce ``node.behaviors.context.BoundContext`` plumbing behavior.
+  [rnix]
+
+**Breaking changes**:
+
+- Remove ``node.behaviors.GetattrChildren``. See ``node.utils.AttributeAccess``
+  instead if you need to access node children via ``__getattr__``.
+  [rnix]
+
+- Importing B/C ``Adopt`` behavior from ``node.behaviors.common``
+  not works any more. Please import from ``node.behaviors``.
+  [rnix]
+
+- Importing B/C ``NodeChildValidate`` behavior from ``node.behaviors.common``
+  not works any more. Please import from ``node.behaviors``.
+  [rnix]
+
+- Importing B/C ``Nodify`` behavior from ``node.behaviors.nodify``
+  not works any more. Please import from ``node.behaviors``.
+  [rnix]
+
+- Remove deprecated B/C import location ``node.parts``.
+  [rnix]
+
+- ``node.behaviors.schema.Schema`` no longer considers wildcard fields.
+  [rnix]
+
+- ``node.behaviors.schema.Schema.__setitem__`` deletes value from related
+  storage for field if value is ``node.utils.UNSET``.
+  [rnix]
+
+- ``node.behaviors.schema.Schema.__getitem__`` always returns default value for
+  field instead of raising ``KeyError`` if no default is set.
+  [rnix]
+
+- Default value of ``node.schema.fields.Field.default`` is ``node.utils.UNSET``
+  now.
+  [rnix]
+
+- ``node.schema.fields.Field.validate`` raises exception if validation fails
+  instead of returning boolean.
+  [rnix]
+
+
+0.9.28 (2021-11-08)
+-------------------
+
+- Add missing ``node.interfaces.INodeAttributes`` interface.
+  [rnix]
+
+- Add missing ``attribute_access_for_attrs`` attribute to ``IAttributes``
+  interface.
+  [rnix]
+
+- Rename ``node.behaviors.common.NodeChildValidate.allow_non_node_childs``
+  to ``allow_non_node_children``. A Deprecation warning is printed if the
+  old attribute is used.
+  [rnix]
+
+- Introduce ``node.behaviors.schema.Schema``,
+  ``node.behaviors.schema.SchemaAsAttributes`` and related schema definitions
+  in ``node.schema``.
+  [rnix]
+
+
+0.9.27 (2021-10-21)
+-------------------
+
+- Expose ``first_key``, ``last_key``, ``next_key`` and ``prev_key`` from
+  odict storage on ``Order`` behavior.
+  [rnix, 2021-10-21]
+
+- Add basic serializer settings mechanism.
+  [rnix, 2021-07-20]
+
+
+0.9.26 (2021-05-10)
+-------------------
+
+- Use ``node.utils.safe_decode`` in ``node.behaviors.nodify.Nodify.treerepr``.
+  [rnix, 2021-05-04]
+
+- Add ``node.utils.safe_encode`` and ``node.utils.safe_decode``.
+  [rnix, 2021-05-04]
+
+
+0.9.25 (2020-03-30)
+-------------------
+
+- Introduce ``uuid_factory`` function on ``node.interfaces.IUUIDAware`` and
+  implement default function in ``node.behaviors.common.UUIDAware``.
+  [rnix, 2020-03-01]
+
+- Rename ``NodeTestCase.expect_error`` to ``NodeTestCase.expectError``.
+  [rnix, 2019-09-04]
+
+- Rename ``NodeTestCase.check_output`` to ``NodeTestCase.checkOutput``.
+  [rnix, 2019-09-04]
+
+- Introduce ``prefix`` keyword argument in ``Nodify.treerepr``.
+  [rnix, 2019-09-04]
+
+
+0.9.24 (2019-07-10)
+-------------------
+
+- Overhaul ``node.behaviors.Order``. Use related functions from ``odict`` where
+  appropriate.
+  [rnix, 2019-07-10]
+
+- Remove superfluous ``extra_require`` from ``setup.py``.
+  [rnix, 2019-04-25]
+
+- Drop Support for python < 2.7 and < 3.3.
+  [rnix, 2019-04-25]
+
+
+0.9.23 (2018-11-07)
+-------------------
+
+- Use property decorators for ``node.behaviors.reference.Reference.uuid``.
+  [rnix, 2017-12-15]
+
+
+0.9.22 (2017-07-18)
+-------------------
+
+- Add ``always_dispatch`` keyword argument to
+  ``node.behaviors.events.EventAttribute`` constructor which defines whether
+  events are always dispatched on ``__set__``, not only if attribute value
+  changes.
+  [rnix, 2017-06-20]
+
+- Use ``node.utils.UNSET`` as default ``default`` value in
+  ``node.behaviors.events.EventAttribute.__init__``.
+  [rnix, 2017-06-19]
+
+- Introduce ``node.behaviors.events.EventAttribute.subscriber`` decorator which
+  can be used to register attribute subscribers.
+  [rnix, 2017-06-19]
+
+- Move event dispatching related classes and functions from ``node.events``
+  to ``node.behaviors.events`` and import it from there in ``node.events``.
+  [rnix, 2017-06-16]
+
+- Introduce ``node.interfaces.IEvents`` and implement
+  ``node.behaviors.events.Events`` behavior. Contains business logic from
+  ``node.events.EventDispatcher``. Use new behavior on ``EventDispatcher``.
+  [rnix, 2017-06-16]
+
+- Create ``suppress_events`` context manager which can be used to
+  suppress event notification in conjunction with ``node.behaviors.Events``
+  behavior.
+  [rnix, 2017-06-15]
+
+- Create ``node.behaviors.fallback.fallback_processing`` context manager and
+  and use it in ``node.behaviors.fallback.Fallback.__getitem__`` to check
+  whether fallback processing is active.
+  [rnix, 2017-06-15]
+
+
+0.9.21 (2017-06-15)
+-------------------
+
+- Introduce ``node.events.EventDispatcher`` and ``node.events.EventAttribute``.
+  [rnix, 2017-06-15]
+
+- Use ``setattr`` in ``instance_property`` decorator instead of
+  ``object.__setattr__`` in order to avoid errors with custom low level
+  ``__setattr__`` implementations.
+  [rnix, 2017-06-14]
+
+
+0.9.20 (2017-06-07)
+-------------------
+
+- Type cast sort key to ``node.compat.UNICODE_TYPE`` in
+  ``node.behaviors.Nodify.treerepr`` to avoid unicode decode errors.
+  [rnix, 2017-06-07]
+
+
+0.9.19 (2017-06-07)
+-------------------
+
+- Python 3 and pypy compatibility.
+  [rnix, 2017-06-02]
+
+- Drop support for Python < 2.7.
+  [rnix, 2017-06-02]
+
+- Add ``__bool__`` to ``node.behaviors.Nodify``.
+  [rnix, 2017-06-02]
+
+- Add ``__bool__`` to ``node.utils.UNSET``.
+  [rnix, 2017-06-02]
+
+- Add ``treerepr`` in ``node.behaviors.nodify.Nodify`` and move code from
+  ``printtree`` to it. Returs tree representation as string instead of printing
+  it. ``printtree`` uses ``treerepr`` now. As enhancement ``treerepr`` sorts
+  children of node if it does not implement ``IOrdered`` in order to ensure
+  consistend output which can be used to write tests against.
+  [rnix, 2017-06-02]
+
+- Use ``object.__getattribute__`` explicitely in
+  ``node.utils.instance_property`` to check whether property value already has
+  been computed in order to avoid problems when oberwriting ``__getattr__``
+  on classes using ``instance_property`` decorator.
+  [rnix, 2017-06-02]
+
+
+0.9.18.1 (2017-02-23)
+---------------------
+
+- Fix permissions.
+  [rnix, 2017-02-23]
+
+
+0.9.18 (2017-02-14)
+-------------------
+
+- Add ``node.utils.node_by_path``.
+  [rnix, 2017-02-07]
+
+- Do not depend on ``unittest2`` since its is not used.
+  [jensens, 2017-01-17]
+
+- Add ``node.behaviors.Fallback`` behavior.
+  [jensens, 2017-01-17]
+
+
+0.9.17 (2017-01-17)
+-------------------
+
+- Add basic JSON serializer and deserializer.
+  [rnix, 2016-12-03]
+
+
+0.9.16 (2015-10-08)
+-------------------
+
+- Only encode name in ``node.behaviors.nodify.Nodify.__repr__`` and
+  ``node.behaviors.nodify.Nodify.noderepr`` if name is unicode instance.
+  [rnix, 2015-10-03]
+
+- Improve ``node.behaviors.nodify.Nodify.printtree``. None node children are
+  printed with key.
+  [rnix, 2015-10-03]
+
+
+0.9.15 (2014-12-17)
+-------------------
+
+- Fix dependency declaration to ``odict`` in order to make setuptools 8.x+
+  happy; using ``>=`` instead of ``>`` now.
+  [jensens, 2014-12-17]
+
+
+0.9.14
+------
+
+- use ``plumbing`` decorator instead of ``plumber`` metaclass.
+  [rnix, 2014-07-31]
+
+
+0.9.13
+------
+
+- Introduce ``node.behaviors.cache.VolatileStorageInvalidate``.
+  [rnix, 2014-01-15]
+
+
+0.9.12
+------
+
+- Add ``zope.component`` to install dependencies.
+  [rnix, 2013-12-09]
+
+
+0.9.11
+------
+
+- Use ``node.utils.UNSET`` instance in
+  ``node.behaviors.mapping.ExtendedWriteMapping.pop``.
+  [rnix, 2013-02-10]
+
+- Improve ``node.utils.Unset``. Add ``Unset`` instance at
+  ``node.utils.UNSET``.
+  [rnix, 2013-02-10]
+
+
+0.9.10
+------
+
+- Fix ``node.utils.StrCodec.encode`` to return value as is if str and decoding
+  failed.
+  [rnix, 2012-11-07]
+
+
+0.9.9
+-----
+
+- Python 2.7 compatibility.
+  [rnix, 2012-10-15]
+
+- Remove ``zope.component.event`` B/C.
+  [rnix, 2012-10-15]
+
+- Remove ``zope.location`` B/C.
+  [rnix, 2012-10-15]
+
+- Remove ``zope.lifecycleevent`` B/C.
+  [rnix, 2012-10-15]
+
+- Pep8.
+  [rnix, 2012-10-15]
+
+
+0.9.8
+-----
+
+- Deprecate the use of ``node.parts``. Use ``node.behaviors`` instead.
+  [rnix, 2012-07-28]
+
+- Adopt to ``plumber`` 1.2
+  [rnix, 2012-07-28]
+
+
+0.9.7
+-----
+
+- Introduce ``node.interfaces.IOrdered`` Marker interface. Set this interface
+  on ``node.parts.storage.OdictStorage``.
+  [rnix, 2012-05-21]
+
+- ``node.parts.mapping.ClonableMapping`` now supports ``deepcopy``.
+  [rnix, 2012-05-18]
+
+- Use ``zope.interface.implementer`` instead of ``zope.interface.implements``
+  all over the place.
+  [rnix, 2012-05-18]
+
+- Remove superfluos interfaces.
+  [rnix, 2012-05-18]
+
+- Remove ``Zodict`` from ``node.utils``.
+  [rnix, 2012-05-18]
+
+- Remove ``AliasedNodespace``, use ``Alias`` part instead.
+  [rnix, 2012-05-18]
+
+- Move aliaser objects from ``node.aliasing`` to ``node.parts.alias``.
+  [rnix, 2012-05-18]
+
+- Remove ``composition`` module.
+  [rnix, 2012-05-18]
+
+- Remove ``bbb`` module.
+  [rnix, 2012-05-18]
+
+
+0.9.6
+-----
+
+- Do not inherit ``node.parts.Reference`` from ``node.parts.UUIDAware``.
+  [rnix, 2012-01-30]
+
+- Set ``uuid`` in ``node.parts.Reference.__init__`` plumb.
+  [rnix, 2012-01-30]
+
+
+0.9.5
+-----
+
+- add ``node.parts.nodify.Nodify.acquire`` function.
+  [rnix, 2011-12-05]
+
+- add ``node.parts.ChildFactory`` plumbing part.
+  [rnix, 2011-12-04]
+
+- add ``node.parts.UUIDAware`` plumbing part.
+  [rnix, 2011-12-02]
+
+- fix ``node.parts.Order.swap`` in order to work with pickled nodes.
+  [rnix, 2011-11-28]
+
+- use ``node.name`` instead of ``node.__name__`` in
+  ``node.parts.nodify.Nodify.path``.
+  [rnix, 2011-11-17]
+
+- add ``swap`` to  ``node.parts.Order``.
+  [rnix, 2011-10-05]
+
+- add ``insertfirst`` and ``insertlast`` to ``node.parts.Order``.
+  [rnix, 2011-10-02]
+
+
+0.9.4
+-----
+
+- add ``node.utils.debug`` decorator.
+  [rnix, 2011-07-23]
+
+- remove non storage contract specific properties from
+  ``node.aliasing.AliasedNodespace``
+  [rnix, 2011-07-18]
+
+- ``node.aliasing`` test completion
+  [rnix, 2011-07-18]
+
+- Add non strict functionality to ``node.aliasing.DictAliaser`` for accessing
+  non aliased keys as is as fallback
+  [rnix, 2011-07-18]
+
+- Consider ``INode`` implementing objects in ``node.utils.StrCodec``
+  [rnix, 2011-07-16]
+
+- Remove duplicate implements in storage parts
+  [rnix, 2011-05-16]
+
+
+0.9.3
+-----
+
+- Increase test coverage
+  [rnix, 2011-05-09]
+
+- Add interfaces ``IFixedChildren`` and ``IGetattrChildren`` for related parts.
+  [rnix, 2011-05-09]
+
+- Rename ``Unicode`` part to ``UnicodeAware``.
+  [rnix, 2011-05-09]
+
+- Add ``node.utils.StrCodec``.
+  [rnix, 2011-05-09]
+
+- Inherit ``INodify`` interface from ``INode``.
+  [rnix, 2011-05-08]
+
+- Locking tests. Add ``time.sleep`` after thread start.
+  [rnix, 2011-05-08]
+
+- Cleanup ``BaseTester``, remove ``sorted_output`` flag (always sort), also
+  search class bases for detection in ``wherefrom``.
+  [rnix, 2011-05-08]
+
+- Remove useless try/except in ``utils.AttributeAccess``.
+  [rnix, 2011-05-08]
+
+- Add ``instance_property`` decorator to utils.
+  [rnix, 2011-05-06]
+
+- Add ``FixedChildren`` and ``GetattrChildren`` parts.
+  [chaoflow, 2011-04-22]
+
+
+0.9.2
+-----
+
+- Add ``__nonzero__`` on ``Nodifiy`` part always return True.
+  [rnix, 2011-03-15]
+
+
+0.9.1
+-----
+
+- Provide ``node.base.Node`` with same behavior like ``zodict.Node`` for
+  migration purposes.
+  [rnix, 2011-02-08]
+
+
+0.9
+---
+
+- Make it work [rnix, chaoflow, et al]
+
+
+License
+=======
+
+Copyright (c) 2009-2021, BlueDynamics Alliance, Austria
+Copyright (c) 2021-2022, Node Contributors
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice, this
+  list of conditions and the following disclaimer in the documentation and/or
+  other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
+ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
+ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `node-1.2/src/node.egg-info/SOURCES.txt` & `node-1.2.1/src/node.egg-info/SOURCES.txt`

 * *Files identical despite different names*

