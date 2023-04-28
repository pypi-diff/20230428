# Comparing `tmp/calfire-wildfires-1.1.0.tar.gz` & `tmp/calfire-wildfires-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calfire-wildfires-1.1.0.tar", last modified: Mon May 30 04:20:11 2022, max compression
+gzip compressed data, was "calfire-wildfires-1.1.1.tar", last modified: Fri Apr 28 19:56:14 2023, max compression
```

## Comparing `calfire-wildfires-1.1.0.tar` & `calfire-wildfires-1.1.1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 04:20:11.865440 calfire-wildfires-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 04:20:11.861440 calfire-wildfires-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 04:20:11.865440 calfire-wildfires-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2928 2022-05-30 04:19:19.000000 calfire-wildfires-1.1.0/.github/workflows/continuous-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-05-30 04:19:19.000000 calfire-wildfires-1.1.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-05-30 04:19:19.000000 calfire-wildfires-1.1.0/.github/workflows/scrape.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1212 2022-05-30 04:19:19.000000 calfire-wildfires-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-05-30 04:19:19.000000 calfire-wildfires-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-05-30 04:19:19.000000 calfire-wildfires-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1251 2022-05-30 04:20:11.865440 calfire-wildfires-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-05-30 04:19:19.000000 calfire-wildfires-1.1.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (121)    28180 2022-05-30 04:19:19.000000 calfire-wildfires-1.1.0/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-05-30 04:19:19.000000 calfire-wildfires-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 04:20:11.865440 calfire-wildfires-1.1.0/calfire_wildfires/
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-05-30 04:19:19.000000 calfire-wildfires-1.1.0/calfire_wildfires/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-05-30 04:19:19.000000 calfire-wildfires-1.1.0/calfire_wildfires/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 04:20:11.865440 calfire-wildfires-1.1.0/calfire_wildfires.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1251 2022-05-30 04:20:11.000000 calfire-wildfires-1.1.0/calfire_wildfires.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      652 2022-05-30 04:20:11.000000 calfire-wildfires-1.1.0/calfire_wildfires.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-30 04:20:11.000000 calfire-wildfires-1.1.0/calfire_wildfires.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-05-30 04:20:11.000000 calfire-wildfires-1.1.0/calfire_wildfires.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-05-30 04:20:11.000000 calfire-wildfires-1.1.0/calfire_wildfires.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-05-30 04:20:11.000000 calfire-wildfires-1.1.0/calfire_wildfires.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 04:20:11.865440 calfire-wildfires-1.1.0/data/
--rw-r--r--   0 runner    (1001) docker     (121)     3384 2022-05-30 04:19:19.000000 calfire-wildfires-1.1.0/data/active.json
--rw-r--r--   0 runner    (1001) docker     (121)    25873 2022-05-30 04:19:19.000000 calfire-wildfires-1.1.0/data/all.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 04:20:11.865440 calfire-wildfires-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-05-30 04:19:19.000000 calfire-wildfires-1.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 04:20:11.861440 calfire-wildfires-1.1.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 04:20:11.865440 calfire-wildfires-1.1.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     3731 2022-05-30 04:19:19.000000 calfire-wildfires-1.1.0/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 04:20:11.865440 calfire-wildfires-1.1.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-05-30 04:19:19.000000 calfire-wildfires-1.1.0/docs/_templates/nav.html
--rw-r--r--   0 runner    (1001) docker     (121)      850 2022-05-30 04:19:19.000000 calfire-wildfires-1.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1750 2022-05-30 04:19:19.000000 calfire-wildfires-1.1.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-05-30 04:19:19.000000 calfire-wildfires-1.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-05-30 04:19:19.000000 calfire-wildfires-1.1.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-05-30 04:20:11.865440 calfire-wildfires-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2194 2022-05-30 04:19:19.000000 calfire-wildfires-1.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-05-30 04:19:19.000000 calfire-wildfires-1.1.0/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:56:14.221748 calfire-wildfires-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:56:14.213748 calfire-wildfires-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:56:14.217748 calfire-wildfires-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/.github/workflows/continuous-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/.github/workflows/scrape.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-28 19:56:14.221748 calfire-wildfires-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    37856 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:56:14.217748 calfire-wildfires-1.1.1/calfire_wildfires/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/calfire_wildfires/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/calfire_wildfires/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:56:14.217748 calfire-wildfires-1.1.1/calfire_wildfires.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-28 19:56:14.000000 calfire-wildfires-1.1.1/calfire_wildfires.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-28 19:56:14.000000 calfire-wildfires-1.1.1/calfire_wildfires.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:56:14.000000 calfire-wildfires-1.1.1/calfire_wildfires.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 19:56:14.000000 calfire-wildfires-1.1.1/calfire_wildfires.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 19:56:14.000000 calfire-wildfires-1.1.1/calfire_wildfires.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 19:56:14.000000 calfire-wildfires-1.1.1/calfire_wildfires.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:56:14.217748 calfire-wildfires-1.1.1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/data/active.json
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/data/all.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:56:14.217748 calfire-wildfires-1.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:56:14.213748 calfire-wildfires-1.1.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:56:14.217748 calfire-wildfires-1.1.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:56:14.217748 calfire-wildfires-1.1.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/docs/_templates/nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-28 19:56:14.221748 calfire-wildfires-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/test.py
```

### Comparing `calfire-wildfires-1.1.0/.github/workflows/continuous-deployment.yml` & `calfire-wildfires-1.1.1/.github/workflows/continuous-deployment.yml`

 * *Files identical despite different names*

### Comparing `calfire-wildfires-1.1.0/.github/workflows/docs.yml` & `calfire-wildfires-1.1.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `calfire-wildfires-1.1.0/.github/workflows/scrape.yml` & `calfire-wildfires-1.1.1/.github/workflows/scrape.yml`

 * *Files identical despite different names*

