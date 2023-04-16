# Comparing `tmp/feloopy-0.2.3.tar.gz` & `tmp/feloopy-0.2.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feloopy-0.2.3.tar", last modified: Tue Feb 28 19:02:32 2023, max compression
+gzip compressed data, was "feloopy-0.2.31.tar", last modified: Sun Apr 16 17:52:08 2023, max compression
```

## Comparing `feloopy-0.2.3.tar` & `feloopy-0.2.31.tar`

### file list

```diff
@@ -1,101 +1,126 @@
-drwxrwxrwx   0        0        0        0 2023-02-28 19:02:32.535970 feloopy-0.2.3/
--rw-rw-rw-   0        0        0     1092 2023-02-28 17:50:52.000000 feloopy-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     7128 2023-02-28 19:02:32.533974 feloopy-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     6535 2023-02-28 17:48:35.000000 feloopy-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-02-28 19:02:32.284785 feloopy-0.2.3/feloopy/
--rw-rw-rw-   0        0        0     6994 2023-02-28 14:22:31.000000 feloopy-0.2.3/feloopy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-28 19:02:32.297809 feloopy-0.2.3/feloopy/algorithms/
--rw-rw-rw-   0        0        0        0 2023-01-29 18:58:40.000000 feloopy-0.2.3/feloopy/algorithms/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-28 19:02:32.299811 feloopy-0.2.3/feloopy/algorithms/exact/
--rw-rw-rw-   0        0        0        0 2023-01-29 18:58:40.000000 feloopy-0.2.3/feloopy/algorithms/exact/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-28 19:02:32.317787 feloopy-0.2.3/feloopy/algorithms/heuristic/
--rw-rw-rw-   0        0        0     2812 2023-02-28 17:36:23.000000 feloopy-0.2.3/feloopy/algorithms/heuristic/DE.py
--rw-rw-rw-   0        0        0     3096 2023-02-28 10:53:56.000000 feloopy-0.2.3/feloopy/algorithms/heuristic/GA.py
--rw-rw-rw-   0        0        0     2347 2023-02-28 10:54:00.000000 feloopy-0.2.3/feloopy/algorithms/heuristic/GWO.py
--rw-rw-rw-   0        0        0     3658 2023-02-28 11:13:47.000000 feloopy-0.2.3/feloopy/algorithms/heuristic/SA.py
--rw-rw-rw-   0        0        0     1794 2023-02-28 11:18:26.000000 feloopy-0.2.3/feloopy/algorithms/heuristic/TS.py
--rw-rw-rw-   0        0        0        0 2023-01-29 18:58:40.000000 feloopy-0.2.3/feloopy/algorithms/heuristic/__init__.py
--rw-rw-rw-   0        0        0    56402 2023-02-28 18:16:06.000000 feloopy-0.2.3/feloopy/feloopy.py
-drwxrwxrwx   0        0        0        0 2023-02-28 19:02:32.330786 feloopy-0.2.3/feloopy/generators/
--rw-rw-rw-   0        0        0      129 2023-02-28 16:33:12.000000 feloopy-0.2.3/feloopy/generators/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-28 19:02:32.409257 feloopy-0.2.3/feloopy/generators/model/
--rw-rw-rw-   0        0        0        0 2023-01-29 18:58:40.000000 feloopy-0.2.3/feloopy/generators/model/__init__.py
--rw-rw-rw-   0        0        0      106 2023-01-29 06:50:50.000000 feloopy-0.2.3/feloopy/generators/model/cplex_model_generator.py
--rw-rw-rw-   0        0        0       68 2023-01-29 06:50:58.000000 feloopy-0.2.3/feloopy/generators/model/cvxpy_model_generator.py
--rw-rw-rw-   0        0        0      141 2023-01-29 11:26:46.000000 feloopy-0.2.3/feloopy/generators/model/cylp_model_generator.py
--rw-rw-rw-   0        0        0     1572 2023-02-28 11:22:53.000000 feloopy-0.2.3/feloopy/generators/model/feloopy_model_generator.py
--rw-rw-rw-   0        0        0      104 2023-02-28 11:23:04.000000 feloopy-0.2.3/feloopy/generators/model/gekko_model_generator.py
--rw-rw-rw-   0        0        0      103 2023-02-28 11:23:11.000000 feloopy-0.2.3/feloopy/generators/model/gurobi_model_generator.py
--rw-rw-rw-   0        0        0       90 2023-01-29 06:51:22.000000 feloopy-0.2.3/feloopy/generators/model/linopy_model_generator.py
--rw-rw-rw-   0        0        0    26710 2023-02-28 11:30:45.000000 feloopy-0.2.3/feloopy/generators/model/mealpy_model_generator.py
--rw-rw-rw-   0        0        0      110 2023-02-28 11:30:55.000000 feloopy-0.2.3/feloopy/generators/model/mip_model_generator.py
--rw-rw-rw-   0        0        0      146 2023-02-28 11:31:01.000000 feloopy-0.2.3/feloopy/generators/model/ortools_model_generator.py
--rw-rw-rw-   0        0        0      100 2023-02-28 11:31:07.000000 feloopy-0.2.3/feloopy/generators/model/picos_model_generator.py
--rw-rw-rw-   0        0        0      126 2023-02-28 11:31:13.000000 feloopy-0.2.3/feloopy/generators/model/pulp_model_generator.py
--rw-rw-rw-   0        0        0       97 2023-02-28 17:34:27.000000 feloopy-0.2.3/feloopy/generators/model/pymprog_model_generator.py
--rw-rw-rw-   0        0        0      108 2023-01-29 06:51:48.000000 feloopy-0.2.3/feloopy/generators/model/pyomo_model_generator.py
--rw-rw-rw-   0        0        0      103 2023-01-29 06:51:52.000000 feloopy-0.2.3/feloopy/generators/model/xpress_model_generator.py
--rw-rw-rw-   0        0        0     2028 2023-02-28 14:20:24.000000 feloopy-0.2.3/feloopy/generators/model_generator.py
-drwxrwxrwx   0        0        0        0 2023-02-28 19:02:32.444252 feloopy-0.2.3/feloopy/generators/result/
--rw-rw-rw-   0        0        0        0 2023-01-29 18:58:40.000000 feloopy-0.2.3/feloopy/generators/result/__init__.py
--rw-rw-rw-   0        0        0      426 2023-02-28 11:41:24.000000 feloopy-0.2.3/feloopy/generators/result/cplex_result_generator.py
--rw-rw-rw-   0        0        0      331 2023-02-28 11:41:37.000000 feloopy-0.2.3/feloopy/generators/result/cvxpy_result_generator.py
--rw-rw-rw-   0        0        0      487 2023-02-28 11:37:58.000000 feloopy-0.2.3/feloopy/generators/result/cylp_result_generator.py
--rw-rw-rw-   0        0        0      547 2023-02-28 11:37:49.000000 feloopy-0.2.3/feloopy/generators/result/gekko_result_generator.py
--rw-rw-rw-   0        0        0     1164 2023-02-28 11:37:37.000000 feloopy-0.2.3/feloopy/generators/result/gurobi_result_generator.py
--rw-rw-rw-   0        0        0      426 2023-02-28 11:37:30.000000 feloopy-0.2.3/feloopy/generators/result/linopy_result_generator.py
--rw-rw-rw-   0        0        0      373 2023-02-28 11:37:06.000000 feloopy-0.2.3/feloopy/generators/result/mip_result_generator.py
--rw-rw-rw-   0        0        0      604 2023-02-28 11:36:57.000000 feloopy-0.2.3/feloopy/generators/result/ortools_result_generator.py
--rw-rw-rw-   0        0        0      396 2023-02-28 11:41:57.000000 feloopy-0.2.3/feloopy/generators/result/picos_result_generator.py
--rw-rw-rw-   0        0        0      475 2023-02-28 11:36:26.000000 feloopy-0.2.3/feloopy/generators/result/pulp_result_generator.py
--rw-rw-rw-   0        0        0      483 2023-02-28 11:42:08.000000 feloopy-0.2.3/feloopy/generators/result/pymprog_result_generator.py
--rw-rw-rw-   0        0        0      451 2023-02-28 11:36:01.000000 feloopy-0.2.3/feloopy/generators/result/pyomo_result_generator.py
--rw-rw-rw-   0        0        0      398 2023-02-28 11:42:18.000000 feloopy-0.2.3/feloopy/generators/result/xpress_result_generator.py
--rw-rw-rw-   0        0        0     5432 2023-02-28 14:14:40.000000 feloopy-0.2.3/feloopy/generators/result_generator.py
-drwxrwxrwx   0        0        0        0 2023-02-28 19:02:32.480774 feloopy-0.2.3/feloopy/generators/solution/
--rw-rw-rw-   0        0        0        0 2023-01-29 18:58:40.000000 feloopy-0.2.3/feloopy/generators/solution/__init__.py
--rw-rw-rw-   0        0        0     1671 2023-02-28 16:36:10.000000 feloopy-0.2.3/feloopy/generators/solution/cplex_solution_generator.py
--rw-rw-rw-   0        0        0     1806 2023-02-28 13:37:57.000000 feloopy-0.2.3/feloopy/generators/solution/cvxpy_solution_generator.py
--rw-rw-rw-   0        0        0     1318 2023-02-28 13:37:51.000000 feloopy-0.2.3/feloopy/generators/solution/cylp_solution_generator.py
--rw-rw-rw-   0        0        0     2912 2023-02-28 12:58:24.000000 feloopy-0.2.3/feloopy/generators/solution/feloopy_solution_generator.py
--rw-rw-rw-   0        0        0     1762 2023-02-28 13:37:38.000000 feloopy-0.2.3/feloopy/generators/solution/gekko_solution_generator.py
--rw-rw-rw-   0        0        0     1264 2023-02-28 13:37:32.000000 feloopy-0.2.3/feloopy/generators/solution/gurobi_solution_generator.py
--rw-rw-rw-   0        0        0     1456 2023-02-28 13:37:25.000000 feloopy-0.2.3/feloopy/generators/solution/linopy_solution_generator.py
--rw-rw-rw-   0        0        0     4280 2023-02-28 14:09:16.000000 feloopy-0.2.3/feloopy/generators/solution/mealpy_solution_generator.py
--rw-rw-rw-   0        0        0     1217 2023-02-28 14:08:34.000000 feloopy-0.2.3/feloopy/generators/solution/mip_solution_generator.py
--rw-rw-rw-   0        0        0     1887 2023-02-28 14:08:31.000000 feloopy-0.2.3/feloopy/generators/solution/ortools_solution_generator.py
--rw-rw-rw-   0        0        0     1594 2023-02-28 14:08:27.000000 feloopy-0.2.3/feloopy/generators/solution/picos_solution_generator.py
--rw-rw-rw-   0        0        0     1988 2023-02-28 14:08:24.000000 feloopy-0.2.3/feloopy/generators/solution/pulp_solution_generator.py
--rw-rw-rw-   0        0        0     1189 2023-02-28 14:08:21.000000 feloopy-0.2.3/feloopy/generators/solution/pymprog_solution_generator.py
--rw-rw-rw-   0        0        0     4346 2023-02-28 14:08:18.000000 feloopy-0.2.3/feloopy/generators/solution/pyomo_solution_generator.py
--rw-rw-rw-   0        0        0     1258 2023-02-28 14:08:13.000000 feloopy-0.2.3/feloopy/generators/solution/xpress_solution_generator.py
--rw-rw-rw-   0        0        0     4485 2023-01-29 15:33:08.000000 feloopy-0.2.3/feloopy/generators/solution_generator.py
-drwxrwxrwx   0        0        0        0 2023-02-28 19:02:32.518971 feloopy-0.2.3/feloopy/generators/variable/
--rw-rw-rw-   0        0        0        0 2023-01-29 21:11:46.000000 feloopy-0.2.3/feloopy/generators/variable/__init__.py
--rw-rw-rw-   0        0        0     2217 2023-02-28 14:13:14.000000 feloopy-0.2.3/feloopy/generators/variable/cplex_variable_generator.py
--rw-rw-rw-   0        0        0     2753 2023-02-28 14:13:18.000000 feloopy-0.2.3/feloopy/generators/variable/cvxpy_variable_generator.py
--rw-rw-rw-   0        0        0     2529 2023-02-28 14:13:22.000000 feloopy-0.2.3/feloopy/generators/variable/cylp_variable_generator.py
--rw-rw-rw-   0        0        0     2245 2023-02-28 14:13:25.000000 feloopy-0.2.3/feloopy/generators/variable/gekko_variable_generator.py
--rw-rw-rw-   0        0        0     3337 2023-02-28 14:13:28.000000 feloopy-0.2.3/feloopy/generators/variable/gurobi_variable_generator.py
--rw-rw-rw-   0        0        0     1809 2023-02-28 14:13:32.000000 feloopy-0.2.3/feloopy/generators/variable/linopy_variable_generator.py
--rw-rw-rw-   0        0        0     2463 2023-02-28 14:13:36.000000 feloopy-0.2.3/feloopy/generators/variable/mip_variable_generator.py
--rw-rw-rw-   0        0        0     3270 2023-02-28 14:13:39.000000 feloopy-0.2.3/feloopy/generators/variable/ortools_variable_generator.py
--rw-rw-rw-   0        0        0     2412 2023-02-28 14:13:42.000000 feloopy-0.2.3/feloopy/generators/variable/picos_variable_generator.py
--rw-rw-rw-   0        0        0     2990 2023-02-28 14:13:47.000000 feloopy-0.2.3/feloopy/generators/variable/pulp_variable_generator.py
--rw-rw-rw-   0        0        0     2494 2023-02-28 14:13:51.000000 feloopy-0.2.3/feloopy/generators/variable/pymprog_variable_generator.py
--rw-rw-rw-   0        0        0     1954 2023-02-28 14:13:54.000000 feloopy-0.2.3/feloopy/generators/variable/pyomo_variable_generator.py
--rw-rw-rw-   0        0        0     4078 2023-02-28 14:13:58.000000 feloopy-0.2.3/feloopy/generators/variable/xpress_variable_generator.py
--rw-rw-rw-   0        0        0     3062 2023-01-29 07:09:12.000000 feloopy-0.2.3/feloopy/generators/variable_generator.py
-drwxrwxrwx   0        0        0        0 2023-02-28 19:02:32.532971 feloopy-0.2.3/feloopy/operators/
--rw-rw-rw-   0        0        0       69 2023-02-28 14:20:41.000000 feloopy-0.2.3/feloopy/operators/__init__.py
--rw-rw-rw-   0        0        0     8018 2023-02-28 17:28:45.000000 feloopy-0.2.3/feloopy/operators/common.py
--rw-rw-rw-   0        0        0      593 2023-02-28 14:21:46.000000 feloopy-0.2.3/feloopy/operators/exact.py
--rw-rw-rw-   0        0        0      307 2023-02-28 14:21:55.000000 feloopy-0.2.3/feloopy/operators/heuristic.py
-drwxrwxrwx   0        0        0        0 2023-02-28 19:02:32.296786 feloopy-0.2.3/feloopy.egg-info/
--rw-rw-rw-   0        0        0     7128 2023-02-28 19:02:32.000000 feloopy-0.2.3/feloopy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3977 2023-02-28 19:02:32.000000 feloopy-0.2.3/feloopy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-28 19:02:32.000000 feloopy-0.2.3/feloopy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      146 2023-02-28 19:02:32.000000 feloopy-0.2.3/feloopy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-28 19:02:32.000000 feloopy-0.2.3/feloopy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-28 19:02:32.535970 feloopy-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1335 2023-02-28 15:08:13.000000 feloopy-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:52:08.178434 feloopy-0.2.31/
+-rw-rw-rw-   0        0        0     1092 2023-03-25 08:57:31.000000 feloopy-0.2.31/LICENSE
+-rw-rw-rw-   0        0        0    12387 2023-04-16 17:52:08.175427 feloopy-0.2.31/PKG-INFO
+-rw-rw-rw-   0        0        0    11761 2023-04-16 17:51:27.000000 feloopy-0.2.31/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 17:52:07.949848 feloopy-0.2.31/feloopy/
+-rw-rw-rw-   0        0        0     9884 2023-04-16 13:41:04.000000 feloopy-0.2.31/feloopy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:52:07.962867 feloopy-0.2.31/feloopy/algorithms/
+-rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/algorithms/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:52:07.963868 feloopy-0.2.31/feloopy/algorithms/constraint/
+-rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/algorithms/constraint/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:52:07.964866 feloopy-0.2.31/feloopy/algorithms/exact/
+-rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/algorithms/exact/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:52:07.982382 feloopy-0.2.31/feloopy/algorithms/heuristic/
+-rw-rw-rw-   0        0        0     2812 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/algorithms/heuristic/DE.py
+-rw-rw-rw-   0        0        0     3096 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/algorithms/heuristic/GA.py
+-rw-rw-rw-   0        0        0     2347 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/algorithms/heuristic/GWO.py
+-rw-rw-rw-   0        0        0     3658 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/algorithms/heuristic/SA.py
+-rw-rw-rw-   0        0        0     1794 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/algorithms/heuristic/TS.py
+-rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/algorithms/heuristic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:52:07.984379 feloopy-0.2.31/feloopy/classes/
+-rw-rw-rw-   0        0        0        0 2023-04-11 13:35:08.000000 feloopy-0.2.31/feloopy/classes/__init__.py
+-rw-rw-rw-   0        0        0     1295 2023-04-11 13:36:26.000000 feloopy-0.2.31/feloopy/classes/empty.py
+-rw-rw-rw-   0        0        0    77481 2023-04-16 17:32:59.000000 feloopy-0.2.31/feloopy/feloopy.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:52:08.002376 feloopy-0.2.31/feloopy/functions/
+-rw-rw-rw-   0        0        0        0 2023-04-11 13:45:00.000000 feloopy-0.2.31/feloopy/functions/__init__.py
+-rw-rw-rw-   0        0        0      488 2023-04-16 13:41:27.000000 feloopy-0.2.31/feloopy/functions/count_operators.py
+-rw-rw-rw-   0        0        0      211 2023-04-16 14:10:14.000000 feloopy-0.2.31/feloopy/functions/fix_operators.py
+-rw-rw-rw-   0        0        0     3029 2023-04-11 13:51:06.000000 feloopy-0.2.31/feloopy/functions/heuristic_operators.py
+-rw-rw-rw-   0        0        0       38 2023-04-11 13:49:57.000000 feloopy-0.2.31/feloopy/functions/math_operators.py
+-rw-rw-rw-   0        0        0      185 2023-04-11 13:50:07.000000 feloopy-0.2.31/feloopy/functions/random_operators.py
+-rw-rw-rw-   0        0        0      305 2023-04-11 13:50:17.000000 feloopy-0.2.31/feloopy/functions/set_operators.py
+-rw-rw-rw-   0        0        0     1669 2023-04-11 13:50:36.000000 feloopy-0.2.31/feloopy/functions/update_operators.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:52:08.015374 feloopy-0.2.31/feloopy/generators/
+-rw-rw-rw-   0        0        0      129 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/generators/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:52:08.049368 feloopy-0.2.31/feloopy/generators/model/
+-rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/generators/model/__init__.py
+-rw-rw-rw-   0        0        0      156 2023-04-11 11:47:49.000000 feloopy-0.2.31/feloopy/generators/model/cplex_cp_model_generator.py
+-rw-rw-rw-   0        0        0      153 2023-04-11 11:48:02.000000 feloopy-0.2.31/feloopy/generators/model/cplex_model_generator.py
+-rw-rw-rw-   0        0        0      136 2023-04-16 12:06:27.000000 feloopy-0.2.31/feloopy/generators/model/cvxpy_model_generator.py
+-rw-rw-rw-   0        0        0      155 2023-04-11 11:48:21.000000 feloopy-0.2.31/feloopy/generators/model/cylp_model_generator.py
+-rw-rw-rw-   0        0        0     1572 2023-04-05 08:38:53.000000 feloopy-0.2.31/feloopy/generators/model/feloopy_model_generator.py
+-rw-rw-rw-   0        0        0      146 2023-04-11 11:49:14.000000 feloopy-0.2.31/feloopy/generators/model/gekko_model_generator.py
+-rw-rw-rw-   0        0        0      133 2023-04-11 11:49:40.000000 feloopy-0.2.31/feloopy/generators/model/gurobi_model_generator.py
+-rw-rw-rw-   0        0        0      104 2023-04-11 11:49:51.000000 feloopy-0.2.31/feloopy/generators/model/linopy_model_generator.py
+-rw-rw-rw-   0        0        0    26710 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/generators/model/mealpy_model_generator.py
+-rw-rw-rw-   0        0        0      140 2023-04-11 11:50:27.000000 feloopy-0.2.31/feloopy/generators/model/mip_model_generator.py
+-rw-rw-rw-   0        0        0      139 2023-04-11 11:50:43.000000 feloopy-0.2.31/feloopy/generators/model/ortools_cp_model_generator.py
+-rw-rw-rw-   0        0        0      156 2023-04-11 11:51:10.000000 feloopy-0.2.31/feloopy/generators/model/ortools_model_generator.py
+-rw-rw-rw-   0        0        0      135 2023-04-11 11:51:26.000000 feloopy-0.2.31/feloopy/generators/model/picos_model_generator.py
+-rw-rw-rw-   0        0        0      156 2023-04-11 11:51:37.000000 feloopy-0.2.31/feloopy/generators/model/pulp_model_generator.py
+-rw-rw-rw-   0        0        0      127 2023-04-11 11:51:46.000000 feloopy-0.2.31/feloopy/generators/model/pymprog_model_generator.py
+-rw-rw-rw-   0        0        0      149 2023-04-11 11:52:04.000000 feloopy-0.2.31/feloopy/generators/model/pyomo_model_generator.py
+-rw-rw-rw-   0        0        0      133 2023-04-11 11:52:21.000000 feloopy-0.2.31/feloopy/generators/model/xpress_model_generator.py
+-rw-rw-rw-   0        0        0     2474 2023-04-11 11:47:11.000000 feloopy-0.2.31/feloopy/generators/model_generator.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:52:08.077881 feloopy-0.2.31/feloopy/generators/result/
+-rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/generators/result/__init__.py
+-rw-rw-rw-   0        0        0      385 2023-04-11 17:07:27.000000 feloopy-0.2.31/feloopy/generators/result/cplex_cp_result_generator.py
+-rw-rw-rw-   0        0        0      453 2023-04-11 17:07:23.000000 feloopy-0.2.31/feloopy/generators/result/cplex_result_generator.py
+-rw-rw-rw-   0        0        0      452 2023-04-16 12:04:52.000000 feloopy-0.2.31/feloopy/generators/result/cvxpy_result_generator.py
+-rw-rw-rw-   0        0        0      504 2023-04-05 08:40:40.000000 feloopy-0.2.31/feloopy/generators/result/cylp_result_generator.py
+-rw-rw-rw-   0        0        0      576 2023-04-05 08:40:56.000000 feloopy-0.2.31/feloopy/generators/result/gekko_result_generator.py
+-rw-rw-rw-   0        0        0     1183 2023-04-05 08:41:25.000000 feloopy-0.2.31/feloopy/generators/result/gurobi_result_generator.py
+-rw-rw-rw-   0        0        0      452 2023-04-05 08:41:37.000000 feloopy-0.2.31/feloopy/generators/result/linopy_result_generator.py
+-rw-rw-rw-   0        0        0      391 2023-04-05 08:41:43.000000 feloopy-0.2.31/feloopy/generators/result/mip_result_generator.py
+-rw-rw-rw-   0        0        0      548 2023-04-05 08:41:48.000000 feloopy-0.2.31/feloopy/generators/result/ortools_cp_result_generator.py
+-rw-rw-rw-   0        0        0      622 2023-04-05 08:41:53.000000 feloopy-0.2.31/feloopy/generators/result/ortools_result_generator.py
+-rw-rw-rw-   0        0        0      414 2023-04-05 08:41:58.000000 feloopy-0.2.31/feloopy/generators/result/picos_result_generator.py
+-rw-rw-rw-   0        0        0      507 2023-04-05 08:42:04.000000 feloopy-0.2.31/feloopy/generators/result/pulp_result_generator.py
+-rw-rw-rw-   0        0        0      500 2023-04-05 08:42:10.000000 feloopy-0.2.31/feloopy/generators/result/pymprog_result_generator.py
+-rw-rw-rw-   0        0        0      469 2023-04-05 08:42:16.000000 feloopy-0.2.31/feloopy/generators/result/pyomo_result_generator.py
+-rw-rw-rw-   0        0        0      417 2023-04-05 08:42:22.000000 feloopy-0.2.31/feloopy/generators/result/xpress_result_generator.py
+-rw-rw-rw-   0        0        0     6254 2023-04-04 11:50:22.000000 feloopy-0.2.31/feloopy/generators/result_generator.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:52:08.118874 feloopy-0.2.31/feloopy/generators/solution/
+-rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/generators/solution/__init__.py
+-rw-rw-rw-   0        0        0     2446 2023-04-11 11:29:12.000000 feloopy-0.2.31/feloopy/generators/solution/cplex_cp_solution_generator.py
+-rw-rw-rw-   0        0        0     3968 2023-04-11 11:29:46.000000 feloopy-0.2.31/feloopy/generators/solution/cplex_solution_generator.py
+-rw-rw-rw-   0        0        0     2929 2023-04-16 12:52:44.000000 feloopy-0.2.31/feloopy/generators/solution/cvxpy_solution_generator.py
+-rw-rw-rw-   0        0        0     1998 2023-04-11 11:30:29.000000 feloopy-0.2.31/feloopy/generators/solution/cylp_solution_generator.py
+-rw-rw-rw-   0        0        0     2947 2023-03-31 08:00:48.000000 feloopy-0.2.31/feloopy/generators/solution/feloopy_solution_generator.py
+-rw-rw-rw-   0        0        0     2740 2023-04-16 13:02:36.000000 feloopy-0.2.31/feloopy/generators/solution/gekko_solution_generator.py
+-rw-rw-rw-   0        0        0     2728 2023-04-11 11:31:20.000000 feloopy-0.2.31/feloopy/generators/solution/gurobi_solution_generator.py
+-rw-rw-rw-   0        0        0     2136 2023-04-11 11:31:33.000000 feloopy-0.2.31/feloopy/generators/solution/linopy_solution_generator.py
+-rw-rw-rw-   0        0        0     4315 2023-04-11 11:31:52.000000 feloopy-0.2.31/feloopy/generators/solution/mealpy_solution_generator.py
+-rw-rw-rw-   0        0        0     1901 2023-04-11 11:32:13.000000 feloopy-0.2.31/feloopy/generators/solution/mip_solution_generator.py
+-rw-rw-rw-   0        0        0     2758 2023-04-11 11:32:29.000000 feloopy-0.2.31/feloopy/generators/solution/ortools_cp_solution_generator.py
+-rw-rw-rw-   0        0        0     3091 2023-04-11 11:32:41.000000 feloopy-0.2.31/feloopy/generators/solution/ortools_solution_generator.py
+-rw-rw-rw-   0        0        0     2278 2023-04-11 11:32:52.000000 feloopy-0.2.31/feloopy/generators/solution/picos_solution_generator.py
+-rw-rw-rw-   0        0        0     3322 2023-04-11 11:33:06.000000 feloopy-0.2.31/feloopy/generators/solution/pulp_solution_generator.py
+-rw-rw-rw-   0        0        0     2054 2023-04-12 06:39:22.000000 feloopy-0.2.31/feloopy/generators/solution/pymprog_solution_generator.py
+-rw-rw-rw-   0        0        0     5576 2023-04-12 06:19:57.000000 feloopy-0.2.31/feloopy/generators/solution/pyomo_solution_generator.py
+-rw-rw-rw-   0        0        0     1935 2023-04-11 15:44:52.000000 feloopy-0.2.31/feloopy/generators/solution/xpress_solution_generator.py
+-rw-rw-rw-   0        0        0     2674 2023-04-11 11:23:04.000000 feloopy-0.2.31/feloopy/generators/solution_generator.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:52:08.160907 feloopy-0.2.31/feloopy/generators/variable/
+-rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/generators/variable/__init__.py
+-rw-rw-rw-   0        0        0     2677 2023-04-04 08:02:30.000000 feloopy-0.2.31/feloopy/generators/variable/cplex_cp_variable_generator.py
+-rw-rw-rw-   0        0        0     2967 2023-04-11 15:32:22.000000 feloopy-0.2.31/feloopy/generators/variable/cplex_variable_generator.py
+-rw-rw-rw-   0        0        0     6460 2023-04-16 12:18:37.000000 feloopy-0.2.31/feloopy/generators/variable/cvxpy_variable_generator.py
+-rw-rw-rw-   0        0        0     2783 2023-03-31 08:38:56.000000 feloopy-0.2.31/feloopy/generators/variable/cylp_variable_generator.py
+-rw-rw-rw-   0        0        0     2621 2023-03-31 08:39:01.000000 feloopy-0.2.31/feloopy/generators/variable/gekko_variable_generator.py
+-rw-rw-rw-   0        0        0     7599 2023-04-16 11:18:49.000000 feloopy-0.2.31/feloopy/generators/variable/gurobi_variable_generator.py
+-rw-rw-rw-   0        0        0     2123 2023-03-31 08:39:06.000000 feloopy-0.2.31/feloopy/generators/variable/linopy_variable_generator.py
+-rw-rw-rw-   0        0        0     2657 2023-03-31 09:21:12.000000 feloopy-0.2.31/feloopy/generators/variable/mip_variable_generator.py
+-rw-rw-rw-   0        0        0     3756 2023-04-04 13:36:46.000000 feloopy-0.2.31/feloopy/generators/variable/ortools_cp_variable_generator.py
+-rw-rw-rw-   0        0        0     3997 2023-03-31 08:36:53.000000 feloopy-0.2.31/feloopy/generators/variable/ortools_variable_generator.py
+-rw-rw-rw-   0        0        0     2888 2023-03-31 08:39:12.000000 feloopy-0.2.31/feloopy/generators/variable/picos_variable_generator.py
+-rw-rw-rw-   0        0        0     3544 2023-03-31 08:39:15.000000 feloopy-0.2.31/feloopy/generators/variable/pulp_variable_generator.py
+-rw-rw-rw-   0        0        0     3048 2023-03-31 08:39:17.000000 feloopy-0.2.31/feloopy/generators/variable/pymprog_variable_generator.py
+-rw-rw-rw-   0        0        0     2326 2023-03-31 08:39:19.000000 feloopy-0.2.31/feloopy/generators/variable/pyomo_variable_generator.py
+-rw-rw-rw-   0        0        0     4552 2023-03-31 08:39:21.000000 feloopy-0.2.31/feloopy/generators/variable/xpress_variable_generator.py
+-rw-rw-rw-   0        0        0     2814 2023-04-04 07:53:39.000000 feloopy-0.2.31/feloopy/generators/variable_generator.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:52:08.167907 feloopy-0.2.31/feloopy/operators/
+-rw-rw-rw-   0        0        0       69 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/operators/__init__.py
+-rw-rw-rw-   0        0        0     9094 2023-04-11 17:03:29.000000 feloopy-0.2.31/feloopy/operators/common.py
+-rw-rw-rw-   0        0        0       89 2023-04-05 08:20:05.000000 feloopy-0.2.31/feloopy/operators/exact.py
+-rw-rw-rw-   0        0        0      187 2023-04-05 08:19:38.000000 feloopy-0.2.31/feloopy/operators/heuristic.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:52:07.960868 feloopy-0.2.31/feloopy.egg-info/
+-rw-rw-rw-   0        0        0    12387 2023-04-16 17:52:07.000000 feloopy-0.2.31/feloopy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4869 2023-04-16 17:52:07.000000 feloopy-0.2.31/feloopy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 17:52:07.000000 feloopy-0.2.31/feloopy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      146 2023-04-16 17:52:07.000000 feloopy-0.2.31/feloopy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-16 17:52:07.000000 feloopy-0.2.31/feloopy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 17:52:08.178434 feloopy-0.2.31/setup.cfg
+-rw-rw-rw-   0        0        0     1368 2023-04-16 17:43:13.000000 feloopy-0.2.31/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:52:08.170416 feloopy-0.2.31/tests/
+-rw-rw-rw-   0        0        0     1029 2023-04-16 17:34:01.000000 feloopy-0.2.31/tests/test_exact_kp.py
+-rw-rw-rw-   0        0        0     1277 2023-04-12 07:11:14.000000 feloopy-0.2.31/tests/test_exact_tsp.py
```

### Comparing `feloopy-0.2.3/LICENSE` & `feloopy-0.2.31/LICENSE`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.3/feloopy/__init__.py` & `feloopy-0.2.31/feloopy/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -170,25 +170,156 @@
                         'OriginalRUN',
                         'OriginalCircleSA',
                         'OriginalHS',
                         'BaseHS'
                         ]
 
 exact_algorithms = [
+
+    # gekko
     ['gekko', 'apopt'],
-    ['ortools', 'bop'],
     ['gekko', 'bpopt'],
-    ['pulp', 'cbc'],
-    ['ortools', 'glop'],
-    ['pymprog', 'glpk'],
     ['gekko', 'ipopt'],
+
+    # ortools
+    ['ortools', 'bop'],
+    ['ortools', 'cbc'],
+    ['ortools', 'clp'],
+    ['ortools', 'cplex_'],
+    ['ortools', 'cplex'],
+    ['ortools', 'glop'],
+    ['ortools', 'glpk_'],
+    ['ortools', 'glpk'],
+    ['ortools', 'gurobi_'],
+    ['ortools', 'gurobi'],
     ['ortools', 'sat'],
     ['ortools', 'scip'],
+    ['ortools', 'xpress_'],
+    ['ortools', 'xpress'],
+
+    # pulp
+    ['pulp', 'cbc'],
+    ['pulp', 'choco'],
+    ['pulp', 'coin'],
+    ['pulp', 'coinmp_dll'],
+    ['pulp', 'cplex_py'],
+    ['pulp', 'cplex'],
+    ['pulp', 'glpk'],
+    ['pulp', 'gurobi_cmd'],
+    ['pulp', 'gurobi'],
+    ['pulp', 'highs'],
+    ['pulp', 'mipcl'],
+    ['pulp', 'mosek'],
+    ['pulp', 'pyglpk'],
+    ['pulp', 'scip'],
+    ['pulp', 'xpress_py'],
+    ['pulp', 'xpress'],
+
+    # cvxpy
+    ['cvxpy', 'osqp'],
+    ['cvxpy', 'ecos'],
+    ['cvxpy', 'cvxopt'],
+    ['cvxpy', 'scs'],
+    ['cvxpy', 'scipy'],
+    ['cvxpy', 'glop'],
+    ['cvxpy', 'glpk'],
+    ['cvxpy', 'glpk_mi'],
+    ['cvxpy', 'gurobi'],
+    ['cvxpy', 'mosek'],
+    ['cvxpy', 'cbc'],
+    ['cvxpy', 'cplex'],
+    ['cvxpy', 'nag'],
+    ['cvxpy', 'pdlp'],
+    ['cvxpy', 'scip'],
+    ['cvxpy', 'xpress'],
+    ['cvxpy', 'copt'],
+    ['cvxpy', 'clarabel'],
+    ['cvxpy', 'proxqp'],
+
+    # cylp
+    ['cylp', 'cbc'],
+
+    # gurobi
+    ['gurobi', 'gurobi'],
+
+    # cplex
+    ['cplex', 'cplex'],
+
+    # linopy
+    ['linopy', 'cbc'],
+    ['linopy', 'glpk'],
+    ['linopy', 'highs'],
+    ['linopy', 'gurobi'],
+    ['linopy', 'xpress'],
+    ['linopy', 'cplex'],
+
+    # mip
+    ['mip', 'cbc'],
+
+    # picos
+    ['picos', 'cplex'],
+    ['picos', 'cvxopt'],
+    ['picos', 'ecos'],
+    ['picos', 'glpk'],
+    ['picos', 'gurobi'],
+    ['picos', 'mosek'],
+    ['picos', 'mskfn'],
+    ['picos', 'osqp'],
+    ['picos', 'scip'],
+    ['picos', 'smcp'],
+
+    # pymprog
+    ['pymprog', 'glpk'],
+
+    # pyomo
+    ['pyomo', 'baron'],
+    ['pyomo', 'cbc'],
+    ['pyomo', 'conopt'],
+    ['pyomo', 'cplex'],
+    ['pyomo', 'cplex_direct'],
+    ['pyomo', 'cplex_persistent'],
+    ['pyomo', 'cyipopt'],
+    ['pyomo', 'gams'],
+    ['pyomo', 'highs'],
+    ['pyomo', 'asl'],
+    ['pyomo', 'gdpopt'],
+    ['pyomo', 'gdpopt.gloa'],
+    ['pyomo', 'gdpopt.lbb'],
+    ['pyomo', 'gdpopt.loa'],
+    ['pyomo', 'gdpopt.ric'],
+    ['pyomo', 'glpk'],
+    ['pyomo', 'gurobi'],
+    ['pyomo', 'gurobi_direct'],
+    ['pyomo', 'gurobi_persistent'],
+    ['pyomo', 'ipopt'],
+    ['pyomo', 'mindtpy'],
+    ['pyomo', 'mosek'],
+    ['pyomo', 'mosek_direct'],
+    ['pyomo', 'mosek_persistent'],
+    ['pyomo', 'mpec_minlp'],
+    ['pyomo', 'mpec_nlp'],
+    ['pyomo', 'multistart'],
+    ['pyomo', 'path'],
+    ['pyomo', 'scip'],
+    ['pyomo', 'trustregion'],
+    ['pyomo', 'xpress'],
+    ['pyomo', 'xpress_direct'],
+    ['pyomo', 'xpress_persistent'],
+
+    # xpress
+    ['xpress', 'xpress'],
+]
+
+constraint_algorithms = [
+
+    ['cplex_cp', 'cplex'],
+    ['ortools_cp', 'ortools']
+
 ]
 
-feloopy_algorithms = [
+feloopy_heuristic_algorithms = [
     'GA',
     'SA',
     'TS',
     'DE',
     'GWO'
-]
+]
```

