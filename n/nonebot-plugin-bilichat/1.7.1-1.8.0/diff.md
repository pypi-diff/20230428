# Comparing `tmp/nonebot_plugin_bilichat-1.7.1.tar.gz` & `tmp/nonebot_plugin_bilichat-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-1.7.1.tar", last modified: Wed Apr 26 17:17:42 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-1.8.0.tar", last modified: Fri Apr 28 16:13:20 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-1.7.1.tar` & `nonebot_plugin_bilichat-1.8.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0    34523 2023-04-26 17:17:10.874528 nonebot_plugin_bilichat-1.7.1/LICENSE
--rw-r--r--   0        0        0    11739 2023-04-26 17:17:10.874528 nonebot_plugin_bilichat-1.7.1/README.md
--rw-r--r--   0        0        0     6000 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     4809 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      871 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     6439 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0     8900 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3800 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      399 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      341 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2854 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1127 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0      387 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/model/content.py
--rw-r--r--   0        0        0       93 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0      323 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-04-26 17:17:10.886528 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1045 2023-04-26 17:17:10.886528 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     5681 2023-04-26 17:17:10.886528 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4856 2023-04-26 17:17:10.886528 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2359 2023-04-26 17:17:10.886528 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1448 2023-04-26 17:17:10.886528 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1068 2023-04-26 17:17:10.886528 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/utils.py
--rw-r--r--   0        0        0     1780 2023-04-26 17:17:10.886528 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1407 2023-04-26 17:17:42.078955 nonebot_plugin_bilichat-1.7.1/pyproject.toml
--rw-r--r--   0        0        0    13028 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-28 16:13:07.264203 nonebot_plugin_bilichat-1.8.0/LICENSE
+-rw-r--r--   0        0        0    11854 2023-04-28 16:13:07.264203 nonebot_plugin_bilichat-1.8.0/README.md
+-rw-r--r--   0        0        0     6000 2023-04-28 16:13:07.272203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     4809 2023-04-28 16:13:07.272203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-04-28 16:13:07.272203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-04-28 16:13:07.272203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-04-28 16:13:07.272203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      871 2023-04-28 16:13:07.272203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     6439 2023-04-28 16:13:07.272203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0     8900 2023-04-28 16:13:07.272203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3800 2023-04-28 16:13:07.272203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      399 2023-04-28 16:13:07.272203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-04-28 16:13:07.272203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0      387 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/model/content.py
+-rw-r--r--   0        0        0      503 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0    27359 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/model/newbing.py
+-rw-r--r--   0        0        0      323 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1045 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     5825 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4916 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2343 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1448 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1068 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/utils.py
+-rw-r--r--   0        0        0     1780 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1407 2023-04-28 16:13:20.916168 nonebot_plugin_bilichat-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0    13143 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.8.0/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-1.7.1/LICENSE` & `nonebot_plugin_bilichat-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.7.1/README.md` & `nonebot_plugin_bilichat-1.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -234,11 +234,12 @@
 在此感谢以下开发者(项目)对本项目做出的贡献：
 
 - [BibiGPT](https://github.com/JimmyLv/BibiGPT) 项目灵感来源
 - [bilibili-API-collect](https://github.com/SocialSisterYi/bilibili-API-collect) 易姐收集的各种 BiliBili Api 及其提供的 gRPC Api 调用方案
 - [BBot-Graia](https://github.com/djkcyl/BBot-Graia) 功能来源 ~~(我 牛 我 自 己)~~
 - [ABot-Graia](https://github.com/djkcyl/ABot-Graia) 永远怀念最好的 ABot 🙏
 - [nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template): 项目的 README 模板
+- [nonebot-plugin-bing-chat](https://github.com/Harry-Jing/nonebot-plugin-bing-chat): newbing解析的代码参考
 
 ## ⏳ Star 趋势
 
 [![Stargazers over time](https://starchart.cc/djkcyl/nonebot-plugin-bilichat.svg)](https://starchart.cc/djkcyl/nonebot-plugin-bilichat)
```

#### html2text {}

```diff
@@ -111,10 +111,11 @@
 (é¡¹ç®)å¯¹æ¬é¡¹ç®ååºçè´¡ç®ï¼ - [BibiGPT](https://github.com/JimmyLv/
 BibiGPT) é¡¹ç®çµææ¥æº - [bilibili-API-collect](https://github.com/
 SocialSisterYi/bilibili-API-collect) æå§æ¶éçåç§ BiliBili Api
 åå¶æä¾ç gRPC Api è°ç¨æ¹æ¡ - [BBot-Graia](https://github.com/djkcyl/
 BBot-Graia) åè½æ¥æº ~~(æ ç æ èª å·±)~~ - [ABot-Graia](https://
 github.com/djkcyl/ABot-Graia) æ°¸è¿æå¿µæå¥½ç ABot ð - [nonebot-
 plugin-template](https://github.com/A-kirami/nonebot-plugin-template):
-é¡¹ç®ç README æ¨¡æ¿ ## â³ Star è¶å¿ [![Stargazers over time](https://
-starchart.cc/djkcyl/nonebot-plugin-bilichat.svg)](https://starchart.cc/djkcyl/
-nonebot-plugin-bilichat)
+é¡¹ç®ç README æ¨¡æ¿ - [nonebot-plugin-bing-chat](https://github.com/Harry-
+Jing/nonebot-plugin-bing-chat): newbingè§£æçä»£ç åè ## â³ Star è¶å¿
+[![Stargazers over time](https://starchart.cc/djkcyl/nonebot-plugin-
+bilichat.svg)](https://starchart.cc/djkcyl/nonebot-plugin-bilichat)
```

### Comparing `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import json
 import random
 import re
 from collections import OrderedDict
 from pathlib import Path
-from typing import List, Dict
+from typing import List, Literal
 
 from EdgeGPT import Chatbot, ConversationStyle
 from nonebot.log import logger
 
 from ..config import plugin_config
 from ..lib.store import BING_APOLOGY
 from ..model.cache import Cache
-from ..model.exception import AbortError
+from ..model.exception import (
+    AbortError,
+    BingChatResponseException,
+)
+from ..model.newbing import BingChatResponse
 from ..optional import capture_exception  # type: ignore
 from .text_to_image import rich_text2image
 
 cookies = json.loads(Path(plugin_config.bilichat_newbing_cookie).read_text("utf-8"))  # type: ignore
 logger.info("Try init bing chatbot")
 init = False
 for count in range(5):
@@ -27,24 +31,24 @@
     except Exception as e:
         logger.error(f"Bing chatbot init failed, retrying {count+1}/5: {e}")
 
 if not init:
     raise RuntimeError("Bing chatbot init failed")
 
 
-def get_small_size_transcripts(title: str, text_data: List[str]):
+def get_small_size_transcripts(title: str, text_data: List[str], type_: Literal["视频字幕", "专栏文章"] = "视频字幕"):
     prompt = (
-        "使用以下Markdown模板为我总结视频字幕数据，除非字幕中的内容无意义，或者内容较少无法总结，或者未提供字幕数据，或者无有效内容，你就不使用模板回复，只回复“无意义”：\
-        ## 概述\
+        f"使用以下Markdown模板为我总结{type_}数据，除非{type_[2:]}中的内容无意义，或者内容较少无法总结，或者未提供{type_[2:]}数据，或者无有效内容，你就不使用模板回复，只回复“无意义”："
+        + "## 概述\
         {内容，尽可能精简总结内容不要太详细}\
         ## 要点\
         - {使用不重复并合适的emoji，仅限一个，禁止重复} {内容不换行大于15字，可多项，条数与有效内容数量呈正比}\
         不要随意翻译任何内容。仅使用中文总结。\
         不说与总结无关的其他内容，你的回复仅限固定格式提供的“概述”和“要点”两项。"
-        + f"视频标题为“{title}”，视频字幕数据如下，立刻开始总结："
+        + f"{type_[:2]}标题为“{title}”，{type_}数据如下，立刻开始总结："
     )
     unique_texts = list(OrderedDict.fromkeys(text_data))
     if plugin_config.bilichat_newbing_token_limit > 0:
         while len(",".join(unique_texts)) + len(prompt) > plugin_config.bilichat_newbing_token_limit:
             unique_texts.pop(random.randint(0, len(unique_texts) - 1))
     return prompt + ",".join(unique_texts)
 
@@ -52,79 +56,80 @@
 def newbing_summary_preprocess(ai_summary: str):
     # https://github.com/djkcyl/nonebot-plugin-bilichat/pull/18
     """Pre-process (clean) the summary content of newbing output"""
     if search_obj := re.search(r"##\s+概述\s+(.*)##\s+要点\s+(.*)", ai_summary, re.S):
         # content separation
         summary = search_obj[1].strip()
         bulletpoint = search_obj[2].strip()
-        # remove reference like [^1^]
-        summary = re.sub(r"\[\^\d+\^\]\s*", "", summary)
-        bulletpoint = re.sub(r"\[\^\d+\^\]\s*", "", bulletpoint)
         # reset line breaks
         bulletpoint = re.sub(r"-\s*\[(.+?)\]\s*", r"\n● \g<1> ", bulletpoint)
         bulletpoint = re.sub(r"\n+", r"\n", bulletpoint).strip()
         # final output
         bing_summary = f"## 总结\n{summary}\n\n## 要点\n{bulletpoint}"
         logger.info(f"Newbing summary: \n{bing_summary}")
         return bing_summary
     else:
         logger.debug(f"Newbing output is meaningless: \n{ai_summary}")
-        return None
+        return ""
 
 
 async def newbing_req(prompt: str):
     logger.debug(f"prompt have {len(prompt)} chars")
-    ans = await bot.ask(
+    raw = await bot.ask(
         prompt=prompt,
         conversation_style=ConversationStyle.creative,
         wss_link="wss://sydney.bing.com/sydney/ChatHub",
     )
     await bot.reset()
-    logger.debug(ans)
-    bing_resp: Dict = ans["item"]["messages"][1]
+    res = BingChatResponse(raw=raw)
     return (
-        newbing_summary_preprocess(bing_resp.get("text", ""))
+        newbing_summary_preprocess(res.content_answer)
         if plugin_config.bilichat_newbing_preprocess
-        else bing_resp.get("text", None)
+        else res.content_answer
     )
 
 
 async def newbing_summarization(cache: Cache, cid: str = "0"):
     meaning = False
     try:
         if not cache.episodes[cid].newbing:
             if cache.id[:2].lower() in ["bv", "av"]:
                 ai_summary = await newbing_req(get_small_size_transcripts(cache.title, cache.episodes[cid].content))
             elif cache.id[:2].lower() == "cv":
                 ai_summary = await newbing_req(
-                    get_small_size_transcripts(cache.title, re.split(r"[，。；,.;\n]+", cache.episodes[cid].content[0]))
+                    get_small_size_transcripts(cache.title, cache.episodes[cid].content, type_="专栏文章")
                 )
             else:
                 raise ValueError(f"Illegal Video(Column) types {cache.id}")
 
-            # 如果为空则是拒绝回答
-            if ai_summary is None:
-                return BING_APOLOGY.read_bytes(), False
-            # 大于 100 认为有意义
-            elif len(ai_summary) > 100:
+            # 大于 50 认为有意义
+            if len(ai_summary) > 50:
                 cache.episodes[cid].newbing = ai_summary
                 cache.save()
                 meaning = True
-            # 小于 100 认为无意义
+            # 小于 50 认为无意义
             else:
                 logger.warning(f"Video(Column) {cache.id} summary failure")
                 cache.episodes[cid].newbing = f"视频(专栏) {cache.id} 总结失败: {ai_summary}"
+
+        elif cache.episodes[cid].newbing == "Refusal to answer":
+            return BING_APOLOGY.read_bytes(), False
         else:
             meaning = True
             logger.info("Using cached newbing summarization")
 
-        if img := await rich_text2image(cache.episodes[cid].newbing or "视频无法总结", "new Bing(testing)"):
+        if img := await rich_text2image(cache.episodes[cid].newbing or "视频无法总结", "new Bing"):
             return img, meaning
         else:
             return f"总结图片生成失败, 直接发送原文:\n{cache.episodes[cid].newbing}", meaning
+    except BingChatResponseException as e:
+        logger.error(f"Video(Column) {cache.id} summary failed: {e}")
+        cache.episodes[cid].newbing = "Refusal to answer"
+        cache.save()
+        return BING_APOLOGY.read_bytes(), False
     except AbortError as e:
         logger.exception(f"Video(Column) {cache.id} summary aborted: {e}")
         return f"视频(专栏) {cache.id} 总结中止: {e}", False
     except Exception as e:
         capture_exception()
         logger.exception(f"Video(Column) {cache.id} summary failed: {e}")
         return f"视频(专栏) {cache.id} 总结失败: {e}", False
```

### Comparing `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/summary/openai.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import asyncio
 import random
 from collections import OrderedDict
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional,Literal
 
 import httpx
 import tiktoken_async
 from loguru import logger
 
 from ..config import plugin_config
 from ..model.openai import OpenAI, TokenUsage
 
 if plugin_config.bilichat_openai_token:
     logger.info("Loading OpenAI Token enc model")
     tiktoken_enc = asyncio.run(tiktoken_async.encoding_for_model(plugin_config.bilichat_openai_model))
     logger.success(f"Enc model {tiktoken_enc.name} load successfully")
 
 
-def get_summarise_prompt(title: str, transcript: str) -> List[Dict[str, str]]:
+def get_summarise_prompt(title: str, transcript: str, type_: Literal["视频字幕", "专栏文章"] = "视频字幕"):
     title = title.replace("\n", " ").strip() if title else ""
     transcript = transcript.replace("\n", " ").strip() if transcript else ""
     return get_full_prompt(
         prompt=(
-            "使用以下Markdown模板为我总结视频字幕数据，除非字幕中的内容无意义，或者内容较少无法总结，或者未提供字幕数据，或者无有效内容，你就不使用模板回复，只回复“无意义”："
+            f"使用以下Markdown模板为我总结{type_}数据，除非{type_[2:]}中的内容无意义，或者内容较少无法总结，或者未提供{type_[2:]}数据，或者无有效内容，你就不使用模板回复，只回复“无意义”："
             "\n## 概述"
             "\n{内容，尽可能精简总结内容不要太详细}"
             "\n## 要点"
             "\n- {使用不重复并合适的emoji，仅限一个，禁止重复} {内容不换行大于15字，可多项，条数与有效内容数量呈正比}"
             "\n不要随意翻译任何内容。仅使用中文总结。"
             "\n不说与总结无关的其他内容，你的回复仅限固定格式提供的“概述”和“要点”两项。"
-            f"\n视频标题名称为“{title}”，视频字幕数据如下，立刻开始总结：“{transcript}”"
+            f"{type_[:2]}标题为“{title}”，{type_}数据如下，立刻开始总结：“{transcript}”"
         )
     )
 
 
 def count_tokens(prompts: List[Dict[str, str]]):
     """根据内容计算 token 数"""
 
@@ -52,17 +52,17 @@
             num_tokens += len(tiktoken_enc.encode(value))
             if key == "name":
                 num_tokens += tokens_per_name
     num_tokens += 3
     return num_tokens
 
 
-def get_small_size_transcripts(text_data: List[str], token_limit: int = plugin_config.bilichat_openai_token_limit):
+def get_small_size_transcripts(title:str,text_data: List[str], token_limit: int = plugin_config.bilichat_openai_token_limit):
     unique_texts = list(OrderedDict.fromkeys(text_data))
-    while count_tokens(get_summarise_prompt("", " ".join(unique_texts))) > token_limit:
+    while count_tokens(get_summarise_prompt(title, " ".join(unique_texts))) > token_limit:
         unique_texts.pop(random.randint(0, len(unique_texts) - 1))
     return " ".join(unique_texts)
 
 
 def get_full_prompt(prompt: Optional[str] = None, system: Optional[str] = None, language: Optional[str] = None):
     plist: List[Dict[str, str]] = []
     if system:
```

### Comparing `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,35 +8,34 @@
 from ..model.exception import AbortError
 from ..optional import capture_exception  # type: ignore
 from .openai import get_small_size_transcripts, get_summarise_prompt, openai_req
 from .text_to_image import rich_text2image
 
 
 async def subtitle_summarise(title: str, sub: List[str]):
-    small_size_transcripts = get_small_size_transcripts(sub)
+    small_size_transcripts = get_small_size_transcripts(title, sub)
     prompt = get_summarise_prompt(title, small_size_transcripts)
     logger.debug(prompt)
     return await openai_req(prompt)
 
 
-async def column_summarise(cv_title: str, cv_text: str):
-    sentences = re.split(r"[，。；,.;\n]+", cv_text)
-    small_size_transcripts = get_small_size_transcripts(sentences)
-    prompt = get_summarise_prompt(cv_title, small_size_transcripts)
+async def column_summarise(cv_title: str, cv_text: List[str]):
+    small_size_transcripts = get_small_size_transcripts(cv_title, cv_text)
+    prompt = get_summarise_prompt(cv_title, small_size_transcripts, type_="专栏文章")
     logger.debug(prompt)
     return await openai_req(prompt)
 
 
 async def openai_summarization(cache: Cache, cid: str = "0"):
     try:
         if not cache.episodes[cid].openai:
             if cache.id[:2].lower() in ["bv", "av"]:
                 ai_summary = await subtitle_summarise(cache.title, cache.episodes[cid].content)
             elif cache.id[:2].lower() == "cv":
-                ai_summary = await column_summarise(cache.title, cache.episodes[cid].content[0])
+                ai_summary = await column_summarise(cache.title, cache.episodes[cid].content)
             else:
                 raise ValueError(f"Illegal Video(Column) types {cache.id}")
 
             if ai_summary.response:
                 cache.episodes[cid].openai = ai_summary.response
                 cache.save()
             else:
```

### Comparing `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/utils.py` & `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.7.1/pyproject.toml` & `nonebot_plugin_bilichat-1.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "1.7.1"
+version = "1.8.0"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "httpx>=0.23.3",
```

### Comparing `nonebot_plugin_bilichat-1.7.1/PKG-INFO` & `nonebot_plugin_bilichat-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 1.7.1
+Version: 1.8.0
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: httpx>=0.23.3
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
@@ -267,11 +267,12 @@
 在此感谢以下开发者(项目)对本项目做出的贡献：
 
 - [BibiGPT](https://github.com/JimmyLv/BibiGPT) 项目灵感来源
 - [bilibili-API-collect](https://github.com/SocialSisterYi/bilibili-API-collect) 易姐收集的各种 BiliBili Api 及其提供的 gRPC Api 调用方案
 - [BBot-Graia](https://github.com/djkcyl/BBot-Graia) 功能来源 ~~(我 牛 我 自 己)~~
 - [ABot-Graia](https://github.com/djkcyl/ABot-Graia) 永远怀念最好的 ABot 🙏
 - [nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template): 项目的 README 模板
+- [nonebot-plugin-bing-chat](https://github.com/Harry-Jing/nonebot-plugin-bing-chat): newbing解析的代码参考
 
 ## ⏳ Star 趋势
 
 [![Stargazers over time](https://starchart.cc/djkcyl/nonebot-plugin-bilichat.svg)](https://starchart.cc/djkcyl/nonebot-plugin-bilichat)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 1.7.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 1.8.0 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 httpx>=0.23.3 Requires-Dist: bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-
 plugin-localstore>=0.4.1 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-
 Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra" Requires-Dist:
@@ -129,10 +129,11 @@
 (é¡¹ç®)å¯¹æ¬é¡¹ç®ååºçè´¡ç®ï¼ - [BibiGPT](https://github.com/JimmyLv/
 BibiGPT) é¡¹ç®çµææ¥æº - [bilibili-API-collect](https://github.com/
 SocialSisterYi/bilibili-API-collect) æå§æ¶éçåç§ BiliBili Api
 åå¶æä¾ç gRPC Api è°ç¨æ¹æ¡ - [BBot-Graia](https://github.com/djkcyl/
 BBot-Graia) åè½æ¥æº ~~(æ ç æ èª å·±)~~ - [ABot-Graia](https://
 github.com/djkcyl/ABot-Graia) æ°¸è¿æå¿µæå¥½ç ABot ð - [nonebot-
 plugin-template](https://github.com/A-kirami/nonebot-plugin-template):
-é¡¹ç®ç README æ¨¡æ¿ ## â³ Star è¶å¿ [![Stargazers over time](https://
-starchart.cc/djkcyl/nonebot-plugin-bilichat.svg)](https://starchart.cc/djkcyl/
-nonebot-plugin-bilichat)
+é¡¹ç®ç README æ¨¡æ¿ - [nonebot-plugin-bing-chat](https://github.com/Harry-
+Jing/nonebot-plugin-bing-chat): newbingè§£æçä»£ç åè ## â³ Star è¶å¿
+[![Stargazers over time](https://starchart.cc/djkcyl/nonebot-plugin-
+bilichat.svg)](https://starchart.cc/djkcyl/nonebot-plugin-bilichat)
```

