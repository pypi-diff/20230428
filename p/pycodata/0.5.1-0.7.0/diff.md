# Comparing `tmp/pycodata-0.5.1.tar.gz` & `tmp/pycodata-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycodata-0.5.1.tar", last modified: Fri Apr 21 13:53:44 2023, max compression
+gzip compressed data, was "pycodata-0.7.0.tar", last modified: Fri Apr 28 05:11:50 2023, max compression
```

## Comparing `pycodata-0.5.1.tar` & `pycodata-0.7.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 mskocic   (1000) mskocic   (1000)        0 2023-04-21 13:53:44.502972 pycodata-0.5.1/
--rw-r--r--   0 mskocic   (1000) mskocic   (1000)    35823 2022-12-23 14:14:18.000000 pycodata-0.5.1/LICENSE.txt
--rw-r--r--   0 mskocic   (1000) mskocic   (1000)      195 2023-04-21 13:47:31.000000 pycodata-0.5.1/MANIFEST.in
--rw-r--r--   0 mskocic   (1000) mskocic   (1000)      778 2023-04-21 13:53:44.502972 pycodata-0.5.1/PKG-INFO
--rw-r--r--   0 mskocic   (1000) mskocic   (1000)      257 2023-04-21 12:39:44.000000 pycodata-0.5.1/README.rst
-drwxr-xr-x   0 mskocic   (1000) mskocic   (1000)        0 2023-04-21 13:53:44.502972 pycodata-0.5.1/pycodata/
--rw-r--r--   0 mskocic   (1000) mskocic   (1000)       97 2023-04-18 08:58:24.000000 pycodata-0.5.1/pycodata/__init__.py
--rw-r--r--   0 mskocic   (1000) mskocic   (1000)    49578 2023-04-18 06:53:49.000000 pycodata-0.5.1/pycodata/codata.h
--rw-r--r--   0 mskocic   (1000) mskocic   (1000)    94888 2023-04-21 12:47:49.000000 pycodata-0.5.1/pycodata/cpycodata.c
-drwxr-xr-x   0 mskocic   (1000) mskocic   (1000)        0 2023-04-21 13:53:44.502972 pycodata-0.5.1/pycodata/tests/
--rw-r--r--   0 mskocic   (1000) mskocic   (1000)        0 2023-04-12 09:50:16.000000 pycodata-0.5.1/pycodata/tests/__init__.py
--rw-r--r--   0 mskocic   (1000) mskocic   (1000)      250 2023-04-21 12:43:29.000000 pycodata-0.5.1/pycodata/tests/test_lib.py
--rw-r--r--   0 mskocic   (1000) mskocic   (1000)      555 2023-04-21 13:49:01.000000 pycodata-0.5.1/pycodata/version.py
-drwxr-xr-x   0 mskocic   (1000) mskocic   (1000)        0 2023-04-21 13:53:44.502972 pycodata-0.5.1/pycodata.egg-info/
--rw-r--r--   0 mskocic   (1000) mskocic   (1000)      778 2023-04-21 13:53:44.000000 pycodata-0.5.1/pycodata.egg-info/PKG-INFO
--rw-r--r--   0 mskocic   (1000) mskocic   (1000)      345 2023-04-21 13:53:44.000000 pycodata-0.5.1/pycodata.egg-info/SOURCES.txt
--rw-r--r--   0 mskocic   (1000) mskocic   (1000)        1 2023-04-21 13:53:44.000000 pycodata-0.5.1/pycodata.egg-info/dependency_links.txt
--rw-r--r--   0 mskocic   (1000) mskocic   (1000)        9 2023-04-21 13:53:44.000000 pycodata-0.5.1/pycodata.egg-info/top_level.txt
--rw-r--r--   0 mskocic   (1000) mskocic   (1000)        0 2023-02-20 07:43:52.000000 pycodata-0.5.1/requirements.txt
--rw-r--r--   0 mskocic   (1000) mskocic   (1000)       38 2023-04-21 13:53:44.502972 pycodata-0.5.1/setup.cfg
--rw-r--r--   0 mskocic   (1000) mskocic   (1000)     1641 2023-04-21 13:47:45.000000 pycodata-0.5.1/setup.py
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-04-28 05:11:50.555708 pycodata-0.7.0/
+-rw-r--r--   0 milan      (501) staff       (20)       20 2023-04-22 07:20:52.000000 pycodata-0.7.0/INSTALL.TXT
+-rw-r--r--   0 milan      (501) staff       (20)    35823 2023-04-22 07:20:52.000000 pycodata-0.7.0/LICENSE.TXT
+-rw-r--r--   0 milan      (501) staff       (20)      195 2023-04-22 07:20:52.000000 pycodata-0.7.0/MANIFEST.in
+-rw-r--r--   0 milan      (501) staff       (20)      996 2023-04-28 05:11:50.555056 pycodata-0.7.0/PKG-INFO
+-rw-r--r--   0 milan      (501) staff       (20)      418 2023-04-26 19:43:03.000000 pycodata-0.7.0/README.rst
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-04-28 05:11:50.549111 pycodata-0.7.0/pycodata/
+-rw-r--r--   0 milan      (501) staff       (20)       97 2023-04-22 07:20:52.000000 pycodata-0.7.0/pycodata/__init__.py
+-rw-r--r--   0 milan      (501) staff       (20)    49578 2023-04-22 07:20:52.000000 pycodata-0.7.0/pycodata/codata.h
+-rw-r--r--   0 milan      (501) staff       (20)    94969 2023-04-27 23:24:15.000000 pycodata-0.7.0/pycodata/cpycodata.c
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-04-28 05:11:50.554226 pycodata-0.7.0/pycodata/tests/
+-rw-r--r--   0 milan      (501) staff       (20)        0 2023-04-22 07:20:52.000000 pycodata-0.7.0/pycodata/tests/__init__.py
+-rw-r--r--   0 milan      (501) staff       (20)      365 2023-04-27 23:38:11.000000 pycodata-0.7.0/pycodata/tests/test_lib.py
+-rw-r--r--   0 milan      (501) staff       (20)      555 2023-04-28 04:56:46.000000 pycodata-0.7.0/pycodata/version.py
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-04-28 05:11:50.552641 pycodata-0.7.0/pycodata.egg-info/
+-rw-r--r--   0 milan      (501) staff       (20)      996 2023-04-28 05:11:50.000000 pycodata-0.7.0/pycodata.egg-info/PKG-INFO
+-rw-r--r--   0 milan      (501) staff       (20)      369 2023-04-28 05:11:50.000000 pycodata-0.7.0/pycodata.egg-info/SOURCES.txt
+-rw-r--r--   0 milan      (501) staff       (20)        1 2023-04-28 05:11:50.000000 pycodata-0.7.0/pycodata.egg-info/dependency_links.txt
+-rw-r--r--   0 milan      (501) staff       (20)        9 2023-04-28 05:11:50.000000 pycodata-0.7.0/pycodata.egg-info/top_level.txt
+-rw-r--r--   0 milan      (501) staff       (20)        0 2023-04-22 07:20:52.000000 pycodata-0.7.0/requirements.txt
+-rw-r--r--   0 milan      (501) staff       (20)       38 2023-04-28 05:11:50.555909 pycodata-0.7.0/setup.cfg
+-rw-r--r--   0 milan      (501) staff       (20)     1562 2023-04-28 05:03:25.000000 pycodata-0.7.0/setup.py
```

### Comparing `pycodata-0.5.1/LICENSE.txt` & `pycodata-0.7.0/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `pycodata-0.5.1/PKG-INFO` & `pycodata-0.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 Metadata-Version: 2.1
 Name: pycodata
-Version: 0.5.1
+Version: 0.7.0
 Summary: pycodata
-Download-URL: https://github.com/MilanSkocic/pycodata
+Home-page: https://milanskocic.github.io/codata/index.html
+Download-URL: https://github.com/MilanSkocic/codata
 Author: Milan Skocic
 Author-email: milan.skocic@icloud.com
 Maintainer: Milan Skocic
 Maintainer-email: milan.skocic@icloud.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 Description
 ============
 
+.. readme_inclusion_start
+
 Python module containing the codata constants.
 
+For now, the wrapper must be compiled using the compiler 
+that was used to compile your python interpreter.
+
+.. readme_inclusion_end
+
 Installation
 ===================
 See  ``INSTALL.txt``.
 
 Dependencies
 ================
```

