# Comparing `tmp/imfp-1.0.5.tar.gz` & `tmp/imfp-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imfp-1.0.5.tar", max compression
+gzip compressed data, was "imfp-1.0.6.tar", max compression
```

## Comparing `imfp-1.0.5.tar` & `imfp-1.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      462 2023-04-03 14:02:24.094637 imfp-1.0.5/imfp/__init__.py
--rw-r--r--   0        0        0     1395 2023-03-28 19:45:40.534999 imfp-1.0.5/imfp/admin.py
--rw-r--r--   0        0        0    15026 2023-03-31 16:08:14.810557 imfp-1.0.5/imfp/data.py
--rw-r--r--   0        0        0     7284 2023-04-03 14:02:58.933141 imfp-1.0.5/imfp/utils.py
--rw-r--r--   0        0        0    11558 2023-03-25 14:05:34.578038 imfp-1.0.5/LICENSE
--rw-r--r--   0        0        0     1006 2023-04-03 15:47:49.735048 imfp-1.0.5/pyproject.toml
--rw-r--r--   0        0        0    20584 2023-04-03 15:35:26.310417 imfp-1.0.5/README.md
--rw-r--r--   0        0        0    20907 1970-01-01 00:00:00.000000 imfp-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      497 2023-04-28 14:16:48.149409 imfp-1.0.6/imfp/__init__.py
+-rw-r--r--   0        0        0     1440 2023-04-28 14:16:48.164413 imfp-1.0.6/imfp/admin.py
+-rw-r--r--   0        0        0    15882 2023-04-28 15:52:05.342677 imfp-1.0.6/imfp/data.py
+-rw-r--r--   0        0        0     8030 2023-04-28 15:52:05.279146 imfp-1.0.6/imfp/utils.py
+-rw-r--r--   0        0        0    11558 2023-03-25 14:05:34.578038 imfp-1.0.6/LICENSE
+-rw-r--r--   0        0        0     1006 2023-04-28 15:56:44.816716 imfp-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0    20704 2023-04-28 15:54:52.910392 imfp-1.0.6/README.md
+-rw-r--r--   0        0        0    21026 1970-01-01 00:00:00.000000 imfp-1.0.6/PKG-INFO
```

### Comparing `imfp-1.0.5/imfp/admin.py` & `imfp-1.0.6/imfp/admin.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,24 +21,31 @@
         forbidden characters.
 
     Examples:
         imf_app_name("my_custom_app_name")
     """
 
     if not isinstance(name, str) or len(name) > 255:
-        raise ValueError("Please provide a valid string as the application "
-                         "name (max length: 255 characters).")
+        raise ValueError(
+            "Please provide a valid string as the application "
+            "name (max length: 255 characters)."
+        )
 
     if name == "imfp" or name == "":
-        warn("Best practice is to choose a unique app name. Use of a default "
-             "or empty app name may result in hitting API rate limits and "
-             "being blocked by the API.", UserWarning)
+        warn(
+            "Best practice is to choose a unique app name. Use of a default "
+            "or empty app name may result in hitting API rate limits and "
+            "being blocked by the API.",
+            UserWarning,
+        )
 
     forbidden_chars = set(range(32)) | {127}
     if any(ord(c) in forbidden_chars for c in name):
-        raise ValueError("The application name contains forbidden characters. "
-                         "Please remove control characters and non-printable "
-                         "ASCII characters.")
+        raise ValueError(
+            "The application name contains forbidden characters. "
+            "Please remove control characters and non-printable "
+            "ASCII characters."
+        )
 
     environ["IMF_APP_NAME"] = name
 
     return None
```

### Comparing `imfp-1.0.5/imfp/data.py` & `imfp-1.0.6/imfp/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,29 +22,27 @@
         DataFrame containing database_id and description columns.
 
     Examples
     --------
     # Return first 6 IMF database IDs and descriptions
     databases = imf_databases()
     """
