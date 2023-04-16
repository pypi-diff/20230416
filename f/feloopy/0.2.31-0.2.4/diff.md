# Comparing `tmp/feloopy-0.2.31.tar.gz` & `tmp/feloopy-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feloopy-0.2.31.tar", last modified: Sun Apr 16 17:52:08 2023, max compression
+gzip compressed data, was "feloopy-0.2.4.tar", last modified: Sun Apr 16 18:25:12 2023, max compression
```

## Comparing `feloopy-0.2.31.tar` & `feloopy-0.2.4.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 17:52:08.178434 feloopy-0.2.31/
--rw-rw-rw-   0        0        0     1092 2023-03-25 08:57:31.000000 feloopy-0.2.31/LICENSE
--rw-rw-rw-   0        0        0    12387 2023-04-16 17:52:08.175427 feloopy-0.2.31/PKG-INFO
--rw-rw-rw-   0        0        0    11761 2023-04-16 17:51:27.000000 feloopy-0.2.31/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 17:52:07.949848 feloopy-0.2.31/feloopy/
--rw-rw-rw-   0        0        0     9884 2023-04-16 13:41:04.000000 feloopy-0.2.31/feloopy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 17:52:07.962867 feloopy-0.2.31/feloopy/algorithms/
--rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/algorithms/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 17:52:07.963868 feloopy-0.2.31/feloopy/algorithms/constraint/
--rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/algorithms/constraint/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 17:52:07.964866 feloopy-0.2.31/feloopy/algorithms/exact/
--rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/algorithms/exact/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 17:52:07.982382 feloopy-0.2.31/feloopy/algorithms/heuristic/
--rw-rw-rw-   0        0        0     2812 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/algorithms/heuristic/DE.py
--rw-rw-rw-   0        0        0     3096 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/algorithms/heuristic/GA.py
--rw-rw-rw-   0        0        0     2347 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/algorithms/heuristic/GWO.py
--rw-rw-rw-   0        0        0     3658 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/algorithms/heuristic/SA.py
--rw-rw-rw-   0        0        0     1794 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/algorithms/heuristic/TS.py
--rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/algorithms/heuristic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 17:52:07.984379 feloopy-0.2.31/feloopy/classes/
--rw-rw-rw-   0        0        0        0 2023-04-11 13:35:08.000000 feloopy-0.2.31/feloopy/classes/__init__.py
--rw-rw-rw-   0        0        0     1295 2023-04-11 13:36:26.000000 feloopy-0.2.31/feloopy/classes/empty.py
--rw-rw-rw-   0        0        0    77481 2023-04-16 17:32:59.000000 feloopy-0.2.31/feloopy/feloopy.py
-drwxrwxrwx   0        0        0        0 2023-04-16 17:52:08.002376 feloopy-0.2.31/feloopy/functions/
--rw-rw-rw-   0        0        0        0 2023-04-11 13:45:00.000000 feloopy-0.2.31/feloopy/functions/__init__.py
--rw-rw-rw-   0        0        0      488 2023-04-16 13:41:27.000000 feloopy-0.2.31/feloopy/functions/count_operators.py
--rw-rw-rw-   0        0        0      211 2023-04-16 14:10:14.000000 feloopy-0.2.31/feloopy/functions/fix_operators.py
--rw-rw-rw-   0        0        0     3029 2023-04-11 13:51:06.000000 feloopy-0.2.31/feloopy/functions/heuristic_operators.py
--rw-rw-rw-   0        0        0       38 2023-04-11 13:49:57.000000 feloopy-0.2.31/feloopy/functions/math_operators.py
--rw-rw-rw-   0        0        0      185 2023-04-11 13:50:07.000000 feloopy-0.2.31/feloopy/functions/random_operators.py
--rw-rw-rw-   0        0        0      305 2023-04-11 13:50:17.000000 feloopy-0.2.31/feloopy/functions/set_operators.py
--rw-rw-rw-   0        0        0     1669 2023-04-11 13:50:36.000000 feloopy-0.2.31/feloopy/functions/update_operators.py
-drwxrwxrwx   0        0        0        0 2023-04-16 17:52:08.015374 feloopy-0.2.31/feloopy/generators/
--rw-rw-rw-   0        0        0      129 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/generators/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 17:52:08.049368 feloopy-0.2.31/feloopy/generators/model/
--rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/generators/model/__init__.py
--rw-rw-rw-   0        0        0      156 2023-04-11 11:47:49.000000 feloopy-0.2.31/feloopy/generators/model/cplex_cp_model_generator.py
--rw-rw-rw-   0        0        0      153 2023-04-11 11:48:02.000000 feloopy-0.2.31/feloopy/generators/model/cplex_model_generator.py
--rw-rw-rw-   0        0        0      136 2023-04-16 12:06:27.000000 feloopy-0.2.31/feloopy/generators/model/cvxpy_model_generator.py
--rw-rw-rw-   0        0        0      155 2023-04-11 11:48:21.000000 feloopy-0.2.31/feloopy/generators/model/cylp_model_generator.py
--rw-rw-rw-   0        0        0     1572 2023-04-05 08:38:53.000000 feloopy-0.2.31/feloopy/generators/model/feloopy_model_generator.py
--rw-rw-rw-   0        0        0      146 2023-04-11 11:49:14.000000 feloopy-0.2.31/feloopy/generators/model/gekko_model_generator.py
--rw-rw-rw-   0        0        0      133 2023-04-11 11:49:40.000000 feloopy-0.2.31/feloopy/generators/model/gurobi_model_generator.py
--rw-rw-rw-   0        0        0      104 2023-04-11 11:49:51.000000 feloopy-0.2.31/feloopy/generators/model/linopy_model_generator.py
--rw-rw-rw-   0        0        0    26710 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/generators/model/mealpy_model_generator.py
--rw-rw-rw-   0        0        0      140 2023-04-11 11:50:27.000000 feloopy-0.2.31/feloopy/generators/model/mip_model_generator.py
--rw-rw-rw-   0        0        0      139 2023-04-11 11:50:43.000000 feloopy-0.2.31/feloopy/generators/model/ortools_cp_model_generator.py
--rw-rw-rw-   0        0        0      156 2023-04-11 11:51:10.000000 feloopy-0.2.31/feloopy/generators/model/ortools_model_generator.py
--rw-rw-rw-   0        0        0      135 2023-04-11 11:51:26.000000 feloopy-0.2.31/feloopy/generators/model/picos_model_generator.py
--rw-rw-rw-   0        0        0      156 2023-04-11 11:51:37.000000 feloopy-0.2.31/feloopy/generators/model/pulp_model_generator.py
--rw-rw-rw-   0        0        0      127 2023-04-11 11:51:46.000000 feloopy-0.2.31/feloopy/generators/model/pymprog_model_generator.py
--rw-rw-rw-   0        0        0      149 2023-04-11 11:52:04.000000 feloopy-0.2.31/feloopy/generators/model/pyomo_model_generator.py
--rw-rw-rw-   0        0        0      133 2023-04-11 11:52:21.000000 feloopy-0.2.31/feloopy/generators/model/xpress_model_generator.py
--rw-rw-rw-   0        0        0     2474 2023-04-11 11:47:11.000000 feloopy-0.2.31/feloopy/generators/model_generator.py
-drwxrwxrwx   0        0        0        0 2023-04-16 17:52:08.077881 feloopy-0.2.31/feloopy/generators/result/
--rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/generators/result/__init__.py
--rw-rw-rw-   0        0        0      385 2023-04-11 17:07:27.000000 feloopy-0.2.31/feloopy/generators/result/cplex_cp_result_generator.py
--rw-rw-rw-   0        0        0      453 2023-04-11 17:07:23.000000 feloopy-0.2.31/feloopy/generators/result/cplex_result_generator.py
--rw-rw-rw-   0        0        0      452 2023-04-16 12:04:52.000000 feloopy-0.2.31/feloopy/generators/result/cvxpy_result_generator.py
--rw-rw-rw-   0        0        0      504 2023-04-05 08:40:40.000000 feloopy-0.2.31/feloopy/generators/result/cylp_result_generator.py
--rw-rw-rw-   0        0        0      576 2023-04-05 08:40:56.000000 feloopy-0.2.31/feloopy/generators/result/gekko_result_generator.py
--rw-rw-rw-   0        0        0     1183 2023-04-05 08:41:25.000000 feloopy-0.2.31/feloopy/generators/result/gurobi_result_generator.py
--rw-rw-rw-   0        0        0      452 2023-04-05 08:41:37.000000 feloopy-0.2.31/feloopy/generators/result/linopy_result_generator.py
--rw-rw-rw-   0        0        0      391 2023-04-05 08:41:43.000000 feloopy-0.2.31/feloopy/generators/result/mip_result_generator.py
--rw-rw-rw-   0        0        0      548 2023-04-05 08:41:48.000000 feloopy-0.2.31/feloopy/generators/result/ortools_cp_result_generator.py
--rw-rw-rw-   0        0        0      622 2023-04-05 08:41:53.000000 feloopy-0.2.31/feloopy/generators/result/ortools_result_generator.py
--rw-rw-rw-   0        0        0      414 2023-04-05 08:41:58.000000 feloopy-0.2.31/feloopy/generators/result/picos_result_generator.py
--rw-rw-rw-   0        0        0      507 2023-04-05 08:42:04.000000 feloopy-0.2.31/feloopy/generators/result/pulp_result_generator.py
--rw-rw-rw-   0        0        0      500 2023-04-05 08:42:10.000000 feloopy-0.2.31/feloopy/generators/result/pymprog_result_generator.py
--rw-rw-rw-   0        0        0      469 2023-04-05 08:42:16.000000 feloopy-0.2.31/feloopy/generators/result/pyomo_result_generator.py
--rw-rw-rw-   0        0        0      417 2023-04-05 08:42:22.000000 feloopy-0.2.31/feloopy/generators/result/xpress_result_generator.py
--rw-rw-rw-   0        0        0     6254 2023-04-04 11:50:22.000000 feloopy-0.2.31/feloopy/generators/result_generator.py
-drwxrwxrwx   0        0        0        0 2023-04-16 17:52:08.118874 feloopy-0.2.31/feloopy/generators/solution/
--rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/generators/solution/__init__.py
--rw-rw-rw-   0        0        0     2446 2023-04-11 11:29:12.000000 feloopy-0.2.31/feloopy/generators/solution/cplex_cp_solution_generator.py
--rw-rw-rw-   0        0        0     3968 2023-04-11 11:29:46.000000 feloopy-0.2.31/feloopy/generators/solution/cplex_solution_generator.py
--rw-rw-rw-   0        0        0     2929 2023-04-16 12:52:44.000000 feloopy-0.2.31/feloopy/generators/solution/cvxpy_solution_generator.py
--rw-rw-rw-   0        0        0     1998 2023-04-11 11:30:29.000000 feloopy-0.2.31/feloopy/generators/solution/cylp_solution_generator.py
--rw-rw-rw-   0        0        0     2947 2023-03-31 08:00:48.000000 feloopy-0.2.31/feloopy/generators/solution/feloopy_solution_generator.py
--rw-rw-rw-   0        0        0     2740 2023-04-16 13:02:36.000000 feloopy-0.2.31/feloopy/generators/solution/gekko_solution_generator.py
--rw-rw-rw-   0        0        0     2728 2023-04-11 11:31:20.000000 feloopy-0.2.31/feloopy/generators/solution/gurobi_solution_generator.py
--rw-rw-rw-   0        0        0     2136 2023-04-11 11:31:33.000000 feloopy-0.2.31/feloopy/generators/solution/linopy_solution_generator.py
--rw-rw-rw-   0        0        0     4315 2023-04-11 11:31:52.000000 feloopy-0.2.31/feloopy/generators/solution/mealpy_solution_generator.py
--rw-rw-rw-   0        0        0     1901 2023-04-11 11:32:13.000000 feloopy-0.2.31/feloopy/generators/solution/mip_solution_generator.py
--rw-rw-rw-   0        0        0     2758 2023-04-11 11:32:29.000000 feloopy-0.2.31/feloopy/generators/solution/ortools_cp_solution_generator.py
--rw-rw-rw-   0        0        0     3091 2023-04-11 11:32:41.000000 feloopy-0.2.31/feloopy/generators/solution/ortools_solution_generator.py
--rw-rw-rw-   0        0        0     2278 2023-04-11 11:32:52.000000 feloopy-0.2.31/feloopy/generators/solution/picos_solution_generator.py
--rw-rw-rw-   0        0        0     3322 2023-04-11 11:33:06.000000 feloopy-0.2.31/feloopy/generators/solution/pulp_solution_generator.py
--rw-rw-rw-   0        0        0     2054 2023-04-12 06:39:22.000000 feloopy-0.2.31/feloopy/generators/solution/pymprog_solution_generator.py
--rw-rw-rw-   0        0        0     5576 2023-04-12 06:19:57.000000 feloopy-0.2.31/feloopy/generators/solution/pyomo_solution_generator.py
--rw-rw-rw-   0        0        0     1935 2023-04-11 15:44:52.000000 feloopy-0.2.31/feloopy/generators/solution/xpress_solution_generator.py
--rw-rw-rw-   0        0        0     2674 2023-04-11 11:23:04.000000 feloopy-0.2.31/feloopy/generators/solution_generator.py
-drwxrwxrwx   0        0        0        0 2023-04-16 17:52:08.160907 feloopy-0.2.31/feloopy/generators/variable/
--rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/generators/variable/__init__.py
--rw-rw-rw-   0        0        0     2677 2023-04-04 08:02:30.000000 feloopy-0.2.31/feloopy/generators/variable/cplex_cp_variable_generator.py
--rw-rw-rw-   0        0        0     2967 2023-04-11 15:32:22.000000 feloopy-0.2.31/feloopy/generators/variable/cplex_variable_generator.py
--rw-rw-rw-   0        0        0     6460 2023-04-16 12:18:37.000000 feloopy-0.2.31/feloopy/generators/variable/cvxpy_variable_generator.py
--rw-rw-rw-   0        0        0     2783 2023-03-31 08:38:56.000000 feloopy-0.2.31/feloopy/generators/variable/cylp_variable_generator.py
--rw-rw-rw-   0        0        0     2621 2023-03-31 08:39:01.000000 feloopy-0.2.31/feloopy/generators/variable/gekko_variable_generator.py
--rw-rw-rw-   0        0        0     7599 2023-04-16 11:18:49.000000 feloopy-0.2.31/feloopy/generators/variable/gurobi_variable_generator.py
--rw-rw-rw-   0        0        0     2123 2023-03-31 08:39:06.000000 feloopy-0.2.31/feloopy/generators/variable/linopy_variable_generator.py
--rw-rw-rw-   0        0        0     2657 2023-03-31 09:21:12.000000 feloopy-0.2.31/feloopy/generators/variable/mip_variable_generator.py
--rw-rw-rw-   0        0        0     3756 2023-04-04 13:36:46.000000 feloopy-0.2.31/feloopy/generators/variable/ortools_cp_variable_generator.py
--rw-rw-rw-   0        0        0     3997 2023-03-31 08:36:53.000000 feloopy-0.2.31/feloopy/generators/variable/ortools_variable_generator.py
--rw-rw-rw-   0        0        0     2888 2023-03-31 08:39:12.000000 feloopy-0.2.31/feloopy/generators/variable/picos_variable_generator.py
--rw-rw-rw-   0        0        0     3544 2023-03-31 08:39:15.000000 feloopy-0.2.31/feloopy/generators/variable/pulp_variable_generator.py
--rw-rw-rw-   0        0        0     3048 2023-03-31 08:39:17.000000 feloopy-0.2.31/feloopy/generators/variable/pymprog_variable_generator.py
--rw-rw-rw-   0        0        0     2326 2023-03-31 08:39:19.000000 feloopy-0.2.31/feloopy/generators/variable/pyomo_variable_generator.py
--rw-rw-rw-   0        0        0     4552 2023-03-31 08:39:21.000000 feloopy-0.2.31/feloopy/generators/variable/xpress_variable_generator.py
--rw-rw-rw-   0        0        0     2814 2023-04-04 07:53:39.000000 feloopy-0.2.31/feloopy/generators/variable_generator.py
-drwxrwxrwx   0        0        0        0 2023-04-16 17:52:08.167907 feloopy-0.2.31/feloopy/operators/
--rw-rw-rw-   0        0        0       69 2023-03-25 08:57:31.000000 feloopy-0.2.31/feloopy/operators/__init__.py
--rw-rw-rw-   0        0        0     9094 2023-04-11 17:03:29.000000 feloopy-0.2.31/feloopy/operators/common.py
--rw-rw-rw-   0        0        0       89 2023-04-05 08:20:05.000000 feloopy-0.2.31/feloopy/operators/exact.py
--rw-rw-rw-   0        0        0      187 2023-04-05 08:19:38.000000 feloopy-0.2.31/feloopy/operators/heuristic.py
-drwxrwxrwx   0        0        0        0 2023-04-16 17:52:07.960868 feloopy-0.2.31/feloopy.egg-info/
--rw-rw-rw-   0        0        0    12387 2023-04-16 17:52:07.000000 feloopy-0.2.31/feloopy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4869 2023-04-16 17:52:07.000000 feloopy-0.2.31/feloopy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 17:52:07.000000 feloopy-0.2.31/feloopy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      146 2023-04-16 17:52:07.000000 feloopy-0.2.31/feloopy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-16 17:52:07.000000 feloopy-0.2.31/feloopy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 17:52:08.178434 feloopy-0.2.31/setup.cfg
--rw-rw-rw-   0        0        0     1368 2023-04-16 17:43:13.000000 feloopy-0.2.31/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 17:52:08.170416 feloopy-0.2.31/tests/
--rw-rw-rw-   0        0        0     1029 2023-04-16 17:34:01.000000 feloopy-0.2.31/tests/test_exact_kp.py
--rw-rw-rw-   0        0        0     1277 2023-04-12 07:11:14.000000 feloopy-0.2.31/tests/test_exact_tsp.py
+drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.945277 feloopy-0.2.4/
+-rw-rw-rw-   0        0        0     1092 2023-03-25 08:57:31.000000 feloopy-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0    12389 2023-04-16 18:25:11.944282 feloopy-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11764 2023-04-16 18:24:34.000000 feloopy-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.713287 feloopy-0.2.4/feloopy/
+-rw-rw-rw-   0        0        0     9884 2023-04-16 13:41:04.000000 feloopy-0.2.4/feloopy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.727268 feloopy-0.2.4/feloopy/algorithms/
+-rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/algorithms/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.728264 feloopy-0.2.4/feloopy/algorithms/constraint/
+-rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/algorithms/constraint/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.731265 feloopy-0.2.4/feloopy/algorithms/exact/
+-rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/algorithms/exact/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.742262 feloopy-0.2.4/feloopy/algorithms/heuristic/
+-rw-rw-rw-   0        0        0     2812 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/algorithms/heuristic/DE.py
+-rw-rw-rw-   0        0        0     3096 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/algorithms/heuristic/GA.py
+-rw-rw-rw-   0        0        0     2347 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/algorithms/heuristic/GWO.py
+-rw-rw-rw-   0        0        0     3658 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/algorithms/heuristic/SA.py
+-rw-rw-rw-   0        0        0     1794 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/algorithms/heuristic/TS.py
+-rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/algorithms/heuristic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.745262 feloopy-0.2.4/feloopy/classes/
+-rw-rw-rw-   0        0        0        0 2023-04-11 13:35:08.000000 feloopy-0.2.4/feloopy/classes/__init__.py
+-rw-rw-rw-   0        0        0     1295 2023-04-11 13:36:26.000000 feloopy-0.2.4/feloopy/classes/empty.py
+-rw-rw-rw-   0        0        0    77008 2023-04-16 18:12:48.000000 feloopy-0.2.4/feloopy/feloopy.py
+drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.760262 feloopy-0.2.4/feloopy/functions/
+-rw-rw-rw-   0        0        0        0 2023-04-11 13:45:00.000000 feloopy-0.2.4/feloopy/functions/__init__.py
+-rw-rw-rw-   0        0        0      488 2023-04-16 13:41:27.000000 feloopy-0.2.4/feloopy/functions/count_operators.py
+-rw-rw-rw-   0        0        0      229 2023-04-16 18:06:45.000000 feloopy-0.2.4/feloopy/functions/fix_operators.py
+-rw-rw-rw-   0        0        0     3029 2023-04-11 13:51:06.000000 feloopy-0.2.4/feloopy/functions/heuristic_operators.py
+-rw-rw-rw-   0        0        0       38 2023-04-11 13:49:57.000000 feloopy-0.2.4/feloopy/functions/math_operators.py
+-rw-rw-rw-   0        0        0      185 2023-04-11 13:50:07.000000 feloopy-0.2.4/feloopy/functions/random_operators.py
+-rw-rw-rw-   0        0        0      305 2023-04-11 13:50:17.000000 feloopy-0.2.4/feloopy/functions/set_operators.py
+-rw-rw-rw-   0        0        0     1669 2023-04-11 13:50:36.000000 feloopy-0.2.4/feloopy/functions/update_operators.py
+drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.771258 feloopy-0.2.4/feloopy/generators/
+-rw-rw-rw-   0        0        0      129 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/generators/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.814776 feloopy-0.2.4/feloopy/generators/model/
+-rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/generators/model/__init__.py
+-rw-rw-rw-   0        0        0      156 2023-04-11 11:47:49.000000 feloopy-0.2.4/feloopy/generators/model/cplex_cp_model_generator.py
+-rw-rw-rw-   0        0        0      153 2023-04-11 11:48:02.000000 feloopy-0.2.4/feloopy/generators/model/cplex_model_generator.py
+-rw-rw-rw-   0        0        0      136 2023-04-16 12:06:27.000000 feloopy-0.2.4/feloopy/generators/model/cvxpy_model_generator.py
+-rw-rw-rw-   0        0        0      155 2023-04-11 11:48:21.000000 feloopy-0.2.4/feloopy/generators/model/cylp_model_generator.py
+-rw-rw-rw-   0        0        0     1572 2023-04-05 08:38:53.000000 feloopy-0.2.4/feloopy/generators/model/feloopy_model_generator.py
+-rw-rw-rw-   0        0        0      146 2023-04-11 11:49:14.000000 feloopy-0.2.4/feloopy/generators/model/gekko_model_generator.py
+-rw-rw-rw-   0        0        0      133 2023-04-11 11:49:40.000000 feloopy-0.2.4/feloopy/generators/model/gurobi_model_generator.py
+-rw-rw-rw-   0        0        0      104 2023-04-11 11:49:51.000000 feloopy-0.2.4/feloopy/generators/model/linopy_model_generator.py
+-rw-rw-rw-   0        0        0    26710 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/generators/model/mealpy_model_generator.py
+-rw-rw-rw-   0        0        0      140 2023-04-11 11:50:27.000000 feloopy-0.2.4/feloopy/generators/model/mip_model_generator.py
+-rw-rw-rw-   0        0        0      139 2023-04-11 11:50:43.000000 feloopy-0.2.4/feloopy/generators/model/ortools_cp_model_generator.py
+-rw-rw-rw-   0        0        0      156 2023-04-11 11:51:10.000000 feloopy-0.2.4/feloopy/generators/model/ortools_model_generator.py
+-rw-rw-rw-   0        0        0      135 2023-04-11 11:51:26.000000 feloopy-0.2.4/feloopy/generators/model/picos_model_generator.py
+-rw-rw-rw-   0        0        0      156 2023-04-11 11:51:37.000000 feloopy-0.2.4/feloopy/generators/model/pulp_model_generator.py
+-rw-rw-rw-   0        0        0      127 2023-04-11 11:51:46.000000 feloopy-0.2.4/feloopy/generators/model/pymprog_model_generator.py
+-rw-rw-rw-   0        0        0      149 2023-04-11 11:52:04.000000 feloopy-0.2.4/feloopy/generators/model/pyomo_model_generator.py
+-rw-rw-rw-   0        0        0      133 2023-04-11 11:52:21.000000 feloopy-0.2.4/feloopy/generators/model/xpress_model_generator.py
+-rw-rw-rw-   0        0        0     2474 2023-04-11 11:47:11.000000 feloopy-0.2.4/feloopy/generators/model_generator.py
+drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.848770 feloopy-0.2.4/feloopy/generators/result/
+-rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/generators/result/__init__.py
+-rw-rw-rw-   0        0        0      385 2023-04-11 17:07:27.000000 feloopy-0.2.4/feloopy/generators/result/cplex_cp_result_generator.py
+-rw-rw-rw-   0        0        0      453 2023-04-11 17:07:23.000000 feloopy-0.2.4/feloopy/generators/result/cplex_result_generator.py
+-rw-rw-rw-   0        0        0      452 2023-04-16 12:04:52.000000 feloopy-0.2.4/feloopy/generators/result/cvxpy_result_generator.py
+-rw-rw-rw-   0        0        0      504 2023-04-05 08:40:40.000000 feloopy-0.2.4/feloopy/generators/result/cylp_result_generator.py
+-rw-rw-rw-   0        0        0      576 2023-04-05 08:40:56.000000 feloopy-0.2.4/feloopy/generators/result/gekko_result_generator.py
+-rw-rw-rw-   0        0        0     1183 2023-04-05 08:41:25.000000 feloopy-0.2.4/feloopy/generators/result/gurobi_result_generator.py
+-rw-rw-rw-   0        0        0      452 2023-04-05 08:41:37.000000 feloopy-0.2.4/feloopy/generators/result/linopy_result_generator.py
+-rw-rw-rw-   0        0        0      391 2023-04-05 08:41:43.000000 feloopy-0.2.4/feloopy/generators/result/mip_result_generator.py
+-rw-rw-rw-   0        0        0      548 2023-04-05 08:41:48.000000 feloopy-0.2.4/feloopy/generators/result/ortools_cp_result_generator.py
+-rw-rw-rw-   0        0        0      622 2023-04-05 08:41:53.000000 feloopy-0.2.4/feloopy/generators/result/ortools_result_generator.py
+-rw-rw-rw-   0        0        0      414 2023-04-05 08:41:58.000000 feloopy-0.2.4/feloopy/generators/result/picos_result_generator.py
+-rw-rw-rw-   0        0        0      507 2023-04-05 08:42:04.000000 feloopy-0.2.4/feloopy/generators/result/pulp_result_generator.py
+-rw-rw-rw-   0        0        0      500 2023-04-05 08:42:10.000000 feloopy-0.2.4/feloopy/generators/result/pymprog_result_generator.py
+-rw-rw-rw-   0        0        0      469 2023-04-05 08:42:16.000000 feloopy-0.2.4/feloopy/generators/result/pyomo_result_generator.py
+-rw-rw-rw-   0        0        0      417 2023-04-05 08:42:22.000000 feloopy-0.2.4/feloopy/generators/result/xpress_result_generator.py
+-rw-rw-rw-   0        0        0     6254 2023-04-04 11:50:22.000000 feloopy-0.2.4/feloopy/generators/result_generator.py
+drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.876770 feloopy-0.2.4/feloopy/generators/solution/
+-rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/generators/solution/__init__.py
+-rw-rw-rw-   0        0        0     2446 2023-04-11 11:29:12.000000 feloopy-0.2.4/feloopy/generators/solution/cplex_cp_solution_generator.py
+-rw-rw-rw-   0        0        0     3968 2023-04-11 11:29:46.000000 feloopy-0.2.4/feloopy/generators/solution/cplex_solution_generator.py
+-rw-rw-rw-   0        0        0     2929 2023-04-16 12:52:44.000000 feloopy-0.2.4/feloopy/generators/solution/cvxpy_solution_generator.py
+-rw-rw-rw-   0        0        0     1998 2023-04-11 11:30:29.000000 feloopy-0.2.4/feloopy/generators/solution/cylp_solution_generator.py
+-rw-rw-rw-   0        0        0     2947 2023-03-31 08:00:48.000000 feloopy-0.2.4/feloopy/generators/solution/feloopy_solution_generator.py
+-rw-rw-rw-   0        0        0     2740 2023-04-16 13:02:36.000000 feloopy-0.2.4/feloopy/generators/solution/gekko_solution_generator.py
+-rw-rw-rw-   0        0        0     2728 2023-04-11 11:31:20.000000 feloopy-0.2.4/feloopy/generators/solution/gurobi_solution_generator.py
+-rw-rw-rw-   0        0        0     2136 2023-04-11 11:31:33.000000 feloopy-0.2.4/feloopy/generators/solution/linopy_solution_generator.py
+-rw-rw-rw-   0        0        0     4315 2023-04-11 11:31:52.000000 feloopy-0.2.4/feloopy/generators/solution/mealpy_solution_generator.py
+-rw-rw-rw-   0        0        0     1901 2023-04-11 11:32:13.000000 feloopy-0.2.4/feloopy/generators/solution/mip_solution_generator.py
+-rw-rw-rw-   0        0        0     2758 2023-04-11 11:32:29.000000 feloopy-0.2.4/feloopy/generators/solution/ortools_cp_solution_generator.py
+-rw-rw-rw-   0        0        0     3091 2023-04-11 11:32:41.000000 feloopy-0.2.4/feloopy/generators/solution/ortools_solution_generator.py
+-rw-rw-rw-   0        0        0     2278 2023-04-11 11:32:52.000000 feloopy-0.2.4/feloopy/generators/solution/picos_solution_generator.py
+-rw-rw-rw-   0        0        0     3322 2023-04-11 11:33:06.000000 feloopy-0.2.4/feloopy/generators/solution/pulp_solution_generator.py
+-rw-rw-rw-   0        0        0     2054 2023-04-12 06:39:22.000000 feloopy-0.2.4/feloopy/generators/solution/pymprog_solution_generator.py
+-rw-rw-rw-   0        0        0     5576 2023-04-12 06:19:57.000000 feloopy-0.2.4/feloopy/generators/solution/pyomo_solution_generator.py
+-rw-rw-rw-   0        0        0     1935 2023-04-11 15:44:52.000000 feloopy-0.2.4/feloopy/generators/solution/xpress_solution_generator.py
+-rw-rw-rw-   0        0        0     2674 2023-04-11 11:23:04.000000 feloopy-0.2.4/feloopy/generators/solution_generator.py
+drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.927279 feloopy-0.2.4/feloopy/generators/variable/
+-rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/generators/variable/__init__.py
+-rw-rw-rw-   0        0        0     2677 2023-04-04 08:02:30.000000 feloopy-0.2.4/feloopy/generators/variable/cplex_cp_variable_generator.py
+-rw-rw-rw-   0        0        0     2967 2023-04-11 15:32:22.000000 feloopy-0.2.4/feloopy/generators/variable/cplex_variable_generator.py
+-rw-rw-rw-   0        0        0     6460 2023-04-16 12:18:37.000000 feloopy-0.2.4/feloopy/generators/variable/cvxpy_variable_generator.py
+-rw-rw-rw-   0        0        0     2783 2023-03-31 08:38:56.000000 feloopy-0.2.4/feloopy/generators/variable/cylp_variable_generator.py
+-rw-rw-rw-   0        0        0     2621 2023-03-31 08:39:01.000000 feloopy-0.2.4/feloopy/generators/variable/gekko_variable_generator.py
+-rw-rw-rw-   0        0        0     7602 2023-04-16 18:11:55.000000 feloopy-0.2.4/feloopy/generators/variable/gurobi_variable_generator.py
+-rw-rw-rw-   0        0        0     2123 2023-03-31 08:39:06.000000 feloopy-0.2.4/feloopy/generators/variable/linopy_variable_generator.py
+-rw-rw-rw-   0        0        0     2657 2023-03-31 09:21:12.000000 feloopy-0.2.4/feloopy/generators/variable/mip_variable_generator.py
+-rw-rw-rw-   0        0        0     3756 2023-04-04 13:36:46.000000 feloopy-0.2.4/feloopy/generators/variable/ortools_cp_variable_generator.py
+-rw-rw-rw-   0        0        0     3997 2023-03-31 08:36:53.000000 feloopy-0.2.4/feloopy/generators/variable/ortools_variable_generator.py
+-rw-rw-rw-   0        0        0     2888 2023-03-31 08:39:12.000000 feloopy-0.2.4/feloopy/generators/variable/picos_variable_generator.py
+-rw-rw-rw-   0        0        0     3544 2023-03-31 08:39:15.000000 feloopy-0.2.4/feloopy/generators/variable/pulp_variable_generator.py
+-rw-rw-rw-   0        0        0     3048 2023-03-31 08:39:17.000000 feloopy-0.2.4/feloopy/generators/variable/pymprog_variable_generator.py
+-rw-rw-rw-   0        0        0     2326 2023-03-31 08:39:19.000000 feloopy-0.2.4/feloopy/generators/variable/pyomo_variable_generator.py
+-rw-rw-rw-   0        0        0     4552 2023-03-31 08:39:21.000000 feloopy-0.2.4/feloopy/generators/variable/xpress_variable_generator.py
+-rw-rw-rw-   0        0        0     2814 2023-04-04 07:53:39.000000 feloopy-0.2.4/feloopy/generators/variable_generator.py
+drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.936279 feloopy-0.2.4/feloopy/operators/
+-rw-rw-rw-   0        0        0       69 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/operators/__init__.py
+-rw-rw-rw-   0        0        0     9094 2023-04-11 17:03:29.000000 feloopy-0.2.4/feloopy/operators/common.py
+-rw-rw-rw-   0        0        0       89 2023-04-05 08:20:05.000000 feloopy-0.2.4/feloopy/operators/exact.py
+-rw-rw-rw-   0        0        0      187 2023-04-05 08:19:38.000000 feloopy-0.2.4/feloopy/operators/heuristic.py
+drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.726265 feloopy-0.2.4/feloopy.egg-info/
+-rw-rw-rw-   0        0        0    12389 2023-04-16 18:25:11.000000 feloopy-0.2.4/feloopy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4869 2023-04-16 18:25:11.000000 feloopy-0.2.4/feloopy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 18:25:11.000000 feloopy-0.2.4/feloopy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      146 2023-04-16 18:25:11.000000 feloopy-0.2.4/feloopy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-16 18:25:11.000000 feloopy-0.2.4/feloopy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 18:25:11.945277 feloopy-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2023-04-16 18:02:29.000000 feloopy-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.943277 feloopy-0.2.4/tests/
+-rw-rw-rw-   0        0        0     1029 2023-04-16 17:34:01.000000 feloopy-0.2.4/tests/test_exact_kp.py
+-rw-rw-rw-   0        0        0     1277 2023-04-12 07:11:14.000000 feloopy-0.2.4/tests/test_exact_tsp.py
```

### Comparing `feloopy-0.2.31/LICENSE` & `feloopy-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/PKG-INFO` & `feloopy-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feloopy
-Version: 0.2.31
+Version: 0.2.4
 Summary: FelooPy: An Integrated Optimization Environment (IOE) for Automated operations research (AutoOR) in Python.
 Home-page: https://github.com/ktafakkori/feloopy
 Download-URL: https://github.com/ktafakkori/feloopy/releases
 Author: Keivan Tafakkori
 Author-email: k.tafakkori@gmail.com
 Maintainer: Keivan Tafakkori
 Maintainer-email: k.tafakkori@gmail.com