### Comparing `pycodata-0.5.1/pycodata/codata.h` & `pycodata-0.7.0/pycodata/codata.h`

 * *Files identical despite different names*

### Comparing `pycodata-0.5.1/pycodata/cpycodata.c` & `pycodata-0.7.0/pycodata/cpycodata.c`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 PyMODINIT_FUNC PyInit_codata(void){
 	PyObject *m;
 	PyObject *d;
 	PyObject *v;
 	m = PyModule_Create(&codata);
 	d = PyModule_GetDict(m);
 
+	v = PyLong_FromLong(2018);
+	PyDict_SetItemString(d, "YEAR", v);
+	Py_INCREF(v);
+
 	v = PyFloat_FromDouble(ALPHA_PARTICLE_ELECTRON_MASS_RATIO);
 	PyDict_SetItemString(d, "ALPHA_PARTICLE_ELECTRON_MASS_RATIO", v);
 	Py_INCREF(v);
 	v = PyFloat_FromDouble(U_ALPHA_PARTICLE_ELECTRON_MASS_RATIO);
 	PyDict_SetItemString(d, "U_ALPHA_PARTICLE_ELECTRON_MASS_RATIO", v);
 	Py_INCREF(v);
```

### Comparing `pycodata-0.5.1/pycodata/version.py` & `pycodata-0.7.0/pycodata/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,14 @@
            '__author_email__',
            '__maintainer__',
            '__maintainer_email__',
            '__copyright__',
            '__license__']
 
 __package_name__ = "pycodata"
