# Comparing `tmp/newspaper_scraper-0.1.3.tar.gz` & `tmp/newspaper_scraper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newspaper_scraper-0.1.3.tar", last modified: Sat Apr  8 17:20:46 2023, max compression
+gzip compressed data, was "newspaper_scraper-0.2.0.tar", last modified: Fri Apr 28 18:00:45 2023, max compression
```

## Comparing `newspaper_scraper-0.1.3.tar` & `newspaper_scraper-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-08 17:20:46.927337 newspaper_scraper-0.1.3/
--rw-r--r--   0 lukas      (501) staff       (20)     4046 2023-04-08 17:20:46.928104 newspaper_scraper-0.1.3/PKG-INFO
--rw-r--r--   0 lukas      (501) staff       (20)     3442 2023-04-08 16:41:35.000000 newspaper_scraper-0.1.3/README.md
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-08 17:20:46.918433 newspaper_scraper-0.1.3/newspaper_scraper/
--rw-r--r--   0 lukas      (501) staff       (20)      261 2023-04-08 17:18:30.000000 newspaper_scraper-0.1.3/newspaper_scraper/__init__.py
--rw-r--r--   0 lukas      (501) staff       (20)     9362 2023-04-08 16:19:39.000000 newspaper_scraper-0.1.3/newspaper_scraper/database.py
--rw-r--r--   0 lukas      (501) staff       (20)    15828 2023-04-08 17:07:32.000000 newspaper_scraper-0.1.3/newspaper_scraper/scraper.py
--rw-r--r--   0 lukas      (501) staff       (20)     1359 2023-04-08 00:32:47.000000 newspaper_scraper-0.1.3/newspaper_scraper/settings.py
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-08 17:20:46.923710 newspaper_scraper-0.1.3/newspaper_scraper/sites/
--rw-r--r--   0 lukas      (501) staff       (20)        0 2023-03-02 19:40:23.000000 newspaper_scraper-0.1.3/newspaper_scraper/sites/__init__.py
--rw-r--r--   0 lukas      (501) staff       (20)     5580 2023-04-07 19:23:07.000000 newspaper_scraper-0.1.3/newspaper_scraper/sites/bild.py
--rw-r--r--   0 lukas      (501) staff       (20)     6877 2023-04-08 16:04:01.000000 newspaper_scraper-0.1.3/newspaper_scraper/sites/spiegel.py
--rw-r--r--   0 lukas      (501) staff       (20)     6397 2023-04-08 17:16:18.000000 newspaper_scraper-0.1.3/newspaper_scraper/sites/welt.py
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-08 17:20:46.924924 newspaper_scraper-0.1.3/newspaper_scraper/utils/
--rw-r--r--   0 lukas      (501) staff       (20)        0 2023-03-02 19:40:25.000000 newspaper_scraper-0.1.3/newspaper_scraper/utils/__init__.py
--rw-r--r--   0 lukas      (501) staff       (20)     1423 2023-04-07 19:51:55.000000 newspaper_scraper-0.1.3/newspaper_scraper/utils/logger.py
--rw-r--r--   0 lukas      (501) staff       (20)     3534 2023-04-08 00:59:24.000000 newspaper_scraper-0.1.3/newspaper_scraper/utils/utils.py
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-08 17:20:46.922130 newspaper_scraper-0.1.3/newspaper_scraper.egg-info/
--rw-r--r--   0 lukas      (501) staff       (20)     4046 2023-04-08 17:20:46.000000 newspaper_scraper-0.1.3/newspaper_scraper.egg-info/PKG-INFO
--rw-r--r--   0 lukas      (501) staff       (20)      595 2023-04-08 17:20:46.000000 newspaper_scraper-0.1.3/newspaper_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 lukas      (501) staff       (20)        1 2023-04-08 17:20:46.000000 newspaper_scraper-0.1.3/newspaper_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 lukas      (501) staff       (20)       64 2023-04-08 17:20:46.000000 newspaper_scraper-0.1.3/newspaper_scraper.egg-info/requires.txt
--rw-r--r--   0 lukas      (501) staff       (20)       18 2023-04-08 17:20:46.000000 newspaper_scraper-0.1.3/newspaper_scraper.egg-info/top_level.txt
--rw-r--r--   0 lukas      (501) staff       (20)      924 2023-04-08 17:18:30.000000 newspaper_scraper-0.1.3/pyproject.toml
--rw-r--r--   0 lukas      (501) staff       (20)      101 2023-04-08 17:20:46.928617 newspaper_scraper-0.1.3/setup.cfg
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-28 18:00:45.219705 newspaper_scraper-0.2.0/
+-rw-r--r--   0 lukas      (501) staff       (20)     1069 2023-04-13 03:30:30.000000 newspaper_scraper-0.2.0/LICENSE
+-rw-r--r--   0 lukas      (501) staff       (20)     5697 2023-04-28 18:00:45.219799 newspaper_scraper-0.2.0/PKG-INFO
+-rw-r--r--   0 lukas      (501) staff       (20)     3824 2023-04-28 17:51:35.000000 newspaper_scraper-0.2.0/README.md
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-28 18:00:45.215572 newspaper_scraper-0.2.0/newspaper_scraper/
+-rw-r--r--   0 lukas      (501) staff       (20)      414 2023-04-28 17:52:31.000000 newspaper_scraper-0.2.0/newspaper_scraper/__init__.py
+-rw-r--r--   0 lukas      (501) staff       (20)      296 2023-04-11 02:03:26.000000 newspaper_scraper-0.2.0/newspaper_scraper/constants.py
+-rw-r--r--   0 lukas      (501) staff       (20)     9516 2023-04-28 14:58:08.000000 newspaper_scraper-0.2.0/newspaper_scraper/database.py
+-rw-r--r--   0 lukas      (501) staff       (20)    20975 2023-04-28 14:48:37.000000 newspaper_scraper-0.2.0/newspaper_scraper/scraper.py
+-rw-r--r--   0 lukas      (501) staff       (20)     1359 2023-04-08 00:32:47.000000 newspaper_scraper-0.2.0/newspaper_scraper/settings.py
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-28 18:00:45.218326 newspaper_scraper-0.2.0/newspaper_scraper/sites/
+-rw-r--r--   0 lukas      (501) staff       (20)        0 2023-03-02 19:40:23.000000 newspaper_scraper-0.2.0/newspaper_scraper/sites/__init__.py
+-rw-r--r--   0 lukas      (501) staff       (20)     5578 2023-04-28 02:09:25.000000 newspaper_scraper-0.2.0/newspaper_scraper/sites/bild.py
+-rw-r--r--   0 lukas      (501) staff       (20)     5660 2023-04-28 16:56:27.000000 newspaper_scraper-0.2.0/newspaper_scraper/sites/handelsblatt.py
+-rw-r--r--   0 lukas      (501) staff       (20)     6875 2023-04-28 02:09:25.000000 newspaper_scraper-0.2.0/newspaper_scraper/sites/spiegel.py
+-rw-r--r--   0 lukas      (501) staff       (20)     6949 2023-04-28 13:46:32.000000 newspaper_scraper-0.2.0/newspaper_scraper/sites/sz.py
+-rw-r--r--   0 lukas      (501) staff       (20)     6098 2023-04-28 02:09:25.000000 newspaper_scraper-0.2.0/newspaper_scraper/sites/welt.py
+-rw-r--r--   0 lukas      (501) staff       (20)     6238 2023-04-28 15:03:43.000000 newspaper_scraper-0.2.0/newspaper_scraper/sites/zeit.py
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-28 18:00:45.219337 newspaper_scraper-0.2.0/newspaper_scraper/utils/
+-rw-r--r--   0 lukas      (501) staff       (20)        0 2023-03-02 19:40:25.000000 newspaper_scraper-0.2.0/newspaper_scraper/utils/__init__.py
+-rw-r--r--   0 lukas      (501) staff       (20)     1423 2023-04-07 19:51:55.000000 newspaper_scraper-0.2.0/newspaper_scraper/utils/logger.py
+-rw-r--r--   0 lukas      (501) staff       (20)     3534 2023-04-11 02:04:40.000000 newspaper_scraper-0.2.0/newspaper_scraper/utils/utils.py
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-28 18:00:45.216400 newspaper_scraper-0.2.0/newspaper_scraper.egg-info/
+-rw-r--r--   0 lukas      (501) staff       (20)     5697 2023-04-28 18:00:45.000000 newspaper_scraper-0.2.0/newspaper_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 lukas      (501) staff       (20)      736 2023-04-28 18:00:45.000000 newspaper_scraper-0.2.0/newspaper_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 lukas      (501) staff       (20)        1 2023-04-28 18:00:45.000000 newspaper_scraper-0.2.0/newspaper_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 lukas      (501) staff       (20)       64 2023-04-28 18:00:45.000000 newspaper_scraper-0.2.0/newspaper_scraper.egg-info/requires.txt
+-rw-r--r--   0 lukas      (501) staff       (20)       18 2023-04-28 18:00:45.000000 newspaper_scraper-0.2.0/newspaper_scraper.egg-info/top_level.txt
+-rw-r--r--   0 lukas      (501) staff       (20)      924 2023-04-28 17:52:31.000000 newspaper_scraper-0.2.0/pyproject.toml
+-rw-r--r--   0 lukas      (501) staff       (20)      101 2023-04-28 18:00:45.220045 newspaper_scraper-0.2.0/setup.cfg
```

### Comparing `newspaper_scraper-0.1.3/PKG-INFO` & `newspaper_scraper-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: newspaper_scraper
-Version: 0.1.3
-Summary: The all-in-one Python package for seamless newspaper article indexing, scraping, and processing – supports public and premium content!
-Author-email: Lukas Trippe <lkstrp@pm.me>
-Project-URL: Homepage, https://github.com/lkstrp/newspaper-scraper
-Keywords: newspaper,article,scraper,index,process,nlp,wrapper
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: nlp
-
 # Newspaper-Scraper  
   
 ##### The all-in-one Python package for seamless newspaper article indexing, scraping, and processing – supports public and premium content!
   
 ## Intro  
 While tools like [newspaper3k](https://newspaper.readthedocs.io/en/latest/) and [goose3](https://github.com/goose3/goose3) can be used for extracting articles from news websites, they need a dedicated article url for older articles and do not support paywall content. This package aims to solve these issues by providing a unified interface for indexing, extracting and processing articles from newspapers.  
 1. Indexing: Index articles from a newspaper website using the [beautifulsoup](https://beautiful-soup-4.readthedocs.io/en/latest/) package for public articles and [selenium](https://selenium-python.readthedocs.io/) for paywall content.  
@@ -26,16 +12,17 @@
   
 ### Supported Newspapers  
 | Logo | Newspaper | Country | Time span | Number of articles |  
 | ----------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------- | ------- | --------- | --------------- |  
 | <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Der_Spiegel_2022_logo.svg/640px-Der_Spiegel_2022_logo.svg.png" height="70"> | [Der Spiegel](https://www.spiegel.de/) | Germany | Since 2000 | tbd |  
 | <img src="https://upload.wikimedia.org/wikipedia/commons/0/0a/Die_Welt_Logo_2015.png" height="70"> | [Die Welt](https://www.welt.de/) | Germany | Since 2000 | tbd  
 | <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e3/Logo_BILD.svg/1920px-Logo_BILD.svg.png" height="70"> | [Bild](https://www.bild.de/) | Germany | Since 2006 | tbd |  
-  
-  
+| <img src="https://upload.wikimedia.org/wikipedia/commons/6/60/Die_Zeit-Logo-Bremen.svg" height="70"> | [Die Zeit](https://www.zeit.de/) | Germany | Since 1946 | tbd |   
+| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/ff/Handelsblatt_201x_logo.svg/2880px-Handelsblatt_201x_logo.svg.png" height="70"> | [Handelsblatt](https://www.handelsblatt.com/) | Germany | Since 2003 | tbd |  
+
 ## Setup  
 It is recommended to install the package in an dedicated Python environment.  
 To install the package via pip, run the following command:  
   
 ```bash  
 pip install newspaper-scraper
 ```  
@@ -44,23 +31,23 @@
   
 ```bash  
 pip install newspaper-scraper[nlp]
 ```  
   
 ## Usage  
 To index, extract and process all public and premium articles from [Der Spiegel](https://www.spiegel.de/), published in August 2021, run the following code:  
-
+  
 ```python  
 import newspaper_scraper as ns  
 from credentials import username, password  
   
-with ns.Spiegel(db_file='articles.db') as spiegel:  
-spiegel.index_published_articles('2021-08-01', '2021-08-31')  
-spiegel.scrape_public_articles()  
-spiegel.scrape_premium_articles(username=username, password=password)  
-spiegel.nlp()  
+with ns.Spiegel(db_file='articles.db') as news:
+news.index_articles_by_date_range('2021-08-01', '2021-08-31')  
+news.scrape_public_articles()
+news.scrape_premium_articles(username=username, password=password)  
+news.nlp()
 ```  
   
 This will create a sqlite database file called `articles.db` in the current working directory. The database contains the following tables:  
 - `tblArticlesIndexed`: Contains all indexed articles with their scraping/ processing status and whether they are public or premium content.  
 - `tblArticlesScraped`: Contains metadata for all parsed articles, provided by goose3.  
 - `tblArticlesProcessed`: Contains nlp features of the cleaned article text, provided by spaCy.
```

### Comparing `newspaper_scraper-0.1.3/newspaper_scraper/database.py` & `newspaper_scraper-0.2.0/newspaper_scraper/database.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """
 This module contains the database class. It is used to store the scraped articles in a SQLite database.
 """
 
 import datetime as dt
-import json
+import pickle
 
 import pandas as pd
+import numpy as np
 import sqlite3
 
 from .utils.logger import log
-from .utils.utils import delay_interrupt
 from .settings import settings
+from .constants import COLUMN_SQL_TYPES
+from .utils.utils import delay_interrupt
 
 # SQL Settings
 sqlite3.lowercase = False
-# Register json converter to save lists in sqlite
-sqlite3.register_adapter(list, lambda lst: json.dumps(lst).encode('utf8'))
-sqlite3.register_converter("json", lambda lst: json.loads(lst.decode('utf8')))
+
+sqlite3.register_adapter(np.ndarray, pickle.dumps)
+sqlite3.register_converter("BLOP", pickle.loads)
 
 
 class Database:
     """
     This class is used to store the scraped articles in a SQLite database.
     """
 
@@ -30,48 +32,41 @@
         self._df_scraped = None  # Only helper for property self.df_scraped
         self._df_processed = None  # Only helper for property self.df_processed
 
         # Is defined in self.connect()
         self._cur = None
         self._conn = None
         self.df_indexed = None
-        self.df_scraped_cols = None
         self.df_scraped_new = None
-        self.df_processed_cols = None
         self.df_processed_new = None
 
         self._last_save = {'df_indexed': dt.datetime.now(),
                            'df_scraped': dt.datetime.now(),
                            'df_processed': dt.datetime.now()}
 
     @delay_interrupt
     def connect(self):
         """
         Connect to the database and load the articles table. If the database does not exist, it will be created.
         """
-        self._conn = sqlite3.connect(self.db_file)
+        self._conn = sqlite3.connect(self.db_file, detect_types=sqlite3.PARSE_DECLTYPES)
         self._cur = self._conn.cursor()
+        self._create_not_existing_tables()
         self.df_indexed = self._load_table('tblArticlesIndexed')
 
-        # For df_scraped table
-        try:
-            self.df_scraped_cols = pd.read_sql_query("select * from tblArticlesScraped where URL='x'",
-                                                     self._conn).columns.tolist()
-        except pd.errors.DatabaseError:
-            self.df_scraped_cols = []
         # Create dataframe for new scraped articles (will be appended to the database, contains only new articles)
-        self.df_scraped_new = pd.DataFrame(columns=self.df_scraped_cols)
-        self.df_scraped_new = self.df_scraped_new.drop('URL', axis=1, errors='ignore')
-        self.df_scraped_new.index.name = 'URL'
-
-        # For df_processed table
-        self.df_processed_cols = ['DateProcessed', 'lemmatized', 'stop_words', 'pos_tags', 'tags', 'deps', 'shapes']
-        self.df_processed_new = pd.DataFrame(columns=self.df_processed_cols)
-        self.df_processed_new = self.df_processed_new.drop('URL', axis=1, errors='ignore')
-        self.df_processed_new.index.name = 'URL'
+        self.df_scraped_new = pd.read_sql_query(f"SELECT * FROM tblArticlesScraped LIMIT 0",
+                                                self._conn,
+                                                index_col='URL',
+                                                parse_dates=['DateScraped'])
+
+        self.df_processed_new = pd.read_sql_query(f"SELECT * FROM tblArticlesProcessed LIMIT 0",
+                                                  self._conn,
+                                                  index_col='URL',
+                                                  parse_dates=['DateProcessed'])
 
     @delay_interrupt
     def close(self):
         """
         Close the database connection and save the articles DataFrame.
         """
         self.save_data('df_indexed', mode='replace', force=True)
@@ -97,129 +92,138 @@
         Return the processed articles DataFrame. If it is not loaded yet, it will be loaded from the database. This may
         take a while.
         """
         if self._df_processed is None:
             self._df_processed = self._load_table('tblArticlesProcessed')
         return self._df_processed
 
+    def _create_not_existing_tables(self):
+        # Create tblArticlesIndexed
+        self._conn.execute("""
+                    CREATE TABLE IF NOT EXISTS tblArticlesIndexed (
+                        URL TEXT PRIMARY KEY,
+                        DateIndexed TIMESTAMP,
+                        NewspaperID TEXT,
+                        PubDateIndexPage TIMESTAMP,
+                        Edition TEXT,
+                        Public INTEGER,
+                        Scraped INTEGER,
+                        Processed INTEGER
+                    )
+                """)
+        # Create tblArticlesScraped
+        self._conn.execute("""
+                    CREATE TABLE IF NOT EXISTS tblArticlesScraped (
+                        URL TEXT PRIMARY KEY,
+                        DateScraped TIMESTAMP
+                    )
+                """)
+        # Create tblArticlesProcessed
+        self._conn.execute("""
+            CREATE TABLE IF NOT EXISTS tblArticlesProcessed (
+                URL TEXT PRIMARY KEY,
+                DateProcessed TIMESTAMP
+            )
+        """)
+
     def _load_table(self, table_name):
         if table_name == 'tblArticlesIndexed':
             log.info(f'Load database from {self.db_file}.')
 
-            try:
-                _df = pd.read_sql_query(f"SELECT * FROM tblArticlesIndexed",
-                                        self._conn,
-                                        index_col='URL',
-                                        parse_dates=['PubDateIndexPage', 'DateIndexed'])
-
-                try:
-                    already_parsed = pd.read_sql_query("SELECT URL FROM tblArticlesScraped", self._conn)
-                    _df['Scraped'] = _df.index.isin(already_parsed['URL'])
-                except pd.errors.DatabaseError:
-                    _df['Scraped'] = False
-
-                try:
-                    already_processed = pd.read_sql_query("SELECT URL FROM tblArticlesProcessed", self._conn)
-                    _df['Processed'] = _df.index.isin(already_processed['URL'])
-                except pd.errors.DatabaseError:
-                    _df['Processed'] = False
-
-                # Handle boolean values
-                _df.Scraped = _df.Scraped.apply(lambda x: True if x == '1' or x == 1 else x)
-                _df.Scraped = _df.Scraped.apply(lambda x: True if x == '1' or x == 1 else x)
-                _df.Public = _df.Public.apply(lambda x: True if x == '1' or x == 1 else x)
-                _df.Public = _df.Public.apply(lambda x: False if x == '0' or x == 0 else x)
-
-                if _df.empty:
-                    percent_scraped = 0
-                    percent_processed = 0
-                else:
-                    percent_scraped = len(_df[_df.Scraped]) / len(_df) * 100
-                    percent_processed = len(_df[_df.Processed]) / len(_df) * 100
-
-                log.info(f'Loaded {len(_df):,} articles from database. '
-                         f'{percent_scraped:.1f}% scraped and '
-                         f'{percent_processed:.1f}% processed.')
-            except pd.errors.DatabaseError:
-                _df = pd.DataFrame(columns=['NewspaperID', 'PubDateIndexPage', 'DateIndexed', 'Public', 'Scraped',
-                                            'Processed'])
-                _df.index.name = 'URL'
-                log.info(f'No database found. Created new database.')
+            _df = pd.read_sql_query(f"SELECT * FROM tblArticlesIndexed",
+                                    self._conn,
+                                    index_col='URL',
+                                    parse_dates=['DateIndexed', 'PubDateIndexPage'])
+
+            already_parsed = pd.read_sql_query("SELECT URL FROM tblArticlesScraped", self._conn)
+            _df['Scraped'] = _df.index.isin(already_parsed['URL'])
+
+            already_processed = pd.read_sql_query("SELECT URL FROM tblArticlesProcessed", self._conn)
+            _df['Processed'] = _df.index.isin(already_processed['URL'])
+
+            # Handle boolean values
+            _df.Public = _df.Public.apply(lambda x: True if x == '1' or x == 1 else x)
+            _df.Public = _df.Public.apply(lambda x: False if x == '0' or x == 0 else x)
+            _df.Scraped = _df.Scraped.apply(lambda x: True if x == '1' or x == 1 else x)
+            _df.Scraped = _df.Scraped.apply(lambda x: True if x == '1' or x == 1 else x)
+            _df.Processed = _df.Processed.apply(lambda x: True if x == '1' or x == 1 else x)
+            _df.Processed = _df.Processed.apply(lambda x: False if x == '0' or x == 0 else x)
+
+            if _df.empty:
+                percent_scraped = 0
+                percent_processed = 0
+            else:
+                percent_scraped = len(_df[_df.Scraped]) / len(_df) * 100
+                percent_processed = len(_df[_df.Processed]) / len(_df) * 100
+
+            log.info(f'Loaded {len(_df):,} articles from database. '
+                     f'{percent_scraped:.1f}% scraped and '
+                     f'{percent_processed:.1f}% processed.')
 
             _df = _df.convert_dtypes()
 
         elif table_name == 'tblArticlesScraped':
             _df = pd.read_sql_query(f"SELECT * FROM tblArticlesScraped",
                                     self._conn,
                                     index_col='URL',
-                                    parse_dates=['DateScrapedHTML'])
-            _df = _df.rename({'CleanedText': 'Text'}, axis=1, errors='ignore')
+                                    parse_dates=['DateScraped'])
 
         elif table_name == 'tblArticlesProcessed':
             _df = pd.read_sql_query(f"SELECT * FROM tblArticlesProcessed",
                                     self._conn,
-                                    index_col='URL')
+                                    index_col='URL',
+                                    parse_dates=['DateProcessed'])
 
         else:
             raise ValueError(f'Table {table_name} not recognized.')
+
         return _df
 
     @delay_interrupt
     def save_data(self, data_name: str, mode: str, force: bool = False):
         """
         Save the articles DataFrame to the database. This method has a built-in delay to prevent saving the database
         too often. The delay is set in the settings file.
         """
         if mode not in ['append', 'replace']:
             raise ValueError(f'Mode {mode} not recognized. Mode must be "append" or "replace".')
 
-        # Check if the save interval has passed otherwise skip saving
-        if self._last_save[data_name] + dt.timedelta(seconds=settings.save_interval) > dt.datetime.now() \
-                and not force:
+        # Check if the save interval has passed, otherwise skip saving
+        if not force and self._last_save[data_name] + dt.timedelta(seconds=settings.save_interval) > dt.datetime.now():
             return
-        else:
-            self._last_save[data_name] = dt.datetime.now()
+
+        self._last_save[data_name] = dt.datetime.now()
 
         if data_name == 'df_indexed':
             _df = self.df_indexed.copy()
-
-            # Convert dates to strings
-            _df.PubDateIndexPage = _df.PubDateIndexPage.apply(str)
-
-            _df.to_sql('tblArticlesIndexed', self._conn, index_label='URL', if_exists=mode)
+            assert self.df_indexed.index.is_unique, 'Index of df_indexed is not unique.'
 
         elif data_name == 'df_scraped':
-            if mode == 'append':
-                _df = self.df_scraped_new.copy()
-                self.df_scraped_new = self.df_scraped_new.head(0)
-            else:
-                _df = self.df_scraped.copy()
-
-            if _df.empty:
-                return
-            try:
-                _df.to_sql('tblArticlesScraped', self._conn, index_label='URL', if_exists=mode)
-            except sqlite3.OperationalError:
-                # Add the missing column, if new columns were added to the DataFrame and are not in the database yet
-                self._cur.execute("PRAGMA table_info(tblArticlesScraped)")
-                columns_info = self._cur.fetchall()
-                for col in _df.columns:
-                    column_exists = any(column_info[1] == col for column_info in columns_info)
-                    if not column_exists:
-                        self._cur.execute("ALTER TABLE tblArticlesScraped ADD COLUMN '{}' TEXT".format(col))
-
-                _df.to_sql('tblArticlesScraped', self._conn, index_label='URL', if_exists=mode)
+            _df = self.df_scraped_new.copy() if mode == 'append' else self.df_scraped.copy()
+            self.df_scraped_new = self.df_scraped_new.head(0) if mode == 'append' else self.df_scraped_new
 
         elif data_name == 'df_processed':
-            if mode == 'append':
-                _df = self.df_processed_new.copy()
-                self.df_processed_new = self.df_processed_new.head(0)
-            else:
-                _df = self.df_processed.copy()
-
-            if _df.empty:
-                return
-
-            _df.to_sql('tblArticlesProcessed', self._conn, index_label='URL', if_exists=mode)
+            _df = self.df_processed_new.copy() if mode == 'append' else self.df_processed.copy()
+            self.df_processed_new = self.df_processed_new.head(0) if mode == 'append' else self.df_processed_new
 
         else:
             raise ValueError(f'Data {data_name} not recognized.')
+
+        if _df.empty:
+            return
+
+        table_name = {'df_indexed': 'tblArticlesIndexed',
+                      'df_scraped': 'tblArticlesScraped',
+                      'df_processed': 'tblArticlesProcessed'}[data_name]
+
+        try:
+            _df.to_sql(table_name, self._conn, index_label='URL', if_exists=mode)
+        except sqlite3.OperationalError:
+            # Add the missing column, if new columns were added to the DataFrame and are not in the database yet
+            self._cur.execute(f"PRAGMA table_info({table_name})")
+            columns_info = self._cur.fetchall()
+            for col in _df.columns:
+                column_exists = any(column_info[1] == col for column_info in columns_info)
+                if not column_exists:
+                    column_type = COLUMN_SQL_TYPES[col] if col in COLUMN_SQL_TYPES else 'TEXT'
+                    self._cur.execute(f"ALTER TABLE {table_name} ADD COLUMN '{col}' {column_type}")
+            _df.to_sql(table_name, self._conn, index_label='URL', if_exists=mode)
```

### Comparing `newspaper_scraper-0.1.3/newspaper_scraper/scraper.py` & `newspaper_scraper-0.2.0/newspaper_scraper/scraper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """
 This module contains the NewspaperManager class which is used to scrape articles from a newspaper website. It is only
 used as a base class for the actual scrapers.
 """
 
 import re
 import datetime as dt
-import sys
 
 import numpy as np
 import pandas as pd
 from goose3 import Goose
 from tqdm.auto import tqdm
 from tqdm.contrib.logging import logging_redirect_tqdm
 
 try:
     import spacy
 except ImportError:
     spacy = None
 
 from .utils.logger import log
 from .settings import settings
+from .constants import NLP_ATTRIBUTES
 from .utils.utils import flatten_dict
 from .utils.utils import get_selenium_webdriver
 from .utils.utils import retry_on_exception
 from .database import Database
 
 
 class NewspaperManager:
@@ -39,17 +39,18 @@
         - _parse_article: Parses the HTML of an article and returns a DataFrame with the parsed infos.
         - _get_published_articles: Not implemented. Needs to be implemented in the actual scraper.
         - _soup_get_html: Not implemented. Needs to be implemented in the actual scraper.
         - _selenium_login: Not implemented. Needs to be implemented in the actual scraper.
     """
 
     def __init__(self, db_file):
-        self._db = Database(db_file=db_file)
-
         self.newspaper_id = re.sub(r'(?<!^)(?=[A-Z])', '_', self.__class__.__name__).lower()
+        log.info(f'Initializing {self.newspaper_id} scraper.')
+
+        self._db = Database(db_file=db_file)
         self._selenium_driver = None
         self._spacy_nlp = None
 
     @property
     def selenium_driver(self):
         """
         Returns the selenium driver. If no driver is set, it tries to get one from the settings file. If this fails, it
@@ -119,15 +120,15 @@
         # Rename CleanedText to Text
         parsed_infos = parsed_infos.rename({'CleanedText': 'Text'}, axis=1)
         parsed_infos.index.name = 'URL'
 
         return parsed_infos
 
     @retry_on_exception
-    def index_published_articles(self, date_from, date_to, skip_existing=True):
+    def index_articles_by_date_range(self, date_from, date_to, skip_existing=True):
         """
         Indexes all articles published between date_from and date_to for a given newspaper. Indexing means that the
         articles are added to the database and their URLs are stored. The actual scraping of the articles is done
         separately with the scrape_public_articles and scrape_premium_articles methods.
 
         Args:
             date_from (dt.datetime or str): The first day to scrape articles from.
@@ -151,53 +152,137 @@
             date_range = date_range.tolist()
 
         if len(date_range) == 0:
             log.info(f'No new days to scrape. Pass skip_existing=False to scrape all days again.')
             return
 
         log.info(f'Start scraping articles for {len(date_range):,} days ({date_from.strftime("%d.%m.%y")} - '
-                 f'{date_to.strftime("%d.%m.%y")}). {len(pd.date_range(date_from, date_to)) - len(date_range)} '
+                 f'{date_to.strftime("%d.%m.%y")}). {len(pd.date_range(date_from, date_to)) - len(date_range):,} '
                  f'days already indexed.')
         counter = 0
         with logging_redirect_tqdm(loggers=[log]):
             for day in tqdm(date_range):
                 counter += 1
 
-                urls, pub_dates = self._get_published_articles(day)
+                urls, pub_dates = self._get_articles_by_date(day)
 
                 assert all([isinstance(pub_date, dt.datetime) for pub_date in pub_dates]), \
                     f'Not all pub_dates are datetime objects.'
                 assert all([pub_date.tzinfo is not None for pub_date in pub_dates]), \
                     f'Not all pub_dates contain timezone info.'
 
+                # Convert pub_dates to UTC
+                pub_dates = [pub_date.astimezone(dt.timezone.utc) for pub_date in pub_dates]
+                # Remove timezone info from pub_dates
+                pub_dates = [pub_date.replace(tzinfo=None) for pub_date in pub_dates]
+
                 # Remove query strings from urls
                 urls = [url.split('?')[0] for url in urls]
 
-                assert all([isinstance(pub_date, dt.datetime) for pub_date in pub_dates]), \
-                    f'Not all pub_dates are datetime objects.'
-
                 urls = pd.DataFrame({'NewspaperID': self.newspaper_id,
                                      'PubDateIndexPage': pub_dates,
                                      'DateIndexed': dt.datetime.now(),
                                      'Public': None,
                                      'Scraped': False,
                                      'Processed': False},
                                     index=urls)
                 # Mark if urls are new
-                urls['new'] = ~urls.index.isin(self._db.df_indexed.index)
-                urls['new'] = urls['new'].astype(bool)
+                urls['new'] = ~urls.index.isin(self._db.df_indexed.index).astype(bool)
 
                 # Add new urls to articles table
                 self._db.df_indexed = pd.concat([self._db.df_indexed, urls[urls['new']].drop('new', axis=1)])
                 log.info(f'{counter}/{len(date_range)}: Indexed {urls.new.sum()}/{len(urls)} articles '
                          f'for {day.strftime("%d.%m.%Y")} (n={len(self._db.df_indexed):,}).')
 
                 self._db.save_data('df_indexed', mode='replace')
 
     @retry_on_exception
+    def index_articles_by_edition(self, edition_from: str, edition_to: str, editions_per_year=55, skip_existing=True):
+        """
+        Index all articles published in between two editions for a given newspaper. Indexing means that the
+        articles are added to the database and their URLs are stored. The actual scraping of the articles is done
+        separately with the scrape_public_articles and scrape_premium_articles methods.
+
+        Args:
+            edition_from (str): The first edition to scrape articles from. The format must be 'YYYY-EDITION'
+                (e.g. '2019-1').
+            edition_to (str): The last edition to scrape articles from. The format must be 'YYYY-EDITION'
+                (e.g. '2019-1').
+            editions_per_year (int, optional): The number of editions per year. Defaults to 55. If edtions across
+                multiple years are scraped, this number is used for all years in between.
+            skip_existing (bool, optional): If True, days that are already indexed are skipped. Defaults to True.
+        """
+        if re.match(r'\d{4}-(?!0)\d{1,2}', edition_from) is None:
+            raise ValueError(f'edition_from must be in the format "YYYY-EDITION" (e.g. "2019-1").')
+        if re.match(r'\d{4}-(?!0)\d{1,2}', edition_to) is None:
+            raise ValueError(f'edition_to must be in the format "YYYY-EDITION" (e.g. "2019-1").')
+
+        year_from = int(edition_from.split('-')[0])
+        year_to = int(edition_to.split('-')[0])
+
+        edition_from = int(edition_from.split('-')[1])
+        edition_to = int(edition_to.split('-')[1])
+
+        edition_range = []
+        for year in range(year_from, year_to + 1):
+            if year == year_from and year == year_to:
+                editions = range(edition_from, edition_to + 1)
+            elif year == year_from:
+                editions = range(edition_from, editions_per_year + 1)
+            elif year == year_to:
+                editions = range(1, edition_to + 1)
+            else:
+                editions = range(1, editions_per_year + 1)
+
+            for edition in editions:
+                edition_range.append(f'{year}-{edition}')
+
+        already_indexed = self._db.df_indexed[(self._db.df_indexed.NewspaperID == self.newspaper_id)]
+        indexed_editions = [edition for edition in already_indexed.Edition.unique().tolist()]
+
+        if skip_existing:
+            edition_range = [edition for edition in edition_range if edition not in indexed_editions]
+
+        if len(edition_range) == 0:
+            log.info(f'No new editions to scrape. Pass skip_existing=False to scrape all days again.')
+            return
+
+        log.info(f'Start scraping articles for {len(edition_range):,} editions ({year_from}-{edition_from} - '
+                 f'{year_to}-{edition_to}).')  # todo add already indexed editions
+
+        counter = 0
+        with logging_redirect_tqdm(loggers=[log]):
+            for edition in tqdm(edition_range, total=len(edition_range)):
+                counter += 1
+                year = int(edition.split('-')[0])
+                edition = int(edition.split('-')[1])
+
+                urls = self._get_articles_by_edition(year, edition)
+
+                # Remove query strings from urls
+                urls = [url.split('?')[0] for url in urls]
+
+                urls = pd.DataFrame({'NewspaperID': self.newspaper_id,
+                                     'Edition': f'{year}-{edition}',
+                                     'DateIndexed': dt.datetime.now(),
+                                     'Public': None,
+                                     'Scraped': False,
+                                     'Processed': False},
+                                    index=urls)
+                # Mark if urls are new
+                urls['new'] = ~urls.index.isin(self._db.df_indexed.index).astype(bool)
+
+                # Add new urls to articles table
+                self._db.df_indexed = pd.concat([self._db.df_indexed, urls[urls['new']].drop('new', axis=1)])
+                log.info(f'{counter}/{len(edition_range)}: Indexed {urls.new.sum()}/{len(urls)} articles '
+                         f'for {year}-{edition} (n={len(self._db.df_indexed):,}).')
+
+                self._db.save_data('df_indexed', mode='replace')
+
+    @retry_on_exception
     def scrape_public_articles(self):
         """
         Checks for all indexed articles if they are publicly available. If they are, the article is scraped and
         the parsed infos are added to the database. If they are not, the article is marked as private. Uses 
         beautifulsoup4 to scrape the articles.
         """
         to_scrape = self._db.df_indexed[(self._db.df_indexed.NewspaperID == self.newspaper_id) &
@@ -216,17 +301,16 @@
                 raw_html, public = self._soup_get_html(url)
 
                 if public:
                     results = self._parse_article(raw_html, url)
 
                     # Notifies if new columns are detected in results
                     for col in results.columns:
-                        if col not in self._db.df_scraped_cols:
-                            self._db.df_scraped_cols.append(col)
-                            # log.info(f'New column detected: {col}')  # todo print can be removed
+                        if col not in self._db.df_scraped_new.columns:
+                            log.info(f'New feature detected: {col}')
 
                     # Add results to articles table
                     self._db.df_scraped_new = pd.concat([self._db.df_scraped_new, results], axis=0)
                     self._db.df_scraped_new.loc[url, 'DateScrapedHTML'] = dt.datetime.now()
                     self._db.df_indexed.at[url, 'Scraped'] = True
 
                     stats.append(1)
@@ -262,30 +346,33 @@
                                         (self._db.df_indexed.Scraped != True)]
 
         # Return if no articles to scrape
         if to_scrape.empty:
             log.info(f'No articles to scrape.')
             return
 
+        # Reset selenium driver
+        if self._selenium_driver is not None:
+            self._selenium_driver.close()
+        self._selenium_driver = None
         # Login
         login_successful = self._selenium_login(username=username, password=password)
         if not login_successful:
             log.warning(f'Login failed. Skip scraping.')
             return
 
         # Scrape articles
         log.info(f'Start scraping {len(to_scrape)} premium articles.')
         counter = 0
         with logging_redirect_tqdm(loggers=[log]):
             for url, row in tqdm(to_scrape.iterrows(), total=len(to_scrape)):
                 counter += 1
 
                 # Scrape article
-                self.selenium_driver.get(url)
-                raw_html = self.selenium_driver.page_source
+                raw_html = self._selenium_get_html(url)
                 results = self._parse_article(raw_html, url)
 
                 # Add results to articles table
                 self._db.df_scraped_new = pd.concat([self._db.df_scraped_new, results], axis=0)
                 self._db.df_scraped_new.loc[url, 'DateScrapedHTML'] = dt.datetime.now()
                 self._db.df_indexed.at[url, 'Scraped'] = True
 
@@ -326,31 +413,48 @@
                 # Save both tables
                 self._db.save_data('df_indexed', mode='replace')
                 self._db.save_data('df_processed', mode='append')
 
     def _process_article(self, text, url):
         doc = self.spacy_nlp(text)
         data = pd.DataFrame(
-            [[[token.lemma_ for token in doc], [token.is_stop for token in doc], [token.pos_ for token in doc],
-              [token.tag_ for token in doc], [token.dep_ for token in doc], [token.shape_ for token in doc]]],
-            columns=['lemmatized', 'stop_words', 'pos_tags', 'tags', 'deps', 'shapes'],
+            [[np.array([token.__getattribute__(attribute) for token in doc]) for attribute in NLP_ATTRIBUTES]],
+            columns=NLP_ATTRIBUTES,
             index=[url]
         )
+        data['left_edge'] = data['left_edge'].apply(lambda x: np.array([token.i for token in x]))
+        data['right_edge'] = data['right_edge'].apply(lambda x: np.array([token.i for token in x]))
+        data['morph'] = data['morph'].apply(lambda x: np.array([token.to_dict() for token in x]))
+
         return data
 
-    def _get_published_articles(self, day):
+    def _get_articles_by_date(self, day):
+        """
+        Exists only as a placeholder. Needs to be implemented by the child class for each newspaper.
+        """
+        raise NotImplemented
+
+    def _get_articles_by_edition(self, year, edition):
         """
         Exists only as a placeholder. Needs to be implemented by the child class for each newspaper.
         """
         raise NotImplemented
 
     def _soup_get_html(self, url):
         """
         Exists only as a placeholder. Needs to be implemented by the child class for each newspaper.
         """
         raise NotImplemented
 
+    def _selenium_get_html(self, url):
+        """
+        Function to get the html of a private article. Uses selenium to get the html. Can be optionally overwritten by
+        the child if a different method is needed.
+        """
+        self.selenium_driver.get(url)
+        return self.selenium_driver.page_source
+
     def _selenium_login(self, username: str, password: str):
         """
         Exists only as a placeholder. Needs to be implemented by the child class for each newspaper.
         """
         raise NotImplemented
```

### Comparing `newspaper_scraper-0.1.3/newspaper_scraper/settings.py` & `newspaper_scraper-0.2.0/newspaper_scraper/settings.py`

 * *Files identical despite different names*

### Comparing `newspaper_scraper-0.1.3/newspaper_scraper/sites/bild.py` & `newspaper_scraper-0.2.0/newspaper_scraper/sites/bild.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         - _selenium_login: Login to the newspaper website to allow scraping of premium content after the login. Uses
             selenium.
     """
 
     def __init__(self, db_file: str = 'articles.db'):
         super().__init__(db_file)
 
-    def _get_published_articles(self, day: dt.date):
+    def _get_articles_by_date(self, day: dt.date):
         """
         Index articles published on a given day and return the urls and publication dates.
 
         Args:
             day (dt.date): Date of the articles to index.
 
         Returns:
```

### Comparing `newspaper_scraper-0.1.3/newspaper_scraper/sites/spiegel.py` & `newspaper_scraper-0.2.0/newspaper_scraper/sites/spiegel.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     def __init__(self, db_file: str = 'articles.db'):
         super().__init__(db_file)
 
         # Set locale to German
         locale.setlocale(locale.LC_TIME, "de_DE")
 
-    def _get_published_articles(self, day: dt.date):
+    def _get_articles_by_date(self, day: dt.date):
         """
         Index articles published on a given day and return the urls and publication dates.
 
         Args:
             day (dt.date): Date of the articles to index.
 
         Returns:
```

### Comparing `newspaper_scraper-0.1.3/newspaper_scraper/sites/welt.py` & `newspaper_scraper-0.2.0/newspaper_scraper/sites/handelsblatt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 """
-This module contains the class to scrape articles from the "Welt" newspaper (https://www.welt.de/).
+This module contains the class to scrape articles from the "Handelsblatt" newspaper (https://www.handelsblatt.com/).
 The class inherits from the NewspaperManager class and needs an implementation of the abstract methods.
 With a similar implementation, it is possible to scrape articles from other news websites.
 """
-import re
 import datetime as dt
-import time
 
 import requests
 from bs4 import BeautifulSoup
-import pandas as pd
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as ec
-from selenium.common.exceptions import NoSuchElementException
+from selenium.common.exceptions import TimeoutException
 
 from ..utils.logger import log
 from ..scraper import NewspaperManager
 
 
-class DeWelt(NewspaperManager):
+class DeHandelsblatt(NewspaperManager):
     """
     This class inherits from the NewspaperManager class and implements the newspaper specific methods.
     These methods are:
         - _get_published_articles: Index articles published on a given day and return the urls and publication dates.
         - _soup_get_html: Determine if an article is premium content and scrape the html if it is not. Uses
             beautifulsoup.
         - _selenium_login: Login to the newspaper website to allow scraping of premium content after the login. Uses
             selenium.
     """
 
     def __init__(self, db_file: str = 'articles.db'):
         super().__init__(db_file)
 
-    def _get_published_articles(self, day: dt.date):
+    def _get_articles_by_date(self, day: dt.date):
         """
         Index articles published on a given day and return the urls and publication dates.
 
         Args:
             day (dt.date): Date of the articles to index.
 
         Returns:
             urls ([str]): List of urls of the articles published on the given day.
             pub_dates ([dt.datetime]): List of publication dates of the articles published on the given day.
               Needs timezone information.
         """
-        URL = f'https://www.welt.de/schlagzeilen/nachrichten-vom-{day.strftime("%-d-%-m-%Y")}.html'
+        URL = f'https://www.handelsblatt.com/archiv/{day.strftime("%Y/%-m/%-d")}'
 
         soup = BeautifulSoup(requests.get(URL).content, "html.parser")
-        articles = soup \
-            .find("div", {"class": "c-tabs__panel-content"}) \
-            .find_all("article", {"class": "c-teaser c-teaser--archive"})
-
-        # Get articles urls
-        urls = ['https://www.welt.de' + article.find('h4').find('a')['href'] for article in articles]
-
-        # Get articles publication dates
-        time_regex = re.compile(r'\d{2}\.\d{2}\.\d{4}\s\|\s\d{2}:\d{2}')
-        pub_dates = [pd.to_datetime(f'{article.find(string=time_regex)}', format='%d.%m.%Y | %H:%M')
-                     for article in articles]
-        # Add timezone Europe/Berlin to pub_dates
-        pub_dates = [pub_date.tz_localize('Europe/Berlin') for pub_date in pub_dates]
+        _articles = soup.find_all("a", {"class": "vhb-teaser-link"})
+        urls = ['https://www.handelsblatt.com' + article['href'] for article in _articles]
+
+        # Also add paginated articles
+        pages_exist = soup.find("div", {"class": "vhb-teaser-pagination"})
+        if pages_exist:
+            page_urls = pages_exist.find("div", {"class": "vhb-tp-list"}).find_all('a')
+            page_urls = ['https://www.handelsblatt.com' + page_url['href'] for page_url in page_urls]
+
+            for page_url in page_urls:
+                soup = BeautifulSoup(requests.get(page_url).content, "html.parser")
+                _articles = soup.find_all("a", {"class": "vhb-teaser-link"})
+                [urls.append('https://www.handelsblatt.com' + article['href']) for article in _articles]
+
+        # Create list of publication dates, since the website does not provide them
+        pub_dates = [dt.datetime.combine(day, dt.datetime.min.time(), tzinfo=dt.timezone.utc)] * len(urls)
 
         assert len(urls) == len(pub_dates), 'Number of urls and pub_dates does not match.'
 
         return urls, pub_dates
 
     def _soup_get_html(self, url: str):
         """
@@ -73,67 +73,51 @@
         Args:
             url (str): Url of the article to scrape.
 
         Returns:
             html (str): Html of the article. If the article is premium content, None is returned.
             is_premium (bool): True if the article is premium content, False otherwise.
         """
-        try:
-            html = requests.get(url).content
-            soup = BeautifulSoup(html, "html.parser")
-            premium_icon = soup.find("header", {"class": "c-content-container"}).\
-                find('a', {"class": "o-dreifaltigkeit__premium-badge"})
-        except AttributeError:
-            log.warning(f'Error scraping {url}.')
-            return None, False
-        return html, not bool(premium_icon)
+        # Handelsblatt uses a login paywall via javascript. Therefore, selenium is needed to login. The following
+        # return indicates that the article is premium content and they are all scraped self.scrape_premium_articles.
+        return None, False
 
     def _selenium_login(self, username: str, password: str):
         """
         Using selenium, login to the newspaper website to allow scraping of premium content after the login. Does three
         things:
-            1. Go to main page and accept cookies.
-            2. Login.
-            3. Check if login was successful.
+            1. Login
+            2. Accept cookies
+            3. Check if login was successful
 
         Args:
             username (str): Username to login to the newspaper website.
             password (str): Password to login to the newspaper website.
 
         Returns:
             bool: True if login was successful, False otherwise.
         """
-        # Go to main page and accept cookies
-        self.selenium_driver.get('https://www.welt.de/')
-        privacy_frame = WebDriverWait(self.selenium_driver, 10).until(
-            ec.presence_of_element_located((By.XPATH, '//iframe[@title="SP Consent Message"]'))
-        )
-        self.selenium_driver.switch_to.frame(privacy_frame)
-        WebDriverWait(self.selenium_driver, 10).until(
-            ec.presence_of_element_located((By.CSS_SELECTOR, 'button[title="Alle akzeptieren"]')))
-        self.selenium_driver.find_element(By.CSS_SELECTOR, 'button[title="Alle akzeptieren"]').click()
-        # Wait and reload page because of ads
-        time.sleep(10)
-        self.selenium_driver.get('https://www.welt.de/')
 
         # Login
-        self.selenium_driver.find_element(By.CSS_SELECTOR, 'button[data-component="LoginButton"]').click()
-        self.selenium_driver.find_element(By.CSS_SELECTOR, 'button[data-qa="PageHeader.Login.Button.Login"]').click()
-        WebDriverWait(self.selenium_driver, 10).until(
-            ec.presence_of_element_located((By.NAME, 'username')))
-        self.selenium_driver.find_element(By.NAME, 'username').send_keys(username)
-        self.selenium_driver.find_element(By.NAME, 'password').send_keys(password)
-        self.selenium_driver.find_element(By.CSS_SELECTOR, 'button[type="submit"]').click()
+        self.selenium_driver.get('https://id.handelsblatt.com/login')
+        self.selenium_driver.find_element(By.XPATH, '//input[@type="email"]').send_keys(username)
+        self.selenium_driver.find_element(By.XPATH, '//input[@type="password"]').send_keys(password)
+        self.selenium_driver.find_element(By.XPATH, '//button[@type="submit"]').click()
+        self.selenium_driver.get('https://www.handelsblatt.com/ ')
+
+        # Accept cookies
+        privacy_frame = WebDriverWait(self.selenium_driver, 10).until(
+            ec.presence_of_element_located((By.XPATH, '//iframe[@title="Iframe title"]')))
+        self.selenium_driver.switch_to.frame(privacy_frame)
+        cookie_accept_button = WebDriverWait(self.selenium_driver, 10).until(
+            ec.element_to_be_clickable((By.XPATH, "//button[contains(text(), 'ZUSTIMMEN')]")))
+        cookie_accept_button.click()
 
         # Check if login was successful
         try:
-            self.selenium_driver.get('https://www.welt.de/meinewelt/')
             WebDriverWait(self.selenium_driver, 10).until(
-                ec.presence_of_element_located((By.CSS_SELECTOR, 'div[data-component-name="home"]')))
-            _elem = self.selenium_driver.find_element(By.CSS_SELECTOR, 'div[data-component-name="home"]')
-            WebDriverWait(_elem, 10).until(ec.presence_of_element_located((By.CSS_SELECTOR, 'div[name="greeting"]')))
-            self.selenium_driver.get('https://www.welt.de')
-            log.info('Logged in to Welt Plus.')
+                ec.presence_of_element_located((By.XPATH, f"//span[contains(text(), '{username}')]")))
+            log.info('Logged in to Handelsblatt.')
             return True
-        except NoSuchElementException:
-            log.warning('Login to Welt Plus failed.')
+        except TimeoutException:
+            log.error('Login to Handelsblatt failed.')
             return False
```

### Comparing `newspaper_scraper-0.1.3/newspaper_scraper/utils/logger.py` & `newspaper_scraper-0.2.0/newspaper_scraper/utils/logger.py`

 * *Files identical despite different names*

### Comparing `newspaper_scraper-0.1.3/newspaper_scraper/utils/utils.py` & `newspaper_scraper-0.2.0/newspaper_scraper/utils/utils.py`

 * *Files identical despite different names*

### Comparing `newspaper_scraper-0.1.3/newspaper_scraper.egg-info/SOURCES.txt` & `newspaper_scraper-0.2.0/newspaper_scraper.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+LICENSE
 README.md
 pyproject.toml
 setup.cfg
 newspaper_scraper/__init__.py
+newspaper_scraper/constants.py
 newspaper_scraper/database.py
 newspaper_scraper/scraper.py
 newspaper_scraper/settings.py
 newspaper_scraper.egg-info/PKG-INFO
 newspaper_scraper.egg-info/SOURCES.txt
 newspaper_scraper.egg-info/dependency_links.txt
 newspaper_scraper.egg-info/requires.txt
 newspaper_scraper.egg-info/top_level.txt
 newspaper_scraper/sites/__init__.py
 newspaper_scraper/sites/bild.py
+newspaper_scraper/sites/handelsblatt.py
 newspaper_scraper/sites/spiegel.py
+newspaper_scraper/sites/sz.py
 newspaper_scraper/sites/welt.py
+newspaper_scraper/sites/zeit.py
 newspaper_scraper/utils/__init__.py
 newspaper_scraper/utils/logger.py
 newspaper_scraper/utils/utils.py
```

### Comparing `newspaper_scraper-0.1.3/pyproject.toml` & `newspaper_scraper-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "newspaper_scraper"
-version = "0.1.3"
+version = "0.2.0"
 description = "The all-in-one Python package for seamless newspaper article indexing, scraping, and processing – supports public and premium content!"
 authors = [{ name = "Lukas Trippe", email = "lkstrp@pm.me" }]
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

