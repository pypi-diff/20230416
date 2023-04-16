# Comparing `tmp/pyristic-1.4.0.tar.gz` & `tmp/pyristic-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyristic-1.4.0.tar", last modified: Sun Feb  5 03:24:43 2023, max compression
+gzip compressed data, was "pyristic-1.4.1.tar", last modified: Sun Apr 16 01:02:21 2023, max compression
```

## Comparing `pyristic-1.4.0.tar` & `pyristic-1.4.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 armando    (501) staff       (20)        0 2023-02-05 03:24:43.352209 pyristic-1.4.0/
--rw-r--r--   0 armando    (501) staff       (20)     1080 2022-08-07 02:06:56.000000 pyristic-1.4.0/LICENSE
--rw-r--r--   0 armando    (501) staff       (20)     4146 2023-02-05 03:24:43.352037 pyristic-1.4.0/PKG-INFO
--rw-r--r--   0 armando    (501) staff       (20)     3396 2022-08-07 02:06:56.000000 pyristic-1.4.0/README.md
-drwxr-xr-x   0 armando    (501) staff       (20)        0 2023-02-05 03:24:43.347061 pyristic-1.4.0/pyristic/
--rw-r--r--   0 armando    (501) staff       (20)       22 2023-02-05 03:21:46.000000 pyristic-1.4.0/pyristic/__init__.py
-drwxr-xr-x   0 armando    (501) staff       (20)        0 2023-02-05 03:24:43.349382 pyristic-1.4.0/pyristic/heuristic/
--rw-r--r--   0 armando    (501) staff       (20)    11904 2023-02-01 04:45:37.000000 pyristic-1.4.0/pyristic/heuristic/EvolutionStrategy_search.py
--rw-r--r--   0 armando    (501) staff       (20)    10013 2023-02-01 04:45:37.000000 pyristic-1.4.0/pyristic/heuristic/EvolutiveProgramming_search.py
--rw-r--r--   0 armando    (501) staff       (20)    11820 2023-02-01 04:45:37.000000 pyristic-1.4.0/pyristic/heuristic/GeneticAlgorithm_search.py
--rw-r--r--   0 armando    (501) staff       (20)     4993 2023-02-01 04:45:37.000000 pyristic-1.4.0/pyristic/heuristic/SimulatedAnnealing_search.py
--rw-r--r--   0 armando    (501) staff       (20)     9091 2023-02-01 04:45:37.000000 pyristic-1.4.0/pyristic/heuristic/Tabu_search.py
--rw-r--r--   0 armando    (501) staff       (20)      260 2022-08-15 01:37:37.000000 pyristic-1.4.0/pyristic/heuristic/__init__.py
-drwxr-xr-x   0 armando    (501) staff       (20)        0 2023-02-05 03:24:43.350300 pyristic-1.4.0/pyristic/utils/
--rw-r--r--   0 armando    (501) staff       (20)      215 2023-02-01 04:45:37.000000 pyristic-1.4.0/pyristic/utils/__init__.py
--rw-r--r--   0 armando    (501) staff       (20)     5751 2023-02-01 04:45:37.000000 pyristic-1.4.0/pyristic/utils/evolutionary_config.py
--rw-r--r--   0 armando    (501) staff       (20)     4260 2023-02-04 19:41:24.000000 pyristic-1.4.0/pyristic/utils/helpers.py
-drwxr-xr-x   0 armando    (501) staff       (20)        0 2023-02-05 03:24:43.351638 pyristic-1.4.0/pyristic/utils/operators/
--rw-r--r--   0 armando    (501) staff       (20)      107 2023-02-01 04:45:37.000000 pyristic-1.4.0/pyristic/utils/operators/__init__.py
--rw-r--r--   0 armando    (501) staff       (20)    13821 2023-02-01 04:45:38.000000 pyristic-1.4.0/pyristic/utils/operators/crossover.py
--rw-r--r--   0 armando    (501) staff       (20)    18929 2023-02-01 04:45:38.000000 pyristic-1.4.0/pyristic/utils/operators/mutation.py
--rw-r--r--   0 armando    (501) staff       (20)     2803 2023-02-01 04:45:38.000000 pyristic-1.4.0/pyristic/utils/operators/population_sample.py
--rw-r--r--   0 armando    (501) staff       (20)    12545 2023-02-01 04:45:38.000000 pyristic-1.4.0/pyristic/utils/operators/selection.py
--rw-r--r--   0 armando    (501) staff       (20)     3960 2023-02-01 04:45:38.000000 pyristic-1.4.0/pyristic/utils/test_function.py
-drwxr-xr-x   0 armando    (501) staff       (20)        0 2023-02-05 03:24:43.347823 pyristic-1.4.0/pyristic.egg-info/
--rw-r--r--   0 armando    (501) staff       (20)     4146 2023-02-05 03:24:43.000000 pyristic-1.4.0/pyristic.egg-info/PKG-INFO
--rw-r--r--   0 armando    (501) staff       (20)      781 2023-02-05 03:24:43.000000 pyristic-1.4.0/pyristic.egg-info/SOURCES.txt
--rw-r--r--   0 armando    (501) staff       (20)        1 2023-02-05 03:24:43.000000 pyristic-1.4.0/pyristic.egg-info/dependency_links.txt
--rw-r--r--   0 armando    (501) staff       (20)       27 2023-02-05 03:24:43.000000 pyristic-1.4.0/pyristic.egg-info/requires.txt
--rw-r--r--   0 armando    (501) staff       (20)        9 2023-02-05 03:24:43.000000 pyristic-1.4.0/pyristic.egg-info/top_level.txt
--rw-r--r--   0 armando    (501) staff       (20)       38 2023-02-05 03:24:43.352258 pyristic-1.4.0/setup.cfg
--rw-r--r--   0 armando    (501) staff       (20)     1122 2023-02-05 03:21:44.000000 pyristic-1.4.0/setup.py
+drwxr-xr-x   0 armando    (501) staff       (20)        0 2023-04-16 01:02:21.997298 pyristic-1.4.1/
+-rw-r--r--   0 armando    (501) staff       (20)     1080 2022-08-07 02:06:56.000000 pyristic-1.4.1/LICENSE
+-rw-r--r--   0 armando    (501) staff       (20)     4146 2023-04-16 01:02:21.996638 pyristic-1.4.1/PKG-INFO
+-rw-r--r--   0 armando    (501) staff       (20)     3396 2022-08-07 02:06:56.000000 pyristic-1.4.1/README.md
+drwxr-xr-x   0 armando    (501) staff       (20)        0 2023-04-16 01:02:21.990682 pyristic-1.4.1/pyristic/
+-rw-r--r--   0 armando    (501) staff       (20)       22 2023-04-16 00:56:08.000000 pyristic-1.4.1/pyristic/__init__.py
+drwxr-xr-x   0 armando    (501) staff       (20)        0 2023-04-16 01:02:21.993563 pyristic-1.4.1/pyristic/heuristic/
+-rw-r--r--   0 armando    (501) staff       (20)    11904 2023-02-01 04:45:37.000000 pyristic-1.4.1/pyristic/heuristic/EvolutionStrategy_search.py
+-rw-r--r--   0 armando    (501) staff       (20)    10013 2023-02-01 04:45:37.000000 pyristic-1.4.1/pyristic/heuristic/EvolutiveProgramming_search.py
+-rw-r--r--   0 armando    (501) staff       (20)    11820 2023-02-01 04:45:37.000000 pyristic-1.4.1/pyristic/heuristic/GeneticAlgorithm_search.py
+-rw-r--r--   0 armando    (501) staff       (20)     4993 2023-02-01 04:45:37.000000 pyristic-1.4.1/pyristic/heuristic/SimulatedAnnealing_search.py
+-rw-r--r--   0 armando    (501) staff       (20)     9104 2023-04-16 00:46:06.000000 pyristic-1.4.1/pyristic/heuristic/Tabu_search.py
+-rw-r--r--   0 armando    (501) staff       (20)      260 2022-08-15 01:37:37.000000 pyristic-1.4.1/pyristic/heuristic/__init__.py
+drwxr-xr-x   0 armando    (501) staff       (20)        0 2023-04-16 01:02:21.994667 pyristic-1.4.1/pyristic/utils/
+-rw-r--r--   0 armando    (501) staff       (20)      215 2023-02-01 04:45:37.000000 pyristic-1.4.1/pyristic/utils/__init__.py
+-rw-r--r--   0 armando    (501) staff       (20)     5751 2023-02-01 04:45:37.000000 pyristic-1.4.1/pyristic/utils/evolutionary_config.py
+-rw-r--r--   0 armando    (501) staff       (20)     4260 2023-04-16 00:44:59.000000 pyristic-1.4.1/pyristic/utils/helpers.py
+drwxr-xr-x   0 armando    (501) staff       (20)        0 2023-04-16 01:02:21.996235 pyristic-1.4.1/pyristic/utils/operators/
+-rw-r--r--   0 armando    (501) staff       (20)      107 2023-02-01 04:45:37.000000 pyristic-1.4.1/pyristic/utils/operators/__init__.py
+-rw-r--r--   0 armando    (501) staff       (20)    13821 2023-02-01 04:45:38.000000 pyristic-1.4.1/pyristic/utils/operators/crossover.py
+-rw-r--r--   0 armando    (501) staff       (20)    18929 2023-02-01 04:45:38.000000 pyristic-1.4.1/pyristic/utils/operators/mutation.py
+-rw-r--r--   0 armando    (501) staff       (20)     2803 2023-02-01 04:45:38.000000 pyristic-1.4.1/pyristic/utils/operators/population_sample.py
+-rw-r--r--   0 armando    (501) staff       (20)    12545 2023-02-01 04:45:38.000000 pyristic-1.4.1/pyristic/utils/operators/selection.py
+-rw-r--r--   0 armando    (501) staff       (20)     3960 2023-02-01 04:45:38.000000 pyristic-1.4.1/pyristic/utils/test_function.py
+drwxr-xr-x   0 armando    (501) staff       (20)        0 2023-04-16 01:02:21.991652 pyristic-1.4.1/pyristic.egg-info/
+-rw-r--r--   0 armando    (501) staff       (20)     4146 2023-04-16 01:02:21.000000 pyristic-1.4.1/pyristic.egg-info/PKG-INFO
+-rw-r--r--   0 armando    (501) staff       (20)      781 2023-04-16 01:02:21.000000 pyristic-1.4.1/pyristic.egg-info/SOURCES.txt
+-rw-r--r--   0 armando    (501) staff       (20)        1 2023-04-16 01:02:21.000000 pyristic-1.4.1/pyristic.egg-info/dependency_links.txt
+-rw-r--r--   0 armando    (501) staff       (20)       27 2023-04-16 01:02:21.000000 pyristic-1.4.1/pyristic.egg-info/requires.txt
+-rw-r--r--   0 armando    (501) staff       (20)        9 2023-04-16 01:02:21.000000 pyristic-1.4.1/pyristic.egg-info/top_level.txt
+-rw-r--r--   0 armando    (501) staff       (20)       38 2023-04-16 01:02:21.997386 pyristic-1.4.1/setup.cfg
+-rw-r--r--   0 armando    (501) staff       (20)     1122 2023-04-16 01:00:47.000000 pyristic-1.4.1/setup.py
```

### Comparing `pyristic-1.4.0/LICENSE` & `pyristic-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyristic-1.4.0/PKG-INFO` & `pyristic-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyristic
-Version: 1.4.0
+Version: 1.4.1
 Summary: Set of metaheuristic for solve optimization problems.
 Home-page: https://github.com/JAOP1/
