# Comparing `tmp/property-lister-1.9.tar.gz` & `tmp/property-lister-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "property-lister-1.9.tar", last modified: Wed Apr 12 13:10:11 2023, max compression
+gzip compressed data, was "property-lister-2.0.tar", last modified: Fri Apr 28 13:27:06 2023, max compression
```

## Comparing `property-lister-1.9.tar` & `property-lister-2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 13:10:11.074415 property-lister-1.9/
--rwxrwx---   0 root         (0) root         (0)     1090 2023-04-09 10:26:05.000000 property-lister-1.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2961 2023-04-12 13:10:11.074415 property-lister-1.9/PKG-INFO
--rwxrwx---   0 root         (0) root         (0)     2594 2023-04-12 13:10:03.000000 property-lister-1.9/README.md
--rwxrwx---   0 root         (0) root         (0)      728 2023-04-12 13:09:51.000000 property-lister-1.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 13:10:11.074415 property-lister-1.9/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 13:10:11.074415 property-lister-1.9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 13:10:11.074415 property-lister-1.9/src/property_lister/
--rwxrwx---   0 root         (0) root         (0)        0 2023-04-09 10:26:05.000000 property-lister-1.9/src/property_lister/__init__.py
--rwxrwx---   0 root         (0) root         (0)     9446 2023-04-12 13:09:40.000000 property-lister-1.9/src/property_lister/property_lister.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 13:10:11.074415 property-lister-1.9/src/property_lister.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2961 2023-04-12 13:10:11.000000 property-lister-1.9/src/property_lister.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      363 2023-04-12 13:10:11.000000 property-lister-1.9/src/property_lister.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 13:10:11.000000 property-lister-1.9/src/property_lister.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-12 13:10:11.000000 property-lister-1.9/src/property_lister.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-12 13:10:11.000000 property-lister-1.9/src/property_lister.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-12 13:10:11.000000 property-lister-1.9/src/property_lister.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:27:06.370049 property-lister-2.0/
+-rwxrwx---   0 root         (0) root         (0)     1090 2023-04-28 13:21:40.000000 property-lister-2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-04-28 13:27:06.370049 property-lister-2.0/PKG-INFO
+-rwxrwx---   0 root         (0) root         (0)     2594 2023-04-28 13:23:50.000000 property-lister-2.0/README.md
+-rwxrwx---   0 root         (0) root         (0)      728 2023-04-28 13:26:29.000000 property-lister-2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 13:27:06.370049 property-lister-2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:27:06.370049 property-lister-2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:27:06.370049 property-lister-2.0/src/property_lister/
+-rwxrwx---   0 root         (0) root         (0)        0 2023-04-28 13:21:40.000000 property-lister-2.0/src/property_lister/__init__.py
+-rwxrwx---   0 root         (0) root         (0)     9486 2023-04-28 13:25:06.000000 property-lister-2.0/src/property_lister/property_lister.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:27:06.370049 property-lister-2.0/src/property_lister.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-04-28 13:27:06.000000 property-lister-2.0/src/property_lister.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      363 2023-04-28 13:27:06.000000 property-lister-2.0/src/property_lister.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 13:27:06.000000 property-lister-2.0/src/property_lister.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-28 13:27:06.000000 property-lister-2.0/src/property_lister.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-28 13:27:06.000000 property-lister-2.0/src/property_lister.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-28 13:27:06.000000 property-lister-2.0/src/property_lister.egg-info/top_level.txt
```

### Comparing `property-lister-1.9/LICENSE` & `property-lister-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `property-lister-1.9/PKG-INFO` & `property-lister-2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: property-lister
-Version: 1.9
+Version: 2.0
 Summary: Extract property list files from an SQLite unencrypted database file.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/property-lister
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Property Lister
 
 Extract and convert property list files from SQLite database files and from other property list files.
@@ -29,31 +29,31 @@
 ## How to Install
 
 ```bash
 pip3 install property-lister
 
 pip3 install --upgrade property-lister
 
-apt-get install -y plistutil
+apt-get -y install plistutil
 ```
 
 ## How to Build and Install Manually
 
 Run the following commands:
 
 ```bash
 git clone https://github.com/ivan-sincek/property-lister && cd property-lister
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/property_lister-1.9-py3-none-any.whl
+python3 -m pip install dist/property_lister-2.0-py3-none-any.whl
 
-apt-get install -y plistutil
+apt-get -y install plistutil
 ```
 
 ## Extracting and Converting
 
 Extract and convert property list files inside Cache.db unencrypted SQLite database file:
 
 ```fundamental