@@ -59,17 +59,17 @@
 
 <div align="center">
 
 <div align="left">
 
 ## News
 
-🎉 _Version 0.2.3 is out: More stable than ever!_ 🎉
+🎉 _Version 0.2.4 is out: Added new functionalities!_ 🎉
 
-🎉 _The next version would focus on solve facilities_ 🎉
+🎉 _The next version would focus on more facilities_ 🎉
 
 💻 _Quick install_: `pip install --upgrade feloopy`
 
 #
 
 ## Introduction
 
@@ -154,23 +154,23 @@
 [vs]: https://code.visualstudio.com/
 [sp]: https://www.anaconda.com/
 [gc]: https://colab.research.google.com/
 
 ### Method 1: Terminal command (e.g., CMD or GC):
 
 ```text
-pip install feloopy==0.2.3
+pip install feloopy==0.2.4
 ```
 
 ### Method 2: IDE command (e.g., Spyder):
 
 _Note_: After installation, this line of code should be deleted.
 
 ```text
-!pip install feloopy==0.2.3
+!pip install feloopy==0.2.4
 ```
 
 ### Method 3: Inside your Python code
 
 _Note_: After installation, this piece of code should be deleted.
 
 ```text
@@ -183,15 +183,15 @@
         pip._internal.main(['install','-U', package])
 
 install('feloopy')
 ```
 
 ### Method 4: From GitHub [Releases][a] section
 
