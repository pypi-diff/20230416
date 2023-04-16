# Comparing `tmp/gnssrefl-1.3.4.tar.gz` & `tmp/gnssrefl-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnssrefl-1.3.4.tar", last modified: Thu Apr 13 15:12:09 2023, max compression
+gzip compressed data, was "gnssrefl-1.3.5.tar", last modified: Sun Apr 16 09:36:43 2023, max compression
```

## Comparing `gnssrefl-1.3.4.tar` & `gnssrefl-1.3.5.tar`

### file list

```diff
@@ -1,89 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:12:09.532938 gnssrefl-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-13 15:12:09.532938 gnssrefl-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:12:09.508937 gnssrefl-1.3.4/gnssrefl/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/EGM96.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/check_rinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/check_rinex2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/computemp1mp2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19095 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/daily_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/daily_avg_cl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:12:09.508937 gnssrefl-1.3.4/gnssrefl/data/
--rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/data/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/download_ioc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/download_noaa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/download_orbits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/download_psmsl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/download_rinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/download_teqc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/download_tides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/download_unr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/download_wsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/felipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/filesizes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15934 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/gnssir.py
--rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/gnssir_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    50572 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/gnsssnr.f
--rw-r--r--   0 runner    (1001) docker     (123)    50579 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/gnsssnrbigger.f
--rw-r--r--   0 runner    (1001) docker     (123)   174546 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/gps.py
--rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/gpssnr.f
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/gpsweek.py
--rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/highrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/installexe_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/invsnr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/invsnr_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    23471 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/karnak_libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/kelly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/llh2xyz.py
--rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/make_json_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    22560 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/nmea2snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/nmea2snr_cl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34269 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/phase_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/pickle_dilemma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/prn2gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/query_unr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/quickLook_cl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19809 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/quickLook_function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5879 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/quickPhase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19480 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/quickPhase_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/quickplt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/read_snr_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    16511 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/refl_zones.py
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/refl_zones_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/refraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/rh_plot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49164 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/rinex2snr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/rinex2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/rinex3_rinex2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/rinex3_snr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24490 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/rinpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/rt_rinex3_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/snow_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/snowdepth_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    60155 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/spline_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    58660 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/subdaily.py
--rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/subdaily_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/veg_multiyr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/vwc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/vwc_input.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/xyz2llh.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/ydoy.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/ymd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:12:09.508937 gnssrefl-1.3.4/gnssrefl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-13 15:12:09.000000 gnssrefl-1.3.4/gnssrefl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-13 15:12:09.000000 gnssrefl-1.3.4/gnssrefl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:12:09.000000 gnssrefl-1.3.4/gnssrefl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-13 15:12:09.000000 gnssrefl-1.3.4/gnssrefl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 15:12:09.000000 gnssrefl-1.3.4/gnssrefl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 15:12:09.000000 gnssrefl-1.3.4/gnssrefl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 15:12:09.532938 gnssrefl-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:12:09.532938 gnssrefl-1.3.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/test/test_gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/test/test_rinex2snr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:36:43.380895 gnssrefl-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-16 09:36:43.380895 gnssrefl-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:36:43.360895 gnssrefl-1.3.5/gnssrefl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/EGM96.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/check_rinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/check_rinex2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/check_rinex_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/computemp1mp2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19095 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/daily_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/daily_avg_cl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:36:43.360895 gnssrefl-1.3.5/gnssrefl/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/data/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/download_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/download_noaa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/download_orbits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/download_psmsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/download_rinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/download_teqc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/download_tides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/download_unr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/download_wsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/felipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/filesizes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15934 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/gnssir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/gnssir_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50572 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/gnsssnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)    50579 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/gnsssnrbigger.f
+-rw-r--r--   0 runner    (1001) docker     (123)   174542 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/gpssnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/gpsweek.py
+-rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/highrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/installexe_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/invsnr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/invsnr_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23471 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/karnak_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/kelly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/llh2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/make_json_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22560 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/nmea2snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/nmea2snr_cl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34269 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/phase_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/pickle_dilemma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/prn2gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/query_unr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/quickLook_cl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19809 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/quickLook_function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5879 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/quickPhase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19480 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/quickPhase_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/quickplt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/read_snr_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16511 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/refl_zones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/refl_zones_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/refraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/rh_plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49164 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/rinex2snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/rinex2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/rinex3_rinex2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/rinex3_snr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24490 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/rinpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/rt_rinex3_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/snow_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/snowdepth_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60155 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/spline_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58741 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/subdaily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/subdaily_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/veg_multiyr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/vwc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/vwc_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/xyz2llh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/ydoy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/ymd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:36:43.360895 gnssrefl-1.3.5/gnssrefl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-16 09:36:43.000000 gnssrefl-1.3.5/gnssrefl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-16 09:36:43.000000 gnssrefl-1.3.5/gnssrefl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 09:36:43.000000 gnssrefl-1.3.5/gnssrefl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-16 09:36:43.000000 gnssrefl-1.3.5/gnssrefl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-16 09:36:43.000000 gnssrefl-1.3.5/gnssrefl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-16 09:36:43.000000 gnssrefl-1.3.5/gnssrefl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 09:36:43.380895 gnssrefl-1.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:36:43.380895 gnssrefl-1.3.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/test/test_gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/test/test_rinex2snr.py
```

### Comparing `gnssrefl-1.3.4/LICENSE` & `gnssrefl-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/PKG-INFO` & `gnssrefl-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 1.3.4
+Version: 1.3.5
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gnssrefl
 
