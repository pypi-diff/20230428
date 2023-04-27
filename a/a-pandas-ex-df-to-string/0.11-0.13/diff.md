# Comparing `tmp/a_pandas_ex_df_to_string-0.11.tar.gz` & `tmp/a_pandas_ex_df_to_string-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a_pandas_ex_df_to_string-0.11.tar", last modified: Sun Oct  2 06:00:12 2022, max compression
+gzip compressed data, was "a_pandas_ex_df_to_string-0.13.tar", last modified: Thu Apr 27 23:28:38 2023, max compression
```

## Comparing `a_pandas_ex_df_to_string-0.11.tar` & `a_pandas_ex_df_to_string-0.13.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-10-02 06:00:12.318900 a_pandas_ex_df_to_string-0.11/
--rw-rw-rw-   0        0        0     1148 2022-10-02 06:00:10.000000 a_pandas_ex_df_to_string-0.11/LICENSE.rst
--rw-rw-rw-   0        0        0      185 2022-10-02 06:00:09.000000 a_pandas_ex_df_to_string-0.11/MANIFEST.in
--rw-rw-rw-   0        0        0     3320 2022-10-02 06:00:12.319876 a_pandas_ex_df_to_string-0.11/PKG-INFO
--rw-rw-rw-   0        0        0     2304 2022-10-02 05:57:33.000000 a_pandas_ex_df_to_string-0.11/README.md
-drwxrwxrwx   0        0        0        0 2022-10-02 06:00:12.316974 a_pandas_ex_df_to_string-0.11/a_pandas_ex_df_to_string/
--rw-rw-rw-   0        0        0     1069 2022-10-02 04:27:48.000000 a_pandas_ex_df_to_string-0.11/a_pandas_ex_df_to_string/LICENSE
--rw-rw-rw-   0        0        0     2304 2022-10-02 05:57:33.000000 a_pandas_ex_df_to_string-0.11/a_pandas_ex_df_to_string/README.MD
--rw-rw-rw-   0        0        0     1752 2022-10-02 05:57:33.000000 a_pandas_ex_df_to_string-0.11/a_pandas_ex_df_to_string/__init__.py
--rw-rw-rw-   0        0        0        6 2022-10-02 06:00:11.000000 a_pandas_ex_df_to_string-0.11/a_pandas_ex_df_to_string/requirements.txt
--rw-rw-rw-   0        0        0     1746 2022-10-02 06:00:11.000000 a_pandas_ex_df_to_string-0.11/a_pandas_ex_df_to_string/thirdparty.json
-drwxrwxrwx   0        0        0        0 2022-10-02 06:00:12.318900 a_pandas_ex_df_to_string-0.11/a_pandas_ex_df_to_string.egg-info/
--rw-rw-rw-   0        0        0     3320 2022-10-02 06:00:12.000000 a_pandas_ex_df_to_string-0.11/a_pandas_ex_df_to_string.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      479 2022-10-02 06:00:12.000000 a_pandas_ex_df_to_string-0.11/a_pandas_ex_df_to_string.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-02 06:00:12.000000 a_pandas_ex_df_to_string-0.11/a_pandas_ex_df_to_string.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-10-02 06:00:12.000000 a_pandas_ex_df_to_string-0.11/a_pandas_ex_df_to_string.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2022-10-02 06:00:12.000000 a_pandas_ex_df_to_string-0.11/a_pandas_ex_df_to_string.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2022-10-02 06:00:12.319876 a_pandas_ex_df_to_string-0.11/setup.cfg
--rw-rw-rw-   0        0        0     1451 2022-10-02 06:00:11.000000 a_pandas_ex_df_to_string-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 23:28:38.812415 a_pandas_ex_df_to_string-0.13/
+-rw-rw-rw-   0        0        0     1148 2023-04-27 23:28:31.000000 a_pandas_ex_df_to_string-0.13/LICENSE.rst
+-rw-rw-rw-   0        0        0      185 2023-04-27 23:28:31.000000 a_pandas_ex_df_to_string-0.13/MANIFEST.in
+-rw-rw-rw-   0        0        0     2993 2023-04-27 23:28:38.812415 a_pandas_ex_df_to_string-0.13/PKG-INFO
+-rw-rw-rw-   0        0        0     2304 2023-04-15 00:18:30.000000 a_pandas_ex_df_to_string-0.13/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 23:28:38.808707 a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string/
+-rw-rw-rw-   0        0        0     1069 2023-04-15 00:18:30.000000 a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string/LICENSE
+-rw-rw-rw-   0        0        0     2304 2023-04-15 00:18:30.000000 a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string/README.MD
+-rw-rw-rw-   0        0        0     2130 2023-04-27 23:27:05.000000 a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string/__init__.py
+-rw-rw-rw-   0        0        0        6 2023-04-27 23:28:37.000000 a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string/requirements.txt
+-rw-rw-rw-   0        0        0     1746 2023-04-27 23:28:37.000000 a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-27 23:28:38.811418 a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string.egg-info/
+-rw-rw-rw-   0        0        0     2993 2023-04-27 23:28:38.000000 a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      479 2023-04-27 23:28:38.000000 a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 23:28:38.000000 a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-27 23:28:38.000000 a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-04-27 23:28:38.000000 a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-04-27 23:28:38.813413 a_pandas_ex_df_to_string-0.13/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2023-04-27 23:28:37.000000 a_pandas_ex_df_to_string-0.13/setup.py
```

### Comparing `a_pandas_ex_df_to_string-0.11/LICENSE.rst` & `a_pandas_ex_df_to_string-0.13/LICENSE.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
  The MIT License (MIT)
