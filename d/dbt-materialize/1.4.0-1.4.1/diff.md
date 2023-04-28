# Comparing `tmp/dbt-materialize-1.4.0.tar.gz` & `tmp/dbt-materialize-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-materialize-1.4.0.tar", last modified: Fri Feb  3 16:13:09 2023, max compression
+gzip compressed data, was "dbt-materialize-1.4.1.tar", last modified: Fri Apr 28 18:04:05 2023, max compression
```

## Comparing `dbt-materialize-1.4.0.tar` & `dbt-materialize-1.4.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-02-03 16:13:09.535012 dbt-materialize-1.4.0/
--rw-r--r--   0 materialize  (2000) materialize  (1001)     5950 2023-02-03 16:13:09.535012 dbt-materialize-1.4.0/PKG-INFO
--rw-r--r--   0 materialize  (2000) materialize  (1001)     5592 2023-02-03 16:12:37.000000 dbt-materialize-1.4.0/README.md
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-02-03 16:13:09.531012 dbt-materialize-1.4.0/dbt/
--rw-r--r--   0 materialize  (2000) materialize  (1001)      729 2023-02-03 16:12:37.000000 dbt-materialize-1.4.0/dbt/__init__.py
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-02-03 16:13:09.531012 dbt-materialize-1.4.0/dbt/adapters/
--rw-r--r--   0 materialize  (2000) materialize  (1001)      729 2023-02-03 16:12:37.000000 dbt-materialize-1.4.0/dbt/adapters/__init__.py
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-02-03 16:13:09.531012 dbt-materialize-1.4.0/dbt/adapters/materialize/
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1159 2023-02-03 16:12:37.000000 dbt-materialize-1.4.0/dbt/adapters/materialize/__init__.py
--rw-r--r--   0 materialize  (2000) materialize  (1001)      801 2023-02-03 16:12:37.000000 dbt-materialize-1.4.0/dbt/adapters/materialize/__version__.py
--rw-r--r--   0 materialize  (2000) materialize  (1001)     3616 2023-02-03 16:12:37.000000 dbt-materialize-1.4.0/dbt/adapters/materialize/connections.py
--rw-r--r--   0 materialize  (2000) materialize  (1001)     4106 2023-02-03 16:12:37.000000 dbt-materialize-1.4.0/dbt/adapters/materialize/impl.py
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1688 2023-02-03 16:12:37.000000 dbt-materialize-1.4.0/dbt/adapters/materialize/relation.py
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-02-03 16:13:09.531012 dbt-materialize-1.4.0/dbt/include/
--rw-r--r--   0 materialize  (2000) materialize  (1001)      729 2023-02-03 16:12:37.000000 dbt-materialize-1.4.0/dbt/include/__init__.py
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-02-03 16:13:09.531012 dbt-materialize-1.4.0/dbt/include/materialize/
--rw-r--r--   0 materialize  (2000) materialize  (1001)      782 2023-02-03 16:12:37.000000 dbt-materialize-1.4.0/dbt/include/materialize/__init__.py
--rw-r--r--   0 materialize  (2000) materialize  (1001)      808 2023-02-03 16:12:37.000000 dbt-materialize-1.4.0/dbt/include/materialize/dbt_project.yml
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-02-03 16:13:09.531012 dbt-materialize-1.4.0/dbt/include/materialize/macros/
--rw-r--r--   0 materialize  (2000) materialize  (1001)     3862 2023-02-03 16:12:37.000000 dbt-materialize-1.4.0/dbt/include/materialize/macros/adapters.sql
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1848 2023-02-03 16:12:37.000000 dbt-materialize-1.4.0/dbt/include/materialize/macros/catalog.sql
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-02-03 16:13:09.535012 dbt-materialize-1.4.0/dbt/include/materialize/macros/materializations/
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1909 2023-02-03 16:12:37.000000 dbt-materialize-1.4.0/dbt/include/materialize/macros/materializations/incremental.sql
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1920 2023-02-03 16:12:37.000000 dbt-materialize-1.4.0/dbt/include/materialize/macros/materializations/materialized_view.sql
--rw-r--r--   0 materialize  (2000) materialize  (1001)     3023 2023-02-03 16:12:37.000000 dbt-materialize-1.4.0/dbt/include/materialize/macros/materializations/seed.sql
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1784 2023-02-03 16:12:37.000000 dbt-materialize-1.4.0/dbt/include/materialize/macros/materializations/sink.sql
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1828 2023-02-03 16:12:37.000000 dbt-materialize-1.4.0/dbt/include/materialize/macros/materializations/source.sql
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1933 2023-02-03 16:12:37.000000 dbt-materialize-1.4.0/dbt/include/materialize/macros/materializations/table.sql
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1960 2023-02-03 16:12:37.000000 dbt-materialize-1.4.0/dbt/include/materialize/macros/materializations/test.sql
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1883 2023-02-03 16:12:37.000000 dbt-materialize-1.4.0/dbt/include/materialize/macros/materializations/view.sql
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-02-03 16:13:09.535012 dbt-materialize-1.4.0/dbt/include/materialize/macros/utils/
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1016 2023-02-03 16:12:37.000000 dbt-materialize-1.4.0/dbt/include/materialize/macros/utils/listagg.sql
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-02-03 16:13:09.535012 dbt-materialize-1.4.0/dbt_materialize.egg-info/
--rw-r--r--   0 materialize  (2000) materialize  (1001)     5950 2023-02-03 16:13:09.000000 dbt-materialize-1.4.0/dbt_materialize.egg-info/PKG-INFO
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1155 2023-02-03 16:13:09.000000 dbt-materialize-1.4.0/dbt_materialize.egg-info/SOURCES.txt
--rw-r--r--   0 materialize  (2000) materialize  (1001)        1 2023-02-03 16:13:09.000000 dbt-materialize-1.4.0/dbt_materialize.egg-info/dependency_links.txt
--rw-r--r--   0 materialize  (2000) materialize  (1001)       52 2023-02-03 16:13:09.000000 dbt-materialize-1.4.0/dbt_materialize.egg-info/requires.txt
--rw-r--r--   0 materialize  (2000) materialize  (1001)        4 2023-02-03 16:13:09.000000 dbt-materialize-1.4.0/dbt_materialize.egg-info/top_level.txt
--rw-r--r--   0 materialize  (2000) materialize  (1001)       38 2023-02-03 16:13:09.535012 dbt-materialize-1.4.0/setup.cfg
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1768 2023-02-03 16:12:37.000000 dbt-materialize-1.4.0/setup.py
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-04-28 18:04:05.043542 dbt-materialize-1.4.1/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     5950 2023-04-28 18:04:05.043542 dbt-materialize-1.4.1/PKG-INFO
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     5592 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/README.md
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-04-28 18:04:05.033542 dbt-materialize-1.4.1/dbt/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)      729 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/__init__.py
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-04-28 18:04:05.033542 dbt-materialize-1.4.1/dbt/adapters/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)      729 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/adapters/__init__.py
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-04-28 18:04:05.033542 dbt-materialize-1.4.1/dbt/adapters/materialize/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1159 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/adapters/materialize/__init__.py
+-rw-r--r--   0 materialize  (2000) materialize  (1001)      801 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/adapters/materialize/__version__.py
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     3431 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/adapters/materialize/connections.py
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     4104 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/adapters/materialize/impl.py
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1688 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/adapters/materialize/relation.py
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-04-28 18:04:05.033542 dbt-materialize-1.4.1/dbt/include/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)      729 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/__init__.py
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-04-28 18:04:05.033542 dbt-materialize-1.4.1/dbt/include/materialize/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)      782 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/__init__.py
+-rw-r--r--   0 materialize  (2000) materialize  (1001)      808 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/dbt_project.yml
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-04-28 18:04:05.043542 dbt-materialize-1.4.1/dbt/include/materialize/macros/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     3862 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/macros/adapters.sql
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1848 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/macros/catalog.sql
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-04-28 18:04:05.043542 dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1909 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/incremental.sql
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1920 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/materialized_view.sql
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     3023 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/seed.sql
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1784 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/sink.sql
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1828 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/source.sql
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1933 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/table.sql
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1960 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/test.sql
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1883 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/view.sql
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-04-28 18:04:05.043542 dbt-materialize-1.4.1/dbt/include/materialize/macros/utils/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1016 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/macros/utils/listagg.sql
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-04-28 18:04:05.043542 dbt-materialize-1.4.1/dbt_materialize.egg-info/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     5950 2023-04-28 18:04:04.000000 dbt-materialize-1.4.1/dbt_materialize.egg-info/PKG-INFO
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1155 2023-04-28 18:04:04.000000 dbt-materialize-1.4.1/dbt_materialize.egg-info/SOURCES.txt
+-rw-r--r--   0 materialize  (2000) materialize  (1001)        1 2023-04-28 18:04:04.000000 dbt-materialize-1.4.1/dbt_materialize.egg-info/dependency_links.txt
+-rw-r--r--   0 materialize  (2000) materialize  (1001)       52 2023-04-28 18:04:04.000000 dbt-materialize-1.4.1/dbt_materialize.egg-info/requires.txt
+-rw-r--r--   0 materialize  (2000) materialize  (1001)        4 2023-04-28 18:04:04.000000 dbt-materialize-1.4.1/dbt_materialize.egg-info/top_level.txt
+-rw-r--r--   0 materialize  (2000) materialize  (1001)       38 2023-04-28 18:04:05.043542 dbt-materialize-1.4.1/setup.cfg
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1768 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/setup.py
```

### Comparing `dbt-materialize-1.4.0/PKG-INFO` & `dbt-materialize-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-materialize
-Version: 1.4.0
+Version: 1.4.1
 Summary: The Materialize adapter plugin for dbt.
 Home-page: https://github.com/MaterializeInc/materialize/blob/main/misc/dbt-materialize
 Author: Materialize, Inc.
 Author-email: support@materialize.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -26,15 +26,15 @@
 source dbt-venv/bin/activate     # activate the virtual environment
 pip install dbt-materialize      # install the adapter
 ```
 
 ## Requirements
 
 <!-- If you update this, bump the constraint in connections.py too. -->
-`dbt-materialize` requires Materialize v0.28.0+.
+`dbt-materialize` requires Materialize v0.49.0+.
 
 ## Configuring your profile
 
 To connect to a Materialize instance, use the reference [profile configuration](https://docs.getdbt.com/reference/warehouse-profiles/materialize-profile#connecting-to-materialize-with-dbt-materialize) in your
 connection profile:
 
 ```yml
