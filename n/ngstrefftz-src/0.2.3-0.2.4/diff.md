# Comparing `tmp/ngstrefftz-src-0.2.3.tar.gz` & `tmp/ngstrefftz-src-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngstrefftz-src-0.2.3.tar", last modified: Thu Apr 27 13:47:46 2023, max compression
+gzip compressed data, was "ngstrefftz-src-0.2.4.tar", last modified: Fri Apr 28 13:08:50 2023, max compression
```

## Comparing `ngstrefftz-src-0.2.3.tar` & `ngstrefftz-src-0.2.4.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:47:46.364179 ngstrefftz-src-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-27 13:47:46.364179 ngstrefftz-src-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:47:46.356179 ngstrefftz-src-0.2.3/external_dependencies/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:47:46.360179 ngstrefftz-src-0.2.3/external_dependencies/ngstents/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:47:46.360179 ngstrefftz-src-0.2.3/external_dependencies/ngstents/py/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/py/_drawtents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/py/ctau_experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/py/tentinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:47:46.360179 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/advection.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/burgers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   133375 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/concurrentqueue.h
--rw-r--r--   0 runner    (1001) docker     (123)    17116 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/conservationlaw.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15095 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/euler.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/maxwell.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/paralleldepend.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/python_conslaw.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/python_tents.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/symbolic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    31227 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    47723 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/tents.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13363 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/tents.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/tentsolver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/tentsolver_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/vis3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/vis3d.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/wave.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:47:46.356179 ngstrefftz-src-0.2.3/ngstrefftz_src.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-27 13:47:46.000000 ngstrefftz-src-0.2.3/ngstrefftz_src.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-27 13:47:46.000000 ngstrefftz-src-0.2.3/ngstrefftz_src.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:47:46.000000 ngstrefftz-src-0.2.3/ngstrefftz_src.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 13:47:46.000000 ngstrefftz-src-0.2.3/ngstrefftz_src.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 13:47:46.000000 ngstrefftz-src-0.2.3/ngstrefftz_src.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 13:47:46.364179 ngstrefftz-src-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:47:46.360179 ngstrefftz-src-0.2.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/airy.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/diffopmapped.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    25648 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/embtrefftz.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/embtrefftz.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/intrule4.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/mesh1dtents.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/mesh1dtents.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/monomialfespace.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/monomialfespace.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/planewavefe.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/planewavefe.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/python_trefftz.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    48909 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/scalarmappedfe.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15001 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/scalarmappedfe.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/specialcoefficientfunction.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/specialcoefficientfunction.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    38072 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/trefftzfespace.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/trefftzfespace.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    43502 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/twavetents.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/twavetents.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:47:46.360179 ngstrefftz-src-0.2.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/test/embt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/test/tents.py
--rw-r--r--   0 runner    (1001) docker     (123)    20932 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/test/trefftz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/test/twave.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:08:50.578526 ngstrefftz-src-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-28 13:08:50.578526 ngstrefftz-src-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:08:50.570526 ngstrefftz-src-0.2.4/external_dependencies/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:08:50.574526 ngstrefftz-src-0.2.4/external_dependencies/ngstents/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-28 13:08:01.000000 ngstrefftz-src-0.2.4/external_dependencies/ngstents/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:08:50.578526 ngstrefftz-src-0.2.4/external_dependencies/ngstents/py/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-28 13:08:01.000000 ngstrefftz-src-0.2.4/external_dependencies/ngstents/py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-28 13:08:01.000000 ngstrefftz-src-0.2.4/external_dependencies/ngstents/py/_drawtents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-28 13:08:01.000000 ngstrefftz-src-0.2.4/external_dependencies/ngstents/py/ctau_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-28 13:08:01.000000 ngstrefftz-src-0.2.4/external_dependencies/ngstents/py/tentinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:08:50.578526 ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-28 13:08:01.000000 ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-28 13:08:01.000000 ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/advection.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-28 13:08:01.000000 ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/burgers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   133375 2023-04-28 13:08:01.000000 ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/concurrentqueue.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17116 2023-04-28 13:08:01.000000 ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/conservationlaw.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15095 2023-04-28 13:08:01.000000 ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/euler.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-04-28 13:08:01.000000 ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/maxwell.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-28 13:08:01.000000 ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/paralleldepend.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-04-28 13:08:01.000000 ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/python_conslaw.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-04-28 13:08:01.000000 ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/python_tents.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-04-28 13:08:01.000000 ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/symbolic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31227 2023-04-28 13:08:01.000000 ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    47723 2023-04-28 13:08:01.000000 ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/tents.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13363 2023-04-28 13:08:01.000000 ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/tents.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-28 13:08:01.000000 ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/tentsolver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-04-28 13:08:01.000000 ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/tentsolver_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-04-28 13:08:01.000000 ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/vis3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-28 13:08:01.000000 ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/vis3d.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-04-28 13:08:01.000000 ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/wave.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:08:50.570526 ngstrefftz-src-0.2.4/ngstrefftz_src.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-28 13:08:50.000000 ngstrefftz-src-0.2.4/ngstrefftz_src.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-28 13:08:50.000000 ngstrefftz-src-0.2.4/ngstrefftz_src.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:08:50.000000 ngstrefftz-src-0.2.4/ngstrefftz_src.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 13:08:50.000000 ngstrefftz-src-0.2.4/ngstrefftz_src.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-28 13:08:50.000000 ngstrefftz-src-0.2.4/ngstrefftz_src.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 13:08:50.578526 ngstrefftz-src-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:08:50.574526 ngstrefftz-src-0.2.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/src/airy.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/src/diffopmapped.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25648 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/src/embtrefftz.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/src/embtrefftz.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/src/intrule4.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/src/mesh1dtents.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/src/mesh1dtents.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/src/monomialfespace.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/src/monomialfespace.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/src/planewavefe.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/src/planewavefe.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/src/python_trefftz.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    48909 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/src/scalarmappedfe.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15001 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/src/scalarmappedfe.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/src/specialcoefficientfunction.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/src/specialcoefficientfunction.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    38072 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/src/trefftzfespace.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/src/trefftzfespace.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    43502 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/src/twavetents.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/src/twavetents.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:08:50.578526 ngstrefftz-src-0.2.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/test/embt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/test/tents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20932 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/test/trefftz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-28 13:08:00.000000 ngstrefftz-src-0.2.4/test/twave.py
```

### Comparing `ngstrefftz-src-0.2.3/LICENSE` & `ngstrefftz-src-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/PKG-INFO` & `ngstrefftz-src-0.2.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngstrefftz-src
-Version: 0.2.3
+Version: 0.2.4
 Summary: NGSTrefftz is an add-on to NGSolve for Trefftz methods.
 Home-page: https://github.com/PaulSt/ngstrefftz
 Author: Paul Stocker
 Author-email: p.stocker@math.uni-goettingen.de
 Requires-Python: >=3.8
 License-File: LICENSE
