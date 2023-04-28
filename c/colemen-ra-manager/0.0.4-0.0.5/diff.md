# Comparing `tmp/colemen_ra_manager-0.0.4.tar.gz` & `tmp/colemen_ra_manager-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colemen_ra_manager-0.0.4.tar", last modified: Thu Mar 30 19:39:21 2023, max compression
+gzip compressed data, was "colemen_ra_manager-0.0.5.tar", last modified: Fri Apr 28 17:49:03 2023, max compression
```

## Comparing `colemen_ra_manager-0.0.4.tar` & `colemen_ra_manager-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 19:39:21.877970 colemen_ra_manager-0.0.4/
--rw-rw-rw-   0        0        0      528 2023-03-30 19:39:21.876972 colemen_ra_manager-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-30 19:39:21.857970 colemen_ra_manager-0.0.4/colemen_ra_manager.egg-info/
--rw-rw-rw-   0        0        0      528 2023-03-30 19:39:21.000000 colemen_ra_manager-0.0.4/colemen_ra_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-03-30 19:39:21.000000 colemen_ra_manager-0.0.4/colemen_ra_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 19:39:21.000000 colemen_ra_manager-0.0.4/colemen_ra_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-03-30 19:39:21.000000 colemen_ra_manager-0.0.4/colemen_ra_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-03-30 19:39:21.000000 colemen_ra_manager-0.0.4/colemen_ra_manager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      587 2023-03-30 13:42:45.000000 colemen_ra_manager-0.0.4/main.py
-drwxrwxrwx   0        0        0        0 2023-03-30 19:39:21.871971 colemen_ra_manager-0.0.4/ramanager/
--rw-rw-rw-   0        0        0    12364 2023-03-30 19:35:19.000000 colemen_ra_manager-0.0.4/ramanager/Project.py
--rw-rw-rw-   0        0        0     7787 2023-03-30 19:31:37.000000 colemen_ra_manager-0.0.4/ramanager/ProjectBase.py
--rw-rw-rw-   0        0        0    11453 2023-03-30 19:39:08.000000 colemen_ra_manager-0.0.4/ramanager/ProjectManager.py
--rw-rw-rw-   0        0        0    15075 2023-03-30 15:40:48.000000 colemen_ra_manager-0.0.4/ramanager/Year.py
--rw-rw-rw-   0        0        0      407 2023-03-30 19:07:01.000000 colemen_ra_manager-0.0.4/ramanager/__init__.py
--rw-rw-rw-   0        0        0     3229 2023-03-30 19:06:28.000000 colemen_ra_manager-0.0.4/ramanager/inputs.py
-drwxrwxrwx   0        0        0        0 2023-03-30 19:39:21.875971 colemen_ra_manager-0.0.4/ramanager/settings/
--rw-rw-rw-   0        0        0       86 2023-03-30 14:04:21.000000 colemen_ra_manager-0.0.4/ramanager/settings/__init__.py
--rw-rw-rw-   0        0        0      435 2023-03-30 19:34:43.000000 colemen_ra_manager-0.0.4/ramanager/settings/control.py
--rw-rw-rw-   0        0        0      710 2023-03-30 14:59:32.000000 colemen_ra_manager-0.0.4/ramanager/settings/types.py
--rw-rw-rw-   0        0        0       42 2023-03-30 19:39:21.877970 colemen_ra_manager-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1488 2023-03-30 19:39:13.000000 colemen_ra_manager-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 17:49:03.728712 colemen_ra_manager-0.0.5/
+-rw-rw-rw-   0        0        0      528 2023-04-28 17:49:03.727712 colemen_ra_manager-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-28 17:49:03.714716 colemen_ra_manager-0.0.5/colemen_ra_manager.egg-info/
+-rw-rw-rw-   0        0        0      528 2023-04-28 17:49:03.000000 colemen_ra_manager-0.0.5/colemen_ra_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2023-04-28 17:49:03.000000 colemen_ra_manager-0.0.5/colemen_ra_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 17:49:03.000000 colemen_ra_manager-0.0.5/colemen_ra_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-28 17:49:03.000000 colemen_ra_manager-0.0.5/colemen_ra_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-28 17:49:03.000000 colemen_ra_manager-0.0.5/colemen_ra_manager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      587 2023-03-30 13:42:45.000000 colemen_ra_manager-0.0.5/main.py
+drwxrwxrwx   0        0        0        0 2023-04-28 17:49:03.723713 colemen_ra_manager-0.0.5/ramanager/
+-rw-rw-rw-   0        0        0    12407 2023-04-24 22:10:25.000000 colemen_ra_manager-0.0.5/ramanager/Project.py
+-rw-rw-rw-   0        0        0     8008 2023-04-28 17:48:20.000000 colemen_ra_manager-0.0.5/ramanager/ProjectBase.py
+-rw-rw-rw-   0        0        0    11453 2023-03-30 19:39:08.000000 colemen_ra_manager-0.0.5/ramanager/ProjectManager.py
+-rw-rw-rw-   0        0        0      769 2023-04-24 22:59:50.000000 colemen_ra_manager-0.0.5/ramanager/TextToSpeech.py
+-rw-rw-rw-   0        0        0    15075 2023-03-30 15:40:48.000000 colemen_ra_manager-0.0.5/ramanager/Year.py
+-rw-rw-rw-   0        0        0      407 2023-03-30 19:07:01.000000 colemen_ra_manager-0.0.5/ramanager/__init__.py
+-rw-rw-rw-   0        0        0     3229 2023-03-30 19:06:28.000000 colemen_ra_manager-0.0.5/ramanager/inputs.py
+drwxrwxrwx   0        0        0        0 2023-04-28 17:49:03.727712 colemen_ra_manager-0.0.5/ramanager/settings/
+-rw-rw-rw-   0        0        0       86 2023-03-30 14:04:21.000000 colemen_ra_manager-0.0.5/ramanager/settings/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-03-30 19:34:43.000000 colemen_ra_manager-0.0.5/ramanager/settings/control.py
+-rw-rw-rw-   0        0        0      710 2023-03-30 14:59:32.000000 colemen_ra_manager-0.0.5/ramanager/settings/types.py
+-rw-rw-rw-   0        0        0       42 2023-04-28 17:49:03.728712 colemen_ra_manager-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1488 2023-04-28 17:48:57.000000 colemen_ra_manager-0.0.5/setup.py
```

### Comparing `colemen_ra_manager-0.0.4/PKG-INFO` & `colemen_ra_manager-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colemen_ra_manager
-Version: 0.0.4
+Version: 0.0.5
 Summary: colemen_ra_manager
 Author: Colemen Atwood
 Author-email: <atwoodcolemen@gmail.com>
 Keywords: python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `colemen_ra_manager-0.0.4/colemen_ra_manager.egg-info/PKG-INFO` & `colemen_ra_manager-0.0.5/colemen_ra_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colemen-ra-manager
-Version: 0.0.4
+Version: 0.0.5
 Summary: colemen_ra_manager
 Author: Colemen Atwood
 Author-email: <atwoodcolemen@gmail.com>
 Keywords: python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `colemen_ra_manager-0.0.4/main.py` & `colemen_ra_manager-0.0.5/main.py`

 * *Files identical despite different names*

### Comparing `colemen_ra_manager-0.0.4/ramanager/Project.py` & `colemen_ra_manager-0.0.5/ramanager/Project.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from string import Template
 import subprocess
 import colemen_utils as c
 
 import ramanager.settings.types as _t
 import ramanager.settings as _settings
 
