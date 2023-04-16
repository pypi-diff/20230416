# Comparing `tmp/network_scanner_kbk-0.0.1.tar.gz` & `tmp/network_scanner_kbk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "C:\Brian\2023\Joby\Challenge\network_scanner_kbk\dist\.tmp-nyn1ndau\network_scanner_kbk-0.0.2.tar", last modified: Sun Apr 16 21:43:36 2023, max compression
```

## Comparing `network_scanner_kbk-0.0.1.tar` & `network_scanner_kbk-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,17 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 network_scanner_kbk-0.0.1/src/__init__.py
--rw-r--r--   0        0        0     7325 2020-02-02 00:00:00.000000 network_scanner_kbk-0.0.1/src/network_scanner.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 network_scanner_kbk-0.0.1/src/ping_example.py
--rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 network_scanner_kbk-0.0.1/test/test_network_scanner.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 network_scanner_kbk-0.0.1/LICENSE
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 network_scanner_kbk-0.0.1/README.md
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 network_scanner_kbk-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 network_scanner_kbk-0.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 21:43:36.687541 network_scanner_kbk-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-04-16 17:12:52.000000 network_scanner_kbk-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      285 2023-04-16 21:43:36.685548 network_scanner_kbk-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      114 2023-04-16 15:31:31.000000 network_scanner_kbk-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 21:43:36.657204 network_scanner_kbk-0.0.2/network_scanner_kbk.egg-info/
+-rw-rw-rw-   0        0        0      285 2023-04-16 21:43:36.000000 network_scanner_kbk-0.0.2/network_scanner_kbk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-04-16 21:43:36.000000 network_scanner_kbk-0.0.2/network_scanner_kbk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 21:43:36.000000 network_scanner_kbk-0.0.2/network_scanner_kbk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-04-16 21:43:36.000000 network_scanner_kbk-0.0.2/network_scanner_kbk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 21:43:36.687541 network_scanner_kbk-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      371 2023-04-16 21:30:39.000000 network_scanner_kbk-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 21:43:36.677542 network_scanner_kbk-0.0.2/src/
+-rw-rw-rw-   0        0        0        0 2023-04-16 15:33:58.000000 network_scanner_kbk-0.0.2/src/__init__.py
+-rw-rw-rw-   0        0        0      304 2023-04-15 22:45:38.000000 network_scanner_kbk-0.0.2/src/example.py
+-rw-rw-rw-   0        0        0     7325 2023-04-16 17:15:22.000000 network_scanner_kbk-0.0.2/src/network_scanner.py
+drwxrwxrwx   0        0        0        0 2023-04-16 21:43:36.682540 network_scanner_kbk-0.0.2/test/
+-rw-rw-rw-   0        0        0     3408 2023-04-15 20:13:16.000000 network_scanner_kbk-0.0.2/test/test_network_scanner.py
```

### Comparing `network_scanner_kbk-0.0.1/src/network_scanner.py` & `network_scanner_kbk-0.0.2/src/network_scanner.py`

 * *Files identical despite different names*

### Comparing `network_scanner_kbk-0.0.1/test/test_network_scanner.py` & `network_scanner_kbk-0.0.2/test/test_network_scanner.py`

 * *Files identical despite different names*

### Comparing `network_scanner_kbk-0.0.1/LICENSE` & `network_scanner_kbk-0.0.2/LICENSE`

 * *Files identical despite different names*

