# Comparing `tmp/scriptengine-tasks-hpc-0.5.0.tar.gz` & `tmp/scriptengine-tasks-hpc-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scriptengine-tasks-hpc-0.5.0.tar", last modified: Fri Sep 30 09:22:26 2022, max compression
+gzip compressed data, was "scriptengine-tasks-hpc-0.6.0.tar", last modified: Fri Apr 28 10:16:32 2023, max compression
```

## Comparing `scriptengine-tasks-hpc-0.5.0.tar` & `scriptengine-tasks-hpc-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 09:22:26.056716 scriptengine-tasks-hpc-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-09-30 09:22:16.000000 scriptengine-tasks-hpc-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-09-30 09:22:26.056716 scriptengine-tasks-hpc-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-09-30 09:22:16.000000 scriptengine-tasks-hpc-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-30 09:22:16.000000 scriptengine-tasks-hpc-0.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 09:22:26.056716 scriptengine-tasks-hpc-0.5.0/scriptengine_hpc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-30 09:22:16.000000 scriptengine-tasks-hpc-0.5.0/scriptengine_hpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3530 2022-09-30 09:22:16.000000 scriptengine-tasks-hpc-0.5.0/scriptengine_hpc/module.py
--rw-r--r--   0 runner    (1001) docker     (121)     4222 2022-09-30 09:22:16.000000 scriptengine-tasks-hpc-0.5.0/scriptengine_hpc/slurm.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-30 09:22:16.000000 scriptengine-tasks-hpc-0.5.0/scriptengine_hpc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 09:22:26.056716 scriptengine-tasks-hpc-0.5.0/scriptengine_tasks_hpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-09-30 09:22:26.000000 scriptengine-tasks-hpc-0.5.0/scriptengine_tasks_hpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-09-30 09:22:26.000000 scriptengine-tasks-hpc-0.5.0/scriptengine_tasks_hpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-30 09:22:26.000000 scriptengine-tasks-hpc-0.5.0/scriptengine_tasks_hpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-09-30 09:22:26.000000 scriptengine-tasks-hpc-0.5.0/scriptengine_tasks_hpc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-30 09:22:26.000000 scriptengine-tasks-hpc-0.5.0/scriptengine_tasks_hpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-09-30 09:22:26.000000 scriptengine-tasks-hpc-0.5.0/scriptengine_tasks_hpc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-30 09:22:26.056716 scriptengine-tasks-hpc-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1594 2022-09-30 09:22:16.000000 scriptengine-tasks-hpc-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:16:32.081647 scriptengine-tasks-hpc-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 10:16:12.000000 scriptengine-tasks-hpc-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-28 10:16:32.081647 scriptengine-tasks-hpc-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-28 10:16:12.000000 scriptengine-tasks-hpc-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-28 10:16:12.000000 scriptengine-tasks-hpc-0.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:16:32.081647 scriptengine-tasks-hpc-0.6.0/scriptengine_hpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 10:16:12.000000 scriptengine-tasks-hpc-0.6.0/scriptengine_hpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-28 10:16:12.000000 scriptengine-tasks-hpc-0.6.0/scriptengine_hpc/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-04-28 10:16:12.000000 scriptengine-tasks-hpc-0.6.0/scriptengine_hpc/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 10:16:12.000000 scriptengine-tasks-hpc-0.6.0/scriptengine_hpc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:16:32.081647 scriptengine-tasks-hpc-0.6.0/scriptengine_tasks_hpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-28 10:16:32.000000 scriptengine-tasks-hpc-0.6.0/scriptengine_tasks_hpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-28 10:16:32.000000 scriptengine-tasks-hpc-0.6.0/scriptengine_tasks_hpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 10:16:32.000000 scriptengine-tasks-hpc-0.6.0/scriptengine_tasks_hpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-28 10:16:32.000000 scriptengine-tasks-hpc-0.6.0/scriptengine_tasks_hpc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-28 10:16:32.000000 scriptengine-tasks-hpc-0.6.0/scriptengine_tasks_hpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 10:16:32.000000 scriptengine-tasks-hpc-0.6.0/scriptengine_tasks_hpc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 10:16:32.081647 scriptengine-tasks-hpc-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-28 10:16:12.000000 scriptengine-tasks-hpc-0.6.0/setup.py
```

### Comparing `scriptengine-tasks-hpc-0.5.0/LICENSE` & `scriptengine-tasks-hpc-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scriptengine-tasks-hpc-0.5.0/PKG-INFO` & `scriptengine-tasks-hpc-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scriptengine-tasks-hpc
-Version: 0.5.0
+Version: 0.6.0
 Summary: ScriptEngine tasks you may need on HPC systems
 Home-page: https://github.com/uwefladrich/scriptengine-tasks-hpc
 Author: Uwe Fladrich
 Author-email: uwe.fladrich@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `scriptengine-tasks-hpc-0.5.0/scriptengine_hpc/module.py` & `scriptengine-tasks-hpc-0.6.0/scriptengine_hpc/module.py`

 * *Files identical despite different names*

