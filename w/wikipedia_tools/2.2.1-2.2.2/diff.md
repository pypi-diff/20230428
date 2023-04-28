# Comparing `tmp/wikipedia_tools-2.2.1.tar.gz` & `tmp/wikipedia_tools-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikipedia_tools-2.2.1.tar", last modified: Mon Mar  6 10:31:34 2023, max compression
+gzip compressed data, was "wikipedia_tools-2.2.2.tar", last modified: Fri Apr 28 13:11:26 2023, max compression
```

## Comparing `wikipedia_tools-2.2.1.tar` & `wikipedia_tools-2.2.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      809 2023-03-06 10:30:11.407905 wikipedia_tools-2.2.1/.gitignore
--rw-r--r--   0        0        0     1087 2023-02-02 12:41:11.859474 wikipedia_tools-2.2.1/LICENSE
--rw-r--r--   0        0        0       13 2023-03-06 09:14:10.632797 wikipedia_tools-2.2.1/MANIFEST.in
--rw-r--r--   0        0        0     5508 2023-03-06 10:29:31.892145 wikipedia_tools-2.2.1/README.md
--rw-r--r--   0        0        0    46275 2023-02-14 11:20:18.342741 wikipedia_tools-2.2.1/data/wikipedia_wikiproject_climate_change_popular_pages.csv
--rw-r--r--   0        0        0     1756 2023-03-06 10:30:55.750518 wikipedia_tools-2.2.1/pyproject.toml
--rw-r--r--   0        0        0      187 2023-03-06 09:14:10.634896 wikipedia_tools-2.2.1/requirements.txt
--rw-r--r--   0        0        0      657 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.1/wikipedia_tools/.gitignore
--rw-r--r--   0        0        0      178 2023-03-06 09:15:47.055300 wikipedia_tools-2.2.1/wikipedia_tools/__init__.py
--rw-r--r--   0        0        0        0 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.1/wikipedia_tools/analyzer/__init__.py
--rw-r--r--   0        0        0     3115 2023-03-06 09:17:55.315451 wikipedia_tools-2.2.1/wikipedia_tools/analyzer/feature_extractor.py
--rw-r--r--   0        0        0    13854 2023-03-06 09:17:55.529729 wikipedia_tools-2.2.1/wikipedia_tools/analyzer/numbers_over_time.py
--rw-r--r--   0        0        0      956 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.1/wikipedia_tools/analyzer/revisions.py
--rw-r--r--   0        0        0      228 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.1/wikipedia_tools/base/wikipedia_w_time/__init__.py
--rw-r--r--   0        0        0     2647 2023-03-06 09:17:55.316899 wikipedia_tools-2.2.1/wikipedia_tools/base/wikipedia_w_time/exceptions.py
--rw-r--r--   0        0        0     1112 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.1/wikipedia_tools/base/wikipedia_w_time/util.py
--rw-r--r--   0        0        0    28546 2023-03-06 09:17:55.617021 wikipedia_tools-2.2.1/wikipedia_tools/base/wikipedia_w_time/wikipedia.py
--rw-r--r--   0        0        0        0 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.1/wikipedia_tools/processor/__init__.py
--rw-r--r--   0        0        0     2042 2023-03-06 09:17:55.289957 wikipedia_tools-2.2.1/wikipedia_tools/processor/loader.py
--rw-r--r--   0        0        0     9938 2023-03-06 09:17:55.472762 wikipedia_tools-2.2.1/wikipedia_tools/processor/processor.py
--rw-r--r--   0        0        0        0 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.1/wikipedia_tools/scraper/__init__.py
--rw-r--r--   0        0        0      503 2023-03-06 10:03:11.021079 wikipedia_tools-2.2.1/wikipedia_tools/scraper/category_extractor.py
--rw-r--r--   0        0        0     7648 2023-03-06 10:20:34.429909 wikipedia_tools-2.2.1/wikipedia_tools/scraper/downloader.py
--rw-r--r--   0        0        0     3595 2023-03-06 09:51:13.612909 wikipedia_tools-2.2.1/wikipedia_tools/scraper/revision_extractor.py
--rw-r--r--   0        0        0     2179 2023-03-06 10:04:05.312903 wikipedia_tools-2.2.1/wikipedia_tools/scraper/wikipedia_parser.py
--rw-r--r--   0        0        0    12707 2023-03-06 09:55:23.169074 wikipedia_tools-2.2.1/wikipedia_tools/scraper/wikirevparser_with_time.py
--rw-r--r--   0        0        0        0 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.1/wikipedia_tools/utils/__init__.py
--rw-r--r--   0        0        0     1615 2023-03-06 09:17:55.360436 wikipedia_tools-2.2.1/wikipedia_tools/utils/properties.py
--rw-r--r--   0        0        0      968 2023-03-06 09:34:35.326387 wikipedia_tools-2.2.1/wikipedia_tools/utils/utils.py
--rw-r--r--   0        0        0     6170 1970-01-01 00:00:00.000000 wikipedia_tools-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0      809 2023-03-06 10:30:11.407905 wikipedia_tools-2.2.2/.gitignore
+-rw-r--r--   0        0        0     1087 2023-02-02 12:41:11.859474 wikipedia_tools-2.2.2/LICENSE
+-rw-r--r--   0        0        0       13 2023-03-06 09:14:10.632797 wikipedia_tools-2.2.2/MANIFEST.in
+-rw-r--r--   0        0        0     5519 2023-04-28 13:10:58.061816 wikipedia_tools-2.2.2/README.md
+-rw-r--r--   0        0        0    46275 2023-02-14 11:20:18.342741 wikipedia_tools-2.2.2/data/wikipedia_wikiproject_climate_change_popular_pages.csv
+-rw-r--r--   0        0        0     1756 2023-04-28 13:07:26.059822 wikipedia_tools-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0      187 2023-03-06 09:14:10.634896 wikipedia_tools-2.2.2/requirements.txt
+-rw-r--r--   0        0        0      657 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.2/wikipedia_tools/.gitignore
+-rw-r--r--   0        0        0      178 2023-03-06 09:15:47.055300 wikipedia_tools-2.2.2/wikipedia_tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.2/wikipedia_tools/analyzer/__init__.py
+-rw-r--r--   0        0        0     3115 2023-03-06 09:17:55.315451 wikipedia_tools-2.2.2/wikipedia_tools/analyzer/feature_extractor.py
+-rw-r--r--   0        0        0    14115 2023-04-28 13:10:48.538528 wikipedia_tools-2.2.2/wikipedia_tools/analyzer/numbers_over_time.py
+-rw-r--r--   0        0        0      956 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.2/wikipedia_tools/analyzer/revisions.py
+-rw-r--r--   0        0        0      228 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.2/wikipedia_tools/base/wikipedia_w_time/__init__.py
+-rw-r--r--   0        0        0     2647 2023-03-06 09:17:55.316899 wikipedia_tools-2.2.2/wikipedia_tools/base/wikipedia_w_time/exceptions.py
+-rw-r--r--   0        0        0     1112 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.2/wikipedia_tools/base/wikipedia_w_time/util.py
+-rw-r--r--   0        0        0    28546 2023-03-06 09:17:55.617021 wikipedia_tools-2.2.2/wikipedia_tools/base/wikipedia_w_time/wikipedia.py
+-rw-r--r--   0        0        0        0 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.2/wikipedia_tools/processor/__init__.py
+-rw-r--r--   0        0        0     2042 2023-03-06 09:17:55.289957 wikipedia_tools-2.2.2/wikipedia_tools/processor/loader.py
+-rw-r--r--   0        0        0     9938 2023-03-06 09:17:55.472762 wikipedia_tools-2.2.2/wikipedia_tools/processor/processor.py
+-rw-r--r--   0        0        0        0 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.2/wikipedia_tools/scraper/__init__.py
+-rw-r--r--   0        0        0      506 2023-03-06 10:32:12.455252 wikipedia_tools-2.2.2/wikipedia_tools/scraper/category_extractor.py
+-rw-r--r--   0        0        0     7651 2023-03-06 10:32:12.530602 wikipedia_tools-2.2.2/wikipedia_tools/scraper/downloader.py
+-rw-r--r--   0        0        0     3595 2023-03-06 09:51:13.612909 wikipedia_tools-2.2.2/wikipedia_tools/scraper/revision_extractor.py
+-rw-r--r--   0        0        0     2240 2023-03-06 10:32:12.476905 wikipedia_tools-2.2.2/wikipedia_tools/scraper/wikipedia_parser.py
+-rw-r--r--   0        0        0    12707 2023-03-06 09:55:23.169074 wikipedia_tools-2.2.2/wikipedia_tools/scraper/wikirevparser_with_time.py
+-rw-r--r--   0        0        0        0 2023-02-02 12:41:11.859981 wikipedia_tools-2.2.2/wikipedia_tools/utils/__init__.py
+-rw-r--r--   0        0        0     1615 2023-03-06 09:17:55.360436 wikipedia_tools-2.2.2/wikipedia_tools/utils/properties.py
+-rw-r--r--   0        0        0      968 2023-03-06 09:34:35.326387 wikipedia_tools-2.2.2/wikipedia_tools/utils/utils.py
+-rw-r--r--   0        0        0     6180 1970-01-01 00:00:00.000000 wikipedia_tools-2.2.2/PKG-INFO
```

### Comparing `wikipedia_tools-2.2.1/.gitignore` & `wikipedia_tools-2.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.1/LICENSE` & `wikipedia_tools-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.1/README.md` & `wikipedia_tools-2.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 ```python
 from wikipedia_tools.scraper import downloader
 from datetime import datetime
 
 wikirevs= downloader.WikiPagesRevision( 
                                         categories = ["Klimaveränderung"],
-                                        revisions_from = utils.get_x_months_ago_date(1), # beguinning of last month, you ca use datetime.now() + dateutil.relativedelta.relativedelta to customized past datetime relatively
+                                        revisions_from = utils.get_x_months_ago_date(1), # beginning of last month, you can use instead datetime.now() + dateutil.relativedelta.relativedelta() to customize past datetime relatively
                                         revisions_to=datetime.now(),
                                         save_each_page= True,
                                         lang="de"
                                         )
 count, destination_folder = wikirevs.download()
 
 ```
