# Comparing `tmp/zoomaker-0.3.0.tar.gz` & `tmp/zoomaker-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoomaker-0.3.0.tar", max compression
+gzip compressed data, was "zoomaker-0.3.1.tar", max compression
```

## Comparing `zoomaker-0.3.0.tar` & `zoomaker-0.3.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     5252 2023-04-28 12:07:13.807392 zoomaker-0.3.0/README.md
--rw-r--r--   0        0        0      416 2023-04-28 13:00:06.190371 zoomaker-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6645 2023-04-28 13:00:02.284666 zoomaker-0.3.0/zoomaker.py
--rw-r--r--   0        0        0     5700 1970-01-01 00:00:00.000000 zoomaker-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     5252 2023-04-28 12:07:13.807392 zoomaker-0.3.1/README.md
+-rw-r--r--   0        0        0      587 2023-04-28 13:10:44.197861 zoomaker-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6645 2023-04-28 13:10:48.598419 zoomaker-0.3.1/zoomaker.py
+-rw-r--r--   0        0        0     5959 1970-01-01 00:00:00.000000 zoomaker-0.3.1/PKG-INFO
```

### Comparing `zoomaker-0.3.0/README.md` & `zoomaker-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `zoomaker-0.3.0/zoomaker.py` & `zoomaker-0.3.1/zoomaker.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
             return None
         return filename
 
 def main():
     parser = argparse.ArgumentParser(description="Install models, git repos and run scripts defined in the zoo.yaml file")
     parser.add_argument("command", nargs="?", default="help", choices=["install", "run"], help="The command to execute.")
     parser.add_argument("script", nargs="?", help="The script name to execute.")
-    parser.add_argument("-v", "--version", action='version', help="The current version of the zoomaker.", version="0.3.0")
+    parser.add_argument("-v", "--version", action='version', help="The current version of the zoomaker.", version="0.3.1")
 
     # print help if no arguments are provided
     try:
         args = parser.parse_args()
     except:
         parser.print_help()
         return
```

### Comparing `zoomaker-0.3.0/PKG-INFO` & `zoomaker-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: zoomaker
-Version: 0.3.0
-Summary: 
+Version: 0.3.1
+Summary: Zoomaker - Friendly house keeping for your AI model zoo and related resources.
+Home-page: https://github.com/hfg-gmuend/zoomaker
 Author: Benedikt Groß
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3.1.31,<4.0.0)
 Requires-Dist: huggingface-hub (>=0.14.0,<0.15.0)
+Project-URL: Documentation, https://github.com/hfg-gmuend/zoomaker
+Project-URL: Repository, https://github.com/hfg-gmuend/zoomaker
 Description-Content-Type: text/markdown
 
 Zoomaker - Friendly house keeping for your AI model zoo and related resources.
 ========
 
 Zoomaker is a command-line tool that helps install AI models, git repositories and run scripts.
```

