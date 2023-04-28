# Comparing `tmp/pywencai-0.6.0.tar.gz` & `tmp/pywencai-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywencai-0.6.0.tar", max compression
+gzip compressed data, was "pywencai-0.7.0.tar", max compression
```

## Comparing `pywencai-0.6.0.tar` & `pywencai-0.7.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1062 2023-04-16 04:33:37.146306 pywencai-0.6.0/LICENSE
--rw-r--r--   0        0        0     2004 2023-04-16 04:33:37.146306 pywencai-0.6.0/README.md
--rw-r--r--   0        0        0      530 2023-04-16 04:33:37.146306 pywencai-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       23 2023-04-16 04:33:37.146306 pywencai-0.6.0/pywencai/__init__.py
--rw-r--r--   0        0        0    39677 2023-04-16 04:33:37.146306 pywencai-0.6.0/pywencai/hexin-v.js
--rw-r--r--   0        0        0     3768 2023-04-16 04:33:37.146306 pywencai-0.6.0/pywencai/wencai.py
--rw-r--r--   0        0        0     2589 1970-01-01 00:00:00.000000 pywencai-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-28 09:32:32.601654 pywencai-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2147 2023-04-28 09:32:32.601654 pywencai-0.7.0/README.md
+-rw-r--r--   0        0        0      530 2023-04-28 09:32:32.605654 pywencai-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-04-28 09:32:32.605654 pywencai-0.7.0/pywencai/__init__.py
+-rw-r--r--   0        0        0    39677 2023-04-28 09:32:32.605654 pywencai-0.7.0/pywencai/hexin-v.js
+-rw-r--r--   0        0        0     4111 2023-04-28 09:32:32.605654 pywencai-0.7.0/pywencai/wencai.py
+-rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 pywencai-0.7.0/PKG-INFO
```

### Comparing `pywencai-0.6.0/LICENSE` & `pywencai-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywencai-0.6.0/README.md` & `pywencai-0.7.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -70,14 +70,20 @@
 | 取值 | 含义 |
 |-|-|
 | stock | 股票 |
 | zhishu | 指数 |
 | fund | 基金 |
 | hkstock | 港股 |
 | usstock | 美股 |
+| threeboard | 新三板 |
+| conbond | 可转债 |
+| insurance | 保险 |
+| futures | 期货 |
+| lccp | 理财 |
+| foreign_exchange | 外汇 |
 
 #### retry
 
 非必填，默认为10，表示请求失败后的重试次数。
 
 #### sleep
```

### Comparing `pywencai-0.6.0/pyproject.toml` & `pywencai-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pywencai"
-version = "0.6.0"
+version = "0.7.0"
 description = ""
 authors = ["pluto <mayuanchi1029@gmail.com>"]
 readme = "README.md"
 
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://pypi.tuna.tsinghua.edu.cn/simple/"
```

### Comparing `pywencai-0.6.0/pywencai/hexin-v.js` & `pywencai-0.7.0/pywencai/hexin-v.js`

 * *Files identical despite different names*

### Comparing `pywencai-0.6.0/pywencai/wencai.py` & `pywencai-0.7.0/pywencai/wencai.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 
 logging.basicConfig(
     level=logging.INFO,
     format='[pywencai] %(asctime)s - %(levelname)s - %(message)s'
 )
 
 # 获取token
-def getToken():
+def get_token():
   with open(os.path.join(os.path.dirname(__file__), 'hexin-v.js'), 'r') as f:
     jscontent = f.read()
   context= execjs.compile(jscontent)
   return context.call("v")
 
 # 获取condition
