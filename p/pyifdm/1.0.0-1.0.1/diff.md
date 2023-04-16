# Comparing `tmp/pyifdm-1.0.0.tar.gz` & `tmp/pyifdm-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyifdm-1.0.0.tar", last modified: Mon Jan 16 10:06:55 2023, max compression
+gzip compressed data, was "pyifdm-1.0.1.tar", last modified: Sun Apr 16 13:07:44 2023, max compression
```

## Comparing `pyifdm-1.0.0.tar` & `pyifdm-1.0.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-01-16 10:06:55.377340 pyifdm-1.0.0/
--rw-rw-rw-   0        0        0     1095 2022-12-20 17:49:15.000000 pyifdm-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    10978 2023-01-16 10:06:55.376339 pyifdm-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    10486 2023-01-10 10:59:43.000000 pyifdm-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-01-16 10:06:54.938473 pyifdm-1.0.0/pyifdm/
--rw-rw-rw-   0        0        0       97 2022-12-21 09:03:53.000000 pyifdm-1.0.0/pyifdm/__init__.py
--rw-rw-rw-   0        0        0     2114 2023-01-10 10:55:13.000000 pyifdm-1.0.0/pyifdm/correlations.py
--rw-rw-rw-   0        0        0     1410 2023-01-05 19:12:54.000000 pyifdm-1.0.0/pyifdm/helpers.py
-drwxrwxrwx   0        0        0        0 2023-01-16 10:06:55.110100 pyifdm-1.0.0/pyifdm/methods/
--rw-rw-rw-   0        0        0      301 2022-12-21 07:12:52.000000 pyifdm-1.0.0/pyifdm/methods/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-16 10:06:55.138372 pyifdm-1.0.0/pyifdm/methods/aras/
--rw-rw-rw-   0        0        0       17 2022-12-21 10:13:28.000000 pyifdm-1.0.0/pyifdm/methods/aras/__init__.py
--rw-rw-rw-   0        0        0     2000 2023-01-06 10:24:02.000000 pyifdm-1.0.0/pyifdm/methods/aras/ifs.py
-drwxrwxrwx   0        0        0        0 2023-01-16 10:06:55.156185 pyifdm-1.0.0/pyifdm/methods/codas/
--rw-rw-rw-   0        0        0       17 2022-12-21 10:18:29.000000 pyifdm-1.0.0/pyifdm/methods/codas/__init__.py
--rw-rw-rw-   0        0        0     4380 2023-01-02 14:07:46.000000 pyifdm-1.0.0/pyifdm/methods/codas/ifs.py
-drwxrwxrwx   0        0        0        0 2023-01-16 10:06:55.175018 pyifdm-1.0.0/pyifdm/methods/copras/
--rw-rw-rw-   0        0        0       17 2022-12-21 10:25:39.000000 pyifdm-1.0.0/pyifdm/methods/copras/__init__.py
--rw-rw-rw-   0        0        0     1902 2023-01-02 14:07:53.000000 pyifdm-1.0.0/pyifdm/methods/copras/ifs.py
-drwxrwxrwx   0        0        0        0 2023-01-16 10:06:55.194177 pyifdm-1.0.0/pyifdm/methods/edas/
--rw-rw-rw-   0        0        0       17 2022-12-21 10:26:45.000000 pyifdm-1.0.0/pyifdm/methods/edas/__init__.py
--rw-rw-rw-   0        0        0     2151 2023-01-02 14:08:00.000000 pyifdm-1.0.0/pyifdm/methods/edas/ifs.py
--rw-rw-rw-   0        0        0     1753 2023-01-10 10:14:57.000000 pyifdm-1.0.0/pyifdm/methods/if_aras.py
--rw-rw-rw-   0        0        0     2167 2023-01-10 09:51:38.000000 pyifdm-1.0.0/pyifdm/methods/if_codas.py
--rw-rw-rw-   0        0        0     1585 2023-01-10 10:24:54.000000 pyifdm-1.0.0/pyifdm/methods/if_copras.py
--rw-rw-rw-   0        0        0     1641 2023-01-10 09:58:57.000000 pyifdm-1.0.0/pyifdm/methods/if_edas.py
--rw-rw-rw-   0        0        0     2150 2023-01-10 09:59:09.000000 pyifdm-1.0.0/pyifdm/methods/if_mabac.py
--rw-rw-rw-   0        0        0     1948 2023-01-10 09:59:19.000000 pyifdm-1.0.0/pyifdm/methods/if_mairca.py
--rw-rw-rw-   0        0        0     1670 2023-01-10 10:25:13.000000 pyifdm-1.0.0/pyifdm/methods/if_moora.py
--rw-rw-rw-   0        0        0     1742 2023-01-02 13:54:13.000000 pyifdm-1.0.0/pyifdm/methods/if_topsis.py
--rw-rw-rw-   0        0        0     1747 2023-01-10 10:15:11.000000 pyifdm-1.0.0/pyifdm/methods/if_vikor.py
-drwxrwxrwx   0        0        0        0 2023-01-16 10:06:55.268958 pyifdm-1.0.0/pyifdm/methods/ifs/
--rw-rw-rw-   0        0        0       74 2022-12-21 09:03:36.000000 pyifdm-1.0.0/pyifdm/methods/ifs/__init__.py
--rw-rw-rw-   0        0        0     6195 2023-01-10 12:19:53.000000 pyifdm-1.0.0/pyifdm/methods/ifs/distance.py
--rw-rw-rw-   0        0        0     3809 2023-01-10 11:45:00.000000 pyifdm-1.0.0/pyifdm/methods/ifs/normalization.py
--rw-rw-rw-   0        0        0     8489 2023-01-10 10:54:32.000000 pyifdm-1.0.0/pyifdm/methods/ifs/score.py
-drwxrwxrwx   0        0        0        0 2023-01-16 10:06:55.291332 pyifdm-1.0.0/pyifdm/methods/mabac/
--rw-rw-rw-   0        0        0       17 2022-12-21 10:29:01.000000 pyifdm-1.0.0/pyifdm/methods/mabac/__init__.py
--rw-rw-rw-   0        0        0     3578 2023-01-02 14:08:11.000000 pyifdm-1.0.0/pyifdm/methods/mabac/ifs.py
-drwxrwxrwx   0        0        0        0 2023-01-16 10:06:55.312973 pyifdm-1.0.0/pyifdm/methods/mairca/
--rw-rw-rw-   0        0        0       17 2022-12-21 10:29:57.000000 pyifdm-1.0.0/pyifdm/methods/mairca/__init__.py
--rw-rw-rw-   0        0        0     2883 2023-01-06 10:44:50.000000 pyifdm-1.0.0/pyifdm/methods/mairca/ifs.py
-drwxrwxrwx   0        0        0        0 2023-01-16 10:06:55.331789 pyifdm-1.0.0/pyifdm/methods/moora/
--rw-rw-rw-   0        0        0       17 2022-12-21 10:34:57.000000 pyifdm-1.0.0/pyifdm/methods/moora/__init__.py
--rw-rw-rw-   0        0        0     2606 2023-01-02 14:08:25.000000 pyifdm-1.0.0/pyifdm/methods/moora/ifs.py
-drwxrwxrwx   0        0        0        0 2023-01-16 10:06:55.352687 pyifdm-1.0.0/pyifdm/methods/topsis/
--rw-rw-rw-   0        0        0       17 2022-12-21 10:36:35.000000 pyifdm-1.0.0/pyifdm/methods/topsis/__init__.py
--rw-rw-rw-   0        0        0     3200 2023-01-02 14:08:32.000000 pyifdm-1.0.0/pyifdm/methods/topsis/ifs.py
--rw-rw-rw-   0        0        0     4168 2023-01-16 10:05:50.000000 pyifdm-1.0.0/pyifdm/methods/validator.py
-drwxrwxrwx   0        0        0        0 2023-01-16 10:06:55.368554 pyifdm-1.0.0/pyifdm/methods/vikor/
--rw-rw-rw-   0        0        0       17 2022-12-21 10:39:26.000000 pyifdm-1.0.0/pyifdm/methods/vikor/__init__.py
--rw-rw-rw-   0        0        0     3212 2023-01-06 11:15:02.000000 pyifdm-1.0.0/pyifdm/methods/vikor/ifs.py
--rw-rw-rw-   0        0        0     5699 2023-01-10 10:56:55.000000 pyifdm-1.0.0/pyifdm/weights.py
-drwxrwxrwx   0        0        0        0 2023-01-16 10:06:54.970129 pyifdm-1.0.0/pyifdm.egg-info/
--rw-rw-rw-   0        0        0    10978 2023-01-16 10:06:54.000000 pyifdm-1.0.0/pyifdm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1229 2023-01-16 10:06:54.000000 pyifdm-1.0.0/pyifdm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-16 10:06:54.000000 pyifdm-1.0.0/pyifdm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-01-16 10:06:54.000000 pyifdm-1.0.0/pyifdm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-01-16 10:06:54.000000 pyifdm-1.0.0/pyifdm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-16 10:06:55.377717 pyifdm-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      798 2023-01-02 11:09:37.000000 pyifdm-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:44.456901 pyifdm-1.0.1/
+-rw-rw-rw-   0        0        0     1095 2022-12-20 17:49:15.000000 pyifdm-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    10978 2023-04-16 13:07:44.455903 pyifdm-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10486 2023-01-10 10:59:43.000000 pyifdm-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:44.343988 pyifdm-1.0.1/pyifdm/
+-rw-rw-rw-   0        0        0       97 2022-12-21 09:03:53.000000 pyifdm-1.0.1/pyifdm/__init__.py
+-rw-rw-rw-   0        0        0     2114 2023-01-10 10:55:13.000000 pyifdm-1.0.1/pyifdm/correlations.py
+-rw-rw-rw-   0        0        0     1410 2023-01-05 19:12:54.000000 pyifdm-1.0.1/pyifdm/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:44.377713 pyifdm-1.0.1/pyifdm/methods/
+-rw-rw-rw-   0        0        0      301 2022-12-21 07:12:52.000000 pyifdm-1.0.1/pyifdm/methods/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:44.381713 pyifdm-1.0.1/pyifdm/methods/aras/
+-rw-rw-rw-   0        0        0       17 2022-12-21 10:13:28.000000 pyifdm-1.0.1/pyifdm/methods/aras/__init__.py
+-rw-rw-rw-   0        0        0     2000 2023-01-06 10:24:02.000000 pyifdm-1.0.1/pyifdm/methods/aras/ifs.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:44.385118 pyifdm-1.0.1/pyifdm/methods/codas/
+-rw-rw-rw-   0        0        0       17 2022-12-21 10:18:29.000000 pyifdm-1.0.1/pyifdm/methods/codas/__init__.py
+-rw-rw-rw-   0        0        0     4380 2023-01-02 14:07:46.000000 pyifdm-1.0.1/pyifdm/methods/codas/ifs.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:44.390117 pyifdm-1.0.1/pyifdm/methods/copras/
+-rw-rw-rw-   0        0        0       17 2022-12-21 10:25:39.000000 pyifdm-1.0.1/pyifdm/methods/copras/__init__.py
+-rw-rw-rw-   0        0        0     1902 2023-01-02 14:07:53.000000 pyifdm-1.0.1/pyifdm/methods/copras/ifs.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:44.395118 pyifdm-1.0.1/pyifdm/methods/edas/
+-rw-rw-rw-   0        0        0       17 2022-12-21 10:26:45.000000 pyifdm-1.0.1/pyifdm/methods/edas/__init__.py
+-rw-rw-rw-   0        0        0     2151 2023-01-02 14:08:00.000000 pyifdm-1.0.1/pyifdm/methods/edas/ifs.py
+-rw-rw-rw-   0        0        0     2388 2023-04-16 12:50:12.000000 pyifdm-1.0.1/pyifdm/methods/if_aras.py
+-rw-rw-rw-   0        0        0     2798 2023-04-16 12:50:51.000000 pyifdm-1.0.1/pyifdm/methods/if_codas.py
+-rw-rw-rw-   0        0        0     2216 2023-04-16 12:51:26.000000 pyifdm-1.0.1/pyifdm/methods/if_copras.py
+-rw-rw-rw-   0        0        0     2280 2023-04-16 12:52:08.000000 pyifdm-1.0.1/pyifdm/methods/if_edas.py
+-rw-rw-rw-   0        0        0     2781 2023-04-16 12:52:55.000000 pyifdm-1.0.1/pyifdm/methods/if_mabac.py
+-rw-rw-rw-   0        0        0     2579 2023-04-16 12:53:43.000000 pyifdm-1.0.1/pyifdm/methods/if_mairca.py
+-rw-rw-rw-   0        0        0     2301 2023-04-16 12:54:34.000000 pyifdm-1.0.1/pyifdm/methods/if_moora.py
+-rw-rw-rw-   0        0        0     2373 2023-04-16 12:55:08.000000 pyifdm-1.0.1/pyifdm/methods/if_topsis.py
+-rw-rw-rw-   0        0        0     2453 2023-04-16 12:56:41.000000 pyifdm-1.0.1/pyifdm/methods/if_vikor.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:44.409115 pyifdm-1.0.1/pyifdm/methods/ifs/
+-rw-rw-rw-   0        0        0       74 2022-12-21 09:03:36.000000 pyifdm-1.0.1/pyifdm/methods/ifs/__init__.py
+-rw-rw-rw-   0        0        0     6195 2023-01-10 12:19:53.000000 pyifdm-1.0.1/pyifdm/methods/ifs/distance.py
+-rw-rw-rw-   0        0        0     3809 2023-01-10 11:45:00.000000 pyifdm-1.0.1/pyifdm/methods/ifs/normalization.py
+-rw-rw-rw-   0        0        0     8489 2023-01-10 10:54:32.000000 pyifdm-1.0.1/pyifdm/methods/ifs/score.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:44.413116 pyifdm-1.0.1/pyifdm/methods/mabac/
+-rw-rw-rw-   0        0        0       17 2022-12-21 10:29:01.000000 pyifdm-1.0.1/pyifdm/methods/mabac/__init__.py
+-rw-rw-rw-   0        0        0     3578 2023-01-02 14:08:11.000000 pyifdm-1.0.1/pyifdm/methods/mabac/ifs.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:44.417120 pyifdm-1.0.1/pyifdm/methods/mairca/
+-rw-rw-rw-   0        0        0       17 2022-12-21 10:29:57.000000 pyifdm-1.0.1/pyifdm/methods/mairca/__init__.py
+-rw-rw-rw-   0        0        0     2883 2023-01-06 10:44:50.000000 pyifdm-1.0.1/pyifdm/methods/mairca/ifs.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:44.420121 pyifdm-1.0.1/pyifdm/methods/moora/
+-rw-rw-rw-   0        0        0       17 2022-12-21 10:34:57.000000 pyifdm-1.0.1/pyifdm/methods/moora/__init__.py
+-rw-rw-rw-   0        0        0     2606 2023-01-02 14:08:25.000000 pyifdm-1.0.1/pyifdm/methods/moora/ifs.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:44.425120 pyifdm-1.0.1/pyifdm/methods/topsis/
+-rw-rw-rw-   0        0        0       17 2022-12-21 10:36:35.000000 pyifdm-1.0.1/pyifdm/methods/topsis/__init__.py
+-rw-rw-rw-   0        0        0     3200 2023-01-02 14:08:32.000000 pyifdm-1.0.1/pyifdm/methods/topsis/ifs.py
+-rw-rw-rw-   0        0        0     4168 2023-01-16 10:05:50.000000 pyifdm-1.0.1/pyifdm/methods/validator.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:44.453901 pyifdm-1.0.1/pyifdm/methods/vikor/
+-rw-rw-rw-   0        0        0       17 2022-12-21 10:39:26.000000 pyifdm-1.0.1/pyifdm/methods/vikor/__init__.py
+-rw-rw-rw-   0        0        0     3212 2023-01-06 11:15:02.000000 pyifdm-1.0.1/pyifdm/methods/vikor/ifs.py
+-rw-rw-rw-   0        0        0     5699 2023-01-10 10:56:55.000000 pyifdm-1.0.1/pyifdm/weights.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:44.362483 pyifdm-1.0.1/pyifdm.egg-info/
+-rw-rw-rw-   0        0        0    10978 2023-04-16 13:07:44.000000 pyifdm-1.0.1/pyifdm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1229 2023-04-16 13:07:44.000000 pyifdm-1.0.1/pyifdm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 13:07:44.000000 pyifdm-1.0.1/pyifdm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-16 13:07:44.000000 pyifdm-1.0.1/pyifdm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-16 13:07:44.000000 pyifdm-1.0.1/pyifdm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 13:07:44.457901 pyifdm-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      798 2023-04-16 12:57:05.000000 pyifdm-1.0.1/setup.py
```

### Comparing `pyifdm-1.0.0/LICENSE` & `pyifdm-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyifdm-1.0.0/PKG-INFO` & `pyifdm-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyifdm
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python library to support Decision Making with Intuitionistic Fuzzy Sets
 Home-page: https://github.com/jwieckowski/pyifdm
 Author: Jakub Więckowski
 Author-email: J.Wieckowski@il-pib.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyifdm-1.0.0/README.md` & `pyifdm-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyifdm-1.0.0/pyifdm/correlations.py` & `pyifdm-1.0.1/pyifdm/correlations.py`

 * *Files identical despite different names*

### Comparing `pyifdm-1.0.0/pyifdm/helpers.py` & `pyifdm-1.0.1/pyifdm/helpers.py`

 * *Files identical despite different names*

### Comparing `pyifdm-1.0.0/pyifdm/methods/aras/ifs.py` & `pyifdm-1.0.1/pyifdm/methods/aras/ifs.py`

 * *Files identical despite different names*

### Comparing `pyifdm-1.0.0/pyifdm/methods/codas/ifs.py` & `pyifdm-1.0.1/pyifdm/methods/codas/ifs.py`

 * *Files identical despite different names*

### Comparing `pyifdm-1.0.0/pyifdm/methods/copras/ifs.py` & `pyifdm-1.0.1/pyifdm/methods/copras/ifs.py`

 * *Files identical despite different names*

### Comparing `pyifdm-1.0.0/pyifdm/methods/edas/ifs.py` & `pyifdm-1.0.1/pyifdm/methods/edas/ifs.py`

 * *Files identical despite different names*

### Comparing `pyifdm-1.0.0/pyifdm/methods/if_codas.py` & `pyifdm-1.0.1/pyifdm/methods/if_codas.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) 2022 Jakub Więckowski
 
 from .codas.ifs import ifs
 from .ifs.normalization import swap_normalization
 from .ifs.distance import euclidean_distance, hamming_distance
