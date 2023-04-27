# Comparing `tmp/pymsasdax-2023.1016.tar.gz` & `tmp/pymsasdax-2023.1017.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymsasdax-2023.1016.tar", last modified: Thu Feb 23 16:22:39 2023, max compression
+gzip compressed data, was "pymsasdax-2023.1017.tar", last modified: Thu Apr 27 21:48:24 2023, max compression
```

## Comparing `pymsasdax-2023.1016.tar` & `pymsasdax-2023.1017.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-02-23 16:22:39.902890 pymsasdax-2023.1016/
--rw-rw-rw-   0        0        0     1084 2023-02-20 22:20:56.000000 pymsasdax-2023.1016/LICENSE
--rw-rw-rw-   0        0        0        0 2023-02-21 01:10:15.000000 pymsasdax-2023.1016/MANIFEST.in
--rw-rw-rw-   0        0        0     5965 2023-02-23 16:22:39.900371 pymsasdax-2023.1016/PKG-INFO
--rw-rw-rw-   0        0        0     4130 2023-02-23 16:20:35.000000 pymsasdax-2023.1016/README.md
--rw-rw-rw-   0        0        0     1218 2023-02-23 16:21:22.000000 pymsasdax-2023.1016/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-23 16:22:39.904890 pymsasdax-2023.1016/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-23 16:22:39.826330 pymsasdax-2023.1016/src/
-drwxrwxrwx   0        0        0        0 2023-02-23 16:22:39.860928 pymsasdax-2023.1016/src/pymsasdax/
--rw-rw-rw-   0        0        0       23 2023-02-23 16:21:22.000000 pymsasdax-2023.1016/src/pymsasdax/__init__.py
--rw-rw-rw-   0        0        0     6925 2023-02-23 16:03:15.000000 pymsasdax-2023.1016/src/pymsasdax/dax.py
-drwxrwxrwx   0        0        0        0 2023-02-23 16:22:39.893419 pymsasdax-2023.1016/src/pymsasdax.egg-info/
--rw-rw-rw-   0        0        0     5965 2023-02-23 16:22:39.000000 pymsasdax-2023.1016/src/pymsasdax.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-02-23 16:22:39.000000 pymsasdax-2023.1016/src/pymsasdax.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-23 16:22:39.000000 pymsasdax-2023.1016/src/pymsasdax.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-02-23 16:22:39.000000 pymsasdax-2023.1016/src/pymsasdax.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-02-23 16:22:39.000000 pymsasdax-2023.1016/src/pymsasdax.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 21:48:24.638844 pymsasdax-2023.1017/
+-rw-rw-rw-   0        0        0     1084 2023-02-20 22:20:56.000000 pymsasdax-2023.1017/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-02-21 01:10:15.000000 pymsasdax-2023.1017/MANIFEST.in
+-rw-rw-rw-   0        0        0     6017 2023-04-27 21:48:24.635797 pymsasdax-2023.1017/PKG-INFO
+-rw-rw-rw-   0        0        0     4182 2023-04-27 21:44:56.000000 pymsasdax-2023.1017/README.md
+-rw-rw-rw-   0        0        0     1218 2023-04-27 21:44:00.000000 pymsasdax-2023.1017/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 21:48:24.641767 pymsasdax-2023.1017/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 21:48:24.536098 pymsasdax-2023.1017/src/
+drwxrwxrwx   0        0        0        0 2023-04-27 21:48:24.576973 pymsasdax-2023.1017/src/pymsasdax/
+-rw-rw-rw-   0        0        0       23 2023-04-27 21:44:00.000000 pymsasdax-2023.1017/src/pymsasdax/__init__.py
+-rw-rw-rw-   0        0        0     6925 2023-04-27 21:39:06.000000 pymsasdax-2023.1017/src/pymsasdax/dax.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:48:24.624692 pymsasdax-2023.1017/src/pymsasdax.egg-info/
+-rw-rw-rw-   0        0        0     6017 2023-04-27 21:48:24.000000 pymsasdax-2023.1017/src/pymsasdax.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-04-27 21:48:24.000000 pymsasdax-2023.1017/src/pymsasdax.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 21:48:24.000000 pymsasdax-2023.1017/src/pymsasdax.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-27 21:48:24.000000 pymsasdax-2023.1017/src/pymsasdax.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-27 21:48:24.000000 pymsasdax-2023.1017/src/pymsasdax.egg-info/top_level.txt
```

### Comparing `pymsasdax-2023.1016/LICENSE` & `pymsasdax-2023.1017/LICENSE`

 * *Files identical despite different names*

### Comparing `pymsasdax-2023.1016/PKG-INFO` & `pymsasdax-2023.1017/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymsasdax
-Version: 2023.1016
+Version: 2023.1017
 Summary: Run DAX queries against Analysis Services and get Pandas Dataframes
 Author-email: Gage Renzi <gagerenzi+pypy@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 grenzi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -119,14 +119,16 @@
     print(df)
 ```
 
 # Dev Notes
 
 ## Version History
 
+* 2023.1017
+  * fix bug using effective_user_name
 * 2023.1016
   * Add at least some docstrings
   * Add Premium XMLA endpoint example
   * Add effective_user_name parameter to connection
   * Pass **kwargs as additional connection string key value pairs
 * 2023.1013
   * Fix issue with column names populating from when i made initial package version
```

