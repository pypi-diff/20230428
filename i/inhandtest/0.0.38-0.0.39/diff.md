# Comparing `tmp/inhandtest-0.0.38.tar.gz` & `tmp/inhandtest-0.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.38.tar", last modified: Thu Apr 27 08:23:33 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.39.tar", last modified: Fri Apr 28 07:02:09 2023, max compression
```

## Comparing `inhandtest-0.0.38.tar` & `inhandtest-0.0.39.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 08:23:33.000000 inhandtest-0.0.38/
--rw-rw-rw-   0        0        0      535 2023-04-27 08:23:33.000000 inhandtest-0.0.38/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.38/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 08:23:33.000000 inhandtest-0.0.38/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.38/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 08:23:33.000000 inhandtest-0.0.38/inhandtest/base_page/
--rw-rw-rw-   0        0        0      134 2023-03-15 06:05:35.000000 inhandtest-0.0.38/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    61990 2023-03-31 06:55:18.000000 inhandtest-0.0.38/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    43917 2023-03-31 07:28:55.000000 inhandtest-0.0.38/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0    10436 2023-04-18 03:34:40.000000 inhandtest-0.0.38/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.38/inhandtest/exception.py
--rw-rw-rw-   0        0        0     3890 2023-03-30 10:08:49.000000 inhandtest-0.0.38/inhandtest/file.py
--rw-rw-rw-   0        0        0    11858 2023-04-04 07:39:23.000000 inhandtest-0.0.38/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.38/inhandtest/inmongodb.py
--rw-rw-rw-   0        0        0    22049 2023-03-30 10:08:49.000000 inhandtest-0.0.38/inhandtest/inmqtt.py
--rw-rw-rw-   0        0        0    45529 2023-04-24 06:54:53.000000 inhandtest-0.0.38/inhandtest/inrequest.py
--rw-rw-rw-   0        0        0    12335 2023-04-06 06:40:29.000000 inhandtest-0.0.38/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     6088 2023-03-30 10:30:59.000000 inhandtest-0.0.38/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     1144 2023-03-30 10:18:47.000000 inhandtest-0.0.38/inhandtest/ip.py
--rw-rw-rw-   0        0        0     3628 2023-04-23 10:47:45.000000 inhandtest-0.0.38/inhandtest/mail.py
--rw-rw-rw-   0        0        0     1222 2023-04-18 01:10:09.000000 inhandtest-0.0.38/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0    32413 2023-04-21 10:20:01.000000 inhandtest-0.0.38/inhandtest/telnet.py
--rw-rw-rw-   0        0        0    24838 2023-04-27 08:19:48.000000 inhandtest-0.0.38/inhandtest/tools.py
--rw-rw-rw-   0        0        0      115 2023-04-24 03:15:39.000000 inhandtest-0.0.38/requirements.txt
--rw-rw-rw-   0        0        0     1419 2023-04-27 08:22:19.000000 inhandtest-0.0.38/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:02:09.000000 inhandtest-0.0.39/
+-rw-rw-rw-   0        0        0      535 2023-04-28 07:02:09.000000 inhandtest-0.0.39/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.39/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 07:02:09.000000 inhandtest-0.0.39/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.39/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:02:09.000000 inhandtest-0.0.39/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      134 2023-03-15 06:05:35.000000 inhandtest-0.0.39/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    61990 2023-03-31 06:55:18.000000 inhandtest-0.0.39/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    43917 2023-03-31 07:28:55.000000 inhandtest-0.0.39/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0    10436 2023-04-18 03:34:40.000000 inhandtest-0.0.39/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.39/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     3890 2023-03-30 10:08:49.000000 inhandtest-0.0.39/inhandtest/file.py
+-rw-rw-rw-   0        0        0    11858 2023-04-04 07:39:23.000000 inhandtest-0.0.39/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.39/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22049 2023-03-30 10:08:49.000000 inhandtest-0.0.39/inhandtest/inmqtt.py
+-rw-rw-rw-   0        0        0    45529 2023-04-24 06:54:53.000000 inhandtest-0.0.39/inhandtest/inrequest.py
+-rw-rw-rw-   0        0        0    12335 2023-04-06 06:40:29.000000 inhandtest-0.0.39/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     6088 2023-03-30 10:30:59.000000 inhandtest-0.0.39/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     1144 2023-03-30 10:18:47.000000 inhandtest-0.0.39/inhandtest/ip.py
+-rw-rw-rw-   0        0        0     3628 2023-04-23 10:47:45.000000 inhandtest-0.0.39/inhandtest/mail.py
+-rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.39/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0    32413 2023-04-21 10:20:01.000000 inhandtest-0.0.39/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0    25167 2023-04-28 06:14:33.000000 inhandtest-0.0.39/inhandtest/tools.py
+-rw-rw-rw-   0        0        0      115 2023-04-24 03:15:39.000000 inhandtest-0.0.39/requirements.txt
+-rw-rw-rw-   0        0        0     1419 2023-04-28 07:02:00.000000 inhandtest-0.0.39/setup.py
```

### Comparing `inhandtest-0.0.38/PKG-INFO` & `inhandtest-0.0.39/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: inhandtest
-Version: 0.0.38
+Version: 0.0.39
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 License: UNKNOWN
 Description: 方便inhand测试同事在自动化测试时，对通用协议或者常用工具及方法做封装，需要使用时即在线安装；
         映翰通出品，追尾必究！
