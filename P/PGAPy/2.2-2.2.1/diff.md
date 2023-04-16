# Comparing `tmp/PGAPy-2.2.tar.gz` & `tmp/PGAPy-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PGAPy-2.2.tar", last modified: Sun Dec  4 16:39:55 2022, max compression
+gzip compressed data, was "PGAPy-2.2.1.tar", last modified: Sun Apr 16 14:30:29 2023, max compression
```

## Comparing `PGAPy-2.2.tar` & `PGAPy-2.2.1.tar`

### file list

```diff
@@ -1,60 +1,87 @@
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2022-12-04 16:39:55.491145 PGAPy-2.2/
--rw-r--r--   0 ralf      (1000) priv      (1011)     1306 2020-05-30 13:50:14.000000 PGAPy-2.2/COPYING
--rw-r--r--   0 ralf      (1000) priv      (1011)     1093 2022-12-02 20:07:09.000000 PGAPy-2.2/MANIFEST.in
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2022-12-04 16:39:55.303146 PGAPy-2.2/PGAPy.egg-info/
--rw-r--r--   0 ralf      (1000) priv      (1011)    57392 2022-12-04 16:39:55.000000 PGAPy-2.2/PGAPy.egg-info/PKG-INFO
--rw-r--r--   0 ralf      (1000) priv      (1011)      985 2022-12-04 16:39:55.000000 PGAPy-2.2/PGAPy.egg-info/SOURCES.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)        1 2022-12-04 16:39:55.000000 PGAPy-2.2/PGAPy.egg-info/dependency_links.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)        4 2022-12-04 16:39:55.000000 PGAPy-2.2/PGAPy.egg-info/top_level.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)    57392 2022-12-04 16:39:55.487146 PGAPy-2.2/PKG-INFO
--rw-r--r--   0 ralf      (1000) priv      (1011)    76124 2022-12-04 16:38:57.000000 PGAPy-2.2/README.html
--rw-r--r--   0 ralf      (1000) priv      (1011)    48784 2022-12-02 19:48:39.000000 PGAPy-2.2/README.rst
--rw-r--r--   0 ralf      (1000) priv      (1011)       22 2022-12-04 16:38:57.000000 PGAPy-2.2/Version.h
--rw-r--r--   0 ralf      (1000) priv      (1011)       14 2022-12-04 16:38:57.000000 PGAPy-2.2/Version.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2022-12-04 16:39:55.363145 PGAPy-2.2/examples/
--rwxr-xr-x   0 ralf      (1000) priv      (1011)     2197 2022-12-02 19:48:39.000000 PGAPy-2.2/examples/cards.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)     2333 2022-12-02 19:48:39.000000 PGAPy-2.2/examples/cards_mutate.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)     2583 2022-12-02 19:48:39.000000 PGAPy-2.2/examples/constraint.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)     4085 2022-12-02 19:48:39.000000 PGAPy-2.2/examples/dtlz2.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)     2608 2022-12-02 19:48:39.000000 PGAPy-2.2/examples/fourbar.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)     4508 2022-12-02 19:48:39.000000 PGAPy-2.2/examples/gears.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2022-12-04 16:39:55.379145 PGAPy-2.2/examples/gp/
--rw-r--r--   0 ralf      (1000) priv      (1011)     2460 2022-12-02 19:48:39.000000 PGAPy-2.2/examples/gp/README.rst
--rwxr-xr-x   0 ralf      (1000) priv      (1011)    22896 2022-12-02 19:48:39.000000 PGAPy-2.2/examples/gp/gp.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)     9217 2022-12-04 15:00:04.000000 PGAPy-2.2/examples/gp/opt_integral.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)     2839 2022-12-04 15:00:37.000000 PGAPy-2.2/examples/gp/opt_parity3.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)     2696 2022-12-04 15:00:57.000000 PGAPy-2.2/examples/gp/opt_xor.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)     3535 2022-12-02 19:48:39.000000 PGAPy-2.2/examples/hello_world_char.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)     2455 2022-12-02 19:48:39.000000 PGAPy-2.2/examples/hello_world_int.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)     2802 2022-12-02 19:48:39.000000 PGAPy-2.2/examples/himmelblau.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)     6986 2022-12-02 19:48:39.000000 PGAPy-2.2/examples/magic_prio.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)    10362 2022-12-02 19:48:39.000000 PGAPy-2.2/examples/magic_square.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)     3568 2022-12-02 19:48:39.000000 PGAPy-2.2/examples/minfloat.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)     2833 2022-12-02 19:48:39.000000 PGAPy-2.2/examples/multi.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)     4730 2022-12-02 19:48:39.000000 PGAPy-2.2/examples/namefull.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)     2290 2022-12-02 19:48:39.000000 PGAPy-2.2/examples/one_max.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2022-12-04 16:39:55.395146 PGAPy-2.2/examples/sequence/
--rw-r--r--   0 ralf      (1000) priv      (1011)      821 2022-08-18 16:53:20.000000 PGAPy-2.2/examples/sequence/croes.tsp
--rw-r--r--   0 ralf      (1000) priv      (1011)     1090 2022-08-18 16:53:20.000000 PGAPy-2.2/examples/sequence/oliver30.tsp
--rwxr-xr-x   0 ralf      (1000) priv      (1011)     5276 2022-08-18 16:53:20.000000 PGAPy-2.2/examples/sequence/plot_tour.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)    50389 2022-12-04 14:54:43.000000 PGAPy-2.2/examples/sequence/tsp.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)     2044 2022-12-02 19:48:39.000000 PGAPy-2.2/examples/sort_numbers.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)     2704 2022-12-02 19:48:39.000000 PGAPy-2.2/examples/twobar.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)     3505 2022-12-02 19:48:39.000000 PGAPy-2.2/examples/vibr.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)     4775 2022-12-02 19:48:39.000000 PGAPy-2.2/examples/xor.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2022-12-04 16:39:55.407146 PGAPy-2.2/pga/
--rw-r--r--   0 ralf      (1000) priv      (1011)     1729 2022-12-04 15:02:41.000000 PGAPy-2.2/pga/__init__.py
--rw-r--r--   0 ralf      (1000) priv      (1011)     2240 2022-12-04 15:02:17.000000 PGAPy-2.2/pga/random.py
--rw-r--r--   0 ralf      (1000) priv      (1011)     3996 2022-12-04 15:25:31.000000 PGAPy-2.2/pga/testsupport.py
--rw-r--r--   0 ralf      (1000) priv      (1011)   113155 2022-12-04 16:19:53.000000 PGAPy-2.2/pgamodule.c
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2022-12-04 16:39:55.239146 PGAPy-2.2/pgapack/
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2022-12-04 16:39:55.411146 PGAPy-2.2/pgapack/docs/
--rw-r--r--   0 ralf      (1000) priv      (1011)   555039 2022-12-04 16:38:59.000000 PGAPy-2.2/pgapack/docs/user_guide.pdf
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2022-12-04 16:39:55.463146 PGAPy-2.2/pgapack/fakempi/
--rw-r--r--   0 ralf      (1000) priv      (1011)     2184 2022-10-26 11:34:30.000000 PGAPy-2.2/pgapack/fakempi/mpi.h
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2022-12-04 16:39:55.467146 PGAPy-2.2/pgapack/include/
--rw-r--r--   0 ralf      (1000) priv      (1011)    60150 2022-12-02 19:37:54.000000 PGAPy-2.2/pgapack/include/pgapack.h
--rw-r--r--   0 ralf      (1000) priv      (1011)       38 2022-12-04 16:39:55.491145 PGAPy-2.2/setup.cfg
--rw-r--r--   0 ralf      (1000) priv      (1011)     8551 2022-12-04 16:04:25.000000 PGAPy-2.2/setup.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2022-12-04 16:39:55.479145 PGAPy-2.2/test/
--rw-r--r--   0 ralf      (1000) priv      (1011)    23792 2022-12-04 15:23:46.000000 PGAPy-2.2/test/test_pgapy.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-04-16 14:30:29.894634 PGAPy-2.2.1/
+-rw-r--r--   0 ralf      (1000) priv      (1011)     1306 2020-05-30 13:50:14.000000 PGAPy-2.2.1/COPYING
+-rw-r--r--   0 ralf      (1000) priv      (1011)     1093 2022-12-02 20:07:09.000000 PGAPy-2.2.1/MANIFEST.in
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-04-16 14:30:29.562634 PGAPy-2.2.1/PGAPy.egg-info/
+-rw-r--r--   0 ralf      (1000) priv      (1011)    60061 2023-04-16 14:30:29.000000 PGAPy-2.2.1/PGAPy.egg-info/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)     1605 2023-04-16 14:30:29.000000 PGAPy-2.2.1/PGAPy.egg-info/SOURCES.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)        1 2023-04-16 14:30:29.000000 PGAPy-2.2.1/PGAPy.egg-info/dependency_links.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)        4 2023-04-16 14:30:29.000000 PGAPy-2.2.1/PGAPy.egg-info/top_level.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)    60061 2023-04-16 14:30:29.894634 PGAPy-2.2.1/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)    80231 2023-04-16 14:30:00.000000 PGAPy-2.2.1/README.html
+-rw-r--r--   0 ralf      (1000) priv      (1011)    50931 2023-04-16 14:07:34.000000 PGAPy-2.2.1/README.rst
+-rw-r--r--   0 ralf      (1000) priv      (1011)       24 2023-04-16 14:30:01.000000 PGAPy-2.2.1/Version.h
+-rw-r--r--   0 ralf      (1000) priv      (1011)       16 2023-04-16 14:30:01.000000 PGAPy-2.2.1/Version.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-04-16 14:30:29.622634 PGAPy-2.2.1/examples/
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)     2197 2022-12-02 19:48:39.000000 PGAPy-2.2.1/examples/cards.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)     2333 2022-12-02 19:48:39.000000 PGAPy-2.2.1/examples/cards_mutate.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)     2583 2022-12-02 19:48:39.000000 PGAPy-2.2.1/examples/constraint.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)     4085 2022-12-02 19:48:39.000000 PGAPy-2.2.1/examples/dtlz2.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)     2608 2022-12-02 19:48:39.000000 PGAPy-2.2.1/examples/fourbar.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)     4508 2022-12-02 19:48:39.000000 PGAPy-2.2.1/examples/gears.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-04-16 14:30:29.638634 PGAPy-2.2.1/examples/gp/
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2460 2022-12-02 19:48:39.000000 PGAPy-2.2.1/examples/gp/README.rst
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)    22896 2022-12-02 19:48:39.000000 PGAPy-2.2.1/examples/gp/gp.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)     9217 2022-12-04 15:00:04.000000 PGAPy-2.2.1/examples/gp/opt_integral.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)     2839 2022-12-04 15:00:37.000000 PGAPy-2.2.1/examples/gp/opt_parity3.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)     2696 2022-12-04 15:00:57.000000 PGAPy-2.2.1/examples/gp/opt_xor.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)     3535 2022-12-02 19:48:39.000000 PGAPy-2.2.1/examples/hello_world_char.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)     2455 2022-12-02 19:48:39.000000 PGAPy-2.2.1/examples/hello_world_int.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)     2802 2022-12-02 19:48:39.000000 PGAPy-2.2.1/examples/himmelblau.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)     6986 2022-12-02 19:48:39.000000 PGAPy-2.2.1/examples/magic_prio.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)    10362 2023-01-10 11:23:19.000000 PGAPy-2.2.1/examples/magic_square.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)     3568 2022-12-02 19:48:39.000000 PGAPy-2.2.1/examples/minfloat.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)     2833 2022-12-02 19:48:39.000000 PGAPy-2.2.1/examples/multi.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)     4730 2022-12-02 19:48:39.000000 PGAPy-2.2.1/examples/namefull.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)     2290 2022-12-02 19:48:39.000000 PGAPy-2.2.1/examples/one_max.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-04-16 14:30:29.650634 PGAPy-2.2.1/examples/sequence/
+-rw-r--r--   0 ralf      (1000) priv      (1011)      821 2022-08-18 16:53:20.000000 PGAPy-2.2.1/examples/sequence/croes.tsp
+-rw-r--r--   0 ralf      (1000) priv      (1011)     1090 2022-08-18 16:53:20.000000 PGAPy-2.2.1/examples/sequence/oliver30.tsp
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)     5276 2022-08-18 16:53:20.000000 PGAPy-2.2.1/examples/sequence/plot_tour.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)    50389 2022-12-04 14:54:43.000000 PGAPy-2.2.1/examples/sequence/tsp.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)     2044 2022-12-02 19:48:39.000000 PGAPy-2.2.1/examples/sort_numbers.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)     2704 2022-12-02 19:48:39.000000 PGAPy-2.2.1/examples/twobar.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)     3505 2022-12-02 19:48:39.000000 PGAPy-2.2.1/examples/vibr.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)     4775 2022-12-02 19:48:39.000000 PGAPy-2.2.1/examples/xor.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-04-16 14:30:29.666634 PGAPy-2.2.1/pga/
+-rw-r--r--   0 ralf      (1000) priv      (1011)     1729 2022-12-04 15:02:41.000000 PGAPy-2.2.1/pga/__init__.py
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2240 2022-12-04 15:02:17.000000 PGAPy-2.2.1/pga/random.py
+-rw-r--r--   0 ralf      (1000) priv      (1011)     3996 2022-12-04 15:25:31.000000 PGAPy-2.2.1/pga/testsupport.py
+-rw-r--r--   0 ralf      (1000) priv      (1011)   113947 2023-04-16 13:28:40.000000 PGAPy-2.2.1/pgamodule.c
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-04-16 14:30:29.502634 PGAPy-2.2.1/pgapack/
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-04-16 14:30:29.670634 PGAPy-2.2.1/pgapack/docs/
+-rw-r--r--   0 ralf      (1000) priv      (1011)   555087 2023-04-16 14:30:03.000000 PGAPy-2.2.1/pgapack/docs/user_guide.pdf
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-04-16 14:30:29.722634 PGAPy-2.2.1/pgapack/fakempi/
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2240 2023-04-16 13:36:21.000000 PGAPy-2.2.1/pgapack/fakempi/mpi.h
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-04-16 14:30:29.726634 PGAPy-2.2.1/pgapack/include/
+-rw-r--r--   0 ralf      (1000) priv      (1011)    66915 2023-04-16 13:16:47.000000 PGAPy-2.2.1/pgapack/include/pgapack.h
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-04-16 14:30:29.874634 PGAPy-2.2.1/pgapack/source/
+-rw-r--r--   0 ralf      (1000) priv      (1011)    35224 2023-04-16 13:16:48.000000 PGAPy-2.2.1/pgapack/source/binary.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)    26834 2023-04-16 13:16:48.000000 PGAPy-2.2.1/pgapack/source/char.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)     9052 2023-04-16 13:16:48.000000 PGAPy-2.2.1/pgapack/source/cmdline.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)    69572 2023-04-16 13:16:48.000000 PGAPy-2.2.1/pgapack/source/create.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)    20380 2023-04-16 13:16:48.000000 PGAPy-2.2.1/pgapack/source/cross.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)    63817 2023-04-16 13:16:48.000000 PGAPy-2.2.1/pgapack/source/debug.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)     9804 2023-04-16 13:16:48.000000 PGAPy-2.2.1/pgapack/source/duplcate.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)    35572 2023-04-16 13:16:48.000000 PGAPy-2.2.1/pgapack/source/evaluate.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)    95299 2023-04-16 13:16:48.000000 PGAPy-2.2.1/pgapack/source/f2c.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)    26363 2023-04-16 13:16:48.000000 PGAPy-2.2.1/pgapack/source/fitness.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)    61076 2023-04-16 13:16:48.000000 PGAPy-2.2.1/pgapack/source/integer.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)    15057 2023-04-16 13:16:48.000000 PGAPy-2.2.1/pgapack/source/linalg.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)    10025 2023-04-16 13:36:21.000000 PGAPy-2.2.1/pgapack/source/mpi_stub.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)    38056 2023-04-16 13:16:48.000000 PGAPy-2.2.1/pgapack/source/mutation.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)    49328 2023-04-16 13:16:48.000000 PGAPy-2.2.1/pgapack/source/parallel.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)    32700 2023-04-16 13:16:48.000000 PGAPy-2.2.1/pgapack/source/pga.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)    49657 2023-04-16 13:16:48.000000 PGAPy-2.2.1/pgapack/source/pop.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)    16516 2023-04-16 13:16:48.000000 PGAPy-2.2.1/pgapack/source/random.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)    48411 2023-04-16 13:16:48.000000 PGAPy-2.2.1/pgapack/source/real.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)    46980 2023-04-16 13:16:48.000000 PGAPy-2.2.1/pgapack/source/report.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)    10171 2023-04-16 13:16:48.000000 PGAPy-2.2.1/pgapack/source/restart.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)    34323 2023-04-16 13:16:48.000000 PGAPy-2.2.1/pgapack/source/select.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)    13423 2023-04-16 13:16:48.000000 PGAPy-2.2.1/pgapack/source/stop.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)    12896 2023-04-16 13:16:48.000000 PGAPy-2.2.1/pgapack/source/system.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)    10711 2023-04-16 13:16:48.000000 PGAPy-2.2.1/pgapack/source/user.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)    43927 2023-04-16 13:16:48.000000 PGAPy-2.2.1/pgapack/source/utility.c
+-rw-r--r--   0 ralf      (1000) priv      (1011)       38 2023-04-16 14:30:29.894634 PGAPy-2.2.1/setup.cfg
+-rw-r--r--   0 ralf      (1000) priv      (1011)     8551 2023-04-16 13:18:12.000000 PGAPy-2.2.1/setup.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-04-16 14:30:29.882634 PGAPy-2.2.1/test/
+-rw-r--r--   0 ralf      (1000) priv      (1011)    23792 2022-12-04 15:23:46.000000 PGAPy-2.2.1/test/test_pgapy.py
```

### Comparing `PGAPy-2.2/COPYING` & `PGAPy-2.2.1/COPYING`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/MANIFEST.in` & `PGAPy-2.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/PGAPy.egg-info/PKG-INFO` & `PGAPy-2.2.1/PGAPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PGAPy
-Version: 2.2
+Version: 2.2.1
 Summary: Python wrapper for pgapack, the parallel genetic algorithm library
 Home-page: http://pgapy.sourceforge.net/
 Author: Ralf Schlatterbeck
 Author-email: rsc@runtux.com
 License: UNKNOWN
 Description: PGAPy: Python Wrapper for PGAPack Parallel Genetic Algorithm Library
         ====================================================================
@@ -13,14 +13,26 @@
         .. |epsilon| unicode:: U+03B5 .. epsilon
         
         :Author: Ralf Schlatterbeck <rsc@runtux.com>
         
         News
         ----
         
+        News 04-2023:
+        
+        - The last build on PyPi was broken for serial installs, it was missing
+          the ``mpi_stub.c`` needed for the serial version. Parallel installs
+          were still possible so I didn't notice, sorry!
+        - Add MPI_Abort to the wrapper, it is called with::
+        
+            pga.MPI_Abort (errcode)
+        
+          See below in secion `Running with MPI`_ how this can be used to abort
+          the MPI run in case of exception in the ``evaluate`` method.
+        
         News 12-2022: Add regression test and update to new upstream with
         several bug-fixes. Includes also some bug fixes in wrapper.
         
         News 10-2022: Add user defined datatypes. Example in ``examples/gp`` use
         user defined data types to implement genetic programming (we represent
         expressions by a tree data structure). This uses the new serialization
         API in pgapack to transfer a Python pickle representation to peer MPI
@@ -64,15 +76,15 @@
         experimentation. It also has shown a remarkably small number of bugs
         over the years. It supports parallel execution via the message
         passing interface MPI_ in addition to a normal "serial" version. That's
         why I wanted to use it in Python, too.
         
         To get started you need the PGAPack library, although
         it now comes bundled with PGApy, to install a *parallel* version you
-        currently need a pre-installed PGApack compiled for the MPI library of
+        currently need a pre-installed PGAPack_ compiled for the MPI library of
         choice. See `Installation`_ section for details.
         
         There currently is not much documentation for PGAPy.
         You really, absolutely need to read the documentation that comes
         with PGAPack.
         The PGAPack user guide is now shipped together with PGAPy. It is
         installed together with some examples in share/pgapy, wherever the
@@ -122,22 +134,14 @@
         As mentioned above, you can find my `PGAPack fork on github`_, this
         repository has the three upstream releases as versions in git and
         contains some updates concerning support of newer MPI_ versions and
         documentation updates.  I've also included patches in the git repository
         of the Debian maintainer of the package, Dirk Eddelbuettel.
         I'm actively maintaining that branch, adding new features and bug-fixes.
         
-        .. _`PGAPack Readme`:
-           https://github.com/schlatterbeck/pgapack/blob/master/README.rst
-        .. _PGAPack:          http://ftp.mcs.anl.gov/pub/pgapack/
-        .. _`PGAPack fork on github`: https://github.com/schlatterbeck/pgapack
-        .. _MPI: http://mpi-forum.org/
-        .. _`my pgapack debian package builder`:
-            https://github.com/schlatterbeck/debian-pgapack
-        
         To get you started, I've included some very simple examples in
         ``examples``, e.g., ``one-max.py`` implements the "Maxbit" example
         similar to one in the PGAPack documentation. The examples were inspired
         by the book "Genetic Algorithms in Python" but are written from scratch
         and don't include any code from the book. The examples illustrates
         several points:
         
@@ -204,43 +208,43 @@
           ``check_stopping_conditions``. An exception of the lowercase-rule is
           whenever a name contains "GA" (for "genetic algorithm"), So
           ``PGASetMaxGAIterValue`` becomes ``max_GA_iter``.
         - Where possible I've made a single class method where PGAPack needs a
           separate function for each datatype, so ``PGAGetBinaryAllele``,
           ``PGAGetCharacterAllele``, ``PGAGetIntegerAllele``, ``PGAGetRealAllele`` all
           become ``get_allele``. Same holds true for ``set_allele``.
-        - Whenever a name in PGApack has a "Value" or "Flag" suffix, I've left
+        - Whenever a name in PGAPack has a "Value" or "Flag" suffix, I've left
           this out, so ``PGAGetFitnessCmaxValue`` becomes ``fitness_cmax``
           and ``PGAGetMutationAndCrossoverFlag`` becomes
           ``mutation_and_crossover``, the only exception to this rule is for the
           two functions ``PGAGetMutationRealValue`` and
           ``PGAGetMutationIntegerValue`` which become ``mutation_value`` not
           just ``mutation``.
         - Some fields can take multiple values (they are implemented by ORing
           integer constants, in python they are specified as a list or tuple of
           constants). These are converted to plural (if not already plural in
-          PGApack), e.g., ``PGASetStoppingRuleType`` becomes ``stopping_rule_types``.
+          PGAPack), e.g., ``PGASetStoppingRuleType`` becomes ``stopping_rule_types``.
         - Internal method names in the wrapper program have a leading PGA\_ |--| so
           the class method ``set_allele`` is implemented by the C-function
           ``PGA_set_allele`` in ``pgamodule.c``.
         
         Constructor Parameters
         ----------------------
         
-        PGApack has a lot of ``PGASet`` and ``PGAGet`` functions for setting
+        PGAPack_ has a lot of ``PGASet`` and ``PGAGet`` functions for setting
         parameters. These are reflected in constructor parameters on the one hand
         and in (typically read-only, but see below) properties of a ``PGA``
         object on the other hand. The
-        following table gives an overview of all the original PGApack names and
-        the names of the python wrapper. For the PGApack name I've only listed
+        following table gives an overview of all the original PGAPack_ names and
+        the names of the python wrapper. For the PGAPack_ name I've only listed
         the ``PGASet`` function, in many cases there is a corresponding
         ``PGAGet`` function. If a corresponding read-only property exists for a
         constructor parameter this is indicated in the "Prop" column. In some
         cases properties are missing because no corresponding ``PGAGet`` function
-        is implemented in PGApack, in other cases returning a numeric value that
+        is implemented in PGAPack_, in other cases returning a numeric value that
         has a symbolic constant in PGApy doesn't make much sense.
         
         The properties have the same name as the constructor parameter.
         There are Properties that don't have a corresponding constructor
         parameter, namely the ``eval_count`` property (returning the count of
         function evaluations), the
         ``GA_iter`` property that returns the current GA generation, and the
@@ -258,15 +262,15 @@
         allele* of the gene. In python this is a sequence of 2-tuples.
         Note that this means that you can have different ranges of allowed values
         for each allele.
         
         The ``num_eval`` property is special: Due to limitations of the C
         programming language, for multiple evaluations in C the first evaluation
         is returned as the function return-value of the ``evaluate`` function
-        and all other parameters are returned in an auxiliary array. PGApack
+        and all other parameters are returned in an auxiliary array. PGAPack_
         specifies the number of auxiliary evaluations to be returned. In Python
         the evaluation function can always return a sequence of evaluation
         values and the ``num_eval`` is one more than ``PGAGetNumAuxEval`` would
         return. The default for ``num_eval`` is 1.
         
         The first two (mandatory) constructor parameters are the type of the gene
         (this takes a Python type, e.g., ``bool`` for a binary genome or ``int``
@@ -278,15 +282,15 @@
         Some properties can now also be set *during* the run of the optimizer.
         These currently are ``crossover_prob``, ``epsilon_exponent``,
         ``multi_obj_precision``, ``p_tournament_prob``, and
         ``uniform_crossover_prob``. Just assign to the member variable of
         the optimizer (child of PGA.pga) object.
         
         ==================================== ================================= ====== ====
-        PGApack name                         Constructor parameter             Type   Prop
+        PGAPack name                         Constructor parameter             Type   Prop
         ==================================== ================================= ====== ====
         ``PGASetCrossoverBoundedFlag``       ``crossover_bounded``             int    yes
         ``PGASetCrossoverBounceBackFlag``    ``crossover_bounce_back``         int    yes
         ``PGASetCrossoverSBXEta``            ``crossover_SBX_eta``             float  yes
         ``PGASetCrossoverSBXOncePerString``  ``crossover_SBX_once_per_string`` int    yes
         ``PGASetCrossoverProb``              ``crossover_prob``                float  yes
         ``PGASetCrossoverType``              ``crossover_type``                sym    no
@@ -424,32 +428,32 @@
         ``set_gene``                  *p, pop, gen*      set gene (user data types)
         ``set_random_seed``           *seed*             None (use constructor!)
         ============================= ================== ===========================
         
         User-Methods
         ------------
         
-        PGApack has the concept of user functions. These allow customization of
+        PGAPack_ has the concept of user functions. These allow customization of
         different areas of a genetic algorihm. In Python they are implemented as
         methods that can be changed in a derived class. One of the methods that
         *must* be implemented in a derived class is the ``evaluate`` function
-        (although technically it is not a user function in PGApack). It
+        (although technically it is not a user function in PGAPack). It
         interprets the gene and returns an evaluation value or a sequence of
         evaluation values if you set the ``num_eval`` constructor parameter.
-        PGApack computes a fitness from the raw evaluation value. For some
+        PGAPack_ computes a fitness from the raw evaluation value. For some
         methods an up-call into the PGA class is possible, for some methods this
         is not possible (and in most cases not reasonable). Note that for the
         ``stop_cond`` method, the standard check for stopping conditions can be
         called with::
         
           self.check_stopping_conditions()
         
         The following table lists the overridable methods with their parameters
         (for the function signature the first parameter *self* is omitted). Note
-        that in PGApack there are additional user functions that are needed for
+        that in PGAPack_ there are additional user functions that are needed for
         user-defined data types which are currently not exposed in Python. In the
         function signatures *p* denotes the index of the individual and *pop*
         denotes the population. If more than one individual is specified (e.g.,
         for crossover) these can be followed by a number. For crossover *c1* and
         *c2* denote the destination individuals (children). The *propability* for
         the mutation method is a floating-point value between 0 and 1. Remember
         to count the number of mutations that happen, and return that value for
@@ -470,15 +474,15 @@
         ``pre_eval``        *pop*                          None              no
         ``print_string``    *file, p, pop*                 None              yes
         =================== ============================== ================= =======
         
         Constants
         ---------
         
-        The following PGApack constants are available:
+        The following PGAPack_ constants are available:
         
         ========================== ===========================================
         Constant                   Description
         ========================== ===========================================
         PGA_CROSSOVER_EDGE         Edge crossover for permutations
         PGA_CROSSOVER_ONEPT        One-point Crossover
         PGA_CROSSOVER_SBX          Simulated Binary Crossover
@@ -586,15 +590,15 @@
         over the serialization of the tree (which is the same for individuals
         with the same tree structure).
         
         
         Missing Features
         ----------------
         
-        As already mentioned, not all functions and constants of PGAPack are
+        As already mentioned, not all functions and constants of PGAPack_ are
         wrapped yet |--| still for many applications the given set should be
         enough. If you need additional functions, you may want to wrap these and
         send_ me a patch.
         
         Reporting Bugs
         --------------
         
@@ -635,15 +639,15 @@
         To install a *serial* version (without parallel programming using MPI_)
         you can simply install from pypi using ``pip``. Alternatively when you
         have unpacked or checked out from sources you can install with::
         
          python3 setup.py install --prefix=/usr/local
         
         If you want a parallel version using an MPI_ (Message-Passing Interface)
-        library you will have to install a parallel version of PGApack first.
+        library you will have to install a parallel version of PGAPack_ first.
         The easiest way to do this is to use `my pgapack debian package builder`_
         from github. Clone this repository, check out the branch ``master``,
         install the build dependencies, they're listed in the file
         ``debian/control`` and build the debian packages using::
         
           dpkg-buildpackage -rfakeroot
         
@@ -651,29 +655,68 @@
         debian, currently these are ``mpich``, ``openmpi``, and ``lam``. In addition
         to the MPI libraries a serial version of the pgapack library is also
         built. Proceed by installing the package pgapack and the MPI backend
         library of choice. If you don't have a preference for an MPI library,
         ``libpgapack-openmpi`` is the package that uses the Debians default
         preferences of an MPI library.
         
-        Once a parallel version of PGApack is installed, you can install PGApy
+        Once a parallel version of PGAPack_ is installed, you can install PGApy
         as follows: You set environment variables for the ``PGA_PARALLEL_VARIANT``
         (one of ``mpich``, ``openmpi``, or ``lam``) and set the ``PGA_MODULE`` to
         ``module_from_parallel_install``. Finally you envoke the setup, e.g.::
         
          export PGA_PARALLEL_VARIANT=openmpi
          export PGA_MODULE=module_from_parallel_install
          python3 setup.py install --prefix=/usr/local
         
+        Note that the same works with ``pip install``, i.e., after installation
+        of a parallel version of PGAPack_ you can directly install with ``pip``::
+        
+         export PGA_PARALLEL_VARIANT=openmpi
+         export PGA_MODULE=module_from_parallel_install
+         pip install pgapy
+        
+        or alternatively depending on how pip is installed on your system::
+        
+         python3 -m pip install pgapy
+        
         If your MPI library is installed in a different place you should study
         the *Extension* configurations in ``setup.py`` to come up with an
         Extension definition that fits your installation. If your installation
         is interesting to more people, feel free to submit a patch that adds
         your Extension-configuration to the standard ``setup.py``.
         
+        Running with MPI
+        ----------------
+        
+        To run a parallel version with MPI_, a parallel version must be
+        installed, see above in section Installation_.
+        
+        For a serial version, PGAPy makes sure that the otimization is aborted
+        if an exception occurs in the ``evaluate`` function. This is currently not
+        the case for MPI, because the framework currently does not support
+        returning information to the rank-0 MPI leader process. A workaround is
+        as follows: Rename your ``evaluate`` method to ``_evaluate`` and catch
+        exceptions in a new ``evaluate`` method that wraps ``_evaluate``.
+        Call ``MPI_Abort`` if an exception occurs::
+        
+            import traceback
+            import sys
+        
+            ...
+        
+            def evaluate (self, p, pop):
+                try:
+                    return self._evaluate (p, pop)
+                except Exception:
+                    # Optionally log exception here
+                    print (traceback.format_exc ())
+                    pga.MPI_Abort (1)
+                    sys.exit (1)
+        
         Testing
         -------
         
         For testing |--| preferrably before installation you can build locally::
         
             python3 setup.py build_ext --inplace
         
@@ -682,15 +725,15 @@
         
             python3 -m pytest test
         
         This runs all the tests and can take a while. Note that the tests run
         most of the examples in the ``examples`` directory with different
         command line parameters where available. To perform several optimization
         runs in a single (Python-) process, we must call ``MPI_Init``
-        *explicitly* (and not relying on PGAPack to call it implicitly). This is
+        *explicitly* (and not relying on PGAPack_ to call it implicitly). This is
         because ``MPI_Init`` may be called only once per process. Calling of
         ``MPI_Init`` and ``MPI_Finalize`` is handled in a fixture in
         ``test/conftest.py``
         
         Coverage
         ++++++++
         
@@ -811,17 +854,31 @@
                 method for generating the pareto surface in nonlinear multicriteria
                 optimization problems. SIAM Journal on Optimization, 8(3):631–657,
                 August 1998.
         
         Changes
         -------
         
+        Version 2.2.1: MPI_Abort
+        
+        - Add MPI_Abort to the wrapper
+        - Include ``mpi_stub.c`` in the release (this is missing if some env
+          variables are set, see above in Installation)
+        
+        Version 2.2: Module directory
+        
+        - Put the pga C-module inside a pga module
+        - Add several python-only modules to pga
+        - pga.__init__ exports everything to this is compatible
+        - pga.random includes a python Random class based on the pgapack random
+          number generator
+        
         Version 2.1: Regression test
         
-        - PGApack bug-fixes discovered during testing
+        - PGAPack bug-fixes discovered during testing
         - Bug-fixes of python wrapper
         - Lots of tests with coverage of wrapper C-code > 90%
         
         Version 2.0: User defined data types
         
         - Implement user defined data types, note that your data type can be
           variable-size, e.g., a tree data structure. The framework takes care
@@ -960,14 +1017,22 @@
         a powerful genetic algorithm library. PGAPy wraps this library for use
         with Python. Pgapack is one of the most complete and accurate genetic
         algorithm implementations out there with a lot of features for
         experimentation.
         
         - Initial Release
         
+        .. _`PGAPack Readme`:
+           https://github.com/schlatterbeck/pgapack/blob/master/README.rst
+        .. _PGAPack:          http://ftp.mcs.anl.gov/pub/pgapack/
+        .. _`PGAPack fork on github`: https://github.com/schlatterbeck/pgapack
+        .. _MPI: http://mpi-forum.org/
+        .. _`my pgapack debian package builder`:
+            https://github.com/schlatterbeck/debian-pgapack
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `PGAPy-2.2/PKG-INFO` & `PGAPy-2.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PGAPy
-Version: 2.2
+Version: 2.2.1
 Summary: Python wrapper for pgapack, the parallel genetic algorithm library
 Home-page: http://pgapy.sourceforge.net/
 Author: Ralf Schlatterbeck
 Author-email: rsc@runtux.com
 License: UNKNOWN
 Description: PGAPy: Python Wrapper for PGAPack Parallel Genetic Algorithm Library
         ====================================================================
