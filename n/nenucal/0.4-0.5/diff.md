# Comparing `tmp/nenucal-0.4.tar.gz` & `tmp/nenucal-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nenucal-0.4.tar", max compression
+gzip compressed data, was "nenucal-0.5.tar", max compression
```

## Comparing `nenucal-0.4.tar` & `nenucal-0.5.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0    35057 2020-04-03 15:29:02.397708 nenucal-0.4/LICENSE
--rw-r--r--   0        0        0     1635 2021-03-10 15:16:32.056750 nenucal-0.4/README.md
--rw-r--r--   0        0        0      167 2021-04-30 14:21:29.295607 nenucal-0.4/nenucal/__init__.py
--rwxr-xr-x   0        0        0    27725 2023-01-13 15:37:24.436455 nenucal-0.4/nenucal/cal.py
--rw-r--r--   0        0        0     3952 2020-04-18 13:41:20.999414 nenucal-0.4/nenucal/cal_config/LBAdefault_after_di.rfis
--rw-r--r--   0        0        0      147 2022-05-26 08:28:41.664798 nenucal-0.4/nenucal/cal_config/dppp_applycal.parset
--rw-r--r--   0        0        0      235 2022-05-26 08:28:43.544789 nenucal-0.4/nenucal/cal_config/dppp_applycal_diag.parset
--rw-r--r--   0        0        0      289 2022-05-26 08:28:40.276805 nenucal-0.4/nenucal/cal_config/dppp_ddecal.parset
--rw-r--r--   0        0        0      125 2020-04-18 13:45:39.383128 nenucal-0.4/nenucal/cal_config/dppp_flagger.parset
--rw-r--r--   0        0        0      172 2022-05-26 08:28:50.868754 nenucal-0.4/nenucal/cal_config/dppp_predict.parset
--rw-r--r--   0        0        0      353 2022-05-26 08:28:53.640740 nenucal-0.4/nenucal/cal_config/dppp_predict_diag.parset
--rw-r--r--   0        0        0      125 2022-05-26 08:28:56.456727 nenucal-0.4/nenucal/cal_config/dppp_predict_nocal.parset
--rw-r--r--   0        0        0       75 2020-10-18 16:53:37.980733 nenucal-0.4/nenucal/cal_config/dppp_preflag.parset
--rw-r--r--   0        0        0      186 2022-05-26 08:29:06.260680 nenucal-0.4/nenucal/cal_config/dppp_subtract.parset
--rw-r--r--   0        0        0      339 2022-05-26 08:29:09.708663 nenucal-0.4/nenucal/cal_config/dppp_subtract_diag.parset
--rw-r--r--   0        0        0      143 2022-05-26 08:29:12.660649 nenucal-0.4/nenucal/cal_config/dppp_subtract_nocal.parset
--rw-r--r--   0        0        0     5666 2023-01-26 13:20:17.546729 nenucal-0.4/nenucal/datahandler.py
--rw-r--r--   0        0        0    11059 2021-09-20 14:57:13.219041 nenucal-0.4/nenucal/delayflag.py
--rw-r--r--   0        0        0     5314 2021-04-30 13:23:07.476762 nenucal-0.4/nenucal/flagutils.py
--rw-r--r--   0        0        0     8346 2022-10-19 15:45:01.373259 nenucal-0.4/nenucal/msutils.py
--rw-r--r--   0        0        0      868 2021-08-30 09:22:02.541727 nenucal-0.4/nenucal/settings.py
--rw-r--r--   0        0        0    10662 2022-12-19 11:10:36.982678 nenucal-0.4/nenucal/skymodel.py
--rw-r--r--   0        0        0    15810 2020-09-17 21:02:14.575691 nenucal-0.4/nenucal/smoothsol.py
--rw-r--r--   0        0        0    11405 2022-10-14 14:07:39.287278 nenucal-0.4/nenucal/tasks.py
--rw-r--r--   0        0        0    50555 2021-10-14 15:28:56.159274 nenucal-0.4/nenucal/templates/Ateam_lowres.skymodel
--rw-r--r--   0        0        0      283 2022-05-24 15:25:36.730085 nenucal-0.4/nenucal/templates/default_img_settings.toml
--rw-r--r--   0        0        0     2127 2021-10-19 20:36:02.701080 nenucal-0.4/nenucal/templates/default_settings.toml
--rw-r--r--   0        0        0      810 2020-04-21 12:34:17.298949 nenucal-0.4/nenucal/templates/ssins_config.toml
--rw-r--r--   0        0        0        0 2019-11-02 13:48:32.657550 nenucal-0.4/nenucal/tests/__init__.py
--rw-r--r--   0        0        0     3440 2021-04-30 13:23:22.172838 nenucal-0.4/nenucal/tests/test_msutils.py
--rw-r--r--   0        0        0      433 2020-04-29 10:03:05.073942 nenucal-0.4/nenucal/tests/test_utils.py
--rw-r--r--   0        0        0        0 2016-07-04 11:35:35.897416 nenucal-0.4/nenucal/tools/__init__.py
--rw-r--r--   0        0        0     6755 2021-09-20 14:56:06.902458 nenucal-0.4/nenucal/tools/bpcal.py
--rw-r--r--   0        0        0     2964 2021-09-08 11:53:49.291721 nenucal-0.4/nenucal/tools/calpipe.py
--rw-r--r--   0        0        0     9545 2022-03-18 15:14:14.978309 nenucal-0.4/nenucal/tools/flagtool.py
--rw-r--r--   0        0        0     3564 2023-02-04 10:38:21.907319 nenucal-0.4/nenucal/tools/imgpipe.py
--rw-r--r--   0        0        0     5416 2022-12-09 14:51:39.176290 nenucal-0.4/nenucal/tools/modeltool.py
--rw-r--r--   0        0        0    13335 2022-12-13 22:23:38.449220 nenucal-0.4/nenucal/tools/nenudata.py
--rwxr-xr-x   0        0        0    13446 2022-12-15 08:12:23.413902 nenucal-0.4/nenucal/tools/soltool.py
--rw-r--r--   0        0        0     2050 2021-08-30 09:48:30.150265 nenucal-0.4/nenucal/utils.py
--rw-r--r--   0        0        0     1102 2023-02-12 14:23:20.679153 nenucal-0.4/pyproject.toml
--rw-r--r--   0        0        0     3279 1970-01-01 00:00:00.000000 nenucal-0.4/setup.py
--rw-r--r--   0        0        0     3023 1970-01-01 00:00:00.000000 nenucal-0.4/PKG-INFO
+-rw-r--r--   0        0        0    35057 2020-04-03 15:29:02.397708 nenucal-0.5/LICENSE
+-rw-r--r--   0        0        0     1635 2021-03-10 15:16:32.056750 nenucal-0.5/README.md
+-rw-r--r--   0        0        0      167 2021-04-30 14:21:29.295607 nenucal-0.5/nenucal/__init__.py
+-rwxr-xr-x   0        0        0    28488 2023-04-21 13:46:00.732112 nenucal-0.5/nenucal/cal.py
+-rw-r--r--   0        0        0     3952 2020-04-18 13:41:20.999414 nenucal-0.5/nenucal/cal_config/LBAdefault_after_di.rfis
+-rw-r--r--   0        0        0      147 2022-05-26 08:28:41.664798 nenucal-0.5/nenucal/cal_config/dppp_applycal.parset
+-rw-r--r--   0        0        0      235 2022-05-26 08:28:43.544789 nenucal-0.5/nenucal/cal_config/dppp_applycal_diag.parset
+-rw-r--r--   0        0        0      289 2022-05-26 08:28:40.276805 nenucal-0.5/nenucal/cal_config/dppp_ddecal.parset
+-rw-r--r--   0        0        0      125 2020-04-18 13:45:39.383128 nenucal-0.5/nenucal/cal_config/dppp_flagger.parset
+-rw-r--r--   0        0        0      172 2022-05-26 08:28:50.868754 nenucal-0.5/nenucal/cal_config/dppp_predict.parset
+-rw-r--r--   0        0        0      353 2022-05-26 08:28:53.640740 nenucal-0.5/nenucal/cal_config/dppp_predict_diag.parset
+-rw-r--r--   0        0        0      125 2022-05-26 08:28:56.456727 nenucal-0.5/nenucal/cal_config/dppp_predict_nocal.parset
+-rw-r--r--   0        0        0       75 2020-10-18 16:53:37.980733 nenucal-0.5/nenucal/cal_config/dppp_preflag.parset
+-rw-r--r--   0        0        0      186 2022-05-26 08:29:06.260680 nenucal-0.5/nenucal/cal_config/dppp_subtract.parset
+-rw-r--r--   0        0        0      339 2022-05-26 08:29:09.708663 nenucal-0.5/nenucal/cal_config/dppp_subtract_diag.parset
+-rw-r--r--   0        0        0      143 2022-05-26 08:29:12.660649 nenucal-0.5/nenucal/cal_config/dppp_subtract_nocal.parset
+-rw-r--r--   0        0        0     5666 2023-01-26 13:20:17.546729 nenucal-0.5/nenucal/datahandler.py
+-rw-r--r--   0        0        0    26307 2023-04-23 22:28:11.169649 nenucal-0.5/nenucal/delayflag.py
+-rw-r--r--   0        0        0     5314 2023-04-21 16:37:36.820627 nenucal-0.5/nenucal/flagutils.py
+-rw-r--r--   0        0        0     8350 2023-03-22 13:21:15.106030 nenucal-0.5/nenucal/msutils.py
+-rw-r--r--   0        0        0      868 2021-08-30 09:22:02.541727 nenucal-0.5/nenucal/settings.py
+-rw-r--r--   0        0        0    10662 2022-12-19 11:10:36.982678 nenucal-0.5/nenucal/skymodel.py
+-rw-r--r--   0        0        0    15810 2020-09-17 21:02:14.575691 nenucal-0.5/nenucal/smoothsol.py
+-rw-r--r--   0        0        0    11405 2022-10-14 14:07:39.287278 nenucal-0.5/nenucal/tasks.py
+-rw-r--r--   0        0        0    50555 2021-10-14 15:28:56.159274 nenucal-0.5/nenucal/templates/Ateam_lowres.skymodel
+-rw-r--r--   0        0        0      283 2022-05-24 15:25:36.730085 nenucal-0.5/nenucal/templates/default_img_settings.toml
+-rw-r--r--   0        0        0     2214 2023-03-31 23:03:26.008112 nenucal-0.5/nenucal/templates/default_settings.toml
+-rw-r--r--   0        0        0      403 2023-04-23 22:30:23.801654 nenucal-0.5/nenucal/templates/default_vis_flagger_config.toml
+-rw-r--r--   0        0        0      810 2020-04-21 12:34:17.298949 nenucal-0.5/nenucal/templates/ssins_config.toml
+-rw-r--r--   0        0        0        0 2019-11-02 13:48:32.657550 nenucal-0.5/nenucal/tests/__init__.py
+-rw-r--r--   0        0        0     3440 2021-04-30 13:23:22.172838 nenucal-0.5/nenucal/tests/test_msutils.py
+-rw-r--r--   0        0        0      433 2020-04-29 10:03:05.073942 nenucal-0.5/nenucal/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2016-07-04 11:35:35.897416 nenucal-0.5/nenucal/tools/__init__.py
+-rw-r--r--   0        0        0     6755 2021-09-20 14:56:06.902458 nenucal-0.5/nenucal/tools/bpcal.py
+-rw-r--r--   0        0        0     2964 2021-09-08 11:53:49.291721 nenucal-0.5/nenucal/tools/calpipe.py
+-rw-r--r--   0        0        0    10448 2023-04-22 09:01:37.366552 nenucal-0.5/nenucal/tools/flagtool.py
+-rw-r--r--   0        0        0     3564 2023-02-04 10:38:21.907319 nenucal-0.5/nenucal/tools/imgpipe.py
+-rw-r--r--   0        0        0     5416 2022-12-09 14:51:39.176290 nenucal-0.5/nenucal/tools/modeltool.py
+-rw-r--r--   0        0        0    13335 2022-12-13 22:23:38.449220 nenucal-0.5/nenucal/tools/nenudata.py
+-rwxr-xr-x   0        0        0    13454 2023-03-22 13:21:15.110030 nenucal-0.5/nenucal/tools/soltool.py
+-rw-r--r--   0        0        0     2050 2021-08-30 09:48:30.150265 nenucal-0.5/nenucal/utils.py
+-rw-r--r--   0        0        0     1102 2023-04-28 09:10:27.974826 nenucal-0.5/pyproject.toml
+-rw-r--r--   0        0        0     3279 1970-01-01 00:00:00.000000 nenucal-0.5/setup.py
+-rw-r--r--   0        0        0     3023 1970-01-01 00:00:00.000000 nenucal-0.5/PKG-INFO
```

### Comparing `nenucal-0.4/LICENSE` & `nenucal-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nenucal-0.4/README.md` & `nenucal-0.5/README.md`

 * *Files identical despite different names*

### Comparing `nenucal-0.4/nenucal/cal.py` & `nenucal-0.5/nenucal/cal.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,24 +84,26 @@
         futils.zip_copy(msins, msouts, self.get_sky_model_bbs(''))
 
 
 class CalSettings(object):
 
     def __init__(self, parmdb='instrument.h5', sol_int=1, sol_int_flux_per_slot_per_sec=0,
                  sol_int_min=2, sol_int_max=120, mode='fulljones', uv_min=None, smoothnessconstraint=4e6,
-                 extra={}, **kargs):
+                 solveralgorithm='directionsolve', solutions_per_direction={}, extra={}, **kargs):
         self.parmdb = parmdb
         self.sol_int = sol_int
         self.cal_mode = mode
         self.uv_min = uv_min
         self.extra_params = extra
         self.sol_int_min = sol_int_min
         self.sol_int_max = sol_int_max
         self.sol_int_flux_per_slot_per_sec = sol_int_flux_per_slot_per_sec
         self.smoothnessconstraint = smoothnessconstraint