```

### Comparing `dbt-materialize-1.4.0/README.md` & `dbt-materialize-1.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 source dbt-venv/bin/activate     # activate the virtual environment
 pip install dbt-materialize      # install the adapter
 ```
 
 ## Requirements
 
 <!-- If you update this, bump the constraint in connections.py too. -->
-`dbt-materialize` requires Materialize v0.28.0+.
+`dbt-materialize` requires Materialize v0.49.0+.
 
 ## Configuring your profile
 
 To connect to a Materialize instance, use the reference [profile configuration](https://docs.getdbt.com/reference/warehouse-profiles/materialize-profile#connecting-to-materialize-with-dbt-materialize) in your
 connection profile:
 
 ```yml
```

### Comparing `dbt-materialize-1.4.0/dbt/__init__.py` & `dbt-materialize-1.4.1/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.0/dbt/adapters/__init__.py` & `dbt-materialize-1.4.1/dbt/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.0/dbt/adapters/materialize/__init__.py` & `dbt-materialize-1.4.1/dbt/adapters/materialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.0/dbt/adapters/materialize/__version__.py` & `dbt-materialize-1.4.1/dbt/adapters/materialize/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # If you bump this version, bump it in setup.py too.
-version = "1.4.0"
+version = "1.4.1"
```

### Comparing `dbt-materialize-1.4.0/dbt/adapters/materialize/connections.py` & `dbt-materialize-1.4.1/dbt/adapters/materialize/connections.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 import dbt.exceptions
 from dbt.adapters.postgres import PostgresConnectionManager, PostgresCredentials
 from dbt.events import AdapterLogger
 from dbt.semver import versions_compatible
 
 # If you bump this version, bump it in README.md too.
