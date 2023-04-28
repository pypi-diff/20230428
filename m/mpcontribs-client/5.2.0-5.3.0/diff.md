# Comparing `tmp/mpcontribs-client-5.2.0.tar.gz` & `tmp/mpcontribs-client-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpcontribs-client-5.2.0.tar", last modified: Wed Apr 26 20:00:15 2023, max compression
+gzip compressed data, was "mpcontribs-client-5.3.0.tar", last modified: Fri Apr 28 00:40:23 2023, max compression
```

## Comparing `mpcontribs-client-5.2.0.tar` & `mpcontribs-client-5.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:00:15.293482 mpcontribs-client-5.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-26 20:00:15.293482 mpcontribs-client-5.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:00:15.289482 mpcontribs-client-5.2.0/mpcontribs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:00:15.289482 mpcontribs-client-5.2.0/mpcontribs/client/
--rw-r--r--   0 runner    (1001) docker     (123)    81148 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/mpcontribs/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:00:15.289482 mpcontribs-client-5.2.0/mpcontribs_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-26 20:00:14.000000 mpcontribs-client-5.2.0/mpcontribs_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-26 20:00:15.000000 mpcontribs-client-5.2.0/mpcontribs_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:00:14.000000 mpcontribs-client-5.2.0/mpcontribs_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:00:14.000000 mpcontribs-client-5.2.0/mpcontribs_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-26 20:00:14.000000 mpcontribs-client-5.2.0/mpcontribs_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 20:00:14.000000 mpcontribs-client-5.2.0/mpcontribs_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:00:15.293482 mpcontribs-client-5.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/macos-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/macos-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/macos-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/macos-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/macos-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/macos-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/ubuntu-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/ubuntu-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 20:00:15.293482 mpcontribs-client-5.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:00:15.293482 mpcontribs-client-5.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:40:23.267774 mpcontribs-client-5.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-28 00:40:11.000000 mpcontribs-client-5.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-28 00:40:23.267774 mpcontribs-client-5.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-28 00:40:11.000000 mpcontribs-client-5.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:40:23.263774 mpcontribs-client-5.3.0/mpcontribs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:40:23.263774 mpcontribs-client-5.3.0/mpcontribs/client/
+-rw-r--r--   0 runner    (1001) docker     (123)    83315 2023-04-28 00:40:11.000000 mpcontribs-client-5.3.0/mpcontribs/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:40:23.263774 mpcontribs-client-5.3.0/mpcontribs_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-28 00:40:22.000000 mpcontribs-client-5.3.0/mpcontribs_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-28 00:40:23.000000 mpcontribs-client-5.3.0/mpcontribs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:40:22.000000 mpcontribs-client-5.3.0/mpcontribs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:40:22.000000 mpcontribs-client-5.3.0/mpcontribs_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-28 00:40:22.000000 mpcontribs-client-5.3.0/mpcontribs_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 00:40:22.000000 mpcontribs-client-5.3.0/mpcontribs_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:40:23.267774 mpcontribs-client-5.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-04-28 00:40:11.000000 mpcontribs-client-5.3.0/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-28 00:40:11.000000 mpcontribs-client-5.3.0/requirements/macos-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-04-28 00:40:11.000000 mpcontribs-client-5.3.0/requirements/macos-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-04-28 00:40:11.000000 mpcontribs-client-5.3.0/requirements/macos-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-04-28 00:40:11.000000 mpcontribs-client-5.3.0/requirements/macos-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-04-28 00:40:11.000000 mpcontribs-client-5.3.0/requirements/macos-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-04-28 00:40:11.000000 mpcontribs-client-5.3.0/requirements/macos-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-04-28 00:40:11.000000 mpcontribs-client-5.3.0/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-04-28 00:40:11.000000 mpcontribs-client-5.3.0/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-28 00:40:11.000000 mpcontribs-client-5.3.0/requirements/ubuntu-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-04-28 00:40:11.000000 mpcontribs-client-5.3.0/requirements/ubuntu-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-28 00:40:11.000000 mpcontribs-client-5.3.0/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-04-28 00:40:11.000000 mpcontribs-client-5.3.0/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 00:40:23.267774 mpcontribs-client-5.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-28 00:40:11.000000 mpcontribs-client-5.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:40:23.267774 mpcontribs-client-5.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-28 00:40:11.000000 mpcontribs-client-5.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-28 00:40:11.000000 mpcontribs-client-5.3.0/tests/test_client.py
```

### Comparing `mpcontribs-client-5.2.0/LICENSE` & `mpcontribs-client-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.2.0/PKG-INFO` & `mpcontribs-client-5.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcontribs-client
-Version: 5.2.0
+Version: 5.3.0
 Summary: client library for MPContribs API
 Home-page: https://github.com/materialsproject/MPContribs/tree/master/mpcontribs-client
 Author: Patrick Huck
 Author-email: phuck@lbl.gov
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mpcontribs-client-5.2.0/README.md` & `mpcontribs-client-5.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.2.0/mpcontribs/client/__init__.py` & `mpcontribs-client-5.3.0/mpcontribs/client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -890,14 +890,73 @@
         project = {
             "name": name, "title": title, "authors": authors, "description": description,
             "references": [{"label": "REF", "url": url}]
         }
         owner = self.projects.createProject(project=project).result().get("owner")
         logger.info(f"Project `{name}` created with owner `{owner}`")
 
