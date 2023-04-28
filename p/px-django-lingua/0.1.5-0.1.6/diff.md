# Comparing `tmp/px-django-lingua-0.1.5.tar.gz` & `tmp/px-django-lingua-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "px-django-lingua-0.1.5.tar", last modified: Fri Aug  6 09:00:14 2021, max compression
+gzip compressed data, was "px-django-lingua-0.1.6.tar", last modified: Fri Apr 28 09:48:37 2023, max compression
```

## Comparing `px-django-lingua-0.1.5.tar` & `px-django-lingua-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-06 09:00:14.927401 px-django-lingua-0.1.5/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1079 2021-06-25 13:47:17.000000 px-django-lingua-0.1.5/LICENSE
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     9656 2021-08-06 09:00:14.927401 px-django-lingua-0.1.5/PKG-INFO
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     9060 2021-08-06 08:58:06.000000 px-django-lingua-0.1.5/README.md
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-06 09:00:14.923401 px-django-lingua-0.1.5/px_django_lingua.egg-info/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     9656 2021-08-06 09:00:14.000000 px-django-lingua-0.1.5/px_django_lingua.egg-info/PKG-INFO
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      480 2021-08-06 09:00:14.000000 px-django-lingua-0.1.5/px_django_lingua.egg-info/SOURCES.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        1 2021-08-06 09:00:14.000000 px-django-lingua-0.1.5/px_django_lingua.egg-info/dependency_links.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       34 2021-08-06 09:00:14.000000 px-django-lingua-0.1.5/px_django_lingua.egg-info/requires.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       11 2021-08-06 09:00:14.000000 px-django-lingua-0.1.5/px_django_lingua.egg-info/top_level.txt
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-06 09:00:14.927401 px-django-lingua-0.1.5/pxd_lingua/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      139 2021-08-06 08:58:43.000000 px-django-lingua-0.1.5/pxd_lingua/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      140 2021-06-25 13:47:17.000000 px-django-lingua-0.1.5/pxd_lingua/admin.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      229 2021-06-25 13:47:17.000000 px-django-lingua-0.1.5/pxd_lingua/apps.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      893 2021-08-03 14:48:50.000000 px-django-lingua-0.1.5/pxd_lingua/conf.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1550 2021-08-06 05:23:54.000000 px-django-lingua-0.1.5/pxd_lingua/db.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      172 2021-08-06 05:23:54.000000 px-django-lingua-0.1.5/pxd_lingua/exceptions.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1454 2021-08-06 06:11:17.000000 px-django-lingua-0.1.5/pxd_lingua/loader.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     8069 2021-08-06 06:22:19.000000 px-django-lingua-0.1.5/pxd_lingua/magic.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     5013 2021-08-05 14:56:38.000000 px-django-lingua-0.1.5/pxd_lingua/models.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1733 2021-08-05 09:33:23.000000 px-django-lingua-0.1.5/pxd_lingua/query.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      139 2021-08-03 14:43:15.000000 px-django-lingua-0.1.5/pxd_lingua/types.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1737 2021-08-06 05:23:54.000000 px-django-lingua-0.1.5/pxd_lingua/utils.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       79 2021-08-06 09:00:14.927401 px-django-lingua-0.1.5/setup.cfg
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1427 2021-08-06 08:44:27.000000 px-django-lingua-0.1.5/setup.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-28 09:48:37.077229 px-django-lingua-0.1.6/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1079 2023-04-28 09:37:51.000000 px-django-lingua-0.1.6/LICENSE
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     9676 2023-04-28 09:48:37.077229 px-django-lingua-0.1.6/PKG-INFO
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     9060 2023-04-28 09:37:51.000000 px-django-lingua-0.1.6/README.md
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-28 09:48:37.073229 px-django-lingua-0.1.6/px_django_lingua.egg-info/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     9676 2023-04-28 09:48:37.000000 px-django-lingua-0.1.6/px_django_lingua.egg-info/PKG-INFO
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      480 2023-04-28 09:48:37.000000 px-django-lingua-0.1.6/px_django_lingua.egg-info/SOURCES.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        1 2023-04-28 09:48:37.000000 px-django-lingua-0.1.6/px_django_lingua.egg-info/dependency_links.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      149 2023-04-28 09:48:37.000000 px-django-lingua-0.1.6/px_django_lingua.egg-info/requires.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       11 2023-04-28 09:48:37.000000 px-django-lingua-0.1.6/px_django_lingua.egg-info/top_level.txt
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-28 09:48:37.077229 px-django-lingua-0.1.6/pxd_lingua/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      139 2023-04-28 09:48:21.000000 px-django-lingua-0.1.6/pxd_lingua/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      140 2023-04-28 09:37:51.000000 px-django-lingua-0.1.6/pxd_lingua/admin.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      229 2023-04-28 09:37:51.000000 px-django-lingua-0.1.6/pxd_lingua/apps.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      893 2023-04-28 09:37:51.000000 px-django-lingua-0.1.6/pxd_lingua/conf.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1550 2023-04-28 09:37:51.000000 px-django-lingua-0.1.6/pxd_lingua/db.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      172 2023-04-28 09:37:51.000000 px-django-lingua-0.1.6/pxd_lingua/exceptions.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1454 2023-04-28 09:37:51.000000 px-django-lingua-0.1.6/pxd_lingua/loader.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     8069 2023-04-28 09:37:51.000000 px-django-lingua-0.1.6/pxd_lingua/magic.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     5013 2023-04-28 09:37:51.000000 px-django-lingua-0.1.6/pxd_lingua/models.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1733 2023-04-28 09:37:51.000000 px-django-lingua-0.1.6/pxd_lingua/query.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      139 2023-04-28 09:37:51.000000 px-django-lingua-0.1.6/pxd_lingua/types.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1737 2023-04-28 09:37:51.000000 px-django-lingua-0.1.6/pxd_lingua/utils.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       79 2023-04-28 09:48:37.077229 px-django-lingua-0.1.6/setup.cfg
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1494 2023-04-28 09:48:29.000000 px-django-lingua-0.1.6/setup.py
```

### Comparing `px-django-lingua-0.1.5/LICENSE` & `px-django-lingua-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `px-django-lingua-0.1.5/PKG-INFO` & `px-django-lingua-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: px-django-lingua
-Version: 0.1.5
+Version: 0.1.6
 Summary: Simple translations implementation for django models.
 Home-page: UNKNOWN
 Author: Alex Tkachenko
 Author-email: preusx.dev@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Lingua
 
 Simple translations implementation for django models.
 
 ## Installation
```