### Comparing `feloopy-0.2.3/feloopy/algorithms/heuristic/DE.py` & `feloopy-0.2.31/feloopy/algorithms/heuristic/DE.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.3/feloopy/algorithms/heuristic/GA.py` & `feloopy-0.2.31/feloopy/algorithms/heuristic/GA.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.3/feloopy/algorithms/heuristic/GWO.py` & `feloopy-0.2.31/feloopy/algorithms/heuristic/GWO.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.3/feloopy/algorithms/heuristic/SA.py` & `feloopy-0.2.31/feloopy/algorithms/heuristic/SA.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.3/feloopy/algorithms/heuristic/TS.py` & `feloopy-0.2.31/feloopy/algorithms/heuristic/TS.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.3/feloopy/generators/model/feloopy_model_generator.py` & `feloopy-0.2.31/feloopy/generators/model/feloopy_model_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.3/feloopy/generators/model/mealpy_model_generator.py` & `feloopy-0.2.31/feloopy/generators/model/mealpy_model_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.3/feloopy/generators/result/gekko_result_generator.py` & `feloopy-0.2.31/feloopy/generators/result/gekko_result_generator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 import gekko as gekko_interface
+
 gekko_status_dict = {0: "not_optimal", 1: "optimal"}
 
-def Get(modelobject, result, input1, input2=None):
+def Get(model_object, result, input1, input2=None):
    