@@ -118,8 +118,8 @@
 
 # Loop over all wiki page revisions with this period and read each wiki page revs as a pandas dataframe
 for page_path in glob(files):
     page_revs_df = pd.read_parquet(page_name)
     # dataframe with columns ['page', 'lang', 'timestamp', 'categories', 'content', 'images', 'links', 'sections', 'urls', 'user']
     # process/use file ....
 
-```
+```
```

#### html2text {}

```diff
@@ -34,18 +34,18 @@
 ( categories = ["Climate_change"], revisions_from = utils.get_x_months_ago_date
 (8), revisions_to=datetime.now(), save_each_page= True ) count,
 destination_folder = wikirevs.download() ``` For german wiki revisions, you can
 set the *lang* attribute to *de* - For example, you can download the German
 Wikipedia page revisions for the Climate_change category, as follows: ```python
 from wikipedia_tools.scraper import downloader from datetime import datetime
 wikirevs= downloader.WikiPagesRevision( categories = ["KlimaverÃ¤nderung"],
-revisions_from = utils.get_x_months_ago_date(1), # beguinning of last month,
-you ca use datetime.now() + dateutil.relativedelta.relativedelta to customized
-past datetime relatively revisions_to=datetime.now(), save_each_page= True,
-lang="de" ) count, destination_folder = wikirevs.download() ``` You can then
-process each file by, for example, reading the parquet file using pandas:
+revisions_from = utils.get_x_months_ago_date(1), # beginning of last month, you
+can use instead datetime.now() + dateutil.relativedelta.relativedelta() to
+customize past datetime relatively revisions_to=datetime.now(), save_each_page=
+True, lang="de" ) count, destination_folder = wikirevs.download() ``` You can
+then process each file by, for example, reading the parquet file using pandas:
 ```python import pandas as pd from glob import glob files = f"
 {destination_folder}/*.parquet" # Loop over all wiki page revisions with this
 period and read each wiki page revs as a pandas dataframe for page_path in glob
 (files): page_revs_df = pd.read_parquet(page_name) # dataframe with columns
 ['page', 'lang', 'timestamp', 'categories', 'content', 'images', 'links',
 'sections', 'urls', 'user'] # process/use file .... ```
