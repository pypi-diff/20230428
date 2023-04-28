# Comparing `tmp/flask_admin_dashboard-0.0.3.tar.gz` & `tmp/flask_admin_dashboard-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_admin_dashboard-0.0.3.tar", last modified: Thu Apr 27 20:35:08 2023, max compression
+gzip compressed data, was "flask_admin_dashboard-0.0.4.tar", last modified: Thu Apr 27 20:57:51 2023, max compression
```

## Comparing `flask_admin_dashboard-0.0.3.tar` & `flask_admin_dashboard-0.0.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:35:08.157458 flask_admin_dashboard-0.0.3/
--rw-r--r--   0 will      (1000) will      (1000)      311 2023-04-27 20:35:08.157458 flask_admin_dashboard-0.0.3/PKG-INFO
--rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:20:25.000000 flask_admin_dashboard-0.0.3/README.md
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:35:08.157458 flask_admin_dashboard-0.0.3/flask_admin_dashboard/
--rw-r--r--   0 will      (1000) will      (1000)       43 2023-04-27 20:30:54.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard/__init__.py
--rw-r--r--   0 will      (1000) will      (1000)     2225 2023-04-27 20:30:47.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard/admin_dashboard.py
--rw-r--r--   0 will      (1000) will      (1000)     2801 2023-04-26 18:04:44.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard/models.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:35:08.157458 flask_admin_dashboard-0.0.3/flask_admin_dashboard/scripts/
--rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:22:08.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard/scripts/__init__.py
--rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:31:46.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard/scripts/cli.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:35:08.157458 flask_admin_dashboard-0.0.3/flask_admin_dashboard/static/
--rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:21:36.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard/static/__init__.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:35:08.157458 flask_admin_dashboard-0.0.3/flask_admin_dashboard/static/assets/
--rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:21:36.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard/static/assets/__init__.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:35:08.157458 flask_admin_dashboard-0.0.3/flask_admin_dashboard/static/css/
--rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:21:36.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard/static/css/__init__.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:35:08.157458 flask_admin_dashboard-0.0.3/flask_admin_dashboard/static/js/
--rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:21:36.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard/static/js/__init__.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:35:08.157458 flask_admin_dashboard-0.0.3/flask_admin_dashboard/storages/
--rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:22:23.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard/storages/__init__.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:35:08.157458 flask_admin_dashboard-0.0.3/flask_admin_dashboard/templates/
--rw-r--r--   0 will      (1000) will      (1000)       45 2023-04-27 19:48:54.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard/templates/__init__.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:35:08.157458 flask_admin_dashboard-0.0.3/flask_admin_dashboard/templates/admin/
--rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:35:52.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard/templates/admin/__init__.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:35:08.157458 flask_admin_dashboard-0.0.3/flask_admin_dashboard/templates/security/
--rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:35:46.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard/templates/security/__init__.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:35:08.157458 flask_admin_dashboard-0.0.3/flask_admin_dashboard/utilities/
--rw-r--r--   0 will      (1000) will      (1000)       45 2023-04-27 19:48:38.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard/utilities/__init__.py
--rw-r--r--   0 will      (1000) will      (1000)     3179 2022-06-15 20:05:15.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard/utilities/cache.py
--rw-r--r--   0 will      (1000) will      (1000)     2230 2022-07-22 00:01:05.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard/utilities/jsonhandler.py
--rw-r--r--   0 will      (1000) will      (1000)      648 2022-12-01 19:01:53.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard/utilities/timehandler.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:35:08.157458 flask_admin_dashboard-0.0.3/flask_admin_dashboard/views/
--rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:35:14.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard/views/__init__.py
--rw-r--r--   0 will      (1000) will      (1000)     1709 2023-04-26 18:41:49.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard/views/admin.py
--rw-r--r--   0 will      (1000) will      (1000)     4034 2023-04-26 20:07:54.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard/views/auth.py
--rw-r--r--   0 will      (1000) will      (1000)      843 2023-01-03 17:13:42.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard/views/logs.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:35:08.157458 flask_admin_dashboard-0.0.3/flask_admin_dashboard.egg-info/
--rw-r--r--   0 will      (1000) will      (1000)      311 2023-04-27 20:35:08.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard.egg-info/PKG-INFO
--rw-r--r--   0 will      (1000) will      (1000)     1172 2023-04-27 20:35:08.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 will      (1000) will      (1000)        1 2023-04-27 20:35:08.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 will      (1000) will      (1000)       65 2023-04-27 20:35:08.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard.egg-info/entry_points.txt
--rw-r--r--   0 will      (1000) will      (1000)      276 2023-04-27 20:35:08.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard.egg-info/requires.txt
--rw-r--r--   0 will      (1000) will      (1000)       22 2023-04-27 20:35:08.000000 flask_admin_dashboard-0.0.3/flask_admin_dashboard.egg-info/top_level.txt
--rw-r--r--   0 will      (1000) will      (1000)       38 2023-04-27 20:35:08.157458 flask_admin_dashboard-0.0.3/setup.cfg
--rw-r--r--   0 will      (1000) will      (1000)     1232 2023-04-27 20:35:03.000000 flask_admin_dashboard-0.0.3/setup.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:57:51.387466 flask_admin_dashboard-0.0.4/
+-rw-r--r--   0 will      (1000) will      (1000)      311 2023-04-27 20:57:51.387466 flask_admin_dashboard-0.0.4/PKG-INFO
+-rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:20:25.000000 flask_admin_dashboard-0.0.4/README.md
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:57:51.387466 flask_admin_dashboard-0.0.4/flask_admin_dashboard/
+-rw-r--r--   0 will      (1000) will      (1000)       43 2023-04-27 20:30:54.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard/__init__.py
+-rw-r--r--   0 will      (1000) will      (1000)     2669 2023-04-27 20:57:24.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard/admin_dashboard.py
+-rw-r--r--   0 will      (1000) will      (1000)     2801 2023-04-26 18:04:44.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard/models.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:57:51.387466 flask_admin_dashboard-0.0.4/flask_admin_dashboard/scripts/
+-rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:22:08.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard/scripts/__init__.py
+-rw-r--r--   0 will      (1000) will      (1000)      610 2023-04-27 20:48:59.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard/scripts/cli.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:57:51.387466 flask_admin_dashboard-0.0.4/flask_admin_dashboard/static/
+-rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:21:36.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard/static/__init__.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:57:51.387466 flask_admin_dashboard-0.0.4/flask_admin_dashboard/static/assets/
+-rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:21:36.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard/static/assets/__init__.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:57:51.387466 flask_admin_dashboard-0.0.4/flask_admin_dashboard/static/css/
+-rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:21:36.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard/static/css/__init__.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:57:51.387466 flask_admin_dashboard-0.0.4/flask_admin_dashboard/static/js/
+-rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:21:36.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard/static/js/__init__.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:57:51.387466 flask_admin_dashboard-0.0.4/flask_admin_dashboard/storages/
+-rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:22:23.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard/storages/__init__.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:57:51.387466 flask_admin_dashboard-0.0.4/flask_admin_dashboard/templates/
+-rw-r--r--   0 will      (1000) will      (1000)       45 2023-04-27 19:48:54.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard/templates/__init__.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:57:51.387466 flask_admin_dashboard-0.0.4/flask_admin_dashboard/templates/admin/
+-rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:35:52.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard/templates/admin/__init__.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:57:51.387466 flask_admin_dashboard-0.0.4/flask_admin_dashboard/templates/security/
+-rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:35:46.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard/templates/security/__init__.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:57:51.387466 flask_admin_dashboard-0.0.4/flask_admin_dashboard/utilities/
+-rw-r--r--   0 will      (1000) will      (1000)       45 2023-04-27 19:48:38.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard/utilities/__init__.py
+-rw-r--r--   0 will      (1000) will      (1000)     3179 2022-06-15 20:05:15.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard/utilities/cache.py
+-rw-r--r--   0 will      (1000) will      (1000)     2230 2022-07-22 00:01:05.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard/utilities/jsonhandler.py
+-rw-r--r--   0 will      (1000) will      (1000)      648 2022-12-01 19:01:53.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard/utilities/timehandler.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:57:51.387466 flask_admin_dashboard-0.0.4/flask_admin_dashboard/views/
+-rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:35:14.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard/views/__init__.py
+-rw-r--r--   0 will      (1000) will      (1000)     1709 2023-04-26 18:41:49.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard/views/admin.py
+-rw-r--r--   0 will      (1000) will      (1000)     4034 2023-04-26 20:07:54.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard/views/auth.py
+-rw-r--r--   0 will      (1000) will      (1000)      843 2023-01-03 17:13:42.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard/views/logs.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-04-27 20:57:51.387466 flask_admin_dashboard-0.0.4/flask_admin_dashboard.egg-info/
+-rw-r--r--   0 will      (1000) will      (1000)      311 2023-04-27 20:57:51.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 will      (1000) will      (1000)     1172 2023-04-27 20:57:51.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 will      (1000) will      (1000)        1 2023-04-27 20:57:51.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 will      (1000) will      (1000)       65 2023-04-27 20:57:51.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard.egg-info/entry_points.txt
+-rw-r--r--   0 will      (1000) will      (1000)      283 2023-04-27 20:57:51.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard.egg-info/requires.txt
+-rw-r--r--   0 will      (1000) will      (1000)       22 2023-04-27 20:57:51.000000 flask_admin_dashboard-0.0.4/flask_admin_dashboard.egg-info/top_level.txt
+-rw-r--r--   0 will      (1000) will      (1000)       38 2023-04-27 20:57:51.387466 flask_admin_dashboard-0.0.4/setup.cfg
+-rw-r--r--   0 will      (1000) will      (1000)     1251 2023-04-27 20:57:30.000000 flask_admin_dashboard-0.0.4/setup.py
```

### Comparing `flask_admin_dashboard-0.0.3/flask_admin_dashboard/admin_dashboard.py` & `flask_admin_dashboard-0.0.4/flask_admin_dashboard/admin_dashboard.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,22 @@
+import os, shutil
 from flask_admin import Admin
 from flask_security import Security, SQLAlchemySessionUserDatastore
 from .views.admin import AdminView
 from .views.auth import ExtendedLoginForm, LogoutMenuLink
 from pathlib import Path
 from flask_admin_dashboard.models import db, migrate, User, Role, UserView, RoleView
 
 user_datastore = SQLAlchemySessionUserDatastore(db.session, User, Role)
 BASE_DIR = Path(__file__).parent.parent.parent.parent.parent.parent.resolve()
 BASE_CONFIG_DIR = Path.joinpath(BASE_DIR, 'config')
 PACKAGE_DIR = Path(__file__).parent.resolve()
