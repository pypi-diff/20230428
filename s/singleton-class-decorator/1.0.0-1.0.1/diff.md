# Comparing `tmp/singleton-class-decorator-1.0.0.tar.gz` & `tmp/singleton-class-decorator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singleton-class-decorator-1.0.0.tar", last modified: Fri Apr 28 05:41:10 2023, max compression
+gzip compressed data, was "singleton-class-decorator-1.0.1.tar", last modified: Fri Apr 28 06:10:58 2023, max compression
```

## Comparing `singleton-class-decorator-1.0.0.tar` & `singleton-class-decorator-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-04-28 05:41:10.993867 singleton-class-decorator-1.0.0/
--rw-r--r--   0 jeremy     (501) staff       (20)     1071 2023-01-12 15:46:35.000000 singleton-class-decorator-1.0.0/LICENSE
--rw-r--r--   0 jeremy     (501) staff       (20)     5482 2023-04-28 05:41:10.993610 singleton-class-decorator-1.0.0/PKG-INFO
--rw-r--r--   0 jeremy     (501) staff       (20)     3908 2023-04-28 05:38:40.000000 singleton-class-decorator-1.0.0/README.md
--rw-r--r--   0 jeremy     (501) staff       (20)        6 2023-04-21 14:55:52.000000 singleton-class-decorator-1.0.0/VERSION.md
--rw-r--r--   0 jeremy     (501) staff       (20)      503 2023-04-28 05:33:14.000000 singleton-class-decorator-1.0.0/pyproject.toml
--rw-r--r--   0 jeremy     (501) staff       (20)       38 2023-04-28 05:41:10.993926 singleton-class-decorator-1.0.0/setup.cfg
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-04-28 05:41:10.991817 singleton-class-decorator-1.0.0/singleton_class_decorator/
--rw-r--r--   0 jeremy     (501) staff       (20)     3498 2023-03-06 06:48:37.000000 singleton-class-decorator-1.0.0/singleton_class_decorator/MetaClasses.py
--rw-r--r--   0 jeremy     (501) staff       (20)        0 2023-01-12 16:01:21.000000 singleton-class-decorator-1.0.0/singleton_class_decorator/__init__.py
--rw-r--r--   0 jeremy     (501) staff       (20)     1316 2023-02-22 07:11:33.000000 singleton-class-decorator-1.0.0/singleton_class_decorator/singleton.py
--rw-r--r--   0 jeremy     (501) staff       (20)      793 2023-02-22 07:11:33.000000 singleton-class-decorator-1.0.0/singleton_class_decorator/utils.py
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-04-28 05:41:10.992569 singleton-class-decorator-1.0.0/singleton_class_decorator.egg-info/
--rw-r--r--   0 jeremy     (501) staff       (20)     5482 2023-04-28 05:41:10.000000 singleton-class-decorator-1.0.0/singleton_class_decorator.egg-info/PKG-INFO
--rw-r--r--   0 jeremy     (501) staff       (20)      443 2023-04-28 05:41:10.000000 singleton-class-decorator-1.0.0/singleton_class_decorator.egg-info/SOURCES.txt
--rw-r--r--   0 jeremy     (501) staff       (20)        1 2023-04-28 05:41:10.000000 singleton-class-decorator-1.0.0/singleton_class_decorator.egg-info/dependency_links.txt
--rw-r--r--   0 jeremy     (501) staff       (20)       26 2023-04-28 05:41:10.000000 singleton-class-decorator-1.0.0/singleton_class_decorator.egg-info/top_level.txt
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-04-28 05:41:10.993223 singleton-class-decorator-1.0.0/tests/
--rw-r--r--   0 jeremy     (501) staff       (20)     2061 2023-01-12 16:01:21.000000 singleton-class-decorator-1.0.0/tests/test_meta_classes.py
--rw-r--r--   0 jeremy     (501) staff       (20)     4586 2023-02-08 07:30:36.000000 singleton-class-decorator-1.0.0/tests/test_singleton.py
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-04-28 06:10:58.304340 singleton-class-decorator-1.0.1/
+-rw-r--r--   0 jeremy     (501) staff       (20)     1071 2023-01-12 15:46:35.000000 singleton-class-decorator-1.0.1/LICENSE
+-rw-r--r--   0 jeremy     (501) staff       (20)     5652 2023-04-28 06:10:58.304094 singleton-class-decorator-1.0.1/PKG-INFO
+-rw-r--r--   0 jeremy     (501) staff       (20)     4078 2023-04-28 06:06:12.000000 singleton-class-decorator-1.0.1/README.md
+-rw-r--r--   0 jeremy     (501) staff       (20)        6 2023-04-28 06:06:46.000000 singleton-class-decorator-1.0.1/VERSION.md
+-rw-r--r--   0 jeremy     (501) staff       (20)      503 2023-04-28 05:33:14.000000 singleton-class-decorator-1.0.1/pyproject.toml
+-rw-r--r--   0 jeremy     (501) staff       (20)       38 2023-04-28 06:10:58.304404 singleton-class-decorator-1.0.1/setup.cfg
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-04-28 06:10:58.302089 singleton-class-decorator-1.0.1/singleton_class_decorator/
+-rw-r--r--   0 jeremy     (501) staff       (20)     3498 2023-03-06 06:48:37.000000 singleton-class-decorator-1.0.1/singleton_class_decorator/MetaClasses.py
+-rw-r--r--   0 jeremy     (501) staff       (20)       58 2023-04-28 06:06:12.000000 singleton-class-decorator-1.0.1/singleton_class_decorator/__init__.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     1316 2023-02-22 07:11:33.000000 singleton-class-decorator-1.0.1/singleton_class_decorator/singleton.py
+-rw-r--r--   0 jeremy     (501) staff       (20)      793 2023-02-22 07:11:33.000000 singleton-class-decorator-1.0.1/singleton_class_decorator/utils.py
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-04-28 06:10:58.303049 singleton-class-decorator-1.0.1/singleton_class_decorator.egg-info/
+-rw-r--r--   0 jeremy     (501) staff       (20)     5652 2023-04-28 06:10:58.000000 singleton-class-decorator-1.0.1/singleton_class_decorator.egg-info/PKG-INFO
+-rw-r--r--   0 jeremy     (501) staff       (20)      443 2023-04-28 06:10:58.000000 singleton-class-decorator-1.0.1/singleton_class_decorator.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)        1 2023-04-28 06:10:58.000000 singleton-class-decorator-1.0.1/singleton_class_decorator.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)       26 2023-04-28 06:10:58.000000 singleton-class-decorator-1.0.1/singleton_class_decorator.egg-info/top_level.txt
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-04-28 06:10:58.303667 singleton-class-decorator-1.0.1/tests/
+-rw-r--r--   0 jeremy     (501) staff       (20)     2061 2023-01-12 16:01:21.000000 singleton-class-decorator-1.0.1/tests/test_meta_classes.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     4586 2023-02-08 07:30:36.000000 singleton-class-decorator-1.0.1/tests/test_singleton.py
```

### Comparing `singleton-class-decorator-1.0.0/LICENSE` & `singleton-class-decorator-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `singleton-class-decorator-1.0.0/PKG-INFO` & `singleton-class-decorator-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singleton-class-decorator
-Version: 1.0.0
+Version: 1.0.1
 Summary: Singleton Class Decorator
 Author-email: Jeremy Ribeiro <jeremy.d.ribeiro@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Jeremy Ribeiro
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -101,14 +101,20 @@
 # this works fine
 isinstance(obj, MyClass)
 ```
 
 # Usage
 
 
