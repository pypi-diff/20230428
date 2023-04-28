# Comparing `tmp/seeme-0.9.5-py3-none-any.whl.zip` & `tmp/seeme-0.9.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4545 bytes, number of entries: 7
+Zip file size: 4560 bytes, number of entries: 7
 -rw-r--r--  2.0 unx      105 b- defN 20-Jun-25 06:28 seeme/__init__.py
--rw-r--r--  2.0 unx    17971 b- defN 20-Aug-24 11:39 seeme/seeme_client.py
--rw-r--r--  2.0 unx       48 b- defN 20-Aug-25 13:04 seeme/version.py
--rw-r--r--  2.0 unx        6 b- defN 20-Aug-25 13:09 seeme-0.9.5.dist-info/top_level.txt
--rw-r--r--  2.0 unx       92 b- defN 20-Aug-25 13:09 seeme-0.9.5.dist-info/WHEEL
--rw-r--r--  2.0 unx      303 b- defN 20-Aug-25 13:09 seeme-0.9.5.dist-info/METADATA
--rw-r--r--  2.0 unx      518 b- defN 20-Aug-25 13:09 seeme-0.9.5.dist-info/RECORD
-7 files, 19043 bytes uncompressed, 3643 bytes compressed:  80.9%
+-rw-r--r--  2.0 unx    18294 b- defN 20-Sep-08 14:38 seeme/seeme_client.py
+-rw-r--r--  2.0 unx       48 b- defN 20-Sep-08 14:31 seeme/version.py
+-rw-r--r--  2.0 unx        6 b- defN 20-Sep-08 14:49 seeme-0.9.6.dist-info/top_level.txt
+-rw-r--r--  2.0 unx       92 b- defN 20-Sep-08 14:49 seeme-0.9.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx      303 b- defN 20-Sep-08 14:49 seeme-0.9.6.dist-info/METADATA
+-rw-r--r--  2.0 unx      518 b- defN 20-Sep-08 14:49 seeme-0.9.6.dist-info/RECORD
+7 files, 19366 bytes uncompressed, 3658 bytes compressed:  81.1%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: seeme/seeme_client.py
 Comment: 
 
 Filename: seeme/version.py
 Comment: 
 
-Filename: seeme-0.9.5.dist-info/top_level.txt
+Filename: seeme-0.9.6.dist-info/top_level.txt
 Comment: 
 
-Filename: seeme-0.9.5.dist-info/WHEEL
+Filename: seeme-0.9.6.dist-info/WHEEL
 Comment: 
 
-Filename: seeme-0.9.5.dist-info/METADATA
+Filename: seeme-0.9.6.dist-info/METADATA
 Comment: 
 
-Filename: seeme-0.9.5.dist-info/RECORD
+Filename: seeme-0.9.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## seeme/seeme_client.py

```diff
@@ -93,25 +93,33 @@
 
     return self.api_post(model_api, model)
 
   # obsolete
   def create_full_model(self, model):
     return self.create_model(model)
     
-  def get_application_id(self, base_framework="pytorch", framework="fastai", base_framework_version="1.5.0", framework_version="1.0.61", application="image_classification"):
+  def get_application_id(self, base_framework="pytorch", framework="fastai", base_framework_version="1.6.0", framework_version="2.0.9", application="image_classification"):
     if self.applications == []:
       self.applications = self.get_applications()
 
     for f in self.applications:
       if f["base_framework"] == base_framework \
         and f["framework"] == framework \
         and f["base_framework_version"] == base_framework_version \
         and f["framework_version"] == framework_version \
         and f["application"] == application:
           return f["id"]
+    
+    for f in self.applications:
+      if f["base_framework"] == base_framework \
+        and f["framework"] == framework \
+        and f["base_framework_version"] in base_framework_version \
+        and f["framework_version"] == framework_version \
+        and f["application"] == application:
+          return f["id"]
       
     raise NotImplementedError()
 
   def get_model(self, model_id:str):
     self.requires_login()
 
     model_api = self.endpoints[MODELS_ENDPOINT] + "/" + model_id
```

## seeme/version.py

```diff
@@ -1,2 +1,2 @@
 __all__ = ['__version__']
-__version__ = '0.9.5'
+__version__ = '0.9.6'
```

