# Comparing `tmp/sosin-1.0.3.tar.gz` & `tmp/sosin-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosin-1.0.3.tar", last modified: Mon Apr 24 10:26:26 2023, max compression
+gzip compressed data, was "sosin-1.0.4.tar", last modified: Fri Apr 28 16:00:39 2023, max compression
```

## Comparing `sosin-1.0.3.tar` & `sosin-1.0.4.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 10:26:26.457757 sosin-1.0.3/
--rw-rw-rw-   0        0        0     1083 2023-04-17 11:46:46.000000 sosin-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     1268 2023-04-24 10:26:26.456733 sosin-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      863 2023-04-17 11:46:46.000000 sosin-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-24 10:26:26.459134 sosin-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      994 2023-04-24 10:12:17.000000 sosin-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 10:26:26.412730 sosin-1.0.3/sosin/
--rw-rw-rw-   0        0        0        0 2023-04-17 12:05:52.000000 sosin-1.0.3/sosin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 10:26:26.431728 sosin-1.0.3/sosin/databases/
--rw-rw-rw-   0        0        0     9667 2023-04-24 02:18:48.000000 sosin-1.0.3/sosin/databases/rdb.py
-drwxrwxrwx   0        0        0        0 2023-04-24 10:26:26.434653 sosin-1.0.3/sosin/rpa/
--rw-rw-rw-   0        0        0    10828 2023-04-22 13:06:11.000000 sosin-1.0.3/sosin/rpa/email_mgr.py
--rw-rw-rw-   0        0        0     3698 2023-04-24 10:25:20.000000 sosin-1.0.3/sosin/rpa/sms_mgr.py
-drwxrwxrwx   0        0        0        0 2023-04-24 10:26:26.439798 sosin-1.0.3/sosin/utils/
--rw-rw-rw-   0        0        0     1687 2023-04-17 11:46:46.000000 sosin-1.0.3/sosin/utils/currency.py
--rw-rw-rw-   0        0        0      304 2023-04-17 11:46:46.000000 sosin-1.0.3/sosin/utils/log.py
--rw-rw-rw-   0        0        0      527 2023-04-17 11:46:46.000000 sosin-1.0.3/sosin/utils/progress.py
--rw-rw-rw-   0        0        0      385 2023-04-17 11:46:46.000000 sosin-1.0.3/sosin/utils/secret.py
-drwxrwxrwx   0        0        0        0 2023-04-24 10:26:26.454741 sosin-1.0.3/sosin/web/
--rw-rw-rw-   0        0        0     1055 2023-04-18 14:49:45.000000 sosin-1.0.3/sosin/web/content.py
--rw-rw-rw-   0        0        0     1018 2023-04-17 11:46:46.000000 sosin-1.0.3/sosin/web/translate.py
--rw-rw-rw-   0        0        0     4796 2023-04-24 07:25:27.000000 sosin-1.0.3/sosin/web/virtual.py
-drwxrwxrwx   0        0        0        0 2023-04-24 10:26:26.430748 sosin-1.0.3/sosin.egg-info/
--rw-rw-rw-   0        0        0     1268 2023-04-24 10:26:26.000000 sosin-1.0.3/sosin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-04-24 10:26:26.000000 sosin-1.0.3/sosin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 10:26:26.000000 sosin-1.0.3/sosin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-24 10:26:26.000000 sosin-1.0.3/sosin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-24 10:26:26.000000 sosin-1.0.3/sosin.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 16:00:39.104548 sosin-1.0.4/
+-rw-rw-rw-   0        0        0     1083 2023-04-17 11:46:46.000000 sosin-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1268 2023-04-28 16:00:39.103953 sosin-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      863 2023-04-17 11:46:46.000000 sosin-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-28 16:00:39.104548 sosin-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      994 2023-04-28 15:53:14.000000 sosin-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:00:39.065524 sosin-1.0.4/sosin/
+-rw-rw-rw-   0        0        0        0 2023-04-17 12:05:52.000000 sosin-1.0.4/sosin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:00:39.091707 sosin-1.0.4/sosin/databases/
+-rw-rw-rw-   0        0        0     4934 2023-04-24 10:38:48.000000 sosin-1.0.4/sosin/databases/fs.py
+-rw-rw-rw-   0        0        0     9667 2023-04-24 02:18:48.000000 sosin-1.0.4/sosin/databases/rdb.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:00:39.094235 sosin-1.0.4/sosin/rpa/
+-rw-rw-rw-   0        0        0    10828 2023-04-22 13:06:11.000000 sosin-1.0.4/sosin/rpa/email_mgr.py
+-rw-rw-rw-   0        0        0     3698 2023-04-24 11:58:43.000000 sosin-1.0.4/sosin/rpa/sms_mgr.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:00:39.098244 sosin-1.0.4/sosin/utils/
+-rw-rw-rw-   0        0        0     1687 2023-04-17 11:46:46.000000 sosin-1.0.4/sosin/utils/currency.py
+-rw-rw-rw-   0        0        0      304 2023-04-17 11:46:46.000000 sosin-1.0.4/sosin/utils/log.py
+-rw-rw-rw-   0        0        0      527 2023-04-17 11:46:46.000000 sosin-1.0.4/sosin/utils/progress.py
+-rw-rw-rw-   0        0        0      385 2023-04-17 11:46:46.000000 sosin-1.0.4/sosin/utils/secret.py
+-rw-rw-rw-   0        0        0      885 2023-04-28 16:00:12.000000 sosin-1.0.4/sosin/utils/zip.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:00:39.101722 sosin-1.0.4/sosin/web/
+-rw-rw-rw-   0        0        0     1055 2023-04-18 14:49:45.000000 sosin-1.0.4/sosin/web/content.py
+-rw-rw-rw-   0        0        0     1018 2023-04-17 11:46:46.000000 sosin-1.0.4/sosin/web/translate.py
+-rw-rw-rw-   0        0        0     4796 2023-04-24 07:25:27.000000 sosin-1.0.4/sosin/web/virtual.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:00:39.088192 sosin-1.0.4/sosin.egg-info/
+-rw-rw-rw-   0        0        0     1268 2023-04-28 16:00:38.000000 sosin-1.0.4/sosin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-04-28 16:00:38.000000 sosin-1.0.4/sosin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 16:00:38.000000 sosin-1.0.4/sosin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-28 16:00:38.000000 sosin-1.0.4/sosin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-28 16:00:38.000000 sosin-1.0.4/sosin.egg-info/top_level.txt
```

### Comparing `sosin-1.0.3/LICENSE` & `sosin-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sosin-1.0.3/PKG-INFO` & `sosin-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosin
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python utils for general works
 Home-page: https://github.com/devsosin/sosin
 Author: Jason Choi
 Author-email: svstar94@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sosin-1.0.3/README.md` & `sosin-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sosin-1.0.3/setup.py` & `sosin-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name                                = "sosin",
