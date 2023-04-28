# Comparing `tmp/wikipedia_tools-2.2.4.tar.gz` & `tmp/wikipedia_tools-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikipedia_tools-2.2.4.tar", last modified: Fri Apr 28 14:51:57 2023, max compression
+gzip compressed data, was "wikipedia_tools-2.2.5.tar", last modified: Fri Apr 28 14:58:49 2023, max compression
```

## Comparing `wikipedia_tools-2.2.4.tar` & `wikipedia_tools-2.2.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      809 2023-03-06 10:30:11.407905 wikipedia_tools-2.2.4/.gitignore
--rw-r--r--   0        0        0     1087 2023-02-02 12:41:11.859474 wikipedia_tools-2.2.4/LICENSE
--rw-r--r--   0        0        0       13 2023-03-06 09:14:10.632797 wikipedia_tools-2.2.4/MANIFEST.in
--rw-r--r--   0        0        0     5519 2023-04-28 13:10:58.061816 wikipedia_tools-2.2.4/README.md
--rw-r--r--   0        0        0    46275 2023-02-14 11:20:18.342741 wikipedia_tools-2.2.4/data/wikipedia_wikiproject_climate_change_popular_pages.csv
--rw-r--r--   0        0        0     1756 2023-04-28 14:51:32.767938 wikipedia_tools-2.2.4/pyproject.toml
--rw-r--r--   0        0        0      187 2023-03-06 09:14:10.634896 wikipedia_tools-2.2.4/requirements.txt
--rw-r--r--   0        0        0      657 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.4/wikipedia_tools/.gitignore
--rw-r--r--   0        0        0      178 2023-03-06 09:15:47.055300 wikipedia_tools-2.2.4/wikipedia_tools/__init__.py
--rw-r--r--   0        0        0        0 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.4/wikipedia_tools/analyzer/__init__.py
--rw-r--r--   0        0        0     3115 2023-03-06 09:17:55.315451 wikipedia_tools-2.2.4/wikipedia_tools/analyzer/feature_extractor.py
--rw-r--r--   0        0        0    14142 2023-04-28 13:16:26.515779 wikipedia_tools-2.2.4/wikipedia_tools/analyzer/numbers_over_time.py
--rw-r--r--   0        0        0      956 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.4/wikipedia_tools/analyzer/revisions.py
--rw-r--r--   0        0        0      228 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.4/wikipedia_tools/base/wikipedia_w_time/__init__.py
--rw-r--r--   0        0        0     2647 2023-03-06 09:17:55.316899 wikipedia_tools-2.2.4/wikipedia_tools/base/wikipedia_w_time/exceptions.py
--rw-r--r--   0        0        0     1112 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.4/wikipedia_tools/base/wikipedia_w_time/util.py
--rw-r--r--   0        0        0    28546 2023-03-06 09:17:55.617021 wikipedia_tools-2.2.4/wikipedia_tools/base/wikipedia_w_time/wikipedia.py
--rw-r--r--   0        0        0        0 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.4/wikipedia_tools/processor/__init__.py
--rw-r--r--   0        0        0     2042 2023-03-06 09:17:55.289957 wikipedia_tools-2.2.4/wikipedia_tools/processor/loader.py
--rw-r--r--   0        0        0    10060 2023-04-28 14:46:31.094626 wikipedia_tools-2.2.4/wikipedia_tools/processor/processor.py
--rw-r--r--   0        0        0        0 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.4/wikipedia_tools/scraper/__init__.py
--rw-r--r--   0        0        0      506 2023-03-06 10:32:12.455252 wikipedia_tools-2.2.4/wikipedia_tools/scraper/category_extractor.py
--rw-r--r--   0        0        0     7651 2023-03-06 10:32:12.530602 wikipedia_tools-2.2.4/wikipedia_tools/scraper/downloader.py
--rw-r--r--   0        0        0     3595 2023-03-06 09:51:13.612909 wikipedia_tools-2.2.4/wikipedia_tools/scraper/revision_extractor.py
--rw-r--r--   0        0        0     2240 2023-03-06 10:32:12.476905 wikipedia_tools-2.2.4/wikipedia_tools/scraper/wikipedia_parser.py
--rw-r--r--   0        0        0    12707 2023-03-06 09:55:23.169074 wikipedia_tools-2.2.4/wikipedia_tools/scraper/wikirevparser_with_time.py
--rw-r--r--   0        0        0        0 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.4/wikipedia_tools/utils/__init__.py
--rw-r--r--   0        0        0     1615 2023-03-06 09:17:55.360436 wikipedia_tools-2.2.4/wikipedia_tools/utils/properties.py
--rw-r--r--   0        0        0      968 2023-03-06 09:34:35.326387 wikipedia_tools-2.2.4/wikipedia_tools/utils/utils.py
--rw-r--r--   0        0        0     6180 1970-01-01 00:00:00.000000 wikipedia_tools-2.2.4/PKG-INFO
+-rw-r--r--   0        0        0      809 2023-03-06 10:30:11.407905 wikipedia_tools-2.2.5/.gitignore
+-rw-r--r--   0        0        0     1087 2023-02-02 12:41:11.859474 wikipedia_tools-2.2.5/LICENSE
+-rw-r--r--   0        0        0       13 2023-03-06 09:14:10.632797 wikipedia_tools-2.2.5/MANIFEST.in
+-rw-r--r--   0        0        0     5519 2023-04-28 13:10:58.061816 wikipedia_tools-2.2.5/README.md
+-rw-r--r--   0        0        0    46275 2023-02-14 11:20:18.342741 wikipedia_tools-2.2.5/data/wikipedia_wikiproject_climate_change_popular_pages.csv
+-rw-r--r--   0        0        0     1756 2023-04-28 14:58:40.420985 wikipedia_tools-2.2.5/pyproject.toml
+-rw-r--r--   0        0        0      187 2023-03-06 09:14:10.634896 wikipedia_tools-2.2.5/requirements.txt
+-rw-r--r--   0        0        0      657 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.5/wikipedia_tools/.gitignore
+-rw-r--r--   0        0        0      178 2023-03-06 09:15:47.055300 wikipedia_tools-2.2.5/wikipedia_tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.5/wikipedia_tools/analyzer/__init__.py
+-rw-r--r--   0        0        0     3115 2023-03-06 09:17:55.315451 wikipedia_tools-2.2.5/wikipedia_tools/analyzer/feature_extractor.py
+-rw-r--r--   0        0        0    14142 2023-04-28 13:16:26.515779 wikipedia_tools-2.2.5/wikipedia_tools/analyzer/numbers_over_time.py
+-rw-r--r--   0        0        0      956 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.5/wikipedia_tools/analyzer/revisions.py
+-rw-r--r--   0        0        0      228 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.5/wikipedia_tools/base/wikipedia_w_time/__init__.py
+-rw-r--r--   0        0        0     2647 2023-03-06 09:17:55.316899 wikipedia_tools-2.2.5/wikipedia_tools/base/wikipedia_w_time/exceptions.py
+-rw-r--r--   0        0        0     1112 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.5/wikipedia_tools/base/wikipedia_w_time/util.py
+-rw-r--r--   0        0        0    28546 2023-03-06 09:17:55.617021 wikipedia_tools-2.2.5/wikipedia_tools/base/wikipedia_w_time/wikipedia.py
+-rw-r--r--   0        0        0        0 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.5/wikipedia_tools/processor/__init__.py
+-rw-r--r--   0        0        0     2042 2023-03-06 09:17:55.289957 wikipedia_tools-2.2.5/wikipedia_tools/processor/loader.py
+-rw-r--r--   0        0        0    10058 2023-04-28 14:58:28.661675 wikipedia_tools-2.2.5/wikipedia_tools/processor/processor.py
+-rw-r--r--   0        0        0        0 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.5/wikipedia_tools/scraper/__init__.py
+-rw-r--r--   0        0        0      506 2023-03-06 10:32:12.455252 wikipedia_tools-2.2.5/wikipedia_tools/scraper/category_extractor.py
+-rw-r--r--   0        0        0     7651 2023-03-06 10:32:12.530602 wikipedia_tools-2.2.5/wikipedia_tools/scraper/downloader.py
+-rw-r--r--   0        0        0     3595 2023-03-06 09:51:13.612909 wikipedia_tools-2.2.5/wikipedia_tools/scraper/revision_extractor.py
+-rw-r--r--   0        0        0     2240 2023-03-06 10:32:12.476905 wikipedia_tools-2.2.5/wikipedia_tools/scraper/wikipedia_parser.py
+-rw-r--r--   0        0        0    12707 2023-03-06 09:55:23.169074 wikipedia_tools-2.2.5/wikipedia_tools/scraper/wikirevparser_with_time.py
+-rw-r--r--   0        0        0        0 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.5/wikipedia_tools/utils/__init__.py
+-rw-r--r--   0        0        0     1615 2023-03-06 09:17:55.360436 wikipedia_tools-2.2.5/wikipedia_tools/utils/properties.py
+-rw-r--r--   0        0        0      968 2023-03-06 09:34:35.326387 wikipedia_tools-2.2.5/wikipedia_tools/utils/utils.py
+-rw-r--r--   0        0        0     6180 1970-01-01 00:00:00.000000 wikipedia_tools-2.2.5/PKG-INFO
```

### Comparing `wikipedia_tools-2.2.4/.gitignore` & `wikipedia_tools-2.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.4/LICENSE` & `wikipedia_tools-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.4/README.md` & `wikipedia_tools-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.4/data/wikipedia_wikiproject_climate_change_popular_pages.csv` & `wikipedia_tools-2.2.5/data/wikipedia_wikiproject_climate_change_popular_pages.csv`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.4/pyproject.toml` & `wikipedia_tools-2.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 
 [project]
 name = "wikipedia_tools"
-version = "2.2.4"
+version = "2.2.5"
 description='This is a Wikipedia Tool to fetch revisions based on a period of time.'
 readme = "README.md"
 authors = [{ name = "Roxanne El Baff", email = "roxanne.elbaff@dlr.de" }]
 license = { file = "LICENSE" }
 keywords=['wikipedia', 'wikipedia revisions', 'wikipedia stats']
 dependencies = ['pandas>=1.0.1',
                       'matplotlib>=3.2.1',
```

