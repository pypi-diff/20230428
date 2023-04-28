# Comparing `tmp/fpdf2-2.7.3.tar.gz` & `tmp/fpdf2-2.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpdf2-2.7.3.tar", last modified: Mon Apr  3 12:13:37 2023, max compression
+gzip compressed data, was "fpdf2-2.7.4.tar", last modified: Fri Apr 28 10:37:06 2023, max compression
```

## Comparing `fpdf2-2.7.3.tar` & `fpdf2-2.7.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:13:37.627780 fpdf2-2.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-04-03 11:56:24.000000 fpdf2-2.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-03 11:56:24.000000 fpdf2-2.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    46179 2023-04-03 12:13:37.627780 fpdf2-2.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    44812 2023-04-03 11:56:24.000000 fpdf2-2.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:13:37.627780 fpdf2-2.7.3/fpdf/
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)   148148 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/drawing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    25512 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    42310 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/fonts.py
--rw-r--r--   0 runner    (1001) docker     (123)   189935 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/fpdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/graphics_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    24955 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/html.py
--rw-r--r--   0 runner    (1001) docker     (123)    16321 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/image_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    16182 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/line_break.py
--rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/linearization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/outline.py
--rw-r--r--   0 runner    (1001) docker     (123)    39076 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/prefs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/structure_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    30943 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/svg.py
--rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/syntax.py
--rw-r--r--   0 runner    (1001) docker     (123)    14414 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    22663 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/transitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-04-03 11:56:24.000000 fpdf2-2.7.3/fpdf/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:13:37.627780 fpdf2-2.7.3/fpdf2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46179 2023-04-03 12:13:37.000000 fpdf2-2.7.3/fpdf2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-03 12:13:37.000000 fpdf2-2.7.3/fpdf2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 12:13:37.000000 fpdf2-2.7.3/fpdf2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-03 12:13:37.000000 fpdf2-2.7.3/fpdf2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-03 12:13:37.000000 fpdf2-2.7.3/fpdf2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-03 12:13:37.631780 fpdf2-2.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-03 11:56:24.000000 fpdf2-2.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:37:06.284544 fpdf2-2.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-04-28 10:13:25.000000 fpdf2-2.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-28 10:13:25.000000 fpdf2-2.7.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    47046 2023-04-28 10:37:06.284544 fpdf2-2.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    45679 2023-04-28 10:13:25.000000 fpdf2-2.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:37:06.280544 fpdf2-2.7.4/fpdf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)   148148 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26118 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42341 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/fonts.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192125 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/fpdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/graphics_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25599 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16972 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/image_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16182 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/line_break.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/linearization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/outline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38984 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/prefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/structure_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30943 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/svg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/syntax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15119 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/transitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:37:06.284544 fpdf2-2.7.4/fpdf2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    47046 2023-04-28 10:37:06.000000 fpdf2-2.7.4/fpdf2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-28 10:37:06.000000 fpdf2-2.7.4/fpdf2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 10:37:06.000000 fpdf2-2.7.4/fpdf2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-28 10:37:06.000000 fpdf2-2.7.4/fpdf2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 10:37:06.000000 fpdf2-2.7.4/fpdf2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-28 10:37:06.284544 fpdf2-2.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-28 10:13:25.000000 fpdf2-2.7.4/setup.py
```

### Comparing `fpdf2-2.7.3/LICENSE` & `fpdf2-2.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.3/PKG-INFO` & `fpdf2-2.7.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: fpdf2
-Version: 2.7.3
-Summary: Simple & fast PDF generation for Python
-Home-page: https://pyfpdf.github.io/fpdf2/
-Download-URL: https://github.com/PyFPDF/fpdf2/tarball/2.7.3
-Author: Olivier PLATHEY ported by Max
-Maintainer: Lucas Cimon
-License: LGPLv3+
-Project-URL: Documentation, https://pyfpdf.github.io/fpdf2/
-Project-URL: Code, https://github.com/PyFPDF/fpdf2
-Project-URL: Issue tracker, https://github.com/PyFPDF/fpdf2/issues
-Keywords: pdf,unicode,png,jpg,ttf,barcode
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Printing
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Processing :: Markup
-Classifier: Topic :: Multimedia :: Graphics
-Classifier: Topic :: Multimedia :: Graphics :: Presentation
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Pypi latest version](https://img.shields.io/pypi/v/fpdf2.svg)](https://pypi.org/pypi/fpdf2#history)
 [![Python Support](https://img.shields.io/pypi/pyversions/fpdf2.svg)](https://pypi.org/project/fpdf2/)
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
 
 [![build status](https://github.com/PyFPDF/fpdf2/workflows/build/badge.svg)](https://github.com/PyFPDF/fpdf2/actions?query=branch%3Amaster)
 [![codecov](https://codecov.io/gh/PyFPDF/fpdf2/branch/master/graph/badge.svg)](https://codecov.io/gh/PyFPDF/fpdf2)
 ![security: bandit, pylint, semgrep](https://img.shields.io/badge/linters-bandit,pylint,semgrep-yellow.svg)
@@ -103,15 +71,15 @@
  * Images & links alternative descriptions, for accessibility
  * Table of contents & [document outline](https://pyfpdf.github.io/fpdf2/DocumentOutlineAndTableOfContents.html)
  * [Document encryption](https://pyfpdf.github.io/fpdf2/Encryption.html) & [document signing](https://pyfpdf.github.io/fpdf2/Signing.html)
  * [Annotations](https://pyfpdf.github.io/fpdf2/Annotations.html), including text highlights, and [file attachments](https://pyfpdf.github.io/fpdf2/FileAttachments.html)
  * [Presentation mode](https://pyfpdf.github.io/fpdf2/Presentations.html) with control over page display duration & transitions
  * Optional basic Markdown-like styling: `**bold**, __italics__`
  * Can render [mathematical equations & charts](https://pyfpdf.github.io/fpdf2/Maths.html)
- * Usage examples with [Django](https://www.djangoproject.com/), [Flask](https://flask.palletsprojects.com), [streamlit](https://streamlit.io/), AWS lambdas... : [Usage in web APIs](https://pyfpdf.github.io/fpdf2/UsageInWebAPI.html)
+ * Usage examples with [Django](https://www.djangoproject.com/), [Flask](https://flask.palletsprojects.com), [FastAPI](https://fastapi.tiangolo.com/), [streamlit](https://streamlit.io/), AWS lambdas... : [Usage in web APIs](https://pyfpdf.github.io/fpdf2/UsageInWebAPI.html)
  * 1000+ unit tests running under Linux & Windows, with `qpdf`-based PDF diffing, timing & memory usage checks, and a high code coverage
 
 Our 350+ reference PDF test files, generated by `fpdf2`, are validated using 3 different checkers:
 
 [![QPDF logo](https://pyfpdf.github.io/fpdf2/qpdf-logo.svg)](https://github.com/qpdf/qpdf)
 [![PDF Checker logo](https://pyfpdf.github.io/fpdf2/pdfchecker-logo.png)](https://www.datalogics.com/products/pdf-tools/pdf-checker/)
 [![VeraPDF logo](https://pyfpdf.github.io/fpdf2/vera-logo.jpg)](https://verapdf.org)
@@ -132,15 +100,15 @@
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-twitter-03A9F4?logo=twitter)](https://twitter.com/share?url=https://github.com/PyFPDF/fpdf2&t=fpdf2)
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-facebook-1976D2?logo=facebook)](https://www.facebook.com/sharer/sharer.php?u=https://github.com/PyFPDF/fpdf2)
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-linkedin-3949AB?logo=linkedin)](https://www.linkedin.com/shareArticle?url=https://github.com/PyFPDF/fpdf2&title=fpdf2)
 
 ## Documentation
 
 - [Documentation Home](https://pyfpdf.github.io/fpdf2/)
-- Tutorial in several languages: [English](https://pyfpdf.github.io/fpdf2/Tutorial.html) - [Deutsch](https://pyfpdf.github.io/fpdf2/Tutorial-de.html) - [español](https://pyfpdf.github.io/fpdf2/Tutorial-es.html) - [हिंदी](https://pyfpdf.github.io/fpdf2/Tutorial-हिंदी.html) - [português](https://pyfpdf.github.io/fpdf2/Tutorial-pt.html) - [Русский](https://pyfpdf.github.io/fpdf2/Tutorial-ru.html) - [Italian](https://pyfpdf.github.io/fpdf2/Tutorial-it.html) - [français](https://pyfpdf.github.io/fpdf2/Tutorial-fr.html) - [Ελληνικά](https://pyfpdf.github.io/fpdf2/Tutorial-gr.html) - [עברית](https://pyfpdf.github.io/fpdf2/Tutorial-he.html) - [简体中文](https://pyfpdf.github.io/fpdf2/Tutorial-zh.html) - [বাংলা](https://pyfpdf.github.io/fpdf2/Tutorial-বাংলা.html)
+- Tutorial in several languages: [English](https://pyfpdf.github.io/fpdf2/Tutorial.html) - [Deutsch](https://pyfpdf.github.io/fpdf2/Tutorial-de.html) - [español](https://pyfpdf.github.io/fpdf2/Tutorial-es.html) - [हिंदी](https://pyfpdf.github.io/fpdf2/Tutorial-hi.html) - [português](https://pyfpdf.github.io/fpdf2/Tutorial-pt.html) - [Русский](https://pyfpdf.github.io/fpdf2/Tutorial-ru.html) - [Italian](https://pyfpdf.github.io/fpdf2/Tutorial-it.html) - [français](https://pyfpdf.github.io/fpdf2/Tutorial-fr.html) - [Ελληνικά](https://pyfpdf.github.io/fpdf2/Tutorial-gr.html) - [עברית](https://pyfpdf.github.io/fpdf2/Tutorial-he.html) - [简体中文](https://pyfpdf.github.io/fpdf2/Tutorial-zh.html) - [বাংলা](https://pyfpdf.github.io/fpdf2/Tutorial-bn.html)
 - Release notes: [CHANGELOG.md](https://github.com/PyFPDF/fpdf2/blob/master/CHANGELOG.md)
 - A series of blog posts: [fpdf2 tag @ ludochaordic](https://chezsoi.org/lucas/blog/tag/fpdf2.html)
 
 You can also have a look at the `tests/`, they're great usage examples!
 
 ## Developement
 
@@ -238,15 +206,15 @@
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://nicholasjin.github.io/"><img src="https://avatars.githubusercontent.com/u/15252734?v=4?s=100" width="100px;" alt="Nicholas Jin"/><br /><sub><b>Nicholas Jin</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Anicholasjin" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://portfolio-yk-jp.vercel.app/"><img src="https://avatars.githubusercontent.com/u/69574727?v=4?s=100" width="100px;" alt="Yusuke"/><br /><sub><b>Yusuke</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=yk-jp" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Tillrzhtgrfho"><img src="https://avatars.githubusercontent.com/u/86628355?v=4?s=100" width="100px;" alt="Tillrzhtgrfho"/><br /><sub><b>Tillrzhtgrfho</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3ATillrzhtgrfho" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://dario.icu/"><img src="https://avatars.githubusercontent.com/u/35274810?v=4?s=100" width="100px;" alt="Dario Ackermann"/><br /><sub><b>Dario Ackermann</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Adarioackermann" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/TzviGreenfeld"><img src="https://avatars.githubusercontent.com/u/43534411?v=4?s=100" width="100px;" alt="Tzvi Greenfeld"/><br /><sub><b>Tzvi Greenfeld</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=TzviGreenfeld" title="Documentation">📖</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/devdev29"><img src="https://avatars.githubusercontent.com/u/88680035?v=4?s=100" width="100px;" alt="devdev29"/><br /><sub><b>devdev29</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=devdev29" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/devdev29"><img src="https://avatars.githubusercontent.com/u/88680035?v=4?s=100" width="100px;" alt="devdev29"/><br /><sub><b>devdev29</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=devdev29" title="Documentation">📖</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=devdev29" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Zenigata"><img src="https://avatars.githubusercontent.com/u/1022393?v=4?s=100" width="100px;" alt="Johan Bonneau"/><br /><sub><b>Johan Bonneau</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=Zenigata" title="Documentation">📖</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jmunoz94"><img src="https://avatars.githubusercontent.com/u/48921408?v=4?s=100" width="100px;" alt="Jesús Alberto Muñoz Mesa"/><br /><sub><b>Jesús Alberto Muñoz Mesa</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=jmunoz94" title="Tests">⚠️</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=jmunoz94" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://jdeep.me"><img src="https://avatars.githubusercontent.com/u/64089730?v=4?s=100" width="100px;" alt="Jaydeep Das"/><br /><sub><b>Jaydeep Das</b></sub></a><br /><a href="#question-JDeepD" title="Answering Questions">💬</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/seanpmulholland"><img src="https://avatars.githubusercontent.com/u/79894395?v=4?s=100" width="100px;" alt="Sean"/><br /><sub><b>Sean</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=seanpmulholland" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/andersonhc"><img src="https://avatars.githubusercontent.com/u/948125?v=4?s=100" width="100px;" alt="Anderson Herzogenrath da Costa"/><br /><sub><b>Anderson Herzogenrath da Costa</b></sub></a><br /><a href="#question-andersonhc" title="Answering Questions">💬</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=andersonhc" title="Code">💻</a> <a href="#research-andersonhc" title="Research">🔬</a> <a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Aandersonhc" title="Bug reports">🐛</a></td>
@@ -262,16 +230,18 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/TheNerdy907"><img src="https://avatars.githubusercontent.com/u/51904226?v=4?s=100" width="100px;" alt="TheNerdy907"/><br /><sub><b>TheNerdy907</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3ATheNerdy907" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/eroux"><img src="https://avatars.githubusercontent.com/u/60868?v=4?s=100" width="100px;" alt="Elie Roux"/><br /><sub><b>Elie Roux</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Aeroux" title="Bug reports">🐛</a> <a href="#ideas-eroux" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=eroux" title="Code">💻</a> <a href="#question-eroux" title="Answering Questions">💬</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/msalem99"><img src="https://avatars.githubusercontent.com/u/89017128?v=4?s=100" width="100px;" alt="msalem"/><br /><sub><b>msalem</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=msalem99" title="Documentation">📖</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/ruiz-manuel"><img src="https://avatars.githubusercontent.com/u/43274578?v=4?s=100" width="100px;" alt="Manuel Ruiz"/><br /><sub><b>Manuel Ruiz</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Aruiz-manuel" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/nsimonovici"><img src="https://avatars.githubusercontent.com/u/44460830?v=4?s=100" width="100px;" alt="Noel"/><br /><sub><b>Noel</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Ansimonovici" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://sites.google.com/view/iamavik/"><img src="https://avatars.githubusercontent.com/u/14172268?v=4?s=100" width="100px;" alt="Avik Sarkar"/><br /><sub><b>Avik Sarkar</b></sub></a><br /><a href="#translation-ssavi-ict" title="Translation">🌍</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=ssavi-ict" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://sites.google.com/view/iamavik/"><img src="https://avatars.githubusercontent.com/u/14172268?v=4?s=100" width="100px;" alt="Avik Sarkar"/><br /><sub><b>Avik Sarkar</b></sub></a><br /><a href="#translation-ssavi-ict" title="Translation">🌍</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=ssavi-ict" title="Documentation">📖</a> <a href="#question-ssavi-ict" title="Answering Questions">💬</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/aeris07"><img src="https://avatars.githubusercontent.com/u/129675592?v=4?s=100" width="100px;" alt="aeris07"/><br /><sub><b>aeris07</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Aaeris07" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/KamarulAdha"><img src="https://avatars.githubusercontent.com/u/52944294?v=4?s=100" width="100px;" alt="KamarulAdha"/><br /><sub><b>KamarulAdha</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=KamarulAdha" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Valerus5685"><img src="https://avatars.githubusercontent.com/u/7953869?v=4?s=100" width="100px;" alt="Valerus5685"/><br /><sub><b>Valerus5685</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3AValerus5685" title="Bug reports">🐛</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `fpdf2-2.7.3/README.md` & `fpdf2-2.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: fpdf2
+Version: 2.7.4
+Summary: Simple & fast PDF generation for Python
+Home-page: https://pyfpdf.github.io/fpdf2/
+Download-URL: https://github.com/PyFPDF/fpdf2/tarball/2.7.4
+Author: Olivier PLATHEY ported by Max
+Maintainer: Lucas Cimon
+License: LGPLv3+
+Project-URL: Documentation, https://pyfpdf.github.io/fpdf2/
+Project-URL: Code, https://github.com/PyFPDF/fpdf2
+Project-URL: Issue tracker, https://github.com/PyFPDF/fpdf2/issues
+Keywords: pdf,unicode,png,jpg,ttf,barcode
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Printing
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Text Processing :: Markup
+Classifier: Topic :: Multimedia :: Graphics
+Classifier: Topic :: Multimedia :: Graphics :: Presentation
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![Pypi latest version](https://img.shields.io/pypi/v/fpdf2.svg)](https://pypi.org/pypi/fpdf2#history)
 [![Python Support](https://img.shields.io/pypi/pyversions/fpdf2.svg)](https://pypi.org/project/fpdf2/)
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
 
 [![build status](https://github.com/PyFPDF/fpdf2/workflows/build/badge.svg)](https://github.com/PyFPDF/fpdf2/actions?query=branch%3Amaster)
 [![codecov](https://codecov.io/gh/PyFPDF/fpdf2/branch/master/graph/badge.svg)](https://codecov.io/gh/PyFPDF/fpdf2)
 ![security: bandit, pylint, semgrep](https://img.shields.io/badge/linters-bandit,pylint,semgrep-yellow.svg)
@@ -71,15 +103,15 @@
  * Images & links alternative descriptions, for accessibility
  * Table of contents & [document outline](https://pyfpdf.github.io/fpdf2/DocumentOutlineAndTableOfContents.html)
  * [Document encryption](https://pyfpdf.github.io/fpdf2/Encryption.html) & [document signing](https://pyfpdf.github.io/fpdf2/Signing.html)
  * [Annotations](https://pyfpdf.github.io/fpdf2/Annotations.html), including text highlights, and [file attachments](https://pyfpdf.github.io/fpdf2/FileAttachments.html)
  * [Presentation mode](https://pyfpdf.github.io/fpdf2/Presentations.html) with control over page display duration & transitions
  * Optional basic Markdown-like styling: `**bold**, __italics__`
  * Can render [mathematical equations & charts](https://pyfpdf.github.io/fpdf2/Maths.html)
- * Usage examples with [Django](https://www.djangoproject.com/), [Flask](https://flask.palletsprojects.com), [streamlit](https://streamlit.io/), AWS lambdas... : [Usage in web APIs](https://pyfpdf.github.io/fpdf2/UsageInWebAPI.html)
+ * Usage examples with [Django](https://www.djangoproject.com/), [Flask](https://flask.palletsprojects.com), [FastAPI](https://fastapi.tiangolo.com/), [streamlit](https://streamlit.io/), AWS lambdas... : [Usage in web APIs](https://pyfpdf.github.io/fpdf2/UsageInWebAPI.html)
  * 1000+ unit tests running under Linux & Windows, with `qpdf`-based PDF diffing, timing & memory usage checks, and a high code coverage
 
 Our 350+ reference PDF test files, generated by `fpdf2`, are validated using 3 different checkers:
 
 [![QPDF logo](https://pyfpdf.github.io/fpdf2/qpdf-logo.svg)](https://github.com/qpdf/qpdf)
 [![PDF Checker logo](https://pyfpdf.github.io/fpdf2/pdfchecker-logo.png)](https://www.datalogics.com/products/pdf-tools/pdf-checker/)
 [![VeraPDF logo](https://pyfpdf.github.io/fpdf2/vera-logo.jpg)](https://verapdf.org)
@@ -100,15 +132,15 @@
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-twitter-03A9F4?logo=twitter)](https://twitter.com/share?url=https://github.com/PyFPDF/fpdf2&t=fpdf2)
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-facebook-1976D2?logo=facebook)](https://www.facebook.com/sharer/sharer.php?u=https://github.com/PyFPDF/fpdf2)
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-linkedin-3949AB?logo=linkedin)](https://www.linkedin.com/shareArticle?url=https://github.com/PyFPDF/fpdf2&title=fpdf2)
 
 ## Documentation
 
 - [Documentation Home](https://pyfpdf.github.io/fpdf2/)
-- Tutorial in several languages: [English](https://pyfpdf.github.io/fpdf2/Tutorial.html) - [Deutsch](https://pyfpdf.github.io/fpdf2/Tutorial-de.html) - [español](https://pyfpdf.github.io/fpdf2/Tutorial-es.html) - [हिंदी](https://pyfpdf.github.io/fpdf2/Tutorial-हिंदी.html) - [português](https://pyfpdf.github.io/fpdf2/Tutorial-pt.html) - [Русский](https://pyfpdf.github.io/fpdf2/Tutorial-ru.html) - [Italian](https://pyfpdf.github.io/fpdf2/Tutorial-it.html) - [français](https://pyfpdf.github.io/fpdf2/Tutorial-fr.html) - [Ελληνικά](https://pyfpdf.github.io/fpdf2/Tutorial-gr.html) - [עברית](https://pyfpdf.github.io/fpdf2/Tutorial-he.html) - [简体中文](https://pyfpdf.github.io/fpdf2/Tutorial-zh.html) - [বাংলা](https://pyfpdf.github.io/fpdf2/Tutorial-বাংলা.html)
+- Tutorial in several languages: [English](https://pyfpdf.github.io/fpdf2/Tutorial.html) - [Deutsch](https://pyfpdf.github.io/fpdf2/Tutorial-de.html) - [español](https://pyfpdf.github.io/fpdf2/Tutorial-es.html) - [हिंदी](https://pyfpdf.github.io/fpdf2/Tutorial-hi.html) - [português](https://pyfpdf.github.io/fpdf2/Tutorial-pt.html) - [Русский](https://pyfpdf.github.io/fpdf2/Tutorial-ru.html) - [Italian](https://pyfpdf.github.io/fpdf2/Tutorial-it.html) - [français](https://pyfpdf.github.io/fpdf2/Tutorial-fr.html) - [Ελληνικά](https://pyfpdf.github.io/fpdf2/Tutorial-gr.html) - [עברית](https://pyfpdf.github.io/fpdf2/Tutorial-he.html) - [简体中文](https://pyfpdf.github.io/fpdf2/Tutorial-zh.html) - [বাংলা](https://pyfpdf.github.io/fpdf2/Tutorial-bn.html)
 - Release notes: [CHANGELOG.md](https://github.com/PyFPDF/fpdf2/blob/master/CHANGELOG.md)
 - A series of blog posts: [fpdf2 tag @ ludochaordic](https://chezsoi.org/lucas/blog/tag/fpdf2.html)
 
 You can also have a look at the `tests/`, they're great usage examples!
 
 ## Developement
 
@@ -206,15 +238,15 @@
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://nicholasjin.github.io/"><img src="https://avatars.githubusercontent.com/u/15252734?v=4?s=100" width="100px;" alt="Nicholas Jin"/><br /><sub><b>Nicholas Jin</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Anicholasjin" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://portfolio-yk-jp.vercel.app/"><img src="https://avatars.githubusercontent.com/u/69574727?v=4?s=100" width="100px;" alt="Yusuke"/><br /><sub><b>Yusuke</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=yk-jp" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Tillrzhtgrfho"><img src="https://avatars.githubusercontent.com/u/86628355?v=4?s=100" width="100px;" alt="Tillrzhtgrfho"/><br /><sub><b>Tillrzhtgrfho</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3ATillrzhtgrfho" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://dario.icu/"><img src="https://avatars.githubusercontent.com/u/35274810?v=4?s=100" width="100px;" alt="Dario Ackermann"/><br /><sub><b>Dario Ackermann</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Adarioackermann" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/TzviGreenfeld"><img src="https://avatars.githubusercontent.com/u/43534411?v=4?s=100" width="100px;" alt="Tzvi Greenfeld"/><br /><sub><b>Tzvi Greenfeld</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=TzviGreenfeld" title="Documentation">📖</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/devdev29"><img src="https://avatars.githubusercontent.com/u/88680035?v=4?s=100" width="100px;" alt="devdev29"/><br /><sub><b>devdev29</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=devdev29" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/devdev29"><img src="https://avatars.githubusercontent.com/u/88680035?v=4?s=100" width="100px;" alt="devdev29"/><br /><sub><b>devdev29</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=devdev29" title="Documentation">📖</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=devdev29" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Zenigata"><img src="https://avatars.githubusercontent.com/u/1022393?v=4?s=100" width="100px;" alt="Johan Bonneau"/><br /><sub><b>Johan Bonneau</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=Zenigata" title="Documentation">📖</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jmunoz94"><img src="https://avatars.githubusercontent.com/u/48921408?v=4?s=100" width="100px;" alt="Jesús Alberto Muñoz Mesa"/><br /><sub><b>Jesús Alberto Muñoz Mesa</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=jmunoz94" title="Tests">⚠️</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=jmunoz94" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://jdeep.me"><img src="https://avatars.githubusercontent.com/u/64089730?v=4?s=100" width="100px;" alt="Jaydeep Das"/><br /><sub><b>Jaydeep Das</b></sub></a><br /><a href="#question-JDeepD" title="Answering Questions">💬</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/seanpmulholland"><img src="https://avatars.githubusercontent.com/u/79894395?v=4?s=100" width="100px;" alt="Sean"/><br /><sub><b>Sean</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=seanpmulholland" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/andersonhc"><img src="https://avatars.githubusercontent.com/u/948125?v=4?s=100" width="100px;" alt="Anderson Herzogenrath da Costa"/><br /><sub><b>Anderson Herzogenrath da Costa</b></sub></a><br /><a href="#question-andersonhc" title="Answering Questions">💬</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=andersonhc" title="Code">💻</a> <a href="#research-andersonhc" title="Research">🔬</a> <a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Aandersonhc" title="Bug reports">🐛</a></td>
@@ -230,16 +262,18 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/TheNerdy907"><img src="https://avatars.githubusercontent.com/u/51904226?v=4?s=100" width="100px;" alt="TheNerdy907"/><br /><sub><b>TheNerdy907</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3ATheNerdy907" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/eroux"><img src="https://avatars.githubusercontent.com/u/60868?v=4?s=100" width="100px;" alt="Elie Roux"/><br /><sub><b>Elie Roux</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Aeroux" title="Bug reports">🐛</a> <a href="#ideas-eroux" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=eroux" title="Code">💻</a> <a href="#question-eroux" title="Answering Questions">💬</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/msalem99"><img src="https://avatars.githubusercontent.com/u/89017128?v=4?s=100" width="100px;" alt="msalem"/><br /><sub><b>msalem</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=msalem99" title="Documentation">📖</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/ruiz-manuel"><img src="https://avatars.githubusercontent.com/u/43274578?v=4?s=100" width="100px;" alt="Manuel Ruiz"/><br /><sub><b>Manuel Ruiz</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Aruiz-manuel" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/nsimonovici"><img src="https://avatars.githubusercontent.com/u/44460830?v=4?s=100" width="100px;" alt="Noel"/><br /><sub><b>Noel</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Ansimonovici" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://sites.google.com/view/iamavik/"><img src="https://avatars.githubusercontent.com/u/14172268?v=4?s=100" width="100px;" alt="Avik Sarkar"/><br /><sub><b>Avik Sarkar</b></sub></a><br /><a href="#translation-ssavi-ict" title="Translation">🌍</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=ssavi-ict" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://sites.google.com/view/iamavik/"><img src="https://avatars.githubusercontent.com/u/14172268?v=4?s=100" width="100px;" alt="Avik Sarkar"/><br /><sub><b>Avik Sarkar</b></sub></a><br /><a href="#translation-ssavi-ict" title="Translation">🌍</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=ssavi-ict" title="Documentation">📖</a> <a href="#question-ssavi-ict" title="Answering Questions">💬</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/aeris07"><img src="https://avatars.githubusercontent.com/u/129675592?v=4?s=100" width="100px;" alt="aeris07"/><br /><sub><b>aeris07</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Aaeris07" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/KamarulAdha"><img src="https://avatars.githubusercontent.com/u/52944294?v=4?s=100" width="100px;" alt="KamarulAdha"/><br /><sub><b>KamarulAdha</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=KamarulAdha" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Valerus5685"><img src="https://avatars.githubusercontent.com/u/7953869?v=4?s=100" width="100px;" alt="Valerus5685"/><br /><sub><b>Valerus5685</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3AValerus5685" title="Bug reports">🐛</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `fpdf2-2.7.3/fpdf/__init__.py` & `fpdf2-2.7.4/fpdf/__init__.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.3/fpdf/actions.py` & `fpdf2-2.7.4/fpdf/actions.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.3/fpdf/annotations.py` & `fpdf2-2.7.4/fpdf/annotations.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.3/fpdf/deprecation.py` & `fpdf2-2.7.4/fpdf/deprecation.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.3/fpdf/drawing.py` & `fpdf2-2.7.4/fpdf/drawing.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.3/fpdf/encryption.py` & `fpdf2-2.7.4/fpdf/encryption.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.3/fpdf/enums.py` & `fpdf2-2.7.4/fpdf/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,14 +126,18 @@
                 int or a string.
         """
         if isinstance(value, cls):
             return value
 
         if isinstance(value, str):
             try:
+                return cls[value.upper()]
+            except KeyError:
+                pass
+            try:
                 flags = cls[value[0].upper()]
                 for char in value[1:]:
                     flags = flags | cls[char.upper()]
                 return flags
             except KeyError:
                 raise ValueError(f"{value} is not a valid {cls.__name__}") from None
 
@@ -194,14 +198,15 @@
             return cls.L
         return super(cls, cls).coerce(value)
 
 
 class TextEmphasis(CoerciveIntFlag):
     """
     Indicates use of bold / italics / underline.
+
     This enum values can be combined with & and | operators:
         style = B | I
     """
 
     B = 1
     "Bold"
 
@@ -227,14 +232,32 @@
             if value.upper() == "ITALICS":
                 return cls.I
             if value.upper() == "UNDERLINE":
                 return cls.U
         return super(cls, cls).coerce(value)
 
 
+class MethodReturnValue(CoerciveIntFlag):
+    """
+    Defines the return value(s) of a FPDF content-rendering method.
+
+    This enum values can be combined with & and | operators:
+        PAGE_BREAK | LINES
+    """
+
+    PAGE_BREAK = 1
+    "The method will return a boolean indicating if a page break occured"
+
+    LINES = 2
+    "The method will return a multi-lines array of strings, after performing word-wrapping"
+
+    HEIGHT = 4
+    "The method will return how much vertical space was used"
+
+
 class TableBordersLayout(CoerciveEnum):
     "Defines how to render table borders"
 
     ALL = intern("ALL")
     "Draw all table cells borders"
 
     NONE = intern("NONE")
```

### Comparing `fpdf2-2.7.3/fpdf/errors.py` & `fpdf2-2.7.4/fpdf/errors.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.3/fpdf/fonts.py` & `fpdf2-2.7.4/fpdf/fonts.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         "family",
         "emphasis",
         "size_pt",
         "color",
         "fill_color",
     )
     family: Optional[str]
-    emphasis: Optional[TextEmphasis]
+    emphasis: Optional[TextEmphasis]  # can be a combination: B | U
     size_pt: Optional[int]
     # Colors are single number grey scales or (red, green, blue) tuples:
     color: Optional[Union[int, tuple, DeviceGray, DeviceRGB]]
     fill_color: Optional[Union[int, tuple, DeviceGray, DeviceRGB]]
 
     def __init__(
         self, family=None, emphasis=None, size_pt=None, color=None, fill_color=None
```

### Comparing `fpdf2-2.7.3/fpdf/fpdf.py` & `fpdf2-2.7.4/fpdf/fpdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     AnnotationFlag,
     AnnotationName,
     CharVPos,
     Corner,
     EncryptionMethod,
     FontDescriptorFlags,
     FileAttachmentAnnotationName,
+    MethodReturnValue,
     PageLayout,
     PageMode,
     PathPaintRule,
     RenderStyle,
     TextEmphasis,
     TextMarkupType,
     TextMode,
@@ -88,15 +89,15 @@
 from .table import Table
 from .util import (
     escape_parens,
     get_scale_factor,
 )
 
 # Public global variables:
-FPDF_VERSION = "2.7.3"
+FPDF_VERSION = "2.7.4"
 PAGE_FORMATS = {
     "a3": (841.89, 1190.55),
     "a4": (595.28, 841.89),
     "a5": (420.94, 595.28),
     "letter": (612, 792),
     "legal": (612, 1008),
 }
@@ -252,15 +253,15 @@
 
 
 def check_page(fn):
     """Decorator to protect drawing methods"""
 
     @wraps(fn)
     def wrapper(self, *args, **kwargs):
-        if not self.page and not kwargs.get("split_only"):
+        if not self.page and not (kwargs.get("dry_run") or kwargs.get("split_only")):
             raise FPDFException("No page open, you need to call add_page() first")
         return fn(self, *args, **kwargs)
 
     return wrapper
 
 
 class FPDF(GraphicsStateMixin):
@@ -3338,32 +3339,51 @@
         x = self.x
         self.add_page(same=True)
         self.x = x  # restore x but not y after drawing header
 
     def _has_next_page(self):
         return self.pages_count > self.page
 
+    @contextmanager
+    def _disable_writing(self):
+        self._out = lambda *args, **kwargs: None
+        prev_page, prev_x, prev_y = self.page, self.x, self.y
+        self._push_local_stack()
+        try:
+            yield
+        finally:
+            self._pop_local_stack()
+            # restore location:
+            for p in range(prev_page + 1, self.page + 1):
+                del self.pages[p]
+            self.page = prev_page
+            self.set_xy(prev_x, prev_y)
+            # restore writing function:
+            del self._out
+
     @check_page
     def multi_cell(
         self,
         w,
         h=None,
         txt="",
         border=0,
         align=Align.J,
         fill=False,
-        split_only=False,
+        split_only=False,  # DEPRECATED
         link="",
         ln="DEPRECATED",
         max_line_height=None,
         markdown=False,
         print_sh=False,
         new_x=XPos.RIGHT,
         new_y=YPos.NEXT,
         wrapmode: WrapMode = WrapMode.WORD,
+        dry_run=False,
+        output=MethodReturnValue.PAGE_BREAK,
     ):
         """
         This method allows printing text with line breaks. They can be automatic
         (breaking at the most recent space or soft-hyphen character) as soon as the text
         reaches the right border of the cell, or explicit (via the `\\n` character).
         As many cells as necessary are stacked, one below the other.
         Text can be aligned, centered or justified. The cell block can be framed and
@@ -3380,35 +3400,68 @@
                 `L`: left ; `T`: top ; `R`: right ; `B`: bottom. Default value: 0.
             align (fpdf.enums.Align, str): Allows to center or align the text.
                 Possible values are:
                 `J`: justify (default value); `L` or empty string: left align;
                 `C`: center; `X`: center around current x; `R`: right align
             fill (bool): Indicates if the cell background must be painted (`True`)
                 or transparent (`False`). Default value: False.
-            split_only (bool): if `True`, does not output anything, only perform
-                word-wrapping and return the resulting multi-lines array of strings.
+            split_only (bool): **DEPRECATED since 2.7.4**:
+                Use `dry_run=True` and `output=("LINES",)` instead.
             link (str): optional link to add on the cell, internal
                 (identifier returned by `add_link`) or external URL.
             new_x (fpdf.enums.XPos, str): New current position in x after the call. Default: RIGHT
             new_y (fpdf.enums.YPos, str): New current position in y after the call. Default: NEXT
             ln (int): **DEPRECATED since 2.5.1**: Use `new_x` and `new_y` instead.
             max_line_height (float): optional maximum height of each sub-cell generated
             markdown (bool): enable minimal markdown-like markup to render part
                 of text as bold / italics / underlined. Default to False.
             print_sh (bool): Treat a soft-hyphen (\\u00ad) as a normal printable
                 character, instead of a line breaking opportunity. Default value: False
             wrapmode (fpdf.enums.WrapMode): "WORD" for word based line wrapping (default),
                 "CHAR" for character based line wrapping.
+            dry_run (bool): if `True`, does not output anything in the document.
+                Can be useful when combined with `output`.
+            output (fpdf.enums.MethodReturnValue): defines what this method returns.
+                If several enum values are joined, the result will be a tuple.
 
         Using `new_x=XPos.RIGHT, new_y=XPos.TOP, maximum height=pdf.font_size` is
         useful to build tables with multiline text in cells.
 
-        Returns: a boolean indicating if page break was triggered,
-            or if `split_only == True`: `txt` splitted into lines in an array
+        Returns: a single value or a tuple, depending on the `output` parameter value
         """
+        if split_only:
+            warnings.warn(
+                (
+                    'The parameter "split_only" is deprecated.'
+                    ' Use instead dry_run=True and output="LINES".'
+                ),
+                DeprecationWarning,
+                stacklevel=3,
+            )
+        if dry_run or split_only:
+            with self._disable_writing():
+                return self.multi_cell(
+                    w=w,
+                    h=h,
+                    txt=txt,
+                    border=border,
+                    align=align,
+                    fill=fill,
+                    link=link,
+                    ln=ln,
+                    max_line_height=max_line_height,
+                    markdown=markdown,
+                    print_sh=print_sh,
+                    new_x=new_x,
+                    new_y=new_y,
+                    wrapmode=wrapmode,
+                    dry_run=False,
+                    split_only=False,
+                    output=MethodReturnValue.LINES if split_only else output,
+                )
         wrapmode = WrapMode.coerce(wrapmode)
         if isinstance(w, str) or isinstance(h, str):
             raise ValueError(
                 "Parameter 'w' and 'h' must be numbers, not strings."
                 " You can omit them by passing string content with txt="
             )
         new_x = XPos.coerce(new_x)
@@ -3439,18 +3492,14 @@
                 ),
                 DeprecationWarning,
                 stacklevel=3,
             )
         align = Align.coerce(align)
 
         page_break_triggered = False
-        if split_only:
-            self._out = lambda *args, **kwargs: None
-            self.add_page = lambda *args, **kwargs: None
-            self._perform_page_break_if_need_be = lambda *args, **kwargs: None
 
         if h is None:
             h = self.font_size
         # If width is 0, set width to available width between margins
         if w == 0:
             w = self.w - self.r_margin - self.x
         maximum_allowed_width = w - 2 * self.c_margin
@@ -3458,14 +3507,15 @@
         # Calculate text length
         txt = self.normalize_text(txt)
         normalized_string = txt.replace("\r", "")
         styled_text_fragments = self._preload_font_styles(normalized_string, markdown)
 
         prev_font_style, prev_underline = self.font_style, self.underline
         prev_x, prev_y = self.x, self.y
+        total_height = 0
 
         if not border:
             border = ""
         elif border == 1:
             border = "LTRB"
 
         text_lines = []
@@ -3486,16 +3536,14 @@
                     "",
                     text_width=0,
                     number_of_spaces=0,
                     justify=False,
                     trailing_nl=False,
                 )
             ]
-        if align == Align.X:
-            prev_x = self.x
         should_render_bottom_blank_cell = False
         for text_line_index, text_line in enumerate(text_lines):
             is_last_line = text_line_index == len(text_lines) - 1
             should_render_bottom_blank_cell = False
             if max_line_height is not None and h > max_line_height:
                 current_cell_height = max_line_height
                 h -= current_cell_height
@@ -3523,14 +3571,15 @@
                 new_x=new_x if not has_line_after else XPos.LEFT,
                 new_y=new_y if not has_line_after else YPos.NEXT,
                 align=Align.L if (align == Align.J and is_last_line) else align,
                 fill=fill,
                 link=link,
             )
             page_break_triggered = page_break_triggered or new_page
+            total_height += current_cell_height
             if not is_last_line and align == Align.X:
                 # prevent cumulative shift to the left
                 self.x = prev_x
         if should_render_bottom_blank_cell:
             new_page = self._render_styled_text_line(
                 TextLine(
                     "",
@@ -3562,34 +3611,37 @@
         if text_line.trailing_nl and new_y in (YPos.LAST, YPos.NEXT):
             # The line renderer can't handle trailing newlines in the text.
             self.ln()
 
         if new_y == YPos.TOP:  # We may have jumped a few lines -> reset
             self.y = prev_y
 
-        if split_only:
-            # restore writing functions
-            del self.add_page
-            del self._out
-            del self._perform_page_break_if_need_be
-            self.set_xy(prev_x, prev_y)  # restore location
-            result = []
-            for text_line in text_lines:
-                characters = []
-                for frag in text_line.fragments:
-                    characters.extend(frag.characters)
-                result.append("".join(characters))
-            return result
         if markdown:
             if self.font_style != prev_font_style:
                 self.font_style = prev_font_style
                 self.current_font = self.fonts[self.font_family + self.font_style]
             self.underline = prev_underline
 
-        return page_break_triggered
+        output = MethodReturnValue.coerce(output)
+        return_value = ()
+        if output & MethodReturnValue.PAGE_BREAK:
+            return_value += (page_break_triggered,)
+        if output & MethodReturnValue.LINES:
+            output_lines = []
+            for text_line in text_lines:
+                characters = []
+                for frag in text_line.fragments:
+                    characters.extend(frag.characters)
+                output_lines.append("".join(characters))
+            return_value += (output_lines,)
+        if output & MethodReturnValue.HEIGHT:
+            return_value += (total_height,)
+        if len(return_value) == 1:
+            return return_value[0]
+        return return_value
 
     @check_page
     def write(
         self,
         h: float = None,
         txt: str = "",
         link: str = "",
@@ -3698,15 +3750,15 @@
 
         **Remarks**:
         * if an image is used several times, only one copy is embedded in the file.
         * when using an animated GIF, only the first frame is used.
 
         Args:
             name: either a string representing a file path to an image, an URL to an image,
-                an io.BytesIO, or a instance of `PIL.Image.Image`
+                bytes, an io.BytesIO, or a instance of `PIL.Image.Image`
             x (float, fpdf.enums.Align): optional horizontal position where to put the image on the page.
                 If not specified or equal to None, the current abscissa is used.
                 `Align.C` can also be passed to center the image horizontally;
                 and `Align.R` to place it along the right page margin
             y (float): optional vertical position where to put the image on the page.
                 If not specified or equal to None, the current ordinate is used.
                 After the call, the current ordinate is moved to the bottom of the image
@@ -3739,14 +3791,18 @@
                 DeprecationWarning,
                 stacklevel=3,
             )
         if str(name).endswith(".svg"):
             # Insert it as a PDF path:
             img = load_image(str(name))
             return self._vector_image(img, x, y, w, h, link, title, alt_text)
+        if isinstance(name, bytes) and _is_svg(name.strip()):
+            return self._vector_image(
+                io.BytesIO(name), x, y, w, h, link, title, alt_text
+            )
         if isinstance(name, io.BytesIO) and _is_svg(name.getvalue().strip()):
             return self._vector_image(name, x, y, w, h, link, title, alt_text)
         name, img, info = self.preload_image(name, dims)
         if "smask" in info:
             self._set_min_pdf_version("1.4")
 
         # Automatic width and height calculation if needed
@@ -3821,22 +3877,23 @@
                 before storing it in the PDF.
 
         Returns: an instance of `ImageInfo`
         """
         if isinstance(name, str):
             img = None
         elif isinstance(name, Image):
-            bytes = name.tobytes()
+            bytes_ = name.tobytes()
             img_hash = hashlib.new("md5", usedforsecurity=False)  # nosec B324
-            img_hash.update(bytes)
+            img_hash.update(bytes_)
             name, img = img_hash.hexdigest(), name
-        elif isinstance(name, io.BytesIO):
-            bytes = name.getvalue().strip()
+        elif isinstance(name, (bytes, io.BytesIO)):
+            bytes_ = name.getvalue() if isinstance(name, io.BytesIO) else name
+            bytes_ = bytes_.strip()
             img_hash = hashlib.new("md5", usedforsecurity=False)  # nosec B324
-            img_hash.update(bytes)
+            img_hash.update(bytes_)
             name, img = img_hash.hexdigest(), name
         else:
             name, img = str(name), name
         info = self.images.get(name)
         if info:
             info["usages"] += 1
         else:
```

### Comparing `fpdf2-2.7.3/fpdf/graphics_state.py` & `fpdf2-2.7.4/fpdf/graphics_state.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.3/fpdf/html.py` & `fpdf2-2.7.4/fpdf/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 "HTML renderer"
 
-__author__ = "Mariano Reingart <reingart@gmail.com>"
-__copyright__ = "Copyright (C) 2010 Mariano Reingart"
-__license__ = "LGPL 3.0"
-
-# Inspired by tuto5.py and several examples from fpdf.org, html2fpdf, etc.
-
 import logging, warnings
 from html.parser import HTMLParser
 
 from .enums import TextEmphasis, XPos, YPos
+from .errors import FPDFException
 from .fonts import FontFace
-from .table import Table
+from .table import Table, TableBordersLayout
 
 import re
 
 LOGGER = logging.getLogger(__name__)
 BULLET_WIN1252 = "\x95"  # BULLET character in Windows-1252 encoding
 DEFAULT_HEADING_SIZES = dict(h1=24, h2=18, h3=14, h4=12, h5=10, h6=8)
 LEADING_SPACE = re.compile(r"^\s+")
@@ -207,14 +202,15 @@
         pdf,
         image_map=None,
         li_tag_indent=5,
         dd_tag_indent=10,
         table_line_separators=False,
         ul_bullet_char=BULLET_WIN1252,
         heading_sizes=None,
+        pre_code_font="courier",
         warn_on_tags_not_matching=True,
         **_,
     ):
         """
         Args:
             pdf (FPDF): an instance of `fpdf.FPDF`
             image_map (function): an optional one-argument function that map <img> "src"
@@ -245,14 +241,15 @@
         self.font_color = 0, 0, 0  # initialize font color, r,g,b format
         self.heading_level = None
         self.heading_sizes = dict(**DEFAULT_HEADING_SIZES)
         self.heading_above = 0.2  # extra space above heading, relative to font size
         self.heading_below = 0.2  # extra space below heading, relative to font size
         if heading_sizes:
             self.heading_sizes.update(heading_sizes)
+        self.pre_code_font = pre_code_font
         self.warn_on_tags_not_matching = warn_on_tags_not_matching
         self._tags_stack = []
         # <table>-related properties:
         self.table_line_separators = table_line_separators
         self.table = None  # becomes a Table instance when processing <table> tags
         self.table_row = None  # becomes a Row instance when processing <tr> tags
         self.tr = None  # becomes a dict of attributes when processing <tr> tags
@@ -376,18 +373,18 @@
             self.set_font(size=hsize)
             if attrs:
                 self.align = attrs.get("align")
         if tag == "hr":
             self.pdf.add_page(same=True)
         if tag == "code":
             self.font_stack.append((self.font_face, self.font_size, self.font_color))
-            self.set_font("courier", 11)
+            self.set_font(self.pre_code_font, 11)
         if tag == "pre":
             self.font_stack.append((self.font_face, self.font_size, self.font_color))
-            self.set_font("courier", 11)
+            self.set_font(self.pre_code_font, 11)
             self.pre_formatted = True
         if tag == "blockquote":
             self.pdf.set_text_color(100, 0, 45)
             self.indent += 1
             self.pdf.ln(3)
         if tag == "ul":
             self.indent += 1
@@ -435,29 +432,41 @@
                 )
             else:
                 borders_layout = (
                     "HORIZONTAL_LINES"
                     if self.table_line_separators
                     else "SINGLE_TOP_LINE"
                 )
+            align = attrs.get("align", "center").upper()
             self.table = Table(
                 self.pdf,
+                align=align,
                 borders_layout=borders_layout,
                 line_height=self.h * 1.30,
                 width=width,
             )
             self.pdf.ln()
         if tag == "tr":
+            if not self.table:
+                raise FPDFException("Invalid HTML: <tr> used outside any <table>")
             self.tr = {k.lower(): v for k, v in attrs.items()}
             self.table_row = self.table.row()
         if tag in ("td", "th"):
+            if not self.table_row:
+                raise FPDFException(f"Invalid HTML: <{tag}> used outside any <tr>")
             self.td_th = {k.lower(): v for k, v in attrs.items()}
             if tag == "th":
                 self.td_th["align"] = "CENTER"
                 self.td_th["b"] = True
+            elif len(self.table.rows) == 1 and not self.table_row.cells:
+                # => we are in the 1st <tr>, and the 1st cell is a <td>
+                # => we do not treat the first row as a header
+                # pylint: disable=protected-access
+                self.table._borders_layout = TableBordersLayout.NONE
+                self.table._first_row_as_headings = False
             if "height" in attrs:
                 LOGGER.warning(
                     'Ignoring unsupported height="%s" specified on a <%s>',
                     attrs["height"],
                     tag,
                 )
             if "width" in attrs:
```

### Comparing `fpdf2-2.7.3/fpdf/image_parsing.py` & `fpdf2-2.7.4/fpdf/image_parsing.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,27 +104,30 @@
     return True
 
 
 def get_img_info(filename, img=None, image_filter="AUTO", dims=None):
     """
     Args:
         filename: in a format that can be passed to load_image
-        img: optional `BytesIO` or `PIL.Image.Image` instance
+        img: optional `bytes`, `BytesIO` or `PIL.Image.Image` instance
         image_filter (str): one of the SUPPORTED_IMAGE_FILTERS
     """
     if Image is None:
         raise EnvironmentError("Pillow not available - fpdf2 cannot insert images")
 
     is_pil_img = True
+    jpeg_inverted = False  # flag to check whether a cmyk image is jpeg or not, if set to True the decode array is inverted in output.py
     img_raw_data = None
     if not img or isinstance(img, (Path, str)):
         img_raw_data = load_image(filename)
         img = Image.open(img_raw_data)
         is_pil_img = False
     elif not isinstance(img, Image.Image):
+        if isinstance(img, bytes):
+            img = BytesIO(img)
         img_raw_data = img
         img = Image.open(img_raw_data)
         is_pil_img = False
 
     img_altered = False
     if dims:
         img = img.resize(dims, resample=RESAMPLE)
@@ -140,42 +143,47 @@
             image_filter = "CCITTFaxDecode"
         else:
             image_filter = "FlateDecode"
 
     if img.mode in ("P", "PA") and image_filter != "FlateDecode":
         img = img.convert("RGBA")
 
-    if img.mode not in ("1", "L", "LA", "RGB", "RGBA", "P", "PA"):
+    if img.mode not in ("1", "L", "LA", "RGB", "RGBA", "P", "PA", "CMYK"):
         img = img.convert("RGBA")
         img_altered = True
 
     w, h = img.size
     info = {}
 
     iccp = None
     if "icc_profile" in img.info:
         if is_iccp_valid(img.info["icc_profile"], filename):
             iccp = img.info["icc_profile"]
 
     if img_raw_data is not None and not img_altered:
         # if we can use the original image bytes directly we do (JPEG and group4 TIFF only):
         if img.format == "JPEG" and image_filter == "DCTDecode":
-            dpn, bpc, colspace = 3, 8, "DeviceRGB"
+            if img.mode in ("RGB", "RGBA"):
+                dpn, bpc, colspace = 3, 8, "DeviceRGB"
+            elif img.mode == "CMYK":
+                dpn, bpc, colspace = 4, 8, "DeviceCMYK"
+                jpeg_inverted = True
             if img.mode == "L":
                 dpn, bpc, colspace = 1, 8, "DeviceGray"
             img_raw_data.seek(0)
             return {
                 "data": img_raw_data.read(),
                 "w": w,
                 "h": h,
                 "cs": colspace,
                 "iccp": iccp,
                 "dpn": dpn,
                 "bpc": bpc,
                 "f": image_filter,
+                "inverted": jpeg_inverted,
                 "dp": f"/Predictor 15 /Colors {dpn} /Columns {w}",
             }
         # We can directly copy the data out of a CCITT Group 4 encoded TIFF, if it
         # only contains a single strip
         if (
             img.format == "TIFF"
             and image_filter == "CCITTFaxDecode"
@@ -212,14 +220,15 @@
                 "w": w,
                 "h": h,
                 "iccp": None,
                 "dpn": dpn,
                 "cs": colspace,
                 "bpc": bpc,
                 "f": image_filter,
+                "inverted": jpeg_inverted,
                 "dp": f"/BlackIs1 {str(not inverted).lower()} /Columns {w} /K -1 /Rows {h}",
             }
 
     # garbage collection
     img_raw_data = None
 
     if img.mode == "1":
@@ -257,14 +266,17 @@
         alpha_channel = slice(1, None, 2)
         info["data"] = _to_data(img, image_filter, remove_slice=alpha_channel)
         if _has_alpha(img, alpha_channel) and image_filter not in (
             "DCTDecode",
             "JPXDecode",
         ):
             info["smask"] = _to_data(img, image_filter, select_slice=alpha_channel)
+    elif img.mode == "CMYK":
+        dpn, bpc, colspace = 4, 8, "DeviceCMYK"
+        info["data"] = _to_data(img, image_filter)
     elif img.mode == "RGB":
         dpn, bpc, colspace = 3, 8, "DeviceRGB"
         info["data"] = _to_data(img, image_filter)
     else:  # RGBA image
         dpn, bpc, colspace = 3, 8, "DeviceRGB"
         alpha_channel = slice(3, None, 4)
         info["data"] = _to_data(img, image_filter, remove_slice=alpha_channel)
@@ -287,14 +299,15 @@
             "w": w,
             "h": h,
             "cs": colspace,
             "iccp": iccp,
             "bpc": bpc,
             "dpn": dpn,
             "f": image_filter,
+            "inverted": jpeg_inverted,
             "dp": dp,
         }
     )
 
     return info
```

### Comparing `fpdf2-2.7.3/fpdf/line_break.py` & `fpdf2-2.7.4/fpdf/line_break.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.3/fpdf/linearization.py` & `fpdf2-2.7.4/fpdf/linearization.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.3/fpdf/outline.py` & `fpdf2-2.7.4/fpdf/outline.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.3/fpdf/output.py` & `fpdf2-2.7.4/fpdf/output.py`

 * *Files 0% similar despite different names*

```diff
@@ -762,18 +762,16 @@
             color_space = PDFArray(
                 ["/Indexed", "/DeviceRGB", f"{len(info['pal']) // 3 - 1}"]
             )
         elif iccp_i is not None:
             iccp_pdf_i = self._ensure_iccp(info)
             color_space = PDFArray(["/ICCBased", str(iccp_pdf_i), str("0"), "R"])
         elif color_space == "DeviceCMYK":
-            decode = "[1 0 1 0 1 0 1 0]"
-            raise NotImplementedError(
-                "fpdf2 does not support DeviceCMYK ColorSpace yet - cf. issue #711"
-            )
+            if info["inverted"] is True:
+                decode = "[1 0 1 0 1 0 1 0]"
 
         decode_parms = f"<<{info['dp']} /BitsPerComponent {info['bpc']}>>"
         img_obj = PDFXObject(
             subtype="Image",
             contents=info["data"],
             width=info["w"],
             height=info["h"],
```

### Comparing `fpdf2-2.7.3/fpdf/prefs.py` & `fpdf2-2.7.4/fpdf/prefs.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.3/fpdf/recorder.py` & `fpdf2-2.7.4/fpdf/recorder.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.3/fpdf/sign.py` & `fpdf2-2.7.4/fpdf/sign.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.3/fpdf/structure_tree.py` & `fpdf2-2.7.4/fpdf/structure_tree.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.3/fpdf/svg.py` & `fpdf2-2.7.4/fpdf/svg.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.3/fpdf/syntax.py` & `fpdf2-2.7.4/fpdf/syntax.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.3/fpdf/table.py` & `fpdf2-2.7.4/fpdf/table.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 from dataclasses import dataclass
 from numbers import Number
-from typing import List, Optional, Union
+from typing import Optional, Union
 
 from .enums import Align, TableBordersLayout, TableCellFillMode
+from .enums import MethodReturnValue
+from .errors import FPDFException
 from .fonts import FontFace
 
 
 DEFAULT_HEADINGS_STYLE = FontFace(emphasis="BOLD")
 
 
+@dataclass(frozen=True)
+class RowLayoutInfo:
+    height: int
+    triggers_page_jump: bool
+
+
 class Table:
     """
     Object that `fpdf.FPDF.table()` yields, used to build a table in the document.
     Detailed usage documentation: https://pyfpdf.github.io/fpdf2/Tables.html
     """
 
     def __init__(
@@ -74,39 +82,61 @@
         self.rows.append(row)
         for cell in cells:
             row.cell(cell)
         return row
 
     def render(self):
         "This is an internal method called by `fpdf.FPDF.table()` once the table is finished"
+        # Starting with some sanity checks:
         if self._width > self._fpdf.epw:
             raise ValueError(
-                f"Invalid value provided .width={self._width}: effective page width is {self._fpdf.epw}"
+                f"Invalid value provided width={self._width}: effective page width is {self._fpdf.epw}"
             )
         table_align = Align.coerce(self._align)
         if table_align == Align.J:
-            raise ValueError("JUSTIFY is an invalid value for table .align")
+            raise ValueError(
+                "JUSTIFY is an invalid value for FPDF.table() 'align' parameter"
+            )
+        if self._first_row_as_headings:
+            if not self._headings_style:
+                raise ValueError(
+                    "headings_style must be provided to FPDF.table() if first_row_as_headings=True"
+                )
+            emphasis = self._headings_style.emphasis
+            if emphasis is not None:
+                family = self._headings_style.family or self._fpdf.font_family
+                font_key = family + emphasis.style
+                if (
+                    font_key not in self._fpdf.core_fonts
+                    and font_key not in self._fpdf.fonts
+                ):
+                    # Raising a more explicit error than the one from set_font():
+                    raise FPDFException(
+                        f"Using font emphasis '{emphasis.style}' in table headings require the corresponding font style to be added using add_font()"
+                    )
+        # Defining table global horizontal position:
         prev_l_margin = self._fpdf.l_margin
         if table_align == Align.C:
             self._fpdf.l_margin = (self._fpdf.w - self._width) / 2
             self._fpdf.x = self._fpdf.l_margin
         elif table_align == Align.R:
-            self._fpdf.l_margin = self._fpdf.w - self._width
+            self._fpdf.l_margin = self._fpdf.w - self._fpdf.r_margin - self._width
             self._fpdf.x = self._fpdf.l_margin
         elif self._fpdf.x != self._fpdf.l_margin:
             self._fpdf.l_margin = self._fpdf.x
+        # Starting the actual rows & cells rendering:
         for i in range(len(self.rows)):
-            with self._fpdf.offset_rendering() as test:
-                self._render_table_row(i)
-            if test.page_break_triggered:
+            row_layout_info = self._get_row_layout_info(i)
+            if row_layout_info.triggers_page_jump:
                 # pylint: disable=protected-access
                 self._fpdf._perform_page_break()
                 if self._first_row_as_headings:  # repeat headings on top:
                     self._render_table_row(0)
-            self._render_table_row(i)
+            self._render_table_row(i, row_layout_info)
+        # Restoring altered FPDF settings:
         self._fpdf.l_margin = prev_l_margin
         self._fpdf.x = self._fpdf.l_margin
 
     def get_cell_border(self, i, j):
         """
         Defines which cell borders should be drawn.
         Returns a string containing some or all of the letters L/R/T/B,
@@ -157,78 +187,59 @@
             border = list("TB")
             if i != 1 and "T" in border:
                 border.remove("T")
             if i != 0 and "B" in border:
                 border.remove("B")
         return "".join(border)
 
-    def _render_table_row(self, i, fill=False, **kwargs):
+    def _render_table_row(self, i, row_layout_info=None, fill=False, **kwargs):
+        if not row_layout_info:
+            row_layout_info = self._get_row_layout_info(i)
         row = self.rows[i]
-        lines_heights_per_cell = self._get_lines_heights_per_cell(i)
-        row_height = max(sum(lines_heights) for lines_heights in lines_heights_per_cell)
         j = 0
         while j < len(row.cells):
-            cell_line_height = row_height / len(lines_heights_per_cell[j])
             self._render_table_cell(
                 i,
                 j,
-                cell_line_height=cell_line_height,
-                row_height=row_height,
+                row_height=row_layout_info.height,
                 fill=fill,
                 **kwargs,
             )
             j += row.cells[j].colspan
-        self._fpdf.ln(row_height)
+        self._fpdf.ln(row_layout_info.height)
 
     # pylint: disable=inconsistent-return-statements
     def _render_table_cell(
         self,
         i,
         j,
-        cell_line_height,
         row_height,
         fill=False,
-        lines_heights_only=False,
         **kwargs,
     ):
-        """
-        If `lines_heights_only` is True, returns a list of lines (subcells) heights.
-        """
         row = self.rows[i]
         cell = row.cells[j]
         col_width = self._get_col_width(i, j, cell.colspan)
-        lines_heights = []
+        img_height = 0
         if cell.img:
-            if lines_heights_only:
-                info = self._fpdf.preload_image(cell.img)[2]
-                img_ratio = info.width / info.height
-                if cell.img_fill_width or row_height * img_ratio > col_width:
-                    img_height = col_width / img_ratio
-                else:
-                    img_height = row_height
-                lines_heights += [img_height]
-            else:
-                x, y = self._fpdf.x, self._fpdf.y
-                self._fpdf.image(
-                    cell.img,
-                    w=col_width,
-                    h=0 if cell.img_fill_width else row_height,
-                    keep_aspect_ratio=True,
-                )
-                self._fpdf.set_xy(x, y)
+            x, y = self._fpdf.x, self._fpdf.y
+            img_height = self._fpdf.image(
+                cell.img,
+                w=col_width,
+                h=0 if cell.img_fill_width else row_height,
+                keep_aspect_ratio=True,
+            ).rendered_height
+            self._fpdf.set_xy(x, y)
         text_align = cell.align or self._text_align
         if not isinstance(text_align, (Align, str)):
             text_align = text_align[j]
         if i == 0 and self._first_row_as_headings:
             style = self._headings_style
         else:
             style = cell.style or row.style
-        if lines_heights_only and style:
-            # Avoid to generate font-switching instructions: BT /F... Tf ET
-            style = style.replace(emphasis=None)
         if style and style.fill_color:
             fill = True
         elif (
             not fill
             and self._cell_fill_color
             and self._cell_fill_mode != TableCellFillMode.NONE
         ):
@@ -241,32 +252,29 @@
         if fill and self._cell_fill_color and not (style and style.fill_color):
             style = (
                 style.replace(fill_color=self._cell_fill_color)
                 if style
                 else FontFace(fill_color=self._cell_fill_color)
             )
         with self._fpdf.use_font_face(style):
-            lines = self._fpdf.multi_cell(
+            page_break, cell_height = self._fpdf.multi_cell(
                 w=col_width,
                 h=row_height,
                 txt=cell.text,
-                max_line_height=cell_line_height,
+                max_line_height=self._line_height,
                 border=self.get_cell_border(i, j),
                 align=text_align,
                 new_x="RIGHT",
                 new_y="TOP",
                 fill=fill,
-                split_only=lines_heights_only,
                 markdown=self._markdown,
+                output=MethodReturnValue.PAGE_BREAK | MethodReturnValue.HEIGHT,
                 **kwargs,
             )
-        if lines_heights_only and not cell.img:
-            lines_heights += (len(lines) or 1) * [self._line_height]
-        if lines_heights_only:
-            return lines_heights
+        return page_break, max(img_height, cell_height)
 
     def _get_col_width(self, i, j, colspan=1):
         if not self._col_widths:
             cols_count = self.rows[i].cols_count
             return colspan * (self._width / cols_count)
         if isinstance(self._col_widths, Number):
             return colspan * self._col_widths
@@ -277,28 +285,36 @@
         # pylint: disable=unsubscriptable-object
         col_width = 0
         for k in range(j, j + colspan):
             col_ratio = self._col_widths[k] / sum(self._col_widths)
             col_width += col_ratio * self._width
         return col_width
 
-    def _get_lines_heights_per_cell(self, i) -> List[List[int]]:
+    def _get_row_layout_info(self, i):
+        """
+        Uses FPDF.offset_rendering() to detect a potential page jump
+        and compute the cells heights.
+        """
         row = self.rows[i]
-        lines_heights = []
-        for j in range(len(row.cells)):
-            lines_heights.append(
-                self._render_table_cell(
+        heights_per_cell = []
+        any_page_break = False
+        # pylint: disable=protected-access
+        with self._fpdf._disable_writing():
+            for j in range(len(row.cells)):
+                page_break, height = self._render_table_cell(
                     i,
                     j,
-                    cell_line_height=self._line_height,
                     row_height=self._line_height,
-                    lines_heights_only=True,
                 )
-            )
-        return lines_heights
+                any_page_break = any_page_break or page_break
+                heights_per_cell.append(height)
+        row_height = (
+            max(height for height in heights_per_cell) if heights_per_cell else 0
+        )
+        return RowLayoutInfo(row_height, any_page_break)
 
 
 class Row:
     "Object that `Table.row()` yields, used to build a row in a table"
 
     def __init__(self, fpdf):
         self._fpdf = fpdf
@@ -337,15 +353,15 @@
             if font_face != self.style:
                 style = font_face
         cell = Cell(text, align, style, img, img_fill_width, colspan)
         self.cells.append(cell)
         return cell
 
 
-@dataclass
+@dataclass(frozen=True)
 class Cell:
     "Internal representation of a table cell"
     __slots__ = (  # RAM usage optimization
         "text",
         "align",
         "style",
         "img",
```

### Comparing `fpdf2-2.7.3/fpdf/template.py` & `fpdf2-2.7.4/fpdf/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,15 +296,16 @@
             style += "U"
         self.splitting_pdf.set_font(element["font"], style, element["size"])
         return self.splitting_pdf.multi_cell(
             w=element["x2"] - element["x1"],
             h=element["y2"] - element["y1"],
             txt=str(text),
             align=element.get("align", ""),
-            split_only=True,
+            dry_run=True,
+            output="LINES",
         )
 
     def _text(
         self,
         *_,
         x1=0,
         y1=0,
@@ -354,15 +355,20 @@
             pdf.cell(w=width, h=height, txt=text, border=0, align=align, fill=fill)
         elif multiline:  # automatic word - warp
             pdf.multi_cell(
                 w=width, h=height, txt=text, border=0, align=align, fill=fill
             )
         else:  # trim to fit exactly the space defined
             text = pdf.multi_cell(
-                w=width, h=height, txt=text, align=align, split_only=True
+                w=width,
+                h=height,
+                txt=text,
+                align=align,
+                dry_run=True,
+                output="LINES",
             )[0]
             pdf.cell(w=width, h=height, txt=text, border=0, align=align, fill=fill)
 
     def _line(
         self,
         *_,
         x1=0,
```

### Comparing `fpdf2-2.7.3/fpdf/transitions.py` & `fpdf2-2.7.4/fpdf/transitions.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.3/fpdf/util.py` & `fpdf2-2.7.4/fpdf/util.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.3/fpdf2.egg-info/PKG-INFO` & `fpdf2-2.7.4/fpdf2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fpdf2
-Version: 2.7.3
+Version: 2.7.4
 Summary: Simple & fast PDF generation for Python
 Home-page: https://pyfpdf.github.io/fpdf2/
-Download-URL: https://github.com/PyFPDF/fpdf2/tarball/2.7.3
+Download-URL: https://github.com/PyFPDF/fpdf2/tarball/2.7.4
 Author: Olivier PLATHEY ported by Max
 Maintainer: Lucas Cimon
 License: LGPLv3+
 Project-URL: Documentation, https://pyfpdf.github.io/fpdf2/
 Project-URL: Code, https://github.com/PyFPDF/fpdf2
 Project-URL: Issue tracker, https://github.com/PyFPDF/fpdf2/issues
 Keywords: pdf,unicode,png,jpg,ttf,barcode
@@ -103,15 +103,15 @@
  * Images & links alternative descriptions, for accessibility
  * Table of contents & [document outline](https://pyfpdf.github.io/fpdf2/DocumentOutlineAndTableOfContents.html)
  * [Document encryption](https://pyfpdf.github.io/fpdf2/Encryption.html) & [document signing](https://pyfpdf.github.io/fpdf2/Signing.html)
  * [Annotations](https://pyfpdf.github.io/fpdf2/Annotations.html), including text highlights, and [file attachments](https://pyfpdf.github.io/fpdf2/FileAttachments.html)
  * [Presentation mode](https://pyfpdf.github.io/fpdf2/Presentations.html) with control over page display duration & transitions
  * Optional basic Markdown-like styling: `**bold**, __italics__`
  * Can render [mathematical equations & charts](https://pyfpdf.github.io/fpdf2/Maths.html)
- * Usage examples with [Django](https://www.djangoproject.com/), [Flask](https://flask.palletsprojects.com), [streamlit](https://streamlit.io/), AWS lambdas... : [Usage in web APIs](https://pyfpdf.github.io/fpdf2/UsageInWebAPI.html)
+ * Usage examples with [Django](https://www.djangoproject.com/), [Flask](https://flask.palletsprojects.com), [FastAPI](https://fastapi.tiangolo.com/), [streamlit](https://streamlit.io/), AWS lambdas... : [Usage in web APIs](https://pyfpdf.github.io/fpdf2/UsageInWebAPI.html)
  * 1000+ unit tests running under Linux & Windows, with `qpdf`-based PDF diffing, timing & memory usage checks, and a high code coverage
 
 Our 350+ reference PDF test files, generated by `fpdf2`, are validated using 3 different checkers:
 
 [![QPDF logo](https://pyfpdf.github.io/fpdf2/qpdf-logo.svg)](https://github.com/qpdf/qpdf)
 [![PDF Checker logo](https://pyfpdf.github.io/fpdf2/pdfchecker-logo.png)](https://www.datalogics.com/products/pdf-tools/pdf-checker/)
 [![VeraPDF logo](https://pyfpdf.github.io/fpdf2/vera-logo.jpg)](https://verapdf.org)
@@ -132,15 +132,15 @@
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-twitter-03A9F4?logo=twitter)](https://twitter.com/share?url=https://github.com/PyFPDF/fpdf2&t=fpdf2)
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-facebook-1976D2?logo=facebook)](https://www.facebook.com/sharer/sharer.php?u=https://github.com/PyFPDF/fpdf2)
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-linkedin-3949AB?logo=linkedin)](https://www.linkedin.com/shareArticle?url=https://github.com/PyFPDF/fpdf2&title=fpdf2)
 
 ## Documentation
 
 - [Documentation Home](https://pyfpdf.github.io/fpdf2/)
-- Tutorial in several languages: [English](https://pyfpdf.github.io/fpdf2/Tutorial.html) - [Deutsch](https://pyfpdf.github.io/fpdf2/Tutorial-de.html) - [español](https://pyfpdf.github.io/fpdf2/Tutorial-es.html) - [हिंदी](https://pyfpdf.github.io/fpdf2/Tutorial-हिंदी.html) - [português](https://pyfpdf.github.io/fpdf2/Tutorial-pt.html) - [Русский](https://pyfpdf.github.io/fpdf2/Tutorial-ru.html) - [Italian](https://pyfpdf.github.io/fpdf2/Tutorial-it.html) - [français](https://pyfpdf.github.io/fpdf2/Tutorial-fr.html) - [Ελληνικά](https://pyfpdf.github.io/fpdf2/Tutorial-gr.html) - [עברית](https://pyfpdf.github.io/fpdf2/Tutorial-he.html) - [简体中文](https://pyfpdf.github.io/fpdf2/Tutorial-zh.html) - [বাংলা](https://pyfpdf.github.io/fpdf2/Tutorial-বাংলা.html)
+- Tutorial in several languages: [English](https://pyfpdf.github.io/fpdf2/Tutorial.html) - [Deutsch](https://pyfpdf.github.io/fpdf2/Tutorial-de.html) - [español](https://pyfpdf.github.io/fpdf2/Tutorial-es.html) - [हिंदी](https://pyfpdf.github.io/fpdf2/Tutorial-hi.html) - [português](https://pyfpdf.github.io/fpdf2/Tutorial-pt.html) - [Русский](https://pyfpdf.github.io/fpdf2/Tutorial-ru.html) - [Italian](https://pyfpdf.github.io/fpdf2/Tutorial-it.html) - [français](https://pyfpdf.github.io/fpdf2/Tutorial-fr.html) - [Ελληνικά](https://pyfpdf.github.io/fpdf2/Tutorial-gr.html) - [עברית](https://pyfpdf.github.io/fpdf2/Tutorial-he.html) - [简体中文](https://pyfpdf.github.io/fpdf2/Tutorial-zh.html) - [বাংলা](https://pyfpdf.github.io/fpdf2/Tutorial-bn.html)
 - Release notes: [CHANGELOG.md](https://github.com/PyFPDF/fpdf2/blob/master/CHANGELOG.md)
 - A series of blog posts: [fpdf2 tag @ ludochaordic](https://chezsoi.org/lucas/blog/tag/fpdf2.html)
 
 You can also have a look at the `tests/`, they're great usage examples!
 
 ## Developement
 
@@ -238,15 +238,15 @@
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://nicholasjin.github.io/"><img src="https://avatars.githubusercontent.com/u/15252734?v=4?s=100" width="100px;" alt="Nicholas Jin"/><br /><sub><b>Nicholas Jin</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Anicholasjin" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://portfolio-yk-jp.vercel.app/"><img src="https://avatars.githubusercontent.com/u/69574727?v=4?s=100" width="100px;" alt="Yusuke"/><br /><sub><b>Yusuke</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=yk-jp" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Tillrzhtgrfho"><img src="https://avatars.githubusercontent.com/u/86628355?v=4?s=100" width="100px;" alt="Tillrzhtgrfho"/><br /><sub><b>Tillrzhtgrfho</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3ATillrzhtgrfho" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://dario.icu/"><img src="https://avatars.githubusercontent.com/u/35274810?v=4?s=100" width="100px;" alt="Dario Ackermann"/><br /><sub><b>Dario Ackermann</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Adarioackermann" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/TzviGreenfeld"><img src="https://avatars.githubusercontent.com/u/43534411?v=4?s=100" width="100px;" alt="Tzvi Greenfeld"/><br /><sub><b>Tzvi Greenfeld</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=TzviGreenfeld" title="Documentation">📖</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/devdev29"><img src="https://avatars.githubusercontent.com/u/88680035?v=4?s=100" width="100px;" alt="devdev29"/><br /><sub><b>devdev29</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=devdev29" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/devdev29"><img src="https://avatars.githubusercontent.com/u/88680035?v=4?s=100" width="100px;" alt="devdev29"/><br /><sub><b>devdev29</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=devdev29" title="Documentation">📖</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=devdev29" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Zenigata"><img src="https://avatars.githubusercontent.com/u/1022393?v=4?s=100" width="100px;" alt="Johan Bonneau"/><br /><sub><b>Johan Bonneau</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=Zenigata" title="Documentation">📖</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jmunoz94"><img src="https://avatars.githubusercontent.com/u/48921408?v=4?s=100" width="100px;" alt="Jesús Alberto Muñoz Mesa"/><br /><sub><b>Jesús Alberto Muñoz Mesa</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=jmunoz94" title="Tests">⚠️</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=jmunoz94" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://jdeep.me"><img src="https://avatars.githubusercontent.com/u/64089730?v=4?s=100" width="100px;" alt="Jaydeep Das"/><br /><sub><b>Jaydeep Das</b></sub></a><br /><a href="#question-JDeepD" title="Answering Questions">💬</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/seanpmulholland"><img src="https://avatars.githubusercontent.com/u/79894395?v=4?s=100" width="100px;" alt="Sean"/><br /><sub><b>Sean</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=seanpmulholland" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/andersonhc"><img src="https://avatars.githubusercontent.com/u/948125?v=4?s=100" width="100px;" alt="Anderson Herzogenrath da Costa"/><br /><sub><b>Anderson Herzogenrath da Costa</b></sub></a><br /><a href="#question-andersonhc" title="Answering Questions">💬</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=andersonhc" title="Code">💻</a> <a href="#research-andersonhc" title="Research">🔬</a> <a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Aandersonhc" title="Bug reports">🐛</a></td>
@@ -262,16 +262,18 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/TheNerdy907"><img src="https://avatars.githubusercontent.com/u/51904226?v=4?s=100" width="100px;" alt="TheNerdy907"/><br /><sub><b>TheNerdy907</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3ATheNerdy907" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/eroux"><img src="https://avatars.githubusercontent.com/u/60868?v=4?s=100" width="100px;" alt="Elie Roux"/><br /><sub><b>Elie Roux</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Aeroux" title="Bug reports">🐛</a> <a href="#ideas-eroux" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=eroux" title="Code">💻</a> <a href="#question-eroux" title="Answering Questions">💬</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/msalem99"><img src="https://avatars.githubusercontent.com/u/89017128?v=4?s=100" width="100px;" alt="msalem"/><br /><sub><b>msalem</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=msalem99" title="Documentation">📖</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/ruiz-manuel"><img src="https://avatars.githubusercontent.com/u/43274578?v=4?s=100" width="100px;" alt="Manuel Ruiz"/><br /><sub><b>Manuel Ruiz</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Aruiz-manuel" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/nsimonovici"><img src="https://avatars.githubusercontent.com/u/44460830?v=4?s=100" width="100px;" alt="Noel"/><br /><sub><b>Noel</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Ansimonovici" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://sites.google.com/view/iamavik/"><img src="https://avatars.githubusercontent.com/u/14172268?v=4?s=100" width="100px;" alt="Avik Sarkar"/><br /><sub><b>Avik Sarkar</b></sub></a><br /><a href="#translation-ssavi-ict" title="Translation">🌍</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=ssavi-ict" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://sites.google.com/view/iamavik/"><img src="https://avatars.githubusercontent.com/u/14172268?v=4?s=100" width="100px;" alt="Avik Sarkar"/><br /><sub><b>Avik Sarkar</b></sub></a><br /><a href="#translation-ssavi-ict" title="Translation">🌍</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=ssavi-ict" title="Documentation">📖</a> <a href="#question-ssavi-ict" title="Answering Questions">💬</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/aeris07"><img src="https://avatars.githubusercontent.com/u/129675592?v=4?s=100" width="100px;" alt="aeris07"/><br /><sub><b>aeris07</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Aaeris07" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/KamarulAdha"><img src="https://avatars.githubusercontent.com/u/52944294?v=4?s=100" width="100px;" alt="KamarulAdha"/><br /><sub><b>KamarulAdha</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=KamarulAdha" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Valerus5685"><img src="https://avatars.githubusercontent.com/u/7953869?v=4?s=100" width="100px;" alt="Valerus5685"/><br /><sub><b>Valerus5685</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3AValerus5685" title="Bug reports">🐛</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `fpdf2-2.7.3/fpdf2.egg-info/SOURCES.txt` & `fpdf2-2.7.4/fpdf2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.3/setup.py` & `fpdf2-2.7.4/setup.py`

 * *Files identical despite different names*

