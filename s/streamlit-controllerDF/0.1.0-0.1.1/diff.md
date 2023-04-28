# Comparing `tmp/streamlit_controllerDF-0.1.0.tar.gz` & `tmp/streamlit_controllerDF-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_controllerDF-0.1.0.tar", last modified: Fri Apr 28 18:07:54 2023, max compression
+gzip compressed data, was "streamlit_controllerDF-0.1.1.tar", last modified: Fri Apr 28 18:33:48 2023, max compression
```

## Comparing `streamlit_controllerDF-0.1.0.tar` & `streamlit_controllerDF-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sunjet    (1000) sunjet    (1000)        0 2023-04-28 18:07:54.211778 streamlit_controllerDF-0.1.0/
--rw-r--r--   0 sunjet    (1000) sunjet    (1000)     5201 2023-04-28 18:07:54.211778 streamlit_controllerDF-0.1.0/PKG-INFO
--rw-r--r--   0 sunjet    (1000) sunjet    (1000)     4070 2023-04-28 07:36:41.000000 streamlit_controllerDF-0.1.0/README.md
-drwxr-xr-x   0 sunjet    (1000) sunjet    (1000)        0 2023-04-28 18:07:54.208444 streamlit_controllerDF-0.1.0/SCDF/
--rw-r--r--   0 sunjet    (1000) sunjet    (1000)       16 2023-04-24 18:44:49.000000 streamlit_controllerDF-0.1.0/SCDF/UnitTests.py
--rw-r--r--   0 sunjet    (1000) sunjet    (1000)       30 2023-04-24 18:44:49.000000 streamlit_controllerDF-0.1.0/SCDF/__init__.py
--rw-r--r--   0 sunjet    (1000) sunjet    (1000)     7227 2023-04-28 06:01:41.000000 streamlit_controllerDF-0.1.0/SCDF/streamlit_controllerDF.py
--rw-r--r--   0 sunjet    (1000) sunjet    (1000)       38 2023-04-28 18:07:54.211778 streamlit_controllerDF-0.1.0/setup.cfg
--rw-r--r--   0 sunjet    (1000) sunjet    (1000)     1766 2023-04-28 18:07:38.000000 streamlit_controllerDF-0.1.0/setup.py
-drwxr-xr-x   0 sunjet    (1000) sunjet    (1000)        0 2023-04-28 18:07:54.211778 streamlit_controllerDF-0.1.0/streamlit_controllerDF.egg-info/
--rw-r--r--   0 sunjet    (1000) sunjet    (1000)     5201 2023-04-28 18:07:54.000000 streamlit_controllerDF-0.1.0/streamlit_controllerDF.egg-info/PKG-INFO
--rw-r--r--   0 sunjet    (1000) sunjet    (1000)      313 2023-04-28 18:07:54.000000 streamlit_controllerDF-0.1.0/streamlit_controllerDF.egg-info/SOURCES.txt
--rw-r--r--   0 sunjet    (1000) sunjet    (1000)        1 2023-04-28 18:07:54.000000 streamlit_controllerDF-0.1.0/streamlit_controllerDF.egg-info/dependency_links.txt
--rw-r--r--   0 sunjet    (1000) sunjet    (1000)       41 2023-04-28 18:07:54.000000 streamlit_controllerDF-0.1.0/streamlit_controllerDF.egg-info/requires.txt
--rw-r--r--   0 sunjet    (1000) sunjet    (1000)        5 2023-04-28 18:07:54.000000 streamlit_controllerDF-0.1.0/streamlit_controllerDF.egg-info/top_level.txt
+drwxr-xr-x   0 sunjet    (1000) sunjet    (1000)        0 2023-04-28 18:33:48.061835 streamlit_controllerDF-0.1.1/
+-rw-r--r--   0 sunjet    (1000) sunjet    (1000)     5211 2023-04-28 18:33:48.061835 streamlit_controllerDF-0.1.1/PKG-INFO
+-rw-r--r--   0 sunjet    (1000) sunjet    (1000)     4080 2023-04-28 18:22:22.000000 streamlit_controllerDF-0.1.1/README.md
+drwxr-xr-x   0 sunjet    (1000) sunjet    (1000)        0 2023-04-28 18:33:48.058501 streamlit_controllerDF-0.1.1/SCDF/
+-rw-r--r--   0 sunjet    (1000) sunjet    (1000)       16 2023-04-24 18:44:49.000000 streamlit_controllerDF-0.1.1/SCDF/UnitTests.py
+-rw-r--r--   0 sunjet    (1000) sunjet    (1000)       30 2023-04-24 18:44:49.000000 streamlit_controllerDF-0.1.1/SCDF/__init__.py
+-rw-r--r--   0 sunjet    (1000) sunjet    (1000)     7227 2023-04-28 06:01:41.000000 streamlit_controllerDF-0.1.1/SCDF/streamlit_controllerDF.py
+-rw-r--r--   0 sunjet    (1000) sunjet    (1000)       38 2023-04-28 18:33:48.061835 streamlit_controllerDF-0.1.1/setup.cfg
+-rw-r--r--   0 sunjet    (1000) sunjet    (1000)     1759 2023-04-28 18:32:53.000000 streamlit_controllerDF-0.1.1/setup.py
+drwxr-xr-x   0 sunjet    (1000) sunjet    (1000)        0 2023-04-28 18:33:48.061835 streamlit_controllerDF-0.1.1/streamlit_controllerDF.egg-info/
+-rw-r--r--   0 sunjet    (1000) sunjet    (1000)     5211 2023-04-28 18:33:47.000000 streamlit_controllerDF-0.1.1/streamlit_controllerDF.egg-info/PKG-INFO
+-rw-r--r--   0 sunjet    (1000) sunjet    (1000)      313 2023-04-28 18:33:47.000000 streamlit_controllerDF-0.1.1/streamlit_controllerDF.egg-info/SOURCES.txt
+-rw-r--r--   0 sunjet    (1000) sunjet    (1000)        1 2023-04-28 18:33:47.000000 streamlit_controllerDF-0.1.1/streamlit_controllerDF.egg-info/dependency_links.txt
+-rw-r--r--   0 sunjet    (1000) sunjet    (1000)       34 2023-04-28 18:33:47.000000 streamlit_controllerDF-0.1.1/streamlit_controllerDF.egg-info/requires.txt
+-rw-r--r--   0 sunjet    (1000) sunjet    (1000)        5 2023-04-28 18:33:47.000000 streamlit_controllerDF-0.1.1/streamlit_controllerDF.egg-info/top_level.txt
```

### Comparing `streamlit_controllerDF-0.1.0/PKG-INFO` & `streamlit_controllerDF-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_controllerDF
-Version: 0.1.0
+Version: 0.1.1
 Summary: A solid base for controlling your data frame, getting quick metrics, and data visualizations using streamlit, pandas, numpy and matplotlib.
 Home-page: https://github.com/joshjetson/SCDF/
 Author: Joshua Dario
 Author-email: joshuajdr@gmail.com
 License: MIT
 Keywords: Python,streamlit,dataframe,data frame,data set,visualization,automatic,widgets,automation,machine learning,quick,controller,controllerdf,controllerDF,streamlit controller,streamlit data frame,streamlit controllerDF
 Classifier: Intended Audience :: Developers