### Comparing `scriptengine-tasks-hpc-0.5.0/scriptengine_hpc/slurm.py` & `scriptengine-tasks-hpc-0.6.0/scriptengine_hpc/slurm.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,45 +27,46 @@
         def is_sbatch_opt(opt):
             return opt not in (
                 "scripts",
                 "hetjob_spec",
                 "stop_after_submit",
                 "submit_from_batch_job",
                 "set_jobid",
+                "sbatch_command",
             ) and not opt.startswith("_")
 
         if in_batch_job() and not do_recursive_submit():
             self.log_debug(
                 "Already running within a batch job and "
                 '"submit_from_batch_job" is not set or false - '
                 "not submitting new job"
             )
             return
 
         # Start building the sbatch command line
-        sbatch_cmd_line = [_SBATCH_CMD]
+        sbatch_cmd_line = [self.getarg("sbatch_command", default=_SBATCH_CMD)]
 
         sbatch_general_args = ["--parsable"]
         for opt, arg in self.__dict__.items():
             if is_sbatch_opt(opt):
                 sbatch_general_args.append(f"--{opt}")
-                if arg:
+                if arg is not None:
                     sbatch_general_args.append(j2render(arg, context))
         sbatch_cmd_line.extend(map(str, sbatch_general_args))
 
         hetjob_spec = self.getarg("hetjob_spec", context, default=[])
         if hetjob_spec:
             self.log_debug("Submiting hetereogeneous SLURM job with sbatch")
             sbatch_hetjob_args = []
             for job_args in hetjob_spec:
                 if len(sbatch_hetjob_args) > 0:
                     sbatch_hetjob_args.append(":")
                 for opt, arg in job_args.items():
                     sbatch_hetjob_args.append(f"--{opt}")
-                    if arg:
+                    if arg is not None:
                         sbatch_hetjob_args.append(j2render(arg, context))
             sbatch_cmd_line.extend(map(str, sbatch_hetjob_args))
 
         scripts = self.getarg("scripts", context, default=None)
         if scripts:
             sbatch_cmd_line.append("se")
             sbatch_cmd_line.extend(
```

### Comparing `scriptengine-tasks-hpc-0.5.0/scriptengine_tasks_hpc.egg-info/PKG-INFO` & `scriptengine-tasks-hpc-0.6.0/scriptengine_tasks_hpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scriptengine-tasks-hpc
-Version: 0.5.0
+Version: 0.6.0
 Summary: ScriptEngine tasks you may need on HPC systems
 Home-page: https://github.com/uwefladrich/scriptengine-tasks-hpc
 Author: Uwe Fladrich
 Author-email: uwe.fladrich@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `scriptengine-tasks-hpc-0.5.0/setup.py` & `scriptengine-tasks-hpc-0.6.0/setup.py`

 * *Files identical despite different names*

