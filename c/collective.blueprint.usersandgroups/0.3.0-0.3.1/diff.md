# Comparing `tmp/collective.blueprint.usersandgroups-0.3.0.tar.gz` & `tmp/collective.blueprint.usersandgroups-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.blueprint.usersandgroups-0.3.0.tar", last modified: Tue Sep 28 12:47:20 2021, max compression
+gzip compressed data, was "collective.blueprint.usersandgroups-0.3.1.tar", last modified: Fri Apr 28 15:15:29 2023, max compression
```

## Comparing `collective.blueprint.usersandgroups-0.3.0.tar` & `collective.blueprint.usersandgroups-0.3.1.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/docs/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4706 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/docs/Makefile
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     8529 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/docs/conf.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      493 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/docs/creategroup.rst
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      769 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/docs/createuser.rst
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      863 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/docs/index.rst
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1531 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/docs/updategroupproperty.rst
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1025 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/docs/updateuserproperty.rst
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/src/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/src/collective/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/src/collective/blueprint/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/src/collective/blueprint/usersandgroups/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/src/collective/blueprint/usersandgroups/tests/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       24 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/src/collective/blueprint/usersandgroups/tests/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     3763 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/src/collective/blueprint/usersandgroups/tests/test_blueprint.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       24 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/src/collective/blueprint/usersandgroups/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     6169 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/src/collective/blueprint/usersandgroups/blueprint.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      630 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/src/collective/blueprint/usersandgroups/configure.zcml
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1162 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/src/collective/blueprint/usersandgroups/testing.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       80 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/src/collective/blueprint/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       80 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/src/collective/__init__.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/src/collective.blueprint.usersandgroups.egg-info/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4999 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/src/collective.blueprint.usersandgroups.egg-info/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1145 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/src/collective.blueprint.usersandgroups.egg-info/SOURCES.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/src/collective.blueprint.usersandgroups.egg-info/dependency_links.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      160 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/src/collective.blueprint.usersandgroups.egg-info/entry_points.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       32 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/src/collective.blueprint.usersandgroups.egg-info/namespace_packages.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/src/collective.blueprint.usersandgroups.egg-info/not-zip-safe
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       73 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/src/collective.blueprint.usersandgroups.egg-info/requires.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       11 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/src/collective.blueprint.usersandgroups.egg-info/top_level.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      266 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/CHANGES.rst
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       92 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/CONTRIBUTORS.rst
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      586 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/DEVELOP.rst
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      667 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/LICENSE.rst
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       67 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/MANIFEST.in
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2673 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/README.rst
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      302 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/setup.cfg
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2339 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/setup.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4999 2021-09-28 12:47:20.000000 collective.blueprint.usersandgroups-0.3.0/PKG-INFO
+drwxr-xr-x   0 s052328876 (528630615) domain users (528600513)        0 2023-04-28 15:15:29.367884 collective.blueprint.usersandgroups-0.3.1/
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)      399 2023-04-28 15:15:28.000000 collective.blueprint.usersandgroups-0.3.1/CHANGES.rst
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)       92 2023-04-28 15:15:28.000000 collective.blueprint.usersandgroups-0.3.1/CONTRIBUTORS.rst
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)      586 2023-04-28 15:15:28.000000 collective.blueprint.usersandgroups-0.3.1/DEVELOP.rst
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)    18092 2023-04-28 15:15:28.000000 collective.blueprint.usersandgroups-0.3.1/LICENSE.GPL
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)      667 2023-04-28 15:15:28.000000 collective.blueprint.usersandgroups-0.3.1/LICENSE.rst
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)      127 2023-04-28 15:15:28.000000 collective.blueprint.usersandgroups-0.3.1/MANIFEST.in
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     4507 2023-04-28 15:15:29.367884 collective.blueprint.usersandgroups-0.3.1/PKG-INFO
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     2673 2023-04-28 15:15:28.000000 collective.blueprint.usersandgroups-0.3.1/README.rst
+drwxr-xr-x   0 s052328876 (528630615) domain users (528600513)        0 2023-04-28 15:15:29.359883 collective.blueprint.usersandgroups-0.3.1/docs/
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     4706 2023-04-28 15:15:28.000000 collective.blueprint.usersandgroups-0.3.1/docs/Makefile
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     8529 2023-04-28 15:15:28.000000 collective.blueprint.usersandgroups-0.3.1/docs/conf.py
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)      493 2023-04-28 15:15:28.000000 collective.blueprint.usersandgroups-0.3.1/docs/creategroup.rst
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)      769 2023-04-28 15:15:28.000000 collective.blueprint.usersandgroups-0.3.1/docs/createuser.rst
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)      863 2023-04-28 15:15:28.000000 collective.blueprint.usersandgroups-0.3.1/docs/index.rst
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     1531 2023-04-28 15:15:28.000000 collective.blueprint.usersandgroups-0.3.1/docs/updategroupproperty.rst
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     1025 2023-04-28 15:15:28.000000 collective.blueprint.usersandgroups-0.3.1/docs/updateuserproperty.rst
+drwxr-xr-x   0 s052328876 (528630615) domain users (528600513)        0 2023-04-28 15:15:29.359883 collective.blueprint.usersandgroups-0.3.1/export_scripts/
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     7074 2023-04-28 15:15:28.000000 collective.blueprint.usersandgroups-0.3.1/export_scripts/plone2.0_export.py
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)      302 2023-04-28 15:15:29.371883 collective.blueprint.usersandgroups-0.3.1/setup.cfg
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     2387 2023-04-28 15:15:28.000000 collective.blueprint.usersandgroups-0.3.1/setup.py
+drwxr-xr-x   0 s052328876 (528630615) domain users (528600513)        0 2023-04-28 15:15:29.355883 collective.blueprint.usersandgroups-0.3.1/src/
+drwxr-xr-x   0 s052328876 (528630615) domain users (528600513)        0 2023-04-28 15:15:29.359883 collective.blueprint.usersandgroups-0.3.1/src/collective/
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)       80 2023-04-28 15:15:28.000000 collective.blueprint.usersandgroups-0.3.1/src/collective/__init__.py
+drwxr-xr-x   0 s052328876 (528630615) domain users (528600513)        0 2023-04-28 15:15:29.367884 collective.blueprint.usersandgroups-0.3.1/src/collective/blueprint/
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)       80 2023-04-28 15:15:28.000000 collective.blueprint.usersandgroups-0.3.1/src/collective/blueprint/__init__.py
+drwxr-xr-x   0 s052328876 (528630615) domain users (528600513)        0 2023-04-28 15:15:29.367884 collective.blueprint.usersandgroups-0.3.1/src/collective/blueprint/usersandgroups/
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)       24 2023-04-28 15:15:28.000000 collective.blueprint.usersandgroups-0.3.1/src/collective/blueprint/usersandgroups/__init__.py
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     6169 2023-04-28 15:15:28.000000 collective.blueprint.usersandgroups-0.3.1/src/collective/blueprint/usersandgroups/blueprint.py
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)      630 2023-04-28 15:15:28.000000 collective.blueprint.usersandgroups-0.3.1/src/collective/blueprint/usersandgroups/configure.zcml
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     1162 2023-04-28 15:15:28.000000 collective.blueprint.usersandgroups-0.3.1/src/collective/blueprint/usersandgroups/testing.py
+drwxr-xr-x   0 s052328876 (528630615) domain users (528600513)        0 2023-04-28 15:15:29.367884 collective.blueprint.usersandgroups-0.3.1/src/collective/blueprint/usersandgroups/tests/
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)       24 2023-04-28 15:15:28.000000 collective.blueprint.usersandgroups-0.3.1/src/collective/blueprint/usersandgroups/tests/__init__.py
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     3763 2023-04-28 15:15:28.000000 collective.blueprint.usersandgroups-0.3.1/src/collective/blueprint/usersandgroups/tests/test_blueprint.py
+drwxr-xr-x   0 s052328876 (528630615) domain users (528600513)        0 2023-04-28 15:15:29.367884 collective.blueprint.usersandgroups-0.3.1/src/collective.blueprint.usersandgroups.egg-info/
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     4507 2023-04-28 15:15:29.000000 collective.blueprint.usersandgroups-0.3.1/src/collective.blueprint.usersandgroups.egg-info/PKG-INFO
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)     1191 2023-04-28 15:15:29.000000 collective.blueprint.usersandgroups-0.3.1/src/collective.blueprint.usersandgroups.egg-info/SOURCES.txt
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)        1 2023-04-28 15:15:29.000000 collective.blueprint.usersandgroups-0.3.1/src/collective.blueprint.usersandgroups.egg-info/dependency_links.txt
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)      160 2023-04-28 15:15:29.000000 collective.blueprint.usersandgroups-0.3.1/src/collective.blueprint.usersandgroups.egg-info/entry_points.txt
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)       32 2023-04-28 15:15:29.000000 collective.blueprint.usersandgroups-0.3.1/src/collective.blueprint.usersandgroups.egg-info/namespace_packages.txt
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)        1 2023-04-28 15:15:29.000000 collective.blueprint.usersandgroups-0.3.1/src/collective.blueprint.usersandgroups.egg-info/not-zip-safe
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)       73 2023-04-28 15:15:29.000000 collective.blueprint.usersandgroups-0.3.1/src/collective.blueprint.usersandgroups.egg-info/requires.txt
+-rw-r--r--   0 s052328876 (528630615) domain users (528600513)       11 2023-04-28 15:15:29.000000 collective.blueprint.usersandgroups-0.3.1/src/collective.blueprint.usersandgroups.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `collective.blueprint.usersandgroups-0.3.0/docs/Makefile` & `collective.blueprint.usersandgroups-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `collective.blueprint.usersandgroups-0.3.0/docs/conf.py` & `collective.blueprint.usersandgroups-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `collective.blueprint.usersandgroups-0.3.0/docs/createuser.rst` & `collective.blueprint.usersandgroups-0.3.1/docs/createuser.rst`

 * *Files identical despite different names*

