# Comparing `tmp/perspective_parquet-0.1.0.tar.gz` & `tmp/perspective_parquet-0.1.1.tar.gz`

## Comparing `perspective_parquet-0.1.0.tar` & `perspective_parquet-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,32 @@
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/.bumpversion.cfg
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/.gitattributes
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/MANIFEST.in
--rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/Makefile
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/setup.py
--rw-r--r--   0        0        0   125754 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/test.parquet
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/binder/postBuild
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/binder/requirements.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/binder/runtime.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/js/.prettierrc.json
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/js/build.js
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/js/package.json
--rw-r--r--   0        0        0   214280 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/js/yarn.lock
--rw-r--r--   0        0        0     7489 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/js/src/js/index.js
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/js/src/js/psp_widget.js
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/js/src/js/utils.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/js/src/less/index.less
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/perspective_parquet/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/perspective_parquet/_version.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/perspective_parquet/extension/install.json
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/perspective_parquet/labextension/package.json
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/perspective_parquet/labextension/static/169.804c1a7cf0ea9dfd1210.js
--rw-r--r--   0        0        0  8132374 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/perspective_parquet/labextension/static/28.1968cb0312a1815497cb.js
--rw-r--r--   0        0        0     7114 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/perspective_parquet/labextension/static/remoteEntry.95fcd5d4b753367e9b01.js
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/perspective_parquet/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/perspective_parquet/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/perspective_parquet/tests/test_all.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/LICENSE
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/README.md
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    15208 2020-02-02 00:00:00.000000 perspective_parquet-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/.bumpversion.cfg
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/.gitattributes
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/MANIFEST.in
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/Makefile
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/setup.py
+-rw-r--r--   0        0        0   125754 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/test.parquet
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/binder/postBuild
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/binder/requirements.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/binder/runtime.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/js/.prettierrc.json
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/js/build.js
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/js/package.json
+-rw-r--r--   0        0        0   214280 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/js/yarn.lock
+-rw-r--r--   0        0        0     7489 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/js/src/js/index.js
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/js/src/js/psp_widget.js
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/js/src/js/utils.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/js/src/less/index.less
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/perspective_parquet/__init__.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/perspective_parquet/extension/install.json
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/perspective_parquet/labextension/package.json
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/perspective_parquet/labextension/static/169.804c1a7cf0ea9dfd1210.js
+-rw-r--r--   0        0        0  8132374 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/perspective_parquet/labextension/static/28.1968cb0312a1815497cb.js
+-rw-r--r--   0        0        0     7114 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/perspective_parquet/labextension/static/remoteEntry.e7c57d2259396dc4d686.js
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/perspective_parquet/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/perspective_parquet/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/perspective_parquet/tests/test_all.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/LICENSE
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/README.md
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    15160 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/PKG-INFO
```

### Comparing `perspective_parquet-0.1.0/.bumpversion.cfg` & `perspective_parquet-0.1.1/.bumpversion.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [bumpversion]
-current_version = 0.1.0
+current_version = 0.1.1
 commit = True
 tag = False
 
-[bumpversion:file:perspective_parquet/_version.py]
+[bumpversion:file:perspective_parquet/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
 
 [bumpversion:file:pyproject.toml]
 search = version = "{current_version}"
 replace = version = "{new_version}"
```

### Comparing `perspective_parquet-0.1.0/CONTRIBUTING.md` & `perspective_parquet-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `perspective_parquet-0.1.0/MANIFEST.in` & `perspective_parquet-0.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `perspective_parquet-0.1.0/Makefile` & `perspective_parquet-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `perspective_parquet-0.1.0/test.parquet` & `perspective_parquet-0.1.1/test.parquet`

 * *Files identical despite different names*

### Comparing `perspective_parquet-0.1.0/js/build.js` & `perspective_parquet-0.1.1/js/build.js`

 * *Files identical despite different names*

### Comparing `perspective_parquet-0.1.0/js/package.json` & `perspective_parquet-0.1.1/js/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.1.1'"}*

```diff
@@ -59,9 +59,9 @@
         "clean:labextension": "rimraf ../perspective_parquet/labextension",
         "clean:lib": "rimraf lib",
         "fix": "prettier --write  \"src/js/*.js\" \"src/less/*.less\" \"*.js\" \"*.json\"",
         "lint": "prettier --check \"src/js/*.js\" \"src/less/*.less\" \"*.js\" \"*.json\"",
         "test": ":"
     },
     "style": "dist/umd/perspective-parquet.css",
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `perspective_parquet-0.1.0/js/yarn.lock` & `perspective_parquet-0.1.1/js/yarn.lock`

 * *Files identical despite different names*

### Comparing `perspective_parquet-0.1.0/js/src/js/index.js` & `perspective_parquet-0.1.1/js/src/js/index.js`

 * *Files identical despite different names*

### Comparing `perspective_parquet-0.1.0/js/src/js/psp_widget.js` & `perspective_parquet-0.1.1/js/src/js/psp_widget.js`

 * *Files identical despite different names*

### Comparing `perspective_parquet-0.1.0/perspective_parquet/labextension/package.json` & `perspective_parquet-0.1.1/perspective_parquet/labextension/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9608974358974359%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.e7c57d2259396dc4d686.js'}}",*

 * * "'version'": "'0.1.1'"}*

