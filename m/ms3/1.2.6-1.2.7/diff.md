# Comparing `tmp/ms3-1.2.6.tar.gz` & `tmp/ms3-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms3-1.2.6.tar", last modified: Wed Apr 26 16:49:09 2023, max compression
+gzip compressed data, was "ms3-1.2.7.tar", last modified: Fri Apr 28 13:53:30 2023, max compression
```

## Comparing `ms3-1.2.6.tar` & `ms3-1.2.7.tar`

### file list

```diff
@@ -1,317 +1,317 @@
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.755867 ms3-1.2.6/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      586 2020-05-03 17:52:04.000000 ms3-1.2.6/.coveragerc
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.532530 ms3-1.2.6/.github/
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.542530 ms3-1.2.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      752 2023-03-18 08:04:35.000000 ms3-1.2.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      599 2023-03-18 08:04:35.000000 ms3-1.2.6/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.542530 ms3-1.2.6/.github/workflows/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      669 2023-01-28 14:33:36.000000 ms3-1.2.6/.github/workflows/draft-pdf.yml
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      541 2023-03-23 18:04:33.000000 ms3-1.2.6/.gitignore
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       90 2020-07-06 00:26:02.000000 ms3-1.2.6/AUTHORS.rst
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    23034 2023-04-26 16:46:43.000000 ms3-1.2.6/CHANGELOG.rst
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    34500 2020-05-07 11:55:51.000000 ms3-1.2.6/LICENSE.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4564 2023-04-26 16:49:09.755867 ms3-1.2.6/PKG-INFO
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4026 2023-03-21 14:17:58.000000 ms3-1.2.6/README.rst
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2094 2022-12-15 11:35:36.000000 ms3-1.2.6/codemeta.json
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.552531 ms3-1.2.6/docs/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)        0 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/.nojekyll
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7593 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/Makefile
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      201 2023-01-28 14:33:36.000000 ms3-1.2.6/docs/README.md
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.555864 ms3-1.2.6/docs/_intersphinx/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      646 2021-10-20 14:43:53.000000 ms3-1.2.6/docs/_intersphinx/bs4_objects.inv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1799 2021-10-20 14:43:53.000000 ms3-1.2.6/docs/_intersphinx/bs4_objects.txt
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.555864 ms3-1.2.6/docs/_static/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       18 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/_static/.gitignore
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       41 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/authors.rst
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.555864 ms3-1.2.6/docs/build/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      230 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/build/.buildinfo
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.579198 ms3-1.2.6/docs/build/.doctrees/
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.579198 ms3-1.2.6/docs/build/.doctrees/api/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2579 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/build/.doctrees/api/modules.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   619252 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/build/.doctrees/api/ms3.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3406 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/build/.doctrees/authors.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6354 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/build/.doctrees/changelog.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001) 10423401 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/build/.doctrees/environment.pickle
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14745 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/build/.doctrees/index.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7547 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/build/.doctrees/install.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4679 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/build/.doctrees/intro.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    96686 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/build/.doctrees/license.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    35413 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/build/.doctrees/manual.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4590 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/build/.doctrees/quick.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)        0 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/build/.nojekyll
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.605865 ms3-1.2.6/docs/build/doctrees/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4366 2023-03-23 18:04:33.000000 ms3-1.2.6/docs/build/doctrees/README.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3594 2023-03-23 18:04:33.000000 ms3-1.2.6/docs/build/doctrees/authors.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   154262 2023-03-23 18:04:33.000000 ms3-1.2.6/docs/build/doctrees/changelog.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001) 13487965 2023-03-23 18:04:33.000000 ms3-1.2.6/docs/build/doctrees/environment.pickle
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    35248 2023-03-23 18:04:33.000000 ms3-1.2.6/docs/build/doctrees/index.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7812 2023-03-23 18:04:33.000000 ms3-1.2.6/docs/build/doctrees/install.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    97335 2023-03-23 18:04:33.000000 ms3-1.2.6/docs/build/doctrees/license.doctree
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.629198 ms3-1.2.6/docs/build/doctrees/manual/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001) 14283956 2023-03-23 18:04:33.000000 ms3-1.2.6/docs/build/doctrees/manual/index.doctree
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.649199 ms3-1.2.6/docs/build/doctrees/old_src/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    79212 2023-03-23 18:04:33.000000 ms3-1.2.6/docs/build/doctrees/old_src/quick_old.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    78946 2023-03-23 18:04:33.000000 ms3-1.2.6/docs/build/doctrees/quick.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001) 17416423 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/doctrees/reference.doctree
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.655866 ms3-1.2.6/docs/build/html/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      230 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/.buildinfo
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)        0 2023-03-18 10:45:36.000000 ms3-1.2.6/docs/build/html/.nojekyll
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15846 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/README.html
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.659199 ms3-1.2.6/docs/build/html/_modules/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15440 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_modules/index.html
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.669199 ms3-1.2.6/docs/build/html/_modules/ms3/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   121982 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_modules/ms3/annotations.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   562760 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_modules/ms3/bs4_parser.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   585871 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_modules/ms3/corpus.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   119721 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_modules/ms3/expand_dcml.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   299877 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_modules/ms3/parse.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   337630 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_modules/ms3/piece.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   326103 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_modules/ms3/score.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   264338 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_modules/ms3/transformations.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   930043 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_modules/ms3/utils.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   139939 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_modules/ms3/view.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    63215 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_modules/re.html
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.672532 ms3-1.2.6/docs/build/html/_sources/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      201 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_sources/README.md.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       41 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/build/html/_sources/authors.rst.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       43 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/build/html/_sources/changelog.rst.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1356 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_sources/index.rst.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1256 2023-01-28 14:33:36.000000 ms3-1.2.6/docs/build/html/_sources/install.rst.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       67 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/build/html/_sources/license.rst.txt
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.672532 ms3-1.2.6/docs/build/html/_sources/manual/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    76626 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_sources/manual/index.md.txt
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.672532 ms3-1.2.6/docs/build/html/_sources/old_src/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    17232 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_sources/old_src/quick_old.rst.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2619 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_sources/quick.md.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7126 2023-03-21 14:17:58.000000 ms3-1.2.6/docs/build/html/_sources/reference.rst.txt
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.675866 ms3-1.2.6/docs/build/html/_static/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4418 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14621 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/basic.css
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4472 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/doctools.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      439 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/documentation_options.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      286 2023-01-21 10:04:25.000000 ms3-1.2.6/docs/build/html/_static/file.png
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   288580 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/jquery-3.6.0.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    89501 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/jquery.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3019 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/jupyter-sphinx.css
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4758 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/language_data.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       90 2023-01-21 10:04:25.000000 ms3-1.2.6/docs/build/html/_static/minus.png
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    39364 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       90 2023-01-21 10:04:25.000000 ms3-1.2.6/docs/build/html/_static/plus.png
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14668 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/pygments.css
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.679199 ms3-1.2.6/docs/build/html/_static/scripts/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    86398 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/scripts/bootstrap.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     5229 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/scripts/pydata-sphinx-theme.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    18215 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/searchtools.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4712 2023-01-21 10:04:25.000000 ms3-1.2.6/docs/build/html/_static/sphinx_highlight.js
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.679199 ms3-1.2.6/docs/build/html/_static/styles/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   144661 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/styles/bootstrap.css
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    58614 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/styles/pydata-sphinx-theme.css
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      106 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/styles/theme.css
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    68420 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    19530 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/underscore.js
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.535864 ms3-1.2.6/docs/build/html/_static/vendor/
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.535864 ms3-1.2.6/docs/build/html/_static/vendor/fontawesome/
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.679199 ms3-1.2.6/docs/build/html/_static/vendor/fontawesome/6.1.2/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7427 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.679199 ms3-1.2.6/docs/build/html/_static/vendor/fontawesome/6.1.2/css/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   101709 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.682533 ms3-1.2.6/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   181264 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   105112 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    60236 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    24028 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   389948 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   154840 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    10084 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4776 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1845 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/_static/webpack-macros.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    16465 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/authors.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    69269 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/changelog.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    79722 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/genindex.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    31724 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/index.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    19975 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/install.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    53099 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/license.html
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.682533 ms3-1.2.6/docs/build/html/manual/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   338361 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/manual/index.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7352 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/objects.inv
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.685866 ms3-1.2.6/docs/build/html/old_src/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    60388 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/old_src/quick_old.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    17021 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/py-modindex.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    47347 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/quick.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)  1763633 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/reference.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15656 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/search.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   130526 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/html/searchindex.js
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.685866 ms3-1.2.6/docs/build/jupyter_execute/
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.685866 ms3-1.2.6/docs/build/jupyter_execute/manual/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   346220 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/jupyter_execute/manual/index.ipynb
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    49220 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/build/jupyter_execute/quick.ipynb
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       43 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/changelog.rst
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      135 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/columns.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    10588 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/conf.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   137117 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/cujus.mscx
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.689199 ms3-1.2.6/docs/examples/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      134 2023-01-02 20:31:46.000000 ms3-1.2.6/docs/examples/access_score_info.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       47 2021-10-16 12:40:03.000000 ms3-1.2.6/docs/examples/parse_directory.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       64 2023-01-02 20:31:46.000000 ms3-1.2.6/docs/examples/parse_directory_mscx.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       58 2023-01-02 20:31:46.000000 ms3-1.2.6/docs/examples/parse_directory_xml.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      199 2023-01-02 20:31:46.000000 ms3-1.2.6/docs/examples/parse_key.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      173 2023-01-02 20:31:46.000000 ms3-1.2.6/docs/examples/parse_other_directory.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      120 2023-01-02 20:31:46.000000 ms3-1.2.6/docs/examples/parse_single_score.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       71 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/index.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1356 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/index.rst
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1256 2023-01-28 14:33:36.000000 ms3-1.2.6/docs/install.rst
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       67 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/license.rst
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.689199 ms3-1.2.6/docs/manual/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      715 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/manual/corpus_after
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      174 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/manual/corpus_before
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    76626 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/manual/index.md
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      488 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/manual/out
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     9940 2021-10-20 14:43:53.000000 ms3-1.2.6/docs/ms3_architecture.drawio
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   218314 2021-10-20 14:43:53.000000 ms3-1.2.6/docs/ms3_architecture.png
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    96827 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/o_quam.mscx
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.689199 ms3-1.2.6/docs/old_src/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15949 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/old_src/quick_old.md
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    17232 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/old_src/quick_old.rst
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   163542 2020-11-02 16:20:48.000000 ms3-1.2.6/docs/quae.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2619 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/quick.md
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7126 2023-03-21 14:17:58.000000 ms3-1.2.6/docs/reference.rst
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       86 2023-03-23 18:04:34.000000 ms3-1.2.6/docs/requirements.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   115684 2021-10-20 14:43:53.000000 ms3-1.2.6/docs/stabat.mscx
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.692533 ms3-1.2.6/new_tests/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7378 2023-04-26 16:41:43.000000 ms3-1.2.6/new_tests/conftest.py
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.535864 ms3-1.2.6/new_tests/inferred_labels/
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.692533 ms3-1.2.6/new_tests/inferred_labels/sweelinck_keyboard/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    19047 2022-12-15 11:35:36.000000 ms3-1.2.6/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   332296 2022-12-15 11:35:36.000000 ms3-1.2.6/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica_results.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   317949 2022-12-15 11:35:36.000000 ms3-1.2.6/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica_results_midi.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      466 2023-01-02 20:31:46.000000 ms3-1.2.6/new_tests/parse_script.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1526 2023-04-26 16:40:54.000000 ms3-1.2.6/new_tests/test_cli.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      403 2023-01-02 20:31:46.000000 ms3-1.2.6/new_tests/test_docs_examples.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    12424 2023-01-02 20:31:46.000000 ms3-1.2.6/new_tests/test_extract.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6352 2023-01-02 20:31:46.000000 ms3-1.2.6/new_tests/test_parse.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3744 2023-01-02 20:31:46.000000 ms3-1.2.6/new_tests/test_score.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      823 2023-01-17 21:52:55.000000 ms3-1.2.6/new_tests/test_transformations.py
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.722533 ms3-1.2.6/old_tests/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   388689 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/05_symph_fant_events.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      959 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/05_symph_fant_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   100539 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/05_symph_fant_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   488895 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/76CASM34A33UM_events.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7268 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/76CASM34A33UM_labels.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2636 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/76CASM34A33UM_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   155973 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/76CASM34A33UM_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4361 2023-01-02 20:31:46.000000 ms3-1.2.6/old_tests/ALL_WARNINGS
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   256806 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/BWV_0815_events.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6833 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/BWV_0815_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   136433 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/BWV_0815_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    16417 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/D973deutscher01_events.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      697 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/D973deutscher01_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     8271 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/D973deutscher01_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)  1490215 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/Did03M-Son_regina-1762-Sarti_events.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7264 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/Did03M-Son_regina-1762-Sarti_labels.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3305 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/Did03M-Son_regina-1762-Sarti_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   317634 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/Did03M-Son_regina-1762-Sarti_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      330 2023-01-02 20:31:46.000000 ms3-1.2.6/old_tests/IGNORED_WARNINGS
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   431522 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/K281-3_events.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14480 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/K281-3_labels.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4560 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/K281-3_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    96112 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/K281-3_notes.tsv
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.729200 ms3-1.2.6/old_tests/MS3/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)  1041665 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/MS3/05_symph_fant.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)  1034028 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/MS3/76CASM34A33UM.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   787637 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/MS3/BWV_0815.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    54002 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/MS3/D973deutscher01.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   701525 2023-03-23 18:04:34.000000 ms3-1.2.6/old_tests/MS3/Did03M-Son_regina-1762-Sarti.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   807371 2023-03-23 18:04:34.000000 ms3-1.2.6/old_tests/MS3/K281-3.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   259369 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/MS3/stabat_03_coloured.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      624 2023-03-23 18:04:34.000000 ms3-1.2.6/old_tests/README.md
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      224 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/conftest.py
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.732533 ms3-1.2.6/old_tests/harmonies/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2524 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/harmonies/76CASM34A33UM.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     9855 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/harmonies/Did03M-Son_regina-1762-Sarti.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    21459 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/harmonies/K281-3.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3905 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/harmonies/stabat_03_coloured.tsv
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.732533 ms3-1.2.6/old_tests/measures/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      889 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/measures/05_symph_fant.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2524 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/measures/76CASM34A33UM.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6504 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/measures/BWV_0815.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      684 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/measures/D973deutscher01.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2706 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/measures/Did03M-Son_regina-1762-Sarti.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4411 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/measures/K281-3.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      790 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/measures/stabat_03_coloured.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     5885 2023-03-23 18:04:34.000000 ms3-1.2.6/old_tests/metadata.tsv
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.739200 ms3-1.2.6/old_tests/notes/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    74055 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/notes/05_symph_fant.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   112389 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/notes/76CASM34A33UM.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   102317 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/notes/BWV_0815.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6173 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/notes/D973deutscher01.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   230316 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/notes/Did03M-Son_regina-1762-Sarti.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    70952 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/notes/K281-3.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    25080 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/notes/stabat_03_coloured.tsv
--rwxr-xr-x   0 hentsche  (1001) hentsche  (1001)       45 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/parse_original.sh
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      750 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/paths1.json
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      844 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/paths2.json
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.739200 ms3-1.2.6/old_tests/repeat_dummies/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6909 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/repeat_dummies/repeats0.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6493 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/repeat_dummies/repeats1.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7376 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/repeat_dummies/repeats2.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   135170 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/stabat_03_coloured_events.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4822 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/stabat_03_coloured_labels.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      790 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/stabat_03_coloured_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    25080 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/stabat_03_coloured_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2207 2023-02-18 19:40:30.000000 ms3-1.2.6/old_tests/test_parse.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      712 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/test_repeats.py
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.745867 ms3-1.2.6/old_tests/test_results/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      921 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/test_results/05_symph_fant_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    98388 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/test_results/05_symph_fant_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7089 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/test_results/76CASM34A33UM_labels.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2536 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/test_results/76CASM34A33UM_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   152525 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/test_results/76CASM34A33UM_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6833 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/test_results/BWV_0815_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   136433 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/test_results/BWV_0815_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      697 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/test_results/D973deutscher01_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     8271 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/test_results/D973deutscher01_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7264 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/test_results/Did03M-Son_regina-1762-Sarti_labels.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3305 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/test_results/Did03M-Son_regina-1762-Sarti_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   317634 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/test_results/Did03M-Son_regina-1762-Sarti_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14099 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/test_results/K281-3_labels.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4391 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/test_results/K281-3_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    94030 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/test_results/K281-3_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4731 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/test_results/stabat_03_coloured_labels.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      758 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/test_results/stabat_03_coloured_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    24478 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/test_results/stabat_03_coloured_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4777 2022-12-15 11:35:36.000000 ms3-1.2.6/old_tests/test_score.py
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.745867 ms3-1.2.6/paper/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    17950 2023-03-21 14:17:58.000000 ms3-1.2.6/paper/paper.bib
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4605 2023-03-21 14:17:58.000000 ms3-1.2.6/paper/paper.md
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   200690 2023-01-28 14:33:36.000000 ms3-1.2.6/paper/paper.pdf
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1364 2023-04-26 16:49:09.755867 ms3-1.2.6/setup.cfg
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      567 2020-05-03 17:52:04.000000 ms3-1.2.6/setup.py
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.749200 ms3-1.2.6/src/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)        0 2020-11-02 16:27:59.000000 ms3-1.2.6/src/__init__.py
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.752534 ms3-1.2.6/src/ms3/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1006 2023-02-18 19:40:30.000000 ms3-1.2.6/src/ms3/__init__.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2402 2023-02-18 19:40:30.000000 ms3-1.2.6/src/ms3/_typing.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    24943 2023-01-12 10:36:52.000000 ms3-1.2.6/src/ms3/annotations.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    41608 2023-03-23 18:04:34.000000 ms3-1.2.6/src/ms3/bs4_measures.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   130482 2023-04-26 16:41:43.000000 ms3-1.2.6/src/ms3/bs4_parser.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    41131 2023-04-26 16:41:43.000000 ms3-1.2.6/src/ms3/cli.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   151734 2023-04-19 06:50:23.000000 ms3-1.2.6/src/ms3/corpus.py
--rwxr-xr-x   0 hentsche  (1001) hentsche  (1001)    26692 2023-01-02 20:31:46.000000 ms3-1.2.6/src/ms3/expand_dcml.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     8416 2023-01-02 20:31:46.000000 ms3-1.2.6/src/ms3/ferocious_names.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    18415 2023-03-18 08:04:35.000000 ms3-1.2.6/src/ms3/logger.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15667 2023-04-26 16:41:43.000000 ms3-1.2.6/src/ms3/operations.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    83765 2023-04-26 16:41:43.000000 ms3-1.2.6/src/ms3/parse.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    82901 2023-03-23 18:04:34.000000 ms3-1.2.6/src/ms3/piece.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    97681 2023-03-23 18:04:34.000000 ms3-1.2.6/src/ms3/score.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    67393 2023-03-23 18:04:34.000000 ms3-1.2.6/src/ms3/transformations.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   219691 2023-04-26 16:41:43.000000 ms3-1.2.6/src/ms3/utils.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    29853 2023-04-26 16:41:43.000000 ms3-1.2.6/src/ms3/view.py
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-26 16:49:09.755867 ms3-1.2.6/src/ms3.egg-info/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4564 2023-04-26 16:49:09.000000 ms3-1.2.6/src/ms3.egg-info/PKG-INFO
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     9420 2023-04-26 16:49:09.000000 ms3-1.2.6/src/ms3.egg-info/SOURCES.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)        1 2023-04-26 16:49:09.000000 ms3-1.2.6/src/ms3.egg-info/dependency_links.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       36 2023-04-26 16:49:09.000000 ms3-1.2.6/src/ms3.egg-info/entry_points.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)        1 2020-05-03 17:52:26.000000 ms3-1.2.6/src/ms3.egg-info/not-zip-safe
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      120 2023-04-26 16:49:09.000000 ms3-1.2.6/src/ms3.egg-info/requires.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)        4 2023-04-26 16:49:09.000000 ms3-1.2.6/src/ms3.egg-info/top_level.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      318 2020-05-03 17:52:04.000000 ms3-1.2.6/tox.ini
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.185244 ms3-1.2.7/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      586 2020-05-03 17:52:04.000000 ms3-1.2.7/.coveragerc
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.091909 ms3-1.2.7/.github/
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.095243 ms3-1.2.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      752 2023-03-18 08:04:35.000000 ms3-1.2.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      599 2023-03-18 08:04:35.000000 ms3-1.2.7/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.095243 ms3-1.2.7/.github/workflows/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      669 2023-01-28 14:33:36.000000 ms3-1.2.7/.github/workflows/draft-pdf.yml
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      541 2023-03-23 18:04:33.000000 ms3-1.2.7/.gitignore
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       90 2020-07-06 00:26:02.000000 ms3-1.2.7/AUTHORS.rst
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    23156 2023-04-28 13:53:00.000000 ms3-1.2.7/CHANGELOG.rst
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    34500 2020-05-07 11:55:51.000000 ms3-1.2.7/LICENSE.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4564 2023-04-28 13:53:30.185244 ms3-1.2.7/PKG-INFO
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4026 2023-03-21 14:17:58.000000 ms3-1.2.7/README.rst
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2094 2022-12-15 11:35:36.000000 ms3-1.2.7/codemeta.json
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.098576 ms3-1.2.7/docs/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)        0 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/.nojekyll
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7593 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/Makefile
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      201 2023-01-28 14:33:36.000000 ms3-1.2.7/docs/README.md
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.098576 ms3-1.2.7/docs/_intersphinx/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      646 2021-10-20 14:43:53.000000 ms3-1.2.7/docs/_intersphinx/bs4_objects.inv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1799 2021-10-20 14:43:53.000000 ms3-1.2.7/docs/_intersphinx/bs4_objects.txt
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.098576 ms3-1.2.7/docs/_static/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       18 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/_static/.gitignore
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       41 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/authors.rst
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.098576 ms3-1.2.7/docs/build/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      230 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.buildinfo
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.108576 ms3-1.2.7/docs/build/.doctrees/
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.108576 ms3-1.2.7/docs/build/.doctrees/api/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2579 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.doctrees/api/modules.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   619252 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.doctrees/api/ms3.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3406 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.doctrees/authors.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6354 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.doctrees/changelog.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001) 10423401 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.doctrees/environment.pickle
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14745 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.doctrees/index.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7547 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.doctrees/install.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4679 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.doctrees/intro.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    96686 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.doctrees/license.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    35413 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.doctrees/manual.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4590 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.doctrees/quick.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)        0 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.nojekyll
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.121910 ms3-1.2.7/docs/build/doctrees/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4366 2023-03-23 18:04:33.000000 ms3-1.2.7/docs/build/doctrees/README.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3594 2023-03-23 18:04:33.000000 ms3-1.2.7/docs/build/doctrees/authors.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   154262 2023-03-23 18:04:33.000000 ms3-1.2.7/docs/build/doctrees/changelog.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001) 13487965 2023-03-23 18:04:33.000000 ms3-1.2.7/docs/build/doctrees/environment.pickle
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    35248 2023-03-23 18:04:33.000000 ms3-1.2.7/docs/build/doctrees/index.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7812 2023-03-23 18:04:33.000000 ms3-1.2.7/docs/build/doctrees/install.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    97335 2023-03-23 18:04:33.000000 ms3-1.2.7/docs/build/doctrees/license.doctree
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.135243 ms3-1.2.7/docs/build/doctrees/manual/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001) 14283956 2023-03-23 18:04:33.000000 ms3-1.2.7/docs/build/doctrees/manual/index.doctree
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.145243 ms3-1.2.7/docs/build/doctrees/old_src/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    79212 2023-03-23 18:04:33.000000 ms3-1.2.7/docs/build/doctrees/old_src/quick_old.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    78946 2023-03-23 18:04:33.000000 ms3-1.2.7/docs/build/doctrees/quick.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001) 17416423 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/doctrees/reference.doctree
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.148577 ms3-1.2.7/docs/build/html/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      230 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/.buildinfo
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)        0 2023-03-18 10:45:36.000000 ms3-1.2.7/docs/build/html/.nojekyll
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15846 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/README.html
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.148577 ms3-1.2.7/docs/build/html/_modules/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15440 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_modules/index.html
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.151910 ms3-1.2.7/docs/build/html/_modules/ms3/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   121982 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_modules/ms3/annotations.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   562760 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_modules/ms3/bs4_parser.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   585871 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_modules/ms3/corpus.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   119721 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_modules/ms3/expand_dcml.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   299877 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_modules/ms3/parse.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   337630 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_modules/ms3/piece.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   326103 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_modules/ms3/score.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   264338 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_modules/ms3/transformations.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   930043 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_modules/ms3/utils.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   139939 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_modules/ms3/view.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    63215 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_modules/re.html
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.155243 ms3-1.2.7/docs/build/html/_sources/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      201 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_sources/README.md.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       41 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/html/_sources/authors.rst.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       43 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/html/_sources/changelog.rst.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1356 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1256 2023-01-28 14:33:36.000000 ms3-1.2.7/docs/build/html/_sources/install.rst.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       67 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/html/_sources/license.rst.txt
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.155243 ms3-1.2.7/docs/build/html/_sources/manual/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    76626 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_sources/manual/index.md.txt
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.155243 ms3-1.2.7/docs/build/html/_sources/old_src/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    17232 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_sources/old_src/quick_old.rst.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2619 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_sources/quick.md.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7126 2023-03-21 14:17:58.000000 ms3-1.2.7/docs/build/html/_sources/reference.rst.txt
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.158577 ms3-1.2.7/docs/build/html/_static/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4418 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14621 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/basic.css
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4472 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/doctools.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      439 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      286 2023-01-21 10:04:25.000000 ms3-1.2.7/docs/build/html/_static/file.png
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   288580 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/jquery-3.6.0.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    89501 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/jquery.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3019 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/jupyter-sphinx.css
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4758 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/language_data.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       90 2023-01-21 10:04:25.000000 ms3-1.2.7/docs/build/html/_static/minus.png
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    39364 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       90 2023-01-21 10:04:25.000000 ms3-1.2.7/docs/build/html/_static/plus.png
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14668 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/pygments.css
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.158577 ms3-1.2.7/docs/build/html/_static/scripts/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    86398 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/scripts/bootstrap.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     5229 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/scripts/pydata-sphinx-theme.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    18215 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/searchtools.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4712 2023-01-21 10:04:25.000000 ms3-1.2.7/docs/build/html/_static/sphinx_highlight.js
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.158577 ms3-1.2.7/docs/build/html/_static/styles/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   144661 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/styles/bootstrap.css
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    58614 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/styles/pydata-sphinx-theme.css
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      106 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/styles/theme.css
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    68420 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    19530 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/underscore.js
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.091909 ms3-1.2.7/docs/build/html/_static/vendor/
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.091909 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.158577 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7427 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.158577 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/css/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   101709 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.158577 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   181264 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   105112 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    60236 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    24028 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   389948 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   154840 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    10084 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4776 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1845 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/webpack-macros.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    16465 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/authors.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    69269 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/changelog.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    79722 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/genindex.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    31724 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/index.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    19975 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/install.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    53099 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/license.html
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.158577 ms3-1.2.7/docs/build/html/manual/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   338361 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/manual/index.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7352 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/objects.inv
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.161910 ms3-1.2.7/docs/build/html/old_src/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    60388 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/old_src/quick_old.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    17021 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/py-modindex.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    47347 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/quick.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)  1763633 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/reference.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15656 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/search.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   130526 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/searchindex.js
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.161910 ms3-1.2.7/docs/build/jupyter_execute/
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.161910 ms3-1.2.7/docs/build/jupyter_execute/manual/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   346220 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/jupyter_execute/manual/index.ipynb
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    49220 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/jupyter_execute/quick.ipynb
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       43 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/changelog.rst
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      135 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/columns.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    10588 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/conf.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   137117 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/cujus.mscx
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.161910 ms3-1.2.7/docs/examples/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      134 2023-01-02 20:31:46.000000 ms3-1.2.7/docs/examples/access_score_info.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       47 2021-10-16 12:40:03.000000 ms3-1.2.7/docs/examples/parse_directory.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       64 2023-01-02 20:31:46.000000 ms3-1.2.7/docs/examples/parse_directory_mscx.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       58 2023-01-02 20:31:46.000000 ms3-1.2.7/docs/examples/parse_directory_xml.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      199 2023-01-02 20:31:46.000000 ms3-1.2.7/docs/examples/parse_key.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      173 2023-01-02 20:31:46.000000 ms3-1.2.7/docs/examples/parse_other_directory.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      120 2023-01-02 20:31:46.000000 ms3-1.2.7/docs/examples/parse_single_score.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       71 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/index.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1356 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/index.rst
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1256 2023-01-28 14:33:36.000000 ms3-1.2.7/docs/install.rst
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       67 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/license.rst
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.161910 ms3-1.2.7/docs/manual/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      715 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/manual/corpus_after
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      174 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/manual/corpus_before
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    76626 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/manual/index.md
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      488 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/manual/out
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     9940 2021-10-20 14:43:53.000000 ms3-1.2.7/docs/ms3_architecture.drawio
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   218314 2021-10-20 14:43:53.000000 ms3-1.2.7/docs/ms3_architecture.png
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    96827 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/o_quam.mscx
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.161910 ms3-1.2.7/docs/old_src/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15949 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/old_src/quick_old.md
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    17232 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/old_src/quick_old.rst
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   163542 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/quae.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2619 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/quick.md
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7126 2023-03-21 14:17:58.000000 ms3-1.2.7/docs/reference.rst
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       86 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/requirements.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   115684 2021-10-20 14:43:53.000000 ms3-1.2.7/docs/stabat.mscx
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.161910 ms3-1.2.7/new_tests/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7378 2023-04-28 13:53:19.000000 ms3-1.2.7/new_tests/conftest.py
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.095243 ms3-1.2.7/new_tests/inferred_labels/
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.165243 ms3-1.2.7/new_tests/inferred_labels/sweelinck_keyboard/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    19047 2022-12-15 11:35:36.000000 ms3-1.2.7/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   332296 2022-12-15 11:35:36.000000 ms3-1.2.7/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica_results.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   317949 2022-12-15 11:35:36.000000 ms3-1.2.7/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica_results_midi.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      466 2023-01-02 20:31:46.000000 ms3-1.2.7/new_tests/parse_script.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3019 2023-04-28 13:53:00.000000 ms3-1.2.7/new_tests/test_cli.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      403 2023-01-02 20:31:46.000000 ms3-1.2.7/new_tests/test_docs_examples.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    12424 2023-01-02 20:31:46.000000 ms3-1.2.7/new_tests/test_extract.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6352 2023-01-02 20:31:46.000000 ms3-1.2.7/new_tests/test_parse.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3744 2023-01-02 20:31:46.000000 ms3-1.2.7/new_tests/test_score.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      823 2023-01-17 21:52:55.000000 ms3-1.2.7/new_tests/test_transformations.py
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.171910 ms3-1.2.7/old_tests/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   388689 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/05_symph_fant_events.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      959 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/05_symph_fant_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   100539 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/05_symph_fant_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   488895 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/76CASM34A33UM_events.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7268 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/76CASM34A33UM_labels.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2636 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/76CASM34A33UM_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   155973 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/76CASM34A33UM_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4361 2023-01-02 20:31:46.000000 ms3-1.2.7/old_tests/ALL_WARNINGS
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   256806 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/BWV_0815_events.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6833 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/BWV_0815_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   136433 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/BWV_0815_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    16417 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/D973deutscher01_events.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      697 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/D973deutscher01_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     8271 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/D973deutscher01_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)  1490215 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/Did03M-Son_regina-1762-Sarti_events.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7264 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/Did03M-Son_regina-1762-Sarti_labels.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3305 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/Did03M-Son_regina-1762-Sarti_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   317634 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/Did03M-Son_regina-1762-Sarti_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      330 2023-01-02 20:31:46.000000 ms3-1.2.7/old_tests/IGNORED_WARNINGS
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   431522 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/K281-3_events.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14480 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/K281-3_labels.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4560 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/K281-3_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    96112 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/K281-3_notes.tsv
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.175244 ms3-1.2.7/old_tests/MS3/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)  1041665 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/MS3/05_symph_fant.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)  1034028 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/MS3/76CASM34A33UM.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   787637 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/MS3/BWV_0815.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    54002 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/MS3/D973deutscher01.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   701525 2023-03-23 18:04:34.000000 ms3-1.2.7/old_tests/MS3/Did03M-Son_regina-1762-Sarti.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   807371 2023-03-23 18:04:34.000000 ms3-1.2.7/old_tests/MS3/K281-3.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   259369 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/MS3/stabat_03_coloured.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      624 2023-03-23 18:04:34.000000 ms3-1.2.7/old_tests/README.md
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      224 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/conftest.py
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.175244 ms3-1.2.7/old_tests/harmonies/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2524 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/harmonies/76CASM34A33UM.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     9855 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/harmonies/Did03M-Son_regina-1762-Sarti.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    21459 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/harmonies/K281-3.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3905 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/harmonies/stabat_03_coloured.tsv
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.178577 ms3-1.2.7/old_tests/measures/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      889 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/measures/05_symph_fant.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2524 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/measures/76CASM34A33UM.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6504 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/measures/BWV_0815.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      684 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/measures/D973deutscher01.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2706 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/measures/Did03M-Son_regina-1762-Sarti.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4411 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/measures/K281-3.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      790 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/measures/stabat_03_coloured.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     5885 2023-03-23 18:04:34.000000 ms3-1.2.7/old_tests/metadata.tsv
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.178577 ms3-1.2.7/old_tests/notes/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    74055 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/notes/05_symph_fant.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   112389 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/notes/76CASM34A33UM.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   102317 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/notes/BWV_0815.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6173 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/notes/D973deutscher01.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   230316 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/notes/Did03M-Son_regina-1762-Sarti.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    70952 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/notes/K281-3.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    25080 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/notes/stabat_03_coloured.tsv
+-rwxr-xr-x   0 hentsche  (1001) hentsche  (1001)       45 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/parse_original.sh
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      750 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/paths1.json
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      844 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/paths2.json
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.178577 ms3-1.2.7/old_tests/repeat_dummies/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6909 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/repeat_dummies/repeats0.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6493 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/repeat_dummies/repeats1.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7376 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/repeat_dummies/repeats2.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   135170 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/stabat_03_coloured_events.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4822 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/stabat_03_coloured_labels.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      790 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/stabat_03_coloured_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    25080 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/stabat_03_coloured_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2207 2023-02-18 19:40:30.000000 ms3-1.2.7/old_tests/test_parse.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      712 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_repeats.py
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.181911 ms3-1.2.7/old_tests/test_results/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      921 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/05_symph_fant_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    98388 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/05_symph_fant_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7089 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/76CASM34A33UM_labels.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2536 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/76CASM34A33UM_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   152525 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/76CASM34A33UM_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6833 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/BWV_0815_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   136433 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/BWV_0815_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      697 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/D973deutscher01_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     8271 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/D973deutscher01_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7264 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/Did03M-Son_regina-1762-Sarti_labels.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3305 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/Did03M-Son_regina-1762-Sarti_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   317634 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/Did03M-Son_regina-1762-Sarti_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14099 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/K281-3_labels.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4391 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/K281-3_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    94030 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/K281-3_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4731 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/stabat_03_coloured_labels.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      758 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/stabat_03_coloured_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    24478 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/stabat_03_coloured_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4777 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_score.py
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.181911 ms3-1.2.7/paper/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    17950 2023-03-21 14:17:58.000000 ms3-1.2.7/paper/paper.bib
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4605 2023-03-21 14:17:58.000000 ms3-1.2.7/paper/paper.md
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   200690 2023-01-28 14:33:36.000000 ms3-1.2.7/paper/paper.pdf
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1364 2023-04-28 13:53:30.188577 ms3-1.2.7/setup.cfg
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      567 2020-05-03 17:52:04.000000 ms3-1.2.7/setup.py
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.181911 ms3-1.2.7/src/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)        0 2020-11-02 16:27:59.000000 ms3-1.2.7/src/__init__.py
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.185244 ms3-1.2.7/src/ms3/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1006 2023-02-18 19:40:30.000000 ms3-1.2.7/src/ms3/__init__.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2402 2023-02-18 19:40:30.000000 ms3-1.2.7/src/ms3/_typing.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    24943 2023-01-12 10:36:52.000000 ms3-1.2.7/src/ms3/annotations.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    41608 2023-03-23 18:04:34.000000 ms3-1.2.7/src/ms3/bs4_measures.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   130482 2023-04-26 16:41:43.000000 ms3-1.2.7/src/ms3/bs4_parser.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    41211 2023-04-28 13:53:00.000000 ms3-1.2.7/src/ms3/cli.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   151734 2023-04-19 06:50:23.000000 ms3-1.2.7/src/ms3/corpus.py
+-rwxr-xr-x   0 hentsche  (1001) hentsche  (1001)    26692 2023-01-02 20:31:46.000000 ms3-1.2.7/src/ms3/expand_dcml.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     8416 2023-01-02 20:31:46.000000 ms3-1.2.7/src/ms3/ferocious_names.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    18415 2023-03-18 08:04:35.000000 ms3-1.2.7/src/ms3/logger.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15645 2023-04-28 13:53:00.000000 ms3-1.2.7/src/ms3/operations.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    83765 2023-04-26 16:41:43.000000 ms3-1.2.7/src/ms3/parse.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    82901 2023-03-23 18:04:34.000000 ms3-1.2.7/src/ms3/piece.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    97681 2023-03-23 18:04:34.000000 ms3-1.2.7/src/ms3/score.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    67393 2023-03-23 18:04:34.000000 ms3-1.2.7/src/ms3/transformations.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   219679 2023-04-28 13:53:00.000000 ms3-1.2.7/src/ms3/utils.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    29853 2023-04-26 16:41:43.000000 ms3-1.2.7/src/ms3/view.py
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.185244 ms3-1.2.7/src/ms3.egg-info/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4564 2023-04-28 13:53:29.000000 ms3-1.2.7/src/ms3.egg-info/PKG-INFO
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     9420 2023-04-28 13:53:30.000000 ms3-1.2.7/src/ms3.egg-info/SOURCES.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)        1 2023-04-28 13:53:29.000000 ms3-1.2.7/src/ms3.egg-info/dependency_links.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       36 2023-04-28 13:53:29.000000 ms3-1.2.7/src/ms3.egg-info/entry_points.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)        1 2023-04-28 13:53:29.000000 ms3-1.2.7/src/ms3.egg-info/not-zip-safe
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      120 2023-04-28 13:53:29.000000 ms3-1.2.7/src/ms3.egg-info/requires.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)        4 2023-04-28 13:53:29.000000 ms3-1.2.7/src/ms3.egg-info/top_level.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      318 2020-05-03 17:52:04.000000 ms3-1.2.7/tox.ini
```

### Comparing `ms3-1.2.6/.coveragerc` & `ms3-1.2.7/.coveragerc`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/.github/ISSUE_TEMPLATE/bug_report.md` & `ms3-1.2.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/.github/ISSUE_TEMPLATE/feature_request.md` & `ms3-1.2.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/.github/workflows/draft-pdf.yml` & `ms3-1.2.7/.github/workflows/draft-pdf.yml`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/.gitignore` & `ms3-1.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/CHANGELOG.rst` & `ms3-1.2.7/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =========
 Changelog
 =========
 
