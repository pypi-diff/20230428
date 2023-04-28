# Comparing `tmp/geo-espresso-0.3.0.dev0.tar.gz` & `tmp/geo-espresso-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo-espresso-0.3.0.dev0.tar", last modified: Mon Apr 24 02:20:43 2023, max compression
+gzip compressed data, was "geo-espresso-0.3.1.tar", last modified: Fri Apr 28 00:11:01 2023, max compression
```

## Comparing `geo-espresso-0.3.0.dev0.tar` & `geo-espresso-0.3.1.tar`

### file list

```diff
@@ -1,203 +1,204 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.442083 geo-espresso-0.3.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-04-24 02:20:43.442083 geo-espresso-0.3.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.422090 geo-espresso-0.3.0.dev0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.422090 geo-espresso-0.3.0.dev0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.422090 geo-espresso-0.3.0.dev0/docs/source/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/_ext/generate_contrib_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.422090 geo-espresso-0.3.0.dev0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    16996 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/_static/contrib_edit1.png
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/_static/contrib_fork.png
--rw-r--r--   0 runner    (1001) docker     (123)    82278 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/_static/contrib_fork2.png
--rw-r--r--   0 runner    (1001) docker     (123)    22274 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/_static/contrib_fork3.png
--rw-r--r--   0 runner    (1001) docker     (123)    35166 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/_static/contrib_fork4.png
--rw-r--r--   0 runner    (1001) docker     (123)    36057 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/_static/contrib_pr1.png
--rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/_static/espresso_arch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/_static/inlab_logo_60px.png
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.422090 geo-espresso-0.3.0.dev0/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.426089 geo-espresso-0.3.0.dev0/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/_templates/autosummary/exception.rst
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/_templates/autosummary/function.rst
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.426089 geo-espresso-0.3.0.dev0/docs/source/contributor_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/contributor_guide/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/contributor_guide/github.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/contributor_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10779 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/contributor_guide/new_contrib.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/contributor_guide/setup.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/contributor_guide/submit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/contributor_guide/video.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.426089 geo-espresso-0.3.0.dev0/docs/source/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)    96856 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/developer_guide/build.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/developer_guide/ci.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/developer_guide/deploy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/developer_guide/develop.rst
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/developer_guide/licence.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/developer_guide/repository.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.426089 geo-espresso-0.3.0.dev0/docs/source/user_guide/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.426089 geo-espresso-0.3.0.dev0/docs/source/user_guide/api/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/user_guide/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/user_guide/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.426089 geo-espresso-0.3.0.dev0/docs/source/user_guide/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/user_guide/contrib/_index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/user_guide/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/user_guide/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/user_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/user_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/user_guide/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/docs/source/user_guide/why.rst
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 02:20:43.442083 geo-espresso-0.3.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.422090 geo-espresso-0.3.0.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.426089 geo-espresso-0.3.0.dev0/src/espresso/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_espresso_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.430087 geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10364 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/_fm_wavefront_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.430087 geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)    38400 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/datasets/cbmod.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.430087 geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/receivers_InLab_lrt_r36.dat
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/receivers_crossb_nwt_r10.dat
--rw-r--r--   0 runner    (1001) docker     (123)    37500 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/sources_InLab_lrt_s500.dat
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/sources_crossb_nwt_s10.dat
--rw-r--r--   0 runner    (1001) docker     (123)  1350000 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/ttimes_InLab_lrt_s500_r36.dat
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/ttimes_crossb_nwt_s10_r10.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.430087 geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/fmst/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1115 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/fmst/compile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.430087 geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/fmst/src/
--rw-r--r--   0 runner    (1001) docker     (123)    57221 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/fmst/src/fm2dss.f90
--rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/waveTracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.430087 geo-espresso-0.3.0.dev0/src/espresso/_gravity_density/
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_gravity_density/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_gravity_density/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_gravity_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21254 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_gravity_density/_gravity_density.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.434086 geo-espresso-0.3.0.dev0/src/espresso/_gravity_density/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_gravity_density/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_gravity_density/data/gravmodel1.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_gravity_density/data/testdata.txt
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_gravity_density/metadata.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.418091 geo-espresso-0.3.0.dev0/src/espresso/_machine/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.434086 geo-espresso-0.3.0.dev0/src/espresso/_machine/build_package/
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_machine/build_package/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9533 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_machine/build_package/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_machine/build_package/check_requires.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_machine/build_package/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14047 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_machine/build_package/criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)    15212 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_machine/build_package/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_machine/build_package/run_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_machine/build_package/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_machine/build_package/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.434086 geo-espresso-0.3.0.dev0/src/espresso/_machine/doc_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_machine/doc_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_machine/doc_utils/gen_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.434086 geo-espresso-0.3.0.dev0/src/espresso/_machine/new_contribution/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.434086 geo-espresso-0.3.0.dev0/src/espresso/_machine/new_contribution/_template/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_machine/new_contribution/_template/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_machine/new_contribution/_template/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_machine/new_contribution/_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.434086 geo-espresso-0.3.0.dev0/src/espresso/_machine/new_contribution/_template/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_machine/new_contribution/_template/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_machine/new_contribution/_template/data/testdata.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_machine/new_contribution/_template/example_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_machine/new_contribution/create_new_contrib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.434086 geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11970 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/_magnetotelluric_1D.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.434086 geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/data/
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/data/16-A_KN2.dat
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.434086 geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/examples/
--rw-r--r--   0 runner    (1001) docker     (123)   125288 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/examples/example_01.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/examples/example_01.py
--rw-r--r--   0 runner    (1001) docker     (123)   101422 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/examples/field_MT.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/examples/field_MT.py
--rw-r--r--   0 runner    (1001) docker     (123)   146169 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.438085 geo-espresso-0.3.0.dev0/src/espresso/_pumping_test/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_pumping_test/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_pumping_test/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_pumping_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14893 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_pumping_test/_pumping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.438085 geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     8122 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/RF.f90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.438085 geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/RFsubs/
--rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/RFsubs/dpythag.f
--rwxr-xr-x   0 runner    (1001) docker     (123)     5500 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/RFsubs/dsvdcmp.f
--rwxr-xr-x   0 runner    (1001) docker     (123)     1336 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/RFsubs/four1.f
--rwxr-xr-x   0 runner    (1001) docker     (123)      326 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/RFsubs/priorvalue.f90
--rwxr-xr-x   0 runner    (1001) docker     (123)    13138 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/RFsubs/qlayer.f
--rwxr-xr-x   0 runner    (1001) docker     (123)     1514 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/RFsubs/ran3.f
--rwxr-xr-x   0 runner    (1001) docker     (123)      343 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/RFsubs/rfi_param.inc
--rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/RFsubs/svbksb.f
--rwxr-xr-x   0 runner    (1001) docker     (123)     4110 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/RFsubs/theo.f
--rwxr-xr-x   0 runner    (1001) docker     (123)     4197 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/RFsubs/theo_noise.f
--rwxr-xr-x   0 runner    (1001) docker     (123)      963 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/RFsubs/voro2qmodel.f90
--rwxr-xr-x   0 runner    (1001) docker     (123)      298 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/RFsubs/whichcell.f90
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/_receiver_function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8649 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/rf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.438085 geo-espresso-0.3.0.dev0/src/espresso/_simple_regression/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_simple_regression/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_simple_regression/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_simple_regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_simple_regression/_simple_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.438085 geo-espresso-0.3.0.dev0/src/espresso/_slug_test/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_slug_test/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_slug_test/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_slug_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_slug_test/_slug_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-24 02:20:43.000000 geo-espresso-0.3.0.dev0/src/espresso/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.438085 geo-espresso-0.3.0.dev0/src/espresso/_xray_tracer/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_xray_tracer/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_xray_tracer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_xray_tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_xray_tracer/_xray_tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.442083 geo-espresso-0.3.0.dev0/src/espresso/_xray_tracer/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_xray_tracer/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55535 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_xray_tracer/data/csiro_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   510434 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_xray_tracer/data/example1.dat
--rw-r--r--   0 runner    (1001) docker     (123)   166740 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_xray_tracer/data/example2.dat
--rw-r--r--   0 runner    (1001) docker     (123)   233604 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_xray_tracer/data/example3.dat
--rw-r--r--   0 runner    (1001) docker     (123)   312372 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/_xray_tracer/data/inlab_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/list_problems.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.442083 geo-espresso-0.3.0.dev0/src/espresso/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/utils/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/utils/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-24 02:20:27.000000 geo-espresso-0.3.0.dev0/src/espresso/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:20:43.442083 geo-espresso-0.3.0.dev0/src/geo_espresso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-04-24 02:20:43.000000 geo-espresso-0.3.0.dev0/src/geo_espresso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-04-24 02:20:43.000000 geo-espresso-0.3.0.dev0/src/geo_espresso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 02:20:43.000000 geo-espresso-0.3.0.dev0/src/geo_espresso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-24 02:20:43.000000 geo-espresso-0.3.0.dev0/src/geo_espresso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 02:20:43.000000 geo-espresso-0.3.0.dev0/src/geo_espresso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.782809 geo-espresso-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-04-28 00:11:01.782809 geo-espresso-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.762809 geo-espresso-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.762809 geo-espresso-0.3.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.762809 geo-espresso-0.3.1/docs/source/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_ext/generate_contrib_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.762809 geo-espresso-0.3.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    16996 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_static/contrib_edit1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_static/contrib_fork.png
+-rw-r--r--   0 runner    (1001) docker     (123)    82278 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_static/contrib_fork2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22274 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_static/contrib_fork3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35166 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_static/contrib_fork4.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36057 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_static/contrib_pr1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_static/espresso_arch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_static/inlab_logo_60px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.762809 geo-espresso-0.3.1/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.762809 geo-espresso-0.3.1/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_templates/autosummary/exception.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_templates/autosummary/function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.762809 geo-espresso-0.3.1/docs/source/contributor_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/contributor_guide/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/contributor_guide/github.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/contributor_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10778 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/contributor_guide/new_contrib.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/contributor_guide/setup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/contributor_guide/submit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/contributor_guide/video.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.766809 geo-espresso-0.3.1/docs/source/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)    96854 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/developer_guide/build.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/developer_guide/ci.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/developer_guide/deploy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/developer_guide/develop.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/developer_guide/licence.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/developer_guide/repository.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.766809 geo-espresso-0.3.1/docs/source/user_guide/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.766809 geo-espresso-0.3.1/docs/source/user_guide/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/user_guide/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/user_guide/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.766809 geo-espresso-0.3.1/docs/source/user_guide/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/user_guide/contrib/_index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/user_guide/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/user_guide/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/user_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/user_guide/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/user_guide/why.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 00:11:01.782809 geo-espresso-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.758809 geo-espresso-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.766809 geo-espresso-0.3.1/src/espresso/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_espresso_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.766809 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10364 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/_fm_wavefront_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.766809 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)    38400 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/cbmod.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.770809 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/receivers_InLab_lrt_r36.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/receivers_crossb_nwt_r10.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    37500 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/sources_InLab_lrt_s500.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/sources_crossb_nwt_s10.dat
+-rw-r--r--   0 runner    (1001) docker     (123)  1350000 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/ttimes_InLab_lrt_s500_r36.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/ttimes_crossb_nwt_s10_r10.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.770809 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/fmst/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1115 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/fmst/compile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.770809 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/fmst/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    57221 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/fmst/src/fm2dss.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/waveTracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.770809 geo-espresso-0.3.1/src/espresso/_gravity_density/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_gravity_density/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_gravity_density/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_gravity_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21254 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_gravity_density/_gravity_density.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.770809 geo-espresso-0.3.1/src/espresso/_gravity_density/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_gravity_density/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_gravity_density/data/gravmodel1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_gravity_density/data/testdata.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_gravity_density/metadata.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.758809 geo-espresso-0.3.1/src/espresso/_machine/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.770809 geo-espresso-0.3.1/src/espresso/_machine/build_package/
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/build_package/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/build_package/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/build_package/check_requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/build_package/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14047 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/build_package/criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15212 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/build_package/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/build_package/run_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/build_package/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/build_package/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.770809 geo-espresso-0.3.1/src/espresso/_machine/doc_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/doc_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/doc_utils/_sample_code.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/doc_utils/gen_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.770809 geo-espresso-0.3.1/src/espresso/_machine/new_contribution/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.774809 geo-espresso-0.3.1/src/espresso/_machine/new_contribution/_template/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/new_contribution/_template/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/new_contribution/_template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/new_contribution/_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.774809 geo-espresso-0.3.1/src/espresso/_machine/new_contribution/_template/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/new_contribution/_template/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/new_contribution/_template/data/testdata.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/new_contribution/_template/example_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/new_contribution/create_new_contrib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.774809 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11970 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/_magnetotelluric_1D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.774809 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/data/16-A_KN2.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.774809 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   125288 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/example_01.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/example_01.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101422 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/field_MT.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/field_MT.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146169 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.774809 geo-espresso-0.3.1/src/espresso/_pumping_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_pumping_test/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_pumping_test/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_pumping_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14893 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_pumping_test/_pumping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.774809 geo-espresso-0.3.1/src/espresso/_receiver_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8122 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RF.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.778809 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/dpythag.f
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5500 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/dsvdcmp.f
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1336 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/four1.f
+-rwxr-xr-x   0 runner    (1001) docker     (123)      326 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/priorvalue.f90
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13138 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/qlayer.f
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1514 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/ran3.f
+-rwxr-xr-x   0 runner    (1001) docker     (123)      343 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/rfi_param.inc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/svbksb.f
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4110 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/theo.f
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4197 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/theo_noise.f
+-rwxr-xr-x   0 runner    (1001) docker     (123)      963 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/voro2qmodel.f90
+-rwxr-xr-x   0 runner    (1001) docker     (123)      298 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/whichcell.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/_receiver_function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8649 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/rf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.778809 geo-espresso-0.3.1/src/espresso/_simple_regression/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_simple_regression/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_simple_regression/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_simple_regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_simple_regression/_simple_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.778809 geo-espresso-0.3.1/src/espresso/_slug_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_slug_test/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_slug_test/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_slug_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_slug_test/_slug_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 00:11:01.000000 geo-espresso-0.3.1/src/espresso/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.778809 geo-espresso-0.3.1/src/espresso/_xray_tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_xray_tracer/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_xray_tracer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_xray_tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_xray_tracer/_xray_tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.778809 geo-espresso-0.3.1/src/espresso/_xray_tracer/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_xray_tracer/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55535 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_xray_tracer/data/csiro_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   510434 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_xray_tracer/data/example1.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   166740 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_xray_tracer/data/example2.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   233604 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_xray_tracer/data/example3.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   312372 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_xray_tracer/data/inlab_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.778809 geo-espresso-0.3.1/src/espresso/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/utils/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.782809 geo-espresso-0.3.1/src/geo_espresso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-04-28 00:11:01.000000 geo-espresso-0.3.1/src/geo_espresso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-04-28 00:11:01.000000 geo-espresso-0.3.1/src/geo_espresso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:11:01.000000 geo-espresso-0.3.1/src/geo_espresso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 00:11:01.000000 geo-espresso-0.3.1/src/geo_espresso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 00:11:01.000000 geo-espresso-0.3.1/src/geo_espresso.egg-info/top_level.txt
```

### Comparing `geo-espresso-0.3.0.dev0/.gitignore` & `geo-espresso-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/CHANGELOG.md` & `geo-espresso-0.3.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Change Log
 
