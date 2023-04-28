# Comparing `tmp/blackduck-c-cpp-1.0.8.tar.gz` & `tmp/blackduck-c-cpp-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackduck-c-cpp-1.0.8.tar", last modified: Tue Apr 12 14:10:25 2022, max compression
+gzip compressed data, was "blackduck-c-cpp-1.0.9.tar", last modified: Wed May 25 13:04:58 2022, max compression
```

## Comparing `blackduck-c-cpp-1.0.8.tar` & `blackduck-c-cpp-1.0.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 kakarlas   (501) staff       (20)        0 2022-04-12 14:10:25.647783 blackduck-c-cpp-1.0.8/
--rw-r--r--   0 kakarlas   (501) staff       (20)      140 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.8/LICENSE
--rw-r--r--   0 kakarlas   (501) staff       (20)       84 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.8/MANIFEST.in
--rw-r--r--   0 kakarlas   (501) staff       (20)    20132 2022-04-12 14:10:25.647374 blackduck-c-cpp-1.0.8/PKG-INFO
--rw-r--r--   0 kakarlas   (501) staff       (20)    19762 2022-04-12 14:10:07.000000 blackduck-c-cpp-1.0.8/README.md
-drwxr-xr-x   0 kakarlas   (501) staff       (20)        0 2022-04-12 14:10:25.624972 blackduck-c-cpp-1.0.8/blackduck_c_cpp/
--rw-r--r--   0 kakarlas   (501) staff       (20)        0 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/__init__.py
-drwxr-xr-x   0 kakarlas   (501) staff       (20)        0 2022-04-12 14:10:25.628316 blackduck-c-cpp-1.0.8/blackduck_c_cpp/bdba/
--rw-r--r--   0 kakarlas   (501) staff       (20)        0 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/bdba/__init__.py
--rw-r--r--   0 kakarlas   (501) staff       (20)     4419 2022-01-31 14:15:16.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/bdba/upload_bdba.py
-drwxr-xr-x   0 kakarlas   (501) staff       (20)        0 2022-04-12 14:10:25.629434 blackduck-c-cpp-1.0.8/blackduck_c_cpp/bdio/
--rw-r--r--   0 kakarlas   (501) staff       (20)        0 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/bdio/__init__.py
--rw-r--r--   0 kakarlas   (501) staff       (20)     5263 2021-11-08 14:36:06.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/bdio/bdio2_python_transformer.py
-drwxr-xr-x   0 kakarlas   (501) staff       (20)        0 2022-04-12 14:10:25.631338 blackduck-c-cpp-1.0.8/blackduck_c_cpp/coverity_json/
--rw-r--r--   0 kakarlas   (501) staff       (20)        0 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/coverity_json/__init__.py
--rw-r--r--   0 kakarlas   (501) staff       (20)     8360 2022-04-12 14:10:07.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/coverity_json/cov_json_parse.py
-drwxr-xr-x   0 kakarlas   (501) staff       (20)        0 2022-04-12 14:10:25.633139 blackduck-c-cpp-1.0.8/blackduck_c_cpp/katiska/
--rw-r--r--   0 kakarlas   (501) staff       (20)        0 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/katiska/__init__.py
-drwxr-xr-x   0 kakarlas   (501) staff       (20)        0 2022-04-12 14:10:25.634735 blackduck-c-cpp-1.0.8/blackduck_c_cpp/katiska/bdio/
--rw-r--r--   0 kakarlas   (501) staff       (20)        0 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/katiska/bdio/__init__.py
--rw-r--r--   0 kakarlas   (501) staff       (20)    26467 2021-10-06 21:25:13.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/katiska/bdio/bdio_entries.py
--rw-r--r--   0 kakarlas   (501) staff       (20)     6407 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/katiska/bdio/bdio_paths.py
--rw-r--r--   0 kakarlas   (501) staff       (20)     4912 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/katiska/custom_types.py
--rw-r--r--   0 kakarlas   (501) staff       (20)      681 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/katiska/version_king.py
-drwxr-xr-x   0 kakarlas   (501) staff       (20)        0 2022-04-12 14:10:25.638396 blackduck-c-cpp-1.0.8/blackduck_c_cpp/pkg_manager/
--rw-r--r--   0 kakarlas   (501) staff       (20)        0 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/pkg_manager/__init__.py
--rw-r--r--   0 kakarlas   (501) staff       (20)     4049 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/pkg_manager/ld_debug_parse.py
--rw-r--r--   0 kakarlas   (501) staff       (20)    52591 2022-02-14 14:37:09.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/pkg_manager/pkg_manager_bom.py
--rw-r--r--   0 kakarlas   (501) staff       (20)     3584 2022-01-31 14:15:12.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/pkg_manager/pkg_manager_detector.py
--rw-r--r--   0 kakarlas   (501) staff       (20)    29927 2022-03-07 14:43:58.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/run_build_capture.py
-drwxr-xr-x   0 kakarlas   (501) staff       (20)        0 2022-04-12 14:10:25.639991 blackduck-c-cpp-1.0.8/blackduck_c_cpp/sig_scanner/
--rw-r--r--   0 kakarlas   (501) staff       (20)        0 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/sig_scanner/__init__.py
--rw-r--r--   0 kakarlas   (501) staff       (20)     5263 2022-04-12 14:10:07.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/sig_scanner/emit_wrapper.py
--rw-r--r--   0 kakarlas   (501) staff       (20)    27830 2022-04-12 14:10:07.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/sig_scanner/run_sig_scanner.py
-drwxr-xr-x   0 kakarlas   (501) staff       (20)        0 2022-04-12 14:10:25.646082 blackduck-c-cpp-1.0.8/blackduck_c_cpp/util/
--rw-r--r--   0 kakarlas   (501) staff       (20)        0 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/util/__init__.py
--rw-r--r--   0 kakarlas   (501) staff       (20)    12391 2021-10-14 16:50:10.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/util/build_log_parser.py
--rw-r--r--   0 kakarlas   (501) staff       (20)    12396 2022-01-31 14:15:12.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/util/c_arg_parser.py
--rw-r--r--   0 kakarlas   (501) staff       (20)     7219 2022-04-12 14:10:07.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/util/cov_install.py
--rw-r--r--   0 kakarlas   (501) staff       (20)     2586 2022-04-12 14:10:07.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/util/global_settings.py
--rw-r--r--   0 kakarlas   (501) staff       (20)     2103 2022-01-31 14:15:12.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/util/hub_api.py
--rw-r--r--   0 kakarlas   (501) staff       (20)     3398 2022-01-31 14:15:16.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/util/util.py
--rw-r--r--   0 kakarlas   (501) staff       (20)      948 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp/util/zip_file.py
-drwxr-xr-x   0 kakarlas   (501) staff       (20)        0 2022-04-12 14:10:25.627795 blackduck-c-cpp-1.0.8/blackduck_c_cpp.egg-info/
--rw-r--r--   0 kakarlas   (501) staff       (20)    20132 2022-04-12 14:10:25.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp.egg-info/PKG-INFO
--rw-r--r--   0 kakarlas   (501) staff       (20)     1422 2022-04-12 14:10:25.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp.egg-info/SOURCES.txt
--rw-r--r--   0 kakarlas   (501) staff       (20)        1 2022-04-12 14:10:25.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp.egg-info/dependency_links.txt
--rw-r--r--   0 kakarlas   (501) staff       (20)       75 2022-04-12 14:10:25.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp.egg-info/entry_points.txt
--rw-r--r--   0 kakarlas   (501) staff       (20)      240 2022-04-12 14:10:25.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp.egg-info/requires.txt
--rw-r--r--   0 kakarlas   (501) staff       (20)       16 2022-04-12 14:10:25.000000 blackduck-c-cpp-1.0.8/blackduck_c_cpp.egg-info/top_level.txt
--rw-r--r--   0 kakarlas   (501) staff       (20)       38 2022-04-12 14:10:25.647896 blackduck-c-cpp-1.0.8/setup.cfg
--rw-r--r--   0 kakarlas   (501) staff       (20)     1422 2022-04-12 14:10:07.000000 blackduck-c-cpp-1.0.8/setup.py
+drwxr-xr-x   0 kakarlas   (501) staff       (20)        0 2022-05-25 13:04:58.459020 blackduck-c-cpp-1.0.9/
+-rw-r--r--   0 kakarlas   (501) staff       (20)      140 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.9/LICENSE
+-rw-r--r--   0 kakarlas   (501) staff       (20)       84 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.9/MANIFEST.in
+-rw-r--r--   0 kakarlas   (501) staff       (20)    20142 2022-05-25 13:04:58.458075 blackduck-c-cpp-1.0.9/PKG-INFO
+-rw-r--r--   0 kakarlas   (501) staff       (20)    19772 2022-05-20 14:26:08.000000 blackduck-c-cpp-1.0.9/README.md
+drwxr-xr-x   0 kakarlas   (501) staff       (20)        0 2022-05-25 13:04:58.280239 blackduck-c-cpp-1.0.9/blackduck_c_cpp/
+-rw-r--r--   0 kakarlas   (501) staff       (20)        0 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/__init__.py
+drwxr-xr-x   0 kakarlas   (501) staff       (20)        0 2022-05-25 13:04:58.367677 blackduck-c-cpp-1.0.9/blackduck_c_cpp/bdba/
+-rw-r--r--   0 kakarlas   (501) staff       (20)        0 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/bdba/__init__.py
+-rw-r--r--   0 kakarlas   (501) staff       (20)     4419 2022-01-31 14:15:16.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/bdba/upload_bdba.py
+drwxr-xr-x   0 kakarlas   (501) staff       (20)        0 2022-05-25 13:04:58.376835 blackduck-c-cpp-1.0.9/blackduck_c_cpp/bdio/
+-rw-r--r--   0 kakarlas   (501) staff       (20)        0 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/bdio/__init__.py
+-rw-r--r--   0 kakarlas   (501) staff       (20)     5263 2021-11-08 14:36:06.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/bdio/bdio2_python_transformer.py
+drwxr-xr-x   0 kakarlas   (501) staff       (20)        0 2022-05-25 13:04:58.382905 blackduck-c-cpp-1.0.9/blackduck_c_cpp/coverity_json/
+-rw-r--r--   0 kakarlas   (501) staff       (20)        0 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/coverity_json/__init__.py
+-rw-r--r--   0 kakarlas   (501) staff       (20)     8360 2022-04-12 14:10:07.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/coverity_json/cov_json_parse.py
+drwxr-xr-x   0 kakarlas   (501) staff       (20)        0 2022-05-25 13:04:58.396906 blackduck-c-cpp-1.0.9/blackduck_c_cpp/katiska/
+-rw-r--r--   0 kakarlas   (501) staff       (20)        0 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/katiska/__init__.py
+drwxr-xr-x   0 kakarlas   (501) staff       (20)        0 2022-05-25 13:04:58.407285 blackduck-c-cpp-1.0.9/blackduck_c_cpp/katiska/bdio/
+-rw-r--r--   0 kakarlas   (501) staff       (20)        0 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/katiska/bdio/__init__.py
+-rw-r--r--   0 kakarlas   (501) staff       (20)    26467 2021-10-06 21:25:13.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/katiska/bdio/bdio_entries.py
+-rw-r--r--   0 kakarlas   (501) staff       (20)     6407 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/katiska/bdio/bdio_paths.py
+-rw-r--r--   0 kakarlas   (501) staff       (20)     4912 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/katiska/custom_types.py
+-rw-r--r--   0 kakarlas   (501) staff       (20)      681 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/katiska/version_king.py
+drwxr-xr-x   0 kakarlas   (501) staff       (20)        0 2022-05-25 13:04:58.419526 blackduck-c-cpp-1.0.9/blackduck_c_cpp/pkg_manager/
+-rw-r--r--   0 kakarlas   (501) staff       (20)        0 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/pkg_manager/__init__.py
+-rw-r--r--   0 kakarlas   (501) staff       (20)     4049 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/pkg_manager/ld_debug_parse.py
+-rw-r--r--   0 kakarlas   (501) staff       (20)    52624 2022-05-20 14:26:08.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/pkg_manager/pkg_manager_bom.py
+-rw-r--r--   0 kakarlas   (501) staff       (20)     3584 2022-01-31 14:15:12.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/pkg_manager/pkg_manager_detector.py
+-rw-r--r--   0 kakarlas   (501) staff       (20)    30053 2022-05-20 16:15:12.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/run_build_capture.py
+drwxr-xr-x   0 kakarlas   (501) staff       (20)        0 2022-05-25 13:04:58.429225 blackduck-c-cpp-1.0.9/blackduck_c_cpp/sig_scanner/
+-rw-r--r--   0 kakarlas   (501) staff       (20)        0 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/sig_scanner/__init__.py
+-rw-r--r--   0 kakarlas   (501) staff       (20)     5263 2022-04-12 14:10:07.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/sig_scanner/emit_wrapper.py
+-rw-r--r--   0 kakarlas   (501) staff       (20)    27830 2022-05-20 14:26:05.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/sig_scanner/run_sig_scanner.py
+drwxr-xr-x   0 kakarlas   (501) staff       (20)        0 2022-05-25 13:04:58.456488 blackduck-c-cpp-1.0.9/blackduck_c_cpp/util/
+-rw-r--r--   0 kakarlas   (501) staff       (20)        0 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/util/__init__.py
+-rw-r--r--   0 kakarlas   (501) staff       (20)    12391 2021-10-14 16:50:10.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/util/build_log_parser.py
+-rw-r--r--   0 kakarlas   (501) staff       (20)    12508 2022-05-20 16:10:51.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/util/c_arg_parser.py
+-rw-r--r--   0 kakarlas   (501) staff       (20)     7219 2022-04-12 14:10:07.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/util/cov_install.py
+-rw-r--r--   0 kakarlas   (501) staff       (20)     2586 2022-04-12 14:10:07.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/util/global_settings.py
+-rw-r--r--   0 kakarlas   (501) staff       (20)     2103 2022-01-31 14:15:12.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/util/hub_api.py
+-rw-r--r--   0 kakarlas   (501) staff       (20)     3398 2022-01-31 14:15:16.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/util/util.py
+-rw-r--r--   0 kakarlas   (501) staff       (20)      948 2021-09-02 14:22:28.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp/util/zip_file.py
+drwxr-xr-x   0 kakarlas   (501) staff       (20)        0 2022-05-25 13:04:58.362197 blackduck-c-cpp-1.0.9/blackduck_c_cpp.egg-info/
+-rw-r--r--   0 kakarlas   (501) staff       (20)    20142 2022-05-25 13:04:57.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp.egg-info/PKG-INFO
+-rw-r--r--   0 kakarlas   (501) staff       (20)     1422 2022-05-25 13:04:57.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp.egg-info/SOURCES.txt
+-rw-r--r--   0 kakarlas   (501) staff       (20)        1 2022-05-25 13:04:57.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp.egg-info/dependency_links.txt
+-rw-r--r--   0 kakarlas   (501) staff       (20)       75 2022-05-25 13:04:57.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp.egg-info/entry_points.txt
+-rw-r--r--   0 kakarlas   (501) staff       (20)      240 2022-05-25 13:04:57.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp.egg-info/requires.txt
+-rw-r--r--   0 kakarlas   (501) staff       (20)       16 2022-05-25 13:04:57.000000 blackduck-c-cpp-1.0.9/blackduck_c_cpp.egg-info/top_level.txt
+-rw-r--r--   0 kakarlas   (501) staff       (20)       38 2022-05-25 13:04:58.459158 blackduck-c-cpp-1.0.9/setup.cfg
+-rw-r--r--   0 kakarlas   (501) staff       (20)     1422 2022-05-20 14:26:08.000000 blackduck-c-cpp-1.0.9/setup.py
```

### Comparing `blackduck-c-cpp-1.0.8/PKG-INFO` & `blackduck-c-cpp-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackduck-c-cpp
-Version: 1.0.8
+Version: 1.0.9
 Summary: Scanning for c/c++ projects using blackduck and coverity tools
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Requires-Python: >=3.6
@@ -167,15 +167,15 @@
   -st [SKIP_TRANSITIVES], --skip_transitives [SKIP_TRANSITIVES]
                         Skipping all transitive dependencies
   -sh [SKIP_INCLUDES], --skip_includes [SKIP_INCLUDES]
                         Skipping all .h & .hpp files from all types of scan
   -sd [SKIP_DYNAMIC], --skip_dynamic [SKIP_DYNAMIC]
                         Skipping all dynamic (.so/.dll) files from all types of scan
   -off [OFFLINE], --offline [OFFLINE]