+        self.solveralgorithm = solveralgorithm
+        self.solutions_per_direction = solutions_per_direction
         self.freq_cache = {}
         self.interval_cache = {}
 
     def get_time_interval(self, msin):
         if msin not in self.interval_cache:
             self.interval_cache[msin] = msutils.get_ms_time_interval(msin)
         return self.interval_cache[msin]
@@ -162,14 +164,15 @@
         return None
 
     def run(self, in_files):
         print(f'Starting {self.name} ...')
         kargs = self.worker_settings.copy()
         del kargs['run_on_file_host']
         del kargs['run_on_file_host_pattern']
+        del kargs['numthreads']
         pool = worker.get_worker_pool(self.name, max_time=self.max_time, **kargs)
         out_files = []
 
         for in_file in in_files:
             host = None
             if self.worker_settings.run_on_file_host and self.worker_settings.run_on_file_host_pattern:
                 r = re.search(self.worker_settings.run_on_file_host_pattern, in_file)
@@ -355,15 +358,18 @@
         date_str = datetime.datetime.now().strftime('%Y-%m-%dT%H:%M:%S')
         return f'{log_dir}/{date_str}_{os.path.basename(msin)}_{log_name}.log'
 
     def build_command(self, msin):
         parameters = self.get_parameters(msin)
         if parameters is None:
             return None
