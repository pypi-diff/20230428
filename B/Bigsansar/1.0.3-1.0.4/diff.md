# Comparing `tmp/Bigsansar-1.0.3.tar.gz` & `tmp/Bigsansar-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bigsansar-1.0.3.tar", last modified: Fri Apr 28 15:27:49 2023, max compression
+gzip compressed data, was "Bigsansar-1.0.4.tar", last modified: Fri Apr 28 15:32:00 2023, max compression
```

## Comparing `Bigsansar-1.0.3.tar` & `Bigsansar-1.0.4.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 15:27:49.356951 Bigsansar-1.0.3/
-drwxrwxrwx   0        0        0        0 2023-04-28 15:27:49.191627 Bigsansar-1.0.3/Bigsansar.egg-info/
--rw-rw-rw-   0        0        0     2934 2023-04-28 15:27:48.000000 Bigsansar-1.0.3/Bigsansar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2254 2023-04-28 15:27:49.000000 Bigsansar-1.0.3/Bigsansar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 15:27:48.000000 Bigsansar-1.0.3/Bigsansar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-28 15:27:48.000000 Bigsansar-1.0.3/Bigsansar.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       82 2023-04-28 15:27:48.000000 Bigsansar-1.0.3/Bigsansar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-28 15:27:48.000000 Bigsansar-1.0.3/Bigsansar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     2934 2023-04-28 15:27:49.356951 Bigsansar-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2243 2023-04-28 15:17:28.000000 Bigsansar-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 15:27:49.216825 Bigsansar-1.0.3/bigsansar/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/__init__.py
--rw-rw-rw-   0        0        0       66 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/admin.py
--rw-rw-rw-   0        0        0      195 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-28 15:27:49.219076 Bigsansar-1.0.3/bigsansar/contrib/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 15:27:49.239320 Bigsansar-1.0.3/bigsansar/contrib/account/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/account/__init__.py
--rw-rw-rw-   0        0        0      510 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/account/admin.py
--rw-rw-rw-   0        0        0      284 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/account/apps.py
--rw-rw-rw-   0        0        0     1176 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/account/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-28 15:27:49.248797 Bigsansar-1.0.3/bigsansar/contrib/account/migrations/
--rw-rw-rw-   0        0        0      999 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/account/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      417 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/account/migrations/__init__.py
--rw-rw-rw-   0        0        0      556 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/account/models.py
--rw-rw-rw-   0        0        0      351 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/account/signals.py
-drwxrwxrwx   0        0        0        0 2023-04-28 15:27:49.250128 Bigsansar-1.0.3/bigsansar/contrib/account/templates/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/account/templates/__init__.py
--rw-rw-rw-   0        0        0       63 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/account/tests.py
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/account/urls.py
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/account/views.py
-drwxrwxrwx   0        0        0        0 2023-04-28 15:27:49.263573 Bigsansar-1.0.3/bigsansar/contrib/blogs/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/blogs/__init__.py
--rw-rw-rw-   0        0        0      541 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/blogs/admin.py
--rw-rw-rw-   0        0        0      195 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/blogs/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-28 15:27:49.269854 Bigsansar-1.0.3/bigsansar/contrib/blogs/migrations/
--rw-rw-rw-   0        0        0     2272 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/blogs/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/blogs/migrations/__init__.py
--rw-rw-rw-   0        0        0     1572 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/blogs/models.py
--rw-rw-rw-   0        0        0       63 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/blogs/tests.py
--rw-rw-rw-   0        0        0       66 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/blogs/views.py
-drwxrwxrwx   0        0        0        0 2023-04-28 15:27:49.287366 Bigsansar-1.0.3/bigsansar/contrib/sites/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/sites/__init__.py
--rw-rw-rw-   0        0        0     1734 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/sites/admin.py
--rw-rw-rw-   0        0        0      203 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/sites/apps.py
--rw-rw-rw-   0        0        0     3018 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/sites/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-28 15:27:49.294036 Bigsansar-1.0.3/bigsansar/contrib/sites/migrations/
--rw-rw-rw-   0        0        0     1816 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/sites/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/sites/migrations/__init__.py
--rw-rw-rw-   0        0        0     1826 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/sites/models.py
-drwxrwxrwx   0        0        0        0 2023-04-28 15:27:49.294036 Bigsansar-1.0.3/bigsansar/contrib/sites/templatetags/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/sites/templatetags/__init__.py
--rw-rw-rw-   0        0        0      408 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/sites/templatetags/pages.py
--rw-rw-rw-   0        0        0       63 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/sites/tests.py
--rw-rw-rw-   0        0        0       66 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/contrib/sites/views.py
-drwxrwxrwx   0        0        0        0 2023-04-28 15:27:49.307520 Bigsansar-1.0.3/bigsansar/core/
--rw-rw-rw-   0        0        0      524 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/core/__init__.py
--rw-rw-rw-   0        0        0      414 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/core/host.py
--rw-rw-rw-   0        0        0     7281 2023-04-27 14:17:52.000000 Bigsansar-1.0.3/bigsansar/core/init.py
--rw-rw-rw-   0        0        0       27 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/main.py
-drwxrwxrwx   0        0        0        0 2023-04-28 15:27:49.311362 Bigsansar-1.0.3/bigsansar/management/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 15:27:49.315574 Bigsansar-1.0.3/bigsansar/management/commands/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/management/commands/__init__.py
--rw-rw-rw-   0        0        0     1122 2023-04-27 12:44:33.000000 Bigsansar-1.0.3/bigsansar/management/commands/createuser.py
-drwxrwxrwx   0        0        0        0 2023-04-28 15:27:49.320600 Bigsansar-1.0.3/bigsansar/migrations/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/migrations/__init__.py
--rw-rw-rw-   0        0        0       60 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/models.py
-drwxrwxrwx   0        0        0        0 2023-04-28 15:27:49.329544 Bigsansar-1.0.3/bigsansar/static/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/static/__init__.py
--rw-rw-rw-   0        0        0     9230 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/static/logo.png
--rw-rw-rw-   0        0        0      525 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/static/style.css
-drwxrwxrwx   0        0        0        0 2023-04-28 15:27:49.356951 Bigsansar-1.0.3/bigsansar/templates/
--rw-rw-rw-   0        0        0      977 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/templates/404.html
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/templates/__init__.py
--rw-rw-rw-   0        0        0      168 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/templates/acc_active_email.html
--rw-rw-rw-   0        0        0     1134 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/templates/base.html
--rw-rw-rw-   0        0        0     2252 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/templates/default.html
--rw-rw-rw-   0        0        0     2250 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/templates/defaultpage.html
--rw-rw-rw-   0        0        0     2171 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/templates/nav.html
--rw-rw-rw-   0        0        0      758 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/templates/parking.html
--rw-rw-rw-   0        0        0       63 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/tests.py
--rw-rw-rw-   0        0        0      821 2023-04-27 12:27:15.000000 Bigsansar-1.0.3/bigsansar/urls.py
--rw-rw-rw-   0        0        0     1846 2023-04-28 15:25:56.000000 Bigsansar-1.0.3/bigsansar/views.py
--rw-rw-rw-   0        0        0       42 2023-04-28 15:27:49.366470 Bigsansar-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1294 2023-04-28 15:27:03.000000 Bigsansar-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:32:00.579005 Bigsansar-1.0.4/
+drwxrwxrwx   0        0        0        0 2023-04-28 15:32:00.413587 Bigsansar-1.0.4/Bigsansar.egg-info/
+-rw-rw-rw-   0        0        0     2934 2023-04-28 15:32:00.000000 Bigsansar-1.0.4/Bigsansar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2254 2023-04-28 15:32:00.000000 Bigsansar-1.0.4/Bigsansar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 15:32:00.000000 Bigsansar-1.0.4/Bigsansar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-04-28 15:32:00.000000 Bigsansar-1.0.4/Bigsansar.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       82 2023-04-28 15:32:00.000000 Bigsansar-1.0.4/Bigsansar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-28 15:32:00.000000 Bigsansar-1.0.4/Bigsansar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2934 2023-04-28 15:32:00.579005 Bigsansar-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2243 2023-04-28 15:17:28.000000 Bigsansar-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 15:32:00.436084 Bigsansar-1.0.4/bigsansar/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/admin.py
+-rw-rw-rw-   0        0        0      195 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:32:00.436084 Bigsansar-1.0.4/bigsansar/contrib/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:32:00.462819 Bigsansar-1.0.4/bigsansar/contrib/account/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/account/__init__.py
+-rw-rw-rw-   0        0        0      510 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/account/admin.py
+-rw-rw-rw-   0        0        0      284 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/account/apps.py
+-rw-rw-rw-   0        0        0     1176 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/account/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:32:00.471619 Bigsansar-1.0.4/bigsansar/contrib/account/migrations/
+-rw-rw-rw-   0        0        0      999 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/account/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      417 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/account/migrations/__init__.py
+-rw-rw-rw-   0        0        0      556 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/account/models.py
+-rw-rw-rw-   0        0        0      351 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/account/signals.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:32:00.474622 Bigsansar-1.0.4/bigsansar/contrib/account/templates/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/account/templates/__init__.py
+-rw-rw-rw-   0        0        0       63 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/account/tests.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/account/urls.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/account/views.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:32:00.489296 Bigsansar-1.0.4/bigsansar/contrib/blogs/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/blogs/__init__.py
+-rw-rw-rw-   0        0        0      541 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/blogs/admin.py
+-rw-rw-rw-   0        0        0      195 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/blogs/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:32:00.493582 Bigsansar-1.0.4/bigsansar/contrib/blogs/migrations/
+-rw-rw-rw-   0        0        0     2272 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/blogs/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/blogs/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1572 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/blogs/models.py
+-rw-rw-rw-   0        0        0       63 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/blogs/tests.py
+-rw-rw-rw-   0        0        0       66 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/blogs/views.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:32:00.513229 Bigsansar-1.0.4/bigsansar/contrib/sites/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/sites/__init__.py
+-rw-rw-rw-   0        0        0     1734 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/sites/admin.py
+-rw-rw-rw-   0        0        0      203 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/sites/apps.py
+-rw-rw-rw-   0        0        0     3018 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/sites/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:32:00.517657 Bigsansar-1.0.4/bigsansar/contrib/sites/migrations/
+-rw-rw-rw-   0        0        0     1816 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/sites/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/sites/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1826 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/sites/models.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:32:00.525891 Bigsansar-1.0.4/bigsansar/contrib/sites/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/sites/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      408 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/sites/templatetags/pages.py
+-rw-rw-rw-   0        0        0       63 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/sites/tests.py
+-rw-rw-rw-   0        0        0       66 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/contrib/sites/views.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:32:00.533599 Bigsansar-1.0.4/bigsansar/core/
+-rw-rw-rw-   0        0        0      524 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/core/__init__.py
+-rw-rw-rw-   0        0        0      414 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/core/host.py
+-rw-rw-rw-   0        0        0     7281 2023-04-27 14:17:52.000000 Bigsansar-1.0.4/bigsansar/core/init.py
+-rw-rw-rw-   0        0        0       27 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/main.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:32:00.536318 Bigsansar-1.0.4/bigsansar/management/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:32:00.538626 Bigsansar-1.0.4/bigsansar/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     1122 2023-04-27 12:44:33.000000 Bigsansar-1.0.4/bigsansar/management/commands/createuser.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:32:00.543201 Bigsansar-1.0.4/bigsansar/migrations/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/migrations/__init__.py
+-rw-rw-rw-   0        0        0       60 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/models.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:32:00.551289 Bigsansar-1.0.4/bigsansar/static/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/static/__init__.py
+-rw-rw-rw-   0        0        0     9230 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/static/logo.png
+-rw-rw-rw-   0        0        0      525 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/static/style.css
+drwxrwxrwx   0        0        0        0 2023-04-28 15:32:00.576270 Bigsansar-1.0.4/bigsansar/templates/
+-rw-rw-rw-   0        0        0      977 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/templates/404.html
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/templates/__init__.py
+-rw-rw-rw-   0        0        0      168 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/templates/acc_active_email.html
+-rw-rw-rw-   0        0        0     1134 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/templates/base.html
+-rw-rw-rw-   0        0        0     2252 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/templates/default.html
+-rw-rw-rw-   0        0        0     2250 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/templates/defaultpage.html
+-rw-rw-rw-   0        0        0     2171 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/templates/nav.html
+-rw-rw-rw-   0        0        0      758 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/templates/parking.html
+-rw-rw-rw-   0        0        0       63 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/tests.py
+-rw-rw-rw-   0        0        0      821 2023-04-27 12:27:15.000000 Bigsansar-1.0.4/bigsansar/urls.py
+-rw-rw-rw-   0        0        0     1864 2023-04-28 15:30:13.000000 Bigsansar-1.0.4/bigsansar/views.py
+-rw-rw-rw-   0        0        0       42 2023-04-28 15:32:00.582347 Bigsansar-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1294 2023-04-28 15:31:55.000000 Bigsansar-1.0.4/setup.py
```

### Comparing `Bigsansar-1.0.3/Bigsansar.egg-info/PKG-INFO` & `Bigsansar-1.0.4/Bigsansar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 1.0.3
+Version: 1.0.4
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://bigsansar.com
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
 Keywords: python,django host,bigsansar,django,django sites framework,django flatpages