### Comparing `collective.blueprint.usersandgroups-0.3.0/docs/index.rst` & `collective.blueprint.usersandgroups-0.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `collective.blueprint.usersandgroups-0.3.0/docs/updategroupproperty.rst` & `collective.blueprint.usersandgroups-0.3.1/docs/updategroupproperty.rst`

 * *Files identical despite different names*

### Comparing `collective.blueprint.usersandgroups-0.3.0/docs/updateuserproperty.rst` & `collective.blueprint.usersandgroups-0.3.1/docs/updateuserproperty.rst`

 * *Files identical despite different names*

### Comparing `collective.blueprint.usersandgroups-0.3.0/src/collective/blueprint/usersandgroups/tests/test_blueprint.py` & `collective.blueprint.usersandgroups-0.3.1/src/collective/blueprint/usersandgroups/tests/test_blueprint.py`

 * *Files identical despite different names*

### Comparing `collective.blueprint.usersandgroups-0.3.0/src/collective/blueprint/usersandgroups/blueprint.py` & `collective.blueprint.usersandgroups-0.3.1/src/collective/blueprint/usersandgroups/blueprint.py`

 * *Files identical despite different names*

### Comparing `collective.blueprint.usersandgroups-0.3.0/src/collective/blueprint/usersandgroups/configure.zcml` & `collective.blueprint.usersandgroups-0.3.1/src/collective/blueprint/usersandgroups/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.blueprint.usersandgroups-0.3.0/src/collective/blueprint/usersandgroups/testing.py` & `collective.blueprint.usersandgroups-0.3.1/src/collective/blueprint/usersandgroups/testing.py`

 * *Files identical despite different names*

