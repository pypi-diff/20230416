# Comparing `tmp/palettable-3.3.1.tar.gz` & `tmp/palettable-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palettable-3.3.1.tar", last modified: Thu Apr  6 04:03:33 2023, max compression
+gzip compressed data, was "palettable-3.3.2.tar", last modified: Sun Apr 16 20:31:10 2023, max compression
```

## Comparing `palettable-3.3.1.tar` & `palettable-3.3.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-06 04:03:33.036478 palettable-3.3.1/
--rw-r--r--   0 jiffyclub   (501) staff       (20)       59 2018-05-14 14:49:57.000000 palettable-3.3.1/MANIFEST.in
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1680 2023-04-06 04:03:33.036626 palettable-3.3.1/PKG-INFO
--rw-r--r--   0 jiffyclub   (501) staff       (20)      985 2015-07-11 16:45:18.000000 palettable-3.3.1/README.rst
--rw-r--r--   0 jiffyclub   (501) staff       (20)    10476 2014-09-11 18:21:02.000000 palettable-3.3.1/ez_setup.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1065 2019-07-11 23:03:53.000000 palettable-3.3.1/license.txt
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-06 04:03:33.000692 palettable-3.3.1/palettable/
--rw-r--r--   0 jiffyclub   (501) staff       (20)      481 2023-04-06 03:51:32.000000 palettable-3.3.1/palettable/__init__.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-06 04:03:33.011593 palettable-3.3.1/palettable/cartocolors/
--rw-r--r--   0 jiffyclub   (501) staff       (20)       89 2017-09-02 05:18:58.000000 palettable-3.3.1/palettable/cartocolors/__init__.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)      932 2017-09-02 05:18:58.000000 palettable-3.3.1/palettable/cartocolors/cartocolorspalette.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     6104 2017-09-02 05:18:58.000000 palettable-3.3.1/palettable/cartocolors/colormaps.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1049 2017-09-02 05:18:58.000000 palettable-3.3.1/palettable/cartocolors/diverging.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1276 2017-09-02 05:18:58.000000 palettable-3.3.1/palettable/cartocolors/qualitative.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1410 2019-09-07 23:30:52.000000 palettable-3.3.1/palettable/cartocolors/sequential.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-06 04:03:33.014086 palettable-3.3.1/palettable/cmocean/
--rw-r--r--   0 jiffyclub   (501) staff       (20)       76 2017-02-20 23:03:00.000000 palettable-3.3.1/palettable/cmocean/__init__.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)      884 2017-02-20 23:03:00.000000 palettable-3.3.1/palettable/cmocean/cmoceanpalette.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)   101253 2017-02-20 23:03:00.000000 palettable-3.3.1/palettable/cmocean/colormaps.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)      817 2017-02-20 23:03:00.000000 palettable-3.3.1/palettable/cmocean/diverging.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1130 2017-02-20 23:03:00.000000 palettable-3.3.1/palettable/cmocean/sequential.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-06 04:03:33.018326 palettable-3.3.1/palettable/colorbrewer/
--rw-r--r--   0 jiffyclub   (501) staff       (20)      116 2015-03-04 06:18:35.000000 palettable-3.3.1/palettable/colorbrewer/__init__.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     6309 2023-04-06 03:47:14.000000 palettable-3.3.1/palettable/colorbrewer/colorbrewer.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)    99495 2023-04-06 03:47:14.000000 palettable-3.3.1/palettable/colorbrewer/colorbrewer_all_schemes.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-06 04:03:33.019781 palettable-3.3.1/palettable/colorbrewer/data/
--rw-r--r--   0 jiffyclub   (501) staff       (20)    37224 2015-03-04 06:18:35.000000 palettable-3.3.1/palettable/colorbrewer/data/colorbrewer_all_schemes.csv
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1712 2015-03-04 06:18:35.000000 palettable-3.3.1/palettable/colorbrewer/data/colorbrewer_licence.txt
--rw-r--r--   0 jiffyclub   (501) staff       (20)      135 2017-02-20 23:03:00.000000 palettable-3.3.1/palettable/colorbrewer/diverging.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)      137 2017-02-20 23:03:00.000000 palettable-3.3.1/palettable/colorbrewer/qualitative.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)      136 2017-02-20 23:03:00.000000 palettable-3.3.1/palettable/colorbrewer/sequential.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-06 04:03:33.021497 palettable-3.3.1/palettable/cubehelix/
--rw-r--r--   0 jiffyclub   (501) staff       (20)      153 2015-05-01 04:35:16.000000 palettable-3.3.1/palettable/cubehelix/__init__.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)    13383 2015-05-01 04:35:16.000000 palettable-3.3.1/palettable/cubehelix/cubehelix.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-06 04:03:33.024607 palettable-3.3.1/palettable/lightbartlein/
--rw-r--r--   0 jiffyclub   (501) staff       (20)       76 2019-07-11 22:44:07.000000 palettable-3.3.1/palettable/lightbartlein/__init__.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     4398 2019-07-11 22:44:07.000000 palettable-3.3.1/palettable/lightbartlein/colordata.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     2181 2019-07-11 22:44:07.000000 palettable-3.3.1/palettable/lightbartlein/diverging.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)      998 2019-07-11 22:44:07.000000 palettable-3.3.1/palettable/lightbartlein/lightbartlein.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1194 2019-07-11 22:44:07.000000 palettable-3.3.1/palettable/lightbartlein/sequential.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-06 04:03:33.026312 palettable-3.3.1/palettable/matplotlib/
--rw-r--r--   0 jiffyclub   (501) staff       (20)      207 2017-02-20 23:03:00.000000 palettable-3.3.1/palettable/matplotlib/__init__.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)    33280 2017-02-20 23:03:00.000000 palettable-3.3.1/palettable/matplotlib/colormaps.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1548 2017-02-20 23:03:00.000000 palettable-3.3.1/palettable/matplotlib/matplotlib.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-06 04:03:33.027651 palettable-3.3.1/palettable/mycarta/
--rw-r--r--   0 jiffyclub   (501) staff       (20)      204 2017-02-20 23:03:00.000000 palettable-3.3.1/palettable/mycarta/__init__.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)    15123 2017-02-20 23:03:00.000000 palettable-3.3.1/palettable/mycarta/colordata.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1491 2017-02-20 23:03:00.000000 palettable-3.3.1/palettable/mycarta/mycarta.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     7200 2017-09-02 05:18:58.000000 palettable-3.3.1/palettable/palette.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-06 04:03:33.030151 palettable-3.3.1/palettable/scientific/
--rw-r--r--   0 jiffyclub   (501) staff       (20)       76 2019-09-07 23:30:52.000000 palettable-3.3.1/palettable/scientific/__init__.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)   122443 2019-09-07 23:30:52.000000 palettable-3.3.1/palettable/scientific/colordata.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)      799 2019-09-07 23:30:52.000000 palettable-3.3.1/palettable/scientific/diverging.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)      888 2019-09-07 23:30:52.000000 palettable-3.3.1/palettable/scientific/scientific.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)      907 2019-09-07 23:30:52.000000 palettable-3.3.1/palettable/scientific/sequential.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-06 04:03:33.031205 palettable-3.3.1/palettable/tableau/
--rw-r--r--   0 jiffyclub   (501) staff       (20)      140 2015-03-04 06:18:35.000000 palettable-3.3.1/palettable/tableau/__init__.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     5921 2015-03-04 06:18:35.000000 palettable-3.3.1/palettable/tableau/tableau.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     7124 2017-09-02 05:18:58.000000 palettable-3.3.1/palettable/utils.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-06 04:03:33.035738 palettable-3.3.1/palettable/wesanderson/
--rw-r--r--   0 jiffyclub   (501) staff       (20)      156 2017-02-20 23:03:00.000000 palettable-3.3.1/palettable/wesanderson/__init__.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)    12587 2019-09-07 18:37:56.000000 palettable-3.3.1/palettable/wesanderson/wesanderson.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-06 04:03:33.008896 palettable-3.3.1/palettable.egg-info/
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1680 2023-04-06 04:03:32.000000 palettable-3.3.1/palettable.egg-info/PKG-INFO
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1792 2023-04-06 04:03:32.000000 palettable-3.3.1/palettable.egg-info/SOURCES.txt
--rw-r--r--   0 jiffyclub   (501) staff       (20)        1 2023-04-06 04:03:32.000000 palettable-3.3.1/palettable.egg-info/dependency_links.txt
--rw-r--r--   0 jiffyclub   (501) staff       (20)       11 2023-04-06 04:03:32.000000 palettable-3.3.1/palettable.egg-info/top_level.txt
--rw-r--r--   0 jiffyclub   (501) staff       (20)       67 2023-04-06 04:03:33.037215 palettable-3.3.1/setup.cfg
--rw-r--r--   0 jiffyclub   (501) staff       (20)      987 2023-04-06 03:51:10.000000 palettable-3.3.1/setup.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-06 04:03:33.036162 palettable-3.3.1/test/
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1154 2017-09-02 05:18:58.000000 palettable-3.3.1/test/test_installed.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.729449 palettable-3.3.2/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)       59 2018-05-14 14:49:57.000000 palettable-3.3.2/MANIFEST.in
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1941 2023-04-16 20:31:10.729606 palettable-3.3.2/PKG-INFO
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      985 2015-07-11 16:45:18.000000 palettable-3.3.2/README.rst
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    10476 2014-09-11 18:21:02.000000 palettable-3.3.2/ez_setup.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1065 2019-07-11 23:03:53.000000 palettable-3.3.2/license.txt
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.687970 palettable-3.3.2/palettable/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      481 2023-04-16 20:30:46.000000 palettable-3.3.2/palettable/__init__.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.694967 palettable-3.3.2/palettable/cartocolors/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)       89 2017-09-02 05:18:58.000000 palettable-3.3.2/palettable/cartocolors/__init__.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      932 2017-09-02 05:18:58.000000 palettable-3.3.2/palettable/cartocolors/cartocolorspalette.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     6104 2017-09-02 05:18:58.000000 palettable-3.3.2/palettable/cartocolors/colormaps.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1049 2017-09-02 05:18:58.000000 palettable-3.3.2/palettable/cartocolors/diverging.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1276 2017-09-02 05:18:58.000000 palettable-3.3.2/palettable/cartocolors/qualitative.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1410 2019-09-07 23:30:52.000000 palettable-3.3.2/palettable/cartocolors/sequential.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.701268 palettable-3.3.2/palettable/cmocean/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)       76 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/cmocean/__init__.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      884 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/cmocean/cmoceanpalette.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)   101253 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/cmocean/colormaps.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      817 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/cmocean/diverging.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1130 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/cmocean/sequential.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.706827 palettable-3.3.2/palettable/colorbrewer/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      116 2015-03-04 06:18:35.000000 palettable-3.3.2/palettable/colorbrewer/__init__.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     6309 2023-04-06 03:47:14.000000 palettable-3.3.2/palettable/colorbrewer/colorbrewer.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    99495 2023-04-06 03:47:14.000000 palettable-3.3.2/palettable/colorbrewer/colorbrewer_all_schemes.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.709638 palettable-3.3.2/palettable/colorbrewer/data/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    37224 2015-03-04 06:18:35.000000 palettable-3.3.2/palettable/colorbrewer/data/colorbrewer_all_schemes.csv
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1712 2015-03-04 06:18:35.000000 palettable-3.3.2/palettable/colorbrewer/data/colorbrewer_licence.txt
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      135 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/colorbrewer/diverging.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      137 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/colorbrewer/qualitative.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      136 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/colorbrewer/sequential.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.711512 palettable-3.3.2/palettable/cubehelix/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      153 2015-05-01 04:35:16.000000 palettable-3.3.2/palettable/cubehelix/__init__.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    13383 2015-05-01 04:35:16.000000 palettable-3.3.2/palettable/cubehelix/cubehelix.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.715813 palettable-3.3.2/palettable/lightbartlein/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)       76 2019-07-11 22:44:07.000000 palettable-3.3.2/palettable/lightbartlein/__init__.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     4398 2019-07-11 22:44:07.000000 palettable-3.3.2/palettable/lightbartlein/colordata.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     2181 2019-07-11 22:44:07.000000 palettable-3.3.2/palettable/lightbartlein/diverging.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      998 2019-07-11 22:44:07.000000 palettable-3.3.2/palettable/lightbartlein/lightbartlein.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1194 2019-07-11 22:44:07.000000 palettable-3.3.2/palettable/lightbartlein/sequential.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.718069 palettable-3.3.2/palettable/matplotlib/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      207 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/matplotlib/__init__.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    33280 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/matplotlib/colormaps.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1548 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/matplotlib/matplotlib.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.720223 palettable-3.3.2/palettable/mycarta/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      204 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/mycarta/__init__.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    15123 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/mycarta/colordata.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1491 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/mycarta/mycarta.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     7200 2017-09-02 05:18:58.000000 palettable-3.3.2/palettable/palette.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.724099 palettable-3.3.2/palettable/scientific/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)       76 2019-09-07 23:30:52.000000 palettable-3.3.2/palettable/scientific/__init__.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)   122443 2019-09-07 23:30:52.000000 palettable-3.3.2/palettable/scientific/colordata.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      799 2019-09-07 23:30:52.000000 palettable-3.3.2/palettable/scientific/diverging.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      888 2019-09-07 23:30:52.000000 palettable-3.3.2/palettable/scientific/scientific.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      907 2019-09-07 23:30:52.000000 palettable-3.3.2/palettable/scientific/sequential.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.725412 palettable-3.3.2/palettable/tableau/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      140 2015-03-04 06:18:35.000000 palettable-3.3.2/palettable/tableau/__init__.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     5921 2015-03-04 06:18:35.000000 palettable-3.3.2/palettable/tableau/tableau.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     7124 2017-09-02 05:18:58.000000 palettable-3.3.2/palettable/utils.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.726869 palettable-3.3.2/palettable/wesanderson/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      156 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/wesanderson/__init__.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    12587 2019-09-07 18:37:56.000000 palettable-3.3.2/palettable/wesanderson/wesanderson.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.689971 palettable-3.3.2/palettable.egg-info/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1941 2023-04-16 20:31:10.000000 palettable-3.3.2/palettable.egg-info/PKG-INFO
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1792 2023-04-16 20:31:10.000000 palettable-3.3.2/palettable.egg-info/SOURCES.txt
+-rw-r--r--   0 jiffyclub   (501) staff       (20)        1 2023-04-16 20:31:10.000000 palettable-3.3.2/palettable.egg-info/dependency_links.txt
+-rw-r--r--   0 jiffyclub   (501) staff       (20)       11 2023-04-16 20:31:10.000000 palettable-3.3.2/palettable.egg-info/top_level.txt
+-rw-r--r--   0 jiffyclub   (501) staff       (20)       67 2023-04-16 20:31:10.730142 palettable-3.3.2/setup.cfg
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1256 2023-04-16 20:30:40.000000 palettable-3.3.2/setup.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.728820 palettable-3.3.2/test/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1154 2017-09-02 05:18:58.000000 palettable-3.3.2/test/test_installed.py
```

### Comparing `palettable-3.3.1/PKG-INFO` & `palettable-3.3.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: palettable
-Version: 3.3.1
+Version: 3.3.2
 Summary: Color palettes for Python
 Home-page: https://jiffyclub.github.io/palettable/
 Author: Matt Davis
 Author-email: jiffyclub@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Visualization
+Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 
 Palettable
 ==========
 
 .. image:: https://travis-ci.org/jiffyclub/palettable.png?branch=master
    :alt: Travis-CI
    :target: https://travis-ci.org/jiffyclub/palettable
```

### Comparing `palettable-3.3.1/README.rst` & `palettable-3.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/ez_setup.py` & `palettable-3.3.2/ez_setup.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/license.txt` & `palettable-3.3.2/license.txt`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/cartocolors/cartocolorspalette.py` & `palettable-3.3.2/palettable/cartocolors/cartocolorspalette.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/cartocolors/colormaps.py` & `palettable-3.3.2/palettable/cartocolors/colormaps.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/cartocolors/diverging.py` & `palettable-3.3.2/palettable/cartocolors/diverging.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/cartocolors/qualitative.py` & `palettable-3.3.2/palettable/cartocolors/qualitative.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/cartocolors/sequential.py` & `palettable-3.3.2/palettable/cartocolors/sequential.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/cmocean/cmoceanpalette.py` & `palettable-3.3.2/palettable/cmocean/cmoceanpalette.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/cmocean/colormaps.py` & `palettable-3.3.2/palettable/cmocean/colormaps.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/cmocean/diverging.py` & `palettable-3.3.2/palettable/cmocean/diverging.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/cmocean/sequential.py` & `palettable-3.3.2/palettable/cmocean/sequential.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/colorbrewer/colorbrewer.py` & `palettable-3.3.2/palettable/colorbrewer/colorbrewer.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/colorbrewer/colorbrewer_all_schemes.py` & `palettable-3.3.2/palettable/colorbrewer/colorbrewer_all_schemes.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/colorbrewer/data/colorbrewer_all_schemes.csv` & `palettable-3.3.2/palettable/colorbrewer/data/colorbrewer_all_schemes.csv`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/colorbrewer/data/colorbrewer_licence.txt` & `palettable-3.3.2/palettable/colorbrewer/data/colorbrewer_licence.txt`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/cubehelix/cubehelix.py` & `palettable-3.3.2/palettable/cubehelix/cubehelix.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/lightbartlein/colordata.py` & `palettable-3.3.2/palettable/lightbartlein/colordata.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/lightbartlein/diverging.py` & `palettable-3.3.2/palettable/lightbartlein/diverging.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/lightbartlein/lightbartlein.py` & `palettable-3.3.2/palettable/lightbartlein/lightbartlein.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/lightbartlein/sequential.py` & `palettable-3.3.2/palettable/lightbartlein/sequential.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/matplotlib/colormaps.py` & `palettable-3.3.2/palettable/matplotlib/colormaps.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/matplotlib/matplotlib.py` & `palettable-3.3.2/palettable/matplotlib/matplotlib.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/mycarta/colordata.py` & `palettable-3.3.2/palettable/mycarta/colordata.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/mycarta/mycarta.py` & `palettable-3.3.2/palettable/mycarta/mycarta.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/palette.py` & `palettable-3.3.2/palettable/palette.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/scientific/colordata.py` & `palettable-3.3.2/palettable/scientific/colordata.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/scientific/diverging.py` & `palettable-3.3.2/palettable/scientific/diverging.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/scientific/scientific.py` & `palettable-3.3.2/palettable/scientific/scientific.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/scientific/sequential.py` & `palettable-3.3.2/palettable/scientific/sequential.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/tableau/tableau.py` & `palettable-3.3.2/palettable/tableau/tableau.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/utils.py` & `palettable-3.3.2/palettable/utils.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable/wesanderson/wesanderson.py` & `palettable-3.3.2/palettable/wesanderson/wesanderson.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/palettable.egg-info/PKG-INFO` & `palettable-3.3.2/palettable.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: palettable
-Version: 3.3.1
+Version: 3.3.2
 Summary: Color palettes for Python
 Home-page: https://jiffyclub.github.io/palettable/
 Author: Matt Davis
 Author-email: jiffyclub@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Visualization
+Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 
 Palettable
 ==========
 
 .. image:: https://travis-ci.org/jiffyclub/palettable.png?branch=master
    :alt: Travis-CI
    :target: https://travis-ci.org/jiffyclub/palettable
```

### Comparing `palettable-3.3.1/palettable.egg-info/SOURCES.txt` & `palettable-3.3.2/palettable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `palettable-3.3.1/test/test_installed.py` & `palettable-3.3.2/test/test_installed.py`

 * *Files identical despite different names*

