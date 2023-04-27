# Comparing `tmp/codext-1.9.4.tar.gz` & `tmp/codext-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codext-1.9.4.tar", last modified: Mon Oct 25 17:20:33 2021, max compression
+gzip compressed data, was "codext-1.9.5.tar", last modified: Sun Nov 14 08:53:30 2021, max compression
```

## Comparing `codext-1.9.4.tar` & `codext-1.9.5.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2021-10-25 17:20:33.069233 codext-1.9.4/
--rw-rw-r--   0 morfal    (1000) morfal    (1000)    35823 2021-03-03 22:12:30.000000 codext-1.9.4/LICENSE
--rw-rw-r--   0 morfal    (1000) morfal    (1000)    11989 2021-10-25 17:20:33.069233 codext-1.9.4/PKG-INFO
--rw-rw-r--   0 morfal    (1000) morfal    (1000)    11159 2021-10-24 09:35:27.000000 codext-1.9.4/README.md
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2021-10-25 17:20:33.065232 codext-1.9.4/codext/
--rw-rw-r--   0 morfal    (1000) morfal    (1000)        7 2021-10-25 17:20:22.000000 codext-1.9.4/codext/VERSION.txt
--rw-rw-r--   0 morfal    (1000) morfal    (1000)    51822 2021-10-25 17:18:36.000000 codext-1.9.4/codext/__common__.py
--rw-rw-r--   0 morfal    (1000) morfal    (1000)      505 2021-03-03 22:12:30.000000 codext-1.9.4/codext/__info__.py
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     8774 2021-10-25 17:05:49.000000 codext-1.9.4/codext/__init__.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2021-10-25 17:20:33.065232 codext-1.9.4/codext/base/
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2690 2021-10-18 19:29:48.000000 codext-1.9.4/codext/base/__init__.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     9125 2021-10-21 13:28:56.000000 codext-1.9.4/codext/base/_base.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     4304 2021-10-23 22:05:15.000000 codext-1.9.4/codext/base/_base2n.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      784 2021-03-03 22:12:30.000000 codext-1.9.4/codext/base/ascii85.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1699 2021-10-18 17:31:49.000000 codext-1.9.4/codext/base/base100.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     3524 2021-10-19 10:01:36.000000 codext-1.9.4/codext/base/base122.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2824 2021-10-19 08:44:16.000000 codext-1.9.4/codext/base/base45.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1500 2021-10-19 10:01:26.000000 codext-1.9.4/codext/base/base85.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     4440 2021-10-17 08:47:48.000000 codext-1.9.4/codext/base/base91.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     3974 2021-10-19 18:17:50.000000 codext-1.9.4/codext/base/baseN.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2021-10-25 17:20:33.069233 codext-1.9.4/codext/binary/
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      165 2021-03-03 22:12:30.000000 codext-1.9.4/codext/binary/__init__.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)    13808 2021-03-03 22:12:30.000000 codext-1.9.4/codext/binary/baudot.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     3122 2021-03-03 22:12:30.000000 codext-1.9.4/codext/binary/bcd.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2163 2021-03-03 22:12:30.000000 codext-1.9.4/codext/binary/excess3.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      622 2021-03-03 22:12:30.000000 codext-1.9.4/codext/binary/gray.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1751 2021-03-03 22:12:30.000000 codext-1.9.4/codext/binary/manchester.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1478 2021-06-28 07:01:41.000000 codext-1.9.4/codext/binary/rotate.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2021-10-25 17:20:33.069233 codext-1.9.4/codext/common/
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      117 2021-03-03 22:12:30.000000 codext-1.9.4/codext/common/__init__.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1850 2021-03-03 22:12:30.000000 codext-1.9.4/codext/common/a1z26.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1398 2021-03-03 22:12:30.000000 codext-1.9.4/codext/common/dummy.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1013 2021-03-03 22:12:30.000000 codext-1.9.4/codext/common/octal.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      918 2021-03-03 22:12:30.000000 codext-1.9.4/codext/common/ordinal.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2021-10-25 17:20:33.069233 codext-1.9.4/codext/compressions/
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      113 2021-10-03 06:58:54.000000 codext-1.9.4/codext/compressions/__init__.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1218 2021-10-03 15:33:00.000000 codext-1.9.4/codext/compressions/gzipp.py
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     2308 2021-10-03 15:32:38.000000 codext-1.9.4/codext/compressions/lz77.py
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     2514 2021-10-03 15:31:53.000000 codext-1.9.4/codext/compressions/lz78.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1728 2021-10-24 10:40:50.000000 codext-1.9.4/codext/compressions/pkzip.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2021-10-25 17:20:33.069233 codext-1.9.4/codext/crypto/
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      227 2021-03-03 22:12:30.000000 codext-1.9.4/codext/crypto/__init__.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      986 2021-03-03 22:12:30.000000 codext-1.9.4/codext/crypto/affine.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1101 2021-03-03 22:12:30.000000 codext-1.9.4/codext/crypto/atbash.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1271 2021-03-03 22:12:30.000000 codext-1.9.4/codext/crypto/bacon.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2102 2021-06-28 07:18:58.000000 codext-1.9.4/codext/crypto/barbie.py
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     1403 2021-10-02 22:07:49.000000 codext-1.9.4/codext/crypto/citrix.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1567 2021-10-24 11:09:17.000000 codext-1.9.4/codext/crypto/rot.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1487 2021-06-28 07:18:42.000000 codext-1.9.4/codext/crypto/scytale.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      935 2021-06-28 07:18:09.000000 codext-1.9.4/codext/crypto/shift.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1004 2021-06-28 07:18:47.000000 codext-1.9.4/codext/crypto/xor.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2021-10-25 17:20:33.069233 codext-1.9.4/codext/languages/
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      215 2021-03-03 22:12:30.000000 codext-1.9.4/codext/languages/__init__.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1339 2021-03-03 22:12:30.000000 codext-1.9.4/codext/languages/braille.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     4630 2021-03-03 22:12:30.000000 codext-1.9.4/codext/languages/ipsum.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      664 2021-03-03 22:12:30.000000 codext-1.9.4/codext/languages/leetspeak.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1665 2021-09-17 10:42:39.000000 codext-1.9.4/codext/languages/morse.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1737 2021-03-03 22:12:30.000000 codext-1.9.4/codext/languages/navajo.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1101 2021-03-03 22:12:30.000000 codext-1.9.4/codext/languages/radio.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2238 2021-03-03 22:12:30.000000 codext-1.9.4/codext/languages/southpark.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1151 2021-03-03 22:12:30.000000 codext-1.9.4/codext/languages/tomtom.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2021-10-25 17:20:33.069233 codext-1.9.4/codext/others/
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      137 2021-10-01 11:34:25.000000 codext-1.9.4/codext/others/__init__.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1688 2021-03-03 22:12:30.000000 codext-1.9.4/codext/others/dna.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)    29273 2021-03-03 22:12:30.000000 codext-1.9.4/codext/others/html.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     3157 2021-03-03 22:12:30.000000 codext-1.9.4/codext/others/letters.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      664 2021-03-03 22:12:30.000000 codext-1.9.4/codext/others/markdown.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      811 2021-03-03 22:12:30.000000 codext-1.9.4/codext/others/url.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2021-10-25 17:20:33.069233 codext-1.9.4/codext/stegano/
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      121 2021-09-25 08:24:42.000000 codext-1.9.4/codext/stegano/__init__.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      657 2021-09-25 08:27:22.000000 codext-1.9.4/codext/stegano/klopf.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1094 2021-03-03 22:12:30.000000 codext-1.9.4/codext/stegano/resistor.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      917 2021-03-03 22:12:30.000000 codext-1.9.4/codext/stegano/sms.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2398 2021-06-28 14:24:41.000000 codext-1.9.4/codext/stegano/whitespace.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2021-10-25 17:20:33.065232 codext-1.9.4/codext.egg-info/
--rw-rw-r--   0 morfal    (1000) morfal    (1000)    11989 2021-10-25 17:20:32.000000 codext-1.9.4/codext.egg-info/PKG-INFO
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     1813 2021-10-25 17:20:32.000000 codext-1.9.4/codext.egg-info/SOURCES.txt
--rw-rw-r--   0 morfal    (1000) morfal    (1000)        1 2021-10-25 17:20:32.000000 codext-1.9.4/codext.egg-info/dependency_links.txt
--rw-rw-r--   0 morfal    (1000) morfal    (1000)      947 2021-10-25 17:20:32.000000 codext-1.9.4/codext.egg-info/entry_points.txt
--rw-rw-r--   0 morfal    (1000) morfal    (1000)       95 2021-10-25 17:20:32.000000 codext-1.9.4/codext.egg-info/requires.txt
--rw-rw-r--   0 morfal    (1000) morfal    (1000)       13 2021-10-25 17:20:32.000000 codext-1.9.4/codext.egg-info/top_level.txt
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     2277 2021-10-25 17:20:33.073233 codext-1.9.4/setup.cfg
--rw-rw-r--   0 morfal    (1000) morfal    (1000)       64 2021-03-03 22:12:30.000000 codext-1.9.4/setup.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2021-10-25 17:20:33.069233 codext-1.9.4/tests/
--rw-rw-r--   0 morfal    (1000) morfal    (1000)        0 2021-03-03 22:12:30.000000 codext-1.9.4/tests/__init__.py
--rw-rw-r--   0 morfal    (1000) morfal    (1000)    12920 2021-10-19 08:57:21.000000 codext-1.9.4/tests/test_base.py
--rw-rw-r--   0 morfal    (1000) morfal    (1000)    11213 2021-10-19 08:41:57.000000 codext-1.9.4/tests/test_common.py
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     7087 2021-10-19 10:00:41.000000 codext-1.9.4/tests/test_generated.py
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     6214 2021-03-03 22:12:30.000000 codext-1.9.4/tests/test_manual.py
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2021-11-14 08:53:30.455854 codext-1.9.5/
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)    35823 2021-03-03 22:12:30.000000 codext-1.9.5/LICENSE
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)    14594 2021-11-14 08:53:30.455854 codext-1.9.5/PKG-INFO
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)    13789 2021-11-06 10:27:51.000000 codext-1.9.5/README.md
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2021-11-14 08:53:30.451854 codext-1.9.5/codext/
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)        7 2021-11-14 08:53:15.000000 codext-1.9.5/codext/VERSION.txt
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)    52182 2021-11-14 08:43:51.000000 codext-1.9.5/codext/__common__.py
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)      505 2021-03-03 22:12:30.000000 codext-1.9.5/codext/__info__.py
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)     8794 2021-10-25 19:56:55.000000 codext-1.9.5/codext/__init__.py
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2021-11-14 08:53:30.451854 codext-1.9.5/codext/base/
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2690 2021-10-18 19:29:48.000000 codext-1.9.5/codext/base/__init__.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     9191 2021-10-27 19:40:35.000000 codext-1.9.5/codext/base/_base.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     4304 2021-10-23 22:05:15.000000 codext-1.9.5/codext/base/_base2n.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)      784 2021-03-03 22:12:30.000000 codext-1.9.5/codext/base/ascii85.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1699 2021-10-18 17:31:49.000000 codext-1.9.5/codext/base/base100.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     3524 2021-10-19 10:01:36.000000 codext-1.9.5/codext/base/base122.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2824 2021-10-19 08:44:16.000000 codext-1.9.5/codext/base/base45.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1500 2021-10-19 10:01:26.000000 codext-1.9.5/codext/base/base85.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     4440 2021-10-17 08:47:48.000000 codext-1.9.5/codext/base/base91.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     4026 2021-10-25 19:19:15.000000 codext-1.9.5/codext/base/baseN.py
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2021-11-14 08:53:30.455854 codext-1.9.5/codext/binary/
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)      165 2021-03-03 22:12:30.000000 codext-1.9.5/codext/binary/__init__.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)    13808 2021-03-03 22:12:30.000000 codext-1.9.5/codext/binary/baudot.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     3122 2021-03-03 22:12:30.000000 codext-1.9.5/codext/binary/bcd.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2146 2021-10-27 19:52:48.000000 codext-1.9.5/codext/binary/excess3.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)      622 2021-03-03 22:12:30.000000 codext-1.9.5/codext/binary/gray.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1751 2021-03-03 22:12:30.000000 codext-1.9.5/codext/binary/manchester.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1466 2021-10-27 19:53:12.000000 codext-1.9.5/codext/binary/rotate.py
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2021-11-14 08:53:30.455854 codext-1.9.5/codext/common/
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)      117 2021-03-03 22:12:30.000000 codext-1.9.5/codext/common/__init__.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1850 2021-03-03 22:12:30.000000 codext-1.9.5/codext/common/a1z26.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1398 2021-03-03 22:12:30.000000 codext-1.9.5/codext/common/dummy.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1013 2021-03-03 22:12:30.000000 codext-1.9.5/codext/common/octal.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)      918 2021-03-03 22:12:30.000000 codext-1.9.5/codext/common/ordinal.py
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2021-11-14 08:53:30.455854 codext-1.9.5/codext/compressions/
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)      113 2021-10-03 06:58:54.000000 codext-1.9.5/codext/compressions/__init__.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1218 2021-10-03 15:33:00.000000 codext-1.9.5/codext/compressions/gzipp.py
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)     2308 2021-10-03 15:32:38.000000 codext-1.9.5/codext/compressions/lz77.py
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)     2514 2021-10-03 15:31:53.000000 codext-1.9.5/codext/compressions/lz78.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1972 2021-11-14 08:46:29.000000 codext-1.9.5/codext/compressions/pkzip.py
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2021-11-14 08:53:30.455854 codext-1.9.5/codext/crypto/
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)      227 2021-03-03 22:12:30.000000 codext-1.9.5/codext/crypto/__init__.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)      986 2021-03-03 22:12:30.000000 codext-1.9.5/codext/crypto/affine.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1101 2021-03-03 22:12:30.000000 codext-1.9.5/codext/crypto/atbash.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1271 2021-03-03 22:12:30.000000 codext-1.9.5/codext/crypto/bacon.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2102 2021-06-28 07:18:58.000000 codext-1.9.5/codext/crypto/barbie.py
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)     1403 2021-10-02 22:07:49.000000 codext-1.9.5/codext/crypto/citrix.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1567 2021-10-24 11:09:17.000000 codext-1.9.5/codext/crypto/rot.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1487 2021-06-28 07:18:42.000000 codext-1.9.5/codext/crypto/scytale.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)      935 2021-06-28 07:18:09.000000 codext-1.9.5/codext/crypto/shift.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1004 2021-06-28 07:18:47.000000 codext-1.9.5/codext/crypto/xor.py
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2021-11-14 08:53:30.455854 codext-1.9.5/codext/languages/
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)      215 2021-03-03 22:12:30.000000 codext-1.9.5/codext/languages/__init__.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1339 2021-03-03 22:12:30.000000 codext-1.9.5/codext/languages/braille.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     4630 2021-03-03 22:12:30.000000 codext-1.9.5/codext/languages/ipsum.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)      664 2021-03-03 22:12:30.000000 codext-1.9.5/codext/languages/leetspeak.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1665 2021-09-17 10:42:39.000000 codext-1.9.5/codext/languages/morse.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1737 2021-03-03 22:12:30.000000 codext-1.9.5/codext/languages/navajo.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1101 2021-03-03 22:12:30.000000 codext-1.9.5/codext/languages/radio.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2238 2021-03-03 22:12:30.000000 codext-1.9.5/codext/languages/southpark.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1151 2021-03-03 22:12:30.000000 codext-1.9.5/codext/languages/tomtom.py
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2021-11-14 08:53:30.455854 codext-1.9.5/codext/others/
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)      137 2021-10-01 11:34:25.000000 codext-1.9.5/codext/others/__init__.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1688 2021-03-03 22:12:30.000000 codext-1.9.5/codext/others/dna.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)    29273 2021-03-03 22:12:30.000000 codext-1.9.5/codext/others/html.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     3157 2021-03-03 22:12:30.000000 codext-1.9.5/codext/others/letters.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)      664 2021-03-03 22:12:30.000000 codext-1.9.5/codext/others/markdown.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)      811 2021-03-03 22:12:30.000000 codext-1.9.5/codext/others/url.py
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2021-11-14 08:53:30.455854 codext-1.9.5/codext/stegano/
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)      121 2021-09-25 08:24:42.000000 codext-1.9.5/codext/stegano/__init__.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)      657 2021-09-25 08:27:22.000000 codext-1.9.5/codext/stegano/klopf.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1094 2021-03-03 22:12:30.000000 codext-1.9.5/codext/stegano/resistor.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)      917 2021-03-03 22:12:30.000000 codext-1.9.5/codext/stegano/sms.py
+-rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2398 2021-06-28 14:24:41.000000 codext-1.9.5/codext/stegano/whitespace.py
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2021-11-14 08:53:30.451854 codext-1.9.5/codext.egg-info/
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)    14594 2021-11-14 08:53:30.000000 codext-1.9.5/codext.egg-info/PKG-INFO
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)     1813 2021-11-14 08:53:30.000000 codext-1.9.5/codext.egg-info/SOURCES.txt
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)        1 2021-11-14 08:53:30.000000 codext-1.9.5/codext.egg-info/dependency_links.txt
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)      947 2021-11-14 08:53:30.000000 codext-1.9.5/codext.egg-info/entry_points.txt
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)       95 2021-11-14 08:53:30.000000 codext-1.9.5/codext.egg-info/requires.txt
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)       13 2021-11-14 08:53:30.000000 codext-1.9.5/codext.egg-info/top_level.txt
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)     2277 2021-11-14 08:53:30.459854 codext-1.9.5/setup.cfg
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)       64 2021-03-03 22:12:30.000000 codext-1.9.5/setup.py
+drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2021-11-14 08:53:30.455854 codext-1.9.5/tests/
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)        0 2021-03-03 22:12:30.000000 codext-1.9.5/tests/__init__.py
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)    12920 2021-10-19 08:57:21.000000 codext-1.9.5/tests/test_base.py
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)    11563 2021-11-14 08:15:38.000000 codext-1.9.5/tests/test_common.py
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)     7087 2021-10-19 10:00:41.000000 codext-1.9.5/tests/test_generated.py
+-rw-rw-r--   0 morfal    (1000) morfal    (1000)     6214 2021-03-03 22:12:30.000000 codext-1.9.5/tests/test_manual.py
```

### Comparing `codext-1.9.4/LICENSE` & `codext-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/PKG-INFO` & `codext-1.9.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,750 +1,862 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 636f 6465  : 2.1.Name: code
-00000020: 7874 0a56 6572 7369 6f6e 3a20 312e 392e  xt.Version: 1.9.
-00000030: 340a 5375 6d6d 6172 793a 204e 6174 6976  4.Summary: Nativ
-00000040: 6520 636f 6465 6373 2065 7874 656e 7369  e codecs extensi
-00000050: 6f6e 0a48 6f6d 652d 7061 6765 3a20 6874  on.Home-page: ht
-00000060: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000070: 2f64 686f 6e64 7461 2f70 7974 686f 6e2d  /dhondta/python-
-00000080: 636f 6465 7874 0a41 7574 686f 723a 2041  codext.Author: A
-00000090: 6c65 7861 6e64 7265 2044 2748 6f6e 6474  lexandre D'Hondt
-000000a0: 0a41 7574 686f 722d 656d 6169 6c3a 2061  .Author-email: a
-000000b0: 6c65 7861 6e64 7265 2e64 686f 6e64 7440  lexandre.dhondt@
-000000c0: 676d 6169 6c2e 636f 6d0a 4c69 6365 6e73  gmail.com.Licens
-000000d0: 653a 2047 504c 7633 0a4b 6579 776f 7264  e: GPLv3.Keyword
-000000e0: 733a 2070 7974 686f 6e2c 6465 7665 6c6f  s: python,develo
-000000f0: 706d 656e 742c 7072 6f67 7261 6d6d 696e  pment,programmin
-00000100: 672c 636f 6465 6373 2c65 6e63 6f64 696e  g,codecs,encodin
-00000110: 6773 0a50 6c61 7466 6f72 6d3a 2055 4e4b  gs.Platform: UNK
-00000120: 4e4f 574e 0a43 6c61 7373 6966 6965 723a  NOWN.Classifier:
-00000130: 2044 6576 656c 6f70 6d65 6e74 2053 7461   Development Sta
-00000140: 7475 7320 3a3a 2035 202d 2050 726f 6475  tus :: 5 - Produ
-00000150: 6374 696f 6e2f 5374 6162 6c65 0a43 6c61  ction/Stable.Cla
-00000160: 7373 6966 6965 723a 2045 6e76 6972 6f6e  ssifier: Environ
-00000170: 6d65 6e74 203a 3a20 436f 6e73 6f6c 650a  ment :: Console.
-00000180: 436c 6173 7369 6669 6572 3a20 496e 7465  Classifier: Inte
-00000190: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
-000001a0: 2044 6576 656c 6f70 6572 730a 436c 6173   Developers.Clas
-000001b0: 7369 6669 6572 3a20 4c69 6365 6e73 6520  sifier: License 
-000001c0: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-000001d0: 3a3a 2047 4e55 2047 656e 6572 616c 2050  :: GNU General P
-000001e0: 7562 6c69 6320 4c69 6365 6e73 6520 7633  ublic License v3
-000001f0: 2028 4750 4c76 3329 0a43 6c61 7373 6966   (GPLv3).Classif
-00000200: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000210: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000220: 686f 6e20 3a3a 2032 0a43 6c61 7373 6966  hon :: 2.Classif
-00000230: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000240: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000250: 686f 6e20 3a3a 2032 2e37 0a43 6c61 7373  hon :: 2.7.Class
-00000260: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000270: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000280: 7974 686f 6e20 3a3a 2033 0a43 6c61 7373  ython :: 3.Class
-00000290: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-000002a0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000002b0: 7974 686f 6e20 3a3a 2033 2e36 0a43 6c61  ython :: 3.6.Cla
-000002c0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-000002d0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000002e0: 2050 7974 686f 6e20 3a3a 2033 2e37 0a43   Python :: 3.7.C
-000002f0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00000300: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000310: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
-00000320: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000330: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000340: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000350: 2e39 0a43 6c61 7373 6966 6965 723a 2054  .9.Classifier: T
-00000360: 6f70 6963 203a 3a20 536f 6674 7761 7265  opic :: Software
-00000370: 2044 6576 656c 6f70 6d65 6e74 203a 3a20   Development :: 
-00000380: 4c69 6272 6172 6965 7320 3a3a 2050 7974  Libraries :: Pyt
-00000390: 686f 6e20 4d6f 6475 6c65 730a 5265 7175  hon Modules.Requ
-000003a0: 6972 6573 2d50 7974 686f 6e3a 2021 3d33  ires-Python: !=3
-000003b0: 2e30 2e2a 2c21 3d33 2e31 2e2a 2c21 3d33  .0.*,!=3.1.*,!=3
-000003c0: 2e32 2e2a 2c21 3d33 2e33 2e2a 2c21 3d33  .2.*,!=3.3.*,!=3
-000003d0: 2e34 2e2a 2c21 3d33 2e35 2e2a 2c3c 342c  .4.*,!=3.5.*,<4,
-000003e0: 3e3d 322e 370a 4465 7363 7269 7074 696f  >=2.7.Descriptio
-000003f0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
-00000400: 7465 7874 2f6d 6172 6b64 6f77 6e0a 4c69  text/markdown.Li
-00000410: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
-00000420: 4e53 450a 0a5b 215b 5079 5069 5d28 6874  NSE..[![PyPi](ht
-00000430: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000440: 732e 696f 2f70 7970 692f 762f 636f 6465  s.io/pypi/v/code
-00000450: 7874 2e73 7667 295d 2868 7474 7073 3a2f  xt.svg)](https:/
-00000460: 2f70 7970 692e 7079 7468 6f6e 2e6f 7267  /pypi.python.org
-00000470: 2f70 7970 692f 636f 6465 7874 2f29 0a5b  /pypi/codext/).[
-00000480: 215b 5265 6164 2054 6865 2044 6f63 735d  ![Read The Docs]
-00000490: 2868 7474 7073 3a2f 2f72 6561 6474 6865  (https://readthe
-000004a0: 646f 6373 2e6f 7267 2f70 726f 6a65 6374  docs.org/project
-000004b0: 732f 7079 7468 6f6e 2d63 6f64 6578 742f  s/python-codext/
-000004c0: 6261 6467 652f 3f76 6572 7369 6f6e 3d6c  badge/?version=l
-000004d0: 6174 6573 7429 5d28 6874 7470 733a 2f2f  atest)](https://
-000004e0: 7079 7468 6f6e 2d63 6f64 6578 742e 7265  python-codext.re
-000004f0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00000500: 6c61 7465 7374 2f3f 6261 6467 653d 6c61  latest/?badge=la
-00000510: 7465 7374 290a 5b21 5b42 7569 6c64 2053  test).[![Build S
-00000520: 7461 7475 735d 2868 7474 7073 3a2f 2f74  tatus](https://t
-00000530: 7261 7669 732d 6369 2e63 6f6d 2f64 686f  ravis-ci.com/dho
-00000540: 6e64 7461 2f70 7974 686f 6e2d 636f 6465  ndta/python-code
-00000550: 7874 2e73 7667 3f62 7261 6e63 683d 6d61  xt.svg?branch=ma
-00000560: 7374 6572 295d 2868 7474 7073 3a2f 2f74  ster)](https://t
-00000570: 7261 7669 732d 6369 2e63 6f6d 2f64 686f  ravis-ci.com/dho
-00000580: 6e64 7461 2f70 7974 686f 6e2d 636f 6465  ndta/python-code
-00000590: 7874 290a 5b21 5b43 6f76 6572 6167 6520  xt).[![Coverage 
-000005a0: 5374 6174 7573 5d28 6874 7470 733a 2f2f  Status](https://
-000005b0: 636f 7665 7261 6c6c 732e 696f 2f72 6570  coveralls.io/rep
-000005c0: 6f73 2f67 6974 6875 622f 6468 6f6e 6474  os/github/dhondt
-000005d0: 612f 7079 7468 6f6e 2d63 6f64 6578 742f  a/python-codext/
-000005e0: 6261 6467 652e 7376 673f 6272 616e 6368  badge.svg?branch
-000005f0: 3d6d 6173 7465 7229 5d28 6874 7470 733a  =master)](https:
-00000600: 2f2f 636f 7665 7261 6c6c 732e 696f 2f67  //coveralls.io/g
-00000610: 6974 6875 622f 6468 6f6e 6474 612f 7079  ithub/dhondta/py
-00000620: 7468 6f6e 2d63 6f64 6578 743f 6272 616e  thon-codext?bran
-00000630: 6368 3d6d 6173 7465 7229 0a5b 215b 5079  ch=master).[![Py
-00000640: 7468 6f6e 2056 6572 7369 6f6e 735d 2868  thon Versions](h
-00000650: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000660: 6473 2e69 6f2f 7079 7069 2f70 7976 6572  ds.io/pypi/pyver
-00000670: 7369 6f6e 732f 636f 6465 7874 2e73 7667  sions/codext.svg
-00000680: 295d 2868 7474 7073 3a2f 2f70 7970 692e  )](https://pypi.
-00000690: 7079 7468 6f6e 2e6f 7267 2f70 7970 692f  python.org/pypi/
-000006a0: 636f 6465 7874 2f29 0a5b 215b 5265 7175  codext/).[![Requ
-000006b0: 6972 656d 656e 7473 2053 7461 7475 735d  irements Status]
-000006c0: 2868 7474 7073 3a2f 2f72 6571 7569 7265  (https://require
-000006d0: 732e 696f 2f67 6974 6875 622f 6468 6f6e  s.io/github/dhon
-000006e0: 6474 612f 7079 7468 6f6e 2d63 6f64 6578  dta/python-codex
-000006f0: 742f 7265 7175 6972 656d 656e 7473 2e73  t/requirements.s
-00000700: 7667 3f62 7261 6e63 683d 6d61 7374 6572  vg?branch=master
-00000710: 295d 2868 7474 7073 3a2f 2f72 6571 7569  )](https://requi
-00000720: 7265 732e 696f 2f67 6974 6875 622f 6468  res.io/github/dh
-00000730: 6f6e 6474 612f 7079 7468 6f6e 2d63 6f64  ondta/python-cod
-00000740: 6578 742f 7265 7175 6972 656d 656e 7473  ext/requirements
-00000750: 2f3f 6272 616e 6368 3d6d 6173 7465 7229  /?branch=master)
-00000760: 0a5b 215b 4b6e 6f77 6e20 5675 6c6e 6572  .[![Known Vulner
-00000770: 6162 696c 6974 6965 735d 2868 7474 7073  abilities](https
-00000780: 3a2f 2f73 6e79 6b2e 696f 2f74 6573 742f  ://snyk.io/test/
-00000790: 6769 7468 7562 2f64 686f 6e64 7461 2f70  github/dhondta/p
-000007a0: 7974 686f 6e2d 636f 6465 7874 2f62 6164  ython-codext/bad
-000007b0: 6765 2e73 7667 3f74 6172 6765 7446 696c  ge.svg?targetFil
-000007c0: 653d 7265 7175 6972 656d 656e 7473 2e74  e=requirements.t
-000007d0: 7874 295d 2868 7474 7073 3a2f 2f73 6e79  xt)](https://sny
-000007e0: 6b2e 696f 2f74 6573 742f 6769 7468 7562  k.io/test/github
-000007f0: 2f64 686f 6e64 7461 2f70 7974 686f 6e2d  /dhondta/python-
-00000800: 636f 6465 7874 3f74 6172 6765 7446 696c  codext?targetFil
-00000810: 653d 7265 7175 6972 656d 656e 7473 2e74  e=requirements.t
-00000820: 7874 290a 5b21 5b4c 6963 656e 7365 5d28  xt).[![License](
-00000830: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000840: 6c64 732e 696f 2f70 7970 692f 6c2f 636f  lds.io/pypi/l/co
-00000850: 6465 7874 2e73 7667 295d 2868 7474 7073  dext.svg)](https
-00000860: 3a2f 2f70 7970 692e 7079 7468 6f6e 2e6f  ://pypi.python.o
-00000870: 7267 2f70 7970 692f 636f 6465 7874 2f29  rg/pypi/codext/)
-00000880: 0a0a 2323 2049 6e74 726f 6475 6374 696f  ..## Introductio
-00000890: 6e0a 0a54 6869 7320 6c69 6272 6172 7920  n..This library 
-000008a0: 6578 7465 6e64 7320 7468 6520 6e61 7469  extends the nati
-000008b0: 7665 205b 6063 6f64 6563 7360 5d28 6874  ve [`codecs`](ht
-000008c0: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
-000008d0: 6e2e 6f72 672f 332f 6c69 6272 6172 792f  n.org/3/library/
-000008e0: 636f 6465 6373 2e68 746d 6c29 206c 6962  codecs.html) lib
-000008f0: 7261 7279 2028 6e61 6d65 6c79 2066 6f72  rary (namely for
-00000900: 2061 6464 696e 6720 6e65 7720 6375 7374   adding new cust
-00000910: 6f6d 2065 6e63 6f64 696e 6773 2061 6e64  om encodings and
-00000920: 2063 6861 7261 6374 6572 206d 6170 7069   character mappi
-00000930: 6e67 7329 2061 6e64 2070 726f 7669 6465  ngs) and provide
-00000940: 7320 6120 6d79 7269 6164 206f 6620 6e65  s a myriad of ne
-00000950: 7720 656e 636f 6469 6e67 7320 2873 7461  w encodings (sta
-00000960: 7469 6320 6f72 2070 6172 616d 6574 7269  tic or parametri
-00000970: 7a65 642c 206c 696b 6520 6072 6f74 6020  zed, like `rot` 
-00000980: 6f72 2060 786f 7260 292c 2068 656e 6365  or `xor`), hence
-00000990: 2069 7473 206e 616d 6564 2063 6f6d 6269   its named combi
-000009a0: 6e69 6e67 202a 434f 4465 6373 2045 5854  ning *CODecs EXT
-000009b0: 656e 7369 6f6e 2a2e 0a0a 0a0a 2323 2053  ension*.....## S
-000009c0: 6574 7570 0a0a 6060 6073 680a 2420 7069  etup..```sh.$ pi
-000009d0: 7020 696e 7374 616c 6c20 636f 6465 7874  p install codext
-000009e0: 0a60 6060 0a0a 2a2a 4e6f 7465 2a2a 3a20  .```..**Note**: 
-000009f0: 536f 6d65 2065 6e63 6f64 696e 6773 2061  Some encodings a
-00000a00: 7265 2061 7661 696c 6162 6c65 2069 6e20  re available in 
-00000a10: 5079 7468 6f6e 2033 206f 6e6c 792e 0a0a  Python 3 only...
-00000a20: 2323 2044 656d 6f6e 7374 7261 7469 6f6e  ## Demonstration
-00000a30: 730a 0a3c 7020 616c 6967 6e3d 2263 656e  s..<p align="cen
-00000a40: 7465 7222 3e3c 696d 6720 7372 633d 2268  ter"><img src="h
-00000a50: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-00000a60: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00000a70: 2f64 686f 6e64 7461 2f70 7974 686f 6e2d  /dhondta/python-
-00000a80: 636f 6465 7874 2f6d 6173 7465 722f 646f  codext/master/do
-00000a90: 6373 2f64 656d 6f73 2f75 7369 6e67 2d63  cs/demos/using-c
-00000aa0: 6f64 6578 742e 6769 6622 2061 6c74 3d22  odext.gif" alt="
-00000ab0: 5573 696e 6720 436f 6445 7874 2066 726f  Using CodExt fro
-00000ac0: 6d20 7468 6520 636f 6d6d 616e 6420 6c69  m the command li
-00000ad0: 6e65 223e 3c2f 703e 0a3c 7020 616c 6967  ne"></p>.<p alig
-00000ae0: 6e3d 2263 656e 7465 7222 3e3c 696d 6720  n="center"><img 
-00000af0: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
-00000b00: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00000b10: 6e74 2e63 6f6d 2f64 686f 6e64 7461 2f70  nt.com/dhondta/p
-00000b20: 7974 686f 6e2d 636f 6465 7874 2f6d 6173  ython-codext/mas
-00000b30: 7465 722f 646f 6373 2f64 656d 6f73 2f75  ter/docs/demos/u
-00000b40: 7369 6e67 2d62 6173 6573 2e67 6966 2220  sing-bases.gif" 
-00000b50: 616c 743d 2255 7369 6e67 2062 6173 6520  alt="Using base 
-00000b60: 746f 6f6c 7320 6672 6f6d 2074 6865 2063  tools from the c
-00000b70: 6f6d 6d61 6e64 206c 696e 6522 3e3c 2f70  ommand line"></p
-00000b80: 3e0a 3c70 2061 6c69 676e 3d22 6365 6e74  >.<p align="cent
-00000b90: 6572 223e 3c69 6d67 2073 7263 3d22 6874  er"><img src="ht
-00000ba0: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00000bb0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00000bc0: 6468 6f6e 6474 612f 7079 7468 6f6e 2d63  dhondta/python-c
-00000bd0: 6f64 6578 742f 6d61 7374 6572 2f64 6f63  odext/master/doc
-00000be0: 732f 6465 6d6f 732f 7573 696e 672d 6465  s/demos/using-de
-00000bf0: 6261 7365 2e67 6966 2220 616c 743d 2255  base.gif" alt="U
-00000c00: 7369 6e67 2074 6865 2064 6562 6173 6520  sing the debase 
-00000c10: 636f 6d6d 616e 6420 6c69 6e65 2074 6f6f  command line too
-00000c20: 6c22 3e3c 2f70 3e0a 0a23 2320 5573 6167  l"></p>..## Usag
-00000c30: 6520 2843 4c49 2074 6f6f 6c29 0a0a 6060  e (CLI tool)..``
-00000c40: 6073 680a 2420 636f 6465 7874 202d 6920  `sh.$ codext -i 
-00000c50: 7465 7374 2e74 7874 2065 6e63 6f64 6520  test.txt encode 
-00000c60: 646e 612d 310a 4754 4741 4743 4747 4754  dna-1.GTGAGCGGGT
-00000c70: 4154 4754 4741 0a24 2065 6368 6f20 2d65  ATGTGA.$ echo -e
-00000c80: 6e20 2274 6573 7422 207c 2063 6f64 6578  n "test" | codex
-00000c90: 7420 656e 636f 6465 206d 6f72 7365 0a2d  t encode morse.-
-00000ca0: 202e 202e 2e2e 202d 0a60 6060 0a0a 5079   . ... -.```..Py
-00000cb0: 7468 6f6e 2033 2028 696e 636c 7564 6573  thon 3 (includes
-00000cc0: 2041 7363 6969 3835 2c20 4261 7365 3835   Ascii85, Base85
-00000cd0: 2c20 4261 7365 3130 3020 616e 6420 6272  , Base100 and br
-00000ce0: 6169 6c6c 6529 3a0a 0a60 6060 7368 0a24  aille):..```sh.$
-00000cf0: 2065 6368 6f20 2d65 6e20 2274 6573 7422   echo -en "test"
-00000d00: 207c 2063 6f64 6578 7420 656e 636f 6465   | codext encode
-00000d10: 2062 7261 696c 6c65 0ae2 a09e e2a0 91e2   braille........
-00000d20: a08e e2a0 9e0a 2420 6563 686f 202d 656e  ......$ echo -en
-00000d30: 2022 7465 7374 2220 7c20 636f 6465 7874   "test" | codext
-00000d40: 2065 6e63 6f64 6520 6261 7365 3130 300a   encode base100.
-00000d50: f09f 91ab f09f 919c f09f 91aa f09f 91ab  ................
-00000d60: 0a60 6060 0a0a 5573 696e 6720 636f 6465  .```..Using code
-00000d70: 6373 2063 6861 696e 696e 673a 0a0a 6060  cs chaining:..``
-00000d80: 6073 680a 2420 6563 686f 202d 656e 2022  `sh.$ echo -en "
-00000d90: 5465 7374 2073 7472 696e 6722 207c 2063  Test string" | c
-00000da0: 6f64 6578 7420 656e 636f 6465 2072 6576  odext encode rev
-00000db0: 6572 7365 0a67 6e69 7274 7320 7473 6554  erse.gnirts tseT
-00000dc0: 0a24 2065 6368 6f20 2d65 6e20 2254 6573  .$ echo -en "Tes
-00000dd0: 7420 7374 7269 6e67 2220 7c20 636f 6465  t string" | code
-00000de0: 7874 2065 6e63 6f64 6520 7265 7665 7273  xt encode revers
-00000df0: 6520 6d6f 7273 650a 2d2d 2e20 2d2e 202e  e morse.--. -. .
-00000e00: 2e20 2e2d 2e20 2d20 2e2e 2e20 2f20 2d20  . .-. - ... / - 
-00000e10: 2e2e 2e20 2e20 2d0a 2420 6563 686f 202d  ... . -.$ echo -
-00000e20: 656e 2022 5465 7374 2073 7472 696e 6722  en "Test string"
-00000e30: 207c 2063 6f64 6578 7420 656e 636f 6465   | codext encode
-00000e40: 2072 6576 6572 7365 206d 6f72 7365 2064   reverse morse d
-00000e50: 6e61 2d32 0a41 4754 4341 4754 4341 4754  na-2.AGTCAGTCAGT
-00000e60: 4741 4741 4141 4754 4341 4754 4741 4741  GAGAAAGTCAGTGAGA
-00000e70: 4141 4754 4741 4754 4741 4741 4141 4754  AAGTGAGTGAGAAAGT
-00000e80: 4741 4754 4341 4754 4741 4741 4141 4754  GAGTCAGTGAGAAAGT
+00000000: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
+00000010: 7222 3e43 6f64 4578 7420 3c61 2068 7265  r">CodExt <a hre
+00000020: 663d 2268 7474 7073 3a2f 2f74 7769 7474  f="https://twitt
+00000030: 6572 2e63 6f6d 2f69 6e74 656e 742f 7477  er.com/intent/tw
+00000040: 6565 743f 7465 7874 3d43 6f64 4578 7425  eet?text=CodExt%
+00000050: 3230 2d25 3230 456e 636f 6469 6e67 2532  20-%20Encoding%2
+00000060: 4664 6563 6f64 696e 6725 3230 616e 7974  Fdecoding%20anyt
+00000070: 6869 6e67 2e25 3044 2530 4150 7974 686f  hing.%0D%0APytho
+00000080: 6e25 3230 6c69 6272 6172 7925 3230 6578  n%20library%20ex
+00000090: 7465 6e64 696e 6725 3230 7468 6525 3230  tending%20the%20
+000000a0: 6e61 7469 7665 2532 3063 6f64 6563 7325  native%20codecs%
+000000b0: 3230 6c69 6272 6172 7925 3230 7769 7468  20library%20with
+000000c0: 2532 306d 616e 7925 3230 6e65 7725 3230  %20many%20new%20
+000000d0: 656e 636f 6469 6e67 7325 3230 616e 6425  encodings%20and%
+000000e0: 3230 7072 6f76 6964 696e 6725 3230 434c  20providing%20CL
+000000f0: 4925 3230 746f 6f6c 7325 3230 7769 7468  I%20tools%20with
+00000100: 2532 3061 2532 3067 7565 7373 2532 3066  %20a%20guess%20f
+00000110: 6561 7475 7265 2532 3062 6173 6564 2532  eature%20based%2
+00000120: 306f 6e25 3230 4149 2e25 3044 2530 4168  0on%20AI.%0D%0Ah
+00000130: 7474 7073 2533 6125 3266 2532 6667 6974  ttps%3a%2f%2fgit
+00000140: 6875 6225 3265 636f 6d25 3266 6468 6f6e  hub%2ecom%2fdhon
+00000150: 6474 6125 3266 7079 7468 6f6e 2d63 6f64  dta%2fpython-cod
+00000160: 6578 7425 3044 2530 4126 6861 7368 7461  ext%0D%0A&hashta
+00000170: 6773 3d70 7974 686f 6e2c 7072 6f67 7261  gs=python,progra
+00000180: 6d6d 696e 672c 656e 636f 6469 6e67 732c  mming,encodings,
+00000190: 636f 6465 6373 2c63 7279 7074 6f67 7261  codecs,cryptogra
+000001a0: 7068 792c 6d6f 7273 652c 6261 7365 2c63  phy,morse,base,c
+000001b0: 7466 746f 6f6c 7322 3e3c 696d 6720 7372  tftools"><img sr
+000001c0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+000001d0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+000001e0: 5477 6565 742d 2d6c 6967 6874 6772 6579  Tweet--lightgrey
+000001f0: 3f6c 6f67 6f3d 7477 6974 7465 7226 7374  ?logo=twitter&st
+00000200: 796c 653d 736f 6369 616c 2220 616c 743d  yle=social" alt=
+00000210: 2254 7765 6574 2220 6865 6967 6874 3d22  "Tweet" height="
+00000220: 3230 222f 3e3c 2f61 3e3c 2f68 313e 0d0a  20"/></a></h1>..
+00000230: 3c68 3320 616c 6967 6e3d 2263 656e 7465  <h3 align="cente
+00000240: 7222 3e45 6e63 6f64 652f 6465 636f 6465  r">Encode/decode
+00000250: 2061 6e79 7468 696e 672e 3c2f 6833 3e0d   anything.</h3>.
+00000260: 0a0d 0a5b 215b 5079 5069 5d28 6874 7470  ...[![PyPi](http
+00000270: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000280: 696f 2f70 7970 692f 762f 636f 6465 7874  io/pypi/v/codext
+00000290: 2e73 7667 295d 2868 7474 7073 3a2f 2f70  .svg)](https://p
+000002a0: 7970 692e 7079 7468 6f6e 2e6f 7267 2f70  ypi.python.org/p
+000002b0: 7970 692f 636f 6465 7874 2f29 0d0a 5b21  ypi/codext/)..[!
+000002c0: 5b52 6561 6420 5468 6520 446f 6373 5d28  [Read The Docs](
+000002d0: 6874 7470 733a 2f2f 7265 6164 7468 6564  https://readthed
+000002e0: 6f63 732e 6f72 672f 7072 6f6a 6563 7473  ocs.org/projects
+000002f0: 2f70 7974 686f 6e2d 636f 6465 7874 2f62  /python-codext/b
+00000300: 6164 6765 2f3f 7665 7273 696f 6e3d 6c61  adge/?version=la
+00000310: 7465 7374 295d 2868 7474 7073 3a2f 2f70  test)](https://p
+00000320: 7974 686f 6e2d 636f 6465 7874 2e72 6561  ython-codext.rea
+00000330: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+00000340: 6174 6573 742f 3f62 6164 6765 3d6c 6174  atest/?badge=lat
+00000350: 6573 7429 0d0a 5b21 5b42 7569 6c64 2053  est)..[![Build S
+00000360: 7461 7475 735d 2868 7474 7073 3a2f 2f74  tatus](https://t
+00000370: 7261 7669 732d 6369 2e63 6f6d 2f64 686f  ravis-ci.com/dho
+00000380: 6e64 7461 2f70 7974 686f 6e2d 636f 6465  ndta/python-code
+00000390: 7874 2e73 7667 3f62 7261 6e63 683d 6d61  xt.svg?branch=ma
+000003a0: 7374 6572 295d 2868 7474 7073 3a2f 2f74  ster)](https://t
+000003b0: 7261 7669 732d 6369 2e63 6f6d 2f64 686f  ravis-ci.com/dho
+000003c0: 6e64 7461 2f70 7974 686f 6e2d 636f 6465  ndta/python-code
+000003d0: 7874 290d 0a5b 215b 436f 7665 7261 6765  xt)..[![Coverage
+000003e0: 2053 7461 7475 735d 2868 7474 7073 3a2f   Status](https:/
+000003f0: 2f63 6f76 6572 616c 6c73 2e69 6f2f 7265  /coveralls.io/re
+00000400: 706f 732f 6769 7468 7562 2f64 686f 6e64  pos/github/dhond
+00000410: 7461 2f70 7974 686f 6e2d 636f 6465 7874  ta/python-codext
+00000420: 2f62 6164 6765 2e73 7667 3f62 7261 6e63  /badge.svg?branc
+00000430: 683d 6d61 7374 6572 295d 2868 7474 7073  h=master)](https
+00000440: 3a2f 2f63 6f76 6572 616c 6c73 2e69 6f2f  ://coveralls.io/
+00000450: 6769 7468 7562 2f64 686f 6e64 7461 2f70  github/dhondta/p
+00000460: 7974 686f 6e2d 636f 6465 7874 3f62 7261  ython-codext?bra
+00000470: 6e63 683d 6d61 7374 6572 290d 0a5b 215b  nch=master)..[![
+00000480: 5079 7468 6f6e 2056 6572 7369 6f6e 735d  Python Versions]
+00000490: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+000004a0: 656c 6473 2e69 6f2f 7079 7069 2f70 7976  elds.io/pypi/pyv
+000004b0: 6572 7369 6f6e 732f 636f 6465 7874 2e73  ersions/codext.s
+000004c0: 7667 295d 2868 7474 7073 3a2f 2f70 7970  vg)](https://pyp
+000004d0: 692e 7079 7468 6f6e 2e6f 7267 2f70 7970  i.python.org/pyp
+000004e0: 692f 636f 6465 7874 2f29 0d0a 5b21 5b52  i/codext/)..[![R
+000004f0: 6571 7569 7265 6d65 6e74 7320 5374 6174  equirements Stat
+00000500: 7573 5d28 6874 7470 733a 2f2f 7265 7175  us](https://requ
+00000510: 6972 6573 2e69 6f2f 6769 7468 7562 2f64  ires.io/github/d
+00000520: 686f 6e64 7461 2f70 7974 686f 6e2d 636f  hondta/python-co
+00000530: 6465 7874 2f72 6571 7569 7265 6d65 6e74  dext/requirement
+00000540: 732e 7376 673f 6272 616e 6368 3d6d 6173  s.svg?branch=mas
+00000550: 7465 7229 5d28 6874 7470 733a 2f2f 7265  ter)](https://re
+00000560: 7175 6972 6573 2e69 6f2f 6769 7468 7562  quires.io/github
+00000570: 2f64 686f 6e64 7461 2f70 7974 686f 6e2d  /dhondta/python-
+00000580: 636f 6465 7874 2f72 6571 7569 7265 6d65  codext/requireme
+00000590: 6e74 732f 3f62 7261 6e63 683d 6d61 7374  nts/?branch=mast
+000005a0: 6572 290d 0a5b 215b 4b6e 6f77 6e20 5675  er)..[![Known Vu
+000005b0: 6c6e 6572 6162 696c 6974 6965 735d 2868  lnerabilities](h
+000005c0: 7474 7073 3a2f 2f73 6e79 6b2e 696f 2f74  ttps://snyk.io/t
+000005d0: 6573 742f 6769 7468 7562 2f64 686f 6e64  est/github/dhond
+000005e0: 7461 2f70 7974 686f 6e2d 636f 6465 7874  ta/python-codext
+000005f0: 2f62 6164 6765 2e73 7667 3f74 6172 6765  /badge.svg?targe
+00000600: 7446 696c 653d 7265 7175 6972 656d 656e  tFile=requiremen
+00000610: 7473 2e74 7874 295d 2868 7474 7073 3a2f  ts.txt)](https:/
+00000620: 2f73 6e79 6b2e 696f 2f74 6573 742f 6769  /snyk.io/test/gi
+00000630: 7468 7562 2f64 686f 6e64 7461 2f70 7974  thub/dhondta/pyt
+00000640: 686f 6e2d 636f 6465 7874 3f74 6172 6765  hon-codext?targe
+00000650: 7446 696c 653d 7265 7175 6972 656d 656e  tFile=requiremen
+00000660: 7473 2e74 7874 290d 0a5b 215b 4c69 6365  ts.txt)..[![Lice
+00000670: 6e73 655d 2868 7474 7073 3a2f 2f69 6d67  nse](https://img
+00000680: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00000690: 2f6c 2f63 6f64 6578 742e 7376 6729 5d28  /l/codext.svg)](
+000006a0: 6874 7470 733a 2f2f 7079 7069 2e70 7974  https://pypi.pyt
+000006b0: 686f 6e2e 6f72 672f 7079 7069 2f63 6f64  hon.org/pypi/cod
+000006c0: 6578 742f 290d 0a0d 0a54 6869 7320 6c69  ext/)....This li
+000006d0: 6272 6172 7920 6578 7465 6e64 7320 7468  brary extends th
+000006e0: 6520 6e61 7469 7665 205b 6063 6f64 6563  e native [`codec
+000006f0: 7360 5d28 6874 7470 733a 2f2f 646f 6373  s`](https://docs
+00000700: 2e70 7974 686f 6e2e 6f72 672f 332f 6c69  .python.org/3/li
+00000710: 6272 6172 792f 636f 6465 6373 2e68 746d  brary/codecs.htm
+00000720: 6c29 206c 6962 7261 7279 2028 6e61 6d65  l) library (name
+00000730: 6c79 2066 6f72 2061 6464 696e 6720 6e65  ly for adding ne
+00000740: 7720 6375 7374 6f6d 2065 6e63 6f64 696e  w custom encodin
+00000750: 6773 2061 6e64 2063 6861 7261 6374 6572  gs and character
+00000760: 206d 6170 7069 6e67 7329 2061 6e64 2070   mappings) and p
+00000770: 726f 7669 6465 7320 6120 6d79 7269 6164  rovides a myriad
+00000780: 206f 6620 6e65 7720 656e 636f 6469 6e67   of new encoding
+00000790: 7320 2873 7461 7469 6320 6f72 2070 6172  s (static or par
+000007a0: 616d 6574 7269 7a65 642c 206c 696b 6520  ametrized, like 
+000007b0: 6072 6f74 6020 6f72 2060 786f 7260 292c  `rot` or `xor`),
+000007c0: 2068 656e 6365 2069 7473 206e 616d 6564   hence its named
+000007d0: 2063 6f6d 6269 6e69 6e67 202a 434f 4465   combining *CODe
+000007e0: 6373 2045 5854 656e 7369 6f6e 2a2e 0d0a  cs EXTension*...
+000007f0: 0d0a 6060 6073 680d 0a24 2070 6970 2069  ..```sh..$ pip i
+00000800: 6e73 7461 6c6c 2063 6f64 6578 740d 0a60  nstall codext..`
+00000810: 6060 0d0a 0d0a 2323 203a 6d61 673a 2044  ``....## :mag: D
+00000820: 656d 6f6e 7374 7261 7469 6f6e 730d 0a0d  emonstrations...
+00000830: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000840: 7222 3e3c 696d 6720 7372 633d 2268 7474  r"><img src="htt
+00000850: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00000860: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f64  sercontent.com/d
+00000870: 686f 6e64 7461 2f70 7974 686f 6e2d 636f  hondta/python-co
+00000880: 6465 7874 2f6d 6173 7465 722f 646f 6373  dext/master/docs
+00000890: 2f64 656d 6f73 2f75 7369 6e67 2d63 6f64  /demos/using-cod
+000008a0: 6578 742e 6769 6622 2061 6c74 3d22 5573  ext.gif" alt="Us
+000008b0: 696e 6720 436f 6445 7874 2066 726f 6d20  ing CodExt from 
+000008c0: 7468 6520 636f 6d6d 616e 6420 6c69 6e65  the command line
+000008d0: 223e 3c2f 703e 0d0a 3c70 2061 6c69 676e  "></p>..<p align
+000008e0: 3d22 6365 6e74 6572 223e 3c69 6d67 2073  ="center"><img s
+000008f0: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+00000900: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00000910: 742e 636f 6d2f 6468 6f6e 6474 612f 7079  t.com/dhondta/py
+00000920: 7468 6f6e 2d63 6f64 6578 742f 6d61 7374  thon-codext/mast
+00000930: 6572 2f64 6f63 732f 6465 6d6f 732f 7573  er/docs/demos/us
+00000940: 696e 672d 6261 7365 732e 6769 6622 2061  ing-bases.gif" a
+00000950: 6c74 3d22 5573 696e 6720 6261 7365 2074  lt="Using base t
+00000960: 6f6f 6c73 2066 726f 6d20 7468 6520 636f  ools from the co
+00000970: 6d6d 616e 6420 6c69 6e65 223e 3c2f 703e  mmand line"></p>
+00000980: 0d0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
+00000990: 6572 223e 3c69 6d67 2073 7263 3d22 6874  er"><img src="ht
+000009a0: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+000009b0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+000009c0: 6468 6f6e 6474 612f 7079 7468 6f6e 2d63  dhondta/python-c
+000009d0: 6f64 6578 742f 6d61 7374 6572 2f64 6f63  odext/master/doc
+000009e0: 732f 6465 6d6f 732f 7573 696e 672d 6465  s/demos/using-de
+000009f0: 6261 7365 2e67 6966 2220 616c 743d 2255  base.gif" alt="U
+00000a00: 7369 6e67 2074 6865 2064 6562 6173 6520  sing the debase 
+00000a10: 636f 6d6d 616e 6420 6c69 6e65 2074 6f6f  command line too
+00000a20: 6c22 3e3c 2f70 3e0d 0a0d 0a23 2320 3a63  l"></p>....## :c
+00000a30: 6f6d 7075 7465 723a 2055 7361 6765 2028  omputer: Usage (
+00000a40: 6d61 696e 2043 4c49 2074 6f6f 6c29 203c  main CLI tool) <
+00000a50: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000a60: 7477 6974 7465 722e 636f 6d2f 696e 7465  twitter.com/inte
+00000a70: 6e74 2f74 7765 6574 3f74 6578 743d 436f  nt/tweet?text=Co
+00000a80: 6445 7874 2532 302d 2532 3045 6e63 6f64  dExt%20-%20Encod
+00000a90: 6525 3246 6465 636f 6465 2532 3061 6e79  e%2Fdecode%20any
+00000aa0: 7468 696e 672e 2530 4425 3041 5079 7468  thing.%0D%0APyth
+00000ab0: 6f6e 2532 3074 6f6f 6c25 3230 666f 7225  on%20tool%20for%
+00000ac0: 3230 656e 636f 6469 6e67 2532 3061 6e64  20encoding%20and
+00000ad0: 2532 3064 6563 6f64 696e 6725 3230 616c  %20decoding%20al
+00000ae0: 6d6f 7374 2532 3061 6e79 7468 696e 672c  most%20anything,
+00000af0: 2532 3069 6e63 6c75 6469 6e67 2532 3061  %20including%20a
+00000b00: 2532 3067 7565 7373 2532 3066 6561 7475  %20guess%20featu
+00000b10: 7265 2532 3062 6173 6564 2532 306f 6e25  re%20based%20on%
+00000b20: 3230 4149 2e25 3044 2530 4168 7474 7073  20AI.%0D%0Ahttps
+00000b30: 2533 6125 3266 2532 6667 6974 6875 6225  %3a%2f%2fgithub%
+00000b40: 3265 636f 6d25 3266 6468 6f6e 6474 6125  2ecom%2fdhondta%
+00000b50: 3266 7079 7468 6f6e 2d63 6f64 6578 7425  2fpython-codext%
+00000b60: 3044 2530 4126 6861 7368 7461 6773 3d70  0D%0A&hashtags=p
+00000b70: 7974 686f 6e2c 656e 636f 6469 6e67 732c  ython,encodings,
+00000b80: 636f 6465 6373 2c63 7279 7074 6f67 7261  codecs,cryptogra
+00000b90: 7068 792c 6d6f 7273 652c 6261 7365 2c73  phy,morse,base,s
+00000ba0: 7465 6761 6e6f 2c73 7465 6761 6e6f 6772  tegano,steganogr
+00000bb0: 6170 6879 2c63 7466 746f 6f6c 7322 3e3c  aphy,ctftools"><
+00000bc0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000bd0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000be0: 6261 6467 652f 5477 6565 7425 3230 2863  badge/Tweet%20(c
+00000bf0: 6f64 6578 7429 2d2d 6c69 6768 7467 7265  odext)--lightgre
+00000c00: 793f 6c6f 676f 3d74 7769 7474 6572 2673  y?logo=twitter&s
+00000c10: 7479 6c65 3d73 6f63 6961 6c22 2061 6c74  tyle=social" alt
+00000c20: 3d22 5477 6565 7420 6f6e 2063 6f64 6578  ="Tweet on codex
+00000c30: 7422 2068 6569 6768 743d 2232 3022 2f3e  t" height="20"/>
+00000c40: 3c2f 613e 0d0a 0d0a 6060 6073 6573 7369  </a>....```sessi
+00000c50: 6f6e 0d0a 2420 636f 6465 7874 202d 6920  on..$ codext -i 
+00000c60: 7465 7374 2e74 7874 2065 6e63 6f64 6520  test.txt encode 
+00000c70: 646e 612d 310d 0a47 5447 4147 4347 4747  dna-1..GTGAGCGGG
+00000c80: 5441 5447 5447 410d 0a0d 0a24 2065 6368  TATGTGA....$ ech
+00000c90: 6f20 2d65 6e20 2274 6573 7422 207c 2063  o -en "test" | c
+00000ca0: 6f64 6578 7420 656e 636f 6465 206d 6f72  odext encode mor
+00000cb0: 7365 0d0a 2d20 2e20 2e2e 2e20 2d0d 0a0d  se..- . ... -...
+00000cc0: 0a24 2065 6368 6f20 2d65 6e20 2274 6573  .$ echo -en "tes
+00000cd0: 7422 207c 2063 6f64 6578 7420 656e 636f  t" | codext enco
+00000ce0: 6465 2062 7261 696c 6c65 0d0a e2a0 9ee2  de braille......
+00000cf0: a091 e2a0 8ee2 a09e 0d0a 0d0a 2420 6563  ............$ ec
+00000d00: 686f 202d 656e 2022 7465 7374 2220 7c20  ho -en "test" | 
+00000d10: 636f 6465 7874 2065 6e63 6f64 6520 6261  codext encode ba
+00000d20: 7365 3130 300d 0af0 9f91 abf0 9f91 9cf0  se100...........
+00000d30: 9f91 aaf0 9f91 ab0d 0a60 6060 0d0a 0d0a  .........```....
+00000d40: 4368 6169 6e69 6e67 2063 6f64 6563 733a  Chaining codecs:
+00000d50: 0d0a 0d0a 6060 6073 680d 0a24 2065 6368  ....```sh..$ ech
+00000d60: 6f20 2d65 6e20 2254 6573 7420 7374 7269  o -en "Test stri
+00000d70: 6e67 2220 7c20 636f 6465 7874 2065 6e63  ng" | codext enc
+00000d80: 6f64 6520 7265 7665 7273 650d 0a67 6e69  ode reverse..gni
+00000d90: 7274 7320 7473 6554 0d0a 0d0a 2420 6563  rts tseT....$ ec
+00000da0: 686f 202d 656e 2022 5465 7374 2073 7472  ho -en "Test str
+00000db0: 696e 6722 207c 2063 6f64 6578 7420 656e  ing" | codext en
+00000dc0: 636f 6465 2072 6576 6572 7365 206d 6f72  code reverse mor
+00000dd0: 7365 0d0a 2d2d 2e20 2d2e 202e 2e20 2e2d  se..--. -. .. .-
+00000de0: 2e20 2d20 2e2e 2e20 2f20 2d20 2e2e 2e20  . - ... / - ... 
+00000df0: 2e20 2d0d 0a0d 0a24 2065 6368 6f20 2d65  . -....$ echo -e
+00000e00: 6e20 2254 6573 7420 7374 7269 6e67 2220  n "Test string" 
+00000e10: 7c20 636f 6465 7874 2065 6e63 6f64 6520  | codext encode 
+00000e20: 7265 7665 7273 6520 6d6f 7273 6520 646e  reverse morse dn
+00000e30: 612d 320d 0a41 4754 4341 4754 4341 4754  a-2..AGTCAGTCAGT
+00000e40: 4741 4741 4141 4754 4341 4754 4741 4741  GAGAAAGTCAGTGAGA
+00000e50: 4141 4754 4741 4754 4741 4741 4141 4754  AAGTGAGTGAGAAAGT
+00000e60: 4741 4754 4341 4754 4741 4741 4141 4754  GAGTCAGTGAGAAAGT
+00000e70: 4341 4741 4141 4754 4741 4754 4741 4754  CAGAAAGTGAGTGAGT
+00000e80: 4741 4741 4141 4754 5441 4741 4141 4754  GAGAAAGTTAGAAAGT
 00000e90: 4341 4741 4141 4754 4741 4754 4741 4754  CAGAAAGTGAGTGAGT
-00000ea0: 4741 4741 4141 4754 5441 4741 4141 4754  GAGAAAGTTAGAAAGT
-00000eb0: 4341 4741 4141 4754 4741 4754 4741 4754  CAGAAAGTGAGTGAGT
-00000ec0: 4741 4741 4141 4754 4741 4741 4141 4754  GAGAAAGTGAGAAAGT
-00000ed0: 430a 2420 6563 686f 202d 656e 2022 5465  C.$ echo -en "Te
-00000ee0: 7374 2073 7472 696e 6722 207c 2063 6f64  st string" | cod
-00000ef0: 6578 7420 656e 636f 6465 2072 6576 6572  ext encode rever
-00000f00: 7365 206d 6f72 7365 2064 6e61 2d32 206f  se morse dna-2 o
-00000f10: 6374 616c 0a31 3031 3130 3731 3234 3130  ctal.10110712410
-00000f20: 3331 3031 3130 3731 3234 3130 3331 3031  3101107124103101
-00000f30: 3130 3731 3234 3130 3731 3031 3130 3731  1071241071011071
-00000f40: 3031 3130 3131 3031 3130 3731 3234 3130  0110110110712410
-00000f50: 3331 3031 3130 3731 3234 3130 3731 3031  3101107124107101
-00000f60: 3130 3731 3031 3130 3131 3031 3130 3731  1071011011011071
-00000f70: 3234 3130 3731 3031 3130 3731 3234 3130  2410710110712410
-00000f80: 3731 3031 3130 3731 3031 3130 3131 3031  7101107101101101
-00000f90: 3130 3731 3234 3130 3731 3031 3130 3731  1071241071011071
-00000fa0: 3234 3130 3331 3031 3130 3731 3234 3130  2410310110712410
-00000fb0: 3731 3031 3130 3731 3031 3130 3131 3031  7101107101101101
-00000fc0: 3130 3731 3234 3130 3331 3031 3130 3731  1071241031011071
-00000fd0: 3031 3130 3131 3031 3130 3731 3234 3130  0110110110712410
-00000fe0: 3731 3031 3130 3731 3234 3130 3731 3031  7101107124107101
-00000ff0: 3130 3731 3234 3130 3731 3031 3130 3731  1071241071011071
-00001000: 3031 3130 3131 3031 3130 3731 3234 3132  0110110110712412
-00001010: 3431 3031 3130 3731 3031 3130 3131 3031  4101107101101101
-00001020: 3130 3731 3234 3130 3331 3031 3130 3731  1071241031011071
-00001030: 3031 3130 3131 3031 3130 3731 3234 3130  0110110110712410
-00001040: 3731 3031 3130 3731 3234 3130 3731 3031  7101107124107101
-00001050: 3130 3731 3234 3130 3731 3031 3130 3731  1071241071011071
-00001060: 3031 3130 3131 3031 3130 3731 3234 3130  0110110110712410
-00001070: 3731 3031 3130 3731 3031 3130 3131 3031  7101107101101101
-00001080: 3130 3731 3234 3130 330a 2420 6563 686f  107124103.$ echo
-00001090: 202d 656e 2022 4147 5443 4147 5443 4147   -en "AGTCAGTCAG
-000010a0: 5447 4147 4141 4147 5443 4147 5447 4147  TGAGAAAGTCAGTGAG
-000010b0: 4141 4147 5447 4147 5447 4147 4141 4147  AAAGTGAGTGAGAAAG
-000010c0: 5447 4147 5443 4147 5447 4147 4141 4147  TGAGTCAGTGAGAAAG
-000010d0: 5443 4147 4141 4147 5447 4147 5447 4147  TCAGAAAGTGAGTGAG
-000010e0: 5447 4147 4141 4147 5454 4147 4141 4147  TGAGAAAGTTAGAAAG
-000010f0: 5443 4147 4141 4147 5447 4147 5447 4147  TCAGAAAGTGAGTGAG
-00001100: 5447 4147 4141 4147 5447 4147 4141 4147  TGAGAAAGTGAGAAAG
-00001110: 5443 2220 7c20 636f 6465 7874 202d 6420  TC" | codext -d 
-00001120: 646e 612d 3220 6d6f 7273 6520 7265 7665  dna-2 morse reve
-00001130: 7273 650a 7465 7374 2073 7472 696e 670a  rse.test string.
-00001140: 6060 600a 0a23 2320 5573 6167 6520 2850  ```..## Usage (P
-00001150: 7974 686f 6e29 0a0a 4765 7474 696e 6720  ython)..Getting 
-00001160: 7468 6520 6c69 7374 206f 6620 6176 6169  the list of avai
-00001170: 6c61 626c 6520 636f 6465 6373 3a0a 0a60  lable codecs:..`
-00001180: 6060 7079 7468 6f6e 0a3e 3e3e 2069 6d70  ``python.>>> imp
-00001190: 6f72 7420 636f 6465 7874 0a3e 3e3e 2063  ort codext.>>> c
-000011a0: 6f64 6578 742e 6c69 7374 2829 0a5b 2761  odext.list().['a
-000011b0: 7363 6969 3835 272c 2027 6261 7365 3835  scii85', 'base85
-000011c0: 272c 2027 6261 7365 3130 3027 2c20 2762  ', 'base100', 'b
-000011d0: 6173 6531 3232 272c 202e 2e2e 2c20 2774  ase122', ..., 't
-000011e0: 6f6d 746f 6d27 2c20 2764 6e61 272c 2027  omtom', 'dna', '
-000011f0: 6874 6d6c 272c 2027 6d61 726b 646f 776e  html', 'markdown
-00001200: 272c 2027 7572 6c27 2c20 2772 6573 6973  ', 'url', 'resis
-00001210: 746f 7227 2c20 2773 6d73 272c 2027 7768  tor', 'sms', 'wh
-00001220: 6974 6573 7061 6365 272c 2027 7768 6974  itespace', 'whit
-00001230: 6573 7061 6365 2d61 6674 6572 2d62 6566  espace-after-bef
-00001240: 6f72 6527 5d0a 6060 600a 0a55 7361 6765  ore'].```..Usage
-00001250: 2065 7861 6d70 6c65 733a 0a0a 6060 6070   examples:..```p
-00001260: 7974 686f 6e0a 3e3e 3e20 636f 6465 7874  ython.>>> codext
-00001270: 2e65 6e63 6f64 6528 2274 6869 7320 6973  .encode("this is
-00001280: 2061 2074 6573 7422 2c20 2262 6173 6535   a test", "base5
-00001290: 382d 6269 7463 6f69 6e22 290a 276a 6f39  8-bitcoin").'jo9
-000012a0: 3177 614c 5141 314e 4e65 426d 5a4b 5546  1waLQA1NNeBmZKUF
-000012b0: 270a 3e3e 3e20 636f 6465 7874 2e65 6e63  '.>>> codext.enc
-000012c0: 6f64 6528 2274 6869 7320 6973 2061 2074  ode("this is a t
-000012d0: 6573 7422 2c20 2262 6173 6535 382d 7269  est", "base58-ri
-000012e0: 7070 6c65 2229 0a27 6a6f 3972 4132 4c51  pple").'jo9rA2LQ
-000012f0: 7772 3434 6542 6d5a 4b37 4527 0a3e 3e3e  wr44eBmZK7E'.>>>
-00001300: 2063 6f64 6578 742e 656e 636f 6465 2822   codext.encode("
-00001310: 7468 6973 2069 7320 6120 7465 7374 222c  this is a test",
-00001320: 2022 6261 7365 3538 2d75 726c 2229 0a27   "base58-url").'
-00001330: 4a4e 3931 577a 6b70 6131 6e6e 4462 4c79  JN91Wzkpa1nnDbLy
-00001340: 6a74 6627 0a60 6060 0a0a 6060 6070 7974  jtf'.```..```pyt
-00001350: 686f 6e0a 3e3e 3e20 636f 6465 6373 2e65  hon.>>> codecs.e
-00001360: 6e63 6f64 6528 2274 6869 7320 6973 2061  ncode("this is a
-00001370: 2074 6573 7422 2c20 2262 6173 6531 3030   test", "base100
-00001380: 2229 0a27 f09f 91ab f09f 919f f09f 91a0  ").'............
-00001390: f09f 91aa f09f 9097 f09f 91a0 f09f 91aa  ................
-000013a0: f09f 9097 f09f 9198 f09f 9097 f09f 91ab  ................
-000013b0: f09f 919c f09f 91aa f09f 91ab 270a 3e3e  ............'.>>
-000013c0: 3e20 636f 6465 6373 2e64 6563 6f64 6528  > codecs.decode(
-000013d0: 22f0 9f91 abf0 9f91 9ff0 9f91 a0f0 9f91  "...............
-000013e0: aaf0 9f90 97f0 9f91 a0f0 9f91 aaf0 9f90  ................
-000013f0: 97f0 9f91 98f0 9f90 97f0 9f91 abf0 9f91  ................
-00001400: 9cf0 9f91 aaf0 9f91 ab22 2c20 2262 6173  .........", "bas
-00001410: 6531 3030 2229 0a27 7468 6973 2069 7320  e100").'this is 
-00001420: 6120 7465 7374 270a 6060 600a 0a60 6060  a test'.```..```
-00001430: 7079 7468 6f6e 0a3e 3e3e 2066 6f72 2069  python.>>> for i
-00001440: 2069 6e20 7261 6e67 6528 3829 3a0a 2020   in range(8):.  
-00001450: 2020 2020 2020 7072 696e 7428 636f 6465        print(code
-00001460: 7874 2e65 6e63 6f64 6528 2274 6869 7320  xt.encode("this 
-00001470: 6973 2061 2074 6573 7422 2c20 2264 6e61  is a test", "dna
-00001480: 2d25 6422 2025 2028 6920 2b20 3129 2929  -%d" % (i + 1)))
-00001490: 0a47 5447 4147 4343 4147 4343 4747 5441  .GTGAGCCAGCCGGTA
-000014a0: 5441 4341 4147 4343 4747 5441 5441 4341  TACAAGCCGGTATACA
-000014b0: 4147 4341 4741 4341 4147 5447 4147 4347  AGCAGACAAGTGAGCG
-000014c0: 4747 5441 5447 5447 410a 4354 4341 4347  GGTATGTGA.CTCACG
-000014d0: 4741 4347 4743 4354 4154 4147 4141 4347  GACGGCCTATAGAACG
-000014e0: 4743 4354 4154 4147 4141 4347 4143 4147  GCCTATAGAACGACAG
-000014f0: 4141 4354 4341 4347 4343 4354 4154 4354  AACTCACGCCCTATCT
-00001500: 4341 0a41 4341 4741 5454 4741 5454 4141  CA.ACAGATTGATTAA
-00001510: 4347 4347 5447 4741 5454 4141 4347 4347  CGCGTGGATTAACGCG
-00001520: 5447 4741 5447 4147 5447 4741 4341 4741  TGGATGAGTGGACAGA
-00001530: 5441 4141 4347 4341 4341 470a 4147 4143  TAAACGCACAG.AGAC
-00001540: 4154 5443 4154 5441 4147 4347 4354 4343  ATTCATTAAGCGCTCC
-00001550: 4154 5441 4147 4347 4354 4343 4154 4341  ATTAAGCGCTCCATCA
-00001560: 4354 4343 4147 4143 4154 4141 4147 4347  CTCCAGACATAAAGCG
-00001570: 4147 4143 0a54 4354 4754 4141 4754 4141  AGAC.TCTGTAAGTAA
-00001580: 5454 4347 4347 4147 4754 4141 5454 4347  TTCGCGAGGTAATTCG
-00001590: 4347 4147 4754 4147 5447 4147 4754 4354  CGAGGTAGTGAGGTCT
-000015a0: 4754 4154 5454 4347 4354 4354 470a 5447  GTATTTCGCTCTG.TG
-000015b0: 5443 5441 4143 5441 4154 5447 4347 4341  TCTAACTAATTGCGCA
-000015c0: 4343 5441 4154 5447 4347 4341 4343 5441  CCTAATTGCGCACCTA
-000015d0: 4354 4341 4343 5447 5443 5441 5454 5447  CTCACCTGTCTATTTG
-000015e0: 4347 5447 5443 0a47 4147 5447 4343 5447  CGTGTC.GAGTGCCTG
-000015f0: 4343 4747 4154 4154 4354 5447 4343 4747  CCGGATATCTTGCCGG
-00001600: 4154 4154 4354 5447 4354 4754 4354 5447  ATATCTTGCTGTCTTG
-00001610: 4147 5447 4347 4747 4154 4147 4147 540a  AGTGCGGGATAGAGT.
-00001620: 4341 4354 4347 4754 4347 4743 4341 5441  CACTCGGTCGGCCATA
-00001630: 5447 5454 4347 4743 4341 5441 5447 5454  TGTTCGGCCATATGTT
-00001640: 4347 5443 5447 5454 4341 4354 4347 4343  CGTCTGTTCACTCGCC
-00001650: 4341 5441 4341 4354 0a3e 3e3e 2063 6f64  CATACACT.>>> cod
-00001660: 6578 742e 6465 636f 6465 2822 4754 4741  ext.decode("GTGA
-00001670: 4743 4341 4743 4347 4754 4154 4143 4141  GCCAGCCGGTATACAA
-00001680: 4743 4347 4754 4154 4143 4141 4743 4147  GCCGGTATACAAGCAG
-00001690: 4143 4141 4754 4741 4743 4747 4754 4154  ACAAGTGAGCGGGTAT
-000016a0: 4754 4741 222c 2022 646e 612d 3122 290a  GTGA", "dna-1").
-000016b0: 2774 6869 7320 6973 2061 2074 6573 7427  'this is a test'
-000016c0: 0a60 6060 0a0a 6060 6070 7974 686f 6e0a  .```..```python.
-000016d0: 3e3e 3e20 636f 6465 6373 2e65 6e63 6f64  >>> codecs.encod
-000016e0: 6528 2274 6869 7320 6973 2061 2074 6573  e("this is a tes
-000016f0: 7422 2c20 226d 6f72 7365 2229 0a27 2d20  t", "morse").'- 
-00001700: 2e2e 2e2e 202e 2e20 2e2e 2e20 2f20 2e2e  .... .. ... / ..
-00001710: 202e 2e2e 202f 202e 2d20 2f20 2d20 2e20   ... / .- / - . 
-00001720: 2e2e 2e20 2d27 0a3e 3e3e 2063 6f64 6563  ... -'.>>> codec
-00001730: 732e 6465 636f 6465 2822 2d20 2e2e 2e2e  s.decode("- ....
-00001740: 202e 2e20 2e2e 2e20 2f20 2e2e 202e 2e2e   .. ... / .. ...
-00001750: 202f 202e 2d20 2f20 2d20 2e20 2e2e 2e20   / .- / - . ... 
-00001760: 2d22 2c20 226d 6f72 7365 2229 0a27 7468  -", "morse").'th
-00001770: 6973 2069 7320 6120 7465 7374 270a 3e3e  is is a test'.>>
-00001780: 3e20 7769 7468 206f 7065 6e28 226d 6f72  > with open("mor
-00001790: 7365 2e74 7874 222c 2027 7727 2c20 656e  se.txt", 'w', en
-000017a0: 636f 6469 6e67 3d22 6d6f 7273 6522 2920  coding="morse") 
-000017b0: 6173 2066 3a0a 0966 2e77 7269 7465 2822  as f:..f.write("
-000017c0: 7468 6973 2069 7320 6120 7465 7374 2229  this is a test")
-000017d0: 0a31 340a 3e3e 3e20 7769 7468 206f 7065  .14.>>> with ope
-000017e0: 6e28 226d 6f72 7365 2e74 7874 222c 656e  n("morse.txt",en
-000017f0: 636f 6469 6e67 3d22 6d6f 7273 6522 2920  coding="morse") 
-00001800: 6173 2066 3a0a 0966 2e72 6561 6428 290a  as f:..f.read().
-00001810: 2774 6869 7320 6973 2061 2074 6573 7427  'this is a test'
-00001820: 0a60 6060 0a0a 6060 6070 7974 686f 6e0a  .```..```python.
-00001830: 3e3e 3e20 636f 6465 7874 2e64 6563 6f64  >>> codext.decod
-00001840: 6528 2222 220a 2020 2020 2020 3d20 2020  e(""".      =   
-00001850: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-00001860: 2020 2020 2020 2020 5820 2020 2020 2020          X       
-00001870: 2020 0a20 2020 3a20 2020 2020 2020 2020    .   :         
-00001880: 2020 200a 2020 2020 2020 7820 2020 2020     .      x     
-00001890: 2020 2020 0a20 206e 2020 0a20 2020 2072      .  n  .    r
-000018a0: 200a 2020 2020 2020 2020 7920 2020 0a20   .        y   . 
-000018b0: 2020 2020 2059 2020 2020 2020 2020 2020       Y          
-000018c0: 2020 0a20 2020 2020 2020 2020 2020 2020    .             
-000018d0: 2079 2020 2020 2020 2020 0a20 2020 2020   y        .     
-000018e0: 7020 2020 200a 2020 2020 2020 2020 2061  p    .         a
-000018f0: 2020 2020 2020 200a 2060 2020 2020 2020         . `      
-00001900: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
-00001910: 206e 2020 2020 2020 2020 2020 2020 0a20   n            . 
-00001920: 2020 2020 2020 2020 207c 2020 2020 0a20           |    . 
-00001930: 2061 2020 2020 2020 2020 2020 0a6f 2020   a          .o  
-00001940: 2020 0a20 2020 2020 2020 6820 2020 2020    .       h     
-00001950: 2020 200a 2020 2020 2020 2020 2020 6020     .          ` 
-00001960: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-00001970: 2020 2020 2020 6720 2020 2020 2020 2020        g         
-00001980: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-00001990: 2020 6f20 0a20 2020 7a20 2020 2020 2022    o .   z      "
-000019a0: 2222 2c20 2277 6869 7465 7370 6163 652d  "", "whitespace-
-000019b0: 6166 7465 722b 6265 666f 7265 2229 0a27  after+before").'
-000019c0: 4353 437b 6e6f 745f 736f 5f69 6e76 6973  CSC{not_so_invis
-000019d0: 6962 6c65 7d27 0a60 6060 0a0a 6060 6070  ible}'.```..```p
-000019e0: 7974 686f 6e0a 3e3e 3e20 7072 696e 7428  ython.>>> print(
-000019f0: 636f 6465 7874 2e65 6e63 6f64 6528 2241  codext.encode("A
-00001a00: 6e20 6578 616d 706c 6520 7465 7374 2073  n example test s
-00001a10: 7472 696e 6722 2c20 2262 6175 646f 742d  tring", "baudot-
-00001a20: 7461 7065 2229 290a 2a2a 2a2e 2a2a 0a20  tape")).***.**. 
-00001a30: 2020 2e20 2a0a 2a2a 2a2e 2a20 0a2a 2020    . *.***.* .*  
-00001a40: 2e20 200a 2020 202e 2a20 0a2a 2020 2e2a  .  .   .* .*  .*
-00001a50: 200a 2020 202e 202a 0a2a 2a20 2e2a 200a   .   . *.** .* .
-00001a60: 2a2a 2a2e 2a2a 0a2a 2a20 2e2a 2a0a 2020  ***.**.** .**.  
-00001a70: 202e 2a20 0a2a 2020 2e20 200a 2a20 2a2e   .* .*  .  .* *.
-00001a80: 202a 0a20 2020 2e2a 200a 2a20 2a2e 2020   *.   .* .* *.  
-00001a90: 0a2a 202a 2e20 2a0a 2a20 202e 2020 0a2a  .* *. *.*  .  .*
-00001aa0: 202a 2e20 200a 2a20 2a2e 202a 0a2a 2a2a   *.  .* *. *.***
-00001ab0: 2e20 200a 2020 2a2e 2a20 0a2a 2a2a 2e2a  .  .  *.* .***.*
-00001ac0: 200a 202a 202e 2a20 0a60 6060 0a0a 2323   . * .* .```..##
-00001ad0: 204c 6973 7420 6f66 2063 6f64 6563 730a   List of codecs.
-00001ae0: 0a2a 2a43 6f64 6563 2a2a 207c 202a 2a43  .**Codec** | **C
-00001af0: 6f6e 7665 7273 696f 6e73 2a2a 207c 202a  onversions** | *
-00001b00: 2a43 6f6d 6d65 6e74 2a2a 0a3a 2d2d 2d3a  *Comment**.:---:
-00001b10: 207c 203a 2d2d 2d3a 207c 202d 2d2d 0a60   | :---: | ---.`
-00001b20: 6131 7a32 3660 207c 2074 6578 7420 3c2d  a1z26` | text <-
-00001b30: 3e20 616c 7068 6162 6574 206f 7264 6572  > alphabet order
-00001b40: 206e 756d 6265 7273 207c 206b 6565 7073   numbers | keeps
-00001b50: 2077 6f72 6473 2077 6869 7465 7370 6163   words whitespac
-00001b60: 652d 7365 7061 7261 7465 6420 616e 6420  e-separated and 
-00001b70: 7573 6573 2061 2063 7573 746f 6d20 6368  uses a custom ch
-00001b80: 6172 6163 7465 7220 7365 7061 7261 746f  aracter separato
-00001b90: 720a 6061 6666 696e 6560 207c 2074 6578  r.`affine` | tex
-00001ba0: 7420 3c2d 3e20 6166 6669 6e65 2063 6970  t <-> affine cip
-00001bb0: 6865 7274 6578 7420 7c20 616b 6120 4166  hertext | aka Af
-00001bc0: 6669 6e65 2043 6970 6865 720a 6061 7363  fine Cipher.`asc
-00001bd0: 6969 3835 6020 7c20 7465 7874 203c 2d3e  ii85` | text <->
-00001be0: 2061 7363 6969 3835 2065 6e63 6f64 6564   ascii85 encoded
-00001bf0: 2074 6578 7420 7c20 5079 7468 6f6e 2033   text | Python 3
-00001c00: 206f 6e6c 790a 6061 7462 6173 6860 207c   only.`atbash` |
-00001c10: 2074 6578 7420 3c2d 3e20 4174 6261 7368   text <-> Atbash
-00001c20: 2063 6970 6865 7274 6578 7420 7c20 616b   ciphertext | ak
-00001c30: 6120 4174 6261 7368 2043 6970 6865 720a  a Atbash Cipher.
-00001c40: 6062 6163 6f6e 6020 7c20 7465 7874 203c  `bacon` | text <
-00001c50: 2d3e 2042 6163 6f6e 2063 6970 6865 7274  -> Bacon ciphert
-00001c60: 6578 7420 7c20 616b 6120 4261 636f 6e69  ext | aka Baconi
-00001c70: 616e 2043 6970 6865 720a 6062 6172 6269  an Cipher.`barbi
-00001c80: 652d 4e60 207c 2074 6578 7420 3c2d 3e20  e-N` | text <-> 
-00001c90: 6261 7262 6965 2063 6970 6865 7274 6578  barbie ciphertex
-00001ca0: 7420 7c20 616b 6120 4261 7262 6965 2054  t | aka Barbie T
-00001cb0: 7970 6577 7269 7465 7220 284e 2062 656c  ypewriter (N bel
-00001cc0: 6f6e 6773 2074 6f20 5b31 2c20 345d 290a  ongs to [1, 4]).
-00001cd0: 6062 6173 6558 5860 207c 2074 6578 7420  `baseXX` | text 
-00001ce0: 3c2d 3e20 6261 7365 5858 207c 2073 6565  <-> baseXX | see
-00001cf0: 205b 6261 7365 2065 6e63 6f64 696e 6773   [base encodings
-00001d00: 5d28 6874 7470 733a 2f2f 7079 7468 6f6e  ](https://python
-00001d10: 2d63 6f64 6578 742e 7265 6164 7468 6564  -codext.readthed
-00001d20: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-00001d30: 2f65 6e63 2f62 6173 652e 6874 6d6c 2920  /enc/base.html) 
-00001d40: 2869 6e63 6c20 6261 7365 3332 2c20 3336  (incl base32, 36
-00001d50: 2c20 3435 2c20 3538 2c20 3632 2c20 3633  , 45, 58, 62, 63
-00001d60: 2c20 3634 2c20 3931 2c20 3130 302c 2031  , 64, 91, 100, 1
-00001d70: 3232 290a 6062 6175 646f 7460 207c 2074  22).`baudot` | t
-00001d80: 6578 7420 3c2d 3e20 4261 7564 6f74 2063  ext <-> Baudot c
-00001d90: 6f64 6520 6269 7473 207c 2073 7570 706f  ode bits | suppo
-00001da0: 7274 7320 4343 4954 542d 312c 2043 4349  rts CCITT-1, CCI
-00001db0: 5454 2d32 2c20 4555 2f46 522c 2049 5441  TT-2, EU/FR, ITA
-00001dc0: 312c 2049 5441 322c 204d 544b 2d32 2028  1, ITA2, MTK-2 (
-00001dd0: 5079 7468 6f6e 3320 6f6e 6c79 292c 2055  Python3 only), U
-00001de0: 4b2c 202e 2e2e 0a60 6263 6460 207c 2074  K, ....`bcd` | t
-00001df0: 6578 7420 3c2d 3e20 6269 6e61 7279 2063  ext <-> binary c
-00001e00: 6f64 6564 2064 6563 696d 616c 2074 6578  oded decimal tex
-00001e10: 7420 7c20 656e 636f 6465 7320 6368 6172  t | encodes char
-00001e20: 6163 7465 7273 2066 726f 6d20 7468 6569  acters from thei
-00001e30: 7220 287a 6572 6f2d 6c65 6674 2d70 6164  r (zero-left-pad
-00001e40: 6465 6429 206f 7264 696e 616c 730a 6062  ded) ordinals.`b
-00001e50: 7261 696c 6c65 6020 7c20 7465 7874 203c  raille` | text <
-00001e60: 2d3e 2062 7261 696c 6c65 2073 796d 626f  -> braille symbo
-00001e70: 6c73 207c 2050 7974 686f 6e20 3320 6f6e  ls | Python 3 on
-00001e80: 6c79 0a60 6369 7472 6978 6020 7c20 7465  ly.`citrix` | te
-00001e90: 7874 203c 2d3e 2043 6974 7269 7820 4354  xt <-> Citrix CT
-00001ea0: 5831 2063 6970 6865 7274 6578 7420 7c20  X1 ciphertext | 
-00001eb0: 616b 6120 4369 7472 6978 2043 5458 3120  aka Citrix CTX1 
-00001ec0: 7061 7373 6f72 6420 656e 636f 6469 6e67  passord encoding
-00001ed0: 0a60 646e 6160 207c 2074 6578 7420 3c2d  .`dna` | text <-
-00001ee0: 3e20 444e 412d 4e20 7365 7175 656e 6365  > DNA-N sequence
-00001ef0: 207c 2069 6d70 6c65 6d65 6e74 7320 7468   | implements th
-00001f00: 6520 3820 7275 6c65 7320 6f66 2044 4e41  e 8 rules of DNA
-00001f10: 2073 6571 7565 6e63 6573 2028 4e20 6265   sequences (N be
-00001f20: 6c6f 6e67 7320 746f 205b 312c 385d 290a  longs to [1,8]).
-00001f30: 6065 7863 6573 7333 6020 7c20 7465 7874  `excess3` | text
-00001f40: 203c 2d3e 2058 5333 2065 6e63 6f64 6564   <-> XS3 encoded
-00001f50: 2074 6578 7420 7c20 7573 6573 2045 7863   text | uses Exc
-00001f60: 6573 732d 3320 2861 6b61 2053 7469 6269  ess-3 (aka Stibi
-00001f70: 747a 2063 6f64 6529 2062 696e 6172 7920  tz code) binary 
-00001f80: 656e 636f 6469 6e67 2074 6f20 636f 6e76  encoding to conv
-00001f90: 6572 7420 6368 6172 6163 7465 7273 2066  ert characters f
-00001fa0: 726f 6d20 7468 6569 7220 6f72 6469 6e61  rom their ordina
-00001fb0: 6c73 0a60 6772 6179 6020 7c20 7465 7874  ls.`gray` | text
-00001fc0: 203c 2d3e 2067 7261 7920 656e 636f 6465   <-> gray encode
-00001fd0: 6420 7465 7874 207c 2061 6b61 2072 6566  d text | aka ref
-00001fe0: 6c65 6374 6564 2062 696e 6172 7920 636f  lected binary co
-00001ff0: 6465 0a60 677a 6970 6020 7c20 7465 7874  de.`gzip` | text
-00002000: 203c 2d3e 2047 7a69 702d 636f 6d70 7265   <-> Gzip-compre
-00002010: 7373 6564 2074 6578 7420 7c20 7374 616e  ssed text | stan
-00002020: 6461 7264 2047 7a69 7020 636f 6d70 7265  dard Gzip compre
-00002030: 7373 696f 6e2f 6465 636f 6d70 7265 7373  ssion/decompress
-00002040: 696f 6e0a 6068 746d 6c60 207c 2074 6578  ion.`html` | tex
-00002050: 7420 3c2d 3e20 4854 4d4c 2065 6e74 6974  t <-> HTML entit
-00002060: 6965 7320 7c20 696d 706c 656d 656e 7473  ies | implements
-00002070: 2065 6e74 6974 6965 7320 6163 636f 7264   entities accord
-00002080: 696e 6720 746f 205b 7468 6973 2072 6566  ing to [this ref
-00002090: 6572 656e 6365 5d28 6874 7470 733a 2f2f  erence](https://
-000020a0: 6465 762e 7733 2e6f 7267 2f68 746d 6c35  dev.w3.org/html5
-000020b0: 2f68 746d 6c2d 6175 7468 6f72 2f63 6861  /html-author/cha
-000020c0: 7272 6566 290a 6069 7073 756d 6020 7c20  rref).`ipsum` | 
-000020d0: 7465 7874 203c 2d3e 206c 6174 696e 2077  text <-> latin w
-000020e0: 6f72 6473 207c 2061 6b61 206c 6f72 656d  ords | aka lorem
-000020f0: 2069 7073 756d 0a60 6b6c 6f70 6660 207c   ipsum.`klopf` |
-00002100: 2074 6578 7420 3c2d 3e20 6b6c 6f70 6620   text <-> klopf 
-00002110: 656e 636f 6465 6420 7465 7874 207c 2050  encoded text | P
-00002120: 6f6c 7962 6975 7320 7371 7561 7265 2077  olybius square w
-00002130: 6974 6820 7472 6976 6961 6c20 616c 7068  ith trivial alph
-00002140: 6162 6574 6963 616c 2064 6973 7472 6962  abetical distrib
-00002150: 7574 696f 6e0a 606c 6565 7473 7065 616b  ution.`leetspeak
-00002160: 6020 7c20 7465 7874 203c 2d3e 206c 6565  ` | text <-> lee
-00002170: 7473 7065 616b 2065 6e63 6f64 6564 2074  tspeak encoded t
-00002180: 6578 7420 7c20 6261 7365 6420 6f6e 206d  ext | based on m
-00002190: 696e 696d 616c 6973 7469 6320 656c 6974  inimalistic elit
-000021a0: 6520 7370 6561 6b69 6e67 2072 756c 6573  e speaking rules
-000021b0: 0a60 6c65 7474 6572 2d69 6e64 6963 6573  .`letter-indices
-000021c0: 6020 7c20 7465 7874 203c 2d3e 2074 6578  ` | text <-> tex
-000021d0: 7420 7769 7468 206c 6574 7465 7220 696e  t with letter in
-000021e0: 6469 6365 7320 7c20 656e 636f 6465 7320  dices | encodes 
-000021f0: 636f 6e73 6f6e 616e 7473 2061 6e64 2f6f  consonants and/o
-00002200: 7220 766f 7765 6c73 2077 6974 6820 7468  r vowels with th
-00002210: 6569 7220 636f 7272 6573 706f 6e64 696e  eir correspondin
-00002220: 6720 696e 6469 6365 730a 606c 7a37 3760  g indices.`lz77`
-00002230: 207c 2074 6578 7420 3c2d 3e20 4c5a 3737   | text <-> LZ77
-00002240: 2d63 6f6d 7072 6573 7365 6420 7465 7874  -compressed text
-00002250: 207c 2063 6f6d 7072 6573 7365 7320 7468   | compresses th
-00002260: 6520 6769 7665 6e20 6461 7461 2077 6974  e given data wit
-00002270: 6820 7468 6520 616c 676f 7269 7468 6d20  h the algorithm 
-00002280: 6f66 204c 656d 7065 6c20 616e 6420 5a69  of Lempel and Zi
-00002290: 7620 6f66 2031 3937 370a 606c 7a37 3860  v of 1977.`lz78`
-000022a0: 207c 2074 6578 7420 3c2d 3e20 4c5a 3738   | text <-> LZ78
-000022b0: 2d63 6f6d 7072 6573 7365 6420 7465 7874  -compressed text
-000022c0: 207c 2063 6f6d 7072 6573 7365 7320 7468   | compresses th
-000022d0: 6520 6769 7665 6e20 6461 7461 2077 6974  e given data wit
-000022e0: 6820 7468 6520 616c 676f 7269 7468 6d20  h the algorithm 
-000022f0: 6f66 204c 656d 7065 6c20 616e 6420 5a69  of Lempel and Zi
-00002300: 7620 6f66 2031 3937 380a 606d 616e 6368  v of 1978.`manch
-00002310: 6573 7465 7260 207c 2074 6578 7420 3c2d  ester` | text <-
-00002320: 3e20 6d61 6e63 6865 7374 6572 2065 6e63  > manchester enc
-00002330: 6f64 6564 2074 6578 7420 7c20 584f 5265  oded text | XORe
-00002340: 7320 6561 6368 2062 6974 206f 6620 7468  s each bit of th
-00002350: 6520 696e 7075 7420 7769 7468 2060 3031  e input with `01
-00002360: 600a 606d 6172 6b64 6f77 6e60 207c 206d  `.`markdown` | m
-00002370: 6172 6b64 6f77 6e20 2d2d 3e20 4854 4d4c  arkdown --> HTML
-00002380: 207c 2075 6e69 6469 7265 6374 696f 6e61   | unidirectiona
-00002390: 6c0a 606d 6f72 7365 6020 7c20 7465 7874  l.`morse` | text
-000023a0: 203c 2d3e 206d 6f72 7365 2065 6e63 6f64   <-> morse encod
-000023b0: 6564 2074 6578 7420 7c20 7573 6573 2077  ed text | uses w
-000023c0: 6869 7465 7370 6163 6520 6173 2061 2073  hitespace as a s
-000023d0: 6570 6172 6174 6f72 0a60 6e61 7661 6a6f  eparator.`navajo
-000023e0: 6020 7c20 7465 7874 203c 2d3e 204e 6176  ` | text <-> Nav
-000023f0: 616a 6f20 7c20 6f6e 6c79 2068 616e 646c  ajo | only handl
-00002400: 6573 206c 6574 7465 7273 2028 6e6f 7420  es letters (not 
-00002410: 6675 6c6c 2077 6f72 6473 2066 726f 6d20  full words from 
-00002420: 7468 6520 4e61 7661 6a6f 2064 6963 7469  the Navajo dicti
-00002430: 6f6e 6172 7929 0a60 6f63 7461 6c60 207c  onary).`octal` |
-00002440: 2074 6578 7420 3c2d 3e20 6f63 7461 6c20   text <-> octal 
-00002450: 6469 6769 7473 207c 2064 756d 6d79 206f  digits | dummy o
-00002460: 6374 616c 2063 6f6e 7665 7273 696f 6e20  ctal conversion 
-00002470: 2863 6f6e 7665 7274 7320 746f 2033 2d64  (converts to 3-d
-00002480: 6967 6974 7320 6772 6f75 7073 290a 606f  igits groups).`o
-00002490: 7264 696e 616c 6020 7c20 7465 7874 203c  rdinal` | text <
-000024a0: 2d3e 206f 7264 696e 616c 2064 6967 6974  -> ordinal digit
-000024b0: 7320 7c20 6475 6d6d 7920 6368 6172 6163  s | dummy charac
-000024c0: 7465 7220 6f72 6469 6e61 6c73 2063 6f6e  ter ordinals con
-000024d0: 7665 7273 696f 6e20 2863 6f6e 7665 7274  version (convert
-000024e0: 7320 746f 2033 2d64 6967 6974 7320 6772  s to 3-digits gr
-000024f0: 6f75 7073 290a 6070 6b7a 6970 5f64 6566  oups).`pkzip_def
-00002500: 6c61 7465 6020 7c20 7465 7874 203c 2d3e  late` | text <->
-00002510: 2064 6566 6c61 7465 6420 7465 7874 207c   deflated text |
-00002520: 2073 7461 6e64 6172 6420 5a69 702d 6465   standard Zip-de
-00002530: 666c 6174 6520 636f 6d70 7265 7373 696f  flate compressio
-00002540: 6e2f 6465 636f 6d70 7265 7373 696f 6e0a  n/decompression.
-00002550: 6070 6b7a 6970 5f62 7a69 7032 6020 7c20  `pkzip_bzip2` | 
-00002560: 7465 7874 203c 2d3e 2042 7a69 7070 6564  text <-> Bzipped
-00002570: 2074 6578 7420 7c20 7374 616e 6461 7264   text | standard
-00002580: 2042 5a69 7032 2063 6f6d 7072 6573 7369   BZip2 compressi
-00002590: 6f6e 2f64 6563 6f6d 7072 6573 7369 6f6e  on/decompression
-000025a0: 0a60 706b 7a69 705f 6c7a 6d61 6020 7c20  .`pkzip_lzma` | 
-000025b0: 7465 7874 203c 2d3e 204c 5a4d 412d 636f  text <-> LZMA-co
-000025c0: 6d70 7265 7373 6564 2074 6578 7420 7c20  mpressed text | 
-000025d0: 7374 616e 6461 7264 204c 5a4d 4120 636f  standard LZMA co
-000025e0: 6d70 7265 7373 696f 6e2f 6465 636f 6d70  mpression/decomp
-000025f0: 7265 7373 696f 6e0a 6072 6164 696f 6020  ression.`radio` 
-00002600: 7c20 7465 7874 203c 2d3e 2072 6164 696f  | text <-> radio
-00002610: 2077 6f72 6473 207c 2061 6b61 204e 4154   words | aka NAT
-00002620: 4f20 6f72 2072 6164 696f 2070 686f 6e65  O or radio phone
-00002630: 7469 6320 616c 7068 6162 6574 0a60 7265  tic alphabet.`re
-00002640: 7369 7374 6f72 6020 7c20 7465 7874 203c  sistor` | text <
-00002650: 2d3e 2072 6573 6973 746f 7220 636f 6c6f  -> resistor colo
-00002660: 7273 207c 2061 6b61 2072 6573 6973 746f  rs | aka resisto
-00002670: 7220 636f 6c6f 7220 636f 6465 730a 6072  r color codes.`r
-00002680: 6f74 6020 7c20 7465 7874 203c 2d3e 2072  ot` | text <-> r
-00002690: 6f74 284e 2920 6369 7068 6572 7465 7874  ot(N) ciphertext
-000026a0: 207c 2061 6b61 2043 6165 7361 7220 6369   | aka Caesar ci
-000026b0: 7068 6572 2028 4e20 6265 6c6f 6e67 7320  pher (N belongs 
-000026c0: 746f 205b 312c 3235 5d29 0a60 726f 7461  to [1,25]).`rota
-000026d0: 7465 6020 7c20 7465 7874 203c 2d3e 204e  te` | text <-> N
-000026e0: 2d62 6974 732d 726f 7461 7465 6420 7465  -bits-rotated te
-000026f0: 7874 207c 2072 6f74 6174 6573 2063 6861  xt | rotates cha
-00002700: 7261 6374 6572 7320 6279 2074 6865 2073  racters by the s
-00002710: 7065 6369 6669 6564 206e 756d 6265 7220  pecified number 
-00002720: 6f66 2062 6974 7320 3b20 5079 7468 6f6e  of bits ; Python
-00002730: 2033 206f 6e6c 790a 6073 6379 7461 6c65   3 only.`scytale
-00002740: 6020 7c20 7465 7874 203c 2d3e 2073 6379  ` | text <-> scy
-00002750: 7461 6c65 2063 6970 6865 7274 6578 7420  tale ciphertext 
-00002760: 7c20 656e 6372 7970 7473 2077 6974 6820  | encrypts with 
-00002770: 4c2c 2074 6865 206e 756d 6265 7220 6f66  L, the number of
-00002780: 206c 6574 7465 7273 206f 6e20 7468 6520   letters on the 
-00002790: 726f 6420 2862 656c 6f6e 6773 2074 6f20  rod (belongs to 
-000027a0: 5b31 2c5b 290a 6073 6869 6674 6020 7c20  [1,[).`shift` | 
-000027b0: 7465 7874 203c 2d3e 2073 6869 6674 284e  text <-> shift(N
-000027c0: 2920 6369 7068 6572 7465 7874 207c 2073  ) ciphertext | s
-000027d0: 6869 6674 206f 7264 696e 616c 7320 7769  hift ordinals wi
-000027e0: 7468 204e 2028 6265 6c6f 6e67 7320 746f  th N (belongs to
-000027f0: 205b 312c 3235 355d 290a 6073 6d73 6020   [1,255]).`sms` 
-00002800: 7c20 7465 7874 203c 2d3e 2070 686f 6e65  | text <-> phone
-00002810: 206b 6579 7374 726f 6b65 7320 7c20 616c   keystrokes | al
-00002820: 736f 2063 616c 6c65 6420 5439 2063 6f64  so called T9 cod
-00002830: 6520 3b20 7573 6573 2022 602d 6022 2061  e ; uses "`-`" a
-00002840: 7320 6120 7365 7061 7261 746f 7220 666f  s a separator fo
-00002850: 7220 656e 636f 6469 6e67 2c20 2260 2d60  r encoding, "`-`
-00002860: 2220 6f72 2022 605f 6022 206f 7220 7768  " or "`_`" or wh
-00002870: 6974 6573 7061 6365 2066 6f72 2064 6563  itespace for dec
-00002880: 6f64 696e 670a 6073 6f75 7468 7061 726b  oding.`southpark
-00002890: 6020 7c20 7465 7874 203c 2d3e 204b 656e  ` | text <-> Ken
-000028a0: 6e79 2773 206c 616e 6775 6167 6520 7c20  ny's language | 
-000028b0: 636f 6e76 6572 7473 206c 6574 7465 7273  converts letters
-000028c0: 2074 6f20 4b65 6e6e 7927 7320 6c61 6e67   to Kenny's lang
-000028d0: 7561 6765 2066 726f 6d20 536f 7574 6870  uage from Southp
-000028e0: 6172 6b20 2877 6869 7465 7370 6163 6520  ark (whitespace 
-000028f0: 6973 2061 6c73 6f20 6861 6e64 6c65 6429  is also handled)
-00002900: 0a60 746f 6d74 6f6d 6020 7c20 7465 7874  .`tomtom` | text
-00002910: 203c 2d3e 2074 6f6d 2d74 6f6d 2065 6e63   <-> tom-tom enc
-00002920: 6f64 6564 2074 6578 7420 7c20 7369 6d69  oded text | simi
-00002930: 6c61 7220 746f 2060 6d6f 7273 6560 2c20  lar to `morse`, 
-00002940: 7573 696e 6720 736c 6173 6865 7320 616e  using slashes an
-00002950: 6420 6261 636b 736c 6173 6865 730a 6075  d backslashes.`u
-00002960: 726c 6020 7c20 7465 7874 203c 2d3e 2055  rl` | text <-> U
-00002970: 524c 2065 6e63 6f64 6564 2074 6578 7420  RL encoded text 
-00002980: 7c20 616b 6120 5552 4c20 656e 636f 6469  | aka URL encodi
-00002990: 6e67 0a60 786f 7260 207c 2074 6578 7420  ng.`xor` | text 
-000029a0: 3c2d 3e20 584f 5228 4e29 2063 6970 6865  <-> XOR(N) ciphe
-000029b0: 7274 6578 7420 7c20 584f 5220 7769 7468  rtext | XOR with
-000029c0: 2061 2073 696e 676c 6520 6279 7465 2028   a single byte (
-000029d0: 4e20 6265 6c6f 6e67 7320 746f 205b 312c  N belongs to [1,
-000029e0: 3235 355d 290a 6077 6869 7465 7370 6163  255]).`whitespac
-000029f0: 6560 207c 2074 6578 7420 3c2d 3e20 7768  e` | text <-> wh
-00002a00: 6974 6573 7061 6365 7320 616e 6420 7461  itespaces and ta
-00002a10: 6273 207c 2072 6570 6c61 6365 7320 6269  bs | replaces bi
-00002a20: 7473 2077 6974 6820 7768 6974 6573 7061  ts with whitespa
-00002a30: 6365 7320 616e 6420 7461 6273 0a0a 4120  ces and tabs..A 
-00002a40: 6665 7720 7661 7269 616e 7473 2061 7265  few variants are
-00002a50: 2061 6c73 6f20 696d 706c 656d 656e 7465   also implemente
-00002a60: 642e 0a0a 2a2a 436f 6465 632a 2a20 7c20  d...**Codec** | 
-00002a70: 2a2a 436f 6e76 6572 7369 6f6e 732a 2a20  **Conversions** 
-00002a80: 7c20 2a2a 436f 6d6d 656e 742a 2a0a 3a2d  | **Comment**.:-
-00002a90: 2d2d 3a20 7c20 3a2d 2d2d 3a20 7c20 2d2d  --: | :---: | --
-00002aa0: 2d0a 6062 6175 646f 742d 7370 6163 6564  -.`baudot-spaced
-00002ab0: 6020 7c20 7465 7874 203c 2d3e 2042 6175  ` | text <-> Bau
-00002ac0: 646f 7420 636f 6465 2067 726f 7570 7320  dot code groups 
-00002ad0: 6f66 2062 6974 7320 7c20 6772 6f75 7073  of bits | groups
-00002ae0: 206f 6620 3520 6269 7473 2061 7265 2077   of 5 bits are w
-00002af0: 6869 7465 7370 6163 652d 7365 7061 7261  hitespace-separa
-00002b00: 7465 640a 6062 6175 646f 742d 7461 7065  ted.`baudot-tape
-00002b10: 6020 7c20 7465 7874 203c 2d3e 2042 6175  ` | text <-> Bau
-00002b20: 646f 7420 636f 6465 2074 6170 6520 7c20  dot code tape | 
-00002b30: 6f75 7470 7574 7320 6120 7374 7269 6e67  outputs a string
-00002b40: 2074 6861 7420 6c6f 6f6b 7320 6c69 6b65   that looks like
-00002b50: 2061 2070 6572 666f 7261 7465 6420 7461   a perforated ta
-00002b60: 7065 0a60 6263 642d 6578 7465 6e64 6564  pe.`bcd-extended
-00002b70: 3060 207c 2074 6578 7420 3c2d 3e20 4243  0` | text <-> BC
-00002b80: 442d 6578 7465 6e64 6564 2074 6578 7420  D-extended text 
-00002b90: 7c20 656e 636f 6465 7320 6368 6172 6163  | encodes charac
-00002ba0: 7465 7273 2066 726f 6d20 7468 6569 7220  ters from their 
-00002bb0: 287a 6572 6f2d 6c65 6674 2d70 6164 6465  (zero-left-padde
-00002bc0: 6429 206f 7264 696e 616c 7320 7573 696e  d) ordinals usin
-00002bd0: 6720 7072 6566 6978 2062 6974 7320 6030  g prefix bits `0
-00002be0: 3030 3060 0a60 6263 642d 6578 7465 6e64  000`.`bcd-extend
-00002bf0: 6564 3160 207c 2074 6578 7420 3c2d 3e20  ed1` | text <-> 
-00002c00: 4243 442d 6578 7465 6e64 6564 2074 6578  BCD-extended tex
-00002c10: 7420 7c20 656e 636f 6465 7320 6368 6172  t | encodes char
-00002c20: 6163 7465 7273 2066 726f 6d20 7468 6569  acters from thei
-00002c30: 7220 287a 6572 6f2d 6c65 6674 2d70 6164  r (zero-left-pad
-00002c40: 6465 6429 206f 7264 696e 616c 7320 7573  ded) ordinals us
-00002c50: 696e 6720 7072 6566 6978 2062 6974 7320  ing prefix bits 
-00002c60: 6031 3131 3160 0a60 6d61 6e63 6865 7374  `1111`.`manchest
-00002c70: 6572 2d69 6e76 6572 7465 6460 207c 2074  er-inverted` | t
-00002c80: 6578 7420 3c2d 3e20 6d61 6e63 6865 7374  ext <-> manchest
-00002c90: 6572 2065 6e63 6f64 6564 2074 6578 7420  er encoded text 
-00002ca0: 7c20 584f 5265 7320 6561 6368 2062 6974  | XORes each bit
-00002cb0: 206f 6620 7468 6520 696e 7075 7420 7769   of the input wi
-00002cc0: 7468 2060 3130 600a 606f 6374 616c 2d73  th `10`.`octal-s
-00002cd0: 7061 6365 6460 207c 2074 6578 7420 3c2d  paced` | text <-
-00002ce0: 3e20 6f63 7461 6c20 6469 6769 7473 2028  > octal digits (
-00002cf0: 7768 6974 6573 7061 6365 2d73 6570 6172  whitespace-separ
-00002d00: 6174 6564 2920 7c20 6475 6d6d 7920 6f63  ated) | dummy oc
-00002d10: 7461 6c20 636f 6e76 6572 7369 6f6e 0a60  tal conversion.`
-00002d20: 6f72 6469 6e61 6c2d 7370 6163 6564 6020  ordinal-spaced` 
-00002d30: 7c20 7465 7874 203c 2d3e 206f 7264 696e  | text <-> ordin
-00002d40: 616c 2064 6967 6974 7320 2877 6869 7465  al digits (white
-00002d50: 7370 6163 652d 7365 7061 7261 7465 6429  space-separated)
-00002d60: 207c 2064 756d 6d79 2063 6861 7261 6374   | dummy charact
-00002d70: 6572 206f 7264 696e 616c 7320 636f 6e76  er ordinals conv
-00002d80: 6572 7369 6f6e 0a60 736f 7574 6870 6172  ersion.`southpar
-00002d90: 6b2d 6963 6173 6560 207c 2074 6578 7420  k-icase` | text 
-00002da0: 3c2d 3e20 4b65 6e6e 7927 7320 6c61 6e67  <-> Kenny's lang
-00002db0: 7561 6765 207c 2073 616d 6520 6173 2060  uage | same as `
-00002dc0: 736f 7574 6870 6172 6b60 2062 7574 2063  southpark` but c
-00002dd0: 6173 6520 696e 7365 6e73 6974 6976 650a  ase insensitive.
-00002de0: 6077 6869 7465 7370 6163 655f 6166 7465  `whitespace_afte
-00002df0: 725f 6265 666f 7265 6020 7c20 7465 7874  r_before` | text
-00002e00: 203c 2d3e 206c 696e 6573 206f 6620 7768   <-> lines of wh
-00002e10: 6974 6573 7061 6365 735b 6c65 7474 6572  itespaces[letter
-00002e20: 5d77 6869 7465 7370 6163 6573 207c 2065  ]whitespaces | e
-00002e30: 6e63 6f64 6573 2063 6861 7261 6374 6572  ncodes character
-00002e40: 7320 6173 206e 6577 2063 6861 7261 6374  s as new charact
-00002e50: 6572 7320 7769 7468 2077 6869 7465 7370  ers with whitesp
-00002e60: 6163 6573 2062 6566 6f72 6520 616e 6420  aces before and 
-00002e70: 6166 7465 7220 6163 636f 7264 696e 6720  after according 
-00002e80: 746f 2061 6e20 6571 7561 7469 6f6e 2064  to an equation d
-00002e90: 6573 6372 6962 6564 2069 6e20 7468 6520  escribed in the 
-00002ea0: 636f 6465 6320 6e61 6d65 2028 652e 672e  codec name (e.g.
-00002eb0: 2022 6077 6869 7465 7370 6163 652b 322a   "`whitespace+2*
-00002ec0: 6166 7465 722d 332a 6265 666f 7265 6022  after-3*before`"
-00002ed0: 290a 0a0a 0a                             )....
+00000ea0: 4741 4741 4141 4754 4741 4741 4141 4754  GAGAAAGTGAGAAAGT
+00000eb0: 430d 0a0d 0a24 2065 6368 6f20 2d65 6e20  C....$ echo -en 
+00000ec0: 2254 6573 7420 7374 7269 6e67 2220 7c20  "Test string" | 
+00000ed0: 636f 6465 7874 2065 6e63 6f64 6520 7265  codext encode re
+00000ee0: 7665 7273 6520 6d6f 7273 6520 646e 612d  verse morse dna-
+00000ef0: 3220 6f63 7461 6c0d 0a31 3031 3130 3731  2 octal..1011071
+00000f00: 3234 3130 3331 3031 3130 3731 3234 3130  2410310110712410
+00000f10: 3331 3031 3130 3731 3234 3130 3731 3031  3101107124107101
+00000f20: 3130 3731 3031 3130 3131 3031 3130 3731  1071011011011071
+00000f30: 3234 3130 3331 3031 3130 3731 3234 3130  2410310110712410
+00000f40: 3731 3031 3130 3731 3031 3130 3131 3031  7101107101101101
+00000f50: 3130 3731 3234 3130 3731 3031 3130 3731  1071241071011071
+00000f60: 3234 3130 3731 3031 3130 3731 3031 3130  2410710110710110
+00000f70: 3131 3031 3130 3731 3234 3130 3731 3031  1101107124107101
+00000f80: 3130 3731 3234 3130 3331 3031 3130 3731  1071241031011071
+00000f90: 3234 3130 3731 3031 3130 3731 3031 3130  2410710110710110
+00000fa0: 3131 3031 3130 3731 3234 3130 3331 3031  1101107124103101
+00000fb0: 3130 3731 3031 3130 3131 3031 3130 3731  1071011011011071
+00000fc0: 3234 3130 3731 3031 3130 3731 3234 3130  2410710110712410
+00000fd0: 3731 3031 3130 3731 3234 3130 3731 3031  7101107124107101
+00000fe0: 3130 3731 3031 3130 3131 3031 3130 3731  1071011011011071
+00000ff0: 3234 3132 3431 3031 3130 3731 3031 3130  2412410110710110
+00001000: 3131 3031 3130 3731 3234 3130 3331 3031  1101107124103101
+00001010: 3130 3731 3031 3130 3131 3031 3130 3731  1071011011011071
+00001020: 3234 3130 3731 3031 3130 3731 3234 3130  2410710110712410
+00001030: 3731 3031 3130 3731 3234 3130 3731 3031  7101107124107101
+00001040: 3130 3731 3031 3130 3131 3031 3130 3731  1071011011011071
+00001050: 3234 3130 3731 3031 3130 3731 3031 3130  2410710110710110
+00001060: 3131 3031 3130 3731 3234 3130 330d 0a0d  1101107124103...
+00001070: 0a24 2065 6368 6f20 2d65 6e20 2241 4754  .$ echo -en "AGT
+00001080: 4341 4754 4341 4754 4741 4741 4141 4754  CAGTCAGTGAGAAAGT
+00001090: 4341 4754 4741 4741 4141 4754 4741 4754  CAGTGAGAAAGTGAGT
+000010a0: 4741 4741 4141 4754 4741 4754 4341 4754  GAGAAAGTGAGTCAGT
+000010b0: 4741 4741 4141 4754 4341 4741 4141 4754  GAGAAAGTCAGAAAGT
+000010c0: 4741 4754 4741 4754 4741 4741 4141 4754  GAGTGAGTGAGAAAGT
+000010d0: 5441 4741 4141 4754 4341 4741 4141 4754  TAGAAAGTCAGAAAGT
+000010e0: 4741 4754 4741 4754 4741 4741 4141 4754  GAGTGAGTGAGAAAGT
+000010f0: 4741 4741 4141 4754 4322 207c 2063 6f64  GAGAAAGTC" | cod
+00001100: 6578 7420 2d64 2064 6e61 2d32 206d 6f72  ext -d dna-2 mor
+00001110: 7365 2072 6576 6572 7365 0d0a 7465 7374  se reverse..test
+00001120: 2073 7472 696e 670d 0a60 6060 0d0a 0d0a   string..```....
+00001130: 2323 203a 636f 6d70 7574 6572 3a20 5573  ## :computer: Us
+00001140: 6167 6520 2862 6173 6520 434c 4920 746f  age (base CLI to
+00001150: 6f6c 2920 3c61 2068 7265 663d 2268 7474  ol) <a href="htt
+00001160: 7073 3a2f 2f74 7769 7474 6572 2e63 6f6d  ps://twitter.com
+00001170: 2f69 6e74 656e 742f 7477 6565 743f 7465  /intent/tweet?te
+00001180: 7874 3d44 6562 6173 6525 3230 2d25 3230  xt=Debase%20-%20
+00001190: 4465 636f 6465 2532 3061 6e79 2532 306d  Decode%20any%20m
+000011a0: 756c 7469 2d6c 6179 6572 2532 3062 6173  ulti-layer%20bas
+000011b0: 652d 656e 636f 6465 6425 3230 7374 7269  e-encoded%20stri
+000011c0: 6e67 2e25 3044 2530 4150 7974 686f 6e25  ng.%0D%0APython%
+000011d0: 3230 746f 6f6c 2532 3066 6f72 2532 3064  20tool%20for%20d
+000011e0: 6563 6f64 696e 6725 3230 616e 7925 3230  ecoding%20any%20
+000011f0: 6261 7365 2d65 6e63 6f64 6564 2532 3073  base-encoded%20s
+00001200: 7472 696e 672c 2532 3065 7665 6e25 3230  tring,%20even%20
+00001210: 7768 656e 2532 3065 6e63 6f64 6564 2532  when%20encoded%2
+00001220: 3077 6974 6825 3230 6d75 6c74 6970 6c65  0with%20multiple
+00001230: 2532 306c 6179 6572 732e 2530 4425 3041  %20layers.%0D%0A
+00001240: 6874 7470 7325 3361 2532 6625 3266 6769  https%3a%2f%2fgi
+00001250: 7468 7562 2532 6563 6f6d 2532 6664 686f  thub%2ecom%2fdho
+00001260: 6e64 7461 2532 6670 7974 686f 6e2d 636f  ndta%2fpython-co
+00001270: 6465 7874 2530 4425 3041 2668 6173 6874  dext%0D%0A&hasht
+00001280: 6167 733d 7079 7468 6f6e 2c62 6173 652c  ags=python,base,
+00001290: 656e 636f 6469 6e67 732c 636f 6465 6373  encodings,codecs
+000012a0: 2c63 7279 7074 6f67 7261 7068 792c 7374  ,cryptography,st
+000012b0: 6567 616e 6f2c 7374 6567 616e 6f67 7261  egano,steganogra
+000012c0: 7068 792c 6374 6674 6f6f 6c73 223e 3c69  phy,ctftools"><i
+000012d0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+000012e0: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+000012f0: 6164 6765 2f54 7765 6574 2532 3028 6465  adge/Tweet%20(de
+00001300: 6261 7365 292d 2d6c 6967 6874 6772 6579  base)--lightgrey
+00001310: 3f6c 6f67 6f3d 7477 6974 7465 7226 7374  ?logo=twitter&st
+00001320: 796c 653d 736f 6369 616c 2220 616c 743d  yle=social" alt=
+00001330: 2254 7765 6574 206f 6e20 6465 6261 7365  "Tweet on debase
+00001340: 2220 6865 6967 6874 3d22 3230 222f 3e3c  " height="20"/><
+00001350: 2f61 3e0d 0a0d 0a60 6060 7365 7373 696f  /a>....```sessio
+00001360: 6e0d 0a24 2065 6368 6f20 2254 6573 7420  n..$ echo "Test 
+00001370: 7374 7269 6e67 2021 2220 7c20 6261 7365  string !" | base
+00001380: 3132 320d 0a2a 2e37 2166 7439 efbf bd2d  122..*.7!ft9...-
+00001390: 6639 c382 0d0a 0d0a 2420 6563 686f 2022  f9......$ echo "
+000013a0: 5465 7374 2073 7472 696e 6720 2122 207c  Test string !" |
+000013b0: 2062 6173 6539 3120 0d0a 224f 4e4b 3b57   base91 .."ONK;W
+000013c0: 445a 4d25 5a25 7845 374c 0d0a 0d0a 2420  DZM%Z%xE7L....$ 
+000013d0: 6563 686f 2022 5465 7374 2073 7472 696e  echo "Test strin
+000013e0: 6720 2122 207c 2062 6173 6539 3120 7c20  g !" | base91 | 
+000013f0: 6261 7365 3835 0d0a 4232 507c 424a 3641  base85..B2P|BJ6A
+00001400: 2b6e 4f28 6a7c 2d63 7474 6c25 0d0a 0d0a  +nO(j|-cttl%....
+00001410: 2420 6563 686f 2022 5465 7374 2073 7472  $ echo "Test str
+00001420: 696e 6720 2122 207c 2062 6173 6539 3120  ing !" | base91 
+00001430: 7c20 6261 7365 3835 207c 2062 6173 6533  | base85 | base3
+00001440: 3620 7c20 6261 7365 3538 2d66 6c69 636b  6 | base58-flick
+00001450: 720d 0a51 5678 3574 7667 6a76 4341 6b58  r..QVx5tvgjvCAkX
+00001460: 614d 5375 4b6f 516d 436e 6a65 4356 3159  aMSuKoQmCnjeCV1Y
+00001470: 7979 5233 5745 7255 5545 7246 660d 0a0d  yyR3WErUUErFf...
+00001480: 0a24 2065 6368 6f20 2254 6573 7420 7374  .$ echo "Test st
+00001490: 7269 6e67 2021 2220 7c20 6261 7365 3931  ring !" | base91
+000014a0: 207c 2062 6173 6538 3520 7c20 6261 7365   | base85 | base
+000014b0: 3336 207c 2062 6173 6535 382d 666c 6963  36 | base58-flic
+000014c0: 6b72 207c 2062 6173 6535 382d 666c 6963  kr | base58-flic
+000014d0: 6b72 202d 6420 7c20 6261 7365 3336 202d  kr -d | base36 -
+000014e0: 6420 7c20 6261 7365 3835 202d 6420 7c20  d | base85 -d | 
+000014f0: 6261 7365 3931 202d 640d 0a54 6573 7420  base91 -d..Test 
+00001500: 7374 7269 6e67 2021 0d0a 6060 600d 0a0d  string !..```...
+00001510: 0a60 6060 7365 7373 696f 6e0d 0a24 2065  .```session..$ e
+00001520: 6368 6f20 2254 6573 7420 7374 7269 6e67  cho "Test string
+00001530: 2021 2220 7c20 6261 7365 3931 207c 2062   !" | base91 | b
+00001540: 6173 6538 3520 7c20 6261 7365 3336 207c  ase85 | base36 |
+00001550: 2062 6173 6535 382d 666c 6963 6b72 207c   base58-flickr |
+00001560: 2064 6562 6173 6520 2d6d 2033 0d0a 5465   debase -m 3..Te
+00001570: 7374 2073 7472 696e 6720 210d 0a0d 0a24  st string !....$
+00001580: 2065 6368 6f20 2254 6573 7420 7374 7269   echo "Test stri
+00001590: 6e67 2021 2220 7c20 6261 7365 3931 207c  ng !" | base91 |
+000015a0: 2062 6173 6538 3520 7c20 6261 7365 3336   base85 | base36
+000015b0: 207c 2062 6173 6535 382d 666c 6963 6b72   | base58-flickr
+000015c0: 207c 2064 6562 6173 6520 2d66 2054 6573   | debase -f Tes
+000015d0: 740d 0a54 6573 7420 7374 7269 6e67 2021  t..Test string !
+000015e0: 0d0a 6060 600d 0a0d 0a23 2320 3a63 6f6d  ..```....## :com
+000015f0: 7075 7465 723a 2055 7361 6765 2028 5079  puter: Usage (Py
+00001600: 7468 6f6e 290d 0a0d 0a47 6574 7469 6e67  thon)....Getting
+00001610: 2074 6865 206c 6973 7420 6f66 2061 7661   the list of ava
+00001620: 696c 6162 6c65 2063 6f64 6563 733a 0d0a  ilable codecs:..
+00001630: 0d0a 6060 6070 7974 686f 6e0d 0a3e 3e3e  ..```python..>>>
+00001640: 2069 6d70 6f72 7420 636f 6465 7874 0d0a   import codext..
+00001650: 0d0a 3e3e 3e20 636f 6465 7874 2e6c 6973  ..>>> codext.lis
+00001660: 7428 290d 0a5b 2761 7363 6969 3835 272c  t()..['ascii85',
+00001670: 2027 6261 7365 3835 272c 2027 6261 7365   'base85', 'base
+00001680: 3130 3027 2c20 2762 6173 6531 3232 272c  100', 'base122',
+00001690: 202e 2e2e 2c20 2774 6f6d 746f 6d27 2c20   ..., 'tomtom', 
+000016a0: 2764 6e61 272c 2027 6874 6d6c 272c 2027  'dna', 'html', '
+000016b0: 6d61 726b 646f 776e 272c 2027 7572 6c27  markdown', 'url'
+000016c0: 2c20 2772 6573 6973 746f 7227 2c20 2773  , 'resistor', 's
+000016d0: 6d73 272c 2027 7768 6974 6573 7061 6365  ms', 'whitespace
+000016e0: 272c 2027 7768 6974 6573 7061 6365 2d61  ', 'whitespace-a
+000016f0: 6674 6572 2d62 6566 6f72 6527 5d0d 0a0d  fter-before']...
+00001700: 0a3e 3e3e 2063 6f64 6578 742e 656e 636f  .>>> codext.enco
+00001710: 6465 2822 7468 6973 2069 7320 6120 7465  de("this is a te
+00001720: 7374 222c 2022 6261 7365 3538 2d62 6974  st", "base58-bit
+00001730: 636f 696e 2229 0d0a 276a 6f39 3177 614c  coin")..'jo91waL
+00001740: 5141 314e 4e65 426d 5a4b 5546 270d 0a0d  QA1NNeBmZKUF'...
+00001750: 0a3e 3e3e 2063 6f64 6578 742e 656e 636f  .>>> codext.enco
+00001760: 6465 2822 7468 6973 2069 7320 6120 7465  de("this is a te
+00001770: 7374 222c 2022 6261 7365 3538 2d72 6970  st", "base58-rip
+00001780: 706c 6522 290d 0a27 6a6f 3972 4132 4c51  ple")..'jo9rA2LQ
+00001790: 7772 3434 6542 6d5a 4b37 4527 0d0a 0d0a  wr44eBmZK7E'....
+000017a0: 3e3e 3e20 636f 6465 7874 2e65 6e63 6f64  >>> codext.encod
+000017b0: 6528 2274 6869 7320 6973 2061 2074 6573  e("this is a tes
+000017c0: 7422 2c20 2262 6173 6535 382d 7572 6c22  t", "base58-url"
+000017d0: 290d 0a27 4a4e 3931 577a 6b70 6131 6e6e  )..'JN91Wzkpa1nn
+000017e0: 4462 4c79 6a74 6627 0d0a 0d0a 3e3e 3e20  DbLyjtf'....>>> 
+000017f0: 636f 6465 6373 2e65 6e63 6f64 6528 2274  codecs.encode("t
+00001800: 6869 7320 6973 2061 2074 6573 7422 2c20  his is a test", 
+00001810: 2262 6173 6531 3030 2229 0d0a 27f0 9f91  "base100")..'...
+00001820: abf0 9f91 9ff0 9f91 a0f0 9f91 aaf0 9f90  ................
+00001830: 97f0 9f91 a0f0 9f91 aaf0 9f90 97f0 9f91  ................
+00001840: 98f0 9f90 97f0 9f91 abf0 9f91 9cf0 9f91  ................
+00001850: aaf0 9f91 ab27 0d0a 0d0a 3e3e 3e20 636f  .....'....>>> co
+00001860: 6465 6373 2e64 6563 6f64 6528 22f0 9f91  decs.decode("...
+00001870: abf0 9f91 9ff0 9f91 a0f0 9f91 aaf0 9f90  ................
+00001880: 97f0 9f91 a0f0 9f91 aaf0 9f90 97f0 9f91  ................
+00001890: 98f0 9f90 97f0 9f91 abf0 9f91 9cf0 9f91  ................
+000018a0: aaf0 9f91 ab22 2c20 2262 6173 6531 3030  .....", "base100
+000018b0: 2229 0d0a 2774 6869 7320 6973 2061 2074  ")..'this is a t
+000018c0: 6573 7427 0d0a 0d0a 3e3e 3e20 666f 7220  est'....>>> for 
+000018d0: 6920 696e 2072 616e 6765 2838 293a 0d0a  i in range(8):..
+000018e0: 2020 2020 2020 2020 7072 696e 7428 636f          print(co
+000018f0: 6465 7874 2e65 6e63 6f64 6528 2274 6869  dext.encode("thi
+00001900: 7320 6973 2061 2074 6573 7422 2c20 2264  s is a test", "d
+00001910: 6e61 2d25 6422 2025 2028 6920 2b20 3129  na-%d" % (i + 1)
+00001920: 2929 0d0a 4754 4741 4743 4341 4743 4347  ))..GTGAGCCAGCCG
+00001930: 4754 4154 4143 4141 4743 4347 4754 4154  GTATACAAGCCGGTAT
+00001940: 4143 4141 4743 4147 4143 4141 4754 4741  ACAAGCAGACAAGTGA
+00001950: 4743 4747 4754 4154 4754 4741 0d0a 4354  GCGGGTATGTGA..CT
+00001960: 4341 4347 4741 4347 4743 4354 4154 4147  CACGGACGGCCTATAG
+00001970: 4141 4347 4743 4354 4154 4147 4141 4347  AACGGCCTATAGAACG
+00001980: 4143 4147 4141 4354 4341 4347 4343 4354  ACAGAACTCACGCCCT
+00001990: 4154 4354 4341 0d0a 4143 4147 4154 5447  ATCTCA..ACAGATTG
+000019a0: 4154 5441 4143 4743 4754 4747 4154 5441  ATTAACGCGTGGATTA
+000019b0: 4143 4743 4754 4747 4154 4741 4754 4747  ACGCGTGGATGAGTGG
+000019c0: 4143 4147 4154 4141 4143 4743 4143 4147  ACAGATAAACGCACAG
+000019d0: 0d0a 4147 4143 4154 5443 4154 5441 4147  ..AGACATTCATTAAG
+000019e0: 4347 4354 4343 4154 5441 4147 4347 4354  CGCTCCATTAAGCGCT
+000019f0: 4343 4154 4341 4354 4343 4147 4143 4154  CCATCACTCCAGACAT
+00001a00: 4141 4147 4347 4147 4143 0d0a 5443 5447  AAAGCGAGAC..TCTG
+00001a10: 5441 4147 5441 4154 5443 4743 4741 4747  TAAGTAATTCGCGAGG
+00001a20: 5441 4154 5443 4743 4741 4747 5441 4754  TAATTCGCGAGGTAGT
+00001a30: 4741 4747 5443 5447 5441 5454 5443 4743  GAGGTCTGTATTTCGC
+00001a40: 5443 5447 0d0a 5447 5443 5441 4143 5441  TCTG..TGTCTAACTA
+00001a50: 4154 5447 4347 4341 4343 5441 4154 5447  ATTGCGCACCTAATTG
+00001a60: 4347 4341 4343 5441 4354 4341 4343 5447  CGCACCTACTCACCTG
+00001a70: 5443 5441 5454 5447 4347 5447 5443 0d0a  TCTATTTGCGTGTC..
+00001a80: 4741 4754 4743 4354 4743 4347 4741 5441  GAGTGCCTGCCGGATA
+00001a90: 5443 5454 4743 4347 4741 5441 5443 5454  TCTTGCCGGATATCTT
+00001aa0: 4743 5447 5443 5454 4741 4754 4743 4747  GCTGTCTTGAGTGCGG
+00001ab0: 4741 5441 4741 4754 0d0a 4341 4354 4347  GATAGAGT..CACTCG
+00001ac0: 4754 4347 4743 4341 5441 5447 5454 4347  GTCGGCCATATGTTCG
+00001ad0: 4743 4341 5441 5447 5454 4347 5443 5447  GCCATATGTTCGTCTG
+00001ae0: 5454 4341 4354 4347 4343 4341 5441 4341  TTCACTCGCCCATACA
+00001af0: 4354 0d0a 3e3e 3e20 636f 6465 7874 2e64  CT..>>> codext.d
+00001b00: 6563 6f64 6528 2247 5447 4147 4343 4147  ecode("GTGAGCCAG
+00001b10: 4343 4747 5441 5441 4341 4147 4343 4747  CCGGTATACAAGCCGG
+00001b20: 5441 5441 4341 4147 4341 4741 4341 4147  TATACAAGCAGACAAG
+00001b30: 5447 4147 4347 4747 5441 5447 5447 4122  TGAGCGGGTATGTGA"
+00001b40: 2c20 2264 6e61 2d31 2229 0d0a 2774 6869  , "dna-1")..'thi
+00001b50: 7320 6973 2061 2074 6573 7427 0d0a 0d0a  s is a test'....
+00001b60: 3e3e 3e20 636f 6465 6373 2e65 6e63 6f64  >>> codecs.encod
+00001b70: 6528 2274 6869 7320 6973 2061 2074 6573  e("this is a tes
+00001b80: 7422 2c20 226d 6f72 7365 2229 0d0a 272d  t", "morse")..'-
+00001b90: 202e 2e2e 2e20 2e2e 202e 2e2e 202f 202e   .... .. ... / .
+00001ba0: 2e20 2e2e 2e20 2f20 2e2d 202f 202d 202e  . ... / .- / - .
+00001bb0: 202e 2e2e 202d 270d 0a0d 0a3e 3e3e 2063   ... -'....>>> c
+00001bc0: 6f64 6563 732e 6465 636f 6465 2822 2d20  odecs.decode("- 
+00001bd0: 2e2e 2e2e 202e 2e20 2e2e 2e20 2f20 2e2e  .... .. ... / ..
+00001be0: 202e 2e2e 202f 202e 2d20 2f20 2d20 2e20   ... / .- / - . 
+00001bf0: 2e2e 2e20 2d22 2c20 226d 6f72 7365 2229  ... -", "morse")
+00001c00: 0d0a 2774 6869 7320 6973 2061 2074 6573  ..'this is a tes
+00001c10: 7427 0d0a 0d0a 3e3e 3e20 7769 7468 206f  t'....>>> with o
+00001c20: 7065 6e28 226d 6f72 7365 2e74 7874 222c  pen("morse.txt",
+00001c30: 2027 7727 2c20 656e 636f 6469 6e67 3d22   'w', encoding="
+00001c40: 6d6f 7273 6522 2920 6173 2066 3a0d 0a09  morse") as f:...
+00001c50: 662e 7772 6974 6528 2274 6869 7320 6973  f.write("this is
+00001c60: 2061 2074 6573 7422 290d 0a31 340d 0a0d   a test")..14...
+00001c70: 0a3e 3e3e 2077 6974 6820 6f70 656e 2822  .>>> with open("
+00001c80: 6d6f 7273 652e 7478 7422 2c65 6e63 6f64  morse.txt",encod
+00001c90: 696e 673d 226d 6f72 7365 2229 2061 7320  ing="morse") as 
+00001ca0: 663a 0d0a 0966 2e72 6561 6428 290d 0a27  f:...f.read()..'
+00001cb0: 7468 6973 2069 7320 6120 7465 7374 270d  this is a test'.
+00001cc0: 0a0d 0a3e 3e3e 2063 6f64 6578 742e 6465  ...>>> codext.de
+00001cd0: 636f 6465 2822 2222 0d0a 2020 2020 2020  code("""..      
+00001ce0: 3d20 2020 2020 2020 2020 2020 200d 0a20  =            .. 
+00001cf0: 2020 2020 2020 2020 2020 2020 2058 2020               X  
+00001d00: 2020 2020 2020 200d 0a20 2020 3a20 2020         ..   :   
+00001d10: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00001d20: 2078 2020 2020 2020 2020 200d 0a20 206e   x         ..  n
+00001d30: 2020 0d0a 2020 2020 7220 0d0a 2020 2020    ..    r ..    
+00001d40: 2020 2020 7920 2020 0d0a 2020 2020 2020      y   ..      
+00001d50: 5920 2020 2020 2020 2020 2020 200d 0a20  Y            .. 
+00001d60: 2020 2020 2020 2020 2020 2020 2079 2020               y  
+00001d70: 2020 2020 2020 0d0a 2020 2020 2070 2020        ..     p  
+00001d80: 2020 0d0a 2020 2020 2020 2020 2061 2020    ..         a  
+00001d90: 2020 2020 200d 0a20 6020 2020 2020 2020       .. `       
+00001da0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00001db0: 206e 2020 2020 2020 2020 2020 2020 0d0a   n            ..
+00001dc0: 2020 2020 2020 2020 2020 7c20 2020 200d            |    .
+00001dd0: 0a20 2061 2020 2020 2020 2020 2020 0d0a  .  a          ..
+00001de0: 6f20 2020 200d 0a20 2020 2020 2020 6820  o    ..       h 
+00001df0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00001e00: 2020 2060 2020 2020 2020 2020 2020 2020     `            
+00001e10: 0d0a 2020 2020 2020 2020 2020 6720 2020  ..          g   
+00001e20: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00001e30: 2020 2020 2020 2020 206f 200d 0a20 2020           o ..   
+00001e40: 7a20 2020 2020 2022 2222 2c20 2277 6869  z      """, "whi
+00001e50: 7465 7370 6163 652d 6166 7465 722b 6265  tespace-after+be
+00001e60: 666f 7265 2229 0d0a 2743 5343 7b6e 6f74  fore")..'CSC{not
+00001e70: 5f73 6f5f 696e 7669 7369 626c 657d 270d  _so_invisible}'.
+00001e80: 0a0d 0a3e 3e3e 2070 7269 6e74 2863 6f64  ...>>> print(cod
+00001e90: 6578 742e 656e 636f 6465 2822 416e 2065  ext.encode("An e
+00001ea0: 7861 6d70 6c65 2074 6573 7420 7374 7269  xample test stri
+00001eb0: 6e67 222c 2022 6261 7564 6f74 2d74 6170  ng", "baudot-tap
+00001ec0: 6522 2929 0d0a 2a2a 2a2e 2a2a 0d0a 2020  e"))..***.**..  
+00001ed0: 202e 202a 0d0a 2a2a 2a2e 2a20 0d0a 2a20   . *..***.* ..* 
+00001ee0: 202e 2020 0d0a 2020 202e 2a20 0d0a 2a20   .  ..   .* ..* 
+00001ef0: 202e 2a20 0d0a 2020 202e 202a 0d0a 2a2a   .* ..   . *..**
+00001f00: 202e 2a20 0d0a 2a2a 2a2e 2a2a 0d0a 2a2a   .* ..***.**..**
+00001f10: 202e 2a2a 0d0a 2020 202e 2a20 0d0a 2a20   .**..   .* ..* 
+00001f20: 202e 2020 0d0a 2a20 2a2e 202a 0d0a 2020   .  ..* *. *..  
+00001f30: 202e 2a20 0d0a 2a20 2a2e 2020 0d0a 2a20   .* ..* *.  ..* 
+00001f40: 2a2e 202a 0d0a 2a20 202e 2020 0d0a 2a20  *. *..*  .  ..* 
+00001f50: 2a2e 2020 0d0a 2a20 2a2e 202a 0d0a 2a2a  *.  ..* *. *..**
+00001f60: 2a2e 2020 0d0a 2020 2a2e 2a20 0d0a 2a2a  *.  ..  *.* ..**
+00001f70: 2a2e 2a20 0d0a 202a 202e 2a20 0d0a 6060  *.* .. * .* ..``
+00001f80: 600d 0a0d 0a23 2320 3a70 6167 655f 7769  `....## :page_wi
+00001f90: 7468 5f63 7572 6c3a 204c 6973 7420 6f66  th_curl: List of
+00001fa0: 2063 6f64 6563 730d 0a0d 0a2a 2a43 6f64   codecs....**Cod
+00001fb0: 6563 2a2a 207c 202a 2a43 6f6e 7665 7273  ec** | **Convers
+00001fc0: 696f 6e73 2a2a 207c 202a 2a43 6f6d 6d65  ions** | **Comme
+00001fd0: 6e74 2a2a 0d0a 3a2d 2d2d 3a20 7c20 3a2d  nt**..:---: | :-
+00001fe0: 2d2d 3a20 7c20 2d2d 2d0d 0a60 6131 7a32  --: | ---..`a1z2
+00001ff0: 3660 207c 2074 6578 7420 3c2d 3e20 616c  6` | text <-> al
+00002000: 7068 6162 6574 206f 7264 6572 206e 756d  phabet order num
+00002010: 6265 7273 207c 206b 6565 7073 2077 6f72  bers | keeps wor
+00002020: 6473 2077 6869 7465 7370 6163 652d 7365  ds whitespace-se
+00002030: 7061 7261 7465 6420 616e 6420 7573 6573  parated and uses
+00002040: 2061 2063 7573 746f 6d20 6368 6172 6163   a custom charac
+00002050: 7465 7220 7365 7061 7261 746f 720d 0a60  ter separator..`
+00002060: 6166 6669 6e65 6020 7c20 7465 7874 203c  affine` | text <
+00002070: 2d3e 2061 6666 696e 6520 6369 7068 6572  -> affine cipher
+00002080: 7465 7874 207c 2061 6b61 2041 6666 696e  text | aka Affin
+00002090: 6520 4369 7068 6572 0d0a 6061 7363 6969  e Cipher..`ascii
+000020a0: 3835 6020 7c20 7465 7874 203c 2d3e 2061  85` | text <-> a
+000020b0: 7363 6969 3835 2065 6e63 6f64 6564 2074  scii85 encoded t
+000020c0: 6578 7420 7c20 5079 7468 6f6e 2033 206f  ext | Python 3 o
+000020d0: 6e6c 790d 0a60 6174 6261 7368 6020 7c20  nly..`atbash` | 
+000020e0: 7465 7874 203c 2d3e 2041 7462 6173 6820  text <-> Atbash 
+000020f0: 6369 7068 6572 7465 7874 207c 2061 6b61  ciphertext | aka
+00002100: 2041 7462 6173 6820 4369 7068 6572 0d0a   Atbash Cipher..
+00002110: 6062 6163 6f6e 6020 7c20 7465 7874 203c  `bacon` | text <
+00002120: 2d3e 2042 6163 6f6e 2063 6970 6865 7274  -> Bacon ciphert
+00002130: 6578 7420 7c20 616b 6120 4261 636f 6e69  ext | aka Baconi
+00002140: 616e 2043 6970 6865 720d 0a60 6261 7262  an Cipher..`barb
+00002150: 6965 2d4e 6020 7c20 7465 7874 203c 2d3e  ie-N` | text <->
+00002160: 2062 6172 6269 6520 6369 7068 6572 7465   barbie cipherte
+00002170: 7874 207c 2061 6b61 2042 6172 6269 6520  xt | aka Barbie 
+00002180: 5479 7065 7772 6974 6572 2028 4e20 6265  Typewriter (N be
+00002190: 6c6f 6e67 7320 746f 205b 312c 2034 5d29  longs to [1, 4])
+000021a0: 0d0a 6062 6173 6558 5860 207c 2074 6578  ..`baseXX` | tex
+000021b0: 7420 3c2d 3e20 6261 7365 5858 207c 2073  t <-> baseXX | s
+000021c0: 6565 205b 6261 7365 2065 6e63 6f64 696e  ee [base encodin
+000021d0: 6773 5d28 6874 7470 733a 2f2f 7079 7468  gs](https://pyth
+000021e0: 6f6e 2d63 6f64 6578 742e 7265 6164 7468  on-codext.readth
+000021f0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+00002200: 7374 2f65 6e63 2f62 6173 652e 6874 6d6c  st/enc/base.html
+00002210: 2920 2869 6e63 6c20 6261 7365 3332 2c20  ) (incl base32, 
+00002220: 3336 2c20 3435 2c20 3538 2c20 3632 2c20  36, 45, 58, 62, 
+00002230: 3633 2c20 3634 2c20 3931 2c20 3130 302c  63, 64, 91, 100,
+00002240: 2031 3232 290d 0a60 6261 7564 6f74 6020   122)..`baudot` 
+00002250: 7c20 7465 7874 203c 2d3e 2042 6175 646f  | text <-> Baudo
+00002260: 7420 636f 6465 2062 6974 7320 7c20 7375  t code bits | su
+00002270: 7070 6f72 7473 2043 4349 5454 2d31 2c20  pports CCITT-1, 
+00002280: 4343 4954 542d 322c 2045 552f 4652 2c20  CCITT-2, EU/FR, 
+00002290: 4954 4131 2c20 4954 4132 2c20 4d54 4b2d  ITA1, ITA2, MTK-
+000022a0: 3220 2850 7974 686f 6e33 206f 6e6c 7929  2 (Python3 only)
+000022b0: 2c20 554b 2c20 2e2e 2e0d 0a60 6263 6460  , UK, .....`bcd`
+000022c0: 207c 2074 6578 7420 3c2d 3e20 6269 6e61   | text <-> bina
+000022d0: 7279 2063 6f64 6564 2064 6563 696d 616c  ry coded decimal
+000022e0: 2074 6578 7420 7c20 656e 636f 6465 7320   text | encodes 
+000022f0: 6368 6172 6163 7465 7273 2066 726f 6d20  characters from 
+00002300: 7468 6569 7220 287a 6572 6f2d 6c65 6674  their (zero-left
+00002310: 2d70 6164 6465 6429 206f 7264 696e 616c  -padded) ordinal
+00002320: 730d 0a60 6272 6169 6c6c 6560 207c 2074  s..`braille` | t
+00002330: 6578 7420 3c2d 3e20 6272 6169 6c6c 6520  ext <-> braille 
+00002340: 7379 6d62 6f6c 7320 7c20 5079 7468 6f6e  symbols | Python
+00002350: 2033 206f 6e6c 790d 0a60 6369 7472 6978   3 only..`citrix
+00002360: 6020 7c20 7465 7874 203c 2d3e 2043 6974  ` | text <-> Cit
+00002370: 7269 7820 4354 5831 2063 6970 6865 7274  rix CTX1 ciphert
+00002380: 6578 7420 7c20 616b 6120 4369 7472 6978  ext | aka Citrix
+00002390: 2043 5458 3120 7061 7373 6f72 6420 656e   CTX1 passord en
+000023a0: 636f 6469 6e67 0d0a 6064 6e61 6020 7c20  coding..`dna` | 
+000023b0: 7465 7874 203c 2d3e 2044 4e41 2d4e 2073  text <-> DNA-N s
+000023c0: 6571 7565 6e63 6520 7c20 696d 706c 656d  equence | implem
+000023d0: 656e 7473 2074 6865 2038 2072 756c 6573  ents the 8 rules
+000023e0: 206f 6620 444e 4120 7365 7175 656e 6365   of DNA sequence
+000023f0: 7320 284e 2062 656c 6f6e 6773 2074 6f20  s (N belongs to 
+00002400: 5b31 2c38 5d29 0d0a 6065 7863 6573 7333  [1,8])..`excess3
+00002410: 6020 7c20 7465 7874 203c 2d3e 2058 5333  ` | text <-> XS3
+00002420: 2065 6e63 6f64 6564 2074 6578 7420 7c20   encoded text | 
+00002430: 7573 6573 2045 7863 6573 732d 3320 2861  uses Excess-3 (a
+00002440: 6b61 2053 7469 6269 747a 2063 6f64 6529  ka Stibitz code)
+00002450: 2062 696e 6172 7920 656e 636f 6469 6e67   binary encoding
+00002460: 2074 6f20 636f 6e76 6572 7420 6368 6172   to convert char
+00002470: 6163 7465 7273 2066 726f 6d20 7468 6569  acters from thei
+00002480: 7220 6f72 6469 6e61 6c73 0d0a 6067 7261  r ordinals..`gra
+00002490: 7960 207c 2074 6578 7420 3c2d 3e20 6772  y` | text <-> gr
+000024a0: 6179 2065 6e63 6f64 6564 2074 6578 7420  ay encoded text 
+000024b0: 7c20 616b 6120 7265 666c 6563 7465 6420  | aka reflected 
+000024c0: 6269 6e61 7279 2063 6f64 650d 0a60 677a  binary code..`gz
+000024d0: 6970 6020 7c20 7465 7874 203c 2d3e 2047  ip` | text <-> G
+000024e0: 7a69 702d 636f 6d70 7265 7373 6564 2074  zip-compressed t
+000024f0: 6578 7420 7c20 7374 616e 6461 7264 2047  ext | standard G
+00002500: 7a69 7020 636f 6d70 7265 7373 696f 6e2f  zip compression/
+00002510: 6465 636f 6d70 7265 7373 696f 6e0d 0a60  decompression..`
+00002520: 6874 6d6c 6020 7c20 7465 7874 203c 2d3e  html` | text <->
+00002530: 2048 544d 4c20 656e 7469 7469 6573 207c   HTML entities |
+00002540: 2069 6d70 6c65 6d65 6e74 7320 656e 7469   implements enti
+00002550: 7469 6573 2061 6363 6f72 6469 6e67 2074  ties according t
+00002560: 6f20 5b74 6869 7320 7265 6665 7265 6e63  o [this referenc
+00002570: 655d 2868 7474 7073 3a2f 2f64 6576 2e77  e](https://dev.w
+00002580: 332e 6f72 672f 6874 6d6c 352f 6874 6d6c  3.org/html5/html
+00002590: 2d61 7574 686f 722f 6368 6172 7265 6629  -author/charref)
+000025a0: 0d0a 6069 7073 756d 6020 7c20 7465 7874  ..`ipsum` | text
+000025b0: 203c 2d3e 206c 6174 696e 2077 6f72 6473   <-> latin words
+000025c0: 207c 2061 6b61 206c 6f72 656d 2069 7073   | aka lorem ips
+000025d0: 756d 0d0a 606b 6c6f 7066 6020 7c20 7465  um..`klopf` | te
+000025e0: 7874 203c 2d3e 206b 6c6f 7066 2065 6e63  xt <-> klopf enc
+000025f0: 6f64 6564 2074 6578 7420 7c20 506f 6c79  oded text | Poly
+00002600: 6269 7573 2073 7175 6172 6520 7769 7468  bius square with
+00002610: 2074 7269 7669 616c 2061 6c70 6861 6265   trivial alphabe
+00002620: 7469 6361 6c20 6469 7374 7269 6275 7469  tical distributi
+00002630: 6f6e 0d0a 606c 6565 7473 7065 616b 6020  on..`leetspeak` 
+00002640: 7c20 7465 7874 203c 2d3e 206c 6565 7473  | text <-> leets
+00002650: 7065 616b 2065 6e63 6f64 6564 2074 6578  peak encoded tex
+00002660: 7420 7c20 6261 7365 6420 6f6e 206d 696e  t | based on min
+00002670: 696d 616c 6973 7469 6320 656c 6974 6520  imalistic elite 
+00002680: 7370 6561 6b69 6e67 2072 756c 6573 0d0a  speaking rules..
+00002690: 606c 6574 7465 722d 696e 6469 6365 7360  `letter-indices`
+000026a0: 207c 2074 6578 7420 3c2d 3e20 7465 7874   | text <-> text
+000026b0: 2077 6974 6820 6c65 7474 6572 2069 6e64   with letter ind
+000026c0: 6963 6573 207c 2065 6e63 6f64 6573 2063  ices | encodes c
+000026d0: 6f6e 736f 6e61 6e74 7320 616e 642f 6f72  onsonants and/or
+000026e0: 2076 6f77 656c 7320 7769 7468 2074 6865   vowels with the
+000026f0: 6972 2063 6f72 7265 7370 6f6e 6469 6e67  ir corresponding
+00002700: 2069 6e64 6963 6573 0d0a 606c 7a37 3760   indices..`lz77`
+00002710: 207c 2074 6578 7420 3c2d 3e20 4c5a 3737   | text <-> LZ77
+00002720: 2d63 6f6d 7072 6573 7365 6420 7465 7874  -compressed text
+00002730: 207c 2063 6f6d 7072 6573 7365 7320 7468   | compresses th
+00002740: 6520 6769 7665 6e20 6461 7461 2077 6974  e given data wit
+00002750: 6820 7468 6520 616c 676f 7269 7468 6d20  h the algorithm 
+00002760: 6f66 204c 656d 7065 6c20 616e 6420 5a69  of Lempel and Zi
+00002770: 7620 6f66 2031 3937 370d 0a60 6c7a 3738  v of 1977..`lz78
+00002780: 6020 7c20 7465 7874 203c 2d3e 204c 5a37  ` | text <-> LZ7
+00002790: 382d 636f 6d70 7265 7373 6564 2074 6578  8-compressed tex
+000027a0: 7420 7c20 636f 6d70 7265 7373 6573 2074  t | compresses t
+000027b0: 6865 2067 6976 656e 2064 6174 6120 7769  he given data wi
+000027c0: 7468 2074 6865 2061 6c67 6f72 6974 686d  th the algorithm
+000027d0: 206f 6620 4c65 6d70 656c 2061 6e64 205a   of Lempel and Z
+000027e0: 6976 206f 6620 3139 3738 0d0a 606d 616e  iv of 1978..`man
+000027f0: 6368 6573 7465 7260 207c 2074 6578 7420  chester` | text 
+00002800: 3c2d 3e20 6d61 6e63 6865 7374 6572 2065  <-> manchester e
+00002810: 6e63 6f64 6564 2074 6578 7420 7c20 584f  ncoded text | XO
+00002820: 5265 7320 6561 6368 2062 6974 206f 6620  Res each bit of 
+00002830: 7468 6520 696e 7075 7420 7769 7468 2060  the input with `
+00002840: 3031 600d 0a60 6d61 726b 646f 776e 6020  01`..`markdown` 
+00002850: 7c20 6d61 726b 646f 776e 202d 2d3e 2048  | markdown --> H
+00002860: 544d 4c20 7c20 756e 6964 6972 6563 7469  TML | unidirecti
+00002870: 6f6e 616c 0d0a 606d 6f72 7365 6020 7c20  onal..`morse` | 
+00002880: 7465 7874 203c 2d3e 206d 6f72 7365 2065  text <-> morse e
+00002890: 6e63 6f64 6564 2074 6578 7420 7c20 7573  ncoded text | us
+000028a0: 6573 2077 6869 7465 7370 6163 6520 6173  es whitespace as
+000028b0: 2061 2073 6570 6172 6174 6f72 0d0a 606e   a separator..`n
+000028c0: 6176 616a 6f60 207c 2074 6578 7420 3c2d  avajo` | text <-
+000028d0: 3e20 4e61 7661 6a6f 207c 206f 6e6c 7920  > Navajo | only 
+000028e0: 6861 6e64 6c65 7320 6c65 7474 6572 7320  handles letters 
+000028f0: 286e 6f74 2066 756c 6c20 776f 7264 7320  (not full words 
+00002900: 6672 6f6d 2074 6865 204e 6176 616a 6f20  from the Navajo 
+00002910: 6469 6374 696f 6e61 7279 290d 0a60 6f63  dictionary)..`oc
+00002920: 7461 6c60 207c 2074 6578 7420 3c2d 3e20  tal` | text <-> 
+00002930: 6f63 7461 6c20 6469 6769 7473 207c 2064  octal digits | d
+00002940: 756d 6d79 206f 6374 616c 2063 6f6e 7665  ummy octal conve
+00002950: 7273 696f 6e20 2863 6f6e 7665 7274 7320  rsion (converts 
+00002960: 746f 2033 2d64 6967 6974 7320 6772 6f75  to 3-digits grou
+00002970: 7073 290d 0a60 6f72 6469 6e61 6c60 207c  ps)..`ordinal` |
+00002980: 2074 6578 7420 3c2d 3e20 6f72 6469 6e61   text <-> ordina
+00002990: 6c20 6469 6769 7473 207c 2064 756d 6d79  l digits | dummy
+000029a0: 2063 6861 7261 6374 6572 206f 7264 696e   character ordin
+000029b0: 616c 7320 636f 6e76 6572 7369 6f6e 2028  als conversion (
+000029c0: 636f 6e76 6572 7473 2074 6f20 332d 6469  converts to 3-di
+000029d0: 6769 7473 2067 726f 7570 7329 0d0a 6070  gits groups)..`p
+000029e0: 6b7a 6970 5f64 6566 6c61 7465 6020 7c20  kzip_deflate` | 
+000029f0: 7465 7874 203c 2d3e 2064 6566 6c61 7465  text <-> deflate
+00002a00: 6420 7465 7874 207c 2073 7461 6e64 6172  d text | standar
+00002a10: 6420 5a69 702d 6465 666c 6174 6520 636f  d Zip-deflate co
+00002a20: 6d70 7265 7373 696f 6e2f 6465 636f 6d70  mpression/decomp
+00002a30: 7265 7373 696f 6e0d 0a60 706b 7a69 705f  ression..`pkzip_
+00002a40: 627a 6970 3260 207c 2074 6578 7420 3c2d  bzip2` | text <-
+00002a50: 3e20 427a 6970 7065 6420 7465 7874 207c  > Bzipped text |
+00002a60: 2073 7461 6e64 6172 6420 425a 6970 3220   standard BZip2 
+00002a70: 636f 6d70 7265 7373 696f 6e2f 6465 636f  compression/deco
+00002a80: 6d70 7265 7373 696f 6e0d 0a60 706b 7a69  mpression..`pkzi
+00002a90: 705f 6c7a 6d61 6020 7c20 7465 7874 203c  p_lzma` | text <
+00002aa0: 2d3e 204c 5a4d 412d 636f 6d70 7265 7373  -> LZMA-compress
+00002ab0: 6564 2074 6578 7420 7c20 7374 616e 6461  ed text | standa
+00002ac0: 7264 204c 5a4d 4120 636f 6d70 7265 7373  rd LZMA compress
+00002ad0: 696f 6e2f 6465 636f 6d70 7265 7373 696f  ion/decompressio
+00002ae0: 6e0d 0a60 7261 6469 6f60 207c 2074 6578  n..`radio` | tex
+00002af0: 7420 3c2d 3e20 7261 6469 6f20 776f 7264  t <-> radio word
+00002b00: 7320 7c20 616b 6120 4e41 544f 206f 7220  s | aka NATO or 
+00002b10: 7261 6469 6f20 7068 6f6e 6574 6963 2061  radio phonetic a
+00002b20: 6c70 6861 6265 740d 0a60 7265 7369 7374  lphabet..`resist
+00002b30: 6f72 6020 7c20 7465 7874 203c 2d3e 2072  or` | text <-> r
+00002b40: 6573 6973 746f 7220 636f 6c6f 7273 207c  esistor colors |
+00002b50: 2061 6b61 2072 6573 6973 746f 7220 636f   aka resistor co
+00002b60: 6c6f 7220 636f 6465 730d 0a60 726f 7460  lor codes..`rot`
+00002b70: 207c 2074 6578 7420 3c2d 3e20 726f 7428   | text <-> rot(
+00002b80: 4e29 2063 6970 6865 7274 6578 7420 7c20  N) ciphertext | 
+00002b90: 616b 6120 4361 6573 6172 2063 6970 6865  aka Caesar ciphe
+00002ba0: 7220 284e 2062 656c 6f6e 6773 2074 6f20  r (N belongs to 
+00002bb0: 5b31 2c32 355d 290d 0a60 726f 7461 7465  [1,25])..`rotate
+00002bc0: 6020 7c20 7465 7874 203c 2d3e 204e 2d62  ` | text <-> N-b
+00002bd0: 6974 732d 726f 7461 7465 6420 7465 7874  its-rotated text
+00002be0: 207c 2072 6f74 6174 6573 2063 6861 7261   | rotates chara
+00002bf0: 6374 6572 7320 6279 2074 6865 2073 7065  cters by the spe
+00002c00: 6369 6669 6564 206e 756d 6265 7220 6f66  cified number of
+00002c10: 2062 6974 7320 3b20 5079 7468 6f6e 2033   bits ; Python 3
+00002c20: 206f 6e6c 790d 0a60 7363 7974 616c 6560   only..`scytale`
+00002c30: 207c 2074 6578 7420 3c2d 3e20 7363 7974   | text <-> scyt
+00002c40: 616c 6520 6369 7068 6572 7465 7874 207c  ale ciphertext |
+00002c50: 2065 6e63 7279 7074 7320 7769 7468 204c   encrypts with L
+00002c60: 2c20 7468 6520 6e75 6d62 6572 206f 6620  , the number of 
+00002c70: 6c65 7474 6572 7320 6f6e 2074 6865 2072  letters on the r
+00002c80: 6f64 2028 6265 6c6f 6e67 7320 746f 205b  od (belongs to [
+00002c90: 312c 5b29 0d0a 6073 6869 6674 6020 7c20  1,[)..`shift` | 
+00002ca0: 7465 7874 203c 2d3e 2073 6869 6674 284e  text <-> shift(N
+00002cb0: 2920 6369 7068 6572 7465 7874 207c 2073  ) ciphertext | s
+00002cc0: 6869 6674 206f 7264 696e 616c 7320 7769  hift ordinals wi
+00002cd0: 7468 204e 2028 6265 6c6f 6e67 7320 746f  th N (belongs to
+00002ce0: 205b 312c 3235 355d 290d 0a60 736d 7360   [1,255])..`sms`
+00002cf0: 207c 2074 6578 7420 3c2d 3e20 7068 6f6e   | text <-> phon
+00002d00: 6520 6b65 7973 7472 6f6b 6573 207c 2061  e keystrokes | a
+00002d10: 6c73 6f20 6361 6c6c 6564 2054 3920 636f  lso called T9 co
+00002d20: 6465 203b 2075 7365 7320 2260 2d60 2220  de ; uses "`-`" 
+00002d30: 6173 2061 2073 6570 6172 6174 6f72 2066  as a separator f
+00002d40: 6f72 2065 6e63 6f64 696e 672c 2022 602d  or encoding, "`-
+00002d50: 6022 206f 7220 2260 5f60 2220 6f72 2077  `" or "`_`" or w
+00002d60: 6869 7465 7370 6163 6520 666f 7220 6465  hitespace for de
+00002d70: 636f 6469 6e67 0d0a 6073 6f75 7468 7061  coding..`southpa
+00002d80: 726b 6020 7c20 7465 7874 203c 2d3e 204b  rk` | text <-> K
+00002d90: 656e 6e79 2773 206c 616e 6775 6167 6520  enny's language 
+00002da0: 7c20 636f 6e76 6572 7473 206c 6574 7465  | converts lette
+00002db0: 7273 2074 6f20 4b65 6e6e 7927 7320 6c61  rs to Kenny's la
+00002dc0: 6e67 7561 6765 2066 726f 6d20 536f 7574  nguage from Sout
+00002dd0: 6870 6172 6b20 2877 6869 7465 7370 6163  hpark (whitespac
+00002de0: 6520 6973 2061 6c73 6f20 6861 6e64 6c65  e is also handle
+00002df0: 6429 0d0a 6074 6f6d 746f 6d60 207c 2074  d)..`tomtom` | t
+00002e00: 6578 7420 3c2d 3e20 746f 6d2d 746f 6d20  ext <-> tom-tom 
+00002e10: 656e 636f 6465 6420 7465 7874 207c 2073  encoded text | s
+00002e20: 696d 696c 6172 2074 6f20 606d 6f72 7365  imilar to `morse
+00002e30: 602c 2075 7369 6e67 2073 6c61 7368 6573  `, using slashes
+00002e40: 2061 6e64 2062 6163 6b73 6c61 7368 6573   and backslashes
+00002e50: 0d0a 6075 726c 6020 7c20 7465 7874 203c  ..`url` | text <
+00002e60: 2d3e 2055 524c 2065 6e63 6f64 6564 2074  -> URL encoded t
+00002e70: 6578 7420 7c20 616b 6120 5552 4c20 656e  ext | aka URL en
+00002e80: 636f 6469 6e67 0d0a 6078 6f72 6020 7c20  coding..`xor` | 
+00002e90: 7465 7874 203c 2d3e 2058 4f52 284e 2920  text <-> XOR(N) 
+00002ea0: 6369 7068 6572 7465 7874 207c 2058 4f52  ciphertext | XOR
+00002eb0: 2077 6974 6820 6120 7369 6e67 6c65 2062   with a single b
+00002ec0: 7974 6520 284e 2062 656c 6f6e 6773 2074  yte (N belongs t
+00002ed0: 6f20 5b31 2c32 3535 5d29 0d0a 6077 6869  o [1,255])..`whi
+00002ee0: 7465 7370 6163 6560 207c 2074 6578 7420  tespace` | text 
+00002ef0: 3c2d 3e20 7768 6974 6573 7061 6365 7320  <-> whitespaces 
+00002f00: 616e 6420 7461 6273 207c 2072 6570 6c61  and tabs | repla
+00002f10: 6365 7320 6269 7473 2077 6974 6820 7768  ces bits with wh
+00002f20: 6974 6573 7061 6365 7320 616e 6420 7461  itespaces and ta
+00002f30: 6273 0d0a 0d0a 4120 6665 7720 7661 7269  bs....A few vari
+00002f40: 616e 7473 2061 7265 2061 6c73 6f20 696d  ants are also im
+00002f50: 706c 656d 656e 7465 642e 0d0a 0d0a 2a2a  plemented.....**
+00002f60: 436f 6465 632a 2a20 7c20 2a2a 436f 6e76  Codec** | **Conv
+00002f70: 6572 7369 6f6e 732a 2a20 7c20 2a2a 436f  ersions** | **Co
+00002f80: 6d6d 656e 742a 2a0d 0a3a 2d2d 2d3a 207c  mment**..:---: |
+00002f90: 203a 2d2d 2d3a 207c 202d 2d2d 0d0a 6062   :---: | ---..`b
+00002fa0: 6175 646f 742d 7370 6163 6564 6020 7c20  audot-spaced` | 
+00002fb0: 7465 7874 203c 2d3e 2042 6175 646f 7420  text <-> Baudot 
+00002fc0: 636f 6465 2067 726f 7570 7320 6f66 2062  code groups of b
+00002fd0: 6974 7320 7c20 6772 6f75 7073 206f 6620  its | groups of 
+00002fe0: 3520 6269 7473 2061 7265 2077 6869 7465  5 bits are white
+00002ff0: 7370 6163 652d 7365 7061 7261 7465 640d  space-separated.
+00003000: 0a60 6261 7564 6f74 2d74 6170 6560 207c  .`baudot-tape` |
+00003010: 2074 6578 7420 3c2d 3e20 4261 7564 6f74   text <-> Baudot
+00003020: 2063 6f64 6520 7461 7065 207c 206f 7574   code tape | out
+00003030: 7075 7473 2061 2073 7472 696e 6720 7468  puts a string th
+00003040: 6174 206c 6f6f 6b73 206c 696b 6520 6120  at looks like a 
+00003050: 7065 7266 6f72 6174 6564 2074 6170 650d  perforated tape.
+00003060: 0a60 6263 642d 6578 7465 6e64 6564 3060  .`bcd-extended0`
+00003070: 207c 2074 6578 7420 3c2d 3e20 4243 442d   | text <-> BCD-
+00003080: 6578 7465 6e64 6564 2074 6578 7420 7c20  extended text | 
+00003090: 656e 636f 6465 7320 6368 6172 6163 7465  encodes characte
+000030a0: 7273 2066 726f 6d20 7468 6569 7220 287a  rs from their (z
+000030b0: 6572 6f2d 6c65 6674 2d70 6164 6465 6429  ero-left-padded)
+000030c0: 206f 7264 696e 616c 7320 7573 696e 6720   ordinals using 
+000030d0: 7072 6566 6978 2062 6974 7320 6030 3030  prefix bits `000
+000030e0: 3060 0d0a 6062 6364 2d65 7874 656e 6465  0`..`bcd-extende
+000030f0: 6431 6020 7c20 7465 7874 203c 2d3e 2042  d1` | text <-> B
+00003100: 4344 2d65 7874 656e 6465 6420 7465 7874  CD-extended text
+00003110: 207c 2065 6e63 6f64 6573 2063 6861 7261   | encodes chara
+00003120: 6374 6572 7320 6672 6f6d 2074 6865 6972  cters from their
+00003130: 2028 7a65 726f 2d6c 6566 742d 7061 6464   (zero-left-padd
+00003140: 6564 2920 6f72 6469 6e61 6c73 2075 7369  ed) ordinals usi
+00003150: 6e67 2070 7265 6669 7820 6269 7473 2060  ng prefix bits `
+00003160: 3131 3131 600d 0a60 6d61 6e63 6865 7374  1111`..`manchest
+00003170: 6572 2d69 6e76 6572 7465 6460 207c 2074  er-inverted` | t
+00003180: 6578 7420 3c2d 3e20 6d61 6e63 6865 7374  ext <-> manchest
+00003190: 6572 2065 6e63 6f64 6564 2074 6578 7420  er encoded text 
+000031a0: 7c20 584f 5265 7320 6561 6368 2062 6974  | XORes each bit
+000031b0: 206f 6620 7468 6520 696e 7075 7420 7769   of the input wi
+000031c0: 7468 2060 3130 600d 0a60 6f63 7461 6c2d  th `10`..`octal-
+000031d0: 7370 6163 6564 6020 7c20 7465 7874 203c  spaced` | text <
+000031e0: 2d3e 206f 6374 616c 2064 6967 6974 7320  -> octal digits 
+000031f0: 2877 6869 7465 7370 6163 652d 7365 7061  (whitespace-sepa
+00003200: 7261 7465 6429 207c 2064 756d 6d79 206f  rated) | dummy o
+00003210: 6374 616c 2063 6f6e 7665 7273 696f 6e0d  ctal conversion.
+00003220: 0a60 6f72 6469 6e61 6c2d 7370 6163 6564  .`ordinal-spaced
+00003230: 6020 7c20 7465 7874 203c 2d3e 206f 7264  ` | text <-> ord
+00003240: 696e 616c 2064 6967 6974 7320 2877 6869  inal digits (whi
+00003250: 7465 7370 6163 652d 7365 7061 7261 7465  tespace-separate
+00003260: 6429 207c 2064 756d 6d79 2063 6861 7261  d) | dummy chara
+00003270: 6374 6572 206f 7264 696e 616c 7320 636f  cter ordinals co
+00003280: 6e76 6572 7369 6f6e 0d0a 6073 6f75 7468  nversion..`south
+00003290: 7061 726b 2d69 6361 7365 6020 7c20 7465  park-icase` | te
+000032a0: 7874 203c 2d3e 204b 656e 6e79 2773 206c  xt <-> Kenny's l
+000032b0: 616e 6775 6167 6520 7c20 7361 6d65 2061  anguage | same a
+000032c0: 7320 6073 6f75 7468 7061 726b 6020 6275  s `southpark` bu
+000032d0: 7420 6361 7365 2069 6e73 656e 7369 7469  t case insensiti
+000032e0: 7665 0d0a 6077 6869 7465 7370 6163 655f  ve..`whitespace_
+000032f0: 6166 7465 725f 6265 666f 7265 6020 7c20  after_before` | 
+00003300: 7465 7874 203c 2d3e 206c 696e 6573 206f  text <-> lines o
+00003310: 6620 7768 6974 6573 7061 6365 735b 6c65  f whitespaces[le
+00003320: 7474 6572 5d77 6869 7465 7370 6163 6573  tter]whitespaces
+00003330: 207c 2065 6e63 6f64 6573 2063 6861 7261   | encodes chara
+00003340: 6374 6572 7320 6173 206e 6577 2063 6861  cters as new cha
+00003350: 7261 6374 6572 7320 7769 7468 2077 6869  racters with whi
+00003360: 7465 7370 6163 6573 2062 6566 6f72 6520  tespaces before 
+00003370: 616e 6420 6166 7465 7220 6163 636f 7264  and after accord
+00003380: 696e 6720 746f 2061 6e20 6571 7561 7469  ing to an equati
+00003390: 6f6e 2064 6573 6372 6962 6564 2069 6e20  on described in 
+000033a0: 7468 6520 636f 6465 6320 6e61 6d65 2028  the codec name (
+000033b0: 652e 672e 2022 6077 6869 7465 7370 6163  e.g. "`whitespac
+000033c0: 652b 322a 6166 7465 722d 332a 6265 666f  e+2*after-3*befo
+000033d0: 7265 6022 290d 0a0d 0a0d 0a23 2320 3a63  re`")......## :c
+000033e0: 6c61 703a 2020 5375 7070 6f72 7465 7273  lap:  Supporters
+000033f0: 0d0a 0d0a 5b21 5b53 7461 7267 617a 6572  ....[![Stargazer
+00003400: 7320 7265 706f 2072 6f73 7465 7220 666f  s repo roster fo
+00003410: 7220 4064 686f 6e64 7461 2f70 7974 686f  r @dhondta/pytho
+00003420: 6e2d 636f 6465 7874 5d28 6874 7470 733a  n-codext](https:
+00003430: 2f2f 7265 706f 726f 7374 6572 2e63 6f6d  //reporoster.com
+00003440: 2f73 7461 7273 2f64 6172 6b2f 6468 6f6e  /stars/dark/dhon
+00003450: 6474 612f 7079 7468 6f6e 2d63 6f64 6578  dta/python-codex
+00003460: 7429 5d28 6874 7470 733a 2f2f 6769 7468  t)](https://gith
+00003470: 7562 2e63 6f6d 2f64 686f 6e64 7461 2f70  ub.com/dhondta/p
+00003480: 7974 686f 6e2d 636f 6465 7874 2f73 7461  ython-codext/sta
+00003490: 7267 617a 6572 7329 0d0a 0d0a 5b21 5b46  rgazers)....[![F
+000034a0: 6f72 6b65 7273 2072 6570 6f20 726f 7374  orkers repo rost
+000034b0: 6572 2066 6f72 2040 6468 6f6e 6474 612f  er for @dhondta/
+000034c0: 7079 7468 6f6e 2d63 6f64 6578 745d 2868  python-codext](h
+000034d0: 7474 7073 3a2f 2f72 6570 6f72 6f73 7465  ttps://reporoste
+000034e0: 722e 636f 6d2f 666f 726b 732f 6461 726b  r.com/forks/dark
+000034f0: 2f64 686f 6e64 7461 2f70 7974 686f 6e2d  /dhondta/python-
+00003500: 636f 6465 7874 295d 2868 7474 7073 3a2f  codext)](https:/
+00003510: 2f67 6974 6875 622e 636f 6d2f 6468 6f6e  /github.com/dhon
+00003520: 6474 612f 7079 7468 6f6e 2d63 6f64 6578  dta/python-codex
+00003530: 742f 6e65 7477 6f72 6b2f 6d65 6d62 6572  t/network/member
+00003540: 7329 0d0a 0d0a 3c70 2061 6c69 676e 3d22  s)....<p align="
+00003550: 6365 6e74 6572 223e 3c61 2068 7265 663d  center"><a href=
+00003560: 2223 223e 3c69 6d67 2073 7263 3d22 6874  "#"><img src="ht
+00003570: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00003580: 732e 696f 2f62 6164 6765 2f42 6163 6b25  s.io/badge/Back%
+00003590: 3230 746f 2532 3074 6f70 2d2d 6c69 6768  20to%20top--ligh
+000035a0: 7467 7265 793f 7374 796c 653d 736f 6369  tgrey?style=soci
+000035b0: 616c 2220 616c 743d 2242 6163 6b20 746f  al" alt="Back to
+000035c0: 2074 6f70 2220 6865 6967 6874 3d22 3230   top" height="20
+000035d0: 222f 3e3c 2f61 3e3c 2f70 3e0d 0a         "/></a></p>..
```

### Comparing `codext-1.9.4/codext/__common__.py` & `codext-1.9.5/codext/__common__.py`

 * *Files 1% similar despite different names*

```diff
@@ -469,15 +469,19 @@
                 temp = []
                 for s in generate_strings_from_regex(search_function.__pattern__, yield_max=16*number):
                     temp.append(s)
                 random.shuffle(temp)
                 i = 0
                 while i < min(number, len(temp)):
                     if not temp[i].isdigit():
-                        e.append(temp[i])
+                        try:
+                            lookup(temp[i])
+                            e.append(temp[i])
+                        except LookupError:
+                            pass
                     i += 1
         for alias, codec in aliases.items():
             if name == codec:
                 if codec not in e:
                     e.append(codec)
                 if not alias.isdigit():
                     e.append(alias)
@@ -690,15 +694,22 @@
     """ Custom decode function relying on the hooked lookup function. """
     return lookup(encoding).decode(obj, errors)[0]
 codecs.decode = decode
 
 
 def encode(obj, encoding='utf-8', errors='strict'):
     """ Custom encode function relying on the hooked lookup function. """
-    return lookup(encoding).encode(obj, errors)[0]
+    n, m = 1, re.search(r"\[(\d+)\]$", encoding)
+    if m:
+        n = int(m.group(1))
+        encoding = re.sub(r"\[(\d+)\]$", "", encoding)
+    ci = lookup(encoding)
+    for i in range(n):
+        obj = ci.encode(obj, errors)[0]
+    return obj
 codecs.encode = encode
 
 
 def lookup(encoding):
     """ Hooked lookup function for searching first for codecs in the local registry of this module. """
     # first, try to match the given encoding with codecs' search functions
     for search_function in __codecs_registry:
```

### Comparing `codext-1.9.4/codext/__init__.py` & `codext-1.9.5/codext/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from ast import literal_eval
 from six import binary_type, text_type
 
 from .__common__ import *
 from .__info__ import __author__, __copyright__, __email__, __license__, __source__, __version__
 
 
-__all__ = ["add", "add_map", "clear", "decode", "encode", "guess", "lookup",  "open", "register", "remove", "reset"]
+__all__ = ["add", "add_map", "clear", "decode", "encode", "guess", "lookup",  "open", "rank", "register", "remove",
+           "reset"]
 
 decode   = codecs.decode
 encode   = codecs.encode
 guess    = codecs.guess
 lookup   = codecs.lookup
 open     = codecs.open
```

### Comparing `codext-1.9.4/codext/base/__init__.py` & `codext-1.9.5/codext/base/__init__.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/base/_base.py` & `codext-1.9.5/codext/base/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,16 @@
     """ Base-N codec factory.
     
     :param charset: charset selection function
     :param pattern: matching pattern for the codec name (first capturing group is used as the parameter for selecting
                      the charset)
     :param pow2:    whether the base codec's N is a power of 2
     """
-    n = len(_get_charset(charset))
+    cs = _get_charset(charset)
+    n = len(cs)
     nb = log(n, 2)
     if pow2 and nb != int(nb):
         raise BaseError("Bad charset ; {} is not a power of 2".format(n))
     
     def encode(param=""):
         a = _get_charset(charset, param)
         def _encode(input, errors="strict"):
@@ -138,15 +139,15 @@
         sl, sc = "\n" not in a, "\n" not in a and not "\r" in a
         def _decode(input, errors="strict"):
             input = _stripl(input, sc, sl)
             return decode_template(input, a, errors), len(input)
         return _decode
     
     kwargs['len_charset'] = n
-    kwargs['printables_rate'] = 1.
+    kwargs['printables_rate'] = float(len([c for c in cs if c in printable])) / len(cs)
     n = "base{}".format(n) if name is None else name
     kwargs['guess'] = kwargs.get('guess', [n])
     add(n, encode, decode, pattern, entropy=nb, **kwargs)
 
 
 def base_generic():
     """ Base-N generic codec. """
```

### Comparing `codext-1.9.4/codext/base/_base2n.py` & `codext-1.9.5/codext/base/_base2n.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/base/ascii85.py` & `codext-1.9.5/codext/base/ascii85.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/base/base100.py` & `codext-1.9.5/codext/base/base100.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/base/base122.py` & `codext-1.9.5/codext/base/base122.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/base/base45.py` & `codext-1.9.5/codext/base/base45.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/base/base85.py` & `codext-1.9.5/codext/base/base85.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/base/base91.py` & `codext-1.9.5/codext/base/base91.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/base/baseN.py` & `codext-1.9.5/codext/base/baseN.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 """
 from ..__common__ import *
 from ._base import base, base_generic, digits, lower, main, upper
 from ._base2n import base2n
 
 
 B2 = {r'': "01", r'[-_]inv(erted)?': "10"}
-base2n(B2, r"^(?:base[-_]?2|bin)(|[-_]inv(?:erted)?|[-_][a-zA-Z0-9]{2})$")
+base2n(B2, r"^(?:base[-_]?2|bin)(|[-_]inv(?:erted)?|[-_](?!.*(.).*\2)[a-zA-Z0-9]{2})$")
 main2 = main(2)
 
 
 B3 = {r'': "123", r'[-_]inv(erted)?': "321"}
-base(B3, r"^base[-_]?3(|[-_]inv(?:erted)?|[-_][a-zA-Z0-9]{3})$")
+base(B3, r"^base[-_]?3(|[-_]inv(?:erted)?|[-_](?!.*(.).*\2)[a-zA-Z0-9]{3})$")
 main3 = main(3)
 
 
 B4 = {r'': "1234", r'[-_]inv(erted)?': "4321"}
-base2n(B4, r"^base[-_]?4(|[-_]inv(?:erted)?|[-_][a-zA-Z0-9]{4})$")
+base2n(B4, r"^base[-_]?4(|[-_]inv(?:erted)?|[-_](?!.*(.).*\2)[a-zA-Z0-9]{4})$")
 main4 = main(4)
 
 
 B8 = {r'': "abcdefgh", r'[-_]inv(erted)?': "hgfedcba"}
-base2n(B8, r"^base[-_]?8(|[-_]inv(?:erted)?|[-_][a-zA-Z0-9]{8})$")
+base2n(B8, r"^base[-_]?8(|[-_]inv(?:erted)?|[-_](?!.*(.).*\2)[a-zA-Z0-9]{8})$")
 main8 = main(8)
 
 
 B16 = {'': digits + "ABCDEF", 'inv': "ABCDEF" + digits}
 base2n(B16, r"^(?:base[-_]?16|hex)(|[-_]inv(?:erted)?)$")
 main16 = main(16, "RFC 4648")
```

### Comparing `codext-1.9.4/codext/binary/baudot.py` & `codext-1.9.5/codext/binary/baudot.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/binary/bcd.py` & `codext-1.9.5/codext/binary/bcd.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/binary/excess3.py` & `codext-1.9.5/codext/binary/excess3.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,10 +57,9 @@
                     d += handle_error("excess3", errors, decode=True)(hb, i)
             if len(d) == 3:
                 r += chr(int(d))
                 d = ""
     return r, len(b(text))
 
 
-add("excess3", excess3_encode, excess3_decode, pattern=r"^(?:excess\-?3|xs\-?3|stibitz)$", entropy=1.,
-    printables_rate=.45)
+add("excess3", excess3_encode, excess3_decode, pattern=r"^(?:excess\-?3|xs\-?3|stibitz)$", printables_rate=.45)
```

### Comparing `codext-1.9.4/codext/binary/gray.py` & `codext-1.9.5/codext/binary/gray.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/binary/manchester.py` & `codext-1.9.5/codext/binary/manchester.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/binary/rotate.py` & `codext-1.9.5/codext/binary/rotate.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,9 +43,9 @@
 
     def rotate_decode(i):
         def decode(text, errors="strict"):
             return _rotaten(text, -_getn(i)), len(text)
         return decode
 
 
-    add("rotate", rotate_encode, rotate_decode, r"rotate(?:[-_]?bits)?[-_]?((?:(?:left|right)[-_]?)?[1-7])$", entropy=1.)
+    add("rotate", rotate_encode, rotate_decode, r"rotate(?:[-_]?bits)?[-_]?((?:(?:left|right)[-_]?)?[1-7])$")
```

### Comparing `codext-1.9.4/codext/common/a1z26.py` & `codext-1.9.5/codext/common/a1z26.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/common/dummy.py` & `codext-1.9.5/codext/common/dummy.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/common/octal.py` & `codext-1.9.5/codext/common/octal.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/common/ordinal.py` & `codext-1.9.5/codext/common/ordinal.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/compressions/gzipp.py` & `codext-1.9.5/codext/compressions/gzipp.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/compressions/lz77.py` & `codext-1.9.5/codext/compressions/lz77.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/compressions/lz78.py` & `codext-1.9.5/codext/compressions/lz78.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/compressions/pkzip.py` & `codext-1.9.5/codext/compressions/pkzip.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,26 +17,33 @@
 _str          = ["test", "This is a test", "@random{512,1024,2048}"]
 __examples1__ = {'enc-dec(pkzip-deflate|deflate)': _str}
 __examples2__ = {'enc-dec(pkzip_bz2|bzip2)':       _str}
 __examples3__ = {'enc-dec(pkzip-lzma|lzma)':       _str}
 
 
 if PY3:
+    NULL = {
+        8:  b"\x03\x00",
+        12: b"BZh9\x17rE8P\x90\x00\x00\x00\x00",
+        14: b"\t\x04\x05\x00]\x00\x00\x80\x00\x00\x83\xff\xfb\xff\xff\xc0\x00\x00\x00",
+    }    
+        
+    
     def pkzip_encode(compression_type):
         def _encode(text, errors="strict"):
             c = zipfile._get_compressor(compression_type)
             return c.compress(b(text)) + c.flush(), len(text)
         return _encode
 
 
     def pkzip_decode(compression_type, name):
         def _decode(data, errors="strict"):
             d = zipfile._get_decompressor(compression_type)
             r = d.decompress(b(data))
-            if len(r) == 0:
+            if len(r) == 0 and b(data) != NULL[compression_type]:
                 return handle_error(name, errors, decode=True)(data[0], 0) if len(data) > 0 else "", len(data)
             return r, len(r)
         return _decode
 
 
     add("pkzip_deflate", pkzip_encode(8), pkzip_decode(8, "deflate"), r"(?:(?:pk)?zip[-_])?deflate",
         entropy=7.9, examples=__examples1__, guess=["deflate"])
```

### Comparing `codext-1.9.4/codext/crypto/affine.py` & `codext-1.9.5/codext/crypto/affine.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/crypto/atbash.py` & `codext-1.9.5/codext/crypto/atbash.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/crypto/bacon.py` & `codext-1.9.5/codext/crypto/bacon.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/crypto/barbie.py` & `codext-1.9.5/codext/crypto/barbie.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/crypto/citrix.py` & `codext-1.9.5/codext/crypto/citrix.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/crypto/rot.py` & `codext-1.9.5/codext/crypto/rot.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/crypto/scytale.py` & `codext-1.9.5/codext/crypto/scytale.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/crypto/shift.py` & `codext-1.9.5/codext/crypto/shift.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/crypto/xor.py` & `codext-1.9.5/codext/crypto/xor.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/languages/braille.py` & `codext-1.9.5/codext/languages/braille.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/languages/ipsum.py` & `codext-1.9.5/codext/languages/ipsum.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/languages/leetspeak.py` & `codext-1.9.5/codext/languages/leetspeak.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/languages/morse.py` & `codext-1.9.5/codext/languages/morse.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/languages/navajo.py` & `codext-1.9.5/codext/languages/navajo.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/languages/radio.py` & `codext-1.9.5/codext/languages/radio.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/languages/southpark.py` & `codext-1.9.5/codext/languages/southpark.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/languages/tomtom.py` & `codext-1.9.5/codext/languages/tomtom.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/others/dna.py` & `codext-1.9.5/codext/others/dna.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/others/html.py` & `codext-1.9.5/codext/others/html.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/others/letters.py` & `codext-1.9.5/codext/others/letters.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/others/markdown.py` & `codext-1.9.5/codext/others/markdown.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/others/url.py` & `codext-1.9.5/codext/others/url.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/stegano/klopf.py` & `codext-1.9.5/codext/stegano/klopf.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/stegano/resistor.py` & `codext-1.9.5/codext/stegano/resistor.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/stegano/sms.py` & `codext-1.9.5/codext/stegano/sms.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext/stegano/whitespace.py` & `codext-1.9.5/codext/stegano/whitespace.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext.egg-info/PKG-INFO` & `codext-1.9.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 636f 6465  : 2.1.Name: code
 00000020: 7874 0a56 6572 7369 6f6e 3a20 312e 392e  xt.Version: 1.9.
-00000030: 340a 5375 6d6d 6172 793a 204e 6174 6976  4.Summary: Nativ
+00000030: 350a 5375 6d6d 6172 793a 204e 6174 6976  5.Summary: Nativ
 00000040: 6520 636f 6465 6373 2065 7874 656e 7369  e codecs extensi
 00000050: 6f6e 0a48 6f6d 652d 7061 6765 3a20 6874  on.Home-page: ht
 00000060: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00000070: 2f64 686f 6e64 7461 2f70 7974 686f 6e2d  /dhondta/python-
 00000080: 636f 6465 7874 0a41 7574 686f 723a 2041  codext.Author: A
 00000090: 6c65 7861 6e64 7265 2044 2748 6f6e 6474  lexandre D'Hondt
 000000a0: 0a41 7574 686f 722d 656d 6169 6c3a 2061  .Author-email: a
@@ -60,691 +60,854 @@
 000003b0: 2e30 2e2a 2c21 3d33 2e31 2e2a 2c21 3d33  .0.*,!=3.1.*,!=3
 000003c0: 2e32 2e2a 2c21 3d33 2e33 2e2a 2c21 3d33  .2.*,!=3.3.*,!=3
 000003d0: 2e34 2e2a 2c21 3d33 2e35 2e2a 2c3c 342c  .4.*,!=3.5.*,<4,
 000003e0: 3e3d 322e 370a 4465 7363 7269 7074 696f  >=2.7.Descriptio
 000003f0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
 00000400: 7465 7874 2f6d 6172 6b64 6f77 6e0a 4c69  text/markdown.Li
 00000410: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
-00000420: 4e53 450a 0a5b 215b 5079 5069 5d28 6874  NSE..[![PyPi](ht
-00000430: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000440: 732e 696f 2f70 7970 692f 762f 636f 6465  s.io/pypi/v/code
-00000450: 7874 2e73 7667 295d 2868 7474 7073 3a2f  xt.svg)](https:/
-00000460: 2f70 7970 692e 7079 7468 6f6e 2e6f 7267  /pypi.python.org
-00000470: 2f70 7970 692f 636f 6465 7874 2f29 0a5b  /pypi/codext/).[
-00000480: 215b 5265 6164 2054 6865 2044 6f63 735d  ![Read The Docs]
-00000490: 2868 7474 7073 3a2f 2f72 6561 6474 6865  (https://readthe
-000004a0: 646f 6373 2e6f 7267 2f70 726f 6a65 6374  docs.org/project
-000004b0: 732f 7079 7468 6f6e 2d63 6f64 6578 742f  s/python-codext/
-000004c0: 6261 6467 652f 3f76 6572 7369 6f6e 3d6c  badge/?version=l
-000004d0: 6174 6573 7429 5d28 6874 7470 733a 2f2f  atest)](https://
-000004e0: 7079 7468 6f6e 2d63 6f64 6578 742e 7265  python-codext.re
-000004f0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00000500: 6c61 7465 7374 2f3f 6261 6467 653d 6c61  latest/?badge=la
-00000510: 7465 7374 290a 5b21 5b42 7569 6c64 2053  test).[![Build S
-00000520: 7461 7475 735d 2868 7474 7073 3a2f 2f74  tatus](https://t
-00000530: 7261 7669 732d 6369 2e63 6f6d 2f64 686f  ravis-ci.com/dho
-00000540: 6e64 7461 2f70 7974 686f 6e2d 636f 6465  ndta/python-code
-00000550: 7874 2e73 7667 3f62 7261 6e63 683d 6d61  xt.svg?branch=ma
-00000560: 7374 6572 295d 2868 7474 7073 3a2f 2f74  ster)](https://t
-00000570: 7261 7669 732d 6369 2e63 6f6d 2f64 686f  ravis-ci.com/dho
-00000580: 6e64 7461 2f70 7974 686f 6e2d 636f 6465  ndta/python-code
-00000590: 7874 290a 5b21 5b43 6f76 6572 6167 6520  xt).[![Coverage 
-000005a0: 5374 6174 7573 5d28 6874 7470 733a 2f2f  Status](https://
-000005b0: 636f 7665 7261 6c6c 732e 696f 2f72 6570  coveralls.io/rep
-000005c0: 6f73 2f67 6974 6875 622f 6468 6f6e 6474  os/github/dhondt
-000005d0: 612f 7079 7468 6f6e 2d63 6f64 6578 742f  a/python-codext/
-000005e0: 6261 6467 652e 7376 673f 6272 616e 6368  badge.svg?branch
-000005f0: 3d6d 6173 7465 7229 5d28 6874 7470 733a  =master)](https:
-00000600: 2f2f 636f 7665 7261 6c6c 732e 696f 2f67  //coveralls.io/g
-00000610: 6974 6875 622f 6468 6f6e 6474 612f 7079  ithub/dhondta/py
-00000620: 7468 6f6e 2d63 6f64 6578 743f 6272 616e  thon-codext?bran
-00000630: 6368 3d6d 6173 7465 7229 0a5b 215b 5079  ch=master).[![Py
-00000640: 7468 6f6e 2056 6572 7369 6f6e 735d 2868  thon Versions](h
-00000650: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000660: 6473 2e69 6f2f 7079 7069 2f70 7976 6572  ds.io/pypi/pyver
-00000670: 7369 6f6e 732f 636f 6465 7874 2e73 7667  sions/codext.svg
-00000680: 295d 2868 7474 7073 3a2f 2f70 7970 692e  )](https://pypi.
-00000690: 7079 7468 6f6e 2e6f 7267 2f70 7970 692f  python.org/pypi/
-000006a0: 636f 6465 7874 2f29 0a5b 215b 5265 7175  codext/).[![Requ
-000006b0: 6972 656d 656e 7473 2053 7461 7475 735d  irements Status]
-000006c0: 2868 7474 7073 3a2f 2f72 6571 7569 7265  (https://require
-000006d0: 732e 696f 2f67 6974 6875 622f 6468 6f6e  s.io/github/dhon
-000006e0: 6474 612f 7079 7468 6f6e 2d63 6f64 6578  dta/python-codex
-000006f0: 742f 7265 7175 6972 656d 656e 7473 2e73  t/requirements.s
-00000700: 7667 3f62 7261 6e63 683d 6d61 7374 6572  vg?branch=master
-00000710: 295d 2868 7474 7073 3a2f 2f72 6571 7569  )](https://requi
-00000720: 7265 732e 696f 2f67 6974 6875 622f 6468  res.io/github/dh
-00000730: 6f6e 6474 612f 7079 7468 6f6e 2d63 6f64  ondta/python-cod
-00000740: 6578 742f 7265 7175 6972 656d 656e 7473  ext/requirements
-00000750: 2f3f 6272 616e 6368 3d6d 6173 7465 7229  /?branch=master)
-00000760: 0a5b 215b 4b6e 6f77 6e20 5675 6c6e 6572  .[![Known Vulner
-00000770: 6162 696c 6974 6965 735d 2868 7474 7073  abilities](https
-00000780: 3a2f 2f73 6e79 6b2e 696f 2f74 6573 742f  ://snyk.io/test/
-00000790: 6769 7468 7562 2f64 686f 6e64 7461 2f70  github/dhondta/p
-000007a0: 7974 686f 6e2d 636f 6465 7874 2f62 6164  ython-codext/bad
-000007b0: 6765 2e73 7667 3f74 6172 6765 7446 696c  ge.svg?targetFil
-000007c0: 653d 7265 7175 6972 656d 656e 7473 2e74  e=requirements.t
-000007d0: 7874 295d 2868 7474 7073 3a2f 2f73 6e79  xt)](https://sny
-000007e0: 6b2e 696f 2f74 6573 742f 6769 7468 7562  k.io/test/github
-000007f0: 2f64 686f 6e64 7461 2f70 7974 686f 6e2d  /dhondta/python-
-00000800: 636f 6465 7874 3f74 6172 6765 7446 696c  codext?targetFil
-00000810: 653d 7265 7175 6972 656d 656e 7473 2e74  e=requirements.t
-00000820: 7874 290a 5b21 5b4c 6963 656e 7365 5d28  xt).[![License](
-00000830: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000840: 6c64 732e 696f 2f70 7970 692f 6c2f 636f  lds.io/pypi/l/co
-00000850: 6465 7874 2e73 7667 295d 2868 7474 7073  dext.svg)](https
-00000860: 3a2f 2f70 7970 692e 7079 7468 6f6e 2e6f  ://pypi.python.o
-00000870: 7267 2f70 7970 692f 636f 6465 7874 2f29  rg/pypi/codext/)
-00000880: 0a0a 2323 2049 6e74 726f 6475 6374 696f  ..## Introductio
-00000890: 6e0a 0a54 6869 7320 6c69 6272 6172 7920  n..This library 
-000008a0: 6578 7465 6e64 7320 7468 6520 6e61 7469  extends the nati
-000008b0: 7665 205b 6063 6f64 6563 7360 5d28 6874  ve [`codecs`](ht
-000008c0: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
-000008d0: 6e2e 6f72 672f 332f 6c69 6272 6172 792f  n.org/3/library/
-000008e0: 636f 6465 6373 2e68 746d 6c29 206c 6962  codecs.html) lib
-000008f0: 7261 7279 2028 6e61 6d65 6c79 2066 6f72  rary (namely for
-00000900: 2061 6464 696e 6720 6e65 7720 6375 7374   adding new cust
-00000910: 6f6d 2065 6e63 6f64 696e 6773 2061 6e64  om encodings and
-00000920: 2063 6861 7261 6374 6572 206d 6170 7069   character mappi
-00000930: 6e67 7329 2061 6e64 2070 726f 7669 6465  ngs) and provide
-00000940: 7320 6120 6d79 7269 6164 206f 6620 6e65  s a myriad of ne
-00000950: 7720 656e 636f 6469 6e67 7320 2873 7461  w encodings (sta
-00000960: 7469 6320 6f72 2070 6172 616d 6574 7269  tic or parametri
-00000970: 7a65 642c 206c 696b 6520 6072 6f74 6020  zed, like `rot` 
-00000980: 6f72 2060 786f 7260 292c 2068 656e 6365  or `xor`), hence
-00000990: 2069 7473 206e 616d 6564 2063 6f6d 6269   its named combi
-000009a0: 6e69 6e67 202a 434f 4465 6373 2045 5854  ning *CODecs EXT
-000009b0: 656e 7369 6f6e 2a2e 0a0a 0a0a 2323 2053  ension*.....## S
-000009c0: 6574 7570 0a0a 6060 6073 680a 2420 7069  etup..```sh.$ pi
-000009d0: 7020 696e 7374 616c 6c20 636f 6465 7874  p install codext
-000009e0: 0a60 6060 0a0a 2a2a 4e6f 7465 2a2a 3a20  .```..**Note**: 
-000009f0: 536f 6d65 2065 6e63 6f64 696e 6773 2061  Some encodings a
-00000a00: 7265 2061 7661 696c 6162 6c65 2069 6e20  re available in 
-00000a10: 5079 7468 6f6e 2033 206f 6e6c 792e 0a0a  Python 3 only...
-00000a20: 2323 2044 656d 6f6e 7374 7261 7469 6f6e  ## Demonstration
-00000a30: 730a 0a3c 7020 616c 6967 6e3d 2263 656e  s..<p align="cen
-00000a40: 7465 7222 3e3c 696d 6720 7372 633d 2268  ter"><img src="h
-00000a50: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-00000a60: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00000a70: 2f64 686f 6e64 7461 2f70 7974 686f 6e2d  /dhondta/python-
-00000a80: 636f 6465 7874 2f6d 6173 7465 722f 646f  codext/master/do
-00000a90: 6373 2f64 656d 6f73 2f75 7369 6e67 2d63  cs/demos/using-c
-00000aa0: 6f64 6578 742e 6769 6622 2061 6c74 3d22  odext.gif" alt="
-00000ab0: 5573 696e 6720 436f 6445 7874 2066 726f  Using CodExt fro
-00000ac0: 6d20 7468 6520 636f 6d6d 616e 6420 6c69  m the command li
-00000ad0: 6e65 223e 3c2f 703e 0a3c 7020 616c 6967  ne"></p>.<p alig
-00000ae0: 6e3d 2263 656e 7465 7222 3e3c 696d 6720  n="center"><img 
-00000af0: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
-00000b00: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00000b10: 6e74 2e63 6f6d 2f64 686f 6e64 7461 2f70  nt.com/dhondta/p
-00000b20: 7974 686f 6e2d 636f 6465 7874 2f6d 6173  ython-codext/mas
-00000b30: 7465 722f 646f 6373 2f64 656d 6f73 2f75  ter/docs/demos/u
-00000b40: 7369 6e67 2d62 6173 6573 2e67 6966 2220  sing-bases.gif" 
-00000b50: 616c 743d 2255 7369 6e67 2062 6173 6520  alt="Using base 
-00000b60: 746f 6f6c 7320 6672 6f6d 2074 6865 2063  tools from the c
-00000b70: 6f6d 6d61 6e64 206c 696e 6522 3e3c 2f70  ommand line"></p
-00000b80: 3e0a 3c70 2061 6c69 676e 3d22 6365 6e74  >.<p align="cent
-00000b90: 6572 223e 3c69 6d67 2073 7263 3d22 6874  er"><img src="ht
-00000ba0: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00000bb0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00000bc0: 6468 6f6e 6474 612f 7079 7468 6f6e 2d63  dhondta/python-c
-00000bd0: 6f64 6578 742f 6d61 7374 6572 2f64 6f63  odext/master/doc
-00000be0: 732f 6465 6d6f 732f 7573 696e 672d 6465  s/demos/using-de
-00000bf0: 6261 7365 2e67 6966 2220 616c 743d 2255  base.gif" alt="U
-00000c00: 7369 6e67 2074 6865 2064 6562 6173 6520  sing the debase 
-00000c10: 636f 6d6d 616e 6420 6c69 6e65 2074 6f6f  command line too
-00000c20: 6c22 3e3c 2f70 3e0a 0a23 2320 5573 6167  l"></p>..## Usag
-00000c30: 6520 2843 4c49 2074 6f6f 6c29 0a0a 6060  e (CLI tool)..``
-00000c40: 6073 680a 2420 636f 6465 7874 202d 6920  `sh.$ codext -i 
-00000c50: 7465 7374 2e74 7874 2065 6e63 6f64 6520  test.txt encode 
-00000c60: 646e 612d 310a 4754 4741 4743 4747 4754  dna-1.GTGAGCGGGT
-00000c70: 4154 4754 4741 0a24 2065 6368 6f20 2d65  ATGTGA.$ echo -e
-00000c80: 6e20 2274 6573 7422 207c 2063 6f64 6578  n "test" | codex
-00000c90: 7420 656e 636f 6465 206d 6f72 7365 0a2d  t encode morse.-
-00000ca0: 202e 202e 2e2e 202d 0a60 6060 0a0a 5079   . ... -.```..Py
-00000cb0: 7468 6f6e 2033 2028 696e 636c 7564 6573  thon 3 (includes
-00000cc0: 2041 7363 6969 3835 2c20 4261 7365 3835   Ascii85, Base85
-00000cd0: 2c20 4261 7365 3130 3020 616e 6420 6272  , Base100 and br
-00000ce0: 6169 6c6c 6529 3a0a 0a60 6060 7368 0a24  aille):..```sh.$
-00000cf0: 2065 6368 6f20 2d65 6e20 2274 6573 7422   echo -en "test"
-00000d00: 207c 2063 6f64 6578 7420 656e 636f 6465   | codext encode
-00000d10: 2062 7261 696c 6c65 0ae2 a09e e2a0 91e2   braille........
-00000d20: a08e e2a0 9e0a 2420 6563 686f 202d 656e  ......$ echo -en
-00000d30: 2022 7465 7374 2220 7c20 636f 6465 7874   "test" | codext
-00000d40: 2065 6e63 6f64 6520 6261 7365 3130 300a   encode base100.
-00000d50: f09f 91ab f09f 919c f09f 91aa f09f 91ab  ................
-00000d60: 0a60 6060 0a0a 5573 696e 6720 636f 6465  .```..Using code
-00000d70: 6373 2063 6861 696e 696e 673a 0a0a 6060  cs chaining:..``
-00000d80: 6073 680a 2420 6563 686f 202d 656e 2022  `sh.$ echo -en "
-00000d90: 5465 7374 2073 7472 696e 6722 207c 2063  Test string" | c
-00000da0: 6f64 6578 7420 656e 636f 6465 2072 6576  odext encode rev
-00000db0: 6572 7365 0a67 6e69 7274 7320 7473 6554  erse.gnirts tseT
-00000dc0: 0a24 2065 6368 6f20 2d65 6e20 2254 6573  .$ echo -en "Tes
-00000dd0: 7420 7374 7269 6e67 2220 7c20 636f 6465  t string" | code
-00000de0: 7874 2065 6e63 6f64 6520 7265 7665 7273  xt encode revers
-00000df0: 6520 6d6f 7273 650a 2d2d 2e20 2d2e 202e  e morse.--. -. .
-00000e00: 2e20 2e2d 2e20 2d20 2e2e 2e20 2f20 2d20  . .-. - ... / - 
-00000e10: 2e2e 2e20 2e20 2d0a 2420 6563 686f 202d  ... . -.$ echo -
-00000e20: 656e 2022 5465 7374 2073 7472 696e 6722  en "Test string"
-00000e30: 207c 2063 6f64 6578 7420 656e 636f 6465   | codext encode
-00000e40: 2072 6576 6572 7365 206d 6f72 7365 2064   reverse morse d
-00000e50: 6e61 2d32 0a41 4754 4341 4754 4341 4754  na-2.AGTCAGTCAGT
-00000e60: 4741 4741 4141 4754 4341 4754 4741 4741  GAGAAAGTCAGTGAGA
-00000e70: 4141 4754 4741 4754 4741 4741 4141 4754  AAGTGAGTGAGAAAGT
-00000e80: 4741 4754 4341 4754 4741 4741 4141 4754  GAGTCAGTGAGAAAGT
-00000e90: 4341 4741 4141 4754 4741 4754 4741 4754  CAGAAAGTGAGTGAGT
-00000ea0: 4741 4741 4141 4754 5441 4741 4141 4754  GAGAAAGTTAGAAAGT
-00000eb0: 4341 4741 4141 4754 4741 4754 4741 4754  CAGAAAGTGAGTGAGT
-00000ec0: 4741 4741 4141 4754 4741 4741 4141 4754  GAGAAAGTGAGAAAGT
-00000ed0: 430a 2420 6563 686f 202d 656e 2022 5465  C.$ echo -en "Te
-00000ee0: 7374 2073 7472 696e 6722 207c 2063 6f64  st string" | cod
-00000ef0: 6578 7420 656e 636f 6465 2072 6576 6572  ext encode rever
-00000f00: 7365 206d 6f72 7365 2064 6e61 2d32 206f  se morse dna-2 o
-00000f10: 6374 616c 0a31 3031 3130 3731 3234 3130  ctal.10110712410
-00000f20: 3331 3031 3130 3731 3234 3130 3331 3031  3101107124103101
-00000f30: 3130 3731 3234 3130 3731 3031 3130 3731  1071241071011071
-00000f40: 3031 3130 3131 3031 3130 3731 3234 3130  0110110110712410
-00000f50: 3331 3031 3130 3731 3234 3130 3731 3031  3101107124107101
-00000f60: 3130 3731 3031 3130 3131 3031 3130 3731  1071011011011071
-00000f70: 3234 3130 3731 3031 3130 3731 3234 3130  2410710110712410
-00000f80: 3731 3031 3130 3731 3031 3130 3131 3031  7101107101101101
-00000f90: 3130 3731 3234 3130 3731 3031 3130 3731  1071241071011071
-00000fa0: 3234 3130 3331 3031 3130 3731 3234 3130  2410310110712410
-00000fb0: 3731 3031 3130 3731 3031 3130 3131 3031  7101107101101101
-00000fc0: 3130 3731 3234 3130 3331 3031 3130 3731  1071241031011071
-00000fd0: 3031 3130 3131 3031 3130 3731 3234 3130  0110110110712410
-00000fe0: 3731 3031 3130 3731 3234 3130 3731 3031  7101107124107101
-00000ff0: 3130 3731 3234 3130 3731 3031 3130 3731  1071241071011071
-00001000: 3031 3130 3131 3031 3130 3731 3234 3132  0110110110712412
-00001010: 3431 3031 3130 3731 3031 3130 3131 3031  4101107101101101
-00001020: 3130 3731 3234 3130 3331 3031 3130 3731  1071241031011071
-00001030: 3031 3130 3131 3031 3130 3731 3234 3130  0110110110712410
-00001040: 3731 3031 3130 3731 3234 3130 3731 3031  7101107124107101
-00001050: 3130 3731 3234 3130 3731 3031 3130 3731  1071241071011071
-00001060: 3031 3130 3131 3031 3130 3731 3234 3130  0110110110712410
-00001070: 3731 3031 3130 3731 3031 3130 3131 3031  7101107101101101
-00001080: 3130 3731 3234 3130 330a 2420 6563 686f  107124103.$ echo
-00001090: 202d 656e 2022 4147 5443 4147 5443 4147   -en "AGTCAGTCAG
-000010a0: 5447 4147 4141 4147 5443 4147 5447 4147  TGAGAAAGTCAGTGAG
-000010b0: 4141 4147 5447 4147 5447 4147 4141 4147  AAAGTGAGTGAGAAAG
-000010c0: 5447 4147 5443 4147 5447 4147 4141 4147  TGAGTCAGTGAGAAAG
-000010d0: 5443 4147 4141 4147 5447 4147 5447 4147  TCAGAAAGTGAGTGAG
-000010e0: 5447 4147 4141 4147 5454 4147 4141 4147  TGAGAAAGTTAGAAAG
-000010f0: 5443 4147 4141 4147 5447 4147 5447 4147  TCAGAAAGTGAGTGAG
-00001100: 5447 4147 4141 4147 5447 4147 4141 4147  TGAGAAAGTGAGAAAG
-00001110: 5443 2220 7c20 636f 6465 7874 202d 6420  TC" | codext -d 
-00001120: 646e 612d 3220 6d6f 7273 6520 7265 7665  dna-2 morse reve
-00001130: 7273 650a 7465 7374 2073 7472 696e 670a  rse.test string.
-00001140: 6060 600a 0a23 2320 5573 6167 6520 2850  ```..## Usage (P
-00001150: 7974 686f 6e29 0a0a 4765 7474 696e 6720  ython)..Getting 
-00001160: 7468 6520 6c69 7374 206f 6620 6176 6169  the list of avai
-00001170: 6c61 626c 6520 636f 6465 6373 3a0a 0a60  lable codecs:..`
-00001180: 6060 7079 7468 6f6e 0a3e 3e3e 2069 6d70  ``python.>>> imp
-00001190: 6f72 7420 636f 6465 7874 0a3e 3e3e 2063  ort codext.>>> c
-000011a0: 6f64 6578 742e 6c69 7374 2829 0a5b 2761  odext.list().['a
-000011b0: 7363 6969 3835 272c 2027 6261 7365 3835  scii85', 'base85
-000011c0: 272c 2027 6261 7365 3130 3027 2c20 2762  ', 'base100', 'b
-000011d0: 6173 6531 3232 272c 202e 2e2e 2c20 2774  ase122', ..., 't
-000011e0: 6f6d 746f 6d27 2c20 2764 6e61 272c 2027  omtom', 'dna', '
-000011f0: 6874 6d6c 272c 2027 6d61 726b 646f 776e  html', 'markdown
-00001200: 272c 2027 7572 6c27 2c20 2772 6573 6973  ', 'url', 'resis
-00001210: 746f 7227 2c20 2773 6d73 272c 2027 7768  tor', 'sms', 'wh
-00001220: 6974 6573 7061 6365 272c 2027 7768 6974  itespace', 'whit
-00001230: 6573 7061 6365 2d61 6674 6572 2d62 6566  espace-after-bef
-00001240: 6f72 6527 5d0a 6060 600a 0a55 7361 6765  ore'].```..Usage
-00001250: 2065 7861 6d70 6c65 733a 0a0a 6060 6070   examples:..```p
-00001260: 7974 686f 6e0a 3e3e 3e20 636f 6465 7874  ython.>>> codext
-00001270: 2e65 6e63 6f64 6528 2274 6869 7320 6973  .encode("this is
-00001280: 2061 2074 6573 7422 2c20 2262 6173 6535   a test", "base5
-00001290: 382d 6269 7463 6f69 6e22 290a 276a 6f39  8-bitcoin").'jo9
-000012a0: 3177 614c 5141 314e 4e65 426d 5a4b 5546  1waLQA1NNeBmZKUF
-000012b0: 270a 3e3e 3e20 636f 6465 7874 2e65 6e63  '.>>> codext.enc
-000012c0: 6f64 6528 2274 6869 7320 6973 2061 2074  ode("this is a t
-000012d0: 6573 7422 2c20 2262 6173 6535 382d 7269  est", "base58-ri
-000012e0: 7070 6c65 2229 0a27 6a6f 3972 4132 4c51  pple").'jo9rA2LQ
-000012f0: 7772 3434 6542 6d5a 4b37 4527 0a3e 3e3e  wr44eBmZK7E'.>>>
-00001300: 2063 6f64 6578 742e 656e 636f 6465 2822   codext.encode("
-00001310: 7468 6973 2069 7320 6120 7465 7374 222c  this is a test",
-00001320: 2022 6261 7365 3538 2d75 726c 2229 0a27   "base58-url").'
-00001330: 4a4e 3931 577a 6b70 6131 6e6e 4462 4c79  JN91Wzkpa1nnDbLy
-00001340: 6a74 6627 0a60 6060 0a0a 6060 6070 7974  jtf'.```..```pyt
-00001350: 686f 6e0a 3e3e 3e20 636f 6465 6373 2e65  hon.>>> codecs.e
-00001360: 6e63 6f64 6528 2274 6869 7320 6973 2061  ncode("this is a
-00001370: 2074 6573 7422 2c20 2262 6173 6531 3030   test", "base100
-00001380: 2229 0a27 f09f 91ab f09f 919f f09f 91a0  ").'............
-00001390: f09f 91aa f09f 9097 f09f 91a0 f09f 91aa  ................
-000013a0: f09f 9097 f09f 9198 f09f 9097 f09f 91ab  ................
-000013b0: f09f 919c f09f 91aa f09f 91ab 270a 3e3e  ............'.>>
-000013c0: 3e20 636f 6465 6373 2e64 6563 6f64 6528  > codecs.decode(
-000013d0: 22f0 9f91 abf0 9f91 9ff0 9f91 a0f0 9f91  "...............
-000013e0: aaf0 9f90 97f0 9f91 a0f0 9f91 aaf0 9f90  ................
-000013f0: 97f0 9f91 98f0 9f90 97f0 9f91 abf0 9f91  ................
-00001400: 9cf0 9f91 aaf0 9f91 ab22 2c20 2262 6173  .........", "bas
-00001410: 6531 3030 2229 0a27 7468 6973 2069 7320  e100").'this is 
-00001420: 6120 7465 7374 270a 6060 600a 0a60 6060  a test'.```..```
-00001430: 7079 7468 6f6e 0a3e 3e3e 2066 6f72 2069  python.>>> for i
-00001440: 2069 6e20 7261 6e67 6528 3829 3a0a 2020   in range(8):.  
-00001450: 2020 2020 2020 7072 696e 7428 636f 6465        print(code
-00001460: 7874 2e65 6e63 6f64 6528 2274 6869 7320  xt.encode("this 
-00001470: 6973 2061 2074 6573 7422 2c20 2264 6e61  is a test", "dna
-00001480: 2d25 6422 2025 2028 6920 2b20 3129 2929  -%d" % (i + 1)))
-00001490: 0a47 5447 4147 4343 4147 4343 4747 5441  .GTGAGCCAGCCGGTA
-000014a0: 5441 4341 4147 4343 4747 5441 5441 4341  TACAAGCCGGTATACA
-000014b0: 4147 4341 4741 4341 4147 5447 4147 4347  AGCAGACAAGTGAGCG
-000014c0: 4747 5441 5447 5447 410a 4354 4341 4347  GGTATGTGA.CTCACG
-000014d0: 4741 4347 4743 4354 4154 4147 4141 4347  GACGGCCTATAGAACG
-000014e0: 4743 4354 4154 4147 4141 4347 4143 4147  GCCTATAGAACGACAG
-000014f0: 4141 4354 4341 4347 4343 4354 4154 4354  AACTCACGCCCTATCT
-00001500: 4341 0a41 4341 4741 5454 4741 5454 4141  CA.ACAGATTGATTAA
-00001510: 4347 4347 5447 4741 5454 4141 4347 4347  CGCGTGGATTAACGCG
-00001520: 5447 4741 5447 4147 5447 4741 4341 4741  TGGATGAGTGGACAGA
-00001530: 5441 4141 4347 4341 4341 470a 4147 4143  TAAACGCACAG.AGAC
-00001540: 4154 5443 4154 5441 4147 4347 4354 4343  ATTCATTAAGCGCTCC
-00001550: 4154 5441 4147 4347 4354 4343 4154 4341  ATTAAGCGCTCCATCA
-00001560: 4354 4343 4147 4143 4154 4141 4147 4347  CTCCAGACATAAAGCG
-00001570: 4147 4143 0a54 4354 4754 4141 4754 4141  AGAC.TCTGTAAGTAA
-00001580: 5454 4347 4347 4147 4754 4141 5454 4347  TTCGCGAGGTAATTCG
-00001590: 4347 4147 4754 4147 5447 4147 4754 4354  CGAGGTAGTGAGGTCT
-000015a0: 4754 4154 5454 4347 4354 4354 470a 5447  GTATTTCGCTCTG.TG
-000015b0: 5443 5441 4143 5441 4154 5447 4347 4341  TCTAACTAATTGCGCA
-000015c0: 4343 5441 4154 5447 4347 4341 4343 5441  CCTAATTGCGCACCTA
-000015d0: 4354 4341 4343 5447 5443 5441 5454 5447  CTCACCTGTCTATTTG
-000015e0: 4347 5447 5443 0a47 4147 5447 4343 5447  CGTGTC.GAGTGCCTG
-000015f0: 4343 4747 4154 4154 4354 5447 4343 4747  CCGGATATCTTGCCGG
-00001600: 4154 4154 4354 5447 4354 4754 4354 5447  ATATCTTGCTGTCTTG
-00001610: 4147 5447 4347 4747 4154 4147 4147 540a  AGTGCGGGATAGAGT.
-00001620: 4341 4354 4347 4754 4347 4743 4341 5441  CACTCGGTCGGCCATA
-00001630: 5447 5454 4347 4743 4341 5441 5447 5454  TGTTCGGCCATATGTT
-00001640: 4347 5443 5447 5454 4341 4354 4347 4343  CGTCTGTTCACTCGCC
-00001650: 4341 5441 4341 4354 0a3e 3e3e 2063 6f64  CATACACT.>>> cod
-00001660: 6578 742e 6465 636f 6465 2822 4754 4741  ext.decode("GTGA
-00001670: 4743 4341 4743 4347 4754 4154 4143 4141  GCCAGCCGGTATACAA
-00001680: 4743 4347 4754 4154 4143 4141 4743 4147  GCCGGTATACAAGCAG
-00001690: 4143 4141 4754 4741 4743 4747 4754 4154  ACAAGTGAGCGGGTAT
-000016a0: 4754 4741 222c 2022 646e 612d 3122 290a  GTGA", "dna-1").
-000016b0: 2774 6869 7320 6973 2061 2074 6573 7427  'this is a test'
-000016c0: 0a60 6060 0a0a 6060 6070 7974 686f 6e0a  .```..```python.
-000016d0: 3e3e 3e20 636f 6465 6373 2e65 6e63 6f64  >>> codecs.encod
-000016e0: 6528 2274 6869 7320 6973 2061 2074 6573  e("this is a tes
-000016f0: 7422 2c20 226d 6f72 7365 2229 0a27 2d20  t", "morse").'- 
-00001700: 2e2e 2e2e 202e 2e20 2e2e 2e20 2f20 2e2e  .... .. ... / ..
-00001710: 202e 2e2e 202f 202e 2d20 2f20 2d20 2e20   ... / .- / - . 
-00001720: 2e2e 2e20 2d27 0a3e 3e3e 2063 6f64 6563  ... -'.>>> codec
-00001730: 732e 6465 636f 6465 2822 2d20 2e2e 2e2e  s.decode("- ....
-00001740: 202e 2e20 2e2e 2e20 2f20 2e2e 202e 2e2e   .. ... / .. ...
-00001750: 202f 202e 2d20 2f20 2d20 2e20 2e2e 2e20   / .- / - . ... 
-00001760: 2d22 2c20 226d 6f72 7365 2229 0a27 7468  -", "morse").'th
-00001770: 6973 2069 7320 6120 7465 7374 270a 3e3e  is is a test'.>>
-00001780: 3e20 7769 7468 206f 7065 6e28 226d 6f72  > with open("mor
-00001790: 7365 2e74 7874 222c 2027 7727 2c20 656e  se.txt", 'w', en
-000017a0: 636f 6469 6e67 3d22 6d6f 7273 6522 2920  coding="morse") 
-000017b0: 6173 2066 3a0a 0966 2e77 7269 7465 2822  as f:..f.write("
-000017c0: 7468 6973 2069 7320 6120 7465 7374 2229  this is a test")
-000017d0: 0a31 340a 3e3e 3e20 7769 7468 206f 7065  .14.>>> with ope
-000017e0: 6e28 226d 6f72 7365 2e74 7874 222c 656e  n("morse.txt",en
-000017f0: 636f 6469 6e67 3d22 6d6f 7273 6522 2920  coding="morse") 
-00001800: 6173 2066 3a0a 0966 2e72 6561 6428 290a  as f:..f.read().
-00001810: 2774 6869 7320 6973 2061 2074 6573 7427  'this is a test'
-00001820: 0a60 6060 0a0a 6060 6070 7974 686f 6e0a  .```..```python.
-00001830: 3e3e 3e20 636f 6465 7874 2e64 6563 6f64  >>> codext.decod
-00001840: 6528 2222 220a 2020 2020 2020 3d20 2020  e(""".      =   
-00001850: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-00001860: 2020 2020 2020 2020 5820 2020 2020 2020          X       
-00001870: 2020 0a20 2020 3a20 2020 2020 2020 2020    .   :         
-00001880: 2020 200a 2020 2020 2020 7820 2020 2020     .      x     
-00001890: 2020 2020 0a20 206e 2020 0a20 2020 2072      .  n  .    r
-000018a0: 200a 2020 2020 2020 2020 7920 2020 0a20   .        y   . 
-000018b0: 2020 2020 2059 2020 2020 2020 2020 2020       Y          
-000018c0: 2020 0a20 2020 2020 2020 2020 2020 2020    .             
-000018d0: 2079 2020 2020 2020 2020 0a20 2020 2020   y        .     
-000018e0: 7020 2020 200a 2020 2020 2020 2020 2061  p    .         a
-000018f0: 2020 2020 2020 200a 2060 2020 2020 2020         . `      
-00001900: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
-00001910: 206e 2020 2020 2020 2020 2020 2020 0a20   n            . 
-00001920: 2020 2020 2020 2020 207c 2020 2020 0a20           |    . 
-00001930: 2061 2020 2020 2020 2020 2020 0a6f 2020   a          .o  
-00001940: 2020 0a20 2020 2020 2020 6820 2020 2020    .       h     
-00001950: 2020 200a 2020 2020 2020 2020 2020 6020     .          ` 
-00001960: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-00001970: 2020 2020 2020 6720 2020 2020 2020 2020        g         
-00001980: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-00001990: 2020 6f20 0a20 2020 7a20 2020 2020 2022    o .   z      "
-000019a0: 2222 2c20 2277 6869 7465 7370 6163 652d  "", "whitespace-
-000019b0: 6166 7465 722b 6265 666f 7265 2229 0a27  after+before").'
-000019c0: 4353 437b 6e6f 745f 736f 5f69 6e76 6973  CSC{not_so_invis
-000019d0: 6962 6c65 7d27 0a60 6060 0a0a 6060 6070  ible}'.```..```p
-000019e0: 7974 686f 6e0a 3e3e 3e20 7072 696e 7428  ython.>>> print(
-000019f0: 636f 6465 7874 2e65 6e63 6f64 6528 2241  codext.encode("A
-00001a00: 6e20 6578 616d 706c 6520 7465 7374 2073  n example test s
-00001a10: 7472 696e 6722 2c20 2262 6175 646f 742d  tring", "baudot-
-00001a20: 7461 7065 2229 290a 2a2a 2a2e 2a2a 0a20  tape")).***.**. 
-00001a30: 2020 2e20 2a0a 2a2a 2a2e 2a20 0a2a 2020    . *.***.* .*  
-00001a40: 2e20 200a 2020 202e 2a20 0a2a 2020 2e2a  .  .   .* .*  .*
-00001a50: 200a 2020 202e 202a 0a2a 2a20 2e2a 200a   .   . *.** .* .
-00001a60: 2a2a 2a2e 2a2a 0a2a 2a20 2e2a 2a0a 2020  ***.**.** .**.  
-00001a70: 202e 2a20 0a2a 2020 2e20 200a 2a20 2a2e   .* .*  .  .* *.
-00001a80: 202a 0a20 2020 2e2a 200a 2a20 2a2e 2020   *.   .* .* *.  
-00001a90: 0a2a 202a 2e20 2a0a 2a20 202e 2020 0a2a  .* *. *.*  .  .*
-00001aa0: 202a 2e20 200a 2a20 2a2e 202a 0a2a 2a2a   *.  .* *. *.***
-00001ab0: 2e20 200a 2020 2a2e 2a20 0a2a 2a2a 2e2a  .  .  *.* .***.*
-00001ac0: 200a 202a 202e 2a20 0a60 6060 0a0a 2323   . * .* .```..##
-00001ad0: 204c 6973 7420 6f66 2063 6f64 6563 730a   List of codecs.
-00001ae0: 0a2a 2a43 6f64 6563 2a2a 207c 202a 2a43  .**Codec** | **C
-00001af0: 6f6e 7665 7273 696f 6e73 2a2a 207c 202a  onversions** | *
-00001b00: 2a43 6f6d 6d65 6e74 2a2a 0a3a 2d2d 2d3a  *Comment**.:---:
-00001b10: 207c 203a 2d2d 2d3a 207c 202d 2d2d 0a60   | :---: | ---.`
-00001b20: 6131 7a32 3660 207c 2074 6578 7420 3c2d  a1z26` | text <-
-00001b30: 3e20 616c 7068 6162 6574 206f 7264 6572  > alphabet order
-00001b40: 206e 756d 6265 7273 207c 206b 6565 7073   numbers | keeps
-00001b50: 2077 6f72 6473 2077 6869 7465 7370 6163   words whitespac
-00001b60: 652d 7365 7061 7261 7465 6420 616e 6420  e-separated and 
-00001b70: 7573 6573 2061 2063 7573 746f 6d20 6368  uses a custom ch
-00001b80: 6172 6163 7465 7220 7365 7061 7261 746f  aracter separato
-00001b90: 720a 6061 6666 696e 6560 207c 2074 6578  r.`affine` | tex
-00001ba0: 7420 3c2d 3e20 6166 6669 6e65 2063 6970  t <-> affine cip
-00001bb0: 6865 7274 6578 7420 7c20 616b 6120 4166  hertext | aka Af
-00001bc0: 6669 6e65 2043 6970 6865 720a 6061 7363  fine Cipher.`asc
-00001bd0: 6969 3835 6020 7c20 7465 7874 203c 2d3e  ii85` | text <->
-00001be0: 2061 7363 6969 3835 2065 6e63 6f64 6564   ascii85 encoded
-00001bf0: 2074 6578 7420 7c20 5079 7468 6f6e 2033   text | Python 3
-00001c00: 206f 6e6c 790a 6061 7462 6173 6860 207c   only.`atbash` |
-00001c10: 2074 6578 7420 3c2d 3e20 4174 6261 7368   text <-> Atbash
-00001c20: 2063 6970 6865 7274 6578 7420 7c20 616b   ciphertext | ak
-00001c30: 6120 4174 6261 7368 2043 6970 6865 720a  a Atbash Cipher.
-00001c40: 6062 6163 6f6e 6020 7c20 7465 7874 203c  `bacon` | text <
-00001c50: 2d3e 2042 6163 6f6e 2063 6970 6865 7274  -> Bacon ciphert
-00001c60: 6578 7420 7c20 616b 6120 4261 636f 6e69  ext | aka Baconi
-00001c70: 616e 2043 6970 6865 720a 6062 6172 6269  an Cipher.`barbi
-00001c80: 652d 4e60 207c 2074 6578 7420 3c2d 3e20  e-N` | text <-> 
-00001c90: 6261 7262 6965 2063 6970 6865 7274 6578  barbie ciphertex
-00001ca0: 7420 7c20 616b 6120 4261 7262 6965 2054  t | aka Barbie T
-00001cb0: 7970 6577 7269 7465 7220 284e 2062 656c  ypewriter (N bel
-00001cc0: 6f6e 6773 2074 6f20 5b31 2c20 345d 290a  ongs to [1, 4]).
-00001cd0: 6062 6173 6558 5860 207c 2074 6578 7420  `baseXX` | text 
-00001ce0: 3c2d 3e20 6261 7365 5858 207c 2073 6565  <-> baseXX | see
-00001cf0: 205b 6261 7365 2065 6e63 6f64 696e 6773   [base encodings
-00001d00: 5d28 6874 7470 733a 2f2f 7079 7468 6f6e  ](https://python
-00001d10: 2d63 6f64 6578 742e 7265 6164 7468 6564  -codext.readthed
-00001d20: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-00001d30: 2f65 6e63 2f62 6173 652e 6874 6d6c 2920  /enc/base.html) 
-00001d40: 2869 6e63 6c20 6261 7365 3332 2c20 3336  (incl base32, 36
-00001d50: 2c20 3435 2c20 3538 2c20 3632 2c20 3633  , 45, 58, 62, 63
-00001d60: 2c20 3634 2c20 3931 2c20 3130 302c 2031  , 64, 91, 100, 1
-00001d70: 3232 290a 6062 6175 646f 7460 207c 2074  22).`baudot` | t
-00001d80: 6578 7420 3c2d 3e20 4261 7564 6f74 2063  ext <-> Baudot c
-00001d90: 6f64 6520 6269 7473 207c 2073 7570 706f  ode bits | suppo
-00001da0: 7274 7320 4343 4954 542d 312c 2043 4349  rts CCITT-1, CCI
-00001db0: 5454 2d32 2c20 4555 2f46 522c 2049 5441  TT-2, EU/FR, ITA
-00001dc0: 312c 2049 5441 322c 204d 544b 2d32 2028  1, ITA2, MTK-2 (
-00001dd0: 5079 7468 6f6e 3320 6f6e 6c79 292c 2055  Python3 only), U
-00001de0: 4b2c 202e 2e2e 0a60 6263 6460 207c 2074  K, ....`bcd` | t
-00001df0: 6578 7420 3c2d 3e20 6269 6e61 7279 2063  ext <-> binary c
-00001e00: 6f64 6564 2064 6563 696d 616c 2074 6578  oded decimal tex
-00001e10: 7420 7c20 656e 636f 6465 7320 6368 6172  t | encodes char
-00001e20: 6163 7465 7273 2066 726f 6d20 7468 6569  acters from thei
-00001e30: 7220 287a 6572 6f2d 6c65 6674 2d70 6164  r (zero-left-pad
-00001e40: 6465 6429 206f 7264 696e 616c 730a 6062  ded) ordinals.`b
-00001e50: 7261 696c 6c65 6020 7c20 7465 7874 203c  raille` | text <
-00001e60: 2d3e 2062 7261 696c 6c65 2073 796d 626f  -> braille symbo
-00001e70: 6c73 207c 2050 7974 686f 6e20 3320 6f6e  ls | Python 3 on
-00001e80: 6c79 0a60 6369 7472 6978 6020 7c20 7465  ly.`citrix` | te
-00001e90: 7874 203c 2d3e 2043 6974 7269 7820 4354  xt <-> Citrix CT
-00001ea0: 5831 2063 6970 6865 7274 6578 7420 7c20  X1 ciphertext | 
-00001eb0: 616b 6120 4369 7472 6978 2043 5458 3120  aka Citrix CTX1 
-00001ec0: 7061 7373 6f72 6420 656e 636f 6469 6e67  passord encoding
-00001ed0: 0a60 646e 6160 207c 2074 6578 7420 3c2d  .`dna` | text <-
-00001ee0: 3e20 444e 412d 4e20 7365 7175 656e 6365  > DNA-N sequence
-00001ef0: 207c 2069 6d70 6c65 6d65 6e74 7320 7468   | implements th
-00001f00: 6520 3820 7275 6c65 7320 6f66 2044 4e41  e 8 rules of DNA
-00001f10: 2073 6571 7565 6e63 6573 2028 4e20 6265   sequences (N be
-00001f20: 6c6f 6e67 7320 746f 205b 312c 385d 290a  longs to [1,8]).
-00001f30: 6065 7863 6573 7333 6020 7c20 7465 7874  `excess3` | text
-00001f40: 203c 2d3e 2058 5333 2065 6e63 6f64 6564   <-> XS3 encoded
-00001f50: 2074 6578 7420 7c20 7573 6573 2045 7863   text | uses Exc
-00001f60: 6573 732d 3320 2861 6b61 2053 7469 6269  ess-3 (aka Stibi
-00001f70: 747a 2063 6f64 6529 2062 696e 6172 7920  tz code) binary 
-00001f80: 656e 636f 6469 6e67 2074 6f20 636f 6e76  encoding to conv
-00001f90: 6572 7420 6368 6172 6163 7465 7273 2066  ert characters f
-00001fa0: 726f 6d20 7468 6569 7220 6f72 6469 6e61  rom their ordina
-00001fb0: 6c73 0a60 6772 6179 6020 7c20 7465 7874  ls.`gray` | text
-00001fc0: 203c 2d3e 2067 7261 7920 656e 636f 6465   <-> gray encode
-00001fd0: 6420 7465 7874 207c 2061 6b61 2072 6566  d text | aka ref
-00001fe0: 6c65 6374 6564 2062 696e 6172 7920 636f  lected binary co
-00001ff0: 6465 0a60 677a 6970 6020 7c20 7465 7874  de.`gzip` | text
-00002000: 203c 2d3e 2047 7a69 702d 636f 6d70 7265   <-> Gzip-compre
-00002010: 7373 6564 2074 6578 7420 7c20 7374 616e  ssed text | stan
-00002020: 6461 7264 2047 7a69 7020 636f 6d70 7265  dard Gzip compre
-00002030: 7373 696f 6e2f 6465 636f 6d70 7265 7373  ssion/decompress
-00002040: 696f 6e0a 6068 746d 6c60 207c 2074 6578  ion.`html` | tex
-00002050: 7420 3c2d 3e20 4854 4d4c 2065 6e74 6974  t <-> HTML entit
-00002060: 6965 7320 7c20 696d 706c 656d 656e 7473  ies | implements
-00002070: 2065 6e74 6974 6965 7320 6163 636f 7264   entities accord
-00002080: 696e 6720 746f 205b 7468 6973 2072 6566  ing to [this ref
-00002090: 6572 656e 6365 5d28 6874 7470 733a 2f2f  erence](https://
-000020a0: 6465 762e 7733 2e6f 7267 2f68 746d 6c35  dev.w3.org/html5
-000020b0: 2f68 746d 6c2d 6175 7468 6f72 2f63 6861  /html-author/cha
-000020c0: 7272 6566 290a 6069 7073 756d 6020 7c20  rref).`ipsum` | 
-000020d0: 7465 7874 203c 2d3e 206c 6174 696e 2077  text <-> latin w
-000020e0: 6f72 6473 207c 2061 6b61 206c 6f72 656d  ords | aka lorem
-000020f0: 2069 7073 756d 0a60 6b6c 6f70 6660 207c   ipsum.`klopf` |
-00002100: 2074 6578 7420 3c2d 3e20 6b6c 6f70 6620   text <-> klopf 
-00002110: 656e 636f 6465 6420 7465 7874 207c 2050  encoded text | P
-00002120: 6f6c 7962 6975 7320 7371 7561 7265 2077  olybius square w
-00002130: 6974 6820 7472 6976 6961 6c20 616c 7068  ith trivial alph
-00002140: 6162 6574 6963 616c 2064 6973 7472 6962  abetical distrib
-00002150: 7574 696f 6e0a 606c 6565 7473 7065 616b  ution.`leetspeak
-00002160: 6020 7c20 7465 7874 203c 2d3e 206c 6565  ` | text <-> lee
-00002170: 7473 7065 616b 2065 6e63 6f64 6564 2074  tspeak encoded t
-00002180: 6578 7420 7c20 6261 7365 6420 6f6e 206d  ext | based on m
-00002190: 696e 696d 616c 6973 7469 6320 656c 6974  inimalistic elit
-000021a0: 6520 7370 6561 6b69 6e67 2072 756c 6573  e speaking rules
-000021b0: 0a60 6c65 7474 6572 2d69 6e64 6963 6573  .`letter-indices
-000021c0: 6020 7c20 7465 7874 203c 2d3e 2074 6578  ` | text <-> tex
-000021d0: 7420 7769 7468 206c 6574 7465 7220 696e  t with letter in
-000021e0: 6469 6365 7320 7c20 656e 636f 6465 7320  dices | encodes 
-000021f0: 636f 6e73 6f6e 616e 7473 2061 6e64 2f6f  consonants and/o
-00002200: 7220 766f 7765 6c73 2077 6974 6820 7468  r vowels with th
-00002210: 6569 7220 636f 7272 6573 706f 6e64 696e  eir correspondin
-00002220: 6720 696e 6469 6365 730a 606c 7a37 3760  g indices.`lz77`
-00002230: 207c 2074 6578 7420 3c2d 3e20 4c5a 3737   | text <-> LZ77
-00002240: 2d63 6f6d 7072 6573 7365 6420 7465 7874  -compressed text
-00002250: 207c 2063 6f6d 7072 6573 7365 7320 7468   | compresses th
-00002260: 6520 6769 7665 6e20 6461 7461 2077 6974  e given data wit
-00002270: 6820 7468 6520 616c 676f 7269 7468 6d20  h the algorithm 
-00002280: 6f66 204c 656d 7065 6c20 616e 6420 5a69  of Lempel and Zi
-00002290: 7620 6f66 2031 3937 370a 606c 7a37 3860  v of 1977.`lz78`
-000022a0: 207c 2074 6578 7420 3c2d 3e20 4c5a 3738   | text <-> LZ78
-000022b0: 2d63 6f6d 7072 6573 7365 6420 7465 7874  -compressed text
-000022c0: 207c 2063 6f6d 7072 6573 7365 7320 7468   | compresses th
-000022d0: 6520 6769 7665 6e20 6461 7461 2077 6974  e given data wit
-000022e0: 6820 7468 6520 616c 676f 7269 7468 6d20  h the algorithm 
-000022f0: 6f66 204c 656d 7065 6c20 616e 6420 5a69  of Lempel and Zi
-00002300: 7620 6f66 2031 3937 380a 606d 616e 6368  v of 1978.`manch
-00002310: 6573 7465 7260 207c 2074 6578 7420 3c2d  ester` | text <-
-00002320: 3e20 6d61 6e63 6865 7374 6572 2065 6e63  > manchester enc
-00002330: 6f64 6564 2074 6578 7420 7c20 584f 5265  oded text | XORe
-00002340: 7320 6561 6368 2062 6974 206f 6620 7468  s each bit of th
-00002350: 6520 696e 7075 7420 7769 7468 2060 3031  e input with `01
-00002360: 600a 606d 6172 6b64 6f77 6e60 207c 206d  `.`markdown` | m
-00002370: 6172 6b64 6f77 6e20 2d2d 3e20 4854 4d4c  arkdown --> HTML
-00002380: 207c 2075 6e69 6469 7265 6374 696f 6e61   | unidirectiona
-00002390: 6c0a 606d 6f72 7365 6020 7c20 7465 7874  l.`morse` | text
-000023a0: 203c 2d3e 206d 6f72 7365 2065 6e63 6f64   <-> morse encod
-000023b0: 6564 2074 6578 7420 7c20 7573 6573 2077  ed text | uses w
-000023c0: 6869 7465 7370 6163 6520 6173 2061 2073  hitespace as a s
-000023d0: 6570 6172 6174 6f72 0a60 6e61 7661 6a6f  eparator.`navajo
-000023e0: 6020 7c20 7465 7874 203c 2d3e 204e 6176  ` | text <-> Nav
-000023f0: 616a 6f20 7c20 6f6e 6c79 2068 616e 646c  ajo | only handl
-00002400: 6573 206c 6574 7465 7273 2028 6e6f 7420  es letters (not 
-00002410: 6675 6c6c 2077 6f72 6473 2066 726f 6d20  full words from 
-00002420: 7468 6520 4e61 7661 6a6f 2064 6963 7469  the Navajo dicti
-00002430: 6f6e 6172 7929 0a60 6f63 7461 6c60 207c  onary).`octal` |
-00002440: 2074 6578 7420 3c2d 3e20 6f63 7461 6c20   text <-> octal 
-00002450: 6469 6769 7473 207c 2064 756d 6d79 206f  digits | dummy o
-00002460: 6374 616c 2063 6f6e 7665 7273 696f 6e20  ctal conversion 
-00002470: 2863 6f6e 7665 7274 7320 746f 2033 2d64  (converts to 3-d
-00002480: 6967 6974 7320 6772 6f75 7073 290a 606f  igits groups).`o
-00002490: 7264 696e 616c 6020 7c20 7465 7874 203c  rdinal` | text <
-000024a0: 2d3e 206f 7264 696e 616c 2064 6967 6974  -> ordinal digit
-000024b0: 7320 7c20 6475 6d6d 7920 6368 6172 6163  s | dummy charac
-000024c0: 7465 7220 6f72 6469 6e61 6c73 2063 6f6e  ter ordinals con
-000024d0: 7665 7273 696f 6e20 2863 6f6e 7665 7274  version (convert
-000024e0: 7320 746f 2033 2d64 6967 6974 7320 6772  s to 3-digits gr
-000024f0: 6f75 7073 290a 6070 6b7a 6970 5f64 6566  oups).`pkzip_def
-00002500: 6c61 7465 6020 7c20 7465 7874 203c 2d3e  late` | text <->
-00002510: 2064 6566 6c61 7465 6420 7465 7874 207c   deflated text |
-00002520: 2073 7461 6e64 6172 6420 5a69 702d 6465   standard Zip-de
-00002530: 666c 6174 6520 636f 6d70 7265 7373 696f  flate compressio
-00002540: 6e2f 6465 636f 6d70 7265 7373 696f 6e0a  n/decompression.
-00002550: 6070 6b7a 6970 5f62 7a69 7032 6020 7c20  `pkzip_bzip2` | 
-00002560: 7465 7874 203c 2d3e 2042 7a69 7070 6564  text <-> Bzipped
-00002570: 2074 6578 7420 7c20 7374 616e 6461 7264   text | standard
-00002580: 2042 5a69 7032 2063 6f6d 7072 6573 7369   BZip2 compressi
-00002590: 6f6e 2f64 6563 6f6d 7072 6573 7369 6f6e  on/decompression
-000025a0: 0a60 706b 7a69 705f 6c7a 6d61 6020 7c20  .`pkzip_lzma` | 
-000025b0: 7465 7874 203c 2d3e 204c 5a4d 412d 636f  text <-> LZMA-co
-000025c0: 6d70 7265 7373 6564 2074 6578 7420 7c20  mpressed text | 
-000025d0: 7374 616e 6461 7264 204c 5a4d 4120 636f  standard LZMA co
-000025e0: 6d70 7265 7373 696f 6e2f 6465 636f 6d70  mpression/decomp
-000025f0: 7265 7373 696f 6e0a 6072 6164 696f 6020  ression.`radio` 
-00002600: 7c20 7465 7874 203c 2d3e 2072 6164 696f  | text <-> radio
-00002610: 2077 6f72 6473 207c 2061 6b61 204e 4154   words | aka NAT
-00002620: 4f20 6f72 2072 6164 696f 2070 686f 6e65  O or radio phone
-00002630: 7469 6320 616c 7068 6162 6574 0a60 7265  tic alphabet.`re
-00002640: 7369 7374 6f72 6020 7c20 7465 7874 203c  sistor` | text <
-00002650: 2d3e 2072 6573 6973 746f 7220 636f 6c6f  -> resistor colo
-00002660: 7273 207c 2061 6b61 2072 6573 6973 746f  rs | aka resisto
-00002670: 7220 636f 6c6f 7220 636f 6465 730a 6072  r color codes.`r
-00002680: 6f74 6020 7c20 7465 7874 203c 2d3e 2072  ot` | text <-> r
-00002690: 6f74 284e 2920 6369 7068 6572 7465 7874  ot(N) ciphertext
-000026a0: 207c 2061 6b61 2043 6165 7361 7220 6369   | aka Caesar ci
-000026b0: 7068 6572 2028 4e20 6265 6c6f 6e67 7320  pher (N belongs 
-000026c0: 746f 205b 312c 3235 5d29 0a60 726f 7461  to [1,25]).`rota
-000026d0: 7465 6020 7c20 7465 7874 203c 2d3e 204e  te` | text <-> N
-000026e0: 2d62 6974 732d 726f 7461 7465 6420 7465  -bits-rotated te
-000026f0: 7874 207c 2072 6f74 6174 6573 2063 6861  xt | rotates cha
-00002700: 7261 6374 6572 7320 6279 2074 6865 2073  racters by the s
-00002710: 7065 6369 6669 6564 206e 756d 6265 7220  pecified number 
-00002720: 6f66 2062 6974 7320 3b20 5079 7468 6f6e  of bits ; Python
-00002730: 2033 206f 6e6c 790a 6073 6379 7461 6c65   3 only.`scytale
-00002740: 6020 7c20 7465 7874 203c 2d3e 2073 6379  ` | text <-> scy
-00002750: 7461 6c65 2063 6970 6865 7274 6578 7420  tale ciphertext 
-00002760: 7c20 656e 6372 7970 7473 2077 6974 6820  | encrypts with 
-00002770: 4c2c 2074 6865 206e 756d 6265 7220 6f66  L, the number of
-00002780: 206c 6574 7465 7273 206f 6e20 7468 6520   letters on the 
-00002790: 726f 6420 2862 656c 6f6e 6773 2074 6f20  rod (belongs to 
-000027a0: 5b31 2c5b 290a 6073 6869 6674 6020 7c20  [1,[).`shift` | 
-000027b0: 7465 7874 203c 2d3e 2073 6869 6674 284e  text <-> shift(N
-000027c0: 2920 6369 7068 6572 7465 7874 207c 2073  ) ciphertext | s
-000027d0: 6869 6674 206f 7264 696e 616c 7320 7769  hift ordinals wi
-000027e0: 7468 204e 2028 6265 6c6f 6e67 7320 746f  th N (belongs to
-000027f0: 205b 312c 3235 355d 290a 6073 6d73 6020   [1,255]).`sms` 
-00002800: 7c20 7465 7874 203c 2d3e 2070 686f 6e65  | text <-> phone
-00002810: 206b 6579 7374 726f 6b65 7320 7c20 616c   keystrokes | al
-00002820: 736f 2063 616c 6c65 6420 5439 2063 6f64  so called T9 cod
-00002830: 6520 3b20 7573 6573 2022 602d 6022 2061  e ; uses "`-`" a
-00002840: 7320 6120 7365 7061 7261 746f 7220 666f  s a separator fo
-00002850: 7220 656e 636f 6469 6e67 2c20 2260 2d60  r encoding, "`-`
-00002860: 2220 6f72 2022 605f 6022 206f 7220 7768  " or "`_`" or wh
-00002870: 6974 6573 7061 6365 2066 6f72 2064 6563  itespace for dec
-00002880: 6f64 696e 670a 6073 6f75 7468 7061 726b  oding.`southpark
-00002890: 6020 7c20 7465 7874 203c 2d3e 204b 656e  ` | text <-> Ken
-000028a0: 6e79 2773 206c 616e 6775 6167 6520 7c20  ny's language | 
-000028b0: 636f 6e76 6572 7473 206c 6574 7465 7273  converts letters
-000028c0: 2074 6f20 4b65 6e6e 7927 7320 6c61 6e67   to Kenny's lang
-000028d0: 7561 6765 2066 726f 6d20 536f 7574 6870  uage from Southp
-000028e0: 6172 6b20 2877 6869 7465 7370 6163 6520  ark (whitespace 
-000028f0: 6973 2061 6c73 6f20 6861 6e64 6c65 6429  is also handled)
-00002900: 0a60 746f 6d74 6f6d 6020 7c20 7465 7874  .`tomtom` | text
-00002910: 203c 2d3e 2074 6f6d 2d74 6f6d 2065 6e63   <-> tom-tom enc
-00002920: 6f64 6564 2074 6578 7420 7c20 7369 6d69  oded text | simi
-00002930: 6c61 7220 746f 2060 6d6f 7273 6560 2c20  lar to `morse`, 
-00002940: 7573 696e 6720 736c 6173 6865 7320 616e  using slashes an
-00002950: 6420 6261 636b 736c 6173 6865 730a 6075  d backslashes.`u
-00002960: 726c 6020 7c20 7465 7874 203c 2d3e 2055  rl` | text <-> U
-00002970: 524c 2065 6e63 6f64 6564 2074 6578 7420  RL encoded text 
-00002980: 7c20 616b 6120 5552 4c20 656e 636f 6469  | aka URL encodi
-00002990: 6e67 0a60 786f 7260 207c 2074 6578 7420  ng.`xor` | text 
-000029a0: 3c2d 3e20 584f 5228 4e29 2063 6970 6865  <-> XOR(N) ciphe
-000029b0: 7274 6578 7420 7c20 584f 5220 7769 7468  rtext | XOR with
-000029c0: 2061 2073 696e 676c 6520 6279 7465 2028   a single byte (
-000029d0: 4e20 6265 6c6f 6e67 7320 746f 205b 312c  N belongs to [1,
-000029e0: 3235 355d 290a 6077 6869 7465 7370 6163  255]).`whitespac
-000029f0: 6560 207c 2074 6578 7420 3c2d 3e20 7768  e` | text <-> wh
-00002a00: 6974 6573 7061 6365 7320 616e 6420 7461  itespaces and ta
-00002a10: 6273 207c 2072 6570 6c61 6365 7320 6269  bs | replaces bi
-00002a20: 7473 2077 6974 6820 7768 6974 6573 7061  ts with whitespa
-00002a30: 6365 7320 616e 6420 7461 6273 0a0a 4120  ces and tabs..A 
-00002a40: 6665 7720 7661 7269 616e 7473 2061 7265  few variants are
-00002a50: 2061 6c73 6f20 696d 706c 656d 656e 7465   also implemente
-00002a60: 642e 0a0a 2a2a 436f 6465 632a 2a20 7c20  d...**Codec** | 
-00002a70: 2a2a 436f 6e76 6572 7369 6f6e 732a 2a20  **Conversions** 
-00002a80: 7c20 2a2a 436f 6d6d 656e 742a 2a0a 3a2d  | **Comment**.:-
-00002a90: 2d2d 3a20 7c20 3a2d 2d2d 3a20 7c20 2d2d  --: | :---: | --
-00002aa0: 2d0a 6062 6175 646f 742d 7370 6163 6564  -.`baudot-spaced
-00002ab0: 6020 7c20 7465 7874 203c 2d3e 2042 6175  ` | text <-> Bau
-00002ac0: 646f 7420 636f 6465 2067 726f 7570 7320  dot code groups 
-00002ad0: 6f66 2062 6974 7320 7c20 6772 6f75 7073  of bits | groups
-00002ae0: 206f 6620 3520 6269 7473 2061 7265 2077   of 5 bits are w
-00002af0: 6869 7465 7370 6163 652d 7365 7061 7261  hitespace-separa
-00002b00: 7465 640a 6062 6175 646f 742d 7461 7065  ted.`baudot-tape
-00002b10: 6020 7c20 7465 7874 203c 2d3e 2042 6175  ` | text <-> Bau
-00002b20: 646f 7420 636f 6465 2074 6170 6520 7c20  dot code tape | 
-00002b30: 6f75 7470 7574 7320 6120 7374 7269 6e67  outputs a string
-00002b40: 2074 6861 7420 6c6f 6f6b 7320 6c69 6b65   that looks like
-00002b50: 2061 2070 6572 666f 7261 7465 6420 7461   a perforated ta
-00002b60: 7065 0a60 6263 642d 6578 7465 6e64 6564  pe.`bcd-extended
-00002b70: 3060 207c 2074 6578 7420 3c2d 3e20 4243  0` | text <-> BC
-00002b80: 442d 6578 7465 6e64 6564 2074 6578 7420  D-extended text 
-00002b90: 7c20 656e 636f 6465 7320 6368 6172 6163  | encodes charac
-00002ba0: 7465 7273 2066 726f 6d20 7468 6569 7220  ters from their 
-00002bb0: 287a 6572 6f2d 6c65 6674 2d70 6164 6465  (zero-left-padde
-00002bc0: 6429 206f 7264 696e 616c 7320 7573 696e  d) ordinals usin
-00002bd0: 6720 7072 6566 6978 2062 6974 7320 6030  g prefix bits `0
-00002be0: 3030 3060 0a60 6263 642d 6578 7465 6e64  000`.`bcd-extend
-00002bf0: 6564 3160 207c 2074 6578 7420 3c2d 3e20  ed1` | text <-> 
-00002c00: 4243 442d 6578 7465 6e64 6564 2074 6578  BCD-extended tex
-00002c10: 7420 7c20 656e 636f 6465 7320 6368 6172  t | encodes char
-00002c20: 6163 7465 7273 2066 726f 6d20 7468 6569  acters from thei
-00002c30: 7220 287a 6572 6f2d 6c65 6674 2d70 6164  r (zero-left-pad
-00002c40: 6465 6429 206f 7264 696e 616c 7320 7573  ded) ordinals us
-00002c50: 696e 6720 7072 6566 6978 2062 6974 7320  ing prefix bits 
-00002c60: 6031 3131 3160 0a60 6d61 6e63 6865 7374  `1111`.`manchest
-00002c70: 6572 2d69 6e76 6572 7465 6460 207c 2074  er-inverted` | t
-00002c80: 6578 7420 3c2d 3e20 6d61 6e63 6865 7374  ext <-> manchest
-00002c90: 6572 2065 6e63 6f64 6564 2074 6578 7420  er encoded text 
-00002ca0: 7c20 584f 5265 7320 6561 6368 2062 6974  | XORes each bit
-00002cb0: 206f 6620 7468 6520 696e 7075 7420 7769   of the input wi
-00002cc0: 7468 2060 3130 600a 606f 6374 616c 2d73  th `10`.`octal-s
-00002cd0: 7061 6365 6460 207c 2074 6578 7420 3c2d  paced` | text <-
-00002ce0: 3e20 6f63 7461 6c20 6469 6769 7473 2028  > octal digits (
-00002cf0: 7768 6974 6573 7061 6365 2d73 6570 6172  whitespace-separ
-00002d00: 6174 6564 2920 7c20 6475 6d6d 7920 6f63  ated) | dummy oc
-00002d10: 7461 6c20 636f 6e76 6572 7369 6f6e 0a60  tal conversion.`
-00002d20: 6f72 6469 6e61 6c2d 7370 6163 6564 6020  ordinal-spaced` 
-00002d30: 7c20 7465 7874 203c 2d3e 206f 7264 696e  | text <-> ordin
-00002d40: 616c 2064 6967 6974 7320 2877 6869 7465  al digits (white
-00002d50: 7370 6163 652d 7365 7061 7261 7465 6429  space-separated)
-00002d60: 207c 2064 756d 6d79 2063 6861 7261 6374   | dummy charact
-00002d70: 6572 206f 7264 696e 616c 7320 636f 6e76  er ordinals conv
-00002d80: 6572 7369 6f6e 0a60 736f 7574 6870 6172  ersion.`southpar
-00002d90: 6b2d 6963 6173 6560 207c 2074 6578 7420  k-icase` | text 
-00002da0: 3c2d 3e20 4b65 6e6e 7927 7320 6c61 6e67  <-> Kenny's lang
-00002db0: 7561 6765 207c 2073 616d 6520 6173 2060  uage | same as `
-00002dc0: 736f 7574 6870 6172 6b60 2062 7574 2063  southpark` but c
-00002dd0: 6173 6520 696e 7365 6e73 6974 6976 650a  ase insensitive.
-00002de0: 6077 6869 7465 7370 6163 655f 6166 7465  `whitespace_afte
-00002df0: 725f 6265 666f 7265 6020 7c20 7465 7874  r_before` | text
-00002e00: 203c 2d3e 206c 696e 6573 206f 6620 7768   <-> lines of wh
-00002e10: 6974 6573 7061 6365 735b 6c65 7474 6572  itespaces[letter
-00002e20: 5d77 6869 7465 7370 6163 6573 207c 2065  ]whitespaces | e
-00002e30: 6e63 6f64 6573 2063 6861 7261 6374 6572  ncodes character
-00002e40: 7320 6173 206e 6577 2063 6861 7261 6374  s as new charact
-00002e50: 6572 7320 7769 7468 2077 6869 7465 7370  ers with whitesp
-00002e60: 6163 6573 2062 6566 6f72 6520 616e 6420  aces before and 
-00002e70: 6166 7465 7220 6163 636f 7264 696e 6720  after according 
-00002e80: 746f 2061 6e20 6571 7561 7469 6f6e 2064  to an equation d
-00002e90: 6573 6372 6962 6564 2069 6e20 7468 6520  escribed in the 
-00002ea0: 636f 6465 6320 6e61 6d65 2028 652e 672e  codec name (e.g.
-00002eb0: 2022 6077 6869 7465 7370 6163 652b 322a   "`whitespace+2*
-00002ec0: 6166 7465 722d 332a 6265 666f 7265 6022  after-3*before`"
-00002ed0: 290a 0a0a 0a                             )....
+00000420: 4e53 450a 0a3c 6831 2061 6c69 676e 3d22  NSE..<h1 align="
+00000430: 6365 6e74 6572 223e 436f 6445 7874 203c  center">CodExt <
+00000440: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000450: 7477 6974 7465 722e 636f 6d2f 696e 7465  twitter.com/inte
+00000460: 6e74 2f74 7765 6574 3f74 6578 743d 436f  nt/tweet?text=Co
+00000470: 6445 7874 2532 302d 2532 3045 6e63 6f64  dExt%20-%20Encod
+00000480: 696e 6725 3246 6465 636f 6469 6e67 2532  ing%2Fdecoding%2
+00000490: 3061 6e79 7468 696e 672e 2530 4425 3041  0anything.%0D%0A
+000004a0: 5079 7468 6f6e 2532 306c 6962 7261 7279  Python%20library
+000004b0: 2532 3065 7874 656e 6469 6e67 2532 3074  %20extending%20t
+000004c0: 6865 2532 306e 6174 6976 6525 3230 636f  he%20native%20co
+000004d0: 6465 6373 2532 306c 6962 7261 7279 2532  decs%20library%2
+000004e0: 3077 6974 6825 3230 6d61 6e79 2532 306e  0with%20many%20n
+000004f0: 6577 2532 3065 6e63 6f64 696e 6773 2532  ew%20encodings%2
+00000500: 3061 6e64 2532 3070 726f 7669 6469 6e67  0and%20providing
+00000510: 2532 3043 4c49 2532 3074 6f6f 6c73 2532  %20CLI%20tools%2
+00000520: 3077 6974 6825 3230 6125 3230 6775 6573  0with%20a%20gues
+00000530: 7325 3230 6665 6174 7572 6525 3230 6261  s%20feature%20ba
+00000540: 7365 6425 3230 6f6e 2532 3041 492e 2530  sed%20on%20AI.%0
+00000550: 4425 3041 6874 7470 7325 3361 2532 6625  D%0Ahttps%3a%2f%
+00000560: 3266 6769 7468 7562 2532 6563 6f6d 2532  2fgithub%2ecom%2
+00000570: 6664 686f 6e64 7461 2532 6670 7974 686f  fdhondta%2fpytho
+00000580: 6e2d 636f 6465 7874 2530 4425 3041 2668  n-codext%0D%0A&h
+00000590: 6173 6874 6167 733d 7079 7468 6f6e 2c70  ashtags=python,p
+000005a0: 726f 6772 616d 6d69 6e67 2c65 6e63 6f64  rogramming,encod
+000005b0: 696e 6773 2c63 6f64 6563 732c 6372 7970  ings,codecs,cryp
+000005c0: 746f 6772 6170 6879 2c6d 6f72 7365 2c62  tography,morse,b
+000005d0: 6173 652c 6374 6674 6f6f 6c73 223e 3c69  ase,ctftools"><i
+000005e0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+000005f0: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00000600: 6164 6765 2f54 7765 6574 2d2d 6c69 6768  adge/Tweet--ligh
+00000610: 7467 7265 793f 6c6f 676f 3d74 7769 7474  tgrey?logo=twitt
+00000620: 6572 2673 7479 6c65 3d73 6f63 6961 6c22  er&style=social"
+00000630: 2061 6c74 3d22 5477 6565 7422 2068 6569   alt="Tweet" hei
+00000640: 6768 743d 2232 3022 2f3e 3c2f 613e 3c2f  ght="20"/></a></
+00000650: 6831 3e0a 3c68 3320 616c 6967 6e3d 2263  h1>.<h3 align="c
+00000660: 656e 7465 7222 3e45 6e63 6f64 652f 6465  enter">Encode/de
+00000670: 636f 6465 2061 6e79 7468 696e 672e 3c2f  code anything.</
+00000680: 6833 3e0a 0a5b 215b 5079 5069 5d28 6874  h3>..[![PyPi](ht
+00000690: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000006a0: 732e 696f 2f70 7970 692f 762f 636f 6465  s.io/pypi/v/code
+000006b0: 7874 2e73 7667 295d 2868 7474 7073 3a2f  xt.svg)](https:/
+000006c0: 2f70 7970 692e 7079 7468 6f6e 2e6f 7267  /pypi.python.org
+000006d0: 2f70 7970 692f 636f 6465 7874 2f29 0a5b  /pypi/codext/).[
+000006e0: 215b 5265 6164 2054 6865 2044 6f63 735d  ![Read The Docs]
+000006f0: 2868 7474 7073 3a2f 2f72 6561 6474 6865  (https://readthe
+00000700: 646f 6373 2e6f 7267 2f70 726f 6a65 6374  docs.org/project
+00000710: 732f 7079 7468 6f6e 2d63 6f64 6578 742f  s/python-codext/
+00000720: 6261 6467 652f 3f76 6572 7369 6f6e 3d6c  badge/?version=l
+00000730: 6174 6573 7429 5d28 6874 7470 733a 2f2f  atest)](https://
+00000740: 7079 7468 6f6e 2d63 6f64 6578 742e 7265  python-codext.re
+00000750: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00000760: 6c61 7465 7374 2f3f 6261 6467 653d 6c61  latest/?badge=la
+00000770: 7465 7374 290a 5b21 5b42 7569 6c64 2053  test).[![Build S
+00000780: 7461 7475 735d 2868 7474 7073 3a2f 2f74  tatus](https://t
+00000790: 7261 7669 732d 6369 2e63 6f6d 2f64 686f  ravis-ci.com/dho
+000007a0: 6e64 7461 2f70 7974 686f 6e2d 636f 6465  ndta/python-code
+000007b0: 7874 2e73 7667 3f62 7261 6e63 683d 6d61  xt.svg?branch=ma
+000007c0: 7374 6572 295d 2868 7474 7073 3a2f 2f74  ster)](https://t
+000007d0: 7261 7669 732d 6369 2e63 6f6d 2f64 686f  ravis-ci.com/dho
+000007e0: 6e64 7461 2f70 7974 686f 6e2d 636f 6465  ndta/python-code
+000007f0: 7874 290a 5b21 5b43 6f76 6572 6167 6520  xt).[![Coverage 
+00000800: 5374 6174 7573 5d28 6874 7470 733a 2f2f  Status](https://
+00000810: 636f 7665 7261 6c6c 732e 696f 2f72 6570  coveralls.io/rep
+00000820: 6f73 2f67 6974 6875 622f 6468 6f6e 6474  os/github/dhondt
+00000830: 612f 7079 7468 6f6e 2d63 6f64 6578 742f  a/python-codext/
+00000840: 6261 6467 652e 7376 673f 6272 616e 6368  badge.svg?branch
+00000850: 3d6d 6173 7465 7229 5d28 6874 7470 733a  =master)](https:
+00000860: 2f2f 636f 7665 7261 6c6c 732e 696f 2f67  //coveralls.io/g
+00000870: 6974 6875 622f 6468 6f6e 6474 612f 7079  ithub/dhondta/py
+00000880: 7468 6f6e 2d63 6f64 6578 743f 6272 616e  thon-codext?bran
+00000890: 6368 3d6d 6173 7465 7229 0a5b 215b 5079  ch=master).[![Py
+000008a0: 7468 6f6e 2056 6572 7369 6f6e 735d 2868  thon Versions](h
+000008b0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000008c0: 6473 2e69 6f2f 7079 7069 2f70 7976 6572  ds.io/pypi/pyver
+000008d0: 7369 6f6e 732f 636f 6465 7874 2e73 7667  sions/codext.svg
+000008e0: 295d 2868 7474 7073 3a2f 2f70 7970 692e  )](https://pypi.
+000008f0: 7079 7468 6f6e 2e6f 7267 2f70 7970 692f  python.org/pypi/
+00000900: 636f 6465 7874 2f29 0a5b 215b 5265 7175  codext/).[![Requ
+00000910: 6972 656d 656e 7473 2053 7461 7475 735d  irements Status]
+00000920: 2868 7474 7073 3a2f 2f72 6571 7569 7265  (https://require
+00000930: 732e 696f 2f67 6974 6875 622f 6468 6f6e  s.io/github/dhon
+00000940: 6474 612f 7079 7468 6f6e 2d63 6f64 6578  dta/python-codex
+00000950: 742f 7265 7175 6972 656d 656e 7473 2e73  t/requirements.s
+00000960: 7667 3f62 7261 6e63 683d 6d61 7374 6572  vg?branch=master
+00000970: 295d 2868 7474 7073 3a2f 2f72 6571 7569  )](https://requi
+00000980: 7265 732e 696f 2f67 6974 6875 622f 6468  res.io/github/dh
+00000990: 6f6e 6474 612f 7079 7468 6f6e 2d63 6f64  ondta/python-cod
+000009a0: 6578 742f 7265 7175 6972 656d 656e 7473  ext/requirements
+000009b0: 2f3f 6272 616e 6368 3d6d 6173 7465 7229  /?branch=master)
+000009c0: 0a5b 215b 4b6e 6f77 6e20 5675 6c6e 6572  .[![Known Vulner
+000009d0: 6162 696c 6974 6965 735d 2868 7474 7073  abilities](https
+000009e0: 3a2f 2f73 6e79 6b2e 696f 2f74 6573 742f  ://snyk.io/test/
+000009f0: 6769 7468 7562 2f64 686f 6e64 7461 2f70  github/dhondta/p
+00000a00: 7974 686f 6e2d 636f 6465 7874 2f62 6164  ython-codext/bad
+00000a10: 6765 2e73 7667 3f74 6172 6765 7446 696c  ge.svg?targetFil
+00000a20: 653d 7265 7175 6972 656d 656e 7473 2e74  e=requirements.t
+00000a30: 7874 295d 2868 7474 7073 3a2f 2f73 6e79  xt)](https://sny
+00000a40: 6b2e 696f 2f74 6573 742f 6769 7468 7562  k.io/test/github
+00000a50: 2f64 686f 6e64 7461 2f70 7974 686f 6e2d  /dhondta/python-
+00000a60: 636f 6465 7874 3f74 6172 6765 7446 696c  codext?targetFil
+00000a70: 653d 7265 7175 6972 656d 656e 7473 2e74  e=requirements.t
+00000a80: 7874 290a 5b21 5b4c 6963 656e 7365 5d28  xt).[![License](
+00000a90: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000aa0: 6c64 732e 696f 2f70 7970 692f 6c2f 636f  lds.io/pypi/l/co
+00000ab0: 6465 7874 2e73 7667 295d 2868 7474 7073  dext.svg)](https
+00000ac0: 3a2f 2f70 7970 692e 7079 7468 6f6e 2e6f  ://pypi.python.o
+00000ad0: 7267 2f70 7970 692f 636f 6465 7874 2f29  rg/pypi/codext/)
+00000ae0: 0a0a 5468 6973 206c 6962 7261 7279 2065  ..This library e
+00000af0: 7874 656e 6473 2074 6865 206e 6174 6976  xtends the nativ
+00000b00: 6520 5b60 636f 6465 6373 605d 2868 7474  e [`codecs`](htt
+00000b10: 7073 3a2f 2f64 6f63 732e 7079 7468 6f6e  ps://docs.python
+00000b20: 2e6f 7267 2f33 2f6c 6962 7261 7279 2f63  .org/3/library/c
+00000b30: 6f64 6563 732e 6874 6d6c 2920 6c69 6272  odecs.html) libr
+00000b40: 6172 7920 286e 616d 656c 7920 666f 7220  ary (namely for 
+00000b50: 6164 6469 6e67 206e 6577 2063 7573 746f  adding new custo
+00000b60: 6d20 656e 636f 6469 6e67 7320 616e 6420  m encodings and 
+00000b70: 6368 6172 6163 7465 7220 6d61 7070 696e  character mappin
+00000b80: 6773 2920 616e 6420 7072 6f76 6964 6573  gs) and provides
+00000b90: 2061 206d 7972 6961 6420 6f66 206e 6577   a myriad of new
+00000ba0: 2065 6e63 6f64 696e 6773 2028 7374 6174   encodings (stat
+00000bb0: 6963 206f 7220 7061 7261 6d65 7472 697a  ic or parametriz
+00000bc0: 6564 2c20 6c69 6b65 2060 726f 7460 206f  ed, like `rot` o
+00000bd0: 7220 6078 6f72 6029 2c20 6865 6e63 6520  r `xor`), hence 
+00000be0: 6974 7320 6e61 6d65 6420 636f 6d62 696e  its named combin
+00000bf0: 696e 6720 2a43 4f44 6563 7320 4558 5465  ing *CODecs EXTe
+00000c00: 6e73 696f 6e2a 2e0a 0a60 6060 7368 0a24  nsion*...```sh.$
+00000c10: 2070 6970 2069 6e73 7461 6c6c 2063 6f64   pip install cod
+00000c20: 6578 740a 6060 600a 0a23 2320 3a6d 6167  ext.```..## :mag
+00000c30: 3a20 4465 6d6f 6e73 7472 6174 696f 6e73  : Demonstrations
+00000c40: 0a0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
+00000c50: 6572 223e 3c69 6d67 2073 7263 3d22 6874  er"><img src="ht
+00000c60: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00000c70: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000c80: 6468 6f6e 6474 612f 7079 7468 6f6e 2d63  dhondta/python-c
+00000c90: 6f64 6578 742f 6d61 7374 6572 2f64 6f63  odext/master/doc
+00000ca0: 732f 6465 6d6f 732f 7573 696e 672d 636f  s/demos/using-co
+00000cb0: 6465 7874 2e67 6966 2220 616c 743d 2255  dext.gif" alt="U
+00000cc0: 7369 6e67 2043 6f64 4578 7420 6672 6f6d  sing CodExt from
+00000cd0: 2074 6865 2063 6f6d 6d61 6e64 206c 696e   the command lin
+00000ce0: 6522 3e3c 2f70 3e0a 3c70 2061 6c69 676e  e"></p>.<p align
+00000cf0: 3d22 6365 6e74 6572 223e 3c69 6d67 2073  ="center"><img s
+00000d00: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+00000d10: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00000d20: 742e 636f 6d2f 6468 6f6e 6474 612f 7079  t.com/dhondta/py
+00000d30: 7468 6f6e 2d63 6f64 6578 742f 6d61 7374  thon-codext/mast
+00000d40: 6572 2f64 6f63 732f 6465 6d6f 732f 7573  er/docs/demos/us
+00000d50: 696e 672d 6261 7365 732e 6769 6622 2061  ing-bases.gif" a
+00000d60: 6c74 3d22 5573 696e 6720 6261 7365 2074  lt="Using base t
+00000d70: 6f6f 6c73 2066 726f 6d20 7468 6520 636f  ools from the co
+00000d80: 6d6d 616e 6420 6c69 6e65 223e 3c2f 703e  mmand line"></p>
+00000d90: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000da0: 7222 3e3c 696d 6720 7372 633d 2268 7474  r"><img src="htt
+00000db0: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00000dc0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f64  sercontent.com/d
+00000dd0: 686f 6e64 7461 2f70 7974 686f 6e2d 636f  hondta/python-co
+00000de0: 6465 7874 2f6d 6173 7465 722f 646f 6373  dext/master/docs
+00000df0: 2f64 656d 6f73 2f75 7369 6e67 2d64 6562  /demos/using-deb
+00000e00: 6173 652e 6769 6622 2061 6c74 3d22 5573  ase.gif" alt="Us
+00000e10: 696e 6720 7468 6520 6465 6261 7365 2063  ing the debase c
+00000e20: 6f6d 6d61 6e64 206c 696e 6520 746f 6f6c  ommand line tool
+00000e30: 223e 3c2f 703e 0a0a 2323 203a 636f 6d70  "></p>..## :comp
+00000e40: 7574 6572 3a20 5573 6167 6520 286d 6169  uter: Usage (mai
+00000e50: 6e20 434c 4920 746f 6f6c 2920 3c61 2068  n CLI tool) <a h
+00000e60: 7265 663d 2268 7474 7073 3a2f 2f74 7769  ref="https://twi
+00000e70: 7474 6572 2e63 6f6d 2f69 6e74 656e 742f  tter.com/intent/
+00000e80: 7477 6565 743f 7465 7874 3d43 6f64 4578  tweet?text=CodEx
+00000e90: 7425 3230 2d25 3230 456e 636f 6465 2532  t%20-%20Encode%2
+00000ea0: 4664 6563 6f64 6525 3230 616e 7974 6869  Fdecode%20anythi
+00000eb0: 6e67 2e25 3044 2530 4150 7974 686f 6e25  ng.%0D%0APython%
+00000ec0: 3230 746f 6f6c 2532 3066 6f72 2532 3065  20tool%20for%20e
+00000ed0: 6e63 6f64 696e 6725 3230 616e 6425 3230  ncoding%20and%20
+00000ee0: 6465 636f 6469 6e67 2532 3061 6c6d 6f73  decoding%20almos
+00000ef0: 7425 3230 616e 7974 6869 6e67 2c25 3230  t%20anything,%20
+00000f00: 696e 636c 7564 696e 6725 3230 6125 3230  including%20a%20
+00000f10: 6775 6573 7325 3230 6665 6174 7572 6525  guess%20feature%
+00000f20: 3230 6261 7365 6425 3230 6f6e 2532 3041  20based%20on%20A
+00000f30: 492e 2530 4425 3041 6874 7470 7325 3361  I.%0D%0Ahttps%3a
+00000f40: 2532 6625 3266 6769 7468 7562 2532 6563  %2f%2fgithub%2ec
+00000f50: 6f6d 2532 6664 686f 6e64 7461 2532 6670  om%2fdhondta%2fp
+00000f60: 7974 686f 6e2d 636f 6465 7874 2530 4425  ython-codext%0D%
+00000f70: 3041 2668 6173 6874 6167 733d 7079 7468  0A&hashtags=pyth
+00000f80: 6f6e 2c65 6e63 6f64 696e 6773 2c63 6f64  on,encodings,cod
+00000f90: 6563 732c 6372 7970 746f 6772 6170 6879  ecs,cryptography
+00000fa0: 2c6d 6f72 7365 2c62 6173 652c 7374 6567  ,morse,base,steg
+00000fb0: 616e 6f2c 7374 6567 616e 6f67 7261 7068  ano,steganograph
+00000fc0: 792c 6374 6674 6f6f 6c73 223e 3c69 6d67  y,ctftools"><img
+00000fd0: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00000fe0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00000ff0: 6765 2f54 7765 6574 2532 3028 636f 6465  ge/Tweet%20(code
+00001000: 7874 292d 2d6c 6967 6874 6772 6579 3f6c  xt)--lightgrey?l
+00001010: 6f67 6f3d 7477 6974 7465 7226 7374 796c  ogo=twitter&styl
+00001020: 653d 736f 6369 616c 2220 616c 743d 2254  e=social" alt="T
+00001030: 7765 6574 206f 6e20 636f 6465 7874 2220  weet on codext" 
+00001040: 6865 6967 6874 3d22 3230 222f 3e3c 2f61  height="20"/></a
+00001050: 3e0a 0a60 6060 7365 7373 696f 6e0a 2420  >..```session.$ 
+00001060: 636f 6465 7874 202d 6920 7465 7374 2e74  codext -i test.t
+00001070: 7874 2065 6e63 6f64 6520 646e 612d 310a  xt encode dna-1.
+00001080: 4754 4741 4743 4747 4754 4154 4754 4741  GTGAGCGGGTATGTGA
+00001090: 0a0a 2420 6563 686f 202d 656e 2022 7465  ..$ echo -en "te
+000010a0: 7374 2220 7c20 636f 6465 7874 2065 6e63  st" | codext enc
+000010b0: 6f64 6520 6d6f 7273 650a 2d20 2e20 2e2e  ode morse.- . ..
+000010c0: 2e20 2d0a 0a24 2065 6368 6f20 2d65 6e20  . -..$ echo -en 
+000010d0: 2274 6573 7422 207c 2063 6f64 6578 7420  "test" | codext 
+000010e0: 656e 636f 6465 2062 7261 696c 6c65 0ae2  encode braille..
+000010f0: a09e e2a0 91e2 a08e e2a0 9e0a 0a24 2065  .............$ e
+00001100: 6368 6f20 2d65 6e20 2274 6573 7422 207c  cho -en "test" |
+00001110: 2063 6f64 6578 7420 656e 636f 6465 2062   codext encode b
+00001120: 6173 6531 3030 0af0 9f91 abf0 9f91 9cf0  ase100..........
+00001130: 9f91 aaf0 9f91 ab0a 6060 600a 0a43 6861  ........```..Cha
+00001140: 696e 696e 6720 636f 6465 6373 3a0a 0a60  ining codecs:..`
+00001150: 6060 7368 0a24 2065 6368 6f20 2d65 6e20  ``sh.$ echo -en 
+00001160: 2254 6573 7420 7374 7269 6e67 2220 7c20  "Test string" | 
+00001170: 636f 6465 7874 2065 6e63 6f64 6520 7265  codext encode re
+00001180: 7665 7273 650a 676e 6972 7473 2074 7365  verse.gnirts tse
+00001190: 540a 0a24 2065 6368 6f20 2d65 6e20 2254  T..$ echo -en "T
+000011a0: 6573 7420 7374 7269 6e67 2220 7c20 636f  est string" | co
+000011b0: 6465 7874 2065 6e63 6f64 6520 7265 7665  dext encode reve
+000011c0: 7273 6520 6d6f 7273 650a 2d2d 2e20 2d2e  rse morse.--. -.
+000011d0: 202e 2e20 2e2d 2e20 2d20 2e2e 2e20 2f20   .. .-. - ... / 
+000011e0: 2d20 2e2e 2e20 2e20 2d0a 0a24 2065 6368  - ... . -..$ ech
+000011f0: 6f20 2d65 6e20 2254 6573 7420 7374 7269  o -en "Test stri
+00001200: 6e67 2220 7c20 636f 6465 7874 2065 6e63  ng" | codext enc
+00001210: 6f64 6520 7265 7665 7273 6520 6d6f 7273  ode reverse mors
+00001220: 6520 646e 612d 320a 4147 5443 4147 5443  e dna-2.AGTCAGTC
+00001230: 4147 5447 4147 4141 4147 5443 4147 5447  AGTGAGAAAGTCAGTG
+00001240: 4147 4141 4147 5447 4147 5447 4147 4141  AGAAAGTGAGTGAGAA
+00001250: 4147 5447 4147 5443 4147 5447 4147 4141  AGTGAGTCAGTGAGAA
+00001260: 4147 5443 4147 4141 4147 5447 4147 5447  AGTCAGAAAGTGAGTG
+00001270: 4147 5447 4147 4141 4147 5454 4147 4141  AGTGAGAAAGTTAGAA
+00001280: 4147 5443 4147 4141 4147 5447 4147 5447  AGTCAGAAAGTGAGTG
+00001290: 4147 5447 4147 4141 4147 5447 4147 4141  AGTGAGAAAGTGAGAA
+000012a0: 4147 5443 0a0a 2420 6563 686f 202d 656e  AGTC..$ echo -en
+000012b0: 2022 5465 7374 2073 7472 696e 6722 207c   "Test string" |
+000012c0: 2063 6f64 6578 7420 656e 636f 6465 2072   codext encode r
+000012d0: 6576 6572 7365 206d 6f72 7365 2064 6e61  everse morse dna
+000012e0: 2d32 206f 6374 616c 0a31 3031 3130 3731  -2 octal.1011071
+000012f0: 3234 3130 3331 3031 3130 3731 3234 3130  2410310110712410
+00001300: 3331 3031 3130 3731 3234 3130 3731 3031  3101107124107101
+00001310: 3130 3731 3031 3130 3131 3031 3130 3731  1071011011011071
+00001320: 3234 3130 3331 3031 3130 3731 3234 3130  2410310110712410
+00001330: 3731 3031 3130 3731 3031 3130 3131 3031  7101107101101101
+00001340: 3130 3731 3234 3130 3731 3031 3130 3731  1071241071011071
+00001350: 3234 3130 3731 3031 3130 3731 3031 3130  2410710110710110
+00001360: 3131 3031 3130 3731 3234 3130 3731 3031  1101107124107101
+00001370: 3130 3731 3234 3130 3331 3031 3130 3731  1071241031011071
+00001380: 3234 3130 3731 3031 3130 3731 3031 3130  2410710110710110
+00001390: 3131 3031 3130 3731 3234 3130 3331 3031  1101107124103101
+000013a0: 3130 3731 3031 3130 3131 3031 3130 3731  1071011011011071
+000013b0: 3234 3130 3731 3031 3130 3731 3234 3130  2410710110712410
+000013c0: 3731 3031 3130 3731 3234 3130 3731 3031  7101107124107101
+000013d0: 3130 3731 3031 3130 3131 3031 3130 3731  1071011011011071
+000013e0: 3234 3132 3431 3031 3130 3731 3031 3130  2412410110710110
+000013f0: 3131 3031 3130 3731 3234 3130 3331 3031  1101107124103101
+00001400: 3130 3731 3031 3130 3131 3031 3130 3731  1071011011011071
+00001410: 3234 3130 3731 3031 3130 3731 3234 3130  2410710110712410
+00001420: 3731 3031 3130 3731 3234 3130 3731 3031  7101107124107101
+00001430: 3130 3731 3031 3130 3131 3031 3130 3731  1071011011011071
+00001440: 3234 3130 3731 3031 3130 3731 3031 3130  2410710110710110
+00001450: 3131 3031 3130 3731 3234 3130 330a 0a24  1101107124103..$
+00001460: 2065 6368 6f20 2d65 6e20 2241 4754 4341   echo -en "AGTCA
+00001470: 4754 4341 4754 4741 4741 4141 4754 4341  GTCAGTGAGAAAGTCA
+00001480: 4754 4741 4741 4141 4754 4741 4754 4741  GTGAGAAAGTGAGTGA
+00001490: 4741 4141 4754 4741 4754 4341 4754 4741  GAAAGTGAGTCAGTGA
+000014a0: 4741 4141 4754 4341 4741 4141 4754 4741  GAAAGTCAGAAAGTGA
+000014b0: 4754 4741 4754 4741 4741 4141 4754 5441  GTGAGTGAGAAAGTTA
+000014c0: 4741 4141 4754 4341 4741 4141 4754 4741  GAAAGTCAGAAAGTGA
+000014d0: 4754 4741 4754 4741 4741 4141 4754 4741  GTGAGTGAGAAAGTGA
+000014e0: 4741 4141 4754 4322 207c 2063 6f64 6578  GAAAGTC" | codex
+000014f0: 7420 2d64 2064 6e61 2d32 206d 6f72 7365  t -d dna-2 morse
+00001500: 2072 6576 6572 7365 0a74 6573 7420 7374   reverse.test st
+00001510: 7269 6e67 0a60 6060 0a0a 2323 203a 636f  ring.```..## :co
+00001520: 6d70 7574 6572 3a20 5573 6167 6520 2862  mputer: Usage (b
+00001530: 6173 6520 434c 4920 746f 6f6c 2920 3c61  ase CLI tool) <a
+00001540: 2068 7265 663d 2268 7474 7073 3a2f 2f74   href="https://t
+00001550: 7769 7474 6572 2e63 6f6d 2f69 6e74 656e  witter.com/inten
+00001560: 742f 7477 6565 743f 7465 7874 3d44 6562  t/tweet?text=Deb
+00001570: 6173 6525 3230 2d25 3230 4465 636f 6465  ase%20-%20Decode
+00001580: 2532 3061 6e79 2532 306d 756c 7469 2d6c  %20any%20multi-l
+00001590: 6179 6572 2532 3062 6173 652d 656e 636f  ayer%20base-enco
+000015a0: 6465 6425 3230 7374 7269 6e67 2e25 3044  ded%20string.%0D
+000015b0: 2530 4150 7974 686f 6e25 3230 746f 6f6c  %0APython%20tool
+000015c0: 2532 3066 6f72 2532 3064 6563 6f64 696e  %20for%20decodin
+000015d0: 6725 3230 616e 7925 3230 6261 7365 2d65  g%20any%20base-e
+000015e0: 6e63 6f64 6564 2532 3073 7472 696e 672c  ncoded%20string,
+000015f0: 2532 3065 7665 6e25 3230 7768 656e 2532  %20even%20when%2
+00001600: 3065 6e63 6f64 6564 2532 3077 6974 6825  0encoded%20with%
+00001610: 3230 6d75 6c74 6970 6c65 2532 306c 6179  20multiple%20lay
+00001620: 6572 732e 2530 4425 3041 6874 7470 7325  ers.%0D%0Ahttps%
+00001630: 3361 2532 6625 3266 6769 7468 7562 2532  3a%2f%2fgithub%2
+00001640: 6563 6f6d 2532 6664 686f 6e64 7461 2532  ecom%2fdhondta%2
+00001650: 6670 7974 686f 6e2d 636f 6465 7874 2530  fpython-codext%0
+00001660: 4425 3041 2668 6173 6874 6167 733d 7079  D%0A&hashtags=py
+00001670: 7468 6f6e 2c62 6173 652c 656e 636f 6469  thon,base,encodi
+00001680: 6e67 732c 636f 6465 6373 2c63 7279 7074  ngs,codecs,crypt
+00001690: 6f67 7261 7068 792c 7374 6567 616e 6f2c  ography,stegano,
+000016a0: 7374 6567 616e 6f67 7261 7068 792c 6374  steganography,ct
+000016b0: 6674 6f6f 6c73 223e 3c69 6d67 2073 7263  ftools"><img src
+000016c0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+000016d0: 6965 6c64 732e 696f 2f62 6164 6765 2f54  ields.io/badge/T
+000016e0: 7765 6574 2532 3028 6465 6261 7365 292d  weet%20(debase)-
+000016f0: 2d6c 6967 6874 6772 6579 3f6c 6f67 6f3d  -lightgrey?logo=
+00001700: 7477 6974 7465 7226 7374 796c 653d 736f  twitter&style=so
+00001710: 6369 616c 2220 616c 743d 2254 7765 6574  cial" alt="Tweet
+00001720: 206f 6e20 6465 6261 7365 2220 6865 6967   on debase" heig
+00001730: 6874 3d22 3230 222f 3e3c 2f61 3e0a 0a60  ht="20"/></a>..`
+00001740: 6060 7365 7373 696f 6e0a 2420 6563 686f  ``session.$ echo
+00001750: 2022 5465 7374 2073 7472 696e 6720 2122   "Test string !"
+00001760: 207c 2062 6173 6531 3232 0a2a 2e37 2166   | base122.*.7!f
+00001770: 7439 efbf bd2d 6639 c382 0a0a 2420 6563  t9...-f9....$ ec
+00001780: 686f 2022 5465 7374 2073 7472 696e 6720  ho "Test string 
+00001790: 2122 207c 2062 6173 6539 3120 0a22 4f4e  !" | base91 ."ON
+000017a0: 4b3b 5744 5a4d 255a 2578 4537 4c0a 0a24  K;WDZM%Z%xE7L..$
+000017b0: 2065 6368 6f20 2254 6573 7420 7374 7269   echo "Test stri
+000017c0: 6e67 2021 2220 7c20 6261 7365 3931 207c  ng !" | base91 |
+000017d0: 2062 6173 6538 350a 4232 507c 424a 3641   base85.B2P|BJ6A
+000017e0: 2b6e 4f28 6a7c 2d63 7474 6c25 0a0a 2420  +nO(j|-cttl%..$ 
+000017f0: 6563 686f 2022 5465 7374 2073 7472 696e  echo "Test strin
+00001800: 6720 2122 207c 2062 6173 6539 3120 7c20  g !" | base91 | 
+00001810: 6261 7365 3835 207c 2062 6173 6533 3620  base85 | base36 
+00001820: 7c20 6261 7365 3538 2d66 6c69 636b 720a  | base58-flickr.
+00001830: 5156 7835 7476 676a 7643 416b 5861 4d53  QVx5tvgjvCAkXaMS
+00001840: 754b 6f51 6d43 6e6a 6543 5631 5979 7952  uKoQmCnjeCV1YyyR
+00001850: 3357 4572 5555 4572 4666 0a0a 2420 6563  3WErUUErFf..$ ec
+00001860: 686f 2022 5465 7374 2073 7472 696e 6720  ho "Test string 
+00001870: 2122 207c 2062 6173 6539 3120 7c20 6261  !" | base91 | ba
+00001880: 7365 3835 207c 2062 6173 6533 3620 7c20  se85 | base36 | 
+00001890: 6261 7365 3538 2d66 6c69 636b 7220 7c20  base58-flickr | 
+000018a0: 6261 7365 3538 2d66 6c69 636b 7220 2d64  base58-flickr -d
+000018b0: 207c 2062 6173 6533 3620 2d64 207c 2062   | base36 -d | b
+000018c0: 6173 6538 3520 2d64 207c 2062 6173 6539  ase85 -d | base9
+000018d0: 3120 2d64 0a54 6573 7420 7374 7269 6e67  1 -d.Test string
+000018e0: 2021 0a60 6060 0a0a 6060 6073 6573 7369   !.```..```sessi
+000018f0: 6f6e 0a24 2065 6368 6f20 2254 6573 7420  on.$ echo "Test 
+00001900: 7374 7269 6e67 2021 2220 7c20 6261 7365  string !" | base
+00001910: 3931 207c 2062 6173 6538 3520 7c20 6261  91 | base85 | ba
+00001920: 7365 3336 207c 2062 6173 6535 382d 666c  se36 | base58-fl
+00001930: 6963 6b72 207c 2064 6562 6173 6520 2d6d  ickr | debase -m
+00001940: 2033 0a54 6573 7420 7374 7269 6e67 2021   3.Test string !
+00001950: 0a0a 2420 6563 686f 2022 5465 7374 2073  ..$ echo "Test s
+00001960: 7472 696e 6720 2122 207c 2062 6173 6539  tring !" | base9
+00001970: 3120 7c20 6261 7365 3835 207c 2062 6173  1 | base85 | bas
+00001980: 6533 3620 7c20 6261 7365 3538 2d66 6c69  e36 | base58-fli
+00001990: 636b 7220 7c20 6465 6261 7365 202d 6620  ckr | debase -f 
+000019a0: 5465 7374 0a54 6573 7420 7374 7269 6e67  Test.Test string
+000019b0: 2021 0a60 6060 0a0a 2323 203a 636f 6d70   !.```..## :comp
+000019c0: 7574 6572 3a20 5573 6167 6520 2850 7974  uter: Usage (Pyt
+000019d0: 686f 6e29 0a0a 4765 7474 696e 6720 7468  hon)..Getting th
+000019e0: 6520 6c69 7374 206f 6620 6176 6169 6c61  e list of availa
+000019f0: 626c 6520 636f 6465 6373 3a0a 0a60 6060  ble codecs:..```
+00001a00: 7079 7468 6f6e 0a3e 3e3e 2069 6d70 6f72  python.>>> impor
+00001a10: 7420 636f 6465 7874 0a0a 3e3e 3e20 636f  t codext..>>> co
+00001a20: 6465 7874 2e6c 6973 7428 290a 5b27 6173  dext.list().['as
+00001a30: 6369 6938 3527 2c20 2762 6173 6538 3527  cii85', 'base85'
+00001a40: 2c20 2762 6173 6531 3030 272c 2027 6261  , 'base100', 'ba
+00001a50: 7365 3132 3227 2c20 2e2e 2e2c 2027 746f  se122', ..., 'to
+00001a60: 6d74 6f6d 272c 2027 646e 6127 2c20 2768  mtom', 'dna', 'h
+00001a70: 746d 6c27 2c20 276d 6172 6b64 6f77 6e27  tml', 'markdown'
+00001a80: 2c20 2775 726c 272c 2027 7265 7369 7374  , 'url', 'resist
+00001a90: 6f72 272c 2027 736d 7327 2c20 2777 6869  or', 'sms', 'whi
+00001aa0: 7465 7370 6163 6527 2c20 2777 6869 7465  tespace', 'white
+00001ab0: 7370 6163 652d 6166 7465 722d 6265 666f  space-after-befo
+00001ac0: 7265 275d 0a0a 3e3e 3e20 636f 6465 7874  re']..>>> codext
+00001ad0: 2e65 6e63 6f64 6528 2274 6869 7320 6973  .encode("this is
+00001ae0: 2061 2074 6573 7422 2c20 2262 6173 6535   a test", "base5
+00001af0: 382d 6269 7463 6f69 6e22 290a 276a 6f39  8-bitcoin").'jo9
+00001b00: 3177 614c 5141 314e 4e65 426d 5a4b 5546  1waLQA1NNeBmZKUF
+00001b10: 270a 0a3e 3e3e 2063 6f64 6578 742e 656e  '..>>> codext.en
+00001b20: 636f 6465 2822 7468 6973 2069 7320 6120  code("this is a 
+00001b30: 7465 7374 222c 2022 6261 7365 3538 2d72  test", "base58-r
+00001b40: 6970 706c 6522 290a 276a 6f39 7241 324c  ipple").'jo9rA2L
+00001b50: 5177 7234 3465 426d 5a4b 3745 270a 0a3e  Qwr44eBmZK7E'..>
+00001b60: 3e3e 2063 6f64 6578 742e 656e 636f 6465  >> codext.encode
+00001b70: 2822 7468 6973 2069 7320 6120 7465 7374  ("this is a test
+00001b80: 222c 2022 6261 7365 3538 2d75 726c 2229  ", "base58-url")
+00001b90: 0a27 4a4e 3931 577a 6b70 6131 6e6e 4462  .'JN91Wzkpa1nnDb
+00001ba0: 4c79 6a74 6627 0a0a 3e3e 3e20 636f 6465  Lyjtf'..>>> code
+00001bb0: 6373 2e65 6e63 6f64 6528 2274 6869 7320  cs.encode("this 
+00001bc0: 6973 2061 2074 6573 7422 2c20 2262 6173  is a test", "bas
+00001bd0: 6531 3030 2229 0a27 f09f 91ab f09f 919f  e100").'........
+00001be0: f09f 91a0 f09f 91aa f09f 9097 f09f 91a0  ................
+00001bf0: f09f 91aa f09f 9097 f09f 9198 f09f 9097  ................
+00001c00: f09f 91ab f09f 919c f09f 91aa f09f 91ab  ................
+00001c10: 270a 0a3e 3e3e 2063 6f64 6563 732e 6465  '..>>> codecs.de
+00001c20: 636f 6465 2822 f09f 91ab f09f 919f f09f  code("..........
+00001c30: 91a0 f09f 91aa f09f 9097 f09f 91a0 f09f  ................
+00001c40: 91aa f09f 9097 f09f 9198 f09f 9097 f09f  ................
+00001c50: 91ab f09f 919c f09f 91aa f09f 91ab 222c  ..............",
+00001c60: 2022 6261 7365 3130 3022 290a 2774 6869   "base100").'thi
+00001c70: 7320 6973 2061 2074 6573 7427 0a0a 3e3e  s is a test'..>>
+00001c80: 3e20 666f 7220 6920 696e 2072 616e 6765  > for i in range
+00001c90: 2838 293a 0a20 2020 2020 2020 2070 7269  (8):.        pri
+00001ca0: 6e74 2863 6f64 6578 742e 656e 636f 6465  nt(codext.encode
+00001cb0: 2822 7468 6973 2069 7320 6120 7465 7374  ("this is a test
+00001cc0: 222c 2022 646e 612d 2564 2220 2520 2869  ", "dna-%d" % (i
+00001cd0: 202b 2031 2929 290a 4754 4741 4743 4341   + 1))).GTGAGCCA
+00001ce0: 4743 4347 4754 4154 4143 4141 4743 4347  GCCGGTATACAAGCCG
+00001cf0: 4754 4154 4143 4141 4743 4147 4143 4141  GTATACAAGCAGACAA
+00001d00: 4754 4741 4743 4747 4754 4154 4754 4741  GTGAGCGGGTATGTGA
+00001d10: 0a43 5443 4143 4747 4143 4747 4343 5441  .CTCACGGACGGCCTA
+00001d20: 5441 4741 4143 4747 4343 5441 5441 4741  TAGAACGGCCTATAGA
+00001d30: 4143 4741 4341 4741 4143 5443 4143 4743  ACGACAGAACTCACGC
+00001d40: 4343 5441 5443 5443 410a 4143 4147 4154  CCTATCTCA.ACAGAT
+00001d50: 5447 4154 5441 4143 4743 4754 4747 4154  TGATTAACGCGTGGAT
+00001d60: 5441 4143 4743 4754 4747 4154 4741 4754  TAACGCGTGGATGAGT
+00001d70: 4747 4143 4147 4154 4141 4143 4743 4143  GGACAGATAAACGCAC
+00001d80: 4147 0a41 4741 4341 5454 4341 5454 4141  AG.AGACATTCATTAA
+00001d90: 4743 4743 5443 4341 5454 4141 4743 4743  GCGCTCCATTAAGCGC
+00001da0: 5443 4341 5443 4143 5443 4341 4741 4341  TCCATCACTCCAGACA
+00001db0: 5441 4141 4743 4741 4741 430a 5443 5447  TAAAGCGAGAC.TCTG
+00001dc0: 5441 4147 5441 4154 5443 4743 4741 4747  TAAGTAATTCGCGAGG
+00001dd0: 5441 4154 5443 4743 4741 4747 5441 4754  TAATTCGCGAGGTAGT
+00001de0: 4741 4747 5443 5447 5441 5454 5443 4743  GAGGTCTGTATTTCGC
+00001df0: 5443 5447 0a54 4754 4354 4141 4354 4141  TCTG.TGTCTAACTAA
+00001e00: 5454 4743 4743 4143 4354 4141 5454 4743  TTGCGCACCTAATTGC
+00001e10: 4743 4143 4354 4143 5443 4143 4354 4754  GCACCTACTCACCTGT
+00001e20: 4354 4154 5454 4743 4754 4754 430a 4741  CTATTTGCGTGTC.GA
+00001e30: 4754 4743 4354 4743 4347 4741 5441 5443  GTGCCTGCCGGATATC
+00001e40: 5454 4743 4347 4741 5441 5443 5454 4743  TTGCCGGATATCTTGC
+00001e50: 5447 5443 5454 4741 4754 4743 4747 4741  TGTCTTGAGTGCGGGA
+00001e60: 5441 4741 4754 0a43 4143 5443 4747 5443  TAGAGT.CACTCGGTC
+00001e70: 4747 4343 4154 4154 4754 5443 4747 4343  GGCCATATGTTCGGCC
+00001e80: 4154 4154 4754 5443 4754 4354 4754 5443  ATATGTTCGTCTGTTC
+00001e90: 4143 5443 4743 4343 4154 4143 4143 540a  ACTCGCCCATACACT.
+00001ea0: 3e3e 3e20 636f 6465 7874 2e64 6563 6f64  >>> codext.decod
+00001eb0: 6528 2247 5447 4147 4343 4147 4343 4747  e("GTGAGCCAGCCGG
+00001ec0: 5441 5441 4341 4147 4343 4747 5441 5441  TATACAAGCCGGTATA
+00001ed0: 4341 4147 4341 4741 4341 4147 5447 4147  CAAGCAGACAAGTGAG
+00001ee0: 4347 4747 5441 5447 5447 4122 2c20 2264  CGGGTATGTGA", "d
+00001ef0: 6e61 2d31 2229 0a27 7468 6973 2069 7320  na-1").'this is 
+00001f00: 6120 7465 7374 270a 0a3e 3e3e 2063 6f64  a test'..>>> cod
+00001f10: 6563 732e 656e 636f 6465 2822 7468 6973  ecs.encode("this
+00001f20: 2069 7320 6120 7465 7374 222c 2022 6d6f   is a test", "mo
+00001f30: 7273 6522 290a 272d 202e 2e2e 2e20 2e2e  rse").'- .... ..
+00001f40: 202e 2e2e 202f 202e 2e20 2e2e 2e20 2f20   ... / .. ... / 
+00001f50: 2e2d 202f 202d 202e 202e 2e2e 202d 270a  .- / - . ... -'.
+00001f60: 0a3e 3e3e 2063 6f64 6563 732e 6465 636f  .>>> codecs.deco
+00001f70: 6465 2822 2d20 2e2e 2e2e 202e 2e20 2e2e  de("- .... .. ..
+00001f80: 2e20 2f20 2e2e 202e 2e2e 202f 202e 2d20  . / .. ... / .- 
+00001f90: 2f20 2d20 2e20 2e2e 2e20 2d22 2c20 226d  / - . ... -", "m
+00001fa0: 6f72 7365 2229 0a27 7468 6973 2069 7320  orse").'this is 
+00001fb0: 6120 7465 7374 270a 0a3e 3e3e 2077 6974  a test'..>>> wit
+00001fc0: 6820 6f70 656e 2822 6d6f 7273 652e 7478  h open("morse.tx
+00001fd0: 7422 2c20 2777 272c 2065 6e63 6f64 696e  t", 'w', encodin
+00001fe0: 673d 226d 6f72 7365 2229 2061 7320 663a  g="morse") as f:
+00001ff0: 0a09 662e 7772 6974 6528 2274 6869 7320  ..f.write("this 
+00002000: 6973 2061 2074 6573 7422 290a 3134 0a0a  is a test").14..
+00002010: 3e3e 3e20 7769 7468 206f 7065 6e28 226d  >>> with open("m
+00002020: 6f72 7365 2e74 7874 222c 656e 636f 6469  orse.txt",encodi
+00002030: 6e67 3d22 6d6f 7273 6522 2920 6173 2066  ng="morse") as f
+00002040: 3a0a 0966 2e72 6561 6428 290a 2774 6869  :..f.read().'thi
+00002050: 7320 6973 2061 2074 6573 7427 0a0a 3e3e  s is a test'..>>
+00002060: 3e20 636f 6465 7874 2e64 6563 6f64 6528  > codext.decode(
+00002070: 2222 220a 2020 2020 2020 3d20 2020 2020  """.      =     
+00002080: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00002090: 2020 2020 2020 5820 2020 2020 2020 2020        X         
+000020a0: 0a20 2020 3a20 2020 2020 2020 2020 2020  .   :           
+000020b0: 200a 2020 2020 2020 7820 2020 2020 2020   .      x       
+000020c0: 2020 0a20 206e 2020 0a20 2020 2072 200a    .  n  .    r .
+000020d0: 2020 2020 2020 2020 7920 2020 0a20 2020          y   .   
+000020e0: 2020 2059 2020 2020 2020 2020 2020 2020     Y            
+000020f0: 0a20 2020 2020 2020 2020 2020 2020 2079  .              y
+00002100: 2020 2020 2020 2020 0a20 2020 2020 7020          .     p 
+00002110: 2020 200a 2020 2020 2020 2020 2061 2020     .         a  
+00002120: 2020 2020 200a 2060 2020 2020 2020 2020       . `        
+00002130: 2020 0a20 2020 2020 2020 2020 2020 206e    .            n
+00002140: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+00002150: 2020 2020 2020 207c 2020 2020 0a20 2061         |    .  a
+00002160: 2020 2020 2020 2020 2020 0a6f 2020 2020            .o    
+00002170: 0a20 2020 2020 2020 6820 2020 2020 2020  .       h       
+00002180: 200a 2020 2020 2020 2020 2020 6020 2020   .          `   
+00002190: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+000021a0: 2020 2020 6720 2020 2020 2020 2020 2020      g           
+000021b0: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
+000021c0: 6f20 0a20 2020 7a20 2020 2020 2022 2222  o .   z      """
+000021d0: 2c20 2277 6869 7465 7370 6163 652d 6166  , "whitespace-af
+000021e0: 7465 722b 6265 666f 7265 2229 0a27 4353  ter+before").'CS
+000021f0: 437b 6e6f 745f 736f 5f69 6e76 6973 6962  C{not_so_invisib
+00002200: 6c65 7d27 0a0a 3e3e 3e20 7072 696e 7428  le}'..>>> print(
+00002210: 636f 6465 7874 2e65 6e63 6f64 6528 2241  codext.encode("A
+00002220: 6e20 6578 616d 706c 6520 7465 7374 2073  n example test s
+00002230: 7472 696e 6722 2c20 2262 6175 646f 742d  tring", "baudot-
+00002240: 7461 7065 2229 290a 2a2a 2a2e 2a2a 0a20  tape")).***.**. 
+00002250: 2020 2e20 2a0a 2a2a 2a2e 2a20 0a2a 2020    . *.***.* .*  
+00002260: 2e20 200a 2020 202e 2a20 0a2a 2020 2e2a  .  .   .* .*  .*
+00002270: 200a 2020 202e 202a 0a2a 2a20 2e2a 200a   .   . *.** .* .
+00002280: 2a2a 2a2e 2a2a 0a2a 2a20 2e2a 2a0a 2020  ***.**.** .**.  
+00002290: 202e 2a20 0a2a 2020 2e20 200a 2a20 2a2e   .* .*  .  .* *.
+000022a0: 202a 0a20 2020 2e2a 200a 2a20 2a2e 2020   *.   .* .* *.  
+000022b0: 0a2a 202a 2e20 2a0a 2a20 202e 2020 0a2a  .* *. *.*  .  .*
+000022c0: 202a 2e20 200a 2a20 2a2e 202a 0a2a 2a2a   *.  .* *. *.***
+000022d0: 2e20 200a 2020 2a2e 2a20 0a2a 2a2a 2e2a  .  .  *.* .***.*
+000022e0: 200a 202a 202e 2a20 0a60 6060 0a0a 2323   . * .* .```..##
+000022f0: 203a 7061 6765 5f77 6974 685f 6375 726c   :page_with_curl
+00002300: 3a20 4c69 7374 206f 6620 636f 6465 6373  : List of codecs
+00002310: 0a0a 2a2a 436f 6465 632a 2a20 7c20 2a2a  ..**Codec** | **
+00002320: 436f 6e76 6572 7369 6f6e 732a 2a20 7c20  Conversions** | 
+00002330: 2a2a 436f 6d6d 656e 742a 2a0a 3a2d 2d2d  **Comment**.:---
+00002340: 3a20 7c20 3a2d 2d2d 3a20 7c20 2d2d 2d0a  : | :---: | ---.
+00002350: 6061 317a 3236 6020 7c20 7465 7874 203c  `a1z26` | text <
+00002360: 2d3e 2061 6c70 6861 6265 7420 6f72 6465  -> alphabet orde
+00002370: 7220 6e75 6d62 6572 7320 7c20 6b65 6570  r numbers | keep
+00002380: 7320 776f 7264 7320 7768 6974 6573 7061  s words whitespa
+00002390: 6365 2d73 6570 6172 6174 6564 2061 6e64  ce-separated and
+000023a0: 2075 7365 7320 6120 6375 7374 6f6d 2063   uses a custom c
+000023b0: 6861 7261 6374 6572 2073 6570 6172 6174  haracter separat
+000023c0: 6f72 0a60 6166 6669 6e65 6020 7c20 7465  or.`affine` | te
+000023d0: 7874 203c 2d3e 2061 6666 696e 6520 6369  xt <-> affine ci
+000023e0: 7068 6572 7465 7874 207c 2061 6b61 2041  phertext | aka A
+000023f0: 6666 696e 6520 4369 7068 6572 0a60 6173  ffine Cipher.`as
+00002400: 6369 6938 3560 207c 2074 6578 7420 3c2d  cii85` | text <-
+00002410: 3e20 6173 6369 6938 3520 656e 636f 6465  > ascii85 encode
+00002420: 6420 7465 7874 207c 2050 7974 686f 6e20  d text | Python 
+00002430: 3320 6f6e 6c79 0a60 6174 6261 7368 6020  3 only.`atbash` 
+00002440: 7c20 7465 7874 203c 2d3e 2041 7462 6173  | text <-> Atbas
+00002450: 6820 6369 7068 6572 7465 7874 207c 2061  h ciphertext | a
+00002460: 6b61 2041 7462 6173 6820 4369 7068 6572  ka Atbash Cipher
+00002470: 0a60 6261 636f 6e60 207c 2074 6578 7420  .`bacon` | text 
+00002480: 3c2d 3e20 4261 636f 6e20 6369 7068 6572  <-> Bacon cipher
+00002490: 7465 7874 207c 2061 6b61 2042 6163 6f6e  text | aka Bacon
+000024a0: 6961 6e20 4369 7068 6572 0a60 6261 7262  ian Cipher.`barb
+000024b0: 6965 2d4e 6020 7c20 7465 7874 203c 2d3e  ie-N` | text <->
+000024c0: 2062 6172 6269 6520 6369 7068 6572 7465   barbie cipherte
+000024d0: 7874 207c 2061 6b61 2042 6172 6269 6520  xt | aka Barbie 
+000024e0: 5479 7065 7772 6974 6572 2028 4e20 6265  Typewriter (N be
+000024f0: 6c6f 6e67 7320 746f 205b 312c 2034 5d29  longs to [1, 4])
+00002500: 0a60 6261 7365 5858 6020 7c20 7465 7874  .`baseXX` | text
+00002510: 203c 2d3e 2062 6173 6558 5820 7c20 7365   <-> baseXX | se
+00002520: 6520 5b62 6173 6520 656e 636f 6469 6e67  e [base encoding
+00002530: 735d 2868 7474 7073 3a2f 2f70 7974 686f  s](https://pytho
+00002540: 6e2d 636f 6465 7874 2e72 6561 6474 6865  n-codext.readthe
+00002550: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+00002560: 742f 656e 632f 6261 7365 2e68 746d 6c29  t/enc/base.html)
+00002570: 2028 696e 636c 2062 6173 6533 322c 2033   (incl base32, 3
+00002580: 362c 2034 352c 2035 382c 2036 322c 2036  6, 45, 58, 62, 6
+00002590: 332c 2036 342c 2039 312c 2031 3030 2c20  3, 64, 91, 100, 
+000025a0: 3132 3229 0a60 6261 7564 6f74 6020 7c20  122).`baudot` | 
+000025b0: 7465 7874 203c 2d3e 2042 6175 646f 7420  text <-> Baudot 
+000025c0: 636f 6465 2062 6974 7320 7c20 7375 7070  code bits | supp
+000025d0: 6f72 7473 2043 4349 5454 2d31 2c20 4343  orts CCITT-1, CC
+000025e0: 4954 542d 322c 2045 552f 4652 2c20 4954  ITT-2, EU/FR, IT
+000025f0: 4131 2c20 4954 4132 2c20 4d54 4b2d 3220  A1, ITA2, MTK-2 
+00002600: 2850 7974 686f 6e33 206f 6e6c 7929 2c20  (Python3 only), 
+00002610: 554b 2c20 2e2e 2e0a 6062 6364 6020 7c20  UK, ....`bcd` | 
+00002620: 7465 7874 203c 2d3e 2062 696e 6172 7920  text <-> binary 
+00002630: 636f 6465 6420 6465 6369 6d61 6c20 7465  coded decimal te
+00002640: 7874 207c 2065 6e63 6f64 6573 2063 6861  xt | encodes cha
+00002650: 7261 6374 6572 7320 6672 6f6d 2074 6865  racters from the
+00002660: 6972 2028 7a65 726f 2d6c 6566 742d 7061  ir (zero-left-pa
+00002670: 6464 6564 2920 6f72 6469 6e61 6c73 0a60  dded) ordinals.`
+00002680: 6272 6169 6c6c 6560 207c 2074 6578 7420  braille` | text 
+00002690: 3c2d 3e20 6272 6169 6c6c 6520 7379 6d62  <-> braille symb
+000026a0: 6f6c 7320 7c20 5079 7468 6f6e 2033 206f  ols | Python 3 o
+000026b0: 6e6c 790a 6063 6974 7269 7860 207c 2074  nly.`citrix` | t
+000026c0: 6578 7420 3c2d 3e20 4369 7472 6978 2043  ext <-> Citrix C
+000026d0: 5458 3120 6369 7068 6572 7465 7874 207c  TX1 ciphertext |
+000026e0: 2061 6b61 2043 6974 7269 7820 4354 5831   aka Citrix CTX1
+000026f0: 2070 6173 736f 7264 2065 6e63 6f64 696e   passord encodin
+00002700: 670a 6064 6e61 6020 7c20 7465 7874 203c  g.`dna` | text <
+00002710: 2d3e 2044 4e41 2d4e 2073 6571 7565 6e63  -> DNA-N sequenc
+00002720: 6520 7c20 696d 706c 656d 656e 7473 2074  e | implements t
+00002730: 6865 2038 2072 756c 6573 206f 6620 444e  he 8 rules of DN
+00002740: 4120 7365 7175 656e 6365 7320 284e 2062  A sequences (N b
+00002750: 656c 6f6e 6773 2074 6f20 5b31 2c38 5d29  elongs to [1,8])
+00002760: 0a60 6578 6365 7373 3360 207c 2074 6578  .`excess3` | tex
+00002770: 7420 3c2d 3e20 5853 3320 656e 636f 6465  t <-> XS3 encode
+00002780: 6420 7465 7874 207c 2075 7365 7320 4578  d text | uses Ex
+00002790: 6365 7373 2d33 2028 616b 6120 5374 6962  cess-3 (aka Stib
+000027a0: 6974 7a20 636f 6465 2920 6269 6e61 7279  itz code) binary
+000027b0: 2065 6e63 6f64 696e 6720 746f 2063 6f6e   encoding to con
+000027c0: 7665 7274 2063 6861 7261 6374 6572 7320  vert characters 
+000027d0: 6672 6f6d 2074 6865 6972 206f 7264 696e  from their ordin
+000027e0: 616c 730a 6067 7261 7960 207c 2074 6578  als.`gray` | tex
+000027f0: 7420 3c2d 3e20 6772 6179 2065 6e63 6f64  t <-> gray encod
+00002800: 6564 2074 6578 7420 7c20 616b 6120 7265  ed text | aka re
+00002810: 666c 6563 7465 6420 6269 6e61 7279 2063  flected binary c
+00002820: 6f64 650a 6067 7a69 7060 207c 2074 6578  ode.`gzip` | tex
+00002830: 7420 3c2d 3e20 477a 6970 2d63 6f6d 7072  t <-> Gzip-compr
+00002840: 6573 7365 6420 7465 7874 207c 2073 7461  essed text | sta
+00002850: 6e64 6172 6420 477a 6970 2063 6f6d 7072  ndard Gzip compr
+00002860: 6573 7369 6f6e 2f64 6563 6f6d 7072 6573  ession/decompres
+00002870: 7369 6f6e 0a60 6874 6d6c 6020 7c20 7465  sion.`html` | te
+00002880: 7874 203c 2d3e 2048 544d 4c20 656e 7469  xt <-> HTML enti
+00002890: 7469 6573 207c 2069 6d70 6c65 6d65 6e74  ties | implement
+000028a0: 7320 656e 7469 7469 6573 2061 6363 6f72  s entities accor
+000028b0: 6469 6e67 2074 6f20 5b74 6869 7320 7265  ding to [this re
+000028c0: 6665 7265 6e63 655d 2868 7474 7073 3a2f  ference](https:/
+000028d0: 2f64 6576 2e77 332e 6f72 672f 6874 6d6c  /dev.w3.org/html
+000028e0: 352f 6874 6d6c 2d61 7574 686f 722f 6368  5/html-author/ch
+000028f0: 6172 7265 6629 0a60 6970 7375 6d60 207c  arref).`ipsum` |
+00002900: 2074 6578 7420 3c2d 3e20 6c61 7469 6e20   text <-> latin 
+00002910: 776f 7264 7320 7c20 616b 6120 6c6f 7265  words | aka lore
+00002920: 6d20 6970 7375 6d0a 606b 6c6f 7066 6020  m ipsum.`klopf` 
+00002930: 7c20 7465 7874 203c 2d3e 206b 6c6f 7066  | text <-> klopf
+00002940: 2065 6e63 6f64 6564 2074 6578 7420 7c20   encoded text | 
+00002950: 506f 6c79 6269 7573 2073 7175 6172 6520  Polybius square 
+00002960: 7769 7468 2074 7269 7669 616c 2061 6c70  with trivial alp
+00002970: 6861 6265 7469 6361 6c20 6469 7374 7269  habetical distri
+00002980: 6275 7469 6f6e 0a60 6c65 6574 7370 6561  bution.`leetspea
+00002990: 6b60 207c 2074 6578 7420 3c2d 3e20 6c65  k` | text <-> le
+000029a0: 6574 7370 6561 6b20 656e 636f 6465 6420  etspeak encoded 
+000029b0: 7465 7874 207c 2062 6173 6564 206f 6e20  text | based on 
+000029c0: 6d69 6e69 6d61 6c69 7374 6963 2065 6c69  minimalistic eli
+000029d0: 7465 2073 7065 616b 696e 6720 7275 6c65  te speaking rule
+000029e0: 730a 606c 6574 7465 722d 696e 6469 6365  s.`letter-indice
+000029f0: 7360 207c 2074 6578 7420 3c2d 3e20 7465  s` | text <-> te
+00002a00: 7874 2077 6974 6820 6c65 7474 6572 2069  xt with letter i
+00002a10: 6e64 6963 6573 207c 2065 6e63 6f64 6573  ndices | encodes
+00002a20: 2063 6f6e 736f 6e61 6e74 7320 616e 642f   consonants and/
+00002a30: 6f72 2076 6f77 656c 7320 7769 7468 2074  or vowels with t
+00002a40: 6865 6972 2063 6f72 7265 7370 6f6e 6469  heir correspondi
+00002a50: 6e67 2069 6e64 6963 6573 0a60 6c7a 3737  ng indices.`lz77
+00002a60: 6020 7c20 7465 7874 203c 2d3e 204c 5a37  ` | text <-> LZ7
+00002a70: 372d 636f 6d70 7265 7373 6564 2074 6578  7-compressed tex
+00002a80: 7420 7c20 636f 6d70 7265 7373 6573 2074  t | compresses t
+00002a90: 6865 2067 6976 656e 2064 6174 6120 7769  he given data wi
+00002aa0: 7468 2074 6865 2061 6c67 6f72 6974 686d  th the algorithm
+00002ab0: 206f 6620 4c65 6d70 656c 2061 6e64 205a   of Lempel and Z
+00002ac0: 6976 206f 6620 3139 3737 0a60 6c7a 3738  iv of 1977.`lz78
+00002ad0: 6020 7c20 7465 7874 203c 2d3e 204c 5a37  ` | text <-> LZ7
+00002ae0: 382d 636f 6d70 7265 7373 6564 2074 6578  8-compressed tex
+00002af0: 7420 7c20 636f 6d70 7265 7373 6573 2074  t | compresses t
+00002b00: 6865 2067 6976 656e 2064 6174 6120 7769  he given data wi
+00002b10: 7468 2074 6865 2061 6c67 6f72 6974 686d  th the algorithm
+00002b20: 206f 6620 4c65 6d70 656c 2061 6e64 205a   of Lempel and Z
+00002b30: 6976 206f 6620 3139 3738 0a60 6d61 6e63  iv of 1978.`manc
+00002b40: 6865 7374 6572 6020 7c20 7465 7874 203c  hester` | text <
+00002b50: 2d3e 206d 616e 6368 6573 7465 7220 656e  -> manchester en
+00002b60: 636f 6465 6420 7465 7874 207c 2058 4f52  coded text | XOR
+00002b70: 6573 2065 6163 6820 6269 7420 6f66 2074  es each bit of t
+00002b80: 6865 2069 6e70 7574 2077 6974 6820 6030  he input with `0
+00002b90: 3160 0a60 6d61 726b 646f 776e 6020 7c20  1`.`markdown` | 
+00002ba0: 6d61 726b 646f 776e 202d 2d3e 2048 544d  markdown --> HTM
+00002bb0: 4c20 7c20 756e 6964 6972 6563 7469 6f6e  L | unidirection
+00002bc0: 616c 0a60 6d6f 7273 6560 207c 2074 6578  al.`morse` | tex
+00002bd0: 7420 3c2d 3e20 6d6f 7273 6520 656e 636f  t <-> morse enco
+00002be0: 6465 6420 7465 7874 207c 2075 7365 7320  ded text | uses 
+00002bf0: 7768 6974 6573 7061 6365 2061 7320 6120  whitespace as a 
+00002c00: 7365 7061 7261 746f 720a 606e 6176 616a  separator.`navaj
+00002c10: 6f60 207c 2074 6578 7420 3c2d 3e20 4e61  o` | text <-> Na
+00002c20: 7661 6a6f 207c 206f 6e6c 7920 6861 6e64  vajo | only hand
+00002c30: 6c65 7320 6c65 7474 6572 7320 286e 6f74  les letters (not
+00002c40: 2066 756c 6c20 776f 7264 7320 6672 6f6d   full words from
+00002c50: 2074 6865 204e 6176 616a 6f20 6469 6374   the Navajo dict
+00002c60: 696f 6e61 7279 290a 606f 6374 616c 6020  ionary).`octal` 
+00002c70: 7c20 7465 7874 203c 2d3e 206f 6374 616c  | text <-> octal
+00002c80: 2064 6967 6974 7320 7c20 6475 6d6d 7920   digits | dummy 
+00002c90: 6f63 7461 6c20 636f 6e76 6572 7369 6f6e  octal conversion
+00002ca0: 2028 636f 6e76 6572 7473 2074 6f20 332d   (converts to 3-
+00002cb0: 6469 6769 7473 2067 726f 7570 7329 0a60  digits groups).`
+00002cc0: 6f72 6469 6e61 6c60 207c 2074 6578 7420  ordinal` | text 
+00002cd0: 3c2d 3e20 6f72 6469 6e61 6c20 6469 6769  <-> ordinal digi
+00002ce0: 7473 207c 2064 756d 6d79 2063 6861 7261  ts | dummy chara
+00002cf0: 6374 6572 206f 7264 696e 616c 7320 636f  cter ordinals co
+00002d00: 6e76 6572 7369 6f6e 2028 636f 6e76 6572  nversion (conver
+00002d10: 7473 2074 6f20 332d 6469 6769 7473 2067  ts to 3-digits g
+00002d20: 726f 7570 7329 0a60 706b 7a69 705f 6465  roups).`pkzip_de
+00002d30: 666c 6174 6560 207c 2074 6578 7420 3c2d  flate` | text <-
+00002d40: 3e20 6465 666c 6174 6564 2074 6578 7420  > deflated text 
+00002d50: 7c20 7374 616e 6461 7264 205a 6970 2d64  | standard Zip-d
+00002d60: 6566 6c61 7465 2063 6f6d 7072 6573 7369  eflate compressi
+00002d70: 6f6e 2f64 6563 6f6d 7072 6573 7369 6f6e  on/decompression
+00002d80: 0a60 706b 7a69 705f 627a 6970 3260 207c  .`pkzip_bzip2` |
+00002d90: 2074 6578 7420 3c2d 3e20 427a 6970 7065   text <-> Bzippe
+00002da0: 6420 7465 7874 207c 2073 7461 6e64 6172  d text | standar
+00002db0: 6420 425a 6970 3220 636f 6d70 7265 7373  d BZip2 compress
+00002dc0: 696f 6e2f 6465 636f 6d70 7265 7373 696f  ion/decompressio
+00002dd0: 6e0a 6070 6b7a 6970 5f6c 7a6d 6160 207c  n.`pkzip_lzma` |
+00002de0: 2074 6578 7420 3c2d 3e20 4c5a 4d41 2d63   text <-> LZMA-c
+00002df0: 6f6d 7072 6573 7365 6420 7465 7874 207c  ompressed text |
+00002e00: 2073 7461 6e64 6172 6420 4c5a 4d41 2063   standard LZMA c
+00002e10: 6f6d 7072 6573 7369 6f6e 2f64 6563 6f6d  ompression/decom
+00002e20: 7072 6573 7369 6f6e 0a60 7261 6469 6f60  pression.`radio`
+00002e30: 207c 2074 6578 7420 3c2d 3e20 7261 6469   | text <-> radi
+00002e40: 6f20 776f 7264 7320 7c20 616b 6120 4e41  o words | aka NA
+00002e50: 544f 206f 7220 7261 6469 6f20 7068 6f6e  TO or radio phon
+00002e60: 6574 6963 2061 6c70 6861 6265 740a 6072  etic alphabet.`r
+00002e70: 6573 6973 746f 7260 207c 2074 6578 7420  esistor` | text 
+00002e80: 3c2d 3e20 7265 7369 7374 6f72 2063 6f6c  <-> resistor col
+00002e90: 6f72 7320 7c20 616b 6120 7265 7369 7374  ors | aka resist
+00002ea0: 6f72 2063 6f6c 6f72 2063 6f64 6573 0a60  or color codes.`
+00002eb0: 726f 7460 207c 2074 6578 7420 3c2d 3e20  rot` | text <-> 
+00002ec0: 726f 7428 4e29 2063 6970 6865 7274 6578  rot(N) ciphertex
+00002ed0: 7420 7c20 616b 6120 4361 6573 6172 2063  t | aka Caesar c
+00002ee0: 6970 6865 7220 284e 2062 656c 6f6e 6773  ipher (N belongs
+00002ef0: 2074 6f20 5b31 2c32 355d 290a 6072 6f74   to [1,25]).`rot
+00002f00: 6174 6560 207c 2074 6578 7420 3c2d 3e20  ate` | text <-> 
+00002f10: 4e2d 6269 7473 2d72 6f74 6174 6564 2074  N-bits-rotated t
+00002f20: 6578 7420 7c20 726f 7461 7465 7320 6368  ext | rotates ch
+00002f30: 6172 6163 7465 7273 2062 7920 7468 6520  aracters by the 
+00002f40: 7370 6563 6966 6965 6420 6e75 6d62 6572  specified number
+00002f50: 206f 6620 6269 7473 203b 2050 7974 686f   of bits ; Pytho
+00002f60: 6e20 3320 6f6e 6c79 0a60 7363 7974 616c  n 3 only.`scytal
+00002f70: 6560 207c 2074 6578 7420 3c2d 3e20 7363  e` | text <-> sc
+00002f80: 7974 616c 6520 6369 7068 6572 7465 7874  ytale ciphertext
+00002f90: 207c 2065 6e63 7279 7074 7320 7769 7468   | encrypts with
+00002fa0: 204c 2c20 7468 6520 6e75 6d62 6572 206f   L, the number o
+00002fb0: 6620 6c65 7474 6572 7320 6f6e 2074 6865  f letters on the
+00002fc0: 2072 6f64 2028 6265 6c6f 6e67 7320 746f   rod (belongs to
+00002fd0: 205b 312c 5b29 0a60 7368 6966 7460 207c   [1,[).`shift` |
+00002fe0: 2074 6578 7420 3c2d 3e20 7368 6966 7428   text <-> shift(
+00002ff0: 4e29 2063 6970 6865 7274 6578 7420 7c20  N) ciphertext | 
+00003000: 7368 6966 7420 6f72 6469 6e61 6c73 2077  shift ordinals w
+00003010: 6974 6820 4e20 2862 656c 6f6e 6773 2074  ith N (belongs t
+00003020: 6f20 5b31 2c32 3535 5d29 0a60 736d 7360  o [1,255]).`sms`
+00003030: 207c 2074 6578 7420 3c2d 3e20 7068 6f6e   | text <-> phon
+00003040: 6520 6b65 7973 7472 6f6b 6573 207c 2061  e keystrokes | a
+00003050: 6c73 6f20 6361 6c6c 6564 2054 3920 636f  lso called T9 co
+00003060: 6465 203b 2075 7365 7320 2260 2d60 2220  de ; uses "`-`" 
+00003070: 6173 2061 2073 6570 6172 6174 6f72 2066  as a separator f
+00003080: 6f72 2065 6e63 6f64 696e 672c 2022 602d  or encoding, "`-
+00003090: 6022 206f 7220 2260 5f60 2220 6f72 2077  `" or "`_`" or w
+000030a0: 6869 7465 7370 6163 6520 666f 7220 6465  hitespace for de
+000030b0: 636f 6469 6e67 0a60 736f 7574 6870 6172  coding.`southpar
+000030c0: 6b60 207c 2074 6578 7420 3c2d 3e20 4b65  k` | text <-> Ke
+000030d0: 6e6e 7927 7320 6c61 6e67 7561 6765 207c  nny's language |
+000030e0: 2063 6f6e 7665 7274 7320 6c65 7474 6572   converts letter
+000030f0: 7320 746f 204b 656e 6e79 2773 206c 616e  s to Kenny's lan
+00003100: 6775 6167 6520 6672 6f6d 2053 6f75 7468  guage from South
+00003110: 7061 726b 2028 7768 6974 6573 7061 6365  park (whitespace
+00003120: 2069 7320 616c 736f 2068 616e 646c 6564   is also handled
+00003130: 290a 6074 6f6d 746f 6d60 207c 2074 6578  ).`tomtom` | tex
+00003140: 7420 3c2d 3e20 746f 6d2d 746f 6d20 656e  t <-> tom-tom en
+00003150: 636f 6465 6420 7465 7874 207c 2073 696d  coded text | sim
+00003160: 696c 6172 2074 6f20 606d 6f72 7365 602c  ilar to `morse`,
+00003170: 2075 7369 6e67 2073 6c61 7368 6573 2061   using slashes a
+00003180: 6e64 2062 6163 6b73 6c61 7368 6573 0a60  nd backslashes.`
+00003190: 7572 6c60 207c 2074 6578 7420 3c2d 3e20  url` | text <-> 
+000031a0: 5552 4c20 656e 636f 6465 6420 7465 7874  URL encoded text
+000031b0: 207c 2061 6b61 2055 524c 2065 6e63 6f64   | aka URL encod
+000031c0: 696e 670a 6078 6f72 6020 7c20 7465 7874  ing.`xor` | text
+000031d0: 203c 2d3e 2058 4f52 284e 2920 6369 7068   <-> XOR(N) ciph
+000031e0: 6572 7465 7874 207c 2058 4f52 2077 6974  ertext | XOR wit
+000031f0: 6820 6120 7369 6e67 6c65 2062 7974 6520  h a single byte 
+00003200: 284e 2062 656c 6f6e 6773 2074 6f20 5b31  (N belongs to [1
+00003210: 2c32 3535 5d29 0a60 7768 6974 6573 7061  ,255]).`whitespa
+00003220: 6365 6020 7c20 7465 7874 203c 2d3e 2077  ce` | text <-> w
+00003230: 6869 7465 7370 6163 6573 2061 6e64 2074  hitespaces and t
+00003240: 6162 7320 7c20 7265 706c 6163 6573 2062  abs | replaces b
+00003250: 6974 7320 7769 7468 2077 6869 7465 7370  its with whitesp
+00003260: 6163 6573 2061 6e64 2074 6162 730a 0a41  aces and tabs..A
+00003270: 2066 6577 2076 6172 6961 6e74 7320 6172   few variants ar
+00003280: 6520 616c 736f 2069 6d70 6c65 6d65 6e74  e also implement
+00003290: 6564 2e0a 0a2a 2a43 6f64 6563 2a2a 207c  ed...**Codec** |
+000032a0: 202a 2a43 6f6e 7665 7273 696f 6e73 2a2a   **Conversions**
+000032b0: 207c 202a 2a43 6f6d 6d65 6e74 2a2a 0a3a   | **Comment**.:
+000032c0: 2d2d 2d3a 207c 203a 2d2d 2d3a 207c 202d  ---: | :---: | -
+000032d0: 2d2d 0a60 6261 7564 6f74 2d73 7061 6365  --.`baudot-space
+000032e0: 6460 207c 2074 6578 7420 3c2d 3e20 4261  d` | text <-> Ba
+000032f0: 7564 6f74 2063 6f64 6520 6772 6f75 7073  udot code groups
+00003300: 206f 6620 6269 7473 207c 2067 726f 7570   of bits | group
+00003310: 7320 6f66 2035 2062 6974 7320 6172 6520  s of 5 bits are 
+00003320: 7768 6974 6573 7061 6365 2d73 6570 6172  whitespace-separ
+00003330: 6174 6564 0a60 6261 7564 6f74 2d74 6170  ated.`baudot-tap
+00003340: 6560 207c 2074 6578 7420 3c2d 3e20 4261  e` | text <-> Ba
+00003350: 7564 6f74 2063 6f64 6520 7461 7065 207c  udot code tape |
+00003360: 206f 7574 7075 7473 2061 2073 7472 696e   outputs a strin
+00003370: 6720 7468 6174 206c 6f6f 6b73 206c 696b  g that looks lik
+00003380: 6520 6120 7065 7266 6f72 6174 6564 2074  e a perforated t
+00003390: 6170 650a 6062 6364 2d65 7874 656e 6465  ape.`bcd-extende
+000033a0: 6430 6020 7c20 7465 7874 203c 2d3e 2042  d0` | text <-> B
+000033b0: 4344 2d65 7874 656e 6465 6420 7465 7874  CD-extended text
+000033c0: 207c 2065 6e63 6f64 6573 2063 6861 7261   | encodes chara
+000033d0: 6374 6572 7320 6672 6f6d 2074 6865 6972  cters from their
+000033e0: 2028 7a65 726f 2d6c 6566 742d 7061 6464   (zero-left-padd
+000033f0: 6564 2920 6f72 6469 6e61 6c73 2075 7369  ed) ordinals usi
+00003400: 6e67 2070 7265 6669 7820 6269 7473 2060  ng prefix bits `
+00003410: 3030 3030 600a 6062 6364 2d65 7874 656e  0000`.`bcd-exten
+00003420: 6465 6431 6020 7c20 7465 7874 203c 2d3e  ded1` | text <->
+00003430: 2042 4344 2d65 7874 656e 6465 6420 7465   BCD-extended te
+00003440: 7874 207c 2065 6e63 6f64 6573 2063 6861  xt | encodes cha
+00003450: 7261 6374 6572 7320 6672 6f6d 2074 6865  racters from the
+00003460: 6972 2028 7a65 726f 2d6c 6566 742d 7061  ir (zero-left-pa
+00003470: 6464 6564 2920 6f72 6469 6e61 6c73 2075  dded) ordinals u
+00003480: 7369 6e67 2070 7265 6669 7820 6269 7473  sing prefix bits
+00003490: 2060 3131 3131 600a 606d 616e 6368 6573   `1111`.`manches
+000034a0: 7465 722d 696e 7665 7274 6564 6020 7c20  ter-inverted` | 
+000034b0: 7465 7874 203c 2d3e 206d 616e 6368 6573  text <-> manches
+000034c0: 7465 7220 656e 636f 6465 6420 7465 7874  ter encoded text
+000034d0: 207c 2058 4f52 6573 2065 6163 6820 6269   | XORes each bi
+000034e0: 7420 6f66 2074 6865 2069 6e70 7574 2077  t of the input w
+000034f0: 6974 6820 6031 3060 0a60 6f63 7461 6c2d  ith `10`.`octal-
+00003500: 7370 6163 6564 6020 7c20 7465 7874 203c  spaced` | text <
+00003510: 2d3e 206f 6374 616c 2064 6967 6974 7320  -> octal digits 
+00003520: 2877 6869 7465 7370 6163 652d 7365 7061  (whitespace-sepa
+00003530: 7261 7465 6429 207c 2064 756d 6d79 206f  rated) | dummy o
+00003540: 6374 616c 2063 6f6e 7665 7273 696f 6e0a  ctal conversion.
+00003550: 606f 7264 696e 616c 2d73 7061 6365 6460  `ordinal-spaced`
+00003560: 207c 2074 6578 7420 3c2d 3e20 6f72 6469   | text <-> ordi
+00003570: 6e61 6c20 6469 6769 7473 2028 7768 6974  nal digits (whit
+00003580: 6573 7061 6365 2d73 6570 6172 6174 6564  espace-separated
+00003590: 2920 7c20 6475 6d6d 7920 6368 6172 6163  ) | dummy charac
+000035a0: 7465 7220 6f72 6469 6e61 6c73 2063 6f6e  ter ordinals con
+000035b0: 7665 7273 696f 6e0a 6073 6f75 7468 7061  version.`southpa
+000035c0: 726b 2d69 6361 7365 6020 7c20 7465 7874  rk-icase` | text
+000035d0: 203c 2d3e 204b 656e 6e79 2773 206c 616e   <-> Kenny's lan
+000035e0: 6775 6167 6520 7c20 7361 6d65 2061 7320  guage | same as 
+000035f0: 6073 6f75 7468 7061 726b 6020 6275 7420  `southpark` but 
+00003600: 6361 7365 2069 6e73 656e 7369 7469 7665  case insensitive
+00003610: 0a60 7768 6974 6573 7061 6365 5f61 6674  .`whitespace_aft
+00003620: 6572 5f62 6566 6f72 6560 207c 2074 6578  er_before` | tex
+00003630: 7420 3c2d 3e20 6c69 6e65 7320 6f66 2077  t <-> lines of w
+00003640: 6869 7465 7370 6163 6573 5b6c 6574 7465  hitespaces[lette
+00003650: 725d 7768 6974 6573 7061 6365 7320 7c20  r]whitespaces | 
+00003660: 656e 636f 6465 7320 6368 6172 6163 7465  encodes characte
+00003670: 7273 2061 7320 6e65 7720 6368 6172 6163  rs as new charac
+00003680: 7465 7273 2077 6974 6820 7768 6974 6573  ters with whites
+00003690: 7061 6365 7320 6265 666f 7265 2061 6e64  paces before and
+000036a0: 2061 6674 6572 2061 6363 6f72 6469 6e67   after according
+000036b0: 2074 6f20 616e 2065 7175 6174 696f 6e20   to an equation 
+000036c0: 6465 7363 7269 6265 6420 696e 2074 6865  described in the
+000036d0: 2063 6f64 6563 206e 616d 6520 2865 2e67   codec name (e.g
+000036e0: 2e20 2260 7768 6974 6573 7061 6365 2b32  . "`whitespace+2
+000036f0: 2a61 6674 6572 2d33 2a62 6566 6f72 6560  *after-3*before`
+00003700: 2229 0a0a 0a23 2320 3a63 6c61 703a 2020  ")...## :clap:  
+00003710: 5375 7070 6f72 7465 7273 0a0a 5b21 5b53  Supporters..[![S
+00003720: 7461 7267 617a 6572 7320 7265 706f 2072  targazers repo r
+00003730: 6f73 7465 7220 666f 7220 4064 686f 6e64  oster for @dhond
+00003740: 7461 2f70 7974 686f 6e2d 636f 6465 7874  ta/python-codext
+00003750: 5d28 6874 7470 733a 2f2f 7265 706f 726f  ](https://reporo
+00003760: 7374 6572 2e63 6f6d 2f73 7461 7273 2f64  ster.com/stars/d
+00003770: 6172 6b2f 6468 6f6e 6474 612f 7079 7468  ark/dhondta/pyth
+00003780: 6f6e 2d63 6f64 6578 7429 5d28 6874 7470  on-codext)](http
+00003790: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+000037a0: 686f 6e64 7461 2f70 7974 686f 6e2d 636f  hondta/python-co
+000037b0: 6465 7874 2f73 7461 7267 617a 6572 7329  dext/stargazers)
+000037c0: 0a0a 5b21 5b46 6f72 6b65 7273 2072 6570  ..[![Forkers rep
+000037d0: 6f20 726f 7374 6572 2066 6f72 2040 6468  o roster for @dh
+000037e0: 6f6e 6474 612f 7079 7468 6f6e 2d63 6f64  ondta/python-cod
+000037f0: 6578 745d 2868 7474 7073 3a2f 2f72 6570  ext](https://rep
+00003800: 6f72 6f73 7465 722e 636f 6d2f 666f 726b  oroster.com/fork
+00003810: 732f 6461 726b 2f64 686f 6e64 7461 2f70  s/dark/dhondta/p
+00003820: 7974 686f 6e2d 636f 6465 7874 295d 2868  ython-codext)](h
+00003830: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00003840: 6d2f 6468 6f6e 6474 612f 7079 7468 6f6e  m/dhondta/python
+00003850: 2d63 6f64 6578 742f 6e65 7477 6f72 6b2f  -codext/network/
+00003860: 6d65 6d62 6572 7329 0a0a 3c70 2061 6c69  members)..<p ali
+00003870: 676e 3d22 6365 6e74 6572 223e 3c61 2068  gn="center"><a h
+00003880: 7265 663d 2223 223e 3c69 6d67 2073 7263  ref="#"><img src
+00003890: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+000038a0: 6965 6c64 732e 696f 2f62 6164 6765 2f42  ields.io/badge/B
+000038b0: 6163 6b25 3230 746f 2532 3074 6f70 2d2d  ack%20to%20top--
+000038c0: 6c69 6768 7467 7265 793f 7374 796c 653d  lightgrey?style=
+000038d0: 736f 6369 616c 2220 616c 743d 2242 6163  social" alt="Bac
+000038e0: 6b20 746f 2074 6f70 2220 6865 6967 6874  k to top" height
+000038f0: 3d22 3230 222f 3e3c 2f61 3e3c 2f70 3e0a  ="20"/></a></p>.
+00003900: 0a0a                                     ..
```

### Comparing `codext-1.9.4/codext.egg-info/SOURCES.txt` & `codext-1.9.5/codext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/codext.egg-info/entry_points.txt` & `codext-1.9.5/codext.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/setup.cfg` & `codext-1.9.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/tests/test_base.py` & `codext-1.9.5/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/tests/test_common.py` & `codext-1.9.5/tests/test_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,17 @@
 
 def getregentry(encoding):
     if encoding == "dummy3":
         return codecs.CodecInfo(name="dummy3", encode=dummy_encode, decode=dummy_decode)
 
 
 class TestCommon(TestCase):
+    def setUp(self):
+        codext.reset()
+    
     def test_add_codec(self):
         self.assertRaises(ValueError, codext.add, "test")
         self.assertRaises(ValueError, codext.add, "test", "BAD")
         self.assertRaises(ValueError, codext.add, "test", lambda: None, "BAD")
         self.assertIsNone(codext.add("dummy", dummy_encode, dummy_decode))
         self.assertEqual(codext.encode("test", "dummy"), "test")
         ci = codext.lookup("dummy")
@@ -75,15 +78,14 @@
         self.assertRaises(ValueError, codext.add_map, "dummy2", ENCMAP, intype="BAD")
         self.assertRaises(ValueError, codext.add_map, "dummy2", ENCMAP, outype="BAD")
         ci = codext.lookup("dummy2")
         for k in ["category", "encmap", "ignore_case", "intype", "no_error", "outype", "repl_char", "sep", "text"]:
             self.assertIn(k, ci.parameters.keys())
     
     def test_list_codecs(self):
-        codext.reset()
         self.assertTrue(len(codext.list()) > 0)
         self.assertTrue(len(codext.list("other")) > 0)
         self.assertTrue(len(codext.list("native")) > 0)
         self.assertTrue(len(codext.list("non-native")) > 0)
         self.assertTrue(len(codext.list("native", "non-native", "crypto", "base")) > 0)
         self.assertTrue(len(codext.list("native", "language", "crypto")) > 0)
         self.assertEqual(set(codext.list()), set(codext.list("native") + codext.list("non-native")))
@@ -125,17 +127,24 @@
         self.assertIsNotNone(list(codext.generate_strings_from_regex(r"[ab]{1,3}")))
         self.assertIsNotNone(list(codext.generate_strings_from_regex(r"(?<=ab)cd")))
         self.assertIsNotNone(list(codext.generate_strings_from_regex(r"(?<=-)\w+")))
         self.assertIsNotNone(list(codext.generate_strings_from_regex(r"([^\s])\1")))
         self.assertIsNotNone(list(codext.generate_strings_from_regex(r"[^\\]")))
         self.assertIsNotNone(list(codext.generate_strings_from_regex(r"[^a]")))
     
+    def test_encode_multiple_rounds(self):
+        self.assertRaises(TypeError, codext.encode, b"test", "utf-8[2]")
+        s = "test"
+        for i in range(3):
+            s = codext.encode(s, "morse")
+        self.assertEqual(s, codext.encode("test", "morse[3]"))
+        self.assertIsNotNone(codext.encode("test", "base64[10]"))
+    
     def test_guess_decode(self):
         _l = lambda d: list(d.items())[0][1] if len(d) > 0 else None
-        codext.reset()
         codext.add("test_codec", lambda x, e="strict": (x + "=", len(x)), lambda x, e="strict": (x[:-1], len(x)-1),
                    "test", no_error=True, bonus_func=lambda *a: True, penalty=-.5)
         self.assertIn("test-codec", codext.list_encodings("test"))
         STR = "This is a test"
         self.assertEqual(STR, _l(codext.guess("VGhpcyBpcyBhIHRlc3Q=", "a test", max_depth=1)))
         self.assertEqual(STR, _l(codext.guess("CJG3Ix8bVcSRMLOqwDUg28aDsT7", "a test", found=["base62"])))
         if hasattr(codext.stopfunc, "lang_en"):
```

### Comparing `codext-1.9.4/tests/test_generated.py` & `codext-1.9.5/tests/test_generated.py`

 * *Files identical despite different names*

### Comparing `codext-1.9.4/tests/test_manual.py` & `codext-1.9.5/tests/test_manual.py`

 * *Files identical despite different names*

