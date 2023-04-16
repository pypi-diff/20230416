# Comparing `tmp/anaflow-1.0.1.tar.gz` & `tmp/anaflow-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/anaflow-1.0.1.tar", last modified: Thu Apr  2 15:16:25 2020, max compression
+gzip compressed data, was "anaflow-1.1.0.tar", last modified: Sun Apr 16 11:43:27 2023, max compression
```

## Comparing `anaflow-1.0.1.tar` & `anaflow-1.1.0.tar`

### file list

```diff
@@ -1,103 +1,26 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-02 15:16:25.373247 anaflow-1.0.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)      170 2020-04-02 15:16:11.000000 anaflow-1.0.1/.coveragerc
--rw-rw-r--   0 travis    (2000) travis    (2000)       96 2020-04-02 15:16:11.000000 anaflow-1.0.1/.gitignore
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2252 2020-04-02 15:16:11.000000 anaflow-1.0.1/.travis.yml
--rwxrwxr-x   0 travis    (2000) travis    (2000)      464 2020-04-02 15:16:11.000000 anaflow-1.0.1/.zenodo.json
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2376 2020-04-02 15:16:11.000000 anaflow-1.0.1/CHANGELOG.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1091 2020-04-02 15:16:11.000000 anaflow-1.0.1/LICENSE
--rwxrwxr-x   0 travis    (2000) travis    (2000)      225 2020-04-02 15:16:11.000000 anaflow-1.0.1/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     5613 2020-04-02 15:16:25.373247 anaflow-1.0.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3428 2020-04-02 15:16:11.000000 anaflow-1.0.1/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-02 15:16:25.357247 anaflow-1.0.1/anaflow/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2121 2020-04-02 15:16:11.000000 anaflow-1.0.1/anaflow/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       21 2020-04-02 15:16:25.000000 anaflow-1.0.1/anaflow/_version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-02 15:16:25.361247 anaflow-1.0.1/anaflow/flow/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1561 2020-04-02 15:16:11.000000 anaflow-1.0.1/anaflow/flow/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7019 2020-04-02 15:16:11.000000 anaflow-1.0.1/anaflow/flow/ext_grf_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    49753 2020-04-02 15:16:11.000000 anaflow-1.0.1/anaflow/flow/heterogeneous.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7793 2020-04-02 15:16:11.000000 anaflow-1.0.1/anaflow/flow/homogeneous.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11330 2020-04-02 15:16:11.000000 anaflow-1.0.1/anaflow/flow/laplace.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-02 15:16:25.361247 anaflow-1.0.1/anaflow/tools/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1676 2020-04-02 15:16:11.000000 anaflow-1.0.1/anaflow/tools/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16299 2020-04-02 15:16:11.000000 anaflow-1.0.1/anaflow/tools/coarse_graining.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14360 2020-04-02 15:16:11.000000 anaflow-1.0.1/anaflow/tools/laplace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12225 2020-04-02 15:16:11.000000 anaflow-1.0.1/anaflow/tools/mean.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15594 2020-04-02 15:16:11.000000 anaflow-1.0.1/anaflow/tools/special.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-02 15:16:25.361247 anaflow-1.0.1/anaflow.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5613 2020-04-02 15:16:25.000000 anaflow-1.0.1/anaflow.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2803 2020-04-02 15:16:25.000000 anaflow-1.0.1/anaflow.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-04-02 15:16:25.000000 anaflow-1.0.1/anaflow.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      187 2020-04-02 15:16:25.000000 anaflow-1.0.1/anaflow.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2020-04-02 15:16:25.000000 anaflow-1.0.1/anaflow.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-02 15:16:25.361247 anaflow-1.0.1/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      612 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)       76 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/requirements.txt
--rwxrwxr-x   0 travis    (2000) travis    (2000)        9 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/requirements_doc.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-02 15:16:25.365247 anaflow-1.0.1/docs/source/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-02 15:16:25.365247 anaflow-1.0.1/docs/source/_templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)      967 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/_templates/layout.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     7560 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      110 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/contents.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/flow.ext_grf_model.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/flow.heterogeneous.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      177 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/flow.homogeneous.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      165 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/flow.laplace.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      211 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/flow.rst
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2129 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      145 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/package.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-02 15:16:25.373247 anaflow-1.0.1/docs/source/pics/
--rw-rw-r--   0 travis    (2000) travis    (2000)    31400 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/pics/01_call_theis.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    56905 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/pics/02_call_ext_theis.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    58189 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/pics/03_call_ext_theis3d.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    60470 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/pics/04_call_ext_theis_tpl.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    56188 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/pics/05_call_neuman2004.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    21779 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/pics/06_compare_extthiem2d_grfsteady.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    22085 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/pics/07_compare_extthiem3d_grfsteady.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    28314 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/pics/08_compare_extthiem2d_neuman.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    44260 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/pics/09_compare_exttheis2d_neuman.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    26563 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/pics/10_convergence_ext_theis_tpl.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    30271 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/pics/11_convergence_ext_grf.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    42336 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/pics/12_compare_theis_quasi_steady.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    42951 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/pics/13_self_defined_transmissivity.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    38051 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/pics/14_interval_theis.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    51748 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/pics/15_accruing_theis.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     4286 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/pics/Anaflow.ico
--rw-rw-r--   0 travis    (2000) travis    (2000)    56688 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/pics/Anaflow.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    11780 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/pics/Anaflow_150.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      192 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/tools.coarse_graining.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      168 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/tools.laplace.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      159 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/tools.mean.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      207 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/tools.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      168 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/tools.special.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      727 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/tutorial_01_call.rst
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2281 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/tutorial_02_extended_theis.rst
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2775 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/tutorial_03_extended_theis3d.rst
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2601 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/tutorial_04_ext_theis_tpl.rst
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2608 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/tutorial_05_neuman2004.rst
--rwxrwxr-x   0 travis    (2000) travis    (2000)     7163 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/tutorial_06_comparison.rst
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4922 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/tutorial_07_convergence.rst
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6082 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/tutorial_08_advanced.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      438 2020-04-02 15:16:11.000000 anaflow-1.0.1/docs/source/tutorials.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-02 15:16:25.373247 anaflow-1.0.1/examples/
--rw-rw-r--   0 travis    (2000) travis    (2000)      378 2020-04-02 15:16:11.000000 anaflow-1.0.1/examples/01_call_theis.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1517 2020-04-02 15:16:11.000000 anaflow-1.0.1/examples/02_call_ext_theis2d.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1913 2020-04-02 15:16:11.000000 anaflow-1.0.1/examples/03_call_ext_theis3d.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1674 2020-04-02 15:16:11.000000 anaflow-1.0.1/examples/04_call_ext_theis_tpl.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1620 2020-04-02 15:16:11.000000 anaflow-1.0.1/examples/05_call_neuman2004.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      902 2020-04-02 15:16:11.000000 anaflow-1.0.1/examples/06_compare_extthiem2d_grfsteady.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      964 2020-04-02 15:16:11.000000 anaflow-1.0.1/examples/07_compare_extthiem3d_grfsteady.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      838 2020-04-02 15:16:11.000000 anaflow-1.0.1/examples/08_compare_extthiem2d_neuman.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1375 2020-04-02 15:16:11.000000 anaflow-1.0.1/examples/09_compare_exttheis2d_neuman.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1072 2020-04-02 15:16:11.000000 anaflow-1.0.1/examples/10_convergence_ext_theis_tpl.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      993 2020-04-02 15:16:11.000000 anaflow-1.0.1/examples/11_convergence_ext_grf.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      934 2020-04-02 15:16:11.000000 anaflow-1.0.1/examples/12_compare_theis_quasi_steady.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2080 2020-04-02 15:16:11.000000 anaflow-1.0.1/examples/13_self_defined_transmissivity.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      567 2020-04-02 15:16:11.000000 anaflow-1.0.1/examples/14_interval_theis.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1179 2020-04-02 15:16:11.000000 anaflow-1.0.1/examples/15_accruing_theis.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)       42 2020-04-02 15:16:11.000000 anaflow-1.0.1/requirements.txt
--rwxrwxr-x   0 travis    (2000) travis    (2000)       41 2020-04-02 15:16:11.000000 anaflow-1.0.1/requirements_setup.txt
--rwxrwxr-x   0 travis    (2000) travis    (2000)       32 2020-04-02 15:16:11.000000 anaflow-1.0.1/requirements_test.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      102 2020-04-02 15:16:25.377247 anaflow-1.0.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2520 2020-04-02 15:16:11.000000 anaflow-1.0.1/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-02 15:16:25.373247 anaflow-1.0.1/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7247 2020-04-02 15:16:11.000000 anaflow-1.0.1/tests/test_anaflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:43:27.627277 anaflow-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-16 11:42:50.000000 anaflow-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-16 11:43:27.627277 anaflow-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-16 11:42:50.000000 anaflow-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-16 11:42:50.000000 anaflow-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 11:43:27.627277 anaflow-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:43:27.623278 anaflow-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:43:27.623278 anaflow-1.1.0/src/anaflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-16 11:42:50.000000 anaflow-1.1.0/src/anaflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-16 11:43:27.000000 anaflow-1.1.0/src/anaflow/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:43:27.623278 anaflow-1.1.0/src/anaflow/flow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-16 11:42:50.000000 anaflow-1.1.0/src/anaflow/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-16 11:42:50.000000 anaflow-1.1.0/src/anaflow/flow/ext_grf_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49692 2023-04-16 11:42:50.000000 anaflow-1.1.0/src/anaflow/flow/heterogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-04-16 11:42:50.000000 anaflow-1.1.0/src/anaflow/flow/homogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-04-16 11:42:50.000000 anaflow-1.1.0/src/anaflow/flow/laplace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:43:27.623278 anaflow-1.1.0/src/anaflow/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-16 11:42:50.000000 anaflow-1.1.0/src/anaflow/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-04-16 11:42:50.000000 anaflow-1.1.0/src/anaflow/tools/coarse_graining.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-04-16 11:42:50.000000 anaflow-1.1.0/src/anaflow/tools/laplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-04-16 11:42:50.000000 anaflow-1.1.0/src/anaflow/tools/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15580 2023-04-16 11:42:50.000000 anaflow-1.1.0/src/anaflow/tools/special.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:43:27.623278 anaflow-1.1.0/src/anaflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-16 11:43:27.000000 anaflow-1.1.0/src/anaflow.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:43:27.623278 anaflow-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-04-16 11:42:50.000000 anaflow-1.1.0/tests/test_anaflow.py
```

### Comparing `anaflow-1.0.1/LICENSE` & `anaflow-1.1.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2019 - 2020 Sebastian Mueller
+Copyright (c) 2019 - 2023 Sebastian Mueller
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `anaflow-1.0.1/PKG-INFO` & `anaflow-1.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,127 +1,19 @@
 Metadata-Version: 2.1
 Name: anaflow
-Version: 1.0.1
+Version: 1.1.0
 Summary: AnaFlow - analytical solutions for the groundwater-flow equation.
-Home-page: https://github.com/GeoStat-Framework/AnaFlow
-Author: Sebastian Mueller
-Author-email: sebastian.mueller@ufz.de
-Maintainer: Sebastian Mueller
-Maintainer-email: sebastian.mueller@ufz.de
+Author-email: Sebastian Mueller <sebastian.mueller@ufz.de>
 License: MIT
-Description: # Welcome to AnaFlow
-        
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1135723.svg)](https://doi.org/10.5281/zenodo.1135723)
-        [![PyPI version](https://badge.fury.io/py/anaflow.svg)](https://badge.fury.io/py/anaflow)
-        [![Build Status](https://travis-ci.com/GeoStat-Framework/AnaFlow.svg?branch=master)](https://travis-ci.com/GeoStat-Framework/AnaFlow)
-        [![Documentation Status](https://readthedocs.org/projects/docs/badge/?version=stable)](https://anaflow.readthedocs.io/en/stable/)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
-        
-        <p align="center">
-        <img src="https://raw.githubusercontent.com/GeoStat-Framework/AnaFlow/master/docs/source/pics/Anaflow.png" alt="AnaFlow-LOGO" width="251px"/>
-        </p>
-        
-        ## Purpose
-        
-        AnaFlow provides several analytical and semi-analytical solutions for the
-        groundwater-flow equation.
-        
-        
-        ## Installation
-        
-        You can install the latest version with the following command:
-        
-            pip install anaflow
-        
-        
-        ## Documentation for AnaFlow
-        
-        You can find the documentation under [geostat-framework.readthedocs.io][doc_link].
-        
-        
-        ### Example
-        
-        In the following the well known Theis function is called an plotted for three
-        different time-steps.
-        
-        ```python
-        import numpy as np
-        from matplotlib import pyplot as plt
-        from anaflow import theis
-        
-        
-        time = [10, 100, 1000]
-        rad = np.geomspace(0.1, 10)
-        
-        head = theis(time=time, rad=rad, transmissivity=1e-4, storage=1e-4, rate=-1e-4)
-        
-        for i, step in enumerate(time):
-            plt.plot(rad, head[i], label="Theis(t={})".format(step))
-        
-        plt.legend()
-        plt.show()
-        ```
-        
-        <p align="center">
-        <img src="https://raw.githubusercontent.com/GeoStat-Framework/AnaFlow/master/docs/source/pics/01_call_theis.png" alt="Theis" width="600px"/>
-        </p>
-        
-        
-        ### Provided Functions
-        
-        The following functions are provided directly
-        
-        * ``thiem`` Thiem solution for steady state pumping
-        * ``theis`` Theis solution for transient pumping
-        * ``ext_thiem_2d`` extended Thiem solution in 2D from *Zech 2013*
-        * ``ext_theis_2d`` extended Theis solution in 2D from *Mueller 2015*
-        * ``ext_thiem_3d`` extended Thiem solution in 3D from *Zech 2013*
-        * ``ext_theis_3d`` extended Theis solution in 3D from *Mueller 2015*
-        * ``neuman2004`` transient solution from *Neuman 2004*
-        * ``neuman2004_steady`` steady solution from *Neuman 2004*
-        * ``grf`` "General Radial Flow" Model from *Barker 1988*
-        * ``ext_grf`` the transient extended GRF model
-        * ``ext_grf_steady`` the steady extended GRF model
-        * ``ext_thiem_tpl`` extended Thiem solution for truncated power laws
-        * ``ext_theis_tpl`` extended Theis solution for truncated power laws
-        * ``ext_thiem_tpl_3d`` extended Thiem solution in 3D for truncated power laws
-        * ``ext_theis_tpl_3d`` extended Theis solution in 3D for truncated power laws
-        
-        
-        ### Laplace Transformation
-        
-        We provide routines to calculate the laplace-transformation as well as the
-        inverse laplace-transformation of a given function
-        
-        * ``get_lap`` Get the laplace transformation of a function
-        * ``get_lap_inv`` Get the inverse laplace transformation of a function
-        
-        
-        ## Requirements
-        
-        - [NumPy >= 1.14.5](https://www.numpy.org)
-        - [SciPy >= 1.1.0](https://www.scipy.org)
-        - [pentapy >= 1.1.0](https://github.com/GeoStat-Framework/pentapy)
-        
-        
-        ## Contact
-        
-        You can contact us via <info@geostat-framework.org>.
-        
-        
-        ## License
-        
-        [MIT][mit_link] © 2019 - 2020
-        
-        [mit_link]: https://github.com/GeoStat-Framework/AnaFlow/blob/master/LICENSE
-        [doc_link]: https://anaflow.readthedocs.io
-        
-Platform: Windows
-Platform: Linux
-Platform: Mac OS-X
+Project-URL: Homepage, https://github.com/GeoStat-Framework/AnaFlow
+Project-URL: Documentation, https://anaflow.readthedocs.io
+Project-URL: Source, https://github.com/GeoStat-Framework/anaflow
+Project-URL: Tracker, https://github.com/GeoStat-Framework/anaflow/issues
+Project-URL: Changelog, https://github.com/GeoStat-Framework/anaflow/blob/main/CHANGELOG.md
+Project-URL: Conda-Forge, https://anaconda.org/conda-forge/anaflow
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
@@ -129,15 +21,127 @@
 Classifier: Operating System :: Microsoft
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: test
-Provides-Extra: dev
+Provides-Extra: check
+License-File: LICENSE
+
+# Welcome to AnaFlow
+
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1135723.svg)](https://doi.org/10.5281/zenodo.1135723)
+[![PyPI version](https://badge.fury.io/py/anaflow.svg)](https://badge.fury.io/py/anaflow)
+[![Build Status](https://github.com/GeoStat-Framework/AnaFlow/workflows/Continuous%20Integration/badge.svg?branch=main)](https://github.com/GeoStat-Framework/AnaFlow/actions)
+[![Documentation Status](https://readthedocs.org/projects/docs/badge/?version=latest)](https://anaflow.readthedocs.io/en/latest/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/GeoStat-Framework/AnaFlow/main/docs/source/pics/Anaflow.png" alt="AnaFlow-LOGO" width="251px"/>
+</p>
+
+## Purpose
+
+AnaFlow provides several analytical and semi-analytical solutions for the
+groundwater-flow equation.
+
+
+## Installation
+
+You can install the latest version with the following command:
+
+    pip install anaflow
+
+
+## Documentation for AnaFlow
+
+You can find the documentation under [https://anaflow.readthedocs.io][doc_link].
+
+
+### Example
+
+In the following the well known Theis function is called an plotted for three
+different time-steps.
+
+```python
+import numpy as np
+from matplotlib import pyplot as plt
+from anaflow import theis
+
+
+time = [10, 100, 1000]
+rad = np.geomspace(0.1, 10)
+
+head = theis(time=time, rad=rad, transmissivity=1e-4, storage=1e-4, rate=-1e-4)
+
+for i, step in enumerate(time):
+    plt.plot(rad, head[i], label="Theis(t={})".format(step))
+
+plt.legend()
+plt.show()
+```
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/GeoStat-Framework/AnaFlow/main/docs/source/pics/01_call_theis.png" alt="Theis" width="600px"/>
+</p>
+
+
+### Provided Functions
+
+The following functions are provided directly
+
+* ``thiem`` Thiem solution for steady state pumping
+* ``theis`` Theis solution for transient pumping
+* ``ext_thiem_2d`` extended Thiem solution in 2D from *Zech 2013*
+* ``ext_theis_2d`` extended Theis solution in 2D from *Mueller 2015*
+* ``ext_thiem_3d`` extended Thiem solution in 3D from *Zech 2013*
+* ``ext_theis_3d`` extended Theis solution in 3D from *Mueller 2015*
+* ``neuman2004`` transient solution from *Neuman 2004*
+* ``neuman2004_steady`` steady solution from *Neuman 2004*
+* ``grf`` "General Radial Flow" Model from *Barker 1988*
+* ``ext_grf`` the transient extended GRF model
+* ``ext_grf_steady`` the steady extended GRF model
+* ``ext_thiem_tpl`` extended Thiem solution for truncated power laws
+* ``ext_theis_tpl`` extended Theis solution for truncated power laws
+* ``ext_thiem_tpl_3d`` extended Thiem solution in 3D for truncated power laws
+* ``ext_theis_tpl_3d`` extended Theis solution in 3D for truncated power laws
+
+
+### Laplace Transformation
+
+We provide routines to calculate the laplace-transformation as well as the
+inverse laplace-transformation of a given function
+
+* ``get_lap`` Get the laplace transformation of a function
+* ``get_lap_inv`` Get the inverse laplace transformation of a function
+
+
+## Requirements
+
+- [NumPy >= 1.14.5](https://www.numpy.org)
+- [SciPy >= 1.1.0](https://www.scipy.org)
+- [pentapy >= 1.1.0](https://github.com/GeoStat-Framework/pentapy)
+
+
+## Contact
+
+You can contact us via <info@geostat-framework.org>.
+
+
+## License
+
+[MIT][mit_link] © 2019 - 2023
+
+[mit_link]: https://github.com/GeoStat-Framework/AnaFlow/blob/main/LICENSE
+[doc_link]: https://anaflow.readthedocs.io
```