+    def update_project(self, update: dict, name: str = None):
+        """Update project info
+
+        Args:
+            update (dict): dictionary containing project info to update
+            name (str): name of the project
+        """
+        if not update:
+            logger.warning("nothing to update")
+            return
+
+        name = self.project or name
+        if not name:
+            logger.error("initialize client with project or set `name` argument!")
+            return
+
+        disallowed = ["is_approved", "stats", "columns", "is_public", "owner"]
+        for k in disallowed:
+            if k in update:
+                logger.warning(f"removing `{k}` from update - not allowed.")
+                update.pop(k)
+                if k == "columns":
+                    logger.info("use `client.init_columns()` to update project columns.")
+                elif k == "is_public":
+                    logger.info("use `client.make_public/private()` to set `is_public`.")
+
+        if not update:
+            logger.warning("nothing to update")
+            return
+
+        fields = list(self.get_model("ProjectsSchema")._properties.keys())
+        for k in disallowed:
+            fields.remove(k)
+
+        fields.append("stats.contributions")
+        project = self.get_project(name=name, fields=fields)
+
+        # allow name update only if no contributions in project
+        if "name" in update and project["stats"]["contributions"] > 0:
+            logger.warning("removing `name` from update - not allowed.")
+            update.pop("name")
+            logger.error("cannot change project name after contributions submitted.")
+
+        payload = {
+            k: v for k, v in update.items()
+            if v and k in fields and project.get(k, None) != v
+        }
+        if not payload:
+            logger.warning("nothing to update")
+            return
+
+        valid, error = self._is_valid_payload("Project", payload)
+        if valid:
+            resp = self.projects.updateProjectByName(pk=name, project=payload).result()
+            if not resp.get("count", 0):
+                logger.error(resp)
+        else:
+            logger.error(error)
+
     def get_contribution(self, cid: str) -> Type[Dict]:
         """Retrieve full contribution entry
 
         Args:
             cid (str): contribution ObjectID
         """
         fields = list(self.get_model("ContributionsSchema")._properties.keys())
```

### Comparing `mpcontribs-client-5.2.0/mpcontribs_client.egg-info/PKG-INFO` & `mpcontribs-client-5.3.0/mpcontribs_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcontribs-client
-Version: 5.2.0
+Version: 5.3.0
 Summary: client library for MPContribs API
 Home-page: https://github.com/materialsproject/MPContribs/tree/master/mpcontribs-client
 Author: Patrick Huck
 Author-email: phuck@lbl.gov
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mpcontribs-client-5.2.0/mpcontribs_client.egg-info/SOURCES.txt` & `mpcontribs-client-5.3.0/mpcontribs_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.2.0/requirements/deployment.txt` & `mpcontribs-client-5.3.0/requirements/deployment.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.2.0/requirements/macos-latest_py3.10.txt` & `mpcontribs-client-5.3.0/requirements/macos-latest_py3.10.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 appnope==0.1.3
     # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
-attrs==22.2.0
+attrs==23.1.0
     # via jsonschema
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
@@ -79,38 +79,38 @@
 monotonic==1.6
     # via bravado
 monty==2023.4.10
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.31.0
+mp-api==0.32.0
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.2
+numpy==1.24.3
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
-palettable==3.3.1
+palettable==3.3.3
     # via pymatgen
 pandas==2.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
@@ -134,15 +134,15 @@
     # via stack-data
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pydantic==1.10.7
     # via emmet-core
-pygments==2.15.0
+pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   mp-api
```

### Comparing `mpcontribs-client-5.2.0/requirements/macos-latest_py3.10_extras.txt` & `mpcontribs-client-5.3.0/requirements/macos-latest_py3.10_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 appnope==0.1.3
     # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
-attrs==22.2.0
+attrs==23.1.0
     # via jsonschema
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
@@ -91,39 +91,39 @@
 monotonic==1.6
     # via bravado
 monty==2023.4.10
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.31.0
+mp-api==0.32.0
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.2
+numpy==1.24.3
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
     #   pytest
