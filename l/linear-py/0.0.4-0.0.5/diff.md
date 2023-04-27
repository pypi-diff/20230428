# Comparing `tmp/linear-py-0.0.4.tar.gz` & `tmp/linear-py-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linear-py-0.0.4.tar", last modified: Tue Apr 18 03:50:53 2023, max compression
+gzip compressed data, was "linear-py-0.0.5.tar", last modified: Thu Apr 27 22:28:16 2023, max compression
```

## Comparing `linear-py-0.0.4.tar` & `linear-py-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 valeness  (1000) valeness  (1000)        0 2023-04-18 03:50:53.511351 linear-py-0.0.4/
--rw-rw-r--   0 valeness  (1000) valeness  (1000)    34901 2023-04-07 18:41:07.000000 linear-py-0.0.4/LICENSE
--rw-rw-r--   0 valeness  (1000) valeness  (1000)      594 2023-04-18 03:50:53.511351 linear-py-0.0.4/PKG-INFO
--rw-rw-r--   0 valeness  (1000) valeness  (1000)      112 2023-04-07 18:41:07.000000 linear-py-0.0.4/README.md
--rw-rw-r--   0 valeness  (1000) valeness  (1000)      104 2023-04-07 18:41:07.000000 linear-py-0.0.4/pyproject.toml
--rw-rw-r--   0 valeness  (1000) valeness  (1000)      738 2023-04-18 03:50:53.511351 linear-py-0.0.4/setup.cfg
-drwxrwxr-x   0 valeness  (1000) valeness  (1000)        0 2023-04-18 03:50:53.507351 linear-py-0.0.4/src/
-drwxrwxr-x   0 valeness  (1000) valeness  (1000)        0 2023-04-18 03:50:53.511351 linear-py-0.0.4/src/linear/
--rw-rw-r--   0 valeness  (1000) valeness  (1000)       47 2023-04-07 18:41:07.000000 linear-py-0.0.4/src/linear/Exceptions.py
--rw-rw-r--   0 valeness  (1000) valeness  (1000)     2104 2023-04-18 03:30:27.000000 linear-py-0.0.4/src/linear/Linear.py
--rw-rw-r--   0 valeness  (1000) valeness  (1000)       26 2023-04-07 18:41:07.000000 linear-py-0.0.4/src/linear/__init__.py
-drwxrwxr-x   0 valeness  (1000) valeness  (1000)        0 2023-04-18 03:50:53.511351 linear-py-0.0.4/src/linear_py.egg-info/
--rw-rw-r--   0 valeness  (1000) valeness  (1000)      594 2023-04-18 03:50:53.000000 linear-py-0.0.4/src/linear_py.egg-info/PKG-INFO
--rw-rw-r--   0 valeness  (1000) valeness  (1000)      295 2023-04-18 03:50:53.000000 linear-py-0.0.4/src/linear_py.egg-info/SOURCES.txt
--rw-rw-r--   0 valeness  (1000) valeness  (1000)        1 2023-04-18 03:50:53.000000 linear-py-0.0.4/src/linear_py.egg-info/dependency_links.txt
--rw-rw-r--   0 valeness  (1000) valeness  (1000)       17 2023-04-18 03:50:53.000000 linear-py-0.0.4/src/linear_py.egg-info/requires.txt
--rw-rw-r--   0 valeness  (1000) valeness  (1000)        7 2023-04-18 03:50:53.000000 linear-py-0.0.4/src/linear_py.egg-info/top_level.txt
+drwxrwxr-x   0 valeness  (1000) valeness  (1000)        0 2023-04-27 22:28:16.601155 linear-py-0.0.5/
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)    34901 2023-04-07 18:41:07.000000 linear-py-0.0.5/LICENSE
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)      594 2023-04-27 22:28:16.601155 linear-py-0.0.5/PKG-INFO
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)      112 2023-04-07 18:41:07.000000 linear-py-0.0.5/README.md
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)      104 2023-04-07 18:41:07.000000 linear-py-0.0.5/pyproject.toml
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)      738 2023-04-27 22:28:16.601155 linear-py-0.0.5/setup.cfg
+drwxrwxr-x   0 valeness  (1000) valeness  (1000)        0 2023-04-27 22:28:16.601155 linear-py-0.0.5/src/
+drwxrwxr-x   0 valeness  (1000) valeness  (1000)        0 2023-04-27 22:28:16.601155 linear-py-0.0.5/src/linear/
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)       47 2023-04-07 18:41:07.000000 linear-py-0.0.5/src/linear/Exceptions.py
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)     2111 2023-04-27 22:27:17.000000 linear-py-0.0.5/src/linear/Linear.py
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)       26 2023-04-07 18:41:07.000000 linear-py-0.0.5/src/linear/__init__.py
+drwxrwxr-x   0 valeness  (1000) valeness  (1000)        0 2023-04-27 22:28:16.601155 linear-py-0.0.5/src/linear_py.egg-info/
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)      594 2023-04-27 22:28:16.000000 linear-py-0.0.5/src/linear_py.egg-info/PKG-INFO
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)      295 2023-04-27 22:28:16.000000 linear-py-0.0.5/src/linear_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)        1 2023-04-27 22:28:16.000000 linear-py-0.0.5/src/linear_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)       17 2023-04-27 22:28:16.000000 linear-py-0.0.5/src/linear_py.egg-info/requires.txt
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)        7 2023-04-27 22:28:16.000000 linear-py-0.0.5/src/linear_py.egg-info/top_level.txt
```

### Comparing `linear-py-0.0.4/LICENSE` & `linear-py-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `linear-py-0.0.4/PKG-INFO` & `linear-py-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linear-py
-Version: 0.0.4
+Version: 0.0.5
 Summary: Integrate with the linear graphQL in a pythonic way
 Home-page: https://gitlab.com/thinkhuman-public/linear-py
 Author: valeness
 Author-email: james@thinkhuman.co
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `linear-py-0.0.4/setup.cfg` & `linear-py-0.0.5/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = linear-py
-version = 0.0.4
+version = 0.0.5
 author = valeness
 author_email = james@thinkhuman.co
 description = Integrate with the linear graphQL in a pythonic way
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/thinkhuman-public/linear-py
 classifiers =
