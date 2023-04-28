# Comparing `tmp/ser2sock-4.1.1.tar.gz` & `tmp/ser2sock-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ser2sock-4.1.1.tar", last modified: Wed Jul  8 19:11:31 2020, max compression
+gzip compressed data, was "ser2sock-4.1.2.tar", last modified: Fri Apr 28 05:19:31 2023, max compression
```

## Comparing `ser2sock-4.1.1.tar` & `ser2sock-4.1.2.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxrwxr-x   0 tcoutinho  (1000) tcoutinho  (1000)        0 2020-07-08 19:11:31.000000 ser2sock-4.1.1/
--rw-rw-r--   0 tcoutinho  (1000) tcoutinho  (1000)     4513 2020-07-08 19:11:31.000000 ser2sock-4.1.1/PKG-INFO
--rw-rw-r--   0 tcoutinho  (1000) tcoutinho  (1000)     2578 2020-07-08 16:59:50.000000 ser2sock-4.1.1/README.md
-drwxrwxr-x   0 tcoutinho  (1000) tcoutinho  (1000)        0 2020-07-08 19:11:31.000000 ser2sock-4.1.1/ser2sock/
--rw-rw-r--   0 tcoutinho  (1000) tcoutinho  (1000)       22 2020-07-08 19:11:18.000000 ser2sock-4.1.1/ser2sock/__init__.py
--rw-rw-r--   0 tcoutinho  (1000) tcoutinho  (1000)    12770 2020-07-08 18:52:15.000000 ser2sock-4.1.1/ser2sock/server.py
-drwxrwxr-x   0 tcoutinho  (1000) tcoutinho  (1000)        0 2020-07-08 19:11:31.000000 ser2sock-4.1.1/ser2sock.egg-info/
--rw-rw-r--   0 tcoutinho  (1000) tcoutinho  (1000)     4513 2020-07-08 19:11:30.000000 ser2sock-4.1.1/ser2sock.egg-info/PKG-INFO
--rw-rw-r--   0 tcoutinho  (1000) tcoutinho  (1000)      289 2020-07-08 19:11:30.000000 ser2sock-4.1.1/ser2sock.egg-info/SOURCES.txt
--rw-rw-r--   0 tcoutinho  (1000) tcoutinho  (1000)        1 2020-07-08 19:11:30.000000 ser2sock-4.1.1/ser2sock.egg-info/dependency_links.txt
--rw-rw-r--   0 tcoutinho  (1000) tcoutinho  (1000)       51 2020-07-08 19:11:30.000000 ser2sock-4.1.1/ser2sock.egg-info/entry_points.txt
--rw-rw-r--   0 tcoutinho  (1000) tcoutinho  (1000)       59 2020-07-08 19:11:30.000000 ser2sock-4.1.1/ser2sock.egg-info/requires.txt
--rw-rw-r--   0 tcoutinho  (1000) tcoutinho  (1000)        9 2020-07-08 19:11:30.000000 ser2sock-4.1.1/ser2sock.egg-info/top_level.txt
--rw-rw-r--   0 tcoutinho  (1000) tcoutinho  (1000)        1 2020-07-08 17:15:54.000000 ser2sock-4.1.1/ser2sock.egg-info/zip-safe
--rw-rw-r--   0 tcoutinho  (1000) tcoutinho  (1000)      604 2020-07-08 19:11:31.000000 ser2sock-4.1.1/setup.cfg
--rw-rw-r--   0 tcoutinho  (1000) tcoutinho  (1000)     2093 2020-07-08 19:11:18.000000 ser2sock-4.1.1/setup.py
+drwxrwxr-x   0 coutinho  (1000) coutinho  (1000)        0 2023-04-28 05:19:31.638167 ser2sock-4.1.2/
+-rw-rw-r--   0 coutinho  (1000) coutinho  (1000)     6450 2023-04-28 05:19:31.642167 ser2sock-4.1.2/PKG-INFO
+-rw-rw-r--   0 coutinho  (1000) coutinho  (1000)     5251 2023-04-28 05:18:57.000000 ser2sock-4.1.2/README.md
+drwxrwxr-x   0 coutinho  (1000) coutinho  (1000)        0 2023-04-28 05:19:31.638167 ser2sock-4.1.2/ser2sock/
+-rw-rw-r--   0 coutinho  (1000) coutinho  (1000)       22 2023-04-28 05:19:06.000000 ser2sock-4.1.2/ser2sock/__init__.py
+-rw-rw-r--   0 coutinho  (1000) coutinho  (1000)     5009 2023-04-28 05:18:57.000000 ser2sock-4.1.2/ser2sock/bridge.py
+-rw-rw-r--   0 coutinho  (1000) coutinho  (1000)     1043 2023-04-28 05:18:57.000000 ser2sock-4.1.2/ser2sock/comm.py
+-rw-rw-r--   0 coutinho  (1000) coutinho  (1000)     2011 2023-04-28 05:18:57.000000 ser2sock-4.1.2/ser2sock/config.py
+-rw-rw-r--   0 coutinho  (1000) coutinho  (1000)     3668 2023-04-28 05:18:57.000000 ser2sock-4.1.2/ser2sock/index.tpl
+-rw-rw-r--   0 coutinho  (1000) coutinho  (1000)     3134 2023-04-28 05:18:57.000000 ser2sock-4.1.2/ser2sock/server.py
+-rw-rw-r--   0 coutinho  (1000) coutinho  (1000)     2042 2023-04-28 05:18:57.000000 ser2sock-4.1.2/ser2sock/web.py
+drwxrwxr-x   0 coutinho  (1000) coutinho  (1000)        0 2023-04-28 05:19:31.638167 ser2sock-4.1.2/ser2sock.egg-info/
+-rw-rw-r--   0 coutinho  (1000) coutinho  (1000)     6450 2023-04-28 05:19:31.000000 ser2sock-4.1.2/ser2sock.egg-info/PKG-INFO
+-rw-rw-r--   0 coutinho  (1000) coutinho  (1000)      379 2023-04-28 05:19:31.000000 ser2sock-4.1.2/ser2sock.egg-info/SOURCES.txt
+-rw-rw-r--   0 coutinho  (1000) coutinho  (1000)        1 2023-04-28 05:19:31.000000 ser2sock-4.1.2/ser2sock.egg-info/dependency_links.txt
+-rw-rw-r--   0 coutinho  (1000) coutinho  (1000)       51 2023-04-28 05:19:31.000000 ser2sock-4.1.2/ser2sock.egg-info/entry_points.txt
+-rw-rw-r--   0 coutinho  (1000) coutinho  (1000)       59 2023-04-28 05:19:31.000000 ser2sock-4.1.2/ser2sock.egg-info/requires.txt
+-rw-rw-r--   0 coutinho  (1000) coutinho  (1000)        9 2023-04-28 05:19:31.000000 ser2sock-4.1.2/ser2sock.egg-info/top_level.txt
+-rw-rw-r--   0 coutinho  (1000) coutinho  (1000)        1 2023-04-28 05:19:31.000000 ser2sock-4.1.2/ser2sock.egg-info/zip-safe
+-rw-rw-r--   0 coutinho  (1000) coutinho  (1000)      604 2023-04-28 05:19:31.642167 ser2sock-4.1.2/setup.cfg
+-rw-rw-r--   0 coutinho  (1000) coutinho  (1000)     2274 2023-04-28 05:19:06.000000 ser2sock-4.1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ser2sock-4.1.1/setup.cfg` & `ser2sock-4.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 4.1.1
+current_version = 4.1.2
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `ser2sock-4.1.1/setup.py` & `ser2sock-4.1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup_requirements = []
 if TESTING:
     if sys.version_info < (3, 7):
         print("testing ser2sock needs python >= 3.7")
         exit(1)
     setup_requirements += ["pytest-runner"]
-test_requirements = ["pytest", "pytest-cov", "pytest-asyncio"]
+test_requirements = ["pytest", "pytest-cov"]
 
 with open("README.md") as f:
     description = f.read()
 
 setup(
     name="ser2sock",
     author="Jose Tiago Macara Coutinho",
@@ -33,14 +33,18 @@
         "Programming Language :: Python :: 2.6",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     description="serial to socket bridge",
     license="GPLv3+",
     long_description=description,
     long_description_content_type="text/markdown",
     keywords="serial line, tcp, udp, bridge, socket, server",
     packages=find_packages(),
@@ -57,16 +61,16 @@
         'ser2sock': ['*.tpl'],
     },
     entry_points={
         'console_scripts': [
             'ser2sock = ser2sock.server:main',
         ],
     },
-    url="https://github.com/tiagooutinho/ser2sock/",
+    url="https://github.com/tiagocoutinho/ser2sock/",
     project_urls={
         "Documentation": "https://tiagocoutinho.github.io/ser2sock/",
         "Source": "https://github.com/tiagocoutinho/ser2sock/",
     },
-    version="4.1.1",
+    version="4.1.2",
     python_requires=">=2.6",
     zip_safe=True
 )
```

