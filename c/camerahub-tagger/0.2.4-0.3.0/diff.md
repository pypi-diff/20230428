# Comparing `tmp/camerahub_tagger-0.2.4.tar.gz` & `tmp/camerahub_tagger-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camerahub_tagger-0.2.4.tar", max compression
+gzip compressed data, was "camerahub_tagger-0.3.0.tar", max compression
```

## Comparing `camerahub_tagger-0.2.4.tar` & `camerahub_tagger-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2839 2023-04-26 20:08:17.718695 camerahub_tagger-0.2.4/README.md
--rw-r--r--   0        0        0        0 2023-04-26 20:08:17.718695 camerahub_tagger-0.2.4/camerahub_tagger/__init__.py
--rw-r--r--   0        0        0     2049 2023-04-26 20:08:17.718695 camerahub_tagger-0.2.4/camerahub_tagger/api.py
--rw-r--r--   0        0        0     2011 2023-04-26 20:08:17.718695 camerahub_tagger-0.2.4/camerahub_tagger/config.py
--rw-r--r--   0        0        0     5519 2023-04-26 20:08:17.718695 camerahub_tagger-0.2.4/camerahub_tagger/funcs.py
--rwxr-xr-x   0        0        0     5468 2023-04-26 20:08:17.718695 camerahub_tagger-0.2.4/camerahub_tagger/main.py
--rw-r--r--   0        0        0      649 2023-04-26 20:08:39.487991 camerahub_tagger-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3565 1970-01-01 00:00:00.000000 camerahub_tagger-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     2839 2023-04-27 19:02:15.940750 camerahub_tagger-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 19:02:15.944750 camerahub_tagger-0.3.0/camerahub_tagger/__init__.py
+-rw-r--r--   0        0        0     2049 2023-04-27 19:02:15.944750 camerahub_tagger-0.3.0/camerahub_tagger/api.py
+-rw-r--r--   0        0        0     2037 2023-04-27 19:02:15.944750 camerahub_tagger-0.3.0/camerahub_tagger/config.py
+-rw-r--r--   0        0        0     6352 2023-04-27 19:02:15.944750 camerahub_tagger-0.3.0/camerahub_tagger/funcs.py
+-rwxr-xr-x   0        0        0     5825 2023-04-27 19:02:15.944750 camerahub_tagger-0.3.0/camerahub_tagger/main.py
+-rw-r--r--   0        0        0      670 2023-04-27 19:02:34.533033 camerahub_tagger-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3607 1970-01-01 00:00:00.000000 camerahub_tagger-0.3.0/PKG-INFO
```

### Comparing `camerahub_tagger-0.2.4/README.md` & `camerahub_tagger-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `camerahub_tagger-0.2.4/camerahub_tagger/api.py` & `camerahub_tagger-0.3.0/camerahub_tagger/api.py`

 * *Files identical despite different names*

### Comparing `camerahub_tagger-0.2.4/camerahub_tagger/config.py` & `camerahub_tagger-0.3.0/camerahub_tagger/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Functions which handle config creation and retrieval for this app
 """
 
 import configparser
 import getpass
 import os
+from termcolor import cprint
 
 def create_config(path):
     """
     Create an empty config file in the user's home dir
     """
     config = configparser.ConfigParser()
 
@@ -23,29 +24,29 @@
 
     l_config.add_section(l_section)
 
     try:
         default = "https://camerahub.info/api"
         l_server = input(f"Enter CameraHub server for profile '{l_section}' (default {default}): ") or default
     except ValueError as error:
-        print('ERROR', error)
+        cprint(error, "red")
     else:
         l_config.set(l_section, "server", l_server)
 
     try:
         l_username = input(f"Enter CameraHub username for {l_server}: ")
     except ValueError as error:
-        print('ERROR', error)
+        cprint(error, "red")
     else:
         l_config.set(l_section, "username", l_username)
 
     try:
         l_password = getpass.getpass(prompt=f"Enter CameraHub password for {l_server}: ")
     except ValueError as error:
-        print('ERROR', error)
+        cprint(error, "red")
     else:
         l_config.set(l_section, "password", l_password)
 
     with open(l_path, "w", encoding="utf-8") as config_file:
         l_config.write(config_file)
```

### Comparing `camerahub_tagger-0.2.4/camerahub_tagger/funcs.py` & `camerahub_tagger-0.3.0/camerahub_tagger/funcs.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Utility functions with few external dependencies
 """
 
 from uuid import UUID
 from os.path import basename
 import re
 from deepdiff import DeepDiff