+## v0.3.1 (27/04/2023)
+
+### Espresso core
+
+- Fix `list_capabilities` and enhance related documentation 
+
+## v0.3.0 (24/04/2023)
+
+First release.
+
 ## v0.3.0.dev0 (24/04/2023)
 
 ### Changed examples
 
 - Fix installation of receiver function on Windows
 - Fix documentation rendering of 1D MT problem
```

### Comparing `geo-espresso-0.3.0.dev0/LICENCE` & `geo-espresso-0.3.1/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/PKG-INFO` & `geo-espresso-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-espresso
-Version: 0.3.0.dev0
+Version: 0.3.1
 Summary: Earth Science PRoblems for the Evaluation of Strategies, Solvers and Optimizers
 Author: InLab, Espresso development team
 Keywords: inversion,inference,python package,geoscience,geophysics
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `geo-espresso-0.3.0.dev0/README.md` & `geo-espresso-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/Makefile` & `geo-espresso-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/_ext/generate_contrib_docs.py` & `geo-espresso-0.3.1/docs/source/_ext/generate_contrib_docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from pathlib import Path
-import importlib
 import sys
 
 import espresso
 
 
 # APV removed following as it is never used(?)
 # CONTRIBS = [nm for nm in dir(esp) if not nm.startswith("_") and nm[0].islower()]
```