- Copyright (c) 2022 Johannes Fischer
+ Copyright (c) 2023 Johannes Fischer
  
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  copies of the Software, and to permit persons to whom the Software is
  furnished to do so, subject to the following conditions:
```

### Comparing `a_pandas_ex_df_to_string-0.11/PKG-INFO` & `a_pandas_ex_df_to_string-0.13/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,77 @@
 Metadata-Version: 2.1
 Name: a_pandas_ex_df_to_string
-Version: 0.11
+Version: 0.13
 Summary: Just a function to convert everything in Pandas DataFrames / Series to string
 Home-page: https://github.com/hansalemaos/a_pandas_ex_df_to_string
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: pandas,numpy,dataframe,series
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Editors :: Text Processing
-Classifier: Topic :: Text Processing :: General
-Classifier: Topic :: Text Processing :: Indexing
-Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
+## Installation
 
-## Installation
-
-```python
-pip install a-pandas-ex-df-to-string
-```
-
-## Usage
-
-```python
-from a_pandas_ex_df_to_string import pd_add_to_string
-pd_add_to_string()
-import pandas as pd
-from random import choice
-csvtests = [
-    "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_long.csv",
-    "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_no2.csv",
-    "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_no2_long.csv",
-    "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_parameters.csv",
-    "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_pm25_long.csv",
-    "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_stations.csv",
-    "https://github.com/pandas-dev/pandas/raw/main/doc/data/baseball.csv",
-    "https://github.com/pandas-dev/pandas/raw/main/doc/data/titanic.csv",
-]
-csvfile = choice(csvtests)
-df = pd.read_csv(csvfile)
-print(df)
-print(df.dtypes)
-df2=df.ds_to_string()
-print(df2)
-print(df2.dtypes)
-
-     id                                        description   name
-0    bc                                       Black Carbon     BC
-1    co                                    Carbon Monoxide     CO
-2   no2                                   Nitrogen Dioxide    NO2
-3    o3                                              Ozone     O3
-4  pm10  Particulate matter less than 10 micrometers in...   PM10
-5  pm25  Particulate matter less than 2.5 micrometers i...  PM2.5
-6   so2                                     Sulfur Dioxide    SO2
-id             object
-description    object
-name           object
-dtype: object
-     id                                        description   name
-0    bc                                       Black Carbon     BC
-1    co                                    Carbon Monoxide     CO
-2   no2                                   Nitrogen Dioxide    NO2
-3    o3                                              Ozone     O3
-4  pm10  Particulate matter less than 10 micrometers in...   PM10
-5  pm25  Particulate matter less than 2.5 micrometers i...  PM2.5
-6   so2                                     Sulfur Dioxide    SO2
-id             string
-description    string
-name           string
-dtype: object
-
-
-
-
-```
+```python
+pip install a-pandas-ex-df-to-string
+```
+
+## Usage
+
+```python
+from a_pandas_ex_df_to_string import pd_add_to_string
+pd_add_to_string()
+import pandas as pd
+from random import choice
+csvtests = [
+    "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_long.csv",
+    "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_no2.csv",
+    "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_no2_long.csv",
+    "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_parameters.csv",
+    "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_pm25_long.csv",
+    "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_stations.csv",
+    "https://github.com/pandas-dev/pandas/raw/main/doc/data/baseball.csv",
+    "https://github.com/pandas-dev/pandas/raw/main/doc/data/titanic.csv",
+]
+csvfile = choice(csvtests)
+df = pd.read_csv(csvfile)
+print(df)
+print(df.dtypes)
+df2=df.ds_to_string()
+print(df2)
+print(df2.dtypes)
+
+     id                                        description   name
+0    bc                                       Black Carbon     BC
+1    co                                    Carbon Monoxide     CO
+2   no2                                   Nitrogen Dioxide    NO2
+3    o3                                              Ozone     O3
+4  pm10  Particulate matter less than 10 micrometers in...   PM10
+5  pm25  Particulate matter less than 2.5 micrometers i...  PM2.5
+6   so2                                     Sulfur Dioxide    SO2
+id             object
+description    object
+name           object
+dtype: object
+     id                                        description   name
+0    bc                                       Black Carbon     BC
+1    co                                    Carbon Monoxide     CO
+2   no2                                   Nitrogen Dioxide    NO2
+3    o3                                              Ozone     O3
+4  pm10  Particulate matter less than 10 micrometers in...   PM10
+5  pm25  Particulate matter less than 2.5 micrometers i...  PM2.5
+6   so2                                     Sulfur Dioxide    SO2
+id             string
+description    string
+name           string
+dtype: object
+
+
+
+
+```
```

### Comparing `a_pandas_ex_df_to_string-0.11/README.md` & `a_pandas_ex_df_to_string-0.13/README.md`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_df_to_string-0.11/a_pandas_ex_df_to_string/LICENSE` & `a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string/LICENSE`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_df_to_string-0.11/a_pandas_ex_df_to_string/README.MD` & `a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string/README.MD`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_df_to_string-0.11/a_pandas_ex_df_to_string/__init__.py` & `a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 from typing import Union
 
 import pandas as pd
 from pandas.core.base import PandasObject
 
+def _conv_col(column):
+    try:
+        return column.astype("string")
+    except Exception:
+        try:
+            return column.apply(lambda x: x.decode('utf-8', 'replace') if not isinstance(x, str) else str(x)).astype(
+            "string")
+        except Exception:
+            return column.apply(lambda x: x.decode('utf-8', 'replace')).astype(
+            "string")
 
 def ds_to_string(df: Union[pd.DataFrame, pd.Series]) -> Union[pd.Series, pd.DataFrame]:
     """
     Example:
     from random import choice
     csvtests = [
     "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_long.csv",
@@ -32,20 +42,23 @@
     if isinstance(df, pd.DataFrame):
         for col in df2.columns:
             if not df2[col].dtype == "string":
                 try:
                     df2[col] = df2[col].fillna(nastring)
                 except Exception:
                     pass
-                df2[col] = df2[col].astype("string")
+                df2[col] = _conv_col(df2[col])
     else:
         try:
             df2 = df2.fillna(nastring)
         except Exception:
             pass
-        df2 = df2.astype("string")
+        df2 = _conv_col(df2)
     df2 = df2.fillna(nastring).copy()
     return df2
 
 
 def pd_add_to_string():
     PandasObject.ds_to_string = ds_to_string
+
+
+
```

