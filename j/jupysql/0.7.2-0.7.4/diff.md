# Comparing `tmp/jupysql-0.7.2.tar.gz` & `tmp/jupysql-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupysql-0.7.2.tar", last modified: Tue Apr 25 23:07:07 2023, max compression
+gzip compressed data, was "jupysql-0.7.4.tar", last modified: Fri Apr 28 17:26:23 2023, max compression
```

## Comparing `jupysql-0.7.2.tar` & `jupysql-0.7.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-25 23:07:07.806642 jupysql-0.7.2/
--rw-r--r--   0 eduardo    (501) staff       (20)    11820 2023-03-30 15:02:40.000000 jupysql-0.7.2/LICENSE
--rw-r--r--   0 eduardo    (501) staff       (20)       52 2022-12-22 14:07:08.000000 jupysql-0.7.2/MANIFEST.in
--rw-r--r--   0 eduardo    (501) staff       (20)     3017 2023-04-25 23:07:07.806695 jupysql-0.7.2/PKG-INFO
--rw-r--r--   0 eduardo    (501) staff       (20)     2354 2023-04-13 14:31:32.000000 jupysql-0.7.2/README.md
--rw-r--r--   0 eduardo    (501) staff       (20)      701 2023-04-21 22:29:05.000000 jupysql-0.7.2/pyproject.toml
--rw-r--r--   0 eduardo    (501) staff       (20)      120 2023-04-25 23:07:07.806876 jupysql-0.7.2/setup.cfg
--rw-r--r--   0 eduardo    (501) staff       (20)     2138 2023-04-19 17:04:46.000000 jupysql-0.7.2/setup.py
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-25 23:07:07.802612 jupysql-0.7.2/src/
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-25 23:07:07.803948 jupysql-0.7.2/src/jupysql.egg-info/
--rw-r--r--   0 eduardo    (501) staff       (20)     3017 2023-04-25 23:07:07.000000 jupysql-0.7.2/src/jupysql.egg-info/PKG-INFO
--rw-r--r--   0 eduardo    (501) staff       (20)      836 2023-04-25 23:07:07.000000 jupysql-0.7.2/src/jupysql.egg-info/SOURCES.txt
--rw-r--r--   0 eduardo    (501) staff       (20)        1 2023-04-25 23:07:07.000000 jupysql-0.7.2/src/jupysql.egg-info/dependency_links.txt
--rw-r--r--   0 eduardo    (501) staff       (20)        1 2022-12-22 14:07:34.000000 jupysql-0.7.2/src/jupysql.egg-info/not-zip-safe
--rw-r--r--   0 eduardo    (501) staff       (20)      491 2023-04-25 23:07:07.000000 jupysql-0.7.2/src/jupysql.egg-info/requires.txt
--rw-r--r--   0 eduardo    (501) staff       (20)        4 2023-04-25 23:07:07.000000 jupysql-0.7.2/src/jupysql.egg-info/top_level.txt
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-25 23:07:07.805737 jupysql-0.7.2/src/sql/
--rw-r--r--   0 eduardo    (501) staff       (20)      169 2023-04-25 23:07:06.000000 jupysql-0.7.2/src/sql/__init__.py
--rw-r--r--   0 eduardo    (501) staff       (20)      544 2023-04-21 22:29:05.000000 jupysql-0.7.2/src/sql/_patch.py
--rw-r--r--   0 eduardo    (501) staff       (20)    10319 2023-04-12 23:53:59.000000 jupysql-0.7.2/src/sql/_testing.py
--rw-r--r--   0 eduardo    (501) staff       (20)     2899 2023-04-21 22:52:16.000000 jupysql-0.7.2/src/sql/column_guesser.py
--rw-r--r--   0 eduardo    (501) staff       (20)     2963 2023-04-25 22:57:19.000000 jupysql-0.7.2/src/sql/command.py
--rw-r--r--   0 eduardo    (501) staff       (20)    17895 2023-04-25 22:57:19.000000 jupysql-0.7.2/src/sql/connection.py
--rw-r--r--   0 eduardo    (501) staff       (20)     1159 2023-04-25 16:22:28.000000 jupysql-0.7.2/src/sql/exceptions.py
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-25 23:07:07.806131 jupysql-0.7.2/src/sql/ggplot/
--rw-r--r--   0 eduardo    (501) staff       (20)      248 2023-03-30 15:02:40.000000 jupysql-0.7.2/src/sql/ggplot/__init__.py
--rw-r--r--   0 eduardo    (501) staff       (20)      446 2023-03-30 15:02:40.000000 jupysql-0.7.2/src/sql/ggplot/aes.py
--rw-r--r--   0 eduardo    (501) staff       (20)     1092 2023-04-21 22:29:05.000000 jupysql-0.7.2/src/sql/ggplot/facet_wrap.py
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-25 23:07:07.806533 jupysql-0.7.2/src/sql/ggplot/geom/
--rw-r--r--   0 eduardo    (501) staff       (20)      158 2023-03-30 15:02:40.000000 jupysql-0.7.2/src/sql/ggplot/geom/__init__.py
--rw-r--r--   0 eduardo    (501) staff       (20)      327 2023-03-30 15:02:40.000000 jupysql-0.7.2/src/sql/ggplot/geom/geom.py
--rw-r--r--   0 eduardo    (501) staff       (20)      463 2023-03-30 15:02:40.000000 jupysql-0.7.2/src/sql/ggplot/geom/geom_boxplot.py
--rw-r--r--   0 eduardo    (501) staff       (20)     1060 2023-03-30 15:02:40.000000 jupysql-0.7.2/src/sql/ggplot/geom/geom_histogram.py
--rw-r--r--   0 eduardo    (501) staff       (20)     2412 2023-03-30 15:02:40.000000 jupysql-0.7.2/src/sql/ggplot/ggplot.py
--rw-r--r--   0 eduardo    (501) staff       (20)    10405 2023-04-25 16:22:28.000000 jupysql-0.7.2/src/sql/inspect.py
--rw-r--r--   0 eduardo    (501) staff       (20)    15400 2023-04-25 19:03:00.000000 jupysql-0.7.2/src/sql/magic.py
--rw-r--r--   0 eduardo    (501) staff       (20)     9161 2023-04-25 16:22:28.000000 jupysql-0.7.2/src/sql/magic_cmd.py
--rw-r--r--   0 eduardo    (501) staff       (20)     2692 2023-04-25 16:22:28.000000 jupysql-0.7.2/src/sql/magic_plot.py
--rw-r--r--   0 eduardo    (501) staff       (20)     2923 2023-04-21 16:12:23.000000 jupysql-0.7.2/src/sql/parse.py
--rw-r--r--   0 eduardo    (501) staff       (20)    15764 2023-04-21 22:29:05.000000 jupysql-0.7.2/src/sql/plot.py
--rw-r--r--   0 eduardo    (501) staff       (20)    16714 2023-04-25 16:22:28.000000 jupysql-0.7.2/src/sql/run.py
--rw-r--r--   0 eduardo    (501) staff       (20)     4949 2023-04-25 16:22:28.000000 jupysql-0.7.2/src/sql/store.py
--rw-r--r--   0 eduardo    (501) staff       (20)      326 2023-03-03 23:16:57.000000 jupysql-0.7.2/src/sql/telemetry.py
--rw-r--r--   0 eduardo    (501) staff       (20)     6923 2023-04-25 16:22:28.000000 jupysql-0.7.2/src/sql/util.py
+drwxr-xr-x   0 idomi      (501) staff       (20)        0 2023-04-28 17:26:23.758298 jupysql-0.7.4/
+-rw-r--r--   0 idomi      (501) staff       (20)    11820 2023-03-13 20:16:41.000000 jupysql-0.7.4/LICENSE
+-rw-r--r--   0 idomi      (501) staff       (20)       52 2022-12-28 16:23:15.000000 jupysql-0.7.4/MANIFEST.in
+-rw-r--r--   0 idomi      (501) staff       (20)     3017 2023-04-28 17:26:23.758382 jupysql-0.7.4/PKG-INFO
+-rw-r--r--   0 idomi      (501) staff       (20)     2354 2023-04-06 15:26:02.000000 jupysql-0.7.4/README.md
+-rw-r--r--   0 idomi      (501) staff       (20)      701 2023-04-21 18:56:18.000000 jupysql-0.7.4/pyproject.toml
+-rw-r--r--   0 idomi      (501) staff       (20)      120 2023-04-28 17:26:23.758697 jupysql-0.7.4/setup.cfg
+-rw-r--r--   0 idomi      (501) staff       (20)     2166 2023-04-28 16:54:46.000000 jupysql-0.7.4/setup.py
+drwxr-xr-x   0 idomi      (501) staff       (20)        0 2023-04-28 17:26:23.749342 jupysql-0.7.4/src/
+drwxr-xr-x   0 idomi      (501) staff       (20)        0 2023-04-28 17:26:23.752275 jupysql-0.7.4/src/jupysql.egg-info/
+-rw-r--r--   0 idomi      (501) staff       (20)     3017 2023-04-28 17:26:23.000000 jupysql-0.7.4/src/jupysql.egg-info/PKG-INFO
+-rw-r--r--   0 idomi      (501) staff       (20)      836 2023-04-28 17:26:23.000000 jupysql-0.7.4/src/jupysql.egg-info/SOURCES.txt
+-rw-r--r--   0 idomi      (501) staff       (20)        1 2023-04-28 17:26:23.000000 jupysql-0.7.4/src/jupysql.egg-info/dependency_links.txt
+-rw-r--r--   0 idomi      (501) staff       (20)        1 2022-12-28 16:24:18.000000 jupysql-0.7.4/src/jupysql.egg-info/not-zip-safe
+-rw-r--r--   0 idomi      (501) staff       (20)      522 2023-04-28 17:26:23.000000 jupysql-0.7.4/src/jupysql.egg-info/requires.txt
+-rw-r--r--   0 idomi      (501) staff       (20)        4 2023-04-28 17:26:23.000000 jupysql-0.7.4/src/jupysql.egg-info/top_level.txt
+drwxr-xr-x   0 idomi      (501) staff       (20)        0 2023-04-28 17:26:23.756136 jupysql-0.7.4/src/sql/
+-rw-r--r--   0 idomi      (501) staff       (20)      169 2023-04-28 17:09:04.000000 jupysql-0.7.4/src/sql/__init__.py
+-rw-r--r--   0 idomi      (501) staff       (20)      544 2023-04-21 18:56:18.000000 jupysql-0.7.4/src/sql/_patch.py
+-rw-r--r--   0 idomi      (501) staff       (20)    10319 2023-04-18 13:56:12.000000 jupysql-0.7.4/src/sql/_testing.py
+-rw-r--r--   0 idomi      (501) staff       (20)     2899 2023-03-03 16:02:07.000000 jupysql-0.7.4/src/sql/column_guesser.py
+-rw-r--r--   0 idomi      (501) staff       (20)     2964 2023-04-27 15:28:18.000000 jupysql-0.7.4/src/sql/command.py
+-rw-r--r--   0 idomi      (501) staff       (20)    17908 2023-04-27 15:28:18.000000 jupysql-0.7.4/src/sql/connection.py
+-rw-r--r--   0 idomi      (501) staff       (20)     1159 2023-04-27 15:28:18.000000 jupysql-0.7.4/src/sql/exceptions.py
+drwxr-xr-x   0 idomi      (501) staff       (20)        0 2023-04-28 17:26:23.756851 jupysql-0.7.4/src/sql/ggplot/
+-rw-r--r--   0 idomi      (501) staff       (20)      248 2023-03-31 19:06:22.000000 jupysql-0.7.4/src/sql/ggplot/__init__.py
+-rw-r--r--   0 idomi      (501) staff       (20)      446 2023-03-31 19:06:22.000000 jupysql-0.7.4/src/sql/ggplot/aes.py
+-rw-r--r--   0 idomi      (501) staff       (20)     1092 2023-04-21 18:56:18.000000 jupysql-0.7.4/src/sql/ggplot/facet_wrap.py
+drwxr-xr-x   0 idomi      (501) staff       (20)        0 2023-04-28 17:26:23.758173 jupysql-0.7.4/src/sql/ggplot/geom/
+-rw-r--r--   0 idomi      (501) staff       (20)      158 2023-03-31 19:06:22.000000 jupysql-0.7.4/src/sql/ggplot/geom/__init__.py
+-rw-r--r--   0 idomi      (501) staff       (20)      327 2023-03-23 19:57:06.000000 jupysql-0.7.4/src/sql/ggplot/geom/geom.py
+-rw-r--r--   0 idomi      (501) staff       (20)      463 2023-03-31 19:06:22.000000 jupysql-0.7.4/src/sql/ggplot/geom/geom_boxplot.py
+-rw-r--r--   0 idomi      (501) staff       (20)     1060 2023-03-31 19:06:22.000000 jupysql-0.7.4/src/sql/ggplot/geom/geom_histogram.py
+-rw-r--r--   0 idomi      (501) staff       (20)     2412 2023-03-31 19:06:22.000000 jupysql-0.7.4/src/sql/ggplot/ggplot.py
+-rw-r--r--   0 idomi      (501) staff       (20)    10405 2023-04-27 15:28:18.000000 jupysql-0.7.4/src/sql/inspect.py
+-rw-r--r--   0 idomi      (501) staff       (20)    15400 2023-04-27 15:28:18.000000 jupysql-0.7.4/src/sql/magic.py
+-rw-r--r--   0 idomi      (501) staff       (20)     9161 2023-04-27 15:28:18.000000 jupysql-0.7.4/src/sql/magic_cmd.py
+-rw-r--r--   0 idomi      (501) staff       (20)     2692 2023-04-27 15:28:18.000000 jupysql-0.7.4/src/sql/magic_plot.py
+-rw-r--r--   0 idomi      (501) staff       (20)     2923 2023-04-18 13:56:12.000000 jupysql-0.7.4/src/sql/parse.py
+-rw-r--r--   0 idomi      (501) staff       (20)    15764 2023-04-21 18:56:18.000000 jupysql-0.7.4/src/sql/plot.py
+-rw-r--r--   0 idomi      (501) staff       (20)    16714 2023-04-27 15:28:18.000000 jupysql-0.7.4/src/sql/run.py
+-rw-r--r--   0 idomi      (501) staff       (20)     4949 2023-04-27 15:28:18.000000 jupysql-0.7.4/src/sql/store.py
+-rw-r--r--   0 idomi      (501) staff       (20)      326 2023-03-03 16:02:07.000000 jupysql-0.7.4/src/sql/telemetry.py
+-rw-r--r--   0 idomi      (501) staff       (20)     6923 2023-04-27 15:28:18.000000 jupysql-0.7.4/src/sql/util.py
```

### Comparing `jupysql-0.7.2/LICENSE` & `jupysql-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.2/PKG-INFO` & `jupysql-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupysql
-Version: 0.7.2
+Version: 0.7.4
 Summary: Better SQL in Jupyter
 Home-page: https://github.com/ploomber/jupysql
 Author: Ploomber
 Author-email: contact@ploomber.io
 Project-URL: Source, https://github.com/ploomber/jupysql
 Keywords: database ipython postgresql mysql duckdb
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jupysql Version: 0.7.2 Summary: Better SQL in
+Metadata-Version: 2.1 Name: jupysql Version: 0.7.4 Summary: Better SQL in
 Jupyter Home-page: https://github.com/ploomber/jupysql Author: Ploomber Author-
 email: contact@ploomber.io Project-URL: Source, https://github.com/ploomber/
 jupysql Keywords: database ipython postgresql mysql duckdb Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Topic ::
 Database Classifier: Topic :: Database :: Front-Ends Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `jupysql-0.7.2/README.md` & `jupysql-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.2/pyproject.toml` & `jupysql-0.7.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.2/setup.py` & `jupysql-0.7.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open("src/sql/__init__.py", "rb") as f:
     VERSION = str(
         ast.literal_eval(_version_re.search(f.read().decode("utf-8")).group(1))
     )
 
 install_requires = [
     "prettytable",
-    "ipython>=1.0",
+    "ipython<=8.12.0; python_version == '3.8'",
     "sqlalchemy",
     "sqlparse",
     "ipython-genutils>=0.1.0",
     "sqlglot",
     "jinja2",
     "sqlglot>=11.3.7",
     "ploomber-core>=0.2.7",
```

