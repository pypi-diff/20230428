# Comparing `tmp/ipsw-0.1.3.tar.gz` & `tmp/ipsw-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipsw-0.1.3.tar", last modified: Fri Apr 14 06:20:47 2023, max compression
+gzip compressed data, was "ipsw-0.1.4.tar", last modified: Thu Apr 27 23:43:23 2023, max compression
```

## Comparing `ipsw-0.1.3.tar` & `ipsw-0.1.4.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.702191 ipsw-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-14 06:20:37.000000 ipsw-0.1.3/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.698191 ipsw-0.1.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-14 06:20:37.000000 ipsw-0.1.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.698191 ipsw-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 06:20:37.000000 ipsw-0.1.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-14 06:20:37.000000 ipsw-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-14 06:20:37.000000 ipsw-0.1.3/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.698191 ipsw-0.1.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-14 06:20:37.000000 ipsw-0.1.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-14 06:20:37.000000 ipsw-0.1.3/Dockerfile-docs
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-14 06:20:37.000000 ipsw-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-14 06:20:37.000000 ipsw-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-14 06:20:37.000000 ipsw-0.1.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-04-14 06:20:47.702191 ipsw-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-14 06:20:37.000000 ipsw-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.698191 ipsw-0.1.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.698191 ipsw-0.1.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-14 06:20:37.000000 ipsw-0.1.3/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.698191 ipsw-0.1.3/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-14 06:20:37.000000 ipsw-0.1.3/docs/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-04-14 06:20:37.000000 ipsw-0.1.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-14 06:20:37.000000 ipsw-0.1.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 06:20:37.000000 ipsw-0.1.3/docs-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.698191 ipsw-0.1.3/ipsw/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 06:20:47.000000 ipsw-0.1.3/ipsw/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.702191 ipsw-0.1.3/ipsw/api/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14662 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/api/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/api/dsc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/api/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/api/macho.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.702191 ipsw-0.1.3/ipsw/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/models/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/models/dsc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/models/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/models/macho.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/models/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.702191 ipsw-0.1.3/ipsw/transport/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/transport/basehttpadapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/transport/npipeconn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/transport/npipesocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/transport/sshconn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/transport/unixconn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.702191 ipsw-0.1.3/ipsw/types/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/types/daemon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.702191 ipsw-0.1.3/ipsw/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/utils/json_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/utils/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/utils/socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.698191 ipsw-0.1.3/ipsw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-04-14 06:20:47.000000 ipsw-0.1.3/ipsw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-14 06:20:47.000000 ipsw-0.1.3/ipsw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 06:20:47.000000 ipsw-0.1.3/ipsw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 06:20:47.000000 ipsw-0.1.3/ipsw.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-14 06:20:47.000000 ipsw-0.1.3/ipsw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-14 06:20:47.000000 ipsw-0.1.3/ipsw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 06:20:37.000000 ipsw-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-14 06:20:37.000000 ipsw-0.1.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.702191 ipsw-0.1.3/scripts /
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-14 06:20:37.000000 ipsw-0.1.3/scripts /release.sh
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-14 06:20:47.702191 ipsw-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-14 06:20:37.000000 ipsw-0.1.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-14 06:20:37.000000 ipsw-0.1.3/test-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-14 06:20:37.000000 ipsw-0.1.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:43:23.659293 ipsw-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-27 23:43:05.000000 ipsw-0.1.4/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:43:23.651293 ipsw-0.1.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-27 23:43:05.000000 ipsw-0.1.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:43:23.651293 ipsw-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-27 23:43:05.000000 ipsw-0.1.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-27 23:43:05.000000 ipsw-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-27 23:43:05.000000 ipsw-0.1.4/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:43:23.651293 ipsw-0.1.4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-27 23:43:05.000000 ipsw-0.1.4/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-27 23:43:05.000000 ipsw-0.1.4/Dockerfile-docs
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-27 23:43:05.000000 ipsw-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-27 23:43:05.000000 ipsw-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-27 23:43:05.000000 ipsw-0.1.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-27 23:43:23.659293 ipsw-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-04-27 23:43:05.000000 ipsw-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:43:23.651293 ipsw-0.1.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:43:23.651293 ipsw-0.1.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-27 23:43:05.000000 ipsw-0.1.4/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:43:23.651293 ipsw-0.1.4/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-27 23:43:05.000000 ipsw-0.1.4/docs/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-04-27 23:43:05.000000 ipsw-0.1.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-27 23:43:05.000000 ipsw-0.1.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 23:43:05.000000 ipsw-0.1.4/docs-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:43:23.651293 ipsw-0.1.4/ipsw/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 23:43:23.000000 ipsw-0.1.4/ipsw/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:43:23.655293 ipsw-0.1.4/ipsw/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14664 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/api/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/api/dsc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/api/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/api/macho.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:43:23.655293 ipsw-0.1.4/ipsw/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/models/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/models/dsc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/models/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/models/macho.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/models/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:43:23.655293 ipsw-0.1.4/ipsw/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/transport/basehttpadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/transport/npipeconn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/transport/npipesocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/transport/sshconn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/transport/unixconn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:43:23.655293 ipsw-0.1.4/ipsw/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/types/daemon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:43:23.659293 ipsw-0.1.4/ipsw/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/utils/json_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/utils/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/utils/socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-27 23:43:05.000000 ipsw-0.1.4/ipsw/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:43:23.655293 ipsw-0.1.4/ipsw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-27 23:43:23.000000 ipsw-0.1.4/ipsw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-27 23:43:23.000000 ipsw-0.1.4/ipsw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 23:43:23.000000 ipsw-0.1.4/ipsw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 23:43:23.000000 ipsw-0.1.4/ipsw.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-27 23:43:23.000000 ipsw-0.1.4/ipsw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-27 23:43:23.000000 ipsw-0.1.4/ipsw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-27 23:43:05.000000 ipsw-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-27 23:43:05.000000 ipsw-0.1.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:43:23.659293 ipsw-0.1.4/scripts /
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-27 23:43:05.000000 ipsw-0.1.4/scripts /release.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-27 23:43:23.659293 ipsw-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-27 23:43:05.000000 ipsw-0.1.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-27 23:43:05.000000 ipsw-0.1.4/test-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-27 23:43:05.000000 ipsw-0.1.4/tox.ini
```

### Comparing `ipsw-0.1.3/.github/dependabot.yml` & `ipsw-0.1.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/.github/workflows/python-publish.yml` & `ipsw-0.1.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/.gitignore` & `ipsw-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/LICENSE` & `ipsw-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/PKG-INFO` & `ipsw-0.1.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipsw
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python library for the ipsw Engine API.
 Home-page: https://github.com/blacktop/ipsw-py
 Maintainer: Blacktop
 License: MIT
 Project-URL: Documentation, https://ipsw-py.readthedocs.io
 Project-URL: Changelog, https://ipsw-py.readthedocs.io/en/stable/change-log.html
 Project-URL: Source, https://github.com/blacktop/ipsw-py