@@ -74,15 +74,15 @@
 </table>
 </tr>
 </td>
 
 ## Installation
 
 ```
-$ pip install controllerDF
+$ pip install streamlit-controllerDF
 ```
 
 ## Getting started
 
 <i>After you pip install the module</i>
 
 <ins>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streamlit_controllerDF Version: 0.1.0 Summary: A
+Metadata-Version: 2.1 Name: streamlit_controllerDF Version: 0.1.1 Summary: A
 solid base for controlling your data frame, getting quick metrics, and data
 visualizations using streamlit, pandas, numpy and matplotlib. Home-page: https:
 //github.com/joshjetson/SCDF/ Author: Joshua Dario Author-email:
 joshuajdr@gmail.com License: MIT Keywords: Python,streamlit,dataframe,data
 frame,data set,visualization,automatic,widgets,automation,machine
 learning,quick,controller,controllerdf,controllerDF,streamlit
 controller,streamlit data frame,streamlit controllerDF Classifier: Intended
@@ -28,19 +28,19 @@
 Documentation Â· Report_a_Bug Â· Demo . Request_Feature Â· Send_a_Pull_Request
 ## Controller DF []() A python library which creates a simple and easy to use
 data frame controller. Using this library, along with streamlit and minimal
 (*included*) code, anyone can spin up a web app which allows you to control,
 manipulate and display a data set quickly and easily. ## Demo
 [/pics/exgif.gif] - Quick column metrics [/pics/ex1.gif] - Rapid column filter
       [/pics/ex3.png] - Instant type based column widgets [/pics/ex2.png]
