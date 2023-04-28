# Comparing `tmp/PyMysqlTools-0.5.8.tar.gz` & `tmp/PyMysqlTools-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMysqlTools-0.5.8.tar", last modified: Thu Nov 10 03:56:48 2022, max compression
+gzip compressed data, was "PyMysqlTools-0.5.9.tar", last modified: Thu Nov 10 11:00:27 2022, max compression
```

## Comparing `PyMysqlTools-0.5.8.tar` & `PyMysqlTools-0.5.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-11-10 03:56:47.980950 PyMysqlTools-0.5.8/
--rw-rw-rw-   0        0        0     1083 2022-11-09 07:31:21.000000 PyMysqlTools-0.5.8/LICENSE
--rw-rw-rw-   0        0        0      143 2022-11-09 07:31:21.000000 PyMysqlTools-0.5.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2594 2022-11-10 03:56:47.980950 PyMysqlTools-0.5.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-11-10 03:56:47.953621 PyMysqlTools-0.5.8/PyMysqlTools/
--rw-rw-rw-   0        0        0     2703 2022-11-09 07:31:21.000000 PyMysqlTools-0.5.8/PyMysqlTools/ClauseGenerator.py
--rw-rw-rw-   0        0        0     4255 2022-11-09 07:31:21.000000 PyMysqlTools-0.5.8/PyMysqlTools/PlanExecutor.py
--rw-rw-rw-   0        0        0    26536 2022-11-10 03:23:11.000000 PyMysqlTools-0.5.8/PyMysqlTools/PyMysqlTools.py
--rw-rw-rw-   0        0        0     2839 2022-11-10 03:51:18.000000 PyMysqlTools-0.5.8/PyMysqlTools/ResultSet.py
--rw-rw-rw-   0        0        0     1249 2022-11-09 07:31:21.000000 PyMysqlTools-0.5.8/PyMysqlTools/SqlActuator.py
--rw-rw-rw-   0        0        0     3597 2022-11-09 09:15:02.000000 PyMysqlTools-0.5.8/PyMysqlTools/SqlGenerator.py
--rw-rw-rw-   0        0        0     1240 2022-11-10 03:53:57.000000 PyMysqlTools-0.5.8/PyMysqlTools/__init__.py
--rw-rw-rw-   0        0        0       68 2022-11-10 03:05:16.000000 PyMysqlTools-0.5.8/PyMysqlTools/config.py
-drwxrwxrwx   0        0        0        0 2022-11-10 03:56:47.978997 PyMysqlTools-0.5.8/PyMysqlTools.egg-info/
--rw-rw-rw-   0        0        0     2594 2022-11-10 03:56:47.000000 PyMysqlTools-0.5.8/PyMysqlTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2022-11-10 03:56:47.000000 PyMysqlTools-0.5.8/PyMysqlTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-10 03:56:47.000000 PyMysqlTools-0.5.8/PyMysqlTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2022-11-10 03:56:47.000000 PyMysqlTools-0.5.8/PyMysqlTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-11-10 03:56:47.000000 PyMysqlTools-0.5.8/PyMysqlTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1991 2022-11-09 07:31:21.000000 PyMysqlTools-0.5.8/README.md
--rw-rw-rw-   0        0        0       50 2022-11-09 07:31:21.000000 PyMysqlTools-0.5.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-11-10 03:56:47.980950 PyMysqlTools-0.5.8/setup.cfg
--rw-rw-rw-   0        0        0     1359 2022-11-09 07:31:21.000000 PyMysqlTools-0.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-10 11:00:27.015107 PyMysqlTools-0.5.9/
+-rw-rw-rw-   0        0        0     1083 2022-11-09 07:31:21.000000 PyMysqlTools-0.5.9/LICENSE
+-rw-rw-rw-   0        0        0      143 2022-11-09 07:31:21.000000 PyMysqlTools-0.5.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2594 2022-11-10 11:00:27.015107 PyMysqlTools-0.5.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-11-10 11:00:27.000466 PyMysqlTools-0.5.9/PyMysqlTools/
+-rw-rw-rw-   0        0        0     2703 2022-11-09 07:31:21.000000 PyMysqlTools-0.5.9/PyMysqlTools/ClauseGenerator.py
+-rw-rw-rw-   0        0        0     4255 2022-11-09 07:31:21.000000 PyMysqlTools-0.5.9/PyMysqlTools/PlanExecutor.py
+-rw-rw-rw-   0        0        0    26690 2022-11-10 10:58:19.000000 PyMysqlTools-0.5.9/PyMysqlTools/PyMysqlTools.py
+-rw-rw-rw-   0        0        0     2842 2022-11-10 10:53:46.000000 PyMysqlTools-0.5.9/PyMysqlTools/ResultSet.py
+-rw-rw-rw-   0        0        0     1249 2022-11-09 07:31:21.000000 PyMysqlTools-0.5.9/PyMysqlTools/SqlActuator.py
+-rw-rw-rw-   0        0        0     3597 2022-11-09 09:15:02.000000 PyMysqlTools-0.5.9/PyMysqlTools/SqlGenerator.py
+-rw-rw-rw-   0        0        0     1240 2022-11-10 10:59:36.000000 PyMysqlTools-0.5.9/PyMysqlTools/__init__.py
+-rw-rw-rw-   0        0        0       68 2022-11-10 03:05:16.000000 PyMysqlTools-0.5.9/PyMysqlTools/config.py
+drwxrwxrwx   0        0        0        0 2022-11-10 11:00:27.013159 PyMysqlTools-0.5.9/PyMysqlTools.egg-info/
+-rw-rw-rw-   0        0        0     2594 2022-11-10 11:00:26.000000 PyMysqlTools-0.5.9/PyMysqlTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2022-11-10 11:00:26.000000 PyMysqlTools-0.5.9/PyMysqlTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-10 11:00:26.000000 PyMysqlTools-0.5.9/PyMysqlTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2022-11-10 11:00:26.000000 PyMysqlTools-0.5.9/PyMysqlTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2022-11-10 11:00:26.000000 PyMysqlTools-0.5.9/PyMysqlTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1991 2022-11-09 07:31:21.000000 PyMysqlTools-0.5.9/README.md
+-rw-rw-rw-   0        0        0       50 2022-11-09 07:31:21.000000 PyMysqlTools-0.5.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2022-11-10 11:00:27.016083 PyMysqlTools-0.5.9/setup.cfg
+-rw-rw-rw-   0        0        0     1359 2022-11-09 07:31:21.000000 PyMysqlTools-0.5.9/setup.py
```

### Comparing `PyMysqlTools-0.5.8/LICENSE` & `PyMysqlTools-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMysqlTools-0.5.8/PKG-INFO` & `PyMysqlTools-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMysqlTools
-Version: 0.5.8
+Version: 0.5.9
 Summary: A library that makes MySQL operation more convenient.
 Home-page: https://gitee.com/uraurara/PyMysqlTools
 Author: ulala
 Author-email: 2713389652@qq.com
 License: MIT
 Keywords: mysql,client,mysqluitls,PyMysqlTools
 Platform: UNKNOWN
