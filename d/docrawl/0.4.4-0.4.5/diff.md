# Comparing `tmp/docrawl-0.4.4.tar.gz` & `tmp/docrawl-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docrawl-0.4.4.tar", last modified: Fri Apr 14 06:40:27 2023, max compression
+gzip compressed data, was "docrawl-0.4.5.tar", last modified: Thu Apr 27 23:47:40 2023, max compression
```

## Comparing `docrawl-0.4.4.tar` & `docrawl-0.4.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 06:40:27.779397 docrawl-0.4.4/
--rw-rw-rw-   0        0        0     1090 2021-08-16 12:38:07.000000 docrawl-0.4.4/LICENSE
--rw-rw-rw-   0        0        0      568 2023-04-14 06:40:27.779397 docrawl-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0       86 2021-08-16 12:38:07.000000 docrawl-0.4.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 06:40:27.763440 docrawl-0.4.4/docrawl/
--rw-rw-rw-   0        0        0        0 2021-08-16 12:40:29.000000 docrawl-0.4.4/docrawl/__init__.py
--rw-rw-rw-   0        0        0    40996 2023-04-14 06:39:31.000000 docrawl-0.4.4/docrawl/docrawl_core.py
--rw-rw-rw-   0        0        0     6355 2023-04-02 21:36:25.000000 docrawl-0.4.4/docrawl/docrawl_launcher.py
--rw-rw-rw-   0        0        0     1108 2023-02-25 18:40:39.000000 docrawl-0.4.4/docrawl/docrawl_logger.py
-drwxrwxrwx   0        0        0        0 2023-04-14 06:40:27.778399 docrawl-0.4.4/docrawl.egg-info/
--rw-rw-rw-   0        0        0      568 2023-04-14 06:40:27.000000 docrawl-0.4.4/docrawl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-04-14 06:40:27.000000 docrawl-0.4.4/docrawl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 06:40:27.000000 docrawl-0.4.4/docrawl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-04-14 06:40:27.000000 docrawl-0.4.4/docrawl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-14 06:40:27.000000 docrawl-0.4.4/docrawl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 06:40:27.779397 docrawl-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0      834 2023-04-14 06:40:23.000000 docrawl-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 23:47:40.446802 docrawl-0.4.5/
+-rw-rw-rw-   0        0        0     1090 2021-08-16 12:38:07.000000 docrawl-0.4.5/LICENSE
+-rw-rw-rw-   0        0        0      568 2023-04-27 23:47:40.446802 docrawl-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2021-08-16 12:38:07.000000 docrawl-0.4.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 23:47:40.431841 docrawl-0.4.5/docrawl/
+-rw-rw-rw-   0        0        0        0 2021-08-16 12:40:29.000000 docrawl-0.4.5/docrawl/__init__.py
+-rw-rw-rw-   0        0        0    41020 2023-04-27 23:46:19.000000 docrawl-0.4.5/docrawl/docrawl_core.py
+-rw-rw-rw-   0        0        0     6355 2023-04-02 21:36:25.000000 docrawl-0.4.5/docrawl/docrawl_launcher.py
+-rw-rw-rw-   0        0        0     1108 2023-02-25 18:40:39.000000 docrawl-0.4.5/docrawl/docrawl_logger.py
+drwxrwxrwx   0        0        0        0 2023-04-27 23:47:40.445804 docrawl-0.4.5/docrawl.egg-info/
+-rw-rw-rw-   0        0        0      568 2023-04-27 23:47:39.000000 docrawl-0.4.5/docrawl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-04-27 23:47:40.000000 docrawl-0.4.5/docrawl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 23:47:39.000000 docrawl-0.4.5/docrawl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-04-27 23:47:40.000000 docrawl-0.4.5/docrawl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-27 23:47:40.000000 docrawl-0.4.5/docrawl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 23:47:40.446802 docrawl-0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      834 2023-04-27 23:47:37.000000 docrawl-0.4.5/setup.py
```

### Comparing `docrawl-0.4.4/LICENSE` & `docrawl-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `docrawl-0.4.4/PKG-INFO` & `docrawl-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrawl
-Version: 0.4.4
+Version: 0.4.5
 Summary: Do automated crawling of pages using scrapy
 Home-page: https://github.com/DovaX/docrawl
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `docrawl-0.4.4/docrawl/docrawl_core.py` & `docrawl-0.4.5/docrawl/docrawl_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     context_xpath = inp['context_xpath']
     output_folder = inp['output_folder']
 
     # Predefined tags by type
     TABLE_TAG = ['table']
     BULLET_TAGS = ['ul', 'ol']
     TEXT_TAGS = ['p', 'strong', 'em', 'div[normalize-space(text())]', 'span[normalize-space(text())]']
-    HEADLINE_TAGS = ['h1', 'h2']
+    HEADLINE_TAGS = ['h1', 'h2', 'h3', 'h4', 'h5', 'h6']
     IMAGE_TAGS = ['img']
     BUTTON_TAGS = ['button', 'a[@role="button"]', 'a[contains(@class, "button")]',
                    'a[contains(@id, "button")]', 'a[@type="button"]', 'a[contains(@class, "btn")]']
 
     # <a> tags, excluding links in menu, links as images, mailto links and links with scripts
     LINK_TAGS = ["""
                     a[@href
```

### Comparing `docrawl-0.4.4/docrawl/docrawl_launcher.py` & `docrawl-0.4.5/docrawl/docrawl_launcher.py`

 * *Files identical despite different names*

### Comparing `docrawl-0.4.4/docrawl/docrawl_logger.py` & `docrawl-0.4.5/docrawl/docrawl_logger.py`

 * *Files identical despite different names*

### Comparing `docrawl-0.4.4/docrawl.egg-info/PKG-INFO` & `docrawl-0.4.5/docrawl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrawl
-Version: 0.4.4
+Version: 0.4.5
 Summary: Do automated crawling of pages using scrapy
 Home-page: https://github.com/DovaX/docrawl
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `docrawl-0.4.4/setup.py` & `docrawl-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='docrawl',
-    version='0.4.4',
+    version='0.4.5',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='Do automated crawling of pages using scrapy',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/docrawl',
     packages=setuptools.find_packages(),
```