```

### Comparing `linear-py-0.0.4/src/linear/Linear.py` & `linear-py-0.0.5/src/linear/Linear.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,35 +36,35 @@
                 query Resource {"""+resource+"""{nodes{id,name}}}
             """
         )
 
         return resource_response["data"][resource]["nodes"]
 
     def create_issue(self, title, description='', project_id='', state_id='', team_id=''):
-        create_response = self.query_grapql(
-            """
+        q = """
             mutation IssueCreate {{
               issueCreate(
                 input: {{
                     title: "{title}"
-                    description: "{description}"
+                    description: {description}
                     projectId: "{project_id}"
                     stateId: "{state_id}"
                     teamId: "{team_id}"
                 }}
               ) {{
                 success
                 issue {{
                   id
                   title
                 }}
               }}
             }}
             """.format(title=title, description=description, project_id=project_id, team_id=team_id, state_id=state_id)
-        )
+        print(q)
+        create_response = self.query_grapql(q)
         return create_response['data']['issueCreate']
 
     def teams(self):
         return self.query_basic_resource('teams')
 
     def states(self):
         return self.query_basic_resource('workflowStates')
```

### Comparing `linear-py-0.0.4/src/linear_py.egg-info/PKG-INFO` & `linear-py-0.0.5/src/linear_py.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linear-py
-Version: 0.0.4
+Version: 0.0.5
 Summary: Integrate with the linear graphQL in a pythonic way
 Home-page: https://gitlab.com/thinkhuman-public/linear-py
 Author: valeness
 Author-email: james@thinkhuman.co
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

