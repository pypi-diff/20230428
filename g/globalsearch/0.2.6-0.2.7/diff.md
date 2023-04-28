# Comparing `tmp/globalsearch-0.2.6.tar.gz` & `tmp/globalsearch-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globalsearch-0.2.6.tar", last modified: Thu Apr 27 19:57:05 2023, max compression
+gzip compressed data, was "globalsearch-0.2.7.tar", last modified: Fri Apr 28 21:20:44 2023, max compression
```

## Comparing `globalsearch-0.2.6.tar` & `globalsearch-0.2.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-27 19:57:05.046732 globalsearch-0.2.6/
--rw-r--r--   0 weiju      (501) staff       (20)      951 2023-04-27 19:57:05.046795 globalsearch-0.2.6/PKG-INFO
--rw-r--r--   0 weiju      (501) staff       (20)      252 2022-12-13 19:27:00.000000 globalsearch-0.2.6/README.md
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-27 19:57:05.042794 globalsearch-0.2.6/bin/
--rwxr--r--   0 weiju      (501) staff       (20)      533 2023-01-09 18:49:49.000000 globalsearch-0.2.6/bin/gs_prepare
--rwxr-xr-x   0 weiju      (501) staff       (20)     1268 2023-02-09 22:31:19.000000 globalsearch-0.2.6/bin/gs_submit
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-27 19:57:05.041982 globalsearch-0.2.6/globalsearch/
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-27 19:57:05.043912 globalsearch-0.2.6/globalsearch/control/
--rw-r--r--   0 weiju      (501) staff       (20)        0 2022-12-10 16:54:29.000000 globalsearch-0.2.6/globalsearch/control/__init__.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     6635 2023-02-24 18:56:53.000000 globalsearch-0.2.6/globalsearch/control/gs_prepare.py
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-27 19:57:05.046508 globalsearch-0.2.6/globalsearch/rnaseq/
--rw-r--r--   0 weiju      (501) staff       (20)        0 2022-12-09 00:21:15.000000 globalsearch-0.2.6/globalsearch/rnaseq/__init__.py
--rw-r--r--   0 weiju      (501) staff       (20)     7239 2023-04-18 20:14:08.000000 globalsearch-0.2.6/globalsearch/rnaseq/find_files.py
--rw-r--r--   0 weiju      (501) staff       (20)     2978 2023-04-07 20:18:38.000000 globalsearch-0.2.6/globalsearch/rnaseq/index_star.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     2130 2023-02-09 22:31:19.000000 globalsearch-0.2.6/globalsearch/rnaseq/make_kallisto_job.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     3120 2023-04-07 20:18:38.000000 globalsearch-0.2.6/globalsearch/rnaseq/make_star_idx_job.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     6330 2023-04-11 22:07:15.000000 globalsearch-0.2.6/globalsearch/rnaseq/make_star_salmon_job.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     1725 2023-04-13 18:08:53.000000 globalsearch-0.2.6/globalsearch/rnaseq/post_star_salmon.py
--rwxr--r--   0 weiju      (501) staff       (20)     5497 2023-01-06 20:10:59.000000 globalsearch-0.2.6/globalsearch/rnaseq/run_kallisto.py
--rw-r--r--   0 weiju      (501) staff       (20)    15368 2023-04-27 17:44:05.000000 globalsearch-0.2.6/globalsearch/rnaseq/run_spladder.py
--rwxr-xr-x   0 weiju      (501) staff       (20)    13271 2023-04-27 19:56:13.000000 globalsearch-0.2.6/globalsearch/rnaseq/run_star_salmon.py
--rw-r--r--   0 weiju      (501) staff       (20)     3662 2023-04-18 21:03:09.000000 globalsearch-0.2.6/globalsearch/rnaseq/trim_galore.py
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-27 19:57:05.043692 globalsearch-0.2.6/globalsearch.egg-info/
--rw-r--r--   0 weiju      (501) staff       (20)      951 2023-04-27 19:57:05.000000 globalsearch-0.2.6/globalsearch.egg-info/PKG-INFO
--rw-r--r--   0 weiju      (501) staff       (20)      751 2023-04-27 19:57:05.000000 globalsearch-0.2.6/globalsearch.egg-info/SOURCES.txt
--rw-r--r--   0 weiju      (501) staff       (20)        1 2023-04-27 19:57:05.000000 globalsearch-0.2.6/globalsearch.egg-info/dependency_links.txt
--rw-r--r--   0 weiju      (501) staff       (20)        1 2022-12-15 20:31:36.000000 globalsearch-0.2.6/globalsearch.egg-info/not-zip-safe
--rw-r--r--   0 weiju      (501) staff       (20)       25 2023-04-27 19:57:05.000000 globalsearch-0.2.6/globalsearch.egg-info/requires.txt
--rw-r--r--   0 weiju      (501) staff       (20)       13 2023-04-27 19:57:05.000000 globalsearch-0.2.6/globalsearch.egg-info/top_level.txt
--rw-r--r--   0 weiju      (501) staff       (20)       67 2023-04-27 19:57:05.047004 globalsearch-0.2.6/setup.cfg
--rw-r--r--   0 weiju      (501) staff       (20)     1611 2023-04-27 19:56:51.000000 globalsearch-0.2.6/setup.py
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-28 21:20:44.589296 globalsearch-0.2.7/
+-rw-r--r--   0 weiju      (501) staff       (20)      951 2023-04-28 21:20:44.589369 globalsearch-0.2.7/PKG-INFO
+-rw-r--r--   0 weiju      (501) staff       (20)      252 2022-12-13 19:27:00.000000 globalsearch-0.2.7/README.md
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-28 21:20:44.585356 globalsearch-0.2.7/bin/
+-rwxr--r--   0 weiju      (501) staff       (20)      533 2023-01-09 18:49:49.000000 globalsearch-0.2.7/bin/gs_prepare
+-rwxr-xr-x   0 weiju      (501) staff       (20)     1268 2023-02-09 22:31:19.000000 globalsearch-0.2.7/bin/gs_submit
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-28 21:20:44.584516 globalsearch-0.2.7/globalsearch/
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-28 21:20:44.586457 globalsearch-0.2.7/globalsearch/control/
+-rw-r--r--   0 weiju      (501) staff       (20)        0 2022-12-10 16:54:29.000000 globalsearch-0.2.7/globalsearch/control/__init__.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     6635 2023-02-24 18:56:53.000000 globalsearch-0.2.7/globalsearch/control/gs_prepare.py
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-28 21:20:44.589017 globalsearch-0.2.7/globalsearch/rnaseq/
+-rw-r--r--   0 weiju      (501) staff       (20)        0 2022-12-09 00:21:15.000000 globalsearch-0.2.7/globalsearch/rnaseq/__init__.py
+-rw-r--r--   0 weiju      (501) staff       (20)     7239 2023-04-18 20:14:08.000000 globalsearch-0.2.7/globalsearch/rnaseq/find_files.py
+-rw-r--r--   0 weiju      (501) staff       (20)     2978 2023-04-07 20:18:38.000000 globalsearch-0.2.7/globalsearch/rnaseq/index_star.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     2130 2023-02-09 22:31:19.000000 globalsearch-0.2.7/globalsearch/rnaseq/make_kallisto_job.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     3120 2023-04-07 20:18:38.000000 globalsearch-0.2.7/globalsearch/rnaseq/make_star_idx_job.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     6330 2023-04-11 22:07:15.000000 globalsearch-0.2.7/globalsearch/rnaseq/make_star_salmon_job.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     1725 2023-04-13 18:08:53.000000 globalsearch-0.2.7/globalsearch/rnaseq/post_star_salmon.py
+-rwxr--r--   0 weiju      (501) staff       (20)     5497 2023-01-06 20:10:59.000000 globalsearch-0.2.7/globalsearch/rnaseq/run_kallisto.py
+-rw-r--r--   0 weiju      (501) staff       (20)    15368 2023-04-27 17:44:05.000000 globalsearch-0.2.7/globalsearch/rnaseq/run_spladder.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)    13295 2023-04-28 21:18:42.000000 globalsearch-0.2.7/globalsearch/rnaseq/run_star_salmon.py
+-rw-r--r--   0 weiju      (501) staff       (20)     3662 2023-04-18 21:03:09.000000 globalsearch-0.2.7/globalsearch/rnaseq/trim_galore.py
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-28 21:20:44.586244 globalsearch-0.2.7/globalsearch.egg-info/
+-rw-r--r--   0 weiju      (501) staff       (20)      951 2023-04-28 21:20:44.000000 globalsearch-0.2.7/globalsearch.egg-info/PKG-INFO
+-rw-r--r--   0 weiju      (501) staff       (20)      751 2023-04-28 21:20:44.000000 globalsearch-0.2.7/globalsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 weiju      (501) staff       (20)        1 2023-04-28 21:20:44.000000 globalsearch-0.2.7/globalsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 weiju      (501) staff       (20)        1 2022-12-15 20:31:36.000000 globalsearch-0.2.7/globalsearch.egg-info/not-zip-safe
+-rw-r--r--   0 weiju      (501) staff       (20)       25 2023-04-28 21:20:44.000000 globalsearch-0.2.7/globalsearch.egg-info/requires.txt
+-rw-r--r--   0 weiju      (501) staff       (20)       13 2023-04-28 21:20:44.000000 globalsearch-0.2.7/globalsearch.egg-info/top_level.txt
+-rw-r--r--   0 weiju      (501) staff       (20)       67 2023-04-28 21:20:44.589591 globalsearch-0.2.7/setup.cfg
+-rw-r--r--   0 weiju      (501) staff       (20)     1611 2023-04-28 21:20:06.000000 globalsearch-0.2.7/setup.py
```

### Comparing `globalsearch-0.2.6/PKG-INFO` & `globalsearch-0.2.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globalsearch
-Version: 0.2.6
+Version: 0.2.7
 Summary: globalsearch is a collection of Python modules and command tools for the Global Search pipeline.
 Home-page: https://github.com/baliga-lab/Global_Search
 Author: Wei-ju Wu
 Author-email: weiju.wu@gmail.com
 Maintainer: Wei-ju Wu
 Maintainer-email: weiju.wu@gmail.com
 License: LGPL V3