### Comparing `geo-espresso-0.3.0.dev0/docs/source/_static/contrib_edit1.png` & `geo-espresso-0.3.1/docs/source/_static/contrib_edit1.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/_static/contrib_fork.png` & `geo-espresso-0.3.1/docs/source/_static/contrib_fork.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/_static/contrib_fork2.png` & `geo-espresso-0.3.1/docs/source/_static/contrib_fork2.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/_static/contrib_fork3.png` & `geo-espresso-0.3.1/docs/source/_static/contrib_fork3.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/_static/contrib_fork4.png` & `geo-espresso-0.3.1/docs/source/_static/contrib_fork4.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/_static/contrib_pr1.png` & `geo-espresso-0.3.1/docs/source/_static/contrib_pr1.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/_static/espresso_arch.svg` & `geo-espresso-0.3.1/docs/source/_static/espresso_arch.svg`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/_static/inlab_logo_60px.png` & `geo-espresso-0.3.1/docs/source/_static/inlab_logo_60px.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/_static/style.css` & `geo-espresso-0.3.1/docs/source/_static/style.css`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/_templates/autosummary/class.rst` & `geo-espresso-0.3.1/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/conf.py` & `geo-espresso-0.3.1/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     # build process.
     app.connect("builder-inited", run_autogen)
 
 
 # -- Project information -----------------------------------------------------
 project = 'Espresso'
 copyright = f"{datetime.date.today().year}, InLab, {project} development team"
-version = "dev" if "dev" in esp.__version__ else f"v{esp.__version__}"
+version = "dev" if "dev" in esp.__version__ else f"v{esp.__version__}".replace(".dirty", "")
 
 
 # -- General configuration ---------------------------------------------------
 sys.path.append(os.path.abspath("./_ext"))
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
@@ -70,15 +70,15 @@
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = [
     ".DS_Store",
     "user_guide/contrib/_index.rst",
-    "contributor_guide/contribute.rst",     # TODO migrate to new_contrib.rst
+    "user_guide/contrib/generated/*/examples/*",
 ]
 
 source_suffix = ".rst"
 source_encoding = "utf-8"
 master_doc = "index"
 pygments_style = "trac"        # https://pygments.org/styles/
 add_function_parentheses = False
```

### Comparing `geo-espresso-0.3.0.dev0/docs/source/contributor_guide/faq.rst` & `geo-espresso-0.3.1/docs/source/contributor_guide/faq.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/contributor_guide/github.rst` & `geo-espresso-0.3.1/docs/source/contributor_guide/github.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/contributor_guide/index.rst` & `geo-espresso-0.3.1/docs/source/contributor_guide/index.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/contributor_guide/new_contrib.rst` & `geo-espresso-0.3.1/docs/source/contributor_guide/new_contrib.rst`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
    * - 2
      - Move meta data files to ``_esp_build/``
      - ``shutil.copy``
    * - 3
      - Move ``src/`` content to ``_esp_build/src/espresso``
      - ``shutil.copytree``
    * - 4
-     - Move ``contrib/`` content to ``_esp_build/src/espresso/`` + ``_esp_build/src/espresso/__init__.py`` + ``_esp_build/src/espresso/list_problems.py``
+     - Move ``contrib/`` content to ``_esp_build/src/espresso/`` + ``_esp_build/src/espresso/__init__.py`` + ``_esp_build/src/espresso/capabilities.py``
      - ``shutil.copytree``, a series of file opening and string manipulation
    * - 5
      - Write dynamic version and extra versioningit configs into ``_esp_build/pyproject.toml``
      - ``versioningit``
    * - 6
      - Install package from ``_esp_build/``
      - ``pip install _esp_build``
```

### Comparing `geo-espresso-0.3.0.dev0/docs/source/contributor_guide/setup.rst` & `geo-espresso-0.3.1/docs/source/contributor_guide/setup.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/contributor_guide/submit.rst` & `geo-espresso-0.3.1/docs/source/contributor_guide/submit.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/contributor_guide/video.rst` & `geo-espresso-0.3.1/docs/source/contributor_guide/video.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/developer_guide/build.rst` & `geo-espresso-0.3.1/docs/source/developer_guide/build.rst`

 * *Files 1% similar despite different names*