-**github version: 1.3.3** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.3.5** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
 Our documentation is now available [here.](https://gnssrefl.readthedocs.io/en/latest/)
 
 The [shortcourse registration page is live.](https://www.earthscope.org/event/2023-gnss-ir-short-course) 
 
 If you want to sign up for the GNSS-IR email list, please contact Kristine Larson.
```

### Comparing `gnssrefl-1.3.4/README.md` & `gnssrefl-1.3.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # gnssrefl
 
-**github version: 1.3.3** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.3.5** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
 Our documentation is now available [here.](https://gnssrefl.readthedocs.io/en/latest/)
 
 The [shortcourse registration page is live.](https://www.earthscope.org/event/2023-gnss-ir-short-course) 
 
 If you want to sign up for the GNSS-IR email list, please contact Kristine Larson.
```

### Comparing `gnssrefl-1.3.4/gnssrefl/EGM96.py` & `gnssrefl-1.3.5/gnssrefl/EGM96.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/check_rinex.py` & `gnssrefl-1.3.5/gnssrefl/check_rinex.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/check_rinex2.py` & `gnssrefl-1.3.5/gnssrefl/check_rinex2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/computemp1mp2.py` & `gnssrefl-1.3.5/gnssrefl/computemp1mp2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/daily_avg.py` & `gnssrefl-1.3.5/gnssrefl/daily_avg.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/daily_avg_cl.py` & `gnssrefl-1.3.5/gnssrefl/daily_avg_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/data/gpt_1wA.pickle` & `gnssrefl-1.3.5/gnssrefl/data/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/download_ioc.py` & `gnssrefl-1.3.5/gnssrefl/download_ioc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/download_noaa.py` & `gnssrefl-1.3.5/gnssrefl/download_noaa.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/download_orbits.py` & `gnssrefl-1.3.5/gnssrefl/download_orbits.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/download_psmsl.py` & `gnssrefl-1.3.5/gnssrefl/download_psmsl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/download_rinex.py` & `gnssrefl-1.3.5/gnssrefl/download_rinex.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,16 @@
 
     If you want to specify an archive:
 
     download_rinex p101 2015 52 0 -archive sopac
 
     RINEX 3 instructions need to be added.
 
+    decimate does not seem to do anything, at least not for RINEX 2.11 files
+
     Parameters
     ----------
     station : str
         4 or 9 character ID of the station.
 
     year : int
         Year
```

### Comparing `gnssrefl-1.3.4/gnssrefl/download_teqc.py` & `gnssrefl-1.3.5/gnssrefl/download_teqc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/download_tides.py` & `gnssrefl-1.3.5/gnssrefl/download_tides.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/download_unr.py` & `gnssrefl-1.3.5/gnssrefl/download_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/download_wsv.py` & `gnssrefl-1.3.5/gnssrefl/download_wsv.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/felipe.py` & `gnssrefl-1.3.5/gnssrefl/felipe.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/filesizes.py` & `gnssrefl-1.3.5/gnssrefl/filesizes.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/gnssir.py` & `gnssrefl-1.3.5/gnssrefl/gnssir.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/gnssir_cl.py` & `gnssrefl-1.3.5/gnssrefl/gnssir_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/gnsssnr.f` & `gnssrefl-1.3.5/gnssrefl/gnsssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/gnsssnrbigger.f` & `gnssrefl-1.3.5/gnssrefl/gnsssnrbigger.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/gps.py` & `gnssrefl-1.3.5/gnssrefl/gps.py`

 * *Files 0% similar despite different names*

```diff
@@ -5424,24 +5424,20 @@
     """
     Picks up a RINEX3 file from BFG network
 
     Parameters 
     -----------
     fstation: string
         4 char station ID
-
     year: integer
         year
-
     doy: integer
         day of year
-
     samplerate: integer
         sample rate of the receiver (default is 30)
-
     debug: boolean
         directory file listing provided if true
         default is false
 
     """
     cdoy = '{:03d}'.format(doy)
     cyyyy = str(year)
```

### Comparing `gnssrefl-1.3.4/gnssrefl/gpssnr.f` & `gnssrefl-1.3.5/gnssrefl/gpssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/gpsweek.py` & `gnssrefl-1.3.5/gnssrefl/gpsweek.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/gpt_1wA.pickle` & `gnssrefl-1.3.5/gnssrefl/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/highrate.py` & `gnssrefl-1.3.5/gnssrefl/highrate.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/installexe_cl.py` & `gnssrefl-1.3.5/gnssrefl/installexe_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/invsnr_cl.py` & `gnssrefl-1.3.5/gnssrefl/invsnr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/invsnr_input.py` & `gnssrefl-1.3.5/gnssrefl/invsnr_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/karnak_libraries.py` & `gnssrefl-1.3.5/gnssrefl/karnak_libraries.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/kelly.py` & `gnssrefl-1.3.5/gnssrefl/kelly.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/llh2xyz.py` & `gnssrefl-1.3.5/gnssrefl/llh2xyz.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/make_json_input.py` & `gnssrefl-1.3.5/gnssrefl/make_json_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/nmea2snr.py` & `gnssrefl-1.3.5/gnssrefl/nmea2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/nmea2snr_cl.py` & `gnssrefl-1.3.5/gnssrefl/nmea2snr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/phase_functions.py` & `gnssrefl-1.3.5/gnssrefl/phase_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/prn2gps.py` & `gnssrefl-1.3.5/gnssrefl/prn2gps.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/query_unr.py` & `gnssrefl-1.3.5/gnssrefl/query_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/quickLook_cl.py` & `gnssrefl-1.3.5/gnssrefl/quickLook_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/quickLook_function.py` & `gnssrefl-1.3.5/gnssrefl/quickLook_function.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/quickPhase.py` & `gnssrefl-1.3.5/gnssrefl/quickPhase.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/quickPhase_function.py` & `gnssrefl-1.3.5/gnssrefl/quickPhase_function.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/quickplt.py` & `gnssrefl-1.3.5/gnssrefl/quickplt.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     parser = argparse.ArgumentParser()
     parser.add_argument("filename", help="filename", type=str)
     parser.add_argument("xcol", help="x-column", type=str)
     parser.add_argument("ycol",   help="y-column", type=str)
     parser.add_argument("-mjd", help="set to True/T if x-values are MJD (should add MM/SS?", type=str,default=None)
     parser.add_argument("-reverse", help="set to True/T to reverse the y-axis", type=str,default=None)
-    parser.add_argument("-ymdh", help="if True/T, columns 1-4 are year mon day hour ", type=str,default=None)
+    parser.add_argument("-ymdhm", help="if True/T, columns 1-4 are year mon day hour minute", type=str,default=None)
     parser.add_argument("-xlabel", type=str, help="optional x-axis label", default=None)
     parser.add_argument("-ylabel", type=str, help="optional y-axis label", default=None)
     parser.add_argument("-symbol", help="plot symbol ", type=str,default=None)
     parser.add_argument("-title", help="optional title", type=str,default=None)
     parser.add_argument("-outfile", help="optional filename for plot", type=str,default=None)
     parser.add_argument("-ylimits", nargs="*",type=float, help="optional ylimits", default=None)
 
@@ -68,16 +68,17 @@
 
     secondFile = False
 
     reverse_sign = False
     if (args.reverse == 'True') or (args.reverse == 'T'):
         reverse_sign = True
 
+    # was previously ymdh
     ymd = False
-    if (args.ymdh == 'True') or (args.ymdh == 'T'):
+    if (args.ymdhm == 'True') or (args.ymdhm == 'T'):
         ymd = True
 
     convert_mjd = False
     if (args.mjd== 'True') or (args.mjd == 'T'):
         convert_mjd = True
 
     commentsign = '%'
@@ -98,24 +99,25 @@
         if len(tvd2) == 0:
             print('empty input file number 2')
             return
 
 
     if ymd == True:
         year = tvd[:,0]; month = tvd[:,1]; day = tvd[:,2];
-        hour = tvd[:,3]
+        hour = tvd[:,3] ; minute = tvd[:,4]
         for i in range(0,len(tvd)):
             if (tvd[i, 4]) > 0:
                 y = int(year[i]); m = int(month[i]); d = int(day[i])
                 # i am sure there is a better way to do this
                 today=datetime.datetime(y,m,d)
                 doy = (today - datetime.datetime(today.year, 1, 1)).days + 1
                 h = int(hour[i])
-                tval.append(y + (doy +  h/24)/365.25);
-                yval.append( tvd[i,4]/1000)
+                mi = int(minute[i])
+                tval.append(y + (doy +  h/24 + mi/24/60)/365.25);
+                yval.append( tvd[i,ycol]/1000)
     else:
         if convert_mjd:
             t1 = Time(tvd[:,xcol],format='mjd')
             t1_utc = t1.utc # change to UTC
             # probably can be done in one step!
             tval =  t1_utc.datetime # change to datetime
             yval = tvd[:,ycol] # save the y values
```

### Comparing `gnssrefl-1.3.4/gnssrefl/read_snr_files.py` & `gnssrefl-1.3.5/gnssrefl/read_snr_files.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/refl_zones.py` & `gnssrefl-1.3.5/gnssrefl/refl_zones.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/refl_zones_cl.py` & `gnssrefl-1.3.5/gnssrefl/refl_zones_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/refraction.py` & `gnssrefl-1.3.5/gnssrefl/refraction.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/rh_plot.py` & `gnssrefl-1.3.5/gnssrefl/rh_plot.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/rinex2snr.py` & `gnssrefl-1.3.5/gnssrefl/rinex2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/rinex2snr_cl.py` & `gnssrefl-1.3.5/gnssrefl/rinex2snr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/rinex3_rinex2.py` & `gnssrefl-1.3.5/gnssrefl/rinex3_rinex2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/rinex3_snr.py` & `gnssrefl-1.3.5/gnssrefl/rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/rinpy.py` & `gnssrefl-1.3.5/gnssrefl/rinpy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/rt_rinex3_snr.py` & `gnssrefl-1.3.5/gnssrefl/rt_rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/snow_functions.py` & `gnssrefl-1.3.5/gnssrefl/snow_functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -145,14 +145,15 @@
     fout.write("{0:s}  \n".format(line3))
 
     # first need to make a daily average of results that passed hte azimuth bare soil
     # get the year values
     yvals = np.unique(usegps[:,0])
     snow = []
     yerr = []
+    std= []
     for y in yvals:
         y=int(y) # make sure y is an integer
         for d in range(1,367): # life is short - just do all day of years
             i = (usegps[:,0] == y) & (usegps[:,1]== d)
             nvals = len(usegps[i,0])
             if (nvals >  0):
                 snowv = np.mean(snowAccum[i])
@@ -166,23 +167,26 @@
                 dd = int(np.unique(usegps[i,4]))
                 # make up a list of results for the plot - will convert to np array later
                 snow.append(snowv)
                 yerr.append(std)
 
                 gobst = np.append(gobst, datetime.datetime(year=y, month=mm, day=dd) )
                 fout.write("{0:4.0f} {1:3.0f}  {2:8.3f}  {3:8.3f}  {4:2.0f}  {5:2.0f}   {6:3.0f} \n".format(y, d, snowv, std, mm, dd,nvals))
+                #print(y,d,snowv)
 
     fout.close()
+    if len(snow) == 0:
+        print('Very likely this failed - and you do not have enough bare soil values')
     snow = np.asarray(snow)
     std = np.asarray(std)
 
     return gobst, snow, std
 
 
-def snow_simple(station,gps,year,longer, doy1,doy2,bs,plt, end_dt,outputpng,outputfile,minS,maxS):
+def snow_simple(station,gps,year,longer, doy1,doy2,bs,plt, end_dt,outputpng,outputfile,minS,maxS,barereq_days):
     """
     simple snow depth algorithm
 
     Parameters
     ----------
     station : str
         4 ch station name
@@ -207,28 +211,32 @@
         name of the output (plot) png file
     outputfile : str
         name of the output snowdepth txt file
     minS : float
         minimum snowdepth for plot (m)
     maxS : float
         maximum snowdepth for plot (m)
+    barereq_days: int
+        min number of days to believe a bare soil average
 
     """
     ii = (gps[:,1] >= doy1) & ((gps[:,1] <= doy2) & (gps[:,0] == bs))
 
     baresoil = gps[ii,2]
     if len(baresoil) == 0:
         print('No values in the bare soil definition. Exiting')
         print('Current settings are ', bs, ' for days ', doy1, doy2)
         sys.exit()
 
-    # require at least 15 values
-    NB = 15
+    # require at least 15 values (set in snowdepth_cl.py)
+    NB = barereq_days
+    print('Found ', len(baresoil), ' daily bare soil values')
     if len(baresoil) < NB:
-        print('Not enough values to define baresoil: ', NB)
+        print('Current settings for bare soil are year/', bs, ' for days ', doy1, doy2)
+        print('Code requires: ', NB)
         sys.exit()
 
     noSnowRH = np.mean(baresoil)
     print('Bare Soil RH: ', '{0:7.3f}'.format( noSnowRH),'(m)' )
 
     starting, ending, left, right = time_limits(year, longer)
 
@@ -302,17 +310,18 @@
 
     plt.savefig(outputpng, dpi=300)
     if pltit:
         plt.show()
 
     return
 
-def snow_azimuthal(station,gps,year,longer, doy1,doy2,bs,plt, end_dt,outputpng,outputfile,minS,maxS):
+def snow_azimuthal(station,gps,year,longer, doy1,doy2,bs,plt, end_dt,outputpng,outputfile,minS,maxS,barereq_days):
     """
     azimuthal snow depth algorithm
+    tries to determine the bare soil correction in 20 degree azimuth swaths
 
     Parameters
     ----------
     station : str
         4 ch station name
     gps : numpy array
         output of daily average RH file
@@ -335,27 +344,31 @@
         name of the output (plot) png file
     outputfile : str
         name of the output snowdepth txt file
     minS : float
         minimum snowdepth for plot (m)
     maxS : float
         maximum snowdepth for plot (m)
+    barereq_days : int 
+        number of days required to trust a bare soil average
 
     """
     ii = (gps[:,1] >= doy1) & ((gps[:,1] <= doy2) & (gps[:,0] == bs))
 
     baresoilAll = gps[ii,:]
     baresoil = gps[ii,2] # 
     if len(baresoil) == 0:
         print('No values in the bare soil definition. Exiting')
         print('Current settings are ', bs, ' for days ', doy1, doy2)
         sys.exit()
 
     # require at least 15 values (this is not very useful)
-    NB = 15
+    # this constraint is actually done later ...
+    # could be removed
+    NB = barereq_days
     if len(baresoil) < NB:
         print('Not enough values to define baresoil: ', NB)
         sys.exit()
 
     starting, ending, left, right = time_limits(year, longer)
 
     # window current water year's data to within time limits
@@ -367,28 +380,30 @@
         sys.exit()
 
     # now get bare soil value for each 20 degree azimuth range
     # year, doy, snowAccum, avgAzim, Nval
 
     rebase = np.empty(shape=[0, 12])
 
+    # how many degrees of azimuth are used in each "bare soil" correction
     delA = 20
     for az in range(0,360-delA,delA):
         # bare soil in the azimuth range
         jj = ( baresoilAll[:,5] >= az)  & (baresoilAll[:,5] <= (az+delA))
         pout = baresoilAll[jj,:]
         nr,nc=np.shape(pout)
 
         # all RH in the azimuth range
         kk = (usegps[:,5] > az) & (usegps[:,5] < (az+delA))
-
-        if nr > NB:
+        # number of unique days where a bare soil retrieval exists
+        ndoy = len(np.unique(pout[:,1]))
+        if ndoy > NB:
             # what is the average RH value for this azimuth bin for bare soil
             bsoil = np.mean(pout[:,2])
-            print('Bare soil in azimuth range ', az, az+delA, np.round(bsoil,2), '(m)')
+            print('In azim. range ', az, az+delA, np.round(bsoil,2), '(m), nvals:', len(pout[:,2]),ndoy)
 
             gps_in_azim = usegps[kk,:]
             nr,nc = np.shape(gps_in_azim)
 
             onecol = bsoil + np.zeros((nr,1)) #
 
             # add a column with bare soil value
```

### Comparing `gnssrefl-1.3.4/gnssrefl/snowdepth_cl.py` & `gnssrefl-1.3.5/gnssrefl/snowdepth_cl.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse
+import matplotlib.pyplot as matplt
 import numpy as np
 import datetime 
 import os
 import sys
 
 import gnssrefl.gps as g
 import gnssrefl.snow_functions as sf
@@ -21,29 +22,30 @@
     parser.add_argument("-bare_date1", help="bare soil start yyyy-mm-dd", type=str, default=None)
     parser.add_argument("-bare_date2", help="bare soil end yyyy-mm-dd", type=str, default=None)
     parser.add_argument("-plt_enddate", help="end date for the plot, yyyy-mm-dd", type=str, default=None)
     parser.add_argument("-plt", help="whether you want the plot to come to the screen", type=str, default=None)
     parser.add_argument("-simple", help="use simple algorithm (default is false)", type=str, default=None)
     parser.add_argument("-medfilter", help="median filter for daily average(m)", type=float, default=None)
     parser.add_argument("-ReqTracks", help="how many arcs needed for daily average)", type=int, default=None)
+    parser.add_argument("-barereq_days", help="how many bare soil values req (default is 15)", type=int, default=None)
 
     args = parser.parse_args().__dict__
 
     # convert all expected boolean inputs from strings to booleans
     #boolean_args = ['plt', 'csv','test']
     boolean_args = ['longer','plt','simple']
     args = str2bool(args, boolean_args)
 
     # only return a dictionary of arguments that were added from the user - all other defaults will be set in code below
     return {key: value for key, value in args.items() if value is not None}
 
 
 def snowdepth(station: str, year: int, minS: float=None, maxS: float=None,
         longer:bool=False, plt:bool=True, bare_date1:str=None, bare_date2:str=None, 
-        plt_enddate:str=None,simple:bool=False, medfilter:float = None, ReqTracks: int = None):
+        plt_enddate:str=None,simple:bool=False, medfilter:float = None, ReqTracks: int = None, barereq_days: int = 15):
     """
     Calculates snow depth for a given station and water year.
     Before you run this code you must have run gnssir for each day of interest.  
 
     You can then run daily_avg to concatenate the results or you can input appropriate 
     values to optional inputs medfilter and ReqTracks.  
 
@@ -92,20 +94,24 @@
         which means you use azimuth corrected bare soil values
     medfilter: float, optional
         to avoid running daily_avg, you can set median filter in meters;
         this is used to remove large outliers
     ReqTracks: int, optional
         to avoid running daily_avg, you can set required number of tracks 
         to create a daily average RH
+    barereq_days: int, optional
+        how many bare soil days are required to trust the result, default is 15
 
     """
     if (medfilter is not None) and (ReqTracks is not None):
         print('Running daily average')
         txtfile=None; pltit = False
         da.daily_avg(station, medfilter, ReqTracks,  txtfile,pltit,'',2005,2030,0,False,0,360,False,None)
+        # do not display these plots
+        matplt.close ('all')
 
     # default days of year used for bare soil
     # september from the fall
     doy1 = 244 
     doy2 = 274
     bs = year - 1
 
@@ -145,17 +151,17 @@
     # this overrides other ways of doing things.
     if bare_date1 is not None:
         bs, doy1 = g.cdate2ydoy(bare_date1)
     if bare_date2 is not None:
         rrrr, doy2 = g.cdate2ydoy(bare_date2)
 
     if simple:
-        sf.snow_simple(station,gps,year,longer, doy1,doy2,bs,plt, end_dt,outputpng,outputfile,minS,maxS)
+        sf.snow_simple(station,gps,year,longer, doy1,doy2,bs,plt, end_dt,outputpng,outputfile,minS,maxS,barereq_days)
     else:
-        sf.snow_azimuthal(station,gps,year,longer, doy1,doy2,bs,plt, end_dt,outputpng,outputfile,minS,maxS)
+        sf.snow_azimuthal(station,gps,year,longer, doy1,doy2,bs,plt, end_dt,outputpng,outputfile,minS,maxS,barereq_days)
 
 def main():
     args = parse_arguments()
     snowdepth(**args)
 
 
 if __name__ == "__main__":
```

### Comparing `gnssrefl-1.3.4/gnssrefl/spline_functions.py` & `gnssrefl-1.3.5/gnssrefl/spline_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/subdaily.py` & `gnssrefl-1.3.5/gnssrefl/subdaily.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,29 +17,30 @@
 import scipy.interpolate as interpolate
 from scipy.interpolate import interp1d
 import math
 
 def writeout_spline_outliers(tvd_bad,txtdir,residual,filename):
     """
 
-    Write splinefit outliers to a file. 
+    Write splinefit outliers to a text file. 
 
     Parameters
     ----------
     tvd_bad : numpy array
         output of the lomb scargle calculations
 
     txtdir : str
         directory for the output, i.e. $REFL_CODE/FiLes/station
 
     residual : numpy array
         outlier in units of meters (!)
 
     filename : str
         name of file being written
+
     """
     nr,nc=tvd_bad.shape
     if nr > 0:
         f = txtdir + '/' + filename
         print(nr, ' Outliers written to: ', f)
         fout = open(f, 'w+')
         # put in a header
@@ -271,15 +272,17 @@
                     ntv[i,15], ntv[i,16],month,day,hour,minute, int(second)))
     fout.close()
 
 
 def readin_and_plot(station, year,d1,d2,plt2screen,extension,sigma,writecsv,azim1,azim2,ampl,
         peak2noise,txtfile,h1,h2,kplt,txtdir,default_usage):
     """
-    reads in RH results and makes various plots to help users assess the quality of the solution
+    Reads in RH results and makes various plots to help users assess the quality of the solution
+
+    This is basically "section 1" of the code
 
     Parameters
     ----------
     station : str
         4 character station name
     year : int
         full year
@@ -478,18 +481,18 @@
 def quickTr(year, doy,frachours):
     """
     takes timing from lomb scargle code (year, doy) and UTC hour (fractional)
     and returns a date string
 
     Parameters
     ----------
-    year : integer
-
-    doy : integer
-
+    year : int
+        full year
+    doy : int
+        day of year
     frachours : float
         real-valued UTC hour 
 
     Returns
     -------
     datestring : str
          date ala YYYY-MM-DD HH-MM-SS
```

### Comparing `gnssrefl-1.3.4/gnssrefl/subdaily_cl.py` & `gnssrefl-1.3.5/gnssrefl/subdaily_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/utils.py` & `gnssrefl-1.3.5/gnssrefl/utils.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/veg_multiyr.py` & `gnssrefl-1.3.5/gnssrefl/veg_multiyr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/vwc.py` & `gnssrefl-1.3.5/gnssrefl/vwc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/vwc_input.py` & `gnssrefl-1.3.5/gnssrefl/vwc_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/xyz2llh.py` & `gnssrefl-1.3.5/gnssrefl/xyz2llh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/ydoy.py` & `gnssrefl-1.3.5/gnssrefl/ydoy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl/ymd.py` & `gnssrefl-1.3.5/gnssrefl/ymd.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/gnssrefl.egg-info/PKG-INFO` & `gnssrefl-1.3.5/gnssrefl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 1.3.4
+Version: 1.3.5
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gnssrefl
 
-**github version: 1.3.3** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.3.5** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
 Our documentation is now available [here.](https://gnssrefl.readthedocs.io/en/latest/)
 
 The [shortcourse registration page is live.](https://www.earthscope.org/event/2023-gnss-ir-short-course) 
 
 If you want to sign up for the GNSS-IR email list, please contact Kristine Larson.
```

### Comparing `gnssrefl-1.3.4/gnssrefl.egg-info/SOURCES.txt` & `gnssrefl-1.3.5/gnssrefl.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 setup.py
 gnssrefl/EGM96.py
 gnssrefl/__init__.py
 gnssrefl/check_rinex.py
 gnssrefl/check_rinex2.py
+gnssrefl/check_rinex_file.py
 gnssrefl/computemp1mp2.py
 gnssrefl/daily_avg.py
 gnssrefl/daily_avg_cl.py
 gnssrefl/download_ioc.py
 gnssrefl/download_noaa.py
 gnssrefl/download_orbits.py
 gnssrefl/download_psmsl.py
```

### Comparing `gnssrefl-1.3.4/gnssrefl.egg-info/entry_points.txt` & `gnssrefl-1.3.5/gnssrefl.egg-info/entry_points.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [console_scripts]
 check_rinex = gnssrefl.check_rinex:main
-check_rinex2 = gnssrefl.check_rinex2:main
+check_rinex_file = gnssrefl.check_rinex_file:main
 daily_avg = gnssrefl.daily_avg_cl:main
 download_orbits = gnssrefl.download_orbits:main
 download_rinex = gnssrefl.download_rinex:main
 download_teqc = gnssrefl.download_teqc:main
 download_tides = gnssrefl.download_tides:main
 download_unr = gnssrefl.download_unr:main
 filesizes = gnssrefl.filesizes:main
```

### Comparing `gnssrefl-1.3.4/pyproject.toml` & `gnssrefl-1.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.4/setup.py` & `gnssrefl-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = ["numpy","wget","scipy","matplotlib","requests","progress","astropy","simplekml","earthscope-sdk"]
 setup(
     name="gnssrefl",
-    version="1.3.4",
+    version="1.3.5",
     author="Kristine Larson",
     author_email="kristinem.larson@gmail.com",
     description="A GNSS reflectometry software package ",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/kristinemlarson/gnssrefl/",
     packages=find_packages(),
@@ -53,15 +53,15 @@
             'download_unr = gnssrefl.download_unr:main',
             'query_unr= gnssrefl.query_unr:main',
             'mp1mp2= gnssrefl.computemp1mp2:main',
             'download_teqc = gnssrefl.download_teqc:main',
             'rinex3_rinex2= gnssrefl.rinex3_rinex2:main',
             'veg_multiyr= gnssrefl.veg_multiyr:main',
             'check_rinex= gnssrefl.check_rinex:main',
-            'check_rinex2= gnssrefl.check_rinex2:main',
+            'check_rinex_file= gnssrefl.check_rinex_file:main',
             'rinex3_snr= gnssrefl.rinex3_snr:main',
             'rt_rinex3_snr= gnssrefl.rt_rinex3_snr:main',
             'filesizes= gnssrefl.filesizes:main',
             'invsnr= gnssrefl.invsnr_cl:main',
             'invsnr_input= gnssrefl.invsnr_input:main',
             'vwc_input= gnssrefl.vwc_input:main',
             'phase= gnssrefl.quickPhase:main',
```

### Comparing `gnssrefl-1.3.4/test/test_gps.py` & `gnssrefl-1.3.5/test/test_gps.py`

 * *Files identical despite different names*