```

### Comparing `globalsearch-0.2.6/bin/gs_prepare` & `globalsearch-0.2.7/bin/gs_prepare`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.6/bin/gs_submit` & `globalsearch-0.2.7/bin/gs_submit`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.6/globalsearch/control/gs_prepare.py` & `globalsearch-0.2.7/globalsearch/control/gs_prepare.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.6/globalsearch/rnaseq/find_files.py` & `globalsearch-0.2.7/globalsearch/rnaseq/find_files.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.6/globalsearch/rnaseq/index_star.py` & `globalsearch-0.2.7/globalsearch/rnaseq/index_star.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.6/globalsearch/rnaseq/make_kallisto_job.py` & `globalsearch-0.2.7/globalsearch/rnaseq/make_kallisto_job.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.6/globalsearch/rnaseq/make_star_idx_job.py` & `globalsearch-0.2.7/globalsearch/rnaseq/make_star_idx_job.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.6/globalsearch/rnaseq/make_star_salmon_job.py` & `globalsearch-0.2.7/globalsearch/rnaseq/make_star_salmon_job.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.6/globalsearch/rnaseq/post_star_salmon.py` & `globalsearch-0.2.7/globalsearch/rnaseq/post_star_salmon.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.6/globalsearch/rnaseq/run_kallisto.py` & `globalsearch-0.2.7/globalsearch/rnaseq/run_kallisto.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.6/globalsearch/rnaseq/run_spladder.py` & `globalsearch-0.2.7/globalsearch/rnaseq/run_spladder.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.6/globalsearch/rnaseq/run_star_salmon.py` & `globalsearch-0.2.7/globalsearch/rnaseq/run_star_salmon.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,19 +112,19 @@
     ## STAR based BAM duplicate removal
     # Mark duplicates with STAR
     print('STAR mark duplicates run command:%s' % star_markdup_cmd, flush=True)
     compl_proc = subprocess.run(star_markdup_command, check=True, capture_output=False, cwd=results_dir)
 
     # Remove marked duplicates withh samtools
     print('Samtools  STAR Dedup Remove run command:%s' % rmsingletonsSTAR_cmd, flush=True)