-                        store bdba and sig tar files and c_cpp_bdio2.jsonld to disk if offline mode is true
+                        store bdba and sig tar files, sig scan json, and raw_bdio.csv to disk if offline mode is true
   -uo [USE_OFFLINE_FILES] --use_offline_files
                         use offline generated files for upload in online mode 
   -md modes, --modes modes
                         comma separated list of modes to run - 'all' - default,'bdba','sig','pkg_mgr'
   -es expand_sig_files, --expand_sig_files expand_sig_files
                         use expand_sig_files for creating exploded directory instead of tar in sig scanner mode 
 ```
```

### Comparing `blackduck-c-cpp-1.0.8/README.md` & `blackduck-c-cpp-1.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
   -st [SKIP_TRANSITIVES], --skip_transitives [SKIP_TRANSITIVES]
                         Skipping all transitive dependencies
   -sh [SKIP_INCLUDES], --skip_includes [SKIP_INCLUDES]
                         Skipping all .h & .hpp files from all types of scan
   -sd [SKIP_DYNAMIC], --skip_dynamic [SKIP_DYNAMIC]
                         Skipping all dynamic (.so/.dll) files from all types of scan
   -off [OFFLINE], --offline [OFFLINE]
-                        store bdba and sig tar files and c_cpp_bdio2.jsonld to disk if offline mode is true
+                        store bdba and sig tar files, sig scan json, and raw_bdio.csv to disk if offline mode is true
   -uo [USE_OFFLINE_FILES] --use_offline_files
                         use offline generated files for upload in online mode 
   -md modes, --modes modes
                         comma separated list of modes to run - 'all' - default,'bdba','sig','pkg_mgr'
   -es expand_sig_files, --expand_sig_files expand_sig_files
                         use expand_sig_files for creating exploded directory instead of tar in sig scanner mode 
 ```
```

