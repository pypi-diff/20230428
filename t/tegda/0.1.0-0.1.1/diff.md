# Comparing `tmp/tegda-0.1.0.tar.gz` & `tmp/tegda-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tegda-0.1.0.tar", last modified: Thu Apr 27 17:53:16 2023, max compression
+gzip compressed data, was "tegda-0.1.1.tar", last modified: Fri Apr 28 18:23:30 2023, max compression
```

## Comparing `tegda-0.1.0.tar` & `tegda-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-27 17:53:16.290167 tegda-0.1.0/
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      171 2023-04-27 17:07:12.000000 tegda-0.1.0/AUTHORS.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     3509 2023-04-27 17:07:12.000000 tegda-0.1.0/CONTRIBUTING.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       89 2023-04-27 17:07:12.000000 tegda-0.1.0/HISTORY.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     1079 2023-04-27 17:07:12.000000 tegda-0.1.0/LICENSE
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      262 2023-04-27 17:07:12.000000 tegda-0.1.0/MANIFEST.in
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     2293 2023-04-27 17:53:16.291169 tegda-0.1.0/PKG-INFO
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     1062 2023-04-27 17:07:12.000000 tegda-0.1.0/README.rst
-drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-27 17:53:16.004262 tegda-0.1.0/docs/
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      606 2023-04-27 17:07:12.000000 tegda-0.1.0/docs/Makefile
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       28 2023-04-27 17:07:12.000000 tegda-0.1.0/docs/authors.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     4808 2023-04-27 17:07:12.000000 tegda-0.1.0/docs/conf.py
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       33 2023-04-27 17:07:12.000000 tegda-0.1.0/docs/contributing.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       28 2023-04-27 17:07:12.000000 tegda-0.1.0/docs/history.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      310 2023-04-27 17:07:12.000000 tegda-0.1.0/docs/index.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     1134 2023-04-27 17:07:12.000000 tegda-0.1.0/docs/installation.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      803 2023-04-27 17:07:12.000000 tegda-0.1.0/docs/make.bat
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       27 2023-04-27 17:07:12.000000 tegda-0.1.0/docs/readme.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       73 2023-04-27 17:07:12.000000 tegda-0.1.0/docs/usage.rst
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      422 2023-04-27 17:53:16.297664 tegda-0.1.0/setup.cfg
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     1424 2023-04-27 17:07:12.000000 tegda-0.1.0/setup.py
-drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-27 17:53:16.069261 tegda-0.1.0/tegda/
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      146 2023-04-27 17:07:12.000000 tegda-0.1.0/tegda/__init__.py
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      393 2023-04-27 17:07:12.000000 tegda-0.1.0/tegda/cli.py
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       19 2023-04-27 17:07:12.000000 tegda-0.1.0/tegda/tegda.py
-drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-27 17:53:16.222394 tegda-0.1.0/tegda.egg-info/
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)     2293 2023-04-27 17:53:14.000000 tegda-0.1.0/tegda.egg-info/PKG-INFO
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      543 2023-04-27 17:53:15.000000 tegda-0.1.0/tegda.egg-info/SOURCES.txt
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)        1 2023-04-27 17:53:14.000000 tegda-0.1.0/tegda.egg-info/dependency_links.txt
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       42 2023-04-27 17:53:14.000000 tegda-0.1.0/tegda.egg-info/entry_points.txt
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)        1 2023-04-27 17:53:14.000000 tegda-0.1.0/tegda.egg-info/not-zip-safe
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       11 2023-04-27 17:53:14.000000 tegda-0.1.0/tegda.egg-info/requires.txt
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)        6 2023-04-27 17:53:14.000000 tegda-0.1.0/tegda.egg-info/top_level.txt
-drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-27 17:53:16.266305 tegda-0.1.0/tests/
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)       35 2023-04-27 17:07:12.000000 tegda-0.1.0/tests/__init__.py
--rwxrwxrwx   0 titorium  (1000) titorium  (1000)      969 2023-04-27 17:07:12.000000 tegda-0.1.0/tests/test_tegda.py
+drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-28 18:23:30.047798 tegda-0.1.1/
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      171 2023-04-27 17:07:12.000000 tegda-0.1.1/AUTHORS.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     3509 2023-04-27 17:07:12.000000 tegda-0.1.1/CONTRIBUTING.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      115 2023-04-27 17:58:03.000000 tegda-0.1.1/HISTORY.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     6131 2023-04-27 18:50:58.000000 tegda-0.1.1/LICENSE
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      262 2023-04-27 17:07:12.000000 tegda-0.1.1/MANIFEST.in
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     2348 2023-04-28 18:23:30.048799 tegda-0.1.1/PKG-INFO
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     1091 2023-04-28 17:23:37.000000 tegda-0.1.1/README.rst
+drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-28 18:23:29.644834 tegda-0.1.1/docs/
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      606 2023-04-27 17:07:12.000000 tegda-0.1.1/docs/Makefile
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       28 2023-04-27 17:07:12.000000 tegda-0.1.1/docs/authors.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     4808 2023-04-27 17:07:12.000000 tegda-0.1.1/docs/conf.py
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       33 2023-04-27 17:07:12.000000 tegda-0.1.1/docs/contributing.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       28 2023-04-27 17:07:12.000000 tegda-0.1.1/docs/history.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      310 2023-04-27 17:07:12.000000 tegda-0.1.1/docs/index.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     1134 2023-04-27 17:07:12.000000 tegda-0.1.1/docs/installation.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      803 2023-04-27 17:07:12.000000 tegda-0.1.1/docs/make.bat
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       27 2023-04-27 17:07:12.000000 tegda-0.1.1/docs/readme.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       73 2023-04-27 17:07:12.000000 tegda-0.1.1/docs/usage.rst
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      422 2023-04-28 18:23:30.056316 tegda-0.1.1/setup.cfg
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     1424 2023-04-28 18:22:22.000000 tegda-0.1.1/setup.py
+drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-28 18:23:29.757675 tegda-0.1.1/tegda/
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      384 2023-04-28 18:22:30.000000 tegda-0.1.1/tegda/__init__.py
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      393 2023-04-27 17:07:12.000000 tegda-0.1.1/tegda/cli.py
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       19 2023-04-27 17:07:12.000000 tegda-0.1.1/tegda/tegda.py
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     1365 2023-04-27 19:21:00.000000 tegda-0.1.1/tegda/utils.py
+drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-28 18:23:29.965166 tegda-0.1.1/tegda.egg-info/
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)     2348 2023-04-28 18:23:28.000000 tegda-0.1.1/tegda.egg-info/PKG-INFO
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      558 2023-04-28 18:23:29.000000 tegda-0.1.1/tegda.egg-info/SOURCES.txt
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)        1 2023-04-28 18:23:28.000000 tegda-0.1.1/tegda.egg-info/dependency_links.txt
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       42 2023-04-28 18:23:28.000000 tegda-0.1.1/tegda.egg-info/entry_points.txt
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)        1 2023-04-28 18:23:28.000000 tegda-0.1.1/tegda.egg-info/not-zip-safe
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       11 2023-04-28 18:23:28.000000 tegda-0.1.1/tegda.egg-info/requires.txt
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)        6 2023-04-28 18:23:28.000000 tegda-0.1.1/tegda.egg-info/top_level.txt
+drwxrwxrwx   0 titorium  (1000) titorium  (1000)        0 2023-04-28 18:23:30.017511 tegda-0.1.1/tests/
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)       35 2023-04-27 17:07:12.000000 tegda-0.1.1/tests/__init__.py
+-rwxrwxrwx   0 titorium  (1000) titorium  (1000)      969 2023-04-27 17:07:12.000000 tegda-0.1.1/tests/test_tegda.py
```

### Comparing `tegda-0.1.0/CONTRIBUTING.rst` & `tegda-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tegda-0.1.0/PKG-INFO` & `tegda-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.2
 Name: tegda
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tegda creates customizable visual representations of data for exploratory analysis.
 Home-page: https://github.com/Robertoarce/tegda
 Author: Roberto Arce Aguirre
 Author-email: roberto_arce_@hotmail.com
 License: MIT license
 Description: =============
