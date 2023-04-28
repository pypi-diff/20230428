# Comparing `tmp/PyNyaaTa-202304261143.tar.gz` & `tmp/PyNyaaTa-202304270737.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNyaaTa-202304261143.tar", last modified: Wed Apr 26 11:43:59 2023, max compression
+gzip compressed data, was "PyNyaaTa-202304270737.tar", last modified: Thu Apr 27 07:37:51 2023, max compression
```

## Comparing `PyNyaaTa-202304261143.tar` & `PyNyaaTa-202304270737.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:43:59.127402 PyNyaaTa-202304261143/
--rw-r--r--   0 root         (0) root         (0)      474 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      151 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3080 2023-04-26 11:43:59.127402 PyNyaaTa-202304261143/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:43:59.047403 PyNyaaTa-202304261143/PyNyaaTa.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3080 2023-04-26 11:43:58.000000 PyNyaaTa-202304261143/PyNyaaTa.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1635 2023-04-26 11:43:58.000000 PyNyaaTa-202304261143/PyNyaaTa.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 11:43:58.000000 PyNyaaTa-202304261143/PyNyaaTa.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-04-26 11:43:58.000000 PyNyaaTa-202304261143/PyNyaaTa.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      263 2023-04-26 11:43:58.000000 PyNyaaTa-202304261143/PyNyaaTa.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-26 11:43:58.000000 PyNyaaTa-202304261143/PyNyaaTa.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2659 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/README.md
--rw-r--r--   0 root         (0) root         (0)      594 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/get404.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:43:59.047403 PyNyaaTa-202304261143/pynyaata/
--rw-r--r--   0 root         (0) root         (0)     8740 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2032 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:43:59.047403 PyNyaaTa-202304261143/pynyaata/connectors/
--rw-r--r--   0 root         (0) root         (0)      699 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/connectors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3895 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/connectors/animeultime.py
--rw-r--r--   0 root         (0) root         (0)     4059 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/connectors/core.py
--rw-r--r--   0 root         (0) root         (0)     3133 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/connectors/nyaa.py
--rw-r--r--   0 root         (0) root         (0)     3594 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/connectors/yggtorrent.py
--rw-r--r--   0 root         (0) root         (0)     2295 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/flarerequests.py
--rw-r--r--   0 root         (0) root         (0)     1092 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/forms.py
--rw-r--r--   0 root         (0) root         (0)     1100 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:43:59.027403 PyNyaaTa-202304261143/pynyaata/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:43:59.083403 PyNyaaTa-202304261143/pynyaata/static/css/
--rw-r--r--   0 root         (0) root         (0)    59028 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/static/css/bulma-prefers-dark.css.map
--rw-r--r--   0 root         (0) root         (0)   172028 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/static/css/bulma-prefers-dark.min.css
--rw-r--r--   0 root         (0) root         (0)    66189 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/static/css/bulma-tooltip.min.css
--rw-r--r--   0 root         (0) root         (0)    98250 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/static/css/bulma.css.map
--rw-r--r--   0 root         (0) root         (0)   206620 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/static/css/bulma.min.css
--rw-r--r--   0 root         (0) root         (0)    21778 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/static/css/font-awesome.css.map
--rw-r--r--   0 root         (0) root         (0)    31000 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/static/css/font-awesome.min.css
--rw-r--r--   0 root         (0) root         (0)     2415 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/static/css/styles.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:43:59.087403 PyNyaaTa-202304261143/pynyaata/static/favicons/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/static/favicons/animeultime.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/static/favicons/blank.png
--rw-r--r--   0 root         (0) root         (0)   137750 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/static/favicons/favicon.ico
--rw-r--r--   0 root         (0) root         (0)     2001 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/static/favicons/nyaa.png
--rw-r--r--   0 root         (0) root         (0)     3107 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/static/favicons/pantsu.png
--rw-r--r--   0 root         (0) root         (0)     3046 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/static/favicons/yggtorrent.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:43:59.111402 PyNyaaTa-202304261143/pynyaata/static/fonts/
--rw-r--r--   0 root         (0) root         (0)   134808 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/static/fonts/FontAwesome.otf
--rw-r--r--   0 root         (0) root         (0)   165742 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/static/fonts/fontawesome-webfont.eot
--rw-r--r--   0 root         (0) root         (0)   444379 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/static/fonts/fontawesome-webfont.svg
--rw-r--r--   0 root         (0) root         (0)   165548 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/static/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 root         (0) root         (0)    98024 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/static/fonts/fontawesome-webfont.woff
--rw-r--r--   0 root         (0) root         (0)    77160 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/static/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:43:59.119402 PyNyaaTa-202304261143/pynyaata/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:43:59.123402 PyNyaaTa-202304261143/pynyaata/templates/admin/
--rw-r--r--   0 root         (0) root         (0)     4378 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/templates/admin/edit.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:43:59.123402 PyNyaaTa-202304261143/pynyaata/templates/admin/folder/
--rw-r--r--   0 root         (0) root         (0)     1007 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/templates/admin/folder/edit.html
--rw-r--r--   0 root         (0) root         (0)     1673 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/templates/admin/folder/list.html
--rw-r--r--   0 root         (0) root         (0)     3431 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/templates/admin/list.html
--rw-r--r--   0 root         (0) root         (0)     2624 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/templates/latest.html
--rw-r--r--   0 root         (0) root         (0)     4617 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/templates/layout.html
--rw-r--r--   0 root         (0) root         (0)     1454 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/templates/list.html
--rw-r--r--   0 root         (0) root         (0)     3032 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/templates/search.html
--rw-r--r--   0 root         (0) root         (0)     1142 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/pynyaata/utils.py
--rw-r--r--   0 root         (0) root         (0)      263 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/run.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 11:43:59.127402 PyNyaaTa-202304261143/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      961 2023-04-26 11:40:54.000000 PyNyaaTa-202304261143/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:37:51.020430 PyNyaaTa-202304270737/
+-rw-r--r--   0 root         (0) root         (0)      474 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      151 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3080 2023-04-27 07:37:51.020430 PyNyaaTa-202304270737/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:37:50.896431 PyNyaaTa-202304270737/PyNyaaTa.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3080 2023-04-27 07:37:50.000000 PyNyaaTa-202304270737/PyNyaaTa.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-04-27 07:37:50.000000 PyNyaaTa-202304270737/PyNyaaTa.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 07:37:50.000000 PyNyaaTa-202304270737/PyNyaaTa.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-04-27 07:37:50.000000 PyNyaaTa-202304270737/PyNyaaTa.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      263 2023-04-27 07:37:50.000000 PyNyaaTa-202304270737/PyNyaaTa.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-27 07:37:50.000000 PyNyaaTa-202304270737/PyNyaaTa.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2659 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/README.md
+-rw-r--r--   0 root         (0) root         (0)      594 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/get404.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:37:50.908431 PyNyaaTa-202304270737/pynyaata/
+-rw-r--r--   0 root         (0) root         (0)     8740 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:37:50.928431 PyNyaaTa-202304270737/pynyaata/connectors/
+-rw-r--r--   0 root         (0) root         (0)      699 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/connectors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3895 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/connectors/animeultime.py
+-rw-r--r--   0 root         (0) root         (0)     4059 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/connectors/core.py
+-rw-r--r--   0 root         (0) root         (0)     3133 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/connectors/nyaa.py
+-rw-r--r--   0 root         (0) root         (0)     3594 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/connectors/yggtorrent.py
+-rw-r--r--   0 root         (0) root         (0)     2295 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/flarerequests.py
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/forms.py
+-rw-r--r--   0 root         (0) root         (0)     1100 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:37:50.892431 PyNyaaTa-202304270737/pynyaata/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:37:50.984430 PyNyaaTa-202304270737/pynyaata/static/css/
+-rw-r--r--   0 root         (0) root         (0)    59028 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/static/css/bulma-prefers-dark.css.map
+-rw-r--r--   0 root         (0) root         (0)   172028 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/static/css/bulma-prefers-dark.min.css
+-rw-r--r--   0 root         (0) root         (0)    66189 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/static/css/bulma-tooltip.min.css
+-rw-r--r--   0 root         (0) root         (0)    98250 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/static/css/bulma.css.map
+-rw-r--r--   0 root         (0) root         (0)   206620 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/static/css/bulma.min.css
+-rw-r--r--   0 root         (0) root         (0)    21778 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/static/css/font-awesome.css.map
+-rw-r--r--   0 root         (0) root         (0)    31000 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/static/css/font-awesome.min.css
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/static/css/styles.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:37:50.988430 PyNyaaTa-202304270737/pynyaata/static/favicons/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/static/favicons/animeultime.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/static/favicons/blank.png
+-rw-r--r--   0 root         (0) root         (0)   137750 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/static/favicons/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/static/favicons/nyaa.png
+-rw-r--r--   0 root         (0) root         (0)     3107 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/static/favicons/pantsu.png
+-rw-r--r--   0 root         (0) root         (0)     3046 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/static/favicons/yggtorrent.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:37:51.008430 PyNyaaTa-202304270737/pynyaata/static/fonts/
+-rw-r--r--   0 root         (0) root         (0)   134808 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/static/fonts/FontAwesome.otf
+-rw-r--r--   0 root         (0) root         (0)   165742 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/static/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 root         (0) root         (0)   444379 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/static/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 root         (0) root         (0)   165548 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/static/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 root         (0) root         (0)    98024 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/static/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 root         (0) root         (0)    77160 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/static/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:37:51.016430 PyNyaaTa-202304270737/pynyaata/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:37:51.020430 PyNyaaTa-202304270737/pynyaata/templates/admin/
+-rw-r--r--   0 root         (0) root         (0)     4378 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/templates/admin/edit.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:37:51.020430 PyNyaaTa-202304270737/pynyaata/templates/admin/folder/
+-rw-r--r--   0 root         (0) root         (0)     1007 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/templates/admin/folder/edit.html
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/templates/admin/folder/list.html
+-rw-r--r--   0 root         (0) root         (0)     3431 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/templates/admin/list.html
+-rw-r--r--   0 root         (0) root         (0)     2624 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/templates/latest.html
+-rw-r--r--   0 root         (0) root         (0)     4617 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/templates/layout.html
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/templates/list.html
+-rw-r--r--   0 root         (0) root         (0)     3032 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/templates/search.html
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/pynyaata/utils.py
+-rw-r--r--   0 root         (0) root         (0)      263 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/run.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 07:37:51.020430 PyNyaaTa-202304270737/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      961 2023-04-27 07:35:13.000000 PyNyaaTa-202304270737/setup.py
```

### Comparing `PyNyaaTa-202304261143/PKG-INFO` & `PyNyaaTa-202304270737/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNyaaTa
-Version: 202304261143
+Version: 202304270737
 Summary: π 😼た, Xéfir's personal animes torrent search engine
 Home-page: https://git.crystalyx.net/Xefir/PyNyaaTa
 Author: Xéfir Destiny
 Author-email: xefir@crystalyx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
