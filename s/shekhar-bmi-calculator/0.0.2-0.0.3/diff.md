# Comparing `tmp/shekhar_bmi_calculator-0.0.2.tar.gz` & `tmp/shekhar_bmi_calculator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shekhar_bmi_calculator-0.0.2.tar", last modified: Wed Apr 26 23:28:03 2023, max compression
+gzip compressed data, was "shekhar_bmi_calculator-0.0.3.tar", last modified: Fri Apr 28 00:31:55 2023, max compression
```

## Comparing `shekhar_bmi_calculator-0.0.2.tar` & `shekhar_bmi_calculator-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 23:28:03.783907 shekhar_bmi_calculator-0.0.2/
--rw-rw-rw-   0        0        0       77 2023-04-26 23:15:11.000000 shekhar_bmi_calculator-0.0.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1084 2023-04-23 15:30:11.000000 shekhar_bmi_calculator-0.0.2/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-04-22 07:23:08.000000 shekhar_bmi_calculator-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      940 2023-04-26 23:28:03.781891 shekhar_bmi_calculator-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-04-23 15:30:09.000000 shekhar_bmi_calculator-0.0.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-26 23:28:03.743800 shekhar_bmi_calculator-0.0.2/bmi_calculator/
--rw-rw-rw-   0        0        0        0 2023-04-26 23:15:14.000000 shekhar_bmi_calculator-0.0.2/bmi_calculator/__init__.py
--rw-rw-rw-   0        0        0       75 2023-04-26 23:15:13.000000 shekhar_bmi_calculator-0.0.2/bmi_calculator/bmi_calculator.py
--rw-rw-rw-   0        0        0       42 2023-04-26 23:28:03.783907 shekhar_bmi_calculator-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      701 2023-04-26 23:27:43.000000 shekhar_bmi_calculator-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 23:28:03.779688 shekhar_bmi_calculator-0.0.2/shekhar_bmi_calculator.egg-info/
--rw-rw-rw-   0        0        0      940 2023-04-26 23:28:03.000000 shekhar_bmi_calculator-0.0.2/shekhar_bmi_calculator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2023-04-26 23:28:03.000000 shekhar_bmi_calculator-0.0.2/shekhar_bmi_calculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 23:28:03.000000 shekhar_bmi_calculator-0.0.2/shekhar_bmi_calculator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-26 23:28:03.000000 shekhar_bmi_calculator-0.0.2/shekhar_bmi_calculator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 00:31:55.722592 shekhar_bmi_calculator-0.0.3/
+-rw-rw-rw-   0        0        0       77 2023-04-26 23:15:11.000000 shekhar_bmi_calculator-0.0.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1084 2023-04-23 15:30:11.000000 shekhar_bmi_calculator-0.0.3/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-22 07:23:08.000000 shekhar_bmi_calculator-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      940 2023-04-28 00:31:55.722592 shekhar_bmi_calculator-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-04-23 15:30:09.000000 shekhar_bmi_calculator-0.0.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 00:31:55.706452 shekhar_bmi_calculator-0.0.3/bmi_calculator/
+-rw-rw-rw-   0        0        0        0 2023-04-26 23:15:14.000000 shekhar_bmi_calculator-0.0.3/bmi_calculator/__init__.py
+-rw-rw-rw-   0        0        0      104 2023-04-28 00:26:12.000000 shekhar_bmi_calculator-0.0.3/bmi_calculator/bmi_calculator.py
+-rw-rw-rw-   0        0        0       42 2023-04-28 00:31:55.722592 shekhar_bmi_calculator-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      701 2023-04-28 00:31:04.000000 shekhar_bmi_calculator-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 00:31:55.721584 shekhar_bmi_calculator-0.0.3/shekhar_bmi_calculator.egg-info/
+-rw-rw-rw-   0        0        0      940 2023-04-28 00:31:55.000000 shekhar_bmi_calculator-0.0.3/shekhar_bmi_calculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-04-28 00:31:55.000000 shekhar_bmi_calculator-0.0.3/shekhar_bmi_calculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 00:31:55.000000 shekhar_bmi_calculator-0.0.3/shekhar_bmi_calculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-28 00:31:55.000000 shekhar_bmi_calculator-0.0.3/shekhar_bmi_calculator.egg-info/top_level.txt
```

### Comparing `shekhar_bmi_calculator-0.0.2/LICENCE.txt` & `shekhar_bmi_calculator-0.0.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `shekhar_bmi_calculator-0.0.2/PKG-INFO` & `shekhar_bmi_calculator-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shekhar_bmi_calculator
-Version: 0.0.2
+Version: 0.0.3
 Summary: A very basic BMI calculator
 Home-page: 
 Author: Sarvesh Shekhar
 Author-email: x22129880@student.ncirl.ie
 License: MIT
 Keywords: bmi calculator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `shekhar_bmi_calculator-0.0.2/setup.py` & `shekhar_bmi_calculator-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3.8'
 ]
  
 setup(
   name='shekhar_bmi_calculator',
-  version='0.0.2',
+  version='0.0.3',
   description='A very basic BMI calculator',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Sarvesh Shekhar',
   author_email='x22129880@student.ncirl.ie',
   license='MIT', 
   classifiers=classifiers,
```

### Comparing `shekhar_bmi_calculator-0.0.2/shekhar_bmi_calculator.egg-info/PKG-INFO` & `shekhar_bmi_calculator-0.0.3/shekhar_bmi_calculator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shekhar-bmi-calculator
-Version: 0.0.2
+Version: 0.0.3
 Summary: A very basic BMI calculator
 Home-page: 
 Author: Sarvesh Shekhar
 Author-email: x22129880@student.ncirl.ie
 License: MIT
 Keywords: bmi calculator
 Classifier: Development Status :: 5 - Production/Stable
```

