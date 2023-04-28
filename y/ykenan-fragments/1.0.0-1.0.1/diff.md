# Comparing `tmp/ykenan_fragments-1.0.0.tar.gz` & `tmp/ykenan_fragments-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_fragments-1.0.0.tar", last modified: Fri Apr 21 11:51:09 2023, max compression
+gzip compressed data, was "ykenan_fragments-1.0.1.tar", last modified: Fri Apr 28 00:59:02 2023, max compression
```

## Comparing `ykenan_fragments-1.0.0.tar` & `ykenan_fragments-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 11:51:09.769950 ykenan_fragments-1.0.0/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_fragments-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_fragments-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      959 2023-04-21 11:51:09.769950 ykenan_fragments-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      419 2023-04-21 09:42:37.000000 ykenan_fragments-1.0.0/README.md
--rw-rw-rw-   0        0        0      773 2023-04-21 09:40:43.000000 ykenan_fragments-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       51 2023-04-21 09:37:07.000000 ykenan_fragments-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 11:51:09.770951 ykenan_fragments-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 11:51:09.753949 ykenan_fragments-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 11:51:09.761949 ykenan_fragments-1.0.0/src/ykenan_fragments/
--rw-rw-rw-   0        0        0    26965 2023-04-21 11:50:12.000000 ykenan_fragments-1.0.0/src/ykenan_fragments/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:51:09.768950 ykenan_fragments-1.0.0/src/ykenan_fragments.egg-info/
--rw-rw-rw-   0        0        0      959 2023-04-21 11:51:09.000000 ykenan_fragments-1.0.0/src/ykenan_fragments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-04-21 11:51:09.000000 ykenan_fragments-1.0.0/src/ykenan_fragments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 11:51:09.000000 ykenan_fragments-1.0.0/src/ykenan_fragments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-21 11:51:09.000000 ykenan_fragments-1.0.0/src/ykenan_fragments.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-21 11:51:09.000000 ykenan_fragments-1.0.0/src/ykenan_fragments.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 00:59:02.050022 ykenan_fragments-1.0.1/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_fragments-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_fragments-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      964 2023-04-28 00:59:02.050022 ykenan_fragments-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-04-21 11:53:38.000000 ykenan_fragments-1.0.1/README.md
+-rw-rw-rw-   0        0        0      773 2023-04-28 00:53:12.000000 ykenan_fragments-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       51 2023-04-21 09:37:07.000000 ykenan_fragments-1.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 00:59:02.051025 ykenan_fragments-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 00:59:02.027023 ykenan_fragments-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 00:59:02.038024 ykenan_fragments-1.0.1/src/ykenan_fragments/
+-rw-rw-rw-   0        0        0    26955 2023-04-28 00:53:12.000000 ykenan_fragments-1.0.1/src/ykenan_fragments/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 00:59:02.048023 ykenan_fragments-1.0.1/src/ykenan_fragments.egg-info/
+-rw-rw-rw-   0        0        0      964 2023-04-28 00:59:01.000000 ykenan_fragments-1.0.1/src/ykenan_fragments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2023-04-28 00:59:02.000000 ykenan_fragments-1.0.1/src/ykenan_fragments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 00:59:01.000000 ykenan_fragments-1.0.1/src/ykenan_fragments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-28 00:59:01.000000 ykenan_fragments-1.0.1/src/ykenan_fragments.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-28 00:59:02.000000 ykenan_fragments-1.0.1/src/ykenan_fragments.egg-info/top_level.txt
```

### Comparing `ykenan_fragments-1.0.0/LICENSE` & `ykenan_fragments-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.0.0/PKG-INFO` & `ykenan_fragments-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ykenan_fragments
-Version: 1.0.0
+Version: 1.0.1
 Summary: Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_fragments
 Keywords: ykenan,fragments
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ykenan_file
+# ykenan_fragments
 
 > **`Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)`**
 
 This is a simple log package. You can see
 [Github-ykenan_file](https://github.com/YuZhengM/ykenan_fragments)
 [PyPI-ykenan_file](https://pypi.org/project/ykenan-fragments/)
```

### Comparing `ykenan_fragments-1.0.0/pyproject.toml` & `ykenan_fragments-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42", "ykenan-log>=0.2.0", "ykenan-file>=0.1.1", "pandas>=1.5.3"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_fragments"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "fragments"]
 description = "Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `ykenan_fragments-1.0.0/src/ykenan_fragments/__init__.py` & `ykenan_fragments-1.0.1/src/ykenan_fragments/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 import pandas as pd
 from pandas import DataFrame
 from ykenan_log import Logger
 import ykenan_file as yf
 import gzip
 
 
-# log 日志
-
 class GetFragments:
 
     def __init__(self, base_path: str, cp_path: str, GSE: str):
         """
         Form an unordered fragments
         :param base_path: Path to store three files
         :param cp_path: Path to generate unordered fragments files
@@ -140,37 +138,37 @@
         # Obtain all file information under this path
         contents_dict: dict = self.file.entry_contents_dict(path, 1)
         filenames: list = contents_dict["name"]
         barcodes_file: dict = {}
         mtx_file: dict = {}
         peaks_file: dict = {}
         # pick up information
-        self.log.info(f"得到 {path} 三个文件信息")
+        self.log.info(f"Obtain three file information for {path}")
         for filename in filenames:
             filename: str
             # Determine if it is a compressed package
             if filename.endswith(".gz"):
                 if filename.count(self.barcodes_key) > 0:
                     barcodes_file: dict = {
                         "name": filename,
                         "path": contents_dict[filename]
                     }
-                    self.log.info(f"{self.barcodes_key} 文件: {barcodes_file}")
+                    self.log.info(f"{self.barcodes_key} file: {barcodes_file}")
                 elif filename.count(self.mtx_key) > 0:
                     mtx_file: dict = {
                         "name": filename,
                         "path": contents_dict[filename]
                     }
-                    self.log.info(f"{self.mtx_key} 文件: {mtx_file}")
+                    self.log.info(f"{self.mtx_key} file: {mtx_file}")
                 elif filename.count(self.peaks_key) > 0:
                     peaks_file: dict = {
                         "name": filename,
                         "path": contents_dict[filename]
                     }
-                    self.log.info(f"{self.peaks_key} 文件: {peaks_file}")
+                    self.log.info(f"{self.peaks_key} file: {peaks_file}")
         return {
             self.barcodes_key: barcodes_file,
             self.mtx_key: mtx_file,
             self.peaks_key: peaks_file
         }
 
     @staticmethod
@@ -213,19 +211,19 @@
         """
         Form fragments file
         :return:
         """
         # Obtain file information
         files: dict = self.get_files(path)
         # Get Barcodes
-        self.log.info(f"正在获取 {self.barcodes_key} 文件信息")
+        self.log.info(f"Getting {self.barcodes_key} file information")
         barcodes: list = self.get_file_content(path, files[self.barcodes_key])
-        self.log.info(f"正在获取 {self.mtx_key} 文件路径")
+        self.log.info(f"Getting {self.mtx_key} file path")
         mtx_path: str = self.get_file_content(path, files[self.mtx_key])
-        self.log.info(f"正在获取 {self.peaks_key} 文件信息")
+        self.log.info(f"Getting {self.peaks_key} file information")
         peaks: list = self.get_file_content(path, files[self.peaks_key])
         # length
         barcodes_len: int = len(barcodes)
         peaks_len: int = len(peaks)
         if barcodes_len < 2 or peaks_len < 2:
             self.log.error(f"Insufficient file read length {self.barcodes_key}: {barcodes_len}, {self.peaks_key}: {peaks_len}")
             raise ValueError("Insufficient file read length")
@@ -243,20 +241,20 @@
             with open(mtx_path, "r", encoding="utf-8") as r:
                 while True:
                     line: str = r.readline().strip()
                     if not line:
                         break
                     if mtx_count >= 500000 and mtx_count % 500000 == 0:
                         if mtx_all_number != 0:
-                            self.log.info(f"已处理 {mtx_count} 行, 已完成 {round(mtx_count / mtx_all_number, 4) * 100} %")
+                            self.log.info(f"Processed {mtx_count} lines, completed {round(mtx_count / mtx_all_number, 4) * 100} %")
                         else:
-                            self.log.info(f"已处理 {mtx_count} 行")
+                            self.log.info(f"Processed {mtx_count} lines")
                     if line.startswith("%"):
                         mtx_start += 1
-                        self.log.info(f"注释信息: {line}")
+                        self.log.info(f"Annotation Information: {line}")
                         mtx_count += 1
                         continue
                     split: list = line.split(" ")
                     # To determine the removal of a length of not 3
                     if len(split) != 3:
                         mtx_count += 1
                         error_count += 1
```

### Comparing `ykenan_fragments-1.0.0/src/ykenan_fragments.egg-info/PKG-INFO` & `ykenan_fragments-1.0.1/src/ykenan_fragments.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ykenan-fragments
-Version: 1.0.0
+Version: 1.0.1
 Summary: Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_fragments
 Keywords: ykenan,fragments
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ykenan_file
+# ykenan_fragments
 
 > **`Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)`**
 
 This is a simple log package. You can see
 [Github-ykenan_file](https://github.com/YuZhengM/ykenan_fragments)
 [PyPI-ykenan_file](https://pypi.org/project/ykenan-fragments/)
```

