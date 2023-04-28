# Comparing `tmp/refractio-1.0.0.tar.gz` & `tmp/refractio-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refractio-1.0.0.tar", last modified: Thu Apr 27 10:36:22 2023, max compression
+gzip compressed data, was "refractio-1.0.1.tar", last modified: Fri Apr 28 11:08:13 2023, max compression
```

## Comparing `refractio-1.0.0.tar` & `refractio-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-04-27 10:36:22.896572 refractio-1.0.0/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      441 2023-04-27 10:36:22.895572 refractio-1.0.0/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       78 2023-04-27 10:35:25.000000 refractio-1.0.0/README.md
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-04-27 10:36:22.894572 refractio-1.0.0/refractio/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        0 2023-04-27 10:09:48.000000 refractio-1.0.0/refractio/__init__.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    10153 2023-04-27 10:09:48.000000 refractio-1.0.0/refractio/refractio.py
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-04-27 10:36:22.895572 refractio-1.0.0/refractio.egg-info/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      441 2023-04-27 10:36:22.000000 refractio-1.0.0/refractio.egg-info/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      227 2023-04-27 10:36:22.000000 refractio-1.0.0/refractio.egg-info/SOURCES.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-04-27 10:36:22.000000 refractio-1.0.0/refractio.egg-info/dependency_links.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      176 2023-04-27 10:36:22.000000 refractio-1.0.0/refractio.egg-info/requires.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-04-27 10:36:22.000000 refractio-1.0.0/refractio.egg-info/top_level.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-04-27 10:36:22.896572 refractio-1.0.0/setup.cfg
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      946 2023-04-27 10:09:48.000000 refractio-1.0.0/setup.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-04-28 11:08:13.588151 refractio-1.0.1/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      605 2023-04-28 11:08:13.587151 refractio-1.0.1/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      527 2023-04-28 10:17:05.000000 refractio-1.0.1/README.md
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-04-28 11:08:13.586151 refractio-1.0.1/refractio/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        0 2023-04-28 10:17:05.000000 refractio-1.0.1/refractio/__init__.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    13016 2023-04-28 10:17:05.000000 refractio-1.0.1/refractio/refractio.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-04-28 11:08:13.587151 refractio-1.0.1/refractio.egg-info/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      605 2023-04-28 11:08:13.000000 refractio-1.0.1/refractio.egg-info/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      227 2023-04-28 11:08:13.000000 refractio-1.0.1/refractio.egg-info/SOURCES.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-04-28 11:08:13.000000 refractio-1.0.1/refractio.egg-info/dependency_links.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      335 2023-04-28 11:08:13.000000 refractio-1.0.1/refractio.egg-info/requires.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-04-28 11:08:13.000000 refractio-1.0.1/refractio.egg-info/top_level.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-04-28 11:08:13.588151 refractio-1.0.1/setup.cfg
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1365 2023-04-28 10:17:05.000000 refractio-1.0.1/setup.py
```

### Comparing `refractio-1.0.0/refractio/refractio.py` & `refractio-1.0.1/refractio/refractio.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,26 +11,32 @@
     """
     Param:
         ds_name,
         user_id=os.getenv("user_id"),
         project_id=os.getenv("project_id"),
         row_count=-1,
         strategy="top"
-    To get pandas dataframe
+    To get pandas dataframe.
+    Need to install mosaic-connector-python for reading dataframe using connector backend,
+    git+https://gitlab+deploy-token-14:myUpFE_XRxShG53Hs6tV@git.lti-aiq.in/mosaic-decisions-2-0/mosaic-connector-python.git@1.0.29.3
     """
     try:
+        print(f'user_id: {user_id}\nproject_id: {project_id}')
         url = f"http://connection-manager:80/connections/api/External/v1/external/getConnConfig/" \
               f"{ds_name}/{user_id}/{project_id}"
         connection_details = requests.get(url, verify=False).json()
 
         if connection_details["params"]["READER"]["type"] == "RDBMS":
             if connection_details["params"]["READER"]["sub_type"] == "SNOWFLAKE":
                 data_frame = get_snowflake_df(connection_details, row_count, strategy)
+            elif connection_details["params"]["READER"]["sub_type"] == "MYSQL":
+                data_frame = get_mysql_df(connection_details, row_count, strategy)
             else:
                 print("Reading dataframe using connector backend")