+from ..helpers import rank
 
 from .validator import Validator
 
 
 class ifCODAS():
     def __init__(self, normalization=swap_normalization, distance_1=euclidean_distance, distance_2=hamming_distance, tau=0.05):
         """
@@ -28,14 +29,15 @@
 
         """
 
         self.normalization = normalization
         self.distance_1 = distance_1
         self.distance_2 = distance_2
         self.tau = tau
+        self.__descending = True
 
     def __call__(self, matrix, weights, types):
         """
         Calculates the alternatives preferences
 
         Parameters
         ----------
@@ -54,8 +56,25 @@
         ----------
             ndarray:
                 Preference calculated for alternatives. Greater values are placed higher in ranking
         """
         # validate data
         Validator.ifs_validation(matrix, weights, types, mixed_types=True)
 
-        return ifs(matrix, weights, types, self.normalization, self.distance_1, self.distance_2, self.tau).astype(float)
+        self.preferences = ifs(matrix, weights, types, self.normalization, self.distance_1, self.distance_2, self.tau).astype(float)
+        return self.preferences
+
+    def rank(self):
+        """
+            Calculates the alternatives ranking based on the obtained preferences
+
+            Returns
+            ----------
+                ndarray:
+                    Ranking of alternatives
+        """
+        try:
+            return rank(self.preferences, self.__descending)
+        except AttributeError:
+            raise AttributeError('Cannot calculate ranking before assessment')
+        except:
+            raise ValueError('Error occurred in ranking calculation')
```

### Comparing `pyifdm-1.0.0/pyifdm/methods/if_copras.py` & `pyifdm-1.0.1/pyifdm/methods/if_topsis.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # Copyright (c) 2022 Jakub Więckowski
 
