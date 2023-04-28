# Comparing `tmp/giternity-0.5.tar.gz` & `tmp/giternity-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/giternity-0.5.tar", last modified: Mon Mar 25 20:02:00 2019, max compression
+gzip compressed data, was "giternity-0.6.tar", last modified: Fri Apr 28 19:58:57 2023, max compression
```

## Comparing `giternity-0.5.tar` & `giternity-0.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 rahiel    (1000) rahiel    (1000)        0 2019-03-25 20:02:00.000000 giternity-0.5/
--rw-r--r--   0 rahiel    (1000) rahiel    (1000)     4327 2019-03-25 20:02:00.000000 giternity-0.5/PKG-INFO
--rw-r--r--   0 rahiel    (1000) rahiel    (1000)     2916 2018-03-29 12:10:57.000000 giternity-0.5/README.md
-drwxr-xr-x   0 rahiel    (1000) rahiel    (1000)        0 2019-03-25 20:02:00.000000 giternity-0.5/giternity.egg-info/
--rw-r--r--   0 rahiel    (1000) rahiel    (1000)     4327 2019-03-25 20:02:00.000000 giternity-0.5/giternity.egg-info/PKG-INFO
--rw-r--r--   0 rahiel    (1000) rahiel    (1000)      231 2019-03-25 20:02:00.000000 giternity-0.5/giternity.egg-info/SOURCES.txt
--rw-r--r--   0 rahiel    (1000) rahiel    (1000)        1 2019-03-25 20:02:00.000000 giternity-0.5/giternity.egg-info/dependency_links.txt
--rw-r--r--   0 rahiel    (1000) rahiel    (1000)       46 2019-03-25 20:02:00.000000 giternity-0.5/giternity.egg-info/entry_points.txt
--rw-r--r--   0 rahiel    (1000) rahiel    (1000)       14 2019-03-25 20:02:00.000000 giternity-0.5/giternity.egg-info/requires.txt
--rw-r--r--   0 rahiel    (1000) rahiel    (1000)       10 2019-03-25 20:02:00.000000 giternity-0.5/giternity.egg-info/top_level.txt
--rw-r--r--   0 rahiel    (1000) rahiel    (1000)     7948 2019-03-25 20:01:32.000000 giternity-0.5/giternity.py
--rw-r--r--   0 rahiel    (1000) rahiel    (1000)       38 2019-03-25 20:02:00.000000 giternity-0.5/setup.cfg
--rw-r--r--   0 rahiel    (1000) rahiel    (1000)     1597 2018-03-29 12:11:05.000000 giternity-0.5/setup.py
+drwxr-xr-x   0 rahielkasim   (501) staff       (20)        0 2023-04-28 19:58:57.110005 giternity-0.6/
+-rw-r--r--   0 rahielkasim   (501) staff       (20)    35149 2023-04-15 12:06:43.000000 giternity-0.6/LICENSE.txt
+-rw-r--r--   0 rahielkasim   (501) staff       (20)      847 2023-04-28 19:58:57.109668 giternity-0.6/PKG-INFO
+-rw-r--r--   0 rahielkasim   (501) staff       (20)     3423 2023-04-15 12:06:43.000000 giternity-0.6/README.md
+drwxr-xr-x   0 rahielkasim   (501) staff       (20)        0 2023-04-28 19:58:57.109126 giternity-0.6/giternity.egg-info/
+-rw-r--r--   0 rahielkasim   (501) staff       (20)      847 2023-04-28 19:58:57.000000 giternity-0.6/giternity.egg-info/PKG-INFO
+-rw-r--r--   0 rahielkasim   (501) staff       (20)      243 2023-04-28 19:58:57.000000 giternity-0.6/giternity.egg-info/SOURCES.txt
+-rw-r--r--   0 rahielkasim   (501) staff       (20)        1 2023-04-28 19:58:57.000000 giternity-0.6/giternity.egg-info/dependency_links.txt
+-rw-r--r--   0 rahielkasim   (501) staff       (20)       45 2023-04-28 19:58:57.000000 giternity-0.6/giternity.egg-info/entry_points.txt
+-rw-r--r--   0 rahielkasim   (501) staff       (20)       14 2023-04-28 19:58:57.000000 giternity-0.6/giternity.egg-info/requires.txt
+-rw-r--r--   0 rahielkasim   (501) staff       (20)       10 2023-04-28 19:58:57.000000 giternity-0.6/giternity.egg-info/top_level.txt
+-rw-r--r--   0 rahielkasim   (501) staff       (20)     8493 2023-04-15 12:08:13.000000 giternity-0.6/giternity.py
+-rw-r--r--   0 rahielkasim   (501) staff       (20)       38 2023-04-28 19:58:57.110170 giternity-0.6/setup.cfg
+-rw-r--r--   0 rahielkasim   (501) staff       (20)     1597 2023-04-15 12:06:43.000000 giternity-0.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `giternity-0.5/README.md` & `giternity-0.6/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # giternity
 
 [![Version](https://img.shields.io/pypi/v/giternity.svg)](https://pypi.org/project/giternity/)
 [![pyversions](https://img.shields.io/pypi/pyversions/giternity.svg)](https://pypi.org/project/giternity/)
-[![Downloads](https://www.cpu.re/static/giternity/downloads.svg)](https://www.cpu.re/static/giternity/downloads-by-python-version.txt)
+[![Downloads](https://img.shields.io/pypi/dm/giternity)](https://pypistats.org/packages/giternity)
 [![License](https://img.shields.io/badge/License-GPLv3+-blue.svg)](https://github.com/rahiel/giternity/blob/master/LICENSE.txt)
 
 Giternity is a tool to mirror git repositories from GitHub. You can specify a
 username/organization to mirror all their repositories, or just individual
 repos. It retrieves some repo metadata so they can be nicely served with
 [cgit][]. Run giternity periodically to update the mirrors.
 
@@ -42,14 +42,30 @@
 
 [github]
 repositories = [
     "rahiel",
     "sunsistemo",
     "TeMPOraL/nyan-mode",
 ]
+
+# Include arbitrary repositories with this pattern (1 [[repos]] block
+# each):
+#
+#    [[repos]]
+#    name = "repo-name"
+#    owner = "owner"
+#    description = "description"
+#    homepage = "https://example.local"
+#    clone_url = "https://git.example.local/owner/repo-name.git"
+[[repos]]
+name = "giternity"
+owner = "rahiel"
+description = "Mirror git repositories and retrieve metadata for cgit "
+homepage = "https://www.rahielkasim.com/mirror-git-repositories-and-serve-them-with-cgit/"
+clone_url = "https://github.com/rahiel/giternity.git"
 ```
 
 Set `git_data_path` to the path where you want to store the git repositories. It
 will contain bare git repositories: the data you usually see in the `.git`
 directory in your projects. To also have the actual working files of the repos,
 set `checkout_path` to where to keep them. If you'll be hosting the repos with
 cgit, set `cgit_url` to the public URL.
