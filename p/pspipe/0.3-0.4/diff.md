# Comparing `tmp/pspipe-0.3.tar.gz` & `tmp/pspipe-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pspipe-0.3.tar", max compression
+gzip compressed data, was "pspipe-0.4.tar", max compression
```

## Comparing `pspipe-0.3.tar` & `pspipe-0.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    35057 2020-03-25 08:38:00.984262 pspipe-0.3/LICENSE
--rw-r--r--   0        0        0     1568 2020-03-22 11:57:27.390814 pspipe-0.3/README.md
--rw-r--r--   0        0        0      167 2021-04-30 13:20:21.564096 pspipe-0.3/pspipe/__init__.py
--rw-r--r--   0        0        0    16280 2022-10-20 08:38:52.912222 pspipe-0.3/pspipe/database.py
--rw-r--r--   0        0        0     3843 2022-07-25 11:03:11.138043 pspipe-0.3/pspipe/obsdata.py
--rw-r--r--   0        0        0     5302 2023-03-29 14:15:56.047218 pspipe-0.3/pspipe/settings.py
--rw-r--r--   0        0        0    41441 2023-02-17 16:42:58.642697 pspipe-0.3/pspipe/tasks.py
--rw-r--r--   0        0        0       71 2020-03-13 17:39:40.322062 pspipe-0.3/pspipe/templates/config/eor_bins_a12.parset
--rw-r--r--   0        0        0      177 2023-03-29 12:33:10.159397 pspipe-0.3/pspipe/templates/config/eor_bins_alo.parset
--rw-r--r--   0        0        0      108 2020-03-13 18:23:45.474787 pspipe-0.3/pspipe/templates/config/eor_bins_hba.parset
--rw-r--r--   0        0        0      123 2020-03-31 09:15:42.863020 pspipe-0.3/pspipe/templates/config/eor_bins_nenufar.parset
--rw-r--r--   0        0        0      864 2022-09-12 12:26:46.680401 pspipe-0.3/pspipe/templates/config/flagger.parset
--rw-r--r--   0        0        0      770 2020-03-13 17:40:31.599661 pspipe-0.3/pspipe/templates/config/flagger_pre_combine.parset
--rw-r--r--   0        0        0      898 2020-03-13 17:51:41.097416 pspipe-0.3/pspipe/templates/config/gpr_config_a12.parset
--rw-r--r--   0        0        0     1256 2020-03-13 17:55:28.669775 pspipe-0.3/pspipe/templates/config/gpr_config_hba.parset
--rw-r--r--   0        0        0      898 2020-03-13 17:51:41.097416 pspipe-0.3/pspipe/templates/config/gpr_config_nenufar.parset
--rw-r--r--   0        0        0      813 2020-03-13 17:54:30.175539 pspipe-0.3/pspipe/templates/config/gpr_config_v.parset
--rw-r--r--   0        0        0      226 2022-07-25 15:45:21.257933 pspipe-0.3/pspipe/templates/config/ps_config_a12.parset
--rw-r--r--   0        0        0      221 2023-03-29 12:43:12.194700 pspipe-0.3/pspipe/templates/config/ps_config_alo.parset
--rw-r--r--   0        0        0      168 2020-03-13 18:25:24.037432 pspipe-0.3/pspipe/templates/config/ps_config_hba.parset
--rw-r--r--   0        0        0      223 2020-03-13 17:49:12.152177 pspipe-0.3/pspipe/templates/config/ps_config_nenufar.parset
--rw-r--r--   0        0        0      425 2020-03-13 18:28:09.415080 pspipe-0.3/pspipe/templates/default_a12.toml
--rw-r--r--   0        0        0      279 2023-03-29 14:18:43.683291 pspipe-0.3/pspipe/templates/default_alo.toml
--rw-r--r--   0        0        0      432 2020-03-13 18:28:03.971158 pspipe-0.3/pspipe/templates/default_hba.toml
--rw-r--r--   0        0        0      441 2020-03-13 18:28:01.531194 pspipe-0.3/pspipe/templates/default_nenufar.toml
--rw-r--r--   0        0        0     1643 2023-02-17 16:38:09.323121 pspipe-0.3/pspipe/templates/default_settings.toml
--rw-r--r--   0        0        0        0 2019-11-02 13:48:32.657550 pspipe-0.3/pspipe/tests/__init__.py
--rw-r--r--   0        0        0      747 2020-04-22 09:29:53.352520 pspipe-0.3/pspipe/tests/test_settings.py
--rw-r--r--   0        0        0      807 2020-04-22 09:30:36.824440 pspipe-0.3/pspipe/tests/test_utils.py
--rw-r--r--   0        0        0        0 2016-07-04 11:35:35.897416 pspipe-0.3/pspipe/tools/__init__.py
--rwxr-xr-x   0        0        0    13754 2023-03-29 14:16:57.671253 pspipe-0.3/pspipe/tools/psdb.py
--rwxr-xr-x   0        0        0     1590 2020-09-18 09:39:32.570445 pspipe-0.3/pspipe/tools/pspipe.py
--rw-r--r--   0        0        0      969 2022-10-20 08:47:04.676001 pspipe-0.3/pspipe/utils.py
--rw-r--r--   0        0        0      887 2023-03-29 14:20:34.679309 pspipe-0.3/pyproject.toml
--rw-r--r--   0        0        0     2967 1970-01-01 00:00:00.000000 pspipe-0.3/setup.py
--rw-r--r--   0        0        0     2808 1970-01-01 00:00:00.000000 pspipe-0.3/PKG-INFO
+-rw-r--r--   0        0        0    35057 2020-03-25 08:38:00.984262 pspipe-0.4/LICENSE
+-rw-r--r--   0        0        0     1568 2020-03-22 11:57:27.390814 pspipe-0.4/README.md
+-rw-r--r--   0        0        0      167 2021-04-30 13:20:21.564096 pspipe-0.4/pspipe/__init__.py
+-rw-r--r--   0        0        0    16280 2022-10-20 08:38:52.912222 pspipe-0.4/pspipe/database.py
+-rw-r--r--   0        0        0     3843 2022-07-25 11:03:11.138043 pspipe-0.4/pspipe/obsdata.py
+-rw-r--r--   0        0        0     5302 2023-03-29 14:15:56.047218 pspipe-0.4/pspipe/settings.py
+-rw-r--r--   0        0        0    42910 2023-04-22 09:04:03.662371 pspipe-0.4/pspipe/tasks.py
+-rw-r--r--   0        0        0       71 2020-03-13 17:39:40.322062 pspipe-0.4/pspipe/templates/config/eor_bins_a12.parset
+-rw-r--r--   0        0        0      177 2023-03-29 12:33:10.159397 pspipe-0.4/pspipe/templates/config/eor_bins_alo.parset
+-rw-r--r--   0        0        0      108 2020-03-13 18:23:45.474787 pspipe-0.4/pspipe/templates/config/eor_bins_hba.parset
+-rw-r--r--   0        0        0      123 2020-03-31 09:15:42.863020 pspipe-0.4/pspipe/templates/config/eor_bins_nenufar.parset
+-rw-r--r--   0        0        0      864 2022-09-12 12:26:46.680401 pspipe-0.4/pspipe/templates/config/flagger.parset
+-rw-r--r--   0        0        0      770 2020-03-13 17:40:31.599661 pspipe-0.4/pspipe/templates/config/flagger_pre_combine.parset
+-rw-r--r--   0        0        0      898 2020-03-13 17:51:41.097416 pspipe-0.4/pspipe/templates/config/gpr_config_a12.parset
+-rw-r--r--   0        0        0     1256 2020-03-13 17:55:28.669775 pspipe-0.4/pspipe/templates/config/gpr_config_hba.parset
+-rw-r--r--   0        0        0      898 2020-03-13 17:51:41.097416 pspipe-0.4/pspipe/templates/config/gpr_config_nenufar.parset
+-rw-r--r--   0        0        0      813 2020-03-13 17:54:30.175539 pspipe-0.4/pspipe/templates/config/gpr_config_v.parset
+-rw-r--r--   0        0        0      226 2022-07-25 15:45:21.257933 pspipe-0.4/pspipe/templates/config/ps_config_a12.parset
+-rw-r--r--   0        0        0      221 2023-03-29 12:43:12.194700 pspipe-0.4/pspipe/templates/config/ps_config_alo.parset
+-rw-r--r--   0        0        0      168 2020-03-13 18:25:24.037432 pspipe-0.4/pspipe/templates/config/ps_config_hba.parset
+-rw-r--r--   0        0        0      223 2020-03-13 17:49:12.152177 pspipe-0.4/pspipe/templates/config/ps_config_nenufar.parset
+-rw-r--r--   0        0        0      425 2020-03-13 18:28:09.415080 pspipe-0.4/pspipe/templates/default_a12.toml
+-rw-r--r--   0        0        0      279 2023-03-29 14:18:43.683291 pspipe-0.4/pspipe/templates/default_alo.toml
+-rw-r--r--   0        0        0      432 2020-03-13 18:28:03.971158 pspipe-0.4/pspipe/templates/default_hba.toml
+-rw-r--r--   0        0        0      441 2020-03-13 18:28:01.531194 pspipe-0.4/pspipe/templates/default_nenufar.toml
+-rw-r--r--   0        0        0     1675 2023-04-21 13:37:32.448319 pspipe-0.4/pspipe/templates/default_settings.toml
+-rw-r--r--   0        0        0        0 2019-11-02 13:48:32.657550 pspipe-0.4/pspipe/tests/__init__.py
+-rw-r--r--   0        0        0      747 2020-04-22 09:29:53.352520 pspipe-0.4/pspipe/tests/test_settings.py
+-rw-r--r--   0        0        0      807 2020-04-22 09:30:36.824440 pspipe-0.4/pspipe/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2016-07-04 11:35:35.897416 pspipe-0.4/pspipe/tools/__init__.py
+-rwxr-xr-x   0        0        0    13754 2023-03-29 14:16:57.671253 pspipe-0.4/pspipe/tools/psdb.py
+-rwxr-xr-x   0        0        0     1590 2020-09-18 09:39:32.570445 pspipe-0.4/pspipe/tools/pspipe.py
+-rw-r--r--   0        0        0      969 2022-10-20 08:47:04.676001 pspipe-0.4/pspipe/utils.py
+-rw-r--r--   0        0        0      887 2023-04-28 09:13:25.702466 pspipe-0.4/pyproject.toml
+-rw-r--r--   0        0        0     2967 1970-01-01 00:00:00.000000 pspipe-0.4/setup.py
+-rw-r--r--   0        0        0     2808 1970-01-01 00:00:00.000000 pspipe-0.4/PKG-INFO
```

### Comparing `pspipe-0.3/LICENSE` & `pspipe-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pspipe-0.3/README.md` & `pspipe-0.4/README.md`

 * *Files identical despite different names*

### Comparing `pspipe-0.3/pspipe/database.py` & `pspipe-0.4/pspipe/database.py`

 * *Files identical despite different names*

### Comparing `pspipe-0.3/pspipe/obsdata.py` & `pspipe-0.4/pspipe/obsdata.py`

 * *Files identical despite different names*

### Comparing `pspipe-0.3/pspipe/settings.py` & `pspipe-0.4/pspipe/settings.py`

 * *Files identical despite different names*

### Comparing `pspipe-0.3/pspipe/tasks.py` & `pspipe-0.4/pspipe/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1072,14 +1072,62 @@
                 self.add_sub_task(DelayFlaggerSubTask(self.settings, ms_file))
 
         self.execute()
 
         return obs_ids
 
 