### Comparing `wikipedia_tools-2.2.4/wikipedia_tools/.gitignore` & `wikipedia_tools-2.2.5/wikipedia_tools/.gitignore`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.4/wikipedia_tools/analyzer/feature_extractor.py` & `wikipedia_tools-2.2.5/wikipedia_tools/analyzer/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.4/wikipedia_tools/analyzer/numbers_over_time.py` & `wikipedia_tools-2.2.5/wikipedia_tools/analyzer/numbers_over_time.py`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.4/wikipedia_tools/analyzer/revisions.py` & `wikipedia_tools-2.2.5/wikipedia_tools/analyzer/revisions.py`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.4/wikipedia_tools/base/wikipedia_w_time/exceptions.py` & `wikipedia_tools-2.2.5/wikipedia_tools/base/wikipedia_w_time/exceptions.py`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.4/wikipedia_tools/base/wikipedia_w_time/util.py` & `wikipedia_tools-2.2.5/wikipedia_tools/base/wikipedia_w_time/util.py`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.4/wikipedia_tools/base/wikipedia_w_time/wikipedia.py` & `wikipedia_tools-2.2.5/wikipedia_tools/base/wikipedia_w_time/wikipedia.py`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.4/wikipedia_tools/processor/loader.py` & `wikipedia_tools-2.2.5/wikipedia_tools/processor/loader.py`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.4/wikipedia_tools/processor/processor.py` & `wikipedia_tools-2.2.5/wikipedia_tools/processor/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,10 +270,10 @@
             ]
             revision_per_period["urls"] = latest_df["urls"].values[0]
             result_arr.append(revision_per_period)
 
     result_df = pd.DataFrame(result_arr)  # , index = ['period', 'title'])
     try:
         result_df.to_csv(fname, index=False)
