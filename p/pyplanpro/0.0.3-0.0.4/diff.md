# Comparing `tmp/pyplanpro-0.0.3.tar.gz` & `tmp/pyplanpro-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyplanpro-0.0.3.tar", last modified: Wed Apr 26 06:19:49 2023, max compression
+gzip compressed data, was "pyplanpro-0.0.4.tar", last modified: Fri Apr 28 07:53:27 2023, max compression
```

## Comparing `pyplanpro-0.0.3.tar` & `pyplanpro-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:49.977352 pyplanpro-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-26 06:19:36.000000 pyplanpro-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-26 06:19:49.977352 pyplanpro-0.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:49.973352 pyplanpro-0.0.3/PyPlanPro/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-26 06:19:36.000000 pyplanpro-0.0.3/PyPlanPro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:49.973352 pyplanpro-0.0.3/PyPlanPro/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:36.000000 pyplanpro-0.0.3/PyPlanPro/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-26 06:19:36.000000 pyplanpro-0.0.3/PyPlanPro/models/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-26 06:19:36.000000 pyplanpro-0.0.3/PyPlanPro/models/resource_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-26 06:19:36.000000 pyplanpro-0.0.3/PyPlanPro/models/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:49.973352 pyplanpro-0.0.3/PyPlanPro/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:36.000000 pyplanpro-0.0.3/PyPlanPro/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-04-26 06:19:36.000000 pyplanpro-0.0.3/PyPlanPro/scheduler/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-26 06:19:36.000000 pyplanpro-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:49.977352 pyplanpro-0.0.3/pyplanpro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-26 06:19:49.000000 pyplanpro-0.0.3/pyplanpro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-26 06:19:49.000000 pyplanpro-0.0.3/pyplanpro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 06:19:49.000000 pyplanpro-0.0.3/pyplanpro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 06:19:49.000000 pyplanpro-0.0.3/pyplanpro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 06:19:49.000000 pyplanpro-0.0.3/pyplanpro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 06:19:49.977352 pyplanpro-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-26 06:19:36.000000 pyplanpro-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:49.977352 pyplanpro-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:36.000000 pyplanpro-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:36.000000 pyplanpro-0.0.3/tests/test_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:53:27.014474 pyplanpro-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-28 07:53:27.014474 pyplanpro-0.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:53:27.010474 pyplanpro-0.0.4/PyPlanPro/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/PyPlanPro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:53:27.010474 pyplanpro-0.0.4/PyPlanPro/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/PyPlanPro/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/PyPlanPro/models/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/PyPlanPro/models/resource_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/PyPlanPro/models/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:53:27.010474 pyplanpro-0.0.4/PyPlanPro/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/PyPlanPro/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/PyPlanPro/scheduler/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/PyPlanPro/scheduler/heuristic_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/PyPlanPro/scheduler/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:53:27.014474 pyplanpro-0.0.4/pyplanpro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-28 07:53:26.000000 pyplanpro-0.0.4/pyplanpro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-28 07:53:26.000000 pyplanpro-0.0.4/pyplanpro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 07:53:26.000000 pyplanpro-0.0.4/pyplanpro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 07:53:26.000000 pyplanpro-0.0.4/pyplanpro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 07:53:26.000000 pyplanpro-0.0.4/pyplanpro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 07:53:27.014474 pyplanpro-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:53:27.014474 pyplanpro-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:53:27.014474 pyplanpro-0.0.4/tests/stress/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/tests/stress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/tests/stress/test_stress_scheduler.py
```

### Comparing `pyplanpro-0.0.3/LICENSE` & `pyplanpro-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyplanpro-0.0.3/PKG-INFO` & `pyplanpro-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplanpro
-Version: 0.0.3
+Version: 0.0.4
 Summary: Task scheduler for python
 Home-page: https://github.com/Oestergaard-A-S/PyPlanPro
 Author: Jacob Østergaard Nielsen
 Author-email: jaoe@oestergaard-as.dk
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -27,18 +27,23 @@
 Schedule tasks to resources within their respective resource groups, minimizing the makespan
 Output the optimal or feasible schedule if found
 ## Requirements
 To run this program, you need to have the following packages installed:
 
 Python 3.6 or later
 ortools (pip install ortools)
+
+## Installation
+```python
+pip install pyplanpro
+```
 ## Usage
 1. Import the necessary classes and functions:
 ```python
-from scheduler import Resource, ResourceGroup, Task, Scheduler
+from pyplanpro import Resource, ResourceGroup, Task, Scheduler
 ```
 2. Define resources and resource groups:
 ```python
 r1_availability_slots = [
      {"slot_id" : 0, "start":0, "end":4},
      {"slot_id" : 1, "start":5, "end":10}
 ]
@@ -56,15 +61,15 @@
 4. Set the scheduling horizon:
 ```python
 horizon = 50
 ```
 5. Call the Scheduler function with tasks and horizon:
 ```python
 s = Scheduler()
