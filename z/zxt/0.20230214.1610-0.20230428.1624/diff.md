# Comparing `tmp/zxt-0.20230214.1610.tar.gz` & `tmp/zxt-0.20230428.1624.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zxt-0.20230214.1610.tar", last modified: Tue Feb 14 08:14:16 2023, max compression
+gzip compressed data, was "zxt-0.20230428.1624.tar", last modified: Fri Apr 28 08:58:20 2023, max compression
```

## Comparing `zxt-0.20230214.1610.tar` & `zxt-0.20230428.1624.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-02-14 08:14:16.671350 zxt-0.20230214.1610/
--rw-rw-rw-   0        0        0    35821 2022-12-30 03:02:11.000000 zxt-0.20230214.1610/LICENSE
--rw-rw-rw-   0        0        0    42522 2023-02-14 08:14:16.672350 zxt-0.20230214.1610/PKG-INFO
--rw-rw-rw-   0        0        0      845 2023-02-06 17:30:16.000000 zxt-0.20230214.1610/README.md
--rw-rw-rw-   0        0        0      815 2023-02-14 08:10:24.000000 zxt-0.20230214.1610/pyproject.toml
--rw-rw-rw-   0        0        0      555 2023-02-14 08:14:16.673672 zxt-0.20230214.1610/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-02-06 17:11:18.000000 zxt-0.20230214.1610/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-14 08:14:16.663635 zxt-0.20230214.1610/zxt/
--rw-rw-rw-   0        0        0        0 2023-02-06 07:46:40.000000 zxt-0.20230214.1610/zxt/__init__.py
--rw-rw-rw-   0        0        0     4302 2023-02-14 08:03:45.000000 zxt-0.20230214.1610/zxt/log_helper.py
--rw-rw-rw-   0        0        0    12100 2023-02-14 08:08:11.000000 zxt-0.20230214.1610/zxt/redis_helper.py
--rw-rw-rw-   0        0        0     7672 2023-02-06 17:05:34.000000 zxt-0.20230214.1610/zxt/sql_helper.py
-drwxrwxrwx   0        0        0        0 2023-02-14 08:14:16.670335 zxt-0.20230214.1610/zxt.egg-info/
--rw-rw-rw-   0        0        0    42522 2023-02-14 08:14:16.000000 zxt-0.20230214.1610/zxt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-02-14 08:14:16.000000 zxt-0.20230214.1610/zxt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-14 08:14:16.000000 zxt-0.20230214.1610/zxt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-02-14 08:14:16.000000 zxt-0.20230214.1610/zxt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-02-14 08:14:16.000000 zxt-0.20230214.1610/zxt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 08:58:20.076342 zxt-0.20230428.1624/
+-rw-rw-rw-   0        0        0    35821 2022-12-30 03:02:11.000000 zxt-0.20230428.1624/LICENSE
+-rw-rw-rw-   0        0        0    42858 2023-04-28 08:58:20.077432 zxt-0.20230428.1624/PKG-INFO
+-rw-rw-rw-   0        0        0     1181 2023-04-28 08:58:03.000000 zxt-0.20230428.1624/README.md
+-rw-rw-rw-   0        0        0      815 2023-04-28 08:24:59.000000 zxt-0.20230428.1624/pyproject.toml
+-rw-rw-rw-   0        0        0      555 2023-04-28 08:58:20.081964 zxt-0.20230428.1624/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-02-06 17:11:18.000000 zxt-0.20230428.1624/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 08:58:20.061621 zxt-0.20230428.1624/zxt/
+-rw-rw-rw-   0        0        0        0 2023-02-06 07:46:40.000000 zxt-0.20230428.1624/zxt/__init__.py
+-rw-rw-rw-   0        0        0     4302 2023-02-14 08:03:45.000000 zxt-0.20230428.1624/zxt/log_helper.py
+-rw-rw-rw-   0        0        0     6720 2023-04-28 08:14:21.000000 zxt-0.20230428.1624/zxt/pth.py
+-rw-rw-rw-   0        0        0    12100 2023-02-14 08:08:11.000000 zxt-0.20230428.1624/zxt/redis_helper.py
+-rw-rw-rw-   0        0        0     8390 2023-04-28 08:40:56.000000 zxt-0.20230428.1624/zxt/sql_helper.py
+drwxrwxrwx   0        0        0        0 2023-04-28 08:58:20.075336 zxt-0.20230428.1624/zxt.egg-info/
+-rw-rw-rw-   0        0        0    42858 2023-04-28 08:58:20.000000 zxt-0.20230428.1624/zxt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-04-28 08:58:20.000000 zxt-0.20230428.1624/zxt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 08:58:20.000000 zxt-0.20230428.1624/zxt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-04-28 08:58:20.000000 zxt-0.20230428.1624/zxt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-28 08:58:20.000000 zxt-0.20230428.1624/zxt.egg-info/top_level.txt
```

### Comparing `zxt-0.20230214.1610/LICENSE` & `zxt-0.20230428.1624/LICENSE`

 * *Files identical despite different names*

### Comparing `zxt-0.20230214.1610/PKG-INFO` & `zxt-0.20230428.1624/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zxt
-Version: 0.20230214.1610
+Version: 0.20230428.1624
 Summary: A handy toolkit
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -707,13 +707,23 @@
 
 3.  升级工具
     python -m pip install --upgrade build
     python -m pip install --upgrade twine
 
 4.  Generating distribution archives (生成档案)
     https://packaging.python.org/en/latest/tutorials/packaging-projects/