+class VisFlaggerSubTask(AbstractSubTask):
+
+    def __init__(self, settings_obj, ms_file):
+        AbstractSubTask.__init__(self, settings_obj, 'flagtool vis_flagger')
+        self.ms_file = ms_file
+
+    def get_log_file(self):
+        return os.path.join(self.ms_file.replace('.MS', '_vis_flagger.log'))
+
+    def get_path(self):
+        d = os.path.join(os.path.dirname(self.ms_file), 'vis_flagger')
+        futils.mkdir(d)
+        return d
+
+    def get_parameters(self):
+        return [self.ms_file, self.settings.vis_flagger.config_file, f'--plot_dir={self.get_path()}',
+                '--backup', f'--backup_file={H5_FLAG_BACKUP}']
+
+
+class VisFlagger(AbstractTask):
+
+    name = 'vis_flagger'
+    desc = 'Apply vis flagger on MS'
+
+    def __init__(self, settings_obj):
+        AbstractTask.__init__(self, 'VisFlagger', settings_obj)
+        self.db = database.Database(self.settings)
+
+    def run(self, obs_ids):
+        for obs_id in obs_ids:
+            if not self.db.has_obs_id(obs_id):
+                print(f'Error: Obs ID {obs_id} does not exist.')
+                return []
+
+            ms_files = self.db.get_obs_id_meta(obs_id).ms_files
+
+            if not ms_files:
+                print(f'Error: Obs ID {obs_id} has no MS files registered.')
+                return []
+
+            for ms_file in np.array(ms_files).flatten():
+                self.add_sub_task(VisFlaggerSubTask(self.settings, ms_file))
+
+        self.execute()
+
+        return obs_ids
+
+
 class SSINSSubTask(AbstractSubTask):
 
     def __init__(self, settings_obj, ms_file):
         AbstractSubTask.__init__(self, settings_obj, 'flagtool ssins')
         self.ms_file = ms_file
 
     def get_log_file(self):