-## Installation ``` $ pip install controllerDF ``` ## Getting started After you
-pip install the module  **Batteries included method:**  Quick start > > - `Copy
-the included test_code.py` > - `Rename the file to your projects name` > ~~~ >
-$ streamlit run your_project.py > ~~~ > - `Drag and drop csv file` > - `Enjoy!`
-**Batteries excluded method:**  Module only > ~~~ > import
+## Installation ``` $ pip install streamlit-controllerDF ``` ## Getting started
+After you pip install the module  **Batteries included method:**  Quick start >
+> - `Copy the included test_code.py` > - `Rename the file to your projects
+name` > ~~~ > $ streamlit run your_project.py > ~~~ > - `Drag and drop csv
+file` > - `Enjoy!`   **Batteries excluded method:**  Module only > ~~~ > import
 streamlit_controllerDF as sc > ~~~ > - `see documentation for usage`  ##
 Documentation
 **class streamlit_controllerDF.Widgets(dataframe, omit_columns=list())** >
 Parameters: >> - dataframe: A pandas data frame >>> - *Two-dimensional, size-
 mutable, potentially heterogeneous tabular data.* >> - omit_columns: A list of
 column names to be excluded >>> - *The column names must be exact* #### Example
 ``` import streamlit_controllerDF as sc import pandas as pd mydf = pd.read_csv
```

### Comparing `streamlit_controllerDF-0.1.0/README.md` & `streamlit_controllerDF-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 </table>
 </tr>
 </td>
 
 ## Installation
 
 ```
-$ pip install controllerDF
+$ pip install streamlit-controllerDF
 ```
 
 ## Getting started
 
 <i>After you pip install the module</i>
 
 <ins>
```

#### html2text {}

```diff
@@ -12,19 +12,19 @@
 Documentation Â· Report_a_Bug Â· Demo . Request_Feature Â· Send_a_Pull_Request
 ## Controller DF []() A python library which creates a simple and easy to use
 data frame controller. Using this library, along with streamlit and minimal
 (*included*) code, anyone can spin up a web app which allows you to control,
 manipulate and display a data set quickly and easily. ## Demo
 [/pics/exgif.gif] - Quick column metrics [/pics/ex1.gif] - Rapid column filter
       [/pics/ex3.png] - Instant type based column widgets [/pics/ex2.png]
-## Installation ``` $ pip install controllerDF ``` ## Getting started After you
-pip install the module  **Batteries included method:**  Quick start > > - `Copy
-the included test_code.py` > - `Rename the file to your projects name` > ~~~ >
-$ streamlit run your_project.py > ~~~ > - `Drag and drop csv file` > - `Enjoy!`
-**Batteries excluded method:**  Module only > ~~~ > import
+## Installation ``` $ pip install streamlit-controllerDF ``` ## Getting started
+After you pip install the module  **Batteries included method:**  Quick start >
+> - `Copy the included test_code.py` > - `Rename the file to your projects
+name` > ~~~ > $ streamlit run your_project.py > ~~~ > - `Drag and drop csv
+file` > - `Enjoy!`   **Batteries excluded method:**  Module only > ~~~ > import
 streamlit_controllerDF as sc > ~~~ > - `see documentation for usage`  ##
 Documentation
 **class streamlit_controllerDF.Widgets(dataframe, omit_columns=list())** >
 Parameters: >> - dataframe: A pandas data frame >>> - *Two-dimensional, size-
 mutable, potentially heterogeneous tabular data.* >> - omit_columns: A list of
 column names to be excluded >>> - *The column names must be exact* #### Example
 ``` import streamlit_controllerDF as sc import pandas as pd mydf = pd.read_csv
```

### Comparing `streamlit_controllerDF-0.1.0/SCDF/streamlit_controllerDF.py` & `streamlit_controllerDF-0.1.1/SCDF/streamlit_controllerDF.py`

 * *Files identical despite different names*

### Comparing `streamlit_controllerDF-0.1.0/setup.py` & `streamlit_controllerDF-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="streamlit_controllerDF",
-    version="0.1.0",
+    version="0.1.1",
     description="A solid base for controlling your data frame, getting quick metrics, and data visualizations using streamlit, pandas, numpy and matplotlib.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/joshjetson/SCDF/",
     author="Joshua Dario",
     author_email="joshuajdr@gmail.com",
     license="MIT",