-    切换到 pyproject.toml 的同级目录
+    切换到 pyproject.toml 的同级目录, 一般先删除 dist 目录(RMDIR /S .\dist\ /Q)
     python -m build
 
 5.  Uploading the distribution archives (上传档案)
     https://packaging.python.org/en/latest/tutorials/packaging-projects/
     python -m twine upload --repository zxt dist/*
+
+#### 调试教程
+
+1.  卸载 zxt 包
+    python -m pip uninstall zxt
+
+2.  从 zxt 的源码中找到 pth.py 所在目录, 在该目录下执行如下命令:
+    python ./pth.py --dflt_opt=C
+
+3.  源码已关联到 python 环境, 可以写代码调用 zxt 包进行调试了
```

### Comparing `zxt-0.20230214.1610/pyproject.toml` & `zxt-0.20230428.1624/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 # https://packaging.python.org/en/latest/tutorials/packaging-projects/#creating-pyproject-toml
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 [project]
 name = "zxt"
-version = "0.20230214.1610"
+version = "0.20230428.1624"
 description = "A handy toolkit"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["tool", "toolkit"]
 # https://pypi.org/pypi?:action=list_classifiers
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `zxt-0.20230214.1610/setup.cfg` & `zxt-0.20230428.1624/setup.cfg`

 * *Files identical despite different names*

### Comparing `zxt-0.20230214.1610/zxt/log_helper.py` & `zxt-0.20230428.1624/zxt/log_helper.py`

 * *Files identical despite different names*

### Comparing `zxt-0.20230214.1610/zxt/redis_helper.py` & `zxt-0.20230428.1624/zxt/redis_helper.py`

 * *Files identical despite different names*

### Comparing `zxt-0.20230214.1610/zxt/sql_helper.py` & `zxt-0.20230428.1624/zxt/sql_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # !/usr/bin/env python3
 # coding=utf8
 """
 一些"代码分析工具"(比如 Pylint)能检出不符合编码风格标准和有潜在风险的代码。
 由于 python 2 和 python 3 部分语法不同，"代码分析工具"会识别 .py 文件头部的解释器来判断该文件 python 版本。
 如果发现 python 3 文件报出了 invalid syntax 错误，可能是由于被当成了 python 2 扫描。
 此时在文件首行加上右面的代码即可：# !/usr/bin/env python3
+
+定义编码【# coding=<encoding name>】参见: http://www.python.org/peps/pep-0263.html
+
+对 SQL 的简单封装，支持 MySQL 和 SQLite
 """
-# http://www.python.org/peps/pep-0263.html
 
 
 import json
 import peewee
 import playhouse.db_url
 import pymysql
 import pymysql.cursors
@@ -25,15 +28,15 @@
     url: str = "sqlite:///:memory:"
     url: str = "mysql://用户:密码@主机:端口/数据库?charset=字符集"
     url: str = "mysql://root:toor@localhost:13306/mysql?charset=utf8"
     sqlhelper = SqlHelper()
     sqlhelper.initialize(url=url, lazy_init=True)
     results: list = sqlhelper.select("SELECT 3*7 AS number;", isDictNotList=True)
     print(results)
-    sqlhelper.execute("CREATE TEMPORARY TABLE temp_test(kkk VARCHAR(255) NOT NULL, vvv VARCHAR(512) NOT NULL);")
+    sqlhelper.execute("CREATE TEMPORARY TABLE temp_test(kkk VARCHAR(256) NOT NULL, vvv VARCHAR(512) NOT NULL);")
     sqlhelper.execute("INSERT INTO temp_test(kkk,vvv)VALUES('k1','v1'),('k2','v2');")
     results: list = sqlhelper.select("SELECT * FROM temp_test;", isDictNotList=True)
     print(results)
     sqlhelper.terminate()
 
     lazy_init: 延迟初始化数据库连接, 真正要执行 SQL 语句的时候, 才开始连接到数据库,
     只有指定的机器可以连接到对应的线上数据库, 多个线上库可能指定了不同的机器,
@@ -74,19 +77,26 @@
 
                 self.connection: Union[peewee.MySQLDatabase, peewee.SqliteDatabase] = playhouse.db_url.connect(url=self.url)  # noqa E501
                 self.cursor = self.connection.cursor()
         pass
 
     def terminate(self) -> None:
         """"""
-        if self.connection:
-            self.cursor.close()
-            self.cursor = None
-            self.connection.close()
-            self.connection = None
+        for _ in range(1):
+            if not self.connection:
+                break
+
+            with self.lock:  # self.lock.acquire(); self.lock.release();
+                if not self.connection:
+                    break
+
+                self.cursor.close()
+                self.cursor = None
+                self.connection.close()
+                self.connection = None
 
     def __del__(self) -> None:
         """"""
         self.terminate()
 
     def select(self, sql: str, isDictNotList: bool = False) -> List[Union[tuple, dict]]:
         """"""
@@ -121,38 +131,45 @@
             results = [dict(zip(head, data)) for data in cursor.fetchall()]
         else:
             head = [col[0] for col in cursor.description]
             results = [data for data in cursor.fetchall()]
             results.insert(0, head)
         return results
 
+    @classmethod
+    def fetchone(cls, cursor: Union[pymysql.cursors.Cursor, sqlite3.Cursor], isDictNotList: bool = False) -> List[Union[tuple, dict]]:
+        '''如果结果是空,且(isDictNotList=True),那么结果为空,不利于保存到文件'''
+        if isDictNotList:
+            head = [col[0] for col in cursor.description]
+            results = [dict(zip(head, data)) for data in (cursor.fetchone(),)]
+        else:
+            head = [col[0] for col in cursor.description]
+            results = [data for data in (cursor.fetchone(),)]
+            results.insert(0, head)
+        return results
+
 
 class SqlHelperSet(object):
     """"""
 
     def __init__(self, *args, **kwargs):
         """"""
         self._connections: Dict[str, SqlHelper] = {}
 
     def initialize(self, conf: Union[str, dict], *args, **kwargs):
         """"""
-        if isinstance(conf, str):
+        if isinstance(conf, str):  # 文件路径,
             with open(file=conf, mode="r", encoding="utf8") as fp:
                 conf_obj = json.load(fp=fp)
         else:
-            conf_obj = conf
+            conf_obj = conf  # 文件内容,
 
         for name, params in conf_obj.items():
             assert isinstance(name, str) and (name != '')  # name 不可为空
             assert isinstance(params, dict)
-            if True:
-                # 数据库接口不支持未知参数, 决定在这里移除(用户自定义的)未知参数, 用户自定义的参数必须包含三个下划线,
-                keys = [key for key in params.keys() if '___' in key]
-                for key in keys:
-                    del params[key]
 
             sql_helper = SqlHelper()
             sql_helper.initialize(**params)
             self._connections[name] = sql_helper
 
         pass
 
@@ -179,32 +196,32 @@
             connection = self._connections.values().__iter__().__next__()
         else:
             connection = self._connections.get(name, None)
 
         return connection
 
     def select(self, sql: str, isDictNotList: bool = False, name: str = None) -> list:
-        """
-        select
-        """
+        """"""
         connection: Optional[SqlHelper] = self._get_connection(name)
         return connection.select(sql=sql, isDictNotList=isDictNotList)
 
 
 if __name__ == '__main__':
     conf_obj = {
-        "default": {
+        "testdb": {
             "url": "mysql://root:toor@localhost:13306/mysql?charset=utf8",
             "lazy_init": True,
+            "__note": "测试环境的MySQL",
         },
         "memory": {
             "url": "sqlite:///:memory:",
             "lazy_init": True,
+            "__note": "内存模式的SQLite",
         }
     }
     shs = SqlHelperSet()
     shs.initialize(conf=conf_obj)
     sql_statement = 'SELECT 3*7 AS number;'
-    results = shs.select(sql_statement, isDictNotList=True, name="default")
+    results = shs.select(sql_statement, isDictNotList=True, name="memory")
     shs.terminate()
     for result in results:
         print(result)
```

### Comparing `zxt-0.20230214.1610/zxt.egg-info/PKG-INFO` & `zxt-0.20230428.1624/zxt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zxt
-Version: 0.20230214.1610
+Version: 0.20230428.1624
 Summary: A handy toolkit
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -707,13 +707,23 @@
 
 3.  升级工具
     python -m pip install --upgrade build
     python -m pip install --upgrade twine
 
 4.  Generating distribution archives (生成档案)
     https://packaging.python.org/en/latest/tutorials/packaging-projects/
-    切换到 pyproject.toml 的同级目录
+    切换到 pyproject.toml 的同级目录, 一般先删除 dist 目录(RMDIR /S .\dist\ /Q)
     python -m build
 
 5.  Uploading the distribution archives (上传档案)
     https://packaging.python.org/en/latest/tutorials/packaging-projects/
     python -m twine upload --repository zxt dist/*
+
+#### 调试教程
+
+1.  卸载 zxt 包
+    python -m pip uninstall zxt
+
+2.  从 zxt 的源码中找到 pth.py 所在目录, 在该目录下执行如下命令:
+    python ./pth.py --dflt_opt=C
+
+3.  源码已关联到 python 环境, 可以写代码调用 zxt 包进行调试了
```