-   dir = +1 if input1[1][input1[2]]=='min' else -1
+   directions = +1 if input1[1][input1[2]]=='min' else -1
+
    input1 = input1[0]
 
    match input1:
       
     case 'variable':
+
         return input2.value[0]
     
     case 'status':
-        return gekko_status_dict.get(modelobject.options.SOLVESTATUS)
+
+        return gekko_status_dict.get(model_object.options.SOLVESTATUS)
          
     case 'objective':
-        return  dir*modelobject.options.objfcnval
+
+        return  directions*model_object.options.objfcnval
 
     case 'time':
+
         return (result[1][1]-result[1][0])
```

### Comparing `feloopy-0.2.3/feloopy/generators/result/gurobi_result_generator.py` & `feloopy-0.2.31/feloopy/generators/result/gurobi_result_generator.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,24 +13,28 @@
     gurobi_interface.GRB.SOLUTION_LIMIT: 'solution limit',
     gurobi_interface.GRB.INTERRUPTED: 'interrupted',
     gurobi_interface.GRB.NUMERIC: 'numerical',
     gurobi_interface.GRB.SUBOPTIMAL: 'suboptimal',
     gurobi_interface.GRB.INPROGRESS: 'inprogress'
 }
 
-def Get(modelobject, result, input1, input2=None):
+def Get(model_object, result, input1, input2=None):
    
    input1 = input1[0]
 
    match input1:
 
     case 'variable':
