# Comparing `tmp/tiktok_uploader-1.0.0.tar.gz` & `tmp/tiktok_uploader-1.0.1.tar.gz`

## Comparing `tiktok_uploader-1.0.0.tar` & `tiktok_uploader-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/.DS_Store
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/LISCENSE
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/.github/workflows/build-hatch.yml
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/.github/workflows/link_checker.yml
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/examples/basic_upload.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/examples/multiple_videos_at_once.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/examples/series_upload.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/src/tiktok_uploader/__init__.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/src/tiktok_uploader/__main__.py
--rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/src/tiktok_uploader/auth.py
--rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/src/tiktok_uploader/browsers.py
--rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/src/tiktok_uploader/cli.py
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/src/tiktok_uploader/config.toml
--rw-r--r--   0        0        0    15745 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/src/tiktok_uploader/upload.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/src/tiktok_uploader/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/tests/test_browsers.py
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/tests/test_upload.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/.gitignore
--rw-r--r--   0        0        0     8787 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/README.md
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     9621 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.1/.DS_Store
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.1/LISCENSE
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.1/.github/workflows/build-hatch.yml
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.1/.github/workflows/link_checker.yml
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.1/examples/basic_upload.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.1/examples/multiple_videos_at_once.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.1/examples/series_upload.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.1/src/tiktok_uploader/__init__.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.1/src/tiktok_uploader/__main__.py
+-rw-r--r--   0        0        0     7186 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.1/src/tiktok_uploader/auth.py
+-rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.1/src/tiktok_uploader/browsers.py
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.1/src/tiktok_uploader/cli.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.1/src/tiktok_uploader/config.toml
+-rw-r--r--   0        0        0    15744 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.1/src/tiktok_uploader/upload.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.1/src/tiktok_uploader/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.1/tests/test_browsers.py
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.1/tests/test_upload.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.1/.gitignore
+-rw-r--r--   0        0        0     8787 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.1/README.md
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     9621 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.1/PKG-INFO
```

### Comparing `tiktok_uploader-1.0.0/.DS_Store` & `tiktok_uploader-1.0.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-1.0.0/LISCENSE` & `tiktok_uploader-1.0.1/LISCENSE`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-1.0.0/.github/workflows/build-hatch.yml` & `tiktok_uploader-1.0.1/.github/workflows/build-hatch.yml`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-1.0.0/examples/multiple_videos_at_once.py` & `tiktok_uploader-1.0.1/examples/multiple_videos_at_once.py`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-1.0.0/examples/series_upload.py` & `tiktok_uploader-1.0.1/examples/series_upload.py`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-1.0.0/src/tiktok_uploader/__init__.py` & `tiktok_uploader-1.0.1/src/tiktok_uploader/__init__.py`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-1.0.0/src/tiktok_uploader/auth.py` & `tiktok_uploader-1.0.1/src/tiktok_uploader/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,23 @@
 
         if not (self.cookies or (username and password)):
             raise InsufficientAuth()
 
         self.username = username
         self.password = password
 
+        if cookies:
+            logger.debug(green("Authenticating browser with cookies"))
+        elif username and password:
+            logger.debug(green("Authenticating browser with username and password"))
+        elif sessionid:
+            logger.debug(green("Authenticating browser with sessionid"))
+        elif cookies_list:
+            logger.debug(green("Authenticating browser with cookies_list"))
+
 
     def authenticate_agent(self, driver):
         """
         Authenticates the agent using the browser backend
         """
         # tries to use cookies
         if not self.cookies and self.username and self.password:
```

### Comparing `tiktok_uploader-1.0.0/src/tiktok_uploader/browsers.py` & `tiktok_uploader-1.0.1/src/tiktok_uploader/browsers.py`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-1.0.0/src/tiktok_uploader/cli.py` & `tiktok_uploader-1.0.1/src/tiktok_uploader/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     # runs the program using the arguments provided
     result = upload_video(
         filename=args.video,
         description=args.description,
         username=args.username,
         password=args.password,
         cookies=args.cookies,
-        session_id=args.sessionid,
+        sessionid=args.sessionid,
         headless=args.headless
     )
 
     print('-------------------------')
     if result:
         print('Error while uploading video')
     else:
```

### Comparing `tiktok_uploader-1.0.0/src/tiktok_uploader/config.toml` & `tiktok_uploader-1.0.1/src/tiktok_uploader/config.toml`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-1.0.0/src/tiktok_uploader/upload.py` & `tiktok_uploader-1.0.1/src/tiktok_uploader/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         The description to set for the video
     cookies : str
         The cookies to use for uploading
     sessionid: str
         The `sessionid` is the only required cookie for uploading,
             but it is recommended to use all cookies to avoid detection
     """
-    auth = AuthBackend(username=username, password=password, cookies=cookies, 
+    auth = AuthBackend(username=username, password=password, cookies=cookies,
                        cookies_list=cookies_list, sessionid=sessionid)
 
     return upload_videos(
             videos=[ { 'path': filename, 'description': description } ],
             auth=auth,
             *args, **kwargs
         )
```

### Comparing `tiktok_uploader-1.0.0/tests/test_browsers.py` & `tiktok_uploader-1.0.1/tests/test_browsers.py`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-1.0.0/tests/test_upload.py` & `tiktok_uploader-1.0.1/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-1.0.0/.gitignore` & `tiktok_uploader-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-1.0.0/README.md` & `tiktok_uploader-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-1.0.0/pyproject.toml` & `tiktok_uploader-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tiktok-uploader"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name = "William Kaiser", email = "wkaisertexas@gmail.com" },
 ]
 description = "An automatic TikTok video uploader w/ CLI. Uploads videos automatically using an automated browser and your cookies for authentication."
 readme = "README.md"
 requires-python = ">=3.0"
 keywords = [
```

### Comparing `tiktok_uploader-1.0.0/PKG-INFO` & `tiktok_uploader-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiktok-uploader
-Version: 1.0.0
+Version: 1.0.1
 Summary: An automatic TikTok video uploader w/ CLI. Uploads videos automatically using an automated browser and your cookies for authentication.
 Project-URL: Source Code, https://github.com/wkaisertexas/tiktok-uploader
 Project-URL: Bug Tracker, https://github.com/wkaisertexas/tiktok-uploader/issues
 Author-email: William Kaiser <wkaisertexas@gmail.com>
 Keywords: Automation,CLI,Command Line,Python,Selenium,TikTok,Upload,Video
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

