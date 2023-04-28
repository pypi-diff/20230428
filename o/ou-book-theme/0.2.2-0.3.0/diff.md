# Comparing `tmp/ou_book_theme-0.2.2.tar.gz` & `tmp/ou_book_theme-0.3.0.tar.gz`

## Comparing `ou_book_theme-0.2.2.tar` & `ou_book_theme-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/CHANGELOG.md
--rw-r--r--   0        0        0    10849 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/package-lock.json
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/package.json
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/rollup.config.js
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/ou_book_theme/__about__.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/ou_book_theme/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/ou_book_theme/assets/scripts/activity.js
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/ou_book_theme/assets/scripts/index.js
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/ou_book_theme/assets/styles/_activity.scss
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/ou_book_theme/assets/styles/_time.scss
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/ou_book_theme/assets/styles/_variables.scss
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/ou_book_theme/assets/styles/_where-next.scss
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/ou_book_theme/assets/styles/index.scss
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/ou_book_theme/extensions/__init__.py
--rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/ou_book_theme/extensions/activity.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/ou_book_theme/extensions/time.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/ou_book_theme/extensions/util.py
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/ou_book_theme/extensions/where_next.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/ou_book_theme/theme/ou_book_theme/theme.conf
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/ou_book_theme/theme/ou_book_theme/static/images/favicon.svg
--rw-r--r--   0        0        0    13489 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/ou_book_theme/theme/ou_book_theme/static/images/logo.svg
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/ou_book_theme/theme/ou_book_theme/static/scripts/ou-book-theme.js
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/ou_book_theme/theme/ou_book_theme/static/styles/ou-book-theme.css
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/.gitignore
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/README.md
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 ou_book_theme-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0    10849 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/package-lock.json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/package.json
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/rollup.config.js
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/__about__.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/assets/scripts/activity.js
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/assets/scripts/index.js
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/assets/styles/_activity.scss
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/assets/styles/_time.scss
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/assets/styles/_variables.scss
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/assets/styles/_where-next.scss
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/assets/styles/index.scss
+-rw-r--r--   0        0        0    21474 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/cli/__init__.py
+-rw-r--r--   0        0        0    40533 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/cli/mermaid-cli/package-lock.json
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/cli/mermaid-cli/package.json
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/extensions/__init__.py
+-rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/extensions/activity.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/extensions/time.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/extensions/util.py
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/extensions/where_next.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/theme/ou_book_theme/theme.conf
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/theme/ou_book_theme/static/images/favicon.svg
+-rw-r--r--   0        0        0    13489 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/theme/ou_book_theme/static/images/logo.svg
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/theme/ou_book_theme/static/scripts/ou-book-theme.js
+-rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/theme/ou_book_theme/static/styles/ou-book-theme.css
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/.gitignore
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/README.md
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/PKG-INFO
```

### Comparing `ou_book_theme-0.2.2/package-lock.json` & `ou_book_theme-0.3.0/package-lock.json`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.2.2/rollup.config.js` & `ou_book_theme-0.3.0/rollup.config.js`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.2.2/ou_book_theme/__init__.py` & `ou_book_theme-0.3.0/ou_book_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.2.2/ou_book_theme/assets/styles/_activity.scss` & `ou_book_theme-0.3.0/ou_book_theme/assets/styles/_activity.scss`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.2.2/ou_book_theme/assets/styles/_where-next.scss` & `ou_book_theme-0.3.0/ou_book_theme/assets/styles/_where-next.scss`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.2.2/ou_book_theme/extensions/activity.py` & `ou_book_theme-0.3.0/ou_book_theme/extensions/activity.py`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.2.2/ou_book_theme/extensions/time.py` & `ou_book_theme-0.3.0/ou_book_theme/extensions/time.py`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.2.2/ou_book_theme/extensions/where_next.py` & `ou_book_theme-0.3.0/ou_book_theme/extensions/where_next.py`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.2.2/ou_book_theme/theme/ou_book_theme/static/images/favicon.svg` & `ou_book_theme-0.3.0/ou_book_theme/theme/ou_book_theme/static/images/favicon.svg`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.2.2/ou_book_theme/theme/ou_book_theme/static/images/logo.svg` & `ou_book_theme-0.3.0/ou_book_theme/theme/ou_book_theme/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.2.2/ou_book_theme/theme/ou_book_theme/static/styles/ou-book-theme.css` & `ou_book_theme-0.3.0/ou_book_theme/theme/ou_book_theme/static/styles/ou-book-theme.css`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.2.2/pyproject.toml` & `ou_book_theme-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -19,19 +19,28 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
+  "lxml",
+  "pyyaml",
+  "rich",
   "sphinx_book_theme>=1.0.1,<2.0.0",
+  "sphinx_design",
   "sphinxcontrib-mermaid>=0.8.1,<1.0.0",
+  "typer[all]",
 ]
 dynamic = ["version"]
 
+[project.scripts]
+obt = "ou_book_theme.cli:main"
+"open-book-theme" = "ou_book_theme.cli:main"
+
 [project.urls]
 Documentation = "https://github.com/unknown/ou-book-theme#readme"
 Issues = "https://github.com/unknown/ou-book-theme/issues"
 Source = "https://github.com/unknown/ou-book-theme"
 
 [tool.hatch.version]
 path = "ou_book_theme/__about__.py"
```

### Comparing `ou_book_theme-0.2.2/PKG-INFO` & `ou_book_theme-0.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
 Name: ou-book-theme
-Version: 0.2.2
+Version: 0.3.0
 Project-URL: Documentation, https://github.com/unknown/ou-book-theme#readme
 Project-URL: Issues, https://github.com/unknown/ou-book-theme/issues
 Project-URL: Source, https://github.com/unknown/ou-book-theme
 Author-email: Mark Hall <mark.hall@open.ac.uk>
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
+Requires-Dist: lxml
+Requires-Dist: pyyaml
+Requires-Dist: rich
 Requires-Dist: sphinx-book-theme<2.0.0,>=1.0.1
+Requires-Dist: sphinx-design
 Requires-Dist: sphinxcontrib-mermaid<1.0.0,>=0.8.1
+Requires-Dist: typer[all]
 Description-Content-Type: text/markdown
 
 # ou-book-theme
 
 [![PyPI - Version](https://img.shields.io/pypi/v/ou-book-theme.svg)](https://pypi.org/project/ou-book-theme)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ou-book-theme.svg)](https://pypi.org/project/ou-book-theme)
```

