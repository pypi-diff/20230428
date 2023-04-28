# Comparing `tmp/SDTcloud-0.0.4.tar.gz` & `tmp/SDTcloud-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SDTcloud-0.0.4.tar", last modified: Fri Apr 28 07:25:02 2023, max compression
+gzip compressed data, was "SDTcloud-0.0.5.tar", last modified: Fri Apr 28 07:30:08 2023, max compression
```

## Comparing `SDTcloud-0.0.4.tar` & `SDTcloud-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-28 07:25:02.890480 SDTcloud-0.0.4/
--rw-r--r--   0 june       (501) staff       (20)      398 2023-04-28 07:25:02.890365 SDTcloud-0.0.4/PKG-INFO
--rw-r--r--   0 june       (501) staff       (20)       12 2023-04-27 00:33:43.000000 SDTcloud-0.0.4/README.md
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-28 07:25:02.889726 SDTcloud-0.0.4/SDTcloud/
--rw-r--r--   0 june       (501) staff       (20)       75 2023-04-27 00:34:53.000000 SDTcloud-0.0.4/SDTcloud/__init__.py
--rw-r--r--   0 june       (501) staff       (20)     4583 2023-04-28 07:24:45.000000 SDTcloud-0.0.4/SDTcloud/sdtcloud.py
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-28 07:25:02.890205 SDTcloud-0.0.4/SDTcloud.egg-info/
--rw-r--r--   0 june       (501) staff       (20)      398 2023-04-28 07:25:02.000000 SDTcloud-0.0.4/SDTcloud.egg-info/PKG-INFO
--rw-r--r--   0 june       (501) staff       (20)      188 2023-04-28 07:25:02.000000 SDTcloud-0.0.4/SDTcloud.egg-info/SOURCES.txt
--rw-r--r--   0 june       (501) staff       (20)        1 2023-04-28 07:25:02.000000 SDTcloud-0.0.4/SDTcloud.egg-info/dependency_links.txt
--rw-r--r--   0 june       (501) staff       (20)        9 2023-04-28 07:25:02.000000 SDTcloud-0.0.4/SDTcloud.egg-info/top_level.txt
--rw-r--r--   0 june       (501) staff       (20)       38 2023-04-28 07:25:02.890510 SDTcloud-0.0.4/setup.cfg
--rw-r--r--   0 june       (501) staff       (20)      656 2023-04-28 07:25:00.000000 SDTcloud-0.0.4/setup.py
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-28 07:30:08.457491 SDTcloud-0.0.5/
+-rw-r--r--   0 june       (501) staff       (20)      398 2023-04-28 07:30:08.457378 SDTcloud-0.0.5/PKG-INFO
+-rw-r--r--   0 june       (501) staff       (20)       12 2023-04-27 00:33:43.000000 SDTcloud-0.0.5/README.md
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-28 07:30:08.456796 SDTcloud-0.0.5/SDTcloud/
+-rw-r--r--   0 june       (501) staff       (20)       75 2023-04-27 00:34:53.000000 SDTcloud-0.0.5/SDTcloud/__init__.py
+-rw-r--r--   0 june       (501) staff       (20)     4560 2023-04-28 07:29:45.000000 SDTcloud-0.0.5/SDTcloud/sdtcloud.py
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-28 07:30:08.457226 SDTcloud-0.0.5/SDTcloud.egg-info/
+-rw-r--r--   0 june       (501) staff       (20)      398 2023-04-28 07:30:08.000000 SDTcloud-0.0.5/SDTcloud.egg-info/PKG-INFO
+-rw-r--r--   0 june       (501) staff       (20)      188 2023-04-28 07:30:08.000000 SDTcloud-0.0.5/SDTcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 june       (501) staff       (20)        1 2023-04-28 07:30:08.000000 SDTcloud-0.0.5/SDTcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 june       (501) staff       (20)        9 2023-04-28 07:30:08.000000 SDTcloud-0.0.5/SDTcloud.egg-info/top_level.txt
+-rw-r--r--   0 june       (501) staff       (20)       38 2023-04-28 07:30:08.457521 SDTcloud-0.0.5/setup.cfg
+-rw-r--r--   0 june       (501) staff       (20)      656 2023-04-28 07:30:04.000000 SDTcloud-0.0.5/setup.py
```

### Comparing `SDTcloud-0.0.4/SDTcloud/sdtcloud.py` & `SDTcloud-0.0.5/SDTcloud/sdtcloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,16 +136,14 @@
         result = json.loads(response.content)
 
         if response.status_code != 200:
             raise Exception(f"[ERROR] {result}")
 
         open(getPath, "wb").write(response.content)
         print("Success upload...")
-
-        return result
     
     # 컨텐츠 등록
     def fput_content(self):
         print("fput")
         
 
 # print("Login")
```

### Comparing `SDTcloud-0.0.4/setup.py` & `SDTcloud-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SDTcloud", # Replace with your own username
-    version="0.0.4",
+    version="0.0.5",
     author="sujune",
     author_email="hoakw@sdt.inc",
     description="SDT cloud API Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

