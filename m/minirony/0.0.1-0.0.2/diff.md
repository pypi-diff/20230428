# Comparing `tmp/Minirony-0.0.1.tar.gz` & `tmp/minirony-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Minirony-0.0.1.tar", last modified: Thu Apr 27 17:45:58 2023, max compression
+gzip compressed data, was "minirony-0.0.2.tar", last modified: Fri Apr 28 19:18:48 2023, max compression
```

## Comparing `Minirony-0.0.1.tar` & `minirony-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 zagnoli   (1000) zagnoli   (1000)        0 2023-04-27 17:45:58.362355 Minirony-0.0.1/
-drwxr-xr-x   0 zagnoli   (1000) zagnoli   (1000)        0 2023-04-27 17:45:58.362355 Minirony-0.0.1/Minirony.egg-info/
--rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)      100 2023-04-27 17:45:58.000000 Minirony-0.0.1/Minirony.egg-info/PKG-INFO
--rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)      281 2023-04-27 17:45:58.000000 Minirony-0.0.1/Minirony.egg-info/SOURCES.txt
--rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)        1 2023-04-27 17:45:58.000000 Minirony-0.0.1/Minirony.egg-info/dependency_links.txt
--rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)        9 2023-04-27 17:45:58.000000 Minirony-0.0.1/Minirony.egg-info/top_level.txt
--rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)      100 2023-04-27 17:45:58.362355 Minirony-0.0.1/PKG-INFO
-drwxr-xr-x   0 zagnoli   (1000) zagnoli   (1000)        0 2023-04-27 17:45:58.362355 Minirony-0.0.1/minirony/
--rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)       28 2023-04-27 17:29:44.000000 Minirony-0.0.1/minirony/__init__.py
--rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)      178 2023-04-25 19:39:48.000000 Minirony-0.0.1/minirony/data_transfer.py
--rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)     1384 2023-04-25 19:39:48.000000 Minirony-0.0.1/minirony/factory.py
--rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)     3542 2023-04-25 19:39:48.000000 Minirony-0.0.1/minirony/helper.py
--rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)     9215 2023-04-25 19:39:48.000000 Minirony-0.0.1/minirony/manager.py
--rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)     1882 2023-04-25 19:39:48.000000 Minirony-0.0.1/minirony/provider.py
--rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)      755 2023-04-27 14:07:48.000000 Minirony-0.0.1/minirony/spark.py
--rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)       38 2023-04-27 17:45:58.362355 Minirony-0.0.1/setup.cfg
--rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)      171 2023-04-27 17:41:40.000000 Minirony-0.0.1/setup.py
+drwxr-xr-x   0 zagnoli   (1000) zagnoli   (1000)        0 2023-04-28 19:18:48.059960 minirony-0.0.2/
+-rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)      100 2023-04-28 19:18:48.059960 minirony-0.0.2/PKG-INFO
+drwxr-xr-x   0 zagnoli   (1000) zagnoli   (1000)        0 2023-04-28 19:18:48.059960 minirony-0.0.2/minirony/
+-rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)       40 2023-04-28 19:10:02.000000 minirony-0.0.2/minirony/__init__.py
+-rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)      178 2023-04-25 19:39:48.000000 minirony-0.0.2/minirony/data_transfer.py
+-rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)     1384 2023-04-25 19:39:48.000000 minirony-0.0.2/minirony/factory.py
+-rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)     3542 2023-04-25 19:39:48.000000 minirony-0.0.2/minirony/helper.py
+-rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)     9630 2023-04-28 19:08:46.000000 minirony-0.0.2/minirony/manager.py
+-rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)     1882 2023-04-25 19:39:48.000000 minirony-0.0.2/minirony/provider.py
+drwxr-xr-x   0 zagnoli   (1000) zagnoli   (1000)        0 2023-04-28 19:18:48.059960 minirony-0.0.2/minirony.egg-info/
+-rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)      100 2023-04-28 19:18:48.000000 minirony-0.0.2/minirony.egg-info/PKG-INFO
+-rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)      263 2023-04-28 19:18:48.000000 minirony-0.0.2/minirony.egg-info/SOURCES.txt
+-rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)        1 2023-04-28 19:18:48.000000 minirony-0.0.2/minirony.egg-info/dependency_links.txt
+-rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)        9 2023-04-28 19:18:48.000000 minirony-0.0.2/minirony.egg-info/top_level.txt
+-rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)       38 2023-04-28 19:18:48.059960 minirony-0.0.2/setup.cfg
+-rw-r--r--   0 zagnoli   (1000) zagnoli   (1000)      171 2023-04-28 19:14:04.000000 minirony-0.0.2/setup.py
```

### Comparing `Minirony-0.0.1/minirony/factory.py` & `minirony-0.0.2/minirony/factory.py`

 * *Files identical despite different names*

### Comparing `Minirony-0.0.1/minirony/helper.py` & `minirony-0.0.2/minirony/helper.py`

 * *Files identical despite different names*

### Comparing `Minirony-0.0.1/minirony/manager.py` & `minirony-0.0.2/minirony/manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,17 +20,26 @@
     DEV = "DEV"
     PROD = "PROD"
 
     def __init__(self):
         self.__create_aws_credentials()
 
     def get_jar_files(self):
-        current_directory = DirectoryManager.get_current_directory()
-        folder = f"{current_directory}/../jars"
-        jars_files = [folder + "/" + file for file in os.listdir(folder)]
+        jars_files = [
+            "com.amazonaws:aws-java-sdk-s3control:1.11.534",
+            "com.amazonaws:aws-java-sdk-core:1.11.534",
+            "com.amazonaws:aws-java-sdk-dynamodb:1.11.534",
+            "com.amazonaws:aws-java-sdk-kms:1.11.534",
+            "com.amazonaws:aws-java-sdk-s3:1.11.534",
+            "io.delta:delta-core_2.12:1.0.0",
+            "org.apache.hadoop:hadoop-aws:3.1.2",
+            "net.snowflake:snowflake-ingest-sdk:1.0.2-beta.4",
+            "net.snowflake:snowflake-jdbc:3.13.22",
+            "net.snowflake:spark-snowflake_2.12:2.11.0-spark_3.1",
+        ]
         jars = ",".join(jars_files)
         return jars
 
     def get_checkpoint_bucket(self):
         return os.getenv("CHECKPOINT_BUCKET")
 
     def get_landingzone_bucket(self):
@@ -128,15 +137,15 @@
         self.s3a_protocol = s3a_protocol
         self.__spark_session = None
         self.jars = jars
         self.aws_credentials = aws_credentials
 
     def get_session(self, app_name):
         spark_config = self.create_config(self.s3a_protocol)
-        spark_config.set("spark.jars", self.jars)
+        spark_config.set("spark.jars.packages", self.jars)
         spark_builder = SparkSession.builder.appName(app_name).config(conf=spark_config)
         self.__spark_session = spark_builder.getOrCreate()
 
         self.__spark_session.sparkContext.setLogLevel("ERROR")
 
         self.__set_credentials()
```

### Comparing `Minirony-0.0.1/minirony/provider.py` & `minirony-0.0.2/minirony/provider.py`

 * *Files identical despite different names*