-    url = 'http://dataservices.imf.org/REST/SDMX_JSON.svc/Dataflow'
+    url = "http://dataservices.imf.org/REST/SDMX_JSON.svc/Dataflow"
     raw_dl = _download_parse(url, times)
 
     database_id = [
-        dataflow['KeyFamilyRef']['KeyFamilyID']
-        for dataflow in raw_dl['Structure']['Dataflows']['Dataflow']
+        dataflow["KeyFamilyRef"]["KeyFamilyID"]
+        for dataflow in raw_dl["Structure"]["Dataflows"]["Dataflow"]
     ]
 
     description = [
-            dataflow['Name']['#text']
-            for dataflow in raw_dl['Structure']['Dataflows']['Dataflow']
-        ]
-    database_list = DataFrame(
-            {'database_id': database_id, 'description': description}
-        )
+        dataflow["Name"]["#text"]
+        for dataflow in raw_dl["Structure"]["Dataflows"]["Dataflow"]
+    ]
+    database_list = DataFrame({"database_id": database_id, "description": description})
     return database_list
 
 
 def imf_parameters(database_id, times=2):
     """
     List input parameters and available parameter values for use in
     making API requests from a given IMF database.
@@ -70,58 +68,59 @@
     Examples
     --------
     # Fetch the full list of indicator codes and descriptions for the Primary
     # Commodity Price System database
     params = imf_parameters(database_id='PCPS')
     """
     if not database_id:
-        raise ValueError('Must supply database_id. Use imf_databases to find.')
+        raise ValueError("Must supply database_id. Use imf_databases to find.")
 
-    url = 'http://dataservices.imf.org/REST/SDMX_JSON.svc/CodeList/'
+    url = "http://dataservices.imf.org/REST/SDMX_JSON.svc/CodeList/"
     try:
         codelist = _imf_dimensions(database_id, times)
     except ValueError as e:
-        if 'There is an issue' in str(e):
-            raise ValueError(f"{e}\n\nDid you supply a valid database_id? "
-                             "Use imf_databases to find.")
+        if "There is an issue" in str(e):
+            raise ValueError(
+                f"{e}\n\nDid you supply a valid database_id? "
+                "Use imf_databases to find."
+            )
         else:
             raise ValueError(e)
 
     def fetch_parameter_data(k, url, times):
-        if codelist.loc[k, 'parameter'] == 'freq':
+        if codelist.loc[k, "parameter"] == "freq":
             return DataFrame(
-                    {
-                        "input_code": ["A", "M", "Q"],
-                        "description": ["Annual", "Monthly", "Quarterly"]
-                    }
-                )
+                {
+                    "input_code": ["A", "M", "Q"],
+                    "description": ["Annual", "Monthly", "Quarterly"],
+                }
+            )
         else:
-            raw = _download_parse(
-                    url + codelist.loc[k, 'code'], times
-                )['Structure']['CodeLists']['CodeList']['Code']
+            raw = _download_parse(url + codelist.loc[k, "code"], times)["Structure"][
+                "CodeLists"
+            ]["CodeList"]["Code"]
             if isinstance(raw, list):
                 return DataFrame(
-                            {
-                                "input_code": [code['@value'] for code in raw],
-                                "description": [code['Description']['#text']
-                                                for code in raw]
-                            }
-                        )
+                    {
+                        "input_code": [code["@value"] for code in raw],
+                        "description": [code["Description"]["#text"] for code in raw],
+                    }
+                )
             else:
                 return DataFrame(
-                        {
-                            "input_code": [raw['@value']],
-                            "description": [raw['Description']['#text']]
-                        }
-                    )
+                    {
+                        "input_code": [raw["@value"]],
+                        "description": [raw["Description"]["#text"]],
+                    }
+                )
 
     parameter_list = {
-            codelist.loc[k, 'parameter']: fetch_parameter_data(k, url, times)
-            for k in range(codelist.shape[0])
-        }
+        codelist.loc[k, "parameter"]: fetch_parameter_data(k, url, times)
+        for k in range(codelist.shape[0])
+    }
 
     return parameter_list
 
 
 def imf_parameter_defs(database_id, times=3, inputs_only=True):
     """
     Get text descriptions of input parameters used in making API
@@ -149,36 +148,43 @@
     Examples
     --------
     # Get names and text descriptions of parameters used in IMF API calls to
     # the Primary Commodity Price System database
     param_defs = imf_parameter_defs(database_id='PCPS')
     """
     if not database_id:
-        raise ValueError('Must supply database_id. Use imf_databases to find.')
+        raise ValueError("Must supply database_id. Use imf_databases to find.")
 
     try:
         parameterlist = _imf_dimensions(database_id, times, inputs_only)[
-                ['parameter', 'description']
-            ]
+            ["parameter", "description"]
+        ]
     except ValueError as e:
-        if 'There is an issue' in str(e):
-            raise ValueError(f"{e}\n\nDid you supply a valid database_id? "
-                             "Use imf_databases to find.")
+        if "There is an issue" in str(e):
+            raise ValueError(
+                f"{e}\n\nDid you supply a valid database_id? "
+                "Use imf_databases to find."
+            )
         else:
             raise ValueError(e)
 
     return parameterlist
 
 
 def imf_dataset(
-            database_id: str, parameters: dict = None, start_year: int = None,
-            end_year: int = None, return_raw: bool = False,
-            print_url: bool = False, times: int = 3,
-            include_metadata: bool = False, **kwargs
-        ):
+    database_id: str,
+    parameters: dict = None,
+    start_year: int = None,
+    end_year: int = None,
+    return_raw: bool = False,
+    print_url: bool = False,
+    times: int = 3,
+    include_metadata: bool = False,
+    **kwargs,
+):
     """
     Download a data series from the IMF.
 
     Args:
         database_id (str): Database ID for the database from which you would
                            like to request data. Can be found using
                            imf_databases().
@@ -220,109 +226,154 @@
         raise ValueError("database_id must be a string.")
 
     years = {}
     if start_year is not None:
         try:
             start_year = str(start_year)
             if start_year.isdigit() and len(start_year) == 4:
-                years['startPeriod'] = start_year
+                years["startPeriod"] = start_year
             else:
-                raise ValueError("start_year must be a four-digit number, "
-                                 "either integer or string.")
+                raise ValueError(
+                    "start_year must be a four-digit number, "
+                    "either integer or string."
+                )
         except Exception:
-            raise ValueError("start_year must be a four-digit number, either "
-                             "integer or string.")
+            raise ValueError(
+                "start_year must be a four-digit number, either " "integer or string."
+            )
     if end_year is not None:
         try:
             end_year = str(end_year)
             if end_year.isdigit() and len(end_year) == 4:
-                years['endPeriod'] = end_year
+                years["endPeriod"] = end_year
             else:
-                raise ValueError("end_year must be a four-digit number, "
-                                 "either integer or string")
+                raise ValueError(
+                    "end_year must be a four-digit number, " "either integer or string"
+                )
         except Exception:
-            raise ValueError("end_year must be a four-digit number, "
-                             "either integer or string")
+            raise ValueError(
+                "end_year must be a four-digit number, " "either integer or string"
+            )
 
     data_dimensions = imf_parameters(database_id, times)
 
     if parameters is not None:
         if kwargs:
-            warn("Parameters list argument cannot be combined with character "
-                 "vector parameters arguments. Character vector parameters "
-                 "arguments will be ignored.")
+            warn(
+                "Parameters list argument cannot be combined with character "
+                "vector parameters arguments. Character vector parameters "
+                "arguments will be ignored."
+            )
         for key in parameters:
             if key not in data_dimensions:
-                raise ValueError(f"{key} not valid parameter(s) for the "
-                                 f"{database_id} database. Use "
-                                 f"imf_parameters('{database_id}') to get "
-                                 "valid parameters.")
+                raise ValueError(
+                    f"{key} not valid parameter(s) for the "
+                    f"{database_id} database. Use "
+                    f"imf_parameters('{database_id}') to get "
+                    "valid parameters."
+                )
             invalid_keys = []
-            for x in list(parameters[key]['input_code']):
-                if x not in list(data_dimensions[key]['input_code']):
+            for x in list(parameters[key]["input_code"]):
+                if x not in list(data_dimensions[key]["input_code"]):
                     invalid_keys.append(x)
             if len(invalid_keys) > 0:
-                warn(f"{invalid_keys} not valid value(s) for {key} and will "
-                     f"be ignored. Use imf_parameters('{database_id}') to get "
-                     "valid parameters.")
-            data_dimensions[key] = data_dimensions[key].iloc[[
-                    index for index, x in enumerate(
-                        data_dimensions[key]['input_code']
-                    ) if x in list(parameters[key]['input_code'])
-                ]]
+                warn(
+                    f"{invalid_keys} not valid value(s) for {key} and will "
+                    f"be ignored. Use imf_parameters('{database_id}') to get "
+                    "valid parameters."
+                )
+            if (
+                set(parameters[key]["input_code"])
+                == set(data_dimensions[key]["input_code"])
+                or len(parameters[key]) == 0
+            ):
+                data_dimensions[key] = data_dimensions[key].iloc[0:0]
+            data_dimensions[key] = data_dimensions[key].iloc[
+                [
+                    index
+                    for index, x in enumerate(data_dimensions[key]["input_code"])
+                    if x in list(parameters[key]["input_code"])
+                ]
+            ]
+        for key in data_dimensions:
+            if key not in parameters:
+                data_dimensions[key] = data_dimensions[key].iloc[0:0]
 
     elif kwargs:
         for key in kwargs:
             if key not in data_dimensions:
-                raise ValueError(f"{key} not valid parameter(s) for the "
-                                 f"{database_id} database. Use "
-                                 f"imf_parameters('{database_id}') to get "
-                                 "valid parameters.")
+                raise ValueError(
+                    f"{key} not valid parameter(s) for the "
+                    f"{database_id} database. Use "
+                    f"imf_parameters('{database_id}') to get "
+                    "valid parameters."
+                )
             invalid_vals = []
             if not isinstance(kwargs[key], list):
                 kwargs[key] = [kwargs[key]]
             for x in kwargs[key]:
-                if x not in data_dimensions[key]['input_code'].tolist():
+                if x not in data_dimensions[key]["input_code"].tolist():
                     invalid_vals.append(x)
             if len(invalid_vals) > 0:
-                warn(f"{invalid_vals} not valid value(s) for {key} and will "
-                     f"be ignored. Use imf_parameters('{database_id}') to get "
-                     "valid parameters.")
-            data_dimensions[key] = data_dimensions[key].iloc[[
-                    index for index, x in enumerate(
-                        data_dimensions[key]['input_code']
-                    ) if x in kwargs[key]
-                ]]
+                warn(
+                    f"{invalid_vals} not valid value(s) for {key} and will "
+                    f"be ignored. Use imf_parameters('{database_id}') to get "
+                    "valid parameters."
+                )
+            if (
+                set(kwargs[key]) == set(data_dimensions[key]["input_code"].tolist())
+                or len(kwargs[key]) == 0
+            ):
+                data_dimensions[key] = data_dimensions[key].iloc[0:0]
+            data_dimensions[key] = data_dimensions[key].iloc[
+                [
+                    index
+                    for index, x in enumerate(data_dimensions[key]["input_code"])
+                    if x in kwargs[key]
+                ]
+            ]
+        for key in data_dimensions:
+            if key not in kwargs:
+                data_dimensions[key] = data_dimensions[key].iloc[0:0]
 
     else:
-        print("User supplied no filter parameters for the API request. "
-              "imf_dataset will attempt to request the entire database.")
+        print(
+            "User supplied no filter parameters for the API request. "
+            "imf_dataset will attempt to request the entire database."
+        )
         for key in data_dimensions:
             data_dimensions[key] = data_dimensions[key].iloc[0:0]
 
-    parameter_string = '.'.join(['+'.join(data_dimensions[key]['input_code'])
-                                 for key in data_dimensions])
-
-    url = (f"http://dataservices.imf.org/REST/SDMX_JSON.svc/"
-           f"CompactData/{database_id}/{parameter_string}")
+    parameter_string = ".".join(
+        ["+".join(data_dimensions[key]["input_code"]) for key in data_dimensions]
+    )
+
+    url = (
+        f"http://dataservices.imf.org/REST/SDMX_JSON.svc/"
+        f"CompactData/{database_id}/{parameter_string}"
+    )
     if years:
         url += f"?{urlencode(years)}"
 
     if print_url:
         print(url)
 
-    raw_dl = _download_parse(url, times)['CompactData']['DataSet']
+    raw_dl = _download_parse(url, times)["CompactData"]["DataSet"]
     try:
-        raw_dl = raw_dl['Series']
+        raw_dl = raw_dl["Series"]
     except Exception:
-        raise ValueError("No data found for that combination of parameters. "
-                         "Try making your request less restrictive.")
+        raise ValueError(
+            "No data found for that combination of parameters. "
+            "Try making your request less restrictive."
+        )
     if raw_dl is None:
-        raise ValueError("No data found for that combination of parameters. "
-                         "Try making your request less restrictive.")
+        raise ValueError(
+            "No data found for that combination of parameters. "
+            "Try making your request less restrictive."
+        )
 
     if return_raw:
         if include_metadata:
             metadata = _imf_metadata(url)
             return metadata, raw_dl
         else:
             return raw_dl
@@ -336,28 +387,27 @@
         return {x: d[x] for x in d if x not in keys}
 
     # Check if raw_dl is a list, and if not, convert it to one
     if not isinstance(raw_dl, list):
         raw_dl = [raw_dl]
 
     def process_data(item):
-
         # Make a data frame of dict items excluding 'Obs'
         if all(is_scalar(value) for value in without_obs(item).values()):
             param_vals = DataFrame.from_dict([without_obs(item)])
         else:
             raise ValueError("Expected item to be scalar, but it's not.")
 
         # Make a data frame from the dicts in 'Obs'
-        if not isinstance(item['Obs'], list):
-            item['Obs'] = [item['Obs']]
-        series = DataFrame.from_dict(item['Obs'])
+        if not isinstance(item["Obs"], list):
+            item["Obs"] = [item["Obs"]]
+        series = DataFrame.from_dict(item["Obs"])
 
         # Create a copy of param_vals for every row in series
-        param_vals = concat([param_vals]*len(series)).reset_index(drop=True)
+        param_vals = concat([param_vals] * len(series)).reset_index(drop=True)
 
         # Column bind param_vals to series
         output = concat([param_vals, series], axis=1)
         return output
 
     result = concat(list(map(process_data, raw_dl)))
     result.columns = result.columns.str.replace("@", "")
```

### Comparing `imfp-1.0.5/imfp/utils.py` & `imfp-1.0.6/imfp/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -73,50 +73,74 @@
     app_name = environ.get("IMF_APP_NAME")
     if app_name:
         app_name = app_name[:255]
     else:
         try:
             app_name = f'imfp/{get_distribution("imfp").version}'
         except DistributionNotFound:
-            app_name = 'imfp'
+            app_name = "imfp"
 
-    headers = {'Accept': 'application/json', 'User-Agent': app_name}
+    headers = {"Accept": "application/json", "User-Agent": app_name}
     for _ in range(times):
-        try:
-            response = _imf_get(URL, headers=headers)
-            content = response.text
-            status = response.status_code
-            json_parsed = loads(content)
-            return json_parsed
-        except JSONDecodeError:
-            if ('Rejected' in content or 'Bandwidth' in content):
+        response = _imf_get(URL, headers=headers)
+        content = response.text
+        status = response.status_code
+
+        if status != 200 or ("<" in content and ">" in content):
+            matches = re.search(">([^<>]+)<", content)  # Updated regular expression
+            inner_text = matches.group(1) if matches else content
+            output_string = re.sub(" GKey\\s*=\\s*[a-f0-9-]+", "", inner_text)
+
+            if "Rejected" in content or "Bandwidth" in content:
+                err_message = (
+                    f"API request failed. URL: '{URL}' "
+                    f"Status: '{status}', "
+                    f"Content: '{output_string}'\n\n"
+                    "API may be overwhelmed by too many "
+                    "requests. Take a break and try again."
+                )
+            elif "Service" in content:
+                err_message = (
+                    f"API request failed. URL: '{URL}' "
+                    f"Status: '{status}', "
+                    f"Content: '{output_string}'\n\n"
+                    "Your requested dataset may be too large. "
+                    "Try narrowing your request and try again."
+                )
+            elif status == 400:
+                err_message = (
+                    f"API request failed. URL: '{URL}' "
+                    f"Status: '{status}', "
+                    f"Content: '{output_string}'\n\n"
+                    "Too many parameters supplied. "
+                    "Please narrow the request and try again."
+                )
+            else:
+                err_message = (
+                    f"API request failed. URL: '{URL}' "
+                    f"Status: '{status}', "
+                    f"Content: '{output_string}'"
+                )
+
+            if _ < times - 1:
+                sleep(5 ** (_ + 1))
+            else:
+                raise ValueError(err_message)
+        else:
+            try:
+                json_parsed = loads(content)
+                return json_parsed
+            except JSONDecodeError:
                 if _ < times - 1:
                     sleep(5 ** (_ + 1))
                 else:
-                    matches = re.search("<[^>]+>(.*?)<\\/[^>]+>", content)
-                    inner_text = matches.group(1)
-                    output_string = re.sub(
-                        " GKey\\s*=\\s*[a-f0-9-]+", "", inner_text
+                    raise ValueError(
+                        f"Content from API could not be parsed as JSON. URL: '{URL}' "
+                        f"Status: '{status}', Content: '{content}'"
                     )
-                    err_message = (f"API request failed. URL: '{URL}' "
-                                   f"Status: '{status}', "
-                                   f"Content: '{output_string}'\n\n"
-                                   "API may be overwhelmed by too many "
-                                   "requests. Take a break and try again.")
-                    raise ValueError(err_message)
-            else:
-                matches = re.search("<[^>]+>(.*?)<\\/[^>]+>", content)
-                inner_text = matches.group(1)
-                output_string = re.sub(
-                    " GKey\\s*=\\s*[a-f0-9-]+", "", inner_text
-                )
-                err_message = (f"API request failed. URL: '{URL}' "
-                               f"Status: '{status}', "
-                               f"Content: '{output_string}'")
-                raise ValueError(err_message)
 
 
 def _imf_dimensions(database_id, times=3, inputs_only=True):
     """
     (Internal) Retrieve the list of codes for dimensions of an individual IMF
     database.
 