@@ -13,14 +13,26 @@
         .. |epsilon| unicode:: U+03B5 .. epsilon
         
         :Author: Ralf Schlatterbeck <rsc@runtux.com>
         
         News
         ----
         
+        News 04-2023:
+        
+        - The last build on PyPi was broken for serial installs, it was missing
+          the ``mpi_stub.c`` needed for the serial version. Parallel installs
+          were still possible so I didn't notice, sorry!
+        - Add MPI_Abort to the wrapper, it is called with::
+        
+            pga.MPI_Abort (errcode)
+        
+          See below in secion `Running with MPI`_ how this can be used to abort
+          the MPI run in case of exception in the ``evaluate`` method.
+        
         News 12-2022: Add regression test and update to new upstream with
         several bug-fixes. Includes also some bug fixes in wrapper.
         
         News 10-2022: Add user defined datatypes. Example in ``examples/gp`` use
         user defined data types to implement genetic programming (we represent
         expressions by a tree data structure). This uses the new serialization
         API in pgapack to transfer a Python pickle representation to peer MPI
@@ -64,15 +76,15 @@
         experimentation. It also has shown a remarkably small number of bugs
         over the years. It supports parallel execution via the message
         passing interface MPI_ in addition to a normal "serial" version. That's
         why I wanted to use it in Python, too.
         
         To get started you need the PGAPack library, although
         it now comes bundled with PGApy, to install a *parallel* version you