-from .copras.ifs import ifs
-from .ifs.score import thakur_score
+from .topsis.ifs import ifs
+from .ifs.distance import normalized_euclidean_distance
+from ..helpers import rank
 
 from .validator import Validator
 
 
-class ifCOPRAS():
-    def __init__(self, score=thakur_score, normalization=None):
+class ifTOPSIS():
+    def __init__(self, distance=normalized_euclidean_distance, normalization=None):
         """
-        Create Intuitionistic Fuzzy COPRAS method object with normalization and score functions
+        Creates Intuitionistic Fuzzy TOPSIS method object with normalization and distance functions
 
         Parameters
         ----------
-            score: callable, default=thakur_score
-                Function used to calculate crisp score of IFS
+            distance: callable, default=normalized_euclidean_distance
+                Function used to calculate distance between two IFS
             
             normalization: callable, default=None
-                Function used to calculate normalized decision matrix
+                Function used to normalize the decision matrix
 
         """
 
-        self.score = score
         self.normalization = normalization
+        self.distance = distance
+        self.__descending = True
 
     def __call__(self, matrix, weights, types):
         """
         Calculates the alternatives preferences
 
         Parameters
         ----------
@@ -34,18 +36,36 @@
                 Decision matrix / alternatives data.
                 Alternatives are in rows and Criteria are in columns.
 
             weights : ndarray
                 Vector of criteria weights in a crisp or Intuitionistic Fuzzy form
 
             types : ndarray
-                Types of criteria, 1 profit, -1 cost
+                Types of criteria, 1 profit, -1 cost.
+                Criteria types cannot be all profit or all cost.
 
         Returns
         ----------
             ndarray:
                 Preference calculated for alternatives. Greater values are placed higher in ranking
         """
         # validate data
