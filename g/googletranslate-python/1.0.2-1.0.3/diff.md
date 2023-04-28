# Comparing `tmp/googletranslate-python-1.0.2.tar.gz` & `tmp/googletranslate-python-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/googletranslate-python-1.0.2.tar", last modified: Mon Feb  6 08:37:13 2023, max compression
+gzip compressed data, was "googletranslate-python-1.0.3.tar", last modified: Fri Apr 28 08:40:58 2023, max compression
```

## Comparing `googletranslate-python-1.0.2.tar` & `googletranslate-python-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-02-06 08:37:13.131390 googletranslate-python-1.0.2/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       64 2023-02-06 07:47:41.000000 googletranslate-python-1.0.2/MANIFEST.in
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     2247 2023-02-06 08:37:13.119728 googletranslate-python-1.0.2/PKG-INFO
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1100 2023-02-06 08:36:52.000000 googletranslate-python-1.0.2/README.md
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-02-06 08:37:12.850396 googletranslate-python-1.0.2/googletranslate_python.egg-info/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     2247 2023-02-06 08:37:12.000000 googletranslate-python-1.0.2/googletranslate_python.egg-info/PKG-INFO
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      469 2023-02-06 08:37:12.000000 googletranslate-python-1.0.2/googletranslate_python.egg-info/SOURCES.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)        1 2023-02-06 08:37:12.000000 googletranslate-python-1.0.2/googletranslate_python.egg-info/dependency_links.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      100 2023-02-06 08:37:12.000000 googletranslate-python-1.0.2/googletranslate_python.egg-info/entry_points.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       27 2023-02-06 08:37:12.000000 googletranslate-python-1.0.2/googletranslate_python.egg-info/requires.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       18 2023-02-06 08:37:12.000000 googletranslate-python-1.0.2/googletranslate_python.egg-info/top_level.txt
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-02-06 08:37:13.068373 googletranslate-python-1.0.2/googletranslatepy/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      234 2023-02-03 09:02:06.000000 googletranslate-python-1.0.2/googletranslatepy/__init__.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     2734 2023-02-06 08:33:29.000000 googletranslate-python-1.0.2/googletranslatepy/bin.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1540 2023-02-03 09:32:55.000000 googletranslate-python-1.0.2/googletranslatepy/translator.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      325 2023-02-03 09:29:02.000000 googletranslate-python-1.0.2/googletranslatepy/util.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      273 2023-02-06 07:47:52.000000 googletranslate-python-1.0.2/googletranslatepy/version.json
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       30 2023-02-02 09:11:26.000000 googletranslate-python-1.0.2/requirements.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       38 2023-02-06 08:37:13.143676 googletranslate-python-1.0.2/setup.cfg
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1378 2023-02-03 09:09:51.000000 googletranslate-python-1.0.2/setup.py
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-04-28 08:40:58.102366 googletranslate-python-1.0.3/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       64 2023-02-06 07:47:41.000000 googletranslate-python-1.0.3/MANIFEST.in
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     2247 2023-04-28 08:40:58.095344 googletranslate-python-1.0.3/PKG-INFO
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     1100 2023-02-06 08:36:52.000000 googletranslate-python-1.0.3/README.md
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-04-28 08:40:57.973407 googletranslate-python-1.0.3/googletranslate_python.egg-info/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     2247 2023-04-28 08:40:57.000000 googletranslate-python-1.0.3/googletranslate_python.egg-info/PKG-INFO
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      469 2023-04-28 08:40:57.000000 googletranslate-python-1.0.3/googletranslate_python.egg-info/SOURCES.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)        1 2023-04-28 08:40:57.000000 googletranslate-python-1.0.3/googletranslate_python.egg-info/dependency_links.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      100 2023-04-28 08:40:57.000000 googletranslate-python-1.0.3/googletranslate_python.egg-info/entry_points.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       27 2023-04-28 08:40:57.000000 googletranslate-python-1.0.3/googletranslate_python.egg-info/requires.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       18 2023-04-28 08:40:57.000000 googletranslate-python-1.0.3/googletranslate_python.egg-info/top_level.txt
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-04-28 08:40:58.072465 googletranslate-python-1.0.3/googletranslatepy/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      234 2023-02-03 09:02:06.000000 googletranslate-python-1.0.3/googletranslatepy/__init__.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     2734 2023-04-28 08:35:37.000000 googletranslate-python-1.0.3/googletranslatepy/bin.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     1560 2023-04-28 08:38:59.000000 googletranslate-python-1.0.3/googletranslatepy/translator.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      325 2023-02-03 09:29:02.000000 googletranslate-python-1.0.3/googletranslatepy/util.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      273 2023-04-28 08:35:18.000000 googletranslate-python-1.0.3/googletranslatepy/version.json
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       30 2023-02-02 09:11:26.000000 googletranslate-python-1.0.3/requirements.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       38 2023-04-28 08:40:58.113029 googletranslate-python-1.0.3/setup.cfg
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     1378 2023-02-03 09:09:51.000000 googletranslate-python-1.0.3/setup.py
```

### Comparing `googletranslate-python-1.0.2/PKG-INFO` & `googletranslate-python-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: googletranslate-python
-Version: 1.0.2
+Version: 1.0.3
 Summary: Google Translate Client with `deep-translator`
 Home-page: https://github.com/suqingdong/googletranslatepy
 Author: suqingdong
 Author-email: suqingdong1114@gmail.com
 License: MIT License
 Description: # Google Translate Client with `deep-translator`
