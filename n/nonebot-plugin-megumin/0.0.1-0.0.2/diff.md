# Comparing `tmp/nonebot-plugin-megumin-0.0.1.tar.gz` & `tmp/nonebot-plugin-megumin-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-megumin-0.0.1.tar", last modified: Fri Apr 28 07:27:57 2023, max compression
+gzip compressed data, was "nonebot-plugin-megumin-0.0.2.tar", last modified: Fri Apr 28 07:37:02 2023, max compression
```

## Comparing `nonebot-plugin-megumin-0.0.1.tar` & `nonebot-plugin-megumin-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 07:27:57.394640 nonebot-plugin-megumin-0.0.1/
--rw-rw-rw-   0        0        0     3233 2023-04-28 07:27:57.390654 nonebot-plugin-megumin-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2632 2023-04-26 15:47:44.000000 nonebot-plugin-megumin-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 07:27:57.330400 nonebot-plugin-megumin-0.0.1/nonebot_plugin_megumin/
--rw-rw-rw-   0        0        0     5126 2023-04-26 12:45:59.000000 nonebot-plugin-megumin-0.0.1/nonebot_plugin_megumin/__init__.py
--rw-rw-rw-   0        0        0      491 2023-04-26 12:45:57.000000 nonebot-plugin-megumin-0.0.1/nonebot_plugin_megumin/cfg.py
--rw-rw-rw-   0        0        0     2925 2023-04-26 12:45:53.000000 nonebot-plugin-megumin-0.0.1/nonebot_plugin_megumin/charm.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:27:57.379099 nonebot-plugin-megumin-0.0.1/nonebot_plugin_megumin.egg-info/
--rw-rw-rw-   0        0        0     3233 2023-04-28 07:27:56.000000 nonebot-plugin-megumin-0.0.1/nonebot_plugin_megumin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-04-28 07:27:57.000000 nonebot-plugin-megumin-0.0.1/nonebot_plugin_megumin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 07:27:56.000000 nonebot-plugin-megumin-0.0.1/nonebot_plugin_megumin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-04-28 07:27:56.000000 nonebot-plugin-megumin-0.0.1/nonebot_plugin_megumin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 07:27:57.400099 nonebot-plugin-megumin-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1121 2023-04-28 07:09:09.000000 nonebot-plugin-megumin-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:37:02.383166 nonebot-plugin-megumin-0.0.2/
+-rw-rw-rw-   0        0        0     3233 2023-04-28 07:37:02.375658 nonebot-plugin-megumin-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2632 2023-04-28 07:36:34.000000 nonebot-plugin-megumin-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 07:37:02.257128 nonebot-plugin-megumin-0.0.2/nonebot_plugin_megumin/
+-rw-rw-rw-   0        0        0     5195 2023-04-28 07:36:01.000000 nonebot-plugin-megumin-0.0.2/nonebot_plugin_megumin/__init__.py
+-rw-rw-rw-   0        0        0      491 2023-04-26 12:45:57.000000 nonebot-plugin-megumin-0.0.2/nonebot_plugin_megumin/cfg.py
+-rw-rw-rw-   0        0        0     2925 2023-04-26 12:45:53.000000 nonebot-plugin-megumin-0.0.2/nonebot_plugin_megumin/charm.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:37:02.369516 nonebot-plugin-megumin-0.0.2/nonebot_plugin_megumin.egg-info/
+-rw-rw-rw-   0        0        0     3233 2023-04-28 07:37:01.000000 nonebot-plugin-megumin-0.0.2/nonebot_plugin_megumin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-04-28 07:37:01.000000 nonebot-plugin-megumin-0.0.2/nonebot_plugin_megumin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 07:37:01.000000 nonebot-plugin-megumin-0.0.2/nonebot_plugin_megumin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-04-28 07:37:01.000000 nonebot-plugin-megumin-0.0.2/nonebot_plugin_megumin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 07:37:02.384151 nonebot-plugin-megumin-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1121 2023-04-28 07:33:43.000000 nonebot-plugin-megumin-0.0.2/setup.py
```

### Comparing `nonebot-plugin-megumin-0.0.1/PKG-INFO` & `nonebot-plugin-megumin-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-megumin
-Version: 0.0.1
+Version: 0.0.2
 Summary:  让你的群友释放爆裂魔法吧！ 
 Author: youlanan
 Author-email: 
 Keywords: python,nonebot,explosion
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -55,20 +55,20 @@
 <details>
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
 
 <details>
 <summary>pip</summary>
 
-    pip install nonebot_plugin_megumin
+    pip install nonebot-plugin-megumin
 </details>
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
-    plugins = ["nonebot_plugin_megumin"]
+    plugins = ["nonebot-plugin-megumin"]
 
 </details>
 
 <details>
 <summary>下载 本仓库源码 安装</summary>
 
     下载后将 nonebot_plugin_megumin 丢进nb目录下的src/plugin目录下, 确保正确配置nb可以载入该目录内的插件
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-megumin Version: 0.0.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-megumin Version: 0.0.2 Summary:
 è®©ä½ çç¾¤åéæ¾çè£é­æ³å§ï¼ Author: youlanan Author-email:
 Keywords: python,nonebot,explosion Classifier: Development Status :: 1 -
 Planning Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: Unix Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
