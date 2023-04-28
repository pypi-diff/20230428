# Comparing `tmp/corut_fastapi_tools-0.0.2-py3-none-any.whl.zip` & `tmp/corut_fastapi_tools-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 3825 bytes, number of entries: 6
--rw-r--r--  2.0 unx      968 b- defN 23-Mar-01 12:45 corut_fastapi_tools/__init__.py
--rw-rw-r--  2.0 unx     1093 b- defN 23-Mar-01 21:11 corut_fastapi_tools-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     2692 b- defN 23-Mar-01 21:11 corut_fastapi_tools-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-01 21:11 corut_fastapi_tools-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Mar-01 21:11 corut_fastapi_tools-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      533 b- defN 23-Mar-01 21:11 corut_fastapi_tools-0.0.2.dist-info/RECORD
-6 files, 5398 bytes uncompressed, 2847 bytes compressed:  47.3%
+Zip file size: 5074 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     1161 b- defN 23-Apr-28 19:35 corut_fastapi_tools/__init__.py
+-rw-r--r--  2.0 unx     3119 b- defN 23-Jan-18 07:24 corut_fastapi_tools/_content_types.py
+-rw-rw-r--  2.0 unx     1093 b- defN 23-Apr-28 19:45 corut_fastapi_tools-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2768 b- defN 23-Apr-28 19:45 corut_fastapi_tools-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 19:45 corut_fastapi_tools-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Apr-28 19:45 corut_fastapi_tools-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      628 b- defN 23-Apr-28 19:45 corut_fastapi_tools-0.0.3.dist-info/RECORD
+7 files, 8881 bytes uncompressed, 3946 bytes compressed:  55.6%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
 Filename: corut_fastapi_tools/__init__.py
 Comment: 
 
-Filename: corut_fastapi_tools-0.0.2.dist-info/LICENSE
+Filename: corut_fastapi_tools/_content_types.py
 Comment: 
 
-Filename: corut_fastapi_tools-0.0.2.dist-info/METADATA
+Filename: corut_fastapi_tools-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: corut_fastapi_tools-0.0.2.dist-info/WHEEL
+Filename: corut_fastapi_tools-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: corut_fastapi_tools-0.0.2.dist-info/top_level.txt
+Filename: corut_fastapi_tools-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: corut_fastapi_tools-0.0.2.dist-info/RECORD
+Filename: corut_fastapi_tools-0.0.3.dist-info/top_level.txt
+Comment: 
+
+Filename: corut_fastapi_tools-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## corut_fastapi_tools/__init__.py

```diff
@@ -5,33 +5,40 @@
 It is aimed to get rid of repetitive lines of code by integrating tools
 that use multiple APIs for FastApi and facilitate repetitive operations.
 
 Details will be shared at
 https://www.ibrahimcorut.com/tr/projects/pypi-corut_fastapi_tools.
 """
 
-import importlib_metadata
+import importlib_metadata as _importlib_metadata
+from ._content_types import ALL_TYPES, get_special_content_types
+from ._content_types import APPS, FONTS, IMAGES, SOUNDS, TEXTS, VIDEOS
 
 __all__ = (
-    "__title__",
-    "__summary__",
-    "__uri__",
-    "__version__",
-    "__author__",
-    "__email__",
-    "__license__",
-    "__copyright__",
-)
+    '__author__',
+    '__copyright__',
+    '__email__',
+    '__license__',
+    '__summary__',
+    '__title__',
+    '__uri__',
+    '__version__',
 
-__copyright__ = "Copyright 2023 ibrahim CÖRÜT"
-metadata = importlib_metadata.metadata("corut_fastapi_tools")
-__title__ = metadata["name"]
-__summary__ = metadata["summary"]
-__uri__ = metadata["home-page"]
-__version__ = metadata["version"]
-__author__ = metadata["author"]
-__email__ = metadata["author-email"]
-__license__ = metadata["license"]
+    'ALL_TYPES',
+    'APPS',
+    'FONTS',
+    'IMAGES',
+    'SOUNDS',
+    'TEXTS',
+    'VIDEOS',
+    'get_special_content_types',
+)
 
-if __name__ == '__main__':
-    for _ in __all__:
-        print(f'{_}'.ljust(13), ':', globals().get(_))
+__copyright__ = 'Copyright 2023 ibrahim CÖRÜT'
+metadata = _importlib_metadata.metadata('corut_fastapi_tools')
+__title__ = metadata['name']
+__summary__ = metadata['summary']
+__uri__ = metadata['home-page']
+__version__ = metadata['version']
+__author__ = metadata['author']
+__email__ = metadata['author-email']
+__license__ = metadata['license']
```