```

### Comparing `googletranslate-python-1.0.2/README.md` & `googletranslate-python-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `googletranslate-python-1.0.2/googletranslate_python.egg-info/PKG-INFO` & `googletranslate-python-1.0.3/googletranslate_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: googletranslate-python
-Version: 1.0.2
+Version: 1.0.3
 Summary: Google Translate Client with `deep-translator`
 Home-page: https://github.com/suqingdong/googletranslatepy
 Author: suqingdong
 Author-email: suqingdong1114@gmail.com
 License: MIT License
 Description: # Google Translate Client with `deep-translator`
```

### Comparing `googletranslate-python-1.0.2/googletranslatepy/bin.py` & `googletranslate-python-1.0.3/googletranslatepy/bin.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 @click.argument('text', nargs=-1)
 @click.version_option(version=version_info['version'], prog_name=version_info['prog'])
 @click.option('-p', '--proxies', help='the proxies url, eg. http://127.0.0.1:1080', envvar='GOOGLE_PROXIES', show_envvar=True)
 @click.option('-s', '--source', help='the source language', default='auto', show_default=True)
 @click.option('-t', '--target', help='the target language', default='zh-CN', show_default=True)
 @click.option('-l', '--languages', help='list all available languages', is_flag=True)
 @click.option('-o', '--outfile', help='the output filename [stdout]')
-@click.option('-t', '--timeout', help='the timeout of requests', type=float, default=5, show_default=True)
+@click.option('-T', '--timeout', help='the timeout of requests', type=float, default=5, show_default=True)
 @click.pass_context
 def cli(ctx, **kwargs):
 
     if kwargs['languages']:
         rich.print_json(json.dumps(
             deep_translator.constants.GOOGLE_LANGUAGES_TO_CODES))
         exit(0)
```

### Comparing `googletranslate-python-1.0.2/googletranslatepy/translator.py` & `googletranslate-python-1.0.3/googletranslatepy/translator.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,28 +18,28 @@
         self.proxies = {'https': proxies} if isinstance(proxies, str) else proxies
         self.trans = deep_translator.GoogleTranslator(
             source=source,
             target=target,
             proxies=self.proxies,
         )
 
-    def translate(self, text):
+    def translate(self, text, **kwargs):
         """
             the length of characters is limited within 5000,
         """
         text_list = textwrap.wrap(
             text,
             width=4999,
             break_long_words=False,
             break_on_hyphens=False,
             drop_whitespace=False,
             replace_whitespace=False,
         )
         try:
-            res = ' '.join(self.trans.translate(t) for t in text_list)
+            res = ' '.join(self.trans.translate(t, **kwargs) for t in text_list)
             return res
         except Exception as e:
             print(e)
             return False
 
     def check_proxies(self, timeout=5):
         url = self.trans._base_url
```

### Comparing `googletranslate-python-1.0.2/setup.py` & `googletranslate-python-1.0.3/setup.py`

 * *Files identical despite different names*