### Comparing `px-django-lingua-0.1.5/README.md` & `px-django-lingua-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `px-django-lingua-0.1.5/px_django_lingua.egg-info/PKG-INFO` & `px-django-lingua-0.1.6/px_django_lingua.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: px-django-lingua
-Version: 0.1.5
+Version: 0.1.6
 Summary: Simple translations implementation for django models.
 Home-page: UNKNOWN
 Author: Alex Tkachenko
 Author-email: preusx.dev@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Lingua
 
 Simple translations implementation for django models.
 
 ## Installation
```

### Comparing `px-django-lingua-0.1.5/pxd_lingua/conf.py` & `px-django-lingua-0.1.6/pxd_lingua/conf.py`

 * *Files identical despite different names*

### Comparing `px-django-lingua-0.1.5/pxd_lingua/db.py` & `px-django-lingua-0.1.6/pxd_lingua/db.py`

 * *Files identical despite different names*

### Comparing `px-django-lingua-0.1.5/pxd_lingua/loader.py` & `px-django-lingua-0.1.6/pxd_lingua/loader.py`

 * *Files identical despite different names*

### Comparing `px-django-lingua-0.1.5/pxd_lingua/magic.py` & `px-django-lingua-0.1.6/pxd_lingua/magic.py`

 * *Files identical despite different names*

### Comparing `px-django-lingua-0.1.5/pxd_lingua/models.py` & `px-django-lingua-0.1.6/pxd_lingua/models.py`

 * *Files identical despite different names*

### Comparing `px-django-lingua-0.1.5/pxd_lingua/query.py` & `px-django-lingua-0.1.6/pxd_lingua/query.py`

 * *Files identical despite different names*

### Comparing `px-django-lingua-0.1.5/pxd_lingua/utils.py` & `px-django-lingua-0.1.6/pxd_lingua/utils.py`

 * *Files identical despite different names*

### Comparing `px-django-lingua-0.1.5/setup.py` & `px-django-lingua-0.1.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,37 +22,39 @@
 setuptools.setup(
     name='px-django-lingua',
     version=version,
     author='Alex Tkachenko',
     author_email='preusx.dev@gmail.com',
     license='MIT License',
     description='Simple translations implementation for django models.',
-    install_requires=(
-        'px-settings==0.1.2',
+    install_requires=[
+        'px-settings>=0.1.2,<0.2.0',
         'django>=2.2,<4',
-    ),
-    extras_requires={
-        'dev': (
+    ],
+    extras_require={
+        'dev': [
             'pytest>=6.0,<7.0',
             'pytest-watch>=4.2,<5.0',
             'pytest-django>=4.3,<5.0',
+            'django-environ',
+            'psycopg2-binary',
             'twine',
-        ),
+        ],
     },
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(exclude=(
         'tests', 'tests.*', 'pilot', 'pilot.*'
     )),
     python_requires='>=3.6',
-    classifiers=(
+    classifiers=[
         'Development Status :: 2 - Pre-Alpha',
 
         'Programming Language :: Python :: 3',
 
         'Intended Audience :: Developers',
         'Topic :: Utilities',
 
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
-    ),
+    ],
 )
```

