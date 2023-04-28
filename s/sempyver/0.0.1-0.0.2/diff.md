# Comparing `tmp/sempyver-0.0.1.tar.gz` & `tmp/sempyver-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sempyver-0.0.1.tar", last modified: Tue Apr  4 08:16:13 2023, max compression
+gzip compressed data, was "sempyver-0.0.2.tar", last modified: Fri Apr 28 08:51:16 2023, max compression
```

## Comparing `sempyver-0.0.1.tar` & `sempyver-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:16:13.244418 sempyver-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-04 08:16:02.000000 sempyver-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-04 08:16:13.244418 sempyver-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-04 08:16:02.000000 sempyver-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-04 08:16:02.000000 sempyver-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:16:13.240418 sempyver-0.0.1/sempyver/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-04 08:16:02.000000 sempyver-0.0.1/sempyver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-04 08:16:02.000000 sempyver-0.0.1/sempyver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-04 08:16:02.000000 sempyver-0.0.1/sempyver/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:16:13.244418 sempyver-0.0.1/sempyver/cli_application/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-04 08:16:02.000000 sempyver-0.0.1/sempyver/cli_application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-04-04 08:16:02.000000 sempyver-0.0.1/sempyver/cli_application/cli_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:16:13.244418 sempyver-0.0.1/sempyver/cli_application/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-04 08:16:02.000000 sempyver-0.0.1/sempyver/cli_application/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-04-04 08:16:02.000000 sempyver-0.0.1/sempyver/cli_application/modules/changelog_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-04-04 08:16:02.000000 sempyver-0.0.1/sempyver/cli_application/modules/changeset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-04 08:16:02.000000 sempyver-0.0.1/sempyver/cli_application/modules/commit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:16:13.244418 sempyver-0.0.1/sempyver/cli_application/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-04 08:16:02.000000 sempyver-0.0.1/sempyver/cli_application/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-04 08:16:02.000000 sempyver-0.0.1/sempyver/cli_application/utilities/tags_for_change.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-04 08:16:02.000000 sempyver-0.0.1/sempyver/cli_application/utilities/theme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:16:13.244418 sempyver-0.0.1/sempyver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-04 08:16:13.000000 sempyver-0.0.1/sempyver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-04 08:16:13.000000 sempyver-0.0.1/sempyver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 08:16:13.000000 sempyver-0.0.1/sempyver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-04 08:16:13.000000 sempyver-0.0.1/sempyver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-04 08:16:13.000000 sempyver-0.0.1/sempyver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-04 08:16:13.000000 sempyver-0.0.1/sempyver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 08:16:13.244418 sempyver-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-04 08:16:02.000000 sempyver-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:51:16.226146 sempyver-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-28 08:51:02.000000 sempyver-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-28 08:51:16.222145 sempyver-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-28 08:51:02.000000 sempyver-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-28 08:51:02.000000 sempyver-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:51:16.222145 sempyver-0.0.2/sempyver/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-28 08:51:02.000000 sempyver-0.0.2/sempyver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-28 08:51:02.000000 sempyver-0.0.2/sempyver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-28 08:51:02.000000 sempyver-0.0.2/sempyver/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:51:16.222145 sempyver-0.0.2/sempyver/cli_application/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-28 08:51:02.000000 sempyver-0.0.2/sempyver/cli_application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-04-28 08:51:02.000000 sempyver-0.0.2/sempyver/cli_application/cli_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:51:16.222145 sempyver-0.0.2/sempyver/cli_application/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-28 08:51:02.000000 sempyver-0.0.2/sempyver/cli_application/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-04-28 08:51:02.000000 sempyver-0.0.2/sempyver/cli_application/modules/changelog_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-04-28 08:51:02.000000 sempyver-0.0.2/sempyver/cli_application/modules/changeset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-28 08:51:02.000000 sempyver-0.0.2/sempyver/cli_application/modules/commit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:51:16.222145 sempyver-0.0.2/sempyver/cli_application/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-28 08:51:02.000000 sempyver-0.0.2/sempyver/cli_application/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-28 08:51:02.000000 sempyver-0.0.2/sempyver/cli_application/utilities/tags_for_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-28 08:51:02.000000 sempyver-0.0.2/sempyver/cli_application/utilities/theme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:51:16.222145 sempyver-0.0.2/sempyver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-28 08:51:16.000000 sempyver-0.0.2/sempyver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-28 08:51:16.000000 sempyver-0.0.2/sempyver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 08:51:16.000000 sempyver-0.0.2/sempyver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 08:51:16.000000 sempyver-0.0.2/sempyver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-28 08:51:16.000000 sempyver-0.0.2/sempyver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 08:51:16.000000 sempyver-0.0.2/sempyver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 08:51:16.226146 sempyver-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-28 08:51:02.000000 sempyver-0.0.2/setup.py
```

### Comparing `sempyver-0.0.1/LICENSE` & `sempyver-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sempyver-0.0.1/pyproject.toml` & `sempyver-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sempyver-0.0.1/sempyver/cli_application/cli_app.py` & `sempyver-0.0.2/sempyver/cli_application/cli_app.py`

 * *Files identical despite different names*

### Comparing `sempyver-0.0.1/sempyver/cli_application/modules/changelog_generator.py` & `sempyver-0.0.2/sempyver/cli_application/modules/changelog_generator.py`

 * *Files identical despite different names*

### Comparing `sempyver-0.0.1/sempyver/cli_application/modules/changeset.py` & `sempyver-0.0.2/sempyver/cli_application/modules/changeset.py`

 * *Files identical despite different names*

### Comparing `sempyver-0.0.1/sempyver/cli_application/modules/commit.py` & `sempyver-0.0.2/sempyver/cli_application/modules/commit.py`

 * *Files identical despite different names*

### Comparing `sempyver-0.0.1/sempyver/cli_application/utilities/tags_for_change.py` & `sempyver-0.0.2/sempyver/cli_application/utilities/tags_for_change.py`

 * *Files identical despite different names*

### Comparing `sempyver-0.0.1/sempyver/cli_application/utilities/theme.py` & `sempyver-0.0.2/sempyver/cli_application/utilities/theme.py`

 * *Files identical despite different names*

### Comparing `sempyver-0.0.1/sempyver.egg-info/SOURCES.txt` & `sempyver-0.0.2/sempyver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sempyver-0.0.1/setup.py` & `sempyver-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,28 +21,42 @@
     if version_coincidence is None:
         raise TypeError("Couldn't find the version in the given file.")
     version = version_coincidence.group(1)
     # Return the version
     return version
 
 
