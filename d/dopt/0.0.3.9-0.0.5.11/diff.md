# Comparing `tmp/dopt-0.0.3.9.tar.gz` & `tmp/dopt-0.0.5.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dopt-0.0.3.9.tar", last modified: Tue Jul 14 14:02:25 2020, max compression
+gzip compressed data, was "dist/dopt-0.0.5.11.tar", last modified: Sun Sep 19 20:40:44 2021, max compression
```

## Comparing `dopt-0.0.3.9.tar` & `dopt-0.0.5.11.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxr-x   0 tung      (1003) tung      (1003)        0 2020-07-14 14:02:25.000000 dopt-0.0.3.9/
--rw-rw-r--   0 tung      (1003) tung      (1003)     2916 2020-07-14 14:02:25.000000 dopt-0.0.3.9/PKG-INFO
--rw-rw-r--   0 tung      (1003) tung      (1003)     2240 2020-07-05 07:47:19.000000 dopt-0.0.3.9/README.md
-drwxrwxr-x   0 tung      (1003) tung      (1003)        0 2020-07-14 14:02:25.000000 dopt-0.0.3.9/dopt/
--rw-rw-r--   0 tung      (1003) tung      (1003)      199 2020-07-14 14:02:20.000000 dopt-0.0.3.9/dopt/__init__.py
-drwxrwxr-x   0 tung      (1003) tung      (1003)        0 2020-07-14 14:02:25.000000 dopt-0.0.3.9/dopt/optimizers/
--rw-rw-r--   0 tung      (1003) tung      (1003)      152 2020-07-05 07:47:19.000000 dopt-0.0.3.9/dopt/optimizers/__init__.py
--rw-rw-r--   0 tung      (1003) tung      (1003)     9432 2020-07-14 03:15:42.000000 dopt-0.0.3.9/dopt/optimizers/neioptimizer.py
--rw-rw-r--   0 tung      (1003) tung      (1003)     5285 2020-07-13 09:33:03.000000 dopt-0.0.3.9/dopt/optimizers/optimizer.py
--rw-rw-r--   0 tung      (1003) tung      (1003)     8265 2020-07-14 13:48:46.000000 dopt-0.0.3.9/dopt/server.py
-drwxrwxr-x   0 tung      (1003) tung      (1003)        0 2020-07-14 14:02:25.000000 dopt-0.0.3.9/dopt/synthetic_objective_function/
--rw-rw-r--   0 tung      (1003) tung      (1003)        0 2020-07-11 03:17:48.000000 dopt-0.0.3.9/dopt/synthetic_objective_function/__init__.py
--rw-rw-r--   0 tung      (1003) tung      (1003)     7587 2020-07-14 14:00:56.000000 dopt-0.0.3.9/dopt/trainer.py
-drwxrwxr-x   0 tung      (1003) tung      (1003)        0 2020-07-14 14:02:25.000000 dopt-0.0.3.9/dopt/utils/
--rw-rw-r--   0 tung      (1003) tung      (1003)      166 2020-07-11 03:17:48.000000 dopt-0.0.3.9/dopt/utils/__init__.py
--rw-rw-r--   0 tung      (1003) tung      (1003)     2696 2020-07-11 07:33:54.000000 dopt-0.0.3.9/dopt/utils/general_utils.py
--rw-rw-r--   0 tung      (1003) tung      (1003)     1477 2020-07-11 03:17:48.000000 dopt-0.0.3.9/dopt/utils/ssh_utils.py
-drwxrwxr-x   0 tung      (1003) tung      (1003)        0 2020-07-14 14:02:25.000000 dopt-0.0.3.9/dopt.egg-info/
--rw-rw-r--   0 tung      (1003) tung      (1003)     2916 2020-07-14 14:02:25.000000 dopt-0.0.3.9/dopt.egg-info/PKG-INFO
--rw-rw-r--   0 tung      (1003) tung      (1003)      452 2020-07-14 14:02:25.000000 dopt-0.0.3.9/dopt.egg-info/SOURCES.txt
--rw-rw-r--   0 tung      (1003) tung      (1003)        1 2020-07-14 14:02:25.000000 dopt-0.0.3.9/dopt.egg-info/dependency_links.txt
--rw-rw-r--   0 tung      (1003) tung      (1003)       11 2020-07-14 14:02:25.000000 dopt-0.0.3.9/dopt.egg-info/top_level.txt
--rw-rw-r--   0 tung      (1003) tung      (1003)       38 2020-07-14 14:02:25.000000 dopt-0.0.3.9/setup.cfg
--rw-rw-r--   0 tung      (1003) tung      (1003)      634 2020-07-14 14:02:18.000000 dopt-0.0.3.9/setup.py
-drwxrwxr-x   0 tung      (1003) tung      (1003)        0 2020-07-14 14:02:25.000000 dopt-0.0.3.9/tests/
--rw-rw-r--   0 tung      (1003) tung      (1003)        0 2020-07-05 07:47:20.000000 dopt-0.0.3.9/tests/__init__.py
--rw-rw-r--   0 tung      (1003) tung      (1003)      648 2020-07-05 07:47:20.000000 dopt-0.0.3.9/tests/test_optimizer.py
--rw-rw-r--   0 tung      (1003) tung      (1003)      545 2020-07-05 07:47:20.000000 dopt-0.0.3.9/tests/test_trainer.py
+drwxrwxr-x   0 tung      (1003) tung      (1003)        0 2021-09-19 20:40:44.000000 dopt-0.0.5.11/
+-rw-rw-r--   0 tung      (1003) tung      (1003)     1076 2020-07-11 03:17:48.000000 dopt-0.0.5.11/LICENSE
+-rw-rw-r--   0 tung      (1003) tung      (1003)     2931 2021-09-19 20:40:44.000000 dopt-0.0.5.11/PKG-INFO
+-rw-rw-r--   0 tung      (1003) tung      (1003)     2240 2020-07-05 07:47:19.000000 dopt-0.0.5.11/README.md
+drwxrwxr-x   0 tung      (1003) tung      (1003)        0 2021-09-19 20:40:44.000000 dopt-0.0.5.11/dopt/
+-rw-rw-r--   0 tung      (1003) tung      (1003)      200 2021-09-19 20:26:07.000000 dopt-0.0.5.11/dopt/__init__.py
+drwxrwxr-x   0 tung      (1003) tung      (1003)        0 2021-09-19 20:40:44.000000 dopt-0.0.5.11/dopt/optimizers/
+-rw-rw-r--   0 tung      (1003) tung      (1003)      152 2020-07-05 07:47:19.000000 dopt-0.0.5.11/dopt/optimizers/__init__.py
+-rw-rw-r--   0 tung      (1003) tung      (1003)    11194 2021-06-07 16:33:59.000000 dopt-0.0.5.11/dopt/optimizers/neioptimizer.py
+-rw-rw-r--   0 tung      (1003) tung      (1003)     6892 2021-06-07 13:31:25.000000 dopt-0.0.5.11/dopt/optimizers/optimizer.py
+-rw-rw-r--   0 tung      (1003) tung      (1003)    14409 2021-09-19 20:21:06.000000 dopt-0.0.5.11/dopt/server.py
+drwxrwxr-x   0 tung      (1003) tung      (1003)        0 2021-09-19 20:40:44.000000 dopt-0.0.5.11/dopt/synthetic_objective_function/
+-rw-rw-r--   0 tung      (1003) tung      (1003)        0 2020-07-11 03:17:48.000000 dopt-0.0.5.11/dopt/synthetic_objective_function/__init__.py
+-rw-rw-r--   0 tung      (1003) tung      (1003)    10845 2021-06-07 14:16:22.000000 dopt-0.0.5.11/dopt/trainer.py
+drwxrwxr-x   0 tung      (1003) tung      (1003)        0 2021-09-19 20:40:44.000000 dopt-0.0.5.11/dopt/utils/
+-rw-rw-r--   0 tung      (1003) tung      (1003)      166 2020-07-11 03:17:48.000000 dopt-0.0.5.11/dopt/utils/__init__.py
+-rw-rw-r--   0 tung      (1003) tung      (1003)     2859 2021-06-07 14:20:24.000000 dopt-0.0.5.11/dopt/utils/general_utils.py
+-rw-rw-r--   0 tung      (1003) tung      (1003)     1477 2020-07-11 03:17:48.000000 dopt-0.0.5.11/dopt/utils/ssh_utils.py
+drwxrwxr-x   0 tung      (1003) tung      (1003)        0 2021-09-19 20:40:44.000000 dopt-0.0.5.11/dopt.egg-info/
+-rw-rw-r--   0 tung      (1003) tung      (1003)     2931 2021-09-19 20:40:44.000000 dopt-0.0.5.11/dopt.egg-info/PKG-INFO
+-rw-rw-r--   0 tung      (1003) tung      (1003)      460 2021-09-19 20:40:44.000000 dopt-0.0.5.11/dopt.egg-info/SOURCES.txt
+-rw-rw-r--   0 tung      (1003) tung      (1003)        1 2021-09-19 20:40:44.000000 dopt-0.0.5.11/dopt.egg-info/dependency_links.txt
+-rw-rw-r--   0 tung      (1003) tung      (1003)       11 2021-09-19 20:40:44.000000 dopt-0.0.5.11/dopt.egg-info/top_level.txt
+-rw-rw-r--   0 tung      (1003) tung      (1003)       38 2021-09-19 20:40:44.000000 dopt-0.0.5.11/setup.cfg
+-rw-rw-r--   0 tung      (1003) tung      (1003)      650 2021-09-19 20:25:21.000000 dopt-0.0.5.11/setup.py
+drwxrwxr-x   0 tung      (1003) tung      (1003)        0 2021-09-19 20:40:44.000000 dopt-0.0.5.11/tests/
+-rw-rw-r--   0 tung      (1003) tung      (1003)        0 2020-07-05 07:47:20.000000 dopt-0.0.5.11/tests/__init__.py
+-rw-rw-r--   0 tung      (1003) tung      (1003)      648 2020-07-05 07:47:20.000000 dopt-0.0.5.11/tests/test_optimizer.py
+-rw-rw-r--   0 tung      (1003) tung      (1003)      545 2020-07-05 07:47:20.000000 dopt-0.0.5.11/tests/test_trainer.py
```

### Comparing `dopt-0.0.3.9/PKG-INFO` & `dopt-0.0.5.11/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dopt
-Version: 0.0.3.9
+Version: 0.0.5.11
 Summary: Distributed Optimizer
