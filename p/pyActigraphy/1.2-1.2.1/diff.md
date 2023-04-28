# Comparing `tmp/pyActigraphy-1.2.tar.gz` & `tmp/pyActigraphy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyActigraphy-1.2.tar", last modified: Wed Mar 22 10:47:00 2023, max compression
+gzip compressed data, was "dist/pyActigraphy-1.2.1.tar", last modified: Fri Apr 28 08:52:41 2023, max compression
```

## Comparing `pyActigraphy-1.2.tar` & `pyActigraphy-1.2.1.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/
--rw-r--r--   0 ghammad    (501) staff       (20)    34728 2018-09-10 19:21:56.000000 pyActigraphy-1.2/LICENSE.md
--rw-r--r--   0 ghammad    (501) staff       (20)     6844 2023-03-22 10:47:00.000000 pyActigraphy-1.2/PKG-INFO
--rw-r--r--   0 ghammad    (501) staff       (20)     6200 2023-03-22 10:46:43.000000 pyActigraphy-1.2/README.rst
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/
--rw-r--r--   0 ghammad    (501) staff       (20)      844 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/__init__.py
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/analysis/
--rw-r--r--   0 ghammad    (501) staff       (20)      308 2023-01-27 15:19:01.000000 pyActigraphy-1.2/pyActigraphy/analysis/__init__.py
--rw-r--r--   0 ghammad    (501) staff       (20)     9295 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/analysis/cosinor.py
--rw-r--r--   0 ghammad    (501) staff       (20)    11135 2023-01-27 15:19:01.000000 pyActigraphy-1.2/pyActigraphy/analysis/flm.py
--rw-r--r--   0 ghammad    (501) staff       (20)    25930 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/analysis/fractal.py
--rw-r--r--   0 ghammad    (501) staff       (20)    25685 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/analysis/lids.py
--rw-r--r--   0 ghammad    (501) staff       (20)    12295 2023-01-27 15:19:01.000000 pyActigraphy-1.2/pyActigraphy/analysis/ssa.py
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/filters/
--rw-r--r--   0 ghammad    (501) staff       (20)      268 2023-01-19 10:23:14.000000 pyActigraphy-1.2/pyActigraphy/filters/__init__.py
--rw-r--r--   0 ghammad    (501) staff       (20)     5902 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/filters/filters.py
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/io/
--rw-r--r--   0 ghammad    (501) staff       (20)      783 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/io/__init__.py
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/io/agd/
--rw-r--r--   0 ghammad    (501) staff       (20)      209 2020-06-23 15:46:28.000000 pyActigraphy-1.2/pyActigraphy/io/agd/__init__.py
--rw-r--r--   0 ghammad    (501) staff       (20)     8185 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/io/agd/agd.py
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/io/atr/
--rw-r--r--   0 ghammad    (501) staff       (20)      213 2020-06-23 15:46:28.000000 pyActigraphy-1.2/pyActigraphy/io/atr/__init__.py
--rw-r--r--   0 ghammad    (501) staff       (20)     8652 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/io/atr/atr.py
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/io/awd/
--rw-r--r--   0 ghammad    (501) staff       (20)      208 2018-08-23 20:09:08.000000 pyActigraphy-1.2/pyActigraphy/io/awd/__init__.py
--rw-r--r--   0 ghammad    (501) staff       (20)     8960 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/io/awd/awd.py
--rw-r--r--   0 ghammad    (501) staff       (20)    15584 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/io/base.py
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/io/bba/
--rw-r--r--   0 ghammad    (501) staff       (20)      317 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/io/bba/__init__.py
--rw-r--r--   0 ghammad    (501) staff       (20)    11980 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/io/bba/bba.py
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/io/dqt/
--rw-r--r--   0 ghammad    (501) staff       (20)      208 2020-06-23 15:46:28.000000 pyActigraphy-1.2/pyActigraphy/io/dqt/__init__.py
--rw-r--r--   0 ghammad    (501) staff       (20)     6054 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/io/dqt/dqt.py
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/io/mesa/
--rw-r--r--   0 ghammad    (501) staff       (20)      210 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/io/mesa/__init__.py
--rw-r--r--   0 ghammad    (501) staff       (20)     7078 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/io/mesa/mesa.py
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/io/mtn/
--rw-r--r--   0 ghammad    (501) staff       (20)      203 2018-08-23 20:09:08.000000 pyActigraphy-1.2/pyActigraphy/io/mtn/__init__.py
--rw-r--r--   0 ghammad    (501) staff       (20)     8359 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/io/mtn/mtn.py
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/io/reader/
--rw-r--r--   0 ghammad    (501) staff       (20)      225 2019-01-11 12:54:58.000000 pyActigraphy-1.2/pyActigraphy/io/reader/__init__.py
--rw-r--r--   0 ghammad    (501) staff       (20)     9518 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/io/reader/reader.py
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/io/rpx/
--rw-r--r--   0 ghammad    (501) staff       (20)      216 2018-08-23 20:09:08.000000 pyActigraphy-1.2/pyActigraphy/io/rpx/__init__.py
--rw-r--r--   0 ghammad    (501) staff       (20)     3012 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/io/rpx/multilang.py
--rw-r--r--   0 ghammad    (501) staff       (20)    14667 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/io/rpx/rpx.py
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/io/tal/
--rw-r--r--   0 ghammad    (501) staff       (20)      216 2023-01-27 15:19:01.000000 pyActigraphy-1.2/pyActigraphy/io/tal/__init__.py
--rw-r--r--   0 ghammad    (501) staff       (20)     7246 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/io/tal/tal.py
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/light/
--rw-r--r--   0 ghammad    (501) staff       (20)     1679 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/light/__init__.py
--rw-r--r--   0 ghammad    (501) staff       (20)     8197 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/light/gendevice.py
--rw-r--r--   0 ghammad    (501) staff       (20)     7343 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/light/light.py
--rw-r--r--   0 ghammad    (501) staff       (20)    32514 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/light/light_metrics.py
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/log/
--rw-r--r--   0 ghammad    (501) staff       (20)      286 2020-06-23 15:46:28.000000 pyActigraphy-1.2/pyActigraphy/log/__init__.py
--rw-r--r--   0 ghammad    (501) staff       (20)     4932 2020-06-23 15:46:28.000000 pyActigraphy-1.2/pyActigraphy/log/baselog.py
--rw-r--r--   0 ghammad    (501) staff       (20)     1551 2020-06-23 15:46:28.000000 pyActigraphy-1.2/pyActigraphy/log/sstlog.py
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/mask/
--rw-r--r--   0 ghammad    (501) staff       (20)      264 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/mask/__init__.py
--rw-r--r--   0 ghammad    (501) staff       (20)     3061 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/mask/utils.py
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/metrics/
--rw-r--r--   0 ghammad    (501) staff       (20)      547 2020-01-24 13:51:54.000000 pyActigraphy-1.2/pyActigraphy/metrics/__init__.py
--rw-r--r--   0 ghammad    (501) staff       (20)    66633 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/metrics/metrics.py
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/recording/
--rw-r--r--   0 ghammad    (501) staff       (20)      204 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/recording/__init__.py
--rw-r--r--   0 ghammad    (501) staff       (20)     5605 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/recording/base.py
--rw-r--r--   0 ghammad    (501) staff       (20)     2466 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/recording/utils.py
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/reports/
--rw-r--r--   0 ghammad    (501) staff       (20)      437 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/reports/__init__.py
--rw-r--r--   0 ghammad    (501) staff       (20)      940 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/reports/report.py
--rw-r--r--   0 ghammad    (501) staff       (20)     5728 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/reports/report_activity.py
--rw-r--r--   0 ghammad    (501) staff       (20)     6361 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/reports/report_sleep.py
--rw-r--r--   0 ghammad    (501) staff       (20)     2472 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/reports/utils.py
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/sleep/
--rw-r--r--   0 ghammad    (501) staff       (20)      317 2020-11-18 15:26:23.000000 pyActigraphy-1.2/pyActigraphy/sleep/__init__.py
--rw-r--r--   0 ghammad    (501) staff       (20)     6502 2020-06-23 15:46:28.000000 pyActigraphy-1.2/pyActigraphy/sleep/diary.py
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/sleep/scoring/
--rw-r--r--   0 ghammad    (501) staff       (20)      349 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/sleep/scoring/__init__.py
--rw-r--r--   0 ghammad    (501) staff       (20)     5859 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/sleep/scoring/csm.py
--rw-r--r--   0 ghammad    (501) staff       (20)     7927 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/sleep/scoring/roenneberg.py
--rw-r--r--   0 ghammad    (501) staff       (20)     1719 2020-06-23 15:46:28.000000 pyActigraphy-1.2/pyActigraphy/sleep/scoring/smp.py
--rw-r--r--   0 ghammad    (501) staff       (20)     1529 2020-06-23 15:46:28.000000 pyActigraphy-1.2/pyActigraphy/sleep/scoring/sri.py
--rw-r--r--   0 ghammad    (501) staff       (20)     8611 2023-01-27 15:19:01.000000 pyActigraphy-1.2/pyActigraphy/sleep/scoring/utils.py
--rw-r--r--   0 ghammad    (501) staff       (20)    63797 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/sleep/scoring_base.py
--rw-r--r--   0 ghammad    (501) staff       (20)     6882 2020-06-23 15:46:28.000000 pyActigraphy-1.2/pyActigraphy/sleep/sleep.py
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/tests/
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/tests/data/
--rw-r--r--   0 ghammad    (501) staff       (20)    70203 2023-01-27 15:19:01.000000 pyActigraphy-1.2/pyActigraphy/tests/data/example_01.AWD
--rw-r--r--   0 ghammad    (501) staff       (20)    69295 2023-01-27 15:19:01.000000 pyActigraphy-1.2/pyActigraphy/tests/data/example_01_mask.AWD
--rw-r--r--   0 ghammad    (501) staff       (20)    32409 2020-01-24 13:51:54.000000 pyActigraphy-1.2/pyActigraphy/tests/data/example_01_sleepdiary.ods
--rw-r--r--   0 ghammad    (501) staff       (20)    32448 2020-01-24 13:51:54.000000 pyActigraphy-1.2/pyActigraphy/tests/data/example_01_sleepdiary_extra_states.ods
--rw-r--r--   0 ghammad    (501) staff       (20)    72128 2023-01-27 15:19:01.000000 pyActigraphy-1.2/pyActigraphy/tests/data/example_02.AWD
--rw-r--r--   0 ghammad    (501) staff       (20)    84789 2023-01-27 15:19:01.000000 pyActigraphy-1.2/pyActigraphy/tests/data/example_03.AWD
--rw-r--r--   0 ghammad    (501) staff       (20)   111010 2023-01-27 15:19:01.000000 pyActigraphy-1.2/pyActigraphy/tests/data/example_04.AWD
--rw-r--r--   0 ghammad    (501) staff       (20)    82232 2023-01-27 15:19:01.000000 pyActigraphy-1.2/pyActigraphy/tests/data/example_05.AWD
--rw-r--r--   0 ghammad    (501) staff       (20)      131 2020-06-23 15:46:28.000000 pyActigraphy-1.2/pyActigraphy/tests/data/example_masklog.csv
--rw-r--r--   0 ghammad    (501) staff       (20)      197 2020-06-23 15:46:28.000000 pyActigraphy-1.2/pyActigraphy/tests/data/example_sstlog.csv
--rw-r--r--   0 ghammad    (501) staff       (20)    13736 2019-08-27 20:51:04.000000 pyActigraphy-1.2/pyActigraphy/tests/data/example_sstlog.ods
--rw-r--r--   0 ghammad    (501) staff       (20)     8704 2020-06-23 15:46:28.000000 pyActigraphy-1.2/pyActigraphy/tests/data/example_sstlog.xls
--rw-r--r--   0 ghammad    (501) staff       (20)     6119 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/tests/data/example_sstlog.xlsx
--rw-r--r--   0 ghammad    (501) staff       (20)     1323 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/tests/data/sample-summary-no-calibration.json
--rw-r--r--   0 ghammad    (501) staff       (20)     1325 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/tests/data/sample-summary-wrong-name.json
--rw-r--r--   0 ghammad    (501) staff       (20)    40316 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/tests/data/sample-summary.json
--rw-r--r--   0 ghammad    (501) staff       (20)   114837 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/tests/data/sample-timeSeries.csv.gz
--rw-r--r--   0 ghammad    (501) staff       (20)    34502 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/tests/data/test_sample.AWD
--rw-r--r--   0 ghammad    (501) staff       (20)   303104 2020-06-23 15:46:28.000000 pyActigraphy-1.2/pyActigraphy/tests/data/test_sample.agd
--rw-r--r--   0 ghammad    (501) staff       (20)   954771 2019-01-11 12:54:58.000000 pyActigraphy-1.2/pyActigraphy/tests/data/test_sample.csv
--rw-r--r--   0 ghammad    (501) staff       (20)    42236 2018-08-23 21:31:00.000000 pyActigraphy-1.2/pyActigraphy/tests/data/test_sample.mtn
--rw-r--r--   0 ghammad    (501) staff       (20)   647206 2020-06-23 15:46:28.000000 pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_atr.txt
--rw-r--r--   0 ghammad    (501) staff       (20)   125506 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_aw4.AWD
--rw-r--r--   0 ghammad    (501) staff       (20)   326330 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_aw7.AWD
--rw-r--r--   0 ghammad    (501) staff       (20)    70507 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_awi.AWD
--rw-r--r--   0 ghammad    (501) staff       (20)   112554 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_awl.AWD
--rw-r--r--   0 ghammad    (501) staff       (20)   121254 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_awlp.AWD
--rw-r--r--   0 ghammad    (501) staff       (20)   106195 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_awmk2.AWD
--rw-r--r--   0 ghammad    (501) staff       (20)    17697 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_aws.AWD
--rw-r--r--   0 ghammad    (501) staff       (20)    45929 2023-03-22 10:46:43.000000 pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_awt.AWD
--rw-r--r--   0 ghammad    (501) staff       (20)  1129717 2020-06-23 15:46:28.000000 pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_dqt.csv
--rw-r--r--   0 ghammad    (501) staff       (20)      344 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_mesa.csv
--rw-r--r--   0 ghammad    (501) staff       (20)  1284380 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_rpx_eng.csv
--rw-r--r--   0 ghammad    (501) staff       (20)   954782 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_rpx_fr.csv
--rw-r--r--   0 ghammad    (501) staff       (20)  1197591 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_rpx_ger_no_light.csv
--rw-r--r--   0 ghammad    (501) staff       (20)  1653023 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_rpx_ger_with_light.csv
--rw-r--r--   0 ghammad    (501) staff       (20)   317518 2023-01-27 15:19:01.000000 pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_tal.txt
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/utils/
--rw-r--r--   0 ghammad    (501) staff       (20)      497 2020-06-23 15:46:28.000000 pyActigraphy-1.2/pyActigraphy/utils/__init__.py
--rw-r--r--   0 ghammad    (501) staff       (20)      483 2020-06-23 15:46:28.000000 pyActigraphy-1.2/pyActigraphy/utils/filters.py
--rw-r--r--   0 ghammad    (501) staff       (20)     1568 2020-06-23 15:46:28.000000 pyActigraphy-1.2/pyActigraphy/utils/utils.py
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy/viz/
--rw-r--r--   0 ghammad    (501) staff       (20)      279 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/viz/__init__.py
--rw-r--r--   0 ghammad    (501) staff       (20)    12816 2023-03-15 17:04:54.000000 pyActigraphy-1.2/pyActigraphy/viz/viz.py
-drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy.egg-info/
--rw-r--r--   0 ghammad    (501) staff       (20)     6844 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy.egg-info/PKG-INFO
--rw-r--r--   0 ghammad    (501) staff       (20)     3972 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy.egg-info/SOURCES.txt
--rw-r--r--   0 ghammad    (501) staff       (20)        1 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy.egg-info/dependency_links.txt
--rw-r--r--   0 ghammad    (501) staff       (20)        1 2018-08-23 20:15:13.000000 pyActigraphy-1.2/pyActigraphy.egg-info/not-zip-safe
--rw-r--r--   0 ghammad    (501) staff       (20)      142 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy.egg-info/requires.txt
--rw-r--r--   0 ghammad    (501) staff       (20)       13 2023-03-22 10:47:00.000000 pyActigraphy-1.2/pyActigraphy.egg-info/top_level.txt
--rw-r--r--   0 ghammad    (501) staff       (20)       38 2023-03-22 10:47:00.000000 pyActigraphy-1.2/setup.cfg
--rw-r--r--   0 ghammad    (501) staff       (20)     4566 2023-03-22 10:46:43.000000 pyActigraphy-1.2/setup.py
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/
+-rw-r--r--   0 ghammad    (501) staff       (20)    34728 2018-09-10 19:21:56.000000 pyActigraphy-1.2.1/LICENSE.md
+-rw-r--r--   0 ghammad    (501) staff       (20)     6846 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/PKG-INFO
+-rw-r--r--   0 ghammad    (501) staff       (20)     6200 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/README.rst
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/
+-rw-r--r--   0 ghammad    (501) staff       (20)      846 2023-04-27 13:22:16.000000 pyActigraphy-1.2.1/pyActigraphy/__init__.py
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/analysis/
+-rw-r--r--   0 ghammad    (501) staff       (20)      308 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/analysis/__init__.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     9295 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/analysis/cosinor.py
+-rw-r--r--   0 ghammad    (501) staff       (20)    11135 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/analysis/flm.py
+-rw-r--r--   0 ghammad    (501) staff       (20)    25930 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/analysis/fractal.py
+-rw-r--r--   0 ghammad    (501) staff       (20)    25685 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/analysis/lids.py
+-rw-r--r--   0 ghammad    (501) staff       (20)    12295 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/analysis/ssa.py
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/filters/
+-rw-r--r--   0 ghammad    (501) staff       (20)      268 2023-01-19 10:23:14.000000 pyActigraphy-1.2.1/pyActigraphy/filters/__init__.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     5902 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/filters/filters.py
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/io/
+-rw-r--r--   0 ghammad    (501) staff       (20)      783 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/io/__init__.py
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/io/agd/
+-rw-r--r--   0 ghammad    (501) staff       (20)      209 2020-06-23 15:46:28.000000 pyActigraphy-1.2.1/pyActigraphy/io/agd/__init__.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     8185 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/io/agd/agd.py
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/io/atr/
+-rw-r--r--   0 ghammad    (501) staff       (20)      213 2020-06-23 15:46:28.000000 pyActigraphy-1.2.1/pyActigraphy/io/atr/__init__.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     8652 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/io/atr/atr.py
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/io/awd/
+-rw-r--r--   0 ghammad    (501) staff       (20)      208 2018-08-23 20:09:08.000000 pyActigraphy-1.2.1/pyActigraphy/io/awd/__init__.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     8968 2023-04-27 13:22:16.000000 pyActigraphy-1.2.1/pyActigraphy/io/awd/awd.py
+-rw-r--r--   0 ghammad    (501) staff       (20)    15584 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/io/base.py
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/io/bba/
+-rw-r--r--   0 ghammad    (501) staff       (20)      317 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/io/bba/__init__.py
+-rw-r--r--   0 ghammad    (501) staff       (20)    11998 2023-04-27 13:22:16.000000 pyActigraphy-1.2.1/pyActigraphy/io/bba/bba.py
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/io/dqt/
+-rw-r--r--   0 ghammad    (501) staff       (20)      208 2020-06-23 15:46:28.000000 pyActigraphy-1.2.1/pyActigraphy/io/dqt/__init__.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     6054 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/io/dqt/dqt.py
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/io/mesa/
+-rw-r--r--   0 ghammad    (501) staff       (20)      210 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/io/mesa/__init__.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     7078 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/io/mesa/mesa.py
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/io/mtn/
+-rw-r--r--   0 ghammad    (501) staff       (20)      203 2018-08-23 20:09:08.000000 pyActigraphy-1.2.1/pyActigraphy/io/mtn/__init__.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     8359 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/io/mtn/mtn.py
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/io/reader/
+-rw-r--r--   0 ghammad    (501) staff       (20)      225 2019-01-11 12:54:58.000000 pyActigraphy-1.2.1/pyActigraphy/io/reader/__init__.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     9947 2023-04-27 13:22:16.000000 pyActigraphy-1.2.1/pyActigraphy/io/reader/reader.py
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/io/rpx/
+-rw-r--r--   0 ghammad    (501) staff       (20)      216 2018-08-23 20:09:08.000000 pyActigraphy-1.2.1/pyActigraphy/io/rpx/__init__.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     3012 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/io/rpx/multilang.py
+-rw-r--r--   0 ghammad    (501) staff       (20)    14667 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/io/rpx/rpx.py
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/io/tal/
+-rw-r--r--   0 ghammad    (501) staff       (20)      216 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/io/tal/__init__.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     7246 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/io/tal/tal.py
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/light/
+-rw-r--r--   0 ghammad    (501) staff       (20)     1679 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/light/__init__.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     8197 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/light/gendevice.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     7343 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/light/light.py
+-rw-r--r--   0 ghammad    (501) staff       (20)    32514 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/light/light_metrics.py
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/log/
+-rw-r--r--   0 ghammad    (501) staff       (20)      286 2020-06-23 15:46:28.000000 pyActigraphy-1.2.1/pyActigraphy/log/__init__.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     4932 2020-06-23 15:46:28.000000 pyActigraphy-1.2.1/pyActigraphy/log/baselog.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     1551 2020-06-23 15:46:28.000000 pyActigraphy-1.2.1/pyActigraphy/log/sstlog.py
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/mask/
+-rw-r--r--   0 ghammad    (501) staff       (20)      264 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/mask/__init__.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     3061 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/mask/utils.py
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/metrics/
+-rw-r--r--   0 ghammad    (501) staff       (20)      547 2020-01-24 13:51:54.000000 pyActigraphy-1.2.1/pyActigraphy/metrics/__init__.py
+-rw-r--r--   0 ghammad    (501) staff       (20)    66633 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/metrics/metrics.py
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/recording/
+-rw-r--r--   0 ghammad    (501) staff       (20)      204 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/recording/__init__.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     5605 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/recording/base.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     2466 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/recording/utils.py
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/reports/
+-rw-r--r--   0 ghammad    (501) staff       (20)      437 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/reports/__init__.py
+-rw-r--r--   0 ghammad    (501) staff       (20)      940 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/reports/report.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     5728 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/reports/report_activity.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     6361 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/reports/report_sleep.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     2472 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/reports/utils.py
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/sleep/
+-rw-r--r--   0 ghammad    (501) staff       (20)      317 2020-11-18 15:26:23.000000 pyActigraphy-1.2.1/pyActigraphy/sleep/__init__.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     6502 2020-06-23 15:46:28.000000 pyActigraphy-1.2.1/pyActigraphy/sleep/diary.py
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/sleep/scoring/
+-rw-r--r--   0 ghammad    (501) staff       (20)      349 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/sleep/scoring/__init__.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     5859 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/sleep/scoring/csm.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     7927 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/sleep/scoring/roenneberg.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     1719 2020-06-23 15:46:28.000000 pyActigraphy-1.2.1/pyActigraphy/sleep/scoring/smp.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     1529 2020-06-23 15:46:28.000000 pyActigraphy-1.2.1/pyActigraphy/sleep/scoring/sri.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     8611 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/sleep/scoring/utils.py
+-rw-r--r--   0 ghammad    (501) staff       (20)    63797 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/sleep/scoring_base.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     6882 2020-06-23 15:46:28.000000 pyActigraphy-1.2.1/pyActigraphy/sleep/sleep.py
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/tests/
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/
+-rw-r--r--   0 ghammad    (501) staff       (20)    70203 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/example_01.AWD
+-rw-r--r--   0 ghammad    (501) staff       (20)    69295 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/example_01_mask.AWD
+-rw-r--r--   0 ghammad    (501) staff       (20)    32409 2020-01-24 13:51:54.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/example_01_sleepdiary.ods
+-rw-r--r--   0 ghammad    (501) staff       (20)    32448 2020-01-24 13:51:54.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/example_01_sleepdiary_extra_states.ods
+-rw-r--r--   0 ghammad    (501) staff       (20)    72128 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/example_02.AWD
+-rw-r--r--   0 ghammad    (501) staff       (20)    84789 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/example_03.AWD
+-rw-r--r--   0 ghammad    (501) staff       (20)   111010 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/example_04.AWD
+-rw-r--r--   0 ghammad    (501) staff       (20)    82232 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/example_05.AWD
+-rw-r--r--   0 ghammad    (501) staff       (20)      131 2020-06-23 15:46:28.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/example_masklog.csv
+-rw-r--r--   0 ghammad    (501) staff       (20)      197 2020-06-23 15:46:28.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/example_sstlog.csv
+-rw-r--r--   0 ghammad    (501) staff       (20)    13736 2019-08-27 20:51:04.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/example_sstlog.ods
+-rw-r--r--   0 ghammad    (501) staff       (20)     8704 2020-06-23 15:46:28.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/example_sstlog.xls
+-rw-r--r--   0 ghammad    (501) staff       (20)     6119 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/example_sstlog.xlsx
+-rw-r--r--   0 ghammad    (501) staff       (20)     1323 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/sample-summary-no-calibration.json
+-rw-r--r--   0 ghammad    (501) staff       (20)     1325 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/sample-summary-wrong-name.json
+-rw-r--r--   0 ghammad    (501) staff       (20)    40316 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/sample-summary.json
+-rw-r--r--   0 ghammad    (501) staff       (20)   114837 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/sample-timeSeries.csv.gz
+-rw-r--r--   0 ghammad    (501) staff       (20)    34502 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample.AWD
+-rw-r--r--   0 ghammad    (501) staff       (20)   303104 2020-06-23 15:46:28.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample.agd
+-rw-r--r--   0 ghammad    (501) staff       (20)   954771 2019-01-11 12:54:58.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample.csv
+-rw-r--r--   0 ghammad    (501) staff       (20)    42236 2018-08-23 21:31:00.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample.mtn
+-rw-r--r--   0 ghammad    (501) staff       (20)   647206 2020-06-23 15:46:28.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_atr.txt
+-rw-r--r--   0 ghammad    (501) staff       (20)   125506 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_aw4.AWD
+-rw-r--r--   0 ghammad    (501) staff       (20)   326330 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_aw7.AWD
+-rw-r--r--   0 ghammad    (501) staff       (20)    70507 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_awi.AWD
+-rw-r--r--   0 ghammad    (501) staff       (20)   112554 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_awl.AWD
+-rw-r--r--   0 ghammad    (501) staff       (20)   121254 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_awlp.AWD
+-rw-r--r--   0 ghammad    (501) staff       (20)   106195 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_awmk2.AWD
+-rw-r--r--   0 ghammad    (501) staff       (20)    17697 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_aws.AWD
+-rw-r--r--   0 ghammad    (501) staff       (20)    45929 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_awt.AWD
+-rw-r--r--   0 ghammad    (501) staff       (20)  1129717 2020-06-23 15:46:28.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_dqt.csv
+-rw-r--r--   0 ghammad    (501) staff       (20)      344 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_mesa.csv
+-rw-r--r--   0 ghammad    (501) staff       (20)  1284380 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_rpx_eng.csv
+-rw-r--r--   0 ghammad    (501) staff       (20)   954782 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_rpx_fr.csv
+-rw-r--r--   0 ghammad    (501) staff       (20)  1197591 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_rpx_ger_no_light.csv
+-rw-r--r--   0 ghammad    (501) staff       (20)  1653023 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_rpx_ger_with_light.csv
+-rw-r--r--   0 ghammad    (501) staff       (20)   317518 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_tal.txt
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/utils/
+-rw-r--r--   0 ghammad    (501) staff       (20)      497 2020-06-23 15:46:28.000000 pyActigraphy-1.2.1/pyActigraphy/utils/__init__.py
+-rw-r--r--   0 ghammad    (501) staff       (20)      483 2020-06-23 15:46:28.000000 pyActigraphy-1.2.1/pyActigraphy/utils/filters.py
+-rw-r--r--   0 ghammad    (501) staff       (20)     1568 2020-06-23 15:46:28.000000 pyActigraphy-1.2.1/pyActigraphy/utils/utils.py
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy/viz/
+-rw-r--r--   0 ghammad    (501) staff       (20)      279 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/viz/__init__.py
+-rw-r--r--   0 ghammad    (501) staff       (20)    12816 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/pyActigraphy/viz/viz.py
+drwxr-xr-x   0 ghammad    (501) staff       (20)        0 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy.egg-info/
+-rw-r--r--   0 ghammad    (501) staff       (20)     6846 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy.egg-info/PKG-INFO
+-rw-r--r--   0 ghammad    (501) staff       (20)     3972 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy.egg-info/SOURCES.txt
+-rw-r--r--   0 ghammad    (501) staff       (20)        1 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy.egg-info/dependency_links.txt
+-rw-r--r--   0 ghammad    (501) staff       (20)        1 2018-08-23 20:15:13.000000 pyActigraphy-1.2.1/pyActigraphy.egg-info/not-zip-safe
+-rw-r--r--   0 ghammad    (501) staff       (20)      142 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy.egg-info/requires.txt
+-rw-r--r--   0 ghammad    (501) staff       (20)       13 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/pyActigraphy.egg-info/top_level.txt
+-rw-r--r--   0 ghammad    (501) staff       (20)       38 2023-04-28 08:52:41.000000 pyActigraphy-1.2.1/setup.cfg
+-rw-r--r--   0 ghammad    (501) staff       (20)     4566 2023-04-03 07:55:43.000000 pyActigraphy-1.2.1/setup.py
```

### Comparing `pyActigraphy-1.2/LICENSE.md` & `pyActigraphy-1.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/PKG-INFO` & `pyActigraphy-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyActigraphy
-Version: 1.2
+Version: 1.2.1
 Summary: Analysis package for actigraphy data
 Home-page: https://github.com/ghammad/pyActigraphy
 Author: Grégory Hammad
 Author-email: gregory.hammad@hotmail.fr
 License: GNU GPL-3.0
 Keywords: actigraphy actimetry analysis python open-source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyActigraphy-1.2/README.rst` & `pyActigraphy-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/__init__.py` & `pyActigraphy-1.2.1/pyActigraphy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,8 +37,8 @@
     "reports",
     "sleep",
     "tests",
     "utils",
     "viz"
 ]
 