### Comparing `pymsasdax-2023.1016/README.md` & `pymsasdax-2023.1017/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,16 @@
     print(df)
 ```
 
 # Dev Notes
 
 ## Version History
 
+* 2023.1017
+  * fix bug using effective_user_name
 * 2023.1016
   * Add at least some docstrings
   * Add Premium XMLA endpoint example
   * Add effective_user_name parameter to connection
   * Pass **kwargs as additional connection string key value pairs
 * 2023.1013
   * Fix issue with column names populating from when i made initial package version
```

### Comparing `pymsasdax-2023.1016/pyproject.toml` & `pymsasdax-2023.1017/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools", ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pymsasdax"
-version = "2023.1016"
+version = "2023.1017"
 description = "Run DAX queries against Analysis Services and get Pandas Dataframes"
 readme = "README.md"
 authors = [{ name = "Gage Renzi", email = "gagerenzi+pypy@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -27,15 +27,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "pip-tools"]
 
 [project.urls]
 Homepage = "https://github.com/grenzi/pymsasdax"
 
 [tool.bumpver]
-current_version = "2023.1016"
+current_version = "2023.1017"
 version_pattern = "YYYY.BUILD"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `pymsasdax-2023.1016/src/pymsasdax/dax.py` & `pymsasdax-2023.1017/src/pymsasdax/dax.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import clr
-import pandas as pd
 import dateparser
+import pandas as pd
 
 
 class Connection:
     """A class for running DAX queries against Microsoft SQL Server Analysis Services Tabular Models, Azure Analysis Services, or Power BI XMLA endpoints
 
     Args:
-    conn_str (str): Optional connection string for the connection.
     initial_catalog (str): Required if conn_str is not specified. Initial Catalog of the server.
     data_source (str): Required if conn_str is not specified. Data Source of the server.
     uid (str): User ID for authentication. Default is empty string.
     password (str): Password for authentication. Default is empty string.
     effective_user_name (str): Username to impersonate, usually a UPN, such as joe@contoso.com
     tidy_column_names (bool): Flag for tidying column names. Default is True.
     tidy_map_function (function): A function to tidy column names. Default is to use the internal one, which leaves capitalization alone, replaces spaces with underscores, and removes square brackets.
     timeout (int): Timeout period (in seconds) for running queries. Default is 30.
+    conn_str (str): Optional connection string for the connection.
     **kwargs: Additional keyword value pairs, will be added to the connection string. 
 
     Raises:
     ValueError: If initial_catalog and data_source are not specified when conn_str is not passed.
 
     Methods:
     _handle_oledb_field(f): Handles different data types returned from OleDbConnection query.
@@ -28,36 +28,36 @@
     __exit__(exc_type, exc_value, traceback): Closes the connection when exiting the context.
     query(daxcmd): Executes a DAX query on the connected server and returns the result as a Pandas DataFrame.
 
     Returns: Nothing
     """
     def __init__(
         self,
-        conn_str=None,
         initial_catalog=None,
         data_source=None,
         uid="",
         password="",
         effective_user_name=None,
         tidy_column_names=True,
         tidy_map_function=None,
         timeout=30,
+        conn_str=None,
         **kwargs
     ):
         """Initializes the Connection object."""
         if conn_str is not None:
             self._connection_string = conn_str
         else:
             if not "initial_catalog" or not "data_source":
                 raise ValueError(
-                    f"initial_catalog and data_source must be specificed if not passing a connection string"
+                    "initial_catalog and data_source must be specificed if not passing a connection string"
                 )
             self._connection_string = f"Provider=MSOLAP;Persist Security Info=True;Initial Catalog={initial_catalog};Data Source={data_source};Timeout={timeout};UID={uid};Password={password}"
             if effective_user_name:
-                self._connection_string += f"EffectiveUserName={effective_user_name};"
+                self._connection_string += f";EffectiveUserName={effective_user_name};"
             for key, value in kwargs.items():
                 self._connection_string += f"{key}={value};"
 
         self._connection = None
         self._tidy_column_names = tidy_column_names
         self._tidy_map_function = tidy_map_function
         clr.AddReference("System.Data")
```

### Comparing `pymsasdax-2023.1016/src/pymsasdax.egg-info/PKG-INFO` & `pymsasdax-2023.1017/src/pymsasdax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymsasdax
-Version: 2023.1016
+Version: 2023.1017
 Summary: Run DAX queries against Analysis Services and get Pandas Dataframes
 Author-email: Gage Renzi <gagerenzi+pypy@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 grenzi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -119,14 +119,16 @@
     print(df)
 ```
 
 # Dev Notes
 
 ## Version History
 
+* 2023.1017
+  * fix bug using effective_user_name
 * 2023.1016
   * Add at least some docstrings
   * Add Premium XMLA endpoint example
   * Add effective_user_name parameter to connection
   * Pass **kwargs as additional connection string key value pairs
 * 2023.1013
   * Fix issue with column names populating from when i made initial package version
```

