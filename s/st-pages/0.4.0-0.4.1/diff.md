# Comparing `tmp/st_pages-0.4.0.tar.gz` & `tmp/st_pages-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_pages-0.4.0.tar", max compression
+gzip compressed data, was "st_pages-0.4.1.tar", max compression
```

## Comparing `st_pages-0.4.0.tar` & `st_pages-0.4.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1074 2023-04-05 19:54:26.536502 st_pages-0.4.0/LICENSE
--rw-r--r--   0        0        0     4597 2023-04-05 19:54:26.536502 st_pages-0.4.0/README.md
--rw-r--r--   0        0        0     1012 2023-04-05 19:54:26.540501 st_pages-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    10915 2023-04-05 19:54:26.540501 st_pages-0.4.0/src/st_pages/__init__.py
--rw-r--r--   0        0        0     5243 1970-01-01 00:00:00.000000 st_pages-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-28 21:21:38.777100 st_pages-0.4.1/LICENSE
+-rw-r--r--   0        0        0     4597 2023-04-28 21:21:38.777100 st_pages-0.4.1/README.md
+-rw-r--r--   0        0        0     1012 2023-04-28 21:21:38.781100 st_pages-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    11017 2023-04-28 21:21:38.781100 st_pages-0.4.1/src/st_pages/__init__.py
+-rw-r--r--   0        0        0     5243 1970-01-01 00:00:00.000000 st_pages-0.4.1/PKG-INFO
```

### Comparing `st_pages-0.4.0/LICENSE` & `st_pages-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `st_pages-0.4.0/README.md` & `st_pages-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `st_pages-0.4.0/pyproject.toml` & `st_pages-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "st-pages"
-version = "0.4.0"
+version = "0.4.1"
 description = "An experimental version of Streamlit Multi-Page Apps"
 authors = ["Zachary Blackwood <zachary@streamlit.io>"]
 readme = "README.md"
 packages = [{include = "st_pages", from = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.9.7 || >3.9.7,<4.0"
```

### Comparing `st_pages-0.4.0/src/st_pages/__init__.py` & `st_pages-0.4.1/src/st_pages/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,27 +292,27 @@
 def _get_indentation_code() -> str:
     styling = ""
     current_pages = get_pages("")
     is_indented = False
     for idx, val in enumerate(current_pages.values()):
         if val.get("is_section"):
             styling += f"""
-                li:nth-child({idx + 1}) a {{
+                div[data-testid=\"stSidebarNav\"] li:nth-child({idx + 1}) a {{
                     pointer-events: none; /* Disable clicking on section header */
                 }}
             """
             is_indented = True
         elif is_indented and not val.get("in_section"):
             # Page is specifically unnested
             # Un-indent all pages until next section
             is_indented = False
         elif is_indented:
             # Unless specifically unnested, indent all pages that aren't section headers
             styling += f"""
-                li:nth-child({idx + 1}) span:nth-child(1) {{
+                div[data-testid=\"stSidebarNav\"] li:nth-child({idx + 1}) span:nth-child(1) {{
                     margin-left: 1.5rem;
                 }}
             """
 
     styling = f"""
         <style>
             {styling}
@@ -357,15 +357,15 @@
             # Set whole section as hidden
             section_hidden = page_name in pages_to_hide
         elif not val.get("in_section"):
             # Reset whole section hiding if we hit a page thats not in a section
             section_hidden = False
         if page_name in pages_to_hide or section_hidden:
             styling += f"""
-                li:nth-child({idx + 1}) {{
+                div[data-testid=\"stSidebarNav\"] li:nth-child({idx + 1}) {{
                     display: none;
                 }}
             """
 
     styling = f"""
         <style>
             {styling}
```

### Comparing `st_pages-0.4.0/PKG-INFO` & `st_pages-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-pages
-Version: 0.4.0
+Version: 0.4.1
 Summary: An experimental version of Streamlit Multi-Page Apps
 Author: Zachary Blackwood
 Author-email: zachary@streamlit.io
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