@@ -75,15 +75,15 @@
 Repeat the same for the app specific directories.
 
 Check my other project on how to [find files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#3-search-for-files-and-directories) and on how to [extract sensitive data from the files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#4-inspect-files).
 
 ## Usage
 
 ```fundamental
-Property Lister v1.9 ( github.com/ivan-sincek/property-lister )
+Property Lister v2.0 ( github.com/ivan-sincek/property-lister )
 
 --- Extract from an SQLite database file ---
 Usage:   property-lister -db database -o out
 Example: property-lister -db Cache.db -o results
 
 --- Extract from a property list file ---
 Usage:   property-lister -pl property-list -o out
```

### Comparing `property-lister-1.9/README.md` & `property-lister-2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -16,31 +16,31 @@
 ## How to Install
 
 ```bash
 pip3 install property-lister
 
 pip3 install --upgrade property-lister
 
-apt-get install -y plistutil
+apt-get -y install plistutil
 ```
 
 ## How to Build and Install Manually
 
 Run the following commands:
 
 ```bash
 git clone https://github.com/ivan-sincek/property-lister && cd property-lister
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/property_lister-1.9-py3-none-any.whl
+python3 -m pip install dist/property_lister-2.0-py3-none-any.whl
 
-apt-get install -y plistutil
+apt-get -y install plistutil
 ```
 
 ## Extracting and Converting
 
 Extract and convert property list files inside Cache.db unencrypted SQLite database file:
 
 ```fundamental
@@ -62,15 +62,15 @@
 Repeat the same for the app specific directories.
 
 Check my other project on how to [find files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#3-search-for-files-and-directories) and on how to [extract sensitive data from the files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#4-inspect-files).
 
 ## Usage
 
 ```fundamental
-Property Lister v1.9 ( github.com/ivan-sincek/property-lister )
+Property Lister v2.0 ( github.com/ivan-sincek/property-lister )
 
 --- Extract from an SQLite database file ---
 Usage:   property-lister -db database -o out
 Example: property-lister -db Cache.db -o results
 
 --- Extract from a property list file ---
 Usage:   property-lister -pl property-list -o out
```

### Comparing `property-lister-1.9/pyproject.toml` & `property-lister-2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "property-lister"
-version = "1.9"
+version = "2.0"
 authors = [{ name = "Ivan Sincek" }]
 description = "Extract property list files from an SQLite unencrypted database file."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
-	"Operating System :: OS Independent"
+	"Operating System :: POSIX :: Linux"
 ]
 dependencies = ["datetime>=5.0", "biplist>=1.0.3"]
 
 [project.urls]
 "Homepage" = "https://github.com/ivan-sincek/property-lister"
 
 [project.scripts]
```

### Comparing `property-lister-1.9/src/property_lister/property_lister.py` & `property-lister-2.0/src/property_lister/property_lister.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 start = datetime.datetime.now()
 
 # -------------------------- INFO --------------------------
 
 def basic():
 	global proceed
 	proceed = False
-	print("Property Lister v1.9 ( github.com/ivan-sincek/property-lister )")
+	print("Property Lister v2.0 ( github.com/ivan-sincek/property-lister )")
 	print("")
 	print("--- Extract from an SQLite database file ---")
 	print("Usage:   property-lister -db database -o out")
 	print("Example: property-lister -db Cache.db -o results")
 	print("")
 	print("--- Extract from a property list file ---")
 	print("Usage:   property-lister -pl property-list -o out")
@@ -252,24 +252,24 @@
 		if not ((args["database"] is not None and args["out"] is not None) or (args["plist"] is not None and args["out"] is not None)) or (args["database"] is not None and args["plist"] is not None) or not check(argc, args):
 			error("Missing a mandatory option (-db, -o)")
 			error("Missing a mandatory option (-pl, -o)", True)
 	else:
 		error("Incorrect usage", True)
 
 	if proceed and check_directory(args["out"]):
-		print("######################################################################")
-		print("#                                                                    #")
-		print("#                        Property Lister v1.9                        #")
-		print("#                                   by Ivan Sincek                   #")
-		print("#                                                                    #")
-		print("# Extract and convert property list files.                           #")
-		print("# GitHub repository at github.com/ivan-sincek/property-lister.       #")
-		print("# Feel free to donate bitcoin at 1BrZM6T7G9RN8vbabnfXu4M6Lpgztq6Y14. #")
-		print("#                                                                    #")
-		print("######################################################################")
+		print("##########################################################################")
+		print("#                                                                        #")
+		print("#                          Property Lister v2.0                          #")
+		print("#                                     by Ivan Sincek                     #")
+		print("#                                                                        #")
+		print("# Extract and convert property list files.                               #")
+		print("# GitHub repository at github.com/ivan-sincek/property-lister.           #")
+		print("# Feel free to donate ETH at 0xbc00e800f29524AD8b0968CEBEAD4cD5C5c1f105. #")
+		print("#                                                                        #")
+		print("##########################################################################")
 		if args["database"]:
 			dump(args["database"], args["out"])
 		elif args["plist"]:
 			for file in args["plist"]:
 				extract(file, args["out"], False)
 		length = len(os.listdir(args["out"]))
 		if not length:
```

### Comparing `property-lister-1.9/src/property_lister.egg-info/PKG-INFO` & `property-lister-2.0/src/property_lister.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: property-lister
-Version: 1.9
+Version: 2.0
 Summary: Extract property list files from an SQLite unencrypted database file.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/property-lister
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Property Lister
 
 Extract and convert property list files from SQLite database files and from other property list files.
@@ -29,31 +29,31 @@
 ## How to Install
 
 ```bash
 pip3 install property-lister
 
 pip3 install --upgrade property-lister
 
-apt-get install -y plistutil
+apt-get -y install plistutil
 ```
 
 ## How to Build and Install Manually
 
 Run the following commands:
 
 ```bash
 git clone https://github.com/ivan-sincek/property-lister && cd property-lister
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/property_lister-1.9-py3-none-any.whl
+python3 -m pip install dist/property_lister-2.0-py3-none-any.whl
 
-apt-get install -y plistutil
+apt-get -y install plistutil
 ```
 
 ## Extracting and Converting
 
 Extract and convert property list files inside Cache.db unencrypted SQLite database file:
 
 ```fundamental
@@ -75,15 +75,15 @@
 Repeat the same for the app specific directories.
 
 Check my other project on how to [find files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#3-search-for-files-and-directories) and on how to [extract sensitive data from the files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#4-inspect-files).
 
 ## Usage
 
 ```fundamental
-Property Lister v1.9 ( github.com/ivan-sincek/property-lister )
+Property Lister v2.0 ( github.com/ivan-sincek/property-lister )
 
 --- Extract from an SQLite database file ---
 Usage:   property-lister -db database -o out
 Example: property-lister -db Cache.db -o results
 
 --- Extract from a property list file ---
 Usage:   property-lister -pl property-list -o out
```