+Version 1.2.7
+=============
+
+* warning files omit system-dependend information from warning headers (6764476)
+* bugfixes
+
 Version 1.2.6
 =============
 
 
 * changes the behaviour of the ``ms3 review`` command
   * after coloring out-of-label notes, issue one warning per dubious label
   * rather than one `warnings.log` file per corpus, create one `<fname>.warnings` file per piece in the `reviewed` folder
```

### Comparing `ms3-1.2.6/LICENSE.txt` & `ms3-1.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/PKG-INFO` & `ms3-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms3
-Version: 1.2.6
+Version: 1.2.7
 Summary: A parser for annotated MuseScore 3 files.
 Home-page: https://github.com/johentsch/ms3
 Author: Johannes Hentschel
 Author-email: johannes.hentschel@epfl.ch
 License: gpl3
 Project-URL: Documentation, https://johentsch.github.io/ms3/
 Platform: any
```

### Comparing `ms3-1.2.6/README.rst` & `ms3-1.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/codemeta.json` & `ms3-1.2.7/codemeta.json`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/Makefile` & `ms3-1.2.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/_intersphinx/bs4_objects.inv` & `ms3-1.2.7/docs/_intersphinx/bs4_objects.inv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/_intersphinx/bs4_objects.txt` & `ms3-1.2.7/docs/_intersphinx/bs4_objects.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/.doctrees/api/modules.doctree` & `ms3-1.2.7/docs/build/.doctrees/api/modules.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/.doctrees/api/ms3.doctree` & `ms3-1.2.7/docs/build/.doctrees/api/ms3.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/.doctrees/authors.doctree` & `ms3-1.2.7/docs/build/.doctrees/authors.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/.doctrees/changelog.doctree` & `ms3-1.2.7/docs/build/.doctrees/changelog.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/.doctrees/environment.pickle` & `ms3-1.2.7/docs/build/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/.doctrees/index.doctree` & `ms3-1.2.7/docs/build/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/.doctrees/install.doctree` & `ms3-1.2.7/docs/build/.doctrees/install.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/.doctrees/intro.doctree` & `ms3-1.2.7/docs/build/.doctrees/intro.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/.doctrees/license.doctree` & `ms3-1.2.7/docs/build/.doctrees/license.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/.doctrees/manual.doctree` & `ms3-1.2.7/docs/build/.doctrees/manual.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/.doctrees/quick.doctree` & `ms3-1.2.7/docs/build/.doctrees/quick.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/doctrees/README.doctree` & `ms3-1.2.7/docs/build/doctrees/README.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/doctrees/authors.doctree` & `ms3-1.2.7/docs/build/doctrees/authors.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/doctrees/changelog.doctree` & `ms3-1.2.7/docs/build/doctrees/changelog.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/doctrees/environment.pickle` & `ms3-1.2.7/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/doctrees/index.doctree` & `ms3-1.2.7/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/doctrees/install.doctree` & `ms3-1.2.7/docs/build/doctrees/install.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/doctrees/license.doctree` & `ms3-1.2.7/docs/build/doctrees/license.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/doctrees/manual/index.doctree` & `ms3-1.2.7/docs/build/doctrees/manual/index.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/doctrees/old_src/quick_old.doctree` & `ms3-1.2.7/docs/build/doctrees/old_src/quick_old.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/doctrees/quick.doctree` & `ms3-1.2.7/docs/build/doctrees/quick.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/doctrees/reference.doctree` & `ms3-1.2.7/docs/build/doctrees/reference.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/README.html` & `ms3-1.2.7/docs/build/html/README.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_modules/index.html` & `ms3-1.2.7/docs/build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_modules/ms3/annotations.html` & `ms3-1.2.7/docs/build/html/_modules/ms3/annotations.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_modules/ms3/bs4_parser.html` & `ms3-1.2.7/docs/build/html/_modules/ms3/bs4_parser.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_modules/ms3/corpus.html` & `ms3-1.2.7/docs/build/html/_modules/ms3/corpus.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_modules/ms3/expand_dcml.html` & `ms3-1.2.7/docs/build/html/_modules/ms3/expand_dcml.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_modules/ms3/parse.html` & `ms3-1.2.7/docs/build/html/_modules/ms3/parse.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_modules/ms3/piece.html` & `ms3-1.2.7/docs/build/html/_modules/ms3/piece.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_modules/ms3/score.html` & `ms3-1.2.7/docs/build/html/_modules/ms3/score.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_modules/ms3/transformations.html` & `ms3-1.2.7/docs/build/html/_modules/ms3/transformations.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_modules/ms3/utils.html` & `ms3-1.2.7/docs/build/html/_modules/ms3/utils.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_modules/ms3/view.html` & `ms3-1.2.7/docs/build/html/_modules/ms3/view.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_modules/re.html` & `ms3-1.2.7/docs/build/html/_modules/re.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_sources/index.rst.txt` & `ms3-1.2.7/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_sources/install.rst.txt` & `ms3-1.2.7/docs/build/html/_sources/install.rst.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_sources/manual/index.md.txt` & `ms3-1.2.7/docs/build/html/_sources/manual/index.md.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_sources/old_src/quick_old.rst.txt` & `ms3-1.2.7/docs/build/html/_sources/old_src/quick_old.rst.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_sources/quick.md.txt` & `ms3-1.2.7/docs/build/html/_sources/quick.md.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_sources/reference.rst.txt` & `ms3-1.2.7/docs/build/html/_sources/reference.rst.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js` & `ms3-1.2.7/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/basic.css` & `ms3-1.2.7/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/doctools.js` & `ms3-1.2.7/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/jquery-3.6.0.js` & `ms3-1.2.7/docs/build/html/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/jquery.js` & `ms3-1.2.7/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/jupyter-sphinx.css` & `ms3-1.2.7/docs/build/html/_static/jupyter-sphinx.css`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/language_data.js` & `ms3-1.2.7/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css` & `ms3-1.2.7/docs/build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/pygments.css` & `ms3-1.2.7/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/scripts/bootstrap.js` & `ms3-1.2.7/docs/build/html/_static/scripts/bootstrap.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/scripts/pydata-sphinx-theme.js` & `ms3-1.2.7/docs/build/html/_static/scripts/pydata-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/searchtools.js` & `ms3-1.2.7/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/sphinx_highlight.js` & `ms3-1.2.7/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/styles/bootstrap.css` & `ms3-1.2.7/docs/build/html/_static/styles/bootstrap.css`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/styles/pydata-sphinx-theme.css` & `ms3-1.2.7/docs/build/html/_static/styles/pydata-sphinx-theme.css`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/underscore-1.13.1.js` & `ms3-1.2.7/docs/build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/underscore.js` & `ms3-1.2.7/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt` & `ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css` & `ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf` & `ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2` & `ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf` & `ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2` & `ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf` & `ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2` & `ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf` & `ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2` & `ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/_static/webpack-macros.html` & `ms3-1.2.7/docs/build/html/_static/webpack-macros.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/authors.html` & `ms3-1.2.7/docs/build/html/authors.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/changelog.html` & `ms3-1.2.7/docs/build/html/changelog.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/genindex.html` & `ms3-1.2.7/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/index.html` & `ms3-1.2.7/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/install.html` & `ms3-1.2.7/docs/build/html/install.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/license.html` & `ms3-1.2.7/docs/build/html/license.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/manual/index.html` & `ms3-1.2.7/docs/build/html/manual/index.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/objects.inv` & `ms3-1.2.7/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/old_src/quick_old.html` & `ms3-1.2.7/docs/build/html/old_src/quick_old.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/py-modindex.html` & `ms3-1.2.7/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/quick.html` & `ms3-1.2.7/docs/build/html/quick.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/reference.html` & `ms3-1.2.7/docs/build/html/reference.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/search.html` & `ms3-1.2.7/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/html/searchindex.js` & `ms3-1.2.7/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/jupyter_execute/manual/index.ipynb` & `ms3-1.2.7/docs/build/jupyter_execute/manual/index.ipynb`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/build/jupyter_execute/quick.ipynb` & `ms3-1.2.7/docs/build/jupyter_execute/quick.ipynb`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/conf.py` & `ms3-1.2.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/cujus.mscx` & `ms3-1.2.7/docs/cujus.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/index.rst` & `ms3-1.2.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/install.rst` & `ms3-1.2.7/docs/install.rst`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/manual/corpus_after` & `ms3-1.2.7/docs/manual/corpus_after`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/manual/index.md` & `ms3-1.2.7/docs/manual/index.md`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/ms3_architecture.drawio` & `ms3-1.2.7/docs/ms3_architecture.drawio`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/ms3_architecture.png` & `ms3-1.2.7/docs/ms3_architecture.png`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/o_quam.mscx` & `ms3-1.2.7/docs/o_quam.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/old_src/quick_old.md` & `ms3-1.2.7/docs/old_src/quick_old.md`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/old_src/quick_old.rst` & `ms3-1.2.7/docs/old_src/quick_old.rst`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/quae.mscx` & `ms3-1.2.7/docs/quae.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/quick.md` & `ms3-1.2.7/docs/quick.md`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/reference.rst` & `ms3-1.2.7/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/docs/stabat.mscx` & `ms3-1.2.7/docs/stabat.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/new_tests/conftest.py` & `ms3-1.2.7/new_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica.tsv` & `ms3-1.2.7/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica_results.tsv` & `ms3-1.2.7/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica_results.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica_results_midi.tsv` & `ms3-1.2.7/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica_results_midi.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/new_tests/test_extract.py` & `ms3-1.2.7/new_tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/new_tests/test_parse.py` & `ms3-1.2.7/new_tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/new_tests/test_score.py` & `ms3-1.2.7/new_tests/test_score.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/new_tests/test_transformations.py` & `ms3-1.2.7/new_tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/05_symph_fant_events.tsv` & `ms3-1.2.7/old_tests/05_symph_fant_events.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/05_symph_fant_measures.tsv` & `ms3-1.2.7/old_tests/05_symph_fant_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/05_symph_fant_notes.tsv` & `ms3-1.2.7/old_tests/05_symph_fant_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/76CASM34A33UM_events.tsv` & `ms3-1.2.7/old_tests/76CASM34A33UM_events.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/76CASM34A33UM_labels.tsv` & `ms3-1.2.7/old_tests/76CASM34A33UM_labels.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/76CASM34A33UM_measures.tsv` & `ms3-1.2.7/old_tests/76CASM34A33UM_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/76CASM34A33UM_notes.tsv` & `ms3-1.2.7/old_tests/76CASM34A33UM_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/ALL_WARNINGS` & `ms3-1.2.7/old_tests/ALL_WARNINGS`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/BWV_0815_events.tsv` & `ms3-1.2.7/old_tests/BWV_0815_events.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/BWV_0815_measures.tsv` & `ms3-1.2.7/old_tests/BWV_0815_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/BWV_0815_notes.tsv` & `ms3-1.2.7/old_tests/BWV_0815_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/D973deutscher01_events.tsv` & `ms3-1.2.7/old_tests/D973deutscher01_events.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/D973deutscher01_measures.tsv` & `ms3-1.2.7/old_tests/D973deutscher01_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/D973deutscher01_notes.tsv` & `ms3-1.2.7/old_tests/D973deutscher01_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/Did03M-Son_regina-1762-Sarti_events.tsv` & `ms3-1.2.7/old_tests/Did03M-Son_regina-1762-Sarti_events.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/Did03M-Son_regina-1762-Sarti_labels.tsv` & `ms3-1.2.7/old_tests/Did03M-Son_regina-1762-Sarti_labels.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/Did03M-Son_regina-1762-Sarti_measures.tsv` & `ms3-1.2.7/old_tests/Did03M-Son_regina-1762-Sarti_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/Did03M-Son_regina-1762-Sarti_notes.tsv` & `ms3-1.2.7/old_tests/Did03M-Son_regina-1762-Sarti_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/K281-3_events.tsv` & `ms3-1.2.7/old_tests/K281-3_events.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/K281-3_labels.tsv` & `ms3-1.2.7/old_tests/K281-3_labels.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/K281-3_measures.tsv` & `ms3-1.2.7/old_tests/K281-3_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/K281-3_notes.tsv` & `ms3-1.2.7/old_tests/K281-3_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/MS3/05_symph_fant.mscx` & `ms3-1.2.7/old_tests/MS3/05_symph_fant.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/MS3/76CASM34A33UM.mscx` & `ms3-1.2.7/old_tests/MS3/76CASM34A33UM.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/MS3/BWV_0815.mscx` & `ms3-1.2.7/old_tests/MS3/BWV_0815.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/MS3/D973deutscher01.mscx` & `ms3-1.2.7/old_tests/MS3/D973deutscher01.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/MS3/Did03M-Son_regina-1762-Sarti.mscx` & `ms3-1.2.7/old_tests/MS3/Did03M-Son_regina-1762-Sarti.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/MS3/K281-3.mscx` & `ms3-1.2.7/old_tests/MS3/K281-3.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/MS3/stabat_03_coloured.mscx` & `ms3-1.2.7/old_tests/MS3/stabat_03_coloured.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/README.md` & `ms3-1.2.7/old_tests/README.md`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/harmonies/76CASM34A33UM.tsv` & `ms3-1.2.7/old_tests/harmonies/76CASM34A33UM.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/harmonies/Did03M-Son_regina-1762-Sarti.tsv` & `ms3-1.2.7/old_tests/harmonies/Did03M-Son_regina-1762-Sarti.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/harmonies/K281-3.tsv` & `ms3-1.2.7/old_tests/harmonies/K281-3.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/harmonies/stabat_03_coloured.tsv` & `ms3-1.2.7/old_tests/harmonies/stabat_03_coloured.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/measures/05_symph_fant.tsv` & `ms3-1.2.7/old_tests/measures/05_symph_fant.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/measures/76CASM34A33UM.tsv` & `ms3-1.2.7/old_tests/measures/76CASM34A33UM.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/measures/BWV_0815.tsv` & `ms3-1.2.7/old_tests/measures/BWV_0815.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/measures/D973deutscher01.tsv` & `ms3-1.2.7/old_tests/measures/D973deutscher01.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/measures/Did03M-Son_regina-1762-Sarti.tsv` & `ms3-1.2.7/old_tests/measures/Did03M-Son_regina-1762-Sarti.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/measures/K281-3.tsv` & `ms3-1.2.7/old_tests/measures/K281-3.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/measures/stabat_03_coloured.tsv` & `ms3-1.2.7/old_tests/measures/stabat_03_coloured.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/metadata.tsv` & `ms3-1.2.7/old_tests/metadata.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/notes/05_symph_fant.tsv` & `ms3-1.2.7/old_tests/notes/05_symph_fant.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/notes/76CASM34A33UM.tsv` & `ms3-1.2.7/old_tests/notes/76CASM34A33UM.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/notes/BWV_0815.tsv` & `ms3-1.2.7/old_tests/notes/BWV_0815.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/notes/D973deutscher01.tsv` & `ms3-1.2.7/old_tests/notes/D973deutscher01.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/notes/Did03M-Son_regina-1762-Sarti.tsv` & `ms3-1.2.7/old_tests/notes/Did03M-Son_regina-1762-Sarti.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/notes/K281-3.tsv` & `ms3-1.2.7/old_tests/notes/K281-3.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/notes/stabat_03_coloured.tsv` & `ms3-1.2.7/old_tests/notes/stabat_03_coloured.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/paths1.json` & `ms3-1.2.7/old_tests/paths1.json`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/paths2.json` & `ms3-1.2.7/old_tests/paths2.json`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/repeat_dummies/repeats0.mscx` & `ms3-1.2.7/old_tests/repeat_dummies/repeats0.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/repeat_dummies/repeats1.mscx` & `ms3-1.2.7/old_tests/repeat_dummies/repeats1.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/repeat_dummies/repeats2.mscx` & `ms3-1.2.7/old_tests/repeat_dummies/repeats2.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/stabat_03_coloured_events.tsv` & `ms3-1.2.7/old_tests/stabat_03_coloured_events.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/stabat_03_coloured_labels.tsv` & `ms3-1.2.7/old_tests/stabat_03_coloured_labels.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/stabat_03_coloured_measures.tsv` & `ms3-1.2.7/old_tests/stabat_03_coloured_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/stabat_03_coloured_notes.tsv` & `ms3-1.2.7/old_tests/stabat_03_coloured_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/test_parse.py` & `ms3-1.2.7/old_tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/test_repeats.py` & `ms3-1.2.7/old_tests/test_repeats.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/test_results/05_symph_fant_measures.tsv` & `ms3-1.2.7/old_tests/test_results/05_symph_fant_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/test_results/05_symph_fant_notes.tsv` & `ms3-1.2.7/old_tests/test_results/05_symph_fant_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/test_results/76CASM34A33UM_labels.tsv` & `ms3-1.2.7/old_tests/test_results/76CASM34A33UM_labels.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/test_results/76CASM34A33UM_measures.tsv` & `ms3-1.2.7/old_tests/test_results/76CASM34A33UM_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/test_results/76CASM34A33UM_notes.tsv` & `ms3-1.2.7/old_tests/test_results/76CASM34A33UM_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/test_results/BWV_0815_measures.tsv` & `ms3-1.2.7/old_tests/test_results/BWV_0815_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/test_results/BWV_0815_notes.tsv` & `ms3-1.2.7/old_tests/test_results/BWV_0815_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/test_results/D973deutscher01_measures.tsv` & `ms3-1.2.7/old_tests/test_results/D973deutscher01_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/test_results/D973deutscher01_notes.tsv` & `ms3-1.2.7/old_tests/test_results/D973deutscher01_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/test_results/Did03M-Son_regina-1762-Sarti_labels.tsv` & `ms3-1.2.7/old_tests/test_results/Did03M-Son_regina-1762-Sarti_labels.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/test_results/Did03M-Son_regina-1762-Sarti_measures.tsv` & `ms3-1.2.7/old_tests/test_results/Did03M-Son_regina-1762-Sarti_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/test_results/Did03M-Son_regina-1762-Sarti_notes.tsv` & `ms3-1.2.7/old_tests/test_results/Did03M-Son_regina-1762-Sarti_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/test_results/K281-3_labels.tsv` & `ms3-1.2.7/old_tests/test_results/K281-3_labels.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/test_results/K281-3_measures.tsv` & `ms3-1.2.7/old_tests/test_results/K281-3_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/test_results/K281-3_notes.tsv` & `ms3-1.2.7/old_tests/test_results/K281-3_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/test_results/stabat_03_coloured_labels.tsv` & `ms3-1.2.7/old_tests/test_results/stabat_03_coloured_labels.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/test_results/stabat_03_coloured_measures.tsv` & `ms3-1.2.7/old_tests/test_results/stabat_03_coloured_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/test_results/stabat_03_coloured_notes.tsv` & `ms3-1.2.7/old_tests/test_results/stabat_03_coloured_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/old_tests/test_score.py` & `ms3-1.2.7/old_tests/test_score.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/paper/paper.bib` & `ms3-1.2.7/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/paper/paper.md` & `ms3-1.2.7/paper/paper.md`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/paper/paper.pdf` & `ms3-1.2.7/paper/paper.pdf`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/setup.cfg` & `ms3-1.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/setup.py` & `ms3-1.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/src/ms3/__init__.py` & `ms3-1.2.7/src/ms3/__init__.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/src/ms3/_typing.py` & `ms3-1.2.7/src/ms3/_typing.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/src/ms3/annotations.py` & `ms3-1.2.7/src/ms3/annotations.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/src/ms3/bs4_measures.py` & `ms3-1.2.7/src/ms3/bs4_measures.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/src/ms3/bs4_parser.py` & `ms3-1.2.7/src/ms3/bs4_parser.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/src/ms3/cli.py` & `ms3-1.2.7/src/ms3/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,21 +302,21 @@
 
     # call ms3 check, collecting all warnings issued while parsing
     if args.ignore_scores + args.ignore_labels < 2:
         what = '' if args.ignore_scores else 'SCORES'
         if args.ignore_labels:
             what += 'LABELS' if what == '' else 'AND LABELS'
         print(f"CHECKING {what}...")
