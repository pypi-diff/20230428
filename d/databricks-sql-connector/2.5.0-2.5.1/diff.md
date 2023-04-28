# Comparing `tmp/databricks_sql_connector-2.5.0.tar.gz` & `tmp/databricks_sql_connector-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_sql_connector-2.5.0.tar", max compression
+gzip compressed data, was "databricks_sql_connector-2.5.1.tar", max compression
```

## Comparing `databricks_sql_connector-2.5.0.tar` & `databricks_sql_connector-2.5.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     3935 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/CHANGELOG.md
--rw-r--r--   0        0        0    11346 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/LICENSE
--rw-r--r--   0        0        0     2723 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/README.md
--rw-r--r--   0        0        0     1416 2023-04-15 04:18:18.493806 databricks_sql_connector-2.5.0/pyproject.toml
--rw-r--r--   0        0        0      295 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/src/databricks/__init__.py
--rw-r--r--   0        0        0     1269 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/src/databricks/sql/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/src/databricks/sql/auth/__init__.py
--rw-r--r--   0        0        0     3894 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/src/databricks/sql/auth/auth.py
--rw-r--r--   0        0        0     5493 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/src/databricks/sql/auth/authenticators.py
--rw-r--r--   0        0        0     9717 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/src/databricks/sql/auth/oauth.py
--rw-r--r--   0        0        0     1201 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/src/databricks/sql/auth/oauth_http_handler.py
--rw-r--r--   0        0        0     1269 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/src/databricks/sql/auth/thrift_http_client.py
--rw-r--r--   0        0        0    36862 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/src/databricks/sql/client.py
--rw-r--r--   0        0        0     2423 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/src/databricks/sql/exc.py
--rw-r--r--   0        0        0        0 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/src/databricks/sql/experimental/__init__.py
--rw-r--r--   0        0        0     2236 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/src/databricks/sql/experimental/oauth_persistence.py
--rwxr-xr-x   0        0        0     8062 2023-04-15 04:17:53.233556 databricks_sql_connector-2.5.0/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote
--rw-r--r--   0        0        0   136849 2023-04-15 04:17:53.233556 databricks_sql_connector-2.5.0/src/databricks/sql/thrift_api/TCLIService/TCLIService.py
--rw-r--r--   0        0        0       49 2023-04-15 04:17:53.233556 databricks_sql_connector-2.5.0/src/databricks/sql/thrift_api/TCLIService/__init__.py
--rw-r--r--   0        0        0     1307 2023-04-15 04:17:53.233556 databricks_sql_connector-2.5.0/src/databricks/sql/thrift_api/TCLIService/constants.py
--rw-r--r--   0        0        0  2077276 2023-04-15 04:17:53.237556 databricks_sql_connector-2.5.0/src/databricks/sql/thrift_api/TCLIService/ttypes.py
--rw-r--r--   0        0        0        0 2023-04-15 04:17:53.237556 databricks_sql_connector-2.5.0/src/databricks/sql/thrift_api/__init__.py
--rw-r--r--   0        0        0    41140 2023-04-15 04:17:53.237556 databricks_sql_connector-2.5.0/src/databricks/sql/thrift_backend.py
--rw-r--r--   0        0        0     6771 2023-04-15 04:17:53.237556 databricks_sql_connector-2.5.0/src/databricks/sql/types.py
--rw-r--r--   0        0        0     6646 2023-04-15 04:17:53.237556 databricks_sql_connector-2.5.0/src/databricks/sql/utils.py
--rw-r--r--   0        0        0       60 2023-04-15 04:17:53.237556 databricks_sql_connector-2.5.0/src/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     9813 2023-04-15 04:17:53.237556 databricks_sql_connector-2.5.0/src/databricks/sqlalchemy/dialect/__init__.py
--rw-r--r--   0        0        0      494 2023-04-15 04:17:53.237556 databricks_sql_connector-2.5.0/src/databricks/sqlalchemy/dialect/base.py
--rw-r--r--   0        0        0      792 2023-04-15 04:17:53.237556 databricks_sql_connector-2.5.0/src/databricks/sqlalchemy/dialect/compiler.py
--rw-r--r--   0        0        0     4106 1970-01-01 00:00:00.000000 databricks_sql_connector-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     4033 2023-04-28 21:02:46.456072 databricks_sql_connector-2.5.1/CHANGELOG.md
+-rw-r--r--   0        0        0    11346 2023-04-28 21:02:46.456072 databricks_sql_connector-2.5.1/LICENSE
+-rw-r--r--   0        0        0     2723 2023-04-28 21:02:46.456072 databricks_sql_connector-2.5.1/README.md
+-rw-r--r--   0        0        0     1416 2023-04-28 21:03:11.912715 databricks_sql_connector-2.5.1/pyproject.toml
+-rw-r--r--   0        0        0      295 2023-04-28 21:02:46.460072 databricks_sql_connector-2.5.1/src/databricks/__init__.py
+-rw-r--r--   0        0        0     1269 2023-04-28 21:02:46.460072 databricks_sql_connector-2.5.1/src/databricks/sql/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 21:02:46.460072 databricks_sql_connector-2.5.1/src/databricks/sql/auth/__init__.py
+-rw-r--r--   0        0        0     3894 2023-04-28 21:02:46.460072 databricks_sql_connector-2.5.1/src/databricks/sql/auth/auth.py
+-rw-r--r--   0        0        0     5493 2023-04-28 21:02:46.460072 databricks_sql_connector-2.5.1/src/databricks/sql/auth/authenticators.py
+-rw-r--r--   0        0        0     9717 2023-04-28 21:02:46.460072 databricks_sql_connector-2.5.1/src/databricks/sql/auth/oauth.py
+-rw-r--r--   0        0        0     1201 2023-04-28 21:02:46.460072 databricks_sql_connector-2.5.1/src/databricks/sql/auth/oauth_http_handler.py
+-rw-r--r--   0        0        0     1269 2023-04-28 21:02:46.460072 databricks_sql_connector-2.5.1/src/databricks/sql/auth/thrift_http_client.py
+-rw-r--r--   0        0        0    36862 2023-04-28 21:02:46.460072 databricks_sql_connector-2.5.1/src/databricks/sql/client.py
+-rw-r--r--   0        0        0     2423 2023-04-28 21:02:46.460072 databricks_sql_connector-2.5.1/src/databricks/sql/exc.py
+-rw-r--r--   0        0        0        0 2023-04-28 21:02:46.460072 databricks_sql_connector-2.5.1/src/databricks/sql/experimental/__init__.py
+-rw-r--r--   0        0        0     2236 2023-04-28 21:02:46.460072 databricks_sql_connector-2.5.1/src/databricks/sql/experimental/oauth_persistence.py
+-rwxr-xr-x   0        0        0     8062 2023-04-28 21:02:46.460072 databricks_sql_connector-2.5.1/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote
+-rw-r--r--   0        0        0   136849 2023-04-28 21:02:46.460072 databricks_sql_connector-2.5.1/src/databricks/sql/thrift_api/TCLIService/TCLIService.py
+-rw-r--r--   0        0        0       49 2023-04-28 21:02:46.460072 databricks_sql_connector-2.5.1/src/databricks/sql/thrift_api/TCLIService/__init__.py
+-rw-r--r--   0        0        0     1307 2023-04-28 21:02:46.460072 databricks_sql_connector-2.5.1/src/databricks/sql/thrift_api/TCLIService/constants.py
+-rw-r--r--   0        0        0  2077276 2023-04-28 21:02:46.468073 databricks_sql_connector-2.5.1/src/databricks/sql/thrift_api/TCLIService/ttypes.py
+-rw-r--r--   0        0        0        0 2023-04-28 21:02:46.468073 databricks_sql_connector-2.5.1/src/databricks/sql/thrift_api/__init__.py
+-rw-r--r--   0        0        0    41140 2023-04-28 21:02:46.468073 databricks_sql_connector-2.5.1/src/databricks/sql/thrift_backend.py
+-rw-r--r--   0        0        0     6771 2023-04-28 21:02:46.468073 databricks_sql_connector-2.5.1/src/databricks/sql/types.py
+-rw-r--r--   0        0        0     6646 2023-04-28 21:02:46.468073 databricks_sql_connector-2.5.1/src/databricks/sql/utils.py
+-rw-r--r--   0        0        0       60 2023-04-28 21:02:46.468073 databricks_sql_connector-2.5.1/src/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     9813 2023-04-28 21:02:46.468073 databricks_sql_connector-2.5.1/src/databricks/sqlalchemy/dialect/__init__.py
+-rw-r--r--   0        0        0      494 2023-04-28 21:02:46.468073 databricks_sql_connector-2.5.1/src/databricks/sqlalchemy/dialect/base.py
+-rw-r--r--   0        0        0      792 2023-04-28 21:02:46.468073 databricks_sql_connector-2.5.1/src/databricks/sqlalchemy/dialect/compiler.py
+-rw-r--r--   0        0        0     4106 1970-01-01 00:00:00.000000 databricks_sql_connector-2.5.1/PKG-INFO
```

### Comparing `databricks_sql_connector-2.5.0/CHANGELOG.md` & `databricks_sql_connector-2.5.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Release History
 
 ## 2.5.x (Unreleased)
 