+def long_description() -> str:
+    """Open the `README.md` file and return the long description
+
+    Returns:
+        - All the `README.md` as a simple and large string
+    """
+    with open("./README.md", encoding="utf-8") as file:
+        description = file.readlines()
+    return "".join(line for line in description)
+
+
 setup(
     name='sempyver',
     version=read_version(),
-    description='Setting up a python package',
-    long_description="",  # ! TO BE ADDED
+    description='Tool for teams to manage the CHANGELOG given a list of different changes.',
+    long_description=long_description(),
+    long_description_content_type='text/markdown',
     author='Ricardo Leal',
     author_email='ricardo.lealpz@gmail.com',
     maintainer='Ricardo Leal',
     maintainer_email='ricardo.lealpz@gmail.com',
     url='',  # ! TO BE ADDED
-    packages=find_packages(include=['sempyver', 'sempyver.*']),
+    packages=find_packages(
+        include=['sempyver', 'sempyver.*', 'sempyver.helpers']),
+    include_package_data=True,
     install_requires=[
         'click~=8.1',
         'inquirer~=3.1',
         'colorama==0.4.6',
         'faker~=17.6'
     ],
     entry_points={
-        'console_scripts': ['sempyver=sempyver.__main__:run']
+        'console_scripts': ['semver=sempyver.__main__:run']
     }
 )
```