+You can import the singleton class decorator as follows:
+
+```python
+from singleton_class_decorator import singleton
+```
+
 ## Simplest use case
 Here are some usage examples. To make a singleton class you simply need to use the singleton decorator
 on your class as follows:
 
 ```python
 @singleton
 class MyClass:
@@ -135,14 +141,16 @@
 
 ```
 
 ## Enabling Inheritance
 
 The above should work for any class. However, if you try to create a child class from `MyClass` an error will be raised. This is because by default the singleton disables inheritance. 
 ```python
+from singleton_class_decorator import singleton
+
 @singleton
 class MyClass:
     ...
 
 # is equivalent to the following
 
 @singleton(is_final=True)
```

### Comparing `singleton-class-decorator-1.0.0/README.md` & `singleton-class-decorator-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -69,14 +69,20 @@
 # this works fine
 isinstance(obj, MyClass)
 ```
 
 # Usage
 
 
+You can import the singleton class decorator as follows:
+
+```python
+from singleton_class_decorator import singleton
+```
+
 ## Simplest use case
 Here are some usage examples. To make a singleton class you simply need to use the singleton decorator
 on your class as follows:
 
 ```python
 @singleton
 class MyClass:
@@ -103,14 +109,16 @@
 
 ```
 
 ## Enabling Inheritance
 
 The above should work for any class. However, if you try to create a child class from `MyClass` an error will be raised. This is because by default the singleton disables inheritance. 
 ```python
+from singleton_class_decorator import singleton
+
 @singleton
 class MyClass:
     ...
 
 # is equivalent to the following
 
 @singleton(is_final=True)
```

### Comparing `singleton-class-decorator-1.0.0/singleton_class_decorator/MetaClasses.py` & `singleton-class-decorator-1.0.1/singleton_class_decorator/MetaClasses.py`

 * *Files identical despite different names*

### Comparing `singleton-class-decorator-1.0.0/singleton_class_decorator/singleton.py` & `singleton-class-decorator-1.0.1/singleton_class_decorator/singleton.py`

 * *Files identical despite different names*

### Comparing `singleton-class-decorator-1.0.0/singleton_class_decorator/utils.py` & `singleton-class-decorator-1.0.1/singleton_class_decorator/utils.py`

 * *Files identical despite different names*

### Comparing `singleton-class-decorator-1.0.0/singleton_class_decorator.egg-info/PKG-INFO` & `singleton-class-decorator-1.0.1/singleton_class_decorator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singleton-class-decorator
-Version: 1.0.0
+Version: 1.0.1
 Summary: Singleton Class Decorator
 Author-email: Jeremy Ribeiro <jeremy.d.ribeiro@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Jeremy Ribeiro
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -101,14 +101,20 @@
 # this works fine
 isinstance(obj, MyClass)
 ```
 
 # Usage
 
 
+You can import the singleton class decorator as follows:
+
+```python
+from singleton_class_decorator import singleton
+```
+
 ## Simplest use case
 Here are some usage examples. To make a singleton class you simply need to use the singleton decorator
 on your class as follows:
 
 ```python
 @singleton
 class MyClass:
@@ -135,14 +141,16 @@
 
 ```
 
 ## Enabling Inheritance
 
 The above should work for any class. However, if you try to create a child class from `MyClass` an error will be raised. This is because by default the singleton disables inheritance. 
 ```python
+from singleton_class_decorator import singleton
+
 @singleton
 class MyClass:
     ...
 
 # is equivalent to the following
 
 @singleton(is_final=True)
```

### Comparing `singleton-class-decorator-1.0.0/tests/test_meta_classes.py` & `singleton-class-decorator-1.0.1/tests/test_meta_classes.py`

 * *Files identical despite different names*

### Comparing `singleton-class-decorator-1.0.0/tests/test_singleton.py` & `singleton-class-decorator-1.0.1/tests/test_singleton.py`

 * *Files identical despite different names*