+## 2.5.1 (2023-04-28)
+
+- Other: Relax sqlalchemy required version as it was unecessarily strict.
+
 ## 2.5.0 (2023-04-14)
 - Add support for External Auth providers
 - Fix: Python HTTP proxies were broken
 - Other: All Thrift requests that timeout during connection will be automatically retried
 
 ## 2.4.1 (2023-03-21)
```

### Comparing `databricks_sql_connector-2.5.0/LICENSE` & `databricks_sql_connector-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.0/README.md` & `databricks_sql_connector-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.0/pyproject.toml` & `databricks_sql_connector-2.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databricks-sql-connector"
-version = "2.5.0"
+version = "2.5.1"
 description = "Databricks SQL Connector for Python"
 authors = ["Databricks <databricks-sql-connector-maintainers@databricks.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "databricks", from = "src"}]
 include = ["CHANGELOG.md"]
 
@@ -19,15 +19,15 @@
 lz4 = "^4.0.2"
 requests="^2.18.1"
 oauthlib="^3.1.0"
 numpy = [
     {version = ">=1.16.6", python = ">=3.7,<3.11"},
     {version = ">=1.23.4", python = ">=3.11"}
 ]
-sqlalchemy = "^1.4.44"
+sqlalchemy = "^1.3.24"
 openpyxl = "^3.0.10"
 alembic = "^1.8.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 mypy = "^0.950"
 pylint = ">=2.12.0"
```

### Comparing `databricks_sql_connector-2.5.0/src/databricks/sql/__init__.py` & `databricks_sql_connector-2.5.1/src/databricks/sql/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 NUMBER = DBAPITypeObject(
     "boolean", "tinyint", "smallint", "int", "bigint", "float", "double", "decimal"
 )
 DATETIME = DBAPITypeObject("timestamp")
 DATE = DBAPITypeObject("date")
 ROWID = DBAPITypeObject()
 
-__version__ = "2.5.0"
+__version__ = "2.5.1"
 USER_AGENT_NAME = "PyDatabricksSqlConnector"
 
 # These two functions are pyhive legacy
 Date = datetime.date
 Timestamp = datetime.datetime
```

### Comparing `databricks_sql_connector-2.5.0/src/databricks/sql/auth/auth.py` & `databricks_sql_connector-2.5.1/src/databricks/sql/auth/auth.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.0/src/databricks/sql/auth/authenticators.py` & `databricks_sql_connector-2.5.1/src/databricks/sql/auth/authenticators.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.0/src/databricks/sql/auth/oauth.py` & `databricks_sql_connector-2.5.1/src/databricks/sql/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.0/src/databricks/sql/auth/oauth_http_handler.py` & `databricks_sql_connector-2.5.1/src/databricks/sql/auth/oauth_http_handler.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.0/src/databricks/sql/auth/thrift_http_client.py` & `databricks_sql_connector-2.5.1/src/databricks/sql/auth/thrift_http_client.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.0/src/databricks/sql/client.py` & `databricks_sql_connector-2.5.1/src/databricks/sql/client.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.0/src/databricks/sql/exc.py` & `databricks_sql_connector-2.5.1/src/databricks/sql/exc.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.0/src/databricks/sql/experimental/oauth_persistence.py` & `databricks_sql_connector-2.5.1/src/databricks/sql/experimental/oauth_persistence.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.0/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote` & `databricks_sql_connector-2.5.1/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.0/src/databricks/sql/thrift_api/TCLIService/TCLIService.py` & `databricks_sql_connector-2.5.1/src/databricks/sql/thrift_api/TCLIService/TCLIService.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.0/src/databricks/sql/thrift_api/TCLIService/constants.py` & `databricks_sql_connector-2.5.1/src/databricks/sql/thrift_api/TCLIService/constants.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.0/src/databricks/sql/thrift_api/TCLIService/ttypes.py` & `databricks_sql_connector-2.5.1/src/databricks/sql/thrift_api/TCLIService/ttypes.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.0/src/databricks/sql/thrift_backend.py` & `databricks_sql_connector-2.5.1/src/databricks/sql/thrift_backend.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.0/src/databricks/sql/types.py` & `databricks_sql_connector-2.5.1/src/databricks/sql/types.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.0/src/databricks/sql/utils.py` & `databricks_sql_connector-2.5.1/src/databricks/sql/utils.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.0/src/databricks/sqlalchemy/dialect/__init__.py` & `databricks_sql_connector-2.5.1/src/databricks/sqlalchemy/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.0/src/databricks/sqlalchemy/dialect/compiler.py` & `databricks_sql_connector-2.5.1/src/databricks/sqlalchemy/dialect/compiler.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.0/PKG-INFO` & `databricks_sql_connector-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-sql-connector
-Version: 2.5.0
+Version: 2.5.1
 Summary: Databricks SQL Connector for Python
 License: Apache-2.0
 Author: Databricks
 Author-email: databricks-sql-connector-maintainers@databricks.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -18,15 +18,15 @@
 Requires-Dist: numpy (>=1.23.4) ; python_version >= "3.11"
 Requires-Dist: oauthlib (>=3.1.0,<4.0.0)
 Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
 Requires-Dist: pandas (>=1.3.0,<2.0.0)
 Requires-Dist: pyarrow (>=10.0.1) ; python_version >= "3.11"
 Requires-Dist: pyarrow (>=6.0.0) ; python_version >= "3.7" and python_version < "3.11"
 Requires-Dist: requests (>=2.18.1,<3.0.0)
-Requires-Dist: sqlalchemy (>=1.4.44,<2.0.0)
+Requires-Dist: sqlalchemy (>=1.3.24,<2.0.0)
 Requires-Dist: thrift (>=0.16.0,<0.17.0)
 Project-URL: Bug Tracker, https://github.com/databricks/databricks-sql-python/issues
 Project-URL: Homepage, https://github.com/databricks/databricks-sql-python
 Description-Content-Type: text/markdown
 
 # Databricks SQL Connector for Python
```

