# Comparing `tmp/gradescope_mean-0.0.8.tar.gz` & `tmp/gradescope_mean-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gradescope_mean-0.0.8.tar", last modified: Wed Apr 26 17:43:47 2023, max compression
+gzip compressed data, was "gradescope_mean-0.0.9.tar", last modified: Fri Apr 28 16:50:48 2023, max compression
```

## Comparing `gradescope_mean-0.0.8.tar` & `gradescope_mean-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-04-26 17:43:47.158263 gradescope_mean-0.0.8/
--rw-rw-r--   0 matt      (1000) matt      (1000)     1068 2022-05-09 19:38:36.000000 gradescope_mean-0.0.8/LICENSE
--rw-rw-r--   0 matt      (1000) matt      (1000)       40 2022-05-10 15:46:26.000000 gradescope_mean-0.0.8/MANIFEST.in
--rw-rw-r--   0 matt      (1000) matt      (1000)     4313 2023-04-26 17:43:47.158263 gradescope_mean-0.0.8/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)     2641 2023-04-25 16:34:44.000000 gradescope_mean-0.0.8/README.md
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-04-26 17:43:47.150263 gradescope_mean-0.0.8/gradescope_mean/
--rw-rw-r--   0 matt      (1000) matt      (1000)       89 2022-12-15 17:55:21.000000 gradescope_mean-0.0.8/gradescope_mean/__init__.py
--rwxrwxr-x   0 matt      (1000) matt      (1000)     2486 2023-04-25 16:34:44.000000 gradescope_mean-0.0.8/gradescope_mean/__main__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1667 2023-04-25 16:34:44.000000 gradescope_mean-0.0.8/gradescope_mean/assign_list.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-04-26 17:43:47.154263 gradescope_mean-0.0.8/gradescope_mean/banner/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-25 16:34:44.000000 gradescope_mean-0.0.8/gradescope_mean/banner/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1595 2023-04-25 16:34:44.000000 gradescope_mean-0.0.8/gradescope_mean/banner/__main__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-04-26 17:43:47.154263 gradescope_mean-0.0.8/gradescope_mean/canvas/
--rw-rw-r--   0 matt      (1000) matt      (1000)       22 2023-04-25 16:34:44.000000 gradescope_mean-0.0.8/gradescope_mean/canvas/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1570 2023-04-26 17:43:12.000000 gradescope_mean-0.0.8/gradescope_mean/canvas/__main__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2619 2023-04-26 17:43:12.000000 gradescope_mean-0.0.8/gradescope_mean/canvas/canvas.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4384 2023-04-25 16:34:44.000000 gradescope_mean-0.0.8/gradescope_mean/config.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      321 2023-04-25 16:34:44.000000 gradescope_mean-0.0.8/gradescope_mean/config.yaml
--rw-rw-r--   0 matt      (1000) matt      (1000)     1431 2022-05-09 19:40:21.000000 gradescope_mean-0.0.8/gradescope_mean/get_mean_drop_low.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    15777 2023-04-25 16:47:18.000000 gradescope_mean-0.0.8/gradescope_mean/gradebook.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1441 2022-12-15 17:55:21.000000 gradescope_mean-0.0.8/gradescope_mean/perc_to_letter.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1242 2022-12-15 17:55:21.000000 gradescope_mean-0.0.8/gradescope_mean/plot.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-04-26 17:43:47.154263 gradescope_mean-0.0.8/gradescope_mean.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)     4313 2023-04-26 17:43:47.000000 gradescope_mean-0.0.8/gradescope_mean.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)      803 2023-04-26 17:43:47.000000 gradescope_mean-0.0.8/gradescope_mean.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-04-26 17:43:47.000000 gradescope_mean-0.0.8/gradescope_mean.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       34 2023-04-26 17:43:47.000000 gradescope_mean-0.0.8/gradescope_mean.egg-info/requires.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       16 2023-04-26 17:43:47.000000 gradescope_mean-0.0.8/gradescope_mean.egg-info/top_level.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)      704 2023-04-26 17:43:19.000000 gradescope_mean-0.0.8/pyproject.toml
--rw-rw-r--   0 matt      (1000) matt      (1000)       38 2023-04-26 17:43:47.158263 gradescope_mean-0.0.8/setup.cfg
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-04-26 17:43:47.158263 gradescope_mean-0.0.8/test/
--rw-rw-r--   0 matt      (1000) matt      (1000)      846 2023-04-25 16:34:44.000000 gradescope_mean-0.0.8/test/test_assign_list.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      296 2023-04-25 16:34:44.000000 gradescope_mean-0.0.8/test/test_config.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1311 2022-05-09 19:40:21.000000 gradescope_mean-0.0.8/test/test_get_mean_drop_low.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     6225 2023-04-25 16:34:44.000000 gradescope_mean-0.0.8/test/test_gradebook.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      927 2022-12-15 17:55:21.000000 gradescope_mean-0.0.8/test/test_perc_to_letter.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-04-28 16:50:48.457888 gradescope_mean-0.0.9/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1068 2022-05-09 19:38:36.000000 gradescope_mean-0.0.9/LICENSE
+-rw-rw-r--   0 matt      (1000) matt      (1000)       40 2022-05-10 15:46:26.000000 gradescope_mean-0.0.9/MANIFEST.in
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4313 2023-04-28 16:50:48.457888 gradescope_mean-0.0.9/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2641 2023-04-25 16:34:44.000000 gradescope_mean-0.0.9/README.md
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-04-28 16:50:48.453888 gradescope_mean-0.0.9/gradescope_mean/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       89 2022-12-15 17:55:21.000000 gradescope_mean-0.0.9/gradescope_mean/__init__.py
+-rwxrwxr-x   0 matt      (1000) matt      (1000)     2486 2023-04-25 16:34:44.000000 gradescope_mean-0.0.9/gradescope_mean/__main__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1667 2023-04-25 16:34:44.000000 gradescope_mean-0.0.9/gradescope_mean/assign_list.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-04-28 16:50:48.453888 gradescope_mean-0.0.9/gradescope_mean/banner/
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-25 16:34:44.000000 gradescope_mean-0.0.9/gradescope_mean/banner/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1289 2023-04-28 16:50:17.000000 gradescope_mean-0.0.9/gradescope_mean/banner/__main__.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-04-28 16:50:48.453888 gradescope_mean-0.0.9/gradescope_mean/canvas/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       22 2023-04-25 16:34:44.000000 gradescope_mean-0.0.9/gradescope_mean/canvas/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1570 2023-04-28 16:50:17.000000 gradescope_mean-0.0.9/gradescope_mean/canvas/__main__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2619 2023-04-28 16:50:17.000000 gradescope_mean-0.0.9/gradescope_mean/canvas/canvas.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4384 2023-04-25 16:34:44.000000 gradescope_mean-0.0.9/gradescope_mean/config.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      321 2023-04-25 16:34:44.000000 gradescope_mean-0.0.9/gradescope_mean/config.yaml
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1431 2022-05-09 19:40:21.000000 gradescope_mean-0.0.9/gradescope_mean/get_mean_drop_low.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    15777 2023-04-25 16:47:18.000000 gradescope_mean-0.0.9/gradescope_mean/gradebook.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1441 2022-12-15 17:55:21.000000 gradescope_mean-0.0.9/gradescope_mean/perc_to_letter.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1242 2022-12-15 17:55:21.000000 gradescope_mean-0.0.9/gradescope_mean/plot.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-04-28 16:50:48.453888 gradescope_mean-0.0.9/gradescope_mean.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)     4313 2023-04-28 16:50:48.000000 gradescope_mean-0.0.9/gradescope_mean.egg-info/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)      803 2023-04-28 16:50:48.000000 gradescope_mean-0.0.9/gradescope_mean.egg-info/SOURCES.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-04-28 16:50:48.000000 gradescope_mean-0.0.9/gradescope_mean.egg-info/dependency_links.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       34 2023-04-28 16:50:48.000000 gradescope_mean-0.0.9/gradescope_mean.egg-info/requires.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       16 2023-04-28 16:50:48.000000 gradescope_mean-0.0.9/gradescope_mean.egg-info/top_level.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)      704 2023-04-28 16:50:26.000000 gradescope_mean-0.0.9/pyproject.toml
+-rw-rw-r--   0 matt      (1000) matt      (1000)       38 2023-04-28 16:50:48.457888 gradescope_mean-0.0.9/setup.cfg
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-04-28 16:50:48.457888 gradescope_mean-0.0.9/test/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      846 2023-04-25 16:34:44.000000 gradescope_mean-0.0.9/test/test_assign_list.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      296 2023-04-25 16:34:44.000000 gradescope_mean-0.0.9/test/test_config.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1311 2022-05-09 19:40:21.000000 gradescope_mean-0.0.9/test/test_get_mean_drop_low.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6225 2023-04-25 16:34:44.000000 gradescope_mean-0.0.9/test/test_gradebook.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      927 2022-12-15 17:55:21.000000 gradescope_mean-0.0.9/test/test_perc_to_letter.py
```

### Comparing `gradescope_mean-0.0.8/LICENSE` & `gradescope_mean-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.8/PKG-INFO` & `gradescope_mean-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradescope_mean
-Version: 0.0.8
+Version: 0.0.9
 Summary: utility to average gradescope csv output to final grades
 Author-email: Matt Higger <matt.higger@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 matt higger
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gradescope_mean-0.0.8/README.md` & `gradescope_mean-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.8/gradescope_mean/__main__.py` & `gradescope_mean-0.0.9/gradescope_mean/__main__.py`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.8/gradescope_mean/assign_list.py` & `gradescope_mean-0.0.9/gradescope_mean/assign_list.py`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.8/gradescope_mean/banner/__main__.py` & `gradescope_mean-0.0.9/gradescope_mean/banner/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -33,15 +33,8 @@
     # output csv
     timestamp = datetime.now().strftime('%b%d_%H%M')
     f_canvas_out = args.grade_full.replace('.csv', f'_banner_{timestamp}.xlsx')
     df.to_excel(f_canvas_out, index=False)
 
 
 if __name__ == '__main__':