@@ -101,36 +101,64 @@
 Get DSC info
 
 ```python
 import ipsw
 
 client = ipsw.IpswClient(base_url='tcp://127.0.0.1:3993')
 
-dsc = client.dsc.get_info("20F5028e__iPhone15,2/dyld_shared_cache_arm64e")
+dsc = client.dsc.open("20F5028e__iPhone15,2/dyld_shared_cache_arm64e")
 print(dsc)
 print(dsc.dylibs[0])
-
-dylib = client.dsc.get_dylib("20F5028e__iPhone15,2/dyld_shared_cache_arm64e", "libswiftCore.dylib")
-print(dylib)
 ```
-```bash
+```python
 <DSC: '(dyld_v1  arm64e) - iOS - FAEC7714-4CCD-3B99-B18F-F5EAB60DE31E'>
 {'index': 1, 'name': '/usr/lib/libobjc.A.dylib', 'version': '876.0.0.0.0', 'uuid': '085A190C-6214-38EA-ACCB-428C3E8AFA65', 'load_address': 6443204608}
 
 <Dylib: '64-bit MachO AARCH64 (ARM64e)'>
 ```
 
+Get dylib inside DSC info
+
+```py
+libswiftCore = dsc.dylib("libswiftCore.dylib")
+print(libswiftCore)
+```
+
+Get DSC symbol addresses
+
+```python
+syms = dsc.sym_addrs([{'pattern': '.*zero.*', 'image': 'libsystem_c.dylib'}])
+print(syms)
+```
+
+Convert between DSC offsets and addresses
+
+```python
+off = dsc.a2o(7624591060)
+adr = dsc.o2a(61146836)
+```
+
+Lookup DSC symbol by address
+
+```python
+print(next(dsc.a2s([7624591060])))
+```
+```json
+{"address":7624591060,"symbol":"__exit","demanged":"__exit","mapping":"__TEXT","uuid":"3AB55994-1201-3908-BE27-52BB7EFA7573","ext":".21","image":"/usr/lib/system/libsystem_kernel.dylib","section":"__text","segment":"__TEXT"}
+```
+
+
 Get MachO info
 
 ```python
 import ipsw
 
 client = ipsw.IpswClient(base_url='tcp://127.0.0.1:3993')
 
-macho = client.macho.get("/bin/ls", arch="arm64e")
+macho = client.macho.open("/bin/ls", arch="arm64e")
 print(macho)
 ```
 ```bash
 <Macho: '64-bit MachO AARCH64 (ARM64e)'>
 ```
 
 ## Community
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ipsw Version: 0.1.3 Summary: A Python library for
+Metadata-Version: 2.1 Name: ipsw Version: 0.1.4 Summary: A Python library for
 the ipsw Engine API. Home-page: https://github.com/blacktop/ipsw-py Maintainer:
 Blacktop License: MIT Project-URL: Documentation, https://ipsw-
 py.readthedocs.io Project-URL: Changelog, https://ipsw-py.readthedocs.io/en/
 stable/change-log.html Project-URL: Source, https://github.com/blacktop/ipsw-py
 Project-URL: Tracker, https://github.com/blacktop/ipsw-py/issues Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Other
 Environment Classifier: Intended Audience :: Developers Classifier: Operating
@@ -29,24 +29,32 @@
 [available on PyPI](https://pypi.org/project/ipsw/). Either add `ipsw` to your
 `requirements.txt` file or install with **pip**: ```bash pip install ipsw ```
 ## Geting Started Get IPSW info ```python import ipsw client = ipsw.IpswClient
 (base_url='tcp://127.0.0.1:3993') info = client.info.get
 ("iPhone15,2_16.5_20F5028e_Restore.ipsw") print(f'{info.version} (
 {info.build})') for device in info.devices: print(f'- {device}') ``` ```bash
 16.5 (20F5028e) - iPhone 14 Pro ``` Get DSC info ```python import ipsw client =
