# Comparing `tmp/CobWeb-lnx-1.0.0.tar.gz` & `tmp/CobWeb-lnx-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CobWeb-lnx-1.0.0.tar", last modified: Wed Apr 26 19:24:50 2023, max compression
+gzip compressed data, was "CobWeb-lnx-1.0.1.tar", last modified: Fri Apr 28 13:59:20 2023, max compression
```

## Comparing `CobWeb-lnx-1.0.0.tar` & `CobWeb-lnx-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 19:24:50.449122 CobWeb-lnx-1.0.0/
--rw-rw-rw-   0        0        0     1094 2022-12-08 18:47:01.000000 CobWeb-lnx-1.0.0/LICENSE.md
--rw-rw-rw-   0        0        0     3856 2023-04-26 19:24:50.450131 CobWeb-lnx-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3098 2023-04-26 17:40:51.000000 CobWeb-lnx-1.0.0/README.md
--rw-rw-rw-   0        0        0      770 2023-04-26 19:24:13.000000 CobWeb-lnx-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      303 2023-04-26 19:24:50.455207 CobWeb-lnx-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-26 19:24:50.386256 CobWeb-lnx-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-26 19:24:50.409851 CobWeb-lnx-1.0.0/src/CobWeb/
--rw-rw-rw-   0        0        0       51 2023-04-26 18:02:34.000000 CobWeb-lnx-1.0.0/src/CobWeb/__init__.py
--rw-rw-rw-   0        0        0    11678 2023-04-26 19:22:36.000000 CobWeb-lnx-1.0.0/src/CobWeb/crawler.py
-drwxrwxrwx   0        0        0        0 2023-04-26 19:24:50.447128 CobWeb-lnx-1.0.0/src/CobWeb_lnx.egg-info/
--rw-rw-rw-   0        0        0     3856 2023-04-26 19:24:50.000000 CobWeb-lnx-1.0.0/src/CobWeb_lnx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-04-26 19:24:50.000000 CobWeb-lnx-1.0.0/src/CobWeb_lnx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 19:24:50.000000 CobWeb-lnx-1.0.0/src/CobWeb_lnx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      189 2023-04-26 19:24:50.000000 CobWeb-lnx-1.0.0/src/CobWeb_lnx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-26 19:24:50.000000 CobWeb-lnx-1.0.0/src/CobWeb_lnx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 13:59:20.856341 CobWeb-lnx-1.0.1/
+-rw-rw-rw-   0        0        0     1094 2022-12-08 18:47:01.000000 CobWeb-lnx-1.0.1/LICENSE.md
+-rw-rw-rw-   0        0        0     3856 2023-04-28 13:59:20.856341 CobWeb-lnx-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3098 2023-04-26 17:40:51.000000 CobWeb-lnx-1.0.1/README.md
+-rw-rw-rw-   0        0        0      770 2023-04-28 13:56:49.000000 CobWeb-lnx-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      480 2023-04-28 13:59:20.859342 CobWeb-lnx-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 13:59:20.801546 CobWeb-lnx-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 13:59:20.815857 CobWeb-lnx-1.0.1/src/CobWeb/
+-rw-rw-rw-   0        0        0       51 2023-04-26 18:02:34.000000 CobWeb-lnx-1.0.1/src/CobWeb/__init__.py
+-rw-rw-rw-   0        0        0    11299 2023-04-28 13:50:41.000000 CobWeb-lnx-1.0.1/src/CobWeb/crawler.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:59:20.854343 CobWeb-lnx-1.0.1/src/CobWeb_lnx.egg-info/
+-rw-rw-rw-   0        0        0     3856 2023-04-28 13:59:20.000000 CobWeb-lnx-1.0.1/src/CobWeb_lnx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-04-28 13:59:20.000000 CobWeb-lnx-1.0.1/src/CobWeb_lnx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 13:59:20.000000 CobWeb-lnx-1.0.1/src/CobWeb_lnx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      362 2023-04-28 13:59:20.000000 CobWeb-lnx-1.0.1/src/CobWeb_lnx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-28 13:59:20.000000 CobWeb-lnx-1.0.1/src/CobWeb_lnx.egg-info/top_level.txt
```

### Comparing `CobWeb-lnx-1.0.0/LICENSE.md` & `CobWeb-lnx-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `CobWeb-lnx-1.0.0/PKG-INFO` & `CobWeb-lnx-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CobWeb-lnx
-Version: 1.0.0
+Version: 1.0.1
 Summary: CobWeb is a Python library for web scraping. The library consists of two classes: Spider and Scraper.
 Author-email: "Gonçalo Marques (_lnx/lnxdread)" <gmgoncalo7@gmail.com>
 Project-URL: Homepage, https://github.com/GoncaloMark/Amara-CobWeb
 Project-URL: Bug Tracker, https://github.com/GoncaloMark/Amara-CobWeb/issues
 Keywords: data,crawler,scraper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CobWeb-lnx-1.0.0/README.md` & `CobWeb-lnx-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `CobWeb-lnx-1.0.0/pyproject.toml` & `CobWeb-lnx-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "CobWeb-lnx"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     { name="Gonçalo Marques (_lnx/lnxdread)", email="gmgoncalo7@gmail.com" },
 ]
 description = "CobWeb is a Python library for web scraping. The library consists of two classes: Spider and Scraper."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `CobWeb-lnx-1.0.0/src/CobWeb/crawler.py` & `CobWeb-lnx-1.0.1/src/CobWeb/crawler.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 from urllib.parse import urlparse, urljoin
 from bs4 import BeautifulSoup
 import yaml
 from os import path
 import itertools
 import asyncio
 import aiohttp
-import threading
-import concurrent.futures
-import multiprocessing
+import timeit
+
 
 ## This class defines a web crawler that can identify internal and external links on a given website.
 
 class Spider:
     """
     Constructor method for the Spider class.
     @param url The URL of the website to be crawled.
@@ -54,15 +53,15 @@
 
     ## Crawls the website and identifies internal and external links.
     async def getLinks(self, session = aiohttp.ClientSession):
         page = await session.request("GET", self._url)
         page.raise_for_status()
         domain_name = urlparse(self._url).netloc
         html = await page.text()
-        soup = BeautifulSoup(html, "html.parser")
+        soup = BeautifulSoup(html, "lxml")
         #TODO: throw netwrok errors like 403 forbidden
 
         # Loop over all <a> tags and get their href attributes.
         for link_tag in soup.find_all("a")[0:self.hops]:
             href = link_tag.attrs.get("href") 
 
             # If there is no href, continue to the next link.
@@ -139,113 +138,106 @@
 
         super().__init__(config["url"], config["hops"])
 
         self.__config = config
         self.__Ilinks = []
         self.__cache = {}
 
-        self._parsed = []
-
-        self.__executor = concurrent.futures.ThreadPoolExecutor(max_workers=multiprocessing.cpu_count())
-
     async def __get_html(self, link, session = aiohttp.ClientSession):
         """
         A private method to download and parse the HTML from the URLs in the Spider object.
 
         Returns:
             BeautifulSoup: A BeautifulSoup object containing the parsed HTML.
 
         """
         if link not in self.__cache:
             page = await session.request("GET", link)
             page.raise_for_status()
             html = await page.text()
-            future = self.__executor.submit(self.__soup_work, link, html)
-            return future.result()
-
-    
-    def __soup_work(self, link, html):
-        lock = threading.Lock()
-        soup = BeautifulSoup(html, "html.parser")
-
-        with lock:
+            soup = BeautifulSoup(html, "lxml")
             self.__cache[link] = soup
-
-        return self.__cache[link]
-    
+            return self.__cache[link]
+            
     async def __parse(self, link, session = aiohttp.ClientSession):
         html = await self.__get_html(link, session)
-        self._parsed.append(html)
+        scrape_list = [[x for x in self.__scrapeByElem(html)], [x for x in self.__scrapeByAttr(html)], [x for x in self.__scrapeByClassName(html)], [x for x in self.__scrapeBySelector(html)]]
+        return (link, {
+            "By_Element": scrape_list[0],
+            "By_Attribute": scrape_list[1],
+            "By_Class": scrape_list[2],
+            "By_Selector": scrape_list[3]
+        })
 
-    def __scrapeByElem(self):
+    def __scrapeByElem(self, html):
         """
         A private method to scrape elements from the HTML using element tags.
 
         Returns:
             List[Tag]: A list of Tag objects containing the scraped elements.
 
         """
         if self.__config.get("tags") is None or len(self.__config["tags"]) == 0:
             return
         
-        for soup, tag in itertools.product(self._parsed, self.__config["tags"]):
-            result = soup.find_all(tag)
+        for tag in self.__config["tags"]:
+            result = html.find_all(tag)
 
             for el in result:
                 yield el
 
-    def __scrapeBySelector(self):
+    def __scrapeBySelector(self, html):
         """
         A private method to scrape elements from the HTML using CSS selectors.
 
         Returns:
             List[Tag]: A list of Tag objects containing the scraped elements.
 
         """
         if self.__config.get("selectors") is None or len(self.__config["selectors"]) == 0:
             return
         result = []
-        for soup, selector in itertools.product(self._parsed, self.__config["selectors"]):
+        for selector in self.__config["selectors"]:
             if selector == "id":
                 for value in self.__config["IDvalue"]:
-                    result.append(soup.select_one("#"+value))
-            result.append(soup.select(selector))
+                    result.append(html.select_one("#"+value))
+            result.append(html.select(selector))
             for el in result:
                 yield el
 
-    def __scrapeByClassName(self):
+    def __scrapeByClassName(self, html):
         """
         A private method to scrape elements from the HTML using class names.
 
         Returns:
             List[Tag]: A list of Tag objects containing the scraped elements.
 
         """
         if self.__config.get("classes") is None or len(self.__config["classes"]) == 0:
             return
         
-        for soup, tag, clsName in itertools.product(self._parsed, self.__config["tags"], self.__config["classes"]):
-            result = soup.find_all(tag, class_=str(clsName))
+        for tag, clsName in itertools.product(self.__config["tags"], self.__config["classes"]):
+            result = html.find_all(tag, class_=str(clsName))
 
             for el in result:
                 yield el
 
-    def __scrapeByAttr(self):
+    def __scrapeByAttr(self, html):
         """
         A private method to scrape elements from the HTML using attributes.
 
         Returns:
             List[Tag]: A list of Tag objects containing the scraped elements.
 
         """
         if self.__config.get("attrs") is None or len(self.__config["attrs"]) == 0:
             return
 
-        for soup, tag, attrName, value in itertools.product(self._parsed, self.__config["tags"], self.__config["attrs"], self.__config["attrV"]):
-            result = soup.find_all(tag, attrs={attrName:value})
+        for tag, attrName, value in itertools.product(self.__config["tags"], self.__config["attrs"], self.__config["attrV"]):
+            result = html.find_all(tag, attrs={attrName:value})
 
             for el in result:
                 yield el
 
     async def __scrape(self):
         """
         A public method to return all the scraped content and prints it.
@@ -266,22 +258,17 @@
             else:
                 self.__Ilinks = [self.__config["url"]]
             tasks = []
             for link in self.__Ilinks:
                 tasks.append(
                     self.__parse(link, session=session)
                 )
-            await asyncio.gather(*tasks)
-            scrape_list = [[x for x in self.__scrapeByElem()], [x for x in self.__scrapeByAttr()], [x for x in self.__scrapeByClassName()], [x for x in self.__scrapeBySelector()]]
-            return {
-                "By_Element": scrape_list[0],
-                "By_Attribute": scrape_list[1],
-                "By_Class": scrape_list[2],
-                "By_Selector": scrape_list[3]
-            }
+            result = [await asyncio.gather(*tasks)]
+            return result
+            
         
     def run(self):
         result = asyncio.run(self.__scrape())
         return result
 
 
     def __str__(self):
@@ -319,22 +306,26 @@
     """ print("Specify config file (YAML) Path!")
     config_path = input()
     if path.exists(config_path) != True:
         raise ValueError """
     
     #SCRAPER TEST WITH CONFIG OBJECT! 
     config = {
-            "url": "https://stackoverflow.com/",
-            "tags": ["h1", "p"]
+            "url": "http://quotes.toscrape.com/",
+            "tags": ["small", "h3"],
+            "hops": 1000
         } 
 
     #config = config_parser(config_file=config_path)
     scrape = Scraper(config=config)
     #scrape.getLinks()
     #print(scrape.showLinks())
-    result = scrape.run()
-    print(result)
+    #result = scrape.run()
+    #print(result)
+    time = timeit.timeit(scrape.run, number=1)
+    print(time)
+    
     """ 
     SPIDER TEST!
     crawl = Spider("url", 10)
     crawl.getLinks()
     print(crawl.showLinks()) """
```

### Comparing `CobWeb-lnx-1.0.0/src/CobWeb_lnx.egg-info/PKG-INFO` & `CobWeb-lnx-1.0.1/src/CobWeb_lnx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CobWeb-lnx
-Version: 1.0.0
+Version: 1.0.1
 Summary: CobWeb is a Python library for web scraping. The library consists of two classes: Spider and Scraper.
 Author-email: "Gonçalo Marques (_lnx/lnxdread)" <gmgoncalo7@gmail.com>
 Project-URL: Homepage, https://github.com/GoncaloMark/Amara-CobWeb
 Project-URL: Bug Tracker, https://github.com/GoncaloMark/Amara-CobWeb/issues
 Keywords: data,crawler,scraper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