-        currently need a pre-installed PGApack compiled for the MPI library of
+        currently need a pre-installed PGAPack_ compiled for the MPI library of
         choice. See `Installation`_ section for details.
         
         There currently is not much documentation for PGAPy.
         You really, absolutely need to read the documentation that comes
         with PGAPack.
         The PGAPack user guide is now shipped together with PGAPy. It is
         installed together with some examples in share/pgapy, wherever the
@@ -122,22 +134,14 @@
         As mentioned above, you can find my `PGAPack fork on github`_, this
         repository has the three upstream releases as versions in git and
         contains some updates concerning support of newer MPI_ versions and
         documentation updates.  I've also included patches in the git repository
         of the Debian maintainer of the package, Dirk Eddelbuettel.
         I'm actively maintaining that branch, adding new features and bug-fixes.
         
-        .. _`PGAPack Readme`:
-           https://github.com/schlatterbeck/pgapack/blob/master/README.rst
-        .. _PGAPack:          http://ftp.mcs.anl.gov/pub/pgapack/
-        .. _`PGAPack fork on github`: https://github.com/schlatterbeck/pgapack
-        .. _MPI: http://mpi-forum.org/
-        .. _`my pgapack debian package builder`:
-            https://github.com/schlatterbeck/debian-pgapack
-        
         To get you started, I've included some very simple examples in
         ``examples``, e.g., ``one-max.py`` implements the "Maxbit" example
         similar to one in the PGAPack documentation. The examples were inspired
         by the book "Genetic Algorithms in Python" but are written from scratch
         and don't include any code from the book. The examples illustrates
         several points:
         
@@ -204,43 +208,43 @@
           ``check_stopping_conditions``. An exception of the lowercase-rule is
           whenever a name contains "GA" (for "genetic algorithm"), So
           ``PGASetMaxGAIterValue`` becomes ``max_GA_iter``.
         - Where possible I've made a single class method where PGAPack needs a
           separate function for each datatype, so ``PGAGetBinaryAllele``,
           ``PGAGetCharacterAllele``, ``PGAGetIntegerAllele``, ``PGAGetRealAllele`` all
           become ``get_allele``. Same holds true for ``set_allele``.
-        - Whenever a name in PGApack has a "Value" or "Flag" suffix, I've left
+        - Whenever a name in PGAPack has a "Value" or "Flag" suffix, I've left
           this out, so ``PGAGetFitnessCmaxValue`` becomes ``fitness_cmax``
           and ``PGAGetMutationAndCrossoverFlag`` becomes
           ``mutation_and_crossover``, the only exception to this rule is for the
           two functions ``PGAGetMutationRealValue`` and
           ``PGAGetMutationIntegerValue`` which become ``mutation_value`` not
           just ``mutation``.
         - Some fields can take multiple values (they are implemented by ORing
           integer constants, in python they are specified as a list or tuple of
           constants). These are converted to plural (if not already plural in
-          PGApack), e.g., ``PGASetStoppingRuleType`` becomes ``stopping_rule_types``.
+          PGAPack), e.g., ``PGASetStoppingRuleType`` becomes ``stopping_rule_types``.
         - Internal method names in the wrapper program have a leading PGA\_ |--| so
           the class method ``set_allele`` is implemented by the C-function
           ``PGA_set_allele`` in ``pgamodule.c``.
         
         Constructor Parameters
         ----------------------
         
-        PGApack has a lot of ``PGASet`` and ``PGAGet`` functions for setting
+        PGAPack_ has a lot of ``PGASet`` and ``PGAGet`` functions for setting
         parameters. These are reflected in constructor parameters on the one hand
         and in (typically read-only, but see below) properties of a ``PGA``
         object on the other hand. The
-        following table gives an overview of all the original PGApack names and
-        the names of the python wrapper. For the PGApack name I've only listed
+        following table gives an overview of all the original PGAPack_ names and
+        the names of the python wrapper. For the PGAPack_ name I've only listed
         the ``PGASet`` function, in many cases there is a corresponding
         ``PGAGet`` function. If a corresponding read-only property exists for a
         constructor parameter this is indicated in the "Prop" column. In some
         cases properties are missing because no corresponding ``PGAGet`` function
-        is implemented in PGApack, in other cases returning a numeric value that
+        is implemented in PGAPack_, in other cases returning a numeric value that
         has a symbolic constant in PGApy doesn't make much sense.
         
         The properties have the same name as the constructor parameter.
         There are Properties that don't have a corresponding constructor
         parameter, namely the ``eval_count`` property (returning the count of
         function evaluations), the
         ``GA_iter`` property that returns the current GA generation, and the
@@ -258,15 +262,15 @@
         allele* of the gene. In python this is a sequence of 2-tuples.
         Note that this means that you can have different ranges of allowed values
         for each allele.
         
         The ``num_eval`` property is special: Due to limitations of the C
         programming language, for multiple evaluations in C the first evaluation
         is returned as the function return-value of the ``evaluate`` function
