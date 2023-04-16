# Comparing `tmp/optiframe-0.2.0.tar.gz` & `tmp/optiframe-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optiframe-0.2.0.tar", max compression
+gzip compressed data, was "optiframe-0.3.0.tar", max compression
```

## Comparing `optiframe-0.2.0.tar` & `optiframe-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     1069 2023-03-29 14:01:26.561203 optiframe-0.2.0/LICENSE
--rw-r--r--   0        0        0     2109 2023-04-07 17:24:23.751578 optiframe-0.2.0/README.md
--rw-r--r--   0        0        0      297 2023-04-06 15:54:45.897421 optiframe-0.2.0/optiframe/__init__.py
--rw-r--r--   0        0        0      272 2023-03-29 14:01:26.561203 optiframe-0.2.0/optiframe/framework/__init__.py
--rw-r--r--   0        0        0     1940 2023-04-06 15:54:45.897421 optiframe-0.2.0/optiframe/framework/default_tasks.py
--rw-r--r--   0        0        0      147 2023-03-29 14:01:26.561203 optiframe-0.2.0/optiframe/framework/errors.py
--rw-r--r--   0        0        0     4425 2023-04-06 15:54:45.897421 optiframe-0.2.0/optiframe/framework/optimizer.py
--rw-r--r--   0        0        0      998 2023-04-06 15:54:45.897421 optiframe-0.2.0/optiframe/framework/tasks.py
--rw-r--r--   0        0        0        0 2023-03-29 14:01:26.561203 optiframe-0.2.0/optiframe/py.typed
--rw-r--r--   0        0        0      175 2023-03-29 14:01:26.561203 optiframe-0.2.0/optiframe/workflow_engine/__init__.py
--rw-r--r--   0        0        0      453 2023-03-29 14:01:26.561203 optiframe-0.2.0/optiframe/workflow_engine/errors.py
--rw-r--r--   0        0        0     6179 2023-03-29 14:01:26.561203 optiframe-0.2.0/optiframe/workflow_engine/step.py
--rw-r--r--   0        0        0      690 2023-03-29 14:01:26.561203 optiframe-0.2.0/optiframe/workflow_engine/task.py
--rw-r--r--   0        0        0     1458 2023-03-29 14:01:26.561203 optiframe-0.2.0/optiframe/workflow_engine/workflow.py
--rw-r--r--   0        0        0      721 2023-04-07 17:25:40.463742 optiframe-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2676 1970-01-01 00:00:00.000000 optiframe-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-12 14:09:36.025204 optiframe-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2109 2023-04-16 17:31:05.640958 optiframe-0.3.0/README.md
+-rw-r--r--   0        0        0      385 2023-04-16 20:21:48.040887 optiframe-0.3.0/optiframe/__init__.py
+-rw-r--r--   0        0        0      414 2023-04-16 20:21:48.040887 optiframe-0.3.0/optiframe/framework/__init__.py
+-rw-r--r--   0        0        0     2561 2023-04-16 20:21:48.040887 optiframe-0.3.0/optiframe/framework/default_tasks.py
+-rw-r--r--   0        0        0      267 2023-04-16 20:21:48.040887 optiframe-0.3.0/optiframe/framework/errors.py
+-rw-r--r--   0        0        0      527 2023-04-16 20:21:48.040887 optiframe-0.3.0/optiframe/framework/metrics.py
+-rw-r--r--   0        0        0     8788 2023-04-16 20:21:48.040887 optiframe-0.3.0/optiframe/framework/optimizer.py
+-rw-r--r--   0        0        0     1036 2023-04-16 20:21:48.040887 optiframe-0.3.0/optiframe/framework/tasks.py
+-rw-r--r--   0        0        0        0 2023-04-01 14:13:27.609904 optiframe-0.3.0/optiframe/py.typed
+-rw-r--r--   0        0        0      306 2023-04-16 20:21:48.040887 optiframe-0.3.0/optiframe/workflow_engine/__init__.py
+-rw-r--r--   0        0        0      495 2023-04-16 20:21:48.040887 optiframe-0.3.0/optiframe/workflow_engine/errors.py
+-rw-r--r--   0        0        0     6858 2023-04-16 20:21:48.040887 optiframe-0.3.0/optiframe/workflow_engine/step.py
+-rw-r--r--   0        0        0     1054 2023-04-16 20:21:48.044887 optiframe-0.3.0/optiframe/workflow_engine/task.py
+-rw-r--r--   0        0        0     2283 2023-04-16 20:21:48.044887 optiframe-0.3.0/optiframe/workflow_engine/workflow.py
+-rw-r--r--   0        0        0     1087 2023-04-16 20:22:42.018131 optiframe-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2997 1970-01-01 00:00:00.000000 optiframe-0.3.0/setup.py
+-rw-r--r--   0        0        0     2676 1970-01-01 00:00:00.000000 optiframe-0.3.0/PKG-INFO
```

### Comparing `optiframe-0.2.0/LICENSE` & `optiframe-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `optiframe-0.2.0/README.md` & `optiframe-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `optiframe-0.2.0/optiframe/framework/default_tasks.py` & `optiframe-0.3.0/optiframe/framework/default_tasks.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,70 @@
+"""The default tasks of the optimization framework.
+
+These tasks are added to the steps automatically when constructing the optimizer.
+"""
 from dataclasses import dataclass
 from typing import Any, Optional
 
 from pulp import LpProblem, LpMinimize, LpAffineExpression, LpStatus, LpMaximize
 
 from optiframe.framework.errors import InfeasibleError
 from optiframe.framework.tasks import BuildMipTask, ExtractSolutionTask
 from optiframe.workflow_engine import Task
 
 
 @dataclass
 class ProblemSettings:
+    """The settings to configure the MIP."""
+
     name: str
     sense: LpMinimize | LpMaximize
 
 
 class CreateProblemTask(BuildMipTask[LpProblem]):
+    """A task to initialize the MIP object."""
+
     problem_settings: ProblemSettings
 
     def __init__(self, problem_settings: ProblemSettings):
         self.problem_settings = problem_settings
 
     def execute(self) -> LpProblem:
+        """Create the `LpProblem` instance to make it available to other tasks."""
         problem = LpProblem(self.problem_settings.name, self.problem_settings.sense)
         # Initialize the objective to an empty expression
         problem.setObjective(LpAffineExpression())
         return problem
 
 
 @dataclass
 class SolveSettings:
+    """The settings to configure the solver."""
+
     # The PuLP solver object to use for the optimization
     solver: Optional[Any]
 
 
 class SolveTask(Task[None]):
+    """The task to execute the solver on the constructed MIP."""
+
     problem: LpProblem
     objective: LpAffineExpression
     solve_settings: SolveSettings
 
     def __init__(
         self,
         problem: LpProblem,
         solve_settings: SolveSettings,
     ):
         self.problem = problem
         self.solve_settings = solve_settings
 
     def execute(self) -> None:
+        """Execute the solver on the constructed MIP."""
         # Solve the problem
         status_code = self.problem.solve(solver=self.solve_settings.solver)
         status = LpStatus[status_code]
 
         if status != "Optimal":
             raise InfeasibleError()
 
@@ -59,16 +73,19 @@
 class SolutionObjValue:
     """The objective value of the solution."""
 
     objective_value: float
 
 
 class ExtractSolutionObjValueTask(ExtractSolutionTask[SolutionObjValue]):
+    """A task to extract the objective value from the solved MIP."""
+
     problem: LpProblem
 
     def __init__(self, problem: LpProblem):
         self.problem = problem
 
     def execute(self) -> SolutionObjValue:
+        """Extract the objective value from the solved MIP."""
         cost = self.problem.objective.value()
 
         return SolutionObjValue(cost)
