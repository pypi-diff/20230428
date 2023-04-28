# Comparing `tmp/RobertCommonBasic-0.1.37.tar.gz` & `tmp/RobertCommonBasic-0.1.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobertCommonBasic-0.1.37.tar", last modified: Thu Apr 27 02:31:17 2023, max compression
+gzip compressed data, was "RobertCommonBasic-0.1.38.tar", last modified: Fri Apr 28 13:07:39 2023, max compression
```

## Comparing `RobertCommonBasic-0.1.37.tar` & `RobertCommonBasic-0.1.38.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.312885 RobertCommonBasic-0.1.37/
--rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonBasic-0.1.37/LICENSE
--rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonBasic-0.1.37/MANIFEST.in
--rw-rw-rw-   0        0        0     1739 2023-04-27 02:31:17.311878 RobertCommonBasic-0.1.37/PKG-INFO
--rw-rw-rw-   0        0        0     1057 2022-01-13 05:29:18.000000 RobertCommonBasic-0.1.37/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.215372 RobertCommonBasic-0.1.37/RobertCommonBasic.egg-info/
--rw-rw-rw-   0        0        0     1739 2023-04-27 02:31:17.000000 RobertCommonBasic-0.1.37/RobertCommonBasic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4427 2023-04-27 02:31:17.000000 RobertCommonBasic-0.1.37/RobertCommonBasic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 02:31:17.000000 RobertCommonBasic-0.1.37/RobertCommonBasic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      169 2023-04-27 02:31:17.000000 RobertCommonBasic-0.1.37/RobertCommonBasic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-27 02:31:17.000000 RobertCommonBasic-0.1.37/RobertCommonBasic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      187 2023-04-19 11:40:39.000000 RobertCommonBasic-0.1.37/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.216852 RobertCommonBasic-0.1.37/robertcommonbasic/
--rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonBasic-0.1.37/robertcommonbasic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.217859 RobertCommonBasic-0.1.37/robertcommonbasic/basic/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.219864 RobertCommonBasic-0.1.37/robertcommonbasic/basic/base/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:39:20.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/base/__init__.py
--rw-rw-rw-   0        0        0      471 2023-01-04 02:45:25.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/base/constant.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.220368 RobertCommonBasic-0.1.37/robertcommonbasic/basic/cache/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/cache/__init__.py
--rw-rw-rw-   0        0        0      667 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/cache/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.222374 RobertCommonBasic-0.1.37/robertcommonbasic/basic/cls/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/cls/__init__.py
--rw-rw-rw-   0        0        0    12322 2023-04-03 03:01:59.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/cls/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.231399 RobertCommonBasic-0.1.37/robertcommonbasic/basic/data/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/data/__init__.py
--rw-rw-rw-   0        0        0    13611 2023-01-31 14:01:59.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/data/conversion.py
--rw-rw-rw-   0        0        0     4537 2022-11-14 07:54:50.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/data/crc16.py
--rw-rw-rw-   0        0        0     2229 2023-04-24 12:56:55.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/data/csv.py
--rw-rw-rw-   0        0        0    39297 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/data/datatuple.py
--rw-rw-rw-   0        0        0     8304 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/data/frame.py
--rw-rw-rw-   0        0        0     1097 2022-11-14 09:48:07.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/data/nametuple.py
--rw-rw-rw-   0        0        0       62 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/data/type.py
--rw-rw-rw-   0        0        0     5064 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/data/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.232398 RobertCommonBasic-0.1.37/robertcommonbasic/basic/decorator/
--rw-rw-rw-   0        0        0        0 2021-12-08 01:56:09.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/decorator/__init__.py
--rw-rw-rw-   0        0        0     1250 2022-12-05 08:07:43.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/decorator/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.235402 RobertCommonBasic-0.1.37/robertcommonbasic/basic/dt/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/dt/__init__.py
--rw-rw-rw-   0        0        0     4474 2022-12-28 02:51:52.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/dt/schedule.py
--rw-rw-rw-   0        0        0    10445 2023-04-10 06:28:17.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/dt/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.240928 RobertCommonBasic-0.1.37/robertcommonbasic/basic/encrypt/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/encrypt/__init__.py
--rw-rw-rw-   0        0        0      583 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/encrypt/aes.py
--rw-rw-rw-   0        0        0     3856 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/encrypt/dsa.py
--rw-rw-rw-   0        0        0      716 2023-03-09 07:09:06.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/encrypt/hash.py
--rw-rw-rw-   0        0        0      338 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/encrypt/md5.py
--rw-rw-rw-   0        0        0     2661 2022-11-14 07:25:08.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/encrypt/rsa.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.242930 RobertCommonBasic-0.1.37/robertcommonbasic/basic/error/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/error/__init__.py
--rw-rw-rw-   0        0        0     2354 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/error/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.243927 RobertCommonBasic-0.1.37/robertcommonbasic/basic/exector/
--rw-rw-rw-   0        0        0        0 2022-08-31 08:25:14.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/exector/__init__.py
--rw-rw-rw-   0        0        0     3641 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/exector/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.252201 RobertCommonBasic-0.1.37/robertcommonbasic/basic/file/
--rw-rw-rw-   0        0        0        0 2022-11-18 02:39:00.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/file/__init__.py
--rw-rw-rw-   0        0        0     3113 2023-04-24 12:56:55.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/file/csv.py
--rw-rw-rw-   0        0        0     1328 2022-11-18 03:22:13.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/file/ini.py
--rw-rw-rw-   0        0        0     1035 2022-11-18 06:23:07.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/file/log.py
--rw-rw-rw-   0        0        0     3157 2022-11-24 03:18:18.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/file/xml.py
--rw-rw-rw-   0        0        0      339 2022-11-18 06:47:46.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/file/yaml.py
--rw-rw-rw-   0        0        0     3039 2023-03-08 07:31:52.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/file/zip.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.254198 RobertCommonBasic-0.1.37/robertcommonbasic/basic/log/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/log/__init__.py
--rw-rw-rw-   0        0        0     6070 2023-04-10 02:23:47.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/log/utils.py
--rw-rw-rw-   0        0        0     1366 2022-12-05 08:20:54.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/log/watch.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.255900 RobertCommonBasic-0.1.37/robertcommonbasic/basic/net/
--rw-rw-rw-   0        0        0        0 2022-06-29 12:44:36.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/net/__init__.py
--rw-rw-rw-   0        0        0     5874 2023-04-11 03:18:26.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/net/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.260414 RobertCommonBasic-0.1.37/robertcommonbasic/basic/os/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/os/__init__.py
--rw-rw-rw-   0        0        0      228 2022-12-14 09:03:01.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/os/cmd.py
--rw-rw-rw-   0        0        0      400 2022-06-29 09:34:23.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/os/env.py
--rw-rw-rw-   0        0        0     3446 2023-03-16 09:00:41.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/os/file.py
--rw-rw-rw-   0        0        0      533 2023-02-06 07:51:13.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/os/path.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.263796 RobertCommonBasic-0.1.37/robertcommonbasic/basic/process/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/process/__init__.py
--rw-rw-rw-   0        0        0     8845 2022-12-14 08:53:18.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/process/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.264794 RobertCommonBasic-0.1.37/robertcommonbasic/basic/profile/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/profile/__init__.py
--rw-rw-rw-   0        0        0     1264 2022-11-18 02:27:39.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/profile/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.266795 RobertCommonBasic-0.1.37/robertcommonbasic/basic/re/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/re/__init__.py
--rw-rw-rw-   0        0        0     1868 2023-02-09 02:47:33.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/re/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.269980 RobertCommonBasic-0.1.37/robertcommonbasic/basic/safetext/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/safetext/__init__.py
--rw-rw-rw-   0        0        0       91 2023-02-03 07:26:22.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/safetext/converter.py
--rw-rw-rw-   0        0        0      377 2022-11-18 02:33:07.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/safetext/funcs.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.271975 RobertCommonBasic-0.1.37/robertcommonbasic/basic/sugar/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/sugar/__init__.py
--rw-rw-rw-   0        0        0      377 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/sugar/funcs.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.277680 RobertCommonBasic-0.1.37/robertcommonbasic/basic/validation/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/validation/__init__.py
--rw-rw-rw-   0        0        0    36389 2023-02-21 08:51:30.000000 RobertCommonBasic-0.1.37/robertcommonbasic/basic/validation/input.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.279877 RobertCommonBasic-0.1.37/robertcommonbasic/tests/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.279877 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:49:18.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.282085 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_cls/
--rw-rw-rw-   0        0        0        0 2022-04-22 02:07:10.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_cls/__init__.py
--rw-rw-rw-   0        0        0     1291 2023-03-02 14:03:08.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_cls/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.287031 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_data/
--rw-rw-rw-   0        0        0        0 2022-01-19 07:38:20.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_data/__init__.py
--rw-rw-rw-   0        0        0      729 2022-06-23 09:21:24.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_data/test_conversion.py
--rw-rw-rw-   0        0        0     5920 2022-04-21 06:58:53.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py
--rw-rw-rw-   0        0        0     2456 2022-01-27 05:56:15.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_data/test_frame.py
--rw-rw-rw-   0        0        0     3568 2023-04-11 13:11:50.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_data/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.288513 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_dt/
--rw-rw-rw-   0        0        0        0 2022-03-08 05:59:28.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_dt/__init__.py
--rw-rw-rw-   0        0        0     2169 2023-02-20 02:34:17.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_dt/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.295642 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_encrypt/
--rw-rw-rw-   0        0        0        0 2021-07-30 08:42:35.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_encrypt/__init__.py
--rw-rw-rw-   0        0        0    32599 2022-07-03 01:41:08.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py
--rw-rw-rw-   0        0        0      270 2022-07-03 01:04:51.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_encrypt/test_md5.py
--rw-rw-rw-   0        0        0     3004 2022-11-22 07:10:43.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.298159 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_exector/
--rw-rw-rw-   0        0        0        0 2022-08-31 08:24:08.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_exector/__init__.py
--rw-rw-rw-   0        0        0     1234 2022-12-05 09:33:27.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_exector/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.302715 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_file/
--rw-rw-rw-   0        0        0        0 2022-11-18 06:48:14.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_file/__init__.py
--rw-rw-rw-   0        0        0     1090 2023-02-03 06:30:00.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_file/test_csv.py
--rw-rw-rw-   0        0        0     4285 2023-02-02 03:00:01.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_file/test_xml.py
--rw-rw-rw-   0        0        0      705 2023-03-08 07:17:17.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_file/test_zip.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.303740 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_net/
--rw-rw-rw-   0        0        0        0 2022-06-29 13:56:13.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_net/__init__.py
--rw-rw-rw-   0        0        0      558 2023-04-11 03:14:26.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_net/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.308983 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_os/
--rw-rw-rw-   0        0        0        0 2022-03-25 04:05:00.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_os/__init__.py
--rw-rw-rw-   0        0        0      258 2022-06-29 09:29:01.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_os/test_env.py
--rw-rw-rw-   0        0        0      449 2022-11-14 02:56:25.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_os/test_file.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.310453 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_re/
--rw-rw-rw-   0        0        0        0 2022-05-18 02:57:45.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_re/__init__.py
--rw-rw-rw-   0        0        0      605 2023-04-11 09:07:57.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_re/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:31:17.310453 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_validation/
--rw-rw-rw-   0        0        0        0 2021-11-19 07:34:54.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_validation/__init__.py
--rw-rw-rw-   0        0        0      218 2022-05-10 03:46:33.000000 RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_validation/test_input.py
--rw-rw-rw-   0        0        0       42 2023-04-27 02:31:17.312885 RobertCommonBasic-0.1.37/setup.cfg
--rw-rw-rw-   0        0        0     3876 2023-04-27 02:31:09.000000 RobertCommonBasic-0.1.37/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.930976 RobertCommonBasic-0.1.38/
+-rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonBasic-0.1.38/LICENSE
+-rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonBasic-0.1.38/MANIFEST.in
+-rw-rw-rw-   0        0        0     1739 2023-04-28 13:07:39.930471 RobertCommonBasic-0.1.38/PKG-INFO
+-rw-rw-rw-   0        0        0     1057 2022-01-13 05:29:18.000000 RobertCommonBasic-0.1.38/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.794827 RobertCommonBasic-0.1.38/RobertCommonBasic.egg-info/
+-rw-rw-rw-   0        0        0     1739 2023-04-28 13:07:39.000000 RobertCommonBasic-0.1.38/RobertCommonBasic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4427 2023-04-28 13:07:39.000000 RobertCommonBasic-0.1.38/RobertCommonBasic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 13:07:39.000000 RobertCommonBasic-0.1.38/RobertCommonBasic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      169 2023-04-28 13:07:39.000000 RobertCommonBasic-0.1.38/RobertCommonBasic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-28 13:07:39.000000 RobertCommonBasic-0.1.38/RobertCommonBasic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      187 2023-04-19 11:40:39.000000 RobertCommonBasic-0.1.38/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.796825 RobertCommonBasic-0.1.38/robertcommonbasic/
+-rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonBasic-0.1.38/robertcommonbasic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.798873 RobertCommonBasic-0.1.38/robertcommonbasic/basic/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.802357 RobertCommonBasic-0.1.38/robertcommonbasic/basic/base/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:39:20.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/base/__init__.py
+-rw-rw-rw-   0        0        0      471 2023-01-04 02:45:25.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/base/constant.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.804883 RobertCommonBasic-0.1.38/robertcommonbasic/basic/cache/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/cache/__init__.py
+-rw-rw-rw-   0        0        0      667 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/cache/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.807687 RobertCommonBasic-0.1.38/robertcommonbasic/basic/cls/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/cls/__init__.py
+-rw-rw-rw-   0        0        0    12322 2023-04-03 03:01:59.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/cls/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.820304 RobertCommonBasic-0.1.38/robertcommonbasic/basic/data/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/data/__init__.py
+-rw-rw-rw-   0        0        0    13611 2023-01-31 14:01:59.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/data/conversion.py
+-rw-rw-rw-   0        0        0     4537 2022-11-14 07:54:50.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/data/crc16.py
+-rw-rw-rw-   0        0        0     2169 2023-04-28 09:36:20.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/data/csv.py
+-rw-rw-rw-   0        0        0    39297 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/data/datatuple.py
+-rw-rw-rw-   0        0        0     8304 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/data/frame.py
+-rw-rw-rw-   0        0        0     1097 2022-11-14 09:48:07.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/data/nametuple.py
+-rw-rw-rw-   0        0        0       62 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/data/type.py
+-rw-rw-rw-   0        0        0     5064 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/data/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.823379 RobertCommonBasic-0.1.38/robertcommonbasic/basic/decorator/
+-rw-rw-rw-   0        0        0        0 2021-12-08 01:56:09.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/decorator/__init__.py
+-rw-rw-rw-   0        0        0     1250 2022-12-05 08:07:43.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/decorator/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.826791 RobertCommonBasic-0.1.38/robertcommonbasic/basic/dt/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/dt/__init__.py
+-rw-rw-rw-   0        0        0     4474 2022-12-28 02:51:52.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/dt/schedule.py
+-rw-rw-rw-   0        0        0    10445 2023-04-10 06:28:17.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/dt/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.834809 RobertCommonBasic-0.1.38/robertcommonbasic/basic/encrypt/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/encrypt/__init__.py
+-rw-rw-rw-   0        0        0      583 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/encrypt/aes.py
+-rw-rw-rw-   0        0        0     3856 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/encrypt/dsa.py
+-rw-rw-rw-   0        0        0      716 2023-03-09 07:09:06.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/encrypt/hash.py
+-rw-rw-rw-   0        0        0      338 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/encrypt/md5.py
+-rw-rw-rw-   0        0        0     2661 2022-11-14 07:25:08.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/encrypt/rsa.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.837190 RobertCommonBasic-0.1.38/robertcommonbasic/basic/error/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/error/__init__.py
+-rw-rw-rw-   0        0        0     2354 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/error/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.840639 RobertCommonBasic-0.1.38/robertcommonbasic/basic/exector/
+-rw-rw-rw-   0        0        0        0 2022-08-31 08:25:14.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/exector/__init__.py
+-rw-rw-rw-   0        0        0     3641 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/exector/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.850252 RobertCommonBasic-0.1.38/robertcommonbasic/basic/file/
+-rw-rw-rw-   0        0        0        0 2022-11-18 02:39:00.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/file/__init__.py
+-rw-rw-rw-   0        0        0     3053 2023-04-28 09:36:20.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/file/csv.py
+-rw-rw-rw-   0        0        0     1328 2022-11-18 03:22:13.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/file/ini.py
+-rw-rw-rw-   0        0        0     1035 2022-11-18 06:23:07.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/file/log.py
+-rw-rw-rw-   0        0        0     3157 2022-11-24 03:18:18.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/file/xml.py
+-rw-rw-rw-   0        0        0      339 2022-11-18 06:47:46.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/file/yaml.py
+-rw-rw-rw-   0        0        0     3039 2023-03-08 07:31:52.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/file/zip.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.854733 RobertCommonBasic-0.1.38/robertcommonbasic/basic/log/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/log/__init__.py
+-rw-rw-rw-   0        0        0     6070 2023-04-10 02:23:47.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/log/utils.py
+-rw-rw-rw-   0        0        0     1366 2022-12-05 08:20:54.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/log/watch.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.857283 RobertCommonBasic-0.1.38/robertcommonbasic/basic/net/
+-rw-rw-rw-   0        0        0        0 2022-06-29 12:44:36.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/net/__init__.py
+-rw-rw-rw-   0        0        0     5874 2023-04-11 03:18:26.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/net/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.865747 RobertCommonBasic-0.1.38/robertcommonbasic/basic/os/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/os/__init__.py
+-rw-rw-rw-   0        0        0      228 2022-12-14 09:03:01.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/os/cmd.py
+-rw-rw-rw-   0        0        0      400 2022-06-29 09:34:23.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/os/env.py
+-rw-rw-rw-   0        0        0     3446 2023-03-16 09:00:41.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/os/file.py
+-rw-rw-rw-   0        0        0      533 2023-02-06 07:51:13.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/os/path.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.867989 RobertCommonBasic-0.1.38/robertcommonbasic/basic/process/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/process/__init__.py
+-rw-rw-rw-   0        0        0     8845 2022-12-14 08:53:18.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/process/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.871010 RobertCommonBasic-0.1.38/robertcommonbasic/basic/profile/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/profile/__init__.py
+-rw-rw-rw-   0        0        0     1264 2022-11-18 02:27:39.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/profile/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.873482 RobertCommonBasic-0.1.38/robertcommonbasic/basic/re/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/re/__init__.py
+-rw-rw-rw-   0        0        0     1868 2023-02-09 02:47:33.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/re/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.877484 RobertCommonBasic-0.1.38/robertcommonbasic/basic/safetext/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/safetext/__init__.py
+-rw-rw-rw-   0        0        0       91 2023-02-03 07:26:22.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/safetext/converter.py
+-rw-rw-rw-   0        0        0      377 2022-11-18 02:33:07.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/safetext/funcs.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.880483 RobertCommonBasic-0.1.38/robertcommonbasic/basic/sugar/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/sugar/__init__.py
+-rw-rw-rw-   0        0        0      377 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/sugar/funcs.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.882893 RobertCommonBasic-0.1.38/robertcommonbasic/basic/validation/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/validation/__init__.py
+-rw-rw-rw-   0        0        0    36389 2023-02-21 08:51:30.000000 RobertCommonBasic-0.1.38/robertcommonbasic/basic/validation/input.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.883899 RobertCommonBasic-0.1.38/robertcommonbasic/tests/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.884899 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:49:18.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.887011 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_cls/
+-rw-rw-rw-   0        0        0        0 2022-04-22 02:07:10.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_cls/__init__.py
+-rw-rw-rw-   0        0        0     1291 2023-03-02 14:03:08.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_cls/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.898052 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_data/
+-rw-rw-rw-   0        0        0        0 2022-01-19 07:38:20.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_data/__init__.py
+-rw-rw-rw-   0        0        0      729 2022-06-23 09:21:24.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_data/test_conversion.py
+-rw-rw-rw-   0        0        0     5920 2022-04-21 06:58:53.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py
+-rw-rw-rw-   0        0        0     2456 2022-01-27 05:56:15.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_data/test_frame.py
+-rw-rw-rw-   0        0        0     3568 2023-04-11 13:11:50.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_data/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.900137 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_dt/
+-rw-rw-rw-   0        0        0        0 2022-03-08 05:59:28.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_dt/__init__.py
+-rw-rw-rw-   0        0        0     2169 2023-02-20 02:34:17.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_dt/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.905143 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_encrypt/
+-rw-rw-rw-   0        0        0        0 2021-07-30 08:42:35.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_encrypt/__init__.py
+-rw-rw-rw-   0        0        0    32599 2022-07-03 01:41:08.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py
+-rw-rw-rw-   0        0        0      270 2022-07-03 01:04:51.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_encrypt/test_md5.py
+-rw-rw-rw-   0        0        0     3004 2022-11-22 07:10:43.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.907140 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_exector/
+-rw-rw-rw-   0        0        0        0 2022-08-31 08:24:08.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_exector/__init__.py
+-rw-rw-rw-   0        0        0     1234 2022-12-05 09:33:27.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_exector/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.913613 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_file/
+-rw-rw-rw-   0        0        0        0 2022-11-18 06:48:14.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_file/__init__.py
+-rw-rw-rw-   0        0        0     1090 2023-02-03 06:30:00.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_file/test_csv.py
+-rw-rw-rw-   0        0        0     4285 2023-02-02 03:00:01.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_file/test_xml.py
+-rw-rw-rw-   0        0        0      705 2023-03-08 07:17:17.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_file/test_zip.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.915624 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_net/
+-rw-rw-rw-   0        0        0        0 2022-06-29 13:56:13.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_net/__init__.py
+-rw-rw-rw-   0        0        0      558 2023-04-11 03:14:26.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_net/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.919789 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_os/
+-rw-rw-rw-   0        0        0        0 2022-03-25 04:05:00.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_os/__init__.py
+-rw-rw-rw-   0        0        0      258 2022-06-29 09:29:01.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_os/test_env.py
+-rw-rw-rw-   0        0        0      449 2022-11-14 02:56:25.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_os/test_file.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.922491 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_re/
+-rw-rw-rw-   0        0        0        0 2022-05-18 02:57:45.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_re/__init__.py
+-rw-rw-rw-   0        0        0      605 2023-04-11 09:07:57.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_re/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:07:39.926198 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_validation/
+-rw-rw-rw-   0        0        0        0 2021-11-19 07:34:54.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_validation/__init__.py
+-rw-rw-rw-   0        0        0      218 2022-05-10 03:46:33.000000 RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_validation/test_input.py
+-rw-rw-rw-   0        0        0       42 2023-04-28 13:07:39.930976 RobertCommonBasic-0.1.38/setup.cfg
+-rw-rw-rw-   0        0        0     3876 2023-04-28 13:04:41.000000 RobertCommonBasic-0.1.38/setup.py
```

### Comparing `RobertCommonBasic-0.1.37/LICENSE` & `RobertCommonBasic-0.1.38/LICENSE`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/PKG-INFO` & `RobertCommonBasic-0.1.38/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonBasic
-Version: 0.1.37
+Version: 0.1.38
 Summary: Robert Common Basic Library
 Home-page: https://github.com/hun0423/RobertCommonBasic
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonBasic-0.1.37/README.md` & `RobertCommonBasic-0.1.38/README.md`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/RobertCommonBasic.egg-info/PKG-INFO` & `RobertCommonBasic-0.1.38/RobertCommonBasic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonBasic
-Version: 0.1.37
+Version: 0.1.38
 Summary: Robert Common Basic Library
 Home-page: https://github.com/hun0423/RobertCommonBasic
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonBasic-0.1.37/RobertCommonBasic.egg-info/SOURCES.txt` & `RobertCommonBasic-0.1.38/RobertCommonBasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/cache/utils.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/cache/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/cls/utils.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/cls/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/data/conversion.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/data/conversion.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/data/crc16.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/data/crc16.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/data/csv.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/data/csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pandas as pd
 from io import StringIO, BytesIO
 from typing import Union, Optional
 from ..os.file import check_file_exist
 
 