-        titorium EGDA
+        Terrific EGDA
         =============
         
         
         .. image:: https://img.shields.io/pypi/v/tegda.svg
                 :target: https://pypi.python.org/pypi/tegda
         
         .. image:: https://img.shields.io/travis/Robertoarce/tegda.svg
@@ -24,25 +24,25 @@
         
         .. image:: https://pyup.io/repos/github/Robertoarce/tegda/shield.svg
              :target: https://pyup.io/repos/github/Robertoarce/tegda/
              :alt: Updates
         
         
         
-        Tegda creates customizable visual representations of data for exploratory analysis.
+        Tegda creates an easy customizable visual representations of data for exploratory analysis.
         
         
         * Free software: MIT license
         * Documentation: https://tegda.readthedocs.io.
         
         
         Features
         --------
         
-        * TODO
+        * Use several visualization
         
         Credits
         -------
         
         This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
         
         .. _Cookiecutter: https://github.com/audreyr/cookiecutter
@@ -53,15 +53,15 @@
         History
         =======
         
         0.1.0 (2023-04-27)
         ------------------
         
         * First release on PyPI.
-        
+        * Adding PyPI and TestPypi
 Keywords: tegda
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tegda-0.1.0/README.rst` & `tegda-0.1.1/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 =============
-titorium EGDA
+Terrific EGDA
 =============
 
 
 .. image:: https://img.shields.io/pypi/v/tegda.svg
         :target: https://pypi.python.org/pypi/tegda
 
 .. image:: https://img.shields.io/travis/Robertoarce/tegda.svg