```

### Comparing `pspipe-0.3/pspipe/templates/config/flagger.parset` & `pspipe-0.4/pspipe/templates/config/flagger.parset`

 * *Files identical despite different names*

### Comparing `pspipe-0.3/pspipe/templates/config/flagger_pre_combine.parset` & `pspipe-0.4/pspipe/templates/config/flagger_pre_combine.parset`

 * *Files identical despite different names*

### Comparing `pspipe-0.3/pspipe/templates/config/gpr_config_a12.parset` & `pspipe-0.4/pspipe/templates/config/gpr_config_a12.parset`

 * *Files identical despite different names*

### Comparing `pspipe-0.3/pspipe/templates/config/gpr_config_hba.parset` & `pspipe-0.4/pspipe/templates/config/gpr_config_hba.parset`

 * *Files identical despite different names*

### Comparing `pspipe-0.3/pspipe/templates/config/gpr_config_nenufar.parset` & `pspipe-0.4/pspipe/templates/config/gpr_config_nenufar.parset`

 * *Files identical despite different names*

### Comparing `pspipe-0.3/pspipe/templates/config/gpr_config_v.parset` & `pspipe-0.4/pspipe/templates/config/gpr_config_v.parset`

 * *Files identical despite different names*

### Comparing `pspipe-0.3/pspipe/templates/default_settings.toml` & `pspipe-0.4/pspipe/templates/default_settings.toml`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,17 @@
 umin = 50
 umax = 400
 n_time_avg = 50
 n_times = 20
 n_sigma_i = 6
 n_sigma_v = 6
 
+[vis_flagger]
+config_file = ''
+
 [image]
 name = 'default'
 umin = 50
 umax = 250
 scale = '0.5amin'
 size = '512 512'
 data_col = 'CORRECTED_DATA'
```

