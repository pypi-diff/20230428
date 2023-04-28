# Comparing `tmp/datajunction-0.0.1a6.tar.gz` & `tmp/datajunction-0.0.1a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datajunction-0.0.1a6.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `datajunction-0.0.1a6.tar` & `datajunction-0.0.1a8.tar`

### file list

```diff
@@ -1,7 +1,20 @@
--rw-r--r--   0        0        0     1081 2023-03-26 08:42:43.476435 datajunction-0.0.1a6/LICENSE.txt
--rw-r--r--   0        0        0     2503 2023-04-22 17:55:26.982921 datajunction-0.0.1a6/README.md
--rw-r--r--   0        0        0      780 2023-04-25 14:27:09.403307 datajunction-0.0.1a6/datajunction/__init__.py
--rw-r--r--   0        0        0    20307 2023-04-25 14:27:09.403874 datajunction-0.0.1a6/datajunction/client.py
--rw-r--r--   0        0        0      108 2023-04-22 17:55:26.983612 datajunction-0.0.1a6/datajunction/exceptions.py
--rw-r--r--   0        0        0     1075 2023-04-26 16:55:41.582167 datajunction-0.0.1a6/pyproject.toml
--rw-r--r--   0        0        0     3515 1970-01-01 00:00:00.000000 datajunction-0.0.1a6/PKG-INFO
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 datajunction-0.0.1a8/.coveragerc
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 datajunction-0.0.1a8/.isort.cfg
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 datajunction-0.0.1a8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 datajunction-0.0.1a8/Makefile
+-rw-r--r--   0        0        0   234651 2020-02-02 00:00:00.000000 datajunction-0.0.1a8/pdm.lock
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 datajunction-0.0.1a8/setup.cfg
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 datajunction-0.0.1a8/tox.ini
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 datajunction-0.0.1a8/datajunction/__about__.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 datajunction-0.0.1a8/datajunction/__init__.py
+-rw-r--r--   0        0        0    21031 2020-02-02 00:00:00.000000 datajunction-0.0.1a8/datajunction/client.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 datajunction-0.0.1a8/datajunction/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datajunction-0.0.1a8/tests/__init__.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 datajunction-0.0.1a8/tests/conftest.py
+-rw-r--r--   0        0        0    34671 2020-02-02 00:00:00.000000 datajunction-0.0.1a8/tests/examples.py
+-rw-r--r--   0        0        0    17083 2020-02-02 00:00:00.000000 datajunction-0.0.1a8/tests/test_client.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 datajunction-0.0.1a8/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 datajunction-0.0.1a8/LICENSE.txt
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 datajunction-0.0.1a8/README.md
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 datajunction-0.0.1a8/pyproject.toml
+-rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 datajunction-0.0.1a8/PKG-INFO
```

### Comparing `datajunction-0.0.1a6/LICENSE.txt` & `datajunction-0.0.1a8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a6/README.md` & `datajunction-0.0.1a8/README.md`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a6/datajunction/__init__.py` & `datajunction-0.0.1a8/datajunction/__init__.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a6/datajunction/client.py` & `datajunction-0.0.1a8/datajunction/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,14 +262,25 @@
             metrics=metrics,
             dimensions=dimensions,
             filters=filters,
             description=description,
             display_name=display_name,
         )
 
+    def new_namespace(
+        self,
+        namespace: str,
+    ) -> "Namespace":
+        """
+        Creates a new namespace on the server
+        """
+        _namespace = Namespace(dj_client=self, namespace=namespace)
+        self.create_namespace(_namespace)
+        return _namespace
+
     def verify_node_exists(self, node_name: str, type_: str) -> Dict[str, Any]:
         """
         Retrieves a node and verifies that it exists and has the expected node type.
         """
         node = self.get_node(node_name)
         if "name" not in node:
             raise DJClientException(f"No node with name {node_name} exists!")
@@ -304,14 +315,27 @@
 
     def namespace(self, _namespace):
         """
         Returns the specified node namespace.
         """
         return Namespace(namespace=_namespace, dj_client=self)
 