-        Validator.ifs_validation(matrix, weights, types)
+        Validator.ifs_validation(matrix, weights, types, mixed_types=True)
 
-        return ifs(matrix, weights, types, self.normalization, self.score).astype(float)
+        self.preferences = ifs(matrix, weights, types, self.normalization, self.distance).astype(float)
+        return self.preferences
+
+    def rank(self):
+        """
+            Calculates the alternatives ranking based on the obtained preferences
+
+            Returns
+            ----------
+                ndarray:
+                    Ranking of alternatives
+        """
+        try:
+            return rank(self.preferences, self.__descending)
+        except AttributeError:
+            raise AttributeError('Cannot calculate ranking before assessment')
+        except:
+            raise ValueError('Error occurred in ranking calculation')
```

### Comparing `pyifdm-1.0.0/pyifdm/methods/if_edas.py` & `pyifdm-1.0.1/pyifdm/methods/if_edas.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) 2022 Jakub Więckowski
 
 from .edas.ifs import ifs
 from .ifs.normalization import swap_normalization
 from .ifs.score import liu_wang_score
+from ..helpers import rank
 
 from .validator import Validator
 
 
 class ifEDAS():
     def __init__(self, normalization=swap_normalization, score=liu_wang_score):
         """
@@ -20,14 +21,15 @@
             score: callable, default=liu_wang_score
                 Function used to calculate crisp score of IFS
 
         """
 
         self.normalization = normalization
         self.score = score