```

### Comparing `wikipedia_tools-2.2.1/data/wikipedia_wikiproject_climate_change_popular_pages.csv` & `wikipedia_tools-2.2.2/data/wikipedia_wikiproject_climate_change_popular_pages.csv`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.1/pyproject.toml` & `wikipedia_tools-2.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 
 [project]
 name = "wikipedia_tools"
-version = "2.2.1"
+version = "2.2.2"
 description='This is a Wikipedia Tool to fetch revisions based on a period of time.'
 readme = "README.md"
 authors = [{ name = "Roxanne El Baff", email = "roxanne.elbaff@dlr.de" }]
 license = { file = "LICENSE" }
 keywords=['wikipedia', 'wikipedia revisions', 'wikipedia stats']
 dependencies = ['pandas>=1.0.1',
                       'matplotlib>=3.2.1',
```

### Comparing `wikipedia_tools-2.2.1/wikipedia_tools/.gitignore` & `wikipedia_tools-2.2.2/wikipedia_tools/.gitignore`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.1/wikipedia_tools/analyzer/feature_extractor.py` & `wikipedia_tools-2.2.2/wikipedia_tools/analyzer/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.1/wikipedia_tools/analyzer/numbers_over_time.py` & `wikipedia_tools-2.2.2/wikipedia_tools/analyzer/numbers_over_time.py`

 * *Files 6% similar despite different names*

