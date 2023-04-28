# Comparing `tmp/MOMORING-1.3.6.tar.gz` & `tmp/MOMORING-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MOMORING-1.3.6.tar", last modified: Wed Mar 23 03:38:19 2022, max compression
+gzip compressed data, was "MOMORING-1.4.0.tar", last modified: Fri Apr 28 10:25:46 2023, max compression
```

## Comparing `MOMORING-1.3.6.tar` & `MOMORING-1.4.0.tar`

### file list

```diff
@@ -1,35 +1,33 @@
-drwxr-xr-x   0 wenzhi.ma (16777216) domain users (16777216)        0 2022-03-23 03:38:19.539647 MOMORING-1.3.6/
-drwxr-xr-x   0 wenzhi.ma (16777216) domain users (16777216)        0 2022-03-23 03:38:19.539647 MOMORING-1.3.6/MOMORING/
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)        0 2022-03-07 01:24:52.000000 MOMORING-1.3.6/MOMORING/__init__.py
-drwxr-xr-x   0 wenzhi.ma (16777216) domain users (16777216)        0 2022-03-23 03:38:19.539647 MOMORING-1.3.6/MOMORING/api/
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)        0 2022-03-07 01:24:52.000000 MOMORING-1.3.6/MOMORING/api/__init__.py
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)     1772 2022-03-23 03:23:29.000000 MOMORING-1.3.6/MOMORING/api/create_project.py
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)      668 2022-03-07 01:24:52.000000 MOMORING-1.3.6/MOMORING/api/create_test.py
-drwxr-xr-x   0 wenzhi.ma (16777216) domain users (16777216)        0 2022-03-23 03:38:19.539647 MOMORING-1.3.6/MOMORING/applications/
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)        0 2022-03-07 01:24:52.000000 MOMORING-1.3.6/MOMORING/applications/__init__.py
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)      557 2022-03-07 01:24:52.000000 MOMORING-1.3.6/MOMORING/applications/cmd.py
-drwxr-xr-x   0 wenzhi.ma (16777216) domain users (16777216)        0 2022-03-23 03:38:19.539647 MOMORING-1.3.6/MOMORING/modules/
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)        0 2022-03-07 01:24:52.000000 MOMORING-1.3.6/MOMORING/modules/__init__.py
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)      581 2022-03-23 03:37:36.000000 MOMORING-1.3.6/MOMORING/modules/create.py
-drwxr-xr-x   0 wenzhi.ma (16777216) domain users (16777216)        0 2022-03-23 03:38:19.539647 MOMORING-1.3.6/MOMORING/modules/files/
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)        0 2022-03-07 01:24:52.000000 MOMORING-1.3.6/MOMORING/modules/files/__init__.py
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)      354 2022-03-23 03:27:59.000000 MOMORING-1.3.6/MOMORING/modules/files/applications_init_template.py
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)      396 2022-03-07 01:24:52.000000 MOMORING-1.3.6/MOMORING/modules/files/applications_template.py
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)     3820 2022-03-07 01:24:52.000000 MOMORING-1.3.6/MOMORING/modules/files/git_ignore_template.py
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)      523 2022-03-07 01:24:52.000000 MOMORING-1.3.6/MOMORING/modules/files/main_template.py
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)     4040 2022-03-17 05:40:45.000000 MOMORING-1.3.6/MOMORING/modules/files/nitrogen_utils.py
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)     1006 2022-03-07 01:24:52.000000 MOMORING-1.3.6/MOMORING/modules/files/readme_template.py
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)      831 2022-03-07 01:24:52.000000 MOMORING-1.3.6/MOMORING/modules/files/test_template.py
-drwxr-xr-x   0 wenzhi.ma (16777216) domain users (16777216)        0 2022-03-23 03:38:19.539647 MOMORING-1.3.6/MOMORING/utils/
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)        0 2022-03-07 01:24:52.000000 MOMORING-1.3.6/MOMORING/utils/__init__.py
-drwxr-xr-x   0 wenzhi.ma (16777216) domain users (16777216)        0 2022-03-23 03:38:19.539647 MOMORING-1.3.6/MOMORING.egg-info/
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)      227 2022-03-23 03:38:19.000000 MOMORING-1.3.6/MOMORING.egg-info/PKG-INFO
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)      808 2022-03-23 03:38:19.000000 MOMORING-1.3.6/MOMORING.egg-info/SOURCES.txt
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)        1 2022-03-23 03:38:19.000000 MOMORING-1.3.6/MOMORING.egg-info/dependency_links.txt
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)       56 2022-03-23 03:38:19.000000 MOMORING-1.3.6/MOMORING.egg-info/entry_points.txt
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)        6 2022-03-23 03:38:19.000000 MOMORING-1.3.6/MOMORING.egg-info/requires.txt
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)        9 2022-03-23 03:38:19.000000 MOMORING-1.3.6/MOMORING.egg-info/top_level.txt
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)      227 2022-03-23 03:38:19.539647 MOMORING-1.3.6/PKG-INFO
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)      219 2022-03-07 01:24:52.000000 MOMORING-1.3.6/README.md
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)       38 2022-03-23 03:38:19.539647 MOMORING-1.3.6/setup.cfg
--rw-r--r--   0 wenzhi.ma (16777216) domain users (16777216)      411 2022-03-23 03:37:43.000000 MOMORING-1.3.6/setup.py
+drwxr-xr-x   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:25:46.502000 MOMORING-1.4.0/
+drwxr-xr-x   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:25:46.501000 MOMORING-1.4.0/MOMORING/
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:17:32.000000 MOMORING-1.4.0/MOMORING/__init__.py
+drwxr-xr-x   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:25:46.501000 MOMORING-1.4.0/MOMORING/api/
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:17:32.000000 MOMORING-1.4.0/MOMORING/api/__init__.py
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)     1788 2023-04-28 10:24:14.000000 MOMORING-1.4.0/MOMORING/api/create_project.py
+drwxr-xr-x   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:25:46.502000 MOMORING-1.4.0/MOMORING/applications/
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:17:32.000000 MOMORING-1.4.0/MOMORING/applications/__init__.py
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      557 2023-04-28 10:17:32.000000 MOMORING-1.4.0/MOMORING/applications/cmd.py
+drwxr-xr-x   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:25:46.502000 MOMORING-1.4.0/MOMORING/modules/
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:17:32.000000 MOMORING-1.4.0/MOMORING/modules/__init__.py
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      581 2023-04-28 10:17:32.000000 MOMORING-1.4.0/MOMORING/modules/create.py
+drwxr-xr-x   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:25:46.502000 MOMORING-1.4.0/MOMORING/modules/files/
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:17:32.000000 MOMORING-1.4.0/MOMORING/modules/files/__init__.py
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      234 2023-04-28 10:18:01.000000 MOMORING-1.4.0/MOMORING/modules/files/applications_init_template.py
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      118 2023-04-28 10:18:58.000000 MOMORING-1.4.0/MOMORING/modules/files/applications_template.py
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)     1953 2023-04-28 10:20:35.000000 MOMORING-1.4.0/MOMORING/modules/files/git_ignore_template.py
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      523 2023-04-28 10:17:32.000000 MOMORING-1.4.0/MOMORING/modules/files/main_template.py
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)     4040 2023-04-28 10:17:32.000000 MOMORING-1.4.0/MOMORING/modules/files/nitrogen_utils.py
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      447 2023-04-28 10:22:53.000000 MOMORING-1.4.0/MOMORING/modules/files/readme_template.py
+drwxr-xr-x   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:25:46.502000 MOMORING-1.4.0/MOMORING/utils/
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:17:32.000000 MOMORING-1.4.0/MOMORING/utils/__init__.py
+drwxr-xr-x   0 mawenzhi  (7016) stonewise  (1001)        0 2023-04-28 10:25:46.501000 MOMORING-1.4.0/MOMORING.egg-info/
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      149 2023-04-28 10:25:46.000000 MOMORING-1.4.0/MOMORING.egg-info/PKG-INFO
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      740 2023-04-28 10:25:46.000000 MOMORING-1.4.0/MOMORING.egg-info/SOURCES.txt
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        1 2023-04-28 10:25:46.000000 MOMORING-1.4.0/MOMORING.egg-info/dependency_links.txt
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)       55 2023-04-28 10:25:46.000000 MOMORING-1.4.0/MOMORING.egg-info/entry_points.txt
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        6 2023-04-28 10:25:46.000000 MOMORING-1.4.0/MOMORING.egg-info/requires.txt
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)        9 2023-04-28 10:25:46.000000 MOMORING-1.4.0/MOMORING.egg-info/top_level.txt
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      149 2023-04-28 10:25:46.502000 MOMORING-1.4.0/PKG-INFO
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      218 2023-04-28 10:25:13.000000 MOMORING-1.4.0/README.md
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)       38 2023-04-28 10:25:46.503000 MOMORING-1.4.0/setup.cfg
+-rw-r--r--   0 mawenzhi  (7016) stonewise  (1001)      408 2023-04-28 10:24:56.000000 MOMORING-1.4.0/setup.py
```

### Comparing `MOMORING-1.3.6/MOMORING/api/create_project.py` & `MOMORING-1.4.0/MOMORING/api/create_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,21 +21,21 @@
     project_name = os.path.basename(project_name)
     create_python_package(project_name)
 
     dirs = ['applications', 'api', 'modules', 'utils']
     for i in dirs:
         create_python_package(os.path.join(project_name, i))
 
