# Comparing `tmp/rfswarm-reporter-1.1.0.tar.gz` & `tmp/rfswarm-reporter-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfswarm-reporter-1.1.0.tar", last modified: Fri Mar 31 03:19:08 2023, max compression
+gzip compressed data, was "rfswarm-reporter-1.1.1.tar", last modified: Fri Apr 28 08:51:31 2023, max compression
```

## Comparing `rfswarm-reporter-1.1.0.tar` & `rfswarm-reporter-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-31 03:19:08.016695 rfswarm-reporter-1.1.0/
--rw-r--r--   0 dave      (1000) dave      (1000)    35149 2023-02-10 08:46:44.000000 rfswarm-reporter-1.1.0/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)     3110 2023-03-31 03:19:08.012695 rfswarm-reporter-1.1.0/PKG-INFO
--rw-r--r--   0 dave      (1000) dave      (1000)     5809 2023-03-31 03:05:35.000000 rfswarm-reporter-1.1.0/README.md
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-31 03:19:08.012695 rfswarm-reporter-1.1.0/rfswarm_reporter/
--rw-r--r--   0 dave      (1000) dave      (1000)       53 2023-03-31 03:19:06.000000 rfswarm-reporter-1.1.0/rfswarm_reporter/__init__.py
--rw-r--r--   0 dave      (1000) dave      (1000)   310619 2023-03-31 03:19:06.000000 rfswarm-reporter-1.1.0/rfswarm_reporter/rfswarm_reporter.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-03-31 03:19:08.012695 rfswarm-reporter-1.1.0/rfswarm_reporter.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     3110 2023-03-31 03:19:07.000000 rfswarm-reporter-1.1.0/rfswarm_reporter.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      343 2023-03-31 03:19:07.000000 rfswarm-reporter-1.1.0/rfswarm_reporter.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-03-31 03:19:07.000000 rfswarm-reporter-1.1.0/rfswarm_reporter.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       80 2023-03-31 03:19:07.000000 rfswarm-reporter-1.1.0/rfswarm_reporter.egg-info/entry_points.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       85 2023-03-31 03:19:07.000000 rfswarm-reporter-1.1.0/rfswarm_reporter.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       17 2023-03-31 03:19:07.000000 rfswarm-reporter-1.1.0/rfswarm_reporter.egg-info/top_level.txt
--rw-r--r--   0 dave      (1000) dave      (1000)     1504 2023-03-31 03:19:06.000000 rfswarm-reporter-1.1.0/setup-reporter.py
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-03-31 03:19:08.016695 rfswarm-reporter-1.1.0/setup.cfg
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-04-28 08:51:31.009142 rfswarm-reporter-1.1.1/
+-rw-r--r--   0 dave      (1000) dave      (1000)    35149 2023-02-10 08:46:44.000000 rfswarm-reporter-1.1.1/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3110 2023-04-28 08:51:31.009142 rfswarm-reporter-1.1.1/PKG-INFO
+-rw-r--r--   0 dave      (1000) dave      (1000)     5809 2023-04-28 08:33:44.000000 rfswarm-reporter-1.1.1/README.md
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-04-28 08:51:31.009142 rfswarm-reporter-1.1.1/rfswarm_reporter/
+-rw-r--r--   0 dave      (1000) dave      (1000)       53 2023-04-28 08:51:30.000000 rfswarm-reporter-1.1.1/rfswarm_reporter/__init__.py
+-rw-r--r--   0 dave      (1000) dave      (1000)   310811 2023-04-28 08:51:30.000000 rfswarm-reporter-1.1.1/rfswarm_reporter/rfswarm_reporter.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-04-28 08:51:31.009142 rfswarm-reporter-1.1.1/rfswarm_reporter.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3110 2023-04-28 08:51:30.000000 rfswarm-reporter-1.1.1/rfswarm_reporter.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      343 2023-04-28 08:51:30.000000 rfswarm-reporter-1.1.1/rfswarm_reporter.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-04-28 08:51:30.000000 rfswarm-reporter-1.1.1/rfswarm_reporter.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       80 2023-04-28 08:51:30.000000 rfswarm-reporter-1.1.1/rfswarm_reporter.egg-info/entry_points.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       85 2023-04-28 08:51:30.000000 rfswarm-reporter-1.1.1/rfswarm_reporter.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       17 2023-04-28 08:51:30.000000 rfswarm-reporter-1.1.1/rfswarm_reporter.egg-info/top_level.txt
+-rw-r--r--   0 dave      (1000) dave      (1000)     1504 2023-04-28 08:51:30.000000 rfswarm-reporter-1.1.1/setup-reporter.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-04-28 08:51:31.009142 rfswarm-reporter-1.1.1/setup.cfg
```

### Comparing `rfswarm-reporter-1.1.0/LICENSE` & `rfswarm-reporter-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rfswarm-reporter-1.1.0/PKG-INFO` & `rfswarm-reporter-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfswarm-reporter
-Version: 1.1.0
+Version: 1.1.1
 Summary: rfswarm reporter
 Home-page: https://github.com/damies13/rfswarm
 Author: damies13
 Author-email: damies13+rfswarm@gmail.com
 License: UNKNOWN
 Project-URL: Getting Help, https://github.com/damies13/rfswarm#getting-help
 Project-URL: Say Thanks!, https://github.com/damies13/rfswarm#donations
