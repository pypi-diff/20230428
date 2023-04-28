# Comparing `tmp/html2notion-0.1.5.tar.gz` & `tmp/html2notion-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html2notion-0.1.5.tar", last modified: Thu Apr 27 02:04:10 2023, max compression
+gzip compressed data, was "html2notion-0.1.6.tar", last modified: Fri Apr 28 05:45:28 2023, max compression
```

## Comparing `html2notion-0.1.5.tar` & `html2notion-0.1.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-27 02:04:10.991210 html2notion-0.1.5/
--rw-r--r--   0 daemonzhao   (501) staff       (20)     1064 2023-03-22 08:52:55.000000 html2notion-0.1.5/LICENSE
--rw-r--r--   0 daemonzhao   (501) staff       (20)     4600 2023-04-27 02:04:10.991558 html2notion-0.1.5/PKG-INFO
--rw-r--r--   0 daemonzhao   (501) staff       (20)     4111 2023-04-23 03:24:11.000000 html2notion-0.1.5/README.md
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-27 02:04:10.965782 html2notion-0.1.5/html2notion/
--rw-r--r--   0 daemonzhao   (501) staff       (20)        0 2023-03-20 01:38:35.000000 html2notion-0.1.5/html2notion/__init__.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     3955 2023-04-23 03:47:45.000000 html2notion-0.1.5/html2notion/main.py
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-27 02:04:10.982001 html2notion-0.1.5/html2notion/translate/
--rw-r--r--   0 daemonzhao   (501) staff       (20)        0 2023-03-20 01:38:35.000000 html2notion-0.1.5/html2notion/translate/__init__.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     4176 2023-04-23 03:24:11.000000 html2notion-0.1.5/html2notion/translate/batch_import.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2724 2023-04-19 01:44:49.000000 html2notion-0.1.5/html2notion/translate/cos_uploader.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     3662 2023-04-24 06:00:38.000000 html2notion-0.1.5/html2notion/translate/html2json.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)    10927 2023-04-27 01:54:11.000000 html2notion-0.1.5/html2notion/translate/html2json_base.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     1452 2023-04-24 05:58:55.000000 html2notion-0.1.5/html2notion/translate/html2json_clipper.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)      430 2023-04-20 02:17:23.000000 html2notion-0.1.5/html2notion/translate/html2json_default.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)    12779 2023-04-27 01:55:39.000000 html2notion-0.1.5/html2notion/translate/html2json_yinxiang.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     7168 2023-04-23 11:21:17.000000 html2notion-0.1.5/html2notion/translate/notion_export.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2389 2023-04-27 01:51:59.000000 html2notion-0.1.5/html2notion/translate/notion_import.py
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-27 02:04:10.986174 html2notion-0.1.5/html2notion/utils/
--rw-r--r--   0 daemonzhao   (501) staff       (20)      427 2023-03-24 02:23:25.000000 html2notion-0.1.5/html2notion/utils/__init__.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)      828 2023-03-22 03:05:54.000000 html2notion-0.1.5/html2notion/utils/load_config.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     1579 2023-04-20 06:50:27.000000 html2notion-0.1.5/html2notion/utils/log.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)      437 2023-04-21 02:46:15.000000 html2notion-0.1.5/html2notion/utils/timeutil.py
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-27 02:04:10.969416 html2notion-0.1.5/html2notion.egg-info/
--rw-r--r--   0 daemonzhao   (501) staff       (20)     4600 2023-04-27 02:04:10.000000 html2notion-0.1.5/html2notion.egg-info/PKG-INFO
--rw-r--r--   0 daemonzhao   (501) staff       (20)      918 2023-04-27 02:04:10.000000 html2notion-0.1.5/html2notion.egg-info/SOURCES.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)        1 2023-04-27 02:04:10.000000 html2notion-0.1.5/html2notion.egg-info/dependency_links.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)       54 2023-04-27 02:04:10.000000 html2notion-0.1.5/html2notion.egg-info/entry_points.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)      170 2023-04-27 02:04:10.000000 html2notion-0.1.5/html2notion.egg-info/requires.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)       12 2023-04-27 02:04:10.000000 html2notion-0.1.5/html2notion.egg-info/top_level.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)      103 2023-03-20 01:38:35.000000 html2notion-0.1.5/pyproject.toml
--rw-r--r--   0 daemonzhao   (501) staff       (20)      852 2023-04-27 02:04:10.992579 html2notion-0.1.5/setup.cfg
--rw-r--r--   0 daemonzhao   (501) staff       (20)       38 2023-03-17 05:39:04.000000 html2notion-0.1.5/setup.py
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-27 02:04:10.990591 html2notion-0.1.5/tests/
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2892 2023-04-20 03:22:55.000000 html2notion-0.1.5/tests/test_batchimport.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     3038 2023-04-20 03:22:52.000000 html2notion-0.1.5/tests/test_cosupload.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2698 2023-04-13 05:01:24.000000 html2notion-0.1.5/tests/test_notionexport.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)    31656 2023-04-27 02:03:06.000000 html2notion-0.1.5/tests/test_yinxiang.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-28 05:45:28.029199 html2notion-0.1.6/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     1064 2023-03-22 08:52:55.000000 html2notion-0.1.6/LICENSE
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     4600 2023-04-28 05:45:28.029345 html2notion-0.1.6/PKG-INFO
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     4111 2023-04-23 03:24:11.000000 html2notion-0.1.6/README.md
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-28 05:45:28.012364 html2notion-0.1.6/html2notion/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)        0 2023-03-20 01:38:35.000000 html2notion-0.1.6/html2notion/__init__.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     3955 2023-04-23 03:47:45.000000 html2notion-0.1.6/html2notion/main.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-28 05:45:28.022434 html2notion-0.1.6/html2notion/translate/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)        0 2023-03-20 01:38:35.000000 html2notion-0.1.6/html2notion/translate/__init__.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     4176 2023-04-23 03:24:11.000000 html2notion-0.1.6/html2notion/translate/batch_import.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     2724 2023-04-19 01:44:49.000000 html2notion-0.1.6/html2notion/translate/cos_uploader.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     3816 2023-04-28 05:32:21.000000 html2notion-0.1.6/html2notion/translate/html2json.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)    14207 2023-04-28 05:42:06.000000 html2notion-0.1.6/html2notion/translate/html2json_base.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     4119 2023-04-28 05:42:00.000000 html2notion-0.1.6/html2notion/translate/html2json_clipper.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      430 2023-04-20 02:17:23.000000 html2notion-0.1.6/html2notion/translate/html2json_default.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     8744 2023-04-28 03:13:54.000000 html2notion-0.1.6/html2notion/translate/html2json_yinxiang.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     7168 2023-04-23 11:21:17.000000 html2notion-0.1.6/html2notion/translate/notion_export.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     2867 2023-04-28 05:18:16.000000 html2notion-0.1.6/html2notion/translate/notion_import.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-28 05:45:28.025379 html2notion-0.1.6/html2notion/utils/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      427 2023-03-24 02:23:25.000000 html2notion-0.1.6/html2notion/utils/__init__.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      828 2023-03-22 03:05:54.000000 html2notion-0.1.6/html2notion/utils/load_config.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     1579 2023-04-20 06:50:27.000000 html2notion-0.1.6/html2notion/utils/log.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      437 2023-04-21 02:46:15.000000 html2notion-0.1.6/html2notion/utils/timeutil.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-28 05:45:28.015441 html2notion-0.1.6/html2notion.egg-info/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     4600 2023-04-28 05:45:27.000000 html2notion-0.1.6/html2notion.egg-info/PKG-INFO
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      918 2023-04-28 05:45:27.000000 html2notion-0.1.6/html2notion.egg-info/SOURCES.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)        1 2023-04-28 05:45:27.000000 html2notion-0.1.6/html2notion.egg-info/dependency_links.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)       54 2023-04-28 05:45:27.000000 html2notion-0.1.6/html2notion.egg-info/entry_points.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      170 2023-04-28 05:45:27.000000 html2notion-0.1.6/html2notion.egg-info/requires.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)       12 2023-04-28 05:45:27.000000 html2notion-0.1.6/html2notion.egg-info/top_level.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      103 2023-03-20 01:38:35.000000 html2notion-0.1.6/pyproject.toml
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      852 2023-04-28 05:45:28.029919 html2notion-0.1.6/setup.cfg
+-rw-r--r--   0 daemonzhao   (501) staff       (20)       38 2023-03-17 05:39:04.000000 html2notion-0.1.6/setup.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-28 05:45:28.028320 html2notion-0.1.6/tests/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     2892 2023-04-20 03:22:55.000000 html2notion-0.1.6/tests/test_batchimport.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     3038 2023-04-20 03:22:52.000000 html2notion-0.1.6/tests/test_cosupload.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     2698 2023-04-13 05:01:24.000000 html2notion-0.1.6/tests/test_notionexport.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)    31656 2023-04-27 02:03:06.000000 html2notion-0.1.6/tests/test_yinxiang.py
```

### Comparing `html2notion-0.1.5/LICENSE` & `html2notion-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.5/PKG-INFO` & `html2notion-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2notion
-Version: 0.1.5
+Version: 0.1.6
 Summary: This tool can accurately convert HTML to Notion notes and is also useful for exporting Evernote notes to Notion.
 Home-page: https://github.com/selfboot/html2notion
 Author: selfboot
 Author-email: xuezaigds@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `html2notion-0.1.5/README.md` & `html2notion-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.5/html2notion/main.py` & `html2notion-0.1.6/html2notion/main.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.5/html2notion/translate/batch_import.py` & `html2notion-0.1.6/html2notion/translate/batch_import.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.5/html2notion/translate/cos_uploader.py` & `html2notion-0.1.6/html2notion/translate/cos_uploader.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.5/html2notion/translate/html2json.py` & `html2notion-0.1.6/html2notion/translate/html2json.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,36 +19,39 @@
     meta_source = html_soup.select_one('html > head > meta[name="source"]')
     exporter_version_content = exporter_version_meta.get( 'content', "") if isinstance(exporter_version_meta, Tag) else ""
 
     meta_source_content = meta_source.get('content', "") if isinstance(meta_source, Tag) else ""
     if isinstance(exporter_version_content, str) and not exporter_version_content.startswith("Evernote"):
         return False
 
-    yinxiang_source_content = ["yinxiang", "desktop", "web"]
+    yinxiang_source_content = ["yinxiang", "desktop"]
     for prefix in yinxiang_source_content:
         if isinstance(meta_source_content, str) and meta_source_content.startswith(prefix):
             return True
     return False
 
 
 """
 <meta name="source-application" content="webclipper.evernote" />
+<meta name="source-application" content="微信" />
 """
 def _is_yinxiang_clipper_html(html_soup):
     exporter_version_meta = html_soup.select_one('html > head > meta[name="exporter-version"]')
     exporter_version_content = exporter_version_meta.get(
         'content', "") if isinstance(
         exporter_version_meta, Tag) else ""
 
     if isinstance(exporter_version_content, str) and not exporter_version_content.startswith("Evernote"):
         return False
     clipper_source_meta = html_soup.select_one('html > head > meta[name="source-application"]')
     clipper_source_content = clipper_source_meta.get('content', "") if isinstance(clipper_source_meta, Tag) else ""
     if isinstance(clipper_source_content, str) and clipper_source_content.endswith("evernote"):
         return True
+    if isinstance(clipper_source_content, str) and clipper_source_content in ("微信"):
+        return True
     return False
 
 
 def _infer_input_type(html_content):
     soup = BeautifulSoup(html_content, 'html.parser')
     if _is_yinxiang_export_html(soup):
         return YinXiang_Type
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `html2notion-0.1.5/html2notion/translate/html2json_base.py` & `html2notion-0.1.6/html2notion/translate/html2json_base.py`

 * *Files 17% similar despite different names*

```diff
@@ -67,15 +67,16 @@
             }.items()
             if value
         }
 
     @staticmethod
     def extract_text_and_parents(tag: PageElement, parents=[]):
         results = []