-Download-URL: https://github.com/JAOP1/pyristic/archive/refs/tags/v1.4.0.tar.gz
+Download-URL: https://github.com/JAOP1/pyristic/archive/refs/tags/v1.4.1.tar.gz
 Author: Jesús Armando Ortíz Peñafiel
 Author-email: armandopenafiel12@gmail.com
 License: MIT
 Keywords: Optimization,Metaheuristic,Python
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pyristic-1.4.0/README.md` & `pyristic-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyristic-1.4.0/pyristic/heuristic/EvolutionStrategy_search.py` & `pyristic-1.4.1/pyristic/heuristic/EvolutionStrategy_search.py`

 * *Files identical despite different names*

### Comparing `pyristic-1.4.0/pyristic/heuristic/EvolutiveProgramming_search.py` & `pyristic-1.4.1/pyristic/heuristic/EvolutiveProgramming_search.py`

 * *Files identical despite different names*

### Comparing `pyristic-1.4.0/pyristic/heuristic/GeneticAlgorithm_search.py` & `pyristic-1.4.1/pyristic/heuristic/GeneticAlgorithm_search.py`

 * *Files identical despite different names*

### Comparing `pyristic-1.4.0/pyristic/heuristic/SimulatedAnnealing_search.py` & `pyristic-1.4.1/pyristic/heuristic/SimulatedAnnealing_search.py`

 * *Files identical despite different names*

### Comparing `pyristic-1.4.0/pyristic/heuristic/Tabu_search.py` & `pyristic-1.4.1/pyristic/heuristic/Tabu_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,18 @@
         self.tabu_list = [[None, None, -1, 100000000]]
         self.timer = timer
 
     def __str__(self):
         printable_object = "\n ---- Tabu list: ---- \n"
         printable_object += f"List size: {self.tabu_list} \n"
         for position, value, iteration, current_timer in self.tabu_list:
-            printable_object += f"p: {position} v:{value} Iteration: {iteration} current timer: {current_timer} \n"
+            printable_object += (
+                f"p: {position} v:{value} Iteration: "
+                f"{iteration} current timer: {current_timer} \n"
+            )
         return printable_object
 
     def push(self, solution: list) -> None:
         """
         Description:
             Append a solution during a time in the tabu list.
         Arguments:
@@ -80,15 +83,15 @@
         Arguments:
             - solution: it is an array of two elements. The first position
             is the location in the current solution and the second position is
             the value replaced.
         """
         # X is [p, v], where p is the position changed and v the new value.
         assert len(solution) == 2
-        for position, value, *internal_items in self.tabu_list:
+        for position, value, *_ in self.tabu_list:
             if solution[0] == position and solution[1] == value:
                 return True
         return False
 
     def reset(self, timer: int) -> None:
         """
         Description:
@@ -132,15 +135,14 @@
 
     def __init__(
         self,
         function: typing.Callable[[np.ndarray], typing.Union[int, float]],
         constraints: list,
         tabu_struct=TabuList(),
     ):
-
         self.tabu_list = tabu_struct  # Initialize tabulist
         self.constraints = constraints
         self.function = function
 
         # Search information.
         self.logger = {}
         self.logger["best_individual"] = None
@@ -183,68 +185,59 @@
             - Init: Numpy array, represent the initial solution or function which generates a random
               initial solution (this solution should be a numpy array).
             - Iterations:  Integer, stop condition.
             - Memory time: Integer, time which a solution is in the tabu list
         ------------------------------------------------------
         """
         try:
-            best_candidate = initial_solution()
+            x_candidate = initial_solution()
         except TypeError:
-            best_candidate = copy.deepcopy(initial_solution)
+            x_candidate = copy.deepcopy(initial_solution)
 
+        f_candidate = self.function(x_candidate)
         self.tabu_list.reset(memory_time)
-
-        self.logger["best_individual"] = None
-        self.logger["best_f"] = None
-
-        f_candidate = self.function(best_candidate)
-
+        self.logger["best_individual"] = np.copy(x_candidate)
+        self.logger["best_f"] = f_candidate
         try:
-            for step_ in tqdm(range(1, iterations + 1), disable=not verbose):
+            for step in tqdm(range(1, iterations + 1), disable=not verbose):
 
                 neighbors = [
                     neighbor
-                    for neighbor in self.get_neighbors(best_candidate, **kwargs)
+                    for neighbor in self.get_neighbors(x_candidate, **kwargs)
                     if not self.tabu_list.find(
-                        self.encode_change(neighbor, best_candidate, **kwargs)
+                        self.encode_change(neighbor, x_candidate, **kwargs)
                     )
                 ]
                 neighbors = np.array(neighbors)
+                try:
+                    neighbors = neighbors[
+                        np.apply_along_axis(self.is_valid, 1, neighbors), :
+                    ]
+                    f_candidates = np.apply_along_axis(
+                        self.function, 1, neighbors
+                    )
 
-                valid_neighbors = neighbors[
-                    np.apply_along_axis(self.is_valid, 1, neighbors), :
-                ]
-
-                # Check if there exists a valid neighbor
-                if len(valid_neighbors) == 0:
-                    continue
-
-                f_feasible_candidates = np.apply_along_axis(
-                    self.function, 1, valid_neighbors
-                )
-
-                ind_min = np.argmin(f_feasible_candidates)
-
-                position, value = self.encode_change(
-                    valid_neighbors[ind_min], best_candidate, **kwargs
-                )
-                self.tabu_list.push([position, value, step_])
-
-                if f_feasible_candidates[ind_min] < f_candidate:
-                    best_candidate = copy.deepcopy(valid_neighbors[ind_min])
-                    f_candidate = f_feasible_candidates[ind_min]
+                    ind_min = np.argmin(f_candidates)
 