-def read_csv(path: Union[str, BytesIO, StringIO], chunksize: Optional[int] = None, parse_dates: bool = False, date_format: Optional[str] = None, keep_default_na: bool = True, na_values: Optional[list] = None, names: Optional[list] = None, sep: Optional[list] = None, true_values: Optional[list] = None, false_values: Optional[list] = None) -> list:
+def read_csv(path: Union[str, BytesIO, StringIO], chunksize: Optional[int] = None, parse_dates: bool = False, keep_default_na: bool = True, na_values: Optional[list] = None, names: Optional[list] = None, sep: Optional[list] = None, true_values: Optional[list] = None, false_values: Optional[list] = None) -> list:
     results = []
-    datas = pd.read_csv(path, chunksize=chunksize, low_memory=False, parse_dates=parse_dates, date_format=date_format, names=names, sep=sep, true_values=true_values, false_values=false_values, keep_default_na=keep_default_na, na_values=na_values)
+    datas = pd.read_csv(path, chunksize=chunksize, low_memory=False, parse_dates=parse_dates, names=names, sep=sep, true_values=true_values, false_values=false_values, keep_default_na=keep_default_na, na_values=na_values)
     if chunksize is not None:
         for data in datas:
             for index, row in data.iterrows():
                 results.append(row.to_dict())
     else:
         for index, row in datas.iterrows():
             results.append(row.to_dict())
