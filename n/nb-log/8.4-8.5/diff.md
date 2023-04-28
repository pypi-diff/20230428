# Comparing `tmp/nb_log-8.4.tar.gz` & `tmp/nb_log-8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nb_log-8.4.tar", last modified: Wed Apr 19 03:37:27 2023, max compression
+gzip compressed data, was "dist\nb_log-8.5.tar", last modified: Fri Apr 28 10:41:41 2023, max compression
```

## Comparing `nb_log-8.4.tar` & `nb_log-8.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 03:37:27.000000 nb_log-8.4/
--rw-rw-rw-   0        0        0    27863 2023-04-19 03:37:27.000000 nb_log-8.4/PKG-INFO
--rw-rw-rw-   0        0        0    26926 2022-12-05 09:46:23.000000 nb_log-8.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 03:37:27.000000 nb_log-8.4/nb_log/
--rw-rw-rw-   0        0        0     2329 2022-09-17 07:28:19.000000 nb_log-8.4/nb_log/__init__.py
--rw-rw-rw-   0        0        0    50524 2023-04-19 03:34:32.000000 nb_log-8.4/nb_log/handlers.py
--rw-rw-rw-   0        0        0    49868 2022-09-17 07:28:19.000000 nb_log-8.4/nb_log/handlers0000.py
--rw-rw-rw-   0        0        0      247 2023-04-18 01:17:35.000000 nb_log-8.4/nb_log/helper.py
--rw-rw-rw-   0        0        0    30621 2023-04-18 02:30:56.000000 nb_log-8.4/nb_log/log_manager.py
--rw-rw-rw-   0        0        0     7782 2023-04-18 01:50:08.000000 nb_log-8.4/nb_log/monkey_print.py
--rw-rw-rw-   0        0        0     9455 2023-04-17 07:36:14.000000 nb_log-8.4/nb_log/nb_log_config_default.py
--rw-rw-rw-   0        0        0     7710 2023-04-13 09:47:00.000000 nb_log-8.4/nb_log/set_nb_log_config.py
-drwxrwxrwx   0        0        0        0 2023-04-19 03:37:27.000000 nb_log-8.4/nb_log.egg-info/
--rw-rw-rw-   0        0        0    27863 2023-04-19 03:37:27.000000 nb_log-8.4/nb_log.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2023-04-19 03:37:27.000000 nb_log-8.4/nb_log.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 03:37:27.000000 nb_log-8.4/nb_log.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      176 2023-04-19 03:37:27.000000 nb_log-8.4/nb_log.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-19 03:37:27.000000 nb_log-8.4/nb_log.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 03:37:27.000000 nb_log-8.4/setup.cfg
--rw-rw-rw-   0        0        0     2325 2023-04-19 03:37:18.000000 nb_log-8.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 10:41:41.000000 nb_log-8.5/
+-rw-rw-rw-   0        0        0    27863 2023-04-28 10:41:41.000000 nb_log-8.5/PKG-INFO
+-rw-rw-rw-   0        0        0    26926 2022-12-05 09:46:23.000000 nb_log-8.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 10:41:41.000000 nb_log-8.5/nb_log/
+-rw-rw-rw-   0        0        0     2369 2023-04-28 10:24:28.000000 nb_log-8.5/nb_log/__init__.py
+-rw-rw-rw-   0        0        0    50691 2023-04-28 10:26:55.000000 nb_log-8.5/nb_log/handlers.py
+-rw-rw-rw-   0        0        0    49868 2022-09-17 07:28:19.000000 nb_log-8.5/nb_log/handlers0000.py
+-rw-rw-rw-   0        0        0      247 2023-04-18 01:17:35.000000 nb_log-8.5/nb_log/helper.py
+-rw-rw-rw-   0        0        0    30621 2023-04-18 02:30:56.000000 nb_log-8.5/nb_log/log_manager.py
+-rw-rw-rw-   0        0        0     7782 2023-04-18 01:50:08.000000 nb_log-8.5/nb_log/monkey_print.py
+-rw-rw-rw-   0        0        0     9455 2023-04-17 07:36:14.000000 nb_log-8.5/nb_log/nb_log_config_default.py
+-rw-rw-rw-   0        0        0     7710 2023-04-13 09:47:00.000000 nb_log-8.5/nb_log/set_nb_log_config.py
+drwxrwxrwx   0        0        0        0 2023-04-28 10:41:41.000000 nb_log-8.5/nb_log.egg-info/
+-rw-rw-rw-   0        0        0    27863 2023-04-28 10:41:40.000000 nb_log-8.5/nb_log.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2023-04-28 10:41:40.000000 nb_log-8.5/nb_log.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 10:41:40.000000 nb_log-8.5/nb_log.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      176 2023-04-28 10:41:40.000000 nb_log-8.5/nb_log.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-28 10:41:40.000000 nb_log-8.5/nb_log.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 10:41:41.000000 nb_log-8.5/setup.cfg
+-rw-rw-rw-   0        0        0     2325 2023-04-28 10:41:33.000000 nb_log-8.5/setup.py
```

### Comparing `nb_log-8.4/PKG-INFO` & `nb_log-8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb_log
-Version: 8.4
+Version: 8.5
 Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
 Home-page: https://github.com/ydf0509/nb_log
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_log-8.4/README.md` & `nb_log-8.5/README.md`

 * *Files identical despite different names*

### Comparing `nb_log-8.4/nb_log/__init__.py` & `nb_log-8.5/nb_log/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
+import time
 from nb_log.set_nb_log_config import use_config_form_nb_log_config_module
 from nb_log import nb_log_config_default
 from nb_log.monkey_print import nb_print, patch_print, reverse_patch_print,stdout_write,stderr_write,print_raw,is_main_process,only_print_on_main_process