```

### Comparing `rfswarm-reporter-1.1.0/README.md` & `rfswarm-reporter-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 |Version|Manager|Agent|Reporter|
 |---|---|---|---|
 |[![Latest PyPI version](https://img.shields.io/pypi/v/rfswarm-manager.svg)](https://pypi.python.org/pypi/rfswarm-manager/) | [![Number of Manager PyPI downloads](https://img.shields.io/pypi/dm/rfswarm-manager.svg)](https://pypi.python.org/pypi/rfswarm-manager/) | [![Number of Agent PyPI downloads](https://img.shields.io/pypi/dm/rfswarm-agent.svg)](https://pypi.python.org/pypi/rfswarm-agent/) | [![Number of Reporter PyPI downloads](https://img.shields.io/pypi/dm/rfswarm-reporter.svg)](https://pypi.python.org/pypi/rfswarm-reporter/) |
 
 | Master | Branch |
 | -- | -- |
-| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=master&label=Linter)](https://github.com/damies13/rfswarm/actions/workflows/superlinter.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=v1.1.0&label=Linter) |
-| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=master&label=Regression%20Tests)](https://github.com/damies13/rfswarm/actions/workflows/Regression_Tests.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=v1.1.0&label=Regression%20Tests) |
+| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=master&label=Linter)](https://github.com/damies13/rfswarm/actions/workflows/superlinter.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=v1.1.1&label=Linter) |
+| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=master&label=Regression%20Tests)](https://github.com/damies13/rfswarm/actions/workflows/Regression_Tests.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=v1.1.1&label=Regression%20Tests) |
 
 <img align="right" src="Doc/Images/Icon_Information.png">
 
 ## About
 rfswarm is a testing tool that allows you use [Robot Framework](https://robotframework.org/) test cases for performance or load testing.
 
 > _Swarm being the collective noun for Robots, just as Flock is for Birds and Herd for Sheep, so it made sense to use swarm for a performance testing tool using Robot Framework, hence rfswarm_
```

### Comparing `rfswarm-reporter-1.1.0/rfswarm_reporter/rfswarm_reporter.py` & `rfswarm-reporter-1.1.1/rfswarm_reporter/rfswarm_reporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 #
 # 	Robot Framework Swarm
 # 		Reporter
-#    Version1.1.0"
+#    Version 1.1.1
 #
 
 import argparse
 import base64  # used for embedding images  # used for xhtml export
 import configparser
 import inspect
 import math
@@ -114,15 +114,15 @@
 			base.debugmsg(8, "res:", res)
 			return res
 		except Exception as e:
 			base.debugmsg(5, "Exception:", e)
 
 
 class ReporterBase():
-	version = "1.1.0"
+	version = "1.1.1"
 	debuglvl = 0
 
 	save_ini = True
 	running = True
 	displaygui = True
 	gui = None
 	darkmode = False
@@ -240,15 +240,15 @@
 					pass
 		# This should cause saveini to fail?
 		return None
 
 	def saveini(self):
 		self.debugmsg(6, "save_ini:", self.save_ini)
 		if self.save_ini:
-			with open(base.reporter_ini, 'w') as configfile:    # save
+			with open(base.reporter_ini, 'w', encoding="utf8") as configfile:    # save
 				base.config.write(configfile)
 				self.debugmsg(6, "File Saved:", self.reporter_ini)
 
 	#
 	# Template Functions
 	#
 	def template_create(self):
@@ -283,15 +283,15 @@
 		# datatype = ResultSummary
 		self.rt_table_set_dt(trs, "ResultSummary")
 
 	def template_save(self, filename):
 		saved = False
 		if filename is None or len(filename) < 1:
 			filename = base.config['Reporter']['Template']
-		with open(filename, 'w') as templatefile:    # save
+		with open(filename, 'w', encoding="utf8") as templatefile:    # save
 			base.report.write(templatefile)
 			self.debugmsg(6, "Template Saved:", filename)
 			saved = True
 		if saved:
 			base.config['Reporter']['Template'] = base.whitespace_set_ini_value(filename)
 			path, file = os.path.split(base.config['Reporter']['Template'])
 			base.config['Reporter']['TemplateDir'] = base.whitespace_set_ini_value(path)
@@ -305,15 +305,15 @@
 			path, file = os.path.split(base.config['Reporter']['Template'])
 			base.config['Reporter']['TemplateDir'] = base.whitespace_set_ini_value(path)
 			base.saveini()
 
 			base.report = None
 			self.reportdata = {}
 			base.report = configparser.ConfigParser()
-			base.report.read(filename)
+			base.report.read(filename, encoding="utf8")
 
 			base.report_item_set_changed_all("TOP")
 
 		else:
 			base.template_create()
 
 	#
@@ -321,29 +321,29 @@
 	#
 
 	def report_save(self):
 		saved = False
 		if 'Reporter' in base.config:
 			if 'Report' in base.config['Reporter']:
 				filename = base.config['Reporter']['Report']
-				with open(filename, 'w') as reportfile:    # save
+				with open(filename, 'w', encoding="utf8") as reportfile:    # save
 					base.report.write(reportfile)
 					self.debugmsg(6, "Report Saved:", filename)
 					saved = True
 		return saved
 
 	def report_open(self):
 		filename = base.config['Reporter']['Report']
 		base.debugmsg(7, "filename: ", filename)
 		base.reportdata = {}
 		base.report = None
 		if len(filename) > 0 and os.path.isfile(filename):
 			base.debugmsg(7, "filename: ", filename, " exists, open")
 			base.report = configparser.ConfigParser()
-			base.report.read(filename)
+			base.report.read(filename, encoding="utf8")
 		else:
 			templatefile = base.whitespace_get_ini_value(base.config['Reporter']['Template'])
 			base.debugmsg(7, "Template: ", templatefile)
 			if len(templatefile) > 0:
 				base.template_open(templatefile)
 			else:
 				base.debugmsg(7, "template_create")
@@ -526,31 +526,34 @@
 		value = self.rs_setting_get('hcolour')
 		if value is None:
 			return "#0000FF"  # Blue
 		else:
 			return value
 
 	def rs_setting_get_font(self):
-		fontlst = list(tkFont.families())
-		base.debugmsg(9, "fontlst", fontlst)
 		value = self.rs_setting_get('font')
-		if value not in fontlst:
-			value = None
-		if value is None:
-			# Verdana, Tahoma, Arial, Helvetica, sans-serif
-			fontorder = ['Helvetica', 'Verdana', 'Tahoma', 'Arial', 'FreeSans']
-			for fnt in fontorder:
-				if fnt in fontlst:
-					return fnt
-			for fnt in fontlst:
-				if 'Sans' in fnt or 'sans' in fnt:
-					return fnt
-			return 'sans-serif'
-		else:
+		if not self.gui:
 			return value
+		else:
+			fontlst = list(tkFont.families())
+			base.debugmsg(9, "fontlst", fontlst)
+			if value not in fontlst:
+				value = None
+			if value is None:
+				# Verdana, Tahoma, Arial, Helvetica, sans-serif
+				fontorder = ['Helvetica', 'Verdana', 'Tahoma', 'Arial', 'FreeSans']
+				for fnt in fontorder:
+					if fnt in fontlst:
+						return fnt
+				for fnt in fontlst:
+					if 'Sans' in fnt or 'sans' in fnt:
+						return fnt
+				return 'sans-serif'
+			else:
+				return value
 
 	def rs_setting_get_fontsize(self):
 		value = self.rs_setting_get_int('fontsize')
 		if value < 1:
 			return 12
 		else:
 			return int(value)
@@ -2327,15 +2330,15 @@
 		if base.args.ini:
 			base.save_ini = False
 			base.debugmsg(5, "base.args.ini: ", base.args.ini)
 			base.reporter_ini = base.args.ini
 
 		if os.path.isfile(base.reporter_ini):
 			base.debugmsg(7, "reporter_ini: ", base.reporter_ini)
-			base.config.read(base.reporter_ini)
+			base.config.read(base.reporter_ini, encoding="utf8")
 		else:
 			base.saveini()
 
 		base.debugmsg(0, "	Configuration File: ", base.reporter_ini)
 
 		base.debugmsg(9, "base.config: ", base.config._sections)
 
@@ -2377,15 +2380,15 @@
 		if 'TemplateDir' not in base.config['Reporter']:
 			base.config['Reporter']['TemplateDir'] = ""
 			base.saveini()
 
 		usetemplate = False
 		if base.args.template:
 			usetemplate = True
-			base.config['Reporter']['Template'] = base.args.template
+			base.config['Reporter']['Template'] = base.whitespace_set_ini_value(base.args.template)
 
 		if base.args.dir:
 			# do some sanity checks before blindly setting
 			rdir = base.args.dir
 			base.debugmsg(5, "rdir:", rdir)
 			if os.path.exists(rdir):
 				if os.path.isfile(rdir):
```

### Comparing `rfswarm-reporter-1.1.0/rfswarm_reporter.egg-info/PKG-INFO` & `rfswarm-reporter-1.1.1/rfswarm_reporter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfswarm-reporter
-Version: 1.1.0
+Version: 1.1.1
 Summary: rfswarm reporter
 Home-page: https://github.com/damies13/rfswarm
 Author: damies13
 Author-email: damies13+rfswarm@gmail.com
 License: UNKNOWN
 Project-URL: Getting Help, https://github.com/damies13/rfswarm#getting-help
 Project-URL: Say Thanks!, https://github.com/damies13/rfswarm#donations
```

### Comparing `rfswarm-reporter-1.1.0/setup-reporter.py` & `rfswarm-reporter-1.1.1/setup-reporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README_PyPi.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="rfswarm-reporter",
-	version="1.1.0",
+	version="1.1.1",
 	author="damies13",
 	author_email="damies13+rfswarm@gmail.com",
 	description="rfswarm reporter",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/damies13/rfswarm",
 	packages=setuptools.find_packages(exclude=["*fswarm_manag*", "*fswarm_agen*", "build/*"]),
```