```

### Comparing `optiframe-0.2.0/optiframe/framework/tasks.py` & `optiframe-0.3.0/optiframe/workflow_engine/task.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,28 @@
+"""A task in the workflow which executes a specific action."""
 import abc
 from typing import TypeVar, Generic
 
-from optiframe import Task
-
 T = TypeVar("T")
 
 
-class ValidateTask(Task[None], abc.ABC):
-    """
-    A task to validate the data describing the problem instance.
-
-    The `execute` method should raise an `AssertionError` if the data is not valid.
-    """
-
-    pass
+class Task(abc.ABC, Generic[T]):
+    """A task in the workflow which executes a specific action.
 
+    The task can generate data and return it from the `execute` function.
+    This data will be made available to the other tasks of the workflow.
 
-class PreProcessingTask(Task[T], abc.ABC, Generic[T]):
+    The task can also depend on data by other tasks by specifying dependencies in the constructor.
+    The type annotation of the constructor parameters determine which dependency will be injected.
+    If the data is generated by a task in the same step, the task will be executed before this one.
     """
-    A task to pre-process the data to make the model smaller or more efficient.
 
-    This can reduce the the total time needed to solve the problem.
-    """
-
-    pass
+    @abc.abstractmethod
+    def execute(self) -> T:
+        """Execute the action of this task.
 
+        This method is called once all the dependencies of the task have been gathered.
+        It can access the data of the dependencies through the `self` parameter.
 
-class BuildMipTask(Task[T], abc.ABC, Generic[T]):
-    """
-    A task to construct (or modify) the mixed integer program.
-
-    This is the central of the optimization package as it modifies the final result.
-    """
-
-    pass
-
-
-class ExtractSolutionTask(Task[T], abc.ABC):
-    """
-    A task to extract the relevant information from the solution of the MIP.
-
-    In this task, variable values can be selected, discarded or aggregated.
-    """
-
-    pass
+        The data that is returned from this method can be used by other tasks.
+        """
+        pass
```

### Comparing `optiframe-0.2.0/optiframe/workflow_engine/step.py` & `optiframe-0.3.0/optiframe/workflow_engine/step.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""The steps of a workflow.
+
+Steps are executed sequentially in the optimization process.
+Each step can contain multiple tasks, which are ordered based on their dependencies.
+"""
+
 from __future__ import annotations
 
 import inspect
 import logging
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Self, Type, Any
@@ -11,75 +17,84 @@
 
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class TaskDependency:
+    """A dependency required by a task, as defined in the `.__init__` method."""
+
     param: str
     annotation: Any
 
     def __repr__(self) -> str:
+        """Get the string representation of a task dependency."""
         return f"{self.param}: {self.annotation.__name__}"
 
     def __str__(self) -> str:
+        """Get a human-readable string of a task dependency."""
         return f"{self.param}: {self.annotation.__name__}"
 
 
 # Data which can be injected into a task.
 # The keys should be class objects which define the type of the data.
 StepData = dict[Any, Any]
 
 
 class Step:
-    """
-    One step in the workflow process.
+    """One step in the workflow process.
 
     Each step is composed of multiple tasks which will be executed within this step.
     Multiple steps are executed sequentially.
     """
 
     name: str
     tasks: list[Type[Task[Any]]]
 
     def __init__(self, name: str):
         self.name = name
         self.tasks = []
 
     def add_task(self, task: Type[Task[Any]]) -> Self:
-        """
-        Register a task to run in this step.
+        """Register a task to run in this step.
 
         :param task: The task to register.
         :return: The same step, to use for function chaining.
         """
         self.tasks.append(task)
         return self
 
     def initialize(self, step_data: StepData) -> InitializedStep:
+        """Initialize a step with data from previous steps.
+
+        This allows data to be passed between steps and be added from the user.
+        """
         return InitializedStep(self, step_data)
 
 
 class InitializedStep:
+    """A step that has been initialized with data."""
+
     step: Step
     step_data: StepData
 
     def __init__(self, step: Step, step_data: StepData):
         self.step = step
         self.step_data = step_data
 
     def name(self) -> str:
+        """Get the name of the step."""
         return self.step.name
 
     def tasks(self) -> list[Type[Task[Any]]]:
+        """Get the tasks that have to be executed during this step."""
         return self.step.tasks
 
     def execute(self) -> StepData:
-        """
-        Execute the step by executing the action of all tasks within it.
+        """Execute the step by executing the action of all tasks within it.
 
         The dependencies of each task are injected automatically.
 
         :raises InjectionError: If the `__init__` or `action` methods are missing type annotations.
         This is necessary to inject the dependencies automatically.
         :raises ScheduleError: If the tasks can't be scheduled,
         e.g. due to circular dependencies.
@@ -145,16 +160,15 @@
         duration = datetime.now() - start_time
 
         logger.info(f"Finished step {self.name()} in {duration.total_seconds():.2f}s.")
 
         return self.step_data
 
     def _task_dependencies(self) -> dict[Type[Task[Any]], list[TaskDependency]]:
-        """
-        Determine which task depends on which type of data.
+        """Determine which task depends on which type of data.
 
         :return: For each task, a list of its dependencies.
         """
         dependencies: dict[Type[Task[Any]], list[TaskDependency]] = dict()
 
         # Collect the dependencies for each task
         for task in self.tasks():
```

### Comparing `optiframe-0.2.0/optiframe/workflow_engine/workflow.py` & `optiframe-0.3.0/optiframe/workflow_engine/workflow.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,75 @@
+"""Complete workflows, composed of steps which are composed of tasks."""
 from __future__ import annotations
 
 from typing import Self, Any
 
 from .step import Step, StepData
 
 
 class Workflow:
-    """
-    A complete workflow.
+    """A complete workflow.
 
     The workflow is composed of steps, which are executed sequentially.
     Each step is composed of tasks, which can depend on each other.
     """
 
     steps: list[Step]
 
     def __init__(self) -> None:
         self.steps = list()
 
     def add_step(self, step: Step) -> Self:
+        """Add a step to the workflow.
+
+        The order in which the steps are added determines the order in which they are executed.
+        """
         self.steps.append(step)
         return self
 
     def initialize(self, *args: Any) -> InitializedWorkflow:
+        """Initialize the workflow with data.
+
+        The data that needs to be added here is the data required by the tasks
+        that is not generated by any other tasks.
+        """
         step_data = {type(data): data for data in args if data is not None}
 
         return InitializedWorkflow(self, step_data)
 
 
 class InitializedWorkflow:
+    """A workflow initialized with data."""
+
     workflow: Workflow
     step_data: StepData
 
     def __init__(self, workflow: Workflow, step_data: StepData):
         self.workflow = workflow
         self.step_data = step_data
 
     def add_data(self, data: Any) -> Self:
+        """Add additional data to the model.
+
+        This can be used to add dependencies needed by tasks that can not
+        be provided by other tasks, but is also not available at initialization.
+        """
         data_type = type(data)
         self.step_data[data_type] = data
         return self
 
     def execute_step(self, index: int) -> StepData:
+        """Execute the step at the given index.
+
+        The indexes start at 0, so 0 is the first step.
+        """
         step = self.workflow.steps[index]
         self.step_data = step.initialize(self.step_data).execute()
         return self.step_data
 
     def execute(self) -> StepData:
+        """Execute all steps sequentially."""
         for step in self.workflow.steps:
             # Execute each step sequentially and update the step data
             self.step_data = step.initialize(self.step_data).execute()
 
         return self.step_data
```

### Comparing `optiframe-0.2.0/PKG-INFO` & `optiframe-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optiframe
-Version: 0.2.0
+Version: 0.3.0
 Summary: A modular framework for mixed integer programming.
 Home-page: https://github.com/TimJentzsch/optiframe
 License: MIT
 Author: Tim Jentzsch
 Author-email: optiframe.projects@timjen.net
 Requires-Python: >=3.11.0rc1
 Classifier: License :: OSI Approved :: MIT License
```