```diff
@@ -44,17 +44,17 @@
 ``pip install .`` from ``_esp_build/`` folder. It does perform slight changes to the 
 files:
 
 #. Versioning template configured in ``setup.py`` is modified. Look at the 
    :ref:`versioning` section below for details.
 #. A prefix of ``_`` is added to all contribution folder names and Python file names
    to ensure cleaner tab completion results (e.g. from a iPython console)
-#. All example classes and names are collected into ``src/espresso/list_problems.py``
+#. All example classes and names are collected into ``src/espresso/capabilities.py``
 #. All examples are run by the build script with a timeout setting of 1 second per
-   method, to quickly build a capability matrix into ``src/espresso/list_problems.py``
+   method, to quickly build a capability matrix into ``src/espresso/capabilities.py``
 #. All examples with ``CMakeLists.txt`` files are recognized as having something to 
    build so the corresponding folders are added to the top-level ``CMakeLists.txt`` 
    file
 
 Implementation wise, 
 
 - Most steps of the build script use Python's inbuilt ``subprocess``, ``os``, ``sys``
```

### Comparing `geo-espresso-0.3.0.dev0/docs/source/developer_guide/ci.rst` & `geo-espresso-0.3.1/docs/source/developer_guide/ci.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/developer_guide/deploy.rst` & `geo-espresso-0.3.1/docs/source/developer_guide/deploy.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/developer_guide/develop.rst` & `geo-espresso-0.3.1/docs/source/developer_guide/develop.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/developer_guide/repository.rst` & `geo-espresso-0.3.1/docs/source/developer_guide/repository.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/index.rst` & `geo-espresso-0.3.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/user_guide/examples.rst` & `geo-espresso-0.3.1/docs/source/user_guide/examples.rst`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     niterations = 100
     epsilon = 0.01
 
     tp = testproblem(example_number = 1)
 
     model = tp.starting_model 
     for k in range(niterations):
-        predictions, G = tp.forward(model, with_jac = True)
+        predictions, G = tp.forward(model, with_jacobian = True)
         residuals = tp.data - predictions
         model -= epsilon * G.T.dot(residuals)
     print(model)
 
 The algorithm here is straightforward:
 
 .. math::
@@ -65,11 +65,11 @@
 
 We compute simulated data and the Jacobian for our current model estimate, and compare this to the 'data' embedded within our :py:class:`EspressoProblem`.
 
 .. code-block:: python
     :linenos:
     :lineno-start: 10
 
-        predictions, G = tp.forward(model, with_jac = True)
+        predictions, G = tp.forward(model, with_jacobian = True)
         residuals = tp.data - predictions
 
 Finally, we update the model accordingly, and iterate until (hopefully!) a good model is found.
```

### Comparing `geo-espresso-0.3.0.dev0/docs/source/user_guide/faq.rst` & `geo-espresso-0.3.1/docs/source/user_guide/faq.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/user_guide/index.rst` & `geo-espresso-0.3.1/docs/source/user_guide/index.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/user_guide/installation.rst` & `geo-espresso-0.3.1/docs/source/user_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/user_guide/usage.rst` & `geo-espresso-0.3.1/docs/source/user_guide/usage.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/docs/source/user_guide/why.rst` & `geo-espresso-0.3.1/docs/source/user_guide/why.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/pyproject.toml` & `geo-espresso-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/setup.py` & `geo-espresso-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/CMakeLists.txt` & `geo-espresso-0.3.1/src/espresso/CMakeLists.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 install(FILES __init__.py DESTINATION .)
 install(FILES _version.py DESTINATION .)
 install(FILES exceptions.py DESTINATION .)
 install(DIRECTORY utils DESTINATION .)
-install(DIRECTORY _magnetotelluric_1D DESTINATION .)
+install (DIRECTORY _machine DESTINATION .)
+install(DIRECTORY _xray_tracer DESTINATION .)
 install(DIRECTORY _slug_test DESTINATION .)
-install(DIRECTORY _fm_wavefront_tracker DESTINATION .)
-add_subdirectory(_fm_wavefront_tracker)
-install(DIRECTORY _gravity_density DESTINATION .)
 install(DIRECTORY _pumping_test DESTINATION .)
-install(DIRECTORY _xray_tracer DESTINATION .)
+install(DIRECTORY _gravity_density DESTINATION .)
+install(DIRECTORY _magnetotelluric_1D DESTINATION .)
+install(DIRECTORY _simple_regression DESTINATION .)
 install(DIRECTORY _receiver_function DESTINATION .)
 add_subdirectory(_receiver_function)