-    nitrogen_utils_path = os.path.join(project_name,
-                                       'utils',
-                                       'nitrogen_utils.py')
-    create_file(nitrogen_utils_path, txt=nitrogen_utils())
-    applications_file_path = os.path.join(project_name,
-                                          'applications',
-                                          'nitrogen_template.py')
-    create_file(applications_file_path, txt=get_applications_template(project_name))
+    # nitrogen_utils_path = os.path.join(project_name,
+    #                                    'utils',
+    #                                    'nitrogen_utils.py')
+    # create_file(nitrogen_utils_path, txt=nitrogen_utils())
+    # applications_file_path = os.path.join(project_name,
+    #                                       'applications',
+    #                                       'nitrogen_template.py')
+    # create_file(applications_file_path, txt=get_applications_template(project_name))
     create_file('main.py', txt=get_main_template())
     create_file('.gitignore', txt=get_git_ignore_template())
     create_file('README.md', txt=get_readme_template(project_name))
 
     create_test_dir('.')
```

### Comparing `MOMORING-1.3.6/MOMORING/applications/cmd.py` & `MOMORING-1.4.0/MOMORING/applications/cmd.py`

 * *Files identical despite different names*

### Comparing `MOMORING-1.3.6/MOMORING/modules/create.py` & `MOMORING-1.4.0/MOMORING/modules/create.py`

 * *Files identical despite different names*

### Comparing `MOMORING-1.3.6/MOMORING/modules/files/git_ignore_template.py` & `MOMORING-1.4.0/MOMORING/modules/files/git_ignore_template.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,143 +1,9 @@
 def get_git_ignore_template():
     txt = '''\
-<<<<<<< HEAD
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
-# Distribution / packaging
-.Python
-build/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-pip-wheel-metadata/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-
-# PyBuilder
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
-# pyenv
-.python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.env
-.venv
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Pyre type checker
-.pyre/
-
-# Pycharm
-.idea/
-=======
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
@@ -267,12 +133,13 @@
 # for test
 test*
 *json
 *example*
 workdir/
 savedpath/
 *dist*
->>>>>>> 0453e51a3eba102a7f0eee0bab675a173e022aac
 /test/
 
+# for Mac
+.DS_Store
 '''
     return txt