-        return f'cd {cwd}; {self.exec_name} {self.parset} msin={msin} {" ".join(parameters)}'
+        n_threads = ''
+        if self.worker_settings.numthreads != 0:
+            n_threads = 'numthreads={self.worker_settings.numthreads}'
+        return f'cd {cwd}; {self.exec_name} {self.parset} msin={msin} {n_threads} {" ".join(parameters)}'
 
     def get_directions_str(self, directions):
         if isinstance(directions, str):
             return f'[[{directions}]]'
         return '[%s]' % ','.join(['[%s]' % k for k in directions])
 
     def get_directions_str_single_list(self, directions):
@@ -415,25 +421,34 @@
         parmdb_out = f'{msin}/{self.settings.parmdb}'
 
         if os.path.exists(parmdb_out):
             os.remove(parmdb_out)
 
         directions = self.sky_model.get_directions(msin, self.directions)
 
+        sol_per_dir = []
+        for direction in directions:
+            if direction in self.settings.solutions_per_direction:
+                sol_per_dir.append(self.settings.solutions_per_direction[direction])
+            else:
+                sol_per_dir.append(1)
+
         sol_int = self.settings.get_sol_int(msin, self.sky_model.get_patch_i(msin, directions))
 
         p = []
         p.append(f'msin.datacolumn={self.data_col}')
         p.append(f'msout.datacolumn={self.data_col_out}')
         p.append(f'cal.sourcedb={self.sky_model.get_sky_model(msin)}')
         p.append(f'cal.directions={self.get_directions_str(directions)}')
         p.append(f'cal.h5parm={parmdb_out}')
         p.append(f'cal.solint={sol_int}')
         p.append(f'cal.mode={self.settings.cal_mode}')
         p.append(f'cal.smoothnessconstraint={self.settings.smoothnessconstraint}')
