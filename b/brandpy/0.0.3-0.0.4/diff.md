# Comparing `tmp/brandpy-0.0.3.tar.gz` & `tmp/brandpy-0.0.4.tar.gz`

## Comparing `brandpy-0.0.3.tar` & `brandpy-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 brandpy-0.0.3/src/__init__.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 brandpy-0.0.3/src/brandpy/__about__.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 brandpy-0.0.3/src/brandpy/__init__.py
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 brandpy-0.0.3/src/brandpy/bw_api_caller.py
--rw-r--r--   0        0        0    10309 2020-02-02 00:00:00.000000 brandpy-0.0.3/src/brandpy/bw_api_helper.py
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 brandpy-0.0.3/src/brandpy/bw_auth_config.py
--rw-r--r--   0        0        0   334905 2020-02-02 00:00:00.000000 brandpy-0.0.3/tests/2022_02_23_H_00_to_2022_02_23_H_01_cdondim_BWAPI_UkraineRussiaWarSO.csv.zip
--rw-r--r--   0        0        0 26474074 2020-02-02 00:00:00.000000 brandpy-0.0.3/tests/BrandwatchAPI_Lookup.ipynb
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 brandpy-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 brandpy-0.0.3/tests/bw_auth_config_test.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 brandpy-0.0.3/tests/end_to_end_test.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 brandpy-0.0.3/tests/import_test.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 brandpy-0.0.3/.gitignore
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 brandpy-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 brandpy-0.0.3/README.md
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 brandpy-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 brandpy-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 brandpy-0.0.4/src/__init__.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 brandpy-0.0.4/src/brandpy/__about__.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 brandpy-0.0.4/src/brandpy/__init__.py
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 brandpy-0.0.4/src/brandpy/bw_api_caller.py
+-rw-r--r--   0        0        0    10309 2020-02-02 00:00:00.000000 brandpy-0.0.4/src/brandpy/bw_api_helper.py
+-rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 brandpy-0.0.4/src/brandpy/bw_auth_config.py
+-rw-r--r--   0        0        0   334905 2020-02-02 00:00:00.000000 brandpy-0.0.4/tests/2022_02_23_H_00_to_2022_02_23_H_01_cdondim_BWAPI_UkraineRussiaWarSO.csv.zip
+-rw-r--r--   0        0        0 26474074 2020-02-02 00:00:00.000000 brandpy-0.0.4/tests/BrandwatchAPI_Lookup.ipynb
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 brandpy-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 brandpy-0.0.4/tests/bw_auth_config_test.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 brandpy-0.0.4/tests/end_to_end_test.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 brandpy-0.0.4/tests/gui_cache_data.json
+-rw-r--r--   0        0        0    19891 2020-02-02 00:00:00.000000 brandpy-0.0.4/tests/gui_test.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 brandpy-0.0.4/tests/import_test.py
+-rw-r--r--   0        0        0  2070445 2020-02-02 00:00:00.000000 brandpy-0.0.4/tests/test_outputs/2023_04_01_00_00_00_to_2023_04_01_22_59_59_cdondim_BWAPI_UkrianeWar_nofilters.csv.zip
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 brandpy-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 brandpy-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 brandpy-0.0.4/README.md
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 brandpy-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 brandpy-0.0.4/PKG-INFO
```

### Comparing `brandpy-0.0.3/src/brandpy/bw_api_caller.py` & `brandpy-0.0.4/src/brandpy/bw_api_caller.py`

 * *Files identical despite different names*

### Comparing `brandpy-0.0.3/src/brandpy/bw_api_helper.py` & `brandpy-0.0.4/src/brandpy/bw_api_helper.py`

 * *Files identical despite different names*

### Comparing `brandpy-0.0.3/src/brandpy/bw_auth_config.py` & `brandpy-0.0.4/src/brandpy/bw_auth_config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,86 +1,96 @@
 import errno
 import os
 import datetime
 import json
 import time
 import getpass
 import requests
-import pandas as pd
 
-import pathlib
-import typing
+
+# import pathlib
+# import typing
 
 
 class BWAuthConfig:
-    def __init__(self, in_token_file_path, in_queue_file_path=None, in_prompt_if_failed=True):
+
+    @staticmethod
+    def request_new_token(in_email, in_pwd):
+        url = f'https://api.brandwatch.com/oauth/token?username={in_email}&grant_type=api-password&client_id=brandwatch-api-client'
+        response = requests.request("POST", url, params={"password": in_pwd})
+        response.raise_for_status()
+        # if 200 != response.status_code:
+        #     print("Failed to get API token.")
+        #     print(response)
+        #     print(response.json())
+        #     raise Exception("Failed to get API token. {}".format(response.json()))
+        # else:
+        #     print("Successfully got the API token.")
+        return response.json()
+
+    @staticmethod
+    def save_token_data_to_file(in_email, in_token_file_path, in_queue_file_path, in_token_json):
+        in_token_json["e-mail"] = in_email
+        in_token_json["expire_on"] = in_token_json['expires_in'] + time.time()
+        in_token_json["queue_file"] = in_queue_file_path
+        with open(in_token_file_path, 'w', encoding="utf-8") as fout:
+            fout.write(json.dumps(in_token_json))
+            expiry_date = datetime.datetime.fromtimestamp(in_token_json["expire_on"])
+            print("Token Saved. Usable untill : {}.".format(expiry_date))
+
+    def __init__(self, in_token_file_path, in_queue_file_path=None, in_prompt_if_failed=False):
         """
         Either reads the token from existing file location or requests a new token from Brandwatch and saves the token to the given file path.
 
         :param in_token_file_path: Path to the json file that stores the access token information
         :type in_token_file_path: Union[str, os.PathLike]
         :param in_prompt_if_failed: If set True, prompts for username & password in case the token file is not found in
                 the given path and requests a token from Brandwatch and saves the newly received token in the path specified.
                 If set False, throws FileNotFoundError in case token file is not found in the given path.
         :type in_prompt_if_failed: bool
         :param in_queue_file_path: The path to the file that will work as your queue time database for rate limit management.
         :type in_queue_file_path: str
         """
         # create token file if not exist