-SUPPORTED_MATERIALIZE_VERSIONS = ">=0.28.0"
+SUPPORTED_MATERIALIZE_VERSIONS = ">=0.49.0"
 
 logger = AdapterLogger("Materialize")
 
 
 @dataclass
 class MaterializeCredentials(PostgresCredentials):
     cluster: Optional[str] = "default"
@@ -60,30 +60,30 @@
 
         # Prevents psycopg connection from automatically opening transactions.
         # More info: https://www.psycopg.org/docs/usage.html#transactions-control
         connection.handle.autocommit = True
 
         cursor = connection.handle.cursor()
 
-        # Upon connection, dbt performs introspection queries that should run in
-        # the mz_introspection cluster for optimal performance. Each materialization
-        # should then handle falling back to the default connection cluster if no
-        # cluster configuration is specified at the model level.
-        mz_introspection_cluster = "mz_introspection"
-        logger.debug("Switching to cluster '{}'".format(mz_introspection_cluster))
-        cursor.execute("SET cluster = %s" % mz_introspection_cluster)
-
-        cursor.execute("SELECT mz_version()")
+        # Check for the current DB version using the "mz_introspection" cluster in case "default"
+        # doesn't exist.
+        cursor.execute("SHOW mz_version")
         mz_version = cursor.fetchone()[0].split()[0].strip("v")
+
         if not versions_compatible(mz_version, SUPPORTED_MATERIALIZE_VERSIONS):
             raise dbt.exceptions.DbtRuntimeError(
                 f"Detected unsupported Materialize version {mz_version}\n"
                 f"  Supported versions: {SUPPORTED_MATERIALIZE_VERSIONS}"
             )
 
