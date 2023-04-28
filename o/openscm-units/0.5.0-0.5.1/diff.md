# Comparing `tmp/openscm-units-0.5.0.tar.gz` & `tmp/openscm-units-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openscm-units-0.5.0.tar", last modified: Tue Sep  7 00:09:49 2021, max compression
+gzip compressed data, was "dist/openscm-units-0.5.1.tar", last modified: Fri Apr 28 07:48:13 2023, max compression
```

## Comparing `openscm-units-0.5.0.tar` & `openscm-units-0.5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-07 00:09:49.000000 openscm-units-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     3364 2021-09-07 00:08:34.000000 openscm-units-0.5.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1552 2021-09-07 00:08:34.000000 openscm-units-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      118 2021-09-07 00:08:34.000000 openscm-units-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2021-09-07 00:09:49.000000 openscm-units-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3872 2021-09-07 00:08:34.000000 openscm-units-0.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      925 2021-09-07 00:09:49.000000 openscm-units-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3456 2021-09-07 00:08:34.000000 openscm-units-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-07 00:09:49.000000 openscm-units-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-07 00:09:49.000000 openscm-units-0.5.0/src/openscm_units/
--rw-r--r--   0 runner    (1001) docker     (121)      233 2021-09-07 00:08:34.000000 openscm-units-0.5.0/src/openscm_units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20668 2021-09-07 00:08:34.000000 openscm-units-0.5.0/src/openscm_units/_unit_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2021-09-07 00:09:49.000000 openscm-units-0.5.0/src/openscm_units/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-07 00:09:49.000000 openscm-units-0.5.0/src/openscm_units/data/
--rw-r--r--   0 runner    (1001) docker     (121)      135 2021-09-07 00:08:34.000000 openscm-units-0.5.0/src/openscm_units/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14607 2021-09-07 00:08:34.000000 openscm-units-0.5.0/src/openscm_units/data/mixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-07 00:09:49.000000 openscm-units-0.5.0/src/openscm_units.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2021-09-07 00:09:49.000000 openscm-units-0.5.0/src/openscm_units.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      447 2021-09-07 00:09:49.000000 openscm-units-0.5.0/src/openscm_units.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-07 00:09:49.000000 openscm-units-0.5.0/src/openscm_units.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      458 2021-09-07 00:09:49.000000 openscm-units-0.5.0/src/openscm_units.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-09-07 00:09:49.000000 openscm-units-0.5.0/src/openscm_units.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    68611 2021-09-07 00:08:34.000000 openscm-units-0.5.0/versioneer.py
+drwxr-xr-x   0 znicholls (1461210280) 2094513965        0 2023-04-28 07:48:13.898023 openscm-units-0.5.1/
+-rw-r--r--   0 znicholls (1461210280) 2094513965     3805 2023-04-28 07:36:36.000000 openscm-units-0.5.1/CHANGELOG.rst
+-rw-r--r--   0 znicholls (1461210280) 2094513965     1552 2021-07-27 07:27:26.000000 openscm-units-0.5.1/LICENSE
+-rw-r--r--   0 znicholls (1461210280) 2094513965      118 2021-09-07 00:01:10.000000 openscm-units-0.5.1/MANIFEST.in
+-rw-r--r--   0 znicholls (1461210280) 2094513965     1382 2023-04-28 07:48:13.898436 openscm-units-0.5.1/PKG-INFO
+-rw-r--r--   0 znicholls (1461210280) 2094513965     3872 2021-07-27 07:27:26.000000 openscm-units-0.5.1/README.rst
+-rw-r--r--   0 znicholls (1461210280) 2094513965      925 2023-04-28 07:48:13.900656 openscm-units-0.5.1/setup.cfg
+-rw-r--r--   0 znicholls (1461210280) 2094513965     3501 2022-05-24 17:23:48.000000 openscm-units-0.5.1/setup.py
+drwxr-xr-x   0 znicholls (1461210280) 2094513965        0 2023-04-28 07:48:13.877330 openscm-units-0.5.1/src/
+drwxr-xr-x   0 znicholls (1461210280) 2094513965        0 2023-04-28 07:48:13.901697 openscm-units-0.5.1/src/openscm_units/
+-rw-r--r--   0 znicholls (1461210280) 2094513965      233 2021-07-27 07:27:26.000000 openscm-units-0.5.1/src/openscm_units/__init__.py
+-rw-r--r--   0 znicholls (1461210280) 2094513965    20654 2023-04-28 07:36:20.000000 openscm-units-0.5.1/src/openscm_units/_unit_registry.py
+-rw-r--r--   0 znicholls (1461210280) 2094513965      497 2023-04-28 07:48:13.901999 openscm-units-0.5.1/src/openscm_units/_version.py
+drwxr-xr-x   0 znicholls (1461210280) 2094513965        0 2023-04-28 07:48:13.896098 openscm-units-0.5.1/src/openscm_units/data/
+-rw-r--r--   0 znicholls (1461210280) 2094513965      135 2021-07-27 07:27:26.000000 openscm-units-0.5.1/src/openscm_units/data/__init__.py
+-rw-r--r--   0 znicholls (1461210280) 2094513965    14607 2021-07-27 07:27:26.000000 openscm-units-0.5.1/src/openscm_units/data/mixtures.py
+drwxr-xr-x   0 znicholls (1461210280) 2094513965        0 2023-04-28 07:48:13.893654 openscm-units-0.5.1/src/openscm_units.egg-info/
+-rw-r--r--   0 znicholls (1461210280) 2094513965     1382 2023-04-28 07:48:13.000000 openscm-units-0.5.1/src/openscm_units.egg-info/PKG-INFO
+-rw-r--r--   0 znicholls (1461210280) 2094513965      447 2023-04-28 07:48:13.000000 openscm-units-0.5.1/src/openscm_units.egg-info/SOURCES.txt
+-rw-r--r--   0 znicholls (1461210280) 2094513965        1 2023-04-28 07:48:13.000000 openscm-units-0.5.1/src/openscm_units.egg-info/dependency_links.txt
+-rw-r--r--   0 znicholls (1461210280) 2094513965      505 2023-04-28 07:48:13.000000 openscm-units-0.5.1/src/openscm_units.egg-info/requires.txt
+-rw-r--r--   0 znicholls (1461210280) 2094513965       14 2023-04-28 07:48:13.000000 openscm-units-0.5.1/src/openscm_units.egg-info/top_level.txt
+-rw-r--r--   0 znicholls (1461210280) 2094513965    68611 2021-07-27 07:27:26.000000 openscm-units-0.5.1/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `openscm-units-0.5.0/CHANGELOG.rst` & `openscm-units-0.5.1/CHANGELOG.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+v0.5.1
+------
+
+- (`#33 <https://github.com/openscm/openscm-units/pull/33>`_) Generate static usage documentation from the introduction notebook
+- (`#34 <https://github.com/openscm/openscm-units/pull/34>`_) Update documentation regarding NOx conversions.
+- (`#38 <https://github.com/openscm/openscm-units/pull/38>`_) Fixed Series.iteritems() removal in pandas, see e.g. `#150 in primap2 <https://github.com/pik-primap/primap2/issues/150>`_
+
+
 v0.5.0
 ------
 
 - (`#30 <https://github.com/openscm/openscm-units/pull/30>`_) Custom metrics are now to be provided as :obj:`pd.DataFrame` rather than being read off disk
 - (`#29 <https://github.com/openscm/openscm-units/pull/29>`_) Load Global Warming Potentials from `globalwarmingpotentials <https://github.com/openclimatedata/globalwarmingpotentials>`_ package.
 
 v0.4.0