+                    position, value = self.encode_change(
+                        neighbors[ind_min], x_candidate, **kwargs
+                    )
+                    self.tabu_list.push([position, value, step])
+                    x_candidate = neighbors[ind_min]
+                    f_candidate = f_candidates
+                    if f_candidates[ind_min] < self.logger["best_f"]:
+                        self.logger["best_individual"] = copy.deepcopy(neighbors[ind_min])
+                        self.logger["best_f"] = f_candidates[ind_min]
+                except ValueError:
+                    pass
                 self.tabu_list.update()
 
         except KeyboardInterrupt:
             LOGGER.error("Interrupted, saving best solution found so far.")
 
-        self.logger["best_individual"] = best_candidate
-        self.logger["best_f"] = f_candidate
-
     def is_valid(self, solution: np.ndarray) -> bool:
         """
         ------------------------------------------------------
         Description:
             Check if the current solution is valid.
         ------------------------------------------------------
         """
```

### Comparing `pyristic-1.4.0/pyristic/utils/evolutionary_config.py` & `pyristic-1.4.1/pyristic/utils/evolutionary_config.py`

 * *Files identical despite different names*

### Comparing `pyristic-1.4.0/pyristic/utils/helpers.py` & `pyristic-1.4.1/pyristic/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         - optimizer_additional_args(optional): additional arguments passed to optimizer.
         - transformer: Function that return a float value. The fuction input is
             the best individual obtained after an execution.
         - verbose: display every solution and objective function.
     ------------------------------------------------------
     """
     data_by_execution = {"execution_time": [], "individual_x": [], "individual_f": []}
-    for i in tqdm(range(num_iterations), file=tqdm_logger, miniters=4,):
+    for _ in tqdm(range(num_iterations), file=tqdm_logger, miniters=4,):
         start_time = time.time()
         optimizer.optimize(*optimizer_args, **optimizer_additional_args)
         data_by_execution["execution_time"].append(time.time() - start_time)
         data_by_execution["individual_x"].append(optimizer.logger["best_individual"])
         function_value = optimizer.logger["best_f"]
         if transformer is not None:
             function_value = transformer(optimizer.logger["best_individual"])
```

### Comparing `pyristic-1.4.0/pyristic/utils/operators/crossover.py` & `pyristic-1.4.1/pyristic/utils/operators/crossover.py`

 * *Files identical despite different names*

### Comparing `pyristic-1.4.0/pyristic/utils/operators/mutation.py` & `pyristic-1.4.1/pyristic/utils/operators/mutation.py`

 * *Files identical despite different names*

### Comparing `pyristic-1.4.0/pyristic/utils/operators/population_sample.py` & `pyristic-1.4.1/pyristic/utils/operators/population_sample.py`

 * *Files identical despite different names*

### Comparing `pyristic-1.4.0/pyristic/utils/operators/selection.py` & `pyristic-1.4.1/pyristic/utils/operators/selection.py`

 * *Files identical despite different names*

### Comparing `pyristic-1.4.0/pyristic/utils/test_function.py` & `pyristic-1.4.1/pyristic/utils/test_function.py`

 * *Files identical despite different names*

### Comparing `pyristic-1.4.0/pyristic.egg-info/PKG-INFO` & `pyristic-1.4.1/pyristic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyristic
-Version: 1.4.0
+Version: 1.4.1
 Summary: Set of metaheuristic for solve optimization problems.
 Home-page: https://github.com/JAOP1/
-Download-URL: https://github.com/JAOP1/pyristic/archive/refs/tags/v1.4.0.tar.gz
+Download-URL: https://github.com/JAOP1/pyristic/archive/refs/tags/v1.4.1.tar.gz
 Author: Jesús Armando Ortíz Peñafiel
 Author-email: armandopenafiel12@gmail.com
 License: MIT
 Keywords: Optimization,Metaheuristic,Python
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pyristic-1.4.0/pyristic.egg-info/SOURCES.txt` & `pyristic-1.4.1/pyristic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyristic-1.4.0/setup.py` & `pyristic-1.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 with open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 
 setup(
     name="pyristic",
-    version="v1.4.0",
+    version="v1.4.1",
     license="MIT",
     description="Set of metaheuristic for solve optimization problems.",
     author="Jesús Armando Ortíz Peñafiel",
     author_email="armandopenafiel12@gmail.com",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/JAOP1/",
-    download_url="https://github.com/JAOP1/pyristic/archive/refs/tags/v1.4.0.tar.gz",
+    download_url="https://github.com/JAOP1/pyristic/archive/refs/tags/v1.4.1.tar.gz",
     keywords=["Optimization", "Metaheuristic", "Python"],
     install_requires=[
         "numpy>=1.15.4",
         "tqdm>=4.28.1",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
```

