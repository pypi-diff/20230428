# Comparing `tmp/obiba_opal-5.1.0.tar.gz` & `tmp/obiba_opal-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obiba_opal-5.1.0.tar", max compression
+gzip compressed data, was "obiba_opal-5.1.1.tar", max compression
```

## Comparing `obiba_opal-5.1.0.tar` & `obiba_opal-5.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    35147 2023-03-10 10:48:57.333324 obiba_opal-5.1.0/LICENSE.txt
--rw-r--r--   0        0        0     3571 2023-03-10 10:48:57.333324 obiba_opal-5.1.0/README.md
--rw-r--r--   0        0        0     1536 2023-03-10 10:48:57.333324 obiba_opal-5.1.0/obiba_opal/__init__.py
--rw-r--r--   0        0        0     6537 2023-03-10 10:48:57.337322 obiba_opal-5.1.0/obiba_opal/analysis.py
--rwxr-xr-x   0        0        0    13633 2023-03-10 10:48:57.337322 obiba_opal-5.1.0/obiba_opal/console.py
--rwxr-xr-x   0        0        0    19710 2023-03-10 10:48:57.337322 obiba_opal-5.1.0/obiba_opal/core.py
--rwxr-xr-x   0        0        0     7183 2023-03-10 10:48:57.337322 obiba_opal-5.1.0/obiba_opal/data.py
--rwxr-xr-x   0        0        0    14684 2023-03-10 10:48:57.337322 obiba_opal-5.1.0/obiba_opal/dictionary.py
--rw-r--r--   0        0        0    24652 2023-03-10 10:48:57.337322 obiba_opal-5.1.0/obiba_opal/exports.py
--rwxr-xr-x   0        0        0     4776 2023-03-10 10:48:57.337322 obiba_opal-5.1.0/obiba_opal/file.py
--rw-r--r--   0        0        0    47546 2023-03-10 10:48:57.337322 obiba_opal-5.1.0/obiba_opal/imports.py
--rw-r--r--   0        0        0    12875 2023-03-10 10:48:57.337322 obiba_opal-5.1.0/obiba_opal/io.py
--rw-r--r--   0        0        0    34794 2023-03-10 10:48:57.337322 obiba_opal-5.1.0/obiba_opal/perm.py
--rwxr-xr-x   0        0        0    11397 2023-03-10 10:48:57.337322 obiba_opal-5.1.0/obiba_opal/project.py
--rw-r--r--   0        0        0     1325 2023-03-10 10:48:57.337322 obiba_opal-5.1.0/obiba_opal/security.py
--rw-r--r--   0        0        0     4871 2023-03-10 10:48:57.337322 obiba_opal-5.1.0/obiba_opal/sql.py
--rwxr-xr-x   0        0        0    10891 2023-03-10 10:48:57.337322 obiba_opal-5.1.0/obiba_opal/subjects.py
--rw-r--r--   0        0        0    15854 2023-03-10 10:48:57.337322 obiba_opal-5.1.0/obiba_opal/system.py
--rw-r--r--   0        0        0    14338 2023-03-10 10:48:57.337322 obiba_opal-5.1.0/obiba_opal/table.py
--rw-r--r--   0        0        0      747 2023-03-10 10:48:57.337322 obiba_opal-5.1.0/pyproject.toml
--rw-r--r--   0        0        0     4529 1970-01-01 00:00:00.000000 obiba_opal-5.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35147 2023-04-28 13:13:51.895934 obiba_opal-5.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     3571 2023-04-28 13:13:51.895934 obiba_opal-5.1.1/README.md
+-rw-r--r--   0        0        0     1536 2023-04-28 13:13:51.895934 obiba_opal-5.1.1/obiba_opal/__init__.py
+-rw-r--r--   0        0        0     6537 2023-04-28 13:13:51.895934 obiba_opal-5.1.1/obiba_opal/analysis.py
+-rwxr-xr-x   0        0        0    13633 2023-04-28 13:13:51.895934 obiba_opal-5.1.1/obiba_opal/console.py
+-rwxr-xr-x   0        0        0    19710 2023-04-28 13:13:51.895934 obiba_opal-5.1.1/obiba_opal/core.py
+-rwxr-xr-x   0        0        0     7183 2023-04-28 13:13:51.895934 obiba_opal-5.1.1/obiba_opal/data.py
+-rwxr-xr-x   0        0        0    14684 2023-04-28 13:13:51.895934 obiba_opal-5.1.1/obiba_opal/dictionary.py
+-rw-r--r--   0        0        0    24652 2023-04-28 13:13:51.895934 obiba_opal-5.1.1/obiba_opal/exports.py
+-rwxr-xr-x   0        0        0     4776 2023-04-28 13:13:51.899936 obiba_opal-5.1.1/obiba_opal/file.py
+-rw-r--r--   0        0        0    47546 2023-04-28 13:13:51.899936 obiba_opal-5.1.1/obiba_opal/imports.py
+-rw-r--r--   0        0        0    12875 2023-04-28 13:13:51.899936 obiba_opal-5.1.1/obiba_opal/io.py
+-rw-r--r--   0        0        0    34898 2023-04-28 13:13:51.899936 obiba_opal-5.1.1/obiba_opal/perm.py
+-rwxr-xr-x   0        0        0    11397 2023-04-28 13:13:51.899936 obiba_opal-5.1.1/obiba_opal/project.py
+-rw-r--r--   0        0        0     1325 2023-04-28 13:13:51.899936 obiba_opal-5.1.1/obiba_opal/security.py
+-rw-r--r--   0        0        0     4871 2023-04-28 13:13:51.899936 obiba_opal-5.1.1/obiba_opal/sql.py
+-rwxr-xr-x   0        0        0    10891 2023-04-28 13:13:51.899936 obiba_opal-5.1.1/obiba_opal/subjects.py
+-rw-r--r--   0        0        0    15854 2023-04-28 13:13:51.899936 obiba_opal-5.1.1/obiba_opal/system.py
+-rw-r--r--   0        0        0    14338 2023-04-28 13:13:51.899936 obiba_opal-5.1.1/obiba_opal/table.py
+-rw-r--r--   0        0        0      804 2023-04-28 13:13:51.899936 obiba_opal-5.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4529 1970-01-01 00:00:00.000000 obiba_opal-5.1.1/PKG-INFO
```

### Comparing `obiba_opal-5.1.0/LICENSE.txt` & `obiba_opal-5.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.0/README.md` & `obiba_opal-5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.0/obiba_opal/__init__.py` & `obiba_opal-5.1.1/obiba_opal/__init__.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.0/obiba_opal/analysis.py` & `obiba_opal-5.1.1/obiba_opal/analysis.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.0/obiba_opal/console.py` & `obiba_opal-5.1.1/obiba_opal/console.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.0/obiba_opal/core.py` & `obiba_opal-5.1.1/obiba_opal/core.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.0/obiba_opal/data.py` & `obiba_opal-5.1.1/obiba_opal/data.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.0/obiba_opal/dictionary.py` & `obiba_opal-5.1.1/obiba_opal/dictionary.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.0/obiba_opal/exports.py` & `obiba_opal-5.1.1/obiba_opal/exports.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.0/obiba_opal/file.py` & `obiba_opal-5.1.1/obiba_opal/file.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.0/obiba_opal/imports.py` & `obiba_opal-5.1.1/obiba_opal/imports.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.0/obiba_opal/io.py` & `obiba_opal-5.1.1/obiba_opal/io.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.0/obiba_opal/perm.py` & `obiba_opal-5.1.1/obiba_opal/perm.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         parser.add_argument('--add', '-a', action='store_true', required=False, help='Add a permission')
         parser.add_argument('--delete', '-d', action='store_true', required=False, help='Delete a permission')
         parser.add_argument('--permission', '-pe', help="Permission to apply: %s" % ', '.join(permissions))
         parser.add_argument('--subject', '-s', required=False, help='Subject name to which the permission will be granted/removed (required on add/delete)')
         parser.add_argument('--type', '-ty', required=True, help='Subject type: user or group')
         parser.add_argument('--json', '-j', action='store_true', help='Pretty JSON formatting of the response')
 