-        if isinstance(tag, NavigableString):
+        # Filter empty content
+        if isinstance(tag, NavigableString) and tag.text:
             results.append((tag.text, parents))
             return results
         elif isinstance(tag, Tag):
             for child in tag.children:
                 if isinstance(child, NavigableString):
                     if child.strip():
                         text = child.text
@@ -290,23 +291,120 @@
     @staticmethod
     def get_color(styles: dict, attrs):
         color = styles.get('color', "")
         if not color and 'color' in attrs:
             color = attrs['color']
         if not color:
             return "default"
+        # If the color_values have 4 items, then it is RGBA and the last value is alpha
+        # rgba(174, 174, 188, 0.2)
         if color.startswith("rgb"):
-            r, g, b = [int(x.strip()) for x in color[4:-1].split(",")]
+            color_values = [int(x.strip()) for x in re.findall(r'\d+', color)]
+            if len(color_values) >= 3:
+                r, g, b = color_values[:3]
+                return Html2JsonBase._closest_color(r, g, b)
         # Check if color is in hexadecimal format
         elif re.match(r'^#(?:[0-9a-fA-F]{3}){1,2}$', color):
             r, g, b = Html2JsonBase._hex_to_rgb(color)
-        else:
-            return "default"
+            return Html2JsonBase._closest_color(r, g, b)
+
+        return "default"
+
+    def convert_paragraph(self, soup):
+        json_obj = {
+            "object": "block",
+            "type": "paragraph",
+            "paragraph": {
+                "rich_text": []
+            }
+        }
+        rich_text = json_obj["paragraph"]["rich_text"]
+        text_obj = self.generate_inline_obj(soup)
+        if text_obj:
+            rich_text.extend(text_obj)
+        return json_obj
+
+    def convert_divider(self, soup):
+        return {
+            "object": "block",
+            "type": "divider",
+            "divider": {}
+        }
+
+    def convert_heading(self, soup):
+        heading_map = {"h1": "heading_1", "h2": "heading_2", "h3": "heading_3",
+                       "h4": "heading_3", "h5": "heading_3", "h6": "heading_3"}
+
+        heading_level = heading_map.get(soup.name, "heading_3")
+        json_obj = {
+            "object": "block",
+            "type": heading_level,
+            heading_level: {
+                "rich_text": []
+            }
+        }
+        rich_text = json_obj[heading_level]["rich_text"]
+        text_obj = self.generate_inline_obj(soup)
+        if text_obj:
+            rich_text.extend(text_obj)
+            return json_obj
+        return None
+
+    # <ol><li><div>first</div></li><li><div>second</div></li><li><div>third</div></li></ol>
+    def convert_numbered_list_item(self, soup):
+        return self.convert_list_items(soup, 'numbered_list_item')
+
+    # <ul><li><div>itemA</div></li><li><div>itemB</div></li><li><div>itemC</div></li></ul>
+    def convert_bulleted_list_item(self, soup):
+        return self.convert_list_items(soup, 'bulleted_list_item')
+
+    def convert_list_items(self, soup, list_type):
+        # Remove heading tags in li
+        for heading in soup.find_all(['h1', 'h2', 'h3', 'h4', 'h5', 'h6']):
+            heading.unwrap()
+
+        items = soup.find_all('li', recursive=True)
+        if not items:
+            logger.warning("No list items found in {soup}")
+
+        json_arr = []
+        for item in items:
+            one_item = self._convert_one_list_item(item, list_type)
+            if one_item:
+                json_arr.append(one_item)
+            else:
+                logger.info(f'empty {item}')
+        return json_arr
 