@@ -127,46 +151,46 @@
         inputs_only (bool, optional): If True, only include input parameters.
         Defaults to True.
 
     Returns:
         pandas.DataFrame: A DataFrame containing the parameter names and their
         corresponding codes and descriptions.
     """
-    URL = (f'http://dataservices.imf.org/REST/SDMX_JSON.svc/DataStructure/'
-           f'{database_id}')
+    URL = (
+        f"http://dataservices.imf.org/REST/SDMX_JSON.svc/DataStructure/"
+        f"{database_id}"
+    )
     raw_dl = _download_parse(URL, times)
 
     code = []
-    for item in raw_dl['Structure']['CodeLists']['CodeList']:
-        code.append(item['@id'])
+    for item in raw_dl["Structure"]["CodeLists"]["CodeList"]:
+        code.append(item["@id"])
     description = []
-    for item in raw_dl['Structure']['CodeLists']['CodeList']:
-        description.append(item['Name']['#text'])
-    codelist_df = DataFrame({'code': code, 'description': description})
+    for item in raw_dl["Structure"]["CodeLists"]["CodeList"]:
+        description.append(item["Name"]["#text"])
+    codelist_df = DataFrame({"code": code, "description": description})
 
     params = [
-        dim['@conceptRef'].lower()
+        dim["@conceptRef"].lower()
         for dim in (
-            raw_dl['Structure']['KeyFamilies']['KeyFamily']['Components']
-            ['Dimension']
+            raw_dl["Structure"]["KeyFamilies"]["KeyFamily"]["Components"]["Dimension"]
         )
-        ]
+    ]
     codes = [
-        dim['@codelist']
+        dim["@codelist"]
         for dim in (
-            raw_dl['Structure']['KeyFamilies']['KeyFamily']['Components']
-            ['Dimension']
+            raw_dl["Structure"]["KeyFamilies"]["KeyFamily"]["Components"]["Dimension"]
         )
-        ]
-    param_code_df = DataFrame({'parameter': params, 'code': codes})
+    ]
+    param_code_df = DataFrame({"parameter": params, "code": codes})
 
     if inputs_only:
-        result_df = param_code_df.merge(codelist_df, on='code', how='left')
+        result_df = param_code_df.merge(codelist_df, on="code", how="left")
     else:
-        result_df = param_code_df.merge(codelist_df, on='code', how='outer')
+        result_df = param_code_df.merge(codelist_df, on="code", how="outer")
 
     return result_df
 
 
 def _imf_metadata(URL, times=3):
     """
     (Internal) Access metadata for a dataset.