@@ -11,17 +11,17 @@
 ## ð± ä»ç» _å¯ä»¥è§¦å ä»¥è§é¢ãæè¯­é³+æå­
 å½¢å¼ççè£é­æ³_ _èªå¸¦å·å±å±è½ãå¯èªå®ä¹éæ¾ä¸è¡¥é­æ¬¡æ°_
 _è®©ç¾¤åé¢ç¥æå¼ºé­æ³çèºæ¯ä¸é­å_ _çè£é­æ³å¦å¦å¦
 (âÅá´Å)Û¶..._ ## ð§ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot_plugin_megumin   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
-è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install nonebot_plugin_megumin  æå¼
+è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install nonebot-plugin-megumin  æå¼
 nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
-é¨åè¿½å åå¥ plugins = ["nonebot_plugin_megumin"]   ä¸è½½
+é¨åè¿½å åå¥ plugins = ["nonebot-plugin-megumin"]   ä¸è½½
 æ¬ä»åºæºç  å®è£ ä¸è½½åå° nonebot_plugin_megumin
 ä¸¢è¿nbç®å½ä¸çsrc/pluginç®å½ä¸,
 ç¡®ä¿æ­£ç¡®éç½®nbå¯ä»¥è½½å¥è¯¥ç®å½åçæä»¶  -
 éè¦åéè§é¢æè¯­é³, æä»¥è¯·ç¡®ä¿ä½ å®è£å¹¶æ­£ç¡®éç½®äºffmpeg -
 å®æä¸è¿°æ­¥éª¤åï¼ä¸è½½é¡¹ç®' ççèµæºå 'ä¸­ç' Explosion.zip ',
 ææç¤ºå°èµæºæ¾ç½®å¨æå®ä½ç½®, ä»¥å®æå®è£ -
 å¯ä¾éæ©çè§¦åå½¢å¼ä¸ºè§é¢/è¯­é³/æ··å, å¨é¡¹ç®ç' cfg.py
```

### Comparing `nonebot-plugin-megumin-0.0.1/README.md` & `nonebot-plugin-megumin-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -39,20 +39,20 @@
 <details>
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
 
 <details>
 <summary>pip</summary>
 
-    pip install nonebot_plugin_megumin
+    pip install nonebot-plugin-megumin
 </details>
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
-    plugins = ["nonebot_plugin_megumin"]
+    plugins = ["nonebot-plugin-megumin"]
 
 </details>
 
 <details>
 <summary>下载 本仓库源码 安装</summary>
 
     下载后将 nonebot_plugin_megumin 丢进nb目录下的src/plugin目录下, 确保正确配置nb可以载入该目录内的插件
```

#### html2text {}

```diff
@@ -4,17 +4,17 @@
 ## ð± ä»ç» _å¯ä»¥è§¦å ä»¥è§é¢ãæè¯­é³+æå­
 å½¢å¼ççè£é­æ³_ _èªå¸¦å·å±å±è½ãå¯èªå®ä¹éæ¾ä¸è¡¥é­æ¬¡æ°_
 _è®©ç¾¤åé¢ç¥æå¼ºé­æ³çèºæ¯ä¸é­å_ _çè£é­æ³å¦å¦å¦
 (âÅá´Å)Û¶..._ ## ð§ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot_plugin_megumin   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
-è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install nonebot_plugin_megumin  æå¼
+è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install nonebot-plugin-megumin  æå¼
 nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
-é¨åè¿½å åå¥ plugins = ["nonebot_plugin_megumin"]   ä¸è½½
+é¨åè¿½å åå¥ plugins = ["nonebot-plugin-megumin"]   ä¸è½½
 æ¬ä»åºæºç  å®è£ ä¸è½½åå° nonebot_plugin_megumin
 ä¸¢è¿nbç®å½ä¸çsrc/pluginç®å½ä¸,
 ç¡®ä¿æ­£ç¡®éç½®nbå¯ä»¥è½½å¥è¯¥ç®å½åçæä»¶  -
 éè¦åéè§é¢æè¯­é³, æä»¥è¯·ç¡®ä¿ä½ å®è£å¹¶æ­£ç¡®éç½®äºffmpeg -
 å®æä¸è¿°æ­¥éª¤åï¼ä¸è½½é¡¹ç®' ççèµæºå 'ä¸­ç' Explosion.zip ',
 ææç¤ºå°èµæºæ¾ç½®å¨æå®ä½ç½®, ä»¥å®æå®è£ -
 å¯ä¾éæ©çè§¦åå½¢å¼ä¸ºè§é¢/è¯­é³/æ··å, å¨é¡¹ç®ç' cfg.py