-1. Download the [feloopy-0.2.3.zip][c] file.
+1. Download the [feloopy-0.2.4.zip][c] file.
 2. Extract it into a specific directory.
 3. Open a terminal in that directory.
 4. Type: `pip install .`
 
 [a]: https://github.com/ktafakkori/feloopy/releases
 [b]: https://git-scm.com/downloads
 [c]: https://github.com/ktafakkori/feloopy/releases/download/0.2.3/feloopy-0.2.3.zip
@@ -249,27 +249,27 @@
 ## Citation
 
 It is recommended to cite this GitHub repository or the Python library if you use its facilities in your work:
 
 - APA 7:
 
 ```text
-Tafakkori, K. (2023). FelooPy: An integrated optimization environment for AutoOR in Python (0.2.3) [Python Library]. https://github.com/ktafakkori/feloopy (Original work published 2023)
+Tafakkori, K. (2023). FelooPy: An integrated optimization environment for AutoOR in Python (0.2.4) [Python Library]. https://github.com/ktafakkori/feloopy (Original work published 2023)
 ```
 
 - LaTeX:
 
 ```text
-@software{ktafakkori2023Feb,
+@software{ktafakkori2023Apr,
   author       = {Keivan Tafakkori},
   title        = {{FelooPy: An integrated optimization environment for AutoOR in Python}},
   year         = {2023},
-  month        = feb,
+  month        = apr,
   publisher    = {GitHub},
-  version      = {v0.2.3},
+  version      = {v0.2.4},
   url          = {https://github.com/ktafakkori/feloopy/}
 }
 ```
 
 ## License
 
 FelooPy is completely free and open-source and licensed under the [MIT][08] license.
