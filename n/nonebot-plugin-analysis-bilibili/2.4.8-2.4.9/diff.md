# Comparing `tmp/nonebot_plugin_analysis_bilibili-2.4.8.tar.gz` & `tmp/nonebot_plugin_analysis_bilibili-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_analysis_bilibili-2.4.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_analysis_bilibili-2.4.9.tar", max compression
```

## Comparing `nonebot_plugin_analysis_bilibili-2.4.8.tar` & `nonebot_plugin_analysis_bilibili-2.4.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2011 2023-01-05 09:01:04.099696 nonebot_plugin_analysis_bilibili-2.4.8/README.md
--rw-r--r--   0        0        0     1503 2023-01-05 09:01:04.103696 nonebot_plugin_analysis_bilibili-2.4.8/nonebot_plugin_analysis_bilibili/__init__.py
--rw-r--r--   0        0        0    14819 2023-01-05 09:01:04.103696 nonebot_plugin_analysis_bilibili-2.4.8/nonebot_plugin_analysis_bilibili/analysis_bilibili.py
--rw-r--r--   0        0        0      576 2023-01-05 09:01:04.103696 nonebot_plugin_analysis_bilibili-2.4.8/pyproject.toml
--rw-r--r--   0        0        0     2865 1970-01-01 00:00:00.000000 nonebot_plugin_analysis_bilibili-2.4.8/setup.py
--rw-r--r--   0        0        0     2872 1970-01-01 00:00:00.000000 nonebot_plugin_analysis_bilibili-2.4.8/PKG-INFO
+-rw-r--r--   0        0        0     2011 2023-02-09 18:26:30.646797 nonebot_plugin_analysis_bilibili-2.4.9/README.md
+-rw-r--r--   0        0        0     1503 2023-02-09 18:26:30.646797 nonebot_plugin_analysis_bilibili-2.4.9/nonebot_plugin_analysis_bilibili/__init__.py
+-rw-r--r--   0        0        0    14823 2023-02-09 18:26:30.646797 nonebot_plugin_analysis_bilibili-2.4.9/nonebot_plugin_analysis_bilibili/analysis_bilibili.py
+-rw-r--r--   0        0        0      576 2023-02-09 18:26:30.646797 nonebot_plugin_analysis_bilibili-2.4.9/pyproject.toml
+-rw-r--r--   0        0        0     2865 1970-01-01 00:00:00.000000 nonebot_plugin_analysis_bilibili-2.4.9/setup.py
+-rw-r--r--   0        0        0     2872 1970-01-01 00:00:00.000000 nonebot_plugin_analysis_bilibili-2.4.9/PKG-INFO
```

### Comparing `nonebot_plugin_analysis_bilibili-2.4.8/README.md` & `nonebot_plugin_analysis_bilibili-2.4.9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_analysis_bilibili-2.4.8/nonebot_plugin_analysis_bilibili/__init__.py` & `nonebot_plugin_analysis_bilibili-2.4.9/nonebot_plugin_analysis_bilibili/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_analysis_bilibili-2.4.8/nonebot_plugin_analysis_bilibili/analysis_bilibili.py` & `nonebot_plugin_analysis_bilibili-2.4.9/nonebot_plugin_analysis_bilibili/analysis_bilibili.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             url = f"https://api.vc.bilibili.com/dynamic_svr/v1/dynamic_svr/get_dynamic_detail?dynamic_id={dynamic_id[2]}"
         return url, page, time
     except Exception:
         return "", None, None
 
 
 async def search_bili_by_title(title: str) -> str:
-    search_url = f"https://api.bilibili.com/x/web-interface/search/all/v2?keyword={urllib.parse.quote(title)}"
+    search_url = f"https://api.bilibili.com/x/web-interface/wbi/search/all/v2?keyword={urllib.parse.quote(title)}"
 
     async with aiohttp.request(
         "GET", search_url, timeout=aiohttp.client.ClientTimeout(10)
     ) as resp:
         result = (await resp.json())["data"]["result"]
 
     for i in result:
```

### Comparing `nonebot_plugin_analysis_bilibili-2.4.8/pyproject.toml` & `nonebot_plugin_analysis_bilibili-2.4.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-analysis-bilibili"
-version = "2.4.8"
+version = "2.4.9"
 description = "nonebot2解析bilibili插件"
 authors = ["mengshouer"]
 license = "MIT"
 readme = "README.md"
 
 repository = "https://github.com/mengshouer/nonebot_plugin_analysis_bilibili"
 keywords = ["nonebot", "nonebot2", "bilibili"]