### Comparing `jupysql-0.7.2/src/jupysql.egg-info/PKG-INFO` & `jupysql-0.7.4/src/jupysql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupysql
-Version: 0.7.2
+Version: 0.7.4
 Summary: Better SQL in Jupyter
 Home-page: https://github.com/ploomber/jupysql
 Author: Ploomber
 Author-email: contact@ploomber.io
 Project-URL: Source, https://github.com/ploomber/jupysql
 Keywords: database ipython postgresql mysql duckdb
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jupysql Version: 0.7.2 Summary: Better SQL in
+Metadata-Version: 2.1 Name: jupysql Version: 0.7.4 Summary: Better SQL in
 Jupyter Home-page: https://github.com/ploomber/jupysql Author: Ploomber Author-
 email: contact@ploomber.io Project-URL: Source, https://github.com/ploomber/
 jupysql Keywords: database ipython postgresql mysql duckdb Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Topic ::
 Database Classifier: Topic :: Database :: Front-Ends Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `jupysql-0.7.2/src/jupysql.egg-info/SOURCES.txt` & `jupysql-0.7.4/src/jupysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.2/src/sql/_patch.py` & `jupysql-0.7.4/src/sql/_patch.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.2/src/sql/_testing.py` & `jupysql-0.7.4/src/sql/_testing.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.2/src/sql/column_guesser.py` & `jupysql-0.7.4/src/sql/column_guesser.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.2/src/sql/command.py` & `jupysql-0.7.4/src/sql/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
             add_conn = False
 
         if one_arg and self.args.line[0] in Connection.connections:
             line_for_command = []
             add_alias = True
         else:
             add_alias = False
+
         self.command_text = " ".join(line_for_command) + "\n" + cell
 
         if self.args.file:
             with open(self.args.file, "r") as infile:
                 self.command_text = infile.read() + "\n" + self.command_text
 
         self.parsed = parse.parse(self.command_text, magic)
```

