# Comparing `tmp/dpi_maps-0.0.1.tar.gz` & `tmp/dpi_maps-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpi_maps-0.0.1.tar", max compression
+gzip compressed data, was "dpi_maps-0.0.2.tar", max compression
```

## Comparing `dpi_maps-0.0.1.tar` & `dpi_maps-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      122 2023-03-13 06:27:28.201197 dpi_maps-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-03-13 06:51:42.697878 dpi_maps-0.0.1/dpi_maps/__init__.py
--rw-r--r--   0        0        0       29 2023-03-10 03:11:54.363527 dpi_maps-0.0.1/dpi_maps/__main__.py
--rw-r--r--   0        0        0     3348 2023-03-13 06:12:20.023854 dpi_maps-0.0.1/dpi_maps/main.py
--rw-r--r--   0        0        0    10894 2023-03-13 06:19:59.032954 dpi_maps-0.0.1/dpi_maps/scrapers.py
--rw-r--r--   0        0        0     1073 2023-03-13 06:09:33.385805 dpi_maps-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      861 1970-01-01 00:00:00.000000 dpi_maps-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      966 2023-04-28 10:59:36.908731 dpi_maps-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-28 10:59:36.912731 dpi_maps-0.0.2/dpi_maps/__init__.py
+-rw-r--r--   0        0        0       29 2023-04-28 10:59:36.912731 dpi_maps-0.0.2/dpi_maps/__main__.py
+-rw-r--r--   0        0        0     3348 2023-04-28 10:59:36.912731 dpi_maps-0.0.2/dpi_maps/main.py
+-rw-r--r--   0        0        0    10889 2023-04-28 10:59:36.912731 dpi_maps-0.0.2/dpi_maps/scrapers.py
+-rw-r--r--   0        0        0     1073 2023-04-28 10:59:36.912731 dpi_maps-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 dpi_maps-0.0.2/PKG-INFO
```

### Comparing `dpi_maps-0.0.1/dpi_maps/main.py` & `dpi_maps-0.0.2/dpi_maps/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 ):
     """
     DPI Map Scaper.
 
     This application retrieves all the maps from the DPI website. It
     requires a valid login to the portal.
 
-    Set DPI_USERNAME and DPI_PASSWORD environment
-    variables before attempting to run any commands.
+    Set DPI_USERNAME and DPI_PASSWORD environment variables before
+    attempting to run any commands.
 
     Use at own risk.
     """
     ctx.obj = GlobalVars(directory=directory, verbose=verbose)
 
 
 @app.command(name="reports")
```

### Comparing `dpi_maps-0.0.1/dpi_maps/scrapers.py` & `dpi_maps-0.0.2/dpi_maps/scrapers.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
             txt = await item.inner_text()
             val = await item.get_attribute("value")
             if val is None:
                 continue
             dropdowns.append({"name": txt, "value": val})
 
         result = []
-        for option in dropdowns[5:7]:
+        for option in dropdowns:
             await self.page.get_by_label("Hunting Area").select_option(option.get("name"))
             pdf = await self.page.query_selector(
                 "#areasList > table > tbody > tr:nth-child(3) > td:nth-child(1) > a"
             )
             kmz = await self.page.query_selector(
                 "#areasList > table > tbody > tr:nth-child(4) > td:nth-child(1) > a"
             )
```

### Comparing `dpi_maps-0.0.1/pyproject.toml` & `dpi_maps-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dpi-maps"
-version = "0.0.1"
+version = "0.0.2"
 description = "Download maps from the Deptment of Prime Industries for use in R license activites."
 authors = ["Daniel Michaels <dan@danielms.site>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 typer = { extras = ["all"], version = "^0.7.0" }
```

