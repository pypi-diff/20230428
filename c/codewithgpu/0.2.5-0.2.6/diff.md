# Comparing `tmp/codewithgpu-0.2.5-py3-none-any.whl.zip` & `tmp/codewithgpu-0.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,31 +1,31 @@
-Zip file size: 35587 bytes, number of entries: 29
+Zip file size: 35503 bytes, number of entries: 29
 -rw-r--r--  2.0 unx     1567 b- defN 23-Apr-25 09:10 codewithgpu/__init__.py
 -rw-r--r--  2.0 unx     1928 b- defN 23-Apr-25 09:34 codewithgpu/cli.py
--rw-r--r--  2.0 unx      185 b- defN 23-Apr-25 09:34 codewithgpu/version.py
+-rw-r--r--  2.0 unx      185 b- defN 23-Apr-28 11:28 codewithgpu/version.py
 -rw-r--r--  2.0 unx      746 b- defN 23-Apr-23 11:05 codewithgpu/data/__init__.py
 -rw-r--r--  2.0 unx     6547 b- defN 23-Apr-23 11:05 codewithgpu/data/dataset.py
 -rw-r--r--  2.0 unx     7177 b- defN 23-Apr-23 11:05 codewithgpu/data/reader.py
 -rw-r--r--  2.0 unx      608 b- defN 23-Apr-23 11:05 codewithgpu/data/record.proto
 -rw-r--r--  2.0 unx     8941 b- defN 23-Apr-23 11:05 codewithgpu/data/record.py
 -rw-r--r--  2.0 unx    10202 b- defN 23-Apr-23 11:05 codewithgpu/data/record_pb2.py
 -rw-r--r--  2.0 unx      780 b- defN 23-Apr-23 11:05 codewithgpu/data/tf_record.proto
 -rw-r--r--  2.0 unx     7299 b- defN 23-Apr-23 11:05 codewithgpu/data/tf_record.py
 -rw-r--r--  2.0 unx    11900 b- defN 23-Apr-23 11:05 codewithgpu/data/tf_record_pb2.py
 -rw-r--r--  2.0 unx      746 b- defN 23-Apr-23 11:05 codewithgpu/inference/__init__.py
 -rw-r--r--  2.0 unx     6128 b- defN 23-Apr-23 11:05 codewithgpu/inference/command.py
 -rw-r--r--  2.0 unx     1474 b- defN 23-Apr-23 11:05 codewithgpu/inference/module.py
 -rw-r--r--  2.0 unx      810 b- defN 23-Apr-25 09:10 codewithgpu/model/__init__.py
--rw-r--r--  2.0 unx     1418 b- defN 23-Apr-23 11:05 codewithgpu/model/download.py
+-rw-r--r--  2.0 unx     1251 b- defN 23-Apr-28 11:28 codewithgpu/model/download.py
 -rw-r--r--  2.0 unx      746 b- defN 23-Apr-23 11:05 codewithgpu/utils/__init__.py
 -rw-r--r--  2.0 unx     4076 b- defN 23-Apr-23 11:05 codewithgpu/utils/cg_cli.py
 -rw-r--r--  2.0 unx     3805 b- defN 23-Apr-23 11:05 codewithgpu/utils/decorator.py
 -rw-r--r--  2.0 unx     3629 b- defN 23-Apr-23 11:05 codewithgpu/utils/deprecation.py
 -rw-r--r--  2.0 unx     3741 b- defN 23-Apr-21 09:27 codewithgpu/utils/logging.py
 -rw-r--r--  2.0 unx     1226 b- defN 23-Apr-21 09:27 codewithgpu/utils/unittest_util.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-25 09:34 codewithgpu-0.2.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     3033 b- defN 23-Apr-25 09:34 codewithgpu-0.2.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 09:34 codewithgpu-0.2.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 23-Apr-25 09:34 codewithgpu-0.2.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       87 b- defN 23-Apr-25 09:34 codewithgpu-0.2.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2469 b- defN 23-Apr-25 09:34 codewithgpu-0.2.5.dist-info/RECORD