+        self.__descending = True
 
     def __call__(self, matrix, weights, types):
         """
         Calculates the alternatives preferences
 
         Parameters
         ----------
@@ -45,8 +47,25 @@
         ----------
             ndarray:
                 Preference calculated for alternatives. Greater values are placed higher in ranking
         """
         # validate data
         Validator.ifs_validation(matrix, weights, types)
 
-        return ifs(matrix, weights, types, self.normalization, self.score).astype(float)
+        self.preferences = ifs(matrix, weights, types, self.normalization, self.score).astype(float)
+        return self.preferences
+        
+    def rank(self):
+        """
+            Calculates the alternatives ranking based on the obtained preferences
+
+            Returns
+            ----------
+                ndarray:
+                    Ranking of alternatives
+        """
+        try:
+            return rank(self.preferences, self.__descending)
+        except AttributeError:
+            raise AttributeError('Cannot calculate ranking before assessment')
+        except:
+            raise ValueError('Error occurred in ranking calculation')
```

### Comparing `pyifdm-1.0.0/pyifdm/methods/if_mabac.py` & `pyifdm-1.0.1/pyifdm/methods/if_mabac.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (c) 2022 Jakub Więckowski
 
 from .mabac.ifs import ifs
 from .ifs.normalization import swap_normalization
 from .ifs.score import liu_wang_score
 from .ifs.distance import luo_distance