+        p.append(f'cal.solveralgorithm={self.settings.solveralgorithm}')
+        p.append(f'cal.solutions_per_direction="{str(sol_per_dir)}"')
 
         for k, v in self.settings.extra_params.items():
             p.append(f'cal.{k}={v}')
 
         if self.settings.uv_min:
             p.append(f'cal.uvlambdamin={self.settings.get_uv_min(msin)}')
 
@@ -486,15 +501,15 @@
 
     def get_parameters(self, msin):
         directions = self.sky_model.get_directions(msin, self.directions)
         if not directions:
             return None
 
         p = []
-        p.append(f'msin.datacolumn={self.col_out}')
+        p.append(f'msin.datacolumn=DATA')
         p.append(f'msout.datacolumn={self.col_out}')
         p.append(f'predict.sourcedb={self.sky_model.get_sky_model(msin)}')
         if self.settings.parmdb.strip():
             p.append(f'predict.directions={self.get_directions_str(directions)}')
             p.append(f'predict.applycal.parmdb={msin}/{self.settings.parmdb}')
         else:
             p.append(f'predict.sources={self.get_directions_str_single_list(directions)}')
```

### Comparing `nenucal-0.4/nenucal/cal_config/LBAdefault_after_di.rfis` & `nenucal-0.5/nenucal/cal_config/LBAdefault_after_di.rfis`

 * *Files identical despite different names*

### Comparing `nenucal-0.4/nenucal/datahandler.py` & `nenucal-0.5/nenucal/datahandler.py`

 * *Files identical despite different names*

### Comparing `nenucal-0.4/nenucal/flagutils.py` & `nenucal-0.5/nenucal/flagutils.py`

 * *Files identical despite different names*

### Comparing `nenucal-0.4/nenucal/msutils.py` & `nenucal-0.5/nenucal/msutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
 
 def get_ms_time_interval(ms_file):
     with tables.table(ms_file) as t:
         return t.getcell('INTERVAL', 0)
 
 
 def get_info_from_ms_files(files):