+    @classmethod
     def _map_permission(self, permission: str, permissions: dict):
         """
         Map permission argument to permission query parameter
         """
         if permission.lower() not in list(permissions.keys()):
             return None
 
@@ -331,27 +332,27 @@
         :param subject: The subject name
         :param type: The subject type ('user' or 'group')
         """
         request = self._make_request()
         request.delete().resource(
                 self._make_delete_ws(['project', project, 'permissions', 'table', table], subject, type)).send()
 
-    def add_perms(self, project: str, tables: list, subject: str, type: str):
+    def add_perms(self, project: str, tables: list, subject: str, type: str, permission: str):
         """
         Add project's tables level permissions.
 
         :param project: The project name
         :param tables: The table names (all if empty)
         :param subject: The subject name
         :param type: The subject type ('user' or 'group')
         :param permission: The permission
         """
         tables_ = self._ensure_tables(project, tables)
         for table in tables_:
-            self.add_perm(project, table, subject, type)
+            self.add_perm(project, table, subject, type, permission)
 
     def add_perm(self, project: str, table: str, subject: str, type: str, permission: str):
         """
         Add project's table level permissions.
 
         :param project: The project name
         :param table: The table name
@@ -461,28 +462,28 @@
         :param subject: The subject name
         :param type: The subject type ('user' or 'group')
         """
         request = self._make_request()
         request.delete().resource(
                 self._make_delete_ws(['project', project, 'permissions', 'table', table, 'variable', variable], subject, type)).send()
 
-    def add_perms(self, project: str, table: str, variables: list, subject: str, type: str):
+    def add_perms(self, project: str, table: str, variables: list, subject: str, type: str, permission: str):
         """
         Add project's table variables level permissions.
 
         :param project: The project name
         :param table: The table name
         :param variables: The variable names (all if empty)
         :param subject: The subject name
         :param type: The subject type ('user' or 'group')
         :param permission: The permission
         """
         variables_ = self._ensure_variables(project, table, variables)
         for variable in variables_:
-            self.add_perm(project, table, variable, subject, type)
+            self.add_perm(project, table, variable, subject, type, permission)
 
     def add_perm(self, project: str, table: str, variable: str, subject: str, type: str, permission: str):
         """
         Add project's table variable level permissions.
 
         :param project: The project name
         :param table: The table name