### Comparing `pspipe-0.3/pspipe/tests/test_settings.py` & `pspipe-0.4/pspipe/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `pspipe-0.3/pspipe/tests/test_utils.py` & `pspipe-0.4/pspipe/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pspipe-0.3/pspipe/tools/psdb.py` & `pspipe-0.4/pspipe/tools/psdb.py`

 * *Files identical despite different names*

### Comparing `pspipe-0.3/pspipe/tools/pspipe.py` & `pspipe-0.4/pspipe/tools/pspipe.py`

 * *Files identical despite different names*

### Comparing `pspipe-0.3/pspipe/utils.py` & `pspipe-0.4/pspipe/utils.py`

 * *Files identical despite different names*

### Comparing `pspipe-0.3/pyproject.toml` & `pspipe-0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pspipe"
-version = "0.3"
+version = "0.4"
 description = "Power spectra pipeline for Cosmic Dawn, Epoch of Reionization radio interferometric experiments"
 authors = ["\"Florent Mertens\" <\"florent.mertens@gmail.com\">"]
 repository = "https://gitlab.com/flomertens/pspipe/"
 readme = 'README.md'
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `pspipe-0.3/setup.py` & `pspipe-0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 entry_points = \
 {'console_scripts': ['psdb = pspipe.tools.psdb:main',
                      'pspipe = pspipe.tools.pspipe:main']}
 
 setup_kwargs = {
     'name': 'pspipe',
-    'version': '0.3',
+    'version': '0.4',
     'description': 'Power spectra pipeline for Cosmic Dawn, Epoch of Reionization radio interferometric experiments',
     'long_description': 'Power Spectra Generation pipeline for CD/EoR experiments\n========================================================\n\npspipe is an analysis pipeline which aims to make generation of high precision power-spectra for Cosmic Dawn and Epoch of Reionization experiments as easy and reproducible as possible. pspipe is the default analysis pipeline of the [Lofar-EoR](http://www.lofar.org/astronomy/eor-ksp/epoch-reionization.html) and [NenuFAR](https://nenufar.obs-nancay.fr/en/homepage-en/) CD projects. It performs all tasks from calibrated data to final the power-spectra, including:\n\n- Post-calibration flagging (using [AOflagger](https://sourceforge.net/p/aoflagger/wiki/Home/) and [SSINS](https://arxiv.org/abs/1906.01093))\n- Visibility gridding (using [WSClean](https://sourceforge.net/p/wsclean/wiki/Home/))\n- Foregrounds modeling and removal (using [GPR](https://doi.org/10.1093/mnras/sty1207), [GMCA](https://arxiv.org/abs/1209.4769), polynomial fitting)\n- Optimal power-spectra generation (using [ps_eor](https://gitlab.com/flomertens/ps_eor))\n\nThanks to its multi-nodes concurrent processing, pspipe is also very fast at crunching hundreds of hour of calibrated data.\n\nInstallation\n------------\n\npspipe can be installed via pip:\n\n    $ pip install pspipe\n\nand requires Python 3.7.0 or higher. For certain tasks, you will also need [DPPP](https://github.com/lofar-astron/DP3/tree/master/DPPP) and [WSClean](https://sourceforge.net/p/wsclean/wiki/Home/)\n\nDocumentation\n--------------\n\nPlease check the [wiki page](https://gitlab.com/flomertens/pspipe/-/wikis/home).\n',
     'author': '"Florent Mertens"',
     'author_email': '"florent.mertens@gmail.com"',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/flomertens/pspipe/',
```

### Comparing `pspipe-0.3/PKG-INFO` & `pspipe-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pspipe
-Version: 0.3
+Version: 0.4
 Summary: Power spectra pipeline for Cosmic Dawn, Epoch of Reionization radio interferometric experiments
 Home-page: https://gitlab.com/flomertens/pspipe/
 Author: "Florent Mertens"
 Author-email: "florent.mertens@gmail.com"
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

