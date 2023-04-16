# Comparing `tmp/rmlab-0.3.0.tar.gz` & `tmp/rmlab-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmlab-0.3.0.tar", last modified: Sun Feb 26 18:49:49 2023, max compression
+gzip compressed data, was "rmlab-0.4.0.tar", last modified: Sun Apr 16 15:04:47 2023, max compression
```

## Comparing `rmlab-0.3.0.tar` & `rmlab-0.4.0.tar`

### file list

```diff
@@ -1,69 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 18:49:49.413577 rmlab-0.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     1080 2023-02-26 18:49:30.000000 rmlab-0.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2214 2023-02-26 18:49:49.413577 rmlab-0.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1381 2023-02-26 18:49:30.000000 rmlab-0.3.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-02-26 18:49:30.000000 rmlab-0.3.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-02-26 18:49:49.414577 rmlab-0.3.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 18:49:49.389574 rmlab-0.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 18:49:49.395575 rmlab-0.3.0/src/rmlab/
--rw-rw-rw-   0 root         (0) root         (0)      916 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 18:49:49.400575 rmlab-0.3.0/src/rmlab/_api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9247 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/_api/base.py
--rw-rw-rw-   0 root         (0) root         (0)    13699 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/_api/fetch.py
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/_api/observability.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/_api/remove.py
--rw-rw-rw-   0 root         (0) root         (0)     2666 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/_api/simulation.py
--rw-rw-rw-   0 root         (0) root         (0)     8617 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/_api/upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 18:49:49.401575 rmlab-0.3.0/src/rmlab/_data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/_data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5931 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/_data/conversions.py
--rw-rw-rw-   0 root         (0) root         (0)     4718 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/_data/enums.py
--rw-rw-rw-   0 root         (0) root         (0)     1937 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/_data/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 18:49:49.401575 rmlab-0.3.0/src/rmlab/_util/
--rw-rw-rw-   0 root         (0) root         (0)     1305 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 18:49:49.402576 rmlab-0.3.0/src/rmlab/api/
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 18:49:49.404576 rmlab-0.3.0/src/rmlab/api/fetch/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/api/fetch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11464 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/api/fetch/core.py
--rw-rw-rw-   0 root         (0) root         (0)     4983 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/api/fetch/flight_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1027 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/api/fetch/parametric.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 18:49:49.404576 rmlab-0.3.0/src/rmlab/api/observability/
--rw-rw-rw-   0 root         (0) root         (0)     1077 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/api/observability/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 18:49:49.405576 rmlab-0.3.0/src/rmlab/api/operations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/api/operations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2732 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/api/operations/optimization.py
--rw-rw-rw-   0 root         (0) root         (0)     2962 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/api/operations/simulation.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/api/remove.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 18:49:49.406576 rmlab-0.3.0/src/rmlab/api/upload/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/api/upload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12344 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/api/upload/core.py
--rw-rw-rw-   0 root         (0) root         (0)     5164 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/api/upload/flight_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 18:49:49.408576 rmlab-0.3.0/src/rmlab/api/upload/parametric/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/api/upload/parametric/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2554 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/api/upload/parametric/customers.py
--rw-rw-rw-   0 root         (0) root         (0)      817 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/api/upload/parametric/filters.py
--rw-rw-rw-   0 root         (0) root         (0)     3663 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/api/upload/parametric/pricing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 18:49:49.409576 rmlab-0.3.0/src/rmlab/data/
--rw-rw-rw-   0 root         (0) root         (0)      700 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2985 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/data/flight.py
--rw-rw-rw-   0 root         (0) root         (0)     9492 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/data/items.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 18:49:49.412577 rmlab-0.3.0/src/rmlab/data/parametric/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/data/parametric/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      275 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/data/parametric/_customers_base.py
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/data/parametric/_pricing_base.py
--rw-rw-rw-   0 root         (0) root         (0)     8671 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/data/parametric/customers_choice.py
--rw-rw-rw-   0 root         (0) root         (0)     5413 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/data/parametric/customers_request.py
--rw-rw-rw-   0 root         (0) root         (0)     7923 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/data/parametric/filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2747 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/data/parametric/pricing_behavior.py
--rw-rw-rw-   0 root         (0) root         (0)    10972 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/data/parametric/pricing_optimizer.py
--rw-rw-rw-   0 root         (0) root         (0)     3922 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/data/parametric/pricing_range.py
--rw-rw-rw-   0 root         (0) root         (0)     4217 2023-02-26 18:49:30.000000 rmlab-0.3.0/src/rmlab/data/scenario.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 18:49:49.397575 rmlab-0.3.0/src/rmlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2214 2023-02-26 18:49:49.000000 rmlab-0.3.0/src/rmlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1675 2023-02-26 18:49:49.000000 rmlab-0.3.0/src/rmlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-26 18:49:49.000000 rmlab-0.3.0/src/rmlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-26 18:49:49.000000 rmlab-0.3.0/src/rmlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-02-26 18:49:49.000000 rmlab-0.3.0/src/rmlab.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.269839 rmlab-0.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-04-16 15:04:27.000000 rmlab-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2214 2023-04-16 15:04:47.269839 rmlab-0.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2023-04-16 15:04:27.000000 rmlab-0.4.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-04-16 15:04:27.000000 rmlab-0.4.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-04-16 15:04:47.270840 rmlab-0.4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.244838 rmlab-0.4.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.250838 rmlab-0.4.0/src/rmlab/
+-rw-rw-rw-   0 root         (0) root         (0)      916 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.255838 rmlab-0.4.0/src/rmlab/_api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9590 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_api/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    14244 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_api/fetch.py
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_api/observability.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_api/remove.py
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_api/simulation.py
+-rw-rw-rw-   0 root         (0) root         (0)    10142 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_api/upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.257839 rmlab-0.4.0/src/rmlab/_data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4993 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_data/conversions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6286 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_data/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     1937 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_data/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.257839 rmlab-0.4.0/src/rmlab/_util/
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.258839 rmlab-0.4.0/src/rmlab/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.259839 rmlab-0.4.0/src/rmlab/api/fetch/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/fetch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11464 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/fetch/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     8419 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/fetch/flight_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4924 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/fetch/parametric.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.260839 rmlab-0.4.0/src/rmlab/api/observability/
+-rw-rw-rw-   0 root         (0) root         (0)     1180 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/observability/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.261839 rmlab-0.4.0/src/rmlab/api/operations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/operations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4951 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/operations/optimization.py
+-rw-rw-rw-   0 root         (0) root         (0)     2962 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/operations/simulation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.261839 rmlab-0.4.0/src/rmlab/api/persistence/
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/persistence/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/remove.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.262839 rmlab-0.4.0/src/rmlab/api/upload/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/upload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13213 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/upload/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     5216 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/upload/flight_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.264839 rmlab-0.4.0/src/rmlab/api/upload/parametric/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/upload/parametric/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2992 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/upload/parametric/customers.py
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/upload/parametric/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     4391 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/upload/parametric/pricing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.266839 rmlab-0.4.0/src/rmlab/data/
+-rw-rw-rw-   0 root         (0) root         (0)      700 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6828 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/flight.py
+-rw-rw-rw-   0 root         (0) root         (0)    10309 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/items.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.269839 rmlab-0.4.0/src/rmlab/data/parametric/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/parametric/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      275 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/parametric/_customers_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/parametric/_pricing_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8670 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/parametric/customers_choice.py
+-rw-rw-rw-   0 root         (0) root         (0)     5413 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/parametric/customers_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     7923 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/parametric/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4450 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/parametric/pricing_behavior.py
+-rw-rw-rw-   0 root         (0) root         (0)    10954 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/parametric/pricing_optimizer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3922 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/parametric/pricing_range.py
+-rw-rw-rw-   0 root         (0) root         (0)     4379 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/scenario.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.252838 rmlab-0.4.0/src/rmlab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2214 2023-04-16 15:04:47.000000 rmlab-0.4.0/src/rmlab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1713 2023-04-16 15:04:47.000000 rmlab-0.4.0/src/rmlab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 15:04:47.000000 rmlab-0.4.0/src/rmlab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 15:04:47.000000 rmlab-0.4.0/src/rmlab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-16 15:04:47.000000 rmlab-0.4.0/src/rmlab.egg-info/top_level.txt
```

### Comparing `rmlab-0.3.0/LICENSE` & `rmlab-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rmlab-0.3.0/PKG-INFO` & `rmlab-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmlab
-Version: 0.3.0
+Version: 0.4.0
 Summary: RMLab python client
 Home-page: https://rmlab.ai
 Author: Anton Rey
 Author-email: aanton.rv@gmail.com
 Project-URL: Bug Tracker, https://rmlab.ai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rmlab-0.3.0/README.md` & `rmlab-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `rmlab-0.3.0/setup.cfg` & `rmlab-0.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rmlab
-version = 0.3.0
+version = 0.4.0
 author = Anton Rey
 author_email = aanton.rv@gmail.com
 description = RMLab python client
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://rmlab.ai
 project_urls =