### Comparing `blackduck-c-cpp-1.0.8/blackduck_c_cpp/bdba/upload_bdba.py` & `blackduck-c-cpp-1.0.9/blackduck_c_cpp/bdba/upload_bdba.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-1.0.8/blackduck_c_cpp/bdio/bdio2_python_transformer.py` & `blackduck-c-cpp-1.0.9/blackduck_c_cpp/bdio/bdio2_python_transformer.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-1.0.8/blackduck_c_cpp/coverity_json/cov_json_parse.py` & `blackduck-c-cpp-1.0.9/blackduck_c_cpp/coverity_json/cov_json_parse.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-1.0.8/blackduck_c_cpp/katiska/bdio/bdio_entries.py` & `blackduck-c-cpp-1.0.9/blackduck_c_cpp/katiska/bdio/bdio_entries.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-1.0.8/blackduck_c_cpp/katiska/bdio/bdio_paths.py` & `blackduck-c-cpp-1.0.9/blackduck_c_cpp/katiska/bdio/bdio_paths.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-1.0.8/blackduck_c_cpp/katiska/custom_types.py` & `blackduck-c-cpp-1.0.9/blackduck_c_cpp/katiska/custom_types.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-1.0.8/blackduck_c_cpp/katiska/version_king.py` & `blackduck-c-cpp-1.0.9/blackduck_c_cpp/katiska/version_king.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-1.0.8/blackduck_c_cpp/pkg_manager/ld_debug_parse.py` & `blackduck-c-cpp-1.0.9/blackduck_c_cpp/pkg_manager/ld_debug_parse.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-1.0.8/blackduck_c_cpp/pkg_manager/pkg_manager_bom.py` & `blackduck-c-cpp-1.0.9/blackduck_c_cpp/pkg_manager/pkg_manager_bom.py`

 * *Files 0% similar despite different names*