+from termcolor import cprint, colored
 
 
 def diff_tags(dicta, dictb):
     """
     Compare two dictionaries of EXIF tags and return a dictionary which contains
     the diff required to apply b's data to a, without destroying data in a.
     """
@@ -46,19 +47,19 @@
 
 
 def yes_or_no(question):
     """
     Prompt for a yes/no answer
     https://gist.github.com/garrettdreyfus/8153571#gistcomment-2586248
     """
-    answer = input(question + "(y/n): ").lower().strip()
+    answer = input(colored(question + "(y/n): ", "magenta")).lower().strip()
     print("")
     while not answer in ('y', 'yes', 'n', 'no'):
-        print("Input yes or no")
-        answer = input(question + "(y/n):").lower().strip()
+        cprint("Input yes or no", "magenta")
+        answer = input(colored(question + "(y/n): ", "magenta")).lower().strip()
         print("")
     return bool(answer[0] == "y")
 
 
 def is_valid_uuid(uuid_to_test, version=4):
     """
     Check if uuid_to_test is a valid UUID.
@@ -136,14 +137,15 @@
         'ExposureTime': 'Exif.Photo.ExposureTime',
         'Copyright': 'Exif.Image.Copyright',
         'FocalLengthIn35mmFilm': 'Exif.Photo.FocalLengthIn35mmFilm',
         'GPSLatitude': 'Exif.GPSInfo.GPSLatitude',
         'GPSLatitudeRef': 'Exif.GPSInfo.GPSLatitudeRef',
         'GPSLongitude': 'Exif.GPSInfo.GPSLongitude',
         'GPSLongitudeRef': 'Exif.GPSInfo.GPSLongitudeRef',
+        'ImageID': 'Exif.Image.ImageID',
     }
 
     exiftag = mapping.get(apitag)
     return exiftag
 
 
 def api2exif(l_apidata):
@@ -171,7 +173,24 @@
             # Do a mapping using the key lookup table
             exifkey = apitag2exiftag(key)
             if exifkey is not None:
                 # Cast all keys as strings
                 l_exifdata[exifkey] = str(value)
 
     return l_exifdata
+
+def asciiart():
+    # pylint: disable=anomalous-backslash-in-string
+    """
+    Return a fancy Ascii Art logo
+    """
+    figlet='''  ____                               _   _       _     
+ / ___|__ _ _ __ ___   ___ _ __ __ _| | | |_   _| |__  
+| |   / _` | '_ ` _ \ / _ \ '__/ _` | |_| | | | | '_ \ 
+| |__| (_| | | | | | |  __/ | | (_| |  _  | |_| | |_) |
+ \____\__,_|_| |_|_|_|\___|_|  \__,_|_| |_|\__,_|_.__/                             
+                |_   _|_ _  __ _  __ _  ___ _ __ 
+                  | |/ _` |/ _` |/ _` |/ _ \ '__|
+                  | | (_| | (_| | (_| |  __/ |   
+                  |_|\__,_|\__, |\__, |\___|_|   
+                           |___/ |___/'''
+    return figlet
```

### Comparing `camerahub_tagger-0.2.4/camerahub_tagger/main.py` & `camerahub_tagger-0.3.0/camerahub_tagger/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """
 CameraHub Tagger
 """
 
 import argparse
 import os
+from pathlib import Path
 from fnmatch import filter as fnfilter
 import pyexiv2
 from requests.models import HTTPError
+from termcolor import cprint
 from camerahub_tagger.config import get_setting
 from camerahub_tagger.api import get_negative, get_scan, create_scan, test_credentials
-from camerahub_tagger.funcs import is_valid_uuid, guess_frame, prompt_frame, api2exif, diff_tags, yes_or_no
+from camerahub_tagger.funcs import is_valid_uuid, guess_frame, prompt_frame, api2exif, diff_tags, yes_or_no, asciiart
 
 # ----------------------------------------------------------------------
 def main():
-    print("CameraHub Tagger")
+    cprint(asciiart(), 'light_blue')
 
     # Read in args
     parser = argparse.ArgumentParser()
     parser.add_argument('-r', '--recursive', help="Search for scans recursively", action='store_true')
     parser.add_argument('-a', '--auto', help="Don't prompt user to identify scans, only guess based on filename", action='store_true')
     parser.add_argument('-y', '--yes', help="Accept all changes without confirmation", action='store_true')
     parser.add_argument('-d', '--dry-run', help="Don't write any tags to image files", action='store_true')
@@ -38,34 +40,38 @@
     # Create auth object
     auth = (username, password)
 
     # Test the credentials we have
     try:
         test_credentials(server, auth)
     except:
-        print("Creds not OK")
+        cprint("Creds not OK", "red")
         raise PermissionError
-    print("Creds OK")
-
-
-    # if no args, scan current folder. consider recursive option
-    # elsif load individual frame
-    # or quit if none
+    cprint("Creds OK", "green")
 
     files = []
     if args.file:
+        # Single file supplied with -f
         files.append(args.file)
     elif args.recursive:
-        # recursive search here
-        pass
+        # Recursive from . with -r
+        purepaths = list(Path('.').rglob('*'))
+        for purepath in purepaths:
+            files.append(str(purepath))
     else:
-        files = fnfilter(os.listdir('.'), '*.[Jj][Pp][Gg]')
+        # Just search in .
+        purepaths = list(Path('.').glob('*'))
+        for purepath in purepaths:
+            files.append(str(purepath))
+
+    # Restrict file list to JPGs
+    files = fnfilter(files, '*.[Jj][Pp][Gg]')
 
     if len(files) == 0:
-        print("No files found")
+        cprint("No files found", "red")
 
     # foreach found photo:
     # read exif data, check for camerahub scan tag
     for file in files:
         print(f"Processing image {file}")
 
         # Extract exif data from file
@@ -97,51 +103,52 @@
                 #	either accept film/frame or just film then prompt frame
                 film, frame = prompt_frame(file)
 
             # Lookup Negative from API
             try:
                 negative = get_negative(film, frame, server, auth)
             except HTTPError as err:
-                print(err)
+                cprint(err, "red")
                 continue
             except:
-                print(f"Couldn't find Negative ID for {file}")
+                cprint(f"Couldn't find Negative ID for {file}", "red")
                 continue
             else:
                 print(f"{file} corresponds to Negative {negative}")
 
             # Create Scan record associated with the Negative
             try:
                 scan = create_scan(negative, file, server, auth)
             except:
-                print(f"Couldn't generate Scan ID for Negative {negative}")
+                cprint(f"Couldn't generate Scan ID for Negative {negative}", "red")
                 continue
             else:
                 print(f"Created new Scan ID {scan}")
 
         # Lookup extended Scan details in API
         try:
             apidata = get_scan(scan, server, auth)
         except:
-            print(f"Couldn't retrieve data for Scan {scan}")
+            cprint(f"Couldn't retrieve data for Scan {scan}", "red")
+            continue
         else:
             print(f"Got data for Scan {scan}")
 
         # mangle CameraHub format tags into EXIF format tags
         exifdata = api2exif(apidata)
 
         # prepare diff of tags
         diff = diff_tags(existing, exifdata)
         prettydiff = diff.pretty()
         diff = diff.to_dict()
 
         # if non-zero diff, ask user to confirm tag write
         if len(diff) > 0:
             # print diff & confirm write
-            print(prettydiff)
+            cprint(prettydiff, "yellow")
 
             if not args.dry_run:
                 if args.yes or yes_or_no("Write this metadata to the file?"):
 
                     # Apply the diff to the image
                     with pyexiv2.Image(file) as img:
                         img.modify_exif(exifdata)
```

### Comparing `camerahub_tagger-0.2.4/PKG-INFO` & `camerahub_tagger-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: camerahub-tagger
-Version: 0.2.4
+Version: 0.3.0
 Summary: EXIF tagger for CameraHub
 Home-page: https://camerahub.info/
 Keywords: EXIF,photography,CameraHub,metadata
 Author: Jonathan Gazeley
 Author-email: me@jonathangazeley.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: deepdiff (>=6.3.0,<7.0.0)
 Requires-Dist: pyexiv2 (>=2.8.1,<3.0.0)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
+Requires-Dist: termcolor (>=2.3.0,<3.0.0)
 Requires-Dist: uuid (>=1.30,<2.0)
 Project-URL: Repository, https://github.com/camerahub/tagger
 Description-Content-Type: text/markdown
 
 # CameraHub Tagger
 
 CameraHub Tagger is a companion command-line app for [CameraHub](https://camerahub.info/) to tag JPG
```