-        with capture_parse_logs(p.logger) as captured_warnings:
-            test_passes = check(p,
-                                ignore_labels=args.ignore_labels,
-                                ignore_scores=args.ignore_scores,
-                                assertion=False,
-                                parallel=False)
-            accumulated_warnings.extend(captured_warnings.content_list)
+        warning = check(p,
+                            ignore_labels=args.ignore_labels,
+                            ignore_scores=args.ignore_scores,
+                            assertion=False,
+                            parallel=False)
+        accumulated_warnings.extend(warning)
+        test_passes = len(warning) == 0
         p.parse_tsv()
     else:
         test_passes = True
         p.parse(parallel=False)
     if p.n_parsed_scores == 0:
         msg = "NO SCORES PARSED, NOTHING TO DO."
         if not args.all:
@@ -330,28 +330,30 @@
     if len(params) > 0:
         print("EXTRACTING FACETS...")
         extract_cmd(args, p)
 
     # color out-of-label tones
     print("COLORING OUT-OF-LABEL TONES...")
     with capture_parse_logs(p.logger) as captured_warnings:
-        test_passes = test_passes and make_coloring_reports_and_warnings(p, out_dir=args.out, threshold=args.threshold)
+        test_passes = make_coloring_reports_and_warnings(p, out_dir=args.out, threshold=args.threshold) and test_passes
         accumulated_warnings.extend(captured_warnings.content_list)
 
     # attribute warnings to pieces based on logger names
     logger2pieceID = {corpus.logger_names[fname]: (c, fname) for c, corpus in p.corpus_objects.items() for fname in corpus.keys()}
     piece2warnings = defaultdict(list)
     for warning in accumulated_warnings:
-        try:
-            match = next(logger_name for component in warning.split() if (logger_name := re.match(r"ms3\.Parse\.(?P<corpus>\S+)\.(?P<fname>\S+)$", component)))
-        except StopIteration:
-            logger.warning(f"This warning contains no valid logger name, skipping: {warning}")
+        warning_lines = warning.splitlines()
+        first_line = warning_lines[0]
+        match = re.search(r"ms3\.Parse\.\S+\.\S+", first_line)
+        if match is None:
+            logger.warning(f"This warning contains no ms3 logger name, skipping: {warning}")
             continue
+        warning_lines[0] = first_line[:match.end()]  # cut off the warning's header everything following the logger name because paths to source code are system-dependent
         pieceID = logger2pieceID[match.group(0)]
-        piece2warnings[pieceID].append(warning)
+        piece2warnings[pieceID].append('\n'.join(warning_lines))
 
 
     # write all warnings to piece-specific warnings files and remove existing files where no warnings were captured
     for pieceID, score_files in p.get_files('scores', unparsed=False, flat=True, include_empty=False).items():
         file = score_files[0]
         warnings_path = compute_path_from_file(file, root_dir=args.out, folder='reviewed')
         warnings_file = os.path.join(warnings_path, file.fname + file.suffix + '.warnings')
