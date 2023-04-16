# Comparing `tmp/wield.control-0.6.0.tar.gz` & `tmp/wield.control-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wield.control-0.6.0.tar", last modified: Fri Apr 14 23:51:03 2023, max compression
+gzip compressed data, was "wield.control-0.6.1.tar", last modified: Sun Apr 16 00:04:39 2023, max compression
```

## Comparing `wield.control-0.6.0.tar` & `wield.control-0.6.1.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.829856 wield.control-0.6.0/
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.789856 wield.control-0.6.0/LICENSES/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    10280 2021-10-12 20:00:04.000000 wield.control-0.6.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1480 2023-04-14 19:17:47.000000 wield.control-0.6.0/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     7048 2021-10-12 20:00:04.000000 wield.control-0.6.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      483 2023-04-14 19:17:47.000000 wield.control-0.6.0/MANIFEST.in
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1034 2023-04-14 19:17:47.000000 wield.control-0.6.0/NOTICE
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1168 2023-04-14 23:51:03.829856 wield.control-0.6.0/PKG-INFO
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      244 2023-04-14 19:17:47.000000 wield.control-0.6.0/README.md
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      449 2023-04-14 19:17:47.000000 wield.control-0.6.0/pyproject.toml
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1138 2023-04-14 23:51:03.829856 wield.control-0.6.0/setup.cfg
--rwxr-xr-x   0 mcculler  (1000) mcculler  (1000)      746 2023-04-14 19:17:47.000000 wield.control-0.6.0/setup.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.781856 wield.control-0.6.0/src/
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.781856 wield.control-0.6.0/src/wield/
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.793856 wield.control-0.6.0/src/wield/control/
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.793856 wield.control-0.6.0/src/wield/control/AAA/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    26500 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/AAA/AAA.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      550 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/AAA/__init__.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1392 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/AAA/_version.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.793856 wield.control-0.6.0/src/wield/control/AAA/test/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     6531 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/AAA/test/test_AAA.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     6840 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/AAA/test/test_AAA_algo.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    13066 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/AAA/test/test_AAA_present.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.797856 wield.control-0.6.0/src/wield/control/ACE/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    51992 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/ACE/ACE.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     4451 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/ACE/ace_electrical.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    10578 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/ACE/ace_optical.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.797856 wield.control-0.6.0/src/wield/control/ACE/test/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3399 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/ACE/test/test_electronics.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    11613 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/ACE/test/test_lqe.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3424 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/ACE/test/test_reduce.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     8212 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/ACE/test/test_statespace.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3203 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/ACE/tupleize.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.801856 wield.control-0.6.0/src/wield/control/MIMO/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      488 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/MIMO/__init__.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      397 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/MIMO/mimo.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    10269 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/MIMO/response.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    23335 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/MIMO/ss.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.801856 wield.control-0.6.0/src/wield/control/MIMO/test/
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.801856 wield.control-0.6.0/src/wield/control/MIMO/test/HSTS/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     5924 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/MIMO/test/HSTS/HSTS_build.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      374 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/MIMO/test/HSTS/__init__.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    13761 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/MIMO/test/HSTS/readFilter.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      375 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/MIMO/test/__init__.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1277 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/MIMO/test/test_MIMO_build.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3712 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/MIMO/util.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.805856 wield.control-0.6.0/src/wield/control/MIMOtable/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     9867 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/MIMOtable/MIMOtable.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      421 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/MIMOtable/__init__.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.805856 wield.control-0.6.0/src/wield/control/SFLU/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    24590 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SFLU/SFLU.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    17847 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SFLU/SFLUcompute.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      377 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SFLU/__init__.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1359 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SFLU/conversions.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.805856 wield.control-0.6.0/src/wield/control/SFLU/cytoscape_flask/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2100 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SFLU/cytoscape_flask/cytoscape_test.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      473 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SFLU/functions.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     6640 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SFLU/nx2tikz.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    11847 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SFLU/optics.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.809856 wield.control-0.6.0/src/wield/control/SFLU/test/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2048 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SFLU/test/T_SFLU.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    11471 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SFLU/test/T_SFLU_DRFPMI.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     5735 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SFLU/test/T_SFLU_DRFPMI_build.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2984 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SFLU/test/T_SFLU_FC.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     8081 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SFLU/test/T_SFLU_OPODRFPMI.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    14176 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SFLU/test/T_SFLU_nx.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    11756 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SFLU/test/quantum_lib.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     6821 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SFLU/utilities.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.809856 wield.control-0.6.0/src/wield/control/SISO/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      526 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SISO/__init__.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1371 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SISO/design.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    21993 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SISO/response.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2364 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SISO/siso.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    12216 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SISO/ss.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.813856 wield.control-0.6.0/src/wield/control/SISO/test/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     8800 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SISO/test/test_SISO_c2d.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3719 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SISO/test/test_SISO_conversion.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     8318 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SISO/test/test_SISO_delay.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2499 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SISO/test/test_lqe_thiran.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1532 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SISO/test/test_spectral_factorization_ZPK.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2705 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SISO/util.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    22217 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SISO/zpk.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     4516 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/SISO/zpk_d2c_c2d.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.813856 wield.control-0.6.0/src/wield/control/TFmath/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     6301 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/TFmath/TF.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      872 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/TFmath/__init__.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3430 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/TFmath/analytic_functionals.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3568 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/TFmath/order_reduce.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.817856 wield.control-0.6.0/src/wield/control/TFmath/root_bunch/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      508 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/TFmath/root_bunch/__init__.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    36606 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/TFmath/root_bunch/root_bunch.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3722 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/TFmath/roots_bin.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    14057 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/TFmath/roots_matching.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      505 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/__init__.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      474 2023-04-14 23:28:28.000000 wield.control-0.6.0/src/wield/control/_version.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.785856 wield.control-0.6.0/src/wield/control/algorithms/
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.817856 wield.control-0.6.0/src/wield/control/algorithms/statespace/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      378 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/algorithms/statespace/__init__.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.817856 wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      747 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/__init__.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     6633 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/broken.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1746 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/delay_algorithms.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3944 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/eig_algorithms.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    15908 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/matrix_algorithms.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     8511 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/reduce_algorithms.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     4301 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/shuffle_algorithms.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      843 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/slycot_algorithms.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     9672 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/ss_algorithms.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.821856 wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/test/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1100 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/test/SS.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1100 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/test/SS_inv.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     5224 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/test/test_SS_algorithms.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3861 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/test/test_SS_models.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2600 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/test/test_delay.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2580 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/test/test_matrix.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1908 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/xfer_algorithms.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    14014 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/zpk_algorithms.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.821856 wield.control-0.6.0/src/wield/control/algorithms/zpk/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      378 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/algorithms/zpk/__init__.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3657 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/algorithms/zpk/order_reduce.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3722 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/algorithms/zpk/roots_bin.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    13769 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/algorithms/zpk/roots_matching.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    22906 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/algorithms/zpk/srootset.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    21868 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/algorithms/zpk/zrootset.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.821856 wield.control-0.6.0/src/wield/control/linear_values/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      551 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/linear_values/__init__.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    15268 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/linear_values/linear_values.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.825856 wield.control-0.6.0/src/wield/control/linear_values/test/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     4577 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/linear_values/test/T_linear_values.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2223 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/plotting.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.825856 wield.control-0.6.0/src/wield/control/statespace/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      377 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/statespace/__init__.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.825856 wield.control-0.6.0/src/wield/control/statespace/fixme/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2444 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/statespace/fixme/dense_builder.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    35334 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/statespace/fixme/statespace.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.829856 wield.control-0.6.0/src/wield/control/statespace/fixme/test/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     9211 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/statespace/fixme/test/IFO_model.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     9052 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/statespace/fixme/test/IFO_model_noM.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     8231 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/statespace/fixme/test/test_IFO_model.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     5805 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/statespace/fixme/test/test_escher.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    19510 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/statespace/fixme/test/test_minreal.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    13522 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/statespace/ss.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2592 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/statespace/ssprint.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2164 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/string_tuple_keys.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.829856 wield.control-0.6.0/src/wield/control/test/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    11851 2023-04-14 19:17:47.000000 wield.control-0.6.0/src/wield/control/test/test_sidles_sigg.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:03.789856 wield.control-0.6.0/src/wield.control.egg-info/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1168 2023-04-14 23:51:03.000000 wield.control-0.6.0/src/wield.control.egg-info/PKG-INFO
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     5090 2023-04-14 23:51:03.000000 wield.control-0.6.0/src/wield.control.egg-info/SOURCES.txt
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)        1 2023-04-14 23:51:03.000000 wield.control-0.6.0/src/wield.control.egg-info/dependency_links.txt
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)       50 2023-04-14 23:51:03.000000 wield.control-0.6.0/src/wield.control.egg-info/requires.txt
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)        6 2023-04-14 23:51:03.000000 wield.control-0.6.0/src/wield.control.egg-info/top_level.txt
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.197292 wield.control-0.6.1/
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.145318 wield.control-0.6.1/LICENSES/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    10280 2021-10-12 20:00:04.000000 wield.control-0.6.1/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1480 2023-04-14 19:17:47.000000 wield.control-0.6.1/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     7048 2021-10-12 20:00:04.000000 wield.control-0.6.1/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      483 2023-04-14 19:17:47.000000 wield.control-0.6.1/MANIFEST.in
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1034 2023-04-14 19:17:47.000000 wield.control-0.6.1/NOTICE
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1168 2023-04-16 00:04:39.197292 wield.control-0.6.1/PKG-INFO
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      244 2023-04-14 19:17:47.000000 wield.control-0.6.1/README.md
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      449 2023-04-14 19:17:47.000000 wield.control-0.6.1/pyproject.toml
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1152 2023-04-16 00:04:39.197292 wield.control-0.6.1/setup.cfg
+-rwxr-xr-x   0 mcculler  (1000) mcculler  (1000)      746 2023-04-14 19:17:47.000000 wield.control-0.6.1/setup.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.133324 wield.control-0.6.1/src/
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.133324 wield.control-0.6.1/src/wield/
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.157312 wield.control-0.6.1/src/wield/control/
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.157312 wield.control-0.6.1/src/wield/control/AAA/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    26500 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/AAA/AAA.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      550 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/AAA/__init__.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1392 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/AAA/_version.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.157312 wield.control-0.6.1/src/wield/control/AAA/test/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     6531 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/AAA/test/test_AAA.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     6840 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/AAA/test/test_AAA_algo.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    13066 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/AAA/test/test_AAA_present.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.161310 wield.control-0.6.1/src/wield/control/ACE/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    51992 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/ACE/ACE.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     4451 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/ACE/ace_electrical.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    10578 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/ACE/ace_optical.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.161310 wield.control-0.6.1/src/wield/control/ACE/test/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3399 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/ACE/test/test_electronics.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    11613 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/ACE/test/test_lqe.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3424 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/ACE/test/test_reduce.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     8212 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/ACE/test/test_statespace.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3203 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/ACE/tupleize.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.161310 wield.control-0.6.1/src/wield/control/MIMO/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      488 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/MIMO/__init__.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      397 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/MIMO/mimo.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    10269 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/MIMO/response.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    23335 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/MIMO/ss.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.165308 wield.control-0.6.1/src/wield/control/MIMO/test/
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.165308 wield.control-0.6.1/src/wield/control/MIMO/test/HSTS/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     5924 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/MIMO/test/HSTS/HSTS_build.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      374 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/MIMO/test/HSTS/__init__.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    13761 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/MIMO/test/HSTS/readFilter.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      375 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/MIMO/test/__init__.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1277 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/MIMO/test/test_MIMO_build.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3712 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/MIMO/util.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.165308 wield.control-0.6.1/src/wield/control/MIMOtable/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     9867 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/MIMOtable/MIMOtable.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      421 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/MIMOtable/__init__.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.165308 wield.control-0.6.1/src/wield/control/SFLU/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    24590 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SFLU/SFLU.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    17847 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SFLU/SFLUcompute.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      377 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SFLU/__init__.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1359 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SFLU/conversions.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.165308 wield.control-0.6.1/src/wield/control/SFLU/cytoscape_flask/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2100 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SFLU/cytoscape_flask/cytoscape_test.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      473 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SFLU/functions.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     6640 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SFLU/nx2tikz.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    11847 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SFLU/optics.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.169306 wield.control-0.6.1/src/wield/control/SFLU/test/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2048 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SFLU/test/T_SFLU.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    11471 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SFLU/test/T_SFLU_DRFPMI.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     5735 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SFLU/test/T_SFLU_DRFPMI_build.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2984 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SFLU/test/T_SFLU_FC.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     8081 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SFLU/test/T_SFLU_OPODRFPMI.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    14176 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SFLU/test/T_SFLU_nx.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    11756 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SFLU/test/quantum_lib.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     6821 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SFLU/utilities.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.169306 wield.control-0.6.1/src/wield/control/SISO/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      526 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SISO/__init__.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1371 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SISO/design.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    21993 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SISO/response.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2364 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SISO/siso.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    12216 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SISO/ss.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.173304 wield.control-0.6.1/src/wield/control/SISO/test/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     8800 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SISO/test/test_SISO_c2d.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3719 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SISO/test/test_SISO_conversion.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     8318 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SISO/test/test_SISO_delay.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2499 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SISO/test/test_lqe_thiran.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1532 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SISO/test/test_spectral_factorization_ZPK.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2705 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SISO/util.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    22217 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SISO/zpk.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     4516 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/SISO/zpk_d2c_c2d.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.185298 wield.control-0.6.1/src/wield/control/TFmath/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     6301 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/TFmath/TF.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      872 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/TFmath/__init__.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3430 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/TFmath/analytic_functionals.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3568 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/TFmath/order_reduce.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.189296 wield.control-0.6.1/src/wield/control/TFmath/root_bunch/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      508 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/TFmath/root_bunch/__init__.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    36606 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/TFmath/root_bunch/root_bunch.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3722 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/TFmath/roots_bin.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    14057 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/TFmath/roots_matching.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      505 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/__init__.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      474 2023-04-16 00:04:01.000000 wield.control-0.6.1/src/wield/control/_version.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.137322 wield.control-0.6.1/src/wield/control/algorithms/
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.189296 wield.control-0.6.1/src/wield/control/algorithms/statespace/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      378 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/algorithms/statespace/__init__.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.189296 wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      747 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/__init__.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     6633 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/broken.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1746 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/delay_algorithms.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3944 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/eig_algorithms.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    15908 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/matrix_algorithms.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     8511 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/reduce_algorithms.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     4301 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/shuffle_algorithms.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      843 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/slycot_algorithms.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     9672 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/ss_algorithms.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.193294 wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/test/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1100 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/test/SS.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1100 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/test/SS_inv.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     5224 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/test/test_SS_algorithms.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3861 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/test/test_SS_models.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2600 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/test/test_delay.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2580 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/test/test_matrix.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1908 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/xfer_algorithms.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    14014 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/zpk_algorithms.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.193294 wield.control-0.6.1/src/wield/control/algorithms/zpk/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      378 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/algorithms/zpk/__init__.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3657 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/algorithms/zpk/order_reduce.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3722 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/algorithms/zpk/roots_bin.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    13769 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/algorithms/zpk/roots_matching.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    22906 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/algorithms/zpk/srootset.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    21868 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/algorithms/zpk/zrootset.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.193294 wield.control-0.6.1/src/wield/control/linear_values/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      551 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/linear_values/__init__.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    15268 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/linear_values/linear_values.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.193294 wield.control-0.6.1/src/wield/control/linear_values/test/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     4577 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/linear_values/test/T_linear_values.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2223 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/plotting.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.193294 wield.control-0.6.1/src/wield/control/statespace/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      377 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/statespace/__init__.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.193294 wield.control-0.6.1/src/wield/control/statespace/fixme/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2444 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/statespace/fixme/dense_builder.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    35334 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/statespace/fixme/statespace.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.193294 wield.control-0.6.1/src/wield/control/statespace/fixme/test/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     9211 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/statespace/fixme/test/IFO_model.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     9052 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/statespace/fixme/test/IFO_model_noM.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     8231 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/statespace/fixme/test/test_IFO_model.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     5805 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/statespace/fixme/test/test_escher.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    19510 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/statespace/fixme/test/test_minreal.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    13522 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/statespace/ss.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2592 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/statespace/ssprint.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2164 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/string_tuple_keys.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.197292 wield.control-0.6.1/src/wield/control/test/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    11851 2023-04-14 19:17:47.000000 wield.control-0.6.1/src/wield/control/test/test_sidles_sigg.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-16 00:04:39.157312 wield.control-0.6.1/src/wield.control.egg-info/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1168 2023-04-16 00:04:39.000000 wield.control-0.6.1/src/wield.control.egg-info/PKG-INFO
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     5090 2023-04-16 00:04:39.000000 wield.control-0.6.1/src/wield.control.egg-info/SOURCES.txt
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)        1 2023-04-16 00:04:39.000000 wield.control-0.6.1/src/wield.control.egg-info/dependency_links.txt
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)       62 2023-04-16 00:04:39.000000 wield.control-0.6.1/src/wield.control.egg-info/requires.txt
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)        6 2023-04-16 00:04:39.000000 wield.control-0.6.1/src/wield.control.egg-info/top_level.txt
```

### Comparing `wield.control-0.6.0/LICENSES/Apache-2.0.txt` & `wield.control-0.6.1/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/LICENSES/BSD-3-Clause.txt` & `wield.control-0.6.1/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/LICENSES/CC0-1.0.txt` & `wield.control-0.6.1/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/NOTICE` & `wield.control-0.6.1/NOTICE`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/PKG-INFO` & `wield.control-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wield.control
-Version: 0.6.0
+Version: 0.6.1
 Summary: Toolkits linear algebra and control systems for signals, physics, and interferometer designs
 Home-page: https://github.com/wieldphysics/wield-control
 Author: Lee McCuller
 Author-email: mcculler@caltech.edu
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/wieldphysics/wield-control/issues
 Project-URL: Source Code, https://github.com/wieldphysics/wield-control
```