-Home-page: https://github.com/pypa/sampleproject
+Home-page: https://gitlab.com/tungtran99/distributed-optimizer
 Author: Tung Tran
 Author-email: sontungtran99@gmail.com
 License: UNKNOWN
 Description: 
         ### How to use
         We'll be running `distributed_optimizer.py` to start the optimization.
           
@@ -36,9 +36,9 @@
          - Step 2: Make sure the appropriate environment can be chosen through ssh tunneling. Try: `ssh [name]@[hostmachine] [YOUR COMMANDS]`
          - Step 3: Add the commands to the `COMMANDS` dictionary.
          - Step 4: Make sure you have a copy of the `distributed_optimizer.py` and related files on all of the machines you intend to use
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `dopt-0.0.3.9/README.md` & `dopt-0.0.5.11/README.md`

 * *Files identical despite different names*

### Comparing `dopt-0.0.3.9/dopt/optimizers/neioptimizer.py` & `dopt-0.0.5.11/dopt/optimizers/neioptimizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,19 +19,61 @@
 from botorch.models.model import Model
 from botorch.acquisition.monte_carlo import qNoisyExpectedImprovement
 from botorch.acquisition.objective import IdentityMCObjective, MCAcquisitionObjective
 from botorch.sampling.samplers import MCSampler, SobolQMCNormalSampler
 from botorch.optim import optimize_acqf
 from botorch.acquisition.objective import ConstrainedMCObjective
 from botorch.utils.sampling import draw_sobol_normal_samples