```

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/data/datatuple.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/data/datatuple.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/data/frame.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/data/frame.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/data/nametuple.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/data/nametuple.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/data/utils.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/data/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/decorator/utils.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/decorator/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/dt/schedule.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/dt/schedule.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/dt/utils.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/dt/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/encrypt/aes.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/encrypt/aes.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/encrypt/dsa.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/encrypt/dsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/encrypt/hash.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/encrypt/hash.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/encrypt/rsa.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/encrypt/rsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/error/utils.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/error/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/exector/utils.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/exector/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/file/csv.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/file/csv.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import pandas as pd
 from io import StringIO, BytesIO
 from typing import Union, Optional
 from ..os.file import check_file_exist, get_file_folder
 from ..os.path import create_dir_if_not_exist
 
 
-def read_csv(path: Union[str, BytesIO, StringIO], chunksize: Optional[int] = None, parse_dates: bool = False, date_format: Optional[str] = None, keep_default_na: bool = True, na_values: Optional[list] = None, names: Optional[list] = None, sep: Optional[str] = None, true_values: Optional[list] = None, false_values: Optional[list] = None) -> list:
+def read_csv(path: Union[str, BytesIO, StringIO], chunksize: Optional[int] = None, parse_dates: bool = False, keep_default_na: bool = True, na_values: Optional[list] = None, names: Optional[list] = None, sep: Optional[str] = None, true_values: Optional[list] = None, false_values: Optional[list] = None) -> list:
     results = []
-    datas = pd.read_csv(path, chunksize=chunksize, low_memory=False, parse_dates=parse_dates, date_format=date_format, names=names, sep=sep, true_values=true_values, false_values=false_values, keep_default_na=keep_default_na, na_values=na_values)
+    datas = pd.read_csv(path, chunksize=chunksize, low_memory=False, parse_dates=parse_dates, names=names, sep=sep, true_values=true_values, false_values=false_values, keep_default_na=keep_default_na, na_values=na_values)
     if chunksize is not None:
         for data in datas:
             for index, row in data.iterrows():
                 results.append(row.to_dict())
     else:
         for index, row in datas.iterrows():
             results.append(row.to_dict())
```

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/file/ini.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/file/ini.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/file/log.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/file/log.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/file/xml.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/file/xml.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/file/zip.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/file/zip.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/log/utils.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/log/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/log/watch.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/log/watch.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/net/utils.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/net/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/os/file.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/os/file.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/os/path.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/os/path.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/process/utils.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/process/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/profile/utils.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/profile/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/re/utils.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/re/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/basic/validation/input.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/basic/validation/input.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_cls/test_utils.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_cls/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_data/test_conversion.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_data/test_conversion.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_data/test_frame.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_data/test_frame.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_data/test_utils.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_data/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_dt/test_utils.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_dt/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_exector/test_utils.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_exector/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_file/test_csv.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_file/test_csv.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_file/test_xml.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_file/test_xml.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_file/test_zip.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_file/test_zip.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_net/test_utils.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_net/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/robertcommonbasic/tests/test_basic/test_re/test_utils.py` & `RobertCommonBasic-0.1.38/robertcommonbasic/tests/test_basic/test_re/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.37/setup.py` & `RobertCommonBasic-0.1.38/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # Package meta-data.
 NAME = 'RobertCommonBasic'
 DESCRIPTION = 'Robert Common Basic Library'
 URL = 'https://github.com/hun0423/RobertCommonBasic'
 EMAIL = '851010070@qq.com'
 AUTHOR = 'Robert0423'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.37'
-DATE = '2023-04-27'
+VERSION = '0.1.38'
+DATE = '2023-04-28'
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