```

### Comparing `ms3-1.2.6/src/ms3/corpus.py` & `ms3-1.2.7/src/ms3/corpus.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/src/ms3/expand_dcml.py` & `ms3-1.2.7/src/ms3/expand_dcml.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/src/ms3/ferocious_names.txt` & `ms3-1.2.7/src/ms3/ferocious_names.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/src/ms3/logger.py` & `ms3-1.2.7/src/ms3/logger.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/src/ms3/operations.py` & `ms3-1.2.7/src/ms3/operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
 
 
 def check(parse_obj: Parse,
           ignore_labels: bool = False,
           ignore_scores: bool = False,
           assertion: bool = False,
-          parallel: bool = True) -> bool:
+          parallel: bool = True) -> List[str]:
     assert ignore_labels + ignore_scores < 2, "Activate either ignore_labels or ignore_scores, not both."
     all_warnings = []
     check_logger = get_logger("ms3.check", level=parse_obj.logger.getEffectiveLevel())
     if not ignore_scores:
         with capture_parse_logs(parse_obj.logger) as captured_warnings:
             parse_obj.parse_scores(parallel=parallel, only_new=False)
             warnings = captured_warnings.content_list
@@ -133,17 +133,15 @@
         if ignore_labels:
             msg = 'All checked scores alright.'
         elif ignore_scores:
             msg = 'All checked labels alright.'
         else:
             msg = 'All checked scores and labels alright.'
         check_logger.info(msg)