+
         return input2.X
     
     case 'status':
-        return  gurobi_status_dict[modelobject.status]
+
+        return  gurobi_status_dict[model_object.status]
          
     case 'objective':
-        return  modelobject.ObjVal
+
+        return  model_object.ObjVal
 
     case 'time':
+        
         return (result[1][1]-result[1][0])
```

### Comparing `feloopy-0.2.3/feloopy/generators/result/ortools_result_generator.py` & `feloopy-0.2.31/feloopy/generators/result/ortools_result_generator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from ortools.linear_solver import pywraplp as ortools_interface
 
 ortools_status_dict = {0: "optimal", 1: "feasible", 2: "infeasible",3: "unbounded", 4: "abnormal", 5: "model_invalid", 6: "not_solved"}
 
-def Get(modelobject, result, input1, input2=None):
+def Get(model_object, result, input1, input2=None):
 
    input1 = input1[0]
 
    match input1:
 
     case 'variable':
+        
         return input2.solution_value()
     
     case 'status':
+
         return ortools_status_dict.get(result[0], "Not Optimal")
          
     case 'objective':
-        return  modelobject.Objective().Value()
+
+        return  model_object.Objective().Value()
 
     case 'time':
+
         return (result[1][1]-result[1][0])
```

### Comparing `feloopy-0.2.3/feloopy/generators/result_generator.py` & `feloopy-0.2.31/feloopy/generators/result_generator.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,20 @@
                 return pyomo_result_generator.Get(ModelObject, ModelSolution, indicator, VariableNameWithIndex)
 
             case 'ortools':
 
                 from .result import ortools_result_generator
                 return ortools_result_generator.Get(ModelObject, ModelSolution, indicator, VariableNameWithIndex)
 
+            case 'ortools_cp':
+
+                from .result import ortools_cp_result_generator
+                return ortools_cp_result_generator.Get(ModelObject, ModelSolution, indicator, VariableNameWithIndex)
+
+
             case 'gekko':
 
                 from .result import gekko_result_generator
                 return gekko_result_generator.Get(ModelObject, ModelSolution, indicator, VariableNameWithIndex)
 
             case 'picos':
 
@@ -48,14 +54,19 @@
                 return pymprog_result_generator.Get(ModelObject, ModelSolution, indicator, VariableNameWithIndex)
 
             case 'cplex':
 
                 from .result import cplex_result_generator
                 return cplex_result_generator.Get(ModelObject, ModelSolution, indicator, VariableNameWithIndex)
 
+            case 'cplex_cp':
+
+                from .result import cplex_cp_result_generator
+                return cplex_cp_result_generator.Get(ModelObject, ModelSolution, indicator, VariableNameWithIndex)
+
             case 'gurobi':
 
                 from .result import gurobi_result_generator
                 return gurobi_result_generator.Get(ModelObject, ModelSolution, indicator, VariableNameWithIndex)
 
             case 'xpress':
 
@@ -87,14 +98,19 @@
                 return pyomo_result_generator.Get(ModelObject, ModelSolution, indicator)
 
             case 'ortools':
 
                 from .result import ortools_result_generator
                 return ortools_result_generator.Get(ModelObject, ModelSolution, indicator)
 
+            case 'ortools_cp':
+
+                from .result import ortools_cp_result_generator
+                return ortools_cp_result_generator.Get(ModelObject, ModelSolution, indicator)
+
             case 'gekko':
 
                 from .result import gekko_result_generator
                 return gekko_result_generator.Get(ModelObject, ModelSolution, indicator)
 
             case 'picos':
 
@@ -117,14 +133,20 @@
                 return pymprog_result_generator.Get(ModelObject, ModelSolution, indicator)
 
             case 'cplex':
 
                 from .result import cplex_result_generator
                 return cplex_result_generator.Get(ModelObject, ModelSolution, indicator)
 
+            case 'cplex_cp':
+
+                from .result import cplex_cp_result_generator
+                return cplex_cp_result_generator.Get(ModelObject, ModelSolution, indicator)
+
+
             case 'gurobi':
 
                 from .result import gurobi_result_generator
                 return gurobi_result_generator.Get(ModelObject, ModelSolution, indicator)
 
             case 'xpress':
```

### Comparing `feloopy-0.2.3/feloopy/generators/solution/feloopy_solution_generator.py` & `feloopy-0.2.31/feloopy/generators/solution/feloopy_solution_generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,28 +10,28 @@
         x,y, status = model_object.solve(fitness_function)
         time_solve_end = timeit.default_timer()
         return  x,y,time_solve_begin,time_solve_end, status
     
     else:
 
         Multiplier = {'max': 1, 'min': -1}
-        dir = Multiplier[objectives_directions[objective_number]]
+        directions = Multiplier[objectives_directions[objective_number]]
         time_solve_begin = []
         time_solve_end = []
-        bestreward = [-dir*np.inf]
-        best_reward_found = -dir*np.inf
+        bestreward = [-directions*np.inf]
+        best_reward_found = -directions*np.inf
         for i in range(number_of_times):
             time_solve_begin.append(timeit.default_timer())
             best_agent, best_reward, status = model_object.solve(fitness_function)
             time_solve_end.append(timeit.default_timer())
             Result = [best_agent, best_reward]
             Result[1] = np.asarray(Result[1])
             Result[1] = Result[1].item()
             bestreward.append(best_reward)
-            if dir*(Result[1]) >= dir*(best_reward_found):
+            if directions*(Result[1]) >= directions*(best_reward_found):
                 best_agent_found = Result[0]
                 best_reward_found = Result[1]
         bestreward.pop(0)
 
         print()
         hour = []
         min = []
```

### Comparing `feloopy-0.2.3/feloopy/generators/solution/linopy_solution_generator.py` & `feloopy-0.2.31/feloopy/generators/solution/mip_solution_generator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,48 @@
-from linopy import Model as LINOPYMODEL
+import mip as mip_interface
 import timeit
 
-linopy_solver_selector = {'cbc': 'cbc', 
-                          'glpk': 'glpk', 
-                          'highs': 'highs',
-                          'gurobi': 'gurobi', 
-                          'xpress': 'xpress', 
-                          'cplex': 'cplex'}
+mip_solver_selector = {'cbc': 'cbc'}
 
-def generate_solution(model_object, objectives_list, constraints_list, dir, labels, mode, solver_name, objective_number=0, algorithm_options=None, user_email=None):
+def generate_solution(features):
+
+    model_object = features['model_object_before_solve']
+    model_objectives = features['objectives']
+    model_constraints = features['constraints']
+    directions = features['directions']
+    constraint_labels= features['constraint_labels']
+    debug = features['debug_mode']
+    time_limit = features['time_limit']
+    absolute_gap = features['absolute_gap']
+    relative_gap = features['relative_gap']
+    thread_count = features['thread_count']
+    solver_name = features['solver_name']
+    objective_id = features['objective_being_optimized']
+    log = features['log']
+    save = features['save_solver_log']
+    save_model = features['write_model_file']
+    email = features['email_address']
+    max_iterations= features['max_iterations']
+    solver_options= features['solver_options']
     