@@ -32,13 +32,13 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent"
     ],
     packages=find_packages(),
     include_package_data=True,
-    install_requires=["streamlit","pandas","matplotlib.pyplot","numpy"],
+    install_requires=["streamlit","pandas","matplotlib","numpy"],
     keywords=['Python','streamlit','dataframe','data frame','data set',
     'visualization','automatic','widgets','automation','machine learning',
     'quick','controller','controllerdf','controllerDF','streamlit controller','streamlit data frame',
     'streamlit controllerDF']
 )
```

### Comparing `streamlit_controllerDF-0.1.0/streamlit_controllerDF.egg-info/PKG-INFO` & `streamlit_controllerDF-0.1.1/streamlit_controllerDF.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-controllerDF
-Version: 0.1.0
+Version: 0.1.1
 Summary: A solid base for controlling your data frame, getting quick metrics, and data visualizations using streamlit, pandas, numpy and matplotlib.
 Home-page: https://github.com/joshjetson/SCDF/
 Author: Joshua Dario
 Author-email: joshuajdr@gmail.com
 License: MIT
 Keywords: Python,streamlit,dataframe,data frame,data set,visualization,automatic,widgets,automation,machine learning,quick,controller,controllerdf,controllerDF,streamlit controller,streamlit data frame,streamlit controllerDF
 Classifier: Intended Audience :: Developers
@@ -74,15 +74,15 @@
 </table>
 </tr>
 </td>
 
 ## Installation
 
 ```
-$ pip install controllerDF
+$ pip install streamlit-controllerDF
 ```
 
 ## Getting started
 
 <i>After you pip install the module</i>
 
 <ins>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streamlit-controllerDF Version: 0.1.0 Summary: A
+Metadata-Version: 2.1 Name: streamlit-controllerDF Version: 0.1.1 Summary: A
 solid base for controlling your data frame, getting quick metrics, and data
 visualizations using streamlit, pandas, numpy and matplotlib. Home-page: https:
 //github.com/joshjetson/SCDF/ Author: Joshua Dario Author-email:
 joshuajdr@gmail.com License: MIT Keywords: Python,streamlit,dataframe,data
 frame,data set,visualization,automatic,widgets,automation,machine
 learning,quick,controller,controllerdf,controllerDF,streamlit
 controller,streamlit data frame,streamlit controllerDF Classifier: Intended
@@ -28,19 +28,19 @@
 Documentation Â· Report_a_Bug Â· Demo . Request_Feature Â· Send_a_Pull_Request
 ## Controller DF []() A python library which creates a simple and easy to use
 data frame controller. Using this library, along with streamlit and minimal
 (*included*) code, anyone can spin up a web app which allows you to control,
 manipulate and display a data set quickly and easily. ## Demo
 [/pics/exgif.gif] - Quick column metrics [/pics/ex1.gif] - Rapid column filter
       [/pics/ex3.png] - Instant type based column widgets [/pics/ex2.png]
-## Installation ``` $ pip install controllerDF ``` ## Getting started After you
-pip install the module  **Batteries included method:**  Quick start > > - `Copy
-the included test_code.py` > - `Rename the file to your projects name` > ~~~ >
-$ streamlit run your_project.py > ~~~ > - `Drag and drop csv file` > - `Enjoy!`
-**Batteries excluded method:**  Module only > ~~~ > import
+## Installation ``` $ pip install streamlit-controllerDF ``` ## Getting started
+After you pip install the module  **Batteries included method:**  Quick start >
+> - `Copy the included test_code.py` > - `Rename the file to your projects
+name` > ~~~ > $ streamlit run your_project.py > ~~~ > - `Drag and drop csv
+file` > - `Enjoy!`   **Batteries excluded method:**  Module only > ~~~ > import
 streamlit_controllerDF as sc > ~~~ > - `see documentation for usage`  ##
 Documentation
 **class streamlit_controllerDF.Widgets(dataframe, omit_columns=list())** >
 Parameters: >> - dataframe: A pandas data frame >>> - *Two-dimensional, size-
 mutable, potentially heterogeneous tabular data.* >> - omit_columns: A list of
 column names to be excluded >>> - *The column names must be exact* #### Example
 ``` import streamlit_controllerDF as sc import pandas as pd mydf = pd.read_csv
```

