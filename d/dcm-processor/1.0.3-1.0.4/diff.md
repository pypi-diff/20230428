# Comparing `tmp/dcm-processor-1.0.3.tar.gz` & `tmp/dcm-processor-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcm-processor-1.0.3.tar", last modified: Sat Apr 22 10:53:25 2023, max compression
+gzip compressed data, was "dcm-processor-1.0.4.tar", last modified: Fri Apr 28 08:27:44 2023, max compression
```

## Comparing `dcm-processor-1.0.3.tar` & `dcm-processor-1.0.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.394013 dcm-processor-1.0.3/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1074 2021-05-11 10:55:48.000000 dcm-processor-1.0.3/LICENSE
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6335 2023-04-22 10:53:25.394322 dcm-processor-1.0.3/PKG-INFO
--rwxr-xr-x   0 giles     (1000) giles     (1000)     5834 2023-04-17 10:06:58.000000 dcm-processor-1.0.3/README.md
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.132198 dcm-processor-1.0.3/dcm_processor/
--rwxr-xr-x   0 giles     (1000) giles     (1000)       61 2021-10-17 14:30:50.000000 dcm-processor-1.0.3/dcm_processor/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    15407 2023-04-15 09:02:58.000000 dcm-processor-1.0.3/dcm_processor/argparser.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    33044 2023-04-22 10:03:38.000000 dcm-processor-1.0.3/dcm_processor/files.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    46033 2023-04-19 12:36:49.000000 dcm-processor-1.0.3/dcm_processor/script.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.085824 dcm-processor-1.0.3/dcm_processor/services/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.085127 dcm-processor-1.0.3/dcm_processor/services/base/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.165520 dcm-processor-1.0.3/dcm_processor/services/base/module/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.289840 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/
--rwxr-xr-x   0 giles     (1000) giles     (1000)   642195 2021-10-17 16:16:14.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)    17869 2021-10-17 16:16:15.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)      526 2023-04-06 14:13:53.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1551 2023-03-31 12:36:10.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    69564 2021-10-17 16:16:15.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.309642 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/config/
--rwxr-xr-x   0 giles     (1000) giles     (1000)    59497 2021-10-17 16:16:15.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script
--rwxr-xr-x   0 giles     (1000) giles     (1000)      248 2021-10-17 16:16:15.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/config/hash_table.csv
--rwxr-xr-x   0 giles     (1000) giles     (1000)       86 2021-10-17 16:16:15.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/config/psudonyms.csv
--rwxr-xr-x   0 giles     (1000) giles     (1000)    10424 2021-10-17 16:16:15.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)   863881 2021-10-17 16:16:16.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)     3471 2023-03-31 12:35:15.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)  1172845 2021-10-17 16:16:18.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)   391834 2021-10-17 16:16:19.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)    28241 2021-10-17 16:16:19.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)   338969 2021-10-17 16:16:20.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/util.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1777 2023-03-31 20:09:03.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/utils.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)       26 2021-10-17 16:16:20.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/requirements.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       72 2021-10-17 16:16:20.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/script.sh
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.326522 dcm-processor-1.0.3/dcm_processor/services/base/module/storageManager/
--rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/storageManager/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)       97 2021-10-17 16:16:20.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/storageManager/header_codes.json
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6218 2023-01-31 18:15:24.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/storageManager/lib.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    10012 2023-01-31 18:15:43.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/storageManager/main.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.330046 dcm-processor-1.0.3/dcm_processor/services/base/module/systemcleaner/
--rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/systemcleaner/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)     3806 2023-04-01 16:24:05.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/systemcleaner/main.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.337447 dcm-processor-1.0.3/dcm_processor/services/base/registry/
--rwxr-xr-x   0 giles     (1000) giles     (1000)      443 2021-10-17 16:16:20.000000 dcm-processor-1.0.3/dcm_processor/services/base/registry/__init__.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.087046 dcm-processor-1.0.3/dcm_processor/services/dcm2nii/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.387526 dcm-processor-1.0.3/dcm_processor/services/dcm2nii/module/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     4030 2023-04-14 14:47:11.000000 dcm-processor-1.0.3/dcm_processor/services/dcm2nii/module/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)  1948128 2023-03-02 19:03:11.000000 dcm-processor-1.0.3/dcm_processor/services/dcm2nii/module/dcm2niix
--rwxr-xr-x   0 giles     (1000) giles     (1000)      406 2023-03-24 20:50:04.000000 dcm-processor-1.0.3/dcm_processor/services/dcm2nii/module/lib.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.391551 dcm-processor-1.0.3/dcm_processor/services/dcm2nii/registry/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1013 2023-04-14 12:17:35.000000 dcm-processor-1.0.3/dcm_processor/services/dcm2nii/registry/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)      288 2023-04-18 12:25:35.000000 dcm-processor-1.0.3/dcm_processor/services/dcm2nii/registry/settings.json
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6682 2023-04-21 16:23:38.000000 dcm-processor-1.0.3/dcm_processor/worker.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.157451 dcm-processor-1.0.3/dcm_processor.egg-info/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6335 2023-04-22 10:53:23.000000 dcm-processor-1.0.3/dcm_processor.egg-info/PKG-INFO
--rwxr-xr-x   0 giles     (1000) giles     (1000)     2368 2023-04-22 10:53:24.000000 dcm-processor-1.0.3/dcm_processor.egg-info/SOURCES.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)        1 2023-04-22 10:53:23.000000 dcm-processor-1.0.3/dcm_processor.egg-info/dependency_links.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       53 2023-04-22 10:53:23.000000 dcm-processor-1.0.3/dcm_processor.egg-info/entry_points.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       76 2023-04-22 10:53:23.000000 dcm-processor-1.0.3/dcm_processor.egg-info/requires.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       14 2023-04-22 10:53:23.000000 dcm-processor-1.0.3/dcm_processor.egg-info/top_level.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       89 2021-10-17 14:23:09.000000 dcm-processor-1.0.3/pyproject.toml
--rwxr-xr-x   0 giles     (1000) giles     (1000)      980 2023-04-22 10:53:25.395849 dcm-processor-1.0.3/setup.cfg
--rwxr-xr-x   0 giles     (1000) giles     (1000)      109 2021-10-17 19:37:23.000000 dcm-processor-1.0.3/setup.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 08:27:44.502306 dcm-processor-1.0.4/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     1074 2021-05-11 10:55:48.000000 dcm-processor-1.0.4/LICENSE
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     6335 2023-04-28 08:27:44.502659 dcm-processor-1.0.4/PKG-INFO
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     5834 2023-04-17 10:06:58.000000 dcm-processor-1.0.4/README.md
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 08:27:44.279574 dcm-processor-1.0.4/dcm_processor/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       61 2021-10-17 14:30:50.000000 dcm-processor-1.0.4/dcm_processor/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    15407 2023-04-15 09:02:58.000000 dcm-processor-1.0.4/dcm_processor/argparser.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    33079 2023-04-24 10:51:24.000000 dcm-processor-1.0.4/dcm_processor/files.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    46033 2023-04-19 12:36:49.000000 dcm-processor-1.0.4/dcm_processor/script.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 08:27:44.265722 dcm-processor-1.0.4/dcm_processor/services/
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 08:27:44.265229 dcm-processor-1.0.4/dcm_processor/services/base/
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 08:27:44.295810 dcm-processor-1.0.4/dcm_processor/services/base/module/
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 08:27:44.398630 dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)   642195 2021-10-17 16:16:14.000000 dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    17869 2021-10-17 16:16:15.000000 dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      526 2023-04-06 14:13:53.000000 dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     1551 2023-03-31 12:36:10.000000 dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    69564 2021-10-17 16:16:15.000000 dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 08:27:44.416350 dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/config/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    59497 2021-10-17 16:16:15.000000 dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      248 2021-10-17 16:16:15.000000 dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/config/hash_table.csv
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       86 2021-10-17 16:16:15.000000 dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/config/psudonyms.csv
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    10424 2021-10-17 16:16:15.000000 dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)   863881 2021-10-17 16:16:16.000000 dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     3471 2023-03-31 12:35:15.000000 dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)  1172845 2021-10-17 16:16:18.000000 dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)   391834 2021-10-17 16:16:19.000000 dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    28241 2021-10-17 16:16:19.000000 dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)   338969 2021-10-17 16:16:20.000000 dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/util.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     1777 2023-03-31 20:09:03.000000 dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/utils.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       26 2021-10-17 16:16:20.000000 dcm-processor-1.0.4/dcm_processor/services/base/module/requirements.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       72 2021-10-17 16:16:20.000000 dcm-processor-1.0.4/dcm_processor/services/base/module/script.sh
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 08:27:44.433892 dcm-processor-1.0.4/dcm_processor/services/base/module/storageManager/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-1.0.4/dcm_processor/services/base/module/storageManager/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       97 2021-10-17 16:16:20.000000 dcm-processor-1.0.4/dcm_processor/services/base/module/storageManager/header_codes.json
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     6218 2023-01-31 18:15:24.000000 dcm-processor-1.0.4/dcm_processor/services/base/module/storageManager/lib.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    10091 2023-04-24 09:30:51.000000 dcm-processor-1.0.4/dcm_processor/services/base/module/storageManager/main.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 08:27:44.449902 dcm-processor-1.0.4/dcm_processor/services/base/module/systemcleaner/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-1.0.4/dcm_processor/services/base/module/systemcleaner/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     3806 2023-04-01 16:24:05.000000 dcm-processor-1.0.4/dcm_processor/services/base/module/systemcleaner/main.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 08:27:44.452294 dcm-processor-1.0.4/dcm_processor/services/base/registry/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      443 2021-10-17 16:16:20.000000 dcm-processor-1.0.4/dcm_processor/services/base/registry/__init__.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 08:27:44.266318 dcm-processor-1.0.4/dcm_processor/services/dcm2nii/
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 08:27:44.493895 dcm-processor-1.0.4/dcm_processor/services/dcm2nii/module/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     4030 2023-04-14 14:47:11.000000 dcm-processor-1.0.4/dcm_processor/services/dcm2nii/module/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)  1948128 2023-03-02 19:03:11.000000 dcm-processor-1.0.4/dcm_processor/services/dcm2nii/module/dcm2niix
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      406 2023-03-24 20:50:04.000000 dcm-processor-1.0.4/dcm_processor/services/dcm2nii/module/lib.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 08:27:44.500605 dcm-processor-1.0.4/dcm_processor/services/dcm2nii/registry/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     1013 2023-04-14 12:17:35.000000 dcm-processor-1.0.4/dcm_processor/services/dcm2nii/registry/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      288 2023-04-18 12:25:35.000000 dcm-processor-1.0.4/dcm_processor/services/dcm2nii/registry/settings.json
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     6682 2023-04-21 16:23:38.000000 dcm-processor-1.0.4/dcm_processor/worker.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-28 08:27:44.286274 dcm-processor-1.0.4/dcm_processor.egg-info/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     6335 2023-04-28 08:27:43.000000 dcm-processor-1.0.4/dcm_processor.egg-info/PKG-INFO
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     2368 2023-04-28 08:27:44.000000 dcm-processor-1.0.4/dcm_processor.egg-info/SOURCES.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)        1 2023-04-28 08:27:43.000000 dcm-processor-1.0.4/dcm_processor.egg-info/dependency_links.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       53 2023-04-28 08:27:43.000000 dcm-processor-1.0.4/dcm_processor.egg-info/entry_points.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       76 2023-04-28 08:27:43.000000 dcm-processor-1.0.4/dcm_processor.egg-info/requires.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       14 2023-04-28 08:27:43.000000 dcm-processor-1.0.4/dcm_processor.egg-info/top_level.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       89 2021-10-17 14:23:09.000000 dcm-processor-1.0.4/pyproject.toml
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      980 2023-04-28 08:27:44.505303 dcm-processor-1.0.4/setup.cfg
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      109 2021-10-17 19:37:23.000000 dcm-processor-1.0.4/setup.py
```

### Comparing `dcm-processor-1.0.3/LICENSE` & `dcm-processor-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.3/PKG-INFO` & `dcm-processor-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcm-processor
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Command line tool for the dicom processor library
 Home-page: https://github.com/giesekow/dcm-processor-cli
 Author: Giles Tetteh
 Author-email: giles.tetteh@tum.de
 Keywords: orthanc,dicom,worker,processor,translation,medical
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dcm-processor-1.0.3/README.md` & `dcm-processor-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.3/dcm_processor/argparser.py` & `dcm-processor-1.0.4/dcm_processor/argparser.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.3/dcm_processor/files.py` & `dcm-processor-1.0.4/dcm_processor/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,17 @@
     {
       "jobName": "storageManager",
       "worker": "base.storageManager.worker",
       "callback": "base.storageManager",
       "dependsOn": null,
       "channel": "default",
       "timeout": "1h",
-      "params": {},
+      "params": {
+        "store_data": false
+      },
       "sortPosition": 0,
       "description": "Storage Service"
     },
     {
       "jobName": "systemClearner",
       "worker": "base.systemcleaner.worker",
       "callback": "base.systemcleaner",
```

### Comparing `dcm-processor-1.0.3/dcm_processor/script.py` & `dcm-processor-1.0.4/dcm_processor/script.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar` & `dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar` & `dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py` & `dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py` & `dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar` & `dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script` & `dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar` & `dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar` & `dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py` & `dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar` & `dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar` & `dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar` & `dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/util.jar` & `dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/util.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/utils.py` & `dcm-processor-1.0.4/dcm_processor/services/base/module/DicomAnonymizerService/utils.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.3/dcm_processor/services/base/module/storageManager/lib.py` & `dcm-processor-1.0.4/dcm_processor/services/base/module/storageManager/lib.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.3/dcm_processor/services/base/module/storageManager/main.py` & `dcm-processor-1.0.4/dcm_processor/services/base/module/storageManager/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,14 +204,17 @@
       f_type = str(f_type).lower()
       fullpath = os.path.join(DATA, store.get("path"))
       tags = {}
 
       destination = store.get("destination", DEFAULT_STORE)
       action = "store-data" if store.get("permanent", False) else "orthanc-only"
 
+      if not params.get("store_data", False):
+        action = "orthanc-only"
+
       if "tags" in store:
         t = store.get("tags")
         if isinstance(t, dict):
           tags = t
 
       if f_type in FORMATS:
         if not os.path.isfile(fullpath):
```

### Comparing `dcm-processor-1.0.3/dcm_processor/services/base/module/systemcleaner/main.py` & `dcm-processor-1.0.4/dcm_processor/services/base/module/systemcleaner/main.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.3/dcm_processor/services/dcm2nii/module/__init__.py` & `dcm-processor-1.0.4/dcm_processor/services/dcm2nii/module/__init__.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.3/dcm_processor/services/dcm2nii/module/dcm2niix` & `dcm-processor-1.0.4/dcm_processor/services/dcm2nii/module/dcm2niix`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.3/dcm_processor/services/dcm2nii/registry/__init__.py` & `dcm-processor-1.0.4/dcm_processor/services/dcm2nii/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.3/dcm_processor/worker.py` & `dcm-processor-1.0.4/dcm_processor/worker.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.3/dcm_processor.egg-info/PKG-INFO` & `dcm-processor-1.0.4/dcm_processor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcm-processor
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Command line tool for the dicom processor library
 Home-page: https://github.com/giesekow/dcm-processor-cli
 Author: Giles Tetteh
 Author-email: giles.tetteh@tum.de
 Keywords: orthanc,dicom,worker,processor,translation,medical
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dcm-processor-1.0.3/dcm_processor.egg-info/SOURCES.txt` & `dcm-processor-1.0.4/dcm_processor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.3/setup.cfg` & `dcm-processor-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dcm-processor
-version = 1.0.3
+version = 1.0.4
 author = Giles Tetteh
 author_email = giles.tetteh@tum.de
 description = A Command line tool for the dicom processor library
 url = https://github.com/giesekow/dcm-processor-cli
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE
```