-    t_start = []
+    t_start = []    
     t_end = []
     t_total = 0
 
     for file in files:
         with tables.table(file, ack=False) as t:
             start = t.getcell('TIME', 0)
             end = t.getcell('TIME', t.nrows() - 1)
```

### Comparing `nenucal-0.4/nenucal/settings.py` & `nenucal-0.5/nenucal/settings.py`

 * *Files identical despite different names*

### Comparing `nenucal-0.4/nenucal/skymodel.py` & `nenucal-0.5/nenucal/skymodel.py`

 * *Files identical despite different names*

### Comparing `nenucal-0.4/nenucal/smoothsol.py` & `nenucal-0.5/nenucal/smoothsol.py`

 * *Files identical despite different names*

### Comparing `nenucal-0.4/nenucal/tasks.py` & `nenucal-0.5/nenucal/tasks.py`

 * *Files identical despite different names*

### Comparing `nenucal-0.4/nenucal/templates/Ateam_lowres.skymodel` & `nenucal-0.5/nenucal/templates/Ateam_lowres.skymodel`

 * *Files identical despite different names*

### Comparing `nenucal-0.4/nenucal/templates/default_settings.toml` & `nenucal-0.5/nenucal/templates/default_settings.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 nodes = 'localhost'
 max_concurrent = 4
 env_file = ''
 debug = false
 dry_run = false
 run_on_file_host = false
 run_on_file_host_pattern = ''
+numthreads = 0
 
 [sky_model]
 int_sky_model = 'lcs165'
 app_sky_model_name = 'app_sky_model'
 app_sky_model_file = ''
 int_ateam_sky_model = 'lowres'
 
