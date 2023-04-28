# Comparing `tmp/pypubmed-1.0.9.tar.gz` & `tmp/pypubmed-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pypubmed-1.0.9.tar", last modified: Mon Jan 25 04:34:36 2021, max compression
+gzip compressed data, was "pypubmed-1.1.0.tar", last modified: Fri Apr 28 02:41:26 2023, max compression
```

## Comparing `pypubmed-1.0.9.tar` & `pypubmed-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2021-01-25 04:34:36.000000 pypubmed-1.0.9/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       63 2020-12-08 08:44:31.000000 pypubmed-1.0.9/MANIFEST.in
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1706 2021-01-25 04:34:36.000000 pypubmed-1.0.9/PKG-INFO
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      592 2020-12-09 07:36:00.000000 pypubmed-1.0.9/README.md
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2021-01-25 04:34:35.000000 pypubmed-1.0.9/pypubmed/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      197 2020-12-10 07:10:17.000000 pypubmed-1.0.9/pypubmed/__init__.py
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2021-01-25 04:34:36.000000 pypubmed-1.0.9/pypubmed/bin/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)        0 2020-08-11 08:30:01.000000 pypubmed-1.0.9/pypubmed/bin/__init__.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1705 2020-12-11 02:19:16.000000 pypubmed-1.0.9/pypubmed/bin/_citations.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     4261 2020-12-11 05:10:36.000000 pypubmed-1.0.9/pypubmed/bin/_search.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1607 2020-12-11 05:10:29.000000 pypubmed-1.0.9/pypubmed/bin/cli.py
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2021-01-25 04:34:36.000000 pypubmed-1.0.9/pypubmed/core/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)        0 2020-09-11 05:55:10.000000 pypubmed-1.0.9/pypubmed/core/__init__.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      616 2020-09-15 08:44:09.000000 pypubmed-1.0.9/pypubmed/core/article.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     2917 2020-12-08 07:47:09.000000 pypubmed-1.0.9/pypubmed/core/citations.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)    10015 2020-12-11 05:05:40.000000 pypubmed-1.0.9/pypubmed/core/eutils.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     5843 2020-12-11 05:21:47.000000 pypubmed-1.0.9/pypubmed/core/export.py
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2021-01-25 04:34:36.000000 pypubmed-1.0.9/pypubmed/util/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      336 2020-12-09 03:34:07.000000 pypubmed-1.0.9/pypubmed/util/__init__.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     5189 2021-01-25 04:34:03.000000 pypubmed-1.0.9/pypubmed/util/xml_parser.py
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2021-01-25 04:34:36.000000 pypubmed-1.0.9/pypubmed/version/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      136 2021-01-25 04:34:16.000000 pypubmed-1.0.9/pypubmed/version/version.json
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2021-01-25 04:34:35.000000 pypubmed-1.0.9/pypubmed.egg-info/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1706 2021-01-25 04:34:35.000000 pypubmed-1.0.9/pypubmed.egg-info/PKG-INFO
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      568 2021-01-25 04:34:35.000000 pypubmed-1.0.9/pypubmed.egg-info/SOURCES.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)        1 2021-01-25 04:34:35.000000 pypubmed-1.0.9/pypubmed.egg-info/dependency_links.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       83 2021-01-25 04:34:35.000000 pypubmed-1.0.9/pypubmed.egg-info/entry_points.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      142 2021-01-25 04:34:35.000000 pypubmed-1.0.9/pypubmed.egg-info/requires.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)        9 2021-01-25 04:34:35.000000 pypubmed-1.0.9/pypubmed.egg-info/top_level.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      142 2021-01-25 04:30:57.000000 pypubmed-1.0.9/requirements.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       38 2021-01-25 04:34:36.000000 pypubmed-1.0.9/setup.cfg
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1540 2020-12-09 08:00:06.000000 pypubmed-1.0.9/setup.py
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-04-28 02:41:26.140064 pypubmed-1.1.0/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       63 2020-12-08 08:44:31.000000 pypubmed-1.1.0/MANIFEST.in
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     1894 2023-04-28 02:41:26.133464 pypubmed-1.1.0/PKG-INFO
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      733 2023-04-28 02:41:07.000000 pypubmed-1.1.0/README.md
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-04-28 02:41:25.771367 pypubmed-1.1.0/pypubmed/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      197 2020-12-10 07:10:17.000000 pypubmed-1.1.0/pypubmed/__init__.py
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-04-28 02:41:25.955008 pypubmed-1.1.0/pypubmed/bin/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)        0 2020-08-11 08:30:01.000000 pypubmed-1.1.0/pypubmed/bin/__init__.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     1705 2020-12-11 02:19:16.000000 pypubmed-1.1.0/pypubmed/bin/_citations.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     5348 2021-03-01 06:29:04.000000 pypubmed-1.1.0/pypubmed/bin/_search.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     1586 2023-04-28 02:21:02.000000 pypubmed-1.1.0/pypubmed/bin/cli.py
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-04-28 02:41:26.050610 pypubmed-1.1.0/pypubmed/core/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)        0 2020-09-11 05:55:10.000000 pypubmed-1.1.0/pypubmed/core/__init__.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      616 2020-09-15 08:44:09.000000 pypubmed-1.1.0/pypubmed/core/article.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     2917 2020-12-08 07:47:09.000000 pypubmed-1.1.0/pypubmed/core/citations.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)    10160 2023-04-28 02:27:59.000000 pypubmed-1.1.0/pypubmed/core/eutils.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     6381 2021-02-23 03:53:38.000000 pypubmed-1.1.0/pypubmed/core/export.py
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-04-28 02:41:26.090122 pypubmed-1.1.0/pypubmed/util/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      336 2020-12-09 03:34:07.000000 pypubmed-1.1.0/pypubmed/util/__init__.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     5631 2021-08-11 05:51:51.000000 pypubmed-1.1.0/pypubmed/util/xml_parser.py
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-04-28 02:41:26.111284 pypubmed-1.1.0/pypubmed/version/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      167 2023-04-28 02:28:48.000000 pypubmed-1.1.0/pypubmed/version/version.json
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-04-28 02:41:25.883358 pypubmed-1.1.0/pypubmed.egg-info/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     1894 2023-04-28 02:41:25.000000 pypubmed-1.1.0/pypubmed.egg-info/PKG-INFO
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      568 2023-04-28 02:41:25.000000 pypubmed-1.1.0/pypubmed.egg-info/SOURCES.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)        1 2023-04-28 02:41:25.000000 pypubmed-1.1.0/pypubmed.egg-info/dependency_links.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       83 2023-04-28 02:41:25.000000 pypubmed-1.1.0/pypubmed.egg-info/entry_points.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      118 2023-04-28 02:41:25.000000 pypubmed-1.1.0/pypubmed.egg-info/requires.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)        9 2023-04-28 02:41:25.000000 pypubmed-1.1.0/pypubmed.egg-info/top_level.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      118 2023-04-28 02:39:17.000000 pypubmed-1.1.0/requirements.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       38 2023-04-28 02:41:26.144073 pypubmed-1.1.0/setup.cfg
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     1540 2020-12-11 03:36:41.000000 pypubmed-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pypubmed-1.0.9/PKG-INFO` & `pypubmed-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: pypubmed
-Version: 1.0.9
+Version: 1.1.0
 Summary: Toolkits for NCBI Pubmed
 Home-page: https://github.com/suqingdong/pypubmed
 Author: suqingdong
