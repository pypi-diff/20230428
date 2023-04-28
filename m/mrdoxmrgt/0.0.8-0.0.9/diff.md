# Comparing `tmp/mrdoxmrgt-0.0.8.tar.gz` & `tmp/mrdoxmrgt-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrdoxmrgt-0.0.8.tar", last modified: Sat Apr 22 06:35:08 2023, max compression
+gzip compressed data, was "mrdoxmrgt-0.0.9.tar", last modified: Fri Apr 28 18:42:25 2023, max compression
```

## Comparing `mrdoxmrgt-0.0.8.tar` & `mrdoxmrgt-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 06:35:08.000000 mrdoxmrgt-0.0.8/
--rw-rw-rw-   0        0        0     1083 2023-04-20 14:15:02.000000 mrdoxmrgt-0.0.8/LICENCE
--rw-rw-rw-   0        0        0      810 2023-04-22 06:35:10.000000 mrdoxmrgt-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-04-20 14:15:34.000000 mrdoxmrgt-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 06:35:08.000000 mrdoxmrgt-0.0.8/mrdoxmrgt/
-drwxrwxrwx   0        0        0        0 2023-04-22 06:35:10.000000 mrdoxmrgt-0.0.8/mrdoxmrgt/GTF/
--rw-rw-rw-   0        0        0        0 2023-04-21 17:55:06.000000 mrdoxmrgt-0.0.8/mrdoxmrgt/GTF/__init__.py
--rw-rw-rw-   0        0        0     3192 2023-04-22 06:26:56.000000 mrdoxmrgt-0.0.8/mrdoxmrgt/GTF/install.py
--rw-rw-rw-   0        0        0     1392 2023-04-22 05:22:14.000000 mrdoxmrgt-0.0.8/mrdoxmrgt/GTF/run.py
--rw-rw-rw-   0        0        0        0 2023-04-21 17:55:06.000000 mrdoxmrgt-0.0.8/mrdoxmrgt/__init__.py
--rw-rw-rw-   0        0        0     2542 2023-04-22 06:34:40.000000 mrdoxmrgt-0.0.8/mrdoxmrgt/_main_.py
-drwxrwxrwx   0        0        0        0 2023-04-22 06:35:08.000000 mrdoxmrgt-0.0.8/mrdoxmrgt.egg-info/
--rw-rw-rw-   0        0        0      810 2023-04-22 06:35:08.000000 mrdoxmrgt-0.0.8/mrdoxmrgt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-04-22 06:35:08.000000 mrdoxmrgt-0.0.8/mrdoxmrgt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 06:35:08.000000 mrdoxmrgt-0.0.8/mrdoxmrgt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-22 06:35:08.000000 mrdoxmrgt-0.0.8/mrdoxmrgt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-22 06:35:08.000000 mrdoxmrgt-0.0.8/mrdoxmrgt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-22 06:35:08.000000 mrdoxmrgt-0.0.8/mrdoxmrgt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 06:35:10.000000 mrdoxmrgt-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1243 2023-04-22 06:34:46.000000 mrdoxmrgt-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 18:42:26.000000 mrdoxmrgt-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2023-04-14 09:24:50.000000 mrdoxmrgt-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      800 2023-04-28 18:42:26.000000 mrdoxmrgt-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-04-14 09:24:50.000000 mrdoxmrgt-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 18:42:26.000000 mrdoxmrgt-0.0.9/mrdoxmrgt/
+-rw-rw-rw-   0        0        0        0 2023-04-28 10:15:20.000000 mrdoxmrgt-0.0.9/mrdoxmrgt/__init__.py
+-rw-rw-rw-   0        0        0     3792 2023-04-28 10:21:08.000000 mrdoxmrgt-0.0.9/mrdoxmrgt/main.py
+-rw-rw-rw-   0        0        0    15122 2023-04-28 10:15:42.000000 mrdoxmrgt-0.0.9/mrdoxmrgt/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 18:42:26.000000 mrdoxmrgt-0.0.9/mrdoxmrgt.egg-info/
+-rw-rw-rw-   0        0        0      800 2023-04-28 18:42:26.000000 mrdoxmrgt-0.0.9/mrdoxmrgt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-04-28 18:42:26.000000 mrdoxmrgt-0.0.9/mrdoxmrgt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 18:42:26.000000 mrdoxmrgt-0.0.9/mrdoxmrgt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-04-28 18:42:26.000000 mrdoxmrgt-0.0.9/mrdoxmrgt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2023-04-28 18:42:26.000000 mrdoxmrgt-0.0.9/mrdoxmrgt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-28 18:42:26.000000 mrdoxmrgt-0.0.9/mrdoxmrgt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 18:42:26.000000 mrdoxmrgt-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1252 2023-04-28 10:22:02.000000 mrdoxmrgt-0.0.9/setup.py
```

### Comparing `mrdoxmrgt-0.0.8/PKG-INFO` & `mrdoxmrgt-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: mrdoxmrgt
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small example package
-Home-page: https://github.com/GreyTechno/SMS_Forwarder
+Home-page: https://github.com/GreyTechno/gtf
 Download-URL: https://github.com/GreyTechno/gtf/archive/pypi.zip
 Author: MR_GT
 Author-email: friendyt89@gmail.com
 License: GPL
 Keywords: a1,a2,a3,a3,a4,a5,a6,a7,a8,a9
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-License-File: LICENCE
+License-File: LICENSE
 
 A small example package HI
```

### Comparing `mrdoxmrgt-0.0.8/mrdoxmrgt.egg-info/PKG-INFO` & `mrdoxmrgt-0.0.9/mrdoxmrgt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: mrdoxmrgt
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small example package
-Home-page: https://github.com/GreyTechno/SMS_Forwarder
+Home-page: https://github.com/GreyTechno/gtf
 Download-URL: https://github.com/GreyTechno/gtf/archive/pypi.zip
 Author: MR_GT
 Author-email: friendyt89@gmail.com
 License: GPL
 Keywords: a1,a2,a3,a3,a4,a5,a6,a7,a8,a9
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-License-File: LICENCE
+License-File: LICENSE
 
 A small example package HI
```

### Comparing `mrdoxmrgt-0.0.8/setup.py` & `mrdoxmrgt-0.0.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mrdoxmrgt',
     packages=find_packages(),
     include_package_data=True,
-    version="0.0.8",
+    version="0.0.9",
     description='A small example package',
     long_description="A small example package HI",
     long_description_content_type="text/markdown",
     author='MR_GT',
     author_email='friendyt89@gmail.com',
-    url='https://github.com/GreyTechno/SMS_Forwarder',
+    url='https://github.com/GreyTechno/gtf',
     download_url="https://github.com/GreyTechno/gtf/archive/pypi.zip",
         keywords=['a1', 'a2', 'a3', 'a3', 'a4',
                   'a5', 'a6', 'a7', 'a8', 'a9'],
     classifiers=[
             'Development Status :: 4 - Beta',
             'Intended Audience :: Developers',
             'Topic :: Software Development :: Libraries :: Python Modules',
             'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
             'Programming Language :: Python :: 3',
             'Operating System :: OS Independent',
             'Environment :: Console',
     ],
-    install_requires=["requests"],
+    install_requires=["requests", "random", "zipfile"],
     license='GPL',
     entry_points={
             'console_scripts': [
-                'mrdoxmrgt = mrdoxmrgt._main_:main',
+                'mrdoxmrgt = mrdoxmrgt.main:Main',
             ],
     },
     python_requires='>=3.5'
 )
```