-        and all other parameters are returned in an auxiliary array. PGApack
+        and all other parameters are returned in an auxiliary array. PGAPack_
         specifies the number of auxiliary evaluations to be returned. In Python
         the evaluation function can always return a sequence of evaluation
         values and the ``num_eval`` is one more than ``PGAGetNumAuxEval`` would
         return. The default for ``num_eval`` is 1.
         
         The first two (mandatory) constructor parameters are the type of the gene
         (this takes a Python type, e.g., ``bool`` for a binary genome or ``int``
@@ -278,15 +282,15 @@
         Some properties can now also be set *during* the run of the optimizer.
         These currently are ``crossover_prob``, ``epsilon_exponent``,
         ``multi_obj_precision``, ``p_tournament_prob``, and
         ``uniform_crossover_prob``. Just assign to the member variable of
         the optimizer (child of PGA.pga) object.
         
         ==================================== ================================= ====== ====
-        PGApack name                         Constructor parameter             Type   Prop
+        PGAPack name                         Constructor parameter             Type   Prop
         ==================================== ================================= ====== ====
         ``PGASetCrossoverBoundedFlag``       ``crossover_bounded``             int    yes
         ``PGASetCrossoverBounceBackFlag``    ``crossover_bounce_back``         int    yes
         ``PGASetCrossoverSBXEta``            ``crossover_SBX_eta``             float  yes
         ``PGASetCrossoverSBXOncePerString``  ``crossover_SBX_once_per_string`` int    yes
         ``PGASetCrossoverProb``              ``crossover_prob``                float  yes
         ``PGASetCrossoverType``              ``crossover_type``                sym    no
@@ -424,32 +428,32 @@
         ``set_gene``                  *p, pop, gen*      set gene (user data types)
         ``set_random_seed``           *seed*             None (use constructor!)
         ============================= ================== ===========================
         
         User-Methods
         ------------
         
-        PGApack has the concept of user functions. These allow customization of
+        PGAPack_ has the concept of user functions. These allow customization of
         different areas of a genetic algorihm. In Python they are implemented as
         methods that can be changed in a derived class. One of the methods that
         *must* be implemented in a derived class is the ``evaluate`` function
-        (although technically it is not a user function in PGApack). It
+        (although technically it is not a user function in PGAPack). It
         interprets the gene and returns an evaluation value or a sequence of
         evaluation values if you set the ``num_eval`` constructor parameter.
-        PGApack computes a fitness from the raw evaluation value. For some
+        PGAPack_ computes a fitness from the raw evaluation value. For some
         methods an up-call into the PGA class is possible, for some methods this
         is not possible (and in most cases not reasonable). Note that for the
         ``stop_cond`` method, the standard check for stopping conditions can be
         called with::
         
           self.check_stopping_conditions()
         
         The following table lists the overridable methods with their parameters
         (for the function signature the first parameter *self* is omitted). Note
-        that in PGApack there are additional user functions that are needed for
+        that in PGAPack_ there are additional user functions that are needed for
         user-defined data types which are currently not exposed in Python. In the
         function signatures *p* denotes the index of the individual and *pop*
         denotes the population. If more than one individual is specified (e.g.,
         for crossover) these can be followed by a number. For crossover *c1* and
         *c2* denote the destination individuals (children). The *propability* for
         the mutation method is a floating-point value between 0 and 1. Remember
         to count the number of mutations that happen, and return that value for
@@ -470,15 +474,15 @@
         ``pre_eval``        *pop*                          None              no
         ``print_string``    *file, p, pop*                 None              yes
         =================== ============================== ================= =======
         
         Constants
         ---------
         
-        The following PGApack constants are available:
+        The following PGAPack_ constants are available:
         
         ========================== ===========================================
         Constant                   Description
         ========================== ===========================================
         PGA_CROSSOVER_EDGE         Edge crossover for permutations
         PGA_CROSSOVER_ONEPT        One-point Crossover
         PGA_CROSSOVER_SBX          Simulated Binary Crossover
@@ -586,15 +590,15 @@
         over the serialization of the tree (which is the same for individuals
         with the same tree structure).
         
         
         Missing Features
         ----------------
         
-        As already mentioned, not all functions and constants of PGAPack are
+        As already mentioned, not all functions and constants of PGAPack_ are
         wrapped yet |--| still for many applications the given set should be
         enough. If you need additional functions, you may want to wrap these and
         send_ me a patch.
         
         Reporting Bugs
         --------------
         
@@ -635,15 +639,15 @@
         To install a *serial* version (without parallel programming using MPI_)
         you can simply install from pypi using ``pip``. Alternatively when you
         have unpacked or checked out from sources you can install with::
         
          python3 setup.py install --prefix=/usr/local
         
         If you want a parallel version using an MPI_ (Message-Passing Interface)
-        library you will have to install a parallel version of PGApack first.
+        library you will have to install a parallel version of PGAPack_ first.
         The easiest way to do this is to use `my pgapack debian package builder`_
         from github. Clone this repository, check out the branch ``master``,
         install the build dependencies, they're listed in the file
         ``debian/control`` and build the debian packages using::
         
           dpkg-buildpackage -rfakeroot
         
@@ -651,29 +655,68 @@
         debian, currently these are ``mpich``, ``openmpi``, and ``lam``. In addition
         to the MPI libraries a serial version of the pgapack library is also
         built. Proceed by installing the package pgapack and the MPI backend
         library of choice. If you don't have a preference for an MPI library,
         ``libpgapack-openmpi`` is the package that uses the Debians default
         preferences of an MPI library.
         
-        Once a parallel version of PGApack is installed, you can install PGApy
+        Once a parallel version of PGAPack_ is installed, you can install PGApy
         as follows: You set environment variables for the ``PGA_PARALLEL_VARIANT``
         (one of ``mpich``, ``openmpi``, or ``lam``) and set the ``PGA_MODULE`` to
         ``module_from_parallel_install``. Finally you envoke the setup, e.g.::
         
          export PGA_PARALLEL_VARIANT=openmpi
          export PGA_MODULE=module_from_parallel_install
          python3 setup.py install --prefix=/usr/local
         
+        Note that the same works with ``pip install``, i.e., after installation
+        of a parallel version of PGAPack_ you can directly install with ``pip``::
+        
+         export PGA_PARALLEL_VARIANT=openmpi
+         export PGA_MODULE=module_from_parallel_install
+         pip install pgapy
+        
+        or alternatively depending on how pip is installed on your system::
+        
+         python3 -m pip install pgapy
+        
         If your MPI library is installed in a different place you should study
         the *Extension* configurations in ``setup.py`` to come up with an
         Extension definition that fits your installation. If your installation
         is interesting to more people, feel free to submit a patch that adds
         your Extension-configuration to the standard ``setup.py``.
         
+        Running with MPI
+        ----------------
+        
+        To run a parallel version with MPI_, a parallel version must be
+        installed, see above in section Installation_.
+        
+        For a serial version, PGAPy makes sure that the otimization is aborted
+        if an exception occurs in the ``evaluate`` function. This is currently not
+        the case for MPI, because the framework currently does not support
+        returning information to the rank-0 MPI leader process. A workaround is
+        as follows: Rename your ``evaluate`` method to ``_evaluate`` and catch
+        exceptions in a new ``evaluate`` method that wraps ``_evaluate``.
+        Call ``MPI_Abort`` if an exception occurs::
+        
+            import traceback
+            import sys
+        
+            ...
+        
+            def evaluate (self, p, pop):
+                try:
+                    return self._evaluate (p, pop)
+                except Exception:
+                    # Optionally log exception here
+                    print (traceback.format_exc ())
+                    pga.MPI_Abort (1)
+                    sys.exit (1)
+        
         Testing
         -------
         
         For testing |--| preferrably before installation you can build locally::
         
             python3 setup.py build_ext --inplace
         
@@ -682,15 +725,15 @@
         
             python3 -m pytest test
         
         This runs all the tests and can take a while. Note that the tests run
         most of the examples in the ``examples`` directory with different
         command line parameters where available. To perform several optimization
         runs in a single (Python-) process, we must call ``MPI_Init``
-        *explicitly* (and not relying on PGAPack to call it implicitly). This is
+        *explicitly* (and not relying on PGAPack_ to call it implicitly). This is
         because ``MPI_Init`` may be called only once per process. Calling of
         ``MPI_Init`` and ``MPI_Finalize`` is handled in a fixture in
         ``test/conftest.py``
         
         Coverage
         ++++++++
         
@@ -811,17 +854,31 @@
                 method for generating the pareto surface in nonlinear multicriteria
                 optimization problems. SIAM Journal on Optimization, 8(3):631–657,
                 August 1998.
         
         Changes
         -------
         
+        Version 2.2.1: MPI_Abort
+        
+        - Add MPI_Abort to the wrapper
+        - Include ``mpi_stub.c`` in the release (this is missing if some env
+          variables are set, see above in Installation)
+        
+        Version 2.2: Module directory
+        
+        - Put the pga C-module inside a pga module
+        - Add several python-only modules to pga
+        - pga.__init__ exports everything to this is compatible
+        - pga.random includes a python Random class based on the pgapack random
+          number generator
+        
         Version 2.1: Regression test
         
-        - PGApack bug-fixes discovered during testing
+        - PGAPack bug-fixes discovered during testing
         - Bug-fixes of python wrapper
         - Lots of tests with coverage of wrapper C-code > 90%
         
         Version 2.0: User defined data types
         
         - Implement user defined data types, note that your data type can be
           variable-size, e.g., a tree data structure. The framework takes care
@@ -960,14 +1017,22 @@
         a powerful genetic algorithm library. PGAPy wraps this library for use
         with Python. Pgapack is one of the most complete and accurate genetic
         algorithm implementations out there with a lot of features for
         experimentation.
         
         - Initial Release
         
+        .. _`PGAPack Readme`:
+           https://github.com/schlatterbeck/pgapack/blob/master/README.rst
+        .. _PGAPack:          http://ftp.mcs.anl.gov/pub/pgapack/
+        .. _`PGAPack fork on github`: https://github.com/schlatterbeck/pgapack
+        .. _MPI: http://mpi-forum.org/
+        .. _`my pgapack debian package builder`:
+            https://github.com/schlatterbeck/debian-pgapack
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `PGAPy-2.2/README.html` & `PGAPy-2.2.1/README.html`

 * *Files 2% similar despite different names*

```diff
@@ -285,14 +285,28 @@
 <tbody valign="top">
 <tr><th class="docinfo-name">Author:</th>
 <td>Ralf Schlatterbeck &lt;<a class="reference external" href="mailto:rsc&#64;runtux.com">rsc&#64;runtux.com</a>&gt;</td></tr>
 </tbody>
 </table>
 <div class="section" id="news">
 <h1>News</h1>
+<p>News 04-2023:</p>
+<ul>
+<li><p class="first">The last build on PyPi was broken for serial installs, it was missing
+the <tt class="docutils literal">mpi_stub.c</tt> needed for the serial version. Parallel installs
+were still possible so I didn't notice, sorry!</p>
+</li>
+<li><p class="first">Add MPI_Abort to the wrapper, it is called with:</p>
+<pre class="literal-block">
+pga.MPI_Abort (errcode)
+</pre>
+<p>See below in secion <a class="reference internal" href="#running-with-mpi">Running with MPI</a> how this can be used to abort
+the MPI run in case of exception in the <tt class="docutils literal">evaluate</tt> method.</p>
+</li>
+</ul>
 <p>News 12-2022: Add regression test and update to new upstream with
 several bug-fixes. Includes also some bug fixes in wrapper.</p>
 <p>News 10-2022: Add user defined datatypes. Example in <tt class="docutils literal">examples/gp</tt> use
 user defined data types to implement genetic programming (we represent
 expressions by a tree data structure). This uses the new serialization
 API in pgapack to transfer a Python pickle representation to peer MPI
 processes. Also incorporate the latest changes in pgapack which
@@ -328,15 +342,15 @@
 implementations out there with a lot of bells and whistles for
 experimentation. It also has shown a remarkably small number of bugs
 over the years. It supports parallel execution via the message
 passing interface <a class="reference external" href="http://mpi-forum.org/">MPI</a> in addition to a normal &quot;serial&quot; version. That's
 why I wanted to use it in Python, too.</p>
 <p>To get started you need the PGAPack library, although
 it now comes bundled with PGApy, to install a <em>parallel</em> version you
-currently need a pre-installed PGApack compiled for the MPI library of
+currently need a pre-installed <a class="reference external" href="http://ftp.mcs.anl.gov/pub/pgapack/">PGAPack</a> compiled for the MPI library of
 choice. See <a class="reference internal" href="#installation">Installation</a> section for details.</p>
 <p>There currently is not much documentation for PGAPy.
 You really, absolutely need to read the documentation that comes
 with PGAPack.
 The PGAPack user guide is now shipped together with PGAPy. It is
 installed together with some examples in share/pgapy, wherever the
 Python installer decides to place this in the final installation
@@ -455,43 +469,43 @@
 <tt class="docutils literal">check_stopping_conditions</tt>. An exception of the lowercase-rule is
 whenever a name contains &quot;GA&quot; (for &quot;genetic algorithm&quot;), So
 <tt class="docutils literal">PGASetMaxGAIterValue</tt> becomes <tt class="docutils literal">max_GA_iter</tt>.</li>
 <li>Where possible I've made a single class method where PGAPack needs a
 separate function for each datatype, so <tt class="docutils literal">PGAGetBinaryAllele</tt>,
 <tt class="docutils literal">PGAGetCharacterAllele</tt>, <tt class="docutils literal">PGAGetIntegerAllele</tt>, <tt class="docutils literal">PGAGetRealAllele</tt> all
 become <tt class="docutils literal">get_allele</tt>. Same holds true for <tt class="docutils literal">set_allele</tt>.</li>
-<li>Whenever a name in PGApack has a &quot;Value&quot; or &quot;Flag&quot; suffix, I've left
+<li>Whenever a name in PGAPack has a &quot;Value&quot; or &quot;Flag&quot; suffix, I've left
 this out, so <tt class="docutils literal">PGAGetFitnessCmaxValue</tt> becomes <tt class="docutils literal">fitness_cmax</tt>
 and <tt class="docutils literal">PGAGetMutationAndCrossoverFlag</tt> becomes
 <tt class="docutils literal">mutation_and_crossover</tt>, the only exception to this rule is for the
 two functions <tt class="docutils literal">PGAGetMutationRealValue</tt> and
 <tt class="docutils literal">PGAGetMutationIntegerValue</tt> which become <tt class="docutils literal">mutation_value</tt> not
 just <tt class="docutils literal">mutation</tt>.</li>
 <li>Some fields can take multiple values (they are implemented by ORing
 integer constants, in python they are specified as a list or tuple of
 constants). These are converted to plural (if not already plural in
-PGApack), e.g., <tt class="docutils literal">PGASetStoppingRuleType</tt> becomes <tt class="docutils literal">stopping_rule_types</tt>.</li>
+PGAPack), e.g., <tt class="docutils literal">PGASetStoppingRuleType</tt> becomes <tt class="docutils literal">stopping_rule_types</tt>.</li>
 <li>Internal method names in the wrapper program have a leading PGA_ – so
 the class method <tt class="docutils literal">set_allele</tt> is implemented by the C-function
 <tt class="docutils literal">PGA_set_allele</tt> in <tt class="docutils literal">pgamodule.c</tt>.</li>
 </ul>
 </div>
 <div class="section" id="constructor-parameters">
 <h1>Constructor Parameters</h1>
-<p>PGApack has a lot of <tt class="docutils literal">PGASet</tt> and <tt class="docutils literal">PGAGet</tt> functions for setting
+<p><a class="reference external" href="http://ftp.mcs.anl.gov/pub/pgapack/">PGAPack</a> has a lot of <tt class="docutils literal">PGASet</tt> and <tt class="docutils literal">PGAGet</tt> functions for setting
 parameters. These are reflected in constructor parameters on the one hand
 and in (typically read-only, but see below) properties of a <tt class="docutils literal">PGA</tt>
 object on the other hand. The
-following table gives an overview of all the original PGApack names and
-the names of the python wrapper. For the PGApack name I've only listed
+following table gives an overview of all the original <a class="reference external" href="http://ftp.mcs.anl.gov/pub/pgapack/">PGAPack</a> names and
+the names of the python wrapper. For the <a class="reference external" href="http://ftp.mcs.anl.gov/pub/pgapack/">PGAPack</a> name I've only listed
 the <tt class="docutils literal">PGASet</tt> function, in many cases there is a corresponding
 <tt class="docutils literal">PGAGet</tt> function. If a corresponding read-only property exists for a
 constructor parameter this is indicated in the &quot;Prop&quot; column. In some
 cases properties are missing because no corresponding <tt class="docutils literal">PGAGet</tt> function
-is implemented in PGApack, in other cases returning a numeric value that
+is implemented in <a class="reference external" href="http://ftp.mcs.anl.gov/pub/pgapack/">PGAPack</a>, in other cases returning a numeric value that
 has a symbolic constant in PGApy doesn't make much sense.</p>
 <p>The properties have the same name as the constructor parameter.
 There are Properties that don't have a corresponding constructor
 parameter, namely the <tt class="docutils literal">eval_count</tt> property (returning the count of
 function evaluations), the
 <tt class="docutils literal">GA_iter</tt> property that returns the current GA generation, and the
 <tt class="docutils literal">mpi_rank</tt> property that returns the MPI rank of the current process
@@ -506,15 +520,15 @@
 <tt class="docutils literal">PGASetIntegerInitRange</tt> functions. These take two values for <em>each
 allele</em> of the gene. In python this is a sequence of 2-tuples.
 Note that this means that you can have different ranges of allowed values
 for each allele.</p>
 <p>The <tt class="docutils literal">num_eval</tt> property is special: Due to limitations of the C
 programming language, for multiple evaluations in C the first evaluation
 is returned as the function return-value of the <tt class="docutils literal">evaluate</tt> function
-and all other parameters are returned in an auxiliary array. PGApack
+and all other parameters are returned in an auxiliary array. <a class="reference external" href="http://ftp.mcs.anl.gov/pub/pgapack/">PGAPack</a>
 specifies the number of auxiliary evaluations to be returned. In Python
 the evaluation function can always return a sequence of evaluation
 values and the <tt class="docutils literal">num_eval</tt> is one more than <tt class="docutils literal">PGAGetNumAuxEval</tt> would
 return. The default for <tt class="docutils literal">num_eval</tt> is 1.</p>
 <p>The first two (mandatory) constructor parameters are the type of the gene
 (this takes a Python type, e.g., <tt class="docutils literal">bool</tt> for a binary genome or <tt class="docutils literal">int</tt>
 for an integer genome) and the length. Note that the <tt class="docutils literal">string_length</tt> is
@@ -530,15 +544,15 @@
 <colgroup>
 <col width="46%" />
 <col width="42%" />
 <col width="8%" />
 <col width="5%" />
 </colgroup>
 <thead valign="bottom">
-<tr><th class="head">PGApack name</th>
+<tr><th class="head">PGAPack name</th>
 <th class="head">Constructor parameter</th>
 <th class="head">Type</th>
 <th class="head">Prop</th>
 </tr>
 </thead>
 <tbody valign="top">
 <tr><td><tt class="docutils literal">PGASetCrossoverBoundedFlag</tt></td>
@@ -1074,32 +1088,32 @@
 <td>None (use constructor!)</td>
 </tr>
 </tbody>
 </table>
 </div>
 <div class="section" id="user-methods">
 <h1>User-Methods</h1>
-<p>PGApack has the concept of user functions. These allow customization of
+<p><a class="reference external" href="http://ftp.mcs.anl.gov/pub/pgapack/">PGAPack</a> has the concept of user functions. These allow customization of
 different areas of a genetic algorihm. In Python they are implemented as
 methods that can be changed in a derived class. One of the methods that
 <em>must</em> be implemented in a derived class is the <tt class="docutils literal">evaluate</tt> function
-(although technically it is not a user function in PGApack). It
+(although technically it is not a user function in PGAPack). It
 interprets the gene and returns an evaluation value or a sequence of
 evaluation values if you set the <tt class="docutils literal">num_eval</tt> constructor parameter.
-PGApack computes a fitness from the raw evaluation value. For some
+<a class="reference external" href="http://ftp.mcs.anl.gov/pub/pgapack/">PGAPack</a> computes a fitness from the raw evaluation value. For some
 methods an up-call into the PGA class is possible, for some methods this
 is not possible (and in most cases not reasonable). Note that for the
 <tt class="docutils literal">stop_cond</tt> method, the standard check for stopping conditions can be
 called with:</p>
 <pre class="literal-block">
 self.check_stopping_conditions()
 </pre>
 <p>The following table lists the overridable methods with their parameters
 (for the function signature the first parameter <em>self</em> is omitted). Note
-that in PGApack there are additional user functions that are needed for
+that in <a class="reference external" href="http://ftp.mcs.anl.gov/pub/pgapack/">PGAPack</a> there are additional user functions that are needed for
 user-defined data types which are currently not exposed in Python. In the
 function signatures <em>p</em> denotes the index of the individual and <em>pop</em>
 denotes the population. If more than one individual is specified (e.g.,
 for crossover) these can be followed by a number. For crossover <em>c1</em> and
 <em>c2</em> denote the destination individuals (children). The <em>propability</em> for
 the mutation method is a floating-point value between 0 and 1. Remember
 to count the number of mutations that happen, and return that value for
@@ -1175,15 +1189,15 @@
 <td>yes</td>
 </tr>
 </tbody>
 </table>
 </div>
 <div class="section" id="constants">
 <h1>Constants</h1>
-<p>The following PGApack constants are available:</p>
+<p>The following <a class="reference external" href="http://ftp.mcs.anl.gov/pub/pgapack/">PGAPack</a> constants are available:</p>
 <table border="1" class="docutils">
 <colgroup>
 <col width="34%" />
 <col width="66%" />
 </colgroup>
 <thead valign="bottom">
 <tr><th class="head">Constant</th>
@@ -1371,15 +1385,15 @@
 implements Genetic Programming with a tree data structure. Note that the
 <tt class="docutils literal">Node</tt> class in <tt class="docutils literal">gp.py</tt> has a <tt class="docutils literal">__hash__</tt> method that builds a hash
 over the serialization of the tree (which is the same for individuals
 with the same tree structure).</p>
 </div>
 <div class="section" id="missing-features">
 <h1>Missing Features</h1>
-<p>As already mentioned, not all functions and constants of PGAPack are
+<p>As already mentioned, not all functions and constants of <a class="reference external" href="http://ftp.mcs.anl.gov/pub/pgapack/">PGAPack</a> are
 wrapped yet – still for many applications the given set should be
 enough. If you need additional functions, you may want to wrap these and
 <a class="reference external" href="mailto:rsc&#64;runtux.com">send</a> me a patch.</p>
 </div>
 <div class="section" id="reporting-bugs">
 <h1>Reporting Bugs</h1>
 <p>Please use the <a class="reference external" href="http://sourceforge.net/tracker/?group_id=152022&amp;atid=782852">Sourceforge Bug Tracker</a>  or the <a class="reference external" href="https://github.com/schlatterbeck/pgapy/issues">Github Bug Tracker</a> and</p>
@@ -1405,44 +1419,82 @@
 <p>To install a <em>serial</em> version (without parallel programming using <a class="reference external" href="http://mpi-forum.org/">MPI</a>)
 you can simply install from pypi using <tt class="docutils literal">pip</tt>. Alternatively when you
 have unpacked or checked out from sources you can install with:</p>
 <pre class="literal-block">
 python3 setup.py install --prefix=/usr/local
 </pre>
 <p>If you want a parallel version using an <a class="reference external" href="http://mpi-forum.org/">MPI</a> (Message-Passing Interface)
-library you will have to install a parallel version of PGApack first.
+library you will have to install a parallel version of <a class="reference external" href="http://ftp.mcs.anl.gov/pub/pgapack/">PGAPack</a> first.
 The easiest way to do this is to use <a class="reference external" href="https://github.com/schlatterbeck/debian-pgapack">my pgapack debian package builder</a>
 from github. Clone this repository, check out the branch <tt class="docutils literal">master</tt>,
 install the build dependencies, they're listed in the file
 <tt class="docutils literal">debian/control</tt> and build the debian packages using:</p>
 <pre class="literal-block">
 dpkg-buildpackage -rfakeroot
 </pre>
 <p>This builds pgapack debian packages for <em>all</em> supported MPI libraries in
 debian, currently these are <tt class="docutils literal">mpich</tt>, <tt class="docutils literal">openmpi</tt>, and <tt class="docutils literal">lam</tt>. In addition
 to the MPI libraries a serial version of the pgapack library is also
 built. Proceed by installing the package pgapack and the MPI backend
 library of choice. If you don't have a preference for an MPI library,
 <tt class="docutils literal"><span class="pre">libpgapack-openmpi</span></tt> is the package that uses the Debians default
 preferences of an MPI library.</p>
-<p>Once a parallel version of PGApack is installed, you can install PGApy
+<p>Once a parallel version of <a class="reference external" href="http://ftp.mcs.anl.gov/pub/pgapack/">PGAPack</a> is installed, you can install PGApy
 as follows: You set environment variables for the <tt class="docutils literal">PGA_PARALLEL_VARIANT</tt>
 (one of <tt class="docutils literal">mpich</tt>, <tt class="docutils literal">openmpi</tt>, or <tt class="docutils literal">lam</tt>) and set the <tt class="docutils literal">PGA_MODULE</tt> to
 <tt class="docutils literal">module_from_parallel_install</tt>. Finally you envoke the setup, e.g.:</p>
 <pre class="literal-block">
 export PGA_PARALLEL_VARIANT=openmpi
 export PGA_MODULE=module_from_parallel_install
 python3 setup.py install --prefix=/usr/local
 </pre>
+<p>Note that the same works with <tt class="docutils literal">pip install</tt>, i.e., after installation
+of a parallel version of <a class="reference external" href="http://ftp.mcs.anl.gov/pub/pgapack/">PGAPack</a> you can directly install with <tt class="docutils literal">pip</tt>:</p>
+<pre class="literal-block">
+export PGA_PARALLEL_VARIANT=openmpi
+export PGA_MODULE=module_from_parallel_install
+pip install pgapy
+</pre>
+<p>or alternatively depending on how pip is installed on your system:</p>
+<pre class="literal-block">
+python3 -m pip install pgapy
+</pre>
 <p>If your MPI library is installed in a different place you should study
 the <em>Extension</em> configurations in <tt class="docutils literal">setup.py</tt> to come up with an
 Extension definition that fits your installation. If your installation
 is interesting to more people, feel free to submit a patch that adds
 your Extension-configuration to the standard <tt class="docutils literal">setup.py</tt>.</p>
 </div>
+<div class="section" id="running-with-mpi">
+<h1>Running with MPI</h1>
+<p>To run a parallel version with <a class="reference external" href="http://mpi-forum.org/">MPI</a>, a parallel version must be
+installed, see above in section <a class="reference internal" href="#installation">Installation</a>.</p>
+<p>For a serial version, PGAPy makes sure that the otimization is aborted
+if an exception occurs in the <tt class="docutils literal">evaluate</tt> function. This is currently not
+the case for MPI, because the framework currently does not support
+returning information to the rank-0 MPI leader process. A workaround is
+as follows: Rename your <tt class="docutils literal">evaluate</tt> method to <tt class="docutils literal">_evaluate</tt> and catch
+exceptions in a new <tt class="docutils literal">evaluate</tt> method that wraps <tt class="docutils literal">_evaluate</tt>.
+Call <tt class="docutils literal">MPI_Abort</tt> if an exception occurs:</p>
+<pre class="literal-block">
+import traceback
+import sys
+
+...
+
+def evaluate (self, p, pop):
+    try:
+        return self._evaluate (p, pop)
+    except Exception:
+        # Optionally log exception here
+        print (traceback.format_exc ())
+        pga.MPI_Abort (1)
+        sys.exit (1)
+</pre>
+</div>
 <div class="section" id="testing">
 <h1>Testing</h1>
 <p>For testing – preferrably before installation you can build locally:</p>
 <pre class="literal-block">
 python3 setup.py build_ext --inplace
 </pre>
 <p>After this you have a <tt class="docutils literal"><span class="pre">pga.*.so</span></tt> file in the local directory. Now you
@@ -1450,15 +1502,15 @@
 <pre class="literal-block">
 python3 -m pytest test
 </pre>
 <p>This runs all the tests and can take a while. Note that the tests run
 most of the examples in the <tt class="docutils literal">examples</tt> directory with different
 command line parameters where available. To perform several optimization
 runs in a single (Python-) process, we must call <tt class="docutils literal">MPI_Init</tt>
-<em>explicitly</em> (and not relying on PGAPack to call it implicitly). This is
+<em>explicitly</em> (and not relying on <a class="reference external" href="http://ftp.mcs.anl.gov/pub/pgapack/">PGAPack</a> to call it implicitly). This is
 because <tt class="docutils literal">MPI_Init</tt> may be called only once per process. Calling of
 <tt class="docutils literal">MPI_Init</tt> and <tt class="docutils literal">MPI_Finalize</tt> is handled in a fixture in
 <tt class="docutils literal">test/conftest.py</tt></p>
 <div class="section" id="coverage">
 <h2>Coverage</h2>
 <p>For the python examples, the coverage can be computed with:</p>
 <pre class="literal-block">
@@ -1631,17 +1683,31 @@
 optimization problems. SIAM Journal on Optimization, 8(3):631–657,
 August 1998.</td></tr>
 </tbody>
 </table>
 </div>
 <div class="section" id="changes">
 <h1>Changes</h1>
+<p>Version 2.2.1: MPI_Abort</p>
+<ul class="simple">
+<li>Add MPI_Abort to the wrapper</li>
+<li>Include <tt class="docutils literal">mpi_stub.c</tt> in the release (this is missing if some env
+variables are set, see above in Installation)</li>
+</ul>
+<p>Version 2.2: Module directory</p>
+<ul class="simple">
+<li>Put the pga C-module inside a pga module</li>
+<li>Add several python-only modules to pga</li>
+<li>pga.__init__ exports everything to this is compatible</li>
+<li>pga.random includes a python Random class based on the pgapack random
+number generator</li>
+</ul>
 <p>Version 2.1: Regression test</p>
 <ul class="simple">
-<li>PGApack bug-fixes discovered during testing</li>
+<li>PGAPack bug-fixes discovered during testing</li>
 <li>Bug-fixes of python wrapper</li>
 <li>Lots of tests with coverage of wrapper C-code &gt; 90%</li>
 </ul>
 <p>Version 2.0: User defined data types</p>
 <ul class="simple">
 <li>Implement user defined data types, note that your data type can be
 variable-size, e.g., a tree data structure. The framework takes care
```

### Comparing `PGAPy-2.2/README.rst` & `PGAPy-2.2.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,26 @@
 .. |epsilon| unicode:: U+03B5 .. epsilon
 
 :Author: Ralf Schlatterbeck <rsc@runtux.com>
 
 News
 ----
 
+News 04-2023:
+
+- The last build on PyPi was broken for serial installs, it was missing
+  the ``mpi_stub.c`` needed for the serial version. Parallel installs
+  were still possible so I didn't notice, sorry!
+- Add MPI_Abort to the wrapper, it is called with::
+
+    pga.MPI_Abort (errcode)
+
+  See below in secion `Running with MPI`_ how this can be used to abort
+  the MPI run in case of exception in the ``evaluate`` method.
+
 News 12-2022: Add regression test and update to new upstream with
 several bug-fixes. Includes also some bug fixes in wrapper.
 
 News 10-2022: Add user defined datatypes. Example in ``examples/gp`` use
 user defined data types to implement genetic programming (we represent
 expressions by a tree data structure). This uses the new serialization
 API in pgapack to transfer a Python pickle representation to peer MPI
@@ -56,15 +68,15 @@
 experimentation. It also has shown a remarkably small number of bugs
 over the years. It supports parallel execution via the message
 passing interface MPI_ in addition to a normal "serial" version. That's
 why I wanted to use it in Python, too.
 
 To get started you need the PGAPack library, although
 it now comes bundled with PGApy, to install a *parallel* version you
-currently need a pre-installed PGApack compiled for the MPI library of
+currently need a pre-installed PGAPack_ compiled for the MPI library of
 choice. See `Installation`_ section for details.
 
 There currently is not much documentation for PGAPy.
 You really, absolutely need to read the documentation that comes
 with PGAPack.
 The PGAPack user guide is now shipped together with PGAPy. It is
 installed together with some examples in share/pgapy, wherever the
@@ -114,22 +126,14 @@
 As mentioned above, you can find my `PGAPack fork on github`_, this
 repository has the three upstream releases as versions in git and
 contains some updates concerning support of newer MPI_ versions and
 documentation updates.  I've also included patches in the git repository
 of the Debian maintainer of the package, Dirk Eddelbuettel.
 I'm actively maintaining that branch, adding new features and bug-fixes.
 
-.. _`PGAPack Readme`:
-   https://github.com/schlatterbeck/pgapack/blob/master/README.rst
-.. _PGAPack:          http://ftp.mcs.anl.gov/pub/pgapack/
-.. _`PGAPack fork on github`: https://github.com/schlatterbeck/pgapack
-.. _MPI: http://mpi-forum.org/
-.. _`my pgapack debian package builder`:
-    https://github.com/schlatterbeck/debian-pgapack
-
 To get you started, I've included some very simple examples in
 ``examples``, e.g., ``one-max.py`` implements the "Maxbit" example
 similar to one in the PGAPack documentation. The examples were inspired
 by the book "Genetic Algorithms in Python" but are written from scratch
 and don't include any code from the book. The examples illustrates
 several points:
 
@@ -196,43 +200,43 @@
   ``check_stopping_conditions``. An exception of the lowercase-rule is
   whenever a name contains "GA" (for "genetic algorithm"), So
   ``PGASetMaxGAIterValue`` becomes ``max_GA_iter``.
 - Where possible I've made a single class method where PGAPack needs a
   separate function for each datatype, so ``PGAGetBinaryAllele``,
   ``PGAGetCharacterAllele``, ``PGAGetIntegerAllele``, ``PGAGetRealAllele`` all
   become ``get_allele``. Same holds true for ``set_allele``.
-- Whenever a name in PGApack has a "Value" or "Flag" suffix, I've left
+- Whenever a name in PGAPack has a "Value" or "Flag" suffix, I've left
   this out, so ``PGAGetFitnessCmaxValue`` becomes ``fitness_cmax``
   and ``PGAGetMutationAndCrossoverFlag`` becomes
   ``mutation_and_crossover``, the only exception to this rule is for the
   two functions ``PGAGetMutationRealValue`` and
   ``PGAGetMutationIntegerValue`` which become ``mutation_value`` not
   just ``mutation``.
 - Some fields can take multiple values (they are implemented by ORing
   integer constants, in python they are specified as a list or tuple of
   constants). These are converted to plural (if not already plural in
-  PGApack), e.g., ``PGASetStoppingRuleType`` becomes ``stopping_rule_types``.
+  PGAPack), e.g., ``PGASetStoppingRuleType`` becomes ``stopping_rule_types``.
 - Internal method names in the wrapper program have a leading PGA\_ |--| so
   the class method ``set_allele`` is implemented by the C-function
   ``PGA_set_allele`` in ``pgamodule.c``.
 
 Constructor Parameters
 ----------------------
 