```diff
@@ -798,15 +798,15 @@
                     "Unable to find previously generated offline files for package manager..please make sure use_offline_files and run_modes are set correctly")
 
     def set_matchtype_per_hub_version(self):
         """ this function gets hub version information and sets matchtype"""
         hub_version = self.hub_api.get_hub_version()
         logging.info("BLACK DUCK VERSION IS {}".format(hub_version))
         vers_result = hub_version.split(".")
-        if int(vers_result[0]) >= 2021 and int(vers_result[1]) >= 6:
+        if (int(vers_result[0]) >= 2021 and int(vers_result[1]) >= 6) or int(vers_result[0]) >= 2022:
             self.direct_match_evidence = 'DIRECT_DEPENDENCY_BINARY'
             self.transitive_match_evidence = 'TRANSITIVE_DEPENDENCY_BINARY'
         else:
             self.direct_match_evidence = 'Binary'
             self.transitive_match_evidence = 'Binary'
 
     def run(self):
```

### Comparing `blackduck-c-cpp-1.0.8/blackduck_c_cpp/pkg_manager/pkg_manager_detector.py` & `blackduck-c-cpp-1.0.9/blackduck_c_cpp/pkg_manager/pkg_manager_detector.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-1.0.8/blackduck_c_cpp/run_build_capture.py` & `blackduck-c-cpp-1.0.9/blackduck_c_cpp/run_build_capture.py`

 * *Files 0% similar despite different names*