-    if solver_name not in linopy_solver_selector.keys():
-        raise RuntimeError("Using solver '%s' is not supported by 'linopy'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
+    if solver_name not in mip_solver_selector.keys():
+        raise RuntimeError("Using solver '%s' is not supported by 'mip'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
     
-    match mode:
+    match debug:
 
         case False:
 
-            match dir[objective_number]:
+            for constraint in model_constraints:
+                model_object += constraint
+
+            match directions[objective_id]:
                 case "min":
-                    model_object.add_objective(objectives_list[objective_number])
+                    model_object.objective = mip_interface.minimize(model_objectives[objective_id]) 
                 case "max":
-                    model_object.add_objective(-objectives_list[objective_number])
-
-            for constraint in constraints_list:
-                model_object.add_constraints(constraint)
-    
+                    model_object.objective = mip_interface.maximize(model_objectives[objective_id])
+                
             time_solve_begin = timeit.default_timer()
-            result = model_object.solve(solver_name=solver_name)
+            result = model_object.optimize()
             time_solve_end = timeit.default_timer()
-            generated_solution = [result, [time_solve_begin, time_solve_end]]
-        
+            generated_solution = [ result, [time_solve_begin, time_solve_end]]
+    
     return generated_solution
```

### Comparing `feloopy-0.2.3/feloopy/generators/solution/mealpy_solution_generator.py` & `feloopy-0.2.31/feloopy/generators/solution/mealpy_solution_generator.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,29 +34,29 @@
                 model_object.history.save_runtime_chart(filename="results/rtc")
                 model_object.history.save_exploration_exploitation_chart(filename="results/eec")
                 model_object.history.save_diversity_chart(filename="results/dc")
 
     else:
 
         Multiplier = {'max': 1, 'min': -1}
-        dir = Multiplier[objectives_directions[objective_number]]
+        directions = Multiplier[objectives_directions[objective_number]]
         time_solve_begin = []
         time_solve_end = []
-        bestreward = [-dir*np.inf]
-        best_reward_found = -dir*np.inf
+        bestreward = [-directions*np.inf]
+        best_reward_found = -directions*np.inf
 
         for i in range(number_of_times):
             time_solve_begin.append(timeit.default_timer())
             best_agent, best_reward = model_object.solve(problem)
             time_solve_end.append(timeit.default_timer())
             Result = [best_agent, best_reward]
             Result[1] = np.asarray(Result[1])
             Result[1] = Result[1].item()
             bestreward.append(best_reward)
-            if dir*(Result[1]) >= dir*(best_reward_found):
+            if directions*(Result[1]) >= directions*(best_reward_found):
                 best_agent_found = Result[0]
                 best_reward_found = Result[1]
         bestreward.pop(0)
 
         print()
         hour = []
         min = []
```

### Comparing `feloopy-0.2.3/feloopy/generators/solution/ortools_solution_generator.py` & `feloopy-0.2.31/feloopy/generators/solution/ortools_solution_generator.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,34 +14,71 @@
     'cplex': 'CPLEX_MIXED_INTEGER_PROGRAMMING',
     'xpress_': 'XPRESS_LINEAR_PROGRAMMING',
     'xpress': 'XPRESS_MIXED_INTEGER_PROGRAMMING',
     'glpk_': 'GLPK_LINEAR_PROGRAMMING',
     'glpk': 'GLPK_MIXED_INTEGER_PROGRAMMING'
 }
 
-def generate_solution(model_object, objectives_list, constraints_list, dir, labels, mode, solver_name, objective_number=0, algorithm_options=None, user_email=None):
+def generate_solution(features):
 
+    model_object = features['model_object_before_solve']
+    model_objectives = features['objectives']
+    model_constraints = features['constraints']
+    directions = features['directions']
+    constraint_labels= features['constraint_labels']
+    debug = features['debug_mode']
+    time_limit = features['time_limit']
+    absolute_gap = features['absolute_gap']
+    relative_gap = features['relative_gap']
+    thread_count = features['thread_count']
+    solver_name = features['solver_name']
+    objective_id = features['objective_being_optimized']
+    log = features['log']
+    save = features['save_solver_log']
+    save_model = features['write_model_file']
+    email = features['email_address']
+    max_iterations= features['max_iterations']
+    solver_options= features['solver_options']
+    
     if solver_name not in ortools_solver_selector.keys():
         raise RuntimeError("Using solver '%s' is not supported by 'ortools'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
     
-    match mode:
+    match debug:
 
         case False:
 
-            match dir[objective_number]:
+            match directions[objective_id]:
 
                 case "min":
-                    model_object.Minimize(objectives_list[objective_number])
+                    model_object.Minimize(model_objectives[objective_id])
 
                 case "max":
-                    model_object.Maximize(objectives_list[objective_number])
+                    model_object.Maximize(model_objectives[objective_id])
 
-            for constraint in constraints_list:
+            for constraint in model_constraints:
                 model_object.Add(constraint)
 
             model_object.CreateSolver(ortools_solver_selector[solver_name])
+            solverParams = ortools_interface.MPSolverParameters()
+
+            if time_limit != None:
+                model_object.set_time_limit(time_limit)
+
+            if thread_count != None:
+                model_object.SetNumThreads(thread_count)
+
+            if relative_gap !=None:
+                solverParams.SetDoubleParam(solverParams.RELATIVE_MIP_GAP, relative_gap)
+
+            if absolute_gap != None:
+                "None"
+                
+            if log:
+
+                "None"
+
             time_solve_begin = timeit.default_timer()
             result = model_object.Solve()
             time_solve_end = timeit.default_timer()
             generated_solution = [result, [time_solve_begin, time_solve_end]]
     
     return generated_solution
```

### Comparing `feloopy-0.2.3/feloopy/generators/solution/pyomo_solution_generator.py` & `feloopy-0.2.31/feloopy/generators/solution/pyomo_solution_generator.py`

 * *Files 26% similar despite different names*

```diff
@@ -44,77 +44,116 @@
     'conopt_online': 'conopt',
     'couenne_online': 'couenne',
     'cplex_online': 'cplex',
     'filmint_online': 'filmint',
     'filter_online': 'filter',
     'ipopt_online': 'ipopt',
     'knitro_online': 'knitro',
-    'l-bfgs-b_online': 'l-bfgs-b',
+    'l-bfgs-b_online': 'l-bfgs-variable_bound',
     'lancelot_online': 'lancelot',
     'lgo_online': 'lgo',
     'loqo_online': 'loqo',
     'minlp_online': 'minlp',
     'minos_online': 'minos',
     'minto_online': 'minto',
     'mosek_online': 'mosek',
     'octeract_online': 'octeract',
     'ooqp_online': 'ooqp',
     'path_online': 'path',
     'raposa_online': 'raposa',
     'snopt_online': 'snopt'
 }
 
-def generate_solution(model_object, objectives_list, constraints_list, dir, labels, mode, solver_name, objective_number=0, algorithm_options=None, user_email=None):
+def generate_solution(features):
 
-    match mode:
+    model_object = features['model_object_before_solve']
+    model_objectives = features['objectives']
+    model_constraints = features['constraints']
+    directions = features['directions']
+    constraint_labels= features['constraint_labels']
+    debug = features['debug_mode']
+    time_limit = features['time_limit']
+    absolute_gap = features['absolute_gap']
+    relative_gap = features['relative_gap']
+    thread_count = features['thread_count']
+    solver_name = features['solver_name']
+    objective_id = features['objective_being_optimized']
+    log = features['log']
+    save = features['save_solver_log']
+    save_model = features['write_model_file']
+    email = features['email_address']
+    max_iterations= features['max_iterations']
+    solver_options= features['solver_options']
+    
+    if log:
+        tee = True
+    else:
+        tee = False
+
+    if max_iterations != None:
+        "None"
+
+    match debug:
 
         case False:
 
-            match dir[objective_number]:
+            match directions[objective_id]:
 
                 case "min":
-                    model_object.OBJ = pyomo_interface.Objective(expr=objectives_list[objective_number], sense=pyomo_interface.minimize)
+                    model_object.OBJ = pyomo_interface.Objective(expr=model_objectives[objective_id], sense=pyomo_interface.minimize)
                 
                 case "max":
-                    model_object.OBJ = pyomo_interface.Objective(expr=objectives_list[objective_number], sense=pyomo_interface.maximize)
+                    model_object.OBJ = pyomo_interface.Objective(expr=model_objectives[objective_id], sense=pyomo_interface.maximize)
 
             model_object.constraint = pyomo_interface.ConstraintList()
 
-            for element in constraints_list:
+            for element in model_constraints:
 
                 model_object.constraint.add(expr=element)
 
             if 'online' not in solver_name:
                 
                 if solver_name not in pyomo_offline_solver_selector.keys():
 
                      raise RuntimeError("Using solver '%s' is not supported by 'pyomo'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
                 
                 solver_manager = pyomo_interface.SolverFactory(pyomo_offline_solver_selector[solver_name])
 
-                if algorithm_options == None:
+                if thread_count != None:
+                
+                    solver_manager.options['threads'] = thread_count
+
+                if time_limit != None:
 
+                    solver_manager.options['timelimit'] = time_limit 
+
+                if relative_gap != None:
+
+                    solver_manager.options['mipgap'] = relative_gap
+                
+                if len(solver_options) == 0:
+                    
                     time_solve_begin = timeit.default_timer()
-                    result = solver_manager.solve(model_object)
+                    result = solver_manager.solve(model_object, tee=tee)
                     time_solve_end = timeit.default_timer()
 
                 else:
 
                     time_solve_begin = timeit.default_timer()
-                    result = solver_manager.solve(model_object, options=algorithm_options)
+                    result = solver_manager.solve(model_object, tee=tee, options=solver_options)
                     time_solve_end = timeit.default_timer()     
 
             else:
                 
                 if solver_name not in pyomo_online_solver_selector.keys():
 
                     raise RuntimeError("Using solver '%s' is not supported by 'pyomo'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
                 
-                os.environ['NEOS_EMAIL'] = user_email
+                os.environ['NEOS_EMAIL'] = email
                 solver_manager = pyomo_interface.SolverManagerFactory('neos')
                 time_solve_begin = timeit.default_timer()
-                result = solver_manager.solve(model_object, solver=pyomo_online_solver_selector[solver_name])
+                result = solver_manager.solve(model_object, solver=pyomo_online_solver_selector[solver_name], tee=tee)
                 time_solve_end = timeit.default_timer()
 
             generated_solution = result, [time_solve_begin, time_solve_end]
         
     return generated_solution
```

### Comparing `feloopy-0.2.3/feloopy/generators/variable/cylp_variable_generator.py` & `feloopy-0.2.31/feloopy/generators/variable/mip_variable_generator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,81 +1,88 @@
+import mip as mip_interface
 import itertools as it
 
 sets = it.product
 
-def generate_variable(modelobject, var_type, var_name, b, dim=0):
+BINARY = mip_interface.BINARY
+POSITIVE = mip_interface.CONTINUOUS
+INTEGER = mip_interface.INTEGER
+FREE = mip_interface.CONTINUOUS
 
-    match var_type:
+def generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim=0):
+
+    match variable_type:
 
         case 'pvar':
 
             '''
 
             Positive Variable Generator
 
 
             '''
 
-            if dim == 0:
-                GeneratedVariable =  modelobject.addVariable(var_name, 1, isInt=False)
+            if variable_dim == 0:
+                GeneratedVariable =  model_object.add_var(var_type=POSITIVE)
             else:
-                if len(dim) == 1:
-                    GeneratedVariable =  {key: modelobject.addVariable(f"{var_name}{key}", 1, isInt=False) for key in dim[0]}
+                if len(variable_dim) == 1:
+                    GeneratedVariable =  {key: model_object.add_var(var_type=POSITIVE) for key in variable_dim[0]}
                 else:
-                    GeneratedVariable =  {key: modelobject.addVariable(f"{var_name}{key}", 1, isInt=False) for key in it.product(*dim)}
-                    
-                    
+                    GeneratedVariable =  {key: model_object.add_var(var_type=POSITIVE) for key in it.product(*variable_dim)}
+                            
         case 'bvar':
 
             '''
 
             Binary Variable Generator
 
 
             '''
 
-            if dim == 0:
-                GeneratedVariable =  modelobject.addVariable(var_name, 0, isInt=False)
+            if variable_dim == 0:
+                GeneratedVariable =  model_object.add_var(var_type=BINARY)
             else:
-                if len(dim) == 1:
-                    GeneratedVariable =  {key: modelobject.addVariable(f"{var_name}{key}", 1, isInt=True) for key in dim[0]}
+                if len(variable_dim) == 1:
+                    GeneratedVariable =  {key: model_object.add_var(var_type=BINARY) for key in variable_dim[0]}
                 else:
-                    GeneratedVariable =  {key: modelobject.addVariable(f"{var_name}{key}", 1, isInt=True) for key in it.product(*dim)}
-
-
+                    GeneratedVariable =  {key: model_object.add_var(var_type=BINARY) for key in it.product(*variable_dim)}
+      
                     
         case 'ivar':
 
             '''
 
             Integer Variable Generator
 
 
             '''
 
-            if dim == 0:
-                GeneratedVariable =  modelobject.addVariable(var_name, 1, isInt=False)
+            if variable_dim == 0:
+                GeneratedVariable =  model_object.add_var(var_type=INTEGER)
             else:
-                if len(dim) == 1:
-                    GeneratedVariable =  {key: modelobject.addVariable(f"{var_name}{key}", 1, isInt=True) for key in dim[0]}
+                if len(variable_dim) == 1:
+                    GeneratedVariable =  {key: model_object.add_var(var_type=INTEGER) for key in variable_dim[0]}
                 else:
-                    GeneratedVariable =  {key: modelobject.addVariable(f"{var_name}{key}", 1, isInt=True) for key in it.product(*dim)}
+                    GeneratedVariable =  {key: model_object.add_var(var_type=INTEGER) for key in it.product(*variable_dim)}
 
                             
         case 'fvar':
 
             '''
 
             Free Variable Generator
 
 
             '''
-
-            if dim == 0:
-                GeneratedVariable =  modelobject.addVariable(var_name, 1, isInt=False)
+            if variable_dim == 0:
+                GeneratedVariable =  model_object.add_var(var_type=POSITIVE)
             else:
-                if len(dim) == 1:
-                    GeneratedVariable =  {key: modelobject.addVariable(f"{var_name}{key}", 1, isInt=False) for key in dim[0]}
+                if len(variable_dim) == 1:
+                    GeneratedVariable =  {key: model_object.add_var(var_type=POSITIVE) for key in variable_dim[0]}
                 else:
-                    GeneratedVariable =  {key: modelobject.addVariable(f"{var_name}{key}", 1, isInt=False) for key in it.product(*dim)}
-                   
-    return GeneratedVariable
+                    GeneratedVariable =  {key: model_object.add_var(var_type=POSITIVE) for key in it.product(*variable_dim)}
+
+
+
+    
+    return  GeneratedVariable
+
```

### Comparing `feloopy-0.2.3/feloopy/generators/variable/linopy_variable_generator.py` & `feloopy-0.2.31/feloopy/generators/variable/pyomo_variable_generator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,85 @@
+import pyomo.environ as pyomo_interface
 import itertools as it
-import pandas as pd
 
 sets = it.product
 
-def generate_variable(modelobject, var_type, var_name, b, dim=0):
+variable = pyomo_interface.Var
 
-    match var_type:
+POSITIVE = pyomo_interface.NonNegativeReals
+BINARY = pyomo_interface.Binary
+INTEGER = pyomo_interface.NonNegativeIntegers
+FREE = pyomo_interface.Reals
+
+
+def generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim=0):
+
+    match variable_type:
 
         case 'pvar':
 
             '''
 
             Positive Variable Generator
 
 
             '''
-            if dim == 0:
-                GeneratedVariable =  modelobject.add_variables(lower=b[0], upper=b[1], name=var_name)
+
+            if variable_dim == 0:
+
+                model_object.add_component(variable_name, variable(initialize=0, domain=POSITIVE, bounds=(variable_bound[0], variable_bound[1])))
+
             else:
-                GeneratedVariable =  modelobject.add_variables(lower=b[0], upper=b[1], coords=pd.Index(dim), name=var_name)
-      
+                model_object.add_component(variable_name, variable([i for i in sets(*variable_dim)], domain=POSITIVE, bounds=(variable_bound[0], variable_bound[1])))
+
         case 'bvar':
 
             '''
 
             Binary Variable Generator
 
 
             '''
 
-            if dim == 0:
-                GeneratedVariable =  modelobject.add_variables(name=var_name, binary=True)
+            if variable_dim == 0:
+
+                model_object.add_component(variable_name, variable(domain=BINARY, bounds=(variable_bound[0], variable_bound[1])))
+
             else:
-                GeneratedVariable =  modelobject.add_variables(coords=pd.Index(dim), name=var_name,  binary=True)
 
-                    
-                    
+                model_object.add_component(variable_name, variable([i for i in sets(*variable_dim)], domain=BINARY, bounds=(variable_bound[0], variable_bound[1])))
+
         case 'ivar':
 
             '''
 
             Integer Variable Generator
 
 
             '''
 
-            if dim == 0:
-                GeneratedVariable =  modelobject.add_variables(lower=b[0], upper=b[1], name=var_name, binary=True)
+            if variable_dim == 0:
+
+                model_object.add_component(variable_name, variable(domain=INTEGER, bounds=(variable_bound[0], variable_bound[1])))
+
             else:
-                GeneratedVariable =  modelobject.add_variables(lower=b[0], upper=b[1], coords=pd.Index(dim), name=var_name,  integer=True)
 
-                            
+                model_object.add_component(variable_name, variable([i for i in sets(*variable_dim)], domain=INTEGER, bounds=(variable_bound[0], variable_bound[1])))
+
         case 'fvar':
 
             '''
 
             Free Variable Generator
 
 
             '''
 
-            if dim == 0:
-                GeneratedVariable =  modelobject.add_variables(lower=b[0], upper=b[1], name=var_name)
+            if variable_dim == 0:
+
+                model_object.add_component(variable_name, variable(domain=FREE, bounds=(variable_bound[0], variable_bound[1])))
+
             else:
-                GeneratedVariable =  modelobject.add_variables(lower=b[0], upper=b[1], coords=pd.Index(dim), name=var_name)
 
-    
-    return  GeneratedVariable
-    
+                model_object.add_component(variable_name, variable([i for i in sets(*variable_dim)], domain=FREE, bounds=(variable_bound[0], variable_bound[1])))
+
+    return model_object.component(variable_name)
```

### Comparing `feloopy-0.2.3/feloopy/generators/variable/ortools_variable_generator.py` & `feloopy-0.2.31/feloopy/generators/variable/ortools_cp_variable_generator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,129 +1,124 @@
 import itertools as it
 
 sets = it.product
 
+def generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim=0):
 