+from ..helpers import rank
 
 from .validator import Validator
 
 
 class ifMABAC():
     def __init__(self, normalization=swap_normalization, distance=luo_distance, score=liu_wang_score, p=2.25, g=0.88):
         """
@@ -32,14 +33,15 @@
         """
 
         self.normalization = normalization
         self.distance = distance
         self.score = score
         self.p = p
         self.g = g
+        self.__descending = True
 
     def __call__(self, matrix, weights, types):
         """
         Calculates the alternatives preferences
 
         Parameters
         ----------
@@ -57,8 +59,25 @@
         ----------
             ndarray:
                 Preference calculated for alternatives. Greater values are placed higher in ranking
         """
         # validate data
         Validator.ifs_validation(matrix, weights, types)
 
-        return ifs(matrix, weights, types, self.normalization, self.distance, self.score, self.p, self.g).astype(float)
+        self.preferences = ifs(matrix, weights, types, self.normalization, self.distance, self.score, self.p, self.g).astype(float)
+        return self.preferences
+
+    def rank(self):
+        """
+            Calculates the alternatives ranking based on the obtained preferences
+
+            Returns
+            ----------
+                ndarray:
+                    Ranking of alternatives
+        """
+        try:
+            return rank(self.preferences, self.__descending)
+        except AttributeError:
+            raise AttributeError('Cannot calculate ranking before assessment')
+        except:
+            raise ValueError('Error occurred in ranking calculation')
```

### Comparing `pyifdm-1.0.0/pyifdm/methods/if_mairca.py` & `pyifdm-1.0.1/pyifdm/methods/if_moora.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 # Copyright (c) 2022 Jakub Więckowski
 