```

### Comparing `feloopy-0.2.31/README.md` & `feloopy-0.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 
 <div align="center">
 
 <div align="left">
 
 ## News
 
-🎉 _Version 0.2.3 is out: More stable than ever!_ 🎉
+🎉 _Version 0.2.4 is out: Added new functionalities!_ 🎉
 
-🎉 _The next version would focus on solve facilities_ 🎉
+🎉 _The next version would focus on more facilities_ 🎉
 
 💻 _Quick install_: `pip install --upgrade feloopy`
 
 #
 
 ## Introduction
 
@@ -138,23 +138,23 @@
 [vs]: https://code.visualstudio.com/
 [sp]: https://www.anaconda.com/
 [gc]: https://colab.research.google.com/
 
 ### Method 1: Terminal command (e.g., CMD or GC):
 
 ```text
-pip install feloopy==0.2.3
+pip install feloopy==0.2.4
 ```
 
 ### Method 2: IDE command (e.g., Spyder):
 
 _Note_: After installation, this line of code should be deleted.
 
 ```text
-!pip install feloopy==0.2.3
+!pip install feloopy==0.2.4
 ```
 
 ### Method 3: Inside your Python code
 
 _Note_: After installation, this piece of code should be deleted.
 
 ```text
@@ -167,15 +167,15 @@
         pip._internal.main(['install','-U', package])
 
 install('feloopy')
 ```
 
 ### Method 4: From GitHub [Releases][a] section
 