### Comparing `anaflow-1.0.1/README.md` & `anaflow-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Welcome to AnaFlow
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1135723.svg)](https://doi.org/10.5281/zenodo.1135723)
 [![PyPI version](https://badge.fury.io/py/anaflow.svg)](https://badge.fury.io/py/anaflow)
-[![Build Status](https://travis-ci.com/GeoStat-Framework/AnaFlow.svg?branch=master)](https://travis-ci.com/GeoStat-Framework/AnaFlow)
-[![Documentation Status](https://readthedocs.org/projects/docs/badge/?version=stable)](https://anaflow.readthedocs.io/en/stable/)
+[![Build Status](https://github.com/GeoStat-Framework/AnaFlow/workflows/Continuous%20Integration/badge.svg?branch=main)](https://github.com/GeoStat-Framework/AnaFlow/actions)
+[![Documentation Status](https://readthedocs.org/projects/docs/badge/?version=latest)](https://anaflow.readthedocs.io/en/latest/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 <p align="center">
-<img src="https://raw.githubusercontent.com/GeoStat-Framework/AnaFlow/master/docs/source/pics/Anaflow.png" alt="AnaFlow-LOGO" width="251px"/>
+<img src="https://raw.githubusercontent.com/GeoStat-Framework/AnaFlow/main/docs/source/pics/Anaflow.png" alt="AnaFlow-LOGO" width="251px"/>
 </p>
 
 ## Purpose
 
 AnaFlow provides several analytical and semi-analytical solutions for the
 groundwater-flow equation.
 
@@ -21,15 +21,15 @@
 You can install the latest version with the following command:
 
     pip install anaflow
 
 
 ## Documentation for AnaFlow
 
-You can find the documentation under [geostat-framework.readthedocs.io][doc_link].
+You can find the documentation under [https://anaflow.readthedocs.io][doc_link].
 
 
 ### Example
 
 In the following the well known Theis function is called an plotted for three
 different time-steps.
 
@@ -48,15 +48,15 @@
     plt.plot(rad, head[i], label="Theis(t={})".format(step))
 
 plt.legend()
 plt.show()
 ```
 
 <p align="center">
-<img src="https://raw.githubusercontent.com/GeoStat-Framework/AnaFlow/master/docs/source/pics/01_call_theis.png" alt="Theis" width="600px"/>
+<img src="https://raw.githubusercontent.com/GeoStat-Framework/AnaFlow/main/docs/source/pics/01_call_theis.png" alt="Theis" width="600px"/>
 </p>
 
 
 ### Provided Functions
 
 The following functions are provided directly
 
@@ -96,11 +96,11 @@
 ## Contact
 
 You can contact us via <info@geostat-framework.org>.
 
 
 ## License
 
-[MIT][mit_link] © 2019 - 2020
+[MIT][mit_link] © 2019 - 2023
 
-[mit_link]: https://github.com/GeoStat-Framework/AnaFlow/blob/master/LICENSE
+[mit_link]: https://github.com/GeoStat-Framework/AnaFlow/blob/main/LICENSE
 [doc_link]: https://anaflow.readthedocs.io
```

### Comparing `anaflow-1.0.1/anaflow/__init__.py` & `anaflow-1.1.0/src/anaflow/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,41 @@
-# -*- coding: utf-8 -*-
 """
 Purpose
 =======
 
 Anaflow provides several analytical and semi-analytical solutions for the
 groundwater-flow-equation.
 
 Subpackages
 ===========
 
 .. autosummary::
-    flow
-    tools
+   :toctree: api
+
+   flow
+   tools
 
 Solutions
 =========
 
 Homogeneous
 ^^^^^^^^^^^
 
-.. currentmodule:: anaflow.flow.homogeneous
+.. currentmodule:: anaflow.flow
 
 Solutions for homogeneous aquifers
 
 .. autosummary::
    thiem
    theis
    grf
 
 Heterogeneous
 ^^^^^^^^^^^^^
 
-.. currentmodule:: anaflow.flow.heterogeneous
-
 Solutions for heterogeneous aquifers
 
 .. autosummary::
    ext_thiem_2d
    ext_thiem_3d
    ext_thiem_tpl
    ext_thiem_tpl_3d
@@ -46,16 +45,14 @@
    ext_thiem_tpl_3d
    neuman2004
    neuman2004_steady
 
 Extended GRF
 ^^^^^^^^^^^^
 
-.. currentmodule:: anaflow.flow.ext_grf_model
-
 The extended general radial flow model.
 
 .. autosummary::
    ext_grf
    ext_grf_steady
 
 Laplace
@@ -76,40 +73,38 @@
 
 Helping functions.
 
 .. autosummary::
    step_f
    specialrange
    specialrange_cut
-
-
 """
 from anaflow.flow import (
-    thiem,
-    theis,
-    grf,
-    ext_thiem_2d,
-    ext_thiem_3d,
-    ext_thiem_tpl,
-    ext_thiem_tpl_3d,
+    ext_grf,
+    ext_grf_steady,
     ext_theis_2d,
     ext_theis_3d,
     ext_theis_tpl,
     ext_theis_tpl_3d,
+    ext_thiem_2d,
+    ext_thiem_3d,
+    ext_thiem_tpl,
+    ext_thiem_tpl_3d,
+    grf,
     neuman2004,
     neuman2004_steady,
-    ext_grf,
-    ext_grf_steady,
+    theis,
+    thiem,
 )
 from anaflow.tools import (
-    get_lap_inv,
     get_lap,
-    step_f,
+    get_lap_inv,
     specialrange,
     specialrange_cut,
+    step_f,
 )
 
 try:
     from anaflow._version import __version__
 except ImportError:  # pragma: nocover
     # package is not installed
     __version__ = "0.0.0.dev0"
```

### Comparing `anaflow-1.0.1/anaflow/flow/__init__.py` & `anaflow-1.1.0/src/anaflow/flow/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,86 +1,83 @@
-# -*- coding: utf-8 -*-
 """
 Anaflow subpackage providing flow-solutions for the groundwater flow equation.
 
 Subpackages
 ^^^^^^^^^^^
 
 .. currentmodule:: anaflow.flow
 
 .. autosummary::
-    homogeneous
-    heterogeneous
-    ext_grf_model
-    laplace
+   :toctree:
+
+   laplace
 
 Solutions
 ^^^^^^^^^
 
 Homogeneous
 ~~~~~~~~~~~
 
-.. currentmodule:: anaflow.flow.homogeneous
-
 Solutions for homogeneous aquifers
 
 .. autosummary::
+   :toctree:
+
    thiem
    theis
    grf
 
 Heterogeneous
 ~~~~~~~~~~~~~
 
-.. currentmodule:: anaflow.flow.heterogeneous
-
 Solutions for heterogeneous aquifers
 
 .. autosummary::
+   :toctree:
+
    ext_thiem_2d
    ext_thiem_3d
    ext_thiem_tpl
    ext_thiem_tpl_3d
    ext_theis_2d
    ext_theis_3d
    ext_theis_tpl
-   ext_thiem_tpl_3d
+   ext_theis_tpl_3d
    neuman2004
    neuman2004_steady
 
 Extended GRF
 ~~~~~~~~~~~~
 
-.. currentmodule:: anaflow.flow.ext_grf_model
-
 The extended general radial flow model.
 
 .. autosummary::
+   :toctree:
+
    ext_grf
    ext_grf_steady
 """
-from anaflow.flow.homogeneous import thiem, theis, grf
+from anaflow.flow.ext_grf_model import ext_grf, ext_grf_steady
 from anaflow.flow.heterogeneous import (
-    ext_thiem_2d,
-    ext_thiem_3d,
-    ext_thiem_tpl,
-    ext_thiem_tpl_3d,
     ext_theis_2d,
     ext_theis_3d,
     ext_theis_tpl,
     ext_theis_tpl_3d,
+    ext_thiem_2d,
+    ext_thiem_3d,
+    ext_thiem_tpl,
+    ext_thiem_tpl_3d,
     neuman2004,
     neuman2004_steady,
 )
-from anaflow.flow.ext_grf_model import ext_grf, ext_grf_steady
+from anaflow.flow.homogeneous import grf, theis, thiem
 
 __all__ = [
     "thiem",
     "theis",
-    "grf_model",
     "ext_thiem_2d",
     "ext_thiem_3d",
     "ext_thiem_tpl",
     "ext_thiem_tpl_3d",
     "ext_theis_2d",
     "ext_theis_3d",
     "ext_theis_tpl",
```

### Comparing `anaflow-1.0.1/anaflow/flow/ext_grf_model.py` & `anaflow-1.1.0/src/anaflow/flow/ext_grf_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 Anaflow subpackage providing the extended GRF Model.
 
 .. currentmodule:: anaflow.flow.ext_grf_model
 
 The following functions are provided
 
@@ -10,16 +9,16 @@
    ext_grf
    ext_grf_steady
 """
 # pylint: disable=C0103
 import numpy as np
 from scipy.integrate import quad as integ
 
-from anaflow.tools.laplace import get_lap_inv
 from anaflow.flow.laplace import grf_laplace
+from anaflow.tools.laplace import get_lap_inv
 from anaflow.tools.special import Shaper, sph_surf
 
 __all__ = ["ext_grf", "ext_grf_steady"]
 
 
 def ext_grf(
     time,
@@ -119,15 +118,15 @@
     r_ref,
     conductivity,
     dim=2,
     lat_ext=1.0,
     rate=-1e-4,
     h_ref=0.0,
     arg_dict=None,
-    **kwargs
+    **kwargs,
 ):
     """
     The extended "General radial flow" model for steady flow.
 
     The general radial flow (GRF) model by Barker introduces an arbitrary
     dimension for radial groundwater flow. We introduced the possibility to
     define radial dependet conductivity.
@@ -172,35 +171,35 @@
        in fractured rock.'',
        Water Resources Research 24.10, 1796-1804, 1988
     """
     arg_dict = {} if arg_dict is None else arg_dict
     kwargs.update(arg_dict)
     Input = Shaper(rad=rad)
     q_fac = rate / (sph_surf(dim) * lat_ext ** (3.0 - dim))  # pumping factor
-    if not r_ref > 0.0:
+    if r_ref <= 0.0:
         raise ValueError("The reference radius needs to be positive.")
-    if not Input.rad_min > 0.0:
+    if Input.rad_min <= 0.0:
         raise ValueError("The given radii need to be positive.")
-    if not dim > 0.0 or dim > 3.0:
+    if dim <= 0.0 or dim > 3.0:
         raise ValueError("The dimension needs to be positiv and <= 3.")
-    if not lat_ext > 0.0:
+    if lat_ext <= 0.0:
         raise ValueError("The lateral extend needs to be positiv.")
 
     if callable(conductivity):
         res = np.zeros(Input.rad_no)
 
         def integrand(val):
             """Integrand."""
             return val ** (1 - dim) / conductivity(val, **kwargs)
 
         for ri, re in enumerate(Input.rad):
             res[ri] = integ(integrand, re, r_ref)[0]
     else:
         con = float(conductivity)
-        if not con > 0:
+        if con <= 0:
             raise ValueError("The Conductivity needs to be positive.")
         if np.isclose(dim, 2):
             res = np.log(r_ref / Input.rad) / con
         else:
             res = (
                 (r_ref ** (2 - dim) - Input.rad ** (2 - dim)) / (2 - dim) / con
             )
```

### Comparing `anaflow-1.0.1/anaflow/flow/heterogeneous.py` & `anaflow-1.1.0/src/anaflow/flow/heterogeneous.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 Anaflow subpackage providing flow solutions in heterogeneous aquifers.
 
 .. currentmodule:: anaflow.flow.heterogeneous
 
 The following functions are provided
 
@@ -14,31 +13,31 @@
    ext_theis_2d
    ext_theis_3d
    ext_theis_tpl
    ext_theis_tpl_3d
    neuman2004
    neuman2004_steady
 """
-# pylint: disable=C0103
+# pylint: disable=C0103,C0302
 import functools as ft
 
 import numpy as np
 from scipy.special import exp1, expi
 
-from anaflow.tools.special import aniso, specialrange_cut, neuman2004_trans
-from anaflow.tools.mean import annular_hmean
+from anaflow.flow.ext_grf_model import ext_grf, ext_grf_steady
 from anaflow.tools.coarse_graining import (
-    T_CG,
-    T_CG_error,
     K_CG,
-    K_CG_error,
+    T_CG,
     TPL_CG,
+    K_CG_error,
+    T_CG_error,
     TPL_CG_error,
 )
-from anaflow.flow.ext_grf_model import ext_grf, ext_grf_steady
+from anaflow.tools.mean import annular_hmean
+from anaflow.tools.special import aniso, neuman2004_trans, specialrange_cut
 
 __all__ = [
     "ext_thiem_2d",
     "ext_thiem_3d",
     "ext_thiem_tpl",
     "ext_thiem_tpl_3d",
     "ext_theis_2d",
@@ -70,14 +69,15 @@
     The extended Thiem solution in 2D.
 
     The extended Thiem solution for steady-state flow under
     a pumping condition in a confined aquifer.
     The type curve is describing the effective drawdown
     in a 2D statistical framework, where the transmissivity distribution is
     following a log-normal distribution with a gaussian correlation function.
+    Presented in [Zech2013]_.
 
     Parameters
     ----------
     rad : :class:`numpy.ndarray`
         Array with all radii where the function should be evaluated
     r_ref : :class:`float`
         Radius of the reference head.
@@ -142,18 +142,18 @@
     if prop <= 0.0:
         raise ValueError("The proportionalityfactor needs to be positive.")
 
     # define some substitions to shorten the result
     chi = -var / 2.0 if T_well is None else np.log(T_well / trans_gmean)
     C = (prop / len_scale) ** 2
     # derive the result
-    res = -expi(-chi / (1.0 + C * rad ** 2))
-    res -= np.exp(-chi) * exp1(chi / (1.0 + C * rad ** 2) - chi)
-    res += expi(-chi / (1.0 + C * r_ref ** 2))
-    res += np.exp(-chi) * exp1(chi / (1.0 + C * r_ref ** 2) - chi)
+    res = -expi(-chi / (1.0 + C * rad**2))
+    res -= np.exp(-chi) * exp1(chi / (1.0 + C * rad**2) - chi)
+    res += expi(-chi / (1.0 + C * r_ref**2))
+    res += np.exp(-chi) * exp1(chi / (1.0 + C * r_ref**2) - chi)
     res *= -rate / (4.0 * np.pi * trans_gmean)
     res += h_ref
     return res
 
 
 ###############################################################################
 # 3D version of extended Thiem
@@ -178,14 +178,15 @@
 
     The extended Thiem solution for steady-state flow under
     a pumping condition in a confined aquifer.
     The type curve is describing the effective drawdown
     in a 3D statistical framework, where the conductivity distribution is
     following a log-normal distribution with a gaussian correlation function
     and taking vertical anisotropy into account.
+    Presented in [Zech2013]_.
 
     Parameters
     ----------
     rad : :class:`numpy.ndarray`
         Array with all radii where the function should be evaluated
     r_ref : :class:`float`
         Reference radius with known head (see `h_ref`)
@@ -234,57 +235,57 @@
     Examples
     --------
     >>> ext_thiem_3d([1,2,3], 10, 0.001, 1, 10, 1, 1, -0.001)
     array([-0.48828026, -0.31472059, -0.22043022])
     """
     rad = np.array(rad, dtype=float)
     # check the input
-    if not r_ref > 0.0:
+    if r_ref <= 0.0:
         raise ValueError("The reference radius needs to be positive.")
-    if not np.min(rad) > 0.0:
+    if np.min(rad) <= 0.0:
         raise ValueError("The given radii need to be positive.")
     if K_well != "KA" and K_well != "KH" and not isinstance(K_well, float):
         raise ValueError(
             "The well-conductivity should be given as float or 'KA' resp 'KH'"
         )
     if isinstance(K_well, float) and K_well <= 0.0:
         raise ValueError("The well-conductivity needs to be positive.")
-    if not cond_gmean > 0.0:
+    if cond_gmean <= 0.0:
         raise ValueError("The gmean conductivity needs to be positive.")
     if var < 0.0:
         raise ValueError("The variance needs to be positive.")
-    if not len_scale > 0.0:
+    if len_scale <= 0.0:
         raise ValueError("The correlationlength needs to be positive.")
-    if not lat_ext > 0.0:
+    if lat_ext <= 0.0:
         raise ValueError("The aquifer-thickness needs to be positive.")
     if not 0.0 < anis <= 1.0:
         raise ValueError("The anisotropy-ratio must be > 0 and <= 1")
-    if not prop > 0.0:
+    if prop <= 0.0:
         raise ValueError("The proportionalityfactor needs to be positive.")
 
     # define some substitions to shorten the result
     K_efu = cond_gmean * np.exp(var * (0.5 - aniso(anis)))
     if K_well == "KH":
         chi = var * (aniso(anis) - 1.0)
     elif K_well == "KA":
         chi = var * aniso(anis)
     else:
         chi = np.log(K_well / K_efu)
 
     C = (prop / len_scale / anis ** (1.0 / 3.0)) ** 2
 
-    sub11 = np.sqrt(1.0 + C * r_ref ** 2)
-    sub12 = np.sqrt(1.0 + C * rad ** 2)
+    sub11 = np.sqrt(1.0 + C * r_ref**2)
+    sub12 = np.sqrt(1.0 + C * rad**2)
 
     sub21 = np.log(sub12 + 1.0) - np.log(sub11 + 1.0)
     sub21 -= 1.0 / sub12 - 1.0 / sub11
 
     sub22 = np.log(sub12) - np.log(sub11)
-    sub22 -= 0.50 / sub12 ** 2 - 0.50 / sub11 ** 2
-    sub22 -= 0.25 / sub12 ** 4 - 0.25 / sub11 ** 4
+    sub22 -= 0.50 / sub12**2 - 0.50 / sub11**2
+    sub22 -= 0.25 / sub12**4 - 0.25 / sub11**4
 
     # derive the result
     res = np.exp(-chi) * (np.log(rad) - np.log(r_ref))
     res += sub21 * np.sinh(chi) + sub22 * (1.0 - np.cosh(chi))
     res *= -rate / (2.0 * np.pi * K_efu * lat_ext)
     res += h_ref
 
@@ -385,27 +386,27 @@
     array([[-0.33737576, -0.17400123, -0.09489812],
            [-0.58443489, -0.40847176, -0.31095166]])
     """
     lap_kwargs = {} if lap_kwargs is None else lap_kwargs
     # check the input
     if r_well < 0.0:
         raise ValueError("The wellradius needs to be >= 0")
-    if not r_bound > r_well:
+    if r_bound <= r_well:
         raise ValueError("The upper boundary needs to be > well radius")
-    if not storage > 0.0:
+    if storage <= 0.0:
         raise ValueError("The Storage needs to be positive.")
-    if not trans_gmean > 0.0:
+    if trans_gmean <= 0.0:
         raise ValueError("The Transmissivity needs to be positive.")
     if var < 0.0:
         raise ValueError("The variance needs to be positive.")
-    if not len_scale > 0.0:
+    if len_scale <= 0.0:
         raise ValueError("The correlationlength needs to be positive.")
-    if T_well is not None and not T_well > 0.0:
+    if T_well is not None and T_well <= 0.0:
         raise ValueError("The well Transmissivity needs to be positive.")
-    if not prop > 0.0:
+    if prop <= 0.0:
         raise ValueError("The proportionality factor needs to be positive.")
     if parts <= 1:
         raise ValueError("The numbor of partitions needs to be at least 2")
     if not 0.0 < far_err < 1.0:
         raise ValueError(
             "The relative error of Transmissivity needs to be within (0,1)"
         )
@@ -541,33 +542,33 @@
     >>> ext_theis_3d([10,100], [1,2,3], 0.001, 0.001, 1, 10, 1, 1, -0.001)
     array([[-0.32756786, -0.16717569, -0.09141211],
            [-0.5416396 , -0.36982684, -0.27798614]])
     """
     # check the input
     if r_well < 0.0:
         raise ValueError("The wellradius needs to be >= 0")
-    if not r_bound > r_well:
+    if r_bound <= r_well:
         raise ValueError("The upper boundary needs to be > well radius")
-    if not storage > 0.0:
+    if storage <= 0.0:
         raise ValueError("The storage needs to be positive.")
-    if not cond_gmean > 0.0:
+    if cond_gmean <= 0.0:
         raise ValueError("The gmean conductivity needs to be positive.")
     if var < 0.0:
         raise ValueError("The variance needs to be positive.")
-    if not len_scale > 0.0:
+    if len_scale <= 0.0:
         raise ValueError("The correlationlength needs to be positive.")
     if K_well != "KA" and K_well != "KH" and not isinstance(K_well, float):
         raise ValueError(
             "The well-conductivity should be given as float or 'KA' resp 'KH'"
         )
-    if isinstance(K_well, float) and not K_well > 0.0:
+    if isinstance(K_well, float) and K_well <= 0.0:
         raise ValueError("The well-conductivity needs to be positive.")
-    if not cond_gmean > 0.0:
+    if cond_gmean <= 0.0:
         raise ValueError("The conductivity needs to be positive.")
-    if not prop > 0.0:
+    if prop <= 0.0:
         raise ValueError("The proportionality factor needs to be positive.")
     if parts <= 1:
         raise ValueError("The numbor of partitions needs to be at least 2")
     if not 0.0 < far_err < 1.0:
         raise ValueError(
             "The relative error of Conductivity needs to be within (0,1)"
         )
@@ -723,35 +724,35 @@
     -----
     If you want to use cartesian coordiantes, just use the formula
     ``r = sqrt(x**2 + y**2)``
     """
     # check the input
     if r_well < 0.0:
         raise ValueError("The wellradius needs to be >= 0")
-    if not r_bound > r_well:
+    if r_bound <= r_well:
         raise ValueError("The upper boundary needs to be > well radius")
-    if not storage > 0.0:
+    if storage <= 0.0:
         raise ValueError("The storage needs to be positive.")
-    if not cond_gmean > 0.0:
+    if cond_gmean <= 0.0:
         raise ValueError("The gmean conductivity needs to be positive.")
-    if not len_scale > 0.0:
+    if len_scale <= 0.0:
         raise ValueError("The correlationlength needs to be positive.")
     if not 0 < hurst < 1:
         raise ValueError("Hurst coefficient needs to be in (0,1)")
     if var is not None and var < 0.0:
         raise ValueError("The variance needs to be positive.")
-    if var is None and not c > 0.0:
+    if var is None and c <= 0.0:
         raise ValueError("The intensity of variation needs to be positive.")
     if K_well != "KA" and K_well != "KH" and not isinstance(K_well, float):
         raise ValueError(
             "The well-conductivity should be given as float or 'KA' resp 'KH'"
         )
-    if isinstance(K_well, float) and not K_well > 0.0:
+    if isinstance(K_well, float) and K_well <= 0.0:
         raise ValueError("The well-conductivity needs to be positive.")
-    if not prop > 0.0:
+    if prop <= 0.0:
         raise ValueError("The proportionality factor needs to be positive.")
     if parts <= 1:
         raise ValueError("The numbor of partitions needs to be at least 2")
     if not 0.0 < far_err < 1.0:
         raise ValueError(
             "The relative error of Conductivity needs to be within (0,1)"
         )
@@ -902,35 +903,35 @@
     -----
     If you want to use cartesian coordiantes, just use the formula
     ``r = sqrt(x**2 + y**2)``
     """
     # check the input
     if r_well < 0.0:
         raise ValueError("The wellradius needs to be >= 0")
-    if not r_bound > r_well:
+    if r_bound <= r_well:
         raise ValueError("The upper boundary needs to be > well radius")
-    if not storage > 0.0:
+    if storage <= 0.0:
         raise ValueError("The storage needs to be positive.")
-    if not cond_gmean > 0.0:
+    if cond_gmean <= 0.0:
         raise ValueError("The gmean conductivity needs to be positive.")
-    if not len_scale > 0.0:
+    if len_scale <= 0.0:
         raise ValueError("The correlationlength needs to be positive.")
     if not 0 < hurst < 1:
         raise ValueError("Hurst coefficient needs to be in (0,1)")
     if var is not None and var < 0.0:
         raise ValueError("The variance needs to be positive.")
-    if var is None and not c > 0.0:
+    if var is None and c <= 0.0:
         raise ValueError("The intensity of variation needs to be positive.")
     if K_well != "KA" and K_well != "KH" and not isinstance(K_well, float):
         raise ValueError(
             "The well-conductivity should be given as float or 'KA' resp 'KH'"
         )
-    if isinstance(K_well, float) and not K_well > 0.0:
+    if isinstance(K_well, float) and K_well <= 0.0:
         raise ValueError("The well-conductivity needs to be positive.")
-    if not prop > 0.0:
+    if prop <= 0.0:
         raise ValueError("The proportionality factor needs to be positive.")
     if parts <= 1:
         raise ValueError("The numbor of partitions needs to be at least 2")
     if not 0.0 < far_err < 1.0:
         raise ValueError(
             "The relative error of Conductivity needs to be within (0,1)"
         )
@@ -1054,31 +1055,31 @@
 
     Notes
     -----
     If you want to use cartesian coordiantes, just use the formula
     ``r = sqrt(x**2 + y**2)``
     """
     # check the input
-    if not cond_gmean > 0.0:
+    if cond_gmean <= 0.0:
         raise ValueError("The gmean conductivity needs to be positive.")
-    if not len_scale > 0.0:
+    if len_scale <= 0.0:
         raise ValueError("The correlationlength needs to be positive.")
     if not 0 < hurst < 1:
         raise ValueError("Hurst coefficient needs to be in (0,1)")
     if var is not None and var < 0.0:
         raise ValueError("The variance needs to be positive.")
-    if var is None and not c > 0.0:
+    if var is None and c <= 0.0:
         raise ValueError("The intensity of variation needs to be positive.")
     if K_well != "KA" and K_well != "KH" and not isinstance(K_well, float):
         raise ValueError(
             "The well-conductivity should be given as float or 'KA' resp 'KH'"
         )
-    if isinstance(K_well, float) and not K_well > 0.0:
+    if isinstance(K_well, float) and K_well <= 0.0:
         raise ValueError("The well-conductivity needs to be positive.")
-    if not prop > 0.0:
+    if prop <= 0.0:
         raise ValueError("The proportionality factor needs to be positive.")
     cond = ft.partial(
         TPL_CG,
         cond_gmean=cond_gmean,
         len_scale=len_scale,
         hurst=hurst,
         var=var,
@@ -1194,31 +1195,31 @@
 
     Notes
     -----
     If you want to use cartesian coordiantes, just use the formula
     ``r = sqrt(x**2 + y**2)``
     """
     # check the input
-    if not cond_gmean > 0.0:
+    if cond_gmean <= 0.0:
         raise ValueError("The gmean conductivity needs to be positive.")
-    if not len_scale > 0.0:
+    if len_scale <= 0.0:
         raise ValueError("The correlationlength needs to be positive.")
     if not 0 < hurst < 1:
         raise ValueError("Hurst coefficient needs to be in (0,1)")
     if var is not None and var < 0.0:
         raise ValueError("The variance needs to be positive.")
-    if var is None and not c > 0.0:
+    if var is None and c <= 0.0:
         raise ValueError("The intensity of variation needs to be positive.")
     if K_well != "KA" and K_well != "KH" and not isinstance(K_well, float):
         raise ValueError(
             "The well-conductivity should be given as float or 'KA' resp 'KH'"
         )
-    if isinstance(K_well, float) and not K_well > 0.0:
+    if isinstance(K_well, float) and K_well <= 0.0:
         raise ValueError("The well-conductivity needs to be positive.")
-    if not prop > 0.0:
+    if prop <= 0.0:
         raise ValueError("The proportionality factor needs to be positive.")
     cond = ft.partial(
         TPL_CG,
         cond_gmean=cond_gmean,
         len_scale=len_scale,
         hurst=hurst,
         var=var,
@@ -1261,14 +1262,15 @@
 ):
     """
     The transient solution for the apparent transmissivity from [Neuman2004].
 
     This solution is build on the apparent transmissivity from Neuman 2004,
     which represents a mean drawdown in an ensemble of pumping tests in
     heterogeneous transmissivity fields following an exponential covariance.
+    Presented in [Neuman2004]_.
 
     Parameters
     ----------
     time : :class:`numpy.ndarray`
         Array with all time-points where the function should be evaluated.
     rad : :class:`numpy.ndarray`
         Array with all radii where the function should be evaluated.
@@ -1314,23 +1316,23 @@
     .. [Neuman2004] Neuman, Shlomo P., Alberto Guadagnini, and Monica Riva.
        ''Type-curve estimation of statistical heterogeneity.''
        Water resources research 40.4, 2004
     """
     # check the input
     if r_well < 0.0:
         raise ValueError("The wellradius needs to be >= 0")
-    if not r_bound > r_well:
+    if r_bound <= r_well:
         raise ValueError("The upper boundary needs to be > well radius")
-    if not storage > 0.0:
+    if storage <= 0.0:
         raise ValueError("The Storage needs to be positive.")
-    if not trans_gmean > 0.0:
+    if trans_gmean <= 0.0:
         raise ValueError("The Transmissivity needs to be positive.")
     if var < 0.0:
         raise ValueError("The variance needs to be positive.")
-    if not len_scale > 0.0:
+    if len_scale <= 0.0:
         raise ValueError("The correlationlength needs to be positive.")
     if parts <= 1:
         raise ValueError("The numbor of partitions needs to be at least 2")
     # genearte rlast from a given relativ-error to farfield-transmissivity
     r_last = 2 * len_scale
     # generate the partition points
     if r_last > r_well:
@@ -1367,14 +1369,15 @@
 ):
     """
     The steady solution for the apparent transmissivity from [Neuman2004].
 
     This solution is build on the apparent transmissivity from Neuman 1994,
     which represents a mean drawdown in an ensemble of pumping tests in
     heterogeneous transmissivity fields following an exponential covariance.
+    Presented in [Neuman2004]_.
 
     Parameters
     ----------
     rad : :class:`numpy.ndarray`
         Array with all radii where the function should be evaluated
     r_ref : :class:`float`
         Radius of the reference head.
@@ -1397,19 +1400,19 @@
     References
     ----------
     .. [Neuman2004] Neuman, Shlomo P., Alberto Guadagnini, and Monica Riva.
        ''Type-curve estimation of statistical heterogeneity.''
        Water resources research 40.4, 2004
     """
     # check the input
-    if not trans_gmean > 0.0:
+    if trans_gmean <= 0.0:
         raise ValueError("The Transmissivity needs to be positive.")
     if var < 0.0:
         raise ValueError("The variance needs to be positive.")
-    if not len_scale > 0.0:
+    if len_scale <= 0.0:
         raise ValueError("The correlationlength needs to be positive.")
 
     return ext_grf_steady(
         rad=rad,
         r_ref=r_ref,
         conductivity=neuman2004_trans,
         dim=2,
```

### Comparing `anaflow-1.0.1/anaflow/flow/homogeneous.py` & `anaflow-1.1.0/src/anaflow/flow/homogeneous.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 Anaflow subpackage providing flow solutions in homogeneous aquifers.
 
 .. currentmodule:: anaflow.flow.homogeneous
 
 The following functions are provided
 
@@ -10,16 +9,16 @@
    thiem
    theis
    grf
 """
 # pylint: disable=C0103
 import numpy as np
 
-from anaflow.tools.special import well_solution, grf_solution
 from anaflow.flow.ext_grf_model import ext_grf, ext_grf_steady
+from anaflow.tools.special import grf_solution, well_solution
 
 __all__ = ["thiem", "theis", "grf"]
 
 
 ###############################################################################
 # Thiem-solution
 ###############################################################################
```

### Comparing `anaflow-1.0.1/anaflow/flow/laplace.py` & `anaflow-1.1.0/src/anaflow/flow/laplace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-# -*- coding: utf-8 -*-
 """
 Anaflow subpackage providing flow solutions in laplace space.
 
 .. currentmodule:: anaflow.flow.laplace
 
 The following functions are provided
 
 .. autosummary::
+   :toctree:
+
    grf_laplace
 """
-# pylint: disable=C0103
+# pylint: disable=C0103,R0915
 import warnings
 
 import numpy as np
-from scipy.special import kv, iv, gamma, erfcx
 from pentapy import solve
+from scipy.special import erfcx, gamma, iv, kv
+
 from anaflow.tools.special import sph_surf
 
 __all__ = ["grf_laplace"]
 
 
 def constant(s):
     """Constant pumping."""
@@ -29,15 +31,15 @@
     """
     Periodic pumping.
 
     Q(t) = Q * cos(a * t)
     """
     if np.isclose(a, 0):
         return constant(s)
-    return 1.0 / (s + a ** 2 / s)
+    return 1.0 / (s + a**2 / s)
 
 
 def slug(s):
     """Slug test."""
     return np.ones_like(s)
 
 
@@ -146,27 +148,27 @@
     # set the conductivity at the well
     K_well = K_part[0] if K_well is None else float(K_well)
     # check the input
     if not len(R_part) - 1 == len(S_part) == len(K_part) > 0:
         raise ValueError("R_part, S_part and K_part need matching lengths.")
     if R_part[0] < 0.0:
         raise ValueError("The wellradius needs to be >= 0.")
-    if not all([r1 < r2 for r1, r2 in zip(R_part[:-1], R_part[1:])]):
+    if not all(r1 < r2 for r1, r2 in zip(R_part[:-1], R_part[1:])):
         raise ValueError("The radii values need to be sorted.")
     if not np.min(rad) > R_part[0] or np.max(rad) > R_part[-1]:
         raise ValueError("The given radii need to be in the given range.")
-    if not all([con > 0 for con in K_part]):
+    if not all(con > 0 for con in K_part):
         raise ValueError("The Conductivity needs to be positiv.")
-    if not all([stor > 0 for stor in S_part]):
+    if not all(stor > 0 for stor in S_part):
         raise ValueError("The Storage needs to be positiv.")
-    if not dim > 0.0 or dim > 3.0:
+    if dim <= 0.0 or dim > 3.0:
         raise ValueError("The dimension needs to be positiv and <= 3.")
-    if not lat_ext > 0.0:
+    if lat_ext <= 0.0:
         raise ValueError("The lateral extend needs to be positiv.")
-    if not K_well > 0:
+    if K_well <= 0:
         raise ValueError("The well conductivity needs to be positiv.")
 
     # initialize the result
     res = np.zeros(s.shape + rad.shape)
     # the first sqrt of the diffusivity values
     diff_sr0 = np.sqrt(S_part[0] / K_part[0])
     # set the general pumping-condtion depending on the well-radius
@@ -194,15 +196,15 @@
                 M[0, 1] = 0  # Bs is 0 in this case either way
             # solve the equation system
             As, Bs = np.linalg.solve(M, V)
 
             # calculate the head
             for ri, re in enumerate(rad):
                 if re < R_part[-1]:
-                    res[si, ri] = re ** nu * (
+                    res[si, ri] = re**nu * (
                         As * kv(nu, Cs * re) + Bs * iv(nu, Cs * re)
                     )
 
     # if there is more than one partition, create an equation system
     else:
         # initialize LHS and RHS for the linear equation system
         # Mb is the banded matrix for the Eq-System
@@ -296,15 +298,15 @@
             # calculate the head (ignore small values)
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore", RuntimeWarning)
                 k0_sub = X[2 * pos] * kv(nu, Cs[pos] * rad)
                 k0_sub[np.abs(X[2 * pos]) < cut_off_prec] = 0
                 i0_sub = X[2 * pos + 1] * iv(nu, Cs[pos] * rad)
                 i0_sub[np.abs(X[2 * pos + 1]) < cut_off_prec] = 0
-                res[si, :] = rad ** nu * (k0_sub + i0_sub)
+                res[si, :] = rad**nu * (k0_sub + i0_sub)
 
     # set problematic values to 0
     # --> the algorithm tends to violate small values,
     #     therefore this approach is suitable
     np.nan_to_num(res, copy=False)
     # scale to pumpingrate
     res *= rate / (K_well * sph_surf(dim) * lat_ext ** (3.0 - dim))
```

### Comparing `anaflow-1.0.1/anaflow/tools/__init__.py` & `anaflow-1.1.0/src/anaflow/tools/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-# -*- coding: utf-8 -*-
 """
 Anaflow subpackage providing miscellaneous tools.
 
 Subpackages
 ^^^^^^^^^^^
 
 .. currentmodule:: anaflow.tools
 
 .. autosummary::
-    laplace
-    mean
-    special
-    coarse_graining
+   :toctree:
+
+   laplace
+   mean
+   special
+   coarse_graining
 
 Functions
 ^^^^^^^^^
 
 Annular mean
 ~~~~~~~~~~~~
 
@@ -63,30 +64,30 @@
 
 Helping functions related to the laplace-transformation
 
 .. autosummary::
    get_lap
    get_lap_inv
 """
+from anaflow.tools.coarse_graining import K_CG, T_CG, TPL_CG
+from anaflow.tools.laplace import get_lap, get_lap_inv
 from anaflow.tools.mean import (
-    annular_fmean,
     annular_amean,
+    annular_fmean,
     annular_gmean,
     annular_hmean,
     annular_pmean,
 )
 from anaflow.tools.special import (
-    step_f,
+    aniso,
+    neuman2004_trans,
     specialrange,
     specialrange_cut,
-    neuman2004_trans,
-    aniso,
+    step_f,
 )
-from anaflow.tools.coarse_graining import T_CG, K_CG, TPL_CG
-from anaflow.tools.laplace import get_lap, get_lap_inv
 
 __all__ = [
     "get_lap",
     "get_lap_inv",
     "annular_fmean",
     "annular_amean",
     "annular_gmean",
```

### Comparing `anaflow-1.0.1/anaflow/tools/coarse_graining.py` & `anaflow-1.1.0/src/anaflow/tools/coarse_graining.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# -*- coding: utf-8 -*-
 """
 Anaflow subpackage providing helper functions related to coarse graining.
 
 .. currentmodule:: anaflow.tools.coarse_graining
 
 The following functions are provided
 
 .. autosummary::
+   :toctree:
 
    T_CG
    T_CG_inverse
    T_CG_error
    K_CG
    K_CG_inverse
    K_CG_error
```

### Comparing `anaflow-1.0.1/anaflow/tools/laplace.py` & `anaflow-1.1.0/src/anaflow/tools/laplace.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-# -*- coding: utf-8 -*-
 """
 Anaflow subpackage providing functions concerning the laplace transformation.
 
 .. currentmodule:: anaflow.tools.laplace
 
 The following functions are provided
 
 .. autosummary::
+   :toctree:
 
    get_lap
    get_lap_inv
    lap_trans
    stehfest
 """
-from math import floor, factorial
+from math import factorial, floor
+
 import numpy as np
 from scipy.integrate import quad
 
 __all__ = ["get_lap", "lap_trans", "get_lap_inv", "stehfest"]
 
 
 def get_lap(func, arg_dict=None, **kwargs):
@@ -117,15 +118,14 @@
         def integrand(val):
             """Integrand for the laplace transform."""
             return np.exp(-phase * val) * func(val, **kwargs)
 
         return integrand
 
     for phase_i, phase_e in np.ndenumerate(phase):
-
         integ = make_integrand(phase_e)
         result[phase_i] = quad(integ, 0, np.inf)[0]
 
     if is_scal:
         result = result.item()
 
     return result
```

### Comparing `anaflow-1.0.1/anaflow/tools/mean.py` & `anaflow-1.1.0/src/anaflow/tools/mean.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-# -*- coding: utf-8 -*-
 """
 Anaflow subpackage providing several mean calculating routines.
 
 .. currentmodule:: anaflow.tools.mean
 
 The following functions are provided
 
 .. autosummary::
+   :toctree:
 
    annular_fmean
    annular_amean
    annular_gmean
    annular_hmean
    annular_pmean
 """
 # pylint: disable=E1137, C0103
 import numpy as np
-
 from scipy.integrate import quad as integ
 
 __all__ = [
     "annular_fmean",
     "annular_amean",
     "annular_gmean",
     "annular_hmean",
@@ -188,15 +187,15 @@
     return annular_fmean(
         func=func,
         val_arr=val_arr,
         f_def=lambda x: x,
         f_inv=lambda x: x,
         ann_dim=ann_dim,
         arg_dict=arg_dict,
-        **kwargs
+        **kwargs,
     )
 
 
 def annular_gmean(func, val_arr, ann_dim=2, arg_dict=None, **kwargs):
     r"""
     Calculating the annular geometric mean.
 
@@ -256,15 +255,15 @@
     return annular_fmean(
         func=func,
         val_arr=val_arr,
         f_def=np.log,
         f_inv=np.exp,
         ann_dim=ann_dim,
         arg_dict=arg_dict,
-        **kwargs
+        **kwargs,
     )
 
 
 def annular_hmean(func, val_arr, ann_dim=2, arg_dict=None, **kwargs):
     r"""
     Calculating the annular harmonic mean.
 
@@ -318,15 +317,15 @@
     return annular_fmean(
         func=func,
         val_arr=val_arr,
         f_def=lambda x: 1.0 / x,
         f_inv=lambda x: 1.0 / x,
         ann_dim=ann_dim,
         arg_dict=arg_dict,
-        **kwargs
+        **kwargs,
     )
 
 
 def annular_pmean(func, val_arr, p=2.0, ann_dim=2, arg_dict=None, **kwargs):
     r"""
     Calculating the annular p-mean.
 
@@ -388,9 +387,9 @@
     return annular_fmean(
         func=func,
         val_arr=val_arr,
         f_def=lambda x: np.power(x, p),
         f_inv=lambda x: np.power(x, 1.0 / p),
         ann_dim=ann_dim,
         arg_dict=arg_dict,
-        **kwargs
+        **kwargs,
     )
```

### Comparing `anaflow-1.0.1/anaflow/tools/special.py` & `anaflow-1.1.0/src/anaflow/tools/special.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# -*- coding: utf-8 -*-
 """
 Anaflow subpackage providing special functions.
 
 .. currentmodule:: anaflow.tools.special
 
 The following functions are provided
 
 .. autosummary::
+   :toctree:
 
    Shaper
    step_f
    sph_surf
    specialrange
    specialrange_cut
    aniso
    well_solution
    grf_solution
    inc_gamma
    tpl_hyp
    neuman2004_trans
 """
-
+# pylint: disable=C0103,R0903
 import numpy as np
-from scipy.special import gamma, gammaincc, exp1, expn, hyp2f1
+from scipy.special import exp1, expn, gamma, gammaincc, hyp2f1
 
 __all__ = [
     "Shaper",
     "step_f",
     "sph_surf",
     "specialrange",
     "specialrange_cut",
@@ -35,15 +35,15 @@
     "grf_solution",
     "inc_gamma",
     "tpl_hyp",
     "neuman2004_trans",
 ]
 
 
-class Shaper(object):
+class Shaper:
     """
     A class to reshape radius-time input-output in a good way.
 
     Parameters
     ----------
     time : :class:`numpy.ndarray` or :class:`float`, optional
         Array with all time-points where the function should be evaluated.
@@ -80,15 +80,15 @@
         self.time_mat = np.outer(
             self.time[self.time_gz], np.ones_like(self.rad)
         )
         self.rad_mat = np.outer(
             np.ones_like(self.time[self.time_gz]), self.rad
         )
 
-        if not self.struc_grid and not self.rad_shape == self.time_shape:
+        if not self.struc_grid and self.rad_shape != self.time_shape:
             raise ValueError("No struc_grid: shape of time & radius differ")
         if np.any(self.time < 0.0):
             raise ValueError("The given times need to be positive.")
         if np.any(self.rad <= 0.0):
             raise ValueError("The given radii need to be non-negative.")
 
     def reshape(self, result):
@@ -179,15 +179,15 @@
             np.linspace(
                 np.power(val_min, 1.0 / typ),
                 np.power(val_max, 1.0 / typ),
                 steps,
             )
         ) ** typ
     else:
-        print("specialrange: unknown typ '{}'. Using linear range".format(typ))
+        print(f"specialrange: unknown typ '{typ}'. Using linear range")
         rng = np.linspace(val_min, val_max, steps)
 
     return rng
 
 
 def specialrange_cut(val_min, val_max, steps, val_cut=None, typ="exp"):
     """
@@ -274,19 +274,19 @@
         raise ValueError("Anisotropy ratio 'e' must be within 0 and 1")
 
     if np.isclose(e, 1):
         res = 1.0 / 3.0
     elif np.isclose(e, 0):
         res = 0.0
     else:
-        res = e / (2 * (1.0 - e ** 2))
+        res = e / (2 * (1.0 - e**2))
         res *= (
             1.0
-            / np.sqrt(1.0 - e ** 2)
-            * np.arctan(np.sqrt(1.0 / e ** 2 - 1.0))
+            / np.sqrt(1.0 - e**2)
+            * np.arctan(np.sqrt(1.0 / e**2 - 1.0))
             - e
         )
 
     return res
 
 
 def well_solution(
@@ -374,15 +374,15 @@
     time_mat = Input.time_mat
     rad_mat = Input.rad_mat
 
     res = np.zeros((Input.time_no, Input.rad_no))
     res[Input.time_gz, :] = (
         rate
         / (4.0 * np.pi * transmissivity)
-        * exp1(rad_mat ** 2 * storage / (4 * transmissivity * time_mat))
+        * exp1(rad_mat**2 * storage / (4 * transmissivity * time_mat))
     )
     res = Input.reshape(res)
     if rate > 0:
         res = np.maximum(res, 0)
     else:
         res = np.minimum(res, 0)
     # add the reference head
@@ -452,15 +452,15 @@
     if not conductivity > 0.0:
         raise ValueError("The Conductivity needs to be positive.")
     if not storage > 0.0:
         raise ValueError("The Storage needs to be positive.")
 
     time_mat = Input.time_mat
     rad_mat = Input.rad_mat
-    u = storage * rad_mat ** 2 / (4 * conductivity * time_mat)
+    u = storage * rad_mat**2 / (4 * conductivity * time_mat)
     nu = 1.0 - dim / 2.0
 
     res = np.zeros((Input.time_no, Input.rad_no))
     res[Input.time_gz, :] = inc_gamma(-nu, u)
     res[Input.time_gz, :] *= (
         rate
         / (4.0 * np.pi ** (1 - nu) * conductivity * lat_ext ** (3.0 - dim))
@@ -489,15 +489,15 @@
         input values
     """
     if np.isclose(s, 0):
         return exp1(x)
     if np.isclose(s, np.around(s)) and s < -0.5:
         return x ** (s - 1) * expn(int(1 - np.around(s)), x)
     if s < 0:
-        return (inc_gamma(s + 1, x) - x ** s * np.exp(-x)) / s
+        return (inc_gamma(s + 1, x) - x**s * np.exp(-x)) / s
     return gamma(s) * gammaincc(s, x)
 
 
 def tpl_hyp(rad, dim, hurst, corr, prop):
     """Hyp_2F1 for the TPL CG model."""
     x = 1.0 / (1.0 + (prop * rad / corr) ** 2)
     return x ** (dim / 2.0) * hyp2f1(dim / 2.0, 1, dim / 2.0 + 1 + hurst, x)
```

### Comparing `anaflow-1.0.1/tests/test_anaflow.py` & `anaflow-1.1.0/tests/test_anaflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-# -*- coding: utf-8 -*-
 """
 This is the unittest of AnaFlow.
 """
 
 import unittest
+
 import numpy as np
+
 import anaflow as af
 
 # import matplotlib.pyplot as plt
 
 
 def inc(arr, delta=0.0):
     return np.all(arr[:-1] <= arr[1:] + delta)
```