```

### Comparing `ngstrefftz-src-0.2.3/README.md` & `ngstrefftz-src-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/external_dependencies/ngstents/README.md` & `ngstrefftz-src-0.2.4/external_dependencies/ngstents/README.md`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/external_dependencies/ngstents/py/_drawtents.py` & `ngstrefftz-src-0.2.4/external_dependencies/ngstents/py/_drawtents.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/external_dependencies/ngstents/py/ctau_experiments.py` & `ngstrefftz-src-0.2.4/external_dependencies/ngstents/py/ctau_experiments.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/external_dependencies/ngstents/py/tentinfo.py` & `ngstrefftz-src-0.2.4/external_dependencies/ngstents/py/tentinfo.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/CMakeLists.txt` & `ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/advection.cpp` & `ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/advection.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/burgers.cpp` & `ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/burgers.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/concurrentqueue.h` & `ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/concurrentqueue.h`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/conservationlaw.hpp` & `ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/conservationlaw.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/euler.cpp` & `ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/euler.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/maxwell.cpp` & `ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/maxwell.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/paralleldepend.hpp` & `ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/paralleldepend.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/python_conslaw.cpp` & `ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/python_conslaw.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/python_tents.cpp` & `ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/python_tents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/symbolic.cpp` & `ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/symbolic.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp` & `ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/tents.cpp` & `ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/tents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/tents.hpp` & `ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/tents.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/tentsolver.hpp` & `ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/tentsolver.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/tentsolver_impl.hpp` & `ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/tentsolver_impl.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/vis3d.cpp` & `ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/vis3d.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/vis3d.hpp` & `ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/vis3d.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/wave.cpp` & `ngstrefftz-src-0.2.4/external_dependencies/ngstents/src/wave.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/ngstrefftz_src.egg-info/PKG-INFO` & `ngstrefftz-src-0.2.4/ngstrefftz_src.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngstrefftz-src
-Version: 0.2.3
+Version: 0.2.4
 Summary: NGSTrefftz is an add-on to NGSolve for Trefftz methods.
 Home-page: https://github.com/PaulSt/ngstrefftz
 Author: Paul Stocker
 Author-email: p.stocker@math.uni-goettingen.de
 Requires-Python: >=3.8
 License-File: LICENSE
