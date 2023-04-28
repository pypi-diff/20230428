# Comparing `tmp/latest_earth_quake_Indonesia_chatur-0.0.4.tar.gz` & `tmp/latest_earth_quake_Indonesia_chatur-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latest_earth_quake_Indonesia_chatur-0.0.4.tar", last modified: Fri Apr 28 01:13:40 2023, max compression
+gzip compressed data, was "latest_earth_quake_Indonesia_chatur-0.0.5.tar", last modified: Fri Apr 28 01:16:19 2023, max compression
```

## Comparing `latest_earth_quake_Indonesia_chatur-0.0.4.tar` & `latest_earth_quake_Indonesia_chatur-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 01:13:40.290414 latest_earth_quake_Indonesia_chatur-0.0.4/
--rw-rw-rw-   0        0        0    35823 2023-04-27 00:11:05.000000 latest_earth_quake_Indonesia_chatur-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      823 2023-04-28 01:13:40.288814 latest_earth_quake_Indonesia_chatur-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      175 2023-04-27 00:17:07.000000 latest_earth_quake_Indonesia_chatur-0.0.4/README.md
--rw-rw-rw-   0        0        0      636 2023-04-28 01:13:08.000000 latest_earth_quake_Indonesia_chatur-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-28 01:13:40.290813 latest_earth_quake_Indonesia_chatur-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-28 01:13:40.245930 latest_earth_quake_Indonesia_chatur-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-28 01:13:40.258799 latest_earth_quake_Indonesia_chatur-0.0.4/src/gempaterkini_chatur/
--rw-rw-rw-   0        0        0     2761 2023-04-28 01:12:42.000000 latest_earth_quake_Indonesia_chatur-0.0.4/src/gempaterkini_chatur/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-27 23:38:48.000000 latest_earth_quake_Indonesia_chatur-0.0.4/src/gempaterkini_chatur/example.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:13:40.286811 latest_earth_quake_Indonesia_chatur-0.0.4/src/latest_earth_quake_Indonesia_chatur.egg-info/
--rw-rw-rw-   0        0        0      823 2023-04-28 01:13:40.000000 latest_earth_quake_Indonesia_chatur-0.0.4/src/latest_earth_quake_Indonesia_chatur.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-04-28 01:13:40.000000 latest_earth_quake_Indonesia_chatur-0.0.4/src/latest_earth_quake_Indonesia_chatur.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 01:13:40.000000 latest_earth_quake_Indonesia_chatur-0.0.4/src/latest_earth_quake_Indonesia_chatur.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-28 01:13:40.000000 latest_earth_quake_Indonesia_chatur-0.0.4/src/latest_earth_quake_Indonesia_chatur.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 01:16:19.678515 latest_earth_quake_Indonesia_chatur-0.0.5/
+-rw-rw-rw-   0        0        0    35823 2023-04-27 00:11:05.000000 latest_earth_quake_Indonesia_chatur-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1047 2023-04-28 01:16:19.677517 latest_earth_quake_Indonesia_chatur-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2023-04-28 01:15:21.000000 latest_earth_quake_Indonesia_chatur-0.0.5/README.md
+-rw-rw-rw-   0        0        0      636 2023-04-28 01:15:45.000000 latest_earth_quake_Indonesia_chatur-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-28 01:16:19.679518 latest_earth_quake_Indonesia_chatur-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 01:16:19.627515 latest_earth_quake_Indonesia_chatur-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 01:16:19.639540 latest_earth_quake_Indonesia_chatur-0.0.5/src/gempaterkini_chatur/
+-rw-rw-rw-   0        0        0     2761 2023-04-28 01:12:42.000000 latest_earth_quake_Indonesia_chatur-0.0.5/src/gempaterkini_chatur/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 23:38:48.000000 latest_earth_quake_Indonesia_chatur-0.0.5/src/gempaterkini_chatur/example.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:16:19.674678 latest_earth_quake_Indonesia_chatur-0.0.5/src/latest_earth_quake_Indonesia_chatur.egg-info/
+-rw-rw-rw-   0        0        0     1047 2023-04-28 01:16:19.000000 latest_earth_quake_Indonesia_chatur-0.0.5/src/latest_earth_quake_Indonesia_chatur.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-04-28 01:16:19.000000 latest_earth_quake_Indonesia_chatur-0.0.5/src/latest_earth_quake_Indonesia_chatur.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 01:16:19.000000 latest_earth_quake_Indonesia_chatur-0.0.5/src/latest_earth_quake_Indonesia_chatur.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-28 01:16:19.000000 latest_earth_quake_Indonesia_chatur-0.0.5/src/latest_earth_quake_Indonesia_chatur.egg-info/top_level.txt
```

### Comparing `latest_earth_quake_Indonesia_chatur-0.0.4/LICENSE` & `latest_earth_quake_Indonesia_chatur-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `latest_earth_quake_Indonesia_chatur-0.0.4/PKG-INFO` & `latest_earth_quake_Indonesia_chatur-0.0.5/src/latest_earth_quake_Indonesia_chatur.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 Metadata-Version: 2.1
-Name: latest_earth_quake_Indonesia_chatur
-Version: 0.0.4
+Name: latest-earth-quake-Indonesia-chatur
+Version: 0.0.5
 Summary: This package will get the latest earthquake (Indonesia) from https://www.bmkg.go.id/ BMKG
 Author-email: Chatur Agus Priyono <chatur.agus.priyono@gmail.com>
 Project-URL: Homepage, https://github.com/chaturap/bmkg-latest-earthquake
 Project-URL: Bug Tracker, https://github.com/chaturap/bmkg-latest-earthquake/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bmkg-latest-earthquake
 This package will get the latest earthquake (Indonesia) from https://www.bmkg.go.id/  BMKG | Meteorological, Climatological, and Geophysical Agency
+
+example using this module
+
+import gempaterkini_chatur
+
+#    if __name__ == '__main__':
+#    print("Aplikasi Utama")
+#    result = gempaterkini_chatur.ekstrasi_data()
+#    gempaterkini_chatur.tampilkan_data(result)
```

### Comparing `latest_earth_quake_Indonesia_chatur-0.0.4/pyproject.toml` & `latest_earth_quake_Indonesia_chatur-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "latest_earth_quake_Indonesia_chatur"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Chatur Agus Priyono", email="chatur.agus.priyono@gmail.com" },
 ]
 description = "This package will get the latest earthquake (Indonesia) from https://www.bmkg.go.id/ BMKG"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `latest_earth_quake_Indonesia_chatur-0.0.4/src/gempaterkini_chatur/__init__.py` & `latest_earth_quake_Indonesia_chatur-0.0.5/src/gempaterkini_chatur/__init__.py`

 * *Files identical despite different names*