```

### Comparing `openscm-units-0.5.0/LICENSE` & `openscm-units-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openscm-units-0.5.0/PKG-INFO` & `openscm-units-0.5.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,15 @@
 Metadata-Version: 2.1
 Name: openscm-units
-Version: 0.5.0
+Version: 0.5.1
 Summary: OpenSCM-Units is a repository for handling of units related to simple climate modelling.
 Home-page: https://github.com/openscm/openscm-units
 Author: Zeb Nicholls, Sven Willner, Jared Lewis, Robert Gieseke
 Author-email: zebedee.nicholls@climate-energy-college.org, sven.willner@pik-potsdam.de, jared.lewis@climate-energy-college.org, rob.g@web.de
 License: 3-Clause BSD License
-Description: OpenSCM-Units
-        ==============
-        
-        .. sec-begin-index
-        
-        OpenSCM-Units is a repository for handling of units related to simple climate modelling.
-        
-        .. sec-end-index
-        
-        License
-        -------
-        
-        .. sec-begin-license
-        
-        OpenSCM-Units is free software under a BSD 3-Clause License, see
-        `LICENSE <https://github.com/openscm/openscm-units/blob/master/LICENSE>`_.
-        
-        .. sec-end-license
 Keywords: openscm,units,python,repo,simple,climate,model
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
@@ -35,7 +17,28 @@
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: deploy
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: notebooks
 Provides-Extra: tests
