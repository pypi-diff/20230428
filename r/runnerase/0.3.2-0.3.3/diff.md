# Comparing `tmp/runnerase-0.3.2.tar.gz` & `tmp/runnerase-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runnerase-0.3.2.tar", last modified: Wed Apr 26 07:26:55 2023, max compression
+gzip compressed data, was "runnerase-0.3.3.tar", last modified: Fri Apr 28 13:12:32 2023, max compression
```

## Comparing `runnerase-0.3.2.tar` & `runnerase-0.3.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:26:55.120911 runnerase-0.3.2/
--rw-rw-rw-   0 root         (0) root         (0)    34575 2023-04-26 07:26:07.000000 runnerase-0.3.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-04-26 07:26:07.000000 runnerase-0.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2650 2023-04-26 07:26:55.120911 runnerase-0.3.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1565 2023-04-26 07:26:07.000000 runnerase-0.3.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1565 2023-04-26 07:26:07.000000 runnerase-0.3.2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:26:55.110911 runnerase-0.3.2/runnerase/
--rw-rw-rw-   0 root         (0) root         (0)      962 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21056 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/calculator.py
--rw-rw-rw-   0 root         (0) root         (0)     5182 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/defaultoptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:26:55.114911 runnerase-0.3.2/runnerase/io/
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11431 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/io/ase.py
--rw-rw-rw-   0 root         (0) root         (0)     7605 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/io/runnerconfig.py
--rw-rw-rw-   0 root         (0) root         (0)     5457 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/io/storageclasses.py
--rw-rw-rw-   0 root         (0) root         (0)    16947 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/io/structuredata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:26:55.117911 runnerase-0.3.2/runnerase/plot/
--rw-rw-rw-   0 root         (0) root         (0)      536 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21605 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/calculator.py
--rw-rw-rw-   0 root         (0) root         (0)     4132 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/fitresults.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:26:55.120911 runnerase-0.3.2/runnerase/plot/mpl_styles/
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/mpl_styles/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/mpl_styles/bar.mplstyle
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/mpl_styles/hist.mplstyle
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/mpl_styles/line.mplstyle
--rw-rw-rw-   0 root         (0) root         (0)     1168 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/mpl_styles/paper.mplstyle
--rw-rw-rw-   0 root         (0) root         (0)      339 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/mpl_styles/presentation.mplstyle
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/mpl_styles/scatterplot.mplstyle
--rw-rw-rw-   0 root         (0) root         (0)     2466 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/scaling.py
--rw-rw-rw-   0 root         (0) root         (0)     2675 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     6585 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/sfvalues.py
--rw-rw-rw-   0 root         (0) root         (0)     1710 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/splittraintest.py
--rw-rw-rw-   0 root         (0) root         (0)     8659 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/symmetryfunctions.py
--rw-rw-rw-   0 root         (0) root         (0)     1746 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/weights.py
--rw-rw-rw-   0 root         (0) root         (0)     1491 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/singlepoint.py
--rw-rw-rw-   0 root         (0) root         (0)    31089 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/storageclasses.py
--rw-rw-rw-   0 root         (0) root         (0)    28833 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/symmetryfunctions.py
--rw-rw-rw-   0 root         (0) root         (0)     4238 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:26:55.112911 runnerase-0.3.2/runnerase.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2650 2023-04-26 07:26:55.000000 runnerase-0.3.2/runnerase.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1114 2023-04-26 07:26:55.000000 runnerase-0.3.2/runnerase.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 07:26:55.000000 runnerase-0.3.2/runnerase.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      276 2023-04-26 07:26:55.000000 runnerase-0.3.2/runnerase.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-26 07:26:55.000000 runnerase-0.3.2/runnerase.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      226 2023-04-26 07:26:55.121911 runnerase-0.3.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      406 2023-04-26 07:26:07.000000 runnerase-0.3.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:26:55.120911 runnerase-0.3.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3117 2023-04-26 07:26:07.000000 runnerase-0.3.2/tests/test_functional.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:12:32.743425 runnerase-0.3.3/
+-rw-rw-rw-   0 root         (0) root         (0)    34575 2023-04-28 13:11:42.000000 runnerase-0.3.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-04-28 13:11:42.000000 runnerase-0.3.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-04-28 13:12:32.743425 runnerase-0.3.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1565 2023-04-28 13:11:42.000000 runnerase-0.3.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1591 2023-04-28 13:11:42.000000 runnerase-0.3.3/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:12:32.732424 runnerase-0.3.3/runnerase/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21056 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/calculator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5182 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/defaultoptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:12:32.736424 runnerase-0.3.3/runnerase/io/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11431 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/io/ase.py
+-rw-rw-rw-   0 root         (0) root         (0)     7605 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/io/runnerconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     5457 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/io/storageclasses.py
+-rw-rw-rw-   0 root         (0) root         (0)    17060 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/io/structuredata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:12:32.739425 runnerase-0.3.3/runnerase/plot/
+-rw-rw-rw-   0 root         (0) root         (0)      536 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/plot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21605 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/plot/calculator.py
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/plot/fitresults.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:12:32.742425 runnerase-0.3.3/runnerase/plot/mpl_styles/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/plot/mpl_styles/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/plot/mpl_styles/bar.mplstyle
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/plot/mpl_styles/hist.mplstyle
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/plot/mpl_styles/line.mplstyle
+-rw-rw-rw-   0 root         (0) root         (0)     1168 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/plot/mpl_styles/paper.mplstyle
+-rw-rw-rw-   0 root         (0) root         (0)      339 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/plot/mpl_styles/presentation.mplstyle
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/plot/mpl_styles/scatterplot.mplstyle
+-rw-rw-rw-   0 root         (0) root         (0)     2466 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/plot/scaling.py
+-rw-rw-rw-   0 root         (0) root         (0)     2675 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/plot/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    11329 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/plot/sfvalues.py
+-rw-rw-rw-   0 root         (0) root         (0)     1710 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/plot/splittraintest.py
+-rw-rw-rw-   0 root         (0) root         (0)     8659 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/plot/symmetryfunctions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1746 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/plot/weights.py
+-rw-rw-rw-   0 root         (0) root         (0)     1491 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/singlepoint.py
+-rw-rw-rw-   0 root         (0) root         (0)    31089 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/storageclasses.py
+-rw-rw-rw-   0 root         (0) root         (0)    28833 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/symmetryfunctions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4238 2023-04-28 13:11:42.000000 runnerase-0.3.3/runnerase/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:12:32.734424 runnerase-0.3.3/runnerase.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-04-28 13:12:32.000000 runnerase-0.3.3/runnerase.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1114 2023-04-28 13:12:32.000000 runnerase-0.3.3/runnerase.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 13:12:32.000000 runnerase-0.3.3/runnerase.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      296 2023-04-28 13:12:32.000000 runnerase-0.3.3/runnerase.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-28 13:12:32.000000 runnerase-0.3.3/runnerase.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      226 2023-04-28 13:12:32.743425 runnerase-0.3.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      406 2023-04-28 13:11:42.000000 runnerase-0.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:12:32.742425 runnerase-0.3.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3117 2023-04-28 13:11:42.000000 runnerase-0.3.3/tests/test_functional.py
```

### Comparing `runnerase-0.3.2/LICENSE` & `runnerase-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.2/PKG-INFO` & `runnerase-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runnerase
-Version: 0.3.2
+Version: 0.3.3
 Summary: An Interface between the Runner Neural Network Energy Representation (RuNNer) and the Atomic Simulation Environment (ASE).
 Author-email: Alexander Knoll <alexknoll@mailbox.org>
 Maintainer-email: Alexander Knoll <alexknoll@mailbox.org>
 License: GPLv3+
 Project-URL: Source, https://gitlab.com/runner-suite/runnerase
 Project-URL: Bugs, https://gitlab.com/runner-suite/runnerase/issues
 Project-URL: Documentation, https://runner-suite.gitlab.com/runnerase
