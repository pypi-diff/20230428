# Comparing `tmp/pydaa-1.6.5-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/pydaa-1.6.8-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 195917 bytes, number of entries: 9
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-27 17:31 pydaa-1.6.5.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-27 17:31 pydaa.libs/
--rwxr-xr-x  2.0 unx   500136 b- defN 23-Apr-27 17:31 pydaa.pypy39-pp73-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      189 b- defN 23-Apr-27 17:31 pydaa.pyi
--rw-r--r--  2.0 unx     1895 b- defN 23-Apr-27 17:31 pydaa-1.6.5.dist-info/METADATA
--rw-r--r--  2.0 unx        6 b- defN 23-Apr-27 17:31 pydaa-1.6.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      554 b- defN 23-Apr-27 17:31 pydaa-1.6.5.dist-info/RECORD
--rw-r--r--  2.0 unx     1684 b- defN 23-Apr-27 17:31 pydaa-1.6.5.dist-info/LICENSE-3RD-PARTY
--rw-r--r--  2.0 unx      162 b- defN 23-Apr-27 17:31 pydaa-1.6.5.dist-info/WHEEL
-9 files, 504626 bytes uncompressed, 194735 bytes compressed:  61.4%
+Zip file size: 195918 bytes, number of entries: 9
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-28 16:05 pydaa-1.6.8.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-28 16:05 pydaa.libs/
+-rwxr-xr-x  2.0 unx   500136 b- defN 23-Apr-28 16:05 pydaa.pypy39-pp73-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      189 b- defN 23-Apr-28 16:05 pydaa.pyi
+-rw-r--r--  2.0 unx     1895 b- defN 23-Apr-28 16:05 pydaa-1.6.8.dist-info/METADATA
+-rw-r--r--  2.0 unx        6 b- defN 23-Apr-28 16:05 pydaa-1.6.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      554 b- defN 23-Apr-28 16:05 pydaa-1.6.8.dist-info/RECORD
+-rw-r--r--  2.0 unx     1684 b- defN 23-Apr-28 16:05 pydaa-1.6.8.dist-info/LICENSE-3RD-PARTY
+-rw-r--r--  2.0 unx      162 b- defN 23-Apr-28 16:05 pydaa-1.6.8.dist-info/WHEEL
+9 files, 504626 bytes uncompressed, 194736 bytes compressed:  61.4%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
-Filename: pydaa-1.6.5.dist-info/
+Filename: pydaa-1.6.8.dist-info/
 Comment: 
 
 Filename: pydaa.libs/
 Comment: 
 
 Filename: pydaa.pypy39-pp73-x86_64-linux-gnu.so
 Comment: 
 
 Filename: pydaa.pyi
 Comment: 
 
-Filename: pydaa-1.6.5.dist-info/METADATA
+Filename: pydaa-1.6.8.dist-info/METADATA
 Comment: 
 
-Filename: pydaa-1.6.5.dist-info/top_level.txt
+Filename: pydaa-1.6.8.dist-info/top_level.txt
 Comment: 
 
-Filename: pydaa-1.6.5.dist-info/RECORD
+Filename: pydaa-1.6.8.dist-info/RECORD
 Comment: 
 
-Filename: pydaa-1.6.5.dist-info/LICENSE-3RD-PARTY
+Filename: pydaa-1.6.8.dist-info/LICENSE-3RD-PARTY
 Comment: 
 
-Filename: pydaa-1.6.5.dist-info/WHEEL
+Filename: pydaa-1.6.8.dist-info/WHEEL
 Comment: 
 
 Zip file comment:
```

## Comparing `pydaa-1.6.5.dist-info/METADATA` & `pydaa-1.6.8.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydaa
-Version: 1.6.5
+Version: 1.6.8
 Summary: python bindings for the daa library
 Home-page: https://github.com/Tomcat-42/pydaa
 Author: Pablo Alessandro Santos Hugen
 Author-email: pablohuggem@gmail.com
 License: Public Domain
 Keywords: daa algorithms data structures sorting searching c++ c++11 c++ module
 Classifier: Development Status :: 4 - Beta
```

## Comparing `pydaa-1.6.5.dist-info/RECORD` & `pydaa-1.6.8.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 pydaa.pypy39-pp73-x86_64-linux-gnu.so,sha256=5txgvqnYZkby3FXbtVVKOOUyVfZ2RNAHDYb5EYVncI4,500136
 pydaa.pyi,sha256=hptll0ujngDWuR25ezx1awjJDgEs9O187HAQXByYTKc,189
-pydaa-1.6.5.dist-info/METADATA,sha256=Tlf7SFe8ZYEXTl3Fv1eLRIgQLg-Sb6EXmSCEXtT1E-0,1895
-pydaa-1.6.5.dist-info/top_level.txt,sha256=uhixZYuky8AgCAOQ7r4IwCNpNrP5xi87OR9pqxT_lcc,6
-pydaa-1.6.5.dist-info/RECORD,,
-pydaa-1.6.5.dist-info/LICENSE-3RD-PARTY,sha256=g5ZbhDuY9nDTqFvQQe1LNyyOxQ17SlmVqDrGl7pnXcs,1684
-pydaa-1.6.5.dist-info/WHEEL,sha256=aIHtXq4XssUHqceM9ZWc7TXyJq4AMH0BhNTZQBcVTZY,162
+pydaa-1.6.8.dist-info/METADATA,sha256=OxlmRx7aUtJlvE8fISHhlUxhOIgegUQxbEMLFeicyG0,1895
+pydaa-1.6.8.dist-info/top_level.txt,sha256=uhixZYuky8AgCAOQ7r4IwCNpNrP5xi87OR9pqxT_lcc,6
+pydaa-1.6.8.dist-info/RECORD,,
+pydaa-1.6.8.dist-info/LICENSE-3RD-PARTY,sha256=g5ZbhDuY9nDTqFvQQe1LNyyOxQ17SlmVqDrGl7pnXcs,1684
+pydaa-1.6.8.dist-info/WHEEL,sha256=aIHtXq4XssUHqceM9ZWc7TXyJq4AMH0BhNTZQBcVTZY,162
```

## Comparing `pydaa-1.6.5.dist-info/LICENSE-3RD-PARTY` & `pydaa-1.6.8.dist-info/LICENSE-3RD-PARTY`

 * *Files identical despite different names*