```

### Comparing `rmlab-0.3.0/src/rmlab/__init__.py` & `rmlab-0.4.0/src/rmlab/__init__.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.3.0/src/rmlab/_api/base.py` & `rmlab-0.4.0/src/rmlab/_api/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,36 +54,46 @@
 ]
 
 _ApiEndpoints = [
     "api-discover-user",
     "api-data-bounded-get-meta",
     "api-data-bounded-get-all",
     "api-data-bounded-get-single",
-    "api-data-bounded-post",
+    "api-data-bounded-post-file",
+    "api-data-bounded-post-json",
     "api-data-flight-get",
     "api-data-flight-post",
     "api-data-flight-thresholds-post",
-    "api-data-pmodel-post",
+    "api-data-pmodel-post-file",
+    "api-data-pmodel-post-json",
+    "api-data-pmodel-get",
     "api-data-unbounded-get-fields",
     "api-data-unbounded-get-ids",
-    "api-data-unbounded-post",
+    "api-data-unbounded-post-file",
+    "api-data-unbounded-post-json",
     "api-data-airline-locations-get-ids",
     "api-data-airline-locations-get-items",
     "api-data-remove-full",
     "api-data-remove-restart",
     "api-data-summary-get-all",
     "api-data-summary-get-single",
     "api-operation-simulation-checkpoint",
     "api-operation-simulation-pause",
     "api-operation-simulation-trigger",
     "api-operation-optimization-trigger",
     "api-operation-optimization-schedule",
+    "api-operation-optimization-input-ids",
+    "api-operation-optimization-scheduled-ids",
+    "api-operation-set-date",
     "api-monitor-activity-user",
     "api-monitor-async-scenario-status",
     "api-monitor-async-scenario-result",
+    "api-snapshot-list",
+    "api-snapshot-save",
+    "api-snapshot-restore",
 ]
 
 _ExpectedEndpointsIds = _AuthEndpoints + _ApiEndpoints
 
 
 def _check_valid_credentials(creds: Mapping[str, Any]):
 
@@ -91,15 +101,15 @@
         raise ValueError(f"Some required keys not found in received credentials")
 
 
 def _check_valid_endpoints(endpoints_ids: Iterable[str]):
 
     for ep_id in endpoints_ids:
         if ep_id not in _ExpectedEndpointsIds:
-            _Logger.warning(f"Unrecognized endpoint `{ep_id}`")
+            _Logger.debug(f"Unrecognized endpoint `{ep_id}`")
 
 
 class APIBaseInternal:
     """Asynchronous context manager providing internal initialization, login and API server calls to derived classes."""
 
     def __init__(
         self,
```

### Comparing `rmlab-0.3.0/src/rmlab/_api/fetch.py` & `rmlab-0.4.0/src/rmlab/_api/fetch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, List, Mapping, Optional, Tuple
+from typing import Any, List, Mapping, Optional, Tuple, Union
 
 from rmlab._data.enums import FlightDataKind, ScenarioState
 from rmlab._data.types import (
     AirlineLocation,
     BoundedItem,
     UnboundedItem,
     fields_of_dataclass,
@@ -22,15 +22,15 @@
     AllBoundedItems,
     AnyAirlineLocationType,
     AnyBoundedType,
     AnyUnboundedType,
     Flight,
     Schedule,
 )
-from rmlab.data.flight import FlightData
+from rmlab.data.flight import FlightData, FlightDataForecastedBooks
 
 
 class APIFetchInternal(APIBaseInternal):
     """Interface to fetch data from server."""
 
     async def _fetch_info(
         self, scen_id: int
@@ -313,30 +313,30 @@
         self,
         scen_id: int,
         ids: List[str],
         kind: FlightDataKind,
         *,
         citysector_id: Optional[str] = None,
         sector_id: Optional[str] = None,
-    ) -> List[FlightData]:
+    ) -> List[Union[FlightData, FlightDataForecastedBooks]]:
         """Fetch flight data arrays of given flights, associated to a citysector or sector, from server.
         At least `citysector_id` and/or `sector_id` associated to the flights must be defined.
 
         Args:
             scen_id (int): Scenario ID
             ids (List[str]): List of flights IDs
             kind (FlightDataKind): Kind of flight data to fetch
             citysector_id (Optional[str], optional): Target citysector ID. Defaults to None.
             sector_id (Optional[str], optional): Target sector ID. Defaults to None.
 
         Raises:
             ValueError: If none of `citysector_id`, `sector_id` is defined
 
         Returns:
-            List[FlightData]: List of containers holding the flight data arrays.
+            List[Union[FlightData, FlightDataForecastedBooks]]: List of containers holding the flight data arrays.
         """
 
         if citysector_id is None and sector_id is None:
             raise ValueError(
                 f"Require definition of either `citysector_id` or `sector_id`"
             )
 
@@ -347,15 +347,15 @@
         if endpoint_limit is None:
             endpoint_limit = float("inf")
 
         if len(ids) > endpoint_limit:
 
             # Sequentially fetch items in chunks to keep the request/response payloads and server load controlled
 
-            ret_data: List[FlightData] = list()
+            ret_data: List[Union[FlightData, FlightDataForecastedBooks]] = list()
 
             for chunk_start in range(0, len(ids), endpoint_limit):
 
                 chunk_end = chunk_start + endpoint_limit
                 if chunk_end > len(ids):
                     chunk_end = -1
 
@@ -388,7 +388,19 @@
                 sector_id=sector_id,
             )
 
             return [
                 S2C_DataKind2ConvertFunction[kind](flight_id, flight_data)
                 for flight_id, flight_data in zip(ids, flights_data)
             ]