```

### Comparing `runnerase-0.3.2/README.md` & `runnerase-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.2/pyproject.toml` & `runnerase-0.3.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ['setuptools', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 
 [project]
 name = 'runnerase'
-version = '0.3.2'
+version = '0.3.3'
 description = 'An Interface between the Runner Neural Network Energy Representation (RuNNer) and the Atomic Simulation Environment (ASE).'
 authors = [
     {name='Alexander Knoll', email='alexknoll@mailbox.org'}
 ]
 maintainers = [
     {name='Alexander Knoll', email='alexknoll@mailbox.org'}
 ]
@@ -33,14 +33,15 @@
     'Typing :: Typed'
 ]
 
 requires-python = '>=3.6'
 dependencies = [
     'numpy>=1.17.0',
     'ase>=3.19.0',
+    'scikit-learn>=1.2.0'
 ]
 
 
 [project.urls]
 Source = 'https://gitlab.com/runner-suite/runnerase'
 Bugs = 'https://gitlab.com/runner-suite/runnerase/issues'
 Documentation = "https://runner-suite.gitlab.com/runnerase"
```

### Comparing `runnerase-0.3.2/runnerase/__init__.py` & `runnerase-0.3.3/runnerase/__init__.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.2/runnerase/calculator.py` & `runnerase-0.3.3/runnerase/calculator.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.2/runnerase/defaultoptions.py` & `runnerase-0.3.3/runnerase/defaultoptions.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.2/runnerase/io/ase.py` & `runnerase-0.3.3/runnerase/io/ase.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.2/runnerase/io/runnerconfig.py` & `runnerase-0.3.3/runnerase/io/runnerconfig.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.2/runnerase/io/storageclasses.py` & `runnerase-0.3.3/runnerase/io/storageclasses.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.2/runnerase/io/structuredata.py` & `runnerase-0.3.3/runnerase/io/structuredata.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,17 @@
         # Add the unit cell information.
         if any(self.pbc):
             atoms.set_cell(self.cell)
 
         atoms.set_initial_charges(self.charges)
         atoms.set_initial_magnetic_moments(self.magmoms)
 