-    from collections import namedtuple
-
-    folder = '/home/matt/Dropbox/teach/DS2500/admin/grades/'
-    Args = namedtuple('Args', ['grade_full', 'term_code', 'crn_list'])
-    args = Args(grade_full=folder + 'grade_full.csv',
-                term_code='asdf',
-                crn_list=['0', '1', '2'])
-    main(args)
+    main()
```

### Comparing `gradescope_mean-0.0.8/gradescope_mean/canvas/__main__.py` & `gradescope_mean-0.0.9/gradescope_mean/canvas/__main__.py`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.8/gradescope_mean/canvas/canvas.py` & `gradescope_mean-0.0.9/gradescope_mean/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.8/gradescope_mean/config.py` & `gradescope_mean-0.0.9/gradescope_mean/config.py`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.8/gradescope_mean/get_mean_drop_low.py` & `gradescope_mean-0.0.9/gradescope_mean/get_mean_drop_low.py`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.8/gradescope_mean/gradebook.py` & `gradescope_mean-0.0.9/gradescope_mean/gradebook.py`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.8/gradescope_mean/perc_to_letter.py` & `gradescope_mean-0.0.9/gradescope_mean/perc_to_letter.py`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.8/gradescope_mean/plot.py` & `gradescope_mean-0.0.9/gradescope_mean/plot.py`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.8/gradescope_mean.egg-info/PKG-INFO` & `gradescope_mean-0.0.9/gradescope_mean.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradescope-mean
-Version: 0.0.8
+Version: 0.0.9
 Summary: utility to average gradescope csv output to final grades
 Author-email: Matt Higger <matt.higger@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 matt higger
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gradescope_mean-0.0.8/gradescope_mean.egg-info/SOURCES.txt` & `gradescope_mean-0.0.9/gradescope_mean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.8/pyproject.toml` & `gradescope_mean-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gradescope_mean"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name = "Matt Higger", email = "matt.higger@gmail.com" },
 ]
 description = "utility to average gradescope csv output to final grades"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `gradescope_mean-0.0.8/test/test_assign_list.py` & `gradescope_mean-0.0.9/test/test_assign_list.py`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.8/test/test_get_mean_drop_low.py` & `gradescope_mean-0.0.9/test/test_get_mean_drop_low.py`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.8/test/test_gradebook.py` & `gradescope_mean-0.0.9/test/test_gradebook.py`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.8/test/test_perc_to_letter.py` & `gradescope_mean-0.0.9/test/test_perc_to_letter.py`

 * *Files identical despite different names*