+
+
+    async def _fetch_pmodel(self,
+                            scen_id: int,
+                            kind: str,
+                            pmodel_id: str):
+        """TODO"""
+
+        return await self._submit_call("api-data-pmodel-get",
+                                       scen_id=scen_id,
+                                       kind=kind,
+                                       pmodel_id=pmodel_id)
```

### Comparing `rmlab-0.3.0/src/rmlab/_api/remove.py` & `rmlab-0.4.0/src/rmlab/_api/remove.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.3.0/src/rmlab/_api/simulation.py` & `rmlab-0.4.0/src/rmlab/_api/simulation.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.3.0/src/rmlab/_api/upload.py` & `rmlab-0.4.0/src/rmlab/_api/upload.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os, logging
-from typing import Optional, Union
+from typing import Optional, Union, Union
 
 from rmlab_http_client.types import FileExtensionType
 
 from rmlab._api.base import APIBaseInternal
 from rmlab._data.conversions import (
-    C2S_FlightDataName2ConvertFunction,
     UploadableDataClassName2DataKind,
     UploadableFlightDataType,
 )
 from rmlab._data.enums import (
     CustomersModelKind,
     ParametricModelKind,
     PricingModelKind,
@@ -30,101 +29,127 @@
 _Logger = logging.getLogger(__name__)
 
 
 class APIUploadInternal(APIBaseInternal):
     """Interface to upload data to server"""
 
     async def _upload_bounded_items(
-        self, scen_id: int, category: BoundedItem, data_fn: str
+        self, scen_id: int, category: BoundedItem, items: Union[str, list]
     ) -> None:
         """Upload a set of bounded items defined in a file.
 
         Args:
             scen_id (int): Scenario ID
             category (BoundedItem): Category
-            data_fn (str): Filename (.csv or .json) defining the items
+            items: Filename (.csv or .json) defining the items or items as json list
 
         Raises:
             ValueError: If category is not bounded
             ValueError: If file extension is invalid
             FileNotFoundError: If file does not exist
         """
 
         if not issubclass(category, BoundedItem):
             raise ValueError(
                 f"Category `{category.__name__}` must inherit from `BoundedItem`"
             )
+        
+        if isinstance(items, str): # filename expected
 
-        if not os.path.exists(data_fn):
-            raise FileNotFoundError(data_fn)
+          if not os.path.exists(items):
+              raise FileNotFoundError(items)
 
-        _, ext = os.path.splitext(data_fn)
-        ext: str = FileExtensionType.str_to_enum_value(ext.replace(".", "")).value
+          _, ext = os.path.splitext(items)
+          ext: str = FileExtensionType.str_to_enum_value(ext.replace(".", "")).value
 
-        _Logger.debug(f"Uploading `{category.__name__}` items")
-
-        await self._submit_call(
-            "api-data-bounded-post",
-            scen_id=scen_id,
-            category=category.__name__.lower(),
-            file=data_fn,
-            extension=ext,
-        )
-
-        _Logger.debug(f"File `{data_fn}` of category `{category.__name__}` uploaded")
+          _Logger.debug(f"Uploading `{category.__name__}` items")
+
+          await self._submit_call(
+              "api-data-bounded-post-file",
+              scen_id=scen_id,
+              category=category.__name__.lower(),
+              content=items,
+              extension=ext,
+          )
+
+          _Logger.debug(f"File `{items}` of category `{category.__name__}` uploaded")
+
+        elif isinstance(items, list): # json expected
+
+          await self._submit_call(
+              "api-data-bounded-post-json",
+              scen_id=scen_id,
+              category=category.__name__.lower(),
+              items=items
+          )
+        else:
+            raise TypeError(f"Unhandled type `{type(items)}`")
+        
 
     async def _upload_unbounded_items(
         self,
         scen_id: int,
         category: UnboundedItem,
-        data_fn: str,
+        items: Union[str, list],
         *,
         citysector_id: Optional[str] = None,
         sector_id: Optional[str] = None,
     ) -> None:
         """Upload a set of unbounded items defined in a file.
         Used to upload a set of flight schedules or a set of flights to server.
 
         Arguments `citysector_id` and `sector_id` are always optional. If any of them provided, concurrent uploads of flights
             files belonging to different citysectors/sectors are allowed.
 
         Args:
             scen_id (int): Scenario ID
             category (UnboundedItem): Category
-            data_fn (str): Filename (.csv or .json) defining the items
+            items (str): Filename (.csv or .json) defining the items or items as json list
             citysector_id (Optional[str], optional): Citysector ID to which items in file are associated. Defaults to None.
             sector_id (Optional[str], optional): Sector ID to which items in file are associated. Defaults to None.
 
         Raises:
             ValueError: If category is not unbounded
             ValueError: If file extension is invalid
             FileNotFoundError: If file does not exist
         """
 
         if not issubclass(category, UnboundedItem):
             raise ValueError(
                 f"Category `{category.__name__}` must inherit from `UnboundedItem`"
             )
 
-        _, ext = os.path.splitext(data_fn)
-        ext: str = FileExtensionType.str_to_enum_value(ext.replace(".", "")).value
-
-        _Logger.debug(f"Uploading `{category.__name__}` items")
-
-        await self._submit_call(
-            "api-data-unbounded-post",
-            scen_id=scen_id,
-            category=category.__name__.lower(),
-            citysector_id=citysector_id,
-            sector_id=sector_id,
-            file=data_fn,
-            extension=ext,
-        )
+        if isinstance(items, str):
+            _, ext = os.path.splitext(items)
+            ext: str = FileExtensionType.str_to_enum_value(ext.replace(".", "")).value
+
+            _Logger.debug(f"Uploading `{category.__name__}` items")
+
+            await self._submit_call(
+                "api-data-unbounded-post-file",
+                scen_id=scen_id,
+                category=category.__name__.lower(),
+                citysector_id=citysector_id,
+                sector_id=sector_id,
+                content=items,
+                extension=ext,
+            )
+        elif isinstance(items, list):
+            await self._submit_call(
+                "api-data-unbounded-post-json",
+                scen_id=scen_id,
+                category=category.__name__.lower(),
+                citysector_id=citysector_id,
+                sector_id=sector_id,
+                items=items
+            )
+        else:
+            raise TypeError(f"Unhandled type `{type(items)}`")
 
-        _Logger.debug(f"File `{data_fn}` of category `{category.__name__}` uploaded")
+        _Logger.debug(f"Items `{items}` of category `{category.__name__}` uploaded")
 
     async def _upload_flight_data(
         self,
         scen_id: int,
         flight_data: UploadableFlightDataType,
         *,
         citysector_id: Optional[str] = None,
@@ -149,82 +174,92 @@
             raise ValueError(
                 f"Require definition of either `citysector_id` or `sector_id`"
             )
 
         flight_data_class_name = type(flight_data).__name__
 
         if flight_data_class_name not in UploadableDataClassName2DataKind:
-            raise ValueError(
-                f"Flight data of type `{type(flight_data)}` cannot be uploaded"
-            )
-
-        flight_id, data = C2S_FlightDataName2ConvertFunction[flight_data_class_name](
-            flight_data
-        )
+            raise TypeError(f"Flight data of type `{type(flight_data)}` cannot be uploaded")
 
-        kind = UploadableDataClassName2DataKind[flight_data_class_name]
+        flight_id, data = flight_data.id_dict()
 
         await self._submit_call(
             "api-data-flight-post",
             scen_id=scen_id,
             flight_id=flight_id,
-            kind=kind,
+            kind=UploadableDataClassName2DataKind[flight_data_class_name].value,
             citysector_id=citysector_id,
             sector_id=sector_id,
             data=data,
         )
 
     async def _upload_parametric_model(
         self,
         scen_id: int,
         parametric_kind: ParametricModelKind,
         kind: Union[CustomersModelKind, PricingModelKind],
-        data_fn: str,
+        content: Union[str, dict],
     ) -> None:
         """Upload a parametric model (a `customers` or a `pricing` model) defined in a file to server.
 
         Args:
             scen_id (int): Scenario ID
             parametric_kind (ParametricModelKind): Parametric kind value (a `customers` or `pricing` parametric model)
             kind (Union[CustomersModelKind, PricingModelKind]): A subkind of parametric model.
             Given parametric_kind=`CUSTOMERS`, any of `REQUEST` or `CHOICE`
             Given parametric_kind=`PRICING`, any of `RANGE`, `BEHAVIOR`, `OPTIMIZER`
-            data_fn (str): Filename (.json) defining the parametric model.
+            content (str): Model content as filename or json dict, defining the parametric model.
         """
 
+        if isinstance(content, str): # File
+            pmodel_id = os.path.basename(content)
+        elif isinstance(content, dict): # Json dict
+            if "id" not in content:
+                raise ValueError(f"Need non-empty string definition in `id` for model")
+            pmodel_id = content.pop("id")
+        else:
+            raise TypeError(f"Unhandled model content type `{type(content)}`")
+
         # Make equivalent parametric models types to ensure correctness before uploading to server
         if parametric_kind == ParametricModelKind.CUSTOMERS:
             if kind == CustomersModelKind.REQUEST:
-                make_customers_request_model_from_json(data_fn)
+                make_customers_request_model_from_json(content)
             elif kind == CustomersModelKind.CHOICE:
-                make_customers_choice_model_from_json(data_fn)
+                make_customers_choice_model_from_json(content)
             else:
                 raise ValueError(f"Unexpected value of `{kind}`")
         elif parametric_kind == ParametricModelKind.PRICING:
             if kind == PricingModelKind.RANGE:
-                make_pricing_range_from_json(data_fn)
+                make_pricing_range_from_json(content)
             elif kind == PricingModelKind.BEHAVIOR:
-                make_pricing_behavior_from_json(data_fn)
+                make_pricing_behavior_from_json(content)
             elif kind == PricingModelKind.OPTIMIZER:
-                make_pricing_optimizer_from_json(data_fn)
+                make_pricing_optimizer_from_json(content)
             else:
                 raise ValueError(f"Unexpected value of `{kind}`")
         else:
             raise ValueError(f"Unexpected value of `{parametric_kind}`")
 
-        _, ext = os.path.splitext(data_fn)
-        ext: str = FileExtensionType.str_to_enum_value(ext.replace(".", "")).value
+        if isinstance(content, str): # File
+
+            _, ext = os.path.splitext(content)
+            ext: str = FileExtensionType.str_to_enum_value(ext.replace(".", "")).value
 
-        _Logger.debug(f"Uploading `{parametric_kind.value}` `{kind.value}` model")
+            await self._submit_call(
+                "api-data-pmodel-post-file",
+                scen_id=str(scen_id),
+                kind=f"{parametric_kind.value}_{kind.value}",
+                pmodel_id=pmodel_id,
+                content=content,
+                extension=ext,
+            )
 
-        pmodel_id = os.path.basename(data_fn)
+        elif isinstance(content, dict): # Json dict
 
-        await self._submit_call(
-            "api-data-pmodel-post",
-            scen_id=str(scen_id),
-            kind=parametric_kind.value + "_" + kind.value,
-            pmodel_id=pmodel_id,
-            file=data_fn,
-            extension=ext,
-        )
+            await self._submit_call(
+                "api-data-pmodel-post-json",
+                scen_id=str(scen_id),
+                kind=f"{parametric_kind.value}_{kind.value}",
+                pmodel_id=pmodel_id,
+                content=content)
 
-        _Logger.debug(f"File `{data_fn}` uploaded as pmodel with id `{pmodel_id}`")
+        _Logger.debug(f"PModel content uploaded with id `{pmodel_id}`")
```

### Comparing `rmlab-0.3.0/src/rmlab/_data/types.py` & `rmlab-0.4.0/src/rmlab/_data/types.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.3.0/src/rmlab/_util/__init__.py` & `rmlab-0.4.0/src/rmlab/_util/__init__.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.3.0/src/rmlab/api/__init__.py` & `rmlab-0.4.0/src/rmlab/api/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 from rmlab.api.upload.core import APIUploadCore
 from rmlab.api.upload.parametric.filters import APIUploadParametric
 from rmlab.api.upload.parametric.customers import APIUploadCustomersModels
 from rmlab.api.upload.parametric.pricing import APIUploadPricingModels
 from rmlab.api.upload.flight_data import APIUploadFlightData
 from rmlab.api.fetch.core import APIFetchCore
 from rmlab.api.fetch.flight_data import APIFetchFlightData
+from rmlab.api.fetch.parametric import APIFetchParametric
 from rmlab.api.observability import APIObservability
 
 class API(
     APISimulation,
     APIOptimization,
     APIUploadCore,
     APIUploadParametric,
     APIUploadCustomersModels,
     APIUploadPricingModels,
     APIUploadFlightData,
     APIRemove,
     APIFetchCore,
     APIFetchFlightData,
+    APIFetchParametric,
     APIObservability,
 ):
     """Complete mixin interface to run simulations, upload local data and fetch/remove remote data"""
 
     pass
```

### Comparing `rmlab-0.3.0/src/rmlab/api/fetch/core.py` & `rmlab-0.4.0/src/rmlab/api/fetch/core.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.3.0/src/rmlab/api/fetch/flight_data.py` & `rmlab-0.4.0/src/rmlab/api/fetch/flight_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 
 from typing import List, Optional
 from rmlab._data.enums import FlightDataKind
 from rmlab._api.fetch import APIFetchInternal
 
 from rmlab.data.flight import (
     FlightDataBooks,
+    FlightDataForecastedBooks,
     FlightDataEvents,
     FlightDataPricePerSeatSettings,
     FlightDataThresholdSettings,
+    FlightDataQForecast
 )
 
 
 class APIFetchFlightData(APIFetchInternal):
     """Exposes functions for fetching flight data from the server."""
 
     async def fetch_flights_data_historic(
@@ -43,14 +45,110 @@
             scen_id,
             ids,
             FlightDataKind.ACTUAL_BOOKS,
             citysector_id=citysector_id,
             sector_id=sector_id,
         )
 
+
+    async def fetch_flights_data_expected(
+        self,
+        scen_id: int,
+        ids: List[str],
+        *,
+        citysector_id: Optional[str] = None,
+        sector_id: Optional[str] = None,
+    ) -> List[FlightDataForecastedBooks]:
+        """Fetch flight data of expected books of given flights, associated to a citysector or sector, from server.
+        At least `citysector_id` and/or `sector_id` associated to the flights must be defined.
+
+        Args:
+            scen_id (int): Scenario ID
+            ids (List[str]): List of flights IDs
+            citysector_id (Optional[str], optional): Target citysector ID. Defaults to None.
+            sector_id (Optional[str], optional): Target sector ID. Defaults to None.
+
+        Raises:
+            ValueError: If none of `citysector_id`, `sector_id` is defined
+
+        Returns:
+            List of expected books data containers of each flight.
+        """
+        return await self._fetch_flights_data(
+            scen_id,
+            ids,
+            FlightDataKind.EXPECTED_BOOKS,
+            citysector_id=citysector_id,
+            sector_id=sector_id,
+        )
+
+
+    async def fetch_flights_data_dynamic(
+        self,
+        scen_id: int,
+        ids: List[str],
+        *,
+        citysector_id: Optional[str] = None,
+        sector_id: Optional[str] = None,
+    ) -> List[FlightDataForecastedBooks]:
+        """Fetch flight data of dynamic books of given flights, associated to a citysector or sector, from server.
+        At least `citysector_id` and/or `sector_id` associated to the flights must be defined.
+
+        Args:
+            scen_id (int): Scenario ID
+            ids (List[str]): List of flights IDs
+            citysector_id (Optional[str], optional): Target citysector ID. Defaults to None.
+            sector_id (Optional[str], optional): Target sector ID. Defaults to None.
+
+        Raises:
+            ValueError: If none of `citysector_id`, `sector_id` is defined
+
+        Returns:
+            List of dynamic books data containers of each flight.
+        """
+        return await self._fetch_flights_data(
+            scen_id,
+            ids,
+            FlightDataKind.DYNAMIC_BOOKS,
+            citysector_id=citysector_id,
+            sector_id=sector_id,
+        )
+
+    async def fetch_flights_data_forecast(
+        self,
+        scen_id: int,
+        ids: List[str],
+        *,
+        citysector_id: Optional[str] = None,
+        sector_id: Optional[str] = None,
+    ) -> List[FlightDataQForecast]:
+        """Fetch forecast flight data of given flights, associated to a citysector or sector, from server.
+        At least `citysector_id` and/or `sector_id` associated to the flights must be defined.
+
+        Args:
+            scen_id (int): Scenario ID
+            ids (List[str]): List of flights IDs
+            citysector_id (Optional[str], optional): Target citysector ID. Defaults to None.
+            sector_id (Optional[str], optional): Target sector ID. Defaults to None.
+
+        Raises:
+            ValueError: If none of `citysector_id`, `sector_id` is defined
+
+        Returns:
+            List of forecast data containers of each flight.
+        """
+
+        return await self._fetch_flights_data(
+            scen_id,
+            ids,
+            FlightDataKind.FORECAST,
+            citysector_id=citysector_id,
+            sector_id=sector_id,
+        )
+
     async def fetch_flights_data_pricing_thresholds(
         self,
         scen_id: int,
         ids: List[str],
         *,
         citysector_id: Optional[str] = None,
         sector_id: Optional[str] = None,
@@ -75,14 +173,15 @@
             scen_id,
             ids,
             FlightDataKind.THRESHOLDS_SETTINGS,
             citysector_id=citysector_id,
             sector_id=sector_id,
         )
 
+
     async def fetch_flights_data_pricing_per_seat(
         self,
         scen_id: int,
         ids: List[str],
         *,
         citysector_id: Optional[str] = None,
         sector_id: Optional[str] = None,
```

### Comparing `rmlab-0.3.0/src/rmlab/api/observability/__init__.py` & `rmlab-0.4.0/src/rmlab/api/observability/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -22,7 +22,11 @@
         if context.lower() not in ["info", "warning", "error", "critical"]:
             raise ValueError(f"Expected log context either 'info', 'warning', 'error' or 'critical'")
         
         if not isinstance(count, int) or (isinstance(count, int) and count <= 0):
             raise ValueError(f"Expected 'count' to be a positive integer")
 
         return await self._fetch_logs(context, count)
+
+    async def fetch_snapshots_list(self):
+
+        return await self._submit_call("api-snapshot-list")
```

### Comparing `rmlab-0.3.0/src/rmlab/api/operations/optimization.py` & `rmlab-0.4.0/src/rmlab/api/operations/optimization.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Interface to trigger optimization passes."""
 
 from datetime import datetime
-from typing import Optional
+from typing import Optional, List
 from rmlab._api.base import APIBaseInternal
-from rmlab._data.types import DateTimeMinFormat
+from rmlab._data.types import DateTimeMinFormat, DateFormat
 
 
 class APIOptimization(APIBaseInternal):
-    """Exposes functions to run and schedule optimization runs on a set of flights."""
+    """Exposes functions to run and schedule optimization runs on a set of flights
+    and to fetch flights related to optimization targets."""
 
     async def trigger_optimization_pass(
         self,
         scen_id: int,
         airline_id: str,
         *,
         citysector_id: Optional[str] = None,
@@ -31,15 +32,15 @@
 
         if citysector_id is None and sector_id is None:
             raise ValueError(
                 f"At least one of `citysector_id`, `sector_id` must be defined"
             )
 
         await self._submit_call(
-            "api-operation-optimize-trigger",
+            "api-operation-optimization-trigger",
             scen_id=scen_id,
             airline_id=airline_id,
             citysector_id=citysector_id,
             sector_id=sector_id,
         )
 
     async def schedule_optimization_pass(
@@ -66,14 +67,77 @@
 
         if citysector_id is None and sector_id is None:
             raise ValueError(
                 f"At least one of `citysector_id`, `sector_id` must be defined"
             )
 
         await self._submit_call(
-            "api-operation-optimize-schedule",
+            "api-operation-optimization-schedule",
             scen_id=scen_id,
             date_time=datetime.strftime(date_time, DateTimeMinFormat),
             airline_id=airline_id,
             citysector_id=citysector_id,
             sector_id=sector_id,
         )
+
+    async def fetch_optimization_input_flights(
+            self,
+            scen_id: int,
+            flight_id: str,
+            citysector_id: str) -> List[str]:
+        """Returns all flights whose data is used as input for optimizing the input flight.
+
+        Args:
+            scen_id (int): Scenario ID.
+            flight_id (str): Flight ID.
+            citysector_id (str): Citysector ID of flight.
+        """
+
+        return await self._submit_call(
+            "api-operation-optimization-input-ids",
+            scen_id=scen_id,
+            flight_id=flight_id,
+            citysector_id=citysector_id)
+
+    async def fetch_optimization_scheduled_flights(
+            self,
+            scen_id: int,
+            airline_id: str,
+            sector_id: str,
+            date_start: datetime,
+            date_end: datetime) -> List[str]:
+        """Returns all flights of an airline in a sector scheduled for optimization passes in a date interval
+
+        Args:
+            scen_id (int): Scenario ID.
+            airline_id (str): Airline ID.
+            sector_id (str): Sector ID of flight.
+            date_start (datetime): Start of date interval.
+            date_end (datetime): End of date interval.
+        """
+
+        return await self._submit_call(
+            "api-operation-optimization-scheduled-ids",
+            scen_id=scen_id,
+            airline_id=airline_id,
+            sector_id=sector_id,
+            ds_start=datetime.strftime(date_start, DateFormat),
+            ds_end=datetime.strftime(date_end, DateFormat))
+
+    async def set_current_date(
+            self,
+            scen_id: int,
+            date_current: datetime):
+        """Set current date.
+
+        Args:
+            scen_id (int): Scenario ID.
+            date_current (datetime): Current date to set.
+        """
+
+        if not isinstance(date_current, datetime):
+            raise TypeError(f"Expected `datetime` type, got `{type(date_current)}`")
+
+        return await self._submit_call(
+            "api-operation-set-date",
+            scen_id=scen_id,
+            ds_current=datetime.strftime(date_current, DateFormat))
```

### Comparing `rmlab-0.3.0/src/rmlab/api/operations/simulation.py` & `rmlab-0.4.0/src/rmlab/api/operations/simulation.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.3.0/src/rmlab/api/remove.py` & `rmlab-0.4.0/src/rmlab/api/remove.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.3.0/src/rmlab/api/upload/core.py` & `rmlab-0.4.0/src/rmlab/api/upload/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,70 @@
 """Interface for core data uploading. """
 
 import os
-from typing import Optional
+from typing import Optional, Union
+from rmlab_errors import raise_from_list
 from rmlab._api.upload import APIUploadInternal
 from rmlab.data.items import (
     Aircraft,
     Airline,
     Airport,
     City,
     Country,
     Schedule,
 )
 
 
 class APIUploadCore(APIUploadInternal):
     """Exposes functions for uploading local data to the server."""
 
-    async def upload_aircrafts(self, scen_id: int, data_fn: str) -> None:
+    async def upload_aircrafts(self, scen_id: int, items: Union[str, list]) -> None:
         """Upload a set of aircrafts defined in a file.
 
 
         Args:
             scen_id (int): Scenario ID
-            data_fn (str): Filename `.csv` or `.json` defining the aircrafts
+            items (str): Filename `.csv` or `.json` defining the aircrafts
 
-        Where `data_fn` can refer to:
+        Where `items` can refer to:
 
         * a **CSV file**, for instance:
         ```csv
         Model,Seat capacity
         Airbus A320-a,174
         Airbus A320-b,180
         ```
 
         * a **JSON file**, for instance:
         ```json
         [
             {"model": "Airbus A320-a", "seat_capacity": 174},
             {"model": "Airbus A320-b", "seat_capacity": 180},
         ]
+
+        * a **JSON list** like the previous.
         ```
 
         Raises:
             ValueError: If file extension is invalid
             FileNotFoundError: If file does not exist
         """
 
         await self._upload_bounded_items(
-            scen_id=scen_id, category=Aircraft, data_fn=data_fn
+            scen_id=scen_id, category=Aircraft, items=items
         )
 
-    async def upload_airlines(self, scen_id: int, data_fn: str) -> None:
+    async def upload_airlines(self, scen_id: int, items: Union[str, list]) -> None:
         """Upload a set of airlines defined in a file.
 
         Args:
             scen_id (int): Scenario ID
-            data_fn (str): Filename `.csv` or `.json` defining the airlines
+            items (str): Filename `.csv` or `.json` defining the airlines
 
-        Where `data_fn` can refer to:
+        Where `items` can refer to:
 
         * a **CSV file**, for instance:
         ```csv
         Name,Type
         MyCarrier,low-cost
         AnotherCarrier,low-cost
         MyLegacyCarrier,legacy
@@ -70,33 +73,35 @@
         * a **JSON file**, for instance:
         ```json
         [
             {"name": "MyCarrier", "type": "low-cost"},
             {"name": "AnotherCarrier", "type": "low-cost"},
             {"name": "MyLegacyCarrier", "type": "legacy"},
         ]
+
+        * a **JSON list** like the previous.
         ```
 
         Raises:
             ValueError: If file extension is invalid
             FileNotFoundError: If file does not exist
         """
 
         await self._upload_bounded_items(
-            scen_id=scen_id, category=Airline, data_fn=data_fn
+            scen_id=scen_id, category=Airline, items=items
         )
 
-    async def upload_airports(self, scen_id: int, data_fn: str) -> None:
+    async def upload_airports(self, scen_id: int, items: Union[str, list]) -> None:
         """Upload a set of airports defined in a file.
 
         Args:
             scen_id (int): Scenario ID
-            data_fn (str): Filename `.csv` or `.json` defining the airports
+            items (str): Filename `.csv` or `.json` defining the airports
 
-        Where `data_fn` can refer to:
+        Where `items` can refer to:
 
         * a **CSV file**, for instance:
         ```csv
         Name,City,Altitude,Latitude,Longitude,ICAO,IATA
         Geneva,Geneva,431,46.238,6.109,LSGG,GVA
         Madrid,Madrid,619,40.294,-3.724,LEMD,MAD
         London Gatwick,London,60,51.148,-0.19,EGKK,LGW
@@ -107,36 +112,38 @@
         ```json
         [
             {"name": "Geneva", "city": "Geneva", "altitude": 431, "latitude": 46.238, "longitude": 6.109, "icao": "LSGG", "iata": "GVA"},
             {"name": "Madrid", "city": "Madrid", "altitude": 619, "latitude": 40.294, "longitude": -3.724, "icao": "LEMD", "iata": "MAD"},
             {"name": "London Gatwick", "city": "London", "altitude": 60, "latitude": 51.148, "longitude": -0.19, "icao": "EGKK", "iata": "LGW"},
             {"name": "London Heathrow", "city": "London", "altitude": 25, "latitude": 51.477, "longitude": -0.461, "icao": "EGLL", "iata": "LHR"},
         ]
+
+        * a **JSON list** like the previous.
         ```
 
         * **NOTE**: Airport *cities* must reference previously uploaded ``City`` items with the same `City.name`.
 
         Raises:
             ValueError: If file extension is invalid
             FileNotFoundError: If file does not exist
             rmlab_errors.ClientError: If any of the referenced cities does not exist in server
         """
 
         await self._upload_bounded_items(
-            scen_id=scen_id, category=Airport, data_fn=data_fn
+            scen_id=scen_id, category=Airport, items=items
         )
 
-    async def upload_cities(self, scen_id: int, data_fn: str) -> None:
+    async def upload_cities(self, scen_id: int, items: Union[str, list]) -> None:
         """Upload a set of cities defined in a file.
 
         Args:
             scen_id (int): Scenario ID
-            data_fn (str): Filename `.csv` or `.json` defining the cities
+            items (str): Filename `.csv` or `.json` defining the cities
 
-        Where ``data_fn`` can refer to:
+        Where ``items`` can refer to:
 
         * a **CSV file**, for instance:
         ```csv
         Name,Country
         Geneva,Swizterland
         Madrid,Spain
         London,United Kingdom
@@ -145,36 +152,38 @@
         * a **JSON file**, for instance:
         ```json
         [
             {"name": "Geneva", "country": "Switzerland"},
             {"name": "Madrid", "country": "Spain"},
             {"name": "London", "country": "United Kingdom"},
         ]
+
+        * a **JSON list** like the previous.
         ```
 
         * **NOTE**: City *countries* must reference previously uploaded ``Country`` items with the same `Country.name`.
 
         Raises:
             ValueError: If file extension is invalid
             FileNotFoundError: If file does not exist
             rmlab_errors.ClientError: If any of the referenced countries does not exist in server
         """
 
         await self._upload_bounded_items(
-            scen_id=scen_id, category=City, data_fn=data_fn
+            scen_id=scen_id, category=City, items=items
         )
 
-    async def upload_countries(self, scen_id: int, data_fn: str) -> None:
+    async def upload_countries(self, scen_id: int, items: Union[str, list]) -> None:
         """Upload a set of countries defined in a file.
 
         Args:
             scen_id (int): Scenario ID
-            data_fn (str): Filename `.csv` or `.json` defining the countries
+            items (str): Filename `.csv` or `.json` defining the countries
 
-        Where `data_fn` can refer to:
+        Where `items` can refer to:
 
         * a **CSV file**, for instance:
         ```csv
         Name,Currency
         Swizterland,chf
         Spain,eur
         United Kingdom,gbp
@@ -183,45 +192,47 @@
         * a **JSON file**, for instance:
         ```json
         [
             {"name": "Switzerland", "currency": "chf"},
             {"name": "Spain", "currency": "eur"},
             {"name": "United Kingdom", "currency": "gbp"},
         ]
+
+        * a **JSON list** like the previous.
         ```
 
         Raises:
             ValueError: If file extension is invalid
             FileNotFoundError: If file does not exist
         """
 
         await self._upload_bounded_items(
-            scen_id=scen_id, category=Country, data_fn=data_fn
+            scen_id=scen_id, category=Country, items=items
         )
 
     async def upload_schedules(
         self,
         scen_id: int,
-        data_fn: str,
+        items: Union[str, list],
         *,
         citysector_id: Optional[str] = None,
         sector_id: Optional[str] = None,
     ) -> None:
         """Upload a set of flights schedules defined in a file.
 
         Args:
             scen_id (int): Scenario ID
-            data_fn (str): Filename `.csv` or `.json` defining the schedules
+            items (str): Filename `.csv` or `.json` defining the schedules
             citysector_id (Optional[str], optional): A citysector ID if all schedules belong to the same citysector. Defaults to None.
             sector_id (Optional[str], optional): A sector ID if all schedules belong to the same sector. Defaults to None.
 
         Arguments `citysector_id` and `sector_id` are always optional. If provided, concurrent uploads of schedules
             files belonging to different citysectors/sectors are allowed.
 
-        Where `data_fn` can refer to:
+        Where `items` can refer to:
 
         * a **CSV file**, for instance:
         ```csv
         Airline,Aircraft,Origin,Destination,Days of Week,Departure time,Duration,Flight number,Sell before days,From Date,To Date
         MyCarrier,Airbus A320-b,MAD,GVA,-2-4-6-,T08:00,T02:00,2277,15,2022-04-01,2022-05-31
         MyCarrier,Airbus A320-a,MAD,GVA,1-3-5-7,T16:00,T02:00,2278,15,2022-04-01,2022-05-31
         MyCarrier,Airbus A320-b,GVA,MAD,-2-4-6-,T10:30,T01:30,2377,15,2022-04-01,2022-05-31
@@ -232,14 +243,16 @@
         ```json
         [
             {"airline": "MyCarrier", "aircraft": "Airbus A320-b", "origin": "MAD", "destination": "GVA", "days_of_week": "-2-4-6-", "departure_time": "T08:00", "duration": "T02:00", "flight_number": "2277", "sell_before_days": 45, "from_date": "2022-04-01", "to_date": "2022-05-31"},
             {"airline": "MyCarrier", "aircraft": "Airbus A320-b", "origin": "MAD", "destination": "GVA", "days_of_week": "1-3-5-7", "departure_time": "T16:00", "duration": "T02:00", "flight_number": "2278", "sell_before_days": 45, "from_date": "2022-04-01", "to_date": "2022-05-31"},
             {"airline": "MyCarrier", "aircraft": "Airbus A320-b", "origin": "GVA", "destination": "MAD", "days_of_week": "-2-4-6-", "departure_time": "T10:30", "duration": "T01:30", "flight_number": "2377", "sell_before_days": 45, "from_date": "2022-04-01", "to_date": "2022-05-31"},
             {"airline": "MyCarrier", "aircraft": "Airbus A320-b", "origin": "GVA", "destination": "MAD", "days_of_week": "1-3-5-7", "departure_time": "T10:30", "duration": "T01:30", "flight_number": "2378", "sell_before_days": 45, "from_date": "2022-04-01", "to_date": "2022-05-31"},
         ]
+
+        * a **JSON list** like the previous.
         ```
 
         * **NOTE**: Schedule *airlines* must reference previously uploaded ``Airline`` items with the same `Airline.name`.
         * **NOTE**: Schedule *aircrafts* must reference previously uploaded ``Aircraft`` items with the same `Aircraft.model`.
         * **NOTE**: Schedule *origins* must reference previously uploaded ``Airport`` items with the same `Airport.iata`.
         * **NOTE**: Schedule *destinations* must reference previously uploaded ``Airport`` items with the same `Airport.iata`.
         * **NOTE**: No two schedules with overlapping date ranges (*from_date*, *to_date*), and overlapping days of week, with the same *flight_number* are allowed.
@@ -250,75 +263,85 @@
             FileNotFoundError: If file does not exist
             rmlab_errors.ClientError: If any of the previous Notes are not satisfied
         """
 
         await self._upload_unbounded_items(
             scen_id,
             Schedule,
-            data_fn,
+            items,
             citysector_id=citysector_id,
             sector_id=sector_id,
         )
 
     async def upload_batch_core(
         self,
         scen_id: int,
         *,
-        aircraft_items_fn: Optional[str] = None,
-        airline_items_fn: Optional[str] = None,
-        airport_items_fn: Optional[str] = None,
-        city_items_fn: Optional[str] = None,
-        country_items_fn: Optional[str] = None,
-        schedule_items_fn: Optional[str] = None,
+        aircraft_items: Optional[Union[str,list]] = None,
+        airline_items: Optional[Union[str,list]] = None,
+        airport_items: Optional[Union[str,list]] = None,
+        city_items: Optional[Union[str,list]] = None,
+        country_items: Optional[Union[str,list]] = None,
+        schedule_items: Optional[Union[str,list]] = None,
     ):
         """Upload a set of items defined in files to server.
 
         Args:
             scen_id (int): Scenario ID
-            aircraft_items_fn (Optional[str], optional): File name with aircraft items. Defaults to None.
-            airline_items_fn (Optional[str], optional): File name with airline items. Defaults to None.
-            airport_items_fn (Optional[str], optional): File name with airport items. Defaults to None.
-            city_items_fn (Optional[str], optional): File name with city items. Defaults to None.
-            country_items_fn (Optional[str], optional): File name with country items. Defaults to None.
-            schedule_items_fn (Optional[str], optional): File name with flights schedule items. Defaults to None.
+            aircraft_items (Optional[Union[str,list]], optional): Aircraft items. Defaults to None.
+            airline_items (Optional[Union[str,list]], optional): Airline items. Defaults to None.
+            airport_items (Optional[Union[str,list]], optional): Airport items. Defaults to None.
+            city_items (Optional[Union[str,list]], optional): City items. Defaults to None.
+            country_items (Optional[Union[str,list]], optional): Country items. Defaults to None.
+            schedule_items (Optional[Union[str,list]], optional): Flights schedule items. Defaults to None.
 
         Raises:
-            FileNotFoundError: If any of the files does not exist
+            FileNotFoundError: If a file with items doesn't exist
+            TypeError: If non-file items are not list-typed.
+            MultipleError: If several errors happened.
         """
 
         not_existing_fns = [
-            fn
-            for fn in [
-                airport_items_fn,
-                airline_items_fn,
-                airport_items_fn,
-                city_items_fn,
-                country_items_fn,
-                schedule_items_fn,
+            FileNotFoundError(items_fn)
+            for items_fn in [
+                aircraft_items,
+                airline_items,
+                airport_items,
+                city_items,
+                country_items,
+                schedule_items,
             ]
-            if fn and not os.path.exists(fn)
+            if isinstance(items_fn, str) and (not os.path.exists(items_fn))
         ]
 
-        if len(not_existing_fns) > 0:
-            raise FileNotFoundError(not_existing_fns)
+        invalid_types = [
+            TypeError(name)
+            for name, items in [
+                ("aircraft_items", aircraft_items),
+                ("airline_items", airline_items),
+                ("airport_items", airport_items),
+                ("city_items", city_items),
+                ("country_items", country_items),
+                ("schedule_items", schedule_items),
+            ]
+            if (not isinstance(items, list)) and (not isinstance(items, str))
+        ]
+
+        raise_from_list(not_existing_fns + invalid_types)
+
+        if airline_items:
+            await self._upload_bounded_items(scen_id, Airline, items=airline_items)
+
+        if aircraft_items:
+            await self._upload_bounded_items(scen_id, Aircraft, items=aircraft_items)
+
+        if country_items:
+            await self._upload_bounded_items(scen_id, Country, items=country_items)
+
+        if city_items:
+            await self._upload_bounded_items(scen_id, City, items=city_items)
 
-        if airline_items_fn:
-            await self._upload_bounded_items(scen_id, Airline, data_fn=airline_items_fn)
+        if airport_items:
+            await self._upload_bounded_items(scen_id, Airport, items=airport_items)
 
-        if aircraft_items_fn:
-            await self._upload_bounded_items(
-                scen_id, Aircraft, data_fn=aircraft_items_fn
-            )
-
-        if country_items_fn:
-            await self._upload_bounded_items(scen_id, Country, data_fn=country_items_fn)
-
-        if city_items_fn:
-            await self._upload_bounded_items(scen_id, City, data_fn=city_items_fn)
-
-        if airport_items_fn:
-            await self._upload_bounded_items(scen_id, Airport, data_fn=airport_items_fn)
-
-        if schedule_items_fn:
-            await self._upload_unbounded_items(
-                scen_id, Schedule, data_fn=schedule_items_fn
-            )
+        if schedule_items:
+            await self._upload_unbounded_items(scen_id, Schedule, items=schedule_items)
```

### Comparing `rmlab-0.3.0/src/rmlab/api/upload/flight_data.py` & `rmlab-0.4.0/src/rmlab/api/upload/flight_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 class APIUploadFlightData(APIUploadInternal):
     """Interface to upload flight data to server"""
 
     async def upload_flights(
         self,
         scen_id: int,
-        data_fn: str,
+        items: Union[str, list],
         *,
         citysector_id: Optional[str] = None,
         sector_id: Optional[str] = None,
     ) -> None:
         """Upload a set of flights defined in a file.
 
         Args:
@@ -43,19 +43,21 @@
 
         * a **JSON file**, for instance:
         ```json
         [
             {"airline": "MyCarrier", "aircraft": "Airbus A320-b", "origin": "MAD", "destination": "GVA", "flight_number": "2277", "on_sale_date": "2022-04-01", "departure_date": "2022-05-15", "departure_time": "T16:30", "duration": "T02:00", },
             {"airline": "MyCarrier", "aircraft": "Airbus A320-b", "origin": "MAD", "destination": "GVA", "flight_number": "2277", "on_sale_date": "2022-04-01", "departure_date": "2022-05-17", "departure_time": "T20:30", "duration": "T02:00", },
         ]
+
+        * a **JSON list** like the previous.
         ```
         """
 
         await self._upload_unbounded_items(
-            scen_id, Flight, data_fn, citysector_id=citysector_id, sector_id=sector_id
+            scen_id, Flight, items, citysector_id=citysector_id, sector_id=sector_id
         )
 
     async def upload_flights_data(
         self,
         scen_id: int,
         flights_data: List[
             Union[
@@ -86,46 +88,46 @@
         """
 
         if citysector_id is None and sector_id is None:
             raise ValueError(
                 f"Require definition of either `citysector_id` or `sector_id`"
             )
 
-        endpoint_limit = self._api_endpoints_limits.data_flight_post
+        # TODO endpoint_limit = self._api_endpoints_limits.data_flight_post
 
-        if len(flights_data) > endpoint_limit:
+        # if len(flights_data) > endpoint_limit:
 
-            # Sequentially upload data in chunks to keep the request payloads and server load controlled
+        #     # Sequentially upload data in chunks to keep the request payloads and server load controlled
 
-            for chunk_start in range(0, len(flights_data), endpoint_limit):
+        #     for chunk_start in range(0, len(flights_data), endpoint_limit):
 
-                chunk_end = chunk_start + endpoint_limit
-                if chunk_end > len(flights_data):
-                    chunk_end = -1
-
-                await run_async_tasks(
-                    [
-                        self._upload_flight_data(
-                            scen_id,
-                            flight_data,
-                            citysector_id=citysector_id,
-                            sector_id=sector_id,
-                        )
-                        for flight_data in flights_data[chunk_start:chunk_end]
-                    ],
-                    return_results=False,
+        #         chunk_end = chunk_start + endpoint_limit
+        #         if chunk_end > len(flights_data):
+        #             chunk_end = -1
+
+        #         await run_async_tasks(
+        #             [
+        #                 self._upload_flight_data(
+        #                     scen_id,
+        #                     flight_data,
+        #                     citysector_id=citysector_id,
+        #                     sector_id=sector_id,
+        #                 )
+        #                 for flight_data in flights_data[chunk_start:chunk_end]
+        #             ],
+        #             return_results=False,
+        #         )
+
+        # else:
+
+        await run_async_tasks(
+            [
+                self._upload_flight_data(
+                    scen_id,
+                    flight_data,
+                    citysector_id=citysector_id,
+                    sector_id=sector_id,
                 )
-
-        else:
-
-            await run_async_tasks(
-                [
-                    self._upload_flight_data(
-                        scen_id,
-                        flight_data,
-                        citysector_id=citysector_id,
-                        sector_id=sector_id,
-                    )
-                    for flight_data in flights_data
-                ],
-                return_results=False,
-            )
+                for flight_data in flights_data
+            ],
+            return_results=False,
+        )
```

### Comparing `rmlab-0.3.0/src/rmlab/api/upload/parametric/customers.py` & `rmlab-0.4.0/src/rmlab/api/upload/parametric/customers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,86 @@
 """Interface for uploading pricing models data."""
 
 import os
-from typing import List, Optional
+from typing import List, Optional, Union
+from rmlab_errors import raise_from_list
 from rmlab._api.upload import APIUploadInternal
 from rmlab._data.enums import (
     CustomersModelKind,
     ParametricModelKind,
 )
 
 
 class APIUploadCustomersModels(APIUploadInternal):
     """Exposes functions for uploading customers models data to the server."""
 
     async def upload_customers_request_model(
         self,
         scen_id: int,
-        data_fn: str,
+        content: Union[str, dict],
     ) -> None:
         """Upload to server a parametric model defined in file, modelling how customers request books.
 
         Args:
             scen_id (int): Scenario ID
-            data_fn (str): Filename (.json) defining the parametric model
+            content (str): Request model as file or json dict (require `id` identifier field if the latter)
         """
 
         await self._upload_parametric_model(
             scen_id,
             parametric_kind=ParametricModelKind.CUSTOMERS,
             kind=CustomersModelKind.REQUEST,
-            data_fn=data_fn,
+            content=content,
         )
 
     async def upload_customers_choice_model(
         self,
         scen_id: int,
-        data_fn: str,
+        content: Union[str, dict],
     ) -> None:
         """Upload to server a parametric model defined in file, modelling how customers choose between competing book offers.
 
         Args:
             scen_id (int): Scenario ID
-            data_fn (str): Filename (.json) defining the parametric model
+            content (str): Request model as file or json dict (require `id` identifier field if the latter)
         """
 
         await self._upload_parametric_model(
             scen_id,
             parametric_kind=ParametricModelKind.CUSTOMERS,
             kind=CustomersModelKind.CHOICE,
-            data_fn=data_fn,
+            content=content,
         )
 
     async def upload_batch_customers_models(
         self,
         scen_id: int,
         *,
-        request_models_fns: Optional[List[str]] = None,
-        choice_models_fns: Optional[List[str]] = None,
+        request_models: Optional[List[Union[str, dict]]] = None,
+        choice_models: Optional[List[Union[str, dict]]] = None,
     ):
-        if request_models_fns is None:
-            request_models_fns = list()
-        if choice_models_fns is None:
-            request_models_fns = list()
-
-        not_existing_fns = [
-            fn for fn in request_models_fns if fn and not os.path.exists(fn)
-        ] + [fn for fn in choice_models_fns if fn and not os.path.exists(fn)]
+        if request_models is None:
+            request_models = list()
+        if choice_models is None:
+            request_models = list()
+
+        not_found_errors = \
+            [FileNotFoundError(fn) for fn in request_models if isinstance(fn, str) and not os.path.exists(fn)] + \
+            [FileNotFoundError(fn) for fn in choice_models if isinstance(fn, str) and not os.path.exists(fn)]
+        
+        type_errors = \
+            [TypeError(cnt) for cnt in request_models if (not isinstance(cnt, dict)) and (not isinstance(cnt, str))] + \
+            [TypeError(cnt) for cnt in choice_models if not isinstance(cnt, dict) and (not isinstance(cnt, str))]
 
-        if len(not_existing_fns) > 0:
-            raise FileNotFoundError(not_existing_fns)
+        raise_from_list(not_found_errors + type_errors)
 
-        for crm in request_models_fns:
+        for crm in request_models:
 
             await self._upload_parametric_model(
                 scen_id, ParametricModelKind.CUSTOMERS, CustomersModelKind.REQUEST, crm
             )
 
-        for ccm in choice_models_fns:
+        for ccm in choice_models:
 
             await self._upload_parametric_model(
                 scen_id, ParametricModelKind.CUSTOMERS, CustomersModelKind.CHOICE, ccm
             )
```

### Comparing `rmlab-0.3.0/src/rmlab/data/__init__.py` & `rmlab-0.4.0/src/rmlab/data/__init__.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.3.0/src/rmlab/data/items.py` & `rmlab-0.4.0/src/rmlab/data/items.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 This script provides dataclasses that represent the relational data components in the server.
 """
-
+import logging
 from typing import List, Union
 from dataclasses import dataclass
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 import importlib
 import inspect
 from rmlab._data.enums import CurrencyKind, DayOfWeek
 
 from rmlab._data.types import (
     AirlineLocation,
     BoundedItem,
@@ -17,14 +17,15 @@
     DateFormat,
     DateTimeMinFormat,
     DerivedItem,
     PricingModelHolder,
     UnboundedItem,
 )
 
+_Logger = logging.getLogger(__name__)
 
 @dataclass
 class PModel(BoundedItem, CoreItem):
     """Item holding a set of parameters.
 
     Args:
         filename (str): Name of file storing the parameters
@@ -207,46 +208,55 @@
 
     airline_id: str
     aircraft_id: str
     origin_id: str
     destination_id: str
     days_of_week: List[DayOfWeek]
     departure_time: timedelta
-    duration: int
+    duration: timedelta
     flight_number: str
     sell_before_days: int
-    from_date: str
-    to_date: str
+    from_date: datetime
+    to_date: datetime
     sector_id: str
     citysector_id: str
     route_id: str
     cityroute_id: str
     from_date_load: datetime
     to_date_load: datetime
     from_date_departure: datetime
     to_date_departure: datetime
 
     def __post_init__(self):
 
         self.sell_before_days = int(self.sell_before_days)
 
+        if isinstance(self.days_of_week, int):
+            self.days_of_week = str(self.days_of_week)
+
         self.days_of_week = [
             DayOfWeek.int_to_enum_value(int(d))
             for d in self.days_of_week.replace("-", "")
         ]
+
         self.departure_time = self.departure_time
 
-        self.from_date = datetime.strptime(self.from_date, DateFormat)
-        self.to_date = datetime.strptime(self.to_date, DateFormat)
-        self.from_date_load = datetime.strptime(self.from_date_load, DateFormat)
-        self.to_date_load = datetime.strptime(self.to_date_load, DateFormat)
-        self.from_date_departure = datetime.strptime(
-            self.from_date_departure, DateFormat
-        )
-        self.to_date_departure = datetime.strptime(self.to_date_departure, DateFormat)
+        if isinstance(self.from_date, str):
+            self.from_date = datetime.strptime(self.from_date, DateFormat).replace(tzinfo=timezone.utc)
+        elif not isinstance(self.from_date, datetime):
+            raise TypeError(f"Expected string or datetime in field `from_date`")
+        if isinstance(self.to_date, str):
+            self.to_date = datetime.strptime(self.to_date, DateFormat).replace(tzinfo=timezone.utc)
+        elif not isinstance(self.to_date, datetime):
+            raise TypeError(f"Expected string or datetime in field `to_date`")
+        # Expect following datetime fields to be strings since they come from server
+        self.from_date_load = datetime.strptime(self.from_date_load, DateFormat).replace(tzinfo=timezone.utc)
+        self.to_date_load = datetime.strptime(self.to_date_load, DateFormat).replace(tzinfo=timezone.utc)
+        self.from_date_departure = datetime.strptime(self.from_date_departure, DateFormat).replace(tzinfo=timezone.utc)
+        self.to_date_departure = datetime.strptime(self.to_date_departure, DateFormat).replace(tzinfo=timezone.utc)
 
         self.departure_time = timedelta(minutes=int(self.departure_time))
         self.duration = timedelta(minutes=int(self.duration))
 
 
 @dataclass
 class Flight(UnboundedItem, DerivedItem, PricingModelHolder):
@@ -281,18 +291,16 @@
     highest_pps: int
 
     def __post_init__(self):
         self.seat_capacity = int(self.seat_capacity)
         self.fares = self.fares.split("-")
         self.lowest_pps = self.lowest_pps
         self.highest_pps = self.highest_pps
-        self.onsale_date_time = datetime.strptime(self.onsale_date_time, DateFormat)
-        self.departure_date_time = datetime.strptime(
-            self.departure_date_time, DateTimeMinFormat
-        )
+        self.onsale_date_time = datetime.strptime(self.onsale_date_time, DateFormat).replace(tzinfo=timezone.utc)
+        self.departure_date_time = datetime.strptime(self.departure_date_time, DateTimeMinFormat).replace(tzinfo=timezone.utc)
 
 
 AnyAirlineLocationType = Union[Sector, CitySector, Route, CityRoute]
 AnyBoundedType = Union[
     PModel,
     Airline,
     Aircraft,
```

### Comparing `rmlab-0.3.0/src/rmlab/data/parametric/customers_choice.py` & `rmlab-0.4.0/src/rmlab/data/parametric/customers_choice.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,15 +252,15 @@
 
         if len(models) > 1:
             return MultipleChoiceModels(
                 id=model_id,
                 filename=filename,
                 cnt=json.dumps(content),
                 hash=md5hash,
-                kind=CustomersModelKind.REQUEST,
+                kind=CustomersModelKind.CHOICE,
                 extension=FileExtensions.JSON,
                 models=models,
             )
         else:
             return models[0]
 
     else:
```

### Comparing `rmlab-0.3.0/src/rmlab/data/parametric/customers_request.py` & `rmlab-0.4.0/src/rmlab/data/parametric/customers_request.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.3.0/src/rmlab/data/parametric/filter.py` & `rmlab-0.4.0/src/rmlab/data/parametric/filter.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.3.0/src/rmlab/data/parametric/pricing_optimizer.py` & `rmlab-0.4.0/src/rmlab/data/parametric/pricing_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 A pricing optimizer completely defines the revenue optimization strategy to apply to 
 flights. In particular, it is needed to define:
 
 1. A **schedule**, to define *when* to trigger optimization passes.
 
 2. A **selector**, to specify the *inputs* of the optimization passes for each flight.
 
-3. An **operator**, to specify the set of *actions* and *algorithms* that will run on the input data, encompasing:
+3. An **operator**, to specify the set of *actions* and *algorithms* that will run on the input data.
 """
 
 
 from dataclasses import dataclass
 import json
 from typing import Any, List, Mapping, Optional, Union
 
@@ -176,35 +176,34 @@
 
     ```py
     op = OptimizerOperator(
       forecaster_type="q-forecast",
       maximizer=OptimizerMaximizer(...),
       aggregate_type="exponential",
       aggregate_value=0.5
-      effects="commit"
+      effects="promote-dynamic-bc-thresholds"
     )
     ```
 
 
     **Example 2**
 
     To create an operator that:
 
-    1. Runs *bayesian* forecaster on all input data
+    1. Runs *Q-Forecast* forecaster on all input data
     2. Aggregates forecast data of all flights *uniformly*
     3. Do not apply the results to the thresholds
 
     we create an operator instance as:
 
     ```py
     op = OptimizerOperator(
       forecaster_type="q-forecast",
       maximizer=OptimizerMaximizer(...),
-      aggregate_type="exponential",
-      aggregate_value=0.5
+      aggregate_type="uniform",
       effects="none"
     )
     ```
 
     """
 
     forecaster_type: OptimizationForecasterKind
```

### Comparing `rmlab-0.3.0/src/rmlab/data/parametric/pricing_range.py` & `rmlab-0.4.0/src/rmlab/data/parametric/pricing_range.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.3.0/src/rmlab/data/scenario.py` & `rmlab-0.4.0/src/rmlab/data/scenario.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 This script provides dataclasses that represent a global information of scenarios.
 """
 
 from dataclasses import dataclass, field
-from datetime import datetime
+from datetime import datetime, timezone
 from typing import List
 
 from rmlab._data.enums import ScenarioDayStatus, ScenarioState
 from rmlab._data.types import DateFormat, DateTimeSecFormat
 
 
 @dataclass
@@ -50,24 +50,22 @@
     checkpoints: List[datetime]
     upload_time: datetime
     state: ScenarioState
 
     def __post_init__(self):
 
         self.day_status = ScenarioDayStatus.str_to_enum_value(self.day_status)
-        self.current = datetime.strptime(self.current, DateFormat)
-        self.next = datetime.strptime(self.next, DateFormat)
-        self.first_flight_load = datetime.strptime(self.first_flight_load, DateFormat)
-        self.last_flight_departure = datetime.strptime(
-            self.last_flight_departure, DateFormat
-        )
+        self.current = datetime.strptime(self.current, DateFormat).replace(tzinfo=timezone.utc)
+        self.next = datetime.strptime(self.next, DateFormat).replace(tzinfo=timezone.utc)
+        self.first_flight_load = datetime.strptime(self.first_flight_load, DateFormat).replace(tzinfo=timezone.utc)
+        self.last_flight_departure = datetime.strptime(self.last_flight_departure, DateFormat).replace(tzinfo=timezone.utc)
         self.checkpoints = [
-            datetime.strptime(chp, DateFormat) for chp in self.checkpoints
+            datetime.strptime(chp, DateFormat).replace(tzinfo=timezone.utc) for chp in self.checkpoints
         ]
-        self.upload_time = datetime.strptime(self.upload_time, DateTimeSecFormat)
+        self.upload_time = datetime.strptime(self.upload_time, DateTimeSecFormat).replace(tzinfo=timezone.utc)
 
 
 @dataclass
 class ItemsCount(Scenario):
     """Counters of items of bounded categories.
 
     Args:
```

### Comparing `rmlab-0.3.0/src/rmlab.egg-info/PKG-INFO` & `rmlab-0.4.0/src/rmlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmlab
-Version: 0.3.0
+Version: 0.4.0
 Summary: RMLab python client
 Home-page: https://rmlab.ai
 Author: Anton Rey
 Author-email: aanton.rv@gmail.com
 Project-URL: Bug Tracker, https://rmlab.ai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rmlab-0.3.0/src/rmlab.egg-info/SOURCES.txt` & `rmlab-0.4.0/src/rmlab.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 src/rmlab/api/fetch/core.py
 src/rmlab/api/fetch/flight_data.py
 src/rmlab/api/fetch/parametric.py
 src/rmlab/api/observability/__init__.py
 src/rmlab/api/operations/__init__.py
 src/rmlab/api/operations/optimization.py
 src/rmlab/api/operations/simulation.py
+src/rmlab/api/persistence/__init__.py
 src/rmlab/api/upload/__init__.py
 src/rmlab/api/upload/core.py
 src/rmlab/api/upload/flight_data.py
 src/rmlab/api/upload/parametric/__init__.py
 src/rmlab/api/upload/parametric/customers.py
 src/rmlab/api/upload/parametric/filters.py
 src/rmlab/api/upload/parametric/pricing.py
```