-__version__ = "0.5.1"
+__version__ = "0.7.0"
 __author__ = "Milan Skocic"
 __author_email__ = "milan.skocic@icloud.com"
 __maintainer__ = __author__
 __maintainer_email__ = __author_email__
 __copyright__ = 'Copyright (C) 2023 ' + __author__
 __license__ = 'GNU General Public License v3 (GPLv3)'
```

### Comparing `pycodata-0.5.1/pycodata.egg-info/PKG-INFO` & `pycodata-0.7.0/pycodata.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 Metadata-Version: 2.1
 Name: pycodata
-Version: 0.5.1
+Version: 0.7.0
 Summary: pycodata
-Download-URL: https://github.com/MilanSkocic/pycodata
+Home-page: https://milanskocic.github.io/codata/index.html
+Download-URL: https://github.com/MilanSkocic/codata
 Author: Milan Skocic
 Author-email: milan.skocic@icloud.com
 Maintainer: Milan Skocic
 Maintainer-email: milan.skocic@icloud.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 Description
 ============
 
+.. readme_inclusion_start
+
 Python module containing the codata constants.
 
+For now, the wrapper must be compiled using the compiler 
+that was used to compile your python interpreter.
+
+.. readme_inclusion_end
+
 Installation
 ===================
 See  ``INSTALL.txt``.
 
 Dependencies
 ================
```

### Comparing `pycodata-0.5.1/setup.py` & `pycodata-0.7.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-import os
-from setuptools import setup, find_packages, Extension
-import configparser
+r"""setup"""
 import importlib
 import pathlib
-import platform
+from setuptools import setup, find_packages, Extension
 
 # Import only version.py file for extracting the version
 spec = importlib.util.spec_from_file_location('version', './pycodata/version.py')
 mod = importlib.util.module_from_spec(spec)
 spec.loader.exec_module(mod)
 
 if __name__ == "__main__":
 
-    mod_ext = Extension(name="pycodata.codata",
-                                         sources=["./pycodata/cpycodata.c"])
+    mod_ext = Extension(name="pycodata.codata", sources=["./pycodata/cpycodata.c"])
     setup(name=mod.__package_name__,
         version=mod.__version__,
         maintainer=mod.__maintainer__,
         maintainer_email=mod.__maintainer_email__,
         author=mod.__author__,
         author_email=mod.__author_email__,
         description=mod.__package_name__,
         long_description=pathlib.Path("README.rst").read_text(encoding="utf-8"),
         long_description_content_type="text/x-rst",
-        #url='https://milanskocic.github.io/pycodata/index.html',
-        download_url='https://github.com/MilanSkocic/pycodata',
+        url='https://milanskocic.github.io/codata/index.html',
+        download_url='https://github.com/MilanSkocic/codata',
         packages=find_packages(),
         include_package_data=False,
         python_requires='>=3.7',
         install_requires=pathlib.Path("requirements.txt").read_text(encoding="utf-8").split('\n'),
         classifiers=["Development Status :: 5 - Production/Stable",
                     "Intended Audience :: Science/Research",
                     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)"],
```