+        # Make sure 'auto_route_introspection_queries' is enabled.
+        var_name = "auto_route_introspection_queries"
+        logger.debug(f"Enabling {var_name}")
+        cursor.execute(f"SET {var_name} = true")
+
         return connection
 
     # Disable transactions. Materialize transactions do not support arbitrary
     # queries in transactions and therefore many of dbt's internal macros
     # produce invalid transactions.
     #
     # Disabling transactions has precedent in dbt-snowflake and dbt-biquery.
```

### Comparing `dbt-materialize-1.4.0/dbt/adapters/materialize/impl.py` & `dbt-materialize-1.4.1/dbt/adapters/materialize/impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,17 +41,17 @@
             cls.validate(raw_index)
             return cls.from_dict(raw_index)
         except ValidationError as exc:
             msg = dbt.exceptions.validator_error_message(exc)
             dbt.exceptions.CompilationError(f"Could not parse index config: {msg}")
         except TypeError:
             dbt.exceptions.CompilationError(
-                f"Invalid index config:\n"
+                "Invalid index config:\n"
                 f"  Got: {raw_index}\n"
-                f'  Expected a dictionary with at minimum a "columns" key'
+                '  Expected a dictionary with at minimum a "columns" key'
             )
 
 
 @dataclass
 class MaterializeConfig(AdapterConfig):
     cluster: Optional[str] = None
```

### Comparing `dbt-materialize-1.4.0/dbt/adapters/materialize/relation.py` & `dbt-materialize-1.4.1/dbt/adapters/materialize/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.0/dbt/include/__init__.py` & `dbt-materialize-1.4.1/dbt/include/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.0/dbt/include/materialize/__init__.py` & `dbt-materialize-1.4.1/dbt/include/materialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.0/dbt/include/materialize/dbt_project.yml` & `dbt-materialize-1.4.1/dbt/include/materialize/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.0/dbt/include/materialize/macros/adapters.sql` & `dbt-materialize-1.4.1/dbt/include/materialize/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.0/dbt/include/materialize/macros/catalog.sql` & `dbt-materialize-1.4.1/dbt/include/materialize/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.0/dbt/include/materialize/macros/materializations/incremental.sql` & `dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.0/dbt/include/materialize/macros/materializations/materialized_view.sql` & `dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.0/dbt/include/materialize/macros/materializations/seed.sql` & `dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.0/dbt/include/materialize/macros/materializations/sink.sql` & `dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/sink.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.0/dbt/include/materialize/macros/materializations/source.sql` & `dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/source.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.0/dbt/include/materialize/macros/materializations/table.sql` & `dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.0/dbt/include/materialize/macros/materializations/test.sql` & `dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.0/dbt/include/materialize/macros/materializations/view.sql` & `dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.0/dbt/include/materialize/macros/utils/listagg.sql` & `dbt-materialize-1.4.1/dbt/include/materialize/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.0/dbt_materialize.egg-info/PKG-INFO` & `dbt-materialize-1.4.1/dbt_materialize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-materialize
-Version: 1.4.0
+Version: 1.4.1
 Summary: The Materialize adapter plugin for dbt.
 Home-page: https://github.com/MaterializeInc/materialize/blob/main/misc/dbt-materialize
 Author: Materialize, Inc.
 Author-email: support@materialize.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -26,15 +26,15 @@
 source dbt-venv/bin/activate     # activate the virtual environment
 pip install dbt-materialize      # install the adapter
 ```
 
 ## Requirements
 
 <!-- If you update this, bump the constraint in connections.py too. -->
-`dbt-materialize` requires Materialize v0.28.0+.
+`dbt-materialize` requires Materialize v0.49.0+.
 
 ## Configuring your profile
 
 To connect to a Materialize instance, use the reference [profile configuration](https://docs.getdbt.com/reference/warehouse-profiles/materialize-profile#connecting-to-materialize-with-dbt-materialize) in your
 connection profile:
 
 ```yml
```

### Comparing `dbt-materialize-1.4.0/dbt_materialize.egg-info/SOURCES.txt` & `dbt-materialize-1.4.1/dbt_materialize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.0/setup.py` & `dbt-materialize-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from setuptools import find_packages
 
 setup(
     name="dbt-materialize",
     # This adapter's minor version should match the required dbt-postgres version,
     # but patch versions may differ.
     # If you bump this version, bump it in __version__.py too.
-    version="1.4.0",
+    version="1.4.1",
     description="The Materialize adapter plugin for dbt.",
     long_description=(Path(__file__).parent / "README.md").open().read(),
     long_description_content_type="text/markdown",
     author="Materialize, Inc.",
     author_email="support@materialize.com",
     url="https://github.com/MaterializeInc/materialize/blob/main/misc/dbt-materialize",
     packages=find_packages(),
```

