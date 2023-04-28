# Comparing `tmp/sbp-4.8.0.tar.gz` & `tmp/sbp-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbp-4.8.0.tar", last modified: Thu Sep 29 03:26:13 2022, max compression
+gzip compressed data, was "sbp-4.9.0.tar", last modified: Tue Nov  1 23:16:51 2022, max compression
```

## Comparing `sbp-4.8.0.tar` & `sbp-4.9.0.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 dockerdev  (1000) dockerdev  (1000)        0 2022-09-29 03:26:13.958110 sbp-4.8.0/
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     1149 2022-09-29 03:26:00.000000 sbp-4.8.0/.gitignore
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)      225 2022-09-29 03:26:00.000000 sbp-4.8.0/MANIFEST.in
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     3509 2022-09-29 03:26:13.959110 sbp-4.8.0/PKG-INFO
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     1831 2022-09-29 03:26:00.000000 sbp-4.8.0/README.rst
-drwxr-xr-x   0 dockerdev  (1000) dockerdev  (1000)        0 2022-09-29 03:26:13.906110 sbp-4.8.0/bin/
--rwxr-xr-x   0 dockerdev  (1000) dockerdev  (1000)      106 2022-04-28 06:48:13.000000 sbp-4.8.0/bin/sbp2json
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     5192 2022-09-29 03:26:00.000000 sbp-4.8.0/deploy.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)       44 2022-09-29 03:26:00.000000 sbp-4.8.0/requirements.txt
-drwxr-xr-x   0 dockerdev  (1000) dockerdev  (1000)        0 2022-09-29 03:26:13.932110 sbp-4.8.0/sbp/
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)        5 2022-09-29 03:25:04.000000 sbp-4.8.0/sbp/RELEASE-VERSION
--rwxr-xr-x   0 dockerdev  (1000) dockerdev  (1000)      636 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/__init__.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)      179 2022-09-29 03:26:13.000000 sbp-4.8.0/sbp/_version.py
--rwxr-xr-x   0 dockerdev  (1000) dockerdev  (1000)    23052 2022-09-29 01:07:51.000000 sbp-4.8.0/sbp/acquisition.py
--rwxr-xr-x   0 dockerdev  (1000) dockerdev  (1000)    14689 2022-09-29 01:07:50.000000 sbp-4.8.0/sbp/bootload.py
-drwxr-xr-x   0 dockerdev  (1000) dockerdev  (1000)        0 2022-09-29 03:26:13.939110 sbp-4.8.0/sbp/client/
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)      619 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/client/__init__.py
-drwxr-xr-x   0 dockerdev  (1000) dockerdev  (1000)        0 2022-09-29 03:26:13.945110 sbp-4.8.0/sbp/client/drivers/
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)        0 2022-04-27 00:14:46.000000 sbp-4.8.0/sbp/client/drivers/__init__.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     3204 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/client/drivers/base_driver.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     2019 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/client/drivers/cdc_driver.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     2958 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/client/drivers/file_driver.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     3912 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/client/drivers/network_drivers.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     1071 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/client/drivers/pyftdi_driver.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     3742 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/client/drivers/pyserial_driver.py
-drwxr-xr-x   0 dockerdev  (1000) dockerdev  (1000)        0 2022-09-29 03:26:13.948110 sbp-4.8.0/sbp/client/examples/
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)        0 2022-04-27 00:14:46.000000 sbp-4.8.0/sbp/client/examples/__init__.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     1706 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/client/examples/simple.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     1756 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/client/examples/tcp.py
--rwxr-xr-x   0 dockerdev  (1000) dockerdev  (1000)     2363 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/client/examples/udp.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     1854 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/client/forwarder.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     5318 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/client/framer.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)    10475 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/client/handler.py
-drwxr-xr-x   0 dockerdev  (1000) dockerdev  (1000)        0 2022-09-29 03:26:13.953110 sbp-4.8.0/sbp/client/loggers/
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)        0 2022-04-27 00:14:46.000000 sbp-4.8.0/sbp/client/loggers/__init__.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     3237 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/client/loggers/base_logger.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     6242 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/client/loggers/json_logger.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)      879 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/client/loggers/null_logger.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     2074 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/client/loggers/rotating_logger.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     1264 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/client/loggers/udp_logger.py
-drwxr-xr-x   0 dockerdev  (1000) dockerdev  (1000)        0 2022-09-29 03:26:13.955110 sbp-4.8.0/sbp/client/util/
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)        0 2022-04-27 00:14:46.000000 sbp-4.8.0/sbp/client/util/__init__.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     6642 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/client/util/fftmonitor.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     4808 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/client/util/settingmonitor.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     2799 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/constants.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     3956 2022-09-29 01:07:50.000000 sbp-4.8.0/sbp/ext_events.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)    28450 2022-09-29 01:07:50.000000 sbp-4.8.0/sbp/file_io.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)    27810 2022-09-29 01:07:50.000000 sbp-4.8.0/sbp/flash.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     7543 2022-09-29 01:07:50.000000 sbp-4.8.0/sbp/gnss.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     7662 2022-09-29 01:07:50.000000 sbp-4.8.0/sbp/imu.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)    24554 2022-09-29 01:07:51.000000 sbp-4.8.0/sbp/integrity.py
-drwxr-xr-x   0 dockerdev  (1000) dockerdev  (1000)        0 2022-09-29 03:26:13.956110 sbp-4.8.0/sbp/jit/
--rwxr-xr-x   0 dockerdev  (1000) dockerdev  (1000)       87 2022-04-27 00:14:46.000000 sbp-4.8.0/sbp/jit/__init__.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)    39715 2022-09-29 01:07:50.000000 sbp-4.8.0/sbp/linux.py
--rwxr-xr-x   0 dockerdev  (1000) dockerdev  (1000)     8729 2022-09-29 01:07:50.000000 sbp-4.8.0/sbp/logging.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     3854 2022-09-29 01:07:50.000000 sbp-4.8.0/sbp/mag.py
--rwxr-xr-x   0 dockerdev  (1000) dockerdev  (1000)     7072 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/msg.py
--rwxr-xr-x   0 dockerdev  (1000) dockerdev  (1000)   163003 2022-09-29 01:07:50.000000 sbp-4.8.0/sbp/navigation.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     5015 2022-09-29 01:07:51.000000 sbp-4.8.0/sbp/ndb.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)   191038 2022-09-29 01:07:52.000000 sbp-4.8.0/sbp/observation.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)    15561 2022-09-29 01:07:50.000000 sbp-4.8.0/sbp/orientation.py
--rwxr-xr-x   0 dockerdev  (1000) dockerdev  (1000)    68405 2022-09-29 01:07:51.000000 sbp-4.8.0/sbp/piksi.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     3801 2022-09-29 01:07:51.000000 sbp-4.8.0/sbp/sbas.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     3646 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/sbp2json.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)    28536 2022-09-29 01:07:50.000000 sbp-4.8.0/sbp/settings.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     6766 2022-09-29 01:07:51.000000 sbp-4.8.0/sbp/signing.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)    13789 2022-09-29 01:07:50.000000 sbp-4.8.0/sbp/solution_meta.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)   101016 2022-09-29 01:07:51.000000 sbp-4.8.0/sbp/ssr.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)    43890 2022-09-29 01:07:50.000000 sbp-4.8.0/sbp/system.py
--rwxr-xr-x   0 dockerdev  (1000) dockerdev  (1000)     3880 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/table.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)    38520 2022-09-29 01:07:51.000000 sbp-4.8.0/sbp/tracking.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     3252 2022-09-29 01:07:50.000000 sbp-4.8.0/sbp/user.py
--rwxr-xr-x   0 dockerdev  (1000) dockerdev  (1000)     2495 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/utils.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     8230 2022-09-29 01:07:50.000000 sbp-4.8.0/sbp/vehicle.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     2998 2022-08-02 23:26:39.000000 sbp-4.8.0/sbp/version.py
-drwxr-xr-x   0 dockerdev  (1000) dockerdev  (1000)        0 2022-09-29 03:26:13.937110 sbp-4.8.0/sbp.egg-info/
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     3509 2022-09-29 03:26:13.000000 sbp-4.8.0/sbp.egg-info/PKG-INFO
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     1622 2022-09-29 03:26:13.000000 sbp-4.8.0/sbp.egg-info/SOURCES.txt
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)        1 2022-09-29 03:26:13.000000 sbp-4.8.0/sbp.egg-info/dependency_links.txt
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)        1 2022-05-02 00:47:39.000000 sbp-4.8.0/sbp.egg-info/not-zip-safe
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)       92 2022-09-29 03:26:13.000000 sbp-4.8.0/sbp.egg-info/requires.txt
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)       13 2022-09-29 03:26:13.000000 sbp-4.8.0/sbp.egg-info/top_level.txt
-drwxr-xr-x   0 dockerdev  (1000) dockerdev  (1000)        0 2022-09-29 03:26:13.957110 sbp-4.8.0/sbp2json/
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)        0 2022-04-27 00:14:46.000000 sbp-4.8.0/sbp2json/__init__.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)       83 2022-04-27 00:14:46.000000 sbp-4.8.0/sbp2json/__main__.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)      103 2022-09-29 03:26:13.961110 sbp-4.8.0/setup.cfg
--rwxr-xr-x   0 dockerdev  (1000) dockerdev  (1000)     6049 2022-09-29 03:26:02.000000 sbp-4.8.0/setup.py
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)       11 2022-09-29 03:26:02.000000 sbp-4.8.0/setup_requirements.txt
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)      112 2022-09-29 03:26:02.000000 sbp-4.8.0/test_requirements.txt
--rw-r--r--   0 dockerdev  (1000) dockerdev  (1000)     1050 2022-09-29 03:26:02.000000 sbp-4.8.0/tox.ini
+drwxr-xr-x   0 adriankong   (501) staff       (20)        0 2022-11-01 23:16:51.724869 sbp-4.9.0/
+-rw-r--r--   0 adriankong   (501) staff       (20)     1149 2022-11-01 23:16:45.000000 sbp-4.9.0/.gitignore
+-rw-r--r--   0 adriankong   (501) staff       (20)      225 2022-11-01 23:16:45.000000 sbp-4.9.0/MANIFEST.in
+-rw-r--r--   0 adriankong   (501) staff       (20)     2818 2022-11-01 23:16:51.724943 sbp-4.9.0/PKG-INFO
+-rw-r--r--   0 adriankong   (501) staff       (20)     1831 2022-11-01 23:16:45.000000 sbp-4.9.0/README.rst
+drwxr-xr-x   0 adriankong   (501) staff       (20)        0 2022-11-01 23:16:51.717863 sbp-4.9.0/bin/
+-rwxr-xr-x   0 adriankong   (501) staff       (20)      106 2022-04-28 06:48:13.000000 sbp-4.9.0/bin/sbp2json
+-rw-r--r--   0 adriankong   (501) staff       (20)     5192 2022-11-01 23:16:45.000000 sbp-4.9.0/deploy.py
+-rw-r--r--   0 adriankong   (501) staff       (20)       44 2022-11-01 23:16:45.000000 sbp-4.9.0/requirements.txt
+drwxr-xr-x   0 adriankong   (501) staff       (20)        0 2022-11-01 23:16:51.721807 sbp-4.9.0/sbp/
+-rw-r--r--   0 adriankong   (501) staff       (20)        5 2022-11-01 23:10:20.000000 sbp-4.9.0/sbp/RELEASE-VERSION
+-rwxr-xr-x   0 adriankong   (501) staff       (20)      636 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/__init__.py
+-rw-r--r--   0 adriankong   (501) staff       (20)      179 2022-11-01 23:16:51.000000 sbp-4.9.0/sbp/_version.py
+-rwxr-xr-x   0 adriankong   (501) staff       (20)    23052 2022-11-01 22:57:39.000000 sbp-4.9.0/sbp/acquisition.py
+-rwxr-xr-x   0 adriankong   (501) staff       (20)    14689 2022-11-01 22:57:38.000000 sbp-4.9.0/sbp/bootload.py
+drwxr-xr-x   0 adriankong   (501) staff       (20)        0 2022-11-01 23:16:51.722711 sbp-4.9.0/sbp/client/
+-rw-r--r--   0 adriankong   (501) staff       (20)      619 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/client/__init__.py
+drwxr-xr-x   0 adriankong   (501) staff       (20)        0 2022-11-01 23:16:51.723339 sbp-4.9.0/sbp/client/drivers/
+-rw-r--r--   0 adriankong   (501) staff       (20)        0 2022-04-27 00:14:46.000000 sbp-4.9.0/sbp/client/drivers/__init__.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     3204 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/client/drivers/base_driver.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     2019 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/client/drivers/cdc_driver.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     2958 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/client/drivers/file_driver.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     3912 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/client/drivers/network_drivers.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     1071 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/client/drivers/pyftdi_driver.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     3742 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/client/drivers/pyserial_driver.py
+drwxr-xr-x   0 adriankong   (501) staff       (20)        0 2022-11-01 23:16:51.723691 sbp-4.9.0/sbp/client/examples/
+-rw-r--r--   0 adriankong   (501) staff       (20)        0 2022-04-27 00:14:46.000000 sbp-4.9.0/sbp/client/examples/__init__.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     1706 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/client/examples/simple.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     1756 2022-10-27 23:11:24.000000 sbp-4.9.0/sbp/client/examples/tcp.py
+-rwxr-xr-x   0 adriankong   (501) staff       (20)     2363 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/client/examples/udp.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     1854 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/client/forwarder.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     5318 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/client/framer.py
+-rw-r--r--   0 adriankong   (501) staff       (20)    10475 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/client/handler.py
+drwxr-xr-x   0 adriankong   (501) staff       (20)        0 2022-11-01 23:16:51.724230 sbp-4.9.0/sbp/client/loggers/
+-rw-r--r--   0 adriankong   (501) staff       (20)        0 2022-04-27 00:14:46.000000 sbp-4.9.0/sbp/client/loggers/__init__.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     3237 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/client/loggers/base_logger.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     6242 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/client/loggers/json_logger.py
+-rw-r--r--   0 adriankong   (501) staff       (20)      879 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/client/loggers/null_logger.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     2074 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/client/loggers/rotating_logger.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     1264 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/client/loggers/udp_logger.py
+drwxr-xr-x   0 adriankong   (501) staff       (20)        0 2022-11-01 23:16:51.724493 sbp-4.9.0/sbp/client/util/
+-rw-r--r--   0 adriankong   (501) staff       (20)        0 2022-04-27 00:14:46.000000 sbp-4.9.0/sbp/client/util/__init__.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     6642 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/client/util/fftmonitor.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     4808 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/client/util/settingmonitor.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     2799 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/constants.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     3956 2022-11-01 22:57:38.000000 sbp-4.9.0/sbp/ext_events.py
+-rw-r--r--   0 adriankong   (501) staff       (20)    28450 2022-11-01 22:57:38.000000 sbp-4.9.0/sbp/file_io.py
+-rw-r--r--   0 adriankong   (501) staff       (20)    27810 2022-11-01 22:57:38.000000 sbp-4.9.0/sbp/flash.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     7543 2022-11-01 22:57:38.000000 sbp-4.9.0/sbp/gnss.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     7662 2022-11-01 22:57:38.000000 sbp-4.9.0/sbp/imu.py
+-rw-r--r--   0 adriankong   (501) staff       (20)    24554 2022-11-01 22:57:39.000000 sbp-4.9.0/sbp/integrity.py
+drwxr-xr-x   0 adriankong   (501) staff       (20)        0 2022-11-01 23:16:51.724592 sbp-4.9.0/sbp/jit/
+-rwxr-xr-x   0 adriankong   (501) staff       (20)       87 2022-04-27 00:14:46.000000 sbp-4.9.0/sbp/jit/__init__.py
+-rw-r--r--   0 adriankong   (501) staff       (20)    39715 2022-11-01 22:57:38.000000 sbp-4.9.0/sbp/linux.py
+-rwxr-xr-x   0 adriankong   (501) staff       (20)     8729 2022-11-01 22:57:38.000000 sbp-4.9.0/sbp/logging.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     3854 2022-11-01 22:57:38.000000 sbp-4.9.0/sbp/mag.py
+-rwxr-xr-x   0 adriankong   (501) staff       (20)     7072 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/msg.py
+-rwxr-xr-x   0 adriankong   (501) staff       (20)   163003 2022-11-01 22:57:38.000000 sbp-4.9.0/sbp/navigation.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     5015 2022-11-01 22:57:39.000000 sbp-4.9.0/sbp/ndb.py
+-rw-r--r--   0 adriankong   (501) staff       (20)   191038 2022-11-01 22:57:40.000000 sbp-4.9.0/sbp/observation.py
+-rw-r--r--   0 adriankong   (501) staff       (20)    15561 2022-11-01 22:57:38.000000 sbp-4.9.0/sbp/orientation.py
+-rwxr-xr-x   0 adriankong   (501) staff       (20)    68405 2022-11-01 22:57:39.000000 sbp-4.9.0/sbp/piksi.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     3801 2022-11-01 22:57:39.000000 sbp-4.9.0/sbp/sbas.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     3646 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/sbp2json.py
+-rw-r--r--   0 adriankong   (501) staff       (20)    28536 2022-11-01 22:57:38.000000 sbp-4.9.0/sbp/settings.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     6766 2022-11-01 22:57:39.000000 sbp-4.9.0/sbp/signing.py
+-rw-r--r--   0 adriankong   (501) staff       (20)    13789 2022-11-01 22:57:38.000000 sbp-4.9.0/sbp/solution_meta.py
+-rw-r--r--   0 adriankong   (501) staff       (20)   101016 2022-11-01 22:57:39.000000 sbp-4.9.0/sbp/ssr.py
+-rw-r--r--   0 adriankong   (501) staff       (20)    43890 2022-11-01 22:57:38.000000 sbp-4.9.0/sbp/system.py
+-rwxr-xr-x   0 adriankong   (501) staff       (20)     3880 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/table.py
+-rw-r--r--   0 adriankong   (501) staff       (20)    38520 2022-11-01 22:57:39.000000 sbp-4.9.0/sbp/tracking.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     3252 2022-11-01 22:57:38.000000 sbp-4.9.0/sbp/user.py
+-rwxr-xr-x   0 adriankong   (501) staff       (20)     2495 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/utils.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     8230 2022-11-01 22:57:38.000000 sbp-4.9.0/sbp/vehicle.py
+-rw-r--r--   0 adriankong   (501) staff       (20)     2998 2022-08-02 23:26:39.000000 sbp-4.9.0/sbp/version.py
+drwxr-xr-x   0 adriankong   (501) staff       (20)        0 2022-11-01 23:16:51.722355 sbp-4.9.0/sbp.egg-info/
+-rw-r--r--   0 adriankong   (501) staff       (20)     2818 2022-11-01 23:16:51.000000 sbp-4.9.0/sbp.egg-info/PKG-INFO
+-rw-r--r--   0 adriankong   (501) staff       (20)     1622 2022-11-01 23:16:51.000000 sbp-4.9.0/sbp.egg-info/SOURCES.txt
+-rw-r--r--   0 adriankong   (501) staff       (20)        1 2022-11-01 23:16:51.000000 sbp-4.9.0/sbp.egg-info/dependency_links.txt
+-rw-r--r--   0 adriankong   (501) staff       (20)        1 2022-05-02 00:47:39.000000 sbp-4.9.0/sbp.egg-info/not-zip-safe
+-rw-r--r--   0 adriankong   (501) staff       (20)       92 2022-11-01 23:16:51.000000 sbp-4.9.0/sbp.egg-info/requires.txt
+-rw-r--r--   0 adriankong   (501) staff       (20)       13 2022-11-01 23:16:51.000000 sbp-4.9.0/sbp.egg-info/top_level.txt
+drwxr-xr-x   0 adriankong   (501) staff       (20)        0 2022-11-01 23:16:51.724782 sbp-4.9.0/sbp2json/
+-rw-r--r--   0 adriankong   (501) staff       (20)        0 2022-04-27 00:14:46.000000 sbp-4.9.0/sbp2json/__init__.py
+-rw-r--r--   0 adriankong   (501) staff       (20)       83 2022-04-27 00:14:46.000000 sbp-4.9.0/sbp2json/__main__.py
+-rw-r--r--   0 adriankong   (501) staff       (20)      103 2022-11-01 23:16:51.725197 sbp-4.9.0/setup.cfg
+-rwxr-xr-x   0 adriankong   (501) staff       (20)     6049 2022-11-01 23:16:45.000000 sbp-4.9.0/setup.py
+-rw-r--r--   0 adriankong   (501) staff       (20)       11 2022-11-01 23:16:45.000000 sbp-4.9.0/setup_requirements.txt
+-rw-r--r--   0 adriankong   (501) staff       (20)      112 2022-11-01 23:16:45.000000 sbp-4.9.0/test_requirements.txt
+-rw-r--r--   0 adriankong   (501) staff       (20)     1050 2022-11-01 23:16:45.000000 sbp-4.9.0/tox.ini
```

### Comparing `sbp-4.8.0/.gitignore` & `sbp-4.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/README.rst` & `sbp-4.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/deploy.py` & `sbp-4.9.0/deploy.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/__init__.py` & `sbp-4.9.0/sbp/__init__.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/acquisition.py` & `sbp-4.9.0/sbp/acquisition.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/bootload.py` & `sbp-4.9.0/sbp/bootload.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/client/__init__.py` & `sbp-4.9.0/sbp/client/__init__.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/client/drivers/base_driver.py` & `sbp-4.9.0/sbp/client/drivers/base_driver.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/client/drivers/cdc_driver.py` & `sbp-4.9.0/sbp/client/drivers/cdc_driver.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/client/drivers/file_driver.py` & `sbp-4.9.0/sbp/client/drivers/file_driver.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/client/drivers/network_drivers.py` & `sbp-4.9.0/sbp/client/drivers/network_drivers.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/client/drivers/pyftdi_driver.py` & `sbp-4.9.0/sbp/client/drivers/pyftdi_driver.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/client/drivers/pyserial_driver.py` & `sbp-4.9.0/sbp/client/drivers/pyserial_driver.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/client/examples/simple.py` & `sbp-4.9.0/sbp/client/examples/simple.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/client/examples/tcp.py` & `sbp-4.9.0/sbp/client/examples/tcp.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/client/examples/udp.py` & `sbp-4.9.0/sbp/client/examples/udp.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/client/forwarder.py` & `sbp-4.9.0/sbp/client/forwarder.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/client/framer.py` & `sbp-4.9.0/sbp/client/framer.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/client/handler.py` & `sbp-4.9.0/sbp/client/handler.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/client/loggers/base_logger.py` & `sbp-4.9.0/sbp/client/loggers/base_logger.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/client/loggers/json_logger.py` & `sbp-4.9.0/sbp/client/loggers/json_logger.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/client/loggers/null_logger.py` & `sbp-4.9.0/sbp/client/loggers/null_logger.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/client/loggers/rotating_logger.py` & `sbp-4.9.0/sbp/client/loggers/rotating_logger.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/client/loggers/udp_logger.py` & `sbp-4.9.0/sbp/client/loggers/udp_logger.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/client/util/fftmonitor.py` & `sbp-4.9.0/sbp/client/util/fftmonitor.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/client/util/settingmonitor.py` & `sbp-4.9.0/sbp/client/util/settingmonitor.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/constants.py` & `sbp-4.9.0/sbp/constants.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/ext_events.py` & `sbp-4.9.0/sbp/ext_events.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/file_io.py` & `sbp-4.9.0/sbp/file_io.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/flash.py` & `sbp-4.9.0/sbp/flash.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/gnss.py` & `sbp-4.9.0/sbp/gnss.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/imu.py` & `sbp-4.9.0/sbp/imu.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/integrity.py` & `sbp-4.9.0/sbp/integrity.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/linux.py` & `sbp-4.9.0/sbp/linux.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/logging.py` & `sbp-4.9.0/sbp/logging.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/mag.py` & `sbp-4.9.0/sbp/mag.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/msg.py` & `sbp-4.9.0/sbp/msg.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/navigation.py` & `sbp-4.9.0/sbp/navigation.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/ndb.py` & `sbp-4.9.0/sbp/ndb.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/observation.py` & `sbp-4.9.0/sbp/observation.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/orientation.py` & `sbp-4.9.0/sbp/orientation.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/piksi.py` & `sbp-4.9.0/sbp/piksi.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/sbas.py` & `sbp-4.9.0/sbp/sbas.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/sbp2json.py` & `sbp-4.9.0/sbp/sbp2json.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/settings.py` & `sbp-4.9.0/sbp/settings.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/signing.py` & `sbp-4.9.0/sbp/signing.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/solution_meta.py` & `sbp-4.9.0/sbp/solution_meta.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/ssr.py` & `sbp-4.9.0/sbp/ssr.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/system.py` & `sbp-4.9.0/sbp/system.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/table.py` & `sbp-4.9.0/sbp/table.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/tracking.py` & `sbp-4.9.0/sbp/tracking.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/user.py` & `sbp-4.9.0/sbp/user.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/utils.py` & `sbp-4.9.0/sbp/utils.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/vehicle.py` & `sbp-4.9.0/sbp/vehicle.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp/version.py` & `sbp-4.9.0/sbp/version.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/sbp.egg-info/SOURCES.txt` & `sbp-4.9.0/sbp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/setup.py` & `sbp-4.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `sbp-4.8.0/tox.ini` & `sbp-4.9.0/tox.ini`

 * *Files identical despite different names*

