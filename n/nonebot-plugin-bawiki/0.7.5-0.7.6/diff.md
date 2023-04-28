# Comparing `tmp/nonebot_plugin_bawiki-0.7.5.tar.gz` & `tmp/nonebot_plugin_bawiki-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bawiki-0.7.5.tar", last modified: Tue Apr 25 14:30:55 2023, max compression
+gzip compressed data, was "nonebot_plugin_bawiki-0.7.6.tar", last modified: Fri Apr 28 10:10:45 2023, max compression
```

## Comparing `nonebot_plugin_bawiki-0.7.5.tar` & `nonebot_plugin_bawiki-0.7.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1068 2023-04-25 14:30:37.375213 nonebot_plugin_bawiki-0.7.5/LICENSE
--rw-r--r--   0        0        0     7660 2023-04-25 14:30:37.375213 nonebot_plugin_bawiki-0.7.5/README.md
--rw-r--r--   0        0        0    15528 2023-04-25 14:30:37.375213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/__init__.py
--rw-r--r--   0        0        0    22575 2023-04-25 14:30:37.375213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/__main__.py
--rw-r--r--   0        0        0     1881 2023-04-25 14:30:37.375213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/config.py
--rw-r--r--   0        0        0     5812 2023-04-25 14:30:37.375213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/data_bawiki.py
--rw-r--r--   0        0        0     8291 2023-04-25 14:30:37.375213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/data_gamekee.py
--rw-r--r--   0        0        0    18827 2023-04-25 14:30:37.375213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/data_schaledb.py
--rw-r--r--   0        0        0     7390 2023-04-25 14:30:37.375213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/gacha.py
--rw-r--r--   0        0        0    21514 2023-04-25 14:30:37.375213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/calender_banner.png
--rw-r--r--   0        0        0  1685142 2023-04-25 14:30:37.375213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_bg.png
--rw-r--r--   0        0        0    13956 2023-04-25 14:30:37.379213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_card_bg.png
--rw-r--r--   0        0        0     2408 2023-04-25 14:30:37.379213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_card_mask.png
--rw-r--r--   0        0        0     4391 2023-04-25 14:30:37.379213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_new.png
--rw-r--r--   0        0        0    10375 2023-04-25 14:30:37.379213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_pickup.png
--rw-r--r--   0        0        0     2022 2023-04-25 14:30:37.379213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_star.png
--rw-r--r--   0        0        0    14652 2023-04-25 14:30:37.379213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_stu_err.png
--rw-r--r--   0        0        0  1764190 2023-04-25 14:30:37.379213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gradient.png
--rw-r--r--   0        0        0      872 2023-04-25 14:30:37.379213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/resource.py
--rw-r--r--   0        0        0     3555 2023-04-25 14:30:37.379213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/util.py
--rw-r--r--   0        0        0     1381 2023-04-25 14:30:55.087487 nonebot_plugin_bawiki-0.7.5/pyproject.toml
--rw-r--r--   0        0        0     9001 1970-01-01 00:00:00.000000 nonebot_plugin_bawiki-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-28 10:10:23.451967 nonebot_plugin_bawiki-0.7.6/LICENSE
+-rw-r--r--   0        0        0     7712 2023-04-28 10:10:23.451967 nonebot_plugin_bawiki-0.7.6/README.md
+-rw-r--r--   0        0        0    15528 2023-04-28 10:10:23.451967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/__init__.py
+-rw-r--r--   0        0        0    22651 2023-04-28 10:10:23.451967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/__main__.py
+-rw-r--r--   0        0        0     1881 2023-04-28 10:10:23.451967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/config.py
+-rw-r--r--   0        0        0     5812 2023-04-28 10:10:23.451967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/data_bawiki.py
+-rw-r--r--   0        0        0     8291 2023-04-28 10:10:23.451967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/data_gamekee.py
+-rw-r--r--   0        0        0    18827 2023-04-28 10:10:23.455967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/data_schaledb.py
+-rw-r--r--   0        0        0     7390 2023-04-28 10:10:23.455967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/gacha.py
+-rw-r--r--   0        0        0    21514 2023-04-28 10:10:23.455967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/calender_banner.png
+-rw-r--r--   0        0        0  1685142 2023-04-28 10:10:23.455967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_bg.png
+-rw-r--r--   0        0        0    13956 2023-04-28 10:10:23.455967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_card_bg.png
+-rw-r--r--   0        0        0     2408 2023-04-28 10:10:23.455967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_card_mask.png
+-rw-r--r--   0        0        0     4391 2023-04-28 10:10:23.455967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_new.png
+-rw-r--r--   0        0        0    10375 2023-04-28 10:10:23.455967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_pickup.png
+-rw-r--r--   0        0        0     2022 2023-04-28 10:10:23.455967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_star.png
+-rw-r--r--   0        0        0    14652 2023-04-28 10:10:23.455967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_stu_err.png
+-rw-r--r--   0        0        0  1764190 2023-04-28 10:10:23.459967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gradient.png
+-rw-r--r--   0        0        0      872 2023-04-28 10:10:23.459967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/resource.py
+-rw-r--r--   0        0        0     3555 2023-04-28 10:10:23.459967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/util.py
+-rw-r--r--   0        0        0     1381 2023-04-28 10:10:45.620214 nonebot_plugin_bawiki-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0     9053 1970-01-01 00:00:00.000000 nonebot_plugin_bawiki-0.7.6/PKG-INFO
```

### Comparing `nonebot_plugin_bawiki-0.7.5/LICENSE` & `nonebot_plugin_bawiki-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.5/README.md` & `nonebot_plugin_bawiki-0.7.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,18 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.7.6
+
+- 修复卡池为空不会提示的 bug
+
 ### 0.7.5
 
 - 插件可以自动帮你配置 PicMenu 的字体了
 - 给抽卡新增了冷却
 
 ### 0.7.2 ~ 0.7.4