+from nb_log import handlers
 from nb_log.log_manager import LogManager, LoggerLevelSetterMixin, LoggerMixin, LoggerMixinDefaultWithFileHandler, get_logger, get_logger_with_filehanlder
-
 if nb_log_config_default.SHOW_PYCHARM_COLOR_SETINGS:
      only_print_on_main_process(
             """
             1)使用pycharm时候，强烈建议按下面的重新自定义设置pycharm的console里面的主题颜色，否则颜色显示瞎眼，代码里面规定的颜色只是大概的红黄蓝绿。在不同的ide软件和主题、字体下是不同的显示效果，需要用户自己设置。
             设置方式为 打开pycharm的 file -> settings -> Editor -> Color Scheme -> Console Colors 选择monokai，点击展开 ANSI colors，
             并重新修改自定义7个颜色，设置Blue为 0454F3 ，Cyan为 06F0F6 ，Green 为 13FC02 ，Magenta为 ff1cd5 ,red为 F80606 ，yellow为 EAFA04 ，gray 为 FFFFFF ，white 为 FFFFFF 。
             不同版本的pycahrm或主题或ide，可以根据控制台根据实际显示设置。
```

### Comparing `nb_log-8.4/nb_log/handlers.py` & `nb_log-8.5/nb_log/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 import os
 import threading
 import traceback
 import socket
 import datetime
 import json
 import time
+
 from collections import OrderedDict
 from pathlib import Path
 from queue import Queue, Empty
 # noinspection PyPackageRequirements
 from kafka import KafkaProducer
-from elasticsearch import Elasticsearch, helpers
+# from elasticsearch import Elasticsearch, helpers  # 性能导入时间消耗2秒,实例化时候再导入。
 from threading import Lock, Thread
 import pymongo
 import requests
 import logging
 from logging import handlers
 from concurrent_log_handler import ConcurrentRotatingFileHandler  # 需要安装。concurrent-log-handler==0.9.1
 # noinspection PyUnresolvedReferences
@@ -31,14 +32,15 @@
 from pythonjsonlogger.jsonlogger import JsonFormatter
 from nb_log import nb_log_config_default
 from nb_log import nb_print
 
 very_nb_print = nb_print
 os_name = os.name
 
+host_name = socket.gethostname()
 
 class MongoHandler(logging.Handler):
     """
     一个mongodb的log handler,支持日志按loggername创建不同的集合写入mongodb中
     """
 
     # msg_pattern = re.compile('(\d+-\d+-\d+ \d+:\d+:\d+) - (\S*?) - (\S*?) - (\d+) - (\S*?) - ([\s\S]*)')
@@ -96,15 +98,15 @@
 
 class KafkaHandler(logging.Handler):
     """
     日志批量写入kafka中。
     """
     ES_INTERVAL_SECONDS = 0.5
 
-    host_name = socket.gethostname()
+    host_name = host_name
     host_process = f'{host_name} -- {os.getpid()}'
 
     script_name = sys.argv[0].split('/')[-1]
 
     task_queue = Queue()
     last_es_op_time = time.time()
     has_start_do_bulk_op = False
@@ -219,22 +221,24 @@
 
 
 class ElasticHandler000(logging.Handler):
     """
     日志批量写入es中。
     """
     ES_INTERVAL_SECONDS = 2
-    host_name = socket.gethostname()
+    host_name = host_name
 
     def __init__(self, elastic_hosts: list, elastic_port, index_prefix='pylog-'):
         """
         :param elastic_hosts:  es的ip地址，数组类型
         :param elastic_port：  es端口
         :param index_prefix: index名字前缀。
         """
+        from elasticsearch import Elasticsearch, helpers
+        self._helpers = helpers
         logging.Handler.__init__(self)
         self._es_client = Elasticsearch(elastic_hosts, port=elastic_port)
         self._index_prefix = index_prefix
         self._task_list = []
         self._task_queue = Queue()
         self._last_es_op_time = time.time()
         t = Thread(target=self._do_bulk_op)
@@ -254,15 +258,15 @@
                 if self._task_queue.qsize() > 10000:
                     very_nb_print('防止意外日志积累太多了，不插入es了。')
                     self.__clear_bulk_task()
                     return
                 # noinspection PyUnresolvedReferences
                 tasks = list(self._task_queue.queue)
                 self.__clear_bulk_task()
-                helpers.bulk(self._es_client, tasks)
+                self._helpers.bulk(self._es_client, tasks)
 
                 self._last_es_op_time = time.time()
             except Exception as e:
                 very_nb_print(e)
             finally:
                 time.sleep(1)
 
@@ -306,15 +310,15 @@
 # noinspection PyUnresolvedReferences
 class ElasticHandler(logging.Handler):
     """
     日志批量写入es中。
     """
     ES_INTERVAL_SECONDS = 0.5
 
-    host_name = socket.gethostname()
+    host_name = host_name
     host_process = f'{host_name} -- {os.getpid()}'
 
     script_name = sys.argv[0]
 
     task_queue = Queue()
     last_es_op_time = time.time()
     has_start_do_bulk_op = False
@@ -688,15 +692,15 @@
 
     def _rollover_and_do_write(self):
         buffer_msgs = ''
         while True:
             try:
                 msg = self.buffer_msgs_queue.get(block=False)
                 buffer_msgs += msg + '\n'
-                if len(buffer_msgs) > 10000*1000:
+                if len(buffer_msgs) > 10000 * 1000:
                     break
             except Empty:
                 break
         if buffer_msgs:
             try:
                 self._do_lock()
                 try:
@@ -830,15 +834,14 @@
                 f'用时{round(time.time() - t_start, 2)} ,发送的内容是--> {record.msg}                    \033[0;35m!!!请去邮箱检查，可能在垃圾邮件中\033[0m')
         except Exception as e:
             # self.handleError(record)
             very_nb_print(
                 f'[log_manager.py]   {time.strftime("%H:%M:%S", time.localtime())}  \033[0;31m !!!!!! 邮件发送失败,原因是： {e} \033[0m')
 
 
-
 class DingTalkHandler(logging.Handler):
     _lock_for_remove_handlers = Lock()
 
     def __init__(self, ding_talk_token=None, time_interval=60):
         super().__init__()
         self.ding_talk_token = ding_talk_token
         self._ding_talk_url = f'https://oapi.dingtalk.com/robot/send?access_token={ding_talk_token}'
@@ -945,15 +948,15 @@
     def _write_to_file(self):  # 也可以重写 close方法，来处理末尾。
         buffer_msgs = ''
         while True:
             # print(self.buffer_msgs_queue.qsize())
             try:
                 msg = self.buffer_msgs_queue.get(block=False)
                 buffer_msgs += msg + '\n'
-                if len(buffer_msgs) > 1000*1000*10:
+                if len(buffer_msgs) > 1000 * 1000 * 10:
                     pass
                     break
             except queue.Empty:
                 break
         if buffer_msgs:
             with FileLock(self.file_path / Path(f'_delete_{self.file_name}.lock')):
                 time_str = time.strftime('%Y-%m-%d')
@@ -1037,15 +1040,15 @@
         :param record:
         :return:
         """
         # noinspection PyBroadException
         try:
             msg = self.format(record)
             self.fp.write(msg + '\n')
-            self.fp.flush() # 需要flush才能及时写入。重写close可以写入程序结束前的缓冲。
+            self.fp.flush()  # 需要flush才能及时写入。重写close可以写入程序结束前的缓冲。
         except Exception as e:
             print(e)
             self.handleError(record)
         if time.time() - self._last_delete_time > 60:
             self._get_fp()
             self._find_and_delete_files()
             self._last_delete_time = time.time()
```

### Comparing `nb_log-8.4/nb_log/handlers0000.py` & `nb_log-8.5/nb_log/handlers0000.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.4/nb_log/log_manager.py` & `nb_log-8.5/nb_log/log_manager.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.4/nb_log/monkey_print.py` & `nb_log-8.5/nb_log/monkey_print.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.4/nb_log/nb_log_config_default.py` & `nb_log-8.5/nb_log/nb_log_config_default.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.4/nb_log/set_nb_log_config.py` & `nb_log-8.5/nb_log/set_nb_log_config.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.4/nb_log.egg-info/PKG-INFO` & `nb_log-8.5/nb_log.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-log
-Version: 8.4
+Version: 8.5
 Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
 Home-page: https://github.com/ydf0509/nb_log
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_log-8.4/setup.py` & `nb_log-8.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ]
 
 if os.name == 'nt':
     install_requires.append('pywin32')
 
 setup(
     name='nb_log',  #
-    version="8.4",
+    version="8.5",
     description=(
         'very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on '
     ),
     keywords=["logging", "logger", "multiprocess file handler", "color handler"],
     # long_description=open('README.md', 'r',encoding='utf8').read(),
     long_description_content_type="text/markdown",
     long_description=open(filepath, 'r', encoding='utf8').read(),
@@ -61,14 +61,14 @@
 """
 打包上传
 python setup.py sdist upload -r pypi
 
 
 
 python setup.py sdist & twine upload dist/nb_log-6.0.tar.gz
-python setup.py sdist & python -m  twine upload dist/nb_log-8.4.tar.gz
+python setup.py sdist & python -m  twine upload dist/nb_log-8.5.tar.gz
 
 twine upload dist/*
 
 
 python -m pip install nb_log --upgrade -i https://pypi.org/simple   # 及时的方式，不用等待 阿里云 豆瓣 同步
 """
```

