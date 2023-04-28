# Comparing `tmp/d2c_mp_sales_forecaster-0.0.1.tar.gz` & `tmp/d2c_mp_sales_forecaster-0.0.2.tar.gz`

## Comparing `d2c_mp_sales_forecaster-0.0.1.tar` & `d2c_mp_sales_forecaster-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,33 @@
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.1/environment.yml
--rw-r--r--   0        0        0    12007 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.1/requirements.txt
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.1/src/d2c_mp_sales_forecaster/D2CMPForecaster.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.1/src/d2c_mp_sales_forecaster/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.1/src/d2c_mp_sales_forecaster/config.toml
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.1/src/d2c_mp_sales_forecaster/config/d2c_forecast_app_style.mplstyle
--rw-r--r--   0        0        0    10021 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.1/src/d2c_mp_sales_forecaster/pages/1_Load_Data.py
--rw-r--r--   0        0        0    17294 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.1/src/d2c_mp_sales_forecaster/pages/2_Product_Selection.py
--rw-r--r--   0        0        0    15125 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.1/src/d2c_mp_sales_forecaster/pages/3_Tune_and_Train.py
--rw-r--r--   0        0        0     8224 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.1/src/d2c_mp_sales_forecaster/pages/4_Forecast_Product.py
--rw-r--r--   0        0        0     6972 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.1/src/d2c_mp_sales_forecaster/pages/5_Distribute_Size_Forecast.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.1/src/d2c_mp_sales_forecaster/pages/__init__.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.1/tests/test_1_Load_Data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.1/tests/test_2_Product_Selection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.1/tests/test_3_Tune_and_Train.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.1/tests/test_4_Forecast_Product.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.1/tests/test_5_Distribute_Size_forecast.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.1/tests/test_D2CMPForecaster.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.1/.gitignore
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.1/LICENSE
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.1/README.md
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/.dockerignore
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/Dockerfile
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/compose.yaml
+-rw-r--r--   0        0        0     8310 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/environment.yml
+-rw-r--r--   0        0        0     8938 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/.vscode/launch.json
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/.vscode/tasks.json
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/D2CMPForecaster.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/config.toml
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/config/db_ddl.sql
+-rw-r--r--   0        0        0    10682 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/pages/_1_Load_Data.py
+-rw-r--r--   0        0        0    17946 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/pages/_2_Product_Selection.py
+-rw-r--r--   0        0        0    16519 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/pages/_3_Tune_and_Train.py
+-rw-r--r--   0        0        0    12702 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/pages/_4_Forecast_Product.py
+-rw-r--r--   0        0        0    10073 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/pages/_5_Distribute_Size_Forecast.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/pages/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/utils/__init__.py
+-rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/utils/db_manager.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/tests/test_1_Load_Data.py
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/tests/test_2_Product_Selection.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/tests/test_3_Tune_and_Train.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/tests/test_4_Forecast_Product.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/tests/test_5_Distribute_Size_forecast.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/tests/test_D2CMPForecaster.py
+-rwxr-xr-x   0        0        0    41114 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/tests/select_product/lag_data.csv
+-rwxr-xr-x   0        0        0    31393 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/tests/select_product/master_data_enc.csv
+-rwxr-xr-x   0        0        0   918353 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/tests/select_product/sales_data.csv
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/README.md
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 d2c_mp_sales_forecaster-0.0.2/PKG-INFO
```

### Comparing `d2c_mp_sales_forecaster-0.0.1/src/d2c_mp_sales_forecaster/D2CMPForecaster.py` & `d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/D2CMPForecaster.py`

 * *Files identical despite different names*

### Comparing `d2c_mp_sales_forecaster-0.0.1/src/d2c_mp_sales_forecaster/pages/1_Load_Data.py` & `d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/pages/_1_Load_Data.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#Imports
+# Imports
 import streamlit as st
 import itertools
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 from datetime import date
 from datetime import timedelta
@@ -12,220 +12,250 @@
 
 st.header("Step 1: Upload datasets for forcasting.")
 
 
 def upload_sales_size_data(uploaded_file) -> tuple:
     """
     Upload, format, and cleanse product sales data by size and day.
-    
+
     Args:
         uploaded_file: A CSV file containing product sales data by size and day.
-        
+
     Returns:
         A tuple of two DataFrames:
             1. all_sales_data: Aggregated product sales data.
             2. all_sales_size_data: Product sales data with proper typing and formatting.
-    """    
+    """
     with st.spinner("Uploading file..."):
-        all_sales_size_data = pd.read_csv(uploaded_file, 
-                                header = 0,
-                                names = ['product','size','ds','y'],
-                                dtype={'product':'object', 'size':'object','date':'object', 'y':'object'},
-                                parse_dates=['ds'],
-                                infer_datetime_format=True
-                                )
-        all_sales_size_data = all_sales_size_data[all_sales_size_data['size']  != 'Result']
-        all_sales_size_data['y'] = all_sales_size_data['y'].str.replace(',','')
+        all_sales_size_data = pd.read_csv(uploaded_file,
+                                          header=0,
+                                          names=['product', 'size', 'ds', 'y'],
+                                          dtype={
+                                              'product': 'object', 'size': 'object', 'date': 'object', 'y': 'object'},
+                                          parse_dates=['ds'],
+                                          infer_datetime_format=True
+                                          )
+        all_sales_size_data = all_sales_size_data[all_sales_size_data['size'] != 'Result']
+        all_sales_size_data['y'] = all_sales_size_data['y'].str.replace(
+            ',', '')
         all_sales_size_data['y'] = all_sales_size_data['y'].astype('int64')
         if 'all_sales_size_data' not in st.session_state:
-            st.session_state['all_sales_size_data'] = all_sales_size_data 
+            st.session_state['all_sales_size_data'] = all_sales_size_data
         else:
             st.session_state['all_sales_size_data'] = all_sales_size_data
-        #Group and save a version of the dataframe aggregated to the product level
-        all_sales_data = all_sales_size_data.groupby(['product','ds']).agg({'y':'sum'})
+        # Group and save a version of the dataframe aggregated to the product level
+        all_sales_data = all_sales_size_data.groupby(
+            ['product', 'ds']).agg({'y': 'sum'})
         all_sales_data.reset_index(inplace=True)
         if 'all_sales_data' not in st.session_state:
             st.session_state['all_sales_data'] = all_sales_data
         else:
             st.session_state['all_sales_data'] = all_sales_data
     st.success("File upload complete!")
     return all_sales_data, all_sales_size_data
-    
+
 
 def upload_master_data(uploaded_md_file) -> tuple:
     """
     Upload product master data.
-    
+
     Args:
         uploaded_md_file: A CSV file containing product master data. The first column should be the unique product key.
-        
+
     Returns:
         A tuple of two DataFrames:
             1. master_data: The uploaded product master data.
             2. master_data_enc: The encoded product master data.
     """
     with st.spinner("Uploading file..."):
         master_data = pd.read_csv(uploaded_md_file, index_col=0)
         master_data.index.rename('product', inplace=True)
         master_data.index = master_data.index.map(str)
-        #Econde the master data --> break this into a separate optional function later.
+        # Econde the master data --> break this into a separate optional function later.
         master_data_enc = pd.get_dummies(master_data)
         master_data_enc = master_data_enc.fillna(0)
         if 'master_data' not in st.session_state:
-            st.session_state['master_data'] = master_data 
+            st.session_state['master_data'] = master_data
         else:
             st.session_state['master_data'] = master_data
         if 'master_data_enc' not in st.session_state:
             st.session_state['master_data_enc'] = master_data_enc
         else:
             st.session_state['master_data_enc'] = master_data_enc
     st.success("File upload complete!")
     return master_data, master_data_enc
 
 
 def upload_events_data(uploaded_ev_file) -> pd.DataFrame:
     """
     Upload holidays and events data.