```

### Comparing `ngstrefftz-src-0.2.3/ngstrefftz_src.egg-info/SOURCES.txt` & `ngstrefftz-src-0.2.4/ngstrefftz_src.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/setup.py` & `ngstrefftz-src-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/src/CMakeLists.txt` & `ngstrefftz-src-0.2.4/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/src/__init__.py` & `ngstrefftz-src-0.2.4/src/__init__.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/src/airy.cpp` & `ngstrefftz-src-0.2.4/src/airy.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/src/diffopmapped.hpp` & `ngstrefftz-src-0.2.4/src/diffopmapped.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/src/embtrefftz.cpp` & `ngstrefftz-src-0.2.4/src/embtrefftz.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/src/embtrefftz.hpp` & `ngstrefftz-src-0.2.4/src/embtrefftz.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/src/intrule4.cpp` & `ngstrefftz-src-0.2.4/src/intrule4.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/src/mesh1dtents.cpp` & `ngstrefftz-src-0.2.4/src/mesh1dtents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/src/monomialfespace.cpp` & `ngstrefftz-src-0.2.4/src/monomialfespace.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -147,10 +147,10 @@
 #ifdef NGS_PYTHON
 void ExportMonomialFESpace (py::module m)
 {
   using namespace ngcomp;
 
   ExportFESpace<MonomialFESpace> (m, "monomialfespace")
       .def ("GetDocu", &MonomialFESpace::GetDocu)
-      .def ("SetWavespeed", &MonomialFESpace::SetWavespeed);
+      .def ("SetCoeff", &MonomialFESpace::SetCoeff);
 }
 #endif // NGS_PYTHON
```

### Comparing `ngstrefftz-src-0.2.3/src/monomialfespace.hpp` & `ngstrefftz-src-0.2.4/src/monomialfespace.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -9,24 +9,24 @@
   class MonomialFESpace : public FESpace
   {
     int D;
     int order;
     int nel;
     int local_ndof;
     int useshift = 1;
-    shared_ptr<CoefficientFunction> wavespeedcf;
+    shared_ptr<CoefficientFunction> coeff_cf = nullptr;
     CSR basismat;
 
   public:
     MonomialFESpace (shared_ptr<MeshAccess> ama, const Flags &flags,
                      bool checkflags = false);
 
-    void SetWavespeed (shared_ptr<CoefficientFunction> awavespeedcf)
+    void SetCoeff (shared_ptr<CoefficientFunction> acoeff_cf)
     {
-      wavespeedcf = awavespeedcf;
+      coeff_cf = acoeff_cf;
     }
 
     string GetClassName () const override { return "monomialfespace"; }
 
     void Update () override;
 
     void GetDofNrs (ElementId ei, Array<DofId> &dnums) const override;
@@ -65,17 +65,17 @@
             {
               Vec<D> v1 = ma->GetPoint<D> (vertex1);
               Vec<D> v2 = ma->GetPoint<D> (vertex2);
               IntegrationRule ir (ma->GetElType (ei), 0);
               ElementTransformation &trafo = ma->GetTrafo (ei, lh);
               MappedIntegrationPoint<D, D> mip (ir[0], trafo);
               mip.Point () = v1;
-              double c1 = wavespeedcf ? wavespeedcf->Evaluate (mip) : 1.0;
+              double c1 = coeff_cf ? coeff_cf->Evaluate (mip) : 1.0;
               mip.Point () = v2;
-              double c2 = wavespeedcf ? wavespeedcf->Evaluate (mip) : 1.0;
+              double c2 = coeff_cf ? coeff_cf->Evaluate (mip) : 1.0;
 
               anisotropicdiam = max (
                   anisotropicdiam,
                   sqrt (L2Norm2 (v1.Range (0, D - 1) - v2.Range (0, D - 1))
                         + pow (c1 * v1 (D - 1) - c2 * v2 (D - 1), 2)));
             }
         }
```

### Comparing `ngstrefftz-src-0.2.3/src/planewavefe.cpp` & `ngstrefftz-src-0.2.4/src/planewavefe.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/src/planewavefe.hpp` & `ngstrefftz-src-0.2.4/src/planewavefe.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/src/python_trefftz.cpp` & `ngstrefftz-src-0.2.4/src/python_trefftz.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/src/scalarmappedfe.cpp` & `ngstrefftz-src-0.2.4/src/scalarmappedfe.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/src/scalarmappedfe.hpp` & `ngstrefftz-src-0.2.4/src/scalarmappedfe.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/src/specialcoefficientfunction.cpp` & `ngstrefftz-src-0.2.4/src/specialcoefficientfunction.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/src/specialcoefficientfunction.hpp` & `ngstrefftz-src-0.2.4/src/specialcoefficientfunction.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/src/trefftzfespace.cpp` & `ngstrefftz-src-0.2.4/src/trefftzfespace.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/src/trefftzfespace.hpp` & `ngstrefftz-src-0.2.4/src/trefftzfespace.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/src/twavetents.cpp` & `ngstrefftz-src-0.2.4/src/twavetents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/src/twavetents.hpp` & `ngstrefftz-src-0.2.4/src/twavetents.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/test/embt.py` & `ngstrefftz-src-0.2.4/test/embt.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/test/tents.py` & `ngstrefftz-src-0.2.4/test/tents.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/test/trefftz.py` & `ngstrefftz-src-0.2.4/test/trefftz.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.3/test/twave.py` & `ngstrefftz-src-0.2.4/test/twave.py`

 * *Files identical despite different names*

