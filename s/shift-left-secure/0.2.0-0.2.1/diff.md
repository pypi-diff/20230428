# Comparing `tmp/shift_left_secure-0.2.0.tar.gz` & `tmp/shift_left_secure-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shift_left_secure-0.2.0.tar", max compression
+gzip compressed data, was "shift_left_secure-0.2.1.tar", max compression
```

## Comparing `shift_left_secure-0.2.0.tar` & `shift_left_secure-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1601 2023-04-27 17:41:42.013917 shift_left_secure-0.2.0/README.md
--rw-r--r--   0        0        0      516 2023-04-28 09:39:26.150186 shift_left_secure-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-29 04:11:10.773184 shift_left_secure-0.2.0/shift_left_secure/__init__.py
--rw-r--r--   0        0        0     1238 2023-03-29 12:35:12.607718 shift_left_secure-0.2.0/shift_left_secure/__main__.py
--rw-r--r--   0        0        0     2843 2023-03-29 11:50:35.517189 shift_left_secure-0.2.0/shift_left_secure/chatgpt_api.py
--rw-r--r--   0        0        0     2504 2023-04-28 06:51:55.743407 shift_left_secure-0.2.0/shift_left_secure/gh_action.py
--rw-r--r--   0        0        0     3773 2023-04-27 18:47:23.586572 shift_left_secure-0.2.0/shift_left_secure/git_handler.py
--rw-r--r--   0        0        0     2978 2023-04-28 06:51:55.743681 shift_left_secure-0.2.0/shift_left_secure/utils.py
--rw-r--r--   0        0        0     2314 1970-01-01 00:00:00.000000 shift_left_secure-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1601 2023-04-27 17:41:42.013917 shift_left_secure-0.2.1/README.md
+-rw-r--r--   0        0        0      516 2023-04-28 12:19:00.185398 shift_left_secure-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-29 04:11:10.773184 shift_left_secure-0.2.1/shift_left_secure/__init__.py
+-rw-r--r--   0        0        0     1238 2023-03-29 12:35:12.607718 shift_left_secure-0.2.1/shift_left_secure/__main__.py
+-rw-r--r--   0        0        0     2843 2023-03-29 11:50:35.517189 shift_left_secure-0.2.1/shift_left_secure/chatgpt_api.py
+-rw-r--r--   0        0        0     2504 2023-04-28 12:18:22.981608 shift_left_secure-0.2.1/shift_left_secure/gh_action.py
+-rw-r--r--   0        0        0     3773 2023-04-27 18:47:23.586572 shift_left_secure-0.2.1/shift_left_secure/git_handler.py
+-rw-r--r--   0        0        0     2978 2023-04-28 06:51:55.743681 shift_left_secure-0.2.1/shift_left_secure/utils.py
+-rw-r--r--   0        0        0     2314 1970-01-01 00:00:00.000000 shift_left_secure-0.2.1/PKG-INFO
```

### Comparing `shift_left_secure-0.2.0/README.md` & `shift_left_secure-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `shift_left_secure-0.2.0/pyproject.toml` & `shift_left_secure-0.2.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shift-left-secure"
-version = "0.2.0"
+version = "0.2.1"
 description = "Mitigate vulnerabilities before pushing code to github/gitlab/bitbucket"
 authors = ["Dhrumil Mistry <56185972+dmdhrumilmistry@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "shift_left_secure"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
```

### Comparing `shift_left_secure-0.2.0/shift_left_secure/__main__.py` & `shift_left_secure-0.2.1/shift_left_secure/__main__.py`

 * *Files identical despite different names*

### Comparing `shift_left_secure-0.2.0/shift_left_secure/chatgpt_api.py` & `shift_left_secure-0.2.1/shift_left_secure/chatgpt_api.py`

 * *Files identical despite different names*

### Comparing `shift_left_secure-0.2.0/shift_left_secure/gh_action.py` & `shift_left_secure-0.2.1/shift_left_secure/gh_action.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,24 +53,24 @@
 
 
 
 if __name__ == '__main__':
     load_dotenv()
 
     # Replace with your GitHub access token
-    OPEN_API_KEY = environ.get('OPEN_API_KEY')
-    ACCESS_TOKEN = environ.get('GITHUB_ACCESS_TOKEN')
-    REPO = environ.get('REPO')
-    PR_NUMBER = int(environ.get('PR_NUMBER','-1'))
+    OPEN_API_KEY = environ.get('OPENAI_API_KEY')
+    ACCESS_TOKEN = environ.get('GH_ACCESS_TOKEN')
+    REPO = environ.get('GH_REPO')
+    PR_NUMBER = int(environ.get('GH_PR_NUMBER','-1'))
 
     should_exit = True
     if not OPEN_API_KEY:
         logger.error('OPEN_API_KEY env variable was not configured.')
     elif not ACCESS_TOKEN:
-        logger.error('GITHUB_ACCESS_TOKEN env variable was not configured.')
+        logger.error('GH_ACCESS_TOKEN env variable was not configured.')
     elif not REPO:
         logger.error('GITHUB_REPO env variable was not configured.')
     elif PR_NUMBER == -1:
         logger.error('PR_NUMBER env variable was not configured.')
     else:
         should_exit = False
         logger.info('ENV vars found.')
```

### Comparing `shift_left_secure-0.2.0/shift_left_secure/git_handler.py` & `shift_left_secure-0.2.1/shift_left_secure/git_handler.py`

 * *Files identical despite different names*

### Comparing `shift_left_secure-0.2.0/shift_left_secure/utils.py` & `shift_left_secure-0.2.1/shift_left_secure/utils.py`

 * *Files identical despite different names*

### Comparing `shift_left_secure-0.2.0/PKG-INFO` & `shift_left_secure-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shift-left-secure
-Version: 0.2.0
+Version: 0.2.1
 Summary: Mitigate vulnerabilities before pushing code to github/gitlab/bitbucket
 Author: Dhrumil Mistry
 Author-email: 56185972+dmdhrumilmistry@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