@@ -589,27 +590,27 @@
         :param subject: The subject name
         :param type: The subject type ('user' or 'group')
         """
         request = self._make_request()
         request.delete().resource(
                 self._make_delete_ws(['project', project, 'permissions', 'resource', resource], subject, type)).send()
 
-    def add_perms(self, project: str, resources: list, subject: str, type: str):
+    def add_perms(self, project: str, resources: list, subject: str, type: str, permission: str):
         """
         Add project's resources level permissions.
 
         :param project: The project name
         :param resources: The resource names (all if empty)
         :param subject: The subject name
         :param type: The subject type ('user' or 'group')
         :param permission: The permission
         """
         resources_ = self._ensure_resources(project, resources)
         for resource in resources_:
-            self.add_perm(project, resource, subject, type)
+            self.add_perm(project, resource, subject, type, permission)
 
     def add_perm(self, project: str, resource: str, subject: str, type: str, permission: str):
         """
         Add project's resource level permissions.
 
         :param project: The project name
         :param resource: The resource name
```

### Comparing `obiba_opal-5.1.0/obiba_opal/project.py` & `obiba_opal-5.1.1/obiba_opal/project.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.0/obiba_opal/security.py` & `obiba_opal-5.1.1/obiba_opal/security.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.0/obiba_opal/sql.py` & `obiba_opal-5.1.1/obiba_opal/sql.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.0/obiba_opal/subjects.py` & `obiba_opal-5.1.1/obiba_opal/subjects.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.0/obiba_opal/system.py` & `obiba_opal-5.1.1/obiba_opal/system.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.0/obiba_opal/table.py` & `obiba_opal-5.1.1/obiba_opal/table.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.0/pyproject.toml` & `obiba_opal-5.1.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "obiba-opal"
-version = "5.1.0"
+version = "5.1.1"
 description = "OBiBa/Opal python client."
 authors = ["Yannick Marcon <yannick.marcon@obiba.org>"]
 maintainers = ["Yannick Marcon <yannick.marcon@obiba.org>"]
 license = "GPL-v3"
 readme = "README.md"
 packages = [{include = "obiba_opal"}]
 homepage = "https://www.obiba.org"
@@ -14,13 +14,16 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/obiba/opal-python-client/issues"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pycurl = "^7.45.2"
 
+[tool.poetry.group.test.dependencies]
+pytest = "^7.2.2"
+
 [tool.poetry.scripts]
 opal = 'obiba_opal.console:run'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `obiba_opal-5.1.0/PKG-INFO` & `obiba_opal-5.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obiba-opal
-Version: 5.1.0
+Version: 5.1.1
 Summary: OBiBa/Opal python client.
 Home-page: https://www.obiba.org
 License: GPL-v3
 Author: Yannick Marcon
 Author-email: yannick.marcon@obiba.org
 Maintainer: Yannick Marcon
 Maintainer-email: yannick.marcon@obiba.org
```