@@ -199,19 +223,16 @@
     output = {
         "XMLschema": raw_dl["GenericMetadata"]["@xmlns:xsd"],
         "message": raw_dl["GenericMetadata"]["@xsi:schemaLocation"],
         "language": (
             raw_dl["GenericMetadata"]["Header"]["Sender"]["Name"]["@xml:lang"]
         ),
         "timestamp": raw_dl["GenericMetadata"]["Header"]["Prepared"],
-        "custodian": (
-            raw_dl["GenericMetadata"]["Header"]["Sender"]["Name"]["#text"]
-        ),
+        "custodian": (raw_dl["GenericMetadata"]["Header"]["Sender"]["Name"]["#text"]),
         "custodian_url": (
             raw_dl["GenericMetadata"]["Header"]["Sender"]["Contact"]["URI"]
         ),
         "custodian_telephone": (
-            raw_dl["GenericMetadata"]["Header"]["Sender"]["Contact"]
-            ["Telephone"]
-        )
+            raw_dl["GenericMetadata"]["Header"]["Sender"]["Contact"]["Telephone"]
+        ),
     }
     return output
```

### Comparing `imfp-1.0.5/LICENSE` & `imfp-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `imfp-1.0.5/pyproject.toml` & `imfp-1.0.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imfp"
-version = "1.0.5"
+version = "1.0.6"
 description = "Python package for downloading economic data from the International Monetary Fund JSON RESTful API endpoint."
 authors = ["Christopher C. Smith <chriscarrollsmith@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/chriscarrollsmith/imfp"
 repository = "https://github.com/chriscarrollsmith/imfp"
 documentation = ""
```