-s.schedule(tasks)
+s.schedule(tasks, horizon= horizon)
 ```
 If a solution is found, the program will print the optimal or feasible schedule with makespan, resource assignments, task start and end times, and durations.
 ```
 Makespan = 8.0
 Assigned to resource 2
 Task (0, 0): starts: 0, end: 8, duration: 8
 ```
```

### Comparing `pyplanpro-0.0.3/PyPlanPro/models/task.py` & `pyplanpro-0.0.4/PyPlanPro/models/task.py`

 * *Files identical despite different names*

### Comparing `pyplanpro-0.0.3/PyPlanPro/scheduler/core.py` & `pyplanpro-0.0.4/PyPlanPro/scheduler/optimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from ortools.sat.python import cp_model
-from ..models.resource import Resource
-from ..models.resource_group import ResourceGroup
-from ..models.task import Task
 import time
 
-class Scheduler:
+class Optimizer:
 
     def __init__(
             self, 
             tasks, 
             horizon,
             time_limit=None,
             solution_limit=None,
@@ -60,72 +57,72 @@
             # set task_start and end variables
             task_start = model.NewIntVar(0, horizon, f'task_start_{task.id}')
             task_end = model.NewIntVar(0, horizon, f'task_end_{task.id}')
             task_vars[task.id]["start"] = task_start
             task_vars[task.id]["end"] = task_end
             for resource in task.get_resources():
                 subtask_durations = []
-                for subtask_id, slot in enumerate(resource.availability_slots):
+                for subtask_id, (slot_start, slot_end) in enumerate(resource.availability_slots):
 
                     # create variables
-                    start = model.NewIntVar(slot["start"], slot["end"], f'start_{slot["start"]}')
-                    end = model.NewIntVar(slot["start"], slot["end"], f'end_{slot["end"]}')
-                    duration = model.NewIntVar(0, task_duration, f'duration_{slot["slot_id"]}')
+                    start = model.NewIntVar(slot_start, slot_end, f'start_{slot_start}')
+                    end = model.NewIntVar(slot_start, slot_end, f'end_{slot_end}')
+                    duration = model.NewIntVar(0, slot_end-slot_start, f'duration_{subtask_id}')
                     subtask_durations.append(duration)
-                    interval = model.NewIntervalVar(start, duration, end, f'interval_{task.id, slot["slot_id"]}')
+                    interval = model.NewIntervalVar(start, duration, end, f'interval_{task.id, subtask_id}')
 
                     # Create a BoolVar if duration greater than 0
-                    duration_gt_zero = model.NewBoolVar(f'duration_gt_zero_{task.id}_{slot["slot_id"]}')
+                    duration_gt_zero = model.NewBoolVar(f'duration_gt_zero_{task.id}_{subtask_id}')
                     model.Add(duration > 0).OnlyEnforceIf(duration_gt_zero)
                     model.Add(duration == 0).OnlyEnforceIf(duration_gt_zero.Not())
 
                     # Craete a BoolVar to check if duration equal sum of subtask durations
-                    duration_eq_sum_duration = model.NewBoolVar(f'duration_eq_sum_duration_{task.id}_{slot["slot_id"]}')
+                    duration_eq_sum_duration = model.NewBoolVar(f'duration_eq_sum_duration_{task.id}_{subtask_id}')
                     model.Add(sum(subtask_durations) == duration).OnlyEnforceIf(duration_eq_sum_duration)
                     model.Add(sum(subtask_durations) != duration).OnlyEnforceIf(duration_eq_sum_duration.Not())
     
                     # Craete a BoolVar to check if tasks has ended
-                    has_ended = model.NewBoolVar(f'has_ended{task.id}_{slot["slot_id"]}')
+                    has_ended = model.NewBoolVar(f'has_ended{task.id}_{subtask_id}')
                     model.Add(sum(subtask_durations) >= task_duration).OnlyEnforceIf(has_ended)
                     model.Add(sum(subtask_durations) < task_duration).OnlyEnforceIf(has_ended.Not())
 
                     # Create a BoolVar to check if slot is task start
-                    is_task_start = model.NewBoolVar(f'is_task_start_{task.id}_{slot["slot_id"]}')
+                    is_task_start = model.NewBoolVar(f'is_task_start_{task.id}_{subtask_id}')
                     model.AddBoolAnd([duration_gt_zero, duration_eq_sum_duration]).OnlyEnforceIf(is_task_start)
                     model.AddBoolOr([duration_gt_zero.Not(), duration_eq_sum_duration.Not()]).OnlyEnforceIf(is_task_start.Not())
 
                     # Create a BoolVar to check if task has ended
-                    is_task_end = model.NewBoolVar(f'is_task_end_{task.id}_{slot["slot_id"]}')
+                    is_task_end = model.NewBoolVar(f'is_task_end_{task.id}_{subtask_id}')
                     model.AddBoolAnd([has_ended, duration_gt_zero]).OnlyEnforceIf(is_task_end)
                     model.AddBoolOr([has_ended.Not(), duration_gt_zero.Not()]).OnlyEnforceIf(is_task_end.Not())
 
                     # Ensure is_in_progress is true when subtask_durations is between > 0 and 10
-                    is_in_progress = model.NewBoolVar(f'task_started_{task.id}_{slot["slot_id"]}')
+                    is_in_progress = model.NewBoolVar(f'task_started_{task.id}_{subtask_id}')
                     model.Add(sum(subtask_durations) > 0).OnlyEnforceIf(is_in_progress)
                     model.Add(sum(subtask_durations) == 0).OnlyEnforceIf(is_in_progress.Not())
                     
                     # Ensure subtasks are continuous 
                     # if task is in progress it should fill the whole slot
-                    model.Add(start == slot["start"]).OnlyEnforceIf((is_in_progress, has_ended.Not(), is_task_start.Not()))
-                    model.Add(end == slot["end"]).OnlyEnforceIf((is_in_progress, has_ended.Not(), is_task_start.Not()))
+                    model.Add(start == slot_start).OnlyEnforceIf((is_in_progress, has_ended.Not(), is_task_start.Not()))
+                    model.Add(end == slot_end).OnlyEnforceIf((is_in_progress, has_ended.Not(), is_task_start.Not()))
 
                     # if task is starting but not ending
-                    model.Add(end == slot["end"]).OnlyEnforceIf((is_task_start, is_task_end.Not()))
+                    model.Add(end == slot_end).OnlyEnforceIf((is_task_start, is_task_end.Not()))
 
                     # if task is ending but not starting
-                    model.Add(start == slot["start"]).OnlyEnforceIf((is_task_end,is_task_start.Not()))        
+                    model.Add(start == slot_start).OnlyEnforceIf((is_task_end,is_task_start.Not()))        
 
                     # set task_stat and task_end
                     model.Add(task_start == start).OnlyEnforceIf(is_task_start).OnlyEnforceIf(resource_bools[task.id,resource.id])       
                     model.Add(task_end == end).OnlyEnforceIf(is_task_end).OnlyEnforceIf(resource_bools[task.id,resource.id])
 
                     # Add the subtask to the list
                     subtask_vars[task.id,resource.id].append({
                         "subtask_id" : subtask_id,
-                        "slot_id": slot["slot_id"],
+                        "slot_id": subtask_id,
                         "start" : start,
                         "duration" : duration,
                         "end" : end,
                         "interval" : interval,
                         "is_task_start" : is_task_start,
                         "is_in_progress" : is_in_progress,
                         "is_task_end" : is_task_end,
@@ -171,15 +168,15 @@
         obj_var = model.NewIntVar(0, horizon, 'makespan')
         model.AddMaxEquality(obj_var, optional_ends)
         model.Minimize(obj_var)
         
         # Create a solver and solve the model
         solver = cp_model.CpSolver()
 
-        solution_printer = VarArraySolutionPrinterWithLimit([obj_var], self.solution_limit)
+        solution_printer = self.VarArraySolutionPrinterWithLimit([obj_var], self.solution_limit)
 
         # Set solver parameters if provided
         if self.time_limit is not None:
             solver.parameters.max_time_in_seconds = self.time_limit
 
         if self.num_search_workers is not None:
             solver.parameters.num_search_workers = self.num_search_workers
@@ -217,28 +214,28 @@
                                     f"duration: {solver.Value(subtask['duration'])}, "
                                     f"bools: {[solver.Value(subtask[field]) for field in ['is_task_start', 'is_in_progress', 'is_task_end', 'duration_gt_zero']]}"
                                     )
                 
         else:
             print("No solution found.")
     
-class VarArraySolutionPrinterWithLimit(cp_model.CpSolverSolutionCallback):
-    """Print intermediate solutions."""
+    class VarArraySolutionPrinterWithLimit(cp_model.CpSolverSolutionCallback):
+        """Print intermediate solutions."""
 
-    def __init__(self, variables, limit=None):
-        cp_model.CpSolverSolutionCallback.__init__(self)
-        self.__variables = variables
-        self.__solution_count = 0
-        self.__solution_limit = limit
-
-    def on_solution_callback(self):
-        self.__solution_count += 1
-        for v in self.__variables:
-            
-            print(f"[INFO] Solution {self.__solution_count}:", '%s=%i' % (v, self.Value(v)), end=' ')
-        if self.__solution_limit: # check if a limit is specified
-            if self.__solution_count >= self.__solution_limit:
-                print('Stop search after %i solutions' % self.__solution_limit)
-                self.StopSearch()
+        def __init__(self, variables, limit=None):
+            cp_model.CpSolverSolutionCallback.__init__(self)
+            self.__variables = variables
+            self.__solution_count = 0
+            self.__solution_limit = limit
+
+        def on_solution_callback(self):
+            self.__solution_count += 1
+            for v in self.__variables:
+                
+                print(f"[INFO] Solution {self.__solution_count}:", '%s=%i' % (v, self.Value(v)))
+            if self.__solution_limit: # check if a limit is specified
+                if self.__solution_count >= self.__solution_limit:
+                    print('Stop search after %i solutions' % self.__solution_limit)
+                    self.StopSearch()
 
-    def solution_count(self):
-        return self.__solution_count
+        def solution_count(self):
+            return self.__solution_count
```

### Comparing `pyplanpro-0.0.3/README.md` & `pyplanpro-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -14,18 +14,23 @@
 Schedule tasks to resources within their respective resource groups, minimizing the makespan
 Output the optimal or feasible schedule if found
 ## Requirements
 To run this program, you need to have the following packages installed:
 
 Python 3.6 or later
 ortools (pip install ortools)
+
+## Installation
+```python
+pip install pyplanpro
+```
 ## Usage
 1. Import the necessary classes and functions:
 ```python
-from scheduler import Resource, ResourceGroup, Task, Scheduler
+from pyplanpro import Resource, ResourceGroup, Task, Scheduler
 ```
 2. Define resources and resource groups:
 ```python
 r1_availability_slots = [
      {"slot_id" : 0, "start":0, "end":4},
      {"slot_id" : 1, "start":5, "end":10}
 ]
@@ -43,15 +48,15 @@
 4. Set the scheduling horizon:
 ```python
 horizon = 50
 ```
 5. Call the Scheduler function with tasks and horizon:
 ```python
 s = Scheduler()
-s.schedule(tasks)
+s.schedule(tasks, horizon= horizon)
 ```
 If a solution is found, the program will print the optimal or feasible schedule with makespan, resource assignments, task start and end times, and durations.
 ```
 Makespan = 8.0
 Assigned to resource 2
 Task (0, 0): starts: 0, end: 8, duration: 8
 ```
```

### Comparing `pyplanpro-0.0.3/pyplanpro.egg-info/PKG-INFO` & `pyplanpro-0.0.4/pyplanpro.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplanpro
-Version: 0.0.3
+Version: 0.0.4
 Summary: Task scheduler for python
 Home-page: https://github.com/Oestergaard-A-S/PyPlanPro
 Author: Jacob Østergaard Nielsen
 Author-email: jaoe@oestergaard-as.dk
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -27,18 +27,23 @@
 Schedule tasks to resources within their respective resource groups, minimizing the makespan
 Output the optimal or feasible schedule if found
 ## Requirements
 To run this program, you need to have the following packages installed:
 
 Python 3.6 or later
 ortools (pip install ortools)
+
+## Installation
+```python
+pip install pyplanpro
+```
 ## Usage
 1. Import the necessary classes and functions:
 ```python
-from scheduler import Resource, ResourceGroup, Task, Scheduler
+from pyplanpro import Resource, ResourceGroup, Task, Scheduler
 ```
 2. Define resources and resource groups:
 ```python
 r1_availability_slots = [
      {"slot_id" : 0, "start":0, "end":4},
      {"slot_id" : 1, "start":5, "end":10}
 ]
@@ -56,15 +61,15 @@
 4. Set the scheduling horizon:
 ```python
 horizon = 50
 ```
 5. Call the Scheduler function with tasks and horizon:
 ```python
 s = Scheduler()
-s.schedule(tasks)
+s.schedule(tasks, horizon= horizon)
 ```
 If a solution is found, the program will print the optimal or feasible schedule with makespan, resource assignments, task start and end times, and durations.
 ```
 Makespan = 8.0
 Assigned to resource 2
 Task (0, 0): starts: 0, end: 8, duration: 8
 ```
```

### Comparing `pyplanpro-0.0.3/setup.py` & `pyplanpro-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         line.strip()
         for line in read(path).split("\n")
         if not line.startswith(('"', "#", "-", "git+"))
     ]
 
 setup(
     name='pyplanpro',
-    version='0.0.3',
+    version='0.0.4',
     author='Jacob Østergaard Nielsen',
     author_email='jaoe@oestergaard-as.dk',
     description='Task scheduler for python',
     long_description=read("README.md"),
     long_description_content_type='text/markdown',
     url='https://github.com/Oestergaard-A-S/PyPlanPro',
     install_requires= read_requirements("requirements.txt"),
```