-        return True
-    else:
-        return False
+    return all_warnings
 
 @function_logger
 def compare(parse_obj: Parse,
             facet: AnnotationsFacet,
             ask: bool = False,
             revision_specifier: Optional[str] = None,
             flip=False) -> Tuple[int, int]:
```

### Comparing `ms3-1.2.6/src/ms3/parse.py` & `ms3-1.2.7/src/ms3/parse.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/src/ms3/piece.py` & `ms3-1.2.7/src/ms3/piece.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/src/ms3/score.py` & `ms3-1.2.7/src/ms3/score.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/src/ms3/transformations.py` & `ms3-1.2.7/src/ms3/transformations.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/src/ms3/utils.py` & `ms3-1.2.7/src/ms3/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 00000420: 7064 6174 655f 6366 672c 204c 6f67 4361  pdate_cfg, LogCa
 00000430: 7074 7572 6572 0a66 726f 6d20 2e5f 7479  pturer.from ._ty
 00000440: 7069 6e67 2069 6d70 6f72 7420 4669 6c65  ping import File
 00000450: 4469 6374 2c20 4661 6365 742c 2056 6965  Dict, Facet, Vie
 00000460: 7744 6963 742c 2046 696c 6544 6174 6166  wDict, FileDataf
 00000470: 7261 6d65 5475 706c 654d 6179 6265 0a0a  rameTupleMaybe..
 00000480: 4d53 335f 5645 5253 494f 4e20 3d20 2731  MS3_VERSION = '1