```

### Comparing `giternity-0.5/giternity.py` & `giternity-0.6/giternity.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from subprocess import CalledProcessError, run
 from typing import Optional
 
 import requests
 import toml
 
 
-__version__ = "0.5"
+__version__ = "0.6"
 
 
 def main():
     parser = argparse.ArgumentParser(description="Mirror git repositories and retrieve metadata for cgit.",
                                      epilog="Homepage: https://github.com/rahiel/giternity")
     parser.add_argument("-c", "--configure", help="configure %(prog)s", action="store_true")
     parser.add_argument("--version", action="version", version="%(prog)s {}".format(__version__))
@@ -65,14 +65,28 @@
                     f.write(gh.repo_to_cgitrc(repo))
             else:
                 for repo in gh.get_repos(r):
                     path = git_data_path + repo["full_name"] + "/"
                     mirror(repo["clone_url"], path)
                     with open(path + "cgitrc", "w") as f:
                         f.write(gh.repo_to_cgitrc(repo))
+    else:
+        gh = Github(cgit_url=cgit_url)
+
+    # Arbitrary git repositories
+    arbitrary_repos = config.get("repos")
+    if arbitrary_repos:
+        for repo in arbitrary_repos:
+            repo['full_name'] = '{}/{}'.format(repo['owner'], repo['name'])
+            path = "{}{}.git/".format(git_data_path, repo['full_name'])
+            url = repo["clone_url"]
+            metadata = gh.repo_to_cgitrc(repo)
+            mirror(repo["clone_url"], path)
+            with open(path + "cgitrc", "w") as f:
+                f.write(metadata)
 
     def find_repos(path: str):
         for entry in os.scandir(path):
             if entry.is_dir():
                 if is_bare_repo(entry.path):
                     clone(entry.path, entry.path.replace(git_data_path, checkout_path))
                 else:
```

### Comparing `giternity-0.5/setup.py` & `giternity-0.6/setup.py`

 * *Files identical despite different names*

