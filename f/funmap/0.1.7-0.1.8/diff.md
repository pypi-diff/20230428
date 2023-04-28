# Comparing `tmp/funmap-0.1.7.tar.gz` & `tmp/funmap-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/funmap-0.1.7.tar", last modified: Tue Feb 28 21:47:13 2023, max compression
+gzip compressed data, was "dist/funmap-0.1.8.tar", last modified: Fri Apr 28 17:44:10 2023, max compression
```

## Comparing `funmap-0.1.7.tar` & `funmap-0.1.8.tar`

### file list

```diff
@@ -1,50 +1,28 @@
-drwxr-xr-x   0 shiz       (501) staff       (20)        0 2023-02-28 21:47:13.000000 funmap-0.1.7/
--rw-r--r--   0 shiz       (501) staff       (20)      154 2022-12-19 18:14:17.000000 funmap-0.1.7/AUTHORS.rst
--rw-r--r--   0 shiz       (501) staff       (20)     3506 2022-12-19 18:14:17.000000 funmap-0.1.7/CONTRIBUTING.rst
--rw-r--r--   0 shiz       (501) staff       (20)       89 2022-12-19 18:14:17.000000 funmap-0.1.7/HISTORY.rst
--rw-r--r--   0 shiz       (501) staff       (20)     1068 2022-12-19 18:14:17.000000 funmap-0.1.7/LICENSE
--rw-r--r--   0 shiz       (501) staff       (20)      324 2022-12-20 21:45:22.000000 funmap-0.1.7/MANIFEST.in
--rw-r--r--   0 shiz       (501) staff       (20)      627 2023-02-28 21:47:13.000000 funmap-0.1.7/PKG-INFO
--rw-r--r--   0 shiz       (501) staff       (20)      182 2023-01-19 17:59:39.000000 funmap-0.1.7/README.rst
-drwxr-xr-x   0 shiz       (501) staff       (20)        0 2023-02-28 21:47:13.000000 funmap-0.1.7/docs/
--rw-r--r--   0 shiz       (501) staff       (20)      607 2022-12-19 18:14:17.000000 funmap-0.1.7/docs/Makefile
--rw-r--r--   0 shiz       (501) staff       (20)       28 2022-12-19 18:14:17.000000 funmap-0.1.7/docs/authors.rst
--rwxr-xr-x   0 shiz       (501) staff       (20)     4756 2022-12-19 18:14:17.000000 funmap-0.1.7/docs/conf.py
--rw-r--r--   0 shiz       (501) staff       (20)       33 2022-12-19 18:14:17.000000 funmap-0.1.7/docs/contributing.rst
--rw-r--r--   0 shiz       (501) staff       (20)       28 2022-12-19 18:14:17.000000 funmap-0.1.7/docs/history.rst
--rw-r--r--   0 shiz       (501) staff       (20)      303 2022-12-19 18:14:17.000000 funmap-0.1.7/docs/index.rst
--rw-r--r--   0 shiz       (501) staff       (20)     1098 2022-12-19 18:14:17.000000 funmap-0.1.7/docs/installation.rst
--rw-r--r--   0 shiz       (501) staff       (20)      804 2022-12-19 18:14:17.000000 funmap-0.1.7/docs/make.bat
--rw-r--r--   0 shiz       (501) staff       (20)       27 2022-12-19 18:14:17.000000 funmap-0.1.7/docs/readme.rst
--rw-r--r--   0 shiz       (501) staff       (20)       67 2022-12-19 18:14:17.000000 funmap-0.1.7/docs/usage.rst
-drwxr-xr-x   0 shiz       (501) staff       (20)        0 2023-02-28 21:47:13.000000 funmap-0.1.7/funmap/
--rw-r--r--   0 shiz       (501) staff       (20)      122 2023-02-28 21:46:46.000000 funmap-0.1.7/funmap/__init__.py
--rw-r--r--   0 shiz       (501) staff       (20)    10866 2023-02-27 23:08:32.000000 funmap-0.1.7/funmap/cli.py
--rw-r--r--   0 shiz       (501) staff       (20)      689 2023-02-20 16:05:59.000000 funmap-0.1.7/funmap/data_urls.py
--rw-r--r--   0 shiz       (501) staff       (20)    39323 2023-02-27 21:55:57.000000 funmap-0.1.7/funmap/funmap.py
--rw-r--r--   0 shiz       (501) staff       (20)    32364 2023-02-27 23:13:45.000000 funmap-0.1.7/funmap/plotting.py
--rw-r--r--   0 shiz       (501) staff       (20)     9565 2023-02-23 17:00:43.000000 funmap-0.1.7/funmap/utils.py
-drwxr-xr-x   0 shiz       (501) staff       (20)        0 2023-02-28 21:47:13.000000 funmap-0.1.7/funmap.egg-info/
--rw-r--r--   0 shiz       (501) staff       (20)      627 2023-02-28 21:47:13.000000 funmap-0.1.7/funmap.egg-info/PKG-INFO
--rw-r--r--   0 shiz       (501) staff       (20)      896 2023-02-28 21:47:13.000000 funmap-0.1.7/funmap.egg-info/SOURCES.txt
--rw-r--r--   0 shiz       (501) staff       (20)        1 2023-02-28 21:47:13.000000 funmap-0.1.7/funmap.egg-info/dependency_links.txt
--rw-r--r--   0 shiz       (501) staff       (20)       43 2023-02-28 21:47:13.000000 funmap-0.1.7/funmap.egg-info/entry_points.txt
--rw-r--r--   0 shiz       (501) staff       (20)        1 2023-02-28 21:47:13.000000 funmap-0.1.7/funmap.egg-info/not-zip-safe
--rw-r--r--   0 shiz       (501) staff       (20)      136 2023-02-28 21:47:13.000000 funmap-0.1.7/funmap.egg-info/requires.txt
--rw-r--r--   0 shiz       (501) staff       (20)        7 2023-02-28 21:47:13.000000 funmap-0.1.7/funmap.egg-info/top_level.txt
--rw-r--r--   0 shiz       (501) staff       (20)      378 2023-02-28 21:47:13.000000 funmap-0.1.7/setup.cfg
--rw-r--r--   0 shiz       (501) staff       (20)     1251 2023-02-28 21:46:46.000000 funmap-0.1.7/setup.py
-drwxr-xr-x   0 shiz       (501) staff       (20)        0 2023-02-28 21:47:13.000000 funmap-0.1.7/tests/
--rw-r--r--   0 shiz       (501) staff       (20)       36 2022-12-19 18:14:17.000000 funmap-0.1.7/tests/__init__.py
-drwxr-xr-x   0 shiz       (501) staff       (20)        0 2023-02-28 21:47:13.000000 funmap-0.1.7/tests/aml_test/
--rw-r--r--   0 shiz       (501) staff       (20)  1678897 2022-12-23 15:29:01.000000 funmap-0.1.7/tests/aml_test/BeatAMl-T.tsv
--rw-r--r--   0 shiz       (501) staff       (20)   265203 2022-12-23 15:29:25.000000 funmap-0.1.7/tests/aml_test/Blood2022-P-T.tsv
--rw-r--r--   0 shiz       (501) staff       (20)    98926 2022-12-23 15:29:42.000000 funmap-0.1.7/tests/aml_test/CCLE-P-T.tsv
--rw-r--r--   0 shiz       (501) staff       (20)   117878 2022-12-23 15:30:00.000000 funmap-0.1.7/tests/aml_test/CCLE-T.tsv
--rw-r--r--   0 shiz       (501) staff       (20)   966047 2022-12-23 15:21:18.000000 funmap-0.1.7/tests/aml_test/ClinseqAML-T.tsv
--rw-r--r--   0 shiz       (501) staff       (20)  1476458 2022-12-23 15:30:43.000000 funmap-0.1.7/tests/aml_test/TCGA_2013-T.tsv
--rw-r--r--   0 shiz       (501) staff       (20)    56410 2022-12-23 15:31:04.000000 funmap-0.1.7/tests/aml_test/target-C.tsv
--rw-r--r--   0 shiz       (501) staff       (20)  1177971 2022-12-23 15:31:19.000000 funmap-0.1.7/tests/aml_test/target-N.tsv
--rw-r--r--   0 shiz       (501) staff       (20)  7021776 2022-12-23 15:44:55.000000 funmap-0.1.7/tests/aml_test/target-T.tsv
--rw-r--r--   0 shiz       (501) staff       (20)      234 2023-01-17 23:46:31.000000 funmap-0.1.7/tests/test_config.yaml
--rw-r--r--   0 shiz       (501) staff       (20)      685 2023-01-17 23:50:36.000000 funmap-0.1.7/tests/test_data.yaml
+drwxr-xr-x   0 shiz       (501) staff       (20)        0 2023-04-28 17:44:10.000000 funmap-0.1.8/
+-rw-r--r--   0 shiz       (501) staff       (20)      154 2022-12-19 18:14:17.000000 funmap-0.1.8/AUTHORS.rst
+-rw-r--r--   0 shiz       (501) staff       (20)     3506 2022-12-19 18:14:17.000000 funmap-0.1.8/CONTRIBUTING.rst
+-rw-r--r--   0 shiz       (501) staff       (20)       89 2022-12-19 18:14:17.000000 funmap-0.1.8/HISTORY.rst
+-rw-r--r--   0 shiz       (501) staff       (20)     1068 2022-12-19 18:14:17.000000 funmap-0.1.8/LICENSE
+-rw-r--r--   0 shiz       (501) staff       (20)      324 2022-12-20 21:45:22.000000 funmap-0.1.8/MANIFEST.in
+-rw-r--r--   0 shiz       (501) staff       (20)      445 2023-04-28 17:44:10.000000 funmap-0.1.8/PKG-INFO
+-rw-r--r--   0 shiz       (501) staff       (20)     2242 2023-04-28 17:31:56.000000 funmap-0.1.8/README.md
+drwxr-xr-x   0 shiz       (501) staff       (20)        0 2023-04-28 17:44:10.000000 funmap-0.1.8/funmap/
+-rw-r--r--   0 shiz       (501) staff       (20)      122 2023-04-28 17:35:30.000000 funmap-0.1.8/funmap/__init__.py
+-rw-r--r--   0 shiz       (501) staff       (20)    10866 2023-03-22 21:50:52.000000 funmap-0.1.8/funmap/cli.py
+-rw-r--r--   0 shiz       (501) staff       (20)      689 2023-02-20 16:05:59.000000 funmap-0.1.8/funmap/data_urls.py
+-rw-r--r--   0 shiz       (501) staff       (20)    39323 2023-03-20 19:49:55.000000 funmap-0.1.8/funmap/funmap.py
+-rw-r--r--   0 shiz       (501) staff       (20)    32364 2023-03-22 21:50:52.000000 funmap-0.1.8/funmap/plotting.py
+-rw-r--r--   0 shiz       (501) staff       (20)     9565 2023-03-22 21:50:52.000000 funmap-0.1.8/funmap/utils.py
+drwxr-xr-x   0 shiz       (501) staff       (20)        0 2023-04-28 17:44:10.000000 funmap-0.1.8/funmap.egg-info/
+-rw-r--r--   0 shiz       (501) staff       (20)      445 2023-04-28 17:44:10.000000 funmap-0.1.8/funmap.egg-info/PKG-INFO
+-rw-r--r--   0 shiz       (501) staff       (20)      447 2023-04-28 17:44:10.000000 funmap-0.1.8/funmap.egg-info/SOURCES.txt
+-rw-r--r--   0 shiz       (501) staff       (20)        1 2023-04-28 17:44:10.000000 funmap-0.1.8/funmap.egg-info/dependency_links.txt
+-rw-r--r--   0 shiz       (501) staff       (20)       43 2023-04-28 17:44:10.000000 funmap-0.1.8/funmap.egg-info/entry_points.txt
+-rw-r--r--   0 shiz       (501) staff       (20)        1 2023-04-28 17:44:10.000000 funmap-0.1.8/funmap.egg-info/not-zip-safe
+-rw-r--r--   0 shiz       (501) staff       (20)      136 2023-04-28 17:44:10.000000 funmap-0.1.8/funmap.egg-info/requires.txt
+-rw-r--r--   0 shiz       (501) staff       (20)        7 2023-04-28 17:44:10.000000 funmap-0.1.8/funmap.egg-info/top_level.txt
+-rw-r--r--   0 shiz       (501) staff       (20)      378 2023-04-28 17:44:10.000000 funmap-0.1.8/setup.cfg
+-rw-r--r--   0 shiz       (501) staff       (20)     1169 2023-04-28 17:43:15.000000 funmap-0.1.8/setup.py
+drwxr-xr-x   0 shiz       (501) staff       (20)        0 2023-04-28 17:44:10.000000 funmap-0.1.8/tests/
+-rw-r--r--   0 shiz       (501) staff       (20)  4123534 2023-04-28 16:40:03.000000 funmap-0.1.8/tests/aml_test.tgz
+-rw-r--r--   0 shiz       (501) staff       (20)      932 2023-04-28 17:01:34.000000 funmap-0.1.8/tests/test_config.yaml
```

### Comparing `funmap-0.1.7/CONTRIBUTING.rst` & `funmap-0.1.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `funmap-0.1.7/LICENSE` & `funmap-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `funmap-0.1.7/funmap/cli.py` & `funmap-0.1.8/funmap/cli.py`

 * *Files identical despite different names*

### Comparing `funmap-0.1.7/funmap/data_urls.py` & `funmap-0.1.8/funmap/data_urls.py`

 * *Files identical despite different names*

### Comparing `funmap-0.1.7/funmap/funmap.py` & `funmap-0.1.8/funmap/funmap.py`

 * *Files identical despite different names*

### Comparing `funmap-0.1.7/funmap/plotting.py` & `funmap-0.1.8/funmap/plotting.py`

 * *Files identical despite different names*

### Comparing `funmap-0.1.7/funmap/utils.py` & `funmap-0.1.8/funmap/utils.py`

 * *Files identical despite different names*

### Comparing `funmap-0.1.7/setup.py` & `funmap-0.1.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #!/usr/bin/env python
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
-with open('README.rst') as readme_file:
-    readme = readme_file.read()
-
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 requirements = [
     'pyyaml',
     'xgboost',
     'numpy',
@@ -39,18 +36,18 @@
     entry_points={
         'console_scripts': [
             'funmap=funmap.cli:main',
         ],
     },
     install_requires=requirements,
     license='MIT license',
-    long_description=readme + '\n\n' + history,
+    long_description='\n\n' + history,
     include_package_data=True,
     keywords=['funmap', 'bioinformatics', 'biological-network'],
     name='funmap',
     packages=find_packages(include=['funmap', 'funmap.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/bzhanglab/funmap',
-    version='0.1.7',
+    version='0.1.8',
     zip_safe=False,
 )
```