+                # Need to install, git+https://gitlab+deploy-token-14:myUpFE_XRxShG53Hs6tV@git.lti-aiq.in/mosaic-decisions-2-0/mosaic-connector-python.git
                 from connector.mosaicio import MosaicioConnector
                 connector = MosaicioConnector()
                 data_frame = connector.getPandasDataFrame(
                     param=connection_details["params"],
                     row_count=row_count,
                     strategy=strategy
                 )
@@ -115,14 +121,73 @@
 
     # Close cursor and connection
     cur.close()
     con.close()
     return data_frame
 
 
+def get_hive_df(connection_details, row_count, strategy):
+    """
+    Param:
+        connection_details: connection details dict
+        row_count: number of rows to be fetched
+        strategy: top/bottom
+    To read data frame form hive connection
+    """
+    import pyhive
+
+    # Establish connection to the Hive Server
+    conn = pyhive.hive.Connection(host=connection_details["params"]["READER"]["host"],
+                                  port=connection_details["params"]["READER"]["port"],
+                                  username=connection_details["params"]["READER"]["user"],
+                                  password=connection_details["params"]["READER"]["password"],
+                                  database=connection_details["params"]["READER"]["database"])
+
+    if int(row_count) > 0:
+        # Generate query
+        query = f"SELECT * FROM {connection_details['params']['READER']['tables']} LIMIT {int(row_count)}"
+    else:
+        query = f"SELECT * FROM {connection_details['params']['READER']['tables']};"
+
+    # Read data from Hive
+    data_frame = pd.read_sql(query, conn)
+
+    # Close the connection
+    conn.close()
+    return data_frame
+
+
+def get_mysql_df(connection_details, row_count, strategy):
+    """
+    Param:
+        connection_details: connection details dict
+        row_count: number of rows to be fetched
+        strategy: top/bottom
+    To read data frame form mysql connection
+    """
+    import pymysql
+
+    conn = pymysql.connect(host=connection_details["params"]["READER"]["host"],
+                           port=int(connection_details["params"]["READER"]["port"]),
+                           user=connection_details["params"]["READER"]["user"],
+                           passwd=connection_details["params"]["READER"]["password"],
+                           db=connection_details["params"]["READER"]["database"])
+
+    if int(row_count) > 0:
+        # Generate query
+        query = f"SELECT * FROM {connection_details['params']['READER']['tables']} LIMIT {int(row_count)}"
+    else:
+        query = f"SELECT * FROM {connection_details['params']['READER']['tables']};"
+    # Read data fromm mysql
+    data_frame = pd.read_sql(query, con=conn)
+    # Close connection
+    conn.close()
+    return data_frame
+
+
 def get_s3_df(connection_details, row_count, strategy):
     """
     Param:
         connection_details: connection details dict
         row_count: number of rows to be fetched
         strategy: top/bottom
     To read data frame form amazon S3 connection
```

### Comparing `refractio-1.0.0/setup.py` & `refractio-1.0.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'REFRACT IO'
 LONG_DESCRIPTION = 'To read and write dataframe from different connectors'
 
 extras_require = {
+    "all": [
+        "snowflake-connector-python[pandas]==3.0.2",
+        "boto3==1.26.116",
+        "azure==4.0.0",
+        "openpyxl==3.1.2",
+        "xlrd==2.0.1",
+        "pysftp==0.2.9",
+        "pymysql==1.0.3"
+    ],
     "snowflake": [
         "snowflake-connector-python[pandas]==3.0.2"
     ],
     "s3": [
         "boto3==1.26.116"
     ],
     "azureblob": [
@@ -16,14 +25,17 @@
     ],
     "local": [
         "openpyxl==3.1.2",
         "xlrd==2.0.1",
     ],
     "sftp": [
         "pysftp==0.2.9"
+    ],
+    "mysql": [
+        "pymysql==1.0.3"
     ]
 }
 
 # Setting up
 setup(
     name="refractio",
     version=VERSION,
@@ -37,8 +49,12 @@
         "pandas==2.0.0"
     ],
     keywords=['refractio'],
     classifiers=[
         "Programming Language :: Python :: 3.8",
     ],
     extras_require=extras_require,
-)
+    project_urls={
+        "Product": "https://www.fosfor.com/refract/",
+        "Source": "https://git.lti-aiq.in/refract-sdk/refract-sdk",
+    }
+)
```