-        return Html2JsonBase._closest_color(r, g, b)
+    def _convert_one_list_item(self, soup, list_type):
+        if list_type not in {'numbered_list_item', 'bulleted_list_item'}:
+            logger.warning(f'Not support list_type')
+
+        json_obj = {
+            "object": "block",
+            list_type: {
+                "rich_text": []
+            },
+            "type": list_type,
+        }
+        rich_text = json_obj[list_type]["rich_text"]
+        text_obj = Html2JsonBase.generate_inline_obj(soup)
+        if text_obj:
+            rich_text.extend(text_obj)
+
+        return json_obj
+
+    # def convert_fail(self, soup):
+    #     return {
+    #         "object": "block",
+    #         "type": "paragraph",
+    #         "paragraph": {
+    #             "rich_text": []
+    #         }
+    #     }
 
     @classmethod
     def register(cls, input_type, subclass):
         cls._registry[input_type] = subclass
 
     @classmethod
     def create(cls, input_type, html_content):
```

### Comparing `html2notion-0.1.5/html2notion/translate/html2json_yinxiang.py` & `html2notion-0.1.6/html2notion/translate/html2json_yinxiang.py`

 * *Files 23% similar despite different names*

```diff
@@ -51,53 +51,14 @@
             converter = getattr(self, f"convert_{block_type}")
             if converter:
                 block = converter(child)
                 if block:
                     self.children.extend([block] if not isinstance(block, list) else block)
             else:
                 logger.warning(f"Unknown block type: {block_type}")
