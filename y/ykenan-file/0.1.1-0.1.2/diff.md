# Comparing `tmp/ykenan_file-0.1.1.tar.gz` & `tmp/ykenan_file-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_file-0.1.1.tar", last modified: Fri Apr 21 09:36:29 2023, max compression
+gzip compressed data, was "ykenan_file-0.1.2.tar", last modified: Fri Apr 28 06:35:32 2023, max compression
```

## Comparing `ykenan_file-0.1.1.tar` & `ykenan_file-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 09:36:29.723255 ykenan_file-0.1.1/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_file-0.1.1/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_file-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      829 2023-04-21 09:36:29.722255 ykenan_file-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-04-21 09:34:27.000000 ykenan_file-0.1.1/README.md
--rw-rw-rw-   0        0        0      676 2023-04-21 09:34:27.000000 ykenan_file-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       32 2023-03-22 07:40:08.000000 ykenan_file-0.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 09:36:29.723255 ykenan_file-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 09:36:29.704256 ykenan_file-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 09:36:29.713256 ykenan_file-0.1.1/src/ykenan_file/
--rw-rw-rw-   0        0        0    23371 2023-04-21 09:34:27.000000 ykenan_file-0.1.1/src/ykenan_file/__init__.py
--rw-rw-rw-   0        0        0      157 2023-04-06 01:49:10.000000 ykenan_file-0.1.1/src/ykenan_file/util.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:36:29.721255 ykenan_file-0.1.1/src/ykenan_file.egg-info/
--rw-rw-rw-   0        0        0      829 2023-04-21 09:36:29.000000 ykenan_file-0.1.1/src/ykenan_file.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-04-21 09:36:29.000000 ykenan_file-0.1.1/src/ykenan_file.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 09:36:29.000000 ykenan_file-0.1.1/src/ykenan_file.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-21 09:36:29.000000 ykenan_file-0.1.1/src/ykenan_file.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-21 09:36:29.000000 ykenan_file-0.1.1/src/ykenan_file.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 06:35:32.440379 ykenan_file-0.1.2/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_file-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_file-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      829 2023-04-28 06:35:32.439379 ykenan_file-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-04-21 09:34:27.000000 ykenan_file-0.1.2/README.md
+-rw-rw-rw-   0        0        0      676 2023-04-28 06:33:51.000000 ykenan_file-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       32 2023-03-22 07:40:08.000000 ykenan_file-0.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 06:35:32.440379 ykenan_file-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 06:35:32.415381 ykenan_file-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 06:35:32.428381 ykenan_file-0.1.2/src/ykenan_file/
+-rw-rw-rw-   0        0        0    23401 2023-04-28 06:33:22.000000 ykenan_file-0.1.2/src/ykenan_file/__init__.py
+-rw-rw-rw-   0        0        0      157 2023-04-06 01:49:10.000000 ykenan_file-0.1.2/src/ykenan_file/util.py
+drwxrwxrwx   0        0        0        0 2023-04-28 06:35:32.437379 ykenan_file-0.1.2/src/ykenan_file.egg-info/
+-rw-rw-rw-   0        0        0      829 2023-04-28 06:35:32.000000 ykenan_file-0.1.2/src/ykenan_file.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-04-28 06:35:32.000000 ykenan_file-0.1.2/src/ykenan_file.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 06:35:32.000000 ykenan_file-0.1.2/src/ykenan_file.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-28 06:35:32.000000 ykenan_file-0.1.2/src/ykenan_file.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-28 06:35:32.000000 ykenan_file-0.1.2/src/ykenan_file.egg-info/top_level.txt
```

### Comparing `ykenan_file-0.1.1/LICENSE` & `ykenan_file-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_file-0.1.1/PKG-INFO` & `ykenan_file-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan_file
-Version: 0.1.1
+Version: 0.1.2
 Summary: File read and write operations
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_file
 Keywords: ykenan,file,read,write
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ykenan_file-0.1.1/pyproject.toml` & `ykenan_file-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42", "ykenan-log>=0.2.0", "pandas>=1.5.3"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_file"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "file", "read", "write"]
 description = "File read and write operations"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `ykenan_file-0.1.1/src/ykenan_file/__init__.py` & `ykenan_file-0.1.2/src/ykenan_file/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     def to_file(self, df: DataFrame, file: str) -> None:
         """
         :param df: DataFrame
         :param file: File path plus name
         """
         self.log.debug(f"create a file: {file}")
         # 导出文件
-        if str(file).endswith(".txt"):
+        if str(file).endswith(".txt") or str(file).endswith(".bed"):
             df.to_csv(file, sep=self.sep, lineterminator=self.line_terminator, header=self.header, encoding=self.encoding, index=self.index)
         elif str(file).endswith(".csv"):
             df.to_csv(file, sep=',', lineterminator=self.line_terminator, header=self.header, encoding=self.encoding, index=self.index)
         elif str(file).endswith(".xls") or str(file).endswith(".xlsx"):
             df.to_excel(file, sheet_name=self.sheet_name, header=self.header, index=self.index)
         else:
             with open(file, 'w', encoding='UTF-8') as f:
```

### Comparing `ykenan_file-0.1.1/src/ykenan_file.egg-info/PKG-INFO` & `ykenan_file-0.1.2/src/ykenan_file.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan-file
-Version: 0.1.1
+Version: 0.1.2
 Summary: File read and write operations
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_file
 Keywords: ykenan,file,read,write
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