```

### Comparing `PyMysqlTools-0.5.8/PyMysqlTools/ClauseGenerator.py` & `PyMysqlTools-0.5.9/PyMysqlTools/ClauseGenerator.py`

 * *Files identical despite different names*

### Comparing `PyMysqlTools-0.5.8/PyMysqlTools/PlanExecutor.py` & `PyMysqlTools-0.5.9/PyMysqlTools/PlanExecutor.py`

 * *Files identical despite different names*

### Comparing `PyMysqlTools-0.5.8/PyMysqlTools/PyMysqlTools.py` & `PyMysqlTools-0.5.9/PyMysqlTools/PyMysqlTools.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         :param type_: 返回集结构类型 [dict/list]
         :return: 结果集
         """
         sql = self._sql_generator.find_by(tb_name, fields, condition)
         return ResultSet(
             self._sql_actuator.actuator_dql(sql),
             type_=type_,
-            fields_=self.show_table_fields(tb_name)
+            fields_=self.show_table_fields(tb_name).all()
         )
 
     def find_by_id(self, tb_name: str, id_: int, fields: list = None) -> ResultSet:
         """
         根据id查询记录
         :param tb_name: 表名
         :param id_: id
@@ -186,15 +186,15 @@
         :return: 结果集
         """
         sql = self._sql_generator.find_by(tb_name, fields, condition)
         sql += self._clause_generator.build_limit_clause(1)
         return ResultSet(
             self._sql_actuator.actuator_dql(sql),
             type_=type_,
-            fields_=self.show_table_fields(tb_name)
+            fields_=self.show_table_fields(tb_name).all()
         )
 
     def find_all(self, tb_name: str) -> ResultSet:
         """
         查询全表记录
         :param tb_name: 表名
         :return: 结果集