```

### Comparing `nonebot-plugin-megumin-0.0.1/nonebot_plugin_megumin/__init__.py` & `nonebot-plugin-megumin-0.0.2/nonebot_plugin_megumin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,10 +130,10 @@
 exhelp = on_command("爆裂魔法帮助", aliases = {'爆裂魔法help', '补魔帮助'}, priority=90)
 @exhelp.handle()
 async def 帮助(event: GroupMessageEvent):
     玩家 = event.user_id
     今天 = await 时间()
     if 无魔防刷屏.get(玩家, {}).get(今天, 0) >= 6:
         return
-    await exp.send(f'吾名惠惠！\n乃浪漫炽热【爆裂魔法】支配者\n每日{释放极限}发的惊人力量！\n以{补魔极限}次【补魔】引渡魔力本源！\n为你之群聊献上爆炎！\n『Explosion！』')
+    await exp.send(f'吾名惠惠！\n乃浪漫炽热【爆裂魔法】支配者\n每日{释放极限}发的惊人力量！\n以{补魔极限}次【补魔】引渡魔力本源！\n为你之群聊献上爆炎！\n『Explosion！』\n\n详细介绍：https://github.com/youlanan/nonebot_plugin_megumin')
     无魔防刷屏.setdefault(玩家, {})
     无魔防刷屏[玩家][今天] = 无魔防刷屏[玩家].get(今天, 0) + 1
```

### Comparing `nonebot-plugin-megumin-0.0.1/nonebot_plugin_megumin/charm.py` & `nonebot-plugin-megumin-0.0.2/nonebot_plugin_megumin/charm.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-megumin-0.0.1/nonebot_plugin_megumin.egg-info/PKG-INFO` & `nonebot-plugin-megumin-0.0.2/nonebot_plugin_megumin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-megumin
-Version: 0.0.1
+Version: 0.0.2
 Summary:  让你的群友释放爆裂魔法吧！ 
 Author: youlanan
 Author-email: 
 Keywords: python,nonebot,explosion
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -55,20 +55,20 @@
 <details>
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
 
 <details>
 <summary>pip</summary>
 
-    pip install nonebot_plugin_megumin
+    pip install nonebot-plugin-megumin
 </details>
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
-    plugins = ["nonebot_plugin_megumin"]
+    plugins = ["nonebot-plugin-megumin"]
 
 </details>
 
 <details>
 <summary>下载 本仓库源码 安装</summary>
 
     下载后将 nonebot_plugin_megumin 丢进nb目录下的src/plugin目录下, 确保正确配置nb可以载入该目录内的插件
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-megumin Version: 0.0.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-megumin Version: 0.0.2 Summary:
 è®©ä½ çç¾¤åéæ¾çè£é­æ³å§ï¼ Author: youlanan Author-email:
 Keywords: python,nonebot,explosion Classifier: Development Status :: 1 -
 Planning Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: Unix Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
@@ -11,17 +11,17 @@
 ## ð± ä»ç» _å¯ä»¥è§¦å ä»¥è§é¢ãæè¯­é³+æå­
 å½¢å¼ççè£é­æ³_ _èªå¸¦å·å±å±è½ãå¯èªå®ä¹éæ¾ä¸è¡¥é­æ¬¡æ°_
 _è®©ç¾¤åé¢ç¥æå¼ºé­æ³çèºæ¯ä¸é­å_ _çè£é­æ³å¦å¦å¦
 (âÅá´Å)Û¶..._ ## ð§ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot_plugin_megumin   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
-è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install nonebot_plugin_megumin  æå¼
+è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install nonebot-plugin-megumin  æå¼
 nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
-é¨åè¿½å åå¥ plugins = ["nonebot_plugin_megumin"]   ä¸è½½
+é¨åè¿½å åå¥ plugins = ["nonebot-plugin-megumin"]   ä¸è½½
 æ¬ä»åºæºç  å®è£ ä¸è½½åå° nonebot_plugin_megumin
 ä¸¢è¿nbç®å½ä¸çsrc/pluginç®å½ä¸,
 ç¡®ä¿æ­£ç¡®éç½®nbå¯ä»¥è½½å¥è¯¥ç®å½åçæä»¶  -
 éè¦åéè§é¢æè¯­é³, æä»¥è¯·ç¡®ä¿ä½ å®è£å¹¶æ­£ç¡®éç½®äºffmpeg -
 å®æä¸è¿°æ­¥éª¤åï¼ä¸è½½é¡¹ç®' ççèµæºå 'ä¸­ç' Explosion.zip ',
 ææç¤ºå°èµæºæ¾ç½®å¨æå®ä½ç½®, ä»¥å®æå®è£ -
 å¯ä¾éæ©çè§¦åå½¢å¼ä¸ºè§é¢/è¯­é³/æ··å, å¨é¡¹ç®ç' cfg.py
```

### Comparing `nonebot-plugin-megumin-0.0.1/setup.py` & `nonebot-plugin-megumin-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # these things are needed for the README.md show on pypi
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = ' 让你的群友释放爆裂魔法吧！ '
 LONG_DESCRIPTION = ' Let your group members unleash their Explosion magic! '
 
 # Setting up
 setup(
     name="nonebot-plugin-megumin",
     version=VERSION,
```