-    compl_proc = subprocess.run(rmsingletonsSTAR_cmd, check=True, capture_output=False, cwd=results_dir)
+    compl_proc = subprocess.run(rmsingletonsSTAR_cmd, shell=True, check=True, capture_output=False, cwd=results_dir)
 
     # Remove marked duplicates withh samtools
     print('Samtools  Collate reads by read name run command:%s' % collatereadsSTAR_cmd, flush=True)
-    compl_proc = subprocess.run(collatereadsSTAR_cmd, check=True, capture_output=False, cwd=results_dir)
+    compl_proc = subprocess.run(collatereadsSTAR_cmd, shell=True, check=True, capture_output=False, cwd=results_dir)
 
 
 ####################### Run Salmon Count ###############################
 # WW: Check the names of the input files they will be different from _out
 def run_salmon_quant(results_dir, folder_name, genome_fasta):
     outfile_prefix = '%s/%s_%s_' %(results_dir, folder_name, args.starPrefix)
     print(outfile_prefix, flush=True)
```

### Comparing `globalsearch-0.2.6/globalsearch/rnaseq/trim_galore.py` & `globalsearch-0.2.7/globalsearch/rnaseq/trim_galore.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.6/globalsearch.egg-info/PKG-INFO` & `globalsearch-0.2.7/globalsearch.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globalsearch
-Version: 0.2.6
+Version: 0.2.7
 Summary: globalsearch is a collection of Python modules and command tools for the Global Search pipeline.
 Home-page: https://github.com/baliga-lab/Global_Search
 Author: Wei-ju Wu
 Author-email: weiju.wu@gmail.com
 Maintainer: Wei-ju Wu
 Maintainer-email: weiju.wu@gmail.com
 License: LGPL V3
```

### Comparing `globalsearch-0.2.6/globalsearch.egg-info/SOURCES.txt` & `globalsearch-0.2.7/globalsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.6/setup.py` & `globalsearch-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 NAME = 'globalsearch'
 PACKAGES = ['globalsearch.rnaseq', 'globalsearch.control']
 DESCRIPTION = 'globalsearch is a collection of Python modules and command tools for the Global Search pipeline.'
 LICENSE = 'LGPL V3'
 URI = 'https://github.com/baliga-lab/Global_Search'
 AUTHOR = 'Wei-ju Wu'
-VERSION = '0.2.6'
+VERSION = '0.2.7'
 
 KEYWORDS = ['global search', 'coral reef']
 
 # See trove classifiers
 # https://testpypi.python.org/pypi?%3Aaction=list_classifiers
 
 CLASSIFIERS = [
```

