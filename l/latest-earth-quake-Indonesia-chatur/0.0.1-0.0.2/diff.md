# Comparing `tmp/latest_earth_quake_Indonesia_chatur-0.0.1.tar.gz` & `tmp/latest_earth_quake_Indonesia_chatur-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latest_earth_quake_Indonesia_chatur-0.0.1.tar", last modified: Fri Apr 28 00:20:54 2023, max compression
+gzip compressed data, was "latest_earth_quake_Indonesia_chatur-0.0.2.tar", last modified: Fri Apr 28 00:46:11 2023, max compression
```

## Comparing `latest_earth_quake_Indonesia_chatur-0.0.1.tar` & `latest_earth_quake_Indonesia_chatur-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 00:20:54.851449 latest_earth_quake_Indonesia_chatur-0.0.1/
--rw-rw-rw-   0        0        0    35823 2023-04-27 00:11:05.000000 latest_earth_quake_Indonesia_chatur-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      823 2023-04-28 00:20:54.850042 latest_earth_quake_Indonesia_chatur-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      175 2023-04-27 00:17:07.000000 latest_earth_quake_Indonesia_chatur-0.0.1/README.md
--rw-rw-rw-   0        0        0      636 2023-04-28 00:18:55.000000 latest_earth_quake_Indonesia_chatur-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-28 00:20:54.851449 latest_earth_quake_Indonesia_chatur-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-28 00:20:54.803449 latest_earth_quake_Indonesia_chatur-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-28 00:20:54.818555 latest_earth_quake_Indonesia_chatur-0.0.1/src/gempaterkini_chatur/
--rw-rw-rw-   0        0        0     2789 2023-04-27 00:10:35.000000 latest_earth_quake_Indonesia_chatur-0.0.1/src/gempaterkini_chatur/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-27 23:38:48.000000 latest_earth_quake_Indonesia_chatur-0.0.1/src/gempaterkini_chatur/example.py
-drwxrwxrwx   0        0        0        0 2023-04-28 00:20:54.847981 latest_earth_quake_Indonesia_chatur-0.0.1/src/latest_earth_quake_Indonesia_chatur.egg-info/
--rw-rw-rw-   0        0        0      823 2023-04-28 00:20:54.000000 latest_earth_quake_Indonesia_chatur-0.0.1/src/latest_earth_quake_Indonesia_chatur.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-04-28 00:20:54.000000 latest_earth_quake_Indonesia_chatur-0.0.1/src/latest_earth_quake_Indonesia_chatur.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 00:20:54.000000 latest_earth_quake_Indonesia_chatur-0.0.1/src/latest_earth_quake_Indonesia_chatur.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-28 00:20:54.000000 latest_earth_quake_Indonesia_chatur-0.0.1/src/latest_earth_quake_Indonesia_chatur.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 00:46:11.433776 latest_earth_quake_Indonesia_chatur-0.0.2/
+-rw-rw-rw-   0        0        0    35823 2023-04-27 00:11:05.000000 latest_earth_quake_Indonesia_chatur-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      823 2023-04-28 00:46:11.432776 latest_earth_quake_Indonesia_chatur-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2023-04-27 00:17:07.000000 latest_earth_quake_Indonesia_chatur-0.0.2/README.md
+-rw-rw-rw-   0        0        0      636 2023-04-28 00:44:59.000000 latest_earth_quake_Indonesia_chatur-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-28 00:46:11.434776 latest_earth_quake_Indonesia_chatur-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 00:46:11.388844 latest_earth_quake_Indonesia_chatur-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 00:46:11.401775 latest_earth_quake_Indonesia_chatur-0.0.2/src/gempaterkini_chatur/
+-rw-rw-rw-   0        0        0     2757 2023-04-28 00:44:40.000000 latest_earth_quake_Indonesia_chatur-0.0.2/src/gempaterkini_chatur/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 23:38:48.000000 latest_earth_quake_Indonesia_chatur-0.0.2/src/gempaterkini_chatur/example.py
+drwxrwxrwx   0        0        0        0 2023-04-28 00:46:11.428777 latest_earth_quake_Indonesia_chatur-0.0.2/src/latest_earth_quake_Indonesia_chatur.egg-info/
+-rw-rw-rw-   0        0        0      823 2023-04-28 00:46:11.000000 latest_earth_quake_Indonesia_chatur-0.0.2/src/latest_earth_quake_Indonesia_chatur.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-04-28 00:46:11.000000 latest_earth_quake_Indonesia_chatur-0.0.2/src/latest_earth_quake_Indonesia_chatur.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 00:46:11.000000 latest_earth_quake_Indonesia_chatur-0.0.2/src/latest_earth_quake_Indonesia_chatur.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-28 00:46:11.000000 latest_earth_quake_Indonesia_chatur-0.0.2/src/latest_earth_quake_Indonesia_chatur.egg-info/top_level.txt
```

### Comparing `latest_earth_quake_Indonesia_chatur-0.0.1/LICENSE` & `latest_earth_quake_Indonesia_chatur-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `latest_earth_quake_Indonesia_chatur-0.0.1/PKG-INFO` & `latest_earth_quake_Indonesia_chatur-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latest_earth_quake_Indonesia_chatur
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package will get the latest earthquake (Indonesia) from https://www.bmkg.go.id/ BMKG
 Author-email: Chatur Agus Priyono <chatur.agus.priyono@gmail.com>
 Project-URL: Homepage, https://github.com/chaturap/bmkg-latest-earthquake
 Project-URL: Bug Tracker, https://github.com/chaturap/bmkg-latest-earthquake/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `latest_earth_quake_Indonesia_chatur-0.0.1/pyproject.toml` & `latest_earth_quake_Indonesia_chatur-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "latest_earth_quake_Indonesia_chatur"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Chatur Agus Priyono", email="chatur.agus.priyono@gmail.com" },
 ]
 description = "This package will get the latest earthquake (Indonesia) from https://www.bmkg.go.id/ BMKG"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `latest_earth_quake_Indonesia_chatur-0.0.1/src/gempaterkini_chatur/__init__.py` & `latest_earth_quake_Indonesia_chatur-0.0.2/src/gempaterkini_chatur/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     print(content.status_code)
     if content.status_code == 200:
         #print(content.text)
 
         soup = BeautifulSoup(content.text, 'html.parser')
         result = soup.find('div', {'class': 'col-md-6 col-xs-6 gempabumi-detail no-padding'})
         result = result.findChildren('li')
-        print(result)
+        #print(result)
 
         magnitudo = None
         kedalaman = None
         koordinat = None
         lintang = None
         bujur = None
         lokasi = None
@@ -59,15 +59,14 @@
 
         title = soup.find('title')
         tanggal = soup.find('span', {'class': 'waktu'})
         waktu = tanggal.text.split(', ')[1]
         tanggal = tanggal.text.split(', ')[0]
 
         print(title.string)
-        #print(soup.prettify())
 
         hasil = dict()
         hasil['tanggal'] = tanggal
         hasil['waktu'] = waktu
         hasil['magnitudo'] = magnitudo
         hasil['kedalaman'] = kedalaman
         hasil['koordinat'] = koordinat
```

### Comparing `latest_earth_quake_Indonesia_chatur-0.0.1/src/latest_earth_quake_Indonesia_chatur.egg-info/PKG-INFO` & `latest_earth_quake_Indonesia_chatur-0.0.2/src/latest_earth_quake_Indonesia_chatur.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latest-earth-quake-Indonesia-chatur
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package will get the latest earthquake (Indonesia) from https://www.bmkg.go.id/ BMKG
 Author-email: Chatur Agus Priyono <chatur.agus.priyono@gmail.com>
 Project-URL: Homepage, https://github.com/chaturap/bmkg-latest-earthquake
 Project-URL: Bug Tracker, https://github.com/chaturap/bmkg-latest-earthquake/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