+        self.token = None
+        self.email = None
         if in_queue_file_path is None:
-            self.queue_file_path = os.path.abspath(os.path.join(os.path.dirname(in_token_file_path), "BWQueryQueue.csv"))
+            self.queue_file_path = os.path.abspath(
+                os.path.join(os.path.dirname(in_token_file_path), "BWQueryQueue.csv"))
         else:
             self.queue_file_path = in_queue_file_path
         self.token_file_path = in_token_file_path
         if not os.path.exists(self.token_file_path):
             print("Token file does not exist.")
             if in_prompt_if_failed:
                 print("Retrieving token from Brandwatch API...")
-                response = self.__get_token()
-                self.__save_token(response)
+                response_json = self.prompt_and_get_token()
+                BWAuthConfig.save_token_data_to_file(self.email, self.token_file_path, self.queue_file_path, response_json)
             else:
                 raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), self.token_file_path)
         # read token from file
-        self.__read_token()
-
-    def __save_token(self, in_response):
-        if 200 == in_response.status_code:
-            print("Successfully got the API token.")
-            token_data = in_response.json()
-            token_data["e-mail"] = self.email
-            token_data["expire_on"] = token_data['expires_in'] + time.time()
-            token_data["queue_file"] = self.queue_file_path
-            with open(self.token_file_path, 'w', encoding="utf-8") as fout:
-                fout.write(json.dumps(token_data))
-                expdate = datetime.datetime.fromtimestamp(token_data["expire_on"])
-                print("Token Saved. Usable untill : {}.".format(expdate))
-        else:
-            print("Failed to get API token.")
-            print(in_response)
-            print(in_response.json())
-            raise Exception("Failed to get API token. {}".format(in_response.json()))
+        self.read_token_data_from_file()
 
-    def __read_token(self):
+    def read_token_data_from_file(self):
         print("Reading form Token file...")
         with open(self.token_file_path, encoding="utf-8") as fin:
-            jsdata = json.load(fin)
-        self.email = jsdata["e-mail"]
-        token = jsdata["access_token"]
-        expiry = jsdata["expire_on"]
+            user_token_data = json.load(fin)
+        self.email = user_token_data["e-mail"]
+        token = user_token_data["access_token"]
+        expiry = user_token_data["expire_on"]
         # make sure it doesn't expire for at least an hour
         print(f"Token belongs to : {self.email}")
         print("Token Expires by : {}".format(datetime.datetime.fromtimestamp(expiry)))
-        self.token = jsdata["access_token"]
-        self.queue_file_path = jsdata["queue_file"]
+        self.token = user_token_data["access_token"]
+        self.queue_file_path = user_token_data["queue_file"]
 
-    def __get_token(self):
+    def prompt_and_get_token(self):
         """
         Prompts the user to enter username and password for retrieving the token from Brandwatch API.
         :return:
         :rtype:
         """
         self.email = input("Enter your username: ")
         pwd = getpass.getpass(prompt="Enter password (program doesn't save this): ")
-        url = f'https://api.brandwatch.com/oauth/token?username={self.email}&grant_type=api-password&client_id=brandwatch-api-client'
-        response = requests.request("POST", url, params={"password": pwd})
+        response_json = BWAuthConfig.request_new_token(self.email, pwd)
         del pwd
-        return response
+        return response_json
```

### Comparing `brandpy-0.0.3/tests/2022_02_23_H_00_to_2022_02_23_H_01_cdondim_BWAPI_UkraineRussiaWarSO.csv.zip` & `brandpy-0.0.4/tests/2022_02_23_H_00_to_2022_02_23_H_01_cdondim_BWAPI_UkraineRussiaWarSO.csv.zip`

 * *Files identical despite different names*

### Comparing `brandpy-0.0.3/tests/BrandwatchAPI_Lookup.ipynb` & `brandpy-0.0.4/tests/BrandwatchAPI_Lookup.ipynb`

 * *Files identical despite different names*

### Comparing `brandpy-0.0.3/tests/end_to_end_test.py` & `brandpy-0.0.4/tests/end_to_end_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime
 import pandas as pd
-from brandpy.src import brandpy
+from BrandPy.src import brandpy
 
 TOKEN_FILE_PATH = "../../secrets/acjBWToken.json"
 QUERY_NAME = "UkrianeWar_nofilters"
 
 bw_auth_config = brandpy.BWAuthConfig(TOKEN_FILE_PATH)
 bw_api_caller = brandpy.BWAPICaller(bw_auth_config)
 bw_api_helper = brandpy.BWAPIHelper(bw_api_caller)
```

### Comparing `brandpy-0.0.3/.gitignore` & `brandpy-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `brandpy-0.0.3/LICENSE.txt` & `brandpy-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `brandpy-0.0.3/pyproject.toml` & `brandpy-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `brandpy-0.0.3/PKG-INFO` & `brandpy-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brandpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: This is a simple python wrapper for lookup calls of Brandwatch API.
 Project-URL: Documentation, https://github.com/deamonpog/BrandPy#readme
 Project-URL: Issues, https://github.com/deamonpog/BrandPy/issues
 Project-URL: Source, https://github.com/deamonpog/BrandPy
 Author-email: deamonpog <pog666@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