-    
+
     Args:
         uploaded_ev_file: A CSV file containing holidays and events data.
-        
+
     Returns:
         events_df: A DataFrame containing the uploaded holidays and events data.
     """
     with st.spinner("Uploading file..."):
-        events_df = pd.read_csv(uploaded_ev_file,                                    
-                                        header = 0,
-                                        names = ['event', 'ds', 'lower_window', 'upper_window'],
-                                        dtype={'event':'object', 'ds':'object','lower_window':'int64', 'upper_window':'int64'},
-                                        parse_dates=['ds'],
-                                        infer_datetime_format=True)
+        events_df = pd.read_csv(uploaded_ev_file,
+                                header=0,
+                                names=['event', 'ds',
+                                       'lower_window', 'upper_window'],
+                                dtype={'event': 'object', 'ds': 'object',
+                                       'lower_window': 'int64', 'upper_window': 'int64'},
+                                parse_dates=['ds'],
+                                infer_datetime_format=True)
         if 'events_df' not in st.session_state:
             st.session_state['events_df'] = events_df
         else:
             st.session_state['events_df'] = events_df
     st.success("File upload complete!")
     return events_df
 
+
 def upload_lag_data(uploaded_lag_file) -> tuple:
     """
     Upload and preprocess lag regressors data.
-    
+
     Args:
         uploaded_lag_file: A CSV file containing lag regressors data.
-        
+
     Returns:
         lag_data: A DataFrame containing the preprocessed lag regressors data.
-    """    
+    """
     with st.spinner("Uploading file..."):
-        lag_data = pd.read_csv(uploaded_lag_file, 
-                                header = 0,
-                                parse_dates=['ds'],
-                                infer_datetime_format=True
-                                )
-        #Set datetime interval to day and ensure timeseries complete by day
+        lag_data = pd.read_csv(uploaded_lag_file,
+                               header=0,
+                               parse_dates=['ds'],
+                               infer_datetime_format=True
+                               )
+        # Set datetime interval to day and ensure timeseries complete by day
         lag_data['ds'] = pd.to_datetime(lag_data['ds'])
         lag_data = lag_data.set_index('ds')
         lag_data = lag_data.resample('1D').ffill().reset_index()
-        #Remove commas and cast all other columns as float64 data type
+        # Remove commas and cast all other columns as float64 data type
         for col in lag_data.columns:
             if col != 'ds':
                 if lag_data[col].dtype == 'object':
                     lag_data[col] = lag_data[col].str.replace(',', '')
                 lag_data[col] = lag_data[col].astype('float64')
         if 'lag_data' not in st.session_state:
-            st.session_state['lag_data'] = lag_data 
+            st.session_state['lag_data'] = lag_data
         else:
             st.session_state['lag_data'] = lag_data
     st.success("File upload complete!")
     return lag_data
 
+
 def upload_future_data(uploaded_future_file) -> tuple:
     """
     Upload and preprocess future regressors data.
-    
+
     Args:
         uploaded_future_file: A CSV file containing future regressors data.
-        
+
     Returns:
         future_data: A DataFrame containing the preprocessed future regressors data.
-    """    
+    """
     with st.spinner("Uploading file..."):
-        future_data = pd.read_csv(uploaded_future_file, 
-                                header = 0,
-                                parse_dates=['ds'],
-                                infer_datetime_format=True
-                                )
-        #set datetime interval to day and ensure timeseries completeness
+        future_data = pd.read_csv(uploaded_future_file,
+                                  header=0,
+                                  parse_dates=['ds'],
+                                  infer_datetime_format=True
+                                  )
+        # set datetime interval to day and ensure timeseries completeness
         future_data['ds'] = pd.to_datetime(future_data['ds'])
         future_data = future_data.set_index('ds')
         future_data = future_data.resample('1D').ffill().reset_index()
         # Remove commas and cast all other columns as float64 data type
         for col in future_data.columns:
             if col != 'ds':
                 if future_data[col].dtype == 'object':
                     future_data[col] = future_data[col].str.replace(',', '')
                 future_data[col] = future_data[col].astype('float64')
         if 'future_data' not in st.session_state:
-            st.session_state['future_data'] = future_data 
+            st.session_state['future_data'] = future_data
         else:
             st.session_state['future_data'] = future_data
     st.success("File upload complete!")
     return future_data
 
 
-#File Uploaders
+@st.cache_resource
+def convert_df(df):
+    """
+    Convert a DataFrame to a CSV string and encode it as utf-8 bytes.
+
+    Args:
+        df: A DataFrame to be converted.
+
+    Returns:
+        A CSV string of the DataFrame encoded as utf-8 bytes.
+    """
+    return df.to_csv().encode('utf-8')
+
+
+# File Uploaders
 st.subheader("a. Upload historical sales by product and size.")
-uploaded_file = st.file_uploader("Select Sales History by Product and Size for Upload")
+uploaded_file = st.file_uploader(
+    "Select Sales History by Product and Size for Upload")
 st.write(uploaded_file)
 if uploaded_file is not None:
     all_sales_data, lag_data = upload_sales_size_data(uploaded_file)
 if 'all_sales_data' in st.session_state:
     st.write("You currently have uploaded the following data:")
     cola, colb = st.columns(2)
     with cola:
         st.subheader('Product Sales History')
         st.write(st.session_state['all_sales_data'])
     with colb:
         st.subheader('Product-Size Sales History')
         st.write(st.session_state['all_sales_size_data'])
 
-st.subheader("b. Upload product attributes for augmenting historicals with similar product sales.")
+st.subheader(
+    "b. Upload product attributes for augmenting historicals with similar product sales.")
 uploaded_md_file = st.file_uploader("Select product master data to upload.")
 st.write(uploaded_md_file)
 if uploaded_md_file is not None:
     master_data, master_data_enc = upload_master_data(uploaded_md_file)
 if 'master_data' in st.session_state:
     st.write("You currently have uploaded the following data:")
     st.subheader('Product Master Data')
     st.write(st.session_state['master_data'])
+    st.download_button(label="Download Encoded Master Data",
+                       data=convert_df(st.session_state['master_data_enc']),
+                       file_name='master_data_enc.csv',
+                       mime='text/csv'
+                       )
 
 st.subheader("c. Upload holidays and special events.  (Optional)")
-uploaded_ev_file = st.file_uploader("Select holidays and events file to upload.")
+uploaded_ev_file = st.file_uploader(
+    "Select holidays and events file to upload.")
 st.write(uploaded_ev_file)
 if uploaded_ev_file is not None:
     events_df = upload_events_data(uploaded_ev_file)
 if 'events_df' in st.session_state:
     st.write("You currently have uploaded the following data:")
     st.subheader('Events')
     st.write(st.session_state['events_df'])
 
 if 'all_sales_data' in st.session_state and 'all_sales_size_data' in st.session_state:
-    st.subheader("d. Upload lag regressors.")
-    uploaded_lag_file = st.file_uploader("Select lag regressor data to upload.")
+    st.subheader("d. Upload lag regressors.  (Optional)")
+    uploaded_lag_file = st.file_uploader(
+        "Select lag regressor data to upload.")
     st.write(uploaded_lag_file)
     if uploaded_lag_file is not None:
         lag_data = upload_lag_data(uploaded_lag_file)
     if 'lag_data' in st.session_state:
         st.write("You currently have uploaded the following data:")
         st.subheader('Lag Regressor Data')
         st.write(st.session_state['lag_data'])
 
-    #st.subheader("e. Upload future regressors.")
-    #uploaded_future_file = st.file_uploader("Select future regressor data to upload.")
-    #st.write(uploaded_future_file)
-    #if uploaded_future_file is not None:
+    # st.subheader("e. Upload future regressors.")
+    # uploaded_future_file = st.file_uploader("Select future regressor data to upload.")
+    # st.write(uploaded_future_file)
+    # if uploaded_future_file is not None:
     #    future_data = upload_future_data(uploaded_future_file)
-    #if 'lag_data' in st.session_state:
+    # if 'lag_data' in st.session_state:
     #    st.write("You currently have uploaded the following data:")
     #    st.subheader('Future Regressor Data')
     #    st.write(st.session_state['future_data'])
```

### Comparing `d2c_mp_sales_forecaster-0.0.1/src/d2c_mp_sales_forecaster/pages/2_Product_Selection.py` & `d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/pages/_2_Product_Selection.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,182 +4,203 @@
 from sklearn.metrics.pairwise import cosine_similarity
 from datetime import date
 from datetime import timedelta
 
 # Page config
 st.set_page_config(page_title="D2C, Dropship, Marketplace Forecasting")
 
+
 def get_len_history(all_sales_data: pd.DataFrame) -> pd.DataFrame:
     """
     Calculate the length of sales history for each product.