```diff
@@ -385,44 +385,50 @@
             desc.lower()
         )
         result_df.to_csv(f"{properties.STATS_FOLDER}/{name}")
     return result_df
 
 
 def get_attr_for_period_as_txt(
-    period_val,
+    period_val: int | list,
     attr_val: str = "links",
     only_popular=False,
     period=properties.DATE_YEAR,
     desc="YEAR",
 ) -> []:  ## could be categories or urls
-    periodic_df = processor.get_wikipedia_page_periodic_overview(
+    original_df = processor.get_wikipedia_page_periodic_overview(
         only_popular=only_popular, period=period, desc=desc
     )
-    periodic_df = periodic_df[periodic_df["period"] == period_val].copy()
-    periodic_df.sort_values(
-        by=["revision_count", "title"], inplace=True, ascending=False
-    )
 
-    result_arr = []
-    for _, row in periodic_df.iterrows():
-        lst_ = ast.literal_eval(row[attr_val])
-        lst_ = [x.replace(" ", "") for x in lst_]
-        if len(lst_) > 0:
-            result_arr.append(". ".join(lst_))
-
-    utils.create_folder(properties.STATS_FOLDER)
-    with open(
-        f"{properties.STATS_FOLDER}/{attr_val}_{period_val}.txt",
-        "w",
-        encoding="utf-8",
-    ) as f:
-        for line in result_arr:
-            f.write(f"{line}\n")
-    return result_arr
+    if type(period_val) == int:
+        period_val = [period_val]
+    res_dict = {}
+    for single_period in period_val:
+        periodic_df = original_df[original_df["period"] == single_period].copy()
+        periodic_df.sort_values(
+            by=["revision_count", "title"], inplace=True, ascending=False
+        )
+
+        result_arr = []
+        for _, row in periodic_df.iterrows():
+            lst_ = ast.literal_eval(row[attr_val])
+            lst_ = [x.replace(" ", "") for x in lst_]
+            if len(lst_) > 0:
+                result_arr.append(". ".join(lst_))
+
+        utils.create_folder(properties.STATS_FOLDER)
+        with open(
+            f"{properties.STATS_FOLDER}/{attr_val}_{single_period}.txt",
+            "w",
+            encoding="utf-8",
+        ) as f:
+            for line in result_arr:
+                f.write(f"{line}\n")
+        res_dict[single_period] = result_arr
+    return res_dict
 
 
 def get_periodic_revisions_percentage(
     only_popular=False,
     period=properties.DATE_YEAR,
     desc="YEAR",
     save: bool = False,
```