-00000490: 2e32 2e36 270a 4c41 5445 5354 5f4d 5553  .2.6'.LATEST_MUS
+00000490: 2e32 2e37 270a 4c41 5445 5354 5f4d 5553  .2.7'.LATEST_MUS
 000004a0: 4553 434f 5245 5f56 4552 5349 4f4e 203d  ESCORE_VERSION =
 000004b0: 2027 332e 362e 3227 0a43 4f4d 5055 5445   '3.6.2'.COMPUTE
 000004c0: 445f 4d45 5441 4441 5441 5f43 4f4c 554d  D_METADATA_COLUM
 000004d0: 4e53 203d 205b 2754 696d 6553 6967 272c  NS = ['TimeSig',
 000004e0: 2027 4b65 7953 6967 272c 2027 6c61 7374   'KeySig', 'last
 000004f0: 5f6d 6327 2c20 276c 6173 745f 6d6e 272c  _mc', 'last_mn',
 00000500: 2027 6c65 6e67 7468 5f71 6227 2c20 276c   'length_qb', 'l
@@ -13658,74 +13658,73 @@
 00035590: 207b 7265 6c5f 7061 7468 7d20 4020 636f   {rel_path} @ co
 000355a0: 6d6d 6974 207b 636f 6d6d 6974 5f69 6e66  mmit {commit_inf
 000355b0: 6f7d 2066 6169 6c65 6420 7769 7468 2074  o} failed with t
 000355c0: 6865 2066 6f6c 6c6f 7769 6e67 2065 7863  he following exc
 000355d0: 6570 7469 6f6e 3a5c 6e7b 657d 2229 0a20  eption:\n{e}"). 
 000355e0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
 000355f0: 6e65 2c20 4e6f 6e65 0a20 2020 206e 6577  ne, None.    new
-00035600: 5f66 696c 6520 3d20 6461 7461 636c 6173  _file = dataclas
-00035610: 7365 732e 7265 706c 6163 6528 6669 6c65  ses.replace(file
-00035620: 2c20 636f 6d6d 6974 5f73 6861 3d63 6f6d  , commit_sha=com
-00035630: 6d69 745f 7368 6129 0a20 2020 2072 6574  mit_sha).    ret
-00035640: 7572 6e20 6e65 775f 6669 6c65 2c20 7061  urn new_file, pa
-00035650: 7273 6564 0a0a 0a40 6675 6e63 7469 6f6e  rsed...@function
-00035660: 5f6c 6f67 6765 720a 6465 6620 6368 6563  _logger.def chec
-00035670: 6b5f 7068 7261 7365 5f61 6e6e 6f74 6174  k_phrase_annotat
-00035680: 696f 6e73 2864 663a 2070 642e 4461 7461  ions(df: pd.Data
-00035690: 4672 616d 652c 0a20 2020 2020 2020 2020  Frame,.         
-000356a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000356b0: 2020 2020 636f 6c75 6d6e 3a20 7374 7229      column: str)
-000356c0: 202d 3e20 626f 6f6c 3a0a 2020 2020 2222   -> bool:.    ""
-000356d0: 2222 2222 0a20 2020 2070 5f63 6f6c 203d  """".    p_col =
-000356e0: 2064 665b 636f 6c75 6d6e 5d0a 2020 2020   df[column].    
-000356f0: 6f70 656e 696e 6720 3d20 705f 636f 6c2e  opening = p_col.
-00035700: 6669 6c6c 6e61 2827 2729 2e73 7472 2e63  fillna('').str.c
-00035710: 6f75 6e74 2827 7b27 290a 2020 2020 636c  ount('{').    cl
-00035720: 6f73 696e 6720 3d20 705f 636f 6c2e 6669  osing = p_col.fi
-00035730: 6c6c 6e61 2827 2729 2e73 7472 2e63 6f75  llna('').str.cou
-00035740: 6e74 2827 7d27 290a 2020 2020 6966 2027  nt('}').    if '
-00035750: 6d6e 5f70 6c61 7974 6872 6f75 6768 2720  mn_playthrough' 
-00035760: 696e 2064 662e 636f 6c75 6d6e 733a 0a20  in df.columns:. 
-00035770: 2020 2020 2020 2070 6f73 6974 696f 6e5f         position_
-00035780: 636f 6c20 3d20 276d 6e5f 706c 6179 7468  col = 'mn_playth
-00035790: 726f 7567 6827 0a20 2020 2065 6c73 653a  rough'.    else:
-000357a0: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-000357b0: 696e 666f 2866 2243 6f6c 756d 6e20 276d  info(f"Column 'm
-000357c0: 6e5f 706c 6179 7468 726f 7567 6827 2069  n_playthrough' i
-000357d0: 7320 6d69 7373 696e 672c 2073 6f20 6d79  s missing, so my
-000357e0: 2061 7373 6573 736d 656e 7420 6f66 2074   assessment of t
-000357f0: 6865 2070 6872 6173 6520 616e 6e6f 7461  he phrase annota
-00035800: 7469 6f6e 7320 6d69 6768 7420 6265 2077  tions might be w
-00035810: 726f 6e67 2e22 290a 2020 2020 2020 2020  rong.").        
-00035820: 706f 7369 7469 6f6e 5f63 6f6c 203d 2027  position_col = '
-00035830: 6d6e 270a 2020 2020 636f 6c75 6d6e 7320  mn'.    columns 
-00035840: 3d20 5b70 6f73 6974 696f 6e5f 636f 6c2c  = [position_col,
-00035850: 2063 6f6c 756d 6e5d 0a20 2020 2069 6620   column].    if 
-00035860: 6f70 656e 696e 672e 7375 6d28 2920 213d  opening.sum() !=
-00035870: 2063 6c6f 7369 6e67 2e73 756d 2829 3a0a   closing.sum():.
-00035880: 2020 2020 2020 2020 6f20 3d20 6466 2e6c          o = df.l
-00035890: 6f63 5b28 6f70 656e 696e 6720 3e20 3029  oc[(opening > 0)
-000358a0: 2c20 636f 6c75 6d6e 735d 0a20 2020 2020  , columns].     
-000358b0: 2020 2063 203d 2064 662e 6c6f 635b 2863     c = df.loc[(c
-000358c0: 6c6f 7369 6e67 203e 2030 292c 2063 6f6c  losing > 0), col
-000358d0: 756d 6e73 5d0a 2020 2020 2020 2020 636f  umns].        co
-000358e0: 6d70 6172 6520 3d20 7064 2e63 6f6e 6361  mpare = pd.conca
-000358f0: 7428 5b6f 2e72 6573 6574 5f69 6e64 6578  t([o.reset_index
-00035900: 2864 726f 703d 5472 7565 292c 2063 2e72  (drop=True), c.r
-00035910: 6573 6574 5f69 6e64 6578 2864 726f 703d  eset_index(drop=
-00035920: 5472 7565 295d 2c20 6178 6973 3d31 290a  True)], axis=1).
-00035930: 2020 2020 2020 2020 6966 2027 6d6e 2720          if 'mn' 
-00035940: 696e 2063 6f6d 7061 7265 3a0a 2020 2020  in compare:.    
-00035950: 2020 2020 2020 2020 636f 6d70 6172 6520          compare 
-00035960: 3d20 636f 6d70 6172 652e 6173 7479 7065  = compare.astype
-00035970: 287b 276d 6e27 3a20 2749 6e74 3634 277d  ({'mn': 'Int64'}
-00035980: 290a 2020 2020 2020 2020 6c6f 6767 6572  ).        logger
-00035990: 2e77 6172 6e69 6e67 2866 2250 6872 6173  .warning(f"Phras
-000359a0: 6520 6265 6769 6e6e 696e 6720 616e 6420  e beginning and 
-000359b0: 656e 6469 6e67 7320 646f 6e27 7420 6d61  endings don't ma
-000359c0: 7463 683a 5c6e 7b63 6f6d 7061 7265 2e74  tch:\n{compare.t
-000359d0: 6f5f 7374 7269 6e67 2869 6e64 6578 3d46  o_string(index=F
-000359e0: 616c 7365 297d 222c 2065 7874 7261 3d7b  alse)}", extra={
-000359f0: 226d 6573 7361 6765 5f69 6422 3a20 2831  "message_id": (1
-00035a00: 362c 297d 290a 2020 2020 2020 2020 7265  6,)}).        re
-00035a10: 7475 726e 2046 616c 7365 0a20 2020 2072  turn False.    r
-00035a20: 6574 7572 6e20 5472 7565 0a              eturn True.
+00035600: 5f66 696c 6520 3d20 7265 706c 6163 6528  _file = replace(
+00035610: 6669 6c65 2c20 636f 6d6d 6974 5f73 6861  file, commit_sha
+00035620: 3d63 6f6d 6d69 745f 7368 6129 0a20 2020  =commit_sha).   
+00035630: 2072 6574 7572 6e20 6e65 775f 6669 6c65   return new_file
+00035640: 2c20 7061 7273 6564 0a0a 0a40 6675 6e63  , parsed...@func
+00035650: 7469 6f6e 5f6c 6f67 6765 720a 6465 6620  tion_logger.def 
+00035660: 6368 6563 6b5f 7068 7261 7365 5f61 6e6e  check_phrase_ann
+00035670: 6f74 6174 696f 6e73 2864 663a 2070 642e  otations(df: pd.
+00035680: 4461 7461 4672 616d 652c 0a20 2020 2020  DataFrame,.     
+00035690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000356a0: 2020 2020 2020 2020 636f 6c75 6d6e 3a20          column: 
+000356b0: 7374 7229 202d 3e20 626f 6f6c 3a0a 2020  str) -> bool:.  
+000356c0: 2020 2222 2222 2222 0a20 2020 2070 5f63    """""".    p_c
+000356d0: 6f6c 203d 2064 665b 636f 6c75 6d6e 5d0a  ol = df[column].
+000356e0: 2020 2020 6f70 656e 696e 6720 3d20 705f      opening = p_
+000356f0: 636f 6c2e 6669 6c6c 6e61 2827 2729 2e73  col.fillna('').s
+00035700: 7472 2e63 6f75 6e74 2827 7b27 290a 2020  tr.count('{').  
+00035710: 2020 636c 6f73 696e 6720 3d20 705f 636f    closing = p_co
+00035720: 6c2e 6669 6c6c 6e61 2827 2729 2e73 7472  l.fillna('').str
+00035730: 2e63 6f75 6e74 2827 7d27 290a 2020 2020  .count('}').    
+00035740: 6966 2027 6d6e 5f70 6c61 7974 6872 6f75  if 'mn_playthrou
+00035750: 6768 2720 696e 2064 662e 636f 6c75 6d6e  gh' in df.column
+00035760: 733a 0a20 2020 2020 2020 2070 6f73 6974  s:.        posit
+00035770: 696f 6e5f 636f 6c20 3d20 276d 6e5f 706c  ion_col = 'mn_pl
+00035780: 6179 7468 726f 7567 6827 0a20 2020 2065  aythrough'.    e
+00035790: 6c73 653a 0a20 2020 2020 2020 206c 6f67  lse:.        log
+000357a0: 6765 722e 696e 666f 2866 2243 6f6c 756d  ger.info(f"Colum
+000357b0: 6e20 276d 6e5f 706c 6179 7468 726f 7567  n 'mn_playthroug
+000357c0: 6827 2069 7320 6d69 7373 696e 672c 2073  h' is missing, s
+000357d0: 6f20 6d79 2061 7373 6573 736d 656e 7420  o my assessment 
+000357e0: 6f66 2074 6865 2070 6872 6173 6520 616e  of the phrase an
+000357f0: 6e6f 7461 7469 6f6e 7320 6d69 6768 7420  notations might 
+00035800: 6265 2077 726f 6e67 2e22 290a 2020 2020  be wrong.").    
+00035810: 2020 2020 706f 7369 7469 6f6e 5f63 6f6c      position_col
+00035820: 203d 2027 6d6e 270a 2020 2020 636f 6c75   = 'mn'.    colu
+00035830: 6d6e 7320 3d20 5b70 6f73 6974 696f 6e5f  mns = [position_
+00035840: 636f 6c2c 2063 6f6c 756d 6e5d 0a20 2020  col, column].   
+00035850: 2069 6620 6f70 656e 696e 672e 7375 6d28   if opening.sum(
+00035860: 2920 213d 2063 6c6f 7369 6e67 2e73 756d  ) != closing.sum
+00035870: 2829 3a0a 2020 2020 2020 2020 6f20 3d20  ():.        o = 
+00035880: 6466 2e6c 6f63 5b28 6f70 656e 696e 6720  df.loc[(opening 
+00035890: 3e20 3029 2c20 636f 6c75 6d6e 735d 0a20  > 0), columns]. 
+000358a0: 2020 2020 2020 2063 203d 2064 662e 6c6f         c = df.lo
+000358b0: 635b 2863 6c6f 7369 6e67 203e 2030 292c  c[(closing > 0),
+000358c0: 2063 6f6c 756d 6e73 5d0a 2020 2020 2020   columns].      
+000358d0: 2020 636f 6d70 6172 6520 3d20 7064 2e63    compare = pd.c
+000358e0: 6f6e 6361 7428 5b6f 2e72 6573 6574 5f69  oncat([o.reset_i
+000358f0: 6e64 6578 2864 726f 703d 5472 7565 292c  ndex(drop=True),
+00035900: 2063 2e72 6573 6574 5f69 6e64 6578 2864   c.reset_index(d
+00035910: 726f 703d 5472 7565 295d 2c20 6178 6973  rop=True)], axis
+00035920: 3d31 290a 2020 2020 2020 2020 6966 2027  =1).        if '
+00035930: 6d6e 2720 696e 2063 6f6d 7061 7265 3a0a  mn' in compare:.
+00035940: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
+00035950: 6172 6520 3d20 636f 6d70 6172 652e 6173  are = compare.as
+00035960: 7479 7065 287b 276d 6e27 3a20 2749 6e74  type({'mn': 'Int
+00035970: 3634 277d 290a 2020 2020 2020 2020 6c6f  64'}).        lo
+00035980: 6767 6572 2e77 6172 6e69 6e67 2866 2250  gger.warning(f"P
+00035990: 6872 6173 6520 6265 6769 6e6e 696e 6720  hrase beginning 
+000359a0: 616e 6420 656e 6469 6e67 7320 646f 6e27  and endings don'
+000359b0: 7420 6d61 7463 683a 5c6e 7b63 6f6d 7061  t match:\n{compa
+000359c0: 7265 2e74 6f5f 7374 7269 6e67 2869 6e64  re.to_string(ind
+000359d0: 6578 3d46 616c 7365 297d 222c 2065 7874  ex=False)}", ext
+000359e0: 7261 3d7b 226d 6573 7361 6765 5f69 6422  ra={"message_id"
+000359f0: 3a20 2831 362c 297d 290a 2020 2020 2020  : (16,)}).      
+00035a00: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
+00035a10: 2020 2072 6574 7572 6e20 5472 7565 0a       return True.
```

### Comparing `ms3-1.2.6/src/ms3/view.py` & `ms3-1.2.7/src/ms3/view.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.6/src/ms3.egg-info/PKG-INFO` & `ms3-1.2.7/src/ms3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms3
-Version: 1.2.6
+Version: 1.2.7
 Summary: A parser for annotated MuseScore 3 files.
 Home-page: https://github.com/johentsch/ms3
 Author: Johannes Hentschel
 Author-email: johannes.hentschel@epfl.ch
 License: gpl3
 Project-URL: Documentation, https://johentsch.github.io/ms3/
 Platform: any
```

### Comparing `ms3-1.2.6/src/ms3.egg-info/SOURCES.txt` & `ms3-1.2.7/src/ms3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