-ipsw.IpswClient(base_url='tcp://127.0.0.1:3993') dsc = client.dsc.get_info
+ipsw.IpswClient(base_url='tcp://127.0.0.1:3993') dsc = client.dsc.open
 ("20F5028e__iPhone15,2/dyld_shared_cache_arm64e") print(dsc) print(dsc.dylibs
-[0]) dylib = client.dsc.get_dylib("20F5028e__iPhone15,2/
-dyld_shared_cache_arm64e", "libswiftCore.dylib") print(dylib) ``` ```bash
+[0]) ``` ```python
 (dyld_v1 arm64e) - iOS - FAEC7714-4CCD-3B99-B18F-F5EAB60DE31E'> {'index': 1,
 'name': '/usr/lib/libobjc.A.dylib', 'version': '876.0.0.0.0', 'uuid':
 '085A190C-6214-38EA-ACCB-428C3E8AFA65', 'load_address': 6443204608}
-64-bit MachO AARCH64 (ARM64e)'> ``` Get MachO info ```python import ipsw client
-= ipsw.IpswClient(base_url='tcp://127.0.0.1:3993') macho = client.macho.get("/
-bin/ls", arch="arm64e") print(macho) ``` ```bash
+64-bit MachO AARCH64 (ARM64e)'> ``` Get dylib inside DSC info ```py
+libswiftCore = dsc.dylib("libswiftCore.dylib") print(libswiftCore) ``` Get DSC
+symbol addresses ```python syms = dsc.sym_addrs([{'pattern': '.*zero.*',
+'image': 'libsystem_c.dylib'}]) print(syms) ``` Convert between DSC offsets and
+addresses ```python off = dsc.a2o(7624591060) adr = dsc.o2a(61146836) ```
+Lookup DSC symbol by address ```python print(next(dsc.a2s([7624591060]))) ```
+```json {"address":7624591060,"symbol":"__exit","demanged":"__exit","mapping":
+"__TEXT","uuid":"3AB55994-1201-3908-BE27-52BB7EFA7573","ext":".21","image":"/
+usr/lib/system/libsystem_kernel.dylib","section":"__text","segment":"__TEXT"}
+``` Get MachO info ```python import ipsw client = ipsw.IpswClient
+(base_url='tcp://127.0.0.1:3993') macho = client.macho.open("/bin/ls",
+arch="arm64e") print(macho) ``` ```bash
 64-bit MachO AARCH64 (ARM64e)'> ``` ## Community You have questions, need
 support and or just want to talk about `ipsw-py`? Here are ways to get in touch
 with the `ipsw-py` community: [![Join Discord](https://img.shields.io/badge/
 Join_our_Discord_server-5865F2?style=for-the-
 badge&logo=discord&logoColor=white)](https://discord.gg/xx2y9yrcgs) [![Follow
 Twitter](https://img.shields.io/badge/follow_on_twitter-1DA1F2?style=for-the-
 badge&logo=twitter&logoColor=white)](https://twitter.com/blacktop__) [![Follow
```

### Comparing `ipsw-0.1.3/README.md` & `ipsw-0.1.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -70,36 +70,64 @@
 Get DSC info
 
 ```python
 import ipsw
 
 client = ipsw.IpswClient(base_url='tcp://127.0.0.1:3993')
 
-dsc = client.dsc.get_info("20F5028e__iPhone15,2/dyld_shared_cache_arm64e")
+dsc = client.dsc.open("20F5028e__iPhone15,2/dyld_shared_cache_arm64e")
 print(dsc)
 print(dsc.dylibs[0])
-
-dylib = client.dsc.get_dylib("20F5028e__iPhone15,2/dyld_shared_cache_arm64e", "libswiftCore.dylib")
-print(dylib)
 ```
-```bash
+```python
 <DSC: '(dyld_v1  arm64e) - iOS - FAEC7714-4CCD-3B99-B18F-F5EAB60DE31E'>
 {'index': 1, 'name': '/usr/lib/libobjc.A.dylib', 'version': '876.0.0.0.0', 'uuid': '085A190C-6214-38EA-ACCB-428C3E8AFA65', 'load_address': 6443204608}
 
 <Dylib: '64-bit MachO AARCH64 (ARM64e)'>
 ```
 
+Get dylib inside DSC info
+
+```py
+libswiftCore = dsc.dylib("libswiftCore.dylib")
+print(libswiftCore)
+```
+
+Get DSC symbol addresses
+
+```python
+syms = dsc.sym_addrs([{'pattern': '.*zero.*', 'image': 'libsystem_c.dylib'}])
+print(syms)
+```
+
+Convert between DSC offsets and addresses
+
+```python
+off = dsc.a2o(7624591060)
+adr = dsc.o2a(61146836)
+```
+
+Lookup DSC symbol by address
+
+```python
+print(next(dsc.a2s([7624591060])))
+```
+```json
+{"address":7624591060,"symbol":"__exit","demanged":"__exit","mapping":"__TEXT","uuid":"3AB55994-1201-3908-BE27-52BB7EFA7573","ext":".21","image":"/usr/lib/system/libsystem_kernel.dylib","section":"__text","segment":"__TEXT"}
+```
+
+
 Get MachO info
 
 ```python
 import ipsw
 
 client = ipsw.IpswClient(base_url='tcp://127.0.0.1:3993')
 
-macho = client.macho.get("/bin/ls", arch="arm64e")
+macho = client.macho.open("/bin/ls", arch="arm64e")
 print(macho)
 ```
 ```bash
 <Macho: '64-bit MachO AARCH64 (ARM64e)'>
 ```
 
 ## Community
```

#### html2text {}

```diff
@@ -12,24 +12,32 @@
 [available on PyPI](https://pypi.org/project/ipsw/). Either add `ipsw` to your
 `requirements.txt` file or install with **pip**: ```bash pip install ipsw ```
 ## Geting Started Get IPSW info ```python import ipsw client = ipsw.IpswClient
 (base_url='tcp://127.0.0.1:3993') info = client.info.get
 ("iPhone15,2_16.5_20F5028e_Restore.ipsw") print(f'{info.version} (
 {info.build})') for device in info.devices: print(f'- {device}') ``` ```bash
 16.5 (20F5028e) - iPhone 14 Pro ``` Get DSC info ```python import ipsw client =
-ipsw.IpswClient(base_url='tcp://127.0.0.1:3993') dsc = client.dsc.get_info
+ipsw.IpswClient(base_url='tcp://127.0.0.1:3993') dsc = client.dsc.open
 ("20F5028e__iPhone15,2/dyld_shared_cache_arm64e") print(dsc) print(dsc.dylibs
-[0]) dylib = client.dsc.get_dylib("20F5028e__iPhone15,2/
-dyld_shared_cache_arm64e", "libswiftCore.dylib") print(dylib) ``` ```bash
+[0]) ``` ```python
 (dyld_v1 arm64e) - iOS - FAEC7714-4CCD-3B99-B18F-F5EAB60DE31E'> {'index': 1,
 'name': '/usr/lib/libobjc.A.dylib', 'version': '876.0.0.0.0', 'uuid':
 '085A190C-6214-38EA-ACCB-428C3E8AFA65', 'load_address': 6443204608}
-64-bit MachO AARCH64 (ARM64e)'> ``` Get MachO info ```python import ipsw client
-= ipsw.IpswClient(base_url='tcp://127.0.0.1:3993') macho = client.macho.get("/
-bin/ls", arch="arm64e") print(macho) ``` ```bash
+64-bit MachO AARCH64 (ARM64e)'> ``` Get dylib inside DSC info ```py
+libswiftCore = dsc.dylib("libswiftCore.dylib") print(libswiftCore) ``` Get DSC
+symbol addresses ```python syms = dsc.sym_addrs([{'pattern': '.*zero.*',
+'image': 'libsystem_c.dylib'}]) print(syms) ``` Convert between DSC offsets and
+addresses ```python off = dsc.a2o(7624591060) adr = dsc.o2a(61146836) ```
+Lookup DSC symbol by address ```python print(next(dsc.a2s([7624591060]))) ```
+```json {"address":7624591060,"symbol":"__exit","demanged":"__exit","mapping":
+"__TEXT","uuid":"3AB55994-1201-3908-BE27-52BB7EFA7573","ext":".21","image":"/
+usr/lib/system/libsystem_kernel.dylib","section":"__text","segment":"__TEXT"}
+``` Get MachO info ```python import ipsw client = ipsw.IpswClient
+(base_url='tcp://127.0.0.1:3993') macho = client.macho.open("/bin/ls",
+arch="arm64e") print(macho) ``` ```bash
 64-bit MachO AARCH64 (ARM64e)'> ``` ## Community You have questions, need
 support and or just want to talk about `ipsw-py`? Here are ways to get in touch
 with the `ipsw-py` community: [![Join Discord](https://img.shields.io/badge/
 Join_our_Discord_server-5865F2?style=for-the-
 badge&logo=discord&logoColor=white)](https://discord.gg/xx2y9yrcgs) [![Follow
 Twitter](https://img.shields.io/badge/follow_on_twitter-1DA1F2?style=for-the-
 badge&logo=twitter&logoColor=white)](https://twitter.com/blacktop__) [![Follow
```

### Comparing `ipsw-0.1.3/docs/conf.py` & `ipsw-0.1.4/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,85 +14,83 @@
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import datetime
 import os
 import sys
-sys.path.insert(0, os.path.abspath('..'))
+
+sys.path.insert(0, os.path.abspath(".."))
 
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
-extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.napoleon',
-    'myst_parser'
-]
+extensions = ["sphinx.ext.autodoc", "sphinx.ext.napoleon", "myst_parser"]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 
 source_suffix = {
-    '.rst': 'restructuredtext',
-    '.txt': 'markdown',
-    '.md': 'markdown',
+    ".rst": "restructuredtext",
+    ".txt": "markdown",
+    ".md": "markdown",
 }
 
 # The encoding of source files.
 #
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = 'ipsw SDK for Python'
+project = "ipsw SDK for Python"
 year = datetime.datetime.now().year
-copyright = '%d Blacktop' % year
-author = 'Blacktop'
+copyright = "%d Blacktop" % year
+author = "Blacktop"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # see https://github.com/pypa/setuptools_scm#usage-from-sphinx
 from importlib.metadata import version
-release = version('ipsw')
+
+release = version("ipsw")
 # for example take major/minor
-version = '.'.join(release.split('.')[:2])
+version = ".".join(release.split(".")[:2])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = 'en'
+language = "en"
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 #
 # today = ''
 #
 # Else, today_fmt is used as the format for a strftime call.
 #
 # today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The reST default role (used for this markup: `text`) to use for all
 # documents.
 #
 # default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
@@ -106,15 +104,15 @@
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
 #
 # show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
 # modindex_common_prefix = []
 
 # If true, keep warnings as "system message" paragraphs in the built documents.
 # keep_warnings = False
 
@@ -123,23 +121,23 @@
 
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'alabaster'
+html_theme = "alabaster"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 html_theme_options = {
-    'description': 'A Python library for the ipsw API',
-    'fixed_sidebar': True,
+    "description": "A Python library for the ipsw API",
+    "fixed_sidebar": True,
 }
 
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 
 # The name for this set of Sphinx documents.
 # "<project> v<release> documentation" by default.
@@ -160,15 +158,15 @@
 # pixels large.
 #
 # html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 # Add any extra paths that contain custom files (such as robots.txt or
 # .htaccess) here, relative to this directory. These files are copied
 # directly to the root of the documentation.
 #
 # html_extra_path = []
 
@@ -182,18 +180,18 @@
 # typographically correct entities.
 #
 # html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
 #
 html_sidebars = {
-    '**': [
-        'about.html',
-        'navigation.html',
-        'searchbox.html',
+    "**": [
+        "about.html",
+        "navigation.html",
+        "searchbox.html",
     ]
 }
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
 #
 # html_additional_pages = {}
@@ -246,42 +244,38 @@
 
 # The name of a javascript file (relative to the configuration directory) that
 # implements a search results scorer. If empty, the default will be used.
 #
 # html_search_scorer = 'scorer.js'
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'ipsw-sdk-pythondoc'
+htmlhelp_basename = "ipsw-sdk-pythondoc"
 
 # -- Options for LaTeX output ---------------------------------------------
 
 latex_elements = {
-     # The paper size ('letterpaper' or 'a4paper').
-     #
-     # 'papersize': 'letterpaper',
-
-     # The font size ('10pt', '11pt' or '12pt').
-     #
-     # 'pointsize': '10pt',
-
-     # Additional stuff for the LaTeX preamble.
-     #
-     # 'preamble': '',
-
-     # Latex figure (float) alignment
-     #
-     # 'figure_align': 'htbp',
+    # The paper size ('letterpaper' or 'a4paper').
+    #
+    # 'papersize': 'letterpaper',
+    # The font size ('10pt', '11pt' or '12pt').
+    #
+    # 'pointsize': '10pt',
+    # Additional stuff for the LaTeX preamble.
+    #
+    # 'preamble': '',
+    # Latex figure (float) alignment
+    #
+    # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'ipsw-sdk-python.tex', 'ipsw-sdk-python Documentation',
-     'Blacktop.', 'manual'),
+    (master_doc, "ipsw-sdk-python.tex", "ipsw-sdk-python Documentation", "Blacktop.", "manual"),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 #
 # latex_logo = None
 
@@ -313,33 +307,36 @@
 # latex_domain_indices = True
 
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'ipsw-sdk-python', 'ipsw-sdk-python Documentation',
-     [author], 1)
-]
+man_pages = [(master_doc, "ipsw-sdk-python", "ipsw-sdk-python Documentation", [author], 1)]
 
 # If true, show URL addresses after external links.
 #
 # man_show_urls = False
 
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'ipsw-sdk-python', 'ipsw-sdk-python Documentation',
-     author, 'ipsw-sdk-python', 'One line description of project.',
-     'Miscellaneous'),
+    (
+        master_doc,
+        "ipsw-sdk-python",
+        "ipsw-sdk-python Documentation",
+        author,
+        "ipsw-sdk-python",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
 ]
 
 # Documents to append as an appendix to all manuals.
 #
 # texinfo_appendices = []
 
 # If false, no module index is generated.