### Comparing `calfire-wildfires-1.1.0/.gitignore` & `calfire-wildfires-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `calfire-wildfires-1.1.0/LICENSE` & `calfire-wildfires-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `calfire-wildfires-1.1.0/Pipfile.lock` & `calfire-wildfires-1.1.1/Pipfile.lock`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9139038231780168%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'d7a48589ea82f0f169eb8a249455ed3e9c054839268b873813f04b76fbc3aaed'}}",*

 * * "'default'": "{'certifi': {'hashes': "*

 * *              "['sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3', "*

 * *              "'sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18'], "*

 * *              "'version': '==2022.12.7'}, 'idna': {'hashes': "*

 * *              "['sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4', "*

 * *            […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "1a02187f64b66122c075e17edacbcbcefe75952247885c8edea6f7dcfc7c6b00"
+            "sha256": "d7a48589ea82f0f169eb8a249455ed3e9c054839268b873813f04b76fbc3aaed"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.9"
         },
         "sources": [
             {
@@ -14,19 +14,19 @@
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "certifi": {
             "hashes": [
-                "sha256:9c5705e395cd70084351dd8ad5c41e65655e08ce46f2ec9cf6c2c08390f71eb7",
-                "sha256:f1d53542ee8cbedbe2118b5686372fb33c297fcd6379b050cca0ef13a597382a"
+                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
+                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.5.18.1"
+            "version": "==2022.12.7"
         },
         "charset-normalizer": {
             "hashes": [
                 "sha256:2857e29ff0d34db842cd7ca3230549d1a697f96ee6d3fb071cfa6c7393832597",
                 "sha256:6881edbebdb17b39b4eaaa821b438bf6eddffb4468cf344f09f89def34a8b1df"
             ],
             "markers": "python_version >= '3'",
@@ -38,206 +38,254 @@
                 "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
             "index": "pypi",
             "version": "==8.1.3"
         },
         "idna": {
             "hashes": [
-                "sha256:84d9dd047ffa80596e0f246e2eab0b391788b0503584e8945f2368256d2735ff",
-                "sha256:9d643ff0a55b762d5cdb124b8eaa99c66322e2157b69160bc32796e824360e6d"
+                "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
+                "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3'",
-            "version": "==3.3"
+            "version": "==3.4"
         },
         "requests": {
             "hashes": [
                 "sha256:68d7c56fd5a8999887728ef304a6d12edc7be74f1cfa47714fc8b414525c9a61",
                 "sha256:f22fa1e554c9ddfd16e6e41ac79759e17be9e492b3587efa038054674760e72d"
             ],
             "index": "pypi",
             "version": "==2.27.1"
         },
         "urllib3": {
             "hashes": [
-                "sha256:44ece4d53fb1706f667c9bd1c648f5469a2ec925fcf3a776667042d645472c14",
-                "sha256:aabaf16477806a5e1dd19aa41f8c2b7950dd3c746362d7e3223dbe6de6ac448e"
+                "sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72",
+                "sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4'",
-            "version": "==1.26.9"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
+            "version": "==1.26.14"
         }
     },
     "develop": {
         "alabaster": {
             "hashes": [
-                "sha256:446438bdcca0e05bd45ea2de1668c1d9b032e1a9154c2c259092d77031ddd359",
-                "sha256:a661d72d58e6ea8a57f7a86e37d86716863ee5e92788398526d58b26a4e4dc02"
+                "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3",
+                "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
             ],
-            "version": "==0.7.12"
+            "markers": "python_version >= '3.6'",
+            "version": "==0.7.13"
         },
         "babel": {
             "hashes": [
-                "sha256:3f349e85ad3154559ac4930c3918247d319f21910d5ce4b25d439ed8693b98d2",
-                "sha256:98aeaca086133efb3e1e2aad0396987490c8425929ddbcfe0550184fdc54cd13"
+                "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
+                "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.10.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.12.1"
         },
         "bleach": {
             "hashes": [
-                "sha256:08a1fe86d253b5c88c92cc3d810fd8048a16d15762e1e5b74d502256e5926aa1",
-                "sha256:c6d6cc054bdc9c83b48b8083e236e5f00f238428666d2ce2e083eaa5fd568565"
+                "sha256:1a1a85c1595e07d8db14c5f09f09e6433502c51c595970edc090551f0db99414",
+                "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==5.0.0"
+            "version": "==6.0.0"
         },
         "certifi": {
             "hashes": [
-                "sha256:9c5705e395cd70084351dd8ad5c41e65655e08ce46f2ec9cf6c2c08390f71eb7",
-                "sha256:f1d53542ee8cbedbe2118b5686372fb33c297fcd6379b050cca0ef13a597382a"
+                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
+                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.5.18.1"
+            "version": "==2022.12.7"
         },
         "cffi": {
             "hashes": [
-                "sha256:00c878c90cb53ccfaae6b8bc18ad05d2036553e6d9d1d9dbcf323bbe83854ca3",
-                "sha256:0104fb5ae2391d46a4cb082abdd5c69ea4eab79d8d44eaaf79f1b1fd806ee4c2",
-                "sha256:06c48159c1abed75c2e721b1715c379fa3200c7784271b3c46df01383b593636",
-                "sha256:0808014eb713677ec1292301ea4c81ad277b6cdf2fdd90fd540af98c0b101d20",
-                "sha256:10dffb601ccfb65262a27233ac273d552ddc4d8ae1bf93b21c94b8511bffe728",
-                "sha256:14cd121ea63ecdae71efa69c15c5543a4b5fbcd0bbe2aad864baca0063cecf27",
-                "sha256:17771976e82e9f94976180f76468546834d22a7cc404b17c22df2a2c81db0c66",
-                "sha256:181dee03b1170ff1969489acf1c26533710231c58f95534e3edac87fff06c443",
-                "sha256:23cfe892bd5dd8941608f93348c0737e369e51c100d03718f108bf1add7bd6d0",
-                "sha256:263cc3d821c4ab2213cbe8cd8b355a7f72a8324577dc865ef98487c1aeee2bc7",
-                "sha256:2756c88cbb94231c7a147402476be2c4df2f6078099a6f4a480d239a8817ae39",
-                "sha256:27c219baf94952ae9d50ec19651a687b826792055353d07648a5695413e0c605",
-                "sha256:2a23af14f408d53d5e6cd4e3d9a24ff9e05906ad574822a10563efcef137979a",
-                "sha256:31fb708d9d7c3f49a60f04cf5b119aeefe5644daba1cd2a0fe389b674fd1de37",
-                "sha256:3415c89f9204ee60cd09b235810be700e993e343a408693e80ce7f6a40108029",
-                "sha256:3773c4d81e6e818df2efbc7dd77325ca0dcb688116050fb2b3011218eda36139",
-                "sha256:3b96a311ac60a3f6be21d2572e46ce67f09abcf4d09344c49274eb9e0bf345fc",
-                "sha256:3f7d084648d77af029acb79a0ff49a0ad7e9d09057a9bf46596dac9514dc07df",
-                "sha256:41d45de54cd277a7878919867c0f08b0cf817605e4eb94093e7516505d3c8d14",
-                "sha256:4238e6dab5d6a8ba812de994bbb0a79bddbdf80994e4ce802b6f6f3142fcc880",
-                "sha256:45db3a33139e9c8f7c09234b5784a5e33d31fd6907800b316decad50af323ff2",
-                "sha256:45e8636704eacc432a206ac7345a5d3d2c62d95a507ec70d62f23cd91770482a",
-                "sha256:4958391dbd6249d7ad855b9ca88fae690783a6be9e86df65865058ed81fc860e",
-                "sha256:4a306fa632e8f0928956a41fa8e1d6243c71e7eb59ffbd165fc0b41e316b2474",
-                "sha256:57e9ac9ccc3101fac9d6014fba037473e4358ef4e89f8e181f8951a2c0162024",
-                "sha256:59888172256cac5629e60e72e86598027aca6bf01fa2465bdb676d37636573e8",
-                "sha256:5e069f72d497312b24fcc02073d70cb989045d1c91cbd53979366077959933e0",
-                "sha256:64d4ec9f448dfe041705426000cc13e34e6e5bb13736e9fd62e34a0b0c41566e",
-                "sha256:6dc2737a3674b3e344847c8686cf29e500584ccad76204efea14f451d4cc669a",
-                "sha256:74fdfdbfdc48d3f47148976f49fab3251e550a8720bebc99bf1483f5bfb5db3e",
-                "sha256:75e4024375654472cc27e91cbe9eaa08567f7fbdf822638be2814ce059f58032",
-                "sha256:786902fb9ba7433aae840e0ed609f45c7bcd4e225ebb9c753aa39725bb3e6ad6",
-                "sha256:8b6c2ea03845c9f501ed1313e78de148cd3f6cad741a75d43a29b43da27f2e1e",
-                "sha256:91d77d2a782be4274da750752bb1650a97bfd8f291022b379bb8e01c66b4e96b",
-                "sha256:91ec59c33514b7c7559a6acda53bbfe1b283949c34fe7440bcf917f96ac0723e",
-                "sha256:920f0d66a896c2d99f0adbb391f990a84091179542c205fa53ce5787aff87954",
-                "sha256:a5263e363c27b653a90078143adb3d076c1a748ec9ecc78ea2fb916f9b861962",
-                "sha256:abb9a20a72ac4e0fdb50dae135ba5e77880518e742077ced47eb1499e29a443c",
-                "sha256:c2051981a968d7de9dd2d7b87bcb9c939c74a34626a6e2f8181455dd49ed69e4",
-                "sha256:c21c9e3896c23007803a875460fb786118f0cdd4434359577ea25eb556e34c55",
-                "sha256:c2502a1a03b6312837279c8c1bd3ebedf6c12c4228ddbad40912d671ccc8a962",
-                "sha256:d4d692a89c5cf08a8557fdeb329b82e7bf609aadfaed6c0d79f5a449a3c7c023",
-                "sha256:da5db4e883f1ce37f55c667e5c0de439df76ac4cb55964655906306918e7363c",
-                "sha256:e7022a66d9b55e93e1a845d8c9eba2a1bebd4966cd8bfc25d9cd07d515b33fa6",
-                "sha256:ef1f279350da2c586a69d32fc8733092fd32cc8ac95139a00377841f59a3f8d8",
-                "sha256:f54a64f8b0c8ff0b64d18aa76675262e1700f3995182267998c31ae974fbc382",
-                "sha256:f5c7150ad32ba43a07c4479f40241756145a1f03b43480e058cfd862bf5041c7",
-                "sha256:f6f824dc3bce0edab5f427efcfb1d63ee75b6fcb7282900ccaf925be84efb0fc",
-                "sha256:fd8a250edc26254fe5b33be00402e6d287f562b6a5b2152dec302fa15bb3e997",
-                "sha256:ffaa5c925128e29efbde7301d8ecaf35c8c60ffbcd6a1ffd3a552177c8e5e796"
+                "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
+                "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
+                "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
+                "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
+                "sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405",
+                "sha256:198caafb44239b60e252492445da556afafc7d1e3ab7a1fb3f0584ef6d742375",
+                "sha256:1e74c6b51a9ed6589199c787bf5f9875612ca4a8a0785fb2d4a84429badaf22a",
+                "sha256:2012c72d854c2d03e45d06ae57f40d78e5770d252f195b93f581acf3ba44496e",
+                "sha256:21157295583fe8943475029ed5abdcf71eb3911894724e360acff1d61c1d54bc",
+                "sha256:2470043b93ff09bf8fb1d46d1cb756ce6132c54826661a32d4e4d132e1977adf",
+                "sha256:285d29981935eb726a4399badae8f0ffdff4f5050eaa6d0cfc3f64b857b77185",
+                "sha256:30d78fbc8ebf9c92c9b7823ee18eb92f2e6ef79b45ac84db507f52fbe3ec4497",
+                "sha256:320dab6e7cb2eacdf0e658569d2575c4dad258c0fcc794f46215e1e39f90f2c3",
+                "sha256:33ab79603146aace82c2427da5ca6e58f2b3f2fb5da893ceac0c42218a40be35",
+                "sha256:3548db281cd7d2561c9ad9984681c95f7b0e38881201e157833a2342c30d5e8c",
+                "sha256:3799aecf2e17cf585d977b780ce79ff0dc9b78d799fc694221ce814c2c19db83",
+                "sha256:39d39875251ca8f612b6f33e6b1195af86d1b3e60086068be9cc053aa4376e21",
+                "sha256:3b926aa83d1edb5aa5b427b4053dc420ec295a08e40911296b9eb1b6170f6cca",
+                "sha256:3bcde07039e586f91b45c88f8583ea7cf7a0770df3a1649627bf598332cb6984",
+                "sha256:3d08afd128ddaa624a48cf2b859afef385b720bb4b43df214f85616922e6a5ac",
+                "sha256:3eb6971dcff08619f8d91607cfc726518b6fa2a9eba42856be181c6d0d9515fd",
+                "sha256:40f4774f5a9d4f5e344f31a32b5096977b5d48560c5592e2f3d2c4374bd543ee",
+                "sha256:4289fc34b2f5316fbb762d75362931e351941fa95fa18789191b33fc4cf9504a",
+                "sha256:470c103ae716238bbe698d67ad020e1db9d9dba34fa5a899b5e21577e6d52ed2",
+                "sha256:4f2c9f67e9821cad2e5f480bc8d83b8742896f1242dba247911072d4fa94c192",
+                "sha256:50a74364d85fd319352182ef59c5c790484a336f6db772c1a9231f1c3ed0cbd7",
+                "sha256:54a2db7b78338edd780e7ef7f9f6c442500fb0d41a5a4ea24fff1c929d5af585",
+                "sha256:5635bd9cb9731e6d4a1132a498dd34f764034a8ce60cef4f5319c0541159392f",
+                "sha256:59c0b02d0a6c384d453fece7566d1c7e6b7bae4fc5874ef2ef46d56776d61c9e",
+                "sha256:5d598b938678ebf3c67377cdd45e09d431369c3b1a5b331058c338e201f12b27",
+                "sha256:5df2768244d19ab7f60546d0c7c63ce1581f7af8b5de3eb3004b9b6fc8a9f84b",
+                "sha256:5ef34d190326c3b1f822a5b7a45f6c4535e2f47ed06fec77d3d799c450b2651e",
+                "sha256:6975a3fac6bc83c4a65c9f9fcab9e47019a11d3d2cf7f3c0d03431bf145a941e",
+                "sha256:6c9a799e985904922a4d207a94eae35c78ebae90e128f0c4e521ce339396be9d",
+                "sha256:70df4e3b545a17496c9b3f41f5115e69a4f2e77e94e1d2a8e1070bc0c38c8a3c",
+                "sha256:7473e861101c9e72452f9bf8acb984947aa1661a7704553a9f6e4baa5ba64415",
+                "sha256:8102eaf27e1e448db915d08afa8b41d6c7ca7a04b7d73af6514df10a3e74bd82",
+                "sha256:87c450779d0914f2861b8526e035c5e6da0a3199d8f1add1a665e1cbc6fc6d02",
+                "sha256:8b7ee99e510d7b66cdb6c593f21c043c248537a32e0bedf02e01e9553a172314",
+                "sha256:91fc98adde3d7881af9b59ed0294046f3806221863722ba7d8d120c575314325",
+                "sha256:94411f22c3985acaec6f83c6df553f2dbe17b698cc7f8ae751ff2237d96b9e3c",
+                "sha256:98d85c6a2bef81588d9227dde12db8a7f47f639f4a17c9ae08e773aa9c697bf3",
+                "sha256:9ad5db27f9cabae298d151c85cf2bad1d359a1b9c686a275df03385758e2f914",
+                "sha256:a0b71b1b8fbf2b96e41c4d990244165e2c9be83d54962a9a1d118fd8657d2045",
+                "sha256:a0f100c8912c114ff53e1202d0078b425bee3649ae34d7b070e9697f93c5d52d",
+                "sha256:a591fe9e525846e4d154205572a029f653ada1a78b93697f3b5a8f1f2bc055b9",
+                "sha256:a5c84c68147988265e60416b57fc83425a78058853509c1b0629c180094904a5",
+                "sha256:a66d3508133af6e8548451b25058d5812812ec3798c886bf38ed24a98216fab2",
+                "sha256:a8c4917bd7ad33e8eb21e9a5bbba979b49d9a97acb3a803092cbc1133e20343c",
+                "sha256:b3bbeb01c2b273cca1e1e0c5df57f12dce9a4dd331b4fa1635b8bec26350bde3",
+                "sha256:cba9d6b9a7d64d4bd46167096fc9d2f835e25d7e4c121fb2ddfc6528fb0413b2",
+                "sha256:cc4d65aeeaa04136a12677d3dd0b1c0c94dc43abac5860ab33cceb42b801c1e8",
+                "sha256:ce4bcc037df4fc5e3d184794f27bdaab018943698f4ca31630bc7f84a7b69c6d",
+                "sha256:cec7d9412a9102bdc577382c3929b337320c4c4c4849f2c5cdd14d7368c5562d",
+                "sha256:d400bfb9a37b1351253cb402671cea7e89bdecc294e8016a707f6d1d8ac934f9",
+                "sha256:d61f4695e6c866a23a21acab0509af1cdfd2c013cf256bbf5b6b5e2695827162",
+                "sha256:db0fbb9c62743ce59a9ff687eb5f4afbe77e5e8403d6697f7446e5f609976f76",
+                "sha256:dd86c085fae2efd48ac91dd7ccffcfc0571387fe1193d33b6394db7ef31fe2a4",
+                "sha256:e00b098126fd45523dd056d2efba6c5a63b71ffe9f2bbe1a4fe1716e1d0c331e",
+                "sha256:e229a521186c75c8ad9490854fd8bbdd9a0c9aa3a524326b55be83b54d4e0ad9",
+                "sha256:e263d77ee3dd201c3a142934a086a4450861778baaeeb45db4591ef65550b0a6",
+                "sha256:ed9cb427ba5504c1dc15ede7d516b84757c3e3d7868ccc85121d9310d27eed0b",
+                "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01",
+                "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"
+            ],
+            "version": "==1.15.1"
+        },
+        "cfgv": {
+            "hashes": [
+                "sha256:c6a0883f3917a037485059700b9e75da2464e6c27051014ad85ba6aaa5884426",
+                "sha256:f5a830efb9ce7a445376bb66ec94c638a9787422f96264c98edc6bdeed8ab736"
             ],
-            "version": "==1.15.0"
+            "markers": "python_full_version >= '3.6.1'",
+            "version": "==3.3.1"
         },
         "charset-normalizer": {
             "hashes": [
                 "sha256:2857e29ff0d34db842cd7ca3230549d1a697f96ee6d3fb071cfa6c7393832597",
                 "sha256:6881edbebdb17b39b4eaaa821b438bf6eddffb4468cf344f09f89def34a8b1df"
             ],
             "markers": "python_version >= '3'",
             "version": "==2.0.12"
         },
-        "commonmark": {
+        "cryptography": {
             "hashes": [
-                "sha256:452f9dc859be7f06631ddcb328b6919c67984aca654e5fefb3914d54691aed60",
-                "sha256:da2f38c92590f83de410ba1a3cbceafbc74fee9def35f9251ba9a971d6d66fd9"
+                "sha256:0f8da300b5c8af9f98111ffd512910bc792b4c77392a9523624680f7956a99d4",
+                "sha256:35f7c7d015d474f4011e859e93e789c87d21f6f4880ebdc29896a60403328f1f",
+                "sha256:4789d1e3e257965e960232345002262ede4d094d1a19f4d3b52e48d4d8f3b885",
+                "sha256:5aa67414fcdfa22cf052e640cb5ddc461924a045cacf325cd164e65312d99502",
+                "sha256:5d2d8b87a490bfcd407ed9d49093793d0f75198a35e6eb1a923ce1ee86c62b41",
+                "sha256:6687ef6d0a6497e2b58e7c5b852b53f62142cfa7cd1555795758934da363a965",
+                "sha256:6f8ba7f0328b79f08bdacc3e4e66fb4d7aab0c3584e0bd41328dce5262e26b2e",
+                "sha256:706843b48f9a3f9b9911979761c91541e3d90db1ca905fd63fee540a217698bc",
+                "sha256:807ce09d4434881ca3a7594733669bd834f5b2c6d5c7e36f8c00f691887042ad",
+                "sha256:83e17b26de248c33f3acffb922748151d71827d6021d98c70e6c1a25ddd78505",
+                "sha256:96f1157a7c08b5b189b16b47bc9db2332269d6680a196341bf30046330d15388",
+                "sha256:aec5a6c9864be7df2240c382740fcf3b96928c46604eaa7f3091f58b878c0bb6",
+                "sha256:b0afd054cd42f3d213bf82c629efb1ee5f22eba35bf0eec88ea9ea7304f511a2",
+                "sha256:c5caeb8188c24888c90b5108a441c106f7faa4c4c075a2bcae438c6e8ca73cef",
+                "sha256:ced4e447ae29ca194449a3f1ce132ded8fcab06971ef5f618605aacaa612beac",
+                "sha256:d1f6198ee6d9148405e49887803907fe8962a23e6c6f83ea7d98f1c0de375695",
+                "sha256:e124352fd3db36a9d4a21c1aa27fd5d051e621845cb87fb851c08f4f75ce8be6",
+                "sha256:e422abdec8b5fa8462aa016786680720d78bdce7a30c652b7fadf83a4ba35336",
+                "sha256:ef8b72fa70b348724ff1218267e7f7375b8de4e8194d1636ee60510aae104cd0",
+                "sha256:f0c64d1bd842ca2633e74a1a28033d139368ad959872533b1bab8c80e8240a0c",
+                "sha256:f24077a3b5298a5a06a8e0536e3ea9ec60e4c7ac486755e5fb6e6ea9b3500106",
+                "sha256:fdd188c8a6ef8769f148f88f859884507b954cc64db6b52f66ef199bb9ad660a",
+                "sha256:fe913f20024eb2cb2f323e42a64bdf2911bb9738a15dba7d3cce48151034e3a8"
             ],
-            "version": "==0.9.1"
+            "index": "pypi",
+            "version": "==39.0.1"
         },
-        "cryptography": {
+        "distlib": {
             "hashes": [
-                "sha256:093cb351031656d3ee2f4fa1be579a8c69c754cf874206be1d4cf3b542042804",
-                "sha256:0cc20f655157d4cfc7bada909dc5cc228211b075ba8407c46467f63597c78178",
-                "sha256:1b9362d34363f2c71b7853f6251219298124aa4cc2075ae2932e64c91a3e2717",
-                "sha256:1f3bfbd611db5cb58ca82f3deb35e83af34bb8cf06043fa61500157d50a70982",
-                "sha256:2bd1096476aaac820426239ab534b636c77d71af66c547b9ddcd76eb9c79e004",
-                "sha256:31fe38d14d2e5f787e0aecef831457da6cec68e0bb09a35835b0b44ae8b988fe",
-                "sha256:3b8398b3d0efc420e777c40c16764d6870bcef2eb383df9c6dbb9ffe12c64452",
-                "sha256:3c81599befb4d4f3d7648ed3217e00d21a9341a9a688ecdd615ff72ffbed7336",
-                "sha256:419c57d7b63f5ec38b1199a9521d77d7d1754eb97827bbb773162073ccd8c8d4",
-                "sha256:46f4c544f6557a2fefa7ac8ac7d1b17bf9b647bd20b16decc8fbcab7117fbc15",
-                "sha256:471e0d70201c069f74c837983189949aa0d24bb2d751b57e26e3761f2f782b8d",
-                "sha256:59b281eab51e1b6b6afa525af2bd93c16d49358404f814fe2c2410058623928c",
-                "sha256:731c8abd27693323b348518ed0e0705713a36d79fdbd969ad968fbef0979a7e0",
-                "sha256:95e590dd70642eb2079d280420a888190aa040ad20f19ec8c6e097e38aa29e06",
-                "sha256:a68254dd88021f24a68b613d8c51d5c5e74d735878b9e32cc0adf19d1f10aaf9",
-                "sha256:a7d5137e556cc0ea418dca6186deabe9129cee318618eb1ffecbd35bee55ddc1",
-                "sha256:aeaba7b5e756ea52c8861c133c596afe93dd716cbcacae23b80bc238202dc023",
-                "sha256:dc26bb134452081859aa21d4990474ddb7e863aa39e60d1592800a8865a702de",
-                "sha256:e53258e69874a306fcecb88b7534d61820db8a98655662a3dd2ec7f1afd9132f",
-                "sha256:ef15c2df7656763b4ff20a9bc4381d8352e6640cfeb95c2972c38ef508e75181",
-                "sha256:f224ad253cc9cea7568f49077007d2263efa57396a2f2f78114066fd54b5c68e",
-                "sha256:f8ec91983e638a9bcd75b39f1396e5c0dc2330cbd9ce4accefe68717e6779e0a"
+                "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
+                "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==37.0.2"
+            "version": "==0.3.6"
         },
         "docutils": {
             "hashes": [
                 "sha256:23010f129180089fbcd3bc08cfefccb3b890b0050e1ca00c867036e9d161b98c",
                 "sha256:679987caf361a7539d76e584cbeddc311e3aee937877c87346f31debc63e9d06"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
             "version": "==0.18.1"
         },
+        "filelock": {
+            "hashes": [
+                "sha256:7b319f24340b51f55a2bf7a12ac0755a9b03e718311dac567a0f4f7fabd2f5de",
+                "sha256:f58d535af89bb9ad5cd4df046f741f8553a418c01a7856bf0d173bbc9f6bd16d"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==3.9.0"
+        },
         "flake8": {
             "hashes": [
                 "sha256:479b1304f72536a55948cb40a32dce8bb0ffe3501e26eaf292c7e60eb5e0428d",
                 "sha256:806e034dda44114815e23c16ef92f95c91e4c71100ff52813adf7132a6ad870d"
             ],
             "index": "pypi",
             "version": "==4.0.1"
         },
+        "identify": {
+            "hashes": [
+                "sha256:89e144fa560cc4cffb6ef2ab5e9fb18ed9f9b3cb054384bab4b95c12f6c309fe",
+                "sha256:93aac7ecf2f6abf879b8f29a8002d3c6de7086b8c28d88e1ad15045a15ab63f9"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==2.5.18"
+        },
         "idna": {
             "hashes": [
-                "sha256:84d9dd047ffa80596e0f246e2eab0b391788b0503584e8945f2368256d2735ff",
-                "sha256:9d643ff0a55b762d5cdb124b8eaa99c66322e2157b69160bc32796e824360e6d"
+                "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
+                "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3'",
-            "version": "==3.3"
+            "version": "==3.4"
         },
         "imagesize": {
             "hashes": [
-                "sha256:1db2f82529e53c3e929e8926a1fa9235aa82d0bd0c580359c67ec31b2fddaa8c",
-                "sha256:cd1750d452385ca327479d45b64d9c7729ecf0b3969a58148298c77092261f9d"
+                "sha256:0d8d18d08f840c19d0ee7ca1fd82490fdc3729b7ac93f49870406ddde8ef8d8b",
+                "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==1.3.0"
+            "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:5d26852efe48c0a32b0509ffbc583fda1a2266545a78d104a6f4aff3db17d700",
-                "sha256:c58c8eb8a762858f49e18436ff552e83914778e50e9d2f1660535ffb364552ec"
+                "sha256:7efb448ec9a5e313a57655d35aa54cd3e01b7e1fbcf72dce1bf06119420f5bad",
+                "sha256:e354bedeb60efa6affdcc8ae121b73544a7aa74156d047311948f6d711cd378d"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==6.0.0"
+        },
+        "jaraco.classes": {
+            "hashes": [
+                "sha256:2353de3288bc6b82120752201c6b1c1a14b058267fa424ed5ce5984e3b922158",
+                "sha256:89559fa5c1d3c34eff6f631ad80bb21f378dbcbb35dd161fd2c6b93f5be2f98a"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==4.11.4"
+            "version": "==3.2.3"
         },
         "jeepney": {
             "hashes": [
                 "sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806",
                 "sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755"
             ],
             "markers": "sys_platform == 'linux'",
@@ -249,87 +297,146 @@
                 "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.1.2"
         },
         "keyring": {
             "hashes": [
-                "sha256:9ef58314bcc823f426b49ec787539a2d73571b37de4cd498f839803b01acff1e",
-                "sha256:dee502cdf18a98211bef428eea11456a33c00718b2f08524fd5727c7f424bffd"
+                "sha256:771ed2a91909389ed6148631de678f82ddc73737d85a927f382a8a1b157898cd",
+                "sha256:ba2e15a9b35e21908d0aaf4e0a47acc52d6ae33444df0da2b49d41a46ef6d678"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.5.1"
+            "version": "==23.13.1"
+        },
+        "markdown-it-py": {
+            "hashes": [
+                "sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30",
+                "sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==2.2.0"
         },
         "markupsafe": {
             "hashes": [
-                "sha256:0212a68688482dc52b2d45013df70d169f542b7394fc744c02a57374a4207003",
-                "sha256:089cf3dbf0cd6c100f02945abeb18484bd1ee57a079aefd52cffd17fba910b88",
-                "sha256:10c1bfff05d95783da83491be968e8fe789263689c02724e0c691933c52994f5",
-                "sha256:33b74d289bd2f5e527beadcaa3f401e0df0a89927c1559c8566c066fa4248ab7",
-                "sha256:3799351e2336dc91ea70b034983ee71cf2f9533cdff7c14c90ea126bfd95d65a",
-                "sha256:3ce11ee3f23f79dbd06fb3d63e2f6af7b12db1d46932fe7bd8afa259a5996603",
-                "sha256:421be9fbf0ffe9ffd7a378aafebbf6f4602d564d34be190fc19a193232fd12b1",
-                "sha256:43093fb83d8343aac0b1baa75516da6092f58f41200907ef92448ecab8825135",
-                "sha256:46d00d6cfecdde84d40e572d63735ef81423ad31184100411e6e3388d405e247",
-                "sha256:4a33dea2b688b3190ee12bd7cfa29d39c9ed176bda40bfa11099a3ce5d3a7ac6",
-                "sha256:4b9fe39a2ccc108a4accc2676e77da025ce383c108593d65cc909add5c3bd601",
-                "sha256:56442863ed2b06d19c37f94d999035e15ee982988920e12a5b4ba29b62ad1f77",
-                "sha256:671cd1187ed5e62818414afe79ed29da836dde67166a9fac6d435873c44fdd02",
-                "sha256:694deca8d702d5db21ec83983ce0bb4b26a578e71fbdbd4fdcd387daa90e4d5e",
-                "sha256:6a074d34ee7a5ce3effbc526b7083ec9731bb3cbf921bbe1d3005d4d2bdb3a63",
-                "sha256:6d0072fea50feec76a4c418096652f2c3238eaa014b2f94aeb1d56a66b41403f",
-                "sha256:6fbf47b5d3728c6aea2abb0589b5d30459e369baa772e0f37a0320185e87c980",
-                "sha256:7f91197cc9e48f989d12e4e6fbc46495c446636dfc81b9ccf50bb0ec74b91d4b",
-                "sha256:86b1f75c4e7c2ac2ccdaec2b9022845dbb81880ca318bb7a0a01fbf7813e3812",
-                "sha256:8dc1c72a69aa7e082593c4a203dcf94ddb74bb5c8a731e4e1eb68d031e8498ff",
-                "sha256:8e3dcf21f367459434c18e71b2a9532d96547aef8a871872a5bd69a715c15f96",
-                "sha256:8e576a51ad59e4bfaac456023a78f6b5e6e7651dcd383bcc3e18d06f9b55d6d1",
-                "sha256:96e37a3dc86e80bf81758c152fe66dbf60ed5eca3d26305edf01892257049925",
-                "sha256:97a68e6ada378df82bc9f16b800ab77cbf4b2fada0081794318520138c088e4a",
-                "sha256:99a2a507ed3ac881b975a2976d59f38c19386d128e7a9a18b7df6fff1fd4c1d6",
-                "sha256:a49907dd8420c5685cfa064a1335b6754b74541bbb3706c259c02ed65b644b3e",
-                "sha256:b09bf97215625a311f669476f44b8b318b075847b49316d3e28c08e41a7a573f",
-                "sha256:b7bd98b796e2b6553da7225aeb61f447f80a1ca64f41d83612e6139ca5213aa4",
-                "sha256:b87db4360013327109564f0e591bd2a3b318547bcef31b468a92ee504d07ae4f",
-                "sha256:bcb3ed405ed3222f9904899563d6fc492ff75cce56cba05e32eff40e6acbeaa3",
-                "sha256:d4306c36ca495956b6d568d276ac11fdd9c30a36f1b6eb928070dc5360b22e1c",
-                "sha256:d5ee4f386140395a2c818d149221149c54849dfcfcb9f1debfe07a8b8bd63f9a",
-                "sha256:dda30ba7e87fbbb7eab1ec9f58678558fd9a6b8b853530e176eabd064da81417",
-                "sha256:e04e26803c9c3851c931eac40c695602c6295b8d432cbe78609649ad9bd2da8a",
-                "sha256:e1c0b87e09fa55a220f058d1d49d3fb8df88fbfab58558f1198e08c1e1de842a",
-                "sha256:e72591e9ecd94d7feb70c1cbd7be7b3ebea3f548870aa91e2732960fa4d57a37",
-                "sha256:e8c843bbcda3a2f1e3c2ab25913c80a3c5376cd00c6e8c4a86a89a28c8dc5452",
-                "sha256:efc1913fd2ca4f334418481c7e595c00aad186563bbc1ec76067848c7ca0a933",
-                "sha256:f121a1420d4e173a5d96e47e9a0c0dcff965afdf1626d28de1460815f7c4ee7a",
-                "sha256:fc7b548b17d238737688817ab67deebb30e8073c95749d55538ed473130ec0c7"
+                "sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed",
+                "sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc",
+                "sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2",
+                "sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460",
+                "sha256:137678c63c977754abe9086a3ec011e8fd985ab90631145dfb9294ad09c102a7",
+                "sha256:1bea30e9bf331f3fef67e0a3877b2288593c98a21ccb2cf29b74c581a4eb3af0",
+                "sha256:22152d00bf4a9c7c83960521fc558f55a1adbc0631fbb00a9471e097b19d72e1",
+                "sha256:22731d79ed2eb25059ae3df1dfc9cb1546691cc41f4e3130fe6bfbc3ecbbecfa",
+                "sha256:2298c859cfc5463f1b64bd55cb3e602528db6fa0f3cfd568d3605c50678f8f03",
+                "sha256:28057e985dace2f478e042eaa15606c7efccb700797660629da387eb289b9323",
+                "sha256:2e7821bffe00aa6bd07a23913b7f4e01328c3d5cc0b40b36c0bd81d362faeb65",
+                "sha256:2ec4f2d48ae59bbb9d1f9d7efb9236ab81429a764dedca114f5fdabbc3788013",
+                "sha256:340bea174e9761308703ae988e982005aedf427de816d1afe98147668cc03036",
+                "sha256:40627dcf047dadb22cd25ea7ecfe9cbf3bbbad0482ee5920b582f3809c97654f",
+                "sha256:40dfd3fefbef579ee058f139733ac336312663c6706d1163b82b3003fb1925c4",
+                "sha256:4cf06cdc1dda95223e9d2d3c58d3b178aa5dacb35ee7e3bbac10e4e1faacb419",
+                "sha256:50c42830a633fa0cf9e7d27664637532791bfc31c731a87b202d2d8ac40c3ea2",
+                "sha256:55f44b440d491028addb3b88f72207d71eeebfb7b5dbf0643f7c023ae1fba619",
+                "sha256:608e7073dfa9e38a85d38474c082d4281f4ce276ac0010224eaba11e929dd53a",
+                "sha256:63ba06c9941e46fa389d389644e2d8225e0e3e5ebcc4ff1ea8506dce646f8c8a",
+                "sha256:65608c35bfb8a76763f37036547f7adfd09270fbdbf96608be2bead319728fcd",
+                "sha256:665a36ae6f8f20a4676b53224e33d456a6f5a72657d9c83c2aa00765072f31f7",
+                "sha256:6d6607f98fcf17e534162f0709aaad3ab7a96032723d8ac8750ffe17ae5a0666",
+                "sha256:7313ce6a199651c4ed9d7e4cfb4aa56fe923b1adf9af3b420ee14e6d9a73df65",
+                "sha256:7668b52e102d0ed87cb082380a7e2e1e78737ddecdde129acadb0eccc5423859",
+                "sha256:7df70907e00c970c60b9ef2938d894a9381f38e6b9db73c5be35e59d92e06625",
+                "sha256:7e007132af78ea9df29495dbf7b5824cb71648d7133cf7848a2a5dd00d36f9ff",
+                "sha256:835fb5e38fd89328e9c81067fd642b3593c33e1e17e2fdbf77f5676abb14a156",
+                "sha256:8bca7e26c1dd751236cfb0c6c72d4ad61d986e9a41bbf76cb445f69488b2a2bd",
+                "sha256:8db032bf0ce9022a8e41a22598eefc802314e81b879ae093f36ce9ddf39ab1ba",
+                "sha256:99625a92da8229df6d44335e6fcc558a5037dd0a760e11d84be2260e6f37002f",
+                "sha256:9cad97ab29dfc3f0249b483412c85c8ef4766d96cdf9dcf5a1e3caa3f3661cf1",
+                "sha256:a4abaec6ca3ad8660690236d11bfe28dfd707778e2442b45addd2f086d6ef094",
+                "sha256:a6e40afa7f45939ca356f348c8e23048e02cb109ced1eb8420961b2f40fb373a",
+                "sha256:a6f2fcca746e8d5910e18782f976489939d54a91f9411c32051b4aab2bd7c513",
+                "sha256:a806db027852538d2ad7555b203300173dd1b77ba116de92da9afbc3a3be3eed",
+                "sha256:abcabc8c2b26036d62d4c746381a6f7cf60aafcc653198ad678306986b09450d",
+                "sha256:b8526c6d437855442cdd3d87eede9c425c4445ea011ca38d937db299382e6fa3",
+                "sha256:bb06feb762bade6bf3c8b844462274db0c76acc95c52abe8dbed28ae3d44a147",
+                "sha256:c0a33bc9f02c2b17c3ea382f91b4db0e6cde90b63b296422a939886a7a80de1c",
+                "sha256:c4a549890a45f57f1ebf99c067a4ad0cb423a05544accaf2b065246827ed9603",
+                "sha256:ca244fa73f50a800cf8c3ebf7fd93149ec37f5cb9596aa8873ae2c1d23498601",
+                "sha256:cf877ab4ed6e302ec1d04952ca358b381a882fbd9d1b07cccbfd61783561f98a",
+                "sha256:d9d971ec1e79906046aa3ca266de79eac42f1dbf3612a05dc9368125952bd1a1",
+                "sha256:da25303d91526aac3672ee6d49a2f3db2d9502a4a60b55519feb1a4c7714e07d",
+                "sha256:e55e40ff0cc8cc5c07996915ad367fa47da6b3fc091fdadca7f5403239c5fec3",
+                "sha256:f03a532d7dee1bed20bc4884194a16160a2de9ffc6354b3878ec9682bb623c54",
+                "sha256:f1cd098434e83e656abf198f103a8207a8187c0fc110306691a2e94a78d0abb2",
+                "sha256:f2bfb563d0211ce16b63c7cb9395d2c682a23187f54c3d79bfec33e6705473c6",
+                "sha256:f8ffb705ffcf5ddd0e80b65ddf7bed7ee4f5a441ea7d3419e861a12eaf41af58"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.1.1"
+            "version": "==2.1.2"
         },
         "mccabe": {
             "hashes": [
                 "sha256:ab8a6258860da4b6677da4bd2fe5dc2c659cff31b3ee4f7f5d64e79735b80d42",
                 "sha256:dd8d182285a0fe56bace7f45b5e7d1a6ebcbf524e8f3bd87eb0f125271b8831f"
             ],
             "version": "==0.6.1"
         },
+        "mdurl": {
+            "hashes": [
+                "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8",
+                "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==0.1.2"
+        },
+        "more-itertools": {
+            "hashes": [
+                "sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d",
+                "sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==9.1.0"
+        },
+        "nodeenv": {
+            "hashes": [
+                "sha256:27083a7b96a25f2f5e1d8cb4b6317ee8aeda3bdd121394e5ac54e498028a042e",
+                "sha256:e0e7f7dfb85fc5394c6fe1e8fa98131a2473e04311a45afb6508f7cf1836fa2b"
+            ],
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
+            "version": "==1.7.0"
+        },
         "packaging": {
             "hashes": [
-                "sha256:dd47c42927d89ab911e606518907cc2d3a1f38bbd026385970643f9c5b8ecfeb",
-                "sha256:ef103e05f519cdc783ae24ea4e2e0f508a9c99b2d4969652eed6a2e1ea5bd522"
+                "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
+                "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==21.3"
+            "markers": "python_version >= '3.7'",
+            "version": "==23.0"
         },
         "pkginfo": {
             "hashes": [
-                "sha256:542e0d0b6750e2e21c20179803e40ab50598d8066d51097a0e382cba9eb02bff",
-                "sha256:c24c487c6a7f72c66e816ab1796b96ac6c3d14d49338293d2141664330b55ffc"
+                "sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546",
+                "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
             ],
-            "version": "==1.8.2"
+            "markers": "python_version >= '3.6'",
+            "version": "==1.9.6"
+        },
+        "platformdirs": {
+            "hashes": [
+                "sha256:13b08a53ed71021350c9e300d4ea8668438fb0046ab3937ac9a29913a1a1350a",
+                "sha256:accc3665857288317f32c7bebb5a8e482ba717b474f3fc1d18ca7f9214be0cef"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==3.1.0"
+        },
+        "pre-commit": {
+            "hashes": [
+                "sha256:10c62741aa5704faea2ad69cb550ca78082efe5697d6f04e5710c3c229afdd10",
+                "sha256:4233a1e38621c87d9dda9808c6606d7e7ba0e087cd56d3fe03202a01d2919615"
+            ],
+            "index": "pypi",
+            "version": "==2.19.0"
         },
         "pycodestyle": {
             "hashes": [
                 "sha256:720f8b39dde8b293825e7ff02c475f3077124006db4f440dcbc9a20b76548a20",
                 "sha256:eddd5847ef438ea1c7870ca7eb78a9d47ce0cdb4851a5523949f2601d0cbbe7f"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
@@ -348,89 +455,121 @@
                 "sha256:3bb3a3f256f4b7968c9c788781e4ff07dce46bdf12339dcda61053375426ee2e"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==2.4.0"
         },
         "pygments": {
             "hashes": [
-                "sha256:5eb116118f9612ff1ee89ac96437bb6b49e8f04d8a13b514ba26f620208e26eb",
-                "sha256:dc9c10fb40944260f6ed4c688ece0cd2048414940f1cea51b8b226318411c519"
+                "sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297",
+                "sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2.12.0"
+            "version": "==2.14.0"
         },
-        "pyparsing": {
+        "pyyaml": {
             "hashes": [
-                "sha256:2b020ecf7d21b687f219b71ecad3631f644a47f01403fa1d1036b0c6416d70fb",
-                "sha256:5026bae9a10eeaefb61dab2f09052b9f4307d44aee4eda64b309723d8d206bbc"
+                "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
+                "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
+                "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
+                "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
+                "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
+                "sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4",
+                "sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07",
+                "sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba",
+                "sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9",
+                "sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287",
+                "sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513",
+                "sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0",
+                "sha256:432557aa2c09802be39460360ddffd48156e30721f5e8d917f01d31694216782",
+                "sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0",
+                "sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92",
+                "sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f",
+                "sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2",
+                "sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc",
+                "sha256:81957921f441d50af23654aa6c5e5eaf9b06aba7f0a19c18a538dc7ef291c5a1",
+                "sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c",
+                "sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86",
+                "sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4",
+                "sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c",
+                "sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34",
+                "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b",
+                "sha256:afa17f5bc4d1b10afd4466fd3a44dc0e245382deca5b3c353d8b757f9e3ecb8d",
+                "sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c",
+                "sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb",
+                "sha256:bfaef573a63ba8923503d27530362590ff4f576c626d86a9fed95822a8255fd7",
+                "sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737",
+                "sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3",
+                "sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d",
+                "sha256:d4b0ba9512519522b118090257be113b9468d804b19d63c71dbcf4a48fa32358",
+                "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53",
+                "sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78",
+                "sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803",
+                "sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a",
+                "sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f",
+                "sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174",
+                "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
             ],
-            "markers": "python_full_version >= '3.6.8'",
-            "version": "==3.0.9"
-        },
-        "pytz": {
-            "hashes": [
-                "sha256:1e760e2fe6a8163bc0b3d9a19c4f84342afa0a2affebfaa84b01b978a02ecaa7",
-                "sha256:e68985985296d9a66a881eb3193b0906246245294a881e7c8afe623866ac6a5c"
-            ],
-            "version": "==2022.1"
+            "markers": "python_version >= '3.6'",
+            "version": "==6.0"
         },
         "readme-renderer": {
             "hashes": [
-                "sha256:73b84905d091c31f36e50b4ae05ae2acead661f6a09a9abb4df7d2ddcdb6a698",
-                "sha256:a727999acfc222fc21d82a12ed48c957c4989785e5865807c65a487d21677497"
+                "sha256:cd653186dfc73055656f090f227f5cb22a046d7f71a841dfa305f55c9a513273",
+                "sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==35.0"
+            "version": "==37.3"
         },
         "requests": {
             "hashes": [
                 "sha256:68d7c56fd5a8999887728ef304a6d12edc7be74f1cfa47714fc8b414525c9a61",
                 "sha256:f22fa1e554c9ddfd16e6e41ac79759e17be9e492b3587efa038054674760e72d"
             ],
             "index": "pypi",
             "version": "==2.27.1"
         },
         "requests-toolbelt": {
             "hashes": [
-                "sha256:380606e1d10dc85c3bd47bf5a6095f815ec007be7a8b69c878507068df059e6f",
-                "sha256:968089d4584ad4ad7c171454f0a5c6dac23971e9472521ea3b6d49d610aa6fc0"
+                "sha256:18565aa58116d9951ac39baa288d3adb5b3ff975c4f25eee78555d89e8f247f7",
+                "sha256:62e09f7ff5ccbda92772a29f394a49c3ad6cb181d568b1337626b2abb628a63d"
             ],
-            "version": "==0.9.1"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==0.10.1"
         },
         "rfc3986": {
             "hashes": [
                 "sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd",
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
-                "sha256:4c586de507202505346f3e32d1363eb9ed6932f0c2f63184dea88983ff4971e2",
-                "sha256:d2bbd99c320a2532ac71ff6a3164867884357da3e3301f0240090c5d2fdac7ec"
+                "sha256:91954fe80cfb7985727a467ca98a7618e5dd15178cc2da10f553b36a93859001",
+                "sha256:a104f37270bf677148d8acb07d33be1569eeee87e2d1beb286a4e9113caf6f2f"
             ],
-            "markers": "python_full_version >= '3.6.3' and python_full_version < '4.0.0'",
-            "version": "==12.4.4"
+            "markers": "python_version >= '3.7'",
+            "version": "==13.3.2"
         },
         "secretstorage": {
             "hashes": [
-                "sha256:0a8eb9645b320881c222e827c26f4cfcf55363e8b374a021981ef886657a912f",
-                "sha256:755dc845b6ad76dcbcbc07ea3da75ae54bb1ea529eb72d15f83d26499a5df319"
+                "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
+                "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
             ],
             "markers": "sys_platform == 'linux'",
-            "version": "==3.3.2"
+            "version": "==3.3.3"
         },
         "setuptools": {
             "hashes": [
-                "sha256:68e45d17c9281ba25dc0104eadd2647172b3472d9e01f911efa57965e8d51a36",
-                "sha256:a43bdedf853c670e5fed28e5623403bad2f73cf02f9a2774e91def6bda8265a7"
+                "sha256:2ee892cd5f29f3373097f5a814697e397cf3ce313616df0af11231e2ad118077",
+                "sha256:b78aaa36f6b90a074c1fa651168723acbf45d14cb1196b6f02c0fd07f17623b2"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==62.3.2"
+            "version": "==67.6.0"
         },
         "setuptools-scm": {
             "hashes": [
                 "sha256:6833ac65c6ed9711a4d5d2266f8024cfa07c533a0e55f4c12f6eff280a5a9e30",
                 "sha256:acea13255093849de7ccb11af9e1fb8bde7067783450cee9ef7a93139bddf6d4"
             ],
             "index": "pypi",
@@ -457,35 +596,35 @@
                 "sha256:af248b21e3282f847ff20feebe7a1985fb34773cbe3fc75bf206897f1a2199c4"
             ],
             "index": "pypi",
             "version": "==5.0.0"
         },
         "sphinxcontrib-applehelp": {
             "hashes": [
-                "sha256:806111e5e962be97c29ec4c1e7fe277bfd19e9652fb1a4392105b43e01af885a",
-                "sha256:a072735ec80e7675e3f432fcae8610ecf509c5f1869d17e2eecff44389cdbc58"
+                "sha256:29d341f67fb0f6f586b23ad80e072c8e6ad0b48417db2bde114a4c9746feb228",
+                "sha256:828f867945bbe39817c210a1abfd1bc4895c8b73fcaade56d45357a348a07d7e"
             ],
-            "markers": "python_version >= '3.5'",
-            "version": "==1.0.2"
+            "markers": "python_version >= '3.8'",
+            "version": "==1.0.4"
         },
         "sphinxcontrib-devhelp": {
             "hashes": [
                 "sha256:8165223f9a335cc1af7ffe1ed31d2871f325254c0423bc0c4c7cd1c1e4734a2e",
                 "sha256:ff7f1afa7b9642e7060379360a67e9c41e8f3121f2ce9164266f61b9f4b338e4"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.2"
         },
         "sphinxcontrib-htmlhelp": {
             "hashes": [
-                "sha256:d412243dfb797ae3ec2b59eca0e52dac12e75a241bf0e4eb861e450d06c6ed07",
-                "sha256:f5f8bb2d0d629f398bf47d0d69c07bc13b65f75a81ad9e2f71a63d4b7a2f6db2"
+                "sha256:0cbdd302815330058422b98a113195c9249825d681e18f11e8b1f78a2f11efff",
+                "sha256:c38cb46dccf316c79de6e5515e1770414b797162b23cd3d06e67020e1d2a6903"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.0.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==2.0.1"
         },
         "sphinxcontrib-jsmath": {
             "hashes": [
                 "sha256:2ec2eaebfb78f3f2078e73666b1415417a116cc848b72e5172e596c871103178",
                 "sha256:a9925e4a4587247ed2191a22df5f6970656cb8ca2bd6284309578f2153e0c4b8"
             ],
             "markers": "python_version >= '3.5'",
@@ -503,14 +642,22 @@
             "hashes": [
                 "sha256:352a9a00ae864471d3a7ead8d7d79f5fc0b57e8b3f95e9867eb9eb28999b92fd",
                 "sha256:aa5f6de5dfdf809ef505c4895e51ef5c9eac17d0f287933eb49ec495280b6952"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.1.5"
         },
+        "toml": {
+            "hashes": [
+                "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
+                "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
+            ],
+            "markers": "python_version >= '2.6' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==0.10.2"
+        },
         "tomli": {
             "hashes": [
                 "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.1"
@@ -521,30 +668,38 @@
                 "sha256:817aa0c0bdc02a5ebe32051e168e23c71a0608334e624c793011f120dbbc05b7"
             ],
             "index": "pypi",
             "version": "==4.0.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:44ece4d53fb1706f667c9bd1c648f5469a2ec925fcf3a776667042d645472c14",
-                "sha256:aabaf16477806a5e1dd19aa41f8c2b7950dd3c746362d7e3223dbe6de6ac448e"
+                "sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72",
+                "sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4'",
-            "version": "==1.26.9"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
+            "version": "==1.26.14"
+        },
+        "virtualenv": {
+            "hashes": [
+                "sha256:3c22fa5a7c7aa106ced59934d2c20a2ecb7f49b4130b8bf444178a16b880fa45",
+                "sha256:a8a4b8ca1e28f864b7514a253f98c1d62b64e31e77325ba279248c65fb4fcef4"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==20.20.0"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
         },
         "zipp": {
             "hashes": [
-                "sha256:56bf8aadb83c24db6c4b577e13de374ccfb67da2078beba1d037c17980bf43ad",
-                "sha256:c4f6e5bbf48e74f7a38e7cc5b0480ff42b0ae5178957d564d18932525d5cf099"
+                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
+                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.8.0"
+            "version": "==3.15.0"
         }
     }
 }
```

### Comparing `calfire-wildfires-1.1.0/calfire_wildfires.egg-info/SOURCES.txt` & `calfire-wildfires-1.1.1/calfire_wildfires.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+.pre-commit-config.yaml
 LICENSE
 MANIFEST.in
 Pipfile
 Pipfile.lock
 README.md
 setup.cfg
 setup.py
```

### Comparing `calfire-wildfires-1.1.0/docs/Makefile` & `calfire-wildfires-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `calfire-wildfires-1.1.0/docs/_static/css/custom.css` & `calfire-wildfires-1.1.1/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `calfire-wildfires-1.1.0/docs/_templates/nav.html` & `calfire-wildfires-1.1.1/docs/_templates/nav.html`

 * *Files identical despite different names*

### Comparing `calfire-wildfires-1.1.0/docs/conf.py` & `calfire-wildfires-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `calfire-wildfires-1.1.0/docs/index.md` & `calfire-wildfires-1.1.1/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,81 +30,81 @@
 000001d0: 7265 7320 2020 2054 6865 206c 6174 6573  res    The lates
 000001e0: 7420 6163 7469 7665 2066 6972 6573 0a20  t active fires. 
 000001f0: 2020 2061 6c6c 2d66 6972 6573 2020 2020     all-fires    
 00000200: 2020 2046 6972 6573 2079 6561 722d 746f     Fires year-to
 00000210: 2d64 6174 652c 2062 6f74 6820 6163 7469  -date, both acti
 00000220: 7665 2061 6e64 2063 6f6e 7461 696e 6564  ve and contained
 00000230: 0a60 6060 0a0a 4672 6f6d 2074 6865 2073  .```..From the s
-00000240: 6865 6c6c 3a20 0a0a 6060 6073 680a 6361  hell: ..```sh.ca
-00000250: 6c66 6972 6577 696c 6466 6972 6573 2061  lfirewildfires a
-00000260: 6c6c 2d66 6972 6573 0a63 616c 6669 7265  ll-fires.calfire
-00000270: 7769 6c64 6669 7265 7320 6163 7469 7665  wildfires active
-00000280: 2d66 6972 6573 0a60 6060 0a0a 2323 2050  -fires.```..## P
-00000290: 7974 686f 6e20 7573 6167 650a 0a49 6d70  ython usage..Imp
-000002a0: 6f72 7420 7468 6520 6c69 6272 6172 792e  ort the library.
-000002b0: 200a 0a60 6060 7079 7468 6f6e 0a69 6d70   ..```python.imp
-000002c0: 6f72 7420 6361 6c66 6972 655f 7769 6c64  ort calfire_wild
-000002d0: 6669 7265 730a 6461 7461 203d 2063 616c  fires.data = cal
-000002e0: 6669 7265 5f77 696c 6466 6972 6573 2e67  fire_wildfires.g
-000002f0: 6574 5f61 6c6c 5f66 6972 6573 2829 0a64  et_all_fires().d
-00000300: 6174 6120 3d20 6361 6c66 6972 655f 7769  ata = calfire_wi
-00000310: 6c64 6669 7265 732e 6765 745f 6163 7469  ldfires.get_acti
-00000320: 7665 5f66 6972 6573 2829 0a60 6060 0a0a  ve_fires().```..
-00000330: 2323 2043 6f6e 7472 6962 7574 696e 670a  ## Contributing.
-00000340: 0a49 6e73 7461 6c6c 2064 6570 656e 6465  .Install depende
-00000350: 6e63 6965 7320 666f 7220 6465 7665 6c6f  ncies for develo
-00000360: 706d 656e 742e 0a0a 6060 6073 680a 7069  pment...```sh.pi
-00000370: 7065 6e76 2069 6e73 7461 6c6c 202d 2d64  penv install --d
-00000380: 6576 0a60 6060 0a0a 5275 6e20 7465 7374  ev.```..Run test
-00000390: 732e 0a0a 6060 6073 680a 7069 7065 6e76  s...```sh.pipenv
-000003a0: 2072 756e 2070 7974 686f 6e20 7465 7374   run python test
-000003b0: 2e70 790a 6060 600a 0a23 2320 4465 7665  .py.```..## Deve
-000003c0: 6c6f 7069 6e67 2074 6865 2043 4c49 0a0a  loping the CLI..
-000003d0: 5468 6520 636f 6d6d 616e 642d 6c69 6e65  The command-line
-000003e0: 2069 6e74 6572 6661 6365 2069 7320 696d   interface is im
-000003f0: 706c 656d 656e 7465 6420 7573 696e 6720  plemented using 
-00000400: 436c 6963 6b20 616e 6420 7365 7475 7074  Click and setupt
-00000410: 6f6f 6c73 2e20 546f 2069 6e73 7461 6c6c  ools. To install
-00000420: 2069 7420 6c6f 6361 6c6c 7920 666f 7220   it locally for 
-00000430: 6465 7665 6c6f 706d 656e 7420 696e 7369  development insi
-00000440: 6465 2079 6f75 7220 7669 7274 7561 6c20  de your virtual 
-00000450: 656e 7669 726f 6e6d 656e 742c 2072 756e  environment, run
-00000460: 2074 6865 2066 6f6c 6c6f 7769 6e67 2069   the following i
-00000470: 6e73 7461 6c6c 6174 696f 6e20 636f 6d6d  nstallation comm
-00000480: 616e 642c 2061 7320 5b70 7265 7363 7269  and, as [prescri
-00000490: 6265 6420 6279 2074 6865 2043 6c69 636b  bed by the Click
-000004a0: 2064 6f63 756d 656e 7461 7469 6f6e 5d28   documentation](
-000004b0: 6874 7470 733a 2f2f 636c 6963 6b2e 7061  https://click.pa
-000004c0: 6c6c 6574 7370 726f 6a65 6374 732e 636f  lletsprojects.co
-000004d0: 6d2f 656e 2f37 2e78 2f73 6574 7570 746f  m/en/7.x/setupto
-000004e0: 6f6c 732f 2373 6574 7570 746f 6f6c 732d  ols/#setuptools-
-000004f0: 696e 7465 6772 6174 696f 6e29 2e0a 0a60  integration)...`
-00000500: 6060 7368 0a70 6970 656e 7620 7275 6e20  ``sh.pipenv run 
-00000510: 7069 7020 696e 7374 616c 6c20 2d2d 6564  pip install --ed
-00000520: 6974 6162 6c65 202e 0a60 6060 0a0a 2323  itable ..```..##
-00000530: 204c 696e 6b73 0a0a 2a20 446f 6373 3a20   Links..* Docs: 
-00000540: 5b70 616c 6577 692e 7265 2f64 6f63 732f  [palewi.re/docs/
-00000550: 6361 6c66 6972 652d 7769 6c64 6669 7265  calfire-wildfire
-00000560: 732f 5d28 6874 7470 733a 2f2f 7061 6c65  s/](https://pale
-00000570: 7769 2e72 652f 646f 6373 2f63 616c 6669  wi.re/docs/calfi
-00000580: 7265 2d77 696c 6466 6972 6573 2f29 0a2a  re-wildfires/).*
-00000590: 2049 7373 7565 733a 205b 6769 7468 7562   Issues: [github
-000005a0: 2e63 6f6d 2f64 6174 6164 6573 6b2f 6361  .com/datadesk/ca
-000005b0: 6c66 6972 652d 7769 6c64 6669 7265 732f  lfire-wildfires/
-000005c0: 6973 7375 6573 5d28 6874 7470 733a 2f2f  issues](https://
-000005d0: 6769 7468 7562 2e63 6f6d 2f64 6174 6164  github.com/datad
-000005e0: 6573 6b2f 6361 6c66 6972 652d 7769 6c64  esk/calfire-wild
-000005f0: 6669 7265 732f 6973 7375 6573 290a 2a20  fires/issues).* 
-00000600: 5061 636b 6167 696e 673a 205b 7079 7069  Packaging: [pypi
-00000610: 2e70 7974 686f 6e2e 6f72 672f 7079 7069  .python.org/pypi
-00000620: 2f63 616c 6669 7265 2d77 696c 6466 6972  /calfire-wildfir
-00000630: 6573 5d28 6874 7470 733a 2f2f 7079 7069  es](https://pypi
-00000640: 2e70 7974 686f 6e2e 6f72 672f 7079 7069  .python.org/pypi
-00000650: 2f63 616c 6669 7265 2d77 696c 6466 6972  /calfire-wildfir
-00000660: 6573 290a 2a20 5465 7374 696e 673a 205b  es).* Testing: [
-00000670: 6769 7468 7562 2e63 6f6d 2f64 6174 6164  github.com/datad
-00000680: 6573 6b2f 6361 6c66 6972 652d 7769 6c64  esk/calfire-wild
-00000690: 6669 7265 732f 6163 7469 6f6e 735d 2868  fires/actions](h
-000006a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000006b0: 6d2f 6461 7461 6465 736b 2f63 616c 6669  m/datadesk/calfi
-000006c0: 7265 2d77 696c 6466 6972 6573 2f61 6374  re-wildfires/act
-000006d0: 696f 6e73 290a                           ions).
+00000240: 6865 6c6c 3a0a 0a60 6060 7368 0a63 616c  hell:..```sh.cal
+00000250: 6669 7265 7769 6c64 6669 7265 7320 616c  firewildfires al
+00000260: 6c2d 6669 7265 730a 6361 6c66 6972 6577  l-fires.calfirew
+00000270: 696c 6466 6972 6573 2061 6374 6976 652d  ildfires active-
+00000280: 6669 7265 730a 6060 600a 0a23 2320 5079  fires.```..## Py
+00000290: 7468 6f6e 2075 7361 6765 0a0a 496d 706f  thon usage..Impo
+000002a0: 7274 2074 6865 206c 6962 7261 7279 2e0a  rt the library..
+000002b0: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
+000002c0: 7420 6361 6c66 6972 655f 7769 6c64 6669  t calfire_wildfi
+000002d0: 7265 730a 0a64 6174 6120 3d20 6361 6c66  res..data = calf
+000002e0: 6972 655f 7769 6c64 6669 7265 732e 6765  ire_wildfires.ge
+000002f0: 745f 616c 6c5f 6669 7265 7328 290a 6461  t_all_fires().da
+00000300: 7461 203d 2063 616c 6669 7265 5f77 696c  ta = calfire_wil
+00000310: 6466 6972 6573 2e67 6574 5f61 6374 6976  dfires.get_activ
+00000320: 655f 6669 7265 7328 290a 6060 600a 0a23  e_fires().```..#
+00000330: 2320 436f 6e74 7269 6275 7469 6e67 0a0a  # Contributing..
+00000340: 496e 7374 616c 6c20 6465 7065 6e64 656e  Install dependen
+00000350: 6369 6573 2066 6f72 2064 6576 656c 6f70  cies for develop
+00000360: 6d65 6e74 2e0a 0a60 6060 7368 0a70 6970  ment...```sh.pip
+00000370: 656e 7620 696e 7374 616c 6c20 2d2d 6465  env install --de
+00000380: 760a 6060 600a 0a52 756e 2074 6573 7473  v.```..Run tests
+00000390: 2e0a 0a60 6060 7368 0a70 6970 656e 7620  ...```sh.pipenv 
+000003a0: 7275 6e20 7079 7468 6f6e 2074 6573 742e  run python test.
+000003b0: 7079 0a60 6060 0a0a 2323 2044 6576 656c  py.```..## Devel
+000003c0: 6f70 696e 6720 7468 6520 434c 490a 0a54  oping the CLI..T
+000003d0: 6865 2063 6f6d 6d61 6e64 2d6c 696e 6520  he command-line 
+000003e0: 696e 7465 7266 6163 6520 6973 2069 6d70  interface is imp
+000003f0: 6c65 6d65 6e74 6564 2075 7369 6e67 2043  lemented using C
+00000400: 6c69 636b 2061 6e64 2073 6574 7570 746f  lick and setupto
+00000410: 6f6c 732e 2054 6f20 696e 7374 616c 6c20  ols. To install 
+00000420: 6974 206c 6f63 616c 6c79 2066 6f72 2064  it locally for d
+00000430: 6576 656c 6f70 6d65 6e74 2069 6e73 6964  evelopment insid
+00000440: 6520 796f 7572 2076 6972 7475 616c 2065  e your virtual e
+00000450: 6e76 6972 6f6e 6d65 6e74 2c20 7275 6e20  nvironment, run 
+00000460: 7468 6520 666f 6c6c 6f77 696e 6720 696e  the following in
+00000470: 7374 616c 6c61 7469 6f6e 2063 6f6d 6d61  stallation comma
+00000480: 6e64 2c20 6173 205b 7072 6573 6372 6962  nd, as [prescrib
+00000490: 6564 2062 7920 7468 6520 436c 6963 6b20  ed by the Click 
+000004a0: 646f 6375 6d65 6e74 6174 696f 6e5d 2868  documentation](h
+000004b0: 7474 7073 3a2f 2f63 6c69 636b 2e70 616c  ttps://click.pal
+000004c0: 6c65 7473 7072 6f6a 6563 7473 2e63 6f6d  letsprojects.com
+000004d0: 2f65 6e2f 372e 782f 7365 7475 7074 6f6f  /en/7.x/setuptoo
+000004e0: 6c73 2f23 7365 7475 7074 6f6f 6c73 2d69  ls/#setuptools-i
+000004f0: 6e74 6567 7261 7469 6f6e 292e 0a0a 6060  ntegration)...``
+00000500: 6073 680a 7069 7065 6e76 2072 756e 2070  `sh.pipenv run p
+00000510: 6970 2069 6e73 7461 6c6c 202d 2d65 6469  ip install --edi
+00000520: 7461 626c 6520 2e0a 6060 600a 0a23 2320  table ..```..## 
+00000530: 4c69 6e6b 730a 0a2a 2044 6f63 733a 205b  Links..* Docs: [
+00000540: 7061 6c65 7769 2e72 652f 646f 6373 2f63  palewi.re/docs/c
+00000550: 616c 6669 7265 2d77 696c 6466 6972 6573  alfire-wildfires
+00000560: 2f5d 2868 7474 7073 3a2f 2f70 616c 6577  /](https://palew
+00000570: 692e 7265 2f64 6f63 732f 6361 6c66 6972  i.re/docs/calfir
+00000580: 652d 7769 6c64 6669 7265 732f 290a 2a20  e-wildfires/).* 
+00000590: 4973 7375 6573 3a20 5b67 6974 6875 622e  Issues: [github.
+000005a0: 636f 6d2f 6461 7461 6465 736b 2f63 616c  com/datadesk/cal
+000005b0: 6669 7265 2d77 696c 6466 6972 6573 2f69  fire-wildfires/i
+000005c0: 7373 7565 735d 2868 7474 7073 3a2f 2f67  ssues](https://g
+000005d0: 6974 6875 622e 636f 6d2f 6461 7461 6465  ithub.com/datade
+000005e0: 736b 2f63 616c 6669 7265 2d77 696c 6466  sk/calfire-wildf
+000005f0: 6972 6573 2f69 7373 7565 7329 0a2a 2050  ires/issues).* P
+00000600: 6163 6b61 6769 6e67 3a20 5b70 7970 692e  ackaging: [pypi.
+00000610: 7079 7468 6f6e 2e6f 7267 2f70 7970 692f  python.org/pypi/
+00000620: 6361 6c66 6972 652d 7769 6c64 6669 7265  calfire-wildfire
+00000630: 735d 2868 7474 7073 3a2f 2f70 7970 692e  s](https://pypi.
+00000640: 7079 7468 6f6e 2e6f 7267 2f70 7970 692f  python.org/pypi/
+00000650: 6361 6c66 6972 652d 7769 6c64 6669 7265  calfire-wildfire
+00000660: 7329 0a2a 2054 6573 7469 6e67 3a20 5b67  s).* Testing: [g
+00000670: 6974 6875 622e 636f 6d2f 6461 7461 6465  ithub.com/datade
+00000680: 736b 2f63 616c 6669 7265 2d77 696c 6466  sk/calfire-wildf
+00000690: 6972 6573 2f61 6374 696f 6e73 5d28 6874  ires/actions](ht
+000006a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000006b0: 2f64 6174 6164 6573 6b2f 6361 6c66 6972  /datadesk/calfir
+000006c0: 652d 7769 6c64 6669 7265 732f 6163 7469  e-wildfires/acti
+000006d0: 6f6e 7329 0a                             ons).
```

### Comparing `calfire-wildfires-1.1.0/docs/make.bat` & `calfire-wildfires-1.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `calfire-wildfires-1.1.0/setup.py` & `calfire-wildfires-1.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+
 from setuptools import setup
 
 
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname)) as f:
         return f.read()
 
@@ -35,40 +36,37 @@
 
     If that issue is resolved, this method can be removed.
     """
     return ""
 
 
 setup(
-    name='calfire-wildfires',
+    name="calfire-wildfires",
     description="Download wildfires data from CalFire",
-    long_description=read('README.md'),
-    long_description_content_type='text/markdown',
-    author='Ben Welsh',
-    author_email='b@palewi.re',
-    url='https://palewi.re/docs/calfire-wildfires/',
+    long_description=read("README.md"),
+    long_description_content_type="text/markdown",
+    author="Ben Welsh",
+    author_email="b@palewi.re",
+    url="https://palewi.re/docs/calfire-wildfires/",
     license="MIT",
     packages=("calfire_wildfires",),
-    install_requires=[
-        "click",
-        "requests"
-    ],
+    install_requires=["click", "requests"],
     entry_points="""
         [console_scripts]
         calfirewildfires=calfire_wildfires.cli:cmd
     """,
     use_scm_version={"version_scheme": version_scheme, "local_scheme": local_version},
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'License :: OSI Approved :: MIT License',
+        "Development Status :: 5 - Production/Stable",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "License :: OSI Approved :: MIT License",
     ],
     project_urls={
-        'Maintainer': 'https://github.com/datadesk',
-        'Source': 'https://github.com/datadesk/calfire-wildfires',
-        'Tracker': 'https://github.com/datadesk/calfire-wildfires/issues'
+        "Maintainer": "https://github.com/datadesk",
+        "Source": "https://github.com/datadesk/calfire-wildfires",
+        "Tracker": "https://github.com/datadesk/calfire-wildfires/issues",
     },
 )
```