-29 files, 102766 bytes uncompressed, 31601 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-28 11:28 codewithgpu-0.2.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3033 b- defN 23-Apr-28 11:28 codewithgpu-0.2.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 11:28 codewithgpu-0.2.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 23-Apr-28 11:28 codewithgpu-0.2.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       87 b- defN 23-Apr-28 11:28 codewithgpu-0.2.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2469 b- defN 23-Apr-28 11:28 codewithgpu-0.2.6.dist-info/RECORD
+29 files, 102599 bytes uncompressed, 31517 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -63,26 +63,26 @@
 
 Filename: codewithgpu/utils/logging.py
 Comment: 
 
 Filename: codewithgpu/utils/unittest_util.py
 Comment: 
 
-Filename: codewithgpu-0.2.5.dist-info/LICENSE
+Filename: codewithgpu-0.2.6.dist-info/LICENSE
 Comment: 
 
-Filename: codewithgpu-0.2.5.dist-info/METADATA
+Filename: codewithgpu-0.2.6.dist-info/METADATA
 Comment: 
 
-Filename: codewithgpu-0.2.5.dist-info/WHEEL
+Filename: codewithgpu-0.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: codewithgpu-0.2.5.dist-info/entry_points.txt
+Filename: codewithgpu-0.2.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: codewithgpu-0.2.5.dist-info/top_level.txt
+Filename: codewithgpu-0.2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: codewithgpu-0.2.5.dist-info/RECORD
+Filename: codewithgpu-0.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## codewithgpu/version.py

```diff
@@ -1,6 +1,6 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
-version = '0.2.5'
-git_version = '3539e7879467c3ceb1bd80a2c93430c41c914499'
+version = '0.2.6'
+git_version = '73bcee4c6c317195eee85556470c5b9763d000bc'
```

## codewithgpu/model/download.py

```diff
@@ -15,17 +15,14 @@
 # ------------------------------------------------------------------------
 
 from codewithgpu.utils.cg_cli import get_os_config
 import os
 
 
 def download(model_name, target_directory=None):
-    if len(model_name.split("/")) < 2:
-        print("ERROR: model name `{}` format invalid. should be <model_name>/<file_name>".format(model_name))
-        return
     if target_directory is None or target_directory == "":
         target_directory = os.getcwd()
     else:
         if not os.path.exists(target_directory):
             os.makedirs(target_directory)
     os_config = get_os_config()
     os_config.download(model_name, target_directory)
```

## Comparing `codewithgpu-0.2.5.dist-info/LICENSE` & `codewithgpu-0.2.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `codewithgpu-0.2.5.dist-info/METADATA` & `codewithgpu-0.2.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codewithgpu
-Version: 0.2.5
+Version: 0.2.6
 Summary: CodeWithGPU Python Client
 Home-page: https://github.com/seetacloud/codewithgpu
 Author: SeetaCloud
 License: Apache License
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: codewithgpu Version: 0.2.5 Summary: CodeWithGPU
+Metadata-Version: 2.1 Name: codewithgpu Version: 0.2.6 Summary: CodeWithGPU
 Python Client Home-page: https://github.com/seetacloud/codewithgpu Author:
 SeetaCloud License: Apache License Platform: UNKNOWN Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: C++ Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
```

## Comparing `codewithgpu-0.2.5.dist-info/RECORD` & `codewithgpu-0.2.6.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 codewithgpu/__init__.py,sha256=H8d6hU-w9tDFMvwdC2X4XzpUjs5EX6UhHs0o5mJnzOE,1567
 codewithgpu/cli.py,sha256=hXeleJlGfEgZTgmz6u3MIH2tXwX-fZAzmwhWah8GcAE,1928
