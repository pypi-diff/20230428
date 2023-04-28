# Comparing `tmp/shift_left_secure-0.2.2.tar.gz` & `tmp/shift_left_secure-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shift_left_secure-0.2.2.tar", max compression
+gzip compressed data, was "shift_left_secure-0.2.3.tar", max compression
```

## Comparing `shift_left_secure-0.2.2.tar` & `shift_left_secure-0.2.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1601 2023-04-27 17:41:42.013917 shift_left_secure-0.2.2/README.md
--rw-r--r--   0        0        0      516 2023-04-28 12:23:43.605956 shift_left_secure-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-29 04:11:10.773184 shift_left_secure-0.2.2/shift_left_secure/__init__.py
--rw-r--r--   0        0        0     1238 2023-03-29 12:35:12.607718 shift_left_secure-0.2.2/shift_left_secure/__main__.py
--rw-r--r--   0        0        0     2843 2023-03-29 11:50:35.517189 shift_left_secure-0.2.2/shift_left_secure/chatgpt_api.py
--rw-r--r--   0        0        0     2537 2023-04-28 12:22:16.965256 shift_left_secure-0.2.2/shift_left_secure/gh_action.py
--rw-r--r--   0        0        0     3773 2023-04-27 18:47:23.586572 shift_left_secure-0.2.2/shift_left_secure/git_handler.py
--rw-r--r--   0        0        0     2978 2023-04-28 06:51:55.743681 shift_left_secure-0.2.2/shift_left_secure/utils.py
--rw-r--r--   0        0        0     2314 1970-01-01 00:00:00.000000 shift_left_secure-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1601 2023-04-27 17:41:42.013917 shift_left_secure-0.2.3/README.md
+-rw-r--r--   0        0        0      516 2023-04-28 12:42:39.836485 shift_left_secure-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-29 04:11:10.773184 shift_left_secure-0.2.3/shift_left_secure/__init__.py
+-rw-r--r--   0        0        0     1238 2023-03-29 12:35:12.607718 shift_left_secure-0.2.3/shift_left_secure/__main__.py
+-rw-r--r--   0        0        0     2843 2023-03-29 11:50:35.517189 shift_left_secure-0.2.3/shift_left_secure/chatgpt_api.py
+-rw-r--r--   0        0        0     2539 2023-04-28 12:42:39.836754 shift_left_secure-0.2.3/shift_left_secure/gh_action.py
+-rw-r--r--   0        0        0     3773 2023-04-27 18:47:23.586572 shift_left_secure-0.2.3/shift_left_secure/git_handler.py
+-rw-r--r--   0        0        0     2978 2023-04-28 06:51:55.743681 shift_left_secure-0.2.3/shift_left_secure/utils.py
+-rw-r--r--   0        0        0     2315 1970-01-01 00:00:00.000000 shift_left_secure-0.2.3/PKG-INFO
```

### Comparing `shift_left_secure-0.2.2/README.md` & `shift_left_secure-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `shift_left_secure-0.2.2/pyproject.toml` & `shift_left_secure-0.2.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "shift-left-secure"
-version = "0.2.2"
+version = "0.2.3"
 description = "Mitigate vulnerabilities before pushing code to github/gitlab/bitbucket"
 authors = ["Dhrumil Mistry <56185972+dmdhrumilmistry@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "shift_left_secure"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
-openapi = "^1.1.0"
 gitpython = "3.1.18"
 pygithub = "^1.58.1"
 python-dotenv = "^1.0.0"
+openai = "^0.27.5"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `shift_left_secure-0.2.2/shift_left_secure/__main__.py` & `shift_left_secure-0.2.3/shift_left_secure/__main__.py`

 * *Files identical despite different names*

### Comparing `shift_left_secure-0.2.2/shift_left_secure/chatgpt_api.py` & `shift_left_secure-0.2.3/shift_left_secure/chatgpt_api.py`

 * *Files identical despite different names*

### Comparing `shift_left_secure-0.2.2/shift_left_secure/gh_action.py` & `shift_left_secure-0.2.3/shift_left_secure/gh_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     OPEN_API_KEY = environ.get('OPENAI_API_KEY')
     ACCESS_TOKEN = environ.get('GH_ACCESS_TOKEN')
     REPO = environ.get('GH_REPO')
     PR_NUMBER = int(environ.get('GH_PR_NUMBER','-1'))
 
     should_exit = True
     if not OPEN_API_KEY:
-        logger.error('OPEN_API_KEY env variable was not configured.')
+        logger.error('OPENAI_API_KEY env variable was not configured.')
     elif not ACCESS_TOKEN:
         logger.error('GH_ACCESS_TOKEN env variable was not configured.')
     elif not REPO:
         logger.error('GH_REPO env variable was not configured.')
     elif PR_NUMBER == -1:
         logger.error('GH_PR_NUMBER env variable was not configured.')
     else:
```

### Comparing `shift_left_secure-0.2.2/shift_left_secure/git_handler.py` & `shift_left_secure-0.2.3/shift_left_secure/git_handler.py`

 * *Files identical despite different names*

### Comparing `shift_left_secure-0.2.2/shift_left_secure/utils.py` & `shift_left_secure-0.2.3/shift_left_secure/utils.py`

 * *Files identical despite different names*

### Comparing `shift_left_secure-0.2.2/PKG-INFO` & `shift_left_secure-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: shift-left-secure
-Version: 0.2.2
+Version: 0.2.3
 Summary: Mitigate vulnerabilities before pushing code to github/gitlab/bitbucket
 Author: Dhrumil Mistry
 Author-email: 56185972+dmdhrumilmistry@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: gitpython (==3.1.18)
-Requires-Dist: openapi (>=1.1.0,<2.0.0)
+Requires-Dist: openai (>=0.27.5,<0.28.0)
 Requires-Dist: pygithub (>=1.58.1,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Shift Left N Secure
 
 Secure your project source code before pushing commits to github/gitlab/bitbucket. Project helps Software Development team to use shift left approach to find and mitigate issues at an early stage instead of taking action once code reaches to the production.
```