-    
+
     Args:
         all_sales_data: A DataFrame containing aggregated product sales data.
-        
+
     Returns:
         sales_minmax_dates: A DataFrame containing the length of sales history for each product.
     """
-    sorted_sales = all_sales_data.sort_values(by=['product','ds'], ascending = True)
-    sales_minmax_dates = sorted_sales.groupby('product').agg({'ds':['min','max'], 'y':'sum'})
-    sales_minmax_dates['len_hist'] = (sales_minmax_dates.loc[:,('ds','max')] - sales_minmax_dates.loc[:,('ds','min')]) / np.timedelta64(1, 'D')
+    sorted_sales = all_sales_data.sort_values(
+        by=['product', 'ds'], ascending=True)
+    sales_minmax_dates = sorted_sales.groupby(
+        'product').agg({'ds': ['min', 'max'], 'y': 'sum'})
+    sales_minmax_dates['len_hist'] = (sales_minmax_dates.loc[:, (
+        'ds', 'max')] - sales_minmax_dates.loc[:, ('ds', 'min')]) / np.timedelta64(1, 'D')
     return sales_minmax_dates
 
+
 @st.cache_data
 def get_similarities(master_data_enc: pd.DataFrame) -> pd.DataFrame:
     """
     Calculate cosine similarity between products based on encoded master data.
-    
+
     Args:
         master_data_enc: A DataFrame containing encoded product master data.
-        
+
     Returns:
         similarity_df: A DataFrame containing the cosine similarity scores between products.
     """
     similarity = cosine_similarity(master_data_enc)
-    similarity_df = pd.DataFrame(similarity, 
-                             index=master_data_enc.index.values,
-                             columns=master_data_enc.index.values)
+    similarity_df = pd.DataFrame(similarity,
+                                 index=master_data_enc.index.values,
+                                 columns=master_data_enc.index.values)
     return similarity_df
 
+
 def check_history_needed(sales_minmax_dates: pd.DataFrame, product_fcst: str, min_req_hist: float = 366.0):
     """
     Check for the minimum history needed for forecasting a specific product.
-    
+
     Args:
         sales_minmax_dates: A DataFrame containing the length of sales history for each product.
         product_fcst: The product to be forecasted.
         min_req_hist: The minimum required history for forecasting (default: 366 days).
-        
+
     Returns:
         min_append_hist_req: The minimum required history to append.
         cutoff_date: The cutoff date for adding history.
     """
-    #lookup length of history for that product
-    len_avail_hist = sales_minmax_dates.loc[sales_minmax_dates.index == product_fcst]['len_hist'].values[0]
-    #difference with minimum required history to identify days gap aka minimum required length of history to append
+    # lookup length of history for that product
+    len_avail_hist = sales_minmax_dates.loc[sales_minmax_dates.index ==
+                                            product_fcst]['len_hist'].values[0]
+    # difference with minimum required history to identify days gap aka minimum required length of history to append
     min_append_hist_req = int(min_req_hist - len_avail_hist)
-    #identify the cutoff to add the length of history to
-    cutoff_date = sales_minmax_dates.loc[sales_minmax_dates.index == product_fcst][('ds','min')] - timedelta(min_append_hist_req)
+    # identify the cutoff to add the length of history to
+    cutoff_date = sales_minmax_dates.loc[sales_minmax_dates.index == product_fcst][(
+        'ds', 'min')] - timedelta(min_append_hist_req)
     return min_append_hist_req, cutoff_date.values[0]
 
 
 def match_product(similarity_df: pd.DataFrame, sales_minmax_dates: pd.DataFrame, product_fcst: str, cutoff_date: np.datetime64,  top_n: int = 1):
     """
     Match a product to similar products based on a similarity DataFrame.
-    
+
     Args:
         similarity_df: A DataFrame containing the cosine similarity scores between products.
         sales_minmax_dates: A DataFrame containing the length of sales history for each product.
         product_fcst: The product to be forecasted.
         cutoff_date: The cutoff date for adding history.
         top_n: The number of top similar products desired (default: 1).
-        
+
     Returns:
         matched: A list of matched similar products.
     """
     # product list of only products that meet minimum length requirements in addition to available history
-    product_list = sales_minmax_dates.loc[sales_minmax_dates[('ds','min')] < cutoff_date].index.values
+    product_list = sales_minmax_dates.loc[sales_minmax_dates[(
+        'ds', 'min')] < cutoff_date].index.values
     # slice similarity dataframe by the product being forecasted on row-index, and the product list on the column-index
-    product_sim = similarity_df.loc[similarity_df.index == product_fcst, product_list].values[0]
+    product_sim = similarity_df.loc[similarity_df.index ==
+                                    product_fcst, product_list].values[0]
     # get products sorted by similarity
     sorted_products = np.argsort(product_sim)[::-1]
     # get matched product id
     matched = product_list[sorted_products[1:top_n+1]]
     return matched
 
+
 def fill_missing(sales_history: pd.DataFrame) -> pd.DataFrame:
     """
     Fill missing values in a sales history DataFrame.
-    
+
     Args:
         sales_history: A DataFrame containing sales history data.
-        
+
     Returns:
         sales_history: A DataFrame with missing values filled.
     """
     sales_history = sales_history.sort_values(by='ds')
     sales_history.index = pd.to_datetime(sales_history['ds'])
     sales_history.drop(columns=['ds'], inplace=True)
     sales_history = sales_history.asfreq('D')
-    #fill all non quantities with forward-fill
+    # fill all non quantities with forward-fill
     for col in sales_history.columns:
-                if col != 'y':
-                    sales_history[col].fillna(method='ffill',inplace=True) 
+        if col != 'y':
+            sales_history[col].fillna(method='ffill', inplace=True)
     # assume a 0 means no sale for that day
-    sales_history['y'].fillna(0, inplace=True) 
+    sales_history['y'].fillna(0, inplace=True)
     sales_history.reset_index(inplace=True)
     return sales_history
 
+
 def merge_regressors(sales_data, lag_data, future_data=None) -> pd.DataFrame:
     """
     Merge sales data with lag and future regressor data.