-palettable==3.3.1
+palettable==3.3.3
     # via pymatgen
 pandas==2.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
@@ -159,15 +159,15 @@
     # via
     #   flake8
     #   pytest-pycodestyle
 pydantic==1.10.7
     # via emmet-core
 pyflakes==3.0.1
     # via flake8
-pygments==2.15.0
+pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   mp-api
```

### Comparing `mpcontribs-client-5.2.0/requirements/macos-latest_py3.8.txt` & `mpcontribs-client-5.3.0/requirements/macos-latest_py3.8.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 appnope==0.1.3
     # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
-attrs==22.2.0
+attrs==23.1.0
     # via jsonschema
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
@@ -83,38 +83,38 @@
 monotonic==1.6
     # via bravado
 monty==2023.4.10
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.31.0
+mp-api==0.32.0
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.2
+numpy==1.24.3
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
-palettable==3.3.1
+palettable==3.3.3
     # via pymatgen
 pandas==2.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
@@ -140,15 +140,15 @@
     # via stack-data
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pydantic==1.10.7
     # via emmet-core
-pygments==2.15.0
+pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   mp-api
```

### Comparing `mpcontribs-client-5.2.0/requirements/macos-latest_py3.8_extras.txt` & `mpcontribs-client-5.3.0/requirements/macos-latest_py3.8_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 appnope==0.1.3
     # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
-attrs==22.2.0
+attrs==23.1.0
     # via jsonschema
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
@@ -95,39 +95,39 @@
 monotonic==1.6
     # via bravado
 monty==2023.4.10
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.31.0
+mp-api==0.32.0
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.2
+numpy==1.24.3
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
     #   pytest
-palettable==3.3.1
+palettable==3.3.3
     # via pymatgen
 pandas==2.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
@@ -165,15 +165,15 @@
     # via
     #   flake8
     #   pytest-pycodestyle
 pydantic==1.10.7
     # via emmet-core
 pyflakes==3.0.1
     # via flake8
-pygments==2.15.0
+pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   mp-api
```

### Comparing `mpcontribs-client-5.2.0/requirements/macos-latest_py3.9.txt` & `mpcontribs-client-5.3.0/requirements/macos-latest_py3.9.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 appnope==0.1.3
     # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
-attrs==22.2.0
+attrs==23.1.0
     # via jsonschema
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
@@ -81,38 +81,38 @@
 monotonic==1.6
     # via bravado
 monty==2023.4.10
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.31.0
+mp-api==0.32.0
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.2
+numpy==1.24.3
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
-palettable==3.3.1
+palettable==3.3.3
     # via pymatgen
 pandas==2.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
@@ -136,15 +136,15 @@
     # via stack-data
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pydantic==1.10.7
     # via emmet-core
-pygments==2.15.0
+pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   mp-api
```

### Comparing `mpcontribs-client-5.2.0/requirements/macos-latest_py3.9_extras.txt` & `mpcontribs-client-5.3.0/requirements/macos-latest_py3.9_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 appnope==0.1.3
     # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
-attrs==22.2.0
+attrs==23.1.0
     # via jsonschema
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
@@ -93,39 +93,39 @@
 monotonic==1.6
     # via bravado
 monty==2023.4.10
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.31.0
+mp-api==0.32.0
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.2
+numpy==1.24.3
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
     #   pytest
-palettable==3.3.1
+palettable==3.3.3
     # via pymatgen
 pandas==2.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
@@ -161,15 +161,15 @@
     # via
     #   flake8
     #   pytest-pycodestyle
 pydantic==1.10.7
     # via emmet-core
 pyflakes==3.0.1
     # via flake8
-pygments==2.15.0
+pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   mp-api
```

### Comparing `mpcontribs-client-5.2.0/requirements/ubuntu-latest_py3.10.txt` & `mpcontribs-client-5.3.0/requirements/ubuntu-latest_py3.10.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 #    pip-compile --output-file=requirements/ubuntu-latest_py3.10.txt --resolver=backtracking
 #
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
-attrs==22.2.0
+attrs==23.1.0
     # via jsonschema
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
@@ -77,38 +77,38 @@
 monotonic==1.6
     # via bravado
 monty==2023.4.10
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.31.0
+mp-api==0.32.0
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.2
+numpy==1.24.3
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
-palettable==3.3.1
+palettable==3.3.3
     # via pymatgen
 pandas==2.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
@@ -132,15 +132,15 @@
     # via stack-data
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pydantic==1.10.7
     # via emmet-core
