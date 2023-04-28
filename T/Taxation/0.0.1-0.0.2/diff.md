# Comparing `tmp/Taxation-0.0.1.tar.gz` & `tmp/Taxation-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Taxation-0.0.1.tar", last modified: Fri Apr 28 09:20:56 2023, max compression
+gzip compressed data, was "Taxation-0.0.2.tar", last modified: Fri Apr 28 09:24:49 2023, max compression
```

## Comparing `Taxation-0.0.1.tar` & `Taxation-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-04-28 09:20:56.304365 Taxation-0.0.1/
--rw-r--r--   0 akshay     (501) staff       (20)       77 2023-04-26 07:11:04.000000 Taxation-0.0.1/CHANGELOG.txt
--rw-r--r--   0 akshay     (501) staff       (20)     1075 2023-04-28 09:19:49.000000 Taxation-0.0.1/LICENCE.txt
--rw-r--r--   0 akshay     (501) staff       (20)       25 2023-04-26 06:35:28.000000 Taxation-0.0.1/MANIFEST.in
--rw-r--r--   0 akshay     (501) staff       (20)      679 2023-04-28 09:20:56.304236 Taxation-0.0.1/PKG-INFO
--rw-r--r--   0 akshay     (501) staff       (20)      122 2023-04-28 09:18:57.000000 Taxation-0.0.1/README.txt
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-04-28 09:20:56.303620 Taxation-0.0.1/Taxation.egg-info/
--rw-r--r--   0 akshay     (501) staff       (20)      679 2023-04-28 09:20:56.000000 Taxation-0.0.1/Taxation.egg-info/PKG-INFO
--rw-r--r--   0 akshay     (501) staff       (20)      268 2023-04-28 09:20:56.000000 Taxation-0.0.1/Taxation.egg-info/SOURCES.txt
--rw-r--r--   0 akshay     (501) staff       (20)        1 2023-04-28 09:20:56.000000 Taxation-0.0.1/Taxation.egg-info/dependency_links.txt
--rw-r--r--   0 akshay     (501) staff       (20)       24 2023-04-28 09:20:56.000000 Taxation-0.0.1/Taxation.egg-info/top_level.txt
--rw-r--r--   0 akshay     (501) staff       (20)       38 2023-04-28 09:20:56.304409 Taxation-0.0.1/setup.cfg
--rw-r--r--   0 akshay     (501) staff       (20)      668 2023-04-28 09:19:20.000000 Taxation-0.0.1/setup.py
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-04-28 09:20:56.303881 Taxation-0.0.1/taxation_properties_pkg/
--rw-r--r--   0 akshay     (501) staff       (20)        0 2023-04-26 07:32:40.000000 Taxation-0.0.1/taxation_properties_pkg/__init__.py
--rw-r--r--   0 akshay     (501) staff       (20)      211 2023-04-28 09:20:04.000000 Taxation-0.0.1/taxation_properties_pkg/taxation_properties.py
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-04-28 09:24:49.316733 Taxation-0.0.2/
+-rw-r--r--   0 akshay     (501) staff       (20)       77 2023-04-26 07:11:04.000000 Taxation-0.0.2/CHANGELOG.txt
+-rw-r--r--   0 akshay     (501) staff       (20)     1076 2023-04-28 09:23:31.000000 Taxation-0.0.2/LICENCE.txt
+-rw-r--r--   0 akshay     (501) staff       (20)       25 2023-04-26 06:35:28.000000 Taxation-0.0.2/MANIFEST.in
+-rw-r--r--   0 akshay     (501) staff       (20)      680 2023-04-28 09:24:49.316597 Taxation-0.0.2/PKG-INFO
+-rw-r--r--   0 akshay     (501) staff       (20)      122 2023-04-28 09:18:57.000000 Taxation-0.0.2/README.txt
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-04-28 09:24:49.316105 Taxation-0.0.2/Taxation.egg-info/
+-rw-r--r--   0 akshay     (501) staff       (20)      680 2023-04-28 09:24:49.000000 Taxation-0.0.2/Taxation.egg-info/PKG-INFO
+-rw-r--r--   0 akshay     (501) staff       (20)      268 2023-04-28 09:24:49.000000 Taxation-0.0.2/Taxation.egg-info/SOURCES.txt
+-rw-r--r--   0 akshay     (501) staff       (20)        1 2023-04-28 09:24:49.000000 Taxation-0.0.2/Taxation.egg-info/dependency_links.txt
+-rw-r--r--   0 akshay     (501) staff       (20)       24 2023-04-28 09:24:49.000000 Taxation-0.0.2/Taxation.egg-info/top_level.txt
+-rw-r--r--   0 akshay     (501) staff       (20)       38 2023-04-28 09:24:49.316776 Taxation-0.0.2/setup.cfg
+-rw-r--r--   0 akshay     (501) staff       (20)      669 2023-04-28 09:24:42.000000 Taxation-0.0.2/setup.py
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-04-28 09:24:49.316402 Taxation-0.0.2/taxation_properties_pkg/
+-rw-r--r--   0 akshay     (501) staff       (20)        0 2023-04-26 07:32:40.000000 Taxation-0.0.2/taxation_properties_pkg/__init__.py
+-rw-r--r--   0 akshay     (501) staff       (20)      211 2023-04-28 09:20:04.000000 Taxation-0.0.2/taxation_properties_pkg/taxation_properties.py
```

### Comparing `Taxation-0.0.1/LICENCE.txt` & `Taxation-0.0.2/LICENCE.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 Begin license text.
 
-Copyright 2023 Rishab
+Copyright 2023 Rishabh
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `Taxation-0.0.1/PKG-INFO` & `Taxation-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Taxation
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is very simple tax calculator
 Home-page: 
-Author: Rishab 
+Author: Rishabh 
 Author-email: x21171203@student.ncirl.ie
 License: MIT
 Keywords: Taxation,Tax calculator
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: MacOS
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Taxation-0.0.1/Taxation.egg-info/PKG-INFO` & `Taxation-0.0.2/Taxation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Taxation
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is very simple tax calculator
 Home-page: 
-Author: Rishab 
+Author: Rishabh 
 Author-email: x21171203@student.ncirl.ie
 License: MIT
 Keywords: Taxation,Tax calculator
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: MacOS
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Taxation-0.0.1/setup.py` & `Taxation-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,19 +6,19 @@
   'Operating System :: MacOS',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3.8'
 ]
  
 setup(
   name='Taxation',
-  version='0.0.1',
+  version='0.0.2',
   description='This is very simple tax calculator',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
-  author='Rishab ',
+  author='Rishabh ',
   author_email='x21171203@student.ncirl.ie',
   license='MIT', 
   classifiers=classifiers,
   keywords='Taxation , Tax calculator', 
   packages=find_packages(),
   install_requires=[''] 
 )
```