-    
+
     Args:
         sales_data: A DataFrame containing sales data.
         lag_data: A DataFrame containing lag regressor data.
         future_data: A DataFrame containing future regressor data (optional).
-        
+
     Returns:
         all_sales_data_lag: A DataFrame with sales data merged with lag and future regressor data.
     """
     all_sales_data_lag = pd.merge(sales_data, lag_data, on='ds', how='inner')
     return all_sales_data_lag
 
+
 def append_history(all_sales_data: pd.DataFrame, matched: list, product_fcst: str, lag_data: pd.DataFrame = None) -> pd.DataFrame:
     """
     Append sales history for a product with the history of a similar product.
-    
+
     Args:
         all_sales_data: A DataFrame containing aggregated product sales data.
         matched: A list of matched similar products.
         product_fcst: The product to be forecasted.
         lag_data: A DataFrame containing lag regressor data (optional).
-        
+
     Returns:
         A tuple of two DataFrames:
             1. appended_history: The appended sales history.
             2. appended_history_product: The appended sales history with the product column.
     """
-    product_history = all_sales_data.loc[all_sales_data['product'] == product_fcst]
+    product_history = all_sales_data.loc[all_sales_data['product']
+                                         == product_fcst]
     min_date = product_history['ds'].min()
     extra_history = all_sales_data.loc[all_sales_data['product'] == matched[0]]
     extra_history = extra_history.loc[extra_history['ds'] < min_date]
-    appended_history_product = fill_missing(pd.concat([product_history, extra_history]))
+    appended_history_product = fill_missing(
+        pd.concat([product_history, extra_history]))
     if lag_data is not None:
-            appended_history_product = merge_regressors(appended_history_product, lag_data)
-    appended_history = appended_history_product.drop(columns='product').copy(deep=True)
+        appended_history_product = merge_regressors(
+            appended_history_product, lag_data)
+    appended_history = appended_history_product.drop(
+        columns='product').copy(deep=True)
     return appended_history, appended_history_product
 
 
 def prepare_non_appended(sales_history: pd.DataFrame, forecast_product: str, all_sales_regressors: pd.DataFrame = None):
     """
     Prepare sales history for a product without appending additional history from similar products.
-    
+
     Args:
         sales_history: A DataFrame containing sales history data.
         forecast_product: The product to be forecasted.
         all_sales_regressors: A DataFrame containing sales data with additional regressors (optional).
-        
+
     Returns:
         A tuple of two DataFrames:
             1. forecast_df: The prepared sales history without the product column.
             2. forecast_df_product: The prepared sales history with the product column.
     """
     if all_sales_regressors is None:
-        forecast_df_product = fill_missing(sales_history.loc[sales_history['product'] == forecast_product])
-        forecast_df = forecast_df_product.loc[:,['ds','y']].copy(deep=True)
+        forecast_df_product = fill_missing(
+            sales_history.loc[sales_history['product'] == forecast_product])
+        forecast_df = forecast_df_product.loc[:, ['ds', 'y']].copy(deep=True)
     else:
-        forecast_df_product = fill_missing(all_sales_regressors.loc[all_sales_regressors['product'] == forecast_product])
-        forecast_df = forecast_df_product.drop(columns='product').copy(deep=True)
+        forecast_df_product = fill_missing(
+            all_sales_regressors.loc[all_sales_regressors['product'] == forecast_product])
+        forecast_df = forecast_df_product.drop(
+            columns='product').copy(deep=True)
     return forecast_df, forecast_df_product
 
+
 def clear_state(key: str):
     """
     Clear the session state for a specified key.