-1. Download the [feloopy-0.2.3.zip][c] file.
+1. Download the [feloopy-0.2.4.zip][c] file.
 2. Extract it into a specific directory.
 3. Open a terminal in that directory.
 4. Type: `pip install .`
 
 [a]: https://github.com/ktafakkori/feloopy/releases
 [b]: https://git-scm.com/downloads
 [c]: https://github.com/ktafakkori/feloopy/releases/download/0.2.3/feloopy-0.2.3.zip
@@ -233,27 +233,27 @@
 ## Citation
 
 It is recommended to cite this GitHub repository or the Python library if you use its facilities in your work:
 
 - APA 7:
 
 ```text
-Tafakkori, K. (2023). FelooPy: An integrated optimization environment for AutoOR in Python (0.2.3) [Python Library]. https://github.com/ktafakkori/feloopy (Original work published 2023)
+Tafakkori, K. (2023). FelooPy: An integrated optimization environment for AutoOR in Python (0.2.4) [Python Library]. https://github.com/ktafakkori/feloopy (Original work published 2023)
 ```
 
 - LaTeX:
 
 ```text
-@software{ktafakkori2023Feb,
+@software{ktafakkori2023Apr,
   author       = {Keivan Tafakkori},
   title        = {{FelooPy: An integrated optimization environment for AutoOR in Python}},
   year         = {2023},
-  month        = feb,
+  month        = apr,
   publisher    = {GitHub},
-  version      = {v0.2.3},
+  version      = {v0.2.4},
   url          = {https://github.com/ktafakkori/feloopy/}
 }
 ```
 
 ## License
 
 FelooPy is completely free and open-source and licensed under the [MIT][08] license.