```diff
@@ -513,14 +513,16 @@
         try:
             cov_emit_link_path = glob.glob(os.path.join(self.cov_bin, 'cov-emit-link*'))[0]
         except IndexError:
             pass
 
         # COV BUILD
         if not self.skip_build:
+            if self.bld_cmd == '':
+                util.error_and_exit("the following argument is required: -bc/--build_cmd")
             self.run_build(cov_emit_link_path, cov_build_path)
 
         # COV EMIT
         emit_wrapper_output_sig, emit_cov_header_files = self.run_cov_emit()
 
         # COV EMIT LINK
         if os.path.exists(cov_emit_link_path):
```

### Comparing `blackduck-c-cpp-1.0.8/blackduck_c_cpp/sig_scanner/emit_wrapper.py` & `blackduck-c-cpp-1.0.9/blackduck_c_cpp/sig_scanner/emit_wrapper.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-1.0.8/blackduck_c_cpp/sig_scanner/run_sig_scanner.py` & `blackduck-c-cpp-1.0.9/blackduck_c_cpp/sig_scanner/run_sig_scanner.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-1.0.8/blackduck_c_cpp/util/build_log_parser.py` & `blackduck-c-cpp-1.0.9/blackduck_c_cpp/util/build_log_parser.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-1.0.8/blackduck_c_cpp/util/c_arg_parser.py` & `blackduck-c-cpp-1.0.9/blackduck_c_cpp/util/c_arg_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,17 @@
 
         self.parser = configargparse.ArgParser(description='Capture all build files and send for analysis.', )
 
         self.parser.add_argument('-c', '--config', is_config_file=True, help='Configuration file path.')
 
         # Add the arguments
         self.parser.add_argument('-bc', '--build_cmd',
-                                 required=True,
+                                 metavar='build_cmd',
+                                 dest='build_cmd',
+                                 default='',
                                  type=str,
                                  help='Command used to execute the build')
 
         self.parser.add_argument('-d', '--build_dir',
                                  required=True,
                                  type=C_Parser.required_dir_exists,
                                  help='Directory from which to run build. Absolute path (not relative) information is required')