### Comparing `jupysql-0.7.2/src/sql/connection.py` & `jupysql-0.7.4/src/sql/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,15 @@
 
         if descriptor:
             is_custom_connection_ = Connection.is_custom_connection(descriptor)
 
             if isinstance(descriptor, Connection):
                 cls.current = descriptor
             elif isinstance(descriptor, Engine):
-                cls.current = Connection(descriptor)
+                cls.current = Connection(descriptor, alias=alias)
             elif is_custom_connection_:
                 cls.current = CustomConnection(descriptor, alias=alias)
             else:
                 existing = rough_dict_get(cls.connections, descriptor)
 
                 # NOTE: I added one indentation level, otherwise
                 # the "existing" variable would not exist if
```

### Comparing `jupysql-0.7.2/src/sql/exceptions.py` & `jupysql-0.7.4/src/sql/exceptions.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.2/src/sql/ggplot/facet_wrap.py` & `jupysql-0.7.4/src/sql/ggplot/facet_wrap.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.2/src/sql/ggplot/geom/geom_histogram.py` & `jupysql-0.7.4/src/sql/ggplot/geom/geom_histogram.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.2/src/sql/ggplot/ggplot.py` & `jupysql-0.7.4/src/sql/ggplot/ggplot.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.2/src/sql/inspect.py` & `jupysql-0.7.4/src/sql/inspect.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.2/src/sql/magic.py` & `jupysql-0.7.4/src/sql/magic.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.2/src/sql/magic_cmd.py` & `jupysql-0.7.4/src/sql/magic_cmd.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.2/src/sql/magic_plot.py` & `jupysql-0.7.4/src/sql/magic_plot.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.2/src/sql/parse.py` & `jupysql-0.7.4/src/sql/parse.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.2/src/sql/plot.py` & `jupysql-0.7.4/src/sql/plot.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.2/src/sql/run.py` & `jupysql-0.7.4/src/sql/run.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.2/src/sql/store.py` & `jupysql-0.7.4/src/sql/store.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.2/src/sql/util.py` & `jupysql-0.7.4/src/sql/util.py`

 * *Files identical despite different names*

