# Comparing `tmp/asimov-gwdata-0.1.2.tar.gz` & `tmp/asimov-gwdata-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asimov-gwdata-0.1.2.tar", last modified: Wed Apr 26 09:16:39 2023, max compression
+gzip compressed data, was "asimov-gwdata-0.1.3.tar", last modified: Fri Apr 28 14:19:29 2023, max compression
```

## Comparing `asimov-gwdata-0.1.2.tar` & `asimov-gwdata-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 09:16:39.242146 asimov-gwdata-0.1.2/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      655 2023-04-26 09:16:39.242146 asimov-gwdata-0.1.2/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      148 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.2/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 09:16:39.242146 asimov-gwdata-0.1.2/asimov_gwdata.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      655 2023-04-26 09:16:39.000000 asimov-gwdata-0.1.2/asimov_gwdata.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      452 2023-04-26 09:16:39.000000 asimov-gwdata-0.1.2/asimov_gwdata.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-04-26 09:16:39.000000 asimov-gwdata-0.1.2/asimov_gwdata.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)      104 2023-04-26 09:16:39.000000 asimov-gwdata-0.1.2/asimov_gwdata.egg-info/entry_points.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       45 2023-04-26 09:16:39.000000 asimov-gwdata-0.1.2/asimov_gwdata.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        9 2023-04-26 09:16:39.000000 asimov-gwdata-0.1.2/asimov_gwdata.egg-info/top_level.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 09:16:39.242146 asimov-gwdata-0.1.2/blueprints/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      168 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.2/blueprints/asimov-analysis.yaml
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 09:16:39.242146 asimov-gwdata-0.1.2/datafind/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        5 2023-02-19 16:31:31.000000 asimov-gwdata-0.1.2/datafind/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5590 2023-04-26 06:19:27.000000 asimov-gwdata-0.1.2/datafind/asimov.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1273 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.2/datafind/datafind_template.yml
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3349 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.2/datafind/main.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1037 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.2/pyproject.toml
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 09:16:39.242146 asimov-gwdata-0.1.2/scripts/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      251 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.2/scripts/asimov-test-script.sh
--rw-r--r--   0 daniel    (1000) daniel    (1000)      121 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.2/scripts/test-calibration-dump.yaml
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-04-26 09:16:39.242146 asimov-gwdata-0.1.2/setup.cfg
--rw-r--r--   0 daniel    (1000) daniel    (1000)      122 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.2/test_settings.yaml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:19:29.648443 asimov-gwdata-0.1.3/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      655 2023-04-28 14:19:29.648443 asimov-gwdata-0.1.3/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      148 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.3/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:19:29.648443 asimov-gwdata-0.1.3/asimov_gwdata.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      655 2023-04-28 14:19:29.000000 asimov-gwdata-0.1.3/asimov_gwdata.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      452 2023-04-28 14:19:29.000000 asimov-gwdata-0.1.3/asimov_gwdata.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-04-28 14:19:29.000000 asimov-gwdata-0.1.3/asimov_gwdata.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      104 2023-04-28 14:19:29.000000 asimov-gwdata-0.1.3/asimov_gwdata.egg-info/entry_points.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       45 2023-04-28 14:19:29.000000 asimov-gwdata-0.1.3/asimov_gwdata.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        9 2023-04-28 14:19:29.000000 asimov-gwdata-0.1.3/asimov_gwdata.egg-info/top_level.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:19:29.648443 asimov-gwdata-0.1.3/blueprints/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      168 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.3/blueprints/asimov-analysis.yaml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:19:29.648443 asimov-gwdata-0.1.3/datafind/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        5 2023-02-19 16:31:31.000000 asimov-gwdata-0.1.3/datafind/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5690 2023-04-28 13:13:22.000000 asimov-gwdata-0.1.3/datafind/asimov.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1273 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.3/datafind/datafind_template.yml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3349 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.3/datafind/main.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1037 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.3/pyproject.toml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:19:29.648443 asimov-gwdata-0.1.3/scripts/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      251 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.3/scripts/asimov-test-script.sh
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      121 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.3/scripts/test-calibration-dump.yaml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-04-28 14:19:29.648443 asimov-gwdata-0.1.3/setup.cfg
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      122 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.3/test_settings.yaml
```

### Comparing `asimov-gwdata-0.1.2/PKG-INFO` & `asimov-gwdata-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asimov-gwdata
-Version: 0.1.2
+Version: 0.1.3
 Summary: An asimov plugin to make downloading gravitational wave data easier
 Author-email: Daniel Williams <daniel.williams@ligo.org>
 License: MIT
 Project-URL: Source code, https://git.ligo.org/asimov/asimov-gwdatahelp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `asimov-gwdata-0.1.2/asimov_gwdata.egg-info/PKG-INFO` & `asimov-gwdata-0.1.3/asimov_gwdata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asimov-gwdata
-Version: 0.1.2
+Version: 0.1.3
 Summary: An asimov plugin to make downloading gravitational wave data easier
 Author-email: Daniel Williams <daniel.williams@ligo.org>
 License: MIT
 Project-URL: Source code, https://git.ligo.org/asimov/asimov-gwdatahelp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `asimov-gwdata-0.1.2/datafind/asimov.py` & `asimov-gwdata-0.1.3/datafind/asimov.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,14 +58,16 @@
             "error": f"{name}.err",
             "log": f"{name}.log",
             "request_disk": "1024",
             "request_memory": "1024",
             "batch_name": f"gwdata/{name}",
             "accounting_group_user": config.get('condor', 'user'),
             "accounting_group": self.production.meta['scheduler']["accounting group"],
+            "+flock_local": "True",
+            "+DESIRED_Sites": htcondor.classad.quote("nogrid"),
         }
 
         job = htcondor.Submit(description)
         os.makedirs(self.production.rundir, exist_ok=True)
         with set_directory(self.production.rundir):
             with open(f"{name}.sub", "w") as subfile:
                 subfile.write(job.__str__())
```

### Comparing `asimov-gwdata-0.1.2/datafind/datafind_template.yml` & `asimov-gwdata-0.1.3/datafind/datafind_template.yml`

 * *Files identical despite different names*

### Comparing `asimov-gwdata-0.1.2/datafind/main.py` & `asimov-gwdata-0.1.3/datafind/main.py`

 * *Files identical despite different names*

### Comparing `asimov-gwdata-0.1.2/pyproject.toml` & `asimov-gwdata-0.1.3/pyproject.toml`

 * *Files identical despite different names*