-
-    def convert_paragraph(self, soup):
-        json_obj = {
-            "object": "block",
-            "type": "paragraph",
-            "paragraph": {
-                "rich_text": []
-            }
-        }
-        rich_text = json_obj["paragraph"]["rich_text"]
-        text_obj = self.generate_inline_obj(soup)
-        if text_obj:
-            rich_text.extend(text_obj)
-        return json_obj
-
-    def convert_divider(self, soup):
-        return {
-            "object": "block",
-            "type": "divider",
-            "divider": {}
-        }
-    
-    def convert_heading(self, soup):
-        heading_map = {"h1": "heading_1", "h2": "heading_2", "h3": "heading_3",
-                       "h4": "heading_3", "h5": "heading_3", "h6": "heading_3"}
-
-        heading_level = heading_map.get(soup.name, "heading_3")
-        json_obj = {
-            "object": "block",
-            "type": heading_level,
-            heading_level: {
-                "rich_text": []
-            }
-        }
-        rich_text = json_obj[heading_level]["rich_text"]
-        text_obj = self.generate_inline_obj(soup)
-        if text_obj:
-            rich_text.extend(text_obj)
-        return json_obj
     
     def convert_code(self, soup):
         json_obj = {
             "object": "block",
             "type": "code",
             "code": {
                 "rich_text": [],
@@ -121,23 +82,14 @@
         if isinstance(style, str):
             style = ''.join(style.split())
             css_dict = {rule.split(':')[0].strip(): rule.split(':')[1].strip() for rule in style.split(';') if rule}
             language = css_dict.get('--en-codeblockLanguage', 'plain text')
             json_obj["code"]["language"] = language
         
         return json_obj
-    
-    def convert_fail(self, soup):
-        return {
-            "object": "block",
-            "type": "paragraph",
-            "paragraph": {
-                "rich_text": []
-            }
-        }
 
     def convert_quote(self, soup):
         json_obj = {
             "object": "block",
             "type": "quote",
             "quote": {
                 "rich_text": []
@@ -223,86 +175,15 @@
             if text_obj:
                 text.extend(text_obj)
             input_tag = child.find('input')
             if input_tag and isinstance(input_tag, Tag) and input_tag.get('checked', 'false') == 'true':
                 json_obj["to_do"]["checked"] = True
             to_do_blocks.append(json_obj)
         return to_do_blocks
-
-    # <ol><li><div>first</div></li><li><div>second</div></li><li><div>third</div></li></ol>
-    def convert_numbered_list_item(self, soup):
-        return self.convert_list_items(soup, 'numbered_list_item')
-
-    # <ul><li><div>itemA</div></li><li><div>itemB</div></li><li><div>itemC</div></li></ul>
-    def convert_bulleted_list_item(self, soup):
-        return self.convert_list_items(soup, 'bulleted_list_item')
-
-    def convert_list_items(self, soup, list_type):
-        items = soup.find_all('li', recursive=True)
-        if not items:
-            logger.warning("No list items found in {soup}")
-
-        json_arr = []
-        for item in items:
-            one_item = self._convert_one_list_item(item, list_type)
-            if one_item:
-                json_arr.append(one_item)
-            else:
-                logger.info(f'empty {item}')
-        return json_arr
-
-    def _convert_one_list_item(self, soup, list_type):
-        if list_type not in {'numbered_list_item', 'bulleted_list_item'}:
-            logger.warning(f'Not support list_type')
-
-        json_obj = {
-            "object": "block",
-            list_type: {
-                "rich_text": []
-            },
-            "type": list_type,
-        }
-        rich_text = json_obj[list_type]["rich_text"]
-        text_obj = Html2JsonBase.generate_inline_obj(soup)
-        if text_obj:
-            rich_text.extend(text_obj)
-
-        return json_obj
-
-    def _recursive_parse_style(self, tag_soup, tag_text, text_params):
-        tag_name = tag_soup.name.lower() if tag_soup.name else ""
-        style = tag_soup.get('style') if tag_name else ""
-        styles = {}
-        if style:
-            styles = {rule.split(':')[0].strip(): rule.split(
-                ':')[1].strip() for rule in style.split(';') if rule}
-
-        text_params["plain_text"] = tag_text
-        if Html2JsonBase.is_bold(tag_name, styles):
-            text_params["bold"] = True
-        if Html2JsonBase.is_italic(tag_name, styles):
-            text_params["italic"] = True
-        if Html2JsonBase.is_strikethrough(tag_name, styles):
-            text_params["strikethrough"] = True
-        if Html2JsonBase.is_underline(tag_name, styles):
-            text_params["underline"] = True
-
-        color = Html2JsonBase.get_color(
-            styles, tag_soup.attrs if tag_name else {})
-        if color != 'default':
-            text_params["color"] = color
-
-        if not tag_soup or isinstance(tag_soup, NavigableString):
-            return
-
-        for child in tag_soup.children:
-            if isinstance(child, Tag):
-                self._recursive_parse_style(child, child.text, text_params)
-        return
-
+  
     def get_block_type(self, single_tag):
         tag_name = single_tag.name
         style = single_tag.get('style') if tag_name else ""
 
         # There are priorities here. It is possible to hit multiple targets 
         # at the same time, and the first one takes precedence.
         if self._check_is_todo(single_tag):
```

### Comparing `html2notion-0.1.5/html2notion/translate/notion_export.py` & `html2notion-0.1.6/html2notion/translate/notion_export.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.5/html2notion/translate/notion_import.py` & `html2notion-0.1.6/html2notion/translate/notion_import.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,30 +36,38 @@
 
     # Doc of create page: https://developers.notion.com/reference/post-page
     @retry(stop=stop_after_attempt(5),
            wait=wait_exponential(multiplier=1, min=3, max=30),
            retry=retry_if_exception_type(RequestTimeoutError))
     async def create_new_page(self, notion_data):
         # logger.debug(f'Create new page: {notion_data["parent"]}, {notion_data["properties"]}')
-        created_page = await self.notion_client.pages.create(
-            **notion_data
-        )
+        # body.children.length should be ≤ `100`,
+        blocks = notion_data.get("children", [])
+        limit_size = 100
+        chunks = [blocks[i: i + limit_size] for i in range(0, len(blocks), limit_size)]
+        if blocks:
+            notion_data.pop("children")
+        first_chunk = chunks[0] if chunks else []
+        created_page = await self.notion_client.pages.create(**notion_data, children=first_chunk)
+        page_id = created_page["id"]
+        for chunk in chunks[1:]:
+            await self.notion_client.blocks.children.append(page_id, children=chunk)
         return created_page
 
 
 async def main(file_path, notion_api_key):
     async with ClientSession() as session:
         async with AsyncClient(auth=notion_api_key) as notion_client:
             importer = NotionImporter(session, notion_client)
             result = await importer.process_file(file_path)
             logger.info(f"Import result: {result}")
 
 
 if __name__ == "__main__":
     test_prepare_conf()
-    file = Path("./demos/Test Case C.html")
+    file = Path("./demos/Test Case E.html")
     notion_api_key = ""
     if 'GITHUB_ACTIONS' in os.environ:
         notion_api_key = os.environ['notion_api_key']
     else:
         notion_api_key = config['notion']['api_key']
     asyncio.run(main(file, notion_api_key))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `html2notion-0.1.5/html2notion/utils/load_config.py` & `html2notion-0.1.6/html2notion/utils/load_config.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.5/html2notion/utils/log.py` & `html2notion-0.1.6/html2notion/utils/log.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.5/html2notion.egg-info/PKG-INFO` & `html2notion-0.1.6/html2notion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2notion
-Version: 0.1.5
+Version: 0.1.6
 Summary: This tool can accurately convert HTML to Notion notes and is also useful for exporting Evernote notes to Notion.
 Home-page: https://github.com/selfboot/html2notion
 Author: selfboot
 Author-email: xuezaigds@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `html2notion-0.1.5/html2notion.egg-info/SOURCES.txt` & `html2notion-0.1.6/html2notion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.5/setup.cfg` & `html2notion-0.1.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = html2notion
-version = 0.1.5
+version = 0.1.6
 author = selfboot
 author_email = xuezaigds@gmail.com
 description = This tool can accurately convert HTML to Notion notes and is also useful for exporting Evernote notes to Notion.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/selfboot/html2notion
 license_files = LICENSE
```

### Comparing `html2notion-0.1.5/tests/test_batchimport.py` & `html2notion-0.1.6/tests/test_batchimport.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.5/tests/test_cosupload.py` & `html2notion-0.1.6/tests/test_cosupload.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.5/tests/test_notionexport.py` & `html2notion-0.1.6/tests/test_notionexport.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.5/tests/test_yinxiang.py` & `html2notion-0.1.6/tests/test_yinxiang.py`

 * *Files identical despite different names*