+from botorch.utils.transforms import (
+    concatenate_pending_points,
+    match_batch_shape,
+    t_batch_mode_transform
+)
 
 from dopt.optimizers.optimizer import Optimizer
 from dopt.utils import generate_seed
 
 
+class qNEIModified(qNoisyExpectedImprovement):
+    def __init__(self, model: Model, X_baseline: Tensor,
+        sampler: Optional[MCSampler] = None,
+        objective: Optional[MCAcquisitionObjective] = None,
+        X_pending: Optional[Tensor] = None,
+        prune_baseline: bool = False,
+    ) -> None:
+        super().__init__(model=model, X_baseline=X_baseline, sampler=sampler, objective=objective,
+                         X_pending=X_pending, prune_baseline=prune_baseline)
+        self.count = 0
+        
+        
+    @concatenate_pending_points
+    @t_batch_mode_transform()
+    def forward(self, X: Tensor) -> Tensor:
+        r"""Evaluate qNoisyExpectedImprovement on the candidate set `X`.
+
+        Args:
+            X: A `batch_shape x q x d`-dim Tensor of t-batches with `q` `d`-dim design
+                points each.
+
+        Returns:
+            A `batch_shape'`-dim Tensor of Noisy Expected Improvement values at the
+            given design points `X`, where `batch_shape'` is the broadcasted batch shape
+            of model and input `X`.
+        """
+        self.count += 1
+        q = X.shape[-2]
+        match_batch_shape(self.X_baseline, X)
+        X_full = torch.cat([X, match_batch_shape(self.X_baseline, X)], dim=-2)        
+        self.posterior = self.model.posterior(X_full)
+        samples = self.sampler(self.posterior)
+        obj = self.objective(samples)
+        diffs = obj[:, :, :q].max(dim=-1)[0] - obj[:, :, q:].max(dim=-1)[0]
+        return diffs.clamp_min(0).mean(dim=0)
+
+
 # Find mean and variance of Gaussian Process
 # TODO: Change this to a Noisy Constrained Optimizer, and acquisition
 #       function can be changed from input
 class NEIOptimizer(Optimizer):
     r"""A Bayesian Optimizer that uses Noisy Expected Improvement
     as the acquisition function.
     
@@ -44,27 +86,29 @@
     MC_SAMPLES = 500
     DTYPE = torch.double
     
     def __init__(
             self, 
             file_name: str,
             bounds: Dict[str, Tuple[float, float]],
+            initial_candidates: Optional[list] = [],
             device: Optional[str] = "cpu",
             seed: Optional[int] = random.randint(1, 100000),
         ) -> None:
         r"""Constructor for  Bayesian optimizer that use Noisy Expected Improvement
         as the acquisition function. 
         
         :param device:              Generate candidates on the chosen device.
         :param bounds:              Boundaries to the search space.
         """
         super().__init__(file_name, bounds=bounds, seed=seed)
         self.device = device
         self.current_model = None
         self.num_constraints = None
+        self.initial_candidates = initial_candidates
         
     def _generate_random_candidate(self) -> Dict[str, Any]:
         r"""Randomly generate a candidate in the known boundaries. Is uniform random."""
         candidate = {}
         for bound_key in self.bounds:
             min_bound, max_bound = self.bounds[bound_key]
             # Uniformly choose a number from the designated range
@@ -84,15 +128,15 @@
         if self.num_constraints == None:
             self.num_constraints = len(self.observations[-1]["constraints"])
             
         # Group candidates, objectives, variances and constraints from observations 
         train_x, train_obj, train_var= [], [], []
         train_cons = [[] for i in range(self.num_constraints)]
         for o in self.observations:
-            train_x.append(list(o["candidate"].values()))
+            train_x.append(list(o["candidate"].values())[:-1]) # Last key of candidate is id
             train_obj.append(o["objective"][0])
             train_var.append(o["objective"][1])
             for i in range(self.num_constraints):
                 train_cons[i].append(o["constraints"][i])
                 
         # Put into torch tensor 
         train_x = torch.tensor(train_x, device=self.device, dtype=NEIOptimizer.DTYPE)
@@ -138,41 +182,43 @@
 
         # define a feasibility-weighted objective for optimization
         constrained_obj = None
         if self.num_constraints > 0:
             constraint_functions = []
             for i in range(self.num_constraints):
                 constraint_idx = i + 1
-                print("Constraint index: ", constraint_idx)
                 constraint_functions.append(lambda Z: Z[..., constraint_idx])
             constrained_obj = ConstrainedMCObjective(
                 objective=lambda Z: Z[..., 0],
                 constraints=constraint_functions
             )
-        self.qNEI = qNoisyExpectedImprovement(
+        self.qNEI = qNEIModified(
             model=self.current_model, 
-            X_baseline=self.observation_list_to_tensor("candidate"),
+            X_baseline=self.observation_to_candidate_tensor(),
             X_pending=self.pending_candidate_list_to_tensor(),
             sampler=qmc_sampler,
             objective=constrained_obj
         )
         
     def generate_candidate(self) -> Dict[str, Any]:
         r"""Draw the best candidate to evaluate based on known observations.
         
         :param is_random: Set to True if want to generate randomly
         """
         
-        if len(self.observations) == 0:
+        if len(self.initial_candidates) > 0:
+            candidate = self.initial_candidates.pop()
+            candidate = dict(sorted(candidate.items()))
+            return candidate
+        elif len(self.observations) == 0 and len(self.initial_candidates) == 0:
             # If no previous observation or if initial candidate(s) are specified (may be more than one)
             # Then use initial candidate(s), If no initial candidate available, generate randomly.
             print("Generating initial candidate(s)")
             return self._generate_random_candidate()
 
-        print(f"Optimizer received \n{self.observations[-1]}")
         mll, model = self._initialize_model()
         fit_gpytorch_model(mll)
         self._initialize_acqf()
 
         # Turn dictionary bounds into torch bounds
         lower_bounds = [bound[0] for bound in self.bounds.values()]
         upper_bounds = [bound[1] for bound in self.bounds.values()]
@@ -196,25 +242,22 @@
             raise Exception("NanError again. There's no way to solve it yet !!!")
 
         # Put parameters together
         candidate = {}
         for i, key in enumerate(self.get_labels()):
             candidate[key] = torch_candidate.cpu().numpy()[0][i]
 
-        print(f"Sending candidate: {candidate}\n"
-              f"Number of observations: {len(self.observations)}")
-
         return candidate
         
-    def observation_list_to_tensor(self, key):
-        return torch.tensor([list(o[key].values()) for o in self.observations], 
+    def observation_to_candidate_tensor(self):
+        return torch.tensor([list(o["candidate"].values())[:-1] for o in self.observations], 
                      device=self.device, dtype=NEIOptimizer.DTYPE)
 
     def pending_candidate_list_to_tensor(self):
-        t = torch.tensor([list(c.values()) for c in self.pending_candidates], 
+        t = torch.tensor([list(c.values())[:-1] for c in self.pending_candidates], 
                      device=self.device, dtype=NEIOptimizer.DTYPE)
         if t.shape[-1] == 0:
             return None
         print("Pending shape:", t.shape)
         return t
```

### Comparing `dopt-0.0.3.9/dopt/optimizers/optimizer.py` & `dopt-0.0.5.11/dopt/optimizers/optimizer.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,27 +19,28 @@
 class Optimizer(ABC):
     r"""Abstract base class for hyperparameter optimizers.
     Optimizer distributes candidates (sets of hyperparameters)
     to Trainers, each of which is on a different machine to 
     compute the objective function in parallel.
     """
     MAX_OBSERVATIONS = 500
+    HEADER_REMOVE_CANDIDATE = "Remove: "
 
     def __init__(self, 
-                 file_name: str,
+                 filename: str,
                  bounds: Dict[str, Tuple[float, float]],
                  seed: Optional[int] = random.randint(1, 100000)) -> None:
         r""" Constructor for Optimizer base class.
         