@@ -42,14 +43,16 @@
 avg.time = 1
 avg.freq = 1
 cal.parmdb = 'instrument_dde.h5'
 cal.sol_int = 20
 cal.mode = 'diagonal'
 cal.uv_min = 10
 cal.smoothnessconstraint = 4e6
+cal.solveralgorithm = 'directionsolve'
+cal.solutions_per_direction = {}
 cal.extra = {}
 do_smooth_sol = true
 plot_sol = true
 smooth_sol.time_min = 15
 smooth_sol.freq_mhz = 1
 smooth_sol.main_time_min = 20
 smooth_sol.main_freq_mhz = 4
```

### Comparing `nenucal-0.4/nenucal/templates/ssins_config.toml` & `nenucal-0.5/nenucal/templates/ssins_config.toml`

 * *Files identical despite different names*

### Comparing `nenucal-0.4/nenucal/tests/test_msutils.py` & `nenucal-0.5/nenucal/tests/test_msutils.py`

 * *Files identical despite different names*

### Comparing `nenucal-0.4/nenucal/tools/bpcal.py` & `nenucal-0.5/nenucal/tools/bpcal.py`

 * *Files identical despite different names*

### Comparing `nenucal-0.4/nenucal/tools/calpipe.py` & `nenucal-0.5/nenucal/tools/calpipe.py`

 * *Files identical despite different names*

### Comparing `nenucal-0.4/nenucal/tools/flagtool.py` & `nenucal-0.5/nenucal/tools/flagtool.py`

 * *Files 7% similar despite different names*

```diff
@@ -247,9 +247,26 @@
             f.plot_delay_ps_iv(plot_dir)
         f.plot_delay_flag(res, plot_dir)
 
     if not dry_run:
         f.save_flag(res)
 
 
+@main.command('vis_flagger')
+@click.argument('ms_in', type=t_dir)
+@click.argument('config', type=t_file)
+@click.option('backup_flag', '--backup', help='Backup flags before vis flagger', is_flag=True)
+@click.option('restore_flag', '--restore', help='Restore previously backup-ed flags', is_flag=True)
+@click.option('--plot_dir', help='Plot directory', type=t_dir, default=None)
+@click.option('--backup_file', help='Backup filename', type=str, default='flags_before_vis_flagger.h5')
+@click.option('--dry_run', help='Do not apply flags', is_flag=True)
+def vis_flagger(ms_in, config, backup_flag, restore_flag, plot_dir, backup_file, dry_run):
+    ''' Run the vis_flagger algorithm on MS_IN with configuration CONFIG '''
+    from nenucal import delayflag
+
+    backup_restore(ms_in, backup_flag, restore_flag, backup_file)
+
+    delayflag.apply_vis_filter(ms_in, config, plot_dir=plot_dir, dry_run=dry_run)
+
+
 if __name__ == '__main__':
     main()
```

### Comparing `nenucal-0.4/nenucal/tools/imgpipe.py` & `nenucal-0.5/nenucal/tools/imgpipe.py`

 * *Files identical despite different names*

### Comparing `nenucal-0.4/nenucal/tools/modeltool.py` & `nenucal-0.5/nenucal/tools/modeltool.py`

 * *Files identical despite different names*

### Comparing `nenucal-0.4/nenucal/tools/nenudata.py` & `nenucal-0.5/nenucal/tools/nenudata.py`

 * *Files identical despite different names*

### Comparing `nenucal-0.4/nenucal/tools/soltool.py` & `nenucal-0.5/nenucal/tools/soltool.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,16 +210,16 @@
         v = sol.amp[:, :, :, dir, pol]
     elif data_type == 'Phase':
         v = sol.phase[:, :, :, dir, pol]
     else:
         print(f'Error: data type {data_type} unknown')
         return
 