### Comparing `wikipedia_tools-2.2.1/wikipedia_tools/analyzer/revisions.py` & `wikipedia_tools-2.2.2/wikipedia_tools/analyzer/revisions.py`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.1/wikipedia_tools/base/wikipedia_w_time/exceptions.py` & `wikipedia_tools-2.2.2/wikipedia_tools/base/wikipedia_w_time/exceptions.py`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.1/wikipedia_tools/base/wikipedia_w_time/util.py` & `wikipedia_tools-2.2.2/wikipedia_tools/base/wikipedia_w_time/util.py`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.1/wikipedia_tools/base/wikipedia_w_time/wikipedia.py` & `wikipedia_tools-2.2.2/wikipedia_tools/base/wikipedia_w_time/wikipedia.py`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.1/wikipedia_tools/processor/loader.py` & `wikipedia_tools-2.2.2/wikipedia_tools/processor/loader.py`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.1/wikipedia_tools/processor/processor.py` & `wikipedia_tools-2.2.2/wikipedia_tools/processor/processor.py`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.1/wikipedia_tools/scraper/downloader.py` & `wikipedia_tools-2.2.2/wikipedia_tools/scraper/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from wikipedia_tools.utils import utils
 import random
 
 
 @dataclasses.dataclass
 class WikiPagesRevision:
     output_file: str = "all"
-    root_folder: str = "."#properties.ROOT_PATH
+    root_folder: str = "."  # properties.ROOT_PATH
     categories: List = dataclasses.field(
         default_factory=lambda: ["Climate_change"]
     )
     revisions_from: datetime = None
     revisions_to: datetime = datetime.now()
     save_each_page: bool = False
     category_depth: int = 3
```

### Comparing `wikipedia_tools-2.2.1/wikipedia_tools/scraper/revision_extractor.py` & `wikipedia_tools-2.2.2/wikipedia_tools/scraper/revision_extractor.py`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.1/wikipedia_tools/scraper/wikipedia_parser.py` & `wikipedia_tools-2.2.2/wikipedia_tools/scraper/wikipedia_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,18 @@
         pages = []
 
     if args.categories:
         pages = set(
             pages
             + reduce(
                 list.__add__,
-                [ce.get_category_pages(c, lang=args.language) for c in args.categories],
+                [
+                    ce.get_category_pages(c, lang=args.language)
+                    for c in args.categories
+                ],
             )
         )
 
     if len(pages) == 0:
         raise Exception(
             "No pages to parse. Please specify a proper category or a file with page names."
         )
```

### Comparing `wikipedia_tools-2.2.1/wikipedia_tools/scraper/wikirevparser_with_time.py` & `wikipedia_tools-2.2.2/wikipedia_tools/scraper/wikirevparser_with_time.py`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.1/wikipedia_tools/utils/properties.py` & `wikipedia_tools-2.2.2/wikipedia_tools/utils/properties.py`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.1/wikipedia_tools/utils/utils.py` & `wikipedia_tools-2.2.2/wikipedia_tools/utils/utils.py`

 * *Files identical despite different names*

### Comparing `wikipedia_tools-2.2.1/PKG-INFO` & `wikipedia_tools-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikipedia_tools
-Version: 2.2.1
+Version: 2.2.2
 Summary: This is a Wikipedia Tool to fetch revisions based on a period of time.
 Keywords: wikipedia,wikipedia revisions,wikipedia stats
 Author-email: Roxanne El Baff <roxanne.elbaff@dlr.de>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: pandas>=1.0.1
 Requires-Dist: matplotlib>=3.2.1