-Author-email: 1078595229@qq.com
+Author-email: suqingdong1114@gmail.com
 License: BSD License
 Project-URL: Documentation, https://pypubmed.readthedocs.io
 Project-URL: Tracker, https://github.com/suqingdong/pypubmed/issues
 Description: # NCBI Pubmed Toolkits
         
         ## Requirements
         - Python3.6+
         
         ## Installation
         ```bash
-        pip3 isntall pypubmed
+        python3 -m pip install -U pypubmed
         ```
         
         ## Usage
         ### `search`
         > search Pubmed with term
         ```bash
         pypubmed search --help
+        
+        # do not translate
+        pypubmed search -l 5 ngs
+        
+        # translate with a local proxies
+        pypubmed -p http://127.0.0.1:1081 search ngs -l 5
         ```
         
         ### `advance-search`
         > advance search builder
         ```bash
         pypubmed advance-search --help
         ```
@@ -40,15 +46,14 @@
         
         ## Todos
         - [ ] HTML output
         - [ ] PDF downloader
         - [ ] GUI application
         - [ ] Local paper manager
         
-        
         ## Documents
         > https://pypubmed.readthedocs.io/en/latest/
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `pypubmed-1.0.9/pypubmed/bin/_citations.py` & `pypubmed-1.1.0/pypubmed/bin/_citations.py`

 * *Files identical despite different names*