-__version__ = '1.2'
+__version__ = '1.2.1'
```

### Comparing `pyActigraphy-1.2/pyActigraphy/analysis/cosinor.py` & `pyActigraphy-1.2.1/pyActigraphy/analysis/cosinor.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/analysis/flm.py` & `pyActigraphy-1.2.1/pyActigraphy/analysis/flm.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/analysis/fractal.py` & `pyActigraphy-1.2.1/pyActigraphy/analysis/fractal.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/analysis/lids.py` & `pyActigraphy-1.2.1/pyActigraphy/analysis/lids.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/analysis/ssa.py` & `pyActigraphy-1.2.1/pyActigraphy/analysis/ssa.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/filters/filters.py` & `pyActigraphy-1.2.1/pyActigraphy/filters/filters.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/io/__init__.py` & `pyActigraphy-1.2.1/pyActigraphy/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/io/agd/agd.py` & `pyActigraphy-1.2.1/pyActigraphy/io/agd/agd.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/io/atr/atr.py` & `pyActigraphy-1.2.1/pyActigraphy/io/atr/atr.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/io/awd/awd.py` & `pyActigraphy-1.2.1/pyActigraphy/io/awd/awd.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
         # extract model from UUID:
         wrn_msg = (
             'Only the first data column will be used, assuming it corresponds '
             'to activity counts.'
         )
         match = re.match(pattern=r'^([A-Za-z])[0-9a-fA-F]+', string=uuid)
         if match:  # check if UUID matches the expected pattern