```

### Comparing `nonebot_plugin_analysis_bilibili-2.4.8/setup.py` & `nonebot_plugin_analysis_bilibili-2.4.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['aiohttp>=3.7,<4.0',
  'nonebot-adapter-onebot>=2.0.0-beta.1,<3.0.0',
  'nonebot2>=2.0.0-beta.5,<3.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-analysis-bilibili',
-    'version': '2.4.8',
+    'version': '2.4.9',
     'description': 'nonebot2解析bilibili插件',
     'long_description': '<!--\n * @Author         : mengshouer\n * @Date           : 2021-03-16 00:00:00\n * @LastEditors    : mengshouer\n * @LastEditTime   : 2021-03-16 00:00:00\n * @Description    : None\n * @GitHub         : https://github.com/mengshouer/nonebot_plugin_analysis_bilibili\n-->\n\n<p align="center">\n  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>\n</p>\n\n<div align="center">\n\n# nonebot_plugin_analysis_bilibili\n\n_✨ NoneBot bilibili 视频、番剧解析插件 ✨_\n\n</div>\n\n<p align="center">\n  <a href="https://raw.githubusercontent.com/cscs181/QQ-Github-Bot/master/LICENSE">\n    <img src="https://img.shields.io/github/license/cscs181/QQ-Github-Bot.svg" alt="license">\n  </a>\n  <a href="https://pypi.python.org/pypi/nonebot-plugin-analysis-bilibili">\n    <img src="https://img.shields.io/pypi/v/nonebot-plugin-analysis-bilibili.svg" alt="pypi">\n  </a>\n  <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">\n</p>\n\n## 使用方式\n\n私聊或群聊发送 bilibili 的小程序/链接\n\n## 额外配置项(可选)\n\n在配置文件中加入\n\n```\nanalysis_blacklist = [123456789] # 不解析里面填写的QQ号发的链接 List[int]\nanalysis_group_blacklist = [123456789] # 不解析里面填写的QQ群号发的链接 List[int]\nanalysis_display_image = true # 是否显示封面 true/false\n\n# 哪种类型需要显示封面，与上一项相冲突，上一项为true则全开 List[str]\nanalysis_display_image_list = ["video", "bangumi", "live", "article", "dynamic"]\n```\n\n## 安装\n\n1. 使用 nb-cli 安装，不需要手动添加入口，更新使用 pip\n\n```\nnb plugin install nonebot_plugin_analysis_bilibili\n```\n\n2. 使用 pip 安装和更新，初次安装需要手动添加入口\n\n```\npip install --upgrade nonebot_plugin_analysis_bilibili\n```\n\npip 安装后在 Nonebot2 入口文件（例如 bot.py ）增加：\n\n```python\nnonebot.load_plugin("nonebot_plugin_analysis_bilibili")\n```\n\n附：支持 a16 最后一版为 2.4.3\n',
     'author': 'mengshouer',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mengshouer/nonebot_plugin_analysis_bilibili',
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_analysis_bilibili'] package_data = \ {'': ['*']}
 install_requires = \ ['aiohttp>=3.7,<4.0', 'nonebot-adapter-onebot>=2.0.0-
 beta.1,<3.0.0', 'nonebot2>=2.0.0-beta.5,<3.0.0'] setup_kwargs = { 'name':
-'nonebot-plugin-analysis-bilibili', 'version': '2.4.8', 'description':
+'nonebot-plugin-analysis-bilibili', 'version': '2.4.9', 'description':
 'nonebot2è§£æbilibiliæä»¶', 'long_description': '\n\n
                                 \n [nonebot]\n
 \n\n
         \n\n# nonebot_plugin_analysis_bilibili\n\n_â¨ NoneBot bilibili
                      è§é¢ãçªå§è§£ææä»¶ â¨_\n\n
 \n\n
                  \n \n_[license]\n\n \n_[pypi]\n\n [python]\n
```

### Comparing `nonebot_plugin_analysis_bilibili-2.4.8/PKG-INFO` & `nonebot_plugin_analysis_bilibili-2.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-analysis-bilibili
-Version: 2.4.8
+Version: 2.4.9
 Summary: nonebot2解析bilibili插件
 Home-page: https://github.com/mengshouer/nonebot_plugin_analysis_bilibili
 License: MIT
 Keywords: nonebot,nonebot2,bilibili
 Author: mengshouer
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-analysis-bilibili Version: 2.4.8
+Metadata-Version: 2.1 Name: nonebot-plugin-analysis-bilibili Version: 2.4.9
 Summary: nonebot2è§£æbilibiliæä»¶ Home-page: https://github.com/mengshouer/
 nonebot_plugin_analysis_bilibili License: MIT Keywords:
 nonebot,nonebot2,bilibili Author: mengshouer Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