@@ -558,40 +558,44 @@
         :param type_: 返回集结构类型 [dict/list]
         :return: 结果集
         """
         sql = self._sql_generator.find_by(tb_name, fields, condition)
         result = ResultSet(
             self._sql_actuator.actuator_dql(sql),
             type_=type_,
-            fields_=self.show_table_fields(tb_name)
+            fields_=self.show_table_fields(tb_name).all()
         )
         self._connect.close()
         return result
 
     def find_by_id(self, tb_name: str, id_: int, fields: list = None) -> ResultSet:
         """
         根据id查询记录
         :param tb_name: 表名
         :param id_: id
         :param fields: 需要查询的字段
         :return: 结果集
         """
         return self.find_by(tb_name, fields, {'id': id_})
 
-    def find_one(self, tb_name: str, fields: list = None, condition=None) -> ResultSet:
+    def find_one(self, tb_name: str, fields: list = None, condition=None, type_=config.DEFAULT_RESULT_SET_TYPE) -> ResultSet:
         """
         根据条件查询单条记录
         :param tb_name: 表名
         :param fields: 需要查询的字段
         :param condition: 查询条件
         :return: 结果集
         """
         sql = self._sql_generator.find_by(tb_name, fields, condition)
         sql += self._clause_generator.build_limit_clause(1)
-        return ResultSet(self._sql_actuator.actuator_dql(sql), type_=list)
+        return ResultSet(
+            self._sql_actuator.actuator_dql(sql),
+            type_=type_,
+            fields_=self.show_table_fields(tb_name).all()
+        )
 
     def find_all(self, tb_name: str) -> ResultSet:
         """
         查询全表记录
         :param tb_name: 表名
         :return: 结果集
         """
```

### Comparing `PyMysqlTools-0.5.8/PyMysqlTools/ResultSet.py` & `PyMysqlTools-0.5.9/PyMysqlTools/ResultSet.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                     self._result.append(row[0])
                 else:
                     self._result.append([None])
         elif type_ == dict:
             if fields_ is None:
                 raise ValueError('[参数错误]', "'type_'为dict时 'fields_' 需要传入参数")
             else:
-                self._fields = fields_
+                self._fields = fields_[0]
                 for row in result:
                     self._result.append(_extract_as_dict(self._fields, row))
         else:
             raise ValueError('[参数数据类型错误]', "'type_' 只能是 list/dict 类型")
 
         if len(result) == 1:
             self._result = list(result[0])
```

### Comparing `PyMysqlTools-0.5.8/PyMysqlTools/SqlActuator.py` & `PyMysqlTools-0.5.9/PyMysqlTools/SqlActuator.py`

 * *Files identical despite different names*

### Comparing `PyMysqlTools-0.5.8/PyMysqlTools/SqlGenerator.py` & `PyMysqlTools-0.5.9/PyMysqlTools/SqlGenerator.py`

 * *Files identical despite different names*

### Comparing `PyMysqlTools-0.5.8/PyMysqlTools/__init__.py` & `PyMysqlTools-0.5.9/PyMysqlTools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 from PyMysqlTools.PyMysqlTools import connect
 from PyMysqlTools.PyMysqlTools import connect_pool
 
-__version__ = "0.5.8"
+__version__ = "0.5.9"
 name = "PyMysqlTools"
```

### Comparing `PyMysqlTools-0.5.8/PyMysqlTools.egg-info/PKG-INFO` & `PyMysqlTools-0.5.9/PyMysqlTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMysqlTools
-Version: 0.5.8
+Version: 0.5.9
 Summary: A library that makes MySQL operation more convenient.
 Home-page: https://gitee.com/uraurara/PyMysqlTools
 Author: ulala
 Author-email: 2713389652@qq.com
 License: MIT
 Keywords: mysql,client,mysqluitls,PyMysqlTools
 Platform: UNKNOWN
```

### Comparing `PyMysqlTools-0.5.8/README.md` & `PyMysqlTools-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `PyMysqlTools-0.5.8/setup.py` & `PyMysqlTools-0.5.9/setup.py`

 * *Files identical despite different names*