```

### Comparing `inhandtest-0.0.38/README.md` & `inhandtest-0.0.39/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.38/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.39/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.38/inhandtest/base_page/base_page.py` & `inhandtest-0.0.39/inhandtest/base_page/base_page.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.38/inhandtest/base_page/table_tr.py` & `inhandtest-0.0.39/inhandtest/base_page/table_tr.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.38/inhandtest/exception.py` & `inhandtest-0.0.39/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.38/inhandtest/file.py` & `inhandtest-0.0.39/inhandtest/file.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.38/inhandtest/inmodbus.py` & `inhandtest-0.0.39/inhandtest/inmodbus.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.38/inhandtest/inmongodb.py` & `inhandtest-0.0.39/inhandtest/inmongodb.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.38/inhandtest/inmqtt.py` & `inhandtest-0.0.39/inhandtest/inmqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.38/inhandtest/inrequest.py` & `inhandtest-0.0.39/inhandtest/inrequest.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.38/inhandtest/insocket.py` & `inhandtest-0.0.39/inhandtest/insocket.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.38/inhandtest/inssh.py` & `inhandtest-0.0.39/inhandtest/inssh.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.38/inhandtest/ip.py` & `inhandtest-0.0.39/inhandtest/ip.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.38/inhandtest/mail.py` & `inhandtest-0.0.39/inhandtest/mail.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.38/inhandtest/pytest_email.html` & `inhandtest-0.0.39/inhandtest/pytest_email.html`

 * *Files 1% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     background-color: #f2f2f2;
   }
   tr:nth-child(even) {
     background-color: #f2f2f2;
   }
     </style>
 </table>
-<p><a href={{report_url}}>报告详情</a></p>
+<p><a href="{{report_url}}">报告详情</a></p>
 </body>
 </html>
```

### Comparing `inhandtest-0.0.38/inhandtest/telnet.py` & `inhandtest-0.0.39/inhandtest/telnet.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.38/inhandtest/tools.py` & `inhandtest-0.0.39/inhandtest/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import os.path
 import random
 import re
 import string
 import subprocess
 import time
 import datetime
+from functools import wraps
 from typing import List
 import pytz
 import winreg
 import requests
 from inhandtest.file import file_hash
 from inhandtest.exception import ResourceNotFoundError
 
@@ -29,15 +30,19 @@
     :param timeout:  循环检测超时时间
     :param interval:  循环检测时间间隔
     :param assertion: 默认期望断言，如果为False时 返回值
     :return:  assertion为False时，返回函数的值
     """
 
     def timeout_(func):
+        @wraps(func)
         def inspector(*args, **kwargs):
+            nonlocal timeout, interval
+            timeout = kwargs.get('timeout') if kwargs.get('timeout') else timeout
+            interval = kwargs.get('timeout') if kwargs.get('interval') else interval
             for i in range(0, timeout + 1, interval):
                 result = func(*args, **kwargs)
                 if not result:
                     logging.info(f'{flag} assert failure, wait for {interval}s inspection')
                     time.sleep(interval)
                     continue
                 else:
@@ -59,22 +64,24 @@
     :param support_product: 方法或类 支持的设备型号 list, 如：['ir302', 'ir305'], 不区分大小写
     :return:
     """
     support_product = [product.lower() for product in support_product]
 
     def wrapper(obj):
         if isinstance(obj, type):
-            def inner(*args, **kwargs):
-                c = obj(*args, **kwargs)
-                if c.product.lower() in support_product:
-                    return obj(*args, **kwargs)
-                else:
-                    raise Exception(f"This class not support this device that product is {c.product}")
-            return inner
+            @wraps(obj, updated=())
+            class Inner(obj):
+                def __init__(self, *args, **kwargs):
+                    super().__init__(*args, **kwargs)
+                    if self.product.lower() not in support_product:
+                        raise Exception(f"This class not support this device that product is {self.product}")
+
+            return Inner
         else:
+            @wraps(obj)
             def inner(self, *args, **kwargs):
                 if self.product.lower() in support_product:
                     return obj(self, *args, **kwargs)
                 else:
                     raise Exception(f"This method not support this device that product is {self.product}")
 
             return inner
@@ -589,11 +596,11 @@
 
 
 if __name__ == '__main__':
     import sys
 
     logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO,
                         stream=sys.stdout)
-    is_installed('Google Chrome123')
+    # is_installed('Google Chrome123')
     # print(windows_cmd('route delete 192.168.2.102 mask 255.255.255.255 192.168.4.2', '操作完成', {' ': '', '\n': ''}))
     # print(generate_password(length=2, lowercase=True, uppercase=True, special_chars=True, chinese_chars=True))
     # print(get_time_stamp('2022-02-18T13:39:32Z', -2))
```

### Comparing `inhandtest-0.0.38/setup.py` & `inhandtest-0.0.39/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 setup
 
 """
 from distutils.core import setup
 
 setup(
     name='inhandtest',
-    version='0.0.38',
+    version='0.0.39',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
```

