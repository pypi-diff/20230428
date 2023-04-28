# Comparing `tmp/pyBCV-1.0.5-py3-none-any.whl.zip` & `tmp/pyBCV-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,11 @@
-Zip file size: 5469 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat       25 b- defN 23-Apr-27 20:51 pyBCV/__init__.py
--rw-rw-rw-  2.0 fat     6493 b- defN 23-Apr-27 20:52 pyBCV/pyBCV.py
--rw-rw-rw-  2.0 fat     1094 b- defN 23-Apr-27 21:10 pyBCV-1.0.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4493 b- defN 23-Apr-27 21:10 pyBCV-1.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-27 21:10 pyBCV-1.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-27 21:10 pyBCV-1.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      518 b- defN 23-Apr-27 21:10 pyBCV-1.0.5.dist-info/RECORD
-7 files, 12721 bytes uncompressed, 4555 bytes compressed:  64.2%
+Zip file size: 6185 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat       25 b- defN 23-Apr-27 21:59 pyBCV/__init__.py
+-rw-rw-rw-  2.0 fat     6498 b- defN 23-Apr-27 21:59 pyBCV/pyBCV.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-27 21:56 pyBCV/core/__init__.py
+-rw-rw-rw-  2.0 fat      856 b- defN 23-Apr-27 20:51 pyBCV/core/requests.py
+-rw-rw-rw-  2.0 fat     1094 b- defN 23-Apr-27 22:03 pyBCV-1.0.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4493 b- defN 23-Apr-27 22:03 pyBCV-1.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-27 22:03 pyBCV-1.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-27 22:03 pyBCV-1.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      672 b- defN 23-Apr-27 22:03 pyBCV-1.0.6.dist-info/RECORD
+9 files, 13736 bytes uncompressed, 5031 bytes compressed:  63.4%
```

## zipnote {}

```diff
@@ -1,22 +1,28 @@
 Filename: pyBCV/__init__.py
 Comment: 
 
 Filename: pyBCV/pyBCV.py
 Comment: 
 
-Filename: pyBCV-1.0.5.dist-info/LICENSE
+Filename: pyBCV/core/__init__.py
 Comment: 
 
-Filename: pyBCV-1.0.5.dist-info/METADATA
+Filename: pyBCV/core/requests.py
 Comment: 
 
-Filename: pyBCV-1.0.5.dist-info/WHEEL
+Filename: pyBCV-1.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: pyBCV-1.0.5.dist-info/top_level.txt
+Filename: pyBCV-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: pyBCV-1.0.5.dist-info/RECORD
+Filename: pyBCV-1.0.6.dist-info/WHEEL
+Comment: 
+
+Filename: pyBCV-1.0.6.dist-info/top_level.txt
+Comment: 
+
+Filename: pyBCV-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyBCV/pyBCV.py

```diff
@@ -1,15 +1,15 @@
 import locale
 from decimal import Decimal
 from typing import Any, Callable
 from datetime import datetime, timedelta
 
 from bs4 import BeautifulSoup
 
-from .core.requests import BCVRequests
+from pyBCV.core.requests import BCVRequests
 
 def _extract_timestamp(soup: BeautifulSoup) -> datetime:
     try:
         return datetime.fromisoformat(
             soup.find("span", "date-display-single").get("content")
         )
     except:
```

## Comparing `pyBCV-1.0.5.dist-info/LICENSE` & `pyBCV-1.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyBCV-1.0.5.dist-info/METADATA` & `pyBCV-1.0.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBCV
-Version: 1.0.5
+Version: 1.0.6
 Summary: PyBCV es una librería desarrollada en el lenguaje de programación Python que se utiliza para recopilar los precios de los tipos de cambio y las tasas informativas proporcionados por el Banco Central de Venezuela (BCV).
 Home-page: https://github.com/fcoagz/pyBCV
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/fcoagz/pyBCV
 Project-URL: Bug Tracker, https://github.com/fcoagz/pyBCV/issues
```