```

### Comparing `feloopy-0.2.31/feloopy/__init__.py` & `feloopy-0.2.4/feloopy/__init__.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/algorithms/heuristic/DE.py` & `feloopy-0.2.4/feloopy/algorithms/heuristic/DE.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/algorithms/heuristic/GA.py` & `feloopy-0.2.4/feloopy/algorithms/heuristic/GA.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/algorithms/heuristic/GWO.py` & `feloopy-0.2.4/feloopy/algorithms/heuristic/GWO.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/algorithms/heuristic/SA.py` & `feloopy-0.2.4/feloopy/algorithms/heuristic/SA.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/algorithms/heuristic/TS.py` & `feloopy-0.2.4/feloopy/algorithms/heuristic/TS.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/classes/empty.py` & `feloopy-0.2.4/feloopy/classes/empty.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/feloopy.py` & `feloopy-0.2.4/feloopy/feloopy.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,18 +226,14 @@
 
             case 'exact':
 
                 from .generators import variable_generator
 
                 return variable_generator.generate_variable(self.features['interface_name'], self.model, 'ptvar', name, variable_bound, variable_dim)
 
-            case 'heuristic':
-
-                return generate_heuristic_variable(self.features, 'ptvar', name, variable_dim, variable_bound, self.agent)
-
         return self.vars[name]
 
     def itvar(self, name, variable_dim=0, variable_bound=[0, None]):
 
         """
         Integer Tensor Variable Definition
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
@@ -262,17 +258,14 @@
 
             case 'exact':
 
                 from .generators import variable_generator
 
                 return variable_generator.generate_variable(self.features['interface_name'], self.model, 'itvar', name, variable_bound, variable_dim)
 
-            case 'heuristic':
-
-                return generate_heuristic_variable(self.features, 'itvar', name, variable_dim, variable_bound, self.agent)
 
         return self.vars[name]
 
     def ftvar(self, name, variable_dim=0, variable_bound=[None, None]):
 
         """
         Free Tensor Variable Definition
