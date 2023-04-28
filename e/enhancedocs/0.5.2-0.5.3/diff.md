# Comparing `tmp/enhancedocs-0.5.2.tar.gz` & `tmp/enhancedocs-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhancedocs-0.5.2.tar", max compression
+gzip compressed data, was "enhancedocs-0.5.3.tar", max compression
```

## Comparing `enhancedocs-0.5.2.tar` & `enhancedocs-0.5.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11341 2023-04-27 19:25:43.287299 enhancedocs-0.5.2/LICENSE
--rw-r--r--   0        0        0     1031 2023-04-27 19:25:43.287299 enhancedocs-0.5.2/README.md
--rw-r--r--   0        0        0      453 2023-04-27 19:25:43.287299 enhancedocs-0.5.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-27 19:25:43.287299 enhancedocs-0.5.2/src/enhancedocs/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 19:25:43.287299 enhancedocs-0.5.2/src/enhancedocs/commands/__init__.py
--rw-r--r--   0        0        0      777 2023-04-27 19:25:43.287299 enhancedocs-0.5.2/src/enhancedocs/commands/ask.py
--rw-r--r--   0        0        0      940 2023-04-27 19:25:43.287299 enhancedocs-0.5.2/src/enhancedocs/commands/build.py
--rw-r--r--   0        0        0     1838 2023-04-27 19:25:43.287299 enhancedocs-0.5.2/src/enhancedocs/commands/push.py
--rw-r--r--   0        0        0     1151 2023-04-27 19:25:43.287299 enhancedocs-0.5.2/src/enhancedocs/config.py
--rw-r--r--   0        0        0      611 2023-04-27 19:25:43.287299 enhancedocs-0.5.2/src/enhancedocs/main.py
--rw-r--r--   0        0        0      311 2023-04-27 19:25:43.287299 enhancedocs-0.5.2/src/enhancedocs/utils.py
--rw-r--r--   0        0        0     1566 1970-01-01 00:00:00.000000 enhancedocs-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-04-28 15:37:31.662551 enhancedocs-0.5.3/LICENSE
+-rw-r--r--   0        0        0     1030 2023-04-28 15:37:31.662551 enhancedocs-0.5.3/README.md
+-rw-r--r--   0        0        0      474 2023-04-28 15:37:31.662551 enhancedocs-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-28 15:37:31.662551 enhancedocs-0.5.3/src/enhancedocs/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 15:37:31.662551 enhancedocs-0.5.3/src/enhancedocs/commands/__init__.py
+-rw-r--r--   0        0        0      778 2023-04-28 15:37:31.662551 enhancedocs-0.5.3/src/enhancedocs/commands/ask.py
+-rw-r--r--   0        0        0     1315 2023-04-28 15:37:31.662551 enhancedocs-0.5.3/src/enhancedocs/commands/build.py
+-rw-r--r--   0        0        0     1842 2023-04-28 15:37:31.662551 enhancedocs-0.5.3/src/enhancedocs/commands/push.py
+-rw-r--r--   0        0        0     1151 2023-04-28 15:37:31.662551 enhancedocs-0.5.3/src/enhancedocs/config.py
+-rw-r--r--   0        0        0      611 2023-04-28 15:37:31.662551 enhancedocs-0.5.3/src/enhancedocs/main.py
+-rw-r--r--   0        0        0     1212 2023-04-28 15:37:31.662551 enhancedocs-0.5.3/src/enhancedocs/utils.py
+-rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 enhancedocs-0.5.3/PKG-INFO
```

### Comparing `enhancedocs-0.5.2/LICENSE` & `enhancedocs-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.2/README.md` & `enhancedocs-0.5.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # EnhanceDocs CLI
 
 EnhanceDocs Command Line Interface (CLI)
 
 [![pypi version](https://img.shields.io/pypi/v/enhancedocs.svg)](https://pypi.org/pypi/enhancedocs/)
-[![Downloads](https://static.pepy.tech/badge/enhancedocs/month)](https://pypi.org/pypi/enhancedocs/)
+[![Downloads](https://static.pepy.tech/badge/enhancedocs/week)](https://pypi.org/pypi/enhancedocs/)
 [![License: MIT](https://img.shields.io/badge/license-Apache--2.0-yellow)](https://www.apache.org/licenses/LICENSE-2.0)
  [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/enhancedocs.svg?style=social&label=Follow%20%40EnhanceDocs)](https://twitter.com/enhancedocs)
 [![](https://dcbadge.vercel.app/api/server/AUDa3KZavw?compact=true&style=flat)](https://discord.gg/AUDa3KZavw)
 
 ## Requirements
 - [Python 3.11.2](https://www.python.org/downloads/)
```

### Comparing `enhancedocs-0.5.2/src/enhancedocs/commands/ask.py` & `enhancedocs-0.5.3/src/enhancedocs/commands/ask.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 
 @click.command()
 @click.option('--project', default=None, help='The project ID')
 @click.argument('question', nargs=-1, type=click.STRING)
 def ask(project, question):
     """Ask a question to your documentation"""
+
     if not question:
         raise click.UsageError('Provide a question')
     question = " ".join(question)
     params = {'question': question}
     if project:
         params['projectId'] = project
     try:
```

### Comparing `enhancedocs-0.5.2/src/enhancedocs/commands/push.py` & `enhancedocs-0.5.3/src/enhancedocs/commands/push.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             response = requests.put(f'{api_base_url}/ingest',
                                     data=file,
                                     params=params,
                                     headers=headers,
                                     stream=True
                                     )
             response.raise_for_status()
-            click.echo(f"✨ Ingestion finished in {response.elapsed.total_seconds()}s")
+            click.echo(f"✨ Ingestion finished in {response.elapsed.total_seconds():.4f}s")
     except requests.exceptions.RequestException as err:
         raise click.ClickException(str(err))
 
 
 def update_project_properties(params):
     try:
         with open('package.json', 'r', encoding='utf-8') as f:
```

### Comparing `enhancedocs-0.5.2/src/enhancedocs/config.py` & `enhancedocs-0.5.3/src/enhancedocs/config.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.2/src/enhancedocs/main.py` & `enhancedocs-0.5.3/src/enhancedocs/main.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.2/PKG-INFO` & `enhancedocs-0.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: enhancedocs
-Version: 0.5.2
+Version: 0.5.3
 Summary: EnhanceDocs Command Line Interface (CLI)
 License: Apache-2.0
 Author: Alvaro Molina
 Author-email: alw3ys@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: pathspec (>=0.11.1,<0.12.0)
 Requires-Dist: requests (>=2.29.0,<3.0.0)
 Requires-Dist: sentry-sdk (>=1.21.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # EnhanceDocs CLI
 
 EnhanceDocs Command Line Interface (CLI)
 
 [![pypi version](https://img.shields.io/pypi/v/enhancedocs.svg)](https://pypi.org/pypi/enhancedocs/)
-[![Downloads](https://static.pepy.tech/badge/enhancedocs/month)](https://pypi.org/pypi/enhancedocs/)
+[![Downloads](https://static.pepy.tech/badge/enhancedocs/week)](https://pypi.org/pypi/enhancedocs/)
 [![License: MIT](https://img.shields.io/badge/license-Apache--2.0-yellow)](https://www.apache.org/licenses/LICENSE-2.0)
  [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/enhancedocs.svg?style=social&label=Follow%20%40EnhanceDocs)](https://twitter.com/enhancedocs)
 [![](https://dcbadge.vercel.app/api/server/AUDa3KZavw?compact=true&style=flat)](https://discord.gg/AUDa3KZavw)
 
 ## Requirements
 - [Python 3.11.2](https://www.python.org/downloads/)
```