```

### Comparing `ipsw-0.1.3/docs/index.rst` & `ipsw-0.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/ipsw/api/client.py` & `ipsw-0.1.4/ipsw/api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,17 +148,17 @@
         if utils.version_lt(self._version, MINIMUM_IPSW_API_VERSION):
             raise InvalidVersion(
                 "API versions below {} are no longer supported by this " "library.".format(MINIMUM_IPSW_API_VERSION)
             )
 
     def _retrieve_server_version(self):
         try:
-            return self.version(api_version=False)["ApiVersion"]
+            return self.version(api_version=False)["api_version"]
         except KeyError:
-            raise IpswException('Invalid response from ipsw daemon: key "ApiVersion"' " is missing.")
+            raise IpswException('Invalid response from ipsw daemon: key "api_version"' " is missing.")
         except Exception as e:
             raise IpswException(f"Error while fetching server API version: {e}")
 
     def _set_request_timeout(self, kwargs):
         """Prepare the kwargs for an HTTP request by inserting the timeout
         parameter, if not already present."""
         kwargs.setdefault("timeout", self.timeout)
```

### Comparing `ipsw-0.1.3/ipsw/api/daemon.py` & `ipsw-0.1.4/ipsw/api/daemon.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/ipsw/api/info.py` & `ipsw-0.1.4/ipsw/api/info.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/ipsw/client.py` & `ipsw-0.1.4/ipsw/client.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/ipsw/constants.py` & `ipsw-0.1.4/ipsw/constants.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/ipsw/errors.py` & `ipsw-0.1.4/ipsw/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 def create_api_error_from_http_exception(e):
     """
     Create a suitable APIError from requests.exceptions.HTTPError.
     """
     response = e.response
     try:
-        explanation = response.json()["message"]
+        explanation = response.json()["error"]
     except ValueError:
         explanation = (response.content or "").strip()
     cls = APIError
     if response.status_code == 404:
         cls = NotFound
     raise cls(e, response=response, explanation=explanation) from e
```

### Comparing `ipsw-0.1.3/ipsw/models/configs.py` & `ipsw-0.1.4/ipsw/models/configs.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/ipsw/models/info.py` & `ipsw-0.1.4/ipsw/models/info.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/ipsw/models/macho.py` & `ipsw-0.1.4/ipsw/models/macho.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,16 +41,23 @@
     @property
     def header(self):
         """
         The header.
         """
         return self.attrs["info"].get("header", None)
 
+    @property
+    def path(self):
+        """
+        The DSC path.
+        """
+        return self.attrs.get("path", None)
+
 
 class MachoCollection(Collection):
     model = Macho
 
-    def get(self, path=None, arch=None):
+    def open(self, path=None, arch=None):
         """
         Get MachO info.
         """
         return self.prepare_model(self.client.api.macho_info(path, arch))
```

### Comparing `ipsw-0.1.3/ipsw/models/resource.py` & `ipsw-0.1.4/ipsw/models/resource.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/ipsw/transport/npipeconn.py` & `ipsw-0.1.4/ipsw/transport/npipeconn.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/ipsw/transport/npipesocket.py` & `ipsw-0.1.4/ipsw/transport/npipesocket.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/ipsw/transport/sshconn.py` & `ipsw-0.1.4/ipsw/transport/sshconn.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/ipsw/transport/unixconn.py` & `ipsw-0.1.4/ipsw/transport/unixconn.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/ipsw/types/daemon.py` & `ipsw-0.1.4/ipsw/types/daemon.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/ipsw/utils/config.py` & `ipsw-0.1.4/ipsw/utils/config.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/ipsw/utils/decorators.py` & `ipsw-0.1.4/ipsw/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/ipsw/utils/json_stream.py` & `ipsw-0.1.4/ipsw/utils/json_stream.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/ipsw/utils/proxy.py` & `ipsw-0.1.4/ipsw/utils/proxy.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/ipsw/utils/socket.py` & `ipsw-0.1.4/ipsw/utils/socket.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/ipsw/utils/utils.py` & `ipsw-0.1.4/ipsw/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/ipsw/version.py` & `ipsw-0.1.4/ipsw/version.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/ipsw.egg-info/PKG-INFO` & `ipsw-0.1.4/ipsw.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipsw
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python library for the ipsw Engine API.
 Home-page: https://github.com/blacktop/ipsw-py
 Maintainer: Blacktop
 License: MIT
 Project-URL: Documentation, https://ipsw-py.readthedocs.io
 Project-URL: Changelog, https://ipsw-py.readthedocs.io/en/stable/change-log.html
 Project-URL: Source, https://github.com/blacktop/ipsw-py