### Comparing `imfp-1.0.5/README.md` & `imfp-1.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # imfp
 
 [![Tests](https://github.com/chriscarrollsmith/imfp/actions/workflows/actions.yml/badge.svg)](https://github.com/chriscarrollsmith/imfp/actions/workflows/actions.yml)
 [![PyPI Version](https://img.shields.io/pypi/v/imfp.svg)](https://pypi.python.org/pypi/imfp)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 `imfp`, by Christopher C. Smith, is a Python package for downloading data from the [International Monetary
 Fund's](http://data.imf.org/) [RESTful JSON
 API](http://datahelp.imf.org/knowledgebase/articles/667681-using-json-restful-web-service).
 
 ## Installation
 
@@ -587,15 +588,15 @@
 
 # Plot prices of different commodities in different colors with seaborn
 seaborn.lineplot(data=df, x='time_period', y='obs_value', hue='commodity');
 ```
 
 
     
-![png](output_32_0.png)
+![png](README_files/plot.png)
     
 
 
 
 Also note that the returned data frame has mysterious-looking codes as values in some columns.
 
 Codes in the `time_format` column are ISO 8601 duration codes. In this case, “P1Y” means “periods of 1 year.” The `unit_mult` column represents the number of zeroes you should add to the value column. For instance, if value is in millions, then the unit multiplier will be 6. If in billions, then the unit multiplier will be 9.
```

### Comparing `imfp-1.0.5/PKG-INFO` & `imfp-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imfp
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python package for downloading economic data from the International Monetary Fund JSON RESTful API endpoint.
 Home-page: https://github.com/chriscarrollsmith/imfp
 License: MIT
 Keywords: economics,finance,IMF,API
 Author: Christopher C. Smith
 Author-email: chriscarrollsmith@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -22,14 +22,15 @@
 Project-URL: Repository, https://github.com/chriscarrollsmith/imfp
 Description-Content-Type: text/markdown
 
 # imfp
 
 [![Tests](https://github.com/chriscarrollsmith/imfp/actions/workflows/actions.yml/badge.svg)](https://github.com/chriscarrollsmith/imfp/actions/workflows/actions.yml)
 [![PyPI Version](https://img.shields.io/pypi/v/imfp.svg)](https://pypi.python.org/pypi/imfp)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 `imfp`, by Christopher C. Smith, is a Python package for downloading data from the [International Monetary
 Fund's](http://data.imf.org/) [RESTful JSON
 API](http://datahelp.imf.org/knowledgebase/articles/667681-using-json-restful-web-service).
 
 ## Installation
 
@@ -611,15 +612,15 @@
 
 # Plot prices of different commodities in different colors with seaborn
 seaborn.lineplot(data=df, x='time_period', y='obs_value', hue='commodity');
 ```
 
 
     
-![png](output_32_0.png)
+![png](README_files/plot.png)
     
 
 
 
 Also note that the returned data frame has mysterious-looking codes as values in some columns.
 
 Codes in the `time_format` column are ISO 8601 duration codes. In this case, “P1Y” means “periods of 1 year.” The `unit_mult` column represents the number of zeroes you should add to the value column. For instance, if value is in millions, then the unit multiplier will be 6. If in billions, then the unit multiplier will be 9.
```