+        if np.isnan(self.totalcharge):
+            self.totalcharge = 0.0
+
         calc = RunnerSinglePointCalculator(
             atoms,
             energy=self.energy,
             forces=self.forces,
             totalcharge=self.totalcharge
         )
 
@@ -298,14 +301,17 @@
             outfile.write(f'atom {xyz[0]:{fmt}} {xyz[1]:{fmt}} {xyz[2]:{fmt}} '
                           f'{element:2s} {charge:{fmt}} {atomenergy:{fmt}} '
                           f'{force_xyz[0]:{fmt}} {force_xyz[1]:{fmt}} '
                           f'{force_xyz[2]:{fmt}}\n')
 
         # Write the energy and total charge, then end this structure.
         outfile.write(f'energy {tempatoms.energy:{fmt}}\n')
+
+        tempatoms.totalcharge = 0.0
+
         outfile.write(f'charge {tempatoms.totalcharge:{fmt}}\n')
         outfile.write('end\n')
 
 
 @writer
 def write_trainteststruct(
     outfile: TextIO,
```

### Comparing `runnerase-0.3.2/runnerase/plot/__init__.py` & `runnerase-0.3.3/runnerase/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.2/runnerase/plot/calculator.py` & `runnerase-0.3.3/runnerase/plot/calculator.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.2/runnerase/plot/fitresults.py` & `runnerase-0.3.3/runnerase/plot/fitresults.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.2/runnerase/plot/mpl_styles/paper.mplstyle` & `runnerase-0.3.3/runnerase/plot/mpl_styles/paper.mplstyle`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.2/runnerase/plot/scaling.py` & `runnerase-0.3.3/runnerase/plot/scaling.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.2/runnerase/plot/setup.py` & `runnerase-0.3.3/runnerase/plot/setup.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.2/runnerase/plot/splittraintest.py` & `runnerase-0.3.3/runnerase/plot/splittraintest.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.2/runnerase/plot/symmetryfunctions.py` & `runnerase-0.3.3/runnerase/plot/symmetryfunctions.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.2/runnerase/plot/weights.py` & `runnerase-0.3.3/runnerase/plot/weights.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.2/runnerase/singlepoint.py` & `runnerase-0.3.3/runnerase/singlepoint.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.2/runnerase/storageclasses.py` & `runnerase-0.3.3/runnerase/storageclasses.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.2/runnerase/symmetryfunctions.py` & `runnerase-0.3.3/runnerase/symmetryfunctions.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.2/runnerase/utils.py` & `runnerase-0.3.3/runnerase/utils.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.2/runnerase.egg-info/PKG-INFO` & `runnerase-0.3.3/runnerase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runnerase
-Version: 0.3.2
+Version: 0.3.3
 Summary: An Interface between the Runner Neural Network Energy Representation (RuNNer) and the Atomic Simulation Environment (ASE).
 Author-email: Alexander Knoll <alexknoll@mailbox.org>
 Maintainer-email: Alexander Knoll <alexknoll@mailbox.org>
 License: GPLv3+
 Project-URL: Source, https://gitlab.com/runner-suite/runnerase
 Project-URL: Bugs, https://gitlab.com/runner-suite/runnerase/issues
 Project-URL: Documentation, https://runner-suite.gitlab.com/runnerase
```

### Comparing `runnerase-0.3.2/runnerase.egg-info/SOURCES.txt` & `runnerase-0.3.3/runnerase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.2/tests/test_functional.py` & `runnerase-0.3.3/tests/test_functional.py`

 * *Files identical despite different names*