-from .mairca.ifs import ifs
-from .ifs.normalization import minmax_normalization
-from .ifs.distance import normalized_euclidean_distance
-from .ifs.score import liu_wang_score
+from .moora.ifs import ifs
+from .ifs.score import zhang_xu_score_2
+from ..helpers import rank
 
 from .validator import Validator
 
-
-class ifMAIRCA():
-    def __init__(self, normalization=minmax_normalization, distance=normalized_euclidean_distance, score=liu_wang_score):
+class ifMOORA():
+    def __init__(self, score=zhang_xu_score_2, normalization=None):
         """
-        Create Intuitionistic Fuzzy MAIRCA method object with normalization and distance functions
+        Create Intuitionistic Fuzzy MOORA method object with normalization and score functions
 
         Parameters
         ----------
-            normalization: callable, default=minmax_normalization
-                Function used to normalize the decision matrix
-
-            distance: callable, default=normalized_euclidean_distance
-                Function used to calculate distance between two IFS
-
-            score: callable, default=liu_wang_score
+            score: callable, default=zhang_xu_score_2
                 Function used to calculate crisp score of IFS
+            
+            normalization: callable, default=None
+                Function used to normalize the decision matrix
 
         """
 
         self.normalization = normalization
-        self.distance = distance
         self.score = score
+        self.__descending = True
 
     def __call__(self, matrix, weights, types):
         """
         Calculates the alternatives preferences
 
         Parameters
         ----------
@@ -40,18 +35,36 @@
                 Decision matrix / alternatives data.
                 Alternatives are in rows and Criteria are in columns.
 
             weights : ndarray
                 Vector of criteria weights in a crisp or Intuitionistic Fuzzy form
 
             types : ndarray
-                Types of criteria, 1 profit, -1 cost
+                Types of criteria, 1 profit, -1 cost.
+                Criteria types cannot be all profit or all cost.
 
         Returns
         ----------
             ndarray:
                 Preference calculated for alternatives. Greater values are placed higher in ranking
         """
         # validate data
-        Validator.ifs_validation(matrix, weights, types)
+        Validator.ifs_validation(matrix, weights, types, mixed_types=True)
 
-        return ifs(matrix, weights, types, self.normalization, self.distance, self.score).astype(float)
+        self.preferences = ifs(matrix, weights, types, self.normalization, self.score).astype(float)
+        return self.preferences
+
+    def rank(self):
+        """
+            Calculates the alternatives ranking based on the obtained preferences
+
+            Returns
+            ----------
+                ndarray:
+                    Ranking of alternatives
+        """
+        try:
+            return rank(self.preferences, self.__descending)
+        except AttributeError:
+            raise AttributeError('Cannot calculate ranking before assessment')
+        except:
+            raise ValueError('Error occurred in ranking calculation')
```

### Comparing `pyifdm-1.0.0/pyifdm/methods/if_vikor.py` & `pyifdm-1.0.1/pyifdm/methods/if_copras.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 # Copyright (c) 2022 Jakub Więckowski
 
-from .vikor.ifs import ifs
-from .ifs.distance import hamming_distance
+from .copras.ifs import ifs
+from .ifs.score import thakur_score
+from ..helpers import rank
 
 from .validator import Validator
 
 
-class ifVIKOR():
-    def __init__(self, distance=hamming_distance, normalization=None, v=0.5):
+class ifCOPRAS():
+    def __init__(self, score=thakur_score, normalization=None):
         """
-        Creates Intuitionistic Fuzzy VIKOR method object with normalization and distance functions
+        Create Intuitionistic Fuzzy COPRAS method object with normalization and score functions
 
         Parameters
         ----------
-            distance: callable, default=hamming_distance
-                Function used to calculate distance between two IFS
+            score: callable, default=thakur_score
+                Function used to calculate crisp score of IFS
             
             normalization: callable, default=None
-                Function used to normalize the decision matrix
+                Function used to calculate normalized decision matrix
 
-            v : float, default=0.5
-                Weight of the strategy (see VIKOR algorithm explanation).
         """
 