```diff
@@ -23,15 +23,15 @@
     "files": [
         "dist/**/*",
         "src/**/*"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.95fcd5d4b753367e9b01.js",
+            "load": "static/remoteEntry.e7c57d2259396dc4d686.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "perspective-python"
                 },
@@ -64,9 +64,9 @@
         "clean:labextension": "rimraf ../perspective_parquet/labextension",
         "clean:lib": "rimraf lib",
         "fix": "prettier --write  \"src/js/*.js\" \"src/less/*.less\" \"*.js\" \"*.json\"",
         "lint": "prettier --check \"src/js/*.js\" \"src/less/*.less\" \"*.js\" \"*.json\"",
         "test": ":"
     },
     "style": "dist/umd/perspective-parquet.css",
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `perspective_parquet-0.1.0/perspective_parquet/labextension/static/169.804c1a7cf0ea9dfd1210.js` & `perspective_parquet-0.1.1/perspective_parquet/labextension/static/169.804c1a7cf0ea9dfd1210.js`

 * *Files identical despite different names*

### Comparing `perspective_parquet-0.1.0/perspective_parquet/labextension/static/28.1968cb0312a1815497cb.js` & `perspective_parquet-0.1.1/perspective_parquet/labextension/static/28.1968cb0312a1815497cb.js`

 * *Files identical despite different names*

### Comparing `perspective_parquet-0.1.0/perspective_parquet/labextension/static/remoteEntry.95fcd5d4b753367e9b01.js` & `perspective_parquet-0.1.1/perspective_parquet/labextension/static/remoteEntry.e7c57d2259396dc4d686.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -106,15 +106,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => k.e(28).then((() => () => k(28))),
                         from: i,
                         eager: !1
                     })
-                })("perspective-parquet", "0.1.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("perspective-parquet", "0.1.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         k.g.importScripts && (e = k.g.location + "");
         var r = k.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `perspective_parquet-0.1.0/perspective_parquet/labextension/static/third-party-licenses.json` & `perspective_parquet-0.1.1/perspective_parquet/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `perspective_parquet-0.1.0/.gitignore` & `perspective_parquet-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `perspective_parquet-0.1.0/LICENSE` & `perspective_parquet-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `perspective_parquet-0.1.0/README.md` & `perspective_parquet-0.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # perspective-parquet
 Parquet file editor in Jupyterlab, built with [Perspective](https://github.com/finos/perspective)
 
-[![Build Status](https://github.com/perspective-community/perspective-parquet/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/perspective-community/perspective-parquet/actions?query=workflow%3A%22Build+Status%22)
+[![Build Status](https://github.com/timkpaine/perspective-parquet/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/timkpaine/perspective-parquet/actions?query=workflow%3A%22Build+Status%22)
 [![PyPI](https://img.shields.io/pypi/l/perspective-parquet.svg)](https://pypi.python.org/pypi/perspective-parquet)
 [![PyPI](https://img.shields.io/pypi/v/perspective-parquet.svg)](https://pypi.python.org/pypi/perspective-parquet)
 [![npm](https://img.shields.io/npm/v/perspective-parquet.svg)](https://www.npmjs.com/package/perspective-parquet)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/perspective-community/perspective-parquet/main?urlpath=lab)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/timkpaine/perspective-parquet/main?urlpath=lab)
 
-![](https://raw.githubusercontent.com/perspective-community/perspective-parquet/main/docs/img/demo.gif)
+![](https://raw.githubusercontent.com/timkpaine/perspective-parquet/main/docs/img/demo.gif)
```

### Comparing `perspective_parquet-0.1.0/pyproject.toml` & `perspective_parquet-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "jupyterlab>=3.5,<4",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "perspective-parquet"
 description = "Parquet viewer for perspective in JupyterLab"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 authors = [
     { name = "Tim Paine", email = "t.paine154@gmail.com" },
 ]
 keywords = [
```

### Comparing `perspective_parquet-0.1.0/PKG-INFO` & `perspective_parquet-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perspective-parquet
-Version: 0.1.0
+Version: 0.1.1
 Summary: Parquet viewer for perspective in JupyterLab
 Project-URL: repository, https://github.com/timkpaine/perspective-parquet
 Project-URL: homepage, https://github.com/timkpaine/perspective-parquet
 Author-email: Tim Paine <t.paine154@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -230,14 +230,14 @@
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
 
 # perspective-parquet
 Parquet file editor in Jupyterlab, built with [Perspective](https://github.com/finos/perspective)
 
-[![Build Status](https://github.com/perspective-community/perspective-parquet/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/perspective-community/perspective-parquet/actions?query=workflow%3A%22Build+Status%22)
+[![Build Status](https://github.com/timkpaine/perspective-parquet/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/timkpaine/perspective-parquet/actions?query=workflow%3A%22Build+Status%22)
 [![PyPI](https://img.shields.io/pypi/l/perspective-parquet.svg)](https://pypi.python.org/pypi/perspective-parquet)
 [![PyPI](https://img.shields.io/pypi/v/perspective-parquet.svg)](https://pypi.python.org/pypi/perspective-parquet)
 [![npm](https://img.shields.io/npm/v/perspective-parquet.svg)](https://www.npmjs.com/package/perspective-parquet)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/perspective-community/perspective-parquet/main?urlpath=lab)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/timkpaine/perspective-parquet/main?urlpath=lab)
 
-![](https://raw.githubusercontent.com/perspective-community/perspective-parquet/main/docs/img/demo.gif)
+![](https://raw.githubusercontent.com/timkpaine/perspective-parquet/main/docs/img/demo.gif)
```

