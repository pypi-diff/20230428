# Comparing `tmp/imfp-1.0.6.tar.gz` & `tmp/imfp-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imfp-1.0.6.tar", max compression
+gzip compressed data, was "imfp-1.0.7.tar", max compression
```

## Comparing `imfp-1.0.6.tar` & `imfp-1.0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      497 2023-04-28 14:16:48.149409 imfp-1.0.6/imfp/__init__.py
--rw-r--r--   0        0        0     1440 2023-04-28 14:16:48.164413 imfp-1.0.6/imfp/admin.py
--rw-r--r--   0        0        0    15882 2023-04-28 15:52:05.342677 imfp-1.0.6/imfp/data.py
--rw-r--r--   0        0        0     8030 2023-04-28 15:52:05.279146 imfp-1.0.6/imfp/utils.py
--rw-r--r--   0        0        0    11558 2023-03-25 14:05:34.578038 imfp-1.0.6/LICENSE
--rw-r--r--   0        0        0     1006 2023-04-28 15:56:44.816716 imfp-1.0.6/pyproject.toml
--rw-r--r--   0        0        0    20704 2023-04-28 15:54:52.910392 imfp-1.0.6/README.md
--rw-r--r--   0        0        0    21026 1970-01-01 00:00:00.000000 imfp-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      497 2023-04-28 14:16:48.149409 imfp-1.0.7/imfp/__init__.py
+-rw-r--r--   0        0        0     1440 2023-04-28 14:16:48.164413 imfp-1.0.7/imfp/admin.py
+-rw-r--r--   0        0        0    16124 2023-04-28 18:38:01.551682 imfp-1.0.7/imfp/data.py
+-rw-r--r--   0        0        0     7988 2023-04-28 18:16:02.883520 imfp-1.0.7/imfp/utils.py
+-rw-r--r--   0        0        0    11558 2023-03-25 14:05:34.578038 imfp-1.0.7/LICENSE
+-rw-r--r--   0        0        0     1025 2023-04-28 18:51:48.980513 imfp-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0    20704 2023-04-28 15:54:52.910392 imfp-1.0.7/README.md
+-rw-r--r--   0        0        0    21026 1970-01-01 00:00:00.000000 imfp-1.0.7/PKG-INFO
```

### Comparing `imfp-1.0.6/imfp/admin.py` & `imfp-1.0.7/imfp/admin.py`

 * *Files identical despite different names*

### Comparing `imfp-1.0.6/imfp/data.py` & `imfp-1.0.7/imfp/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -394,16 +394,22 @@
         # Make a data frame of dict items excluding 'Obs'
         if all(is_scalar(value) for value in without_obs(item).values()):
             param_vals = DataFrame.from_dict([without_obs(item)])
         else:
             raise ValueError("Expected item to be scalar, but it's not.")
 
         # Make a data frame from the dicts in 'Obs'
-        if not isinstance(item["Obs"], list):
-            item["Obs"] = [item["Obs"]]
+        try:
+            if not isinstance(item["Obs"], list):
+                item["Obs"] = [item["Obs"]]
+        except:
+            raise ValueError(
+                "No observations found for that combination of parameters. "
+                "start_year and end_year may be outside the dataset's range."
+            )
         series = DataFrame.from_dict(item["Obs"])
 
         # Create a copy of param_vals for every row in series
         param_vals = concat([param_vals] * len(series)).reset_index(drop=True)
 
         # Column bind param_vals to series
         output = concat([param_vals, series], axis=1)
```

### Comparing `imfp-1.0.6/imfp/utils.py` & `imfp-1.0.7/imfp/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,16 +82,16 @@
     headers = {"Accept": "application/json", "User-Agent": app_name}
     for _ in range(times):
         response = _imf_get(URL, headers=headers)
         content = response.text
         status = response.status_code
 
         if status != 200 or ("<" in content and ">" in content):
-            matches = re.search(">([^<>]+)<", content)  # Updated regular expression
-            inner_text = matches.group(1) if matches else content
+            matches = re.search("<[^>]+>(.*?)<\\/[^>]+>", content)
+            inner_text = matches.group(1)
             output_string = re.sub(" GKey\\s*=\\s*[a-f0-9-]+", "", inner_text)
 
             if "Rejected" in content or "Bandwidth" in content:
                 err_message = (
                     f"API request failed. URL: '{URL}' "
                     f"Status: '{status}', "
                     f"Content: '{output_string}'\n\n"
```

### Comparing `imfp-1.0.6/LICENSE` & `imfp-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `imfp-1.0.6/pyproject.toml` & `imfp-1.0.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imfp"
-version = "1.0.6"
+version = "1.0.7"
 description = "Python package for downloading economic data from the International Monetary Fund JSON RESTful API endpoint."
 authors = ["Christopher C. Smith <chriscarrollsmith@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/chriscarrollsmith/imfp"
 repository = "https://github.com/chriscarrollsmith/imfp"
 documentation = ""
@@ -24,11 +24,12 @@
 pandas = "^1.5.3"
 requests = "^2.28.2"
 
 [tool.poetry.group.dev.dependencies]
 responses = "^0.23.1"
 pytest = "^7.2.2"
 pytest-runner = "^6.0.0"
+black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `imfp-1.0.6/README.md` & `imfp-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `imfp-1.0.6/PKG-INFO` & `imfp-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imfp
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python package for downloading economic data from the International Monetary Fund JSON RESTful API endpoint.
 Home-page: https://github.com/chriscarrollsmith/imfp
 License: MIT
 Keywords: economics,finance,IMF,API
 Author: Christopher C. Smith
 Author-email: chriscarrollsmith@gmail.com
 Requires-Python: >=3.8,<4.0
```

