# Comparing `tmp/with_timeout-0.0.4.tar.gz` & `tmp/with_timeout-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "with_timeout-0.0.4.tar", last modified: Thu Apr 27 14:14:27 2023, max compression
+gzip compressed data, was "with_timeout-0.0.5.tar", last modified: Fri Apr 28 04:41:49 2023, max compression
```

## Comparing `with_timeout-0.0.4.tar` & `with_timeout-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-04-27 14:14:27.002614 with_timeout-0.0.4/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1069 2023-04-27 12:58:14.000000 with_timeout-0.0.4/LICENSE
--rw-r--r--   0 jeffrey    (501) staff       (20)       17 2023-04-27 13:07:40.000000 with_timeout-0.0.4/MANIFEST.in
--rw-r--r--   0 jeffrey    (501) staff       (20)      542 2023-04-27 14:14:27.002723 with_timeout-0.0.4/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)      154 2023-04-27 13:07:40.000000 with_timeout-0.0.4/README.md
--rw-r--r--   0 jeffrey    (501) staff       (20)       79 2023-04-27 14:14:27.002981 with_timeout-0.0.4/setup.cfg
--rw-r--r--   0 jeffrey    (501) staff       (20)      733 2023-04-27 14:13:51.000000 with_timeout-0.0.4/setup.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-04-27 14:14:27.002391 with_timeout-0.0.4/with_timeout.egg-info/
--rw-r--r--   0 jeffrey    (501) staff       (20)      542 2023-04-27 14:14:26.000000 with_timeout-0.0.4/with_timeout.egg-info/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)      243 2023-04-27 14:14:26.000000 with_timeout-0.0.4/with_timeout.egg-info/SOURCES.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-04-27 14:14:26.000000 with_timeout-0.0.4/with_timeout.egg-info/dependency_links.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       15 2023-04-27 14:14:26.000000 with_timeout-0.0.4/with_timeout.egg-info/requires.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       13 2023-04-27 14:14:26.000000 with_timeout-0.0.4/with_timeout.egg-info/top_level.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     1304 2023-04-27 13:02:50.000000 with_timeout-0.0.4/with_timeout.py
+drwxrwxr-x   0 jeffrey   (1000) jeffrey   (1000)        0 2023-04-28 04:41:49.283637 with_timeout-0.0.5/
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     1069 2023-04-28 04:39:41.000000 with_timeout-0.0.5/LICENSE
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)       17 2023-04-28 04:39:41.000000 with_timeout-0.0.5/MANIFEST.in
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)      516 2023-04-28 04:41:49.283637 with_timeout-0.0.5/PKG-INFO
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)      154 2023-04-28 04:39:41.000000 with_timeout-0.0.5/README.md
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)       79 2023-04-28 04:41:49.283637 with_timeout-0.0.5/setup.cfg
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)      727 2023-04-28 04:41:18.000000 with_timeout-0.0.5/setup.py
+drwxrwxr-x   0 jeffrey   (1000) jeffrey   (1000)        0 2023-04-28 04:41:49.283637 with_timeout-0.0.5/with_timeout.egg-info/
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)      516 2023-04-28 04:41:49.000000 with_timeout-0.0.5/with_timeout.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)      243 2023-04-28 04:41:49.000000 with_timeout-0.0.5/with_timeout.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)        1 2023-04-28 04:41:49.000000 with_timeout-0.0.5/with_timeout.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)       15 2023-04-28 04:41:49.000000 with_timeout-0.0.5/with_timeout.egg-info/requires.txt
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)       13 2023-04-28 04:41:49.000000 with_timeout-0.0.5/with_timeout.egg-info/top_level.txt
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     1304 2023-04-28 04:39:41.000000 with_timeout-0.0.5/with_timeout.py
```

### Comparing `with_timeout-0.0.4/LICENSE` & `with_timeout-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `with_timeout-0.0.4/PKG-INFO` & `with_timeout-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: with_timeout
-Version: 0.0.4
+Version: 0.0.5
 Summary: 模拟requests的timeout参数，使任意函数都拥有超时跳出的功能，防止访问超时阻塞影响代码的运行
 Home-page: https://github.com/snjyor/with_timeout
-Author: Jeffrey Yang
+Author: snjyor
 Author-email: snjyor@163.com
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 安装
 
 ```
 pip install with_timeout
@@ -21,9 +20,7 @@
 ```python
 from with_timeout import with_timeout
 @with_timeout(5)
 def my_func():
     pass
 ```
 
-
-
```

### Comparing `with_timeout-0.0.4/setup.py` & `with_timeout-0.0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 abs_path = path.abspath(path.dirname(__file__))
 with io.open(path.join(abs_path, 'README.md'), encoding='utf-8') as f:
     readme_data = f.read()
 
 setup(
     name='with_timeout',
     py_modules=['with_timeout'],
-    version='0.0.4',
+    version='0.0.5',
     description='模拟requests的timeout参数，使任意函数都拥有超时跳出的功能，防止访问超时阻塞影响代码的运行',
-    author='Jeffrey Yang',
+    author='snjyor',
     author_email='snjyor@163.com',
     url='https://github.com/snjyor/with_timeout',
     install_requires=[
         'beautifulsoup4'
     ],
     license='MIT',
     long_description=readme_data,
```

### Comparing `with_timeout-0.0.4/with_timeout.py` & `with_timeout-0.0.5/with_timeout.py`

 * *Files identical despite different names*

