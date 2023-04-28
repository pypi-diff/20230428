# Comparing `tmp/dokos-1.0.5.tar.gz` & `tmp/dokos-1.0.6.tar.gz`

## Comparing `dokos-1.0.5.tar` & `dokos-1.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 dokos-1.0.5/.gitlab-ci.yml
--rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 dokos-1.0.5/10-million-password-list-top-1000.txt
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 dokos-1.0.5/pyproject.tmpl
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dokos-1.0.5/requirements.txt
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 dokos-1.0.5/.vscode/launch.json
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dokos-1.0.5/src/dokos/VERSION
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dokos-1.0.5/src/dokos/__init__.py
--rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 dokos-1.0.5/src/dokos/__main__.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 dokos-1.0.5/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 dokos-1.0.5/LICENSE
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 dokos-1.0.5/README.md
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 dokos-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 dokos-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 dokos-1.0.6/.gitlab-ci.yml
+-rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 dokos-1.0.6/10-million-password-list-top-1000.txt
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 dokos-1.0.6/pyproject.tmpl
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dokos-1.0.6/requirements.txt
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 dokos-1.0.6/.vscode/launch.json
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dokos-1.0.6/src/dokos/VERSION
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dokos-1.0.6/src/dokos/__init__.py
+-rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 dokos-1.0.6/src/dokos/__main__.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 dokos-1.0.6/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 dokos-1.0.6/LICENSE
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 dokos-1.0.6/README.md
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 dokos-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 dokos-1.0.6/PKG-INFO
```

### Comparing `dokos-1.0.5/.gitlab-ci.yml` & `dokos-1.0.6/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dokos-1.0.5/10-million-password-list-top-1000.txt` & `dokos-1.0.6/10-million-password-list-top-1000.txt`

 * *Files identical despite different names*

### Comparing `dokos-1.0.5/pyproject.tmpl` & `dokos-1.0.6/pyproject.tmpl`

 * *Files identical despite different names*

### Comparing `dokos-1.0.5/.vscode/launch.json` & `dokos-1.0.6/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dokos-1.0.5/src/dokos/__main__.py` & `dokos-1.0.6/src/dokos/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 PASSWORDS = []
 
 # found passwords
 FOUND = []
 
 def print_safe(string) :
     with LOCK:
-	    print(string)
+        print(string)
 
-def show_version() : 
+def show_version() :
     # where is this file located
     dirname = os.path.dirname(__file__)
     with open(os.path.join(dirname, './VERSION')) as version_file:
         version = version_file.read().strip()
         print("v" + version)
 
 def show_header() :
@@ -65,44 +65,44 @@
             ARGS.password_field : password
         }
 
     encoded_data = urllib.parse.urlencode(data).encode('ascii')
 
     request = urllib.request.Request(ARGS.url, encoded_data)
     try:
-        
         response = urllib.request.urlopen(request)
         page = response.read().decode()
 
         if not ARGS.failed in page :
             FOUND.append(password)
+            if ARGS.stop_on_first :
+                # ask threads to stop
+                global RUN
+                RUN = False
 
     except urllib.error.HTTPError as e:
         print_safe("Error: " + repr(e))
 
     except urllib.error.URLError as e:
-        print_safe("Error: " + repr(e))   
+        print_safe("Error: " + repr(e))
 
 def try_passwords(passwords):
     '''
     Try a list of passwords
     '''
 
     for password in passwords :
         global COUNT
         COUNT += 1
         # we were interrupted by user
         if not RUN :
             break
         password = password.strip()
-        print_safe("login: " + ARGS.login + " password: " + password)
+        print_safe("Trying " + ARGS.login + " and password " + password + " ...")
         try_password(password)
-        # stop if we found a password
-        if ARGS.stop_on_first and len(FOUND) > 0:
-            break
 
 def islice(iterable, *args):
     '''
     https://docs.python.org/3/library/itertools.html#recipes
     # islice('ABCDEFG', 2) --> A B
     # islice('ABCDEFG', 2, 4) --> C D
     # islice('ABCDEFG', 2, None) --> C D E F G
```

### Comparing `dokos-1.0.5/.gitignore` & `dokos-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `dokos-1.0.5/LICENSE` & `dokos-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dokos-1.0.5/README.md` & `dokos-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `dokos-1.0.5/pyproject.toml` & `dokos-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "Dokos"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Thibault Debatty", email="t.debatty@cylab.be" },
 ]
 description = "HTTP login cracker"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `dokos-1.0.5/PKG-INFO` & `dokos-1.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dokos
-Version: 1.0.5
+Version: 1.0.6
 Summary: HTTP login cracker
 Project-URL: Homepage, https://gitlab.cylab.be/cylab/dokos
 Project-URL: Bug Tracker, https://gitlab.cylab.be/cylab/dokos/-/issues
 Author-email: Thibault Debatty <t.debatty@cylab.be>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