-def generate_variable(modelobject, var_type, var_name, b, dim=0):
-
-    if b[0] == None: b[0] = -modelobject.infinity()
-    
-    if b[1] == None: b[1] = modelobject.infinity()
-
-    match var_type:
+    match variable_type:
 
         case 'pvar':
 
             '''
 
             Positive Variable Generator
 
 
             '''
 
-            
-            if dim == 0:
+            if variable_bound[0] == 0:
+
+                variable_bound[0] = 0
+
+            if variable_dim == 0:
                 
-                GeneratedVariable =  modelobject.NumVar(b[0], b[1], var_name)
+                GeneratedVariable =  model_object.NewNumVar(variable_bound[0], variable_bound[1], variable_name)
             
             else:
                 
-                if len(dim) == 1:
+                if len(variable_dim) == 1:
                     
-                    GeneratedVariable =  {key: modelobject.NumVar(b[0], b[1], f"{var_name}{key}") for key in dim[0]}
+                    GeneratedVariable =  {key: model_object.NewNumVar(variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in variable_dim[0]}
                 
                 else:
                     
-                    GeneratedVariable =  {key: modelobject.NumVar(b[0], b[1], f"{var_name}{key}") for key in it.product(*dim)}
+                    GeneratedVariable =  {key: model_object.NewNumVar(variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in it.product(*variable_dim)}
 
 
                     
         case 'bvar':
 
             '''
 
             Binary Variable Generator
 
 
             '''
 
-            if dim == 0:
+            if variable_bound[0] == 0:
+
+                variable_bound[0] = 0
+            
+            
+            if variable_bound[1] == 1:
+
+                variable_bound[1] = 1
+
+            if variable_dim == 0:
                 
-                GeneratedVariable =  modelobject.IntVar(b[0], b[1], var_name)
+                GeneratedVariable =  model_object.NewIntVar(variable_bound[0], variable_bound[1], variable_name)
             
             else:
                 
-                if len(dim) == 1:
+                if len(variable_dim) == 1:
                     
-                    GeneratedVariable =  {key: modelobject.IntVar(b[0], b[1], f"{var_name}{key}") for key in dim[0]}
+                    GeneratedVariable =  {key: model_object.NewIntVar(variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in variable_dim[0]}
                 
                 else:
                     
-                    GeneratedVariable =  {key: modelobject.IntVar(b[0], b[1], f"{var_name}{key}") for key in it.product(*dim)}
+                    GeneratedVariable =  {key: model_object.NewIntVar(variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in it.product(*variable_dim)}
 
                   
                     
         case 'ivar':
 
             '''
 
             Integer Variable Generator
 
 
             '''
 
-            if b[0] == 0:
-
-                b[0] = 0
-
-            if b[1] == None:
+            if variable_bound[0] == 0:
 
-                b[1] = modelobject.infinity()
+                variable_bound[0] = 0
 
-            if dim == 0:
+            if variable_dim == 0:
 
-                GeneratedVariable = modelobject.IntVar(b[0], b[1], var_name)
+                GeneratedVariable = model_object.NewIntVar(variable_bound[0], variable_bound[1], variable_name)
 
             else:
                 
-                if len(dim) == 1:
+                if len(variable_dim) == 1:
                     
-                    GeneratedVariable = {key: modelobject.IntVar(b[0], b[1], f"{var_name}{key}") for key in dim[0]}
+                    GeneratedVariable = {key: model_object.NewIntVar(variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in variable_dim[0]}
                 
                 else:
                     
-                    GeneratedVariable = {key: modelobject.IntVar(b[0], b[1], f"{var_name}{key}") for key in it.product(*dim)}
+                    GeneratedVariable = {key: model_object.NewIntVar(variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in it.product(*variable_dim)}
 
 
 
         case 'fvar':
 
             '''
 
             Free Variable Generator
 
 
             '''
 
-            if b[0] == None:
-                
-                b[0] = -modelobject.infinity()
-            
-            if b[1] == None:
-                
-                b[1] = modelobject.infinity()
-
-            if dim == 0:
+            if variable_dim == 0:
                 
-                GeneratedVariable = modelobject.NumVar(b[0], b[1], var_name)
+                GeneratedVariable = model_object.NewNumVar(variable_bound[0], variable_bound[1], variable_name)
             
             else:
                 
-                if len(dim) == 1:
+                if len(variable_dim) == 1:
                     
-                    GeneratedVariable = {key: modelobject.NumVar(b[0], b[1], f"{var_name}{key}") for key in dim[0]}
+                    GeneratedVariable = {key: model_object.NewNumVar(variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in variable_dim[0]}
                 
                 else:
                     
-                    GeneratedVariable = {key: modelobject.NumVar(b[0], b[1], f"{var_name}{key}") for key in it.product(*dim)}
+                    GeneratedVariable = {key: model_object.NewNumVar(variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in it.product(*variable_dim)}
     
     return GeneratedVariable
```

### Comparing `feloopy-0.2.3/feloopy/generators/variable/pymprog_variable_generator.py` & `feloopy-0.2.31/feloopy/generators/variable/pymprog_variable_generator.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,81 +2,81 @@
 import itertools as it
 
 sets = it.product
 
 VariableGenerator = pymprog_interface.var
 
 
-def generate_variable(modelobject, var_type, var_name, b, dim=0):
+def generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim=0):
 
-    match var_type:
+    match variable_type:
 
         case 'pvar':
 
             '''
 
             Positive Variable Generator
 
 
             '''
 
-            if dim == 0:
-                GeneratedVariable =  VariableGenerator(var_name, bounds=(b[0], b[1]))
+            if variable_dim == 0:
+                GeneratedVariable =  VariableGenerator(variable_name, bounds=(variable_bound[0], variable_bound[1]))
             else:
-                if len(dim) == 1:
-                    GeneratedVariable =  {key: VariableGenerator(var_name, bounds=(b[0], b[1])) for key in dim[0]}
+                if len(variable_dim) == 1:
+                    GeneratedVariable =  {key: VariableGenerator(variable_name, bounds=(variable_bound[0], variable_bound[1])) for key in variable_dim[0]}
                 else:
-                    GeneratedVariable =  {key: VariableGenerator(var_name, bounds=(b[0], b[1])) for key in it.product(*dim)}
+                    GeneratedVariable =  {key: VariableGenerator(variable_name, bounds=(variable_bound[0], variable_bound[1])) for key in it.product(*variable_dim)}
 
 
         case 'bvar':
 
             '''
 
             Binary Variable Generator
 
 
             '''
-            if dim == 0:
-                GeneratedVariable =  VariableGenerator(var_name, bounds=(b[0], b[1]), kind=int)
+            if variable_dim == 0:
+                GeneratedVariable =  VariableGenerator(variable_name, bounds=(variable_bound[0], variable_bound[1]), kind=int)
             else:
-                if len(dim) == 1:
-                    GeneratedVariable =  {key: VariableGenerator(var_name, bounds=(b[0], b[1]), kind=int) for key in dim[0]}
+                if len(variable_dim) == 1:
+                    GeneratedVariable =  {key: VariableGenerator(variable_name, bounds=(variable_bound[0], variable_bound[1]), kind=int) for key in variable_dim[0]}
                 else:
-                    GeneratedVariable =  {key: VariableGenerator(var_name, bounds=(b[0], b[1]), kind=int) for key in it.product(*dim)}
+                    GeneratedVariable =  {key: VariableGenerator(variable_name, bounds=(variable_bound[0], variable_bound[1]), kind=int) for key in it.product(*variable_dim)}
        
         case 'ivar':
 
             '''
 
             Integer Variable Generator
 
 
             '''
 
-            if dim == 0:
-                GeneratedVariable =  VariableGenerator(var_name, bounds=(b[0], b[1]), kind=int)
+            if variable_dim == 0:
+                GeneratedVariable =  VariableGenerator(variable_name, bounds=(variable_bound[0], variable_bound[1]), kind=int)
             else:
-                if len(dim) == 1:
-                    GeneratedVariable =  {key: VariableGenerator(var_name, bounds=(b[0], b[1]), kind=int) for key in dim[0]}
+                if len(variable_dim) == 1:
+                    GeneratedVariable =  {key: VariableGenerator(variable_name, bounds=(variable_bound[0], variable_bound[1]), kind=int) for key in variable_dim[0]}
                 else:
-                    GeneratedVariable =  {key: VariableGenerator(var_name, bounds=(b[0], b[1]), kind=int) for key in it.product(*dim)}
+                    GeneratedVariable =  {key: VariableGenerator(variable_name, bounds=(variable_bound[0], variable_bound[1]), kind=int) for key in it.product(*variable_dim)}
 
                 
         case 'fvar':
 
             '''
 
             Free Variable Generator
 
 
             '''
 
-            if dim == 0:
-                GeneratedVariable =  VariableGenerator(var_name, bounds=(b[0], b[1]))
+            if variable_dim == 0:
+                GeneratedVariable =  VariableGenerator(variable_name, bounds=(variable_bound[0], variable_bound[1]))
             else:
-                if len(dim) == 1:
-                    GeneratedVariable =  {key: VariableGenerator(var_name, bounds=(b[0], b[1])) for key in dim[0]}
+                if len(variable_dim) == 1:
+                    GeneratedVariable =  {key: VariableGenerator(variable_name, bounds=(variable_bound[0], variable_bound[1])) for key in variable_dim[0]}
                 else:
-                    GeneratedVariable =  {key: VariableGenerator(var_name, bounds=(b[0], b[1])) for key in it.product(*dim)}
+                    GeneratedVariable =  {key: VariableGenerator(variable_name, bounds=(variable_bound[0], variable_bound[1])) for key in it.product(*variable_dim)}
 
     return  GeneratedVariable
```

### Comparing `feloopy-0.2.3/feloopy/generators/variable/xpress_variable_generator.py` & `feloopy-0.2.31/feloopy/generators/variable/xpress_variable_generator.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,137 +5,137 @@
 
 VariableGenerator = xpress_interface.var
 
 INFINITY = xpress_interface.infinity
 BINARY = xpress_interface.binary
 INTEGER = xpress_interface.integer
 
-def generate_variable(modelobject, var_type, var_name, b, dim=0):
+def generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim=0):
 
-    if b[0] == None: b[0] = -INFINITY
+    if variable_bound[0] == None: variable_bound[0] = -INFINITY
     
-    if b[1] == None: b[1] = +INFINITY
+    if variable_bound[1] == None: variable_bound[1] = +INFINITY
 
-    match var_type:
+    match variable_type:
 
         case 'pvar':
 
             '''
 
             Positive Variable Generator
 
 
             '''
 
-            if dim == 0:
+            if variable_dim == 0:
                 
-                GeneratedVariable =VariableGenerator(lb=b[0],ub=b[1])
+                GeneratedVariable =VariableGenerator(lb=variable_bound[0],ub=variable_bound[1])
                 
-                modelobject.addVariable(GeneratedVariable)
+                model_object.addVariable(GeneratedVariable)
                 
             else:
                 
-                if len(dim) == 1:
+                if len(variable_dim) == 1:
                     
-                    GeneratedVariable = [VariableGenerator(lb=b[0],ub=b[1]) for key in dim[0]]
+                    GeneratedVariable = [VariableGenerator(lb=variable_bound[0],ub=variable_bound[1]) for key in variable_dim[0]]
                     
-                    modelobject.addVariable(GeneratedVariable)
+                    model_object.addVariable(GeneratedVariable)
                     
                 else:
                     
-                    GeneratedVariable = {key:VariableGenerator(name= f"{var_name}{key}", lb=b[0],ub=b[1]) for key in sets(*dim)}
+                    GeneratedVariable = {key:VariableGenerator(name= f"{variable_name}{key}", lb=variable_bound[0],ub=variable_bound[1]) for key in sets(*variable_dim)}
                     
-                    modelobject.addVariable(GeneratedVariable)
+                    model_object.addVariable(GeneratedVariable)
                     
         case 'bvar':
 
             '''
 
             Binary Variable Generator
 
 
             '''
 
-            if dim == 0:
+            if variable_dim == 0:
                 
                 GeneratedVariable =VariableGenerator(vartype=BINARY)
                 
-                modelobject.addVariable(GeneratedVariable)
+                model_object.addVariable(GeneratedVariable)
                 
             else:
                 
-                if len(dim) == 1:
+                if len(variable_dim) == 1:
                     
-                    GeneratedVariable = [VariableGenerator(vartype=BINARY) for key in dim[0]]
+                    GeneratedVariable = [VariableGenerator(vartype=BINARY) for key in variable_dim[0]]
                     
-                    modelobject.addVariable(GeneratedVariable)
+                    model_object.addVariable(GeneratedVariable)
                     
                 else:
                     
-                    GeneratedVariable = {key:VariableGenerator(name= f"{var_name}{key}", lb=b[0],ub=b[1],vartype=BINARY) for key in sets(*dim)}
+                    GeneratedVariable = {key:VariableGenerator(name= f"{variable_name}{key}", lb=variable_bound[0],ub=variable_bound[1],vartype=BINARY) for key in sets(*variable_dim)}
                     
-                    modelobject.addVariable(GeneratedVariable)
+                    model_object.addVariable(GeneratedVariable)
                     
         case 'ivar':
 
             '''
 
             Integer Variable Generator
 
 
             '''
 
-            if dim == 0:
+            if variable_dim == 0:
                 
                 GeneratedVariable =VariableGenerator(vartype=INTEGER)
                 
-                modelobject.addVariable(GeneratedVariable)
+                model_object.addVariable(GeneratedVariable)
                 
             else:
                 
-                if len(dim) == 1:
+                if len(variable_dim) == 1:
                     
-                    GeneratedVariable = {key:VariableGenerator(vartype=INTEGER) for key in dim[0]}
+                    GeneratedVariable = {key:VariableGenerator(vartype=INTEGER) for key in variable_dim[0]}
                     
-                    modelobject.addVariable(GeneratedVariable)
+                    model_object.addVariable(GeneratedVariable)
                     
                 else:
                     
-                    GeneratedVariable = {key:VariableGenerator(name= f"{var_name}{key}", lb=b[0],ub=b[1],vartype=INTEGER) for key in sets(*dim)}
+                    GeneratedVariable = {key:VariableGenerator(name= f"{variable_name}{key}", lb=variable_bound[0],ub=variable_bound[1],vartype=INTEGER) for key in sets(*variable_dim)}
                     
-                    modelobject.addVariable(GeneratedVariable)
+                    model_object.addVariable(GeneratedVariable)
                     
         case 'fvar':
 
             '''
 
             Free Variable Generator
 
 
             '''
 
-            if dim == 0:
+            if variable_dim == 0:
                 
-                GeneratedVariable =VariableGenerator(lb=b[0],ub=b[1])
+                GeneratedVariable =VariableGenerator(lb=variable_bound[0],ub=variable_bound[1])
                 
-                modelobject.addVariable(GeneratedVariable)
+                model_object.addVariable(GeneratedVariable)
                 
             else:
                 
-                if len(dim) == 1:
+                if len(variable_dim) == 1:
                     
-                    GeneratedVariable = [VariableGenerator(lb=b[0],ub=b[1]) for key in dim[0]]
+                    GeneratedVariable = [VariableGenerator(lb=variable_bound[0],ub=variable_bound[1]) for key in variable_dim[0]]
                     
-                    modelobject.addVariable(GeneratedVariable)
+                    model_object.addVariable(GeneratedVariable)
                     
                 else:
                     
-                    GeneratedVariable = {key:VariableGenerator(name= f"{var_name}{key}", lb=b[0],ub=b[1]) for key in sets(*dim)}
+                    GeneratedVariable = {key:VariableGenerator(name= f"{variable_name}{key}", lb=variable_bound[0],ub=variable_bound[1]) for key in sets(*variable_dim)}
                     
-                    modelobject.addVariable(GeneratedVariable)
+                    model_object.addVariable(GeneratedVariable)
     
     return GeneratedVariable
```

### Comparing `feloopy-0.2.3/feloopy/generators/variable_generator.py` & `feloopy-0.2.31/feloopy/generators/variable_generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,84 @@
 def generate_variable(interface_name, model_object, variable_type, variable_name, variable_bound, variable_dim):
 
+    inputs = {'model_object': model_object, 
+              'variable_type': variable_type, 
+              'variable_name': variable_name, 
+              'variable_bound': variable_bound, 
+              'variable_dim': variable_dim }
+
     match interface_name:
 
         case 'pulp':
 
             from .variable import pulp_variable_generator
-            return pulp_variable_generator.generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim)
+            return pulp_variable_generator.generate_variable(**inputs)
 
         case 'pyomo':
 
             from .variable import pyomo_variable_generator
-            return pyomo_variable_generator.generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim)
+            return pyomo_variable_generator.generate_variable(**inputs)
 
         case 'ortools':
 
             from .variable import ortools_variable_generator
-            return ortools_variable_generator.generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim)
+            return ortools_variable_generator.generate_variable(**inputs)
+
+        case 'ortools_cp':
+
+            from .variable import ortools_cp_variable_generator
+            return ortools_cp_variable_generator.generate_variable(**inputs)
 
         case 'gekko':
 
             from .variable import gekko_variable_generator
-            return gekko_variable_generator.generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim)
+            return gekko_variable_generator.generate_variable(**inputs)
 
         case 'picos':
 
             from .variable import picos_variable_generator
-            return picos_variable_generator.generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim)
+            return picos_variable_generator.generate_variable(**inputs)
 
         case 'cvxpy':
 
             from .variable import cvxpy_variable_generator
-            return cvxpy_variable_generator.generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim)
+            return cvxpy_variable_generator.generate_variable(**inputs)
 
         case 'cylp':
 
             from .variable import cylp_variable_generator