-    version                             = "1.0.3",
+    version                             = "1.0.4",
     license                             = 'MIT',
     author                              = "Jason Choi",
     author_email                        = "svstar94@gmail.com",
     description                         = "Python utils for general works",
     long_description                    = open('README.md').read(),
     url                                 = "https://github.com/devsosin/sosin",
     install_requires                    = ['requests', 'beautifulsoup4', 'PyMySQL',],
```

### Comparing `sosin-1.0.3/sosin/databases/rdb.py` & `sosin-1.0.4/sosin/databases/rdb.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.3/sosin/rpa/email_mgr.py` & `sosin-1.0.4/sosin/rpa/email_mgr.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.3/sosin/rpa/sms_mgr.py` & `sosin-1.0.4/sosin/rpa/sms_mgr.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.3/sosin/utils/currency.py` & `sosin-1.0.4/sosin/utils/currency.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.3/sosin/utils/progress.py` & `sosin-1.0.4/sosin/utils/progress.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.3/sosin/web/content.py` & `sosin-1.0.4/sosin/web/content.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.3/sosin/web/translate.py` & `sosin-1.0.4/sosin/web/translate.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.3/sosin/web/virtual.py` & `sosin-1.0.4/sosin/web/virtual.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.3/sosin.egg-info/PKG-INFO` & `sosin-1.0.4/sosin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosin
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python utils for general works
 Home-page: https://github.com/devsosin/sosin
 Author: Jason Choi
 Author-email: svstar94@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