### Comparing `collective.blueprint.usersandgroups-0.3.0/src/collective.blueprint.usersandgroups.egg-info/SOURCES.txt` & `collective.blueprint.usersandgroups-0.3.1/src/collective.blueprint.usersandgroups.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 CHANGES.rst
 CONTRIBUTORS.rst
 DEVELOP.rst
+LICENSE.GPL
 LICENSE.rst
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 docs/Makefile
 docs/conf.py
 docs/creategroup.rst
 docs/createuser.rst
 docs/index.rst
 docs/updategroupproperty.rst
 docs/updateuserproperty.rst
+export_scripts/plone2.0_export.py
 src/collective/__init__.py
 src/collective.blueprint.usersandgroups.egg-info/PKG-INFO
 src/collective.blueprint.usersandgroups.egg-info/SOURCES.txt
 src/collective.blueprint.usersandgroups.egg-info/dependency_links.txt
 src/collective.blueprint.usersandgroups.egg-info/entry_points.txt
 src/collective.blueprint.usersandgroups.egg-info/namespace_packages.txt
 src/collective.blueprint.usersandgroups.egg-info/not-zip-safe
```

### Comparing `collective.blueprint.usersandgroups-0.3.0/DEVELOP.rst` & `collective.blueprint.usersandgroups-0.3.1/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `collective.blueprint.usersandgroups-0.3.0/LICENSE.rst` & `collective.blueprint.usersandgroups-0.3.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.blueprint.usersandgroups-0.3.0/README.rst` & `collective.blueprint.usersandgroups-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `collective.blueprint.usersandgroups-0.3.0/setup.py` & `collective.blueprint.usersandgroups-0.3.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,19 +12,20 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="collective.blueprint.usersandgroups",
-    version='0.3.0',
+    version='0.3.1',
     description="transmogrifier blueprints for importing users and groups into plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
+        "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
         "Framework :: Plone :: 4.3",
         "Framework :: Plone :: 5.1",
         "Framework :: Plone :: 5.2",
         "Programming Language :: Python",
@@ -46,15 +47,15 @@
     },
     license="GPL version 2",
     packages=find_packages("src", exclude=["ez_setup"]),
     namespace_packages=["collective", "collective.blueprint"],
     package_dir={"": "src"},
     include_package_data=True,
     zip_safe=False,
-    python_requires="==2.7, >=3.7",
+    python_requires=">=2.7",
     install_requires=[
         "collective.transmogrifier",
         "setuptools",
     ],
     extras_require={
         "test": ["plone.api", "plone.app.testing"],
     },
```