-    vmax = np.nanquantile(v[~v.mask & ~np.isnan(v) & (v != 0)], 0.999)
-    vmin = np.nanquantile(v[~v.mask & ~np.isnan(v) & (v != 0)], 0.001)
+        vmax = np.nanquantile(v[~v.mask & ~np.isnan(v) & (v != 0)], 0.999)
+        vmin = np.nanquantile(v[~v.mask & ~np.isnan(v) & (v != 0)], 0.001)
     extent = [0, len(sol.time), sol.freqs.min() * 1e-6, sol.freqs.max() * 1e-6]
 
     n = v.shape[2]
     ncols, nrows = int(np.ceil(np.sqrt(n))), int(np.ceil(n / np.ceil(np.sqrt(n))))
 
     fig, axs = plt.subplots(ncols=ncols, nrows=nrows, sharey=True, figsize=(1 + 2 * ncols, 1 + 1.5 * nrows),
                             sharex=True)
```

### Comparing `nenucal-0.4/nenucal/utils.py` & `nenucal-0.5/nenucal/utils.py`

 * *Files identical despite different names*

### Comparing `nenucal-0.4/pyproject.toml` & `nenucal-0.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nenucal"
-version = "0.4"
+version = "0.5"
 description = "Calibration pipeline for the NenuFAR Cosmic Dawn project"
 authors = ["\"Florent Mertens\" <\"florent.mertens@gmail.com\">"]
 license = "GPL-3.0-or-later"
 readme = 'README.md'
 repository = "https://gitlab.com/flomertens/nenucal-cd"
 
 [tool.poetry.dependencies]
```

### Comparing `nenucal-0.4/setup.py` & `nenucal-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                      'imgpipe = nenucal.tools.imgpipe:main',
                      'modeltool = nenucal.tools.modeltool:main',
                      'nenudata = nenucal.tools.nenudata:main',
                      'soltool = nenucal.tools.soltool:main']}
 
 setup_kwargs = {
     'name': 'nenucal',
-    'version': '0.4',
+    'version': '0.5',
     'description': 'Calibration pipeline for the NenuFAR Cosmic Dawn project',
     'long_description': 'NenuCAL CD\n==========\n\nCalibration pipeline and set of utilities for the NenuFAR Cosmic Dawn project. The calibration uses the standard LOFAR [DPPP](https://github.com/lofar-astron/DP3/tree/master/DPPP) in the background and should be general enough to be used by any NenuFAR projects.\n\nInstallation\n------------\n\nnenucal-cd can be installed via pip:\n\n    $ pip install nenucal-cd\n\nand requires Python 3.7.0 or higher. For most tasks, you will also need [DPPP](https://github.com/lofar-astron/DP3/tree/master/DPPP), [LSMTool](https://www.astron.nl/citt/lsmtool/overview.html) that you can install with the command:\n\n    $ pip install git+https://github.com/darafferty/LSMTool.git\n\nand [LoSoTo](https://revoltek.github.io/losoto/) that you can install with the command:\n\n    $ pip install git+https://github.com/revoltek/losoto\n\nUsage\n-----\n\nCalibration is performed using the `calpipe` utility. You will find [here some documentations](https://gitlab.com/flomertens/nenucal-cd/-/wikis/Calibrating-NenuFAR-data) on how to use it.\n\nAdditionally to calpipe, this package provides a tool to manage the FLAG column and run a SSINS flagger ([flagtool](https://gitlab.com/flomertens/nenucal-cd/-/wikis/flagging-utility)), a tool to plot and smooth gain solutions ([soltool](https://gitlab.com/flomertens/nenucal-cd/-/wikis/soltool-utility)) and a tool to produce apparent sky model from catalog ([modeltool](https://gitlab.com/flomertens/nenucal-cd/-/wikis/sky-model-utility)).\n\nContact\n-------\n\nDo not hesitate to fill an [issue](https://gitlab.com/flomertens/nenucal-cd/-/issues) or contact me if you encounter a problem with this package.\n',
     'author': '"Florent Mertens"',
     'author_email': '"florent.mertens@gmail.com"',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/flomertens/nenucal-cd',
```

### Comparing `nenucal-0.4/PKG-INFO` & `nenucal-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nenucal
-Version: 0.4
+Version: 0.5
 Summary: Calibration pipeline for the NenuFAR Cosmic Dawn project
 Home-page: https://gitlab.com/flomertens/nenucal-cd
 License: GPL-3.0-or-later
 Author: "Florent Mertens"
 Author-email: "florent.mertens@gmail.com"
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