@@ -296,19 +289,15 @@
 
         match self.features['solution_method']:
 
             case 'exact':
 
                 from .generators import variable_generator
 
-                return variable_generator.generate_variable(self.features['interface_name'], self.model, 'tvar', name, variable_bound, variable_dim)
-
-            case 'heuristic':
-
-                return generate_heuristic_variable(self.features, 'tvar', name, variable_dim, variable_bound, self.agent)
+                return variable_generator.generate_variable(self.features['interface_name'], self.model, 'ftvar', name, variable_bound, variable_dim)
 
         return self.vars[name]
 
     def bvar(self, name, variable_dim=0, variable_bound=[0, 1]):
 
         """
         Binary Variable Definition
@@ -1195,15 +1184,15 @@
         print(A)
         print("~~~~~~~~~~~~\n")
 
         return A
 
     def report(self):
 
-        print("\n~~~~~~~~~~~~~~\nFELOOPY v0.2.3\n~~~~~~~~~~~~~~")
+        print("\n~~~~~~~~~~~~~~\nFELOOPY v0.2.4\n~~~~~~~~~~~~~~")
 
         import datetime
 
         e = datetime.datetime.now()
 
         print("\n~~~~~~~~~~~\nDATE & TIME\n~~~~~~~~~~~")
         print(e.strftime("%Y-%m-%d %H:%M:%S"))
@@ -1995,15 +1984,15 @@
         print(A)
         print("~~~~~~~~~~~~\n")
 
         return A
 
     def report(self):
 
-        print("\n~~~~~~~~~~~~~~\nFELOOPY v0.2.3\n~~~~~~~~~~~~~~")
+        print("\n~~~~~~~~~~~~~~\nFELOOPY v0.2.4\n~~~~~~~~~~~~~~")
 
         import datetime
 
         e = datetime.datetime.now()
 
         print("\n~~~~~~~~~~~\nDATE & TIME\n~~~~~~~~~~~")
         print(e.strftime("%Y-%m-%d %H:%M:%S"))
```

### Comparing `feloopy-0.2.31/feloopy/functions/heuristic_operators.py` & `feloopy-0.2.4/feloopy/functions/heuristic_operators.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/functions/update_operators.py` & `feloopy-0.2.4/feloopy/functions/update_operators.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/model/feloopy_model_generator.py` & `feloopy-0.2.4/feloopy/generators/model/feloopy_model_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/model/mealpy_model_generator.py` & `feloopy-0.2.4/feloopy/generators/model/mealpy_model_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/model_generator.py` & `feloopy-0.2.4/feloopy/generators/model_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/result/gekko_result_generator.py` & `feloopy-0.2.4/feloopy/generators/result/gekko_result_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/result/gurobi_result_generator.py` & `feloopy-0.2.4/feloopy/generators/result/gurobi_result_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/result/ortools_cp_result_generator.py` & `feloopy-0.2.4/feloopy/generators/result/ortools_cp_result_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/result/ortools_result_generator.py` & `feloopy-0.2.4/feloopy/generators/result/ortools_result_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/result_generator.py` & `feloopy-0.2.4/feloopy/generators/result_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/solution/cplex_cp_solution_generator.py` & `feloopy-0.2.4/feloopy/generators/solution/cplex_cp_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/solution/cplex_solution_generator.py` & `feloopy-0.2.4/feloopy/generators/solution/cplex_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/solution/cvxpy_solution_generator.py` & `feloopy-0.2.4/feloopy/generators/solution/cvxpy_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/solution/cylp_solution_generator.py` & `feloopy-0.2.4/feloopy/generators/solution/cylp_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/solution/feloopy_solution_generator.py` & `feloopy-0.2.4/feloopy/generators/solution/feloopy_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/solution/gekko_solution_generator.py` & `feloopy-0.2.4/feloopy/generators/solution/gekko_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/solution/gurobi_solution_generator.py` & `feloopy-0.2.4/feloopy/generators/solution/gurobi_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/solution/linopy_solution_generator.py` & `feloopy-0.2.4/feloopy/generators/solution/linopy_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/solution/mealpy_solution_generator.py` & `feloopy-0.2.4/feloopy/generators/solution/mealpy_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/solution/mip_solution_generator.py` & `feloopy-0.2.4/feloopy/generators/solution/mip_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/solution/ortools_cp_solution_generator.py` & `feloopy-0.2.4/feloopy/generators/solution/ortools_cp_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/solution/ortools_solution_generator.py` & `feloopy-0.2.4/feloopy/generators/solution/ortools_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/solution/picos_solution_generator.py` & `feloopy-0.2.4/feloopy/generators/solution/picos_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/solution/pulp_solution_generator.py` & `feloopy-0.2.4/feloopy/generators/solution/pulp_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/solution/pymprog_solution_generator.py` & `feloopy-0.2.4/feloopy/generators/solution/pymprog_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/solution/pyomo_solution_generator.py` & `feloopy-0.2.4/feloopy/generators/solution/pyomo_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/solution/xpress_solution_generator.py` & `feloopy-0.2.4/feloopy/generators/solution/xpress_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/solution_generator.py` & `feloopy-0.2.4/feloopy/generators/solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/variable/cplex_cp_variable_generator.py` & `feloopy-0.2.4/feloopy/generators/variable/cplex_cp_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/variable/cplex_variable_generator.py` & `feloopy-0.2.4/feloopy/generators/variable/cplex_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/variable/cvxpy_variable_generator.py` & `feloopy-0.2.4/feloopy/generators/variable/cvxpy_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/variable/cylp_variable_generator.py` & `feloopy-0.2.4/feloopy/generators/variable/cylp_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/variable/gekko_variable_generator.py` & `feloopy-0.2.4/feloopy/generators/variable/gekko_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/variable/gurobi_variable_generator.py` & `feloopy-0.2.4/feloopy/generators/variable/gurobi_variable_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,29 +133,29 @@
 
                     generated_variable = model_object.addMVar((len(variable_dim[0]),len(variable_dim[1])),vtype=POSITIVE,lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
 
                 else:
                     
                     generated_variable = model_object.addMVar(tuple([len(key) for key in variable_dim]),vtype=POSITIVE,lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
 
-        case 'ptvar':
+        case 'ftvar':
 
             '''
 
             Free Tensor Variable Generator
 
             '''
 
             if variable_dim == 0: generated_variable = model_object.addVar(vtype=FREE, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
 
             else:
                 
-                if len(variable_dim) == 1:generated_variable = model_object.addMVar((len(variable_dim[0])),vtype=FREE,lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
-                elif len(variable_dim) == 2:generated_variable = model_object.addMVar((len(variable_dim[0]),len(variable_dim[1])),vtype=FREE,lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
-                else:generated_variable = model_object.addMVar(tuple([len(key) for key in variable_dim]),vtype=FREE,lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+                if len(variable_dim) == 1: generated_variable = model_object.addMVar((len(variable_dim[0])),vtype=FREE,lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+                elif len(variable_dim) == 2: generated_variable = model_object.addMVar((len(variable_dim[0]),len(variable_dim[1])),vtype=FREE,lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+                else: generated_variable = model_object.addMVar(tuple([len(key) for key in variable_dim]),vtype=FREE,lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
 
 
         case 'btvar':
 
             '''
 
             Binary Tensor Variable Generator
```

### Comparing `feloopy-0.2.31/feloopy/generators/variable/linopy_variable_generator.py` & `feloopy-0.2.4/feloopy/generators/variable/linopy_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/variable/mip_variable_generator.py` & `feloopy-0.2.4/feloopy/generators/variable/mip_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/variable/ortools_cp_variable_generator.py` & `feloopy-0.2.4/feloopy/generators/variable/ortools_cp_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/variable/ortools_variable_generator.py` & `feloopy-0.2.4/feloopy/generators/variable/ortools_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/variable/picos_variable_generator.py` & `feloopy-0.2.4/feloopy/generators/variable/picos_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/variable/pulp_variable_generator.py` & `feloopy-0.2.4/feloopy/generators/variable/pulp_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/variable/pymprog_variable_generator.py` & `feloopy-0.2.4/feloopy/generators/variable/pymprog_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/variable/pyomo_variable_generator.py` & `feloopy-0.2.4/feloopy/generators/variable/pyomo_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/variable/xpress_variable_generator.py` & `feloopy-0.2.4/feloopy/generators/variable/xpress_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/generators/variable_generator.py` & `feloopy-0.2.4/feloopy/generators/variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy/operators/common.py` & `feloopy-0.2.4/feloopy/operators/common.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/feloopy.egg-info/PKG-INFO` & `feloopy-0.2.4/feloopy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feloopy
-Version: 0.2.31
+Version: 0.2.4
 Summary: FelooPy: An Integrated Optimization Environment (IOE) for Automated operations research (AutoOR) in Python.
 Home-page: https://github.com/ktafakkori/feloopy
 Download-URL: https://github.com/ktafakkori/feloopy/releases
 Author: Keivan Tafakkori
 Author-email: k.tafakkori@gmail.com
 Maintainer: Keivan Tafakkori
 Maintainer-email: k.tafakkori@gmail.com
@@ -59,17 +59,17 @@
 
 <div align="center">
 
 <div align="left">
 
 ## News
 
-🎉 _Version 0.2.3 is out: More stable than ever!_ 🎉
+🎉 _Version 0.2.4 is out: Added new functionalities!_ 🎉
 
-🎉 _The next version would focus on solve facilities_ 🎉
+🎉 _The next version would focus on more facilities_ 🎉
 
 💻 _Quick install_: `pip install --upgrade feloopy`
 
 #
 
 ## Introduction
 
@@ -154,23 +154,23 @@
 [vs]: https://code.visualstudio.com/
 [sp]: https://www.anaconda.com/
 [gc]: https://colab.research.google.com/
 
 ### Method 1: Terminal command (e.g., CMD or GC):
 
 ```text
-pip install feloopy==0.2.3
+pip install feloopy==0.2.4
 ```
 
 ### Method 2: IDE command (e.g., Spyder):
 
 _Note_: After installation, this line of code should be deleted.
 
 ```text
-!pip install feloopy==0.2.3
+!pip install feloopy==0.2.4
 ```
 
 ### Method 3: Inside your Python code
 
 _Note_: After installation, this piece of code should be deleted.
 
 ```text
@@ -183,15 +183,15 @@
         pip._internal.main(['install','-U', package])
 
 install('feloopy')
 ```
 
 ### Method 4: From GitHub [Releases][a] section
 
-1. Download the [feloopy-0.2.3.zip][c] file.
+1. Download the [feloopy-0.2.4.zip][c] file.
 2. Extract it into a specific directory.
 3. Open a terminal in that directory.
 4. Type: `pip install .`
 
 [a]: https://github.com/ktafakkori/feloopy/releases
 [b]: https://git-scm.com/downloads
 [c]: https://github.com/ktafakkori/feloopy/releases/download/0.2.3/feloopy-0.2.3.zip
@@ -249,27 +249,27 @@
 ## Citation
 
 It is recommended to cite this GitHub repository or the Python library if you use its facilities in your work:
 
 - APA 7:
 
 ```text
-Tafakkori, K. (2023). FelooPy: An integrated optimization environment for AutoOR in Python (0.2.3) [Python Library]. https://github.com/ktafakkori/feloopy (Original work published 2023)
+Tafakkori, K. (2023). FelooPy: An integrated optimization environment for AutoOR in Python (0.2.4) [Python Library]. https://github.com/ktafakkori/feloopy (Original work published 2023)
 ```
 
 - LaTeX:
 
 ```text
-@software{ktafakkori2023Feb,
+@software{ktafakkori2023Apr,
   author       = {Keivan Tafakkori},
   title        = {{FelooPy: An integrated optimization environment for AutoOR in Python}},
   year         = {2023},
-  month        = feb,
+  month        = apr,
   publisher    = {GitHub},
-  version      = {v0.2.3},
+  version      = {v0.2.4},
   url          = {https://github.com/ktafakkori/feloopy/}
 }
 ```
 
 ## License
 
 FelooPy is completely free and open-source and licensed under the [MIT][08] license.
```

### Comparing `feloopy-0.2.31/feloopy.egg-info/SOURCES.txt` & `feloopy-0.2.4/feloopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/setup.py` & `feloopy-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
 
     name='feloopy',
 
-    version='0.2.31',
+    version='0.2.4',
 
     description='FelooPy: An Integrated Optimization Environment (IOE) for Automated operations research (AutoOR) in Python.',
 
     long_description=open('README.md', encoding="utf8").read(),
 
     long_description_content_type='text/markdown',
```

### Comparing `feloopy-0.2.31/tests/test_exact_kp.py` & `feloopy-0.2.4/tests/test_exact_kp.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.31/tests/test_exact_tsp.py` & `feloopy-0.2.4/tests/test_exact_tsp.py`

 * *Files identical despite different names*