-install(DIRECTORY _simple_regression DESTINATION .)
+install(DIRECTORY _fm_wavefront_tracker DESTINATION .)
+add_subdirectory(_fm_wavefront_tracker)
```

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_espresso_problem.py` & `geo-espresso-0.3.1/src/espresso/_espresso_problem.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/CMakeLists.txt` & `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/LICENCE` & `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/README.md` & `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/__init__.py` & `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/__init__.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/_fm_wavefront_tracker.py` & `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/_fm_wavefront_tracker.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/datasets/cbmod.txt` & `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/cbmod.txt`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/receivers_InLab_lrt_r36.dat` & `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/receivers_InLab_lrt_r36.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/receivers_crossb_nwt_r10.dat` & `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/receivers_crossb_nwt_r10.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/sources_InLab_lrt_s500.dat` & `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/sources_InLab_lrt_s500.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/sources_crossb_nwt_s10.dat` & `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/sources_crossb_nwt_s10.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/ttimes_InLab_lrt_s500_r36.dat` & `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/ttimes_InLab_lrt_s500_r36.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/ttimes_crossb_nwt_s10_r10.dat` & `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/ttimes_crossb_nwt_s10_r10.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/fmst/compile` & `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/fmst/compile`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/fmst/src/fm2dss.f90` & `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/fmst/src/fm2dss.f90`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_fm_wavefront_tracker/waveTracker.py` & `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/waveTracker.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_gravity_density/LICENCE` & `geo-espresso-0.3.1/src/espresso/_gravity_density/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_gravity_density/README.md` & `geo-espresso-0.3.1/src/espresso/_gravity_density/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_gravity_density/_gravity_density.py` & `geo-espresso-0.3.1/src/espresso/_gravity_density/_gravity_density.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_gravity_density/metadata.yml` & `geo-espresso-0.3.1/src/espresso/_gravity_density/metadata.yml`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_machine/build_package/_utils.py` & `geo-espresso-0.3.1/src/espresso/_machine/build_package/_utils.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_machine/build_package/build.py` & `geo-espresso-0.3.1/src/espresso/_machine/build_package/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Build the Python package "espresso"
 
 1. clean "_esp_build/"
 2. "/<meta-data-files>" => "_esp_build/"
 3. generate "_version.py"
 4. "src/" => "_esp_build/src/"
-5. "contrib/" => "_esp_build/src/espresso/" + "__init__.py" + "list_problems.py"
+5. "contrib/" => "_esp_build/src/espresso/" + "__init__.py" + "capabilities.py"
 6. remove `.core` from versioningit_config
 7. "espresso_machine/" => _esp_build/src/_machine"
 8. build capability_matrix
 9. `pip install .`      (can be disabled by `--no-install`)
 
 Usage: python build.py [--pre] [--post] [--no-install] [-c <example_name>] [--file <file_name>]
 """
@@ -70,19 +70,23 @@
     if prefix is None:
         copytree(
             folder_path,
             dest_path,
             # dirs_exist_ok=True,
             ignore=ignore_patterns("*.pyc", "tmp*", "__pycache__"),
         )
-    else:           # moving contributions source
+    else:  # moving contributions source
         for f in os.listdir(folder_path):
             src = f"{folder_path}/{f}"
             dst = f"{dest_path}/{prefix}{f}"
-            if is_cache(f) or not os.path.isdir(src) or (only_include is not None and f not in only_include):
+            if (
+                is_cache(f)
+                or not os.path.isdir(src)
+                or (only_include is not None and f not in only_include)
+            ):
                 continue
             copytree(
                 src,
                 dst,
                 ignore=ignore_patterns(
                     "*.pyc",
                     "__pycache__",
@@ -161,46 +165,53 @@
         prefix="_",
         only_include=specified_problems,
     )
     # collect a list of contributions + related strings to write later
     contribs = []
     init_file_imports = "\n"
     init_file_all_cls = "\n_all_problems = [\n"
+    init_file_deletes = "\n"
     for path in Path(CONTRIB_SRC).iterdir():
         contrib = os.path.basename(path)  # name
         if path.is_dir() and (
             specified_problems is None or contrib in specified_problems
         ):
             contrib_class = _utils.problem_name_to_class(contrib)  # class
             contribs.append(contrib)
             init_file_imports += f"from ._{contrib} import {contrib_class}\n"
             init_file_all_cls += f"    {contrib_class},\n"
+            init_file_deletes += f"del {contrib_class}\n"
     init_file_all_cls += "]"
     # some constant strings to append to init file later
     init_file_imp_funcs = (
-        "\nfrom .list_problems import list_problem_names, list_problems"
+        "\nfrom .capabilities import list_problem_names, list_problems,"
+        " list_capabilities\n"
     )
     init_file_add_all_nms = "\n__all__ += list_problem_names()"
-    init_file_add_funcs = "\n__all__ += ['list_problem_names', 'list_problems']\n"
+    init_file_add_funcs = (
+        "\n__all__ += ['list_problem_names', 'list_problems', 'list_capabilities']\n"
+    )
     # write all above to files
     # compiled_code_list = set()
     with open(f"{BUILD_DIR}/src/{MODULE_NAME}/CMakeLists.txt", "a") as f:
+        f.write(f"install (DIRECTORY _machine DESTINATION .)\n")
         for contrib in contribs:
             f.write(f"install(DIRECTORY _{contrib} DESTINATION .)\n")
             if Path(f"{CONTRIB_SRC}/{contrib}/CMakeLists.txt").exists():
                 f.write(f"add_subdirectory(_{contrib})\n")
                 # compiled_code_list.add(contrib)
     with open(f"{BUILD_DIR}/src/{MODULE_NAME}/__init__.py", "a") as f:
         f.write(init_file_imports)
         f.write(init_file_imp_funcs)
         f.write(init_file_add_all_nms)
         f.write(init_file_add_funcs)
-    with open(f"{BUILD_DIR}/src/{MODULE_NAME}/list_problems.py", "a") as f:
+    with open(f"{BUILD_DIR}/src/{MODULE_NAME}/capabilities.py", "a") as f:
         f.write(init_file_imports)
         f.write(init_file_all_cls)
+        f.write(init_file_deletes)
     # with open(f"{ROOT_DIR}/contrib/{PROBLEMS_TO_COMPILE_FILE}", "w") as f:
     #     f.writelines(compiled_code_list)
 
 
 # 7 move espresso_machine into espresso/_machine
 def move_espresso_machine():
     move_folder_content(MACHINE_SRC, f"{BUILD_DIR}/src/espresso/_machine")
@@ -211,15 +222,15 @@
     # see if any contribution is specified through command line args
     specified_problems = _utils.problems_to_run_names_only()
     with _utils.suppress_stdout():
         capability_report = report.capability_report(
             problems_to_check=specified_problems
         )
     report_to_write = json.dumps(capability_report, indent=4)
-    with open(f"{BUILD_DIR}/src/{MODULE_NAME}/list_problems.py", "a") as f:
+    with open(f"{BUILD_DIR}/src/{MODULE_NAME}/capabilities.py", "a") as f:
         f.write("\n\n_capability_matrix = ")
         f.write(report_to_write)
 
 
 # printing helper
 def println_with_emoji(content, emoji):
     try:
@@ -243,15 +254,15 @@
     ),
     # ( install_pkg, "Building Python package: geo-espresso..." ),
 ]
 
 
 def build():
     println_with_emoji("Package building...", "🛠")
-    for (step, desc) in build_pipeline:
+    for step, desc in build_pipeline:
         println_with_emoji(desc, "🗂")
         try:
             step()
         except Exception as e:
             println_with_emoji(f"Problem occurred in this step: {desc}\n", "❗️")
             raise e
         print("OK.")
```

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_machine/build_package/check_requires.py` & `geo-espresso-0.3.1/src/espresso/_machine/build_package/check_requires.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_machine/build_package/conftest.py` & `geo-espresso-0.3.1/src/espresso/_machine/build_package/conftest.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_machine/build_package/criteria.py` & `geo-espresso-0.3.1/src/espresso/_machine/build_package/criteria.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_machine/build_package/report.py` & `geo-espresso-0.3.1/src/espresso/_machine/build_package/report.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_machine/build_package/run_examples.py` & `geo-espresso-0.3.1/src/espresso/_machine/build_package/run_examples.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_machine/build_package/test_examples.py` & `geo-espresso-0.3.1/src/espresso/_machine/build_package/test_examples.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_machine/build_package/validate.py` & `geo-espresso-0.3.1/src/espresso/_machine/build_package/validate.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_machine/doc_utils/gen_docs.py` & `geo-espresso-0.3.1/src/espresso/_machine/doc_utils/gen_docs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 r"""
-Module to contain funtions that help generate documentation
+Module to contain functions that help generate documentation
 """
 from pathlib import Path
 from shutil import copy
 import os
-import espresso as esp
+import espresso
 
 
 def read_metadata(contrib_name, lines):
     # - problem_title
     # - problem_short_description
     # - author_names
     # - contact_name
     # - contact_email
     # - [optional] citations -> []
     # - [optional] linked_sites -> [(name, link)]
     contrib_class_name = contrib_name.title().replace("_", "")
-    contrib_class = getattr(esp, contrib_class_name)
+    contrib_class = getattr(espresso, contrib_class_name)
     class_metadata = contrib_class.metadata
     lines.append(":::{admonition} Contribution Metadata for ")
     lines[-1] += "*" + class_metadata["problem_title"] + "* \n:class: important"
     # metadata - short description
     lines.append(class_metadata["problem_short_description"])
     lines.append("```{eval-rst}")
     # metadata - authors