-PGApack has a lot of ``PGASet`` and ``PGAGet`` functions for setting
+PGAPack_ has a lot of ``PGASet`` and ``PGAGet`` functions for setting
 parameters. These are reflected in constructor parameters on the one hand
 and in (typically read-only, but see below) properties of a ``PGA``
 object on the other hand. The
-following table gives an overview of all the original PGApack names and
-the names of the python wrapper. For the PGApack name I've only listed
+following table gives an overview of all the original PGAPack_ names and
+the names of the python wrapper. For the PGAPack_ name I've only listed
 the ``PGASet`` function, in many cases there is a corresponding
 ``PGAGet`` function. If a corresponding read-only property exists for a
 constructor parameter this is indicated in the "Prop" column. In some
 cases properties are missing because no corresponding ``PGAGet`` function
-is implemented in PGApack, in other cases returning a numeric value that
+is implemented in PGAPack_, in other cases returning a numeric value that
 has a symbolic constant in PGApy doesn't make much sense.
 
 The properties have the same name as the constructor parameter.
 There are Properties that don't have a corresponding constructor
 parameter, namely the ``eval_count`` property (returning the count of
 function evaluations), the
 ``GA_iter`` property that returns the current GA generation, and the
@@ -250,15 +254,15 @@
 allele* of the gene. In python this is a sequence of 2-tuples.
 Note that this means that you can have different ranges of allowed values
 for each allele.
 
 The ``num_eval`` property is special: Due to limitations of the C
 programming language, for multiple evaluations in C the first evaluation
 is returned as the function return-value of the ``evaluate`` function
