# Comparing `tmp/richspot-1.0.0.tar.gz` & `tmp/richspot-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "richspot-1.0.0.tar", last modified: Mon Apr 10 13:09:28 2023, max compression
+gzip compressed data, was "richspot-1.0.1.tar", last modified: Fri Apr 28 17:06:52 2023, max compression
```

## Comparing `richspot-1.0.0.tar` & `richspot-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35149 2023-04-09 12:26:55.492952 richspot-1.0.0/LICENSE
--rw-r--r--   0        0        0     1839 2023-04-10 13:04:21.741580 richspot-1.0.0/README.md
--rw-r--r--   0        0        0     1290 2023-04-10 13:06:09.537588 richspot-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3818 2023-04-09 20:11:12.292021 richspot-1.0.0/richspot.py
--rw-r--r--   0        0        0     2726 1970-01-01 00:00:00.000000 richspot-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-09 12:26:55.492952 richspot-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2032 2023-04-28 16:56:40.314045 richspot-1.0.1/README.md
+-rw-r--r--   0        0        0     1290 2023-04-28 17:03:40.874075 richspot-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4994 2023-04-28 17:04:03.860077 richspot-1.0.1/richspot.py
+-rw-r--r--   0        0        0     2919 1970-01-01 00:00:00.000000 richspot-1.0.1/PKG-INFO
```

### Comparing `richspot-1.0.0/LICENSE` & `richspot-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `richspot-1.0.0/README.md` & `richspot-1.0.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 # Table of Contents
 
 1.  [RichSpot](#org0b141a4)
     1.  [Ncspot discord rich presence add-on](#org5e7e59d)
+    1.  [Assets Notice](#org5e7e592)
     2.  [Installing / Running RichSpot](#org14af663)
         1.  [Through PyPi](#org1cd60f9)
         2.  [Manually](#org6ef52cc)
         3.  [Running](#org597ff1a)
     3.  [Requirements](#orgfa35322)
         1.  [How to obtain client id and authorization token?](#org5997f48)
         2.  [WARNING ⚠](#org6cef86a)
@@ -24,14 +25,18 @@
 Thus using **RichSpot** makes it possible to do.
 
 ![img](https://raw.githubusercontent.com/M1ndo/RichSpot/main/imgs/example.png)
 
 
 <a id="org14af663"></a>
 
+## Assets Notice
+Assets will not be visible until they're cached this is a limitation of =discord=.
+It will take atleast 10-15 min before they're visible.
+
 ## Installing / Running RichSpot
 
 
 <a id="org1cd60f9"></a>
 
 ### Through PyPi
```

### Comparing `richspot-1.0.0/pyproject.toml` & `richspot-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "richspot"
 description = "ncspot discord rich presence"
-version = "1.0.0"
+version = "1.0.1"
 keywords = ["Spotify", "Spotify Rich Presence", "Rich Presence", "Ncspot", "Ncspot Rich Presence", "Discord", "Discord Rich Presence", "Spotify Connect"]
 authors = [
     { name = "Younes Ben El", email = "ybenel@duck.com" }
 ]
 dependencies = [
     "pypresence",
     "requests",
```

### Comparing `richspot-1.0.0/PKG-INFO` & `richspot-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: richspot
-Version: 1.0.0
+Version: 1.0.1
 Summary: ncspot discord rich presence
 Keywords: Spotify,Spotify Rich Presence,Rich Presence,Ncspot,Ncspot Rich Presence,Discord,Discord Rich Presence,Spotify Connect
 Author-email: Younes Ben El <ybenel@duck.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -20,14 +20,15 @@
 Project-URL: Source, https://github.com/m1ndo/RichSpot
 
 
 # Table of Contents
 
 1.  [RichSpot](#org0b141a4)
     1.  [Ncspot discord rich presence add-on](#org5e7e59d)
+    1.  [Assets Notice](#org5e7e592)
     2.  [Installing / Running RichSpot](#org14af663)
         1.  [Through PyPi](#org1cd60f9)
         2.  [Manually](#org6ef52cc)
         3.  [Running](#org597ff1a)
     3.  [Requirements](#orgfa35322)
         1.  [How to obtain client id and authorization token?](#org5997f48)
         2.  [WARNING ⚠](#org6cef86a)
@@ -45,14 +46,18 @@
 Thus using **RichSpot** makes it possible to do.
 
 ![img](https://raw.githubusercontent.com/M1ndo/RichSpot/main/imgs/example.png)
 
 
 <a id="org14af663"></a>
 
+## Assets Notice
+Assets will not be visible until they're cached this is a limitation of =discord=.
+It will take atleast 10-15 min before they're visible.
+
 ## Installing / Running RichSpot
 
 
 <a id="org1cd60f9"></a>
 
 ### Through PyPi
```

