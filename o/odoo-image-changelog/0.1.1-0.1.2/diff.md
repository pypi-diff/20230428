# Comparing `tmp/odoo_image_changelog-0.1.1.tar.gz` & `tmp/odoo_image_changelog-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/odoo_image_changelog-0.1.1.tar", last modified: Fri Apr 28 06:15:39 2023, max compression
+gzip compressed data, was "odoo_image_changelog-0.1.2.tar", last modified: Fri Apr 28 07:55:58 2023, max compression
```

## Comparing `odoo_image_changelog-0.1.1.tar` & `odoo_image_changelog-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 vrenaville  (1110) docker     (998)        0 2023-04-28 06:15:39.000000 odoo_image_changelog-0.1.1/
-drwxr-xr-x   0 vrenaville  (1110) docker     (998)        0 2023-04-28 06:15:39.000000 odoo_image_changelog-0.1.1/odoo_image_changelog/
--rw-r--r--   0 vrenaville  (1110) docker     (998)     4917 2023-04-28 06:00:08.000000 odoo_image_changelog-0.1.1/odoo_image_changelog/main.py
--rw-r--r--   0 vrenaville  (1110) docker     (998)      134 2023-04-28 06:12:40.000000 odoo_image_changelog-0.1.1/odoo_image_changelog/__init__.py
--rw-r--r--   0 vrenaville  (1110) docker     (998)     4902 2023-04-20 09:36:51.000000 odoo_image_changelog-0.1.1/odoo_image_changelog/github_helpers.py
--rw-r--r--   0 vrenaville  (1110) docker     (998)        0 2023-04-20 09:33:13.000000 odoo_image_changelog-0.1.1/README.rst
--rw-r--r--   0 vrenaville  (1110) docker     (998)      355 2023-04-28 06:15:39.000000 odoo_image_changelog-0.1.1/PKG-INFO
-drwxr-xr-x   0 vrenaville  (1110) docker     (998)        0 2023-04-28 06:15:39.000000 odoo_image_changelog-0.1.1/odoo_image_changelog.egg-info/
--rw-r--r--   0 vrenaville  (1110) docker     (998)      355 2023-04-28 06:15:39.000000 odoo_image_changelog-0.1.1/odoo_image_changelog.egg-info/PKG-INFO
--rw-r--r--   0 vrenaville  (1110) docker     (998)       71 2023-04-28 06:15:39.000000 odoo_image_changelog-0.1.1/odoo_image_changelog.egg-info/entry_points.txt
--rw-r--r--   0 vrenaville  (1110) docker     (998)        1 2023-04-28 06:15:39.000000 odoo_image_changelog-0.1.1/odoo_image_changelog.egg-info/dependency_links.txt
--rw-r--r--   0 vrenaville  (1110) docker     (998)      386 2023-04-28 06:15:39.000000 odoo_image_changelog-0.1.1/odoo_image_changelog.egg-info/SOURCES.txt
--rw-r--r--   0 vrenaville  (1110) docker     (998)       21 2023-04-28 06:15:39.000000 odoo_image_changelog-0.1.1/odoo_image_changelog.egg-info/requires.txt
--rw-r--r--   0 vrenaville  (1110) docker     (998)       21 2023-04-28 06:15:39.000000 odoo_image_changelog-0.1.1/odoo_image_changelog.egg-info/top_level.txt
--rw-r--r--   0 vrenaville  (1110) docker     (998)       38 2023-04-28 06:15:39.000000 odoo_image_changelog-0.1.1/setup.cfg
--rw-r--r--   0 vrenaville  (1110) docker     (998)      619 2023-04-28 06:04:07.000000 odoo_image_changelog-0.1.1/setup.py
+drwxr-xr-x   0 vrenaville  (1110) docker     (998)        0 2023-04-28 07:55:58.169784 odoo_image_changelog-0.1.2/
+-rw-r--r--   0 vrenaville  (1110) docker     (998)     1799 2023-04-20 08:54:35.000000 odoo_image_changelog-0.1.2/.gitignore
+-rw-r--r--   0 vrenaville  (1110) docker     (998)      355 2023-04-28 07:55:58.169784 odoo_image_changelog-0.1.2/PKG-INFO
+-rw-r--r--   0 vrenaville  (1110) docker     (998)        0 2023-04-20 09:33:13.000000 odoo_image_changelog-0.1.2/README.rst
+drwxr-xr-x   0 vrenaville  (1110) docker     (998)        0 2023-04-28 07:55:58.169784 odoo_image_changelog-0.1.2/odoo_image_changelog/
+-rw-r--r--   0 vrenaville  (1110) docker     (998)      132 2023-04-28 07:54:07.000000 odoo_image_changelog-0.1.2/odoo_image_changelog/__init__.py
+-rw-r--r--   0 vrenaville  (1110) docker     (998)     4902 2023-04-20 09:36:51.000000 odoo_image_changelog-0.1.2/odoo_image_changelog/github_helpers.py
+-rw-r--r--   0 vrenaville  (1110) docker     (998)     4898 2023-04-28 07:53:43.000000 odoo_image_changelog-0.1.2/odoo_image_changelog/main.py
+drwxr-xr-x   0 vrenaville  (1110) docker     (998)        0 2023-04-28 07:55:58.169784 odoo_image_changelog-0.1.2/odoo_image_changelog.egg-info/
+-rw-r--r--   0 vrenaville  (1110) docker     (998)      355 2023-04-28 07:55:58.000000 odoo_image_changelog-0.1.2/odoo_image_changelog.egg-info/PKG-INFO
+-rw-r--r--   0 vrenaville  (1110) docker     (998)      397 2023-04-28 07:55:58.000000 odoo_image_changelog-0.1.2/odoo_image_changelog.egg-info/SOURCES.txt
+-rw-r--r--   0 vrenaville  (1110) docker     (998)        1 2023-04-28 07:55:58.000000 odoo_image_changelog-0.1.2/odoo_image_changelog.egg-info/dependency_links.txt
+-rw-r--r--   0 vrenaville  (1110) docker     (998)       71 2023-04-28 07:55:58.000000 odoo_image_changelog-0.1.2/odoo_image_changelog.egg-info/entry_points.txt
+-rw-r--r--   0 vrenaville  (1110) docker     (998)       21 2023-04-28 07:55:58.000000 odoo_image_changelog-0.1.2/odoo_image_changelog.egg-info/requires.txt
+-rw-r--r--   0 vrenaville  (1110) docker     (998)       21 2023-04-28 07:55:58.000000 odoo_image_changelog-0.1.2/odoo_image_changelog.egg-info/top_level.txt
+-rw-r--r--   0 vrenaville  (1110) docker     (998)       38 2023-04-28 07:55:58.169784 odoo_image_changelog-0.1.2/setup.cfg
+-rw-r--r--   0 vrenaville  (1110) docker     (998)      619 2023-04-28 07:53:56.000000 odoo_image_changelog-0.1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `odoo_image_changelog-0.1.1/odoo_image_changelog/main.py` & `odoo_image_changelog-0.1.2/odoo_image_changelog/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,23 +45,22 @@
 ):
     if stable:
         hash_yaml = get_previous_stable_rev(current_running_build)
         hash_file = f"{current_running_build}/HASH_STABLE"
     else:
         hash_yaml = get_previous_unstable_rev(current_running_build)
         hash_file = f"{current_running_build}/HASH_UNSTABLE"
-        # We reset the current_hash for stable
-        hash_yaml["current_hash"] = ""
 
     content_array = []
     githubodooinstance = GithubHelper(githubinstance.token, ODOO_REPO)
     changelog_array, current_hash = githubodooinstance.get_changelog(
         current_running_build,
         hash_yaml["previous_hash"],
-        hash_yaml["current_hash"],
+        # We reset the current_hash for unstable
+        hash_yaml["current_hash"] if stable else "",
     )
     if changelog_array:
         if stable:
             change_log_file = f"{current_running_build}/CHANGELOG.md"
         else:
             change_log_file = f"{current_running_build}/CHANGELOG_UNSTABLE.md"
```

### Comparing `odoo_image_changelog-0.1.1/odoo_image_changelog/github_helpers.py` & `odoo_image_changelog-0.1.2/odoo_image_changelog/github_helpers.py`

 * *Files identical despite different names*

### Comparing `odoo_image_changelog-0.1.1/setup.py` & `odoo_image_changelog-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="odoo_image_changelog",
-    version="0.1.1",
+    version="0.1.2",
     description="a odoo changelog generator",
     url="https://github.com/camptocamp/odoo-image-changelog",
     author="Camptocamp (Vincent Renaville)",
     author_email="vincent.renaville@camptocamp.com",
     packages=["odoo_image_changelog"],
     install_requires=[
         "PyGithub",
```