+    def create_namespace(self, namespace: "Namespace"):
+        """
+        Helper function to create a namespace.
+        """
+        response = self._session.post(
+            f"/namespaces/{namespace.namespace}/",
+            timeout=self._timeout,
+        )
+        json_response = response.json()
+        if response.status_code == 409:
+            raise DJClientException(json_response["message"])
+        return json_response
+
     def delete_node(self, node: "Node"):
         """
         Delete this node
         """
         response = self._session.delete(f"/nodes/{node.name}/", timeout=self._timeout)
         return response
```

### Comparing `datajunction-0.0.1a6/pyproject.toml` & `datajunction-0.0.1a8/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,60 @@
 [build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
-[tool.poetry]
+[tool.pdm.build]
+includes = ["datajunction"]
+
+[project]
 name = "datajunction"
-version = "0.0.1a6"
-readme = "README.md"
-repository = "https://github.com/DataJunction/dj"
+dynamic = ["version"]
 description = "DataJunction client library for connecting to a DataJunction server"
-authors = ["DataJunction Authors"]
-license = "MIT"
-packages = [
-    { include = "datajunction" },
+authors = [
+    {name = "DataJunction Authors", email = "yian.shang@gmail.com"},
 ]
+dependencies = [
+    "pandas>=2.0.1",
+    "pydantic>=1.10.7",
+]
+requires-python = ">=3.8,<4.0"
+readme = "README.md"
+license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+[tool.hatch.version]
+path = "datajunction/__about__.py"
+
+[project.urls]
+repository = "https://github.com/DataJunction/dj"
+
+[tool.pdm.dev-dependencies]
+test = [
+    "pre-commit>=3.2.2",
+    "pylint>=2.17.3",
+    "pytest-asyncio>=0.21.0",
+    "pytest-cov>=4.0.0",
+    "pytest-integration>=0.2.3",
+    "pytest-mock>=3.10.0",
+    "pytest>=7.3.1",
+    "responses>=0.23.1",
+    "fastapi>=0.79.0",
+    "dj @ {root:uri}/../..",
+]
+
+[tool.hatch.metadata]
+allow-direct-references = true
+
 [tool.coverage.run]
 source = ['datajunction/']
 
 [tool.isort]
 src_paths = ["datajunction/", "tests/"]
 profile = 'black'
-
-[tool.poetry.dependencies]
-python = "^3.8"
-pandas = ">=2"
-pydantic = ">=1"
-
-[tool.poetry.group.dev.dependencies]
-coverage = "7.2.2"
-pre-commit = "3.2.0"
-pytest = "7.2.2"
-responses = "0.23.1"
-datajunction-server = "*"
```

### Comparing `datajunction-0.0.1a6/PKG-INFO` & `datajunction-0.0.1a8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 Metadata-Version: 2.1
 Name: datajunction
-Version: 0.0.1a6
+Version: 0.0.1a8
 Summary: DataJunction client library for connecting to a DataJunction server
-Home-page: https://github.com/DataJunction/dj
+Project-URL: repository, https://github.com/DataJunction/dj
+Author-email: DataJunction Authors <yian.shang@gmail.com>
 License: MIT
-Author: DataJunction Authors
-Requires-Python: >=3.8,<4.0
+License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: pandas (>=2)
-Requires-Dist: pydantic (>=1)
-Project-URL: Repository, https://github.com/DataJunction/dj
+Requires-Python: <4.0,>=3.8
+Requires-Dist: pandas>=2.0.1
+Requires-Dist: pydantic>=1.10.7
 Description-Content-Type: text/markdown
 
 # DataJunction Python Client
 
 ## Installation
 To install:
 ```
@@ -164,8 +159,7 @@
       count(repair_order_id) AS num_repair_orders
     FROM repair_orders
     """,
     description="Number of repair orders",
 )
 num_repair_orders.save()
 ```
-
```