-pygments==2.15.0
+pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   mp-api
```

### Comparing `mpcontribs-client-5.2.0/requirements/ubuntu-latest_py3.10_extras.txt` & `mpcontribs-client-5.3.0/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 #    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt --resolver=backtracking
 #
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
-attrs==22.2.0
+attrs==23.1.0
     # via jsonschema
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
@@ -89,39 +89,39 @@
 monotonic==1.6
     # via bravado
 monty==2023.4.10
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.31.0
+mp-api==0.32.0
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.2
+numpy==1.24.3
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
     #   pytest
-palettable==3.3.1
+palettable==3.3.3
     # via pymatgen
 pandas==2.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
@@ -157,15 +157,15 @@
     # via
     #   flake8
     #   pytest-pycodestyle
 pydantic==1.10.7
     # via emmet-core
 pyflakes==3.0.1
     # via flake8
-pygments==2.15.0
+pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   mp-api
```

### Comparing `mpcontribs-client-5.2.0/requirements/ubuntu-latest_py3.8.txt` & `mpcontribs-client-5.3.0/requirements/ubuntu-latest_py3.8.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 #    pip-compile --output-file=requirements/ubuntu-latest_py3.8.txt --resolver=backtracking
 #
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
-attrs==22.2.0
+attrs==23.1.0
     # via jsonschema
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
@@ -81,38 +81,38 @@
 monotonic==1.6
     # via bravado
 monty==2023.4.10
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.31.0
+mp-api==0.32.0
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.2
+numpy==1.24.3
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
-palettable==3.3.1
+palettable==3.3.3
     # via pymatgen
 pandas==2.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
@@ -138,15 +138,15 @@
     # via stack-data
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pydantic==1.10.7
     # via emmet-core
-pygments==2.15.0
+pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   mp-api
```

### Comparing `mpcontribs-client-5.2.0/requirements/ubuntu-latest_py3.8_extras.txt` & `mpcontribs-client-5.3.0/requirements/ubuntu-latest_py3.8_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 #    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.8_extras.txt --resolver=backtracking
 #
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
-attrs==22.2.0
+attrs==23.1.0
     # via jsonschema
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
@@ -93,39 +93,39 @@
 monotonic==1.6
     # via bravado
 monty==2023.4.10
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.31.0
+mp-api==0.32.0
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.2
+numpy==1.24.3
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
     #   pytest
-palettable==3.3.1
+palettable==3.3.3
     # via pymatgen
 pandas==2.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
@@ -163,15 +163,15 @@
     # via
     #   flake8
     #   pytest-pycodestyle
 pydantic==1.10.7
     # via emmet-core
 pyflakes==3.0.1
     # via flake8
-pygments==2.15.0
+pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   mp-api
```

### Comparing `mpcontribs-client-5.2.0/requirements/ubuntu-latest_py3.9.txt` & `mpcontribs-client-5.3.0/requirements/ubuntu-latest_py3.9.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 #    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt --resolver=backtracking
 #
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
-attrs==22.2.0
+attrs==23.1.0
     # via jsonschema
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
@@ -79,38 +79,38 @@
 monotonic==1.6
     # via bravado
 monty==2023.4.10
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.31.0
+mp-api==0.32.0
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.2
+numpy==1.24.3
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
-palettable==3.3.1
+palettable==3.3.3
     # via pymatgen
 pandas==2.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
@@ -134,15 +134,15 @@
     # via stack-data
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pydantic==1.10.7
     # via emmet-core
-pygments==2.15.0
+pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   mp-api
```

### Comparing `mpcontribs-client-5.2.0/requirements/ubuntu-latest_py3.9_extras.txt` & `mpcontribs-client-5.3.0/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 #    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.9_extras.txt --resolver=backtracking
 #
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
-attrs==22.2.0
+attrs==23.1.0
     # via jsonschema
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
@@ -91,39 +91,39 @@
 monotonic==1.6
     # via bravado
 monty==2023.4.10
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.31.0
+mp-api==0.32.0
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.2
+numpy==1.24.3
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
     #   pytest
-palettable==3.3.1
+palettable==3.3.3
     # via pymatgen
 pandas==2.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
@@ -159,15 +159,15 @@
     # via
     #   flake8
     #   pytest-pycodestyle
 pydantic==1.10.7
     # via emmet-core
 pyflakes==3.0.1
     # via flake8
-pygments==2.15.0
+pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   mp-api
```

### Comparing `mpcontribs-client-5.2.0/setup.py` & `mpcontribs-client-5.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.2.0/tests/test_client.py` & `mpcontribs-client-5.3.0/tests/test_client.py`

 * *Files identical despite different names*