-            return cylp_variable_generator.generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim)
+            return cylp_variable_generator.generate_variable(**inputs)
 
         case 'pymprog':
 
             from .variable import pymprog_variable_generator
-            return pymprog_variable_generator.generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim)
+            return pymprog_variable_generator.generate_variable(**inputs)
 
         case 'cplex':
 
             from .variable import cplex_variable_generator
-            return cplex_variable_generator.generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim)
+            return cplex_variable_generator.generate_variable(**inputs)
+
+        case 'cplex_cp':
+
+            from .variable import cplex_cp_variable_generator
+            return cplex_cp_variable_generator.generate_variable(**inputs)
 
         case 'gurobi':
 
             from .variable import gurobi_variable_generator
-            return gurobi_variable_generator.generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim)
+            return gurobi_variable_generator.generate_variable(**inputs)
 
         case 'xpress':
 
             from .variable import xpress_variable_generator
-            return xpress_variable_generator.generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim)
+            return xpress_variable_generator.generate_variable(**inputs)
 
         case 'mip':
 
             from .variable import mip_variable_generator
-            return mip_variable_generator.generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim)
+            return mip_variable_generator.generate_variable(**inputs)
 
         case 'linopy':
 
             from .variable import linopy_variable_generator
-            return linopy_variable_generator.generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim)
+            return linopy_variable_generator.generate_variable(**inputs)
```

### Comparing `feloopy-0.2.3/feloopy/operators/common.py` & `feloopy-0.2.31/feloopy/operators/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,19 +3,77 @@
 import os
 import sys
 import pandas as pd
 import numpy as np
 import itertools as it
 import matplotlib.style as style
 import matplotlib.pyplot as plt