### Comparing `pypubmed-1.0.9/pypubmed/bin/_search.py` & `pypubmed-1.1.0/pypubmed/bin/_search.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,103 +1,135 @@
 import os
 import re
 import click
 import datetime
+import pickle
 
 from dateutil.parser import parse as date_parse
 
+from pypubmed.util import safe_open
 from pypubmed.core.export import Export
 
 search_examples = click.style('''
 examples:
 
     pypubmed search ngs -l 5 -o ngs.xlsx
 
     pypubmed search 'NGS[Title] AND Disease[Title/Abstract]' -o ngs_disease.xlsx
 
     pypubmed search 1,2,3,4
 
     pypubmed search pmid_list.txt
 ''', fg='yellow')
 @click.command(help=click.style('search with pmid or a term', bold=True, fg='green'), epilog=search_examples, no_args_is_help=True)
-@click.option('-c', '--cited', help='get cited information', default=False, is_flag=True)
+@click.option('-cit', '--cited', help='get cited information', default=False, is_flag=True)
 @click.option('-n', '--no-translate', help='do not translate the abstract', default=False, is_flag=True)
 @click.option('-b', '--batch-size', help='the batch size for efetch', default=10, type=int, show_default=True)
 @click.option('-min', '--min-factor', help='filter with IF', type=float)
 @click.option('-l', '--limit', help='limit the count of output', type=int)
 @click.option('-f', '--fields', help='the fields to export')
 @click.option('-o', '--outfile', help='the output filename', default='pubmed.xlsx', show_default=True)
+@click.option('-a', '--author', help='export information of authors', is_flag=True, hidden=True)
+
+@click.option('-c', '--cache', help='store translated result to a cache file', is_flag=True)
+@click.option('-s', '--retstart', help='the number of start', type=int, default=0, show_default=True)
+
 @click.argument('term', nargs=1)
 @click.pass_obj
 def search(obj, **kwargs):
     
-    articles = obj['eutils'].search(translate=not kwargs['no_translate'], **kwargs)
-
     data = []