```

### Comparing `PyNyaaTa-202304261143/PyNyaaTa.egg-info/PKG-INFO` & `PyNyaaTa-202304270737/PyNyaaTa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNyaaTa
-Version: 202304261143
+Version: 202304270737
 Summary: π 😼た, Xéfir's personal animes torrent search engine
 Home-page: https://git.crystalyx.net/Xefir/PyNyaaTa
 Author: Xéfir Destiny
 Author-email: xefir@crystalyx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
```

### Comparing `PyNyaaTa-202304261143/PyNyaaTa.egg-info/SOURCES.txt` & `PyNyaaTa-202304270737/PyNyaaTa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/README.md` & `PyNyaaTa-202304270737/README.md`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/get404.py` & `PyNyaaTa-202304270737/get404.py`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/__init__.py` & `PyNyaaTa-202304270737/pynyaata/__init__.py`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/config.py` & `PyNyaaTa-202304270737/pynyaata/config.py`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/connectors/__init__.py` & `PyNyaaTa-202304270737/pynyaata/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/connectors/animeultime.py` & `PyNyaaTa-202304270737/pynyaata/connectors/animeultime.py`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/connectors/core.py` & `PyNyaaTa-202304270737/pynyaata/connectors/core.py`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/connectors/nyaa.py` & `PyNyaaTa-202304270737/pynyaata/connectors/nyaa.py`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/connectors/yggtorrent.py` & `PyNyaaTa-202304270737/pynyaata/connectors/yggtorrent.py`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/flarerequests.py` & `PyNyaaTa-202304270737/pynyaata/flarerequests.py`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/forms.py` & `PyNyaaTa-202304270737/pynyaata/forms.py`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/models.py` & `PyNyaaTa-202304270737/pynyaata/models.py`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/static/css/bulma-prefers-dark.css.map` & `PyNyaaTa-202304270737/pynyaata/static/css/bulma-prefers-dark.css.map`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/static/css/bulma-prefers-dark.min.css` & `PyNyaaTa-202304270737/pynyaata/static/css/bulma-prefers-dark.min.css`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/static/css/bulma-tooltip.min.css` & `PyNyaaTa-202304270737/pynyaata/static/css/bulma-tooltip.min.css`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/static/css/bulma.css.map` & `PyNyaaTa-202304270737/pynyaata/static/css/bulma.css.map`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/static/css/bulma.min.css` & `PyNyaaTa-202304270737/pynyaata/static/css/bulma.min.css`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/static/css/font-awesome.css.map` & `PyNyaaTa-202304270737/pynyaata/static/css/font-awesome.css.map`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/static/css/font-awesome.min.css` & `PyNyaaTa-202304270737/pynyaata/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/static/css/styles.css` & `PyNyaaTa-202304270737/pynyaata/static/css/styles.css`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/static/favicons/animeultime.png` & `PyNyaaTa-202304270737/pynyaata/static/favicons/animeultime.png`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/static/favicons/favicon.ico` & `PyNyaaTa-202304270737/pynyaata/static/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/static/favicons/nyaa.png` & `PyNyaaTa-202304270737/pynyaata/static/favicons/nyaa.png`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/static/favicons/pantsu.png` & `PyNyaaTa-202304270737/pynyaata/static/favicons/pantsu.png`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/static/favicons/yggtorrent.png` & `PyNyaaTa-202304270737/pynyaata/static/favicons/yggtorrent.png`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/static/fonts/FontAwesome.otf` & `PyNyaaTa-202304270737/pynyaata/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/static/fonts/fontawesome-webfont.eot` & `PyNyaaTa-202304270737/pynyaata/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/static/fonts/fontawesome-webfont.svg` & `PyNyaaTa-202304270737/pynyaata/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/static/fonts/fontawesome-webfont.ttf` & `PyNyaaTa-202304270737/pynyaata/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/static/fonts/fontawesome-webfont.woff` & `PyNyaaTa-202304270737/pynyaata/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/static/fonts/fontawesome-webfont.woff2` & `PyNyaaTa-202304270737/pynyaata/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/templates/admin/edit.html` & `PyNyaaTa-202304270737/pynyaata/templates/admin/edit.html`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/templates/admin/folder/edit.html` & `PyNyaaTa-202304270737/pynyaata/templates/admin/folder/edit.html`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/templates/admin/folder/list.html` & `PyNyaaTa-202304270737/pynyaata/templates/admin/folder/list.html`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/templates/admin/list.html` & `PyNyaaTa-202304270737/pynyaata/templates/admin/list.html`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/templates/latest.html` & `PyNyaaTa-202304270737/pynyaata/templates/latest.html`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/templates/layout.html` & `PyNyaaTa-202304270737/pynyaata/templates/layout.html`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/templates/list.html` & `PyNyaaTa-202304270737/pynyaata/templates/list.html`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/templates/search.html` & `PyNyaaTa-202304270737/pynyaata/templates/search.html`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/pynyaata/utils.py` & `PyNyaaTa-202304270737/pynyaata/utils.py`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202304261143/setup.py` & `PyNyaaTa-202304270737/setup.py`

 * *Files identical despite different names*