@@ -16,25 +16,25 @@
 
 .. image:: https://pyup.io/repos/github/Robertoarce/tegda/shield.svg
      :target: https://pyup.io/repos/github/Robertoarce/tegda/
      :alt: Updates
 
 
 
-Tegda creates customizable visual representations of data for exploratory analysis.
+Tegda creates an easy customizable visual representations of data for exploratory analysis.
 
 
 * Free software: MIT license
 * Documentation: https://tegda.readthedocs.io.
 
 
 Features
 --------
 
-* TODO
+* Use several visualization
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
```

### Comparing `tegda-0.1.0/docs/Makefile` & `tegda-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tegda-0.1.0/docs/conf.py` & `tegda-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tegda-0.1.0/docs/installation.rst` & `tegda-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tegda-0.1.0/docs/make.bat` & `tegda-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tegda-0.1.0/setup.py` & `tegda-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords='tegda',
     name='tegda',
     packages=find_packages(include=['tegda', 'tegda.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Robertoarce/tegda',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

### Comparing `tegda-0.1.0/tegda.egg-info/PKG-INFO` & `tegda-0.1.1/tegda.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.2
 Name: tegda
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tegda creates customizable visual representations of data for exploratory analysis.
 Home-page: https://github.com/Robertoarce/tegda
 Author: Roberto Arce Aguirre
 Author-email: roberto_arce_@hotmail.com
 License: MIT license
 Description: =============
-        titorium EGDA
+        Terrific EGDA
         =============
         
         
         .. image:: https://img.shields.io/pypi/v/tegda.svg
                 :target: https://pypi.python.org/pypi/tegda
         
         .. image:: https://img.shields.io/travis/Robertoarce/tegda.svg
@@ -24,25 +24,25 @@
         
         .. image:: https://pyup.io/repos/github/Robertoarce/tegda/shield.svg
              :target: https://pyup.io/repos/github/Robertoarce/tegda/
              :alt: Updates
         
         
         
-        Tegda creates customizable visual representations of data for exploratory analysis.
+        Tegda creates an easy customizable visual representations of data for exploratory analysis.
         
         
         * Free software: MIT license
         * Documentation: https://tegda.readthedocs.io.
         
         
         Features
         --------
         
-        * TODO
+        * Use several visualization
         
         Credits
         -------
         
         This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
         
         .. _Cookiecutter: https://github.com/audreyr/cookiecutter
@@ -53,15 +53,15 @@
         History
         =======
         
         0.1.0 (2023-04-27)
         ------------------
         
         * First release on PyPI.
-        
+        * Adding PyPI and TestPypi
 Keywords: tegda
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tegda-0.1.0/tegda.egg-info/SOURCES.txt` & `tegda-0.1.1/tegda.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 tegda/__init__.py
 tegda/cli.py
 tegda/tegda.py
+tegda/utils.py
 tegda.egg-info/PKG-INFO
 tegda.egg-info/SOURCES.txt
 tegda.egg-info/dependency_links.txt
 tegda.egg-info/entry_points.txt
 tegda.egg-info/not-zip-safe
 tegda.egg-info/requires.txt
 tegda.egg-info/top_level.txt
```

### Comparing `tegda-0.1.0/tests/test_tegda.py` & `tegda-0.1.1/tests/test_tegda.py`

 * *Files identical despite different names*