@@ -56,41 +56,84 @@
             for (name, link) in class_metadata["linked_sites"]:
                 lines.append(f"  - [{name}]({link})")
     # ending
     lines.append("```")
     lines.append(":::")
 
 
+def write_sample_code(class_name, name, lines):
+    capabilities = espresso.list_capabilities(class_name)[class_name]
+    problem_var_name = f"my{name}"
+    lines.append(f"## Example usage for `{class_name}` \n")
+    with open(Path(__file__).resolve().parent / "_sample_code.txt", "r") as f:
+        optional = False
+        for line in f:
+            if "Optional API" in line:
+                optional = True
+            if "<problem_var_name>." in line:
+                attr_name = line.split("<problem_var_name>.")[1].split("(")[0].strip()
+                if attr_name not in capabilities and optional:
+                    continue
+                elif attr_name in capabilities:
+                    capabilities.remove(attr_name)
+            line = line.replace("<problem_var_name>", problem_var_name)
+            line = line.replace("<class_name>", class_name)
+            lines.append(line.strip())
+    if capabilities:
+        additional_api = f"Additional attributes to explore: {capabilities}."
+        additional_api = additional_api.replace("'", "`")
+        lines.append(additional_api)
+
+
+def write_example_files(contrib_dir, dest_contrib_dir, lines):
+    if "examples" in os.listdir(contrib_dir):
+        lines.append("## Example files \n")
+        for file_name in os.listdir(contrib_dir / "examples"):
+            if file_name.endswith(".pyc") or file_name == "__pycache__":
+                continue
+            link_file(contrib_dir / "examples", dest_contrib_dir, file_name, lines)
+    
+
 def read_file(contrib_dir, dest_contrib_dir, file_name, lines):
     src_path = contrib_dir / file_name
     dst_path = dest_contrib_dir / file_name
     copy(src_path, dst_path)
-    lines.append("```{include} ./" + file_name + "\n```")
+    lines.append("```{include} ./" + file_name + "\n```\n")
+
+
+def link_file(contrib_dir, dest_contrib_dir, file_name, lines):
+    src_path = contrib_dir / file_name
+    dst_path = dest_contrib_dir / "examples" / file_name
+    os.makedirs(dest_contrib_dir / "examples", exist_ok=True)
+    copy(src_path, dst_path)
+    lines.append("- {download}" + f"`examples/{file_name}`")
 
 
 def contribs(BASE_PATH, DEST_PATH):
-    names = [cls.__module__.split(".")[-1] for cls in esp.list_problems()]
+    names = [cls.__module__.split(".")[-1] for cls in espresso.list_problems()]
+    class_names = espresso.list_problem_names()
     all_contribs = [
         (contrib, Path(f"{BASE_PATH}/{contrib}"), Path(f"{DEST_PATH}/{contrib}"))
         for contrib in names
     ]
     all_contribs = [
         contrib
         for contrib in all_contribs
         if contrib[1].exists() and contrib[1].is_dir()
     ]
-    return all_contribs
+    return zip(all_contribs, class_names)
 
 
 def gen_contrib_docs(BASE_PATH, DEST_PATH):
     os.mkdir(DEST_PATH)
     # prepare index file
     index_lines = []
     # move info for each contribution
-    for (contrib, src_folder, dst_folder) in contribs(BASE_PATH, DEST_PATH):
+    for (contrib, src_folder, dst_folder), class_name in \
+        contribs(BASE_PATH, DEST_PATH):
         # make new folder docs/source/contrib/<contrib-name>
         os.mkdir(dst_folder)
         lines = []
         # Provide hint about where this file came from
         lines.append(
             "<!--- This file was automatically generated by \n"
             "      _ext/generate_contrib_docs.py based on the\n"
@@ -98,14 +141,18 @@
             "      README.md and LICENCE. \n"
             "-->\n\n"
         )
         # include README.md
         read_file(src_folder, dst_folder, "README.md", lines)
         # format metadata content
         read_metadata(contrib, lines)
+        # format sample code based on capability matrix
+        write_sample_code(class_name, contrib, lines)
+        # format example files (if any)
+        write_example_files(src_folder, dst_folder, lines)
         # include LICENCE
         lines.append("\n## LICENCE\n")
         read_file(src_folder, dst_folder, "LICENCE", lines)
         # write to index.md file
         with open(f"{dst_folder}/index.md", "w") as f:
             f.write("\n".join(lines))
         # add contrib link to contrib/index.rst