-and all other parameters are returned in an auxiliary array. PGApack
+and all other parameters are returned in an auxiliary array. PGAPack_
 specifies the number of auxiliary evaluations to be returned. In Python
 the evaluation function can always return a sequence of evaluation
 values and the ``num_eval`` is one more than ``PGAGetNumAuxEval`` would
 return. The default for ``num_eval`` is 1.
 
 The first two (mandatory) constructor parameters are the type of the gene
 (this takes a Python type, e.g., ``bool`` for a binary genome or ``int``
@@ -270,15 +274,15 @@
 Some properties can now also be set *during* the run of the optimizer.
 These currently are ``crossover_prob``, ``epsilon_exponent``,
 ``multi_obj_precision``, ``p_tournament_prob``, and
 ``uniform_crossover_prob``. Just assign to the member variable of
 the optimizer (child of PGA.pga) object.
 
 ==================================== ================================= ====== ====
-PGApack name                         Constructor parameter             Type   Prop
+PGAPack name                         Constructor parameter             Type   Prop
 ==================================== ================================= ====== ====
 ``PGASetCrossoverBoundedFlag``       ``crossover_bounded``             int    yes
 ``PGASetCrossoverBounceBackFlag``    ``crossover_bounce_back``         int    yes
 ``PGASetCrossoverSBXEta``            ``crossover_SBX_eta``             float  yes
 ``PGASetCrossoverSBXOncePerString``  ``crossover_SBX_once_per_string`` int    yes
 ``PGASetCrossoverProb``              ``crossover_prob``                float  yes
 ``PGASetCrossoverType``              ``crossover_type``                sym    no
@@ -416,32 +420,32 @@
 ``set_gene``                  *p, pop, gen*      set gene (user data types)
 ``set_random_seed``           *seed*             None (use constructor!)
 ============================= ================== ===========================
 
 User-Methods
 ------------
 
-PGApack has the concept of user functions. These allow customization of
+PGAPack_ has the concept of user functions. These allow customization of
 different areas of a genetic algorihm. In Python they are implemented as
 methods that can be changed in a derived class. One of the methods that
 *must* be implemented in a derived class is the ``evaluate`` function
-(although technically it is not a user function in PGApack). It
+(although technically it is not a user function in PGAPack). It
 interprets the gene and returns an evaluation value or a sequence of
 evaluation values if you set the ``num_eval`` constructor parameter.
-PGApack computes a fitness from the raw evaluation value. For some
+PGAPack_ computes a fitness from the raw evaluation value. For some
 methods an up-call into the PGA class is possible, for some methods this
 is not possible (and in most cases not reasonable). Note that for the
 ``stop_cond`` method, the standard check for stopping conditions can be
 called with::
 
   self.check_stopping_conditions()
 
 The following table lists the overridable methods with their parameters
 (for the function signature the first parameter *self* is omitted). Note
-that in PGApack there are additional user functions that are needed for
+that in PGAPack_ there are additional user functions that are needed for
 user-defined data types which are currently not exposed in Python. In the
 function signatures *p* denotes the index of the individual and *pop*
 denotes the population. If more than one individual is specified (e.g.,
 for crossover) these can be followed by a number. For crossover *c1* and
 *c2* denote the destination individuals (children). The *propability* for
 the mutation method is a floating-point value between 0 and 1. Remember
 to count the number of mutations that happen, and return that value for
@@ -462,15 +466,15 @@
 ``pre_eval``        *pop*                          None              no
 ``print_string``    *file, p, pop*                 None              yes
 =================== ============================== ================= =======
 
 Constants
 ---------
 
-The following PGApack constants are available:
+The following PGAPack_ constants are available:
 
 ========================== ===========================================
 Constant                   Description
 ========================== ===========================================
 PGA_CROSSOVER_EDGE         Edge crossover for permutations
 PGA_CROSSOVER_ONEPT        One-point Crossover
 PGA_CROSSOVER_SBX          Simulated Binary Crossover
@@ -578,15 +582,15 @@
 over the serialization of the tree (which is the same for individuals
 with the same tree structure).
 
 
 Missing Features
 ----------------
 
-As already mentioned, not all functions and constants of PGAPack are
+As already mentioned, not all functions and constants of PGAPack_ are
 wrapped yet |--| still for many applications the given set should be
 enough. If you need additional functions, you may want to wrap these and
 send_ me a patch.
 
 Reporting Bugs
 --------------
 
@@ -627,15 +631,15 @@
 To install a *serial* version (without parallel programming using MPI_)
 you can simply install from pypi using ``pip``. Alternatively when you
 have unpacked or checked out from sources you can install with::
 
  python3 setup.py install --prefix=/usr/local
 
 If you want a parallel version using an MPI_ (Message-Passing Interface)
-library you will have to install a parallel version of PGApack first.
+library you will have to install a parallel version of PGAPack_ first.
 The easiest way to do this is to use `my pgapack debian package builder`_
 from github. Clone this repository, check out the branch ``master``,
 install the build dependencies, they're listed in the file
 ``debian/control`` and build the debian packages using::
 
   dpkg-buildpackage -rfakeroot
 
@@ -643,29 +647,68 @@
 debian, currently these are ``mpich``, ``openmpi``, and ``lam``. In addition
 to the MPI libraries a serial version of the pgapack library is also
 built. Proceed by installing the package pgapack and the MPI backend
 library of choice. If you don't have a preference for an MPI library,
 ``libpgapack-openmpi`` is the package that uses the Debians default
 preferences of an MPI library.
 
-Once a parallel version of PGApack is installed, you can install PGApy
+Once a parallel version of PGAPack_ is installed, you can install PGApy
 as follows: You set environment variables for the ``PGA_PARALLEL_VARIANT``
 (one of ``mpich``, ``openmpi``, or ``lam``) and set the ``PGA_MODULE`` to
 ``module_from_parallel_install``. Finally you envoke the setup, e.g.::
 
  export PGA_PARALLEL_VARIANT=openmpi
  export PGA_MODULE=module_from_parallel_install
  python3 setup.py install --prefix=/usr/local
 
+Note that the same works with ``pip install``, i.e., after installation
+of a parallel version of PGAPack_ you can directly install with ``pip``::
+
+ export PGA_PARALLEL_VARIANT=openmpi
+ export PGA_MODULE=module_from_parallel_install
+ pip install pgapy
+
+or alternatively depending on how pip is installed on your system::
+
+ python3 -m pip install pgapy
+
 If your MPI library is installed in a different place you should study
 the *Extension* configurations in ``setup.py`` to come up with an
 Extension definition that fits your installation. If your installation
 is interesting to more people, feel free to submit a patch that adds
 your Extension-configuration to the standard ``setup.py``.
 
+Running with MPI
+----------------
+
+To run a parallel version with MPI_, a parallel version must be
+installed, see above in section Installation_.
+
+For a serial version, PGAPy makes sure that the otimization is aborted
+if an exception occurs in the ``evaluate`` function. This is currently not
+the case for MPI, because the framework currently does not support
+returning information to the rank-0 MPI leader process. A workaround is
+as follows: Rename your ``evaluate`` method to ``_evaluate`` and catch
+exceptions in a new ``evaluate`` method that wraps ``_evaluate``.
+Call ``MPI_Abort`` if an exception occurs::
+
+    import traceback
+    import sys
+
+    ...
+
+    def evaluate (self, p, pop):
+        try:
+            return self._evaluate (p, pop)
+        except Exception:
+            # Optionally log exception here
+            print (traceback.format_exc ())
+            pga.MPI_Abort (1)
+            sys.exit (1)
+
 Testing
 -------
 
 For testing |--| preferrably before installation you can build locally::
 
     python3 setup.py build_ext --inplace
 
@@ -674,15 +717,15 @@
 
     python3 -m pytest test
 
 This runs all the tests and can take a while. Note that the tests run
 most of the examples in the ``examples`` directory with different
 command line parameters where available. To perform several optimization
 runs in a single (Python-) process, we must call ``MPI_Init``
-*explicitly* (and not relying on PGAPack to call it implicitly). This is
+*explicitly* (and not relying on PGAPack_ to call it implicitly). This is
 because ``MPI_Init`` may be called only once per process. Calling of
 ``MPI_Init`` and ``MPI_Finalize`` is handled in a fixture in
 ``test/conftest.py``
 
 Coverage
 ++++++++
 
@@ -803,17 +846,31 @@
         method for generating the pareto surface in nonlinear multicriteria
         optimization problems. SIAM Journal on Optimization, 8(3):631–657,
         August 1998.
 
 Changes
 -------
 
+Version 2.2.1: MPI_Abort
+
+- Add MPI_Abort to the wrapper
+- Include ``mpi_stub.c`` in the release (this is missing if some env
+  variables are set, see above in Installation)
+
+Version 2.2: Module directory
+
+- Put the pga C-module inside a pga module
+- Add several python-only modules to pga
+- pga.__init__ exports everything to this is compatible
+- pga.random includes a python Random class based on the pgapack random
+  number generator
+
 Version 2.1: Regression test
 
-- PGApack bug-fixes discovered during testing
+- PGAPack bug-fixes discovered during testing
 - Bug-fixes of python wrapper
 - Lots of tests with coverage of wrapper C-code > 90%
 
 Version 2.0: User defined data types
 
 - Implement user defined data types, note that your data type can be
   variable-size, e.g., a tree data structure. The framework takes care
@@ -951,7 +1008,15 @@
 PGAPy is a wrapper for PGAPack, the parallel genetic algorithm library,
 a powerful genetic algorithm library. PGAPy wraps this library for use
 with Python. Pgapack is one of the most complete and accurate genetic
 algorithm implementations out there with a lot of features for
 experimentation.
 
 - Initial Release
+
+.. _`PGAPack Readme`:
+   https://github.com/schlatterbeck/pgapack/blob/master/README.rst
+.. _PGAPack:          http://ftp.mcs.anl.gov/pub/pgapack/
+.. _`PGAPack fork on github`: https://github.com/schlatterbeck/pgapack
+.. _MPI: http://mpi-forum.org/
+.. _`my pgapack debian package builder`:
+    https://github.com/schlatterbeck/debian-pgapack
```

### Comparing `PGAPy-2.2/examples/cards.py` & `PGAPy-2.2.1/examples/cards.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/cards_mutate.py` & `PGAPy-2.2.1/examples/cards_mutate.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/constraint.py` & `PGAPy-2.2.1/examples/constraint.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/dtlz2.py` & `PGAPy-2.2.1/examples/dtlz2.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/fourbar.py` & `PGAPy-2.2.1/examples/fourbar.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/gears.py` & `PGAPy-2.2.1/examples/gears.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/gp/README.rst` & `PGAPy-2.2.1/examples/gp/README.rst`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/gp/gp.py` & `PGAPy-2.2.1/examples/gp/gp.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/gp/opt_integral.py` & `PGAPy-2.2.1/examples/gp/opt_integral.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/gp/opt_parity3.py` & `PGAPy-2.2.1/examples/gp/opt_parity3.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/gp/opt_xor.py` & `PGAPy-2.2.1/examples/gp/opt_xor.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/hello_world_char.py` & `PGAPy-2.2.1/examples/hello_world_char.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/hello_world_int.py` & `PGAPy-2.2.1/examples/hello_world_int.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/himmelblau.py` & `PGAPy-2.2.1/examples/himmelblau.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/magic_prio.py` & `PGAPy-2.2.1/examples/magic_prio.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/magic_square.py` & `PGAPy-2.2.1/examples/magic_square.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/minfloat.py` & `PGAPy-2.2.1/examples/minfloat.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/multi.py` & `PGAPy-2.2.1/examples/multi.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/namefull.py` & `PGAPy-2.2.1/examples/namefull.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/one_max.py` & `PGAPy-2.2.1/examples/one_max.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/sequence/croes.tsp` & `PGAPy-2.2.1/examples/sequence/croes.tsp`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/sequence/oliver30.tsp` & `PGAPy-2.2.1/examples/sequence/oliver30.tsp`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/sequence/plot_tour.py` & `PGAPy-2.2.1/examples/sequence/plot_tour.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/sequence/tsp.py` & `PGAPy-2.2.1/examples/sequence/tsp.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/sort_numbers.py` & `PGAPy-2.2.1/examples/sort_numbers.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/twobar.py` & `PGAPy-2.2.1/examples/twobar.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/vibr.py` & `PGAPy-2.2.1/examples/vibr.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/examples/xor.py` & `PGAPy-2.2.1/examples/xor.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/pga/__init__.py` & `PGAPy-2.2.1/pga/__init__.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/pga/random.py` & `PGAPy-2.2.1/pga/random.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/pga/testsupport.py` & `PGAPy-2.2.1/pga/testsupport.py`

 * *Files identical despite different names*

### Comparing `PGAPy-2.2/pgamodule.c` & `PGAPy-2.2.1/pgamodule.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Copyright (C) 2005-22 Dr. Ralf Schlatterbeck Open Source Consulting.
+/* Copyright (C) 2005-23 Dr. Ralf Schlatterbeck Open Source Consulting.
  * Reichergasse 131, A-3411 Weidling.
  * Web: http://www.runtux.com Email: office@runtux.com
  * ****************************************************************************
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
@@ -261,40 +261,57 @@
  * finally an MPI_finit) because MPI_Init may be called only once.
  * These are *module* methods (not PGA object methods)
  */
 
 static PyObject *PGA_MPI_Init (PyObject *self, PyObject *args, PyObject *kw)
 {
     int argc;
+    int ret = 0;
     char **c_argv = NULL;
     PyObject *pyargv;
     static char *kwlist [] = {"argv", NULL};
 
     if (!PyArg_ParseTupleAndKeywords (args, kw, "O", kwlist, &pyargv)) {
         return NULL;
     }
     c_argv = parse_argv (pyargv, &argc);
     Py_DECREF (pyargv);
-    MPI_Init (&argc, &c_argv);
-    Py_INCREF (Py_None);
-    return Py_None;
+    ret = MPI_Init (&argc, &c_argv);
+    return Py_BuildValue ("i", ret);
+}
+
+static PyObject *PGA_MPI_Abort (PyObject *self, PyObject *args, PyObject *kw)
+{
+    int errorcode = 0;
+    int ret = 0;
+    static char *kwlist [] =
+        { "errorcode"
+        , NULL
+        };
+    if (!PyArg_ParseTupleAndKeywords (args, kw, "i", kwlist, &errorcode)) {
+        return NULL;
+    }
+    ret = MPI_Abort (MPI_COMM_WORLD, errorcode);
+    return Py_BuildValue ("i", ret);
 }
 
 /* We don't care if someone calls this with arguments */
 static PyObject *PGA_MPI_Finalize (PyObject *self, PyObject *args, PyObject *kw)
 {
-    MPI_Finalize ();
-    Py_INCREF (Py_None);
-    return Py_None;
+    int ret = MPI_Finalize ();
+    return Py_BuildValue ("i", ret);
 }
 
 static PyMethodDef Module_Methods [] =
 { { "das_dennis", (PyCFunction)das_dennis, METH_VARARGS | METH_KEYWORDS
   , "Return Das/Dennis points"
   }
+, { "MPI_Abort", (PyCFunction)PGA_MPI_Abort, METH_VARARGS | METH_KEYWORDS
+  , "Abort MPI"
+  }
 , { "MPI_Finalize", (PyCFunction)PGA_MPI_Finalize, METH_VARARGS | METH_KEYWORDS
   , "Finalize MPI"
   }
 , { "MPI_Init", (PyCFunction)PGA_MPI_Init, METH_VARARGS | METH_KEYWORDS
   , "Initialize MPI"
   }
 , { NULL } /* EMPTY VALUE AS END-MARKER */
@@ -3358,14 +3375,24 @@
     PGAContext *ctx;
     if (!(ctx = get_context (self))) {
         return NULL;
     }
     return Py_BuildValue ("i", PGAGetNumAuxEval (ctx) + 1);
 }
 
+/* Special getter for maximize */
+static PyObject *PGA_maximize (PyObject *self, void *closure)
+{
+    PGAContext *ctx;
+    if (!(ctx = get_context (self))) {
+        return NULL;
+    }
+    return Py_BuildValue ("i", PGAGetOptDirFlag (ctx) == PGA_MAXIMIZE ? 1:0);
+}
+
 /* Yet another explicit getter which uses the default mpi communicator */
 static PyObject *PGA_mpi_rank (PyObject *self, void *closure)
 {
     PGAContext *ctx;
     if (!(ctx = get_context (self))) {
         return NULL;
     }
@@ -3411,14 +3438,15 @@
 , GETTER_ENTRY (fitness_cmax)
 , GETTER_ENTRY (fitness_min_type)
 , GETTER_ENTRY (fitness_type)
 , GETTER_ENTRY (GA_iter)
 , GETTER_ENTRY (max_fitness_rank)
 , GETTER_ENTRY (max_GA_iter)
 , GETTER_ENTRY (max_similarity)
+, GETTER_ENTRY (maximize)
 , GETTER_ENTRY (mpi_n_proc)
 , GETTER_ENTRY (mpi_rank)
 , GETSET_ENTRY (multi_obj_precision)
 , GETTER_ENTRY (mutation_and_crossover)
 , GETTER_ENTRY (mutation_or_crossover)
 , GETTER_ENTRY (mutation_only)
 , GETTER_ENTRY (mutation_poly_eta)
```

### Comparing `PGAPy-2.2/pgapack/docs/user_guide.pdf` & `PGAPy-2.2.1/pgapack/docs/user_guide.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 2% similar despite different names*

#### pdftotext {} -

```diff
@@ -12,15 +12,15 @@
 Genetic Algorithm Library
 by
 
 David Levine
 Mathematics and Computer Science Division
 and contributors
 
-January 31, 1996, last updated Oct 2022
+January 31, 1996, last updated Jan 2023
 This work was supported by the Mathematical, Information, and
 Computational Sciences Division subprogram of the Office of Computational and Technology Research, U.S. Department of Energy, under
 Contract W-31-109-Eng-38.
 This is not the original report, it contains small fixes reported by users
 and documentation updates for new features.
 
 Acknowledgments
@@ -1469,18 +1469,19 @@
 values out of the GA and return the value calculated by f.
 
 4.11
 
 Report Options
 
 PGASetPrintFrequencyValue(ctx,40) will print population statistics every 40 iterations. The default
-is every ten iterations. The best evaluation is always printed. To print additional statistics, set
-the second argument of the function PGASetPrintOptions to PGA REPORT ONLINE, PGA REPORT OFFLINE,
-PGA REPORT WORST, PGA REPORT AVERAGE, PGA REPORT HAMMING, or PGA REPORT STRING to print the online
-analysis, offline analysis, worst evaluation, average evaluation, Hamming distance, or string itself, respectively. PGASetPrintOptions may be called multiple times to specify multiple print options.
+is every ten iterations. The best evaluation is always printed. To print additional statistics, set the
+second argument of the function PGASetPrintOptions to PGA_REPORT_ONLINE, PGA_REPORT_OFFLINE,
+PGA_REPORT_WORST, PGA_REPORT_AVERAGE, PGA_REPORT_GENE_DISTANCE, or PGA_REPORT_STRING to print
+the online analysis, offline analysis, worst evaluation, average evaluation, genetic distance, or string itself,
+respectively. PGASetPrintOptions may be called multiple times to specify multiple print options.
 
 4.12
 
 Utility Functions
 
 4.12.1
 
@@ -1516,16 +1517,15 @@
 4.12.3
 
 Miscellaneous
 
 PGAGetGAIterValue(ctx) will return the current iteration of the GA. PGAGetBestIndex(ctx,pop)
 (PGAGetWorstIndex) will return the index of the most (least) fit member of population pop.
 PGAUpdateOffline(ctx,pop) (PGAUpdateOnline) will update the offline (online) analysis based on the
-new generation’s results. PGAHammingDistance(ctx,pop) returns a double, which is the average Hamming
-distance between the binary strings in population pop. The function call
+new generation’s results. PGAGeneDistance(ctx,pop) returns a double, which is the average genetic distance between the strings in population pop. The function call
 PGAError(ctx, "popindex=", PGA_FATAL, PGA_INT, (void *)&popindex)
 will print the message “popindex=-1” (assuming the value of popindex is -1) and then exit PGAPack. If
 the third argument had been PGA WARNING instead, execution would have continued. In addition to PGA INT,
 valid data types are PGA DOUBLE, PGA CHAR, and PGA VOID.
 
 4.13
 
@@ -1840,18 +1840,19 @@
 as this will cause an infinite loop to occur. Note that in a parallel program PGACheckStoppingConditions
 should only be called by the master process (see Chapter 9).
 The end of generation function (which is null by default) may be used for gathering statistics about the
 GA, displaying custom output, etc. This function is called after all generational computation is complete, but
 before the population pointers (PGA NEWPOP, PGA OLDPOP) have been switched and the standard PGAPack
 output printed. Therefore, be sure to use PGA NEWPOP as the population pointer. There is no mechanism for
 suppressing the standard PGAPack generational output.
-The genetic difference function computes the genetic difference of two individuals. It is only used when
-restricted tournament selection is in use. There are implementations for the standard data types: For binary
-alleles it uses the hamming distance. For real- and integer valued genes it uses an allele-by-allele absolute
-value of the difference by default (also know as Manhattan distance), i.e.
+The genetic difference function computes the genetic difference of two individuals. It is used when
+restricted tournament selection is in use. In addition it is used when reporting of genetic distance is selected by
+calling PGASetPrintOptions with PGA_REPORT_GENE_DISTANCE. There are implementations for the standard
+data types: For binary alleles it uses the hamming distance. For real- and integer valued genes it uses an
+allele-by-allele absolute value of the difference by default (also know as Manhattan distance), i.e.
 s−1
 X
 
 |aij − aik |
 
 i=0
 
@@ -1861,15 +1862,17 @@
 PGASetUserFunction(ctx, PGARealEuclidianDistance);
 or for the integer data type:
 PGASetUserFunction(ctx, PGAIntegerEuclidianDistance);
 This will use the Euclidian distance:
 v
 us−1
 uX
-t (aij − aik )2
+t (a − a )2
+ij
+ik
 i=0
 
 When using user-defined data types together with restricted tournament selection, an implementation of the
 distance function for the user-defined data type has to be provided.
 The Pre-Evaluate Hook function can be used for performing actions that need to be done before evaluating
 the generated individuals after crossover and mutation. It can be used, e.g., for repairing genes after crossover
 and mutation before evaluating them. It can also be used in concert with the end of generation function
@@ -1877,15 +1880,14 @@
 while the pre evaluate hook would look up newly-generated individuals in the cache: If a newly-generated
 individual is found in the cache, an evaluation can be saved which may have an impact on the runtime if
 evaluation is costly. Note that the probability of cache hits may be higher for binary and integer alleles
 than for real alleles. Note that for non-parallel implementations, caching could also be implemented in the
 evaluate function but for parallel implementations this would not work because each parallel instance would
 use a separate cache. The pre evaluation user function is called only in the master instance for a parallel
 implementation.
-
 37
 
 6.2
 
 Example Problem: C
 
 P
@@ -2700,76 +2702,61 @@
 Fortran (and C) programmers may access the trace facility via function calls.
 The function
 PGASetDebugLevel may be called to set a debug level. For example, call PGASetDebugLevel(ctx,12)
 would produce the same output shown in Figure 11.1. PGAClearDebugLevel(ctx,12) will clear prints
 associated with debug level 12. PGAPrintDebugOptions(ctx) will print the list of available debug options.
 The function PGASetDebugLevelByName will turn on debugging of the named function. For example, PGASetDebugLevelByName(ctx,’’PGACrossover’’) will enable all the trace prints of PGACrossover.
 PGAClearDebugLevelByName will disable the tracing of the specified function.
-Users can use the trace facility in their own functions (e.g., their evaluation function) in two ways.
-First, they can insert PGADebugPrint function calls in their functions using one of the symbolic constants
-defined in the header file pgapack.h. These are PGA DEBUG ENTERED, PGA DEBUG EXIT, PGA DEBUG MALLOC,
-PGA DEBUG PRINTVAR, PGA DEBUG SEND, and PGA DEBUG RECV for entering a function, exiting a function, allocating memory, print a variable’s value, and sending or receiving a string, respectively.
-For example, PGADebugPrint(ctx, PGA DEBUG ENTERED, "MyFunc", "Entered", PGA VOID, NULL)
-will print the line
-0: MyFunc
-
-: Entered
-
-when the debug level of 12 is specified. PGADebugPrint(ctx, PGA DEBUG PRINTVAR, "MyFunc", "i =
-", PGA INT, (void *) &i) will print the line
-0: MyFunc
-
-: i =
-
-1
-
-when the debug level of 82 is specified. Users can also use the reserved debug levels of 1–10 to customize the
-trace facilities for use in their own functions. For example PGADebugPrint( ctx, 5, "MyFunc", "After
-call to MyCleanUp", PGA VOID, NULL); will print the line
-55
-
-0: PGACreate
+0: PGACreate
 0: PGASetRandomSeed
 0: PGASetMaxGAIterValue
 0: PGASetUp
-0: PGACreatePop
-0: PGACreateIndividual
-:
-:
-0: PGACreateIndividual
-0: PGACreatePop
-0: PGACreateIndividual
-:
 :
 0: PGARun
 0: PGARunSeq
 0: PGAEvaluate
 0: PGAFitness
 0: PGAGetStringLength
 :
-:
 
 : Entered
 : Entered
 : Entered
 : Entered
 : Entered
 : Entered
-
 : Entered
 : Entered
 : Entered
 
-: Entered
-: Entered
-: Entered
-: Entered
+Figure 11.1: PGAPack Partial Trace Output for Maxbit Example
+
+55
+
+Users can use the trace facility in their own functions (e.g., their evaluation function) in two ways.
+First, they can insert PGADebugPrint function calls in their functions using one of the symbolic constants
+defined in the header file pgapack.h. These are PGA DEBUG ENTERED, PGA DEBUG EXIT, PGA DEBUG MALLOC,
+PGA DEBUG PRINTVAR, PGA DEBUG SEND, and PGA DEBUG RECV for entering a function, exiting a function, allocating memory, print a variable’s value, and sending or receiving a string, respectively.
+For example, PGADebugPrint(ctx, PGA DEBUG ENTERED, "MyFunc", "Entered", PGA VOID, NULL)
+will print the line
+0: MyFunc
+
 : Entered
 
-Figure 11.1: PGAPack Partial Trace Output for Maxbit Example
+when the debug level of 12 is specified. PGADebugPrint(ctx, PGA DEBUG PRINTVAR, "MyFunc", "i =
+", PGA INT, (void *) &i) will print the line
+0: MyFunc
+
+: i =
+
+1
+
+when the debug level of 82 is specified. Users can also use the reserved debug levels of 1–10 to customize the
+trace facilities for use in their own functions. For example PGADebugPrint( ctx, 5, "MyFunc", "After
+call to MyCleanUp", PGA VOID, NULL); will print the line
 0: MyFunc
 
 : After call to MyCleanUp
 
 when the debug level of five is specified.
 Note that we use MPI COMM WORLD (1) for the random number seed and (2) for PGADebugPrint calls.
 
@@ -2925,15 +2912,15 @@
 
 CONCEPT
 Print strings
 Print offline statistics
 Print online statistics
 Print best string
 Print worst string
-Print Hamming distance
+Print genetic distance
 Randomly initialize population
 Probability of initializing a bit to one
 How to initialize real strings
 Real initialization range
 How to initialize integer strings
 Integer initialization range
 How to initialize character strings
@@ -3097,20 +3084,20 @@
 – PGA CINIT MIXED
 – PGA IINIT PERMUTE
 – PGA IINIT RANGE
 – PGA RINIT PERCENT
 – PGA RINIT RANGE
 • Report Options
 
-– PGA REPORT ONLINE
-– PGA REPORT OFFLINE
-– PGA REPORT HAMMING
-– PGA REPORT STRING
-– PGA REPORT WORST
-– PGA REPORT AVERAGE
+– PGA_REPORT_ONLINE
+– PGA_REPORT_OFFLINE
+– PGA_REPORT_GENE_DISTANCE
+– PGA_REPORT_STRING
+– PGA_REPORT_WORST
+– PGA_REPORT_AVERAGE
 • Selection
 
 – PGA_SELECT_PROPORTIONAL
 – PGA_SELECT_SUS
 – PGA_SELECT_TOURNAMENT
 – PGA_SELECT_PTOURNAMENT
 – PGA_SELECT_TRUNCATION
@@ -3327,15 +3314,15 @@
 PGAGetStoppingRuleType(PGAContext *ctx)
 PGAGetStringLength(PGAContext *ctx)
 PGAGetTournamentSize(PGAContext *ctx)
 PGAGetTournamentWithReplacement(PGAContext *ctx)
 PGAGetTruncationProportion(PGAContext *ctx)
 PGAGetUniformCrossoverProb(PGAContext *ctx)
 PGAGetWorstIndex(PGAContext *ctx, int pop)
-PGAHammingDistance(PGAContext *ctx, int popindex)
+PGAGeneDistance(PGAContext *ctx, int popindex)
 PGAMean(PGAContext *ctx, double *a, int n)
 PGAMutate(PGAContext *ctx, int p, int pop)
 65
 
 Type
 void
 void
@@ -3888,15 +3875,15 @@
 
 [15] W. Gropp, E. Lusk, and A. Skjellum. USING MPI Portable Parallel Programming with the MessagePassing Interface. The MIT Press, Cambrigde, 1994.
 [16] Georges Harik. Finding multiple solutions in problems of bounded difficulty. IlliGAL Report 94002,
 Illinois Genetic Algorithm Lab, May 1994.
 [17] Georges R. Harik. Finding multimodal solutions using restricted tournament selection. In Larry J.
 Eshelman, editor, Proceedings of the International Conference on Genetic Algorithms (ICGA), pages
 24–31. Morgan Kaufmann, July 1995.
-[18] Georges R. Harik and David E. Goldberg. Learning linkage. In Richard K. Belew and Michael D. Vose:,
+[18] Georges R. Harik and David E. Goldberg. Learning linkage. In Richard K. Belew and Michael D. Vose,
 editors, Foundations of Genetic Algorithms (FOGA) 4, pages 247–262, San Diego, CA, August 1996.
 Morgan Kaufmann.
 [19] J. Holland. Adaption in Natural and Artificial Systems. MIT Press, Cambrigde, 1992.
 [20] Himanshu Jain and Kalyanmoy Deb. An evolutionary many-objective optimization algorithm using
 reference-point-based nondominated sorting approach, part II: Handling constraints and extending to
 an adaptive approach. IEEE Transactions on Evolutionary Computation, 18(4):602–622, August 2014.
 [21] Martin Pelikan. Hierarchical Bayesian Optimization Algorithm: Toward a New Generation of Evolutionary Algorithms, volume 170 of Studies in Fuzziness and Soft Computing. Springer, 2005.
```

### Comparing `PGAPy-2.2/pgapack/fakempi/mpi.h` & `PGAPy-2.2.1/pgapack/fakempi/mpi.h`

 * *Files 9% similar despite different names*

```diff
@@ -39,25 +39,29 @@
 #define MPI_PROC_NULL       (-1)
 #define MPI_ANY_SOURCE      (-2)
 #define MPI_ANY_TAG         (-1)
 
 #define MPI_STATUS_IGNORE   (void *)NULL
 
 /*  Declare prototypes for the MPI functions.  */
-int MPI_Get_address(void *, MPI_Aint *);
-int MPI_Bcast(void *, int, MPI_Datatype, int, MPI_Comm);
-int MPI_Comm_dup(MPI_Comm, MPI_Comm *);
-int MPI_Comm_free(MPI_Comm *);
-int MPI_Comm_rank(MPI_Comm, int *);
-int MPI_Comm_size(MPI_Comm, int *);
-int MPI_Finalize(void);
-int MPI_Finalized(int *);
-int MPI_Init(int *, char ***);
-int MPI_Initialized(int *);
-int MPI_Probe(int, int, MPI_Comm, MPI_Status *);
-int MPI_Send(void *, int, MPI_Datatype, int, int, MPI_Comm);
+int MPI_Abort (MPI_Comm, int);
+int MPI_Get_address (void *, MPI_Aint *);
+int MPI_Bcast (void *, int, MPI_Datatype, int, MPI_Comm);
+int MPI_Comm_dup (MPI_Comm, MPI_Comm *);
+int MPI_Comm_free (MPI_Comm *);
+int MPI_Comm_rank (MPI_Comm, int *);
+int MPI_Comm_size (MPI_Comm, int *);
+int MPI_Finalize (void);
+int MPI_Finalized (int *);
+int MPI_Init (int *, char ***);
+int MPI_Initialized (int *);
+int MPI_Probe (int, int, MPI_Comm, MPI_Status *);
+int MPI_Send (void *, int, MPI_Datatype, int, int, MPI_Comm);
 int MPI_Recv(void *, int, MPI_Datatype, int, int, MPI_Comm, MPI_Status *);
-int MPI_Sendrecv(void *, int, MPI_Datatype, int, int, void *, int,
-	         MPI_Datatype, int, int, MPI_Comm, MPI_Status *);
-int MPI_Type_commit(MPI_Datatype *);
-int MPI_Type_free(MPI_Datatype *);
-int MPI_Type_create_struct(int, int *, MPI_Aint *, MPI_Datatype *, MPI_Datatype *);
+int MPI_Sendrecv
+    ( void *, int, MPI_Datatype, int, int, void *, int
+    , MPI_Datatype, int, int, MPI_Comm, MPI_Status *
+    );
+int MPI_Type_commit (MPI_Datatype *);
+int MPI_Type_free (MPI_Datatype *);
+int MPI_Type_create_struct
+    (int, int *, MPI_Aint *, MPI_Datatype *, MPI_Datatype *);
```

### Comparing `PGAPy-2.2/setup.py` & `PGAPy-2.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Copyright (C) 2005-22 Dr. Ralf Schlatterbeck Open Source Consulting.
+# Copyright (C) 2005-23 Dr. Ralf Schlatterbeck Open Source Consulting.
 # Reichergasse 131, A-3411 Weidling.
 # Web: http://www.runtux.com Email: office@runtux.com
 # ****************************************************************************
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are
 # met:
 #
```

### Comparing `PGAPy-2.2/test/test_pgapy.py` & `PGAPy-2.2.1/test/test_pgapy.py`

 * *Files identical despite different names*