-def getParams(**kwargs):
+def get_robot_data(**kwargs):
   retry = kwargs.get('retry', 10)
   sleep = kwargs.get('sleep', 0)
   question = kwargs.get('query')
   log = kwargs.get('log', False)
   query_type = kwargs.get('query_type', 'stock')
   data = {
     'perpage': 10,
@@ -42,42 +42,54 @@
   while count < retry :
     time.sleep(sleep)
     res = rq.request(
       method='POST',
       url='http://www.iwencai.com/customized/chart/get-robot-data',
       json=data,
       headers={
-        'hexin-v': getToken(),
+        'hexin-v': get_token(),
         'User-Agent': ua.random
       }
     )
     result = json.loads(res.text)
-    params = {
-      'condition': result['data']['answer'][0]['txt'][0]['content']['components'][0]['data']['meta']['extra']['condition'],
-      'comp_id': result['data']['answer'][0]['txt'][0]['content']['components'][0]['cid'],
-      'uuid': result['data']['answer'][0]['txt'][0]['content']['components'][0]['puuid']
-    }
+    content = result['data']['answer'][0]['txt'][0]['content']
+    if type(content) == str:
+      content = json.loads(content)
+    components0 = content['components'][0]
+    meta = components0['data']['meta']
+    params = {}
+    if meta:
+      params = {
+        'condition': components0['data']['meta']['extra']['condition'],
+        'comp_id': components0['cid'],
+        'uuid': components0['puuid']
+      }
+    else:
+      datas = components0['data']['datas']
+      params = {
+        'datas': pd.DataFrame.from_dict(datas)
+      }
     
-    log and logging.info(f'获取params成功')
+    log and logging.info(f'获取get_robot_data成功')
     return params
-  log and logging.info(f'获取params失败')
+  log and logging.info(f'获取get_robot_data失败')
   return None
 
 # 替换key
 def replace_key(key):
     key_map = {
         'question': 'query',
         'sort_key': 'urp_sort_index',
         'sort_order': 'urp_sort_way'
     }
     return key_map.get(key, key)
 
 
 # 获取每页数据
-def getPage(**kwargs):
+def get_page(**kwargs):
   retry = kwargs.pop('retry', 10)
   sleep = kwargs.pop('sleep', 0)
   log = kwargs.pop('log', False)
 
   data = {
     'perpage': 100,
     'page': 1,
@@ -91,15 +103,15 @@
     time.sleep(sleep)
     try: 
       res = rq.request(
         method='POST',
         url='http://www.iwencai.com/gateway/urp/v7/landing/getDataList',
         data=data,
         headers={
-          'hexin-v': getToken(),
+          'hexin-v': get_token(),
           'User-Agent': ua.random
         },
         timeout=(5, 10)
       )
       result = json.loads(res.text)
       list = result['answer']['components'][0]['data']['datas']
       log and logging.info(f'第{data.get("page")}页成功')
@@ -108,43 +120,47 @@
       log and logging.warning(f'{count+1}次尝试失败')
       count+=1
   log and logging.error(f'第{data.get("page")}页失败')
   return pd.DataFrame.from_dict([])
   
 
 # 是否继续循环
-def canLoop(loop, count):
+def can_loop(loop, count):
   if (loop is True):
     return True
   else: 
     return count < loop
 
 # 循环分页
-def loopPage(loop, **kwargs):
+def loop_page(loop, **kwargs):
   count = 0
   resultPageLen = 1
   result = None
   if 'page' not in kwargs:
     kwargs['page'] = 1
   initPage = kwargs['page']
 
-  while resultPageLen > 0 and canLoop(loop, count):
+  while resultPageLen > 0 and can_loop(loop, count):
     kwargs['page'] = initPage + count
-    resultPage = getPage(**kwargs)
+    resultPage = get_page(**kwargs)
     resultPageLen = len(resultPage)
     count = count + 1
     if result is None:
       result = resultPage
     else:
       result = pd.concat([result, resultPage], ignore_index=True)
   
   return result
 
 # 获取结果
 def get(loop=False, **kwargs):
   kwargs = {replace_key(key): value for key, value in kwargs.items()}
-  params = getParams(**kwargs)
-  kwargs = {**kwargs, **params}
-  if loop:
-    return loopPage(loop, **kwargs)
+  params = get_robot_data(**kwargs)
+  datas = params.get('datas', None)
+  if datas is not None:
+    return datas
   else:
-    return getPage(**kwargs)
+    kwargs = {**kwargs, **params}
+    if loop:
+      return loop_page(loop, **kwargs)
+    else:
+      return get_page(**kwargs)
```

### Comparing `pywencai-0.6.0/PKG-INFO` & `pywencai-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywencai
-Version: 0.6.0
+Version: 0.7.0
 Summary: 
 Author: pluto
 Author-email: mayuanchi1029@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -88,14 +88,20 @@
 | 取值 | 含义 |
 |-|-|
 | stock | 股票 |
 | zhishu | 指数 |
 | fund | 基金 |
 | hkstock | 港股 |
 | usstock | 美股 |
+| threeboard | 新三板 |
+| conbond | 可转债 |
+| insurance | 保险 |
+| futures | 期货 |
+| lccp | 理财 |
+| foreign_exchange | 外汇 |
 
 #### retry
 
 非必填，默认为10，表示请求失败后的重试次数。
 
 #### sleep
```