-    for n, article in enumerate(articles, 1):
-        obj['eutils'].logger.debug('{}. {}'.format(n, article))
-
-        # filter impact factor
-        if kwargs['min_factor'] and (article.impact_factor != '.' and article.impact_factor < kwargs['min_factor']):
-            continue
-
-        data.append(article.to_dict())
-        if kwargs['limit'] and n >= kwargs['limit']:
-            break
+    translate_cache = {}
+    cache_file = '.translate.cache.pkl'
+    if os.path.isfile(cache_file):
+        with safe_open(cache_file, 'rb') as f:
+            translate_cache = pickle.load(f)
+
+    articles = obj['eutils'].search(translate=not kwargs['no_translate'], translate_cache=translate_cache, **kwargs)
+
+    try:
+        for n, article in enumerate(articles, 1):
+            obj['eutils'].logger.debug(f'{n}. {article}')
+
+            # store translated result to cache file
+            if kwargs['cache']:
+                translate_cache[article.pmid] = article.abstract_cn
+
+            # filter impact factor
+            if kwargs['min_factor'] and (article.impact_factor != '.' and article.impact_factor < kwargs['min_factor']):
+                continue
+
+            # export author information or not
+            if not kwargs['author']:
+                del article.author_mail
+                del article.author_first
+                del article.author_last
+
+            data.append(article.to_dict())
+
+            if kwargs['limit'] and n >= kwargs['limit']:
+                break
+    except KeyboardInterrupt:
+        pass
 
     if kwargs['min_factor']:
         obj['eutils'].logger.info('A total of {} articles were found, {} remaining after filtering IF>={}'.format(n, len(data), kwargs['min_factor']))
 
+    if kwargs['cache']:
+        with safe_open(cache_file, 'wb') as out:
+            pickle.dump(translate_cache, out)
+        obj['eutils'].logger.debug(f'save cache file: {cache_file}')
+
     Export(data, **kwargs).export()
 
 
 @click.command(help=click.style('generate advance search string', bold=True, fg='cyan'))
 @click.pass_obj
 def advance_search(obj, **kwargs):
     fields = obj['eutils'].validate_fields()
 
     query_box = ''
     while True:
         number = click.prompt('>>> please choose a number of field', type=int, default=48)
         field = fields[number][1]
-        click.secho('your choice is: {number} - {field}'.format(**locals()), fg='cyan')
+        click.secho(f'your choice is: {number} - {field}', fg='cyan')
 
         if field.startswith('Date - '):
             start = click.prompt('>>> please enter the start date(YYYY-MM-DD)', value_proc=date_parse).strftime('%Y/%m/%d')
             end = click.prompt('>>> please enter the end date', default='3000', value_proc=date_parse)
             if end != '3000':
                 end = end.strftime('%Y/%m/%d')
-            term = '("{start}"[{field}] : "{end}"[{field}])'.format(**locals())
+            term = f'("{start}"[{field}] : "{end}"[{field}])'
         else:
             term = click.prompt('>>> please enter a search term')
             if field == 'All Fields':
-                term = '{term}'.format(**locals())
+                term = f'{term}'
             else:
-                term = '"{term}"[{field}]'.format(**locals())
+                term = f'"{term}"[{field}]'
 
         if not query_box:
             query_box = term
         else:
             logic = click.prompt('>>> please input the logic', type=click.Choice(['and', 'or', 'not']), default='and').upper()
-            query_box = '({query_box}) {logic} ({term})'.format(**locals())
+            query_box = f'({query_box}) {logic} ({term})'
 
         click.secho('query box now: ' + query_box, fg='bright_green')
 
         if click.confirm('input finish?'):
             break
 
-    click.secho('final query box: {}'.format(query_box), fg='bright_cyan')
+    click.secho(f'final query box: {query_box}', fg='bright_cyan')
     res = obj['eutils'].esearch(query_box, retmax=1, head=True)
 
     if res['count']:
         details = []
         for each in res['translationstack']:
             if isinstance(each, dict):
                 details += ['{term}:{count}'.format(**each)]
         click.secho('count:\t{count}\nquery:\t{querytranslation}\ndetail:\t{detail}'.format(detail=', '.join(details), **res), fg='yellow')
 
         if click.confirm('search with this query box?'):
             outfile = re.sub(r'[\'"\(\)\[\]/ ]+', '_', query_box).strip('_') + '.xlsx'
             outfile = click.prompt('output filename', default=outfile, show_default=True)
-            os.system('pypubmed search "{}" -o {}'.format(query_box, outfile))
+            os.system(f'pypubmed search "{query_box}" -o {outfile}')
     else:
         click.echo(res)