-    
+
     Args:
         key: The key to be cleared from the session state.
     """
     if key in st.session_state:
         st.session_state[key] = None
 
 
@@ -192,55 +213,62 @@
 if 'matched' not in st.session_state:
     st.session_state['matched'] = None
 
 if 'forecast_product' not in st.session_state:
     st.session_state['forecast_product'] = None
 
 
-#Title
+# Title
 st.title("D2C, Dropship, Marketplace Forecasting")
 
-#Select the product that will be used for forecasting.
+# Select the product that will be used for forecasting.
 st.header("2. Select product for forecasting.")
 
 if 'master_data' not in st.session_state:
     st.write("Please go to Load Data and upload a product attribute file to be able to choose a product for forecasting.")
 else:
     if st.session_state['forecast_product'] is not None:
-       st.session_state['forecast_product'] = forecast_product = st.table(st.session_state['master_data']).selectbox('Select a product ID', 
-                                                                              st.session_state['master_data'].index, 
-                                                                              index=st.session_state['master_data'].index.get_loc(st.session_state['forecast_product']),
-                                                                              on_change=clear_state('matched'))
+        st.session_state['forecast_product'] = forecast_product = st.table(st.session_state['master_data']).selectbox('Select a product ID',
+                                                                                                                      st.session_state[
+                                                                                                                          'master_data'].index,
+                                                                                                                      index=st.session_state['master_data'].index.get_loc(
+                                                                                                                          st.session_state['forecast_product']),
+                                                                                                                      on_change=clear_state('matched'))
     else:
-        st.session_state['forecast_product'] = forecast_product = st.table(st.session_state['master_data']).selectbox('Select a product ID', 
-                                                                               st.session_state['master_data'].index, 
-                                                                               index=0,
-                                                                               on_change=clear_state('matched'))
+        st.session_state['forecast_product'] = forecast_product = st.table(st.session_state['master_data']).selectbox('Select a product ID',
+                                                                                                                      st.session_state[
+                                                                                                                          'master_data'].index,
+                                                                                                                      index=0,
+                                                                                                                      on_change=clear_state('matched'))
     cola, colb = st.columns(2)
     with cola:
         st.write("You selected:", st.session_state['forecast_product'])
-        st.write(st.session_state['master_data'].loc[st.session_state['forecast_product']])
+        st.write(
+            st.session_state['master_data'].loc[st.session_state['forecast_product']])
     with colb:
         if 'all_sales_data' in st.session_state:
             if 'lag_data' in st.session_state:
                 st.session_state['all_sales_regressors'] = pd.DataFrame
-                st.session_state['all_sales_regressors'] = merge_regressors(st.session_state['all_sales_data'], st.session_state['lag_data'])
-                st.write("Sales history:") 
-                st.write(st.session_state['all_sales_regressors'].loc[st.session_state['all_sales_regressors']['product'] == st.session_state['forecast_product'],:]
+                st.session_state['all_sales_regressors'] = merge_regressors(
+                    st.session_state['all_sales_data'], st.session_state['lag_data'])
+                st.write("Sales history:")
+                st.write(st.session_state['all_sales_regressors'].loc[st.session_state['all_sales_regressors']['product'] == st.session_state['forecast_product'], :]
                          .sort_values(by='ds'))
             else:
-                st.write("Sales history:") 
-                st.write(st.session_state['all_sales_data'].loc[st.session_state['all_sales_data']['product'] == st.session_state['forecast_product'],:])
+                st.write("Sales history:")
+                st.write(st.session_state['all_sales_data'].loc[st.session_state['all_sales_data']
+                         ['product'] == st.session_state['forecast_product'], :])
         else:
-            st.write("Please load sales history data for the product ", st.session_state['forecast_product'], " before proceeding further.")
+            st.write("Please load sales history data for the product ",
+                     st.session_state['forecast_product'], " before proceeding further.")
 
-            
 
-#Section for identifying similar products
-st.subheader("Optional - Match most similar product for sufficient historical data for forecasting. ")
+# Section for identifying similar products
+st.subheader(
+    "Optional - Match most similar product for sufficient historical data for forecasting. ")
 
 
 st.write("It is necessary to have at minimum one year of sales history for the NeuralPropeht algorithm to pick up on seasonal affects effectively.  For products with not enough sales history, or for new products, we will use Cosine Similarity on the encoded product master to identify a product that is most-similar, and append that to the desired product history to be able to come up with a better forecast. \
         For reference on the meaning of Cosine Similarity: https://www.geeksforgeeks.org/cosine-similarity/")
 st.write("If you loaded additional regressors on the previous page, these will be automatically inner-joined to the forecast product dataset.")
 
 # Select if we want to use cosine similarity to extend product history?
@@ -248,67 +276,74 @@
     "Identify most-similar product to extend historical data for forecasting?", help="Uses cosine similarity to match most-similar product and appends similar product sales to forecast product sales data to be at least one year in length. "
 )
 
 
 colc, cold = st.columns(2)
 if use_similarity:
     if 'all_sales_data' in st.session_state:
-        #This sets up base values for calculating and appending history based on the uploaded data
-        sales_minmax_dates = get_len_history(st.session_state['all_sales_data'])
-        top_n = 1 #Only find one most-similar product to matach and append history
+        # This sets up base values for calculating and appending history based on the uploaded data
+        sales_minmax_dates = get_len_history(
+            st.session_state['all_sales_data'])
+        top_n = 1  # Only find one most-similar product to matach and append history
         similarity_df = get_similarities(st.session_state['master_data_enc'])
-        min_append_hist_req, cutoff_date = check_history_needed(sales_minmax_dates, st.session_state['forecast_product'])
+        min_append_hist_req, cutoff_date = check_history_needed(
+            sales_minmax_dates, st.session_state['forecast_product'])
 
-        #Determine if history appendage is required, and if so, append history of the most-similar identified product
+        # Determine if history appendage is required, and if so, append history of the most-similar identified product
         if min_append_hist_req > 0:
-            st.session_state['matched'] = match_product(similarity_df, sales_minmax_dates, st.session_state['forecast_product'], cutoff_date, top_n)
+            st.session_state['matched'] = match_product(
+                similarity_df, sales_minmax_dates, st.session_state['forecast_product'], cutoff_date, top_n)
             if 'lag_data' in st.session_state:
-                st.session_state['forecast_df'], st.session_state['forecast_df_product']  = append_history(st.session_state['all_sales_data'], 
-                                                                                                           st.session_state['matched'], 
-                                                                                                           st.session_state['forecast_product'],
-                                                                                                           st.session_state['lag_data'])
+                st.session_state['forecast_df'], st.session_state['forecast_df_product'] = append_history(st.session_state['all_sales_data'],
+                                                                                                          st.session_state['matched'],
+                                                                                                          st.session_state[
+                    'forecast_product'],
+                    st.session_state['lag_data'])
             else:
-                st.session_state['forecast_df'], st.session_state['forecast_df_product']  = append_history(st.session_state['all_sales_data'], 
-                                                                                                           st.session_state['matched'], 
-                                                                                                           st.session_state['forecast_product']
-                                                                                                           )        
+                st.session_state['forecast_df'], st.session_state['forecast_df_product'] = append_history(st.session_state['all_sales_data'],
+                                                                                                          st.session_state['matched'],
+                                                                                                          st.session_state[
+                    'forecast_product']
+                )
         else:
             if 'all_sales_regressors' in st.session_state:
-                st.session_state['forecast_df'], st.session_state['forecast_df_product']  = prepare_non_appended(st.session_state['all_sales_data'], 
-                                                                                                         st.session_state['forecast_product'],
-                                                                                                         st.session_state['all_sales_regressors'])
+                st.session_state['forecast_df'], st.session_state['forecast_df_product'] = prepare_non_appended(st.session_state['all_sales_data'],
+                                                                                                                st.session_state[
+                    'forecast_product'],
+                    st.session_state['all_sales_regressors'])
             else:
-                st.session_state['forecast_df'], st.session_state['forecast_df_product']  = prepare_non_appended(st.session_state['all_sales_data'], 
-                                                                                                         st.session_state['forecast_product'])
-        
+                st.session_state['forecast_df'], st.session_state['forecast_df_product'] = prepare_non_appended(st.session_state['all_sales_data'],
+                                                                                                                st.session_state['forecast_product'])
+
         if 'forecast_df_product' in st.session_state:
             with colc:
                 st.write("This is the data-set that will be used for forecasting:")
                 st.write(st.session_state['forecast_df_product'])
             with cold:
                 if st.session_state['matched'] is not None:
-                    st.write('Identified most-similar product based on uploaded attributes using cosine similarity:')
-                    st.write(st.session_state['master_data'].loc[st.session_state['matched']])
+                    st.write(
+                        'Identified most-similar product based on uploaded attributes using cosine similarity:')
+                    st.write(
+                        st.session_state['master_data'].loc[st.session_state['matched']])
                 else:
-                    st.write('Sufficient historical data identified, there is no need to append similar product history.')
+                    st.write(
+                        'Sufficient historical data identified, there is no need to append similar product history.')
     else:
         st.write("Please upload sales history from the Load Data page to proceed.")
 
 else:
-    #If the user does not select to append historicals, set up the forecast dataframe with just the chosen product
-    
+    # If the user does not select to append historicals, set up the forecast dataframe with just the chosen product
+
     if 'all_sales_data' in st.session_state:
         if 'all_sales_regressors' in st.session_state:
-            st.session_state['forecast_df'], st.session_state['forecast_df_product']  = prepare_non_appended(st.session_state['all_sales_data'], 
-                                                                                                         st.session_state['forecast_product'],
-                                                                                                         st.session_state['all_sales_regressors'])
+            st.session_state['forecast_df'], st.session_state['forecast_df_product'] = prepare_non_appended(st.session_state['all_sales_data'],
+                                                                                                            st.session_state[
+                'forecast_product'],
+                st.session_state['all_sales_regressors'])
         else:
-            st.session_state['forecast_df'], st.session_state['forecast_df_product']  = prepare_non_appended(st.session_state['all_sales_data'], 
-                                                                                                         st.session_state['forecast_product'])
+            st.session_state['forecast_df'], st.session_state['forecast_df_product'] = prepare_non_appended(st.session_state['all_sales_data'],
+                                                                                                            st.session_state['forecast_product'])
         with colc:
             st.write("This is the data-set that will be used for forecasting:")
             st.write(st.session_state['forecast_df_product'])
     else:
         st.write("Please upload sales history from the Load Data page to proceed.")
-
-
-
```

### Comparing `d2c_mp_sales_forecaster-0.0.1/src/d2c_mp_sales_forecaster/pages/3_Tune_and_Train.py` & `d2c_mp_sales_forecaster-0.0.2/src/d2c_mp_sales_forecaster/pages/_3_Tune_and_Train.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,84 +2,89 @@
 import itertools
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 from datetime import date
 from datetime import timedelta
 from neuralprophet import NeuralProphet, set_log_level, set_random_seed, utils
-from sklearn.metrics import mean_squared_error 
+from sklearn.metrics import mean_squared_error
 from sklearn.metrics import mean_absolute_error
 from sklearn.metrics import mean_absolute_percentage_error
 
 # Page config
 st.set_page_config(page_title="D2C, Dropship, Marketplace Forecasting")
 
+
 @st.cache_resource(show_spinner=False)
-def fit_complete(params: dict, df: pd.DataFrame, events_df: pd.DataFrame = None) -> NeuralProphet:
+def fit_complete(params: dict, df: pd.DataFrame, events_df: pd.DataFrame = None, fit_spinner_text="Fitting the model for product") -> NeuralProphet:
     """
     Fit a NeuralProphet model to the complete dataset using the selected params or the best parameters obtained from cross-validation.