@@ -101,36 +101,64 @@
 Get DSC info
 
 ```python
 import ipsw
 
 client = ipsw.IpswClient(base_url='tcp://127.0.0.1:3993')
 
-dsc = client.dsc.get_info("20F5028e__iPhone15,2/dyld_shared_cache_arm64e")
+dsc = client.dsc.open("20F5028e__iPhone15,2/dyld_shared_cache_arm64e")
 print(dsc)
 print(dsc.dylibs[0])
-
-dylib = client.dsc.get_dylib("20F5028e__iPhone15,2/dyld_shared_cache_arm64e", "libswiftCore.dylib")
-print(dylib)
 ```
-```bash
+```python
 <DSC: '(dyld_v1  arm64e) - iOS - FAEC7714-4CCD-3B99-B18F-F5EAB60DE31E'>
 {'index': 1, 'name': '/usr/lib/libobjc.A.dylib', 'version': '876.0.0.0.0', 'uuid': '085A190C-6214-38EA-ACCB-428C3E8AFA65', 'load_address': 6443204608}
 
 <Dylib: '64-bit MachO AARCH64 (ARM64e)'>
 ```
 
+Get dylib inside DSC info
+
+```py
+libswiftCore = dsc.dylib("libswiftCore.dylib")
+print(libswiftCore)
+```
+
+Get DSC symbol addresses
+
+```python
+syms = dsc.sym_addrs([{'pattern': '.*zero.*', 'image': 'libsystem_c.dylib'}])
+print(syms)
+```
+
+Convert between DSC offsets and addresses
+
+```python
+off = dsc.a2o(7624591060)
+adr = dsc.o2a(61146836)
+```
+
+Lookup DSC symbol by address
+
+```python
+print(next(dsc.a2s([7624591060])))
+```
+```json
+{"address":7624591060,"symbol":"__exit","demanged":"__exit","mapping":"__TEXT","uuid":"3AB55994-1201-3908-BE27-52BB7EFA7573","ext":".21","image":"/usr/lib/system/libsystem_kernel.dylib","section":"__text","segment":"__TEXT"}
+```
+
+
 Get MachO info
 
 ```python
 import ipsw
 
 client = ipsw.IpswClient(base_url='tcp://127.0.0.1:3993')
 