## Comparing `corut_fastapi_tools-0.0.2.dist-info/LICENSE` & `corut_fastapi_tools-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `corut_fastapi_tools-0.0.2.dist-info/METADATA` & `corut_fastapi_tools-0.0.3.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corut-fastapi-tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Includes facilitating plugins for Fastapi
 Home-page: https://pypi.org/project/corut_fastapi_tools
 Author: ibrahim CÖRÜT
 Author-email: ibrhmcorut@gmail.com
 License: MIT License
 Project-URL: Documentation, https://www.ibrahimcorut.com/en/projects/pypi-corut_fastapi_tools
 Project-URL: Source Code, https://www.ibrahimcorut.com/en/projects/pypi-corut_fastapi_tools
@@ -14,22 +14,25 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp
+Requires-Dist: aiohttp-retry
 Requires-Dist: asyncpg
 Requires-Dist: boto3
 Requires-Dist: botocore
 Requires-Dist: databases
 Requires-Dist: fastapi
 Requires-Dist: hypercorn
 Requires-Dist: importlib-metadata
 Requires-Dist: openai
+Requires-Dist: openpyxl
 Requires-Dist: pandas
 Requires-Dist: psutil
 Requires-Dist: psycopg2-binary
 Requires-Dist: pydantic
 Requires-Dist: pyjwt
 Requires-Dist: pytest
 Requires-Dist: pytest-html
```

## Comparing `corut_fastapi_tools-0.0.2.dist-info/RECORD` & `corut_fastapi_tools-0.0.3.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,6 +1,7 @@
-corut_fastapi_tools/__init__.py,sha256=LuA7Gahb76y2gwqYpbTUBXm22VUhn6VT2sFPFZ64Myc,968
-corut_fastapi_tools-0.0.2.dist-info/LICENSE,sha256=ZX_WMQQ5bWI_phl-V9VjROO1ua50MjHTKqDqB906AxQ,1093
-corut_fastapi_tools-0.0.2.dist-info/METADATA,sha256=rSX3grkseNHY0nNOA_5K1_4FxPJEkOj8evHn5fcydTo,2692
-corut_fastapi_tools-0.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-corut_fastapi_tools-0.0.2.dist-info/top_level.txt,sha256=SyS-IR2c9xSLfq0UcEtOgMUrQiWlpGaCY1dd-1dM5Xo,20
-corut_fastapi_tools-0.0.2.dist-info/RECORD,,
+corut_fastapi_tools/__init__.py,sha256=xdCv619UKPzAUSbu9B2B-HYH0xlWNBpSAx7m53JkzCc,1161
+corut_fastapi_tools/_content_types.py,sha256=keaB5aMigrtHWzqs10jqmyaLLkHwKOUBOrcpudymxL8,3119
+corut_fastapi_tools-0.0.3.dist-info/LICENSE,sha256=ZX_WMQQ5bWI_phl-V9VjROO1ua50MjHTKqDqB906AxQ,1093
+corut_fastapi_tools-0.0.3.dist-info/METADATA,sha256=U4rwsvegCKLJZaPN5_FFnbWP9z53mX1WWfhbvRtGXIk,2768
+corut_fastapi_tools-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+corut_fastapi_tools-0.0.3.dist-info/top_level.txt,sha256=SyS-IR2c9xSLfq0UcEtOgMUrQiWlpGaCY1dd-1dM5Xo,20
+corut_fastapi_tools-0.0.3.dist-info/RECORD,,
```