```

### Comparing `MOMORING-1.3.6/MOMORING/modules/files/main_template.py` & `MOMORING-1.4.0/MOMORING/modules/files/main_template.py`

 * *Files identical despite different names*

### Comparing `MOMORING-1.3.6/MOMORING/modules/files/nitrogen_utils.py` & `MOMORING-1.4.0/MOMORING/modules/files/nitrogen_utils.py`

 * *Files identical despite different names*

### Comparing `MOMORING-1.3.6/MOMORING.egg-info/SOURCES.txt` & `MOMORING-1.4.0/MOMORING.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,19 @@
 MOMORING.egg-info/SOURCES.txt
 MOMORING.egg-info/dependency_links.txt
 MOMORING.egg-info/entry_points.txt
 MOMORING.egg-info/requires.txt
 MOMORING.egg-info/top_level.txt
 MOMORING/api/__init__.py
 MOMORING/api/create_project.py
-MOMORING/api/create_test.py
 MOMORING/applications/__init__.py
 MOMORING/applications/cmd.py
 MOMORING/modules/__init__.py
 MOMORING/modules/create.py
 MOMORING/modules/files/__init__.py
 MOMORING/modules/files/applications_init_template.py
 MOMORING/modules/files/applications_template.py
 MOMORING/modules/files/git_ignore_template.py
 MOMORING/modules/files/main_template.py
 MOMORING/modules/files/nitrogen_utils.py
 MOMORING/modules/files/readme_template.py
-MOMORING/modules/files/test_template.py
 MOMORING/utils/__init__.py
```