```

### Comparing `pypubmed-1.0.9/pypubmed/bin/cli.py` & `pypubmed-1.1.0/pypubmed/bin/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 
 @click.group(context_settings=CONTEXT_SETTINGS, epilog=__epilog__, help=click.style(version_info['desc'], fg='bright_blue', bold=True))
 @click.option('-l', '--log-level', help='the mode of loggging',
               show_default=True, default='debug',
               type=click.Choice(log_level_maps.keys()))
 @click.option('-k', '--api-key', help='the api_key of NCBI Pubmed, NCBI_API_KEY environment is available',
               envvar='NCBI_API_KEY', show_envvar=True)
-@click.option('-u', '--url', help='the service url of google translate', default='translate.google.cn', show_default=True)
+@click.option('-p', '--proxies', help='the proxies for google translate, eg. http://127.0.0.1:1080',)
 @click.version_option(version=version_info['version'], prog_name='pypubmed')
 @click.pass_context
 def cli(ctx, **kwargs):
 
     kwargs['log_level'] = log_level_maps[kwargs['log_level']]
-    e = Eutils(api_key=kwargs['api_key'], service_url=kwargs['url'])
+    e = Eutils(api_key=kwargs['api_key'], proxies=kwargs['proxies'])
     e.logger.level = int(kwargs['log_level'])
     ctx.obj = {
         'eutils': e
     }
 
 
 def main():
```

### Comparing `pypubmed-1.0.9/pypubmed/core/article.py` & `pypubmed-1.1.0/pypubmed/core/article.py`

 * *Files identical despite different names*

### Comparing `pypubmed-1.0.9/pypubmed/core/citations.py` & `pypubmed-1.1.0/pypubmed/core/citations.py`

 * *Files identical despite different names*

### Comparing `pypubmed-1.0.9/pypubmed/core/eutils.py` & `pypubmed-1.1.0/pypubmed/core/eutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 import datetime
 
 import click
 import prettytable
 
 from dateutil.parser import parse as date_parse
 
-from impact_factor import ImpactFactor
-from simple_googletrans import GoogleTrans
+from impact_factor.core import Factor as ImpactFactor
+from googletranslatepy import Translator as GoogleTrans
 from simple_loggers import SimpleLogger
 from webrequests import WebRequest
 
 
 from pypubmed.util import xml_parser
 from pypubmed.core.article import Article
 
@@ -34,19 +34,22 @@
             id          id(s) for efetch
             field       field for esearch
     """
     base_url = 'https://eutils.ncbi.nlm.nih.gov/entrez/eutils/'
     logger = SimpleLogger('Eutils')
     IF = ImpactFactor()
 
-    def __init__(self, db='pubmed', service_url='translate.google.cn', api_key=None, **kwargs):
+    def __init__(self, db='pubmed', proxies=None, api_key=None, **kwargs):
         self.db = db
         self.api_key = api_key
         self.validate_api_key()
-        self.TR = GoogleTrans(service_url=service_url)
+        self.TR = GoogleTrans(proxies=proxies)
+
+        self.TR_OK = self.TR.check_proxies()
+
 
     def parse_params(self, **kwargs):
         """
             - add default db
             - add api_key if available
         """
         params = {'db': self.db}
@@ -66,63 +69,72 @@
             > -search from a database from given term
             >> - esearch.cgi?db=pubmed&term=ngs
             >> - esearch.cgi?db=pubmed&term=ngs&retmode=xml&field=TIAB
             >> - esearch.cgi?db=pubmed&term=ngs[Title/Abstract]&retmode=xml
         """
         url = self.base_url + 'esearch.fcgi'
         params = self.parse_params(term=term, retmode='json', retstart=retstart, retmax=retmax, **kwargs)