+import math as mt
 
 from tabulate import tabulate as tb
 
 sets = it.product
 
+def random_number_generator(key):
+
+    return np.random.default_rng(key)
+
+def make_set(input): 
+
+    if type(input)==int: 
+
+        return range(input) 
+    
+    else: 
+
+        return set(input)
+    
+def make_uniform_param(rng, lb, ub, variable_dim=0):
+
+    if variable_dim == 0:
+
+        return rng.uniform(low=lb, high=ub)
+    
+    else:
+
+        return rng.uniform(low=lb, high=ub, size=([len(i) for i in variable_dim]))
+
+def exponent(input):
+    return np.exp(input)
+
+def floor(input):
+    return np.floor(input)
+
+def ceil(input):
+    return np.ceil(input)
+
+def round(input):
+    return np.round(input)
+
+def log_of_base(input, base):
+    return mt.log(input, base)
+
+def log(input):
+    return np.log(input)
+
+def log10(input):
+    return np.log10(input)
+
+def sqrt(input):
+    return np.sqrt(input)
+
+def sin(input):
+    return np.sin(input)
+
+def cos(input):
+    return np.cos(input)
+
+def power(input1, input2):
+    return input1**input2
+
 def install(package):
     '''
     Package Installer!
     ~~~~~~~~~~~~~~~~~~
 
     *package: enter a string representing the name of the package (e.g., 'numpy' or 'feloopy')
 
@@ -54,64 +112,72 @@
 def end_timer(show=False):
     '''
     Timer Ends Here!
     ~~~~~~~~~~~~~~~~
     '''
     global EndTime
     EndTime = timeit.default_timer()
-    sec = round((EndTime - StartTime), 3)% (24 * 3600)
+    sec = round(EndTime - StartTime)% (24 * 3600)
     hour = sec // 3600
     sec %= 3600
     min = sec // 60
     sec %= 60
     if show:
         print("Elapsed time (microseconds):", (EndTime-StartTime)*10**6)
         print("Elapsed time (hour:min:sec):", "%02d:%02d:%02d" % (hour, min, sec))
     return EndTime
 
-def load_from_excel(data_file: str, data_dimension: list, number_of_row_id_cols: int, number_of_col_id_rows: int, indices_list: list, sheet_name: str, path=None):
+
+def load_from_excel(data_file: str, data_dimension: list, shape: list, indices_list: None, sheet_name: str, path=None):
         
         '''
         Multi-Dimensional Excel Parameter Reader! 
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
         *data_file: Name of the dataset file (e.g., data.xlsx)
         *data_dimension: data_dimension of the dataset
-        *number_of_row_id_cols: Number of indices that exist in each row from left (e.g., 0, 1, 2, 3...)
-        *number_of_col_id_rows: Number of indices that exist in each column from top (e.g., 0, 1, 2, 3...)
+        *shape[0]: Number of indices that exist in each row from left (e.g., 0, 1, 2, 3...)
+        *shape[1]: Number of indices that exist in each column from top (e.g., 0, 1, 2, 3...)
         *indices_list: The string which accompanies index counter (e.g., if row0, row1, ... and col0,col1, then index is ['row','col'])
         *sheet_name: Name of the excel sheet in which the corresponding parameter exists.
         *path: specify directory of the dataset file (if not provided, the dataset file should exist in the same directory as the code.)
         '''
+
         if path == None:
             data_file = os.path.join(sys.path[0], data_file)
         else:
             data_file = path
 
-        parameter = pd.read_excel(data_file, header=[i for i in range(number_of_col_id_rows)], index_col=[i for i in range(number_of_row_id_cols)], sheet_name=sheet_name)
+        if len(shape) ==2:
 
-        if (number_of_row_id_cols == 1 and number_of_col_id_rows == 1) or (number_of_row_id_cols == 1 and number_of_col_id_rows == 0) or (number_of_row_id_cols == 0 and number_of_col_id_rows == 0) or (number_of_row_id_cols == 0 and number_of_col_id_rows == 1):
+            if (shape[0] == 1 and shape[1] == 1) or (shape[0] == 1 and shape[1] == 0) or (shape[0] == 0 and shape[1] == 0) or (shape[0] == 0 and shape[1] == 1):
 
-            return parameter.to_numpy()
+                return  pd.read_excel(data_file, index_col=0, sheet_name=sheet_name).to_numpy()
 
-        else:
+            else:
 
-            created_par = np.zeros(shape=([len(i) for i in data_dimension]))
+                parameter = pd.read_excel(data_file, header=[i for i in range(shape[1])], index_col=[i for i in range(shape[0])], sheet_name=sheet_name)
 
-            for keys in it.product(*data_dimension):
+                created_par = np.zeros(shape=([len(i) for i in data_dimension]))
 
-                try:
+                for keys in it.product(*data_dimension):
 
-                    created_par[keys] = parameter.loc[tuple([indices_list[i]+str(keys[i]) for i in range(number_of_row_id_cols)]), tuple([indices_list[i]+str(keys[i]) for i in range(number_of_row_id_cols, len(indices_list))])]
+                    try:
 
-                except:
+                        created_par[keys] = parameter.loc[tuple([indices_list[i]+str(keys[i]) for i in range(shape[0])]), tuple([indices_list[i]+str(keys[i]) for i in range(shape[0], len(indices_list))])]
 
-                    created_par[keys] = None
+                    except:
+
+                        created_par[keys] = None
+
+                return created_par
+        else:
+            par = pd.read_excel(data_file, index_col=0, sheet_name=sheet_name).to_numpy()
 
-            return created_par
+            return par.reshape(par.shape[0],)
 
 def version(INPUT):
 
     print(INPUT.__version__)
     
     return(INPUT)
```

### Comparing `feloopy-0.2.3/feloopy.egg-info/SOURCES.txt` & `feloopy-0.2.31/feloopy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,83 +5,104 @@
 feloopy/feloopy.py
 feloopy.egg-info/PKG-INFO
 feloopy.egg-info/SOURCES.txt
 feloopy.egg-info/dependency_links.txt
 feloopy.egg-info/requires.txt
 feloopy.egg-info/top_level.txt
 feloopy/algorithms/__init__.py
+feloopy/algorithms/constraint/__init__.py
 feloopy/algorithms/exact/__init__.py
 feloopy/algorithms/heuristic/DE.py
 feloopy/algorithms/heuristic/GA.py
 feloopy/algorithms/heuristic/GWO.py
 feloopy/algorithms/heuristic/SA.py
 feloopy/algorithms/heuristic/TS.py
 feloopy/algorithms/heuristic/__init__.py
+feloopy/classes/__init__.py
+feloopy/classes/empty.py
+feloopy/functions/__init__.py
+feloopy/functions/count_operators.py
+feloopy/functions/fix_operators.py
+feloopy/functions/heuristic_operators.py
+feloopy/functions/math_operators.py
+feloopy/functions/random_operators.py
+feloopy/functions/set_operators.py
+feloopy/functions/update_operators.py
 feloopy/generators/__init__.py
 feloopy/generators/model_generator.py
 feloopy/generators/result_generator.py
 feloopy/generators/solution_generator.py
 feloopy/generators/variable_generator.py
 feloopy/generators/model/__init__.py
+feloopy/generators/model/cplex_cp_model_generator.py
 feloopy/generators/model/cplex_model_generator.py
 feloopy/generators/model/cvxpy_model_generator.py
 feloopy/generators/model/cylp_model_generator.py
 feloopy/generators/model/feloopy_model_generator.py
 feloopy/generators/model/gekko_model_generator.py
 feloopy/generators/model/gurobi_model_generator.py
 feloopy/generators/model/linopy_model_generator.py
 feloopy/generators/model/mealpy_model_generator.py
 feloopy/generators/model/mip_model_generator.py
+feloopy/generators/model/ortools_cp_model_generator.py
 feloopy/generators/model/ortools_model_generator.py
 feloopy/generators/model/picos_model_generator.py
 feloopy/generators/model/pulp_model_generator.py
 feloopy/generators/model/pymprog_model_generator.py
 feloopy/generators/model/pyomo_model_generator.py
 feloopy/generators/model/xpress_model_generator.py
 feloopy/generators/result/__init__.py
+feloopy/generators/result/cplex_cp_result_generator.py
 feloopy/generators/result/cplex_result_generator.py
 feloopy/generators/result/cvxpy_result_generator.py
 feloopy/generators/result/cylp_result_generator.py
 feloopy/generators/result/gekko_result_generator.py
 feloopy/generators/result/gurobi_result_generator.py
 feloopy/generators/result/linopy_result_generator.py
 feloopy/generators/result/mip_result_generator.py
+feloopy/generators/result/ortools_cp_result_generator.py
 feloopy/generators/result/ortools_result_generator.py
 feloopy/generators/result/picos_result_generator.py
 feloopy/generators/result/pulp_result_generator.py
 feloopy/generators/result/pymprog_result_generator.py
 feloopy/generators/result/pyomo_result_generator.py
 feloopy/generators/result/xpress_result_generator.py
 feloopy/generators/solution/__init__.py
+feloopy/generators/solution/cplex_cp_solution_generator.py
 feloopy/generators/solution/cplex_solution_generator.py
 feloopy/generators/solution/cvxpy_solution_generator.py
 feloopy/generators/solution/cylp_solution_generator.py
 feloopy/generators/solution/feloopy_solution_generator.py
 feloopy/generators/solution/gekko_solution_generator.py
 feloopy/generators/solution/gurobi_solution_generator.py
 feloopy/generators/solution/linopy_solution_generator.py
 feloopy/generators/solution/mealpy_solution_generator.py
 feloopy/generators/solution/mip_solution_generator.py
+feloopy/generators/solution/ortools_cp_solution_generator.py
 feloopy/generators/solution/ortools_solution_generator.py
 feloopy/generators/solution/picos_solution_generator.py
 feloopy/generators/solution/pulp_solution_generator.py
 feloopy/generators/solution/pymprog_solution_generator.py
 feloopy/generators/solution/pyomo_solution_generator.py
 feloopy/generators/solution/xpress_solution_generator.py
 feloopy/generators/variable/__init__.py
+feloopy/generators/variable/cplex_cp_variable_generator.py
 feloopy/generators/variable/cplex_variable_generator.py
 feloopy/generators/variable/cvxpy_variable_generator.py
 feloopy/generators/variable/cylp_variable_generator.py
 feloopy/generators/variable/gekko_variable_generator.py
 feloopy/generators/variable/gurobi_variable_generator.py
 feloopy/generators/variable/linopy_variable_generator.py
 feloopy/generators/variable/mip_variable_generator.py
+feloopy/generators/variable/ortools_cp_variable_generator.py
 feloopy/generators/variable/ortools_variable_generator.py
 feloopy/generators/variable/picos_variable_generator.py
 feloopy/generators/variable/pulp_variable_generator.py
 feloopy/generators/variable/pymprog_variable_generator.py
 feloopy/generators/variable/pyomo_variable_generator.py
 feloopy/generators/variable/xpress_variable_generator.py
 feloopy/operators/__init__.py
 feloopy/operators/common.py
 feloopy/operators/exact.py
-feloopy/operators/heuristic.py
+feloopy/operators/heuristic.py
+tests/test_exact_kp.py
+tests/test_exact_tsp.py
```

### Comparing `feloopy-0.2.3/setup.py` & `feloopy-0.2.31/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
 
     name='feloopy',
 
-    version='0.2.3',
+    version='0.2.31',
 
-    description='FelooPy: An Integrated Optimization Environment (IOE) for AutoOR in Python.',
+    description='FelooPy: An Integrated Optimization Environment (IOE) for Automated operations research (AutoOR) in Python.',
 
     long_description=open('README.md', encoding="utf8").read(),
 
     long_description_content_type='text/markdown',
 
     keywords=['Optimization', 'Machine_Learning', 'Simulation', 'Operations_Research', 'Computer_Science', 'Data_Science'],
```