-macho = client.macho.get("/bin/ls", arch="arm64e")
+macho = client.macho.open("/bin/ls", arch="arm64e")
 print(macho)
 ```
 ```bash
 <Macho: '64-bit MachO AARCH64 (ARM64e)'>
 ```
 
 ## Community
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ipsw Version: 0.1.3 Summary: A Python library for
+Metadata-Version: 2.1 Name: ipsw Version: 0.1.4 Summary: A Python library for
 the ipsw Engine API. Home-page: https://github.com/blacktop/ipsw-py Maintainer:
 Blacktop License: MIT Project-URL: Documentation, https://ipsw-
 py.readthedocs.io Project-URL: Changelog, https://ipsw-py.readthedocs.io/en/
 stable/change-log.html Project-URL: Source, https://github.com/blacktop/ipsw-py
 Project-URL: Tracker, https://github.com/blacktop/ipsw-py/issues Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Other
 Environment Classifier: Intended Audience :: Developers Classifier: Operating
@@ -29,24 +29,32 @@
 [available on PyPI](https://pypi.org/project/ipsw/). Either add `ipsw` to your
 `requirements.txt` file or install with **pip**: ```bash pip install ipsw ```
 ## Geting Started Get IPSW info ```python import ipsw client = ipsw.IpswClient
 (base_url='tcp://127.0.0.1:3993') info = client.info.get
 ("iPhone15,2_16.5_20F5028e_Restore.ipsw") print(f'{info.version} (
 {info.build})') for device in info.devices: print(f'- {device}') ``` ```bash
 16.5 (20F5028e) - iPhone 14 Pro ``` Get DSC info ```python import ipsw client =
-ipsw.IpswClient(base_url='tcp://127.0.0.1:3993') dsc = client.dsc.get_info
+ipsw.IpswClient(base_url='tcp://127.0.0.1:3993') dsc = client.dsc.open
 ("20F5028e__iPhone15,2/dyld_shared_cache_arm64e") print(dsc) print(dsc.dylibs
-[0]) dylib = client.dsc.get_dylib("20F5028e__iPhone15,2/
-dyld_shared_cache_arm64e", "libswiftCore.dylib") print(dylib) ``` ```bash
+[0]) ``` ```python
 (dyld_v1 arm64e) - iOS - FAEC7714-4CCD-3B99-B18F-F5EAB60DE31E'> {'index': 1,
 'name': '/usr/lib/libobjc.A.dylib', 'version': '876.0.0.0.0', 'uuid':
 '085A190C-6214-38EA-ACCB-428C3E8AFA65', 'load_address': 6443204608}