+
+        # print(params)
+
         result = WebRequest.get_response(url, params=params).json()['esearchresult']
 
         if head:
             return result
 
         self.logger.info('{count} articles found with term: {querytranslation}'.format(**result))
+
+        if limit is None and int(result['count']) > 250:
+            self.logger.warning('too many results, you can limit output with option "-l/--limit N", '
+                                'or simplify your input with sub-command "advance-search" ')
+            exit(1)
+
         idlist = result['idlist']
 
         while int(result['retstart']) + int(result['retmax']) < int(result['count']):
-            if limit and int(result['retstart']) + int(result['retmax']) > limit:
+            if limit and len(idlist) >= limit:
                 break
             retstart = int(result['retstart']) + int(result['retmax'])
             params = self.parse_params(term=term, retmode='json', retstart=retstart, retmax=retmax, **kwargs)
             result = WebRequest.get_response(url, params=params).json()['esearchresult']
             idlist += result['idlist']
 
+        if limit:
+            self.logger.info('limit {} from {}'.format(limit, result['count']))
+            idlist = idlist[:limit]
+
         if idlist:
-            self.logger.info('idlist: {} ...'.format(', '.join(idlist[:10])))
+            self.logger.debug('idlist: {} ...'.format(', '.join(idlist[:10])))
         else:
             self.logger.warning('no result for term: {}'.format(term))
+
         return idlist
 
-    def efetch(self, ids, batch_size=5, show_process=False, **kwargs):
+    def efetch(self, ids, batch_size=5, **kwargs):
         """
             https://www.ncbi.nlm.nih.gov/books/NBK25499/#chapter4.EFetch
 
             > - fetch from a database for given ids
             >> efetch.cgi?db=pubmed&id=1,2,3
         """
         url = self.base_url + 'efetch.fcgi'
 
         self.logger.info('fetching start: total {}, batch_size: {}'.format(len(ids), batch_size))
 