```

### Comparing `Bigsansar-1.0.3/Bigsansar.egg-info/SOURCES.txt` & `Bigsansar-1.0.4/Bigsansar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.3/LICENSE` & `Bigsansar-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.3/PKG-INFO` & `Bigsansar-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 1.0.3
+Version: 1.0.4
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://bigsansar.com
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
 Keywords: python,django host,bigsansar,django,django sites framework,django flatpages
```

### Comparing `Bigsansar-1.0.3/README.md` & `Bigsansar-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.3/bigsansar/contrib/account/forms.py` & `Bigsansar-1.0.4/bigsansar/contrib/account/forms.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.3/bigsansar/contrib/account/migrations/0001_initial.py` & `Bigsansar-1.0.4/bigsansar/contrib/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.3/bigsansar/contrib/account/models.py` & `Bigsansar-1.0.4/bigsansar/contrib/account/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.3/bigsansar/contrib/blogs/admin.py` & `Bigsansar-1.0.4/bigsansar/contrib/blogs/admin.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.3/bigsansar/contrib/blogs/migrations/0001_initial.py` & `Bigsansar-1.0.4/bigsansar/contrib/blogs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.3/bigsansar/contrib/blogs/models.py` & `Bigsansar-1.0.4/bigsansar/contrib/blogs/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.3/bigsansar/contrib/sites/admin.py` & `Bigsansar-1.0.4/bigsansar/contrib/sites/admin.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.3/bigsansar/contrib/sites/forms.py` & `Bigsansar-1.0.4/bigsansar/contrib/sites/forms.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.3/bigsansar/contrib/sites/migrations/0001_initial.py` & `Bigsansar-1.0.4/bigsansar/contrib/sites/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.3/bigsansar/contrib/sites/models.py` & `Bigsansar-1.0.4/bigsansar/contrib/sites/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.3/bigsansar/core/__init__.py` & `Bigsansar-1.0.4/bigsansar/core/__init__.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.3/bigsansar/core/init.py` & `Bigsansar-1.0.4/bigsansar/core/init.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.3/bigsansar/management/commands/createuser.py` & `Bigsansar-1.0.4/bigsansar/management/commands/createuser.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.3/bigsansar/static/logo.png` & `Bigsansar-1.0.4/bigsansar/static/logo.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.3/bigsansar/static/style.css` & `Bigsansar-1.0.4/bigsansar/static/style.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.3/bigsansar/templates/404.html` & `Bigsansar-1.0.4/bigsansar/templates/404.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.3/bigsansar/templates/base.html` & `Bigsansar-1.0.4/bigsansar/templates/base.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.3/bigsansar/templates/default.html` & `Bigsansar-1.0.4/bigsansar/templates/default.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.3/bigsansar/templates/defaultpage.html` & `Bigsansar-1.0.4/bigsansar/templates/defaultpage.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.3/bigsansar/templates/nav.html` & `Bigsansar-1.0.4/bigsansar/templates/nav.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.3/bigsansar/templates/parking.html` & `Bigsansar-1.0.4/bigsansar/templates/parking.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.3/bigsansar/urls.py` & `Bigsansar-1.0.4/bigsansar/urls.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.3/bigsansar/views.py` & `Bigsansar-1.0.4/bigsansar/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     except:
         current_site = get_current_site(request)
         time = datetime.datetime.now()
         return render(request, 'parking.html', {'domain': current_site, 'time': time})
 
     else:
-        asp = '/' + str(db.id) + '/' + 'index.html'
+        asp = 'templates/' + str(db.id) + '/' + 'index.html'
         full_url = os.path.join(BASE_DIR, asp)
         template = loader.select_template((full_url, DEFAULT_TEMPLATE))
 
         return HttpResponse(template.render({}, request))
 
 
 def pathviews(request, url):
@@ -46,11 +46,11 @@
         pages.objects.filter(domain=db, slug=get_pagename).update(visitor=pagetotal)
 
     except:
 
         return render(request, '404.html')
 
     else:
-        asp = '/' + str(db.id) + '/' + page.slug + '.html'
+        asp = 'templates/' + str(db.id) + '/' + page.slug + '.html'
         full_url = os.path.join(BASE_DIR, asp)
         template = loader.select_template((full_url, default_page))
         return HttpResponse(template.render({'path': url}, request))
```

### Comparing `Bigsansar-1.0.3/setup.py` & `Bigsansar-1.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Bigsansar",
-    version="1.0.3",
+    version="1.0.4",
     author="Bikash Pokhrel",
     author_email="bigsansaroffice@gmail.com",
     description="Build one in minutes with bigsansar - a visual site building tool!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bigsansar.com",
     project_urls={
```