-codewithgpu/version.py,sha256=s7HAjRyO4ZYoa8uhBqjD3L6I4OYUSBxe8QzOsKsuJFA,185
+codewithgpu/version.py,sha256=ED7vO1g1cg9LTmK_KlPop53O945muhEbKXdHy6Aqh1s,185
 codewithgpu/data/__init__.py,sha256=BS1ku8WVrSQXgBXqv0day5ZxbstsOQbW5bWQjyVjoOs,746
 codewithgpu/data/dataset.py,sha256=lhm1KAR12xb3-AUtHWvYjhPEytL3ozpIY6RDVdsr_Wc,6547
 codewithgpu/data/reader.py,sha256=obDLYyFvZf0WxXdeDMYwqsS14vgXPKvvIxRv7vfA-HE,7177
 codewithgpu/data/record.proto,sha256=mToQiLJ9idcmEoaKwEbCNffe1Cv4ZcNoUhyW2oTvw-Y,608
 codewithgpu/data/record.py,sha256=xD53qMX1UWAXrOemlhXuiYZfHxbw0lXGUDof9IsRbfM,8941
 codewithgpu/data/record_pb2.py,sha256=0eygLJUOK3KKsQXBOBbwB-wh-kMQW5Z35ZMAVs0vlsA,10202
 codewithgpu/data/tf_record.proto,sha256=iA-8rb9uDY6g-FFcpAsHW3He1Djc_pRzKXjtk2V3UlI,780
 codewithgpu/data/tf_record.py,sha256=VTfBgEpuvsrSH42irj8Q8DySrJQQet29tLc7hrOk6rk,7299
 codewithgpu/data/tf_record_pb2.py,sha256=OMgulDnqXpDArdyHnI32yy_EOvNggWcOl779grQJ838,11900
 codewithgpu/inference/__init__.py,sha256=BS1ku8WVrSQXgBXqv0day5ZxbstsOQbW5bWQjyVjoOs,746
 codewithgpu/inference/command.py,sha256=7RUMuMQqGLZXc398OtmZmuSuUuc4bfF_uO1cEblNyf0,6128
 codewithgpu/inference/module.py,sha256=59dLqKDfK5D5a3CyvtpKy1X9Osp4F0Bxg7WyVU_0bgw,1474
 codewithgpu/model/__init__.py,sha256=OK5APRO8AeMQraAyfBfiftMooDXz-NLezQYc3zj8qE4,810
-codewithgpu/model/download.py,sha256=-SJ7EPqkKYEQTmIQCezDfLgx6YKtPoWuoxbfyTCu89A,1418
+codewithgpu/model/download.py,sha256=eYeF64E2QqfJN21CwtbCLNC4HJTY-7Q3LZcv6MKoC1Q,1251
 codewithgpu/utils/__init__.py,sha256=BS1ku8WVrSQXgBXqv0day5ZxbstsOQbW5bWQjyVjoOs,746
 codewithgpu/utils/cg_cli.py,sha256=3Urv0uigHTPjfRF4EdSrk1hQbloCIUlgahe3ymL0pdo,4076
 codewithgpu/utils/decorator.py,sha256=eavLk-cu8K9kiTNquJjAwVIziQ2-dG23aFTe3i_1Vkk,3805
 codewithgpu/utils/deprecation.py,sha256=JNzJijpwuXdu9nf4pOzlLqmFvrCM__JZRy5zVU_Xkk8,3629
 codewithgpu/utils/logging.py,sha256=psQyhYN4RRfhcohMvOMIRb2SEsfsRzk3rQzhelhGjgI,3741
 codewithgpu/utils/unittest_util.py,sha256=jz2HVLIHe_TlrQ9QJ-HOg0Erf-QEVmfuQDo0Q4BkfDw,1226
-codewithgpu-0.2.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-codewithgpu-0.2.5.dist-info/METADATA,sha256=7G6Kp71GA-l_GdrJLyKOE044KH8S7YVNmbSeLNgfP7I,3033
-codewithgpu-0.2.5.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-codewithgpu-0.2.5.dist-info/entry_points.txt,sha256=uIKsOHrbYlsA2As8st4u2hBbCA5pGUjKwJuRJUpK0MQ,49
-codewithgpu-0.2.5.dist-info/top_level.txt,sha256=orLQMHWZMLDPkZO_r-8233w9F1YzYk6xqY7Oti5-P4s,87
-codewithgpu-0.2.5.dist-info/RECORD,,
+codewithgpu-0.2.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+codewithgpu-0.2.6.dist-info/METADATA,sha256=KSwznmovedABrhDi7eiXBjvICYDC2rGh2DY6_tWh78Y,3033
+codewithgpu-0.2.6.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+codewithgpu-0.2.6.dist-info/entry_points.txt,sha256=uIKsOHrbYlsA2As8st4u2hBbCA5pGUjKwJuRJUpK0MQ,49
+codewithgpu-0.2.6.dist-info/top_level.txt,sha256=orLQMHWZMLDPkZO_r-8233w9F1YzYk6xqY7Oti5-P4s,87
+codewithgpu-0.2.6.dist-info/RECORD,,
```

