# Comparing `tmp/odoo_image_changelog-0.1.0.tar.gz` & `tmp/odoo_image_changelog-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/odoo_image_changelog-0.1.0.tar", last modified: Thu Apr 20 11:35:41 2023, max compression
+gzip compressed data, was "dist/odoo_image_changelog-0.1.1.tar", last modified: Fri Apr 28 06:15:39 2023, max compression
```

## Comparing `odoo_image_changelog-0.1.0.tar` & `odoo_image_changelog-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vrenaville  (1110) docker     (998)        0 2023-04-20 11:35:41.000000 odoo_image_changelog-0.1.0/
-drwxr-xr-x   0 vrenaville  (1110) docker     (998)        0 2023-04-20 11:35:41.000000 odoo_image_changelog-0.1.0/odoo_image_changelog/
--rw-r--r--   0 vrenaville  (1110) docker     (998)     4905 2023-04-20 11:35:31.000000 odoo_image_changelog-0.1.0/odoo_image_changelog/main.py
--rw-r--r--   0 vrenaville  (1110) docker     (998)      134 2023-04-20 11:12:03.000000 odoo_image_changelog-0.1.0/odoo_image_changelog/__init__.py
--rw-r--r--   0 vrenaville  (1110) docker     (998)     4902 2023-04-20 09:36:51.000000 odoo_image_changelog-0.1.0/odoo_image_changelog/github_helpers.py
--rw-r--r--   0 vrenaville  (1110) docker     (998)        0 2023-04-20 09:33:13.000000 odoo_image_changelog-0.1.0/README.rst
--rw-r--r--   0 vrenaville  (1110) docker     (998)      355 2023-04-20 11:35:41.000000 odoo_image_changelog-0.1.0/PKG-INFO
-drwxr-xr-x   0 vrenaville  (1110) docker     (998)        0 2023-04-20 11:35:41.000000 odoo_image_changelog-0.1.0/odoo_image_changelog.egg-info/
--rw-r--r--   0 vrenaville  (1110) docker     (998)      355 2023-04-20 11:35:41.000000 odoo_image_changelog-0.1.0/odoo_image_changelog.egg-info/PKG-INFO
--rw-r--r--   0 vrenaville  (1110) docker     (998)       71 2023-04-20 11:35:41.000000 odoo_image_changelog-0.1.0/odoo_image_changelog.egg-info/entry_points.txt
--rw-r--r--   0 vrenaville  (1110) docker     (998)        1 2023-04-20 11:35:41.000000 odoo_image_changelog-0.1.0/odoo_image_changelog.egg-info/dependency_links.txt
--rw-r--r--   0 vrenaville  (1110) docker     (998)      386 2023-04-20 11:35:41.000000 odoo_image_changelog-0.1.0/odoo_image_changelog.egg-info/SOURCES.txt
--rw-r--r--   0 vrenaville  (1110) docker     (998)       21 2023-04-20 11:35:41.000000 odoo_image_changelog-0.1.0/odoo_image_changelog.egg-info/requires.txt
--rw-r--r--   0 vrenaville  (1110) docker     (998)       21 2023-04-20 11:35:41.000000 odoo_image_changelog-0.1.0/odoo_image_changelog.egg-info/top_level.txt
--rw-r--r--   0 vrenaville  (1110) docker     (998)       38 2023-04-20 11:35:41.000000 odoo_image_changelog-0.1.0/setup.cfg
--rw-r--r--   0 vrenaville  (1110) docker     (998)      619 2023-04-20 11:12:40.000000 odoo_image_changelog-0.1.0/setup.py
+drwxr-xr-x   0 vrenaville  (1110) docker     (998)        0 2023-04-28 06:15:39.000000 odoo_image_changelog-0.1.1/
+drwxr-xr-x   0 vrenaville  (1110) docker     (998)        0 2023-04-28 06:15:39.000000 odoo_image_changelog-0.1.1/odoo_image_changelog/
+-rw-r--r--   0 vrenaville  (1110) docker     (998)     4917 2023-04-28 06:00:08.000000 odoo_image_changelog-0.1.1/odoo_image_changelog/main.py
+-rw-r--r--   0 vrenaville  (1110) docker     (998)      134 2023-04-28 06:12:40.000000 odoo_image_changelog-0.1.1/odoo_image_changelog/__init__.py
+-rw-r--r--   0 vrenaville  (1110) docker     (998)     4902 2023-04-20 09:36:51.000000 odoo_image_changelog-0.1.1/odoo_image_changelog/github_helpers.py
+-rw-r--r--   0 vrenaville  (1110) docker     (998)        0 2023-04-20 09:33:13.000000 odoo_image_changelog-0.1.1/README.rst
+-rw-r--r--   0 vrenaville  (1110) docker     (998)      355 2023-04-28 06:15:39.000000 odoo_image_changelog-0.1.1/PKG-INFO
+drwxr-xr-x   0 vrenaville  (1110) docker     (998)        0 2023-04-28 06:15:39.000000 odoo_image_changelog-0.1.1/odoo_image_changelog.egg-info/
+-rw-r--r--   0 vrenaville  (1110) docker     (998)      355 2023-04-28 06:15:39.000000 odoo_image_changelog-0.1.1/odoo_image_changelog.egg-info/PKG-INFO
+-rw-r--r--   0 vrenaville  (1110) docker     (998)       71 2023-04-28 06:15:39.000000 odoo_image_changelog-0.1.1/odoo_image_changelog.egg-info/entry_points.txt
+-rw-r--r--   0 vrenaville  (1110) docker     (998)        1 2023-04-28 06:15:39.000000 odoo_image_changelog-0.1.1/odoo_image_changelog.egg-info/dependency_links.txt
+-rw-r--r--   0 vrenaville  (1110) docker     (998)      386 2023-04-28 06:15:39.000000 odoo_image_changelog-0.1.1/odoo_image_changelog.egg-info/SOURCES.txt
+-rw-r--r--   0 vrenaville  (1110) docker     (998)       21 2023-04-28 06:15:39.000000 odoo_image_changelog-0.1.1/odoo_image_changelog.egg-info/requires.txt
+-rw-r--r--   0 vrenaville  (1110) docker     (998)       21 2023-04-28 06:15:39.000000 odoo_image_changelog-0.1.1/odoo_image_changelog.egg-info/top_level.txt
+-rw-r--r--   0 vrenaville  (1110) docker     (998)       38 2023-04-28 06:15:39.000000 odoo_image_changelog-0.1.1/setup.cfg
+-rw-r--r--   0 vrenaville  (1110) docker     (998)      619 2023-04-28 06:04:07.000000 odoo_image_changelog-0.1.1/setup.py
```

### Comparing `odoo_image_changelog-0.1.0/odoo_image_changelog/main.py` & `odoo_image_changelog-0.1.1/odoo_image_changelog/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         # for stable do it manually and tag release as stable
         if not stable:
             # if no previous hash we just set previous_hash as the
             # current one
             if not previous_hash:
                 hash_yaml["previous_hash"] = current_hash
             else:
-                hash_yaml["previous_hash"] = previous_hash
+                hash_yaml["previous_hash"] = hash_yaml["current_hash"]
             hash_yaml["current_hash"] = current_hash
         # Then we will update it
         githubinstance.update_changelog(
             current_running_build,
             change_log_file,
             changelog_string,
             hash_to_string(data=hash_yaml),
```

### Comparing `odoo_image_changelog-0.1.0/odoo_image_changelog/github_helpers.py` & `odoo_image_changelog-0.1.1/odoo_image_changelog/github_helpers.py`

 * *Files identical despite different names*

### Comparing `odoo_image_changelog-0.1.0/setup.py` & `odoo_image_changelog-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="odoo_image_changelog",
-    version="0.1.0",
+    version="0.1.1",
     description="a odoo changelog generator",
     url="https://github.com/camptocamp/odoo-image-changelog",
     author="Camptocamp (Vincent Renaville)",
     author_email="vincent.renaville@camptocamp.com",
     packages=["odoo_image_changelog"],
     install_requires=[
         "PyGithub",
```