### Comparing `wield.control-0.6.0/setup.cfg` & `wield.control-0.6.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wield.control
-version = 0.6.0
+version = 0.6.1
 license = Apache-2.0
 license_files = LICENSES/*, NOTICE
 author = Lee McCuller
 author_email = mcculler@caltech.edu
 description = Toolkits linear algebra and control systems for signals, physics, and interferometer designs
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -23,14 +23,16 @@
 [options]
 setup_requires = 
 	setuptools>=46
 install_requires = 
 	setuptools_scm>=6.0.0
 	wield.bunch
 	wield.utilities
+	numpy
+	scipy
 package_dir = 
 	=src
 packages = find_namespace:
 
 [options.packages.find]
 where = src
```

### Comparing `wield.control-0.6.0/setup.py` & `wield.control-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/AAA/AAA.py` & `wield.control-0.6.1/src/wield/control/AAA/AAA.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/AAA/__init__.py` & `wield.control-0.6.1/src/wield/control/AAA/__init__.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/AAA/_version.py` & `wield.control-0.6.1/src/wield/control/AAA/_version.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/AAA/test/test_AAA.py` & `wield.control-0.6.1/src/wield/control/AAA/test/test_AAA.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/AAA/test/test_AAA_algo.py` & `wield.control-0.6.1/src/wield/control/AAA/test/test_AAA_algo.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/AAA/test/test_AAA_present.py` & `wield.control-0.6.1/src/wield/control/AAA/test/test_AAA_present.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/ACE/ACE.py` & `wield.control-0.6.1/src/wield/control/ACE/ACE.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/ACE/ace_electrical.py` & `wield.control-0.6.1/src/wield/control/ACE/ace_electrical.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/ACE/ace_optical.py` & `wield.control-0.6.1/src/wield/control/ACE/ace_optical.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/ACE/test/test_electronics.py` & `wield.control-0.6.1/src/wield/control/ACE/test/test_electronics.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/ACE/test/test_lqe.py` & `wield.control-0.6.1/src/wield/control/ACE/test/test_lqe.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/ACE/test/test_reduce.py` & `wield.control-0.6.1/src/wield/control/ACE/test/test_reduce.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/ACE/test/test_statespace.py` & `wield.control-0.6.1/src/wield/control/ACE/test/test_statespace.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/ACE/tupleize.py` & `wield.control-0.6.1/src/wield/control/ACE/tupleize.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/MIMO/response.py` & `wield.control-0.6.1/src/wield/control/MIMO/response.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/MIMO/ss.py` & `wield.control-0.6.1/src/wield/control/MIMO/ss.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/MIMO/test/HSTS/HSTS_build.py` & `wield.control-0.6.1/src/wield/control/MIMO/test/HSTS/HSTS_build.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/MIMO/test/HSTS/readFilter.py` & `wield.control-0.6.1/src/wield/control/MIMO/test/HSTS/readFilter.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/MIMO/test/test_MIMO_build.py` & `wield.control-0.6.1/src/wield/control/MIMO/test/test_MIMO_build.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/MIMO/util.py` & `wield.control-0.6.1/src/wield/control/MIMO/util.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/MIMOtable/MIMOtable.py` & `wield.control-0.6.1/src/wield/control/MIMOtable/MIMOtable.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SFLU/SFLU.py` & `wield.control-0.6.1/src/wield/control/SFLU/SFLU.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SFLU/SFLUcompute.py` & `wield.control-0.6.1/src/wield/control/SFLU/SFLUcompute.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SFLU/conversions.py` & `wield.control-0.6.1/src/wield/control/SFLU/conversions.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SFLU/cytoscape_flask/cytoscape_test.py` & `wield.control-0.6.1/src/wield/control/SFLU/cytoscape_flask/cytoscape_test.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SFLU/nx2tikz.py` & `wield.control-0.6.1/src/wield/control/SFLU/nx2tikz.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SFLU/optics.py` & `wield.control-0.6.1/src/wield/control/SFLU/optics.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SFLU/test/T_SFLU.py` & `wield.control-0.6.1/src/wield/control/SFLU/test/T_SFLU.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SFLU/test/T_SFLU_DRFPMI.py` & `wield.control-0.6.1/src/wield/control/SFLU/test/T_SFLU_DRFPMI.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SFLU/test/T_SFLU_DRFPMI_build.py` & `wield.control-0.6.1/src/wield/control/SFLU/test/T_SFLU_DRFPMI_build.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SFLU/test/T_SFLU_FC.py` & `wield.control-0.6.1/src/wield/control/SFLU/test/T_SFLU_FC.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SFLU/test/T_SFLU_OPODRFPMI.py` & `wield.control-0.6.1/src/wield/control/SFLU/test/T_SFLU_OPODRFPMI.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SFLU/test/T_SFLU_nx.py` & `wield.control-0.6.1/src/wield/control/SFLU/test/T_SFLU_nx.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SFLU/test/quantum_lib.py` & `wield.control-0.6.1/src/wield/control/SFLU/test/quantum_lib.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SFLU/utilities.py` & `wield.control-0.6.1/src/wield/control/SFLU/utilities.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SISO/__init__.py` & `wield.control-0.6.1/src/wield/control/SISO/__init__.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SISO/design.py` & `wield.control-0.6.1/src/wield/control/SISO/design.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SISO/response.py` & `wield.control-0.6.1/src/wield/control/SISO/response.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SISO/siso.py` & `wield.control-0.6.1/src/wield/control/SISO/siso.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SISO/ss.py` & `wield.control-0.6.1/src/wield/control/SISO/ss.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SISO/test/test_SISO_c2d.py` & `wield.control-0.6.1/src/wield/control/SISO/test/test_SISO_c2d.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SISO/test/test_SISO_conversion.py` & `wield.control-0.6.1/src/wield/control/SISO/test/test_SISO_conversion.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SISO/test/test_SISO_delay.py` & `wield.control-0.6.1/src/wield/control/SISO/test/test_SISO_delay.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SISO/test/test_lqe_thiran.py` & `wield.control-0.6.1/src/wield/control/SISO/test/test_lqe_thiran.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SISO/test/test_spectral_factorization_ZPK.py` & `wield.control-0.6.1/src/wield/control/SISO/test/test_spectral_factorization_ZPK.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SISO/util.py` & `wield.control-0.6.1/src/wield/control/SISO/util.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SISO/zpk.py` & `wield.control-0.6.1/src/wield/control/SISO/zpk.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/SISO/zpk_d2c_c2d.py` & `wield.control-0.6.1/src/wield/control/SISO/zpk_d2c_c2d.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/TFmath/TF.py` & `wield.control-0.6.1/src/wield/control/TFmath/TF.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/TFmath/__init__.py` & `wield.control-0.6.1/src/wield/control/TFmath/__init__.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/TFmath/analytic_functionals.py` & `wield.control-0.6.1/src/wield/control/TFmath/analytic_functionals.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/TFmath/order_reduce.py` & `wield.control-0.6.1/src/wield/control/TFmath/order_reduce.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/TFmath/root_bunch/root_bunch.py` & `wield.control-0.6.1/src/wield/control/TFmath/root_bunch/root_bunch.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/TFmath/roots_bin.py` & `wield.control-0.6.1/src/wield/control/TFmath/roots_bin.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/TFmath/roots_matching.py` & `wield.control-0.6.1/src/wield/control/TFmath/roots_matching.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/__init__.py` & `wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/__init__.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/broken.py` & `wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/broken.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/delay_algorithms.py` & `wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/delay_algorithms.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/eig_algorithms.py` & `wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/eig_algorithms.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/matrix_algorithms.py` & `wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/matrix_algorithms.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/reduce_algorithms.py` & `wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/reduce_algorithms.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/shuffle_algorithms.py` & `wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/shuffle_algorithms.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/slycot_algorithms.py` & `wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/slycot_algorithms.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/ss_algorithms.py` & `wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/ss_algorithms.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/test/SS.py` & `wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/test/SS.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/test/SS_inv.py` & `wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/test/SS_inv.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/test/test_SS_algorithms.py` & `wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/test/test_SS_algorithms.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/test/test_SS_models.py` & `wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/test/test_SS_models.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/test/test_delay.py` & `wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/test/test_delay.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/test/test_matrix.py` & `wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/test/test_matrix.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/xfer_algorithms.py` & `wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/xfer_algorithms.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/algorithms/statespace/dense/zpk_algorithms.py` & `wield.control-0.6.1/src/wield/control/algorithms/statespace/dense/zpk_algorithms.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/algorithms/zpk/order_reduce.py` & `wield.control-0.6.1/src/wield/control/algorithms/zpk/order_reduce.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/algorithms/zpk/roots_bin.py` & `wield.control-0.6.1/src/wield/control/algorithms/zpk/roots_bin.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/algorithms/zpk/roots_matching.py` & `wield.control-0.6.1/src/wield/control/algorithms/zpk/roots_matching.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/algorithms/zpk/srootset.py` & `wield.control-0.6.1/src/wield/control/algorithms/zpk/srootset.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/algorithms/zpk/zrootset.py` & `wield.control-0.6.1/src/wield/control/algorithms/zpk/zrootset.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/linear_values/__init__.py` & `wield.control-0.6.1/src/wield/control/linear_values/__init__.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/linear_values/linear_values.py` & `wield.control-0.6.1/src/wield/control/linear_values/linear_values.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/linear_values/test/T_linear_values.py` & `wield.control-0.6.1/src/wield/control/linear_values/test/T_linear_values.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/plotting.py` & `wield.control-0.6.1/src/wield/control/plotting.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/statespace/fixme/dense_builder.py` & `wield.control-0.6.1/src/wield/control/statespace/fixme/dense_builder.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/statespace/fixme/statespace.py` & `wield.control-0.6.1/src/wield/control/statespace/fixme/statespace.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/statespace/fixme/test/IFO_model.py` & `wield.control-0.6.1/src/wield/control/statespace/fixme/test/IFO_model.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/statespace/fixme/test/IFO_model_noM.py` & `wield.control-0.6.1/src/wield/control/statespace/fixme/test/IFO_model_noM.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/statespace/fixme/test/test_IFO_model.py` & `wield.control-0.6.1/src/wield/control/statespace/fixme/test/test_IFO_model.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/statespace/fixme/test/test_escher.py` & `wield.control-0.6.1/src/wield/control/statespace/fixme/test/test_escher.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/statespace/fixme/test/test_minreal.py` & `wield.control-0.6.1/src/wield/control/statespace/fixme/test/test_minreal.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/statespace/ss.py` & `wield.control-0.6.1/src/wield/control/statespace/ss.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/statespace/ssprint.py` & `wield.control-0.6.1/src/wield/control/statespace/ssprint.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/string_tuple_keys.py` & `wield.control-0.6.1/src/wield/control/string_tuple_keys.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield/control/test/test_sidles_sigg.py` & `wield.control-0.6.1/src/wield/control/test/test_sidles_sigg.py`

 * *Files identical despite different names*

### Comparing `wield.control-0.6.0/src/wield.control.egg-info/PKG-INFO` & `wield.control-0.6.1/src/wield.control.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wield.control
-Version: 0.6.0
+Version: 0.6.1
 Summary: Toolkits linear algebra and control systems for signals, physics, and interferometer designs
 Home-page: https://github.com/wieldphysics/wield-control
 Author: Lee McCuller
 Author-email: mcculler@caltech.edu
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/wieldphysics/wield-control/issues
 Project-URL: Source Code, https://github.com/wieldphysics/wield-control
```

### Comparing `wield.control-0.6.0/src/wield.control.egg-info/SOURCES.txt` & `wield.control-0.6.1/src/wield.control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