@@ -191,15 +193,15 @@
                                  help='Skipping all .so files from all types of scan')
 
         self.parser.add_argument('-off', '--offline',
                                  type=C_Parser.str2bool,
                                  nargs='?',
                                  const=True,
                                  default=False,
-                                 help='store bdba and sig tar files and c_cpp_bdio2.jsonld to disk if offline mode is true')
+                                 help='store bdba and sig tar files, sig scan json, and raw_bdio.csv to disk if offline mode is true')
 
         self.parser.add_argument('-md', '--modes',
                                  metavar='modes',
                                  dest='modes',
                                  type=str,
                                  default="ALL",
                                  help="comma separated list of modes to run - 'all'(default),'bdba','sig','pkg_mgr'")
```

### Comparing `blackduck-c-cpp-1.0.8/blackduck_c_cpp/util/cov_install.py` & `blackduck-c-cpp-1.0.9/blackduck_c_cpp/util/cov_install.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-1.0.8/blackduck_c_cpp/util/global_settings.py` & `blackduck-c-cpp-1.0.9/blackduck_c_cpp/util/global_settings.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-1.0.8/blackduck_c_cpp/util/hub_api.py` & `blackduck-c-cpp-1.0.9/blackduck_c_cpp/util/hub_api.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-1.0.8/blackduck_c_cpp/util/util.py` & `blackduck-c-cpp-1.0.9/blackduck_c_cpp/util/util.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-1.0.8/blackduck_c_cpp/util/zip_file.py` & `blackduck-c-cpp-1.0.9/blackduck_c_cpp/util/zip_file.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-1.0.8/blackduck_c_cpp.egg-info/PKG-INFO` & `blackduck-c-cpp-1.0.9/blackduck_c_cpp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackduck-c-cpp
-Version: 1.0.8
+Version: 1.0.9
 Summary: Scanning for c/c++ projects using blackduck and coverity tools
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Requires-Python: >=3.6
@@ -167,15 +167,15 @@
   -st [SKIP_TRANSITIVES], --skip_transitives [SKIP_TRANSITIVES]
                         Skipping all transitive dependencies
   -sh [SKIP_INCLUDES], --skip_includes [SKIP_INCLUDES]
                         Skipping all .h & .hpp files from all types of scan
   -sd [SKIP_DYNAMIC], --skip_dynamic [SKIP_DYNAMIC]
                         Skipping all dynamic (.so/.dll) files from all types of scan
   -off [OFFLINE], --offline [OFFLINE]
-                        store bdba and sig tar files and c_cpp_bdio2.jsonld to disk if offline mode is true
+                        store bdba and sig tar files, sig scan json, and raw_bdio.csv to disk if offline mode is true
   -uo [USE_OFFLINE_FILES] --use_offline_files
                         use offline generated files for upload in online mode 
   -md modes, --modes modes
                         comma separated list of modes to run - 'all' - default,'bdba','sig','pkg_mgr'
   -es expand_sig_files, --expand_sig_files expand_sig_files
                         use expand_sig_files for creating exploded directory instead of tar in sig scanner mode 
 ```
```

### Comparing `blackduck-c-cpp-1.0.8/blackduck_c_cpp.egg-info/SOURCES.txt` & `blackduck-c-cpp-1.0.9/blackduck_c_cpp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-1.0.8/setup.py` & `blackduck-c-cpp-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="blackduck-c-cpp",
-    version="1.0.8",
+    version="1.0.9",
     description="Scanning for c/c++ projects using blackduck and coverity tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=["requests>=2.5.3",
                       "numpy>=1.19.5",
                       "pandas>=1.1.5",
```