-        :param file_name:   Name of the file
+        :param filename:   Name of the file
                             that stores observations
         :param bounds:      Boundaries to the search space
         :param seed:        To ensure reproducibility
         """
-        self.file_name = file_name
+        self.filename = filename
         self.bounds = dict(sorted(bounds.items()))
         
         # Ensure reproducibility
         random.seed(seed)
         torch.manual_seed(generate_seed())
         np.random.seed(generate_seed())
         
@@ -70,73 +71,104 @@
     
     def get_labels(self):
         return self.bounds.keys()
     
     def _load_observations(self):
         r"""Load observations from existing file. If file doesn't
         exist, create a new file"""
-        if path.exists(self.file_name):
+        if path.exists(self.filename):
             # Load observations
-            with open(self.file_name, "r") as f:
+            with open(self.filename, "r") as f:
                 for line in f.readlines():
                     self.observations.append(json.loads(line))
         else:
             # Create a new file
-            with open(self.file_name, "w") as f:
+            with open(self.filename, "w") as f:
                 pass
     
     def _save_observation(self, observation):
         r"""Save ONE acquired observation into a storing file"""
-        with open(self.file_name, "a") as f:
+        with open(self.filename, "a") as f:
             f.write(json.dumps(observation, indent=None) + "\n")
             
     def remove_pending_candidate(self, observation):
         """Candidates from returning observations, successful or failed,
         are to be removed from the pending_candidates list
         
         :param observation: A single observation
         """
         candidate_to_remove = observation["candidate"]
+        if candidate_to_remove not in self.pending_candidates:
+            raise Exception("Candidate not found in pending candidates!")
         self.pending_candidates = [candidate 
                                    for candidate in self.pending_candidates
                                    if candidate != candidate_to_remove]
 
-    def run(self, conn) -> None:
+    def run(self, conn, logger, lock) -> None:
         """Optimization loop. 
         Generate candidate to send to Server, then receive further
         candidate(s) from Server, and then generate, and so
         on."""
         self._set_server_connection(conn)
         while self.is_running():
             try:
                 responses = self.server_conn.recv()
-                print("Optimizer received:", responses)
+                with lock:
+                    logger.debug(f"Optimizer received: {responses}")
             except EOFError:
                 # When the other end is closed
-                print("Exitting Optimizer")
+                with lock:
+                    logger.debug("Exitting Optimizer")
                 return
             
-            # Handle the server's response
-            for response in responses.split("\n")[:-1]:                
-                if response.strip() == "{}":
+            # Handle the server's response(s)
+            for response in responses.split("\n")[:-1]:    
+                response = response.strip()
+                if response == "{}":
+                    pass
+                elif Optimizer.HEADER_REMOVE_CANDIDATE in response:
+                    # Remove pending candidate
+                    candidate = json.loads(response[len(Optimizer.HEADER_REMOVE_CANDIDATE):].strip())
+                    self.remove_pending_candidate({"candidate": candidate})
+                    with lock:
+                        logger.debug(f"Removed candidate: {candidate}")
                     continue
-                    
-                observation = json.loads(response)
-                if observation["contention_failure"] == False:
-                    self.observations.append(observation)
-                    self._save_observation(observation) 
-                self.remove_pending_candidate(observation) 
+                else:
+                    observation = json.loads(response)
+                    if observation["contention_failure"] == False:
+                        self.observations.append(observation)
+                        self._save_observation(observation) 
+                    self.remove_pending_candidate(observation) 
                 
-             # Find one potential candidate to try next based on the info
-            candidate: Dict[str, Any] = self.generate_candidate()
-            self.pending_candidates.append(candidate)
-            
-            reply = json.dumps({"candidate": candidate})
-            self.server_conn.send(reply)                
-            print("Optimizer sent:", reply)
+                 # Find one potential candidate to try next based on the info
+                candidate: Dict[str, Any] = self.generate_candidate()
+                candidate["id"] = self.generate_id()
+                self.pending_candidates.append(candidate)
+
+                reply = json.dumps({"candidate": candidate})
+                self.server_conn.send(reply)                # <---- This
+                with lock:
+                    logger.debug(f"Optimizer sent: {reply}")
+                
+            with lock:
+                logger.debug(f"Number of observations: {len(self.observations)}")
+                logger.debug(f"Number of pending candidates: {len(self.pending_candidates)}")
+                logger.debug(f"Pending candidates: {json.dumps(self.pending_candidates)}")
+                logger.warning(f"Pending candidates: {json.dumps(self.pending_candidates)}")
+          
+            
+    def generate_id(self):
+        current_ids = [o["candidate"]["id"] for o in self.observations]
+        current_ids += [candidate["id"] for candidate in self.pending_candidates]
+        i = 1
+        while i <= len(current_ids) + 1:
+            if i not in current_ids:
+                break
+            i += 1    
+        return i
         
     @abstractmethod
     def generate_candidate(self) \
             -> Dict[str, Any]:
         r"""Draw the best candidate to evaluate based on known observations."""
         raise NotImplementedError
```

### Comparing `dopt-0.0.3.9/dopt/utils/general_utils.py` & `dopt-0.0.5.11/dopt/utils/general_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 r"""
 Helper functions
 """
 import sys
 import time
+from datetime import datetime
 from contextlib import contextmanager
 import torch
 import random
 import subprocess
 
 @contextmanager
 def add_prefix_to_print(prefix): 
@@ -36,15 +37,14 @@
     return model(torch.rand(*(image_dim))).data.shape
 
 def generate_seed():
     return random.randint(1, 100000)
 
 def get_gpu_info():
     sp = subprocess.Popen(['nvidia-smi', '-q'], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-    
     out_str = sp.communicate()
     out_list = out_str[0].decode("utf8").split('\n')
     out_dict = {}
     for item in out_list:
         try:
             key, val = item.split(':')
             key, val = key.strip(), val.strip()
@@ -54,32 +54,34 @@
                 out_dict[key] = [val]
         except:
             pass
     return out_dict
 
 def get_general_info(pid):
     sp = subprocess.Popen(["ps", "-up", str(pid)], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-
     out_str = sp.communicate()
     outputs = out_str[0].decode("utf8").split("\n")
     labels = outputs[0].split()
     info = outputs[1].split()
     if len(info) > len(labels): # Join commands that were splitted
         last_label_idx = len(labels)-1 
         info[last_label_idx] = " ".join(info[last_label_idx:])
         info = info[:len(labels)]
     process_info = {labels[i]: info[i] for i in range(len(info))}
     return process_info
 
 def get_all_gpu_processes_info():
     processes = {}
     out_dict = get_gpu_info()
-    max_gpu = int(out_dict["Total"][0].split()[0])
-    
+    if "Total" in out_dict:    
+        max_gpu = int(out_dict["Total"][0].split()[0])
+    else:
+        max_gpu = -1
     processes["max_gpu"] = max_gpu
+    processes["time_updated"] = datetime.now().strftime("%m/%d/%Y-%H:%M:%S")
     for i, process_id in enumerate(out_dict["Process ID"]):
         process_info = get_general_info(process_id)
         processes[process_id] = {
             "name": out_dict["Name"][i],
             "user": process_info["USER"],
             "gpu_used": int(out_dict["Used GPU Memory"][i].split()[0]),
             "%cpu_used": float(process_info["%CPU"]),
```

### Comparing `dopt-0.0.3.9/dopt/utils/ssh_utils.py` & `dopt-0.0.5.11/dopt/utils/ssh_utils.py`

 * *Files identical despite different names*

### Comparing `dopt-0.0.3.9/dopt.egg-info/PKG-INFO` & `dopt-0.0.5.11/dopt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dopt
-Version: 0.0.3.9
+Version: 0.0.5.11
 Summary: Distributed Optimizer
-Home-page: https://github.com/pypa/sampleproject
+Home-page: https://gitlab.com/tungtran99/distributed-optimizer
 Author: Tung Tran
 Author-email: sontungtran99@gmail.com
 License: UNKNOWN
 Description: 
         ### How to use
         We'll be running `distributed_optimizer.py` to start the optimization.
           
@@ -36,9 +36,9 @@
          - Step 2: Make sure the appropriate environment can be chosen through ssh tunneling. Try: `ssh [name]@[hostmachine] [YOUR COMMANDS]`
          - Step 3: Add the commands to the `COMMANDS` dictionary.
          - Step 4: Make sure you have a copy of the `distributed_optimizer.py` and related files on all of the machines you intend to use
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `dopt-0.0.3.9/tests/test_optimizer.py` & `dopt-0.0.5.11/tests/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `dopt-0.0.3.9/tests/test_trainer.py` & `dopt-0.0.5.11/tests/test_trainer.py`

 * *Files identical despite different names*