@@ -118,15 +118,15 @@
 
 ```python
 from wikipedia_tools.scraper import downloader
 from datetime import datetime
 
 wikirevs= downloader.WikiPagesRevision( 
                                         categories = ["Klimaveränderung"],
-                                        revisions_from = utils.get_x_months_ago_date(1), # beguinning of last month, you ca use datetime.now() + dateutil.relativedelta.relativedelta to customized past datetime relatively
+                                        revisions_from = utils.get_x_months_ago_date(1), # beginning of last month, you can use instead datetime.now() + dateutil.relativedelta.relativedelta() to customize past datetime relatively
                                         revisions_to=datetime.now(),
                                         save_each_page= True,
                                         lang="de"
                                         )
 count, destination_folder = wikirevs.download()
 
 ```
@@ -141,7 +141,8 @@
 # Loop over all wiki page revisions with this period and read each wiki page revs as a pandas dataframe
 for page_path in glob(files):
     page_revs_df = pd.read_parquet(page_name)
     # dataframe with columns ['page', 'lang', 'timestamp', 'categories', 'content', 'images', 'links', 'sections', 'urls', 'user']
     # process/use file ....
 
 ```
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wikipedia_tools Version: 2.2.1 Summary: This is a
+Metadata-Version: 2.1 Name: wikipedia_tools Version: 2.2.2 Summary: This is a
 Wikipedia Tool to fetch revisions based on a period of time. Keywords:
 wikipedia,wikipedia revisions,wikipedia stats Author-email: Roxanne El Baff
 elbaff@dlr.de> Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Requires-Dist: pandas>=1.0.1 Requires-Dist: matplotlib>=3.2.1 Requires-Dist:
 pymediawiki==0.7.2 Requires-Dist: IPy>=1.01 Requires-Dist: seaborn>=0.11.2
 Requires-Dist: nlpaf>1.0.0; python_version <= "3.8" Requires-Dist: tqdm==4.43.0
 Requires-Dist: dataclasses==0.6 Requires-Dist: beautifulsoup4 Requires-Dist:
@@ -45,18 +45,18 @@
 ( categories = ["Climate_change"], revisions_from = utils.get_x_months_ago_date
 (8), revisions_to=datetime.now(), save_each_page= True ) count,
 destination_folder = wikirevs.download() ``` For german wiki revisions, you can
 set the *lang* attribute to *de* - For example, you can download the German
 Wikipedia page revisions for the Climate_change category, as follows: ```python
 from wikipedia_tools.scraper import downloader from datetime import datetime
 wikirevs= downloader.WikiPagesRevision( categories = ["KlimaverÃ¤nderung"],
-revisions_from = utils.get_x_months_ago_date(1), # beguinning of last month,
-you ca use datetime.now() + dateutil.relativedelta.relativedelta to customized
-past datetime relatively revisions_to=datetime.now(), save_each_page= True,
-lang="de" ) count, destination_folder = wikirevs.download() ``` You can then
-process each file by, for example, reading the parquet file using pandas:
+revisions_from = utils.get_x_months_ago_date(1), # beginning of last month, you
+can use instead datetime.now() + dateutil.relativedelta.relativedelta() to
+customize past datetime relatively revisions_to=datetime.now(), save_each_page=
+True, lang="de" ) count, destination_folder = wikirevs.download() ``` You can
+then process each file by, for example, reading the parquet file using pandas:
 ```python import pandas as pd from glob import glob files = f"
 {destination_folder}/*.parquet" # Loop over all wiki page revisions with this
 period and read each wiki page revs as a pandas dataframe for page_path in glob
 (files): page_revs_df = pd.read_parquet(page_name) # dataframe with columns
 ['page', 'lang', 'timestamp', 'categories', 'content', 'images', 'links',
 'sections', 'urls', 'user'] # process/use file .... ```
```