-        with click.progressbar(length=len(ids), show_percent=True, empty_char=' ', fill_char='>') as pbar:
-            for n in range(0, len(ids), batch_size):
-                _id = ','.join(ids[n:n+batch_size])
-                if show_process:
-                    end =  n + batch_size if n + batch_size <= len(ids) else len(ids)
-                    pbar.label = 'Fetching {}-{}'.format(n+1, end)
-                    pbar.update(batch_size)
-                n += batch_size
-
-                params = self.parse_params(id=_id, retmode='xml')
-
-                xml = WebRequest.get_response(url, params=params).text
-                
-                for context in xml_parser.parse(xml):
-                    article = Article(**context)
-                    yield article
+        for n in range(0, len(ids), batch_size):
+            _id = ','.join(ids[n:n+batch_size])
+
+            self.logger.debug(f'fetching xml: {n+1} - {n+batch_size}')
+            params = self.parse_params(id=_id, retmode='xml')
+            xml = WebRequest.get_response(url, params=params).text
+            
+            self.logger.debug(f'parsing xml: {n+1} - {n+batch_size}')
+            for context in xml_parser.parse(xml):
+                article = Article(**context)
+                yield article
 
     def einfo(self, **kwargs):
         """
             https://www.ncbi.nlm.nih.gov/books/NBK25499/#chapter4.EInfo
 
             > - show all database list
             >> einfo.fcgi?db=
@@ -227,44 +239,39 @@
             self.logger.warning('invalid api_key, please check: {}'.format(self.api_key))
             self.api_key = None
         else:
             self.logger.info('Valid api_key: {}'.format(self.api_key))
             with open(configfile, 'w') as out:
                 out.write(self.api_key)
 
-    def search(self, term, cited=True, translate=True, impact_factor=True, limit=None, **kwargs):
+    def search(self, term, cited=True, translate=True, impact_factor=True, translate_cache=None, **kwargs):
         """
             term:
                 - string, eg. 'ngs AND disease'
                 - pmid, eg. 1,2,3
                 - file with pmid
         """
         if os.path.isfile(term):
             idlist = open(term).read().strip().split()
         elif all(each.isdigit() for each in term.split(',')):
             idlist = term.split(',')
         else:
-            idlist = self.esearch(term, limit=limit)
-
-        # print(kwargs);exit()
+            idlist = self.esearch(term, **kwargs)
 
         articles = self.efetch(idlist, **kwargs)
         for article in articles:
             if impact_factor:
                 res = self.IF.search(article.issn) or self.IF.search(article.e_issn)
-                article.impact_factor = res['factor'] if res else '.'
+                article.impact_factor = res[0]['factor'] if res else '.'
 
             if cited:
                 article.cited = self.get_cited(article.pmid)
-                
-            if translate:
-                article.abstract_cn = 'translate failed'
-                n = 0
-                while n < 5:
-                    n += 1
+
+            if translate and self.TR_OK:
+                if translate_cache and translate_cache.get(article.pmid):
+                    article.abstract_cn = translate_cache.get(article.pmid)
+                else:
                     try:
                         article.abstract_cn = self.TR.translate(article.abstract)
-                        break
                     except Exception as e:
-                        print(e)
-                        time.sleep(3)
+                        article.abstract_cn = 'translate failed'
             yield article
```

### Comparing `pypubmed-1.0.9/pypubmed/core/export.py` & `pypubmed-1.1.0/pypubmed/core/export.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,18 +9,30 @@
 from pypubmed.util import safe_open
 
 
 class Export(object):
 
     logger = SimpleLogger('Export')
 
-    def __init__(self, data, outfile='out.xlsx', outtype=None, fields=None, **kwargs):
+    def __init__(self, data, outfile='out.xlsx', outtype=None, fields=None, fillna='.', **kwargs):
         self.outfile = outfile
         self.outtype = outtype or outfile.split('.')[-1]
-        self.data = list(self.filter_data(data, fields)) if fields else data
+        # self.data = list(self.filter_data(data, fields)) if fields else data
+        self.data = list(self.reformat_data(data, fields=fields, fillna=fillna))
+
+    def reformat_data(self, data, fields, fillna):
+
+        if fields:
+            field_list = fields.strip(',').split(',')
+        else:
+            field_list = data[0].keys()
+
+        for context in data:
+            out_ctx = {k: v or fillna for k, v in context.items() if k in field_list}
+            yield out_ctx
 
     def filter_data(self, data, fields):
         fields = fields.strip(',').split(',')
         for context in data:
             out_ctx = {k: v for k, v in context.items() if k in fields}
             yield out_ctx
 
@@ -124,19 +136,23 @@
                     except:
                         try:
                             value = json.dumps(value, ensure_ascii=False)
                         except:
                             value = str(value)
                 elif type(value) == dict:
                     value = json.dumps(value, ensure_ascii=False)
-                    
-                _ = sheet.cell(row, col, value=value)
+                
+                try:
+                    _ = sheet.cell(row, col, value=value)
+                except:
+                    _ = sheet.cell(row, col, value=str(value))
+
                 _.fill = PatternFill(start_color=color, end_color=color, fill_type="solid")
 
-                if key in ('pmid', 'pmc', 'doi') and value != '.':
+                if key in ('pmid', 'pmc', 'doi') and value not in ('.', None):
                     _.hyperlink = self.add_hyperlink(key, value)
                     _.font = Font(color=colors.BLUE, italic=True)
 
                 wrap_text = None
                 if key in ('abstract', 'abstract_cn'):
                     wrap_text = True
```

### Comparing `pypubmed-1.0.9/pypubmed/util/xml_parser.py` & `pypubmed-1.1.0/pypubmed/util/xml_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -117,37 +117,46 @@
 
             context['abstract'] = parse_abstract(Article.xpath('Abstract/AbstractText'))
             
             author_mail = []
 
             author_list = []
             for author in Article.xpath('AuthorList/Author'):
-                name = [each.text for each in author.xpath('*')][:3]  # LastName, ForeName, Initials
-                author_list.append(name)
+                names = [each.text for each in author.xpath('*')][:3]  # LastName, ForeName, Initials
+                names = [n for n in names if n]
+                author_list.append(' '.join([names[-1], names[0]]))
+
                 affiliation = '\n'.join(author.xpath('AffiliationInfo/Affiliation/text()'))
                 mail = re.findall(r'([^\s]+?@.+)\.', str(affiliation))
                 if mail:
-                    mail = '{}:{}'.format(' '.join(name), mail[0])
+                    mail = '{}:{}'.format(' '.join(names), mail[0])
                     author_mail.append(mail)
 
             context['author_mail'] = '\n'.join(author_mail) or '.'
+            authors = Article.xpath('AuthorList/Author/AffiliationInfo/Affiliation/text()')
+            context['author_first'] = context['author_last'] = '.'
+            if authors:
+                context['author_first'] = authors[0]
+                if len(authors) > 1:
+                    context['author_last'] = authors[-1]
 
-            context['authors'] = author_list
+            context['authors'] = ',\n'.join(author_list)
 
             context['pub_types'] = Article.xpath('PublicationTypeList/PublicationType/text()')
             context['doi'] = PubmedArticle.findtext('PubmedData/ArticleIdList/ArticleId[@IdType="doi"]')
             context['pmc'] = PubmedArticle.findtext('PubmedData/ArticleIdList/ArticleId[@IdType="pmc"]')
 
             yield context
 
 
 if __name__ == '__main__':
     import json
     from webrequests import WebRequest
     
     pmid = '17284678,9997'
     pmid = '28143587'
+    pmid = '33577981'
     
     url = f'https://eutils.ncbi.nlm.nih.gov/entrez/eutils/efetch.fcgi?db=pubmed&id={pmid}&retmode=xml'
     resp = WebRequest.get_response(url)
     for context in parse(resp.text):
         print(json.dumps(context, indent=2))
```

### Comparing `pypubmed-1.0.9/pypubmed.egg-info/PKG-INFO` & `pypubmed-1.1.0/pypubmed.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: pypubmed
-Version: 1.0.9
+Version: 1.1.0
 Summary: Toolkits for NCBI Pubmed
 Home-page: https://github.com/suqingdong/pypubmed
 Author: suqingdong
-Author-email: 1078595229@qq.com
+Author-email: suqingdong1114@gmail.com
 License: BSD License
 Project-URL: Documentation, https://pypubmed.readthedocs.io
 Project-URL: Tracker, https://github.com/suqingdong/pypubmed/issues
 Description: # NCBI Pubmed Toolkits
         
         ## Requirements
         - Python3.6+
         
         ## Installation
         ```bash
-        pip3 isntall pypubmed
+        python3 -m pip install -U pypubmed
         ```
         
         ## Usage
         ### `search`
         > search Pubmed with term
         ```bash
         pypubmed search --help
+        
+        # do not translate
+        pypubmed search -l 5 ngs
+        
+        # translate with a local proxies
+        pypubmed -p http://127.0.0.1:1081 search ngs -l 5
         ```
         
         ### `advance-search`
         > advance search builder
         ```bash
         pypubmed advance-search --help
         ```
@@ -40,15 +46,14 @@
         
         ## Todos
         - [ ] HTML output
         - [ ] PDF downloader
         - [ ] GUI application
         - [ ] Local paper manager
         
-        
         ## Documents
         > https://pypubmed.readthedocs.io/en/latest/
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `pypubmed-1.0.9/pypubmed.egg-info/SOURCES.txt` & `pypubmed-1.1.0/pypubmed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypubmed-1.0.9/setup.py` & `pypubmed-1.1.0/setup.py`

 * *Files identical despite different names*