### Comparing `a_pandas_ex_df_to_string-0.11/a_pandas_ex_df_to_string/thirdparty.json` & `a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string/thirdparty.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {'0': "{'LicenseText': 'BSD 3-Clause License\\n\\nCopyright (c) 2008-2011, AQR Capital Management, "*

 * *      'LLC, Lambda Foundry, Inc. and PyData Development Team\\nAll rights reserved.\\n\\nCopyright '*

 * *      '(c) 2011-2023, Open source contributors.\\n\\nRedistribution and use in source and binary '*

 * *      'forms, with or without\\nmodification, are permitted provided that the following conditions '*

 * *      'are met:\\n\\n* Redistributions of source code must retain the above copyright notice, '*

 * *      'this\\n […]*

```diff
@@ -1,8 +1,8 @@
 [
     {
         "License": "BSD License",
-        "LicenseText": "BSD 3-Clause License\n\nCopyright (c) 2008-2011, AQR Capital Management, LLC, Lambda Foundry, Inc. and PyData Development Team\nAll rights reserved.\n\nCopyright (c) 2011-2021, Open source contributors.\n\nRedistribution and use in source and binary forms, with or without\nmodification, are permitted provided that the following conditions are met:\n\n* Redistributions of source code must retain the above copyright notice, this\n  list of conditions and the following disclaimer.\n\n* Redistributions in binary form must reproduce the above copyright notice,\n  this list of conditions and the following disclaimer in the documentation\n  and/or other materials provided with the distribution.\n\n* Neither the name of the copyright holder nor the names of its\n  contributors may be used to endorse or promote products derived from\n  this software without specific prior written permission.\n\nTHIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS \"AS IS\"\nAND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE\nIMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE\nDISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE\nFOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL\nDAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR\nSERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER\nCAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,\nOR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE\nOF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n",
+        "LicenseText": "BSD 3-Clause License\n\nCopyright (c) 2008-2011, AQR Capital Management, LLC, Lambda Foundry, Inc. and PyData Development Team\nAll rights reserved.\n\nCopyright (c) 2011-2023, Open source contributors.\n\nRedistribution and use in source and binary forms, with or without\nmodification, are permitted provided that the following conditions are met:\n\n* Redistributions of source code must retain the above copyright notice, this\n  list of conditions and the following disclaimer.\n\n* Redistributions in binary form must reproduce the above copyright notice,\n  this list of conditions and the following disclaimer in the documentation\n  and/or other materials provided with the distribution.\n\n* Neither the name of the copyright holder nor the names of its\n  contributors may be used to endorse or promote products derived from\n  this software without specific prior written permission.\n\nTHIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS \"AS IS\"\nAND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE\nIMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE\nDISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE\nFOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL\nDAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR\nSERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER\nCAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,\nOR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE\nOF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n",
         "Name": "pandas",
-        "Version": "1.4.3"
+        "Version": "2.0.0"
     }
 ]
```