+        self.score = score
         self.normalization = normalization
-        self.distance = distance
-        self.v = v
+        self.__descending = True
 
     def __call__(self, matrix, weights, types):
         """
         Calculates the alternatives preferences
 
         Parameters
         ----------
@@ -42,14 +41,30 @@
 
             types : ndarray
                 Types of criteria, 1 profit, -1 cost
 
         Returns
         ----------
             ndarray:
-                Preference calculated for alternatives. Lower values are placed higher in ranking
+                Preference calculated for alternatives. Greater values are placed higher in ranking
         """
         # validate data
         Validator.ifs_validation(matrix, weights, types)
 
-        return ifs(matrix, weights, types, self.normalization, self.distance, self.v)
+        self.preferences = ifs(matrix, weights, types, self.normalization, self.score).astype(float)
+        return self.preferences
 
+    def rank(self):
+        """
+            Calculates the alternatives ranking based on the obtained preferences
+
+            Returns
+            ----------
+                ndarray:
+                    Ranking of alternatives
+        """
+        try:
+            return rank(self.preferences, self.__descending)
+        except AttributeError:
+            raise AttributeError('Cannot calculate ranking before assessment')
+        except:
+            raise ValueError('Error occurred in ranking calculation')
```

### Comparing `pyifdm-1.0.0/pyifdm/methods/ifs/distance.py` & `pyifdm-1.0.1/pyifdm/methods/ifs/distance.py`

 * *Files identical despite different names*

### Comparing `pyifdm-1.0.0/pyifdm/methods/ifs/normalization.py` & `pyifdm-1.0.1/pyifdm/methods/ifs/normalization.py`

 * *Files identical despite different names*

### Comparing `pyifdm-1.0.0/pyifdm/methods/ifs/score.py` & `pyifdm-1.0.1/pyifdm/methods/ifs/score.py`

 * *Files identical despite different names*

### Comparing `pyifdm-1.0.0/pyifdm/methods/mabac/ifs.py` & `pyifdm-1.0.1/pyifdm/methods/mabac/ifs.py`

 * *Files identical despite different names*

### Comparing `pyifdm-1.0.0/pyifdm/methods/mairca/ifs.py` & `pyifdm-1.0.1/pyifdm/methods/mairca/ifs.py`

 * *Files identical despite different names*

### Comparing `pyifdm-1.0.0/pyifdm/methods/moora/ifs.py` & `pyifdm-1.0.1/pyifdm/methods/moora/ifs.py`

 * *Files identical despite different names*

### Comparing `pyifdm-1.0.0/pyifdm/methods/topsis/ifs.py` & `pyifdm-1.0.1/pyifdm/methods/topsis/ifs.py`

 * *Files identical despite different names*

### Comparing `pyifdm-1.0.0/pyifdm/methods/validator.py` & `pyifdm-1.0.1/pyifdm/methods/validator.py`

 * *Files identical despite different names*

### Comparing `pyifdm-1.0.0/pyifdm/methods/vikor/ifs.py` & `pyifdm-1.0.1/pyifdm/methods/vikor/ifs.py`

 * *Files identical despite different names*

### Comparing `pyifdm-1.0.0/pyifdm/weights.py` & `pyifdm-1.0.1/pyifdm/weights.py`

 * *Files identical despite different names*

### Comparing `pyifdm-1.0.0/pyifdm.egg-info/PKG-INFO` & `pyifdm-1.0.1/pyifdm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyifdm
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python library to support Decision Making with Intuitionistic Fuzzy Sets
 Home-page: https://github.com/jwieckowski/pyifdm
 Author: Jakub Więckowski
 Author-email: J.Wieckowski@il-pib.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyifdm-1.0.0/pyifdm.egg-info/SOURCES.txt` & `pyifdm-1.0.1/pyifdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyifdm-1.0.0/setup.py` & `pyifdm-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyifdm",
-    version="1.0.0",
+    version="1.0.1",
     author="Jakub Więckowski",
     author_email="J.Wieckowski@il-pib.pl",
     description="Python library to support Decision Making with Intuitionistic Fuzzy Sets",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jwieckowski/pyifdm",
     packages=setuptools.find_packages(),
```