```

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_machine/new_contribution/_template/LICENCE` & `geo-espresso-0.3.1/src/espresso/_machine/new_contribution/_template/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_machine/new_contribution/_template/example_name.py` & `geo-espresso-0.3.1/src/espresso/_machine/new_contribution/_template/example_name.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_machine/new_contribution/create_new_contrib.py` & `geo-espresso-0.3.1/src/espresso/_machine/new_contribution/create_new_contrib.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/LICENCE` & `geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/README.md` & `geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/__init__.py` & `geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/__init__.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/_magnetotelluric_1D.py` & `geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/_magnetotelluric_1D.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/data/16-A_KN2.dat` & `geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/data/16-A_KN2.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/examples/example_01.ipynb` & `geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/example_01.ipynb`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/examples/example_01.py` & `geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/example_01.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/examples/field_MT.ipynb` & `geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/field_MT.ipynb`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/examples/field_MT.py` & `geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/field_MT.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.ipynb` & `geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.ipynb`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.py` & `geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_pumping_test/LICENCE` & `geo-espresso-0.3.1/src/espresso/_pumping_test/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_pumping_test/README.md` & `geo-espresso-0.3.1/src/espresso/_pumping_test/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_pumping_test/_pumping_test.py` & `geo-espresso-0.3.1/src/espresso/_pumping_test/_pumping_test.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/CMakeLists.txt` & `geo-espresso-0.3.1/src/espresso/_receiver_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/LICENCE` & `geo-espresso-0.3.1/src/espresso/_receiver_function/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/README.md` & `geo-espresso-0.3.1/src/espresso/_receiver_function/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/RF.f90` & `geo-espresso-0.3.1/src/espresso/_receiver_function/RF.f90`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/RFsubs/dsvdcmp.f` & `geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/dsvdcmp.f`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/RFsubs/four1.f` & `geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/four1.f`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/RFsubs/qlayer.f` & `geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/qlayer.f`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/RFsubs/ran3.f` & `geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/ran3.f`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/RFsubs/svbksb.f` & `geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/svbksb.f`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/RFsubs/theo.f` & `geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/theo.f`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/RFsubs/theo_noise.f` & `geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/theo_noise.f`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/RFsubs/voro2qmodel.f90` & `geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/voro2qmodel.f90`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/__init__.py` & `geo-espresso-0.3.1/src/espresso/_receiver_function/__init__.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/_receiver_function.py` & `geo-espresso-0.3.1/src/espresso/_receiver_function/_receiver_function.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_receiver_function/rf.py` & `geo-espresso-0.3.1/src/espresso/_receiver_function/rf.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_simple_regression/LICENCE` & `geo-espresso-0.3.1/src/espresso/_simple_regression/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_simple_regression/_simple_regression.py` & `geo-espresso-0.3.1/src/espresso/_simple_regression/_simple_regression.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_slug_test/LICENCE` & `geo-espresso-0.3.1/src/espresso/_slug_test/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_slug_test/README.md` & `geo-espresso-0.3.1/src/espresso/_slug_test/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_slug_test/_slug_test.py` & `geo-espresso-0.3.1/src/espresso/_slug_test/_slug_test.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_xray_tracer/LICENCE` & `geo-espresso-0.3.1/src/espresso/_xray_tracer/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_xray_tracer/README.md` & `geo-espresso-0.3.1/src/espresso/_xray_tracer/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_xray_tracer/_xray_tracer.py` & `geo-espresso-0.3.1/src/espresso/_xray_tracer/_xray_tracer.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_xray_tracer/data/csiro_logo.png` & `geo-espresso-0.3.1/src/espresso/_xray_tracer/data/csiro_logo.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_xray_tracer/data/example1.dat` & `geo-espresso-0.3.1/src/espresso/_xray_tracer/data/example1.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_xray_tracer/data/example2.dat` & `geo-espresso-0.3.1/src/espresso/_xray_tracer/data/example2.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_xray_tracer/data/example3.dat` & `geo-espresso-0.3.1/src/espresso/_xray_tracer/data/example3.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/_xray_tracer/data/inlab_logo.png` & `geo-espresso-0.3.1/src/espresso/_xray_tracer/data/inlab_logo.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/exceptions.py` & `geo-espresso-0.3.1/src/espresso/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+"""
+===================
+Espresso exceptions
+===================
+
+Submodule for Espresso exceptions.
+
+"""
+
 class EspressoError(Exception):
     """Base class for all Espresso errors
     """
     pass
 
 # Multiple inheritance means this can be caught by all of the following:
 # ... except InvalidExampleError
@@ -31,9 +40,7 @@
         msg = "Unrecognised example number.\n\nPlease refer to the Espresso documentation " \
               "(https://geo-espresso.readthedocs.io/)\nfor full details of the examples " \
               "provided within this test problem."
         if len(super_msg)>0:
             return msg+"\n\n"+super_msg
         else:
             return msg
-
-
```

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/list_problems.py` & `geo-espresso-0.3.1/src/espresso/capabilities.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,55 @@
+"""
+=======================
+Understand capabilities
+=======================
+
+Submodule for listing capabilities in Espresso problems.
+
+To programatically see what problems are available in Espresso, these functions are 
+helpful:
+
+"""
+
+import typing
+
 _all_problems = []
 _capability_matrix = dict()
 
 def list_problem_names(capabilities: list = None):
-    """Returns a list of all Espresso problem names"""
+    """Returns a list of all Espresso problem names
+    
+    Parameters
+    ----------
+    capabilities : list
+        a list of strings to filter the problem names, default to None
+    
+    Examples
+    --------
+    >>> import espresso
+    >>> problem_names = espresso.list_problem_names()
+    """
     _problems = list_problems(capabilities)
     _all_names = [p.__name__ for p in _problems]
     return _all_names
 
 def list_problems(capabilities: list = None):
-    """Returns a list of all Espresso problem classes"""
+    """Returns a list of all Espresso problem classes
+    
+    Parameters
+    ----------
+    capabilities : list
+        a list of strings to filter the problem classes, default to None
+    
+    Examples
+    --------
+    >>> import espresso
+    >>> problems = espresso.list_problems()
+    >>> problems_with_model_plotting = epsresso.list_problems(['plot_model']])
+    """
     if capabilities is None:
         return _all_problems
     elif not isinstance(capabilities, (list, set, tuple)):
         raise ValueError(
             "pass in a list of capabilities, e.g. "
             "`espresso.list_problems(['plot_model'])"
         )
@@ -28,16 +65,37 @@
                 _problem_names.append(p)
         _problems = []
         for p in _all_problems:
             if p.__name__ in _problem_names:
                 _problems.append(p)
         return _problems
 
-def list_capability(problem_names: list) -> dict:
-    return {k:v for k,v in _capability_matrix.items() if k in problem_names}
+def list_capabilities(problem_names: typing.Union[list, str] = None) -> dict:
+    """Returns a dictionary of capabilities filtered by problem names
+    
+    Parameters
+    ----------
+    problem_names : list
+        a list of strings of problem names, default to None
+    
+    Examples
+    --------
+    >>> import espresso
+    >>> capabilities = espresso.list_capabilities(['SimpleRegression'])
+    """
+    all_capabilities = dict()
+    for problem, report in _capability_matrix.items():
+        all_capabilities[problem] = [k for k, v in report.items() if v == 1]
+    if problem_names is None:
+        return all_capabilities
+    else:
+        problem_names = [problem_names] if isinstance(problem_names, str) else problem_names
+        filtered_capabilities = {k: v for k,v in all_capabilities.items() if k in problem_names}
+        return filtered_capabilities
+
 
 # from .example_name import ExampleName
 
 # _all_problems = [ ExampleName, ]
 
 # _capability_matrix = {
 #     "ExampleName": {
@@ -45,54 +103,60 @@
 #         "data_size": 1,
 #         "starting_model": 1,
 #         ...
 #     },
 #     ...
 # }
 
-from ._magnetotelluric_1D import Magnetotelluric1D
+from ._xray_tracer import XrayTracer
 from ._slug_test import SlugTest
-from ._fm_wavefront_tracker import FmWavefrontTracker
-from ._gravity_density import GravityDensity
 from ._pumping_test import PumpingTest
-from ._xray_tracer import XrayTracer
-from ._receiver_function import ReceiverFunction
+from ._gravity_density import GravityDensity
+from ._magnetotelluric_1D import Magnetotelluric1D
 from ._simple_regression import SimpleRegression
+from ._receiver_function import ReceiverFunction
+from ._fm_wavefront_tracker import FmWavefrontTracker
 
 _all_problems = [
-    Magnetotelluric1D,
+    XrayTracer,
     SlugTest,
-    FmWavefrontTracker,
-    GravityDensity,
     PumpingTest,
-    XrayTracer,
-    ReceiverFunction,
+    GravityDensity,
+    Magnetotelluric1D,
     SimpleRegression,
+    ReceiverFunction,
+    FmWavefrontTracker,
 ]
