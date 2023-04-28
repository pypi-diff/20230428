# Comparing `tmp/SDTcloud-0.0.2.tar.gz` & `tmp/SDTcloud-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SDTcloud-0.0.2.tar", last modified: Thu Apr 27 00:52:36 2023, max compression
+gzip compressed data, was "SDTcloud-0.0.3.tar", last modified: Fri Apr 28 07:19:57 2023, max compression
```

## Comparing `SDTcloud-0.0.2.tar` & `SDTcloud-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-27 00:52:36.027404 SDTcloud-0.0.2/
--rw-r--r--   0 june       (501) staff       (20)      398 2023-04-27 00:52:36.027257 SDTcloud-0.0.2/PKG-INFO
--rw-r--r--   0 june       (501) staff       (20)       12 2023-04-27 00:33:43.000000 SDTcloud-0.0.2/README.md
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-27 00:52:36.026272 SDTcloud-0.0.2/SDTcloud/
--rw-r--r--   0 june       (501) staff       (20)       75 2023-04-27 00:34:53.000000 SDTcloud-0.0.2/SDTcloud/__init__.py
--rw-r--r--   0 june       (501) staff       (20)     4394 2023-04-27 00:52:06.000000 SDTcloud-0.0.2/SDTcloud/sdtcloud.py
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-27 00:52:36.027053 SDTcloud-0.0.2/SDTcloud.egg-info/
--rw-r--r--   0 june       (501) staff       (20)      398 2023-04-27 00:52:35.000000 SDTcloud-0.0.2/SDTcloud.egg-info/PKG-INFO
--rw-r--r--   0 june       (501) staff       (20)      188 2023-04-27 00:52:36.000000 SDTcloud-0.0.2/SDTcloud.egg-info/SOURCES.txt
--rw-r--r--   0 june       (501) staff       (20)        1 2023-04-27 00:52:35.000000 SDTcloud-0.0.2/SDTcloud.egg-info/dependency_links.txt
--rw-r--r--   0 june       (501) staff       (20)        9 2023-04-27 00:52:35.000000 SDTcloud-0.0.2/SDTcloud.egg-info/top_level.txt
--rw-r--r--   0 june       (501) staff       (20)       38 2023-04-27 00:52:36.027442 SDTcloud-0.0.2/setup.cfg
--rw-r--r--   0 june       (501) staff       (20)      656 2023-04-27 00:52:15.000000 SDTcloud-0.0.2/setup.py
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-28 07:19:57.019131 SDTcloud-0.0.3/
+-rw-r--r--   0 june       (501) staff       (20)      398 2023-04-28 07:19:57.019020 SDTcloud-0.0.3/PKG-INFO
+-rw-r--r--   0 june       (501) staff       (20)       12 2023-04-27 00:33:43.000000 SDTcloud-0.0.3/README.md
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-28 07:19:57.018448 SDTcloud-0.0.3/SDTcloud/
+-rw-r--r--   0 june       (501) staff       (20)       75 2023-04-27 00:34:53.000000 SDTcloud-0.0.3/SDTcloud/__init__.py
+-rw-r--r--   0 june       (501) staff       (20)     4574 2023-04-28 07:19:42.000000 SDTcloud-0.0.3/SDTcloud/sdtcloud.py
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-28 07:19:57.018876 SDTcloud-0.0.3/SDTcloud.egg-info/
+-rw-r--r--   0 june       (501) staff       (20)      398 2023-04-28 07:19:56.000000 SDTcloud-0.0.3/SDTcloud.egg-info/PKG-INFO
+-rw-r--r--   0 june       (501) staff       (20)      188 2023-04-28 07:19:56.000000 SDTcloud-0.0.3/SDTcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 june       (501) staff       (20)        1 2023-04-28 07:19:56.000000 SDTcloud-0.0.3/SDTcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 june       (501) staff       (20)        9 2023-04-28 07:19:56.000000 SDTcloud-0.0.3/SDTcloud.egg-info/top_level.txt
+-rw-r--r--   0 june       (501) staff       (20)       38 2023-04-28 07:19:57.019160 SDTcloud-0.0.3/setup.cfg
+-rw-r--r--   0 june       (501) staff       (20)      656 2023-04-28 07:19:52.000000 SDTcloud-0.0.3/setup.py
```

### Comparing `SDTcloud-0.0.2/SDTcloud/sdtcloud.py` & `SDTcloud-0.0.3/SDTcloud/sdtcloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,14 +130,21 @@
         
         headers = {
             "Authorization": self.userToken
         }
 
         response = requests.request('get',f"{self.url}/stackbase/v1/contents/download/{fileId}", headers=headers)
         result = json.loads(response.content)
+
+        if response.status_code != 200:
+            raise Exception(f"[ERROR] {result}")
+
+        open(getPath, "wb").write(response.content)
+        print("Success upload...")
+
         return result
     
     # 컨텐츠 등록
     def fput_content(self):
         print("fput")
         
 
@@ -156,8 +163,8 @@
 # # print("create folder")
 # # sdt_client.create_folder("5c0ab969-0397-45e8-8d97-b6fc20496a16", "", "sdtcloud-test")
 
 # # print("get List of tree")
 # # print(sdt_client.get_tree("5c0ab969-0397-45e8-8d97-b6fc20496a16", ""))
 
 # print("get List of tree")
-# sdt_client.get_tree("5c0ab969-0397-45e8-8d97-b6fc20496a16", "57d77d33-913f-4932-95a8-ea15b0de812e")
+# sdt_client.get_tree("5c0ab969-0397-45e8-8d97-b6fc20496a16", "57d77d33-913f-4932-95a8-ea15b0de812e")
```

### Comparing `SDTcloud-0.0.2/setup.py` & `SDTcloud-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SDTcloud", # Replace with your own username
-    version="0.0.2",
+    version="0.0.3",
     author="sujune",
     author_email="hoakw@sdt.inc",
     description="SDT cloud API Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