-            dcode = match.groups()[0]
+            dcode = match.groups()[0].upper()
             if dcode in RawAWD.device_code.keys():
                 return dcode
             else:
                 warnings.warn(
                     'The model specified in the UUID ({})'.format(dcode)
                     + ' is not supported at the moment.\n'
                     + 'List of supported Actiwatch models:\n'
```

### Comparing `pyActigraphy-1.2/pyActigraphy/io/base.py` & `pyActigraphy-1.2.1/pyActigraphy/io/base.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/io/bba/bba.py` & `pyActigraphy-1.2.1/pyActigraphy/io/bba/bba.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,28 +270,28 @@
             meta_data = json.load(file)
 
         # check filename consistency:
         # - META-DATA: file-name = 'basename'.cwa[.gz]
         # - INPUT DATA: input_fname = 'basename'-timeSeries.csv[.gz]
 
         match_basename = re.match(
-            pattern=r'^(\w*)-timeSeries.csv(\.gz)?',
+            pattern=r'^(.+?)-timeSeries.csv(\.gz)?',
             string=os.path.basename(input_fname)
         )
         if match_basename:
             input_basename = match_basename.groups()[0]
         else:
             raise ValueError(
                 'Could extract file basename (XXX-timeSeries.csv.gz)'
                 + ' from input filename: {}'.format(input_fname)
             )
 
         if not re.match(
             pattern=r'{}.(cwa|CWA)(\.gz)?'.format(input_basename),
-            string=meta_data['file-name']
+            string=os.path.basename(meta_data['file-name'])
         ):
             raise ValueError(
                 'Attempting to read a metadata file referring to another '
                 + 'input file.\n'
                 + '- Input file: {}\n'.format(os.path.basename(input_fname))
                 + '- Extracted basename: {}\n'.format(input_basename)
                 + '- Metadata ref: {}\n'.format(
```

### Comparing `pyActigraphy-1.2/pyActigraphy/io/dqt/dqt.py` & `pyActigraphy-1.2.1/pyActigraphy/io/dqt/dqt.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/io/mesa/mesa.py` & `pyActigraphy-1.2.1/pyActigraphy/io/mesa/mesa.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/io/mtn/mtn.py` & `pyActigraphy-1.2.1/pyActigraphy/io/mtn/mtn.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/io/reader/reader.py` & `pyActigraphy-1.2.1/pyActigraphy/io/reader/reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 from pandas import Timedelta
 from pandas.tseries.frequencies import to_offset
 from pyActigraphy.metrics import ForwardMetricsMixin
 from joblib import Parallel, delayed
 from ..agd import read_raw_agd
 from ..atr import read_raw_atr
 from ..awd import read_raw_awd
+from ..bba import read_raw_bba
 from ..dqt import read_raw_dqt
+from ..mesa import read_raw_mesa
 from ..mtn import read_raw_mtn
 from ..rpx import read_raw_rpx
 from ..tal import read_raw_tal
 from pyActigraphy.log import read_sst_log
 
 
 class RawReader(ForwardMetricsMixin):
@@ -227,16 +229,18 @@
         E.g. '/path/to/my/files/*.csv'
     reader_type: str
         Reader type.
         Supported types:
 
         * AGD ((w)GT3X(+)), ActiGraph)
         * ATR (ActTrust, Condor Instruments)
-        * AWD (ActiWatch 4, CamNtech)
+        * AWD (ActiWatch 4/7/L/L-Plus/T, CamNtech)
+        * BBA (Biobankaccelerometer)
         * DQT (Daqtometers, Daqtix)
+        * MESA (MESA dataset, NSRR)
         * MTN (MotionWatch8, CamNtech)
         * RPX (Actiwatch, Respironics)
         * TAL (Tempatilumi, CE Brasil)
 
     n_jobs: int
         Number of CPU to use for parallel reading
     prefer: str
@@ -253,15 +257,17 @@
 
     Returns
     -------
     raw : Instance of RawReader
         An object containing raw data
     """
 
-    supported_types = ['AGD', 'ATR', 'AWD', 'DQT', 'MTN', 'RPX', 'TAL']
+    supported_types = [
+        'AGD', 'ATR', 'AWD', 'BBA', 'DQT', 'MESA', 'MTN', 'RPX', 'TAL'
+    ]
     if reader_type not in supported_types:
         raise ValueError(
             'Type {0} unsupported. Supported types: {1}'.format(
                 reader_type, supported_types
             )
         )
 
@@ -280,17 +286,23 @@
         ),
         'ATR': lambda files: parallel_reader(
             n_jobs, read_raw_atr, files, prefer, verbose, **kwargs
         ),
         'AWD': lambda files: parallel_reader(
             n_jobs, read_raw_awd, files, prefer, verbose, **kwargs
         ),
+        'BBA': lambda files: parallel_reader(
+            n_jobs, read_raw_bba, files, prefer, verbose, **kwargs
+        ),
         'DQT': lambda files: parallel_reader(
             n_jobs, read_raw_dqt, files, prefer, verbose, **kwargs
         ),
+        'MESA': lambda files: parallel_reader(
+            n_jobs, read_raw_mesa, files, prefer, verbose, **kwargs
+        ),
         'MTN': lambda files: parallel_reader(
             n_jobs, read_raw_mtn, files, prefer, verbose, **kwargs
         ),
         'RPX': lambda files: parallel_reader(
             n_jobs, read_raw_rpx, files, prefer, verbose, **kwargs
         ),
         'TAL': lambda files: parallel_reader(
```

### Comparing `pyActigraphy-1.2/pyActigraphy/io/rpx/multilang.py` & `pyActigraphy-1.2.1/pyActigraphy/io/rpx/multilang.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/io/rpx/rpx.py` & `pyActigraphy-1.2.1/pyActigraphy/io/rpx/rpx.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/io/tal/tal.py` & `pyActigraphy-1.2.1/pyActigraphy/io/tal/tal.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/light/__init__.py` & `pyActigraphy-1.2.1/pyActigraphy/light/__init__.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/light/gendevice.py` & `pyActigraphy-1.2.1/pyActigraphy/light/gendevice.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/light/light.py` & `pyActigraphy-1.2.1/pyActigraphy/light/light.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/light/light_metrics.py` & `pyActigraphy-1.2.1/pyActigraphy/light/light_metrics.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/log/baselog.py` & `pyActigraphy-1.2.1/pyActigraphy/log/baselog.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/log/sstlog.py` & `pyActigraphy-1.2.1/pyActigraphy/log/sstlog.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/mask/utils.py` & `pyActigraphy-1.2.1/pyActigraphy/mask/utils.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/metrics/__init__.py` & `pyActigraphy-1.2.1/pyActigraphy/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/metrics/metrics.py` & `pyActigraphy-1.2.1/pyActigraphy/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/recording/base.py` & `pyActigraphy-1.2.1/pyActigraphy/recording/base.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/recording/utils.py` & `pyActigraphy-1.2.1/pyActigraphy/recording/utils.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/reports/report.py` & `pyActigraphy-1.2.1/pyActigraphy/reports/report.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/reports/report_activity.py` & `pyActigraphy-1.2.1/pyActigraphy/reports/report_activity.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/reports/report_sleep.py` & `pyActigraphy-1.2.1/pyActigraphy/reports/report_sleep.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/reports/utils.py` & `pyActigraphy-1.2.1/pyActigraphy/reports/utils.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/sleep/diary.py` & `pyActigraphy-1.2.1/pyActigraphy/sleep/diary.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/sleep/scoring/csm.py` & `pyActigraphy-1.2.1/pyActigraphy/sleep/scoring/csm.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/sleep/scoring/roenneberg.py` & `pyActigraphy-1.2.1/pyActigraphy/sleep/scoring/roenneberg.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/sleep/scoring/smp.py` & `pyActigraphy-1.2.1/pyActigraphy/sleep/scoring/smp.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/sleep/scoring/sri.py` & `pyActigraphy-1.2.1/pyActigraphy/sleep/scoring/sri.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/sleep/scoring/utils.py` & `pyActigraphy-1.2.1/pyActigraphy/sleep/scoring/utils.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/sleep/scoring_base.py` & `pyActigraphy-1.2.1/pyActigraphy/sleep/scoring_base.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/sleep/sleep.py` & `pyActigraphy-1.2.1/pyActigraphy/sleep/sleep.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/example_01.AWD` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/example_01.AWD`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/example_01_mask.AWD` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/example_01_mask.AWD`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/example_01_sleepdiary.ods` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/example_01_sleepdiary.ods`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/example_01_sleepdiary_extra_states.ods` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/example_01_sleepdiary_extra_states.ods`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/example_02.AWD` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/example_02.AWD`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/example_03.AWD` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/example_03.AWD`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/example_04.AWD` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/example_04.AWD`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/example_05.AWD` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/example_05.AWD`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/example_sstlog.ods` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/example_sstlog.ods`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/example_sstlog.xls` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/example_sstlog.xls`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/example_sstlog.xlsx` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/example_sstlog.xlsx`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/sample-summary-no-calibration.json` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/sample-summary-no-calibration.json`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/sample-summary-wrong-name.json` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/sample-summary-wrong-name.json`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/sample-summary.json` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/sample-summary.json`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/sample-timeSeries.csv.gz` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/sample-timeSeries.csv.gz`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/test_sample.AWD` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample.AWD`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/test_sample.agd` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample.agd`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/test_sample.csv` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample.csv`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/test_sample.mtn` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample.mtn`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_atr.txt` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_atr.txt`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_aw4.AWD` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_aw4.AWD`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_aw7.AWD` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_aw7.AWD`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_awi.AWD` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_awi.AWD`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_awl.AWD` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_awl.AWD`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_awlp.AWD` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_awlp.AWD`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_awmk2.AWD` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_awmk2.AWD`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_aws.AWD` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_aws.AWD`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_awt.AWD` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_awt.AWD`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_dqt.csv` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_dqt.csv`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_rpx_eng.csv` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_rpx_eng.csv`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_rpx_fr.csv` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_rpx_fr.csv`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_rpx_ger_no_light.csv` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_rpx_ger_no_light.csv`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_rpx_ger_with_light.csv` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_rpx_ger_with_light.csv`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/tests/data/test_sample_tal.txt` & `pyActigraphy-1.2.1/pyActigraphy/tests/data/test_sample_tal.txt`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/utils/utils.py` & `pyActigraphy-1.2.1/pyActigraphy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy/viz/viz.py` & `pyActigraphy-1.2.1/pyActigraphy/viz/viz.py`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/pyActigraphy.egg-info/PKG-INFO` & `pyActigraphy-1.2.1/pyActigraphy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyActigraphy
-Version: 1.2
+Version: 1.2.1
 Summary: Analysis package for actigraphy data
 Home-page: https://github.com/ghammad/pyActigraphy
 Author: Grégory Hammad
 Author-email: gregory.hammad@hotmail.fr
 License: GNU GPL-3.0
 Keywords: actigraphy actimetry analysis python open-source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyActigraphy-1.2/pyActigraphy.egg-info/SOURCES.txt` & `pyActigraphy-1.2.1/pyActigraphy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyActigraphy-1.2/setup.py` & `pyActigraphy-1.2.1/setup.py`

 * *Files identical despite different names*