+del XrayTracer
+del SlugTest
+del PumpingTest
+del GravityDensity
+del Magnetotelluric1D
+del SimpleRegression
+del ReceiverFunction
+del FmWavefrontTracker
+
 
 _capability_matrix = {
-    "Magnetotelluric1D": {
+    "XrayTracer": {
         "model_size": 1,
         "data_size": 1,
         "good_model": 1,
         "starting_model": 1,
         "data": 1,
-        "forward": 1,
+        "forward": 0,
         "description": 1,
-        "covariance_matrix": 1,
-        "inverse_covariance_matrix": 1,
-        "jacobian": 1,
+        "covariance_matrix": 0,
+        "inverse_covariance_matrix": 0,
+        "jacobian": 0,
         "plot_model": 1,
-        "plot_data": 1,
-        "misfit": 1,
+        "plot_data": 0,
+        "misfit": 0,
         "log_likelihood": 0,
-        "log_prior": 0,
-        "set_start_model": 1,
-        "set_start_mesh": 1,
-        "set_obs_data": 1
+        "log_prior": 0
     },
     "SlugTest": {
         "model_size": 1,
         "data_size": 1,
         "good_model": 1,
         "starting_model": 1,
         "data": 1,
@@ -103,34 +167,30 @@
         "jacobian": 0,
         "plot_model": 1,
         "plot_data": 0,
         "misfit": 0,
         "log_likelihood": 1,
         "log_prior": 0
     },
-    "FmWavefrontTracker": {
+    "PumpingTest": {
         "model_size": 1,
         "data_size": 1,
         "good_model": 1,
         "starting_model": 1,
         "data": 1,
-        "forward": 1,
-        "description": 0,
-        "covariance_matrix": 0,
-        "inverse_covariance_matrix": 0,
-        "jacobian": 1,
+        "forward": 0,
+        "description": 1,
+        "covariance_matrix": 1,
+        "inverse_covariance_matrix": 1,
+        "jacobian": 0,
         "plot_model": 1,
         "plot_data": 0,
         "misfit": 0,
-        "log_likelihood": 0,
-        "log_prior": 0,
-        "clean_tmp_files": 1,
-        "tmp_files": 1,
-        "tmp_paths": 1,
-        "exe_fm2dss": 1
+        "log_likelihood": 1,
+        "log_prior": 0
     },
     "GravityDensity": {
         "model_size": 1,
         "data_size": 1,
         "good_model": 1,
         "starting_model": 1,
         "data": 1,
@@ -141,43 +201,46 @@
         "jacobian": 1,
         "plot_model": 1,
         "plot_data": 1,
         "misfit": 0,
         "log_likelihood": 0,
         "log_prior": 0
     },
-    "PumpingTest": {
+    "Magnetotelluric1D": {
         "model_size": 1,
         "data_size": 1,
         "good_model": 1,
         "starting_model": 1,
         "data": 1,
-        "forward": 0,
+        "forward": 1,
         "description": 1,
         "covariance_matrix": 1,
         "inverse_covariance_matrix": 1,
-        "jacobian": 0,
+        "jacobian": 1,
         "plot_model": 1,
-        "plot_data": 0,
-        "misfit": 0,
-        "log_likelihood": 1,
-        "log_prior": 0
+        "plot_data": 1,
+        "misfit": 1,
+        "log_likelihood": 0,
+        "log_prior": 0,
+        "set_start_model": 1,
+        "set_obs_data": 1,
+        "set_start_mesh": 1
     },
-    "XrayTracer": {
+    "SimpleRegression": {
         "model_size": 1,
         "data_size": 1,
         "good_model": 1,
         "starting_model": 1,
         "data": 1,
-        "forward": 0,
+        "forward": 1,
         "description": 1,
-        "covariance_matrix": 0,
-        "inverse_covariance_matrix": 0,
-        "jacobian": 0,
-        "plot_model": 1,
+        "covariance_matrix": 1,
+        "inverse_covariance_matrix": 1,
+        "jacobian": 1,
+        "plot_model": 0,
         "plot_data": 0,
         "misfit": 0,
         "log_likelihood": 0,
         "log_prior": 0
     },
     "ReceiverFunction": {
         "model_size": 1,
@@ -193,25 +256,29 @@
         "plot_model": 1,
         "plot_data": 1,
         "misfit": 0,
         "log_likelihood": 1,
         "log_prior": 1,
         "rf": 1
     },
-    "SimpleRegression": {
+    "FmWavefrontTracker": {
         "model_size": 1,
         "data_size": 1,
         "good_model": 1,
         "starting_model": 1,
         "data": 1,
         "forward": 1,
-        "description": 1,
-        "covariance_matrix": 1,
-        "inverse_covariance_matrix": 1,
+        "description": 0,
+        "covariance_matrix": 0,
+        "inverse_covariance_matrix": 0,
         "jacobian": 1,
-        "plot_model": 0,
+        "plot_model": 1,
         "plot_data": 0,
         "misfit": 0,
         "log_likelihood": 0,
-        "log_prior": 0
+        "log_prior": 0,
+        "tmp_paths": 1,
+        "clean_tmp_files": 1,
+        "tmp_files": 1,
+        "exe_fm2dss": 1
     }
 }
```

### Comparing `geo-espresso-0.3.0.dev0/src/espresso/utils/data_loader.py` & `geo-espresso-0.3.1/src/espresso/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.0.dev0/src/geo_espresso.egg-info/PKG-INFO` & `geo-espresso-0.3.1/src/geo_espresso.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-espresso
-Version: 0.3.0.dev0
+Version: 0.3.1
 Summary: Earth Science PRoblems for the Evaluation of Strategies, Solvers and Optimizers
 Author: InLab, Espresso development team
 Keywords: inversion,inference,python package,geoscience,geophysics
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `geo-espresso-0.3.0.dev0/src/geo_espresso.egg-info/SOURCES.txt` & `geo-espresso-0.3.1/src/geo_espresso.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,16 @@
 docs/source/user_guide/why.rst
 docs/source/user_guide/api/index.rst
 docs/source/user_guide/contrib/_index.rst
 src/espresso/CMakeLists.txt
 src/espresso/__init__.py
 src/espresso/_espresso_problem.py
 src/espresso/_version.py
+src/espresso/capabilities.py
 src/espresso/exceptions.py
-src/espresso/list_problems.py
 src/espresso/version.py
 src/espresso/_fm_wavefront_tracker/.gitignore
 src/espresso/_fm_wavefront_tracker/CMakeLists.txt
 src/espresso/_fm_wavefront_tracker/LICENCE
 src/espresso/_fm_wavefront_tracker/README.md
 src/espresso/_fm_wavefront_tracker/__init__.py
 src/espresso/_fm_wavefront_tracker/_fm_wavefront_tracker.py
@@ -87,14 +87,15 @@
 src/espresso/_machine/build_package/conftest.py
 src/espresso/_machine/build_package/criteria.py
 src/espresso/_machine/build_package/report.py
 src/espresso/_machine/build_package/run_examples.py
 src/espresso/_machine/build_package/test_examples.py
 src/espresso/_machine/build_package/validate.py
 src/espresso/_machine/doc_utils/__init__.py
+src/espresso/_machine/doc_utils/_sample_code.txt
 src/espresso/_machine/doc_utils/gen_docs.py
 src/espresso/_machine/new_contribution/create_new_contrib.py
 src/espresso/_machine/new_contribution/_template/LICENCE
 src/espresso/_machine/new_contribution/_template/README.md
 src/espresso/_machine/new_contribution/_template/__init__.py
 src/espresso/_machine/new_contribution/_template/example_name.py
 src/espresso/_machine/new_contribution/_template/data/__init__.py
```

