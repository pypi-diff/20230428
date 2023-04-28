# Comparing `tmp/SDTcloud-0.0.3.tar.gz` & `tmp/SDTcloud-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SDTcloud-0.0.3.tar", last modified: Fri Apr 28 07:19:57 2023, max compression
+gzip compressed data, was "SDTcloud-0.0.4.tar", last modified: Fri Apr 28 07:25:02 2023, max compression
```

## Comparing `SDTcloud-0.0.3.tar` & `SDTcloud-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-28 07:19:57.019131 SDTcloud-0.0.3/
--rw-r--r--   0 june       (501) staff       (20)      398 2023-04-28 07:19:57.019020 SDTcloud-0.0.3/PKG-INFO
--rw-r--r--   0 june       (501) staff       (20)       12 2023-04-27 00:33:43.000000 SDTcloud-0.0.3/README.md
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-28 07:19:57.018448 SDTcloud-0.0.3/SDTcloud/
--rw-r--r--   0 june       (501) staff       (20)       75 2023-04-27 00:34:53.000000 SDTcloud-0.0.3/SDTcloud/__init__.py
--rw-r--r--   0 june       (501) staff       (20)     4574 2023-04-28 07:19:42.000000 SDTcloud-0.0.3/SDTcloud/sdtcloud.py
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-28 07:19:57.018876 SDTcloud-0.0.3/SDTcloud.egg-info/
--rw-r--r--   0 june       (501) staff       (20)      398 2023-04-28 07:19:56.000000 SDTcloud-0.0.3/SDTcloud.egg-info/PKG-INFO
--rw-r--r--   0 june       (501) staff       (20)      188 2023-04-28 07:19:56.000000 SDTcloud-0.0.3/SDTcloud.egg-info/SOURCES.txt
--rw-r--r--   0 june       (501) staff       (20)        1 2023-04-28 07:19:56.000000 SDTcloud-0.0.3/SDTcloud.egg-info/dependency_links.txt
--rw-r--r--   0 june       (501) staff       (20)        9 2023-04-28 07:19:56.000000 SDTcloud-0.0.3/SDTcloud.egg-info/top_level.txt
--rw-r--r--   0 june       (501) staff       (20)       38 2023-04-28 07:19:57.019160 SDTcloud-0.0.3/setup.cfg
--rw-r--r--   0 june       (501) staff       (20)      656 2023-04-28 07:19:52.000000 SDTcloud-0.0.3/setup.py
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-28 07:25:02.890480 SDTcloud-0.0.4/
+-rw-r--r--   0 june       (501) staff       (20)      398 2023-04-28 07:25:02.890365 SDTcloud-0.0.4/PKG-INFO
+-rw-r--r--   0 june       (501) staff       (20)       12 2023-04-27 00:33:43.000000 SDTcloud-0.0.4/README.md
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-28 07:25:02.889726 SDTcloud-0.0.4/SDTcloud/
+-rw-r--r--   0 june       (501) staff       (20)       75 2023-04-27 00:34:53.000000 SDTcloud-0.0.4/SDTcloud/__init__.py
+-rw-r--r--   0 june       (501) staff       (20)     4583 2023-04-28 07:24:45.000000 SDTcloud-0.0.4/SDTcloud/sdtcloud.py
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-28 07:25:02.890205 SDTcloud-0.0.4/SDTcloud.egg-info/
+-rw-r--r--   0 june       (501) staff       (20)      398 2023-04-28 07:25:02.000000 SDTcloud-0.0.4/SDTcloud.egg-info/PKG-INFO
+-rw-r--r--   0 june       (501) staff       (20)      188 2023-04-28 07:25:02.000000 SDTcloud-0.0.4/SDTcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 june       (501) staff       (20)        1 2023-04-28 07:25:02.000000 SDTcloud-0.0.4/SDTcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 june       (501) staff       (20)        9 2023-04-28 07:25:02.000000 SDTcloud-0.0.4/SDTcloud.egg-info/top_level.txt
+-rw-r--r--   0 june       (501) staff       (20)       38 2023-04-28 07:25:02.890510 SDTcloud-0.0.4/setup.cfg
+-rw-r--r--   0 june       (501) staff       (20)      656 2023-04-28 07:25:00.000000 SDTcloud-0.0.4/setup.py
```

### Comparing `SDTcloud-0.0.3/SDTcloud/sdtcloud.py` & `SDTcloud-0.0.4/SDTcloud/sdtcloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         print("test")
     
     # 컨텐츠 삭제
     def delete_content(self):
         print("test")
 
     # 컨텐츠 다운로드
-    def fget_content(self, fileId):
+    def fget_content(self, fileId, getPath):
         
         headers = {
             "Authorization": self.userToken
         }
 
         response = requests.request('get',f"{self.url}/stackbase/v1/contents/download/{fileId}", headers=headers)
         result = json.loads(response.content)
```

### Comparing `SDTcloud-0.0.3/setup.py` & `SDTcloud-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SDTcloud", # Replace with your own username
-    version="0.0.3",
+    version="0.0.4",
     author="sujune",
     author_email="hoakw@sdt.inc",
     description="SDT cloud API Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