-    except Exception e:
+    except Exception:
         print("Failed to save File")
     return result_df
```

### Comparing `wikipedia_tools-2.2.4/wikipedia_tools/scraper/downloader.py` & `wikipedia_tools-2.2.5/wikipedia_tools/scraper/downloader.py`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.4/wikipedia_tools/scraper/revision_extractor.py` & `wikipedia_tools-2.2.5/wikipedia_tools/scraper/revision_extractor.py`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.4/wikipedia_tools/scraper/wikipedia_parser.py` & `wikipedia_tools-2.2.5/wikipedia_tools/scraper/wikipedia_parser.py`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.4/wikipedia_tools/scraper/wikirevparser_with_time.py` & `wikipedia_tools-2.2.5/wikipedia_tools/scraper/wikirevparser_with_time.py`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.4/wikipedia_tools/utils/properties.py` & `wikipedia_tools-2.2.5/wikipedia_tools/utils/properties.py`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.4/wikipedia_tools/utils/utils.py` & `wikipedia_tools-2.2.5/wikipedia_tools/utils/utils.py`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.4/PKG-INFO` & `wikipedia_tools-2.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikipedia_tools
-Version: 2.2.4
+Version: 2.2.5
 Summary: This is a Wikipedia Tool to fetch revisions based on a period of time.
 Keywords: wikipedia,wikipedia revisions,wikipedia stats
 Author-email: Roxanne El Baff <roxanne.elbaff@dlr.de>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: pandas>=1.0.1
 Requires-Dist: matplotlib>=3.2.1
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wikipedia_tools Version: 2.2.4 Summary: This is a
+Metadata-Version: 2.1 Name: wikipedia_tools Version: 2.2.5 Summary: This is a
 Wikipedia Tool to fetch revisions based on a period of time. Keywords:
 wikipedia,wikipedia revisions,wikipedia stats Author-email: Roxanne El Baff
 elbaff@dlr.de> Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Requires-Dist: pandas>=1.0.1 Requires-Dist: matplotlib>=3.2.1 Requires-Dist:
 pymediawiki==0.7.2 Requires-Dist: IPy>=1.01 Requires-Dist: seaborn>=0.11.2
 Requires-Dist: nlpaf>1.0.0; python_version <= "3.8" Requires-Dist: tqdm==4.43.0
 Requires-Dist: dataclasses==0.6 Requires-Dist: beautifulsoup4 Requires-Dist:
```