+License-File: LICENSE
+
+OpenSCM-Units
+==============
+
+.. sec-begin-index
+
+OpenSCM-Units is a repository for handling of units related to simple climate modelling.
+
+.. sec-end-index
+
+License
+-------
+
+.. sec-begin-license
+
+OpenSCM-Units is free software under a BSD 3-Clause License, see
+`LICENSE <https://github.com/openscm/openscm-units/blob/master/LICENSE>`_.
+
+.. sec-end-license
+
```

### Comparing `openscm-units-0.5.0/README.rst` & `openscm-units-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `openscm-units-0.5.0/setup.cfg` & `openscm-units-0.5.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 inherit = false
 match = (?!test_|_version).*\.py
 
 [tool:pytest]
 testpaths = tests
 
 [versioneer]
-vcs = git
+VCS = git
 style = pep440
 versionfile_source = src/openscm_units/_version.py
 versionfile_build = openscm_units/_version.py
 tag_prefix = v
 parentdir_prefix = openscm_units-
 
 [egg_info]
```

### Comparing `openscm-units-0.5.0/setup.py` & `openscm-units-0.5.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 PACKAGES = find_packages(SOURCE_DIR)  # no exclude as only searching in `src`
 PACKAGE_DIR = {"": SOURCE_DIR}
 
 REQUIREMENTS = ["pandas", "pint", "globalwarmingpotentials"]
 REQUIREMENTS_NOTEBOOKS = ["notebook", "seaborn"]
 REQUIREMENTS_TESTS = ["codecov", "coverage", "nbval", "pytest-cov", "pytest>=4.0"]
-REQUIREMENTS_DOCS = ["sphinx>=1.4", "sphinx_rtd_theme"]
+REQUIREMENTS_DOCS = ["sphinx>=1.4", "sphinx_rtd_theme", "nbsphinx", "ipykernel"]
 REQUIREMENTS_DEPLOY = ["twine>=1.11.0", "setuptools>=38.6.0", "wheel>=0.31.0"]
 
 REQUIREMENTS_DEV = [
     *[
         "bandit",
         "black",
         "black-nb",
@@ -35,14 +35,15 @@
         "isort",
         "mypy",
         "nbdime",
         "numpy",
         "pydocstyle",
         "pylint>=2.4.4",
         "dephell_changelogs",
+        "nbsphinx",
     ],
     *REQUIREMENTS_DEPLOY,
     *REQUIREMENTS_DOCS,
     *REQUIREMENTS_NOTEBOOKS,
     *REQUIREMENTS_TESTS,
 ]
```

### Comparing `openscm-units-0.5.0/src/openscm_units/_unit_registry.py` & `openscm-units-0.5.1/src/openscm_units/_unit_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 define here are emissions units i.e. the stuff. Here we include as many of the canonical
 emissions units, and their conversions, as possible.
 
 For emissions units, there are a few cases to be considered:
 
 - fairly obvious ones e.g. carbon dioxide emissions can be provided in 'C' or 'CO2' and
   converting between the two is possible
-- less obvious ones e.g. NOx emissions can be provided in 'N' or 'NOx' (a short-hand
-  which is assumed to be NO2), we provide conversions between these two
+- less obvious ones e.g. NOx emissions can be provided in 'N' or 'NOx', we provide
+  conversions between these two which can be enabled if needed (see below).
 - case-sensitivity. In order to provide a simplified interface, using all uppercase
   versions of any unit is also valid e.g. ``unit_registry("HFC4310mee")`` is the same as
   ``unit_registry("HFC4310MEE")``
 - hyphens and underscores in units. In order to be Pint compatible and to simplify
   things, we strip all hyphens and underscores from units.
 
 As a convenience, we allow users to combine the mass and the type of emissions to make a