```

#### html2text {}

```diff
@@ -39,17 +39,18 @@
 126.com> ## ð¡ é¸£è°¢ ### [RainNight0](https://github.com/RainNight0) -
 æ¥ç¨è¡¨ html æ¨¡æ¿æä¾ï¼å·²å¼ç¨ï¼ ### `bawiki-data`
 æ°æ®æºè´¡ç®åè¡¨ - è§ [bawiki-data](http://github.com/lgc2333/bawiki-
 data) ## ð° èµå© æè°¢åä½å¤§ä½¬çæåâ¦â¦ï¼ï¼æ¬ fw
 å®å¨ææ¿ä¸å°½â¦â¦ - [ç±åçµ](https://afdian.net/@lgc2333) -
 èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ ![è®¨é¥­](https://raw.githubusercontent.com/
 lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ###
-0.7.5 - æä»¶å¯ä»¥èªå¨å¸®ä½ éç½® PicMenu çå­ä½äº -
-ç»æ½å¡æ°å¢äºå·å´ ### 0.7.2 ~ 0.7.4 - ä¿®å¤ bug ### 0.7.1 -
-æ´æ¹éç½®é¡¹åç§° ### 0.7.0 - ä¿®å¤ SchaleDB æºæ¥ç¨è¡¨åºéçé®é¢ -
+0.7.6 - ä¿®å¤å¡æ± ä¸ºç©ºä¸ä¼æç¤ºç bug ### 0.7.5 -
+æä»¶å¯ä»¥èªå¨å¸®ä½ éç½® PicMenu çå­ä½äº - ç»æ½å¡æ°å¢äºå·å´
+### 0.7.2 ~ 0.7.4 - ä¿®å¤ bug ### 0.7.1 - æ´æ¹éç½®é¡¹åç§° ### 0.7.0 -
+ä¿®å¤ SchaleDB æºæ¥ç¨è¡¨åºéçé®é¢ -
 æ·»å äºå ä¸ªéç½®é¡¹ï¼ç°å¨å¯ä»¥å¨ `.env`
 æä»¶ä¸­ä¿®æ¹æ°æ®æºé¾æ¥äº - ä¿®æ¹äºé»è®¤æ°æ®æºé¾æ¥ -
 ä¹°äºä¸çäºç CDNï¼è®¾ç½®çæ°æ®ç¼å­ 12
 å°æ¶ãä¸ç¥éç°å¨éåº¦æä¹æ ·â¦â¦
 å¸æä¸è¦æäººææææâ¦â¦ æè°¢å¤§ä½¬åç¨çå·²å¤æ¡åå
 [cyberczy.xyz](http://cyberczy.xyz/)ï¼ - å¶ä»å°æ´æ¹ ### 0.6.4 -
 ä¿®å¤ç±äº `imageutils` æ¥å£æ¹å¨é æçç»å¾å¤±è´¥ç bug ### 0.6.3 -
```

### Comparing `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/__init__.py` & `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from nonebot.plugin import PluginMetadata
 
 require("nonebot_plugin_apscheduler")
 require("nonebot_plugin_htmlrender")
 
 from . import __main__ as __main__  # noqa: E402
 
-__version__ = "0.7.5"
+__version__ = "0.7.6"
 __plugin_meta__ = PluginMetadata(
     name="BAWiki",
     description="碧蓝档案Wiki插件",
     usage=(
         "感谢各位sensei使用本插件！\n"
         "插件有缓存机制，每3小时自动清空一次，如果插件遇到问题可以先手动清空缓存试一下捏\n"
         "装载PicMenu插件即可查看插件详细菜单哦\n"
```

### Comparing `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/__main__.py` & `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -576,14 +576,17 @@
 
 
 def get_1st_pool(data: dict) -> Optional[GachaPool]:
     if not data:
         return None
 
     pool_data = data["current_pools"]
+    if not pool_data:
+        return None
+
     pool = pool_data[0]
     return GachaPool(name=pool["name"], pool=pool["pool"], index=0)
 
 
 change_pool = on_command("ba切换卡池")
 
 
@@ -620,18 +623,19 @@
         try:
             gacha_data = await db_get_gacha_data()
         except:
             logger.exception("获取抽卡基本数据失败")
             await matcher.finish("获取抽卡基本数据失败，请检查后台输出")
 
         pool_data = gacha_data["current_pools"]
-        if not pool_data:
+        first_pool = get_1st_pool(gacha_data)
+        if not first_pool:
             await matcher.finish("当前没有可切换的卡池")
 
-        pool_obj = gacha_pool_index.get(qq) or get_1st_pool(gacha_data)
+        pool_obj = gacha_pool_index.get(qq) or first_pool
         if not pool_obj:
             await matcher.finish("当前没有UP池可供切换")
 
         if (index := pool_obj.index) is not None:
             index += 1
             if len(pool_data) <= index:
                 index = 0
```

### Comparing `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/config.py` & `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/data_bawiki.py` & `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/data_bawiki.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/data_gamekee.py` & `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/data_gamekee.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/data_schaledb.py` & `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/data_schaledb.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/gacha.py` & `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/gacha.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/calender_banner.png` & `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/calender_banner.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_bg.png` & `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_bg.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_card_bg.png` & `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_card_bg.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_card_mask.png` & `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_card_mask.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_new.png` & `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_new.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_pickup.png` & `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_pickup.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_star.png` & `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_star.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_stu_err.png` & `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_stu_err.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gradient.png` & `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gradient.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/resource.py` & `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/resource.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/util.py` & `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/util.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.5/pyproject.toml` & `nonebot_plugin_bawiki-0.7.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-bawiki"
-version = "0.7.5"
+version = "0.7.6"
 description = "A nonebot2 plugin for Blue Archive."
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "aiohttp>=3.8.3",
     "nonebot2>=2.0.0b5",
```

### Comparing `nonebot_plugin_bawiki-0.7.5/PKG-INFO` & `nonebot_plugin_bawiki-0.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bawiki
-Version: 0.7.5
+Version: 0.7.6
 Summary: A nonebot2 plugin for Blue Archive.
 Keywords: blue archive nonebot nonebot2 bot qq
 Home-page: https://github.com/lgc2333/nonebot-plugin-bawiki/
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Topic :: Communications
@@ -184,14 +184,18 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.7.6
+
+- 修复卡池为空不会提示的 bug
+
 ### 0.7.5
 
 - 插件可以自动帮你配置 PicMenu 的字体了
 - 给抽卡新增了冷却
 
 ### 0.7.2 ~ 0.7.4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bawiki Version: 0.7.5 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-bawiki Version: 0.7.6 Summary: A
 nonebot2 plugin for Blue Archive. Keywords: blue archive nonebot nonebot2 bot
 qq Home-page: https://github.com/lgc2333/nonebot-plugin-bawiki/ Author-Email:
 student_2333
 126.com> License: MIT Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Topic :: Communications Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Communications :: Chat :: ICQ Classifier: Topic :: Games/
 Entertainment Classifier: Topic :: Games/Entertainment :: Board Games
@@ -58,17 +58,18 @@
 126.com> ## ð¡ é¸£è°¢ ### [RainNight0](https://github.com/RainNight0) -
 æ¥ç¨è¡¨ html æ¨¡æ¿æä¾ï¼å·²å¼ç¨ï¼ ### `bawiki-data`
 æ°æ®æºè´¡ç®åè¡¨ - è§ [bawiki-data](http://github.com/lgc2333/bawiki-
 data) ## ð° èµå© æè°¢åä½å¤§ä½¬çæåâ¦â¦ï¼ï¼æ¬ fw
 å®å¨ææ¿ä¸å°½â¦â¦ - [ç±åçµ](https://afdian.net/@lgc2333) -
 èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ ![è®¨é¥­](https://raw.githubusercontent.com/
 lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ###
-0.7.5 - æä»¶å¯ä»¥èªå¨å¸®ä½ éç½® PicMenu çå­ä½äº -
-ç»æ½å¡æ°å¢äºå·å´ ### 0.7.2 ~ 0.7.4 - ä¿®å¤ bug ### 0.7.1 -
-æ´æ¹éç½®é¡¹åç§° ### 0.7.0 - ä¿®å¤ SchaleDB æºæ¥ç¨è¡¨åºéçé®é¢ -
+0.7.6 - ä¿®å¤å¡æ± ä¸ºç©ºä¸ä¼æç¤ºç bug ### 0.7.5 -
+æä»¶å¯ä»¥èªå¨å¸®ä½ éç½® PicMenu çå­ä½äº - ç»æ½å¡æ°å¢äºå·å´
+### 0.7.2 ~ 0.7.4 - ä¿®å¤ bug ### 0.7.1 - æ´æ¹éç½®é¡¹åç§° ### 0.7.0 -
+ä¿®å¤ SchaleDB æºæ¥ç¨è¡¨åºéçé®é¢ -
 æ·»å äºå ä¸ªéç½®é¡¹ï¼ç°å¨å¯ä»¥å¨ `.env`
 æä»¶ä¸­ä¿®æ¹æ°æ®æºé¾æ¥äº - ä¿®æ¹äºé»è®¤æ°æ®æºé¾æ¥ -
 ä¹°äºä¸çäºç CDNï¼è®¾ç½®çæ°æ®ç¼å­ 12
 å°æ¶ãä¸ç¥éç°å¨éåº¦æä¹æ ·â¦â¦
 å¸æä¸è¦æäººææææâ¦â¦ æè°¢å¤§ä½¬åç¨çå·²å¤æ¡åå
 [cyberczy.xyz](http://cyberczy.xyz/)ï¼ - å¶ä»å°æ´æ¹ ### 0.6.4 -
 ä¿®å¤ç±äº `imageutils` æ¥å£æ¹å¨é æçç»å¾å¤±è´¥ç bug ### 0.6.3 -
```