-    
+
     Args:
         params: A dictionary containing the best hyperparameters.
         df: A DataFrame containing the dataset to be fit.
         events_df: A DataFrame containing events data (optional).
-        
+
     Returns:
         A fitted NeuralProphet model.
     """
-    #Fit the whole training set with best params
+    # Fit the whole training set with best params
     with st.spinner(fit_spinner_text):
         m = NeuralProphet(**params)
         for col in df.columns:
-                if col != 'y' and col != 'ds':
-                    m = m.add_lagged_regressor(names=col)
+            if col != 'y' and col != 'ds':
+                m = m.add_lagged_regressor(names=col)
         if events_df is not None:
             m.add_events(['Cyber Week'], mode='additive')
             data_ev = m.create_df_with_events(df, events_df)
             fit_metrics = m.fit(df=data_ev, freq="D")
         else:
             fit_metrics = m.fit(df=df, freq="D")
         st.write("Metrics from model fit:", fit_metrics)
         st.session_state['fit_flag'] = True
     st.success("Model fit complete!", icon="✅")
     return m
 
+
 @st.cache_resource(show_spinner=False)
 def cross_val_tune(params: dict, df: pd.DataFrame, forecast_product: str, events_df: pd.DataFrame = None, horizon: int = 30) -> tuple:
     """
     Perform hyperparameter tuning using cross-validation for a given forecast product.
-    
+
     Args:
         params: A dictionary containing the parameters to be tuned.
         df: A DataFrame containing the dataset.
         forecast_product: The product to be forecasted.
         events_df: A DataFrame containing events data (optional).
         horizon: The forecast horizon in days (default: 30).