+LOGS_DIR = Path.joinpath(BASE_DIR, 'logs')
+
+
 
 class AdminDashboard(Admin):
 
     def __init__(self, app):
         db.app = app
         db.init_app(app)
         migrate.init_app(app, db, render_as_batch=True)
@@ -28,18 +32,26 @@
 
     @staticmethod
     def setup_user():
         role = user_datastore.find_role('SUPER_USER')
         if role is None:
             user_datastore.create_role(name='SUPER_USER', description='Super user access.')
             role = user_datastore.find_role('SUPER_USER')
-        user_datastore.create_user(username='will', password='test')
+        user_datastore.create_user(username='will', password="test")
         user = user_datastore.find_user(username='will')
         # role = user_datastore.find_role('SUPER_USER')
         user_datastore.add_role_to_user(user, role)
         db.session.commit()
 
-    def initialize_admin(self):
+    @staticmethod
+    def initialize_admin():
+        if not os.path.exists(LOGS_DIR):
+            os.makedirs(LOGS_DIR)
         templates_src = Path.joinpath(Path(PACKAGE_DIR), f'templates')
         templates_dst = Path.joinpath(Path(BASE_DIR), f'templates')
         shutil.copytree(templates_src, templates_dst, symlinks=True, ignore=None, ignore_dangling_symlinks=False,
                         dirs_exist_ok=True)