+
 from ramanager.ProjectBase import ProjectBase
 
 # VALID_PROJECT_TYPES = ["general","python","3dprint"]
 
 @dataclass
 class Project(ProjectBase):
 
@@ -34,23 +35,23 @@
         description:str=None,
         project_type:str=None,
         ):
         super().__init__(main, year, directory,project_id,title,description,project_type,)
 
 
 
-
 class GeneralProject(ProjectBase):
 
 
     def create_master(self):
         print(f"GeneralProject.create_master")
         print(f"self.dir_path:{self.dir_path}")
         c.dirs.create(self.dir_path)
         self.directory = c.dirs.get_folder(self.dir_path)
+        self.speak_complete()
 
 class PrintingProject(ProjectBase):
 
 
     def __init__(
         self,
         main:_t.main_type,
@@ -284,14 +285,16 @@
                 #     "description":self.description,
                 #     "title_snake_case":self.sub_dir_name,
                 # }
             # c.dirs.create(dst)
         self._run_build_setup()
         
         c.con.log(f"Successfully Created Project {self.title}","green invert")
+        
+
 
     def create_python_venv(self):
         c.con.log("    Creating Python virtual environment.","info")
         subprocess.run("python -m venv .venv",cwd=self.sub_dir_path,check=True, capture_output=True, text=True)
         install_cfu = "activate.bat & pip install colemen-utils"
         install_pylint = "activate.bat & pip install pylint"
         try:
```

### Comparing `colemen_ra_manager-0.0.4/ramanager/ProjectBase.py` & `colemen_ra_manager-0.0.5/ramanager/ProjectBase.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import time
 
 import colemen_utils as c
 
 import ramanager.settings.types as _t
 import ramanager.settings as _settings
 
-
+from ramanager.TextToSpeech import TextToSpeech
 
 
 @dataclass
 class ProjectBase:
     main:_t.main_type = None
 
     '''A reference to the project manager.'''
@@ -119,14 +119,18 @@
             "description":self.description,
             "timestamp":self.timestamp,
         }
 
 
         return sum_data
 
+    def speak_complete(self):
+        tts = TextToSpeech()
+        tts.speak(f"Project {self.year.cur_year_four[-2:]} {self.project_id} {self.title} has been created.")
+
 
     # @property
     # def file_path(self):
     #     '''
     #         Get this ProjectBase's file_path
 
     #         `default`:None
```

### Comparing `colemen_ra_manager-0.0.4/ramanager/ProjectManager.py` & `colemen_ra_manager-0.0.5/ramanager/ProjectManager.py`

 * *Files identical despite different names*

### Comparing `colemen_ra_manager-0.0.4/ramanager/Year.py` & `colemen_ra_manager-0.0.5/ramanager/Year.py`

 * *Files identical despite different names*

### Comparing `colemen_ra_manager-0.0.4/ramanager/inputs.py` & `colemen_ra_manager-0.0.5/ramanager/inputs.py`

 * *Files identical despite different names*

### Comparing `colemen_ra_manager-0.0.4/ramanager/settings/types.py` & `colemen_ra_manager-0.0.5/ramanager/settings/types.py`

 * *Files identical despite different names*

### Comparing `colemen_ra_manager-0.0.4/setup.py` & `colemen_ra_manager-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from glob import glob
 from setuptools import setup, find_packages
 import colemen_utilities.build_utils.general as _gen
 
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'colemen_ra_manager'
 LONG_DESCRIPTION = 'Refactoring the ra9 project manager into its own library'
 
 
 _root_path = f"{os.getcwd()}/ramanager"
 PY_MODULES = _gen.list_py_modules(
     _root_path,
```