-        
+
     Returns:
         A tuple containing:
             1. best_metrics: A DataFrame containing the best test metrics from cross-validation.
             2. best_params: A dictionary containing the best hyperparameters.
     """
     METRICS = ["MAE", "RMSE"]
     fold_pct = horizon/len(df)
 
-    st.write("Applying five-fold cross-validation to the forecast model for " + forecast_product)
+    st.write(
+        "Applying five-fold cross-validation to the forecast model for " + forecast_product)
 
     param_grid = params
 
     # Generate all combinations of parameters
-    all_params = [dict(zip(param_grid.keys(), v)) for v in itertools.product(*param_grid.values())]
-    cv_test_loss = [] 
+    all_params = [dict(zip(param_grid.keys(), v))
+                  for v in itertools.product(*param_grid.values())]
+    cv_test_loss = []
     test_metrics_list = []
     best_metrics = []
 
     # Use cross validation to evaluate all parameters
     for i, params in enumerate(all_params):
-        folds = NeuralProphet(**params).crossvalidation_split_df(df, freq="D", k=5, fold_pct=fold_pct, fold_overlap_pct=0)
+        folds = NeuralProphet(**params).crossvalidation_split_df(df,
+                                                                 freq="D", k=5, fold_pct=fold_pct, fold_overlap_pct=0)
         metrics_train = pd.DataFrame(columns=METRICS)
         metrics_test = pd.DataFrame(columns=METRICS)
         for df_train, df_test in folds:
             m = NeuralProphet(**params)
             for col in df.columns:
                 if col != 'y' and col != 'ds':
                     m = m.add_lagged_regressor(names=col)
@@ -90,41 +95,43 @@
                 train = m.fit(df=df_train_ev, freq="D")
                 test = m.test(df=df_test_ev)
             else:
                 train = m.fit(df=df_train, freq="D")
                 test = m.test(df=df_test)
             metrics_train = metrics_train.append(train.iloc[-1])
             metrics_test = metrics_test.append(test.iloc[-1])
-        cv_test_loss.append(metrics_test['MSELoss'].mean()) 
+        cv_test_loss.append(metrics_test['MSELoss'].mean())
         test_metrics_list.append(metrics_test)
     best_params = all_params[np.argmin(cv_test_loss)]
     best_metrics = test_metrics_list[np.argmin(cv_test_loss)]
 
     st.write("Best model test metrics from cross-validation:")
     st.write(best_metrics)
     st.write("Best model test metrics mean across 5 folds: ")
     st.write(best_metrics.mean())
     st.write("Resulting hyperparmeters from cross-validation:")
     st.write(best_params)
 
     return best_metrics, best_params
 
+
 def is_events():
     """
     Check if events data is available in the session state.
 
     Returns:
         The events data if available, otherwise None.
     """
     if 'events_df' in st.session_state:
         return st.session_state['events_df']
     else:
         return None
 
-#Setup key session_state variables needed for cross-page use
+# Setup key session_state variables needed for cross-page use
+
 
 if 'hyperparam_options' not in st.session_state:
     st.session_state['hyperparam_options'] = {}
 
 if 'selected_options' not in st.session_state:
     st.session_state['selected_options'] = {}
 
@@ -145,156 +152,182 @@
 
 normalize_list = ['soft', 'minmax', 'soft1', 'standardize', 'off']
 
 # Start section for formatting the page
 
 st.header("3. Select, tune, and train the forecasting model.")
 
-if st.session_state['forecast_df'].empty:  
-    st.write("Please first load sales data and select a product to forecast to be able to setup and train a forecasting model.")
-else:
-
-    tab_auto, tab_select = st.tabs(["Automatic Hyperparameter Tuning", "Manual Hyperparameter Selection"])
-
-    #Re-used variables across tabs
-    fit_spinner_text = "Fitting the model for product " + st.session_state['forecast_product'] + " with selected hyperparameters..."
-
-    with tab_select:
-
-        st.subheader("Select hyperparamters to tune a forecasting model for the selected product: ", st.session_state['forecast_product'])
-
-        with st.form("param_grid_form"):
-            # Add a title to the form
-            st.write("Select options for param_grid")
-            
-            # Define the options for each parameter
-            seasonality_mode_options = st.selectbox('Select seasonality_mode', ['additive', 'multiplicative'])
-            loss_func_options = st.selectbox('Select loss_func', ['MSE', 'MAE'])
-            n_changepoints = 10
-            n_changepoints_options = st.slider('Select n_changepoints', min_value=1, max_value=20, value=n_changepoints)
-            changepoints_range = 10.0
-            changepoints_range_options = st.slider('Select changepoints_range', min_value=0.01, max_value=20.0, value=changepoints_range)
-            normalize_options = st.selectbox('Select normalization method', normalize_list)
-            n_lags_options = st.slider('Select n_lags', min_value=7, max_value=90, value=30)
-            n_forecasts_options = st.slider('Select n_forecasts', min_value=7, max_value=90, value=30)
-            num_hidden_layers_options = st.selectbox('Select num_hidden_layers',[0,1,2])
-            
-            # Add a submit button to the form
-            submitted = st.form_submit_button("Submit")
-            
-            # If the user submitted the form, print the selected options
-            if submitted:
-                # Create a dictionary to store the selected options
-                st.session_state['selected_options'] = {
-                    'seasonality_mode':seasonality_mode_options,
-                    'loss_func':loss_func_options,
-                    'n_changepoints':n_changepoints_options,
-                    'changepoints_range':changepoints_range_options,
-                    'normalize':normalize_options,
-                    'num_hidden_layers':num_hidden_layers_options,
-                    'n_lags':n_lags_options,
-                    'n_forecasts':n_forecasts_options
-                }
-
-                #Also store iterable version of params dict for common cross-validation function use.
-                selections_to_lists = lambda x: {k: [v] for k, v in x.items()}
-                st.session_state['iter_selections'] = selections_to_lists(st.session_state['selected_options'])
-
-            st.write("Selected options:")
-            st.write(st.session_state['selected_options'])
-
-
-        if st.session_state['selected_options']:
-
-            with st.expander("Cross-Validation"):   
-                if st.button("Cross-Validate"):
-                    with st.spinner("Performing cross-validation... (Please do not refresh or close this tab while running to complete this task.)"):
-                        st.session_state['metrics_test'], st.session_state['selected_options'] = cross_val_tune(
-                            params=st.session_state['iter_selections'], 
-                            df=st.session_state['forecast_df'], 
-                            forecast_product=st.session_state['forecast_product'],
-                            events_df=is_events(),
-                            horizon = int(st.session_state['selected_options']['n_forecasts'])) 
-                    st.success("Cross-validation complete!", icon="✅")
-                else:
-                    st.write("Push \"Cross-Validate\" to perform 5-fold backtesting cross-validation with your selected hyperparameters.")
-
+if 'forecast_df' in st.session_state:
+    if st.session_state['forecast_df'].empty:
+        st.write("Please first load sales data and select a product to forecast to be able to setup and train a forecasting model.")
+    else:
 
-            with st.expander("Fit Model to Complete Dataset"):
-                st.write("Current Identified Best Parameters: ")
-                st.write(st.session_state['selected_options'])
-                if st.button("Fit Model", key='fit_select'):
-                        st.session_state["m"] = fit_complete(params=st.session_state['selected_options'], 
-                                         df=st.session_state['forecast_df'],
-                                         events_df=is_events())
-                else:
-                    st.write("Fit the model with the full data-set for the selected product.  This is required for moving to forecast prediction.")
+        tab_auto, tab_select = st.tabs(
+            ["Automatic Hyperparameter Tuning", "Manual Hyperparameter Selection"])
 
+        # Re-used variables across tabs
+        fit_spinner_text = "Fitting the model for product " + \
+            st.session_state['forecast_product'] + \
+            " with selected hyperparameters..."
 
+        with tab_select:
 
-        with tab_auto:
-            
-            st.subheader("Select options and ranges for an automated grid-search to find the best hyperparameters: ", st.session_state['forecast_product'])
+            st.subheader("Select hyperparamters to tune a forecasting model for the selected product: ",
+                         st.session_state['forecast_product'])
 
-            with st.form("hyper_grid_form"):
+            with st.form("param_grid_form"):
                 # Add a title to the form
-                st.write("Select options for hyperparameter search.")
-                
+                st.write("Select options for param_grid")
+
                 # Define the options for each parameter
-                seasonality_mode_options = st.multiselect('Select seasonality_mode', ['additive', 'multiplicative'], default='additive')
-                loss_func_options = st.multiselect('Select loss_func', ['MSE', 'MAE'], default='MSE')
-                n_cp_min, n_cp_max = st.slider('Select n_changepoints (min=1/max=20)', min_value=1, max_value=20, value=(5,10))
-                n_cp_steps = st.number_input('Select step-size for n_changepoints (min=1/max=10)', min_value=1, max_value=10, value=5)
-                cp_range_min, cp_range_max = st.slider('Select changepoints_range (min=0.01/max=20.0)', min_value=0.01, max_value=20.0, value=(1.0, 10.0))
-                cp_range_steps = st.number_input('Select step-size for n_changepoints (min=0.01/max=10.0)', min_value=0.01, max_value=10.0, value=9.0)
-                normalize_options = st.multiselect('Select normalization method', normalize_list, default='soft')
-                n_lags_options = st.slider('Select n_lags', min_value=7, max_value=90, value=30)
-                n_forecasts_options = st.slider('Select n_forecasts', min_value=7, max_value=90, value=30)
-                num_hidden_layers_options = st.multiselect('Select num_hidden_layers',[0,1,2], default=0)
-                
+                seasonality_mode_options = st.selectbox(
+                    'Select seasonality_mode', ['additive', 'multiplicative'])
+                loss_func_options = st.selectbox(
+                    'Select loss_func', ['MSE', 'MAE'])
+                n_changepoints = 10
+                n_changepoints_options = st.slider(
+                    'Select n_changepoints', min_value=1, max_value=20, value=n_changepoints)
+                changepoints_range = 10.0
+                changepoints_range_options = st.slider(
+                    'Select changepoints_range', min_value=0.01, max_value=20.0, value=changepoints_range)
+                normalize_options = st.selectbox(
+                    'Select normalization method', normalize_list)
+                n_lags_options = st.slider(
+                    'Select n_lags', min_value=7, max_value=90, value=30)
+                n_forecasts_options = st.slider(
+                    'Select n_forecasts', min_value=7, max_value=90, value=30)
+                num_hidden_layers_options = st.selectbox(
+                    'Select num_hidden_layers', [0, 1, 2])
+
                 # Add a submit button to the form
                 submitted = st.form_submit_button("Submit")
-                
+
                 # If the user submitted the form, print the selected options
                 if submitted:
                     # Create a dictionary to store the selected options
-                    st.session_state['hyperparam_options'] = {
-                        'seasonality_mode':seasonality_mode_options,
-                        'loss_func':loss_func_options,
-                        'n_changepoints':np.arange(n_cp_min, n_cp_max+1, n_cp_steps).tolist(),
-                        'changepoints_range':np.arange(cp_range_min, cp_range_max+0.01, cp_range_steps).tolist(),
+                    st.session_state['selected_options'] = {
+                        'seasonality_mode': seasonality_mode_options,
+                        'loss_func': loss_func_options,
+                        'n_changepoints': n_changepoints_options,
+                        'changepoints_range': changepoints_range_options,
                         'normalize': normalize_options,
-                        'num_hidden_layers':num_hidden_layers_options,
-                        'n_lags':[n_lags_options],
-                        'n_forecasts':[n_forecasts_options]
-                        
+                        'num_hidden_layers': num_hidden_layers_options,
+                        'n_lags': n_lags_options,
+                        'n_forecasts': n_forecasts_options
                     }
 
+                    # Also store iterable version of params dict for common cross-validation function use.
+                    def selections_to_lists(x): return {
+                        k: [v] for k, v in x.items()}
+                    st.session_state['iter_selections'] = selections_to_lists(
+                        st.session_state['selected_options'])
+
                 st.write("Selected options:")
-                st.write(st.session_state['hyperparam_options'])
+                st.write(st.session_state['selected_options'])
 
+            if st.session_state['selected_options']:
 
-            if st.session_state['hyperparam_options']:
-                with st.expander("Hyperparameter Search"):   
-                    if st.button("Grid Search"):
-                        with st.spinner("Performing grid search for best hyperparameters... (Please do not refresh or close this tab while running to complete this task.)"):
-                            st.session_state['metrics_test'], st.session_state['best_params'] = cross_val_tune(
-                                params=st.session_state['hyperparam_options'], 
+                with st.expander("Cross-Validation"):
+                    if st.button("Cross-Validate"):
+                        with st.spinner("Performing cross-validation... (Please do not refresh or close this tab while running to complete this task.)"):
+                            st.session_state['metrics_test'], st.session_state['selected_options'] = cross_val_tune(
+                                params=st.session_state['iter_selections'],
                                 df=st.session_state['forecast_df'],
                                 forecast_product=st.session_state['forecast_product'],
                                 events_df=is_events(),
-                                horizon = int(st.session_state['hyperparam_options']['n_forecasts'][0]))  
+                                horizon=int(st.session_state['selected_options']['n_forecasts']))
                         st.success("Cross-validation complete!", icon="✅")
                     else:
-                        st.write("Push \"Cross-Validate\" to Grid Search for best hyperparameters using 5-fold backtesting cross-validation.")
+                        st.write(
+                            "Push \"Cross-Validate\" to perform 5-fold backtesting cross-validation with your selected hyperparameters.")
 
-            if st.session_state['best_params']:
                 with st.expander("Fit Model to Complete Dataset"):
                     st.write("Current Identified Best Parameters: ")
-                    st.write(st.session_state['best_params'])
-                    if st.button("Fit Model", key='fit_auto'):
-                        st.session_state["m"] = fit_complete(params=st.session_state['best_params'], 
+                    st.write(st.session_state['selected_options'])
+                    if st.button("Fit Model", key='fit_select'):
+                        st.session_state["m"] = fit_complete(params=st.session_state['selected_options'],
                                                              df=st.session_state['forecast_df'],
-                                                             events_df=is_events()) 
+                                                             events_df=is_events(),
+                                                             fit_spinner_text=fit_spinner_text)
                     else:
-                        st.write("Fit the model with the full data-set and best hyperparameters from grid search for the selected product.  \n", 
-                                 "This is required for moving to forecast prediction.")
+                        st.write(
+                            "Fit the model with the full data-set for the selected product.  This is required for moving to forecast prediction.")
+
+            with tab_auto:
+
+                st.subheader("Select options and ranges for an automated grid-search to find the best hyperparameters: ",
+                             st.session_state['forecast_product'])
+
+                with st.form("hyper_grid_form"):
+                    # Add a title to the form
+                    st.write("Select options for hyperparameter search.")
+
+                    # Define the options for each parameter
+                    seasonality_mode_options = st.multiselect(
+                        'Select seasonality_mode', ['additive', 'multiplicative'], default='additive')
+                    loss_func_options = st.multiselect(
+                        'Select loss_func', ['MSE', 'MAE'], default='MSE')
+                    n_cp_min, n_cp_max = st.slider(
+                        'Select n_changepoints (min=1/max=20)', min_value=1, max_value=20, value=(5, 10))
+                    n_cp_steps = st.number_input(
+                        'Select step-size for n_changepoints (min=1/max=10)', min_value=1, max_value=10, value=5)
+                    cp_range_min, cp_range_max = st.slider(
+                        'Select changepoints_range (min=0.01/max=20.0)', min_value=0.01, max_value=20.0, value=(1.0, 10.0))
+                    cp_range_steps = st.number_input(
+                        'Select step-size for n_changepoints (min=0.01/max=10.0)', min_value=0.01, max_value=10.0, value=9.0)
+                    normalize_options = st.multiselect(
+                        'Select normalization method', normalize_list, default='soft')
+                    n_lags_options = st.slider(
+                        'Select n_lags', min_value=7, max_value=90, value=30)
+                    n_forecasts_options = st.slider(
+                        'Select n_forecasts', min_value=7, max_value=90, value=30)
+                    num_hidden_layers_options = st.multiselect(
+                        'Select num_hidden_layers', [0, 1, 2], default=0)
+
+                    # Add a submit button to the form
+                    submitted = st.form_submit_button("Submit")
+
+                    # If the user submitted the form, print the selected options
+                    if submitted:
+                        # Create a dictionary to store the selected options
+                        st.session_state['hyperparam_options'] = {
+                            'seasonality_mode': seasonality_mode_options,
+                            'loss_func': loss_func_options,
+                            'n_changepoints': np.arange(n_cp_min, n_cp_max+1, n_cp_steps).tolist(),
+                            'changepoints_range': np.arange(cp_range_min, cp_range_max+0.01, cp_range_steps).tolist(),
+                            'normalize': normalize_options,
+                            'num_hidden_layers': num_hidden_layers_options,
+                            'n_lags': [n_lags_options],
+                            'n_forecasts': [n_forecasts_options]
+
+                        }
+
+                    st.write("Selected options:")
+                    st.write(st.session_state['hyperparam_options'])
+
+                if st.session_state['hyperparam_options']:
+                    with st.expander("Hyperparameter Search"):
+                        if st.button("Grid Search"):
+                            with st.spinner("Performing grid search for best hyperparameters... (Please do not refresh or close this tab while running to complete this task.)"):
+                                st.session_state['metrics_test'], st.session_state['best_params'] = cross_val_tune(
+                                    params=st.session_state['hyperparam_options'],
+                                    df=st.session_state['forecast_df'],
+                                    forecast_product=st.session_state['forecast_product'],
+                                    events_df=is_events(),
+                                    horizon=int(st.session_state['hyperparam_options']['n_forecasts'][0]))
+                            st.success("Cross-validation complete!", icon="✅")
+                        else:
+                            st.write(
+                                "Push \"Cross-Validate\" to Grid Search for best hyperparameters using 5-fold backtesting cross-validation.")
+
+                if st.session_state['best_params']:
+                    with st.expander("Fit Model to Complete Dataset"):
+                        st.write("Current Identified Best Parameters: ")
+                        st.write(st.session_state['best_params'])
+                        if st.button("Fit Model", key='fit_auto'):
+                            st.session_state["m"] = fit_complete(params=st.session_state['best_params'],
+                                                                 df=st.session_state['forecast_df'],
+                                                                 events_df=is_events(),
+                                                                 fit_spinner_text=fit_spinner_text)
+                        else:
+                            st.write("Fit the model with the full data-set and best hyperparameters from grid search for the selected product.  \n",
+                                     "This is required for moving to forecast prediction.")
```

### Comparing `d2c_mp_sales_forecaster-0.0.1/tests/test_1_Load_Data.py` & `d2c_mp_sales_forecaster-0.0.2/tests/test_1_Load_Data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 import pandas as pd
 from io import StringIO
-from ..src.d2c_mp_sales_forecaster.pages.1_Load_Data import (
+from d2c_mp_sales_forecaster.pages._1_Load_Data import (
     upload_sales_size_data,
     upload_master_data,
     upload_events_data,
     upload_lag_data,
     upload_future_data,
 )
```

### Comparing `d2c_mp_sales_forecaster-0.0.1/.gitignore` & `d2c_mp_sales_forecaster-0.0.2/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,19 @@
 .pytest_cache/
 cover/
 
 # Translations
 *.mo
 *.pot
 
+#Streamlit stuff:
+.streamlit
+.streamlit/secrets.toml
+.streamlit/postgres_secrets.env
+
 # Django stuff:
 *.log
 local_settings.py
 db.sqlite3
 db.sqlite3-journal
 
 # Flask stuff:
@@ -148,13 +153,16 @@
 
 # pytype static type analyzer
 .pytype/
 
 # Cython debug symbols
 cython_debug/
 
+#git stuff
+gitmsg.txt
+
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
```

### Comparing `d2c_mp_sales_forecaster-0.0.1/LICENSE` & `d2c_mp_sales_forecaster-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `d2c_mp_sales_forecaster-0.0.1/pyproject.toml` & `d2c_mp_sales_forecaster-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "d2c_mp_sales_forecaster"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Ryan Handerhan", email="rhanderh@alumni.cmu.edu" },
 ]
 description = "An application for forecasting direct-to-consumer sales quantities using the NeuralProphet algorithm from Meta."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