@@ -141,14 +141,15 @@
     ...     unit_registry("NH3").to("N")
     <Quantity(0.823529412, 'N')>
 
 """
 import math
 
 import globalwarmingpotentials
+import pandas as pd
 import pint
 
 from .data.mixtures import MIXTURES
 
 # Standard gases. If the value is:
 # - str: this entry defines a base gas unit
 # - list: this entry defines a derived unit
@@ -337,15 +338,15 @@
         """
         Add standard units.
 
         Has to be done separately because of pint's weird initializing.
         """
         self._add_gases(_STANDARD_GASES)
 
-        self._add_gases({x: x for x in MIXTURES.keys()})
+        self._add_gases({x: x for x in MIXTURES})
 
         self.define("a = 1 * year = annum = yr")
         self.define("h = hour")
         self.define("d = day")
         self.define("degreeC = degC")
         self.define("degreeF = degF")
         self.define("kt = 1000 * t")  # since kt is used for "knot" in the defaults
@@ -382,28 +383,28 @@
         self.define("g{symbol} = g * {symbol}".format(symbol=symbol))
         self.define("t{symbol} = t * {symbol}".format(symbol=symbol))
 
     def _add_gases(self, gases):
         for symbol, value in gases.items():
             if isinstance(value, str):
                 # symbol is base unit
-                self.define("{} = [{}]".format(symbol, value))
+                self.define(f"{symbol} = [{value}]")
                 if value != symbol:
-                    self.define("{} = {}".format(value, symbol))
+                    self.define(f"{value} = {symbol}")
             else:
                 # symbol has conversion and aliases
-                self.define("{} = {}".format(symbol, value[0]))
+                self.define(f"{symbol} = {value[0]}")
                 for alias in value[1:]:
-                    self.define("{} = {}".format(alias, symbol))
+                    self.define(f"{alias} = {symbol}")
 
             self._add_mass_emissions_joint_version(symbol)
 
             # Add alias for upper case symbol:
             if symbol.upper() != symbol:
-                self.define("{} = {}".format(symbol.upper(), symbol))
+                self.define(f"{symbol.upper()} = {symbol}")
                 self._add_mass_emissions_joint_version(symbol.upper())
 
     def _add_contexts(self):
         """
         Add contexts
         """
         _ch4_context = pint.Context("CH4_conversions")
@@ -459,20 +460,20 @@
         if self._metric_conversions is None:
             metric_conversions = globalwarmingpotentials.as_frame()
         else:
             metric_conversions = self._metric_conversions
 
         self._add_metric_conversions_from_df(metric_conversions)
 
-    def _add_metric_conversions_from_df(self, metric_conversions):
+    def _add_metric_conversions_from_df(self, metric_conversions: pd.DataFrame):
         # could make this public in future
         for col in metric_conversions:
-            metric_conversion = metric_conversions[col]
+            metric_conversion: pd.Series = metric_conversions[col]
             transform_context = pint.Context(col)
-            for label, val in metric_conversion.iteritems():
+            for label, val in metric_conversion.items():
                 transform_context = self._add_gwp_to_context(
                     transform_context, label, val
                 )
 
             for mixture in MIXTURES:
                 constituents = self.split_gas_mixture(1 * self(mixture))
                 try:
```

### Comparing `openscm-units-0.5.0/src/openscm_units/data/mixtures.py` & `openscm-units-0.5.1/src/openscm_units/data/mixtures.py`

 * *Files identical despite different names*

### Comparing `openscm-units-0.5.0/src/openscm_units.egg-info/PKG-INFO` & `openscm-units-0.5.1/src/openscm_units.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,15 @@
 Metadata-Version: 2.1
 Name: openscm-units
-Version: 0.5.0
+Version: 0.5.1
 Summary: OpenSCM-Units is a repository for handling of units related to simple climate modelling.
 Home-page: https://github.com/openscm/openscm-units
 Author: Zeb Nicholls, Sven Willner, Jared Lewis, Robert Gieseke
 Author-email: zebedee.nicholls@climate-energy-college.org, sven.willner@pik-potsdam.de, jared.lewis@climate-energy-college.org, rob.g@web.de
 License: 3-Clause BSD License
-Description: OpenSCM-Units
-        ==============
-        
-        .. sec-begin-index
-        
-        OpenSCM-Units is a repository for handling of units related to simple climate modelling.
-        
-        .. sec-end-index
-        
-        License
-        -------
-        
-        .. sec-begin-license
-        
-        OpenSCM-Units is free software under a BSD 3-Clause License, see
-        `LICENSE <https://github.com/openscm/openscm-units/blob/master/LICENSE>`_.
-        
-        .. sec-end-license
 Keywords: openscm,units,python,repo,simple,climate,model
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
@@ -35,7 +17,28 @@
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: deploy
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: notebooks
 Provides-Extra: tests
+License-File: LICENSE
+
+OpenSCM-Units
+==============
+
+.. sec-begin-index
+
+OpenSCM-Units is a repository for handling of units related to simple climate modelling.
+
+.. sec-end-index
+
+License
+-------
+
+.. sec-begin-license
+
+OpenSCM-Units is free software under a BSD 3-Clause License, see
+`LICENSE <https://github.com/openscm/openscm-units/blob/master/LICENSE>`_.
+
+.. sec-end-license
+
```

### Comparing `openscm-units-0.5.0/versioneer.py` & `openscm-units-0.5.1/versioneer.py`

 * *Files identical despite different names*