### Comparing `a_pandas_ex_df_to_string-0.11/a_pandas_ex_df_to_string.egg-info/PKG-INFO` & `a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,83 +1,77 @@
 Metadata-Version: 2.1
 Name: a-pandas-ex-df-to-string
-Version: 0.11
+Version: 0.13
 Summary: Just a function to convert everything in Pandas DataFrames / Series to string
 Home-page: https://github.com/hansalemaos/a_pandas_ex_df_to_string
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: pandas,numpy,dataframe,series
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Editors :: Text Processing
-Classifier: Topic :: Text Processing :: General
-Classifier: Topic :: Text Processing :: Indexing
-Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
+## Installation
 
-## Installation
-
-```python
-pip install a-pandas-ex-df-to-string
-```
-
-## Usage
-
-```python
-from a_pandas_ex_df_to_string import pd_add_to_string
-pd_add_to_string()
-import pandas as pd
-from random import choice
-csvtests = [
-    "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_long.csv",
-    "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_no2.csv",
-    "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_no2_long.csv",
-    "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_parameters.csv",
-    "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_pm25_long.csv",
-    "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_stations.csv",
-    "https://github.com/pandas-dev/pandas/raw/main/doc/data/baseball.csv",
-    "https://github.com/pandas-dev/pandas/raw/main/doc/data/titanic.csv",
-]
-csvfile = choice(csvtests)
-df = pd.read_csv(csvfile)
-print(df)
-print(df.dtypes)
-df2=df.ds_to_string()
-print(df2)
-print(df2.dtypes)
-
-     id                                        description   name
-0    bc                                       Black Carbon     BC
-1    co                                    Carbon Monoxide     CO
-2   no2                                   Nitrogen Dioxide    NO2
-3    o3                                              Ozone     O3
-4  pm10  Particulate matter less than 10 micrometers in...   PM10
-5  pm25  Particulate matter less than 2.5 micrometers i...  PM2.5
-6   so2                                     Sulfur Dioxide    SO2
-id             object
-description    object
-name           object
-dtype: object
-     id                                        description   name
-0    bc                                       Black Carbon     BC
-1    co                                    Carbon Monoxide     CO
-2   no2                                   Nitrogen Dioxide    NO2
-3    o3                                              Ozone     O3
-4  pm10  Particulate matter less than 10 micrometers in...   PM10
-5  pm25  Particulate matter less than 2.5 micrometers i...  PM2.5
-6   so2                                     Sulfur Dioxide    SO2
-id             string
-description    string
-name           string
-dtype: object
-
-
-
-
-```
+```python
+pip install a-pandas-ex-df-to-string
+```
+
+## Usage
+
+```python
+from a_pandas_ex_df_to_string import pd_add_to_string
+pd_add_to_string()
+import pandas as pd
+from random import choice
+csvtests = [
+    "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_long.csv",
+    "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_no2.csv",
+    "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_no2_long.csv",
+    "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_parameters.csv",
+    "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_pm25_long.csv",
+    "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_stations.csv",
+    "https://github.com/pandas-dev/pandas/raw/main/doc/data/baseball.csv",
+    "https://github.com/pandas-dev/pandas/raw/main/doc/data/titanic.csv",
+]
+csvfile = choice(csvtests)
+df = pd.read_csv(csvfile)
+print(df)
+print(df.dtypes)
+df2=df.ds_to_string()
+print(df2)
+print(df2.dtypes)
+
+     id                                        description   name
+0    bc                                       Black Carbon     BC
+1    co                                    Carbon Monoxide     CO
+2   no2                                   Nitrogen Dioxide    NO2
+3    o3                                              Ozone     O3
+4  pm10  Particulate matter less than 10 micrometers in...   PM10
+5  pm25  Particulate matter less than 2.5 micrometers i...  PM2.5
+6   so2                                     Sulfur Dioxide    SO2
+id             object
+description    object
+name           object
+dtype: object
+     id                                        description   name
+0    bc                                       Black Carbon     BC
+1    co                                    Carbon Monoxide     CO
+2   no2                                   Nitrogen Dioxide    NO2
+3    o3                                              Ozone     O3
+4  pm10  Particulate matter less than 10 micrometers in...   PM10
+5  pm25  Particulate matter less than 2.5 micrometers i...  PM2.5
+6   so2                                     Sulfur Dioxide    SO2
+id             string
+description    string
+name           string
+dtype: object
+
+
+
+
+```
```