+
+        static_src = Path.joinpath(Path(PACKAGE_DIR), f'static')
+        static_dst = Path.joinpath(Path(BASE_DIR), f'static')
+        shutil.copytree(static_src, static_dst, symlinks=True, ignore=None, ignore_dangling_symlinks=False,
+                        dirs_exist_ok=True)
```

### Comparing `flask_admin_dashboard-0.0.3/flask_admin_dashboard/models.py` & `flask_admin_dashboard-0.0.4/flask_admin_dashboard/models.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-0.0.3/flask_admin_dashboard/utilities/cache.py` & `flask_admin_dashboard-0.0.4/flask_admin_dashboard/utilities/cache.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-0.0.3/flask_admin_dashboard/utilities/jsonhandler.py` & `flask_admin_dashboard-0.0.4/flask_admin_dashboard/utilities/jsonhandler.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-0.0.3/flask_admin_dashboard/utilities/timehandler.py` & `flask_admin_dashboard-0.0.4/flask_admin_dashboard/utilities/timehandler.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-0.0.3/flask_admin_dashboard/views/admin.py` & `flask_admin_dashboard-0.0.4/flask_admin_dashboard/views/admin.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-0.0.3/flask_admin_dashboard/views/auth.py` & `flask_admin_dashboard-0.0.4/flask_admin_dashboard/views/auth.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-0.0.3/flask_admin_dashboard/views/logs.py` & `flask_admin_dashboard-0.0.4/flask_admin_dashboard/views/logs.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-0.0.3/flask_admin_dashboard.egg-info/SOURCES.txt` & `flask_admin_dashboard-0.0.4/flask_admin_dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-0.0.3/setup.py` & `flask_admin_dashboard-0.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='flask_admin_dashboard',
-    version='0.0.3',
+    version='0.0.4',
     description='Admin Dashboard for Flask',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/theapiguys/flask_admin_dashboard',
     readme="README.md",
     author='Will @ TheAPIGuys',
     author_email='will@theapiguys.com',
@@ -26,15 +26,16 @@
         "SQLAlchemy-serializer==1.4.1",
         "Flask-WTF==1.0.1",
         "WTForms==3.0.1",
         "Flask-Login==0.6.2",
         "Flask-Mail==0.9.1",
         "Flask-Migrate==4.0.4",
         "Flask-Principal==0.4.0",
-        "pytz"
+        "pytz",
+        "shutil"
     ],
     entry_points={
         'console_scripts': [
             'admin = flask_admin_dashboard.scripts.cli:cli',
         ],
 
     },
```