-64-bit MachO AARCH64 (ARM64e)'> ``` Get MachO info ```python import ipsw client
-= ipsw.IpswClient(base_url='tcp://127.0.0.1:3993') macho = client.macho.get("/
-bin/ls", arch="arm64e") print(macho) ``` ```bash
+64-bit MachO AARCH64 (ARM64e)'> ``` Get dylib inside DSC info ```py
+libswiftCore = dsc.dylib("libswiftCore.dylib") print(libswiftCore) ``` Get DSC
+symbol addresses ```python syms = dsc.sym_addrs([{'pattern': '.*zero.*',
+'image': 'libsystem_c.dylib'}]) print(syms) ``` Convert between DSC offsets and
+addresses ```python off = dsc.a2o(7624591060) adr = dsc.o2a(61146836) ```
+Lookup DSC symbol by address ```python print(next(dsc.a2s([7624591060]))) ```
+```json {"address":7624591060,"symbol":"__exit","demanged":"__exit","mapping":
+"__TEXT","uuid":"3AB55994-1201-3908-BE27-52BB7EFA7573","ext":".21","image":"/
+usr/lib/system/libsystem_kernel.dylib","section":"__text","segment":"__TEXT"}
+``` Get MachO info ```python import ipsw client = ipsw.IpswClient
+(base_url='tcp://127.0.0.1:3993') macho = client.macho.open("/bin/ls",
+arch="arm64e") print(macho) ``` ```bash
 64-bit MachO AARCH64 (ARM64e)'> ``` ## Community You have questions, need
 support and or just want to talk about `ipsw-py`? Here are ways to get in touch
 with the `ipsw-py` community: [![Join Discord](https://img.shields.io/badge/
 Join_our_Discord_server-5865F2?style=for-the-
 badge&logo=discord&logoColor=white)](https://discord.gg/xx2y9yrcgs) [![Follow
 Twitter](https://img.shields.io/badge/follow_on_twitter-1DA1F2?style=for-the-
 badge&logo=twitter&logoColor=white)](https://twitter.com/blacktop__) [![Follow
```

### Comparing `ipsw-0.1.3/ipsw.egg-info/SOURCES.txt` & `ipsw-0.1.4/ipsw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/scripts /release.sh` & `ipsw-0.1.4/scripts /release.sh`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.3/setup.py` & `ipsw-0.1.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,76 +6,72 @@
 from setuptools import find_packages
 from setuptools import setup
 
 ROOT_DIR = os.path.dirname(__file__)
 SOURCE_DIR = os.path.join(ROOT_DIR)
 
 requirements = [
-    'packaging >= 23.0',
-    'requests >= 2.28.2',
-    'urllib3 >= 1.26.15',
-    'websocket-client >= 1.5.1',
-    'pyyaml >= 6.0',
+    "packaging >= 23.0",
+    "requests >= 2.28.2",
+    "urllib3 >= 1.26.15",
+    "websocket-client >= 1.5.1",
+    "pyyaml >= 6.0",
 ]
 
 extras_require = {
     # win32 APIs if on Windows (required for npipe support)
-    ':sys_platform == "win32"': 'pywin32>=306',
-
+    ':sys_platform == "win32"': "pywin32>=306",
     # This is now a no-op, as similarly the requests[security] extra is
     # a no-op as of requests 2.26.0, this is always available/by default now
     # see https://github.com/psf/requests/pull/5867
-    'tls': [],
-
+    "tls": [],
     # Only required when connecting using the ssh:// protocol
-    'ssh': ['paramiko>=3.1.0'],
+    "ssh": ["paramiko>=3.1.0"],
 }
 
-with open('./test-requirements.txt') as test_reqs_txt:
+with open("./test-requirements.txt") as test_reqs_txt:
     test_requirements = [line for line in test_reqs_txt]
 
 
-long_description = ''
-with codecs.open('./README.md', encoding='utf-8') as readme_md:
+long_description = ""
+with codecs.open("./README.md", encoding="utf-8") as readme_md:
     long_description = readme_md.read()
 
 setup(
     name="ipsw",
-    use_scm_version={
-        'write_to': 'ipsw/_version.py'
-    },
+    use_scm_version={"write_to": "ipsw/_version.py"},
     description="A Python library for the ipsw Engine API.",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    url='https://github.com/blacktop/ipsw-py',
+    long_description_content_type="text/markdown",
+    url="https://github.com/blacktop/ipsw-py",
     project_urls={
-        'Documentation': 'https://ipsw-py.readthedocs.io',
-        'Changelog': 'https://ipsw-py.readthedocs.io/en/stable/change-log.html',  # noqa: E501
-        'Source': 'https://github.com/blacktop/ipsw-py',
-        'Tracker': 'https://github.com/blacktop/ipsw-py/issues',
+        "Documentation": "https://ipsw-py.readthedocs.io",
+        "Changelog": "https://ipsw-py.readthedocs.io/en/stable/change-log.html",  # noqa: E501
+        "Source": "https://github.com/blacktop/ipsw-py",
+        "Tracker": "https://github.com/blacktop/ipsw-py/issues",
     },
     packages=find_packages(exclude=["tests.*", "tests"]),
-    setup_requires=['setuptools_scm'],
+    setup_requires=["setuptools_scm"],
     install_requires=requirements,
     tests_require=test_requirements,
     extras_require=extras_require,
-    python_requires='>=3.7',
+    python_requires=">=3.7",
     zip_safe=False,
-    test_suite='tests',
+    test_suite="tests",
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Environment :: Other Environment',
-        'Intended Audience :: Developers',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Topic :: Software Development',
-        'Topic :: Utilities',
-        'License :: OSI Approved :: Apache Software License',
+        "Development Status :: 5 - Production/Stable",
+        "Environment :: Other Environment",
+        "Intended Audience :: Developers",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Topic :: Software Development",
+        "Topic :: Utilities",
+        "License :: OSI Approved :: Apache Software License",
     ],
-    maintainer='Blacktop',
-)
+    maintainer="Blacktop",
+)
```

